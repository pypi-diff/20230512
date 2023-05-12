# Comparing `tmp/pixelbin-2.1.0.tar.gz` & `tmp/pixelbin-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelbin-2.1.0.tar", max compression
+gzip compressed data, was "pixelbin-2.1.1.tar", max compression
```

## Comparing `pixelbin-2.1.0.tar` & `pixelbin-2.1.1.tar`

### file list

```diff
@@ -1,66 +1,65 @@
--rw-r--r--   0        0        0     1065 2022-05-27 05:55:59.335216 pixelbin-2.1.0/LICENSE
--rw-r--r--   0        0        0     5229 2022-11-08 19:12:32.304049 pixelbin-2.1.0/README.md
--rw-r--r--   0        0        0    72126 2023-02-03 06:42:04.214238 pixelbin-2.1.0/documentation/platform/ASSETS.md
--rw-r--r--   0        0        0     3589 2022-11-08 19:12:32.304660 pixelbin-2.1.0/documentation/platform/ORGANIZATION.md
--rw-r--r--   0        0        0      176 2022-05-27 05:55:59.310022 pixelbin-2.1.0/documentation/platform/README.md
--rw-r--r--   0        0        0      167 2022-05-27 05:55:59.312424 pixelbin-2.1.0/pixelbin/__init__.py
--rw-r--r--   0        0        0        0 2022-05-27 06:01:25.401889 pixelbin-2.1.0/pixelbin/common/__init__.py
--rw-r--r--   0        0        0     3289 2023-02-03 06:42:04.214984 pixelbin-2.1.0/pixelbin/common/aiohttp_helper.py
--rw-r--r--   0        0        0      165 2022-05-27 06:01:25.402704 pixelbin-2.1.0/pixelbin/common/constants.py
--rw-r--r--   0        0        0      276 2022-05-27 05:55:59.314728 pixelbin-2.1.0/pixelbin/common/date_helper.py
--rw-r--r--   0        0        0     1241 2022-11-08 19:12:32.304888 pixelbin-2.1.0/pixelbin/common/exceptions.py
--rw-r--r--   0        0        0     2733 2022-05-27 06:01:25.403240 pixelbin-2.1.0/pixelbin/common/utils.py
--rw-r--r--   0        0        0      272 2022-05-27 06:01:25.403508 pixelbin-2.1.0/pixelbin/platform/OAuthClient.py
--rw-r--r--   0        0        0    57491 2023-02-03 06:42:04.215714 pixelbin-2.1.0/pixelbin/platform/PixelbinClient.py
--rw-r--r--   0        0        0     1164 2022-05-27 06:01:25.404202 pixelbin-2.1.0/pixelbin/platform/PixelbinConfig.py
--rw-r--r--   0        0        0     2289 2022-05-27 06:01:25.404411 pixelbin-2.1.0/pixelbin/platform/PlatformAPIClient.py
--rw-r--r--   0        0        0        0 2022-05-27 05:55:59.316752 pixelbin-2.1.0/pixelbin/platform/__init__.py
--rw-r--r--   0        0        0      318 2022-05-27 05:55:59.316973 pixelbin-2.1.0/pixelbin/platform/enums.py
--rw-r--r--   0        0        0      345 2023-02-03 06:42:04.215978 pixelbin-2.1.0/pixelbin/platform/models/AddCredentialsRequest.py
--rw-r--r--   0        0        0      297 2023-02-03 06:42:04.216164 pixelbin-2.1.0/pixelbin/platform/models/AddCredentialsResponse.py
--rw-r--r--   0        0        0      392 2023-02-03 06:42:04.216350 pixelbin-2.1.0/pixelbin/platform/models/AddPresetRequest.py
--rw-r--r--   0        0        0      446 2023-02-03 06:42:04.216479 pixelbin-2.1.0/pixelbin/platform/models/AddPresetResponse.py
--rw-r--r--   0        0        0      466 2022-11-08 19:12:32.305375 pixelbin-2.1.0/pixelbin/platform/models/AppOrgDetails.py
--rw-r--r--   0        0        0      650 2022-05-27 05:55:59.317908 pixelbin-2.1.0/pixelbin/platform/models/AppSchema.py
--rw-r--r--   0        0        0     2938 2023-02-03 06:42:04.216843 pixelbin-2.1.0/pixelbin/platform/models/AssetsValidator.py
--rw-r--r--   0        0        0      240 2022-05-27 05:55:59.318322 pixelbin-2.1.0/pixelbin/platform/models/BaseSchema.py
--rw-r--r--   0        0        0      331 2022-05-27 05:55:59.318534 pixelbin-2.1.0/pixelbin/platform/models/CreateFolderRequest.py
--rw-r--r--   0        0        0      630 2023-02-03 06:42:04.217084 pixelbin-2.1.0/pixelbin/platform/models/Credentials.py
--rw-r--r--   0        0        0      286 2023-02-03 06:42:04.217347 pixelbin-2.1.0/pixelbin/platform/models/CredentialsItem.py
--rw-r--r--   0        0        0      592 2023-02-03 06:42:04.217573 pixelbin-2.1.0/pixelbin/platform/models/DeleteCredentialsResponse.py
--rw-r--r--   0        0        0      321 2022-05-27 05:55:59.318746 pixelbin-2.1.0/pixelbin/platform/models/DeleteMultipleFilesRequest.py
--rw-r--r--   0        0        0      349 2022-05-27 05:55:59.318959 pixelbin-2.1.0/pixelbin/platform/models/Delimiter.py
--rw-r--r--   0        0        0      287 2022-05-27 05:55:59.319154 pixelbin-2.1.0/pixelbin/platform/models/ErrorSchema.py
--rw-r--r--   0        0        0      732 2022-05-27 05:55:59.319473 pixelbin-2.1.0/pixelbin/platform/models/FileUploadRequest.py
--rw-r--r--   0        0        0      826 2022-05-27 05:55:59.319760 pixelbin-2.1.0/pixelbin/platform/models/FilesResponse.py
--rw-r--r--   0        0        0      424 2022-05-27 05:55:59.319957 pixelbin-2.1.0/pixelbin/platform/models/FoldersResponse.py
--rw-r--r--   0        0        0      481 2023-02-03 06:42:04.217778 pixelbin-2.1.0/pixelbin/platform/models/GetAncestorsResponse.py
--rw-r--r--   0        0        0      296 2023-02-03 06:42:04.217984 pixelbin-2.1.0/pixelbin/platform/models/GetCredentialsResponse.py
--rw-r--r--   0        0        0      384 2023-02-03 06:42:04.218175 pixelbin-2.1.0/pixelbin/platform/models/GetFilesWithConstraintsItem.py
--rw-r--r--   0        0        0      528 2023-02-03 06:42:04.218367 pixelbin-2.1.0/pixelbin/platform/models/GetFilesWithConstraintsRequest.py
--rw-r--r--   0        0        0      461 2023-02-03 06:42:04.218564 pixelbin-2.1.0/pixelbin/platform/models/GetPresetsResponse.py
--rw-r--r--   0        0        0      442 2022-05-27 05:55:59.320141 pixelbin-2.1.0/pixelbin/platform/models/ListFilesResponse.py
--rw-r--r--   0        0        0      590 2022-05-27 05:55:59.320346 pixelbin-2.1.0/pixelbin/platform/models/OrganizationDetailSchema.py
--rw-r--r--   0        0        0      270 2022-11-08 19:12:32.305605 pixelbin-2.1.0/pixelbin/platform/models/OrganizationValidator.py
--rw-r--r--   0        0        0      326 2022-05-27 05:55:59.320885 pixelbin-2.1.0/pixelbin/platform/models/PresignedUrl.py
--rw-r--r--   0        0        0      736 2022-05-27 05:55:59.321142 pixelbin-2.1.0/pixelbin/platform/models/SignedUploadRequest.py
--rw-r--r--   0        0        0      352 2022-05-27 05:55:59.321384 pixelbin-2.1.0/pixelbin/platform/models/SignedUploadResponse.py
--rw-r--r--   0        0        0      583 2022-05-27 05:55:59.321727 pixelbin-2.1.0/pixelbin/platform/models/TransformationModuleResponse.py
--rw-r--r--   0        0        0      474 2022-05-27 05:55:59.321995 pixelbin-2.1.0/pixelbin/platform/models/TransformationModulesResponse.py
--rw-r--r--   0        0        0      299 2023-02-03 06:42:04.218752 pixelbin-2.1.0/pixelbin/platform/models/UpdateCredentialsRequest.py
--rw-r--r--   0        0        0      553 2022-05-27 05:55:59.322258 pixelbin-2.1.0/pixelbin/platform/models/UpdateFileRequest.py
--rw-r--r--   0        0        0      294 2022-05-27 05:55:59.322486 pixelbin-2.1.0/pixelbin/platform/models/UpdateFolderRequest.py
--rw-r--r--   0        0        0      294 2023-02-03 06:42:04.219019 pixelbin-2.1.0/pixelbin/platform/models/UpdatePresetRequest.py
--rw-r--r--   0        0        0      774 2022-05-27 05:55:59.322832 pixelbin-2.1.0/pixelbin/platform/models/UploadResponse.py
--rw-r--r--   0        0        0      730 2022-05-27 05:55:59.323111 pixelbin-2.1.0/pixelbin/platform/models/UrlUploadRequest.py
--rw-r--r--   0        0        0     2248 2023-02-03 06:42:04.219260 pixelbin-2.1.0/pixelbin/platform/models/__init__.py
--rw-r--r--   0        0        0      542 2022-05-27 05:55:59.323718 pixelbin-2.1.0/pixelbin/platform/models/exploreFolderResponse.py
--rw-r--r--   0        0        0      598 2022-05-27 05:55:59.325079 pixelbin-2.1.0/pixelbin/platform/models/exploreItem.py
--rw-r--r--   0        0        0      440 2022-05-27 05:55:59.325358 pixelbin-2.1.0/pixelbin/platform/models/exploreResponse.py
--rw-r--r--   0        0        0      411 2022-05-27 05:55:59.325644 pixelbin-2.1.0/pixelbin/platform/models/folderItem.py
--rw-r--r--   0        0        0      466 2022-05-27 05:55:59.325929 pixelbin-2.1.0/pixelbin/platform/models/page.py
--rw-r--r--   0        0        0        0 2022-05-27 06:01:25.404488 pixelbin-2.1.0/pixelbin/utils/__init__.py
--rw-r--r--   0        0        0     8462 2022-11-08 19:12:32.306120 pixelbin-2.1.0/pixelbin/utils/url.py
--rw-r--r--   0        0        0      724 2023-02-03 06:42:04.219556 pixelbin-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     6217 2023-02-03 06:44:32.588080 pixelbin-2.1.0/setup.py
--rw-r--r--   0        0        0     6015 2023-02-03 06:44:32.588644 pixelbin-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-05-27 05:55:59.335216 pixelbin-2.1.1/LICENSE
+-rw-r--r--   0        0        0     5229 2022-11-08 19:12:32.304049 pixelbin-2.1.1/README.md
+-rw-r--r--   0        0        0    71822 2023-05-12 08:24:33.226873 pixelbin-2.1.1/documentation/platform/ASSETS.md
+-rw-r--r--   0        0        0     3589 2022-11-08 19:12:32.304660 pixelbin-2.1.1/documentation/platform/ORGANIZATION.md
+-rw-r--r--   0        0        0      176 2022-05-27 05:55:59.310022 pixelbin-2.1.1/documentation/platform/README.md
+-rw-r--r--   0        0        0      167 2022-05-27 05:55:59.312424 pixelbin-2.1.1/pixelbin/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-27 06:01:25.401889 pixelbin-2.1.1/pixelbin/common/__init__.py
+-rw-r--r--   0        0        0     3709 2023-05-12 08:24:33.227089 pixelbin-2.1.1/pixelbin/common/aiohttp_helper.py
+-rw-r--r--   0        0        0      165 2022-05-27 06:01:25.402704 pixelbin-2.1.1/pixelbin/common/constants.py
+-rw-r--r--   0        0        0      276 2022-05-27 05:55:59.314728 pixelbin-2.1.1/pixelbin/common/date_helper.py
+-rw-r--r--   0        0        0     1241 2022-11-08 19:12:32.304888 pixelbin-2.1.1/pixelbin/common/exceptions.py
+-rw-r--r--   0        0        0     2733 2022-05-27 06:01:25.403240 pixelbin-2.1.1/pixelbin/common/utils.py
+-rw-r--r--   0        0        0      272 2022-05-27 06:01:25.403508 pixelbin-2.1.1/pixelbin/platform/OAuthClient.py
+-rw-r--r--   0        0        0    57491 2023-02-03 06:42:04.215714 pixelbin-2.1.1/pixelbin/platform/PixelbinClient.py
+-rw-r--r--   0        0        0     1164 2022-05-27 06:01:25.404202 pixelbin-2.1.1/pixelbin/platform/PixelbinConfig.py
+-rw-r--r--   0        0        0     2289 2023-05-12 08:24:33.227557 pixelbin-2.1.1/pixelbin/platform/PlatformAPIClient.py
+-rw-r--r--   0        0        0        0 2022-05-27 05:55:59.316752 pixelbin-2.1.1/pixelbin/platform/__init__.py
+-rw-r--r--   0        0        0      318 2022-05-27 05:55:59.316973 pixelbin-2.1.1/pixelbin/platform/enums.py
+-rw-r--r--   0        0        0      345 2023-02-03 06:42:04.215978 pixelbin-2.1.1/pixelbin/platform/models/AddCredentialsRequest.py
+-rw-r--r--   0        0        0      297 2023-02-03 06:42:04.216164 pixelbin-2.1.1/pixelbin/platform/models/AddCredentialsResponse.py
+-rw-r--r--   0        0        0      392 2023-02-03 06:42:04.216350 pixelbin-2.1.1/pixelbin/platform/models/AddPresetRequest.py
+-rw-r--r--   0        0        0      446 2023-02-03 06:42:04.216479 pixelbin-2.1.1/pixelbin/platform/models/AddPresetResponse.py
+-rw-r--r--   0        0        0      466 2022-11-08 19:12:32.305375 pixelbin-2.1.1/pixelbin/platform/models/AppOrgDetails.py
+-rw-r--r--   0        0        0      650 2022-05-27 05:55:59.317908 pixelbin-2.1.1/pixelbin/platform/models/AppSchema.py
+-rw-r--r--   0        0        0     2938 2023-02-03 06:42:04.216843 pixelbin-2.1.1/pixelbin/platform/models/AssetsValidator.py
+-rw-r--r--   0        0        0      240 2022-05-27 05:55:59.318322 pixelbin-2.1.1/pixelbin/platform/models/BaseSchema.py
+-rw-r--r--   0        0        0      331 2022-05-27 05:55:59.318534 pixelbin-2.1.1/pixelbin/platform/models/CreateFolderRequest.py
+-rw-r--r--   0        0        0      630 2023-02-03 06:42:04.217084 pixelbin-2.1.1/pixelbin/platform/models/Credentials.py
+-rw-r--r--   0        0        0      286 2023-02-03 06:42:04.217347 pixelbin-2.1.1/pixelbin/platform/models/CredentialsItem.py
+-rw-r--r--   0        0        0      592 2023-02-03 06:42:04.217573 pixelbin-2.1.1/pixelbin/platform/models/DeleteCredentialsResponse.py
+-rw-r--r--   0        0        0      321 2022-05-27 05:55:59.318746 pixelbin-2.1.1/pixelbin/platform/models/DeleteMultipleFilesRequest.py
+-rw-r--r--   0        0        0      349 2022-05-27 05:55:59.318959 pixelbin-2.1.1/pixelbin/platform/models/Delimiter.py
+-rw-r--r--   0        0        0      287 2022-05-27 05:55:59.319154 pixelbin-2.1.1/pixelbin/platform/models/ErrorSchema.py
+-rw-r--r--   0        0        0      732 2022-05-27 05:55:59.319473 pixelbin-2.1.1/pixelbin/platform/models/FileUploadRequest.py
+-rw-r--r--   0        0        0      826 2022-05-27 05:55:59.319760 pixelbin-2.1.1/pixelbin/platform/models/FilesResponse.py
+-rw-r--r--   0        0        0      424 2022-05-27 05:55:59.319957 pixelbin-2.1.1/pixelbin/platform/models/FoldersResponse.py
+-rw-r--r--   0        0        0      481 2023-02-03 06:42:04.217778 pixelbin-2.1.1/pixelbin/platform/models/GetAncestorsResponse.py
+-rw-r--r--   0        0        0      384 2023-02-03 06:42:04.218175 pixelbin-2.1.1/pixelbin/platform/models/GetFilesWithConstraintsItem.py
+-rw-r--r--   0        0        0      528 2023-02-03 06:42:04.218367 pixelbin-2.1.1/pixelbin/platform/models/GetFilesWithConstraintsRequest.py
+-rw-r--r--   0        0        0      461 2023-02-03 06:42:04.218564 pixelbin-2.1.1/pixelbin/platform/models/GetPresetsResponse.py
+-rw-r--r--   0        0        0      442 2022-05-27 05:55:59.320141 pixelbin-2.1.1/pixelbin/platform/models/ListFilesResponse.py
+-rw-r--r--   0        0        0      590 2022-05-27 05:55:59.320346 pixelbin-2.1.1/pixelbin/platform/models/OrganizationDetailSchema.py
+-rw-r--r--   0        0        0      270 2022-11-08 19:12:32.305605 pixelbin-2.1.1/pixelbin/platform/models/OrganizationValidator.py
+-rw-r--r--   0        0        0      326 2022-05-27 05:55:59.320885 pixelbin-2.1.1/pixelbin/platform/models/PresignedUrl.py
+-rw-r--r--   0        0        0      736 2022-05-27 05:55:59.321142 pixelbin-2.1.1/pixelbin/platform/models/SignedUploadRequest.py
+-rw-r--r--   0        0        0      352 2022-05-27 05:55:59.321384 pixelbin-2.1.1/pixelbin/platform/models/SignedUploadResponse.py
+-rw-r--r--   0        0        0      583 2022-05-27 05:55:59.321727 pixelbin-2.1.1/pixelbin/platform/models/TransformationModuleResponse.py
+-rw-r--r--   0        0        0      474 2022-05-27 05:55:59.321995 pixelbin-2.1.1/pixelbin/platform/models/TransformationModulesResponse.py
+-rw-r--r--   0        0        0      299 2023-02-03 06:42:04.218752 pixelbin-2.1.1/pixelbin/platform/models/UpdateCredentialsRequest.py
+-rw-r--r--   0        0        0      553 2022-05-27 05:55:59.322258 pixelbin-2.1.1/pixelbin/platform/models/UpdateFileRequest.py
+-rw-r--r--   0        0        0      294 2022-05-27 05:55:59.322486 pixelbin-2.1.1/pixelbin/platform/models/UpdateFolderRequest.py
+-rw-r--r--   0        0        0      294 2023-02-03 06:42:04.219019 pixelbin-2.1.1/pixelbin/platform/models/UpdatePresetRequest.py
+-rw-r--r--   0        0        0      774 2022-05-27 05:55:59.322832 pixelbin-2.1.1/pixelbin/platform/models/UploadResponse.py
+-rw-r--r--   0        0        0      730 2022-05-27 05:55:59.323111 pixelbin-2.1.1/pixelbin/platform/models/UrlUploadRequest.py
+-rw-r--r--   0        0        0     2248 2023-02-03 06:42:04.219260 pixelbin-2.1.1/pixelbin/platform/models/__init__.py
+-rw-r--r--   0        0        0      542 2022-05-27 05:55:59.323718 pixelbin-2.1.1/pixelbin/platform/models/exploreFolderResponse.py
+-rw-r--r--   0        0        0      598 2022-05-27 05:55:59.325079 pixelbin-2.1.1/pixelbin/platform/models/exploreItem.py
+-rw-r--r--   0        0        0      440 2022-05-27 05:55:59.325358 pixelbin-2.1.1/pixelbin/platform/models/exploreResponse.py
+-rw-r--r--   0        0        0      411 2022-05-27 05:55:59.325644 pixelbin-2.1.1/pixelbin/platform/models/folderItem.py
+-rw-r--r--   0        0        0      466 2022-05-27 05:55:59.325929 pixelbin-2.1.1/pixelbin/platform/models/page.py
+-rw-r--r--   0        0        0        0 2022-05-27 06:01:25.404488 pixelbin-2.1.1/pixelbin/utils/__init__.py
+-rw-r--r--   0        0        0     8462 2022-11-08 19:12:32.306120 pixelbin-2.1.1/pixelbin/utils/url.py
+-rw-r--r--   0        0        0      762 2023-05-12 08:24:33.228223 pixelbin-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6269 2023-05-12 08:25:01.613765 pixelbin-2.1.1/setup.py
+-rw-r--r--   0        0        0     6095 2023-05-12 08:25:01.614354 pixelbin-2.1.1/PKG-INFO
```

### Comparing `pixelbin-2.1.0/LICENSE` & `pixelbin-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/README.md` & `pixelbin-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/documentation/platform/ASSETS.md` & `pixelbin-2.1.1/documentation/platform/ASSETS.md`

 * *Files 0% similar despite different names*

```diff
@@ -795,36 +795,28 @@
 | name     | str  | yes      | Name of the folder         |
 | path     | str  | no       | path of containing folder. |
 
 Create a new folder at the specified path. Also creates the ancestors if they do not exist.
 
 _Returned Response:_
 
-[List[FoldersResponse]](#foldersresponse)
+[FoldersResponse](#foldersresponse)
 
 Success - List of all created folders
 
 <details>
 <summary><i>&nbsp; Example:</i></summary>
 
 ```json
-[
-    {
-        "_id": "dummy-uuid",
-        "name": "subDir",
-        "path": "dir",
-        "isActive": true
-    },
-    {
-        "_id": "dummy-uuid-2",
-        "name": "subDir",
-        "path": "dir",
-        "isActive": true
-    }
-]
+{
+    "_id": "dummy-uuid",
+    "name": "subDir",
+    "path": "dir",
+    "isActive": true
+}
 ```
 
 </details>
 
 ### getFolderDetails
 
 **Summary**: Get folder details
@@ -999,36 +991,28 @@
 | -------- | ---- | -------- | ---------------------------- |
 | \_id     | str  | yes      | \_id of folder to be deleted |
 
 Delete folder and all its children permanently.
 
 _Returned Response:_
 
-[List[FoldersResponse]](#foldersresponse)
+[FoldersResponse](#foldersresponse)
 
 Success
 
 <details>
 <summary><i>&nbsp; Example:</i></summary>
 
 ```json
-[
-    {
-        "_id": "dummy-uuid",
-        "name": "subDir",
-        "path": "dir",
-        "isActive": true
-    },
-    {
-        "_id": "dummy-uuid-2",
-        "name": "subDir",
-        "path": "dir",
-        "isActive": true
-    }
-]
+{
+    "_id": "dummy-uuid",
+    "name": "subDir",
+    "path": "dir",
+    "isActive": true
+}
 ```
 
 </details>
 
 ### getFolderAncestors
 
 **Summary**: Get all ancestors of a folder
```

### Comparing `pixelbin-2.1.0/documentation/platform/ORGANIZATION.md` & `pixelbin-2.1.1/documentation/platform/ORGANIZATION.md`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/common/aiohttp_helper.py` & `pixelbin-2.1.1/pixelbin/common/aiohttp_helper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,90 @@
 """Python code/pixelbin/common/aiohttp_helper.py."""
 
 import time
 
 import aiohttp
 import ujson
+from typing import Union
 
 from .constants import HTTP_TIMEOUT
 from .date_helper import get_ist_now
 
 class AiohttpHelper:
     """Aiohttp Helper."""
 
     @staticmethod
+    def __get_formdata():
+        return aiohttp.formdata.FormData(quote_fields=False)
+
+    @staticmethod
     async def parse_data(data):
         """parse_data."""
         try:
             text = ujson.loads(data)
 
         except ValueError:
             text = {}
 
         return text
-
-    async def request(self, method:str, url:str, params:dict, data:dict, headers:dict, timeout_allowed:int=HTTP_TIMEOUT) -> dict:
-        """
-        summary - call api using aiohttp 
-        
-        :param - method : request method type : Type - str
-        :param - url : url to be hit : Type - str
-        :param - params : query params : Type - dict
-        :param - data : request body data : Type - dict
-        :param - headers : request headers : Type - dict
-        :param - timeout_allowed : timeout for request in seconds : Type - int    
-        """
+    
+    async def __make_request(self, method:str, url:str, params:dict, data:Union[str, aiohttp.formdata.FormData], headers:dict, timeout_allowed:int) -> dict:
         start_time = time.time()
         timeout = aiohttp.ClientTimeout(total=timeout_allowed)
-        async with aiohttp.ClientSession(headers=headers, timeout=timeout) as session:
-            response = {
+        response = {
                 "url": url,
                 "method": method,
                 "params": params,
                 "data": data,
                 "external_call_request_time": str(get_ist_now()),
                 "status_code": None,
                 "text": "",
                 "headers": "",
                 "cookies": None,
                 "error_message": "",
-            }
-            if data:
-                if "file" in data.keys():
-                    fdata = aiohttp.formdata.FormData()
-                    for k, v in data.items():
-                        if isinstance(v, list):
-                            for ele in v:
-                                fdata.add_field(k,ele)
-                        else:                                
-                            value = ujson.dumps(v, escape_forward_slashes=False) if isinstance(v, dict) or isinstance(v, bool) else v
-                            fdata.add_field(k,value)
-                    data = fdata
-                else:
-                    data = ujson.dumps(data, escape_forward_slashes=False)
-            async with session.request(method.upper(), url=url, params=params, data=data) as resp:        
+        }
+
+        async with aiohttp.ClientSession(headers=headers, timeout=timeout) as session:
+           async with session.request(method.upper(), url=url, params=params, data=data) as resp:        
                 response["status_code"] = resp.status
                 response["headers"] = dict(resp.headers)
                 response["cookies"] = dict(resp.cookies)
                 try:
                     response["content"] = await resp.content.read()  # resp.content is a StreamReader
                     response["text"] = response["content"].decode()  # converting to str
                 except UnicodeDecodeError as err:
                     response["error_message"] = f"Error occurred while converting bytes to string - {err}"
                     response["latency"] = time.time() - start_time
                     response["json"] = await self.parse_data(response["text"])
                 except Exception as request_error:
                     response["status_code"] = 999
                     response["latency"] = (time.time() - start_time)
                     response["text"] = request_error
-            return response
+        return response
+
+    async def request(self, method:str, url:str, params:dict, data:dict, headers:dict, timeout_allowed:int=HTTP_TIMEOUT) -> dict:
+        """
+        summary - call api using aiohttp 
+        
+        :param - method : request method type : Type - str
+        :param - url : url to be hit : Type - str
+        :param - params : query params : Type - dict
+        :param - data : request body data : Type - dict
+        :param - headers : request headers : Type - dict
+        :param - timeout_allowed : timeout for request in seconds : Type - int    
+        """
+        if data:
+            if "file" in data.keys():
+                form_data = self.__get_formdata()
+                for k, v in data.items():
+                    if isinstance(v, list):
+                        for ele in v:
+                            form_data.add_field(k,ele)
+                    else:                                
+                        value = ujson.dumps(v, escape_forward_slashes=False) if isinstance(v, dict) or isinstance(v, bool) else v
+                        form_data.add_field(k,value)
+                data = form_data
+            else:
+                data = ujson.dumps(data, escape_forward_slashes=False)
+            
+        response = await self.__make_request(method=method, url=url, params=params, data=data, headers=headers, timeout_allowed=timeout_allowed)
+        return response
```

### Comparing `pixelbin-2.1.0/pixelbin/common/exceptions.py` & `pixelbin-2.1.1/pixelbin/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/common/utils.py` & `pixelbin-2.1.1/pixelbin/common/utils.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/PixelbinClient.py` & `pixelbin-2.1.1/pixelbin/platform/PixelbinClient.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/PixelbinConfig.py` & `pixelbin-2.1.1/pixelbin/platform/PixelbinConfig.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/PlatformAPIClient.py` & `pixelbin-2.1.1/pixelbin/platform/PlatformAPIClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,24 +26,24 @@
         if contentType != "" and contentType != "multipart/form-data" and len(body)>0:
             headers["Content-Type"] = contentType
         data = body
         if contentType == "multipart/form-data":
             data = None
             
         if query and method.upper() == "GET":
-            get_parmas = {}
+            get_params = {}
             for k, v in query.items():
                 if isinstance(v, list):
                     for i in range(len(v)):
-                        get_parmas[f"{k}[{i}]"] = v[i]
+                        get_params[f"{k}[{i}]"] = v[i]
                 elif isinstance(v, bool):
-                    get_parmas[k] = ujson.dumps(v)
+                    get_params[k] = ujson.dumps(v)
                 else:
-                    get_parmas[k] = v
-            query = get_parmas
+                    get_params[k] = v
+            query = get_params
 
         query_string = await create_query_string(query)
 
         headers_with_sign = await add_signature_to_headers(
             domain=conf.domain,
             method=method,
             url=url,
```

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/AppSchema.py` & `pixelbin-2.1.1/pixelbin/platform/models/AppSchema.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/AssetsValidator.py` & `pixelbin-2.1.1/pixelbin/platform/models/AssetsValidator.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/Credentials.py` & `pixelbin-2.1.1/pixelbin/platform/models/Credentials.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/DeleteCredentialsResponse.py` & `pixelbin-2.1.1/pixelbin/platform/models/DeleteCredentialsResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/FileUploadRequest.py` & `pixelbin-2.1.1/pixelbin/platform/models/FileUploadRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/FilesResponse.py` & `pixelbin-2.1.1/pixelbin/platform/models/FilesResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/GetFilesWithConstraintsRequest.py` & `pixelbin-2.1.1/pixelbin/platform/models/GetFilesWithConstraintsRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/OrganizationDetailSchema.py` & `pixelbin-2.1.1/pixelbin/platform/models/OrganizationDetailSchema.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/SignedUploadRequest.py` & `pixelbin-2.1.1/pixelbin/platform/models/SignedUploadRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/TransformationModuleResponse.py` & `pixelbin-2.1.1/pixelbin/platform/models/TransformationModuleResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/UpdateFileRequest.py` & `pixelbin-2.1.1/pixelbin/platform/models/UpdateFileRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/UploadResponse.py` & `pixelbin-2.1.1/pixelbin/platform/models/UploadResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/UrlUploadRequest.py` & `pixelbin-2.1.1/pixelbin/platform/models/UrlUploadRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/__init__.py` & `pixelbin-2.1.1/pixelbin/platform/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/exploreFolderResponse.py` & `pixelbin-2.1.1/pixelbin/platform/models/exploreFolderResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/platform/models/exploreItem.py` & `pixelbin-2.1.1/pixelbin/platform/models/exploreItem.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pixelbin/utils/url.py` & `pixelbin-2.1.1/pixelbin/utils/url.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.0/pyproject.toml` & `pixelbin-2.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pixelbin"
-version = "2.1.0"
+version = "2.1.1"
 description = "Pixelbin SDK for Python"
 authors = ["Pixelbin <dev@pixelbin.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pixelbin-dev/pixelbin-python-sdk"
 repository = "https://github.com/pixelbin-dev/pixelbin-python-sdk"
 keywords = ["Pixelbin"]
@@ -14,13 +14,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.8.1"
 ujson = "^5.2.0"
 pytz = "^2022.1"
 marshmallow = "^3.15.0"
+pytest = "^7.2.2"
+coverage = "^7.2.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pixelbin-2.1.0/setup.py` & `pixelbin-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,23 @@
  'pixelbin.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.1,<4.0.0',
+ 'coverage>=7.2.1,<8.0.0',
  'marshmallow>=3.15.0,<4.0.0',
+ 'pytest>=7.2.2,<8.0.0',
  'pytz>=2022.1,<2023.0',
  'ujson>=5.2.0,<6.0.0']
 
 setup_kwargs = {
     'name': 'pixelbin',
-    'version': '2.1.0',
+    'version': '2.1.1',
     'description': 'Pixelbin SDK for Python',
     'long_description': '# Pixelbin Backend SDK for Python\n\nPixelbin Backend SDK for python helps you integrate the core Pixelbin features with your application.\n\n## Getting Started\n\nGetting started with Pixelbin Backend SDK for Python\n\n### Installation\n\n```\npip install pixelbin\n```\n\n---\n\n### Usage\n\n#### Quick Example\n\n```python\nimport asyncio\n\nfrom pixelbin import PixelbinClient, PixelbinConfig\n\n# create client with your API_TOKEN\nconfig = PixelbinConfig({\n    "domain": "https://api.pixelbin.io",\n    "apiSecret": "API_TOKEN",\n})\n\n# Create a pixelbin instance\npixelbin:PixelbinClient = PixelbinClient(config=config)\n\n# Sync method call\ntry:\n    result = pixelbin.assets.listFiles()\n    print(result)\nexcept Exception as e:\n    print(e)\n\n# Async method call\ntry:\n    result = asyncio.get_event_loop().run_until_complete(pixelbin.assets.listFilesAsync())\n    print(result)\nexcept Exception as e:\n    print(e)\n```\n\n## Utilities\n\nPixelbin provides url utilities to construct and deconstruct Pixelbin urls.\n\n### url_to_obj\n\nDeconstruct a pixelbin url\n\n| parameter            | description          | example                                                                                               |\n| -------------------- | -------------------- | ----------------------------------------------------------------------------------------------------- |\n| pixelbinUrl (string) | A valid pixelbin url | `https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg` |\n\n**Returns**:\n\n| property                | description                            | example                    |\n| ----------------------- | -------------------------------------- | -------------------------- |\n| cloudName (string)      | The cloudname extracted from the url   | `your-cloud-name`          |\n| zone (string)           | 6 character zone slug                  | `z-slug`                   |\n| version (string)        | cdn api version                        | `v2`                       |\n| options (object)        | optional query parameters              |                            |\n| transformations (array) | Extracted transformations from the url |                            |\n| filePath                | Path to the file on Pixelbin storage   | `/path/to/image.jpeg`      |\n| baseUrl (string)        | Base url                               | `https://cdn.pixelbin.io/` |\n\nExample:\n\n```python\nfrom pixelbin.utils.url import url_to_obj\n\npixelbinUrl = "https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg?dpr=2.0&f_auto=True"\nobj = url_to_obj(pixelbinUrl)\n# obj\n# {\n#     "cloudName": "your-cloud-name",\n#     "zone": "z-slug",\n#     "version": "v2",\n#     "options": {\n#         "dpr": 2.0,\n#         "f_auto": True,\n#     },\n#     "transformations": [\n#         {\n#             "plugin": "t",\n#             "name": "resize",\n#             "values": [\n#                 {\n#                     "key": "h",\n#                     "value": "100"\n#                 },\n#                 {\n#                     "key": "w",\n#                     "value": "200"\n#                 }\n#             ]\n#         },\n#         {\n#             "plugin": "t",\n#             "name": "flip",\n#         }\n#     ],\n#     "filePath": "path/to/image.jpeg",\n#     "baseUrl": "https://cdn.pixelbin.io"\n# }\n```\n\n### obj_to_url\n\nConverts the extracted url obj to a Pixelbin url.\n\n| property                | description                            | example                    |\n| ----------------------- | -------------------------------------- | -------------------------- |\n| cloudName (string)      | The cloudname extracted from the url   | `your-cloud-name`          |\n| zone (string)           | 6 character zone slug                  | `z-slug`                   |\n| version (string)        | cdn api version                        | `v2`                       |\n| options (object)        | optional query parameters              |                            |\n| transformations (array) | Extracted transformations from the url |                            |\n| filePath                | Path to the file on Pixelbin storage   | `/path/to/image.jpeg`      |\n| baseUrl (string)        | Base url                               | `https://cdn.pixelbin.io/` |\n\n```python\nfrom pixelbin.utils.url import obj_to_url\n\nobj = {\n    cloudName: "your-cloud-name",\n    zone: "z-slug",\n    version: "v2",\n    options: {\n        dpr: 2.0,\n        f_auto: True,\n    },\n    transformations: [\n        {\n            plugin: "t",\n            name: "resize",\n            values: [\n                {\n                    key: "h",\n                    value: "100",\n                },\n                {\n                    key: "w",\n                    value: "200",\n                },\n            ],\n        },\n        {\n            plugin: "t",\n            name: "flip",\n        },\n    ],\n    filePath: "path/to/image.jpeg",\n    baseUrl: "https://cdn.pixelbin.io",\n}\nurl = obj_to_url(obj) # obj is as shown above\n# url\n# https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg?dpr=2.0&f_auto=True\n```\n\n## Documentation\n\n-   [API docs](documentation/platform/README.md)\n',
     'author': 'Pixelbin',
     'author_email': 'dev@pixelbin.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/pixelbin-dev/pixelbin-python-sdk',
```

### Comparing `pixelbin-2.1.0/PKG-INFO` & `pixelbin-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pixelbin
-Version: 2.1.0
+Version: 2.1.1
 Summary: Pixelbin SDK for Python
 Home-page: https://github.com/pixelbin-dev/pixelbin-python-sdk
 License: MIT
 Keywords: Pixelbin
 Author: Pixelbin
 Author-email: dev@pixelbin.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: coverage (>=7.2.1,<8.0.0)
 Requires-Dist: marshmallow (>=3.15.0,<4.0.0)
+Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: pytz (>=2022.1,<2023.0)
 Requires-Dist: ujson (>=5.2.0,<6.0.0)
 Project-URL: Repository, https://github.com/pixelbin-dev/pixelbin-python-sdk
 Description-Content-Type: text/markdown
 
 # Pixelbin Backend SDK for Python
```

