# Comparing `tmp/histcite-python-0.1.5.tar.gz` & `tmp/histcite-python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-0.1.5.tar", last modified: Fri May  5 05:51:03 2023, max compression
+gzip compressed data, was "histcite-python-0.2.0.tar", last modified: Fri May 12 07:25:54 2023, max compression
```

## Comparing `histcite-python-0.1.5.tar` & `histcite-python-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:51:03.588145 histcite-python-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-05 05:50:52.000000 histcite-python-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-05 05:51:03.588145 histcite-python-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-05 05:50:52.000000 histcite-python-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:51:03.584145 histcite-python-0.1.5/histcite/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 05:50:52.000000 histcite-python-0.1.5/histcite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-05 05:50:52.000000 histcite-python-0.1.5/histcite/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-05 05:50:52.000000 histcite-python-0.1.5/histcite/compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-05 05:50:52.000000 histcite-python-0.1.5/histcite/network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-05 05:50:52.000000 histcite-python-0.1.5/histcite/parse_citation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-05 05:50:52.000000 histcite-python-0.1.5/histcite/process_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:51:03.588145 histcite-python-0.1.5/histcite_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-05 05:51:03.000000 histcite-python-0.1.5/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-05 05:51:03.000000 histcite-python-0.1.5/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:51:03.000000 histcite-python-0.1.5/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 05:51:03.000000 histcite-python-0.1.5/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 05:51:03.000000 histcite-python-0.1.5/histcite_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 05:51:03.000000 histcite-python-0.1.5/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:51:03.588145 histcite-python-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-05 05:50:52.000000 histcite-python-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:51:03.588145 histcite-python-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-05 05:50:52.000000 histcite-python-0.1.5/tests/test_compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-05 05:50:52.000000 histcite-python-0.1.5/tests/test_network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-05 05:50:52.000000 histcite-python-0.1.5/tests/test_parse_citation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:25:54.777446 histcite-python-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 07:25:37.000000 histcite-python-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-05-12 07:25:54.777446 histcite-python-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-05-12 07:25:37.000000 histcite-python-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:25:54.773446 histcite-python-0.2.0/histcite/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/parse_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/recognize_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:25:54.773446 histcite-python-0.2.0/histcite_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-05-12 07:25:54.000000 histcite-python-0.2.0/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-12 07:25:54.000000 histcite-python-0.2.0/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:25:54.000000 histcite-python-0.2.0/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 07:25:54.000000 histcite-python-0.2.0/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 07:25:54.000000 histcite-python-0.2.0/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 07:25:54.000000 histcite-python-0.2.0/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 07:25:54.777446 histcite-python-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-12 07:25:37.000000 histcite-python-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:25:54.777446 histcite-python-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-12 07:25:37.000000 histcite-python-0.2.0/tests/test_compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-12 07:25:37.000000 histcite-python-0.2.0/tests/test_network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-12 07:25:37.000000 histcite-python-0.2.0/tests/test_parse_reference.py
```

### Comparing `histcite-python-0.1.5/LICENSE` & `histcite-python-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.5/PKG-INFO` & `histcite-python-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.1.5
+Version: 0.2.0
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -19,50 +19,60 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，并且可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为国科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
+
+最近更新：
+- `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持，并对调用方式进行调整；
 
 核心功能：
 - 生成引文网络图；
-- 生成包含文献、作者、机构、期刊、关键词等分析单元的引文统计数据；  
+- 生成包含文献、作者、机构、期刊、关键词等分析单元的统计数据；  
 
-## 术语说明
+术语说明：
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
 - `LCS`, Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如`TLCS` = 总本地引文分数；
 - `Recs`， 记录数；
-- Web of science题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
+- `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
+- 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
 
 ## 快速开始
-> 适用于本工具的数据集，来源Web of Science核心合集，<b> Tab delimited file/制表符分隔文件</b> 格式，导出内容选择 <b>Full Record and Cited References/全记录与引用的参考文献</b> 或者是 <b>Custome selection/自定义选择项</b>，全选字段，下载之后不要修改文件名，放在某个文件夹内；  
 ```console
 # 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
+## 数据准备
+| 数据来源 | 下载说明 |
+| :---: | --- |
+| `Web of Science` | 核心合集，格式选择 Tab delimited file/制表符分隔文件，导出内容选择 Full Record and Cited References/全记录与引用的参考文献 或者是 Custome selection/自定义选择项，全选字段 |
+| `CSSCI` | 从CSSCI数据库正常导出即可 |
+> 注：文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹下。
+
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
+| -t | --source_type | 题录数据来源，可选 `wos` 或 `cssci`，必须指定 |
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
-| -g | --graph | 是否仅生成图文件，指定该参数表示 `True`, 无需传值 |
+| -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
 
 ```console
-$ 假设下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数设置为 100
-$ histcite -f /Users/.../downloads/dataset -n 100
+$ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
+$ histcite -f /Users/.../downloads/dataset -t wos -n 100
 ```
-
-> 结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot` 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。 
+> 结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
 
 生成的引文网络图：
 
 <img src="examples/graph.svg">
 
 对应的文献节点信息：
 
@@ -76,54 +86,61 @@
 |    ...    |               |      |                                                  |      |      |
 
 2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
 
 ```python
 import os
 import pandas as pd
-from histcite.process_table import ParseTable
+from histcite.process_file import ProcessFile
 from histcite.compute_metrics import ComputeMetrics
-from histcite.network_graph import Graphviz
+from histcite.network_graph import GraphViz
 
 # 读取数据，解析引文
 folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
-process = ProcessTable(folder_path)
+source_type = 'wos'
+process = ProcessFile(folder_path, source_type)
 process.concat_table() # 合并多个文件
 process.process_citation() # 识别引文关系
 docs_table = process.docs_table
 reference_table = process.reference_table
 
 # 基本描述统计
-cm = ComputeMetrics(docs_table, reference_table)
+cm = ComputeMetrics(docs_table, reference_table, source_type)
 cm.write2excel(os.path.join(folder_path,'result','statistics.xlsx'))
 
 # 生成引文网络图文件
-graph = Graphviz(docs_table)
+graph = GraphViz(docs_table, source_type)
 doc_indices = docs_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
 graph_dot_file = graph.generate_dot_file(doc_indices, allow_external_node=False)
 
 # 保存引文网络图文件
 with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
-    f.write(dot_text)
+    f.write(graph_dot_file)
 
 # 保存引文网络图节点文件
 graph_node_file = graph.generate_graph_node_file()
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
-> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
+> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
 
 ## 工具对比：
 | 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
 | :-: | :-: | :-: |
-| 是否跨平台 | 是 | 否，仅限 `Windows` |
+| 是否跨平台 | 是 | 否，仅限 Windows |
 | 是否开源 | 是 | 否 |
+| 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
-| 性能 | ... | |
 
 ## Q&A
 1、如何识别引文关系？  
-每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` 信息，则判断 `第一作者`、`发表年份`、`期刊名称`、`期号` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用关系。  
+`Web of Science:` 每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` ，则判断 `一作`、`发表年份`、`期刊名称`、`期次` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用。  
+`CSSCI:` 通过 `一作 `和 `题名` 两个字段进行判断。  
+
+2、如何去重？  
+`Web of Science:` 按照 `UT` 入藏号字段进行去重。  
+`CSSCI:` 按照 `一作` 和 `题名` 两个字段进行去重。
 
 ## TODO
-- [ ] 支持 `scopus` 题录数据
-- [ ] 构建 `GUI` 页面
+- [x] 支持 `CSSCI` 题录数据
+- [ ] 支持 `Scopus` 题录数据
+- [ ] 支持 `PubMed` 题录数据
```

### Comparing `histcite-python-0.1.5/README.md` & `histcite-python-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，并且可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为国科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
+
+最近更新：
+- `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持，并对调用方式进行调整；
 
 核心功能：
 - 生成引文网络图；
-- 生成包含文献、作者、机构、期刊、关键词等分析单元的引文统计数据；  
+- 生成包含文献、作者、机构、期刊、关键词等分析单元的统计数据；  
 
-## 术语说明
+术语说明：
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
 - `LCS`, Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如`TLCS` = 总本地引文分数；
 - `Recs`， 记录数；
-- Web of science题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
+- `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
+- 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
 
 ## 快速开始
-> 适用于本工具的数据集，来源Web of Science核心合集，<b> Tab delimited file/制表符分隔文件</b> 格式，导出内容选择 <b>Full Record and Cited References/全记录与引用的参考文献</b> 或者是 <b>Custome selection/自定义选择项</b>，全选字段，下载之后不要修改文件名，放在某个文件夹内；  
 ```console
 # 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
+## 数据准备
+| 数据来源 | 下载说明 |
+| :---: | --- |
+| `Web of Science` | 核心合集，格式选择 Tab delimited file/制表符分隔文件，导出内容选择 Full Record and Cited References/全记录与引用的参考文献 或者是 Custome selection/自定义选择项，全选字段 |
+| `CSSCI` | 从CSSCI数据库正常导出即可 |
+> 注：文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹下。
+
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
+| -t | --source_type | 题录数据来源，可选 `wos` 或 `cssci`，必须指定 |
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
-| -g | --graph | 是否仅生成图文件，指定该参数表示 `True`, 无需传值 |
+| -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
 
 ```console
-$ 假设下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数设置为 100
-$ histcite -f /Users/.../downloads/dataset -n 100
+$ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
+$ histcite -f /Users/.../downloads/dataset -t wos -n 100
 ```
-
-> 结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot` 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。 
+> 结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
 
 生成的引文网络图：
 
 <img src="examples/graph.svg">
 
 对应的文献节点信息：
 
@@ -53,54 +63,61 @@
 |    ...    |               |      |                                                  |      |      |
 
 2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
 
 ```python
 import os
 import pandas as pd
-from histcite.process_table import ParseTable
+from histcite.process_file import ProcessFile
 from histcite.compute_metrics import ComputeMetrics
-from histcite.network_graph import Graphviz
+from histcite.network_graph import GraphViz
 
 # 读取数据，解析引文
 folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
-process = ProcessTable(folder_path)
+source_type = 'wos'
+process = ProcessFile(folder_path, source_type)
 process.concat_table() # 合并多个文件
 process.process_citation() # 识别引文关系
 docs_table = process.docs_table
 reference_table = process.reference_table
 
 # 基本描述统计
-cm = ComputeMetrics(docs_table, reference_table)
+cm = ComputeMetrics(docs_table, reference_table, source_type)
 cm.write2excel(os.path.join(folder_path,'result','statistics.xlsx'))
 
 # 生成引文网络图文件
-graph = Graphviz(docs_table)
+graph = GraphViz(docs_table, source_type)
 doc_indices = docs_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
 graph_dot_file = graph.generate_dot_file(doc_indices, allow_external_node=False)
 
 # 保存引文网络图文件
 with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
-    f.write(dot_text)
+    f.write(graph_dot_file)
 
 # 保存引文网络图节点文件
 graph_node_file = graph.generate_graph_node_file()
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
-> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
+> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
 
 ## 工具对比：
 | 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
 | :-: | :-: | :-: |
-| 是否跨平台 | 是 | 否，仅限 `Windows` |
+| 是否跨平台 | 是 | 否，仅限 Windows |
 | 是否开源 | 是 | 否 |
+| 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
-| 性能 | ... | |
 
 ## Q&A
 1、如何识别引文关系？  
-每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` 信息，则判断 `第一作者`、`发表年份`、`期刊名称`、`期号` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用关系。  
+`Web of Science:` 每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` ，则判断 `一作`、`发表年份`、`期刊名称`、`期次` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用。  
+`CSSCI:` 通过 `一作 `和 `题名` 两个字段进行判断。  
+
+2、如何去重？  
+`Web of Science:` 按照 `UT` 入藏号字段进行去重。  
+`CSSCI:` 按照 `一作` 和 `题名` 两个字段进行去重。
 
 ## TODO
-- [ ] 支持 `scopus` 题录数据
-- [ ] 构建 `GUI` 页面
+- [x] 支持 `CSSCI` 题录数据
+- [ ] 支持 `Scopus` 题录数据
+- [ ] 支持 `PubMed` 题录数据
```

### Comparing `histcite-python-0.1.5/histcite/cli.py` & `histcite-python-0.2.0/histcite/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import os
 import argparse
 from histcite.compute_metrics import ComputeMetrics
-from histcite.process_table import ProcessTable
+from histcite.process_file import ProcessFile
 from histcite.network_graph import GraphViz
     
 def main():
     parser = argparse.ArgumentParser(description='A Python interface to histcite.')
     parser.add_argument('-f','--folder_path', type=str, required=True, help='folder path of the downloaded files')
+    parser.add_argument('-t','--source_type', type=str, required=True, choices=['wos','cssci'], help='source type of the downloaded files')
     parser.add_argument('-n','--node_num', type=int, default=50, help='node number in the citation network graph')
     parser.add_argument('-g','--graph', action="store_true", help='generate graph file only')
     args = parser.parse_args()
 
-    # 将结果存放在用户指定的 folder_path 下的result文件夹中
+    # 将结果存放在用户指定的folder_path下的result文件夹中
     output_path = os.path.join(args.folder_path,'result')
     if not os.path.exists(output_path):
         os.mkdir(output_path)
-    process = ProcessTable(args.folder_path)
+    process = ProcessFile(args.folder_path, args.source_type)
     process.concat_table()
     process.process_citation()
     docs_table = process.docs_table
     reference_table = process.reference_table
 
     if not args.graph:
-        cm = ComputeMetrics(docs_table, reference_table)
+        cm = ComputeMetrics(docs_table, reference_table, args.source_type)
         cm_output_path = os.path.join(output_path,'statistics.xlsx')
         cm.write2excel(cm_output_path)
 
     doc_indices = docs_table.sort_values('LCS', ascending=False).index[:args.node_num]
-    graph = GraphViz(docs_table)
+    graph = GraphViz(docs_table,args.source_type)
     
     # 生成图文件
     graph_dot_file = graph.generate_dot_file(doc_indices)
     graph_dot_path = os.path.join(output_path,'graph.dot')
     with open(graph_dot_path,'w') as f:
         f.write(graph_dot_file)
```

### Comparing `histcite-python-0.1.5/histcite/network_graph.py` & `histcite-python-0.2.0/histcite/network_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pandas as pd
 
 class GraphViz:
 
-    def __init__(self,docs_table):
+    def __init__(self,docs_table:pd.DataFrame,source_type:str):
         self.docs_table = docs_table
+        self.source_type = source_type
         self.year_empty_index = set(docs_table[docs_table['PY'].isna()].index)
 
     def __obtain_groups(self):
         """obtain groups of docs by year"""
 
         year_series = self.docs_table.loc[self.node_list,'PY']
         groups = year_series.groupby(year_series)
@@ -86,14 +87,23 @@
             
         for dot_edge in dot_edge_list:
             dot_text += dot_edge
         dot_text += '}'
         return dot_text
     
     def generate_graph_node_file(self)->pd.DataFrame:
-        use_cols = ['doc_index','AU','PY','SO','VL','BP','LCS','TC']
+        if self.source_type == 'wos':
+            use_cols = ['doc_index','AU','PY','SO','VL','BP','LCS','TC']
+        elif self.source_type == 'cssci':
+            use_cols = ['doc_index','AU','PY','SO','LCS']
+        else:
+            raise ValueError('invalid source type')
         graph_node_table = self.docs_table.loc[self.node_list,use_cols]
-        graph_node_table = graph_node_table.rename(columns={'TC':'GCS'})
+        
+        try:
+            graph_node_table = graph_node_table.rename(columns={'TC':'GCS'})
+        except KeyError:
+            pass
         return graph_node_table
     
     def _export_graph_node_file(self,file_path:str):
         self.generate_graph_node_file().to_excel(file_path,index=False)
```

### Comparing `histcite-python-0.1.5/histcite_python.egg-info/PKG-INFO` & `histcite-python-0.2.0/histcite_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.1.5
+Version: 0.2.0
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -19,50 +19,60 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，并且可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为国科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
+
+最近更新：
+- `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持，并对调用方式进行调整；
 
 核心功能：
 - 生成引文网络图；
-- 生成包含文献、作者、机构、期刊、关键词等分析单元的引文统计数据；  
+- 生成包含文献、作者、机构、期刊、关键词等分析单元的统计数据；  
 
-## 术语说明
+术语说明：
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
 - `LCS`, Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如`TLCS` = 总本地引文分数；
 - `Recs`， 记录数；
-- Web of science题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
+- `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
+- 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
 
 ## 快速开始
-> 适用于本工具的数据集，来源Web of Science核心合集，<b> Tab delimited file/制表符分隔文件</b> 格式，导出内容选择 <b>Full Record and Cited References/全记录与引用的参考文献</b> 或者是 <b>Custome selection/自定义选择项</b>，全选字段，下载之后不要修改文件名，放在某个文件夹内；  
 ```console
 # 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
+## 数据准备
+| 数据来源 | 下载说明 |
+| :---: | --- |
+| `Web of Science` | 核心合集，格式选择 Tab delimited file/制表符分隔文件，导出内容选择 Full Record and Cited References/全记录与引用的参考文献 或者是 Custome selection/自定义选择项，全选字段 |
+| `CSSCI` | 从CSSCI数据库正常导出即可 |
+> 注：文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹下。
+
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
+| -t | --source_type | 题录数据来源，可选 `wos` 或 `cssci`，必须指定 |
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
-| -g | --graph | 是否仅生成图文件，指定该参数表示 `True`, 无需传值 |
+| -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
 
 ```console
-$ 假设下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数设置为 100
-$ histcite -f /Users/.../downloads/dataset -n 100
+$ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
+$ histcite -f /Users/.../downloads/dataset -t wos -n 100
 ```
-
-> 结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot` 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。 
+> 结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
 
 生成的引文网络图：
 
 <img src="examples/graph.svg">
 
 对应的文献节点信息：
 
@@ -76,54 +86,61 @@
 |    ...    |               |      |                                                  |      |      |
 
 2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
 
 ```python
 import os
 import pandas as pd
-from histcite.process_table import ParseTable
+from histcite.process_file import ProcessFile
 from histcite.compute_metrics import ComputeMetrics
-from histcite.network_graph import Graphviz
+from histcite.network_graph import GraphViz
 
 # 读取数据，解析引文
 folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
-process = ProcessTable(folder_path)
+source_type = 'wos'
+process = ProcessFile(folder_path, source_type)
 process.concat_table() # 合并多个文件
 process.process_citation() # 识别引文关系
 docs_table = process.docs_table
 reference_table = process.reference_table
 
 # 基本描述统计
-cm = ComputeMetrics(docs_table, reference_table)
+cm = ComputeMetrics(docs_table, reference_table, source_type)
 cm.write2excel(os.path.join(folder_path,'result','statistics.xlsx'))
 
 # 生成引文网络图文件
-graph = Graphviz(docs_table)
+graph = GraphViz(docs_table, source_type)
 doc_indices = docs_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
 graph_dot_file = graph.generate_dot_file(doc_indices, allow_external_node=False)
 
 # 保存引文网络图文件
 with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
-    f.write(dot_text)
+    f.write(graph_dot_file)
 
 # 保存引文网络图节点文件
 graph_node_file = graph.generate_graph_node_file()
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
-> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
+> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
 
 ## 工具对比：
 | 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
 | :-: | :-: | :-: |
-| 是否跨平台 | 是 | 否，仅限 `Windows` |
+| 是否跨平台 | 是 | 否，仅限 Windows |
 | 是否开源 | 是 | 否 |
+| 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
-| 性能 | ... | |
 
 ## Q&A
 1、如何识别引文关系？  
-每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` 信息，则判断 `第一作者`、`发表年份`、`期刊名称`、`期号` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用关系。  
+`Web of Science:` 每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` ，则判断 `一作`、`发表年份`、`期刊名称`、`期次` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用。  
+`CSSCI:` 通过 `一作 `和 `题名` 两个字段进行判断。  
+
+2、如何去重？  
+`Web of Science:` 按照 `UT` 入藏号字段进行去重。  
+`CSSCI:` 按照 `一作` 和 `题名` 两个字段进行去重。
 
 ## TODO
-- [ ] 支持 `scopus` 题录数据
-- [ ] 构建 `GUI` 页面
+- [x] 支持 `CSSCI` 题录数据
+- [ ] 支持 `Scopus` 题录数据
+- [ ] 支持 `PubMed` 题录数据
```

### Comparing `histcite-python-0.1.5/setup.py` & `histcite-python-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="histcite-python",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.1.5",
+    version="0.2.0",
     description="A Python interface to histcite.",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["histcite","web of science","citation network"],
     license="MIT",
     url="https://github.com/doublessay/histcite-python",
     packages=["histcite"],
```

