# Comparing `tmp/satori-ci-1.1.9.tar.gz` & `tmp/satori_ci-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori-ci-1.1.9.tar", last modified: Thu Apr 13 16:55:44 2023, max compression
+gzip compressed data, was "satori_ci-1.2.4.tar", last modified: Fri May 12 21:33:04 2023, max compression
```

## Comparing `satori-ci-1.1.9.tar` & `satori_ci-1.2.4.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-03-28 19:49:33.588036 satori-ci-1.1.9/LICENSE
--rw-r--r--   0        0        0     4984 2023-03-28 19:49:33.588180 satori-ci-1.1.9/README.md
--rw-r--r--   0        0        0      594 2023-04-13 16:53:36.657115 satori-ci-1.1.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588599 satori-ci-1.1.9/src/satorici/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588697 satori-ci-1.1.9/src/satorici/classes/__init__.py
--rw-r--r--   0        0        0     3307 2023-04-13 16:53:36.657556 satori-ci-1.1.9/src/satorici/classes/api.py
--rw-r--r--   0        0        0     1830 2023-03-28 19:49:33.588923 satori-ci-1.1.9/src/satorici/classes/bundler.py
--rw-r--r--   0        0        0    17164 2023-04-13 16:53:36.657899 satori-ci-1.1.9/src/satorici/classes/satori.py
--rw-r--r--   0        0        0     5865 2023-03-28 19:49:33.589279 satori-ci-1.1.9/src/satorici/classes/utils.py
--rwxr-xr-x   0        0        0     5890 2023-03-31 17:35:44.200461 satori-ci-1.1.9/src/satorici/satori_module.py
--rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 satori-ci-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-28 19:49:33.588036 satori_ci-1.2.4/LICENSE
+-rw-r--r--   0        0        0     4984 2023-03-28 19:49:33.588180 satori_ci-1.2.4/README.md
+-rw-r--r--   0        0        0      646 2023-05-12 21:33:04.773533 satori_ci-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588599 satori_ci-1.2.4/src/satorici/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588697 satori_ci-1.2.4/src/satorici/classes/__init__.py
+-rw-r--r--   0        0        0     4270 2023-05-12 21:32:46.495727 satori_ci-1.2.4/src/satorici/classes/api.py
+-rw-r--r--   0        0        0     1770 2023-05-12 21:32:46.495905 satori_ci-1.2.4/src/satorici/classes/bundler.py
+-rw-r--r--   0        0        0     2807 2023-05-12 21:32:46.496024 satori_ci-1.2.4/src/satorici/classes/playbooks.py
+-rw-r--r--   0        0        0    21020 2023-05-12 21:32:46.496333 satori_ci-1.2.4/src/satorici/classes/satori.py
+-rw-r--r--   0        0        0     9016 2023-05-12 21:32:46.496583 satori_ci-1.2.4/src/satorici/classes/utils.py
+-rw-r--r--   0        0        0     1440 2023-05-12 21:32:46.496752 satori_ci-1.2.4/src/satorici/classes/validations.py
+-rwxr-xr-x   0        0        0     6027 2023-05-12 21:32:46.496979 satori_ci-1.2.4/src/satorici/satori_module.py
+-rw-r--r--   0        0        0    46006 1970-01-01 00:00:00.000000 satori_ci-1.2.4/PKG-INFO
```

### Comparing `satori-ci-1.1.9/LICENSE` & `satori_ci-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `satori-ci-1.1.9/README.md` & `satori_ci-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `satori-ci-1.1.9/pyproject.toml` & `satori_ci-1.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 [project]
 name = "satori-ci"
-version = "1.1.9"
+version = "1.2.4"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyyaml>=6.0",
     "tqdm>=4.64.1",
     "colorama>=0.4.6",
+    "flatdict>=4.0.1",
+    "rich>=13.0",
+    "gitpython>=3.1.31",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://www.satori-ci.com"
 
 [project.scripts]
 satori-cli = "satorici.satori_module:main"
 
-[tool.pdm]
-
 [build-system]
 requires = [
-    "pdm-pep517>=0.12.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
+
+[tool]
```

### Comparing `satori-ci-1.1.9/src/satorici/classes/bundler.py` & `satori_ci-1.2.4/src/satorici/classes/bundler.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,31 +13,26 @@
 def is_import(value):
     return isinstance(value, list) and (
         all(isinstance(e, str) and IMPORT_REGEX.fullmatch(e) for e in value)
     )
 
 
 def is_input(value):
-    return isinstance(value, list) and (
-        all(isinstance(e, (str, dict)) for e in value)
-    )
+    return isinstance(value, list) and (all(isinstance(e, (str, dict)) for e in value))
 
 
 def get_local_files(config: dict):
     paths = {"imports": set(), "inputs": set()}
     for value in config.values():
         if is_import(value):
-            paths["imports"].update([
-                p[7:] for p in value if p.startswith("file")
-            ])
+            paths["imports"].update([p[7:] for p in value if p.startswith("file")])
         elif is_input(value):
-            paths["inputs"].update([
-                p.get("file") for p in value
-                if isinstance(p, dict) and p.get("file")
-            ])
+            paths["inputs"].update(
+                [p.get("file") for p in value if isinstance(p, dict) and p.get("file")]
+            )
         elif isinstance(value, dict):
             paths.update(get_local_files(value))
     return paths
 
 
 def get_references(stream, dir):
     file_list = get_local_files(yaml.safe_load(stream))
```

### Comparing `satori-ci-1.1.9/src/satorici/classes/satori.py` & `satori_ci-1.2.4/src/satorici/classes/satori.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+import ast
 import json
 import os
 import shutil
 import sys
 import tempfile
 import uuid
 from pathlib import Path
 import time
 import requests
 import yaml
+from typing import Union
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 from colorama import Fore
+from argparse import Namespace
 
 from satorici.classes.api import SatoriAPI
 from satorici.classes.bundler import make_bundle
 from satorici.classes.utils import (
     dict_formatter,
     filter_params,
     autoformat,
@@ -22,33 +25,38 @@
     FAIL_COLOR,
     KEYNAME_COLOR,
     SATORIURL_COLOR,
     VALUE_COLOR,
     UUID4_REGEX,
     autocolor,
     puts,
+    table_generator,
+    argument,
+    log,
 )
+from satorici.classes.validations import get_parameters, validate_parameters
+from satorici.classes.playbooks import display_public_playbooks
 
 
 class Satori:
     """Have some class"""
 
-    def __init__(self, profile="default", config=False):
+    def __init__(self, args: Union[Namespace, argument], config=False) -> None:
         """Turn on the engines"""
-        self.profile = profile
+        self.profile = args.profile
         self.config_paths = [
             f"{Path.home()}/.satori_credentials.yml",
             ".satori_credentials.yml",
         ]
         self.verbose = False
         if not config:
             self.load_config()
-            self.api = SatoriAPI(self.token, self.server)
+            self.api = SatoriAPI(self.token, self.server, args)
 
-    def load_config(self):
+    def load_config(self) -> None:
         """Load the config file and set the token on the headers"""
         config_file = None
         for file in self.config_paths:
             if Path(file).is_file():
                 config_file = Path(file)
                 break
 
@@ -103,47 +111,72 @@
         config.setdefault(self.profile, {})[key] = value
 
         with open(config_file, "w") as f:
             f.write(yaml.safe_dump(config))
 
         puts(Fore.LIGHTGREEN_EX, key.capitalize() + " saved")
 
-    def run(self, args):
-        exec_data = None
-        if os.path.isdir(args.path):
+    def run(self, args: Union[Namespace, argument]):
+        path = Path(args.path)
+        params = set()
+
+        if getattr(args, "data", False):
+            try:
+                data = ast.literal_eval(args.data)
+
+                if not validate_parameters(args.data):
+                    raise
+
+                params.update(data.keys())
+            except Exception:
+                puts(FAIL_COLOR, "Malformed parameters")
+                sys.exit(1)
+
+        if path.is_dir():
+            playbook = path / ".satori.yml"
+        elif path.is_file():
+            playbook = path
+        else:
+            puts(FAIL_COLOR, "Satori can not access to file/folder")
+            sys.exit(1)
+
+        with playbook.open() as f:
+            variables = get_parameters(yaml.safe_load(f))
+            if variables != params:
+                puts(FAIL_COLOR, f"Required parameters: {variables - params}")
+                sys.exit(1)
+
+        if path.is_dir():
             exec_data = self.run_folder(args)
-        elif os.path.isfile(args.path):
+        else:  # is file
             exec_data = self.run_file(args)
-        else:
-            puts(FAIL_COLOR, "Unknown file type")  # is a device?
-            sys.exit(1)
         if args.sync and exec_data:
             self.run_sync(exec_data)
 
-    def run_file(self, args) -> dict:
+    def run_file(self, args: Union[Namespace, argument]) -> dict:
         """Just run"""
         playbook = args.path
         if playbook is None:
             print(
                 f"Define the Satori playbook file:\n{sys.argv[0]} run -p playbook.yml"
             )
-            return False
+            sys.exit(1)
 
         if not os.path.isfile(playbook):
             puts(FAIL_COLOR, f"Playbook not found: {playbook}")
-            return False
+            sys.exit(1)
 
         bundle = make_bundle(playbook)
         is_monitor = check_monitor(playbook)
-        url = self.api.get_bundle_presigned_post(args)
+        url = self.api.runs("bundle", args.data)
+        log.debug(url)
         res = requests.post(
-            url["url"],
-            url["fields"],
-            files={"file": bundle},
+            url["url"], url["fields"], files={"file": bundle}, timeout=None
         )
+        log.debug(res.text)
         if not res.ok:
             puts(FAIL_COLOR, "File upload failed")
             sys.exit(1)
         if is_monitor:
             exec_type = "monitor"
             exec_id = url["monitor"]
             print(KEYNAME_COLOR + "Monitor ID: " + VALUE_COLOR + f"{exec_id}")
@@ -156,68 +189,70 @@
                 KEYNAME_COLOR
                 + "Report: "
                 + SATORIURL_COLOR
                 + f"https://www.satori-ci.com/report_details/?n={exec_id}"
             )
         return {"type": exec_type, "id": exec_id}
 
-    def run_folder(self, args) -> dict:
+    def run_folder(self, args: Union[Namespace, argument]) -> dict:
         """Upload directory and run"""
         directory = args.path
         if directory is None:
             print(
                 "Define the directory with the Satori playbook:"
                 f"\n{sys.argv[0]} run -p ./directory_with_playbook"
             )
-            return False
+            sys.exit(1)
 
         if not os.path.isdir(directory):
             puts(FAIL_COLOR, f"Directory not found: {directory}")
-            return False
+            sys.exit(1)
 
         satori_yml = Path(directory, ".satori.yml")
-        bundle = make_bundle(satori_yml, from_dir=True)
+        bundle = make_bundle(str(satori_yml), from_dir=True)
         is_monitor = check_monitor(satori_yml)
         temp_file = Path(tempfile.gettempdir(), str(uuid.uuid4()))
         full_path = f"{temp_file}.zip"
 
         try:
-            shutil.make_archive(temp_file, "zip", directory)
+            shutil.make_archive(str(temp_file), "zip", directory)
         except Exception as e:
             puts(FAIL_COLOR, f"Could not compress directory: {e}")
-            return False
-
-        res = self.api.get_archive_presigned_post(args)
+            sys.exit(1)
 
+        res = self.api.runs("archive", args.data)
+        log.debug(res)
         arc = res["archive"]
         bun = res["bundle"]
         mon = res["monitor"]
 
         try:
             bar_params = {
                 "total": os.stat(full_path).st_size,
                 "unit": "B",
                 "desc": "Archive upload",
                 "unit_scale": True,
             }
             with tqdm(**bar_params) as t, open(full_path, "rb") as f:
                 w = CallbackIOWrapper(t.update, f, "read")
-                res = requests.post(arc["url"], arc["fields"], files={"file": w})
+                file = {"file": w}
+                res = requests.post(
+                    arc["url"], arc["fields"], files=file, timeout=None  # type: ignore
+                )
         finally:
             os.remove(full_path)
 
         if not res.ok:
             print("Archive upload failed")
             sys.exit(1)
 
         res = requests.post(
-            bun["url"],
-            bun["fields"],
-            files={"file": bundle},
+            bun["url"], bun["fields"], files={"file": bundle}, timeout=None
         )
+        log.debug(res.text)
         if not res.ok:
             print("Bundle upload failed")
             sys.exit(1)
 
         if is_monitor:
             exec_type = "monitor"
             exec_id = mon
@@ -233,40 +268,51 @@
                 )
             )
         return {"type": exec_type, "id": exec_id}
 
     def run_sync(self, exec_data: dict) -> None:
         puts(KEYNAME_COLOR, "Fetching data...", end="\r")
         start_time = time.time()
+        spin = "-\\|/"
+        pos = 0
         while True:
+            pos += 1
+            if pos >= len(spin):
+                pos = 0
             time.sleep(1)
             elapsed = time.time() - start_time
             elapsed_text = f"Elapsed time: {elapsed:.1f}s"
             try:
-                report_data = self.api.report_get("get", {"id": exec_data["id"]})
+                report_data = self.api.reports(
+                    "GET", exec_data["id"], "", raise_error=True
+                )
             except requests.HTTPError as e:
                 code = e.response.status_code
                 if code in (404, 403):
                     print(
-                        autocolor(f"Report status: Unknown | {elapsed_text}"), end="\r"
+                        autocolor(
+                            f"{spin[pos]} Report status: Unknown | {elapsed_text}"
+                        ),
+                        end="\r",
                     )
                     continue
                 else:
                     puts(FAIL_COLOR, f"Failed to get data\nStatus code: {code}")
                     sys.exit(1)
+
             status = report_data.get("status", "Unknown")
             if status in ("Completed", "Undefined"):
                 fails = report_data["fails"]
                 if fails is None:
                     result = "Unknown"
                 else:
                     result = "Pass" if fails == 0 else f"Fail({fails})"
                 print(
                     autocolor(
-                        f"Report status: {status} | Result: {result} | {elapsed_text}"
+                        f"- Report status: {status} | Result: {result} | {elapsed_text}"
                     ),
                     end="\r\n",
                 )
                 report_out = []
                 # Remove keys
                 json_data = report_data.get("json") or []
                 for report in json_data:
@@ -285,194 +331,225 @@
                     if comments:
                         puts(FAIL_COLOR, f"Error: {comments}")
                     sys.exit(1)
                 else:
                     # Return code 0 if report status==pass else 1
                     sys.exit(0 if report_data["fails"] == 0 else 1)
             else:
-                print(autocolor(f"Report status: {status} | {elapsed_text}"), end="\r")
+                print(
+                    autocolor(f"{spin[pos]} Report status: {status} | {elapsed_text}"),
+                    end="\r",
+                )
 
-    def repo(self, args):
+    def repo(self, args: Union[Namespace, argument]):
         """Run Satori on multiple commits"""
-        params = filter_params(args, ("id"))
+        params = filter_params(args, ("id",))
+        if args.playbook:
+            playbook = Path(args.playbook)
+            if playbook.is_file():
+                args.playbook = playbook.read_text()
         if args.action == "scan":
             params = filter_params(
-                args, ("id", "coverage", "from", "to", "branch", "data")
+                args, ("coverage", "from", "to", "branch", "data", "playbook")
             )
+            params["url"] = args.id
+            info = self.api.repos_scan("GET", "", "", params=params)
         elif args.action == "clean":
             params = filter_params(args, ("id", "delete_commits"))
+            info = self.api.repos("GET", args.id, args.action, params=params)
         elif args.action == "tests":
             params = filter_params(args, ("id", "filter", "all", "limit", "fail"))
+            info = self.api.repos("GET", args.id, args.action, params=params)
         elif args.action == "run":
-            params = filter_params(args, ("id", "data"))
+            params = filter_params(args, ("id", "data", "playbook"))
+            info = self.api.repos_scan("GET", args.id, "last", params=params)
+        elif args.action == "scan-stop":
+            info = self.api.repos_scan("GET", args.id, "stop", params=params)
+        elif args.action == "scan-status":
+            info = self.api.repos_scan("GET", args.id, "status", params=params)
+        elif args.action == "check-forks":
+            info = self.api.repos_scan("GET", args.id, args.action, params=params)
         elif args.action == "check-commits":
             params = filter_params(args, ("id", "branch"))
-        elif args.action not in (
-            "commits",
-            "check-forks",
-            "scan-stop",
-            "scan-status",
-            "get",
-            "download",
-        ):
-            print("Unknown subcommand")
+            info = self.api.repos_scan("GET", args.id, args.action, params=params)
+        elif args.action in ("commits", "", "download", "pending"):
+            info = self.api.repos("GET", args.id, args.action, params=params)
+        else:
+            puts(FAIL_COLOR, "Unknown subcommand")
             sys.exit(1)
-        info = self.api.repo_get(args, params)
-        if args.id != "list" or args.action != "get" or args.json:
+
+        if args.id != "" or args.action != "" or args.json:
             autoformat(info, jsonfmt=args.json, list_separator="-" * 48)
         else:
             print("Pending actions:")
             autoformat(info["pending"])
             print("\nRepos:")
             autoformat(info["list"], list_separator="-" * 48)
         if args.action == "run" and args.sync:
+            if isinstance(info, list):
+                info = info[0]
             report = info.get("status", "")
             match = UUID4_REGEX.findall(report)
             if match:
                 self.run_sync({"type": "report", "id": match[0]})
 
-    def report(self, args):
+    def report(self, args: Union[Namespace, argument]):
         """Show a list of reports"""
-        params = filter_params(args, ("id"))
-        if args.action == "get":
+        params = filter_params(args, ("id",))
+        if args.action == "":
             params = filter_params(args, ("id", "page", "limit", "filter"))
-            res = self.api.report_get(args.action, params)
+            res = self.api.reports("GET", args.id, "", params=params)
             if isinstance(res, list) and not args.json:
                 for commit in res:
                     dict_formatter(commit)
                     puts(Fore.LIGHTBLACK_EX, ("_" * 48) + "\n")
             else:
                 autoformat(res, jsonfmt=args.json)
             if not args.json:
                 print(f"Current page: {args.page}")
         elif args.action == "output":
             self.output(args, params)
         elif args.action == "stop":
-            res = self.api.report_get(args.action, params)
+            res = self.api.reports("GET", args.id, "stop")
             autoformat(res, jsonfmt=args.json)
         elif args.action == "delete":
-            res = self.api.report_delete(params)
-            autoformat(res, jsonfmt=args.json)
+            self.api.report_delete(params)
+            print("Report deleted")
         else:
             print("Unknown subcommand")
             sys.exit(1)
 
-    def monitor(self, args):
+    def monitor(self, args: Union[Namespace, argument]):
         """Get information about the"""
-        params = filter_params(args, ("id"))
+        params = filter_params(args, ("id",))
         if args.action == "delete":
-            info = self.api.monitor_delete(params)
-        elif args.action in ("start", "stop", "get"):
-            info = self.api.monitor_get(args.action, params)
+            self.api.monitor_delete(params)
+            print("Monitor deleted")
+            sys.exit(0)
+        elif args.action == "":
+            info = self.api.monitors("GET", args.id, "")
+        elif args.action in ("start", "stop"):
+            info = self.api.monitors("PATCH", args.id, args.action)
         else:
             print("Unknown subcommand")
             sys.exit(1)
-        if args.id != "list" or args.action != "get" or args.json:
+        if args.id != "" or args.action != "" or args.json:
             autoformat(info, jsonfmt=args.json, list_separator="*" * 48)
         else:
             if len(info["pending"]) > 1:
                 print("Pending actions:")
                 autoformat(info["pending"])
             print("\nMonitors:")
-            autoformat(info["list"], list_separator="-" * 48)
+            autoformat(info["list"], list_separator="-" * 48, table=True)
 
     def output(self, args, params):
         """Returns commands output"""
-
         try:
-            if uuid.UUID(args.id):
-                data = self.api.report_get(args.action, params)
+            uuid.UUID(args.id)
         except ValueError:
+            puts(FAIL_COLOR, f"{args.id} is not a valid report ID")
             sys.exit(1)
+        data = self.api.reports("GET", args.id, args.action, params=params)
 
-        if not args.json:
+        if not args.json:  # default output
             outputs = data.pop("output", [])
             for key, value in data.items():
                 print(f"{key}: {value}")
 
             for row in outputs:
-                print("-" * 30)
+                puts(Fore.LIGHTBLACK_EX, "-" * 48)
+                puts(Fore.CYAN, f"test_name: {row['test_name']}")
+                puts(KEYNAME_COLOR, "command: ", Fore.LIGHTBLUE_EX, row["command"])
                 for key, value in row.items():
-                    print(f"{key}: {value}")
+                    if key in ("test_name", "command"):
+                        continue
+                    val_color = VALUE_COLOR
+                    if key == "stdout":
+                        val_color = Fore.LIGHTGREEN_EX
+                    elif key == "stderr":
+                        val_color = Fore.LIGHTRED_EX
+                    elif key == "return_code":
+                        val_color = Fore.YELLOW
+                    puts(KEYNAME_COLOR, f"{key}: ", val_color, str(value))
         else:
             print(json.dumps(data, indent=2))
 
-    def dashboard(self, args):
+    def dashboard(self, args: Union[Namespace, argument]):
         """Get user dashboard"""
         info = self.api.dashboard()
         if args.json:
             autoformat(info, jsonfmt=True)
         else:
             len_mon = len(info["Actions"]["Monitors"])
             len_rep = len(info["Actions"]["Repos"])
             if len_mon > 0 or len_rep > 0:
-                print("Actions required:")
+                # print pending actions
                 if len_mon > 0:
-                    print("  Monitors:")
-                    autoformat(info["Actions"]["Monitors"], indent=1)
+                    print("Monitors(Actions required):")
+                    mon_items = []
+                    for m in info["Actions"]["Monitors"]:
+                        for key in m:
+                            mon_items.append([key, m[key]])
+                    table_generator(["Name", "Pending action"], mon_items, "bold green")
                 if len_rep > 0:
-                    print("  Repos:")
-                    autoformat(info["Actions"]["Repos"], indent=1)
+                    print("Repos(Actions required):")
+                    rep_items = []
+                    for r in info["Actions"]["Repos"]:
+                        for key in r:
+                            rep_items.append([key, r[key]])
+                    table_generator(["Name", "Pending action"], rep_items, "bold green")
             for title in info:
                 if title == "Actions":
                     continue
                 if title == "Monitors":
                     if len(info[title]) == 0:
                         print("\nMonitors: no active monitors defined")
                         continue
                 print(f"\n{title}:")
+                items = []
                 n = 0
                 for i in info[title]:
                     n += 1
                     for key in i:
-                        print(f"{n}) {key.capitalize()}: {i[key]}")
+                        items.append([str(n), key, i[key]])
+                table_generator(["Nº", "Name", "Status"], items, "bold blue")
 
-    def playbook(self, args):
+    def playbook(self, args: Union[Namespace, argument]):
         """Get playbooks"""
-        if args.action == "get":
+        if args.public:
+            display_public_playbooks()
+
+        if args.action == "":
             params = filter_params(args, ("id", "limit", "page"))
             data = self.api.playbook_get(params)
             if args.json:
-                print(json.dumps(data))
+                autoformat(data, jsonfmt=True)
                 sys.exit(1)
-            if args.id == "all":
-                data = list(
-                    map(
-                        lambda x: {
-                            "ID": x["ID"],
-                            "URI": x["URI"],
-                            "Name": x["Name"],
-                            # Add a new line to remove indent
-                            "Playbook": f"\n{x['Playbook']}",
-                        },
-                        data,
-                    )
-                )
         elif args.action == "delete":
-            params = filter_params(args, ("id"))
+            params = filter_params(args, ("id",))
             data = self.api.playbook_delete(params)
         else:
             print("Unknown subcommand")
             sys.exit(1)
         autoformat(data, jsonfmt=args.json, list_separator="-" * 48)
 
-    def team(self, args):
+    def team(self, args: Union[Namespace, argument]):
         """Get information about the"""
-        params = filter_params(args, ("id"))
-        if args.action == "get":
-            info = self.api.team_get(params)
+        params = filter_params(args, ("id",))
+        if args.action == "":
+            info = self.api.teams("GET", "", "", params=params)
         elif args.action == "create":
-            info = self.api.team_post(params)
+            info = self.api.teams("PUT", args.id, "", data=params)
         elif args.action == "members":
-            info = self.api.team_members_get(params)
+            info = self.api.teams("GET", args.id, "members", params=params)
         elif args.action == "add_member":
             params = filter_params(args, ("id", "email", "role"))
-            info = self.api.team_members_put(params)
+            info = self.api.teams("PUT", args.id, "members", data=params)
         elif args.action == "repos":
-            info = self.api.team_repos_get(params)
+            info = self.api.teams("PUT", args.id, "repos", data=params)
         elif args.action == "add_repo":
             params = filter_params(args, ("id", "repo"))
-            info = self.api.team_repos_put(params)
+            info = self.api.teams("PUT", args.id, "repos", data=params)
         else:
             print("Unknown subcommand")
             sys.exit(1)
-        autoformat(info, jsonfmt=args.json, list_separator="*" * 48)
+        autoformat(info, jsonfmt=args.json, list_separator="*" * 48, table=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `satori-ci-1.1.9/src/satorici/classes/utils.py` & `satori_ci-1.2.4/src/satorici/classes/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,95 @@
 from typing import Union
 import json
 import yaml
 import re
+from typing import Any
 from colorama import Fore, Style
+from rich.logging import RichHandler
+import logging
+from rich import print_json
+from rich.console import Console
+from rich.syntax import Syntax
+from rich.table import Table
+import random
 
 __decorations = "▢•○░"
+__random_colors = ["green", "blue", "red"]
 # IDs
 UUID4_REGEX = re.compile(
     r"[0-9a-f]{8}-[0-9a-f]{4}-4[0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}",
     re.I,
 )
 # Regex
 PASS_REGEX = re.compile(r"(pass|completed)", re.IGNORECASE)
 RUNNING_REGEX = re.compile(r"(pending|running)", re.IGNORECASE)
 FAIL_REGEX = re.compile(r"(fail(\(\d+\))?|error)", re.IGNORECASE)
 UNKNOWN_REGEX = re.compile(r"(unknown|undefined)", re.IGNORECASE)
 SATORIURL_REGEX = re.compile(r"(https?:\/\/(www\.)satori-ci\.com\S+)")
-KEYNAME_REGEX = re.compile(r"(([^\w]|^)\w[\w\s]*:\s*)(?!\/\/)")
+KEYNAME_REGEX = re.compile(r"(([^\w]|^)\w[\w\s]*:\s*)(?!\/\/)")  # ex: "key: "
 # Colors outputs
 PASS_COLOR = Fore.LIGHTGREEN_EX
 FAIL_COLOR = Fore.LIGHTRED_EX
 UNKNOWN_COLOR = Fore.LIGHTYELLOW_EX
 RUNNING_COLOR = Fore.LIGHTBLUE_EX
 KEYNAME_COLOR = Fore.WHITE
 SATORIURL_COLOR = Fore.LIGHTBLUE_EX
 VALUE_COLOR = Fore.CYAN
 MULTILINE_COLOR = Fore.YELLOW
 
+logging.basicConfig(
+    level="CRITICAL",
+    format="%(message)s",
+    handlers=[RichHandler(rich_tracebacks=True, show_time=False)],
+)
+log = logging.getLogger()
+console = Console(log_path=False, log_time=False)
+
 
 def get_decoration(indent):
     return (
         Style.DIM
         + "  " * indent
         + __decorations[indent % len(__decorations)]
         + " "
         + Style.RESET_ALL
     )
 
 
 def dict_formatter(
-    obj: dict, capitalize: bool = False, indent: int = 0, list_separator: str = None
+    obj: dict,
+    capitalize: bool = False,
+    indent: int = 0,
+    list_separator: Union[str, None] = None,
 ):
     for key in obj.keys():
         indent_text = get_decoration(indent)
         key_text = key.capitalize() if capitalize else key
         if isinstance(obj[key], dict):
             print(indent_text + KEYNAME_COLOR + f"{key_text}:" + Style.RESET_ALL)
             dict_formatter(obj[key], capitalize, indent + 1, list_separator)
         elif isinstance(obj[key], list):
             print(indent_text + KEYNAME_COLOR + f"{key_text}:" + Style.RESET_ALL)
             list_formatter(obj[key], capitalize, indent + 1, list_separator)
         else:
             item = str(obj[key])
-            print(
-                indent_text
-                + KEYNAME_COLOR
-                + f"{key_text}: "
-                + get_value_color(item)
-                + item
-                + Style.RESET_ALL
-            )
+            color = get_value_color(item)
+            print(indent_text + KEYNAME_COLOR + f"{key_text}: ", end="")
+            if item.count("\n") > 0:
+                if autosyntax(item, indent + 2):
+                    continue
+            # Not JSON or YAML
+            print(color + item + Style.RESET_ALL)
 
 
 def list_formatter(
-    obj: dict, capitalize: bool = False, indent: int = 0, list_separator: str = None
+    obj: list,
+    capitalize: bool = False,
+    indent: int = 0,
+    list_separator: Union[str, None] = None,
 ):
     for item in obj:
         indent_text = get_decoration(indent)
         if isinstance(item, dict):
             dict_formatter(item, capitalize, indent + 1, list_separator)
         elif isinstance(item, list):
             list_formatter(item, capitalize, indent + 1, list_separator)
@@ -80,53 +102,62 @@
                 + Fore.LIGHTBLACK_EX
                 + list_separator
                 + Style.RESET_ALL
             )
 
 
 def autoformat(
-    obj: any,
+    obj: Any,
     capitalize: bool = False,
     indent: int = 0,
     jsonfmt: bool = False,
-    list_separator: str = None,
-    color: any = None,
-):
+    list_separator: Union[str, None] = None,
+    color: str = "",
+    table: bool = False,
+) -> None:
     """Format and print a dict, list or other var
 
     Parameters
     ----------
-    obj : any
+    obj : Any
         Var to print
     capitalize : bool, optional
         Capitalize dict keys, by default False
     ident : bool, optional
         Indent length, by default 0
     jsonfmt: bool, optional
         Print as json, by default False
     list_separator: str, optional
         List separator
     """
     if jsonfmt:
-        print(json.dumps(obj, indent=indent, default=str))
+        print_json(json.dumps(obj, default=str), indent=(indent + 1) * 2)
     else:
         if isinstance(obj, dict):
             dict_formatter(obj, capitalize, indent, list_separator)
         elif isinstance(obj, list):
+            if table and len(obj) > 0 and isinstance(obj[0], dict):
+                head_color = random.choice(__random_colors)  # nosec
+                autotable(obj, f"bold {head_color}")
+                return None
             list_formatter(obj, capitalize, indent, list_separator)
+        elif isinstance(obj, str):
+            if obj.count("\n") > 0:
+                if not autosyntax(obj, indent):
+                    print(obj)
         else:
             print(color + str(obj) + Style.RESET_ALL)
 
 
-def filter_params(params: any, filter_keys: Union[tuple, list]) -> dict:
+def filter_params(params: Any, filter_keys: Union[tuple, list]) -> dict:
     """Filter elements of a dict/namespace according to a list of keys
 
     Parameters
     ----------
-    params : any
+    params : Any
         dict or namespace to filter
     filter_keys : Union[tuple, list]
         List of keys to return from dict or namespace
 
     Returns
     -------
     dict
@@ -146,22 +177,22 @@
 
 
 def puts(color: str = Style.NORMAL, *args, **kargs):
     """Print with colors, resets the color after printing
 
     Parameters
     ----------
-    color : any, optional
+    color : Any, optional
         Color of the text, by default Style.NORMAL
     """
     # color, args adds an empty space??
     print(color + "".join(args), Style.RESET_ALL, **kargs)
 
 
-def get_value_color(item: any) -> str:
+def get_value_color(item: Any) -> str:
     item = str(item)
     color = VALUE_COLOR
     if item.count("\n") > 0:
         color = f"\n{MULTILINE_COLOR}"
     else:
         if PASS_REGEX.search(item):
             color = PASS_COLOR
@@ -184,7 +215,85 @@
     txt = KEYNAME_REGEX.sub(rf"{KEYNAME_COLOR}\1{VALUE_COLOR}", txt)
     txt = PASS_REGEX.sub(rf"{PASS_COLOR}\1{rst}", txt)
     txt = RUNNING_REGEX.sub(rf"{RUNNING_COLOR}\1{rst}", txt)
     txt = FAIL_REGEX.sub(rf"{FAIL_COLOR}\1{rst}", txt)
     txt = UNKNOWN_REGEX.sub(rf"{UNKNOWN_COLOR}\1{rst}", txt)
     txt = SATORIURL_REGEX.sub(rf"{SATORIURL_COLOR}\1{rst}", txt)
     return txt
+
+
+def autosyntax(item: str, indent: int) -> bool:
+    ind = (indent) * 2
+    try:
+        json.loads(item)
+    except Exception:
+        try:
+            yaml.safe_load(item)
+        except Exception:  # Not YAML/JSON
+            return False
+        else:  # Is YAML
+            yml = Syntax(item, "YAML", padding=(0, ind), theme="fruity", word_wrap=True)
+            print()
+            console.log(yml)
+            return True
+    else:  # Is JSON
+        print()
+        print_json(item, indent=ind)
+        return True
+
+
+def table_generator(headers: list, items: list, header_style=None):
+    table = Table(show_header=True, header_style=header_style)
+    for header in headers:
+        table.add_column(header)
+    for item in items:
+        cells = []
+        for i in item:
+            if PASS_REGEX.search(i):
+                styled = "[green]" + i
+            elif FAIL_REGEX.search(i):
+                styled = "[red]" + i
+            elif UNKNOWN_REGEX.search(i):
+                styled = "[yellow]" + i
+            elif RUNNING_REGEX.search(i):
+                styled = "[blue]" + i
+            else:
+                styled = i
+            cells.append(styled)
+        table.add_row(*cells)
+    console.log(table)
+
+
+class argument:
+    def __init__(self) -> None:
+        self.id = str()
+        self.action = str()
+        self.profile = str()
+        self.debug = bool()
+        self.json = bool()
+        self.path = str()
+        self.data = Any
+        self.sync = bool()
+        self.timeout = int()
+        self.playbook = str()
+        self.page = int()
+        self.public = bool()
+
+
+def autotable(items: list[dict], header_style=None) -> None:
+    headers = []
+    # get headers
+    for i in items:
+        for h in i.keys():
+            if h not in headers:
+                headers.append(h)
+    rows = []
+    # get rows
+    for item in items:
+        row = []
+        for key in headers:
+            if key in item:
+                row.append(item[key])
+            else:
+                row.append("")
+        rows.append(row)
+    table_generator(headers, rows, header_style)
```

### Comparing `satori-ci-1.1.9/src/satorici/satori_module.py` & `satori_ci-1.2.4/src/satorici/satori_module.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-import argparse
+from argparse import ArgumentParser
 import sys
 from importlib import metadata
-
-from requests import HTTPError, Response
 from colorama import just_fix_windows_console, Fore, Back
 
 from satorici.classes.satori import Satori
-from satorici.classes.utils import autoformat, puts
+from satorici.classes.utils import puts
 
 VERSION = metadata.version("satori-ci")
 just_fix_windows_console()
 
 
-def add_satori_arguments(cmd):
+def add_satori_arguments(cmd: ArgumentParser):
     # satori-cli repo|report|monitor|... {id} {action} ...
-    cmd.add_argument("id", nargs="?", type=str, default="list")
-    cmd.add_argument("action", nargs="?", type=str, default="get")
+    cmd.add_argument("id", nargs="?", type=str, default="", help="Object ID")
+    cmd.add_argument(
+        "action", nargs="?", type=str, default="", help="Action to perform"
+    )
 
 
 def main():
     puts(
         Fore.LIGHTBLACK_EX,
         f"Satori CI {VERSION} - Automated Software Testing Platform",
         file=sys.stderr,
@@ -31,41 +31,51 @@
             "Minimum Python version 3.9 required, the current version is "
             f"{sys.version_info.major}.{sys.version_info.minor}\n"
             "How To Install Python 3.10 on Ubuntu:\n"
             "https://computingforgeeks.com/how-to-install-python-on-ubuntu-linux-system"
         )
         sys.exit(0)
 
-    baseparser = argparse.ArgumentParser(add_help=False)
+    baseparser = ArgumentParser(add_help=False)
     baseparser.add_argument("-p", "--profile", default="default")
     baseparser.add_argument("-j", "--json", action="store_true", help="JSON output")
     baseparser.add_argument("--debug", action="store_true", help="Debug mode")
+    baseparser.add_argument("--timeout", type=int, default=180, help="Request timeout")
+    baseparser.add_argument(
+        "--version", "-v", action="version", version=f"%(prog)s {VERSION}"
+    )
 
-    parser = argparse.ArgumentParser(parents=[baseparser])
+    parser = ArgumentParser(parents=[baseparser])
     subparsers = parser.add_subparsers(dest="subcommand")
 
     # config token "user_token"
     config_cmd = subparsers.add_parser("config", parents=[baseparser])
     config_cmd.add_argument("key")
     config_cmd.add_argument("value")
 
+    # dashboard
+    subparsers.add_parser("dashboard", parents=[baseparser])
+
     # run playbook.yml
     run_cmd = subparsers.add_parser("run", parents=[baseparser])
     run_cmd.add_argument("path")
     run_cmd.add_argument("-s", "--sync", default=False, action="store_true")
     run_cmd.add_argument("-d", "--data", type=str, default="", help="Secrets")
 
     # playbook {id} <delete>
     playbook_cmd = subparsers.add_parser("playbook", parents=[baseparser])
     playbook_cmd.add_argument(
         "-n", "--page", dest="page", type=int, default=1, help="Playbooks page number"
     )
     playbook_cmd.add_argument(
         "-l", "--limit", dest="limit", type=int, default=5, help="Page limit number"
     )
+    playbook_cmd.add_argument(
+        "--public", action="store_true", help="Fetch public satori playbooks"
+    )
     add_satori_arguments(playbook_cmd)
 
     # repo {id} <commits|check-commits|check-forks|scan|scan-stop|run|clean>
     repo_cmd = subparsers.add_parser("repo", parents=[baseparser])
     repo_cmd.add_argument("-c", "--coverage", type=float, default=1, help="coverage")
     repo_cmd.add_argument("--skip-check", default=False, action="store_true")
     repo_cmd.add_argument("-f", "--from", type=str, default="", help="From Date")
@@ -76,14 +86,15 @@
     repo_cmd.add_argument(
         "-b", "--branch", type=str, default="main", help="Repo branch"
     )
     repo_cmd.add_argument("--filter", type=str, help="Filter names")
     repo_cmd.add_argument("-a", "--all", default=False, action="store_true")
     repo_cmd.add_argument("-l", "--limit", type=int, default=100, help="Limit number")
     repo_cmd.add_argument("--fail", default=False, action="store_true")
+    repo_cmd.add_argument("--playbook", type=str, help="Playbook")
     add_satori_arguments(repo_cmd)
 
     # report {id} <output|stop|delete>
     report_cmd = subparsers.add_parser("report", parents=[baseparser])
     report_cmd.add_argument(
         "-n", "--page", type=int, default=1, help="Commit page number"
     )
@@ -96,30 +107,30 @@
         type=str,
         default="",
         help="Filters: from,to,satori_error,status",
     )
     add_satori_arguments(report_cmd)
 
     # monitor {id} <start|stop|delete>
-    monitor_cmd = subparsers.add_parser("monitor", parents=[baseparser])  # noqa: F841
+    monitor_cmd = subparsers.add_parser("monitor", parents=[baseparser])
     add_satori_arguments(monitor_cmd)
 
     # team {id} create|members|add_member|repos|add_repo
     team_cmd = subparsers.add_parser("team", parents=[baseparser])
     team_cmd.add_argument("--email", type=str, help="User email")
     team_cmd.add_argument("--role", type=str, default="READ", help="User role")
     team_cmd.add_argument("--repo", type=str, default=None, help="Repo name")
     add_satori_arguments(team_cmd)
 
     args = parser.parse_args()
 
     if args.subcommand == "config":
-        instance = Satori(args.profile, config=True)
+        instance = Satori(args, config=True)
     else:
-        instance = Satori(args.profile)
+        instance = Satori(args)
 
     try:
         if args.subcommand == "config":
             instance.save_config(args.key, args.value)
         elif args.subcommand == "run":
             instance.run(args)
         elif args.subcommand == "playbook":
@@ -133,20 +144,11 @@
         elif args.subcommand == "team":
             instance.team(args)
         elif args.subcommand in (None, "dashboard"):
             instance.dashboard(args)
     except KeyboardInterrupt:
         puts(Back.RED, "Interrupted by user")
         sys.exit(1)
-    except HTTPError as e:
-        res: Response = e.response
-        status = {"Status code": res.status_code}
-        status.update(res.json())
-        if args.json:
-            puts(Fore.RED, str(status))
-        else:
-            autoformat(status, capitalize=True, color=Fore.RED)
-        sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

