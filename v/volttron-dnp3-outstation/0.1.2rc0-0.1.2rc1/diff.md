# Comparing `tmp/volttron_dnp3_outstation-0.1.2rc0.tar.gz` & `tmp/volttron_dnp3_outstation-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_dnp3_outstation-0.1.2rc0.tar", max compression
+gzip compressed data, was "volttron_dnp3_outstation-0.1.2rc1.tar", max compression
```

## Comparing `volttron_dnp3_outstation-0.1.2rc0.tar` & `volttron_dnp3_outstation-0.1.2rc1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11927 2023-05-12 19:02:11.345475 volttron_dnp3_outstation-0.1.2rc0/LICENSE
--rw-r--r--   0        0        0    17123 2023-05-12 19:02:11.345475 volttron_dnp3_outstation-0.1.2rc0/README.md
--rw-r--r--   0        0        0     2031 2023-05-12 19:04:07.709452 volttron_dnp3_outstation-0.1.2rc0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-12 19:01:16.851476 volttron_dnp3_outstation-0.1.2rc0/src/dnp3_outstation/__init__.py
--rw-r--r--   0        0        0    10014 2023-05-12 19:01:16.851476 volttron_dnp3_outstation-0.1.2rc0/src/dnp3_outstation/agent.py
--rw-r--r--   0        0        0        0 2023-05-12 19:01:16.851476 volttron_dnp3_outstation-0.1.2rc0/src/vdnp3_outstation/__init__.py
--rw-r--r--   0        0        0       89 2023-05-12 19:01:16.851476 volttron_dnp3_outstation-0.1.2rc0/src/vdnp3_outstation/__main__.py
--rw-r--r--   0        0        0    10858 2023-05-12 19:02:11.345475 volttron_dnp3_outstation-0.1.2rc0/src/vdnp3_outstation/run_volttron_dnp3_outstation_cli.py
--rw-r--r--   0        0        0    18492 1970-01-01 00:00:00.000000 volttron_dnp3_outstation-0.1.2rc0/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-05-12 19:04:31.877522 volttron_dnp3_outstation-0.1.2rc1/LICENSE
+-rw-r--r--   0        0        0    17123 2023-05-12 19:04:31.877522 volttron_dnp3_outstation-0.1.2rc1/README.md
+-rw-r--r--   0        0        0     2005 2023-05-12 19:06:24.679016 volttron_dnp3_outstation-0.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-12 19:04:31.877522 volttron_dnp3_outstation-0.1.2rc1/src/dnp3_outstation/__init__.py
+-rw-r--r--   0        0        0    10014 2023-05-12 19:04:31.877522 volttron_dnp3_outstation-0.1.2rc1/src/dnp3_outstation/agent.py
+-rw-r--r--   0        0        0        0 2023-05-12 19:04:31.877522 volttron_dnp3_outstation-0.1.2rc1/src/vdnp3_outstation/__init__.py
+-rw-r--r--   0        0        0       89 2023-05-12 19:04:31.877522 volttron_dnp3_outstation-0.1.2rc1/src/vdnp3_outstation/__main__.py
+-rw-r--r--   0        0        0    10858 2023-05-12 19:04:31.877522 volttron_dnp3_outstation-0.1.2rc1/src/vdnp3_outstation/run_volttron_dnp3_outstation_cli.py
+-rw-r--r--   0        0        0    18710 1970-01-01 00:00:00.000000 volttron_dnp3_outstation-0.1.2rc1/setup.py
+-rw-r--r--   0        0        0    18492 1970-01-01 00:00:00.000000 volttron_dnp3_outstation-0.1.2rc1/PKG-INFO
```

### Comparing `volttron_dnp3_outstation-0.1.2rc0/LICENSE` & `volttron_dnp3_outstation-0.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_dnp3_outstation-0.1.2rc0/README.md` & `volttron_dnp3_outstation-0.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `volttron_dnp3_outstation-0.1.2rc0/pyproject.toml` & `volttron_dnp3_outstation-0.1.2rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ignore_missing_imports = true
 
 [tool.mypy-pytz]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-dnp3-outstation"
-version = "0.1.2rc0"
+version = "0.1.2rc1"
 description = "A Volttron agent that acts as a dnp3 outstation."
 authors = ["Kefei Mo <kefei.mo@pnnl.gov>"]
 license = "Apache-2.0"
 maintainers = ["Volttron Team <volttron@pnnl.gov>"]
 readme = "README.md"
 homepage = "https://github.com/eclipse-volttron/volttron-dnp3-outstation"
 repository = "https://github.com/eclipse-volttron/volttron-dnp3-outstation"
@@ -50,15 +50,14 @@
 pytest = ">=6.2.4"
 pytest-cov = ">=3.0.0"
 pytest-env = ">0.0.0"
 black = ">=21.5b2"
 pre-commit = ">=2.13.0"
 volttron-testing = ">=0.3.1a7"
 mypy = ">=0.982"
-pytest-timeout = "^2.1.0"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = ">=4.5.0"
 sphinx-rtd-theme = ">=1.0.0"
 
 [tool.poetry.scripts]  # entry point (note: vctl start will attempt to run this)
 volttron-dnp3-outstation = "dnp3_outstation.agent:main"
```

### Comparing `volttron_dnp3_outstation-0.1.2rc0/src/dnp3_outstation/agent.py` & `volttron_dnp3_outstation-0.1.2rc1/src/dnp3_outstation/agent.py`

 * *Files identical despite different names*

### Comparing `volttron_dnp3_outstation-0.1.2rc0/src/vdnp3_outstation/run_volttron_dnp3_outstation_cli.py` & `volttron_dnp3_outstation-0.1.2rc1/src/vdnp3_outstation/run_volttron_dnp3_outstation_cli.py`

 * *Files identical despite different names*

### Comparing `volttron_dnp3_outstation-0.1.2rc0/PKG-INFO` & `volttron_dnp3_outstation-0.1.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-dnp3-outstation
-Version: 0.1.2rc0
+Version: 0.1.2rc1
 Summary: A Volttron agent that acts as a dnp3 outstation.
 Home-page: https://github.com/eclipse-volttron/volttron-dnp3-outstation
 License: Apache-2.0
 Keywords: volttron,agent,dnp3,outstation,application
 Author: Kefei Mo
 Author-email: kefei.mo@pnnl.gov
 Maintainer: Volttron Team
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volttron-dnp3-outstation Version: 0.1.2rc0 Summary:
+Metadata-Version: 2.1 Name: volttron-dnp3-outstation Version: 0.1.2rc1 Summary:
 A Volttron agent that acts as a dnp3 outstation. Home-page: https://github.com/
 eclipse-volttron/volttron-dnp3-outstation License: Apache-2.0 Keywords:
 volttron,agent,dnp3,outstation,application Author: Kefei Mo Author-email:
 kefei.mo@pnnl.gov Maintainer: Volttron Team Maintainer-email: volttron@pnnl.gov
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: Apache Software License
```

