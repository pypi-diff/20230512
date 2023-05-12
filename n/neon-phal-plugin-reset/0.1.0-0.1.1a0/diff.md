# Comparing `tmp/neon-phal-plugin-reset-0.1.0.tar.gz` & `tmp/neon-phal-plugin-reset-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-reset-0.1.0.tar", last modified: Thu Feb  2 20:55:20 2023, max compression
+gzip compressed data, was "neon-phal-plugin-reset-0.1.1a0.tar", last modified: Fri May 12 19:14:05 2023, max compression
```

## Comparing `neon-phal-plugin-reset-0.1.0.tar` & `neon-phal-plugin-reset-0.1.1a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:55:20.493727 neon-phal-plugin-reset-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-02-02 20:55:17.000000 neon-phal-plugin-reset-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-02 20:55:17.000000 neon-phal-plugin-reset-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-02 20:55:20.493727 neon-phal-plugin-reset-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-02-02 20:55:17.000000 neon-phal-plugin-reset-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:55:20.493727 neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset/
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-02-02 20:55:17.000000 neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-02-02 20:55:17.000000 neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-02-02 20:55:17.000000 neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset/create_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-02-02 20:55:17.000000 neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:55:20.493727 neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-02 20:55:20.000000 neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-02 20:55:20.000000 neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 20:55:20.000000 neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-02 20:55:20.000000 neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-02 20:55:20.000000 neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-02 20:55:20.000000 neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:55:20.493727 neon-phal-plugin-reset-0.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-02 20:55:17.000000 neon-phal-plugin-reset-0.1.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 20:55:20.493727 neon-phal-plugin-reset-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-02-02 20:55:17.000000 neon-phal-plugin-reset-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:14:05.542487 neon-phal-plugin-reset-0.1.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-12 19:14:05.542487 neon-phal-plugin-reset-0.1.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:14:05.542487 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/create_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-12 19:14:04.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:14:05.542487 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-12 19:14:05.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-12 19:14:05.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:14:05.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-12 19:14:05.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-12 19:14:05.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 19:14:05.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:14:05.542487 neon-phal-plugin-reset-0.1.1a0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:14:05.542487 neon-phal-plugin-reset-0.1.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/setup.py
```

### Comparing `neon-phal-plugin-reset-0.1.0/LICENSE.md` & `neon-phal-plugin-reset-0.1.1a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.1.0/PKG-INFO` & `neon-phal-plugin-reset-0.1.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-reset
-Version: 0.1.0
+Version: 0.1.1a0
 Summary: Device Reset Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-reset
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description: # Neon Reset Plugin
         Plugin to handle factory reset requests. Note that this plugin will install system
```

### Comparing `neon-phal-plugin-reset-0.1.0/README.md` & `neon-phal-plugin-reset-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset/__init__.py` & `neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,31 +80,32 @@
         Handle a request to update configuration. Optionally restarts core
         services after update to ensure reload of default params
         """
         from neon_utils.packaging_utils import get_package_version_spec
         version = message.data.get("version") or \
             get_package_version_spec("neon-core").split('a')[0]
         LOG.info(f"Getting default config for Neon version: {version}")
+        default_branch = "master" if version.startswith("22.") else "dev"
+        default_dl_url = "https://github.com/neongeckocom/" \
+                         f"neon-image-recipe/archive/{default_branch}.zip"
         try:
             download_url = f"https://github.com/neongeckocom/" \
                            f"neon-image-recipe/archive/{version}.zip"
             LOG.debug(f"Downloading from {download_url}")
             download_extract_zip(download_url, "/tmp/neon/",
                                  skill_folder_name="neon-image-recipe")
         except BadZipFile:
             LOG.warning(f"No branch for version: {version}. Trying default")
-            download_url = "https://github.com/neongeckocom/" \
-                           "neon-image-recipe/archive/master.zip"
+            download_url = default_dl_url
             LOG.debug(f"Downloading from {download_url}")
             download_extract_zip(download_url, "/tmp/neon/",
                                  skill_folder_name="neon-image-recipe")
         except Exception as e:
             LOG.exception(e)
-            download_url = "https://github.com/neongeckocom/" \
-                           "neon-image-recipe/archive/master.zip"
+            download_url = default_dl_url
             LOG.debug(f"Downloading from {download_url}")
             download_extract_zip(download_url, "/tmp/neon/",
                                  skill_folder_name="neon-image-recipe")
 
         # Contents are now at /tmp/neon/neon-image-recipe
         try:
             if message.data.get('skill_config'):
```

### Comparing `neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset/config.py` & `neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/config.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset/create_media.py` & `neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/create_media.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset/version.py` & `neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.0"
+__version__ = "0.1.1a0"
```

### Comparing `neon-phal-plugin-reset-0.1.0/neon_phal_plugin_reset.egg-info/PKG-INFO` & `neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-reset
-Version: 0.1.0
+Version: 0.1.1a0
 Summary: Device Reset Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-reset
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description: # Neon Reset Plugin
         Plugin to handle factory reset requests. Note that this plugin will install system
```

### Comparing `neon-phal-plugin-reset-0.1.0/setup.py` & `neon-phal-plugin-reset-0.1.1a0/setup.py`

 * *Files identical despite different names*

