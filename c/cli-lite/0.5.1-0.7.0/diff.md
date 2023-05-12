# Comparing `tmp/cli-lite-0.5.1.tar.gz` & `tmp/cli-lite-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-lite-0.5.1.tar", last modified: Tue Jan 10 16:15:20 2023, max compression
+gzip compressed data, was "cli-lite-0.7.0.tar", last modified: Fri May 12 08:39:46 2023, max compression
```

## Comparing `cli-lite-0.5.1.tar` & `cli-lite-0.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-rw-rw-   0        0        0      112 2023-01-10 16:14:12.748142 cli-lite-0.5.1/clilte/__init__.py
--rw-rw-rw-   0        0        0     2632 2023-01-10 16:01:39.037163 cli-lite-0.5.1/clilte/builtin.py
--rw-rw-rw-   0        0        0     8512 2023-01-10 16:14:12.821947 cli-lite-0.5.1/clilte/main.py
--rw-rw-rw-   0        0        0     1092 2022-07-03 16:27:16.504000 cli-lite-0.5.1/LICENSE
--rw-rw-rw-   0        0        0     1205 2023-01-10 16:14:12.784046 cli-lite-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0      917 2023-01-10 16:14:50.411574 cli-lite-0.5.1/README.md
--rw-rw-rw-   0        0        0     1707 2023-01-10 16:15:20.188473 cli-lite-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      160 2023-05-12 07:56:09.908946 cli-lite-0.7.0/clilte/__init__.py
+-rw-r--r--   0        0        0     2434 2023-05-12 08:29:33.663742 cli-lite-0.7.0/clilte/builtin.py
+-rw-r--r--   0        0        0     8028 2023-05-12 08:19:17.334983 cli-lite-0.7.0/clilte/core.py
+-rw-r--r--   0        0        0     1092 2022-07-03 16:27:16.504000 cli-lite-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1213 2023-05-12 08:39:24.337139 cli-lite-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1069 2023-05-12 08:39:24.351103 cli-lite-0.7.0/README.md
+-rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 cli-lite-0.7.0/PKG-INFO
```

### Comparing `cli-lite-0.5.1/clilte/main.py` & `cli-lite-0.7.0/clilte/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,252 +2,235 @@
 
 import sys
 from abc import ABCMeta, abstractmethod
 from contextlib import contextmanager
 from contextvars import ContextVar
 from dataclasses import dataclass, field, InitVar
 from importlib.metadata import entry_points
-from typing import Any, Callable, TypeVar, overload, Literal
+from pathlib import Path
+from typing import Callable, TypeVar, overload, Literal
 
 from arclet.alconna import (
     Alconna,
     Arparma,
-    ArparmaBehavior,
+    Args,
+    Option,
+    CommandMeta,
     command_manager,
-    namespace,
-    output_manager,
+    namespace
 )
-from arclet.alconna.tools import ArgParserTextFormatter
+from arclet.alconna.exceptions import SpecialOptionTriggered
+from arclet.alconna.tools import ShellTextFormatter, RichConsoleFormatter
 
 cli_instance: ContextVar[CommandLine] = ContextVar("litecli")
 
 
 @dataclass
-class CommandMetadata:
+class PluginMetadata:
     name: str
     version: str
     description: str = field(default="Unknown")
     tags: list[str] = field(default_factory=list)
     author: list[str] = field(default_factory=list)
+    priority: int = field(default=16)
 
 
-def _generate_behavior(func: Callable[[Arparma], Any]) -> ArparmaBehavior:
-    class _(ArparmaBehavior):
-        operate = staticmethod(func)
-
-    return _()
-
-
-class BaseCommand(metaclass=ABCMeta):
-    _option = False
+class BasePlugin(metaclass=ABCMeta):
 
     def __init__(self):
-        self.metadata = self.meta()
-        self.command = self.init()
-        self.command.reset_namespace(
-            cli_instance.get().prefix, not self.__class__._option
-        )
-        self.command.behaviors.append(_generate_behavior(self.dispatch))
-        if (
-            not self.command.meta.description
-            or self.command.meta.description == "Unknown"
-        ):
-            self.command.meta = (
-                self.metadata.description or self.metadata.name or "Unknown"
-            )
-
-    def __init_subclass__(cls, **kwargs):
-        if kwargs.get("option", False):
-            cls._option = True
-        super().__init_subclass__()
+        self.metadata: PluginMetadata = self.meta()
+        self.command: Alconna | str = self.init()
+        if isinstance(self.command, Alconna):
+            self.name: str = self.command.name
+            if (
+                not self.command.meta.description
+                or self.command.meta.description == "Unknown"
+            ):
+                self.command.meta = (
+                        self.metadata.description or self.metadata.name or "Unknown"
+                )
+            command_manager.delete(self.command)
+            ns = cli_instance.get()._command.namespace_config
+            self.command.namespace = ns.name
+            self.command.path = f"{ns.name}::{self.command.name}"
+            self.command.prefixes = []
+            self.command.options = self.command.options[:-3]
+
+            self.command.meta.fuzzy_match = ns.fuzzy_match or self.command.meta.fuzzy_match
+            self.command.meta.raise_exception = ns.raise_exception or self.command.meta.raise_exception
+            self.command._hash = self.command._calc_hash()
+            command_manager.register(self.command)
+        else:
+            self.name: str = self.command
 
     @abstractmethod
-    def init(self) -> Alconna:
+    def init(self) -> Alconna | str:
         """
         插件创建方法, 该方法只会调用一次
+
+        若返回 Alconna, 则表示创建一个新的子命令, 该子命令的名称为插件的名称
+
+        若返回 str, 则表示该插件不创建子命令, 该 str 会成为插件的名称
         """
 
     @abstractmethod
-    def dispatch(self, result: Arparma):
+    def meta(self) -> PluginMetadata:
         """
-        当该插件命令解析成功后该方法负责将解析结果分发给指定的处理函数
+        提供描述信息的方法
         """
 
     @abstractmethod
-    def meta(self) -> CommandMetadata:
+    def dispatch(self, result: Arparma) -> bool | None:
         """
-        提供描述信息的方法
+        插件的主要逻辑
+
+        若返回 True, 则表示插件继续传播
+        若返回 None, 则表示插件传播结束
+        若返回 False, 则表示命令执行结束
+        """
+
+    def supply_options(self) -> list[Option] | None:
+        """
+        为主命令提供额外的选项
         """
+        return
 
 
-_storage: dict[str, list[type[BaseCommand]]] = {}
-TCommand = TypeVar("TCommand", bound=BaseCommand)
+_storage: dict[str, list[type[BasePlugin]]] = {}
+TPlugin = TypeVar("TPlugin", bound=BasePlugin)
 
 
 def register(target: str):
-    def wrapper(cls: type[BaseCommand]):
+    def wrapper(cls: type[BasePlugin]):
         _storage.setdefault(target, []).append(cls)
         return cls
 
     return wrapper
 
 
-@dataclass
-class Helper:
-    cli: CommandLine
-
-    def cmds(self):
-        yield from self.cli.commands.keys()
-
-    def cmd_descriptions(self):
-        for cmd in self.cli.commands.values():
-            yield cmd.metadata.description
-
-    def opts(self):
-        for name, opt in self.cli.options.items():
-            if opt.command.headers and opt.command.command:
-                yield f"[{''.join(map(str, opt.command.headers))}]{opt.command.command}"
-            elif opt.command.headers:
-                yield f"{', '.join(sorted(map(str, opt.command.headers), key=len))}"
-            else:
-                yield name
-
-    def opts_descriptions(self):
-        for opt in self.cli.commands.values():
-            yield opt.metadata.description
-
-    def cmd_line(self, name, desc, max_len: int = 0):
-        return f"  {name:<{max_len}}    {desc}"
-
-    def opt_line(self, name, desc, max_len: int = 0):
-        return f"  {name:<{max_len}}    {desc}"
-
-    def lines(self, cmd_title: str = "Commands", opt_title: str = "Options"):
-        cmds, opts, = list(self.cmds()), list(self.opts())
-        cmd_desc, opt_desc = list(self.cmd_descriptions()), list(self.opts_descriptions())
-        max_len = max(max(map(len, cmds or [''])), max(map(len, opts or [''])))
-        cmd_string = "\n".join(self.cmd_line(i, j, max_len) for i, j in zip(cmds, cmd_desc))
-        opt_string = "\n".join(self.opt_line(i, j, max_len) for i, j in zip(opts, opt_desc))
-        return f"{cmd_title}:\n{cmd_string}\n{opt_title}:\n{opt_string}"
-
-    def help(self):
-        footer = f"Use '{self.cli.prefix} <command> --help' for more information about a command."
-        return f"{self.cli.name}\n\n{self.lines()}\n\n{footer}"
-
-
 @dataclass(repr=True)
 class CommandLine:
-    prefix: str
-    name: str
+    title: str
     version: str
-    output_action: Callable[[str], ...] = field(default=lambda x: print(x))
+    _name: InitVar[str | None] = field(default=None)
     load_preset: bool = field(default=True)
+    rich: bool = field(default=False)
     fuzzy_match: InitVar[bool] = field(default=False)
-    argparser_formatter: InitVar[bool] = field(default=False)
-    _helper: InitVar[type[Helper]] = field(default=Helper)
-    helper: Helper = field(init=False)
-    commands: dict[str, BaseCommand] = field(init=False, default_factory=dict)
-    options: dict[str, BaseCommand] = field(init=False, default_factory=dict)
-
-    def __post_init__(self, fuzzy_match: bool, argparser_formatter: bool, _helper: type[Helper]):
-        self.prefix = self.prefix.lower().replace(" ", "_")
-        self.helper = _helper(self)
-        with namespace(self.prefix) as np:
+    plugins: dict[str, BasePlugin] = field(default_factory=dict, init=False)
+    _command: Alconna = field(init=False)
+    callback: Callable[[Arparma], None] = field(default_factory=lambda: (lambda x: None), init=False)
+
+    def __post_init__(self, _name: str | None, fuzzy_match: bool):
+        if _name is None:
+            self._command = Alconna(
+                formatter_type=RichConsoleFormatter if self.rich else ShellTextFormatter,
+                meta=CommandMeta(fuzzy_match=fuzzy_match, description=self.title)
+            )
+        else:
+            self._command = Alconna(
+                _name,
+                formatter_type=RichConsoleFormatter if self.rich else ShellTextFormatter,
+                meta=CommandMeta(fuzzy_match=fuzzy_match, description=self.title),
+            )
+        with namespace(self.name) as np:
             np.headers = []
             np.separators = (" ",)
             np.fuzzy_match = fuzzy_match
-            if argparser_formatter:
-                np.formatter_type = ArgParserTextFormatter
+            np.formatter_type = RichConsoleFormatter if self.rich else ShellTextFormatter
+
+    @property
+    def name(self):
+        return self._command.command
 
     @classmethod
     def current(cls):
         return cli_instance.get()
 
     @contextmanager
     def using(self):
         token = cli_instance.set(self)
         yield
         cli_instance.reset(token)
 
-    def add(self, *command: type[TCommand]):
+    def arguments(self, args: Args):
+        command_manager.delete(self._command)
+        self._command.args.__merge__(args)
+        command_manager.register(self._command)
+
+    def set_callback(self, callback: Callable[[Arparma], None]):
+        self.callback = callback
+
+    def add(self, *command: type[TPlugin]):
         with self.using():
-            res: list[TCommand] = [cls() for cls in command]
+            res: list[TPlugin] = [cls() for cls in command]
         for plg in res:
-            if plg._option or plg.command.command.startswith("-"):
-                self.options[plg.command.name] = plg
-            else:
-                self.commands[plg.command.name] = plg
+            self.plugins[plg.name] = plg
+            if isinstance(plg.command, Alconna):
+                self._command.add(plg.command)
+            if _opts := plg.supply_options():
+                for _opt in _opts:
+                    self._command.add(_opt)
         return res
 
     def preset(self):
-        for cls in _storage.get(self.prefix, []) + _storage.get("*", []):
+        for cls in _storage.get(self._command.command, []) + _storage.get("*", []):
             self.add(cls)
 
     def load_register(self, target: str):
-        if target in (self.prefix, "*"):
+        if target in (self._command.command, "*"):
             return
         for cls in _storage.get(target, []):
             self.add(cls)
 
     def load_entry(self):
         for entry in entry_points().get(f"litecli.{self.name}.plugins", []):
             self.add(entry.load())
 
     @overload
-    def get_command(self, plg: type[TCommand], default: Literal[True]) -> TCommand:
+    def get_plugin(self, plg: type[TPlugin], default: Literal[True]) -> TPlugin:
         ...
 
-    def get_command(self, plg: type[TCommand], default: bool = False) -> TCommand | None:
+    def get_plugin(self, plg: type[TPlugin], default: bool = False) -> TPlugin | None:
         return next(
-            filter(lambda x: isinstance(x, plg), self.commands.values()),
+            filter(lambda x: isinstance(x, plg), self.plugins.values()),
             self.add(plg)[0] if default else None,
         )
 
     def query(self, *tag: str):
         yield from filter(
-            lambda x: set(x.metadata.tags).issuperset(tag), self.commands.values()
+            lambda x: set(x.metadata.tags).issuperset(tag), self.plugins.values()
         )
 
     @property
     def help(self):
-        return self.helper.help()
+        return self._command.get_help()
 
-    def main(self, args: list[str] | None = None):
+    def main(self, *args: str):
         if self.load_preset:
             self.preset()
         self.load_entry()
-        args = sys.argv[1:] or args
-        if args and args[0] == self.prefix:
-            args.pop(0)
-        if not args:
-            return self.output_action(self.help)
-        text = " ".join(args)
+        if args:
+            res = self._command.parse(list(args))  # type: ignore
+        else:
+            path = Path(sys.argv[0])
+            head = path.parent.stem if str(path.parent) not in (".", "/", "\\") else path.stem
+            if head != self._command.command:
+                res = self._command.parse(sys.argv[1:])  # type: ignore
+            else:
+                res = self._command.parse([head, *sys.argv[1:]])  # type: ignore
+        if not res.matched:
+            if isinstance(res.error_info, SpecialOptionTriggered):
+                return
+            return print(res.error_info)
+        if res.non_component and not res.all_matched_args:
+            return print(self.help)
         with self.using():
-            for alc in command_manager.get_commands(namespace=self.prefix):
-                may_output_text = None
-
-                def _h(string):
-                    nonlocal may_output_text
-                    may_output_text = string
-
-                output_manager.set_action(_h, alc.name)
-                try:
-                    _res = alc.parse(text)
-                except Exception as e:
-                    _res = Arparma(alc.path, text)
-                    _res.head_matched = False
-                    _res.matched = False
-                    _res.error_info = repr(e)
-                if not may_output_text and not _res.matched and not _res.head_matched:
-                    continue
-                if not may_output_text and _res.error_info:
-                    may_output_text = f"{self.name}\n\n{alc.get_help()}"
-                if not may_output_text and _res.matched:
+            for plg in sorted(self.plugins.values(), key=lambda x: x.metadata.priority):
+                ans = plg.dispatch(res)
+                if ans is None:
                     break
-                if may_output_text:
-                    self.output_action(may_output_text)
-                    break
-            else:
-                return self.output_action(self.help)
+                if not ans:
+                    return
+            self.callback(res)
 
 
-__all__ = ["CommandMetadata", "BaseCommand", "CommandLine", "register", "Helper"]
+__all__ = ["PluginMetadata", "BasePlugin", "CommandLine", "register"]
```

### Comparing `cli-lite-0.5.1/LICENSE` & `cli-lite-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-lite-0.5.1/pyproject.toml` & `cli-lite-0.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "cli-lite"
-version = "0.5.1"
+version = "0.7.0"
 description = "A simple framework to build a cli tool, base on Alconna"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
-    "arclet-alconna>=1.4.3",
-    "arclet-alconna-tools>=0.3.3",
+    "arclet-alconna<2.0.0, >=1.7.1",
+    "arclet-alconna-tools>=0.6.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "commandline",
     "cli-tool",
     "plugin",
```

### Comparing `cli-lite-0.5.1/PKG-INFO` & `cli-lite-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-lite
-Version: 0.5.1
+Version: 0.7.0
 Summary: A simple framework to build a cli tool, base on Alconna
 License: MIT
 Keywords: commandline,cli-tool,plugin,cli,litecli
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -29,40 +29,44 @@
 ```
 
 ## example
 
 write as sample:
 
 ```python
-from clilte import BaseCommand, CommandLine, CommandMetadata
-from arclet.alconna import Alconna, Arparma, Args
+# example.py
+from clilte import BasePlugin, CommandLine, PluginMetadata
+from arclet.alconna import Alconna, Arparma, Args, CommandMeta
 
 
-class MyCommand(BaseCommand):
+class MyPlugin(BasePlugin):
 
-    def init(self) -> Alconna:
-        return Alconna("hello", Args["name", str])
+    def init(self) -> Alconna | str:
+        return Alconna("hello", Args["name", str], meta=CommandMeta("test command"))
 
-    def dispatch(self, result: Arparma):
-        return print(f"Hello! {result.name}")
+    def meta(self) -> PluginMetadata:
+        return PluginMetadata("hello", "0.0.1", "my first plugin", ["dev"], ["john"])
 
-    def meta(self) -> CommandMetadata:
-        return CommandMetadata("hello", "0.0.1", "my first plugin", ["dev"], ["john"])
+    def dispatch(self, result: Arparma) -> bool | None:
+        return print(f"Hello! {result.name}")
 
 
 if __name__ == '__main__':
-    cli = CommandLine(
-        "test",
-        "My first CLI",
-        "0.0.1"
-    )
-    cli.add(MyCommand)
+    cli = CommandLine(title="My first CLI", version="example 0.0.1")
+    cli.add(MyPlugin)
+    cli.load_register('builtin.cache')
     cli.main()
 ```
 
 and execute the line:
 
-```powershell
-python test.py hello world
+```shell
+python example.py hello world
+```
+
+you will get the result:
+
+```shell
+Hello! world
 ```
```

