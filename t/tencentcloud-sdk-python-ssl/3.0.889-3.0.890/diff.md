# Comparing `tmp/tencentcloud-sdk-python-ssl-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-ssl-3.0.890.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.889.tar", last modified: Thu May 11 03:10:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.890.tar", last modified: Fri May 12 03:42:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssl-3.0.889.tar` & `tencentcloud-sdk-python-ssl-3.0.890.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 03:10:37.000000 tencentcloud-sdk-python-ssl-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:10:37.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/ssl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/ssl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/ssl/v20191205/
--rw-r--r--   0 root         (0) root         (0)     6906 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/ssl/v20191205/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/ssl/v20191205/__init__.py
--rw-r--r--   0 root         (0) root         (0)   132644 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/ssl/v20191205/models.py
--rw-r--r--   0 root         (0) root         (0)    28567 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/ssl/v20191205/ssl_client.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 03:10:37.000000 tencentcloud-sdk-python-ssl-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud_sdk_python_ssl.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:10:38.000000 tencentcloud-sdk-python-ssl-3.0.889/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/ssl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/ssl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/ssl/v20191205/
+-rw-r--r--   0 root         (0) root         (0)     6906 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/ssl/v20191205/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/ssl/v20191205/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   133829 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/ssl/v20191205/models.py
+-rw-r--r--   0 root         (0) root         (0)    28567 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/ssl/v20191205/ssl_client.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud_sdk_python_ssl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 03:42:38.000000 tencentcloud-sdk-python-ssl-3.0.890/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.889/README.rst` & `tencentcloud-sdk-python-ssl-3.0.890/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/ssl/v20191205/errorcodes.py` & `tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/ssl/v20191205/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/ssl/v20191205/models.py` & `tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/ssl/v20191205/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,32 +591,42 @@
         :type CompanyProvince: str
         :param CompanyCity: 公司所在城市
         :type CompanyCity: str
         :param CompanyAddress: 公司所在详细地址
         :type CompanyAddress: str
         :param CompanyPhone: 公司电话
         :type CompanyPhone: str
+        :param IdType: 类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IdType: str
+        :param IdNumber: ID号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IdNumber: str
         """
         self.CompanyName = None
         self.CompanyId = None
         self.CompanyCountry = None
         self.CompanyProvince = None
         self.CompanyCity = None
         self.CompanyAddress = None
         self.CompanyPhone = None
+        self.IdType = None
+        self.IdNumber = None
 
 
     def _deserialize(self, params):
         self.CompanyName = params.get("CompanyName")
         self.CompanyId = params.get("CompanyId")
         self.CompanyCountry = params.get("CompanyCountry")
         self.CompanyProvince = params.get("CompanyProvince")
         self.CompanyCity = params.get("CompanyCity")
         self.CompanyAddress = params.get("CompanyAddress")
         self.CompanyPhone = params.get("CompanyPhone")
+        self.IdType = params.get("IdType")
+        self.IdNumber = params.get("IdNumber")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1304,14 +1314,23 @@
         :type SubmittedData: :class:`tencentcloud.ssl.v20191205.models.SubmittedData`
         :param Deployable: 是否可部署。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Deployable: bool
         :param Tags: 标签列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tags: list of Tags
+        :param CAEncryptAlgorithms: CA证书的所有加密方式	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CAEncryptAlgorithms: list of str
+        :param CACommonNames: CA证书的所有通用名称	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CACommonNames: list of str
+        :param CAEndTimes: CA证书所有的到期时间	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CAEndTimes: list of str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.OwnerUin = None
         self.ProjectId = None
         self.From = None
         self.CertificateType = None
@@ -1339,14 +1358,17 @@
         self.IsWildcard = None
         self.IsDv = None
         self.IsVulnerability = None
         self.RenewAble = None
         self.SubmittedData = None
         self.Deployable = None
         self.Tags = None
+        self.CAEncryptAlgorithms = None
+        self.CACommonNames = None
+        self.CAEndTimes = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.OwnerUin = params.get("OwnerUin")
         self.ProjectId = params.get("ProjectId")
         self.From = params.get("From")
@@ -1386,14 +1408,17 @@
         self.Deployable = params.get("Deployable")
         if params.get("Tags") is not None:
             self.Tags = []
             for item in params.get("Tags"):
                 obj = Tags()
                 obj._deserialize(item)
                 self.Tags.append(obj)
+        self.CAEncryptAlgorithms = params.get("CAEncryptAlgorithms")
+        self.CACommonNames = params.get("CACommonNames")
+        self.CAEndTimes = params.get("CAEndTimes")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeCertificatesRequest(AbstractModel):
     """DescribeCertificates请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.889/tencentcloud/ssl/v20191205/ssl_client.py` & `tencentcloud-sdk-python-ssl-3.0.890/tencentcloud/ssl/v20191205/ssl_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.890/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.889/setup.py` & `tencentcloud-sdk-python-ssl-3.0.890/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.889/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.890/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

