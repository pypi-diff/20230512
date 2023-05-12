# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.890.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.889.tar", last modified: Thu May 11 03:08:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.890.tar", last modified: Fri May 12 03:17:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.889.tar` & `tencentcloud-sdk-python-redis-3.0.890.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    86880 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   295489 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    87124 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297155 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 03:17:18.000000 tencentcloud-sdk-python-redis-3.0.890/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.889/README.rst` & `tencentcloud-sdk-python-redis-3.0.890/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.890/tencentcloud/redis/v20180412/redis_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,15 +552,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDBSecurityGroups(self, request):
-        """本接口(DescribeDBSecurityGroups)用于查询实例的安全组详情。
+        """本接口（DescribeDBSecurityGroups）用于查询实例的安全组详情。
 
         :param request: Request instance for DescribeDBSecurityGroups.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeDBSecurityGroupsRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.DescribeDBSecurityGroupsResponse`
 
         """
         try:
@@ -575,15 +575,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeInstanceAccount(self, request):
-        """查看实例子账号信息
+        """本接口（DescribeInstanceAccount）用于查看实例子账号信息。
 
         :param request: Request instance for DescribeInstanceAccount.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceAccountRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceAccountResponse`
 
         """
         try:
@@ -897,15 +897,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeInstanceParams(self, request):
-        """查询实例参数列表
+        """本接口（DescribeInstanceParams）用于查询实例参数列表。
 
         :param request: Request instance for DescribeInstanceParams.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceParamsRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceParamsResponse`
 
         """
         try:
@@ -920,15 +920,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeInstanceSecurityGroup(self, request):
-        """查询实例安全组信息
+        """本接口（DescribeInstanceSecurityGroup）用于查询实例安全组信息。
 
         :param request: Request instance for DescribeInstanceSecurityGroup.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceSecurityGroupRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceSecurityGroupResponse`
 
         """
         try:
@@ -966,15 +966,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeInstanceZoneInfo(self, request):
-        """查询Redis节点详细信息
+        """本接口（DescribeInstanceZoneInfo）用于查询 Redis 节点详细信息。
 
         :param request: Request instance for DescribeInstanceZoneInfo.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceZoneInfoRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceZoneInfoResponse`
 
         """
         try:
@@ -1518,15 +1518,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ManualBackupInstance(self, request):
-        """手动备份Redis实例
+        """本接口（ManualBackupInstance）用于手动备份Redis实例。
 
         :param request: Request instance for ManualBackupInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.ManualBackupInstanceRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.ManualBackupInstanceResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.890/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.890/tencentcloud/redis/v20180412/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,30 +21,38 @@
 class Account(AbstractModel):
     """子账号信息
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID
+        :param InstanceId: 实例 ID。
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceId: str
-        :param AccountName: 账号名称（如果是主账号，名称为root）
+        :param AccountName: 账号名称。
 注意：此字段可能返回 null，表示取不到有效值。
         :type AccountName: str
-        :param Remark: 账号描述信息
+        :param Remark: 账号描述信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Remark: str
-        :param Privilege: 读写策略：r-只读，w-只写，rw-读写
+        :param Privilege: 读写权限策略。
+- r：只读。
+- w：只写。
+- rw：读写。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Privilege: str
-        :param ReadonlyPolicy: 路由策略：master-主节点，replication-从节点
+        :param ReadonlyPolicy: 只读路由策略。
+- master：主节点。
+- replication：从节点。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ReadonlyPolicy: list of str
-        :param Status: 子账号状态：1-账号变更中，2-账号有效，-4-账号已删除
+        :param Status: 子账号状态.
+- 1：账号变更中。
+- 2：账号有效。
+- 4：账号已删除。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Status: int
         """
         self.InstanceId = None
         self.AccountName = None
         self.Remark = None
         self.Privilege = None
@@ -1798,15 +1806,16 @@
 
     """
 
     def __init__(self):
         r"""
         :param Product: 数据库引擎名称，本接口取值：redis。
         :type Product: str
-        :param InstanceId: 实例ID，格式如：cdb-c1nl9rpv或者cdbro-c1nl9rpv，与云数据库控制台页面中显示的实例ID相同。
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
+
         :type InstanceId: str
         """
         self.Product = None
         self.InstanceId = None
 
 
     def _deserialize(self, params):
@@ -1826,17 +1835,17 @@
 
     """
 
     def __init__(self):
         r"""
         :param Groups: 安全组规则。
         :type Groups: list of SecurityGroup
-        :param VIP: 安全组生效内网地址。
+        :param VIP: 实例内网IPv4地址。
         :type VIP: str
-        :param VPort: 安全组生效内网端口。
+        :param VPort: 内网端口。
         :type VPort: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Groups = None
         self.VIP = None
         self.VPort = None
@@ -1858,19 +1867,19 @@
 class DescribeInstanceAccountRequest(AbstractModel):
     """DescribeInstanceAccount请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
         :type InstanceId: str
-        :param Limit: 分页大小
+        :param Limit: 分页大小。
         :type Limit: int
-        :param Offset: 分页偏移量
+        :param Offset: 分页偏移量。取Limit整数倍。计算公式：offset=limit*(页码-1)。
         :type Offset: int
         """
         self.InstanceId = None
         self.Limit = None
         self.Offset = None
 
 
@@ -1890,18 +1899,18 @@
 class DescribeInstanceAccountResponse(AbstractModel):
     """DescribeInstanceAccount返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Accounts: 账号详细信息
+        :param Accounts: 账号详细信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Accounts: list of Account
-        :param TotalCount: 账号个数
+        :param TotalCount: 账号个数。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TotalCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Accounts = None
         self.TotalCount = None
@@ -2790,15 +2799,15 @@
 class DescribeInstanceParamsRequest(AbstractModel):
     """DescribeInstanceParams请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例Id
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
         :type InstanceId: str
         """
         self.InstanceId = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
@@ -2814,23 +2823,23 @@
 class DescribeInstanceParamsResponse(AbstractModel):
     """DescribeInstanceParams返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TotalCount: 实例参数个数
+        :param TotalCount: 参数列表总数量。
         :type TotalCount: int
-        :param InstanceEnumParam: 实例枚举类型参数
+        :param InstanceEnumParam: 实例枚举类型参数。
         :type InstanceEnumParam: list of InstanceEnumParam
-        :param InstanceIntegerParam: 实例整型参数
+        :param InstanceIntegerParam: 实例整型参数。
         :type InstanceIntegerParam: list of InstanceIntegerParam
-        :param InstanceTextParam: 实例字符型参数
+        :param InstanceTextParam: 实例字符型参数。
         :type InstanceTextParam: list of InstanceTextParam
-        :param InstanceMultiParam: 实例多选项型参数
+        :param InstanceMultiParam: 实例多选项型参数。
         :type InstanceMultiParam: list of InstanceMultiParam
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TotalCount = None
         self.InstanceEnumParam = None
         self.InstanceIntegerParam = None
@@ -2871,15 +2880,15 @@
 class DescribeInstanceSecurityGroupRequest(AbstractModel):
     """DescribeInstanceSecurityGroup请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceIds: 实例列表
+        :param InstanceIds: 实例 ID 列表。例如;["crs-f2ho5rsz\n"]
         :type InstanceIds: list of str
         """
         self.InstanceIds = None
 
 
     def _deserialize(self, params):
         self.InstanceIds = params.get("InstanceIds")
@@ -2895,15 +2904,15 @@
 class DescribeInstanceSecurityGroupResponse(AbstractModel):
     """DescribeInstanceSecurityGroup返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceSecurityGroupsDetail: 实例安全组信息
+        :param InstanceSecurityGroupsDetail: 实例安全组信息。
         :type InstanceSecurityGroupsDetail: list of InstanceSecurityGroupDetail
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.InstanceSecurityGroupsDetail = None
         self.RequestId = None
 
@@ -2981,15 +2990,15 @@
 class DescribeInstanceZoneInfoRequest(AbstractModel):
     """DescribeInstanceZoneInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例Id，如：crs-6ubhgouj
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
         :type InstanceId: str
         """
         self.InstanceId = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
@@ -3005,17 +3014,17 @@
 class DescribeInstanceZoneInfoResponse(AbstractModel):
     """DescribeInstanceZoneInfo返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TotalCount: 实例节点组的个数
+        :param TotalCount: 实例节点组的个数。
         :type TotalCount: int
-        :param ReplicaGroups: 实例节点组列表
+        :param ReplicaGroups: 实例节点组列表。
         :type ReplicaGroups: list of ReplicaGroup
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TotalCount = None
         self.ReplicaGroups = None
         self.RequestId = None
@@ -3557,25 +3566,26 @@
 class DescribeProxySlowLogRequest(AbstractModel):
     """DescribeProxySlowLog请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例Id
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
+
         :type InstanceId: str
-        :param BeginTime: 开始时间
+        :param BeginTime: 慢查询的开始时间。
         :type BeginTime: str
-        :param EndTime: 结束时间
+        :param EndTime: 慢查询的结束时间。
         :type EndTime: str
-        :param MinQueryTime: 慢查询阈值（单位：毫秒）
+        :param MinQueryTime: 慢查询阈值，单位：毫秒。
         :type MinQueryTime: int
-        :param Limit: 页面大小
+        :param Limit: 分页大小。默认为 20，取值范围[20,1000]。
         :type Limit: int
-        :param Offset: 偏移量，取Limit整数倍
+        :param Offset: 偏移量，取Limit整数倍。
         :type Offset: int
         """
         self.InstanceId = None
         self.BeginTime = None
         self.EndTime = None
         self.MinQueryTime = None
         self.Limit = None
@@ -3601,17 +3611,17 @@
 class DescribeProxySlowLogResponse(AbstractModel):
     """DescribeProxySlowLog返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TotalCount: 慢查询总数
+        :param TotalCount: 慢查询总数。
         :type TotalCount: int
-        :param InstanceProxySlowLogDetail: 慢查询详情
+        :param InstanceProxySlowLogDetail: 慢查询详情。
         :type InstanceProxySlowLogDetail: list of InstanceProxySlowlogDetail
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TotalCount = None
         self.InstanceProxySlowLogDetail = None
         self.RequestId = None
@@ -3773,15 +3783,15 @@
         :type InstanceId: str
         :param BeginTime: 预查询慢日志的起始时间。
         :type BeginTime: str
         :param EndTime: 预查询慢日志的结束时间。
         :type EndTime: str
         :param MinQueryTime: 慢查询平均执行时间阈值，单位：毫秒。
         :type MinQueryTime: int
-        :param Limit: 每个页面展示的慢查询条数，默认值为20。
+        :param Limit: 每个页面展示的慢查询条数，默认值为20。取值范围：[20,1000]。
         :type Limit: int
         :param Offset: 慢查询条数的偏移量，取Limit整数倍。计算公式：offset=limit*(页码-1)。
         :type Offset: int
         :param Role: 节点所属角色。<ul><li>master：主节点。</li><li>slave：从节点。</li></ul>
         :type Role: str
         """
         self.InstanceId = None
@@ -4840,29 +4850,33 @@
 class InstanceEnumParam(AbstractModel):
     """实例枚举类型参数描述
 
     """
 
     def __init__(self):
         r"""
-        :param ParamName: 参数名
+        :param ParamName: 参数名称。
         :type ParamName: str
-        :param ValueType: 参数类型：enum
+        :param ValueType: 参数类型，例如：Enum。
         :type ValueType: str
-        :param NeedRestart: 修改后是否需要重启：true，false
+        :param NeedRestart: 参数值修改后是否需要重启。
+- true：需要。
+- false：不需要。
         :type NeedRestart: str
-        :param DefaultValue: 参数默认值
+        :param DefaultValue: 参数默认值。
         :type DefaultValue: str
-        :param CurrentValue: 当前运行参数值
+        :param CurrentValue: 参数当前运行值。
         :type CurrentValue: str
-        :param Tips: 参数说明
+        :param Tips: 参数说明。
         :type Tips: str
-        :param EnumValue: 参数可取值
+        :param EnumValue: 参数可取的值。
         :type EnumValue: list of str
-        :param Status: 参数状态, 1: 修改中， 2：修改完成
+        :param Status: 参数修改状态。
+- 1: 修改中。
+- 2：修改完成。
         :type Status: int
         """
         self.ParamName = None
         self.ValueType = None
         self.NeedRestart = None
         self.DefaultValue = None
         self.CurrentValue = None
@@ -4953,29 +4967,33 @@
 class InstanceMultiParam(AbstractModel):
     """实例多选项类型参数描述
 
     """
 
     def __init__(self):
         r"""
-        :param ParamName: 参数名
+        :param ParamName: 参数名称。
         :type ParamName: str
-        :param ValueType: 参数类型：multi
+        :param ValueType: 参数类型。例如：multi。
         :type ValueType: str
-        :param NeedRestart: 修改后是否需要重启：true，false
+        :param NeedRestart: 参数修改后是否需要重启。
+- true：需要。
+- false：不需要。
         :type NeedRestart: str
-        :param DefaultValue: 参数默认值
+        :param DefaultValue: 参数默认值。
         :type DefaultValue: str
-        :param CurrentValue: 当前运行参数值
+        :param CurrentValue: 当前运行参数值。
         :type CurrentValue: str
-        :param Tips: 参数说明
+        :param Tips: 参数说明。
         :type Tips: str
-        :param EnumValue: 参数说明
+        :param EnumValue: 参数说明。
         :type EnumValue: list of str
-        :param Status: 参数状态, 1: 修改中， 2：修改完成
+        :param Status: 参数修改的状态。
+- 1：修改中。
+- 2：修改完成。
         :type Status: int
         """
         self.ParamName = None
         self.ValueType = None
         self.NeedRestart = None
         self.DefaultValue = None
         self.CurrentValue = None
@@ -5149,17 +5167,17 @@
 class InstanceSecurityGroupDetail(AbstractModel):
     """实例安全组信息
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例Id
+        :param InstanceId: 实例 ID。
         :type InstanceId: str
-        :param SecurityGroupDetails: 安全组信息
+        :param SecurityGroupDetails: 安全组信息，包括：安全组 ID、安全组名称、安全组出入站规则。
         :type SecurityGroupDetails: list of SecurityGroupDetail
         """
         self.InstanceId = None
         self.SecurityGroupDetails = None
 
 
     def _deserialize(self, params):
@@ -5542,29 +5560,33 @@
 class InstanceTextParam(AbstractModel):
     """实例字符型参数描述
 
     """
 
     def __init__(self):
         r"""
-        :param ParamName: 参数名
+        :param ParamName: 参数名称。
         :type ParamName: str
-        :param ValueType: 参数类型：text
+        :param ValueType: 参数类型。例如：text。
         :type ValueType: str
-        :param NeedRestart: 修改后是否需要重启：true，false
+        :param NeedRestart: 参数修改后是否需要重启。
+- true：需要。
+- false：不需要。
         :type NeedRestart: str
-        :param DefaultValue: 参数默认值
+        :param DefaultValue: 参数默认值。
         :type DefaultValue: str
-        :param CurrentValue: 当前运行参数值
+        :param CurrentValue: 参数当前运行值。
         :type CurrentValue: str
-        :param Tips: 参数说明
+        :param Tips: 参数说明。
         :type Tips: str
-        :param TextValue: 参数可取值
+        :param TextValue: 参数可取值。
         :type TextValue: list of str
-        :param Status: 参数状态, 1: 修改中， 2：修改完成
+        :param Status: 参数修改状态。
+- 1: 修改中。
+- 2：修改完成。
         :type Status: int
         """
         self.ParamName = None
         self.ValueType = None
         self.NeedRestart = None
         self.DefaultValue = None
         self.CurrentValue = None
@@ -5762,19 +5784,22 @@
 class ManualBackupInstanceRequest(AbstractModel):
     """ManualBackupInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 待操作的实例ID，可通过 DescribeInstance接口返回值中的 InstanceId 获取。
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
         :type InstanceId: str
-        :param Remark: 备份的备注信息
+        :param Remark: 手动备份任务的备注信息。
         :type Remark: str
-        :param StorageDays: 保存天数。0代表指定默认保留时间
+        :param StorageDays: 备份数据的保存天数。
+- 单位：天；默认值为7天；取值范围：[0.1825]。如果超过 7天，请[提交工单](https://console.cloud.tencent.com/workorder/category)申请。
+- 如果不配置该参数，默认与自动备份的保留时间一致。
+- 如果未设置自动备份，默认为7天。
         :type StorageDays: int
         """
         self.InstanceId = None
         self.Remark = None
         self.StorageDays = None
 
 
@@ -7063,23 +7088,23 @@
 class RedisNode(AbstractModel):
     """Redis节点的运行信息
 
     """
 
     def __init__(self):
         r"""
-        :param Keys: 节点key的个数
+        :param Keys: Redis 节点上 Key 的个数。
         :type Keys: int
-        :param Slot: 节点slot分布
+        :param Slot: Redis 节点 Slot 分布范围。例如：0-5460。
         :type Slot: str
-        :param NodeId: 节点的序列ID
+        :param NodeId: 节点的序列 ID。
         :type NodeId: str
-        :param Status: 节点的状态
+        :param Status: 节点的状态。
         :type Status: str
-        :param Role: 节点角色
+        :param Role: 节点角色。
         :type Role: str
         """
         self.Keys = None
         self.Slot = None
         self.NodeId = None
         self.Status = None
         self.Role = None
@@ -7369,23 +7394,23 @@
 
     def _deserialize(self, params):
         self.DealId = params.get("DealId")
         self.RequestId = params.get("RequestId")
 
 
 class ReplicaGroup(AbstractModel):
-    """实例节点信息
+    """实例节点组信息
 
     """
 
     def __init__(self):
         r"""
-        :param GroupId: 节点组ID
+        :param GroupId: 节点组 ID。
         :type GroupId: int
-        :param GroupName: 节点组的名称，主节点为空
+        :param GroupName: 节点组的名称，主节点为空。
         :type GroupName: str
         :param ZoneId: 节点的可用区ID，比如ap-guangzhou-1
         :type ZoneId: str
         :param Role: 节点组类型，master为主节点，replica为副本节点
         :type Role: str
         :param RedisNodes: 节点组节点列表
         :type RedisNodes: list of RedisNode
@@ -7612,27 +7637,27 @@
 class SecurityGroupDetail(AbstractModel):
     """安全组详情
 
     """
 
     def __init__(self):
         r"""
-        :param ProjectId: 项目Id
+        :param ProjectId: 项目ID。
         :type ProjectId: int
-        :param CreateTime: 创建时间
+        :param CreateTime: 创建安全组的时间。
         :type CreateTime: str
-        :param SecurityGroupId: 安全组Id
+        :param SecurityGroupId: 安全组 ID。
         :type SecurityGroupId: str
-        :param SecurityGroupName: 安全组名称
+        :param SecurityGroupName: 安全组名称。
         :type SecurityGroupName: str
-        :param SecurityGroupRemark: 安全组标记
+        :param SecurityGroupRemark: 安全组标记。
         :type SecurityGroupRemark: str
-        :param InboundRule: 安全组入站规则
+        :param InboundRule: 安全组入站规则，即控制访问数据库的来源。
         :type InboundRule: list of SecurityGroupsInboundAndOutbound
-        :param OutboundRule: 安全组出站规则
+        :param OutboundRule: 安全组出站规则。
         :type OutboundRule: list of SecurityGroupsInboundAndOutbound
         """
         self.ProjectId = None
         self.CreateTime = None
         self.SecurityGroupId = None
         self.SecurityGroupName = None
         self.SecurityGroupRemark = None
@@ -7670,21 +7695,21 @@
 class SecurityGroupsInboundAndOutbound(AbstractModel):
     """安全组出入规则
 
     """
 
     def __init__(self):
         r"""
-        :param Action: 执行动作
+        :param Action: 标识出入数据库的IP与端口是否被允许。
         :type Action: str
-        :param Ip: IP地址
+        :param Ip: 出入数据库的IP地址
         :type Ip: str
-        :param Port: 端口号
+        :param Port: 端口号。
         :type Port: str
-        :param Proto: 协议类型
+        :param Proto: 协议类型。
         :type Proto: str
         """
         self.Action = None
         self.Ip = None
         self.Port = None
         self.Proto = None
```

### Comparing `tencentcloud-sdk-python-redis-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.890/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-redis-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.890/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.889/setup.py` & `tencentcloud-sdk-python-redis-3.0.890/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.889/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.890/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.889
+Version: 3.0.890
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

