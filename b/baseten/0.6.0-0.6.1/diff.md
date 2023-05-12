# Comparing `tmp/baseten-0.6.0.tar.gz` & `tmp/baseten-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseten-0.6.0.tar", max compression
+gzip compressed data, was "baseten-0.6.1.tar", max compression
```

## Comparing `baseten-0.6.0.tar` & `baseten-0.6.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     5041 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/__init__.py
--rw-r--r--   0        0        0    12867 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/baseten_deployed_model.py
--rw-r--r--   0        0        0     5539 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/cli.py
--rw-r--r--   0        0        0      541 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/client_commands/baseten_cli.py
--rw-r--r--   0        0        0     1143 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/client_commands/dataset_cli.py
--rw-r--r--   0        0        0     5953 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/client_commands/finetuning_cli.py
--rw-r--r--   0        0        0     1088 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/client_commands/models_cli.py
--rw-r--r--   0        0        0      927 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/client_commands/pretrained_cli.py
--rw-r--r--   0        0        0        0 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/__init__.py
--rw-r--r--   0        0        0    29147 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/api.py
--rw-r--r--   0        0        0     2512 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/core.py
--rw-r--r--   0        0        0     1475 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/error_handler.py
--rw-r--r--   0        0        0     6576 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/files.py
--rw-r--r--   0        0        0     4292 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/lib_support.py
--rw-r--r--   0        0        0    18044 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/model_deployer.py
--rw-r--r--   0        0        0     2847 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/settings.py
--rw-r--r--   0        0        0     1787 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/tar.py
--rw-r--r--   0        0        0      907 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/types.py
--rw-r--r--   0        0        0     3413 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/util.py
--rw-r--r--   0        0        0      207 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/__init__.py
--rw-r--r--   0        0        0     7086 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/flan_t5.py
--rw-r--r--   0        0        0      284 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/foundational_model.py
--rw-r--r--   0        0        0     5130 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/llama.py
--rw-r--r--   0        0        0    13478 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/stable_diffusion.py
--rw-r--r--   0        0        0     4878 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/util.py
--rw-r--r--   0        0        0     3481 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/whisper.py
--rw-r--r--   0        0        0      389 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/training/__init__.py
--rw-r--r--   0        0        0     2852 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/training/datasets.py
--rw-r--r--   0        0        0    33964 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/training/finetuning.py
--rw-r--r--   0        0        0     6681 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/training/logs.py
--rw-r--r--   0        0        0      479 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/training/utils.py
--rw-r--r--   0        0        0      763 2023-04-13 00:37:53.974550 baseten-0.6.0/pypi_readme.md
--rw-r--r--   0        0        0     2008 2023-04-13 00:40:03.950711 baseten-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 baseten-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     5041 2023-03-14 19:25:36.820485 baseten-0.6.1/baseten/__init__.py
+-rw-r--r--   0        0        0    12867 2023-04-26 05:33:19.913195 baseten-0.6.1/baseten/baseten_deployed_model.py
+-rw-r--r--   0        0        0     5539 2023-03-14 19:25:36.820729 baseten-0.6.1/baseten/cli.py
+-rw-r--r--   0        0        0      541 2023-02-14 00:04:32.681509 baseten-0.6.1/baseten/client_commands/baseten_cli.py
+-rw-r--r--   0        0        0     1143 2023-03-14 19:25:36.820839 baseten-0.6.1/baseten/client_commands/dataset_cli.py
+-rw-r--r--   0        0        0     5953 2023-03-14 19:25:36.820951 baseten-0.6.1/baseten/client_commands/finetuning_cli.py
+-rw-r--r--   0        0        0     1088 2023-02-14 00:04:32.681737 baseten-0.6.1/baseten/client_commands/models_cli.py
+-rw-r--r--   0        0        0      927 2023-02-14 00:04:32.681832 baseten-0.6.1/baseten/client_commands/pretrained_cli.py
+-rw-r--r--   0        0        0        0 2020-02-24 19:56:47.919582 baseten-0.6.1/baseten/common/__init__.py
+-rw-r--r--   0        0        0    29181 2023-04-26 05:33:19.913453 baseten-0.6.1/baseten/common/api.py
+-rw-r--r--   0        0        0     2512 2023-03-14 19:25:36.821235 baseten-0.6.1/baseten/common/core.py
+-rw-r--r--   0        0        0     1475 2023-02-14 00:04:32.682197 baseten-0.6.1/baseten/common/error_handler.py
+-rw-r--r--   0        0        0     6576 2023-04-26 05:33:19.913604 baseten-0.6.1/baseten/common/files.py
+-rw-r--r--   0        0        0     4292 2023-02-14 00:04:32.682365 baseten-0.6.1/baseten/common/lib_support.py
+-rw-r--r--   0        0        0    18084 2023-04-26 05:34:55.796434 baseten-0.6.1/baseten/common/model_deployer.py
+-rw-r--r--   0        0        0     2847 2023-03-14 19:25:36.821572 baseten-0.6.1/baseten/common/settings.py
+-rw-r--r--   0        0        0     1787 2023-04-26 05:33:19.913952 baseten-0.6.1/baseten/common/tar.py
+-rw-r--r--   0        0        0      907 2023-02-14 00:04:32.682690 baseten-0.6.1/baseten/common/types.py
+-rw-r--r--   0        0        0     3413 2023-04-26 05:33:19.914225 baseten-0.6.1/baseten/common/util.py
+-rw-r--r--   0        0        0      207 2023-04-26 05:33:19.915001 baseten-0.6.1/baseten/models/__init__.py
+-rw-r--r--   0        0        0     7086 2023-04-26 05:33:19.915160 baseten-0.6.1/baseten/models/flan_t5.py
+-rw-r--r--   0        0        0      284 2023-03-14 19:25:36.821929 baseten-0.6.1/baseten/models/foundational_model.py
+-rw-r--r--   0        0        0     5130 2023-04-26 05:33:19.915251 baseten-0.6.1/baseten/models/llama.py
+-rw-r--r--   0        0        0    13478 2023-03-14 19:25:36.822053 baseten-0.6.1/baseten/models/stable_diffusion.py
+-rw-r--r--   0        0        0     4878 2023-02-14 00:04:32.683173 baseten-0.6.1/baseten/models/util.py
+-rw-r--r--   0        0        0     3481 2023-03-14 19:25:36.822153 baseten-0.6.1/baseten/models/whisper.py
+-rw-r--r--   0        0        0      389 2023-04-26 05:33:19.915367 baseten-0.6.1/baseten/training/__init__.py
+-rw-r--r--   0        0        0     2852 2023-03-14 19:25:36.822255 baseten-0.6.1/baseten/training/datasets.py
+-rw-r--r--   0        0        0    33964 2023-04-26 05:33:19.915588 baseten-0.6.1/baseten/training/finetuning.py
+-rw-r--r--   0        0        0     6681 2023-03-14 19:25:36.822543 baseten-0.6.1/baseten/training/logs.py
+-rw-r--r--   0        0        0      479 2023-02-14 00:04:32.683738 baseten-0.6.1/baseten/training/utils.py
+-rw-r--r--   0        0        0      763 2023-03-14 19:25:36.842612 baseten-0.6.1/pypi_readme.md
+-rw-r--r--   0        0        0     2008 2023-04-26 05:35:14.728094 baseten-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 baseten-0.6.1/setup.py
+-rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 baseten-0.6.1/PKG-INFO
```

### Comparing `baseten-0.6.0/baseten/__init__.py` & `baseten-0.6.1/baseten/__init__.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/baseten_deployed_model.py` & `baseten-0.6.1/baseten/baseten_deployed_model.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/cli.py` & `baseten-0.6.1/baseten/cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/client_commands/baseten_cli.py` & `baseten-0.6.1/baseten/client_commands/baseten_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/client_commands/dataset_cli.py` & `baseten-0.6.1/baseten/client_commands/dataset_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/client_commands/finetuning_cli.py` & `baseten-0.6.1/baseten/client_commands/finetuning_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/client_commands/models_cli.py` & `baseten-0.6.1/baseten/client_commands/models_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/client_commands/pretrained_cli.py` & `baseten-0.6.1/baseten/client_commands/pretrained_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/common/api.py` & `baseten-0.6.1/baseten/common/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1106,13 +1106,14 @@
 @with_api_key_or_jwt
 def get_organization_credits(auth_token: AuthToken) -> List[dict]:
     query_string = """
     query {
         organization {
             monetary_credit_granted
             monetary_credit_balance
+            payment_method_status
         }
     }
     """
 
     resp = _post_graphql_query(auth_token, query_string)
     return resp["data"]["organization"]
```

### Comparing `baseten-0.6.0/baseten/common/core.py` & `baseten-0.6.1/baseten/common/core.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/common/error_handler.py` & `baseten-0.6.1/baseten/common/error_handler.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/common/files.py` & `baseten-0.6.1/baseten/common/files.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/common/lib_support.py` & `baseten-0.6.1/baseten/common/lib_support.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/common/model_deployer.py` & `baseten-0.6.1/baseten/common/model_deployer.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,24 +282,19 @@
 
     TrussLocalConfigHandler.add_signature(truss_hash, truss_signature)
 
     patch_request = truss_handle.calc_patch(truss_hash)
     if patch_request is None:
         return TryPatchDraftTrussResponse.needs_full_deploy_response("unable to calculate patch.")
 
-    if patch_request.prev_hash == patch_request.next_hash:
+    if patch_request.prev_hash == patch_request.next_hash or len(patch_request.patch_ops) == 0:
         return TryPatchDraftTrussResponse.success_response(
             dev_model_version_info, success_message="No changes observed skipping deploy"
         )
 
-    if len(patch_request.patch_ops) == 0:
-        # This shouldn't normally happen, hash check should catch this.
-        # Fallback to full deploy.
-        return TryPatchDraftTrussResponse.needs_full_deploy_response("no patchable changes found.")
-
     resp = api.patch_draft_truss(
         model_name=model_name,
         client_version=baseten.__version__,
         patch=patch_request,
     )
     if resp["succeeded"] is False:
         needs_full_deploy = True
@@ -393,40 +388,45 @@
 def _generate_organization_credit_logs():
     credits = api.get_organization_credits()
     credit_granted_cents = credits["monetary_credit_granted"]
     if credit_granted_cents == 0:
         # If the organization has never been granted monetary credits, omit any credit-related logging
         return
     credit_balance_cents = credits["monetary_credit_balance"]
+    needs_payment_method = credits["payment_method_status"] == "NEEDS_PAYMENT_METHOD"
     credit_balance_str = (
         "{:.2f}".format(round(credit_balance_cents / 100, 2))
         if credit_balance_cents != 0
         else str(credit_balance_cents)
     )
-    no_credit_remaining = credit_balance_cents <= 0 and credit_granted_cents != 0
+    no_credit_remaining = (
+        credit_balance_cents <= 0 and credit_granted_cents != 0 and needs_payment_method
+    )
     emoji_prefix = "💸"
     if credit_granted_cents == credit_balance_cents:
         emoji_prefix = "💰"
     elif no_credit_remaining:
         emoji_prefix = "🫙"
     suffix = (
         " Any previously-deployed model versions have been deactivated."
         if no_credit_remaining
         else ""
     )
-    logger.info(
-        f"{emoji_prefix} Your workspace has ${credit_balance_str} of model resource credit remaining.{suffix}"
-    )
-    billing_url = f"{settings.get_server_url()}/settings/billing"
-    add_payment_method_str = (
-        f"💳 Add a payment method to reactivate your models and deploy new versions: {billing_url}"
-        if no_credit_remaining
-        else f"💳 Add a payment method to keep your models running once credit runs out: {billing_url}"
-    )
-    logger.info(add_payment_method_str)
+    if needs_payment_method or credit_balance_cents > 0:
+        logger.info(
+            f"{emoji_prefix} Your workspace has ${credit_balance_str} of model resource credit remaining.{suffix}"
+        )
+    if needs_payment_method:
+        billing_url = f"{settings.get_server_url()}/settings/billing"
+        add_payment_method_str = (
+            f"💳 Add a payment method to reactivate your models and deploy new versions: {billing_url}"
+            if no_credit_remaining
+            else f"💳 Add a payment method to keep your models running once credit runs out: {billing_url}"
+        )
+        logger.info(add_payment_method_str)
 
 
 def _archive_truss(b10_truss: TrussHandle):
     try:
         truss_dir = b10_truss._spec.truss_dir
         temp_file = create_tar_with_progress_bar(truss_dir)
     except PermissionError:
```

### Comparing `baseten-0.6.0/baseten/common/settings.py` & `baseten-0.6.1/baseten/common/settings.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/common/tar.py` & `baseten-0.6.1/baseten/common/tar.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/common/types.py` & `baseten-0.6.1/baseten/common/types.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/common/util.py` & `baseten-0.6.1/baseten/common/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/models/flan_t5.py` & `baseten-0.6.1/baseten/models/flan_t5.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/models/llama.py` & `baseten-0.6.1/baseten/models/llama.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/models/stable_diffusion.py` & `baseten-0.6.1/baseten/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/models/util.py` & `baseten-0.6.1/baseten/models/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/models/whisper.py` & `baseten-0.6.1/baseten/models/whisper.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/training/datasets.py` & `baseten-0.6.1/baseten/training/datasets.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/training/finetuning.py` & `baseten-0.6.1/baseten/training/finetuning.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/baseten/training/logs.py` & `baseten-0.6.1/baseten/training/logs.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/pypi_readme.md` & `baseten-0.6.1/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `baseten-0.6.0/pyproject.toml` & `baseten-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baseten"
-version = "0.6.0"
+version = "0.6.1"
 description = "Deploy machine learning models to Baseten"
 readme = "pypi_readme.md"
 authors = [
     "Amir Haghighat <amir@baseten.co>",
     "Phil Howes <phil@baseten.co>",
     "Tuhin Srivastava <tuhin@baseten.co>",
 ]
```

### Comparing `baseten-0.6.0/PKG-INFO` & `baseten-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseten
-Version: 0.6.0
+Version: 0.6.1
 Summary: Deploy machine learning models to Baseten
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Amir Haghighat
 Author-email: amir@baseten.co
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

