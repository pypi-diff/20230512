# Comparing `tmp/retaped_tui-1.0rc3.tar.gz` & `tmp/retaped_tui-1.0rc5.tar.gz`

## Comparing `retaped_tui-1.0rc3.tar` & `retaped_tui-1.0rc5.tar`

### file list

```diff
@@ -1,14 +1,76 @@
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/Retaped.yaml
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/.vscode/launch.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/__init__.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/aboutRT-tui.txt
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/globals.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/login.py
--rw-r--r--   0        0        0     9366 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/structures.py
--rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/widgets.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/src/retaped_tui/npyscreen/wgselectone.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/LICENSE
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/pyproject.toml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 retaped_tui-1.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/.vscode/launch.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/aboutRT-tui.txt
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/globals.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/login.py
+-rw-r--r--   0        0        0     9366 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/structures.py
+-rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/widgets.py
+-rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/__init__.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/apNPSApplication.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/apNPSApplicationAdvanced.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/apNPSApplicationEvents.py
+-rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/apNPSApplicationManaged.py
+-rw-r--r--   0        0        0    10257 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/apOptions.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/eveventhandler.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/fmActionForm.py
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/fmActionFormV2.py
+-rw-r--r--   0        0        0     8371 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/fmFileSelector.py
+-rw-r--r--   0        0        0    16155 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/fmForm.py
+-rw-r--r--   0        0        0     8245 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/fmFormMultiPage.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/fmFormMutt.py
+-rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/fmFormMuttActive.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/fmFormWithMenus.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/fmPopup.py
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/fm_form_edit_loop.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/globals.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/muMenu.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/muNewMenu.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/npysGlobalOptions.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/npysNPSFilteredData.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/npysThemeManagers.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/npysThemes.py
+-rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/npysTree.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/npyspmfuncs.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/npyssafewrapper.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/proto_fm_screen_area.py
+-rw-r--r--   0        0        0     9374 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/stdfmemail.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/utilNotify.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/util_viewhelp.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgFormControlCheckbox.py
+-rw-r--r--   0        0        0     7840 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgNMenuDisplay.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgannotatetextbox.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgautocomplete.py
+-rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgboxwidget.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgbutton.py
+-rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgcheckbox.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgcombobox.py
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgdatecombo.py
+-rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgeditmultiline.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgfilenamecombo.py
+-rw-r--r--   0        0        0    12412 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wggrid.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wggridcoltitles.py
+-rw-r--r--   0        0        0    10265 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgmonthbox.py
+-rw-r--r--   0        0        0    31961 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgmultiline.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgmultilineeditable.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgmultilinetree.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgmultilinetreeselectable.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgmultiselect.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgmultiselecttree.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgpassword.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgselectone.py
+-rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgslider.py
+-rw-r--r--   0        0        0    21858 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgtextbox.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgtextbox_controlchrs.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgtextboxunicode.py
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgtexttokens.py
+-rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgtitlefield.py
+-rw-r--r--   0        0        0    31166 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgwidget.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgwidget_proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/compatibility_code/__init__.py
+-rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/compatibility_code/npysNPSTree.py
+-rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/src/retaped_tui/npyscreen/compatibility_code/oldtreeclasses.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/LICENSE
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/pyproject.toml
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 retaped_tui-1.0rc5/PKG-INFO
```

### Comparing `retaped_tui-1.0rc3/src/retaped_tui/globals.py` & `retaped_tui-1.0rc5/src/retaped_tui/globals.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc3/src/retaped_tui/login.py` & `retaped_tui-1.0rc5/src/retaped_tui/login.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc3/src/retaped_tui/main.py` & `retaped_tui-1.0rc5/src/retaped_tui/main.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc3/src/retaped_tui/widgets.py` & `retaped_tui-1.0rc5/src/retaped_tui/widgets.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc3/src/retaped_tui/npyscreen/wgselectone.py` & `retaped_tui-1.0rc5/src/retaped_tui/npyscreen/wgselectone.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc3/LICENSE` & `retaped_tui-1.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc3/PKG-INFO` & `retaped_tui-1.0rc5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: retaped_tui
-Version: 1.0rc3
+Version: 1.0rc5
 Summary: A Revolt client for the terminal
 Project-URL: Homepage, https://github.com/error-404-null-not-found/Retaped-tui
 Project-URL: Bug Tracker, https://github.com/error-404-null-not-found/Retaped-tui/issues
 Author-email: Tetra Green <giggabyte6@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.10
+Requires-Dist: npyscreen
+Requires-Dist: pyaml
+Requires-Dist: requests
+Requires-Dist: websockets
 Description-Content-Type: text/markdown
 
 # Retaped-TUI
 A shitty TUI Revolt client (real). Also currently the only TUI Revolt client
```

