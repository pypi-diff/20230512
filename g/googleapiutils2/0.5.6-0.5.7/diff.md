# Comparing `tmp/googleapiutils2-0.5.6.tar.gz` & `tmp/googleapiutils2-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.5.6.tar", max compression
+gzip compressed data, was "googleapiutils2-0.5.7.tar", max compression
```

## Comparing `googleapiutils2-0.5.6.tar` & `googleapiutils2-0.5.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.5.6/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.5.6/README.md
--rw-r--r--   0        0        0       96 2023-01-30 06:00:44.616601 googleapiutils2-0.5.6/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-01-15 05:10:18.196566 googleapiutils2-0.5.6/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    17597 2023-05-11 16:28:47.016478 googleapiutils2-0.5.6/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.5.6/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.5.6/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1049 2022-12-30 01:32:12.342019 googleapiutils2-0.5.6/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.5.6/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      118 2023-01-30 06:00:44.617619 googleapiutils2-0.5.6/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     6494 2023-05-09 18:46:09.012912 googleapiutils2-0.5.6/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    17179 2023-05-11 16:28:47.017272 googleapiutils2-0.5.6/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     4925 2023-05-11 16:28:47.017646 googleapiutils2-0.5.6/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     7387 2023-05-11 16:28:47.018058 googleapiutils2-0.5.6/googleapiutils2/utils.py
--rw-r--r--   0        0        0      811 2023-05-11 16:29:09.434718 googleapiutils2-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 googleapiutils2-0.5.6/setup.py
--rw-r--r--   0        0        0     6166 1970-01-01 00:00:00.000000 googleapiutils2-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.5.7/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.5.7/README.md
+-rw-r--r--   0        0        0       96 2023-01-30 06:00:44.616601 googleapiutils2-0.5.7/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-01-15 05:10:18.196566 googleapiutils2-0.5.7/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    17597 2023-05-11 16:28:47.016478 googleapiutils2-0.5.7/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.5.7/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.5.7/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1049 2022-12-30 01:32:12.342019 googleapiutils2-0.5.7/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.5.7/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      118 2023-01-30 06:00:44.617619 googleapiutils2-0.5.7/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     6494 2023-05-09 18:46:09.012912 googleapiutils2-0.5.7/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    17179 2023-05-11 16:28:47.017272 googleapiutils2-0.5.7/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     4925 2023-05-11 16:28:47.017646 googleapiutils2-0.5.7/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     7387 2023-05-11 16:28:47.018058 googleapiutils2-0.5.7/googleapiutils2/utils.py
+-rw-r--r--   0        0        0      811 2023-05-12 17:24:45.709013 googleapiutils2-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 googleapiutils2-0.5.7/setup.py
+-rw-r--r--   0        0        0     6166 1970-01-01 00:00:00.000000 googleapiutils2-0.5.7/PKG-INFO
```

### Comparing `googleapiutils2-0.5.6/LICENSE` & `googleapiutils2-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.6/README.md` & `googleapiutils2-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.6/googleapiutils2/drive/drive.py` & `googleapiutils2-0.5.7/googleapiutils2/drive/drive.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.6/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.5.7/googleapiutils2/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.6/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.5.7/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.6/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.5.7/googleapiutils2/sheets/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.6/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.5.7/googleapiutils2/sheets/sheets.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.6/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.5.7/googleapiutils2/sheets/sheets_value_range.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.6/googleapiutils2/utils.py` & `googleapiutils2-0.5.7/googleapiutils2/utils.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.6/pyproject.toml` & `googleapiutils2-0.5.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.5.6"
+version = "0.5.7"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 google-auth-httplib2 = "^0.1.0"
 google-auth-oauthlib = "^0.5.1"
 google-api-python-client = "^2.47.0"
 requests = "^2.28.1"
-pandas = "^1.5.3"
 cachetools = "^5.2.1"
 google-api-python-client-stubs = "^1.11.0"
+pandas = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 types-requests = "^2.28.9"
 types-cachetools = "^5.2.1"
 pytest = "^7.2.0"
 pandas-stubs = "^2.0.1.230501"
 black = "^22.6.0"
```

### Comparing `googleapiutils2-0.5.6/setup.py` & `googleapiutils2-0.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 
 install_requires = \
 ['cachetools>=5.2.1,<6.0.0',
  'google-api-python-client-stubs>=1.11.0,<2.0.0',
  'google-api-python-client>=2.47.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.1,<0.6.0',
- 'pandas>=1.5.3,<2.0.0',
+ 'pandas>=2.0.1,<3.0.0',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'googleapiutils2',
-    'version': '0.5.6',
+    'version': '0.5.7',
     'description': "Wrapper for Google's Python API.",
     'long_description': '# googleapiutils2\n\nUtilities for\n[Google\'s v2 Python API](https://github.com/googleapis/google-api-python-client).\nCurrently supports sections of the following resources:\n\n-   [Drive](https://developers.google.com/drive/api/reference/rest/v3): `DriveResource`,\n    `FilesResource`, `PermissionsResource`, `RepliesResource`, `...`\n-   [Sheets](https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets):\n    `SpreadsheetsResource`, `ValuesResource`, `...`\n-   [Geocoding](https://developers.google.com/maps/documentation/geocoding/overview)\n\n## Quickstart\n\nThis project requires Python `^3.10` to run.\n\nSeveral dependencies are needed, namely the aforesaid Google Python API, but also\nGoogle\'s oauth library, and `requests`. Pre-bundled for ease of use are the fairly\nmonolithic `google-api-stubs`, which greatly improves the usage experience.\n\n### via [`poetry`](https://python-poetry.org/docs/)\n\nInstall poetry, then run\n\n> poetry install\n\nAnd you\'re done.\n\n## Overview\n\nThe library was written to be consistent with Google\'s own Python API - just a little\neasier to use. Most `Drive` and `Sheets` operations are supported using explicit\nparameters. But most functions thereof take a `**kwargs` parameter (used for parameter\nforwarding) to allow for the more granular usage of the underlying API.\n\nA note on IDs: anytime a resource ID is needed, one can be provide the actual resource\nID, or the URL to the resource. If a URL is provided, this mapping is cached for future\nuse.\n\n## Authentication\n\nBefore using a `Drive` or `Sheets` object, one must first authenticate. This is done via\nthe `google.oauth2` library, creating a `Credentials` object.\n\nThe library supports two methods of authentication:\n\n-   via a Google service account (recommended, see more\n    [here](https://cloud.google.com/iam/docs/creating-managing-service-accounts))\n-   via OAuth2 (see more\n    [here](https://developers.google.com/identity/protocols/oauth2/native-app))\n\nWith a service account, one can programmatically access resources without user input.\nThis is by far the easiest route, but requires a bit of setup.\n\nIf not using a service account, the library will attempt to open a browser window to\nauthenticate using the provided credentials. This authentication is cached for future\nusage (though it does expire on some interval) - so an valid token path is required.\n\nSee the [`get_oauth2_creds`](googleapiutils2/utils.py) function for more information.\n\n## Drive\n\nExample: copy a file to a folder.\n\n```python\ncreds = get_oauth2_creds(config_obj)\ndrive = Drive(creds)\n\nfilename = "Heyy"\n\nfile = drive.get_name(filename, parents=[FOLDER_URL])\nif file is not None:\n    drive.delete(file["id"])\n\nfile = drive.copy(file_id=FILE_ID, to_filename=filename, to_folder_id=FOLDER_URL)\n```\n\nWhat the above does is:\n\n-   Get the OAuth2 credentials from the `config_obj` object (JSON object representing\n    the requisite credentials, see\n    [here](https://developers.google.com/identity/protocols/oauth2/native-app#step-2:-send-a-request-to-googles-oauth-2.0-server)\n    for more information).\n-   create a `Drive` object thereupon.\n-   Get the file with the given name, and delete it if it exists.\n-   Copy the file with the given ID to the given folder, and return the new file.\n\n## Sheets\n\nExample: update a range of cells in a sheet.\n\n```python\ncreds = get_oauth2_creds(config_path)\nsheets = Sheets(creds)\n\nSheet1 = SheetsValueRange(sheets, SHEET_ID, sheet_name="Sheet1")\n\nrows = [\n    {\n        "Heyy": "99",\n    }\n]\nSheet1[2:3, ...].update(rows)\n```\n\nWhat the above does is:\n\n-   Get the OAuth2 credentials from the `config_path` file (see\n    [here](https://developers.google.com/identity/protocols/oauth2/native-app#step-2:-send-a-request-to-googles-oauth-2.0-server)\n    for more information).\n-   create a `Sheets` object thereupon.\n-   Create a `SheetsValueRange` object, which is a wrapper around the\n    `spreadsheets.values` API.\n-   Update the range `Sheet1!A2:B3` with the given rows.\n\nNote the slicing syntax, which will feel quite familiar for any user of Numpy or Pandas.\n\n### SheetSlice\n\nA `SheetsValueRange` object can be sliced in a similar manner to that of a Numpy array.\nThe syntax is as follows:\n\n    slc = Sheet[rows, cols]\n\nWherein `rows` and `cols` are either integers, slices of integers (stride is not\nsupported), strings (in A1 notation), or ellipses (`...`).\n\nNote that Google\'s implementation of A1 notation is 1-indexed; 0 is invalid (e.g., 1\nmaps to `A`, 2 to `B`, etc.)\n\n```py\nix = SheetSlice["Sheet1", 1:3, 2:4] #  "Sheet1!B2:D4"\nix = SheetSlice["Sheet1", "A1:B2"]  #  "Sheet1!A1:B2"\nix = SheetSlice[1:3, 2:4]           #  "Sheet1!B2:D4"\nix = SheetSlice["A1:B2"]            #  "Sheet1!A1:B2"\nix = SheetSlice[..., 1:3]           #  "Sheet1!A1:Z3"\n\nvalues = {\n    SheetSlice["A1:B2"]: [\n        ["Heyy", "99"],\n        ["Heyy", "99"],\n    ],\n} # "Sheet1!A1:B2" = [["Heyy", "99"], ["Heyy", "99"]]\n```\n\nA `SheetSlice` can also be used as a key into a `SheetsValueRange`, or a dictionary (to\nuse in updating a sheet\'s range via `.update()`, for example). Further, a\n`SheetsValueRange` can be sliced in a similar manner to that of a `SheetSlice`.\n\n```py\nSheet1[2:3, ...].update(rows)\n...\n```\n',
     'author': 'Mike Babb',
     'author_email': 'mike7400@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mkbabb/googleapiutils2',
```

### Comparing `googleapiutils2-0.5.6/PKG-INFO` & `googleapiutils2-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.5.6
+Version: 0.5.7
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cachetools (>=5.2.1,<6.0.0)
 Requires-Dist: google-api-python-client (>=2.47.0,<3.0.0)
 Requires-Dist: google-api-python-client-stubs (>=1.11.0,<2.0.0)
 Requires-Dist: google-auth-httplib2 (>=0.1.0,<0.2.0)
 Requires-Dist: google-auth-oauthlib (>=0.5.1,<0.6.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/mkbabb/googleapiutils2
 Description-Content-Type: text/markdown
 
 # googleapiutils2
 
 Utilities for
```

