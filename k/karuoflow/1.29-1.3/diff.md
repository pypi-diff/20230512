# Comparing `tmp/karuoflow-1.29.tar.gz` & `tmp/karuoflow-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karuoflow-1.29.tar", last modified: Sun Nov  6 14:37:54 2022, max compression
+gzip compressed data, was "karuoflow-1.3.tar", last modified: Fri May 12 05:52:56 2023, max compression
```

## Comparing `karuoflow-1.29.tar` & `karuoflow-1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-11-06 14:37:54.216325 karuoflow-1.29/
--rw-rw-r--   0 work      (1000) work      (1000)     1063 2021-12-01 06:30:43.000000 karuoflow-1.29/LICENSE
--rw-rw-r--   0 work      (1000) work      (1000)      277 2022-11-06 14:37:54.216325 karuoflow-1.29/PKG-INFO
--rw-rw-r--   0 work      (1000) work      (1000)       38 2021-12-01 06:30:43.000000 karuoflow-1.29/README.md
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-11-06 14:37:54.215325 karuoflow-1.29/karuoflow/
--rw-rw-r--   0 work      (1000) work      (1000)     2106 2022-11-06 14:36:38.000000 karuoflow-1.29/karuoflow/__init__.py
--rw-rw-r--   0 work      (1000) work      (1000)     2558 2021-12-01 06:30:43.000000 karuoflow-1.29/karuoflow/datadef.py
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-11-06 14:37:54.216325 karuoflow-1.29/karuoflow/db/
--rw-rw-r--   0 work      (1000) work      (1000)      151 2021-12-01 06:30:43.000000 karuoflow-1.29/karuoflow/db/__init__.py
--rw-rw-r--   0 work      (1000) work      (1000)      764 2021-12-01 06:30:43.000000 karuoflow-1.29/karuoflow/db/session.py
--rw-rw-r--   0 work      (1000) work      (1000)     7251 2021-12-01 06:30:43.000000 karuoflow-1.29/karuoflow/db/tables.py
--rw-rw-r--   0 work      (1000) work      (1000)     2510 2021-12-01 06:30:43.000000 karuoflow-1.29/karuoflow/error_code.py
--rw-rw-r--   0 work      (1000) work      (1000)    29629 2022-11-06 14:35:15.000000 karuoflow-1.29/karuoflow/flowapp.py
--rw-rw-r--   0 work      (1000) work      (1000)    19421 2022-11-06 01:54:57.000000 karuoflow-1.29/karuoflow/flowmodelagent.py
--rw-rw-r--   0 work      (1000) work      (1000)     6854 2022-11-06 01:38:36.000000 karuoflow-1.29/karuoflow/initflow.py
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-11-06 14:37:54.216325 karuoflow-1.29/karuoflow/test/
--rw-rw-r--   0 work      (1000) work      (1000)        0 2021-12-01 06:30:43.000000 karuoflow-1.29/karuoflow/test/__init__.py
--rw-rw-r--   0 work      (1000) work      (1000)    11334 2022-11-06 02:27:07.000000 karuoflow-1.29/karuoflow/test/test_initenvironment.py
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-11-06 14:37:54.215325 karuoflow-1.29/karuoflow.egg-info/
--rw-rw-r--   0 work      (1000) work      (1000)      277 2022-11-06 14:37:53.000000 karuoflow-1.29/karuoflow.egg-info/PKG-INFO
--rw-rw-r--   0 work      (1000) work      (1000)      466 2022-11-06 14:37:53.000000 karuoflow-1.29/karuoflow.egg-info/SOURCES.txt
--rw-rw-r--   0 work      (1000) work      (1000)        1 2022-11-06 14:37:53.000000 karuoflow-1.29/karuoflow.egg-info/dependency_links.txt
--rw-rw-r--   0 work      (1000) work      (1000)       26 2022-11-06 14:37:53.000000 karuoflow-1.29/karuoflow.egg-info/requires.txt
--rw-rw-r--   0 work      (1000) work      (1000)       10 2022-11-06 14:37:53.000000 karuoflow-1.29/karuoflow.egg-info/top_level.txt
--rw-rw-r--   0 work      (1000) work      (1000)       38 2022-11-06 14:37:54.216325 karuoflow-1.29/setup.cfg
--rw-rw-r--   0 work      (1000) work      (1000)      685 2021-12-01 06:30:43.000000 karuoflow-1.29/setup.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-05-12 05:52:56.280072 karuoflow-1.3/
+-rw-rw-r--   0 work      (1001) work      (1001)     1063 2023-05-12 05:20:22.000000 karuoflow-1.3/LICENSE
+-rw-rw-r--   0 work      (1001) work      (1001)      286 2023-05-12 05:52:56.280072 karuoflow-1.3/PKG-INFO
+-rw-rw-r--   0 work      (1001) work      (1001)       38 2023-05-12 05:20:22.000000 karuoflow-1.3/README.md
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-05-12 05:52:56.278072 karuoflow-1.3/karuoflow/
+-rw-rw-r--   0 work      (1001) work      (1001)     2169 2023-05-12 05:34:37.000000 karuoflow-1.3/karuoflow/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)     2558 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/datadef.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-05-12 05:52:56.279072 karuoflow-1.3/karuoflow/db/
+-rw-rw-r--   0 work      (1001) work      (1001)      151 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/db/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)      764 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/db/session.py
+-rw-rw-r--   0 work      (1001) work      (1001)     7251 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/db/tables.py
+-rw-rw-r--   0 work      (1001) work      (1001)     2510 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/error_code.py
+-rw-rw-r--   0 work      (1001) work      (1001)    30609 2023-05-12 05:33:33.000000 karuoflow-1.3/karuoflow/flowapp.py
+-rw-rw-r--   0 work      (1001) work      (1001)    19421 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/flowmodelagent.py
+-rw-rw-r--   0 work      (1001) work      (1001)     6854 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/initflow.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-05-12 05:52:56.280072 karuoflow-1.3/karuoflow/test/
+-rw-rw-r--   0 work      (1001) work      (1001)        0 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/test/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)    11800 2023-05-12 05:49:21.000000 karuoflow-1.3/karuoflow/test/test_initenvironment.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-05-12 05:52:56.279072 karuoflow-1.3/karuoflow.egg-info/
+-rw-rw-r--   0 work      (1001) work      (1001)      286 2023-05-12 05:52:55.000000 karuoflow-1.3/karuoflow.egg-info/PKG-INFO
+-rw-rw-r--   0 work      (1001) work      (1001)      466 2023-05-12 05:52:55.000000 karuoflow-1.3/karuoflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 work      (1001) work      (1001)        1 2023-05-12 05:52:55.000000 karuoflow-1.3/karuoflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 work      (1001) work      (1001)       26 2023-05-12 05:52:55.000000 karuoflow-1.3/karuoflow.egg-info/requires.txt
+-rw-rw-r--   0 work      (1001) work      (1001)       10 2023-05-12 05:52:55.000000 karuoflow-1.3/karuoflow.egg-info/top_level.txt
+-rw-rw-r--   0 work      (1001) work      (1001)       38 2023-05-12 05:52:56.280072 karuoflow-1.3/setup.cfg
+-rw-rw-r--   0 work      (1001) work      (1001)      685 2023-05-12 05:20:22.000000 karuoflow-1.3/setup.py
```

### Comparing `karuoflow-1.29/LICENSE` & `karuoflow-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `karuoflow-1.29/karuoflow/__init__.py` & `karuoflow-1.3/karuoflow/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,10 +27,11 @@
 @version 1.23 [2021-10-18] 增加 QueryJobViaRelationPrimaryKey 接口，已审核数据增加除重
 @version 1.24 [2021-12-01] 修复bug，获取待审核列表时，排序未生效
 @version 1.25 [2022-03-10] 增加AppendSign 接口，供批量追加审核节点，（多能上会申请定制化场景需求）
 @version 1.26 [2022-03-14] 修正了查询已审核申请列表数据问题，该问题由关联查询引起，但模糊匹配仍然存在问题
 @version 1.27 [2022-03-14] 修正了1.26版本中join查询的条件bug
 @version 1.28 [2022-11-06] 针对sqlalchemy的缓存问题，对db操作包裹db_session.begin()事务上下文
 @version 1.29 [2022-11-06] 针对sqlalchemy的缓存问题，对db操作包裹db_session.begin()事务上下文，该机制因为在外部系统中传入了session，并在传入前开启了事务，因此会报错，先退回。
+@version 1.30 [2023-05-12] 增加更新ext_data字段的函数
 '''
 
-__version__ = 1.29
+__version__ = 1.30
```

### Comparing `karuoflow-1.29/karuoflow/datadef.py` & `karuoflow-1.3/karuoflow/datadef.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.29/karuoflow/db/session.py` & `karuoflow-1.3/karuoflow/db/session.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.29/karuoflow/db/tables.py` & `karuoflow-1.3/karuoflow/db/tables.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.29/karuoflow/error_code.py` & `karuoflow-1.3/karuoflow/error_code.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.29/karuoflow/flowapp.py` & `karuoflow-1.3/karuoflow/flowapp.py`

 * *Files 5% similar despite different names*

```diff
@@ -688,8 +688,32 @@
                     _result.setErrorInfor(KaruoFlowErrors.ERR_DB_EXCEPTION, str(e))
                 finally:
                     self.db_session.close()
             else:
                 _result.setErrorInfor(KaruoFlowErrors.ERR_FLOW_STAGE_ERROR, KaruoFlowErrors.errorMsg(KaruoFlowErrors.ERR_FLOW_STAGE_ERROR))
         else: 
             _result.setErrorInfor(KaruoFlowErrors.ERR_DATA_NOT_FOUND, KaruoFlowErrors.errorMsg(KaruoFlowErrors.ERR_DATA_NOT_FOUND))
+        return _result
+
+    def UpdateJobExtdata(self, jobid: int, ext_data: dict) -> OperResult:
+        """
+        更新审核任务的扩展字段数据
+        :param jobid int 审批任务编号
+        :param ext_data dict 扩展字段数据
+        """
+        _result = OperResult()
+        apply_job = self.db_session.query(TblFlowJob).filter(TblFlowJob.id==jobid).first()
+        if apply_job:
+            try:
+                apply_job.ext_data = ext_data
+                flag_modified(apply_job, "ext_data")
+                self.db_session.commit()
+                _result.setSuccess()
+            except SQLAlchemyError as e:
+                    self.db_session.rollback()
+                    _result.setErrorInfor(KaruoFlowErrors.ERR_DB_EXCEPTION, str(e))
+            finally:
+                self.db_session.close()
+        else:
+            _result.setErrorInfor(KaruoFlowErrors.ERR_DATA_NOT_FOUND, KaruoFlowErrors.errorMsg(KaruoFlowErrors.ERR_DATA_NOT_FOUND))
+
         return _result
```

### Comparing `karuoflow-1.29/karuoflow/flowmodelagent.py` & `karuoflow-1.3/karuoflow/flowmodelagent.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.29/karuoflow/initflow.py` & `karuoflow-1.3/karuoflow/initflow.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.29/karuoflow/test/test_initenvironment.py` & `karuoflow-1.3/karuoflow/test/test_initenvironment.py`

 * *Files 3% similar despite different names*

```diff
@@ -264,9 +264,23 @@
         '''
         _append_node = [FlowCustomRuleNode("dn_hold_meeting", ["liudehua", "liangchaowei"], "上会申请", "law", "法律专责")]
         _append_node += [FlowCustomRuleNode("dn_hold_meeting", ["haha", "xixi", "hehe"], "上会申请", "dep_leader", "部门会签")]
         _append_node += [FlowCustomRuleNode("dn_hold_meeting", ["xujing", "wangtao"], "上会申请", "corp_leader", "领导会签")]
         result = self.flow_app.AppendSign(173, _append_node)
         pprint(result)
 
+    def testUpdateExtdata(self):
+        """
+        测试更新扩展数据字段
+        """
+        _jobid = 5521
+        _item = self.flow_app.QueryJob(_jobid)
+        if _item.isSuccess:
+            _ext_data = _item.data["job"]["ext_data"]
+            print(_ext_data)
+            if isinstance(_ext_data, dict):
+                _ext_data.update({"inuse": 1})
+            res = self.flow_app.UpdateJobExtdata(_jobid, _ext_data)
+            print(res.toDict)
+
 if "__main__" == __name__:
     unittest.main()
```

### Comparing `karuoflow-1.29/setup.py` & `karuoflow-1.3/setup.py`

 * *Files identical despite different names*

