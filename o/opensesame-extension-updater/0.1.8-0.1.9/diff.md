# Comparing `tmp/opensesame_extension_updater-0.1.8.tar.gz` & `tmp/opensesame_extension_updater-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensesame_extension_updater-0.1.8.tar", max compression
+gzip compressed data, was "opensesame_extension_updater-0.1.9.tar", max compression
```

## Comparing `opensesame_extension_updater-0.1.8.tar` & `opensesame_extension_updater-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      108 2023-04-01 10:44:17.824821 opensesame_extension_updater-0.1.8/opensesame_extensions/updater/__init__.py
--rw-r--r--   0        0        0      564 2023-04-01 10:44:17.824821 opensesame_extension_updater-0.1.8/opensesame_extensions/updater/updater/__init__.py
--rw-r--r--   0        0        0     2383 2023-04-01 10:44:17.824821 opensesame_extension_updater-0.1.8/opensesame_extensions/updater/updater/update_widget.py
--rw-r--r--   0        0        0     2789 2023-04-01 10:44:17.824821 opensesame_extension_updater-0.1.8/opensesame_extensions/updater/updater/update_widget.ui
--rw-r--r--   0        0        0     9842 2023-04-01 10:44:17.824821 opensesame_extension_updater-0.1.8/opensesame_extensions/updater/updater/updater.py
--rw-r--r--   0        0        0      645 2023-04-01 10:44:17.824821 opensesame_extension_updater-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1238 2023-04-01 10:44:17.824821 opensesame_extension_updater-0.1.8/readme.md
--rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 opensesame_extension_updater-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      108 2023-04-01 13:58:51.666358 opensesame_extension_updater-0.1.9/opensesame_extensions/updater/__init__.py
+-rw-r--r--   0        0        0      564 2023-04-01 13:58:51.666358 opensesame_extension_updater-0.1.9/opensesame_extensions/updater/updater/__init__.py
+-rw-r--r--   0        0        0     2383 2023-04-01 13:58:51.666358 opensesame_extension_updater-0.1.9/opensesame_extensions/updater/updater/update_widget.py
+-rw-r--r--   0        0        0     2789 2023-04-01 13:58:51.666358 opensesame_extension_updater-0.1.9/opensesame_extensions/updater/updater/update_widget.ui
+-rw-r--r--   0        0        0    10149 2023-04-01 13:58:51.666358 opensesame_extension_updater-0.1.9/opensesame_extensions/updater/updater/updater.py
+-rw-r--r--   0        0        0      645 2023-04-01 13:58:51.666358 opensesame_extension_updater-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1238 2023-04-01 13:58:51.666358 opensesame_extension_updater-0.1.9/readme.md
+-rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 opensesame_extension_updater-0.1.9/PKG-INFO
```

### Comparing `opensesame_extension_updater-0.1.8/opensesame_extensions/updater/updater/__init__.py` & `opensesame_extension_updater-0.1.9/opensesame_extensions/updater/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_updater-0.1.8/opensesame_extensions/updater/updater/update_widget.py` & `opensesame_extension_updater-0.1.9/opensesame_extensions/updater/updater/update_widget.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_updater-0.1.8/opensesame_extensions/updater/updater/update_widget.ui` & `opensesame_extension_updater-0.1.9/opensesame_extensions/updater/updater/update_widget.ui`

 * *Files identical despite different names*

### Comparing `opensesame_extension_updater-0.1.8/opensesame_extensions/updater/updater/updater.py` & `opensesame_extension_updater-0.1.9/opensesame_extensions/updater/updater/updater.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,26 +128,27 @@
     for info in pkg_list:
         if info['name'] == pkg:
             info['platform'] = 'pypi'
             return info, parse(info['version'])
     return None, None
 
 
-def _check_conda(pkg):
+def _check_conda(pkg, prereleases):
     """Checks the latest version of a package on conda"""
-    info = _run('conda', 'search', 'pkg', '--info --json')
+    info = _run('conda', 'search', pkg, '--info', '--json')
     version = parse('0')
     if info is None:
         return version
     if pkg not in info:
         return version
     for release in info[pkg]:
         ver = parse(release['version'])
-        if not ver.is_prerelease:
-            version = max(version, ver)
+        if ver.is_prerelease and not prereleases:
+            continue
+        version = max(version, ver)
     return version
 
 
 def _check_pypi(pkg, prereleases):
     """Checks the latest version of a package on pypi"""
     req = requests.get(f'https://pypi.python.org/pypi/{pkg}/json')
     version = parse('0')
@@ -163,20 +164,20 @@
 
 
 def _check_update(pkg, pkg_info_fnc, prereleases):
     """Checks whether a package can be updated. Returns a UpdateInfo object
     if yes, and None otherwise.
     """
     info, current = pkg_info_fnc(pkg)
-    print(pkg, info, current)
     if info is None:
         return
     pypi = info['platform'] == 'pypi'
-    latest = _check_pypi(pkg, prereleases) if pypi else _check_conda(pkg)
-    print(latest)
+    latest = _check_pypi(pkg, prereleases) if pypi \
+        else _check_conda(pkg, prereleases)
+    print(f'checking updates for {pkg}: platform={info["platform"]}, current={current}, latest={latest}')
     if latest <= current:
         return
     return UpdateInfo(pkg, current, latest, pypi)
 
 
 def _check_updates(queue, pkgs, prereleases):
     """The main process function that checks for each package in pkgs whether
@@ -281,16 +282,20 @@
                           ' --pre' if cfg.updater_prereleases else '')
         self._update_script = '\n'.join(script)
         self.extension_manager.fire('notify',
                                     message=_('Some packages can be updated'))
         self.create_action()
         
     def create_action(self):
-        if self._widget is None and self._updates:
-            super().create_action()
+        if self._widget is not None or not self._updates:
+            return
+        super().create_action()
+        if 'OpensesameIde' not in self.extension_manager:
+            return
+        self.extension_manager['OpensesameIde']._toolbar.addAction(self.action)
 
     def _show_updates(self):
         if self._widget is None:
             from .update_widget import UpdateWidget
             self._widget = UpdateWidget(self.main_window)
         self.tabwidget.add(self._widget, 'system-software-update',
                            _('Updates available'), switch=True)
```

### Comparing `opensesame_extension_updater-0.1.8/pyproject.toml` & `opensesame_extension_updater-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opensesame-extension-updater"
-version = "0.1.8"
+version = "0.1.9"
 description = "Checks for updates to extensions and plugins in OpenSesame"
 authors = ["Sebastiaan Mathôt <s.mathot@cogsci.nl>"]
 readme = "readme.md"
 packages = [
     {include = "opensesame_extensions"},
 ]
 license = "COPYING"
```

### Comparing `opensesame_extension_updater-0.1.8/readme.md` & `opensesame_extension_updater-0.1.9/readme.md`

 * *Files identical despite different names*

### Comparing `opensesame_extension_updater-0.1.8/PKG-INFO` & `opensesame_extension_updater-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensesame-extension-updater
-Version: 0.1.8
+Version: 0.1.9
 Summary: Checks for updates to extensions and plugins in OpenSesame
 Home-page: https://osdoc.cogsci.nl
 License: COPYING
 Author: Sebastiaan Mathôt
 Author-email: s.mathot@cogsci.nl
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
```

