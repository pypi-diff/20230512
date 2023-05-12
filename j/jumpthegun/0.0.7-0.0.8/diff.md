# Comparing `tmp/jumpthegun-0.0.7.tar.gz` & `tmp/jumpthegun-0.0.8.tar.gz`

## Comparing `jumpthegun-0.0.7.tar` & `jumpthegun-0.0.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/.flake8
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/test_requirements.txt
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/tox.ini
--rwxr-xr-x   0        0        0     5461 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun.sh
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/__version__.py
--rw-r--r--   0        0        0    13304 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/jumpthegunctl.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/output_redirect.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/testutils.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/tools.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/__init__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/LICENSE
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/README.md
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/VERSION
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/__init__.py
--rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/_api.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/_error.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/_soft.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/_unix.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/_util.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/_windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/tests/test_jumpthegun.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/tests/test_tools.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/tests/testproj/.flake8
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/tests/testproj/bad.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/tests/testproj/good.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/tests/testproj/pyproject.toml
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/LICENSE
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/README.md
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 jumpthegun-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/.flake8
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/test_requirements.txt
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/tox.ini
+-rwxr-xr-x   0        0        0     5725 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun.sh
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/__version__.py
+-rw-r--r--   0        0        0    13304 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/jumpthegunctl.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/output_redirect.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/testutils.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/tools.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/__init__.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/LICENSE
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/README.md
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/VERSION
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/__init__.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/_api.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/_error.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/_soft.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/_unix.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/_util.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/_windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/tests/test_jumpthegun.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/tests/test_tools.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/tests/testproj/.flake8
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/tests/testproj/bad.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/tests/testproj/good.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/tests/testproj/pyproject.toml
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/README.md
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 jumpthegun-0.0.8/PKG-INFO
```

### Comparing `jumpthegun-0.0.7/tox.ini` & `jumpthegun-0.0.8/tox.ini`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/src/jumpthegun.sh` & `jumpthegun-0.0.8/src/jumpthegun.sh`

 * *Files 7% similar despite different names*

```diff
@@ -49,16 +49,17 @@
 -h|--help)
   usage && exit 0 ;;
 start|stop|restart|version|--version)
   [[ "$2" =~ -h|--help ]] && usage && exit 0
   tool_name="$2"
 
   # Find the tool's Python executable and check if it has JumpTheGun installed.
-  tool_path="$(command -v -- "$tool_name")"
-  shebang="$(head -n 1 -- "$tool_path")"
+  tool_path="$(command -v -- "$tool_name" 2>/dev/null)" || err_exit "Command not found: $tool_name"
+  shebang="$(head -n 1 -- "$tool_path" 2>/dev/null)"
+  [[ "${shebang:0:2}" == "#!" ]] || err_exit "No shebang (#!) found in script: $tool_path"
   if ! python_executable="$(${shebang#\#!} -c 'import sys; print(sys.executable); import jumpthegun' 2>/dev/null)"; then
     # Find JumpTheGun's code.
     SCRIPT_DIR=$( cd -- "$( dirname -- "${BASH_SOURCE[0]}" )" &> /dev/null && pwd )
     jumpthegunctl_path="$SCRIPT_DIR/jumpthegunctl"
     jumpthegunctl_shebang="$(head -n 1 -- "$jumpthegunctl_path")"
     jumpthegunctl_python_executable="$(${jumpthegunctl_shebang#\#!} -c 'import sys; print(sys.executable)')"
     jumpthegun_lib_dir="$("$jumpthegunctl_python_executable" -c 'import jumpthegun, os; print(os.path.dirname(jumpthegun.__file__))')"
@@ -78,15 +79,16 @@
       export PYTHONPATH="$cache_dir:$PYTHONPATH"
     else
       export PYTHONPATH="$cache_dir"
     fi
   fi
 
   # Run JumpTheGun.
-  exec "$python_executable" -c "from jumpthegun.jumpthegunctl import main; main()" "$@"
+  set -f  # Disable filename expansion (globbing).
+  exec $python_executable -c "from jumpthegun.jumpthegunctl import main; main()" "$@"
   ;;
 run)
   shift
   [[ $# -eq 0 ]] && usage && exit 1
   if [[ "$1" == "--no-autorun" ]]; then
     autorun=0
     shift
@@ -137,32 +139,32 @@
 function forward_signal() {
   kill -s "$1" "$pid"
 }
 for sig in INT TERM USR1 USR2; do
   trap "forward_signal $sig" "$sig"
 done
 
-# Send strings with bytes len prepended.
-function send_with_bytes_len_prefix() {
-  to_send_str="$*"
-  to_send_bytes_len="$(echo -n "$to_send_str" | wc -c | cut -f1)"
-  printf '%d\n%s' "$to_send_bytes_len" "$to_send_str" >&3
-}
-
-
-# Send cmdline arguments.
-send_with_bytes_len_prefix "$@"
-
-# Send cwd.
-send_with_bytes_len_prefix "$PWD"
+# Send argv and cwd.
+oLang="${LANG-}" oLcAll="${LC_ALL-}"
+LANG=C LC_ALL=C
+# Add an x in front to avoid special-casing having zero arguments.
+argv_str=$(printf ' %q' x "$@")
+# Remove the leading " x ".
+argv_str="${argv_str:3}"
+printf '%d\n%s%d\n%s' "${#argv_str}" "$argv_str" "${#PWD}" "$PWD" >&3
+LANG="$oLang" LC_ALL="$oLcAll"
 
 # Send env vars.
 x="$(mktemp)"
 env -0 > "$x" 2>/dev/null
-du -b "$x" | cut -f 1 >&3
+if [[ $OSTYPE == "darwin"* ]]; then
+  stat -f %z "$x" >&3
+else
+  stat -c %s "$x" >&3
+fi
 cat "$x" >&3
 rm "$x"
 
 
 # Read stdout and stderr from connection, line by line, and echo them.
 IFS=
 while read -r -u 3 line; do
```

### Comparing `jumpthegun-0.0.7/src/jumpthegun/jumpthegunctl.py` & `jumpthegun-0.0.8/src/jumpthegun/jumpthegunctl.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/src/jumpthegun/output_redirect.py` & `jumpthegun-0.0.8/src/jumpthegun/output_redirect.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/src/jumpthegun/tools.py` & `jumpthegun-0.0.8/src/jumpthegun/tools.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/src/jumpthegun/utils.py` & `jumpthegun-0.0.8/src/jumpthegun/utils.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/LICENSE` & `jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/README.md` & `jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/README.md`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/__init__.py` & `jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/__init__.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/_api.py` & `jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/_api.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/_soft.py` & `jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/_soft.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/_unix.py` & `jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/_unix.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/_util.py` & `jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/_util.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/src/jumpthegun/_vendor/filelock/_windows.py` & `jumpthegun-0.0.8/src/jumpthegun/_vendor/filelock/_windows.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/tests/test_jumpthegun.py` & `jumpthegun-0.0.8/tests/test_jumpthegun.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/.gitignore` & `jumpthegun-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/LICENSE` & `jumpthegun-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/README.md` & `jumpthegun-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/pyproject.toml` & `jumpthegun-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.7/PKG-INFO` & `jumpthegun-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jumpthegun
-Version: 0.0.7
+Version: 0.0.8
 Summary: Make Python CLI tools win the speed race, by cheating!
 Project-URL: Homepage, https://github.com/taleinat/jumpthegun
 Author-email: Tal Einat <taleinat@gmail.com>
 License: Apache-2.0
 License-File: LICENSE
 Keywords: cli
 Classifier: Development Status :: 1 - Planning
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jumpthegun Version: 0.0.7 Summary: Make Python CLI
+Metadata-Version: 2.1 Name: jumpthegun Version: 0.0.8 Summary: Make Python CLI
 tools win the speed race, by cheating! Project-URL: Homepage, https://
 github.com/taleinat/jumpthegun Author-email: Tal Einat
 gmail.com> License: Apache-2.0 License-File: LICENSE Keywords: cli Classifier:
 Development Status :: 1 - Planning Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
```

