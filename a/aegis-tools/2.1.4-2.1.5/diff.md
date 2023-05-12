# Comparing `tmp/aegis-tools-2.1.4.tar.gz` & `tmp/aegis-tools-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.1.4.tar", last modified: Fri May  5 18:35:21 2023, max compression
+gzip compressed data, was "aegis-tools-2.1.5.tar", last modified: Fri May 12 16:03:16 2023, max compression
```

## Comparing `aegis-tools-2.1.4.tar` & `aegis-tools-2.1.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-05 18:35:21.949747 aegis-tools-2.1.4/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-05-05 18:35:21.945747 aegis-tools-2.1.4/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-05 18:35:21.925747 aegis-tools-2.1.4/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.4/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18100 2022-11-21 04:55:50.000000 aegis-tools-2.1.4/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.4/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.4/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-04-04 22:56:26.000000 aegis-tools-2.1.4/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7276 2023-04-24 22:47:56.000000 aegis-tools-2.1.4/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    42564 2023-05-05 18:15:10.000000 aegis-tools-2.1.4/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-05 18:35:21.937747 aegis-tools-2.1.4/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.4/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.4/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.4/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.4/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-03-13 22:09:08.000000 aegis-tools-2.1.4/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31593 2023-04-24 21:25:57.000000 aegis-tools-2.1.4/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-05 18:35:21.945747 aegis-tools-2.1.4/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.4/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.4/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.4/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.4/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-04-27 02:34:36.000000 aegis-tools-2.1.4/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.4/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.4/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.4/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.4/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.4/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.4/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.4/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.4/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73309 2023-05-05 18:28:25.000000 aegis-tools-2.1.4/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-05 18:35:21.945747 aegis-tools-2.1.4/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-05-05 18:35:21.000000 aegis-tools-2.1.4/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-05-05 18:35:21.000000 aegis-tools-2.1.4/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-05-05 18:35:21.000000 aegis-tools-2.1.4/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-05-05 18:35:21.000000 aegis-tools-2.1.4/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-05-05 18:35:21.000000 aegis-tools-2.1.4/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-05-05 18:35:21.000000 aegis-tools-2.1.4/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-05-05 18:35:21.949747 aegis-tools-2.1.4/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-05-05 18:33:29.000000 aegis-tools-2.1.4/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-12 16:03:16.109043 aegis-tools-2.1.5/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-05-12 16:03:16.109043 aegis-tools-2.1.5/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-12 16:03:16.093043 aegis-tools-2.1.5/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.5/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18804 2023-05-12 16:02:53.000000 aegis-tools-2.1.5/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.5/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.5/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-04-04 22:56:26.000000 aegis-tools-2.1.5/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7276 2023-04-24 22:47:56.000000 aegis-tools-2.1.5/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    42564 2023-05-05 18:15:10.000000 aegis-tools-2.1.5/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-12 16:03:16.101043 aegis-tools-2.1.5/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.5/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.5/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.5/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.5/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-03-13 22:09:08.000000 aegis-tools-2.1.5/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31593 2023-04-24 21:25:57.000000 aegis-tools-2.1.5/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-12 16:03:16.109043 aegis-tools-2.1.5/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.5/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.5/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.5/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.5/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-04-27 02:34:36.000000 aegis-tools-2.1.5/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.5/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.5/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.5/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.5/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.5/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.5/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.5/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.5/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73309 2023-05-05 18:28:25.000000 aegis-tools-2.1.5/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-12 16:03:16.109043 aegis-tools-2.1.5/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-05-12 16:03:16.000000 aegis-tools-2.1.5/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-05-12 16:03:16.000000 aegis-tools-2.1.5/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-05-12 16:03:16.000000 aegis-tools-2.1.5/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-05-12 16:03:16.000000 aegis-tools-2.1.5/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-05-12 16:03:16.000000 aegis-tools-2.1.5/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-05-12 16:03:16.000000 aegis-tools-2.1.5/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-05-12 16:03:16.109043 aegis-tools-2.1.5/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-05-12 16:03:01.000000 aegis-tools-2.1.5/setup.py
```

### Comparing `aegis-tools-2.1.4/LICENSE` & `aegis-tools-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/PKG-INFO` & `aegis-tools-2.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.4
+Version: 2.1.5
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.4/README.md` & `aegis-tools-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/aegis_.py` & `aegis-tools-2.1.5/aegis/aegis_.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/build.py` & `aegis-tools-2.1.5/aegis/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,26 +94,32 @@
             version_json.write('{"version": "%s"}\n' % self.next_tag)
             version_json.close()
             # Set up virtualenv
             if self._shell_exec("virtualenv --python=/usr/bin/python3 --system-site-packages virtualenv", cwd=self.build_dir, build_step='build'):
                 return
             if self._shell_exec("virtualenv/bin/pip --cache-dir .cache install -e .", cwd=self.build_dir, build_step='build'):
                 return
-            # Set up and run yarn if it's installed
+            # Set up and run npm if it's installed TODO and package.lock file exists in the root of repository
+            package_lock = os.path.exists(os.path.join(self.build_dir, 'package-lock.json'))
+            self.npm, stderr, exit_status = aegis.stdlib.shell('which npm', cwd=self.src_dir)
+            if self.npm and package_lock:
+                if self._shell_exec("npm install", cwd=self.build_dir, build_step='build'):
+                    return
+                if self._shell_exec("npm run %s" % self.build_row['env'], cwd=self.build_dir, build_step='build'):
+                    return
+            # Set up and run yarn if it's installed TODO and yarn.lock file exists in the root of repository
+            yarn_lock = os.path.exists(os.path.join(self.build_dir, 'yarn.lock'))
             self.yarn, stderr, exit_status = aegis.stdlib.shell('which yarn', cwd=self.src_dir)
-            if self.yarn:
-                yarn_dir = aegis.config.get('yarn_dir')
-                if yarn_dir:
-                    yarn_dir = os.path.join(self.build_dir, yarn_dir)
-                else:
-                    yarn_dir = self.build_dir
-                if self._shell_exec("yarn install", cwd=yarn_dir, build_step='build'):
+            if self.yarn and yarn_lock:
+                if self._shell_exec("yarn install", cwd=self.build_dir, build_step='build'):
                     return
-                if self._shell_exec("yarn run %s" % self.build_row['env'], cwd=yarn_dir, build_step='build'):
+                if self._shell_exec("yarn run %s" % self.build_row['env'], cwd=self.build_dir, build_step='build'):
                     return
+            # If we (essentially) ran webpack, build a version file and check file size
+            if (self.yarn and yarn_lock) or (self.npm and package_lock):
                 build_file_version = self.next_tag
                 if self.build_row['env'] in options.build_local_envs:
                     build_file_version = 'local'
                 build_file_name = options.build_output_file % {'version': build_file_version}
                 build_output_file = os.path.join(self.build_dir, build_file_name)
                 if os.path.exists(build_output_file):
                     build_size = os.path.getsize(build_output_file)
```

### Comparing `aegis-tools-2.1.4/aegis/config.py` & `aegis-tools-2.1.5/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/database.py` & `aegis-tools-2.1.5/aegis/database.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/hydra.py` & `aegis-tools-2.1.5/aegis/hydra.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/mailer.py` & `aegis-tools-2.1.5/aegis/mailer.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/model.py` & `aegis-tools-2.1.5/aegis/model.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.1.5/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.1.5/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/sql/build-mysql.sql` & `aegis-tools-2.1.5/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/sql/build-pgsql.sql` & `aegis-tools-2.1.5/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.1.5/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/sql/google_signin.sql` & `aegis-tools-2.1.5/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.1.5/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.1.5/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/sql/member_auth.sql` & `aegis-tools-2.1.5/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.1.5/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/sql/reports.sql` & `aegis-tools-2.1.5/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/stdlib.py` & `aegis-tools-2.1.5/aegis/stdlib.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/templates/build.html` & `aegis-tools-2.1.5/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/templates/build_confirm.html` & `aegis-tools-2.1.5/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/templates/build_form.html` & `aegis-tools-2.1.5/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/templates/build_view.html` & `aegis-tools-2.1.5/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/templates/frame.html` & `aegis-tools-2.1.5/aegis/templates/frame.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/templates/hydra.html` & `aegis-tools-2.1.5/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/templates/hydra_form.html` & `aegis-tools-2.1.5/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/templates/hydra_queue.html` & `aegis-tools-2.1.5/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/templates/report.html` & `aegis-tools-2.1.5/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/templates/report_form.html` & `aegis-tools-2.1.5/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/templates/reports.html` & `aegis-tools-2.1.5/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/templates/w3.css` & `aegis-tools-2.1.5/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/threadpool.py` & `aegis-tools-2.1.5/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis/webapp.py` & `aegis-tools-2.1.5/aegis/webapp.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.1.5/aegis_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.4
+Version: 2.1.5
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.4/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.1.5/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.4/setup.py` & `aegis-tools-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import os
 import setuptools
 
 setuptools.setup (
     name = 'aegis-tools',
-    version = '2.1.4',
+    version = '2.1.5',
     description = 'Aegis is a set of battle-tested tools and tricks to help everyone make better software',
     long_description = 'A combination of tools and framework, Aegis has multiple different uses. You can import it and use the thoroughly made and tested functions. You can use it as a natural extension for the tornado web framework. And you can use it to quickly create a new web application with the structure already built-in, and follow along.',
     author = "Michael D'Agosta",
     author_email = 'mdagosta@codebug.com',
     url = 'https://github.com/mdagosta/aegis',
     python_requires='>=3.6',
     packages = ['aegis'],
```

