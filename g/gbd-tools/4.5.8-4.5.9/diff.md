# Comparing `tmp/gbd_tools-4.5.8.tar.gz` & `tmp/gbd_tools-4.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.5.8.tar", last modified: Thu May 11 11:41:56 2023, max compression
+gzip compressed data, was "gbd_tools-4.5.9.tar", last modified: Fri May 12 14:39:37 2023, max compression
```

## Comparing `gbd_tools-4.5.8.tar` & `gbd_tools-4.5.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:41:56.882307 gbd_tools-4.5.8/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.5.8/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.5.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3757 2023-05-11 11:41:56.878307 gbd_tools-4.5.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.5.8/README.md
--rwxrwxr-x   0 root         (0) root         (0)    12008 2023-05-10 10:58:05.000000 gbd_tools-4.5.8/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:41:56.874307 gbd_tools-4.5.8/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.5.8/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9800 2023-05-11 11:40:24.000000 gbd_tools-4.5.8/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.5.8/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    10587 2023-05-08 06:51:06.000000 gbd_tools-4.5.8/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     6455 2023-05-10 11:45:07.000000 gbd_tools-4.5.8/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5461 2023-05-10 15:10:05.000000 gbd_tools-4.5.8/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12359 2023-04-25 15:02:02.000000 gbd_tools-4.5.8/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.5.8/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-05 18:48:49.000000 gbd_tools-4.5.8/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:41:56.874307 gbd_tools-4.5.8/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.5.8/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7756 2023-05-10 08:09:50.000000 gbd_tools-4.5.8/gbd_init/cnf_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.5.8/gbd_init/cnf_transformers.py
--rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.5.8/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.5.8/gbd_init/initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:41:56.874307 gbd_tools-4.5.8/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.5.8/gbd_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:41:56.874307 gbd_tools-4.5.8/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:41:56.878307 gbd_tools-4.5.8/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.5.8/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.5.8/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.5.8/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.5.8/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.5.8/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:41:56.878307 gbd_tools-4.5.8/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.5.8/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:41:56.878307 gbd_tools-4.5.8/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3757 2023-05-11 11:41:56.000000 gbd_tools-4.5.8/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2023-05-11 11:41:56.000000 gbd_tools-4.5.8/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 11:41:56.000000 gbd_tools-4.5.8/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-11 11:41:56.000000 gbd_tools-4.5.8/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-11 11:41:56.000000 gbd_tools-4.5.8/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-11 11:41:56.000000 gbd_tools-4.5.8/gbd_tools.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.5.8/server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 11:41:56.882307 gbd_tools-4.5.8/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1034 2023-05-11 11:40:51.000000 gbd_tools-4.5.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.431838 gbd_tools-4.5.9/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.5.9/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.5.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-05-12 14:39:37.431838 gbd_tools-4.5.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.5.9/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    12709 2023-05-12 14:36:20.000000 gbd_tools-4.5.9/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.427838 gbd_tools-4.5.9/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.5.9/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10378 2023-05-12 14:36:28.000000 gbd_tools-4.5.9/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.5.9/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    10844 2023-05-12 14:34:38.000000 gbd_tools-4.5.9/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     6455 2023-05-10 11:45:07.000000 gbd_tools-4.5.9/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5461 2023-05-10 15:10:05.000000 gbd_tools-4.5.9/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12359 2023-04-25 15:02:02.000000 gbd_tools-4.5.9/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.5.9/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-05 18:48:49.000000 gbd_tools-4.5.9/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.427838 gbd_tools-4.5.9/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.5.9/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7756 2023-05-10 08:09:50.000000 gbd_tools-4.5.9/gbd_init/cnf_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.5.9/gbd_init/cnf_transformers.py
+-rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.5.9/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.5.9/gbd_init/initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.427838 gbd_tools-4.5.9/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.5.9/gbd_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.427838 gbd_tools-4.5.9/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.427838 gbd_tools-4.5.9/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.5.9/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.5.9/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.5.9/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.5.9/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.5.9/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.431838 gbd_tools-4.5.9/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.5.9/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.431838 gbd_tools-4.5.9/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-05-12 14:39:37.000000 gbd_tools-4.5.9/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      772 2023-05-12 14:39:37.000000 gbd_tools-4.5.9/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 14:39:37.000000 gbd_tools-4.5.9/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-12 14:39:37.000000 gbd_tools-4.5.9/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-12 14:39:37.000000 gbd_tools-4.5.9/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-12 14:39:37.000000 gbd_tools-4.5.9/gbd_tools.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    11998 2023-05-11 12:09:25.000000 gbd_tools-4.5.9/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 14:39:37.431838 gbd_tools-4.5.9/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1034 2023-05-12 14:38:56.000000 gbd_tools-4.5.9/setup.py
```

### Comparing `gbd_tools-4.5.8/LICENSE` & `gbd_tools-4.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/PKG-INFO` & `gbd_tools-4.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_tools
-Version: 4.5.8
+Version: 4.5.9
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.5.8/README.md` & `gbd_tools-4.5.9/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd.py` & `gbd_tools-4.5.9/gbd.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,20 +62,25 @@
     init_sani(api, args.context, rlimits, args.query, args.hashes, target_db=args.target_db)
 
 
 def cli_create(api: GBD, args):
     api.create_feature(args.name, args.unique, args.target_db)
 
 def cli_delete(api: GBD, args):
-    if args.hashes and len(args.hashes) > 0 or args.values and len(args.values):
+    if args.hashes and len(args.hashes) or args.values and len(args.values):
         if args.force or util.confirm("Delete attributes of given hashes and/or values from '{}'?".format(args.name)):
             api.reset_values(args.name, args.values, args.hashes)
     elif args.force or util.confirm("Delete feature '{}' and all associated attributes?".format(args.name)):
         api.delete_feature(args.name)
 
+def cli_cleanup(api: GBD, args):
+    if args.hashes and len(args.hashes):
+        if args.force or util.confirm("Delete attributes of given hashes from all features?"):
+            api.delete_hashes(args.hashes, args.target_db)
+
 def cli_rename(api: GBD, args):
     api.rename_feature(args.old_name, args.new_name)
 
 def cli_copy(api: GBD, args):
     api.copy_feature(args.old_name, args.new_name, args.target_db, args.query, args.hashes)
 
 
@@ -182,14 +187,20 @@
     parser_delete = subparsers.add_parser('delete', help='Delete all values assiociated with given hashes (via argument or stdin) or remove feature if no hashes are given')
     parser_delete.add_argument('--hashes', help='Hashes for which to delete values', nargs='*', default=[])
     parser_delete.add_argument('--values', help='Values to delete', nargs='*', default=[])
     parser_delete.add_argument('name', type=column_type, help='Name of feature')
     parser_delete.add_argument('-f', '--force', action='store_true', help='Do not ask for confirmation')
     parser_delete.set_defaults(func=cli_delete)
 
+    parser_cleanup = subparsers.add_parser('cleanup', help='Delete given hashes from all features')
+    parser_cleanup.add_argument('--hashes', help='Hashes for which to delete values', nargs='*', default=[])
+    parser_cleanup.add_argument('-f', '--force', action='store_true', help='Do not ask for confirmation')
+    parser_cleanup.add_argument('--target_db', help='Target database (default: first in list)', default=None)
+    parser_cleanup.set_defaults(func=cli_cleanup)
+
     parser_rename = subparsers.add_parser('rename', help='Rename feature')
     parser_rename.add_argument('old_name', type=column_type, help='Old name of feature')
     parser_rename.add_argument('new_name', type=column_type, help='New name of feature')
     parser_rename.set_defaults(func=cli_rename)
 
     parser_copy = subparsers.add_parser('copy', help='Copy feature')
     add_query_and_hashes_arguments(parser_copy)
```

### Comparing `gbd_tools-4.5.8/gbd_core/api.py` & `gbd_tools-4.5.9/gbd_core/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,14 +121,30 @@
             for values_slice in util.slice_iterator(values, 10):
                 self.database.delete(feature, values_slice, [], target_db)
         elif len(hashes):
             for hashes_slice in util.slice_iterator(hashes, 10):
                 self.database.delete(feature, [], hashes_slice, target_db)
 
 
+    def delete_hashes(self, hashes, target_db=None):
+        """ Delete all values for given hashes
+            
+            Args:
+                hashes (list): list of hashes (=benchmark ids) to be deleted
+                target_db (str, optional): name of target database
+                    if None, default database (first in list) is used
+
+            Raises:
+                GBDException, if feature does not exist
+        """
+        if not len(hashes):
+            raise GBDException("No hashes given")
+        self.database.delete_hashes_entirely(hashes, target_db)
+
+
     def get_databases(self):
         """ Get list of database names
 
             Returns: list of database names
         """
         return list(self.database.get_databases())
```

### Comparing `gbd_tools-4.5.8/gbd_core/contexts.py` & `gbd_tools-4.5.9/gbd_core/contexts.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_core/database.py` & `gbd_tools-4.5.9/gbd_core/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -252,13 +252,19 @@
             remaining = [ r[0] for r in self.query("SELECT DISTINCT(hash) FROM {d}.{tab} WHERE hash in ('{h}')".format(d=db, tab=fname, h="', '".join(hashlist))) ]
             setnone = [ h for h in hashlist if not h in remaining ]
             self.execute("UPDATE {d}.features SET {col} = 'None' WHERE hash IN ('{h}')".format(d=db, col=fname, h="', '".join(setnone)))
         else:
             self.execute("UPDATE {d}.features SET {col} = '{default}' WHERE {w}".format(d=db, col=fname, default=finfo.default, w=where))
 
 
+    def delete_hashes_entirely(self, hashes, target_db=None):
+        tables = self.get_tables([ target_db ])
+        for table in tables:
+            self.execute("DELETE FROM {}.{} WHERE hash IN ('{h}')".format(target_db, table, h="', '".join(hashes)))
+
+
     def copy_feature(self, old_name, new_name, target_db, hashlist=[]):
         old_finfo = self.finfo(old_name)
         data = self.query("SELECT hash, {col} FROM {d}.{tab} WHERE hash IN ('{h}')".format(d=old_finfo.database, col=old_finfo.column, tab=old_finfo.table, h="', '".join(hashlist)))
         for (hash, value) in data:
             self.set_values(new_name, value, [hash], target_db)
```

### Comparing `gbd_tools-4.5.8/gbd_core/grammar.py` & `gbd_tools-4.5.9/gbd_core/grammar.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_core/query.py` & `gbd_tools-4.5.9/gbd_core/query.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_core/schema.py` & `gbd_tools-4.5.9/gbd_core/schema.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_core/util.py` & `gbd_tools-4.5.9/gbd_core/util.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_core/util_argparse.py` & `gbd_tools-4.5.9/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_init/cnf_extractors.py` & `gbd_tools-4.5.9/gbd_init/cnf_extractors.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_init/cnf_transformers.py` & `gbd_tools-4.5.9/gbd_init/cnf_transformers.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_init/gbdhash.py` & `gbd_tools-4.5.9/gbd_init/gbdhash.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_init/initializer.py` & `gbd_tools-4.5.9/gbd_init/initializer.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.5.9/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.5.9/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.5.9/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_server/static/main.css` & `gbd_tools-4.5.9/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_server/static/w3.js` & `gbd_tools-4.5.9/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_server/templates/index.html` & `gbd_tools-4.5.9/gbd_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.5.9/gbd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-tools
-Version: 4.5.8
+Version: 4.5.9
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.5.8/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.5.9/gbd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.8/server.py` & `gbd_tools-4.5.9/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     return Response(json_blob, status=200, mimetype="application/json")
 
 def page_response(query, database, page=0):
     with GBD(app.config['database'], verbose=app.config['verbose']) as gbd:
         start = page * 1000
         end = start + 1000
         try:
-            df = gbd.query(query, resolve=app.config["features"][database], collapse="MIN")
+            df = gbd.query(query, resolve=app.config["features"][database], collapse="GROUP_CONCAT")
             #for col in df.columns:
             #    df[col] = df[col].apply(lambda x: round(float(x), 2) if util.is_number(x) and '.' in x else x)
         except (GBDException, DatabaseException, ParserException) as err:
             return error_response("{}, {}".format(type(err), str(err)), request.remote_addr, errno=500)
         return render_template('index.html', 
             query=query, 
             result=df.iloc[start:end, :].values.tolist(),
```

### Comparing `gbd_tools-4.5.8/setup.py` & `gbd_tools-4.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.5.8',
+  version='4.5.9',
   description='GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser, Karlsruhe Institute of Technology (KIT)',
   author_email='markus.iser@kit.edu',
   packages=[
```

