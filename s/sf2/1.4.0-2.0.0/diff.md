# Comparing `tmp/sf2-1.4.0.tar.gz` & `tmp/sf2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sf2-1.4.0.tar", last modified: Fri Aug 26 07:10:58 2022, max compression
+gzip compressed data, was "sf2-2.0.0.tar", last modified: Fri May 12 13:50:27 2023, max compression
```

## Comparing `sf2-1.4.0.tar` & `sf2-2.0.0.tar`

### file list

```diff
@@ -1,26 +1,59 @@
-drwxrwxr-x   0 lmoulin   (1000) lmoulin   (1000)        0 2022-08-26 07:10:58.483303 sf2-1.4.0/
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)    11357 2022-08-19 12:39:23.000000 sf2-1.4.0/LICENSE
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     4690 2022-08-26 07:10:58.483303 sf2-1.4.0/PKG-INFO
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     3291 2022-08-20 17:03:57.000000 sf2-1.4.0/README.md
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)       38 2022-08-26 07:10:58.483303 sf2-1.4.0/setup.cfg
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     1058 2022-08-26 07:07:27.000000 sf2-1.4.0/setup.py
-drwxrwxr-x   0 lmoulin   (1000) lmoulin   (1000)        0 2022-08-26 07:10:58.467303 sf2-1.4.0/sf2/
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)        0 2022-08-19 07:50:43.000000 sf2-1.4.0/sf2/__init__.py
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)       64 2022-08-19 08:51:08.000000 sf2-1.4.0/sf2/__main__.py
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     2040 2022-08-20 17:03:57.000000 sf2-1.4.0/sf2/args.py
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     5321 2022-08-26 07:07:27.000000 sf2-1.4.0/sf2/cipher.py
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     5143 2022-08-20 17:03:57.000000 sf2-1.4.0/sf2/decryptgui.py
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     3232 2022-08-20 17:03:57.000000 sf2-1.4.0/sf2/editgui.py
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     5959 2022-08-20 17:03:57.000000 sf2-1.4.0/sf2/encryptgui.py
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     3620 2022-08-26 07:07:27.000000 sf2-1.4.0/sf2/extern.py
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     3129 2022-08-26 07:07:27.000000 sf2-1.4.0/sf2/sf2.py
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     3692 2022-08-20 17:03:57.000000 sf2-1.4.0/sf2/sf2gui.py
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     2895 2022-08-20 17:03:57.000000 sf2-1.4.0/sf2/verifygui.py
-drwxrwxr-x   0 lmoulin   (1000) lmoulin   (1000)        0 2022-08-26 07:10:58.483303 sf2-1.4.0/sf2.egg-info/
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     4690 2022-08-26 07:10:58.000000 sf2-1.4.0/sf2.egg-info/PKG-INFO
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)      381 2022-08-26 07:10:58.000000 sf2-1.4.0/sf2.egg-info/SOURCES.txt
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)        1 2022-08-26 07:10:58.000000 sf2-1.4.0/sf2.egg-info/dependency_links.txt
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)       63 2022-08-26 07:10:58.000000 sf2-1.4.0/sf2.egg-info/entry_points.txt
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)        1 2022-08-20 16:57:34.000000 sf2-1.4.0/sf2.egg-info/not-zip-safe
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)       31 2022-08-26 07:10:58.000000 sf2-1.4.0/sf2.egg-info/requires.txt
--rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)        4 2022-08-26 07:10:58.000000 sf2-1.4.0/sf2.egg-info/top_level.txt
+drwxrwxr-x   0 lmoulin   (1000) lmoulin   (1000)        0 2023-05-12 13:50:27.545188 sf2-2.0.0/
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     1072 2023-05-12 13:38:37.000000 sf2-2.0.0/LICENSE
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)    11369 2023-05-12 13:50:27.545188 sf2-2.0.0/PKG-INFO
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     9058 2023-05-12 13:38:37.000000 sf2-2.0.0/README.md
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)       38 2023-05-12 13:50:27.545188 sf2-2.0.0/setup.cfg
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     1091 2023-05-12 13:50:06.000000 sf2-2.0.0/setup.py
+drwxrwxr-x   0 lmoulin   (1000) lmoulin   (1000)        0 2023-05-12 13:50:27.541188 sf2-2.0.0/sf2/
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)        0 2022-08-19 07:50:43.000000 sf2-2.0.0/sf2/__init__.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)       83 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/__main__.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     6935 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/args.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     3776 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/auth_sign.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     5314 2022-10-13 11:54:27.000000 sf2-2.0.0/sf2/cipher.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)    13004 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/container_base.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)    11038 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/container_ssh.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)      789 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/convert_container.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     6977 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/core.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     7984 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/core_with_environment.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     3704 2022-08-30 13:20:20.000000 sf2-2.0.0/sf2/fernetramfile.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)      651 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/file_object.py
+drwxrwxr-x   0 lmoulin   (1000) lmoulin   (1000)        0 2023-05-12 13:50:27.541188 sf2-2.0.0/sf2/gui/
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)        0 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/gui/__init__.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)      701 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/gui/about.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     2413 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/gui/change_password.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     3675 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/gui/convert.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     6887 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/gui/decrypt.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     4069 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/gui/encrypt.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     5649 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/gui/gui.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     3467 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/gui/new.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     5987 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/gui/open.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     7863 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/gui/ssh.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     1180 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/gui/tools.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     5731 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/gui/verify.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     2913 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/json_support.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     1142 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/msgpack_support.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     9173 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/openinram.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     7393 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/sf2.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)      933 2023-05-12 13:38:37.000000 sf2-2.0.0/sf2/ssh_file_object.py
+drwxrwxr-x   0 lmoulin   (1000) lmoulin   (1000)        0 2023-05-12 13:50:27.541188 sf2-2.0.0/sf2.egg-info/
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)    11369 2023-05-12 13:50:27.000000 sf2-2.0.0/sf2.egg-info/PKG-INFO
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     1090 2023-05-12 13:50:27.000000 sf2-2.0.0/sf2.egg-info/SOURCES.txt
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)        1 2023-05-12 13:50:27.000000 sf2-2.0.0/sf2.egg-info/dependency_links.txt
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)       38 2023-05-12 13:50:27.000000 sf2-2.0.0/sf2.egg-info/entry_points.txt
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)        1 2022-08-20 16:57:34.000000 sf2-2.0.0/sf2.egg-info/not-zip-safe
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)       84 2023-05-12 13:50:27.000000 sf2-2.0.0/sf2.egg-info/requires.txt
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)        4 2023-05-12 13:50:27.000000 sf2-2.0.0/sf2.egg-info/top_level.txt
+drwxrwxr-x   0 lmoulin   (1000) lmoulin   (1000)        0 2023-05-12 13:50:27.545188 sf2-2.0.0/test/
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     5893 2023-05-12 13:38:37.000000 sf2-2.0.0/test/test_args.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     2159 2023-05-12 13:38:37.000000 sf2-2.0.0/test/test_auth_sign.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     2676 2023-05-12 13:38:37.000000 sf2-2.0.0/test/test_container_base.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     3888 2023-05-12 13:38:37.000000 sf2-2.0.0/test/test_container_ssh.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)      924 2023-05-12 13:38:37.000000 sf2-2.0.0/test/test_convert_container.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     4509 2023-05-12 13:38:37.000000 sf2-2.0.0/test/test_core.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     9081 2023-05-12 13:38:37.000000 sf2-2.0.0/test/test_core_with_environment.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     1289 2022-08-30 13:23:24.000000 sf2-2.0.0/test/test_fernetramfile.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     1380 2023-05-12 13:38:37.000000 sf2-2.0.0/test/test_file_object.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     1493 2023-05-12 13:38:37.000000 sf2-2.0.0/test/test_json_support.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)      675 2023-05-12 13:38:37.000000 sf2-2.0.0/test/test_msgpack_support.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     4200 2023-05-12 13:38:37.000000 sf2-2.0.0/test/test_openinram.py
+-rw-rw-r--   0 lmoulin   (1000) lmoulin   (1000)     1868 2023-05-12 13:38:37.000000 sf2-2.0.0/test/test_ssh_file_object.py
```

### Comparing `sf2-1.4.0/setup.py` & `sf2-2.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from setuptools import setup, find_packages
  
 setup(name='sf2',
-    version='1.4.0',
+    version='2.0.0',
     url='https://github.com/laulin/sf2',
-    license='Apachev2',
+    license='MIT',
     author='Laurent MOULIN',
     author_email='gignops@gmail.com',
-    description='Encrypt and decrypt your file with Fernet algorithm',
-    packages=find_packages(exclude=['tests', "etc", "build", "dist", "sf2.egg-info"]),
-    install_requires=["cryptography", "dearpygui", "inotify"],
+    description='Share and work in team your files in full safety thanks to SSH keys.',
+    packages=find_packages(exclude=['test', "etc", "build", "dist", "sf2.egg-info", "bin"]),
+    install_requires=["cryptography", "inotify", "msgpack", "flufl.lock", "password-validator", "pyyaml", "pywebio", "pywebview"],
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     zip_safe=False,
     classifiers=[
       "Programming Language :: Python :: 3",
-      "License :: OSI Approved :: Apache Software License",
+      "License :: OSI Approved :: MIT License",
       "Operating System :: OS Independent",
       "Development Status :: 5 - Production/Stable",
       "Intended Audience :: Information Technology",
       "Topic :: Security :: Cryptography"
     ],
     python_requires='>=3',
       entry_points={
             'console_scripts': [ 
-            'sf2 = sf2.sf2:main', 
-            'sf2gui = sf2.sf2gui:main'
+            'sf2 = sf2.sf2:main'
             ] 
       }
 )
```

### Comparing `sf2-1.4.0/sf2/cipher.py` & `sf2-2.0.0/sf2/cipher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import base64
-from operator import contains
 import os
 import json
 
 from cryptography.fernet import Fernet
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 
 class Cipher:
     def __init__(self) -> None:
         pass
 
-    def password_2_key(self, salt:bytes, password:str)->bytes:
+    def password_2_key(self, salt:bytes, password:str, iterations:int=480000)->bytes:
         """
         It takes a salt and a password and returns a key for Fernet module
         
         :param salt: a random string of bytes
         :type salt: bytes
         :param password: The password to use for the key derivation
         :type password: str
```

