# Comparing `tmp/columbo-0.13.0.post1.tar.gz` & `tmp/columbo-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "columbo-0.13.0.post1.tar", last modified: Fri May 12 20:28:23 2023, max compression
+gzip compressed data, was "dist/columbo-0.9.0.tar", last modified: Fri Dec 18 19:55:18 2020, max compression
```

## Comparing `columbo-0.13.0.post1.tar` & `columbo-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:23.353845 columbo-0.13.0.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-12 20:28:23.353845 columbo-0.13.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:23.353845 columbo-0.13.0.post1/columbo/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/columbo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/columbo/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/columbo/_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    30990 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/columbo/_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/columbo/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/columbo/_user_io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/columbo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:23.353845 columbo-0.13.0.post1/columbo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-12 20:28:23.000000 columbo-0.13.0.post1/columbo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-12 20:28:23.000000 columbo-0.13.0.post1/columbo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:28:23.000000 columbo-0.13.0.post1/columbo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 20:28:23.000000 columbo-0.13.0.post1/columbo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 20:28:23.000000 columbo-0.13.0.post1/columbo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-12 20:28:23.353845 columbo-0.13.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:23.353845 columbo-0.13.0.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/tests/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/tests/exception_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21780 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/tests/interaction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/tests/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-12 20:28:12.000000 columbo-0.13.0.post1/tests/user_io_test.py
+drwxrwxr-x   0 patrick   (1001) patrick   (1000)        0 2020-12-18 19:55:18.240258 columbo-0.9.0/
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)       18 2020-08-28 15:10:08.000000 columbo-0.9.0/MANIFEST.in
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)     4701 2020-12-18 19:55:18.240258 columbo-0.9.0/PKG-INFO
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)     3232 2020-12-18 19:54:05.000000 columbo-0.9.0/README.md
+drwxrwxr-x   0 patrick   (1001) patrick   (1000)        0 2020-12-18 19:55:18.236258 columbo-0.9.0/columbo/
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)      720 2020-12-18 19:53:48.000000 columbo-0.9.0/columbo/__init__.py
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)     7456 2020-08-28 15:10:08.000000 columbo-0.9.0/columbo/_cli.py
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)      618 2020-08-28 15:10:08.000000 columbo-0.9.0/columbo/_exception.py
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)    20760 2020-08-28 15:10:08.000000 columbo-0.9.0/columbo/_interaction.py
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)      417 2020-08-28 15:10:08.000000 columbo-0.9.0/columbo/_types.py
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)     3394 2020-08-28 15:10:08.000000 columbo-0.9.0/columbo/_user_io.py
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)        0 2020-10-09 18:44:15.000000 columbo-0.9.0/columbo/py.typed
+drwxrwxr-x   0 patrick   (1001) patrick   (1000)        0 2020-12-18 19:55:18.240258 columbo-0.9.0/columbo.egg-info/
+-rw-r--r--   0 patrick   (1001) patrick   (1000)     4701 2020-12-18 19:55:18.000000 columbo-0.9.0/columbo.egg-info/PKG-INFO
+-rw-r--r--   0 patrick   (1001) patrick   (1000)      336 2020-12-18 19:55:18.000000 columbo-0.9.0/columbo.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick   (1001) patrick   (1000)        1 2020-12-18 19:55:18.000000 columbo-0.9.0/columbo.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick   (1001) patrick   (1000)       20 2020-12-18 19:55:18.000000 columbo-0.9.0/columbo.egg-info/requires.txt
+-rw-r--r--   0 patrick   (1001) patrick   (1000)        8 2020-12-18 19:55:18.000000 columbo-0.9.0/columbo.egg-info/top_level.txt
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)      367 2020-08-28 15:10:08.000000 columbo-0.9.0/pyproject.toml
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)       38 2020-12-18 19:55:18.240258 columbo-0.9.0/setup.cfg
+-rw-rw-r--   0 patrick   (1001) patrick   (1000)     1259 2020-12-18 19:54:05.000000 columbo-0.9.0/setup.py
```

### Comparing `columbo-0.13.0.post1/PKG-INFO` & `columbo-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,173 +1,121 @@
 Metadata-Version: 2.1
 Name: columbo
-Version: 0.13.0.post1
+Version: 0.9.0
 Summary: Specify a dynamic set of questions to ask a user and get their answers.
-Home-page: https://github.com/plannigan/columbo
+Home-page: https://github.com/wayfair-incubator/columbo
 Author: Patrick Lannigan
-Author-email: p.lannigan@gmail.com
+Author-email: plannigan@wayfair.com
+License: UNKNOWN
+Description: [![CI pipeline status](https://github.com/wayfair-incubator/columbo/workflows/CI/badge.svg?branch=main)][ci]
+        [![PyPI](https://img.shields.io/pypi/v/columbo)][pypi]
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/columbo)][pypi]
+        [![codecov](https://codecov.io/gh/wayfair-incubator/columbo/branch/main/graph/badge.svg)][codecov]
+        [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)][mypy-home]
+        [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)][black-home]
+        
+        # Columbo
+        
+        Specify a dynamic set of questions to ask a user and get their answers.
+        
+        `columbo`'s feature set allows a program to:
+        
+        * Ask multiple types of questions:
+            * Yes or No
+            * Multiple choice
+            * Open-ended
+        * Validate the response provided by the user.
+        * Use answers from earlier questions:
+            * As part of the text of a question
+            * As part of the text of a default value
+            * To decide if a question should be skipped
+        * Accept answers from the command line in addition to prompting the user.
+        
+        ## Example
+        
+        ### User Prompts
+        
+        The primary use of `columbo` is to define a sequence of interactions that are used to prompt a user to provide answers
+        using a terminal. Below is a sample which shows some ways this can be used.
+        
+        ```python
+        import columbo
+        
+        interactions = [
+            columbo.Echo("Welcome to the Columbo example"),
+            columbo.Acknowledge(
+                "Press enter to start"
+            ),
+            columbo.BasicQuestion(
+                "user",
+                "What is your name?",
+                default="Patrick",
+            ),
+            columbo.BasicQuestion(
+                "user_email",
+                lambda answers: f"""What email address should be used to contact {answers["user"]}?""",
+                default="me@example.com"
+            ),
+            columbo.Choice(
+                "mood",
+                "How are you feeling today?",
+                options=["happy", "sad", "sleepy", "confused"],
+                default="happy",
+            ),
+            columbo.Confirm("likes_dogs", "Do you like dogs?", default=True),
+        ]
+        
+        answers = columbo.get_answers(interactions)
+        print(answers)
+        ```
+        
+        Below shows the output when the user accepts the default values for most of the questions. The user provides a different
+        value for the email and explicitly confirms that they like dogs.
+        
+        ```text
+        Welcome to the Columbo example
+        Press enter to start
+         
+        What is your name? [Patrick]:
+        
+        What email address should be used to contact Patrick? [me@example.com]: patrick@example.com
+        
+        How are you feeling today?
+        1 - happy
+        2 - sad
+        3 - sleepy
+        4 - confused
+        Enter the number of your choice [1]:
+        
+        Do you like dogs? (Y/n): y
+        
+        {'user': 'Patrick', 'user_email': 'patrick@example.com', 'mood': 'happy', 'likes_dogs': True}
+        ```
+        
+        ### Command Line Answers
+        
+        TODO
+        
+        ## Documentation
+        
+        Check out the [project documentation][columbo-docs].
+        
+        For an overview on how repository structure and how to work with the code base, read the
+        [Development Guide][development-docs].
+        
+        [ci]: https://github.com/wayfair-incubator/columbo/actions
+        [pypi]: https://pypi.org/project/columbo/
+        [codecov]: https://codecov.io/gh/wayfair-incubator/columbo
+        [mypy-home]: http://mypy-lang.org/
+        [black-home]: https://github.com/psf/black
+        [columbo-docs]: https://github.com/wayfair-incubator/columbo/
+        [development-docs]: https://github.com/wayfair-incubator/columbo/development-guide/
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![CI pipeline status](https://github.com/plannigan/columbo/workflows/CI/badge.svg?branch=main)][ci]
-[![PyPI](https://img.shields.io/pypi/v/columbo)][pypi]
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/columbo)][pypi]
-[![codecov](https://codecov.io/gh/plannigan/columbo/branch/main/graph/badge.svg)][codecov]
-[![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)][mypy-home]
-[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)][black-home]
-
-# Columbo
-
-Specify a dynamic set of questions to ask a user and get their answers.
-
-`columbo`'s feature set allows a program to:
-
-* Ask multiple types of questions:
-    * Yes or No
-    * Multiple choice
-    * Open-ended
-* Validate the response provided by the user.
-* Use answers from earlier questions:
-    * As part of the text of a question
-    * As part of the text of a default value
-    * To decide if a question should be skipped
-* Accept answers from the command line in addition to prompting the user.
-
-## Example
-
-### User Prompts
-
-The primary use of `columbo` is to define a sequence of interactions that are used to prompt a user to provide answers
-using a terminal. Below is a sample which shows some ways this can be used.
-
-```python
-import columbo
-
-interactions = [
-    columbo.Echo("Welcome to the Columbo example"),
-    columbo.Acknowledge(
-        "Press enter to start"
-    ),
-    columbo.BasicQuestion(
-        "user",
-        "What is your name?",
-        default="Patrick",
-    ),
-    columbo.BasicQuestion(
-        "user_email",
-        lambda answers: f"""What email address should be used to contact {answers["user"]}?""",
-        default="me@example.com"
-    ),
-    columbo.Choice(
-        "mood",
-        "How are you feeling today?",
-        options={
-            "happy": "😀",
-            "sad": "😢",
-            "sleepy": "🥱",
-            "confused": "🤔",
-        },
-        default="happy",
-    ),
-    columbo.Confirm("likes_dogs", "Do you like dogs?", default=True),
-]
-
-answers = columbo.get_answers(interactions)
-print(answers)
-```
-
-Below shows the output when the user accepts the default values for most of the questions. The user provides a different
-value for the email and explicitly confirms that they like dogs.
-
-```text
-Welcome to the Columbo example
-Press enter to start
- 
-What is your name? [Patrick]:
-
-What email address should be used to contact Patrick? [me@example.com]: patrick@example.com
-
-How are you feeling today?
-1 - 😀
-2 - 😢
-3 - 🥱
-4 - 🤔
-Enter the number of your choice [1]:
-
-Do you like dogs? (Y/n): y
-
-{'user': 'Patrick', 'user_email': 'patrick@example.com', 'mood': 'happy', 'likes_dogs': True}
-```
-
-### Command Line Answers
-
-In addition to the interactive prompts, `columbo` can also parse command line arguments for interactions. This is done by
-changing `columbo.get_answers()` to `columbo.parse_args()`. Below shows the output when using the same interactions from above.
-
-```shell
-$ python columbo_example.py --user-email patrick@example.com --likes-dogs
-{'user': 'Patrick', 'user_email': 'patrick@example.com', 'mood': 'happy', 'likes_dogs': True}
-```
-
-<details>
-    <summary>The full example</summary>
-
-```python
-import columbo
-
-interactions = [
-    columbo.Echo("Welcome to the Columbo example"),
-    columbo.Acknowledge(
-        "Press enter to start"
-    ),
-    columbo.BasicQuestion(
-        "user",
-        "What is your name?",
-        default="Patrick",
-    ),
-    columbo.BasicQuestion(
-        "user_email",
-        lambda answers: f"""What email address should be used to contact {answers["user"]}?""",
-        default="me@example.com"
-    ),
-    columbo.Choice(
-        "mood",
-        "How are you feeling today?",
-        options=["happy", "sad", "sleepy", "confused"],
-        default="happy",
-    ),
-    columbo.Confirm("likes_dogs", "Do you like dogs?", default=True),
-]
-
-answers = columbo.parse_args(interactions)
-print(answers)
-```
-</details>
-
-## Documentation
-
-Check out the [project documentation][columbo-docs].
-
-For an overview on how repository structure and how to work with the code base, read the
-[Development Guide][development-docs].
-
-
-## Credits
-
-The development of this project was originally funded and incubated by [Wayfair](https://github.com/wayfair-incubator).
-
-[ci]: https://github.com/plannigan/columbo/actions
-[pypi]: https://pypi.org/project/columbo/
-[codecov]: https://codecov.io/gh/plannigan/columbo
-[mypy-home]: http://mypy-lang.org/
-[black-home]: https://github.com/psf/black
-[columbo-docs]: https://plannigan.github.io/columbo/latest/
-[development-docs]: https://plannigan.github.io/columbo/latest/development-guide/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `columbo-0.13.0.post1/README.md` & `columbo-0.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-[![CI pipeline status](https://github.com/plannigan/columbo/workflows/CI/badge.svg?branch=main)][ci]
+[![CI pipeline status](https://github.com/wayfair-incubator/columbo/workflows/CI/badge.svg?branch=main)][ci]
 [![PyPI](https://img.shields.io/pypi/v/columbo)][pypi]
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/columbo)][pypi]
-[![codecov](https://codecov.io/gh/plannigan/columbo/branch/main/graph/badge.svg)][codecov]
+[![codecov](https://codecov.io/gh/wayfair-incubator/columbo/branch/main/graph/badge.svg)][codecov]
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)][mypy-home]
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)][black-home]
 
 # Columbo
 
 Specify a dynamic set of questions to ask a user and get their answers.
 
@@ -46,20 +46,15 @@
         "user_email",
         lambda answers: f"""What email address should be used to contact {answers["user"]}?""",
         default="me@example.com"
     ),
     columbo.Choice(
         "mood",
         "How are you feeling today?",
-        options={
-            "happy": "😀",
-            "sad": "😢",
-            "sleepy": "🥱",
-            "confused": "🤔",
-        },
+        options=["happy", "sad", "sleepy", "confused"],
         default="happy",
     ),
     columbo.Confirm("likes_dogs", "Do you like dogs?", default=True),
 ]
 
 answers = columbo.get_answers(interactions)
 print(answers)
@@ -73,82 +68,36 @@
 Press enter to start
  
 What is your name? [Patrick]:
 
 What email address should be used to contact Patrick? [me@example.com]: patrick@example.com
 
 How are you feeling today?
-1 - 😀
-2 - 😢
-3 - 🥱
-4 - 🤔
+1 - happy
+2 - sad
+3 - sleepy
+4 - confused
 Enter the number of your choice [1]:
 
 Do you like dogs? (Y/n): y
 
 {'user': 'Patrick', 'user_email': 'patrick@example.com', 'mood': 'happy', 'likes_dogs': True}
 ```
 
 ### Command Line Answers
 
-In addition to the interactive prompts, `columbo` can also parse command line arguments for interactions. This is done by
-changing `columbo.get_answers()` to `columbo.parse_args()`. Below shows the output when using the same interactions from above.
-
-```shell
-$ python columbo_example.py --user-email patrick@example.com --likes-dogs
-{'user': 'Patrick', 'user_email': 'patrick@example.com', 'mood': 'happy', 'likes_dogs': True}
-```
-
-<details>
-    <summary>The full example</summary>
-
-```python
-import columbo
-
-interactions = [
-    columbo.Echo("Welcome to the Columbo example"),
-    columbo.Acknowledge(
-        "Press enter to start"
-    ),
-    columbo.BasicQuestion(
-        "user",
-        "What is your name?",
-        default="Patrick",
-    ),
-    columbo.BasicQuestion(
-        "user_email",
-        lambda answers: f"""What email address should be used to contact {answers["user"]}?""",
-        default="me@example.com"
-    ),
-    columbo.Choice(
-        "mood",
-        "How are you feeling today?",
-        options=["happy", "sad", "sleepy", "confused"],
-        default="happy",
-    ),
-    columbo.Confirm("likes_dogs", "Do you like dogs?", default=True),
-]
-
-answers = columbo.parse_args(interactions)
-print(answers)
-```
-</details>
+TODO
 
 ## Documentation
 
 Check out the [project documentation][columbo-docs].
 
 For an overview on how repository structure and how to work with the code base, read the
 [Development Guide][development-docs].
 
-
-## Credits
-
-The development of this project was originally funded and incubated by [Wayfair](https://github.com/wayfair-incubator).
-
-[ci]: https://github.com/plannigan/columbo/actions
+[ci]: https://github.com/wayfair-incubator/columbo/actions
 [pypi]: https://pypi.org/project/columbo/
-[codecov]: https://codecov.io/gh/plannigan/columbo
+[codecov]: https://codecov.io/gh/wayfair-incubator/columbo
 [mypy-home]: http://mypy-lang.org/
 [black-home]: https://github.com/psf/black
-[columbo-docs]: https://plannigan.github.io/columbo/latest/
-[development-docs]: https://plannigan.github.io/columbo/latest/development-guide/
+[columbo-docs]: https://github.com/wayfair-incubator/columbo/
+[development-docs]: https://github.com/wayfair-incubator/columbo/development-guide/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `columbo-0.13.0.post1/columbo/__init__.py` & `columbo-0.9.0/columbo/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,30 +6,25 @@
     DuplicateQuestionNameException,
 )
 from columbo._interaction import (  # noqa: F401
     Acknowledge,
     BasicQuestion,
     Choice,
     Confirm,
-    Displayable,
     Echo,
     Interaction,
     Question,
     get_answers,
 )
 from columbo._types import (  # noqa: F401
     Answer,
     Answers,
     MutableAnswers,
     OptionList,
-    Options,
     ShouldAsk,
     StaticOrDynamicValue,
-    ValidationFailure,
-    ValidationResponse,
-    ValidationSuccess,
     Validator,
 )
 
-__version__ = "0.13.0.post1"
-__author__ = "Patrick Lannigan <p.lannigan@gmail.com>"
+__version__ = "0.9.0"
+__author__ = "Patrick Lannigan <plannigan@wayfair.com>"
 __all__ = []  # type: ignore
```

### Comparing `columbo-0.13.0.post1/columbo/_cli.py` & `columbo-0.9.0/columbo/_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from columbo._interaction import (
     Acknowledge,
     BasicQuestion,
     Choice,
     Confirm,
     Echo,
     Interaction,
-    canonical_arg_name,
     to_value,
     validate_duplicate_question_names,
 )
 from columbo._types import Answers, MutableAnswers
 
 CliResult = Union[str, bool]
 CliResults = Dict[str, CliResult]
@@ -39,17 +38,16 @@
     :param exit_on_error: If `True`, print the CLI usage and exit the application. Otherwise, raise an exception with
         the error information.
     :param answers: An initial dictionary of answers to start from.
     :param parser_name: Optional name to be used in error text. If omitted, the name of the process will be used.
     :return: Answers based on the given arguments.
     :raises SystemExit: A value passed to CLI argument was not valid and `exit_on_error` was `True`.
     :raises CliException: A value passed to CLI argument was not valid and `exit_on_error` was `False`.
-    :raises DuplicateQuestionNameException: One of the given questions attempted to reuse a name. When a value is
-        provided for `answers`, those are considered as well.
-    :raises ValueError: One of the given `Interaction`s was not a valid type or was misconfigured in some way.
+    :raises DuplicateQuestionNameException: One of the given questions attempts to reuse a name. This includes a
+        question that was used to create `answers` if given.
     """
     validate_duplicate_question_names(interactions, answers)
     parser = create_parser(interactions, parser_name)
 
     if not exit_on_error:
         _patch_parser_error(parser)
 
@@ -67,16 +65,15 @@
     interactions: Collection[Interaction], parser_name: Optional[str] = None
 ) -> str:
     """
     Produce CLI help text for a given set of interactions.
 
     :param interactions: Interactions that should be turned into CLI arguments.
     :param parser_name: Optional name to be used in help text. If omitted, the name of the process will be used.
-    :raises DuplicateQuestionNameException: One of the given questions attempted to reuse a name.
-    :raises ValueError: One of the given `Interaction`s was not a valid type.
+    :raises DuplicateQuestionNameException: One of the given questions attempts to reuse a name.
     """
     validate_duplicate_question_names(interactions)
     return create_parser(interactions, parser_name).format_help()
 
 
 def create_parser(
     interactions: Collection[Interaction], parser_name: Optional[str] = None
@@ -105,35 +102,32 @@
 
 
 @singledispatch
 def _add_argument_for(question: Any, _: ArgumentParser) -> None:
     raise ValueError(f"Unsupported interaction type {type(question)}")
 
 
-# singledispatch for >=3.7 can use type annotations, but support for Union requires =>3.11
 @_add_argument_for.register(Acknowledge)
 @_add_argument_for.register(Echo)
-def _add_argument_for_noop(
-    question: Union[Acknowledge, Echo], parser: ArgumentParser
-) -> None:
+def _add_argument_for_noop(question, parser: ArgumentParser) -> None:
     pass
 
 
-@_add_argument_for.register
+@_add_argument_for.register(BasicQuestion)
 def _add_argument_for_basic(question: BasicQuestion, parser: ArgumentParser) -> None:
     _add_argument(parser, question.name, question.cli_help)
 
 
-@_add_argument_for.register
+@_add_argument_for.register(Confirm)
 def _add_argument_for_confirm(question: Confirm, parser: ArgumentParser) -> None:
     _add_flag(parser, question.name, question.cli_help, active=True)
     _add_flag(parser, question.name, question.cli_help, active=False)
 
 
-@_add_argument_for.register
+@_add_argument_for.register(Choice)
 def _add_argument_for_choice(question: Choice, parser: ArgumentParser) -> None:
     options = question.options
     _add_argument(
         parser,
         question.name,
         question.cli_help,
         # For dynamic options we don't restrict the values in the CLI.
@@ -162,15 +156,15 @@
 ) -> None:
     raise ValueError(f"Unsupported interaction type {type(question)}")
 
 
 @_update_answers.register(Acknowledge)
 @_update_answers.register(Echo)
 def _update_answers_noop(
-    question: Union[Acknowledge, Echo], cli_values: CliResults, answers: MutableAnswers
+    question, cli_values: CliResults, answers: MutableAnswers
 ) -> None:
     pass
 
 
 @_update_answers.register(BasicQuestion)
 @_update_answers.register(Choice)
 def _update_answers_validate(
@@ -179,23 +173,23 @@
     answers: MutableAnswers,
 ) -> None:
     if not question.should_ask(answers):
         return
     value = cast(str, cli_values.get(question.name))
     if value is None:
         value = to_value(question.default, answers, str)
-    result = question.validate(value, answers)
-    if not result.valid:
+    error = question.validate(value, answers)
+    if error:
         raise CliException.invalid_value(
-            value, canonical_arg_name(question.name), result.error
+            value, _canonical_arg_name(question.name), error
         )
     answers[question.name] = value
 
 
-@_update_answers.register
+@_update_answers.register(Confirm)
 def _update_answers_confirm(
     question: Confirm, cli_values: CliResults, answers: MutableAnswers
 ) -> None:
     if not question.should_ask(answers):
         return
     value = cli_values.get(question.name)
     if value is None:
@@ -208,15 +202,15 @@
     name: str,
     cli_help: Optional[str],
     dest: Optional[str] = None,
     action: str = "store",
     **kwargs,
 ) -> None:
     parser.add_argument(
-        canonical_arg_name(name),
+        _canonical_arg_name(name),
         action=action,
         dest=dest or name,
         help=cli_help,
         **kwargs,
     )
 
 
@@ -234,7 +228,11 @@
         name if active else f"no-{name}",
         cli_help,
         dest=name,
         action="store_const",
         const=active,
         **kwargs,
     )
+
+
+def _canonical_arg_name(name: str) -> str:
+    return f"--{name.lower().replace(' ', '-').replace('_', '-')}"
```

### Comparing `columbo-0.13.0.post1/columbo/_exception.py` & `columbo-0.9.0/columbo/_exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 
 class DuplicateQuestionNameException(ColumboException):
     """Multiple questions use the same name."""
 
 
 class CliException(ColumboException):
-    """An error occurred while processing command line arguments."""
-
     @classmethod
     def invalid_value(
         cls, value: str, argument_name: str, error_message: Optional[str] = None
     ) -> "CliException":
         formatted_error_message = f": {error_message}" if error_message else ""
         return cls(
             f"'{value}' is not a valid value for '{argument_name}'{formatted_error_message}"
```

### Comparing `columbo-0.13.0.post1/columbo/_user_io.py` & `columbo-0.9.0/columbo/_user_io.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Helpful wrappers for prompt-toolkit functionality.
 """
 
-from typing import Mapping
+from typing import Collection
 
 from prompt_toolkit import shortcuts
 from prompt_toolkit.formatted_text import merge_formatted_text
 from prompt_toolkit.key_binding.key_bindings import KeyBindings
 from prompt_toolkit.key_binding.key_processor import KeyPressEvent
 from prompt_toolkit.keys import Keys
 from prompt_toolkit.validation import Validator
@@ -50,29 +50,29 @@
     echo("")
 
     return answer
 
 
 def multiple_choice(
     question: str,
-    options: Mapping[str, str],
+    options: Collection[str],
     default: str,
     no_user_input: bool = False,
     **kwargs,
 ) -> str:
     if len(options) == 0:
         raise ValueError("options must contain at least one value")
 
     prompt_lines = [question]
     default_choice = None
     choice_map = {}
-    for i, (value, label) in enumerate(options.items()):
+    for i, value in enumerate(options):
         key = str(i + 1)
         choice_map[key] = value
-        prompt_lines.append(f"{key} - {label}")
+        prompt_lines.append(f"{key} - {value}")
 
         if default == value:
             default_choice = key
 
     if default_choice is None:
         raise ValueError(f"""Default "{default}" was not an option {options}""")
```

### Comparing `columbo-0.13.0.post1/columbo.egg-info/PKG-INFO` & `columbo-0.9.0/columbo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,173 +1,121 @@
 Metadata-Version: 2.1
 Name: columbo
-Version: 0.13.0.post1
+Version: 0.9.0
 Summary: Specify a dynamic set of questions to ask a user and get their answers.
-Home-page: https://github.com/plannigan/columbo
+Home-page: https://github.com/wayfair-incubator/columbo
 Author: Patrick Lannigan
-Author-email: p.lannigan@gmail.com
+Author-email: plannigan@wayfair.com
+License: UNKNOWN
+Description: [![CI pipeline status](https://github.com/wayfair-incubator/columbo/workflows/CI/badge.svg?branch=main)][ci]
+        [![PyPI](https://img.shields.io/pypi/v/columbo)][pypi]
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/columbo)][pypi]
+        [![codecov](https://codecov.io/gh/wayfair-incubator/columbo/branch/main/graph/badge.svg)][codecov]
+        [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)][mypy-home]
+        [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)][black-home]
+        
+        # Columbo
+        
+        Specify a dynamic set of questions to ask a user and get their answers.
+        
+        `columbo`'s feature set allows a program to:
+        
+        * Ask multiple types of questions:
+            * Yes or No
+            * Multiple choice
+            * Open-ended
+        * Validate the response provided by the user.
+        * Use answers from earlier questions:
+            * As part of the text of a question
+            * As part of the text of a default value
+            * To decide if a question should be skipped
+        * Accept answers from the command line in addition to prompting the user.
+        
+        ## Example
+        
+        ### User Prompts
+        
+        The primary use of `columbo` is to define a sequence of interactions that are used to prompt a user to provide answers
+        using a terminal. Below is a sample which shows some ways this can be used.
+        
+        ```python
+        import columbo
+        
+        interactions = [
+            columbo.Echo("Welcome to the Columbo example"),
+            columbo.Acknowledge(
+                "Press enter to start"
+            ),
+            columbo.BasicQuestion(
+                "user",
+                "What is your name?",
+                default="Patrick",
+            ),
+            columbo.BasicQuestion(
+                "user_email",
+                lambda answers: f"""What email address should be used to contact {answers["user"]}?""",
+                default="me@example.com"
+            ),
+            columbo.Choice(
+                "mood",
+                "How are you feeling today?",
+                options=["happy", "sad", "sleepy", "confused"],
+                default="happy",
+            ),
+            columbo.Confirm("likes_dogs", "Do you like dogs?", default=True),
+        ]
+        
+        answers = columbo.get_answers(interactions)
+        print(answers)
+        ```
+        
+        Below shows the output when the user accepts the default values for most of the questions. The user provides a different
+        value for the email and explicitly confirms that they like dogs.
+        
+        ```text
+        Welcome to the Columbo example
+        Press enter to start
+         
+        What is your name? [Patrick]:
+        
+        What email address should be used to contact Patrick? [me@example.com]: patrick@example.com
+        
+        How are you feeling today?
+        1 - happy
+        2 - sad
+        3 - sleepy
+        4 - confused
+        Enter the number of your choice [1]:
+        
+        Do you like dogs? (Y/n): y
+        
+        {'user': 'Patrick', 'user_email': 'patrick@example.com', 'mood': 'happy', 'likes_dogs': True}
+        ```
+        
+        ### Command Line Answers
+        
+        TODO
+        
+        ## Documentation
+        
+        Check out the [project documentation][columbo-docs].
+        
+        For an overview on how repository structure and how to work with the code base, read the
+        [Development Guide][development-docs].
+        
+        [ci]: https://github.com/wayfair-incubator/columbo/actions
+        [pypi]: https://pypi.org/project/columbo/
+        [codecov]: https://codecov.io/gh/wayfair-incubator/columbo
+        [mypy-home]: http://mypy-lang.org/
+        [black-home]: https://github.com/psf/black
+        [columbo-docs]: https://github.com/wayfair-incubator/columbo/
+        [development-docs]: https://github.com/wayfair-incubator/columbo/development-guide/
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![CI pipeline status](https://github.com/plannigan/columbo/workflows/CI/badge.svg?branch=main)][ci]
-[![PyPI](https://img.shields.io/pypi/v/columbo)][pypi]
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/columbo)][pypi]
-[![codecov](https://codecov.io/gh/plannigan/columbo/branch/main/graph/badge.svg)][codecov]
-[![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)][mypy-home]
-[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)][black-home]
-
-# Columbo
-
-Specify a dynamic set of questions to ask a user and get their answers.
-
-`columbo`'s feature set allows a program to:
-
-* Ask multiple types of questions:
-    * Yes or No
-    * Multiple choice
-    * Open-ended
-* Validate the response provided by the user.
-* Use answers from earlier questions:
-    * As part of the text of a question
-    * As part of the text of a default value
-    * To decide if a question should be skipped
-* Accept answers from the command line in addition to prompting the user.
-
-## Example
-
-### User Prompts
-
-The primary use of `columbo` is to define a sequence of interactions that are used to prompt a user to provide answers
-using a terminal. Below is a sample which shows some ways this can be used.
-
-```python
-import columbo
-
-interactions = [
-    columbo.Echo("Welcome to the Columbo example"),
-    columbo.Acknowledge(
-        "Press enter to start"
-    ),
-    columbo.BasicQuestion(
-        "user",
-        "What is your name?",
-        default="Patrick",
-    ),
-    columbo.BasicQuestion(
-        "user_email",
-        lambda answers: f"""What email address should be used to contact {answers["user"]}?""",
-        default="me@example.com"
-    ),
-    columbo.Choice(
-        "mood",
-        "How are you feeling today?",
-        options={
-            "happy": "😀",
-            "sad": "😢",
-            "sleepy": "🥱",
-            "confused": "🤔",
-        },
-        default="happy",
-    ),
-    columbo.Confirm("likes_dogs", "Do you like dogs?", default=True),
-]
-
-answers = columbo.get_answers(interactions)
-print(answers)
-```
-
-Below shows the output when the user accepts the default values for most of the questions. The user provides a different
-value for the email and explicitly confirms that they like dogs.
-
-```text
-Welcome to the Columbo example
-Press enter to start
- 
-What is your name? [Patrick]:
-
-What email address should be used to contact Patrick? [me@example.com]: patrick@example.com
-
-How are you feeling today?
-1 - 😀
-2 - 😢
-3 - 🥱
-4 - 🤔
-Enter the number of your choice [1]:
-
-Do you like dogs? (Y/n): y
-
-{'user': 'Patrick', 'user_email': 'patrick@example.com', 'mood': 'happy', 'likes_dogs': True}
-```
-
-### Command Line Answers
-
-In addition to the interactive prompts, `columbo` can also parse command line arguments for interactions. This is done by
-changing `columbo.get_answers()` to `columbo.parse_args()`. Below shows the output when using the same interactions from above.
-
-```shell
-$ python columbo_example.py --user-email patrick@example.com --likes-dogs
-{'user': 'Patrick', 'user_email': 'patrick@example.com', 'mood': 'happy', 'likes_dogs': True}
-```
-
-<details>
-    <summary>The full example</summary>
-
-```python
-import columbo
-
-interactions = [
-    columbo.Echo("Welcome to the Columbo example"),
-    columbo.Acknowledge(
-        "Press enter to start"
-    ),
-    columbo.BasicQuestion(
-        "user",
-        "What is your name?",
-        default="Patrick",
-    ),
-    columbo.BasicQuestion(
-        "user_email",
-        lambda answers: f"""What email address should be used to contact {answers["user"]}?""",
-        default="me@example.com"
-    ),
-    columbo.Choice(
-        "mood",
-        "How are you feeling today?",
-        options=["happy", "sad", "sleepy", "confused"],
-        default="happy",
-    ),
-    columbo.Confirm("likes_dogs", "Do you like dogs?", default=True),
-]
-
-answers = columbo.parse_args(interactions)
-print(answers)
-```
-</details>
-
-## Documentation
-
-Check out the [project documentation][columbo-docs].
-
-For an overview on how repository structure and how to work with the code base, read the
-[Development Guide][development-docs].
-
-
-## Credits
-
-The development of this project was originally funded and incubated by [Wayfair](https://github.com/wayfair-incubator).
-
-[ci]: https://github.com/plannigan/columbo/actions
-[pypi]: https://pypi.org/project/columbo/
-[codecov]: https://codecov.io/gh/plannigan/columbo
-[mypy-home]: http://mypy-lang.org/
-[black-home]: https://github.com/psf/black
-[columbo-docs]: https://plannigan.github.io/columbo/latest/
-[development-docs]: https://plannigan.github.io/columbo/latest/development-guide/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

