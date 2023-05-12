# Comparing `tmp/ovos_PHAL-0.0.5a4-py3-none-any.whl.zip` & `tmp/ovos_PHAL-0.0.5a5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9313 bytes, number of entries: 12
--rw-r--r--  2.0 unx      148 b- defN 23-Apr-11 22:53 ovos_PHAL/__init__.py
--rw-r--r--  2.0 unx      572 b- defN 23-Apr-11 22:53 ovos_PHAL/__main__.py
--rw-r--r--  2.0 unx     2569 b- defN 23-Apr-11 22:53 ovos_PHAL/admin.py
--rw-r--r--  2.0 unx     1436 b- defN 23-Apr-11 22:53 ovos_PHAL/detection.py
--rw-r--r--  2.0 unx     3047 b- defN 23-Apr-11 22:53 ovos_PHAL/service.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-11 22:54 ovos_PHAL/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Apr-11 22:54 ovos_PHAL-0.0.5a4.dist-info/LICENSE
--rw-r--r--  2.0 unx      899 b- defN 23-Apr-11 22:54 ovos_PHAL-0.0.5a4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 22:54 ovos_PHAL-0.0.5a4.dist-info/WHEEL
--rw-r--r--  2.0 unx       94 b- defN 23-Apr-11 22:54 ovos_PHAL-0.0.5a4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-11 22:54 ovos_PHAL-0.0.5a4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      966 b- defN 23-Apr-11 22:54 ovos_PHAL-0.0.5a4.dist-info/RECORD
-12 files, 21359 bytes uncompressed, 7689 bytes compressed:  64.0%
+Zip file size: 9562 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      148 b- defN 23-May-12 20:32 ovos_PHAL/__init__.py
+-rw-r--r--  2.0 unx      572 b- defN 23-May-12 20:32 ovos_PHAL/__main__.py
+-rw-r--r--  2.0 unx     2569 b- defN 23-May-12 20:32 ovos_PHAL/admin.py
+-rw-r--r--  2.0 unx     1436 b- defN 23-May-12 20:32 ovos_PHAL/detection.py
+-rw-r--r--  2.0 unx     3047 b- defN 23-May-12 20:32 ovos_PHAL/service.py
+-rw-r--r--  2.0 unx      177 b- defN 23-May-12 20:32 ovos_PHAL/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-May-12 20:32 ovos_PHAL-0.0.5a5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1384 b- defN 23-May-12 20:32 ovos_PHAL-0.0.5a5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 20:32 ovos_PHAL-0.0.5a5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       94 b- defN 23-May-12 20:32 ovos_PHAL-0.0.5a5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-May-12 20:32 ovos_PHAL-0.0.5a5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      967 b- defN 23-May-12 20:32 ovos_PHAL-0.0.5a5.dist-info/RECORD
+12 files, 21845 bytes uncompressed, 7938 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: ovos_PHAL/service.py
 Comment: 
 
 Filename: ovos_PHAL/version.py
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a4.dist-info/LICENSE
+Filename: ovos_PHAL-0.0.5a5.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a4.dist-info/METADATA
+Filename: ovos_PHAL-0.0.5a5.dist-info/METADATA
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a4.dist-info/WHEEL
+Filename: ovos_PHAL-0.0.5a5.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a4.dist-info/entry_points.txt
+Filename: ovos_PHAL-0.0.5a5.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a4.dist-info/top_level.txt
+Filename: ovos_PHAL-0.0.5a5.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a4.dist-info/RECORD
+Filename: ovos_PHAL-0.0.5a5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_PHAL/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 5
-VERSION_ALPHA = 4
+VERSION_ALPHA = 5
 # END_VERSION_BLOCK
```

## Comparing `ovos_PHAL-0.0.5a4.dist-info/LICENSE` & `ovos_PHAL-0.0.5a5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_PHAL-0.0.5a4.dist-info/METADATA` & `ovos_PHAL-0.0.5a5.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL
-Version: 0.0.5a4
-Summary: UNKNOWN
+Version: 0.0.5a5
+Summary: Plugin based Hardware Abstraction Layer for OVOS
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL
 Author: jarbasAi
 Author-email: jarbasai@mailfence.com
 License: apache-2.0
 Platform: UNKNOWN
+Description-Content-Type: text/markdown
 Requires-Dist: ovos-utils (>=0.0.31a6,~=0.0)
 Requires-Dist: ovos-bus-client (>=0.0.3a16,~=0.0)
 Requires-Dist: ovos-workshop (>=0.0.12a3,~=0.0)
 Requires-Dist: ovos-config (>=0.0.8a3,~=0.0)
 Requires-Dist: ovos-plugin-manager (>=0.0.23a5,~=0.0)
 Requires-Dist: ovos-phal-plugin-connectivity-events (>=0.0.1,~=0.0)
 Requires-Dist: ovos-PHAL-plugin-wallpaper-manager (>=0.0.0,~=0.0)
 Requires-Dist: ovos-PHAL-plugin-network-manager (>=1.0.0,~=1.0)
 Requires-Dist: ovos-phal-plugin-ipgeo (>=0.0.1,~=0.0)
 Requires-Dist: ovos-PHAL-plugin-oauth (>=0.0.1,~=0.0)
 Requires-Dist: ovos-PHAL-plugin-system (>=0.0.1,~=0.0)
 Requires-Dist: ovos-PHAL-plugin-color-scheme-manager (>=1.0.0,~=1.0)
 
-UNKNOWN
+# ovos_PHAL
+
+Plugin based Hardware Abstraction Layer
+
+a wrapper for software system level abstraction, where based on the environment either through known configuration or via fingerprinting, only specific plugins load to interface with the system and specific hardware
+
+A PHAL plugin can provide anything from hardware integrations (respeaker, mk1, mk2....) or system integrations (network manager, ovos shell)
```

## Comparing `ovos_PHAL-0.0.5a4.dist-info/RECORD` & `ovos_PHAL-0.0.5a5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ovos_PHAL/__init__.py,sha256=01I5hydahUGIIOXvvE2nM3Nul5Vr5YabvYM2aEh0TkQ,148
 ovos_PHAL/__main__.py,sha256=CsDEsncExx6vYTSJYkLDD6uL1hZXxwZA2KbKezr0Swo,572
 ovos_PHAL/admin.py,sha256=DJbRTi0orOnBRIZXpqf7ya_fZI3za8gJRze2VTRYYOQ,2569
 ovos_PHAL/detection.py,sha256=GujqinjXF467EdMk80StP1he1bYUHUWvSQ1j7mYJbe8,1436
 ovos_PHAL/service.py,sha256=fEzfP5RAASL_qui90CL3gjGDwVnluIfMLHTtnYty2Jw,3047
-ovos_PHAL/version.py,sha256=cKXdvCe6mkZOCYR1os_noY-8Ug8zh6pEIlyy1GuTY-k,177
-ovos_PHAL-0.0.5a4.dist-info/LICENSE,sha256=ujdvnin8cAYCsJhQhQxfUSvS5yCf7RAk24ltOrau7rA,11349
-ovos_PHAL-0.0.5a4.dist-info/METADATA,sha256=s576RLEHpDq8cmq22FSloT1WI1i6Emjv0Rt8YQ3dP-0,899
-ovos_PHAL-0.0.5a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_PHAL-0.0.5a4.dist-info/entry_points.txt,sha256=iLNb-d0BX90d0YvhjUz0tr6l9-keqtJvUbj_djyE1vA,94
-ovos_PHAL-0.0.5a4.dist-info/top_level.txt,sha256=Pt4y92j6yi3cwUiC_jA7_7ztrK5zhkW3zQj0szVT8h0,10
-ovos_PHAL-0.0.5a4.dist-info/RECORD,,
+ovos_PHAL/version.py,sha256=nzsSHz085o-JI3_hWf58LlOWNJE9VNIC67f5iq5DyrA,177
+ovos_PHAL-0.0.5a5.dist-info/LICENSE,sha256=ujdvnin8cAYCsJhQhQxfUSvS5yCf7RAk24ltOrau7rA,11349
+ovos_PHAL-0.0.5a5.dist-info/METADATA,sha256=faiy3p1AU_tcfP_yf4AF50Bwrnd9Hpdo8mz8Yi1L-Qo,1384
+ovos_PHAL-0.0.5a5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_PHAL-0.0.5a5.dist-info/entry_points.txt,sha256=iLNb-d0BX90d0YvhjUz0tr6l9-keqtJvUbj_djyE1vA,94
+ovos_PHAL-0.0.5a5.dist-info/top_level.txt,sha256=Pt4y92j6yi3cwUiC_jA7_7ztrK5zhkW3zQj0szVT8h0,10
+ovos_PHAL-0.0.5a5.dist-info/RECORD,,
```

