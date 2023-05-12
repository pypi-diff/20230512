# Comparing `tmp/hoyo-daily-logins-helper-2.1.0.tar.gz` & `tmp/hoyo-daily-logins-helper-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-2.1.0.tar", last modified: Wed May 10 03:53:56 2023, max compression
+gzip compressed data, was "hoyo-daily-logins-helper-2.2.0.tar", last modified: Fri May 12 03:43:10 2023, max compression
```

## Comparing `hoyo-daily-logins-helper-2.1.0.tar` & `hoyo-daily-logins-helper-2.2.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:56.154625 hoyo-daily-logins-helper-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:56.150625 hoyo-daily-logins-helper-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:56.150625 hoyo-daily-logins-helper-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-10 03:53:56.154625 hoyo-daily-logins-helper-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/hoyo-daily-logins-helper.toml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:56.150625 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:53:56.154625 hoyo-daily-logins-helper-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:56.150625 hoyo-daily-logins-helper-2.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/src/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/src/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/src/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/hoyo-daily-logins-helper.toml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/src/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/scheduler.py
```

### Comparing `hoyo-daily-logins-helper-2.1.0/.github/workflows/tests.yml` & `hoyo-daily-logins-helper-2.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.1.0/.gitignore` & `hoyo-daily-logins-helper-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.1.0/LICENSE` & `hoyo-daily-logins-helper-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.1.0/PKG-INFO` & `hoyo-daily-logins-helper-2.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.1.0
+Version: 2.2.0
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -135,12 +135,50 @@
 
 [[accounts]]
 identifier = "My Starrail Account #2"
 game = "starrail"
 cookie = "My Starrail Cookie..."
 ```
 
+## Scheduler mode
+
+Scheduler mode can only be used if you are working with a configuration file. To
+enable the scheduler mode, set ``enable_scheduler = true`` in the `config` section.
+
+```toml
+[config]
+# ...
+enable_scheduler = true
+
+[[accounts]]
+# ....
+```
+
+This feature also requires you to set account regions which you can do like this:
+
+```toml
+[config]
+# ...
+enable_scheduler = true
+region = "EU"
+
+[[accounts]]
+identifier = "My Starrail Account #1"
+game = "starrail"
+cookie = "My Starrail Cookie..."
+# this account is in the EU region and we set this as the default so you dont have to do anything
+
+[[accounts]]
+identifier = "My Starrail Account #2"
+game = "starrail"
+cookie = "My Starrail Cookie..."
+# this account is in a different region so you have to explicitly overwrite this
+region = "Asia"
+```
+
+If you are not setting the regions properly the scheduler will run at the wrong time.
+
 ## License
 
 GNU General Public License v3
 
 ![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.1.0/README.md` & `hoyo-daily-logins-helper-2.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -124,12 +124,50 @@
 
 [[accounts]]
 identifier = "My Starrail Account #2"
 game = "starrail"
 cookie = "My Starrail Cookie..."
 ```
 
+## Scheduler mode
+
+Scheduler mode can only be used if you are working with a configuration file. To
+enable the scheduler mode, set ``enable_scheduler = true`` in the `config` section.
+
+```toml
+[config]
+# ...
+enable_scheduler = true
+
+[[accounts]]
+# ....
+```
+
+This feature also requires you to set account regions which you can do like this:
+
+```toml
+[config]
+# ...
+enable_scheduler = true
+region = "EU"
+
+[[accounts]]
+identifier = "My Starrail Account #1"
+game = "starrail"
+cookie = "My Starrail Cookie..."
+# this account is in the EU region and we set this as the default so you dont have to do anything
+
+[[accounts]]
+identifier = "My Starrail Account #2"
+game = "starrail"
+cookie = "My Starrail Cookie..."
+# this account is in a different region so you have to explicitly overwrite this
+region = "Asia"
+```
+
+If you are not setting the regions properly the scheduler will run at the wrong time.
+
 ## License
 
 GNU General Public License v3
 
 ![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.1.0/hoyo-daily-logins-helper.toml.template` & `hoyo-daily-logins-helper-2.2.0/hoyo-daily-logins-helper.toml.template`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/PKG-INFO` & `hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.1.0
+Version: 2.2.0
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -135,12 +135,50 @@
 
 [[accounts]]
 identifier = "My Starrail Account #2"
 game = "starrail"
 cookie = "My Starrail Cookie..."
 ```
 
+## Scheduler mode
+
+Scheduler mode can only be used if you are working with a configuration file. To
+enable the scheduler mode, set ``enable_scheduler = true`` in the `config` section.
+
+```toml
+[config]
+# ...
+enable_scheduler = true
+
+[[accounts]]
+# ....
+```
+
+This feature also requires you to set account regions which you can do like this:
+
+```toml
+[config]
+# ...
+enable_scheduler = true
+region = "EU"
+
+[[accounts]]
+identifier = "My Starrail Account #1"
+game = "starrail"
+cookie = "My Starrail Cookie..."
+# this account is in the EU region and we set this as the default so you dont have to do anything
+
+[[accounts]]
+identifier = "My Starrail Account #2"
+game = "starrail"
+cookie = "My Starrail Cookie..."
+# this account is in a different region so you have to explicitly overwrite this
+region = "Asia"
+```
+
+If you are not setting the regions properly the scheduler will run at the wrong time.
+
 ## License
 
 GNU General Public License v3
 
 ![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt` & `hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 .gitignore
 Dockerfile
 LICENSE
 Makefile
 README.md
 hoyo-daily-logins-helper.toml.template
 pyproject.toml
+requirements.txt
 setup.py
 .github/workflows/deploy.yml
 .github/workflows/tests.yml
 hoyo_daily_logins_helper.egg-info/PKG-INFO
 hoyo_daily_logins_helper.egg-info/SOURCES.txt
 hoyo_daily_logins_helper.egg-info/dependency_links.txt
 hoyo_daily_logins_helper.egg-info/entry_points.txt
 hoyo_daily_logins_helper.egg-info/requires.txt
 hoyo_daily_logins_helper.egg-info/top_level.txt
 src/__init__.py
 src/__main__.py
 src/_version.py
+src/consts.py
 src/games.py
 src/http.py
-src/main.py
+src/main.py
+src/scheduler.py
```

### Comparing `hoyo-daily-logins-helper-2.1.0/pyproject.toml` & `hoyo-daily-logins-helper-2.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 keywords = ["genshin", "genshin-impact", "starrail", "honkai-starrail", "game"]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
 dependencies = [
     "requests",
     "comboparse",
+    "pytz",
+    "apscheduler",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 hoyo-daily-logins-helper = "src.main:main"
 
 [tool.setuptools]
```

### Comparing `hoyo-daily-logins-helper-2.1.0/src/games.py` & `hoyo-daily-logins-helper-2.2.0/src/games.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.1.0/src/http.py` & `hoyo-daily-logins-helper-2.2.0/src/http.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.1.0/src/main.py` & `hoyo-daily-logins-helper-2.2.0/src/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import sys
 import tomllib
 from pathlib import Path
 
 import comboparse
 
 from src._version import __version__
+from src.consts import DEFAULT_LANGUAGE
 from src.games import GAMES, game_perform_checkin
 from src.http import http_set_user_agent
-
-_DEFAULT_LANGUAGE = "en-us"
+from src.scheduler import run_scheduler
 
 
 def main():
     """ Main function for CLI """
     cli_args = list(sys.argv[1:])
     default_file = Path("hoyo-daily-logins-helper.toml")
 
@@ -79,15 +79,15 @@
         help="run the requests against the API with a different user agent",
         action="store",
     )
 
     parser.add_argument(
         "--language",
         help="return results in a different language",
-        default=_DEFAULT_LANGUAGE,
+        default=DEFAULT_LANGUAGE,
     )
 
     parser.add_argument(
         "--config-file",
         help="use TOML config file for account configuration",
         action="store",
     )
@@ -125,49 +125,50 @@
         if "LANGUAGE" in os.environ:
             args.language = os.environ["LANGUAGE"]
         if "COOKIE" in os.environ:
             args.cookie = [os.environ["COOKIE"]]
         if "GAME" in os.environ:
             args.game = [os.environ["GAME"]]
 
+    enable_scheduler = False
     account_identifiers = [None for _ in args.game]
 
     if args.config_file:
         logging.info(f"Found config file at: {args.config_file}")
 
         with open(args.config_file, "rb") as file:
-            data = tomllib.load(file)
+            config_data = tomllib.load(file)
 
             # parse config from toml file
-            debug_mode = data.get("config", {}).get("debug", None)
-
-            if debug_mode:
-                args.debug = True
-
-            language = data.get("config", {}).get("language", None)
+            language = config_data.get("config", {}).get("language", None)
 
             if language:
                 args.language = language
 
-            user_agent = data.get("config", {}).get("user-agent", None)
+            user_agent = config_data.get("config", {}).get("user-agent", None)
 
             if user_agent:
                 args.user_agent = user_agent
 
+            enable_scheduler = config_data.get("config", {})\
+                .get("enable_scheduler", False)
+
             # parse accounts
-            for index, account in enumerate(data.get("accounts", [])):
+            for index, account in enumerate(config_data.get("accounts", [])):
                 game = account.get("game", None)
                 cookie = account.get("cookie", None)
 
                 if not game:
                     logging.error(f"account #{index} has no game selected")
                     continue
 
                 if game not in GAMES:
-                    logging.error(f"account #{index} has invalid game '{game}' set")
+                    logging.error(
+                        f"account #{index} has invalid game '{game}' set"
+                    )
                     continue
 
                 if not cookie:
                     logging.error(f"account #{index} has no cookie set")
                     continue
 
                 account_identifiers.append(account.get("identifier", None))
@@ -180,14 +181,18 @@
             f"games ({len(args.game)}) does not match"
         )
         exit(1)
 
     if args.user_agent:
         http_set_user_agent(args.user_agent)
 
+    if enable_scheduler:
+        run_scheduler(config_data, args.language)
+        return
+
     for index, game in enumerate(args.game):
         identifier = f"Account #{index}"
         cookie = args.cookie[index]
 
         if account_identifiers[index]:
             identifier = account_identifiers[index]
```

