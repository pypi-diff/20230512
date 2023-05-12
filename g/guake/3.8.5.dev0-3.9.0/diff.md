# Comparing `tmp/guake-3.8.5.dev0.tar.gz` & `tmp/guake-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guake-3.8.5.dev0.tar", last modified: Sun Feb  6 11:22:34 2022, max compression
+gzip compressed data, was "guake-3.9.0.tar", last modified: Sun Jun 12 13:53:06 2022, max compression
```

## Comparing `guake-3.8.5.dev0.tar` & `guake-3.9.0.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.415878 guake-3.8.5.dev0/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/.deepsource.toml
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/.pep8rc
--rw-r--r--   0 runner    (1001) docker     (121)    15868 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)    18002 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14785 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    51442 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-02-06 11:22:34.415878 guake-3.8.5.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      766 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)    66981 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.399877 guake-3.8.5.dev0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6812 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     6730 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.399877 guake-3.8.5.dev0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.399877 guake-3.8.5.dev0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/_static/.placeholder
--rw-r--r--   0 runner    (1001) docker     (121)     8778 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.399877 guake-3.8.5.dev0/docs/source/contributing/
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/contributing/basic.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/contributing/dev_env.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/contributing/hacking.rst
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/contributing/packaging.rst
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/contributing/release.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.399877 guake-3.8.5.dev0/docs/source/project/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/project/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/project/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/project/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/project/release_notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.399877 guake-3.8.5.dev0/docs/source/user/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/user/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/user/dbus.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2626 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/user/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/user/features.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/user/gtk3.rst
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3632 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/user/installing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/docs/source/user/whatisguake.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.403878 guake-3.8.5.dev0/guake/
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-02-06 11:22:34.000000 guake-3.8.5.dev0/guake/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/about.py
--rw-r--r--   0 runner    (1001) docker     (121)    25587 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/boxes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3373 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2453 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2958 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/customcommands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.407878 guake-3.8.5.dev0/guake/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5743 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/about.glade
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/autostart-guake.desktop
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/guake-prefs.template.desktop
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/guake.desktop.metainfo.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3242 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/guake.glade
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/guake.template.desktop
--rw-r--r--   0 runner    (1001) docker     (121)    34000 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/org.guake.gschema.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.407878 guake-3.8.5.dev0/guake/data/pixmaps/
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/add_tab.png
--rw-r--r--   0 runner    (1001) docker     (121)    10759 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/guake-128.png
--rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/guake-48.png
--rw-r--r--   0 runner    (1001) docker     (121)     4156 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/guake-64.png
--rw-r--r--   0 runner    (1001) docker     (121)     2974 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/guake-notification.png
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/guake-tray.png
--rw-r--r--   0 runner    (1001) docker     (121)   212131 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/guake-tray.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4156 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/guake.png
--rw-r--r--   0 runner    (1001) docker     (121)   182473 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/intro-large.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   145443 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/intro-medium.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    70962 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/intro-small.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    71682 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/quick-open-python-exception.png
--rw-r--r--   0 runner    (1001) docker     (121)    39605 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/quick-open-selection.png
--rw-r--r--   0 runner    (1001) docker     (121)    18944 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/quick-open.png
--rw-r--r--   0 runner    (1001) docker     (121)   125880 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/screenshot-fullscreen.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    35306 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/pixmaps/screenshot-small.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   235433 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/prefs.glade
--rw-r--r--   0 runner    (1001) docker     (121)    10326 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/data/search.glade
--rwxr-xr-x   0 runner    (1001) docker     (121)     6827 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/dbusiface.py
--rw-r--r--   0 runner    (1001) docker     (121)     5250 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3863 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/globals.py
--rw-r--r--   0 runner    (1001) docker     (121)    21482 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/gsettings.py
--rw-r--r--   0 runner    (1001) docker     (121)    58891 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/guake_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/guake_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/guake_toggle.py
--rw-r--r--   0 runner    (1001) docker     (121)    10084 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/keybindings.py
--rw-r--r--   0 runner    (1001) docker     (121)    18459 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     7530 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/menus.py
--rw-r--r--   0 runner    (1001) docker     (121)    23335 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/notebook.py
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)    55379 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/palettes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2802 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/guake/paths.py
--rw-r--r--   0 runner    (1001) docker     (121)    58887 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/prefs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4512 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     8318 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/simplegladeapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     6133 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/split_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2409 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/support.py
--rw-r--r--   0 runner    (1001) docker     (121)    25914 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/terminal.py
--rw-r--r--   0 runner    (1001) docker     (121)     3655 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/theme.py
--rw-r--r--   0 runner    (1001) docker     (121)    18206 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/guake/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.403878 guake-3.8.5.dev0/guake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-02-06 11:22:34.000000 guake-3.8.5.dev0/guake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-02-06 11:22:34.000000 guake-3.8.5.dev0/guake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-06 11:22:34.000000 guake-3.8.5.dev0/guake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-02-06 11:22:34.000000 guake-3.8.5.dev0/guake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-02-06 11:22:34.000000 guake-3.8.5.dev0/guake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-06 11:22:34.000000 guake-3.8.5.dev0/guake.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.415878 guake-3.8.5.dev0/po/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/po/LINGUAS
--rw-r--r--   0 runner    (1001) docker     (121)    32033 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/ca.mo
--rw-r--r--   0 runner    (1001) docker     (121)    45027 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/ca.po
--rw-r--r--   0 runner    (1001) docker     (121)    30649 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/cs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    43631 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/cs.po
--rw-r--r--   0 runner    (1001) docker     (121)    27542 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/de.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35963 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/de.po
--rw-r--r--   0 runner    (1001) docker     (121)     7348 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/el.mo
--rw-r--r--   0 runner    (1001) docker     (121)    37556 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/el.po
--rw-r--r--   0 runner    (1001) docker     (121)    31415 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/es.mo
--rw-r--r--   0 runner    (1001) docker     (121)    44482 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/es.po
--rw-r--r--   0 runner    (1001) docker     (121)     7481 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/fa.mo
--rw-r--r--   0 runner    (1001) docker     (121)    37354 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/fa.po
--rw-r--r--   0 runner    (1001) docker     (121)    33653 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/fi.mo
--rw-r--r--   0 runner    (1001) docker     (121)    44901 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/fi.po
--rw-r--r--   0 runner    (1001) docker     (121)    23851 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/fr.mo
--rw-r--r--   0 runner    (1001) docker     (121)    42909 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/fr.po
--rw-r--r--   0 runner    (1001) docker     (121)     8150 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/gl.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35597 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/gl.po
--rw-r--r--   0 runner    (1001) docker     (121)    32629 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/hr.mo
--rw-r--r--   0 runner    (1001) docker     (121)    44452 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/hr.po
--rw-r--r--   0 runner    (1001) docker     (121)     8085 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/hu.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35226 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/hu.po
--rw-r--r--   0 runner    (1001) docker     (121)     6712 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/id.mo
--rw-r--r--   0 runner    (1001) docker     (121)    32673 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/id.po
--rw-r--r--   0 runner    (1001) docker     (121)    23793 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/it.mo
--rw-r--r--   0 runner    (1001) docker     (121)    40924 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/it.po
--rw-r--r--   0 runner    (1001) docker     (121)    18936 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/ja.mo
--rw-r--r--   0 runner    (1001) docker     (121)    31656 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/ja.po
--rw-r--r--   0 runner    (1001) docker     (121)    16491 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/ko.mo
--rw-r--r--   0 runner    (1001) docker     (121)    37702 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/ko.po
--rw-r--r--   0 runner    (1001) docker     (121)    17968 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/nb.mo
--rw-r--r--   0 runner    (1001) docker     (121)    42633 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/nb.po
--rw-r--r--   0 runner    (1001) docker     (121)    33830 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/nl.mo
--rw-r--r--   0 runner    (1001) docker     (121)    45266 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/nl.po
--rw-r--r--   0 runner    (1001) docker     (121)     6777 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/pa.mo
--rw-r--r--   0 runner    (1001) docker     (121)    36587 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/pa.po
--rw-r--r--   0 runner    (1001) docker     (121)    27192 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/pl.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35349 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/pl.po
--rw-r--r--   0 runner    (1001) docker     (121)    17899 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/pt_BR.mo
--rw-r--r--   0 runner    (1001) docker     (121)    39287 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/pt_BR.po
--rw-r--r--   0 runner    (1001) docker     (121)    38899 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/ru.mo
--rw-r--r--   0 runner    (1001) docker     (121)    53492 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/ru.po
--rw-r--r--   0 runner    (1001) docker     (121)    26533 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/sv.mo
--rw-r--r--   0 runner    (1001) docker     (121)    34400 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/sv.po
--rw-r--r--   0 runner    (1001) docker     (121)    33502 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/tr.mo
--rw-r--r--   0 runner    (1001) docker     (121)    44886 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/tr.po
--rw-r--r--   0 runner    (1001) docker     (121)    11116 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/uk.mo
--rw-r--r--   0 runner    (1001) docker     (121)    37602 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/uk.po
--rw-r--r--   0 runner    (1001) docker     (121)    24023 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/zh_CN.mo
--rw-r--r--   0 runner    (1001) docker     (121)    39972 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/zh_CN.po
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/po/zh_TW.mo
--rw-r--r--   0 runner    (1001) docker     (121)    22967 2022-02-06 11:22:31.000000 guake-3.8.5.dev0/po/zh_TW.po
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-02-06 11:22:32.000000 guake-3.8.5.dev0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 11:22:34.415878 guake-3.8.5.dev0/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/scripts/all-sitedirs-in-prefix.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1198 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/scripts/bootstrap-dev-arch.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1485 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/scripts/bootstrap-dev-debian.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1138 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/scripts/bootstrap-dev-fedora.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      380 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/scripts/bootstrap-dev-pip.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      787 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/scripts/colortest
--rwxr-xr-x   0 runner    (1001) docker     (121)      310 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/scripts/run-local-prefs.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      362 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/scripts/run-local.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      225 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/scripts/test-exception.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      342 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/scripts/weird_urls.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-02-06 11:22:34.415878 guake-3.8.5.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-02-06 11:18:34.000000 guake-3.8.5.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.700087 guake-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-06-12 13:48:14.000000 guake-3.9.0/.deepsource.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2022-06-12 13:48:14.000000 guake-3.9.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-06-12 13:48:14.000000 guake-3.9.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2022-06-12 13:48:14.000000 guake-3.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-06-12 13:48:14.000000 guake-3.9.0/.pep8rc
+-rw-r--r--   0 runner    (1001) docker     (121)    15868 2022-06-12 13:48:14.000000 guake-3.9.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)    18002 2022-06-12 13:48:14.000000 guake-3.9.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-06-12 13:48:14.000000 guake-3.9.0/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-06-12 13:48:14.000000 guake-3.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    14772 2022-06-12 13:48:14.000000 guake-3.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)    51468 2022-06-12 13:48:14.000000 guake-3.9.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4153 2022-06-12 13:53:06.700087 guake-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2022-06-12 13:48:14.000000 guake-3.9.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (121)    76430 2022-06-12 13:48:14.000000 guake-3.9.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-06-12 13:48:14.000000 guake-3.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.680085 guake-3.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     6812 2022-06-12 13:48:14.000000 guake-3.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     6730 2022-06-12 13:48:14.000000 guake-3.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.680085 guake-3.9.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.680085 guake-3.9.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/_static/.placeholder
+-rw-r--r--   0 runner    (1001) docker     (121)     8346 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.680085 guake-3.9.0/docs/source/contributing/
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/contributing/basic.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/contributing/dev_env.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/contributing/hacking.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/contributing/packaging.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/contributing/release.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.680085 guake-3.9.0/docs/source/project/
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/project/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/project/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/project/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/project/release_notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.684086 guake-3.9.0/docs/source/user/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/user/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/user/dbus.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/user/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3649 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/user/features.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/user/gtk3.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3632 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/user/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-06-12 13:48:14.000000 guake-3.9.0/docs/source/user/whatisguake.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.688086 guake-3.9.0/guake/
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-06-12 13:48:14.000000 guake-3.9.0/guake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-06-12 13:53:06.000000 guake-3.9.0/guake/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-06-12 13:48:14.000000 guake-3.9.0/guake/about.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26191 2022-06-12 13:48:14.000000 guake-3.9.0/guake/boxes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3373 2022-06-12 13:48:14.000000 guake-3.9.0/guake/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2453 2022-06-12 13:48:14.000000 guake-3.9.0/guake/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2958 2022-06-12 13:48:14.000000 guake-3.9.0/guake/customcommands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.688086 guake-3.9.0/guake/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5743 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/about.glade
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/autostart-guake.desktop
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/guake-prefs.template.desktop
+-rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/guake.desktop.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     3242 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/guake.glade
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/guake.template.desktop
+-rw-r--r--   0 runner    (1001) docker     (121)    34611 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/org.guake.gschema.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.692086 guake-3.9.0/guake/data/pixmaps/
+-rw-r--r--   0 runner    (1001) docker     (121)      855 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/add_tab.png
+-rw-r--r--   0 runner    (1001) docker     (121)    10759 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/guake-128.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/guake-48.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4156 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/guake-64.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2974 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/guake-notification.png
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/guake-tray.png
+-rw-r--r--   0 runner    (1001) docker     (121)   212131 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/guake-tray.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     4156 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/guake.png
+-rw-r--r--   0 runner    (1001) docker     (121)   182473 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/intro-large.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   145443 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/intro-medium.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)    70962 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/intro-small.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)    71682 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/quick-open-python-exception.png
+-rw-r--r--   0 runner    (1001) docker     (121)    39605 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/quick-open-selection.png
+-rw-r--r--   0 runner    (1001) docker     (121)    18944 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/quick-open.png
+-rw-r--r--   0 runner    (1001) docker     (121)   125880 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/screenshot-fullscreen.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)    35306 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/pixmaps/screenshot-small.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   236408 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/prefs.glade
+-rw-r--r--   0 runner    (1001) docker     (121)    10326 2022-06-12 13:48:14.000000 guake-3.9.0/guake/data/search.glade
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7170 2022-06-12 13:48:14.000000 guake-3.9.0/guake/dbusiface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5250 2022-06-12 13:48:14.000000 guake-3.9.0/guake/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3849 2022-06-12 13:48:14.000000 guake-3.9.0/guake/globals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21496 2022-06-12 13:48:14.000000 guake-3.9.0/guake/gsettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60137 2022-06-12 13:48:14.000000 guake-3.9.0/guake/guake_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-06-12 13:48:14.000000 guake-3.9.0/guake/guake_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2022-06-12 13:48:14.000000 guake-3.9.0/guake/guake_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10932 2022-06-12 13:48:14.000000 guake-3.9.0/guake/keybindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18945 2022-06-12 13:48:14.000000 guake-3.9.0/guake/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7530 2022-06-12 13:48:14.000000 guake-3.9.0/guake/menus.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23375 2022-06-12 13:48:14.000000 guake-3.9.0/guake/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-06-12 13:48:14.000000 guake-3.9.0/guake/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)    55379 2022-06-12 13:48:14.000000 guake-3.9.0/guake/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2802 2022-06-12 13:53:05.000000 guake-3.9.0/guake/paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)    59376 2022-06-12 13:48:14.000000 guake-3.9.0/guake/prefs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4512 2022-06-12 13:48:14.000000 guake-3.9.0/guake/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8245 2022-06-12 13:48:14.000000 guake-3.9.0/guake/simplegladeapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6133 2022-06-12 13:48:14.000000 guake-3.9.0/guake/split_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2409 2022-06-12 13:48:14.000000 guake-3.9.0/guake/support.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25938 2022-06-12 13:48:14.000000 guake-3.9.0/guake/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3268 2022-06-12 13:48:14.000000 guake-3.9.0/guake/theme.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19207 2022-06-12 13:48:14.000000 guake-3.9.0/guake/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.688086 guake-3.9.0/guake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4153 2022-06-12 13:53:06.000000 guake-3.9.0/guake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-06-12 13:53:06.000000 guake-3.9.0/guake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-12 13:53:06.000000 guake-3.9.0/guake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-06-12 13:53:06.000000 guake-3.9.0/guake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-06-12 13:53:06.000000 guake-3.9.0/guake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-12 13:53:06.000000 guake-3.9.0/guake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.700087 guake-3.9.0/po/
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-06-12 13:48:14.000000 guake-3.9.0/po/LINGUAS
+-rw-r--r--   0 runner    (1001) docker     (121)    32033 2022-06-12 13:53:05.000000 guake-3.9.0/po/ca.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    45384 2022-06-12 13:53:03.000000 guake-3.9.0/po/ca.po
+-rw-r--r--   0 runner    (1001) docker     (121)    30649 2022-06-12 13:53:05.000000 guake-3.9.0/po/cs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    43988 2022-06-12 13:53:03.000000 guake-3.9.0/po/cs.po
+-rw-r--r--   0 runner    (1001) docker     (121)    27542 2022-06-12 13:53:05.000000 guake-3.9.0/po/de.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    36320 2022-06-12 13:53:03.000000 guake-3.9.0/po/de.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7348 2022-06-12 13:53:05.000000 guake-3.9.0/po/el.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    37913 2022-06-12 13:53:03.000000 guake-3.9.0/po/el.po
+-rw-r--r--   0 runner    (1001) docker     (121)    31415 2022-06-12 13:53:05.000000 guake-3.9.0/po/es.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    44839 2022-06-12 13:53:03.000000 guake-3.9.0/po/es.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7481 2022-06-12 13:53:05.000000 guake-3.9.0/po/fa.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    37711 2022-06-12 13:53:03.000000 guake-3.9.0/po/fa.po
+-rw-r--r--   0 runner    (1001) docker     (121)    33653 2022-06-12 13:53:05.000000 guake-3.9.0/po/fi.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    45258 2022-06-12 13:53:03.000000 guake-3.9.0/po/fi.po
+-rw-r--r--   0 runner    (1001) docker     (121)    23851 2022-06-12 13:53:05.000000 guake-3.9.0/po/fr.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    43266 2022-06-12 13:53:03.000000 guake-3.9.0/po/fr.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8150 2022-06-12 13:53:05.000000 guake-3.9.0/po/gl.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35954 2022-06-12 13:53:03.000000 guake-3.9.0/po/gl.po
+-rw-r--r--   0 runner    (1001) docker     (121)    32629 2022-06-12 13:53:05.000000 guake-3.9.0/po/hr.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    44809 2022-06-12 13:53:03.000000 guake-3.9.0/po/hr.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8085 2022-06-12 13:53:05.000000 guake-3.9.0/po/hu.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35583 2022-06-12 13:53:03.000000 guake-3.9.0/po/hu.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6712 2022-06-12 13:53:05.000000 guake-3.9.0/po/id.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    33030 2022-06-12 13:53:03.000000 guake-3.9.0/po/id.po
+-rw-r--r--   0 runner    (1001) docker     (121)    23793 2022-06-12 13:53:05.000000 guake-3.9.0/po/it.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    41281 2022-06-12 13:53:03.000000 guake-3.9.0/po/it.po
+-rw-r--r--   0 runner    (1001) docker     (121)    18936 2022-06-12 13:53:05.000000 guake-3.9.0/po/ja.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    32013 2022-06-12 13:53:04.000000 guake-3.9.0/po/ja.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16491 2022-06-12 13:53:05.000000 guake-3.9.0/po/ko.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    38059 2022-06-12 13:53:03.000000 guake-3.9.0/po/ko.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17968 2022-06-12 13:53:05.000000 guake-3.9.0/po/nb.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    42990 2022-06-12 13:53:03.000000 guake-3.9.0/po/nb.po
+-rw-r--r--   0 runner    (1001) docker     (121)    33830 2022-06-12 13:53:05.000000 guake-3.9.0/po/nl.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    45623 2022-06-12 13:53:03.000000 guake-3.9.0/po/nl.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6777 2022-06-12 13:53:05.000000 guake-3.9.0/po/pa.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    36944 2022-06-12 13:53:03.000000 guake-3.9.0/po/pa.po
+-rw-r--r--   0 runner    (1001) docker     (121)    27192 2022-06-12 13:53:05.000000 guake-3.9.0/po/pl.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35706 2022-06-12 13:53:03.000000 guake-3.9.0/po/pl.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17899 2022-06-12 13:53:05.000000 guake-3.9.0/po/pt_BR.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    39644 2022-06-12 13:53:03.000000 guake-3.9.0/po/pt_BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    38899 2022-06-12 13:53:05.000000 guake-3.9.0/po/ru.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    53849 2022-06-12 13:53:03.000000 guake-3.9.0/po/ru.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26533 2022-06-12 13:53:05.000000 guake-3.9.0/po/sv.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    34757 2022-06-12 13:53:03.000000 guake-3.9.0/po/sv.po
+-rw-r--r--   0 runner    (1001) docker     (121)    33502 2022-06-12 13:53:05.000000 guake-3.9.0/po/tr.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    45243 2022-06-12 13:53:04.000000 guake-3.9.0/po/tr.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11116 2022-06-12 13:53:05.000000 guake-3.9.0/po/uk.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    37959 2022-06-12 13:53:03.000000 guake-3.9.0/po/uk.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24023 2022-06-12 13:53:05.000000 guake-3.9.0/po/zh_CN.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    40329 2022-06-12 13:53:04.000000 guake-3.9.0/po/zh_CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-06-12 13:53:05.000000 guake-3.9.0/po/zh_TW.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    23324 2022-06-12 13:53:03.000000 guake-3.9.0/po/zh_TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-12 13:48:14.000000 guake-3.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-06-12 13:53:05.000000 guake-3.9.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-06-12 13:53:05.000000 guake-3.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 13:53:06.700087 guake-3.9.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-12 13:48:14.000000 guake-3.9.0/scripts/all-sitedirs-in-prefix.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1198 2022-06-12 13:48:14.000000 guake-3.9.0/scripts/bootstrap-dev-arch.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1485 2022-06-12 13:48:14.000000 guake-3.9.0/scripts/bootstrap-dev-debian.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1138 2022-06-12 13:48:14.000000 guake-3.9.0/scripts/bootstrap-dev-fedora.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      380 2022-06-12 13:48:14.000000 guake-3.9.0/scripts/bootstrap-dev-pip.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      787 2022-06-12 13:48:14.000000 guake-3.9.0/scripts/colortest
+-rwxr-xr-x   0 runner    (1001) docker     (121)      310 2022-06-12 13:48:14.000000 guake-3.9.0/scripts/run-local-prefs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      362 2022-06-12 13:48:14.000000 guake-3.9.0/scripts/run-local.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      225 2022-06-12 13:48:14.000000 guake-3.9.0/scripts/test-exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      342 2022-06-12 13:48:14.000000 guake-3.9.0/scripts/weird_urls.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-06-12 13:53:06.700087 guake-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-06-12 13:48:14.000000 guake-3.9.0/setup.py
```

### Comparing `guake-3.8.5.dev0/.editorconfig` & `guake-3.9.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/.gitignore` & `guake-3.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/.pylintrc` & `guake-3.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/COPYING` & `guake-3.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/Makefile` & `guake-3.9.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 	dconf reset -f /apps/guake/
 
 
 all: clean dev style checks dists test docs
 
 dev: clean-ln-venv ensure-pip pipenv-install-dev requirements ln-venv setup-githook \
 	 prepare-install install-dev-locale
-dev-actions: ensure-pip-system pipenv-install-dev requirements prepare-install
+dev-actions: ensure-pip-system pipenv-install-dev prepare-install
 
 ensure-pip:
 	./scripts/bootstrap-dev-pip.sh
 
 ensure-pip-system:
 	./scripts/bootstrap-dev-pip.sh system
```

### Comparing `guake-3.8.5.dev0/NEWS.rst` & `guake-3.9.0/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Guake Change Log
 ################
 
-3.8.4
+3.8.5
 =====
 
 New Features
 ------------
 
 - ``--is-visible`` option returns 1 when visible, and 0 when not
 
@@ -68,14 +68,19 @@
 - German (@m1ga, @rMb93)
 - Indonesian (@rezaalmanda)
 - Polish (@piotrdrag)
 - Russian (@vantu5z)
 - Swedish (@MorganAntonsson)
 - Turkish (@Draconis-25, @ersen0)
 
+3.8.4
+=====
+
+Unreleased.
+
 3.8.3
 =====
 
 Unreleased.
 
 3.8.2
 =====
```

### Comparing `guake-3.8.5.dev0/PKG-INFO` & `guake-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guake
-Version: 3.8.5.dev0
+Version: 3.9.0
 Summary: Guake Terminal
 Home-page: https://github.com/Guake/guake
 Author: Gaetan Semet
 Author-email: gaetan@xeberon.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
```

### Comparing `guake-3.8.5.dev0/Pipfile` & `guake-3.9.0/Pipfile`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 name = "pypi"
 
 [requires]
 python_version = "3"
 
 [dev-packages]
 "autopep8" = "*"
-"flake8" = "*"
+"flake8" = ">=3.8.0,<4.0.0"
 "pep8" = "*"
 pylint = "*"
 typed-ast = "*"
 astroid = "*"
 fiximports = ">=0.1.18"
 mock = ">=2.0.0"
 pytest-mock = "*"
@@ -30,13 +30,13 @@
 scandir = {markers = "python_version > '3.5'"}
 pyfakefs = "*"
 pytest-cov = "*"
 pew = "*"
 black = "==21.8b0"
 flakehell = "*"
 toml = "*"
-dataclasses = "*"
 
 [packages]
 pbr = "*"
 wheel = "*"
 typing = {markers = "python_version > '3.5'"}
+pyyaml = "*"
```

### Comparing `guake-3.8.5.dev0/Pipfile.lock` & `guake-3.9.0/Pipfile.lock`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9117505500550055%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'db17cdb4a1f7621cfed5e66c92df1ea73f1e94a8b587952fcebad77360157600'}}",*

 * * "'default'": "{'pbr': {'hashes': "*

 * *              "['sha256:27108648368782d07bbf1cb468ad2e2eeef29086affd14087a6d04b7de8af4ec', "*

 * *              "'sha256:66bc5a34912f408bb3925bf21231cb6f59206267b7f63f3503ef865c1a292e25'], "*

 * *              "'version': '==5.8.1'}, 'wheel': {'hashes': "*

 * *              "['sha256:4bdcd7d840138086126cd09254dc6195fb4fc6f01c050a1d7236f2630db1d22a', "*

 * *              "'sh […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "b69b985a0f7aa2c4219cdb943aa2d2a8ae53008321823ede34c1d792bece4315"
+            "sha256": "db17cdb4a1f7621cfed5e66c92df1ea73f1e94a8b587952fcebad77360157600"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3"
         },
         "sources": [
             {
@@ -14,53 +14,92 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "pbr": {
             "hashes": [
-                "sha256:42df03e7797b796625b1029c0400279c7c34fd7df24a7d7818a1abb5b38710dd",
-                "sha256:c68c661ac5cc81058ac94247278eeda6d2e6aecb3e227b0387c30d277e7ef8d4"
+                "sha256:27108648368782d07bbf1cb468ad2e2eeef29086affd14087a6d04b7de8af4ec",
+                "sha256:66bc5a34912f408bb3925bf21231cb6f59206267b7f63f3503ef865c1a292e25"
             ],
             "index": "pypi",
-            "version": "==5.6.0"
+            "version": "==5.8.1"
+        },
+        "pyyaml": {
+            "hashes": [
+                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
+                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
+                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
+                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
+                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
+                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
+                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
+                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
+                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
+                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
+                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
+                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
+                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
+                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
+                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
+                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
+                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
+                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
+                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
+                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
+                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
+                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
+                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
+                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
+                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
+                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
+                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
+                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
+                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
+                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
+                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
+                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
+                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+            ],
+            "index": "pypi",
+            "version": "==6.0"
         },
         "typing": {
             "hashes": [
                 "sha256:1187fb9c82fd670d10aa07bbb6cfcfe4bdda42d6fab8d5134f04e8c4d0b71cc9",
                 "sha256:283d868f5071ab9ad873e5e52268d611e851c870a2ba354193026f2dfb29d8b5"
             ],
             "index": "pypi",
             "markers": "python_version > '3.5'",
             "version": "==3.7.4.3"
         },
         "wheel": {
             "hashes": [
-                "sha256:21014b2bd93c6d0034b6ba5d35e4eb284340e09d63c59aef6fc14b0f346146fd",
-                "sha256:e2ef7239991699e3355d54f8e968a21bb940a1dbf34a4d226741e64462516fad"
+                "sha256:4bdcd7d840138086126cd09254dc6195fb4fc6f01c050a1d7236f2630db1d22a",
+                "sha256:e9a504e793efbca1b8e0e9cb979a249cf4a0a7b5b8c9e8b65a5e39d49529c1c4"
             ],
             "index": "pypi",
-            "version": "==0.37.0"
+            "version": "==0.37.1"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359",
                 "sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02"
             ],
             "version": "==0.7.12"
         },
         "astroid": {
             "hashes": [
-                "sha256:dcc06f6165f415220013801642bd6c9808a02967070919c4b746c6864c205471",
-                "sha256:fe81f80c0b35264acb5653302ffbd935d394f1775c5e4487df745bf9c2442708"
+                "sha256:4e5ba10571e197785e312966ea5efb2f5783176d4c1a73fa922d474ae2be59f7",
+                "sha256:f1af57483cd17e963b2eddce8361e00fc593d1520fe19948488e94ff6476bd71"
             ],
             "index": "pypi",
-            "version": "==2.8.0"
+            "version": "==2.11.3"
         },
         "attrs": {
             "hashes": [
                 "sha256:2d27e3784d7a565d36ab851fe94887c5eccd6a463168875832a1be79c82828b4",
                 "sha256:626ba8234211db98e869df76230a137c4c40a12d72445c45d5f5b716f076e2fd"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -158,45 +197,48 @@
                 "sha256:fd8a250edc26254fe5b33be00402e6d287f562b6a5b2152dec302fa15bb3e997",
                 "sha256:ffaa5c925128e29efbde7301d8ecaf35c8c60ffbcd6a1ffd3a552177c8e5e796"
             ],
             "version": "==1.15.0"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:876d180e9d7432c5d1dfd4c5d26b72f099d503e8fcc0feb7532c9289be60fcbd",
-                "sha256:cb957888737fc0bbcd78e3df769addb41fd1ff8cf950dc9e7ad7793f1bf44455"
+                "sha256:2857e29ff0d34db842cd7ca3230549d1a697f96ee6d3fb071cfa6c7393832597",
+                "sha256:6881edbebdb17b39b4eaaa821b438bf6eddffb4468cf344f09f89def34a8b1df"
             ],
             "markers": "python_version >= '3'",
-            "version": "==2.0.10"
+            "version": "==2.0.12"
         },
         "click": {
             "hashes": [
-                "sha256:353f466495adaeb40b6b5f592f9f91cb22372351c84caeb068132442a4518ef3",
-                "sha256:410e932b050f5eed773c4cda94de75971c89cdb3155a72a0831139a79e5ecb5b"
+                "sha256:6a7a62563bbfabfda3a38f3023a1db4a35978c0abd76f6c9605ecd6554d6d9b1",
+                "sha256:8458d7b1287c5fb128c90e23381cf99dcde74beaf6c7ff6384ce84d6fe090adb"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==8.0.3"
+            "version": "==8.0.4"
         },
         "colorama": {
             "hashes": [
                 "sha256:5941b2b48a20143d2267e95b1c2a7603ce057ee39fd88e7329b0c292aa16869b",
                 "sha256:9f47eda37229f68eee03b24b9748937c7dc3868f906e8ba69fbcbdd3bc5dc3e2"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==0.4.4"
         },
         "colorlog": {
             "hashes": [
-                "sha256:af99440154a01f27c09256760ea3477982bf782721feaa345904e806879df4d8",
-                "sha256:b13da382156711f7973bf7cbd1f40ea544aff51fde5dc3fb8f3fa602c321d645"
+                "sha256:344f73204009e4c83c5b6beb00b3c45dc70fcdae3c80db919e0a4171d006fde8",
+                "sha256:351c51e866c86c3217f08e4b067a7974a678be78f07f85fc2d55b8babde6d94e"
             ],
             "index": "pypi",
-            "version": "==6.4.1"
+            "version": "==6.6.0"
         },
         "coverage": {
+            "extras": [
+                "toml"
+            ],
             "hashes": [
                 "sha256:01774a2c2c729619760320270e42cd9e797427ecfddd32c2a7b639cdc481f3c0",
                 "sha256:03b20e52b7d31be571c9c06b74746746d4eb82fc260e594dc662ed48145e9efd",
                 "sha256:0a7726f74ff63f41e95ed3a89fef002916c828bb5fcae83b505b49d81a066884",
                 "sha256:1219d760ccfafc03c0822ae2e06e3b1248a8e6d1a70928966bafc6838d3c9e48",
                 "sha256:13362889b2d46e8d9f97c421539c97c963e34031ab0cb89e8ca83a10cc71ac76",
                 "sha256:174cf9b4bef0db2e8244f82059a5a72bd47e1d40e71c68ab055425172b16b7d0",
@@ -243,45 +285,53 @@
                 "sha256:fb8b8ee99b3fffe4fd86f4c81b35a6bf7e4462cba019997af2fe679365db0c49"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.2"
         },
         "cryptography": {
             "hashes": [
-                "sha256:0a817b961b46894c5ca8a66b599c745b9a3d9f822725221f0e0fe49dc043a3a3",
-                "sha256:2d87cdcb378d3cfed944dac30596da1968f88fb96d7fc34fdae30a99054b2e31",
-                "sha256:30ee1eb3ebe1644d1c3f183d115a8c04e4e603ed6ce8e394ed39eea4a98469ac",
-                "sha256:391432971a66cfaf94b21c24ab465a4cc3e8bf4a939c1ca5c3e3a6e0abebdbcf",
-                "sha256:39bdf8e70eee6b1c7b289ec6e5d84d49a6bfa11f8b8646b5b3dfe41219153316",
-                "sha256:4caa4b893d8fad33cf1964d3e51842cd78ba87401ab1d2e44556826df849a8ca",
-                "sha256:53e5c1dc3d7a953de055d77bef2ff607ceef7a2aac0353b5d630ab67f7423638",
-                "sha256:596f3cd67e1b950bc372c33f1a28a0692080625592ea6392987dba7f09f17a94",
-                "sha256:5d59a9d55027a8b88fd9fd2826c4392bd487d74bf628bb9d39beecc62a644c12",
-                "sha256:6c0c021f35b421ebf5976abf2daacc47e235f8b6082d3396a2fe3ccd537ab173",
-                "sha256:73bc2d3f2444bcfeac67dd130ff2ea598ea5f20b40e36d19821b4df8c9c5037b",
-                "sha256:74d6c7e80609c0f4c2434b97b80c7f8fdfaa072ca4baab7e239a15d6d70ed73a",
-                "sha256:7be0eec337359c155df191d6ae00a5e8bbb63933883f4f5dffc439dac5348c3f",
-                "sha256:94ae132f0e40fe48f310bba63f477f14a43116f05ddb69d6fa31e93f05848ae2",
-                "sha256:bb5829d027ff82aa872d76158919045a7c1e91fbf241aec32cb07956e9ebd3c9",
-                "sha256:ca238ceb7ba0bdf6ce88c1b74a87bffcee5afbfa1e41e173b1ceb095b39add46",
-                "sha256:ca28641954f767f9822c24e927ad894d45d5a1e501767599647259cbf030b903",
-                "sha256:e0344c14c9cb89e76eb6a060e67980c9e35b3f36691e15e1b7a9e58a0a6c6dc3",
-                "sha256:ebc15b1c22e55c4d5566e3ca4db8689470a0ca2babef8e3a9ee057a8b82ce4b1",
-                "sha256:ec63da4e7e4a5f924b90af42eddf20b698a70e58d86a72d943857c4c6045b3ee"
+                "sha256:0a3bf09bb0b7a2c93ce7b98cb107e9170a90c51a0162a20af1c61c765b90e60b",
+                "sha256:1f64a62b3b75e4005df19d3b5235abd43fa6358d5516cfc43d87aeba8d08dd51",
+                "sha256:32db5cc49c73f39aac27574522cecd0a4bb7384e71198bc65a0d23f901e89bb7",
+                "sha256:4881d09298cd0b669bb15b9cfe6166f16fc1277b4ed0d04a22f3d6430cb30f1d",
+                "sha256:4e2dddd38a5ba733be6a025a1475a9f45e4e41139d1321f412c6b360b19070b6",
+                "sha256:53e0285b49fd0ab6e604f4c5d9c5ddd98de77018542e88366923f152dbeb3c29",
+                "sha256:70f8f4f7bb2ac9f340655cbac89d68c527af5bb4387522a8413e841e3e6628c9",
+                "sha256:7b2d54e787a884ffc6e187262823b6feb06c338084bbe80d45166a1cb1c6c5bf",
+                "sha256:7be666cc4599b415f320839e36367b273db8501127b38316f3b9f22f17a0b815",
+                "sha256:8241cac0aae90b82d6b5c443b853723bcc66963970c67e56e71a2609dc4b5eaf",
+                "sha256:82740818f2f240a5da8dfb8943b360e4f24022b093207160c77cadade47d7c85",
+                "sha256:8897b7b7ec077c819187a123174b645eb680c13df68354ed99f9b40a50898f77",
+                "sha256:c2c5250ff0d36fd58550252f54915776940e4e866f38f3a7866d92b32a654b86",
+                "sha256:ca9f686517ec2c4a4ce930207f75c00bf03d94e5063cbc00a1dc42531511b7eb",
+                "sha256:d2b3d199647468d410994dbeb8cec5816fb74feb9368aedf300af709ef507e3e",
+                "sha256:da73d095f8590ad437cd5e9faf6628a218aa7c387e1fdf67b888b47ba56a17f0",
+                "sha256:e167b6b710c7f7bc54e67ef593f8731e1f45aa35f8a8a7b72d6e42ec76afd4b3",
+                "sha256:ea634401ca02367c1567f012317502ef3437522e2fc44a3ea1844de028fa4b84",
+                "sha256:ec6597aa85ce03f3e507566b8bcdf9da2227ec86c4266bd5e6ab4d9e0cc8dab2",
+                "sha256:f64b232348ee82f13aac22856515ce0195837f6968aeaa94a3d0353ea2ec06a6"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==36.0.1"
+            "version": "==36.0.2"
         },
         "dataclasses": {
             "hashes": [
-                "sha256:454a69d788c7fda44efd71e259be79577822f5e3f53f029a22d08004e951dc9f",
-                "sha256:6988bd2b895eef432d562370bb707d540f32f7360ab13da45340101bc2307d84"
+                "sha256:0201d89fa866f68c8ebd9d08ee6ff50c0b255f8ec63a71c16fda7af82bb887bf",
+                "sha256:8479067f342acf957dc82ec415d355ab5edb7e7646b90dc6e2fd1d96ad084c97"
             ],
-            "index": "pypi",
-            "version": "==0.6"
+            "markers": "python_version < '3.7'",
+            "version": "==0.8"
+        },
+        "dill": {
+            "hashes": [
+                "sha256:7e40e4a70304fd9ceab3535d36e58791d9c4a776b38ec7f7ec9afc8d3dca4d4f",
+                "sha256:9f9734205146b2b353ab3fec9af0070237b6ddae78452af83d2fca84d739e675"
+            ],
+            "markers": "python_version >= '2.7' and python_version != '3.0'",
+            "version": "==0.3.4"
         },
         "distlib": {
             "hashes": [
                 "sha256:6564fe0a8f51e734df6333d08b8b94d4ea8ee6b99b5ed50613f731fd4089f34b",
                 "sha256:e4b58818180336dc9c529bfb9a0b58728ffc09ad92027a3f30b7cd91e3458579"
             ],
             "version": "==0.3.4"
@@ -292,58 +342,58 @@
                 "sha256:cf316c8370a737a022b72b56874f6602acf974a37a9fba42ec2876387549fc61"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==0.17.1"
         },
         "dulwich": {
             "hashes": [
-                "sha256:10e7930236e9be118bd3ac5650188efc4bba4d504bbce0b534d59a728ef2672b",
-                "sha256:2998e950e899d564f7b96679384e6083696f9006f8e5d9d17178180733fdcadd",
-                "sha256:35bb491f5d9961af6e5ff04344d23973452afaa3686faef8582506049e0fa148",
-                "sha256:3b023c6e93b3d3c5d2634d3137cb5e1ae562602c4168df0e979675efeafde1f5",
-                "sha256:3b476b338ada4654a881ad3af1946e373609e19726e112b6cd980a0a7a8a1428",
-                "sha256:42c090a96bf617ba198611257b0333b07c37bce6975fb4c090b32e309c534e41",
-                "sha256:45c4c8d24cd40633cddd4198ff1d63875e4373301b38b34d0027164f87831a7b",
-                "sha256:46c1e26810f87bfd7a3658366499bceb47399f1f5f1cc8e13333e493ad555a7c",
-                "sha256:49d2999deaebbb91568c2f99e478117ffb46ee16ef4138d606990a89d25a4611",
-                "sha256:4aabc6b704f6e5c6f874f8d4ef818b0b39e9cd997a22e5959bdc09357f7e5106",
-                "sha256:5408b95e1927f5446cc2b784a81a51048091d06356075049687dbd85336824c4",
-                "sha256:5682bb5b4da89f571a6ded65bd8a570ccb90dd6d402bf7ca22f1182ef2a32ada",
-                "sha256:66f886b314f4fb0e3d8defe9e78f3ff9ddc5a9db85780bc0f91456267ebeabaa",
-                "sha256:98fca502ab62405b50be389e056d827b4645746ef02541e42a5ef24b1ac6cd41",
-                "sha256:a92df4f612984e5d37356f3e02b5864a4ad740b790f83e5510fa91cc14acedae",
-                "sha256:ad7b04706f197b0c39e63635a6c2c53adcc41755dd341a24ba034ea2a432a2d5",
-                "sha256:bdbc80809a0d211ccb160eb0a5a699b9a0c51c8bfcb0b87fe2d34c40e3e68d45",
-                "sha256:cd979fe0b83b4157ef5558b51e872386b3141af5c6268baa6a24224446bf45c8",
-                "sha256:d287fdd8a067ffc26b0f914b930e3e42189aeebd952d88aa5cf4a8df66b93604",
-                "sha256:e05f81dde255cd95a7e139f7e6a590f4c734a7c57b6f7f8fba4c201564883a67",
-                "sha256:f7b785b2adf497a73b77b0d66a823ea55154576207f00623ebb8ef89b38cabd3"
+                "sha256:134a2f586847c2c58569959a784d7a875b551df4226b639267302217799e4234",
+                "sha256:195b21c7a8f85cb2de8938d54fcc6d589d1ccbceaa63bb117796b531065bb68b",
+                "sha256:22c61a24edb699564b49a9701b723a08fa773f5d3322e8a0cabda897ae86816e",
+                "sha256:28ac2374f09487b02a8cb9b2fad083c358fc927bcfe9803d971614bc00e25076",
+                "sha256:3616a949053eb6bdf34581f57d1f6cb7192a4bb635be1a02c37f6f6dda032277",
+                "sha256:3d3d07b5aa51e6b7d08707c62932da86adbbaaa62552a0129b37d413735c7786",
+                "sha256:428b5fbb79f8cfba2f5ac6826cc813d1903b44b0780e9ec57e54cbd0f44feb61",
+                "sha256:581c6aa825c9267794747c5cc5ec3831960d96ca7fd9eb0158989e9a4099cbb1",
+                "sha256:5d94cd182fb0da4ec2f182be977b27b9cc1d7dbd0ee9bbf991e101a95fdcd3d8",
+                "sha256:6dc9b082f6ace9890de572260a575a09a996d617f5930edd2858c6f8fedfd7fb",
+                "sha256:8d683b4f30b1dae6b1668336f62f10ff57ebf2a1252c7cc76ad3eeff973879eb",
+                "sha256:953f6301a9df8a091fa88d55eed394a88bf9988cde8be341775354910918c196",
+                "sha256:9759cf611503681bcdd2950c9d2db04d1c057ecbb62d6fccd095b13771864f1c",
+                "sha256:9bdea3a4e8e5e3b1dbd513d9ab8a692f8a9a6f4760633e25c006446bce56fc5e",
+                "sha256:9d85b6b41c4be6df9ecdc4014d3cbe78a5a44a73c97bccbefac3e5de83bb74be",
+                "sha256:bf228800785754d7a55d52c5f122c26c3ced51f0f3df727fde2c9fefb71d5d76",
+                "sha256:c008b6b562af76cf011d3b5450a0d30edc96feeee7856b081d7400bc7cf42653",
+                "sha256:c4f4c59445dc5c2341e9cb2fe35e51a890e8a5f42178abec0a96044811c558a9",
+                "sha256:e11cc7a30b42dbbe5a0b6ebbfbfbb07138a5ffd6175bab2ddbabc9882a1c0438",
+                "sha256:f221c3c2fd10260419905bb673cd00129d491e3ed38c7a8d3ac2c7662682dd9b",
+                "sha256:f563e9f51e83c47a7df2f3cea79919f700e50d1e5556b6b753730b9cd2be1f47"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==0.20.30"
+            "version": "==0.20.35"
         },
         "e1839a8": {
             "editable": true,
             "path": "."
         },
         "entrypoints": {
             "hashes": [
-                "sha256:589f874b313739ad35be6e0cd7efde2a4e9b6fea91edcc34e58ecbb8dbe56d19",
-                "sha256:c70dd71abe5a8c85e55e12c19bd91ccfeec11a6e99044204511f9ed547d48451"
+                "sha256:b706eddaa9218a19ebcd67b56818f05bb27589b1ca9e8d797b74affad4ccacd4",
+                "sha256:f174b5ff827504fd3cd97cc3f8649f3693f51538c7e4bdf3ef002c8429d42f9f"
             ],
-            "markers": "python_version >= '2.7'",
-            "version": "==0.3"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.4"
         },
         "filelock": {
             "hashes": [
-                "sha256:38b4f4c989f9d06d44524df1b24bd19e167d851f19b50bf3e3559952dddc5b80",
-                "sha256:cf0fc6a2f8d26bd900f19bf33915ca70ba4dd8c56903eeb14e1e7a2fd7590146"
+                "sha256:0f12f552b42b5bf60dba233710bf71337d35494fc8bdd4fd6d9f6d082ad45e06",
+                "sha256:a4bc51381e01502a30e9f06dd4fa19a1712eab852b6fb0f84fd7cce0793d8ca3"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.4.2"
+            "markers": "python_version >= '3.6'",
+            "version": "==3.4.1"
         },
         "fiximports": {
             "hashes": [
                 "sha256:dafb83f981b430530bef61baf516e1e84d8cb1e202ecadb7d7988a3d0fddb875",
                 "sha256:f0216ee55a1bca8ff2a578a9bfc39181ce4553abc4401dd9b6f7c46164e62a13"
             ],
             "index": "pypi",
@@ -361,14 +411,18 @@
             "hashes": [
                 "sha256:208836d8d24194d50cfa4c1fc99f681f3c537cc232edcd06455abc2971460893",
                 "sha256:48a3a9b46136240e52b3b32a78a0826c45f6dcf7d980c30f758c1db5b1439c0b"
             ],
             "index": "pypi",
             "version": "==0.9.0"
         },
+        "guake": {
+            "editable": true,
+            "path": "."
+        },
         "idna": {
             "hashes": [
                 "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
                 "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
             ],
             "markers": "python_version >= '3'",
             "version": "==3.3"
@@ -379,33 +433,41 @@
                 "sha256:cd1750d452385ca327479d45b64d9c7729ecf0b3969a58148298c77092261f9d"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.3.0"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:92a8b58ce734b2a4494878e0ecf7d79ccd7a128b5fc6014c401e0b61f006f0f6",
-                "sha256:b7cf7d3fef75f1e4c80a96ca660efbd51473d7e8f39b5ab9210febc7809012a4"
+                "sha256:65a9576a5b2d58ca44d133c42a241905cc45e34d2c06fd5ba2bafa221e5d7b5e",
+                "sha256:766abffff765960fcc18003801f7044eb6755ffae4521c8e8ce8e83b9c9b0668"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==4.10.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==4.8.3"
+        },
+        "importlib-resources": {
+            "hashes": [
+                "sha256:33a95faed5fc19b4bc16b29a6eeae248a3fe69dd55d4d229d2b480e23eeaad45",
+                "sha256:d756e2f85dd4de2ba89be0b21dba2a3bbec2e871a42a3a16719258a11f87506b"
+            ],
+            "markers": "python_version < '3.7'",
+            "version": "==5.4.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:011e24c64b7f47f6ebd835bb12a743f2fbe9a26d4cecaa7f53bc4f35ee9da8b3",
                 "sha256:bc3af051d7d14b2ee5ef9969666def0cd1a000e121eaea580d4a313df4b37f32"
             ],
             "version": "==1.1.1"
         },
         "isort": {
             "hashes": [
                 "sha256:6f62d78e2f89b4500b080fe3a81690850cd254227f27f75c3a0c491a1f351ba7",
                 "sha256:e8443a5e7a020e9d7f97f1d7d9cd17c88bcb3bc7e218bf9cf5095fe550be2951"
             ],
-            "markers": "python_version < '4.0' and python_full_version >= '3.6.1'",
+            "markers": "python_version < '4' and python_full_version >= '3.6.1'",
             "version": "==5.10.1"
         },
         "jeepney": {
             "hashes": [
                 "sha256:1b5a0ea5c0e7b166b2f5895b91a08c14de8915afda4407fb5022a195224958ac",
                 "sha256:fa9e232dfa0c498bd0b8a3a73b8d8a31978304dcef0515adc859d4e096f96f4f"
             ],
@@ -418,19 +480,19 @@
                 "sha256:611bb273cd68f3b993fabdc4064fc858c5b47a973cb5aa7999ec1ba405c87cd7"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.0.3"
         },
         "keyring": {
             "hashes": [
-                "sha256:9012508e141a80bd1c0b6778d5c610dd9f8c464d75ac6774248500503f972fb9",
-                "sha256:b0d28928ac3ec8e42ef4cc227822647a19f1d544f21f96457965dc01cf555261"
+                "sha256:17e49fb0d6883c2b4445359434dba95aad84aabb29bbff044ad0ed7100232eca",
+                "sha256:89cbd74d4683ed164c8082fb38619341097741323b3786905c6dac04d6915a55"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.5.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==23.4.1"
         },
         "lazy-object-proxy": {
             "hashes": [
                 "sha256:043651b6cb706eee4f91854da4a089816a6606c1428fd391573ef8cb642ae4f7",
                 "sha256:07fa44286cda977bd4803b656ffc1c9b7e3bc7dff7d34263446aec8f8c96f88a",
                 "sha256:12f3bb77efe1367b2515f8cb4790a11cffae889148ad33adad07b9b55e0ab22c",
                 "sha256:2052837718516a94940867e16b1bb10edb069ab475c3ad84fd1e1a6dd2c0fcfc",
@@ -574,34 +636,34 @@
                 "sha256:ef103e05f519cdc783ae24ea4e2e0f508a9c99b2d4969652eed6a2e1ea5bd522"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==21.3"
         },
         "pathlib2": {
             "hashes": [
-                "sha256:3a130b266b3a36134dcc79c17b3c7ac9634f083825ca6ea9d8f557ee6195c9c8",
-                "sha256:7d8bcb5555003cdf4a8d2872c538faa3a0f5d20630cb360e518ca3b981795e5f"
+                "sha256:5266a0fd000452f1b3467d782f079a4343c63aaa119221fbdc4e39577489ca5b",
+                "sha256:9fe0edad898b83c0c3e199c842b27ed216645d2e177757b2dd67384d4113c641"
             ],
             "index": "pypi",
-            "version": "==2.3.6"
+            "version": "==2.3.7.post1"
         },
         "pathspec": {
             "hashes": [
                 "sha256:7d15c4ddb0b5c802d161efc417ec1a2558ea2653c2e8ad9c19098201dc1c993a",
                 "sha256:e564499435a2673d586f6b2130bb5b95f04a3ba06f81b8f895b651a3c76aabb1"
             ],
             "version": "==0.9.0"
         },
         "pbr": {
             "hashes": [
-                "sha256:42df03e7797b796625b1029c0400279c7c34fd7df24a7d7818a1abb5b38710dd",
-                "sha256:c68c661ac5cc81058ac94247278eeda6d2e6aecb3e227b0387c30d277e7ef8d4"
+                "sha256:27108648368782d07bbf1cb468ad2e2eeef29086affd14087a6d04b7de8af4ec",
+                "sha256:66bc5a34912f408bb3925bf21231cb6f59206267b7f63f3503ef865c1a292e25"
             ],
             "index": "pypi",
-            "version": "==5.6.0"
+            "version": "==5.8.1"
         },
         "pep8": {
             "hashes": [
                 "sha256:b22cfae5db09833bb9bd7c8463b53e1a9c9b39f12e304a8d0bba729c501827ee",
                 "sha256:fe249b52e20498e59e0b5c5256aa52ee99fc295b26ec9eaa85776ffdb9fe6374"
             ],
             "index": "pypi",
@@ -621,19 +683,19 @@
                 "sha256:fd11ba3d0fdb4c07fbc5ecbba0b1b719809420f25038f8ee3cd913d3faa3033a"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==21.3.1"
         },
         "pipenv": {
             "hashes": [
-                "sha256:3b80b4512934b9d8e8ce12c988394642ff96bb697680e5b092e59af503178327",
-                "sha256:f84d7119239b22ab2ac2b8fbc7d619d83cf41135206d72a17c4f151cda529fd0"
+                "sha256:3ac62c1121477b0758b0eef9e47643d5a2ba1b57e47a0789620ce5ef9bbc007e",
+                "sha256:53562bf69d9e5238f99a1e2101c356746b1c0aefa5dceb9b8a84a5a3e201de0d"
             ],
-            "index": "pypi",
-            "version": "==2022.1.8"
+            "markers": "python_version >= '3.6'",
+            "version": "==2022.4.8"
         },
         "pipenv-to-requirements": {
             "hashes": [
                 "sha256:1c18682a4ec70eb07261d2b558df3ee22ea00192663a1b98fd1e45e22946c163",
                 "sha256:cb70471a17a7d4658caffe989539413313d51df1b3a54838bcd7e7d3ab3fcc18"
             ],
             "index": "pypi",
@@ -644,19 +706,19 @@
                 "sha256:542e0d0b6750e2e21c20179803e40ab50598d8066d51097a0e382cba9eb02bff",
                 "sha256:c24c487c6a7f72c66e816ab1796b96ac6c3d14d49338293d2141664330b55ffc"
             ],
             "version": "==1.8.2"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:1d7385c7db91728b83efd0ca99a5afb296cab9d0ed8313a45ed8ba17967ecfca",
-                "sha256:440633ddfebcc36264232365d7840a970e75e1018d15b4327d11f91909045fda"
+                "sha256:367a5e80b3d04d2428ffa76d33f124cf11e8fff2acdaa9b43d545f5c7d661ef2",
+                "sha256:8868bbe3c3c80d42f20156f22e7131d2fb321f5bc86a2a345375c6481a67021d"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.4.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==2.4.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -679,24 +741,23 @@
             "version": "==2.7.0"
         },
         "pycparser": {
             "hashes": [
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.21"
         },
         "pyfakefs": {
             "hashes": [
-                "sha256:002a065dcbf59c2caa039e4fc4ba01d1d636aa63ee9c794d4c9fc01f0e2d6dc0",
-                "sha256:03a0e8e34e7250a458a640ca72c4c2c569bafc7e51a4c2d6c4ac62a426f60301"
+                "sha256:6bb4e27457b0bc90e3ebfe5aed4f1b8c32a18713ba44e925f304bb9b9816a03c",
+                "sha256:914d7bf994406cfbefee0b4d45918f60c15b406afe93f8194a804da5a450a822"
             ],
             "index": "pypi",
-            "version": "==4.5.1"
+            "version": "==4.5.6"
         },
         "pyflakes": {
             "hashes": [
                 "sha256:7893783d01b8a89811dd72d7dfd4d84ff098e5eed95cfa8905b22bbffe52efc3",
                 "sha256:f5bc8ecabc05bb9d291eb5203d6810b49040f6ff446a756326104746cc00c1db"
             ],
             "index": "pypi",
@@ -708,58 +769,58 @@
                 "sha256:4e426f72023d88d03b2fa258de560726ce890ff3b630f88c21cbb8b2503b8c6a"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==2.11.2"
         },
         "pylint": {
             "hashes": [
-                "sha256:0f358e221c45cbd4dad2a1e4b883e75d28acdcccd29d40c76eb72b307269b126",
-                "sha256:2c9843fff1a88ca0ad98a256806c82c5a8f86086e7ccbdb93297d86c3f90c436"
+                "sha256:8b1265173abaf37c2e7a21989d05fd6b0f8032c6772f85abe3b0652903aac66c",
+                "sha256:939e67253d1b8569a4c827d933debf603f999ba745775c66e36463922d4e320b"
             ],
             "index": "pypi",
-            "version": "==2.11.1"
+            "version": "==2.13.6"
         },
         "pyparsing": {
             "hashes": [
-                "sha256:04ff808a5b90911829c55c4e26f75fa5ca8a2f5f36aa3a51f68e27033341d3e4",
-                "sha256:d9bdec0013ef1eb5a84ab39a3b3868911598afa494f5faa038647101504e2b81"
+                "sha256:7bf433498c016c4314268d95df76c81b842a4cb2b276fa3312cfb1e1d85f6954",
+                "sha256:ef7b523f6356f763771559412c0d7134753f037822dad1b16945b7b846f7ad06"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.0.6"
+            "markers": "python_full_version >= '3.6.8'",
+            "version": "==3.0.8"
         },
         "pytest": {
             "hashes": [
-                "sha256:131b36680866a76e6781d13f101efb86cf674ebb9762eb70d3082b6f29889e89",
-                "sha256:7310f8d27bc79ced999e760ca304d69f6ba6c6649c0b60fb0e04a4a77cacc134"
+                "sha256:9ce3ff477af913ecf6321fe337b93a2c0dcf2a0a1439c43f5452112c1e4280db",
+                "sha256:e30905a0c131d3d94b89624a1cc5afec3e0ba2fbdb151867d8e0ebd49850f171"
             ],
             "index": "pypi",
-            "version": "==6.2.5"
+            "version": "==7.0.1"
         },
         "pytest-cov": {
             "hashes": [
-                "sha256:261bb9e47e65bd099c89c3edf92972865210c36813f80ede5277dceb77a4a62a",
-                "sha256:261ceeb8c227b726249b376b8526b600f38667ee314f910353fa318caa01f4d7"
+                "sha256:578d5d15ac4a25e5f961c938b85a05b09fdaae9deef3bb6de9a6e766622ca7a6",
+                "sha256:e7f0f5b1617d2210a2cabc266dfe2f4c75a8d32fb89eafb7ad9d06f6d076d470"
             ],
             "index": "pypi",
-            "version": "==2.12.1"
+            "version": "==3.0.0"
         },
         "pytest-mock": {
             "hashes": [
                 "sha256:30c2f2cc9759e76eee674b81ea28c9f0b94f8f0445a1b87762cadf774f0df7e3",
                 "sha256:40217a058c52a63f1042f0784f62009e976ba824c418cced42e88d5f40ab0e62"
             ],
             "index": "pypi",
             "version": "==3.6.1"
         },
         "pytz": {
             "hashes": [
-                "sha256:3672058bc3453457b622aab7a1c3bfd5ab0bdae451512f6cf25f64ed37f5b87c",
-                "sha256:acad2d8b20a1af07d4e4c9d2e9285c5ed9104354062f275f3fcd88dcef4f1326"
+                "sha256:1e760e2fe6a8163bc0b3d9a19c4f84342afa0a2affebfaa84b01b978a02ecaa7",
+                "sha256:e68985985296d9a66a881eb3193b0906246245294a881e7c8afe623866ac6a5c"
             ],
-            "version": "==2021.3"
+            "version": "==2022.1"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
                 "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
@@ -789,114 +850,115 @@
                 "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
                 "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
                 "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
                 "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
                 "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
-            "markers": "python_version >= '3.6'",
+            "index": "pypi",
             "version": "==6.0"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:a50a0f2123a4c1145ac6f420e1a348aafefcc9211c846e3d51df05fe3d865b7d",
-                "sha256:b512beafa6798260c7d5af3e1b1f097e58bfcd9a575da7c4ddd5e037490a5b85"
+                "sha256:262510fe6aae81ed4e94d8b169077f325614c0b1a45916a80442c6576264a9c2",
+                "sha256:dfb4d17f21706d145f7473e0b61ca245ba58e810cf9b2209a48239677f82e5b0"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==32.0"
+            "version": "==34.0"
         },
         "regex": {
             "hashes": [
-                "sha256:0416f7399e918c4b0e074a0f66e5191077ee2ca32a0f99d4c187a62beb47aa05",
-                "sha256:05b7d6d7e64efe309972adab77fc2af8907bb93217ec60aa9fe12a0dad35874f",
-                "sha256:0617383e2fe465732af4509e61648b77cbe3aee68b6ac8c0b6fe934db90be5cc",
-                "sha256:07856afef5ffcc052e7eccf3213317fbb94e4a5cd8177a2caa69c980657b3cb4",
-                "sha256:0f594b96fe2e0821d026365f72ac7b4f0b487487fb3d4aaf10dd9d97d88a9737",
-                "sha256:139a23d1f5d30db2cc6c7fd9c6d6497872a672db22c4ae1910be22d4f4b2068a",
-                "sha256:162abfd74e88001d20cb73ceaffbfe601469923e875caf9118333b1a4aaafdc4",
-                "sha256:2207ae4f64ad3af399e2d30dde66f0b36ae5c3129b52885f1bffc2f05ec505c8",
-                "sha256:2409b5c9cef7054dde93a9803156b411b677affc84fca69e908b1cb2c540025d",
-                "sha256:2fee3ed82a011184807d2127f1733b4f6b2ff6ec7151d83ef3477f3b96a13d03",
-                "sha256:30ab804ea73972049b7a2a5c62d97687d69b5a60a67adca07eb73a0ddbc9e29f",
-                "sha256:3598893bde43091ee5ca0a6ad20f08a0435e93a69255eeb5f81b85e81e329264",
-                "sha256:3b5df18db1fccd66de15aa59c41e4f853b5df7550723d26aa6cb7f40e5d9da5a",
-                "sha256:3c5fb32cc6077abad3bbf0323067636d93307c9fa93e072771cf9a64d1c0f3ef",
-                "sha256:416c5f1a188c91e3eb41e9c8787288e707f7d2ebe66e0a6563af280d9b68478f",
-                "sha256:42b50fa6666b0d50c30a990527127334d6b96dd969011e843e726a64011485da",
-                "sha256:432bd15d40ed835a51617521d60d0125867f7b88acf653e4ed994a1f8e4995dc",
-                "sha256:473e67837f786404570eae33c3b64a4b9635ae9f00145250851a1292f484c063",
-                "sha256:4aaa4e0705ef2b73dd8e36eeb4c868f80f8393f5f4d855e94025ce7ad8525f50",
-                "sha256:50a7ddf3d131dc5633dccdb51417e2d1910d25cbcf842115a3a5893509140a3a",
-                "sha256:529801a0d58809b60b3531ee804d3e3be4b412c94b5d267daa3de7fadef00f49",
-                "sha256:537ca6a3586931b16a85ac38c08cc48f10fc870a5b25e51794c74df843e9966d",
-                "sha256:53db2c6be8a2710b359bfd3d3aa17ba38f8aa72a82309a12ae99d3c0c3dcd74d",
-                "sha256:5537f71b6d646f7f5f340562ec4c77b6e1c915f8baae822ea0b7e46c1f09b733",
-                "sha256:563d5f9354e15e048465061509403f68424fef37d5add3064038c2511c8f5e00",
-                "sha256:5d408a642a5484b9b4d11dea15a489ea0928c7e410c7525cd892f4d04f2f617b",
-                "sha256:61600a7ca4bcf78a96a68a27c2ae9389763b5b94b63943d5158f2a377e09d29a",
-                "sha256:6650f16365f1924d6014d2ea770bde8555b4a39dc9576abb95e3cd1ff0263b36",
-                "sha256:666abff54e474d28ff42756d94544cdfd42e2ee97065857413b72e8a2d6a6345",
-                "sha256:68a067c11463de2a37157930d8b153005085e42bcb7ad9ca562d77ba7d1404e0",
-                "sha256:6e1d2cc79e8dae442b3fa4a26c5794428b98f81389af90623ffcc650ce9f6732",
-                "sha256:74cbeac0451f27d4f50e6e8a8f3a52ca074b5e2da9f7b505c4201a57a8ed6286",
-                "sha256:780b48456a0f0ba4d390e8b5f7c661fdd218934388cde1a974010a965e200e12",
-                "sha256:788aef3549f1924d5c38263104dae7395bf020a42776d5ec5ea2b0d3d85d6646",
-                "sha256:7ee1227cf08b6716c85504aebc49ac827eb88fcc6e51564f010f11a406c0a667",
-                "sha256:7f301b11b9d214f83ddaf689181051e7f48905568b0c7017c04c06dfd065e244",
-                "sha256:83ee89483672b11f8952b158640d0c0ff02dc43d9cb1b70c1564b49abe92ce29",
-                "sha256:85bfa6a5413be0ee6c5c4a663668a2cad2cbecdee367630d097d7823041bdeec",
-                "sha256:9345b6f7ee578bad8e475129ed40123d265464c4cfead6c261fd60fc9de00bcf",
-                "sha256:93a5051fcf5fad72de73b96f07d30bc29665697fb8ecdfbc474f3452c78adcf4",
-                "sha256:962b9a917dd7ceacbe5cd424556914cb0d636001e393b43dc886ba31d2a1e449",
-                "sha256:96fc32c16ea6d60d3ca7f63397bff5c75c5a562f7db6dec7d412f7c4d2e78ec0",
-                "sha256:98ba568e8ae26beb726aeea2273053c717641933836568c2a0278a84987b2a1a",
-                "sha256:a3feefd5e95871872673b08636f96b61ebef62971eab044f5124fb4dea39919d",
-                "sha256:a955b747d620a50408b7fdf948e04359d6e762ff8a85f5775d907ceced715129",
-                "sha256:b43c2b8a330a490daaef5a47ab114935002b13b3f9dc5da56d5322ff218eeadb",
-                "sha256:b483c9d00a565633c87abd0aaf27eb5016de23fed952e054ecc19ce32f6a9e7e",
-                "sha256:b9ed0b1e5e0759d6b7f8e2f143894b2a7f3edd313f38cf44e1e15d360e11749b",
-                "sha256:ba05430e819e58544e840a68b03b28b6d328aff2e41579037e8bab7653b37d83",
-                "sha256:ca49e1ab99593438b204e00f3970e7a5f70d045267051dfa6b5f4304fcfa1dbf",
-                "sha256:ca5f18a75e1256ce07494e245cdb146f5a9267d3c702ebf9b65c7f8bd843431e",
-                "sha256:cd410a1cbb2d297c67d8521759ab2ee3f1d66206d2e4328502a487589a2cb21b",
-                "sha256:ce298e3d0c65bd03fa65ffcc6db0e2b578e8f626d468db64fdf8457731052942",
-                "sha256:d5ca078bb666c4a9d1287a379fe617a6dccd18c3e8a7e6c7e1eb8974330c626a",
-                "sha256:d5fd67df77bab0d3f4ea1d7afca9ef15c2ee35dfb348c7b57ffb9782a6e4db6e",
-                "sha256:da1a90c1ddb7531b1d5ff1e171b4ee61f6345119be7351104b67ff413843fe94",
-                "sha256:dba70f30fd81f8ce6d32ddeef37d91c8948e5d5a4c63242d16a2b2df8143aafc",
-                "sha256:dc07f021ee80510f3cd3af2cad5b6a3b3a10b057521d9e6aaeb621730d320c5a",
-                "sha256:dd33eb9bdcfbabab3459c9ee651d94c842bc8a05fabc95edf4ee0c15a072495e",
-                "sha256:e0538c43565ee6e703d3a7c3bdfe4037a5209250e8502c98f20fea6f5fdf2965",
-                "sha256:e1f54b9b4b6c53369f40028d2dd07a8c374583417ee6ec0ea304e710a20f80a0",
-                "sha256:e32d2a2b02ccbef10145df9135751abea1f9f076e67a4e261b05f24b94219e36",
-                "sha256:e6096b0688e6e14af6a1b10eaad86b4ff17935c49aa774eac7c95a57a4e8c296",
-                "sha256:e71255ba42567d34a13c03968736c5d39bb4a97ce98188fafb27ce981115beec",
-                "sha256:ed2e07c6a26ed4bea91b897ee2b0835c21716d9a469a96c3e878dc5f8c55bb23",
-                "sha256:eef2afb0fd1747f33f1ee3e209bce1ed582d1896b240ccc5e2697e3275f037c7",
-                "sha256:f23222527b307970e383433daec128d769ff778d9b29343fb3496472dc20dabe",
-                "sha256:f341ee2df0999bfdf7a95e448075effe0db212a59387de1a70690e4acb03d4c6",
-                "sha256:f5be7805e53dafe94d295399cfbe5227f39995a997f4fd8539bf3cbdc8f47ca8",
-                "sha256:f7f325be2804246a75a4f45c72d4ce80d2443ab815063cdf70ee8fb2ca59ee1b",
-                "sha256:f8af619e3be812a2059b212064ea7a640aff0568d972cd1b9e920837469eb3cb",
-                "sha256:fa8c626d6441e2d04b6ee703ef2d1e17608ad44c7cb75258c09dd42bacdfc64b",
-                "sha256:fbb9dc00e39f3e6c0ef48edee202f9520dafb233e8b51b06b8428cfcb92abd30",
-                "sha256:fff55f3ce50a3ff63ec8e2a8d3dd924f1941b250b0aac3d3d42b687eeff07a8e"
+                "sha256:0066a6631c92774391f2ea0f90268f0d82fffe39cb946f0f9c6b382a1c61a5e5",
+                "sha256:0100f0ded953b6b17f18207907159ba9be3159649ad2d9b15535a74de70359d3",
+                "sha256:01c913cf573d1da0b34c9001a94977273b5ee2fe4cb222a5d5b320f3a9d1a835",
+                "sha256:0214ff6dff1b5a4b4740cfe6e47f2c4c92ba2938fca7abbea1359036305c132f",
+                "sha256:029e9e7e0d4d7c3446aa92474cbb07dafb0b2ef1d5ca8365f059998c010600e6",
+                "sha256:0317eb6331146c524751354ebef76a7a531853d7207a4d760dfb5f553137a2a4",
+                "sha256:04b5ee2b6d29b4a99d38a6469aa1db65bb79d283186e8460542c517da195a8f6",
+                "sha256:04c09b9651fa814eeeb38e029dc1ae83149203e4eeb94e52bb868fadf64852bc",
+                "sha256:058054c7a54428d5c3e3739ac1e363dc9347d15e64833817797dc4f01fb94bb8",
+                "sha256:060f9066d2177905203516c62c8ea0066c16c7342971d54204d4e51b13dfbe2e",
+                "sha256:0a7b75cc7bb4cc0334380053e4671c560e31272c9d2d5a6c4b8e9ae2c9bd0f82",
+                "sha256:0e2630ae470d6a9f8e4967388c1eda4762706f5750ecf387785e0df63a4cc5af",
+                "sha256:174d964bc683b1e8b0970e1325f75e6242786a92a22cedb2a6ec3e4ae25358bd",
+                "sha256:25ecb1dffc5e409ca42f01a2b2437f93024ff1612c1e7983bad9ee191a5e8828",
+                "sha256:286908cbe86b1a0240a867aecfe26a439b16a1f585d2de133540549831f8e774",
+                "sha256:303b15a3d32bf5fe5a73288c316bac5807587f193ceee4eb6d96ee38663789fa",
+                "sha256:34bb30c095342797608727baf5c8aa122406aa5edfa12107b8e08eb432d4c5d7",
+                "sha256:3e265b388cc80c7c9c01bb4f26c9e536c40b2c05b7231fbb347381a2e1c8bf43",
+                "sha256:3e4d710ff6539026e49f15a3797c6b1053573c2b65210373ef0eec24480b900b",
+                "sha256:42eb13b93765c6698a5ab3bcd318d8c39bb42e5fa8a7fcf7d8d98923f3babdb1",
+                "sha256:48081b6bff550fe10bcc20c01cf6c83dbca2ccf74eeacbfac240264775fd7ecf",
+                "sha256:491fc754428514750ab21c2d294486223ce7385446f2c2f5df87ddbed32979ae",
+                "sha256:4d1445824944e642ffa54c4f512da17a953699c563a356d8b8cbdad26d3b7598",
+                "sha256:530a3a16e57bd3ea0dff5ec2695c09632c9d6c549f5869d6cf639f5f7153fb9c",
+                "sha256:591d4fba554f24bfa0421ba040cd199210a24301f923ed4b628e1e15a1001ff4",
+                "sha256:5a86cac984da35377ca9ac5e2e0589bd11b3aebb61801204bd99c41fac516f0d",
+                "sha256:5b1ceede92400b3acfebc1425937454aaf2c62cd5261a3fabd560c61e74f6da3",
+                "sha256:5b2e24f3ae03af3d8e8e6d824c891fea0ca9035c5d06ac194a2700373861a15c",
+                "sha256:6504c22c173bb74075d7479852356bb7ca80e28c8e548d4d630a104f231e04fb",
+                "sha256:673f5a393d603c34477dbad70db30025ccd23996a2d0916e942aac91cc42b31a",
+                "sha256:6ca6dcd17f537e9f3793cdde20ac6076af51b2bd8ad5fe69fa54373b17b48d3c",
+                "sha256:6e1d8ed9e61f37881c8db383a124829a6e8114a69bd3377a25aecaeb9b3538f8",
+                "sha256:75a5e6ce18982f0713c4bac0704bf3f65eed9b277edd3fb9d2b0ff1815943327",
+                "sha256:76435a92e444e5b8f346aed76801db1c1e5176c4c7e17daba074fbb46cb8d783",
+                "sha256:764e66a0e382829f6ad3bbce0987153080a511c19eb3d2f8ead3f766d14433ac",
+                "sha256:78ce90c50d0ec970bd0002462430e00d1ecfd1255218d52d08b3a143fe4bde18",
+                "sha256:794a6bc66c43db8ed06698fc32aaeaac5c4812d9f825e9589e56f311da7becd9",
+                "sha256:797437e6024dc1589163675ae82f303103063a0a580c6fd8d0b9a0a6708da29e",
+                "sha256:7b7494df3fdcc95a1f76cf134d00b54962dd83189520fd35b8fcd474c0aa616d",
+                "sha256:7d1a6e403ac8f1d91d8f51c441c3f99367488ed822bda2b40836690d5d0059f5",
+                "sha256:7f63877c87552992894ea1444378b9c3a1d80819880ae226bb30b04789c0828c",
+                "sha256:8923e1c5231549fee78ff9b2914fad25f2e3517572bb34bfaa3aea682a758683",
+                "sha256:8afcd1c2297bc989dceaa0379ba15a6df16da69493635e53431d2d0c30356086",
+                "sha256:8b1cc70e31aacc152a12b39245974c8fccf313187eead559ee5966d50e1b5817",
+                "sha256:8d1f3ea0d1924feb4cf6afb2699259f658a08ac6f8f3a4a806661c2dfcd66db1",
+                "sha256:940570c1a305bac10e8b2bc934b85a7709c649317dd16520471e85660275083a",
+                "sha256:947a8525c0a95ba8dc873191f9017d1b1e3024d4dc757f694e0af3026e34044a",
+                "sha256:9beb03ff6fe509d6455971c2489dceb31687b38781206bcec8e68bdfcf5f1db2",
+                "sha256:9c144405220c5ad3f5deab4c77f3e80d52e83804a6b48b6bed3d81a9a0238e4c",
+                "sha256:a98ae493e4e80b3ded6503ff087a8492db058e9c68de371ac3df78e88360b374",
+                "sha256:aa2ce79f3889720b46e0aaba338148a1069aea55fda2c29e0626b4db20d9fcb7",
+                "sha256:aa5eedfc2461c16a092a2fabc5895f159915f25731740c9152a1b00f4bcf629a",
+                "sha256:ab5d89cfaf71807da93c131bb7a19c3e19eaefd613d14f3bce4e97de830b15df",
+                "sha256:b4829db3737480a9d5bfb1c0320c4ee13736f555f53a056aacc874f140e98f64",
+                "sha256:b52771f05cff7517f7067fef19ffe545b1f05959e440d42247a17cd9bddae11b",
+                "sha256:b8248f19a878c72d8c0a785a2cd45d69432e443c9f10ab924c29adda77b324ae",
+                "sha256:b9809404528a999cf02a400ee5677c81959bc5cb938fdc696b62eb40214e3632",
+                "sha256:c155a1a80c5e7a8fa1d9bb1bf3c8a953532b53ab1196092749bafb9d3a7cbb60",
+                "sha256:c33ce0c665dd325200209340a88438ba7a470bd5f09f7424e520e1a3ff835b52",
+                "sha256:c5adc854764732dbd95a713f2e6c3e914e17f2ccdc331b9ecb777484c31f73b6",
+                "sha256:cb374a2a4dba7c4be0b19dc7b1adc50e6c2c26c3369ac629f50f3c198f3743a4",
+                "sha256:cd00859291658fe1fda48a99559fb34da891c50385b0bfb35b808f98956ef1e7",
+                "sha256:ce3057777a14a9a1399b81eca6a6bfc9612047811234398b84c54aeff6d536ea",
+                "sha256:d0a5a1fdc9f148a8827d55b05425801acebeeefc9e86065c7ac8b8cc740a91ff",
+                "sha256:dad3991f0678facca1a0831ec1ddece2eb4d1dd0f5150acb9440f73a3b863907",
+                "sha256:dc7b7c16a519d924c50876fb152af661a20749dcbf653c8759e715c1a7a95b18",
+                "sha256:dcbb7665a9db9f8d7642171152c45da60e16c4f706191d66a1dc47ec9f820aed",
+                "sha256:df037c01d68d1958dad3463e2881d3638a0d6693483f58ad41001aa53a83fcea",
+                "sha256:f08a7e4d62ea2a45557f561eea87c907222575ca2134180b6974f8ac81e24f06",
+                "sha256:f16cf7e4e1bf88fecf7f41da4061f181a6170e179d956420f84e700fb8a3fd6b",
+                "sha256:f2c53f3af011393ab5ed9ab640fa0876757498aac188f782a0c620e33faa2a3d",
+                "sha256:f320c070dea3f20c11213e56dbbd7294c05743417cde01392148964b7bc2d31a",
+                "sha256:f553a1190ae6cd26e553a79f6b6cfba7b8f304da2071052fa33469da075ea625",
+                "sha256:fc8c7958d14e8270171b3d72792b609c057ec0fa17d507729835b5cff6b7f69a"
             ],
-            "version": "==2021.11.10"
+            "markers": "python_version >= '3.6'",
+            "version": "==2022.3.15"
         },
         "reno": {
             "extras": [
                 "sphinx"
             ],
             "hashes": [
-                "sha256:5c3dbe6ea2f46d4138fb4a596c4e947eb0fa79f06cf9cf7b831d8171960ad534",
-                "sha256:5e77ce1707c7e3e1b0e9e72abe2d32c59af44df00a588601e2e362bad1b0fb41"
+                "sha256:55aae4c84c4849ea9d426c295d281bb5535e6ad54cebdc9f81d8d6511c08786b",
+                "sha256:822f433c7b48c5a4bbd248d4af418eae8856043c2dae777d392cb4c974cbb2e2"
             ],
             "index": "pypi",
-            "version": "==3.4.0"
+            "version": "==3.5.0"
         },
         "requests": {
             "hashes": [
                 "sha256:68d7c56fd5a8999887728ef304a6d12edc7be74f1cfa47714fc8b414525c9a61",
                 "sha256:f22fa1e554c9ddfd16e6e41ac79759e17be9e492b3587efa038054674760e72d"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
@@ -907,23 +969,18 @@
                 "sha256:380606e1d10dc85c3bd47bf5a6095f815ec007be7a8b69c878507068df059e6f",
                 "sha256:968089d4584ad4ad7c171454f0a5c6dac23971e9472521ea3b6d49d610aa6fc0"
             ],
             "version": "==0.9.1"
         },
         "rfc3986": {
             "hashes": [
-                "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
-                "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
+                "sha256:270aaf10d87d0d4e095063c65bf3ddbc6ee3d0b226328ce21e036f946e421835",
+                "sha256:a86d6e1f5b1dc238b218b012df0aa79409667bb209e58da56d0b94704e712a97"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.0.0"
-        },
-        "sanitized-package": {
-            "editable": true,
-            "path": "."
+            "version": "==1.5.0"
         },
         "scandir": {
             "hashes": [
                 "sha256:2586c94e907d99617887daed6c1d102b5ca28f1085f90446554abf1faf73123e",
                 "sha256:2ae41f43797ca0c11591c0c35f2f5875fa99f8797cb1a1fd440497ec0ae4b022",
                 "sha256:2b8e3888b11abb2217a32af0766bc06b65cc4a928d8727828ee68af5a967fa6f",
                 "sha256:2c712840c2e2ee8dfaf36034080108d30060d759c7b73a01a52251cc8989f11f",
@@ -937,27 +994,35 @@
             ],
             "index": "pypi",
             "markers": "python_version > '3.5'",
             "version": "==1.10.0"
         },
         "secretstorage": {
             "hashes": [
-                "sha256:422d82c36172d88d6a0ed5afdec956514b189ddbfb72fefab0c8a1cee4eaf71f",
-                "sha256:fd666c51a6bf200643495a04abb261f83229dcb6fd8472ec393df7ffc8b6f195"
+                "sha256:0a8eb9645b320881c222e827c26f4cfcf55363e8b374a021981ef886657a912f",
+                "sha256:755dc845b6ad76dcbcbc07ea3da75ae54bb1ea529eb72d15f83d26499a5df319"
             ],
             "markers": "sys_platform == 'linux'",
-            "version": "==3.3.1"
+            "version": "==3.3.2"
         },
         "setuptools": {
             "hashes": [
-                "sha256:2404879cda71495fc4d5cbc445ed52fdaddf352b36e40be8dcc63147cb4edabe",
-                "sha256:68eb94073fc486091447fcb0501efd6560a0e5a1839ba249e5ff3c4c93f05f90"
+                "sha256:22c7348c6d2976a52632c67f7ab0cdf40147db7789f9aed18734643fe9cf3373",
+                "sha256:4ce92f1e1f8f01233ee9952c04f6b81d1e02939d6e1b488428154974a4d0783e"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==60.5.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==59.6.0"
+        },
+        "setuptools-scm": {
+            "hashes": [
+                "sha256:6833ac65c6ed9711a4d5d2266f8024cfa07c533a0e55f4c12f6eff280a5a9e30",
+                "sha256:acea13255093849de7ccb11af9e1fb8bde7067783450cee9ef7a93139bddf6d4"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==6.4.2"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -968,19 +1033,19 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:0a8836751a68306b3fe97ecbe44db786f8479c3bf4b80e3a7f5c838657b4698c",
-                "sha256:6a11ea5dd0bdb197f9c2abc2e0ce73e01340464feaece525e64036546d24c851"
+                "sha256:7bf8ca9637a4ee15af412d1a1d9689fec70523a68ca9bb9127c2f3eeb344e2e6",
+                "sha256:ebf612653238bcc8f4359627a9b7ce44ede6fdd75d9d30f68255c7383d3a6226"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==4.3.2"
+            "version": "==4.5.0"
         },
         "sphinx-rtd-theme": {
             "hashes": [
                 "sha256:4d35a56f4508cfee4c4fb604373ede6feae2a306731d533f409ef5c3496fdbd8",
                 "sha256:eec6d497e4c2195fa0e8b2016b337532b8a699a68bcb22a512870e16925c6a5c"
             ],
             "index": "pypi",
@@ -1056,87 +1121,81 @@
                 "sha256:e3069e4be3ead9668e21cb9b074cd948f7b3113fd9c8bba083f48247aab8b11c"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.2.3"
         },
         "tqdm": {
             "hashes": [
-                "sha256:8dd278a422499cd6b727e6ae4061c40b48fce8b76d1ccbf5d34fca9b7f925b0c",
-                "sha256:d359de7217506c9851b7869f3708d8ee53ed70a1b8edbba4dbcb47442592920d"
+                "sha256:40be55d30e200777a307a7585aee69e4eabb46b4ec6a4b4a5f2d9f11e7d5408d",
+                "sha256:74a2cdefe14d11442cedf3ba4e21a3b84ff9a2dbdc6cfae2c34addb2a14a5ea6"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==4.62.3"
+            "version": "==4.64.0"
         },
         "twine": {
             "hashes": [
-                "sha256:087328e9bb405e7ce18527a2dca4042a84c7918658f951110b38bc135acab218",
-                "sha256:4caec0f1ed78dc4c9b83ad537e453d03ce485725f2aea57f1bb3fdde78dae936"
+                "sha256:8efa52658e0ae770686a13b675569328f1fba9837e5de1867bfe5f46a9aefe19",
+                "sha256:d0550fca9dc19f3d5e8eadfce0c227294df0a2a951251a4385797c8a6198b7c8"
             ],
             "index": "pypi",
-            "version": "==3.4.2"
+            "version": "==3.8.0"
         },
         "typed-ast": {
             "hashes": [
-                "sha256:01ae5f73431d21eead5015997ab41afa53aa1fbe252f9da060be5dad2c730ace",
-                "sha256:067a74454df670dcaa4e59349a2e5c81e567d8d65458d480a5b3dfecec08c5ff",
-                "sha256:0fb71b8c643187d7492c1f8352f2c15b4c4af3f6338f21681d3681b3dc31a266",
-                "sha256:1b3ead4a96c9101bef08f9f7d1217c096f31667617b58de957f690c92378b528",
-                "sha256:2068531575a125b87a41802130fa7e29f26c09a2833fea68d9a40cf33902eba6",
-                "sha256:209596a4ec71d990d71d5e0d312ac935d86930e6eecff6ccc7007fe54d703808",
-                "sha256:2c726c276d09fc5c414693a2de063f521052d9ea7c240ce553316f70656c84d4",
-                "sha256:398e44cd480f4d2b7ee8d98385ca104e35c81525dd98c519acff1b79bdaac363",
-                "sha256:52b1eb8c83f178ab787f3a4283f68258525f8d70f778a2f6dd54d3b5e5fb4341",
-                "sha256:5feca99c17af94057417d744607b82dd0a664fd5e4ca98061480fd8b14b18d04",
-                "sha256:7538e495704e2ccda9b234b82423a4038f324f3a10c43bc088a1636180f11a41",
-                "sha256:760ad187b1041a154f0e4d0f6aae3e40fdb51d6de16e5c99aedadd9246450e9e",
-                "sha256:777a26c84bea6cd934422ac2e3b78863a37017618b6e5c08f92ef69853e765d3",
-                "sha256:95431a26309a21874005845c21118c83991c63ea800dd44843e42a916aec5899",
-                "sha256:9ad2c92ec681e02baf81fdfa056fe0d818645efa9af1f1cd5fd6f1bd2bdfd805",
-                "sha256:9c6d1a54552b5330bc657b7ef0eae25d00ba7ffe85d9ea8ae6540d2197a3788c",
-                "sha256:aee0c1256be6c07bd3e1263ff920c325b59849dc95392a05f258bb9b259cf39c",
-                "sha256:af3d4a73793725138d6b334d9d247ce7e5f084d96284ed23f22ee626a7b88e39",
-                "sha256:b36b4f3920103a25e1d5d024d155c504080959582b928e91cb608a65c3a49e1a",
-                "sha256:b9574c6f03f685070d859e75c7f9eeca02d6933273b5e69572e5ff9d5e3931c3",
-                "sha256:bff6ad71c81b3bba8fa35f0f1921fb24ff4476235a6e94a26ada2e54370e6da7",
-                "sha256:c190f0899e9f9f8b6b7863debfb739abcb21a5c054f911ca3596d12b8a4c4c7f",
-                "sha256:c907f561b1e83e93fad565bac5ba9c22d96a54e7ea0267c708bffe863cbe4075",
-                "sha256:cae53c389825d3b46fb37538441f75d6aecc4174f615d048321b716df2757fb0",
-                "sha256:dd4a21253f42b8d2b48410cb31fe501d32f8b9fbeb1f55063ad102fe9c425e40",
-                "sha256:dde816ca9dac1d9c01dd504ea5967821606f02e510438120091b84e852367428",
-                "sha256:f2362f3cb0f3172c42938946dbc5b7843c2a28aec307c49100c8b38764eb6927",
-                "sha256:f328adcfebed9f11301eaedfa48e15bdece9b519fb27e6a8c01aa52a17ec31b3",
-                "sha256:f8afcf15cc511ada719a88e013cec87c11aff7b91f019295eb4530f96fe5ef2f",
-                "sha256:fb1bbeac803adea29cedd70781399c99138358c26d05fcbd23c13016b7f5ec65"
+                "sha256:20d5118e494478ef2d3a2702d964dae830aedd7b4d3b626d003eea526be18718",
+                "sha256:27e46cdd01d6c3a0dd8f728b6a938a6751f7bd324817501c15fb056307f918c6",
+                "sha256:27f25232e2dd0edfe1f019d6bfaaf11e86e657d9bdb7b0956db95f560cceb2b3",
+                "sha256:3042bfc9ca118712c9809201f55355479cfcdc17449f9f8db5e744e9625c6805",
+                "sha256:37e5349d1d5de2f4763d534ccb26809d1c24b180a477659a12c4bde9dd677d74",
+                "sha256:4fff9fdcce59dc61ec1b317bdb319f8f4e6b69ebbe61193ae0a60c5f9333dc49",
+                "sha256:542cd732351ba8235f20faa0fc7398946fe1a57f2cdb289e5497e1e7f48cfedb",
+                "sha256:5dc2c11ae59003d4a26dda637222d9ae924387f96acae9492df663843aefad55",
+                "sha256:8831479695eadc8b5ffed06fdfb3e424adc37962a75925668deeb503f446c0a3",
+                "sha256:8cdf91b0c466a6c43f36c1964772918a2c04cfa83df8001ff32a89e357f8eb06",
+                "sha256:8e0b8528838ffd426fea8d18bde4c73bcb4167218998cc8b9ee0a0f2bfe678a6",
+                "sha256:8ef1d96ad05a291f5c36895d86d1375c0ee70595b90f6bb5f5fdbee749b146db",
+                "sha256:9ad3b48cf2b487be140072fb86feff36801487d4abb7382bb1929aaac80638ea",
+                "sha256:9cc9e1457e1feb06b075c8ef8aeb046a28ec351b1958b42c7c31c989c841403a",
+                "sha256:9e237e74fd321a55c90eee9bc5d44be976979ad38a29bbd734148295c1ce7617",
+                "sha256:c9f1a27592fac87daa4e3f16538713d705599b0a27dfe25518b80b6b017f0a6d",
+                "sha256:d64dabc6336ddc10373922a146fa2256043b3b43e61f28961caec2a5207c56d5",
+                "sha256:e20d196815eeffb3d76b75223e8ffed124e65ee62097e4e73afb5fec6b993e7a",
+                "sha256:e34f9b9e61333ecb0f7d79c21c28aa5cd63bec15cb7e1310d7d3da6ce886bc9b",
+                "sha256:ed44e81517364cb5ba367e4f68fca01fba42a7a4690d40c07886586ac267d9b9",
+                "sha256:ee852185964744987609b40aee1d2eb81502ae63ee8eef614558f96a56c1902d",
+                "sha256:f60d9de0d087454c91b3999a296d0c4558c1666771e3460621875021bf899af9",
+                "sha256:f818c5b81966d4728fec14caa338e30a70dfc3da577984d38f97816c4b3071ec",
+                "sha256:fd5df1313915dbd70eaaa88c19030b441742e8b05e6103c631c83b75e0435ccc"
             ],
             "index": "pypi",
-            "version": "==1.4.3"
+            "version": "==1.5.3"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:4ca091dea149f945ec56afb48dae714f21e8692ef22a395223bcd328961b6a0e",
-                "sha256:7f001e5ac290a0c0401508864c7ec868be4e701886d5b573a9528ed3973d9d3b"
+                "sha256:1a9462dcc3347a79b1f1c0271fbe79e844580bb598bafa1ed208b94da3cdcd42",
+                "sha256:21c85e0fe4b9a155d0799430b0ad741cdce7e359660ccbd8b530613e8df88ce2"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==4.0.1"
+            "version": "==4.1.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:000ca7f471a233c2251c6c7023ee85305721bfdf18621ebff4fd17a8653427ed",
-                "sha256:0e7c33d9a63e7ddfcb86780aac87befc2fbddf46c58dbb487e0855f7ceec283c"
+                "sha256:44ece4d53fb1706f667c9bd1c648f5469a2ec925fcf3a776667042d645472c14",
+                "sha256:aabaf16477806a5e1dd19aa41f8c2b7950dd3c746362d7e3223dbe6de6ac448e"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4.0'",
-            "version": "==1.26.8"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
+            "version": "==1.26.9"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:339f16c4a86b44240ba7223d0f93a7887c3ca04b5f9c8129da7958447d079b09",
-                "sha256:d8458cf8d59d0ea495ad9b34c2599487f8a7772d796f9910858376d1600dd2dd"
+                "sha256:e617f16e25b42eb4f6e74096b9c9e37713cf10bf30168fb4a739f3fa8f898a3a",
+                "sha256:ef589a79795589aada0c1c5b319486797c03b67ac3984c48c669c0e4f50df3a5"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==20.13.0"
+            "version": "==20.14.1"
         },
         "virtualenv-clone": {
             "hashes": [
                 "sha256:418ee935c36152f8f153c79824bb93eaf6f0f7984bae31d3f48f350b9183501a",
                 "sha256:44d5263bceed0bac3e1424d64f798095233b64def1c5689afa43dc3223caf5b0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1147,29 +1206,93 @@
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "wrapt": {
             "hashes": [
-                "sha256:b62ffa81fb85f4332a4f609cab4ac40709470da05643a082ec1eb88e6d9b97d7"
+                "sha256:00108411e0f34c52ce16f81f1d308a571df7784932cc7491d1e94be2ee93374b",
+                "sha256:01f799def9b96a8ec1ef6b9c1bbaf2bbc859b87545efbecc4a78faea13d0e3a0",
+                "sha256:09d16ae7a13cff43660155383a2372b4aa09109c7127aa3f24c3cf99b891c330",
+                "sha256:14e7e2c5f5fca67e9a6d5f753d21f138398cad2b1159913ec9e9a67745f09ba3",
+                "sha256:167e4793dc987f77fd476862d32fa404d42b71f6a85d3b38cbce711dba5e6b68",
+                "sha256:1807054aa7b61ad8d8103b3b30c9764de2e9d0c0978e9d3fc337e4e74bf25faa",
+                "sha256:1f83e9c21cd5275991076b2ba1cd35418af3504667affb4745b48937e214bafe",
+                "sha256:21b1106bff6ece8cb203ef45b4f5778d7226c941c83aaaa1e1f0f4f32cc148cd",
+                "sha256:22626dca56fd7f55a0733e604f1027277eb0f4f3d95ff28f15d27ac25a45f71b",
+                "sha256:23f96134a3aa24cc50614920cc087e22f87439053d886e474638c68c8d15dc80",
+                "sha256:2498762814dd7dd2a1d0248eda2afbc3dd9c11537bc8200a4b21789b6df6cd38",
+                "sha256:28c659878f684365d53cf59dc9a1929ea2eecd7ac65da762be8b1ba193f7e84f",
+                "sha256:2eca15d6b947cfff51ed76b2d60fd172c6ecd418ddab1c5126032d27f74bc350",
+                "sha256:354d9fc6b1e44750e2a67b4b108841f5f5ea08853453ecbf44c81fdc2e0d50bd",
+                "sha256:36a76a7527df8583112b24adc01748cd51a2d14e905b337a6fefa8b96fc708fb",
+                "sha256:3a0a4ca02752ced5f37498827e49c414d694ad7cf451ee850e3ff160f2bee9d3",
+                "sha256:3a71dbd792cc7a3d772ef8cd08d3048593f13d6f40a11f3427c000cf0a5b36a0",
+                "sha256:3a88254881e8a8c4784ecc9cb2249ff757fd94b911d5df9a5984961b96113fff",
+                "sha256:47045ed35481e857918ae78b54891fac0c1d197f22c95778e66302668309336c",
+                "sha256:4775a574e9d84e0212f5b18886cace049a42e13e12009bb0491562a48bb2b758",
+                "sha256:493da1f8b1bb8a623c16552fb4a1e164c0200447eb83d3f68b44315ead3f9036",
+                "sha256:4b847029e2d5e11fd536c9ac3136ddc3f54bc9488a75ef7d040a3900406a91eb",
+                "sha256:59d7d92cee84a547d91267f0fea381c363121d70fe90b12cd88241bd9b0e1763",
+                "sha256:5a0898a640559dec00f3614ffb11d97a2666ee9a2a6bad1259c9facd01a1d4d9",
+                "sha256:5a9a1889cc01ed2ed5f34574c90745fab1dd06ec2eee663e8ebeefe363e8efd7",
+                "sha256:5b835b86bd5a1bdbe257d610eecab07bf685b1af2a7563093e0e69180c1d4af1",
+                "sha256:5f24ca7953f2643d59a9c87d6e272d8adddd4a53bb62b9208f36db408d7aafc7",
+                "sha256:61e1a064906ccba038aa3c4a5a82f6199749efbbb3cef0804ae5c37f550eded0",
+                "sha256:65bf3eb34721bf18b5a021a1ad7aa05947a1767d1aa272b725728014475ea7d5",
+                "sha256:6807bcee549a8cb2f38f73f469703a1d8d5d990815c3004f21ddb68a567385ce",
+                "sha256:68aeefac31c1f73949662ba8affaf9950b9938b712fb9d428fa2a07e40ee57f8",
+                "sha256:6915682f9a9bc4cf2908e83caf5895a685da1fbd20b6d485dafb8e218a338279",
+                "sha256:6d9810d4f697d58fd66039ab959e6d37e63ab377008ef1d63904df25956c7db0",
+                "sha256:729d5e96566f44fccac6c4447ec2332636b4fe273f03da128fff8d5559782b06",
+                "sha256:748df39ed634851350efa87690c2237a678ed794fe9ede3f0d79f071ee042561",
+                "sha256:763a73ab377390e2af26042f685a26787c402390f682443727b847e9496e4a2a",
+                "sha256:8323a43bd9c91f62bb7d4be74cc9ff10090e7ef820e27bfe8815c57e68261311",
+                "sha256:8529b07b49b2d89d6917cfa157d3ea1dfb4d319d51e23030664a827fe5fd2131",
+                "sha256:87fa943e8bbe40c8c1ba4086971a6fefbf75e9991217c55ed1bcb2f1985bd3d4",
+                "sha256:88236b90dda77f0394f878324cfbae05ae6fde8a84d548cfe73a75278d760291",
+                "sha256:891c353e95bb11abb548ca95c8b98050f3620a7378332eb90d6acdef35b401d4",
+                "sha256:89ba3d548ee1e6291a20f3c7380c92f71e358ce8b9e48161401e087e0bc740f8",
+                "sha256:8c6be72eac3c14baa473620e04f74186c5d8f45d80f8f2b4eda6e1d18af808e8",
+                "sha256:9a242871b3d8eecc56d350e5e03ea1854de47b17f040446da0e47dc3e0b9ad4d",
+                "sha256:9a3ff5fb015f6feb78340143584d9f8a0b91b6293d6b5cf4295b3e95d179b88c",
+                "sha256:9a5a544861b21e0e7575b6023adebe7a8c6321127bb1d238eb40d99803a0e8bd",
+                "sha256:9d57677238a0c5411c76097b8b93bdebb02eb845814c90f0b01727527a179e4d",
+                "sha256:9d8c68c4145041b4eeae96239802cfdfd9ef927754a5be3f50505f09f309d8c6",
+                "sha256:9d9fcd06c952efa4b6b95f3d788a819b7f33d11bea377be6b8980c95e7d10775",
+                "sha256:a0057b5435a65b933cbf5d859cd4956624df37b8bf0917c71756e4b3d9958b9e",
+                "sha256:a65bffd24409454b889af33b6c49d0d9bcd1a219b972fba975ac935f17bdf627",
+                "sha256:b0ed6ad6c9640671689c2dbe6244680fe8b897c08fd1fab2228429b66c518e5e",
+                "sha256:b21650fa6907e523869e0396c5bd591cc326e5c1dd594dcdccac089561cacfb8",
+                "sha256:b3f7e671fb19734c872566e57ce7fc235fa953d7c181bb4ef138e17d607dc8a1",
+                "sha256:b77159d9862374da213f741af0c361720200ab7ad21b9f12556e0eb95912cd48",
+                "sha256:bb36fbb48b22985d13a6b496ea5fb9bb2a076fea943831643836c9f6febbcfdc",
+                "sha256:d066ffc5ed0be00cd0352c95800a519cf9e4b5dd34a028d301bdc7177c72daf3",
+                "sha256:d332eecf307fca852d02b63f35a7872de32d5ba8b4ec32da82f45df986b39ff6",
+                "sha256:d808a5a5411982a09fef6b49aac62986274ab050e9d3e9817ad65b2791ed1425",
+                "sha256:d9bdfa74d369256e4218000a629978590fd7cb6cf6893251dad13d051090436d",
+                "sha256:db6a0ddc1282ceb9032e41853e659c9b638789be38e5b8ad7498caac00231c23",
+                "sha256:debaf04f813ada978d7d16c7dfa16f3c9c2ec9adf4656efdc4defdf841fc2f0c",
+                "sha256:f0408e2dbad9e82b4c960274214af533f856a199c9274bd4aff55d4634dedc33",
+                "sha256:f2f3bc7cd9c9fcd39143f11342eb5963317bd54ecc98e3650ca22704b69d9653"
             ],
-            "version": "==1.12.1"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==1.14.0"
         },
         "yapf": {
             "hashes": [
-                "sha256:408fb9a2b254c302f49db83c59f9aa0b4b0fd0ec25be3a5c51181327922ff63d",
-                "sha256:e3a234ba8455fe201eaa649cdac872d590089a18b661e39bbac7020978dd9c2e"
+                "sha256:8fea849025584e486fd06d6ba2bed717f396080fd3cc236ba10cb97c4c51cf32",
+                "sha256:a3f5085d37ef7e3e004c4ba9f9b3e40c54ff1901cd111f05145ae313a7c67d1b"
             ],
             "index": "pypi",
-            "version": "==0.31.0"
+            "version": "==0.32.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:9f50f446828eb9d45b267433fd3e9da8d801f614129124863f9c51ebceafb87d",
-                "sha256:b47250dd24f92b7dd6a0a8fc5244da14608f3ca90a5efcd37a3b1642fac9a375"
+                "sha256:71c644c5369f4a6e07636f0aa966270449561fcea2e3d6747b8d23efaa9d7832",
+                "sha256:9fe5ea21568a0a70e50f273397638d39b03353731e6cbbb3fd8502a33fec40bc"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.7.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==3.6.0"
         }
     }
 }
```

### Comparing `guake-3.8.5.dev0/README.rst` & `guake-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/docs/Makefile` & `guake-3.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/docs/make.bat` & `guake-3.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/docs/source/conf.py` & `guake-3.9.0/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import os
-import sys
-
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration ------------------------------------------------
 
@@ -254,21 +251,7 @@
 #texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 #texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 #texinfo_no_detailmenu = False
-
-# html_theme_options = {
-#     'canonical_url': 'http://guake.readthedocs.io/en/latest/',
-#     'logo_only': False,
-#     'display_version': True,
-#     'prev_next_buttons_location': 'bottom',
-#     'style_external_links': False,
-#     'vcs_pageview_mode': '',
-#     # Toc options
-#     'collapse_navigation': True,
-#     'sticky_navigation': True,
-#     'navigation_depth': 4,
-#     'titles_only': False
-# }
```

### Comparing `guake-3.8.5.dev0/docs/source/contributing/basic.rst` & `guake-3.9.0/docs/source/contributing/basic.rst`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/docs/source/contributing/dev_env.rst` & `guake-3.9.0/docs/source/contributing/dev_env.rst`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/docs/source/contributing/hacking.rst` & `guake-3.9.0/docs/source/contributing/hacking.rst`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/docs/source/contributing/packaging.rst` & `guake-3.9.0/docs/source/contributing/packaging.rst`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/docs/source/index.rst` & `guake-3.9.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/docs/source/user/faq.rst` & `guake-3.9.0/docs/source/user/faq.rst`

 * *Files 11% similar despite different names*

```diff
@@ -42,26 +42,26 @@
 (the default for Ubuntu is ``/usr/local/lib/python3.x/dist-packages/guake``).
 
 So on Ubuntu the following commands are equivalent:
 
 .. code-block:: bash
 
     $ sudo make install
-    $ sudo make install PREFIX=/usr/lobal
+    $ sudo make install PREFIX=/usr/local
 
 On Archlinux this can be done by passing ``/usr`` as ``PREFIX``:
 
 .. code-block:: bash
 
     $ sudo make install PREFIX=/usr
 
-which will changes the installation destination to ``/usr/lib/python3.x/site-packages/guake``.
+which changes the installation destination to ``/usr/lib/python3.x/site-packages/guake``.
 
-Note that the install script automatically determines to use whether to use
-``dist-packages`` or ``site-packaes``.
+Note that the install script automatically determines whether to use
+``dist-packages`` or ``site-packages``.
 
 For more details checkout the official PKGBUILD at
 `archlinux.org <https://www.archlinux.org/packages/community/any/guake/>`_, the PKGBUILD on
 the `aur <http://aur.archlinux.org/packages/guake-git>`_ or this
 `gist <https://gist.github.com/aichingm/ed35ba3b136be4424b1ac947207dbca3>`_.
 
 Why Guake crashes with Tmux and Byubu?
```

### Comparing `guake-3.8.5.dev0/docs/source/user/features.rst` & `guake-3.9.0/docs/source/user/features.rst`

 * *Files 8% similar despite different names*

```diff
@@ -110,7 +110,15 @@
 
 Tab UUID
 ========
 
 Tabs are uniquely identified with a UUID. Each terminal receives this UUID in the following
 environment varialbe: ``GUAKE_TAB_UUID``. It can be used to rename the tab from the command line
 using ``--tab-index 3c542bc1-7c99-4e73-8d37-e08281bd592c``.
+
+
+Per-directory `.guake.yml` file
+=============================
+
+If there is a file named `.guake.yml` in the current working directory of the shell associated with a tab, Guake will try to read the title from there. The current format is very simple and it will probably change in the future::
+
+    title: "My Great Project"
```

### Comparing `guake-3.8.5.dev0/docs/source/user/gtk3.rst` & `guake-3.9.0/docs/source/user/gtk3.rst`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/docs/source/user/installing.rst` & `guake-3.9.0/docs/source/user/installing.rst`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/docs/source/user/whatisguake.rst` & `guake-3.9.0/docs/source/user/whatisguake.rst`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/__init__.py` & `guake-3.9.0/guake/__init__.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/about.py` & `guake-3.9.0/guake/about.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,18 +35,14 @@
     """The About Guake dialog class"""
 
     def __init__(self):
         super().__init__(gladefile("about.glade"), root="aboutdialog")
         dialog = self.get_widget("aboutdialog")
 
         # images
-        # ipath = pixmapfile('guake-notification.png')
-        # img = gtk.gdk.pixbuf_new_from_file(ipath)
-
-        # img = pixmapfile('guake-notification.png')
         image = Gtk.Image()
         image.set_from_file(pixmapfile("guake-notification.png"))
         pixbuf = image.get_pixbuf()
 
         dialog.set_property("logo", pixbuf)
 
         dialog.set_name(_("Guake Terminal"))
```

### Comparing `guake-3.8.5.dev0/guake/boxes.py` & `guake-3.9.0/guake/boxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,17 +253,17 @@
                     break
 
                 # Waiting for UI update..
                 while Gtk.events_pending():
                     Gtk.main_iteration()
 
             if cur["type"].endswith("v"):
-                box = box.split_v()
+                box = box.split_v_no_save()
             else:
-                box = box.split_h()
+                box = box.split_h_no_save()
             self.restore_box_layout(box.get_child1(), panes)
             self.restore_box_layout(box.get_child2(), panes)
         else:
             if box.terminal:
                 term = box.terminal
                 # Remove signal handler from terminal
                 for i in term.handler_ids:
@@ -408,15 +408,15 @@
         self.pack_start(self.terminal, True, True, 0)
         self.terminal.show()
         self.add_scroll_bar()
 
     def add_scroll_bar(self):
         """Packs the scrollbar."""
         adj = self.terminal.get_vadjustment()
-        self.scroll = Gtk.VScrollbar(adj)
+        self.scroll = Gtk.Scrollbar.new(Gtk.Orientation.VERTICAL, adj)
         self.scroll.show()
         self.pack_start(self.scroll, False, False, 0)
 
         self.terminal.handler_ids.append(
             self.terminal.connect("scroll-event", self.__scroll_event_cb)
         )
 
@@ -458,15 +458,25 @@
 
     def split_h(self):
         return self.split(DualTerminalBox.ORIENT_V)
 
     def split_v(self):
         return self.split(DualTerminalBox.ORIENT_H)
 
+    def split_h_no_save(self):
+        return self.split_no_save(DualTerminalBox.ORIENT_V)
+
+    def split_v_no_save(self):
+        return self.split_no_save(DualTerminalBox.ORIENT_H)
+
+    @save_tabs_when_changed
     def split(self, orientation):
+        self.split_no_save(orientation)
+
+    def split_no_save(self, orientation):
         notebook = self.get_notebook()
         parent = self.get_parent()  # RootTerminalBox
 
         if orientation == DualTerminalBox.ORIENT_H:
             position = self.get_allocation().width / 2
         else:
             position = self.get_allocation().height / 2
@@ -477,14 +487,18 @@
         dual_terminal_box = DualTerminalBox(orientation)
         dual_terminal_box.set_position(position)
         parent.replace_child(self, dual_terminal_box)
         dual_terminal_box.set_child_first(self)
         dual_terminal_box.set_child_second(terminal_box)
         terminal_box.show()
         dual_terminal_box.show()
+        if self.terminal is not None:
+            # preserve font and font_scale in the new terminal
+            terminal.set_font(self.terminal.font)
+            terminal.font_scale = self.terminal.font_scale
         notebook.terminal_attached(terminal)
 
         return dual_terminal_box
 
     def get_guake(self):
         return self.get_parent().get_guake()
 
@@ -609,14 +623,15 @@
             try:
                 next(box.iter_terminals()).grab_focus()
             except StopIteration:
                 log.error("Both panes are empty")
         else:
             box.get_terminal().grab_focus()
 
+    @save_tabs_when_changed
     def remove_dead_child(self, child):
         if self.get_child1() is child:
             living_child = self.get_child2()
             self.remove(living_child)
             self.get_parent().replace_child(self, living_child)
             self.grab_box_terminal_focus(living_child)
         elif self.get_child2() is child:
@@ -628,16 +643,16 @@
             print("I have never seen this widget!")
 
 
 class TabLabelEventBox(Gtk.EventBox):
     def __init__(self, notebook, text, settings):
         super().__init__()
         self.notebook = notebook
-        self.box = Gtk.Box(Gtk.Orientation.HORIZONTAL, 0, visible=True)
-        self.label = Gtk.Label(text, visible=True)
+        self.box = Gtk.Box(homogeneous=Gtk.Orientation.HORIZONTAL, spacing=0, visible=True)
+        self.label = Gtk.Label(label=text, visible=True)
         self.close_button = Gtk.Button(
             image=Gtk.Image.new_from_icon_name("window-close", Gtk.IconSize.MENU),
             relief=Gtk.ReliefStyle.NONE,
         )
         self.close_button.connect("clicked", self.on_close)
         settings.general.bind(
             "tab-close-buttons", self.close_button, "visible", Gio.SettingsBindFlags.GET
```

### Comparing `guake-3.8.5.dev0/guake/callbacks.py` & `guake-3.9.0/guake/callbacks.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/common.py` & `guake-3.9.0/guake/common.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/customcommands.py` & `guake-3.9.0/guake/customcommands.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/about.glade` & `guake-3.9.0/guake/data/about.glade`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/autostart-guake.desktop` & `guake-3.9.0/guake/data/autostart-guake.desktop`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/guake.desktop.metainfo.xml` & `guake-3.9.0/guake/data/guake.desktop.metainfo.xml`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/guake.glade` & `guake-3.9.0/guake/data/guake.glade`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/org.guake.gschema.xml` & `guake-3.9.0/guake/data/org.guake.gschema.xml`

 * *Files 2% similar despite different names*

#### Comparing `guake-3.8.5.dev0/guake/data/org.guake.gschema.xml` & `guake-3.9.0/guake/data/org.guake.gschema.xml`

```diff
@@ -42,14 +42,19 @@
       <description>If true, when guake restored the tabs, it will notify the user that the tabs has been restored</description>
     </key>
     <key name="save-tabs-when-changed" type="b">
       <default>true</default>
       <summary>Automatically save tabs session when changed</summary>
       <description>If true, when tabs has changed (add / delete ...etc.), it will automatically saved the tabs session</description>
     </key>
+    <key name="load-guake-yml" type="b">
+      <default>true</default>
+      <summary>Load settings from guake.yml</summary>
+      <description>If true, when a change in the cwd is detected settings are changed based on the content of the file `cwd`/.guake.yml</description>
+    </key>
     <key name="use-login-shell" type="b">
       <default>false</default>
       <summary>Login shell</summary>
       <description>If true, the commands in terminal will be executed in a login shell.</description>
     </key>
     <key name="use-trayicon" type="b">
       <default>true</default>
@@ -85,15 +90,15 @@
       <default>false</default>
       <summary>Refocus window.</summary>
       <description>Refocus window instead of closing.</description>
     </key>
     <key name="tab-ontop" type="b">
       <default>false</default>
       <summary>Tab on top.</summary>
-      <description>Makes tab bar on top of the Guake window. Per default, tabs appears bellow the terminal. Setting this to True will move the tab on top of the terminal. Requires a restart.</description>
+      <description>Makes tab bar on top of the Guake window. Per default, tabs appear below the terminal. Setting this to True will move the tab on top of the terminal. Requires a restart.</description>
     </key>
     <key name="new-tab-after" type="b">
       <default>false</default>
       <summary>New tabs appear after the current tab.</summary>
       <description>Makes new tabs appear after the currently selected tab, instead of at the end.</description>
     </key>
     <key name="window-losefocus" type="b">
@@ -235,15 +240,15 @@
       <default>false</default>
       <summary>Set window title to current tab name</summary>
       <description>If true, Guake will update its window title from the current tab name. It is useful when you work with applications that use windows title, (keepass, automatic time tracker apps)</description>
     </key>
     <key name="compat-backspace" type="s">
       <default>'ascii-delete'</default>
       <summary>Backspace Compatibility</summary>
-      <description>Defines the behavior of backscape key.</description>
+      <description>Defines the behavior of backspace key.</description>
     </key>
     <key name="compat-delete" type="s">
       <default>'delete-sequence'</default>
       <summary>Delete Compatibility</summary>
       <description>Defines the behavior of delete key.</description>
     </key>
     <key name="word-chars" type="s">
@@ -260,15 +265,15 @@
       <default>true</default>
       <summary>Give focus to guake if tab is opened (OBSOLETE).</summary>
       <description>If the guake window is out of focus but open, enabling this will give it back the focus instead of closing the window.</description>
     </key>
     <key name="custom-command-file" type="s">
       <default>'~/.config/guake/custom_command.json'</default>
       <summary>Path to the default custom command json file.</summary>
-      <description>Path to the default custom command json file. If is blank or the json file is not in a proper format the terminal context menu will be built without custom commands. If the file is a valid json with recognized structure theterminak context menu will be buit with the commands read inside.</description>
+      <description>Path to the default custom command json file. If is blank or the json file is not in a proper format the terminal context menu will be built without custom commands. If the file is a valid json with recognized structure theterminak context menu will be built with the commands read inside.</description>
     </key>
     <key name="open-tab-cwd" type="b">
       <default>true</default>
       <summary>Open new tab in the current working directory</summary>
       <description>Open new tab in the current working directory</description>
     </key>
     <key name="max-tab-name-length" type="i">
@@ -409,14 +414,19 @@
       <description>Accelerator to active function that closes the current selected tab.</description>
     </key>
     <key name="search-on-web" type="s">
       <default>'&lt;Control&gt;&lt;Shift&gt;l'</default>
       <summary>Search current selected text on the web</summary>
       <description>Accelerator to active function that search on the web the current selected text on the terminal.</description>
     </key>
+    <key name="open-link-under-terminal-cursor" type="s">
+      <default>'&lt;Control&gt;&lt;Shift&gt;o'</default>
+      <summary>Open link under terminal cursor</summary>
+      <description>Accelerator to active function that opens the link (URL) under the current terminal cursor.</description>
+    </key>
     <key name="move-tab-left" type="s">
       <default>'&lt;Control&gt;&lt;Shift&gt;Page_Up'</default>
       <summary>Move left current tab</summary>
       <description>Move the current tab to the left</description>
     </key>
     <key name="move-tab-right" type="s">
       <default>'&lt;Control&gt;&lt;Shift&gt;Page_Down'</default>
@@ -520,20 +530,20 @@
     </key>
     <key name="decrease-height" type="s">
       <default>'&lt;Control&gt;Up'</default>
       <summary>Decrease height.</summary>
       <description>Decrease the screen height.</description>
     </key>
     <key name="increase-transparency" type="s">
-      <default>'&lt;Control&gt;&lt;Shift&gt;Up'</default>
+      <default>'&lt;Control&gt;&lt;Shift&gt;b'</default>
       <summary>Increase transparency.</summary>
       <description>Increase the terminal transparency.</description>
     </key>
     <key name="decrease-transparency" type="s">
-      <default>'&lt;Control&gt;&lt;Shift&gt;Down'</default>
+      <default>'&lt;Control&gt;&lt;Shift&gt;n'</default>
       <summary>Decrease transparency.</summary>
       <description>Decrease the terminal transparency.</description>
     </key>
     <key name="clipboard-copy" type="s">
       <default>'&lt;Control&gt;&lt;Shift&gt;c'</default>
       <summary>Copy clipboard.</summary>
       <description>Copy the clipboard content.</description>
```

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/add_tab.png` & `guake-3.9.0/guake/data/pixmaps/add_tab.png`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/guake-128.png` & `guake-3.9.0/guake/data/pixmaps/guake-128.png`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/guake-48.png` & `guake-3.9.0/guake/data/pixmaps/guake-48.png`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/guake-64.png` & `guake-3.9.0/guake/data/pixmaps/guake-64.png`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/guake-notification.png` & `guake-3.9.0/guake/data/pixmaps/guake-notification.png`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/guake-tray.png` & `guake-3.9.0/guake/data/pixmaps/guake-tray.png`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/guake-tray.svg` & `guake-3.9.0/guake/data/pixmaps/guake-tray.svg`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/guake.png` & `guake-3.9.0/guake/data/pixmaps/guake.png`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/intro-large.jpg` & `guake-3.9.0/guake/data/pixmaps/intro-large.jpg`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/intro-medium.jpg` & `guake-3.9.0/guake/data/pixmaps/intro-medium.jpg`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/intro-small.jpg` & `guake-3.9.0/guake/data/pixmaps/intro-small.jpg`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/quick-open-python-exception.png` & `guake-3.9.0/guake/data/pixmaps/quick-open-python-exception.png`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/quick-open-selection.png` & `guake-3.9.0/guake/data/pixmaps/quick-open-selection.png`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/quick-open.png` & `guake-3.9.0/guake/data/pixmaps/quick-open.png`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/screenshot-fullscreen.jpg` & `guake-3.9.0/guake/data/pixmaps/screenshot-fullscreen.jpg`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/pixmaps/screenshot-small.jpg` & `guake-3.9.0/guake/data/pixmaps/screenshot-small.jpg`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/data/prefs.glade` & `guake-3.9.0/guake/data/prefs.glade`

 * *Files 0% similar despite different names*

#### Comparing `guake-3.8.5.dev0/guake/data/prefs.glade` & `guake-3.9.0/guake/data/prefs.glade`

```diff
@@ -267,15 +267,26 @@
                                           </object>
                                           <packing>
                                             <property name="left-attach">0</property>
                                             <property name="top-attach">2</property>
                                           </packing>
                                         </child>
                                         <child>
-                                          <placeholder/>
+                                          <object class="GtkCheckButton" id="load-guake-yml">
+                                            <property name="label" translatable="yes">Load settings from `cwd`/.guake.yml</property>
+                                            <property name="visible">True</property>
+                                            <property name="can-focus">True</property>
+                                            <property name="receives-default">False</property>
+                                            <property name="draw-indicator">True</property>
+                                            <signal name="toggled" handler="on_load_guake_yml_toggled" swapped="no"/>
+                                          </object>
+                                          <packing>
+                                            <property name="left-attach">0</property>
+                                            <property name="top-attach">3</property>
+                                          </packing>
                                         </child>
                                         <child>
                                           <placeholder/>
                                         </child>
                                         <child>
                                           <placeholder/>
                                         </child>
```

### Comparing `guake-3.8.5.dev0/guake/data/search.glade` & `guake-3.9.0/guake/data/search.glade`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/dbusiface.py` & `guake-3.9.0/guake/dbusiface.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,14 +149,19 @@
         self.guake.set_colors_from_settings_on_page()
 
     @dbus.service.method(DBUS_NAME)
     def reset_colors_current(self):
         self.guake.reset_terminal_custom_colors(current_terminal=True)
         self.guake.set_colors_from_settings_on_page(current_terminal_only=True)
 
+    @dbus.service.method(DBUS_NAME, in_signature="s")
+    def execute_command(self, command):
+        self.guake.add_tab()
+        self.guake.execute_command(command)
+
     @dbus.service.method(DBUS_NAME, in_signature="i", out_signature="s")
     def get_tab_name(self, tab_index=0):
         return self.guake.get_notebook().get_tab_text_index(tab_index)
 
     @dbus.service.method(DBUS_NAME, in_signature="ss")
     def rename_tab_uuid(self, tab_uuid, new_text):
         self.guake.rename_tab_uuid(tab_uuid, new_text, True)
@@ -192,7 +197,11 @@
     @dbus.service.method(DBUS_NAME)
     def v_split_current_terminal(self):
         self.guake.get_notebook().get_current_terminal().get_parent().split_v()
 
     @dbus.service.method(DBUS_NAME)
     def h_split_current_terminal(self):
         self.guake.get_notebook().get_current_terminal().get_parent().split_h()
+
+    @dbus.service.method(DBUS_NAME, in_signature="s", out_signature="i")
+    def get_index_from_uuid(self, tab_uuid):
+        return self.guake.get_index_from_uuid(tab_uuid)
```

### Comparing `guake-3.8.5.dev0/guake/dialogs.py` & `guake-3.9.0/guake/dialogs.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/globals.py` & `guake-3.9.0/guake/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     (
         "Python pytest report",
         r"^\s.*\:\:[a-zA-Z0-9\_]+\s",
         r"^\s*(.*\:\:[a-zA-Z0-9\_]+)\s",
     ),
     (
         "line starts by 'ERROR in Filename:line' pattern (GCC/make). File path should exists.",
-        r"\s.\S[^\s\s].[a-zA-Z0-9\/\_\-\.\ ]+\.?[a-zA-Z0-9]+\:[0-9]+",
+        r"[a-zA-Z0-9\/\_\-\.\]+\.?[a-zA-Z0-9]+\:[0-9]+",
         r"\s.\S[^\s\s].(.*)\:([0-9]+)",
     ),
     (
         "line starts by 'Filename:line' pattern (GCC/make). File path should exists.",
         r"^\s*[a-zA-Z0-9\/\_\-\.\ ]+\.?[a-zA-Z0-9]+\:[0-9]+",
         r"^\s*(.*)\:([0-9]+)",
     ),
```

### Comparing `guake-3.8.5.dev0/guake/gsettings.py` & `guake-3.9.0/guake/gsettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         """If the gconf var use_default_font be changed, this method
         will be called and will change the font style to the gnome
         default or to the chosen font in style/font/style in all
         terminals open.
         """
         font_name = None
         if settings.get_boolean(key):
-            gio_settings = Gio.Settings("org.gnome.desktop.interface")
+            gio_settings = Gio.Settings(schema="org.gnome.desktop.interface")
             font_name = gio_settings.get_string("monospace-font-name")
         else:
             font_name = self.settings.styleFont.get_string("style")
         if not font_name:
             log.error("Error: unable to find font name (%s)", font_name)
             return
         font = Pango.FontDescription(font_name)
@@ -374,15 +374,15 @@
         if terminal_uuid:
             terminal = self.guake.notebook_manager.get_terminal_by_uuid(terminal_uuid)
             terminals = (terminal,) if terminal else ()
         else:
             terminals = self.guake.notebook_manager.iter_terminals()
 
         if self.settings.general.get_boolean("use-default-font"):
-            gio_settings = Gio.Settings("org.gnome.desktop.interface")
+            gio_settings = Gio.Settings(schema="org.gnome.desktop.interface")
             font_name = gio_settings.get_string("monospace-font-name")
         else:
             font_name = settings.get_string(key)
 
         font = Pango.FontDescription(font_name)
         for i in terminals:
             i.set_font(font)
```

### Comparing `guake-3.8.5.dev0/guake/guake_app.py` & `guake-3.9.0/guake/guake_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 import gi
 
 gi.require_version("Gtk", "3.0")
 gi.require_version("Gdk", "3.0")
 gi.require_version("Keybinder", "3.0")
 from gi.repository import GLib
-from gi.repository import GObject
 from gi.repository import Gdk
 from gi.repository import Gio
 from gi.repository import Gtk
 from gi.repository import Keybinder
 
 from guake import gtk_version
 from guake import guake_version
@@ -66,14 +65,15 @@
 from guake.prefs import PrefsDialog
 from guake.prefs import refresh_user_start
 from guake.settings import Settings
 from guake.simplegladeapp import SimpleGladeApp
 from guake.theme import patch_gtk_theme
 from guake.theme import select_gtk_theme
 from guake.utils import BackgroundImageManager
+from guake.utils import FileManager
 from guake.utils import FullscreenManager
 from guake.utils import HidePrevention
 from guake.utils import RectCalculator
 from guake.utils import TabNameUtils
 from guake.utils import get_server_time
 from guake.utils import save_tabs_when_changed
 
@@ -82,18 +82,16 @@
 instance = None
 RESPONSE_FORWARD = 0
 RESPONSE_BACKWARD = 1
 
 # Disable find feature until python-vte hasn't been updated
 enable_find = False
 
-GObject.threads_init()
-
 # Setting gobject program name
-GObject.set_prgname(NAME)
+GLib.set_prgname(NAME)
 
 GDK_WINDOW_STATE_WITHDRAWN = 1
 GDK_WINDOW_STATE_ICONIFIED = 2
 GDK_WINDOW_STATE_STICKY = 8
 GDK_WINDOW_STATE_ABOVE = 32
 
 
@@ -169,14 +167,16 @@
             show = Gtk.MenuItem(_("Show"))
             show.set_sensitive(True)
             show.connect("activate", self.show_hide)
             show.show()
             menu.prepend(show)
             self.tray_icon.set_menu(menu)
 
+        self.display_tab_names = 0
+
         # important widgets
         self.window = self.get_widget("window-root")
         self.window.set_name("guake-terminal")
         self.window.set_keep_above(True)
         self.mainframe = self.get_widget("mainframe")
         self.mainframe.remove(self.get_widget("notebook-teminals"))
 
@@ -187,14 +187,17 @@
 
         # BackgroundImageManager
         self.background_image_manager = BackgroundImageManager(self.window)
 
         # FullscreenManager
         self.fullscreen_manager = FullscreenManager(self.settings, self.window, self)
 
+        # Start the file manager (only used by guake.yml so far).
+        self.fm = FileManager()
+
         # Workspace tracking
         self.notebook_manager = NotebookManager(
             self.window,
             self.mainframe,
             self.settings.general.get_boolean("workspace-specific-tab-sets"),
             self.terminal_spawned,
             self.page_deleted,
@@ -218,16 +221,14 @@
 
         # Controls the transparency state needed for function accel_toggle_transparency
         self.transparency_toggled = False
 
         # store the default window title to reset it when update is not wanted
         self.default_window_title = self.window.get_title()
 
-        self.display_tab_names = 0
-
         self.window.connect("focus-out-event", self.on_window_losefocus)
         self.window.connect("focus-in-event", self.on_window_takefocus)
 
         # Handling the delete-event of the main window to avoid
         # problems when closing it.
         def destroy(*args):
             self.hide()
@@ -304,15 +305,15 @@
             self.window.set_app_paintable(True)
             self.window.transparency = True
             self.window.realize()
             if self.window.get_property("visible"):
                 self.hide()
                 self.show()
         else:
-            log.warn("System doesn't support transparency")
+            log.warning("System doesn't support transparency")
             self.window.transparency = False
             self.window.set_visual(screen.get_system_visual())
 
     # new color methods should be moved to the GuakeTerminal class
 
     def _load_palette(self):
         colorRGBA = Gdk.RGBA(0, 0, 0, 0)
@@ -1098,29 +1099,54 @@
 
         # TODO NOTEBOOK this code only works if there is only one terminal in a
         # page, this need to be rewritten
         for terminal in self.get_notebook().iter_terminals():
             page_num = self.get_notebook().page_num(terminal.get_parent())
             self.get_notebook().rename_page(page_num, self.compute_tab_title(terminal), False)
 
+    def load_cwd_guake_yaml(self, vte) -> dict:
+        # Read the content of .guake.yml in cwd
+        if not self.settings.general.get_boolean("load-guake-yml"):
+            return {}
+
+        cwd = Path(vte.get_current_directory())
+        filename = str(cwd.joinpath(".guake.yml"))
+
+        try:
+            content = self.fm.read_yaml(filename)
+        except Exception:
+            log.debug("Unexpected error reading %s.", filename, exc_info=True)
+            content = {}
+
+        if not isinstance(content, dict):
+            content = {}
+        return content
+
     def compute_tab_title(self, vte):
         """Compute the tab title"""
+
+        guake_yml = self.load_cwd_guake_yaml(vte)
+
+        if "title" in guake_yml:
+            return guake_yml["title"]
+
         vte_title = vte.get_window_title() or _("Terminal")
         try:
             current_directory = vte.get_current_directory()
             if self.display_tab_names == 1 and vte_title.endswith(current_directory):
                 parts = current_directory.split("/")
                 parts = [s[:1] for s in parts[:-1]] + [parts[-1]]
                 vte_title = vte_title[: len(vte_title) - len(current_directory)] + "/".join(parts)
             if self.display_tab_names == 2:
                 vte_title = current_directory.split("/")[-1]
                 if not vte_title:
                     vte_title = "(root)"
         except OSError:
             pass
+
         return TabNameUtils.shorten(vte_title, self.settings)
 
     def check_if_terminal_directory_changed(self, term):
         @save_tabs_when_changed
         def terminal_directory_changed(self):
             # Yep, just used for save tabs when changed
             pass
@@ -1147,14 +1173,15 @@
         # this may return -1, should be checked ;)
         nb = self.get_notebook()
         page_num = nb.page_num(box)
         for nb in self.notebook_manager.iter_notebooks():
             page_num = nb.page_num(box)
             if page_num != -1:
                 break
+
         # if tab has been renamed by user, don't override.
         if not getattr(box, "custom_label_set", False):
             title = self.compute_tab_title(vte)
             nb.rename_page(page_num, title, False)
             self.update_window_title(title)
         else:
             text = nb.get_tab_text_page(box)
@@ -1182,14 +1209,21 @@
         (page_index,) = (
             index
             for index, t in enumerate(self.get_notebook().iter_terminals())
             if t.get_uuid() == term_uuid
         )
         self.get_notebook().rename_page(page_index, new_text, user_set)
 
+    def get_index_from_uuid(self, term_uuid):
+        term_uuid = uuid.UUID(term_uuid)
+        for index, t in enumerate(self.get_notebook().iter_terminals()):
+            if t.get_uuid() == term_uuid:
+                return index
+        return -1
+
     def rename_current_tab(self, new_text, user_set=False):
         page_num = self.get_notebook().get_current_page()
         self.get_notebook().rename_page(page_num, new_text, user_set)
 
     def terminal_spawned(self, notebook, terminal, pid):
         self.load_config(terminal_uuid=terminal.uuid)
         terminal.handler_ids.append(
@@ -1275,27 +1309,33 @@
     def get_selected_uuidtab(self):
         # TODO DBUS ONLY
         """Returns the uuid of the current selected terminal"""
         page_num = self.get_notebook().get_current_page()
         terminals = self.get_notebook().get_terminals_for_page(page_num)
         return str(terminals[0].get_uuid())
 
+    def open_link_under_terminal_cursor(self, *args):
+        current_term = self.get_notebook().get_current_terminal()
+        if current_term is None:
+            return
+        url = current_term.get_link_under_terminal_cursor()
+        current_term.browse_link_under_cursor(url)
+
     def search_on_web(self, *args):
         """Search for the selected text on the web"""
         # TODO KEYBINDINGS ONLY
         current_term = self.get_notebook().get_current_terminal()
 
         if current_term.get_has_selection():
             current_term.copy_clipboard()
             guake_clipboard = Gtk.Clipboard.get_default(self.window.get_display())
             search_query = guake_clipboard.wait_for_text()
             search_query = quote_plus(search_query)
             if search_query:
-                # TODO: search provider should be selectable (someone might
-                # prefer bing.com, the internet is a strange place ¯\_(ツ)_/¯ )
+                # TODO: search provider should be selectable.
                 search_url = f"https://www.google.com/search?q={search_query}&safe=off"
                 Gtk.show_uri(self.window.get_screen(), search_url, get_server_time(self.window))
         return True
 
     def set_tab_position(self, *args):
         if self.settings.general.get_boolean("tab-ontop"):
             self.get_notebook().set_tab_pos(Gtk.PositionType.TOP)
@@ -1437,15 +1477,15 @@
 
                 # Restore each frames' tabs from config
                 # NOTE: If frame implement in future, we will need to update this code
                 for tabs in frames:
                     for index, tab in enumerate(tabs):
                         if tab.get("panes", False):
                             box, page_num, term = nb.new_page_with_focus(
-                                label=tab["label"], empty=True
+                                label=tab["label"], user_set=tab["custom_label_set"], empty=True
                             )
                             box.restore_box_layout(box.child, tab["panes"])
                         else:
                             directory = (
                                 tab["panes"][0]["directory"]
                                 if len(tab.get("panes", [])) == 1
                                 else tab.get("directory", None)
```

### Comparing `guake-3.8.5.dev0/guake/guake_logging.py` & `guake-3.9.0/guake/guake_logging.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/keybindings.py` & `guake-3.9.0/guake/keybindings.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,21 +13,23 @@
 General Public License for more details.
 
 You should have received a copy of the GNU General Public
 License along with this program; if not, write to the
 Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor,
 Boston, MA 02110-1301 USA
 """
-from collections import defaultdict
 import logging
 
+from collections import defaultdict
+
 import gi
 
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
+from gi.repository import Gdk
 
 from guake import notifier
 from guake.common import pixmapfile
 from guake.split_utils import FocusMover
 from guake.split_utils import SplitMover
 
 log = logging.getLogger(__name__)
@@ -41,14 +43,15 @@
         """Constructor of Keyboard, only receives the guake instance
         to be used in internal methods.
         """
         self.guake = guake
         self.accel_group = None  # see reload_accelerators
         self._lookup = None
         self._masks = None
+        self.keymap = Gdk.Keymap.get_for_display(Gdk.Display.get_default())
 
         # Setup global keys
         self.globalhotkeys = {}
         globalkeys = ["show-hide", "show-focus"]
         for key in globalkeys:
             guake.settings.keybindingsGlobal.onChangedValue(key, self.reload_global)
             guake.settings.keybindingsGlobal.triggerOnChangedValue(
@@ -78,14 +81,15 @@
             ("zoom-out", self.guake.accel_zoom_out),
             ("increase-height", self.guake.accel_increase_height),
             ("decrease-height", self.guake.accel_decrease_height),
             ("increase-transparency", self.guake.accel_increase_transparency),
             ("decrease-transparency", self.guake.accel_decrease_transparency),
             ("toggle-transparency", self.guake.accel_toggle_transparency),
             ("search-on-web", self.guake.search_on_web),
+            ("open-link-under-terminal-cursor", self.guake.open_link_under_terminal_cursor),
             ("move-tab-left", self.guake.accel_move_tab_left),
             ("move-tab-right", self.guake.accel_move_tab_right),
             ("switch-tab1", self.guake.gen_accel_switch_tabN(0)),
             ("switch-tab2", self.guake.gen_accel_switch_tabN(1)),
             ("switch-tab3", self.guake.gen_accel_switch_tabN(2)),
             ("switch-tab4", self.guake.gen_accel_switch_tabN(3)),
             ("switch-tab5", self.guake.gen_accel_switch_tabN(4)),
@@ -219,22 +223,41 @@
                         "Please use Guake Preferences dialog to choose another "
                         "key"
                     )
                     % label,
                     filename,
                 )
         elif key == "show-focus" and not self.guake.hotkeys.bind(value, self.guake.show_focus):
-            log.warn("can't bind show-focus key")
+            log.warning("can't bind show-focus key")
 
     def activate(self, window, event):
         """If keystroke matches a key binding, activate keybinding. Otherwise, allow
         keystroke to pass through."""
-        key = event.hardware_keycode
+        key = event.keyval
         mod = event.state
 
+        # Set keyval to the first available English keyboard value if character is non-latin
+        # and a english keyval is found
+        if event.keyval > 126:
+            for i in self.keymap.get_entries_for_keycode(event.hardware_keycode)[2]:
+                if 0 < i <= 126:
+                    key = i
+                    break
+
+        if mod & Gdk.ModifierType.SHIFT_MASK:
+            if key == Gdk.KEY_ISO_Left_Tab:
+                key = Gdk.KEY_Tab
+            else:
+                key = Gdk.keyval_to_lower(key)
+        else:
+            keys = Gdk.keyval_convert_case(key)
+            if key != keys[1]:
+                key = keys[0]
+                mod &= ~Gdk.ModifierType.SHIFT_MASK
+
         mask = mod & self._masks
 
         func = self._lookup[mask].get(key, None)
         if func:
             func()
             return True
 
@@ -250,14 +273,15 @@
         self.load_accelerators()
         self.guake.accel_group = self
 
     def load_accelerators(self):
         """Reads all gconf paths under /apps/guake/keybindings/local
         and adds to the _lookup.
         """
+
         for binding, action in self.keys:
-            key, keycodes, mask = Gtk.accelerator_parse_with_keycode(
+            key, mask = Gtk.accelerator_parse(
                 self.guake.settings.keybindingsLocal.get_string(binding)
             )
-            if keycodes and keycodes[0]:
-                self._lookup[mask][keycodes[0]] = action
+            if key > 0:
+                self._lookup[mask][key] = action
                 self._masks |= mask
```

### Comparing `guake-3.8.5.dev0/guake/main.py` & `guake-3.9.0/guake/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     """Parses the command line parameters and decide if dbus methods
     should be called or not. If there is already a guake instance
     running it will be used and a True value will be returned,
     otherwise, false will be returned.
     """
     # Force to xterm-256 colors for compatibility with some old command line programs
     os.environ["TERM"] = "xterm-256color"
+    os.environ["TERM_PROGRAM"] = "guake"
 
     # do not use version keywords here, pbr might be slow to find the version of Guake module
     parser = OptionParser()
     parser.add_option(
         "-V",
         "--version",
         dest="version",
@@ -188,14 +189,23 @@
         dest="selected_tab",
         action="store_true",
         default=False,
         help=_("Return the selected tab index."),
     )
 
     parser.add_option(
+        "-x",
+        "--uuid-index",
+        dest="uuid_index",
+        action="store",
+        default="",
+        help=_("Return the index of the tab with the given terminal UUID, -1 if not found"),
+    )
+
+    parser.add_option(
         "-l",
         "--selected-tablabel",
         dest="selected_tablabel",
         action="store_true",
         default=False,
         help=_("Return the selected tab label."),
     )
@@ -239,15 +249,15 @@
 
     parser.add_option(
         "-e",
         "--execute-command",
         dest="command",
         action="store",
         default="",
-        help=_("Execute an arbitrary command in the selected tab."),
+        help=_("Execute an arbitrary command in a new tab."),
     )
 
     parser.add_option(
         "-i",
         "--tab-index",
         dest="tab_index",
         action="store",
@@ -522,14 +532,19 @@
         only_show_hide = options.show
 
     if options.selected_tablabel:
         selectedlabel = remote_object.get_selected_tablabel()
         sys.stdout.write(f"{selectedlabel}\n")
         only_show_hide = options.show
 
+    if options.uuid_index:
+        selectedIndex = remote_object.get_index_from_uuid(options.uuid_index)
+        sys.stdout.write(f"{selectedIndex}\n")
+        only_show_hide = options.show
+
     if options.split_vertical:
         remote_object.v_split_current_terminal()
         only_show_hide = options.show
 
     if options.split_horizontal:
         remote_object.h_split_current_terminal()
         only_show_hide = options.show
@@ -608,23 +623,23 @@
         remote_object.show_hide()
 
     if options.execute_startup_script:
         if not already_running:
             startup_script = instance.settings.general.get_string("startup-script")
             if startup_script:
                 log.info("Calling startup script: %s", startup_script)
-                with subprocess.Popen(
+                pid = subprocess.Popen(  # pylint: disable=consider-using-with
                     [startup_script],
-                    shell=True,
+                    shell=False,
                     stdin=None,
                     stdout=None,
                     stderr=None,
                     close_fds=True,
-                ) as pid:
-                    log.info("Startup script started with pid: %s", pid)
+                )
+                log.info("Startup script started with pid: %s", pid)
                 # Please ensure this is the last line !!!!
     else:
         log.info("--no-startup-script argument defined, so don't execute the startup script")
     if already_running:
         log.info("Guake is already running")
     return already_running
```

### Comparing `guake-3.8.5.dev0/guake/menus.py` & `guake-3.9.0/guake/menus.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/notebook.py` & `guake-3.9.0/guake/notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,22 +64,22 @@
         self.set_property("is-focus", True)
         self.set_property("expand", True)
 
         if GObject.signal_lookup("terminal-spawned", TerminalNotebook) == 0:
             GObject.signal_new(
                 "terminal-spawned",
                 TerminalNotebook,
-                GObject.SIGNAL_RUN_LAST,
+                GObject.SignalFlags.RUN_LAST,
                 GObject.TYPE_NONE,
                 (GObject.TYPE_PYOBJECT, GObject.TYPE_INT),
             )
             GObject.signal_new(
                 "page-deleted",
                 TerminalNotebook,
-                GObject.SIGNAL_RUN_LAST,
+                GObject.SignalFlags.RUN_LAST,
                 GObject.TYPE_NONE,
                 (),
             )
 
         self.scroll_callback = NotebookScrollCallback(self)
         self.add_events(Gdk.EventMask.SCROLL_MASK)
         self.connect("scroll-event", self.scroll_callback.on_scroll)
@@ -411,15 +411,15 @@
 
     def new_page_with_focus(
         self, directory=None, label=None, user_set=False, position=None, empty=False
     ):
         box, page_num, terminal = self.new_page(directory, position=position, empty=empty)
         self.set_current_page(page_num)
         if not label:
-            self.rename_page(page_num, _("Terminal"), False)
+            self.rename_page(page_num, self.guake.compute_tab_title(terminal), False)
         else:
             self.rename_page(page_num, label, user_set)
         if terminal is not None:
             terminal.grab_focus()
         return box, page_num, terminal
 
     def rename_page(self, page_index, new_text, user_set=False):
@@ -507,15 +507,15 @@
         page_deleted_cb,
     ):
         GObject.Object.__init__(self)
         if not GObject.signal_lookup("notebook-created", self):
             GObject.signal_new(
                 "notebook-created",
                 self,
-                GObject.SIGNAL_RUN_LAST,
+                GObject.SignalFlags.RUN_LAST,
                 GObject.TYPE_NONE,
                 (GObject.TYPE_PYOBJECT, GObject.TYPE_INT),
             )
         self.current_notebook = 0
         self.notebooks = {}
         self.window = window
         self.notebook_parent = notebook_parent
```

### Comparing `guake-3.8.5.dev0/guake/notifier.py` & `guake-3.9.0/guake/notifier.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/palettes.py` & `guake-3.9.0/guake/palettes.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/paths.py` & `guake-3.9.0/guake/paths.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/prefs.py` & `guake-3.9.0/guake/prefs.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,14 +182,18 @@
         ],
     },
     {
         "label": _("Extra features"),
         "key": "extra",
         "keys": [
             {"key": "search-on-web", "label": _("Search selected text on web")},
+            {
+                "key": "open-link-under-terminal-cursor",
+                "label": _("Open URL under terminal cursor"),
+            },
         ],
     },
 ]
 
 html_escape_table = {
     "&": "&amp;",
     '"': "&quot;",
@@ -243,14 +247,18 @@
         """Changes the activity of restore-tabs-notify in dconf"""
         self.settings.general.set_boolean("restore-tabs-notify", chk.get_active())
 
     def on_save_tabs_when_changed_toggled(self, chk):
         """Changes the activity of save-tabs-when-changed in dconf"""
         self.settings.general.set_boolean("save-tabs-when-changed", chk.get_active())
 
+    def on_load_guake_yml_toggled(self, chk):
+        """Changes the activity of load-guake-yml"""
+        self.settings.general.set_boolean("load-guake-yml", chk.get_active())
+
     def on_default_shell_changed(self, combo):
         """Changes the activity of default_shell in dconf"""
         citer = combo.get_active_iter()
         if not citer:
             return
         shell = combo.get_model().get_value(citer, 0)
         # we unset the value (restore to default) when user chooses to use
@@ -1004,14 +1012,18 @@
         value = self.settings.general.get_boolean("restore-tabs-notify")
         self.get_widget("restore-tabs-notify").set_active(value)
 
         # save tabs when changed
         value = self.settings.general.get_boolean("save-tabs-when-changed")
         self.get_widget("save-tabs-when-changed").set_active(value)
 
+        # save tabs when changed
+        value = self.settings.general.get_boolean("load-guake-yml")
+        self.get_widget("load-guake-yml").set_active(value)
+
         # login shell
         value = self.settings.general.get_boolean("use-login-shell")
         self.get_widget("use_login_shell").set_active(value)
 
         # tray icon
         value = self.settings.general.get_boolean("use-trayicon")
         self.get_widget("use_trayicon").set_active(value)
```

### Comparing `guake-3.8.5.dev0/guake/settings.py` & `guake-3.9.0/guake/settings.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/simplegladeapp.py` & `guake-3.9.0/guake/simplegladeapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,14 @@
 
         if root:
             self.main_widget = self.builder.get_object(root)
             self.main_widget.show_all()
         else:
             self.main_widget = None
 
-        # self.glade = self.create_glade(self.glade_path, root, domain)
-
         self.normalize_names()
         # Widgets are loaded and can be refered as self.widget_name
 
     def __repr__(self):
         class_name = self.__class__.__name__
         if self.main_widget:
             root = Gtk.Widget.get_name(self.main_widget)
```

### Comparing `guake-3.8.5.dev0/guake/split_utils.py` & `guake-3.9.0/guake/split_utils.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/support.py` & `guake-3.9.0/guake/support.py`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/guake/terminal.py` & `guake-3.9.0/guake/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,14 @@
         self.handler_ids = []
         self.handler_ids.append(self.connect("button-press-event", self.button_press))
         self.connect("child-exited", self.on_child_exited)  # Call on_child_exited, don't remove it
         self.connect("selection-changed", self.copy_on_select)
         self.matched_value = ""
         self.font_scale_index = 0
         self._pid = None
-        # self.custom_bgcolor = None
-        # self.custom_fgcolor = None
         self.found_link = None
         self.uuid = uuid.uuid4()
 
         # Custom colors
         self.custom_bgcolor = None
         self.custom_fgcolor = None
         self.custom_palette = None
@@ -226,21 +224,21 @@
             # reference from vte/bindings/vala/app.vala, flags = 0x40080400u
             # also ref: https://mail.gnome.org/archives/commits-list/2016-September/msg06218.html
             VTE_REGEX_FLAGS = 0x40080400
             for expr in TERMINAL_MATCH_EXPRS:
                 tag = self.match_add_regex(
                     Vte.Regex.new_for_match(expr, len(expr), VTE_REGEX_FLAGS), 0
                 )
-                self.match_set_cursor_type(tag, Gdk.CursorType.HAND2)
+                self.match_set_cursor_name(tag, "hand")
 
             for _useless, match, _otheruseless in QUICK_OPEN_MATCHERS:
                 tag = self.match_add_regex(
                     Vte.Regex.new_for_match(match, len(match), VTE_REGEX_FLAGS), 0
                 )
-                self.match_set_cursor_type(tag, Gdk.CursorType.HAND2)
+                self.match_set_cursor_name(tag, "hand")
         except (
             GLib.Error,
             AttributeError,
         ):  # pylint: disable=catching-non-exception
             try:
                 compile_flag = 0
                 if (Vte.MAJOR_VERSION, Vte.MINOR_VERSION) >= (0, 44):
@@ -309,16 +307,14 @@
                 # "<File>::<python_function>"
                 m = re.compile(r"^(.*)\:\:([a-zA-Z0-9\_]+)$").match(text)
                 if m:
                     text = m.group(1)
                     py_func = m.group(2).strip()
 
         def find_lineno(text, pt, lineno, py_func):
-            # print("text={!r}, pt={!r}, lineno={!r}, py_func={!r}".format(text,
-            #                                                              pt, lineno, py_func))
             if lineno:
                 return lineno
             if not py_func:
                 return
             with pt.open() as f:
                 for i, line in enumerate(f.readlines()):
                     if line.startswith(f"def {py_func}"):
@@ -474,29 +470,37 @@
                 value = f"ftp://{value}"
             elif TERMINAL_MATCH_TAGS[tag] == "email":
                 value = f"mailto:{value}"
 
         if value:
             return value
 
+    def get_link_under_terminal_cursor(self):
+        cursor_position = self.get_cursor_position()
+        matched_string = self.match_check(cursor_position.column, cursor_position.row)
+        link = self.handleTerminalMatch(matched_string)
+        if link:
+            return link
+
     def get_link_under_cursor(self):
         return self.found_link
 
-    def browse_link_under_cursor(self):
+    def browse_link_under_cursor(self, url=None):
         # TODO move the call to xdg-open to guake.utils
-        if not self.found_link:
+        if not self.found_link and url is None:
             return
-        log.debug("Opening link: %s", self.found_link)
-        cmd = ["xdg-open", self.found_link]
+        url = url if url is not None else self.found_link
+        log.debug("Opening link: %s", url)
+        cmd = ["xdg-open", url]
         with subprocess.Popen(cmd, shell=False):
             pass
 
     def set_font(self, font):
         self.font = font
-        self.set_font_scale_index(0)
+        self.set_font_scale_index(self.font_scale)
 
     def set_font_scale_index(self, scale_index):
         self.font_scale_index = clamp(scale_index, -6, 12)
 
         font = Pango.FontDescription(self.font.to_string())
         scale_factor = 2 ** (self.font_scale_index / 6)
         new_size = int(scale_factor * font.get_size())
@@ -515,15 +519,14 @@
 
     def decrease_font_size(self):
         self.font_scale -= 1
 
     def kill(self):
         pid = self.pid
         threading.Thread(target=self.delete_shell, args=(pid,)).start()
-        # start_new_thread(self.delete_shell, (pid,))
 
     def delete_shell(self, pid):
         """Kill the shell with SIGHUP
 
         NOTE: Leave it alone, DO NOT USE os.waitpid
 
         > sys:1: Warning: GChildWatchSource: Exit status of a child process was requested but
```

### Comparing `guake-3.8.5.dev0/guake/utils.py` & `guake-3.9.0/guake/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 You should have received a copy of the GNU General Public
 License along with this program; if not, write to the
 Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor,
 Boston, MA 02110-1301 USA
 """
 import enum
 import logging
+import os
 import subprocess
 import time
-import os
+import yaml
 
 import cairo
 
 import gi
 
 gi.require_version("Gtk", "3.0")
 gi.require_version("Gdk", "3.0")
@@ -35,15 +36,14 @@
 from gi.repository import Gdk
 from gi.repository import Gtk
 from guake.globals import ALIGN_BOTTOM
 from guake.globals import ALIGN_CENTER
 from guake.globals import ALIGN_LEFT
 from guake.globals import ALIGN_RIGHT
 from guake.globals import ALIGN_TOP
-from guake.globals import ALWAYS_ON_PRIMARY
 
 try:
     from gi.repository import GdkX11
 except ImportError:
     GdkX11 = False
 
 log = logging.getLogger(__name__)
@@ -67,31 +67,31 @@
 
 
 # Decorator for save-tabs-when-changed
 def save_tabs_when_changed(func):
     """Decorator for save-tabs-when-changed"""
 
     def wrapper(*args, **kwargs):
-        func(*args, **kwargs)
-        log.debug("mom, I've been called: %s %s", func.__name__, func)
-
         # Find me the Guake!
         clsname = args[0].__class__.__name__
         g = None
         if clsname == "Guake":
             g = args[0]
         elif getattr(args[0], "get_guake", None):
             g = args[0].get_guake()
         elif getattr(args[0], "get_notebook", None):
             g = args[0].get_notebook().guake
         elif getattr(args[0], "guake", None):
             g = args[0].guake
         elif getattr(args[0], "notebook", None):
             g = args[0].notebook.guake
 
+        func(*args, **kwargs)
+        log.debug("mom, I've been called: %s %s", func.__name__, func)
+
         # Tada!
         if g and g.settings.general.get_boolean("save-tabs-when-changed"):
             g.save_tabs()
 
     return wrapper
 
 
@@ -106,14 +106,54 @@
     # XXX: Hardcode?
     with open(filename, "rb") as f:
         prefs = f.read()
     with subprocess.Popen(["dconf", "load", "/apps/guake/"], stdin=subprocess.PIPE) as p:
         p.communicate(input=prefs)
 
 
+class FileManager:
+    def __init__(self, delta=1.0):
+        self._cache = {}
+        self._delta = max(0.0, delta)
+
+    def clear(self):
+        self._cache.clear()
+
+    def read_yaml(self, filename: str):
+
+        content = None
+
+        try:
+            content = self.read(filename)
+        except PermissionError:
+            log.debug("PermissionError while reading %s.", filename)
+        except FileNotFoundError:
+            log.debug("File %s does not exists.", filename)
+        except UnicodeDecodeError:
+            log.debug("Encoding error %s (we assume is utf-8).", filename)
+
+        if content is not None:
+            try:
+                content = yaml.safe_load(content)
+            except yaml.YAMLError:
+                log.debug("YAMLError reading %s.", filename)
+                content = None
+        return content
+
+    def read(self, filename: str) -> str:
+        # Return the content of a file from the fs or from cache.
+        if (
+            filename not in self._cache
+            or self._cache[filename]["time"] + self._delta < time.monotonic()
+        ):
+            with open(filename, mode="r", encoding="utf-8") as fd:
+                self._cache[filename] = {"time": time.monotonic(), "content": fd.read()}
+        return self._cache[filename]["content"]
+
+
 class TabNameUtils:
     @classmethod
     def shorten(cls, text, settings):
         use_vte_titles = settings.general.get_boolean("use-vte-titles")
         if not use_vte_titles:
             return text
         max_name_length = settings.general.get_int("max-tab-name-length")
@@ -226,17 +266,16 @@
         log.debug("  width_percents = %s", width_percents)
         log.debug("  halignment = %s", halignment)
         log.debug("  valignment = %s", valignment)
         log.debug("  hdisplacement = %s", hdisplacement)
         log.debug("  vdisplacement = %s", vdisplacement)
 
         # get the rectangle just from the destination monitor
-        screen = window.get_screen()
         monitor = cls.get_final_window_monitor(settings, window)
-        window_rect = screen.get_monitor_geometry(monitor)
+        window_rect = monitor.get_workarea()
         log.debug("Current monitor geometry")
         log.debug("  window_rect.x: %s", window_rect.x)
         log.debug("  window_rect.y: %s", window_rect.y)
         log.debug("  window_rect.height: %s", window_rect.height)
         log.debug("  window_rect.width: %s", window_rect.width)
 
         total_height = window_rect.height
@@ -281,42 +320,37 @@
             window.move(window_rect.x, window_rect.y)
             log.debug("Updated window position: %r", window.get_position())
 
         return window_rect
 
     @classmethod
     def get_final_window_monitor(cls, settings, window):
-        """Gets the final screen number for the main window of guake."""
+        """Gets the final monitor for the main window of guake."""
 
-        screen = window.get_screen()
+        display = window.get_display()
 
         # fetch settings
         use_mouse = settings.general.get_boolean("mouse-display")
-        dest_screen = settings.general.get_int("display-n")
+        num_monitor = settings.general.get_int("display-n")
 
         if use_mouse:
+            pointer = display.get_default_seat().get_pointer()
+            if pointer is None:
+                monitor = display.get_primary_monitor()
+            else:
+                _, x, y = pointer.get_position()
+                monitor = display.get_monitor_at_point(x, y)
+        else:
+            monitor = display.get_monitor(num_monitor)
+            if monitor is None:
+                # monitor not found or num_monitor is wrong
+                # by default we use the primary monitor
+                monitor = display.get_primary_monitor()
 
-            # TODO PORT get_pointer is deprecated
-            # https://developer.gnome.org/gtk3/stable/GtkWidget.html#gtk-widget-get-pointer
-            win, x, y, _ = screen.get_root_window().get_pointer()
-            dest_screen = screen.get_monitor_at_point(x, y)
-
-        # If Guake is configured to use a screen that is not currently attached,
-        # default to 'primary display' option.
-        n_screens = screen.get_n_monitors()
-        if dest_screen > n_screens - 1:
-            settings.general.set_boolean("mouse-display", False)
-            settings.general.set_int("display-n", dest_screen)
-            dest_screen = screen.get_primary_monitor()
-
-        # Use primary display if configured
-        if dest_screen == ALWAYS_ON_PRIMARY:
-            dest_screen = screen.get_primary_monitor()
-
-        return dest_screen
+        return monitor
 
 
 class ImageLayoutMode(enum.IntEnum):
     SCALE = 0
     TILE = 1
     CENTER = 2
     STRETCH = 3
@@ -417,15 +451,17 @@
     def draw(self, widget, cr):
         if not self.bg_surface:
             return
 
         # Step 1. Get target surface
         #         (paint background image into widget size surface by layout mode)
         surface = self.render_target(
-            widget.get_allocated_width(), widget.get_allocated_height(), self.layout_mode
+            widget.get_allocated_width(),
+            widget.get_allocated_height(),
+            self.layout_mode,
         )
 
         cr.save()
         # Step 2. Paint target surface to context (in our case, the RootTerminalBox)
         #
         #         At this step, RootTerminalBox will be painted to our background image,
         #         and all the draw done by VTE has been overlapped.
@@ -436,15 +472,17 @@
         # Step 3. Re-paint child draw result to a new surface
         #
         #         We need to re-paint what we overlapped in previous step,
         #         so we paint our child (again, in lifecycle view) into a similar surface.
         #
         child = widget.get_child()
         child_surface = cr.get_target().create_similar(
-            cairo.CONTENT_COLOR_ALPHA, child.get_allocated_width(), child.get_allocated_height()
+            cairo.CONTENT_COLOR_ALPHA,
+            child.get_allocated_width(),
+            child.get_allocated_height(),
         )
         child_cr = cairo.Context(child_surface)
 
         # Re-paint child draw into child context (which using child_surface as target)
         widget.propagate_draw(child, child_cr)
 
         # Step 3.1 Re-paint search revealer
```

### Comparing `guake-3.8.5.dev0/guake.egg-info/PKG-INFO` & `guake-3.9.0/guake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guake
-Version: 3.8.5.dev0
+Version: 3.9.0
 Summary: Guake Terminal
 Home-page: https://github.com/Guake/guake
 Author: Gaetan Semet
 Author-email: gaetan@xeberon.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
```

### Comparing `guake-3.8.5.dev0/guake.egg-info/SOURCES.txt` & `guake-3.9.0/guake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/ca.mo` & `guake-3.9.0/po/ca.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/ca.po` & `guake-3.9.0/po/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -1628,14 +1628,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "S'ha produït un error en definir la drecera de teclat"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "No s'ha pogut enllaçar la tecla global <b>%s</b>."
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/cs.mo` & `guake-3.9.0/po/cs.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/cs.po` & `guake-3.9.0/po/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -1612,14 +1612,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "chyba klávesových zkratek"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "Nelze nastavit globální <b>%s</b> klávesu"
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/de.mo` & `guake-3.9.0/po/de.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/de.po` & `guake-3.9.0/po/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -1395,7 +1395,24 @@
 #: guake/data/prefs.glade:2135
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
+
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
```

### Comparing `guake-3.8.5.dev0/po/el.mo` & `guake-3.9.0/po/el.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/el.po` & `guake-3.9.0/po/el.po`

 * *Files 0% similar despite different names*

```diff
@@ -1562,14 +1562,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "σφάλμα συντόμευσης πληκτρολογίου"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "Αδυναμία καθολικής σύνδεσης του πλήκτρου \"%s\""
 
 #, fuzzy
```

### Comparing `guake-3.8.5.dev0/po/es.mo` & `guake-3.9.0/po/es.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/es.po` & `guake-3.9.0/po/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -1632,14 +1632,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "Error al asignar tecla"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "No se pudo asignar la tecla %s"
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/fa.mo` & `guake-3.9.0/po/fa.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/fa.po` & `guake-3.9.0/po/fa.po`

 * *Files 2% similar despite different names*

```diff
@@ -1561,14 +1561,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "خطا در باگزاری کلید"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "نمی‌توان کلید <b>%s</b> را بارگزاری کرد"
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/fi.mo` & `guake-3.9.0/po/fi.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/fi.po` & `guake-3.9.0/po/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -1656,7 +1656,24 @@
 #: guake/data/prefs.glade:2135
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
+
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
```

### Comparing `guake-3.8.5.dev0/po/fr.mo` & `guake-3.9.0/po/fr.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/fr.po` & `guake-3.9.0/po/fr.po`

 * *Files 0% similar despite different names*

```diff
@@ -1304,14 +1304,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "Show support infomations"
 #~ msgstr "Afficher les informations pour le support"
 
 #~ msgid "Use workspace-specific tab sets (requires restart)"
 #~ msgstr "Utiliser les bureaux virtuels pour les onglets (redémarrage requis)"
 
 #~ msgid ""
```

### Comparing `guake-3.8.5.dev0/po/gl.mo` & `guake-3.9.0/po/gl.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/gl.po` & `guake-3.9.0/po/gl.po`

 * *Files 1% similar despite different names*

```diff
@@ -1576,14 +1576,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "erro de combinación de teclas"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "Non foi posíbel combinar a clave global <b>%s</b> "
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/hr.mo` & `guake-3.9.0/po/hr.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/hr.po` & `guake-3.9.0/po/hr.po`

 * *Files 0% similar despite different names*

```diff
@@ -1630,14 +1630,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "Greška dodjeljivanja tipke"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "Nemoguće je dodjeliti globalnu <b>%s</b> tipku"
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/hu.mo` & `guake-3.9.0/po/hu.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/hu.po` & `guake-3.9.0/po/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -1577,14 +1577,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "Hiba történt a billentyűkombináció hozzárendelésekor"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "Globális billentyűkombináció hozzárendelése meghiúsult:<b>%s</b>."
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/id.mo` & `guake-3.9.0/po/id.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/id.po` & `guake-3.9.0/po/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -1527,9 +1527,26 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "http://guake.org"
 #~ msgstr "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/it.mo` & `guake-3.9.0/po/it.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/it.po` & `guake-3.9.0/po/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -1595,14 +1595,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "errore di assegnazione tasto"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "Impossibile impostare globalmente il tasto <b>%s</b>"
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/ja.mo` & `guake-3.9.0/po/ja.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/ja.po` & `guake-3.9.0/po/ja.po`

 * *Files 0% similar despite different names*

```diff
@@ -1307,7 +1307,24 @@
 #: guake/data/prefs.glade:2135
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
+
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
```

### Comparing `guake-3.8.5.dev0/po/ko.mo` & `guake-3.9.0/po/ko.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/ko.po` & `guake-3.9.0/po/ko.po`

 * *Files 1% similar despite different names*

```diff
@@ -1559,14 +1559,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "키 바인딩 에러"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "글로벌 키 <b>%s</b> 바인딩을 실패했습니다."
 
 #~ msgid "<b>Quick Open configuration</b>"
```

### Comparing `guake-3.8.5.dev0/po/nb.mo` & `guake-3.9.0/po/nb.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/nb.po` & `guake-3.9.0/po/nb.po`

 * *Files 1% similar despite different names*

```diff
@@ -1679,14 +1679,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "Hurtigtast error"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "Kunne ikke lagre <b>%s</b> tasten"
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/nl.mo` & `guake-3.9.0/po/nl.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/nl.po` & `guake-3.9.0/po/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -1655,14 +1655,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr "Regelhoogte (VTE >= 0.52)"
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr "Regelbreedte (VTE >= 0.52)"
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "Fout bij toets-binding"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "Globale toets <b>%s</b> kan niet worden gebonden"
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/pa.mo` & `guake-3.9.0/po/pa.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/pa.po` & `guake-3.9.0/po/pa.po`

 * *Files 0% similar despite different names*

```diff
@@ -1548,14 +1548,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "ਕੁੰਜੀ ਬਾਈਡਿੰਗ ਗਲਤੀ"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "ਗਲੋਬਲ <b>%s</b> ਕੁੰਜੀ ਬਾਈਡਿੰਗ ਲਈ ਅਸਮਰੱਥ"
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/pl.mo` & `guake-3.9.0/po/pl.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/pl.po` & `guake-3.9.0/po/pl.po`

 * *Files 2% similar despite different names*

```diff
@@ -1380,7 +1380,24 @@
 #: guake/data/prefs.glade:2135
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
+
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
```

### Comparing `guake-3.8.5.dev0/po/pt_BR.mo` & `guake-3.9.0/po/pt_BR.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/pt_BR.po` & `guake-3.9.0/po/pt_BR.po`

 * *Files 0% similar despite different names*

```diff
@@ -1574,14 +1574,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "erro na associação de atalhos"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "Impossível associar a tecla <b>%s</b>"
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/ru.mo` & `guake-3.9.0/po/ru.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/ru.po` & `guake-3.9.0/po/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -1634,14 +1634,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "Path to script executed on Guake start:"
 #~ msgstr "Путь к скрипту, запускаемому при старте Guake:"
 
 #~ msgid "0 means no size limit"
 #~ msgstr "0 - без ограничения размера"
 
 #~ msgid "Custom Commands"
```

### Comparing `guake-3.8.5.dev0/po/sv.mo` & `guake-3.9.0/po/sv.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/sv.po` & `guake-3.9.0/po/sv.po`

 * *Files 0% similar despite different names*

```diff
@@ -1374,7 +1374,24 @@
 #: guake/data/prefs.glade:2135
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr "Linjehöjdskala (VTE >= 0,52)"
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr "Linjebreddskala (VTE >= 0,52)"
+
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
```

### Comparing `guake-3.8.5.dev0/po/tr.mo` & `guake-3.9.0/po/tr.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/tr.po` & `guake-3.9.0/po/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -1630,14 +1630,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr "Satır Yüksekliği Ölçeği (VTE >= 0.52)"
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr "Satır Genişliği Ölçeği (VTE >= 0.52)"
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "kısayol atama hatası"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "Genel <b>%s</b> tuşu atanamadı"
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/uk.mo` & `guake-3.9.0/po/uk.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/uk.po` & `guake-3.9.0/po/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -1539,14 +1539,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "key binding error"
 #~ msgstr "не вдалося створити прив’язку клавіш"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
 #~ msgstr "Не вийшло створити прив’язку глобальної комбінації клавіш <b>%s</b>"
 
 #~ msgid "http://guake.org"
```

### Comparing `guake-3.8.5.dev0/po/zh_CN.mo` & `guake-3.9.0/po/zh_CN.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/zh_CN.po` & `guake-3.9.0/po/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -1578,14 +1578,31 @@
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
 
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
+
 #~ msgid "0 means no size limit"
 #~ msgstr "0表示没有大小限制"
 
 #~ msgid "key binding error"
 #~ msgstr "键绑定出错"
 
 #~ msgid "Unable to bind global <b>%s</b> key"
```

### Comparing `guake-3.8.5.dev0/po/zh_TW.mo` & `guake-3.9.0/po/zh_TW.mo`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/po/zh_TW.po` & `guake-3.9.0/po/zh_TW.po`

 * *Files 0% similar despite different names*

```diff
@@ -1237,7 +1237,24 @@
 #: guake/data/prefs.glade:2135
 msgid "Line Height Scale (VTE >= 0.52)"
 msgstr ""
 
 #: guake/data/prefs.glade:2172
 msgid "Line Width Scale (VTE >= 0.52)"
 msgstr ""
+
+#: guake/main.py:201
+msgid ""
+"Return the index of the tab with the given terminal UUID, -1 if not found"
+msgstr ""
+
+#: guake/main.py:256
+msgid "Execute an arbitrary command in a new tab."
+msgstr ""
+
+#: guake/prefs.py:191
+msgid "Open URL under terminal cursor"
+msgstr ""
+
+#: guake/data/prefs.glade:275
+msgid "Load settings from `cwd`/.guake.yml"
+msgstr ""
```

### Comparing `guake-3.8.5.dev0/requirements-dev.txt` & `guake-3.9.0/requirements-dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 ################################################################################
 
 -e .
 astroid
 autopep8
 black==21.8b0
 colorlog
-dataclasses
 fiximports>=0.1.18
-flake8
+flake8>=3.8.0,<4.0.0
 flakehell
 mock>=2.0.0
 pathlib2
 pep8
 pew
 pipenv-to-requirements
 pyfakefs
```

### Comparing `guake-3.8.5.dev0/requirements.txt` & `guake-3.9.0/requirements.txt`

 * *Files 26% similar despite different names*

```diff
@@ -7,9 +7,10 @@
 # that do not support `Pipfile` yet.
 #
 # Do NOT edit it directly, use `pipenv install [-d]` to modify `Pipfile` and
 # `Pipfile.lock` and then regenerate `requirements*.txt`.
 ################################################################################
 
 pbr
+pyyaml
 typing ; python_version > '3.5'
 wheel
```

### Comparing `guake-3.8.5.dev0/scripts/bootstrap-dev-arch.sh` & `guake-3.9.0/scripts/bootstrap-dev-arch.sh`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/scripts/bootstrap-dev-debian.sh` & `guake-3.9.0/scripts/bootstrap-dev-debian.sh`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/scripts/bootstrap-dev-fedora.sh` & `guake-3.9.0/scripts/bootstrap-dev-fedora.sh`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/scripts/colortest` & `guake-3.9.0/scripts/colortest`

 * *Files identical despite different names*

### Comparing `guake-3.8.5.dev0/setup.cfg` & `guake-3.9.0/setup.cfg`

 * *Files identical despite different names*

