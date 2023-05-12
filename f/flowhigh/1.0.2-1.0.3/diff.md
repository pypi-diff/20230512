# Comparing `tmp/flowhigh-1.0.2.tar.gz` & `tmp/flowhigh-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowhigh-1.0.2.tar", last modified: Wed Apr 26 10:35:19 2023, max compression
+gzip compressed data, was "flowhigh-1.0.3.tar", last modified: Fri May 12 13:34:51 2023, max compression
```

## Comparing `flowhigh-1.0.2.tar` & `flowhigh-1.0.3.tar`

### file list

```diff
@@ -1,105 +1,107 @@
--rw-r--r--   0        0        0       36 2023-04-26 09:11:00.000000 flowhigh-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-26 10:33:56.000000 flowhigh-1.0.2/flowhigh/__init__.py
--rw-r--r--   0        0        0       56 2023-04-26 09:11:00.000000 flowhigh-1.0.2/flowhigh/auth/__init__.py
--rw-r--r--   0        0        0     8326 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/auth/authentication.py
--rw-r--r--   0        0        0        0 2023-04-26 10:33:56.000000 flowhigh-1.0.2/flowhigh/extraction/__init__.py
--rw-r--r--   0        0        0     7073 2023-04-26 09:11:00.000000 flowhigh-1.0.2/flowhigh/extraction/extractor.py
--rw-r--r--   0        0        0       49 2023-04-26 09:11:00.000000 flowhigh-1.0.2/flowhigh/format/__init__.py
--rw-r--r--   0        0        0    10952 2023-04-26 09:11:00.000000 flowhigh-1.0.2/flowhigh/format/formatting.py
--rw-r--r--   0        0        0      930 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/AP_Types.py
--rw-r--r--   0        0        0     1254 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/Agg.py
--rw-r--r--   0        0        0       79 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/AggType.py
--rw-r--r--   0        0        0     8613 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/AntiPattern.py
--rw-r--r--   0        0        0      702 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/AntiPatterns.py
--rw-r--r--   0        0        0     1842 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/Asterisk.py
--rw-r--r--   0        0        0     2159 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/Attr.py
--rw-r--r--   0        0        0      314 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/BaseExpr.py
--rw-r--r--   0        0        0      298 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/BaseExprCollectionHolder.py
--rw-r--r--   0        0        0      276 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/BaseExprHolder.py
--rw-r--r--   0        0        0       77 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/BetweenType.py
--rw-r--r--   0        0        0     1525 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Case.py
--rw-r--r--   0        0        0     1173 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Cast.py
--rw-r--r--   0        0        0     1083 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/ColumnDef.py
--rw-r--r--   0        0        0      974 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/Const.py
--rw-r--r--   0        0        0      156 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/CoordinateBlock.py
--rw-r--r--   0        0        0     3437 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Copy.py
--rw-r--r--   0        0        0     2518 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/Create.py
--rw-r--r--   0        0        0     1808 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/CreateStage.py
--rw-r--r--   0        0        0     3289 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/CreateTableStatement.py
--rw-r--r--   0        0        0     1529 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/CreateView.py
--rw-r--r--   0        0        0      946 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Current.py
--rw-r--r--   0        0        0     1493 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/DBO.py
--rw-r--r--   0        0        0      634 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/DBOHier.py
--rw-r--r--   0        0        0       65 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/DBOSubType.py
--rw-r--r--   0        0        0      101 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/DBOType.py
--rw-r--r--   0        0        0       99 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/DefinedAsType.py
--rw-r--r--   0        0        0      984 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/Delete.py
--rw-r--r--   0        0        0     3269 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/DeleteStatement.py
--rw-r--r--   0        0        0       73 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/Direction.py
--rw-r--r--   0        0        0     4748 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/Ds.py
--rw-r--r--   0        0        0      445 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/DsAction.py
--rw-r--r--   0        0        0      130 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/DsSubType.py
--rw-r--r--   0        0        0      153 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/DsType.py
--rw-r--r--   0        0        0     1576 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/Edge.py
--rw-r--r--   0        0        0     1031 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/Else.py
--rw-r--r--   0        0        0      636 2023-04-26 10:34:10.000000 flowhigh-1.0.2/flowhigh/model/Error.py
--rw-r--r--   0        0        0      125 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/Expr.py
--rw-r--r--   0        0        0       94 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/ExprCollectionHolder.py
--rw-r--r--   0        0        0      378 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/ExprExprCollectionHolder.py
--rw-r--r--   0        0        0      319 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/ExprExprHolder.py
--rw-r--r--   0        0        0       84 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/ExprHolder.py
--rw-r--r--   0        0        0      915 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/Filter.py
--rw-r--r--   0        0        0       82 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/FilterType.py
--rw-r--r--   0        0        0     1848 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Frame.py
--rw-r--r--   0        0        0     2925 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Func.py
--rw-r--r--   0        0        0      405 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/FuncType.py
--rw-r--r--   0        0        0      750 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/In.py
--rw-r--r--   0        0        0     1065 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/InlineTable.py
--rw-r--r--   0        0        0     2056 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/Insert.py
--rw-r--r--   0        0        0     3269 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/InsertStatement.py
--rw-r--r--   0        0        0     1816 2023-04-26 10:34:10.000000 flowhigh-1.0.2/flowhigh/model/Join.py
--rw-r--r--   0        0        0       90 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/JoinSubType.py
--rw-r--r--   0        0        0      105 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/JoinType.py
--rw-r--r--   0        0        0     1857 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/MatchRecognize.py
--rw-r--r--   0        0        0      996 2023-04-26 10:34:12.000000 flowhigh-1.0.2/flowhigh/model/Merge.py
--rw-r--r--   0        0        0     3265 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/MergeStatement.py
--rw-r--r--   0        0        0     1061 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/MultiValue.py
--rw-r--r--   0        0        0       79 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/Named.py
--rw-r--r--   0        0        0     1278 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/Op.py
--rw-r--r--   0        0        0     1784 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/OpType.py
--rw-r--r--   0        0        0       81 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/Ordered.py
--rw-r--r--   0        0        0      935 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/Out.py
--rw-r--r--   0        0        0      984 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/Page.py
--rw-r--r--   0        0        0       87 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/PageType.py
--rw-r--r--   0        0        0     2067 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/ParSeQL.py
--rw-r--r--   0        0        0      104 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/ParSeQLStatus.py
--rw-r--r--   0        0        0     1253 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/Position.py
--rw-r--r--   0        0        0       78 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/Quantifier.py
--rw-r--r--   0        0        0     1220 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/QueryingStage.py
--rw-r--r--   0        0        0      125 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/ReferencableExpr.py
--rw-r--r--   0        0        0     2201 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Rotate.py
--rw-r--r--   0        0        0       84 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/Searchable.py
--rw-r--r--   0        0        0      758 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/Sort.py
--rw-r--r--   0        0        0     3355 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/Statement.py
--rw-r--r--   0        0        0     1887 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/StructRef.py
--rw-r--r--   0        0        0      241 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/SubString.py
--rw-r--r--   0        0        0     5522 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/TableFunc.py
--rw-r--r--   0        0        0     1633 2023-04-26 10:34:10.000000 flowhigh-1.0.2/flowhigh/model/TableSample.py
--rw-r--r--   0        0        0      992 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/Then.py
--rw-r--r--   0        0        0     1266 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/TreeNode.py
--rw-r--r--   0        0        0       82 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/TypeCast.py
--rw-r--r--   0        0        0      984 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/Update.py
--rw-r--r--   0        0        0     3269 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/UpdateStatement.py
--rw-r--r--   0        0        0     1274 2023-04-26 10:34:12.000000 flowhigh-1.0.2/flowhigh/model/When.py
--rw-r--r--   0        0        0      648 2023-04-26 10:34:10.000000 flowhigh-1.0.2/flowhigh/model/WrappedExpr.py
--rw-r--r--   0        0        0      107 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/WrappedExprs.py
--rw-r--r--   0        0        0     4040 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/__init__.py
--rw-r--r--   0        0        0       60 2023-04-26 09:11:00.000000 flowhigh-1.0.2/flowhigh/utils/__init__.py
--rw-r--r--   0        0        0    63547 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/utils/converter.py
--rw-r--r--   0        0        0     1254 2023-04-26 09:11:00.000000 flowhigh-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 10:33:56.000000 flowhigh-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 10:33:56.000000 flowhigh-1.0.2/tests/formatting-test/__init__.py
--rw-r--r--   0        0        0    82533 2023-04-26 09:11:00.000000 flowhigh-1.0.2/tests/formatting-test/format_test.py
--rw-r--r--   0        0        0    24130 2023-04-26 09:11:00.000000 flowhigh-1.0.2/tests/input.json
--rw-r--r--   0        0        0      879 2023-04-26 09:11:00.000000 flowhigh-1.0.2/tests/test.py
--rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 flowhigh-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       36 2023-04-18 12:50:40.081985 flowhigh-1.0.3/README.md
+-rw-r--r--   0        0        0       29 2023-05-04 15:09:52.704629 flowhigh-1.0.3/flowhigh/__init__.py
+-rw-r--r--   0        0        0       56 2023-04-18 12:50:40.081985 flowhigh-1.0.3/flowhigh/auth/__init__.py
+-rw-r--r--   0        0        0     8225 2023-05-12 13:33:02.000000 flowhigh-1.0.3/flowhigh/auth/authentication.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:34:02.813544 flowhigh-1.0.3/flowhigh/extraction/__init__.py
+-rw-r--r--   0        0        0     7073 2023-04-18 12:50:40.082985 flowhigh-1.0.3/flowhigh/extraction/extractor.py
+-rw-r--r--   0        0        0       49 2023-04-18 12:50:40.082985 flowhigh-1.0.3/flowhigh/format/__init__.py
+-rw-r--r--   0        0        0    10952 2023-04-18 12:50:40.082985 flowhigh-1.0.3/flowhigh/format/formatting.py
+-rw-r--r--   0        0        0      930 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/AP_Types.py
+-rw-r--r--   0        0        0     1254 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/Agg.py
+-rw-r--r--   0        0        0       76 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/AggType.py
+-rw-r--r--   0        0        0     8613 2023-05-12 13:32:54.000000 flowhigh-1.0.3/flowhigh/model/AntiPattern.py
+-rw-r--r--   0        0        0      702 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/AntiPatterns.py
+-rw-r--r--   0        0        0     1842 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/Asterisk.py
+-rw-r--r--   0        0        0     2159 2023-05-12 13:32:53.000000 flowhigh-1.0.3/flowhigh/model/Attr.py
+-rw-r--r--   0        0        0      314 2023-05-12 13:32:55.000000 flowhigh-1.0.3/flowhigh/model/BaseExpr.py
+-rw-r--r--   0        0        0      298 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/BaseExprCollectionHolder.py
+-rw-r--r--   0        0        0      276 2023-05-12 13:32:54.000000 flowhigh-1.0.3/flowhigh/model/BaseExprHolder.py
+-rw-r--r--   0        0        0       77 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/BetweenType.py
+-rw-r--r--   0        0        0     1525 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/Case.py
+-rw-r--r--   0        0        0     1173 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/Cast.py
+-rw-r--r--   0        0        0     1083 2023-05-12 13:32:55.000000 flowhigh-1.0.3/flowhigh/model/ColumnDef.py
+-rw-r--r--   0        0        0      974 2023-05-12 13:32:55.000000 flowhigh-1.0.3/flowhigh/model/Const.py
+-rw-r--r--   0        0        0      156 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/CoordinateBlock.py
+-rw-r--r--   0        0        0     3437 2023-05-12 13:32:55.000000 flowhigh-1.0.3/flowhigh/model/Copy.py
+-rw-r--r--   0        0        0     2518 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/Create.py
+-rw-r--r--   0        0        0     1808 2023-05-12 13:32:54.000000 flowhigh-1.0.3/flowhigh/model/CreateStage.py
+-rw-r--r--   0        0        0     3289 2023-05-12 13:32:55.000000 flowhigh-1.0.3/flowhigh/model/CreateTableStatement.py
+-rw-r--r--   0        0        0     1529 2023-05-12 13:32:53.000000 flowhigh-1.0.3/flowhigh/model/CreateView.py
+-rw-r--r--   0        0        0      946 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/Current.py
+-rw-r--r--   0        0        0     1493 2023-05-12 13:32:53.000000 flowhigh-1.0.3/flowhigh/model/DBO.py
+-rw-r--r--   0        0        0      634 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/DBOHier.py
+-rw-r--r--   0        0        0       65 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/DBOSubType.py
+-rw-r--r--   0        0        0      101 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/DBOType.py
+-rw-r--r--   0        0        0       99 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/DefinedAsType.py
+-rw-r--r--   0        0        0      984 2023-05-12 13:32:52.000000 flowhigh-1.0.3/flowhigh/model/Delete.py
+-rw-r--r--   0        0        0     3269 2023-05-12 13:32:53.000000 flowhigh-1.0.3/flowhigh/model/DeleteStatement.py
+-rw-r--r--   0        0        0       73 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/Direction.py
+-rw-r--r--   0        0        0     4113 2023-05-12 13:32:55.000000 flowhigh-1.0.3/flowhigh/model/Ds.py
+-rw-r--r--   0        0        0      445 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/DsAction.py
+-rw-r--r--   0        0        0      130 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/DsSubType.py
+-rw-r--r--   0        0        0      153 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/DsType.py
+-rw-r--r--   0        0        0     1576 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/Edge.py
+-rw-r--r--   0        0        0     1031 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/Else.py
+-rw-r--r--   0        0        0      636 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/Error.py
+-rw-r--r--   0        0        0      125 2023-05-12 13:32:55.000000 flowhigh-1.0.3/flowhigh/model/Expr.py
+-rw-r--r--   0        0        0       94 2023-05-12 13:32:54.000000 flowhigh-1.0.3/flowhigh/model/ExprCollectionHolder.py
+-rw-r--r--   0        0        0      378 2023-05-12 13:32:55.000000 flowhigh-1.0.3/flowhigh/model/ExprExprCollectionHolder.py
+-rw-r--r--   0        0        0      319 2023-05-12 13:32:54.000000 flowhigh-1.0.3/flowhigh/model/ExprExprHolder.py
+-rw-r--r--   0        0        0       84 2023-05-12 13:32:55.000000 flowhigh-1.0.3/flowhigh/model/ExprHolder.py
+-rw-r--r--   0        0        0      915 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/Filter.py
+-rw-r--r--   0        0        0       98 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/FilterType.py
+-rw-r--r--   0        0        0     1848 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/Frame.py
+-rw-r--r--   0        0        0     3129 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/Func.py
+-rw-r--r--   0        0        0      331 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/FuncSubType.py
+-rw-r--r--   0        0        0      120 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/FuncType.py
+-rw-r--r--   0        0        0      750 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/In.py
+-rw-r--r--   0        0        0     1065 2023-05-12 13:32:53.000000 flowhigh-1.0.3/flowhigh/model/InlineTable.py
+-rw-r--r--   0        0        0     2056 2023-05-12 13:32:53.000000 flowhigh-1.0.3/flowhigh/model/Insert.py
+-rw-r--r--   0        0        0     3269 2023-05-12 13:32:53.000000 flowhigh-1.0.3/flowhigh/model/InsertStatement.py
+-rw-r--r--   0        0        0     1816 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/Join.py
+-rw-r--r--   0        0        0       90 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/JoinSubType.py
+-rw-r--r--   0        0        0      105 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/JoinType.py
+-rw-r--r--   0        0        0     1857 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/MatchRecognize.py
+-rw-r--r--   0        0        0      996 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/Merge.py
+-rw-r--r--   0        0        0     3265 2023-05-12 13:32:54.000000 flowhigh-1.0.3/flowhigh/model/MergeStatement.py
+-rw-r--r--   0        0        0       82 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/Modifier.py
+-rw-r--r--   0        0        0     1061 2023-05-12 13:32:54.000000 flowhigh-1.0.3/flowhigh/model/MultiValue.py
+-rw-r--r--   0        0        0       79 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/Named.py
+-rw-r--r--   0        0        0     1278 2023-05-12 13:32:52.000000 flowhigh-1.0.3/flowhigh/model/Op.py
+-rw-r--r--   0        0        0     1806 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/OpType.py
+-rw-r--r--   0        0        0       81 2023-05-12 13:32:53.000000 flowhigh-1.0.3/flowhigh/model/Ordered.py
+-rw-r--r--   0        0        0      935 2023-05-12 13:32:55.000000 flowhigh-1.0.3/flowhigh/model/Out.py
+-rw-r--r--   0        0        0      984 2023-05-12 13:32:53.000000 flowhigh-1.0.3/flowhigh/model/Page.py
+-rw-r--r--   0        0        0       87 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/PageType.py
+-rw-r--r--   0        0        0     2067 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/ParSeQL.py
+-rw-r--r--   0        0        0      104 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/ParSeQLStatus.py
+-rw-r--r--   0        0        0     1253 2023-05-12 13:32:54.000000 flowhigh-1.0.3/flowhigh/model/Position.py
+-rw-r--r--   0        0        0       78 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/Quantifier.py
+-rw-r--r--   0        0        0     1220 2023-05-12 13:32:54.000000 flowhigh-1.0.3/flowhigh/model/QueryingStage.py
+-rw-r--r--   0        0        0      125 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/ReferencableExpr.py
+-rw-r--r--   0        0        0     2201 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/Rotate.py
+-rw-r--r--   0        0        0       84 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/Searchable.py
+-rw-r--r--   0        0        0      758 2023-05-12 13:32:54.000000 flowhigh-1.0.3/flowhigh/model/Sort.py
+-rw-r--r--   0        0        0     3355 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/Statement.py
+-rw-r--r--   0        0        0     1887 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/StructRef.py
+-rw-r--r--   0        0        0      241 2023-05-12 13:32:55.000000 flowhigh-1.0.3/flowhigh/model/SubString.py
+-rw-r--r--   0        0        0     5208 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/TableFunc.py
+-rw-r--r--   0        0        0     1633 2023-05-12 13:32:57.000000 flowhigh-1.0.3/flowhigh/model/TableSample.py
+-rw-r--r--   0        0        0      992 2023-05-12 13:32:54.000000 flowhigh-1.0.3/flowhigh/model/Then.py
+-rw-r--r--   0        0        0     1266 2023-05-12 13:33:00.000000 flowhigh-1.0.3/flowhigh/model/TreeNode.py
+-rw-r--r--   0        0        0       82 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/TypeCast.py
+-rw-r--r--   0        0        0      984 2023-05-12 13:32:53.000000 flowhigh-1.0.3/flowhigh/model/Update.py
+-rw-r--r--   0        0        0     3269 2023-05-12 13:32:54.000000 flowhigh-1.0.3/flowhigh/model/UpdateStatement.py
+-rw-r--r--   0        0        0     1274 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/When.py
+-rw-r--r--   0        0        0      648 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/WrappedExpr.py
+-rw-r--r--   0        0        0      107 2023-05-12 13:32:56.000000 flowhigh-1.0.3/flowhigh/model/WrappedExprs.py
+-rw-r--r--   0        0        0     4085 2023-05-12 13:32:58.000000 flowhigh-1.0.3/flowhigh/model/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-25 14:58:11.305696 flowhigh-1.0.3/flowhigh/utils/__init__.py
+-rw-r--r--   0        0        0    69353 2023-05-12 13:33:02.000000 flowhigh-1.0.3/flowhigh/utils/converter.py
+-rw-r--r--   0        0        0     1254 2023-05-04 22:24:07.664985 flowhigh-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-12 13:34:02.813544 flowhigh-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:34:02.813544 flowhigh-1.0.3/tests/formatting-test/__init__.py
+-rw-r--r--   0        0        0    82533 2023-04-18 12:50:40.083985 flowhigh-1.0.3/tests/formatting-test/format_test.py
+-rw-r--r--   0        0        0    24130 2023-05-04 15:09:52.746628 flowhigh-1.0.3/tests/input.json
+-rw-r--r--   0        0        0      879 2023-04-18 12:50:40.083985 flowhigh-1.0.3/tests/test.py
+-rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 flowhigh-1.0.3/PKG-INFO
```

### Comparing `flowhigh-1.0.2/flowhigh/auth/authentication.py` & `flowhigh-1.0.3/flowhigh/auth/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 
 import requests
 import time
 
 
 class Authentication:
     _base_url = "https://auth.sonra.io/oauth/"
-    _CLIENT_ID = "KpSwXfTVDUoArPizUDi3Wg6CfT5n6RNT"
+    _CLIENT_ID = "TA2gGqeNX59sJiIgvuTxsSu1o09OjEUM"
     _AUDIENCE = "https://flowhigh.sonra.io/api/"
     _SCOPE = "offline_access+openid"
-    _REALM = "FlowHigh-DEV-DB"
 
     # The secret location where the JSON containing the access token is stored.
     TOKEN_PATH = os.path.join(
         expanduser("~"),
         '.parseql',
         'parseql.json',
     )
@@ -65,16 +64,15 @@
 
         :param refresh_token: The refresh token obtained from the json in the secret location
         :return: Access token IF the user is authenticated ELSE `None`
         """
         url = cls._base_url + "token"
         payload = "grant_type=refresh_token" \
                   + "&client_id=" + cls._CLIENT_ID \
-                  + "&refresh_token=" + refresh_token \
-                  + "&realm=" + cls._REALM
+                  + "&refresh_token=" + refresh_token
         headers = {'content-type': "application/x-www-form-urlencoded"}
 
         response = requests.post(url, data=payload, headers=headers)
         if response.status_code == 200:
             json_data = json.loads(response.content)
             if "access_token" in json_data:
                 cls.save_token(json_data)
@@ -121,15 +119,15 @@
 
         :param device_code: The device code of the current user. Obtained from POST Request to OAuth
         :param polling_interval: The frequency at which POST request is to be sent to OAuth to receive token
         :return: Access token IF user is authenticated ELSE `None`
         """
         url = cls._base_url + "token"
         payload = "grant_type=urn:ietf:params:oauth:grant-type:device_code&device_code=" \
-                  + device_code + "&client_id=" + cls._CLIENT_ID + "&realm=" + cls._REALM
+                  + device_code + "&client_id=" + cls._CLIENT_ID
         headers = {'content-type': "application/x-www-form-urlencoded"}
 
         while True:
             # Keep polling until we receive a response which is handled above
             time.sleep(polling_interval)
             response = requests.post(url, data=payload, headers=headers)
             json_data = json.loads(response.content)
```

### Comparing `flowhigh-1.0.2/flowhigh/extraction/extractor.py` & `flowhigh-1.0.3/flowhigh/extraction/extractor.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/format/formatting.py` & `flowhigh-1.0.3/flowhigh/format/formatting.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/AP_Types.py` & `flowhigh-1.0.3/flowhigh/model/AP_Types.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Agg.py` & `flowhigh-1.0.3/flowhigh/model/Agg.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/AntiPattern.py` & `flowhigh-1.0.3/flowhigh/model/AntiPattern.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/AntiPatterns.py` & `flowhigh-1.0.3/flowhigh/model/AntiPatterns.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Asterisk.py` & `flowhigh-1.0.3/flowhigh/model/Asterisk.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Attr.py` & `flowhigh-1.0.3/flowhigh/model/Attr.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Case.py` & `flowhigh-1.0.3/flowhigh/model/Case.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Cast.py` & `flowhigh-1.0.3/flowhigh/model/Cast.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/ColumnDef.py` & `flowhigh-1.0.3/flowhigh/model/ColumnDef.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Const.py` & `flowhigh-1.0.3/flowhigh/model/Const.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Copy.py` & `flowhigh-1.0.3/flowhigh/model/Copy.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Create.py` & `flowhigh-1.0.3/flowhigh/model/Create.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/CreateStage.py` & `flowhigh-1.0.3/flowhigh/model/CreateStage.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/CreateTableStatement.py` & `flowhigh-1.0.3/flowhigh/model/CreateTableStatement.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/CreateView.py` & `flowhigh-1.0.3/flowhigh/model/CreateView.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Current.py` & `flowhigh-1.0.3/flowhigh/model/Current.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/DBO.py` & `flowhigh-1.0.3/flowhigh/model/DBO.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/DBOHier.py` & `flowhigh-1.0.3/flowhigh/model/DBOHier.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Delete.py` & `flowhigh-1.0.3/flowhigh/model/Delete.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/DeleteStatement.py` & `flowhigh-1.0.3/flowhigh/model/DeleteStatement.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Ds.py` & `flowhigh-1.0.3/flowhigh/model/TableFunc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,101 @@
 
+from flowhigh.model.Sort import Sort
+from flowhigh.model.Frame import Frame
+from flowhigh.model.Ds import Ds
 from flowhigh.model.DsType import DsType
 from flowhigh.model.DsSubType import DsSubType
 from flowhigh.model.DsAction import DsAction
 from flowhigh.model.Out import Out
 from flowhigh.model.In import In
-from flowhigh.model.Agg import Agg
-from flowhigh.model.Sort import Sort
-from flowhigh.model.Page import Page
 from flowhigh.model.MatchRecognize import MatchRecognize
 from flowhigh.model.TableSample import TableSample
 from flowhigh.model.Direction import Direction
-from flowhigh.model.BaseExpr import BaseExpr
-from flowhigh.model.ReferencableExpr import ReferencableExpr
-from flowhigh.model.Named import Named
-from flowhigh.model.Searchable import Searchable
-from flowhigh.model.TypeCast import TypeCast
+from flowhigh.model.Ordered import Ordered
 
 
-class Ds(BaseExpr, ReferencableExpr, Named, Searchable, TypeCast):
-    agg: Agg = None
-    refsch: str = None
-    fullref: str = None
-    refdb: str = None
-    in_: In = None
-    matchRecognize: MatchRecognize = None
-    setOp: list = []
+class TableFunc(Ds, Ordered):
+    names: list = []
+    partition: list = []
+    options: list = []
     sort: Sort = None
-    type_: DsType = None
-    out: Out = None
-    filter_: list = []
-    tableSample: TableSample = None
-    pos: str = None
-    refds: str = None
-    name: str = None
-    action: DsAction = None
-    alias: str = None
-    subType: DsSubType = None
-    refTo: str = None
-    page: Page = None
-    direction: Direction = None
+    tableFuncType: str = None
+    frame: Frame = None
+    subQuery: Ds = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class DsBuilder (object):
-    construction: Ds
+class TableFuncBuilder (object):
+    construction: TableFunc
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = Ds()
+        self.construction = TableFunc()
+    
+    def with_type(self, type_: DsType):
+        child = type_
+        self.construction.type_ = child
     
-    def with_agg(self, agg: Agg):
-        child = agg
-        if TreeNode in Agg.mro():
+    def with_modifiers(self, modifiers: list):
+        child = modifiers
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), modifiers)):
+            self.construction.add_child(node)
+        self.construction.modifiers = child
+    
+    def with_out(self, out: Out):
+        child = out
+        if TreeNode in Out.mro():
             self.construction.add_child(child)
-        self.construction.agg = child
+        self.construction.out = child
+    
+    def with_partition(self, partition: list):
+        child = partition
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), partition)):
+            self.construction.add_child(node)
+        self.construction.partition = child
+    
+    def with_pos(self, pos: str):
+        child = pos
+        self.construction.pos = child
+    
+    def with_refds(self, refds: str):
+        child = refds
+        self.construction.refds = child
+    
+    def with_options(self, options: list):
+        child = options
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), options)):
+            self.construction.add_child(node)
+        self.construction.options = child
+    
+    def with_action(self, action: DsAction):
+        child = action
+        self.construction.action = child
+    
+    def with_alias(self, alias: str):
+        child = alias
+        self.construction.alias = child
+    
+    def with_refTo(self, refTo: str):
+        child = refTo
+        self.construction.refTo = child
+    
+    def with_tableFuncType(self, tableFuncType: str):
+        child = tableFuncType
+        self.construction.tableFuncType = child
+    
+    def with_direction(self, direction: Direction):
+        child = direction
+        self.construction.direction = child
     
     def with_refsch(self, refsch: str):
         child = refsch
         self.construction.refsch = child
     
     def with_fullref(self, fullref: str):
         child = fullref
@@ -75,87 +107,63 @@
     
     def with_in(self, in_: In):
         child = in_
         if TreeNode in In.mro():
             self.construction.add_child(child)
         self.construction.in_ = child
     
-    def with_setOp(self, setOp: list):
-        child = setOp
-        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), setOp)):
-            self.construction.add_child(node)
-        self.construction.setOp = child
-    
     def with_matchRecognize(self, matchRecognize: MatchRecognize):
         child = matchRecognize
         if TreeNode in MatchRecognize.mro():
             self.construction.add_child(child)
         self.construction.matchRecognize = child
     
+    def with_setOp(self, setOp: list):
+        child = setOp
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), setOp)):
+            self.construction.add_child(node)
+        self.construction.setOp = child
+    
     def with_sort(self, sort: Sort):
         child = sort
         if TreeNode in Sort.mro():
             self.construction.add_child(child)
         self.construction.sort = child
     
-    def with_type(self, type_: DsType):
-        child = type_
-        self.construction.type_ = child
-    
-    def with_out(self, out: Out):
-        child = out
-        if TreeNode in Out.mro():
+    def with_subQuery(self, subQuery: Ds):
+        child = subQuery
+        if TreeNode in Ds.mro():
             self.construction.add_child(child)
-        self.construction.out = child
+        self.construction.subQuery = child
     
     def with_tableSample(self, tableSample: TableSample):
         child = tableSample
         if TreeNode in TableSample.mro():
             self.construction.add_child(child)
         self.construction.tableSample = child
     
-    def with_filter(self, filter_: list):
-        child = filter_
-        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), filter_)):
+    def with_names(self, names: list):
+        child = names
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), names)):
             self.construction.add_child(node)
-        self.construction.filter_ = child
-    
-    def with_pos(self, pos: str):
-        child = pos
-        self.construction.pos = child
-    
-    def with_refds(self, refds: str):
-        child = refds
-        self.construction.refds = child
+        self.construction.names = child
     
     def with_name(self, name: str):
         child = name
         self.construction.name = child
     
-    def with_action(self, action: DsAction):
-        child = action
-        self.construction.action = child
-    
-    def with_alias(self, alias: str):
-        child = alias
-        self.construction.alias = child
-    
     def with_subType(self, subType: DsSubType):
         child = subType
         self.construction.subType = child
     
-    def with_page(self, page: Page):
-        child = page
-        if TreeNode in Page.mro():
+    def with_dboref(self, dboref: str):
+        child = dboref
+        self.construction.dboref = child
+    
+    def with_frame(self, frame: Frame):
+        child = frame
+        if TreeNode in Frame.mro():
             self.construction.add_child(child)
-        self.construction.page = child
-    
-    def with_refTo(self, refTo: str):
-        child = refTo
-        self.construction.refTo = child
-    
-    def with_direction(self, direction: Direction):
-        child = direction
-        self.construction.direction = child
+        self.construction.frame = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.2/flowhigh/model/Edge.py` & `flowhigh-1.0.3/flowhigh/model/Edge.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Else.py` & `flowhigh-1.0.3/flowhigh/model/Else.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Error.py` & `flowhigh-1.0.3/flowhigh/model/Error.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Filter.py` & `flowhigh-1.0.3/flowhigh/model/Filter.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Frame.py` & `flowhigh-1.0.3/flowhigh/model/Frame.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Func.py` & `flowhigh-1.0.3/flowhigh/model/Func.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 from flowhigh.model.FuncType import FuncType
+from flowhigh.model.FuncSubType import FuncSubType
 from flowhigh.model.Quantifier import Quantifier
 from flowhigh.model.Sort import Sort
 from flowhigh.model.WrappedExpr import WrappedExpr
 from flowhigh.model.Frame import Frame
 from flowhigh.model.Direction import Direction
 from flowhigh.model.BaseExpr import BaseExpr
 from flowhigh.model.Named import Named
@@ -11,14 +12,15 @@
 
 
 class Func(BaseExpr, Named, TypeCast):
     partition: list = []
     name: str = None
     withinGroup: Sort = None
     exprs: list = []
+    subType: FuncSubType = None
     expr: WrappedExpr = None
     sort: Sort = None
     type_: FuncType = None
     quantifier: Quantifier = None
     frame: Frame = None
 
     def __init__(self):
@@ -68,14 +70,18 @@
     
     def with_expr(self, expr: WrappedExpr):
         child = expr
         if TreeNode in WrappedExpr.mro():
             self.construction.add_child(child)
         self.construction.expr = child
     
+    def with_subType(self, subType: FuncSubType):
+        child = subType
+        self.construction.subType = child
+    
     def with_sort(self, sort: Sort):
         child = sort
         if TreeNode in Sort.mro():
             self.construction.add_child(child)
         self.construction.sort = child
     
     def with_quantifier(self, quantifier: Quantifier):
```

### Comparing `flowhigh-1.0.2/flowhigh/model/In.py` & `flowhigh-1.0.3/flowhigh/model/In.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/InlineTable.py` & `flowhigh-1.0.3/flowhigh/model/InlineTable.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Insert.py` & `flowhigh-1.0.3/flowhigh/model/Insert.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/InsertStatement.py` & `flowhigh-1.0.3/flowhigh/model/InsertStatement.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Join.py` & `flowhigh-1.0.3/flowhigh/model/Join.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/MatchRecognize.py` & `flowhigh-1.0.3/flowhigh/model/MatchRecognize.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Merge.py` & `flowhigh-1.0.3/flowhigh/model/Merge.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/MergeStatement.py` & `flowhigh-1.0.3/flowhigh/model/MergeStatement.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/MultiValue.py` & `flowhigh-1.0.3/flowhigh/model/MultiValue.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Op.py` & `flowhigh-1.0.3/flowhigh/model/Op.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/OpType.py` & `flowhigh-1.0.3/flowhigh/model/OpType.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,62 +43,63 @@
     IS_NOT_TRUE = 39
     IS_NOT_FALSE = 40
     IS_NOT_UNKNOWN = 41
     PARENTHESIS = 42
     NOT_EXISTS = 43
     DIV = 44
     MULTI = 45
-    BETWEEN = 46
-    NEQJ = 47
-    EXISTS = 48
-    INTERSECT = 49
-    UNION = 50
-    EXCEPT = 51
-    SETMINUS = 52
-    UNION_ALL = 53
-    UNION_DISTINCT = 54
-    REGEXP = 55
-    ASSIGN = 56
-    MATCH = 57
-    NOT_MATCH = 58
-    COLLATE = 59
-    NOT_LIKE_ALL = 60
-    NOT_LIKE_ANY = 61
-    NOT_LIKE_SOME = 62
-    NOT_IN = 63
-    NOT_RLIKE_ALL = 64
-    NOT_RLIKE_ANY = 65
-    NOT_RLIKE_SOME = 66
-    NOT_REGEXP_ALL = 67
-    NOT_REGEXP_ANY = 68
-    NOT_REGEXP_SOME = 69
-    NOT_REGEXP = 70
-    NOT_RLIKE = 71
-    RLIKE_ANY = 72
-    RLIKE_ALL = 73
-    RLIKE_SOME = 74
-    REGEXP_ANY = 75
-    REGEXP_SOME = 76
-    REGEXP_ALL = 77
-    EQ_ALL = 78
-    EQ_ANY = 79
-    NEQ_ALL = 80
-    NEQ_ANY = 81
-    NEQJ_ALL = 82
-    NEQJ_ANY = 83
-    LT_ALL = 84
-    LT_ANY = 85
-    LTE_ALL = 86
-    LTE_ANY = 87
-    GT_ALL = 88
-    GT_ANY = 89
-    GTE_ALL = 90
-    GTE_ANY = 91
-    NSEQ_ANY = 92
-    NSEQ_ALL = 93
-    NSEQ = 94
-    CASE = 95
-    AMPERSAND = 96
-    SOME = 97
-    BOOL_TRUE = 98
-    BOOL_FALSE = 99
+    NOT_BETWEEN = 46
+    BETWEEN = 47
+    NEQJ = 48
+    EXISTS = 49
+    INTERSECT = 50
+    UNION = 51
+    EXCEPT = 52
+    SETMINUS = 53
+    UNION_ALL = 54
+    UNION_DISTINCT = 55
+    REGEXP = 56
+    ASSIGN = 57
+    MATCH = 58
+    NOT_MATCH = 59
+    COLLATE = 60
+    NOT_LIKE_ALL = 61
+    NOT_LIKE_ANY = 62
+    NOT_LIKE_SOME = 63
+    NOT_IN = 64
+    NOT_RLIKE_ALL = 65
+    NOT_RLIKE_ANY = 66
+    NOT_RLIKE_SOME = 67
+    NOT_REGEXP_ALL = 68
+    NOT_REGEXP_ANY = 69
+    NOT_REGEXP_SOME = 70
+    NOT_REGEXP = 71
+    NOT_RLIKE = 72
+    RLIKE_ANY = 73
+    RLIKE_ALL = 74
+    RLIKE_SOME = 75
+    REGEXP_ANY = 76
+    REGEXP_SOME = 77
+    REGEXP_ALL = 78
+    EQ_ALL = 79
+    EQ_ANY = 80
+    NEQ_ALL = 81
+    NEQ_ANY = 82
+    NEQJ_ALL = 83
+    NEQJ_ANY = 84
+    LT_ALL = 85
+    LT_ANY = 86
+    LTE_ALL = 87
+    LTE_ANY = 88
+    GT_ALL = 89
+    GT_ANY = 90
+    GTE_ALL = 91
+    GTE_ANY = 92
+    NSEQ_ANY = 93
+    NSEQ_ALL = 94
+    NSEQ = 95
+    CASE = 96
+    AMPERSAND = 97
+    SOME = 98
+    BOOL_TRUE = 99
+    BOOL_FALSE = 100
```

### Comparing `flowhigh-1.0.2/flowhigh/model/Out.py` & `flowhigh-1.0.3/flowhigh/model/Out.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Page.py` & `flowhigh-1.0.3/flowhigh/model/Page.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/ParSeQL.py` & `flowhigh-1.0.3/flowhigh/model/ParSeQL.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Position.py` & `flowhigh-1.0.3/flowhigh/model/Position.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/QueryingStage.py` & `flowhigh-1.0.3/flowhigh/model/QueryingStage.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Rotate.py` & `flowhigh-1.0.3/flowhigh/model/Rotate.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Sort.py` & `flowhigh-1.0.3/flowhigh/model/Sort.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Statement.py` & `flowhigh-1.0.3/flowhigh/model/Statement.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/StructRef.py` & `flowhigh-1.0.3/flowhigh/model/StructRef.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/TableSample.py` & `flowhigh-1.0.3/flowhigh/model/TableSample.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Then.py` & `flowhigh-1.0.3/flowhigh/model/Then.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/TreeNode.py` & `flowhigh-1.0.3/flowhigh/model/TreeNode.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/Update.py` & `flowhigh-1.0.3/flowhigh/model/Update.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/UpdateStatement.py` & `flowhigh-1.0.3/flowhigh/model/UpdateStatement.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/When.py` & `flowhigh-1.0.3/flowhigh/model/When.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/WrappedExpr.py` & `flowhigh-1.0.3/flowhigh/model/WrappedExpr.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/flowhigh/model/__init__.py` & `flowhigh-1.0.3/flowhigh/model/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 
 from flowhigh.model.Delete import Delete, DeleteBuilder
 from flowhigh.model.Op import Op, OpBuilder
 from flowhigh.model.InlineTable import InlineTable, InlineTableBuilder
 from flowhigh.model.Ordered import Ordered
 from flowhigh.model.Page import Page, PageBuilder
-from flowhigh.model.Insert import Insert, InsertBuilder
 from flowhigh.model.Update import Update, UpdateBuilder
+from flowhigh.model.Insert import Insert, InsertBuilder
 from flowhigh.model.DeleteStatement import DeleteStatement, DeleteStatementBuilder
+from flowhigh.model.Attr import Attr, AttrBuilder
 from flowhigh.model.CreateView import CreateView, CreateViewBuilder
 from flowhigh.model.InsertStatement import InsertStatement, InsertStatementBuilder
-from flowhigh.model.Attr import Attr, AttrBuilder
 from flowhigh.model.DBO import DBO, DBOBuilder
 from flowhigh.model.TreeNode import TreeNode
 from flowhigh.model.CreateStage import CreateStage, CreateStageBuilder
 from flowhigh.model.Sort import Sort, SortBuilder
 from flowhigh.model.Then import Then, ThenBuilder
-from flowhigh.model.MergeStatement import MergeStatement, MergeStatementBuilder
 from flowhigh.model.MultiValue import MultiValue, MultiValueBuilder
-from flowhigh.model.AntiPattern import AntiPattern, AntiPatternBuilder
+from flowhigh.model.MergeStatement import MergeStatement, MergeStatementBuilder
 from flowhigh.model.ExprExprHolder import ExprExprHolder
+from flowhigh.model.AntiPattern import AntiPattern, AntiPatternBuilder
 from flowhigh.model.BaseExprHolder import BaseExprHolder
 from flowhigh.model.UpdateStatement import UpdateStatement, UpdateStatementBuilder
 from flowhigh.model.QueryingStage import QueryingStage, QueryingStageBuilder
 from flowhigh.model.Position import Position, PositionBuilder
 from flowhigh.model.ExprCollectionHolder import ExprCollectionHolder
 from flowhigh.model.Const import Const, ConstBuilder
 from flowhigh.model.SubString import SubString
@@ -38,25 +38,26 @@
 from flowhigh.model.TypeCast import TypeCast
 from flowhigh.model.Current import Current, CurrentBuilder
 from flowhigh.model.Cast import Cast, CastBuilder
 from flowhigh.model.Frame import Frame, FrameBuilder
 from flowhigh.model.WrappedExprs import WrappedExprs
 from flowhigh.model.Rotate import Rotate, RotateBuilder
 from flowhigh.model.BaseExprCollectionHolder import BaseExprCollectionHolder
-from flowhigh.model.In import In, InBuilder
 from flowhigh.model.Func import Func, FuncBuilder
+from flowhigh.model.In import In, InBuilder
 from flowhigh.model.ReferencableExpr import ReferencableExpr
 from flowhigh.model.Case import Case, CaseBuilder
 from flowhigh.model.StructRef import StructRef, StructRefBuilder
 from flowhigh.model.AntiPatterns import AntiPatterns, AntiPatternsBuilder
 from flowhigh.model.Create import Create, CreateBuilder
-from flowhigh.model.Searchable import Searchable
-from flowhigh.model.MatchRecognize import MatchRecognize, MatchRecognizeBuilder
 from flowhigh.model.DBOHier import DBOHier, DBOHierBuilder
+from flowhigh.model.MatchRecognize import MatchRecognize, MatchRecognizeBuilder
+from flowhigh.model.Searchable import Searchable
 from flowhigh.model.Asterisk import Asterisk, AsteriskBuilder
+from flowhigh.model.Modifier import Modifier
 from flowhigh.model.Agg import Agg, AggBuilder
 from flowhigh.model.Named import Named
 from flowhigh.model.Statement import Statement, StatementBuilder
 from flowhigh.model.CoordinateBlock import CoordinateBlock
 from flowhigh.model.ParSeQL import ParSeQL, ParSeQLBuilder
 from flowhigh.model.TableSample import TableSample, TableSampleBuilder
 from flowhigh.model.Join import Join, JoinBuilder
```

### Comparing `flowhigh-1.0.2/flowhigh/utils/converter.py` & `flowhigh-1.0.3/flowhigh/utils/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 import requests
 import json
 
 from requests import RequestException, Timeout
-from typing import Type, Tuple, Union
+from typing import Tuple, Union
+
 from flowhigh.auth import Authentication
-from flowhigh.model.TreeNode import RegistryBase, TreeNode
+from flowhigh.model.TreeNode import RegistryBase
 from flowhigh.model import *
 from flowhigh.model.Delete import DeleteBuilder
 from flowhigh.model.Op import OpBuilder
 from flowhigh.model.InlineTable import InlineTableBuilder
 from flowhigh.model.Page import PageBuilder
-from flowhigh.model.Insert import InsertBuilder
 from flowhigh.model.Update import UpdateBuilder
+from flowhigh.model.Insert import InsertBuilder
 from flowhigh.model.DeleteStatement import DeleteStatementBuilder
+from flowhigh.model.Attr import AttrBuilder
 from flowhigh.model.CreateView import CreateViewBuilder
 from flowhigh.model.InsertStatement import InsertStatementBuilder
-from flowhigh.model.Attr import AttrBuilder
 from flowhigh.model.DBO import DBOBuilder
 from flowhigh.model.CreateStage import CreateStageBuilder
 from flowhigh.model.Sort import SortBuilder
 from flowhigh.model.Then import ThenBuilder
-from flowhigh.model.MergeStatement import MergeStatementBuilder
 from flowhigh.model.MultiValue import MultiValueBuilder
+from flowhigh.model.MergeStatement import MergeStatementBuilder
 from flowhigh.model.AntiPattern import AntiPatternBuilder
 from flowhigh.model.UpdateStatement import UpdateStatementBuilder
 from flowhigh.model.QueryingStage import QueryingStageBuilder
 from flowhigh.model.Position import PositionBuilder
 from flowhigh.model.Const import ConstBuilder
 from flowhigh.model.CreateTableStatement import CreateTableStatementBuilder
 from flowhigh.model.ColumnDef import ColumnDefBuilder
 from flowhigh.model.Ds import DsBuilder
 from flowhigh.model.Out import OutBuilder
 from flowhigh.model.Copy import CopyBuilder
 from flowhigh.model.Current import CurrentBuilder
 from flowhigh.model.Cast import CastBuilder
 from flowhigh.model.Frame import FrameBuilder
 from flowhigh.model.Rotate import RotateBuilder
-from flowhigh.model.In import InBuilder
 from flowhigh.model.Func import FuncBuilder
+from flowhigh.model.In import InBuilder
 from flowhigh.model.Case import CaseBuilder
 from flowhigh.model.StructRef import StructRefBuilder
 from flowhigh.model.AntiPatterns import AntiPatternsBuilder
 from flowhigh.model.Create import CreateBuilder
-from flowhigh.model.MatchRecognize import MatchRecognizeBuilder
 from flowhigh.model.DBOHier import DBOHierBuilder
+from flowhigh.model.MatchRecognize import MatchRecognizeBuilder
 from flowhigh.model.Asterisk import AsteriskBuilder
 from flowhigh.model.Agg import AggBuilder
 from flowhigh.model.Statement import StatementBuilder
 from flowhigh.model.ParSeQL import ParSeQLBuilder
 from flowhigh.model.TableSample import TableSampleBuilder
 from flowhigh.model.Join import JoinBuilder
 from flowhigh.model.Error import ErrorBuilder
@@ -87,15 +88,15 @@
             access_token = Authentication.authenticate_user()
             assert access_token, "UNAUTHENTICATED!"
             headers = {
                 "User-Agent": "python/sqlanalyzer-0.0.1",
                 "Content-type": "application/json",
                 "Authorization": "Bearer " + access_token
             }
-            url = "https://fhdev.sonra.io/api/process"
+            url = "https://flowhigh.sonra.io/api/process"
             data = {"sql": sql, "json": True, "xml": True}
             response = requests.post(url, json=data, headers=headers, timeout=5)
             # refresh token is invalid -> retry authentication
             if response.status_code == 401:
                 access_token = Authentication.request_device_code()
                 headers = {
                     "User-Agent": "python/sqlanalyzer-0.0.1",
@@ -122,15 +123,15 @@
         return cls.from_sql(sql=txt)
 
     def get_statements(self):
         return self._parsed_tree.statement
 
     @classmethod
     def get_main_dataset(cls, statement: Statement):
-        return statement.ds[-1]
+        return next(filter(lambda ds: ds.type_ == "root", statement.ds))
 
     def get_input(self, statement: Statement):
         return self.get_main_dataset(statement).in_
 
     def get_antipattern_of_statement(self, statement: Statement):
         """
         Returns the Anti-patterns for a statement
@@ -148,15 +149,15 @@
         statements = self.get_statements()
         for statement in statements:
             antipatterns.extend(statement.antiPatterns)
 
         return antipatterns
 
     @classmethod
-    def get_nodes_by_types(cls, types: Union[Tuple, str]):
+    def get_nodes_by_types(cls, types: Union[str, Tuple]):
         """
         Get the list of nodes in tree of a given type
         :param types: the type or the tuple of types
         :return: list of nodes that match the given types
         """
         return list(filter(lambda x: isinstance(x, types), RegistryBase.get_registry()))
 
@@ -172,51 +173,20 @@
     @classmethod
     def get_node_raw_text(cls, node):
         """
         Get the sql text at the node's coordinates in query
         :param node:
         :return: the sql at the node's coordinates
         """
-        if not node.pos:
-            return
-        stat = cls.find_first_ancestor_of_type(node, Statement)
-        source_lower_bound, source_upper_bound = node.pos.split('-')
-        return cls.get_raw_query(stat)[int(source_lower_bound): int(source_upper_bound)]
-
-    @classmethod
-    def get_ds_name(cls, node):
-        """
-        Get the node's dataset name
-        :param node:
-        :return: name of the node's dataset
-        """
-        if getattr(node, "alias", None):
-            return node.alias
-        if getattr(node, "refds", None):
-            return node.refds
-        ancestor = cls.find_first_ancestor_of_type(node, Ds)
-        return ancestor.alias or ancestor.refds
-
-    @classmethod
-    def is_set_operation(cls, statement: Statement):
-        """
-        Check if input queries are combined by set operators
-        :param statement:
-        :return: True if any of INTERSECT/MINUS/EXCEPT/UNION [ ALL ] in query
-        """
-        return getattr(cls.get_main_dataset(statement), "setOp", None)
-
-    @classmethod
-    def get_set_operator(cls, statement: Statement):
-        """
-        Extract the set operator from query
-        :param statement:
-        :return: Any of INTERSECT/MINUS/EXCEPT/UNION [ ALL ]
-        """
-        return cls.get_main_dataset(statement).setOp
+        raw = ''
+        if getattr(node, 'pos', None):
+            stat = cls.find_ancestor_of_type(node, Statement)
+            source_lower_bound, length = node.pos.split('-')  # NOQA
+            raw = cls.get_raw_query(stat)[int(source_lower_bound): int(source_lower_bound) + int(length)]
+        return " ".join(raw.split())
 
     @classmethod
     def search_node_by_id(cls, node_id: int):
         """
         Find a node in the tree based on its id
         :param node_id:
         :return: a node with the given id or None
@@ -226,58 +196,232 @@
     @classmethod
     def search_node_by_pos(cls, pos: str):
         """
         Find a node based on its position in query
         :param pos:
         :return: the node at the given coordinates or None
         """
-        return next(filter(lambda x: x.pos == pos, RegistryBase.get_registry()), None)
+        return next(filter(lambda x: getattr(x, 'pos', None) and x.pos == pos, RegistryBase.get_registry()), None)
+
+    @classmethod
+    def search_origin_reference(cls, attref: str):
+        """
+        Find a node based on its origin reference
+        :param attref: the coordinates of the referenced node
+        :return: the node at the given coordinates or None
+        """
+        return cls.search_node_by_pos(attref)
 
     @classmethod
     def get_out_columns(cls, statement):
         """
         Get the set of columns returned by the input query
         :param statement:
         :return: the set of columns returned by the input query
         """
         out = cls.get_main_dataset(statement).out
         return out.exprs
 
+    def get_DBO_hierarchy(self):
+        """
+        Get the DBO hierarchy
+        :return: the hierarchy with all the DBOs
+        """
+        return self._parsed_tree.DBOHier_.dbo
+
+    def get_tables(self):
+        """
+        Returns the list of table used in query
+        :return: the set of tables used by the input query
+        """
+        return [dbo for dbo in self.get_DBO_hierarchy() if dbo.type_ == "TABLE"]
+
+    def get_table_columns(self, table: DBO):
+        """
+        Returns the list of given table's columns
+        :param table: the DBO representing the physical table
+        :return: its set of columns
+        """
+        return table.dbo
+
+    def get_where_cols(self, statement: Statement):
+        """
+        List the attributes used in filters
+        :param statement: The input statement object with the submitted SQL
+        :return the Set of attributes
+        """
+        def _get_where_cols(node: TreeNode, accum: set):
+            if not node:
+                return
+            if isinstance(node, Ds) and node.modifiers:
+                cols = [self.find_descendants_of_type(f.op, (Attr,)) for f in node.modifiers
+                        if isinstance(f, Filter) and f.type_ == 'filtreg']
+                accum.update(*cols)
+            for child in node.get_children():
+                _get_where_cols(child, accum)
+
+        l = set()
+        _get_where_cols(statement, l)
+        return set(map(lambda attr: self.get_object_from_dbohier(attr.dboref), l))
+
+    def get_having_cols(self, statement: Statement):
+        """
+        List the attributes used in HAVING clause
+        :param statement: The input statement object with the submitted SQL
+        :return: the Set of attributes
+        """
+        def _get_having_cols(node: TreeNode, accum: set):
+            if not node:
+                return
+            if isinstance(node, Ds) and node.modifiers:
+                exprs = [f.op for f in node.modifiers if isinstance(f, Filter) and f.type_ == 'filtagg']
+                for e in exprs:
+                    for attr in self.find_descendants_of_type(e, (Attr,)):
+                        # e.g. select department_id, count(department_id) x
+                        # from employees group by department_id having x < 10;
+                        if attr.attref:
+                            exprs.append(self.search_origin_reference(attr.attref))
+                            continue
+                        accum.add(self.get_object_from_dbohier(attr.dboref))
+            for child in node.get_children():
+                _get_having_cols(child, accum)
+
+        l = set()
+        _get_having_cols(statement, l)
+        return l
+
+    def get_groupby_cols(self, statement: Statement):
+        """
+        List the attributes used in GROUP BY
+        :param statement: The input statement object with the submitted SQL
+        :return: the Set of attributes
+        """
+        def _get_groupby_cols(node: TreeNode, accum: set):
+            if not node:
+                return
+            if isinstance(node, Agg):
+                out_ds: Out = self.find_ancestor_of_type(node, (Ds,)).out
+                exprs = node.exprs
+                for e in exprs:
+                    for attr in self.find_descendants_of_type(e, (Attr,)):
+                        if attr.refoutidx:
+                            exprs.append(out_ds.exprs[int(attr.refoutidx) - 1])
+                            continue
+                        if attr.attref:
+                            exprs.append(self.search_origin_reference(attr.attref))
+                            continue
+                        dboref = self.get_object_from_dbohier(attr.dboref)
+                        accum.add(dboref) if dboref else None
+            for child in node.get_children():
+                _get_groupby_cols(child, accum)
+
+        l = set()
+        _get_groupby_cols(statement, l)
+        return l
+
+    def get_orderby_cols(self, statement: Statement):
+        """
+        List the attributes used in ORDER BY
+        :param statement: The input statement object with the submitted SQL
+        :return: the Set of attributes
+        """
+        def _get_sort_cols(node: TreeNode, accum: set):
+            if not node:
+                return
+            if isinstance(node, Sort):
+                out_ds: Out = self.find_ancestor_of_type(node, (Ds,)).out
+                exprs = node.exprs
+                for e in exprs:
+                    for attr in self.find_descendants_of_type(e, (Attr,)):
+                        if attr.refoutidx:
+                            exprs.append(out_ds.exprs[int(attr.refoutidx) - 1])
+                            continue
+                        if attr.attref:
+                            exprs.append(self.search_origin_reference(attr.attref))
+                            continue
+                        dboref = self.get_object_from_dbohier(attr.dboref)
+                        accum.add(dboref) if dboref else None
+            for child in node.get_children():
+                _get_sort_cols(child, accum)
+
+        l = set()
+        _get_sort_cols(statement, l)
+        return l
+
+    def get_object_from_dbohier(self, dboref: str):
+        """
+        Look up the DBO element in the hierarchy based on the oid
+        :param dboref: DBO reference
+        :return: the DBO matching the dboref if any
+        """
+        def _get_obj_from_dbohier(dbo: DBO):
+            if not dbo:
+                return
+            if dbo.oid == dboref:
+                return dbo
+            for child in dbo.dbo:
+                res = _get_obj_from_dbohier(child)
+                if res:
+                    return res
+
+        for d in self.get_DBO_hierarchy():
+            match = _get_obj_from_dbohier(d)
+            if match:
+                return match
+
     @classmethod
-    def find_first_ancestor_of_type(cls, node: TreeNode, clazz: Union[Tuple, TreeNode]):
+    def get_DBO_fullref(cls, dbo: DBO):
+        """
+        Return the DBO's fully qualified name
+        :param dbo: the DBO object whose name needs to be calculated
+        :return: the DBO's fully qualified name
+        """
+        if not dbo:
+            return
+        parent = dbo.get_parent()
+        if parent and isinstance(parent, DBOHier):
+            return dbo.name
+        if parent and isinstance(dbo, DBO):
+            return ".".join(filter(None, (cls.get_DBO_fullref(parent), dbo.name.casefold())))
+
+    @classmethod
+    def find_ancestor_of_type(cls, node: TreeNode, clazz: Union[TreeNode, Tuple]):
         """
         Find the node's immediate ancestor by its type
-        :param node:
-        :param clazz:
+        :param node: the node whose ancestor needs to be returned
+        :param clazz: the type to match
         :return: the node's ancestor or None
         """
         if node.get_parent() is None:
             return None
         parent_obj = node.get_parent()
         if isinstance(parent_obj, clazz):
             return parent_obj
-        return cls.find_first_ancestor_of_type(parent_obj, clazz)
+        return cls.find_ancestor_of_type(parent_obj, clazz)
 
     @classmethod
-    def find_descendants_of_type(cls, node: TreeNode, clazz: Union[Tuple, TreeNode]):
+    def find_descendants_of_type(cls, node: TreeNode, clazz: Union[TreeNode, Tuple], all=True):
         """
         Find the list of children based on their type
-        :param node:
-        :param clazz:
+        :param node: the node whose ancestor needs to be returned
+        :param clazz: the type to match
+        :param all: True if to return all descendants matching the from all the sub-levels. Default: True
         :return: the set of descendants
         """
         def _find_descendants_of_type(source_obj, accum):
             if not source_obj:
                 return
             if isinstance(source_obj, clazz):
-                accum.append(source_obj)
-                return
+                accum.add(source_obj)
+                if not all:
+                    return
             for child in source_obj.get_children():
                 _find_descendants_of_type(child, accum)
-        l = []
+
+        l = set()
         _find_descendants_of_type(node, l)
         return l
 
     
     def _convert_Delete(self, kwargs):
         obj = DeleteBuilder()
         
@@ -338,14 +482,30 @@
         if "type" in kwargs:
             obj.with_type(kwargs["type"])
         
         if "value" in kwargs:
             obj.with_value(self._convert_node(kwargs["value"]))
         return obj.build()
     
+    def _convert_Update(self, kwargs):
+        obj = UpdateBuilder()
+        
+        if "pos" in kwargs:
+            obj.with_pos(self._convert_node(kwargs["pos"]))
+        
+        if "alias" in kwargs:
+            obj.with_alias(self._convert_node(kwargs["alias"]))
+        
+        if "ds" in kwargs:
+            obj.with_ds(self._convert_node(kwargs["ds"]))
+        
+        if "direction" in kwargs:
+            obj.with_direction(kwargs["direction"])
+        return obj.build()
+    
     def _convert_Insert(self, kwargs):
         obj = InsertBuilder()
         
         if "ctes" in kwargs:
             obj.with_ctes([self._convert_node(f) for f in kwargs["ctes"]])
         
         if "isElse" in kwargs:
@@ -369,30 +529,14 @@
         if "overwrite" in kwargs:
             obj.with_overwrite(self._convert_node(kwargs["overwrite"]))
         
         if "direction" in kwargs:
             obj.with_direction(kwargs["direction"])
         return obj.build()
     
-    def _convert_Update(self, kwargs):
-        obj = UpdateBuilder()
-        
-        if "pos" in kwargs:
-            obj.with_pos(self._convert_node(kwargs["pos"]))
-        
-        if "alias" in kwargs:
-            obj.with_alias(self._convert_node(kwargs["alias"]))
-        
-        if "ds" in kwargs:
-            obj.with_ds(self._convert_node(kwargs["ds"]))
-        
-        if "direction" in kwargs:
-            obj.with_direction(kwargs["direction"])
-        return obj.build()
-    
     def _convert_DeleteStatement(self, kwargs):
         obj = DeleteStatementBuilder()
         
         if "pos" in kwargs:
             obj.with_pos(self._convert_node(kwargs["pos"]))
         
         if "merge" in kwargs:
@@ -428,14 +572,54 @@
         if "delete" in kwargs:
             obj.with_delete([self._convert_node(f) for f in kwargs["delete"]])
         
         if "ds" in kwargs:
             obj.with_ds([self._convert_node(f) for f in kwargs["ds"]])
         return obj.build()
     
+    def _convert_Attr(self, kwargs):
+        obj = AttrBuilder()
+        
+        if "refsch" in kwargs:
+            obj.with_refsch(self._convert_node(kwargs["refsch"]))
+        
+        if "fullref" in kwargs:
+            obj.with_fullref(self._convert_node(kwargs["fullref"]))
+        
+        if "refvar" in kwargs:
+            obj.with_refvar(self._convert_node(kwargs["refvar"]))
+        
+        if "refdb" in kwargs:
+            obj.with_refdb(self._convert_node(kwargs["refdb"]))
+        
+        if "pos" in kwargs:
+            obj.with_pos(self._convert_node(kwargs["pos"]))
+        
+        if "refds" in kwargs:
+            obj.with_refds(self._convert_node(kwargs["refds"]))
+        
+        if "refatt" in kwargs:
+            obj.with_refatt(self._convert_node(kwargs["refatt"]))
+        
+        if "alias" in kwargs:
+            obj.with_alias(self._convert_node(kwargs["alias"]))
+        
+        if "attref" in kwargs:
+            obj.with_attref(self._convert_node(kwargs["attref"]))
+        
+        if "refoutidx" in kwargs:
+            obj.with_refoutidx(self._convert_node(kwargs["refoutidx"]))
+        
+        if "dboref" in kwargs:
+            obj.with_dboref(self._convert_node(kwargs["dboref"]))
+        
+        if "direction" in kwargs:
+            obj.with_direction(kwargs["direction"])
+        return obj.build()
+    
     def _convert_CreateView(self, kwargs):
         obj = CreateViewBuilder()
         
         if "pos" in kwargs:
             obj.with_pos(self._convert_node(kwargs["pos"]))
         
         if "columns" in kwargs:
@@ -493,54 +677,14 @@
         if "delete" in kwargs:
             obj.with_delete([self._convert_node(f) for f in kwargs["delete"]])
         
         if "ds" in kwargs:
             obj.with_ds([self._convert_node(f) for f in kwargs["ds"]])
         return obj.build()
     
-    def _convert_Attr(self, kwargs):
-        obj = AttrBuilder()
-        
-        if "refsch" in kwargs:
-            obj.with_refsch(self._convert_node(kwargs["refsch"]))
-        
-        if "fullref" in kwargs:
-            obj.with_fullref(self._convert_node(kwargs["fullref"]))
-        
-        if "refvar" in kwargs:
-            obj.with_refvar(self._convert_node(kwargs["refvar"]))
-        
-        if "refdb" in kwargs:
-            obj.with_refdb(self._convert_node(kwargs["refdb"]))
-        
-        if "pos" in kwargs:
-            obj.with_pos(self._convert_node(kwargs["pos"]))
-        
-        if "refds" in kwargs:
-            obj.with_refds(self._convert_node(kwargs["refds"]))
-        
-        if "refatt" in kwargs:
-            obj.with_refatt(self._convert_node(kwargs["refatt"]))
-        
-        if "alias" in kwargs:
-            obj.with_alias(self._convert_node(kwargs["alias"]))
-        
-        if "attref" in kwargs:
-            obj.with_attref(self._convert_node(kwargs["attref"]))
-        
-        if "refoutidx" in kwargs:
-            obj.with_refoutidx(self._convert_node(kwargs["refoutidx"]))
-        
-        if "dboref" in kwargs:
-            obj.with_dboref(self._convert_node(kwargs["dboref"]))
-        
-        if "direction" in kwargs:
-            obj.with_direction(kwargs["direction"])
-        return obj.build()
-    
     def _convert_DBO(self, kwargs):
         obj = DBOBuilder()
         
         if "dbo" in kwargs:
             obj.with_dbo([self._convert_node(f) for f in kwargs["dbo"]])
         
         if "name" in kwargs:
@@ -615,14 +759,30 @@
         if "expr" in kwargs:
             obj.with_expr(self._convert_node(kwargs["expr"]))
         
         if "direction" in kwargs:
             obj.with_direction(kwargs["direction"])
         return obj.build()
     
+    def _convert_MultiValue(self, kwargs):
+        obj = MultiValueBuilder()
+        
+        if "pos" in kwargs:
+            obj.with_pos(self._convert_node(kwargs["pos"]))
+        
+        if "exprs" in kwargs:
+            obj.with_exprs([self._convert_node(f) for f in kwargs["exprs"]])
+        
+        if "alias" in kwargs:
+            obj.with_alias(self._convert_node(kwargs["alias"]))
+        
+        if "direction" in kwargs:
+            obj.with_direction(kwargs["direction"])
+        return obj.build()
+    
     def _convert_MergeStatement(self, kwargs):
         obj = MergeStatementBuilder()
         
         if "pos" in kwargs:
             obj.with_pos(self._convert_node(kwargs["pos"]))
         
         if "merge" in kwargs:
@@ -658,30 +818,14 @@
         if "delete" in kwargs:
             obj.with_delete([self._convert_node(f) for f in kwargs["delete"]])
         
         if "ds" in kwargs:
             obj.with_ds([self._convert_node(f) for f in kwargs["ds"]])
         return obj.build()
     
-    def _convert_MultiValue(self, kwargs):
-        obj = MultiValueBuilder()
-        
-        if "pos" in kwargs:
-            obj.with_pos(self._convert_node(kwargs["pos"]))
-        
-        if "exprs" in kwargs:
-            obj.with_exprs([self._convert_node(f) for f in kwargs["exprs"]])
-        
-        if "alias" in kwargs:
-            obj.with_alias(self._convert_node(kwargs["alias"]))
-        
-        if "direction" in kwargs:
-            obj.with_direction(kwargs["direction"])
-        return obj.build()
-    
     def _convert_AntiPattern(self, kwargs):
         obj = AntiPatternBuilder()
         
         if "severity" in kwargs:
             obj.with_severity(self._convert_node(kwargs["severity"]))
         
         if "readability" in kwargs:
@@ -869,76 +1013,70 @@
         if "type" in kwargs:
             obj.with_type(self._convert_node(kwargs["type"]))
         return obj.build()
     
     def _convert_Ds(self, kwargs):
         obj = DsBuilder()
         
-        if "agg" in kwargs:
-            obj.with_agg(self._convert_node(kwargs["agg"]))
-        
         if "refsch" in kwargs:
             obj.with_refsch(self._convert_node(kwargs["refsch"]))
         
         if "fullref" in kwargs:
             obj.with_fullref(self._convert_node(kwargs["fullref"]))
         
         if "refdb" in kwargs:
             obj.with_refdb(self._convert_node(kwargs["refdb"]))
         
         if "in" in kwargs:
             obj.with_in(self._convert_node(kwargs["in"]))
         
-        if "setOp" in kwargs:
-            obj.with_setOp([self._convert_node(f) for f in kwargs["setOp"]])
-        
         if "matchRecognize" in kwargs:
             obj.with_matchRecognize(self._convert_node(kwargs["matchRecognize"]))
         
-        if "sort" in kwargs:
-            obj.with_sort(self._convert_node(kwargs["sort"]))
+        if "setOp" in kwargs:
+            obj.with_setOp([self._convert_node(f) for f in kwargs["setOp"]])
         
         if "type" in kwargs:
             obj.with_type(kwargs["type"])
         
+        if "modifiers" in kwargs:
+            obj.with_modifiers([self._convert_node(f) for f in kwargs["modifiers"]])
+        
         if "out" in kwargs:
             obj.with_out(self._convert_node(kwargs["out"]))
         
         if "tableSample" in kwargs:
             obj.with_tableSample(self._convert_node(kwargs["tableSample"]))
         
-        if "filter" in kwargs:
-            obj.with_filter([self._convert_node(f) for f in kwargs["filter"]])
-        
         if "pos" in kwargs:
             obj.with_pos(self._convert_node(kwargs["pos"]))
         
         if "refds" in kwargs:
             obj.with_refds(self._convert_node(kwargs["refds"]))
         
         if "name" in kwargs:
             obj.with_name(self._convert_node(kwargs["name"]))
         
-        if "action" in kwargs:
-            obj.with_action(kwargs["action"])
-        
         if "alias" in kwargs:
             obj.with_alias(self._convert_node(kwargs["alias"]))
         
+        if "action" in kwargs:
+            obj.with_action(kwargs["action"])
+        
         if "subType" in kwargs:
             obj.with_subType(kwargs["subType"])
         
-        if "page" in kwargs:
-            obj.with_page(self._convert_node(kwargs["page"]))
-        
         if "refTo" in kwargs:
             obj.with_refTo(self._convert_node(kwargs["refTo"]))
         
         if "direction" in kwargs:
             obj.with_direction(kwargs["direction"])
+        
+        if "dboref" in kwargs:
+            obj.with_dboref(self._convert_node(kwargs["dboref"]))
         return obj.build()
     
     def _convert_Out(self, kwargs):
         obj = OutBuilder()
         
         if "pos" in kwargs:
             obj.with_pos(self._convert_node(kwargs["pos"]))
@@ -1095,24 +1233,14 @@
         if "aggregate" in kwargs:
             obj.with_aggregate(self._convert_node(kwargs["aggregate"]))
         
         if "direction" in kwargs:
             obj.with_direction(kwargs["direction"])
         return obj.build()
     
-    def _convert_In(self, kwargs):
-        obj = InBuilder()
-        
-        if "pos" in kwargs:
-            obj.with_pos(self._convert_node(kwargs["pos"]))
-        
-        if "exprs" in kwargs:
-            obj.with_exprs([self._convert_node(f) for f in kwargs["exprs"]])
-        return obj.build()
-    
     def _convert_Func(self, kwargs):
         obj = FuncBuilder()
         
         if "partition" in kwargs:
             obj.with_partition([self._convert_node(f) for f in kwargs["partition"]])
         
         if "pos" in kwargs:
@@ -1129,14 +1257,17 @@
         
         if "alias" in kwargs:
             obj.with_alias(self._convert_node(kwargs["alias"]))
         
         if "expr" in kwargs:
             obj.with_expr(self._convert_node(kwargs["expr"]))
         
+        if "subType" in kwargs:
+            obj.with_subType(kwargs["subType"])
+        
         if "sort" in kwargs:
             obj.with_sort(self._convert_node(kwargs["sort"]))
         
         if "quantifier" in kwargs:
             obj.with_quantifier(kwargs["quantifier"])
         
         if "type" in kwargs:
@@ -1145,14 +1276,24 @@
         if "frame" in kwargs:
             obj.with_frame(self._convert_node(kwargs["frame"]))
         
         if "direction" in kwargs:
             obj.with_direction(kwargs["direction"])
         return obj.build()
     
+    def _convert_In(self, kwargs):
+        obj = InBuilder()
+        
+        if "pos" in kwargs:
+            obj.with_pos(self._convert_node(kwargs["pos"]))
+        
+        if "exprs" in kwargs:
+            obj.with_exprs([self._convert_node(f) for f in kwargs["exprs"]])
+        return obj.build()
+    
     def _convert_Case(self, kwargs):
         obj = CaseBuilder()
         
         if "pos" in kwargs:
             obj.with_pos(self._convert_node(kwargs["pos"]))
         
         if "Else" in kwargs:
@@ -1257,14 +1398,21 @@
         if "clusterBy" in kwargs:
             obj.with_clusterBy([self._convert_node(f) for f in kwargs["clusterBy"]])
         
         if "ds" in kwargs:
             obj.with_ds([self._convert_node(f) for f in kwargs["ds"]])
         return obj.build()
     
+    def _convert_DBOHier(self, kwargs):
+        obj = DBOHierBuilder()
+        
+        if "dbo" in kwargs:
+            obj.with_dbo([self._convert_node(f) for f in kwargs["dbo"]])
+        return obj.build()
+    
     def _convert_MatchRecognize(self, kwargs):
         obj = MatchRecognizeBuilder()
         
         if "partitionBy" in kwargs:
             obj.with_partitionBy(self._convert_node(kwargs["partitionBy"]))
         
         if "measures" in kwargs:
@@ -1291,21 +1439,14 @@
         if "rowMatchCondition" in kwargs:
             obj.with_rowMatchCondition(self._convert_node(kwargs["rowMatchCondition"]))
         
         if "direction" in kwargs:
             obj.with_direction(kwargs["direction"])
         return obj.build()
     
-    def _convert_DBOHier(self, kwargs):
-        obj = DBOHierBuilder()
-        
-        if "dbo" in kwargs:
-            obj.with_dbo([self._convert_node(f) for f in kwargs["dbo"]])
-        return obj.build()
-    
     def _convert_Asterisk(self, kwargs):
         obj = AsteriskBuilder()
         
         if "refsch" in kwargs:
             obj.with_refsch(self._convert_node(kwargs["refsch"]))
         
         if "fullref" in kwargs:
@@ -1543,20 +1684,20 @@
         if "type" in kwargs:
             obj.with_type(kwargs["type"])
         return obj.build()
     
     def _convert_TableFunc(self, kwargs):
         obj = TableFuncBuilder()
         
-        if "agg" in kwargs:
-            obj.with_agg(self._convert_node(kwargs["agg"]))
-        
         if "type" in kwargs:
             obj.with_type(kwargs["type"])
         
+        if "modifiers" in kwargs:
+            obj.with_modifiers([self._convert_node(f) for f in kwargs["modifiers"]])
+        
         if "out" in kwargs:
             obj.with_out(self._convert_node(kwargs["out"]))
         
         if "partition" in kwargs:
             obj.with_partition([self._convert_node(f) for f in kwargs["partition"]])
         
         if "pos" in kwargs:
@@ -1603,31 +1744,28 @@
         
         if "sort" in kwargs:
             obj.with_sort(self._convert_node(kwargs["sort"]))
         
         if "subQuery" in kwargs:
             obj.with_subQuery(self._convert_node(kwargs["subQuery"]))
         
-        if "filter" in kwargs:
-            obj.with_filter([self._convert_node(f) for f in kwargs["filter"]])
-        
         if "tableSample" in kwargs:
             obj.with_tableSample(self._convert_node(kwargs["tableSample"]))
         
         if "names" in kwargs:
             obj.with_names([self._convert_node(f) for f in kwargs["names"]])
         
         if "name" in kwargs:
             obj.with_name(self._convert_node(kwargs["name"]))
         
         if "subType" in kwargs:
             obj.with_subType(kwargs["subType"])
         
-        if "page" in kwargs:
-            obj.with_page(self._convert_node(kwargs["page"]))
+        if "dboref" in kwargs:
+            obj.with_dboref(self._convert_node(kwargs["dboref"]))
         
         if "frame" in kwargs:
             obj.with_frame(self._convert_node(kwargs["frame"]))
         return obj.build()
     
     def _convert_Else(self, kwargs):
         obj = ElseBuilder()
@@ -1680,38 +1818,38 @@
             return self._convert_Delete(kwargs)
         if kwargs["eltype"].lower() == "op":
             return self._convert_Op(kwargs)
         if kwargs["eltype"].lower() == "inlinetable":
             return self._convert_InlineTable(kwargs)
         if kwargs["eltype"].lower() == "page":
             return self._convert_Page(kwargs)
-        if kwargs["eltype"].lower() == "insert":
-            return self._convert_Insert(kwargs)
         if kwargs["eltype"].lower() == "update":
             return self._convert_Update(kwargs)
+        if kwargs["eltype"].lower() == "insert":
+            return self._convert_Insert(kwargs)
         if kwargs["eltype"].lower() == "deletestatement":
             return self._convert_DeleteStatement(kwargs)
+        if kwargs["eltype"].lower() == "attr":
+            return self._convert_Attr(kwargs)
         if kwargs["eltype"].lower() == "createview":
             return self._convert_CreateView(kwargs)
         if kwargs["eltype"].lower() == "insertstatement":
             return self._convert_InsertStatement(kwargs)
-        if kwargs["eltype"].lower() == "attr":
-            return self._convert_Attr(kwargs)
         if kwargs["eltype"].lower() == "dbo":
             return self._convert_DBO(kwargs)
         if kwargs["eltype"].lower() == "createstage":
             return self._convert_CreateStage(kwargs)
         if kwargs["eltype"].lower() == "sort":
             return self._convert_Sort(kwargs)
         if kwargs["eltype"].lower() == "then":
             return self._convert_Then(kwargs)
-        if kwargs["eltype"].lower() == "mergestatement":
-            return self._convert_MergeStatement(kwargs)
         if kwargs["eltype"].lower() == "multivalue":
             return self._convert_MultiValue(kwargs)
+        if kwargs["eltype"].lower() == "mergestatement":
+            return self._convert_MergeStatement(kwargs)
         if kwargs["eltype"].lower() == "antipattern":
             return self._convert_AntiPattern(kwargs)
         if kwargs["eltype"].lower() == "updatestatement":
             return self._convert_UpdateStatement(kwargs)
         if kwargs["eltype"].lower() == "queryingstage":
             return self._convert_QueryingStage(kwargs)
         if kwargs["eltype"].lower() == "position":
@@ -1732,30 +1870,30 @@
             return self._convert_Current(kwargs)
         if kwargs["eltype"].lower() == "cast":
             return self._convert_Cast(kwargs)
         if kwargs["eltype"].lower() == "frame":
             return self._convert_Frame(kwargs)
         if kwargs["eltype"].lower() == "rotate":
             return self._convert_Rotate(kwargs)
-        if kwargs["eltype"].lower() == "in":
-            return self._convert_In(kwargs)
         if kwargs["eltype"].lower() == "func":
             return self._convert_Func(kwargs)
+        if kwargs["eltype"].lower() == "in":
+            return self._convert_In(kwargs)
         if kwargs["eltype"].lower() == "case":
             return self._convert_Case(kwargs)
         if kwargs["eltype"].lower() == "structref":
             return self._convert_StructRef(kwargs)
         if kwargs["eltype"].lower() == "antipatterns":
             return self._convert_AntiPatterns(kwargs)
         if kwargs["eltype"].lower() == "create":
             return self._convert_Create(kwargs)
-        if kwargs["eltype"].lower() == "matchrecognize":
-            return self._convert_MatchRecognize(kwargs)
         if kwargs["eltype"].lower() == "dbohier":
             return self._convert_DBOHier(kwargs)
+        if kwargs["eltype"].lower() == "matchrecognize":
+            return self._convert_MatchRecognize(kwargs)
         if kwargs["eltype"].lower() == "asterisk":
             return self._convert_Asterisk(kwargs)
         if kwargs["eltype"].lower() == "agg":
             return self._convert_Agg(kwargs)
         if kwargs["eltype"].lower() == "statement":
             return self._convert_Statement(kwargs)
         if kwargs["eltype"].lower() == "parseql":
```

### Comparing `flowhigh-1.0.2/pyproject.toml` & `flowhigh-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flowhigh"
-version = "1.0.2"
+version = "1.0.3"
 description = "Python SDK for FlowHigh"
 authors = [
     { name = "sonra", email = "support@sonra.io" },
 ]
 dependencies = [
     "requests>=2.14.0",
 ]
```

### Comparing `flowhigh-1.0.2/tests/formatting-test/format_test.py` & `flowhigh-1.0.3/tests/formatting-test/format_test.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/tests/input.json` & `flowhigh-1.0.3/tests/input.json`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/tests/test.py` & `flowhigh-1.0.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.2/PKG-INFO` & `flowhigh-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowhigh
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python SDK for FlowHigh
 License: Proprietary
 Keywords: SQLAnalyzer SDK Python
 Author-email: sonra <support@sonra.io>
 Requires-Python: >=3.6
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

