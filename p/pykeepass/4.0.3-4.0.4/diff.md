# Comparing `tmp/pykeepass-4.0.3.tar.gz` & `tmp/pykeepass-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeepass-4.0.3.tar", last modified: Tue Jun 21 16:20:07 2022, max compression
+gzip compressed data, was "pykeepass-4.0.4.tar", last modified: Fri May 12 06:07:39 2023, max compression
```

## Comparing `pykeepass-4.0.3.tar` & `pykeepass-4.0.4.tar`

### file list

```diff
@@ -1,35 +1,44 @@
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2022-06-21 16:20:07.205303 pykeepass-4.0.3/
--rw-r--r--   0 evan      (1000) evan      (1000)    35147 2021-03-05 05:26:01.000000 pykeepass-4.0.3/LICENSE
--rw-r--r--   0 evan      (1000) evan      (1000)      179 2021-03-05 05:26:01.000000 pykeepass-4.0.3/MANIFEST.in
--rw-r--r--   0 evan      (1000) evan      (1000)    14711 2022-06-21 16:20:07.205303 pykeepass-4.0.3/PKG-INFO
--rw-r--r--   0 evan      (1000) evan      (1000)    14407 2022-06-21 07:18:16.000000 pykeepass-4.0.3/README.rst
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2022-06-21 16:20:07.201302 pykeepass-4.0.3/pykeepass/
--rw-r--r--   0 evan      (1000) evan      (1000)      132 2021-03-15 16:25:40.000000 pykeepass-4.0.3/pykeepass/__init__.py
--rw-r--r--   0 evan      (1000) evan      (1000)     1378 2021-03-05 05:26:01.000000 pykeepass-4.0.3/pykeepass/attachment.py
--rw-r--r--   0 evan      (1000) evan      (1000)     5208 2022-03-29 18:04:43.000000 pykeepass-4.0.3/pykeepass/baseelement.py
--rw-r--r--   0 evan      (1000) evan      (1000)     1365 2021-03-05 05:26:01.000000 pykeepass-4.0.3/pykeepass/blank_database.kdbx
--rw-r--r--   0 evan      (1000) evan      (1000)    10226 2022-06-21 07:07:59.000000 pykeepass-4.0.3/pykeepass/entry.py
--rw-r--r--   0 evan      (1000) evan      (1000)      411 2022-03-18 04:26:05.000000 pykeepass-4.0.3/pykeepass/exceptions.py
--rw-r--r--   0 evan      (1000) evan      (1000)     3142 2022-03-18 04:26:05.000000 pykeepass-4.0.3/pykeepass/group.py
--rw-r--r--   0 evan      (1000) evan      (1000)     1166 2022-03-18 04:26:05.000000 pykeepass-4.0.3/pykeepass/icons.py
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2022-06-21 16:20:07.205303 pykeepass-4.0.3/pykeepass/kdbx_parsing/
--rw-r--r--   0 evan      (1000) evan      (1000)       23 2021-03-05 05:26:01.000000 pykeepass-4.0.3/pykeepass/kdbx_parsing/__init__.py
--rw-r--r--   0 evan      (1000) evan      (1000)    13134 2022-03-18 04:26:05.000000 pykeepass-4.0.3/pykeepass/kdbx_parsing/common.py
--rw-r--r--   0 evan      (1000) evan      (1000)      750 2021-07-23 16:46:01.000000 pykeepass-4.0.3/pykeepass/kdbx_parsing/kdbx.py
--rw-r--r--   0 evan      (1000) evan      (1000)     4922 2022-03-18 04:26:05.000000 pykeepass-4.0.3/pykeepass/kdbx_parsing/kdbx3.py
--rw-r--r--   0 evan      (1000) evan      (1000)     7954 2022-03-29 18:04:43.000000 pykeepass-4.0.3/pykeepass/kdbx_parsing/kdbx4.py
--rw-r--r--   0 evan      (1000) evan      (1000)    15444 2021-03-05 05:26:01.000000 pykeepass-4.0.3/pykeepass/kdbx_parsing/pytwofish.py
--rw-r--r--   0 evan      (1000) evan      (1000)    13307 2021-03-05 05:26:01.000000 pykeepass-4.0.3/pykeepass/kdbx_parsing/twofish.py
--rw-r--r--   0 evan      (1000) evan      (1000)    30710 2022-06-21 07:16:20.000000 pykeepass-4.0.3/pykeepass/pykeepass.py
--rw-r--r--   0 evan      (1000) evan      (1000)      680 2022-02-16 22:22:34.000000 pykeepass-4.0.3/pykeepass/setters.py
--rw-r--r--   0 evan      (1000) evan      (1000)       48 2022-06-21 16:19:16.000000 pykeepass-4.0.3/pykeepass/version.py
--rw-r--r--   0 evan      (1000) evan      (1000)     2848 2022-06-21 06:51:40.000000 pykeepass-4.0.3/pykeepass/xpath.py
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2022-06-21 16:20:07.201302 pykeepass-4.0.3/pykeepass.egg-info/
--rw-r--r--   0 evan      (1000) evan      (1000)    14711 2022-06-21 16:20:07.000000 pykeepass-4.0.3/pykeepass.egg-info/PKG-INFO
--rw-r--r--   0 evan      (1000) evan      (1000)      719 2022-06-21 16:20:07.000000 pykeepass-4.0.3/pykeepass.egg-info/SOURCES.txt
--rw-r--r--   0 evan      (1000) evan      (1000)        1 2022-06-21 16:20:07.000000 pykeepass-4.0.3/pykeepass.egg-info/dependency_links.txt
--rw-r--r--   0 evan      (1000) evan      (1000)       80 2022-06-21 16:20:07.000000 pykeepass-4.0.3/pykeepass.egg-info/requires.txt
--rw-r--r--   0 evan      (1000) evan      (1000)       10 2022-06-21 16:20:07.000000 pykeepass-4.0.3/pykeepass.egg-info/top_level.txt
--rw-r--r--   0 evan      (1000) evan      (1000)      111 2022-03-29 18:04:43.000000 pykeepass-4.0.3/requirements.txt
--rw-r--r--   0 evan      (1000) evan      (1000)       38 2022-06-21 16:20:07.205303 pykeepass-4.0.3/setup.cfg
--rw-r--r--   0 evan      (1000) evan      (1000)      886 2022-03-29 18:04:43.000000 pykeepass-4.0.3/setup.py
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-05-12 06:07:39.699094 pykeepass-4.0.4/
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-05-12 06:07:39.691094 pykeepass-4.0.4/.github/
+-rw-r--r--   0 evan      (1000) evan      (1000)      180 2022-06-27 23:09:55.000000 pykeepass-4.0.4/.github/dependabot.yml
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-05-12 06:07:39.691094 pykeepass-4.0.4/.github/workflows/
+-rw-r--r--   0 evan      (1000) evan      (1000)      725 2022-12-27 21:23:49.000000 pykeepass-4.0.4/.github/workflows/ci.yaml
+-rw-r--r--   0 evan      (1000) evan      (1000)       82 2022-12-26 00:46:40.000000 pykeepass-4.0.4/.gitignore
+-rw-r--r--   0 evan      (1000) evan      (1000)     2511 2023-05-12 06:00:00.000000 pykeepass-4.0.4/CHANGELOG.rst
+-rw-r--r--   0 evan      (1000) evan      (1000)    35147 2021-03-05 05:26:01.000000 pykeepass-4.0.4/LICENSE
+-rw-r--r--   0 evan      (1000) evan      (1000)      179 2021-03-05 05:26:01.000000 pykeepass-4.0.4/MANIFEST.in
+-rw-r--r--   0 evan      (1000) evan      (1000)      317 2022-07-20 18:02:33.000000 pykeepass-4.0.4/Makefile
+-rw-r--r--   0 evan      (1000) evan      (1000)    14903 2023-05-12 06:07:39.699094 pykeepass-4.0.4/PKG-INFO
+-rw-r--r--   0 evan      (1000) evan      (1000)    14582 2023-05-12 06:07:16.000000 pykeepass-4.0.4/README.rst
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-05-12 06:07:39.695094 pykeepass-4.0.4/pykeepass/
+-rw-r--r--   0 evan      (1000) evan      (1000)      132 2022-07-15 21:42:52.000000 pykeepass-4.0.4/pykeepass/__init__.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     1657 2022-07-20 18:02:33.000000 pykeepass-4.0.4/pykeepass/attachment.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     5208 2022-07-20 18:02:33.000000 pykeepass-4.0.4/pykeepass/baseelement.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     1365 2021-03-05 05:26:01.000000 pykeepass-4.0.4/pykeepass/blank_database.kdbx
+-rw-r--r--   0 evan      (1000) evan      (1000)     3641 2022-07-20 18:02:33.000000 pykeepass-4.0.4/pykeepass/deprecated.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    12590 2023-05-12 05:57:00.000000 pykeepass-4.0.4/pykeepass/entry.py
+-rw-r--r--   0 evan      (1000) evan      (1000)      411 2022-06-27 23:09:55.000000 pykeepass-4.0.4/pykeepass/exceptions.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     3412 2022-12-26 00:46:40.000000 pykeepass-4.0.4/pykeepass/group.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     2403 2022-07-20 18:02:33.000000 pykeepass-4.0.4/pykeepass/icons.py
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-05-12 06:07:39.699094 pykeepass-4.0.4/pykeepass/kdbx_parsing/
+-rw-r--r--   0 evan      (1000) evan      (1000)       23 2021-03-05 05:26:01.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/__init__.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    13134 2022-07-15 21:41:20.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/common.py
+-rw-r--r--   0 evan      (1000) evan      (1000)      933 2022-11-14 23:31:17.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/kdbx.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     4922 2022-06-27 23:09:55.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/kdbx3.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     7954 2022-07-20 18:02:33.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/kdbx4.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    15444 2023-05-12 05:56:39.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/pytwofish.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    13307 2021-03-05 05:26:01.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/twofish.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    29383 2022-12-26 00:46:40.000000 pykeepass-4.0.4/pykeepass/pykeepass.py
+-rw-r--r--   0 evan      (1000) evan      (1000)      680 2022-02-16 22:22:34.000000 pykeepass-4.0.4/pykeepass/setters.py
+-rw-r--r--   0 evan      (1000) evan      (1000)       48 2023-05-12 06:00:15.000000 pykeepass-4.0.4/pykeepass/version.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     2848 2022-12-26 00:46:38.000000 pykeepass-4.0.4/pykeepass/xpath.py
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-05-12 06:07:39.695094 pykeepass-4.0.4/pykeepass.egg-info/
+-rw-r--r--   0 evan      (1000) evan      (1000)    14903 2023-05-12 06:07:39.000000 pykeepass-4.0.4/pykeepass.egg-info/PKG-INFO
+-rw-r--r--   0 evan      (1000) evan      (1000)      847 2023-05-12 06:07:39.000000 pykeepass-4.0.4/pykeepass.egg-info/SOURCES.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)        1 2023-05-12 06:07:39.000000 pykeepass-4.0.4/pykeepass.egg-info/dependency_links.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)       80 2023-05-12 06:07:39.000000 pykeepass-4.0.4/pykeepass.egg-info/requires.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)       10 2023-05-12 06:07:39.000000 pykeepass-4.0.4/pykeepass.egg-info/top_level.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)      125 2022-07-20 18:02:33.000000 pykeepass-4.0.4/requirements-rtd.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)      111 2022-07-20 18:02:33.000000 pykeepass-4.0.4/requirements.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)       38 2023-05-12 06:07:39.699094 pykeepass-4.0.4/setup.cfg
+-rw-r--r--   0 evan      (1000) evan      (1000)      934 2023-05-12 06:02:15.000000 pykeepass-4.0.4/setup.py
```

### Comparing `pykeepass-4.0.3/LICENSE` & `pykeepass-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.3/PKG-INFO` & `pykeepass-4.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pykeepass
-Version: 4.0.3
+Version: 4.0.4
 Summary: Python library to interact with keepass databases (supports KDBX3 and KDBX4)
 Home-page: https://github.com/libkeepass/pykeepass
 Author: Philipp Schmitt
 Author-email: philipp@schmitt.co
 License: GPL3
-Platform: UNKNOWN
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 pykeepass
 ============
 
 .. image:: https://github.com/libkeepass/pykeepass/workflows/CI/badge.svg
    :target: https://github.com/libkeepass/pykeepass/actions?query=workflow%3ACI
@@ -251,34 +251,34 @@
 
    # save the database
    >>> kp.save()
 
 Attachments
 -----------
 
-In this section, *binary* refers to the bytes of the attached data (stored at the root level of the database), while *attachment* is a reference to a binary (stored in an entry).  A binary can have none, one or many attachments.
+In this section, *binary* refers to the bytes of the attached data (stored at the root level of the database), while *attachment* is a reference to a binary (stored in an entry).  A binary can be referenced by none, one or many attachments.
 
 **add_binary** (data, compressed=True, protected=True)
 
-where ``data`` is bytes.  Adds a blob of data to the database. The attachment reference must still be added to an entry (see below).  ``compressed`` only applies to KDBX3 and ``protected`` only applies to KDBX4.  Returns id of attachment.
+where ``data`` is bytes.  Adds a blob of data to the database. The attachment reference must still be added to an entry (see below).  ``compressed`` only applies to KDBX3 and ``protected`` only applies to KDBX4 (no effect if used on wrong database version).  Returns id of attachment.
 
 **delete_binary** (id)
 
 where ``id`` is an int.  Removes binary data from the database and deletes any attachments that reference it.  Since attachments reference binaries by their positional index, attachments that reference binaries with id > ``id`` will automatically be decremented.
 
 **find_attachments** (id=None, filename=None, element=None, recursive=True, regex=False, flags=None, history=False, first=False)
 
 where ``id`` is an int, ``filename`` is a string, and element is an ``Entry`` or ``Group`` to search under.
 
 * if ``first=False``, the function returns a list of ``Attachment`` s or ``[]`` if there are no matches
 * if ``first=True``, the function returns the first ``Attachment`` match, or ``None`` if there are no matches
 
 **binaries**
 
-list of bytestrings containing binary data.  List index corresponds to attachment id.
+list of bytestrings containing binary data.  List index corresponds to attachment id
 
 **attachments**
 
 list containing all ``Attachment`` s in the database.
 
 **Entry.add_attachment** (id, filename)
 
@@ -389,14 +389,18 @@
 
 where ``filename`` is the path of the file to save to.  If ``filename`` is not given, the path given in ``read`` will be used.
 
 **password**
 
 string containing database password.  Can also be set.  Use ``None`` for no password.
 
+**filename**
+
+string containing path to database.  Can also be set
+
 **keyfile**
 
 string containing path to the database keyfile.  Can also be set.  Use ``None`` for no keyfile.
 
 **version**
 
 tuple containing database version.  e.g. ``(3, 1)`` is a KDBX version 3.1 database.
@@ -421,22 +425,20 @@
 
 pretty print database XML to file
 
 
 Tests and Debugging
 -------------------
 
-Run tests with :code:`python tests/tests.py`
+Run tests with :code:`python tests/tests.py` or :code:`python tests/tests.py SomeSpecificTest`
 
 Enable debugging when doing tests in console:
 
    >>> from pykeepass.pykeepass import debug_setup
    >>> debug_setup()
    >>> kp.entries[0]
    DEBUG:pykeepass.pykeepass:xpath query: //Entry
    DEBUG:pykeepass.pykeepass:xpath query: (ancestor::Group)[last()]
    DEBUG:pykeepass.pykeepass:xpath query: (ancestor::Group)[last()]
    DEBUG:pykeepass.pykeepass:xpath query: String/Key[text()="Title"]/../Value
    DEBUG:pykeepass.pykeepass:xpath query: String/Key[text()="UserName"]/../Value
    Entry: "root_entry (foobar_user)"
-
-
```

### Comparing `pykeepass-4.0.3/README.rst` & `pykeepass-4.0.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -240,34 +240,34 @@
 
    # save the database
    >>> kp.save()
 
 Attachments
 -----------
 
-In this section, *binary* refers to the bytes of the attached data (stored at the root level of the database), while *attachment* is a reference to a binary (stored in an entry).  A binary can have none, one or many attachments.
+In this section, *binary* refers to the bytes of the attached data (stored at the root level of the database), while *attachment* is a reference to a binary (stored in an entry).  A binary can be referenced by none, one or many attachments.
 
 **add_binary** (data, compressed=True, protected=True)
 
-where ``data`` is bytes.  Adds a blob of data to the database. The attachment reference must still be added to an entry (see below).  ``compressed`` only applies to KDBX3 and ``protected`` only applies to KDBX4.  Returns id of attachment.
+where ``data`` is bytes.  Adds a blob of data to the database. The attachment reference must still be added to an entry (see below).  ``compressed`` only applies to KDBX3 and ``protected`` only applies to KDBX4 (no effect if used on wrong database version).  Returns id of attachment.
 
 **delete_binary** (id)
 
 where ``id`` is an int.  Removes binary data from the database and deletes any attachments that reference it.  Since attachments reference binaries by their positional index, attachments that reference binaries with id > ``id`` will automatically be decremented.
 
 **find_attachments** (id=None, filename=None, element=None, recursive=True, regex=False, flags=None, history=False, first=False)
 
 where ``id`` is an int, ``filename`` is a string, and element is an ``Entry`` or ``Group`` to search under.
 
 * if ``first=False``, the function returns a list of ``Attachment`` s or ``[]`` if there are no matches
 * if ``first=True``, the function returns the first ``Attachment`` match, or ``None`` if there are no matches
 
 **binaries**
 
-list of bytestrings containing binary data.  List index corresponds to attachment id.
+list of bytestrings containing binary data.  List index corresponds to attachment id
 
 **attachments**
 
 list containing all ``Attachment`` s in the database.
 
 **Entry.add_attachment** (id, filename)
 
@@ -378,14 +378,18 @@
 
 where ``filename`` is the path of the file to save to.  If ``filename`` is not given, the path given in ``read`` will be used.
 
 **password**
 
 string containing database password.  Can also be set.  Use ``None`` for no password.
 
+**filename**
+
+string containing path to database.  Can also be set
+
 **keyfile**
 
 string containing path to the database keyfile.  Can also be set.  Use ``None`` for no keyfile.
 
 **version**
 
 tuple containing database version.  e.g. ``(3, 1)`` is a KDBX version 3.1 database.
@@ -410,15 +414,15 @@
 
 pretty print database XML to file
 
 
 Tests and Debugging
 -------------------
 
-Run tests with :code:`python tests/tests.py`
+Run tests with :code:`python tests/tests.py` or :code:`python tests/tests.py SomeSpecificTest`
 
 Enable debugging when doing tests in console:
 
    >>> from pykeepass.pykeepass import debug_setup
    >>> debug_setup()
    >>> kp.entries[0]
    DEBUG:pykeepass.pykeepass:xpath query: //Entry
```

### Comparing `pykeepass-4.0.3/pykeepass/baseelement.py` & `pykeepass-4.0.4/pykeepass/baseelement.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.3/pykeepass/blank_database.kdbx` & `pykeepass-4.0.4/pykeepass/blank_database.kdbx`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.3/pykeepass/group.py` & `pykeepass-4.0.4/pykeepass/group.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,59 +38,65 @@
                 )
             assert element.tag == 'Group', 'The provided element is not a Group '\
                 'element, but a {}'.format(element.tag)
             self._element = element
 
     @property
     def name(self):
+        """str: get or set group name"""
         return self._get_subelement_text('Name')
 
     @name.setter
     def name(self, value):
         return self._set_subelement_text('Name', value)
 
     @property
     def notes(self):
+        """str: get or set group notes"""
         return self._get_subelement_text('Notes')
 
     @notes.setter
     def notes(self, value):
         return self._set_subelement_text('Notes', value)
 
     @property
     def entries(self):
-        # FIXME
-        # It may be better to keep a list of Entries as a (list) property
-        # ... but that may become out of sync and what is supposed to happen
-        # when an entry is updated?!
-        # On the other side this would make things like "e in g.entries" work
+        """:obj:`list` of :obj:`Entry`: get list of entries in this group"""
         return [pykeepass.entry.Entry(element=x, kp=self._kp) for x in self._element.findall('Entry')]
 
     @property
     def subgroups(self):
+        """:obj:`list` of :obj:`Group`: get list of groups in this group"""
         return [Group(element=x, kp=self._kp) for x in self._element.findall('Group')]
 
     @property
     def is_root_group(self):
+        """bool: return True if this is the database root"""
         return self._element.getparent().tag == 'Root'
 
     @property
     def path(self):
+        """:obj:`list` of (:obj:`str` or None): a list containing names of all parent groups, not including root"""
         # The root group is an orphan
         if self.is_root_group or self.parentgroup is None:
             return []
         p = self.parentgroup
         path = [self.name]
         while p is not None and not p.is_root_group:
             if p.name is not None:  # dont make the root group appear
                 path.insert(0, p.name)
             p = p.parentgroup
         return path
 
     def append(self, entries):
+        """Add copy of an entry to this group
+
+        Args:
+            entries (:obj:`Entry` or :obj:`list` of :obj:`Entry`)
+        """
         if type(entries) is list:
             for e in entries:
                 self._element.append(e._element)
         else:
             self._element.append(entries._element)
 
     def __str__(self):
```

### Comparing `pykeepass-4.0.3/pykeepass/kdbx_parsing/common.py` & `pykeepass-4.0.4/pykeepass/kdbx_parsing/common.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.3/pykeepass/kdbx_parsing/kdbx.py` & `pykeepass-4.0.4/pykeepass/kdbx_parsing/kdbx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from construct import Struct, Switch, Bytes, Int16ul, RawCopy, this
+from construct import Struct, Switch, Bytes, Int16ul, RawCopy, Check, this
 from .kdbx3 import DynamicHeader as DynamicHeader3
 from .kdbx3 import Body as Body3
 from .kdbx4 import DynamicHeader as DynamicHeader4
 from .kdbx4 import Body as Body4
 
+# verify file signature
+def check_signature(ctx):
+    return ctx.sig1 == b'\x03\xd9\xa2\x9a' and ctx.sig2 == b'\x67\xFB\x4B\xB5'
+
 KDBX = Struct(
     "header" / RawCopy(
         Struct(
-            "magic1" / Bytes(4),
-            "magic2" / Bytes(4),
+            "sig1" / Bytes(4),
+            "sig2" / Bytes(4),
+            "sig_check" / Check(check_signature),
             "minor_version" / Int16ul,
             "major_version" / Int16ul,
             "dynamic_header" / Switch(
                 this.major_version,
                 {3: DynamicHeader3,
                  4: DynamicHeader4
                  }
```

### Comparing `pykeepass-4.0.3/pykeepass/kdbx_parsing/kdbx3.py` & `pykeepass-4.0.4/pykeepass/kdbx_parsing/kdbx3.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.3/pykeepass/kdbx_parsing/kdbx4.py` & `pykeepass-4.0.4/pykeepass/kdbx_parsing/kdbx4.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.3/pykeepass/kdbx_parsing/pytwofish.py` & `pykeepass-4.0.4/pykeepass/kdbx_parsing/pytwofish.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.3/pykeepass/kdbx_parsing/twofish.py` & `pykeepass-4.0.4/pykeepass/kdbx_parsing/twofish.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.3/pykeepass/pykeepass.py` & `pykeepass-4.0.4/pykeepass/pykeepass.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 import re
 import shutil
 import struct
 import uuid
 import zlib
 
 from binascii import Error as BinasciiError
-from construct import Container, ChecksumError
+from construct import Container, ChecksumError, CheckError
 from copy import deepcopy
 from dateutil import parser, tz
 from datetime import datetime, timedelta
 from lxml import etree
 from lxml.builder import E
+from pathlib import Path
 
 from pykeepass.attachment import Attachment
 from pykeepass.entry import Entry
 from pykeepass.exceptions import *
 from pykeepass.group import Group
 from pykeepass.kdbx_parsing.kdbx import KDBX
 from pykeepass.kdbx_parsing.kdbx4 import kdf_uuids
@@ -108,27 +109,34 @@
                 self.kdbx = KDBX.parse_file(
                     filename,
                     password=password,
                     keyfile=keyfile,
                     transformed_key=transformed_key
                 )
 
+        except CheckError as e:
+            if e.path == '(parsing) -> header -> sig_check':
+                raise HeaderChecksumError("Not a KeePass database")
+            else:
+                raise
+
+        # body integrity/verification
         except ChecksumError as e:
             if e.path in (
                     '(parsing) -> body -> cred_check', # KDBX4
                     '(parsing) -> cred_check' # KDBX3
                     ):
-                raise CredentialsError
+                raise CredentialsError("Invalid credentials")
             elif e.path == '(parsing) -> body -> sha256':
-                raise HeaderChecksumError
+                raise HeaderChecksumError("Corrupted database")
             elif e.path in (
                     '(parsing) -> body -> payload -> hmac_hash', # KDBX4
                     '(parsing) -> xml -> block_hash' # KDBX3
                     ):
-                raise PayloadChecksumError
+                raise PayloadChecksumError("Error reading database contents")
             else:
                 raise
 
     def reload(self):
         """Reload current database using previous credentials """
 
         self.read(self.filename, self.password, self.keyfile)
@@ -154,16 +162,15 @@
                 password=self.password,
                 keyfile=self.keyfile,
                 transformed_key=transformed_key
             )
         else:
             # save to temporary file to prevent database clobbering
             # see issues 223, 101
-            # FIXME python2 - use pathlib.Path.withsuffix
-            filename_tmp = filename + '.tmp'
+            filename_tmp = Path(filename).with_suffix('.tmp')
             try:
                 KDBX.build_file(
                     self.kdbx,
                     filename_tmp,
                     password=self.password,
                     keyfile=self.keyfile,
                     transformed_key=transformed_key
@@ -284,14 +291,17 @@
                 False, function returns list of matches or empty list.  Default
                 is False.
             history (bool): If True, history entries are included in results.
                 Default is False.
             cast (bool): If True, matches are instead instantiated as
                 pykeepass Group, Entry, or Attachment objects.  An exception
                 is raised if a match cannot be cast.  Default is False.
+
+        Returns:
+            `Group`, `Entry`, `Attachment`, or `lxml.etree.Element`
         """
 
         if tree is None:
             tree = self.tree
         logger.debug('xpath query: ' + xpath_str)
         elements = tree.xpath(
             xpath_str, namespaces={'re': 'http://exslt.org/regular-expressions'}
@@ -316,14 +326,15 @@
         if first:
             res = res[0] if res else None
 
         return res
 
     def _find(self, prefix, keys_xp, path=None, tree=None, first=False,
               history=False, regex=False, flags=None, **kwargs):
+        """Internal function for converting a search into an XPath string"""
 
         xp = ''
 
         if path is not None:
 
             first = True
 
@@ -388,61 +399,43 @@
         uuid_str = base64.b64encode( entry_or_group.uuid.bytes).decode('utf-8')
         elem = self._xpath('./UUID[text()="{}"]/..'.format(uuid_str), tree=recyclebin_group._element, first=True, history=False, cast=False)
         return elem is None
 
 
     # ---------- Groups ----------
 
-    def find_groups(self, recursive=True, path=None, group=None, **kwargs):
+    from .deprecated import (
+        find_groups_by_name, find_groups_by_path, find_groups_by_uuid,
+        find_groups_by_notes
+    )
 
-        prefix = '//Group' if recursive else '/Group'
-        res = self._find(prefix, group_xp, path=path, tree=group, **kwargs)
-        return res
+    def find_groups(self, recursive=True, path=None, group=None, **kwargs):
+        """
+        Find groups in a database
 
-    def find_groups_by_name(self, group_name, regex=False, flags=None,
-                            group=None, first=False):
-        return self.find_groups(
-            name=group_name,
-            regex=regex,
-            flags=flags,
-            group=group,
-            first=first
-        )
+        Args:
+            name (str): name of group
+            first (bool): return first result instead of list (default False)
+            recursive (bool): do a recursive search of all groups/subgroups
+            path (str): do group search starting from path
+            group (Group): search underneath group
+            uuid (uuid.UUID): group UUID
+            regex (bool): whether `str` search arguments contain [XSLT style][XSLT style] regular expression
+            flags (str): XPath [flags][flags]
 
-    def find_groups_by_path(self, group_path_str=None, regex=False, flags=None,
-                            group=None, first=False):
-        return self.find_groups(
-            path=group_path_str,
-            regex=regex,
-            flags=flags,
-            group=group,
-            first=first
-        )
+        Returns:
+            :obj:`list` of :obj:`Group` or :obj:`Group`
 
-    def find_groups_by_uuid(self, uuid, regex=False, flags=None,
-                            group=None, history=False, first=False):
-        return self.find_groups(
-            uuid=uuid,
-            regex=regex,
-            flags=flags,
-            group=group,
-            history=history,
-            first=first
-        )
+        [XSLT style]: https://www.xml.com/pub/a/2003/06/04/tr.html
+        [flags]: https://www.w3.org/TR/xpath-functions/#flags
+        """
 
-    def find_groups_by_notes(self, notes, regex=False, flags=None,
-                             group=None, history=False, first=False):
-        return self.find_groups(
-            notes=notes,
-            regex=regex,
-            flags=flags,
-            group=group,
-            history=history,
-            first=first
-        )
+        prefix = '//Group' if recursive else '/Group'
+        res = self._find(prefix, group_xp, path=path, tree=group, **kwargs)
+        return res
 
     # creates a new group and all parent groups, if necessary
     def add_group(self, destination_group, group_name, icon=None, notes=None):
         logger.debug('Creating group {}'.format(group_name))
 
         if icon:
             group = Group(name=group_name, icon=icon, notes=notes, kp=self)
@@ -451,37 +444,14 @@
         destination_group.append(group)
 
         return group
 
     def delete_group(self, group):
         group.delete()
 
-    def deref(self, value):
-        if not value:
-            return value
-        references = set(re.findall(r'({REF:([TUPANI])@([TUPANI]):([^}]+)})', value))
-        if not references:
-            return value
-        field_to_attribute = {
-            'T': 'title',
-            'U': 'username',
-            'P': 'password',
-            'A': 'url',
-            'N': 'notes',
-            'I': 'uuid',
-        }
-        for ref, wanted_field, search_in, search_value in references:
-            wanted_field = field_to_attribute[wanted_field]
-            search_in = field_to_attribute[search_in]
-            if search_in == 'uuid':
-                search_value = uuid.UUID(search_value)
-            ref_entry = self.find_entries(first=True, **{search_in: search_value})
-            value = value.replace(ref, getattr(ref_entry, wanted_field))
-        return self.deref(value)
-
     def move_group(self, group, destination_group):
         destination_group.append(group)
 
     def _create_or_get_recyclebin_group(self, **kwargs):
         existing_group = self.recyclebin_group
         if existing_group is not None:
             return existing_group
@@ -513,108 +483,28 @@
         while len(group.subgroups):
             self.delete_group(group.subgroups[0])
         while len(group.entries):
             self.delete_entry(group.entries[0])
 
     # ---------- Entries ----------
 
+
+    from .deprecated import (
+        find_entries_by_title, find_entries_by_username, find_entries_by_password,
+        find_entries_by_url, find_entries_by_path, find_entries_by_notes,
+        find_entries_by_string, find_entries_by_uuid
+    )
+
     def find_entries(self, recursive=True, path=None, group=None, **kwargs):
 
         prefix = '//Entry' if recursive else '/Entry'
         res = self._find(prefix, entry_xp, path=path, tree=group, **kwargs)
 
         return res
 
-    def find_entries_by_title(self, title, regex=False, flags=None,
-                              group=None, history=False, first=False):
-        return self.find_entries(
-            title=title,
-            regex=regex,
-            flags=flags,
-            group=group,
-            history=history,
-            first=first
-        )
-
-    def find_entries_by_username(self, username, regex=False, flags=None,
-                                 group=None, history=False, first=False):
-        return self.find_entries(
-            username=username,
-            regex=regex,
-            flags=flags,
-            group=group,
-            history=history,
-            first=first
-        )
-
-    def find_entries_by_password(self, password, regex=False, flags=None,
-                                 group=None, history=False, first=False):
-        return self.find_entries(
-            password=password,
-            regex=regex,
-            flags=flags,
-            group=group,
-            history=history,
-            first=first
-        )
-
-    def find_entries_by_url(self, url, regex=False, flags=None,
-                            group=None, history=False, first=False):
-        return self.find_entries(
-            url=url,
-            regex=regex,
-            flags=flags,
-            group=group,
-            history=history,
-            first=first
-        )
-
-    def find_entries_by_notes(self, notes, regex=False, flags=None,
-                              group=None, history=False, first=False):
-        return self.find_entries(
-            notes=notes,
-            regex=regex,
-            flags=flags,
-            group=group,
-            history=history,
-            first=first
-        )
-
-    def find_entries_by_path(self, path, regex=False, flags=None,
-                             group=None, history=False, first=False):
-        return self.find_entries(
-            path=path,
-            regex=regex,
-            flags=flags,
-            group=group,
-            history=history,
-            first=first
-        )
-
-    def find_entries_by_uuid(self, uuid, regex=False, flags=None,
-                             group=None, history=False, first=False):
-        return self.find_entries(
-            uuid=uuid,
-            regex=regex,
-            flags=flags,
-            group=group,
-            history=history,
-            first=first
-        )
-
-    def find_entries_by_string(self, string, regex=False, flags=None,
-                               group=None, history=False, first=False):
-        return self.find_entries(
-            string=string,
-            regex=regex,
-            flags=flags,
-            group=group,
-            history=history,
-            first=first
-        )
 
     def add_entry(self, destination_group, title, username,
                   password, url=None, notes=None, expiry_time=None,
                   tags=None, otp=None, icon=None, force_creation=False):
 
         entries = self.find_entries(
             title=title,
@@ -683,21 +573,24 @@
     def binaries(self):
         if self.version >= (4, 0):
             # first byte is a prepended flag
             binaries = [a.data[1:] for a in self.kdbx.body.payload.inner_header.binary]
         else:
             binaries = []
             for elem in self._xpath('/KeePassFile/Meta/Binaries/Binary'):
-                if elem.get('Compressed') == 'True':
-                    data = zlib.decompress(
-                        base64.b64decode(elem.text),
-                        zlib.MAX_WBITS | 32
-                    )
+                if elem.text is not None:
+                    if elem.get('Compressed') == 'True':
+                        data = zlib.decompress(
+                            base64.b64decode(elem.text),
+                            zlib.MAX_WBITS | 32
+                        )
+                    else:
+                        data = base64.b64decode(elem.text)
                 else:
-                    data = base64.b64decode(elem.text)
+                    data = b''
                 binaries.insert(int(elem.attrib['ID']), data)
 
         return binaries
 
     def add_binary(self, data, compressed=True, protected=True):
         if self.version >= (4, 0):
             # add protected flag byte
@@ -755,95 +648,123 @@
         binaries_gt = self._xpath(
             '//Binary/Value[@Ref > "{}"]/..'.format(id),
             cast=True
         )
         for reference in binaries_gt:
             reference.id = reference.id - 1
 
+    # ---------- Misc ----------
+
+    def deref(self, value):
+
+        """Dereference [field reference][fieldref] of Entry
+
+        Args:
+            ref (str): KeePass reference string to another field
+
+        Returns:
+            str or uuid.UUID
+
+        [fieldref]: https://keepass.info/help/base/fieldrefs.html
+        """
+        if not value:
+            return value
+        references = set(re.findall(r'({REF:([TUPANI])@([TUPANI]):([^}]+)})', value))
+        if not references:
+            return value
+        field_to_attribute = {
+            'T': 'title',
+            'U': 'username',
+            'P': 'password',
+            'A': 'url',
+            'N': 'notes',
+            'I': 'uuid',
+        }
+        for ref, wanted_field, search_in, search_value in references:
+            wanted_field = field_to_attribute[wanted_field]
+            search_in = field_to_attribute[search_in]
+            if search_in == 'uuid':
+                search_value = uuid.UUID(search_value)
+            ref_entry = self.find_entries(first=True, **{search_in: search_value})
+            value = value.replace(ref, getattr(ref_entry, wanted_field))
+        return self.deref(value)
+
+
     # ---------- Credential Changing and Expiry ----------
 
-    # make password/keyfile into property instead of attribute so
-    # MasterKeyChanged can be set correctly
     @property
     def password(self):
+        """str: Get or set database password"""
         return self._password
 
     @password.setter
     def password(self, password):
         self._password = password
         self.credchange_date = datetime.now()
 
     @property
     def keyfile(self):
+        """str or pathlib.Path: get or set database keyfile"""
         return self._keyfile
 
     @keyfile.setter
     def keyfile(self, keyfile):
         self._keyfile = keyfile
         self.credchange_date = datetime.now()
 
     @property
     def credchange_required_days(self):
-        """Days until password update should be required"""
+        """int: Days until password update should be required"""
         e = self._xpath('/KeePassFile/Meta/MasterKeyChangeForce', first=True)
         if e is not None:
             return int(e.text)
 
     @property
     def credchange_recommended_days(self):
-        """Days until password update should be recommended"""
+        """int: Days until password update should be recommended"""
         e = self._xpath('/KeePassFile/Meta/MasterKeyChangeRec', first=True)
         if e is not None:
             return int(e.text)
 
     @credchange_required_days.setter
     def credchange_required_days(self, days):
-        """Set credentials required expiry days
-
-        Args:
-            days (int): days from password change until expiry
-        """
-
         path = '/KeePassFile/Meta/MasterKeyChangeForce'
         item = self._xpath(path, first=True)
         item.text = str(days)
 
     @credchange_recommended_days.setter
     def credchange_recommended_days(self, days):
-        """Set credentials recommended expiry days
-
-        Args:
-            days (int): days from password change until warning
-        """
-
         path = '/KeePassFile/Meta/MasterKeyChangeRec'
         item = self._xpath(path, first=True)
         item.text = str(days)
 
     @property
     def credchange_date(self):
+        """datetime.datetime: get or set UTC time of last credential change"""
         e = self._xpath('/KeePassFile/Meta/MasterKeyChanged', first=True)
         if e is not None:
             return self._decode_time(e.text)
 
     @credchange_date.setter
     def credchange_date(self, date):
         time = self._xpath('/KeePassFile/Meta/MasterKeyChanged', first=True)
         time.text = self._encode_time(date)
 
     @property
     def credchange_required(self):
+        """bool: Check if credential change is required"""
         change_date = self.credchange_date
         if change_date is None or self.credchange_required_days == -1:
             return False
         now_date = self._datetime_to_utc(datetime.now())
         return (now_date - change_date).days > self.credchange_required_days
 
     @property
     def credchange_recommended(self):
+        """bool: Check if credential change is recommended"""
         change_date = self.credchange_date
         if change_date is None or self.credchange_recommended_days == -1:
             return False
         now_date = self._datetime_to_utc(datetime.now())
         return (now_date - change_date).days > self.credchange_recommended_days
 
     # ---------- Datetime Functions ----------
@@ -852,15 +773,15 @@
         """Convert naive datetimes to UTC"""
 
         if not dt.tzinfo:
             dt = dt.replace(tzinfo=tz.gettz())
         return dt.astimezone(tz.gettz('UTC'))
 
     def _encode_time(self, value):
-        """Convert datetime to base64 or plaintext string"""
+        """bytestring or plaintext string: Convert datetime to base64 or plaintext string"""
 
         if self.version >= (4, 0):
             diff_seconds = int(
                 (
                     self._datetime_to_utc(value) -
                     datetime(
                         year=1,
@@ -873,15 +794,15 @@
             return base64.b64encode(
                 struct.pack('<Q', diff_seconds)
             ).decode('utf-8')
         else:
             return self._datetime_to_utc(value).isoformat()
 
     def _decode_time(self, text):
-        """Convert base64 time or plaintext time to datetime"""
+        """datetime.datetime: Convert base64 time or plaintext time to datetime"""
 
         if self.version >= (4, 0):
             # decode KDBX4 date from b64 format
             try:
                 return (
                     datetime(year=1, month=1, day=1, tzinfo=tz.gettz('UTC')) +
                     timedelta(
@@ -898,14 +819,30 @@
                 text,
                 tzinfos={'UTC': tz.gettz('UTC')}
             )
 
 def create_database(
         filename, password=None, keyfile=None, transformed_key=None
 ):
+    """
+    Create a new database at ``filename`` with supplied credentials.
+
+    Args:
+        filename (:obj:`str`, optional): path to database or stream object.
+            If None, the path given when the database was opened is used.
+        password (:obj:`str`, optional): database password.  If None,
+            database is assumed to have no password
+        keyfile (:obj:`str`, optional): path to keyfile.  If None,
+            database is assumed to have no keyfile
+        transformed_key (:obj:`bytes`, optional): precomputed transformed
+            key.
+
+    Returns:
+        PyKeePass
+    """
     keepass_instance = PyKeePass(
         BLANK_DATABASE_LOCATION, BLANK_DATABASE_PASSWORD
     )
 
     keepass_instance.filename = filename
     keepass_instance.password = password
     keepass_instance.keyfile = keyfile
```

### Comparing `pykeepass-4.0.3/pykeepass/setters.py` & `pykeepass-4.0.4/pykeepass/setters.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.3/pykeepass/xpath.py` & `pykeepass-4.0.4/pykeepass/xpath.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.3/pykeepass.egg-info/PKG-INFO` & `pykeepass-4.0.4/pykeepass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pykeepass
-Version: 4.0.3
+Version: 4.0.4
 Summary: Python library to interact with keepass databases (supports KDBX3 and KDBX4)
 Home-page: https://github.com/libkeepass/pykeepass
 Author: Philipp Schmitt
 Author-email: philipp@schmitt.co
 License: GPL3
-Platform: UNKNOWN
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 pykeepass
 ============
 
 .. image:: https://github.com/libkeepass/pykeepass/workflows/CI/badge.svg
    :target: https://github.com/libkeepass/pykeepass/actions?query=workflow%3ACI
@@ -251,34 +251,34 @@
 
    # save the database
    >>> kp.save()
 
 Attachments
 -----------
 
-In this section, *binary* refers to the bytes of the attached data (stored at the root level of the database), while *attachment* is a reference to a binary (stored in an entry).  A binary can have none, one or many attachments.
+In this section, *binary* refers to the bytes of the attached data (stored at the root level of the database), while *attachment* is a reference to a binary (stored in an entry).  A binary can be referenced by none, one or many attachments.
 
 **add_binary** (data, compressed=True, protected=True)
 
-where ``data`` is bytes.  Adds a blob of data to the database. The attachment reference must still be added to an entry (see below).  ``compressed`` only applies to KDBX3 and ``protected`` only applies to KDBX4.  Returns id of attachment.
+where ``data`` is bytes.  Adds a blob of data to the database. The attachment reference must still be added to an entry (see below).  ``compressed`` only applies to KDBX3 and ``protected`` only applies to KDBX4 (no effect if used on wrong database version).  Returns id of attachment.
 
 **delete_binary** (id)
 
 where ``id`` is an int.  Removes binary data from the database and deletes any attachments that reference it.  Since attachments reference binaries by their positional index, attachments that reference binaries with id > ``id`` will automatically be decremented.
 
 **find_attachments** (id=None, filename=None, element=None, recursive=True, regex=False, flags=None, history=False, first=False)
 
 where ``id`` is an int, ``filename`` is a string, and element is an ``Entry`` or ``Group`` to search under.
 
 * if ``first=False``, the function returns a list of ``Attachment`` s or ``[]`` if there are no matches
 * if ``first=True``, the function returns the first ``Attachment`` match, or ``None`` if there are no matches
 
 **binaries**
 
-list of bytestrings containing binary data.  List index corresponds to attachment id.
+list of bytestrings containing binary data.  List index corresponds to attachment id
 
 **attachments**
 
 list containing all ``Attachment`` s in the database.
 
 **Entry.add_attachment** (id, filename)
 
@@ -389,14 +389,18 @@
 
 where ``filename`` is the path of the file to save to.  If ``filename`` is not given, the path given in ``read`` will be used.
 
 **password**
 
 string containing database password.  Can also be set.  Use ``None`` for no password.
 
+**filename**
+
+string containing path to database.  Can also be set
+
 **keyfile**
 
 string containing path to the database keyfile.  Can also be set.  Use ``None`` for no keyfile.
 
 **version**
 
 tuple containing database version.  e.g. ``(3, 1)`` is a KDBX version 3.1 database.
@@ -421,22 +425,20 @@
 
 pretty print database XML to file
 
 
 Tests and Debugging
 -------------------
 
-Run tests with :code:`python tests/tests.py`
+Run tests with :code:`python tests/tests.py` or :code:`python tests/tests.py SomeSpecificTest`
 
 Enable debugging when doing tests in console:
 
    >>> from pykeepass.pykeepass import debug_setup
    >>> debug_setup()
    >>> kp.entries[0]
    DEBUG:pykeepass.pykeepass:xpath query: //Entry
    DEBUG:pykeepass.pykeepass:xpath query: (ancestor::Group)[last()]
    DEBUG:pykeepass.pykeepass:xpath query: (ancestor::Group)[last()]
    DEBUG:pykeepass.pykeepass:xpath query: String/Key[text()="Title"]/../Value
    DEBUG:pykeepass.pykeepass:xpath query: String/Key[text()="UserName"]/../Value
    Entry: "root_entry (foobar_user)"
-
-
```

### Comparing `pykeepass-4.0.3/setup.py` & `pykeepass-4.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 setup(
     name="pykeepass",
     version=version["__version__"],
     license="GPL3",
     description="Python library to interact with keepass databases "
     "(supports KDBX3 and KDBX4)",
     long_description=README,
+    long_description_content_type='text/x-rst',
     author="Philipp Schmitt",
     author_email="philipp@schmitt.co",
     url="https://github.com/libkeepass/pykeepass",
     packages=find_packages(include=['pykeepass', 'pykeepass.*']),
     install_requires=[
         "python-dateutil",
         # FIXME python2 - last version to support python2
```

