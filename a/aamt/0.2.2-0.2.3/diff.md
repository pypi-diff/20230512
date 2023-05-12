# Comparing `tmp/aamt-0.2.2.tar.gz` & `tmp/aamt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aamt-0.2.2.tar", max compression
+gzip compressed data, was "aamt-0.2.3.tar", max compression
```

## Comparing `aamt-0.2.2.tar` & `aamt-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      117 2023-02-02 03:17:30.642752 aamt-0.2.2/aamt/__init__.py
--rw-r--r--   0        0        0     1358 2022-11-24 03:37:14.496202 aamt-0.2.2/aamt/cli.py
--rw-r--r--   0        0        0     1192 2023-01-31 07:14:07.219295 aamt-0.2.2/aamt/config.py
--rw-r--r--   0        0        0     1348 2023-01-31 07:15:12.401270 aamt-0.2.2/aamt/fixture.py
--rw-r--r--   0        0        0     6409 2023-02-02 03:09:41.058052 aamt-0.2.2/aamt/plugin.py
--rw-r--r--   0        0        0    55194 2023-02-02 03:16:58.263208 aamt-0.2.2/aamt/sample.py
--rw-r--r--   0        0        0     7104 2023-01-31 09:25:07.460581 aamt-0.2.2/aamt/scaffold.py
--rw-r--r--   0        0        0      925 2023-02-02 03:17:15.042508 aamt-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      542 2023-02-02 03:16:39.219687 aamt-0.2.2/README.md
--rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 aamt-0.2.2/setup.py
--rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 aamt-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      117 2023-02-02 03:17:30.642752 aamt-0.2.3/aamt/__init__.py
+-rw-r--r--   0        0        0     1358 2022-11-24 03:37:14.496202 aamt-0.2.3/aamt/cli.py
+-rw-r--r--   0        0        0     1192 2023-01-31 07:14:07.219295 aamt-0.2.3/aamt/config.py
+-rw-r--r--   0        0        0     1348 2023-01-31 07:15:12.401270 aamt-0.2.3/aamt/fixture.py
+-rw-r--r--   0        0        0     6409 2023-02-02 03:09:41.058052 aamt-0.2.3/aamt/plugin.py
+-rw-r--r--   0        0        0    55311 2023-05-12 05:14:49.077860 aamt-0.2.3/aamt/sample.py
+-rw-r--r--   0        0        0     7104 2023-01-31 09:25:07.460581 aamt-0.2.3/aamt/scaffold.py
+-rw-r--r--   0        0        0      925 2023-05-12 05:19:49.083686 aamt-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      542 2023-02-02 03:16:39.219687 aamt-0.2.3/README.md
+-rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 aamt-0.2.3/setup.py
+-rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 aamt-0.2.3/PKG-INFO
```

### Comparing `aamt-0.2.2/aamt/cli.py` & `aamt-0.2.3/aamt/cli.py`

 * *Files identical despite different names*

### Comparing `aamt-0.2.2/aamt/config.py` & `aamt-0.2.3/aamt/config.py`

 * *Files identical despite different names*

### Comparing `aamt-0.2.2/aamt/fixture.py` & `aamt-0.2.3/aamt/fixture.py`

 * *Files identical despite different names*

### Comparing `aamt-0.2.2/aamt/plugin.py` & `aamt-0.2.3/aamt/plugin.py`

 * *Files identical despite different names*

### Comparing `aamt-0.2.2/aamt/sample.py` & `aamt-0.2.3/aamt/sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -530,15 +530,15 @@
 emailhelper_content = """
 # -*- coding: utf-8 -*-
 
 # @Software: PyCharm
 # @File: emailhelper.py
 # @Author: xuefeng365
 # @E-mail: 120158568@qq.com,
-# @Site: 
+# @Site: www.51automate.cn
 # @Time: 11月 24, 2022
 
 import smtplib  # 加载smtplib模块
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 
 from email.utils import formataddr
@@ -769,15 +769,15 @@
 """
 project_content = """
 # -*- coding: UTF-8 -*-
 # @Software: PyCharm
 # @File: project.py
 # @Author: xuefeng365
 # @E-mail: 120158568@qq.com,
-# @Site:
+# @Site: www.51automate.cn
 # @Time: 11月 23, 2022
 
 import os
 import configparser
 import yaml
 from loguru import logger
 
@@ -847,14 +847,15 @@
         with open(test_data_path, encoding="utf-8") as f:
             return yaml.load(f.read(), Loader=yaml.FullLoader)
 
 
 def get_file_path(file_name, middle='file'):
     '''
     file_name: 文件名，比如 xiaoxin.png
+    middle： 文件夹，如果有文件夹嵌套，建议写在Config类里面
     '''
     filePath = os.path.join(settings.root_dir, middle,file_name)
     return filePath
 
 
 
 if __name__ == '__main__':
@@ -1210,14 +1211,15 @@
 
 # @Software: PyCharm
 # @File: conftest.py
 # @Author: xuefeng365
 # @E-mail: 120158568@qq.com,
 # @Site: www.51automate.cn
 # @Time: 11月 25, 2022
+
 import pytest
 from aamt.plugin import aamt_plugins
 
 # 加载aamt插件
 from api.offer_doctor.doctor_need_api import Dictor_need
 
 pytest_plugins = aamt_plugins()
```

### Comparing `aamt-0.2.2/aamt/scaffold.py` & `aamt-0.2.3/aamt/scaffold.py`

 * *Files identical despite different names*

### Comparing `aamt-0.2.2/pyproject.toml` & `aamt-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aamt"
-version = "0.2.2"
+version = "0.2.3"
 description = "基于pytest的接口自动化测试工具模板"
 authors = ["xuefeng365 <120158568@qq.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/xuefeng365/aamt-template.git"
 repository = "https://github.com/xuefeng365/aamt-template.git"
 packages = [{include = "aamt"}]
```

### Comparing `aamt-0.2.2/README.md` & `aamt-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `aamt-0.2.2/setup.py` & `aamt-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 entry_points = \
 {'console_scripts': ['aamt = aamt.cli:main'],
  'pytest11': ['aamt = aamt.plugin:Plugin']}
 
 setup_kwargs = {
     'name': 'aamt',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': '基于pytest的接口自动化测试工具模板',
     'long_description': '## AAMT 项目模版\n> 用于生成 基于pytest的接口自动化脚手架\n\npython 版本\n\n> 3.9\n\n安装最新版本\n\n> pip install aamt\n\n指定版本安装\n\n> pip install aamt==0.2.2\n\n升级aamt\n\n> pip install -U aamt\n\n创建项目脚手架 \n\n> aamt startproject demo\n\n创建项目脚手架(自动创建虚拟环境)\n\n> aamt startproject demo -venv\n\n外网速度慢，pandas可能安装失败，推荐用国内镜像\n\n> pip --default-timeout=6000 install -i https://pypi.tuna.tsinghua.edu.cn/simple aamt\n\n\n\n',
     'author': 'xuefeng365',
     'author_email': '120158568@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/xuefeng365/aamt-template.git',
```

### Comparing `aamt-0.2.2/PKG-INFO` & `aamt-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aamt
-Version: 0.2.2
+Version: 0.2.3
 Summary: 基于pytest的接口自动化测试工具模板
 Home-page: https://github.com/xuefeng365/aamt-template.git
 License: MIT
 Author: xuefeng365
 Author-email: 120158568@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

