# Comparing `tmp/rnsh-0.0.9.tar.gz` & `tmp/rnsh-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnsh-0.0.9.tar", max compression
+gzip compressed data, was "rnsh-0.1.0.tar", max compression
```

## Comparing `rnsh-0.0.9.tar` & `rnsh-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1105 2023-02-11 05:21:53.643929 rnsh-0.0.9/LICENSE
--rw-r--r--   0        0        0    10326 2023-02-14 21:43:08.818325 rnsh-0.0.9/README.md
--rw-r--r--   0        0        0      659 2023-02-18 19:12:59.806758 rnsh-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1623 2023-02-14 21:43:08.818325 rnsh-0.0.9/rnsh/__init__.py
--rw-r--r--   0        0        0     5517 2023-02-14 21:43:08.818325 rnsh-0.0.9/rnsh/args.py
--rw-r--r--   0        0        0      798 2023-02-17 16:48:38.181439 rnsh-0.0.9/rnsh/exception.py
--rw-r--r--   0        0        0      210 2023-02-18 06:09:41.069929 rnsh-0.0.9/rnsh/helpers.py
--rw-r--r--   0        0        0    25592 2023-02-18 14:10:38.940197 rnsh-0.0.9/rnsh/process.py
--rw-r--r--   0        0        0    11619 2023-02-18 06:09:41.069929 rnsh-0.0.9/rnsh/protocol.py
--rw-r--r--   0        0        0     7661 2023-02-18 06:09:41.069929 rnsh-0.0.9/rnsh/retry.py
--rw-r--r--   0        0        0    20447 2023-02-18 13:44:36.361172 rnsh-0.0.9/rnsh/rnsh.py
--rw-r--r--   0        0        0     5225 2023-02-18 14:10:38.940197 rnsh-0.0.9/rnsh/rnslogging.py
--rw-r--r--   0        0        0    16291 2023-02-18 06:09:41.069929 rnsh-0.0.9/rnsh/session.py
--rw-r--r--   0        0        0     1609 2023-02-11 14:06:05.513301 rnsh-0.0.9/rnsh/testlogging.py
--rw-r--r--   0        0        0    11334 1970-01-01 00:00:00.000000 rnsh-0.0.9/setup.py
--rw-r--r--   0        0        0    10901 1970-01-01 00:00:00.000000 rnsh-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-02-11 05:21:53.643929 rnsh-0.1.0/LICENSE
+-rw-r--r--   0        0        0    11943 2023-02-25 11:21:04.980385 rnsh-0.1.0/README.md
+-rw-r--r--   0        0        0      799 2023-05-12 14:08:15.604382 rnsh-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1708 2023-05-11 18:54:53.778369 rnsh-0.1.0/rnsh/__init__.py
+-rw-r--r--   0        0        0     5806 2023-02-23 12:37:08.619322 rnsh-0.1.0/rnsh/args.py
+-rw-r--r--   0        0        0      798 2023-02-17 16:48:38.181439 rnsh-0.1.0/rnsh/exception.py
+-rw-r--r--   0        0        0      817 2023-02-19 00:35:54.411700 rnsh-0.1.0/rnsh/helpers.py
+-rw-r--r--   0        0        0    14698 2023-05-11 18:27:14.823616 rnsh-0.1.0/rnsh/initiator.py
+-rw-r--r--   0        0        0     7255 2023-05-11 18:27:14.823616 rnsh-0.1.0/rnsh/listener.py
+-rw-r--r--   0        0        0      644 2023-02-23 12:37:08.623322 rnsh-0.1.0/rnsh/loop.py
+-rw-r--r--   0        0        0    25592 2023-02-18 14:10:38.940197 rnsh-0.1.0/rnsh/process.py
+-rw-r--r--   0        0        0     4206 2023-03-08 22:54:16.949580 rnsh-0.1.0/rnsh/protocol.py
+-rw-r--r--   0        0        0     7661 2023-02-18 06:09:41.069929 rnsh-0.1.0/rnsh/retry.py
+-rw-r--r--   0        0        0     5749 2023-05-11 18:27:14.823616 rnsh-0.1.0/rnsh/rnsh.py
+-rw-r--r--   0        0        0     5225 2023-02-18 14:10:38.940197 rnsh-0.1.0/rnsh/rnslogging.py
+-rw-r--r--   0        0        0    15334 2023-03-08 22:54:16.949580 rnsh-0.1.0/rnsh/session.py
+-rw-r--r--   0        0        0     1609 2023-02-11 14:06:05.513301 rnsh-0.1.0/rnsh/testlogging.py
+-rw-r--r--   0        0        0    12618 1970-01-01 00:00:00.000000 rnsh-0.1.0/PKG-INFO
```

### Comparing `rnsh-0.0.9/LICENSE` & `rnsh-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rnsh-0.0.9/README.md` & `rnsh-0.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,22 +5,14 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/rnsh?color=informational&label=Installs&logo=pypi)
 
 `rnsh` is a utility written in Python that facilitates shell 
 sessions over [Reticulum](https://reticulum.network) networks. 
 It is based on the `rnx` utility that ships with Reticulum and
 aims to provide a similar experience to SSH.
 
-`rnsh` is still a little raw; there are some things that are 
-implemented badly, and many other things that haven't been 
-built at all (yet). Signals (i.e. Ctrl-C) need some work, so have
-another terminal handy to send a SIGTERM if things glitch
-out.
-
-Anyway, there's a lot of room for improvement.
-
 ## Contents
 
 - [Alpha Disclaimer](#reminder--alpha-software)
 - [Recent Changes](#recent-changes)
 - [Quickstart](#quickstart)
 - [Options](#options)
 - [How it works](#how-it-works)
@@ -30,48 +22,35 @@
 ### Reminder: Alpha Software
 These early versions will be buggy. There will sometimes be major
 breaking changes to the command line parameters between releases.
 There will sometimes be breaking changes in the protocol between
 releases. Use at your own peril!
 
 ## Recent Changes
-### v0.0.8
-- Improved test suite exposed several issues with the handling of
-command line arguments which are now fixed
-- Fixed a race condition that would cause remote characters to be 
-  lost intermittently when running remote commands that finish
-  immediately.
-- Added automated testing that actually spins up a random listener
-  and initiator in a private Reticulum network and passes data
-  between them, uncovering more issues which are now fixed.
-- Fixed (hopefully) an issue where `rnsh` doesn't know what
-  version it is.
-
-### v0.0.7
-Added `-A` command line option. This listener option causes the
-remote command line to be appended to the arguments list of the
-launched program. This allows the listener to jail connections
-to a particular executable while still allowing parameters.
-
-### v0.0.6
-Minor improvements in transport efficiency
-
-### v0.0.5
-#### Remote command line and pipe compatibility
-Command line options have changed somewhat to allow the initiator
-to supply a command line. This allows `rnsh` to function similarly
-to SSH. You can pipe into or out of `rnsh` to send input through
-remote commands or remote command output through other commands.
-
-This behavior can be blocked on the listener with the `-C` option.
-
-When the initiator does not supply a command, the listener uses
-a default command specified on its command line. If a default
-command is not specified, the listener falls back to the shell
-of the user it is running under.
+### v0.0.12
+- Remove service name from RNS destination aspects. Service name
+  now selects a suffix for the identity file and should only be
+  supplied on the listener. The initiator only needs the destination
+  hash of the listener to connect.
+- Show a spinner during link establishment on tty sessions
+- Attempt to catch and beautify exceptions on initiator
+
+### v0.0.11
+- Event loop bursting improves throughput and CPU utilization on
+  both listener and initiator.
+- Packet retries use RNS resend feature to prevent duplicate
+  packets.
+
+### v0.0.10
+- Rate limit window change events to prevent saturation of transport
+- Tweaked some loop timers to improve CPU utilization
+
+### v0.0.9
+- Switch to a new packet-based protocol
+- Bug fixes and dependency updates
 
 ## Quickstart
 
 Tested (thus far) on Python 3.11 macOS 13.1 ARM64. Should
 run on Python 3.6+ on Linux or Unix. WSL probably works. 
 Cygwin might work, too.
 
@@ -88,17 +67,16 @@
 ```shell
 # On listener
 rnsh -l -p
 
 # On initiator
 rnsh -p
 ```
-Note: if you are using a non-default identity or service name, be
-sure to supply these options with `-p` as the identity and 
-destination hashes will change depending on these settings.
+Note: service name no longer is supplied on initiator. The destination
+      hash encapsulates this information.
 
 #### Listener
 - Listening for default service name ("default").
 - Using user's default Reticulum config dir (~/.reticulum).
 - Using default identity ($RNSCONFIGDIR/storage/identities/rnsh).
 - Allowing remote identity `6d47805065fa470852cf1b1ef417a1ac` to connect.
 - Launching `/bin/zsh` on authorized connect.
@@ -113,28 +91,28 @@
 ```shell
 rnsh a5f72aefc2cb3cdba648f73f77c4e887
 ```
 
 ## Options
 ```
 Usage:
-    rnsh [--config <configdir>] [-i <identityfile>] [-s <service_name>] [-l] -p
-    rnsh -l [--config <configfile>] [-i <identityfile>] [-s <service_name>] 
-         [-v... | -q...] [-b <period>] (-n | -a <identity_hash> [-a <identity_hash>] ...) 
-         [-A | -C] [[--] <program> [<arg> ...]]
-    rnsh [--config <configfile>] [-i <identityfile>] [-s <service_name>] 
-         [-v... | -q...] [-N] [-m] [-w <timeout>] <destination_hash> 
-         [[--] <program> [<arg> ...]]
+    rnsh -l [-c <configdir>] [-i <identityfile> | -s <service_name>] [-v... | -q...] -p
+    rnsh -l [-c <configdir>] [-i <identityfile> | -s <service_name>] [-v... | -q...] 
+            [-b <period>] (-n | -a <identity_hash> [-a <identity_hash>] ...) [-A | -C] 
+            [[--] <program> [<arg> ...]]
+    rnsh [-c <configdir>] [-i <identityfile>] [-v... | -q...] -p
+    rnsh [-c <configdir>] [-i <identityfile>] [-v... | -q...] [-N] [-m] [-w <timeout>] 
+         <destination_hash> [[--] <program> [<arg> ...]]
     rnsh -h
     rnsh --version
 
 Options:
-    --config DIR                 Alternate Reticulum config directory to use
+    -c DIR --config DIR          Alternate Reticulum config directory to use
     -i FILE --identity FILE      Specific identity file to use
-    -s NAME --service NAME       Listen on/connect to specific service name if not default
+    -s NAME --service NAME       Service name for identity file if not default
     -p --print-identity          Print identity information and exit
     -l --listen                  Listen (server) mode. If supplied, <program> <arg>...will 
                                    be used as the command line when the initiator does not
                                    provide one or when remote command is disabled. If
                                    <program> is not supplied, the default shell of the 
                                    user rnsh is running under will be used.
     -b --announce PERIOD         Announce on startup and every PERIOD seconds
@@ -161,22 +139,38 @@
 ## How it works
 ### Listeners
 Listener instances are the servers. Each listener is configured 
 with an RNS identity, and a service name. Together, RNS makes
 these into a destination hash that can be used to connect to
 your listener.
    
-Multiple listeners can use the same identity. As long as 
-they are given different service names. They will have 
-different destination hashes and not conflict.
-
-Listeners must be configured with a command line to run (at 
-least at this time). The identity hash string is set in the
-environment variable RNS_REMOTE_IDENTITY for use in child
-programs.
+Each listener must use a unique identity. The `-s` parameter
+can be used to specify a service name, which creates a unique
+identity file.
+
+Listeners can be configured with a command line to run on
+connect. Initiators can supply a command line as well. There 
+are several different options for the way the command line 
+is handled:
+
+- `-C` no initiator command line is allowed; the connection will
+  be terminated if one is supplied.
+- `-A` initiator-supplied command line is appended to listener-
+  configured command line
+- With neither of these options, the listener will use the first 
+  valid command line from this list:
+  1. Initiator-supplied command line
+  2. Listener command line argument
+  3. Default shell of user listener is running under
+
+
+If the `-n` option is not set on the listener, the initiator
+is required to identify before starting a command. The program 
+will be started with the initiator's identity hash string is set 
+in the environment variable `RNS_REMOTE_IDENTITY`.
 
 Listeners are set up using the `-l` flag.
    
 ### Initiators
 Initiators are the clients. Each initiator has an identity
 hash which is used as an authentication mechanism on Reticulum.
 You'll need this value to configure the listener to allow 
@@ -192,55 +186,99 @@
 initiator.
     
 I recommend staying pretty vanilla to start with and
 trying `/bin/zsh` or whatever your favorite shell is these 
 days. The shell should start in login mode. Ideally it
 works just like an `ssh` shell session.
 
-### Protocol
-The protocol is build on top of the Reticulum `Request` and
-`Packet` APIs.
-
-- After the initiator identifies on the connection, it enters
-  a request loop. 
-- When idle, the initiator will periodically 
-  poll the listener. 
-- When the initiator has data available (i.e the user typed 
-  some characters), the initiator will send that data to the
-  listener in a request, and the listener will respond with 
-  any data available from the listener. 
-- When the listener has new data available, it notifies the 
-  initiator using a notification packet. The initiator then 
-  makes a request to the listener to fetch the data.
+## Protocol
+The protocol is build on top of the Reticulum `Packet` API.
+Application software sends and receives `Message` objects,
+which are encapsulated by `Packet` objects. Messages are
+(currently) sent one per packet, and only one packet is
+sent at a time (per link). The next packet is not sent until 
+the receiver proves the outstanding packet.
+
+A future update will work to allow a sliding window of
+outstanding packets to improve channel utilization.
+
+### Session Establishment
+1. Initiator establishes link. Listener session enters state 
+   `LSSTATE_WAIT_IDENT`, or `LSSTATE_WAIT_VERS` if running
+   with `--no-auth` option.
+
+2. Initiator identifies on link if not using `--no-id`.
+   - If using `--allowed-hash`, listener validates identity 
+      against configuration and if no match, sends a 
+      protocol error message and tears down link after prune
+      timer.
+3. Initiator transmits a `VersionInformationMessage`, which
+   is evaluated by the server for compatibility. If
+   incompatible, a protocol error is sent. 
+4. Listener responds with a `VersionInfoMessage` and enters 
+   state `LSSTATE_WAIT_CMD`
+5. Initiator evaluates the listener's version information
+   for compatibility and if incompatible, tears down link.
+6. Initiator sends an `ExecuteCommandMessage` (which could 
+   be an empty command) and enters the session event loop.
+7. Listener evaluates the command message against the
+   configured options such as `-A` or `-C` and responds
+   with a protocol error if not allowed.
+8. Listener starts the program. If success, the listener
+   enters the session event loop. If failure, responds
+   with a `CommandExitedMessage`.
+
+### Session Event Loop
+##### Listener state `LSSTATE_RUNNING`
+Process messages received from initiator.
+- `WindowSizeMessage`: set window size on child tty if appropriate
+- `StreamDataMessage`: binary data stream for child process;
+  streams ids 0, 1, 2 = stdin, stdout, stderr
+- `NoopMessage`: no operation - listener replies with `NoopMessage`
+- When link is torn down, child process is terminated if running and 
+  session destroyed
+- If command terminates, a `CommandExitedMessage` is sent and session
+  is pruned after an idle timeout.
+##### Initiator state `ISSTATE_RUNNING`
+Process messages received from listener.
+- `ErrorMessage`: print error, terminate link, and exit
+- `StreamDataMessage`: binary stream information; 
+   streams ids 0, 1, 2 = stdin, stdout, stderr
+- `CommandExitedMessage`: remote command exited
+- If link is torn down unexpectedly, print message and exit
+
    
 ## Roadmap
 1. Plan a better roadmap
 2. ?
 3. Keep my day job
 
 ## TODO
 - [X] ~~Initial version~~
 - [X] ~~Pip package with command-line utility support~~
 - [X] ~~Publish to PyPI~~
 - [X] ~~Improve signal handling~~
 - [X] ~~Make it scriptable (currently requires a tty)~~
 - [X] ~~Protocol improvements (throughput!)~~
 - [X] ~~Documentation improvements~~
+- [X] ~~Fix issues with running `rnsh` in a binary pipeline, i.e. 
+  piping the output of `tar` over `rsh`.~~
 - [ ] Test on several platforms
 - [ ] Fix issues that come up with testing
-- [ ] Fix issues with running `rnsh` in a binary pipeline, i.e. 
-  piping the output of `tar` over `rsh`.
-- [ ] Beta release
+- [ ] v0.1.0 beta
 - [ ] Test and fix more issues
-- [ ] V1.0
+- [ ] More betas
 - [ ] Enhancement Ideas
-  - [ ] `authorized_keys` mode similar to SSH
+  - [ ] `authorized_keys` mode similar to SSH to allow one listener
+        process to serve multiple users
   - [ ] Git over `rnsh` (git remote helper)
   - [ ] Sliding window acknowledgements for improved throughput
+- [ ] v1.0 someday probably maybe
 
 ## Miscellaneous
 
-By piping into/out of `rnsh`, it should be possible to transfer
+By piping into/out of `rnsh`, it is possible to transfer
 files using the same method discussed in 
 [this article](https://cromwell-intl.com/open-source/tar-and-ssh.html).
-I tested it just now and it doesn't work right. There's probably some
-subtle garbling of the data at one end of the stream or the other.
+It's not terribly fast currently, due to the round-trip rule 
+enforced by the protocol. Sliding window acknowledgements will
+speed this up significantly.
```

### Comparing `rnsh-0.0.9/rnsh/__init__.py` & `rnsh-0.1.0/rnsh/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,13 +27,17 @@
 
 def _get_version():
     try:
         try:
             import tomli
             return tomli.load(open(os.path.join(os.path.dirname(module_dir), "pyproject.toml"), "rb"))["tool"]["poetry"]["version"]
         except:
-            from importlib.metadata import version
-            return version(__package__)
+            try:
+                import pkg_resources
+                return pkg_resources.get_distribution("rnsh").version
+            except:
+                return "0.0.0"
+
     except:
         return "0.0.0"
 
 __version__ = _get_version()
```

### Comparing `rnsh-0.0.9/rnsh/args.py` & `rnsh-0.1.0/rnsh/args.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,28 +14,28 @@
     except ValueError:
         return arr, []
 
 
 usage = \
 '''
 Usage:
-    rnsh [--config <configdir>] [-i <identityfile>] [-s <service_name>] [-l] -p
-    rnsh -l [--config <configfile>] [-i <identityfile>] [-s <service_name>] 
-         [-v... | -q...] [-b <period>] (-n | -a <identity_hash> [-a <identity_hash>] ...) 
-         [-A | -C] [[--] <program> [<arg> ...]]
-    rnsh [--config <configfile>] [-i <identityfile>] [-s <service_name>] 
-         [-v... | -q...] [-N] [-m] [-w <timeout>] <destination_hash> 
-         [[--] <program> [<arg> ...]]
+    rnsh -l [-c <configdir>] [-i <identityfile> | -s <service_name>] [-v... | -q...] -p
+    rnsh -l [-c <configdir>] [-i <identityfile> | -s <service_name>] [-v... | -q...] 
+            [-b <period>] (-n | -a <identity_hash> [-a <identity_hash>] ...) [-A | -C] 
+            [[--] <program> [<arg> ...]]
+    rnsh [-c <configdir>] [-i <identityfile>] [-v... | -q...] -p
+    rnsh [-c <configdir>] [-i <identityfile>] [-v... | -q...] [-N] [-m] [-w <timeout>] 
+         <destination_hash> [[--] <program> [<arg> ...]]
     rnsh -h
     rnsh --version
 
 Options:
-    --config DIR                 Alternate Reticulum config directory to use
+    -c DIR --config DIR          Alternate Reticulum config directory to use
     -i FILE --identity FILE      Specific identity file to use
-    -s NAME --service NAME       Listen on/connect to specific service name if not default
+    -s NAME --service NAME       Service name for identity file if not default
     -p --print-identity          Print identity information and exit
     -l --listen                  Listen (server) mode. If supplied, <program> <arg>...will 
                                    be used as the command line when the initiator does not
                                    provide one or when remote command is disabled. If
                                    <program> is not supplied, the default shell of the 
                                    user rnsh is running under will be used.
     -b --announce PERIOD         Announce on startup and every PERIOD seconds
@@ -55,14 +55,15 @@
                                      Listener ->  INFO
                                                   DEBUG    (insane)
     -v --verbose                 Increase verbosity (move level down), multiple increases effect
     --version                    Show version
     -h --help                    Show this help
 '''
 
+DEFAULT_SERVICE_NAME = "default"
 
 class Args:
     def __init__(self, argv: [str]):
         global usage
         try:
             self.argv = argv
             self.program_args = []
@@ -71,17 +72,19 @@
             if next(filter(lambda a: a == "-l" or a == "--listen", self.docopts_argv), None) is not None \
                     and len(self.program_args) > 0:
                 self.docopts_argv.append(self.program_args[0])
                 self.program_args = self.program_args[1:]
     
             args = docopt.docopt(usage, argv=self.docopts_argv[1:], version=f"rnsh {rnsh.__version__}")
             # json.dump(args, sys.stdout)
-    
-            self.service_name = args.get("--service", None) or "default"
+
             self.listen = args.get("--listen", None) or False
+            self.service_name = args.get("--service", None)
+            if self.listen and (self.service_name is None or len(self.service_name) > 0):
+                self.service_name = DEFAULT_SERVICE_NAME
             self.identity = args.get("--identity", None)
             self.config = args.get("--config", None)
             self.print_identity = args.get("--print-identity", None) or False
             self.verbose = args.get("--verbose", None) or 0
             self.quiet = args.get("--quiet", None) or 0
             announce = args.get("--announce", None)
             self.announce = None
@@ -101,14 +104,18 @@
             self.no_id = args.get("--no-id", None) or False
             self.mirror = args.get("--mirror", None) or False
             self.timeout = args.get("--timeout", None) or RNS.Transport.PATH_REQUEST_TIMEOUT
             self.destination = args.get("<destination_hash>", None)
             self.help = args.get("--help", None) or False
             self.command_line = [self.program] if self.program else []
             self.command_line.extend(self.program_args)
+        except docopt.DocoptExit:
+            print()
+            print(usage)
+            sys.exit(1)
         except Exception as e:
             print(f"Error parsing arguments: {e}")
             print()
             print(usage)
             sys.exit(1)
 
         if self.help:
```

### Comparing `rnsh-0.0.9/rnsh/exception.py` & `rnsh-0.1.0/rnsh/exception.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.0.9/rnsh/process.py` & `rnsh-0.1.0/rnsh/process.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.0.9/rnsh/retry.py` & `rnsh-0.1.0/rnsh/retry.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.0.9/rnsh/rnslogging.py` & `rnsh-0.1.0/rnsh/rnslogging.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.0.9/rnsh/session.py` & `rnsh-0.1.0/rnsh/session.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 from abc import abstractmethod, ABC
 from multiprocessing import Manager
 import os
 import RNS
 
 import logging as __logging
 
-from rnsh.protocol import MessageOutletBase, _TReceipt, MessageState
-
 module_logger = __logging.getLogger(__name__)
 
 _TLink = TypeVar("_TLink")
 
 class SEType(enum.IntEnum):
     SE_LINK_CLOSED = 0
 
@@ -40,49 +38,50 @@
     LSSTATE_ERROR      = 5
     LSSTATE_TEARDOWN   = 6
 
 
 _TIdentity = TypeVar("_TIdentity")
 
 
-class LSOutletBase(protocol.MessageOutletBase):
+class LSOutletBase(ABC):
     @abstractmethod
     def set_initiator_identified_callback(self, cb: Callable[[LSOutletBase, _TIdentity], None]):
         raise NotImplemented()
 
     @abstractmethod
     def set_link_closed_callback(self, cb: Callable[[LSOutletBase], None]):
         raise NotImplemented()
 
     @abstractmethod
     def unset_link_closed_callback(self):
         raise NotImplemented()
 
+    @property
     @abstractmethod
-    def teardown(self):
+    def rtt(self):
         raise NotImplemented()
 
     @abstractmethod
-    def __init__(self):
+    def teardown(self):
         raise NotImplemented()
 
 
 class ListenerSession:
     sessions: List[ListenerSession] = []
-    messenger: protocol.Messenger = protocol.Messenger(retry_delay_min=5)
     allowed_identity_hashes: [any] = []
     allow_all: bool = False
     allow_remote_command: bool = False
     default_command: [str] = []
     remote_cmd_as_args = False
 
-    def __init__(self, outlet: LSOutletBase, loop: asyncio.AbstractEventLoop):
+    def __init__(self, outlet: LSOutletBase, channel: RNS.Channel.Channel, loop: asyncio.AbstractEventLoop):
         self._log = module_logger.getChild(self.__class__.__name__)
         self._log.info(f"Session started for {outlet}")
         self.outlet = outlet
+        self.channel = channel
         self.outlet.set_initiator_identified_callback(self._initiator_identified)
         self.outlet.set_link_closed_callback(self._link_closed)
         self.loop = loop
         self.state: LSState = None
         self.remote_identity = None
         self.term: str | None = None
         self.stdin_is_pipe: bool = False
@@ -97,16 +96,21 @@
         self.stdout_buf = bytearray()
         self.stdout_eof_sent = False
         self.stderr_buf = bytearray()
         self.stderr_eof_sent = False
         self.return_code: int | None = None
         self.return_code_sent = False
         self.process: process.CallbackSubprocess | None = None
-        self._set_state(LSState.LSSTATE_WAIT_IDENT)
+        if self.allow_all:
+            self._set_state(LSState.LSSTATE_WAIT_VERS)
+        else:
+            self._set_state(LSState.LSSTATE_WAIT_IDENT)
         self.sessions.append(self)
+        protocol.register_message_types(self.channel)
+        self.channel.add_message_handler(self._handle_message)
 
     def _terminated(self, return_code: int):
         self.return_code = return_code
 
     def _set_state(self, state: LSState, timeout_factor: float = 10.0):
         timeout = max(self.outlet.rtt * timeout_factor, max(self.outlet.rtt * 2, 10)) if timeout_factor is not None else None
         self._log.debug(f"Set state: {state.name}, timeout {timeout}")
@@ -120,16 +124,16 @@
             # self._log.debug("call_inner")
             if delay == 0:
                 func()
             else:
                 self.loop.call_later(delay, func)
         self.loop.call_soon_threadsafe(call_inner)
 
-    def send(self, message: protocol.Message):
-        self.messenger.send(self.outlet, message)
+    def send(self, message: RNS.MessageBase):
+        self.channel.send(message)
 
     def _protocol_error(self, name: str):
         self.terminate(f"Protocol error ({name})")
 
     def _protocol_timeout_error(self, name: str):
         self.terminate(f"Protocol timeout error: {name}")
 
@@ -163,82 +167,87 @@
         outlet.unset_link_closed_callback()
 
         if outlet != self.outlet:
             self._log.debug("Link closed received from incorrect outlet")
             return
 
         self._log.debug(f"link_closed {outlet}")
-        self.messenger.clear_retries(self.outlet)
         self.terminate()
 
     def _initiator_identified(self, outlet, identity):
         if outlet != self.outlet:
             self._log.debug("Identity received from incorrect outlet")
             return
 
         self._log.info(f"initiator_identified {identity} on link {outlet}")
-        if self.state != LSState.LSSTATE_WAIT_IDENT:
+        if self.state not in [LSState.LSSTATE_WAIT_IDENT, LSState.LSSTATE_WAIT_VERS]:
             self._protocol_error(LSState.LSSTATE_WAIT_IDENT.name)
 
         if not self.allow_all and identity.hash not in self.allowed_identity_hashes:
             self.terminate("Identity is not allowed.")
 
         self.remote_identity = identity
-        self.outlet.set_packet_received_callback(self._packet_received)
         self._set_state(LSState.LSSTATE_WAIT_VERS)
 
     @classmethod
-    async def pump_all(cls):
+    async def pump_all(cls) -> True:
+        processed_any = False
         for session in cls.sessions:
-            session.pump()
+            processed = session.pump()
+            processed_any = processed_any or processed
             await asyncio.sleep(0)
 
 
     @classmethod
     async def terminate_all(cls, reason: str):
         for session in cls.sessions:
             session.terminate(reason)
             await asyncio.sleep(0)
 
-    def pump(self):
-
+    def pump(self) -> bool:
         try:
             if self.state != LSState.LSSTATE_RUNNING:
-                return
-            elif not self.messenger.is_outlet_ready(self.outlet):
-                return
+                return False
+            elif not self.channel.is_ready_to_send():
+                return False
             elif len(self.stderr_buf) > 0:
-                mdu = self.outlet.mdu - 16
+                mdu = protocol.StreamDataMessage.MAX_DATA_LEN
                 data = self.stderr_buf[:mdu]
                 self.stderr_buf = self.stderr_buf[mdu:]
                 send_eof = self.process.stderr_eof and len(data) == 0 and not self.stderr_eof_sent
                 self.stderr_eof_sent = self.stderr_eof_sent or send_eof
                 msg = protocol.StreamDataMessage(protocol.StreamDataMessage.STREAM_ID_STDERR,
                                                  data, send_eof)
                 self.send(msg)
                 if send_eof:
                     self.stderr_eof_sent = True
+                return True
             elif len(self.stdout_buf) > 0:
-                mdu = self.outlet.mdu - 16
+                mdu = protocol.StreamDataMessage.MAX_DATA_LEN
                 data = self.stdout_buf[:mdu]
                 self.stdout_buf = self.stdout_buf[mdu:]
                 send_eof = self.process.stdout_eof and len(data) == 0 and not self.stdout_eof_sent
                 self.stdout_eof_sent = self.stdout_eof_sent or send_eof
                 msg = protocol.StreamDataMessage(protocol.StreamDataMessage.STREAM_ID_STDOUT,
                                                  data, send_eof)
                 self.send(msg)
+                if send_eof:
+                    self.stdout_eof_sent = True
+                return True
             elif self.return_code is not None and not self.return_code_sent:
                 msg = protocol.CommandExitedMessage(self.return_code)
                 self.send(msg)
                 self.return_code_sent = True
                 self._call(functools.partial(self._check_protocol_timeout,
                                              lambda: self.state == LSState.LSSTATE_RUNNING, "CommandExitedMessage"),
                            max(self.outlet.rtt * 5, 10))
+                return False
         except Exception as ex:
             self._log.exception("Error during pump", ex)
+        return False
 
     def _terminate_process(self):
         with contextlib.suppress(Exception):
             if self.process and self.process.running:
                 self.process.terminate()
 
     def _start_cmd(self, cmdline: [str], pipe_stdin: bool, pipe_stdout: bool, pipe_stderr: bool, tcflags: [any],
@@ -266,15 +275,16 @@
 
         def stderr(data: bytes):
             self.stderr_buf.extend(data)
 
         try:
             self.process = process.CallbackSubprocess(argv=self.cmdline,
                                                       env={"TERM": self.term or os.environ.get("TERM", None),
-                                                            "RNS_REMOTE_IDENTITY": RNS.prettyhexrep(self.remote_identity.hash) or ""},
+                                                            "RNS_REMOTE_IDENTITY": (RNS.prettyhexrep(self.remote_identity.hash)
+                                                                if self.remote_identity and self.remote_identity.hash else "")},
                                                       loop=self.loop,
                                                       stdout_callback=stdout,
                                                       stderr_callback=stderr,
                                                       terminated_callback=self._terminated,
                                                       stdin_is_pipe=self.stdin_is_pipe,
                                                       stdout_is_pipe=self.stdout_is_pipe,
                                                       stderr_is_pipe=self.stderr_is_pipe)
@@ -294,15 +304,18 @@
 
     def _received_stdin(self, data: bytes, eof: bool):
         if data and len(data) > 0:
             self.process.write(data)
         if eof:
             self.process.close_stdin()
 
-    def _handle_message(self, message: protocol.Message):
+    def _handle_message(self, message: RNS.MessageBase):
+        if self.state == LSState.LSSTATE_WAIT_IDENT:
+            self._protocol_error("Identification required")
+            return
         if self.state == LSState.LSSTATE_WAIT_VERS:
             if not isinstance(message, protocol.VersionInfoMessage):
                 self._protocol_error(self.state.name)
                 return
             self._log.info(f"version {message.sw_version}, protocol {message.protocol_version} on link {self.outlet}")
             if message.protocol_version != protocol.PROTOCOL_VERSION:
                 self.terminate("Incompatible protocol")
@@ -334,25 +347,14 @@
         elif self.state in [LSState.LSSTATE_ERROR, LSState.LSSTATE_TEARDOWN]:
             self._log.error(f"Received packet, but in state {self.state.name}")
             return
         else:
             self._protocol_error("unexpected message")
             return
 
-    def _packet_received(self, outlet: protocol.MessageOutletBase, raw: bytes):
-        if outlet != self.outlet:
-            self._log.debug("Packet received from incorrect outlet")
-            return
-
-        try:
-            message = self.messenger.receive(raw)
-            self._handle_message(message)
-        except Exception as ex:
-            self._protocol_error("unusable packet")
-
 
 class RNSOutlet(LSOutletBase):
 
     def set_initiator_identified_callback(self, cb: Callable[[LSOutletBase, _TIdentity], None]):
         def inner_cb(link, identity: _TIdentity):
             cb(self, identity)
 
@@ -366,58 +368,24 @@
 
     def unset_link_closed_callback(self):
         self.link.set_link_closed_callback(None)
 
     def teardown(self):
         self.link.teardown()
 
-    def send(self, raw: bytes) -> RNS.PacketReceipt:
-        packet = RNS.Packet(self.link, raw)
-        packet.send()
-        return packet.receipt
-
-    @property
-    def mdu(self) -> int:
-        return self.link.MDU
-
     @property
     def rtt(self) -> float:
         return self.link.rtt
 
-    @property
-    def is_usuable(self):
-        return True #self.link.status in [RNS.Link.ACTIVE]
-
-    def get_receipt_state(self, receipt: RNS.PacketReceipt) -> MessageState:
-        status = receipt.get_status()
-        if status == RNS.PacketReceipt.SENT:
-            return protocol.MessageState.MSGSTATE_SENT
-        if status == RNS.PacketReceipt.DELIVERED:
-            return protocol.MessageState.MSGSTATE_DELIVERED
-        if status == RNS.PacketReceipt.FAILED:
-            return protocol.MessageState.MSGSTATE_FAILED
-        else:
-            raise Exception(f"Unexpected receipt state: {status}")
-
-    def timed_out(self):
-        self.link.teardown()
-
     def __str__(self):
         return f"Outlet RNS Link {self.link}"
 
-    def set_packet_received_callback(self, cb: Callable[[MessageOutletBase, bytes], None]):
-        def inner_cb(message, packet: RNS.Packet):
-            packet.prove()
-            cb(self, message)
-
-        self.link.set_packet_callback(inner_cb)
-
     def __init__(self, link: RNS.Link):
         self.link = link
         link.lsoutlet = self
-        link.msgoutlet = self
+
     @staticmethod
     def get_outlet(link: RNS.Link):
         if hasattr(link, "lsoutlet"):
             return link.lsoutlet
 
         return RNSOutlet(link)
```

### Comparing `rnsh-0.0.9/rnsh/testlogging.py` & `rnsh-0.1.0/rnsh/testlogging.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.0.9/setup.py` & `rnsh-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,305 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rnsh
+Version: 0.1.0
+Summary: Shell over Reticulum
+License: MIT
+Author: acehoss
+Author-email: acehoss@acehoss.net
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: docopt (>=0.6.2,<0.7.0)
+Requires-Dist: rns (>=0.5.2,<0.6.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['rnsh']
+# `r n s h`  Shell over Reticulum 
+[![CI](https://github.com/acehoss/rnsh/actions/workflows/python-package.yml/badge.svg)](https://github.com/acehoss/rnsh/actions/workflows/python-package.yml) 
+[![Release](https://github.com/acehoss/rnsh/actions/workflows/python-publish.yml/badge.svg)](https://github.com/acehoss/rnsh/actions/workflows/python-publish.yml) 
+[![PyPI version](https://badge.fury.io/py/rnsh.svg)](https://badge.fury.io/py/rnsh)  
+![PyPI - Downloads](https://img.shields.io/pypi/dw/rnsh?color=informational&label=Installs&logo=pypi)
 
-package_data = \
-{'': ['*']}
+`rnsh` is a utility written in Python that facilitates shell 
+sessions over [Reticulum](https://reticulum.network) networks. 
+It is based on the `rnx` utility that ships with Reticulum and
+aims to provide a similar experience to SSH.
 
-install_requires = \
-['docopt>=0.6.2,<0.7.0', 'rns>=0.4.9,<0.5.0', 'tomli>=2.0.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['rnsh = rnsh.rnsh:rnsh_cli']}
-
-setup_kwargs = {
-    'name': 'rnsh',
-    'version': '0.0.9',
-    'description': 'Shell over Reticulum',
-    'long_description': '# `r n s h` \xa0Shell over Reticulum \n[![CI](https://github.com/acehoss/rnsh/actions/workflows/python-package.yml/badge.svg)](https://github.com/acehoss/rnsh/actions/workflows/python-package.yml)\xa0\n[![Release](https://github.com/acehoss/rnsh/actions/workflows/python-publish.yml/badge.svg)](https://github.com/acehoss/rnsh/actions/workflows/python-publish.yml)\xa0\n[![PyPI version](https://badge.fury.io/py/rnsh.svg)](https://badge.fury.io/py/rnsh) \xa0\n![PyPI - Downloads](https://img.shields.io/pypi/dw/rnsh?color=informational&label=Installs&logo=pypi)\n\n`rnsh` is a utility written in Python that facilitates shell \nsessions over [Reticulum](https://reticulum.network) networks. \nIt is based on the `rnx` utility that ships with Reticulum and\naims to provide a similar experience to SSH.\n\n`rnsh` is still a little raw; there are some things that are \nimplemented badly, and many other things that haven\'t been \nbuilt at all (yet). Signals (i.e. Ctrl-C) need some work, so have\nanother terminal handy to send a SIGTERM if things glitch\nout.\n\nAnyway, there\'s a lot of room for improvement.\n\n## Contents\n\n- [Alpha Disclaimer](#reminder--alpha-software)\n- [Recent Changes](#recent-changes)\n- [Quickstart](#quickstart)\n- [Options](#options)\n- [How it works](#how-it-works)\n- [Roadmap](#roadmap)\n- [Active TODO](#todo)\n\n### Reminder: Alpha Software\nThese early versions will be buggy. There will sometimes be major\nbreaking changes to the command line parameters between releases.\nThere will sometimes be breaking changes in the protocol between\nreleases. Use at your own peril!\n\n## Recent Changes\n### v0.0.8\n- Improved test suite exposed several issues with the handling of\ncommand line arguments which are now fixed\n- Fixed a race condition that would cause remote characters to be \n  lost intermittently when running remote commands that finish\n  immediately.\n- Added automated testing that actually spins up a random listener\n  and initiator in a private Reticulum network and passes data\n  between them, uncovering more issues which are now fixed.\n- Fixed (hopefully) an issue where `rnsh` doesn\'t know what\n  version it is.\n\n### v0.0.7\nAdded `-A` command line option. This listener option causes the\nremote command line to be appended to the arguments list of the\nlaunched program. This allows the listener to jail connections\nto a particular executable while still allowing parameters.\n\n### v0.0.6\nMinor improvements in transport efficiency\n\n### v0.0.5\n#### Remote command line and pipe compatibility\nCommand line options have changed somewhat to allow the initiator\nto supply a command line. This allows `rnsh` to function similarly\nto SSH. You can pipe into or out of `rnsh` to send input through\nremote commands or remote command output through other commands.\n\nThis behavior can be blocked on the listener with the `-C` option.\n\nWhen the initiator does not supply a command, the listener uses\na default command specified on its command line. If a default\ncommand is not specified, the listener falls back to the shell\nof the user it is running under.\n\n## Quickstart\n\nTested (thus far) on Python 3.11 macOS 13.1 ARM64. Should\nrun on Python 3.6+ on Linux or Unix. WSL probably works. \nCygwin might work, too.\n\n- Activate a virtualenv\n- `pip3 install rnsh`\n  - Or from a `whl` release, `pip3 install /path/to/rnsh-0.0.1-py3-none-any.whl`\n- Configure Reticulum interfaces, check with `rnstatus`\n- Ready to run `rnsh`. The options are shown below.\n\n### Example: Shell server\n#### Setup\nBefore running the listener or initiator, you\'ll need to get the \nlistener destination hash and the initiator identity hash.\n```shell\n# On listener\nrnsh -l -p\n\n# On initiator\nrnsh -p\n```\nNote: if you are using a non-default identity or service name, be\nsure to supply these options with `-p` as the identity and \ndestination hashes will change depending on these settings.\n\n#### Listener\n- Listening for default service name ("default").\n- Using user\'s default Reticulum config dir (~/.reticulum).\n- Using default identity ($RNSCONFIGDIR/storage/identities/rnsh).\n- Allowing remote identity `6d47805065fa470852cf1b1ef417a1ac` to connect.\n- Launching `/bin/zsh` on authorized connect.\n```shell\nrnsh -l -a 6d47805065fa470852cf1b1ef417a1ac -- /bin/zsh\n```\n#### Initiator\n- Connecting to default service name ("default").\n- Using user\'s default Reticulum config dir (~/.reticulum).\n- Using default identity ($RNSCONFIGDIR/storage/identities/rnsh).\n- Connecting to destination `a5f72aefc2cb3cdba648f73f77c4e887`\n```shell\nrnsh a5f72aefc2cb3cdba648f73f77c4e887\n```\n\n## Options\n```\nUsage:\n    rnsh [--config <configdir>] [-i <identityfile>] [-s <service_name>] [-l] -p\n    rnsh -l [--config <configfile>] [-i <identityfile>] [-s <service_name>] \n         [-v... | -q...] [-b <period>] (-n | -a <identity_hash> [-a <identity_hash>] ...) \n         [-A | -C] [[--] <program> [<arg> ...]]\n    rnsh [--config <configfile>] [-i <identityfile>] [-s <service_name>] \n         [-v... | -q...] [-N] [-m] [-w <timeout>] <destination_hash> \n         [[--] <program> [<arg> ...]]\n    rnsh -h\n    rnsh --version\n\nOptions:\n    --config DIR                 Alternate Reticulum config directory to use\n    -i FILE --identity FILE      Specific identity file to use\n    -s NAME --service NAME       Listen on/connect to specific service name if not default\n    -p --print-identity          Print identity information and exit\n    -l --listen                  Listen (server) mode. If supplied, <program> <arg>...will \n                                   be used as the command line when the initiator does not\n                                   provide one or when remote command is disabled. If\n                                   <program> is not supplied, the default shell of the \n                                   user rnsh is running under will be used.\n    -b --announce PERIOD         Announce on startup and every PERIOD seconds\n                                 Specify 0 for PERIOD to announce on startup only.\n    -a HASH --allowed HASH       Specify identities allowed to connect\n    -n --no-auth                 Disable authentication\n    -N --no-id                   Disable identify on connect\n    -A --remote-command-as-args  Concatenate remote command to argument list of <program>/shell\n    -C --no-remote-command       Disable executing command line from remote\n    -m --mirror                  Client returns with code of remote process\n    -w TIME --timeout TIME       Specify client connect and request timeout in seconds\n    -q --quiet                   Increase quietness (move level up), multiple increases effect\n                                          DEFAULT LOGGING LEVEL\n                                                  CRITICAL (silent)\n                                    Initiator ->  ERROR\n                                                  WARNING\n                                     Listener ->  INFO\n                                                  DEBUG    (insane)\n    -v --verbose                 Increase verbosity (move level down), multiple increases effect\n    --version                    Show version\n    -h --help                    Show this help\n```\n\n## How it works\n### Listeners\nListener instances are the servers. Each listener is configured \nwith an RNS identity, and a service name. Together, RNS makes\nthese into a destination hash that can be used to connect to\nyour listener.\n   \nMultiple listeners can use the same identity. As long as \nthey are given different service names. They will have \ndifferent destination hashes and not conflict.\n\nListeners must be configured with a command line to run (at \nleast at this time). The identity hash string is set in the\nenvironment variable RNS_REMOTE_IDENTITY for use in child\nprograms.\n\nListeners are set up using the `-l` flag.\n   \n### Initiators\nInitiators are the clients. Each initiator has an identity\nhash which is used as an authentication mechanism on Reticulum.\nYou\'ll need this value to configure the listener to allow \nyour connection. It is possible to run the server without \nauthentication, but hopefully it\'s obvious that this is an\nadvanced use case. \n    \nTo get the identity hash, use the `-p` flag.\n    \nWith the initiator identity set up in the listener command\nline, and with the listener identity copied (you\'ll need to\ndo `-p` on the listener side, too), you can run the\ninitiator.\n    \nI recommend staying pretty vanilla to start with and\ntrying `/bin/zsh` or whatever your favorite shell is these \ndays. The shell should start in login mode. Ideally it\nworks just like an `ssh` shell session.\n\n### Protocol\nThe protocol is build on top of the Reticulum `Request` and\n`Packet` APIs.\n\n- After the initiator identifies on the connection, it enters\n  a request loop. \n- When idle, the initiator will periodically \n  poll the listener. \n- When the initiator has data available (i.e the user typed \n  some characters), the initiator will send that data to the\n  listener in a request, and the listener will respond with \n  any data available from the listener. \n- When the listener has new data available, it notifies the \n  initiator using a notification packet. The initiator then \n  makes a request to the listener to fetch the data.\n   \n## Roadmap\n1. Plan a better roadmap\n2. ?\n3. Keep my day job\n\n## TODO\n- [X] ~~Initial version~~\n- [X] ~~Pip package with command-line utility support~~\n- [X] ~~Publish to PyPI~~\n- [X] ~~Improve signal handling~~\n- [X] ~~Make it scriptable (currently requires a tty)~~\n- [X] ~~Protocol improvements (throughput!)~~\n- [X] ~~Documentation improvements~~\n- [ ] Test on several platforms\n- [ ] Fix issues that come up with testing\n- [ ] Fix issues with running `rnsh` in a binary pipeline, i.e. \n  piping the output of `tar` over `rsh`.\n- [ ] Beta release\n- [ ] Test and fix more issues\n- [ ] V1.0\n- [ ] Enhancement Ideas\n  - [ ] `authorized_keys` mode similar to SSH\n  - [ ] Git over `rnsh` (git remote helper)\n  - [ ] Sliding window acknowledgements for improved throughput\n\n## Miscellaneous\n\nBy piping into/out of `rnsh`, it should be possible to transfer\nfiles using the same method discussed in \n[this article](https://cromwell-intl.com/open-source/tar-and-ssh.html).\nI tested it just now and it doesn\'t work right. There\'s probably some\nsubtle garbling of the data at one end of the stream or the other.\n',
-    'author': 'acehoss',
-    'author_email': 'acehoss@acehoss.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+## Contents
 
+- [Alpha Disclaimer](#reminder--alpha-software)
+- [Recent Changes](#recent-changes)
+- [Quickstart](#quickstart)
+- [Options](#options)
+- [How it works](#how-it-works)
+- [Roadmap](#roadmap)
+- [Active TODO](#todo)
+
+### Reminder: Alpha Software
+These early versions will be buggy. There will sometimes be major
+breaking changes to the command line parameters between releases.
+There will sometimes be breaking changes in the protocol between
+releases. Use at your own peril!
+
+## Recent Changes
+### v0.0.12
+- Remove service name from RNS destination aspects. Service name
+  now selects a suffix for the identity file and should only be
+  supplied on the listener. The initiator only needs the destination
+  hash of the listener to connect.
+- Show a spinner during link establishment on tty sessions
+- Attempt to catch and beautify exceptions on initiator
+
+### v0.0.11
+- Event loop bursting improves throughput and CPU utilization on
+  both listener and initiator.
+- Packet retries use RNS resend feature to prevent duplicate
+  packets.
+
+### v0.0.10
+- Rate limit window change events to prevent saturation of transport
+- Tweaked some loop timers to improve CPU utilization
+
+### v0.0.9
+- Switch to a new packet-based protocol
+- Bug fixes and dependency updates
+
+## Quickstart
+
+Tested (thus far) on Python 3.11 macOS 13.1 ARM64. Should
+run on Python 3.6+ on Linux or Unix. WSL probably works. 
+Cygwin might work, too.
+
+- Activate a virtualenv
+- `pip3 install rnsh`
+  - Or from a `whl` release, `pip3 install /path/to/rnsh-0.0.1-py3-none-any.whl`
+- Configure Reticulum interfaces, check with `rnstatus`
+- Ready to run `rnsh`. The options are shown below.
+
+### Example: Shell server
+#### Setup
+Before running the listener or initiator, you'll need to get the 
+listener destination hash and the initiator identity hash.
+```shell
+# On listener
+rnsh -l -p
+
+# On initiator
+rnsh -p
+```
+Note: service name no longer is supplied on initiator. The destination
+      hash encapsulates this information.
+
+#### Listener
+- Listening for default service name ("default").
+- Using user's default Reticulum config dir (~/.reticulum).
+- Using default identity ($RNSCONFIGDIR/storage/identities/rnsh).
+- Allowing remote identity `6d47805065fa470852cf1b1ef417a1ac` to connect.
+- Launching `/bin/zsh` on authorized connect.
+```shell
+rnsh -l -a 6d47805065fa470852cf1b1ef417a1ac -- /bin/zsh
+```
+#### Initiator
+- Connecting to default service name ("default").
+- Using user's default Reticulum config dir (~/.reticulum).
+- Using default identity ($RNSCONFIGDIR/storage/identities/rnsh).
+- Connecting to destination `a5f72aefc2cb3cdba648f73f77c4e887`
+```shell
+rnsh a5f72aefc2cb3cdba648f73f77c4e887
+```
+
+## Options
+```
+Usage:
+    rnsh -l [-c <configdir>] [-i <identityfile> | -s <service_name>] [-v... | -q...] -p
+    rnsh -l [-c <configdir>] [-i <identityfile> | -s <service_name>] [-v... | -q...] 
+            [-b <period>] (-n | -a <identity_hash> [-a <identity_hash>] ...) [-A | -C] 
+            [[--] <program> [<arg> ...]]
+    rnsh [-c <configdir>] [-i <identityfile>] [-v... | -q...] -p
+    rnsh [-c <configdir>] [-i <identityfile>] [-v... | -q...] [-N] [-m] [-w <timeout>] 
+         <destination_hash> [[--] <program> [<arg> ...]]
+    rnsh -h
+    rnsh --version
+
+Options:
+    -c DIR --config DIR          Alternate Reticulum config directory to use
+    -i FILE --identity FILE      Specific identity file to use
+    -s NAME --service NAME       Service name for identity file if not default
+    -p --print-identity          Print identity information and exit
+    -l --listen                  Listen (server) mode. If supplied, <program> <arg>...will 
+                                   be used as the command line when the initiator does not
+                                   provide one or when remote command is disabled. If
+                                   <program> is not supplied, the default shell of the 
+                                   user rnsh is running under will be used.
+    -b --announce PERIOD         Announce on startup and every PERIOD seconds
+                                 Specify 0 for PERIOD to announce on startup only.
+    -a HASH --allowed HASH       Specify identities allowed to connect
+    -n --no-auth                 Disable authentication
+    -N --no-id                   Disable identify on connect
+    -A --remote-command-as-args  Concatenate remote command to argument list of <program>/shell
+    -C --no-remote-command       Disable executing command line from remote
+    -m --mirror                  Client returns with code of remote process
+    -w TIME --timeout TIME       Specify client connect and request timeout in seconds
+    -q --quiet                   Increase quietness (move level up), multiple increases effect
+                                          DEFAULT LOGGING LEVEL
+                                                  CRITICAL (silent)
+                                    Initiator ->  ERROR
+                                                  WARNING
+                                     Listener ->  INFO
+                                                  DEBUG    (insane)
+    -v --verbose                 Increase verbosity (move level down), multiple increases effect
+    --version                    Show version
+    -h --help                    Show this help
+```
+
+## How it works
+### Listeners
+Listener instances are the servers. Each listener is configured 
+with an RNS identity, and a service name. Together, RNS makes
+these into a destination hash that can be used to connect to
+your listener.
+   
+Each listener must use a unique identity. The `-s` parameter
+can be used to specify a service name, which creates a unique
+identity file.
+
+Listeners can be configured with a command line to run on
+connect. Initiators can supply a command line as well. There 
+are several different options for the way the command line 
+is handled:
+
+- `-C` no initiator command line is allowed; the connection will
+  be terminated if one is supplied.
+- `-A` initiator-supplied command line is appended to listener-
+  configured command line
+- With neither of these options, the listener will use the first 
+  valid command line from this list:
+  1. Initiator-supplied command line
+  2. Listener command line argument
+  3. Default shell of user listener is running under
+
+
+If the `-n` option is not set on the listener, the initiator
+is required to identify before starting a command. The program 
+will be started with the initiator's identity hash string is set 
+in the environment variable `RNS_REMOTE_IDENTITY`.
+
+Listeners are set up using the `-l` flag.
+   
+### Initiators
+Initiators are the clients. Each initiator has an identity
+hash which is used as an authentication mechanism on Reticulum.
+You'll need this value to configure the listener to allow 
+your connection. It is possible to run the server without 
+authentication, but hopefully it's obvious that this is an
+advanced use case. 
+    
+To get the identity hash, use the `-p` flag.
+    
+With the initiator identity set up in the listener command
+line, and with the listener identity copied (you'll need to
+do `-p` on the listener side, too), you can run the
+initiator.
+    
+I recommend staying pretty vanilla to start with and
+trying `/bin/zsh` or whatever your favorite shell is these 
+days. The shell should start in login mode. Ideally it
+works just like an `ssh` shell session.
+
+## Protocol
+The protocol is build on top of the Reticulum `Packet` API.
+Application software sends and receives `Message` objects,
+which are encapsulated by `Packet` objects. Messages are
+(currently) sent one per packet, and only one packet is
+sent at a time (per link). The next packet is not sent until 
+the receiver proves the outstanding packet.
+
+A future update will work to allow a sliding window of
+outstanding packets to improve channel utilization.
+
+### Session Establishment
+1. Initiator establishes link. Listener session enters state 
+   `LSSTATE_WAIT_IDENT`, or `LSSTATE_WAIT_VERS` if running
+   with `--no-auth` option.
+
+2. Initiator identifies on link if not using `--no-id`.
+   - If using `--allowed-hash`, listener validates identity 
+      against configuration and if no match, sends a 
+      protocol error message and tears down link after prune
+      timer.
+3. Initiator transmits a `VersionInformationMessage`, which
+   is evaluated by the server for compatibility. If
+   incompatible, a protocol error is sent. 
+4. Listener responds with a `VersionInfoMessage` and enters 
+   state `LSSTATE_WAIT_CMD`
+5. Initiator evaluates the listener's version information
+   for compatibility and if incompatible, tears down link.
+6. Initiator sends an `ExecuteCommandMessage` (which could 
+   be an empty command) and enters the session event loop.
+7. Listener evaluates the command message against the
+   configured options such as `-A` or `-C` and responds
+   with a protocol error if not allowed.
+8. Listener starts the program. If success, the listener
+   enters the session event loop. If failure, responds
+   with a `CommandExitedMessage`.
+
+### Session Event Loop
+##### Listener state `LSSTATE_RUNNING`
+Process messages received from initiator.
+- `WindowSizeMessage`: set window size on child tty if appropriate
+- `StreamDataMessage`: binary data stream for child process;
+  streams ids 0, 1, 2 = stdin, stdout, stderr
+- `NoopMessage`: no operation - listener replies with `NoopMessage`
+- When link is torn down, child process is terminated if running and 
+  session destroyed
+- If command terminates, a `CommandExitedMessage` is sent and session
+  is pruned after an idle timeout.
+##### Initiator state `ISSTATE_RUNNING`
+Process messages received from listener.
+- `ErrorMessage`: print error, terminate link, and exit
+- `StreamDataMessage`: binary stream information; 
+   streams ids 0, 1, 2 = stdin, stdout, stderr
+- `CommandExitedMessage`: remote command exited
+- If link is torn down unexpectedly, print message and exit
+
+   
+## Roadmap
+1. Plan a better roadmap
+2. ?
+3. Keep my day job
+
+## TODO
+- [X] ~~Initial version~~
+- [X] ~~Pip package with command-line utility support~~
+- [X] ~~Publish to PyPI~~
+- [X] ~~Improve signal handling~~
+- [X] ~~Make it scriptable (currently requires a tty)~~
+- [X] ~~Protocol improvements (throughput!)~~
+- [X] ~~Documentation improvements~~
+- [X] ~~Fix issues with running `rnsh` in a binary pipeline, i.e. 
+  piping the output of `tar` over `rsh`.~~
+- [ ] Test on several platforms
+- [ ] Fix issues that come up with testing
+- [ ] v0.1.0 beta
+- [ ] Test and fix more issues
+- [ ] More betas
+- [ ] Enhancement Ideas
+  - [ ] `authorized_keys` mode similar to SSH to allow one listener
+        process to serve multiple users
+  - [ ] Git over `rnsh` (git remote helper)
+  - [ ] Sliding window acknowledgements for improved throughput
+- [ ] v1.0 someday probably maybe
+
+## Miscellaneous
+
+By piping into/out of `rnsh`, it is possible to transfer
+files using the same method discussed in 
+[this article](https://cromwell-intl.com/open-source/tar-and-ssh.html).
+It's not terribly fast currently, due to the round-trip rule 
+enforced by the protocol. Sliding window acknowledgements will
+speed this up significantly.
 
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

