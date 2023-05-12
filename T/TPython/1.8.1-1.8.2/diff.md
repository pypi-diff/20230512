# Comparing `tmp/TPython-1.8.1-py2.py3-none-any.whl.zip` & `tmp/TPython-1.8.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8490 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat       68 b- defN 23-May-08 16:50 tpy/__init__.py
+Zip file size: 8493 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat       64 b- defN 23-May-12 17:15 tpy/__init__.py
 -rw-rw-rw-  2.0 fat       31 b- defN 23-Feb-20 17:02 tpy/__main__.py
 -rw-rw-rw-  2.0 fat     3961 b- defN 23-May-07 11:56 tpy/config.py
 -rw-rw-rw-  2.0 fat      903 b- defN 23-May-07 11:40 tpy/jsonc.py
--rw-rw-rw-  2.0 fat    12048 b- defN 23-May-08 16:50 tpy/tpy.py
--rw-rw-rw-  2.0 fat     1062 b- defN 23-May-08 16:51 TPython-1.8.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2482 b- defN 23-May-08 16:51 TPython-1.8.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-08 16:51 TPython-1.8.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       37 b- defN 23-May-08 16:51 TPython-1.8.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        4 b- defN 23-May-08 16:51 TPython-1.8.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      827 b- defN 23-May-08 16:51 TPython-1.8.1.dist-info/RECORD
-11 files, 21533 bytes uncompressed, 7104 bytes compressed:  67.0%
+-rw-rw-rw-  2.0 fat    12054 b- defN 23-May-12 17:15 tpy/tpy.py
+-rw-rw-rw-  2.0 fat     1062 b- defN 23-May-12 17:16 TPython-1.8.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2482 b- defN 23-May-12 17:16 TPython-1.8.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-12 17:16 TPython-1.8.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       37 b- defN 23-May-12 17:16 TPython-1.8.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        4 b- defN 23-May-12 17:16 TPython-1.8.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      827 b- defN 23-May-12 17:16 TPython-1.8.2.dist-info/RECORD
+11 files, 21535 bytes uncompressed, 7107 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: tpy/jsonc.py
 Comment: 
 
 Filename: tpy/tpy.py
 Comment: 
 
-Filename: TPython-1.8.1.dist-info/LICENSE
+Filename: TPython-1.8.2.dist-info/LICENSE
 Comment: 
 
-Filename: TPython-1.8.1.dist-info/METADATA
+Filename: TPython-1.8.2.dist-info/METADATA
 Comment: 
 
-Filename: TPython-1.8.1.dist-info/WHEEL
+Filename: TPython-1.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: TPython-1.8.1.dist-info/entry_points.txt
+Filename: TPython-1.8.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: TPython-1.8.1.dist-info/top_level.txt
+Filename: TPython-1.8.2.dist-info/top_level.txt
 Comment: 
 
-Filename: TPython-1.8.1.dist-info/RECORD
+Filename: TPython-1.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tpy/__init__.py

```diff
@@ -1,4 +1,4 @@
 from .tpy import main
 
 __all__ = ['main']
-__version__ = '1.8.1'
+VERSION = '1.8.2'
```

## tpy/tpy.py

```diff
@@ -19,25 +19,25 @@
     sys.exit('Module not found: colorama')
 
 # Vars
 cell_number: int = 1
 err: bool = False
 ind: bool = False
 namespace: dict = {'__builtins__': __builtins__, '__name__': '__main__', '__doc__': 'Automatically created module for TPython interactive environment', '__package__': None, '__loader__': None, '__spec__': None, '__annotations__': {}}
-VERSION: str = '1.8'
+VERSION: str = '1.8.2'
 
 # Exception prettifier
 def exc() -> None:
     name, value = sys.exc_info()[0:2] # type: ignore
     name: str = name.__name__ # type: ignore
     top_bar = "----------------------------------------------------------------------" if os.get_terminal_size().columns > 70 else "-"*os.get_terminal_size().columns
     if name == 'SyntaxError':
         line: str = value.args[1][3] # type: ignore
         err_highlight: str = ' '*(value.offset - 1) + ('^'*(value.end_offset - value.offset) if value.end_offset - value.offset != 0 else '^') # type: ignore
-        value: = value.args[0] # type: ignore
+        value: str = value.args[0] # type: ignore
         if line.endswith('\n'):
             line = line.removesuffix('\n')
         exc: str = f'{Fore.LIGHTGREEN_EX}{top_bar}\n{Fore.LIGHTRED_EX}{name} {Fore.LIGHTGREEN_EX}in Cell {Fore.GREEN}{cell_number}\n{Fore.RESET}{line}\n{err_highlight}\n\n{Fore.LIGHTRED_EX}{name}{Fore.RESET}: {value}'
     else:
         exc: str = f'{Fore.LIGHTGREEN_EX}{top_bar}\n{Fore.LIGHTRED_EX}{name} {Fore.LIGHTGREEN_EX}in Cell {Fore.GREEN}{cell_number}{(len(top_bar)-len(name)-len(str(cell_number))-42)*" "}Traceback (most recent call last)\n\n{Fore.LIGHTRED_EX}{name}{Fore.RESET}: {value}'
     print(exc)
```

## Comparing `TPython-1.8.1.dist-info/LICENSE` & `TPython-1.8.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `TPython-1.8.1.dist-info/METADATA` & `TPython-1.8.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TPython
-Version: 1.8.1
+Version: 1.8.2
 Summary: A better python REPL
 Home-page: https://github.com/Techlord210/TPython
 Author: Techlord210
 Author-email: techlord210@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

