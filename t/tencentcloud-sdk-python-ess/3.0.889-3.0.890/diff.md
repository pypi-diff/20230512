# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.890.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.889.tar", last modified: Thu May 11 02:49:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.890.tar", last modified: Fri May 12 02:10:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.889.tar` & `tencentcloud-sdk-python-ess-3.0.890.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    49606 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23727 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   220367 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:49:47.000000 tencentcloud-sdk-python-ess-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    50630 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23727 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   222168 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 02:10:45.000000 tencentcloud-sdk-python-ess-3.0.890/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.889/README.rst` & `tencentcloud-sdk-python-ess-3.0.890/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.890/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.889/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.890/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateChannelSubOrganizationModifyQrCode(self, request):
+        """生成子客编辑企业信息二维码
+
+        :param request: Request instance for CreateChannelSubOrganizationModifyQrCode.
+        :type request: :class:`tencentcloud.ess.v20201111.models.CreateChannelSubOrganizationModifyQrCodeRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.CreateChannelSubOrganizationModifyQrCodeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateChannelSubOrganizationModifyQrCode", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateChannelSubOrganizationModifyQrCodeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateConvertTaskApi(self, request):
         """上传了word、excel文件后，通过该接口发起文件转换任务，将word、excel文件转换为pdf文件。
 
         :param request: Request instance for CreateConvertTaskApi.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateConvertTaskApiRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateConvertTaskApiResponse`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.889/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.890/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.889/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.890/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -886,14 +886,69 @@
     def _deserialize(self, params):
         self.BatchCancelFlowUrl = params.get("BatchCancelFlowUrl")
         self.FailMessages = params.get("FailMessages")
         self.UrlExpireOn = params.get("UrlExpireOn")
         self.RequestId = params.get("RequestId")
 
 
+class CreateChannelSubOrganizationModifyQrCodeRequest(AbstractModel):
+    """CreateChannelSubOrganizationModifyQrCode请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Operator: 操作人
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param ApplicationId: 应用编号
+        :type ApplicationId: str
+        """
+        self.Operator = None
+        self.ApplicationId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self.Operator = UserInfo()
+            self.Operator._deserialize(params.get("Operator"))
+        self.ApplicationId = params.get("ApplicationId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateChannelSubOrganizationModifyQrCodeResponse(AbstractModel):
+    """CreateChannelSubOrganizationModifyQrCode返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param QrCodeUrl: 二维码下载链接
+        :type QrCodeUrl: str
+        :param ExpiredTime: 二维码失效时间 unix 时间戳 精确到秒
+        :type ExpiredTime: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.QrCodeUrl = None
+        self.ExpiredTime = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.QrCodeUrl = params.get("QrCodeUrl")
+        self.ExpiredTime = params.get("ExpiredTime")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateConvertTaskApiRequest(AbstractModel):
     """CreateConvertTaskApi请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-ess-3.0.889/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.890/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.890/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.889/setup.py` & `tencentcloud-sdk-python-ess-3.0.890/setup.py`

 * *Files identical despite different names*

