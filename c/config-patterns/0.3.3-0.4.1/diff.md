# Comparing `tmp/config_patterns-0.3.3.tar.gz` & `tmp/config_patterns-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_patterns-0.3.3.tar", last modified: Sun Mar 19 18:26:55 2023, max compression
+gzip compressed data, was "config_patterns-0.4.1.tar", last modified: Fri May 12 18:21:35 2023, max compression
```

## Comparing `config_patterns-0.3.3.tar` & `config_patterns-0.4.1.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-19 18:26:55.418138 config_patterns-0.3.3/
--rw-r--r--   0 sanhehu    (505) staff       (20)      509 2023-02-04 16:31:06.000000 config_patterns-0.3.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     1125 2023-02-04 16:31:06.000000 config_patterns-0.3.3/LICENSE.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      323 2023-02-04 16:31:06.000000 config_patterns-0.3.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)     4016 2023-03-19 18:26:55.417984 config_patterns-0.3.3/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     2892 2023-03-19 18:26:24.000000 config_patterns-0.3.3/README.rst
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-19 18:26:55.413572 config_patterns-0.3.3/config_patterns/
--rw-r--r--   0 sanhehu    (505) staff       (20)      303 2023-03-19 18:25:14.000000 config_patterns-0.3.3/config_patterns/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-03-19 18:23:31.000000 config_patterns-0.3.3/config_patterns/_version.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-19 18:26:55.415140 config_patterns-0.3.3/config_patterns/aws/
--rw-r--r--   0 sanhehu    (505) staff       (20)        0 2023-02-05 15:33:20.000000 config_patterns-0.3.3/config_patterns/aws/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2134 2023-03-19 18:14:46.000000 config_patterns-0.3.3/config_patterns/aws/s3.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2462 2023-03-19 17:57:37.000000 config_patterns-0.3.3/config_patterns/aws/ssm.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      128 2023-02-04 16:59:17.000000 config_patterns-0.3.3/config_patterns/compat.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-19 18:26:55.415422 config_patterns-0.3.3/config_patterns/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2023-02-04 16:31:06.000000 config_patterns-0.3.3/config_patterns/docs/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1406 2023-02-04 21:58:48.000000 config_patterns-0.3.3/config_patterns/jsonutils.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1094 2023-02-04 16:45:15.000000 config_patterns-0.3.3/config_patterns/paths.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-19 18:26:55.415850 config_patterns-0.3.3/config_patterns/patterns/
--rw-r--r--   0 sanhehu    (505) staff       (20)        0 2023-02-04 16:36:01.000000 config_patterns-0.3.3/config_patterns/patterns/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    21150 2023-03-19 18:20:50.000000 config_patterns-0.3.3/config_patterns/patterns/multi_env_json.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-19 18:26:55.416716 config_patterns-0.3.3/config_patterns/tests/
--rw-r--r--   0 sanhehu    (505) staff       (20)       58 2022-12-10 20:46:07.000000 config_patterns-0.3.3/config_patterns/tests/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      241 2022-12-10 20:46:07.000000 config_patterns-0.3.3/config_patterns/tests/boto_ses.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1216 2022-12-10 20:46:07.000000 config_patterns-0.3.3/config_patterns/tests/helper.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-19 18:26:55.417279 config_patterns-0.3.3/config_patterns/vendor/
--rw-r--r--   0 sanhehu    (505) staff       (20)       25 2023-02-04 16:40:33.000000 config_patterns-0.3.3/config_patterns/vendor/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    44420 2023-02-04 16:40:34.000000 config_patterns-0.3.3/config_patterns/vendor/strutils.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-19 18:26:55.414562 config_patterns-0.3.3/config_patterns.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)     4016 2023-03-19 18:26:55.000000 config_patterns-0.3.3/config_patterns.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)      875 2023-03-19 18:26:55.000000 config_patterns-0.3.3/config_patterns.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-03-19 18:26:55.000000 config_patterns-0.3.3/config_patterns.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      433 2023-03-19 18:26:55.000000 config_patterns-0.3.3/config_patterns.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       16 2023-03-19 18:26:55.000000 config_patterns-0.3.3/config_patterns.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)     1752 2023-03-19 18:24:32.000000 config_patterns-0.3.3/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)       73 2023-02-12 06:33:55.000000 config_patterns-0.3.3/requirements-aws.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      370 2023-02-05 20:32:10.000000 config_patterns-0.3.3/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      621 2023-02-04 16:31:06.000000 config_patterns-0.3.3/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      183 2023-02-04 16:31:06.000000 config_patterns-0.3.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       65 2023-02-12 04:28:31.000000 config_patterns-0.3.3/requirements.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-03-19 18:26:55.418186 config_patterns-0.3.3/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     7961 2023-02-12 04:28:39.000000 config_patterns-0.3.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.070524 config_patterns-0.4.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 01:08:10.000000 config_patterns-0.4.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-05-12 01:08:10.000000 config_patterns-0.4.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      323 2023-05-12 01:08:10.000000 config_patterns-0.4.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4016 2023-05-12 18:21:35.070383 config_patterns-0.4.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2892 2023-05-12 01:08:10.000000 config_patterns-0.4.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.067404 config_patterns-0.4.1/config_patterns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      303 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-12 18:21:00.000000 config_patterns-0.4.1/config_patterns/_version.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.068493 config_patterns-0.4.1/config_patterns/aws/
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/aws/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5169 2023-05-12 16:38:32.000000 config_patterns-0.4.1/config_patterns/aws/s3.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2792 2023-05-12 16:35:47.000000 config_patterns-0.4.1/config_patterns/aws/ssm.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.068601 config_patterns-0.4.1/config_patterns/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1406 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/jsonutils.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      182 2023-05-12 03:09:13.000000 config_patterns-0.4.1/config_patterns/logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      724 2023-05-12 03:09:31.000000 config_patterns-0.4.1/config_patterns/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.068829 config_patterns-0.4.1/config_patterns/patterns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/patterns/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    22411 2023-05-12 18:09:09.000000 config_patterns-0.4.1/config_patterns/patterns/multi_env_json.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.069308 config_patterns-0.4.1/config_patterns/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      149 2023-05-12 03:10:02.000000 config_patterns-0.4.1/config_patterns/tests/boto_ses.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1216 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.069769 config_patterns-0.4.1/config_patterns/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-12 15:37:26.000000 config_patterns-0.4.1/config_patterns/vendor/nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    44420 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/vendor/strutils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.068043 config_patterns-0.4.1/config_patterns.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4016 2023-05-12 18:21:35.000000 config_patterns-0.4.1/config_patterns.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      960 2023-05-12 18:21:35.000000 config_patterns-0.4.1/config_patterns.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-12 18:21:35.000000 config_patterns-0.4.1/config_patterns.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      438 2023-05-12 18:21:35.000000 config_patterns-0.4.1/config_patterns.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       16 2023-05-12 18:21:35.000000 config_patterns-0.4.1/config_patterns.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2126 2023-05-12 18:20:49.000000 config_patterns-0.4.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)       73 2023-05-12 18:03:12.000000 config_patterns-0.4.1/requirements-aws.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-05-12 01:08:10.000000 config_patterns-0.4.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-12 01:08:10.000000 config_patterns-0.4.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-05-12 16:53:20.000000 config_patterns-0.4.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       65 2023-05-12 01:08:10.000000 config_patterns-0.4.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-12 18:21:35.070567 config_patterns-0.4.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7961 2023-05-12 01:08:10.000000 config_patterns-0.4.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.070101 config_patterns-0.4.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      258 2023-05-12 01:08:10.000000 config_patterns-0.4.1/tests/test_import.py
```

### Comparing `config_patterns-0.3.3/LICENSE.txt` & `config_patterns-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `config_patterns-0.3.3/PKG-INFO` & `config_patterns-0.4.1/config_patterns.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: config_patterns
-Version: 0.3.3
+Name: config-patterns
+Version: 0.4.1
 Summary: Implement common config management patterns.
 Home-page: https://github.com/MacHu-GWU/config_patterns-project
-Download-URL: https://pypi.python.org/pypi/config_patterns/0.3.3#downloads
+Download-URL: https://pypi.python.org/pypi/config_patterns/0.4.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `config_patterns-0.3.3/README.rst` & `config_patterns-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `config_patterns-0.3.3/config_patterns/aws/ssm.py` & `config_patterns-0.4.1/config_patterns/aws/ssm.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,20 @@
     import boto3
     import boto_session_manager
     import pysecret
     import aws_console_url
 except ImportError:  # pragma: no cover
     pass
 
+from ..logger import logger
 
+
+@logger.start_and_end(
+    msg="deploy config to SSM parameter",
+)
 def deploy_parameter(
     bsm: "boto_session_manager.BotoSesManager",
     parameter_name: str,
     parameter_data: dict,
     parameter_with_encryption: bool,
     tags: T.Optional[dict] = None,
 ) -> T.Optional["pysecret.Parameter"]:
@@ -26,58 +31,63 @@
     Deploy (Create or Update) AWS SSM parameter store.
 
     :param bsm: the ``boto_session_manager.BotoSesManager`` object.
     :param parameter_name: parameter name.
     :param parameter_data: parameter data in python dict.
     :param parameter_with_encryption: do you want to encrypt the data at rest?
     :param tags: optional key value tags.
+
+    :return: a ``pysecret.Parameter`` object to indicate the deployed parameter.
+        if returns None, then no deployment happened.
     """
     aws_console = aws_console_url.AWSConsole(aws_region=bsm.aws_region)
-    print(f"🚀️ deploy SSM Parameter {parameter_name!r} ...")
-    print(f"preview at: {aws_console.ssm.get_parameter(parameter_name)}")
+    logger.info(f"🚀️ deploy SSM Parameter {parameter_name!r} ...")
+    logger.info(f"preview at: {aws_console.ssm.get_parameter(parameter_name)}")
     parameter = pysecret.deploy_parameter(
         bsm.ssm_client,
         name=parameter_name,
         data=parameter_data,
         use_default_kms_key=parameter_with_encryption,
         type_is_secure_string=True,
         tier_is_intelligent=True,
         tags=tags,
         overwrite=True,
     )
     if parameter is None:
-        print("parameter data is the same as existing one, do nothing.")
+        logger.info("parameter data is the same as existing one, do nothing.")
     else:
-        print(f"successfully deployed version {parameter.Version}")
-    print("done!")
+        logger.info(f"successfully deployed version {parameter.Version}")
     return parameter
 
 
+@logger.start_and_end(
+    msg="delete config from SSM parameter",
+)
 def delete_parameter(
     bsm: "boto_session_manager.BotoSesManager",
     parameter_name: str,
 ) -> bool:
     """
     Delete AWS SSM parameter.
 
     Ref:
 
     - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_parameter
 
     :return: a boolean value indicating whether a deletion happened.
     """
     aws_console = aws_console_url.AWSConsole(aws_region=bsm.aws_region)
-    print(f"🗑️ delete SSM Parameter {parameter_name!r} ...")
-    print(f"verify at: {aws_console.ssm.get_parameter(parameter_name)}")
+    logger.info(f"🗑️ delete SSM Parameter {parameter_name!r} ...")
+    logger.info(f"verify at: {aws_console.ssm.get_parameter(parameter_name)}")
 
     try:
         bsm.ssm_client.delete_parameter(Name=parameter_name)
         delete_happened = True
     except Exception as e:
         if "ParameterNotFound" in str(e):
-            print("not exists, do nothing.")
+            logger.info("not exists, do nothing.")
             delete_happened = False
         else:
             raise e
 
-    print("done!")
+    logger.info("done!")
     return delete_happened
```

### Comparing `config_patterns-0.3.3/config_patterns/jsonutils.py` & `config_patterns-0.4.1/config_patterns/jsonutils.py`

 * *Files identical despite different names*

### Comparing `config_patterns-0.3.3/config_patterns/patterns/multi_env_json.py` & `config_patterns-0.4.1/config_patterns/patterns/multi_env_json.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
 #
 try:
     import pysecret
     import aws_console_url
 
     from ..aws.ssm import deploy_parameter, delete_parameter
-    from ..aws.s3 import deploy_config, delete_config
+    from ..aws.s3 import deploy_config, delete_config, S3Object
 except ImportError:  # pragma: no cover
     pass
 
-
+from ..logger import logger
 from ..jsonutils import json_loads
 from ..compat import cached_property
 from ..vendor.strutils import camel2under, slugify
 
 
 def validate_project_name(project_name: str):
     if project_name[0] not in string.ascii_lowercase:
@@ -161,24 +161,137 @@
 
 
 @dataclasses.dataclass
 class ConfigDeployment:
     """
     Represent a config deployment on remote data store.
 
-    :param uri: the unique resource identifier to the config data store.
-        for AWS, it is the ARN
-    :param data: the config data in python dict
+    It has the following methods:
+
+    - :meth:`~ConfigDeployment.deploy_to_ssm_parameter`
+    - :meth:`~ConfigDeployment.deploy_to_s3`
+    - :meth:`~ConfigDeployment.delete_from_ssm_parameter`
+    - :meth:`~ConfigDeployment.delete_from_s3`
+
+    :param parameter_name: the logic name of this deployment
+    :param parameter_data: the config data in python dict
     :param project_name: project name
     :param env_name: environment name
+    :param deployment: the deployment object, it can be either AWS Parameter or S3 Object
+    :param deletion: whether there is a deletion happened
     """
-    uri: str = dataclasses.field()
-    data: dict = dataclasses.field()
+
+    parameter_name: str = dataclasses.field()
+    parameter_data: dict = dataclasses.field()
     project_name: str = dataclasses.field()
     env_name: str = dataclasses.field()
+    deployment: T.Optional[T.Union["pysecret.Parameter", S3Object]] = dataclasses.field(
+        default=None
+    )
+    deletion: T.Optional[bool] = dataclasses.field(default=None)
+
+    @property
+    def parameter_name_for_arn(self) -> str:
+        """
+        Return the parameter name for ARN. The parameter name could have
+        a leading "/", in this case, we should strip it out.
+        """
+        if self.parameter_name.startswith("/"):  # pragma: no cover
+            return self.parameter_name[1:]
+        else:
+            return self.parameter_name
+
+    def deploy_to_ssm_parameter(
+        self,
+        bsm: "boto_session_manager.BotoSesManager",
+        parameter_with_encryption: bool,
+        tags: T.Optional[T.Dict[str, str]] = None,
+        verbose: bool = True,
+    ):
+        """
+        Deploy config to AWS SSM Parameter Store.
+        """
+        if tags is None:
+            tags = dict(
+                ProjectName=self.project_name,
+                EnvName=self.env_name,
+            )
+        with logger.disabled(
+            disable=not verbose,
+        ):
+            self.deployment = deploy_parameter(
+                bsm=bsm,
+                parameter_name=self.parameter_name,
+                parameter_data=self.parameter_data,
+                parameter_with_encryption=parameter_with_encryption,
+                tags=tags,
+            )
+            return self.deployment
+
+    def deploy_to_s3(
+        self,
+        bsm: "boto_session_manager.BotoSesManager",
+        s3dir_config: str,
+        tags: T.Optional[T.Dict[str, str]] = None,
+        verbose: bool = True,
+    ):
+        """
+        Deploy config to AWS S3.
+        """
+        if tags is None:
+            tags = dict(
+                ProjectName=self.project_name,
+                EnvName=self.env_name,
+            )
+        with logger.disabled(
+            disable=not verbose,
+        ):
+            self.deployment = deploy_config(
+                bsm=bsm,
+                s3path_config=f"{s3dir_config}{self.parameter_name_for_arn}.json",
+                config_data=self.parameter_data,
+                tags=tags,
+            )
+            return self.deployment
+
+    def delete_from_ssm_parameter(
+        self,
+        bsm: "boto_session_manager.BotoSesManager",
+        verbose: bool = True,
+    ):
+        """
+        Delete config from AWS SSM Parameter Store.
+        """
+        with logger.disabled(
+            disable=not verbose,
+        ):
+            self.deletion = delete_parameter(
+                bsm=bsm,
+                parameter_name=self.parameter_name,
+            )
+            return self.deletion
+
+    def delete_from_s3(
+        self,
+        bsm: "boto_session_manager.BotoSesManager",
+        s3dir_config: str,
+        verbose: bool = True,
+    ):
+        """
+        Delete config from AWS S3.
+        """
+        with logger.disabled(
+            disable=not verbose,
+        ):
+            s3_uri = f"{s3dir_config}{self.parameter_name_for_arn}.json"
+            self.deletion = delete_config(
+                bsm=bsm,
+                s3path_config=s3_uri,
+            )
+            return self.deletion
 
 
 @dataclasses.dataclass
 class BaseConfig:
     """
     The base class for multi-environment config object.
 
@@ -382,31 +495,33 @@
                 "you want to read config from local config json file.\n"
                 "2. set both ``parameter_name`` and ``parameter_with_encryption`` "
                 "to indicate that you want to read from AWS Parameter Store.\n"
                 "3. set ``s3path_config`` similar to s3://my-bucket/my-project/dev.json "
                 "to indicate that you want to read from AWS S3.\n"
             )
 
-    def _prepare_deploy(
-        self,
-    ) -> T.List[T.Tuple[str, dict, str, str]]:  # pragma: no cover
+    def prepare_deploy(self) -> T.List[ConfigDeployment]:
         """
         split the consolidated config into per environment config.
 
-        :return a list of tuple, each tuple has four item: 1. parameter_name,
-            2. parameter_data, 3. project_name, 4. env_name.
+        :return a list of deployment.
         """
-        parameter_list: T.List[T.Tuple[str, dict, str, str]] = list()
+        deployment_list: T.List[ConfigDeployment] = list()
 
         # manually add all env parameter, the name is project_name only
         # without env_name
         parameter_name = self.parameter_name
         parameter_data = {"data": self.data, "secret_data": self.secret_data}
-        parameter_list.append(
-            (parameter_name, parameter_data, self.project_name, "all")
+        deployment_list.append(
+            ConfigDeployment(
+                parameter_name=parameter_name,
+                parameter_data=parameter_data,
+                project_name=self.project_name,
+                env_name="all",
+            )
         )
 
         # add per env parameter
         for env_name in self.EnvEnum:
             env_name = self.EnvEnum.ensure_str(env_name)
             env = self.get_env(env_name)
             parameter_name = env.parameter_name
@@ -416,181 +531,130 @@
                     "envs": {env.env_name: self.data["envs"][env.env_name]},
                 },
                 "secret_data": {
                     "shared": self.secret_data["shared"],
                     "envs": {env.env_name: self.secret_data["envs"][env.env_name]},
                 },
             }
-            parameter_list.append(
-                (parameter_name, parameter_data, env.project_name, env.env_name)
+            deployment_list.append(
+                ConfigDeployment(
+                    parameter_name=parameter_name,
+                    parameter_data=parameter_data,
+                    project_name=env.project_name,
+                    env_name=env.env_name,
+                )
             )
 
-        return parameter_list
+        return deployment_list
 
     def deploy(
         self,
         bsm: "boto_session_manager.BotoSesManager",
         parameter_with_encryption: T.Optional[bool] = None,
         s3dir_config: T.Optional[str] = None,
         tags: T.Optional[T.Dict[str, str]] = None,
-    ) -> T.List[T.Optional[ConfigDeployment]]:  # pragma: no cover
+        verbose: bool = True,
+    ) -> T.List[ConfigDeployment]:
         """
         Deploy the project config of all environments to configuration store.
         Currently, it supports:
 
         1. deploy to AWS Parameter Store
         2. deploy to AWS S3
 
+        Note:
+
+            this function should ONLY run from the project admin's trusted laptop.
+
         :param bsm:
         :param parameter_with_encryption:
         :param s3dir_config:
+        :param tags:
+        :param verbose:
 
-        Note:
-
-            this function should ONLY run from the project admin's trusted laptop.
+        :return: a list of :class:`ConfigDeployment`.
         """
-        config_deployment_list: T.List[T.Optional[ConfigDeployment]] = list()
         if parameter_with_encryption is not None:
             # validate arguments
             if not (
                 (parameter_with_encryption is True)
                 or (parameter_with_encryption is False)
             ):
-                raise ValueError
-            print("deploy parameter store for all environment")
-            parameter_list = self._prepare_deploy()
-            for (
-                parameter_name,
-                parameter_data,
-                project_name,
-                env_name,
-            ) in parameter_list:
-                if tags is None:
-                    tags = dict(
-                        ProjectName=project_name,
-                        EnvName=env_name,
-                    )
-                deploy_parameter(
+                raise ValueError("parameter_with_encryption has to be True or False!")
+            deployment_list = self.prepare_deploy()
+            for deployment in deployment_list:
+                deployment.deploy_to_ssm_parameter(
                     bsm=bsm,
-                    parameter_name=parameter_name,
-                    parameter_data=parameter_data,
                     parameter_with_encryption=parameter_with_encryption,
                     tags=tags,
+                    verbose=verbose,
                 )
-                config_deployment_list.append(
-                    ConfigDeployment(
-                        uri=f"arn:aws:ssm:{bsm.aws_region}:{bsm.aws_account_id}:parameter/{parameter_name}",
-                        data=parameter_data,
-                        project_name=project_name,
-                        env_name=env_name,
-                    )
-                )
-            return config_deployment_list
+            return deployment_list
         elif s3dir_config is not None:
-            if not s3dir_config.endswith("/"):
-                raise ValueError(
-                    "s3dir_config has to be a folder and end with /, "
-                    "a valid example: 's3://my-bucket/my-project/'."
-                )
-            parameter_list = self._prepare_deploy()
-            # s3_uri = deploy_config(
-            #     bsm=bsm,
-            #     s3path_config=f"{s3dir_config}all.json",
-            #     config_data=parameter_list[0][1],
-            #     tags=dict(
-            #         ProjectName=parameter_list[0][2],
-            #         EnvName=parameter_list[0][3],
-            #     ),
-            # )
-            # config_deployment_list.append(
-            #     ConfigDeployment(
-            #         uri=s3_uri,
-            #         data=parameter_list[0][1],
-            #         project_name=parameter_list[0][2],
-            #         env_name=parameter_list[0][3],
-            #     )
-            # )
-
-            for parameter_name, parameter_data, project_name, env_name in parameter_list:
-                if tags is None:
-                    tags = dict(
-                        ProjectName=project_name,
-                        EnvName=env_name,
-                    )
-                s3_uri = deploy_config(
+            deployment_list = self.prepare_deploy()
+            for deployment in deployment_list:
+                deployment.deploy_to_s3(
                     bsm=bsm,
-                    s3path_config=f"{s3dir_config}{parameter_name}.json",
-                    config_data=parameter_data,
+                    s3dir_config=s3dir_config,
                     tags=tags,
+                    verbose=verbose,
                 )
-                config_deployment_list.append(
-                    ConfigDeployment(
-                        uri=s3_uri,
-                        data=parameter_data,
-                        project_name=project_name,
-                        env_name=env_name,
-                    )
-                )
-            return config_deployment_list
+            return deployment_list
         else:
             raise ValueError(
                 "The arguments has to meet one of these criteria:\n"
                 "1. set ``parameter_with_encryption`` to True or False to indicate that "
                 "you want to deploy to AWS Parameter Store.\n"
                 "2. set ``s3dir_config`` similar to s3://my-bucket/my-project/ "
                 "to indicate that you want to deploy to S3."
             )
 
     def delete(
         self,
         bsm: "boto_session_manager.BotoSesManager",
         use_parameter_store: T.Optional[bool] = None,
         s3dir_config: T.Optional[str] = None,
-    ):  # pragma: no cover
+        verbose: bool = True,
+    ):
         """
         Delete the all project config of all environments from configuration store.
 
         Currently, it supports:
 
         1. delete from AWS Parameter Store
         2. delete from AWS S3
 
         :param bsm:
         :param use_parameter_store:
         :param s3dir_config:
+        :param verbose:
+
+        :return: a list of :class:`ConfigDeployment`.
 
         Note:
 
             this function should ONLY run from the project admin's trusted laptop.
         """
         if (bsm is not None) and (use_parameter_store is True):
-            print("delete parameter store for all environment")
-            parameter_list = self._prepare_deploy()
-            for parameter_name, _, _, _ in parameter_list:
-                delete_parameter(
+            deployment_list = self.prepare_deploy()
+            for deployment in deployment_list:
+                deployment.delete_from_ssm_parameter(
                     bsm=bsm,
-                    parameter_name=parameter_name,
+                    verbose=verbose,
                 )
+            return deployment_list
         elif (bsm is not None) and (s3dir_config is not None):
-            if not s3dir_config.endswith("/"):
-                raise ValueError(
-                    "s3dir_config has to be a folder and end with /, "
-                    "a valid example: s3://my-bucket/my-project/."
-                )
-            parameter_list = self._prepare_deploy()
-            # delete_config(
-            #     bsm=bsm,
-            #     s3path_config=f"{s3dir_config}{pro}.json",
-            # )
-
-            for parameter_name, _, _, _ in parameter_list:
-                delete_config(
+            deployment_list = self.prepare_deploy()
+            for deployment in deployment_list:
+                deployment.delete_from_s3(
                     bsm=bsm,
-                    s3path_config=f"{s3dir_config}{parameter_name}.json",
+                    s3dir_config=s3dir_config,
+                    verbose=verbose,
                 )
+            return deployment_list
         else:
             raise ValueError(
                 "The arguments has to meet one of these criteria:\n"
                 "1. set ``use_parameter_store`` to True to indicate that "
                 "you want to delete config from AWS Parameter Store.\n"
                 "2. set ``s3dir_config`` similar to s3://my-bucket/my-project/ "
                 "to indicate that you want to delete config file from S3."
```

### Comparing `config_patterns-0.3.3/config_patterns/tests/helper.py` & `config_patterns-0.4.1/config_patterns/tests/helper.py`

 * *Files identical despite different names*

### Comparing `config_patterns-0.3.3/config_patterns/vendor/strutils.py` & `config_patterns-0.4.1/config_patterns/vendor/strutils.py`

 * *Files identical despite different names*

### Comparing `config_patterns-0.3.3/config_patterns.egg-info/PKG-INFO` & `config_patterns-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: config-patterns
-Version: 0.3.3
+Name: config_patterns
+Version: 0.4.1
 Summary: Implement common config management patterns.
 Home-page: https://github.com/MacHu-GWU/config_patterns-project
-Download-URL: https://pypi.python.org/pypi/config_patterns/0.3.3#downloads
+Download-URL: https://pypi.python.org/pypi/config_patterns/0.4.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `config_patterns-0.3.3/config_patterns.egg-info/SOURCES.txt` & `config_patterns-0.4.1/config_patterns.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 requirements-test.txt
 requirements.txt
 setup.py
 config_patterns/__init__.py
 config_patterns/_version.py
 config_patterns/compat.py
 config_patterns/jsonutils.py
+config_patterns/logger.py
 config_patterns/paths.py
 config_patterns.egg-info/PKG-INFO
 config_patterns.egg-info/SOURCES.txt
 config_patterns.egg-info/dependency_links.txt
 config_patterns.egg-info/requires.txt
 config_patterns.egg-info/top_level.txt
 config_patterns/aws/__init__.py
@@ -25,8 +26,10 @@
 config_patterns/docs/__init__.py
 config_patterns/patterns/__init__.py
 config_patterns/patterns/multi_env_json.py
 config_patterns/tests/__init__.py
 config_patterns/tests/boto_ses.py
 config_patterns/tests/helper.py
 config_patterns/vendor/__init__.py
-config_patterns/vendor/strutils.py
+config_patterns/vendor/nest_logger.py
+config_patterns/vendor/strutils.py
+tests/test_import.py
```

### Comparing `config_patterns-0.3.3/release-history.rst` & `config_patterns-0.4.1/release-history.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,25 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.4.1 (2023-05-12)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- the :mod:`config_pattern.patterns.multi_env_json` now support deploying to multiple AWS Account with different AWS profiles.
+
+**Minor Improvements**
+
+- refactor the :mod:`config_pattern.patterns.multi_env_json` to make it more maintainable.
+
+
 0.3.3 (2023-03-19)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - the ``config_pattern.patterns.multi_env_json.BaseConfig.deploy`` method now returns a list of ``config_pattern.patterns.multi_env_json.ConfigDeployment``deployment`` objects.
```

### Comparing `config_patterns-0.3.3/requirements-doc.txt` & `config_patterns-0.4.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `config_patterns-0.3.3/setup.py` & `config_patterns-0.4.1/setup.py`

 * *Files identical despite different names*

