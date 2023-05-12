# Comparing `tmp/dialoger-0.0.1.tar.gz` & `tmp/dialoger-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialoger-0.0.1.tar", last modified: Fri May 12 01:19:19 2023, max compression
+gzip compressed data, was "dialoger-1.0.0.tar", last modified: Fri May 12 08:17:51 2023, max compression
```

## Comparing `dialoger-0.0.1.tar` & `dialoger-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 01:19:19.206172 dialoger-0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-05-11 22:56:13.000000 dialoger-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     5380 2023-05-12 01:19:19.205173 dialoger-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4044 2023-05-12 00:09:06.000000 dialoger-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 01:19:19.144923 dialoger-0.0.1/dialoger/
--rw-rw-rw-   0        0        0     3086 2023-05-11 23:48:12.000000 dialoger-0.0.1/dialoger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 01:19:19.204189 dialoger-0.0.1/dialoger/images/
--rw-rw-rw-   0        0        0     4958 2023-05-11 11:57:21.000000 dialoger-0.0.1/dialoger/images/alert.ico
--rw-rw-rw-   0        0        0     1659 2023-05-11 11:54:50.000000 dialoger-0.0.1/dialoger/images/alert.png
--rw-rw-rw-   0        0        0     4958 2023-05-11 11:57:32.000000 dialoger-0.0.1/dialoger/images/error.ico
--rw-rw-rw-   0        0        0     2003 2023-05-11 11:54:58.000000 dialoger-0.0.1/dialoger/images/error.png
--rw-rw-rw-   0        0        0     4958 2023-05-11 11:58:22.000000 dialoger-0.0.1/dialoger/images/info.ico
--rw-rw-rw-   0        0        0     2061 2023-05-11 11:55:06.000000 dialoger-0.0.1/dialoger/images/info.png
--rw-rw-rw-   0        0        0     4958 2023-05-11 11:56:30.000000 dialoger-0.0.1/dialoger/images/question.ico
--rw-rw-rw-   0        0        0     2169 2023-05-11 11:55:20.000000 dialoger-0.0.1/dialoger/images/question.png
--rw-rw-rw-   0        0        0     4958 2023-05-11 11:56:22.000000 dialoger-0.0.1/dialoger/images/success.ico
--rw-rw-rw-   0        0        0     2094 2023-05-11 11:55:13.000000 dialoger-0.0.1/dialoger/images/success.png
--rw-rw-rw-   0        0        0     8857 2023-05-11 23:29:40.000000 dialoger-0.0.1/dialoger/input.py
--rw-rw-rw-   0        0        0     4241 2023-05-11 12:16:09.000000 dialoger-0.0.1/dialoger/options.py
-drwxrwxrwx   0        0        0        0 2023-05-12 01:19:19.161939 dialoger-0.0.1/dialoger.egg-info/
--rw-rw-rw-   0        0        0     5380 2023-05-12 01:19:19.000000 dialoger-0.0.1/dialoger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-05-12 01:19:19.000000 dialoger-0.0.1/dialoger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 01:19:19.000000 dialoger-0.0.1/dialoger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-12 01:19:19.000000 dialoger-0.0.1/dialoger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 01:19:19.206172 dialoger-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1695 2023-05-12 01:00:16.000000 dialoger-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:51.975411 dialoger-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-12 08:17:38.000000 dialoger-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-12 08:17:51.971411 dialoger-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-12 08:17:38.000000 dialoger-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:51.971411 dialoger-1.0.0/dialoger/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:51.971411 dialoger-1.0.0/dialoger/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/images/alert.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/images/alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/images/error.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/images/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/images/info.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/images/info.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/images/question.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/images/question.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/images/success.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/images/success.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-12 08:17:38.000000 dialoger-1.0.0/dialoger/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:51.971411 dialoger-1.0.0/dialoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-12 08:17:51.000000 dialoger-1.0.0/dialoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-12 08:17:51.000000 dialoger-1.0.0/dialoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:17:51.000000 dialoger-1.0.0/dialoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 08:17:51.000000 dialoger-1.0.0/dialoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:17:51.975411 dialoger-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-12 08:17:38.000000 dialoger-1.0.0/setup.py
```

### Comparing `dialoger-0.0.1/LICENSE` & `dialoger-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Guilherme Saldanha
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 Guilherme Saldanha
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `dialoger-0.0.1/PKG-INFO` & `dialoger-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-Metadata-Version: 2.1
-Name: dialoger
-Version: 0.0.1
-Summary: A package that provides a simple and user-friendly interface for creating interactive windows in Tkinter. Provides functions to create input windows, option list windows, alerts, information, errors and confirmation windows with options. Simplify user interaction with your program quickly and efficiently. One of the main functions is that it is possible to use patterns for certain answers, which allows requiring the user to have a date pattern, or input of numbers.
-Home-page: https://github.com/guisaldanha/dialoger
-Author: Guilherme Saldanha
-Author-email: guisaldanha@gmail.com
-License: MIT
-Keywords: tkinter,dialog,dialoger,dialogbox,dialogboxer,dialoguer,dialoguerbox,box,user interface,interactive,input,choices,alert,information,error,confirmation,easy-to-use,efficiency,user-friendly,pattern,date,number,date pattern,number pattern,pattern input,pattern input date,pattern input number
-Classifier: Intended Audience :: Developers
-Classifier: License :: Freely Distributable
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Communications
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Dialoger
-
-[![PyPI version](https://img.shields.io/pypi/v/dialoger)](https://img.shields.io/pypi/v/logandprint) [![License](https://img.shields.io/github/license/guisaldanha/dialoger)](LICENSE) [![Downloads](https://img.shields.io/pypi/dm/dialoger)](https://img.shields.io/pypi/dm/dialoger)
-
-Dialoger is a Python package that provides a set of functions to create interactive dialog windows in Tkinter with ease.
-
-## Installation
-
-You can install Dialoger using pip:
-
-```shell
-pip install dialoger
-```
-
-## Usage
-
-Dialoger provides a set of functions to create interactive dialog windows in Tkinter with ease. The functions are: `ask`, `askwithanswers`, `confirm`, `alert`, `info`, `error` and `success`.
-
-### ask
-
-The `ask` function creates a dialog window with a question and a text input. It returns the text inputted by the user.
-
-#### Parameters
-
-- `title`: The title of the dialog window.
-- `question`: The question to be asked to the user.
-- `answer_type`: The type of the answer. Can be `str`, `int`, `float`, `alphanumeric` or `password`.
-- `answer_default` (optional): The default answer. If `None`, the text input will be empty.
-- `pattern` (optional): A pattern to validate the answer. # will be replaced by the number. For example, `##/##/####` can be used to ask for a date or `###.###.###-##` to ask for a CPF. If `None`, no pattern will be used.
-- `allow_empty` (optional): If `True`, the user can leave the text input empty. If `False`, the user must input something.
-- `allow_cancel` (optional): If `True`, the user can cancel the dialog window. If `False`, the user must answer the question.
-
-```python
-import dialoger
-
-date = dialoger.ask('Birth date''', 'What is your birth date?', 'str', pattern='##/##/####', allow_empty=False, allow_cancel=False)
-
-print(f"You were born in {date}")
-```
-
-### askwithanswers
-
-The `askwithanswers` function creates a dialog window with a question and a list of choices. It returns the choice selected by the user.
-
-#### Parameters
-
-- `title`: The title of the dialog window.
-- `question`: The question to be asked to the user.
-- `choices`: A list of choices.
-
-```python
-import dialoger
-
-answer = dialoger.askwithanswers('Favorite color', 'What is your favorite color?', ['Red', 'Green', 'Blue'])
-
-print(f"Your favorite color is {answer}")
-```
-
-### confirm
-
-The `confirm` function creates a dialog window with a message and two buttons. It returns `True` if the user clicks the first button, or `False` if the user clicks the second button. The default buttons are "Yes" and "No", but you can change them by passing a list of strings as the `choices` parameter.
-
-#### Parameters
-
-- `title`: The title of the dialog window.
-- `message`: The message to be displayed to the user.
-- `choices` (optional): A list of strings to be used as the buttons. The first string will be used as the first button, and the second string will be used as the second button. If `None`, the default buttons will be used.
-
-```python
-import dialoger
-
-answer = dialoger.confirm('Confirm', 'Are you sure you want to delete this file?')
-
-if answer:
-    print('File deleted')
-else:
-    print('File not deleted')
-```
-
-### alert, info, error and success
-
-The `alert`, `info`, `error` and `success` functions create a dialog window with a message and a button. They don't return anything.
-
-#### Parameters
-
-- `title`: The title of the dialog window.
-- `message`: The message to be displayed to the user.
-
-```python
-import dialoger
-
-dialoger.alert('Alert', 'This is an alert')
-dialoger.info('Info', 'This is an info')
-dialoger.error('Error', 'This is an error')
-dialoger.success('Success', 'This is a success')
-```
-
-## License
-
-Dialoger is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
-
-## Contributing
-
-Contributions are welcome! You can contribute by opening an issue or submitting a pull request.
-
-## Credits
-
-Dialoger was created by [Guilherme Saldanha](https://guisaldanha.com).
+Metadata-Version: 2.1
+Name: dialoger
+Version: 1.0.0
+Summary: A package that provides a simple and user-friendly interface for creating interactive windows in Tkinter. Provides functions to create input windows, option list windows, alerts, information, errors and confirmation windows with options. Simplify user interaction with your program quickly and efficiently. One of the main functions is that it is possible to use patterns for certain answers, which allows requiring the user to have a date pattern, or input of numbers.
+Home-page: https://github.com/guisaldanha/dialoger
+Author: Guilherme Saldanha
+Author-email: guisaldanha@gmail.com
+License: MIT
+Keywords: tkinter,dialog,dialoger,dialogbox,dialogboxer,dialoguer,dialoguerbox,box,user interface,interactive,input,choices,alert,information,error,confirmation,easy-to-use,efficiency,user-friendly,pattern,date,number,date pattern,number pattern,pattern input,pattern input date,pattern input number
+Classifier: Intended Audience :: Developers
+Classifier: License :: Freely Distributable
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Communications
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Dialoger
+
+[![PyPI version](https://img.shields.io/pypi/v/dialoger)](https://img.shields.io/pypi/v/logandprint) [![License](https://img.shields.io/github/license/guisaldanha/dialoger)](LICENSE) [![Downloads](https://img.shields.io/pypi/dm/dialoger)](https://img.shields.io/pypi/dm/dialoger)
+
+Dialoger is a Python package that provides a set of functions to create interactive dialog windows in Tkinter with ease.
+
+## Installation
+
+You can install Dialoger using pip:
+
+```shell
+pip install dialoger
+```
+
+## Usage
+
+Dialoger provides a set of functions to create interactive dialog windows in Tkinter with ease. The functions are: `ask`, `askwithanswers`, `confirm`, `alert`, `info`, `error` and `success`.
+
+### ask
+
+The `ask` function creates a dialog window with a question and a text input. It returns the text inputted by the user.
+
+#### Parameters
+
+- `title`: The title of the dialog window.
+- `question`: The question to be asked to the user.
+- `answer_type`: The type of the answer. Can be `str`, `int`, `float`, `alphanumeric` or `password`.
+- `answer_default` (optional): The default answer. If `None`, the text input will be empty.
+- `pattern` (optional): A pattern to validate the answer. # will be replaced by the number. For example, `##/##/####` can be used to ask for a date or `###.###.###-##` to ask for a CPF. If `None`, no pattern will be used.
+- `allow_empty` (optional): If `True`, the user can leave the text input empty. If `False`, the user must input something.
+- `allow_cancel` (optional): If `True`, the user can cancel the dialog window. If `False`, the user must answer the question.
+
+```python
+import dialoger
+
+date = dialoger.ask('Birth date''', 'What is your birth date?', 'str', pattern='##/##/####', allow_empty=False, allow_cancel=False)
+
+print(f"You were born in {date}")
+```
+
+### askwithanswers
+
+The `askwithanswers` function creates a dialog window with a question and a list of choices. It returns the choice selected by the user.
+
+#### Parameters
+
+- `title`: The title of the dialog window.
+- `question`: The question to be asked to the user.
+- `choices`: A list of choices.
+
+```python
+import dialoger
+
+answer = dialoger.askwithanswers('Favorite color', 'What is your favorite color?', ['Red', 'Green', 'Blue'])
+
+print(f"Your favorite color is {answer}")
+```
+
+### confirm
+
+The `confirm` function creates a dialog window with a message and two buttons. It returns `True` if the user clicks the first button, or `False` if the user clicks the second button. The default buttons are "Yes" and "No", but you can change them by passing a list of strings as the `choices` parameter.
+
+#### Parameters
+
+- `title`: The title of the dialog window.
+- `message`: The message to be displayed to the user.
+- `choices` (optional): A list of strings to be used as the buttons. The first string will be used as the first button, and the second string will be used as the second button. If `None`, the default buttons will be used.
+
+```python
+import dialoger
+
+answer = dialoger.confirm('Confirm', 'Are you sure you want to delete this file?')
+
+if answer:
+    print('File deleted')
+else:
+    print('File not deleted')
+```
+
+### alert, info, error and success
+
+The `alert`, `info`, `error` and `success` functions create a dialog window with a message and a button. They don't return anything.
+
+#### Parameters
+
+- `title`: The title of the dialog window.
+- `message`: The message to be displayed to the user.
+
+```python
+import dialoger
+
+dialoger.alert('Alert', 'This is an alert')
+dialoger.info('Info', 'This is an info')
+dialoger.error('Error', 'This is an error')
+dialoger.success('Success', 'This is a success')
+```
+
+## License
+
+Dialoger is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
+
+## Contributing
+
+Contributions are welcome! You can contribute by opening an issue or submitting a pull request.
+
+## Credits
+
+Dialoger was created by [Guilherme Saldanha](https://guisaldanha.com).
```

### Comparing `dialoger-0.0.1/README.md` & `dialoger-1.0.0/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-# Dialoger
-
-[![PyPI version](https://img.shields.io/pypi/v/dialoger)](https://img.shields.io/pypi/v/logandprint) [![License](https://img.shields.io/github/license/guisaldanha/dialoger)](LICENSE) [![Downloads](https://img.shields.io/pypi/dm/dialoger)](https://img.shields.io/pypi/dm/dialoger)
-
-Dialoger is a Python package that provides a set of functions to create interactive dialog windows in Tkinter with ease.
-
-## Installation
-
-You can install Dialoger using pip:
-
-```shell
-pip install dialoger
-```
-
-## Usage
-
-Dialoger provides a set of functions to create interactive dialog windows in Tkinter with ease. The functions are: `ask`, `askwithanswers`, `confirm`, `alert`, `info`, `error` and `success`.
-
-### ask
-
-The `ask` function creates a dialog window with a question and a text input. It returns the text inputted by the user.
-
-#### Parameters
-
-- `title`: The title of the dialog window.
-- `question`: The question to be asked to the user.
-- `answer_type`: The type of the answer. Can be `str`, `int`, `float`, `alphanumeric` or `password`.
-- `answer_default` (optional): The default answer. If `None`, the text input will be empty.
-- `pattern` (optional): A pattern to validate the answer. # will be replaced by the number. For example, `##/##/####` can be used to ask for a date or `###.###.###-##` to ask for a CPF. If `None`, no pattern will be used.
-- `allow_empty` (optional): If `True`, the user can leave the text input empty. If `False`, the user must input something.
-- `allow_cancel` (optional): If `True`, the user can cancel the dialog window. If `False`, the user must answer the question.
-
-```python
-import dialoger
-
-date = dialoger.ask('Birth date''', 'What is your birth date?', 'str', pattern='##/##/####', allow_empty=False, allow_cancel=False)
-
-print(f"You were born in {date}")
-```
-
-### askwithanswers
-
-The `askwithanswers` function creates a dialog window with a question and a list of choices. It returns the choice selected by the user.
-
-#### Parameters
-
-- `title`: The title of the dialog window.
-- `question`: The question to be asked to the user.
-- `choices`: A list of choices.
-
-```python
-import dialoger
-
-answer = dialoger.askwithanswers('Favorite color', 'What is your favorite color?', ['Red', 'Green', 'Blue'])
-
-print(f"Your favorite color is {answer}")
-```
-
-### confirm
-
-The `confirm` function creates a dialog window with a message and two buttons. It returns `True` if the user clicks the first button, or `False` if the user clicks the second button. The default buttons are "Yes" and "No", but you can change them by passing a list of strings as the `choices` parameter.
-
-#### Parameters
-
-- `title`: The title of the dialog window.
-- `message`: The message to be displayed to the user.
-- `choices` (optional): A list of strings to be used as the buttons. The first string will be used as the first button, and the second string will be used as the second button. If `None`, the default buttons will be used.
-
-```python
-import dialoger
-
-answer = dialoger.confirm('Confirm', 'Are you sure you want to delete this file?')
-
-if answer:
-    print('File deleted')
-else:
-    print('File not deleted')
-```
-
-### alert, info, error and success
-
-The `alert`, `info`, `error` and `success` functions create a dialog window with a message and a button. They don't return anything.
-
-#### Parameters
-
-- `title`: The title of the dialog window.
-- `message`: The message to be displayed to the user.
-
-```python
-import dialoger
-
-dialoger.alert('Alert', 'This is an alert')
-dialoger.info('Info', 'This is an info')
-dialoger.error('Error', 'This is an error')
-dialoger.success('Success', 'This is a success')
-```
-
-## License
-
-Dialoger is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
-
-## Contributing
-
-Contributions are welcome! You can contribute by opening an issue or submitting a pull request.
-
-## Credits
-
-Dialoger was created by [Guilherme Saldanha](https://guisaldanha.com).
+# Dialoger
+
+[![PyPI version](https://img.shields.io/pypi/v/dialoger)](https://img.shields.io/pypi/v/logandprint) [![License](https://img.shields.io/github/license/guisaldanha/dialoger)](LICENSE) [![Downloads](https://img.shields.io/pypi/dm/dialoger)](https://img.shields.io/pypi/dm/dialoger)
+
+Dialoger is a Python package that provides a set of functions to create interactive dialog windows in Tkinter with ease.
+
+## Installation
+
+You can install Dialoger using pip:
+
+```shell
+pip install dialoger
+```
+
+## Usage
+
+Dialoger provides a set of functions to create interactive dialog windows in Tkinter with ease. The functions are: `ask`, `askwithanswers`, `confirm`, `alert`, `info`, `error` and `success`.
+
+### ask
+
+The `ask` function creates a dialog window with a question and a text input. It returns the text inputted by the user.
+
+#### Parameters
+
+- `title`: The title of the dialog window.
+- `question`: The question to be asked to the user.
+- `answer_type`: The type of the answer. Can be `str`, `int`, `float`, `alphanumeric` or `password`.
+- `answer_default` (optional): The default answer. If `None`, the text input will be empty.
+- `pattern` (optional): A pattern to validate the answer. # will be replaced by the number. For example, `##/##/####` can be used to ask for a date or `###.###.###-##` to ask for a CPF. If `None`, no pattern will be used.
+- `allow_empty` (optional): If `True`, the user can leave the text input empty. If `False`, the user must input something.
+- `allow_cancel` (optional): If `True`, the user can cancel the dialog window. If `False`, the user must answer the question.
+
+```python
+import dialoger
+
+date = dialoger.ask('Birth date''', 'What is your birth date?', 'str', pattern='##/##/####', allow_empty=False, allow_cancel=False)
+
+print(f"You were born in {date}")
+```
+
+### askwithanswers
+
+The `askwithanswers` function creates a dialog window with a question and a list of choices. It returns the choice selected by the user.
+
+#### Parameters
+
+- `title`: The title of the dialog window.
+- `question`: The question to be asked to the user.
+- `choices`: A list of choices.
+
+```python
+import dialoger
+
+answer = dialoger.askwithanswers('Favorite color', 'What is your favorite color?', ['Red', 'Green', 'Blue'])
+
+print(f"Your favorite color is {answer}")
+```
+
+### confirm
+
+The `confirm` function creates a dialog window with a message and two buttons. It returns `True` if the user clicks the first button, or `False` if the user clicks the second button. The default buttons are "Yes" and "No", but you can change them by passing a list of strings as the `choices` parameter.
+
+#### Parameters
+
+- `title`: The title of the dialog window.
+- `message`: The message to be displayed to the user.
+- `choices` (optional): A list of strings to be used as the buttons. The first string will be used as the first button, and the second string will be used as the second button. If `None`, the default buttons will be used.
+
+```python
+import dialoger
+
+answer = dialoger.confirm('Confirm', 'Are you sure you want to delete this file?')
+
+if answer:
+    print('File deleted')
+else:
+    print('File not deleted')
+```
+
+### alert, info, error and success
+
+The `alert`, `info`, `error` and `success` functions create a dialog window with a message and a button. They don't return anything.
+
+#### Parameters
+
+- `title`: The title of the dialog window.
+- `message`: The message to be displayed to the user.
+
+```python
+import dialoger
+
+dialoger.alert('Alert', 'This is an alert')
+dialoger.info('Info', 'This is an info')
+dialoger.error('Error', 'This is an error')
+dialoger.success('Success', 'This is a success')
+```
+
+## License
+
+Dialoger is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
+
+## Contributing
+
+Contributions are welcome! You can contribute by opening an issue or submitting a pull request.
+
+## Credits
+
+Dialoger was created by [Guilherme Saldanha](https://guisaldanha.com).
```

### Comparing `dialoger-0.0.1/dialoger/__init__.py` & `dialoger-1.0.0/dialoger/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-from dialoger.options import options
-from dialoger.input import input
-from tkinter import messagebox
-
-
-def ask(title:str, question:str, answer_type:str, answer_default:str = None, pattern:str = None, allow_empty:bool = True, allow_cancel:bool = True) -> str:
-    """
-    Create an input window
-
-    Args:
-        title (str): window title
-        question (str): question to be asked
-        answer_type (str): type of answer (int, float, alphanumeric, str)
-        allow_empty (bool, optional): allow empty answer. Defaults to True.
-        answer_default (str, optional): default answer. Defaults to None.
-
-    Returns:
-        str: answer
-    """
-    return input(title=title, question=question, answer_type=answer_type, answer_default=answer_default, pattern=pattern, allow_empty=allow_empty, allow_cancel=allow_cancel, icon="question").get_answer()
-
-
-def askwithanswers(title:str, question:str, choices:list) -> str:
-    """
-    Create an window with a list of choices
-
-    Args:
-        title (str): window title
-        question (str): question to be asked
-        choices (list): list of choices
-
-    Returns:
-        str: choice
-    """
-    return options(title=title, message=question, choices=choices, icon="question").choice
-
-
-def confirm(title:str, message:str, choices:list=["Yes", "No"]) -> bool:
-    """
-    Create an confirmation window, with 2 choices, True is returned if the first choice is selected, False otherwise
-
-    Args:
-        title (str): window title
-        message (str): message to be shown
-        choices (list, optional): list of choices. Defaults to ["Yes", "No"]
-    """
-    assert len(choices) == 2, "The list of options must contain exactly two options."
-    assert isinstance(choices[0], str) and isinstance(choices[1], str), "Options must be strings."
-    # Gets the user's choice
-    choice = askwithanswers(title=title, question=message, choices=choices)
-    # If the user's choice is the first option, return True
-    return choice == choices[0]
-
-
-def alert(title:str, message:str) -> str:
-    """
-    Create an alert window
-
-    Args:
-        title (str): window title
-        message (str): message to be shown
-    """
-    options(title=title, message=message, choices=["OK"], icon="alert")
-
-
-def info(title:str, message:str) -> str:
-    """
-    Create an information window
-
-    Args:
-        title (str): window title
-        message (str): message to be shown
-    """
-    options(title=title, message=message, choices=["OK"], icon="info")
-
-
-def error(title:str, message:str) -> str:
-    """
-    Create an error window
-
-    Args:
-        title (str): window title
-        message (str): message to be shown
-    """
-    options(title=title, message=message, choices=["OK"], icon="error")
-
-
-def success(title:str, message:str) -> str:
-    """
-    Create an success window
-
-    Args:
-        title (str): window title
-        message (str): message to be shown
-    """
-    options(title=title, message=message, choices=["OK"], icon="success")
+from dialoger.options import options
+from dialoger.input import input
+from tkinter import messagebox
+
+
+def ask(title:str, question:str, answer_type:str, answer_default:str = None, pattern:str = None, allow_empty:bool = True, allow_cancel:bool = True) -> str:
+    """
+    Create an input window
+
+    Args:
+        title (str): window title
+        question (str): question to be asked
+        answer_type (str): type of answer (int, float, alphanumeric, str)
+        allow_empty (bool, optional): allow empty answer. Defaults to True.
+        answer_default (str, optional): default answer. Defaults to None.
+
+    Returns:
+        str: answer
+    """
+    return input(title=title, question=question, answer_type=answer_type, answer_default=answer_default, pattern=pattern, allow_empty=allow_empty, allow_cancel=allow_cancel, icon="question").get_answer()
+
+
+def askwithanswers(title:str, question:str, choices:list) -> str:
+    """
+    Create an window with a list of choices
+
+    Args:
+        title (str): window title
+        question (str): question to be asked
+        choices (list): list of choices
+
+    Returns:
+        str: choice
+    """
+    return options(title=title, message=question, choices=choices, icon="question").choice
+
+
+def confirm(title:str, message:str, choices:list=["Yes", "No"]) -> bool:
+    """
+    Create an confirmation window, with 2 choices, True is returned if the first choice is selected, False otherwise
+
+    Args:
+        title (str): window title
+        message (str): message to be shown
+        choices (list, optional): list of choices. Defaults to ["Yes", "No"]
+    """
+    assert len(choices) == 2, "The list of options must contain exactly two options."
+    assert isinstance(choices[0], str) and isinstance(choices[1], str), "Options must be strings."
+    # Gets the user's choice
+    choice = askwithanswers(title=title, question=message, choices=choices)
+    # If the user's choice is the first option, return True
+    return choice == choices[0]
+
+
+def alert(title:str, message:str) -> str:
+    """
+    Create an alert window
+
+    Args:
+        title (str): window title
+        message (str): message to be shown
+    """
+    options(title=title, message=message, choices=["OK"], icon="alert")
+
+
+def info(title:str, message:str) -> str:
+    """
+    Create an information window
+
+    Args:
+        title (str): window title
+        message (str): message to be shown
+    """
+    options(title=title, message=message, choices=["OK"], icon="info")
+
+
+def error(title:str, message:str) -> str:
+    """
+    Create an error window
+
+    Args:
+        title (str): window title
+        message (str): message to be shown
+    """
+    options(title=title, message=message, choices=["OK"], icon="error")
+
+
+def success(title:str, message:str) -> str:
+    """
+    Create an success window
+
+    Args:
+        title (str): window title
+        message (str): message to be shown
+    """
+    options(title=title, message=message, choices=["OK"], icon="success")
```

### Comparing `dialoger-0.0.1/dialoger/images/alert.ico` & `dialoger-1.0.0/dialoger/images/alert.ico`

 * *Files identical despite different names*

### Comparing `dialoger-0.0.1/dialoger/images/alert.png` & `dialoger-1.0.0/dialoger/images/alert.png`

 * *Files identical despite different names*

### Comparing `dialoger-0.0.1/dialoger/images/error.ico` & `dialoger-1.0.0/dialoger/images/error.ico`

 * *Files identical despite different names*

### Comparing `dialoger-0.0.1/dialoger/images/error.png` & `dialoger-1.0.0/dialoger/images/error.png`

 * *Files identical despite different names*

### Comparing `dialoger-0.0.1/dialoger/images/info.ico` & `dialoger-1.0.0/dialoger/images/info.ico`

 * *Files identical despite different names*

### Comparing `dialoger-0.0.1/dialoger/images/info.png` & `dialoger-1.0.0/dialoger/images/info.png`

 * *Files identical despite different names*

### Comparing `dialoger-0.0.1/dialoger/images/question.ico` & `dialoger-1.0.0/dialoger/images/question.ico`

 * *Files identical despite different names*

### Comparing `dialoger-0.0.1/dialoger/images/question.png` & `dialoger-1.0.0/dialoger/images/question.png`

 * *Files identical despite different names*

### Comparing `dialoger-0.0.1/dialoger/images/success.ico` & `dialoger-1.0.0/dialoger/images/success.ico`

 * *Files identical despite different names*

### Comparing `dialoger-0.0.1/dialoger/images/success.png` & `dialoger-1.0.0/dialoger/images/success.png`

 * *Files identical despite different names*

### Comparing `dialoger-0.0.1/dialoger/input.py` & `dialoger-1.0.0/dialoger/input.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,242 +1,242 @@
-import tkinter as tk
-import os
-
-class input:
-    def __init__(self, title, question, answer_type="str", answer_default=None, pattern=None, allow_empty=True, allow_cancel=True, icon=None):
-        """
-        Initialize the window
-
-        Args:
-            title (str): window title
-            question (str): question to be asked
-            answer_type (str, optional): type of answer (int, float, alphanumeric, str). Defaults to "str".
-            allow_empty (bool, optional): allow empty answer. Defaults to True.
-            answer_default (_type_, optional): default answer. Defaults to None.
-            allow_cancel (bool, optional): allow cancel. Defaults to True.
-        """
-        # Initialize variables
-        self.question = question
-        self.answer_type = answer_type
-        self.allow_empty = allow_empty
-        self.answer_default = answer_default
-        self.allow_cancel = allow_cancel
-        self.pattern = pattern
-        self.closed = False
-        # Create window
-        self.root = tk.Tk()
-        self.root.title(title)
-        self.root.resizable(False, False)
-        self.root.geometry("+400+250")
-        self.root.wm_minsize(250, 50)
-        # self.root.wm_attributes('-toolwindow', 'True') # Remove the icon, minimize and maximize buttons
-        self.root.attributes('-topmost', True) # Always on top
-        self.root.bind("<Key>", self.key_pressed)
-        # Validate if the window can be closed
-        if self.allow_cancel:
-            self.root.protocol("WM_DELETE_WINDOW", self.close)
-        else:
-            self.root.protocol("WM_DELETE_WINDOW", lambda: None)
-        # Frame for the question
-        frmLabel = tk.Frame(self.root, background="white")
-        if icon:
-            imagepath = os.path.join(os.path.dirname(__file__), "images", icon)
-            self.root.iconbitmap(imagepath + '.ico')
-            image = tk.PhotoImage(file=imagepath + '.png')
-            titleImg = tk.Label(frmLabel, image=image, background="white")
-            titleImg.pack(side=tk.LEFT, anchor=tk.N,  padx=(15,3), pady=15)
-
-        wraplength = 400
-        titleMsg = tk.Label(frmLabel, text=self.question, background="white", justify=tk.LEFT, wraplength=wraplength)
-        titleMsg.pack(side=tk.LEFT, padx=(3,15), pady=15)
-        frmLabel.pack(expand=True, fill=tk.BOTH)
-
-        # Frame for the entry
-        frmEntry = tk.Frame(self.root, background="white")
-        self.entry = tk.Entry(frmEntry, validate="key")
-        if self.answer_type == "int":
-            self.entry.config(validatecommand=(self.root.register(self.validate_int), '%P'))
-        elif self.answer_type == "alphanumeric":
-            self.entry.config(validatecommand=(self.root.register(self.validate_alphanumeric), '%P'))
-        elif self.answer_type == "float":
-            self.entry.config(validatecommand=(self.root.register(self.validate_float), '%P'))
-        elif self.answer_type == "password":
-            self.entry.config(validatecommand=(self.root.register(self.validate_str), '%P'), show="*")
-        else:
-            self.entry.config(validatecommand=(self.root.register(self.validate_str), '%P'))
-        self.entry.bind("<Key>", self.key_pressed)
-        self.entry.focus()
-        self.entry.pack(padx=10, pady=(5,15), ipady=3)
-        frmEntry.pack(expand=True, fill=tk.BOTH)
-        # Frame for the buttons
-        frmButtons = tk.Frame(self.root)
-        self.button = tk.Button(frmButtons, text="OK", command=self.set_answer)
-        if not self.allow_empty:
-            self.button.config(state="disabled")
-        if self.answer_default is not None:
-            self.entry.insert(0, self.answer_default)
-            self.entry.select_range(0, tk.END)
-        self.button.pack(side=tk.LEFT, padx=10, pady=10, ipadx=3)
-        if self.allow_cancel:
-            self.buttonCancel = tk.Button(frmButtons, text="Cancel", command=self.close)
-            self.buttonCancel.pack(side=tk.LEFT, padx=10, pady=10, ipadx=3)
-            self.buttonCancel.bind("<Key>", lambda event: self.close())
-        if self.pattern is not None:
-            self.button.config(state="disabled")
-            self.entry.bind('<KeyRelease>', self.format_input)
-        frmButtons.pack(expand=True)
-        # Set focus on the window
-        self.root.after(300, lambda: [self.root.focus_force(), self.entry.focus_set()])
-        # Start the window
-        self.root.mainloop()
-
-    def format_input(self, event):
-        """Format the input according to the pattern"""
-        input = ''.join([c for c in self.entry.get() if c.isdigit()])
-        partial = ''
-        for char in self.pattern:
-            if char == '#':
-                if input:
-                    partial += input[0]
-                    input = input[1:]
-                else:
-                    partial += '#'
-            else:
-                partial += char
-
-        # Replaces all # with empty
-        result = ''.join([c for c in partial if c != '#'])
-
-        # while the last character is not a number, remove the last character
-        while len(result) > 0 and not result[-1].isdigit():
-            result = result[:-1]
-
-        # updates the entry's content with the formatted entry
-        self.entry.delete(0, tk.END)
-        self.entry.insert(0, result)
-
-        if len(self.entry.get()) != len(self.pattern):
-            self.button.config(state="disabled")
-
-    def validate_int(self, value):
-        """
-        Validate if the value is an integer
-
-        Args:
-            value (str): value to be validated
-
-        Returns:
-            bool: True if the value is an integer, False otherwise
-        """
-        if value.isdigit() or value == "":
-            self.button.config(state="normal")
-            return True
-        else:
-            return False
-
-    def validate_alphanumeric(self, value):
-        """
-        Validate if the value is alphanumeric
-
-        Args:
-            value (str): value to be validated
-
-        Returns:
-            bool: True if the value is alphanumeric, False otherwise
-        """
-        if value.isalnum() or value == "":
-            self.button.config(state="normal")
-            return True
-        else:
-            return False
-
-    def validate_float(self, value):
-        """
-        Validate if the value is a float
-
-        Args:
-            value (str): value to be validated
-
-        Returns:
-            bool: True if the value is a float, False otherwise
-        """
-        if value.replace(".", "").isdigit() or value == "":
-            self.button.config(state="normal")
-            return True
-        else:
-            return False
-
-    def validate_str(self, value):
-        """
-        Validate if the value is a string
-
-        Args:
-            value (str): value to be validated
-
-        Returns:
-            bool: True if the value is a string, False otherwise
-        """
-        self.button.config(state="normal")
-        return True
-
-    def key_pressed(self, event):
-        """
-        Handles keystrokes in the window for UI updates
-
-        Args:
-            event (event): key press event
-        """
-        # Escape
-        if event.keycode == 27:
-            if self.allow_cancel:
-                self.close()
-        # Enter
-        if event.keycode == 13:
-            if self.validate_answer():
-                self.root.quit()
-
-    def validate_answer(self):
-        """
-        Validate the answer
-
-        Returns:
-            bool: True if the answer is valid, False otherwise
-        """
-        if not self.allow_empty and self.entry.get() == "":
-            return False
-        if self.answer_type == "int" and not self.entry.get().isdigit():
-            return False
-        if self.answer_type == "alphanumeric" and not self.entry.get().isalnum():
-            return False
-        if self.answer_type == "float" and not self.entry.get().replace(".", "").isdigit():
-            return False
-        if self.pattern is not None:
-            if len(self.entry.get()) != len(self.pattern):
-                return False
-        return True
-
-    def close(self):
-        """
-        Close the window and set the answer to None
-        """
-        self.closed = True
-        self.root.destroy()
-
-    def set_answer(self):
-        """
-        Set the answer and close the window
-        """
-        if self.validate_answer():
-            self.root.quit()
-
-    def get_answer(self):
-        """
-        Get the answer and close the window
-
-        Returns:
-            str: answer
-        """
-        if self.closed:
-            return None
-        answer = self.entry.get()
-        self.root.destroy()
-        return answer
+import tkinter as tk
+import os
+
+class input:
+    def __init__(self, title, question, answer_type="str", answer_default=None, pattern=None, allow_empty=True, allow_cancel=True, icon=None):
+        """
+        Initialize the window
+
+        Args:
+            title (str): window title
+            question (str): question to be asked
+            answer_type (str, optional): type of answer (int, float, alphanumeric, str). Defaults to "str".
+            allow_empty (bool, optional): allow empty answer. Defaults to True.
+            answer_default (_type_, optional): default answer. Defaults to None.
+            allow_cancel (bool, optional): allow cancel. Defaults to True.
+        """
+        # Initialize variables
+        self.question = question
+        self.answer_type = answer_type
+        self.allow_empty = allow_empty
+        self.answer_default = answer_default
+        self.allow_cancel = allow_cancel
+        self.pattern = pattern
+        self.closed = False
+        # Create window
+        self.root = tk.Tk()
+        self.root.title(title)
+        self.root.resizable(False, False)
+        self.root.geometry("+400+250")
+        self.root.wm_minsize(250, 50)
+        # self.root.wm_attributes('-toolwindow', 'True') # Remove the icon, minimize and maximize buttons
+        self.root.attributes('-topmost', True) # Always on top
+        self.root.bind("<Key>", self.key_pressed)
+        # Validate if the window can be closed
+        if self.allow_cancel:
+            self.root.protocol("WM_DELETE_WINDOW", self.close)
+        else:
+            self.root.protocol("WM_DELETE_WINDOW", lambda: None)
+        # Frame for the question
+        frmLabel = tk.Frame(self.root, background="white")
+        if icon:
+            imagepath = os.path.join(os.path.dirname(__file__), "images", icon)
+            self.root.iconbitmap(imagepath + '.ico')
+            image = tk.PhotoImage(file=imagepath + '.png')
+            titleImg = tk.Label(frmLabel, image=image, background="white")
+            titleImg.pack(side=tk.LEFT, anchor=tk.N,  padx=(15,3), pady=15)
+
+        wraplength = 400
+        titleMsg = tk.Label(frmLabel, text=self.question, background="white", justify=tk.LEFT, wraplength=wraplength)
+        titleMsg.pack(side=tk.LEFT, padx=(3,15), pady=15)
+        frmLabel.pack(expand=True, fill=tk.BOTH)
+
+        # Frame for the entry
+        frmEntry = tk.Frame(self.root, background="white")
+        self.entry = tk.Entry(frmEntry, validate="key")
+        if self.answer_type == "int":
+            self.entry.config(validatecommand=(self.root.register(self.validate_int), '%P'))
+        elif self.answer_type == "alphanumeric":
+            self.entry.config(validatecommand=(self.root.register(self.validate_alphanumeric), '%P'))
+        elif self.answer_type == "float":
+            self.entry.config(validatecommand=(self.root.register(self.validate_float), '%P'))
+        elif self.answer_type == "password":
+            self.entry.config(validatecommand=(self.root.register(self.validate_str), '%P'), show="*")
+        else:
+            self.entry.config(validatecommand=(self.root.register(self.validate_str), '%P'))
+        self.entry.bind("<Key>", self.key_pressed)
+        self.entry.focus()
+        self.entry.pack(padx=10, pady=(5,15), ipady=3)
+        frmEntry.pack(expand=True, fill=tk.BOTH)
+        # Frame for the buttons
+        frmButtons = tk.Frame(self.root)
+        self.button = tk.Button(frmButtons, text="OK", command=self.set_answer)
+        if not self.allow_empty:
+            self.button.config(state="disabled")
+        if self.answer_default is not None:
+            self.entry.insert(0, self.answer_default)
+            self.entry.select_range(0, tk.END)
+        self.button.pack(side=tk.LEFT, padx=10, pady=10, ipadx=3)
+        if self.allow_cancel:
+            self.buttonCancel = tk.Button(frmButtons, text="Cancel", command=self.close)
+            self.buttonCancel.pack(side=tk.LEFT, padx=10, pady=10, ipadx=3)
+            self.buttonCancel.bind("<Key>", lambda event: self.close())
+        if self.pattern is not None:
+            self.button.config(state="disabled")
+            self.entry.bind('<KeyRelease>', self.format_input)
+        frmButtons.pack(expand=True)
+        # Set focus on the window
+        self.root.after(300, lambda: [self.root.focus_force(), self.entry.focus_set()])
+        # Start the window
+        self.root.mainloop()
+
+    def format_input(self, event):
+        """Format the input according to the pattern"""
+        input = ''.join([c for c in self.entry.get() if c.isdigit()])
+        partial = ''
+        for char in self.pattern:
+            if char == '#':
+                if input:
+                    partial += input[0]
+                    input = input[1:]
+                else:
+                    partial += '#'
+            else:
+                partial += char
+
+        # Replaces all # with empty
+        result = ''.join([c for c in partial if c != '#'])
+
+        # while the last character is not a number, remove the last character
+        while len(result) > 0 and not result[-1].isdigit():
+            result = result[:-1]
+
+        # updates the entry's content with the formatted entry
+        self.entry.delete(0, tk.END)
+        self.entry.insert(0, result)
+
+        if len(self.entry.get()) != len(self.pattern):
+            self.button.config(state="disabled")
+
+    def validate_int(self, value):
+        """
+        Validate if the value is an integer
+
+        Args:
+            value (str): value to be validated
+
+        Returns:
+            bool: True if the value is an integer, False otherwise
+        """
+        if value.isdigit() or value == "":
+            self.button.config(state="normal")
+            return True
+        else:
+            return False
+
+    def validate_alphanumeric(self, value):
+        """
+        Validate if the value is alphanumeric
+
+        Args:
+            value (str): value to be validated
+
+        Returns:
+            bool: True if the value is alphanumeric, False otherwise
+        """
+        if value.isalnum() or value == "":
+            self.button.config(state="normal")
+            return True
+        else:
+            return False
+
+    def validate_float(self, value):
+        """
+        Validate if the value is a float
+
+        Args:
+            value (str): value to be validated
+
+        Returns:
+            bool: True if the value is a float, False otherwise
+        """
+        if value.replace(".", "").isdigit() or value == "":
+            self.button.config(state="normal")
+            return True
+        else:
+            return False
+
+    def validate_str(self, value):
+        """
+        Validate if the value is a string
+
+        Args:
+            value (str): value to be validated
+
+        Returns:
+            bool: True if the value is a string, False otherwise
+        """
+        self.button.config(state="normal")
+        return True
+
+    def key_pressed(self, event):
+        """
+        Handles keystrokes in the window for UI updates
+
+        Args:
+            event (event): key press event
+        """
+        # Escape
+        if event.keycode == 27:
+            if self.allow_cancel:
+                self.close()
+        # Enter
+        if event.keycode == 13:
+            if self.validate_answer():
+                self.root.quit()
+
+    def validate_answer(self):
+        """
+        Validate the answer
+
+        Returns:
+            bool: True if the answer is valid, False otherwise
+        """
+        if not self.allow_empty and self.entry.get() == "":
+            return False
+        if self.answer_type == "int" and not self.entry.get().isdigit():
+            return False
+        if self.answer_type == "alphanumeric" and not self.entry.get().isalnum():
+            return False
+        if self.answer_type == "float" and not self.entry.get().replace(".", "").isdigit():
+            return False
+        if self.pattern is not None:
+            if len(self.entry.get()) != len(self.pattern):
+                return False
+        return True
+
+    def close(self):
+        """
+        Close the window and set the answer to None
+        """
+        self.closed = True
+        self.root.destroy()
+
+    def set_answer(self):
+        """
+        Set the answer and close the window
+        """
+        if self.validate_answer():
+            self.root.quit()
+
+    def get_answer(self):
+        """
+        Get the answer and close the window
+
+        Returns:
+            str: answer
+        """
+        if self.closed:
+            return None
+        answer = self.entry.get()
+        self.root.destroy()
+        return answer
```

### Comparing `dialoger-0.0.1/dialoger/options.py` & `dialoger-1.0.0/dialoger/options.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-import tkinter as tk
-import os
-
-class options():
-
-    def __init__(self, title:str, message:str, choices:list, icon=None) -> None:
-        """
-        Initialize the window
-
-        Args:
-            title (str): window title
-            message (str): message to be shown
-            choices (list): list of choices
-        """
-        # Create window
-        self.root = tk.Tk()
-        self.root.title(title)
-        self.root.resizable(False, False)
-        self.root.geometry("+400+250")
-        self.root.wm_minsize(250, 50)
-        self.root.attributes('-topmost', True) # Always on top
-        # self.root.wm_attributes('-toolwindow', 'True') # Remove the icon, minimize and maximize buttons
-        self.root.protocol("WM_DELETE_WINDOW", self.close())
-        self.root.bind("<Key>", self.key_pressed_in_root)
-        # Frame for the message
-        frmLabel = tk.Frame(self.root, background="white")
-        if icon:
-            imagepath = os.path.join(os.path.dirname(__file__), "images", icon)
-            self.root.iconbitmap(imagepath + '.ico')
-            image = tk.PhotoImage(file=imagepath + '.png')
-            titleImg = tk.Label(frmLabel, image=image, background="white")
-            titleImg.pack(side=tk.LEFT, anchor=tk.N,  padx=(15,3), pady=15)
-
-        wraplength = 400 if len(choices) < 3 else 650
-
-        titleMsg = tk.Label(frmLabel, text=message, background="white", justify=tk.LEFT, wraplength=wraplength)
-        titleMsg.pack(side=tk.LEFT, padx=(3,15), pady=15)
-
-        frmLabel.pack(expand=True, fill=tk.BOTH)
-        # Frame for the buttons
-        frmButtons = tk.Frame(self.root)
-        self.buttons = []
-        for choice in choices:
-            self.buttons.append(tk.Button(frmButtons, text=choice, borderwidth = 1, command=lambda x=choice: self.set_choice(self.root, x)))
-            self.buttons[-1].bind("<Key>", self.button_pressed_key)
-            self.buttons[-1].pack(side=tk.LEFT, padx=10, pady=10, ipadx=5, ipady=1)
-        self.buttons[0].focus_set()
-        frmButtons.pack(expand=True)
-        # Set focus on the window
-        self.root.after(300, lambda: [self.root.focus_force(), self.buttons[0].focus_set()])
-        # Start the window
-        self.root.mainloop()
-
-
-    def set_choice(self, root:tk.Tk, choice:str) -> str:
-        """
-        Set the choice and close the window
-
-        Args:
-            root (tkinter.Tk): root window
-            choice (str): choice
-
-        Returns:
-            str: choice
-        """
-        self.choice = choice
-        root.destroy()
-        return choice
-
-    def close(self):
-        """
-        Close the window and set the choice to None
-        """
-        self.choice = None
-
-    def key_pressed_in_root(self, event):
-        """
-        Handles keystrokes in the window for UI updates
-
-        Args:
-            event (event): key press event
-        """
-        # Escape
-        if event.keycode == 27:
-            self.root.destroy()
-
-    def button_pressed_key(self, event):
-        """
-        Handles button key presses for UI updates
-
-        Args:
-            event (event): key press event
-        """
-        # Enter
-        if event.keycode == 13:
-            self.set_choice(self.root, event.widget['text'])
-        # Down or Right
-        if event.keycode == 40 or event.keycode == 39:
-            self.next_button(event.widget)
-        # Up or Left
-        if event.keycode == 38 or event.keycode == 37:
-            self.previous_button(event.widget)
-
-    def next_button(self, button):
-        """
-        Select the next button
-
-        Args:
-            button (button): current button
-        """
-        i = self.buttons.index(button)
-        if i < len(self.buttons) - 1:
-            self.buttons[i + 1].focus_set()
-        else:
-            self.buttons[0].focus_set()
-
-    def previous_button(self, button):
-        """
-        Sekect the previous button
-
-        Args:
-            button (button): current button
-        """
-        i = self.buttons.index(button)
-        if i > 0:
-            self.buttons[i - 1].focus_set()
-        else:
-            self.buttons[-1].focus_set()
+import tkinter as tk
+import os
+
+class options():
+
+    def __init__(self, title:str, message:str, choices:list, icon=None) -> None:
+        """
+        Initialize the window
+
+        Args:
+            title (str): window title
+            message (str): message to be shown
+            choices (list): list of choices
+        """
+        # Create window
+        self.root = tk.Tk()
+        self.root.title(title)
+        self.root.resizable(False, False)
+        self.root.geometry("+400+250")
+        self.root.wm_minsize(250, 50)
+        self.root.attributes('-topmost', True) # Always on top
+        # self.root.wm_attributes('-toolwindow', 'True') # Remove the icon, minimize and maximize buttons
+        self.root.protocol("WM_DELETE_WINDOW", self.close())
+        self.root.bind("<Key>", self.key_pressed_in_root)
+        # Frame for the message
+        frmLabel = tk.Frame(self.root, background="white")
+        if icon:
+            imagepath = os.path.join(os.path.dirname(__file__), "images", icon)
+            self.root.iconbitmap(imagepath + '.ico')
+            image = tk.PhotoImage(file=imagepath + '.png')
+            titleImg = tk.Label(frmLabel, image=image, background="white")
+            titleImg.pack(side=tk.LEFT, anchor=tk.N,  padx=(15,3), pady=15)
+
+        wraplength = 400 if len(choices) < 3 else 650
+
+        titleMsg = tk.Label(frmLabel, text=message, background="white", justify=tk.LEFT, wraplength=wraplength)
+        titleMsg.pack(side=tk.LEFT, padx=(3,15), pady=15)
+
+        frmLabel.pack(expand=True, fill=tk.BOTH)
+        # Frame for the buttons
+        frmButtons = tk.Frame(self.root)
+        self.buttons = []
+        for choice in choices:
+            self.buttons.append(tk.Button(frmButtons, text=choice, borderwidth = 1, command=lambda x=choice: self.set_choice(self.root, x)))
+            self.buttons[-1].bind("<Key>", self.button_pressed_key)
+            self.buttons[-1].pack(side=tk.LEFT, padx=10, pady=10, ipadx=5, ipady=1)
+        self.buttons[0].focus_set()
+        frmButtons.pack(expand=True)
+        # Set focus on the window
+        self.root.after(300, lambda: [self.root.focus_force(), self.buttons[0].focus_set()])
+        # Start the window
+        self.root.mainloop()
+
+
+    def set_choice(self, root:tk.Tk, choice:str) -> str:
+        """
+        Set the choice and close the window
+
+        Args:
+            root (tkinter.Tk): root window
+            choice (str): choice
+
+        Returns:
+            str: choice
+        """
+        self.choice = choice
+        root.destroy()
+        return choice
+
+    def close(self):
+        """
+        Close the window and set the choice to None
+        """
+        self.choice = None
+
+    def key_pressed_in_root(self, event):
+        """
+        Handles keystrokes in the window for UI updates
+
+        Args:
+            event (event): key press event
+        """
+        # Escape
+        if event.keycode == 27:
+            self.root.destroy()
+
+    def button_pressed_key(self, event):
+        """
+        Handles button key presses for UI updates
+
+        Args:
+            event (event): key press event
+        """
+        # Enter
+        if event.keycode == 13:
+            self.set_choice(self.root, event.widget['text'])
+        # Down or Right
+        if event.keycode == 40 or event.keycode == 39:
+            self.next_button(event.widget)
+        # Up or Left
+        if event.keycode == 38 or event.keycode == 37:
+            self.previous_button(event.widget)
+
+    def next_button(self, button):
+        """
+        Select the next button
+
+        Args:
+            button (button): current button
+        """
+        i = self.buttons.index(button)
+        if i < len(self.buttons) - 1:
+            self.buttons[i + 1].focus_set()
+        else:
+            self.buttons[0].focus_set()
+
+    def previous_button(self, button):
+        """
+        Sekect the previous button
+
+        Args:
+            button (button): current button
+        """
+        i = self.buttons.index(button)
+        if i > 0:
+            self.buttons[i - 1].focus_set()
+        else:
+            self.buttons[-1].focus_set()
```

### Comparing `dialoger-0.0.1/dialoger.egg-info/PKG-INFO` & `dialoger-1.0.0/dialoger.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-Metadata-Version: 2.1
-Name: dialoger
-Version: 0.0.1
-Summary: A package that provides a simple and user-friendly interface for creating interactive windows in Tkinter. Provides functions to create input windows, option list windows, alerts, information, errors and confirmation windows with options. Simplify user interaction with your program quickly and efficiently. One of the main functions is that it is possible to use patterns for certain answers, which allows requiring the user to have a date pattern, or input of numbers.
-Home-page: https://github.com/guisaldanha/dialoger
-Author: Guilherme Saldanha
-Author-email: guisaldanha@gmail.com
-License: MIT
-Keywords: tkinter,dialog,dialoger,dialogbox,dialogboxer,dialoguer,dialoguerbox,box,user interface,interactive,input,choices,alert,information,error,confirmation,easy-to-use,efficiency,user-friendly,pattern,date,number,date pattern,number pattern,pattern input,pattern input date,pattern input number
-Classifier: Intended Audience :: Developers
-Classifier: License :: Freely Distributable
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Communications
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Dialoger
-
-[![PyPI version](https://img.shields.io/pypi/v/dialoger)](https://img.shields.io/pypi/v/logandprint) [![License](https://img.shields.io/github/license/guisaldanha/dialoger)](LICENSE) [![Downloads](https://img.shields.io/pypi/dm/dialoger)](https://img.shields.io/pypi/dm/dialoger)
-
-Dialoger is a Python package that provides a set of functions to create interactive dialog windows in Tkinter with ease.
-
-## Installation
-
-You can install Dialoger using pip:
-
-```shell
-pip install dialoger
-```
-
-## Usage
-
-Dialoger provides a set of functions to create interactive dialog windows in Tkinter with ease. The functions are: `ask`, `askwithanswers`, `confirm`, `alert`, `info`, `error` and `success`.
-
-### ask
-
-The `ask` function creates a dialog window with a question and a text input. It returns the text inputted by the user.
-
-#### Parameters
-
-- `title`: The title of the dialog window.
-- `question`: The question to be asked to the user.
-- `answer_type`: The type of the answer. Can be `str`, `int`, `float`, `alphanumeric` or `password`.
-- `answer_default` (optional): The default answer. If `None`, the text input will be empty.
-- `pattern` (optional): A pattern to validate the answer. # will be replaced by the number. For example, `##/##/####` can be used to ask for a date or `###.###.###-##` to ask for a CPF. If `None`, no pattern will be used.
-- `allow_empty` (optional): If `True`, the user can leave the text input empty. If `False`, the user must input something.
-- `allow_cancel` (optional): If `True`, the user can cancel the dialog window. If `False`, the user must answer the question.
-
-```python
-import dialoger
-
-date = dialoger.ask('Birth date''', 'What is your birth date?', 'str', pattern='##/##/####', allow_empty=False, allow_cancel=False)
-
-print(f"You were born in {date}")
-```
-
-### askwithanswers
-
-The `askwithanswers` function creates a dialog window with a question and a list of choices. It returns the choice selected by the user.
-
-#### Parameters
-
-- `title`: The title of the dialog window.
-- `question`: The question to be asked to the user.
-- `choices`: A list of choices.
-
-```python
-import dialoger
-
-answer = dialoger.askwithanswers('Favorite color', 'What is your favorite color?', ['Red', 'Green', 'Blue'])
-
-print(f"Your favorite color is {answer}")
-```
-
-### confirm
-
-The `confirm` function creates a dialog window with a message and two buttons. It returns `True` if the user clicks the first button, or `False` if the user clicks the second button. The default buttons are "Yes" and "No", but you can change them by passing a list of strings as the `choices` parameter.
-
-#### Parameters
-
-- `title`: The title of the dialog window.
-- `message`: The message to be displayed to the user.
-- `choices` (optional): A list of strings to be used as the buttons. The first string will be used as the first button, and the second string will be used as the second button. If `None`, the default buttons will be used.
-
-```python
-import dialoger
-
-answer = dialoger.confirm('Confirm', 'Are you sure you want to delete this file?')
-
-if answer:
-    print('File deleted')
-else:
-    print('File not deleted')
-```
-
-### alert, info, error and success
-
-The `alert`, `info`, `error` and `success` functions create a dialog window with a message and a button. They don't return anything.
-
-#### Parameters
-
-- `title`: The title of the dialog window.
-- `message`: The message to be displayed to the user.
-
-```python
-import dialoger
-
-dialoger.alert('Alert', 'This is an alert')
-dialoger.info('Info', 'This is an info')
-dialoger.error('Error', 'This is an error')
-dialoger.success('Success', 'This is a success')
-```
-
-## License
-
-Dialoger is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
-
-## Contributing
-
-Contributions are welcome! You can contribute by opening an issue or submitting a pull request.
-
-## Credits
-
-Dialoger was created by [Guilherme Saldanha](https://guisaldanha.com).
+Metadata-Version: 2.1
+Name: dialoger
+Version: 1.0.0
+Summary: A package that provides a simple and user-friendly interface for creating interactive windows in Tkinter. Provides functions to create input windows, option list windows, alerts, information, errors and confirmation windows with options. Simplify user interaction with your program quickly and efficiently. One of the main functions is that it is possible to use patterns for certain answers, which allows requiring the user to have a date pattern, or input of numbers.
+Home-page: https://github.com/guisaldanha/dialoger
+Author: Guilherme Saldanha
+Author-email: guisaldanha@gmail.com
+License: MIT
+Keywords: tkinter,dialog,dialoger,dialogbox,dialogboxer,dialoguer,dialoguerbox,box,user interface,interactive,input,choices,alert,information,error,confirmation,easy-to-use,efficiency,user-friendly,pattern,date,number,date pattern,number pattern,pattern input,pattern input date,pattern input number
+Classifier: Intended Audience :: Developers
+Classifier: License :: Freely Distributable
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Communications
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Dialoger
+
+[![PyPI version](https://img.shields.io/pypi/v/dialoger)](https://img.shields.io/pypi/v/logandprint) [![License](https://img.shields.io/github/license/guisaldanha/dialoger)](LICENSE) [![Downloads](https://img.shields.io/pypi/dm/dialoger)](https://img.shields.io/pypi/dm/dialoger)
+
+Dialoger is a Python package that provides a set of functions to create interactive dialog windows in Tkinter with ease.
+
+## Installation
+
+You can install Dialoger using pip:
+
+```shell
+pip install dialoger
+```
+
+## Usage
+
+Dialoger provides a set of functions to create interactive dialog windows in Tkinter with ease. The functions are: `ask`, `askwithanswers`, `confirm`, `alert`, `info`, `error` and `success`.
+
+### ask
+
+The `ask` function creates a dialog window with a question and a text input. It returns the text inputted by the user.
+
+#### Parameters
+
+- `title`: The title of the dialog window.
+- `question`: The question to be asked to the user.
+- `answer_type`: The type of the answer. Can be `str`, `int`, `float`, `alphanumeric` or `password`.
+- `answer_default` (optional): The default answer. If `None`, the text input will be empty.
+- `pattern` (optional): A pattern to validate the answer. # will be replaced by the number. For example, `##/##/####` can be used to ask for a date or `###.###.###-##` to ask for a CPF. If `None`, no pattern will be used.
+- `allow_empty` (optional): If `True`, the user can leave the text input empty. If `False`, the user must input something.
+- `allow_cancel` (optional): If `True`, the user can cancel the dialog window. If `False`, the user must answer the question.
+
+```python
+import dialoger
+
+date = dialoger.ask('Birth date''', 'What is your birth date?', 'str', pattern='##/##/####', allow_empty=False, allow_cancel=False)
+
+print(f"You were born in {date}")
+```
+
+### askwithanswers
+
+The `askwithanswers` function creates a dialog window with a question and a list of choices. It returns the choice selected by the user.
+
+#### Parameters
+
+- `title`: The title of the dialog window.
+- `question`: The question to be asked to the user.
+- `choices`: A list of choices.
+
+```python
+import dialoger
+
+answer = dialoger.askwithanswers('Favorite color', 'What is your favorite color?', ['Red', 'Green', 'Blue'])
+
+print(f"Your favorite color is {answer}")
+```
+
+### confirm
+
+The `confirm` function creates a dialog window with a message and two buttons. It returns `True` if the user clicks the first button, or `False` if the user clicks the second button. The default buttons are "Yes" and "No", but you can change them by passing a list of strings as the `choices` parameter.
+
+#### Parameters
+
+- `title`: The title of the dialog window.
+- `message`: The message to be displayed to the user.
+- `choices` (optional): A list of strings to be used as the buttons. The first string will be used as the first button, and the second string will be used as the second button. If `None`, the default buttons will be used.
+
+```python
+import dialoger
+
+answer = dialoger.confirm('Confirm', 'Are you sure you want to delete this file?')
+
+if answer:
+    print('File deleted')
+else:
+    print('File not deleted')
+```
+
+### alert, info, error and success
+
+The `alert`, `info`, `error` and `success` functions create a dialog window with a message and a button. They don't return anything.
+
+#### Parameters
+
+- `title`: The title of the dialog window.
+- `message`: The message to be displayed to the user.
+
+```python
+import dialoger
+
+dialoger.alert('Alert', 'This is an alert')
+dialoger.info('Info', 'This is an info')
+dialoger.error('Error', 'This is an error')
+dialoger.success('Success', 'This is a success')
+```
+
+## License
+
+Dialoger is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
+
+## Contributing
+
+Contributions are welcome! You can contribute by opening an issue or submitting a pull request.
+
+## Credits
+
+Dialoger was created by [Guilherme Saldanha](https://guisaldanha.com).
```

### Comparing `dialoger-0.0.1/setup.py` & `dialoger-1.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from setuptools import find_packages, setup
-
-package_name = 'dialoger'
-version = '0.0.1'
-
-setup(
-    name=package_name,
-    packages=find_packages(),
-    version=version,
-    package_data={
-        'dialoger': ['images/*'],
-    },
-    description='A package that provides a simple and user-friendly interface for creating interactive windows in Tkinter. Provides functions to create input windows, option list windows, alerts, information, errors and confirmation windows with options. Simplify user interaction with your program quickly and efficiently. One of the main functions is that it is possible to use patterns for certain answers, which allows requiring the user to have a date pattern, or input of numbers.',
-    long_description=open('README.md').read(),
-    long_description_content_type="text/markdown",
-    author='Guilherme Saldanha',
-    author_email='guisaldanha@gmail.com',
-    url='https://github.com/guisaldanha/dialoger',
-    license='MIT',
-    keywords=['tkinter', 'dialog', 'dialoger', 'dialogbox', 'dialogboxer', 'dialoguer', 'dialoguerbox', 'box', 'user interface', 'interactive', 'input', 'choices', 'alert', 'information', 'error', 'confirmation', 'easy-to-use', 'efficiency', 'user-friendly', 'pattern', 'date', 'number', 'date pattern', 'number pattern', 'pattern input', 'pattern input date', 'pattern input number'],
-    classifiers=[
-        'Intended Audience :: Developers',
-        'License :: Freely Distributable',
-        'Operating System :: Microsoft :: Windows',
-        'Operating System :: Unix',
-        'Programming Language :: Python :: 3.11',
-        'Topic :: Communications',
-        'Topic :: Utilities',
-    ],
-)
+from setuptools import find_packages, setup
+
+package_name = 'dialoger'
+version = '1.0.0'
+
+setup(
+    name=package_name,
+    packages=find_packages(),
+    version=version,
+    package_data={
+        'dialoger': ['images/*'],
+    },
+    description='A package that provides a simple and user-friendly interface for creating interactive windows in Tkinter. Provides functions to create input windows, option list windows, alerts, information, errors and confirmation windows with options. Simplify user interaction with your program quickly and efficiently. One of the main functions is that it is possible to use patterns for certain answers, which allows requiring the user to have a date pattern, or input of numbers.',
+    long_description=open('README.md').read(),
+    long_description_content_type="text/markdown",
+    author='Guilherme Saldanha',
+    author_email='guisaldanha@gmail.com',
+    url='https://github.com/guisaldanha/dialoger',
+    license='MIT',
+    keywords=['tkinter', 'dialog', 'dialoger', 'dialogbox', 'dialogboxer', 'dialoguer', 'dialoguerbox', 'box', 'user interface', 'interactive', 'input', 'choices', 'alert', 'information', 'error', 'confirmation', 'easy-to-use', 'efficiency', 'user-friendly', 'pattern', 'date', 'number', 'date pattern', 'number pattern', 'pattern input', 'pattern input date', 'pattern input number'],
+    classifiers=[
+        'Intended Audience :: Developers',
+        'License :: Freely Distributable',
+        'Operating System :: Microsoft :: Windows',
+        'Operating System :: Unix',
+        'Programming Language :: Python :: 3.11',
+        'Topic :: Communications',
+        'Topic :: Utilities',
+    ],
+)
```

