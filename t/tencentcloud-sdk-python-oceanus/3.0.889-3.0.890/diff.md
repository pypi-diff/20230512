# Comparing `tmp/tencentcloud-sdk-python-oceanus-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-oceanus-3.0.890.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.889.tar", last modified: Thu May 11 03:07:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.890.tar", last modified: Fri May 12 03:11:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-oceanus-3.0.889.tar` & `tencentcloud-sdk-python-oceanus-3.0.890.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/oceanus/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/oceanus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/oceanus/v20190422/
--rw-r--r--   0 root         (0) root         (0)     9176 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/oceanus/v20190422/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/oceanus/v20190422/__init__.py
--rw-r--r--   0 root         (0) root         (0)   111986 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/oceanus/v20190422/models.py
--rw-r--r--   0 root         (0) root         (0)    23497 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/oceanus/v20190422/oceanus_client.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud_sdk_python_oceanus.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:07:25.000000 tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/oceanus/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/oceanus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/oceanus/v20190422/
+-rw-r--r--   0 root         (0) root         (0)     9176 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/oceanus/v20190422/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/oceanus/v20190422/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112543 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/oceanus/v20190422/models.py
+-rw-r--r--   0 root         (0) root         (0)    23497 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/oceanus/v20190422/oceanus_client.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud_sdk_python_oceanus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 03:11:20.000000 tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.889/README.rst` & `tencentcloud-sdk-python-oceanus-3.0.890/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/oceanus/v20190422/errorcodes.py` & `tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/oceanus/v20190422/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/oceanus/v20190422/models.py` & `tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/oceanus/v20190422/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,14 +206,17 @@
         :type RunningCu: float
         :param PayMode: 0 后付费,1 预付费
 注意：此字段可能返回 null，表示取不到有效值。
         :type PayMode: int
         :param IsNeedManageNode: 前端区分 集群是否需要2CU逻辑 因为历史集群 变配不需要, default 1  新集群都需要
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsNeedManageNode: int
+        :param ClusterSessions: session集群信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterSessions: list of ClusterSession
         """
         self.ClusterId = None
         self.Name = None
         self.Region = None
         self.AppId = None
         self.OwnerUin = None
         self.CreatorUin = None
@@ -242,14 +245,15 @@
         self.FreeCu = None
         self.DefaultLogCollectConf = None
         self.CustomizedDNSEnabled = None
         self.Correlations = None
         self.RunningCu = None
         self.PayMode = None
         self.IsNeedManageNode = None
+        self.ClusterSessions = None
 
 
     def _deserialize(self, params):
         self.ClusterId = params.get("ClusterId")
         self.Name = params.get("Name")
         self.Region = params.get("Region")
         self.AppId = params.get("AppId")
@@ -297,23 +301,35 @@
             for item in params.get("Correlations"):
                 obj = WorkSpaceClusterItem()
                 obj._deserialize(item)
                 self.Correlations.append(obj)
         self.RunningCu = params.get("RunningCu")
         self.PayMode = params.get("PayMode")
         self.IsNeedManageNode = params.get("IsNeedManageNode")
+        if params.get("ClusterSessions") is not None:
+            self.ClusterSessions = []
+            for item in params.get("ClusterSessions"):
+                obj = ClusterSession()
+                obj._deserialize(item)
+                self.ClusterSessions.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ClusterSession(AbstractModel):
+    """session集群信息
+
+    """
+
+
 class ClusterVersion(AbstractModel):
     """集群的版本相关信息
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud/oceanus/v20190422/oceanus_client.py` & `tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud/oceanus/v20190422/oceanus_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.890/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.889/setup.py` & `tencentcloud-sdk-python-oceanus-3.0.890/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.889/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.890/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

