# Comparing `tmp/vot-toolkit-0.6.0.tar.gz` & `tmp/vot-toolkit-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vot-toolkit-0.6.0.tar", last modified: Fri May  5 11:13:24 2023, max compression
+gzip compressed data, was "vot-toolkit-0.6.1.tar", last modified: Fri May 12 15:14:46 2023, max compression
```

## Comparing `vot-toolkit-0.6.0.tar` & `vot-toolkit-0.6.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.603696 vot-toolkit-0.6.0/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      211 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/MANIFEST.in
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3646 2023-05-05 11:13:24.603696 vot-toolkit-0.6.0/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2716 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/README.md
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      295 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/requirements.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2023-05-05 11:13:24.603696 vot-toolkit-0.6.0/setup.cfg
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1427 2023-05-05 11:11:52.000000 vot-toolkit-0.6.0/setup.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.575696 vot-toolkit-0.6.0/vot/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1867 2021-04-20 09:19:05.000000 vot-toolkit-0.6.0/vot/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      158 2021-04-20 09:19:05.000000 vot-toolkit-0.6.0/vot/__main__.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.579696 vot-toolkit-0.6.0/vot/analysis/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    15920 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/analysis/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    21427 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/analysis/_processor.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7608 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/analysis/accuracy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2517 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/analysis/failures.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16706 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/analysis/longterm.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12235 2023-04-18 14:33:10.000000 vot-toolkit-0.6.0/vot/analysis/multistart.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8824 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/analysis/supervised.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.579696 vot-toolkit-0.6.0/vot/dataset/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16723 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14672 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/dataset/cow.png
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3079 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/dummy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5356 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/got10k.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11511 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/otb.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4924 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/proxy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3753 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/trackingnet.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9243 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/vot.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.583696 vot-toolkit-0.6.0/vot/document/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12362 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/document/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      465 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/document/commands.tex
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5273 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/document/common.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5217 2021-04-15 12:10:29.000000 vot-toolkit-0.6.0/vot/document/html.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    89476 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/document/jquery.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5748 2022-03-11 09:29:31.000000 vot-toolkit-0.6.0/vot/document/latex.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16184 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/document/pure.css
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      647 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/document/report.css
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1212 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/document/report.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9933 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/document/table.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        0 2022-03-23 08:48:42.000000 vot-toolkit-0.6.0/vot/document/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.583696 vot-toolkit-0.6.0/vot/experiment/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7508 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/experiment/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      798 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/experiment/helpers.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7180 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/experiment/multirun.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3044 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/experiment/multistart.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3214 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/experiment/transformer.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.587696 vot-toolkit-0.6.0/vot/region/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2373 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/region/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8674 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/region/io.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9593 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/region/raster.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10172 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/region/shapes.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/region/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.587696 vot-toolkit-0.6.0/vot/stack/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3047 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      253 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/otb100.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      251 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/otb50.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/tests/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      183 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/tests/basic.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      550 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/tests/multiobject.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      638 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/tests/segmentation.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      863 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      351 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2013.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      374 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2014.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/vot2015/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      405 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2015/rgb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      322 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2015/tir.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/vot2016/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      540 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2016/rgb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2016/tir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      856 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2017.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/vot2018/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2018/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      791 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2018/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/vot2019/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2019/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2019/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2019/rgbtir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      789 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2019/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/vot2020/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2020/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2020/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2020/rgbtir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2020/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/vot2021/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2021/lt.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2021/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2021/st.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.595696 vot-toolkit-0.6.0/vot/stack/vot2022/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      422 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2022/depth.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      482 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/vot2022/lt.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      424 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/vot2022/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/vot2022/stb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/vot2022/sts.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      388 2023-05-04 11:42:13.000000 vot-toolkit-0.6.0/vot/stack/vots2023.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.595696 vot-toolkit-0.6.0/vot/tracker/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    19651 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/tracker/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      763 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/tracker/dummy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6642 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/tracker/results.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      476 2021-04-20 09:19:05.000000 vot-toolkit-0.6.0/vot/tracker/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    19771 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/tracker/trax.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.599696 vot-toolkit-0.6.0/vot/utilities/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12508 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/utilities/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16157 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/utilities/cli.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2635 2021-04-15 12:10:29.000000 vot-toolkit-0.6.0/vot/utilities/data.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8255 2021-04-15 12:10:29.000000 vot-toolkit-0.6.0/vot/utilities/draw.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3609 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/utilities/migration.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3798 2021-04-20 09:19:05.000000 vot-toolkit-0.6.0/vot/utilities/net.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8133 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/utilities/notebook.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       45 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/version.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.599696 vot-toolkit-0.6.0/vot/workspace/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7013 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/workspace/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10512 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/workspace/storage.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1782 2022-03-11 09:29:31.000000 vot-toolkit-0.6.0/vot/workspace/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.603696 vot-toolkit-0.6.0/vot_toolkit.egg-info/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3646 2023-05-05 11:13:24.000000 vot-toolkit-0.6.0/vot_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2409 2023-05-05 11:13:24.000000 vot-toolkit-0.6.0/vot_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2023-05-05 11:13:24.000000 vot-toolkit-0.6.0/vot_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       48 2023-05-05 11:13:24.000000 vot-toolkit-0.6.0/vot_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-05 11:13:24.000000 vot-toolkit-0.6.0/vot_toolkit.egg-info/requires.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        4 2023-05-05 11:13:24.000000 vot-toolkit-0.6.0/vot_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.168255 vot-toolkit-0.6.1/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      211 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/MANIFEST.in
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3646 2023-05-12 15:14:46.168255 vot-toolkit-0.6.1/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2716 2023-05-09 11:09:24.000000 vot-toolkit-0.6.1/README.md
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      295 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/requirements.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2023-05-12 15:14:46.168255 vot-toolkit-0.6.1/setup.cfg
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1427 2023-05-09 11:09:24.000000 vot-toolkit-0.6.1/setup.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.140256 vot-toolkit-0.6.1/vot/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1889 2023-05-10 17:51:17.000000 vot-toolkit-0.6.1/vot/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      158 2021-04-20 09:19:05.000000 vot-toolkit-0.6.1/vot/__main__.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.144255 vot-toolkit-0.6.1/vot/analysis/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    15920 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/analysis/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    21427 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/analysis/_processor.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7608 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/analysis/accuracy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2517 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/analysis/failures.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16706 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/analysis/longterm.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12235 2023-04-18 14:33:10.000000 vot-toolkit-0.6.1/vot/analysis/multistart.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8824 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/analysis/supervised.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.148255 vot-toolkit-0.6.1/vot/dataset/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16723 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/dataset/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14672 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/dataset/cow.png
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3079 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/dataset/dummy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5356 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/dataset/got10k.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11511 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/dataset/otb.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4924 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/dataset/proxy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3753 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/dataset/trackingnet.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9239 2023-05-10 17:51:17.000000 vot-toolkit-0.6.1/vot/dataset/vot.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.152255 vot-toolkit-0.6.1/vot/document/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12362 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/document/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      465 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/document/commands.tex
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5273 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/document/common.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5217 2021-04-15 12:10:29.000000 vot-toolkit-0.6.1/vot/document/html.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    89476 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/document/jquery.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5748 2022-03-11 09:29:31.000000 vot-toolkit-0.6.1/vot/document/latex.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16184 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/document/pure.css
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      647 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/document/report.css
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1212 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/document/report.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9933 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/document/table.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        0 2022-03-23 08:48:42.000000 vot-toolkit-0.6.1/vot/document/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.152255 vot-toolkit-0.6.1/vot/experiment/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7631 2023-05-12 15:11:47.000000 vot-toolkit-0.6.1/vot/experiment/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      798 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/experiment/helpers.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7180 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/experiment/multirun.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3044 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/experiment/multistart.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3214 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/experiment/transformer.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.152255 vot-toolkit-0.6.1/vot/region/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2373 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/region/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9258 2023-05-12 12:23:17.000000 vot-toolkit-0.6.1/vot/region/io.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9593 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/region/raster.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10172 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/region/shapes.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3238 2023-05-12 11:54:32.000000 vot-toolkit-0.6.1/vot/region/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.156256 vot-toolkit-0.6.1/vot/stack/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3047 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      253 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/otb100.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      251 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/otb50.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.156256 vot-toolkit-0.6.1/vot/stack/tests/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      183 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/tests/basic.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      550 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/tests/multiobject.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      638 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/tests/segmentation.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      863 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      351 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2013.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      374 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2014.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.156256 vot-toolkit-0.6.1/vot/stack/vot2015/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      405 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2015/rgb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      322 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2015/tir.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.156256 vot-toolkit-0.6.1/vot/stack/vot2016/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      540 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2016/rgb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2016/tir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      856 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2017.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.156256 vot-toolkit-0.6.1/vot/stack/vot2018/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2018/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      791 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2018/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.160256 vot-toolkit-0.6.1/vot/stack/vot2019/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2019/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2019/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2019/rgbtir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      789 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2019/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.160256 vot-toolkit-0.6.1/vot/stack/vot2020/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2020/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2020/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2020/rgbtir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2020/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.160256 vot-toolkit-0.6.1/vot/stack/vot2021/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2021/lt.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2021/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2021/st.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.164255 vot-toolkit-0.6.1/vot/stack/vot2022/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      422 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2022/depth.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      482 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/vot2022/lt.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      424 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/vot2022/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/vot2022/stb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/vot2022/sts.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2023-05-10 17:51:17.000000 vot-toolkit-0.6.1/vot/stack/vots2023.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.164255 vot-toolkit-0.6.1/vot/tracker/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    19774 2023-05-12 15:12:58.000000 vot-toolkit-0.6.1/vot/tracker/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      763 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/tracker/dummy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6642 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/tracker/results.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      476 2021-04-20 09:19:05.000000 vot-toolkit-0.6.1/vot/tracker/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    19771 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/tracker/trax.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.168255 vot-toolkit-0.6.1/vot/utilities/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12508 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/utilities/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16476 2023-05-10 17:51:17.000000 vot-toolkit-0.6.1/vot/utilities/cli.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2635 2021-04-15 12:10:29.000000 vot-toolkit-0.6.1/vot/utilities/data.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8255 2021-04-15 12:10:29.000000 vot-toolkit-0.6.1/vot/utilities/draw.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3609 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/utilities/migration.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3798 2021-04-20 09:19:05.000000 vot-toolkit-0.6.1/vot/utilities/net.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8133 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/utilities/notebook.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       45 2023-05-09 11:09:24.000000 vot-toolkit-0.6.1/vot/version.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.168255 vot-toolkit-0.6.1/vot/workspace/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7013 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/workspace/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10512 2023-05-12 11:16:07.000000 vot-toolkit-0.6.1/vot/workspace/storage.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1786 2023-05-12 10:35:28.000000 vot-toolkit-0.6.1/vot/workspace/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.168255 vot-toolkit-0.6.1/vot_toolkit.egg-info/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3646 2023-05-12 15:14:45.000000 vot-toolkit-0.6.1/vot_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2409 2023-05-12 15:14:45.000000 vot-toolkit-0.6.1/vot_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2023-05-12 15:14:45.000000 vot-toolkit-0.6.1/vot_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       48 2023-05-12 15:14:45.000000 vot-toolkit-0.6.1/vot_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-12 15:14:45.000000 vot-toolkit-0.6.1/vot_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        4 2023-05-12 15:14:45.000000 vot-toolkit-0.6.1/vot_toolkit.egg-info/top_level.txt
```

### Comparing `vot-toolkit-0.6.0/PKG-INFO` & `vot-toolkit-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vot-toolkit
-Version: 0.6.0
+Version: 0.6.1
 Summary: Perform visual object tracking experiments and analyze results
 Home-page: https://github.com/votchallenge/toolkit
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Description: 
         The VOT evaluation toolkit
@@ -29,15 +29,15 @@
         ----------------
         
         The development of this package was supported by Sloveninan research agency (ARRS) projects Z2-1866 and J2-316.
         
         License
         -------
         
-        Copyright (C) 2021 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
+        Copyright (C) 2023 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
         
         This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
         
         This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
         
         You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `vot-toolkit-0.6.0/README.md` & `vot-toolkit-0.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ----------------
 
 The development of this package was supported by Sloveninan research agency (ARRS) projects Z2-1866 and J2-316.
 
 License
 -------
 
-Copyright (C) 2021 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
+Copyright (C) 2023 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `vot-toolkit-0.6.0/setup.py` & `vot-toolkit-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/__init__.py` & `vot-toolkit-0.6.1/vot/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     import requests
     pattern = r"^__version__ = ['\"]([^'\"]*)['\"]"
 
     version_url = "https://github.com/votchallenge/vot-toolkit-python/raw/master/vot/version.py"
 
     try:
         get_logger().debug("Checking for new version")
-        response = requests.get(version_url, timeout=2)
+        response = requests.get(version_url, timeout=5, allow_redirects=True)
     except Exception as e:
         get_logger().debug("Unable to retrieve version information %s", e)
         return False, None
 
     if not response:
         return False, None
```

### Comparing `vot-toolkit-0.6.0/vot/analysis/__init__.py` & `vot-toolkit-0.6.1/vot/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/analysis/_processor.py` & `vot-toolkit-0.6.1/vot/analysis/_processor.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/analysis/accuracy.py` & `vot-toolkit-0.6.1/vot/analysis/accuracy.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/analysis/failures.py` & `vot-toolkit-0.6.1/vot/analysis/failures.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/analysis/longterm.py` & `vot-toolkit-0.6.1/vot/analysis/longterm.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/analysis/multistart.py` & `vot-toolkit-0.6.1/vot/analysis/multistart.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/analysis/supervised.py` & `vot-toolkit-0.6.1/vot/analysis/supervised.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/dataset/__init__.py` & `vot-toolkit-0.6.1/vot/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/dataset/cow.png` & `vot-toolkit-0.6.1/vot/dataset/cow.png`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/dataset/dummy.py` & `vot-toolkit-0.6.1/vot/dataset/dummy.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/dataset/got10k.py` & `vot-toolkit-0.6.1/vot/dataset/got10k.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/dataset/otb.py` & `vot-toolkit-0.6.1/vot/dataset/otb.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/dataset/proxy.py` & `vot-toolkit-0.6.1/vot/dataset/proxy.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/dataset/trackingnet.py` & `vot-toolkit-0.6.1/vot/dataset/trackingnet.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/dataset/vot.py` & `vot-toolkit-0.6.1/vot/dataset/vot.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,16 +64,16 @@
         self._metadata["width"], self._metadata["height"] = six.next(six.itervalues(channels)).size
 
         lenghts = [len(t) for t in channels.values()]
         assert all([x == lenghts[0] for x in lenghts]), "Sequence channels have different lengths"
         length = lenghts[0]
 
         objectsfiles = glob.glob(os.path.join(self._base, 'groundtruth_*.txt'))
+        objects = {}
         if len(objectsfiles) > 0:
-            objects = {}
             for objectfile in objectsfiles:
                 groundtruth = read_trajectory(os.path.join(objectfile))
                 if len(groundtruth) < length: groundtruth += [Special(Sequence.UNKNOWN)] * (length - len(groundtruth))
                 objectid = os.path.basename(objectfile)[12:-4]
                 objects[objectid] = groundtruth
         else:
             groundtruth_file = os.path.join(self._base, self.metadata("groundtruth", "groundtruth.txt"))
```

### Comparing `vot-toolkit-0.6.0/vot/document/__init__.py` & `vot-toolkit-0.6.1/vot/document/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/document/common.py` & `vot-toolkit-0.6.1/vot/document/common.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/document/html.py` & `vot-toolkit-0.6.1/vot/document/html.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/document/jquery.js` & `vot-toolkit-0.6.1/vot/document/jquery.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/document/latex.py` & `vot-toolkit-0.6.1/vot/document/latex.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/document/pure.css` & `vot-toolkit-0.6.1/vot/document/pure.css`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/document/report.css` & `vot-toolkit-0.6.1/vot/document/report.css`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/document/report.js` & `vot-toolkit-0.6.1/vot/document/report.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/document/table.js` & `vot-toolkit-0.6.1/vot/document/table.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/experiment/__init__.py` & `vot-toolkit-0.6.1/vot/experiment/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,15 +101,16 @@
     def _get_runtime(self, tracker: "Tracker", sequence: "Sequence", multiobject=False):
         from ..tracker import SingleObjectTrackerRuntime, RealtimeTrackerRuntime, MultiObjectTrackerRuntime
 
         runtime = tracker.runtime()
 
         if multiobject:
             if not runtime.multiobject:
-                runtime = MultiObjectTrackerRuntime(runtime)
+                raise TrackerException("Tracker {} does not support multi-object experiments".format(tracker.identifier))
+                #runtime = MultiObjectTrackerRuntime(runtime)
         else:
             runtime = SingleObjectTrackerRuntime(runtime)
 
         if not self.realtime is None:
             grace = to_number(self.realtime.grace, min_n=0)
             fps = to_number(self.realtime.fps, min_n=0, conversion=float)
             interval = 1 / float(sequence.metadata("fps", fps))
```

### Comparing `vot-toolkit-0.6.0/vot/experiment/helpers.py` & `vot-toolkit-0.6.1/vot/experiment/helpers.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/experiment/multirun.py` & `vot-toolkit-0.6.1/vot/experiment/multirun.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/experiment/multistart.py` & `vot-toolkit-0.6.1/vot/experiment/multistart.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/experiment/transformer.py` & `vot-toolkit-0.6.1/vot/experiment/transformer.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/region/__init__.py` & `vot-toolkit-0.6.1/vot/region/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/region/io.py` & `vot-toolkit-0.6.1/vot/region/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import struct
 import io
 
 import numpy as np
 from numba import jit
 
 @jit(nopython=True)
-def mask_to_rle(m):
+def mask_to_rle(m, maxstride=100000000):
     """
     # Input: 2-D numpy array
     # Output: list of numbers (1st number = #0s, 2nd number = #1s, 3rd number = #0s, ...)
     """
     # reshape mask to vector
     v = m.reshape((m.shape[0] * m.shape[1]))
 
@@ -25,22 +25,36 @@
     # check if first element is 1, so first element in RLE (number of zeros) must be set to 0
     if v[0] > 0:
         rle.append(0)
 
     # go over all elements and check if two consecutive are the same
     for i in range(1, v.size):
         if v[i] != v[i - 1]:
-            rle.append(i - last_idx)
+            length = i - last_idx
+            # if length is larger than maxstride, split it into multiple elements
+            while length > maxstride:
+                rle.append(maxstride)
+                rle.append(0)
+                length -= maxstride
+            # add remaining length
+            if length > 0:
+                rle.append(length)
             last_idx = i
 
     if v.size > 0:
         # handle last element of rle
         if last_idx < v.size - 1:
             # last element is the same as one element before it - add number of these last elements
-            rle.append(v.size - last_idx)
+            length = v.size - last_idx
+            while length > maxstride:
+                rle.append(maxstride)
+                rle.append(0)
+                length -= maxstride
+            if length > 0:
+                rle.append(length)
         else:
             # last element is different than one element before - add 1
             rle.append(1)
 
     return rle
 
 @jit(nopython=True)
@@ -80,15 +94,14 @@
     rle = np.array([el for el in elements[4:]], dtype=np.int32)
 
     # create mask from RLE within target region
     mask = rle_to_mask(rle, region_w, region_h)
 
     return mask, (tl_x, tl_y)
 
-
 from vot.region.raster import mask_bounds
 
 def encode_mask(mask):
     """
     mask: input binary mask, type: uint8
     output: full RLE encoding in the format: (x0, y0, w, h), RLE
     first get minimal axis-aligned region which contains all positive pixels
@@ -175,15 +188,15 @@
         elif type == 1: r = Rectangle(*read("<ffff"))
         elif type == 2:
             n, = read("<H")
             values = read("<%df" % (2 * n))
             r = Polygon(list(zip(values[0::2], values[1::2])))
         elif type == 3:
             tl_x, tl_y, region_w, region_h, n = read("<hhHHH")
-            rle = read("<%dH" % (n))
+            rle = np.array(read("<%dH" % (n)), dtype=np.int32)
             r = Mask(rle_to_mask(rle, region_w, region_h), (tl_x, tl_y))
         else:
             raise IOError("Wrong region type")
         trajectory.append(r)
     return trajectory
 
 def write_trajectory_binary(fp: io.RawIOBase, data: List["Region"]):
@@ -194,15 +207,15 @@
     fp.write(struct.pack("<hI", 1, len(data)))
 
     for r in data:
         if isinstance(r, Special): fp.write(struct.pack("<BI", 0, r.code))
         elif isinstance(r, Rectangle): fp.write(struct.pack("<Bffff", 1, r.x, r.y, r.width, r.height))
         elif isinstance(r, Polygon): fp.write(struct.pack("<BH%df" % (2 * r.size), 2, r.size, *[item for sublist in r.points() for item in sublist]))
         elif isinstance(r, Mask): 
-            rle = mask_to_rle(r.mask)
+            rle = mask_to_rle(r.mask, maxstride=255*255)
             fp.write(struct.pack("<BhhHHH%dH" % len(rle), 3, r.offset[0], r.offset[1], r.mask.shape[1], r.mask.shape[0], len(rle), *rle))
         else:
             raise IOError("Wrong region type")
 
 def read_trajectory(fp: Union[str, TextIO]):
     if isinstance(fp, str):
         try:
```

### Comparing `vot-toolkit-0.6.0/vot/region/raster.py` & `vot-toolkit-0.6.1/vot/region/raster.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/region/shapes.py` & `vot-toolkit-0.6.1/vot/region/shapes.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/region/tests.py` & `vot-toolkit-0.6.1/vot/region/tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -65,8 +65,19 @@
         bint = read_trajectory(binf)
         txtt = read_trajectory(txtf)
 
         o1 = calculate_overlaps(bint, txtt, None)
         o2 = calculate_overlaps(bint, trajectory, None)
 
         self.assertTrue(np.all(np.array(o1) == 1))
-        self.assertTrue(np.all(np.array(o2) == 1))
+        self.assertTrue(np.all(np.array(o2) == 1))
+
+    def test_rle(self):
+        from vot.region.io import rle_to_mask, mask_to_rle 
+        rle = [0, 2, 122103, 9, 260, 19, 256, 21, 256, 22, 254, 24, 252, 26, 251, 27, 250, 28, 249, 28, 250, 28, 249, 28, 249, 29, 249, 30, 247, 33, 245, 33, 244, 34, 244, 37, 241, 39, 239, 41, 237, 41, 236, 43, 235, 45, 234, 47, 233, 47, 231, 48, 230, 48, 230, 11, 7, 29, 231, 9, 9, 29, 230, 8, 11, 28, 230, 7, 12, 28, 230, 7, 13, 27, 231, 5, 14, 27, 233, 2, 16, 26, 253, 23, 255, 22, 256, 20, 258, 19, 259, 17, 3]
+        rle = np.array(rle)
+        m1 = rle_to_mask(np.array(rle, dtype=np.int32), 277, 478)
+
+        r2 = mask_to_rle(m1, maxstride=255)
+        m2 = rle_to_mask(np.array(r2, dtype=np.int32), 277, 478)
+
+        np.testing.assert_array_equal(m1, m2)
```

### Comparing `vot-toolkit-0.6.0/vot/stack/__init__.py` & `vot-toolkit-0.6.1/vot/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/stack/tests/multiobject.yaml` & `vot-toolkit-0.6.1/vot/stack/tests/multiobject.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/stack/tests/segmentation.yaml` & `vot-toolkit-0.6.1/vot/stack/tests/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/stack/tests.py` & `vot-toolkit-0.6.1/vot/stack/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/stack/vot2016/rgb.yaml` & `vot-toolkit-0.6.1/vot/stack/vot2016/rgb.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/stack/vot2017.yaml` & `vot-toolkit-0.6.1/vot/stack/vot2017.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/stack/vot2018/shortterm.yaml` & `vot-toolkit-0.6.1/vot/stack/vot2018/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/stack/vot2019/shortterm.yaml` & `vot-toolkit-0.6.1/vot/stack/vot2019/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/stack/vot2020/shortterm.yaml` & `vot-toolkit-0.6.1/vot/stack/vot2020/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/stack/vot2021/st.yaml` & `vot-toolkit-0.6.1/vot/stack/vot2021/st.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/stack/vot2022/stb.yaml` & `vot-toolkit-0.6.1/vot/stack/vot2022/stb.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/stack/vot2022/sts.yaml` & `vot-toolkit-0.6.1/vot/stack/vot2022/sts.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/tracker/__init__.py` & `vot-toolkit-0.6.1/vot/tracker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -544,14 +544,15 @@
 
         if not new is None: raise TrackerException("Only supports single object tracking", tracker=self.tracker)
         status = self._runtime.update(frame, new, properties)
         if isinstance(status, list): status = status[0]
         return status
 
 class MultiObjectTrackerRuntime(TrackerRuntime):
+    """ This is a wrapper for tracker runtimes that do not support multi object tracking. It is still work in progress."""
 
     def __init__(self, runtime: TrackerRuntime):
         super().__init__(runtime.tracker)
         if self._runtime.multiobject:
             self._runtime = runtime
         else:
             self._runtime = [runtime]
```

### Comparing `vot-toolkit-0.6.0/vot/tracker/dummy.py` & `vot-toolkit-0.6.1/vot/tracker/dummy.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/tracker/results.py` & `vot-toolkit-0.6.1/vot/tracker/results.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/tracker/trax.py` & `vot-toolkit-0.6.1/vot/tracker/trax.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/utilities/__init__.py` & `vot-toolkit-0.6.1/vot/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/utilities/cli.py` & `vot-toolkit-0.6.1/vot/utilities/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,32 +328,35 @@
         manifest = dict(identifier=tracker.identifier, configuration=tracker.describe(),
             timestamp="{:%Y-%m-%dT%H-%M-%S.%f%z}".format(timestamp), platform=sys.platform,
             python=sys.version, toolkit=toolkit_version())
 
         with zipfile.ZipFile(workspace.storage.write(archive_name, binary=True), mode="w") as archive:
             for f in all_files:
                 info = zipfile.ZipInfo(filename=os.path.join(f[1], f[2], f[0]), date_time=timestamp.timetuple())
-                with io.TextIOWrapper(archive.open(info, mode="w")) as fout, f[3].read(f[0]) as fin:
-                    copyfileobj(fin, fout)
+                with archive.open(info, mode="w") as fout, f[3].read(f[0]) as fin:
+                    if isinstance(fin, io.TextIOBase):
+                        copyfileobj(fin, io.TextIOWrapper(fout))
+                    else:
+                        copyfileobj(fin, fout)
                 progress.relative(1)
 
             info = zipfile.ZipInfo(filename="manifest.yml", date_time=timestamp.timetuple())
             with io.TextIOWrapper(archive.open(info, mode="w")) as fout:
                 yaml.dump(manifest, fout)
 
     logger.info("Result packaging successful, archive available in %s", archive_name)
 
 def main():
-    """Entrypoint to the VOT Command Line Interface utility, should be executed as a program and provided with arguments.
+    """Entrypoint to the toolkit Command Line Interface utility, should be executed as a program and provided with arguments.
     """
     stream = logging.StreamHandler()
     stream.setFormatter(ColoredFormatter())
     logger.addHandler(stream)
 
-    parser = argparse.ArgumentParser(description='VOT Toolkit Command Line Utility', prog="vot")
+    parser = argparse.ArgumentParser(description='VOT Toolkit Command Line Interface', prog="vot")
     parser.add_argument("--debug", "-d", default=False, help="Backup backend", required=False, action='store_true')
     parser.add_argument("--registry", default=".", help='Tracker registry paths', required=False, action=EnvDefault, \
         separator=os.path.pathsep, envvar='VOT_REGISTRY')
 
     subparsers = parser.add_subparsers(help='commands', dest='action', title="Commands")
 
     test_parser = subparsers.add_parser('test', help='Test a tracker integration on a synthetic sequence')
@@ -389,27 +392,33 @@
         args = parser.parse_args()
 
         logger.setLevel(logging.INFO)
 
         if args.debug or check_debug():
             logger.setLevel(logging.DEBUG)
 
-        update, version = check_updates()
-        if update:
-            logger.warning("A newer version of the VOT toolkit is available (%s), please update.", version)
+        def check_version():
+            update, version = check_updates()
+            if update:
+                logger.warning("A newer version of the VOT toolkit is available (%s), please update.", version)
 
         if args.action == "test":
+            check_version()
             do_test(args)
         elif args.action == "initialize":
+            check_version()
             do_workspace(args)
         elif args.action == "evaluate":
+            check_version()
             do_evaluate(args)
         elif args.action == "analysis":
+            check_version()
             do_analysis(args)
         elif args.action == "pack":
+            check_version()
             do_pack(args)
         else:
             parser.print_help()
 
     except argparse.ArgumentError as e:
         logger.error(e)
         exit(-1)
```

### Comparing `vot-toolkit-0.6.0/vot/utilities/data.py` & `vot-toolkit-0.6.1/vot/utilities/data.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/utilities/draw.py` & `vot-toolkit-0.6.1/vot/utilities/draw.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/utilities/migration.py` & `vot-toolkit-0.6.1/vot/utilities/migration.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/utilities/net.py` & `vot-toolkit-0.6.1/vot/utilities/net.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/utilities/notebook.py` & `vot-toolkit-0.6.1/vot/utilities/notebook.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/workspace/__init__.py` & `vot-toolkit-0.6.1/vot/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/workspace/storage.py` & `vot-toolkit-0.6.1/vot/workspace/storage.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.0/vot/workspace/tests.py` & `vot-toolkit-0.6.1/vot/workspace/tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     def test_workspace_create(self):
         """Test if workspace creation works
         """
        
         get_logger().setLevel(logging.WARN) # Disable progress bar
 
-        default_config = dict(stack="testing", registry=["./trackers.ini"])
+        default_config = dict(stack="tests/basic", registry=["./trackers.ini"])
 
         with tempfile.TemporaryDirectory() as testdir:
             Workspace.initialize(testdir, default_config, download=True)
             Workspace.load(testdir)
 
     def test_cache(self):
         """Test if local storage cache works
```

### Comparing `vot-toolkit-0.6.0/vot_toolkit.egg-info/PKG-INFO` & `vot-toolkit-0.6.1/vot_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vot-toolkit
-Version: 0.6.0
+Version: 0.6.1
 Summary: Perform visual object tracking experiments and analyze results
 Home-page: https://github.com/votchallenge/toolkit
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Description: 
         The VOT evaluation toolkit
@@ -29,15 +29,15 @@
         ----------------
         
         The development of this package was supported by Sloveninan research agency (ARRS) projects Z2-1866 and J2-316.
         
         License
         -------
         
-        Copyright (C) 2021 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
+        Copyright (C) 2023 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
         
         This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
         
         This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
         
         You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `vot-toolkit-0.6.0/vot_toolkit.egg-info/SOURCES.txt` & `vot-toolkit-0.6.1/vot_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

