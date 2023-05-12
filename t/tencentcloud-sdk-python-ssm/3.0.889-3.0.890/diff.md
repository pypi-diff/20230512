# Comparing `tmp/tencentcloud-sdk-python-ssm-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-ssm-3.0.890.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssm-3.0.889.tar", last modified: Thu May 11 03:10:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssm-3.0.890.tar", last modified: Fri May 12 03:42:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssm-3.0.889.tar` & `tencentcloud-sdk-python-ssm-3.0.890.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/ssm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/ssm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/ssm/v20190923/
--rw-r--r--   0 root         (0) root         (0)    24513 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/ssm/v20190923/ssm_client.py
--rw-r--r--   0 root         (0) root         (0)     3474 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/ssm/v20190923/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/ssm/v20190923/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63662 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/ssm/v20190923/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud_sdk_python_ssm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud_sdk_python_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud_sdk_python_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/tencentcloud_sdk_python_ssm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:10:52.000000 tencentcloud-sdk-python-ssm-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/ssm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/ssm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/ssm/v20190923/
+-rw-r--r--   0 root         (0) root         (0)    24513 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/ssm/v20190923/ssm_client.py
+-rw-r--r--   0 root         (0) root         (0)     3474 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/ssm/v20190923/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/ssm/v20190923/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64486 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/ssm/v20190923/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud_sdk_python_ssm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud_sdk_python_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud_sdk_python_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/tencentcloud_sdk_python_ssm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 03:42:55.000000 tencentcloud-sdk-python-ssm-3.0.890/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.889/README.rst` & `tencentcloud-sdk-python-ssm-3.0.890/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/ssm/v20190923/ssm_client.py` & `tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/ssm/v20190923/ssm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/ssm/v20190923/errorcodes.py` & `tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/ssm/v20190923/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/ssm/v20190923/models.py` & `tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/ssm/v20190923/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,43 +239,51 @@
 
     """
 
     def __init__(self):
         r"""
         :param SecretName: 凭据名称，同一region内不可重复，最长128字节，使用字母、数字或者 - _ 的组合，第一个字符必须为字母或者数字。一旦创建不可修改。
         :type SecretName: str
-        :param VersionId: 凭据版本，查询凭据信息时需要根据SecretName 和 VersionId进行查询，最长64 字节，使用字母、数字或者 - _ . 的组合并且以字母或数字开头。
+        :param VersionId: 凭据版本，查询凭据信息时需要根据SecretName 和 VersionId进行查询，最长64 字节，使用字母、数字或者 - _ . 的组合并且以字母或数字开头。若为空，则使用默认的初始凭据版本号。可选，若为空或该凭据为云产品类凭据，则该版本号默认为 SSM_Current。
         :type VersionId: str
         :param Description: 描述信息，用于详细描述用途等，最大支持2048字节。
         :type Description: str
         :param KmsKeyId: 指定对凭据进行加密的KMS CMK。如果为空则表示使用Secrets Manager为您默认创建的CMK进行加密。您也可以指定在同region 下自行创建的KMS CMK进行加密。
         :type KmsKeyId: str
+        :param SecretType: 凭据类型，默认为自定义凭据。
+        :type SecretType: int
         :param SecretBinary: 二进制凭据信息base64编码后的明文。SecretBinary 和 SecretString 必须且只能设置一个，最大支持4096字节。
         :type SecretBinary: str
         :param SecretString: 文本类型凭据信息明文（不需要进行base64编码）。SecretBinary 和 SecretString 必须且只能设置一个，，最大支持4096字节。
         :type SecretString: str
+        :param AdditionalConfig: JSON 格式字符串，用于指定特定凭据类型的额外配置。
+        :type AdditionalConfig: str
         :param Tags: 标签列表
         :type Tags: list of Tag
         """
         self.SecretName = None
         self.VersionId = None
         self.Description = None
         self.KmsKeyId = None
+        self.SecretType = None
         self.SecretBinary = None
         self.SecretString = None
+        self.AdditionalConfig = None
         self.Tags = None
 
 
     def _deserialize(self, params):
         self.SecretName = params.get("SecretName")
         self.VersionId = params.get("VersionId")
         self.Description = params.get("Description")
         self.KmsKeyId = params.get("KmsKeyId")
+        self.SecretType = params.get("SecretType")
         self.SecretBinary = params.get("SecretBinary")
         self.SecretString = params.get("SecretString")
+        self.AdditionalConfig = params.get("AdditionalConfig")
         if params.get("Tags") is not None:
             self.Tags = []
             for item in params.get("Tags"):
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
         memeber_set = set(params.keys())
@@ -661,14 +669,17 @@
         :type ProjectID: int
         :param AssociatedInstanceIDs: 当凭据类型为SSH密钥对凭据时，此字段有效，用于表示SSH密钥对所关联的CVM实例ID。
 注意：此字段可能返回 null，表示取不到有效值。
         :type AssociatedInstanceIDs: list of str
         :param TargetUin: 当凭据类型为云API密钥对凭据时，此字段有效，用于表示此云API密钥对所属的用户UIN。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TargetUin: int
+        :param AdditionalConfig: 凭据额外配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AdditionalConfig: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.SecretName = None
         self.Description = None
         self.KmsKeyId = None
         self.CreateUin = None
@@ -680,14 +691,15 @@
         self.ResourceID = None
         self.RotationStatus = None
         self.RotationFrequency = None
         self.ResourceName = None
         self.ProjectID = None
         self.AssociatedInstanceIDs = None
         self.TargetUin = None
+        self.AdditionalConfig = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.SecretName = params.get("SecretName")
         self.Description = params.get("Description")
         self.KmsKeyId = params.get("KmsKeyId")
@@ -700,14 +712,15 @@
         self.ResourceID = params.get("ResourceID")
         self.RotationStatus = params.get("RotationStatus")
         self.RotationFrequency = params.get("RotationFrequency")
         self.ResourceName = params.get("ResourceName")
         self.ProjectID = params.get("ProjectID")
         self.AssociatedInstanceIDs = params.get("AssociatedInstanceIDs")
         self.TargetUin = params.get("TargetUin")
+        self.AdditionalConfig = params.get("AdditionalConfig")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeSupportedProductsRequest(AbstractModel):
     """DescribeSupportedProducts请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssm-3.0.890/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.889'
+__version__ = '3.0.890'
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-ssm-3.0.890/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssm
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Ssm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.889/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssm-3.0.890/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssm
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Ssm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.889/setup.py` & `tencentcloud-sdk-python-ssm-3.0.890/setup.py`

 * *Files identical despite different names*

