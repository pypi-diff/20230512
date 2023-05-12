# Comparing `tmp/promptlayer-0.1.80.tar.gz` & `tmp/promptlayer-0.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/promptlayer-0.1.80.tar", last modified: Fri Mar 31 18:03:30 2023, max compression
+gzip compressed data, was "dist/promptlayer-0.1.81.tar", last modified: Fri May 12 18:11:38 2023, max compression
```

## Comparing `promptlayer-0.1.80.tar` & `promptlayer-0.1.81.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-03-31 18:03:30.693754 promptlayer-0.1.80/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.80/LICENSE
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-03-31 18:03:30.693467 promptlayer-0.1.80/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.80/README.md
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-03-31 18:03:30.687587 promptlayer-0.1.80/promptlayer/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      341 2023-03-13 20:43:03.000000 promptlayer-0.1.80/promptlayer/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-03-31 18:03:30.690037 promptlayer-0.1.80/promptlayer/langchain/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.80/promptlayer/langchain/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-03-31 18:03:30.690765 promptlayer-0.1.80/promptlayer/langchain/llms/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.80/promptlayer/langchain/llms/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.80/promptlayer/langchain/llms/openai.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2689 2023-03-27 21:24:30.000000 promptlayer-0.1.80/promptlayer/promptlayer.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-03-31 18:03:30.691742 promptlayer-0.1.80/promptlayer/prompts/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.80/promptlayer/prompts/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1285 2023-03-31 18:02:42.000000 promptlayer-0.1.80/promptlayer/prompts/prompts.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-03-31 18:03:30.692576 promptlayer-0.1.80/promptlayer/track/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.80/promptlayer/track/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      945 2023-03-31 18:02:42.000000 promptlayer-0.1.80/promptlayer/track/track.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    12965 2023-03-31 18:02:42.000000 promptlayer-0.1.80/promptlayer/utils.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-03-31 18:03:30.689711 promptlayer-0.1.80/promptlayer.egg-info/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-03-31 18:03:30.000000 promptlayer-0.1.80/promptlayer.egg-info/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      502 2023-03-31 18:03:30.000000 promptlayer-0.1.80/promptlayer.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-03-31 18:03:30.000000 promptlayer-0.1.80/promptlayer.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-03-31 18:03:30.000000 promptlayer-0.1.80/promptlayer.egg-info/requires.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-03-31 18:03:30.000000 promptlayer-0.1.80/promptlayer.egg-info/top_level.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-03-31 18:03:30.693863 promptlayer-0.1.80/setup.cfg
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      832 2023-03-31 18:02:50.000000 promptlayer-0.1.80/setup.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.661507 promptlayer-0.1.81/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.81/LICENSE
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-12 18:11:38.661229 promptlayer-0.1.81/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.81/README.md
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.655578 promptlayer-0.1.81/promptlayer/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      341 2023-03-13 20:43:03.000000 promptlayer-0.1.81/promptlayer/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.658336 promptlayer-0.1.81/promptlayer/langchain/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.81/promptlayer/langchain/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.659003 promptlayer-0.1.81/promptlayer/langchain/llms/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.81/promptlayer/langchain/llms/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.81/promptlayer/langchain/llms/openai.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2689 2023-03-27 21:24:30.000000 promptlayer-0.1.81/promptlayer/promptlayer.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.659679 promptlayer-0.1.81/promptlayer/prompts/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.81/promptlayer/prompts/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1285 2023-03-31 18:02:42.000000 promptlayer-0.1.81/promptlayer/prompts/prompts.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.660711 promptlayer-0.1.81/promptlayer/track/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.81/promptlayer/track/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.81/promptlayer/track/track.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    12965 2023-03-31 18:02:42.000000 promptlayer-0.1.81/promptlayer/utils.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.657969 promptlayer-0.1.81/promptlayer.egg-info/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-12 18:11:38.000000 promptlayer-0.1.81/promptlayer.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      502 2023-05-12 18:11:38.000000 promptlayer-0.1.81/promptlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-05-12 18:11:38.000000 promptlayer-0.1.81/promptlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-05-12 18:11:38.000000 promptlayer-0.1.81/promptlayer.egg-info/requires.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-05-12 18:11:38.000000 promptlayer-0.1.81/promptlayer.egg-info/top_level.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-05-12 18:11:38.661613 promptlayer-0.1.81/setup.cfg
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      832 2023-05-12 18:11:05.000000 promptlayer-0.1.81/setup.py
```

### Comparing `promptlayer-0.1.80/LICENSE` & `promptlayer-0.1.81/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.80/PKG-INFO` & `promptlayer-0.1.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.80
+Version: 0.1.81
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.80 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.81 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.80/README.md` & `promptlayer-0.1.81/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.80/promptlayer/langchain/llms/openai.py` & `promptlayer-0.1.81/promptlayer/langchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.80/promptlayer/promptlayer.py` & `promptlayer-0.1.81/promptlayer/promptlayer.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.80/promptlayer/prompts/prompts.py` & `promptlayer-0.1.81/promptlayer/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.80/promptlayer/utils.py` & `promptlayer-0.1.81/promptlayer/utils.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.80/promptlayer.egg-info/PKG-INFO` & `promptlayer-0.1.81/promptlayer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.80
+Version: 0.1.81
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.80 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.81 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.80/setup.py` & `promptlayer-0.1.81/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,12 +13,12 @@
     description="PromptLayer is a package to keep track of your GPT models training",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Magniv",
     author_email="hello@magniv.io",
     url="https://www.promptlayer.com",
     project_urls={"Documentation": "https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629",},
-    version="0.1.80",
+    version="0.1.81",
     py_modules=["promptlayer"],
     packages=find_packages(),
     install_requires=["requests", "openai", "langchain"],
 )
```

