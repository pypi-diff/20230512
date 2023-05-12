# Comparing `tmp/kivalu-0.19.0.tar.gz` & `tmp/kivalu-0.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivalu-0.19.0.tar", last modified: Sat Apr  1 15:07:03 2023, max compression
+gzip compressed data, was "kivalu-0.21.0.tar", last modified: Fri May 12 17:59:40 2023, max compression
```

## Comparing `kivalu-0.19.0.tar` & `kivalu-0.21.0.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-01 15:07:03.020089 kivalu-0.19.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-04-01 08:32:07.000000 kivalu-0.19.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-04-01 15:07:03.020089 kivalu-0.19.0/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-01 15:07:03.020089 kivalu-0.19.0/kivalu/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11803 2023-04-01 11:40:08.000000 kivalu-0.19.0/kivalu/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-01 15:07:03.020089 kivalu-0.19.0/kivalu.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-04-01 15:07:02.000000 kivalu-0.19.0/kivalu.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      205 2023-04-01 15:07:03.000000 kivalu-0.19.0/kivalu.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-01 15:07:02.000000 kivalu-0.19.0/kivalu.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-04-01 15:07:02.000000 kivalu-0.19.0/kivalu.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-04-01 15:07:02.000000 kivalu-0.19.0/kivalu.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-01 15:07:03.020089 kivalu-0.19.0/scripts/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       52 2023-04-01 11:54:51.000000 kivalu-0.19.0/scripts/kivalu-setup
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-01 15:07:03.020089 kivalu-0.19.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-04-01 12:23:33.000000 kivalu-0.19.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 17:59:40.170964 kivalu-0.21.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-05-07 10:57:06.000000 kivalu-0.21.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-05-12 17:59:40.170964 kivalu-0.21.0/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 17:59:40.170964 kivalu-0.21.0/kivalu/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13449 2023-05-12 17:28:52.000000 kivalu-0.21.0/kivalu/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 17:59:40.170964 kivalu-0.21.0/kivalu.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-05-12 17:59:40.000000 kivalu-0.21.0/kivalu.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      295 2023-05-12 17:59:40.000000 kivalu-0.21.0/kivalu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-12 17:59:40.000000 kivalu-0.21.0/kivalu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-05-12 17:59:40.000000 kivalu-0.21.0/kivalu.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-05-12 17:59:40.000000 kivalu-0.21.0/kivalu.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 17:59:40.170964 kivalu-0.21.0/scripts/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       52 2023-05-07 10:57:06.000000 kivalu-0.21.0/scripts/kivalu-setup
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-12 17:59:40.170964 kivalu-0.21.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-05-12 17:47:08.000000 kivalu-0.21.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 17:59:40.170964 kivalu-0.21.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1100 2023-05-12 16:53:14.000000 kivalu-0.21.0/tests/test_argumentparser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8781 2023-05-12 17:28:52.000000 kivalu-0.21.0/tests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1017 2023-05-12 16:53:14.000000 kivalu-0.21.0/tests/test_main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2203 2023-05-07 10:57:06.000000 kivalu-0.21.0/tests/test_server.py
```

### Comparing `kivalu-0.19.0/LICENSE` & `kivalu-0.21.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kivalu-0.19.0/PKG-INFO` & `kivalu-0.21.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivalu
-Version: 0.19.0
+Version: 0.21.0
 Summary: Nested key-value system with built-in inheritance and templating, designed for configuration management
 Home-page: https://zebr0.io/projects/kivalu
 Download-URL: https://gitlab.com/zebr0/kivalu
 Author: Thomas JOUANNOT
 Author-email: mazerty@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kivalu-0.19.0/kivalu/__init__.py` & `kivalu-0.21.0/kivalu/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,99 +4,116 @@
 import http.server
 import json
 import threading
 from pathlib import Path
 from typing import List, Optional, Any
 
 import jinja2
+import requests.exceptions
 import requests_cache
 
 ENCODING = "utf-8"
 
 URL = "url"
+FAILOVER = "failover"
 LEVELS = "levels"
 EXTRA_VARS = "extra-vars"
+TIMEOUT = "timeout"
 CACHE = "cache"
 
 URL_DEFAULT = "https://hub.zebr0.io"
+FAILOVER_DEFAULT = ""
 LEVELS_DEFAULT = []
 EXTRA_VARS_DEFAULT = {}
+TIMEOUT_DEFAULT = 3.05  # see https://docs.python-requests.org/en/master/user/advanced/#timeouts
 CACHE_DEFAULT = 300
 CONFIGURATION_FILE_DEFAULT = Path("/etc/kivalu.conf")
 
 
 class Client:
     """
     Nested key-value system with built-in inheritance and templating, designed for configuration management.
 
     This Client can connect to any key-value server that follows HTTP REST standards.
-    For now it only supports plain text responses, JSON support is in the works.
+    For now, it only supports plain text responses, JSON support is in the works.
 
     Nested keys and inheritance:
     To fully exploit the Client, you should define a structure in the naming of your keys, like "<project>/<environment/<key>".
     Then use the "levels" parameter of the constructor to point to a specific project and environment, like ["mattermost", "production"].
-    Finally, use the get() function to fetch a key and it will automatically look for the most specific value possible.
+    Finally, use the get() function to fetch a key, and it will automatically look for the most specific value possible.
     Note that you don't have to duplicate keys for each project and environment, as they can be inherited from their parent level.
 
     Templating:
     By default, values are processed through the Jinja templating engine.
-    You can refer to the constructor parameters {{ url }}, {{ levels[x] }} or any given extra variable.
+    You can refer to the constructor parameters {{ url }}, {{ failover }}, {{ levels[x] }} or any given extra variable.
     You can also include the value from another key {{ "another-key" | get }} or the content of a file {{ "/path/to/the/file" | read }}.
     Visit https://jinja.palletsprojects.com to learn more about filters, blocks and other features of Jinja that you can use.
 
     Configuration file:
-    Client configuration can also be read from a JSON file, a simple dictionary with the "url", "levels", "extra_vars" and "cache" keys.
+    Client configuration can also be read from a JSON file.
     The save_configuration() function can help you create one from an existing Client.
     The suggested default path can be used for a system-wide configuration.
     If provided, constructor parameters will always supersede the values from the configuration file, which in turn supersede the default values.
 
     Note that the inheritance and templating mechanisms are performed by the client, to be as server-agnostic as possible.
 
     :param url: URL of the key-value server, defaults to https://hub.zebr0.io
+    :param failover: Failover URL in case there is a ConnectionError with the main URL, defaults to ""
     :param levels: levels of specialization (e.g. ["mattermost", "production"] for a <project>/<environment>/<key> structure), defaults to []
     :param extra_vars: dictionary that can be used to declare extra variables to the templating engine, defaults to {}
-    :param cache: in seconds, the duration of the cache of http responses, defaults to 300 seconds
+    :param timeout: in seconds, the duration of the timeout of http requests, defaults to 3.05
+    :param cache: in seconds, the duration of the cache of http responses, defaults to 300
     :param configuration_file: path to the configuration file, defaults to /etc/kivalu.conf for a system-wide configuration
     """
 
-    def __init__(self, *, url: str = None, levels: Optional[List[str]] = None, cache: int = None, extra_vars: dict = None, configuration_file: Path = CONFIGURATION_FILE_DEFAULT, **_) -> None:
+    def __init__(self, *, url: str = None, failover: str = None, levels: Optional[List[str]] = None, extra_vars: dict = None, timeout: float = None, cache: int = None, configuration_file: Path = CONFIGURATION_FILE_DEFAULT, **_) -> None:
         self.configuration_file = configuration_file
 
         # first set default values
         self.url = URL_DEFAULT
+        self.failover = FAILOVER_DEFAULT
         self.levels = LEVELS_DEFAULT
         self.extra_vars = EXTRA_VARS_DEFAULT
+        self.timeout = TIMEOUT_DEFAULT
         self.cache = CACHE_DEFAULT
 
         # then override with the configuration file if present
         try:
             configuration = json.loads(configuration_file.read_text(ENCODING))
 
             self.url = configuration.get(URL, URL_DEFAULT)
+            self.failover = configuration.get(FAILOVER, FAILOVER_DEFAULT)
             self.levels = configuration.get(LEVELS, LEVELS_DEFAULT)
             self.extra_vars = configuration.get(EXTRA_VARS, EXTRA_VARS_DEFAULT)
+            self.timeout = configuration.get(TIMEOUT, TIMEOUT_DEFAULT)
             self.cache = configuration.get(CACHE, CACHE_DEFAULT)
         except OSError:
             pass  # configuration file not found, ignored
 
         # finally override with the parameters if present
         if url is not None:
             self.url = url
+        if failover is not None:
+            self.failover = failover
         if levels is not None:
             self.levels = levels
         if extra_vars is not None:
             self.extra_vars = extra_vars
+        if timeout is not None:
+            self.timeout = timeout
         if cache is not None:
             self.cache = cache
 
         # templating setup
         self.jinja_environment = jinja2.Environment(keep_trailing_newline=True)
         self.jinja_environment.globals[URL] = self.url
+        self.jinja_environment.globals[FAILOVER] = self.failover
         self.jinja_environment.globals[LEVELS] = self.levels
         self.jinja_environment.globals.update(self.extra_vars)
+        self.jinja_environment.globals["configuration"] = json.dumps({URL: self.url, FAILOVER: self.failover, LEVELS: self.levels, EXTRA_VARS: self.extra_vars, TIMEOUT: self.timeout, CACHE: self.cache})
         self.jinja_environment.filters["get"] = self.get
         self.jinja_environment.filters["read"] = read
 
         # http requests setup
         self.http_session = requests_cache.CachedSession(backend="memory", expire_after=cache)
 
     def get(self, key: str, default: str = "", template: bool = True, strip: bool = True, extra_vars: dict = None) -> str:
@@ -111,15 +128,18 @@
         :param strip: shall the value be stripped off leading and trailing white spaces?
         :param extra_vars: dictionary that can be used to declare extra variables to the templating engine
         :return: the resulting value of the key
         """
 
         # let's do this with a nice recursive function :)
         def fetch(levels):
-            response = self.http_session.get("/".join([self.url] + levels + [key]))
+            try:
+                response = self.http_session.get("/".join([self.url] + levels + [key]), timeout=self.timeout)
+            except requests.exceptions.ConnectionError:  # basically a retry, either on the failover url or the main one
+                response = self.http_session.get("/".join([self.failover or self.url] + levels + [key]), timeout=self.timeout)
 
             if response.ok:
                 return response.text  # if the key is found, we return the value
             elif levels:
                 return fetch(levels[:-1])  # if not, we try at the parent level
             else:
                 return default  # if we're at the top level, the key just doesn't exist, we return the default value
@@ -132,16 +152,15 @@
         return value
 
     def save_configuration(self) -> None:
         """
         Saves the Client's configuration to a JSON file.
         """
 
-        configuration = {URL: self.url, LEVELS: self.levels, EXTRA_VARS: self.extra_vars, CACHE: self.cache}
-        self.configuration_file.write_text(json.dumps(configuration), ENCODING)
+        self.configuration_file.write_text(self.jinja_environment.globals["configuration"], ENCODING)
 
 
 class TestServer:
     """
     Rudimentary key-value HTTP server, for development or testing purposes only.
     The keys and their values are stored in a dictionary, that can be defined either in the constructor or through the "data" attribute.
     Access logs are also available through the "access_logs" attribute.
@@ -227,31 +246,38 @@
     :param kwargs: keyword arguments of the ArgumentParser constructor
     :return: the customized ArgumentParser
     """
 
     argparser = argparse.ArgumentParser(*args, **kwargs)
 
     class DictionaryAction(argparse.Action):
+        """
+        Argparse Action that combines the given arguments into a dictionary.
+        Must be used in conjunction with "nargs=2".
+        """
+
         def __call__(self, parser, namespace, values, option_string=...):
             dictionary = getattr(namespace, self.dest) or {}
             dictionary[values[0]] = values[1]
             setattr(namespace, self.dest, dictionary)
 
     argparser.add_argument("-u", "--url", help=f"URL of the key-value server, defaults to {URL_DEFAULT}", metavar="<url>")
-    argparser.add_argument("-l", "--levels", action="append", help=f'levels of specialization (e.g. "mattermost production" for a <project>/<environment>/<key> structure), defaults to {LEVELS_DEFAULT}', metavar="<level>")
+    argparser.add_argument("--failover", help='Failover URL in case there is a ConnectionError with the main URL, defaults to ""', metavar="<url>")
+    argparser.add_argument("-l", "--level", action="append", dest=LEVELS, help="level of specialization (e.g. project name, environment, etc.), can be specified multiple times", metavar="<level>")
     argparser.add_argument("-e", "--extra-vars", nargs=2, action=DictionaryAction, help="extra variable (key/value) for the templating engine, can be specified multiple times", metavar="<string>")
+    argparser.add_argument("-t", "--timeout", type=float, help=f"in seconds, the duration of the timeout of http requests, defaults to {TIMEOUT_DEFAULT}", metavar="<duration>")
     argparser.add_argument("-c", "--cache", type=int, help=f"in seconds, the duration of the cache of http responses, defaults to {CACHE_DEFAULT}", metavar="<duration>")
     argparser.add_argument("-f", "--configuration-file", type=Path, default=CONFIGURATION_FILE_DEFAULT, help=f"path to the configuration file, defaults to {CONFIGURATION_FILE_DEFAULT} for a system-wide configuration", metavar="<path>")
 
     return argparser
 
 
 def main(args: Optional[List[str]] = None) -> None:
     argparser = build_argument_parser(description="Saves kivalu's configuration in a JSON file.")
-    argparser.add_argument("-t", "--test", help="tests the configuration by fetching a key", metavar="<key>")
+    argparser.add_argument("--test", help="tests the configuration by fetching a key", metavar="<key>")
     args = argparser.parse_args(args)
 
     # creates a client from the given parameters, then saves the configuration
     client = Client(**vars(args))
     client.save_configuration()
 
     if args.test:
```

### Comparing `kivalu-0.19.0/kivalu.egg-info/PKG-INFO` & `kivalu-0.21.0/kivalu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivalu
-Version: 0.19.0
+Version: 0.21.0
 Summary: Nested key-value system with built-in inheritance and templating, designed for configuration management
 Home-page: https://zebr0.io/projects/kivalu
 Download-URL: https://gitlab.com/zebr0/kivalu
 Author: Thomas JOUANNOT
 Author-email: mazerty@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kivalu-0.19.0/setup.py` & `kivalu-0.21.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="kivalu",
-    version="0.19.0",
+    version="0.21.0",
     description="Nested key-value system with built-in inheritance and templating, designed for configuration management",
     long_description="TODO",
     long_description_content_type="text/markdown",
     author="Thomas JOUANNOT",
     author_email="mazerty@gmail.com",
     url="https://zebr0.io/projects/kivalu",
     download_url="https://gitlab.com/zebr0/kivalu",
```

