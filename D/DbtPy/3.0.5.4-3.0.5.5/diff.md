# Comparing `tmp/DbtPy-3.0.5.4.tar.gz` & `tmp/DbtPy-3.0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DbtPy-3.0.5.4.tar", last modified: Thu Jun  9 02:53:35 2022, max compression
+gzip compressed data, was "dist/DbtPy-3.0.5.5.tar", last modified: Fri May 12 05:30:59 2023, max compression
```

## Comparing `DbtPy-3.0.5.4.tar` & `DbtPy-3.0.5.5.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 02:53:35.000000 DbtPy-3.0.5.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 02:53:35.000000 DbtPy-3.0.5.4/DbtPy.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1380 2022-06-09 02:53:35.000000 DbtPy-3.0.5.4/DbtPy.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5463 2022-06-09 02:53:35.000000 DbtPy-3.0.5.4/DbtPy.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-06-09 02:53:35.000000 DbtPy-3.0.5.4/DbtPy.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       15 2022-06-09 02:53:35.000000 DbtPy-3.0.5.4/DbtPy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 02:53:35.000000 DbtPy-3.0.5.4/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 02:53:35.000000 DbtPy-3.0.5.4/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)       18 2020-08-14 14:46:01.000000 DbtPy-3.0.5.4/tests/data/data1.txt
--rw-rw-rw-   0 root         (0) root         (0)       18 2020-08-14 14:46:01.000000 DbtPy-3.0.5.4/tests/data/data2.txt
--rw-rw-rw-   0 root         (0) root         (0)       18 2020-08-14 14:46:01.000000 DbtPy-3.0.5.4/tests/data/data3.txt
--rw-rw-rw-   0 root         (0) root         (0)       18 2020-08-14 14:46:01.000000 DbtPy-3.0.5.4/tests/data/data4.txt
--rw-rw-rw-   0 root         (0) root         (0)        8 2020-08-14 14:46:01.000000 DbtPy-3.0.5.4/tests/data/test_6755.txt
--rw-rw-rw-   0 root         (0) root         (0)        2 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4461 2020-08-14 14:46:01.000000 DbtPy-3.0.5.4/tests/pic1.jpg
--rw-rw-rw-   0 root         (0) root         (0)     3070 2020-08-14 14:46:01.000000 DbtPy-3.0.5.4/tests/spook.png
--rw-rw-rw-   0 root         (0) root         (0)    29172 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_000_PrepareDb.py
--rw-rw-rw-   0 root         (0) root         (0)      647 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_001_ConnDb.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_003_NumAffectedRows.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_004_ConnWrongUserPwd.py
--rw-rw-rw-   0 root         (0) root         (0)      724 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_005_ConnBadUserBadPwd.py
--rw-rw-rw-   0 root         (0) root         (0)     1403 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_006_ConnPassingOpts.py
--rw-rw-rw-   0 root         (0) root         (0)     2184 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_008_ColumnInfo.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_010_UpdateRowCount.py
--rw-rw-rw-   0 root         (0) root         (0)      871 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_011_DeleteRowCount.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_015_InsertDeleteRowCount_01.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_016_InsertDeleteRowCount_02.py
--rw-rw-rw-   0 root         (0) root         (0)     1325 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_020_RollbackDelete.py
--rw-rw-rw-   0 root         (0) root         (0)     1937 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_021_CommitDelete.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_022_RollbackInsert.py
--rw-rw-rw-   0 root         (0) root         (0)     1284 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_023_ColumnPrivileges.py
--rw-rw-rw-   0 root         (0) root         (0)     3261 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_024_ForeignKeys.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_025_PrimaryKeys.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_030_Result.py
--rw-rw-rw-   0 root         (0) root         (0)     1330 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_031_ResultIndexPosition.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_032_ResultIndexName.py
--rw-rw-rw-   0 root         (0) root         (0)     1283 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_033_ResultOutSequenceColumn.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_034_FetchAssoc.py
--rw-rw-rw-   0 root         (0) root         (0)     1464 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_035_FetchRow_01.py
--rw-rw-rw-   0 root         (0) root         (0)    28312 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_036_FetchRow_02.py
--rw-rw-rw-   0 root         (0) root         (0)    16367 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_037_FetchRowIndexPos.py
--rw-rw-rw-   0 root         (0) root         (0)    16581 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_038_FetchRowIndexPosNested_01.py
--rw-rw-rw-   0 root         (0) root         (0)     8924 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_039_FetchRowIndexPosNested_02.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_03a_ResultNonExistCol.py
--rw-rw-rw-   0 root         (0) root         (0)     1281 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_040_FetchTuple.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_045_FetchTupleBinaryData_01.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_048_FetchTupleBinaryData_02.py
--rw-rw-rw-   0 root         (0) root         (0)     1216 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_049_InsertNoneParam.py
--rw-rw-rw-   0 root         (0) root         (0)      511 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_050_AutocommitStatus.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_051_SetAutocommit_01.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_052_SetAutocommit_02.py
--rw-rw-rw-   0 root         (0) root         (0)     1218 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_054_CursorType.py
--rw-rw-rw-   0 root         (0) root         (0)     1897 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_060_Tables_01.py
--rw-rw-rw-   0 root         (0) root         (0)     1920 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_061_Tables_02.py
--rw-rw-rw-   0 root         (0) root         (0)     2027 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_062_Tables_03.py
--rw-rw-rw-   0 root         (0) root         (0)      601 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_063_Tables_04.py
--rw-rw-rw-   0 root         (0) root         (0)     1926 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_064_Tables_05.py
--rw-rw-rw-   0 root         (0) root         (0)     1850 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_065_FilterTableName.py
--rw-rw-rw-   0 root         (0) root         (0)     3281 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_066_TableObjects.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_070_Close.py
--rw-rw-rw-   0 root         (0) root         (0)      956 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_071_CloseSuccess.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_081_ConnWrongUser.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_082_ConnWrongPwd.py
--rw-rw-rw-   0 root         (0) root         (0)      566 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_091_ConnmsgWrongUser.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_092_ConnmsgWrongPwd.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_100_SelectDeleteInsertFieldCount.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_101_InsertDeleteFieldCount.py
--rw-rw-rw-   0 root         (0) root         (0)      912 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_102_NumFieldsSelect_01.py
--rw-rw-rw-   0 root         (0) root         (0)     2005 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_103_NumFieldsSelect_02.py
--rw-rw-rw-   0 root         (0) root         (0)     1197 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_110_FieldNum.py
--rw-rw-rw-   0 root         (0) root         (0)     1856 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_111_FieldNumAddCol.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_112_FieldNumDiffCaseColNames.py
--rw-rw-rw-   0 root         (0) root         (0)     1241 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_113_DateTest.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_114_NumericTest_01.py
--rw-rw-rw-   0 root         (0) root         (0)     2132 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_115_NumericTest_02.py
--rw-rw-rw-   0 root         (0) root         (0)     1476 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_116_ConnActive.py
--rw-rw-rw-   0 root         (0) root         (0)     1885 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_120_FieldName.py
--rw-rw-rw-   0 root         (0) root         (0)     2229 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_121_FieldNameAddCol.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_122_FieldNameDiffCaseColNames.py
--rw-rw-rw-   0 root         (0) root         (0)   163950 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_123_FieldNamePos_01.py
--rw-rw-rw-   0 root         (0) root         (0)    17097 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_124_FieldNamePos_02.py
--rw-rw-rw-   0 root         (0) root         (0)     1695 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_125_FieldNamePos_03.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_130_PrepExecuteSelectStmt.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_131_PrepareExecuteSelectStatementParams.py
--rw-rw-rw-   0 root         (0) root         (0)     1015 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_132_ExecuteStatementArrayMultipleParams.py
--rw-rw-rw-   0 root         (0) root         (0)     1928 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_133_ExecuteLongInputParams.py
--rw-rw-rw-   0 root         (0) root         (0)     1014 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_140_BindParamSelectStmt.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_141_BindParamSelectStmtMultipleParams_01.py
--rw-rw-rw-   0 root         (0) root         (0)     1640 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_142_BindParamSelectStmtMultipleParams_02.py
--rw-rw-rw-   0 root         (0) root         (0)     1257 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_143_BindParamInsertStmtNoneParam.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_144_BindParamInsertStmtPARAM_FILE.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_145_BindRetrieveNoneEmptyString.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_146_CallSPINAndOUTParams.py
--rw-rw-rw-   0 root         (0) root         (0)     1125 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_147_PrepareWithWrongType.py
--rw-rw-rw-   0 root         (0) root         (0)     1952 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_148_CallSPDiffBindPattern_01.py
--rw-rw-rw-   0 root         (0) root         (0)    10656 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_150_FetchAssocSelect_01.py
--rw-rw-rw-   0 root         (0) root         (0)     9158 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_151_FetchAssocSelect_02.py
--rw-rw-rw-   0 root         (0) root         (0)     7743 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_152_FetchAssocSelect_03.py
--rw-rw-rw-   0 root         (0) root         (0)     2750 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_153_FetchAssocSelect_04.py
--rw-rw-rw-   0 root         (0) root         (0)     8174 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_154_AllFetches.py
--rw-rw-rw-   0 root         (0) root         (0)    17678 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_155_FetchAssocSelect_05.py
--rw-rw-rw-   0 root         (0) root         (0)     7683 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_156_FetchAssocNestedSelects_01.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_157_FetchAssocScrollableCursor_01.py
--rw-rw-rw-   0 root         (0) root         (0)     4699 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_159_FetchAssocSeveralRows_01.py
--rw-rw-rw-   0 root         (0) root         (0)     1764 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_157a_FetchAssocWithoutScrollableCursorErr.py
--rw-rw-rw-   0 root         (0) root         (0)     2295 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_157b_FetchAssocScrollableCursor_02.py
--rw-rw-rw-   0 root         (0) root         (0)     6711 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_158_FetchAssocNestedSelects_02.py
--rw-rw-rw-   0 root         (0) root         (0)     3116 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_159a_FetchAssocSeveralRows_02.py
--rw-rw-rw-   0 root         (0) root         (0)    19143 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_160_FetchBoth.py
--rw-rw-rw-   0 root         (0) root         (0)     6083 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_161_FetchBothNestedSelects_01.py
--rw-rw-rw-   0 root         (0) root         (0)     6316 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_162_FetchBothNestedSelects_02.py
--rw-rw-rw-   0 root         (0) root         (0)     1891 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_180_StmtErrMsg.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_190_ColumnsTable_01.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_191_ColumnsTable_02.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_197_StatisticsIndexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_200_MultipleRsltsetsUniformColDefs.py
--rw-rw-rw-   0 root         (0) root         (0)     1737 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_201_MultipleRsltsetsDiffColDefs.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_210_FieldDisplaySize_01.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_211_FieldDisplaySize_02.py
--rw-rw-rw-   0 root         (0) root         (0)      936 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_212_FieldDisplaySize_03.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_213_FieldDisplaySize_04.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_230_FieldTypePos.py
--rw-rw-rw-   0 root         (0) root         (0)     1971 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_231_FieldTypeName.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_232_FieldTypePosName.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_240_FieldWidthPosName_01.py
--rw-rw-rw-   0 root         (0) root         (0)     1080 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_241_FieldWidthPosName_02.py
--rw-rw-rw-   0 root         (0) root         (0)      868 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_250_FreeResult_01.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_251_FreeResult_02.py
--rw-rw-rw-   0 root         (0) root         (0)     1687 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_261_FetchObjectAccess.py
--rw-rw-rw-   0 root         (0) root         (0)     2662 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_264_InsertRetrieveBIGINTTypeColumn.py
--rw-rw-rw-   0 root         (0) root         (0)     6371 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_265_NoAffectedRows.py
--rw-rw-rw-   0 root         (0) root         (0)     4587 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_300_ServerInfo.py
--rw-rw-rw-   0 root         (0) root         (0)     2035 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_310_ClientInfo.py
--rw-rw-rw-   0 root         (0) root         (0)     2914 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_311_InsertSelectDeleteNumLiterals.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_312_CacheBoundParameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1863 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_313_Collection.py
--rw-rw-rw-   0 root         (0) root         (0)     2359 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_314_Collection_Param.py
--rw-rw-rw-   0 root         (0) root         (0)     1514 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_315_UDT.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_316_UDT_Param.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_6528_ScopingProblemBindParam.py
--rw-rw-rw-   0 root         (0) root         (0)     1108 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_6561_InsertNULLValues.py
--rw-rw-rw-   0 root         (0) root         (0)     2167 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_6755_ExtraNULLChar_ResultCLOBCol.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_6792_FieldTypeRetStrDatetimeTimestamp.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_InsertRetrieveDateTimeTypeColumn.py
--rw-rw-rw-   0 root         (0) root         (0)     2014 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_SmartTrigger.py
--rw-rw-rw-   0 root         (0) root         (0)     3181 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_decimal.py
--rw-rw-rw-   0 root         (0) root         (0)     1737 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_spinout_timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/test_warn.py
--rw-rw-rw-   0 root         (0) root         (0)     1334 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/xtest_012_KeysetDrivenCursorSelect01.py
--rw-rw-rw-   0 root         (0) root         (0)     1305 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/xtest_013_KeysetDrivenCursorSelect02.py
--rw-rw-rw-   0 root         (0) root         (0)     2510 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/xtest_014_KeysetDrivenCursorNegativeRow.py
--rw-rw-rw-   0 root         (0) root         (0)     1784 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/xtest_018_selectRowcountPrefetchSetOpt.py
--rw-rw-rw-   0 root         (0) root         (0)     1028 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/xtest_019_selectRowcountPrefetchPrepOpt.py
--rw-rw-rw-   0 root         (0) root         (0)     3844 2020-12-13 05:04:27.000000 DbtPy-3.0.5.4/tests/xtest_053_AttrThruConn.py
--rw-rw-rw-   0 root         (0) root         (0)    56905 2021-04-07 06:17:36.000000 DbtPy-3.0.5.4/DbtPyDbi.py
--rw-rw-rw-   0 root         (0) root         (0)      464 2021-04-07 06:18:00.000000 DbtPy-3.0.5.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      268 2022-04-12 12:27:38.000000 DbtPy-3.0.5.4/README.md
--rw-r--r--   0 root         (0) root         (0)       17 2021-04-07 06:13:38.000000 DbtPy-3.0.5.4/README.rst
--rw-r--r--   0 root         (0) root         (0)    42788 2021-04-07 06:11:45.000000 DbtPy-3.0.5.4/WIKI.md
--rw-rw-rw-   0 root         (0) root         (0)   431196 2022-02-11 07:49:15.000000 DbtPy-3.0.5.4/dbtpyc.c
--rw-rw-rw-   0 root         (0) root         (0)    26324 2021-04-07 06:16:44.000000 DbtPy-3.0.5.4/dbtpyc.h
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-06-09 02:53:35.000000 DbtPy-3.0.5.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     9100 2022-04-12 12:25:14.000000 DbtPy-3.0.5.4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     3960 2021-04-07 06:18:42.000000 DbtPy-3.0.5.4/testfunctions.py
--rw-rw-rw-   0 root         (0) root         (0)     2528 2021-04-07 06:20:10.000000 DbtPy-3.0.5.4/tests.py
--rw-r--r--   0 root         (0) root         (0)     1380 2022-06-09 02:53:35.000000 DbtPy-3.0.5.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 05:30:59.000000 DbtPy-3.0.5.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 05:30:59.000000 DbtPy-3.0.5.5/DbtPy.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     5463 2023-05-12 05:30:59.000000 DbtPy-3.0.5.5/DbtPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-12 05:30:59.000000 DbtPy-3.0.5.5/DbtPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-12 05:30:59.000000 DbtPy-3.0.5.5/DbtPy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2023-05-12 05:30:59.000000 DbtPy-3.0.5.5/DbtPy.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    26324 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/dbtpyc.h
+-rw-rw-rw-   0 root         (0) root         (0)     3960 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/testfunctions.py
+-rw-r--r--   0 root         (0) root         (0)      322 2023-05-12 03:00:57.000000 DbtPy-3.0.5.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 05:30:59.000000 DbtPy-3.0.5.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_310_ClientInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_033_ResultOutSequenceColumn.py
+-rw-rw-rw-   0 root         (0) root         (0)     7683 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_156_FetchAssocNestedSelects_01.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_211_FieldDisplaySize_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_316_UDT_Param.py
+-rw-rw-rw-   0 root         (0) root         (0)     1784 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/xtest_018_selectRowcountPrefetchSetOpt.py
+-rw-rw-rw-   0 root         (0) root         (0)    29172 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_000_PrepareDb.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_212_FieldDisplaySize_03.py
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_6755_ExtraNULLChar_ResultCLOBCol.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_030_Result.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_048_FetchTupleBinaryData_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     2359 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_314_Collection_Param.py
+-rw-rw-rw-   0 root         (0) root         (0)     4699 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_159_FetchAssocSeveralRows_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_122_FieldNameDiffCaseColNames.py
+-rw-rw-rw-   0 root         (0) root         (0)     6316 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_162_FetchBothNestedSelects_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     2184 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_008_ColumnInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2132 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_115_NumericTest_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     8924 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_039_FetchRowIndexPosNested_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     1937 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_021_CommitDelete.py
+-rw-rw-rw-   0 root         (0) root         (0)     1952 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_148_CallSPDiffBindPattern_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_142_BindParamSelectStmtMultipleParams_02.py
+-rw-rw-rw-   0 root         (0) root         (0)   163950 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_123_FieldNamePos_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_060_Tables_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     2750 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_153_FetchAssocSelect_04.py
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_110_FieldNum.py
+-rw-rw-rw-   0 root         (0) root         (0)     8174 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_154_AllFetches.py
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/xtest_013_KeysetDrivenCursorSelect02.py
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_232_FieldTypePosName.py
+-rw-rw-rw-   0 root         (0) root         (0)     1920 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_061_Tables_02.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_052_SetAutocommit_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_6528_ScopingProblemBindParam.py
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_120_FieldName.py
+-rw-rw-rw-   0 root         (0) root         (0)     2229 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_121_FieldNameAddCol.py
+-rw-rw-rw-   0 root         (0) root         (0)     1514 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_315_UDT.py
+-rw-rw-rw-   0 root         (0) root         (0)     2295 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_157b_FetchAssocScrollableCursor_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_141_BindParamSelectStmtMultipleParams_01.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_045_FetchTupleBinaryData_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/spook.png
+-rw-rw-rw-   0 root         (0) root         (0)     2014 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_SmartTrigger.py
+-rw-rw-rw-   0 root         (0) root         (0)    16367 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_037_FetchRowIndexPos.py
+-rw-rw-rw-   0 root         (0) root         (0)    16581 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_038_FetchRowIndexPosNested_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/pic1.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    19143 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_160_FetchBoth.py
+-rw-rw-rw-   0 root         (0) root         (0)     1891 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_180_StmtErrMsg.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_157_FetchAssocScrollableCursor_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     1863 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_313_Collection.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_092_ConnmsgWrongPwd.py
+-rw-rw-rw-   0 root         (0) root         (0)     6371 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_265_NoAffectedRows.py
+-rw-rw-rw-   0 root         (0) root         (0)     4587 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_300_ServerInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_03a_ResultNonExistCol.py
+-rw-rw-rw-   0 root         (0) root         (0)    10656 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_150_FetchAssocSelect_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_6792_FieldTypeRetStrDatetimeTimestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2914 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_311_InsertSelectDeleteNumLiterals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1695 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_125_FieldNamePos_03.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_131_PrepareExecuteSelectStatementParams.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_034_FetchAssoc.py
+-rw-rw-rw-   0 root         (0) root         (0)      787 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_251_FreeResult_02.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_070_Close.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_016_InsertDeleteRowCount_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_101_InsertDeleteFieldCount.py
+-rw-rw-rw-   0 root         (0) root         (0)     1971 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_231_FieldTypeName.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_InsertRetrieveDateTimeTypeColumn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_132_ExecuteStatementArrayMultipleParams.py
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_157a_FetchAssocWithoutScrollableCursorErr.py
+-rw-rw-rw-   0 root         (0) root         (0)     3844 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/xtest_053_AttrThruConn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1334 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/xtest_012_KeysetDrivenCursorSelect01.py
+-rw-rw-rw-   0 root         (0) root         (0)     3116 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_159a_FetchAssocSeveralRows_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_025_PrimaryKeys.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_240_FieldWidthPosName_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_230_FieldTypePos.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_200_MultipleRsltsetsUniformColDefs.py
+-rw-rw-rw-   0 root         (0) root         (0)    28312 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_036_FetchRow_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     1281 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_040_FetchTuple.py
+-rw-rw-rw-   0 root         (0) root         (0)     9158 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_151_FetchAssocSelect_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_213_FieldDisplaySize_04.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_022_RollbackInsert.py
+-rw-rw-rw-   0 root         (0) root         (0)     1928 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_133_ExecuteLongInputParams.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_312_CacheBoundParameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1125 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_147_PrepareWithWrongType.py
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_140_BindParamSelectStmt.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_004_ConnWrongUserPwd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_049_InsertNoneParam.py
+-rw-rw-rw-   0 root         (0) root         (0)    17097 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_124_FieldNamePos_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_210_FieldDisplaySize_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     3281 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_066_TableObjects.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_190_ColumnsTable_01.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_082_ConnWrongPwd.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_003_NumAffectedRows.py
+-rw-rw-rw-   0 root         (0) root         (0)     7743 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_152_FetchAssocSelect_03.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_010_UpdateRowCount.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_146_CallSPINAndOUTParams.py
+-rw-rw-rw-   0 root         (0) root         (0)     1218 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_054_CursorType.py
+-rw-rw-rw-   0 root         (0) root         (0)     1850 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_065_FilterTableName.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_191_ColumnsTable_02.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_130_PrepExecuteSelectStmt.py
+-rw-rw-rw-   0 root         (0) root         (0)    17678 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_155_FetchAssocSelect_05.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_114_NumericTest_01.py
+-rw-rw-rw-   0 root         (0) root         (0)      871 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_011_DeleteRowCount.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_081_ConnWrongUser.py
+-rw-rw-rw-   0 root         (0) root         (0)     6083 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_161_FetchBothNestedSelects_01.py
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_005_ConnBadUserBadPwd.py
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_197_StatisticsIndexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_143_BindParamInsertStmtNoneParam.py
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_261_FetchObjectAccess.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_051_SetAutocommit_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_6561_InsertNULLValues.py
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_015_InsertDeleteRowCount_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/xtest_014_KeysetDrivenCursorNegativeRow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_145_BindRetrieveNoneEmptyString.py
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_spinout_timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_032_ResultIndexName.py
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_111_FieldNumAddCol.py
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_020_RollbackDelete.py
+-rw-rw-rw-   0 root         (0) root         (0)     2662 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_264_InsertRetrieveBIGINTTypeColumn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_201_MultipleRsltsetsDiffColDefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_144_BindParamInsertStmtPARAM_FILE.py
+-rw-rw-rw-   0 root         (0) root         (0)     6711 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_158_FetchAssocNestedSelects_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     2005 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_103_NumFieldsSelect_02.py
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_001_ConnDb.py
+-rw-rw-rw-   0 root         (0) root         (0)      601 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_063_Tables_04.py
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_050_AutocommitStatus.py
+-rw-rw-rw-   0 root         (0) root         (0)      566 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_091_ConnmsgWrongUser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_006_ConnPassingOpts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_064_Tables_05.py
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_031_ResultIndexPosition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_116_ConnActive.py
+-rw-rw-rw-   0 root         (0) root         (0)      956 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_071_CloseSuccess.py
+-rw-rw-rw-   0 root         (0) root         (0)     1464 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_035_FetchRow_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_023_ColumnPrivileges.py
+-rw-rw-rw-   0 root         (0) root         (0)     3181 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_decimal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_100_SelectDeleteInsertFieldCount.py
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_062_Tables_03.py
+-rw-rw-rw-   0 root         (0) root         (0)     1028 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/xtest_019_selectRowcountPrefetchPrepOpt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 05:30:59.000000 DbtPy-3.0.5.5/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/data/data1.txt
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/data/data2.txt
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/data/data3.txt
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/data/data4.txt
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/data/test_6755.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_241_FieldWidthPosName_02.py
+-rw-rw-rw-   0 root         (0) root         (0)     3261 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_024_ForeignKeys.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_112_FieldNumDiffCaseColNames.py
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_113_DateTest.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_102_NumFieldsSelect_01.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_warn.py
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests/test_250_FreeResult_01.py
+-rw-r--r--   0 root         (0) root         (0)    42788 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/WIKI.md
+-rw-rw-rw-   0 root         (0) root         (0)     2528 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/tests.py
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)    56905 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/DbtPyDbi.py
+-rw-rw-rw-   0 root         (0) root         (0)   431196 2023-05-12 02:56:58.000000 DbtPy-3.0.5.5/dbtpyc.c
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-05-12 05:30:59.000000 DbtPy-3.0.5.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-12 05:30:59.000000 DbtPy-3.0.5.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     9221 2023-05-12 05:30:17.000000 DbtPy-3.0.5.5/setup.py
```

### Comparing `DbtPy-3.0.5.4/DbtPy.egg-info/PKG-INFO` & `DbtPy-3.0.5.5/DbtPy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,15 @@
 Metadata-Version: 2.1
 Name: DbtPy
-Version: 3.0.5.4
+Version: 3.0.5.5
 Summary: GBase 8s native Python driver
 Home-page: https://gbasedbt.com/DbtPy
 Author: Informix Application Development Team & GBase 8s Support Team
+Author-email: dbt@gbasedbt.com
 License: Apache License 2.0
-Description: ### 更新记录  
-        3.0.5.4  
-        ----  
-        1，更新文档说明；  
-        2，去除下载ssl验证；  
-        
-        3.0.5.3  
-        ----  
-        1，支持bigint和bigserial字段类型；  
-        
-        3.0.5  
-        ----  
-        1，Fork from IfxPy 3.0.5  
-        
-        ### 限制  
-        1，大对象支持（text/byte/clob/blob）；  
-        
-        
 Keywords: GBase 8s Python Enterprise
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
@@ -35,7 +18,31 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: ~=3.4
 Description-Content-Type: text/markdown
+
+### 更新记录  
+3.0.5.5
+----
+1，增加aarch64的ODBC下载地址；
+
+3.0.5.4  
+----  
+1，更新文档说明；  
+2，去除下载ssl验证；  
+
+3.0.5.3  
+----  
+1，支持bigint和bigserial字段类型；  
+
+3.0.5  
+----  
+1，Fork from IfxPy 3.0.5  
+
+### 限制  
+1，大对象支持（text/byte/clob/blob）；  
+
+
+
```

### Comparing `DbtPy-3.0.5.4/DbtPy.egg-info/SOURCES.txt` & `DbtPy-3.0.5.5/DbtPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/pic1.jpg` & `DbtPy-3.0.5.5/tests/pic1.jpg`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/spook.png` & `DbtPy-3.0.5.5/tests/spook.png`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_000_PrepareDb.py` & `DbtPy-3.0.5.5/tests/test_000_PrepareDb.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_001_ConnDb.py` & `DbtPy-3.0.5.5/tests/test_001_ConnDb.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_003_NumAffectedRows.py` & `DbtPy-3.0.5.5/tests/test_003_NumAffectedRows.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_004_ConnWrongUserPwd.py` & `DbtPy-3.0.5.5/tests/test_004_ConnWrongUserPwd.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_005_ConnBadUserBadPwd.py` & `DbtPy-3.0.5.5/tests/test_005_ConnBadUserBadPwd.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_006_ConnPassingOpts.py` & `DbtPy-3.0.5.5/tests/test_006_ConnPassingOpts.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_008_ColumnInfo.py` & `DbtPy-3.0.5.5/tests/test_008_ColumnInfo.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_010_UpdateRowCount.py` & `DbtPy-3.0.5.5/tests/test_010_UpdateRowCount.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_011_DeleteRowCount.py` & `DbtPy-3.0.5.5/tests/test_011_DeleteRowCount.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_015_InsertDeleteRowCount_01.py` & `DbtPy-3.0.5.5/tests/test_015_InsertDeleteRowCount_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_016_InsertDeleteRowCount_02.py` & `DbtPy-3.0.5.5/tests/test_016_InsertDeleteRowCount_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_020_RollbackDelete.py` & `DbtPy-3.0.5.5/tests/test_020_RollbackDelete.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_021_CommitDelete.py` & `DbtPy-3.0.5.5/tests/test_021_CommitDelete.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_022_RollbackInsert.py` & `DbtPy-3.0.5.5/tests/test_022_RollbackInsert.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_023_ColumnPrivileges.py` & `DbtPy-3.0.5.5/tests/test_023_ColumnPrivileges.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_024_ForeignKeys.py` & `DbtPy-3.0.5.5/tests/test_024_ForeignKeys.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_025_PrimaryKeys.py` & `DbtPy-3.0.5.5/tests/test_025_PrimaryKeys.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_030_Result.py` & `DbtPy-3.0.5.5/tests/test_030_Result.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_031_ResultIndexPosition.py` & `DbtPy-3.0.5.5/tests/test_031_ResultIndexPosition.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_032_ResultIndexName.py` & `DbtPy-3.0.5.5/tests/test_032_ResultIndexName.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_033_ResultOutSequenceColumn.py` & `DbtPy-3.0.5.5/tests/test_033_ResultOutSequenceColumn.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_034_FetchAssoc.py` & `DbtPy-3.0.5.5/tests/test_034_FetchAssoc.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_035_FetchRow_01.py` & `DbtPy-3.0.5.5/tests/test_035_FetchRow_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_036_FetchRow_02.py` & `DbtPy-3.0.5.5/tests/test_036_FetchRow_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_037_FetchRowIndexPos.py` & `DbtPy-3.0.5.5/tests/test_037_FetchRowIndexPos.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_038_FetchRowIndexPosNested_01.py` & `DbtPy-3.0.5.5/tests/test_038_FetchRowIndexPosNested_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_039_FetchRowIndexPosNested_02.py` & `DbtPy-3.0.5.5/tests/test_039_FetchRowIndexPosNested_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_03a_ResultNonExistCol.py` & `DbtPy-3.0.5.5/tests/test_03a_ResultNonExistCol.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_040_FetchTuple.py` & `DbtPy-3.0.5.5/tests/test_040_FetchTuple.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_045_FetchTupleBinaryData_01.py` & `DbtPy-3.0.5.5/tests/test_045_FetchTupleBinaryData_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_048_FetchTupleBinaryData_02.py` & `DbtPy-3.0.5.5/tests/test_048_FetchTupleBinaryData_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_049_InsertNoneParam.py` & `DbtPy-3.0.5.5/tests/test_049_InsertNoneParam.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_051_SetAutocommit_01.py` & `DbtPy-3.0.5.5/tests/test_051_SetAutocommit_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_052_SetAutocommit_02.py` & `DbtPy-3.0.5.5/tests/test_052_SetAutocommit_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_054_CursorType.py` & `DbtPy-3.0.5.5/tests/test_054_CursorType.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_060_Tables_01.py` & `DbtPy-3.0.5.5/tests/test_060_Tables_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_061_Tables_02.py` & `DbtPy-3.0.5.5/tests/test_061_Tables_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_062_Tables_03.py` & `DbtPy-3.0.5.5/tests/test_062_Tables_03.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_063_Tables_04.py` & `DbtPy-3.0.5.5/tests/test_063_Tables_04.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_064_Tables_05.py` & `DbtPy-3.0.5.5/tests/test_064_Tables_05.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_065_FilterTableName.py` & `DbtPy-3.0.5.5/tests/test_065_FilterTableName.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_066_TableObjects.py` & `DbtPy-3.0.5.5/tests/test_066_TableObjects.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_070_Close.py` & `DbtPy-3.0.5.5/tests/test_070_Close.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_071_CloseSuccess.py` & `DbtPy-3.0.5.5/tests/test_071_CloseSuccess.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_081_ConnWrongUser.py` & `DbtPy-3.0.5.5/tests/test_081_ConnWrongUser.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_091_ConnmsgWrongUser.py` & `DbtPy-3.0.5.5/tests/test_091_ConnmsgWrongUser.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_092_ConnmsgWrongPwd.py` & `DbtPy-3.0.5.5/tests/test_092_ConnmsgWrongPwd.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_100_SelectDeleteInsertFieldCount.py` & `DbtPy-3.0.5.5/tests/test_100_SelectDeleteInsertFieldCount.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_101_InsertDeleteFieldCount.py` & `DbtPy-3.0.5.5/tests/test_101_InsertDeleteFieldCount.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_102_NumFieldsSelect_01.py` & `DbtPy-3.0.5.5/tests/test_102_NumFieldsSelect_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_103_NumFieldsSelect_02.py` & `DbtPy-3.0.5.5/tests/test_103_NumFieldsSelect_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_110_FieldNum.py` & `DbtPy-3.0.5.5/tests/test_110_FieldNum.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_111_FieldNumAddCol.py` & `DbtPy-3.0.5.5/tests/test_111_FieldNumAddCol.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_112_FieldNumDiffCaseColNames.py` & `DbtPy-3.0.5.5/tests/test_112_FieldNumDiffCaseColNames.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_113_DateTest.py` & `DbtPy-3.0.5.5/tests/test_113_DateTest.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_114_NumericTest_01.py` & `DbtPy-3.0.5.5/tests/test_114_NumericTest_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_115_NumericTest_02.py` & `DbtPy-3.0.5.5/tests/test_115_NumericTest_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_116_ConnActive.py` & `DbtPy-3.0.5.5/tests/test_116_ConnActive.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_120_FieldName.py` & `DbtPy-3.0.5.5/tests/test_120_FieldName.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_121_FieldNameAddCol.py` & `DbtPy-3.0.5.5/tests/test_121_FieldNameAddCol.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_122_FieldNameDiffCaseColNames.py` & `DbtPy-3.0.5.5/tests/test_122_FieldNameDiffCaseColNames.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_123_FieldNamePos_01.py` & `DbtPy-3.0.5.5/tests/test_123_FieldNamePos_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_124_FieldNamePos_02.py` & `DbtPy-3.0.5.5/tests/test_124_FieldNamePos_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_125_FieldNamePos_03.py` & `DbtPy-3.0.5.5/tests/test_125_FieldNamePos_03.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_130_PrepExecuteSelectStmt.py` & `DbtPy-3.0.5.5/tests/test_130_PrepExecuteSelectStmt.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_131_PrepareExecuteSelectStatementParams.py` & `DbtPy-3.0.5.5/tests/test_131_PrepareExecuteSelectStatementParams.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_132_ExecuteStatementArrayMultipleParams.py` & `DbtPy-3.0.5.5/tests/test_132_ExecuteStatementArrayMultipleParams.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_133_ExecuteLongInputParams.py` & `DbtPy-3.0.5.5/tests/test_133_ExecuteLongInputParams.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_140_BindParamSelectStmt.py` & `DbtPy-3.0.5.5/tests/test_140_BindParamSelectStmt.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_141_BindParamSelectStmtMultipleParams_01.py` & `DbtPy-3.0.5.5/tests/test_141_BindParamSelectStmtMultipleParams_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_142_BindParamSelectStmtMultipleParams_02.py` & `DbtPy-3.0.5.5/tests/test_142_BindParamSelectStmtMultipleParams_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_143_BindParamInsertStmtNoneParam.py` & `DbtPy-3.0.5.5/tests/test_143_BindParamInsertStmtNoneParam.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_144_BindParamInsertStmtPARAM_FILE.py` & `DbtPy-3.0.5.5/tests/test_144_BindParamInsertStmtPARAM_FILE.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_145_BindRetrieveNoneEmptyString.py` & `DbtPy-3.0.5.5/tests/test_145_BindRetrieveNoneEmptyString.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_146_CallSPINAndOUTParams.py` & `DbtPy-3.0.5.5/tests/test_146_CallSPINAndOUTParams.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_147_PrepareWithWrongType.py` & `DbtPy-3.0.5.5/tests/test_147_PrepareWithWrongType.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_148_CallSPDiffBindPattern_01.py` & `DbtPy-3.0.5.5/tests/test_148_CallSPDiffBindPattern_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_150_FetchAssocSelect_01.py` & `DbtPy-3.0.5.5/tests/test_150_FetchAssocSelect_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_151_FetchAssocSelect_02.py` & `DbtPy-3.0.5.5/tests/test_151_FetchAssocSelect_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_152_FetchAssocSelect_03.py` & `DbtPy-3.0.5.5/tests/test_152_FetchAssocSelect_03.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_153_FetchAssocSelect_04.py` & `DbtPy-3.0.5.5/tests/test_153_FetchAssocSelect_04.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_154_AllFetches.py` & `DbtPy-3.0.5.5/tests/test_154_AllFetches.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_155_FetchAssocSelect_05.py` & `DbtPy-3.0.5.5/tests/test_155_FetchAssocSelect_05.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_156_FetchAssocNestedSelects_01.py` & `DbtPy-3.0.5.5/tests/test_156_FetchAssocNestedSelects_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_157_FetchAssocScrollableCursor_01.py` & `DbtPy-3.0.5.5/tests/test_157_FetchAssocScrollableCursor_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_159_FetchAssocSeveralRows_01.py` & `DbtPy-3.0.5.5/tests/test_159_FetchAssocSeveralRows_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_157a_FetchAssocWithoutScrollableCursorErr.py` & `DbtPy-3.0.5.5/tests/test_157a_FetchAssocWithoutScrollableCursorErr.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_157b_FetchAssocScrollableCursor_02.py` & `DbtPy-3.0.5.5/tests/test_157b_FetchAssocScrollableCursor_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_158_FetchAssocNestedSelects_02.py` & `DbtPy-3.0.5.5/tests/test_158_FetchAssocNestedSelects_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_159a_FetchAssocSeveralRows_02.py` & `DbtPy-3.0.5.5/tests/test_159a_FetchAssocSeveralRows_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_160_FetchBoth.py` & `DbtPy-3.0.5.5/tests/test_160_FetchBoth.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_161_FetchBothNestedSelects_01.py` & `DbtPy-3.0.5.5/tests/test_161_FetchBothNestedSelects_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_162_FetchBothNestedSelects_02.py` & `DbtPy-3.0.5.5/tests/test_162_FetchBothNestedSelects_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_180_StmtErrMsg.py` & `DbtPy-3.0.5.5/tests/test_180_StmtErrMsg.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_190_ColumnsTable_01.py` & `DbtPy-3.0.5.5/tests/test_190_ColumnsTable_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_191_ColumnsTable_02.py` & `DbtPy-3.0.5.5/tests/test_191_ColumnsTable_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_197_StatisticsIndexes.py` & `DbtPy-3.0.5.5/tests/test_197_StatisticsIndexes.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_200_MultipleRsltsetsUniformColDefs.py` & `DbtPy-3.0.5.5/tests/test_200_MultipleRsltsetsUniformColDefs.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_201_MultipleRsltsetsDiffColDefs.py` & `DbtPy-3.0.5.5/tests/test_201_MultipleRsltsetsDiffColDefs.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_210_FieldDisplaySize_01.py` & `DbtPy-3.0.5.5/tests/test_210_FieldDisplaySize_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_211_FieldDisplaySize_02.py` & `DbtPy-3.0.5.5/tests/test_211_FieldDisplaySize_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_212_FieldDisplaySize_03.py` & `DbtPy-3.0.5.5/tests/test_212_FieldDisplaySize_03.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_213_FieldDisplaySize_04.py` & `DbtPy-3.0.5.5/tests/test_213_FieldDisplaySize_04.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_230_FieldTypePos.py` & `DbtPy-3.0.5.5/tests/test_230_FieldTypePos.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_231_FieldTypeName.py` & `DbtPy-3.0.5.5/tests/test_231_FieldTypeName.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_232_FieldTypePosName.py` & `DbtPy-3.0.5.5/tests/test_232_FieldTypePosName.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_240_FieldWidthPosName_01.py` & `DbtPy-3.0.5.5/tests/test_240_FieldWidthPosName_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_241_FieldWidthPosName_02.py` & `DbtPy-3.0.5.5/tests/test_241_FieldWidthPosName_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_250_FreeResult_01.py` & `DbtPy-3.0.5.5/tests/test_250_FreeResult_01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_251_FreeResult_02.py` & `DbtPy-3.0.5.5/tests/test_251_FreeResult_02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_261_FetchObjectAccess.py` & `DbtPy-3.0.5.5/tests/test_261_FetchObjectAccess.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_264_InsertRetrieveBIGINTTypeColumn.py` & `DbtPy-3.0.5.5/tests/test_264_InsertRetrieveBIGINTTypeColumn.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_265_NoAffectedRows.py` & `DbtPy-3.0.5.5/tests/test_265_NoAffectedRows.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_300_ServerInfo.py` & `DbtPy-3.0.5.5/tests/test_300_ServerInfo.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_310_ClientInfo.py` & `DbtPy-3.0.5.5/tests/test_310_ClientInfo.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_311_InsertSelectDeleteNumLiterals.py` & `DbtPy-3.0.5.5/tests/test_311_InsertSelectDeleteNumLiterals.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_312_CacheBoundParameters.py` & `DbtPy-3.0.5.5/tests/test_312_CacheBoundParameters.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_313_Collection.py` & `DbtPy-3.0.5.5/tests/test_313_Collection.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_314_Collection_Param.py` & `DbtPy-3.0.5.5/tests/test_314_Collection_Param.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_315_UDT.py` & `DbtPy-3.0.5.5/tests/test_315_UDT.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_316_UDT_Param.py` & `DbtPy-3.0.5.5/tests/test_316_UDT_Param.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_6528_ScopingProblemBindParam.py` & `DbtPy-3.0.5.5/tests/test_6528_ScopingProblemBindParam.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_6561_InsertNULLValues.py` & `DbtPy-3.0.5.5/tests/test_6561_InsertNULLValues.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_6755_ExtraNULLChar_ResultCLOBCol.py` & `DbtPy-3.0.5.5/tests/test_6755_ExtraNULLChar_ResultCLOBCol.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_6792_FieldTypeRetStrDatetimeTimestamp.py` & `DbtPy-3.0.5.5/tests/test_6792_FieldTypeRetStrDatetimeTimestamp.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_InsertRetrieveDateTimeTypeColumn.py` & `DbtPy-3.0.5.5/tests/test_InsertRetrieveDateTimeTypeColumn.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_SmartTrigger.py` & `DbtPy-3.0.5.5/tests/test_SmartTrigger.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_decimal.py` & `DbtPy-3.0.5.5/tests/test_decimal.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_spinout_timestamp.py` & `DbtPy-3.0.5.5/tests/test_spinout_timestamp.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/test_warn.py` & `DbtPy-3.0.5.5/tests/test_warn.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/xtest_012_KeysetDrivenCursorSelect01.py` & `DbtPy-3.0.5.5/tests/xtest_012_KeysetDrivenCursorSelect01.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/xtest_013_KeysetDrivenCursorSelect02.py` & `DbtPy-3.0.5.5/tests/xtest_013_KeysetDrivenCursorSelect02.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/xtest_014_KeysetDrivenCursorNegativeRow.py` & `DbtPy-3.0.5.5/tests/xtest_014_KeysetDrivenCursorNegativeRow.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/xtest_018_selectRowcountPrefetchSetOpt.py` & `DbtPy-3.0.5.5/tests/xtest_018_selectRowcountPrefetchSetOpt.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/xtest_019_selectRowcountPrefetchPrepOpt.py` & `DbtPy-3.0.5.5/tests/xtest_019_selectRowcountPrefetchPrepOpt.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests/xtest_053_AttrThruConn.py` & `DbtPy-3.0.5.5/tests/xtest_053_AttrThruConn.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/DbtPyDbi.py` & `DbtPy-3.0.5.5/DbtPyDbi.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/WIKI.md` & `DbtPy-3.0.5.5/WIKI.md`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/dbtpyc.c` & `DbtPy-3.0.5.5/dbtpyc.c`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/dbtpyc.h` & `DbtPy-3.0.5.5/dbtpyc.h`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/setup.py` & `DbtPy-3.0.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     long_desc = f.read()
 
 # Writing the Setup Script
 # https://docs.python.org/3.4/distutils/setupscript.html#distutils-installing-scripts
 
 
 PACKAGE   = 'DbtPy'
-VERSION   = '3.0.5.4'
+VERSION   = '3.0.5.5'
 VERSION2X = '2.7.1'
 LICENSE   = 'Apache License 2.0'
 DbtPyLongDescription='GBase 8s native Python driver is a high performing data access interface suitable for highly scalable enterprise with GBase 8s database.'
 
 # Python 3.4 and up and not commit to Python 4 support yet
 PYTHON_REQ = '~=3.4'
 
@@ -72,15 +72,19 @@
 	
 if('win32' in sys.platform):
 	os_ = 'win'
 	cliFileName = 'GBase8s_3.0-Win64-ODBC-Driver.zip'
 	prefix = 'build/lib.win-amd64-' + str(sys.version_info[0])+"."+str(sys.version_info[1]) + '/'
 elif ('linux' in sys.platform):
 	os_ = 'linux'
-	cliFileName = 'GBase8s_3.0-Linux64-ODBC-Driver.tar.gz'
+	if(platform.machine() in ('aarch64','arm64')):
+		cliFileName = 'GBase8s_3.0-Aarch64-ODBC-Driver.tar.gz'        
+	else:
+		cliFileName = 'GBase8s_3.0-Linux64-ODBC-Driver.tar.gz'
+
 	prefix = 'build/lib.linux-'+ platform.processor() + '-' + str(sys.version_info[0])+"."+str(sys.version_info[1]) + '/'
 else:
 	cliFileName = 'Unknown'
 
 gbasedbtdir = os.getenv('GBASEDBTDIR', '')
 csdk_home = os.getenv('CSDK_HOME', '')
 
@@ -210,15 +214,15 @@
        #    'Documentation': 'https://gbasedbt.com/DbtPy/wiki/',
        #    'Source': 'https://gbasedbt.com/DbtPy/',
        #    'Tracker': 'https://gbasedbt.com/DbtPy/',
        #},
        python_requires = PYTHON_REQ,
 
        author          = 'Informix Application Development Team & GBase 8s Support Team',
-       #author_email    = 'dbt@gbasedbt.com',
+       author_email    = 'dbt@gbasedbt.com',
 
        # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
        classifiers=[
            # How mature is this project? Common values are
            #   3 - Alpha
            #   4 - Beta
            #   5 - Production/Stable
```

### Comparing `DbtPy-3.0.5.4/testfunctions.py` & `DbtPy-3.0.5.5/testfunctions.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/tests.py` & `DbtPy-3.0.5.5/tests.py`

 * *Files identical despite different names*

### Comparing `DbtPy-3.0.5.4/PKG-INFO` & `DbtPy-3.0.5.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,15 @@
 Metadata-Version: 2.1
 Name: DbtPy
-Version: 3.0.5.4
+Version: 3.0.5.5
 Summary: GBase 8s native Python driver
 Home-page: https://gbasedbt.com/DbtPy
 Author: Informix Application Development Team & GBase 8s Support Team
+Author-email: dbt@gbasedbt.com
 License: Apache License 2.0
-Description: ### 更新记录  
-        3.0.5.4  
-        ----  
-        1，更新文档说明；  
-        2，去除下载ssl验证；  
-        
-        3.0.5.3  
-        ----  
-        1，支持bigint和bigserial字段类型；  
-        
-        3.0.5  
-        ----  
-        1，Fork from IfxPy 3.0.5  
-        
-        ### 限制  
-        1，大对象支持（text/byte/clob/blob）；  
-        
-        
 Keywords: GBase 8s Python Enterprise
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
@@ -35,7 +18,31 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: ~=3.4
 Description-Content-Type: text/markdown
+
+### 更新记录  
+3.0.5.5
+----
+1，增加aarch64的ODBC下载地址；
+
+3.0.5.4  
+----  
+1，更新文档说明；  
+2，去除下载ssl验证；  
+
+3.0.5.3  
+----  
+1，支持bigint和bigserial字段类型；  
+
+3.0.5  
+----  
+1，Fork from IfxPy 3.0.5  
+
+### 限制  
+1，大对象支持（text/byte/clob/blob）；  
+
+
+
```

