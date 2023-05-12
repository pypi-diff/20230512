# Comparing `tmp/elm-messenger-0.1.4.tar.gz` & `tmp/elm-messenger-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.1.4.tar", last modified: Tue May  9 06:58:18 2023, max compression
+gzip compressed data, was "elm-messenger-0.1.5.tar", last modified: Fri May 12 15:46:09 2023, max compression
```

## Comparing `elm-messenger-0.1.4.tar` & `elm-messenger-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-09 06:58:18.261228 elm-messenger-0.1.4/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.4/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-09 06:58:18.261228 elm-messenger-0.1.4/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.4/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-09 06:58:18.261228 elm-messenger-0.1.4/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-09 06:58:18.000000 elm-messenger-0.1.4/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      344 2023-05-09 06:58:18.000000 elm-messenger-0.1.4/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-09 06:58:18.000000 elm-messenger-0.1.4/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-09 06:58:18.000000 elm-messenger-0.1.4/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-09 06:58:18.000000 elm-messenger-0.1.4/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-09 06:58:18.000000 elm-messenger-0.1.4/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-09 06:58:18.261228 elm-messenger-0.1.4/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.4/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.4/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)     9308 2023-05-09 01:19:04.000000 elm-messenger-0.1.4/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-09 06:58:18.261228 elm-messenger-0.1.4/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.4/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-12 15:46:09.385113 elm-messenger-0.1.5/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.5/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-12 15:46:09.385113 elm-messenger-0.1.5/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.5/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-12 15:46:09.385113 elm-messenger-0.1.5/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-12 15:46:09.000000 elm-messenger-0.1.5/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2023-05-12 15:46:09.000000 elm-messenger-0.1.5/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-12 15:46:09.000000 elm-messenger-0.1.5/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-12 15:46:09.000000 elm-messenger-0.1.5/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-12 15:46:09.000000 elm-messenger-0.1.5/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-12 15:46:09.000000 elm-messenger-0.1.5/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-12 15:46:09.385113 elm-messenger-0.1.5/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.5/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.5/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    13716 2023-05-12 15:44:18.000000 elm-messenger-0.1.5/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.1.5/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-12 15:46:09.385113 elm-messenger-0.1.5/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.5/setup.py
```

