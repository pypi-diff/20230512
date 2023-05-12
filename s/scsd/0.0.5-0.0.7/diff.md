# Comparing `tmp/scsd-0.0.5.tar.gz` & `tmp/scsd-0.0.7.tar.gz`

## Comparing `scsd-0.0.5.tar` & `scsd-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scsd-0.0.5/Dockerfile
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scsd-0.0.5/requirements.txt
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 scsd-0.0.5/scsd
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scsd-0.0.5/scsd.conf.sample
--rw-r--r--   0        0        0    34178 2020-02-02 00:00:00.000000 scsd-0.0.5/test
--rw-r--r--   0        0        0    27749 2020-02-02 00:00:00.000000 scsd-0.0.5/test.html
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scsd-0.0.5/docker/cron-root
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/__init__.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/__main__.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/args.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/config.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/db.py
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/err.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/logger.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/notifier.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/parser.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/storage.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/web.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 scsd-0.0.5/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 scsd-0.0.5/LICENSE
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 scsd-0.0.5/README.md
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 scsd-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 scsd-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scsd-0.0.7/Dockerfile
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 scsd-0.0.7/requirements.txt
+-rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 scsd-0.0.7/scsd
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scsd-0.0.7/scsd.conf.sample
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 scsd-0.0.7/docker/cron-root
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/__init__.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/__main__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/args.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/auth.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/config.py
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/db.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/err.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/logger.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/notifier.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/parser.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/storage.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/web.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 scsd-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 scsd-0.0.7/LICENSE
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 scsd-0.0.7/README.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 scsd-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 scsd-0.0.7/PKG-INFO
```

### Comparing `scsd-0.0.5/steamCloudSaveDownloader/__main__.py` & `scsd-0.0.7/steamCloudSaveDownloader/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 from . import args
 from . import web
 from . import db
 from . import storage
+from .auth import auth
 from .err import err
 from .notifier import notifier
 from .config import config
 import logging
 import sys
+import os
 
 logger = None
 
 def __main__():
     logging.basicConfig(
         format='%(asctime)s [%(levelname)s] %(message)s',
         datefmt='%Y-%m-%d %H:%M:%S')
     global logger
     logger = logging.getLogger('scsd')
     try:
         notifier_ = None
         parsed_args = args.args().parse(sys.argv[1:])
 
+        if 'auth' in parsed_args and \
+                parsed_args['auth'] is not None and \
+                len(parsed_args['auth']) != 0:
+            print("Auth")
+            auth_ = auth(parsed_args['auth'], parsed_args['save_dir'])
+            exit(1)
+
         if parsed_args['conf'] is not None:
             parsed_args = config(parsed_args['conf']).get_conf()
 
         logger.setLevel(args.args.convert_log_level(parsed_args['log_level']))
         logger.debug(parsed_args)
 
         notifier_ = notifier.create_instance(
@@ -40,15 +49,15 @@
     end_msg = "Process ended noramlly"
     logger.info(end_msg)
     notifier_.send(end_msg, True)
     exit(0)
 
 def main(parsed_args):
 
-    web_ = web.web(parsed_args['cookie'])
+    web_ = web.web(os.path.join(parsed_args['save_dir'], 'session.sb'))
 
     db_ = db.db(parsed_args['save_dir'], parsed_args['rotation'])
     storage_ = storage.storage(parsed_args['save_dir'], db_)
 
     game_list = web_.get_list()
 
     for game in game_list:
@@ -76,15 +85,15 @@
                 )
             continue
 
         for file_info in file_infos:
             file_id = db_.get_file_id(game['app_id'], file_info['filename'])
             if (not db_.is_file_outdated(file_id, file_info['time'])):
                 continue
-            logger.info(f"Downloading {file_info['filename']}")
+            logger.info(f"  Downloading {file_info['filename']}")
             storage_.rotate_file(
                 game['app_id'],
                 file_info['filename'],
                 file_info['path'],
                 file_id)
             web_.download_game_save(
                 file_info['link'],
```

### Comparing `scsd-0.0.5/steamCloudSaveDownloader/args.py` & `scsd-0.0.7/steamCloudSaveDownloader/args.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,28 @@
         options, remainder = self.parser.parse_known_args()
 
         # Break if config file is given
         if options.conf is not None:
             return
 
         self.parser.add_argument(
+            "-a",
+            metavar="username",
+            type=str,
+            dest="auth",
+            help="Save authentication"
+        )
+
+
+        self.parser.add_argument(
             "-c",
             metavar="cookie_file",
             dest="cookie",
             type=argparse.FileType('r'),
-            required=True,
+            required=False,
             help="Netscape HTTP Cookie File of store.steampowered.com"
         )
 
         self.parser.add_argument(
             "-d",
             metavar="save_dir",
             dest="save_dir",
```

### Comparing `scsd-0.0.5/steamCloudSaveDownloader/config.py` & `scsd-0.0.7/steamCloudSaveDownloader/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import configparser
 import os
 import pathlib
 from .err import err
 from .err import err_enum
-from .notifier import notifier
+from .notifier import notifier, notify_method
 
 Defaults = {
     "rotation": 15,
     "log_level": 2,
     "notifier": "",
     "webhook": "",
 }
@@ -47,17 +47,14 @@
         self.parsed[entry] = Defaults[entry]
 
     def parse_required(self):
         if 'Required' not in self.parser:
             self.raise_err("No [Required] section found")
         required = self.parser['Required']
 
-        self.check_and_raise(required, 'cookie')
-        self.parsed['cookie'] = self.is_file(required['cookie'])
-
         self.check_and_raise(required, 'save_dir')
         self.parsed['save_dir'] = self.is_path(required['save_dir'])
 
     def parse_optional_section(self, p_section:str, p_entries:list):
         if p_section in self.parser:
             section = self.parser[p_section]
         else:
```

### Comparing `scsd-0.0.5/steamCloudSaveDownloader/db.py` & `scsd-0.0.7/steamCloudSaveDownloader/db.py`

 * *Files identical despite different names*

### Comparing `scsd-0.0.5/steamCloudSaveDownloader/err.py` & `scsd-0.0.7/steamCloudSaveDownloader/err.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     CANNOT_RETRIEVE_GAME_FILES = 3
     CANNOT_PARSE_GAME_FILES = 4
     CANNOT_INITIALIZE_DB = 5
     CANNOT_CREATE_DIRECTORY = 6
     INVALID_WEBHOOK_URL = 7
     INVALID_COOKIE_FORMAT = 8,
     INVALID_CONFIG = 9
+    LOGIN_FAIL = 10
 
 ERR_INFO = {
     err_enum.CANNOT_RETRIEVE_LIST: [
         logging.ERROR,
         "Cannot retrieve list from steam. Please make sure connected to Internet and cookie is valid."
     ],
     err_enum.CANNOT_PARSE_LIST: [
@@ -47,14 +48,18 @@
     err_enum.INVALID_COOKIE_FORMAT: [
         logging.ERROR,
         "Invalid cookie format. Should be Netscape format"
     ],
     err_enum.INVALID_CONFIG: [
         logging.ERROR,
         "Invalid config format: "
+    ],
+    err_enum.LOGIN_FAIL: [
+        logging.ERROR,
+        "Login fail, please try again"
     ]
 }
 
 
 class err(Exception):
     def log(self):
         msg = self.message
```

### Comparing `scsd-0.0.5/steamCloudSaveDownloader/notifier.py` & `scsd-0.0.7/steamCloudSaveDownloader/notifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     '''
     instance = None
 
     def get_enum(name:str):
         if name.lower() == 'discord':
             return notify_method.Discord
         else:
-            return None
+            return notify_method.Nop
 
     def is_supported(name:str):
         if len(name) == 0:
             return True
         enum_ = notifier.get_enum(name)
         if enum_ is None:
             return False
@@ -48,15 +48,17 @@
         method_enum = notifier.get_enum(method)
         notifier.instance = notifier(method_enum, **kwargs)
 
         return notifier.instance
 
     def __init__(self, method:notify_method, **kwargs):
         self.method = method
-        if (self.method == notify_method.Discord):
+        if (self.method == notify_method.Nop):
+            pass
+        elif (self.method == notify_method.Discord):
             assert 'webhook' in kwargs, 'Discord method requires webhook'
             self.webhook = kwargs['webhook']
 
             if len(self.webhook) == 0:
                 logger.error(err.get_msg(err_enum.INVALID_WEBHOOK_URL))
                 exit(1)
         else:
@@ -72,11 +74,13 @@
         else:
             actual_msg = f'[scsd-{__version__}] '
         if ok:
             actual_msg += ":white_check_mark: "
         else:
             actual_msg += ":x: "
         actual_msg += f' {msg}'
-        if self.method == notify_method.Discord:
+        if self.method == notify_method.Nop:
+            return
+        elif self.method == notify_method.Discord:
             self.discord_send(actual_msg)
         else:
             assert False
```

### Comparing `scsd-0.0.5/steamCloudSaveDownloader/parser.py` & `scsd-0.0.7/steamCloudSaveDownloader/parser.py`

 * *Files identical despite different names*

### Comparing `scsd-0.0.5/steamCloudSaveDownloader/storage.py` & `scsd-0.0.7/steamCloudSaveDownloader/storage.py`

 * *Files identical despite different names*

### Comparing `scsd-0.0.5/steamCloudSaveDownloader/web.py` & `scsd-0.0.7/steamCloudSaveDownloader/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from . import err
 from .err import err_enum
 from .parser import web_parser
 import requests
-from http.cookiejar import MozillaCookieJar
-import pickle # Remove After Mock
+import pickle
 import shutil
 import time
 import random
 
 g_dbg_mode = False
 g_web_acc_link = "https://store.steampowered.com/account/?l=english"
 g_web_link = "https://store.steampowered.com/account/remotestorage/?l=english"
@@ -18,23 +17,22 @@
         if not g_dbg_mode:
             time.sleep(random.randint(g_random_sleep_interval[0], g_random_sleep_interval[1]))
         return func(*args, **kwargs)
     return wrapper
 
 class web:
     def __init__(self, cookie):
-        self.cookie_file = cookie
-        self.cookies = MozillaCookieJar(self.cookie_file)
+        self.web_parser = web_parser()
+        self.session = requests.Session()
+        self.cookie_pkl = cookie
         try:
-            self.cookies.load()
+            with open(self.cookie_pkl, 'rb') as f:
+                self.session.cookies.update(pickle.load(f))
         except:
             raise err.err(err_enum.INVALID_COOKIE_FORMAT)
-        self.web_parser = web_parser()
-        self.session = requests.Session()
-        self.session.cookies = self.cookies
 
         response = self.session.get(g_web_acc_link)
 
     # Return list of {"Game": name, "Link", link}
     @random_sleep
     def get_list(self):
         response = None
```

### Comparing `scsd-0.0.5/.gitignore` & `scsd-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `scsd-0.0.5/LICENSE` & `scsd-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scsd-0.0.5/README.md` & `scsd-0.0.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -35,7 +35,8 @@
 ### CI
 - Gen executable for linux/windows
 
 ### Misc
 - Banners
 
 ### Logger
+100,000 Limit
```

### Comparing `scsd-0.0.5/pyproject.toml` & `scsd-0.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['hatchling', 'hatch-requirements-txt']
 build-backend = "hatchling.build"
 
 [project]
 name = "scsd"
-version = "0.0.5"
+version = "0.0.7"
 authors = [
   { name="hchsu"}
 ]
 description = "Steam Cloud Save Downloader"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `scsd-0.0.5/PKG-INFO` & `scsd-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: scsd
-Version: 0.0.5
+Version: 0.0.7
 Summary: Steam Cloud Save Downloader
 Project-URL: Homepage, https://github.com/hhhhhojeihsu/steamCloudSaveDownloader
 Project-URL: Bug Tracker, https://github.com/hhhhhojeihsu/steamCloudSaveDownloader/issues
 Author: hchsu
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: beautifulsoup4<5,>=4.12.2
 Requires-Dist: discord-webhook<2,>=1.1.0
 Requires-Dist: requests<3,>=2.28.2
+Requires-Dist: steam<2,>=1.4.4
 Description-Content-Type: text/markdown
 
 # steamCloudSaveDownloader
 Download Save on Steam Cloud
 
 ## Early Stage Prototype: DO NOT USE
 
@@ -52,7 +53,8 @@
 ### CI
 - Gen executable for linux/windows
 
 ### Misc
 - Banners
 
 ### Logger
+100,000 Limit
```

