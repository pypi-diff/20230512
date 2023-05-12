# Comparing `tmp/aiida-shell-0.5.1.tar.gz` & `tmp/aiida-shell-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-shell-0.5.1.tar", last modified: Wed May  3 22:10:15 2023, max compression
+gzip compressed data, was "aiida-shell-0.5.2.tar", last modified: Fri May 12 20:07:03 2023, max compression
```

## Comparing `aiida-shell-0.5.1.tar` & `aiida-shell-0.5.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      184 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/.readthedocs.yml
--rw-r--r--   0        0        0    11029 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0      448 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/CITATION.cff
--rw-r--r--   0        0        0     1076 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0      728 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/README.md
--rw-r--r--   0        0        0      638 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/Makefile
--rw-r--r--   0        0        0     1323 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/conf.py
--rw-r--r--   0        0        0    15543 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/howto.rst
--rw-r--r--   0        0        0    25440 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/images/logo-column.png
--rw-r--r--   0        0        0   164551 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/images/logo-column.svg
--rw-r--r--   0        0        0   167883 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/images/logo-text.svg
--rw-r--r--   0        0        0      429 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/index.rst
--rw-r--r--   0        0        0      590 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/installation.rst
--rw-r--r--   0        0        0     3191 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      239 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/src/aiida_shell/__init__.py
--rw-r--r--   0        0        0      127 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/src/aiida_shell/calculations/__init__.py
--rw-r--r--   0        0        0    13771 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/calculations/shell.py
--rw-r--r--   0        0        0      167 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/data/__init__.py
--rw-r--r--   0        0        0     1624 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/data/code.py
--rw-r--r--   0        0        0     5518 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/data/pickled.py
--rw-r--r--   0        0        0      141 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/engine/__init__.py
--rw-r--r--   0        0        0      151 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/engine/launchers/__init__.py
--rw-r--r--   0        0        0     8797 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/engine/launchers/shell_job.py
--rw-r--r--   0        0        0      128 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/parsers/__init__.py
--rw-r--r--   0        0        0     5572 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/parsers/shell.py
--rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 aiida-shell-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      230 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/.readthedocs.yml
+-rw-r--r--   0        0        0    12194 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0      448 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/CITATION.cff
+-rw-r--r--   0        0        0     1076 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/LICENSE.txt
+-rw-r--r--   0        0        0      728 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/README.md
+-rw-r--r--   0        0        0      638 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/docs/Makefile
+-rw-r--r--   0        0        0     1323 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/docs/source/conf.py
+-rw-r--r--   0        0        0    16290 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/docs/source/howto.rst
+-rw-r--r--   0        0        0    25440 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/docs/source/images/logo-column.png
+-rw-r--r--   0        0        0   164551 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/docs/source/images/logo-column.svg
+-rw-r--r--   0        0        0   167883 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/docs/source/images/logo-text.svg
+-rw-r--r--   0        0        0      429 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/docs/source/index.rst
+-rw-r--r--   0        0        0      590 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/docs/source/installation.rst
+-rw-r--r--   0        0        0     3191 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      239 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/calculations/__init__.py
+-rw-r--r--   0        0        0    14339 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/calculations/shell.py
+-rw-r--r--   0        0        0      167 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/data/__init__.py
+-rw-r--r--   0        0        0     1624 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/data/code.py
+-rw-r--r--   0        0        0     5518 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/data/pickled.py
+-rw-r--r--   0        0        0      141 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/engine/__init__.py
+-rw-r--r--   0        0        0      151 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/engine/launchers/__init__.py
+-rw-r--r--   0        0        0     8797 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/engine/launchers/shell_job.py
+-rw-r--r--   0        0        0      128 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/parsers/__init__.py
+-rw-r--r--   0        0        0     5572 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/parsers/shell.py
+-rw-r--r--   0        0        0       26 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/py.typed
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 aiida-shell-0.5.2/PKG-INFO
```

### Comparing `aiida-shell-0.5.1/CHANGELOG.md` & `aiida-shell-0.5.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,35 @@
 # Change log
 
+## `v0.5.2` - 2023-05-12
+
+### Features
+- `ShellJob`: Add the optional `redirect_stderr` input [[92f726b]](https://github.com/sphuber/aiida-shell/commit/92f726b5fcd631dc4aaa85505869e2dabca9b77c)
+
+    A common practice when running shell commands is to redirect the content, written to the stderr file descriptor, to stdout.
+    This is normally accomplished as follows:
+
+        date > stdout 2>&1
+
+    This behaviour can now be reproduced by setting the ``metadata.options.redirect_stderr`` input to ``True``:
+
+        from aiida_shell import launch_shell_job
+        results, node = launch_shell_job(
+            'date',
+            metadata={'options': {'redirect_stderr': True}}
+        )
+
+### Fixes
+- `ShellJob`: Add `invalidates_cache=True` to exit codes < `400` [[4d405e1]](https://github.com/sphuber/aiida-shell/commit/4d405e168aa46a8e1d878e2e4040cc128cc651fa)
+
+### Devops
+- Add the `py.typed` file following PEP 561 [[680a0e9]](https://github.com/sphuber/aiida-shell/commit/680a0e9e4a8888c6967ce7c3b531da551f210401)
+- Update Python version on RTD to 3.11 [[2cfd4a2]](https://github.com/sphuber/aiida-shell/commit/2cfd4a243cf4db45800e5e84f78acec08fa9844d)
+
+
 ## `v0.5.1` - 2023-05-04
 
 ### Fixes
 - `ShellJob`: Remove `tot_num_mpiprocs` from `resources` default [[5e61c89]](https://github.com/sphuber/aiida-shell/commit/5e61c891958f705eaf56d8b590227011f16706ef)
 - `launch_shell_job`: Only `which` command if code doesn't already exist [[c1c31ab]](https://github.com/sphuber/aiida-shell/commit/c1c31ab404abcad4778accc8c01c3afbb818dfc8)
```

### Comparing `aiida-shell-0.5.1/LICENSE.txt` & `aiida-shell-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/README.md` & `aiida-shell-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/docs/Makefile` & `aiida-shell-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/docs/source/conf.py` & `aiida-shell-0.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/docs/source/howto.rst` & `aiida-shell-0.5.2/docs/source/howto.rst`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,41 @@
 
 which prints ``string a``.
 
 N.B.: one might be tempted to simply define the ``arguments`` as ``'< {input}'``, but this won't work as the ``<`` symbol will be quoted and will be read as a literal command line argument, not as the redirection symbol.
 This is why passing the ``<`` in the ``arguments`` input will result in a validation error.
 
 
+Redirecting stderr to the stdout file
+=====================================
+
+A common practice when running shell commands is to redirect the content, written to the stderr file descriptor, to stdout.
+This is normally accomplished as follows:
+
+.. code-block:: bash
+
+    date > stdout 2>&1
+
+To reproduce this behaviour, set the ``metadata.option.redirect_stderr`` input to ``True``:
+
+.. code-block:: python
+
+    from aiida_shell import launch_shell_job
+    results, node = launch_shell_job(
+        'date',
+        metadata={'options': {'redirect_stderr': True}}
+    )
+
+If the option is not specified, or set to ``False``, the stderr will be redirected to the file named ``stderr``, as follows:
+
+.. code-block:: bash
+
+    date > stdout 2> stderr
+
+
 Defining outputs
 ================
 
 When the shell command is executed, AiiDA captures by default the content written to the stdout and stderr file descriptors.
 The content is wrapped in a ``SinglefileData`` node and attached to the ``ShellJob`` with the ``stdout`` and ``stderr`` link labels, respectively.
 Any other output files that need to be captured can be defined using the ``outputs`` keyword argument.
```

### Comparing `aiida-shell-0.5.1/docs/source/images/logo-column.png` & `aiida-shell-0.5.2/docs/source/images/logo-column.png`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/docs/source/images/logo-column.svg` & `aiida-shell-0.5.2/docs/source/images/logo-column.svg`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/docs/source/images/logo-text.svg` & `aiida-shell-0.5.2/docs/source/images/logo-text.svg`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/docs/source/installation.rst` & `aiida-shell-0.5.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/pyproject.toml` & `aiida-shell-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/src/aiida_shell/calculations/shell.py` & `aiida-shell-0.5.2/src/aiida_shell/calculations/shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,54 +37,69 @@
             'arguments', valid_type=List, required=False, serializer=to_aiida_type, validator=cls.validate_arguments
         )
         spec.input('outputs', valid_type=List, required=False, serializer=to_aiida_type, validator=cls.validate_outputs)
         spec.input(
             'parser', valid_type=PickledData, required=False, serializer=PickledData, validator=cls.validate_parser
         )
         spec.input(
+            'metadata.options.redirect_stderr',
+            valid_type=bool,
+            required=False,
+            help='If set to ``True``, the stderr file descriptor is redirected to stdout.'
+        )
+        spec.input(
             'metadata.options.filename_stdin',
             valid_type=str,
             required=False,
             help='Filename that should be redirected to the shell command using the stdin file descriptor.'
         )
-        spec.inputs['code'].required = True
         spec.input(
             'metadata.options.additional_retrieve',
             required=False,
             valid_type=list,
             help='List of filepaths that are to be retrieved in addition to defaults and those specified in the '
             '`outputs` input. This is useful if files need to be retrieved for a custom `parser`.'
         )
+        spec.inputs['code'].required = True
 
         options = spec.inputs['metadata']['options']  # type: ignore[index]
         options['parser_name'].default = 'core.shell'  # type: ignore[index]
         options['resources'].default = {'num_machines': 1}  # type: ignore[index]
 
         spec.outputs.dynamic = True
 
         spec.exit_code(
             300,
             'ERROR_OUTPUT_STATUS_MISSING',
-            message='Exit status could not be determined: exit status file was not retrieved.'
+            message='Exit status could not be determined: exit status file was not retrieved.',
+            invalidates_cache=True,
         )
         spec.exit_code(
             301,
             'ERROR_OUTPUT_STATUS_INVALID',
-            message='Exit status could not be determined: exit status file does not contain a valid integer.'
+            message='Exit status could not be determined: exit status file does not contain a valid integer.',
+            invalidates_cache=True,
+        )
+        spec.exit_code(
+            302,
+            'ERROR_OUTPUT_STDOUT_MISSING',
+            message='The stdout file was not retrieved.',
+            invalidates_cache=True,
         )
-        spec.exit_code(302, 'ERROR_OUTPUT_STDOUT_MISSING', message='The stdout file was not retrieved.')
         spec.exit_code(
             303,
             'ERROR_OUTPUT_FILEPATHS_MISSING',
-            message='One or more output files defined in the `outputs` input were not retrieved: {missing_filepaths}.'
+            message='One or more output files defined in the `outputs` input were not retrieved: {missing_filepaths}.',
+            invalidates_cache=True,
         )
         spec.exit_code(
             310,
             'ERROR_PARSER_HOOK_EXCEPTED',
-            message='Callable specified in the `parser` input excepted: {exception}.'
+            message='Callable specified in the `parser` input excepted: {exception}.',
+            invalidates_cache=True,
         )
         spec.exit_code(
             400, 'ERROR_COMMAND_FAILED', message='The command exited with a non-zero status: {status} {stderr}.'
         )
         spec.exit_code(
             410,
             'ERROR_STDERR_NOT_EMPTY',
@@ -199,17 +214,21 @@
         if filename_stdin and filename_stdin in processed_arguments:
             processed_arguments.remove(filename_stdin)
 
         code_info = CodeInfo()
         code_info.code_uuid = inputs['code'].uuid
         code_info.cmdline_params = processed_arguments
         code_info.stdin_name = filename_stdin
-        code_info.stderr_name = self.FILENAME_STDERR
         code_info.stdout_name = self.node.get_option('output_filename') or self.FILENAME_STDOUT
 
+        if self.node.get_option('redirect_stderr'):
+            code_info.join_files = True
+        else:
+            code_info.stderr_name = self.FILENAME_STDERR
+
         calc_info = CalcInfo()
         calc_info.codes_info = [code_info]
         calc_info.append_text = f'echo $? > {self.FILENAME_STATUS}'
         calc_info.retrieve_temporary_list = retrieve_list
 
         return calc_info
```

### Comparing `aiida-shell-0.5.1/src/aiida_shell/data/code.py` & `aiida-shell-0.5.2/src/aiida_shell/data/code.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/src/aiida_shell/data/pickled.py` & `aiida-shell-0.5.2/src/aiida_shell/data/pickled.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/src/aiida_shell/engine/launchers/shell_job.py` & `aiida-shell-0.5.2/src/aiida_shell/engine/launchers/shell_job.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/src/aiida_shell/parsers/shell.py` & `aiida-shell-0.5.2/src/aiida_shell/parsers/shell.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.1/PKG-INFO` & `aiida-shell-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-shell
-Version: 0.5.1
+Version: 0.5.2
 Summary: AiiDA plugin that makes running shell commands easy.
 Keywords: aiida,workflows
 Author-email: "Sebastiaan P. Huber" <mail@sphuber.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AiiDA
```

