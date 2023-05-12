# Comparing `tmp/yokkaichi-1.3.1.tar.gz` & `tmp/yokkaichi-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yokkaichi-1.3.1.tar", last modified: Mon Apr 24 19:14:03 2023, max compression
+gzip compressed data, was "yokkaichi-1.4.1.tar", last modified: Fri May 12 19:45:41 2023, max compression
```

## Comparing `yokkaichi-1.3.1.tar` & `yokkaichi-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-04-24 19:14:03.005697 yokkaichi-1.3.1/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.3.1/LICENSE.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2712 2023-04-24 19:14:03.005697 yokkaichi-1.3.1/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1954 2023-03-10 22:19:25.000000 yokkaichi-1.3.1/README.md
--rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-04-24 19:14:03.005697 yokkaichi-1.3.1/setup.cfg
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1389 2023-04-09 23:36:24.000000 yokkaichi-1.3.1/setup.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-04-24 19:14:03.005697 yokkaichi-1.3.1/yokkaichi/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2967 2023-04-09 23:36:24.000000 yokkaichi-1.3.1/yokkaichi/MasscanScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     6520 2023-04-24 19:13:21.000000 yokkaichi-1.3.1/yokkaichi/ServerScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-01-14 23:17:48.000000 yokkaichi-1.3.1/yokkaichi/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     7971 2023-04-09 23:36:24.000000 yokkaichi-1.3.1/yokkaichi/__main__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-04-24 19:13:21.000000 yokkaichi-1.3.1/yokkaichi/_version.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       54 2023-04-09 23:36:24.000000 yokkaichi-1.3.1/yokkaichi/rich_console.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-04-24 19:14:03.005697 yokkaichi-1.3.1/yokkaichi.egg-info/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2712 2023-04-24 19:14:02.000000 yokkaichi-1.3.1/yokkaichi.egg-info/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)      335 2023-04-24 19:14:02.000000 yokkaichi-1.3.1/yokkaichi.egg-info/SOURCES.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-04-24 19:14:02.000000 yokkaichi-1.3.1/yokkaichi.egg-info/dependency_links.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       50 2023-04-24 19:14:02.000000 yokkaichi-1.3.1/yokkaichi.egg-info/requires.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-04-24 19:14:02.000000 yokkaichi-1.3.1/yokkaichi.egg-info/top_level.txt
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-12 19:45:41.444591 yokkaichi-1.4.1/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.4.1/LICENSE.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-12 19:45:41.444591 yokkaichi-1.4.1/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2252 2023-05-12 19:27:27.000000 yokkaichi-1.4.1/README.md
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-05-12 19:45:41.444591 yokkaichi-1.4.1/setup.cfg
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1529 2023-05-12 19:42:32.000000 yokkaichi-1.4.1/setup.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-12 19:45:41.444591 yokkaichi-1.4.1/yokkaichi/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2921 2023-05-12 18:51:44.000000 yokkaichi-1.4.1/yokkaichi/MasscanScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     6071 2023-05-12 18:51:44.000000 yokkaichi-1.4.1/yokkaichi/ServerScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-05-12 19:42:32.000000 yokkaichi-1.4.1/yokkaichi/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     8205 2023-05-12 19:42:32.000000 yokkaichi-1.4.1/yokkaichi/__main__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1261 2023-05-12 18:51:44.000000 yokkaichi-1.4.1/yokkaichi/args_to_cfg.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3874 2023-05-12 18:51:44.000000 yokkaichi-1.4.1/yokkaichi/config_loader.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1160 2023-05-12 18:51:44.000000 yokkaichi-1.4.1/yokkaichi/port_parser.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-12 19:45:41.444591 yokkaichi-1.4.1/yokkaichi.egg-info/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-12 19:45:41.000000 yokkaichi-1.4.1/yokkaichi.egg-info/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      364 2023-05-12 19:45:41.000000 yokkaichi-1.4.1/yokkaichi.egg-info/SOURCES.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-05-12 19:45:41.000000 yokkaichi-1.4.1/yokkaichi.egg-info/dependency_links.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       91 2023-05-12 19:45:41.000000 yokkaichi-1.4.1/yokkaichi.egg-info/requires.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-05-12 19:45:41.000000 yokkaichi-1.4.1/yokkaichi.egg-info/top_level.txt
```

### Comparing `yokkaichi-1.3.1/LICENSE.txt` & `yokkaichi-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.3.1/PKG-INFO` & `yokkaichi-1.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.3.1
+Version: 1.4.1
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
+License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -30,28 +31,29 @@
 - Query integration
 
 ### Planned features (not in a specific order)
 - WWW interface
 - Bot joining the servers
 - Cleaning up the code
 - Docker support
+- Optimization
+- Scanning for pre-Netty (<1.7) servers
 
 ### Installation
 - Easy installation (from PyPI)
 ```
 pip install yokkaichi
 ```
 - Manual installation (from git)
 ```
 git clone https://github.com/Oreeeee/yokkaichi
 cd yokkaichi
 pip install .
 ```
 
 ### Usage
-You can use this script by invoking `python -m yokkaichi` and passing in arguments in the CLI. You can get the list of availible options by invoking `python -m yokkaichi -h`
+1. Using a config file
+Instead of passing in arguments, you can pass the configuration file with `--config` argument. When no additional file name is provided, Yokkaichi will use `yokkaichi.toml` for the file name. When the config file name you provided doesn't exist, Yokkaichi will create an example file for you. Modify it how you like and rerun Yokkaichi. Configuration files are not forwards or backwards compatible and you will have to adjust it every major change. 
+2. You can also use this script by passing in arguments in the CLI. You can get the list of availible options by invoking `python -m yokkaichi -h`.
 
 ### Using the masscan integration
 You need to have [masscan](https://github.com/robertdavidgraham/masscan) in your PATH, or in the same directory from which you are running this software. Make sure that the binary is named `masscan` (Unix) or `masscan.exe` (Windows).
-
-### Example
-`python -m yokkaichi --java --masscan --masscan-countries US CA CN -p "25560-25569,34000,19843" --ip2location-db data/IP2LOCATION-LITE-DB11.BIN --ip2location-cache --output data/servers.json`
```

### Comparing `yokkaichi-1.3.1/README.md` & `yokkaichi-1.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,28 +11,29 @@
 - Query integration
 
 ### Planned features (not in a specific order)
 - WWW interface
 - Bot joining the servers
 - Cleaning up the code
 - Docker support
+- Optimization
+- Scanning for pre-Netty (<1.7) servers
 
 ### Installation
 - Easy installation (from PyPI)
 ```
 pip install yokkaichi
 ```
 - Manual installation (from git)
 ```
 git clone https://github.com/Oreeeee/yokkaichi
 cd yokkaichi
 pip install .
 ```
 
 ### Usage
-You can use this script by invoking `python -m yokkaichi` and passing in arguments in the CLI. You can get the list of availible options by invoking `python -m yokkaichi -h`
+1. Using a config file
+Instead of passing in arguments, you can pass the configuration file with `--config` argument. When no additional file name is provided, Yokkaichi will use `yokkaichi.toml` for the file name. When the config file name you provided doesn't exist, Yokkaichi will create an example file for you. Modify it how you like and rerun Yokkaichi. Configuration files are not forwards or backwards compatible and you will have to adjust it every major change. 
+2. You can also use this script by passing in arguments in the CLI. You can get the list of availible options by invoking `python -m yokkaichi -h`.
 
 ### Using the masscan integration
 You need to have [masscan](https://github.com/robertdavidgraham/masscan) in your PATH, or in the same directory from which you are running this software. Make sure that the binary is named `masscan` (Unix) or `masscan.exe` (Windows).
-
-### Example
-`python -m yokkaichi --java --masscan --masscan-countries US CA CN -p "25560-25569,34000,19843" --ip2location-db data/IP2LOCATION-LITE-DB11.BIN --ip2location-cache --output data/servers.json`
```

### Comparing `yokkaichi-1.3.1/setup.py` & `yokkaichi-1.4.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,38 @@
+from yokkaichi import __version__ as yokkaichi_ver
 from setuptools import setup
 from pathlib import Path
+import sys
 
 # Load README from README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-# Get version from yokkaichi/_version.py
-with open("yokkaichi/_version.py", "r") as f:
-    file_contents = f.read().strip()
-    no_var_name = file_contents.replace("__version__ = ", "")
-    version = no_var_name.replace('"', "")
+# Enforce Python version (3.7+)
+if sys.version_info[1] < 7:
+    sys.exit(
+        "Yokkaichi will NOT run on Python 3.6 and older. You can build the package yourself and remove the check, but don't report bugs that happen!"
+    )
 
 setup(
     name="yokkaichi",
-    version=version,
+    version=yokkaichi_ver,
     description="Shodan-like server scanner for Minecraft (formely mcserverscanner)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Oreeeee",
+    license="MIT",
     url="https://github.com/Oreeeee/yokkaichi",
     install_requires=[
         "rich",
         "mcstatus",
         "ip2location",
         "python-masscan",
         "requests",
+        'tomli >= 1.1.0 ; python_version < "3.11"',
     ],
     classifiers=[
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
```

### Comparing `yokkaichi-1.3.1/yokkaichi/MasscanScan.py` & `yokkaichi-1.4.1/yokkaichi/MasscanScan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from .rich_console import console
+from .constants.rich_console import console
 from pathlib import Path
 import platform
 import masscan
 import json
 
 
 class MasscanScan:
-    def __init__(self, ip_list, port_list, masscan_args, masscan_output):
+    def __init__(self, cfg, ip_list):
         # Declare variables
+        self.cfg = cfg
         self.ip_list = ip_list
-        self.port_list = port_list
-        self.masscan_args = masscan_args
-        self.masscan_output = masscan_output
 
         # Create masscan object
         self.mas = masscan.PortScanner()
 
         # Convert IP and port list to masscan friendly format
         self.mas_ip_list = self.convert_ip_list()
         self.mas_port_list = self.convert_port_list()
@@ -29,50 +27,52 @@
         # Remove the first space
         mas_ip_list = mas_ip_list[1:]
 
         return mas_ip_list
 
     def convert_port_list(self):
         mas_port_list = ""
-        for port in self.port_list:
+        for port in self.cfg.ports:
             # Add a comma every port in the list
             mas_port_list += f",{port}"
 
         # Remove the first comma
         mas_port_list = mas_port_list[1:]
 
         return mas_port_list
 
     def save_output(self, masscan_results):
-        Path(self.masscan_output).touch()
-        with open(self.masscan_output, "w") as f:
+        Path(self.cfg.masscan_output_location).touch()
+        with open(self.cfg.masscan_output_location, "w") as f:
             f.write(json.dumps(masscan_results, indent=4))
         console.print(
-            f"Saved masscan results to [bold cyan]{self.masscan_output}[/bold cyan]",
+            f"Saved masscan results to [bold cyan]{self.cfg.masscan_output_location}[/bold cyan]",
             style="green",
         )
 
     def start_scan(self):
         console.print(
-            f"Starting masscan with [bold white]{len(self.ip_list)}[/bold white] entries and [bold white]{len(self.port_list)}[/bold white] ports",
+            f"Starting masscan with [bold white]{len(self.ip_list)}[/bold white] entries and [bold white]{len(self.cfg.ports)}[/bold white] ports",
             style="cyan",
         )
         if platform.system() == "Windows":
             console.print(
                 "If the scanning doesn't work, start this script as admin!",
                 style="bold yellow",
             )
             self.mas.scan(
-                self.mas_ip_list, ports=self.mas_port_list, arguments=self.masscan_args
+                self.mas_ip_list,
+                ports=self.mas_port_list,
+                arguments=self.cfg.masscan_args,
             )
         else:
             self.mas.scan(
                 self.mas_ip_list,
                 ports=self.mas_port_list,
-                arguments=self.masscan_args,
+                arguments=self.cfg.masscan_args,
                 sudo=True,
             )
 
         # Dict-ify masscan results
         masscan_results = json.loads(self.mas.scan_result)
 
         online_ip_amount = len(masscan_results["scan"])
@@ -83,11 +83,11 @@
 
         console.print(
             f"[bold white]{open_port_amount}[/bold white] ports open on [bold white]{online_ip_amount}[/bold white] IPs",
             style="green",
         )
 
         # Save the results if provided
-        if self.masscan_output != "":
+        if self.cfg.masscan_output:
             self.save_output(masscan_results)
 
         return masscan_results
```

### Comparing `yokkaichi-1.3.1/yokkaichi/ServerScan.py` & `yokkaichi-1.4.1/yokkaichi/ServerScan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,44 @@
 # Import modules
 from mcstatus import BedrockServer, JavaServer
-from .rich_console import console
+from .constants.rich_console import console
 from datetime import datetime
 import IP2Location
 import threading
 import json
 import ast
 
 
 class ServerScan:
-    def __init__(
-        self,
-        ports,
-        platforms,
-        query,
-        ip2location_db_file,
-        ip2location_cache,
-        output_file,
-        ip_list,
-        masscan_list,
-    ):
-        self.ip_list = ip_list
+    def __init__(self, cfg, masscan_list, ip_list):
+        self.cfg = cfg
         self.masscan_list = masscan_list
-        self.ports = ports
-        self.platforms = platforms
-        self.query = query
-        self.ip2location_db_file = ip2location_db_file
-        self.ip2location_cache = ip2location_cache
-        self.output_file = output_file
+        self.ip_list = ip_list
 
         self.results = {"server_list": []}
         self.lock = threading.Lock()
 
-    def start_scan(self, thread_count):
-        if self.ip2location_db_file != "":
+    def start_scan(self):
+        if self.cfg.use_ip2location:
             console.print("Loading IP2Location database", style="cyan")
-            if self.ip2location_cache:
+            if self.cfg.ip2location_cache:
                 self.ip2location_db = IP2Location.IP2Location(
-                    self.ip2location_db_file, "SHARED_MEMORY"
+                    self.cfg.ip2location_db, "SHARED_MEMORY"
                 )
             else:
-                self.ip2location_db = IP2Location.IP2Location(self.ip2location_db_file)
+                self.ip2location_db = IP2Location.IP2Location(self.cfg.ip2location_db)
 
         console.print(
-            f"Loading [bold white]{thread_count}[/bold white] threads!", style="cyan"
+            f"Loading [bold white]{self.cfg.threads}[/bold white] threads!",
+            style="cyan",
         )
 
         thread_list = []
 
-        for _ in range(thread_count):
+        for _ in range(self.cfg.threads):
             thread = threading.Thread(target=self.scan_server)
             thread_list.append(thread)
 
         for thread in thread_list:
             thread.start()
 
         for thread in thread_list:
@@ -84,15 +70,15 @@
                     return
                 ports = []
                 for port_info in self.masscan_list["scan"][ip]:
                     ports.append(port_info["port"])
                 self.masscan_list["scan"].pop(ip)
 
             for port in ports:
-                for server_platform in self.platforms:
+                for server_platform in self.cfg.platforms:
                     try:
                         self.check_server(ip, port, server_platform)
                     except Exception:
                         with self.lock:
                             console.print(
                                 f"[-] {ip}:{port} for {server_platform} is offline!",
                                 style="red",
@@ -106,16 +92,16 @@
                     self.ip_list.pop(0)
                 except IndexError:
                     print(
                         f"No more IPs in IP list in thread {threading.current_thread().name}"
                     )
                     return
 
-            for port in self.ports:
-                for server_platform in self.platforms:
+            for port in self.cfg.ports:
+                for server_platform in self.cfg.platforms:
                     try:
                         self.check_server(ip, port, server_platform)
                     except Exception as e:
                         with self.lock:
                             console.print(
                                 f"[-] {ip}:{port} for {server_platform} is offline!",
                                 style="red",
@@ -124,15 +110,15 @@
     def check_server(self, ip, port, server_platform):
         if server_platform == "Java":
             server_lookup = JavaServer.lookup(f"{ip}:{port}")
         if server_platform == "Bedrock":
             server_lookup = BedrockServer.lookup(f"{ip}:{port}")
 
         # Get player list
-        if self.query:
+        if self.cfg.query_java:
             try:
                 player_list = server_lookup.query().players.names
             except Exception as e:
                 console.print(f"[!] Query failed for {ip}:{port}", style="yellow")
                 player_list = None
         else:
             player_list = None
@@ -164,22 +150,18 @@
         with self.lock:
             console.print(
                 f"[+] {server_platform} server found at {ip}:{port}!", style="green"
             )
             self.add_to_file(server_info)
 
     def get_location_data(self, ip):
-        if self.ip2location_db_file == "":
-            # Return None if the database doesn't exist
-            return None
-
         # Make the data be a string
         ip2location_data_str = str(self.ip2location_db.get_all(ip))
         # Convert the data to dict
         ip2location_data_dict = ast.literal_eval(ip2location_data_str)
 
         return ip2location_data_dict
 
     def add_to_file(self, server_info):
         self.results["server_list"].append(server_info)
-        with open(self.output_file, "w", encoding="utf-8") as f:
+        with open(self.cfg.output_file, "w", encoding="utf-8") as f:
             json.dump(self.results, f, indent=4, ensure_ascii=False)
```

### Comparing `yokkaichi-1.3.1/yokkaichi/__main__.py` & `yokkaichi-1.4.1/yokkaichi/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 # Import modules
+from .constants.rich_console import console
+from .port_parser import parse_port_range
+from .args_to_cfg import args_to_cfg
 from .MasscanScan import MasscanScan
 from .ServerScan import ServerScan
-from ._version import __version__
-from .rich_console import console
+from yokkaichi import __version__
+from . import config_loader
 import platform
 import argparse
 import requests
 import pathlib
 
+try:
+    import tomllib
+except ModuleNotFoundError:
+    # Use tomli instead (Python versions before 3.11)
+    import tomli as tomllib
+
+
+def display_version():
+    console.print(
+        f"yokkaichi [bold cyan]{__version__}[/bold cyan] on [bold cyan]{platform.python_implementation()} {platform.python_version()}[/bold cyan]",
+        style="green",
+    )
+    exit()
+
 
 def get_country_ips(countries):
     country_ip_list = []
     for country in countries:
         # Download CIDRs for country
         cidr_list = requests.get(
             f"https://raw.githubusercontent.com/herrbischoff/country-ip-blocks/master/ipv4/{country.lower()}.cidr"
@@ -41,150 +58,127 @@
     except FileNotFoundError:
         console.print("ERROR! IP LIST/MASSCAN LIST NOT FOUND!", style="red")
         exit(1)
 
     return ips
 
 
-def parse_port_range(unparsed_args: str) -> list:
-    def verify_ints(port: any) -> None:
+def main(cfg):
+    if args.show_version:
+        # Show the version and exit
+        display_version()
+
+    # Load the config file
+    if args.config_file != None:
         try:
-            int(port)
-        except TypeError:
+            cfg = config_loader.parse_cfg(args.config_file)
+            # TODO: Make use of it
+        except tomllib.TOMLDecodeError:
             console.print(
-                f"Couldn't parse: [bold white]{port}[/bold white]", style="red"
+                "Config file is invalid! (Failed parsing TOML)", style="bold red"
             )
-            exit(1)
-
-    ports: list[int] = []
-    # Parse all separate port/ranges, separated by commas
-    separate_values: list[str] = unparsed_args.split(",")
-    # Parse all ranges
-    for value in separate_values:
-        # Check if it's a range
-        if "-" in value:
-            # Parse the range
-            port_range: list[str] = value.split("-")
-            range_start: str = port_range[0]
-            range_end: str = port_range[1]
-            for port in (range_start, range_end):
-                verify_ints(port)
-            for port in range(
-                int(range_start), int(range_end) + 1
-            ):  # Range end needs to be offset by 1 to make the range inclusive
-                ports.append(port)
-        else:
-            verify_ints(value)
-            ports.append(int(value))
-
-    return list(set(ports))
-
-
-def main():
-    if args.show_version:
-        # Show the version and exit
-        console.print(
-            f"yokkaichi [bold cyan]{__version__}[/bold cyan] on [bold cyan]{platform.python_implementation()} {platform.python_version()}[/bold cyan]",
-            style="green",
-        )
-        exit()
+        except FileNotFoundError:
+            console.print(
+                f"[bold white]{args.config_file}[/bold white] doesn't exist. Create a sample config in this location? (y/n) ",
+                style="yellow",
+                end="",
+            )
+            if input().lower() == "y":
+                config_loader.write_cfg(args.config_file)
+                console.print(
+                    f"Created a new config file at [bold white]{args.config_file}[/bold white]. Adjust it to your preferences",
+                    style="green",
+                )
+                exit(0)
 
     # Check does output file exists
-    if pathlib.Path(args.output_file).is_file():
+    if pathlib.Path(cfg.output).is_file():
         console.print(
             "Output file exists. Continuing will overwrite this file. Proceed? (y/n) ",
             style="yellow",
             end="",
         )
-        if input() == "n":
+        if input().lower() == "n":
             exit(0)
     else:
         # Touch the file
-        pathlib.Path(args.output_file).touch()
+        pathlib.Path(cfg.output).touch()
 
     # Check does IP2Location db exist
-    if args.ip2location_db != "" and not pathlib.Path(args.ip2location_db).is_file():
+    if cfg.use_ip2location and not pathlib.Path(cfg.ip2location_db).is_file():
         console.print("This IP2Location DB doesn't exist", style="bold red")
         exit(1)
 
-    ports = parse_port_range(args.ports)
-
-    # Add platforms to a list
-    platforms = []
-    if args.java:
-        platforms.append("Java")
-    if args.bedrock:
-        platforms.append("Bedrock")
-
-    if args.ip_list != "":
+    if cfg.ip_list_scan:
         console.print("Loading IPs", style="cyan")
-        ip_list = load_ip_list(args.ip_list)
+        ip_list = load_ip_list(cfg.ip_list)
         console.print(f"Loaded {len(ip_list)} IPs", style="green")
     else:
         ip_list = None
 
-    if args.masscan:
+    if cfg.masscan_scan:
         masscan_ips_from_file = []
         masscan_ips_for_countries = []
-        if args.masscan_ip_list != "":
-            # Load masscan IP list
-            masscan_ips_from_file = load_ip_list(args.masscan_ip_list)
-        if args.masscan_countries != None:
+        if cfg.masscan_ip_source == "countries":
             # Get CIDR ranges for countries
-            masscan_ips_for_countries = get_country_ips(args.masscan_countries)
+            masscan_ips = get_country_ips(cfg.masscan_country_list)
+        elif cfg.masscan_ip_source == "list":
+            # Load masscan IP list
+            masscan_ips = load_ip_list(cfg.masscan_ip_list)
 
         # Combine two sources of masscan IPs together
-        masscan_ips = masscan_ips_from_file + masscan_ips_for_countries
+        # masscan_ips = masscan_ips_from_file + masscan_ips_for_countries
 
         # Start masscan
-        masscan_scanner = MasscanScan(
-            masscan_ips, ports, args.masscan_args, args.masscan_json_output
-        )
+        masscan_scanner = MasscanScan(cfg, masscan_ips)
         masscan_results = masscan_scanner.start_scan()
     else:
         masscan_results = None
 
     # print(clr.Fore.CYAN + "Loading IPs")
     # ips = load_file()
 
-    ServerScan(
-        ip_list=ip_list,
-        masscan_list=masscan_results,
-        ports=ports,
-        platforms=platforms,
-        query=args.query,
-        ip2location_db_file=args.ip2location_db,
-        ip2location_cache=args.ip2location_cache,
-        output_file=args.output_file,
-    ).start_scan(args.thread_count)
+    ServerScan(cfg=cfg, masscan_list=masscan_results, ip_list=ip_list).start_scan()
 
 
 if __name__ == "__main__":
-    # Parse arguments
     parser = argparse.ArgumentParser(allow_abbrev=False)
     parser.add_argument(
         "-j", "--java", dest="java", help="Scan for Java servers", action="store_true"
     )
     parser.add_argument(
         "-b",
         "--bedrock",
         dest="bedrock",
         help="Scan for Bedrock servers",
         action="store_true",
     )
     parser.add_argument(
+        "--ip-list-scan",
+        dest="ip_list_scan",
+        help="Scan from IP list (slow and outdated, use masscan instead)",
+        action="store_true",
+    )
+    parser.add_argument(
         "--ip-list", dest="ip_list", help="Location to IP List", type=str, default=""
     )
     parser.add_argument(
         "--masscan",
         dest="masscan",
         help="Enable scanning with masscan",
         action="store_true",
     )
     parser.add_argument(
+        "--masscan-method",
+        dest="masscan_method",
+        help="Where to look for IPs for masscan? Possible values: countries, list",
+        type=str,
+        default="countries",
+    )
+    parser.add_argument(
         "--masscan-ip-list",
         dest="masscan_ip_list",
         help="Location to IP (or CIDR) list to scan by masscan before scanning with mcserver scanner",
         type=str,
         default="",
     )
     parser.add_argument(
@@ -246,21 +240,32 @@
         "-o",
         "--output",
         dest="output_file",
         help="Output JSON file",
         default="out.json",
     )
     parser.add_argument(
+        "-c",
+        "--config",
+        dest="config_file",
+        help="Configuration file (example one will be created if it doesn't exist)",
+        default=None,
+        const="yokkaichi.toml",
+        nargs="?",
+    )
+    parser.add_argument(
         "-v",
         "--version",
         dest="show_version",
         help="Show version and quit",
         action="store_true",
     )
     parser.set_defaults(java=False, bedrock=False, query=False)
     args = parser.parse_args()
 
+    cfg = args_to_cfg(args)
+
     # if args.java and args.bedrock == False:
     #     print("You need to choose either Java or Bedrock")
     #     exit(1)
 
-    main()
+    main(cfg)
```

### Comparing `yokkaichi-1.3.1/yokkaichi.egg-info/PKG-INFO` & `yokkaichi-1.4.1/yokkaichi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.3.1
+Version: 1.4.1
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
+License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -30,28 +31,29 @@
 - Query integration
 
 ### Planned features (not in a specific order)
 - WWW interface
 - Bot joining the servers
 - Cleaning up the code
 - Docker support
+- Optimization
+- Scanning for pre-Netty (<1.7) servers
 
 ### Installation
 - Easy installation (from PyPI)
 ```
 pip install yokkaichi
 ```
 - Manual installation (from git)
 ```
 git clone https://github.com/Oreeeee/yokkaichi
 cd yokkaichi
 pip install .
 ```
 
 ### Usage
-You can use this script by invoking `python -m yokkaichi` and passing in arguments in the CLI. You can get the list of availible options by invoking `python -m yokkaichi -h`
+1. Using a config file
+Instead of passing in arguments, you can pass the configuration file with `--config` argument. When no additional file name is provided, Yokkaichi will use `yokkaichi.toml` for the file name. When the config file name you provided doesn't exist, Yokkaichi will create an example file for you. Modify it how you like and rerun Yokkaichi. Configuration files are not forwards or backwards compatible and you will have to adjust it every major change. 
+2. You can also use this script by passing in arguments in the CLI. You can get the list of availible options by invoking `python -m yokkaichi -h`.
 
 ### Using the masscan integration
 You need to have [masscan](https://github.com/robertdavidgraham/masscan) in your PATH, or in the same directory from which you are running this software. Make sure that the binary is named `masscan` (Unix) or `masscan.exe` (Windows).
-
-### Example
-`python -m yokkaichi --java --masscan --masscan-countries US CA CN -p "25560-25569,34000,19843" --ip2location-db data/IP2LOCATION-LITE-DB11.BIN --ip2location-cache --output data/servers.json`
```

