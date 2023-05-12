# Comparing `tmp/encrypt_decrypt_fields-1.2.5.tar.gz` & `tmp/encrypt_decrypt_fields-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encrypt_decrypt_fields-1.2.5.tar", max compression
+gzip compressed data, was "encrypt_decrypt_fields-1.3.5.tar", max compression
```

## Comparing `encrypt_decrypt_fields-1.2.5.tar` & `encrypt_decrypt_fields-1.3.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2021-12-07 12:02:34.029482 encrypt_decrypt_fields-1.2.5/LICENSE
--rw-r--r--   0        0        0     2039 2022-11-30 19:22:44.967530 encrypt_decrypt_fields-1.2.5/README.md
--rw-r--r--   0        0        0      179 2021-12-07 12:07:50.975803 encrypt_decrypt_fields-1.2.5/encrypt_decrypt_fields/__init__.py
--rw-r--r--   0        0        0      522 2021-12-07 12:02:34.029740 encrypt_decrypt_fields-1.2.5/encrypt_decrypt_fields/alchemy_fields.py
--rw-r--r--   0        0        0      775 2023-03-14 07:35:53.367115 encrypt_decrypt_fields-1.2.5/encrypt_decrypt_fields/crypto.py
--rw-r--r--   0        0        0      716 2023-03-14 07:35:53.370719 encrypt_decrypt_fields-1.2.5/encrypt_decrypt_fields/django_fields.py
--rw-r--r--   0        0        0     1144 2023-03-14 07:35:50.238588 encrypt_decrypt_fields-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 encrypt_decrypt_fields-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-12-07 12:02:34.029482 encrypt_decrypt_fields-1.3.5/LICENSE
+-rw-r--r--   0        0        0     2039 2022-11-30 19:22:44.967530 encrypt_decrypt_fields-1.3.5/README.md
+-rw-r--r--   0        0        0      179 2021-12-07 12:07:50.975803 encrypt_decrypt_fields-1.3.5/encrypt_decrypt_fields/__init__.py
+-rw-r--r--   0        0        0      522 2021-12-07 12:02:34.029740 encrypt_decrypt_fields-1.3.5/encrypt_decrypt_fields/alchemy_fields.py
+-rw-r--r--   0        0        0      775 2023-03-14 07:35:53.367115 encrypt_decrypt_fields-1.3.5/encrypt_decrypt_fields/crypto.py
+-rw-r--r--   0        0        0      716 2023-03-14 07:35:53.370719 encrypt_decrypt_fields-1.3.5/encrypt_decrypt_fields/django_fields.py
+-rw-r--r--   0        0        0     1146 2023-05-12 16:37:27.384819 encrypt_decrypt_fields-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 encrypt_decrypt_fields-1.3.5/PKG-INFO
```

### Comparing `encrypt_decrypt_fields-1.2.5/LICENSE` & `encrypt_decrypt_fields-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `encrypt_decrypt_fields-1.2.5/README.md` & `encrypt_decrypt_fields-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `encrypt_decrypt_fields-1.2.5/encrypt_decrypt_fields/alchemy_fields.py` & `encrypt_decrypt_fields-1.3.5/encrypt_decrypt_fields/alchemy_fields.py`

 * *Files identical despite different names*

### Comparing `encrypt_decrypt_fields-1.2.5/encrypt_decrypt_fields/crypto.py` & `encrypt_decrypt_fields-1.3.5/encrypt_decrypt_fields/crypto.py`

 * *Files identical despite different names*

### Comparing `encrypt_decrypt_fields-1.2.5/encrypt_decrypt_fields/django_fields.py` & `encrypt_decrypt_fields-1.3.5/encrypt_decrypt_fields/django_fields.py`

 * *Files identical despite different names*

### Comparing `encrypt_decrypt_fields-1.2.5/pyproject.toml` & `encrypt_decrypt_fields-1.3.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encrypt-decrypt-fields"
-version = "1.2.5"
+version = "1.3.5"
 description = "Encrypt and decrypt for django model field."
 authors = ["Denis Novikov <alpden550@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -20,16 +20,16 @@
 homepage = 'https://github.com/alpden550/django-encrypt-decrypt'
 repository = 'https://github.com/alpden550/django-encrypt-decrypt'
 keywords = ["django", "django-orm", "cryptography", "development", "orm", "sqlachemy-orm"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 SQLAlchemy = "^1.4.19"
-cryptography = ">37.0"
 Django = "*"
+cryptography = "^40.0.2"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.1.1"
 pytest = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `encrypt_decrypt_fields-1.2.5/PKG-INFO` & `encrypt_decrypt_fields-1.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encrypt-decrypt-fields
-Version: 1.2.5
+Version: 1.3.5
 Summary: Encrypt and decrypt for django model field.
 Home-page: https://github.com/alpden550/django-encrypt-decrypt
 License: MIT
 Keywords: django,django-orm,cryptography,development,orm,sqlachemy-orm
 Author: Denis Novikov
 Author-email: alpden550@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Topic :: Software Development
 Requires-Dist: Django
 Requires-Dist: SQLAlchemy (>=1.4.19,<2.0.0)
-Requires-Dist: cryptography (>37.0)
+Requires-Dist: cryptography (>=40.0.2,<41.0.0)
 Project-URL: Repository, https://github.com/alpden550/django-encrypt-decrypt
 Description-Content-Type: text/markdown
 
 # ORM Encrypt Decrypt Fields
  
 A Django and SQLAlchemy model field that encrypts your data based SHA256 algorithm and Fernet (symmetric encryption) when saving to the model field.  The fernet module guarantees that data encrypted using it cannot be further manipulated or read without the key.  It keeps data always encrypted in the database.
```

