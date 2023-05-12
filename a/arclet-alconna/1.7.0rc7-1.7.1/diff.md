# Comparing `tmp/arclet-alconna-1.7.0rc7.tar.gz` & `tmp/arclet-alconna-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.0rc7.tar", last modified: Tue May  9 04:08:31 2023, max compression
+gzip compressed data, was "arclet-alconna-1.7.1.tar", last modified: Fri May 12 08:36:21 2023, max compression
```

## Comparing `arclet-alconna-1.7.0rc7.tar` & `arclet-alconna-1.7.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc7/LICENSE
--rw-r--r--   0        0        0     2813 2023-05-07 16:32:54.439874 arclet-alconna-1.7.0rc7/pyproject.toml
--rw-r--r--   0        0        0     6702 2023-05-08 08:04:29.409891 arclet-alconna-1.7.0rc7/README-EN.md
--rw-r--r--   0        0        0     1087 2023-05-09 04:08:23.241662 arclet-alconna-1.7.0rc7/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 16:29:22.798529 arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/__init__.py
--rw-r--r--   0        0        0    18068 2023-05-09 02:30:18.661298 arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_analyser.py
--rw-r--r--   0        0        0     8454 2023-05-09 02:55:46.376874 arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_argv.py
--rw-r--r--   0        0        0    23058 2023-05-09 03:22:21.186877 arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_handlers.py
--rw-r--r--   0        0        0     7811 2023-05-08 06:38:21.959747 arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_header.py
--rw-r--r--   0        0        0      837 2023-05-07 16:29:22.801529 arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_util.py
--rw-r--r--   0        0        0     1785 2023-05-08 05:11:19.754526 arclet-alconna-1.7.0rc7/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    14478 2023-05-08 06:44:47.137906 arclet-alconna-1.7.0rc7/src/arclet/alconna/args.py
--rw-r--r--   0        0        0     1435 2023-05-08 17:20:30.396974 arclet-alconna-1.7.0rc7/src/arclet/alconna/argv.py
--rw-r--r--   0        0        0    15913 2023-05-07 16:32:41.201286 arclet-alconna-1.7.0rc7/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0    12902 2023-05-08 05:22:02.753182 arclet-alconna-1.7.0rc7/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     1889 2023-05-08 06:44:58.844442 arclet-alconna-1.7.0rc7/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     4872 2023-05-09 02:30:18.674447 arclet-alconna-1.7.0rc7/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     4463 2023-05-08 15:45:12.657524 arclet-alconna-1.7.0rc7/src/arclet/alconna/config.py
--rw-r--r--   0        0        0    14858 2023-05-08 12:05:48.939938 arclet-alconna-1.7.0rc7/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     2615 2023-05-07 16:32:47.490076 arclet-alconna-1.7.0rc7/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1070 2023-05-07 16:32:49.003053 arclet-alconna-1.7.0rc7/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0    11252 2023-05-08 16:28:22.675096 arclet-alconna-1.7.0rc7/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0       99 2023-05-07 16:29:22.812601 arclet-alconna-1.7.0rc7/src/arclet/alconna/i18n/.config.json
--rw-r--r--   0        0        0     3565 2023-05-07 16:29:22.813522 arclet-alconna-1.7.0rc7/src/arclet/alconna/i18n/en-US.json
--rw-r--r--   0        0        0     3602 2023-05-07 16:29:22.813850 arclet-alconna-1.7.0rc7/src/arclet/alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0    16956 2023-05-08 17:23:28.473144 arclet-alconna-1.7.0rc7/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1430 2023-05-07 16:32:50.831111 arclet-alconna-1.7.0rc7/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1943 2023-05-07 16:32:51.478127 arclet-alconna-1.7.0rc7/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     3940 2023-05-07 16:32:52.687122 arclet-alconna-1.7.0rc7/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2023-05-07 16:29:22.816522 arclet-alconna-1.7.0rc7/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     5813 2023-05-07 16:32:58.355410 arclet-alconna-1.7.0rc7/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     3584 2023-05-07 16:32:58.778521 arclet-alconna-1.7.0rc7/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0     3254 2023-05-08 06:48:40.755418 arclet-alconna-1.7.0rc7/tests/analyser_test.py
--rw-r--r--   0        0        0     7223 2023-05-07 16:29:22.820523 arclet-alconna-1.7.0rc7/tests/args_test.py
--rw-r--r--   0        0        0     2167 2023-05-07 16:32:42.508980 arclet-alconna-1.7.0rc7/tests/base_test.py
--rw-r--r--   0        0        0     3113 2023-05-08 06:49:11.411375 arclet-alconna-1.7.0rc7/tests/components_test.py
--rw-r--r--   0        0        0     1199 2023-05-07 16:29:22.822522 arclet-alconna-1.7.0rc7/tests/config_test.py
--rw-r--r--   0        0        0    23219 2023-05-09 02:35:51.817251 arclet-alconna-1.7.0rc7/tests/core_test.py
--rw-r--r--   0        0        0      505 2023-05-07 16:29:22.823526 arclet-alconna-1.7.0rc7/tests/util_test.py
--rw-r--r--   0        0        0     7366 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc7/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.1/LICENSE
+-rw-r--r--   0        0        0     2810 2023-05-11 05:55:21.918053 arclet-alconna-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6702 2023-05-11 05:55:23.383958 arclet-alconna-1.7.1/README-EN.md
+-rw-r--r--   0        0        0     1084 2023-05-12 08:33:12.923713 arclet-alconna-1.7.1/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:53:44.746150 arclet-alconna-1.7.1/src/arclet/alconna/_internal/__init__.py
+-rw-r--r--   0        0        0    17787 2023-05-12 08:33:12.924712 arclet-alconna-1.7.1/src/arclet/alconna/_internal/_analyser.py
+-rw-r--r--   0        0        0     8476 2023-05-11 05:53:44.748144 arclet-alconna-1.7.1/src/arclet/alconna/_internal/_argv.py
+-rw-r--r--   0        0        0    23045 2023-05-11 05:53:44.748144 arclet-alconna-1.7.1/src/arclet/alconna/_internal/_handlers.py
+-rw-r--r--   0        0        0     7811 2023-05-11 05:53:44.749146 arclet-alconna-1.7.1/src/arclet/alconna/_internal/_header.py
+-rw-r--r--   0        0        0      837 2023-05-11 05:53:44.749146 arclet-alconna-1.7.1/src/arclet/alconna/_internal/_util.py
+-rw-r--r--   0        0        0     1543 2023-05-11 05:54:34.441719 arclet-alconna-1.7.1/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    14429 2023-05-11 05:55:00.317381 arclet-alconna-1.7.1/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     1499 2023-05-11 05:53:44.752371 arclet-alconna-1.7.1/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    15660 2023-05-11 05:55:01.638197 arclet-alconna-1.7.1/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0    13248 2023-05-11 05:55:02.886909 arclet-alconna-1.7.1/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     1889 2023-05-11 05:55:04.954858 arclet-alconna-1.7.1/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     4867 2023-05-11 05:53:44.757144 arclet-alconna-1.7.1/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     4465 2023-05-11 05:55:07.597153 arclet-alconna-1.7.1/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    14139 2023-05-11 05:55:11.101320 arclet-alconna-1.7.1/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     2617 2023-05-11 05:55:14.716787 arclet-alconna-1.7.1/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1009 2023-05-11 05:55:16.833416 arclet-alconna-1.7.1/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0    11287 2023-05-11 05:55:17.442184 arclet-alconna-1.7.1/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0       99 2023-05-11 05:53:44.763145 arclet-alconna-1.7.1/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3565 2023-05-11 05:53:44.764143 arclet-alconna-1.7.1/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3602 2023-05-11 05:53:44.764143 arclet-alconna-1.7.1/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    16956 2023-05-11 05:55:18.044404 arclet-alconna-1.7.1/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1484 2023-05-11 05:55:18.667097 arclet-alconna-1.7.1/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1943 2023-05-11 05:55:19.651541 arclet-alconna-1.7.1/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     3940 2023-05-11 05:55:20.308191 arclet-alconna-1.7.1/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:53:44.769149 arclet-alconna-1.7.1/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     5815 2023-05-11 05:55:25.933152 arclet-alconna-1.7.1/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     3586 2023-05-11 05:55:26.563876 arclet-alconna-1.7.1/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0     3246 2023-05-11 05:53:44.772143 arclet-alconna-1.7.1/tests/analyser_test.py
+-rw-r--r--   0        0        0     7583 2023-05-11 05:53:44.773143 arclet-alconna-1.7.1/tests/args_test.py
+-rw-r--r--   0        0        0     2167 2023-05-11 05:55:03.459296 arclet-alconna-1.7.1/tests/base_test.py
+-rw-r--r--   0        0        0     3113 2023-05-11 05:53:44.774144 arclet-alconna-1.7.1/tests/components_test.py
+-rw-r--r--   0        0        0     1199 2023-05-11 05:53:44.774144 arclet-alconna-1.7.1/tests/config_test.py
+-rw-r--r--   0        0        0    23493 2023-05-12 08:33:12.926710 arclet-alconna-1.7.1/tests/core_test.py
+-rw-r--r--   0        0        0      505 2023-05-11 05:53:44.775105 arclet-alconna-1.7.1/tests/util_test.py
+-rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 arclet-alconna-1.7.1/PKG-INFO
```

### Comparing `arclet-alconna-1.7.0rc7/LICENSE` & `arclet-alconna-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc7/pyproject.toml` & `arclet-alconna-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-version = "1.7.0rc7"
+version = "1.7.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
```

### Comparing `arclet-alconna-1.7.0rc7/README-EN.md` & `arclet-alconna-1.7.1/README-EN.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/__init__.py` & `arclet-alconna-1.7.1/src/arclet/alconna/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 from .builtin import set_default
 from .model import OptionResult, SubcommandResult, HeadResult
 from .output import output_manager
 from .formatter import TextFormatter
 from .duplication import Duplication
 from .stub import ArgsStub, OptionStub, SubcommandStub
 
-__version__ = "1.7.0rc7"
+__version__ = "1.7.1"
 
 # backward compatibility
 Arpamar = Arparma
 DataCollectionContainer = Argv
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_analyser.py` & `arclet-alconna-1.7.1/src/arclet/alconna/_internal/_analyser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 from __future__ import annotations
 
 import re
 import traceback
-from re import Match
-from typing import TYPE_CHECKING, Any, Generic, Callable, Set
 from dataclasses import dataclass, field
-from typing_extensions import Self, TypeAlias
+from re import Match
+from typing import TYPE_CHECKING, Any, Callable, Generic, Set
+
 from tarina import lang
+from typing_extensions import Self, TypeAlias
 
-from ..manager import command_manager, ShortcutArgs
-from ..exceptions import (
-    ParamsUnmatched,
-    ArgumentMissing,
-    FuzzyMatchSuccess,
-    PauseTriggered,
-    SpecialOptionTriggered,
-    TerminateLoop
-)
 from ..action import Action
 from ..args import Args
+from ..arparma import Arparma
 from ..base import Option, Subcommand
 from ..completion import comp_ctx
-from ..model import Sentence, HeadResult, OptionResult, SubcommandResult
-from ..arparma import Arparma
-from ..typing import TDC
 from ..config import Namespace, config
+from ..exceptions import (
+    ArgumentMissing, FuzzyMatchSuccess, ParamsUnmatched, PauseTriggered, SpecialOptionTriggered
+)
+from ..manager import ShortcutArgs, command_manager
+from ..model import HeadResult, OptionResult, Sentence, SubcommandResult
 from ..output import output_manager
-from ._util import levenshtein
+from ..typing import TDC
 from ._handlers import (
-    analyse_args, analyse_param, analyse_header, handle_opt_default,
-    handle_help, handle_shortcut, handle_completion, prompt
+    analyse_args, analyse_header, analyse_param,
+    handle_completion, handle_help, handle_opt_default,
+    handle_shortcut, prompt
 )
 from ._header import Header
-
+from ._util import levenshtein
 
 if TYPE_CHECKING:
-    from ._argv import Argv
     from ..core import Alconna
+    from ._argv import Argv
 
 _SPECIAL = {
     "help": handle_help,
     "shortcut": handle_shortcut,
     "completion": handle_completion
 }
 
@@ -208,19 +204,16 @@
 
         Returns:
             Self: 自身
 
         Raises:
             ArgumentMissing: 参数缺失
         """
-        while True:
-            try:
-                analyse_param(self, argv, self.command.separators)
-            except TerminateLoop:
-                break
+        while analyse_param(self, argv, self.command.separators):
+            pass
         if self.default_main_only and not self.args_result:
             self.args_result = analyse_args(argv, self.self_args)
         if not self.args_result and self.need_main_args:
             raise ArgumentMissing(lang.require("subcommand", "args_missing").format(name=self.command.dest))
         return self
 
     def get_sub_analyser(self, target: Subcommand) -> SubAnalyser[TDC] | None:
@@ -398,39 +391,35 @@
         if isinstance(exc, ArgumentMissing) and comp_ctx.get(None):
             raise PauseTriggered(prompt(self, argv))
         if self.command.meta.raise_exception:
             raise exc
         return self.export(argv, True, exc)
 
     def analyse(self, argv: Argv[TDC]) -> Arparma[TDC] | None:
-        while True:
-            try:
-                analyse_param(self, argv)
-            except TerminateLoop:
-                break
-            except FuzzyMatchSuccess as e:
-                output_manager.send(self.command.name, lambda: str(e))
-                return self.export(argv, True)
-            except SpecialOptionTriggered as sot:
-                return _SPECIAL[sot.args[0]](self, argv)
-            except (ParamsUnmatched, ArgumentMissing) as e1:
-                if (rest := argv.release()) and isinstance(rest[-1], str):
-                    if rest[-1] in argv.completion_names:
-                        last = argv.bak_data[-1]
-                        argv.bak_data[-1] = last[:last.rfind(rest[-1])]
-                        return handle_completion(self, argv)
-                    if handler := argv.special.get(rest[-1]):
-                        return _SPECIAL[handler](self, argv)
-                if isinstance(e1, ArgumentMissing) and comp_ctx.get(None):
-                    raise PauseTriggered(prompt(self, argv)) from e1
-                if self.command.meta.raise_exception:
-                    raise
-                return self.export(argv, True, e1)
-            if argv.current_index == argv.ndata:
-                break
+        try:
+            while analyse_param(self, argv) and argv.current_index != argv.ndata:
+                pass
+        except FuzzyMatchSuccess as e:
+            output_manager.send(self.command.name, lambda: str(e))
+            return self.export(argv, True)
+        except SpecialOptionTriggered as sot:
+            return _SPECIAL[sot.args[0]](self, argv)
+        except (ParamsUnmatched, ArgumentMissing) as e1:
+            if (rest := argv.release()) and isinstance(rest[-1], str):
+                if rest[-1] in argv.completion_names:
+                    last = argv.bak_data[-1]
+                    argv.bak_data[-1] = last[:last.rfind(rest[-1])]
+                    return handle_completion(self, argv)
+                if handler := argv.special.get(rest[-1]):
+                    return _SPECIAL[handler](self, argv)
+            if isinstance(e1, ArgumentMissing) and comp_ctx.get(None):
+                raise PauseTriggered(prompt(self, argv)) from e1
+            if self.command.meta.raise_exception:
+                raise
+            return self.export(argv, True, e1)
 
         if self.default_main_only and not self.args_result:
             self.args_result = analyse_args(argv, self.self_args)
 
     def export(
         self,
         argv: Argv[TDC],
@@ -442,15 +431,15 @@
         Args:
             argv (Argv[TDC]): 命令行参数
             fail (bool, optional): 是否解析失败. Defaults to False.
             exception (BaseException | None, optional): 解析失败时的异常. Defaults to None.
         """
         result = Arparma(self.command.path, argv.origin, not fail, self.header_result)
         if fail:
-            result.error_info = repr(exception or traceback.format_exc(limit=1))
+            result.error_info = exception or repr(traceback.format_exc(limit=1))
             result.error_data = argv.release()
         else:
             if self.default_opt_result:
                 handle_opt_default(self.default_opt_result, self.options_result)
             if self.default_sub_result:
                 for k, v in self.default_sub_result.items():
                     if k not in self.subcommands_result:
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_argv.py` & `arclet-alconna-1.7.1/src/arclet/alconna/_internal/_argv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field, InitVar
-from typing import Any, Callable, Generic, ClassVar, Iterable
+from dataclasses import InitVar, dataclass, field
+from typing import Any, Callable, ClassVar, Generic, Iterable
+
+from tarina import lang, split, split_once
 from typing_extensions import Self
-from tarina import split, split_once, lang
 
 from ..args import Arg
-from ..config import Namespace, config
 from ..base import Option, Subcommand
+from ..config import Namespace, config
 from ..exceptions import NullMessage
 from ..typing import TDC
 
 
-
 @dataclass(repr=True)
 class Argv(Generic[TDC]):
     """命令行参数"""
     namespace: InitVar[Namespace] = field(default=config.default_namespace)
     fuzzy_match: bool = field(default=False)
     """当前命令是否模糊匹配"""
-    preprocessors: dict[str, Callable[..., Any]] = field(default_factory=dict)
+    preprocessors: dict[type, Callable[..., Any]] = field(default_factory=dict)
     """命令元素的预处理器"""
     to_text: Callable[[Any], str | None] = field(default=lambda x: x if isinstance(x, str) else None)
     """将命令元素转换为文本, 或者返回None以跳过该元素"""
     separators: tuple[str, ...] = field(default=(' ',))
     """命令分隔符"""
-    filter_out: list[str] = field(default_factory=list)
+    filter_out: list[type] = field(default_factory=list)
     """需要过滤掉的命令元素"""
     checker: Callable[[Any], bool] | None = field(default=None)
     """检查传入命令"""
     converter: Callable[[str | list], TDC] = field(default=lambda x: x)
     """将字符串或列表转为目标命令类型"""
     filter_crlf: bool = field(default=True)
     """是否过滤掉换行符"""
@@ -62,19 +62,19 @@
         self.special.update(
             [(i, "help") for i in namespace.builtin_option_name['help']] +
             [(i, "completion") for i in namespace.builtin_option_name['completion']] +
             [(i, "shortcut") for i in namespace.builtin_option_name['shortcut']]
         )
         self.completion_names = namespace.builtin_option_name['completion']
         if __cache := self.__class__._cache.get(self.__class__, {}):
-            self.preprocessors.update(__cache["preprocessors"] or {})
-            self.filter_out.extend(__cache["filter_out"] or [])
-            self.to_text = __cache["to_text"] or self.to_text
-            self.checker = __cache["checker"] or self.checker
-            self.converter = __cache["converter"] or self.converter
+            self.preprocessors.update(__cache.get("preprocessors") or {})
+            self.filter_out.extend(__cache.get("filter_out") or [])
+            self.to_text = __cache.get("to_text") or self.to_text
+            self.checker = __cache.get("checker") or self.checker
+            self.converter = __cache.get("converter") or self.converter
 
     def reset(self):
         """重置命令行参数"""
         self.current_index = 0
         self.ndata = 0
         self.bak_data = []
         self.raw_data = []
@@ -104,19 +104,20 @@
         """
         self.reset()
         if self.checker and not self.checker(data):
             raise TypeError(data)
         self.origin = data
         if data.__class__ is str:
             data = [data]  # type: ignore
-        i, raw_data = 0, self.raw_data
+        i = 0
+        raw_data = self.raw_data
         for unit in data:
-            if (uname := unit.__class__.__name__) in self.filter_out:
+            if (utype := unit.__class__) in self.filter_out:
                 continue
-            if (proc := self.preprocessors.get(uname)) and (res := proc(unit)):
+            if (proc := self.preprocessors.get(utype)) and (res := proc(unit)):
                 unit = res
             if (text := self.to_text(unit)) is None:
                 raw_data.append(unit)
             elif not (res := text.strip()):
                 continue
             else:
                 raw_data.append(res)
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_handlers.py` & `arclet-alconna-1.7.1/src/arclet/alconna/_internal/_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING, Any, Iterable
-from tarina import Empty, lang
-from nepattern import AllParam, BasePattern, AnyOne, AnyString
+
+from nepattern import AllParam, AnyOne, AnyString, BasePattern
 from nepattern.util import TPattern
+from tarina import Empty, lang
 
-from ._header import Double, Header
 from ..action import Action
-from ..args import Arg, Args, STRING
+from ..args import STRING, Arg, Args
 from ..base import Option, Subcommand
-from ..config import config
 from ..completion import Prompt, comp_ctx
+from ..config import config
 from ..exceptions import (
-    ArgumentMissing, FuzzyMatchSuccess, ParamsUnmatched, SpecialOptionTriggered, PauseTriggered, TerminateLoop
+    ArgumentMissing, FuzzyMatchSuccess, ParamsUnmatched, PauseTriggered, SpecialOptionTriggered
 )
-from ..model import OptionResult, Sentence, HeadResult
+from ..model import HeadResult, OptionResult, Sentence
 from ..output import output_manager
 from ..typing import KeyWordVar, MultiVar
+from ._header import Double, Header
 from ._util import levenshtein
 
 if TYPE_CHECKING:
+    from ._analyser import Analyser, SubAnalyser
     from ._argv import Argv
-    from ._analyser import SubAnalyser, Analyser
 
 
 def _handle_keyword(
     argv: Argv,
     value: KeyWordVar,
     may_arg: Any,
     seps: tuple[str, ...],
@@ -103,18 +104,17 @@
 
 def _loop(
     argv: Argv,
     _loop: int,
     seps: tuple[str, ...],
     value: MultiVar,
     default: Any,
-    args: Args
+    kw: KeyWordVar | None
 ):
     """循环参数"""
-    kw = args[args.var_keyword].value.base if args.var_keyword else None
     result = []
     for _ in range(_loop):
         _m_arg, _m_str = argv.next(seps)
         if not _m_arg:
             continue
         if _m_str and (
             _m_arg in argv.param_ids or
@@ -144,31 +144,31 @@
     Args:
         argv (Argv): 命令行参数
         args (Args): 参数集合
         arg (Arg): 参数单元
         result_dict (dict[str, Any]): 结果字典
     """
     seps = arg.separators
-    value = arg.value
+    value: MultiVar = arg.value  # type: ignore
     key = arg.name
     default = arg.field.default
     kw = value.base.__class__ == KeyWordVar
-    _m_rest_arg = len(args) - len(result_dict)
-    _m_rest_all_param_count = len(argv.release(seps))
+    _rest = len(args) - len(result_dict)
+    _all_count = len(argv.release(seps))
     if not kw and not args.var_keyword or kw and not args.var_positional:
-        loop = _m_rest_all_param_count - _m_rest_arg + 1
+        loop = _all_count - _rest + 1
     elif not kw:
-        loop = _m_rest_all_param_count - (_m_rest_arg - 2*(args[args.var_keyword].value.flag == "*"))
+        loop = _all_count - (_rest - 2*(args.var_keyword.flag == "*"))
     else:
-        loop = _m_rest_all_param_count - (_m_rest_arg - 2*(args[args.var_positional].value.flag == "*"))
+        loop = _all_count - (_rest - 2*(args.var_positional.flag == "*"))
     if value.length > 0:
         loop = min(loop, value.length)
     result_dict[key] = (
         _loop_kw(argv, loop, seps, value, default) if kw
-        else _loop(argv, loop, seps, value, default, args)
+        else _loop(argv, loop, seps, value, default, value.base if kw else None)
     )
     if kw:
         kwargs = result_dict[key]
         if not isinstance(kwargs, dict):
             kwargs = {key: kwargs}
         result_dict[key] = kwargs
     else:
@@ -200,15 +200,15 @@
         may_arg, _str = argv.next(arg.separators)
         if _str and may_arg in argv.completion_names:
             raise SpecialOptionTriggered("completion")
         if not may_arg or (_str and may_arg in argv.param_ids):
             argv.rollback(may_arg)
             if default_val is not None:
                 result[key] = None if default_val is Empty else default_val
-            elif value.__class__ is MultiVar and value.flag == '*':
+            elif value.__class__ is MultiVar and value.flag == '*':  # type: ignore
                 result[key] = ()
             elif not arg.optional:
                 raise ArgumentMissing(lang.require("args", "missing").format(key=key))
             continue
         if value.__class__ is MultiVar:
             argv.rollback(may_arg)
             multi_arg_handler(argv, args, arg, result)  # type: ignore
@@ -386,25 +386,25 @@
         _param = None
     elif _text in analyser.compile_params:
         _param = analyser.compile_params[_text]
     elif analyser.compact_params and (res := analyse_compact_params(analyser, argv)):
         if res.__class__ is str:
             raise ParamsUnmatched(res)
         argv.context = None
-        return
+        return True
     else:
         _param = None
     if not _param and analyser.command.nargs and not analyser.args_result:
         analyser.args_result = analyse_args(argv, analyser.self_args)
         if analyser.args_result:
             argv.context = None
-            return
+            return True
     if _param.__class__ is Sentence:
         analyser.sentences.append(argv.next()[0])
-        return
+        return True
     if _param.__class__ is Option:
         if _param.requires and analyser.sentences != _param.requires:
             raise ParamsUnmatched(
                 lang.require("option", "require_error").format(source=_param.name, target=' '.join(analyser.sentences))
             )
         analyse_option(analyser, argv, _param)
     elif _param.__class__ is list:
@@ -434,17 +434,18 @@
                 )
             )
         try:
             _param.process(argv)
         finally:
             analyser.subcommands_result[_param.command.dest] = _param.result()
     else:
-        raise TerminateLoop(str(_text))
+        return False
     analyser.sentences.clear()
     argv.context = None
+    return True
 
 
 def analyse_header(header: Header, argv: Argv) -> HeadResult:
     """分析头部
 
     Args:
         header (Header): 头部
@@ -502,15 +503,15 @@
 def handle_help(analyser: Analyser, argv: Argv):
     """处理帮助选项触发"""
     _help_param = [str(i) for i in argv.release(recover=True) if str(i) not in argv.special]
     output_manager.send(
         analyser.command.name,
         lambda: analyser.command.formatter.format_node(_help_param),
     )
-    return analyser.export(argv, True)
+    return analyser.export(argv, True, SpecialOptionTriggered('help'))
 
 
 _args = Args["delete;?", "delete"]["name", str]["command", str, "_"]
 
 
 def handle_shortcut(analyser: Analyser, argv: Argv):
     """处理快捷命令触发"""
@@ -524,15 +525,15 @@
             opt_v["name"],
             None if opt_v["command"] == "_" else {"command": argv.converter(opt_v["command"])},
             bool(opt_v.get("delete"))
         )
         output_manager.send(analyser.command.name, lambda: msg)
     except Exception as e:
         output_manager.send(analyser.command.name, lambda: str(e))
-    return analyser.export(argv, True)
+    return analyser.export(argv, True, SpecialOptionTriggered('shortcut'))
 
 
 def _prompt_unit(analyser: Analyser, argv: Argv, trig: Arg):
     if trig.field.completion:
         comp = trig.field.completion()
         if isinstance(comp, str):
             return [Prompt(comp, False)]
@@ -603,8 +604,8 @@
     if res := prompt(analyser, argv, trigger):
         if comp_ctx.get(None):
             raise PauseTriggered(res)
         output_manager.send(
             analyser.command.name,
             lambda: f"{lang.require('completion', 'node')}\n* " + "\n* ".join([i.text for i in res]),
         )
-    return analyser.export(argv, True, 'NoneType: None\n')  # type: ignore
+    return analyser.export(argv, True, SpecialOptionTriggered('completion'))  # type: ignore
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_header.py` & `arclet-alconna-1.7.1/src/arclet/alconna/_internal/_header.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_util.py` & `arclet-alconna-1.7.1/src/arclet/alconna/_internal/_util.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/args.py` & `arclet-alconna-1.7.1/src/arclet/alconna/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 import sys
 from copy import deepcopy
 from enum import Enum
 from functools import partial
 from typing import Any, Callable, Generic, Iterable, Sequence, TypeVar, Union
 
-from nepattern import AllParam, AnyOne, BasePattern, UnionPattern, all_patterns, type_parser
+from nepattern import AllParam, AnyOne, BasePattern, RawStr, UnionPattern, all_patterns, type_parser
 from tarina import Empty, get_signature, lang
 from typing_extensions import Self
 
 from .exceptions import InvalidParam
 from .typing import KeyWordVar, MultiVar
 
 
@@ -54,15 +54,15 @@
 
 @dc.dataclass(**safe_dcls_kw(init=False, eq=True, unsafe_hash=True, slots=True))
 class Arg:
     """参数单元"""
 
     name: str = dc.field(compare=True, hash=True)
     """参数单元的名称"""
-    value: Union[BasePattern, AllParam.__class__] = dc.field(compare=False, hash=True)
+    value: BasePattern = dc.field(compare=False, hash=True)
     """参数单元的值"""
     field: Field[Any] = dc.field(compare=False, hash=False)
     """参数单元的字段"""
     notice: str | None = dc.field(compare=False, hash=False)
     """参数单元的注释"""
     flag: set[ArgFlag] = dc.field(compare=False, hash=False)
     """参数单元的标识"""
@@ -92,33 +92,33 @@
             flags (list[ArgFlag], optional): 参数单元的标识. Defaults to None.
         """
         if not isinstance(name, str) or name.startswith('$'):
             raise InvalidParam(lang.require("args", "name_error"))
         if not name.strip():
             raise InvalidParam(lang.require("args", "name_empty"))
         self.name = name
-        _value = type_parser(value or name)
+        _value = type_parser(value or RawStr(name))
         default = field if isinstance(field, Field) else Field(field)
         if isinstance(_value, UnionPattern) and _value.optional:
             default.default = Empty if default.default is None else default.default
         if default.default == "...":
             default.default = Empty
         if _value is Empty:
             raise InvalidParam(lang.require("args", "value_error").format(target=name))
         self.value = _value
         self.field = default
         self.notice = notice
         self.separators = (seps,) if isinstance(seps, str) else tuple(seps)
         flags = flags or []
-        if res := re.match(r"^.+?#(?P<notice>[^;?!/#]+)", name):
+        if res := re.match(r"^(?P<name>.+?)#(?P<notice>[^;?!/#]+)", name):
             self.notice = res["notice"]
-            self.name = name.replace(f"#{res['notice']}", "")
-        if res := re.match(r"^.+?;(?P<flag>[?!/]+)", self.name):
+            self.name = res["name"]
+        if res := re.match(r"^(?P<name>.+?)(;)?(?P<flag>[?!/]+)", self.name):
             flags.extend(ArgFlag(c) for c in res["flag"])
-            self.name = self.name.replace(f";{res['flag']}", "")
+            self.name = res["name"]
         self.flag = set(flags)
         self.optional = ArgFlag.OPTIONAL in self.flag
         self.hidden = ArgFlag.HIDDEN in self.flag
         self.anonymous = self.name.startswith("_key_")
         if ArgFlag.ANTI in self.flag and self.value not in (AnyOne, AllParam):
             self.value = deepcopy(self.value).reverse()
 
@@ -162,18 +162,18 @@
     也可以使用特殊方法 `__getattr__` 来构造参数集合, 例如:
 
         >>> Args.name[str]
         Args('name': str)
     """
     argument: list[Arg]
     """参数单元组"""
-    var_positional: str | None
-    """可变参数的名称"""
-    var_keyword: str | None
-    """可变关键字参数的名称"""
+    var_positional: MultiVar | None
+    """可变参数"""
+    var_keyword: MultiVar | None
+    """可变关键字参数"""
     keyword_only: list[str]
     """仅关键字参数的名称"""
     optional_count: int
     """可选参数的数量"""
 
     @classmethod
     def from_callable(cls, target: Callable) -> tuple[Args, bool]:
@@ -300,19 +300,19 @@
                 continue
             self._visit.add(arg.name)
             _limit = False
             if isinstance(arg.value, MultiVar) and not _limit:
                 if isinstance(arg.value.base, KeyWordVar):
                     if self.var_keyword:
                         raise InvalidParam(lang.require("args", "duplicate_kwargs"))
-                    self.var_keyword = arg.name
+                    self.var_keyword = arg.value
                 elif self.var_positional:
                     raise InvalidParam(lang.require("args", "duplicate_varargs"))
                 else:
-                    self.var_positional = arg.name
+                    self.var_positional = arg.value
                 _limit = True
             if isinstance(arg.value, KeyWordVar):
                 if self.var_keyword or self.var_positional:
                     raise InvalidParam(lang.require("args", "exclude_mutable_args"))
                 self.keyword_only.append(arg.name)
                 if arg.value.sep in arg.separators:
                     _tmp.insert(-1, Arg(f"_key_{arg.name}", value=f"-*{arg.name}"))
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/argv.py` & `arclet-alconna-1.7.1/src/arclet/alconna/argv.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from __future__ import annotations
 
 from contextvars import ContextVar
 from typing import Any, Callable
 
-from .typing import TDC
 from ._internal._argv import Argv
+from .typing import TDC
 
 __argv_type__: ContextVar[type[Argv]] = ContextVar("argv_type", default=Argv)
 
 
 def set_default_argv_type(argv_type: type[Argv]):
     """设置默认的命令行参数类型"""
     __argv_type__.set(argv_type)
 
 
 def argv_config(
     target: type[Argv] | None = None,
-    preprocessors: dict[str, Callable[..., Any]] | None = None,
+    preprocessors: dict[type, Callable[..., Any]] | None = None,
     to_text: Callable[[Any], str | None] | None = None,
-    filter_out: list[str] | None = None,
+    filter_out: list[type] | None = None,
     checker: Callable[[Any], bool] | None = None,
     converter: Callable[[str | list], TDC] | None = None
 ):
     """配置命令行参数
 
     Args:
         target (type[Argv] | None, optional): 目标命令类型.
-        preprocessors (dict[str, Callable[..., Any]] | None, optional): 命令元素的预处理器.
+        preprocessors (dict[type, Callable[..., Any]] | None, optional): 命令元素的预处理器.
         to_text (Callable[[Any], str | None] | None, optional): 将命令元素转换为文本, 或者返回None以跳过该元素.
-        filter_out (list[str] | None, optional): 需要过滤掉的命令元素.
+        filter_out (list[type] | None, optional): 需要过滤掉的命令元素.
         checker (Callable[[Any], bool] | None, optional): 检查传入命令.
         converter (Callable[[str | list], TDC] | None, optional): 将字符串或列表转为目标命令类型.
     """
-    Argv._cache.setdefault(target or __argv_type__.get(), {}).update(locals())
+    Argv._cache.setdefault(
+        target or __argv_type__.get(), {}
+    ).update({k: v for k, v in locals().items() if v is not None})
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/arparma.py` & `arclet-alconna-1.7.1/src/arclet/alconna/arparma.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from abc import ABCMeta, abstractmethod
 from contextlib import suppress
 from dataclasses import dataclass, field
 from functools import lru_cache
 from types import MappingProxyType
 from typing import Any, Callable, Generic, Mapping, TypeVar, overload
-from tarina import get_signature, generic_isinstance, Empty, lang
+
+from tarina import Empty, generic_isinstance, get_signature, lang
 from typing_extensions import Self
 
 from .exceptions import BehaveCancelled, OutBoundsBehave
 from .model import HeadResult, OptionResult, SubcommandResult
 from .typing import TDC
 
 T = TypeVar('T')
@@ -186,27 +187,23 @@
         """执行行为器
 
         Args:
             behaviors (list[ArparmaBehavior] | None, optional): 要执行的行为器列表
         Returns:
             Self: 返回自身
         """
-        if behaviors := (self.source.behaviors + (behaviors or [])):
-            exc_behaviors = []
-            for behavior in behaviors:
-                exc_behaviors.extend(requirement_handler(behavior))
-            for b in exc_behaviors:
-                b.before_operate(self)
-            for b in exc_behaviors:
-                try:
-                    b.operate(self)
-                except BehaveCancelled:
-                    continue
-                except OutBoundsBehave as e:
-                    return self.fail(e)
+        for b in behaviors:
+            b.before_operate(self)
+        for b in behaviors:
+            try:
+                b.operate(self)
+            except BehaveCancelled:
+                continue
+            except OutBoundsBehave as e:
+                return self.fail(e)
         return self
 
     def call(self, target: Callable[..., T], **additional) -> T:
         """依据 `Arparma` 中的数据调用函数
 
         Args:
             target (Callable[..., T]): 要调用的函数
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/base.py` & `arclet-alconna-1.7.1/src/arclet/alconna/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 """Alconna 的基础内容相关"""
 from __future__ import annotations
 
 from functools import reduce
-from typing import Iterable, Sequence, overload, Any
-from typing_extensions import Self
+from dataclasses import replace
+from typing import Any, Iterable, Sequence, overload
+
 from tarina import lang
+from typing_extensions import Self
 
 from .action import Action, store
 from .args import Arg, Args
 from .exceptions import InvalidParam
 from .model import OptionResult, SubcommandResult
 
 
 def _handle_default(node: CommandNode):
     if node.default is None:
         return
     act = node.action
+    if act.type == 1 and not isinstance(act.value, list):
+        act = node.action = replace(act, value=[act.value])
+    elif act.type == 2 and not isinstance(act.value, int):
+        act = node.action = replace(act, value=1)
     if isinstance(node.default, (OptionResult, SubcommandResult)):
         if act.type == 0 and act.value is ...:
-            act.value = node.default.value
+            node.action = Action(act.type, node.default.value)
         if act.type == 1:
             if not isinstance(node.default.value, list):
                 node.default.value = [node.default.value]
             if act.value[0] is ...:
-                act.value = node.default.value[:]
+                node.action = Action(act.type, node.default.value[:])
         if act.type == 2 and not isinstance(node.default.value, int):
             node.default.value = 1
     else:
         if act.type == 0 and act.value is ...:
-            act.value = node.default
+            node.action = Action(act.type, node.default)
         if act.type == 1:
             if not isinstance(node.default, list):
                 node.default = [node.default]
             if act.value[0] is ...:
-                act.value = node.default[:]
+                node.action = Action(act.type, node.default[:])
         if act.type == 2 and not isinstance(node.default, int):
             node.default = 1
 
 
 class CommandNode:
     """命令节点基类, 规定基础组件所含属性"""
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/builtin.py` & `arclet-alconna-1.7.1/src/arclet/alconna/builtin.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/completion.py` & `arclet-alconna-1.7.1/src/arclet/alconna/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Any, TYPE_CHECKING
+from typing import TYPE_CHECKING
+
 from tarina import ContextModel, lang
 
 from .exceptions import PauseTriggered
 from .manager import command_manager
 from .output import output_manager
 
-
 if TYPE_CHECKING:
     from .core import Alconna
 
 
 @dataclass(eq=True, frozen=True, unsafe_hash=True)
 class Prompt:
     text: str = field(hash=True)
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/config.py` & `arclet-alconna-1.7.1/src/arclet/alconna/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import ContextManager, TypedDict, Callable, Any, TYPE_CHECKING
-from tarina import lang
 from pathlib import Path
+from typing import TYPE_CHECKING, Any, Callable, ContextManager, TypedDict
+
+from tarina import lang
 
-from .typing import TPrefixes, DataCollection
+from .typing import DataCollection, TPrefixes
 
 if TYPE_CHECKING:
     from .formatter import TextFormatter
 
 
 class OptionNames(TypedDict):
     help: set[str]
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/core.py` & `arclet-alconna-1.7.1/src/arclet/alconna/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,54 @@
 """Alconna 主体"""
 from __future__ import annotations
 
 import sys
 from dataclasses import dataclass, field
-from functools import partial, reduce
+from functools import partial
 from pathlib import Path
 from typing import Any, Callable, Generic, Sequence, TypeVar, overload
 
 from tarina import init_spec, lang
 from typing_extensions import Self
 
 from ._internal._analyser import Analyser, TCompile
 from .args import Arg, Args
-from .arparma import Arparma, ArparmaBehavior
+from .arparma import Arparma, ArparmaBehavior, requirement_handler
 from .base import Option, Subcommand
 from .config import Namespace, config
 from .duplication import Duplication
 from .exceptions import ExecuteFailed, NullMessage
 from .formatter import TextFormatter
 from .manager import ShortcutArgs, command_manager
-from .typing import TDC, TPrefixes, DataCollection, CommandMeta
+from .typing import TDC, CommandMeta, DataCollection, TPrefixes
 
 T_Duplication = TypeVar('T_Duplication', bound=Duplication)
 T = TypeVar("T")
 TDC1 = TypeVar("TDC1", bound=DataCollection[Any])
 
 
+def add_builtin_options(options: list[Option | Subcommand], ns: Namespace) -> None:
+    options.append(
+        Option("|".join(ns.builtin_option_name['help']), help_text=lang.require("builtin", "option_help")),
+    )
+    options.append(
+        Option(
+            "|".join(ns.builtin_option_name['shortcut']),
+            Args["delete;?", "delete"]["name", str]["command", str, "_"],
+            help_text=lang.require("builtin", "option_shortcut")
+        )
+    )
+    options.append(
+        Option(
+            "|".join(ns.builtin_option_name['completion']),
+            help_text=lang.require("builtin", "option_completion")
+        )
+    )
+
+
 @dataclass(init=True, unsafe_hash=True)
 class ArparmaExecutor(Generic[T]):
     """Arparma 执行器
 
     Attributes:
         target(Callable[..., T]): 目标函数
     """
@@ -109,19 +128,19 @@
             namespace (str | Namespace | None, optional): 命令命名空间, 默认为 'Alconna'
             separators (str | set[str] | Sequence[str] | None, optional): 命令参数分隔符, 默认为 `' '`
             behaviors (list[ArparmaBehavior] | None, optional): 命令解析行为器
             formatter_type (type[TextFormatter] | None, optional): 指定的命令帮助文本格式器类型
         """
         if not namespace:
             ns_config = config.default_namespace
-        elif isinstance(namespace, Namespace):
-            ns_config = config.namespaces.setdefault(namespace.name, namespace)
-        else:
+        elif isinstance(namespace, str):
             ns_config = config.namespaces.setdefault(namespace, Namespace(namespace))
-        self.prefixes = next(filter(lambda x: isinstance(x, list), args + (ns_config.prefixes.copy(),)))  # type: ignore
+        else:
+            ns_config = namespace
+        self.prefixes = next(filter(lambda x: isinstance(x, list), args), ns_config.prefixes.copy())  # type: ignore
         try:
             self.command = next(filter(lambda x: not isinstance(x, (list, Option, Subcommand, Args, Arg)), args))
         except StopIteration:
             if self.prefixes:
                 self.command = ""
             else:
                 path = Path(sys.argv[0])
@@ -131,41 +150,28 @@
         self.meta = meta or CommandMeta()
         if self.meta.example:
             self.meta.example = self.meta.example.replace("$", str(self.prefixes[0]) if self.prefixes else "")
         self.meta.fuzzy_match = self.meta.fuzzy_match or ns_config.fuzzy_match
         self.meta.raise_exception = self.meta.raise_exception or ns_config.raise_exception
         self.meta.compact = self.meta.compact or ns_config.compact
         options = [i for i in args if isinstance(i, (Option, Subcommand))]
-        options.append(
-            Option("|".join(ns_config.builtin_option_name['help']), help_text=lang.require("builtin", "option_help")),
-        )
-        options.append(
-            Option(
-                "|".join(ns_config.builtin_option_name['shortcut']),
-                Args["delete;?", "delete"]["name", str]["command", str, "_"],
-                help_text=lang.require("builtin", "option_shortcut")
-            )
-        )
-        options.append(
-            Option(
-                "|".join(ns_config.builtin_option_name['completion']),
-                help_text=lang.require("builtin", "option_completion")
-            )
-        )
-        name = f"{self.command or self.prefixes[0]}".replace(command_manager.sign, "")  # type: ignore
+        add_builtin_options(options, ns_config)
+        name = f"{self.command or self.prefixes[0]}"  # type: ignore
         self.path = f"{self.namespace}::{name}"
+        _args = Args()
+        for i in filter(lambda x: isinstance(x, (Args, Arg)), args):
+            _args << i
         super().__init__(
             "ALCONNA::",
-            reduce(lambda x, y: x + y, [Args()] + [i for i in args if isinstance(i, (Arg, Args))]),  # type: ignore
-            *options,
-            dest=name,
-            separators=separators or ns_config.separators,
+            _args, *options, dest=name, separators=separators or ns_config.separators,
         )
         self.name = name
-        self.behaviors = behaviors or []
+        self.behaviors = []
+        for behavior in behaviors or []:
+            self.behaviors.extend(requirement_handler(behavior))
         command_manager.register(self)
         self._executors: list[ArparmaExecutor] = []
         self.union = set()
 
     @property
     def namespace_config(self) -> Namespace:
         return config.namespaces[self.namespace]
@@ -180,41 +186,22 @@
         command_manager.delete(self)
         if isinstance(namespace, str):
             namespace = config.namespaces.setdefault(namespace, Namespace(namespace))
         self.namespace = namespace.name
         self.path = f"{self.namespace}::{self.name}"
         if header:
             self.prefixes = namespace.prefixes.copy()
-        self.options[-3] = Option(
-            "|".join(namespace.builtin_option_name['help']), help_text=lang.require("builtin", "option_help")
-        )
-        self.options[-2] = Option(
-            "|".join(namespace.builtin_option_name['shortcut']),
-            Args["delete;?", "delete"]["name", str]["command", str, "_"],
-            help_text=lang.require("builtin", "option_shortcut")
-        )
-        self.options[-1] = Option(
-            "|".join(namespace.builtin_option_name['completion']),
-            help_text=lang.require("builtin", "option_completion")
-        )
+        self.options = self.options[:-3]
+        add_builtin_options(self.options, namespace)
         self.meta.fuzzy_match = namespace.fuzzy_match or self.meta.fuzzy_match
         self.meta.raise_exception = namespace.raise_exception or self.meta.raise_exception
         self._hash = self._calc_hash()
         command_manager.register(self)
         return self
 
-    def reset_behaviors(self, behaviors: list[ArparmaBehavior]) -> Self:
-        """重新设置解析行为器
-
-        Args:
-            behaviors (list[ArparmaBehavior]): 解析行为器
-        """
-        self.behaviors[1:] = behaviors
-        return self
-
     def get_help(self) -> str:
         """返回该命令的帮助信息"""
         return self.formatter.format_node()
 
     def shortcut(self, key: str, args: ShortcutArgs[TDC] | None = None, delete: bool = False):
         """操作快捷命令
 
@@ -294,17 +281,15 @@
     def parse(self, message: TDC) -> Arparma[TDC]:
         ...
 
     @overload
     def parse(self, message, *, duplication: type[T_Duplication]) -> T_Duplication:
         ...
 
-    def parse(
-        self, message: TDC, *, duplication: type[T_Duplication] | None = None
-    ) -> Arparma[TDC] | T_Duplication:
+    def parse(self, message: TDC, *, duplication: type[T_Duplication] | None = None) -> Arparma[TDC] | T_Duplication:
         """命令分析功能, 传入字符串或消息链, 返回一个特定的数据集合类
         
         Args:
             message (TDC): 命令消息
             duplication (type[T_Duplication], optional): 指定的`副本`类型
         Returns:
             Arparma[TDC] | T_Duplication: 若`duplication`参数为`None`则返回`Arparma`对象, 否则返回`duplication`类型的对象
@@ -314,15 +299,15 @@
         try:
             arp = self._parse(message)
         except NullMessage as e:
             if self.meta.raise_exception:
                 raise e
             return Arparma(self.path, message, False, error_info=e)
         if arp.matched:
-            arp = arp.execute()
+            arp = arp.execute(self.behaviors)
             if self._executors:
                 for ext in self._executors:
                     arp.call(ext.target)
         return duplication(arp) if duplication else arp
 
     def bind(self, active: bool = True):
         """绑定命令执行器
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/duplication.py` & `arclet-alconna-1.7.1/src/arclet/alconna/duplication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from inspect import isclass
 from typing import cast
+
 from tarina import Empty
 
 from .arparma import Arparma
 from .stub import ArgsStub, BaseStub, OptionStub, SubcommandStub
 
 
 class Duplication:
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/exceptions.py` & `arclet-alconna-1.7.1/src/arclet/alconna/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,11 +43,7 @@
 
 class PauseTriggered(Exception):
     """解析状态保存触发"""
 
 
 class SpecialOptionTriggered(Exception):
     """内置选项解析触发"""
-
-
-class TerminateLoop(Exception):
-    """终止循环"""
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/formatter.py` & `arclet-alconna-1.7.1/src/arclet/alconna/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
-from contextlib import suppress
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any
+
+from nepattern import AllParam, AnyOne, AnyString
 from tarina import Empty, lang
-from nepattern import AllParam, BasePattern
 
 from .args import Arg, Args
 from .base import Option, Subcommand
 
 if TYPE_CHECKING:
     from .core import Alconna
 
@@ -185,15 +185,16 @@
         if str(parameter.value).strip("'\"") == name:
             return f"[{name}]" if parameter.optional else name
         if parameter.hidden:
             return f"[{name}]" if parameter.optional else f"<{name}>"
         if parameter.value is AllParam:
             return f"<...{name}>"
         arg = f"[{name}" if parameter.optional else f"<{name}"
-        arg += f": {parameter.value}"
+        if parameter.value not in (AnyOne, AnyString):
+            arg += f": {parameter.value}"
         if parameter.field.display is Empty:
             arg += " = None"
         elif parameter.field.display is not None:
             arg += f" = {parameter.field.display}"
         return f"{arg}]" if parameter.optional else f"{arg}>"
 
     def parameters(self, args: Args) -> str:
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/i18n/en-US.json` & `arclet-alconna-1.7.1/src/arclet/alconna/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/i18n/zh-CN.json` & `arclet-alconna-1.7.1/src/arclet/alconna/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/manager.py` & `arclet-alconna-1.7.1/src/arclet/alconna/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 import contextlib
 import re
 import shelve
 import weakref
 from copy import copy
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Match, TypedDict, Union, overload, Generic
-from typing_extensions import NotRequired
-from tarina import LRU, lang
+from typing import TYPE_CHECKING, Any, Generic, Match, TypedDict, Union, overload
 from weakref import WeakKeyDictionary, WeakValueDictionary
 
+from tarina import LRU, lang
+from typing_extensions import NotRequired
+
 from .argv import Argv, __argv_type__
 from .arparma import Arparma
 from .config import Namespace, config
 from .exceptions import ExceedMaxCount
-from .typing import DataCollection, TDC, CommandMeta
-
+from .typing import TDC, CommandMeta, DataCollection
 
 if TYPE_CHECKING:
     from ._internal._analyser import Analyser
     from .core import Alconna
 
 
     class ShortcutArgs(TypedDict, Generic[TDC]):
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/model.py` & `arclet-alconna-1.7.1/src/arclet/alconna/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from dataclasses import dataclass
 _repr_ = lambda self: "(" + " ".join([f"{k}={getattr(self, k, ...)!r}" for k in self.__slots__]) + ")"
 
 
 @dataclass(init=False, eq=True)
 class Sentence:
     __slots__ = ("name")
-    __repr__ = _repr_
+    __str__ = lambda self: self.name
+    __repr__ = lambda self: self.name
     def __init__(self, name):
         self.name = name
 
 
 @dataclass(init=False, eq=True)
 class OptionResult:
     __slots__ = ("value", "args")
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/model.pyi` & `arclet-alconna-1.7.1/src/arclet/alconna/model.pyi`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/output.py` & `arclet-alconna-1.7.1/src/arclet/alconna/output.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/stub.py` & `arclet-alconna-1.7.1/src/arclet/alconna/stub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass, field
 from inspect import isclass
 from typing import Any, Generic, TypeVar
+
 from nepattern import AllParam, AnyOne, BasePattern
 from typing_extensions import Self
 
 from .args import Args
 from .base import Option, Subcommand
 from .model import OptionResult, SubcommandResult
```

### Comparing `arclet-alconna-1.7.0rc7/src/arclet/alconna/typing.py` & `arclet-alconna-1.7.1/src/arclet/alconna/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Alconna 参数相关"""
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TypeVar, Iterator, runtime_checkable, Protocol, Union, Any, Literal, Tuple, Dict, List
-from nepattern import BasePattern, type_parser, MatchMode
+from typing import Any, Dict, Iterator, List, Literal, Protocol, Tuple, TypeVar, Union, runtime_checkable
+
+from nepattern import BasePattern, MatchMode, type_parser
 
 TPrefixes = Union[List[Union[str, object]], List[Tuple[object, str]]]
 DataUnit = TypeVar("DataUnit", covariant=True)
 
 
 @runtime_checkable
 class DataCollection(Protocol[DataUnit]):
```

### Comparing `arclet-alconna-1.7.0rc7/tests/analyser_test.py` & `arclet-alconna-1.7.1/tests/analyser_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,49 +39,49 @@
 
 
 Face = gen_unit("face")
 At = gen_unit("at")
 
 
 def test_filter_out():
-    argv_config(filter_out=["int"])
+    argv_config(filter_out=[int])
     ana = Alconna("ana", Args["foo", str])
     assert ana.parse(["ana", 123, "bar"]).matched is True
     assert ana.parse("ana bar").matched is True
     argv_config(filter_out=[])
     ana_1 = Alconna("ana", Args["foo", str])
     assert ana_1.parse(["ana", 123, "bar"]).matched is False
 
 
 def test_preprocessor():
-    argv_config(preprocessors={"float": int})
+    argv_config(preprocessors={float: int})
     ana1 = Alconna("ana1", Args["bar", int])
     assert ana1.parse(["ana1", 123.06]).matched is True
     assert ana1.parse(["ana1", 123.06]).bar == 123
     argv_config(preprocessors={})
     ana1_1 = Alconna("ana1", Args["bar", int])
     assert ana1_1.parse(["ana1", 123.06]).matched is False
 
 
 def test_with_set_unit():
     argv_config(
-        preprocessors={"Segment": lambda x: str(x) if x.type == "text" else None}
+        preprocessors={Segment: lambda x: str(x) if x.type == "text" else None}
     )
 
     ana2 = Alconna("ana2", Args["foo", At]["bar", Face])
     res = ana2.parse([Segment.text("ana2"), Segment.at(123456), Segment.face(103)])
     assert res.matched is True
     assert res.foo.data['qq'] == '123456'
     assert not ana2.parse([Segment.text("ana2"), Segment.face(103), Segment.at(123456)]).matched
     argv_config()
 
 
 def test_unhashable_unit():
     argv_config(
-        preprocessors={"Segment": lambda x: str(x) if x.type == "text" else None}
+        preprocessors={Segment: lambda x: str(x) if x.type == "text" else None}
     )
 
     ana3 = Alconna("ana3", Args["foo", At])
     print(ana3.parse(["ana3", Segment.at(123)]))
     print(ana3.parse(["ana3", Segment.face(123)]))
 
     ana3_1 = Alconna("ana3_1", Option("--foo", Args["bar", int]))
```

### Comparing `arclet-alconna-1.7.0rc7/tests/args_test.py` & `arclet-alconna-1.7.1/tests/args_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,27 +120,33 @@
     assert analyse_args(arg11_2, ["1.2"]) == analyse_args(arg11_1, ["1.2"])
 
 
 def test_optional():
     arg13 = Args.foo[str].add("bar", value=int, flags="?")
     assert analyse_args(arg13, ["abc 123"]) == {"foo": "abc", "bar": 123}
     assert analyse_args(arg13, ["abc"]) == {"foo": "abc"}
+    arg13_1 = Args.foo[str]["bar?", int]
+    assert analyse_args(arg13_1, ["abc 123"]) == {"foo": "abc", "bar": 123}
+    assert analyse_args(arg13_1, ["abc"]) == {"foo": "abc"}
+    arg13_2 = Args.foo[str]["bar;?", int]
+    assert analyse_args(arg13_2, ["abc 123"]) == {"foo": "abc", "bar": 123}
+    assert analyse_args(arg13_2, ["abc"]) == {"foo": "abc"}
 
 
 def test_kwonly():
     arg14 = Args.foo[str].add("bar", value=Kw[int])
     assert analyse_args(arg14, ["abc bar=123"]) == {
         "foo": "abc",
         "bar": 123,
     }
     assert analyse_args(arg14, ["abc 123"], raise_exception=False) != {
         "foo": "abc",
         "bar": 123,
     }
-    arg14_1 = Args["--width;?", Kw[int], 1280]["--height;?", Kw[int], 960]
+    arg14_1 = Args["--width;?", Kw[int], 1280]["--height?", Kw[int], 960]
     assert analyse_args(arg14_1, ["--width=960 --height=960"]) == {
         "--width": 960,
         "--height": 960,
     }
     arg14_2 = Args.foo[str]["bar", KeyWordVar(int, " ")]["baz", KeyWordVar(bool, ":")]
     assert analyse_args(arg14_2, ["abc -bar 123 baz:false"]) == {
         "bar": 123,
```

### Comparing `arclet-alconna-1.7.0rc7/tests/base_test.py` & `arclet-alconna-1.7.1/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc7/tests/components_test.py` & `arclet-alconna-1.7.1/tests/components_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc7/tests/config_test.py` & `arclet-alconna-1.7.1/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc7/tests/core_test.py` & `arclet-alconna-1.7.1/tests/core_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,16 +408,19 @@
     assert res5.content == "print(123)"
     assert not alc16_1.parse("echo 123 456").matched
     res6 = alc16_1.parse(["echo1", "123", "456 789"])
     assert res6.content == "print('123\n456\n789')"
 
 
 def test_help():
+    from arclet.alconna.exceptions import SpecialOptionTriggered
+
     alc17 = Alconna("core17") + Option("foo", Args["bar", str])
-    alc17.parse("core17 --help")
+    res = alc17.parse("core17 --help")
+    assert isinstance(res.error_info, SpecialOptionTriggered)
     alc17.parse("core17 --help foo")
     alc17_1 = Alconna(
         "core17_1",
         Option("foo bar abc baz", Args["qux", int]),
         Option("foo qux bar", Args["baz", str]),
     )
     alc17_1.parse("core17_1 --help")
@@ -436,14 +439,16 @@
         "bar", Args["baz#ANOTHER TEST", KeyWordVar(str)]
     )
     print("")
     print(alc19.get_help())
 
 
 def test_completion():
+    from arclet.alconna.exceptions import SpecialOptionTriggered
+
     alc20 = (
         "core20"
         + Option("fool")
         + Option(
             "foo",
             Args.bar[
                 "a|b|c", Field(completion=lambda: "test completion; choose a, b or c")
@@ -460,15 +465,16 @@
     alc20.parse("core20 f --comp")
     alc20.parse("core20 fo --comp")
     alc20.parse("core20 foo --comp")
     alc20.parse("core20 fool --comp")
     alc20.parse("core20 off c --comp")
 
     alc20_1 = Alconna("core20_1", Args.foo[int], Option("bar"))
-    alc20_1.parse("core20_1 -cp")
+    res = alc20_1.parse("core20_1 -cp")
+    assert isinstance(res.error_info, SpecialOptionTriggered)
 
 
 def test_completion_interface():
     alc21 = Alconna("core21", Args.foo[int], Args.bar[str])
     print("\n", "no interface [failed]:", alc21.parse("core21"))
     print("\n", "interface [pending]:")
     with CompSession(alc21) as comp:
```

### Comparing `arclet-alconna-1.7.0rc7/PKG-INFO` & `arclet-alconna-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.0rc7
+Version: 1.7.1
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 License: MIT
 Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

