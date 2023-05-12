# Comparing `tmp/ansys-mechanical-core-0.7.3.tar.gz` & `tmp/ansys-mechanical-core-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-mechanical-core-0.7.3.tar", last modified: Thu Apr 20 12:11:26 2023, max compression
+gzip compressed data, was "ansys-mechanical-core-0.8.0.tar", last modified: Fri May 12 13:26:39 2023, max compression
```

## Comparing `ansys-mechanical-core-0.7.3.tar` & `ansys-mechanical-core-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1089 2023-04-20 12:11:06.263142 ansys-mechanical-core-0.7.3/LICENSE
--rw-r--r--   0        0        0     5456 2023-04-20 12:11:06.263142 ansys-mechanical-core-0.7.3/README.rst
--rw-r--r--   0        0        0     3922 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     1242 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/__init__.py
--rw-r--r--   0        0        0      536 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/_version.py
--rw-r--r--   0        0        0      167 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/__init__.py
--rw-r--r--   0        0        0     5088 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/app.py
--rw-r--r--   0        0        0     1392 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/config.py
--rw-r--r--   0        0        0      819 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/imports.py
--rw-r--r--   0        0        0     1344 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/initializer.py
--rw-r--r--   0        0        0     1958 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/loader.py
--rw-r--r--   0        0        0     2022 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/logging.py
--rw-r--r--   0        0        0      852 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/resolver.py
--rw-r--r--   0        0        0     1287 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/runtime.py
--rw-r--r--   0        0        0      703 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/shims.py
--rw-r--r--   0        0        0     3312 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/errors.py
--rw-r--r--   0        0        0      113 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/examples/__init__.py
--rw-r--r--   0        0        0     2992 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/examples/downloads.py
--rw-r--r--   0        0        0     5505 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/launcher.py
--rw-r--r--   0        0        0    23658 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/logging.py
--rw-r--r--   0        0        0    83310 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/mechanical.py
--rw-r--r--   0        0        0     4215 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/misc.py
--rw-r--r--   0        0        0    25079 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/pool.py
--rw-r--r--   0        0        0     8178 1970-01-01 00:00:00.000000 ansys-mechanical-core-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-12 13:26:24.233918 ansys-mechanical-core-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5456 2023-05-12 13:26:24.233918 ansys-mechanical-core-0.8.0/README.rst
+-rw-r--r--   0        0        0     3943 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1242 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/__init__.py
+-rw-r--r--   0        0        0      536 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/_version.py
+-rw-r--r--   0        0        0      167 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/__init__.py
+-rw-r--r--   0        0        0     5219 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/app.py
+-rw-r--r--   0        0        0     1392 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/config.py
+-rw-r--r--   0        0        0      819 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/imports.py
+-rw-r--r--   0        0        0     1825 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/initializer.py
+-rw-r--r--   0        0        0     1958 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/loader.py
+-rw-r--r--   0        0        0     2022 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/logging.py
+-rw-r--r--   0        0        0      852 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/resolver.py
+-rw-r--r--   0        0        0     1287 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/runtime.py
+-rw-r--r--   0        0        0      703 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/shims.py
+-rw-r--r--   0        0        0     3312 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/errors.py
+-rw-r--r--   0        0        0      113 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/examples/__init__.py
+-rw-r--r--   0        0        0     2992 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/examples/downloads.py
+-rw-r--r--   0        0        0     5505 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/launcher.py
+-rw-r--r--   0        0        0    23658 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/logging.py
+-rw-r--r--   0        0        0    87557 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/mechanical.py
+-rw-r--r--   0        0        0     4215 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/misc.py
+-rw-r--r--   0        0        0    25243 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/pool.py
+-rw-r--r--   0        0        0     8130 1970-01-01 00:00:00.000000 ansys-mechanical-core-0.8.0/PKG-INFO
```

### Comparing `ansys-mechanical-core-0.7.3/LICENSE` & `ansys-mechanical-core-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/README.rst` & `ansys-mechanical-core-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/pyproject.toml` & `ansys-mechanical-core-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-mechanical-core"
-version = "0.7.3"
+version = "0.8.0"
 description = "A python wrapper for Ansys Mechanical"
 readme = "README.rst"
 requires-python = ">=3.7,<4.0"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -17,15 +17,14 @@
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering :: Information Analysis',
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -44,38 +43,38 @@
 Documentation = "https://mechanical.docs.pyansys.com"
 Source = "https://github.com/pyansys/pymechanical"
 Homepage = "https://github.com/pyansys/pymechanical"
 Tracker = "https://github.com/pyansys/pymechanical/issues"
 
 [project.optional-dependencies]
 tests = [
-    "pytest==7.3.0",
+    "pytest==7.3.1",
     "pytest-cov==4.0.0",
     "pytest-print==0.3.1",
 ]
 doc = [
-    "Sphinx==5.3.0",
-    "ansys-sphinx-theme==0.9.7",
-    "grpcio==1.53.0",
+    "Sphinx==6.2.0", # BLOCKED BY sphinx-design - Cannot upgrade to Sphinx 7 for now
+    "ansys-sphinx-theme==0.9.8",
+    "grpcio==1.54.0",
     "imageio-ffmpeg==0.4.8",
-    "imageio==2.27.0",
+    "imageio==2.28.1",
     "jupyter_sphinx==0.4.0",
     "jupyterlab>=3.2.8",
     "matplotlib==3.7.1",
     "numpydoc==1.5.0",
     "plotly==5.14.1",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
     "pythreejs==2.4.2",
-    "pyvista==0.38.5",
+    "pyvista==0.39.0",
     "sphinx-autobuild==2021.3.14",
-    "sphinx-autodoc-typehints==1.22",
-    "sphinx-copybutton==0.5.1",
-    "sphinx_design==0.3.0",
-    "sphinx-gallery==0.12.2",
+    "sphinx-autodoc-typehints==1.23.0",
+    "sphinx-copybutton==0.5.2",
+    "sphinx_design==0.4.1",
+    "sphinx-gallery==0.13.0",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
     "sphinxemoji==0.2.0",
 ]
 
 [tool.flit.module]
 name = "ansys.mechanical.core"
```

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/__init__.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/_version.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/_version.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/app.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         """
         global INSTANCES
         from ansys.mechanical.core import BUILDING_GALLERY
 
         if BUILDING_GALLERY:
             if len(INSTANCES) != 0:
                 self._app = INSTANCES[0]
+                self._app.new()
                 self._version = self._app.version
                 self._disposed = True
                 return
         if len(INSTANCES) > 0:
             raise Exception("Cannot have more than one embedded mechanical instance")
         self._version = kwargs.get("version")
         if self._version == None:
@@ -121,14 +122,18 @@
         """Save the project as."""
         self.DataModel.Project.SaveAs(path)
 
     def new(self):
         """Clear to a new application."""
         self.DataModel.Project.New()
 
+    def close(self):
+        """Close the application."""
+        self.ExtAPI.Application.Close()
+
     def execute_script(self, script: str):
         """Execute the given script with the internal IronPython engine."""
         SCRIPT_SCOPE = "pymechanical-internal"
         if not hasattr(self, "script_engine"):
             import clr
 
             clr.AddReference("Ansys.Mechanical.Scripting")
```

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/config.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/config.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/imports.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/imports.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/initializer.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/initializer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Initializer for Mechanical embedding. Sets up paths and resolvers."""
+from importlib.metadata import distribution
 import os
 from pathlib import Path
 import sys
+import warnings
 
 from ansys.mechanical.core.embedding.loader import load_clr
 from ansys.mechanical.core.embedding.resolver import resolve
 
 INITIALIZED_VERSION = None
 
 
@@ -34,12 +36,24 @@
     INITIALIZED_VERSION = version
 
     __disable_sec()
 
     # need to add system path in order to import the assembly with the resolver
     __add_sys_path(version)
 
+    # Check if 'pythonnet' is installed... and if so, throw warning
+    try:
+        distribution("pythonnet")
+        warnings.warn(
+            "The pythonnet package was found in your environment "
+            "which interferes with the ansys-pythonnet package. "
+            "Some APIs may not work due to pythonnet being installed.",
+            stacklevel=2,
+        )
+    except ModuleNotFoundError:
+        pass
+
     # load the CLR with mono that is shipped with the unified ansys installer
     load_clr(os.environ[f"AWP_ROOT{version}"])
 
     # attach the resolver
     resolve(version)
```

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/loader.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/loader.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/logging.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/logging.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/resolver.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/resolver.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/runtime.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/runtime.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/shims.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/shims.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/errors.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/examples/downloads.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/launcher.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/logging.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/mechanical.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/mechanical.py`

 * *Files 3% similar despite different names*

```diff
@@ -723,15 +723,24 @@
     @property
     def log(self):
         """Log associated with the current Mechanical instance."""
         return self._log
 
     @property
     def version(self) -> str:
-        """Get the Mechanical version based on the instance."""
+        """Get the Mechanical version based on the instance.
+
+        Examples
+        --------
+        Get the version of the connected Mechanical instance.
+
+        >>> mechanical.version
+        '231'
+
+        """
         if self._version == None:
             try:
                 self._disable_logging = True
                 script = (
                     'clr.AddReference("Ans.Utilities")\n'
                     "import Ansys\n"
                     "config = Ansys.Utilities.ApplicationConfiguration.DefaultConfiguration\n"
@@ -1154,14 +1163,17 @@
         )
 
     def run_python_script(
         self, script_block: str, enable_logging=False, log_level="WARNING", progress_interval=2000
     ):
         """Run a Python script block inside Mechanical.
 
+        It returns the string value of the last executed statement. If the value cannot be
+        returned as a string, it will return an empty string.
+
         Parameters
         ----------
         script_block : str
             Script block (one or more lines) to run.
         enable_logging: bool, optional
             Whether to enable logging. The default is ``False``.
         log_level: str
@@ -1171,25 +1183,80 @@
             Frequency in milliseconds for getting log messages from the server.
             The default is ``2000``.
 
         Returns
         -------
         str
             Script result.
+
+        Examples
+        --------
+        Return a value from a simple calculation.
+
+        >>> mechanical.run_python_script('2+3')
+        '5'
+
+        Return a string value from Project object.
+
+        >>> mechanical.run_python_script('ExtAPI.DataModel.Project.ProductVersion')
+        '2023 R1'
+
+        Return an empty string, when you try to return the Project object.
+
+        >>> mechanical.run_python_script('ExtAPI.DataModel.Project')
+        ''
+
+        Return an empty string for assignments.
+
+        >>> mechanical.run_python_script('version = ExtAPI.DataModel.Project.ProductVersion')
+        ''
+
+        Return value from the last executed statement from a variable.
+
+        >>> script='''
+            addition = 2 + 3
+            multiplication = 3 * 4
+            multiplication
+            '''
+        >>> mechanical.run_python_script(script)
+        '12'
+
+        Return value from last executed statement from a function call.
+
+        >>> script='''
+            import math
+            math.pow(2,3)
+            '''
+        >>> mechanical.run_python_script(script)
+        '8'
+
+        Handle an error scenario.
+
+        >>> script = 'hello_world()'
+        >>> import grpc
+        >>> try:
+                mechanical.run_python_script(script)
+            except grpc.RpcError as error:
+                print(error.details())
+        name 'hello_world' is not defined
+
         """
         self.verify_valid_connection()
-        response = self.__call_run_python_script(
+        result_as_string = self.__call_run_python_script(
             script_block, enable_logging, log_level, progress_interval
         )
-        return response.script_result
+        return result_as_string
 
     def run_python_script_from_file(
         self, file_path, enable_logging=False, log_level="WARNING", progress_interval=2000
     ):
-        """Run a Python file inside Mechanical.
+        """Run the contents a python file inside Mechanical.
+
+        It returns the string value of the last executed statement. If the value cannot be
+        returned as a string, it will return an empty string.
 
         Parameters
         ----------
         file_path :
             Path for the Python file.
         enable_logging: bool, optional
             Whether to enable logging. The default is ``False``.
@@ -1200,14 +1267,37 @@
             Frequency in milliseconds for getting log messages from the server.
             The default is ``2000``.
 
         Returns
         -------
         str
             Script result.
+
+        Examples
+        --------
+        Return a value from a simple calculation.
+
+        Contents of **simple.py** file
+
+        2+3
+
+        >>> mechanical.run_python_script('simple.py')
+        '5'
+
+        Return a value from a simple function call.
+
+        Contents of  **test.py** file
+
+        import math
+
+        math.pow(2,3)
+
+        >>> mechanical.run_python_script('test.py')
+        '8'
+
         """
         self.verify_valid_connection()
         self.log_debug(f"run_python_script_from_file started")
         script_code = Mechanical.__readfile(file_path)
         self.log_debug(f"run_python_script_from_file started")
         return self.run_python_script(script_code, enable_logging, log_level, progress_interval)
 
@@ -1216,14 +1306,21 @@
 
         Parameters
         ----------
         force : bool, optional
             Whether to force Mechanical to exit. The default is ``False``, in which case
             only Mechanical in UI mode asks for confirmation. This parameter overrides
             any environment variables that may inhibit exiting Mechanical.
+
+        Examples
+        --------
+        Exit Mechanical.
+
+        >>> mechanical.Exit(force=True)
+
         """
         if not force:
             if not get_start_instance():
                 self.log_info("Ignoring exit due to PYMECHANICAL_START_INSTANCE=False")
                 return
 
             # or building the gallery
@@ -1384,27 +1481,38 @@
                 chunk = mechanical_pb2.Chunk(payload=piece, size=length)
                 yield mechanical_pb2.FileUploadRequest(
                     file_name=os.path.basename(file_name), file_location=file_location, chunk=chunk
                 )
 
     @property
     def project_directory(self):
-        """Get the project directory for the currently connected Mechanical instance."""
+        """Get the project directory for the currently connected Mechanical instance.
+
+        Examples
+        --------
+        Get the project directory of the connected Mechanical instance.
+
+        >>> mechanical.project_directory
+        '/tmp/ANSYS.username.1/AnsysMech3F97/Project_Mech_Files/'
+
+        """
         return self.run_python_script("ExtAPI.DataModel.Project.ProjectDirectory")
 
     def list_files(self):
         """List the files in the working directory of Mechanical.
 
         Returns
         -------
         list
             List of files in the working directory of Mechanical.
 
         Examples
         --------
+        List the files in the working directory.
+
         >>> files = mechanical.list_files()
         >>> for file in files: print(file)
         """
         result = self.run_python_script(
             "import pymechanical_helpers\npymechanical_helpers.GetAllProjectFiles(ExtAPI)"
         )
 
@@ -1479,63 +1587,72 @@
         target_dir=None,
         chunk_size=DEFAULT_CHUNK_SIZE,
         progress_bar=None,
         recursive=False,
     ):  # pragma: no cover
         """Download files from the working directory of the Mechanical instance.
 
+         It downloads them from the working directory to the target directory. It returns the list
+         of local file paths for the downloaded files.
+
         Parameters
         ----------
         files : str, list[str], tuple(str)
             One or more files on the Mechanical server to download. The files must be
             in the same directory as the Mechanical instance. You can use the
             :func:`Mechanical.list_files <ansys.mechanical.core.mechanical.list_files>`
             function to list current files. Alternatively, you can specify *glob expressions* to
             match file names. For example, you could use ``file*`` to match every file whose
             name starts with ``file``.
         target_dir: str
-            Default directory to copy the downloaded files to. The default is ``None``.
+            Default directory to copy the downloaded files to. The default is ``None`` and
+            current working directory will be used as target directory.
         chunk_size : int, optional
             Chunk size in bytes. The default is ``262144``. The value must be less than 4 MB.
         progress_bar : bool, optional
             Whether to show a progress bar using  ``tqdm``. The default is ``None``, in
             which case a progress bar is shown. A progress bar is helpful for viewing download
             progress.
         recursive : bool, optional
             Whether to use recursion when using a glob pattern search. The default is ``False``.
 
+        Returns
+        -------
+        List[str]
+            List of local file paths.
+
         Notes
         -----
         There are some considerations to keep in mind when using the ``download()`` method:
 
         * The glob pattern search does not search recursively in remote instances.
         * In a remote instance, it is not possible to list or download files in a
           location other than the Mechanical working directory.
         * If you are connected to a local instance and provide a file path, downloading files
           from a different folder is allowed but is not recommended.
 
         Examples
         --------
         Download a single file.
 
-        >>> mechanical.download('file.out')
+        >>> local_file_path_list = mechanical.download('file.out')
 
         Download all files starting with ``file``.
 
-        >>> mechanical.download('file*')
+        >>> local_file_path_list = mechanical.download('file*')
 
         Download every file in the Mechanical working directory.
 
-        >>> mechanical.download('*.*')
+        >>> local_file_path_list = mechanical.download('*.*')
 
         Alternatively, the recommended method is to use the
         :func:`download_project() <ansys.mechanical.core.mechanical.Mechanical.download_project>`
         method to download all files.
 
-        >>> mechanical.download_project()
+        >>> local_file_path_list = mechanical.download_project()
 
         """
         self.verify_valid_connection()
 
         if chunk_size > 4 * 1024 * 1024:  # 4MB
             raise ValueError(
                 f"Chunk sizes bigger than 4 MB can generate unstable behaviour in PyMechanical. "
@@ -1683,29 +1800,39 @@
             pbar.close()
 
         return file_size
 
     def download_project(self, extensions=None, target_dir=None, progress_bar=False):
         """Download all project files in the working directory of the Mechanical instance.
 
+        It downloads them from the working directory to the target directory. It returns the list
+        of local file paths for the downloaded files.
+
         Parameters
         ----------
         extensions : list[str], tuple[str], optional
             List of extensions for filtering files before downloading them. The
             default is ``None``.
         target_dir : str, optional
             Path for downloading the files to. The default is ``None``.
         progress_bar : bool, optional
             Whether to show a progress bar using ``tqdm``. The default is ``False``.
             A progress bar is helpful for viewing download progress.
 
         Returns
         -------
         List[str]
-            List of downloaded files.
+            List of local file paths.
+
+        Examples
+        --------
+        Download all the files in the project.
+
+        >>> local_file_path_list = mechanical.download_project()
+
         """
         destination_directory = target_dir.rstrip("\\/")
 
         # let us create the directory, if it doesn't exist
         if destination_directory:
             path = pathlib.Path(destination_directory)
             path.mkdir(parents=True, exist_ok=True)
@@ -1765,15 +1892,23 @@
                 files=file, target_dir=new_path_dir, progress_bar=progress_bar
             )
             list_of_files.extend(temp_files)
 
         return list_of_files
 
     def clear(self):
-        """Clear the database."""
+        """Clear the database.
+
+        Examples
+        --------
+        Clear the database.
+
+        >>> mechanical.clear()
+
+        """
         self.run_python_script("ExtAPI.DataModel.Project.New()")
 
     def _make_dummy_call(self):
         try:
             self._disable_logging = True
             self.run_python_script("ExtAPI.DataModel.Project.ProjectDirectory")
         except grpc.RpcError:  # pragma: no cover
@@ -1819,42 +1954,66 @@
         log_level_server = self.convert_to_server_log_level(log_level)
         request = mechanical_pb2.RunScriptRequest()
         request.script_code = script_code
         request.enable_logging = enable_logging
         request.logger_severity = log_level_server
         request.progress_interval = progress_interval
 
-        response = None
+        result = ""
         self._busy = True
 
         try:
             for runscript_response in self._stub.RunPythonScript(request):
                 if runscript_response.log_info == "__done__":
-                    response = runscript_response
+                    result = runscript_response.script_result
                     break
                 else:
                     if enable_logging:
                         self.log_message(log_level, runscript_response.log_info)
+        except grpc.RpcError as error:
+            error_info = error.details()
+            error_info_lower = error_info.lower()
+            # For the given script, return value cannot be converted to string.
+            if (
+                "the expected result" in error_info_lower
+                and "cannot be return via this API." in error_info
+            ):
+                if enable_logging:
+                    self.log_debug(f"Ignoring the conversion error.{error_info}")
+                result = ""
+            else:
+                raise
         finally:
             self._busy = False
 
         self._log_mechanical_script(script_code)
 
-        return response
+        return result
 
     def log_message(self, log_level, message):
         """Log the message using the given log level.
 
          Parameters
         ----------
         log_level: str
             Level of logging. Options are ``"DEBUG"``, ``"INFO"``, ``"WARNING"``,
             and ``"ERROR"``.
         message : str
             Message to log.
+
+        Examples
+        --------
+        Log a debug message.
+
+        >>> mechanical.log_message('DEBUG', 'debug message')
+
+        Log an info message.
+
+        >>> mechanical.log_message('INFO', 'info message')
+
         """
         if log_level == "DEBUG":
             self.log_debug(message)
         elif log_level == "INFO":
             self.log_info(message)
         elif log_level == "WARNING":
             self.log_warning(message)
```

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/misc.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/misc.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/pool.py` & `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -669,13 +669,22 @@
                             ).join()
                     except Exception as e:
                         LOG.error(e, exc_info=True)
             time.sleep(refresh)
 
     @property
     def ports(self):
-        """Get a list of the ports that are used."""
+        """Get a list of the ports that are used.
+
+        Examples
+        --------
+        Get the list of ports used by the pool of Mechanical instances.
+
+        >>> pool.ports
+        [10001, 10002]
+
+        """
         return [inst._port for inst in self if inst is not None]
 
     def __str__(self):
         """Get the string representation of this object."""
         return "Mechanical pool with %d active instances" % len(self)
```

### Comparing `ansys-mechanical-core-0.7.3/PKG-INFO` & `ansys-mechanical-core-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 Metadata-Version: 2.1
 Name: ansys-mechanical-core
-Version: 0.7.3
+Version: 0.8.0
 Summary: A python wrapper for Ansys Mechanical
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: ansys_api_mechanical==0.1.0
 Requires-Dist: ansys-pythonnet==3.1.0rc1
 Requires-Dist: importlib-metadata>=4.0
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: grpcio>=1.30.0
 Requires-Dist: protobuf>=3.12.2,<3.21.0
 Requires-Dist: ansys-platform-instancemanagement>=1.0.1
 Requires-Dist: tqdm>=4.45.0
-Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.9.7 ; extra == "doc"
-Requires-Dist: grpcio==1.53.0 ; extra == "doc"
+Requires-Dist: Sphinx==6.2.0 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.8 ; extra == "doc"
+Requires-Dist: grpcio==1.54.0 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
-Requires-Dist: imageio==2.27.0 ; extra == "doc"
+Requires-Dist: imageio==2.28.1 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.4.0 ; extra == "doc"
 Requires-Dist: jupyterlab>=3.2.8 ; extra == "doc"
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: plotly==5.14.1 ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
 Requires-Dist: pythreejs==2.4.2 ; extra == "doc"
-Requires-Dist: pyvista==0.38.5 ; extra == "doc"
+Requires-Dist: pyvista==0.39.0 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==1.22 ; extra == "doc"
-Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
-Requires-Dist: sphinx_design==0.3.0 ; extra == "doc"
-Requires-Dist: sphinx-gallery==0.12.2 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==1.23.0 ; extra == "doc"
+Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
+Requires-Dist: sphinx_design==0.4.1 ; extra == "doc"
+Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.2.0 ; extra == "doc"
-Requires-Dist: pytest==7.3.0 ; extra == "tests"
+Requires-Dist: pytest==7.3.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
 Requires-Dist: pytest-print==0.3.1 ; extra == "tests"
 Project-URL: Documentation, https://mechanical.docs.pyansys.com
 Project-URL: Homepage, https://github.com/pyansys/pymechanical
 Project-URL: Source, https://github.com/pyansys/pymechanical
 Project-URL: Tracker, https://github.com/pyansys/pymechanical/issues
 Provides-Extra: doc
```

