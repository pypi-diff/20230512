# Comparing `tmp/retaped_tui-1.0rc6.tar.gz` & `tmp/retaped_tui-1.0rc7.tar.gz`

## Comparing `retaped_tui-1.0rc6.tar` & `retaped_tui-1.0rc7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/.vscode/launch.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/__init__.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/aboutRT-tui.txt
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/globals.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/login.py
--rw-r--r--   0        0        0     9373 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/structures.py
--rw-r--r--   0        0        0     8276 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/widgets.py
--rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/__init__.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/apNPSApplication.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/apNPSApplicationAdvanced.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/apNPSApplicationEvents.py
--rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/apNPSApplicationManaged.py
--rw-r--r--   0        0        0    10257 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/apOptions.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/eveventhandler.py
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmActionForm.py
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmActionFormV2.py
--rw-r--r--   0        0        0     8371 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmFileSelector.py
--rw-r--r--   0        0        0    16155 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmForm.py
--rw-r--r--   0        0        0     8245 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmFormMultiPage.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmFormMutt.py
--rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmFormMuttActive.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmFormWithMenus.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmPopup.py
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fm_form_edit_loop.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/globals.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/muMenu.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/muNewMenu.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npysGlobalOptions.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npysNPSFilteredData.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npysThemeManagers.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npysThemes.py
--rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npysTree.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npyspmfuncs.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npyssafewrapper.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/proto_fm_screen_area.py
--rw-r--r--   0        0        0     9374 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/stdfmemail.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/utilNotify.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/util_viewhelp.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgFormControlCheckbox.py
--rw-r--r--   0        0        0     7840 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgNMenuDisplay.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgannotatetextbox.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgautocomplete.py
--rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgboxwidget.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgbutton.py
--rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgcheckbox.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgcombobox.py
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgdatecombo.py
--rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgeditmultiline.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgfilenamecombo.py
--rw-r--r--   0        0        0    12412 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wggrid.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wggridcoltitles.py
--rw-r--r--   0        0        0    10265 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmonthbox.py
--rw-r--r--   0        0        0    31961 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmultiline.py
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmultilineeditable.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmultilinetree.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmultilinetreeselectable.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmultiselect.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmultiselecttree.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgpassword.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgselectone.py
--rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgslider.py
--rw-r--r--   0        0        0    21858 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgtextbox.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgtextbox_controlchrs.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgtextboxunicode.py
--rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgtexttokens.py
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgtitlefield.py
--rw-r--r--   0        0        0    31166 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgwidget.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgwidget_proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/compatibility_code/__init__.py
--rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/compatibility_code/npysNPSTree.py
--rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/src/retaped_tui/npyscreen/compatibility_code/oldtreeclasses.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/LICENSE
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/README.md
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/pyproject.toml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 retaped_tui-1.0rc6/PKG-INFO
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/.vscode/launch.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/aboutRT-tui.txt
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/globals.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/login.py
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/structures.py
+-rw-r--r--   0        0        0     8276 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/widgets.py
+-rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/__init__.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/apNPSApplication.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/apNPSApplicationAdvanced.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/apNPSApplicationEvents.py
+-rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/apNPSApplicationManaged.py
+-rw-r--r--   0        0        0    10257 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/apOptions.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/eveventhandler.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmActionForm.py
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmActionFormV2.py
+-rw-r--r--   0        0        0     8371 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmFileSelector.py
+-rw-r--r--   0        0        0    16155 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmForm.py
+-rw-r--r--   0        0        0     8245 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmFormMultiPage.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmFormMutt.py
+-rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmFormMuttActive.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmFormWithMenus.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmPopup.py
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fm_form_edit_loop.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/globals.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/muMenu.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/muNewMenu.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npysGlobalOptions.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npysNPSFilteredData.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npysThemeManagers.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npysThemes.py
+-rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npysTree.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npyspmfuncs.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npyssafewrapper.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/proto_fm_screen_area.py
+-rw-r--r--   0        0        0     9374 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/stdfmemail.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/utilNotify.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/util_viewhelp.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgFormControlCheckbox.py
+-rw-r--r--   0        0        0     7840 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgNMenuDisplay.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgannotatetextbox.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgautocomplete.py
+-rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgboxwidget.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgbutton.py
+-rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgcheckbox.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgcombobox.py
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgdatecombo.py
+-rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgeditmultiline.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgfilenamecombo.py
+-rw-r--r--   0        0        0    12412 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wggrid.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wggridcoltitles.py
+-rw-r--r--   0        0        0    10265 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmonthbox.py
+-rw-r--r--   0        0        0    31961 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmultiline.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmultilineeditable.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmultilinetree.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmultilinetreeselectable.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmultiselect.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmultiselecttree.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgpassword.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgselectone.py
+-rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgslider.py
+-rw-r--r--   0        0        0    21858 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgtextbox.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgtextbox_controlchrs.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgtextboxunicode.py
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgtexttokens.py
+-rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgtitlefield.py
+-rw-r--r--   0        0        0    31166 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgwidget.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgwidget_proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/compatibility_code/__init__.py
+-rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/compatibility_code/npysNPSTree.py
+-rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/src/retaped_tui/npyscreen/compatibility_code/oldtreeclasses.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/LICENSE
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/README.md
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/pyproject.toml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 retaped_tui-1.0rc7/PKG-INFO
```

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/globals.py` & `retaped_tui-1.0rc7/src/retaped_tui/globals.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/login.py` & `retaped_tui-1.0rc7/src/retaped_tui/login.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/main.py` & `retaped_tui-1.0rc7/src/retaped_tui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     globals.websocket.send(json.dumps({"type": "Authenticate", "token": globals.token}))
 
 
 async def ws():
     try:
         wsInit()
     except TimeoutError:
-        npyscreen.notify('Connection FAILED')
+        npyscreen.notify('WS failed to connect', title='Connection failed')
         time.sleep(1)
         exit()
     while True:
         try:
             message = globals.websocket.recv()
         except TimeoutError:
             npyscreen.notify('Reconnecting', title='Disconnected')
@@ -112,20 +112,20 @@
 
 def sendMessage(totallyanargument):
     input = globals.inputBox.value
     if not globals.editingMessage:
         message = requests.post(f'{globals.apiEndpoint}/channels/{globals.currentChannel}/messages', headers={
             'x-session-token': globals.token}, data=json.dumps({'content': input, 'replies': globals.replies}))
         if message.status_code != 200:
-            npyscreen.notify(title='Failed to send')
+            npyscreen.notify(f'Status code: {message.status_code}', title='Failed to send')
             return 1
     else:
         message = requests.patch(f'{globals.apiEndpoint}/channels/{globals.currentChannel}/messages/{globals.editingMessageMsg.id}', headers={'x-session-token': globals.token}, data=json.dumps({'content': input}))
         if message.status_code != 200:
-                npyscreen.notify(title='Failed to send')
+                npyscreen.notify(f'Status code: {message.status_code}',title='Failed to send')
                 return 1
     globals.inputBox.value = ''
     clearReplies()
 
 def clearReplies():
     if globals.editingMessage:
         globals.inputBox.value=''
```

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/widgets.py` & `retaped_tui-1.0rc7/src/retaped_tui/widgets.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/__init__.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/__init__.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/apNPSApplication.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/apNPSApplication.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/apNPSApplicationEvents.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/apNPSApplicationEvents.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/apNPSApplicationManaged.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/apNPSApplicationManaged.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/apOptions.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/apOptions.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/eveventhandler.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/eveventhandler.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmActionForm.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmActionForm.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmActionFormV2.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmActionFormV2.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmFileSelector.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmFileSelector.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmForm.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmForm.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmFormMultiPage.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmFormMultiPage.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmFormMutt.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmFormMutt.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmFormMuttActive.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmFormMuttActive.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmFormWithMenus.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmFormWithMenus.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fmPopup.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fmPopup.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/fm_form_edit_loop.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/fm_form_edit_loop.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/muMenu.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/muMenu.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/muNewMenu.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/muNewMenu.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npysNPSFilteredData.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npysNPSFilteredData.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npysThemeManagers.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npysThemeManagers.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npysThemes.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npysThemes.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npysTree.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npysTree.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npyspmfuncs.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npyspmfuncs.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/npyssafewrapper.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/npyssafewrapper.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/proto_fm_screen_area.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/proto_fm_screen_area.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/stdfmemail.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/stdfmemail.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/utilNotify.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/utilNotify.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/util_viewhelp.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/util_viewhelp.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgFormControlCheckbox.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgFormControlCheckbox.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgNMenuDisplay.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgNMenuDisplay.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgannotatetextbox.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgannotatetextbox.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgautocomplete.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgautocomplete.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgboxwidget.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgboxwidget.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgbutton.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgbutton.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgcheckbox.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgcheckbox.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgcombobox.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgcombobox.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgdatecombo.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgdatecombo.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgeditmultiline.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgeditmultiline.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgfilenamecombo.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgfilenamecombo.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wggrid.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wggrid.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wggridcoltitles.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wggridcoltitles.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmonthbox.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmonthbox.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmultiline.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmultiline.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmultilineeditable.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmultilineeditable.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmultilinetree.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmultilinetree.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmultilinetreeselectable.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmultilinetreeselectable.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmultiselect.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmultiselect.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgmultiselecttree.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgmultiselecttree.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgpassword.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgpassword.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgselectone.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgselectone.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgslider.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgslider.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgtextbox.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgtextbox.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgtextbox_controlchrs.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgtextbox_controlchrs.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgtextboxunicode.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgtextboxunicode.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgtexttokens.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgtexttokens.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgtitlefield.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgtitlefield.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgwidget.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgwidget.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/wgwidget_proto.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/wgwidget_proto.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/compatibility_code/npysNPSTree.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/compatibility_code/npysNPSTree.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/src/retaped_tui/npyscreen/compatibility_code/oldtreeclasses.py` & `retaped_tui-1.0rc7/src/retaped_tui/npyscreen/compatibility_code/oldtreeclasses.py`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/LICENSE` & `retaped_tui-1.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `retaped_tui-1.0rc6/pyproject.toml` & `retaped_tui-1.0rc7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "retaped_tui"
-version = "1.0-rc6"
+version = "1.0-rc7"
 authors = [
   { name="Tetra Green", email="giggabyte6@gmail.com" },
 ]
 description = "A Revolt client for the terminal"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `retaped_tui-1.0rc6/PKG-INFO` & `retaped_tui-1.0rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retaped_tui
-Version: 1.0rc6
+Version: 1.0rc7
 Summary: A Revolt client for the terminal
 Project-URL: Homepage, https://github.com/error-404-null-not-found/Retaped-tui
 Project-URL: Bug Tracker, https://github.com/error-404-null-not-found/Retaped-tui/issues
 Author-email: Tetra Green <giggabyte6@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

