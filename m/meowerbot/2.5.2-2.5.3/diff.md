# Comparing `tmp/meowerbot-2.5.2.tar.gz` & `tmp/meowerbot-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meowerbot-2.5.2.tar", max compression
+gzip compressed data, was "meowerbot-2.5.3.tar", max compression
```

## Comparing `meowerbot-2.5.2.tar` & `meowerbot-2.5.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.5.2/LICENSE
--rw-r--r--   0        0        0      154 2023-04-24 21:38:04.560934 meowerbot-2.5.2/MeowerBot/__init__.py
--rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.5.2/MeowerBot/_Commands.py
--rw-r--r--   0        0        0     1381 2023-04-24 21:38:04.548919 meowerbot-2.5.2/MeowerBot/API.py
--rw-r--r--   0        0        0    13593 2023-04-18 21:45:43.038089 meowerbot-2.5.2/MeowerBot/Bot.py
--rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.5.2/MeowerBot/cloudlink/__init__.py
--rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.5.2/MeowerBot/cloudlink/cloudlink.py
--rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.5.2/MeowerBot/cog.py
--rw-r--r--   0        0        0     2084 2023-04-15 02:19:55.402707 meowerbot-2.5.2/MeowerBot/command.py
--rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.5.2/MeowerBot/context.py
--rw-r--r--   0        0        0      566 2023-04-24 21:38:04.561918 meowerbot-2.5.2/pyproject.toml
--rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.5.2/README.md
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 meowerbot-2.5.2/setup.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 meowerbot-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.5.3/LICENSE
+-rw-r--r--   0        0        0      154 2023-04-24 21:38:04.560934 meowerbot-2.5.3/MeowerBot/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.5.3/MeowerBot/_Commands.py
+-rw-r--r--   0        0        0     1381 2023-04-24 21:38:04.548919 meowerbot-2.5.3/MeowerBot/API.py
+-rw-r--r--   0        0        0    13858 2023-05-12 00:23:19.898042 meowerbot-2.5.3/MeowerBot/Bot.py
+-rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.5.3/MeowerBot/cloudlink/__init__.py
+-rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.5.3/MeowerBot/cloudlink/cloudlink.py
+-rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.5.3/MeowerBot/cog.py
+-rw-r--r--   0        0        0     2436 2023-05-12 00:38:58.514877 meowerbot-2.5.3/MeowerBot/command.py
+-rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.5.3/MeowerBot/context.py
+-rw-r--r--   0        0        0      566 2023-05-12 00:40:21.284157 meowerbot-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.5.3/README.md
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 meowerbot-2.5.3/setup.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 meowerbot-2.5.3/PKG-INFO
```

### Comparing `meowerbot-2.5.2/LICENSE` & `meowerbot-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.2/MeowerBot/API.py` & `meowerbot-2.5.3/MeowerBot/API.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.2/MeowerBot/Bot.py` & `meowerbot-2.5.3/MeowerBot/Bot.py`

 * *Files 9% similar despite different names*

```diff
@@ -91,14 +91,20 @@
 
     def run_cb(self, cbid, args=(), kwargs=None):  # cq: ignore
         if cbid not in self.callbacks:
             return  # ignore
 
         if not kwargs:
             kwargs = {}
+        
+        if cbid == "error" and isinstance(args[0], KeyboardInterrupt()): 
+            self.logger.error("KeyboardInterrupt")
+            self.bad_exit = True
+            self.stop()
+            return 
 
         kwargs["bot"] = self
         for callback in self.callbacks[cbid]:
             try:
                 callback(
                     *args, **kwargs
                 )  # multi callback per id is supported (unlike cloudlink 0.1.7.3 LOL)
@@ -133,25 +139,14 @@
             self.logger.error(traceback.format_exc())
             self.run_cb("error", args=(e, ))
 
     def __handle_on_connect__(self):
         self.wss.sendPacket(
             {
                 "cmd": "direct",
-                "val": {
-                    "cmd": "ip",
-                    "val": requests.get("https://api.meower.org/ip").text,
-                },
-                "listener": "__meowerbot__send_ip",
-            }
-        )
-
-        self.wss.sendPacket(
-            {
-                "cmd": "direct",
                 "val": {"cmd": "type", "val": "py"},
             }
         )
         self.wss.sendPacket(
             {
                 "cmd": "direct",
                 "val": "meower",
@@ -169,15 +164,15 @@
             cmd = AppCommand(func, name=name, args=args)
 
             info = cmd.info()
             info[cmd.name]["command"] = cmd
 
             self.commands.update(info)
 
-            return func
+            return cmd #allow subcommands without a cog
 
         return inner
 
     def register_cog(self, cog):
         info = cog.get_info()
         self.cogs[cog.__class__.__name__] = cog
         self.commands.update(info)
@@ -257,30 +252,38 @@
 
             self.wss.state = 0 #type: ignore
             self.wss.client(self.server) #type: ignore
             return #dont want the close callback to be called here
 
         self.run_cb("close", args=args, kwargs=kwargs)
 
+    def handle_bridges(self, packet):
+        if packet["val"]["u"] in self.__bridges__ and ": " in packet["val"]["p"]:
+                split = packet["val"]["p"].split(": ", 1)
+                packet["val"]["p"] = split[1]
+                packet["val"]["u"] = split[0]
+        
+        if packet["val"]["p"].startswith(self.prefix+"#0000"):
+            packet["val"]["p"] = packet["val"]["p"].replace("#0000", self.prefix)
+        
+        return packet
+
     def __handle_packet__(self, packet):
         if packet["cmd"] == "statuscode":
 
             self._handle_status(packet["val"], packet.get("listener", None))
 
             listener = packet.get("listener", None)
             return self.run_cb("statuscode", args=(packet["val"], listener))
 
         elif packet["cmd"] == "ulist":
             self.run_cb("ulist", self.wss.statedata["ulist"]["usernames"])
 
         elif packet["cmd"] == "direct" and "post_origin" in packet["val"]:
-            if packet["val"]["u"] in self.__bridges__ and ": " in packet["val"]["p"]:
-                split = packet["val"]["p"].split(": ", 1)
-                packet["val"]["p"] = split[1]
-                packet["val"]["u"] = split[0]
+            packet = self.handle_bridges(packet)
 
             ctx = CTX(packet["val"], self)
             if "message" in self.callbacks:
                 self.run_cb("message", args=(ctx.message,))
 
             else:
 
@@ -320,14 +323,15 @@
 
     def run_command(self, message):
         args = shlex.split(str(message))
 
         try:
             self.commands[args[0]]["command"].run_cmd(message.ctx, *args[1:])
         except KeyError as e:
+            self.logger.error(traceback.format_exc())
             self.run_cb("error", args=(e,))
 
     def send_msg(self, msg, to="home"):
         self._last_to = to
         self._last_sent = msg
         try:
             if to == "home":
```

### Comparing `meowerbot-2.5.2/MeowerBot/cloudlink/cloudlink.py` & `meowerbot-2.5.3/MeowerBot/cloudlink/cloudlink.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.2/MeowerBot/cog.py` & `meowerbot-2.5.3/MeowerBot/cog.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.2/MeowerBot/command.py` & `meowerbot-2.5.3/MeowerBot/command.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,32 +19,44 @@
 
     def __call__(self, *args):
         raise RuntimeError("AppCommand is not callable")
 
     def register_class(self, con):
         self.connected = con
 
+        for subcommand in self.subcommands.values():
+            subcommand.register_class(con)
+
     def subcommand(self, name=None, args=0):
         def inner(func):
 
             cmd = AppCommand(func, name=name, args=args)
             cmd.register_class(self.connected)
 
-            self.subcommands[name] = cmd.info()
+            self.subcommands.update(cmd.info())
 
 
             return func #dont want mb to register this as a root command
-
         return inner
+    
 
     def run_cmd(self, ctx, *args):
+        print(
+            f"Running command {self.name} with args {args} and ctx {ctx} and connected {self.connected}"
+
+        )
         
-        if self.subcommands and (args[0] if len(args) >= 1 else None) in self.subcommands:
+        try:
             self.subcommands[args[0]]["command"].run_cmd(ctx, *args[1:])
             return
+        except KeyError:
+            print(f"KeyError: {args}")
+            print(f"Subcommands: {self.subcommands}")
+        except IndexError:
+            print(f"IndexError: {args}")
         
         if not self.args == 0:
             args = args[: self.args]
 
         if self.connected is None:
             self.func(ctx, *args)
         else:
```

### Comparing `meowerbot-2.5.2/MeowerBot/context.py` & `meowerbot-2.5.3/MeowerBot/context.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.2/pyproject.toml` & `meowerbot-2.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MeowerBot"
-version = "2.5.2"
+version = "2.5.3"
 description = "A meower bot lib for py"
 authors = ["showierdata9978 <68120127+showierdata9978@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "MeowerBot"}
 ]
```

### Comparing `meowerbot-2.5.2/setup.py` & `meowerbot-2.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.0,<3.0.0', 'websocket-client']
 
 setup_kwargs = {
     'name': 'meowerbot',
-    'version': '2.5.2',
+    'version': '2.5.3',
     'description': 'A meower bot lib for py',
     'long_description': '# MeowerBot.py\n\nA bot lib for Meower\n\n\n## License\n\nsee [LICENSE](./LICENSE)\n\n\n## docs\n\nThe Docs are located [here](https://meowerbot-py.showierdata.tech/)\n\n\n## Quick Example\n\nlook at the [tests directory](./tests) for examples ',
     'author': 'showierdata9978',
     'author_email': '68120127+showierdata9978@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/MeowerBots/MeowerBot.py',
```

### Comparing `meowerbot-2.5.2/PKG-INFO` & `meowerbot-2.5.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meowerbot
-Version: 2.5.2
+Version: 2.5.3
 Summary: A meower bot lib for py
 Home-page: https://github.com/MeowerBots/MeowerBot.py
 License: MIT
 Author: showierdata9978
 Author-email: 68120127+showierdata9978@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

