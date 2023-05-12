# Comparing `tmp/coral_decimal_mask-0.3.3.tar.gz` & `tmp/coral_decimal_mask-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coral_decimal_mask-0.3.3.tar", max compression
+gzip compressed data, was "coral_decimal_mask-0.4.0.tar", max compression
```

## Comparing `coral_decimal_mask-0.3.3.tar` & `coral_decimal_mask-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1556 2022-12-13 12:09:24.548182 coral_decimal_mask-0.3.3/README.md
--rw-r--r--   0        0        0        0 2022-12-13 12:09:24.548182 coral_decimal_mask-0.3.3/decimal_mask/__init__.py
--rw-r--r--   0        0        0       98 2022-12-13 12:09:24.548182 coral_decimal_mask-0.3.3/decimal_mask/apps.py
--rw-r--r--   0        0        0     3118 2023-02-14 11:55:14.376676 coral_decimal_mask-0.3.3/decimal_mask/static/decimal_mask/DecimalMask.js
--rw-r--r--   0        0        0      141 2022-12-13 12:09:24.548182 coral_decimal_mask-0.3.3/decimal_mask/static/decimal_mask/init.js
--rw-r--r--   0        0        0     2273 2023-02-16 18:36:07.404859 coral_decimal_mask-0.3.3/decimal_mask/widgets.py
--rw-r--r--   0        0        0     1306 2023-02-16 18:41:48.391169 coral_decimal_mask-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2276 1970-01-01 00:00:00.000000 coral_decimal_mask-0.3.3/setup.py
--rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 coral_decimal_mask-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1556 2022-12-13 12:09:24.548182 coral_decimal_mask-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-13 12:09:24.548182 coral_decimal_mask-0.4.0/decimal_mask/__init__.py
+-rw-r--r--   0        0        0       98 2022-12-13 12:09:24.548182 coral_decimal_mask-0.4.0/decimal_mask/apps.py
+-rw-r--r--   0        0        0     3118 2023-02-14 11:55:14.376676 coral_decimal_mask-0.4.0/decimal_mask/static/decimal_mask/DecimalMask.js
+-rw-r--r--   0        0        0      141 2022-12-13 12:09:24.548182 coral_decimal_mask-0.4.0/decimal_mask/static/decimal_mask/init.js
+-rw-r--r--   0        0        0     2273 2023-02-16 18:36:07.404859 coral_decimal_mask-0.4.0/decimal_mask/widgets.py
+-rw-r--r--   0        0        0     1288 2023-05-12 12:46:09.349689 coral_decimal_mask-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 coral_decimal_mask-0.4.0/setup.py
+-rw-r--r--   0        0        0     2280 1970-01-01 00:00:00.000000 coral_decimal_mask-0.4.0/PKG-INFO
```

### Comparing `coral_decimal_mask-0.3.3/README.md` & `coral_decimal_mask-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `coral_decimal_mask-0.3.3/decimal_mask/static/decimal_mask/DecimalMask.js` & `coral_decimal_mask-0.4.0/decimal_mask/static/decimal_mask/DecimalMask.js`

 * *Files identical despite different names*

### Comparing `coral_decimal_mask-0.3.3/decimal_mask/widgets.py` & `coral_decimal_mask-0.4.0/decimal_mask/widgets.py`

 * *Files identical despite different names*

### Comparing `coral_decimal_mask-0.3.3/pyproject.toml` & `coral_decimal_mask-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coral-decimal-mask"
-version = "0.3.3"
+version = "0.4.0"
 description = "Django mask decimal fields"
 authors = ["Coral Sistemas"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     'Environment :: Web Environment',
     'Framework :: Django',
@@ -17,21 +17,20 @@
 ]
 packages = [
     {include = "decimal_mask"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-Django = "^4.0.4"
 
 [tool.poetry.dev-dependencies]
-black = "^23.1.0"
+black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.10.1"
-pytest = "^7.2.0"
+pytest = "^7.3.1"
 pytest-django = "^4.5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `coral_decimal_mask-0.3.3/setup.py` & `coral_decimal_mask-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,24 @@
 
 packages = \
 ['decimal_mask']
 
 package_data = \
 {'': ['*'], 'decimal_mask': ['static/decimal_mask/*']}
 
-install_requires = \
-['Django>=4.0.4,<5.0.0']
-
 setup_kwargs = {
     'name': 'coral-decimal-mask',
-    'version': '0.3.3',
+    'version': '0.4.0',
     'description': 'Django mask decimal fields',
     'long_description': '# Coral Decimal Mask\n\nWidgets que aplicam mascaras nos forms do django.\n\n## Instalação\n\n```sh\npython -m pip install coral-decimal-mask\n```\n\n## Como usar\n\n#### Adicione `decimal_mask` em `INSTALLED_APPS`:\n\n```py\nINSTALLED_APPS = [\n    ...\n    "decimal_mask",\n]\n```\n\n#### Configure seus widgets: \n\n```py\nfrom django import forms\nfrom decimal_mask.widgets import DecimalMaskWidget, MoneyMaskWidget, PercentMaskWidget\n\n\nclass MyForm(forms.Form):\n    value1 = forms.DecimalField(widget=DecimalMaskWidget())\n    value2 = forms.DecimalField(\n        widget=DecimalMaskWidget(\n            decimal_attrs={\n                "locales": "pt-BR",\n                "decimalPlaces": 2,\n                "format": {\n                    "style": "currency",\n                    "currency": "BRL",\n                },\n            },\n        ),\n    ) # ou usar forms.DecimalField(widget=MoneyMaskWidget())\n    value3 = forms.DecimalField(widget=PercentMaskWidget())\n```\n\n- O parâmetro `decimal_attrs` são algumas opções para construir o objeto javascript [Intl.NumberFormat](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Intl/NumberFormat).\n\n  - `locales` é o primeiro parâmetro de `Intl.NumberFormat` referente a linguagem utilizada na interface do usuário da sua aplicação.\n\n  - `decimalPlaces` é o número de casas decimais que a mascara vai considerar.\n\n  - `format` é um `dict` com as informações do parâmetro `options` de `Intl.NumberFormat`.\n\n\n## Contribuindo com o projeto\n\n```py\n(venv) poetry install\n(venv) pytest\n```\n',
     'author': 'Coral Sistemas',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
-    'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `coral_decimal_mask-0.3.3/PKG-INFO` & `coral_decimal_mask-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coral-decimal-mask
-Version: 0.3.3
+Version: 0.4.0
 Summary: Django mask decimal fields
 License: MIT
 Author: Coral Sistemas
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Dist: Django (>=4.0.4,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Coral Decimal Mask
 
 Widgets que aplicam mascaras nos forms do django.
 
 ## Instalação
```

