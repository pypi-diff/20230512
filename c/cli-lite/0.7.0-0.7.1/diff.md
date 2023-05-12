# Comparing `tmp/cli-lite-0.7.0.tar.gz` & `tmp/cli-lite-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-lite-0.7.0.tar", last modified: Fri May 12 08:39:46 2023, max compression
+gzip compressed data, was "cli-lite-0.7.1.tar", last modified: Fri May 12 11:28:31 2023, max compression
```

## Comparing `cli-lite-0.7.0.tar` & `cli-lite-0.7.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      160 2023-05-12 07:56:09.908946 cli-lite-0.7.0/clilte/__init__.py
--rw-r--r--   0        0        0     2434 2023-05-12 08:29:33.663742 cli-lite-0.7.0/clilte/builtin.py
--rw-r--r--   0        0        0     8028 2023-05-12 08:19:17.334983 cli-lite-0.7.0/clilte/core.py
--rw-r--r--   0        0        0     1092 2022-07-03 16:27:16.504000 cli-lite-0.7.0/LICENSE
--rw-r--r--   0        0        0     1213 2023-05-12 08:39:24.337139 cli-lite-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1069 2023-05-12 08:39:24.351103 cli-lite-0.7.0/README.md
--rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 cli-lite-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      160 2023-05-12 07:56:09.908946 cli-lite-0.7.1/clilte/__init__.py
+-rw-r--r--   0        0        0     2434 2023-05-12 08:29:33.663742 cli-lite-0.7.1/clilte/builtin.py
+-rw-r--r--   0        0        0     8082 2023-05-12 11:14:44.638054 cli-lite-0.7.1/clilte/core.py
+-rw-r--r--   0        0        0     1092 2022-07-03 16:27:16.504000 cli-lite-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1213 2023-05-12 11:14:58.969068 cli-lite-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1069 2023-05-12 08:39:24.351103 cli-lite-0.7.1/README.md
+-rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 cli-lite-0.7.1/PKG-INFO
```

### Comparing `cli-lite-0.7.0/clilte/builtin.py` & `cli-lite-0.7.1/clilte/builtin.py`

 * *Files identical despite different names*

### Comparing `cli-lite-0.7.0/clilte/core.py` & `cli-lite-0.7.1/clilte/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,22 @@
 )
 from arclet.alconna.exceptions import SpecialOptionTriggered
 from arclet.alconna.tools import ShellTextFormatter, RichConsoleFormatter
 
 cli_instance: ContextVar[CommandLine] = ContextVar("litecli")
 
 
+def handle_argv():
+    path = Path(sys.argv[0])
+    head = path.stem
+    if head == "__main__":
+        head = path.parent.stem
+    return head
+
+
 @dataclass
 class PluginMetadata:
     name: str
     version: str
     description: str = field(default="Unknown")
     tags: list[str] = field(default_factory=list)
     author: list[str] = field(default_factory=list)
@@ -207,16 +215,15 @@
     def main(self, *args: str):
         if self.load_preset:
             self.preset()
         self.load_entry()
         if args:
             res = self._command.parse(list(args))  # type: ignore
         else:
-            path = Path(sys.argv[0])
-            head = path.parent.stem if str(path.parent) not in (".", "/", "\\") else path.stem
+            head = handle_argv()
             if head != self._command.command:
                 res = self._command.parse(sys.argv[1:])  # type: ignore
             else:
                 res = self._command.parse([head, *sys.argv[1:]])  # type: ignore
         if not res.matched:
             if isinstance(res.error_info, SpecialOptionTriggered):
                 return
```

### Comparing `cli-lite-0.7.0/LICENSE` & `cli-lite-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-lite-0.7.0/pyproject.toml` & `cli-lite-0.7.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "cli-lite"
-version = "0.7.0"
+version = "0.7.1"
 description = "A simple framework to build a cli tool, base on Alconna"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
-    "arclet-alconna<2.0.0, >=1.7.1",
+    "arclet-alconna<2.0.0, >=1.7.2",
     "arclet-alconna-tools>=0.6.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "commandline",
     "cli-tool",
```

### Comparing `cli-lite-0.7.0/README.md` & `cli-lite-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cli-lite-0.7.0/PKG-INFO` & `cli-lite-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-lite
-Version: 0.7.0
+Version: 0.7.1
 Summary: A simple framework to build a cli tool, base on Alconna
 License: MIT
 Keywords: commandline,cli-tool,plugin,cli,litecli
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

