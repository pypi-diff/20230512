# Comparing `tmp/consolo-0.2.5.tar.gz` & `tmp/consolo-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consolo-0.2.5.tar", last modified: Thu Mar  9 16:24:14 2023, max compression
+gzip compressed data, was "consolo-0.2.6.tar", last modified: Fri May 12 16:12:48 2023, max compression
```

## Comparing `consolo-0.2.5.tar` & `consolo-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-01-30 17:06:51.935441 consolo-0.2.5/LICENSE
--rw-r--r--   0        0        0     2507 2023-03-09 14:58:26.423097 consolo-0.2.5/README.md
--rw-r--r--   0        0        0      823 2023-03-09 16:23:40.685333 consolo-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        1 2023-03-09 14:20:21.843320 consolo-0.2.5/src/consolo/__init__.py
--rwxr-xr-x   0        0        0    11214 2023-03-09 16:08:31.739553 consolo-0.2.5/src/consolo/consolo.py
--rw-r--r--   0        0        0     3035 1970-01-01 00:00:00.000000 consolo-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-01-30 17:06:51.935441 consolo-0.2.6/LICENSE
+-rw-r--r--   0        0        0     6224 2023-05-12 16:12:29.441117 consolo-0.2.6/README.md
+-rw-r--r--   0        0        0      823 2023-05-12 16:12:43.085145 consolo-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-03-09 14:20:21.843320 consolo-0.2.6/src/consolo/__init__.py
+-rwxr-xr-x   0        0        0    12510 2023-05-12 14:47:34.137046 consolo-0.2.6/src/consolo/consolo.py
+-rw-r--r--   0        0        0     6752 1970-01-01 00:00:00.000000 consolo-0.2.6/PKG-INFO
```

### Comparing `consolo-0.2.5/LICENSE` & `consolo-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `consolo-0.2.5/pyproject.toml` & `consolo-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "consolo"
-version = "0.2.5"
+version = "0.2.6"
 description = "Utility for pseudo-mounting an AWS lambda filesystem locally"
 authors = [
     { name = "Ashton Honnecke", email = "ashton@pixelstub.com" },
 ]
 dependencies = [
     "argdantic>=0.3.0",
     "boto3>=1.26.87",
```

### Comparing `consolo-0.2.5/src/consolo/consolo.py` & `consolo-0.2.6/src/consolo/consolo.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,35 +99,51 @@
 
 class LambdaReloader(LambdaWrapper):
     """Map an AWS function onto a local dir."""
 
     def __init__(
         self,
         profile_name: str,
-        function_name: str,
         local_root: str,
         allow_file_creation: bool,
+        function_name: str = None,
     ) -> None:
         """Set AWS profile, AWS function name and local path to src."""
         self.profile_name = profile_name
-        self.function_name = function_name
         self.local_root = Path(local_root)
+        self.config = {}
+
+        if not function_name:
+            self.read_config()
+            function_name = self.load_function_name()
+
+        self.function_name = function_name
+        if not self.function_name:
+            print("Unable to determine function name.")
+            exit()
+
+        self.config = {"function_name": self.function_name}
+        self.write_config()
+
         self.allow_file_creation = allow_file_creation
         self.suppressed_uploads = False
 
     @property
     def archive_dir(self) -> Path:
         """Location for building archive of function."""
         return Path("/tmp")
 
     @property
     def archive(self) -> Path:
         """Get the archive filename."""
         return self.archive_dir.joinpath(".".join([self.function_name, "zip"]))
 
+    def load_function_name(self):
+        return self.config.get("function_name")
+
     def validate_root(self) -> bool:
         """Raise if destination directory does not exist."""
         if not os.path.isdir(self.local_root):
             raise RuntimeError(f"Local dir {self.local_root} does not exist.")
 
         return True
 
@@ -155,14 +171,35 @@
         return self.archive_dir.joinpath(f".consolo.{self.function_name}.json")
 
     def write_manifest(self) -> None:
         """Write the in memory list of files to local storate."""
         with open(self.manifest_path, "w", encoding="utf-8") as f:
             return json.dump(self.manifest, f, ensure_ascii=False, indent=4)
 
+    def read_config(self):
+        """Read the local list of files in the lambda."""
+
+        try:
+            with open(self.config_path, "r", encoding="utf-8") as f:
+                self.config = json.load(f)
+
+            return self.config
+        except Exception:
+            return {}
+
+    @property
+    def config_path(self) -> Path:
+        """Path to the local config file."""
+        return self.local_root.joinpath(".consolo.config.json")
+
+    def write_config(self) -> None:
+        """Write the in memory list of files to local storate."""
+        with open(self.config_path, "w", encoding="utf-8") as f:
+            return json.dump(self.config, f, ensure_ascii=False, indent=4)
+
     def expand_function_code(self) -> None:
         """Unpack the archive."""
         shutil.unpack_archive(self.archive, self.local_root)
 
     def clobber_local(self) -> None:
         """Download AWS lambda onto local directory.
 
@@ -236,14 +273,15 @@
             response = self.lambda_client.update_function_code(
                 FunctionName=self.function_name, ZipFile=self.read_archive()
             )
         except ClientError as err:
             if err.response["Error"]["Code"] == "ResourceConflictException":
                 # TODO: suppress this
                 logger.debug("Tried to upload while uploading.")
+                logger.info("Please ensure you are not editing in the console.")
                 self.suppressed_uploads = True
                 return
 
             logger.error(
                 "Couldn't update function %s. Here's why: %s: %s",
                 self.function_name,
                 err.response["Error"]["Code"],
@@ -302,32 +340,34 @@
 
 parser = ArgParser()
 
 
 @parser.command()
 def _main(
     profile_name: str,
-    function_name: str,
     path: str,
+    function_name: str = None,
     upload: bool = False,
     download: bool = False,
     create: bool = False,
     verbose: bool = False,
 ) -> None:
     """Entrypoint for AWS lambda hot reloader, CLI args in signature."""
     log_level = "INFO"
     if verbose:
         log_level = "DEBUG"
 
     logging.basicConfig(level=log_level)
 
+    relative_path = path
+    path = Path(relative_path).absolute()
+
     reloader = LambdaReloader(
-        profile_name, function_name, path, allow_file_creation=create
+        profile_name, path, allow_file_creation=create, function_name=function_name,
     )
-
     reloader.validate_root()
 
     if upload and not download:
         print("Not supported yet.")
         exit(1)
         reloader.update_function_code()
     elif download and not upload:
```

