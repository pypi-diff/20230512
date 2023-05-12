# Comparing `tmp/mobicontrol-0.1.5.tar.gz` & `tmp/mobicontrol-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mobicontrol-0.1.5.tar", last modified: Fri Aug 13 12:01:43 2021, max compression
+gzip compressed data, was "mobicontrol-0.2.0.tar", last modified: Fri May 12 07:37:32 2023, max compression
```

## Comparing `mobicontrol-0.1.5.tar` & `mobicontrol-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dkAndHej   (502) staff       (20)        0 2021-08-13 12:01:43.000000 mobicontrol-0.1.5/
--rw-r--r--   0 dkAndHej   (502) staff       (20)      185 2021-08-13 12:01:43.000000 mobicontrol-0.1.5/PKG-INFO
-drwxr-xr-x   0 dkAndHej   (502) staff       (20)        0 2021-08-13 12:01:43.000000 mobicontrol-0.1.5/mobicontrol/
--rw-r--r--   0 dkAndHej   (502) staff       (20)        0 2021-08-13 06:58:57.000000 mobicontrol-0.1.5/mobicontrol/__init__.py
--rw-r--r--   0 dkAndHej   (502) staff       (20)      245 2021-08-13 09:09:08.000000 mobicontrol-0.1.5/mobicontrol/utils.py
-drwxr-xr-x   0 dkAndHej   (502) staff       (20)        0 2021-08-13 12:01:43.000000 mobicontrol-0.1.5/mobicontrol/scripts/
--rw-r--r--   0 dkAndHej   (502) staff       (20)        0 2021-08-13 11:43:57.000000 mobicontrol-0.1.5/mobicontrol/scripts/__init__.py
--rw-r--r--   0 dkAndHej   (502) staff       (20)      386 2021-08-13 08:22:02.000000 mobicontrol-0.1.5/mobicontrol/scripts/fetch_token.py
--rw-r--r--   0 dkAndHej   (502) staff       (20)      922 2021-08-13 10:24:52.000000 mobicontrol-0.1.5/mobicontrol/scripts/upload_package.py
--rw-r--r--   0 dkAndHej   (502) staff       (20)     2883 2021-08-13 12:01:07.000000 mobicontrol-0.1.5/mobicontrol/main.py
--rw-r--r--   0 dkAndHej   (502) staff       (20)      334 2021-08-13 12:01:28.000000 mobicontrol-0.1.5/setup.py
-drwxr-xr-x   0 dkAndHej   (502) staff       (20)        0 2021-08-13 12:01:43.000000 mobicontrol-0.1.5/mobicontrol.egg-info/
--rw-r--r--   0 dkAndHej   (502) staff       (20)      185 2021-08-13 12:01:43.000000 mobicontrol-0.1.5/mobicontrol.egg-info/PKG-INFO
--rw-r--r--   0 dkAndHej   (502) staff       (20)      390 2021-08-13 12:01:43.000000 mobicontrol-0.1.5/mobicontrol.egg-info/SOURCES.txt
--rw-r--r--   0 dkAndHej   (502) staff       (20)       62 2021-08-13 12:01:43.000000 mobicontrol-0.1.5/mobicontrol.egg-info/entry_points.txt
--rw-r--r--   0 dkAndHej   (502) staff       (20)       15 2021-08-13 12:01:43.000000 mobicontrol-0.1.5/mobicontrol.egg-info/requires.txt
--rw-r--r--   0 dkAndHej   (502) staff       (20)       12 2021-08-13 12:01:43.000000 mobicontrol-0.1.5/mobicontrol.egg-info/top_level.txt
--rw-r--r--   0 dkAndHej   (502) staff       (20)        1 2021-08-13 12:01:43.000000 mobicontrol-0.1.5/mobicontrol.egg-info/dependency_links.txt
--rw-r--r--   0 dkAndHej   (502) staff       (20)       38 2021-08-13 12:01:43.000000 mobicontrol-0.1.5/setup.cfg
+drwxr-xr-x   0 dkAndHej   (502) staff       (20)        0 2023-05-12 07:37:32.654420 mobicontrol-0.2.0/
+-rw-r--r--   0 dkAndHej   (502) staff       (20)      136 2023-05-12 07:37:32.654021 mobicontrol-0.2.0/PKG-INFO
+drwxr-xr-x   0 dkAndHej   (502) staff       (20)        0 2023-05-12 07:37:32.645459 mobicontrol-0.2.0/mobicontrol/
+-rw-r--r--   0 dkAndHej   (502) staff       (20)        0 2021-08-13 06:58:57.000000 mobicontrol-0.2.0/mobicontrol/__init__.py
+-rw-r--r--   0 dkAndHej   (502) staff       (20)     4688 2023-05-12 07:31:59.000000 mobicontrol-0.2.0/mobicontrol/main.py
+drwxr-xr-x   0 dkAndHej   (502) staff       (20)        0 2023-05-12 07:37:32.653233 mobicontrol-0.2.0/mobicontrol/scripts/
+-rw-r--r--   0 dkAndHej   (502) staff       (20)        0 2021-08-13 11:43:57.000000 mobicontrol-0.2.0/mobicontrol/scripts/__init__.py
+-rw-r--r--   0 dkAndHej   (502) staff       (20)      386 2021-08-13 08:22:02.000000 mobicontrol-0.2.0/mobicontrol/scripts/fetch_token.py
+-rw-r--r--   0 dkAndHej   (502) staff       (20)      754 2023-05-12 07:19:36.000000 mobicontrol-0.2.0/mobicontrol/scripts/upload_apk.py
+-rw-r--r--   0 dkAndHej   (502) staff       (20)      245 2021-08-13 09:09:08.000000 mobicontrol-0.2.0/mobicontrol/utils.py
+drwxr-xr-x   0 dkAndHej   (502) staff       (20)        0 2023-05-12 07:37:32.650476 mobicontrol-0.2.0/mobicontrol.egg-info/
+-rw-r--r--   0 dkAndHej   (502) staff       (20)      136 2023-05-12 07:37:32.000000 mobicontrol-0.2.0/mobicontrol.egg-info/PKG-INFO
+-rw-r--r--   0 dkAndHej   (502) staff       (20)      386 2023-05-12 07:37:32.000000 mobicontrol-0.2.0/mobicontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 dkAndHej   (502) staff       (20)        1 2023-05-12 07:37:32.000000 mobicontrol-0.2.0/mobicontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 dkAndHej   (502) staff       (20)       62 2023-05-12 07:37:32.000000 mobicontrol-0.2.0/mobicontrol.egg-info/entry_points.txt
+-rw-r--r--   0 dkAndHej   (502) staff       (20)       15 2023-05-12 07:37:32.000000 mobicontrol-0.2.0/mobicontrol.egg-info/requires.txt
+-rw-r--r--   0 dkAndHej   (502) staff       (20)       12 2023-05-12 07:37:32.000000 mobicontrol-0.2.0/mobicontrol.egg-info/top_level.txt
+-rw-r--r--   0 dkAndHej   (502) staff       (20)       38 2023-05-12 07:37:32.654553 mobicontrol-0.2.0/setup.cfg
+-rw-r--r--   0 dkAndHej   (502) staff       (20)      298 2023-05-12 07:37:17.000000 mobicontrol-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mobicontrol-0.1.5/mobicontrol/scripts/upload_package.py` & `mobicontrol-0.2.0/mobicontrol/scripts/upload_apk.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,21 @@
-import requests
-import click
-
-def upload_package(url, token, file, filename):
+def get_apk_upload_data(url, token, file, filename):
     lf = "\r\n"
     boundary = "mc_boundary"
 
-    body =  f"--{boundary}{lf}" 
+    body = f"--{boundary}{lf}"
     body += f"Content-Type: application/vnd.android.application.metadata+json{lf}{lf}"
-    body += '{"DeviceFamily":"AndroidPlus"}' + lf +lf
-    body += f'--{boundary}{lf}'
-    body += f'Content-Type: application/vnd.android.application{lf}'
-    body += f'Content-Transfer-Encoding: Binary{lf}'
+    body += '{"DeviceFamily":"AndroidPlus"}' + lf + lf
+    body += f"--{boundary}{lf}"
+    body += f"Content-Type: application/vnd.android.application{lf}"
+    body += f"Content-Transfer-Encoding: Binary{lf}"
     body += f'Content-Disposition: attachment; filename="{filename}"{lf}{lf}'
-    body += file + lf 
+    body += file + lf
     body += f"--{boundary}--"
 
     headers = {
-        'Authorization': f"Bearer {token}",
-        'Accept': "application/json",
-        'Content-Type': f"multipart/related; boundary={boundary}",
+        "Authorization": f"Bearer {token}",
+        "Accept": "application/json",
+        "Content-Type": f"multipart/related; boundary={boundary}",
     }
 
-    try:
-        response = requests.post(f"{url}/packages", headers=headers, data=body)
-    except Exception as e:
-        click.echo(e)
-
-    return response.json()
+    return headers, body
```

