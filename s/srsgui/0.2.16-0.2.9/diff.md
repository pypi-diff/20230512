# Comparing `tmp/srsgui-0.2.16.tar.gz` & `tmp/srsgui-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-h87fld5t\srsgui-0.2.16.tar", last modified: Fri May 12 21:48:43 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-ps3u1u8m\srsgui-0.2.9.tar", last modified: Tue Apr 11 21:39:00 2023, max compression
```

## Comparing `srsgui-0.2.16.tar` & `srsgui-0.2.9.tar`

### file list

```diff
@@ -1,113 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.445550 srsgui-0.2.16/
--rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.16/.gitignore
--rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.16/LICENSE.txt
--rw-rw-rw-   0        0        0     3331 2023-05-12 21:48:43.445550 srsgui-0.2.16/PKG-INFO
--rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.16/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.337724 srsgui-0.2.16/docs/
--rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/Makefile
--rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/autodoc.bat
--rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.357729 srsgui-0.2.16/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.367744 srsgui-0.2.16/docs/source/_static/
--rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/conf.py
--rw-rw-rw-   0        0        0     6097 2023-05-11 18:52:38.000000 srsgui-0.2.16/docs/source/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.16/docs/source/create-task.rst
--rw-rw-rw-   0        0        0     6111 2023-05-11 18:59:55.000000 srsgui-0.2.16/docs/source/define-instrument.rst
--rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.16/docs/source/example.rst
--rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.16/docs/source/index.rst
--rw-rw-rw-   0        0        0     4397 2023-05-11 18:35:43.000000 srsgui-0.2.16/docs/source/installation.rst
--rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/srsgui.inst.rst
--rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/srsgui.rst
--rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.16/docs/source/srsgui.task.rst
--rw-rw-rw-   0        0        0      557 2023-05-11 18:10:15.000000 srsgui-0.2.16/docs/source/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1761 2023-05-11 18:09:50.000000 srsgui-0.2.16/docs/source/srsgui.ui.rst
--rw-rw-rw-   0        0        0     1197 2023-04-25 23:39:24.000000 srsgui-0.2.16/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.16/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 21:48:43.445550 srsgui-0.2.16/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.16/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.367744 srsgui-0.2.16/srsgui/
--rw-rw-rw-   0        0        0     1538 2023-05-12 21:43:30.000000 srsgui-0.2.16/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.16/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.331033 srsgui-0.2.16/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.377754 srsgui-0.2.16/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.377754 srsgui-0.2.16/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.16/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.387729 srsgui-0.2.16/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.395548 srsgui-0.2.16/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.16/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9767 2023-05-11 21:10:00.000000 srsgui-0.2.16/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.395548 srsgui-0.2.16/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     8189 2023-05-03 16:28:26.000000 srsgui-0.2.16/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8653 2023-05-03 18:08:35.000000 srsgui-0.2.16/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    11214 2023-05-03 16:38:33.000000 srsgui-0.2.16/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    14719 2023-05-12 17:44:46.000000 srsgui-0.2.16/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10260 2023-05-11 23:50:12.000000 srsgui-0.2.16/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.16/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.405575 srsgui-0.2.16/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-04-10 22:51:26.000000 srsgui-0.2.16/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.16/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5203 2023-04-11 00:24:36.000000 srsgui-0.2.16/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6711 2023-05-01 19:53:04.000000 srsgui-0.2.16/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    22017 2023-04-25 23:39:24.000000 srsgui-0.2.16/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.435579 srsgui-0.2.16/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.16/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     6019 2023-04-25 23:39:24.000000 srsgui-0.2.16/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.445550 srsgui-0.2.16/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0        0 2023-05-11 18:21:35.000000 srsgui-0.2.16/srsgui/ui/commandtree/__init__.py
--rw-rw-rw-   0        0        0     3820 2023-05-08 22:24:37.000000 srsgui-0.2.16/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     1484 2023-05-08 22:25:43.000000 srsgui-0.2.16/srsgui/ui/commandtree/commandhandler.py
--rw-rw-rw-   0        0        0    11930 2023-05-11 18:15:24.000000 srsgui-0.2.16/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     8215 2023-05-08 22:27:34.000000 srsgui-0.2.16/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     4953 2023-05-12 00:08:01.000000 srsgui-0.2.16/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3331 2023-04-25 23:39:24.000000 srsgui-0.2.16/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     4128 2023-05-11 18:29:21.000000 srsgui-0.2.16/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     4806 2023-04-25 23:39:24.000000 srsgui-0.2.16/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9679 2023-05-10 21:45:12.000000 srsgui-0.2.16/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.16/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    15759 2023-04-25 23:39:24.000000 srsgui-0.2.16/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    13689 2023-05-01 19:10:07.000000 srsgui-0.2.16/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.445550 srsgui-0.2.16/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.16/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.16/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    24695 2023-05-01 19:05:09.000000 srsgui-0.2.16/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.16/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.16/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:48:43.377754 srsgui-0.2.16/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3331 2023-05-12 21:48:43.000000 srsgui-0.2.16/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3060 2023-05-12 21:48:43.000000 srsgui-0.2.16/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 21:48:43.000000 srsgui-0.2.16/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-12 21:48:43.000000 srsgui-0.2.16/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-05-12 21:48:43.000000 srsgui-0.2.16/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-12 21:48:43.000000 srsgui-0.2.16/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.979862 srsgui-0.2.9/
+-rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.9/.gitignore
+-rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3330 2023-04-11 21:39:00.979862 srsgui-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.889910 srsgui-0.2.9/docs/
+-rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/Makefile
+-rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/autodoc.bat
+-rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.899904 srsgui-0.2.9/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/docs/source/_static/
+-rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/conf.py
+-rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/create-task.rst
+-rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/define-instrument.rst
+-rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/example.rst
+-rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/index.rst
+-rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/installation.rst
+-rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.rst
+-rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.task.rst
+-rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:39:00.979862 srsgui-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-04-11 21:34:20.000000 srsgui-0.2.9/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.9/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.879943 srsgui-0.2.9/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.929916 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.939882 srsgui-0.2.9/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.9/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9578 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.939882 srsgui-0.2.9/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    14665 2023-04-11 20:13:55.000000 srsgui-0.2.9/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10049 2023-04-11 18:04:43.000000 srsgui-0.2.9/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.9/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.949878 srsgui-0.2.9/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.9/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5203 2023-04-11 00:24:36.000000 srsgui-0.2.9/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.9/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    22234 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.959872 srsgui-0.2.9/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.969903 srsgui-0.2.9/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.py
+-rw-rw-rw-   0        0        0     3362 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.ui
+-rw-rw-rw-   0        0        0     3489 2023-04-11 17:28:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0    10180 2023-04-10 18:03:49.000000 srsgui-0.2.9/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     7833 2023-04-11 17:29:16.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     4755 2023-04-11 17:22:27.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3127 2023-04-11 21:33:12.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     3844 2023-04-11 17:33:14.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/jsonmodel.py
+-rw-rw-rw-   0        0        0     4803 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/ui/commandtree/ui_commandcapturewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-04-11 17:35:42.000000 srsgui-0.2.9/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.9/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    14127 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    13671 2023-04-11 00:24:36.000000 srsgui-0.2.9/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.979862 srsgui-0.2.9/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.9/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    24758 2023-04-10 15:41:10.000000 srsgui-0.2.9/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.9/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.9/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3330 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3162 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.2.16/.gitignore` & `srsgui-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/LICENSE.txt` & `srsgui-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/PKG-INFO` & `srsgui-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.16
+Version: 0.2.9
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.16/README.md` & `srsgui-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/Makefile` & `srsgui-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/make.bat` & `srsgui-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/_static/cg-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/_static/connect-dialog-box-capture.png` & `srsgui-0.2.9/docs/source/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/_static/example-screen-capture-1.png` & `srsgui-0.2.9/docs/source/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/_static/example-screen-capture-2.png` & `srsgui-0.2.9/docs/source/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/_static/initial-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/_static/second-task-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/_static/terminal-with-example-2.png` & `srsgui-0.2.9/docs/source/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/_static/terminal-with-example.png` & `srsgui-0.2.9/docs/source/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/conf.py` & `srsgui-0.2.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/create-project.rst` & `srsgui-0.2.9/docs/source/create-project.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 
     /Project root directory
         /instruments
         /tasks
         project.taskconfig
 
 A project directory has a .taskconfig configuration file and multiple Python
-modules in two special subdirectory: instruments and tasks.
+modules in two special subdirectory: instruments, tasks.
 Whenever open a .taskconfig file from the SRSGUI application,
-Python modules in those directories will be forced to reload.
+Python modules in those directories are forced to reload.
 
 Typically, a Python interpreter loads a module when it is imported for the first time,
-and never check again if the module is modified. When you make changes to a module, save it,
-and run a script using it, you would not see the changes because the Python interpreter
-would not use the modified module, as long as the previous copy of the module is in memory.
-The Python interpreter needs to restart to take an effect of the changed modules.
+and never check again if the module is modified. When you make changes to a module,
+and import the module again with a Python interpreter, it ignores it
+because it is already imported before. The Python interpreter needs to restart
+to take an effect of the changed modules.
 
 When you open a .taskconfig file again from the ``srsgui`` application,
 it reloads all the Python modules in the 2 subdirectories.
 It helps when you modify and debug a module in the subdirectories.
 Instead of restart the application every time a module is changed,
 you can reopen the .taskconfig file to see the changes from modified modules.
 If you modify a Python module other than the ones in the 2 directories
@@ -70,26 +70,26 @@
 .. code-block::
 
     name: srsgui example project using an oscilloscope and a clock generator
 
     inst: cg,  instruments.cg635,   CG635
     inst: osc, instruments.sds1202, SDS1202
 
-    task: *IDN test,    tasks.first,  FirstTask
+    task: \*IDN test,    tasks.first,  FirstTask
     task: Plot example, tasks.second, SecondTask
     ...
 
 
 The keyword 'name:' is use as
 
     - Title of the SRSGUI application main window (Look at the top of
       this :ref:`screen capture <top-of-screen-capture-1>`.
     - Directory name for the project data saving under ~/home/task-results
 
-You can specify a list of instrument classes to be included in the project using 'inst:' keyword.
+You can specify a list instrument classes to be included in the project using 'inst:' keyword.
 The first column after the keyword is the name of the instrument used across the project:
 
     - Menu items under **Instruments** menu. It is used to connect and disconnect
       the selected instrument.
     - Tab labels in Instrument Info panel (in the top left corner under the red STOP button
       in this :ref:`screen capture <top-of-screen-capture-1>`.
     - Name used in terminal to specify a instrument. Make it short if you use a lot
@@ -132,15 +132,15 @@
 
 The keyword 'task:' is used to specify a task class to be used in the configuration file.
 the first column after the 'task:' keyword is the name of the task,
 the second is path to the module, the third one is the name of the task class.
 It specifies a task class in the same way with instrument classes.
 
 When you open a .taskconfig file, in ``srsgui`` application, the names of the tasks
-appear as menu items under the Task menu, as shown at the top of
+appear as menu items under the Task menu (at the top of
 this :ref:`screen capture <top-of-screen-capture-1>`.
 
 You can select one of the task items and run the task.
 
 
 .. _PyVisa: https://pyvisa.readthedocs.io/en/latest/
 .. _srsinst.sr860: https://pypi.org/project/srsinst.sr860/
```

### Comparing `srsgui-0.2.16/docs/source/create-task.rst` & `srsgui-0.2.9/docs/source/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/define-instrument.rst` & `srsgui-0.2.9/docs/source/define-instrument.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-Defining instrument classes------------------------------an instrument class is a subclass derived from the:class:`Instrument<srsgui.inst.instrument.Instrument>` class.Minimum requirement is to have **_IdString** to check if a connectedinstrument is a correct instrument  that can be used with the class... code-block::    from srsgui import Instrument    class CG635(Instrument):        _IdString = 'CG635'        _term_char = b'\r'  # Add this line if the carriage return is the termination character                            # of the instrument, instead of the line feed (ASCII: 0x10, b'\n').If the instrument has:    1. the **\*IDN?** remote command    2. either RS232 serial communication or Ethernet TCPIP communication port available,the instrument can be connected and used in task scripts and in the terminal,with 4 lines of definition like above. If it does not have the \*IDN? remote command,:meth:`check_id()<srsgui.inst.instrument.Instrument.check_id>` method in Instrumentclass needs to be reimplemented.Available_interfaces^^^^^^^^^^^^^^^^^^^^^`Available_interface` defines what kind of communication is available for the instrument,the base :class:`Instrument<srsgui.inst.instrument.Instrument>` class has the followingdefinition for serial and TCPIP communication interfaces:.. code-block::    available_interfaces = [        [   SerialInterface,            {                'port': FindListInput(),                'baud_rate': IntegerListInput([9600, 115200]),                'hardware_flow_control': BoolInput(['Off', 'On'])            }        ],        [   TcpipInterface,            {                'ip_address': Ip4Input('192.168.1.10'),                'port': IntegerInput(23)            }        ]    ]If your instrument needs other than serial and TCPIP interfaces, ``srsgui`` allows to addother communication classes derived from:class:`Interface <srsgui.inst.communication.interface.Interface>` class.Currently there are two external communication interfaces are available from`srsinst.sr860`_ package: ``Vxi11Interface`` and ``VisaInterface``,which covers for VXI11_, GPIB_ and USB-TMC_. You can import the interface modulesfrom `srsinst.sr860`_ .Available_interfaces in SSR865 class is define as following:.. code-block::    available_interfaces = [        [   Vxi11Interface,            {                'ip_address': Ip4Input('192.168.1.10'),            }        ],        [   VisaInterface,            {                'resource': FindListInput(),            }        ],        [   TcpipInterface,            {                'ip_address': Ip4Input('192.168.1.10'),                'port': 23            }        ],        [   SerialInterface,            {                'port': FindListInput(),                'baud_rate': IntegerListInput([9600, 19200, 38400, 115200,                                               230400, 460800], 3)            }        ],    ]The definition of available_interfaces is all you need to do to get a customizeddialog box opened for the instrument in ``srsgui`` application... figure:: ./_static/connect-dialog-box-capture.png    :align: center    :figclass: align-centerFor ``VisaInterface``, you have to get PyVISA_ working before running ``srsgui`` application.It involves installation of the PyVISA package and its backend library.Refer to PyVISA_ documentation for installation detail.From Python interpreter, you can connect and use a instrument, once its ``Instrument`` class is defined... code-block::    C:\srsgui>python    Python 3.8.3 (tags/v3.8.3:6f8c832, May 13 2020, 22:37:02) [MSC v.1924 64 bit (AMD64)] on win32    Type "help", "copyright", "credits" or "license" for more information.    >>>    >>> from srsinst.sr860 import SR860    >>> from srsgui import SerialInte    >>> SerialInterface.find()    ['COM3', 'COM4', 'COM256']    >>> lia = SR860('serial','COM4',115200, False)    >>> lia.query_text('*idn?')    'Stanford_Research_Systems,SR865A,002725,v1.34'    >>> lia.disconnect()    >>>    >>> from srsinst.sr860 import VisaInterface    >>> VisaInterface.find()    ['USB0::0xB506::0x2000::002725::INSTR', 'GPIB0::4::INSTR']    >>> lia.connect('visa', 'USB0::0xB506::0x2000::002725::INSTR')    >>> lia.query_text('*idn?')    'Stanford_Research_Systems,SR865A,002725,v1.34\n'    >>>Well, these operations are what you can do with PyVISA_ itself. Defining an instrument class,adding it in a .taskconfig file, and opening it in ``srsgui`` application let youuse the terminal to interact with multiple instrument at once, and use high level ``Instrument``class attributes and methods.Below is an image of terminal captured with the example project opened.As you can see, you can interact with the clock generator and oscilloscope in many ways.There are two commands for osc: \*idn?, sara? used, and two commands for cg:\*idn?, freq(?) used in the terminal... figure:: ./_static/terminal-with-example.png    :align: center    :figclass: align-center|Component, Commands and IndexCommands^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^:class:`Instrument <srsgui.inst.instrument.Instrument>` class uses:class:`Component <srsgui.inst.component.Component>` class,:mod:`Command <srsgui.inst.commands>` classes and:mod:`IndexCommand <srsgui.inst.indexcommands>` classesto organize the functionality of an instrument.If you have to deal with hundreds of remote commands to use an instrument remotely,organizing them in a manageable way is crucial. `Srsinst.sr860`_ package shows how theseconvenience classes are used to organize a large set of remote commands... _PyVisa: https://pyvisa.readthedocs.io/en/latest/.. _srsinst.sr860: https://pypi.org/project/srsinst.sr860/.. _VXI11: https://www.lxistandard.org/About/VXI-11-and-LXI.aspx.. _GPIB: https://en.wikipedia.org/wiki/IEEE-488.. _USB-TMC: https://www.testandmeasurementtips.com/remote-communication-with-usbtmc-faq/.. _thread: https://realpython.com/intro-to-python-threading/.. _QThread: https://doc.qt.io/qt-6/qthread.html
+Defining instrument classes------------------------------an instrument class is a subclass derived from the:class:`Instrument<srsgui.inst.instrument.Instrument>` class.Minimum requirement is to have **_IdString** to check if a connectedinstrument is a correct instrument  that can be used with the class... code-block::    from srsgui import Instrument    class CG635(Instrument):        _IdString = 'CG635'        _term_char = b'\r'  # Add this line if the carriage return is the termination character                            # of the instrument, instead of the line feed (ASCII: 0x10, b'\n').If the instrument has:    1. the **\*IDN?** remote command    2. either RS232 serial communication or Ethernet TCPIP communication port available,the instrument can be connected and used in task scripts and in the terminal,with 4 lines of definition like above. If it does not have the \*IDN? remote command,:meth:`check_id()<srsgui.inst.instrument.Instrument.check_id>` method in Instrumentclass needs to be reimplemented.Available_interfaces^^^^^^^^^^^^^^^^^^^^^`Available_interface` defines what kind of communication is available for the instrument,the base :class:`Instrument<srsgui.inst.instrument.Instrument>` class has the followingdefinition for serial and TCPIP communication interfaces:.. code-block::    available_interfaces = [        [   SerialInterface,            {                'port': FindListInput(),                'baud_rate': IntegerListInput([9600, 115200]),                'hardware_flow_control': BoolInput(['Off', 'On'])            }        ],        [   TcpipInterface,            {                'ip_address': Ip4Input('192.168.1.10'),                'port': IntegerInput(23)            }        ]    ]If your instrument needs other than serial and TCPIP interfaces, ``srsgui`` allows to addother communication classes derived from:class:`Interface <srsgui.inst.communication.interface.Interface>` class.Currently there are two external communication interfaces are available from`srsinst.sr860`_ package: ``Vxi11Interface`` and ``VisaInterface``,which covers for VXI11_, GPIB_ and USB-TMC_. You can import the interface modulesfrom `srsinst.sr860`_ .Available_interfaces in SSR865 class is define as following:.. code-block::    available_interfaces = [        [   Vxi11Interface,            {                'ip_address': Ip4Input('192.168.1.10'),            }        ],        [   VisaInterface,            {                'resource': FindListInput(),            }        ],        [   TcpipInterface,            {                'ip_address': Ip4Input('192.168.1.10'),                'port': 23            }        ],        [   SerialInterface,            {                'port': FindListInput(),                'baud_rate': IntegerListInput([9600, 19200, 38400, 115200,                                               230400, 460800], 3)            }        ],    ]The definition of available_interfaces is all you need to do to get a customizeddialog box opened for the instrument in ``srsgui`` application... figure:: ./_static/connect-dialog-box-capture.png    :align: center    :figclass: align-centerFor ``VisaInterface``, you have to get PyVISA_ working before running ``srsgui`` application.It involves installation of the PyVISA package and its backend library.Refer to PyVISA_ documentation for installation detail.From Python interpreter, you can connect and use a instrument, once its ``Instrument`` class is defined... code-block::    C:\srsgui>python    Python 3.8.3 (tags/v3.8.3:6f8c832, May 13 2020, 22:37:02) [MSC v.1924 64 bit (AMD64)] on win32    Type "help", "copyright", "credits" or "license" for more information.    >>>    >>> from srsinst.sr860 import SR865    >>> from srsgui import SerialInte    >>> SerialInterface.find()    ['COM3', 'COM4', 'COM256']    >>> lia = SR865('serial','COM4',115200, False)    >>> lia.query_text('*idn?')    'Stanford_Research_Systems,SR865A,002725,v1.34'    >>> lia.disconnect()    >>>    >>> from srsinst.sr860 import VisaInterface    >>> VisaInterface.find()    ['USB0::0xB506::0x2000::002725::INSTR', 'GPIB0::4::INSTR']    >>> lia.connect('visa', 'USB0::0xB506::0x2000::002725::INSTR')    >>> lia.query_text('*idn?')    'Stanford_Research_Systems,SR865A,002725,v1.34\n'    >>>Well, these operations are what you can do with PyVISA_ itself. Defining an instrument class,adding it in a .taskconfig file, and opening it in ``srsgui`` application let youuse the terminal to interact with multiple instrument at once, and use high level ``Instrument``class attributes and methods.Below is an image of terminal captured with the example project opened.As you can see, you can interact with the clock generator and oscilloscope in many ways.There are two commands for osc: \*idn?, sara? used, and two commands for cg:\*idn?, freq(?) used in the terminal... figure:: ./_static/terminal-with-example.png    :align: center    :figclass: align-center|Component, Commands and IndexCommands^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^:class:`Instrument <srsgui.inst.instrument.Instrument>` class uses:class:`Component <srsgui.inst.component.Component>` class,:mod:`Command <srsgui.inst.commands>` classes and:mod:`IndexCommand <srsgui.inst.indexcommands>` classesto organize the functionality of an instrument.If you have to deal with hundreds of remote commands to use an instrument remotely,organizing them in a manageable way is crucial. `Srsinst.sr860`_ package shows how theseconvenience classes are used to organize a large set of remote commands... _PyVisa: https://pyvisa.readthedocs.io/en/latest/.. _srsinst.sr860: https://pypi.org/project/srsinst.sr860/.. _VXI11: https://www.lxistandard.org/About/VXI-11-and-LXI.aspx.. _GPIB: https://en.wikipedia.org/wiki/IEEE-488.. _USB-TMC: https://www.testandmeasurementtips.com/remote-communication-with-usbtmc-faq/.. _thread: https://realpython.com/intro-to-python-threading/.. _QThread: https://doc.qt.io/qt-6/qthread.html
```

### Comparing `srsgui-0.2.16/docs/source/example.rst` & `srsgui-0.2.9/docs/source/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/index.rst` & `srsgui-0.2.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/installation.rst` & `srsgui-0.2.9/docs/source/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         python -m pip show pyqt5
 
     will show if pyside2_ or pyqt5_ is installed.
 
 .. note::
     In order to maintain the MIT_ license for your projects or modified ``srsgui``, you have to use
-    pyside6_ or pyside2_. Note that pyqt5_ imposes GPLv3_ license to packages using pyqt5_.
+    pyside6_ or pyside2_. Note that GPLv3_ is the license requirement of pyqt5_.
 
 Running srsgui application
 ----------------------------
 
 After ``srsgui`` is installed, you can start ``srsgui`` application from the command line
 
 .. code-block::
@@ -101,15 +101,15 @@
 
 If you see the application is open and running, the installation is successful!
 
 .. note::
     Instead of seeing the application running, you may get errors, probably ImportError.
     Carefully look through the exception traceback to find out which package causes the error.
     When the latest python is installed, some packages may not install properly. If the problem
-    is not from ``srsgui`` directly, web search of the problem usually leads to a fix.
+    is not from ``srsgui`` directly, web search of the problem usually finds a fix.
 
 
 .. _install-packages: https://packaging.python.org/en/latest/tutorials/installing-packages/
 .. _install-python: https://realpython.com/installing-python/
 .. _virtual-environment: https://realpython.com/python-virtual-environments-a-primer/
 .. _venv: https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/
 .. _pip: https://realpython.com/what-is-pip/
```

### Comparing `srsgui-0.2.16/docs/source/srsgui.inst.communications.rst` & `srsgui-0.2.9/docs/source/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/srsgui.inst.rst` & `srsgui-0.2.9/docs/source/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/srsgui.task.rst` & `srsgui-0.2.9/docs/source/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/docs/source/srsgui.ui.qt.rst` & `srsgui-0.2.9/docs/source/srsgui.ui.qt.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+srsgui.ui.qt package~
+======================
 
 .. automodule:: srsgui.ui.qt
    :members:
    :undoc-members:
    :show-inheritance:
 
 srsgui.ui.qt.QtCore module
```

### Comparing `srsgui-0.2.16/docs/source/srsgui.ui.rst` & `srsgui-0.2.9/docs/source/srsgui.ui.rst`

 * *Files 11% similar despite different names*

```diff
@@ -71,23 +71,14 @@
 -----------------------
 
 .. automodule:: srsgui.ui.stdout
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree package
-------------------------------
-
-.. toctree::
-   :maxdepth: 4
-
-   srsgui.ui.commandtree.rst
-
-
 srsgui.ui.qt package
 ----------------------
 
 .. toctree::
    :maxdepth: 4
 
    srsgui.ui.qt.rst
```

### Comparing `srsgui-0.2.16/pyproject.toml` & `srsgui-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,23 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering"
 ]
 dependencies = [
-    "pyserial >= 3",
+    "pyserial>=3",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "srsgui.__version__"}
 
 [project.optional-dependencies]
-full = ['matplotlib >= 3.6.2', 'pyside6 != 6.5.0']
+full = ['matplotlib>=3.6.2', 'pyside6!=6.5.0']
+
 
 [project.scripts]
 srsgui = "srsgui.__main__:main"
 
 # ... other project metadata fields as specified in:
 #     https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
```

### Comparing `srsgui-0.2.16/srsgui/__init__.py` & `srsgui-0.2.9/srsgui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.2.16"  # Global version number
+__version__ = "0.2.9"  # Global version number
```

### Comparing `srsgui-0.2.16/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/inst/__init__.py` & `srsgui-0.2.9/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/inst/commands.py` & `srsgui-0.2.9/srsgui/inst/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,28 +73,25 @@
 
     def __get__(self, instance, instance_type):
         if instance is None:
             return self
         query_string = self._get_command_format.format(self.remote_command)
         reply = None
         try:
-            reply = instance.comm.query_text(query_string).strip()
+            reply = instance.comm.query_text(query_string)
             if callable(self._get_convert_function):
                 self._value = self._get_convert_function(reply)
 
             else:
                 self._value = reply
         except InstCommunicationError:
             raise InstQueryError('Error during querying: CMD: {}'.format(query_string))
         except ValueError:
-            if reply:
-                raise InstQueryError('Error during conversion CMD: {} Reply: {}, Hex:{}'
-                                     .format(query_string, reply, (*map(hex, reply.encode('ascii')),)))
-            else:
-                raise InstQueryError('CMD: {} returned "{}"'.format(query_string, reply))
+            raise InstQueryError('Error during conversion CMD: {} Reply: {}'
+                                 .format(query_string, reply))
         return self._value
 
     def __set__(self, instance, value):
         if instance is None:
             return
 
         try:
@@ -215,15 +212,15 @@
 
 class FloatCommand(Command):
     """
     Descriptor for a remote command to
     **set** and **query** a **float** value
     """
 
-    def __init__(self, remote_command_name, unit='', min=-1e6, max=1e6, step=1e-9,
+    def __init__(self, remote_command_name, unit='', min=-1000.0, max=1000.0, step=0.1,
                  significant_figures=4, default_value=None):
         super().__init__(remote_command_name, default_value)
         self._get_convert_function = float
 
         self.unit = unit
         self.maximum = max
         self.minimum = min
```

### Comparing `srsgui-0.2.16/srsgui/inst/communications/interface.py` & `srsgui-0.2.9/srsgui/inst/communications/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,23 +125,14 @@
         Use send instead.
 
         :param cmd: a string of command that will be internally converted to bytes
         :return: None
         """
         raise NotImplementedError
 
-    def _write_binary(self, binary_array: bytes):
-        """
-        Send an array of bytes over an interface without the lock.
-        It does not append the termination character at the end of the array.
-
-        :return: None
-        """
-        raise NotImplementedError
-
     def _recv(self):
         """
         Receive a reply up to the termination character over an interface without the lock.
         It should be implemented in subclasses.
         This is a protected method that a user should not call directly,
         because it is not thread-safe.  Use recv instead.
```

### Comparing `srsgui-0.2.16/srsgui/inst/communications/serial_ports.py` & `srsgui-0.2.9/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/inst/communications/serialinterface.py` & `srsgui-0.2.9/srsgui/inst/communications/serialinterface.py`

 * *Files 8% similar despite different names*

```diff
@@ -136,25 +136,14 @@
         try:
             self._serial.write(bytecmd)
         except (self.port_not_open_error, AttributeError):
             raise InstCommunicationError('Port not open to write')
         except serial.SerialException:
             raise InstCommunicationError("Sending cmd '{}' to port '{}' failed".format(cmd, self._port))
 
-    def _write_bibary(self, binary_array):
-        if type(binary_array) not in (bytes, bytearray):
-            raise TypeError('_write_binary requires bytes or bytearray')
-        try:
-            self._serial.write(binary_array)
-        except (self.port_not_open_error, AttributeError):
-            raise InstCommunicationError('Port not open to write')
-        except serial.SerialException:
-            raise InstCommunicationError("writing binary '{}' to port '{}' failed".format(
-                (*map(hex, binary_array),), self._port))
-
     def _recv(self):
         """
         Receive a reply over serial interface without the lock.
         This is a protected method that a user should not call directly,
         because it is not thread-safe. Use recv instead.
 
         :return: bytes. It should be converted to string explicitly
```

### Comparing `srsgui-0.2.16/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.2.9/srsgui/inst/communications/tcpipinterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,23 +50,14 @@
 
         try:
             self.socket.sendall(byte_cmd)
         except OSError:
             raise InstCommunicationError("Sending cmd '{}' to IP address: '{}' failed"
                                          .format(cmd, self._ip_address))
 
-    def _write_binary(self, binary_array):
-        if type(binary_array) not in (bytes, bytearray):
-            raise TypeError('_write_binary requires bytes or bytearray')
-        try:
-            self.socket.sendall(binary_array)
-        except OSError:
-            raise InstCommunicationError("Writing binary '{}' to IP address: '{}' failed"
-                                         .format((*map(hex, binary_array),), self._ip_address))
-
     def _recv(self):
         """
         Receive a reply over TCP/IP without the lock.
         This is a protected method that a user should not call directly,
         because it is not thread-safe.  Use recv instead.
 
         :return: bytes. It should be converted to string explicitly
```

### Comparing `srsgui-0.2.16/srsgui/inst/component.py` & `srsgui-0.2.9/srsgui/inst/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,14 @@
 
     def is_connected(self):
         """
         check if the current communication interface is open
         """
         return self.comm.is_connected()
 
-    def parent(self):
-        return self._parent
-
     def set_name(self, name):
         """
         Set the name of the component
         """
         self._name = name
 
     def get_name(self):
```

### Comparing `srsgui-0.2.16/srsgui/inst/exceptions.py` & `srsgui-0.2.9/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/inst/indexcommands.py` & `srsgui-0.2.9/srsgui/inst/indexcommands.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,31 +86,27 @@
     def __set__(self, instance, value):
         raise InstSetError('No set for IndexCommand for {}'
                            .format(self.remote_command))
 
     def __getitem__(self, index):
         converted_index = self._convert_index(index)
         query_string = '{}? {}'.format(self.remote_command, converted_index)
-        reply = None
         value = None
         try:
             reply = self._parent.comm.query_text(query_string)
             if callable(self._get_convert_function):
                 value = self._get_convert_function(reply)
 
             else:
                 value = reply
         except InstCommunicationError:
             raise InstQueryError('Error during querying: CMD: {}'.format(query_string))
         except ValueError:
-            if reply:
-                raise InstQueryError('Error during conversion CMD: {} Reply: {}, Hex:{}'
-                                     .format(query_string, reply, (*map(hex, reply.encode('ascii')),)))
-            else:
-                raise InstQueryError('CMD: {} returned "{}"'.format(query_string, reply))
+            raise InstQueryError('Error during conversion CMD: {} Reply: {}'
+                                 .format(query_string, reply))
         return value
 
     def __setitem__(self, index, value):
         converted_index = self._convert_index(index)
         set_string = '{} {}, '.format(self.remote_command, converted_index)
         try:
             if callable(self._set_convert_function):
@@ -203,28 +199,27 @@
 
 class IntIndexGetCommand(IntIndexCommand):
     """
     Command class for a remote command with index
     using only **query** returning an **integer**, without **set**.
     """
     _set_enable = False
-
     def __setitem__(self, instance, value):
         raise InstIndexError('No set allowed for index command {}'
                              .format(self.remote_command))
 
 
 class FloatIndexCommand(IndexCommand):
     """
     Command class for a remote command with index
     using **set** and **query** returning an **float**
     """
 
     def __init__(self, remote_command_name, index_max, index_min=0, index_dict=None,
-                 unit='', value_min=-1e6, value_max=1e6, step=1e-9, significant_figures=4, default_valaue=0.0 ):
+                 unit='', value_min=-1e6, value_max=1e6, step=0.1, significant_figures=4, default_valaue=0.0 ):
         super().__init__(remote_command_name, index_max, index_min, index_dict)
         self._get_convert_function = float
 
         self.unit = unit
         self.maximum = value_max
         self.minimum = value_min
         self.step = step
```

### Comparing `srsgui-0.2.16/srsgui/inst/instrument.py` & `srsgui-0.2.9/srsgui/inst/instrument.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/task/callbacks.py` & `srsgui-0.2.9/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/task/config.py` & `srsgui-0.2.9/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/task/inputs.py` & `srsgui-0.2.9/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/task/sessionhandler.py` & `srsgui-0.2.9/srsgui/task/sessionhandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 
 import json
 import logging
 from pathlib import Path
 from datetime import datetime
 
+# from wip.local_results import LocalClient
+# from wip.wip_api import DutNotRegisteredError
+
 from srsgui.task.taskresult import TaskResult
 
 RedBold = '<font color="red"><b>{}</b></font>'
 logger = logging.getLogger(__name__)
 
+logging.getLogger('urllib3').setLevel(logging.WARNING)
+
 
 class SessionHandler(object):
     def __init__(self, use_file=False, use_db=False, use_api=False):
         self.use_file = False
         self.use_db = False
         self.use_api = False
         self._is_session_open = False
```

### Comparing `srsgui-0.2.16/srsgui/task/task.py` & `srsgui-0.2.9/srsgui/task/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             self._keep_running = False
 
     def delay(self, seconds):
         """
         Check if the task is stopped and wait for the given seconds.
         """
         if not self._keep_running:
-            raise Task.TaskException('Task is requested to stop')
+            raise KeyboardInterrupt('Task is stopped')
         else:
             time.sleep(seconds)
 
     def set_session_handler(self, session_handler):
         """
         Parent should set a session handler for Task to use file output.
         """
@@ -350,15 +350,15 @@
     def clear_figures(self):
         """
         Clear all the figures in figure_dict
         """
         for fig in self.figure_dict.values():
             if hasattr(fig, 'canvas'):
                 fig.clear()
-                self.request_figure_update(fig)
+                self.request_figure_update()
 
     def is_running(self):
         """
         Task should check is_running() is True.
         If it returns False, Task should stop ASAP.
         """
         return self._keep_running
@@ -512,18 +512,24 @@
             raise TypeError('{} is not  a Figure'.format(type(figure)))
         self.callbacks.figure_update_requested(figure)
 
     # It needs a matching update() as a slot to run from UI
     def notify_data_available(self, data={}):
         self.callbacks.data_available(data)
 
+    # These callbacks are used to update display for streaming data from another class or thread
+    # Signals are wrapped as a callback functions 
+
+    def data_available_callback(self, data={}, *args):
+        self.callbacks.data_available(data)
+
     def update(self, data: dict):
         """
-        when notify_data_available is called, this method handles data processing
-        and display update. By default, it does no data handling, but figure update request.
+        when data_available signal emits, this method handles display update.
+        By default, it does no data handling, but figure update request.
         GUI related data processing needs to be done here to be handled
         in proper order by the GUI event loop handler.
         """
         self.request_figure_update()
 
     def get_instrument(self, name):
         """Get an instrument from parent's inst_dict and check its validity"""
```

### Comparing `srsgui-0.2.16/srsgui/task/taskresult.py` & `srsgui-0.2.9/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/commandhandler.py` & `srsgui-0.2.9/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/commandterminal.py` & `srsgui-0.2.9/srsgui/ui/commandterminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,10 @@
             self.command_requested.emit(cmd, '')
 
         except Exception as e:
             self.tbCommand.append('Error: {}'.format(str(e)))
 
     def handle_command(self, cmd, reply):
         try:
-            if reply:
-                self.tbCommand.append(f'{cmd}   ==>   {reply}')
-            else:
-                self.tbCommand.append(f'{cmd}')
-
+            self.tbCommand.append(f'{cmd}  :  {reply}')
         except Exception as e:
             self.tbCommand.append('Error from CommandTerminal: {}'.format(str(e)))
```

### Comparing `srsgui-0.2.16/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commanddelegate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-import logging
 
 from srsgui.ui.qt.QtCore import Qt
 from srsgui.ui.qt.QtWidgets import QStyledItemDelegate, QComboBox
 
 from srsgui.inst import DictCommand, FloatCommand, IntCommand, \
                         FloatIndexCommand, IntIndexCommand, DictIndexCommand
 
 from .commandspinbox import FloatSpinBox, IntegerSpinBox
 from .commanditem import Index
 
-logger = logging.getLogger(__file__)
-
 
 class CommandDelegate(QStyledItemDelegate):
     """ A custom delegate for editing CommandItem """
     def __init__(self, parent=None):
         super().__init__(parent)
 
     def createEditor(self, parent, option, index):
@@ -22,80 +19,75 @@
         if item.comp_type == Index:
             comp = item.parent().comp
             comp_type = item.parent().comp_type
         else:
             comp = item.comp
             comp_type = item.comp_type
 
-        if issubclass(comp_type, FloatCommand) or issubclass(comp_type, FloatIndexCommand):
+        if comp_type in (FloatCommand, FloatIndexCommand):
             editor = FloatSpinBox(parent)
             editor.setDecimals(10)
             editor.setSingleStep(0.1)
             editor.setMinimum(comp.minimum)
             editor.setMaximum(comp.maximum)
-            editor.setSuffix(' ' + comp.unit)
+            editor.setSuffix(comp.unit)
             editor.set_significant_figures(comp.significant_figures)
             editor.set_minimum_step(comp.step)
             return editor
 
-        elif issubclass(comp_type, IntCommand) or issubclass(comp_type, IntIndexCommand):
+        elif comp_type in (IntCommand, IntIndexCommand):
             editor = IntegerSpinBox(parent)
             editor.setMinimum(comp.minimum)
             editor.setMaximum(comp.maximum)
-            editor.setSuffix(' ' + comp.unit)
+            editor.setSuffix(comp.unit)
             return editor
 
         elif comp_type in (DictCommand, DictIndexCommand):
             editor = QComboBox(parent)
             for key in comp.set_dict.keys():
                 editor.addItem(str(key))
             return editor
 
         else:
             return super().createEditor(parent, option, index)
 
     def setEditorData(self, editor, index):
-
         if type(editor) in (FloatSpinBox, IntegerSpinBox):
             item = index.internalPointer()
             val = index.model().data(index, Qt.EditRole)
             editor.setValue(val)
 
         elif type(editor) == QComboBox:
             item = index.internalPointer()
             val = index.model().data(index, Qt.EditRole)
             editor.setCurrentText(str(val))
         return super().setEditorData(editor, index)
 
     def setModelData(self, editor, model, index):
+        item = index.internalPointer()
+        if item.comp_type == Index:
+            comp = item.parent().comp
+            comp_type = item.parent().comp_type
+        else:
+            comp = item.comp
+            comp_type = item.comp_type
 
-        try:
-            item = index.internalPointer()
-            if item.comp_type == Index:
-                comp = item.parent().comp
-                comp_type = item.parent().comp_type
-            else:
-                comp = item.comp
-                comp_type = item.comp_type
-
-            if issubclass(comp_type, FloatCommand) or issubclass(comp_type, FloatIndexCommand):
-                value = editor.value()
-                model.setData(index, value, Qt.EditRole)
-                item.precision = editor.precision
-            elif issubclass(comp_type, IntCommand) or issubclass(comp_type, IntIndexCommand):
-                pass
-
-                value = editor.value()
-                model.setData(index, value, Qt.EditRole)
-            elif comp_type in (DictCommand, DictIndexCommand):
-                val = editor.currentText()
-                convert = type(list(comp.get_dict.keys())[0])
-                value = convert(val)
-                model.setData(index, value, Qt.EditRole)
-            else:
-                return super().setModelData(editor, model, index)
-        except Exception as e:
-            logger.error(e)
+        if comp_type in (FloatCommand, FloatIndexCommand):
+            value = editor.value()
+            model.setData(index, value, Qt.EditRole)
+            item.precision = editor.precision
+            return True
+        elif comp_type in (IntCommand, IntIndexCommand):
+            value = editor.value()
+            model.setData(index, value, Qt.EditRole)
+            return True
+        elif comp_type in (DictCommand, DictIndexCommand):
+            val = editor.currentText()
+            convert = type(list(comp.get_dict.keys())[0])
+            value = convert(val)
+            model.setData(index, value, Qt.EditRole)
+            return True
+        return super().setModelData(editor, model, index)
 
     def updateEditorGeometry(self, editor, option, index):
         return super().updateEditorGeometry(editor, option, index)
```

### Comparing `srsgui-0.2.16/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commanditem.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,746 +1,637 @@
-00000000: 0d0a 696d 706f 7274 2074 696d 650d 0a69  ..import time..i
-00000010: 6d70 6f72 7420 6d61 7468 0d0a 0d0a 6672  mport math....fr
-00000020: 6f6d 2073 7273 6775 6920 696d 706f 7274  om srsgui import
-00000030: 2043 6f6d 706f 6e65 6e74 0d0a 6672 6f6d   Component..from
-00000040: 2073 7273 6775 692e 696e 7374 2069 6d70   srsgui.inst imp
-00000050: 6f72 7420 436f 6d6d 616e 642c 2049 6e64  ort Command, Ind
-00000060: 6578 436f 6d6d 616e 642c 205c 0d0a 2020  exCommand, \..  
-00000070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000080: 2020 2020 2020 466c 6f61 7443 6f6d 6d61        FloatComma
-00000090: 6e64 2c20 466c 6f61 7449 6e64 6578 436f  nd, FloatIndexCo
-000000a0: 6d6d 616e 640d 0a0d 0a0d 0a63 6c61 7373  mmand......class
-000000b0: 2049 6e64 6578 3a0d 0a20 2020 2070 6173   Index:..    pas
-000000c0: 730d 0a0d 0a0d 0a63 6c61 7373 2043 6f6d  s......class Com
-000000d0: 6d61 6e64 4974 656d 3a0d 0a20 2020 2022  mandItem:..    "
-000000e0: 2222 0d0a 2020 2020 436f 6d6d 616e 6420  ""..    Command 
-000000f0: 6974 656d 2063 6f72 7265 7370 6f6e 6469  item correspondi
-00000100: 6e67 2074 6f20 6120 6c69 6e65 2069 6e20  ng to a line in 
-00000110: 5154 7265 6556 6965 772e 2049 7420 656e  QTreeView. It en
-00000120: 6361 7073 756c 6174 6573 0d0a 2020 2020  capsulates..    
-00000130: 436f 6d70 6f6e 656e 742c 2043 6f6d 6d61  Component, Comma
-00000140: 6e64 2c20 616e 6420 496e 6465 7820 636c  nd, and Index cl
-00000150: 6173 7320 7573 6564 2069 6e20 7372 7367  ass used in srsg
-00000160: 7569 2e49 6e73 7472 756d 656e 7420 636c  ui.Instrument cl
-00000170: 6173 732e 0d0a 2020 2020 2222 220d 0a0d  ass...    """...
-00000180: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00000190: 5f28 7365 6c66 2c20 7061 7265 6e74 3a20  _(self, parent: 
-000001a0: 2243 6f6d 6d61 6e64 4974 656d 2220 3d20  "CommandItem" = 
-000001b0: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
-000001c0: 7365 6c66 2e5f 7061 7265 6e74 203d 2070  self._parent = p
-000001d0: 6172 656e 740d 0a20 2020 2020 2020 2073  arent..        s
-000001e0: 656c 662e 5f63 6869 6c64 7265 6e20 3d20  elf._children = 
-000001f0: 5b5d 0d0a 2020 2020 2020 2020 7365 6c66  []..        self
-00000200: 2e5f 7661 6c75 6520 3d20 4e6f 6e65 0d0a  ._value = None..
-00000210: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00000220: 2020 7365 6c66 2e6e 616d 6520 3d20 2222    self.name = ""
-00000230: 0d0a 2020 2020 2020 2020 7365 6c66 2e76  ..        self.v
-00000240: 616c 7565 5f74 7970 6520 3d20 4e6f 6e65  alue_type = None
-00000250: 2020 2320 5468 6572 6520 6172 6520 3320    # There are 3 
-00000260: 7479 7065 7320 6f66 2076 616c 7565 733a  types of values:
-00000270: 2073 7472 2c20 696e 742c 2061 6e64 2066   str, int, and f
-00000280: 6c6f 6174 0d0a 0d0a 2020 2020 2020 2020  loat....        
-00000290: 7365 6c66 2e63 6f6d 7020 3d20 4e6f 6e65  self.comp = None
-000002a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-000002b0: 6f6d 705f 7479 7065 203d 204e 6f6e 6520  omp_type = None 
-000002c0: 2020 2320 5468 6572 6520 6172 6520 3520    # There are 5 
-000002d0: 7479 7065 7320 6f66 2063 6f6d 706f 6e65  types of compone
-000002e0: 6e74 733a 2043 6f6d 706f 6e65 6e74 2c20  nts: Component, 
-000002f0: 436f 6d6d 616e 6473 2c20 496e 6465 7843  Commands, IndexC
-00000300: 6f6d 6d61 6e64 732c 206d 6574 686f 6420  ommands, method 
-00000310: 616e 6420 496e 6465 780d 0a20 2020 2020  and Index..     
-00000320: 2020 2073 656c 662e 7365 745f 656e 6162     self.set_enab
-00000330: 6c65 203d 2046 616c 7365 0d0a 2020 2020  le = False..    
-00000340: 2020 2020 7365 6c66 2e67 6574 5f65 6e61      self.get_ena
-00000350: 626c 6520 3d20 4661 6c73 650d 0a20 2020  ble = False..   
-00000360: 2020 2020 2073 656c 662e 6973 5f6d 6574       self.is_met
-00000370: 686f 6420 3d20 4661 6c73 650d 0a20 2020  hod = False..   
-00000380: 2020 2020 2073 656c 662e 6578 636c 7564       self.exclud
-00000390: 6564 203d 2046 616c 7365 0d0a 2020 2020  ed = False..    
-000003a0: 2020 2020 7365 6c66 2e72 6177 5f72 656d      self.raw_rem
-000003b0: 6f74 655f 636f 6d6d 616e 6420 3d20 2222  ote_command = ""
-000003c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-000003d0: 696d 6573 7461 6d70 203d 2030 2e30 0d0a  imestamp = 0.0..
-000003e0: 2020 2020 2020 2020 7365 6c66 2e71 7565          self.que
-000003f0: 7279 5f75 7064 6174 655f 7065 7269 6f64  ry_update_period
-00000400: 203d 2030 2e33 0d0a 0d0a 2020 2020 6465   = 0.3....    de
-00000410: 6620 6170 7065 6e64 4368 696c 6428 7365  f appendChild(se
-00000420: 6c66 2c20 6974 656d 3a20 2243 6f6d 6d61  lf, item: "Comma
-00000430: 6e64 4974 656d 2229 3a0d 0a20 2020 2020  ndItem"):..     
-00000440: 2020 2022 2222 4164 6420 6974 656d 2061     """Add item a
-00000450: 7320 6120 6368 696c 6422 2222 0d0a 2020  s a child"""..  
-00000460: 2020 2020 2020 7365 6c66 2e5f 6368 696c        self._chil
-00000470: 6472 656e 2e61 7070 656e 6428 6974 656d  dren.append(item
-00000480: 290d 0a0d 0a20 2020 2064 6566 2063 6869  )....    def chi
-00000490: 6c64 2873 656c 662c 2072 6f77 3a20 696e  ld(self, row: in
-000004a0: 7429 202d 3e20 2243 6f6d 6d61 6e64 4974  t) -> "CommandIt
-000004b0: 656d 223a 0d0a 2020 2020 2020 2020 2222  em":..        ""
-000004c0: 2252 6574 7572 6e20 7468 6520 6368 696c  "Return the chil
-000004d0: 6420 6f66 2074 6865 2063 7572 7265 6e74  d of the current
-000004e0: 2069 7465 6d20 6672 6f6d 2074 6865 2067   item from the g
-000004f0: 6976 656e 2072 6f77 2222 220d 0a20 2020  iven row"""..   
-00000500: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00000510: 2e5f 6368 696c 6472 656e 5b72 6f77 5d0d  ._children[row].
-00000520: 0a0d 0a20 2020 2064 6566 2070 6172 656e  ...    def paren
-00000530: 7428 7365 6c66 2920 2d3e 2022 436f 6d6d  t(self) -> "Comm
-00000540: 616e 6449 7465 6d22 3a0d 0a20 2020 2020  andItem":..     
-00000550: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
-00000560: 2070 6172 656e 7420 6f66 2074 6865 2063   parent of the c
-00000570: 7572 7265 6e74 2069 7465 6d22 2222 0d0a  urrent item"""..
-00000580: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00000590: 656c 662e 5f70 6172 656e 740d 0a0d 0a20  elf._parent.... 
-000005a0: 2020 2064 6566 2063 6869 6c64 436f 756e     def childCoun
-000005b0: 7428 7365 6c66 2920 2d3e 2069 6e74 3a0d  t(self) -> int:.
-000005c0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-000005d0: 726e 2074 6865 206e 756d 6265 7220 6f66  rn the number of
-000005e0: 2063 6869 6c64 7265 6e20 6f66 2074 6865   children of the
-000005f0: 2063 7572 7265 6e74 2069 7465 6d22 2222   current item"""
-00000600: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000610: 206c 656e 2873 656c 662e 5f63 6869 6c64   len(self._child
-00000620: 7265 6e29 0d0a 0d0a 2020 2020 6465 6620  ren)....    def 
-00000630: 726f 7728 7365 6c66 2920 2d3e 2069 6e74  row(self) -> int
-00000640: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
-00000650: 7475 726e 2074 6865 2072 6f77 2077 6865  turn the row whe
-00000660: 7265 2074 6865 2063 7572 7265 6e74 2069  re the current i
-00000670: 7465 6d20 6f63 6375 7069 6573 2069 6e20  tem occupies in 
-00000680: 7468 6520 7061 7265 6e74 2222 220d 0a20  the parent""".. 
-00000690: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000006a0: 6c66 2e5f 7061 7265 6e74 2e5f 6368 696c  lf._parent._chil
-000006b0: 6472 656e 2e69 6e64 6578 2873 656c 6629  dren.index(self)
-000006c0: 2069 6620 7365 6c66 2e5f 7061 7265 6e74   if self._parent
-000006d0: 2065 6c73 6520 300d 0a0d 0a20 2020 2040   else 0....    @
-000006e0: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
-000006f0: 6620 7661 6c75 6528 7365 6c66 293a 0d0a  f value(self):..
-00000700: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00000710: 6e20 7468 6520 7661 6c75 6520 6f66 2074  n the value of t
-00000720: 6865 2063 7572 7265 6e74 2069 7465 6d22  he current item"
-00000730: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-00000740: 726e 2073 656c 662e 5f76 616c 7565 0d0a  rn self._value..
-00000750: 0d0a 2020 2020 4076 616c 7565 2e73 6574  ..    @value.set
-00000760: 7465 720d 0a20 2020 2064 6566 2076 616c  ter..    def val
-00000770: 7565 2873 656c 662c 2076 616c 7565 293a  ue(self, value):
-00000780: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00000790: 7661 6c75 6520 3d20 7661 6c75 650d 0a0d  value = value...
-000007a0: 0a20 2020 2064 6566 2071 7565 7279 5f76  .    def query_v
-000007b0: 616c 7565 2873 656c 6629 3a0d 0a20 2020  alue(self):..   
-000007c0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-000007d0: 2020 2020 2020 2074 7320 3d20 7469 6d65         ts = time
-000007e0: 2e74 696d 6528 290d 0a20 2020 2020 2020  .time()..       
-000007f0: 2020 2020 2069 6620 7473 202d 2073 656c       if ts - sel
-00000800: 662e 7469 6d65 7374 616d 7020 3c20 7365  f.timestamp < se
-00000810: 6c66 2e71 7565 7279 5f75 7064 6174 655f  lf.query_update_
-00000820: 7065 7269 6f64 3a20 2023 2044 6f6e 2774  period:  # Don't
-00000830: 2075 7064 6174 6520 746f 6f20 6f66 7465   update too ofte
-00000840: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00000850: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00000860: 7661 6c75 650d 0a0d 0a20 2020 2020 2020  value....       
-00000870: 2020 2020 2069 6620 7365 6c66 2e63 6f6d       if self.com
-00000880: 705f 7479 7065 203d 3d20 496e 6465 7820  p_type == Index 
-00000890: 616e 6420 7365 6c66 2e67 6574 5f65 6e61  and self.get_ena
-000008a0: 626c 6520 616e 6420 6e6f 7420 7365 6c66  ble and not self
-000008b0: 2e65 7863 6c75 6465 643a 0d0a 2020 2020  .excluded:..    
-000008c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000008d0: 2e5f 7661 6c75 6520 3d20 7365 6c66 2e5f  ._value = self._
-000008e0: 7061 7265 6e74 2e63 6f6d 702e 5f5f 6765  parent.comp.__ge
-000008f0: 7469 7465 6d5f 5f28 7365 6c66 2e63 6f6d  titem__(self.com
-00000900: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
-00000910: 2020 2020 7365 6c66 2e76 616c 7565 5f74      self.value_t
-00000920: 7970 6520 3d20 7479 7065 2873 656c 662e  ype = type(self.
-00000930: 5f76 616c 7565 290d 0a20 2020 2020 2020  _value)..       
-00000940: 2020 2020 2020 2020 2073 656c 662e 7469           self.ti
-00000950: 6d65 7374 616d 7020 3d20 7473 0d0a 2020  mestamp = ts..  
-00000960: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
-00000970: 7373 7562 636c 6173 7328 7479 7065 2873  ssubclass(type(s
-00000980: 656c 662e 636f 6d70 292c 2043 6f6d 6d61  elf.comp), Comma
-00000990: 6e64 2920 616e 6420 7365 6c66 2e67 6574  nd) and self.get
-000009a0: 5f65 6e61 626c 6520 616e 6420 6e6f 7420  _enable and not 
-000009b0: 7365 6c66 2e65 7863 6c75 6465 643a 0d0a  self.excluded:..
-000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 7365 6c66 2e5f 7661 6c75 6520 3d20 7365  self._value = se
-000009e0: 6c66 2e63 6f6d 702e 5f5f 6765 745f 5f28  lf.comp.__get__(
-000009f0: 7365 6c66 2e5f 7061 7265 6e74 2e63 6f6d  self._parent.com
-00000a00: 702c 2073 656c 662e 5f70 6172 656e 742e  p, self._parent.
-00000a10: 636f 6d70 2e5f 5f63 6c61 7373 5f5f 290d  comp.__class__).
-00000a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000a30: 2073 656c 662e 7661 6c75 655f 7479 7065   self.value_type
-00000a40: 203d 2074 7970 6528 7365 6c66 2e5f 7661   = type(self._va
-00000a50: 6c75 6529 0d0a 2020 2020 2020 2020 2020  lue)..          
-00000a60: 2020 2020 2020 7365 6c66 2e74 696d 6573        self.times
-00000a70: 7461 6d70 203d 2074 730d 0a20 2020 2020  tamp = ts..     
-00000a80: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00000a90: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-00000aa0: 2020 2020 2020 2070 7269 6e74 2827 5175         print('Qu
-00000ab0: 6572 7920 6572 726f 723a 207b 7d20 7b7d  ery error: {} {}
-00000ac0: 272e 666f 726d 6174 2865 2c20 7365 6c66  '.format(e, self
-00000ad0: 2e6e 616d 6529 290d 0a20 2020 2020 2020  .name))..       
-00000ae0: 2066 696e 616c 6c79 3a0d 0a20 2020 2020   finally:..     
-00000af0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00000b00: 6c66 2e5f 7661 6c75 650d 0a0d 0a20 2020  lf._value....   
-00000b10: 2064 6566 2073 6574 5f76 616c 7565 2873   def set_value(s
-00000b20: 656c 662c 2076 616c 7565 293a 0d0a 2020  elf, value):..  
-00000b30: 2020 2020 2020 2222 2253 6574 2076 616c        """Set val
-00000b40: 7565 2074 6f20 7468 6520 696e 7374 7275  ue to the instru
-00000b50: 6d65 6e74 2061 6e64 2075 7064 6174 6520  ment and update 
-00000b60: 7468 6520 7661 6c75 6520 6f66 2074 6865  the value of the
-00000b70: 2069 7465 6d22 2222 0d0a 2020 2020 2020   item"""..      
-00000b80: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00000b90: 2020 2020 6966 2073 656c 662e 636f 6d70      if self.comp
-00000ba0: 5f74 7970 6520 3d3d 2049 6e64 6578 3a0d  _type == Index:.
-00000bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000bc0: 2073 656c 662e 5f70 6172 656e 742e 636f   self._parent.co
-00000bd0: 6d70 2e5f 5f73 6574 6974 656d 5f5f 2873  mp.__setitem__(s
-00000be0: 656c 662e 636f 6d70 2c20 7661 6c75 6529  elf.comp, value)
-00000bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000c00: 2020 7365 6c66 2e5f 7661 6c75 6520 3d20    self._value = 
-00000c10: 7365 6c66 2e5f 7061 7265 6e74 2e63 6f6d  self._parent.com
-00000c20: 702e 5f5f 6765 7469 7465 6d5f 5f28 7365  p.__getitem__(se
-00000c30: 6c66 2e63 6f6d 7029 0d0a 2020 2020 2020  lf.comp)..      
-00000c40: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00000c50: 696d 6573 7461 6d70 203d 2074 696d 652e  imestamp = time.
-00000c60: 7469 6d65 2829 0d0a 2020 2020 2020 2020  time()..        
-00000c70: 2020 2020 656c 6966 2069 7373 7562 636c      elif issubcl
-00000c80: 6173 7328 7479 7065 2873 656c 662e 636f  ass(type(self.co
-00000c90: 6d70 292c 2043 6f6d 6d61 6e64 293a 0d0a  mp), Command):..
-00000ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cb0: 7365 6c66 2e63 6f6d 702e 5f5f 7365 745f  self.comp.__set_
-00000cc0: 5f28 7365 6c66 2e5f 7061 7265 6e74 2e63  _(self._parent.c
-00000cd0: 6f6d 702c 2076 616c 7565 290d 0a20 2020  omp, value)..   
-00000ce0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00000cf0: 662e 5f76 616c 7565 203d 2073 656c 662e  f._value = self.
-00000d00: 636f 6d70 2e5f 5f67 6574 5f5f 2873 656c  comp.__get__(sel
-00000d10: 662e 5f70 6172 656e 742e 636f 6d70 2c20  f._parent.comp, 
-00000d20: 7365 6c66 2e5f 7061 7265 6e74 2e63 6f6d  self._parent.com
-00000d30: 702e 5f5f 636c 6173 735f 5f29 0d0a 2020  p.__class__)..  
-00000d40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00000d50: 6c66 2e74 696d 6573 7461 6d70 203d 2074  lf.timestamp = t
-00000d60: 696d 652e 7469 6d65 2829 0d0a 2020 2020  ime.time()..    
-00000d70: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00000d80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00000d90: 656c 662e 5f76 616c 7565 203d 2076 616c  elf._value = val
-00000da0: 7565 0d0a 2020 2020 2020 2020 6578 6365  ue..        exce
-00000db0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00000dc0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000dd0: 7072 696e 7428 2753 6574 2065 7272 6f72  print('Set error
-00000de0: 3a20 7b7d 207b 7d27 2e66 6f72 6d61 7428  : {} {}'.format(
-00000df0: 652c 2073 656c 662e 6e61 6d65 2929 0d0a  e, self.name))..
-00000e00: 0d0a 2020 2020 6465 6620 6973 5f65 6469  ..    def is_edi
-00000e10: 7461 626c 6528 7365 6c66 293a 0d0a 2020  table(self):..  
-00000e20: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-00000e30: 5472 7565 2069 6620 7468 6520 6974 656d  True if the item
-00000e40: 2069 7320 6564 6974 6162 6c65 2222 220d   is editable""".
-00000e50: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00000e60: 2e63 6f6d 705f 7479 7065 203d 3d20 496e  .comp_type == In
-00000e70: 6465 7820 616e 6420 5c0d 0a20 2020 2020  dex and \..     
-00000e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000e90: 7365 745f 656e 6162 6c65 2061 6e64 2073  set_enable and s
-00000ea0: 656c 662e 6765 745f 656e 6162 6c65 2061  elf.get_enable a
-00000eb0: 6e64 206e 6f74 2073 656c 662e 6578 636c  nd not self.excl
-00000ec0: 7564 6564 3a0d 0a20 2020 2020 2020 2020  uded:..         
-00000ed0: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
-00000ee0: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
-00000ef0: 7562 636c 6173 7328 7479 7065 2873 656c  ubclass(type(sel
-00000f00: 662e 636f 6d70 292c 2043 6f6d 6d61 6e64  f.comp), Command
-00000f10: 2920 616e 6420 5c0d 0a20 2020 2020 2020  ) and \..       
-00000f20: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00000f30: 745f 656e 6162 6c65 2061 6e64 2073 656c  t_enable and sel
-00000f40: 662e 6765 745f 656e 6162 6c65 2061 6e64  f.get_enable and
-00000f50: 206e 6f74 2073 656c 662e 6578 636c 7564   not self.exclud
-00000f60: 6564 3a0d 0a20 2020 2020 2020 2020 2020  ed:..           
-00000f70: 2072 6574 7572 6e20 5472 7565 0d0a 2020   return True..  
-00000f80: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00000f90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000fa0: 4661 6c73 650d 0a0d 0a20 2020 2064 6566  False....    def
-00000fb0: 2067 6574 5f66 6f72 6d61 7474 6564 5f76   get_formatted_v
-00000fc0: 616c 7565 2873 656c 6629 3a0d 0a20 2020  alue(self):..   
-00000fd0: 2020 2020 2022 2222 5265 7475 726e 2066       """Return f
-00000fe0: 6f72 6d61 7474 6564 2076 616c 7565 206f  ormatted value o
-00000ff0: 6620 6120 666c 6f61 7422 2222 0d0a 0d0a  f a float"""....
-00001000: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-00001010: 7365 6c66 2e76 616c 7565 0d0a 2020 2020  self.value..    
-00001020: 2020 2020 6966 2076 616c 7565 2069 7320      if value is 
-00001030: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00001040: 2020 2072 6574 7572 6e20 4e6f 6e65 0d0a     return None..
-00001050: 0d0a 2020 2020 2020 2020 636f 6d70 203d  ..        comp =
-00001060: 204e 6f6e 650d 0a20 2020 2020 2020 2069   None..        i
-00001070: 6620 7365 6c66 2e63 6f6d 705f 7479 7065  f self.comp_type
-00001080: 203d 3d20 496e 6465 783a 0d0a 2020 2020   == Index:..    
-00001090: 2020 2020 2020 2020 636f 6d70 203d 2073          comp = s
-000010a0: 656c 662e 7061 7265 6e74 2829 2e63 6f6d  elf.parent().com
-000010b0: 700d 0a20 2020 2020 2020 2065 6c69 6620  p..        elif 
-000010c0: 6973 7375 6263 6c61 7373 2874 7970 6528  issubclass(type(
-000010d0: 7365 6c66 2e63 6f6d 7029 2c20 436f 6d6d  self.comp), Comm
-000010e0: 616e 6429 206f 7220 5c0d 0a20 2020 2020  and) or \..     
-000010f0: 2020 2020 2020 2020 6973 7375 6263 6c61          issubcla
-00001100: 7373 2874 7970 6528 7365 6c66 2e63 6f6d  ss(type(self.com
-00001110: 7029 2c20 496e 6465 7843 6f6d 6d61 6e64  p), IndexCommand
-00001120: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00001130: 636f 6d70 203d 2073 656c 662e 636f 6d70  comp = self.comp
-00001140: 0d0a 0d0a 2020 2020 2020 2020 666d 7420  ....        fmt 
-00001150: 3d20 636f 6d70 2e66 6d74 2069 6620 636f  = comp.fmt if co
-00001160: 6d70 2061 6e64 2068 6173 6174 7472 2863  mp and hasattr(c
-00001170: 6f6d 702c 2027 666d 7427 2920 656c 7365  omp, 'fmt') else
-00001180: 2027 270d 0a20 2020 2020 2020 2075 6e69   ''..        uni
-00001190: 7420 3d20 636f 6d70 2e75 6e69 7420 6966  t = comp.unit if
-000011a0: 2063 6f6d 7020 616e 6420 6861 7361 7474   comp and hasatt
-000011b0: 7228 636f 6d70 2c20 2775 6e69 7427 2920  r(comp, 'unit') 
-000011c0: 656c 7365 2027 270d 0a0d 0a20 2020 2020  else ''....     
-000011d0: 2020 2069 6620 636f 6d70 2061 6e64 2028     if comp and (
-000011e0: 6973 7375 6263 6c61 7373 2874 7970 6528  issubclass(type(
-000011f0: 636f 6d70 292c 2046 6c6f 6174 496e 6465  comp), FloatInde
-00001200: 7843 6f6d 6d61 6e64 2920 6f72 0d0a 2020  xCommand) or..  
-00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001220: 2020 2069 7373 7562 636c 6173 7328 7479     issubclass(ty
-00001230: 7065 2863 6f6d 7029 2c20 466c 6f61 7443  pe(comp), FloatC
-00001240: 6f6d 6d61 6e64 2929 3a0d 0a20 2020 2020  ommand)):..     
-00001250: 2020 2020 2020 2069 6620 7661 6c75 6520         if value 
-00001260: 3d3d 2030 2e30 3a0d 0a20 2020 2020 2020  == 0.0:..       
-00001270: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001280: 2730 2720 2b20 6627 207b 756e 6974 7d27  '0' + f' {unit}'
-00001290: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-000012a0: 6570 203d 2063 6f6d 702e 7374 6570 0d0a  ep = comp.step..
-000012b0: 2020 2020 2020 2020 2020 2020 7369 676e              sign
-000012c0: 6966 6963 616e 745f 6669 6775 7265 7320  ificant_figures 
-000012d0: 3d20 636f 6d70 2e73 6967 6e69 6669 6361  = comp.significa
-000012e0: 6e74 5f66 6967 7572 6573 0d0a 0d0a 2020  nt_figures....  
-000012f0: 2020 2020 2020 2020 2020 6465 6369 6d61            decima
-00001300: 6c73 203d 206d 6174 682e 6365 696c 282d  ls = math.ceil(-
-00001310: 6d61 7468 2e6c 6f67 3130 2873 7465 7029  math.log10(step)
-00001320: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-00001330: 6967 6974 7320 3d20 6d61 7468 2e63 6569  igits = math.cei
-00001340: 6c28 6d61 7468 2e6c 6f67 3130 2861 6273  l(math.log10(abs
-00001350: 2876 616c 7565 2929 2920 6966 2076 616c  (value))) if val
-00001360: 7565 2065 6c73 6520 300d 0a20 2020 2020  ue else 0..     
-00001370: 2020 2020 2020 2070 7265 6369 7369 6f6e         precision
-00001380: 203d 206d 696e 2864 6563 696d 616c 732c   = min(decimals,
-00001390: 2073 6967 6e69 6669 6361 6e74 5f66 6967   significant_fig
-000013a0: 7572 6573 202d 2064 6967 6974 7329 0d0a  ures - digits)..
-000013b0: 2020 2020 2020 2020 2020 2020 7072 6563              prec
-000013c0: 6973 696f 6e20 3d20 6d61 7828 7072 6563  ision = max(prec
-000013d0: 6973 696f 6e2c 2030 290d 0a20 2020 2020  ision, 0)..     
-000013e0: 2020 2020 2020 2069 6620 6162 7328 7661         if abs(va
-000013f0: 6c75 6529 203e 3d20 302e 3120 6f72 2070  lue) >= 0.1 or p
-00001400: 7265 6369 7369 6f6e 203c 2073 6967 6e69  recision < signi
-00001410: 6669 6361 6e74 5f66 6967 7572 6573 3a0d  ficant_figures:.
-00001420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001430: 2023 2052 656d 6f76 6520 7472 6169 6c69   # Remove traili
-00001440: 6e67 207a 6572 6f73 2061 6e64 2072 6574  ng zeros and ret
-00001450: 7572 6e0d 0a20 2020 2020 2020 2020 2020  urn..           
-00001460: 2020 2020 2073 203d 2066 277b 7661 6c75       s = f'{valu
-00001470: 653a 2e7b 7072 6563 6973 696f 6e7d 667d  e:.{precision}f}
-00001480: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00001490: 2020 2069 6620 272e 2720 696e 2073 3a0d     if '.' in s:.
-000014a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000014b0: 2020 2020 2072 6574 7572 6e20 732e 7273       return s.rs
-000014c0: 7472 6970 2827 3027 292e 7273 7472 6970  trip('0').rstrip
-000014d0: 2827 2e27 2920 2b20 6627 207b 756e 6974  ('.') + f' {unit
-000014e0: 7d27 0d0a 2020 2020 2020 2020 2020 2020  }'..            
-000014f0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00001500: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00001510: 6574 7572 6e20 7320 2b20 6627 207b 756e  eturn s + f' {un
-00001520: 6974 7d27 0d0a 2020 2020 2020 2020 2020  it}'..          
-00001530: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00001540: 2020 2020 2020 2020 2076 203d 2066 277b           v = f'{
-00001550: 7661 6c75 653a 2e7b 7369 676e 6966 6963  value:.{signific
-00001560: 616e 745f 6669 6775 7265 737d 657d 270d  ant_figures}e}'.
-00001570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001580: 2023 2052 656d 6f76 6520 7472 6169 6c69   # Remove traili
-00001590: 6e67 207a 6572 6f73 2062 6566 6f72 6520  ng zeros before 
-000015a0: 2765 2720 616e 6420 7265 7475 726e 0d0a  'e' and return..
-000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015c0: 7420 3d20 762e 7370 6c69 7428 2765 2729  t = v.split('e')
-000015d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000015e0: 2020 7265 7475 726e 2066 277b 745b 305d    return f'{t[0]
-000015f0: 2e72 7374 7269 7028 2230 2229 2e72 7374  .rstrip("0").rst
-00001600: 7269 7028 222e 2229 7d65 7b74 5b31 5d7d  rip(".")}e{t[1]}
-00001610: 2720 2b20 6627 2020 7b75 6e69 747d 270d  ' + f'  {unit}'.
-00001620: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00001630: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001640: 726e 2066 277b 7661 6c75 653a 7b66 6d74  rn f'{value:{fmt
-00001650: 7d7d 2720 2b20 6627 207b 756e 6974 7d27  }}' + f' {unit}'
-00001660: 0d0a 0d0a 2020 2020 6465 6620 636f 6e73  ....    def cons
-00001670: 7472 7563 745f 7365 745f 636f 6d6d 616e  truct_set_comman
-00001680: 645f 7374 7269 6e67 2873 656c 662c 2076  d_string(self, v
-00001690: 616c 7565 293a 0d0a 2020 2020 2020 2020  alue):..        
-000016a0: 2222 220d 0a20 2020 2020 2020 2043 6f6e  """..        Con
-000016b0: 7374 7275 6374 2070 7974 686f 6e20 636f  struct python co
-000016c0: 6d6d 616e 6420 7374 7269 6e67 2063 6f72  mmand string cor
-000016d0: 7265 7370 6f6e 6469 6e67 2074 6f20 7468  responding to th
-000016e0: 6520 6974 656d 0d0a 2020 2020 2020 2020  e item..        
-000016f0: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-00001700: 662e 6e61 6d65 5f62 7566 6665 7220 3d20  f.name_buffer = 
-00001710: 5b5d 0d0a 2020 2020 2020 2020 7365 6c66  []..        self
-00001720: 2e67 6574 5f6e 616d 655f 7374 7269 6e67  .get_name_string
-00001730: 2873 656c 6629 0d0a 2020 2020 2020 2020  (self)..        
-00001740: 7365 6c66 2e6e 616d 655f 6275 6666 6572  self.name_buffer
-00001750: 2e72 6576 6572 7365 2829 0d0a 2020 2020  .reverse()..    
-00001760: 2020 2020 6966 2074 7970 6528 7661 6c75      if type(valu
-00001770: 6529 2069 7320 7374 723a 0d0a 2020 2020  e) is str:..    
-00001780: 2020 2020 2020 2020 7320 3d20 277b 7d20          s = '{} 
-00001790: 3d20 227b 7d22 272e 666f 726d 6174 2827  = "{}"'.format('
-000017a0: 2e27 2e6a 6f69 6e28 7365 6c66 2e6e 616d  .'.join(self.nam
-000017b0: 655f 6275 6666 6572 292c 2076 616c 7565  e_buffer), value
-000017c0: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-000017d0: 0d0a 2020 2020 2020 2020 2020 2020 7320  ..            s 
-000017e0: 3d20 277b 7d20 3d20 7b7d 272e 666f 726d  = '{} = {}'.form
-000017f0: 6174 2827 2e27 2e6a 6f69 6e28 7365 6c66  at('.'.join(self
-00001800: 2e6e 616d 655f 6275 6666 6572 292c 2076  .name_buffer), v
-00001810: 616c 7565 290d 0a0d 0a20 2020 2020 2020  alue)....       
-00001820: 2073 203d 2073 2e72 6570 6c61 6365 2827   s = s.replace('
-00001830: 2e5b 272c 2027 5b27 290d 0a20 2020 2020  .[', '[')..     
-00001840: 2020 2072 6574 7572 6e20 730d 0a0d 0a20     return s.... 
-00001850: 2020 2064 6566 2067 6574 5f6e 616d 655f     def get_name_
-00001860: 7374 7269 6e67 2873 656c 662c 2069 7465  string(self, ite
-00001870: 6d29 3a0d 0a20 2020 2020 2020 2069 6620  m):..        if 
-00001880: 6974 656d 2e63 6f6d 705f 7479 7065 203d  item.comp_type =
-00001890: 3d20 496e 6465 783a 0d0a 2020 2020 2020  = Index:..      
-000018a0: 2020 2020 2020 6966 2074 7970 6528 6974        if type(it
-000018b0: 656d 2e63 6f6d 7029 2069 7320 7374 723a  em.comp) is str:
-000018c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000018d0: 2020 7365 6c66 2e6e 616d 655f 6275 6666    self.name_buff
-000018e0: 6572 2e61 7070 656e 6428 275b 227b 7d22  er.append('["{}"
-000018f0: 5d27 2e66 6f72 6d61 7428 6974 656d 2e6e  ]'.format(item.n
-00001900: 616d 6529 290d 0a20 2020 2020 2020 2020  ame))..         
-00001910: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00001920: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00001930: 616d 655f 6275 6666 6572 2e61 7070 656e  ame_buffer.appen
-00001940: 6428 275b 7b7d 5d27 2e66 6f72 6d61 7428  d('[{}]'.format(
-00001950: 6974 656d 2e6e 616d 6529 290d 0a20 2020  item.name))..   
-00001960: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00001970: 2020 2020 2020 2020 7365 6c66 2e6e 616d          self.nam
-00001980: 655f 6275 6666 6572 2e61 7070 656e 6428  e_buffer.append(
-00001990: 6974 656d 2e6e 616d 6529 0d0a 2020 2020  item.name)..    
-000019a0: 2020 2020 6966 2069 7465 6d2e 7061 7265      if item.pare
-000019b0: 6e74 2829 3a0d 0a20 2020 2020 2020 2020  nt():..         
-000019c0: 2020 2073 656c 662e 6765 745f 6e61 6d65     self.get_name
-000019d0: 5f73 7472 696e 6728 6974 656d 2e70 6172  _string(item.par
-000019e0: 656e 7428 2929 0d0a 0d0a 2020 2020 4063  ent())....    @c
-000019f0: 6c61 7373 6d65 7468 6f64 0d0a 2020 2020  lassmethod..    
-00001a00: 6465 6620 6c6f 6164 280d 0a20 2020 2020  def load(..     
-00001a10: 2020 2063 6c73 2c20 636f 6d70 2c20 7061     cls, comp, pa
-00001a20: 7265 6e74 3a20 2243 6f6d 6d61 6e64 4974  rent: "CommandIt
-00001a30: 656d 2220 3d20 4e6f 6e65 2920 2d3e 2022  em" = None) -> "
-00001a40: 436f 6d6d 616e 6449 7465 6d22 3a0d 0a20  CommandItem":.. 
-00001a50: 2020 2020 2020 2022 2222 4372 6561 7465         """Create
-00001a60: 2061 2027 726f 6f74 2720 436f 6d6d 616e   a 'root' Comman
-00001a70: 6449 7465 6d20 6672 6f6d 2061 2043 6f6d  dItem from a Com
-00001a80: 706f 6e65 6e74 2061 6e64 200d 0a20 2020  ponent and ..   
-00001a90: 2020 2020 2070 6f70 756c 6174 6520 6974       populate it
-00001aa0: 7320 7375 6263 6f6d 706f 6e65 6e74 2061  s subcomponent a
-00001ab0: 6e64 2063 6f6d 6d61 6e64 7320 7265 6375  nd commands recu
-00001ac0: 7273 6976 656c 792e 0d0a 0d0a 2020 2020  rsively.....    
-00001ad0: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
-00001ae0: 2020 2020 2020 2020 2020 436f 6d6d 616e            Comman
-00001af0: 6449 7465 6d3a 2043 6f6d 6d61 6e64 4974  dItem: CommandIt
-00001b00: 656d 0d0a 2020 2020 2020 2020 2222 220d  em..        """.
-00001b10: 0a20 2020 2020 2020 2072 6f6f 745f 6974  .        root_it
-00001b20: 656d 203d 2043 6f6d 6d61 6e64 4974 656d  em = CommandItem
-00001b30: 2870 6172 656e 7429 0d0a 2020 2020 2020  (parent)..      
-00001b40: 2020 726f 6f74 5f69 7465 6d2e 6e61 6d65    root_item.name
-00001b50: 203d 2022 726f 6f74 220d 0a20 2020 2020   = "root"..     
-00001b60: 2020 2072 6f6f 745f 6974 656d 2e63 6f6d     root_item.com
-00001b70: 7020 3d20 636f 6d70 0d0a 0d0a 2020 2020  p = comp....    
-00001b80: 2020 2020 6966 2069 7373 7562 636c 6173      if issubclas
-00001b90: 7328 636f 6d70 2e5f 5f63 6c61 7373 5f5f  s(comp.__class__
-00001ba0: 2c20 436f 6d70 6f6e 656e 7429 3a0d 0a20  , Component):.. 
-00001bb0: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
-00001bc0: 6974 656d 2e6e 616d 6520 3d20 636f 6d70  item.name = comp
-00001bd0: 2e67 6574 5f6e 616d 6528 290d 0a20 2020  .get_name()..   
-00001be0: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-00001bf0: 6e20 636f 6d70 2e5f 5f64 6963 745f 5f3a  n comp.__dict__:
-00001c00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001c10: 2020 6966 206a 203d 3d20 275f 7061 7265    if j == '_pare
-00001c20: 6e74 273a 0d0a 2020 2020 2020 2020 2020  nt':..          
-00001c30: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00001c40: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00001c50: 2020 2020 696e 7374 616e 6365 203d 2063      instance = c
-00001c60: 6f6d 702e 5f5f 6469 6374 5f5f 5b6a 5d0d  omp.__dict__[j].
-00001c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001c80: 2069 6620 6973 7375 6263 6c61 7373 2869   if issubclass(i
-00001c90: 6e73 7461 6e63 652e 5f5f 636c 6173 735f  nstance.__class_
-00001ca0: 5f2c 2020 436f 6d70 6f6e 656e 7429 3a20  _,  Component): 
-00001cb0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00001cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001cd0: 2020 2020 2063 6869 6c64 203d 2063 6c73       child = cls
-00001ce0: 2e6c 6f61 6428 696e 7374 616e 6365 2c20  .load(instance, 
-00001cf0: 726f 6f74 5f69 7465 6d29 0d0a 2020 2020  root_item)..    
+00000000: 0d0a 696d 706f 7274 2074 696d 650d 0a66  ..import time..f
+00000010: 726f 6d20 7372 7367 7569 2069 6d70 6f72  rom srsgui impor
+00000020: 7420 436f 6d70 6f6e 656e 740d 0a66 726f  t Component..fro
+00000030: 6d20 7372 7367 7569 2e69 6e73 7420 696d  m srsgui.inst im
+00000040: 706f 7274 2043 6f6d 6d61 6e64 2c20 496e  port Command, In
+00000050: 6465 7843 6f6d 6d61 6e64 2c20 5c0d 0a20  dexCommand, \.. 
+00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000070: 2020 2020 2020 2046 6c6f 6174 436f 6d6d         FloatComm
+00000080: 616e 642c 2046 6c6f 6174 496e 6465 7843  and, FloatIndexC
+00000090: 6f6d 6d61 6e64 0d0a 0d0a 0d0a 636c 6173  ommand......clas
+000000a0: 7320 496e 6465 783a 0d0a 2020 2020 7061  s Index:..    pa
+000000b0: 7373 0d0a 0d0a 0d0a 636c 6173 7320 436f  ss......class Co
+000000c0: 6d6d 616e 6449 7465 6d3a 0d0a 2020 2020  mmandItem:..    
+000000d0: 2222 2241 2043 6f6d 6d61 6e64 2069 7465  """A Command ite
+000000e0: 6d20 636f 7272 6573 706f 6e64 696e 6720  m corresponding 
+000000f0: 746f 2061 206c 696e 6520 696e 2051 5472  to a line in QTr
+00000100: 6565 5669 6577 2222 220d 0a0d 0a20 2020  eeView"""....   
+00000110: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000120: 6c66 2c20 7061 7265 6e74 3a20 2243 6f6d  lf, parent: "Com
+00000130: 6d61 6e64 4974 656d 2220 3d20 4e6f 6e65  mandItem" = None
+00000140: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00000150: 2e5f 7061 7265 6e74 203d 2070 6172 656e  ._parent = paren
+00000160: 740d 0a20 2020 2020 2020 2073 656c 662e  t..        self.
+00000170: 5f63 6869 6c64 7265 6e20 3d20 5b5d 0d0a  _children = []..
+00000180: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
+00000190: 6c75 6520 3d20 4e6f 6e65 0d0a 2020 2020  lue = None..    
+000001a0: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
+000001b0: 6c66 2e6e 616d 6520 3d20 2222 0d0a 2020  lf.name = ""..  
+000001c0: 2020 2020 2020 7365 6c66 2e76 616c 7565        self.value
+000001d0: 5f74 7970 6520 3d20 4e6f 6e65 2020 2320  _type = None  # 
+000001e0: 5468 6572 6520 6172 6520 3320 7479 7065  There are 3 type
+000001f0: 7320 6f66 2076 616c 7565 733a 2073 7472  s of values: str
+00000200: 2c20 696e 742c 2061 6e64 2066 6c6f 6174  , int, and float
+00000210: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00000220: 7265 6369 7369 6f6e 203d 2034 0d0a 2020  recision = 4..  
+00000230: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00000240: 7365 6c66 2e63 6f6d 7020 3d20 4e6f 6e65  self.comp = None
+00000250: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00000260: 6f6d 705f 7479 7065 203d 204e 6f6e 6520  omp_type = None 
+00000270: 2020 2320 5468 6572 6520 6172 6520 3520    # There are 5 
+00000280: 7479 7065 7320 6f66 2063 6f6d 706f 6e65  types of compone
+00000290: 6e74 733a 2043 6f6d 706f 6e65 6e74 2c20  nts: Component, 
+000002a0: 436f 6d6d 616e 6473 2c20 496e 6465 7843  Commands, IndexC
+000002b0: 6f6d 6d61 6e64 732c 206d 6574 686f 6420  ommands, method 
+000002c0: 616e 6420 496e 6465 780d 0a20 2020 2020  and Index..     
+000002d0: 2020 2073 656c 662e 7365 745f 656e 6162     self.set_enab
+000002e0: 6c65 203d 2046 616c 7365 0d0a 2020 2020  le = False..    
+000002f0: 2020 2020 7365 6c66 2e67 6574 5f65 6e61      self.get_ena
+00000300: 626c 6520 3d20 4661 6c73 650d 0a20 2020  ble = False..   
+00000310: 2020 2020 2073 656c 662e 6973 5f6d 6574       self.is_met
+00000320: 686f 6420 3d20 4661 6c73 650d 0a20 2020  hod = False..   
+00000330: 2020 2020 2073 656c 662e 6578 636c 7564       self.exclud
+00000340: 6564 203d 2046 616c 7365 0d0a 2020 2020  ed = False..    
+00000350: 2020 2020 7365 6c66 2e72 6177 5f72 656d      self.raw_rem
+00000360: 6f74 655f 636f 6d6d 616e 6420 3d20 2222  ote_command = ""
+00000370: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00000380: 696d 6573 7461 6d70 203d 2030 2e30 0d0a  imestamp = 0.0..
+00000390: 0d0a 2020 2020 6465 6620 6170 7065 6e64  ..    def append
+000003a0: 4368 696c 6428 7365 6c66 2c20 6974 656d  Child(self, item
+000003b0: 3a20 2243 6f6d 6d61 6e64 4974 656d 2229  : "CommandItem")
+000003c0: 3a0d 0a20 2020 2020 2020 2022 2222 4164  :..        """Ad
+000003d0: 6420 6974 656d 2061 7320 6120 6368 696c  d item as a chil
+000003e0: 6422 2222 0d0a 2020 2020 2020 2020 7365  d"""..        se
+000003f0: 6c66 2e5f 6368 696c 6472 656e 2e61 7070  lf._children.app
+00000400: 656e 6428 6974 656d 290d 0a0d 0a20 2020  end(item)....   
+00000410: 2064 6566 2063 6869 6c64 2873 656c 662c   def child(self,
+00000420: 2072 6f77 3a20 696e 7429 202d 3e20 2243   row: int) -> "C
+00000430: 6f6d 6d61 6e64 4974 656d 223a 0d0a 2020  ommandItem":..  
+00000440: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00000450: 7468 6520 6368 696c 6420 6f66 2074 6865  the child of the
+00000460: 2063 7572 7265 6e74 2069 7465 6d20 6672   current item fr
+00000470: 6f6d 2074 6865 2067 6976 656e 2072 6f77  om the given row
+00000480: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+00000490: 7572 6e20 7365 6c66 2e5f 6368 696c 6472  urn self._childr
+000004a0: 656e 5b72 6f77 5d0d 0a0d 0a20 2020 2064  en[row]....    d
+000004b0: 6566 2070 6172 656e 7428 7365 6c66 2920  ef parent(self) 
+000004c0: 2d3e 2022 436f 6d6d 616e 6449 7465 6d22  -> "CommandItem"
+000004d0: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
+000004e0: 7475 726e 2074 6865 2070 6172 656e 7420  turn the parent 
+000004f0: 6f66 2074 6865 2063 7572 7265 6e74 2069  of the current i
+00000500: 7465 6d22 2222 0d0a 2020 2020 2020 2020  tem"""..        
+00000510: 7265 7475 726e 2073 656c 662e 5f70 6172  return self._par
+00000520: 656e 740d 0a0d 0a20 2020 2064 6566 2063  ent....    def c
+00000530: 6869 6c64 436f 756e 7428 7365 6c66 2920  hildCount(self) 
+00000540: 2d3e 2069 6e74 3a0d 0a20 2020 2020 2020  -> int:..       
+00000550: 2022 2222 5265 7475 726e 2074 6865 206e   """Return the n
+00000560: 756d 6265 7220 6f66 2063 6869 6c64 7265  umber of childre
+00000570: 6e20 6f66 2074 6865 2063 7572 7265 6e74  n of the current
+00000580: 2069 7465 6d22 2222 0d0a 2020 2020 2020   item"""..      
+00000590: 2020 7265 7475 726e 206c 656e 2873 656c    return len(sel
+000005a0: 662e 5f63 6869 6c64 7265 6e29 0d0a 0d0a  f._children)....
+000005b0: 2020 2020 6465 6620 726f 7728 7365 6c66      def row(self
+000005c0: 2920 2d3e 2069 6e74 3a0d 0a20 2020 2020  ) -> int:..     
+000005d0: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
+000005e0: 2072 6f77 2077 6865 7265 2074 6865 2063   row where the c
+000005f0: 7572 7265 6e74 2069 7465 6d20 6f63 6375  urrent item occu
+00000600: 7069 6573 2069 6e20 7468 6520 7061 7265  pies in the pare
+00000610: 6e74 2222 220d 0a20 2020 2020 2020 2072  nt"""..        r
+00000620: 6574 7572 6e20 7365 6c66 2e5f 7061 7265  eturn self._pare
+00000630: 6e74 2e5f 6368 696c 6472 656e 2e69 6e64  nt._children.ind
+00000640: 6578 2873 656c 6629 2069 6620 7365 6c66  ex(self) if self
+00000650: 2e5f 7061 7265 6e74 2065 6c73 6520 300d  ._parent else 0.
+00000660: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+00000670: 0d0a 2020 2020 6465 6620 7661 6c75 6528  ..    def value(
+00000680: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000690: 2222 2252 6574 7572 6e20 7468 6520 7661  """Return the va
+000006a0: 6c75 6520 6f66 2074 6865 2063 7572 7265  lue of the curre
+000006b0: 6e74 2069 7465 6d22 2222 0d0a 2020 2020  nt item"""..    
+000006c0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+000006d0: 2020 2020 2020 7473 203d 2074 696d 652e        ts = time.
+000006e0: 7469 6d65 2829 0d0a 2020 2020 2020 2020  time()..        
+000006f0: 2020 2020 6966 2074 7320 2d20 7365 6c66      if ts - self
+00000700: 2e74 696d 6573 7461 6d70 203c 2030 2e31  .timestamp < 0.1
+00000710: 3a20 2320 5570 6461 7465 2076 616c 7565  : # Update value
+00000720: 206c 6174 6572 2074 6861 6e20 302e 3120   later than 0.1 
+00000730: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00000740: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00000750: 7661 6c75 650d 0a0d 0a20 2020 2020 2020  value....       
+00000760: 2020 2020 2069 6620 7365 6c66 2e63 6f6d       if self.com
+00000770: 705f 7479 7065 203d 3d20 496e 6465 7820  p_type == Index 
+00000780: 616e 6420 7365 6c66 2e67 6574 5f65 6e61  and self.get_ena
+00000790: 626c 6520 616e 6420 6e6f 7420 7365 6c66  ble and not self
+000007a0: 2e65 7863 6c75 6465 643a 0d0a 2020 2020  .excluded:..    
+000007b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000007c0: 2e5f 7661 6c75 6520 3d20 7365 6c66 2e5f  ._value = self._
+000007d0: 7061 7265 6e74 2e63 6f6d 702e 5f5f 6765  parent.comp.__ge
+000007e0: 7469 7465 6d5f 5f28 7365 6c66 2e63 6f6d  titem__(self.com
+000007f0: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
+00000800: 2020 2020 7365 6c66 2e5f 7661 6c75 655f      self._value_
+00000810: 7479 7065 203d 2074 7970 6528 7365 6c66  type = type(self
+00000820: 2e5f 7661 6c75 6529 0d0a 2020 2020 2020  ._value)..      
+00000830: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00000840: 696d 6573 7461 6d70 203d 2074 730d 0a20  imestamp = ts.. 
+00000850: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00000860: 6973 7375 6263 6c61 7373 2874 7970 6528  issubclass(type(
+00000870: 7365 6c66 2e63 6f6d 7029 2c20 436f 6d6d  self.comp), Comm
+00000880: 616e 6429 2061 6e64 2073 656c 662e 6765  and) and self.ge
+00000890: 745f 656e 6162 6c65 2061 6e64 206e 6f74  t_enable and not
+000008a0: 2073 656c 662e 6578 636c 7564 6564 3a0d   self.excluded:.
+000008b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000008c0: 2073 656c 662e 5f76 616c 7565 203d 2073   self._value = s
+000008d0: 656c 662e 636f 6d70 2e5f 5f67 6574 5f5f  elf.comp.__get__
+000008e0: 2873 656c 662e 5f70 6172 656e 742e 636f  (self._parent.co
+000008f0: 6d70 2c20 7365 6c66 2e5f 7061 7265 6e74  mp, self._parent
+00000900: 2e63 6f6d 702e 5f5f 636c 6173 735f 5f29  .comp.__class__)
+00000910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000920: 2020 7365 6c66 2e5f 7661 6c75 655f 7479    self._value_ty
+00000930: 7065 203d 2074 7970 6528 7365 6c66 2e5f  pe = type(self._
+00000940: 7661 6c75 6529 0d0a 2020 2020 2020 2020  value)..        
+00000950: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+00000960: 6573 7461 6d70 203d 2074 730d 0a20 2020  estamp = ts..   
+00000970: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000990: 7365 6c66 2e5f 7661 6c75 655f 7479 7065  self._value_type
+000009a0: 203d 2074 7970 6528 7365 6c66 2e5f 7661   = type(self._va
+000009b0: 6c75 6529 0d0a 0d0a 2020 2020 2020 2020  lue)....        
+000009c0: 2020 2020 2320 526f 756e 6420 666c 6f61      # Round floa
+000009d0: 7420 746f 2069 7473 2070 7265 6369 7369  t to its precisi
+000009e0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+000009f0: 6966 2073 656c 662e 636f 6d70 5f74 7970  if self.comp_typ
+00000a00: 6520 3d3d 2046 6c6f 6174 436f 6d6d 616e  e == FloatComman
+00000a10: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
+00000a20: 2020 2020 7365 6c66 2e5f 7661 6c75 6520      self._value 
+00000a30: 3d20 726f 756e 6428 7365 6c66 2e5f 7661  = round(self._va
+00000a40: 6c75 652c 2073 656c 662e 7072 6563 6973  lue, self.precis
+00000a50: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
+00000a60: 2020 656c 6966 2073 656c 662e 636f 6d70    elif self.comp
+00000a70: 5f74 7970 6520 3d3d 2049 6e64 6578 2061  _type == Index a
+00000a80: 6e64 2073 656c 662e 5f70 6172 656e 742e  nd self._parent.
+00000a90: 636f 6d70 5f74 7970 6520 3d3d 2046 6c6f  comp_type == Flo
+00000aa0: 6174 496e 6465 7843 6f6d 6d61 6e64 3a0d  atIndexCommand:.
+00000ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ac0: 2073 656c 662e 5f76 616c 7565 203d 2072   self._value = r
+00000ad0: 6f75 6e64 2873 656c 662e 5f76 616c 7565  ound(self._value
+00000ae0: 2c20 7365 6c66 2e70 7265 6369 7369 6f6e  , self.precision
+00000af0: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
+00000b00: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00000b10: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00000b20: 7269 6e74 2865 2c20 7365 6c66 2e6e 616d  rint(e, self.nam
+00000b30: 6529 0d0a 2020 2020 2020 2020 7265 7475  e)..        retu
+00000b40: 726e 2073 656c 662e 5f76 616c 7565 0d0a  rn self._value..
+00000b50: 0d0a 2020 2020 4076 616c 7565 2e73 6574  ..    @value.set
+00000b60: 7465 720d 0a20 2020 2064 6566 2076 616c  ter..    def val
+00000b70: 7565 2873 656c 662c 2076 616c 7565 293a  ue(self, value):
+00000b80: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00000b90: 7661 6c75 6520 3d20 7661 6c75 650d 0a0d  value = value...
+00000ba0: 0a20 2020 2064 6566 2073 6574 5f76 616c  .    def set_val
+00000bb0: 7565 2873 656c 662c 2076 616c 7565 293a  ue(self, value):
+00000bc0: 0d0a 2020 2020 2020 2020 2222 2253 6574  ..        """Set
+00000bd0: 2076 616c 7565 2074 6f20 7468 6520 696e   value to the in
+00000be0: 7374 7275 6d65 6e74 2061 6e64 2075 7064  strument and upd
+00000bf0: 6174 6520 7468 6520 7661 6c75 6520 6f66  ate the value of
+00000c00: 2074 6865 2069 7465 6d22 2222 0d0a 2020   the item"""..  
+00000c10: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00000c20: 6d70 5f74 7970 6520 3d3d 2049 6e64 6578  mp_type == Index
+00000c30: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00000c40: 656c 662e 5f70 6172 656e 742e 636f 6d70  elf._parent.comp
+00000c50: 2e5f 5f73 6574 6974 656d 5f5f 2873 656c  .__setitem__(sel
+00000c60: 662e 636f 6d70 2c20 7661 6c75 6529 0d0a  f.comp, value)..
+00000c70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000c80: 2e5f 7661 6c75 6520 3d20 7365 6c66 2e5f  ._value = self._
+00000c90: 7061 7265 6e74 2e63 6f6d 702e 5f5f 6765  parent.comp.__ge
+00000ca0: 7469 7465 6d5f 5f28 7365 6c66 2e63 6f6d  titem__(self.com
+00000cb0: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
+00000cc0: 7365 6c66 2e74 696d 6573 7461 6d70 203d  self.timestamp =
+00000cd0: 2074 696d 652e 7469 6d65 2829 0d0a 2020   time.time()..  
+00000ce0: 2020 2020 2020 656c 6966 2069 7373 7562        elif issub
+00000cf0: 636c 6173 7328 7479 7065 2873 656c 662e  class(type(self.
+00000d00: 636f 6d70 292c 2043 6f6d 6d61 6e64 293a  comp), Command):
+00000d10: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00000d20: 6c66 2e63 6f6d 702e 5f5f 7365 745f 5f28  lf.comp.__set__(
+00000d30: 7365 6c66 2e5f 7061 7265 6e74 2e63 6f6d  self._parent.com
+00000d40: 702c 2076 616c 7565 290d 0a20 2020 2020  p, value)..     
+00000d50: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
+00000d60: 7565 203d 2073 656c 662e 636f 6d70 2e5f  ue = self.comp._
+00000d70: 5f67 6574 5f5f 2873 656c 662e 5f70 6172  _get__(self._par
+00000d80: 656e 742e 636f 6d70 2c20 7365 6c66 2e5f  ent.comp, self._
+00000d90: 7061 7265 6e74 2e63 6f6d 702e 5f5f 636c  parent.comp.__cl
+00000da0: 6173 735f 5f29 0d0a 2020 2020 2020 2020  ass__)..        
+00000db0: 2020 2020 7365 6c66 2e74 696d 6573 7461      self.timesta
+00000dc0: 6d70 203d 2074 696d 652e 7469 6d65 2829  mp = time.time()
+00000dd0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00000de0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00000df0: 662e 5f76 616c 7565 203d 2076 616c 7565  f._value = value
+00000e00: 0d0a 0d0a 2020 2020 6465 6620 6973 5f65  ....    def is_e
+00000e10: 6469 7461 626c 6528 7365 6c66 293a 0d0a  ditable(self):..
+00000e20: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00000e30: 6e20 5472 7565 2069 6620 7468 6520 6974  n True if the it
+00000e40: 656d 2069 7320 6564 6974 6162 6c65 2222  em is editable""
+00000e50: 220d 0a20 2020 2020 2020 2069 6620 7365  "..        if se
+00000e60: 6c66 2e63 6f6d 705f 7479 7065 203d 3d20  lf.comp_type == 
+00000e70: 496e 6465 7820 616e 6420 5c0d 0a20 2020  Index and \..   
+00000e80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00000e90: 662e 7365 745f 656e 6162 6c65 2061 6e64  f.set_enable and
+00000ea0: 2073 656c 662e 6765 745f 656e 6162 6c65   self.get_enable
+00000eb0: 2061 6e64 206e 6f74 2073 656c 662e 6578   and not self.ex
+00000ec0: 636c 7564 6564 3a0d 0a20 2020 2020 2020  cluded:..       
+00000ed0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00000ee0: 0d0a 2020 2020 2020 2020 656c 6966 2069  ..        elif i
+00000ef0: 7373 7562 636c 6173 7328 7479 7065 2873  ssubclass(type(s
+00000f00: 656c 662e 636f 6d70 292c 2043 6f6d 6d61  elf.comp), Comma
+00000f10: 6e64 2920 616e 6420 5c0d 0a20 2020 2020  nd) and \..     
+00000f20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000f30: 7365 745f 656e 6162 6c65 2061 6e64 2073  set_enable and s
+00000f40: 656c 662e 6765 745f 656e 6162 6c65 2061  elf.get_enable a
+00000f50: 6e64 206e 6f74 2073 656c 662e 6578 636c  nd not self.excl
+00000f60: 7564 6564 3a0d 0a20 2020 2020 2020 2020  uded:..         
+00000f70: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
+00000f80: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00000f90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000fa0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2064  n False....    d
+00000fb0: 6566 2067 6574 5f75 6e69 7428 7365 6c66  ef get_unit(self
+00000fc0: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
+00000fd0: 6574 7572 6e20 7468 6520 756e 6974 206f  eturn the unit o
+00000fe0: 6620 7468 6520 6974 656d 2222 220d 0a20  f the item""".. 
+00000ff0: 2020 2020 2020 2063 6f6d 7020 3d20 4e6f         comp = No
+00001000: 6e65 0d0a 2020 2020 2020 2020 6966 2073  ne..        if s
+00001010: 656c 662e 636f 6d70 5f74 7970 6520 3d3d  elf.comp_type ==
+00001020: 2049 6e64 6578 3a0d 0a20 2020 2020 2020   Index:..       
+00001030: 2020 2020 2063 6f6d 7020 3d20 7365 6c66       comp = self
+00001040: 2e70 6172 656e 7428 292e 636f 6d70 0d0a  .parent().comp..
+00001050: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
+00001060: 7562 636c 6173 7328 7479 7065 2873 656c  ubclass(type(sel
+00001070: 662e 636f 6d70 292c 2043 6f6d 6d61 6e64  f.comp), Command
+00001080: 2920 6f72 205c 0d0a 2020 2020 2020 2020  ) or \..        
+00001090: 2020 2020 2069 7373 7562 636c 6173 7328       issubclass(
+000010a0: 7479 7065 2873 656c 662e 636f 6d70 292c  type(self.comp),
+000010b0: 2049 6e64 6578 436f 6d6d 616e 6429 3a0d   IndexCommand):.
+000010c0: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
+000010d0: 7020 3d20 7365 6c66 2e63 6f6d 700d 0a0d  p = self.comp...
+000010e0: 0a20 2020 2020 2020 2069 6620 636f 6d70  .        if comp
+000010f0: 2061 6e64 2068 6173 6174 7472 2863 6f6d   and hasattr(com
+00001100: 702c 2027 756e 6974 2729 3a0d 0a20 2020  p, 'unit'):..   
+00001110: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001120: 636f 6d70 2e75 6e69 740d 0a20 2020 2020  comp.unit..     
+00001130: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00001140: 2020 2020 2020 7265 7475 726e 2022 220d        return "".
+00001150: 0a0d 0a20 2020 2064 6566 2067 6574 5f66  ...    def get_f
+00001160: 6f72 6d61 7428 7365 6c66 293a 0d0a 2020  ormat(self):..  
+00001170: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00001180: 7468 6520 666f 726d 6174 206f 6620 7468  the format of th
+00001190: 6520 6974 656d 2222 220d 0a20 2020 2020  e item"""..     
+000011a0: 2020 2063 6f6d 7020 3d20 4e6f 6e65 0d0a     comp = None..
+000011b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000011c0: 636f 6d70 5f74 7970 6520 3d3d 2049 6e64  comp_type == Ind
+000011d0: 6578 3a0d 0a20 2020 2020 2020 2020 2020  ex:..           
+000011e0: 2063 6f6d 7020 3d20 7365 6c66 2e70 6172   comp = self.par
+000011f0: 656e 7428 292e 636f 6d70 0d0a 2020 2020  ent().comp..    
+00001200: 2020 2020 656c 6966 2069 7373 7562 636c      elif issubcl
+00001210: 6173 7328 7479 7065 2873 656c 662e 636f  ass(type(self.co
+00001220: 6d70 292c 2043 6f6d 6d61 6e64 2920 6f72  mp), Command) or
+00001230: 205c 0d0a 2020 2020 2020 2020 2020 2020   \..            
+00001240: 2069 7373 7562 636c 6173 7328 7479 7065   issubclass(type
+00001250: 2873 656c 662e 636f 6d70 292c 2049 6e64  (self.comp), Ind
+00001260: 6578 436f 6d6d 616e 6429 3a0d 0a20 2020  exCommand):..   
+00001270: 2020 2020 2020 2020 2063 6f6d 7020 3d20           comp = 
+00001280: 7365 6c66 2e63 6f6d 700d 0a0d 0a20 2020  self.comp....   
+00001290: 2020 2020 2069 6620 636f 6d70 2061 6e64       if comp and
+000012a0: 2068 6173 6174 7472 2863 6f6d 702c 2027   hasattr(comp, '
+000012b0: 666d 7427 293a 0d0a 2020 2020 2020 2020  fmt'):..        
+000012c0: 2020 2020 7265 7475 726e 2063 6f6d 702e      return comp.
+000012d0: 666d 740d 0a20 2020 2020 2020 2065 6c73  fmt..        els
+000012e0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000012f0: 7265 7475 726e 2027 270d 0a0d 0a20 2020  return ''....   
+00001300: 2040 636c 6173 736d 6574 686f 640d 0a20   @classmethod.. 
+00001310: 2020 2064 6566 206c 6f61 6428 0d0a 2020     def load(..  
+00001320: 2020 2020 2020 636c 732c 2063 6f6d 702c        cls, comp,
+00001330: 2070 6172 656e 743a 2022 436f 6d6d 616e   parent: "Comman
+00001340: 6449 7465 6d22 203d 204e 6f6e 652c 2073  dItem" = None, s
+00001350: 6f72 743d 4661 6c73 650d 0a20 2020 2029  ort=False..    )
+00001360: 202d 3e20 2243 6f6d 6d61 6e64 4974 656d   -> "CommandItem
+00001370: 223a 0d0a 2020 2020 2020 2020 2222 2243  ":..        """C
+00001380: 7265 6174 6520 6120 2772 6f6f 7427 2043  reate a 'root' C
+00001390: 6f6d 6d61 6e64 4974 656d 2066 726f 6d20  ommandItem from 
+000013a0: 6120 436f 6d70 6f6e 656e 7420 616e 6420  a Component and 
+000013b0: 0d0a 2020 2020 2020 2020 706f 7075 6c61  ..        popula
+000013c0: 7465 2069 7473 2073 7562 636f 6d70 6f6e  te its subcompon
+000013d0: 656e 7420 616e 6420 636f 6d6d 616e 6473  ent and commands
+000013e0: 2072 6563 7572 7369 7665 6c79 2e0d 0a0d   recursively....
+000013f0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00001400: 3a0d 0a20 2020 2020 2020 2020 2020 2043  :..            C
+00001410: 6f6d 6d61 6e64 4974 656d 3a20 436f 6d6d  ommandItem: Comm
+00001420: 616e 6449 7465 6d0d 0a20 2020 2020 2020  andItem..       
+00001430: 2022 2222 0d0a 2020 2020 2020 2020 726f   """..        ro
+00001440: 6f74 5f69 7465 6d20 3d20 436f 6d6d 616e  ot_item = Comman
+00001450: 6449 7465 6d28 7061 7265 6e74 290d 0a20  dItem(parent).. 
+00001460: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001470: 2e6e 616d 6520 3d20 2272 6f6f 7422 0d0a  .name = "root"..
+00001480: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
+00001490: 6d2e 636f 6d70 203d 2063 6f6d 700d 0a0d  m.comp = comp...
+000014a0: 0a20 2020 2020 2020 2069 6620 6973 7375  .        if issu
+000014b0: 6263 6c61 7373 2863 6f6d 702e 5f5f 636c  bclass(comp.__cl
+000014c0: 6173 735f 5f2c 2043 6f6d 706f 6e65 6e74  ass__, Component
+000014d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000014e0: 666f 7220 6a20 696e 2063 6f6d 702e 5f5f  for j in comp.__
+000014f0: 6469 6374 5f5f 3a0d 0a20 2020 2020 2020  dict__:..       
+00001500: 2020 2020 2020 2020 2069 6620 6a20 3d3d           if j ==
+00001510: 2027 5f70 6172 656e 7427 3a0d 0a20 2020   '_parent':..   
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00001540: 2020 2020 2020 2020 2020 2069 6e73 7461             insta
+00001550: 6e63 6520 3d20 636f 6d70 2e5f 5f64 6963  nce = comp.__dic
+00001560: 745f 5f5b 6a5d 0d0a 2020 2020 2020 2020  t__[j]..        
+00001570: 2020 2020 2020 2020 6966 2069 7373 7562          if issub
+00001580: 636c 6173 7328 696e 7374 616e 6365 2e5f  class(instance._
+00001590: 5f63 6c61 7373 5f5f 2c20 2043 6f6d 706f  _class__,  Compo
+000015a0: 6e65 6e74 293a 2020 2020 2020 2020 2020  nent):          
+000015b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000015c0: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+000015d0: 6420 3d20 636c 732e 6c6f 6164 2869 6e73  d = cls.load(ins
+000015e0: 7461 6e63 652c 2072 6f6f 745f 6974 656d  tance, root_item
+000015f0: 2c20 736f 7274 290d 0a20 2020 2020 2020  , sort)..       
+00001600: 2020 2020 2020 2020 2020 2020 2063 6869               chi
+00001610: 6c64 2e6e 616d 6520 3d20 6a0d 0a20 2020  ld.name = j..   
+00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001630: 2063 6869 6c64 2e63 6f6d 7020 3d20 696e   child.comp = in
+00001640: 7374 616e 6365 0d0a 2020 2020 2020 2020  stance..        
+00001650: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00001660: 6e73 7461 6e63 6520 696e 2063 6f6d 702e  nstance in comp.
+00001670: 6578 636c 7564 655f 6361 7074 7572 653a  exclude_capture:
+00001680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001690: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+000016a0: 6578 636c 7564 6564 203d 2054 7275 650d  excluded = True.
+000016b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000016c0: 2020 2020 2063 6869 6c64 2e63 6f6d 705f       child.comp_
+000016d0: 7479 7065 203d 2074 7970 6528 696e 7374  type = type(inst
+000016e0: 616e 6365 290d 0a20 2020 2020 2020 2020  ance)..         
+000016f0: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
+00001700: 6974 656d 2e61 7070 656e 6443 6869 6c64  item.appendChild
+00001710: 2863 6869 6c64 290d 0a0d 0a20 2020 2020  (child)....     
+00001720: 2020 2020 2020 2063 7572 7265 6e74 5f61         current_a
+00001730: 7474 7269 6275 7465 7320 3d20 5b5d 0d0a  ttributes = []..
+00001740: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00001750: 6320 696e 2063 6f6d 702e 5f5f 636c 6173  c in comp.__clas
+00001760: 735f 5f2e 5f5f 6d72 6f5f 5f3a 2020 2320  s__.__mro__:  # 
+00001770: 6c6f 6f70 2074 6872 6f75 6768 2074 6865  loop through the
+00001780: 2063 6c61 7373 6573 2069 6e63 6c75 6469   classes includi
+00001790: 6e67 2073 7570 6572 2063 6c61 7373 6573  ng super classes
+000017a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000017b0: 2020 6966 206e 6f74 2069 7373 7562 636c    if not issubcl
+000017c0: 6173 7328 632c 2043 6f6d 706f 6e65 6e74  ass(c, Component
+000017d0: 293a 2020 2320 6974 2073 686f 756c 6420  ):  # it should 
+000017e0: 6265 2061 2073 7562 636c 6173 7320 6f66  be a subclass of
+000017f0: 2043 6f6d 706f 6e65 6e74 0d0a 2020 2020   Component..    
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 6272 6561 6b0d 0a20 2020 2020 2020 2020  break..         
+00001820: 2020 2020 2020 2069 6620 6320 3d3d 2043         if c == C
+00001830: 6f6d 706f 6e65 6e74 3a20 2023 2042 7574  omponent:  # But
+00001840: 2069 7420 7368 6f75 6c64 206e 6f74 2062   it should not b
+00001850: 6520 436f 6d70 6f6e 656e 740d 0a20 2020  e Component..   
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2062 7265 616b 0d0a 0d0a 2020 2020 2020   break....      
+00001880: 2020 2020 2020 2020 2020 666f 7220 6b65            for ke
+00001890: 7920 696e 2063 2e5f 5f64 6963 745f 5f3a  y in c.__dict__:
+000018a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000018b0: 2020 2020 2020 636d 645f 696e 7374 616e        cmd_instan
+000018c0: 6365 203d 2063 2e5f 5f64 6963 745f 5f5b  ce = c.__dict__[
+000018d0: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
+000018e0: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+000018f0: 2069 6e20 6375 7272 656e 745f 6174 7472   in current_attr
+00001900: 6962 7574 6573 3a0d 0a20 2020 2020 2020  ibutes:..       
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00001930: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001940: 7572 7265 6e74 5f61 7474 7269 6275 7465  urrent_attribute
+00001950: 732e 6170 7065 6e64 286b 6579 290d 0a0d  s.append(key)...
+00001960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001970: 2020 2020 2069 6620 6973 7375 6263 6c61       if issubcla
+00001980: 7373 2863 6d64 5f69 6e73 7461 6e63 652e  ss(cmd_instance.
+00001990: 5f5f 636c 6173 735f 5f2c 2043 6f6d 6d61  __class__, Comma
+000019a0: 6e64 293a 0d0a 2020 2020 2020 2020 2020  nd):..          
+000019b0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+000019c0: 696c 6420 3d20 636c 732e 6c6f 6164 2863  ild = cls.load(c
+000019d0: 6d64 5f69 6e73 7461 6e63 652c 2072 6f6f  md_instance, roo
+000019e0: 745f 6974 656d 2c20 736f 7274 290d 0a20  t_item, sort).. 
+000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a00: 2020 2020 2020 2063 6869 6c64 2e6e 616d         child.nam
+00001a10: 6520 3d20 6b65 790d 0a20 2020 2020 2020  e = key..       
+00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a30: 2063 6869 6c64 2e63 6f6d 7020 3d20 636d   child.comp = cm
+00001a40: 645f 696e 7374 616e 6365 0d0a 2020 2020  d_instance..    
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 2020 2020 6368 696c 642e 636f 6d70 5f74      child.comp_t
+00001a70: 7970 6520 3d20 7479 7065 2863 6d64 5f69  ype = type(cmd_i
+00001a80: 6e73 7461 6e63 6529 0d0a 0d0a 2020 2020  nstance)....    
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 2020 2020 726f 6f74 5f69 7465 6d2e 6170      root_item.ap
+00001ab0: 7065 6e64 4368 696c 6428 6368 696c 6429  pendChild(child)
+00001ac0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00001ad0: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
+00001ae0: 7562 636c 6173 7328 636d 645f 696e 7374  ubclass(cmd_inst
+00001af0: 616e 6365 2e5f 5f63 6c61 7373 5f5f 2c20  ance.__class__, 
+00001b00: 496e 6465 7843 6f6d 6d61 6e64 293a 0d0a  IndexCommand):..
+00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b20: 2020 2020 2020 2020 6368 696c 6420 3d20          child = 
+00001b30: 636c 732e 6c6f 6164 2863 6d64 5f69 6e73  cls.load(cmd_ins
+00001b40: 7461 6e63 652c 2072 6f6f 745f 6974 656d  tance, root_item
+00001b50: 2c20 736f 7274 290d 0a20 2020 2020 2020  , sort)..       
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b70: 2063 6869 6c64 2e6e 616d 6520 3d20 6b65   child.name = ke
+00001b80: 790d 0a20 2020 2020 2020 2020 2020 2020  y..             
+00001b90: 2020 2020 2020 2020 2020 2063 6869 6c64             child
+00001ba0: 2e63 6f6d 7020 3d20 636d 645f 696e 7374  .comp = cmd_inst
+00001bb0: 616e 6365 0d0a 2020 2020 2020 2020 2020  ance..          
+00001bc0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+00001bd0: 696c 642e 636f 6d70 5f74 7970 6520 3d20  ild.comp_type = 
+00001be0: 7479 7065 2863 6d64 5f69 6e73 7461 6e63  type(cmd_instanc
+00001bf0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00001c00: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+00001c10: 5f69 7465 6d2e 6170 7065 6e64 4368 696c  _item.appendChil
+00001c20: 6428 6368 696c 6429 0d0a 0d0a 2020 2020  d(child)....    
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 656c 6966 2063 616c 6c61 626c 6528 636d  elif callable(cm
+00001c50: 645f 696e 7374 616e 6365 293a 0d0a 2020  d_instance):..  
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 6966 2069 7373 7562 636c        if issubcl
+00001c80: 6173 7328 636d 645f 696e 7374 616e 6365  ass(cmd_instance
+00001c90: 2e5f 5f63 6c61 7373 5f5f 2c20 7479 7065  .__class__, type
+00001ca0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cc0: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 6966 206b 6579 2e73 7461 7274 7377    if key.startsw
+00001cf0: 6974 6828 275f 2729 3a0d 0a20 2020 2020  ith('_'):..     
 00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 6368 696c 642e 6e61 6d65 203d 206a 0d0a  child.name = j..
-00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d30: 2020 2020 6368 696c 642e 636f 6d70 203d      child.comp =
-00001d40: 2069 6e73 7461 6e63 650d 0a20 2020 2020   instance..     
-00001d50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001d60: 6620 696e 7374 616e 6365 2069 6e20 636f  f instance in co
-00001d70: 6d70 2e65 7863 6c75 6465 5f63 6170 7475  mp.exclude_captu
-00001d80: 7265 3a0d 0a20 2020 2020 2020 2020 2020  re:..           
-00001d90: 2020 2020 2020 2020 2020 2020 2063 6869               chi
-00001da0: 6c64 2e65 7863 6c75 6465 6420 3d20 5472  ld.excluded = Tr
-00001db0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00001dc0: 2020 2020 2020 2020 6368 696c 642e 636f          child.co
-00001dd0: 6d70 5f74 7970 6520 3d20 7479 7065 2869  mp_type = type(i
-00001de0: 6e73 7461 6e63 6529 0d0a 2020 2020 2020  nstance)..      
-00001df0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00001e00: 6f74 5f69 7465 6d2e 6170 7065 6e64 4368  ot_item.appendCh
-00001e10: 696c 6428 6368 696c 6429 0d0a 0d0a 2020  ild(child)....  
-00001e20: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00001e30: 745f 6174 7472 6962 7574 6573 203d 205b  t_attributes = [
-00001e40: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
-00001e50: 6f72 2063 2069 6e20 636f 6d70 2e5f 5f63  or c in comp.__c
-00001e60: 6c61 7373 5f5f 2e5f 5f6d 726f 5f5f 3a20  lass__.__mro__: 
-00001e70: 2023 206c 6f6f 7020 7468 726f 7567 6820   # loop through 
-00001e80: 7468 6520 636c 6173 7365 7320 696e 636c  the classes incl
-00001e90: 7564 696e 6720 7375 7065 7220 636c 6173  uding super clas
-00001ea0: 7365 730d 0a20 2020 2020 2020 2020 2020  ses..           
-00001eb0: 2020 2020 2069 6620 6e6f 7420 6973 7375       if not issu
-00001ec0: 6263 6c61 7373 2863 2c20 436f 6d70 6f6e  bclass(c, Compon
-00001ed0: 656e 7429 3a20 2023 2069 7420 7368 6f75  ent):  # it shou
-00001ee0: 6c64 2062 6520 6120 7375 6263 6c61 7373  ld be a subclass
-00001ef0: 206f 6620 436f 6d70 6f6e 656e 740d 0a20   of Component.. 
-00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f10: 2020 2062 7265 616b 0d0a 2020 2020 2020     break..      
-00001f20: 2020 2020 2020 2020 2020 6966 2063 203d            if c =
-00001f30: 3d20 436f 6d70 6f6e 656e 743a 2020 2320  = Component:  # 
-00001f40: 4275 7420 6974 2073 686f 756c 6420 6e6f  But it should no
-00001f50: 7420 6265 2043 6f6d 706f 6e65 6e74 0d0a  t be Component..
-00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f70: 2020 2020 6272 6561 6b0d 0a0d 0a20 2020      break....   
-00001f80: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00001f90: 206b 6579 2069 6e20 632e 5f5f 6469 6374   key in c.__dict
-00001fa0: 5f5f 3a0d 0a20 2020 2020 2020 2020 2020  __:..           
-00001fb0: 2020 2020 2020 2020 2063 6d64 5f69 6e73           cmd_ins
-00001fc0: 7461 6e63 6520 3d20 632e 5f5f 6469 6374  tance = c.__dict
-00001fd0: 5f5f 5b6b 6579 5d0d 0a20 2020 2020 2020  __[key]..       
-00001fe0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00001ff0: 6b65 7920 696e 2063 7572 7265 6e74 5f61  key in current_a
-00002000: 7474 7269 6275 7465 733a 0d0a 2020 2020  ttributes:..    
-00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002020: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
-00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002040: 2020 6375 7272 656e 745f 6174 7472 6962    current_attrib
-00002050: 7574 6573 2e61 7070 656e 6428 6b65 7929  utes.append(key)
-00002060: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00002070: 2020 2020 2020 2020 6966 2069 7373 7562          if issub
-00002080: 636c 6173 7328 636d 645f 696e 7374 616e  class(cmd_instan
-00002090: 6365 2e5f 5f63 6c61 7373 5f5f 2c20 436f  ce.__class__, Co
-000020a0: 6d6d 616e 6429 3a0d 0a20 2020 2020 2020  mmand):..       
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 2063 6869 6c64 203d 2063 6c73 2e6c 6f61   child = cls.loa
-000020d0: 6428 636d 645f 696e 7374 616e 6365 2c20  d(cmd_instance, 
-000020e0: 726f 6f74 5f69 7465 6d29 0d0a 2020 2020  root_item)..    
-000020f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002100: 2020 2020 6368 696c 642e 6e61 6d65 203d      child.name =
-00002110: 206b 6579 0d0a 2020 2020 2020 2020 2020   key..          
-00002120: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00002130: 696c 642e 636f 6d70 203d 2063 6d64 5f69  ild.comp = cmd_i
-00002140: 6e73 7461 6e63 650d 0a20 2020 2020 2020  nstance..       
-00002150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002160: 2063 6869 6c64 2e63 6f6d 705f 7479 7065   child.comp_type
-00002170: 203d 2074 7970 6528 636d 645f 696e 7374   = type(cmd_inst
-00002180: 616e 6365 290d 0a0d 0a20 2020 2020 2020  ance)....       
-00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021a0: 2072 6f6f 745f 6974 656d 2e61 7070 656e   root_item.appen
-000021b0: 6443 6869 6c64 2863 6869 6c64 290d 0a0d  dChild(child)...
-000021c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021d0: 2020 2020 2065 6c69 6620 6973 7375 6263       elif issubc
-000021e0: 6c61 7373 2863 6d64 5f69 6e73 7461 6e63  lass(cmd_instanc
-000021f0: 652e 5f5f 636c 6173 735f 5f2c 2049 6e64  e.__class__, Ind
-00002200: 6578 436f 6d6d 616e 6429 3a0d 0a20 2020  exCommand):..   
-00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002220: 2020 2020 2063 6869 6c64 203d 2063 6c73       child = cls
-00002230: 2e6c 6f61 6428 636d 645f 696e 7374 616e  .load(cmd_instan
-00002240: 6365 2c20 726f 6f74 5f69 7465 6d29 0d0a  ce, root_item)..
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2020 2020 2020 2020 6368 696c 642e 6e61          child.na
-00002270: 6d65 203d 206b 6579 0d0a 2020 2020 2020  me = key..      
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 6368 696c 642e 636f 6d70 203d 2063    child.comp = c
-000022a0: 6d64 5f69 6e73 7461 6e63 650d 0a20 2020  md_instance..   
-000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022c0: 2020 2020 2063 6869 6c64 2e63 6f6d 705f       child.comp_
-000022d0: 7479 7065 203d 2074 7970 6528 636d 645f  type = type(cmd_
-000022e0: 696e 7374 616e 6365 290d 0a20 2020 2020  instance)..     
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002300: 2020 2072 6f6f 745f 6974 656d 2e61 7070     root_item.app
-00002310: 656e 6443 6869 6c64 2863 6869 6c64 290d  endChild(child).
-00002320: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00002330: 2020 2020 2020 2065 6c69 6620 6361 6c6c         elif call
-00002340: 6162 6c65 2863 6d64 5f69 6e73 7461 6e63  able(cmd_instanc
-00002350: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00002360: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00002370: 6973 7375 6263 6c61 7373 2863 6d64 5f69  issubclass(cmd_i
-00002380: 6e73 7461 6e63 652e 5f5f 636c 6173 735f  nstance.__class_
-00002390: 5f2c 2074 7970 6529 3a0d 0a20 2020 2020  _, type):..     
+00001d10: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00001d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d30: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d50: 2020 2063 6869 6c64 203d 2063 6c73 2e6c     child = cls.l
+00001d60: 6f61 6428 636d 645f 696e 7374 616e 6365  oad(cmd_instance
+00001d70: 2c20 726f 6f74 5f69 7465 6d2c 2073 6f72  , root_item, sor
+00001d80: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00001d90: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+00001da0: 642e 6e61 6d65 203d 206b 6579 0d0a 2020  d.name = key..  
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 2020 2020 6368 696c 642e 636f 6d70        child.comp
+00001dd0: 203d 2063 6d64 5f69 6e73 7461 6e63 650d   = cmd_instance.
+00001de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001df0: 2020 2020 2020 2020 2063 6869 6c64 2e63           child.c
+00001e00: 6f6d 705f 7479 7065 203d 2074 7970 6528  omp_type = type(
+00001e10: 636d 645f 696e 7374 616e 6365 290d 0a20  cmd_instance).. 
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001e40: 2e61 7070 656e 6443 6869 6c64 2863 6869  .appendChild(chi
+00001e50: 6c64 290d 0a20 2020 2020 2020 2065 6c73  ld)..        els
+00001e60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001e70: 6966 2063 616c 6c61 626c 6528 636f 6d70  if callable(comp
+00001e80: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001e90: 2020 2020 726f 6f74 5f69 7465 6d2e 636f      root_item.co
+00001ea0: 6d70 203d 2063 6f6d 700d 0a20 2020 2020  mp = comp..     
+00001eb0: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
+00001ec0: 6974 656d 2e63 6f6d 705f 7479 7065 203d  item.comp_type =
+00001ed0: 2074 7970 6528 636f 6d70 290d 0a20 2020   type(comp)..   
+00001ee0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00001ef0: 745f 6974 656d 2e69 735f 6d65 7468 6f64  t_item.is_method
+00001f00: 203d 2054 7275 650d 0a0d 0a20 2020 2020   = True....     
+00001f10: 2020 2020 2020 2065 6c69 6620 6973 7375         elif issu
+00001f20: 6263 6c61 7373 2874 7970 6528 636f 6d70  bclass(type(comp
+00001f30: 292c 2043 6f6d 6d61 6e64 293a 0d0a 2020  ), Command):..  
+00001f40: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+00001f50: 6f74 5f69 7465 6d2e 636f 6d70 203d 2063  ot_item.comp = c
+00001f60: 6f6d 700d 0a20 2020 2020 2020 2020 2020  omp..           
+00001f70: 2020 2020 2072 6f6f 745f 6974 656d 2e63       root_item.c
+00001f80: 6f6d 705f 7479 7065 203d 2074 7970 6528  omp_type = type(
+00001f90: 636f 6d70 290d 0a20 2020 2020 2020 2020  comp)..         
+00001fa0: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001fb0: 2e65 7863 6c75 6465 6420 3d20 636f 6d70  .excluded = comp
+00001fc0: 2069 6e20 726f 6f74 5f69 7465 6d2e 7061   in root_item.pa
+00001fd0: 7265 6e74 2829 2e63 6f6d 702e 6578 636c  rent().comp.excl
+00001fe0: 7564 655f 6361 7074 7572 650d 0a20 2020  ude_capture..   
+00001ff0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00002000: 745f 6974 656d 2e72 6177 5f72 656d 6f74  t_item.raw_remot
+00002010: 655f 636f 6d6d 616e 6420 3d20 636f 6d70  e_command = comp
+00002020: 2e72 656d 6f74 655f 636f 6d6d 616e 640d  .remote_command.
+00002030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002040: 2072 6f6f 745f 6974 656d 2e73 6574 5f65   root_item.set_e
+00002050: 6e61 626c 6520 3d20 636f 6d70 2e5f 7365  nable = comp._se
+00002060: 745f 656e 6162 6c65 0d0a 2020 2020 2020  t_enable..      
+00002070: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
+00002080: 7465 6d2e 6765 745f 656e 6162 6c65 203d  tem.get_enable =
+00002090: 2063 6f6d 702e 5f67 6574 5f65 6e61 626c   comp._get_enabl
+000020a0: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
+000020b0: 2065 6c69 6620 6973 7375 6263 6c61 7373   elif issubclass
+000020c0: 2874 7970 6528 636f 6d70 292c 2049 6e64  (type(comp), Ind
+000020d0: 6578 436f 6d6d 616e 6429 3a0d 0a20 2020  exCommand):..   
+000020e0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+000020f0: 745f 6974 656d 2e63 6f6d 7020 3d20 636f  t_item.comp = co
+00002100: 6d70 0d0a 2020 2020 2020 2020 2020 2020  mp..            
+00002110: 2020 2020 726f 6f74 5f69 7465 6d2e 636f      root_item.co
+00002120: 6d70 5f74 7970 6520 3d20 7479 7065 2863  mp_type = type(c
+00002130: 6f6d 7029 0d0a 2020 2020 2020 2020 2020  omp)..          
+00002140: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
+00002150: 6578 636c 7564 6564 203d 2063 6f6d 7020  excluded = comp 
+00002160: 696e 2072 6f6f 745f 6974 656d 2e70 6172  in root_item.par
+00002170: 656e 7428 292e 636f 6d70 2e65 7863 6c75  ent().comp.exclu
+00002180: 6465 5f63 6170 7475 7265 0d0a 2020 2020  de_capture..    
+00002190: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+000021a0: 5f69 7465 6d2e 7261 775f 7265 6d6f 7465  _item.raw_remote
+000021b0: 5f63 6f6d 6d61 6e64 203d 2063 6f6d 702e  _command = comp.
+000021c0: 7265 6d6f 7465 5f63 6f6d 6d61 6e64 0d0a  remote_command..
+000021d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021e0: 726f 6f74 5f69 7465 6d2e 7365 745f 656e  root_item.set_en
+000021f0: 6162 6c65 203d 2063 6f6d 702e 5f73 6574  able = comp._set
+00002200: 5f65 6e61 626c 650d 0a20 2020 2020 2020  _enable..       
+00002210: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
+00002220: 656d 2e67 6574 5f65 6e61 626c 6520 3d20  em.get_enable = 
+00002230: 636f 6d70 2e5f 6765 745f 656e 6162 6c65  comp._get_enable
+00002240: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00002250: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00002260: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002270: 2063 6f6d 702e 696e 6465 785f 6469 6374   comp.index_dict
+00002280: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022a0: 2020 2069 6e64 6578 203d 2063 6f6d 702e     index = comp.
+000022b0: 696e 6465 785f 6d69 6e0d 0a20 2020 2020  index_min..     
+000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022d0: 2020 2077 6869 6c65 2069 6e64 6578 203c     while index <
+000022e0: 3d20 636f 6d70 2e69 6e64 6578 5f6d 6178  = comp.index_max
+000022f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002300: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002310: 6869 6c64 203d 2063 6c73 2e6c 6f61 6428  hild = cls.load(
+00002320: 696e 6465 782c 2072 6f6f 745f 6974 656d  index, root_item
+00002330: 2c20 736f 7274 290d 0a20 2020 2020 2020  , sort)..       
+00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002350: 2020 2020 2063 6869 6c64 2e6e 616d 6520       child.name 
+00002360: 3d20 6627 7b69 6e64 6578 7d27 0d0a 2020  = f'{index}'..  
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+00002390: 636f 6d70 203d 2069 6e64 6578 0d0a 2020  comp = index..  
 000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023b0: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-000023c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000023d0: 2020 2020 2020 2020 2069 6620 6b65 792e           if key.
-000023e0: 7374 6172 7473 7769 7468 2827 5f27 293a  startswith('_'):
-000023f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002400: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00002410: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
+000023b0: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+000023c0: 636f 6d70 5f74 7970 6520 3d20 496e 6465  comp_type = Inde
+000023d0: 780d 0a20 2020 2020 2020 2020 2020 2020  x..             
+000023e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000023f0: 6869 6c64 2e65 7863 6c75 6465 6420 3d20  hild.excluded = 
+00002400: 726f 6f74 5f69 7465 6d2e 6578 636c 7564  root_item.exclud
+00002410: 6564 0d0a 2020 2020 2020 2020 2020 2020  ed..            
 00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002440: 2020 2020 2020 2020 2020 6368 696c 6420            child 
-00002450: 3d20 636c 732e 6c6f 6164 2863 6d64 5f69  = cls.load(cmd_i
-00002460: 6e73 7461 6e63 652c 2072 6f6f 745f 6974  nstance, root_it
-00002470: 656d 290d 0a20 2020 2020 2020 2020 2020  em)..           
-00002480: 2020 2020 2020 2020 2020 2020 2063 6869               chi
-00002490: 6c64 2e6e 616d 6520 3d20 6b65 790d 0a20  ld.name = key.. 
+00002430: 6368 696c 642e 7365 745f 656e 6162 6c65  child.set_enable
+00002440: 203d 2072 6f6f 745f 6974 656d 2e73 6574   = root_item.set
+00002450: 5f65 6e61 626c 650d 0a20 2020 2020 2020  _enable..       
+00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002470: 2020 2020 2063 6869 6c64 2e67 6574 5f65       child.get_e
+00002480: 6e61 626c 6520 3d20 726f 6f74 5f69 7465  nable = root_ite
+00002490: 6d2e 6765 745f 656e 6162 6c65 0d0a 2020  m.get_enable..  
 000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024b0: 2020 2020 2020 2063 6869 6c64 2e63 6f6d         child.com
-000024c0: 7020 3d20 636d 645f 696e 7374 616e 6365  p = cmd_instance
-000024d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000024e0: 2020 2020 2020 2020 2020 6368 696c 642e            child.
-000024f0: 636f 6d70 5f74 7970 6520 3d20 7479 7065  comp_type = type
-00002500: 2863 6d64 5f69 6e73 7461 6e63 6529 0d0a  (cmd_instance)..
-00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002520: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-00002530: 6d2e 6170 7065 6e64 4368 696c 6428 6368  m.appendChild(ch
-00002540: 696c 6429 0d0a 2020 2020 2020 2020 656c  ild)..        el
-00002550: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00002560: 2069 6620 6361 6c6c 6162 6c65 2863 6f6d   if callable(com
-00002570: 7029 3a0d 0a20 2020 2020 2020 2020 2020  p):..           
-00002580: 2020 2020 2072 6f6f 745f 6974 656d 2e63       root_item.c
-00002590: 6f6d 7020 3d20 636f 6d70 0d0a 2020 2020  omp = comp..    
-000025a0: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-000025b0: 5f69 7465 6d2e 636f 6d70 5f74 7970 6520  _item.comp_type 
-000025c0: 3d20 7479 7065 2863 6f6d 7029 0d0a 2020  = type(comp)..  
-000025d0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-000025e0: 6f74 5f69 7465 6d2e 6973 5f6d 6574 686f  ot_item.is_metho
-000025f0: 6420 3d20 5472 7565 0d0a 0d0a 2020 2020  d = True....    
-00002600: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
-00002610: 7562 636c 6173 7328 7479 7065 2863 6f6d  ubclass(type(com
-00002620: 7029 2c20 436f 6d6d 616e 6429 3a0d 0a20  p), Command):.. 
-00002630: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00002640: 6f6f 745f 6974 656d 2e63 6f6d 7020 3d20  oot_item.comp = 
-00002650: 636f 6d70 0d0a 2020 2020 2020 2020 2020  comp..          
-00002660: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
-00002670: 636f 6d70 5f74 7970 6520 3d20 7479 7065  comp_type = type
-00002680: 2863 6f6d 7029 0d0a 2020 2020 2020 2020  (comp)..        
-00002690: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-000026a0: 6d2e 6578 636c 7564 6564 203d 2063 6f6d  m.excluded = com
-000026b0: 7020 696e 2072 6f6f 745f 6974 656d 2e70  p in root_item.p
-000026c0: 6172 656e 7428 292e 636f 6d70 2e65 7863  arent().comp.exc
-000026d0: 6c75 6465 5f63 6170 7475 7265 0d0a 2020  lude_capture..  
-000026e0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-000026f0: 6f74 5f69 7465 6d2e 7261 775f 7265 6d6f  ot_item.raw_remo
-00002700: 7465 5f63 6f6d 6d61 6e64 203d 2063 6f6d  te_command = com
-00002710: 702e 7265 6d6f 7465 5f63 6f6d 6d61 6e64  p.remote_command
-00002720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002730: 2020 726f 6f74 5f69 7465 6d2e 7365 745f    root_item.set_
-00002740: 656e 6162 6c65 203d 2063 6f6d 702e 5f73  enable = comp._s
-00002750: 6574 5f65 6e61 626c 650d 0a20 2020 2020  et_enable..     
-00002760: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
-00002770: 6974 656d 2e67 6574 5f65 6e61 626c 6520  item.get_enable 
-00002780: 3d20 636f 6d70 2e5f 6765 745f 656e 6162  = comp._get_enab
-00002790: 6c65 0d0a 0d0a 2020 2020 2020 2020 2020  le....          
-000027a0: 2020 656c 6966 2069 7373 7562 636c 6173    elif issubclas
-000027b0: 7328 7479 7065 2863 6f6d 7029 2c20 496e  s(type(comp), In
-000027c0: 6465 7843 6f6d 6d61 6e64 293a 0d0a 2020  dexCommand):..  
-000027d0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-000027e0: 6f74 5f69 7465 6d2e 636f 6d70 203d 2063  ot_item.comp = c
-000027f0: 6f6d 700d 0a20 2020 2020 2020 2020 2020  omp..           
-00002800: 2020 2020 2072 6f6f 745f 6974 656d 2e63       root_item.c
-00002810: 6f6d 705f 7479 7065 203d 2074 7970 6528  omp_type = type(
-00002820: 636f 6d70 290d 0a20 2020 2020 2020 2020  comp)..         
-00002830: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
-00002840: 2e65 7863 6c75 6465 6420 3d20 636f 6d70  .excluded = comp
-00002850: 2069 6e20 726f 6f74 5f69 7465 6d2e 7061   in root_item.pa
-00002860: 7265 6e74 2829 2e63 6f6d 702e 6578 636c  rent().comp.excl
-00002870: 7564 655f 6361 7074 7572 650d 0a20 2020  ude_capture..   
-00002880: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-00002890: 745f 6974 656d 2e72 6177 5f72 656d 6f74  t_item.raw_remot
-000028a0: 655f 636f 6d6d 616e 6420 3d20 636f 6d70  e_command = comp
-000028b0: 2e72 656d 6f74 655f 636f 6d6d 616e 640d  .remote_command.
-000028c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000028d0: 2072 6f6f 745f 6974 656d 2e73 6574 5f65   root_item.set_e
-000028e0: 6e61 626c 6520 3d20 636f 6d70 2e5f 7365  nable = comp._se
-000028f0: 745f 656e 6162 6c65 0d0a 2020 2020 2020  t_enable..      
-00002900: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
-00002910: 7465 6d2e 6765 745f 656e 6162 6c65 203d  tem.get_enable =
-00002920: 2063 6f6d 702e 5f67 6574 5f65 6e61 626c   comp._get_enabl
-00002930: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-00002940: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00002950: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002960: 6620 636f 6d70 2e69 6e64 6578 5f64 6963  f comp.index_dic
-00002970: 7420 6973 204e 6f6e 653a 0d0a 2020 2020  t is None:..    
-00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 2020 2020 696e 6465 7820 3d20 636f 6d70      index = comp
-000029a0: 2e69 6e64 6578 5f6d 696e 0d0a 2020 2020  .index_min..    
-000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029c0: 2020 2020 7768 696c 6520 696e 6465 7820      while index 
-000029d0: 3c3d 2063 6f6d 702e 696e 6465 785f 6d61  <= comp.index_ma
-000029e0: 783a 0d0a 2020 2020 2020 2020 2020 2020  x:..            
-000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a00: 6368 696c 6420 3d20 636c 732e 6c6f 6164  child = cls.load
-00002a10: 2869 6e64 6578 2c20 726f 6f74 5f69 7465  (index, root_ite
-00002a20: 6d29 0d0a 2020 2020 2020 2020 2020 2020  m)..            
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a40: 6368 696c 642e 6e61 6d65 203d 2066 277b  child.name = f'{
-00002a50: 696e 6465 787d 270d 0a20 2020 2020 2020  index}'..       
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 2020 2020 2063 6869 6c64 2e63 6f6d 7020       child.comp 
-00002a80: 3d20 696e 6465 780d 0a20 2020 2020 2020  = index..       
-00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002aa0: 2020 2020 2063 6869 6c64 2e63 6f6d 705f       child.comp_
-00002ab0: 7479 7065 203d 2049 6e64 6578 0d0a 2020  type = Index..  
-00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ad0: 2020 2020 2020 2020 2020 6368 696c 642e            child.
-00002ae0: 6578 636c 7564 6564 203d 2072 6f6f 745f  excluded = root_
-00002af0: 6974 656d 2e65 7863 6c75 6465 640d 0a20  item.excluded.. 
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00002b20: 2e73 6574 5f65 6e61 626c 6520 3d20 726f  .set_enable = ro
-00002b30: 6f74 5f69 7465 6d2e 7365 745f 656e 6162  ot_item.set_enab
-00002b40: 6c65 0d0a 2020 2020 2020 2020 2020 2020  le..            
-00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b60: 6368 696c 642e 6765 745f 656e 6162 6c65  child.get_enable
-00002b70: 203d 2072 6f6f 745f 6974 656d 2e67 6574   = root_item.get
-00002b80: 5f65 6e61 626c 650d 0a20 2020 2020 2020  _enable..       
-00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ba0: 2020 2020 2072 6f6f 745f 6974 656d 2e61       root_item.a
-00002bb0: 7070 656e 6443 6869 6c64 2863 6869 6c64  ppendChild(child
-00002bc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002bd0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002be0: 6e64 6578 202b 3d20 310d 0a20 2020 2020  ndex += 1..     
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00002c00: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00002c10: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00002c20: 7220 6b65 7920 696e 2063 6f6d 702e 696e  r key in comp.in
-00002c30: 6465 785f 6469 6374 3a0d 0a20 2020 2020  dex_dict:..     
-00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c50: 2020 2020 2020 2063 6869 6c64 203d 2063         child = c
-00002c60: 6c73 2e6c 6f61 6428 6b65 792c 2072 6f6f  ls.load(key, roo
-00002c70: 745f 6974 656d 290d 0a20 2020 2020 2020  t_item)..       
-00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c90: 2020 2020 2063 6869 6c64 2e6e 616d 6520       child.name 
-00002ca0: 3d20 6627 7b6b 6579 7d27 0d0a 2020 2020  = f'{key}'..    
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cc0: 2020 2020 2020 2020 6368 696c 642e 636f          child.co
-00002cd0: 6d70 203d 206b 6579 0d0a 2020 2020 2020  mp = key..      
-00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cf0: 2020 2020 2020 6368 696c 642e 636f 6d70        child.comp
-00002d00: 5f74 7970 6520 3d20 496e 6465 780d 0a20  _type = Index.. 
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d20: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00002d30: 2e65 786c 7564 6564 203d 2072 6f6f 745f  .exluded = root_
-00002d40: 6974 656d 2e65 7863 6c75 6465 640d 0a20  item.excluded.. 
-00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d60: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00002d70: 2e73 6574 5f65 6e61 626c 6520 3d20 636f  .set_enable = co
-00002d80: 6d70 2e5f 7365 745f 656e 6162 6c65 0d0a  mp._set_enable..
-00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002da0: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00002db0: 642e 6765 745f 656e 6162 6c65 203d 2063  d.get_enable = c
-00002dc0: 6f6d 702e 5f67 6574 5f65 6e61 626c 650d  omp._get_enable.
-00002dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002de0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-00002df0: 745f 6974 656d 2e61 7070 656e 6443 6869  t_item.appendChi
-00002e00: 6c64 2863 6869 6c64 290d 0a20 2020 2020  ld(child)..     
-00002e10: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00002e20: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00002e30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002e40: 2020 2020 2020 2070 7269 6e74 2866 2720         print(f' 
-00002e50: 207b 7479 7065 2865 297d 207b 657d 2063   {type(e)} {e} c
-00002e60: 6f6d 6d61 6e64 3a7b 636f 6d70 2e72 656d  ommand:{comp.rem
-00002e70: 6f74 655f 636f 6d6d 616e 647d 2729 0d0a  ote_command}')..
-00002e80: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00002e90: 6f6f 745f 6974 656d 0d0a                 oot_item..
+000024b0: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
+000024c0: 7465 6d2e 6170 7065 6e64 4368 696c 6428  tem.appendChild(
+000024d0: 6368 696c 6429 0d0a 2020 2020 2020 2020  child)..        
+000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024f0: 2020 2020 696e 6465 7820 2b3d 2031 0d0a      index += 1..
+00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002510: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002530: 2020 2066 6f72 206b 6579 2069 6e20 636f     for key in co
+00002540: 6d70 2e69 6e64 6578 5f64 6963 743a 0d0a  mp.index_dict:..
+00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002560: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+00002570: 6420 3d20 636c 732e 6c6f 6164 286b 6579  d = cls.load(key
+00002580: 2c20 726f 6f74 5f69 7465 6d2c 2073 6f72  , root_item, sor
+00002590: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 6368 696c 642e 6e61 6d65 203d 2066 277b  child.name = f'{
+000025c0: 6b65 797d 270d 0a20 2020 2020 2020 2020  key}'..         
+000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025e0: 2020 2063 6869 6c64 2e63 6f6d 7020 3d20     child.comp = 
+000025f0: 6b65 790d 0a20 2020 2020 2020 2020 2020  key..           
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2063 6869 6c64 2e63 6f6d 705f 7479 7065   child.comp_type
+00002620: 203d 2049 6e64 6578 0d0a 2020 2020 2020   = Index..      
+00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002640: 2020 2020 2020 6368 696c 642e 6578 6c75        child.exlu
+00002650: 6465 6420 3d20 726f 6f74 5f69 7465 6d2e  ded = root_item.
+00002660: 6578 636c 7564 6564 0d0a 2020 2020 2020  excluded..      
+00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002680: 2020 2020 2020 6368 696c 642e 7365 745f        child.set_
+00002690: 656e 6162 6c65 203d 2063 6f6d 702e 5f73  enable = comp._s
+000026a0: 6574 5f65 6e61 626c 650d 0a20 2020 2020  et_enable..     
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026c0: 2020 2020 2020 2063 6869 6c64 2e67 6574         child.get
+000026d0: 5f65 6e61 626c 6520 3d20 636f 6d70 2e5f  _enable = comp._
+000026e0: 6765 745f 656e 6162 6c65 0d0a 2020 2020  get_enable..    
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002700: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
+00002710: 6d2e 6170 7065 6e64 4368 696c 6428 6368  m.appendChild(ch
+00002720: 696c 6429 0d0a 2020 2020 2020 2020 2020  ild)..          
+00002730: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00002740: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 7072 696e 7428 6627 2020 7b74 7970    print(f'  {typ
+00002770: 6528 6529 7d20 7b65 7d20 636f 6d6d 616e  e(e)} {e} comman
+00002780: 643a 7b63 6f6d 702e 7265 6d6f 7465 5f63  d:{comp.remote_c
+00002790: 6f6d 6d61 6e64 7d20 696e 6465 783a 207b  ommand} index: {
+000027a0: 696e 6465 787d 2729 0d0a 2020 2020 2020  index}')..      
+000027b0: 2020 7265 7475 726e 2072 6f6f 745f 6974    return root_it
+000027c0: 656d 0d0a                                em..
```

### Comparing `srsgui-0.2.16/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandmodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,60 @@
 
+import time
+import json
 import sys
-
 from typing import Any, Iterable, List, Dict, Union
 
 from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView
 from srsgui.ui.qt.QtGui import QBrush, QColor
-from srsgui.ui.qt.QtCore import QAbstractItemModel, QModelIndex, \
-                                QObject, Qt, Signal
+from srsgui.ui.qt.QtCore import QAbstractItemModel, QModelIndex, QObject, Qt, QFileInfo
 
 from srsgui import Component
 
 from .commanditem import CommandItem, Index
 from .commanddelegate import CommandDelegate
-from .commandhandler import CommandHandler
 
 
 class CommandModel(QAbstractItemModel):
     """ An editable model of Command and Component """
 
-    # Signal to request to process a query to an outside command processor
-    query_requested = Signal(QModelIndex)
-
-    # Signal to request to process a set to an outside command processor
-    set_requested = Signal(tuple)
-
-    # Signal to display full Python command to CommandTerminal
-    set_command_sent = Signal(str, str)
-
     def __init__(self, parent: QObject = None):
         super().__init__(parent)
 
+        self.show_methods = True
+        self.show_excluded = True
+        self.show_set_only = True
+        self.show_query_only = True
         self.show_raw_remote_command = True
 
         self._rootItem = CommandItem()
-        self._headers = ("  Command  ", "  Value  ")
+        self._headers = ("  command  ", "  value  ")
 
     def clear(self):
         """ Clear data from the model """
         self.load(Component())
 
-    def load(self, document: Component):
+    def load(self, document: Component, sort=False):
         """Load model from a nested dictionary returned by json.loads()
 
         Arguments:
             document (dict): JSON-compatible dictionary
         """
 
         assert isinstance(
             document, Component
-        ), "`document` must be a Component, " f"not {type(document)}"
+        ), "`document` must be of dict, list or tuple, " f"not {type(document)}"
 
         self.beginResetModel()
 
-        self._rootItem = CommandItem.load(document)
+        self._rootItem = CommandItem.load(document, sort=sort)
         self._rootItem.value_type = type(document)
 
         self.endResetModel()
+
         return True
 
     def data(self, index: QModelIndex, role: Qt.ItemDataRole) -> Any:
         """Override from QAbstractItemModel
 
         Return data from an item according index and role
         """
@@ -70,72 +65,76 @@
         if role == Qt.DisplayRole:
             if index.column() == 0:
                 item = index.internalPointer()
                 name = item.name
 
                 if self.show_raw_remote_command:
                     name += f' <{item.raw_remote_command}>' if item.raw_remote_command else ''
-
-                name += ' [M]' if item.is_method else ''
-                name += ' [EX]' if item.excluded else ''
-                name += ' [SO]' if item.set_enable and not item.get_enable else ''
-                name += ' [QO]' if item.get_enable and not item.set_enable else ''
+                if self.show_methods:
+                    name += ' [M]' if item.is_method else ''
+                if self.show_excluded:
+                    name += ' [EX]' if item.excluded else ''
+                if self.show_set_only:
+                    name += ' [SO]' if item.set_enable and not item.get_enable else ''
+                if self.show_query_only:
+                    name += ' [QO]' if item.get_enable and not item.set_enable else ''
                 return name
 
             if index.column() == 1:
                 item = index.internalPointer()
-                self.query_requested.emit(index)
-                return item.get_formatted_value()
+                v = item.value
+                if v is None:
+                    return
+                unit = item.get_unit()
+                fmt = item.get_format()
+                try:
+                    if unit:
+                        val = f'{v:{fmt}}  {item.get_unit()}'
+                    else:
+                        val = f'{v:{fmt}}'
+                except ValueError:
+                    print(f'ValueError: {item.raw_remote_command} {v} {fmt} {unit}')
+                    val = f'{v}'
+                return val
 
         elif role == Qt.EditRole:
             if index.column() == 1:
                 item = index.internalPointer()
-                self.query_requested.emit(index)
-                return item.value
+                val = item.value
+                # print('data', item.name, item.comp, val)
+                return val
 
         elif role == Qt.BackgroundRole:
             item = index.internalPointer()
             if item.comp_type != Index and issubclass(item.comp_type, Component):
                 return QBrush(QColor(243, 230, 225))
             if item.row() % 2 == 0:
                 return QBrush(QColor(240, 240, 253))
 
-        elif role == Qt.ToolTipRole:
-            item = index.internalPointer()
-            if item.is_method or issubclass(item.comp_type, Component):
-                if hasattr(item.comp, '__doc__') and index.column() == 0:
-                    return item.comp.__doc__
-
     def setData(self, index: QModelIndex, value: Any, role: Qt.ItemDataRole):
         """Override from QAbstractItemModel
 
         Set CommandItem according to index and role
 
         Args:
             index (QModelIndex)
             value (Any)
             role (Qt.ItemDataRole)
         """
 
         if role == Qt.EditRole:
-
             if index.column() == 1:
                 item = index.internalPointer()
-                self.set_requested.emit((index, value))
-                sent_command = item.construct_set_command_string(value)
-                self.set_command_sent.emit(sent_command, None)
-
-                # item.set_value(value)
-                # self.dataChanged.emit(index, index, [Qt.EditRole])
+                item.set_value(value)
+                self.dataChanged.emit(index, index, [Qt.EditRole])
                 return True
-
             return False
     
     def headerData(self, section: int, orientation: Qt.Orientation,
-                   role: Qt.ItemDataRole):
+                   role: Qt.ItemDataRole    ):
         """Override from QAbstractItemModel
 
         it returns only data for columns (orientation = Horizontal)
         """
         if role != Qt.DisplayRole:
             return None
 
@@ -216,24 +215,14 @@
         """Return True if item is editable, False otherwise"""
         item = index.internalPointer()
         if type(item) == CommandItem:
             return item.is_editable()
         else:
             return False
 
-    def handle_command(self, cmd_tuple):
-        """
-        External command processor calls this slot once a command is processed
-        """
-        index = cmd_tuple[0]
-        value = cmd_tuple[1]
-        changed = cmd_tuple[2]
-        if changed:
-            self.dataChanged.emit(index, index, [Qt.DisplayRole, Qt.EditRole])
-
 
 if __name__ == "__main__":
     from srsinst.sr860 import SR860
 
     app = QApplication(sys.argv)
     view = QTreeView()
     delegate = CommandDelegate()
```

### Comparing `srsgui-0.2.16/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandspinbox.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 from srsgui.ui.qt.QtWidgets import QApplication, QWidget, QSpinBox, QDoubleSpinBox, \
                                    QLabel, QFormLayout, QWidget, QPushButton, \
                                    QHBoxLayout, QSpacerItem, QSizePolicy
 
 
 class IntegerSpinBox(QSpinBox):
     """
-    Adjust step size depending on the cursor position
+    Adjust step size depending on the cursor postion
     """
 
     def stepBy(self, steps):
         prefix_len = len(self.prefix())
-        suffix_len = len(self.suffix())
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
         cur_pos = self.lineEdit().cursorPosition()
-        sep_pos = len(text) - suffix_len
+        sep_pos = len(text)
 
         if cur_pos < min_pos:
             return
 
         exponent = sep_pos - cur_pos
 
         single_step = 10 ** exponent
@@ -33,94 +32,89 @@
         super().stepBy(steps)
 
         self.lineEdit().deselect()
 
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
-        new_sep_pos = len(text) - suffix_len
+        new_sep_pos = len(text)
 
         new_cur_pos = cur_pos + new_sep_pos - sep_pos
         if new_cur_pos < min_pos:
             new_cur_pos = min_pos
         self.lineEdit().setCursorPosition(new_cur_pos)
 
 
 class FloatSpinBox(QDoubleSpinBox):
     """
-    Adjust step size depending on the cursor position
+    Adjust step size depending on the cursor postion
     """
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.minimum_step = 0.1
         self.significant_figures = 4
-        self.precision = 3
-        self.decis = 3
+        self.precision = 1
 
     def set_minimum_step(self, value):
         self.minimum_step = value
         step = self.minimum_step if self.minimum_step > 1e-12 else 1e-12
-        self.decis = math.ceil(-math.log10(step))
+        self.decimals = math.ceil(math.log10(1.0 / step))
 
     def set_significant_figures(self, value):
         self.significant_figures = value
 
     def valueFromText(self, text):
         try:
             if self.suffix():
                 unit_len = len(self.suffix())
                 value = float(text[:-unit_len])
-
             else:
                 value = float(text)
             if value < self.minimum():
                 value = self.minimum()
             elif value > self.maximum():
                 value = self.maximum()
-
         except ValueError:
             print('valueFromText ValueError', text, self.suffix())
             value = self.minimum()
         return value
 
     def textFromValue(self, value):
-        prec = self.decis
+        prec = self.decimals
         try:
             if value == 0:
                 return '0.0'
 
             digits = math.ceil(math.log10(abs(value)))
-            """
+            # digits = 0 if digits < 0 else digits
+
             if digits == self.significant_figures:
                 step = 1
             else:
                 step = 10 ** (digits - self.significant_figures)
             value = round(value / step) * step
-            """
             prec = self.significant_figures - digits
-            prec = self.decis if prec > self.decis else prec
-            prec = 0 if prec < 0 else prec
-            self.precision = prec
-            format_string = '{:.' + str(prec) + 'f}'
-            text = format_string.format(value)
+            if prec > self.decimals:
+                prec = self.decimals
         except Exception as e:
             print(e)
-            return ''
+        self.precision = prec
+        format_string = '{:.' + str(prec) + 'f}'
+        text = format_string.format(value)
         return text
 
     def stepBy(self, steps):
         prefix_len = len(self.prefix())
-        suffix_len = len(self.suffix())
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
         cur_pos = self.lineEdit().cursorPosition()
         sep_pos = text.find('.')
         if sep_pos < 0:
-            sep_pos = len(text) - suffix_len
+            sep_pos = len(text)
 
         if cur_pos < min_pos:
             return
 
         exponent = sep_pos - cur_pos
         if exponent == -1:
             cur_pos += 1
@@ -136,15 +130,15 @@
         self.lineEdit().deselect()
 
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
         new_sep_pos = text.find('.')
         if new_sep_pos < 0:
-            new_sep_pos = len(text) - suffix_len
+            new_sep_pos = len(text)
 
         new_cur_pos = cur_pos + new_sep_pos - sep_pos
         if new_cur_pos < min_pos:
             new_cur_pos = min_pos
         self.lineEdit().setCursorPosition(new_cur_pos)
```

### Comparing `srsgui-0.2.16/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandtreeview.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import inspect
 import logging
 
 from srsgui.ui.qt.QtCore import Qt, QModelIndex
-from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView
+from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView, QPushButton
 
 from .commandmodel import CommandModel
 from .commanddelegate import CommandDelegate
 from .commandspinbox import RunButton
 
 
 class CommandTreeView(QTreeView):
@@ -47,20 +47,15 @@
         for i in range(self.model().rowCount(parent)):
             index = self.model().index(i, 0, parent)
             self.connect_methods_to_buttons(index)
             try:
                 item = index.internalPointer()
                 if item.is_method:
                     widget_index = self.model().index(i, 1, parent)
-                    spec = inspect.getfullargspec(item.comp)
-                    if spec.defaults is None:
-                        flag = len(spec.args) == 1
-                    else:
-                        flag = len(spec.args) - len(spec.defaults) == 1
-                    if flag:
+                    if len(inspect.getfullargspec(item.comp).args) == 1:
                         parent_comp = item.parent().comp
                         meth = getattr(parent_comp, item.name)
                         if meth and meth.__func__ in parent_comp.allow_run_button:
                             button = RunButton()
                             button.pressed.connect(meth)
                             self.setIndexWidget(widget_index, button)
             except Exception as e:
```

### Comparing `srsgui-0.2.16/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,19 +8,14 @@
 from .commandmodel import CommandModel
 from .commanddelegate import CommandDelegate
 
 logger = logging.getLogger(__name__)
 
 
 class CommandTreeWidget(QWidget, Ui_CommandTreeWidget):
-    """
-    CommandTreeWidget is used to display an Instrument class in a tree view
-    based on Qt Model/View architecture.
-    """
-
     def __init__(self, parent=None):
         super(CommandTreeWidget, self).__init__(parent)
         self.parent = parent
         self.setupUi(self)
 
         self.inst = None
         self.name = None
@@ -65,21 +60,20 @@
     def on_method_changed(self, state):
         self.tree_view.method_included = state
         self.tree_view.update_item_display()
 
     def on_raw_command_changed(self, state):
         self.tree_view.show_raw_command = state
         self.model.show_raw_remote_command = self.tree_view.show_raw_command
-        self.model.dataChanged.emit(QModelIndex(), QModelIndex())
 
     def on_capture_clicked(self):
         if self.inst is not None and self.inst.is_connected():
             try:
                 self.model.show_raw_remote_command = self.show_raw_command
-                self.model.load(self.inst)
+                self.model.load(self.inst, False)
                 self.tree_view.expandToDepth(1)
                 self.tree_view.resizeColumnToContents(0)
                 # self.tree_view.collapseAll()
                 self.tree_view.update_item_display()
                 self.tree_view.connect_methods_to_buttons()
 
             except Exception as e:
@@ -89,16 +83,14 @@
 
     def on_expand_clicked(self):
         self.tree_view.expandAll()
 
     def on_collapse_clicked(self):
         self.tree_view.collapseAll()
 
-    def closeEvent(self, event) -> None:
-        self.model.command_handler.stop()
 
 if __name__ == '__main__':
     import sys
     from srsgui.ui.qt.QtWidgets import QApplication, QHeaderView
     from srsinst.sr860 import SR860
 
     app = QApplication(sys.argv)
```

### Comparing `srsgui-0.2.16/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/connectdlg.py` & `srsgui-0.2.9/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/deviceinfohandler.py` & `srsgui-0.2.9/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/dockhandler.py` & `srsgui-0.2.9/srsgui/ui/dockhandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 
 from matplotlib.figure import Figure
 import matplotlib.image as mpimg
 
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 
-from .commandhandler import CommandHandler as TerminalCommandHandler
-from .commandtree.commandhandler import CommandHandler as CommandTreeCommandHandler
-
 from .commandterminal import CommandTerminal
-
 # from .commandtree.commandcapturewidget import CommandCaptureWidget
 from .commandtree.commandtreewidget import CommandTreeWidget
 
 logger = logging.getLogger(__name__)
 
 # define matplotlib level before importing to suppress debug messages
 logging.getLogger('matplotlib').setLevel(logging.WARNING)
@@ -60,20 +56,14 @@
             parent.menu_Docks.triggered.disconnect()
         except:
             pass
         actions = parent.menu_Docks.actions()
         for action in actions:
             parent.menu_Docks.removeAction(action)
 
-        # terminal_command_handler needs to access to self.parent.inst_dict
-        self.terminal_command_handler = TerminalCommandHandler(self.parent)
-
-        # CommandItemModel uses command_tree_command_handler to access Commands
-        self.command_tree_command_handler = CommandTreeCommandHandler()
-
         self.init_figure_dock(self.DefaultFigureName)
         self.init_terminal()
         self.init_console()
         self.init_inst_dock('instrument info')
         list(self.dock_dict.values())[-1].hide()
 
         fig = self.dock_dict.pop(self.DefaultFigureName)
@@ -149,19 +139,14 @@
             terminal_dock.setWindowTitle(name)
             terminal_dock.setMinimumSize(250, 150)
 
             self.terminal_widget = CommandTerminal(self.parent)
             terminal_dock.setWidget(self.terminal_widget)
             self.parent.addDockWidget(Qt.RightDockWidgetArea, terminal_dock)
             self.dock_dict[name] = terminal_dock
-
-            # Commands from terminal are processed by terminal_command_handler
-            self.terminal_widget.command_requested.connect(self.terminal_command_handler.process_command)
-            self.terminal_command_handler.command_processed.connect(self.terminal_widget.handle_command)
-
         except Exception as e:
             logger.error(e)
 
     def init_inst_dock(self, name):
         try:
             inst_dock = QDockWidget(self.parent)
             inst_dock.setObjectName(name)
@@ -170,21 +155,14 @@
             title = self.TitleFormat.format(name)
             inst_dock.setWindowTitle(title)
             inst_dock.setMinimumSize(200, 350)
 
             # inst_dock.command_capture_widget = CommandCaptureWidget(self.parent)
             inst_dock.command_capture_widget = CommandTreeWidget(self.parent)
 
-            # Connect the command handler in parent to signals and slots in CommandModel
-            inst_dock.command_capture_widget.model.set_command_sent.connect(self.terminal_widget.handle_command)
-            inst_dock.command_capture_widget.model.query_requested.connect(self.command_tree_command_handler.worker.handle_query)
-            inst_dock.command_capture_widget.model.set_requested.connect(self.command_tree_command_handler.worker.handle_set)
-            self.command_tree_command_handler.worker.query_processed.connect(inst_dock.command_capture_widget.model.handle_command)
-            self.command_tree_command_handler.worker.set_processed.connect(inst_dock.command_capture_widget.model.handle_command)
-
             inst_dock.setWidget(inst_dock.command_capture_widget)
             self.parent.addDockWidget(Qt.LeftDockWidgetArea, inst_dock)
             self.dock_dict[title] = inst_dock
             self.active_inst_dock_names.append(title)
             if len(self.active_inst_dock_names) > 1:
                 self.parent.tabifyDockWidget(
                     self.dock_dict[self.active_inst_dock_names[0]], inst_dock)
@@ -380,11 +358,7 @@
                     dock.toolbar.show()
         else:
             self.action_toolbar.setText('Show Toolbar')
             self.toolbar_visible = False
             for dock in self.dock_dict.values():
                 if hasattr(dock, 'toolbar'):
                     dock.toolbar.hide()
-
-    def stop_command_handlers(self):
-        self.terminal_command_handler.stop()
-        self.command_tree_command_handler.stop()
```

### Comparing `srsgui-0.2.16/srsgui/ui/inputpanel.py` & `srsgui-0.2.9/srsgui/ui/inputpanel.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,24 +91,24 @@
                     if not self.inst_dict[self.inst_name].is_connected:
                         raise ValueError('{} is not connected'.format(self.inst_name))
 
                     p.set_inst_name(self.inst_name)
                     if issubclass(p.cmd_instance.__class__, IntCommand) or \
                        issubclass(p.cmd_instance.__class__, IntIndexCommand):
                         widget = QSpinBox()
-                        widget.setSuffix(' ' + p.cmd_instance.unit)
+                        widget.setSuffix(p.cmd_instance.unit)
                         widget.setMaximum(p.cmd_instance.maximum)
                         widget.setMinimum(p.cmd_instance.minimum)
                         widget.setSingleStep(p.cmd_instance.step)
                         widget.setAlignment(Qt.AlignRight)
 
                     elif issubclass(p.cmd_instance.__class__, FloatCommand) or \
                          issubclass(p.cmd_instance.__class__, FloatIndexCommand):
                         widget = QDoubleSpinBox()
-                        widget.setSuffix(' ' + p.cmd_instance.unit)
+                        widget.setSuffix(p.cmd_instance.unit)
                         widget.setMaximum(p.cmd_instance.maximum)
                         widget.setMinimum(p.cmd_instance.minimum)
                         widget.setSingleStep(p.cmd_instance.step)
                         widget.setDecimals(math.ceil(math.log10(1.0 / p.cmd_instance.step)))
                         widget.setAlignment(Qt.AlignRight)
 
                     elif issubclass(p.cmd_instance.__class__, DictCommand) or \
@@ -152,15 +152,15 @@
                     widget.setMaximum(p.value)
                     widget.setEnabled(False)
                 else:
                     widget.setMinimum(p.minimum)
                     widget.setMaximum(p.maximum)
                     widget.setEnabled(True)
                 widget.setSingleStep(p.single_step)
-                widget.setSuffix(' ' + p.suffix)
+                widget.setSuffix(p.suffix)
                 widget.setValue(p.value)
 
                 label = QLabel(name.capitalize())
                 layout.addWidget(label, row, self.FirstColumn)
                 layout.addWidget(widget, row, self.SecondColumn)
                 row += 1
```

### Comparing `srsgui-0.2.16/srsgui/ui/qt/QtCore.py` & `srsgui-0.2.9/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/qt/QtGui.py` & `srsgui-0.2.9/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.2.9/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/qt/__init__.py` & `srsgui-0.2.9/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/qtloghandler.py` & `srsgui-0.2.9/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/resource_rc.py` & `srsgui-0.2.9/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/signalhandler.py` & `srsgui-0.2.9/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/srslogo.jpg` & `srsgui-0.2.9/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/stdout.py` & `srsgui-0.2.9/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/taskmain.py` & `srsgui-0.2.9/srsgui/ui/taskmain.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 from .inputpanel import InputPanel
 from .signalhandler import SignalHandler
 
 from .stdout import StdOut
 from .qtloghandler import QtLogHandler
 from .deviceinfohandler import DeviceInfoHandler
-
 from .dockhandler import DockHandler
+from .commandhandler import CommandHandler
 
 from srsgui.task.config import Config
 from srsgui.task.sessionhandler import SessionHandler
 from srsgui.task.task import Task, Bold
 
 from srsgui import __version__
 
@@ -73,20 +73,22 @@
         self.data_dict = {}
 
         # self.inst_dict holds instances of subclass of Instrument
         self.inst_dict = {}
         self.inst_info_handler = DeviceInfoHandler(self)
 
         self.dock_handler = DockHandler(self)
-        self.command_handler = self.dock_handler.terminal_command_handler
         self.console = self.dock_handler.console
         self.terminal_widget = self.dock_handler.terminal_widget
         self.plotDockWidget = self.dock_handler.get_dock()
 
         # Make the terminal not blocking for log query
+        self.command_handler = CommandHandler(self)
+        self.terminal_widget.command_requested.connect(self.command_handler.process_command)
+        self.command_handler.command_processed.connect(self.terminal_widget.handle_command)
 
         self.geometry_dict = {}
         try:
             default_config_file = self.DefaultConfigFile
             self.config = Config()
             self.base_data_dir = self.config.base_data_dir
             self.base_log_file_name = self.config.base_log_file_name
@@ -218,43 +220,44 @@
             for name in self.task_dict:
                 m = self.menu_Tasks
 
                 # set up submenu structure
                 p = self.config.task_path_dict[name]
                 if p:
                     tokens = p.split('/')
+                    exists = False
                     for token in tokens:
-                        exists = False
-                        na = None
                         if type(m) == QAction:
                             ma = m.menu()
                             if ma:
                                 m = ma
                             else:
                                 continue
                         for action in m.actions():
                             if token == action.text():
                                 na = action
                                 exists = True
                                 break
                         if not exists:
                             na = m.addMenu(QMenu(token, m))
                         m = na
+                        exists = False
                     if type(m) == QAction:
                         ma = m.menu()
                         if ma:
                             m = ma
                         else:
                             continue
                 action_task = QAction(self)
                 action_task.setText(name)
                 m.addAction(action_task)
         except Exception as e:
             logger.error('Error adding to Task menu Task:{}  Error: {}'.format(name, e))
 
+
     def get_logo_file(self):
         return self.LogoFile
 
     def print_redirect(self, text):
         """
         Handles text output for stdout, stderr and various text output
         from :class:`srsgui.task.task.Task`
@@ -553,15 +556,15 @@
             logger.error('display_question error: {}'.format(e))
 
     def closeEvent(self, event):
         if self.okToContinue():
             # Save settings
             self.save_settings()
 
-            self.dock_handler.stop_command_handlers()
+            self.command_handler.stop()
 
             # Close instruments
             inst_dict = self.inst_dict
             for key in inst_dict:
                 if hasattr(inst_dict[key], "disconnect"):
                     inst_dict[key].disconnect()
         else:
@@ -581,20 +584,15 @@
         except Exception as e:
             logger.error(f"Error in handle_initial_image: {e}")
 
     def onAbout(self,checked):
         msg = ''
         for name in self.inst_dict:
             inst = self.inst_dict[name]
-            if hasattr(inst, __version__):
-                version = inst.__version__
-            else:
-                version = 'N/A'
-
-            msg += '{} version: {}\n'.format(inst.__class__.__name__, version)
+            msg += '{} version: {}\n'.format(inst.__class__.__name__, inst.__version__)
         msg += '\nSrsgui version: {}\n'.format(__version__)
         msg += '\n{} version: {}\n'.format(QT_BINDER, QT_BINDER_VERSION)
         msg += 'Python version: {}\n'.format(sys.version)
         self.display_question(msg, None)
 
     def load_settings(self):
         try:
```

### Comparing `srsgui-0.2.16/srsgui/ui/taskmain.ui` & `srsgui-0.2.9/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui/ui/ui_taskmain.py` & `srsgui-0.2.9/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.16/srsgui.egg-info/PKG-INFO` & `srsgui-0.2.9/srsgui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.16
+Version: 0.2.9
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.16/srsgui.egg-info/SOURCES.txt` & `srsgui-0.2.9/srsgui.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -77,20 +77,22 @@
 srsgui/ui/resource_rc.py
 srsgui/ui/signalhandler.py
 srsgui/ui/srslogo.jpg
 srsgui/ui/stdout.py
 srsgui/ui/taskmain.py
 srsgui/ui/taskmain.ui
 srsgui/ui/ui_taskmain.py
-srsgui/ui/commandtree/__init__.py
+srsgui/ui/commandtree/commandcapturewidget.py
+srsgui/ui/commandtree/commandcapturewidget.ui
 srsgui/ui/commandtree/commanddelegate.py
-srsgui/ui/commandtree/commandhandler.py
 srsgui/ui/commandtree/commanditem.py
 srsgui/ui/commandtree/commandmodel.py
 srsgui/ui/commandtree/commandspinbox.py
 srsgui/ui/commandtree/commandtreeview.py
 srsgui/ui/commandtree/commandtreewidget.py
+srsgui/ui/commandtree/jsonmodel.py
+srsgui/ui/commandtree/ui_commandcapturewidget.py
 srsgui/ui/commandtree/ui_commandtreewidget.py
 srsgui/ui/qt/QtCore.py
 srsgui/ui/qt/QtGui.py
 srsgui/ui/qt/QtWidgets.py
 srsgui/ui/qt/__init__.py
```

