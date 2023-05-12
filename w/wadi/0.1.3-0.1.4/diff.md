# Comparing `tmp/wadi-0.1.3.tar.gz` & `tmp/wadi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wadi-0.1.3.tar", last modified: Mon May  8 07:37:10 2023, max compression
+gzip compressed data, was "wadi-0.1.4.tar", last modified: Fri May 12 10:54:46 2023, max compression
```

## Comparing `wadi-0.1.3.tar` & `wadi-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:37:10.103058 wadi-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 07:36:56.000000 wadi-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-08 07:37:10.103058 wadi-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-08 07:36:56.000000 wadi-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:37:10.103058 wadi-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-08 07:36:56.000000 wadi-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:37:10.099058 wadi-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 07:36:56.000000 wadi-0.1.3/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:37:10.099058 wadi-0.1.3/wadi/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/dataobject.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/documentation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/filereader.py
--rw-r--r--   0 runner    (1001) docker     (123)    17600 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/harmonizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/infotable.py
--rw-r--r--   0 runner    (1001) docker     (123)    29659 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/unitconverter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:37:10.103058 wadi-0.1.3/wadi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-08 07:37:10.000000 wadi-0.1.3/wadi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-08 07:37:10.000000 wadi-0.1.3/wadi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:37:10.000000 wadi-0.1.3/wadi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-08 07:37:10.000000 wadi-0.1.3/wadi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 07:37:10.000000 wadi-0.1.3/wadi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:54:46.936150 wadi-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 10:54:32.000000 wadi-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-12 10:54:46.936150 wadi-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-12 10:54:32.000000 wadi-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:54:46.936150 wadi-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-12 10:54:32.000000 wadi-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:54:46.928150 wadi-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-12 10:54:32.000000 wadi-0.1.4/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:54:46.932150 wadi-0.1.4/wadi/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/documentation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/filereader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/harmonizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/infotable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29684 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/unitconverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:54:46.936150 wadi-0.1.4/wadi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-12 10:54:46.000000 wadi-0.1.4/wadi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-12 10:54:46.000000 wadi-0.1.4/wadi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:54:46.000000 wadi-0.1.4/wadi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-12 10:54:46.000000 wadi-0.1.4/wadi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 10:54:46.000000 wadi-0.1.4/wadi.egg-info/top_level.txt
```

### Comparing `wadi-0.1.3/LICENSE` & `wadi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wadi-0.1.3/PKG-INFO` & `wadi-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: wadi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generic importer for water quality data of the (Dutch) water laboratory
 Home-page: https://github.com/KWR-Water/wadi
 Author: KWR Water Research Institute
 Author-email: martin.korevaar@kwrwater.nl, martin.van.der.schans@kwrwater.nl
 License: MIT
 Project-URL: Source, https://github.com/KWR-Water/wadi
 Project-URL: Documentation, http://wadi.readthedocs.io/en/latest/
 Project-URL: Tracker, https://github.com/KWR-Water/wadi/issues
 Project-URL: Help, https://github.com/KWR-Water/wadi/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # WaDI
 
-![Documentation](https://readthedocs.org/projects/wadi/badge/?version=latest&style=flat)
-![Pypi packaging](https://github.com/KWR-Water/wadi/actions/workflows/python-package.yml/badge.svg)
+[![Documentation](https://readthedocs.org/projects/wadi/badge/?version=latest&style=flat)](https://wadi.readthedocs.io/en/latest/#)
+[![Pypi packaging](https://github.com/KWR-Water/wadi/actions/workflows/python-package.yml/badge.svg)](https://github.com/KWR-Water/wadi/actions/workflows/python-package.yml)
 
 WaDI is a very generic importer for (almost) all (excel) formats in which water quality data of the (Dutch) water
 laboratory is shared
 
 
 ## Installation
```

### Comparing `wadi-0.1.3/README.md` & `wadi-0.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # WaDI
 
-![Documentation](https://readthedocs.org/projects/wadi/badge/?version=latest&style=flat)
-![Pypi packaging](https://github.com/KWR-Water/wadi/actions/workflows/python-package.yml/badge.svg)
+[![Documentation](https://readthedocs.org/projects/wadi/badge/?version=latest&style=flat)](https://wadi.readthedocs.io/en/latest/#)
+[![Pypi packaging](https://github.com/KWR-Water/wadi/actions/workflows/python-package.yml/badge.svg)](https://github.com/KWR-Water/wadi/actions/workflows/python-package.yml)
 
 WaDI is a very generic importer for (almost) all (excel) formats in which water quality data of the (Dutch) water
 laboratory is shared
 
 
 ## Installation
```

### Comparing `wadi-0.1.3/setup.py` & `wadi-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,44 +3,48 @@
 
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 setup(
     name='wadi',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(exclude=['tests*']),
     license='MIT',
     description='Generic importer for water quality data of the (Dutch) water laboratory',
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Other Audience',
         'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Hydrology',
     ],
-    python_requires='>=3.9',
+    python_requires='>=3.8',
     project_urls={
     'Source': 'https://github.com/KWR-Water/wadi',
     'Documentation': 'http://wadi.readthedocs.io/en/latest/',
     'Tracker': 'https://github.com/KWR-Water/wadi/issues',
     'Help': 'https://github.com/KWR-Water/wadi/issues'
     },
     install_requires=[
-        'pandas>=0.23',
+        'pandas>=1,<2',
         'pint',
         'requests',
         'molmass',
         'openpyxl>=3.0.0',
-        'googletrans',
-        'fuzzywuzzy'
+        'googletrans==3.1.0a0',
+        'fuzzywuzzy',
+        'levenshtein>=0.20.9',
+        'python-Levenshtein>=0.20.9',
+        'requests'
         ],
     include_package_data=True,
     url='https://github.com/KWR-Water/wadi',
     author='KWR Water Research Institute',
     author_email='martin.korevaar@kwrwater.nl, martin.van.der.schans@kwrwater.nl',
 )
```

### Comparing `wadi-0.1.3/wadi/api_utils.py` & `wadi-0.1.4/wadi/api_utils.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.3/wadi/base.py` & `wadi-0.1.4/wadi/base.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.3/wadi/dataobject.py` & `wadi-0.1.4/wadi/dataobject.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.3/wadi/documentation_helpers.py` & `wadi-0.1.4/wadi/documentation_helpers.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.3/wadi/filereader.py` & `wadi-0.1.4/wadi/filereader.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     def __call__(
         self,
         file_path,
         format="stacked",  # str, immutable
         c_dict=None,
         mask=None,
         lod_column=None,
+        extract_units_from_feature_name=False,
         pd_reader="read_excel",  # str, immutable
         **kwargs,
     ):
 
         """
         This method provides an interface for the user to set the
         attributes that determine the FileReader object behavior.
@@ -79,22 +80,25 @@
             Default: None
         lod_column : str, optional
             Name of the column that contains information about whether the 
             reported measurement value is below or above the limit of 
             detection (LOD). If a valid column name is specified, the
             symbol is prefixed to the measurement value.
             Only used when the format is 'stacked'. Default: None
+        extract_units_from_feature_name : bool
+            Indicates if the feature name also contains the units. Default:
+            False
         pd_reader : str, optional
             Name of the Pandas function to read the file. Must be a valid
             function name. While all functions implemented in Pandas could
             be used in principle, the design of WaDI has not been tested
             for functions other than read_excel and read_csv. Default:
             'read_excel'.
-        **kwargs: dict, optionalt
-            Dictionary with kwargs for the 'pdt_retader' function. The
+        **kwargs: dict, optional
+            Dictionary with kwargs for the 'pd_reader' function. The
             kwargs can be a mix of WaDI specific keywords and valid
             keyword arguments for the 'pd_reader' function.
         """
 
         self._file_path = file_path
         self._pd_reader = pd_reader
 
@@ -107,14 +111,15 @@
 
         # Use c_dict to look up the names of the columns with the compulsory
         # names for stacked data.
         self._c_dict = c_dict or DEFAULT_C_DICT
 
         self._mask = mask
         self._lod_column = lod_column
+        self._extract_units_from_feature_name = extract_units_from_feature_name
 
         self._kwargs = copy.deepcopy(vars()["kwargs"])  # deepcopy just to be sure
 
     def _execute(self):
         """
         This method imports the data from a file format readable by
         Pandas. Before calling the Pandas reader function, it checks
@@ -170,14 +175,15 @@
         # data type)
         infotable = InfoTable(
             df,
             self._format,
             self._c_dict,
             units,
             datatypes,
+            self._extract_units_from_feature_name,
         )
 
         # Write the __str__ representation of the InfoTable to the
         # log file.
         self._log(infotable)
 
         # Write the log string to the log file
```

### Comparing `wadi-0.1.3/wadi/harmonizer.py` & `wadi-0.1.4/wadi/harmonizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,18 @@
 
         # Use the regex split function to split the string. A cell value
         # like <0.5 will be parsed into the following list ['', '<', '0.5'].
         substrings = re.split(self._bd_RE, v)
         # Check if there are three substrings
         if len(substrings) == 3:
             # Convert the third substring to a float and apply the uc_factor.
-            rv = float(substrings[2].replace(self._decimal_str, ".")) * conversion_factor
+            try:
+                rv = float(substrings[2].replace(self._decimal_str, ".")) * conversion_factor
+            except ValueError:
+                rv = substrings[2]
             # Prefix the smaller-than symbol without any leading and
             # only a single trailing space and return as a string.
             return f"{substrings[1].strip()} {rv}"
         # If the split function returned only one value it can be a number.
         # In that case try to convert the substring to a float and return
         # it after applying the conversion factor.
         elif len(substrings) == 1:
```

### Comparing `wadi-0.1.3/wadi/infotable.py` & `wadi-0.1.4/wadi/infotable.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from collections import UserDict
 import pandas as pd
 import re
 
+from wadi.utils import parse_name_and_units
+
 DICT_KEYS = ['name', 
              'unit', 
              'values',
              'sampleids', # Only for stacked 
              'datatype',
              'alias_n',
              'alias_u',
@@ -32,14 +34,15 @@
 
     def __init__(self,
         df,
         format,
         c_dict,
         units, 
         datatypes,
+        extract_units_from_feature_name,
         ):
         """
         Initialization method. Creates a nested dict with information
         about the imported data.
 
         Parameters
         ----------
@@ -57,14 +60,16 @@
             list is created by the '_read_file' function based on the unit_row
             kwarg passed by the user to read_data.
         datatypes : list of strings
             List with the datatype for each feature (or sampleinfo data). This
             list is created by the '_read_file' function based on the datatype
             kwarg passed by the user to read_data. Datatypes must all 
             be in VALID_DATATYPES.
+        extract_units_from_feature_name : bool
+            Indicates if the feature name also contains the units.
         """
 
         # Use the c_dict to identify the names of the columns with
         # the sampleids, the features (either sample information 
         # like location or the name of a chemical substance), the
         # units and the measurement values.
         if (format == 'stacked'):
@@ -86,34 +91,42 @@
             ufus = (df[col_f] + df[col_u].fillna('')).dropna().unique()
             for fu in ufus:
                 # Select a unique feature + unit combination
                 idx = (df[col_f] + df[col_u].fillna('') == fu)
                 # Set the key in the infotable to the first element in the
                 # feature name column (all values in the column will be equal)
                 key_0 = df.loc[idx, col_f].iloc[0]
+                feature_name = key_0
+                units_str = df.loc[idx, col_u].iloc[0]
+                if extract_units_from_feature_name == True:
+                    feature_name, units_str = parse_name_and_units(feature_name)
+                    
                 # Define the dictionary with the required data
-                dict_1 = {'name': key_0,
-                          'unit': df.loc[idx, col_u].iloc[0], 
+                dict_1 = {'name': feature_name,
+                          'unit': units_str, 
                           'sampleids': df.loc[idx, col_s],
                           'values': df.loc[idx, col_v],
                           'datatype': 'feature'}
                 # Add dict_1 to the info_table
                 dict_0[key_0] = dict_1
         elif (format == 'wide'):
             # Iterate over the columns in the DataFrame
             for i, key_0 in enumerate(df.columns):
                 # Pandas adds a dot followed by a number for duplicate columns
                 # so to get the real feature name, it must be removed
-                col_name = key_0
-                duplicate_nr = re.search('\.\d+$', col_name)
+                feature_name = key_0
+                duplicate_nr = re.search('\.\d+$', feature_name)
                 if duplicate_nr:
-                    col_name = col_name.removesuffix(duplicate_nr.group()) # Requires Python 3.9 or later
+                    feature_name = feature_name[:-len(duplicate_nr.group())]
+                units_str = units[i]
+                if extract_units_from_feature_name == True:
+                    feature_name, units_str = parse_name_and_units(feature_name)
                 # Define the dictionary with the required data
-                dict_1 = {'name': col_name,
-                          'unit': units[i], 
+                dict_1 = {'name': feature_name,
+                          'unit': units_str, 
                           'values': df[key_0],
                           'datatype': datatypes[i]}
                 # Add dict_1 to the info_table
                 dict_0[key_0] = dict_1
 
         # Add aliases to ensure an alias is always defined, 
         # even if mapping does not result in any match.
```

### Comparing `wadi-0.1.3/wadi/mapper.py` & `wadi-0.1.4/wadi/mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,17 +120,17 @@
             An instance of the UserDict class containing the
             imported data.
         """
         # The json file resides in the parent directory of the
         # current module's py file. The __file__ attribute returns
         # the pathname of the current py file and .parent
         # provides its parent directory.
-        filepath = Path(__file__).parent
+        filepath = Path(__file__).resolve().parent
         # Import the file into a DataFrame.
-        dfj = pd.read_json(Path(filepath, "default_feature_map.json"))
+        dfj = pd.read_json(Path(filepath, "mapping_data", "default_feature_map.json"))
         # Use the DataFrame's explode function to transform any keys
         # that are a list (or list-like) into a row. The corresponding
         # value is duplicated for each list element that becomes a row.
         dfd = dfj[[keys, values]].explode(keys).dropna()
         # Convert the DataFrame to a dictionary
         rv_dict = dfd.set_index(keys)[values].to_dict()
         # Values are lists, gives problems when they become aliases so
@@ -149,17 +149,17 @@
         ----------
         result : class instance
             An instance of the UserDict class containing the
             imported data.
         """
 
         rv_dict = {}
-        filepath = Path(Path(__file__).parents[1], "hgc_constants")
+        filepath = Path(__file__).resolve().parent
         for fname in ["atoms.csv", "ions.csv", "other_than_concentrations.csv"]:
-            df = pd.read_csv(Path(filepath, fname), comment='#')
+            df = pd.read_csv(Path(filepath, "mapping_data", fname), comment='#')
             rv_dict = {**rv_dict, **df.set_index("feature")["unit"].to_dict()}
 
         return cls(rv_dict)
 
     @classmethod
     def pubchem_cas_dict(
         cls,
```

### Comparing `wadi-0.1.3/wadi/unitconverter.py` & `wadi-0.1.4/wadi/unitconverter.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.3/wadi/utils.py` & `wadi-0.1.4/wadi/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections import UserList
 import inspect
 import re
 
 import numpy as np
 
-DEFAULT_FUZZY_MINSCORES = {1: 100, 3: 100, 4: 90, 5: 85, 6: 80, 8: 75}
+# DEFAULT_FUZZY_MINSCORES = {1: 100, 3: 100, 4: 90, 5: 85, 6: 80, 8: 75}
+DEFAULT_FUZZY_MINSCORES = {1: 100, 3: 100, 4: 90, 5: 85, 6: 80}
 
 
 def check_arg(arg, valid_args):
     """
     Function that checks if an argument is an element of a list of valid
     arguments.
 
@@ -101,14 +102,62 @@
                 if len(l) < min_elements:
                     raise ValueError(error_msg)
             else:
                 raise TypeError(error_msg)
     else:
         raise TypeError("Expected a nested list")
 
+def parse_name_and_units(s):
+    """
+    This function attempts to extract the feature name and units from 
+    a string. It tries to split the string at the first space character.
+    The first item before the space is the feature name (verbatim). If
+    the part after the space contains any parentheses, brackets or accolades
+    these are stripped off and the remaining part is considered to contain
+    the units. For example, it will correctly recognize the following 
+    formats: 'Ca', 'Mg mg/l', 'Na (mg/l)', 'NO3 [mg N/l]', 'SO4 {mg/l S}'.
+    The units for 'Ca tot mg/l' will be incorrectly inferred because the
+    string contains two spaces.
+
+    Parameters
+    ----------
+    s : str
+        A string from which the name and units must be extracted.
+
+    Returns
+    -------
+    name : str
+        The feature name extracted from 's'. For the example strings above, 
+        the resulting names will be 'Ca', 'Mg', 'Na', 'NO3', 'SO4' and 'Ca'.
+    units: str
+        The units extracted from 's'. For the example strings above, the 
+        corresponding units will be '', 'mg/l', 'mg/l', 'mg N/l', 
+        'mg/l S' and 'tot mg/l'.
+    """
+
+    # Split string at the first space.
+    split_str = s.split(sep=None, maxsplit=1)
+    # If the string contains no space separator the
+    # string is considered to be the feature name. An
+    # empty string is returned for the units.
+    if len(split_str) == 1:
+        return split_str[0], ""
+    # If the string was sucessfully split, the
+    # first list element is considered to be the 
+    # feature name, the second the units.
+    elif len(split_str) == 2:
+        # Use a regular expression to strip off any
+        # parentheses, brackets or accolades from the
+        # string with the units.
+        return split_str[0], re.sub("[\(\)\[\]\{\}]", "", split_str[1])
+    
+    # For empty strings the list returned by the split
+    # function will be empty. Return empty strings for
+    # both name and units in that case.
+    return "", ""
 
 class StringList(UserList):
     """
     Class with convenience methods for lists of strings.
     """
     def __init__(self, initlist=None):
         """
```

### Comparing `wadi-0.1.3/wadi.egg-info/PKG-INFO` & `wadi-0.1.4/wadi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: wadi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generic importer for water quality data of the (Dutch) water laboratory
 Home-page: https://github.com/KWR-Water/wadi
 Author: KWR Water Research Institute
 Author-email: martin.korevaar@kwrwater.nl, martin.van.der.schans@kwrwater.nl
 License: MIT
 Project-URL: Source, https://github.com/KWR-Water/wadi
 Project-URL: Documentation, http://wadi.readthedocs.io/en/latest/
 Project-URL: Tracker, https://github.com/KWR-Water/wadi/issues
 Project-URL: Help, https://github.com/KWR-Water/wadi/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # WaDI
 
-![Documentation](https://readthedocs.org/projects/wadi/badge/?version=latest&style=flat)
-![Pypi packaging](https://github.com/KWR-Water/wadi/actions/workflows/python-package.yml/badge.svg)
+[![Documentation](https://readthedocs.org/projects/wadi/badge/?version=latest&style=flat)](https://wadi.readthedocs.io/en/latest/#)
+[![Pypi packaging](https://github.com/KWR-Water/wadi/actions/workflows/python-package.yml/badge.svg)](https://github.com/KWR-Water/wadi/actions/workflows/python-package.yml)
 
 WaDI is a very generic importer for (almost) all (excel) formats in which water quality data of the (Dutch) water
 laboratory is shared
 
 
 ## Installation
```

