# Comparing `tmp/cpggen-1.1.1.tar.gz` & `tmp/cpggen-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.1.1.tar", max compression
+gzip compressed data, was "cpggen-1.1.2.tar", max compression
```

## Comparing `cpggen-1.1.1.tar` & `cpggen-1.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-10 01:53:37.866433 cpggen-1.1.1/LICENSE
--rw-r--r--   0        0        0    11604 2023-05-10 01:53:37.866433 cpggen-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-10 01:53:37.866433 cpggen-1.1.1/cpggen/__init__.py
--rw-r--r--   0        0        0    19564 2023-05-10 01:53:37.866433 cpggen-1.1.1/cpggen/cli.py
--rw-r--r--   0        0        0    37417 2023-05-10 01:53:37.870433 cpggen-1.1.1/cpggen/executor.py
--rw-r--r--   0        0        0     1015 2023-05-10 01:53:37.870433 cpggen-1.1.1/cpggen/logger.py
--rw-r--r--   0        0        0    14143 2023-05-10 01:53:37.870433 cpggen-1.1.1/cpggen/utils.py
--rw-r--r--   0        0        0     1326 2023-05-10 01:53:37.870433 cpggen-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    12976 1970-01-01 00:00:00.000000 cpggen-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 13:54:12.748805 cpggen-1.1.2/LICENSE
+-rw-r--r--   0        0        0    11802 2023-05-12 13:54:12.748805 cpggen-1.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 13:54:12.748805 cpggen-1.1.2/cpggen/__init__.py
+-rw-r--r--   0        0        0    19698 2023-05-12 13:54:12.748805 cpggen-1.1.2/cpggen/cli.py
+-rw-r--r--   0        0        0    37900 2023-05-12 13:54:12.748805 cpggen-1.1.2/cpggen/executor.py
+-rw-r--r--   0        0        0     1015 2023-05-12 13:54:12.748805 cpggen-1.1.2/cpggen/logger.py
+-rw-r--r--   0        0        0    14556 2023-05-12 13:54:12.748805 cpggen-1.1.2/cpggen/utils.py
+-rw-r--r--   0        0        0     1326 2023-05-12 13:54:12.748805 cpggen-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    13174 1970-01-01 00:00:00.000000 cpggen-1.1.2/PKG-INFO
```

### Comparing `cpggen-1.1.1/LICENSE` & `cpggen-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.1/README.md` & `cpggen-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.1/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.2/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.1/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.2/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -193,24 +193,28 @@
 
 cpggen can run in server mode.
 
 ```
 cpggen --server
 ```
 
-You can invoke the endpoint `/cpg` to generate CPG.
+You can invoke the endpoint `/cpg` to generate CPG from a path, http or package url. Parameters can be passed using GET or POST request.
 
 ```
 curl "http://127.0.0.1:7072/cpg?src=/Volumes/Work/sandbox/vulnerable-aws-koa-app&out_dir=/tmp/cpg_out&lang=js"
 ```
 
 ```
 curl "http://127.0.0.1:7072/cpg?url=https://github.com/HooliCorp/vulnerable-aws-koa-app&out_dir=/tmp/cpg_out&lang=js"
 ```
 
+```
+curl "http://127.0.0.1:7072/cpg?url=pkg:maven/org.apache.commons/commons-io@1.3.2&out_dir=/tmp/cpg_out"
+```
+
 ## Languages supported
 
 | Language    | Requires build | Maturity |
 | ----------- | -------------- | -------- |
 | C           | No             | High     |
 | C++         | No             | High     |
 | Java        | No (\*)        | Medium   |
```

### Comparing `cpggen-1.1.1/cpggen/cli.py` & `cpggen-1.1.2/cpggen/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,14 +274,15 @@
             use_parse=use_parse,
             auto_build=auto_build,
             extra_args={
                 "skip_sbom": skip_sbom,
                 "slice_mode": slice_mode,
                 "for_export": export,
                 "for_slice": slice,
+                "url": url,
             },
         )
         if mlist:
             app_manifest_list += mlist
         if slice and mlist:
             for ml in mlist:
                 if not os.path.exists(ml.get("cpg")):
@@ -340,14 +341,15 @@
     use_container=False,
     use_parse=False,
     auto_build=False,
     skip_sbom=False,
     export=False,
     slice=False,
     slice_mode=None,
+    url=None,
 ):
     if __name__ in ("__main__", "cpggen.cli"):
         with Pool(processes=os.cpu_count(), initializer=init_worker) as pool:
             try:
                 for lang in languages:
                     LOG.debug(f"Generating CPG for the language {lang} at {src}")
                     pool.apply_async(
@@ -362,14 +364,15 @@
                             use_parse,
                             auto_build,
                             {
                                 "skip_sbom": skip_sbom,
                                 "slice_mode": slice_mode,
                                 "for_export": export,
                                 "for_slice": slice,
+                                "url": url,
                             },
                         ),
                     )
                 pool.close()
             except KeyboardInterrupt:
                 pool.terminate()
             pool.join()
@@ -516,15 +519,17 @@
             console.print(
                 "Alternatively, ensure docker or podman is available to use cpggen container image"
             )
     # GitHub action is very weird
     if os.getenv("GITHUB_PATH") and utils.check_command("joern"):
         joern_home = ""
     is_temp_dir = False
+    url = ""
     if src.startswith("http") or src.startswith("git://") or src.startswith("pkg:"):
+        url = src
         clone_dir = tempfile.mkdtemp(prefix="cpggen")
         if src.startswith("pkg:"):
             download_file = utils.download_package(src, clone_dir)
             if download_file and os.path.exists(download_file):
                 src = clone_dir
         else:
             src = utils.clone_repo(src, clone_dir)
@@ -548,14 +553,15 @@
         use_container=use_container,
         use_parse=use_parse,
         auto_build=args.auto_build,
         skip_sbom=args.skip_sbom,
         export=args.export,
         slice=args.slice,
         slice_mode=args.slice_mode,
+        url=url,
     )
     if args.export or args.slice:
         export_slice_cpg(
             src,
             cpg_out_dir,
             joern_home=joern_home,
             use_container=use_container,
```

### Comparing `cpggen-1.1.1/cpggen/executor.py` & `cpggen-1.1.2/cpggen/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     find_files,
     find_go_mods,
     find_gradle_files,
     find_java_artifacts,
     find_makefiles,
     find_pom_files,
     find_sbt_files,
+    to_friendly_name,
 )
 
 runtimeValues = {}
 svmem = psutil.virtual_memory()
 max_memory = bytes2human(getattr(svmem, "available"), format="%(value).0f%(symbol)s")
 cpu_count = str(psutil.cpu_count())
 
@@ -123,17 +124,14 @@
     "cpp-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
     "java": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "java-with-deps": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.m2",
     "java-with-gradle-deps": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.gradle/caches/modules-2/files-2.1",
     "jimple": "%(joern_home)sjimple2cpg%(only_bat_ext)s%(android_jar)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "binary": "%(joern_home)sghidra2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "js": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "ts": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "javascript": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "typescript": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin-with-deps": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --download-dependencies",
     "kotlin-with-classpath": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --classpath %(home_dir)s/.m2 --classpath %(home_dir)s/.gradle/caches/modules-2/files-2.1",
     "php": "%(joern_home)sphp2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "python": "%(joern_home)spysrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "csharp": "%(joern_home)sbin%(os_path_sep)scsharp2cpg%(exe_ext)s -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-errors --no-log-file --ignore-tests -l error",
     "dotnet": "%(joern_home)sbin%(os_path_sep)scsharp2cpg%(exe_ext)s -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-errors --no-log-file --ignore-tests -l error",
@@ -147,14 +145,23 @@
     "parse": "%(joern_home)sjoern-parse%(only_bat_ext)s -J-Xmx%(memory)s --language %(parse_lang)s --output %(cpg_out)s %(src)s",
     "export": "%(joern_home)sjoern-export%(only_bat_ext)s -J-Xmx%(memory)s --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
     "slice": "%(joern_home)sjoern-slice%(only_bat_ext)s -J-Xmx%(memory)s --dummy-types true --exclude-operators true -m %(slice_mode)s --out %(slice_out)s %(cpg_out)s",
     "qwiet": "sl%(exe_ext)s analyze %(policy)s%(vcs_correction)s--tag app.group=%(group)s --app %(app)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
     "dot2png": "dot -Tpng %(dot_file)s -o %(png_out)s",
 }
 
+cpg_tools_map["npm"] = cpg_tools_map["js"]
+cpg_tools_map["ts"] = cpg_tools_map["js"]
+cpg_tools_map["javascript"] = cpg_tools_map["js"]
+cpg_tools_map["typescript"] = cpg_tools_map["js"]
+cpg_tools_map["maven"] = cpg_tools_map["jimple"]
+cpg_tools_map["pypi"] = cpg_tools_map["python"]
+cpg_tools_map["nuget"] = cpg_tools_map["csharp"]
+cpg_tools_map["golang"] = cpg_tools_map["go"]
+
 build_tools_map = {
     "csharp": ["dotnet", "build"],
     "jar": {
         "maven": [
             get("MVN_CMD", "%(maven_cmd)s"),
             "compile",
             "package",
@@ -476,25 +483,25 @@
                 and (extra_args.get("for_export") or extra_args.get("for_slice"))
             ):
                 cpg_cmd_lang = "parse"
             cmd_with_args = cpg_tools_map.get(cpg_cmd_lang)
             if not cmd_with_args:
                 return
             # Perform build first
-            if auto_build or build_tools_map.get(tool_lang):
+            if build_tools_map.get(tool_lang):
                 if os.getenv("CI"):
-                    LOG.info(
+                    LOG.debug(
                         f"Automatically building {src} for {tool_lang}. To speed up this step, cache the build dependencies using the CI cache settings."
                     )
                 elif use_container:
-                    LOG.info(
+                    LOG.debug(
                         f"Attempting to build {src} for {tool_lang} using the bundled build tools from the container image."
                     )
                 else:
-                    LOG.info(
+                    LOG.debug(
                         f"Attempting to build {src} for {tool_lang} using the locally available build tools.\nFor better results, please ensure the correct version of these tools are installed for your application.\nAlternatively, use container image based execution."
                     )
                 lang_build_crashes[tool_lang] = do_build(tool_lang, src, cwd, env)
             uber_jar = ""
             csharp_artifacts = ""
             # For languages like scala, jsp or jar we need to create a uber jar containing all jar, war files from the source directory
             if "uber_jar" in cmd_with_args:
@@ -779,18 +786,25 @@
                         # Let's improve the name for github action
                         if app_base_name == "workspace" and os.getenv(
                             "GITHUB_REPOSITORY"
                         ):
                             app_base_name = os.getenv("GITHUB_REPOSITORY").split("/")[
                                 -1
                             ]
+                        full_app_name = extra_args.get(
+                            "full_app_name", f"{app_base_name}-{language}"
+                        )
+                        if extra_args.get("url") and extra_args.get("url").startswith(
+                            "pkg:"
+                        ):
+                            full_app_name = to_friendly_name(extra_args.get("url"))
                         app_manifest = {
                             "src": amodule,
                             "group": app_base_name,
-                            "app": f"{app_base_name}-{language}",
+                            "app": full_app_name,
                             "cpg": cpg_out,
                             "sbom": sbom_out,
                             "slice_out": slice_out,
                             "language": language,
                             "tool_lang": tool_lang,
                             "cpg_frontend_invocation": " ".join(cmd_list_with_args),
                             "sbom_invocation": " ".join(sbom_cmd_list_with_args),
```

### Comparing `cpggen-1.1.1/cpggen/logger.py` & `cpggen-1.1.2/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.1/cpggen/utils.py` & `cpggen-1.1.2/cpggen/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -327,14 +327,19 @@
     is_java_like = False
     home_dir = str(Path.home())
     maven_cache = os.path.join(home_dir, ".m2")
     gradle_cache = os.path.join(home_dir, ".gradle", "caches", "modules-2", "files-2.1")
     maven_cache_exists = os.path.exists(maven_cache)
     gradle_cache_exists = os.path.exists(gradle_cache)
     project_types = []
+    # Is this a package url
+    if src_dir.startswith("pkg:"):
+        purl_data = PackageURL.from_string(src_dir)
+        if purl_data and purl_data.type:
+            return [purl_data.type]
     if find_python_reqfiles(src_dir) or find_files(src_dir, ".py", False, True):
         project_types.append("python")
     if find_files(src_dir, "composer.json", False, True) or find_files(
         src_dir, ".php", False, True
     ):
         project_types.append("php")
     if find_files(src_dir, ".sbt", False, True) or find_files(
@@ -474,7 +479,15 @@
                 download_task = progress.add_task("Download", total=total)
                 for chunk in response.iter_bytes():
                     download_file.write(chunk)
                     progress.update(
                         download_task, completed=response.num_bytes_downloaded
                     )
                 return download_file.name
+
+
+def to_friendly_name(purl_str):
+    """Convert package url to a friendly name"""
+    purl_data = PackageURL.from_string(purl_str)
+    name = purl_data.name
+    version = purl_data.version
+    return f"{name}-{version}"
```

### Comparing `cpggen-1.1.1/pyproject.toml` & `cpggen-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.1.1"
+version = "1.1.2"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-1.1.1/PKG-INFO` & `cpggen-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.1.1
+Version: 1.1.2
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
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.1/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.2/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.1/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.2/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -226,24 +226,28 @@
 
 cpggen can run in server mode.
 
 ```
 cpggen --server
 ```
 
-You can invoke the endpoint `/cpg` to generate CPG.
+You can invoke the endpoint `/cpg` to generate CPG from a path, http or package url. Parameters can be passed using GET or POST request.
 
 ```
 curl "http://127.0.0.1:7072/cpg?src=/Volumes/Work/sandbox/vulnerable-aws-koa-app&out_dir=/tmp/cpg_out&lang=js"
 ```
 
 ```
 curl "http://127.0.0.1:7072/cpg?url=https://github.com/HooliCorp/vulnerable-aws-koa-app&out_dir=/tmp/cpg_out&lang=js"
 ```
 
+```
+curl "http://127.0.0.1:7072/cpg?url=pkg:maven/org.apache.commons/commons-io@1.3.2&out_dir=/tmp/cpg_out"
+```
+
 ## Languages supported
 
 | Language    | Requires build | Maturity |
 | ----------- | -------------- | -------- |
 | C           | No             | High     |
 | C++         | No             | High     |
 | Java        | No (\*)        | Medium   |
```

