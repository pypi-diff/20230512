# Comparing `tmp/retaped_tui-1.0rc2.tar.gz` & `tmp/retaped_tui-1.0rc3.tar.gz`

## Comparing `retaped_tui-1.0rc2.tar` & `retaped_tui-1.0rc3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/.vscode/launch.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/src/retaped_tui/__init__.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/src/retaped_tui/aboutRT-tui.txt
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/src/retaped_tui/globals.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/src/retaped_tui/login.py
--rw-r--r--   0        0        0     9366 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/src/retaped_tui/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/src/retaped_tui/structures.py
--rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/src/retaped_tui/widgets.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/src/retaped_tui/npyscreen/wgselectone.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/LICENSE
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/pyproject.toml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 retaped_tui-1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/Retaped.yaml
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/.vscode/launch.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/aboutRT-tui.txt
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/globals.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/login.py
+-rw-r--r--   0        0        0     9366 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/structures.py
+-rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/widgets.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/npyscreen/wgselectone.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/LICENSE
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/PKG-INFO
```

### Comparing `retaped_tui-1.0rc2/src/retaped_tui/globals.py` & `retaped_tui-1.0rc3/src/retaped_tui/globals.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc2/src/retaped_tui/login.py` & `retaped_tui-1.0rc3/src/retaped_tui/login.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,21 +6,18 @@
 from . import globals
 class LoginForm(npyscreen.ActionForm):
     def create(self):
         self.name = 'Login'
         self.email=self.add(npyscreen.TitleText, name='Email')
         self.password=self.add(npyscreen.TitlePassword, name='Password')
         self.add(npyscreen.FixedText, value='Advanced options')
-        self.apiEnd=self.add(npyscreen.TitleText, name='API endpoint')
-        self.wsEnd=self.add(npyscreen.FixedText, name='WS endpoint')
+        self.apiEnd=self.add(npyscreen.TitleText, name='API endpoint', value='https://api.revolt.lea.pet')
+        self.wsEnd=self.add(npyscreen.TitleText, name='WS endpoint', value='wss://ws.revolt.lea.pet')
         self.edit()
     def on_ok(self):
-        if self.apiEnd.value and self.wsEnd.value:
-            globals.apiEndpoint=self.apiEnd.value
-            globals.wsEndpoint=self.wsEnd.value
         if self.email.value and self.password.value:
             response = requests.post(f'{globals.apiEndpoint}/auth/session/login', data=json.dumps({'email': self.email.value, 'password': self.password.value}))
             if response.status_code != 200:
                 exit(1)
             globals.token = response.json()['token']
             config = open(f'{globals.configPath}/Retaped.yaml', 'w')
             config.write(yaml.safe_dump({'token': globals.token, 'api-endpoint': globals.apiEndpoint, 'ws-endpoint': globals.wsEndpoint}))
```

### Comparing `retaped_tui-1.0rc2/src/retaped_tui/main.py` & `retaped_tui-1.0rc3/src/retaped_tui/main.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc2/src/retaped_tui/widgets.py` & `retaped_tui-1.0rc3/src/retaped_tui/widgets.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc2/src/retaped_tui/npyscreen/wgselectone.py` & `retaped_tui-1.0rc3/src/retaped_tui/npyscreen/wgselectone.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc2/LICENSE` & `retaped_tui-1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc2/pyproject.toml` & `retaped_tui-1.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "retaped_tui"
-version = "1.0-rc2"
+version = "1.0-rc3"
 authors = [
   { name="Tetra Green", email="giggabyte6@gmail.com" },
 ]
 description = "A Revolt client for the terminal"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `retaped_tui-1.0rc2/PKG-INFO` & `retaped_tui-1.0rc3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retaped_tui
-Version: 1.0rc2
+Version: 1.0rc3
 Summary: A Revolt client for the terminal
 Project-URL: Homepage, https://github.com/error-404-null-not-found/Retaped-tui
 Project-URL: Bug Tracker, https://github.com/error-404-null-not-found/Retaped-tui/issues
 Author-email: Tetra Green <giggabyte6@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

