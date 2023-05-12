# Comparing `tmp/tencentcloud-sdk-python-monitor-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-monitor-3.0.890.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.889.tar", last modified: Thu May 11 02:58:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.890.tar", last modified: Fri May 12 03:10:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-monitor-3.0.889.tar` & `tencentcloud-sdk-python-monitor-3.0.890.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/monitor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/monitor/v20180724/
--rw-r--r--   0 root         (0) root         (0)    10348 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/monitor/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   143620 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/monitor/v20180724/monitor_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/monitor/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)   552386 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/monitor/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud_sdk_python_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:58:26.000000 tencentcloud-sdk-python-monitor-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/monitor/v20180724/
+-rw-r--r--   0 root         (0) root         (0)    10348 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/monitor/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   144635 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/monitor/v20180724/monitor_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/monitor/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   552994 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/monitor/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud_sdk_python_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 03:10:05.000000 tencentcloud-sdk-python-monitor-3.0.890/setup.cfg
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.889/README.rst` & `tencentcloud-sdk-python-monitor-3.0.890/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/monitor/v20180724/errorcodes.py` & `tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/monitor/v20180724/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/monitor/v20180724/monitor_client.py` & `tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/monitor/v20180724/monitor_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1341,14 +1341,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeClusterAgentCreatingProgress(self, request):
+        """获取prom实例中集群详细的关联状态
+
+        :param request: Request instance for DescribeClusterAgentCreatingProgress.
+        :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeClusterAgentCreatingProgressRequest`
+        :rtype: :class:`tencentcloud.monitor.v20180724.models.DescribeClusterAgentCreatingProgressResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeClusterAgentCreatingProgress", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeClusterAgentCreatingProgressResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeConditionsTemplateList(self, request):
         """获取条件模板列表
 
         :param request: Request instance for DescribeConditionsTemplateList.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeConditionsTemplateListRequest`
         :rtype: :class:`tencentcloud.monitor.v20180724.models.DescribeConditionsTemplateListResponse`
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/monitor/v20180724/models.py` & `tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/monitor/v20180724/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5282,14 +5282,37 @@
         self.NoShieldedSum = params.get("NoShieldedSum")
         if params.get("InstanceGroup") is not None:
             self.InstanceGroup = DescribeBindingPolicyObjectListInstanceGroup()
             self.InstanceGroup._deserialize(params.get("InstanceGroup"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeClusterAgentCreatingProgressRequest(AbstractModel):
+    """DescribeClusterAgentCreatingProgress请求参数结构体
+
+    """
+
+
+class DescribeClusterAgentCreatingProgressResponse(AbstractModel):
+    """DescribeClusterAgentCreatingProgress返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeConditionsTemplateListRequest(AbstractModel):
     """DescribeConditionsTemplateList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-monitor-3.0.890/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-monitor-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.890/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.889/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.890/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.889/setup.py` & `tencentcloud-sdk-python-monitor-3.0.890/setup.py`

 * *Files identical despite different names*

