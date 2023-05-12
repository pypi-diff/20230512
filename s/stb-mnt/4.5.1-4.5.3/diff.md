# Comparing `tmp/stb_mnt-4.5.1.tar.gz` & `tmp/stb_mnt-4.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stb_mnt-4.5.1.tar", max compression
+gzip compressed data, was "stb_mnt-4.5.3.tar", max compression
```

## Comparing `stb_mnt-4.5.1.tar` & `stb_mnt-4.5.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2023-01-09 22:18:45.026759 stb_mnt-4.5.1/LICENSE
--rw-r--r--   0        0        0     4129 2023-02-18 16:39:59.028161 stb_mnt-4.5.1/README.md
--rw-r--r--   0        0        0     1329 2023-03-12 18:52:22.031659 stb_mnt-4.5.1/pyproject.toml
--rw-r--r--   0        0        0       69 2023-01-09 19:47:55.893082 stb_mnt-4.5.1/stb/__init__.py
--rw-r--r--   0        0        0     2702 2023-02-17 18:43:44.943340 stb_mnt-4.5.1/stb/__main__.py
--rw-r--r--   0        0        0       79 2023-01-09 22:02:40.485385 stb_mnt-4.5.1/stb/__version__.py
--rw-r--r--   0        0        0     7339 2023-03-12 18:54:33.634270 stb_mnt-4.5.1/stb/config.py
--rw-r--r--   0        0        0     5389 2023-01-24 13:50:32.276659 stb_mnt-4.5.1/stb/db.py
--rw-r--r--   0        0        0     3966 2023-02-21 18:34:18.607097 stb_mnt-4.5.1/stb/graph.py
--rw-r--r--   0        0        0        0 2022-09-25 11:30:34.799917 stb_mnt-4.5.1/stb/py.typed
--rw-r--r--   0        0        0      813 2023-02-23 20:17:01.377182 stb_mnt-4.5.1/stb/run.py
--rw-r--r--   0        0        0     6003 2023-02-23 20:17:57.890205 stb_mnt-4.5.1/stb/setup.py
--rwxr-xr-x   0        0        0     6365 2023-01-26 09:29:16.979999 stb_mnt-4.5.1/stb/update.py
--rw-r--r--   0        0        0     3183 2023-01-24 21:17:59.489998 stb_mnt-4.5.1/stb/use.py
--rw-r--r--   0        0        0        0 2023-01-24 13:47:27.999993 stb_mnt-4.5.1/stb/utils/__init__.py
--rw-r--r--   0        0        0     4852 2023-01-24 20:56:14.909999 stb_mnt-4.5.1/stb/utils/common.py
--rw-r--r--   0        0        0     2725 2023-01-24 20:22:14.616666 stb_mnt-4.5.1/stb/utils/dependency_parser.py
--rw-r--r--   0        0        0     5334 1970-01-01 00:00:00.000000 stb_mnt-4.5.1/setup.py
--rw-r--r--   0        0        0     5181 1970-01-01 00:00:00.000000 stb_mnt-4.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-01-09 22:18:45.026759 stb_mnt-4.5.3/LICENSE
+-rw-r--r--   0        0        0     4275 2023-05-12 12:46:48.810016 stb_mnt-4.5.3/README.md
+-rw-r--r--   0        0        0     1329 2023-05-12 13:25:40.840047 stb_mnt-4.5.3/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-01-09 19:47:55.893082 stb_mnt-4.5.3/stb/__init__.py
+-rw-r--r--   0        0        0     2702 2023-02-17 18:43:44.943340 stb_mnt-4.5.3/stb/__main__.py
+-rw-r--r--   0        0        0       79 2023-01-09 22:02:40.485385 stb_mnt-4.5.3/stb/__version__.py
+-rw-r--r--   0        0        0     7339 2023-03-12 18:54:33.634270 stb_mnt-4.5.3/stb/config.py
+-rw-r--r--   0        0        0     5389 2023-01-24 13:50:32.276659 stb_mnt-4.5.3/stb/db.py
+-rw-r--r--   0        0        0     3966 2023-02-21 18:34:18.607097 stb_mnt-4.5.3/stb/graph.py
+-rw-r--r--   0        0        0        0 2022-09-25 11:30:34.799917 stb_mnt-4.5.3/stb/py.typed
+-rw-r--r--   0        0        0      813 2023-02-23 20:17:01.377182 stb_mnt-4.5.3/stb/run.py
+-rw-r--r--   0        0        0     6005 2023-05-12 13:12:28.356703 stb_mnt-4.5.3/stb/setup.py
+-rwxr-xr-x   0        0        0     6365 2023-01-26 09:29:16.979999 stb_mnt-4.5.3/stb/update.py
+-rw-r--r--   0        0        0     3251 2023-05-12 13:11:06.760035 stb_mnt-4.5.3/stb/use.py
+-rw-r--r--   0        0        0        0 2023-01-24 13:47:27.999993 stb_mnt-4.5.3/stb/utils/__init__.py
+-rw-r--r--   0        0        0     4852 2023-01-24 20:56:14.909999 stb_mnt-4.5.3/stb/utils/common.py
+-rw-r--r--   0        0        0     2725 2023-01-24 20:22:14.616666 stb_mnt-4.5.3/stb/utils/dependency_parser.py
+-rw-r--r--   0        0        0     5485 1970-01-01 00:00:00.000000 stb_mnt-4.5.3/setup.py
+-rw-r--r--   0        0        0     5327 1970-01-01 00:00:00.000000 stb_mnt-4.5.3/PKG-INFO
```

### Comparing `stb_mnt-4.5.1/LICENSE` & `stb_mnt-4.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.1/README.md` & `stb_mnt-4.5.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # stb
 
 A universal tool for local microservice management
 
+## Requirements
+
+* [Poetry](https://python-poetry.org/) - Required for setup functionality 
+* [Pyenv](https://github.com/pyenv/pyenv) - Optional
+
 ## Installation
 
 ```bash
 pipx install stb-mnt
 ```
 
 ## Usage
```

### Comparing `stb_mnt-4.5.1/pyproject.toml` & `stb_mnt-4.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "stb-mnt"
 packages = [{ include = "stb" }]
-version = "4.5.1"
+version = "4.5.3"
 description = "A universal tool for local microservice management."
 readme = "README.md"
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
 ]
```

### Comparing `stb_mnt-4.5.1/stb/__main__.py` & `stb_mnt-4.5.3/stb/__main__.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.1/stb/config.py` & `stb_mnt-4.5.3/stb/config.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.1/stb/db.py` & `stb_mnt-4.5.3/stb/db.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.1/stb/graph.py` & `stb_mnt-4.5.3/stb/graph.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.1/stb/run.py` & `stb_mnt-4.5.3/stb/run.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.1/stb/setup.py` & `stb_mnt-4.5.3/stb/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 @CONFIG.requires("git_url")
 def setup_services(services: List[str], skip_existing: bool) -> None:
     if not "git_url" in CONFIG:
         raise typer.BadParameter("You must set the git_url in the config file before you can use this command")
     if not PYENV_INSTALLED:
         typer.echo("Failed to locate pyenv. Will use the system python version(s) instead", err=True)
     installable_pyenv_versions = [
-        clean_python_version(" \t~^*") for v in sh("pyenv install --list", capture=True).stdout.split("\n") if v.strip()
+        clean_python_version(v) for v in sh("pyenv install --list", capture=True).stdout.split("\n") if v.strip()
     ]
 
     repositories_to_clone = get_repositories_to_clone(services, skip_existing)
 
     for name, link in repositories_to_clone:
         setup_service(name, link, installable_pyenv_versions)
 
@@ -84,15 +84,15 @@
 
 
 def get_usable_pyenv_version(current: str, available: Sequence[str], install: bool = False) -> Optional[str]:
     for version in reversed(available):
         version = version.strip("* \t\n")
         if version.startswith(current):
             if install:
-                sh(f"pyenv install {version}")
+                sh_with_log(f"pyenv install {version}")
             return version
 
 
 def get_repositories_to_clone(repo_names: List[str], skip_existing: bool) -> List[Tuple[str, str]]:
     """Expands gitlab repo names to include all repos if the name is a group or a namespace"""
     expanded_repo_names = []
```

### Comparing `stb_mnt-4.5.1/stb/update.py` & `stb_mnt-4.5.3/stb/update.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.1/stb/use.py` & `stb_mnt-4.5.3/stb/use.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, List
 
 import tomli as toml
 import typer
 from pysh import sh, which
 
 from stb.config import CONFIG
+from stb.utils.common import sh_with_log
 
 from .utils.dependency_parser import parse_dependency_specification
 
 PYENV_INSTALLED = which("pyenv")
 
 
 def use_packages(requirements: List[str], editable: bool = False, fix: bool = False) -> None:
@@ -46,22 +47,22 @@
                     "You must set the pypi_source in the config file before you can use this command"
                 )
 
             extras_arg = f'[{",".join(extras)}]' if extras else ""
             version_based_requirements.append(f'"{spec.name}{extras_arg}@{version}"')
 
     if fix:
-        sh(f"poetry remove {' '.join(existing_requirements)}")
+        sh_with_log(f"poetry remove {' '.join(existing_requirements)}")
 
     for requirement in path_based_requirements:
-        sh(f"poetry add {requirement} {editable_arg}")
+        sh_with_log(f"poetry add {requirement} {editable_arg}")
 
     if version_based_requirements:
         formatted_version_based_requirements = " ".join(version_based_requirements)
-        sh(f"poetry add {formatted_version_based_requirements} --source={CONFIG['pypi_source']}")
+        sh_with_log(f"poetry add {formatted_version_based_requirements} --source={CONFIG['pypi_source']}")
 
 
 def extract_package_info_from_pyproject(package_name: str, dependencies: "dict[str, str | dict]") -> "dict[str, Any]":
     if package_name in dependencies:
         old_value = dependencies[package_name]
 
         # oatmeal = "3.8.3"
```

### Comparing `stb_mnt-4.5.1/stb/utils/common.py` & `stb_mnt-4.5.3/stb/utils/common.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.1/stb/utils/dependency_parser.py` & `stb_mnt-4.5.3/stb/utils/dependency_parser.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.1/setup.py` & `stb_mnt-4.5.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,17 @@
  'typing-extensions>=4.3.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['stb = stb:app']}
 
 setup_kwargs = {
     'name': 'stb-mnt',
-    'version': '4.5.1',
+    'version': '4.5.3',
     'description': 'A universal tool for local microservice management.',
-    'long_description': '# stb\n\nA universal tool for local microservice management\n\n## Installation\n\n```bash\npipx install stb-mnt\n```\n\n## Usage\n\n### Setup\n\n* To download and setup my_company/backend/service1 microservice as a subdirectory to the current working directory, use:\n\n```bash\nstb setup my_company/backend/service1\n```\n\n* To download and setup my_company/backend/service1 and my_company/backend/service2 as subdirectories to current working directory, use:\n\n```bash\nstb setup my_company/backend/service1 my_company/backend/service2\n```\n\n* To setup all backend services, use:\n\n```bash\nstb setup my_company/backend\n```\n\nNote that if you want to clone repositories, you must first set a `git_url` using `stb config set git_url` command\n\n### Update\n\n* To update .env file in accordance with .env.example in a microservice:\n\n```bash\nstb update env\n```\n\n* To synchronize service ports between all installed microservices (you can specify which ones will run locally with the `--local` option):\n\n```bash\nstb update ports\n```\n\n* To update poetry.lock file, install dependencies, stash current changes, checkout to master, pull from remote, and recreate databases:\n\n```bash\nstb update package -piucd\n```\n\nor  \n\n```bash\nstb update package --pull --update --checkout --reset-databases\n```\n\n### DB\n\n* To upgrade migrations in a microservice:\n\n```bash\nstb db upgrade\n```\n\n* To create databases and upgrade its migrations in a microservice:\n\n```bash\nstb db create\n```\n\n* To drop databases in a microservice:\n\n```bash\nstb db drop\n```\n\n* To drop and recreate databases, and upgrade migrations in a microservice:\n\n```bash\nstb db reset\n```\n\n* To upgrade migrations in parallel for faster upgrades (useful for large monoliths with multiple databases), you can use the -p (--parallel) option:\n\n```bash\nstb db create -p\n```\n  \n```bash\nstb db reset -p\n```\n  \n* To force dropping of databases in case another program is using them at the same time, you can use the -f (--force) option:\n\n```bash\nstb db drop -f\n```\n  \n```bash\nstb db reset -f\n```\n  \n### Use\n\n`stb use` allows you to take a company private package and install either a cloud version or a local version of it. STB will preserve all extras, automatically set package source, and will gracefully handle any issues that might happen while updating.\n\n* To install a local version of `my_package` that is located at `../my_package`:\n\n```bash\nstb use ../my_package\n```\n\n* To install a local version of `my_package` that is located at `../my_package` in editable mode:\n\n```bash\nstb use ../my_package --editable\n```\n\n* To install a cloud version of `my_package` with tag `8.3.1`:\n\n```bash\nstb use "my_package==8.3.1"\n```\n\n* To install a cloud version of my_package with tag `8.3.1`, my_other_package with any tag higher than `1.2.3`, and my_third_package with any tag more than or equal to `4.5.6` and less than `5.0.0`:\n\n```bash\nstb use "my_package==8.3.1" "my_other_package>1.2.3" "my_third_package^4.5.6"\n```\n\n### Run\n\n* To update and run the select services concurrently:\n\n```bash\nstb run service1 service2\n```\n\n### Config\n\n* To set a git url for cloning:\n\n```bash\nstb config set git_url git@gitlab.my_company.com\n```\n\n### Graph\n\n* To get a dependency graph of your microservices:\n\n```bash\nstb graph json my_company/backend/ my_company/infrastructure/\n```\n\n* To get a dependency graph of your microservices as an svg image (requires graphviz):\n\n```bash\nstb graph graphviz my_company/backend/ my_company/infrastructure/\n```\n\n### How directories are selected for update/db\n\nFor every update, you can specify:\n\n1) A microservice directory, which will cause stb to update only that microservice\n2) Several microservice directories, which will cause stb to update these microservices and integrate them together (for example, `update ports` assigns ports to local microservices and updates their links in other microservices to match the assigned ports)\n3) A directory with multiple microservice subdirectories inside it, which is equivalent to (2) with the list of subdirectories as arguments\n4) Nothing, which will choose the current working directory as the first argument and will be equivalent to (1) or (3)\n',
+    'long_description': '# stb\n\nA universal tool for local microservice management\n\n## Requirements\n\n* [Poetry](https://python-poetry.org/) - Required for setup functionality \n* [Pyenv](https://github.com/pyenv/pyenv) - Optional\n\n## Installation\n\n```bash\npipx install stb-mnt\n```\n\n## Usage\n\n### Setup\n\n* To download and setup my_company/backend/service1 microservice as a subdirectory to the current working directory, use:\n\n```bash\nstb setup my_company/backend/service1\n```\n\n* To download and setup my_company/backend/service1 and my_company/backend/service2 as subdirectories to current working directory, use:\n\n```bash\nstb setup my_company/backend/service1 my_company/backend/service2\n```\n\n* To setup all backend services, use:\n\n```bash\nstb setup my_company/backend\n```\n\nNote that if you want to clone repositories, you must first set a `git_url` using `stb config set git_url` command\n\n### Update\n\n* To update .env file in accordance with .env.example in a microservice:\n\n```bash\nstb update env\n```\n\n* To synchronize service ports between all installed microservices (you can specify which ones will run locally with the `--local` option):\n\n```bash\nstb update ports\n```\n\n* To update poetry.lock file, install dependencies, stash current changes, checkout to master, pull from remote, and recreate databases:\n\n```bash\nstb update package -piucd\n```\n\nor  \n\n```bash\nstb update package --pull --update --checkout --reset-databases\n```\n\n### DB\n\n* To upgrade migrations in a microservice:\n\n```bash\nstb db upgrade\n```\n\n* To create databases and upgrade its migrations in a microservice:\n\n```bash\nstb db create\n```\n\n* To drop databases in a microservice:\n\n```bash\nstb db drop\n```\n\n* To drop and recreate databases, and upgrade migrations in a microservice:\n\n```bash\nstb db reset\n```\n\n* To upgrade migrations in parallel for faster upgrades (useful for large monoliths with multiple databases), you can use the -p (--parallel) option:\n\n```bash\nstb db create -p\n```\n  \n```bash\nstb db reset -p\n```\n  \n* To force dropping of databases in case another program is using them at the same time, you can use the -f (--force) option:\n\n```bash\nstb db drop -f\n```\n  \n```bash\nstb db reset -f\n```\n  \n### Use\n\n`stb use` allows you to take a company private package and install either a cloud version or a local version of it. STB will preserve all extras, automatically set package source, and will gracefully handle any issues that might happen while updating.\n\n* To install a local version of `my_package` that is located at `../my_package`:\n\n```bash\nstb use ../my_package\n```\n\n* To install a local version of `my_package` that is located at `../my_package` in editable mode:\n\n```bash\nstb use ../my_package --editable\n```\n\n* To install a cloud version of `my_package` with tag `8.3.1`:\n\n```bash\nstb use "my_package==8.3.1"\n```\n\n* To install a cloud version of my_package with tag `8.3.1`, my_other_package with any tag higher than `1.2.3`, and my_third_package with any tag more than or equal to `4.5.6` and less than `5.0.0`:\n\n```bash\nstb use "my_package==8.3.1" "my_other_package>1.2.3" "my_third_package^4.5.6"\n```\n\n### Run\n\n* To update and run the select services concurrently:\n\n```bash\nstb run service1 service2\n```\n\n### Config\n\n* To set a git url for cloning:\n\n```bash\nstb config set git_url git@gitlab.my_company.com\n```\n\n### Graph\n\n* To get a dependency graph of your microservices:\n\n```bash\nstb graph json my_company/backend/ my_company/infrastructure/\n```\n\n* To get a dependency graph of your microservices as an svg image (requires graphviz):\n\n```bash\nstb graph graphviz my_company/backend/ my_company/infrastructure/\n```\n\n### How directories are selected for update/db\n\nFor every update, you can specify:\n\n1) A microservice directory, which will cause stb to update only that microservice\n2) Several microservice directories, which will cause stb to update these microservices and integrate them together (for example, `update ports` assigns ports to local microservices and updates their links in other microservices to match the assigned ports)\n3) A directory with multiple microservice subdirectories inside it, which is equivalent to (2) with the list of subdirectories as arguments\n4) Nothing, which will choose the current working directory as the first argument and will be equivalent to (1) or (3)\n',
     'author': 'Stanislav Zmiev',
     'author_email': 'szmiev2000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `stb_mnt-4.5.1/PKG-INFO` & `stb_mnt-4.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stb-mnt
-Version: 4.5.1
+Version: 4.5.3
 Summary: A universal tool for local microservice management.
 Author: Stanislav Zmiev
 Author-email: szmiev2000@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
@@ -25,14 +25,19 @@
 Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # stb
 
 A universal tool for local microservice management
 
+## Requirements
+
+* [Poetry](https://python-poetry.org/) - Required for setup functionality 
+* [Pyenv](https://github.com/pyenv/pyenv) - Optional
+
 ## Installation
 
 ```bash
 pipx install stb-mnt
 ```
 
 ## Usage
```

