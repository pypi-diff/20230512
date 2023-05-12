# Comparing `tmp/dcicutils-7.4.0.tar.gz` & `tmp/dcicutils-7.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.4.0.tar", max compression
+gzip compressed data, was "dcicutils-7.4.1.tar", max compression
```

## Comparing `dcicutils-7.4.0.tar` & `dcicutils-7.4.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1098 2023-05-01 13:05:57.392337 dcicutils-7.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-05-01 13:05:57.392337 dcicutils-7.4.0/README.rst
--rw-r--r--   0        0        0        0 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3587 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46729 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    31947 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20234 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   154304 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3987 2023-05-01 13:05:57.396337 dcicutils-7.4.0/pyproject.toml
--rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 dcicutils-7.4.0/setup.py
--rw-r--r--   0        0        0     2998 1970-01-01 00:00:00.000000 dcicutils-7.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-12 17:56:15.118342 dcicutils-7.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-05-12 17:56:15.122341 dcicutils-7.4.1/README.rst
+-rw-r--r--   0        0        0        0 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3587 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46739 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    32242 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20234 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   154684 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11044 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3987 2023-05-12 17:56:15.126341 dcicutils-7.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 dcicutils-7.4.1/setup.py
+-rw-r--r--   0        0        0     2998 1970-01-01 00:00:00.000000 dcicutils-7.4.1/PKG-INFO
```

### Comparing `dcicutils-7.4.0/LICENSE.txt` & `dcicutils-7.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/README.rst` & `dcicutils-7.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/base.py` & `dcicutils-7.4.1/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/beanstalk_utils.py` & `dcicutils-7.4.1/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/cloudformation_utils.py` & `dcicutils-7.4.1/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/codebuild_utils.py` & `dcicutils-7.4.1/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/command_utils.py` & `dcicutils-7.4.1/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/common.py` & `dcicutils-7.4.1/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/creds_utils.py` & `dcicutils-7.4.1/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/data_utils.py` & `dcicutils-7.4.1/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/deployment_utils.py` & `dcicutils-7.4.1/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/diff_utils.py` & `dcicutils-7.4.1/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/docker_utils.py` & `dcicutils-7.4.1/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/ecr_scripts.py` & `dcicutils-7.4.1/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/ecr_utils.py` & `dcicutils-7.4.1/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/ecs_utils.py` & `dcicutils-7.4.1/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/env_base.py` & `dcicutils-7.4.1/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/env_manager.py` & `dcicutils-7.4.1/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/env_scripts.py` & `dcicutils-7.4.1/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/env_utils.py` & `dcicutils-7.4.1/dcicutils/env_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     # Although it's fine to call an environment your staging environment without enabling this,
     # what the system means about something being the stg environment is that it's the stage side of a mirror.
     # -kmp 24-Jul-2021
     STAGE_MIRRORING_ENABLED = None  # if True, orchestration-enabled function may offer mirroring behavior
     ORCHESTRATED_APP = None  # This allows us to tell 'cgap' from 'fourfront', in case there ever is one.
     PRD_ENV_NAME = None  # the name of the prod env
     PRODUCTION_ECR_REPOSITORY = None  # the name of an ecr repository shared between stg and prd
-    PUBLIC_URL_TABLE = None  # dictionary mapping envnames & pseudo_envnames to public urls
+    PUBLIC_URL_TABLE = None  # list of dictionaries mapping envnames & pseudo_envnames to public urls
     STG_ENV_NAME = None  # the name of the stage env (or None)
     TEST_ENVS = None  # a list of environments that are for testing
     WEBPROD_PSEUDO_ENV = None
 
     DEV_SUFFIX_FOR_TESTING = ".abc123def456ghi789.us-east-1.rds.amazonaws.com"
 
     SAMPLE_TEMPLATE_FOR_CGAP_TESTING = {
```

### Comparing `dcicutils-7.4.0/dcicutils/env_utils_legacy.py` & `dcicutils-7.4.1/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/es_utils.py` & `dcicutils-7.4.1/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/exceptions.py` & `dcicutils-7.4.1/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/ff_mocks.py` & `dcicutils-7.4.1/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/ff_utils.py` & `dcicutils-7.4.1/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/function_cache_decorator.py` & `dcicutils-7.4.1/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/glacier_utils.py` & `dcicutils-7.4.1/dcicutils/glacier_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                                 version_id: str = None,) -> Union[dict, None]:
         """ Restores a file from glacier given the bucket, key and duration of restore
 
         :param bucket: bucket where the file is stored
         :param key: key under which the file is stored
         :param days: number of days to store in the temporary location
         :param version_id: version ID to restore if applicable
-        :return: response if successful or None
+        :return: response, if successful, or else None
         """
         try:
             args = {
                 'Bucket': bucket,
                 'Key': key,
                 'RestoreRequest': {'Days': days}
             }
@@ -161,15 +161,15 @@
             return response
         except Exception as e:
             PRINT(f'Error restoring object {key} from Glacier storage class: {str(e)}')
             return None
 
     def is_restore_finished(self, bucket: str, key: str) -> bool:
         """ Heads the object to see if it has been restored - note that from the POV of the API,
-            the object is still in Glacier but it has been restored to its original location and
+            the object is still in Glacier, but it has been restored to its original location and
             can be downloaded immediately
 
         :param bucket: bucket of original file location
         :param key: key of original file location
         :return: boolean whether the restore was successful yet
         """
         try:  # extract temporary location by heading object
@@ -229,15 +229,15 @@
 
     def delete_glaciered_object_versions(self, bucket: str, key: str, delete_all_versions: bool = False) -> bool:
         """ Deletes glaciered object versions of the given bucket/key, clearing all versions in glacier if the
             delete_all_versions flag is specified
 
         :param bucket: bucket location containing key
         :param key: file name in s3 to delete
-        :param delete_all_versions: whether or not to delete all glacier versions or just the most recent one
+        :param delete_all_versions: whether to delete all glacier versions or rather than just the most recent one
         :return: True if success or False if failed
         """
         try:
             response = self.s3.list_object_versions(Bucket=bucket, Prefix=key)
             versions = sorted(response.get('Versions', []), key=lambda x: x['LastModified'], reverse=True)
             deleted = False
             for v in versions:
@@ -262,16 +262,16 @@
             to change storage class
 
         :param bucket: bucket to copy from
         :param key: key to copy within bucket
         :param total_size: total size of object
         :param part_size: what size to divide the object into when uploading the chunks
         :param storage_class: new storage class to use
-        :param version_id: object version Id, if applicable
-        :return: response if successful, None otherwise
+        :param version_id: object version ID, if applicable
+        :return: response, if successful, or else None
         """
         try:
             part_size = part_size * 1024 * 1024  # convert MB to B
             num_parts = int(total_size / part_size) + 1
             if num_parts > MAX_MULTIPART_CHUNKS:
                 raise GlacierRestoreException(f'Must user a part_size larger than {part_size}'
                                               f' that will result in fewer than {MAX_MULTIPART_CHUNKS} chunks')
@@ -421,16 +421,17 @@
                     version_id = None
                     for bucket, key in files_meta:
                         if versioning:
                             response = self.s3.list_object_versions(Bucket=bucket, Prefix=key)
                             versions = sorted(response.get('Versions', []), key=lambda x: x['LastModified'],
                                               reverse=True)
                             version_id = versions[0]['VersionId']
-                        future = executor.submit(self.copy_object_back_to_original_location, bucket, key, storage_class,
-                                                 version_id)
+                        future = executor.submit(  # noQA - TODO: PyCharm doesn't like this call for some reason
+                            self.copy_object_back_to_original_location,
+                            bucket=bucket, key=key, storage_class=storage_class, version_id=version_id)
                         futures.append(future)
                 for future in tqdm(futures, total=len(atid_list)):
                     res = future.result()
                     if res:
                         success.append(res)
                     else:
                         errors.append(res)
@@ -444,15 +445,17 @@
                 accumulated_results = []
                 for bucket, key in files_meta:
                     version_id = None
                     if versioning:
                         response = self.s3.list_object_versions(Bucket=bucket, Prefix=key)
                         versions = sorted(response.get('Versions', []), key=lambda x: x['LastModified'], reverse=True)
                         version_id = versions[0]['VersionId']
-                    resp = self.copy_object_back_to_original_location(bucket, key, storage_class, version_id)
+                    resp = self.copy_object_back_to_original_location(bucket=bucket, key=key,
+                                                                      storage_class=storage_class,
+                                                                      version_id=version_id)
                     if resp:
                         accumulated_results.append(_atid)
                 if len(accumulated_results) == len(files_meta):  # all files for this @id were successful
                     success.append(_atid)
                 else:
                     errors.append(_atid)
         if len(errors) != 0:
```

### Comparing `dcicutils-7.4.0/dcicutils/jh_utils.py` & `dcicutils-7.4.1/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/kibana/dashboards.json` & `dcicutils-7.4.1/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/kibana/readme.md` & `dcicutils-7.4.1/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/lang_utils.py` & `dcicutils-7.4.1/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/log_utils.py` & `dcicutils-7.4.1/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/misc_utils.py` & `dcicutils-7.4.1/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/obfuscation_utils.py` & `dcicutils-7.4.1/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/opensearch_utils.py` & `dcicutils-7.4.1/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/qa_checkers.py` & `dcicutils-7.4.1/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/qa_utils.py` & `dcicutils-7.4.1/dcicutils/qa_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,18 +403,18 @@
     def __enter__(self):
         return self.stream
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         content = self.stream.getvalue()
         file_system = self.file_system
         if file_system.exists(self.file):
-            if FILE_SYSTEM_VERBOSE:  # noQA - Debugging option. Doesn't need testing.
+            if FILE_SYSTEM_VERBOSE:  # pragma: no cover - Debugging option. Doesn't need testing.
                 PRINT(f"Preparing to overwrite {self.file}.")
             file_system.prepare_for_overwrite(self.file)
-        if FILE_SYSTEM_VERBOSE:  # noQA - Debugging option. Doesn't need testing.
+        if FILE_SYSTEM_VERBOSE:  # pragma: no cover - Debugging option. Doesn't need testing.
             PRINT(f"Writing {content!r} to {self.file}.")
         file_system.files[self.file] = content if isinstance(content, bytes) else content.encode(self.encoding)
 
 
 class MockFileSystem:
     """Extremely low-tech mock file system."""
 
@@ -455,15 +455,15 @@
 
     def remove(self, file):
         self._maybe_auto_mirror_file(file)
         if self.files.pop(file, None) is None:
             raise FileNotFoundError("No such file or directory: %s" % file)
 
     def open(self, file, mode='r', encoding=None):
-        if FILE_SYSTEM_VERBOSE:  # noQA - Debugging option. Doesn't need testing.
+        if FILE_SYSTEM_VERBOSE:  # pragma: no cover - Debugging option. Doesn't need testing.
             PRINT("Opening %r in mode %r." % (file, mode))
         if mode in ('w', 'wt', 'w+', 'w+t', 'wt+'):
             return self._open_for_write(file_system=self, file=file, binary=False, encoding=encoding)
         elif mode in ('wb', 'w+b', 'wb+'):
             return self._open_for_write(file_system=self, file=file, binary=True, encoding=encoding)
         elif mode in ('r', 'rt', 'r+', 'r+t', 'rt+'):
             return self._open_for_read(file, binary=False, encoding=encoding)
@@ -473,15 +473,15 @@
             raise AssertionError("Mocked io.open doesn't handle mode=%r." % mode)
 
     def _open_for_read(self, file, binary=False, encoding=None):
         self._maybe_auto_mirror_file(file)
         content = self.files.get(file)
         if content is None:
             raise FileNotFoundError("No such file or directory: %s" % file)
-        if FILE_SYSTEM_VERBOSE:  # noQA - Debugging option. Doesn't need testing.
+        if FILE_SYSTEM_VERBOSE:  # pragma: no cover - Debugging option. Doesn't need testing.
             PRINT("Read %r from %s." % (content, file))
         return io.BytesIO(content) if binary else io.StringIO(content.decode(encoding or self.default_encoding))
 
     def _open_for_write(self, file_system, file, binary=False, encoding=None):
         self._do_not_mirror(file)
         return MockFileWriter(file_system=file_system, file=file, binary=binary,
                               encoding=encoding or self.default_encoding)
@@ -2265,21 +2265,25 @@
         "image/png": [".png"],
         "application/json": [".json"],
         "text/plain": [".txt", ".text"],
         "binary/octet-stream": [".fo"],
     }
 
     def put_object(self, *, Bucket, Key, Body, ContentType=None, **kwargs):  # noqa - Uppercase argument names are chosen by AWS
+        # TODO: This is not mocking other args like ACL that we might use ACL='public-read' or ACL='private'
+        #       grep for ACL= in tibanna, tibanna_ff, or dcicutils for examples of these values.
         # TODO: Shouldn't this be checking for required arguments (e.g., for SSE)? -kmp 9-May-2022
         if ContentType is not None:
             exts = self.PUT_OBJECT_CONTENT_TYPES.get(ContentType)
             assert exts, "Unimplemented mock .put_object content type %s for Key=%s" % (ContentType, Key)
             assert any(Key.endswith(ext) for ext in exts), (
                     "mock .put_object expects Key=%s to end in one of %s for ContentType=%s" % (Key, exts, ContentType))
         assert not kwargs, "put_object mock doesn't support %s." % kwargs
+        if isinstance(Body, str):
+            Body = Body.encode('utf-8')  # we just assume utf-8, which AWS seems to as well
         self.s3_files.files[Bucket + "/" + Key] = Body
         return {
             'ETag': self._content_etag(Body)
         }
 
     @staticmethod
     def _content_etag(content):
```

### Comparing `dcicutils-7.4.0/dcicutils/redis_tools.py` & `dcicutils-7.4.1/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/redis_utils.py` & `dcicutils-7.4.1/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/s3_utils.py` & `dcicutils-7.4.1/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.4.1/dcicutils/scripts/publish_to_pypi.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 def verify_git_repo() -> bool:
     """
     If this (the current directory) looks like a git repo then return True,
     otherwise prints a warning and returns False.
     """
     _, status = execute_command("git rev-parse --is-inside-work-tree")
     if status != 0:
-        print("You are not in a git repo directory!")
+        PRINT("You are not in a git repo directory!")
         return False
     return True
 
 
 def verify_unstaged_changes() -> bool:
     """
     If the current git repo has no unstaged changes then returns True,
```

### Comparing `dcicutils-7.4.0/dcicutils/secrets_utils.py` & `dcicutils-7.4.1/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/snapshot_utils.py` & `dcicutils-7.4.1/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.4.1/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/task_utils.py` & `dcicutils-7.4.1/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/dcicutils/trace_utils.py` & `dcicutils-7.4.1/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.0/pyproject.toml` & `dcicutils-7.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.4.0"
+version = "7.4.1"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.4.0/setup.py` & `dcicutils-7.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.4.0',
+    'version': '7.4.1',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.4.0/PKG-INFO` & `dcicutils-7.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.4.0
+Version: 7.4.1
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

