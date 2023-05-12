# Comparing `tmp/onboardme-1.0.0.tar.gz` & `tmp/onboardme-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.0.0.tar", max compression
+gzip compressed data, was "onboardme-1.0.1.tar", max compression
```

## Comparing `onboardme-1.0.0.tar` & `onboardme-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2023-03-18 21:02:57.842562 onboardme-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0    11849 2023-03-18 21:02:57.842562 onboardme-1.0.0/README.md
--rwxr-xr-x   0        0        0     6667 2023-03-18 21:02:57.870562 onboardme-1.0.0/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2023-03-18 21:02:57.870562 onboardme-1.0.0/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2023-03-18 21:02:57.870562 onboardme-1.0.0/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     2671 2023-03-18 21:02:57.870562 onboardme-1.0.0/onboardme/console_logging.py
--rw-r--r--   0        0        0     1544 2023-03-18 21:02:57.870562 onboardme-1.0.0/onboardme/constants.py
--rw-r--r--   0        0        0     4935 2023-03-18 21:02:57.870562 onboardme-1.0.0/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5606 2023-03-18 21:02:57.874562 onboardme-1.0.0/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-03-18 21:02:57.874562 onboardme-1.0.0/onboardme/firewall.py
--rwxr-xr-x   0        0        0     5692 2023-03-18 21:02:57.874562 onboardme-1.0.0/onboardme/help_text.py
--rw-r--r--   0        0        0     3123 2023-03-18 21:02:57.874562 onboardme-1.0.0/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2023-03-18 21:02:57.874562 onboardme-1.0.0/onboardme/misc.py
--rwxr-xr-x   0        0        0     8517 2023-03-18 21:02:57.874562 onboardme-1.0.0/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0       97 2023-03-18 21:02:57.874562 onboardme-1.0.0/onboardme/scripts/get_apt_list.sh
--rwxr-xr-x   0        0        0      233 2023-03-18 21:02:57.874562 onboardme-1.0.0/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-03-18 21:02:57.874562 onboardme-1.0.0/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2023-03-18 21:02:57.874562 onboardme-1.0.0/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1915 2023-03-18 21:02:57.874562 onboardme-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    13230 1970-01-01 00:00:00.000000 onboardme-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0    11868 2023-05-12 16:18:28.185568 onboardme-1.0.1/README.md
+-rwxr-xr-x   0        0        0     6667 2023-03-18 21:01:43.622076 onboardme-1.0.1/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.0.1/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.0.1/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     2671 2022-11-18 16:13:55.305455 onboardme-1.0.1/onboardme/console_logging.py
+-rw-r--r--   0        0        0     1544 2023-03-18 21:01:43.623119 onboardme-1.0.1/onboardme/constants.py
+-rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.0.1/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.0.1/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.0.1/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     5706 2023-05-12 16:18:28.187688 onboardme-1.0.1/onboardme/help_text.py
+-rw-r--r--   0        0        0     3123 2023-03-18 21:01:43.626062 onboardme-1.0.1/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.0.1/onboardme/misc.py
+-rwxr-xr-x   0        0        0     8607 2023-05-12 16:18:28.188160 onboardme-1.0.1/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.0.1/onboardme/scripts/get_apt_list.sh
+-rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.0.1/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.0.1/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.0.1/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1913 2023-05-12 16:18:28.189143 onboardme-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    13249 1970-01-01 00:00:00.000000 onboardme-1.0.1/PKG-INFO
```

### Comparing `onboardme-1.0.0/LICENSE.txt` & `onboardme-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.0/README.md` & `onboardme-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -138,16 +138,15 @@
 
 ### Configuration
 onboardme has lots of CLI options, but you can also use config files. You have to create these files for the time being.
 
 Config files are in `~/.config/onboardme/` (will use `$XDG_CONFIG_HOME`, if defined). Examples below:
 
 <details>
-<summary><code>config.yml</code></summary>
-
+<summary><code>~/.config/onboardme/config.yml</code></summary>
 
 ```yaml
 log:
   # Full path to a file you'd like to log to. Creates file if it doesn't exist
   file: ""
   # what level of logs to output (DEBUG, INFO, WARN, ERROR)
   level: "INFO"
```

#### html2text {}

```diff
@@ -54,46 +54,47 @@
 ```bash # should also work with pipx, if you'd like to use that instead pip
 install --user onboardme ``` You can read more in depth at the [Getting Started
 Docs] ð! There's also more [docs] on basically every program that onboardme
 touches. ### Upgrades If you're on python 3.11, you should be able to do:
 ```bash pip3.11 install --upgrade onboardme ``` ### Configuration onboardme has
 lots of CLI options, but you can also use config files. You have to create
 these files for the time being. Config files are in `~/.config/onboardme/`
-(will use `$XDG_CONFIG_HOME`, if defined). Examples below:  config.yml ```yaml
-log: # Full path to a file you'd like to log to. Creates file if it doesn't
-exist file: "" # what level of logs to output (DEBUG, INFO, WARN, ERROR) level:
-"INFO" # steps refer to a specific function in the list of functions we run
-steps: # these are mac specific steps Darwin: # clones dot files into home dir/
-git fetches updates for dot files - dot_files # install packages - packages #
-adds nerdfonts - font_setup # runs :Lazy sync to install all your plugins -
-neovim_setup # sets up touchID for sudo - sudo_setup # these are linux specific
-steps Linux: - dot_files - packages - font_setup - neovim_setup # add your user
-to the docker group - group_setup dot_files: # personal git repo URL for your
-dot files, defaults to jessebot/dot_files git_url: "https://github.com/
-jessebot/dot_files.git" # the branch to use for the git repo above, defaults to
-main git_branch: "main" # !CAREFUL: runs a `git reset --hard`, which will
-overwite/delete local files in ~ that # conflict with the above defined git
-repo url and branch. You should run # `onboardme -s dot_files` to get the files
-that would be overwritten overwrite: false # basic package config package: #
-Remove any of the below pkg managers to only run the remaining pkg managers
-managers: # these are macOS specific steps Darwin: - brew - pip3.11 # these are
-linux specific steps Linux: - brew - pip3.11 - apt - snap - flatpak # list of
-extra existing packages groups to install groups: - default # uncomment these
-to add them as default installed package groups # - gui # - gaming # - devops
-```  ## Under the Hood Made and tested for these operating systems: [![Tested
-on Ventura with an M1 and older generation](https://img.shields.io/badge/
-mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)](https://
-wikiless.org/wiki/MacOS?lang=en) [![Tested only on Debian Bookworm](https://
-img.shields.io/badge/Debian-A81D33?style=for-the-
-badge&logo=debian&logoColor=white)](https://www.debian.org/) [![Tested only on
-ubuntu servers](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-
-badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/) And optomized for the
-following programs: [![made-with-neovim](https://img.shields.io/badge/NeoVim-
-0f191f?style=for-the-badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/)
-[![made-with-python](https://img.shields.io/badge/Python-FFD43B?style=for-the-
+(will use `$XDG_CONFIG_HOME`, if defined). Examples below:  ~/.config/
+onboardme/config.yml ```yaml log: # Full path to a file you'd like to log to.
+Creates file if it doesn't exist file: "" # what level of logs to output
+(DEBUG, INFO, WARN, ERROR) level: "INFO" # steps refer to a specific function
+in the list of functions we run steps: # these are mac specific steps Darwin: #
+clones dot files into home dir/git fetches updates for dot files - dot_files #
+install packages - packages # adds nerdfonts - font_setup # runs :Lazy sync to
+install all your plugins - neovim_setup # sets up touchID for sudo - sudo_setup
+# these are linux specific steps Linux: - dot_files - packages - font_setup -
+neovim_setup # add your user to the docker group - group_setup dot_files: #
+personal git repo URL for your dot files, defaults to jessebot/dot_files
+git_url: "https://github.com/jessebot/dot_files.git" # the branch to use for
+the git repo above, defaults to main git_branch: "main" # !CAREFUL: runs a `git
+reset --hard`, which will overwite/delete local files in ~ that # conflict with
+the above defined git repo url and branch. You should run # `onboardme -
+s dot_files` to get the files that would be overwritten overwrite: false #
+basic package config package: # Remove any of the below pkg managers to only
+run the remaining pkg managers managers: # these are macOS specific steps
+Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
+pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
+install groups: - default # uncomment these to add them as default installed
+package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
+tested for these operating systems: [![Tested on Ventura with an M1 and older
+generation](https://img.shields.io/badge/mac%20os-000000?style=for-the-
+badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
+[Tested only on Debian Bookworm](https://img.shields.io/badge/Debian-
+A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
+www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
+badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
+ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
+(https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
+badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
+(https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
 (https://img.shields.io/badge/GNU%20Bash-000000?style=for-the-
 badge&logo=GNU%20Bash&logoColor=#5c983b)](https://www.gnu.org/software/bash/)
 [![made-with-powerline](https://img.shields.io/badge/powerline-
 000000?style=for-the-badge&logo=powerline&logoColor=#5c983b)](https://
 powerline.readthedocs.io/en/master/overview.html) #### Built using these great
 tools: [[rich python library logo with with yellow snake]](https://github.com/
```

### Comparing `onboardme-1.0.0/onboardme/__init__.py` & `onboardme-1.0.1/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.0/onboardme/config/firewall/iptables.sh` & `onboardme-1.0.1/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.0/onboardme/console_logging.py` & `onboardme-1.0.1/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.0/onboardme/constants.py` & `onboardme-1.0.1/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.0/onboardme/dot_files.py` & `onboardme-1.0.1/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.0/onboardme/env_config.py` & `onboardme-1.0.1/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.0/onboardme/firewall.py` & `onboardme-1.0.1/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.0/onboardme/help_text.py` & `onboardme-1.0.1/onboardme/help_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,8 +156,8 @@
                             title="⌥  Options",
                             title_align="left",
                             subtitle=url,
                             subtitle_align="right"))
 
         # I use this to print a pretty svg at the end sometimes
         if RECORD:
-            console.save_svg("docs/onboardme/screenshots/help_text.svg")
+            console.save_svg("docs/onboardme/screenshots/help_text.svg", title="term")
```

### Comparing `onboardme-1.0.0/onboardme/ide_setup.py` & `onboardme-1.0.1/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.0/onboardme/misc.py` & `onboardme-1.0.1/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.0/onboardme/pkg_management.py` & `onboardme-1.0.1/onboardme/pkg_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,20 @@
 
 def install_brew_taps(taps: list) -> None:
     """
     Checks current brew taps, and then runs brew tap {tap} on any taps that are
     in a list of git repos from packages.yaml, and aren't already tapped
     """
     log.info("Checking current taps.")
-    current_taps = subproc(["brew tap"]).split('\n')
+    existing_taps = subproc(["brew tap"])
+    try:
+        current_taps = existing_taps.split('\n')
+    except:
+        current_taps = []
+    
     log.debug(f"taps list is: {taps}")
     log.debug(f"Current taps are: {current_taps}")
 
     # for each tap, complete cmd by prepending `brew tap`
     for index, tap in enumerate(taps):
         log.debug(f"index: {index} tap: {tap}")
         # only brew tap if they don't already exist
```

### Comparing `onboardme-1.0.0/onboardme/subproc.py` & `onboardme-1.0.1/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.0/onboardme/sudo_setup.py` & `onboardme-1.0.1/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.0/pyproject.toml` & `onboardme-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.0.0"
+version       = "1.0.1"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = ["Jesse Hitch <jessebot@linux.com>",
                  "Max Roby <emax@cloudydev.net>"]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
 documentation = "https://jessebot.github.io/onboardme/onboardme"
 repository    = "http://github.com/jessebot/onboardme"
@@ -26,15 +26,15 @@
 rich                = "^13.3"
 PyYAML              = "^6.0"
 GitPython           = "^3.1"
 wget                = "^3.2"
 xdg-base-dirs       = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.1.1"
+pre-commit = "^3.1"
 
 [[tool.poetry.source]]
 name = "testpypi"
 url = "https://test.pypi.org/simple/"
 default = false
 secondary = false
```

### Comparing `onboardme-1.0.0/PKG-INFO` & `onboardme-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.0.0
+Version: 1.0.1
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
@@ -168,16 +168,15 @@
 
 ### Configuration
 onboardme has lots of CLI options, but you can also use config files. You have to create these files for the time being.
 
 Config files are in `~/.config/onboardme/` (will use `$XDG_CONFIG_HOME`, if defined). Examples below:
 
 <details>
-<summary><code>config.yml</code></summary>
-
+<summary><code>~/.config/onboardme/config.yml</code></summary>
 
 ```yaml
 log:
   # Full path to a file you'd like to log to. Creates file if it doesn't exist
   file: ""
   # what level of logs to output (DEBUG, INFO, WARN, ERROR)
   level: "INFO"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onboardme Version: 1.0.0 Summary: Install dot files
+Metadata-Version: 2.1 Name: onboardme Version: 1.0.1 Summary: Install dot files
 and packages, including a base mode with sensible defaults to run on most
 computers running Debian based distros or macOS. Home-page: http://github.com/
 jessebot/onboardme License: AGPL-3.0-or-later Keywords:
 onboardme,onboarding,desktop-setup,development-environment Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
@@ -73,46 +73,47 @@
 ```bash # should also work with pipx, if you'd like to use that instead pip
 install --user onboardme ``` You can read more in depth at the [Getting Started
 Docs] ð! There's also more [docs] on basically every program that onboardme
 touches. ### Upgrades If you're on python 3.11, you should be able to do:
 ```bash pip3.11 install --upgrade onboardme ``` ### Configuration onboardme has
 lots of CLI options, but you can also use config files. You have to create
 these files for the time being. Config files are in `~/.config/onboardme/`
-(will use `$XDG_CONFIG_HOME`, if defined). Examples below:  config.yml ```yaml
-log: # Full path to a file you'd like to log to. Creates file if it doesn't
-exist file: "" # what level of logs to output (DEBUG, INFO, WARN, ERROR) level:
-"INFO" # steps refer to a specific function in the list of functions we run
-steps: # these are mac specific steps Darwin: # clones dot files into home dir/
-git fetches updates for dot files - dot_files # install packages - packages #
-adds nerdfonts - font_setup # runs :Lazy sync to install all your plugins -
-neovim_setup # sets up touchID for sudo - sudo_setup # these are linux specific
-steps Linux: - dot_files - packages - font_setup - neovim_setup # add your user
-to the docker group - group_setup dot_files: # personal git repo URL for your
-dot files, defaults to jessebot/dot_files git_url: "https://github.com/
-jessebot/dot_files.git" # the branch to use for the git repo above, defaults to
-main git_branch: "main" # !CAREFUL: runs a `git reset --hard`, which will
-overwite/delete local files in ~ that # conflict with the above defined git
-repo url and branch. You should run # `onboardme -s dot_files` to get the files
-that would be overwritten overwrite: false # basic package config package: #
-Remove any of the below pkg managers to only run the remaining pkg managers
-managers: # these are macOS specific steps Darwin: - brew - pip3.11 # these are
-linux specific steps Linux: - brew - pip3.11 - apt - snap - flatpak # list of
-extra existing packages groups to install groups: - default # uncomment these
-to add them as default installed package groups # - gui # - gaming # - devops
-```  ## Under the Hood Made and tested for these operating systems: [![Tested
-on Ventura with an M1 and older generation](https://img.shields.io/badge/
-mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)](https://
-wikiless.org/wiki/MacOS?lang=en) [![Tested only on Debian Bookworm](https://
-img.shields.io/badge/Debian-A81D33?style=for-the-
-badge&logo=debian&logoColor=white)](https://www.debian.org/) [![Tested only on
-ubuntu servers](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-
-badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/) And optomized for the
-following programs: [![made-with-neovim](https://img.shields.io/badge/NeoVim-
-0f191f?style=for-the-badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/)
-[![made-with-python](https://img.shields.io/badge/Python-FFD43B?style=for-the-
+(will use `$XDG_CONFIG_HOME`, if defined). Examples below:  ~/.config/
+onboardme/config.yml ```yaml log: # Full path to a file you'd like to log to.
+Creates file if it doesn't exist file: "" # what level of logs to output
+(DEBUG, INFO, WARN, ERROR) level: "INFO" # steps refer to a specific function
+in the list of functions we run steps: # these are mac specific steps Darwin: #
+clones dot files into home dir/git fetches updates for dot files - dot_files #
+install packages - packages # adds nerdfonts - font_setup # runs :Lazy sync to
+install all your plugins - neovim_setup # sets up touchID for sudo - sudo_setup
+# these are linux specific steps Linux: - dot_files - packages - font_setup -
+neovim_setup # add your user to the docker group - group_setup dot_files: #
+personal git repo URL for your dot files, defaults to jessebot/dot_files
+git_url: "https://github.com/jessebot/dot_files.git" # the branch to use for
+the git repo above, defaults to main git_branch: "main" # !CAREFUL: runs a `git
+reset --hard`, which will overwite/delete local files in ~ that # conflict with
+the above defined git repo url and branch. You should run # `onboardme -
+s dot_files` to get the files that would be overwritten overwrite: false #
+basic package config package: # Remove any of the below pkg managers to only
+run the remaining pkg managers managers: # these are macOS specific steps
+Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
+pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
+install groups: - default # uncomment these to add them as default installed
+package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
+tested for these operating systems: [![Tested on Ventura with an M1 and older
+generation](https://img.shields.io/badge/mac%20os-000000?style=for-the-
+badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
+[Tested only on Debian Bookworm](https://img.shields.io/badge/Debian-
+A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
+www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
+badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
+ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
+(https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
+badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
+(https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
 (https://img.shields.io/badge/GNU%20Bash-000000?style=for-the-
 badge&logo=GNU%20Bash&logoColor=#5c983b)](https://www.gnu.org/software/bash/)
 [![made-with-powerline](https://img.shields.io/badge/powerline-
 000000?style=for-the-badge&logo=powerline&logoColor=#5c983b)](https://
 powerline.readthedocs.io/en/master/overview.html) #### Built using these great
 tools: [[rich python library logo with with yellow snake]](https://github.com/
```

