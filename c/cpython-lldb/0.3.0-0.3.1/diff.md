# Comparing `tmp/cpython-lldb-0.3.0.tar.gz` & `tmp/cpython_lldb-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpython-lldb-0.3.0.tar", max compression
+gzip compressed data, was "cpython_lldb-0.3.1.tar", max compression
```

## Comparing `cpython-lldb-0.3.0.tar` & `cpython_lldb-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1082 2021-10-06 07:37:41.454389 cpython-lldb-0.3.0/LICENSE
--rw-r--r--   0        0        0     9314 2021-10-06 07:37:41.454389 cpython-lldb-0.3.0/README.md
--rw-r--r--   0        0        0    36814 2021-10-06 07:37:41.458389 cpython-lldb-0.3.0/cpython_lldb.py
--rw-r--r--   0        0        0      783 2021-10-06 07:37:51.862566 cpython-lldb-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    10359 2021-10-06 07:37:52.862965 cpython-lldb-0.3.0/setup.py
--rw-r--r--   0        0        0    10292 2021-10-06 07:37:52.863938 cpython-lldb-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-12 21:31:27.597205 cpython_lldb-0.3.1/LICENSE
+-rw-r--r--   0        0        0     8973 2023-05-12 21:31:27.597205 cpython_lldb-0.3.1/README.md
+-rw-r--r--   0        0        0    36903 2023-05-12 21:31:27.597205 cpython_lldb-0.3.1/cpython_lldb.py
+-rw-r--r--   0        0        0      802 2023-05-12 21:31:41.266453 cpython_lldb-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     9920 1970-01-01 00:00:00.000000 cpython_lldb-0.3.1/PKG-INFO
```

### Comparing `cpython-lldb-0.3.0/LICENSE` & `cpython_lldb-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cpython-lldb-0.3.0/README.md` & `cpython_lldb-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 Overview
 ========
 
+![build status](https://github.com/malor/cpython-lldb/actions/workflows/tests.yml/badge.svg)
+
 `cpython_lldb` is an LLDB extension for debugging Python programs.
 
 It may be useful for troubleshooting stuck threads and crashes in the interpreter,
 or external libraries. Unlike most Python debuggers, LLDB allows you to attach to
 a running process w/o instrumenting it in advance, or load a coredump and do a
 post-mortem analysis of a problem.
 
@@ -57,14 +59,36 @@
 ```shell
 $ mkdir -p ~/.lldb/cpython_lldb
 $ python -m pip install --target ~/.lldb/cpython_lldb cpython-lldb
 $ echo "command script import ~/.lldb/cpython_lldb/cpython_lldb.py" >> ~/.lldbinit
 $ chmod +x ~/.lldbinit
 ```
 
+MacOS
+-----
+LLDB bundled with MacOS is linked with the system version of CPython which may not even
+be in your PATH. To locate the right version of the interpreter, use:
+```shell
+$ lldb --print-script-interpreter-info
+```
+The output of the command above is a JSON with the following structure:
+```
+{
+  "executable":"/Library/.../Python3.framework/Versions/3.9/bin/python3",
+  "language":"python",
+  "lldb-pythonpath":"/Library/.../LLDB.framework/Resources/Python",
+  "prefix":"/Library/.../Python3.framework/Versions/3.9"
+}
+```
+Where the value for "executable" is the CPython version that should be used to install
+cpython_lldb for LLDB to be able to successfully import the script:
+```shell
+$(lldb --print-script-interpreter-info | jq -r .executable) -m pip install cpython_lldb
+```
+
 Usage
 =====
 
 Start a new LLDB session:
 
 ```shell
 $ lldb /usr/bin/python
@@ -271,44 +295,14 @@
 >>> import io
 >>> Segmentation fault
 ```
 
 It's recommended that you use the latest LLDB release from the official [APT repo](https://apt.llvm.org/) instead
 of the one shipped with your distro.
 
-Conflicting Python versions on Mac OS
--------------------------------------
-
-If you see an error like this:
-
-```
-Traceback (most recent call last):
-  File "<input>", line 1, in <module>
-  File "/usr/local/Cellar/python/2.7.13/Frameworks/Python.framework/Versions/2.7/lib/python2.7/io.py", line 51, in <module>
-    import _io
-ImportError: dlopen(/usr/local/Cellar/python/2.7.13/Frameworks/Python.framework/Versions/2.7/lib/python2.7/lib-dynload/_io.so, 2): Symbol not found: __PyCodecInfo_GetIncrementalDecoder
-  Referenced from: /usr/local/Cellar/python/2.7.13/Frameworks/Python.framework/Versions/2.7/lib/python2.7/lib-dynload/_io.so
-  Expected in: flat namespace
- in /usr/local/Cellar/python/2.7.13/Frameworks/Python.framework/Versions/2.7/lib/python2.7/lib-dynload/_io.so
-```
-
-then the version of LLDB, that is shipped with Mac OS and linked against the system CPython,
-is trying to use CPython installed via Homebrew. This won't work. You need to make sure LLDB
-picks up the correct CPython version on start. One way to achieve that would be modifying
-`$PATH`, e.g. by creating a wrapper for `lldb`:
-
-```
-#!/bin/sh
-
-export PATH=/usr/bin:$PATH
-exec lldb "$@"
-```
-
-and putting it to `/usr/local/bin`.
-
 See this [page](https://github.com/vadimcn/vscode-lldb/wiki/Troubleshooting) for advice on
 troubleshooting of LLDB.
 
 Development
 ===========
 
 Running tests
@@ -325,16 +319,14 @@
 To run the tests against a specific CPython (or LLDB) version, do:
 
 ```
 $ PY_VERSION=X.Y LLDB_VERSION=Z make test
 ```
 
 Supported CPython versions are:
-* `3.5`
-* `3.6`
 * `3.7`
 * `3.8`
 * `3.9`
 * `3.10`
 
 Supported LLDB versions:
 * `7`
```

### Comparing `cpython-lldb-0.3.0/cpython_lldb.py` & `cpython_lldb-0.3.1/cpython_lldb.py`

 * *Files 0% similar despite different names*

```diff
@@ -751,15 +751,19 @@
         return self.__doc__
 
     def __call__(self, debugger, command, exe_ctx, result):
         try:
             args = self.argument_parser.parse_args(shlex.split(command))
             self.execute(debugger, args, result)
         except Exception as e:
-            result.SetError(u'Failed to execute command `{}`: {}'.format(self.command, e))
+            msg = u'Failed to execute command `{}`: {}'.format(self.command, e)
+            if six.PY2:
+                msg = msg.encode('utf-8')
+
+            result.SetError(msg)
 
     @property
     def argument_parser(self):
         """ArgumentParser instance used for this command.
 
         The default parser does not have any arguments and only prints a help
         message based on the command description.
```

### Comparing `cpython-lldb-0.3.0/pyproject.toml` & `cpython_lldb-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "cpython-lldb"
-version = "0.3.0"
+version = "0.3.1"
 description = "LLDB script for debugging of CPython processes"
 license = "MIT"
 
 authors = [
     "Roman Podoliaka <roman.podoliaka@gmail.com>",
 ]
 
 readme = "README.md"
 repository = "https://github.com/malor/cpython-lldb"
 homepage = "https://github.com/malor/cpython-lldb"
 
 keywords = ["debugging", "lldb", "cpython"]
 
 [tool.poetry.dependencies]
-python = "~2.7 || ^3.5"
+python = "~2.7 || ^3.7"
 six = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
+pexpect = "^4.8.0"
 # we want to specify the depedency on pytest here as well, but that confuses poetry, so we rely
 # on pytest-xdist to depend on pytest transitively instead
 pytest-xdist = [
     {version = "^1.34.0", python = "<3.6"},
-    {version = "^2.3.0",  python = "^3.6"},
+    {version = "^3.1.0",  python = "^3.7"},
 ]
 test_extension = { path = "tests/test_extension/" }
```

### Comparing `cpython-lldb-0.3.0/setup.py` & `cpython_lldb-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,367 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cpython-lldb
+Version: 0.3.1
+Summary: LLDB script for debugging of CPython processes
+Home-page: https://github.com/malor/cpython-lldb
+License: MIT
+Keywords: debugging,lldb,cpython
+Author: Roman Podoliaka
+Author-email: roman.podoliaka@gmail.com
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: six (>=1.0.0,<2.0.0)
+Project-URL: Repository, https://github.com/malor/cpython-lldb
+Description-Content-Type: text/markdown
 
-modules = \
-['cpython_lldb']
-install_requires = \
-['six>=1.0.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'cpython-lldb',
-    'version': '0.3.0',
-    'description': 'LLDB script for debugging of CPython processes',
-    'long_description': 'Overview\n========\n\n`cpython_lldb` is an LLDB extension for debugging Python programs.\n\nIt may be useful for troubleshooting stuck threads and crashes in the interpreter,\nor external libraries. Unlike most Python debuggers, LLDB allows you to attach to\na running process w/o instrumenting it in advance, or load a coredump and do a\npost-mortem analysis of a problem.\n\nWhen analyzing the state of a Python process, normally you would only have\naccess to the *intepreter-level* information: every variable would be of type\nPyObject\\*, and stack traces would only contain CPython internal calls and\ncalls to external libraries. Unless you are a CPython developer troubleshooting\nsome bug in the implementation of the interpreter, that is typically not\nvery useful. This extension, however, allows you to extract the *application-level*\ninformation about execution of a program: print the values of variables,\nlist the source code, display Python stack traces, etc.\n\nWhile CPython itself provides a similar extension for gdb [out of the box](\nhttps://github.com/python/cpython/blob/master/Tools/gdb/libpython.py),\none might still prefer to use LLDB as a debugger, e.g. on Mac OS.\n\n`cpython_lldb` requires CPython to be built with debugging symbols, which is\nnot the case for some Linux distros (most notably Arch Linux). CPython official\n[Docker images](https://hub.docker.com/_/python) are known to work correctly,\nas they are used for integration testing.\n\n\nFeatures\n========\n\n`cpython_lldb` targets CPython 3.5+ and supports the following features:\n\n* pretty-priting of built-in types (int, bool, float, bytes, str, none, tuple, list, set, frozenset, dict)\n* printing of Python-level stack traces\n* printing of local variables\n* listing the source code\n* walking up and down the Python call stack\n\nInstallation\n============\n\nIf your version of LLDB is linked against system libpython, it\'s recommended\nthat you install the extension to the user site packages directory and allow\nit to be loaded automatically on start of a new LLDB session:\n\n```shell\n$ python -m pip install --user cpython-lldb\n$ echo "command script import cpython_lldb" >> ~/.lldbinit\n$ chmod +x ~/.lldbinit\n```\n\nAlternatively, you can install the extension to some other location on disk\nand tell LLDB to load it from there, e.g. ~/.lldb:\n\n```shell\n$ mkdir -p ~/.lldb/cpython_lldb\n$ python -m pip install --target ~/.lldb/cpython_lldb cpython-lldb\n$ echo "command script import ~/.lldb/cpython_lldb/cpython_lldb.py" >> ~/.lldbinit\n$ chmod +x ~/.lldbinit\n```\n\nUsage\n=====\n\nStart a new LLDB session:\n\n```shell\n$ lldb /usr/bin/python\n```\n\nor attach to an existing CPython process:\n\n```shell\n$ lldb /usr/bin/python -p $PID\n```\n\nIf you\'ve followed the installation steps, the extension will now be automatically\nloaded on start of a new LLDB session and register some Python-specific commands:\n\n```\n(lldb) help\n...\nCurrent user-defined commands:\n  py-bt     -- Print a Python-level call trace of the selected thread.\n  py-down   -- Select a newer Python stack frame.\n  py-list   -- List the source code of the Python module that is currently being executed.\n  py-locals -- Print the values of local variables in the selected Python frame.\n  py-up     -- Select an older Python stack frame.\nFor more information on any command, type \'help <command-name>\'.\n```\n\nPretty-printing\n---------------\n\nAll known `PyObject`\'s (i.e. built-in types) are automatically pretty-printed\nwhen encountered, as if you tried to get a `repr()` of something in Python REPL,\ne.g.:\n\n```\n(lldb) frame variable v\n(PyObject *) v = 0x0000000100793c00 42\n(lldb) p v->ob_type->tp_name\n(const char *) $3 = 0x000000010017d42a "int"\n```\n\nStack traces\n------------\n\nUse `py-bt` to print a full application-level stack trace of the current thread, e.g.:\n\n```\n(lldb) py-bt\nTraceback (most recent call last):\n  File "test.py", line 15, in <module>\n    fc()\n  File "test.py", line 12, in fc\n    fb()\n  File "test.py", line 8, in fb\n    fa()\n  File "test.py", line 2, in fa\n    abs(1)\n```\n\nWalking up and down the call stack\n----------------------------------\n\nUse `py-up` and `py-down` to select an older or a newer Python call stack frame, e.g.:\n\n```\n(lldb) py-up\n  File "/Users/malor/src/cpython/test.py", line 6, in cb\n    self.ca()\n(lldb) py-up\n  File "/Users/malor/src/cpython/test.py", line 20, in f_static\n    c.cb()\n(lldb) py-down\n  File "/Users/malor/src/cpython/test.py", line 6, in cb\n    self.ca()\n(lldb) py-down\n  File "/Users/malor/src/cpython/test.py", line 3, in ca\n    abs(1)\n(lldb) py-down\n*** Newest frame\n```\n\nPrinting of local variables\n---------------------------\n\nUse `py-locals` to print the values of local variables in the selected frame:\n\n```\n(lldb) py-locals\na = 42\nargs = (1, 2, 3)\nb = [1, u\'hello\', u\'\\\\u0442\\\\u0435\\\\u0441\\\\u0442\']\nc = ([1], 2, [[3]])\nd = u\'test\'\ne = {u\'a\': -1, u\'b\': 0, u\'c\': 1}\neggs = 42\nkwargs = {u\'foo\': \'spam\'}\nspam = u\'foobar\'\n```\n\nListing the source code\n-----------------------\n\nUse `py-list` to list the source code that is currently being executed in the selected\nPython frame, e.g.:\n\n```\n(lldb) py-list\n    1    SOME_CONST = 42\n    2\n    3\n    4    def fa():\n   >5        abs(1)\n    6        return 1\n    7\n    8\n    9    def fb():\n   10        1 + 1\n```\n\nThe command also accepts optional `start` and `end` arguments that allow to\nlist the source code within a specific range of lines, e.g.:\n\n```\n(lldb) py-list 4\n    4    def fa():\n   >5        abs(1)\n    6        return 1\n    7\n    8\n    9    def fb():\n   10        1 + 1\n   11        fa()\n   12\n   13\n   14    def fc():\n```\n\nor:\n\n```\n(lldb) py-list 4 11\n    4    def fa():\n   >5        abs(1)\n    6        return 1\n    7\n    8\n    9    def fb():\n   10        1 + 1\n   11        fa()\n```\n\nPotential issues and how to solve them\n======================================\n\nCPython 2.7.x\n-------------\n\nCPython 2.7.x is not supported. There are currently no plans to support it in the future.\n\nMissing debugging symbols\n-------------------------\n\nCPython debugging symbols are required. You can check if they are available as follows:\n\n```shell\n$ lldb /usr/bin/python\n$ (lldb) type lookup PyObject\n```\n\nIf debugging symbols are not available, you\'ll see something like:\n\n```shell\nno type was found matching \'PyObject\'\n```\n\nSome Linux distros ship debugging symbols separately. To fix the problem on Debian / Ubuntu do:\n\n```shell\n$ sudo apt-get install python-dbg\n```\n\non CentOS / Fedora / RHEL do:\n\n```shell\n$ sudo yum install python-debuginfo\n```\n\nOther distros, like Arch Linux, do not provide debugging symbols in the package repos. In this case,\nyou would need to build CPython from source. Please refer to official [CPython](https://devguide.python.org/setup/#compiling)\nor [distro](https://wiki.archlinux.org/index.php/Debug_-_Getting_Traces) docs for instructions.\n\nAlternatively, you can use official CPython [Docker images](https://hub.docker.com/_/python).\n\n\nBroken LLDB scripting\n---------------------\n\nSome Linux distros (most notably Debian Stretch) are shipped with a version of LLDB in which Python scripting\ntriggers a segmentation fault when executing any non-trivial operation:\n\n```shell\n$ lldb\n(lldb) script\nPython Interactive Interpreter. To exit, type \'quit()\', \'exit()\' or Ctrl-D.\n>>> import io\n>>> Segmentation fault\n```\n\nIt\'s recommended that you use the latest LLDB release from the official [APT repo](https://apt.llvm.org/) instead\nof the one shipped with your distro.\n\nConflicting Python versions on Mac OS\n-------------------------------------\n\nIf you see an error like this:\n\n```\nTraceback (most recent call last):\n  File "<input>", line 1, in <module>\n  File "/usr/local/Cellar/python/2.7.13/Frameworks/Python.framework/Versions/2.7/lib/python2.7/io.py", line 51, in <module>\n    import _io\nImportError: dlopen(/usr/local/Cellar/python/2.7.13/Frameworks/Python.framework/Versions/2.7/lib/python2.7/lib-dynload/_io.so, 2): Symbol not found: __PyCodecInfo_GetIncrementalDecoder\n  Referenced from: /usr/local/Cellar/python/2.7.13/Frameworks/Python.framework/Versions/2.7/lib/python2.7/lib-dynload/_io.so\n  Expected in: flat namespace\n in /usr/local/Cellar/python/2.7.13/Frameworks/Python.framework/Versions/2.7/lib/python2.7/lib-dynload/_io.so\n```\n\nthen the version of LLDB, that is shipped with Mac OS and linked against the system CPython,\nis trying to use CPython installed via Homebrew. This won\'t work. You need to make sure LLDB\npicks up the correct CPython version on start. One way to achieve that would be modifying\n`$PATH`, e.g. by creating a wrapper for `lldb`:\n\n```\n#!/bin/sh\n\nexport PATH=/usr/bin:$PATH\nexec lldb "$@"\n```\n\nand putting it to `/usr/local/bin`.\n\nSee this [page](https://github.com/vadimcn/vscode-lldb/wiki/Troubleshooting) for advice on\ntroubleshooting of LLDB.\n\nDevelopment\n===========\n\nRunning tests\n-------------\n\nTests currently require `make` and `docker` to be installed.\n\nTo run the tests against the *latest* released CPython version, do:\n\n```\n$ make test\n```\n\nTo run the tests against a specific CPython (or LLDB) version, do:\n\n```\n$ PY_VERSION=X.Y LLDB_VERSION=Z make test\n```\n\nSupported CPython versions are:\n* `3.5`\n* `3.6`\n* `3.7`\n* `3.8`\n* `3.9`\n* `3.10`\n\nSupported LLDB versions:\n* `7`\n* `8`\n* `9`\n* `10`\n* `11`\n\nContributors\n============\n\nKudos to everyone who have contributed to this project!\n\n* Marco Neumann\n',
-    'author': 'Roman Podoliaka',
-    'author_email': 'roman.podoliaka@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/malor/cpython-lldb',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'python_requires': '>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*',
+Overview
+========
+
+![build status](https://github.com/malor/cpython-lldb/actions/workflows/tests.yml/badge.svg)
+
+`cpython_lldb` is an LLDB extension for debugging Python programs.
+
+It may be useful for troubleshooting stuck threads and crashes in the interpreter,
+or external libraries. Unlike most Python debuggers, LLDB allows you to attach to
+a running process w/o instrumenting it in advance, or load a coredump and do a
+post-mortem analysis of a problem.
+
+When analyzing the state of a Python process, normally you would only have
+access to the *intepreter-level* information: every variable would be of type
+PyObject\*, and stack traces would only contain CPython internal calls and
+calls to external libraries. Unless you are a CPython developer troubleshooting
+some bug in the implementation of the interpreter, that is typically not
+very useful. This extension, however, allows you to extract the *application-level*
+information about execution of a program: print the values of variables,
+list the source code, display Python stack traces, etc.
+
+While CPython itself provides a similar extension for gdb [out of the box](
+https://github.com/python/cpython/blob/master/Tools/gdb/libpython.py),
+one might still prefer to use LLDB as a debugger, e.g. on Mac OS.
+
+`cpython_lldb` requires CPython to be built with debugging symbols, which is
+not the case for some Linux distros (most notably Arch Linux). CPython official
+[Docker images](https://hub.docker.com/_/python) are known to work correctly,
+as they are used for integration testing.
+
+
+Features
+========
+
+`cpython_lldb` targets CPython 3.5+ and supports the following features:
+
+* pretty-priting of built-in types (int, bool, float, bytes, str, none, tuple, list, set, frozenset, dict)
+* printing of Python-level stack traces
+* printing of local variables
+* listing the source code
+* walking up and down the Python call stack
+
+Installation
+============
+
+If your version of LLDB is linked against system libpython, it's recommended
+that you install the extension to the user site packages directory and allow
+it to be loaded automatically on start of a new LLDB session:
+
+```shell
+$ python -m pip install --user cpython-lldb
+$ echo "command script import cpython_lldb" >> ~/.lldbinit
+$ chmod +x ~/.lldbinit
+```
+
+Alternatively, you can install the extension to some other location on disk
+and tell LLDB to load it from there, e.g. ~/.lldb:
+
+```shell
+$ mkdir -p ~/.lldb/cpython_lldb
+$ python -m pip install --target ~/.lldb/cpython_lldb cpython-lldb
+$ echo "command script import ~/.lldb/cpython_lldb/cpython_lldb.py" >> ~/.lldbinit
+$ chmod +x ~/.lldbinit
+```
+
+MacOS
+-----
+LLDB bundled with MacOS is linked with the system version of CPython which may not even
+be in your PATH. To locate the right version of the interpreter, use:
+```shell
+$ lldb --print-script-interpreter-info
+```
+The output of the command above is a JSON with the following structure:
+```
+{
+  "executable":"/Library/.../Python3.framework/Versions/3.9/bin/python3",
+  "language":"python",
+  "lldb-pythonpath":"/Library/.../LLDB.framework/Resources/Python",
+  "prefix":"/Library/.../Python3.framework/Versions/3.9"
 }
+```
+Where the value for "executable" is the CPython version that should be used to install
+cpython_lldb for LLDB to be able to successfully import the script:
+```shell
+$(lldb --print-script-interpreter-info | jq -r .executable) -m pip install cpython_lldb
+```
+
+Usage
+=====
+
+Start a new LLDB session:
+
+```shell
+$ lldb /usr/bin/python
+```
+
+or attach to an existing CPython process:
+
+```shell
+$ lldb /usr/bin/python -p $PID
+```
+
+If you've followed the installation steps, the extension will now be automatically
+loaded on start of a new LLDB session and register some Python-specific commands:
+
+```
+(lldb) help
+...
+Current user-defined commands:
+  py-bt     -- Print a Python-level call trace of the selected thread.
+  py-down   -- Select a newer Python stack frame.
+  py-list   -- List the source code of the Python module that is currently being executed.
+  py-locals -- Print the values of local variables in the selected Python frame.
+  py-up     -- Select an older Python stack frame.
+For more information on any command, type 'help <command-name>'.
+```
+
+Pretty-printing
+---------------
+
+All known `PyObject`'s (i.e. built-in types) are automatically pretty-printed
+when encountered, as if you tried to get a `repr()` of something in Python REPL,
+e.g.:
+
+```
+(lldb) frame variable v
+(PyObject *) v = 0x0000000100793c00 42
+(lldb) p v->ob_type->tp_name
+(const char *) $3 = 0x000000010017d42a "int"
+```
+
+Stack traces
+------------
+
+Use `py-bt` to print a full application-level stack trace of the current thread, e.g.:
+
+```
+(lldb) py-bt
+Traceback (most recent call last):
+  File "test.py", line 15, in <module>
+    fc()
+  File "test.py", line 12, in fc
+    fb()
+  File "test.py", line 8, in fb
+    fa()
+  File "test.py", line 2, in fa
+    abs(1)
+```
+
+Walking up and down the call stack
+----------------------------------
+
+Use `py-up` and `py-down` to select an older or a newer Python call stack frame, e.g.:
+
+```
+(lldb) py-up
+  File "/Users/malor/src/cpython/test.py", line 6, in cb
+    self.ca()
+(lldb) py-up
+  File "/Users/malor/src/cpython/test.py", line 20, in f_static
+    c.cb()
+(lldb) py-down
+  File "/Users/malor/src/cpython/test.py", line 6, in cb
+    self.ca()
+(lldb) py-down
+  File "/Users/malor/src/cpython/test.py", line 3, in ca
+    abs(1)
+(lldb) py-down
+*** Newest frame
+```
+
+Printing of local variables
+---------------------------
+
+Use `py-locals` to print the values of local variables in the selected frame:
+
+```
+(lldb) py-locals
+a = 42
+args = (1, 2, 3)
+b = [1, u'hello', u'\\u0442\\u0435\\u0441\\u0442']
+c = ([1], 2, [[3]])
+d = u'test'
+e = {u'a': -1, u'b': 0, u'c': 1}
+eggs = 42
+kwargs = {u'foo': 'spam'}
+spam = u'foobar'
+```
+
+Listing the source code
+-----------------------
+
+Use `py-list` to list the source code that is currently being executed in the selected
+Python frame, e.g.:
+
+```
+(lldb) py-list
+    1    SOME_CONST = 42
+    2
+    3
+    4    def fa():
+   >5        abs(1)
+    6        return 1
+    7
+    8
+    9    def fb():
+   10        1 + 1
+```
+
+The command also accepts optional `start` and `end` arguments that allow to
+list the source code within a specific range of lines, e.g.:
+
+```
+(lldb) py-list 4
+    4    def fa():
+   >5        abs(1)
+    6        return 1
+    7
+    8
+    9    def fb():
+   10        1 + 1
+   11        fa()
+   12
+   13
+   14    def fc():
+```
+
+or:
+
+```
+(lldb) py-list 4 11
+    4    def fa():
+   >5        abs(1)
+    6        return 1
+    7
+    8
+    9    def fb():
+   10        1 + 1
+   11        fa()
+```
+
+Potential issues and how to solve them
+======================================
+
+CPython 2.7.x
+-------------
+
+CPython 2.7.x is not supported. There are currently no plans to support it in the future.
+
+Missing debugging symbols
+-------------------------
+
+CPython debugging symbols are required. You can check if they are available as follows:
+
+```shell
+$ lldb /usr/bin/python
+$ (lldb) type lookup PyObject
+```
+
+If debugging symbols are not available, you'll see something like:
+
+```shell
+no type was found matching 'PyObject'
+```
+
+Some Linux distros ship debugging symbols separately. To fix the problem on Debian / Ubuntu do:
+
+```shell
+$ sudo apt-get install python-dbg
+```
+
+on CentOS / Fedora / RHEL do:
+
+```shell
+$ sudo yum install python-debuginfo
+```
+
+Other distros, like Arch Linux, do not provide debugging symbols in the package repos. In this case,
+you would need to build CPython from source. Please refer to official [CPython](https://devguide.python.org/setup/#compiling)
+or [distro](https://wiki.archlinux.org/index.php/Debug_-_Getting_Traces) docs for instructions.
+
+Alternatively, you can use official CPython [Docker images](https://hub.docker.com/_/python).
+
+
+Broken LLDB scripting
+---------------------
+
+Some Linux distros (most notably Debian Stretch) are shipped with a version of LLDB in which Python scripting
+triggers a segmentation fault when executing any non-trivial operation:
+
+```shell
+$ lldb
+(lldb) script
+Python Interactive Interpreter. To exit, type 'quit()', 'exit()' or Ctrl-D.
+>>> import io
+>>> Segmentation fault
+```
+
+It's recommended that you use the latest LLDB release from the official [APT repo](https://apt.llvm.org/) instead
+of the one shipped with your distro.
+
+See this [page](https://github.com/vadimcn/vscode-lldb/wiki/Troubleshooting) for advice on
+troubleshooting of LLDB.
+
+Development
+===========
+
+Running tests
+-------------
+
+Tests currently require `make` and `docker` to be installed.
+
+To run the tests against the *latest* released CPython version, do:
+
+```
+$ make test
+```
+
+To run the tests against a specific CPython (or LLDB) version, do:
+
+```
+$ PY_VERSION=X.Y LLDB_VERSION=Z make test
+```
+
+Supported CPython versions are:
+* `3.7`
+* `3.8`
+* `3.9`
+* `3.10`
+
+Supported LLDB versions:
+* `7`
+* `8`
+* `9`
+* `10`
+* `11`
+
+Contributors
+============
+
+Kudos to everyone who have contributed to this project!
 
+* Marco Neumann
 
-setup(**setup_kwargs)
```

