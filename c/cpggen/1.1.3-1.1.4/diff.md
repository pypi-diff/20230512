# Comparing `tmp/cpggen-1.1.3.tar.gz` & `tmp/cpggen-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.1.3.tar", max compression
+gzip compressed data, was "cpggen-1.1.4.tar", max compression
```

## Comparing `cpggen-1.1.3.tar` & `cpggen-1.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-12 16:06:01.399358 cpggen-1.1.3/LICENSE
--rw-r--r--   0        0        0    11802 2023-05-12 16:06:01.399358 cpggen-1.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-12 16:06:01.399358 cpggen-1.1.3/cpggen/__init__.py
--rw-r--r--   0        0        0    19898 2023-05-12 16:06:01.399358 cpggen-1.1.3/cpggen/cli.py
--rw-r--r--   0        0        0    37900 2023-05-12 16:06:01.399358 cpggen-1.1.3/cpggen/executor.py
--rw-r--r--   0        0        0     1015 2023-05-12 16:06:01.399358 cpggen-1.1.3/cpggen/logger.py
--rw-r--r--   0        0        0    14556 2023-05-12 16:06:01.403359 cpggen-1.1.3/cpggen/utils.py
--rw-r--r--   0        0        0     1326 2023-05-12 16:06:01.403359 cpggen-1.1.3/pyproject.toml
--rw-r--r--   0        0        0    13174 1970-01-01 00:00:00.000000 cpggen-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 21:35:17.130652 cpggen-1.1.4/LICENSE
+-rw-r--r--   0        0        0    11907 2023-05-12 21:35:17.130652 cpggen-1.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 21:35:17.134652 cpggen-1.1.4/cpggen/__init__.py
+-rw-r--r--   0        0        0    20677 2023-05-12 21:35:17.134652 cpggen-1.1.4/cpggen/cli.py
+-rw-r--r--   0        0        0    39149 2023-05-12 21:35:17.134652 cpggen-1.1.4/cpggen/executor.py
+-rw-r--r--   0        0        0     1078 2023-05-12 21:35:17.134652 cpggen-1.1.4/cpggen/logger.py
+-rw-r--r--   0        0        0    14556 2023-05-12 21:35:17.134652 cpggen-1.1.4/cpggen/utils.py
+-rw-r--r--   0        0        0     1326 2023-05-12 21:35:17.134652 cpggen-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0    13279 1970-01-01 00:00:00.000000 cpggen-1.1.4/PKG-INFO
```

### Comparing `cpggen-1.1.3/LICENSE` & `cpggen-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.3/README.md` & `cpggen-1.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.3/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.4/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.3/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.4/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -283,14 +283,15 @@
 | CPGGEN_MEMORY           | Heap memory to use for frontends. Default computed                         |
 | AT_DEBUG_MODE           | Set to debug to enable debug logging                                       |
 | CPG_EXPORT              | Set to true to export CPG graphs in dot format                             |
 | CPG_EXPORT_REPR         | Graph to export. Default all                                               |
 | CPG_EXPORT_FORMAT       | Export format. Default dot                                                 |
 | CPG_SLICE               | Set to true to slice CPG                                                   |
 | CPG_SLICE_MODE          | Slice mode. Default Usages                                                 |
+| CPG_VECTORS             | Set to true to generate vector representations of code from CPG            |
 | SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI               |
 | CDXGEN_ARGS             | Extra arguments to pass to cdxgen                                          |
 | ENABLE_SBOM             | Enable SBoM generation using cdxgen                                        |
 | JIMPLE_ANDROID_JAR      | Path to android.jar for use with jimple for .apk or .dex to CPG conversion |
 
 ## GitHub actions
```

### Comparing `cpggen-1.1.3/cpggen/cli.py` & `cpggen-1.1.4/cpggen/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,14 +158,21 @@
     parser.add_argument(
         "--use-parse",
         dest="use_parse",
         help="Use joern-parse command instead of invoking the language frontends. Useful when default overlays are important",
         action="store_true",
         default=False,
     )
+    parser.add_argument(
+        "--vectors",
+        action="store_true",
+        default=True if os.getenv("CPG_VECTORS") in ("true", "1") else False,
+        dest="vectors",
+        help="Extract vector representations of code from CPG",
+    )
     return parser.parse_args()
 
 
 @app.get("/")
 async def index():
     return {}
 
@@ -195,28 +202,31 @@
     skip_sbom = True
     export = False
     slice = False
     use_parse = False
     slice_mode = "Usages"
     app_manifest_list = []
     errors_warnings = []
+    vectors = False
     if not params:
         params = {}
     if q.get("url"):
         url = q.get("url")
     if q.get("src"):
         src = q.get("src")
     if q.get("out_dir"):
         cpg_out_dir = q.get("out_dir")
     if q.get("lang"):
         languages = q.get("lang")
     if q.get("export", "") in ("true", "1"):
         export = True
     if q.get("slice", "") in ("true", "1"):
         slice = True
+    if q.get("vectors", "") in ("true", "1"):
+        vectors = True
     if q.get("slice_mode"):
         slice_mode = q.get("slice_mode")
     if q.get("auto_build", "") in ("false", "0"):
         auto_build = False
     if q.get("skip_sbom", "") in ("false", "0"):
         skip_sbom = False
     if not url and params.get("url"):
@@ -231,14 +241,16 @@
         auto_build = False
     if params.get("skip_sbom", "") in ("false", "0"):
         skip_sbom = False
     if params.get("export", "") in ("true", "1"):
         export = True
     if params.get("slice", "") in ("true", "1"):
         slice = True
+    if params.get("vectors", "") in ("true", "1"):
+        vectors = True
     if params.get("slice_mode"):
         slice_mode = params.get("slice_mode")
     if not src and not url:
         return {"error": "true", "message": "path or url is required"}, 500
     # If src contains url, then reassign
     if not url and (
         src.startswith("http") or src.startswith("git://") or src.startswith("pkg:")
@@ -279,14 +291,15 @@
             use_parse=use_parse,
             auto_build=auto_build,
             extra_args={
                 "skip_sbom": skip_sbom,
                 "slice_mode": slice_mode,
                 "for_export": export,
                 "for_slice": slice,
+                "for_vectors": vectors,
                 "url": url,
             },
         )
         if mlist:
             app_manifest_list += mlist
         if slice and mlist:
             for ml in mlist:
@@ -347,14 +360,15 @@
     use_parse=False,
     auto_build=False,
     skip_sbom=False,
     export=False,
     slice=False,
     slice_mode=None,
     url=None,
+    vectors=False,
 ):
     if __name__ in ("__main__", "cpggen.cli"):
         with Pool(processes=os.cpu_count(), initializer=init_worker) as pool:
             try:
                 for lang in languages:
                     LOG.debug(f"Generating CPG for the language {lang} at {src}")
                     pool.apply_async(
@@ -369,14 +383,15 @@
                             use_parse,
                             auto_build,
                             {
                                 "skip_sbom": skip_sbom,
                                 "slice_mode": slice_mode,
                                 "for_export": export,
                                 "for_slice": slice,
+                                "for_vectors": vectors,
                                 "url": url,
                             },
                         ),
                     )
                 pool.close()
             except KeyboardInterrupt:
                 pool.terminate()
@@ -405,18 +420,24 @@
     use_parse,
     export,
     export_repr,
     export_format,
     export_out_dir,
     slice,
     slice_mode,
+    vectors,
 ):
     if __name__ in ("__main__", "cpggen.cli"):
         with Pool(processes=os.cpu_count(), initializer=init_worker) as pool:
             try:
+                export_tool = "export"
+                if slice:
+                    export_tool = "slice"
+                elif vectors:
+                    export_tool = "vectors"
                 cpg_manifests = collect_cpg_manifests(cpg_out_dir)
                 for amanifest in cpg_manifests:
                     with open(amanifest) as mfp:
                         manifest_obj = json.load(mfp)
                         if not manifest_obj or not manifest_obj.get("cpg"):
                             continue
                         app_export_out_dir = os.path.join(
@@ -447,15 +468,15 @@
                         if export:
                             LOG.debug(
                                 f"""Exporting CPG for the app {manifest_obj["app"]} from {cpg_path} to {app_export_out_dir}"""
                             )
                         pool.apply_async(
                             executor.exec_tool,
                             (
-                                "export" if export else "slice",
+                                export_tool,
                                 cpg_path,
                                 app_export_out_dir,
                                 cpg_out_dir,
                                 joern_home,
                                 use_container,
                                 use_parse,
                                 False,
@@ -562,28 +583,30 @@
         use_parse=use_parse,
         auto_build=args.auto_build,
         skip_sbom=args.skip_sbom,
         export=args.export,
         slice=args.slice,
         slice_mode=args.slice_mode,
         url=url,
+        vectors=args.vectors,
     )
-    if args.export or args.slice:
+    if args.export or args.slice or args.vectors:
         export_slice_cpg(
             src,
             cpg_out_dir,
             joern_home=joern_home,
             use_container=use_container,
             use_parse=use_parse,
             export=args.export,
             export_repr=args.export_repr,
             export_format=args.export_format,
             export_out_dir=export_out_dir,
             slice=args.slice,
             slice_mode=args.slice_mode,
+            vectors=args.vectors,
         )
     if is_temp_dir:
         try:
             shutil.rmtree(src)
         except Exception:
             # Ignore cleanup errors
             pass
```

### Comparing `cpggen-1.1.3/cpggen/executor.py` & `cpggen-1.1.4/cpggen/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     "jar": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jar-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "scala": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nojsp --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "sbom": "%(cdxgen_cmd)s%(exe_ext)s%(cdxgen_args)s -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
     "parse": "%(joern_home)sjoern-parse%(only_bat_ext)s -J-Xmx%(memory)s --language %(parse_lang)s --output %(cpg_out)s %(src)s",
+    "vectors": "%(joern_home)sjoern-vectors%(only_bat_ext)s -J-Xmx%(memory)s --out %(cpg_out)s %(src)s",
     "export": "%(joern_home)sjoern-export%(only_bat_ext)s -J-Xmx%(memory)s --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
     "slice": "%(joern_home)sjoern-slice%(only_bat_ext)s -J-Xmx%(memory)s --dummy-types true --exclude-operators true -m %(slice_mode)s --out %(slice_out)s %(cpg_out)s",
     "qwiet": "sl%(exe_ext)s analyze %(policy)s%(vcs_correction)s--tag app.group=%(group)s --app %(app)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
     "dot2png": "dot -Tpng %(dot_file)s -o %(png_out)s",
 }
 
 cpg_tools_map["npm"] = cpg_tools_map["js"]
@@ -224,14 +225,15 @@
     "go": "golang",
     "csharp": "csharp",
     "dotnet": "csharp",
     "cpp": "newc",
     "c": "newc",
     "binary": "ghidra",
     "ruby": "rubysrc",
+    "jimple": "java",
 }
 
 
 def qwiet_analysis(app_manifest, src, cwd, env):
     try:
         relative_path = os.path.relpath(cwd, src)
         if relative_path and not relative_path.startswith(".."):
@@ -467,14 +469,16 @@
                 stdout = subprocess.PIPE
                 stderr = stdout
             tool_verb = f"Building CPG with {tool_lang} frontend"
             if tool_lang == "export":
                 tool_verb = "Exporting CPG with joern-export"
             elif tool_lang == "slice":
                 tool_verb = "Slicing CPG with joern-slice"
+            elif tool_lang == "vectors":
+                tool_verb = "Generating CPG vectors with joern-vectors"
             task = progress.add_task(
                 "[green]" + tool_verb,
                 total=100,
                 start=False,
             )
             cpg_cmd_lang = tool_lang
             # If the intention is to export or slice then use joern-parse
@@ -543,15 +547,15 @@
                     else os.path.abspath(
                         os.path.join(
                             cpg_out_dir,
                             f"{os.path.basename(amodule)}-{tool_lang_simple}-cpg.bin.zip",
                         )
                     )
                 )
-                if tool_lang == "export":
+                if tool_lang in ("export", "vectors"):
                     cpg_out = os.path.abspath(cpg_out_dir)
                 elif tool_lang == "slice":
                     if not slice_out:
                         slice_out = cpg_out.replace(".bin.zip", ".slices")
                     cpg_out = src
                 else:
                     sbom_out = (
@@ -629,15 +633,15 @@
                         )
                     else:
                         LOG.warn(
                             f"{lang_cmd} is not found. Ensure the PATH variable in your container image is set to the bin directory of Joern."
                         )
                     return
                 # Is this an Export or Slice task?
-                if tool_lang in ("export", "slice"):
+                if tool_lang in ("export", "slice", "vectors"):
                     try:
                         progress.update(
                             task,
                             description=f"{tool_lang.capitalize()} CPG",
                             completed=90,
                             total=100,
                         )
@@ -647,14 +651,21 @@
                             stderr=stderr,
                             cwd=cwd,
                             env=env,
                             check=False,
                             shell=use_shell,
                             encoding="utf-8",
                         )
+                        # Bug. joern-vectors doesn't create json
+                        if tool_lang == "vectors" and cp and cp.stdout:
+                            os.makedirs(cpg_out_dir, exist_ok=True)
+                            with open(
+                                os.path.join(cpg_out_dir, "vectors.json"), mode="w"
+                            ) as fp:
+                                fp.write(cp.stdout)
                         if cp and cp.returncode and cp.stderr:
                             LOG.warn(
                                 f"{tool_lang.capitalize()} operation has failed for {src}"
                             )
                             if not os.getenv("AT_DEBUG_MODE"):
                                 LOG.info(
                                     "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
@@ -666,20 +677,31 @@
                                 LOG.info(cp.stderr)
                                 LOG.info("------------------------------")
                                 LOG.info(
                                     f"Command used {' '.join(cmd_list_with_args)}\nPlease report the above error to https://github.com/joernio/joern/issues"
                                 )
                         else:
                             check_dir = (
-                                cpg_out_dir if tool_lang == "export" else slice_out
+                                cpg_out_dir
+                                if tool_lang in ("export")
+                                else (
+                                    os.path.join(cpg_out_dir, "vectors.json")
+                                    if tool_lang == "vectors"
+                                    else slice_out
+                                )
                             )
                             if os.path.exists(check_dir):
-                                LOG.info(
-                                    f"CPG {src} successfully {tool_lang + ('d' if tool_lang.endswith('e') else 'ed')} to {check_dir}"
-                                )
+                                if tool_lang == "vectors":
+                                    LOG.info(
+                                        f"CPG {src} successfully vectorized to {check_dir}"
+                                    )
+                                else:
+                                    LOG.info(
+                                        f"CPG {src} successfully {tool_lang + ('d' if tool_lang.endswith('e') else 'ed')} to {check_dir}"
+                                    )
                                 # Convert dot files to png
                                 if tool_lang == "export":
                                     progress.update(
                                         task,
                                         description="Convert exported graph to png",
                                         completed=95,
                                         total=100,
```

### Comparing `cpggen-1.1.3/cpggen/logger.py` & `cpggen-1.1.4/cpggen/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
 import os
 
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.theme import Theme
 
+for _ in ("httpx",):
+    logging.getLogger(_).disabled = True
+
 custom_theme = Theme({"info": "cyan", "warning": "purple4", "danger": "bold red"})
 console = Console(
     log_time=False,
     log_path=False,
     theme=custom_theme,
     width=280,
     color_system="256",
```

### Comparing `cpggen-1.1.3/cpggen/utils.py` & `cpggen-1.1.4/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.3/pyproject.toml` & `cpggen-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.1.3"
+version = "1.1.4"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-1.1.3/PKG-INFO` & `cpggen-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.1.3
+Version: 1.1.4
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8.1,<3.12
@@ -60,23 +60,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.3/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.4/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.3/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.4/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -316,14 +316,15 @@
 | CPGGEN_MEMORY           | Heap memory to use for frontends. Default computed                         |
 | AT_DEBUG_MODE           | Set to debug to enable debug logging                                       |
 | CPG_EXPORT              | Set to true to export CPG graphs in dot format                             |
 | CPG_EXPORT_REPR         | Graph to export. Default all                                               |
 | CPG_EXPORT_FORMAT       | Export format. Default dot                                                 |
 | CPG_SLICE               | Set to true to slice CPG                                                   |
 | CPG_SLICE_MODE          | Slice mode. Default Usages                                                 |
+| CPG_VECTORS             | Set to true to generate vector representations of code from CPG            |
 | SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI               |
 | CDXGEN_ARGS             | Extra arguments to pass to cdxgen                                          |
 | ENABLE_SBOM             | Enable SBoM generation using cdxgen                                        |
 | JIMPLE_ANDROID_JAR      | Path to android.jar for use with jimple for .apk or .dex to CPG conversion |
 
 ## GitHub actions
```

