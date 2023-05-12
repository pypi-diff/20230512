# Comparing `tmp/tencentcloud-sdk-python-omics-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-omics-3.0.890.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-omics-3.0.889.tar", last modified: Thu May 11 03:07:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-omics-3.0.890.tar", last modified: Fri May 12 03:11:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-omics-3.0.889.tar` & `tencentcloud-sdk-python-omics-3.0.890.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud_sdk_python_omics.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud_sdk_python_omics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud_sdk_python_omics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud_sdk_python_omics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud_sdk_python_omics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/
--rw-r--r--   0 root         (0) root         (0)     8751 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/omics_client.py
--rw-r--r--   0 root         (0) root         (0)     1373 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46322 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:11:42.000000 tencentcloud-sdk-python-omics-3.0.890/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-12 03:11:41.000000 tencentcloud-sdk-python-omics-3.0.890/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:11:42.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud_sdk_python_omics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 03:11:42.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud_sdk_python_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-12 03:11:42.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud_sdk_python_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-12 03:11:42.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud_sdk_python_omics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 03:11:42.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud_sdk_python_omics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:11:42.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:11:42.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud/omics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:11:42.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud/omics/v20221128/
+-rw-r--r--   0 root         (0) root         (0)    11298 2023-05-12 03:11:41.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud/omics/v20221128/omics_client.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-05-12 03:11:41.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud/omics/v20221128/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:11:41.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud/omics/v20221128/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55938 2023-05-12 03:11:41.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud/omics/v20221128/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:11:41.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud/omics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 03:11:41.000000 tencentcloud-sdk-python-omics-3.0.890/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-12 03:11:42.000000 tencentcloud-sdk-python-omics-3.0.890/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-12 03:11:41.000000 tencentcloud-sdk-python-omics-3.0.890/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 03:11:42.000000 tencentcloud-sdk-python-omics-3.0.890/setup.cfg
```

### Comparing `tencentcloud-sdk-python-omics-3.0.889/README.rst` & `tencentcloud-sdk-python-omics-3.0.890/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.889/tencentcloud_sdk_python_omics.egg-info/PKG-INFO` & `tencentcloud-sdk-python-omics-3.0.890/tencentcloud_sdk_python_omics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-omics
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Omics SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/omics_client.py` & `tencentcloud-sdk-python-omics-3.0.890/tencentcloud/omics/v20221128/omics_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -137,14 +137,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeTables(self, request):
+        """查询表格。
+
+        :param request: Request instance for DescribeTables.
+        :type request: :class:`tencentcloud.omics.v20221128.models.DescribeTablesRequest`
+        :rtype: :class:`tencentcloud.omics.v20221128.models.DescribeTablesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeTables", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeTablesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeTablesRows(self, request):
+        """查询表格行数据。
+
+        :param request: Request instance for DescribeTablesRows.
+        :type request: :class:`tencentcloud.omics.v20221128.models.DescribeTablesRowsRequest`
+        :rtype: :class:`tencentcloud.omics.v20221128.models.DescribeTablesRowsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeTablesRows", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeTablesRowsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def GetRunCalls(self, request):
         """查询作业详情。
 
         :param request: Request instance for GetRunCalls.
         :type request: :class:`tencentcloud.omics.v20221128.models.GetRunCallsRequest`
         :rtype: :class:`tencentcloud.omics.v20221128.models.GetRunCallsResponse`
 
@@ -204,14 +250,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def RetryRuns(self, request):
+        """重试任务。
+
+        :param request: Request instance for RetryRuns.
+        :type request: :class:`tencentcloud.omics.v20221128.models.RetryRunsRequest`
+        :rtype: :class:`tencentcloud.omics.v20221128.models.RetryRunsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RetryRuns", params, headers=headers)
+            response = json.loads(body)
+            model = models.RetryRunsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def RunApplication(self, request):
         """运行应用。
 
         :param request: Request instance for RunApplication.
         :type request: :class:`tencentcloud.omics.v20221128.models.RunApplicationRequest`
```

### Comparing `tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/errorcodes.py` & `tencentcloud-sdk-python-omics-3.0.890/tencentcloud/omics/v20221128/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/models.py` & `tencentcloud-sdk-python-omics-3.0.890/tencentcloud/omics/v20221128/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -418,14 +418,164 @@
             for item in params.get("Runs"):
                 obj = Run()
                 obj._deserialize(item)
                 self.Runs.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeTablesRequest(AbstractModel):
+    """DescribeTables请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProjectId: 项目ID。
+        :type ProjectId: str
+        :param Limit: 返回数量，默认为10，最大值为100。
+        :type Limit: int
+        :param Offset: 偏移量，默认为0。
+        :type Offset: int
+        :param Filters: 过滤器，支持过滤字段：
+- Name：表格名称
+- TableId：表格ID
+        :type Filters: list of Filter
+        """
+        self.ProjectId = None
+        self.Limit = None
+        self.Offset = None
+        self.Filters = None
+
+
+    def _deserialize(self, params):
+        self.ProjectId = params.get("ProjectId")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeTablesResponse(AbstractModel):
+    """DescribeTables返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 结果总数。
+        :type TotalCount: int
+        :param Tables: 表格列表。
+        :type Tables: list of Table
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.Tables = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("Tables") is not None:
+            self.Tables = []
+            for item in params.get("Tables"):
+                obj = Table()
+                obj._deserialize(item)
+                self.Tables.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeTablesRowsRequest(AbstractModel):
+    """DescribeTablesRows请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProjectId: 项目ID。
+        :type ProjectId: str
+        :param TableId: 表格ID。
+        :type TableId: str
+        :param Limit: 返回数量，默认为10，最大值为100。
+        :type Limit: int
+        :param Offset: 偏移量，默认为0。
+        :type Offset: int
+        :param Filters: 过滤器，支持过滤字段：
+- Tr：表格数据，支持模糊查询
+- TableRowUuid：表格行UUID
+        :type Filters: list of Filter
+        """
+        self.ProjectId = None
+        self.TableId = None
+        self.Limit = None
+        self.Offset = None
+        self.Filters = None
+
+
+    def _deserialize(self, params):
+        self.ProjectId = params.get("ProjectId")
+        self.TableId = params.get("TableId")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeTablesRowsResponse(AbstractModel):
+    """DescribeTablesRows返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 结果总数。
+        :type TotalCount: int
+        :param Rows: 表格行列表。
+        :type Rows: list of TableRow
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.Rows = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("Rows") is not None:
+            self.Rows = []
+            for item in params.get("Rows"):
+                obj = TableRow()
+                obj._deserialize(item)
+                self.Rows.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class Environment(AbstractModel):
     """组学平台环境详情。
 
     """
 
     def __init__(self):
         r"""
@@ -845,14 +995,59 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RetryRunsRequest(AbstractModel):
+    """RetryRuns请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProjectId: 关联项目ID。
+        :type ProjectId: str
+        :param RunUuids: 任务UUID。
+        :type RunUuids: list of str
+        """
+        self.ProjectId = None
+        self.RunUuids = None
+
+
+    def _deserialize(self, params):
+        self.ProjectId = params.get("ProjectId")
+        self.RunUuids = params.get("RunUuids")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RetryRunsResponse(AbstractModel):
+    """RetryRuns返回参数结构体
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
 class Run(AbstractModel):
     """任务。
 
     """
 
     def __init__(self):
         r"""
@@ -1353,14 +1548,134 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class Table(AbstractModel):
+    """表格。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TableId: 表格ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TableId: str
+        :param ProjectId: 关联项目ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProjectId: str
+        :param Name: 表格名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param Description: 表格描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param Columns: 表格列
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Columns: list of TableColumn
+        :param CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param Creator: 创建人
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Creator: str
+        """
+        self.TableId = None
+        self.ProjectId = None
+        self.Name = None
+        self.Description = None
+        self.Columns = None
+        self.CreateTime = None
+        self.Creator = None
+
+
+    def _deserialize(self, params):
+        self.TableId = params.get("TableId")
+        self.ProjectId = params.get("ProjectId")
+        self.Name = params.get("Name")
+        self.Description = params.get("Description")
+        if params.get("Columns") is not None:
+            self.Columns = []
+            for item in params.get("Columns"):
+                obj = TableColumn()
+                obj._deserialize(item)
+                self.Columns.append(obj)
+        self.CreateTime = params.get("CreateTime")
+        self.Creator = params.get("Creator")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TableColumn(AbstractModel):
+    """表格列。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Header: 列名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Header: str
+        :param DataType: 列数据类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DataType: str
+        """
+        self.Header = None
+        self.DataType = None
+
+
+    def _deserialize(self, params):
+        self.Header = params.get("Header")
+        self.DataType = params.get("DataType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TableRow(AbstractModel):
+    """表格行。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TableRowUuid: 表格行UUID。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TableRowUuid: str
+        :param Content: 表格行内容。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Content: list of str
+        """
+        self.TableRowUuid = None
+        self.Content = None
+
+
+    def _deserialize(self, params):
+        self.TableRowUuid = params.get("TableRowUuid")
+        self.Content = params.get("Content")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class VPCOption(AbstractModel):
     """私有网络配置。
 
     """
```

### Comparing `tencentcloud-sdk-python-omics-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-omics-3.0.890/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-omics-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-omics-3.0.890/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-omics
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Omics SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-omics-3.0.889/setup.py` & `tencentcloud-sdk-python-omics-3.0.890/setup.py`

 * *Files identical despite different names*

