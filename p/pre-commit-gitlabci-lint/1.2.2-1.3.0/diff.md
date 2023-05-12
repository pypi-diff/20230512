# Comparing `tmp/pre-commit-gitlabci-lint-1.2.2.tar.gz` & `tmp/pre-commit-gitlabci-lint-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre-commit-gitlabci-lint-1.2.2.tar", last modified: Mon Feb 27 02:57:19 2023, max compression
+gzip compressed data, was "pre-commit-gitlabci-lint-1.3.0.tar", last modified: Fri May 12 16:31:36 2023, max compression
```

## Comparing `pre-commit-gitlabci-lint-1.2.2.tar` & `pre-commit-gitlabci-lint-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-27 02:57:19.163551 pre-commit-gitlabci-lint-1.2.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-02-27 02:57:18.000000 pre-commit-gitlabci-lint-1.2.2/.mypy.ini
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1089 2023-02-27 02:57:18.000000 pre-commit-gitlabci-lint-1.2.2/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2023-02-27 02:57:18.000000 pre-commit-gitlabci-lint-1.2.2/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3482 2023-02-27 02:57:19.163551 pre-commit-gitlabci-lint-1.2.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2883 2023-02-27 02:57:18.000000 pre-commit-gitlabci-lint-1.2.2/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2023-02-27 02:57:19.163551 pre-commit-gitlabci-lint-1.2.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1562 2023-02-27 02:57:18.000000 pre-commit-gitlabci-lint-1.2.2/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-27 02:57:19.163551 pre-commit-gitlabci-lint-1.2.2/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-27 02:57:19.163551 pre-commit-gitlabci-lint-1.2.2/src/gitlabci_lint/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-27 02:57:18.000000 pre-commit-gitlabci-lint-1.2.2/src/gitlabci_lint/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8066 2023-02-27 02:57:18.000000 pre-commit-gitlabci-lint-1.2.2/src/gitlabci_lint/validate.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-27 02:57:19.163551 pre-commit-gitlabci-lint-1.2.2/src/pre_commit_gitlabci_lint.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3482 2023-02-27 02:57:19.000000 pre-commit-gitlabci-lint-1.2.2/src/pre_commit_gitlabci_lint.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      381 2023-02-27 02:57:19.000000 pre-commit-gitlabci-lint-1.2.2/src/pre_commit_gitlabci_lint.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-02-27 02:57:19.000000 pre-commit-gitlabci-lint-1.2.2/src/pre_commit_gitlabci_lint.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2023-02-27 02:57:19.000000 pre-commit-gitlabci-lint-1.2.2/src/pre_commit_gitlabci_lint.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2023-02-27 02:57:19.000000 pre-commit-gitlabci-lint-1.2.2/src/pre_commit_gitlabci_lint.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 16:31:35.994535 pre-commit-gitlabci-lint-1.3.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/.mypy.ini
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1089 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3053 2023-05-12 16:31:35.994535 pre-commit-gitlabci-lint-1.3.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2453 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2023-05-12 16:31:35.994535 pre-commit-gitlabci-lint-1.3.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1582 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 16:31:35.994535 pre-commit-gitlabci-lint-1.3.0/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 16:31:35.994535 pre-commit-gitlabci-lint-1.3.0/src/gitlabci_lint/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/src/gitlabci_lint/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8263 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/src/gitlabci_lint/validate.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 16:31:35.994535 pre-commit-gitlabci-lint-1.3.0/src/pre_commit_gitlabci_lint.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3053 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/src/pre_commit_gitlabci_lint.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/src/pre_commit_gitlabci_lint.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/src/pre_commit_gitlabci_lint.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/src/pre_commit_gitlabci_lint.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/src/pre_commit_gitlabci_lint.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2023-05-12 16:31:35.000000 pre-commit-gitlabci-lint-1.3.0/src/pre_commit_gitlabci_lint.egg-info/top_level.txt
```

### Comparing `pre-commit-gitlabci-lint-1.2.2/LICENSE` & `pre-commit-gitlabci-lint-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pre-commit-gitlabci-lint-1.2.2/PKG-INFO` & `pre-commit-gitlabci-lint-1.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,65 @@
-Metadata-Version: 2.1
-Name: pre-commit-gitlabci-lint
-Version: 1.2.2
-Summary: Validate your GitLab CI with GitLab's API endpoint.
-Home-page: https://github.com/bjd2385/pre-commit-gitlabci-lint
-Author: Emma Doyle
-Author-email: bjd2385.linux@gmail.com
-Project-URL: Bug Reports, https://github.com/bjd2385/pre-commit-gitlabci-lint/issues
-Project-URL: Source, https://github.com/bjd2385/pre-commit-gitlabci-lint
-Keywords: pre-commit,GitLab,CI,continuous integration
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # GitLab CI lint pre-commit hook
 
-This is a [pre-commit](https://pre-commit.com/) hook that uses GitLab's `/api/v4/ci/lint` linting endpoint to validate the contents of `.gitlab-ci.yml` files. This is similar to how CircleCI pre-commit hooks validate that product's required configs: by uploading your config to their API.
+This is a [pre-commit](https://pre-commit.com/) hook that uses GitLab's `/api/v4/ci/lint` linting endpoint to validate the contents of `.gitlab-ci.yml` files. This is similar to CircleCI pre-commit hooks that validate that product's configuration files.
 
 ```text
 $ gitlabci-lint --help
-usage: gitlabci-lint [-h] [-c CONFIGS] [-C GITLABCI_LINT_CONFIG] [-B [BASE_URL]] [--version] [-q]
+usage: gitlabci-lint [-h] [-c CONFIGS] [-C GITLABCI_LINT_CONFIG] [-b [BASE_URL]] [--version] [-q]
 
 Validate your GitLab CI with GitLab's API endpoint.
 
 options:
   -h, --help            show this help message and exit
   -c CONFIGS, --configs CONFIGS
                         CI Config files to check. (default: .gitlab-ci.yml)
   -C GITLABCI_LINT_CONFIG, --gitlabci-lint-config GITLABCI_LINT_CONFIG
                         Pass parameters via config file. Looks first at '.gitlabci-lint.toml', then '$HOME/.config/gitlabci-lint/config.toml', unless otherwise specified.
-  -B [BASE_URL], --base-url [BASE_URL]
+  -b [BASE_URL], -B [BASE_URL], --base-url [BASE_URL]
                         Base GitLab URL. (default: https://gitlab.com/)
+  -p PROJECT_ID, -P PROJECT_ID, --project-id PROJECT_ID
+                        Project ID to use with the lint API.
   --version             show program's version number and exit
   -q, -Q, --quiet       Silently fail and pass, without output, unless improperly configured. (default: False)
 ```
 
-By default, this tool sends your configuration to [https://gitlab.com](https://gitlab.com), though this can be overridden (see below for an example or the help text above).
-
 ## Install
 
 ```shell
 pip install pre-commit-gitlabci-lint
 ```
 
 ## Usage
 
-### Requirements
-
-GitLab Lint API now [requires authorization](https://gitlab.com/gitlab-org/gitlab/-/issues/321290).
+### Setup
 
 1. [Create an access token](https://gitlab.com/-/profile/personal_access_tokens) with `api` scope.
-2. Set access token value as a `GITLAB_TOKEN` or `GITLABCI_LINT_TOKEN` environment variable.
-3. Ensure Python version available is 3.8 or later.
-
-> **Warning:** GitLab tokens should not be shared. If leaked they can cause significant harm. Never store tokens in a repoitory.
+2. Set access token value in an environment variable named `GITLAB_TOKEN` or `GITLABCI_LINT_TOKEN`.
+3. Add the projectId for your gitlab project as a command line argument, or set it in the config file.
+4. Ensure the virtualenv Python version is 3.8 or later.
 
 ### Example
 
 An example `.pre-commit-config.yaml`:
 
 ```yaml
 ---
 repos:
   - repo: https://github.com/bjd2385/pre-commit-gitlabci-lint
     rev: <latest release>
     hooks:
       - id: gitlabci-lint
-      # args: [-b, 'https://custom.gitlab.host.com']
+      # args: [-b, 'https://custom.gitlab.host.com', '-p', '12345678']
 ```
 
-### Configuration files
+### Use configuration files
 
 No configuration file is required for use. However, if you'd rather specify settings in your repo, you may create a config file located at `/root/of/repo/.gitlabci-lint.toml`, or `$HOME/.config/.gitlabci-lint/config.toml`, such as the following.
 
 ```toml
 [gitlabci-lint]
 quiet = false
 base-url = "https://gitlab.com"
+project-id = "12345678"
 configs = [ ".gitlab-ci.yml" ]
 token = "$GITLAB_TOKEN"
-```
-
-## Development
-
-Install dependencies by running `./scripts/dependencies.sh`. Or, if you already have `yarn` in your path, `yarn install:deps`.
-
-### Releases
-
-Update `setup.py/version`-string and tag this repo's master branch with the same version string (prefixed by '`v`.)
+```
```

### Comparing `pre-commit-gitlabci-lint-1.2.2/README.md` & `pre-commit-gitlabci-lint-1.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,80 @@
+Metadata-Version: 2.1
+Name: pre-commit-gitlabci-lint
+Version: 1.3.0
+Summary: Validate your GitLab CI with GitLab's API endpoint.
+Home-page: https://github.com/bjd2385/pre-commit-gitlabci-lint
+Author: Emma Doyle
+Author-email: bjd2385.linux@gmail.com
+Project-URL: Bug Reports, https://github.com/bjd2385/pre-commit-gitlabci-lint/issues
+Project-URL: Source, https://github.com/bjd2385/pre-commit-gitlabci-lint
+Keywords: pre-commit,GitLab,CI,continuous integration
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # GitLab CI lint pre-commit hook
 
-This is a [pre-commit](https://pre-commit.com/) hook that uses GitLab's `/api/v4/ci/lint` linting endpoint to validate the contents of `.gitlab-ci.yml` files. This is similar to how CircleCI pre-commit hooks validate that product's required configs: by uploading your config to their API.
+This is a [pre-commit](https://pre-commit.com/) hook that uses GitLab's `/api/v4/ci/lint` linting endpoint to validate the contents of `.gitlab-ci.yml` files. This is similar to CircleCI pre-commit hooks that validate that product's configuration files.
 
 ```text
 $ gitlabci-lint --help
-usage: gitlabci-lint [-h] [-c CONFIGS] [-C GITLABCI_LINT_CONFIG] [-B [BASE_URL]] [--version] [-q]
+usage: gitlabci-lint [-h] [-c CONFIGS] [-C GITLABCI_LINT_CONFIG] [-b [BASE_URL]] [--version] [-q]
 
 Validate your GitLab CI with GitLab's API endpoint.
 
 options:
   -h, --help            show this help message and exit
   -c CONFIGS, --configs CONFIGS
                         CI Config files to check. (default: .gitlab-ci.yml)
   -C GITLABCI_LINT_CONFIG, --gitlabci-lint-config GITLABCI_LINT_CONFIG
                         Pass parameters via config file. Looks first at '.gitlabci-lint.toml', then '$HOME/.config/gitlabci-lint/config.toml', unless otherwise specified.
-  -B [BASE_URL], --base-url [BASE_URL]
+  -b [BASE_URL], -B [BASE_URL], --base-url [BASE_URL]
                         Base GitLab URL. (default: https://gitlab.com/)
+  -p PROJECT_ID, -P PROJECT_ID, --project-id PROJECT_ID
+                        Project ID to use with the lint API.
   --version             show program's version number and exit
   -q, -Q, --quiet       Silently fail and pass, without output, unless improperly configured. (default: False)
 ```
 
-By default, this tool sends your configuration to [https://gitlab.com](https://gitlab.com), though this can be overridden (see below for an example or the help text above).
-
 ## Install
 
 ```shell
 pip install pre-commit-gitlabci-lint
 ```
 
 ## Usage
 
-### Requirements
-
-GitLab Lint API now [requires authorization](https://gitlab.com/gitlab-org/gitlab/-/issues/321290).
+### Setup
 
 1. [Create an access token](https://gitlab.com/-/profile/personal_access_tokens) with `api` scope.
-2. Set access token value as a `GITLAB_TOKEN` or `GITLABCI_LINT_TOKEN` environment variable.
-3. Ensure Python version available is 3.8 or later.
-
-> **Warning:** GitLab tokens should not be shared. If leaked they can cause significant harm. Never store tokens in a repoitory.
+2. Set access token value in an environment variable named `GITLAB_TOKEN` or `GITLABCI_LINT_TOKEN`.
+3. Add the projectId for your gitlab project as a command line argument, or set it in the config file.
+4. Ensure the virtualenv Python version is 3.8 or later.
 
 ### Example
 
 An example `.pre-commit-config.yaml`:
 
 ```yaml
 ---
 repos:
   - repo: https://github.com/bjd2385/pre-commit-gitlabci-lint
     rev: <latest release>
     hooks:
       - id: gitlabci-lint
-      # args: [-b, 'https://custom.gitlab.host.com']
+      # args: [-b, 'https://custom.gitlab.host.com', '-p', '12345678']
 ```
 
-### Configuration files
+### Use configuration files
 
 No configuration file is required for use. However, if you'd rather specify settings in your repo, you may create a config file located at `/root/of/repo/.gitlabci-lint.toml`, or `$HOME/.config/.gitlabci-lint/config.toml`, such as the following.
 
 ```toml
 [gitlabci-lint]
 quiet = false
 base-url = "https://gitlab.com"
+project-id = "12345678"
 configs = [ ".gitlab-ci.yml" ]
 token = "$GITLAB_TOKEN"
 ```
-
-## Development
-
-Install dependencies by running `./scripts/dependencies.sh`. Or, if you already have `yarn` in your path, `yarn install:deps`.
-
-### Releases
-
-Update `setup.py/version`-string and tag this repo's master branch with the same version string (prefixed by '`v`.)
```

### Comparing `pre-commit-gitlabci-lint-1.2.2/setup.py` & `pre-commit-gitlabci-lint-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,27 +19,29 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='pre-commit-gitlabci-lint',
-    version='1.2.2',
+    version='1.3.0',
     description='Validate your GitLab CI with GitLab\'s API endpoint.',
     cmdclass=cmd_classes,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Emma Doyle',
     author_email='bjd2385.linux@gmail.com',
     keywords='pre-commit, GitLab, CI, continuous integration',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     python_requires='>=3.8, <4',
     url = 'https://github.com/bjd2385/pre-commit-gitlabci-lint',
-    install_requires=[],
+    install_requires=[
+        'toml'
+    ],
     entry_points={
         "console_scripts": ["gitlabci-lint = gitlabci_lint.validate:cli"]
     },
     project_urls={  # Optional
         'Bug Reports': 'https://github.com/bjd2385/pre-commit-gitlabci-lint/issues',
         'Source': 'https://github.com/bjd2385/pre-commit-gitlabci-lint'
     },
```

### Comparing `pre-commit-gitlabci-lint-1.2.2/src/gitlabci_lint/validate.py` & `pre-commit-gitlabci-lint-1.3.0/src/gitlabci_lint/validate.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 """
 
 
 import argparse
 import json
 import os
 import sys
-import configparser
+import toml
 import importlib.metadata as meta
 import pathlib
 
 from urllib.error import HTTPError
 from urllib.parse import urljoin
 from urllib.request import Request, urlopen
 from http import HTTPStatus
 from functools import partial
 from typing import List, Optional
 
 
 __version__ = meta.version('pre-commit-gitlabci-lint')
 
-
 errprint = partial(print, file=sys.stderr)
 
 default_config_section = 'gitlabci-lint'
 default_base_url: str = 'https://gitlab.com/'
 default_quiet: bool = False
 default_configs: List[str] = list()
 
 
-def validateCiConfig(token: str, baseUrl: str, configs: List[str], silent: bool) -> int:
+def validateCiConfig(token: str, baseUrl: str, project_id: str, configs: List[str], silent: bool) -> int:
     """
     Validate the input GitLab CI config against the validation API endpoint.
 
     Args:
         baseUrl: The location of the GitLab instance.
+        project_id: A gitlab project id.
         configFile: The GitLab CI file to validate.
         silent: Whether or not to output text on success or failure, unless improperly configured.
                 Allows the use of exit codes in scripts without redirecting stdout.
 
     Returns:
         An exit code, zero if successful and the CI config is valid.
     """
@@ -53,15 +53,15 @@
                         'content': f.read()
                     }
                 )
         except (FileNotFoundError, PermissionError):
             errprint(f'Cannot open {config}')
             returnValue = 1
         else:
-            url = urljoin(baseUrl, '/api/v4/ci/lint')
+            url = urljoin(baseUrl, f'/api/v4/projects/{project_id}/ci/lint')
             headers = {
                 'Content-Type': 'application/json',
                 'Content-Length': str(len(data))
             }
 
             # Get around mypy typing issue with if statement.
             if token:
@@ -82,21 +82,21 @@
                     if lint_output['status'] == 'invalid':
                         returnValue = 1
                 else:
                     # Lint verbosely.
                     with urlopen(request) as response:
                         lint_output = json.loads(response.read())
 
-                    if lint_output['status'] == 'invalid':
+                    if not lint_output['valid']:
                         errprint('=======')
                         for error in lint_output['errors']:
                             errprint(error)
                         returnValue = 1
                         errprint('=======')
-                    elif lint_output['status'] == 'valid' and lint_output['warnings']:
+                    elif lint_output['valid'] and lint_output['warnings']:
                         print(f'Config file at \'{config}\' is valid, with warnings:', end=' ')
                         for warning in lint_output['warnings']:
                             errprint(warning)
                     else:
                         print(f'Config file at \'{config}\' is valid.')
 
             except HTTPError as exc:
@@ -113,43 +113,38 @@
                 returnValue = 1
         if returnValue == 1:
             break
 
     return returnValue
 
 
-def config(conf: Optional[str] =None) -> configparser.ConfigParser:
+def config(conf: Optional[str] =None) -> dict:
     """
     Read a config file, if it exists, from standard locations.
 
     Returns:
         dict: The parsed config file.
     """
-    c = configparser.ConfigParser(
-        default_section=default_config_section
-    )
-
     config_locations = [conf] if conf else [
         '.gitlabci-lint.toml',
         os.path.expandvars('$HOME/.config/gitlabci-lint/config.toml')
     ]
 
     for loc in config_locations:
         try:
             if pathlib.Path(loc).exists():
-                c.read(pathlib.Path(loc))
-                break
+                return toml.load(pathlib.Path(loc))
             elif conf:
                 errprint(f'Could not locate config file at {loc}, please ensure this file exists.')
                 sys.exit(1)
         except PermissionError:
             errprint(f'Could not access config file at {loc}, check permissions.')
             sys.exit(1)
 
-    return c
+    return {}
 
 
 def cli() -> None:
     """
     Set up CLI for gitlabci-lint pre-commit hook.
     """
     parser = argparse.ArgumentParser(
@@ -169,67 +164,67 @@
 
     parser.add_argument(
         '-b', '-B', '--base-url', nargs='?', default=default_base_url,
         help=f'Base GitLab URL. (default: {default_base_url})'
     )
 
     parser.add_argument(
+        '-p', '-P', '--project-id',
+        help='Project ID to use with the lint API.'
+    )
+
+    parser.add_argument(
         '--version', action='version',
         version=f'%(prog)s {__version__}'
     )
 
     parser.add_argument(
         '-q', '-Q', '--quiet', action='store_true', default=False,
         help='Silently fail and pass, without output, unless improperly configured. '
              '(default: False)'
     )
 
     args = parser.parse_args()
 
     # If a gitlabci-lint config was specified via CLI, override the default search locations.
     hook_config_file_CLI = args.gitlabci_lint_config
-    if hook_config_file_CLI:
-        filesystem_config = config(*hook_config_file_CLI)
-    else:
-        filesystem_config = config()
+    filesystem_config = config(*hook_config_file_CLI) if hook_config_file_CLI else config()
 
     # Parse a potential config file, with defaults / fallback values matching the CLI's defaults.
-    quiet_CONF = filesystem_config[default_config_section].get('quiet', str(default_quiet).lower())
-    base_url_CONF = os.path.expandvars(filesystem_config[default_config_section].get('base-url', default_base_url))
-    configs_CONF = list(
-        map(
-            os.path.expandvars,
-            json.loads(filesystem_config[default_config_section].get('configs', str(default_configs)))
-        )
-    )
-    token_CONF = os.path.expandvars(filesystem_config[default_config_section].get('configs', ''))
+    gitlabci_lint_section = filesystem_config.get('gitlabci-lint', {})
+    quiet_CONF = gitlabci_lint_section.get('quiet', default_quiet)
+    base_url_CONF = os.path.expandvars(gitlabci_lint_section.get('base-url', default_base_url))
+    project_id_CONF = os.path.expandvars(gitlabci_lint_section.get('project-id', ''))
+    configs_CONF = list(map(os.path.expandvars, gitlabci_lint_section.get('configs', default_configs)))
+    token_CONF = os.path.expandvars(gitlabci_lint_section.get('token', ''))
 
     quiet_CLI = args.quiet
     base_url_CLI = args.base_url
     configs_CLI = args.configs
+    project_id_CLI = args.project_id
 
     # Decide which vars, configuration file or cli, take precendence. Basically how this logic works is, if a setting is
     # enabled in either the config file or via CLI args, it takes precedence.
     quiet = quiet_CONF == 'true' or quiet_CLI
     base_url = base_url_CLI if (base_url_CLI != default_base_url) else (base_url_CONF if (base_url_CONF != default_base_url) else base_url_CLI)
     configs = configs_CLI if (configs_CLI != default_configs) else (configs_CONF if (configs_CONF != default_configs) else configs_CLI)
+    project_id = project_id_CLI if project_id_CLI else project_id_CONF
+    if not project_id:
+        errprint('ERROR: No project ID specified. Please specify a project ID as a command line argument or in the config file.')
+        sys.exit(1)
 
     if not configs:
         # Set default, since there's a bug in argparse that I can't seem to overcome with specifying
         # multiple flags and defaults.
         configs = ['.gitlab-ci.yml']
 
-    token: Optional[str]
     if token_CONF:
         token = os.path.expandvars(token_CONF)
     elif not ((token := os.getenv('GITLABCI_LINT_TOKEN')) or (token := os.getenv('GITLAB_TOKEN'))):
         errprint('ERROR: Neither \'GITLABCI_LINT_TOKEN\' nor \'GITLAB_TOKEN\' set.')
         sys.exit(1)
 
-    if (exitCode := validateCiConfig(token, base_url, configs, quiet)) != os.EX_OK:
-            sys.exit(exitCode)
-
-    sys.exit(os.EX_OK)
+    sys.exit(validateCiConfig(token, base_url, project_id, configs, quiet))
 
 
 if __name__ == '__main__':
     cli()
```

