# Comparing `tmp/NbRisk-35.0.0.tar.gz` & `tmp/NbRisk-35.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NbRisk-35.0.0.tar", last modified: Wed May 10 14:31:10 2023, max compression
+gzip compressed data, was "NbRisk-35.0.1.tar", last modified: Thu May 11 23:04:26 2023, max compression
```

## Comparing `NbRisk-35.0.0.tar` & `NbRisk-35.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.175196 NbRisk-35.0.0/
--rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-35.0.0/LICENSE
--rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-35.0.0/MANIFEST.in
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.167196 NbRisk-35.0.0/NbRisk.egg-info/
--rw-rw-r--   0 renato    (1000) renato    (1000)     3011 2023-05-10 14:31:10.000000 NbRisk-35.0.0/NbRisk.egg-info/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     1526 2023-05-10 14:31:10.000000 NbRisk-35.0.0/NbRisk.egg-info/SOURCES.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-05-10 14:31:10.000000 NbRisk-35.0.0/NbRisk.egg-info/dependency_links.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        8 2023-05-10 14:31:10.000000 NbRisk-35.0.0/NbRisk.egg-info/top_level.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)     3011 2023-05-10 14:31:10.175196 NbRisk-35.0.0/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     2582 2023-04-21 03:01:56.000000 NbRisk-35.0.0/README.md
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.171196 NbRisk-35.0.0/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)      662 2023-04-02 19:37:23.000000 NbRisk-35.0.0/nb_risk/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-35.0.0/nb_risk/admin.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.171196 NbRisk-35.0.0/nb_risk/api/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.0/nb_risk/api/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      988 2023-04-21 01:31:32.000000 NbRisk-35.0.0/nb_risk/api/nested_serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     5107 2023-05-10 14:09:32.000000 NbRisk-35.0.0/nb_risk/api/serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 NbRisk-35.0.0/nb_risk/api/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 NbRisk-35.0.0/nb_risk/api/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 NbRisk-35.0.0/nb_risk/choices.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2023-04-25 01:55:31.000000 NbRisk-35.0.0/nb_risk/columns.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3295 2023-04-25 01:50:42.000000 NbRisk-35.0.0/nb_risk/cve.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1633 2023-04-21 01:17:07.000000 NbRisk-35.0.0/nb_risk/filters.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4997 2023-05-10 14:08:50.000000 NbRisk-35.0.0/nb_risk/forms.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.0/nb_risk/middleware.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.171196 NbRisk-35.0.0/nb_risk/migrations/
--rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-35.0.0/nb_risk/migrations/0001_initial.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 NbRisk-35.0.0/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 NbRisk-35.0.0/nb_risk/migrations/0003_control.py
--rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 NbRisk-35.0.0/nb_risk/migrations/0004_alter_vulnerability_options.py
--rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-35.0.0/nb_risk/migrations/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     8511 2023-05-10 12:47:27.000000 NbRisk-35.0.0/nb_risk/models.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4078 2023-05-10 13:19:51.000000 NbRisk-35.0.0/nb_risk/navigation.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.0/nb_risk/signals.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3428 2023-05-10 13:24:07.000000 NbRisk-35.0.0/nb_risk/tables.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      770 2023-04-02 19:37:24.000000 NbRisk-35.0.0/nb_risk/template_content.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.167196 NbRisk-35.0.0/nb_risk/templates/
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.175196 NbRisk-35.0.0/nb_risk/templates/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)     2236 2023-05-10 14:28:34.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/control.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1272 2023-05-10 14:28:23.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/control_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1272 2023-05-10 14:28:29.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/control_risks.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/generic_vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/risk.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2604 2023-05-10 14:28:43.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/threatevent.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      898 2023-05-10 14:28:39.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/threatsource.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     3216 2023-05-10 14:28:51.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      996 2023-05-10 14:28:47.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability_search.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     5961 2023-05-10 13:18:51.000000 NbRisk-35.0.0/nb_risk/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       23 2023-05-10 13:48:53.000000 NbRisk-35.0.0/nb_risk/version.py
--rw-rw-r--   0 renato    (1000) renato    (1000)    10306 2023-05-10 14:21:42.000000 NbRisk-35.0.0/nb_risk/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       38 2023-05-10 14:31:10.175196 NbRisk-35.0.0/setup.cfg
--rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-35.0.0/setup.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:26.039620 NbRisk-35.0.1/
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-35.0.1/LICENSE
+-rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-35.0.1/MANIFEST.in
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:25.943619 NbRisk-35.0.1/NbRisk.egg-info/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3127 2023-05-11 23:04:25.000000 NbRisk-35.0.1/NbRisk.egg-info/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1526 2023-05-11 23:04:25.000000 NbRisk-35.0.1/NbRisk.egg-info/SOURCES.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-05-11 23:04:25.000000 NbRisk-35.0.1/NbRisk.egg-info/dependency_links.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        8 2023-05-11 23:04:25.000000 NbRisk-35.0.1/NbRisk.egg-info/top_level.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3127 2023-05-11 23:04:26.035620 NbRisk-35.0.1/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2698 2023-05-11 21:21:40.000000 NbRisk-35.0.1/README.md
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:25.967619 NbRisk-35.0.1/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)      662 2023-04-02 19:37:23.000000 NbRisk-35.0.1/nb_risk/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-35.0.1/nb_risk/admin.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:25.975619 NbRisk-35.0.1/nb_risk/api/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.1/nb_risk/api/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      988 2023-04-21 01:31:32.000000 NbRisk-35.0.1/nb_risk/api/nested_serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5107 2023-05-10 14:35:17.000000 NbRisk-35.0.1/nb_risk/api/serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 NbRisk-35.0.1/nb_risk/api/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 NbRisk-35.0.1/nb_risk/api/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 NbRisk-35.0.1/nb_risk/choices.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2023-04-25 01:55:31.000000 NbRisk-35.0.1/nb_risk/columns.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3295 2023-04-25 01:50:42.000000 NbRisk-35.0.1/nb_risk/cve.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1633 2023-04-21 01:17:07.000000 NbRisk-35.0.1/nb_risk/filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4997 2023-05-10 14:35:17.000000 NbRisk-35.0.1/nb_risk/forms.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.1/nb_risk/middleware.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:25.983619 NbRisk-35.0.1/nb_risk/migrations/
+-rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-35.0.1/nb_risk/migrations/0001_initial.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 NbRisk-35.0.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 NbRisk-35.0.1/nb_risk/migrations/0003_control.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 NbRisk-35.0.1/nb_risk/migrations/0004_alter_vulnerability_options.py
+-rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-35.0.1/nb_risk/migrations/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     8511 2023-05-10 12:47:27.000000 NbRisk-35.0.1/nb_risk/models.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4078 2023-05-10 13:19:51.000000 NbRisk-35.0.1/nb_risk/navigation.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.1/nb_risk/signals.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3428 2023-05-10 13:24:07.000000 NbRisk-35.0.1/nb_risk/tables.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      770 2023-04-02 19:37:24.000000 NbRisk-35.0.1/nb_risk/template_content.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:25.931619 NbRisk-35.0.1/nb_risk/templates/
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:26.015620 NbRisk-35.0.1/nb_risk/templates/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1199 2023-05-11 22:46:19.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/control.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-11 22:46:32.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/control_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-11 22:46:26.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/control_risks.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/generic_vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/risk.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1939 2023-05-11 22:33:43.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/threatevent.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-11 22:34:00.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/threatsource.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2455 2023-05-11 21:46:58.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-11 21:46:54.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability_search.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4982 2023-05-11 23:00:59.000000 NbRisk-35.0.1/nb_risk/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       23 2023-05-11 22:48:14.000000 NbRisk-35.0.1/nb_risk/version.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10228 2023-05-11 22:45:54.000000 NbRisk-35.0.1/nb_risk/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       38 2023-05-11 23:04:26.039620 NbRisk-35.0.1/setup.cfg
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-35.0.1/setup.py
```

### Comparing `NbRisk-35.0.0/LICENSE` & `NbRisk-35.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/NbRisk.egg-info/PKG-INFO` & `NbRisk-35.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-Metadata-Version: 2.1
-Name: NbRisk
-Version: 35.0.0
-Summary: NIST 800-30 Risk Management for Netbox
-Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
-Author: Renato Almdida Oliveira
-Author-email: renato.almeida.oliveira@gmail.com
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Netbox Nbrisk
 [Netbox](https://github.com/netbox-community/netbox) Plugin inspired in NIST 800-30 Risk Management  **BETA VERSION**
 
 
 ## Compatibility
 
 This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 3.4.0 and later.
 
 ## Installation
 
 The plugin is available as a Python package and can be installed with pip.
 To ensure NBRisk plugin is automatically re-installed during future upgrades, create a file named local_requirements.txt (if not already existing) in the NetBox root directory (alongside requirements.txt) and list the NBRisk package:
 
+### For NetBox 3.4.x
+```shell
+# echo "NbRisk==^34.0.0" >> local_requirements.txt 
+```
+### For NetBox 3.5.x
 ```shell
-# echo "NbRisk" >> local_requirements.txt
+# echo "NbRisk==^35.0.0" >> local_requirements.txt 
 ```
 
 Once installed, the plugin needs to be enabled in your configuration.py
 
 ```python
 # In your configuration.py
 PLUGINS = ["nb_risk"]
@@ -94,8 +86,7 @@
 ### Threat Event View
 
 ![image](https://user-images.githubusercontent.com/16046203/214702045-c3e01bfe-1b2c-4100-ae00-c42d3f23cfdb.png)
 
 ### Risks View
 
 ![image](https://user-images.githubusercontent.com/16046203/214702218-b74e9f49-6a0d-4789-8518-32e99ef7fead.png)
-
```

### Comparing `NbRisk-35.0.0/NbRisk.egg-info/SOURCES.txt` & `NbRisk-35.0.1/NbRisk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/PKG-INFO` & `NbRisk-35.0.1/NbRisk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 35.0.0
+Version: 35.0.1
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
@@ -20,16 +20,21 @@
 This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 3.4.0 and later.
 
 ## Installation
 
 The plugin is available as a Python package and can be installed with pip.
 To ensure NBRisk plugin is automatically re-installed during future upgrades, create a file named local_requirements.txt (if not already existing) in the NetBox root directory (alongside requirements.txt) and list the NBRisk package:
 
+### For NetBox 3.4.x
 ```shell
-# echo "NbRisk" >> local_requirements.txt
+# echo "NbRisk==^34.0.0" >> local_requirements.txt 
+```
+### For NetBox 3.5.x
+```shell
+# echo "NbRisk==^35.0.0" >> local_requirements.txt 
 ```
 
 Once installed, the plugin needs to be enabled in your configuration.py
 
 ```python
 # In your configuration.py
 PLUGINS = ["nb_risk"]
@@ -94,8 +99,7 @@
 ### Threat Event View
 
 ![image](https://user-images.githubusercontent.com/16046203/214702045-c3e01bfe-1b2c-4100-ae00-c42d3f23cfdb.png)
 
 ### Risks View
 
 ![image](https://user-images.githubusercontent.com/16046203/214702218-b74e9f49-6a0d-4789-8518-32e99ef7fead.png)
-
```

### Comparing `NbRisk-35.0.0/README.md` & `NbRisk-35.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,40 @@
+Metadata-Version: 2.1
+Name: NbRisk
+Version: 35.0.1
+Summary: NIST 800-30 Risk Management for Netbox
+Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
+Author: Renato Almdida Oliveira
+Author-email: renato.almeida.oliveira@gmail.com
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Framework :: Django
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Netbox Nbrisk
 [Netbox](https://github.com/netbox-community/netbox) Plugin inspired in NIST 800-30 Risk Management  **BETA VERSION**
 
 
 ## Compatibility
 
 This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 3.4.0 and later.
 
 ## Installation
 
 The plugin is available as a Python package and can be installed with pip.
 To ensure NBRisk plugin is automatically re-installed during future upgrades, create a file named local_requirements.txt (if not already existing) in the NetBox root directory (alongside requirements.txt) and list the NBRisk package:
 
+### For NetBox 3.4.x
+```shell
+# echo "NbRisk==^34.0.0" >> local_requirements.txt 
+```
+### For NetBox 3.5.x
 ```shell
-# echo "NbRisk" >> local_requirements.txt
+# echo "NbRisk==^35.0.0" >> local_requirements.txt 
 ```
 
 Once installed, the plugin needs to be enabled in your configuration.py
 
 ```python
 # In your configuration.py
 PLUGINS = ["nb_risk"]
@@ -81,8 +99,7 @@
 ### Threat Event View
 
 ![image](https://user-images.githubusercontent.com/16046203/214702045-c3e01bfe-1b2c-4100-ae00-c42d3f23cfdb.png)
 
 ### Risks View
 
 ![image](https://user-images.githubusercontent.com/16046203/214702218-b74e9f49-6a0d-4789-8518-32e99ef7fead.png)
-
```

### Comparing `NbRisk-35.0.0/nb_risk/__init__.py` & `NbRisk-35.0.1/nb_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/api/nested_serializers.py` & `NbRisk-35.0.1/nb_risk/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/api/serializers.py` & `NbRisk-35.0.1/nb_risk/api/serializers.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/api/views.py` & `NbRisk-35.0.1/nb_risk/api/views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/choices.py` & `NbRisk-35.0.1/nb_risk/choices.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/columns.py` & `NbRisk-35.0.1/nb_risk/columns.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/cve.py` & `NbRisk-35.0.1/nb_risk/cve.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/filters.py` & `NbRisk-35.0.1/nb_risk/filters.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/forms.py` & `NbRisk-35.0.1/nb_risk/forms.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/migrations/0001_initial.py` & `NbRisk-35.0.1/nb_risk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py` & `NbRisk-35.0.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/migrations/0003_control.py` & `NbRisk-35.0.1/nb_risk/migrations/0003_control.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/models.py` & `NbRisk-35.0.1/nb_risk/models.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/navigation.py` & `NbRisk-35.0.1/nb_risk/navigation.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/tables.py` & `NbRisk-35.0.1/nb_risk/tables.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/template_content.py` & `NbRisk-35.0.1/nb_risk/template_content.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/templates/nb_risk/control.html` & `NbRisk-35.0.1/nb_risk/templates/nb_risk/risk.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,58 @@
 {% extends 'generic/object.html' %}
 {% load render_table from django_tables2 %}
-{% load tabs %}
 
 
-{% block tabs %}
-  <ul class="nav nav-tabs px-3">
-    {# Primary tab #}
-    <li class="nav-item" role="presentation">
-      <a class="nav-link{% if not tab %} active{% endif %}" href="{{ object.get_absolute_url }}">{{ object|meta:"verbose_name"|bettertitle }}</a>
-    </li>
-    <li role="presentation" class="nav-item">
-        <a href="{% url 'plugins:nb_risk:control_risks' pk=object.pk %}" class="nav-link{% if tab == 'risks' %} active{% endif %}">
-            Risks  {% if risks_count  %}<span class="badge bg-secondary">{{ risks_count }}</span>{% endif %}
-        </a>
-    </li>
-    <li role="presentation" class="nav-item">
-        <a href="{% url 'plugins:nb_risk:control_assets' pk=object.pk %}" class="nav-link{% if tab == 'assets' %} active{% endif %}">
-            Related Assets  {% if assets_count  %}<span class="badge bg-secondary">{{ assets_count }}</span>{% endif %}
-        </a>
-    </li>
-
-    {# Include tabs for registered model views #}
-    {% model_view_tabs object %}
-  </ul>
-{% endblock tabs %}
 
 {% block content %}
 <div class="row mb-3">
     <div class="col col-md-6">
         <div class="card">
-            <h5 class="card-header">Control</h5>
+            <h5 class="card-header">Vulnerability</h5>
             <div class="card-body">
                 <table class="table table-hover attr-table">
                     <tr>
                         <th scope="row">Name</th>
                         <td>{{ object.name }}</td>
                     </tr>
                     <tr>
-                        <th scope="row">Category</th>
-                        <td>{{ object.category }}</td>
+                        <th scope="row">Description</th>
+                        <td>{{ object.description }}</td>
+                    </tr>
+                    <th scope="row">Threat Event</th>
+                        <td>
+                            {% if object.threat_event %}
+                            {% if object.threat_event.get_absolute_url %}
+                                <a href="{{ object.threat_event.get_absolute_url }}">{{ object.threat_event }}</a>                            
+                            {% endif %}
+                            {% else %}
+                                ---
+                            {% endif %}
+                        </td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Likelihood</th>
+                        <td>{{ object.likelihood }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Level of Impact</th>
+                        <td>{{ object.impact }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Level of Risk</th>
+                        <td>{{ object.risk_level }}</td>
                     </tr>
                 </table>
             </div>
         </div>
-    </div>
-    <div class="col col-md-6">
-        <div class="card">
-            <h5 class="card-header">Notes</h5>
-            <div class="card-body">
-              {{ object.notes | markdown  }}
-            </div>
-        </div> 
-    </div>
-</div>
-<div class="row mb-3">
-    <div class="col col-md-6">
-        {% include 'inc/panels/comments.html' %}
-        {% include 'inc/panels/custom_fields.html' %}
         {% include 'inc/panels/tags.html' %}
     </div>
-           
+    <div class="col col-md-6">        
+        <div class="card">
+          <h5 class="card-header">Notes</h5>
+          <div class="card-body">
+            {{ object.notes | markdown  }}
+          </div>
+        </div>
+      </div>
 </div>
-
-
-
-
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,17 +1,12 @@
 {% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
-{% load tabs %} {% block tabs %}
-    * {# Primary tab #}
-    * {{_object|meta:"verbose_name"|bettertitle_}}
-    * Risks_{%_if_risks_count_%}{{_risks_count_}}{%_endif_%}
-    * Related_Assets_{%_if_assets_count_%}{{_assets_count_}}{%_endif_%}
-    * {# Include tabs for registered model views #} {% model_view_tabs object
-      %}
-{% endblock tabs %} {% block content %}
-** Control **
-Name     {{ object.name }}
-Category {{ object.category }}
+{% block content %}
+** Vulnerability **
+Name            {{ object.name }}
+Description     {{ object.description }}
+Likelihood      {{ object.likelihood }}
+Level of Impact {{ object.impact }}
+Level of Risk   {{ object.risk_level }}
+{% include 'inc/panels/tags.html' %}
 ** Notes **
 {{ object.notes | markdown }}
-{% include 'inc/panels/comments.html' %} {% include 'inc/panels/
-custom_fields.html' %} {% include 'inc/panels/tags.html' %}
 {% endblock %}
```

### Comparing `NbRisk-35.0.0/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html` & `NbRisk-35.0.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/templates/nb_risk/risk.html` & `NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,77 @@
 {% extends 'generic/object.html' %}
+{% load humanize %}
+{% load helpers %}
 {% load render_table from django_tables2 %}
 
 
-
 {% block content %}
 <div class="row mb-3">
     <div class="col col-md-6">
         <div class="card">
             <h5 class="card-header">Vulnerability</h5>
             <div class="card-body">
                 <table class="table table-hover attr-table">
                     <tr>
                         <th scope="row">Name</th>
                         <td>{{ object.name }}</td>
                     </tr>
                     <tr>
-                        <th scope="row">Description</th>
-                        <td>{{ object.description }}</td>
-                    </tr>
-                    <th scope="row">Threat Event</th>
-                        <td>
-                            {% if object.threat_event %}
-                            {% if object.threat_event.get_absolute_url %}
-                                <a href="{{ object.threat_event.get_absolute_url }}">{{ object.threat_event }}</a>                            
-                            {% endif %}
-                            {% else %}
-                                ---
-                            {% endif %}
-                        </td>
+                        <th scope="row">CVE</th>
+                        <td>{{ object.cve }}</td>
                     </tr>
                     <tr>
-                        <th scope="row">Likelihood</th>
-                        <td>{{ object.likelihood }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Level of Impact</th>
-                        <td>{{ object.impact }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Level of Risk</th>
-                        <td>{{ object.risk_level }}</td>
+                        <th scope="row">Description</th>
+                        <td>{{ object.description }}</td>
                     </tr>
                 </table>
             </div>
         </div>
-        {% include 'inc/panels/tags.html' %}
-    </div>
-    <div class="col col-md-6">        
         <div class="card">
           <h5 class="card-header">Notes</h5>
           <div class="card-body">
             {{ object.notes | markdown  }}
           </div>
+        </div>        
+    </div>
+    <div class="col col-md-6">        
+      <div class="card">
+        <h5 class="card-header">CVSSv2 Score</h5>
+        <div class="card-body">
+          <table class="table table-hover attr-table">
+            <tr>
+              <th scope="row">Access Vector (AV)</th>
+              <td>{{ object.cvssaccessVector }}</td>
+            </tr>
+            <tr>
+              <th scope="row">Access Complexity (AC)</th>
+              <td>{{ object.cvssaccessComplexity }}</td>
+            </tr>
+            <tr>
+              <th scope="row">Authentication (Au)</th>
+              <td>{{ object.cvssauthentication }}</td>
+            </tr>
+            <tr>
+              <th scope="row">Confidentiality Impact (C)</th>
+              <td>{{ object.cvssconfidentialityImpact }}</td>
+            </tr>
+            <tr>
+              <th scope="row">Integrity Impact (I)</th>
+              <td>{{ object.cvssintegrityImpact }}</td>
+            </tr>
+            <tr>
+              <th scope="row">Availability Impact (A)</th>
+              <td>{{ object.cvssavailabilityImpact }}</td>
+            </tr>
+            <tr>
+              <th scope="row">Base Score</th>
+              <td>{{ object.cvssbaseScore }}</td>
+            </tr> 
+          </table>
         </div>
       </div>
+      {% include 'inc/panels/tags.html' %}
+    </div>
+
 </div>
-{% endblock %}
+{% endblock %}
+
```

#### html2text {}

```diff
@@ -1,12 +1,18 @@
-{% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
-{% block content %}
+{% extends 'generic/object.html' %} {% load humanize %} {% load helpers %} {%
+load render_table from django_tables2 %} {% block content %}
 ** Vulnerability **
-Name            {{ object.name }}
-Description     {{ object.description }}
-Likelihood      {{ object.likelihood }}
-Level of Impact {{ object.impact }}
-Level of Risk   {{ object.risk_level }}
-{% include 'inc/panels/tags.html' %}
+Name        {{ object.name }}
+CVE         {{ object.cve }}
+Description {{ object.description }}
 ** Notes **
 {{ object.notes | markdown }}
+** CVSSv2 Score **
+Access Vector (AV)         {{ object.cvssaccessVector }}
+Access Complexity (AC)     {{ object.cvssaccessComplexity }}
+Authentication (Au)        {{ object.cvssauthentication }}
+Confidentiality Impact (C) {{ object.cvssconfidentialityImpact }}
+Integrity Impact (I)       {{ object.cvssintegrityImpact }}
+Availability Impact (A)    {{ object.cvssavailabilityImpact }}
+Base Score                 {{ object.cvssbaseScore }}
+{% include 'inc/panels/tags.html' %}
 {% endblock %}
```

### Comparing `NbRisk-35.0.0/nb_risk/templates/nb_risk/threatsource.html` & `NbRisk-35.0.1/nb_risk/templates/nb_risk/threatsource.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability_search.html` & `NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability_search.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.0/nb_risk/views.py` & `NbRisk-35.0.1/nb_risk/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,26 +40,25 @@
 # ThreatEvent Views
 
 
 class ThreatEventView(generic.ObjectView):
     queryset = models.ThreatEvent.objects.all()
 
 
-class ThreatEventVulnerabilityView(generic.ObjectView):
+@register_model_view(models.ThreatEvent, name='vulnerabilities')
+class ThreatEventVulnerabilityView(generic.ObjectChildrenView):
     queryset = models.ThreatEvent.objects.all()
+    child_model = models.Vulnerability
+    table = tables.VulnerabilityExploitListTable
     template_name = "nb_risk/threatevent_vulnerabilities.html"
+    tab = ViewTab(label='Exploit Vulnerabilities', badge=lambda obj: obj.vulnerability.all().count(), hide_if_empty=True)
 
-    def get_extra_context(self, request, instance):
-        vulnerabilities = instance.vulnerability.all()
-        table = tables.VulnerabilityExploitListTable(vulnerabilities)
-        data = {
-            "tab": "vulnerabilities",
-            "table": table,
-        }
-        return data
+    def get_children(self, request, parent):
+            childrens = parent.vulnerability.all()
+            return childrens
 
 
 class ThreatEventListView(generic.ObjectListView):
     queryset = models.ThreatEvent.objects.all()
     table = tables.ThreatEventTable
     filterset = filters.ThreatEventFilterSet
     filterset_form = forms.ThreatEventFilterForm
@@ -81,39 +80,28 @@
 
 # Vulnerability Views
 
 
 class VulnerabilityView(generic.ObjectView):
     queryset = models.Vulnerability.objects.all()
 
-    def get_extra_context(self, request, instance):
-        affected_assets_count = models.VulnerabilityAssignment.objects.filter(
-            vulnerability=instance
-        ).count()
-        data = {
-            "affected_assets_count": affected_assets_count,
-        }
-        return data
-
 
-class VulnerabilityAffectedAssetsView(generic.ObjectView):
+@register_model_view(models.Vulnerability, name='affected_assets')
+class VulnerabilityAffectedAssetsView(generic.ObjectChildrenView):
     queryset = models.Vulnerability.objects.all()
+    child_model = models.Vulnerability
+    table = tables.VulnerabilityAssignmentListTable
     template_name = "nb_risk/vulnerability_affected_assets.html"
+    tab = ViewTab(label='Affected Assets', badge=lambda obj: models.VulnerabilityAssignment.objects.filter(vulnerability=obj).count(), hide_if_empty=True)
 
-    def get_extra_context(self, request, instance):
-        assets = models.VulnerabilityAssignment.objects.filter(vulnerability=instance)
-        table = tables.VulnerabilityAssignmentListTable(assets)
-        data = {
-            "tab": "affected_assets",
-            "affected_assets_count": assets.count(),
-            "table": table,
-        }
-        return data
-
+    def get_children(self, request, parent):
+            childrens = models.VulnerabilityAssignment.objects.filter(vulnerability=parent)
+            return childrens
 
+    
 class VulnerabilityListView(generic.ObjectListView):
     queryset = models.Vulnerability.objects.all()
     table = tables.VulnerabilityTable
     filterset = filters.VulnerabilityFilterSet
     filterset_form = forms.VulnerabilityFilterForm
     template_name = "nb_risk/vulnerability_list.html"
 
@@ -268,50 +256,46 @@
         assets = models.VulnerabilityAssignment.objects.filter(threat_events__in=thread_events)
         data = {
             "risks_count": risks.count(),
             "assets_count": assets.count(),
         }
         return data
 
-class ControlRisksView(generic.ObjectView):
+@register_model_view(models.Control, name='risks')
+class ControlRisksView(generic.ObjectChildrenView):
     queryset = models.Control.objects.all()
+    child_model = models.Risk
+    table = tables.RiskTable
     template_name = "nb_risk/control_risks.html"
-    
-    def get_extra_context(self, request, instance):
+    tab = ViewTab(label='Risks', badge=lambda obj: obj.risk.all().count(), hide_if_empty=True)
+
+    def get_children(self, request, parent):
+            childrens = parent.risk.all()
+            return childrens
+
+def _get_assets(instance):
         risks = instance.risk.all()
         thread_events = []
         for risk in risks:
             thread_events.append(risk.threat_event)
         assets = models.VulnerabilityAssignment.objects.filter(threat_events__in=thread_events)
-        table = tables.RiskTable(risks)
-        data = {
-            "tab": "risks",
-            "risks_count": risks.count(),
-            "assets_count": assets.count(),
-            "table": table,
-        }
-        return data
+        return assets
 
-class ControlAssetsView(generic.ObjectView):
+@register_model_view(models.Control, name='assets')
+class ControlAssetsView(generic.ObjectChildrenView):
     queryset = models.Control.objects.all()
+    child_model = models.VulnerabilityAssignment
+    table = tables.VulnerabilityAssignmentListTable
     template_name = "nb_risk/control_assets.html"
-    
-    def get_extra_context(self, request, instance):
-        risks = instance.risk.all()
-        thread_events = []
-        for risk in risks:
-            thread_events.append(risk.threat_event)
-        assets = models.VulnerabilityAssignment.objects.filter(threat_events__in=thread_events)
-        table = tables.VulnerabilityAssignmentListTable(assets)
-        data = {
-            "tab": "assets",
-            "assets_count": assets.count(),
-            "table": table,
-        }
-        return data
+    tab = ViewTab(label='Related Assets', badge=lambda obj: _get_assets(obj).count(), hide_if_empty=True)
+
+
+    def get_children(self, request, parent):
+            childrens = _get_assets(parent)
+            return childrens
 
 class ControlEditView(generic.ObjectEditView):
     queryset = models.Control.objects.all()
     form = forms.ControlForm
 
 class ControlDeleteView(generic.ObjectDeleteView):
     queryset = models.Control.objects.all()
```

### Comparing `NbRisk-35.0.0/setup.py` & `NbRisk-35.0.1/setup.py`

 * *Files identical despite different names*

