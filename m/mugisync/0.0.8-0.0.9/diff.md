# Comparing `tmp/mugisync-0.0.8-py3-none-any.whl.zip` & `tmp/mugisync-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5458 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     9332 b- defN 22-Sep-01 10:48 mugisync/__init__.py
+Zip file size: 5748 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat    10587 b- defN 22-Sep-08 09:46 mugisync/__init__.py
 -rw-rw-rw-  2.0 fat       60 b- defN 21-May-18 09:17 mugisync/__main__.py
--rw-rw-rw-  2.0 fat     1095 b- defN 22-Sep-01 10:50 mugisync-0.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1045 b- defN 22-Sep-01 10:50 mugisync-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Sep-01 10:50 mugisync-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       44 b- defN 22-Sep-01 10:50 mugisync-0.0.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 22-Sep-01 10:50 mugisync-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      638 b- defN 22-Sep-01 10:50 mugisync-0.0.8.dist-info/RECORD
-8 files, 12315 bytes uncompressed, 4338 bytes compressed:  64.8%
+-rw-rw-rw-  2.0 fat     1095 b- defN 22-Sep-08 09:48 mugisync-0.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1045 b- defN 22-Sep-08 09:48 mugisync-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Sep-08 09:48 mugisync-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       44 b- defN 22-Sep-08 09:48 mugisync-0.0.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 22-Sep-08 09:48 mugisync-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      639 b- defN 22-Sep-08 09:48 mugisync-0.0.9.dist-info/RECORD
+8 files, 13571 bytes uncompressed, 4628 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: mugisync/__init__.py
 Comment: 
 
 Filename: mugisync/__main__.py
 Comment: 
 
-Filename: mugisync-0.0.8.dist-info/LICENSE
+Filename: mugisync-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: mugisync-0.0.8.dist-info/METADATA
+Filename: mugisync-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: mugisync-0.0.8.dist-info/WHEEL
+Filename: mugisync-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: mugisync-0.0.8.dist-info/entry_points.txt
+Filename: mugisync-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: mugisync-0.0.8.dist-info/top_level.txt
+Filename: mugisync-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: mugisync-0.0.8.dist-info/RECORD
+Filename: mugisync-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mugisync/__init__.py

```diff
@@ -5,14 +5,21 @@
 import shutil
 import datetime
 from dataclasses import dataclass
 import argparse
 import re
 import paramiko
 
+# set DEBUG_MUGISYNC=1
+# DEBUG_MUGISYNC=1
+if 'DEBUG_MUGISYNC' in os.environ and os.environ['DEBUG_MUGISYNC'] == "1":
+    debug_print = print
+else:
+    debug_print = lambda *args, **kwargs: None
+
 @dataclass
 class MainArgs:
     src: str
     dst: str
     include: list = None
     exclude: list = None
     short_log: bool = False
@@ -168,58 +175,84 @@
             ok = ok and copy_to_dst(src, dst, logger)
             if ok:
                 logger.print_copied(src, dst)
             else:
                 logger.print_info("Rescheduling {}".format(src))
             return ok
 
+ALGORITHMS = ['ecdsa','ed25519','rsa','dsa']
+
 def main(*main_args):
     
     colorama_init()
 
     example_text = """examples:
-    mugisync /path/to/src /path/to/dst -i "*.cpp" -e "moc_*" ".git"
-    mugisync /src/path/libfoo.dll /dst/path
-    mugisync /path/to/src root@192.168.0.1:/root/src
+  mugisync /path/to/src /path/to/dst -i "*.cpp" -e "moc_*" ".git"
+  mugisync /src/path/libfoo.dll /dst/path
+  mugisync /path/to/src root@192.168.0.1:/root/src
     """
 
-    parser = argparse.ArgumentParser(prog="mugi-sync", epilog=example_text, formatter_class=argparse.RawDescriptionHelpFormatter)
+    parser = argparse.ArgumentParser(prog="mugisync", epilog=example_text, formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('src', help="source directory or file")
     parser.add_argument('dst', help="destination directory or file (or remote path)")
     parser.add_argument('-i','--include', nargs='+', help="include globs")
     parser.add_argument('-e','--exclude', nargs='+', help="exclude globs")
     parser.add_argument('-c','--create', action='store_true', help="create target directory")
-    parser.add_argument('-p', '--password', help='ssh password')
-    parser.add_argument('-k','--key', help='path to ssh key file, defaults to ~/.ssh/id_rsa if no password provided')
+    parser.add_argument('-P', '--password', help='ssh password')
+    parser.add_argument('-k','--key', help='path to ssh key file, if no password provided tries to find ssh key with common name in ~/.ssh')
+    parser.add_argument('-a', '--algorithm', choices=ALGORITHMS, help='ssh key algorithm')
 
     if len(main_args) == 2:
         args = MainArgs(*main_args)
     else:
         args = parser.parse_args()
+    
+    debug_print(args)
 
     m = re.match('(.+)@(.+):(.+)', args.dst)
     sftp_mode = m is not None
 
-    print('sftp_mode',sftp_mode)
+    #print('sftp_mode',sftp_mode)
+
+    logger = Logger(args.src, args.dst)
 
     sshArgs = None
+    key = None
     if sftp_mode:
-        if args.password is None and args.key is None:
-            key = os.path.join(os.path.expanduser('~'),'.ssh','id_rsa')
-        else:
+        if args.key:
             key = args.key
+            if os.path.exists(key):
+                debug_print('ssh key found {}'.format(key))
+            else:
+                logger.print_error('{} not exist'.format(key))
+                key = None
+        elif args.algorithm:
+            key = os.path.join(os.path.expanduser('~'),'.ssh','id_{}'.format(args.algorithm))
+            if os.path.exists(key):
+                debug_print('ssh key found {}'.format(key))
+            else:
+                logger.print_error('{} not exist'.format(key))
+                key = None
+        elif args.password is None:
+            for name in ALGORITHMS:
+                key = os.path.join(os.path.expanduser('~'),'.ssh','id_{}'.format(name))
+                if os.path.exists(key):
+                    debug_print('ssh key found {}'.format(key))
+                    break
+            else:
+                key = None
+                logger.print_error('no ssh key found and no password provided')
+    
         user = m.group(1)
         host = m.group(2)
         dst = m.group(3)
         sshArgs = SshArgs(host=host, user=user, password=args.password, key=key, src=args.src, dst=dst)
     
     #print(args); exit(0)
 
-    logger = Logger(args.src, args.dst)
-
     if sshArgs is None and args.create:
         makedirs(args.dst)
         if not os.path.isdir(args.dst):
             logger.print_error("Failed to create {}".format(args.dst))
             return
 
     if sshArgs is None and os.path.isdir(args.src) and os.path.isfile(args.dst):
```

## Comparing `mugisync-0.0.8.dist-info/LICENSE` & `mugisync-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mugisync-0.0.8.dist-info/METADATA` & `mugisync-0.0.9.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mugisync
-Version: 0.0.8
-Summary: Continously syncronizes local directory with another local or shared directory (poor person's syncthing) or remote directory over ssh (poor person's one way sshfs)
+Version: 0.0.9
+Summary: Continously syncronizes local directory with another local or shared directory (poor person's syncthing) or remote directory over ssh (poor person's one-way sshfs)
 Home-page: https://github.com/mugiseyebrows/mugi-sync
 Author: Stanislav Doronin
 Author-email: mugisbrows@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Dist: eventloop
 Requires-Dist: colorama
 Requires-Dist: paramiko
 
 
 # mugisync
 
-Continously syncronizes local directory with another local or shared directory (poor person's syncthing) or remote directory over ssh (poor person's one way sshfs).
+Continously syncronizes local directory with another local or shared directory (poor person's syncthing) or remote directory over ssh (poor person's one-way sshfs).
 
 ## Installing
 
 Mugisync can be installed via pip as follows:
 
 ```bash
 pip install mugisync
```

