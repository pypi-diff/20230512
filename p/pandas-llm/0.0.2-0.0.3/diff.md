# Comparing `tmp/pandas_llm-0.0.2.tar.gz` & `tmp/pandas_llm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_llm-0.0.2.tar", last modified: Fri May 12 08:27:42 2023, max compression
+gzip compressed data, was "pandas_llm-0.0.3.tar", last modified: Fri May 12 08:48:26 2023, max compression
```

## Comparing `pandas_llm-0.0.2.tar` & `pandas_llm-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-05-12 08:27:42.081392 pandas_llm-0.0.2/
--rw-r--r--   0 alessioricco   (501) staff       (20)     1068 2023-05-11 12:07:22.000000 pandas_llm-0.0.2/LICENSE
--rw-r--r--   0 alessioricco   (501) staff       (20)     2552 2023-05-12 08:27:42.081480 pandas_llm-0.0.2/PKG-INFO
--rw-r--r--   0 alessioricco   (501) staff       (20)     1735 2023-05-11 22:18:20.000000 pandas_llm-0.0.2/README.md
-drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-05-12 08:27:42.080373 pandas_llm-0.0.2/pandas_llm/
--rw-r--r--   0 alessioricco   (501) staff       (20)       32 2023-05-11 15:03:14.000000 pandas_llm-0.0.2/pandas_llm/__init__.py
--rw-r--r--   0 alessioricco   (501) staff       (20)     2511 2023-05-11 15:38:43.000000 pandas_llm-0.0.2/pandas_llm/example-chatbot.py
--rw-r--r--   0 alessioricco   (501) staff       (20)      902 2023-05-11 16:51:08.000000 pandas_llm-0.0.2/pandas_llm/example.py
--rw-r--r--   0 alessioricco   (501) staff       (20)     7081 2023-05-11 21:57:26.000000 pandas_llm-0.0.2/pandas_llm/pandas_llm.py
--rw-r--r--   0 alessioricco   (501) staff       (20)     1967 2023-05-11 12:28:50.000000 pandas_llm-0.0.2/pandas_llm/sandbox.py
-drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-05-12 08:27:42.081257 pandas_llm-0.0.2/pandas_llm.egg-info/
--rw-r--r--   0 alessioricco   (501) staff       (20)     2552 2023-05-12 08:27:42.000000 pandas_llm-0.0.2/pandas_llm.egg-info/PKG-INFO
--rw-r--r--   0 alessioricco   (501) staff       (20)      327 2023-05-12 08:27:42.000000 pandas_llm-0.0.2/pandas_llm.egg-info/SOURCES.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)        1 2023-05-12 08:27:42.000000 pandas_llm-0.0.2/pandas_llm.egg-info/dependency_links.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)      341 2023-05-12 08:27:42.000000 pandas_llm-0.0.2/pandas_llm.egg-info/requires.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)       11 2023-05-12 08:27:42.000000 pandas_llm-0.0.2/pandas_llm.egg-info/top_level.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)       79 2023-05-12 08:27:42.081776 pandas_llm-0.0.2/setup.cfg
--rw-r--r--   0 alessioricco   (501) staff       (20)     2189 2023-05-12 08:27:30.000000 pandas_llm-0.0.2/setup.py
+drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-05-12 08:48:26.398585 pandas_llm-0.0.3/
+-rw-r--r--   0 alessioricco   (501) staff       (20)     1068 2023-05-11 12:07:22.000000 pandas_llm-0.0.3/LICENSE
+-rw-r--r--   0 alessioricco   (501) staff       (20)     2552 2023-05-12 08:48:26.398689 pandas_llm-0.0.3/PKG-INFO
+-rw-r--r--   0 alessioricco   (501) staff       (20)     1735 2023-05-12 08:44:14.000000 pandas_llm-0.0.3/README.md
+drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-05-12 08:48:26.397087 pandas_llm-0.0.3/pandas_llm/
+-rw-r--r--   0 alessioricco   (501) staff       (20)       32 2023-05-11 15:03:14.000000 pandas_llm-0.0.3/pandas_llm/__init__.py
+-rw-r--r--   0 alessioricco   (501) staff       (20)     2511 2023-05-11 15:38:43.000000 pandas_llm-0.0.3/pandas_llm/example-chatbot.py
+-rw-r--r--   0 alessioricco   (501) staff       (20)      902 2023-05-11 16:51:08.000000 pandas_llm-0.0.3/pandas_llm/example.py
+-rw-r--r--   0 alessioricco   (501) staff       (20)     7081 2023-05-11 21:57:26.000000 pandas_llm-0.0.3/pandas_llm/pandas_llm.py
+-rw-r--r--   0 alessioricco   (501) staff       (20)     1967 2023-05-11 12:28:50.000000 pandas_llm-0.0.3/pandas_llm/sandbox.py
+drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-05-12 08:48:26.398443 pandas_llm-0.0.3/pandas_llm.egg-info/
+-rw-r--r--   0 alessioricco   (501) staff       (20)     2552 2023-05-12 08:48:26.000000 pandas_llm-0.0.3/pandas_llm.egg-info/PKG-INFO
+-rw-r--r--   0 alessioricco   (501) staff       (20)      327 2023-05-12 08:48:26.000000 pandas_llm-0.0.3/pandas_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)        1 2023-05-12 08:48:26.000000 pandas_llm-0.0.3/pandas_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)      187 2023-05-12 08:48:26.000000 pandas_llm-0.0.3/pandas_llm.egg-info/requires.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)       11 2023-05-12 08:48:26.000000 pandas_llm-0.0.3/pandas_llm.egg-info/top_level.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)       79 2023-05-12 08:48:26.399041 pandas_llm-0.0.3/setup.cfg
+-rw-r--r--   0 alessioricco   (501) staff       (20)     2035 2023-05-12 08:46:42.000000 pandas_llm-0.0.3/setup.py
```

### Comparing `pandas_llm-0.0.2/LICENSE` & `pandas_llm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_llm-0.0.2/PKG-INFO` & `pandas_llm-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pandas_llm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Conversational Pandas Dataframes
 Home-page: https://github.com/DashyDashOrg/pandas-llm
-Download-URL: https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.2
+Download-URL: https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.3
 Author: DashyDash
 Author-email: alessio@dashydash.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/DashyDashOrg/pandas-llm/issues
 Keywords: pypi,pandas-llm,pandas,llm,ai,openai,chatgpt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 pandas-llm is a lightweight Python library that extends pandas to allow querying datasets using OpenAI prompts. This powerful tool leverages the natural language processing capabilities of OpenAI to offer intuitive, language-based querying of your pandas dataframes.
 
 ## Installation
 
 Install pandas-llm using pip:
 
 ```shell
-pip install pandas_llm
+pip install pandas-llm
 ```
 
 ## Features
 - Query pandas dataframes using natural language prompts.
 - Leverage the power of OpenAI's language models in your data analysis.
 - Seamless integration with existing pandas functions.
```

### Comparing `pandas_llm-0.0.2/README.md` & `pandas_llm-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pandas-llm is a lightweight Python library that extends pandas to allow querying datasets using OpenAI prompts. This powerful tool leverages the natural language processing capabilities of OpenAI to offer intuitive, language-based querying of your pandas dataframes.
 
 ## Installation
 
 Install pandas-llm using pip:
 
 ```shell
-pip install pandas_llm
+pip install pandas-llm
 ```
 
 ## Features
 - Query pandas dataframes using natural language prompts.
 - Leverage the power of OpenAI's language models in your data analysis.
 - Seamless integration with existing pandas functions.
```

### Comparing `pandas_llm-0.0.2/pandas_llm/example-chatbot.py` & `pandas_llm-0.0.3/pandas_llm/example-chatbot.py`

 * *Files identical despite different names*

### Comparing `pandas_llm-0.0.2/pandas_llm/example.py` & `pandas_llm-0.0.3/pandas_llm/example.py`

 * *Files identical despite different names*

### Comparing `pandas_llm-0.0.2/pandas_llm/pandas_llm.py` & `pandas_llm-0.0.3/pandas_llm/pandas_llm.py`

 * *Files identical despite different names*

### Comparing `pandas_llm-0.0.2/pandas_llm/sandbox.py` & `pandas_llm-0.0.3/pandas_llm/sandbox.py`

 * *Files identical despite different names*

### Comparing `pandas_llm-0.0.2/pandas_llm.egg-info/PKG-INFO` & `pandas_llm-0.0.3/pandas_llm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pandas-llm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Conversational Pandas Dataframes
 Home-page: https://github.com/DashyDashOrg/pandas-llm
-Download-URL: https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.2
+Download-URL: https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.3
 Author: DashyDash
 Author-email: alessio@dashydash.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/DashyDashOrg/pandas-llm/issues
 Keywords: pypi,pandas-llm,pandas,llm,ai,openai,chatgpt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 pandas-llm is a lightweight Python library that extends pandas to allow querying datasets using OpenAI prompts. This powerful tool leverages the natural language processing capabilities of OpenAI to offer intuitive, language-based querying of your pandas dataframes.
 
 ## Installation
 
 Install pandas-llm using pip:
 
 ```shell
-pip install pandas_llm
+pip install pandas-llm
 ```
 
 ## Features
 - Query pandas dataframes using natural language prompts.
 - Leverage the power of OpenAI's language models in your data analysis.
 - Seamless integration with existing pandas functions.
```

### Comparing `pandas_llm-0.0.2/setup.py` & `pandas_llm-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pandas_llm',                           # should match the package folder
-    version='0.0.2',                                # important for updates
+    version='0.0.3',                                # important for updates
     license='MIT',                                  # should match your chosen license
     description='Conversational Pandas Dataframes',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='DashyDash',
     author_email='alessio@dashydash.com',
     url='https://github.com/DashyDashOrg/pandas-llm', 
@@ -25,31 +25,31 @@
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
-        "aiohttp>=3.8.4",
-        "aiosignal>=1.3.1",
-        "async-timeout>=4.0.2",
-        "attrs>=23.1.0",
-        "certifi>=2023.5.7",
-        "charset-normalizer>=3.1.0",
-        "frozenlist>=1.3.3",
-        "idna>=3.4",
-        "multidict>=6.0.4",
-        "numpy>=1.24.3",
-        "openai>=0.27.6",
-        "pandas>=2.0.1",
-        "python-dateutil>=2.8.2",
-        "pytz>=2023.3",
-        "requests>=2.30.0",
-        "RestrictedPython>=6.0",
-        "six>=1.16.0",
-        "tqdm>=4.65.0",
-        "tzdata>=2023.3",
-        "urllib3>=2.0.2",
-        "yarl>=1.9.2",
+        "aiohttp",
+        "aiosignal",
+        "async-timeout",
+        "attrs",
+        "certifi",
+        "charset-normalizer",
+        "frozenlist",
+        "idna",
+        "multidict",
+        "numpy",
+        "openai",
+        "pandas",
+        "python-dateutil",
+        "pytz",
+        "requests",
+        "RestrictedPython",
+        "six",
+        "tqdm",
+        "tzdata",
+        "urllib3",
+        "yarl",
     ],   
-    download_url="https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.2",
+    download_url="https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.3",
 )
```

