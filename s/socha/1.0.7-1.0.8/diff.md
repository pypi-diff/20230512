# Comparing `tmp/socha-1.0.7.tar.gz` & `tmp/socha-1.0.8.tar.gz`

## Comparing `socha-1.0.7.tar` & `socha-1.0.8.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 socha-1.0.7/changes.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 socha-1.0.7/requirements.txt
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 socha-1.0.7/start.sh
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 socha-1.0.7/socha/__init__.py
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 socha-1.0.7/socha/starter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/networking/__init__.py
--rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/networking/game_client.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/networking/network_socket.py
--rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/networking/xml_protocol_interface.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/plugin/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/plugin/penguins/__init__.py
--rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/plugin/penguins/board.py
--rw-r--r--   0        0        0     9243 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/plugin/penguins/coordinate.py
--rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/plugin/penguins/game_state.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/plugin/penguins/team.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/protocol/__init__.py
--rw-r--r--   0        0        0    17852 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/protocol/protocol.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/protocol/protocol_packet.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 socha-1.0.7/socha/api/protocol/room_message.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 socha-1.0.7/socha/utils/__init__.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 socha-1.0.7/socha/utils/package_builder.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 socha-1.0.7/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 socha-1.0.7/LICENSE
--rw-r--r--   0        0        0    10021 2020-02-02 00:00:00.000000 socha-1.0.7/README.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 socha-1.0.7/pyproject.toml
--rw-r--r--   0        0        0    10966 2020-02-02 00:00:00.000000 socha-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 socha-1.0.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    15116 2020-02-02 00:00:00.000000 socha-1.0.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 socha-1.0.8/requirements.txt
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 socha-1.0.8/start.sh
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 socha-1.0.8/socha/__init__.py
+-rw-r--r--   0        0        0     7798 2020-02-02 00:00:00.000000 socha-1.0.8/socha/starter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/networking/__init__.py
+-rw-r--r--   0        0        0    13811 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/networking/game_client.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/networking/network_socket.py
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/networking/xml_protocol_interface.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/plugin/penguins/__init__.py
+-rw-r--r--   0        0        0    16025 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/plugin/penguins/board.py
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/plugin/penguins/coordinate.py
+-rw-r--r--   0        0        0     6518 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/plugin/penguins/game_state.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/plugin/penguins/team.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/plugin/penguins/utils.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/protocol/__init__.py
+-rw-r--r--   0        0        0    18778 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/protocol/protocol.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/protocol/protocol_packet.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 socha-1.0.8/socha/api/protocol/room_message.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 socha-1.0.8/socha/utils/__init__.py
+-rw-r--r--   0        0        0     8928 2020-02-02 00:00:00.000000 socha-1.0.8/socha/utils/package_builder.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 socha-1.0.8/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 socha-1.0.8/LICENSE
+-rw-r--r--   0        0        0    10021 2020-02-02 00:00:00.000000 socha-1.0.8/README.md
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 socha-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0    10966 2020-02-02 00:00:00.000000 socha-1.0.8/PKG-INFO
```

### Comparing `socha-1.0.7/start.sh` & `socha-1.0.8/start.sh`

 * *Files identical despite different names*

### Comparing `socha-1.0.7/socha/__init__.py` & `socha-1.0.8/socha/__init__.py`

 * *Files identical despite different names*

### Comparing `socha-1.0.7/socha/starter.py` & `socha-1.0.8/socha/starter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,124 @@
 """
 This is the main entry point for the SoCha application.
 """
 import argparse
 import datetime
+import json
 import logging
+import urllib.request
 
 import pkg_resources
-import urllib.request
-import json
 
 from socha.api.networking.game_client import GameClient, IClientHandler
 from socha.utils.package_builder import SochaPackageBuilder
 
 
 class Starter:
     """
     When this is called, the client will try to connect to the server and join a game.
     When successful, the client will start the loop and call the on_update and calculate_move methods,
     if the server sends updates.
     """
 
     def __init__(self, logic: IClientHandler, host: str = "localhost", port: int = 13050, reservation: str = None,
-                 room_id: str = None, survive: bool = False, auto_reconnect: bool = False,
-                 log: bool = False, verbose: bool = False, build: str = None):
+                 room_id: str = None, password: str = None, survive: bool = False, auto_reconnect: bool = False,
+                 headless: bool = False, log: bool = False, verbose: bool = False, build: str = None,
+                 log_level: int = logging.INFO):
         """
         All these arguments can be overwritten, when parsed via start arguments,
         or you initialize this class with the desired values.
 
-        :param logic: Your logic the client will call, if moves are requested.
-        :param host: The host that the client should connect to.
-        :param port: The port of the host.
-        :param reservation: Reservation code for a prepared game.
-        :param room_id: Room Id the client will try to connect.
-        :param survive: If True the client will keep running, even if the connection to the server is terminated.
-        :param log: If True the client will write a log file to the current directory.
-        :param verbose: Verbose option for logging.
+        Args:
+            logic: Your logic the client will call, if moves are requested.
+            host: The host that the client should connect to.
+            port: The port of the host.
+            reservation: Reservation code for a prepared game.
+            room_id: Room ID the client will try to connect.
+            password: Password for the server for authentication as admin.
+            survive: If True the client keep running, even if the connection to the server is terminated.
+            auto_reconnect: If True the client will try to reconnect to the server, if the connection is lost.
+            headless: If True the client will not use the penguin plugin.
+            log: If True the client write a log file to the current directory.
+            verbose: Verbose option for logging.
+            build: If set, the client will build a zip package with the given name.
         """
+        VERBOSE = 15
+        logging.addLevelName(VERBOSE, "VERBOSE")
+
         args = self._handle_start_args()
 
         self.write_log: bool = args.log or log
         self.verbose = args.verbose or verbose
-        self._setup_debugger(self.verbose)
+        self.log_level = args.log_level or log_level
+        self._setup_debugger(self.verbose, self.log_level)
 
         self.check_socha_version()
 
         self.build: str = args.build or build
         if self.build:
             builder = SochaPackageBuilder(self.build)
             builder.build_package()
             exit(0)
 
         self.host: str = args.host or host
         self.port: int = args.port or port
         self.reservation: str = args.reservation or reservation
         self.room_id: str = args.room or room_id
+        if self.room_id and self.reservation:
+            logging.warning("The room ID is not taken into account because a reservation is available.")
+        self.password: str = args.password or password
+        if self.password and (self.reservation or self.room_id):
+            logging.warning("The password is not taken into account because a reservation or Room ID is available.")
         self.survive: bool = args.survive or survive
         self.auto_reconnect: bool = args.auto_reconnect or auto_reconnect
+        self.headless: bool = args.headless or headless
 
         self.client = GameClient(host=self.host, port=self.port, handler=logic, reservation=self.reservation,
-                                 room_id=room_id, auto_reconnect=self.auto_reconnect, survive=self.survive)
+                                 room_id=room_id, password=self.password, auto_reconnect=self.auto_reconnect,
+                                 survive=self.survive, headless=self.headless)
 
         self.client.join()
 
         self.client.start()
 
-    def _setup_debugger(self, verbose: bool):
+    def _setup_debugger(self, verbose: bool, log_level: int):
         if verbose:
             level: int = logging.DEBUG
         else:
-            level: int = logging.INFO
+            level: int = log_level
 
         if self.write_log:
             now = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
             logging.basicConfig(filename=f"log{now}", level=level,
                                 format="%(asctime)s: %(levelname)s - %(message)s")
             logging.getLogger().addHandler(logging.StreamHandler())
         else:
             logging.basicConfig(level=level, format="%(asctime)s: %(levelname)s - %(message)s")
         logging.info("Starting...")
-        logging.critical("\nDiese Version von SoCha hat einige Änderungen.\n"
-                         "Deshalb wird Code welcher mit 1.0.0 und niedriger geschrieben wurde ein paar Fehler haben.\n"
-                         "Hilfe, um seinen Code anzupassen kann man unter: \n"
-                         "https://github.com/FalconsSky/socha-python-client/blob/master/changes.md\n"
-                         "finden, oder mir eine E-Mail oder Nachricht auf Discord schreiben.")
+        logging.info(
+            "We would greatly appreciate it if you could share any issues "
+            "or feature requests you may have regarding socha by either creating "
+            "an issue on our GitHub repository or contributing to the project."
+            "\n(https://github.com/maxblan/socha-python-client)")
 
     @staticmethod
     def check_socha_version():
         package_name = 'socha'
         try:
             installed_version = pkg_resources.get_distribution(package_name).version
             response = urllib.request.urlopen(f"https://pypi.org/pypi/{package_name}/json")
             json_data = json.loads(response.read())
             latest_version = json_data['info']['version']
             if installed_version != latest_version:
                 logging.warning(
                     f"A newer version ({latest_version}) of {package_name} is available. You have version "
                     f"{installed_version}.")
+            else:
+                logging.info(f"You're running the latest version of {package_name} ({latest_version})")
         except pkg_resources.DistributionNotFound:
             logging.error(f"{package_name} is not installed.")
         except urllib.error.URLError as e:
             logging.warning(
                 f"Could not check the latest version of {package_name} due to {type(e).__name__}: {e}")
 
     @staticmethod
@@ -108,17 +127,22 @@
                                          epilog='Please make sure that the server is already running, '
                                                 'before you start your player.')
         parser.add_argument('--help', action='help', help='Prints this help message.')
         parser.add_argument('-h', '--host', help='The host to connect to. The default is \'localhost\'.')
         parser.add_argument('-p', '--port', help='The port of the host. The default is 13050.', type=int)
         parser.add_argument('-r', '--reservation', help='Reservation code for a prepared game.', type=str)
         parser.add_argument('-R', '--room', help='Room Id the client will try to connect.', type=str)
+        parser.add_argument('-P', '--password', help='Password which will be used to authenticate with the server.',
+                            type=str)
         parser.add_argument('-s', '--survive', action='store_true',
                             help='If present the client will keep running, even if the connection to the server is '
                                  'terminated.')
         parser.add_argument('-l', '--log', action='store_true',
                             help='If present the client will write a log file to the current directory.')
-        parser.add_argument('-v', '--verbose', action='store_true', help='Verbose option for logging.')
+        parser.add_argument('-v', '--verbose', action='store_true', help='Verbose option for logging.  '
+                                                                         'This cancels out the log-level argument.')
+        parser.add_argument('-L', '--log_level', help='Sets the log level.', type=int)
         parser.add_argument('--auto-reconnect', action='store_true',
                             help='Automatically reconnect to the server if the connection is lost.')
+        parser.add_argument('--headless', action='store_true', help='Starts the client without the penguin plugin.')
         parser.add_argument('-b', '--build', help='Builds the this script into a package with all its dependencies.')
         return parser.parse_args()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `socha-1.0.7/socha/api/networking/network_socket.py` & `socha-1.0.8/socha/api/networking/network_socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         Initializes the NetworkSocket object with the specified host, port, and timeout values.
         The socket is not yet connected to a server.
 
         Args:
             host (str): The hostname or IP address of the server to connect to. Defaults to "localhost".
             port (int): The port number to connect to on the server. Defaults to 13050.
             timeout (float): The timeout for socket operations, in seconds. Defaults to 0.1.
-            connected (bool): Whether or not the socket is currently connected to the server.
+            connected (bool): Whether the socket is currently connected to the server.
             socket (socket.socket): The underlying socket object.
             buffer (bytes): A buffer for storing received data.
         """
         self.host = host
         self.port = port
         self.timeout = timeout
         self.connected = False
@@ -56,15 +56,16 @@
         """
         Attempts to receive data from the server. The received data is processed using a regular expression to extract
         complete messages. If a complete message is found, it is returned as bytes and removed from the buffer.
         If no complete message is found, None is returned.
 
         If a timeout occurs or a connection reset error is encountered, the socket is closed and None is returned.
         """
-        regex = re.compile(br"<((room[\s\S]+?</room>)|errorpacket[\s\S]+?</errorpacket>|.*?/>)")
+        regex = re.compile(
+            br"<((room[\s\S]+?</room>)|errorpacket[\s\S]+?</errorpacket>|prepared[\s\S]+?</prepared>|.*?/>)")
         while True:
             try:
                 chunk = self.socket.recv(16129)
             except socket.timeout:
                 chunk = b""
             except ConnectionResetError:
                 self.close()
```

### Comparing `socha-1.0.7/socha/api/networking/xml_protocol_interface.py` & `socha-1.0.8/socha/api/networking/xml_protocol_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
-Here are all incoming byte streams and all outgoing protocol objects handelt.
+Here are all incoming byte streams and all outgoing protocol objects handheld.
 """
 import contextlib
 import logging
 from typing import Iterator, Callable, Any
 
 from xsdata.formats.dataclass.context import XmlContext
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.parsers.config import ParserConfig
 from xsdata.formats.dataclass.parsers.handlers import XmlEventHandler
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
 from socha.api.networking.network_socket import NetworkSocket
-from socha.api.plugin.penguins.team import TeamEnum, Move
+from socha.api.plugin.penguins.team import TeamEnum
 from socha.api.protocol.protocol import *
 
 
-def customClassFactory(clazz, params: dict):
+def custom_class_factory(clazz, params: dict):
     if clazz.__name__ == "Data":
         try:
             params.pop("class_binding")
         except KeyError:
             ...
         if params.get("class_value") == "welcomeMessage":
             welcome_message = WelcomeMessage(Team(name=TeamEnum.ONE if params.get("name") == "ONE" else TeamEnum.TWO,
@@ -55,31 +55,31 @@
     def __init__(self, host: str, port: int):
         self.network_interface = NetworkSocket(host, port)
         self.connect()
         self.running = False
         self.first_time = True
 
         context = XmlContext()
-        deserialize_config = ParserConfig(class_factory=customClassFactory)
+        deserialize_config = ParserConfig(class_factory=custom_class_factory)
         self.deserializer = XmlParser(handler=XmlEventHandler, context=context, config=deserialize_config)
 
         serialize_config = SerializerConfig(pretty_print=True, xml_declaration=False)
         self.serializer = XmlSerializer(config=serialize_config)
 
     def connect(self):
         """
         Creates a TCP connection with the server.
         """
         self.network_interface.connect()
 
     def disconnect(self):
         """
-        Sends a closing xml to the server and closes the connection afterwards.
+        Sends a closing xml to the server and closes the connection afterward.
         """
-        self._send(Close())
+        self.send(Close())
         self.network_interface.close()
 
     def _receive(self):
         """
         Gets a receiving byte stream from the server and deserializes it into an object.
 
         :return: The next object in the stream, or None if the server returns an empty response.
@@ -98,15 +98,15 @@
             self.running = False
             raise
         except Exception as e:
             logging.error("An error occurred while receiving data from the server: %s", e)
             self.running = False
             raise
 
-    def _send(self, obj: ProtocolPacket) -> None:
+    def send(self, obj: ProtocolPacket) -> None:
         """
         Sends an object to the server.
 
         :param obj: The object to send. Must not be `None`.
         """
         if obj is None:
             raise ValueError("Cannot send `None` to server")
@@ -117,40 +117,35 @@
         try:
             self.network_interface.send(shipment)
         except Exception as e:
             logging.exception("Error sending shipment to server: %s", e)
             raise
         else:
             logging.debug("Sent shipment to server: %s", shipment)
+        self.first_time = False
 
     @contextlib.contextmanager
     def _encode_context(self) -> Iterator[Callable[[Any], bytes]]:
         """
         A context manager that yields a function for encoding objects as bytes.
         """
 
         def encode(obj: Any) -> bytes:
             return self._serialize_object(obj)
 
         yield encode
 
-    def _deserialize_object(self, byteStream: bytes) -> ProtocolPacket:
+    def _deserialize_object(self, byte_stream: bytes) -> ProtocolPacket:
         """
         Deserialize a xml byte stream to a ProtocolPacket.
-        :param byteStream: The byte stream to deserialize.
+        :param byte_stream: The byte stream to deserialize.
         :return: The deserialized ProtocolPacket child.
         """
-        return self.deserializer.from_bytes(byteStream)
+        return self.deserializer.from_bytes(byte_stream)
 
     def _serialize_object(self, object_class: object) -> bytes:
         """
         Serialize a ProtocolPacket child to a xml byte stream.
         :param object_class: The ProtocolPacket child to serialize.
         :return: The serialized byte stream.
         """
-        if isinstance(object_class, Move):
-            from_value = From(x=object_class.from_value.x, y=object_class.from_value.y)
-            to_value = To(x=object_class.to_value.x, y=object_class.to_value.y)
-            data = Data(class_value="move", from_value=from_value, to=to_value)
-            return self.serializer.render(data).encode("utf-8")
-
         return self.serializer.render(object_class).encode("utf-8")
```

### Comparing `socha-1.0.7/socha/api/plugin/penguins/board.py` & `socha-1.0.8/socha/api/plugin/penguins/board.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 import _pickle as pickle
+import dataclasses
 import logging
-import warnings
-from typing import List, Union, Optional
+from dataclasses import dataclass
+from itertools import chain, takewhile
+from operator import attrgetter
+from typing import List, Union, Optional, Generator, Iterator
 
 from socha.api.plugin.penguins.coordinate import HexCoordinate, Vector, CartesianCoordinate
 from socha.api.plugin.penguins.team import Penguin, TeamEnum, Move
 
 
+@dataclass(frozen=True, order=True, unsafe_hash=True)
 class Field:
     """
     Represents a field in the game.
     """
 
-    def __init__(self, coordinate: HexCoordinate, penguin: Optional[Penguin], fish: int):
-        """
-        The Field represents a field on the game board.
-        It says what state itself it has and where it is on the board.
-
-        Args:
-            coordinate:
-            penguin:
-            fish:
-        """
-        self.coordinate = coordinate
-        self.penguin = penguin
-        self.fish = fish
+    coordinate: HexCoordinate
+    penguin: Optional[Penguin]
+    fish: int
 
     def is_empty(self) -> bool:
         """
         :return: True if the field is has no fishes and no penguin, False otherwise.
         """
         return True if not self.penguin and self.fish == 0 else False
 
@@ -80,46 +74,28 @@
             destination: The destination coordinate.
 
         Returns:
             Vector: The direction of the move.
         """
         return destination.subtract_vector(self.coordinate.to_vector()).to_vector()
 
-    def __eq__(self, other):
-        if isinstance(other, self.__class__):
-            return self.coordinate == other.coordinate and self.penguin == other.penguin and self.fish == other.fish
-        return False
-
-    def __repr__(self):
-        return f"Field({self.coordinate}, {self.penguin}, Fish({self.fish}))"
-
 
+@dataclass(frozen=True, order=True, unsafe_hash=True)
 class Board:
     """
     Class which represents a game board. Consisting of a two-dimensional array of fields.
     """
 
-    def __init__(self, board: List[List[Field]]):
-        """
-        The Board shows the state where each field is, how many fish and which team is on each field.
-
-        :param board: The game field as a two-dimensional array of fields.
-        """
-        self.board = board
+    board: List[List[Field]]
 
     def get_empty_fields(self) -> List[Field]:
         """
         :return: A list of all empty fields.
         """
-        fields: List[Field] = []
-        for row in self.board:
-            for field in row:
-                if field.is_empty():
-                    fields.append(field)
-        return fields
+        return list(filter(lambda field: field.is_empty(), chain(*self.board)))
 
     def is_occupied(self, coordinates: HexCoordinate) -> bool:
         """
         :param coordinates: The coordinates of the field.
         :return: True if the field is occupied, false otherwise.
         """
         return self.get_field(coordinates).is_occupied()
@@ -127,16 +103,16 @@
     def is_valid(self, coordinates: HexCoordinate) -> bool:
         """
         Checks if the coordinates are in the boundaries of the board.
 
         :param coordinates: The coordinates of the field.
         :return: True if the field is valid, false otherwise.
         """
-        arrayCoordinates = coordinates.to_cartesian()
-        return 0 <= arrayCoordinates.x < self.width() and 0 <= arrayCoordinates.y < self.height()
+        array_coordinates = coordinates.to_cartesian()
+        return 0 <= array_coordinates.x < self.width() and 0 <= array_coordinates.y < self.height()
 
     def width(self) -> int:
         """
         :return: The width of the board.
         """
         return len(self.board[0])
 
@@ -175,17 +151,15 @@
         """
         Gets the field at the given position no matter if it is valid or not.
 
         :param position: The position of the field.
         :return: The field at the given position, or None if the position is not valid.
         """
         cartesian = position.to_cartesian()
-        if self.is_valid(position):
-            return self._get_field(cartesian.x, cartesian.y)
-        return None
+        return self._get_field(cartesian.x, cartesian.y) if self.is_valid(position) else None
 
     def get_field_by_index(self, index: int) -> Field:
         """
         Gets the field at the given index. The index is the position of the field in the board.
         The field of the board is calculated as follows:
 
         - `x = index / width`
@@ -207,15 +181,15 @@
         return [field for row in self.board for field in row]
 
     def compare_to(self, other: 'Board') -> List[Field]:
         """
         Compares two boards and returns a list of the Fields that are different.
 
         :param other: The other board to compare to.
-        :return: A list of Fields that are different or a empty list if the boards are equal.
+        :return: A list of Fields that are different or an empty list if the boards are equal.
         """
         if not isinstance(other, Board):
             raise TypeError("Can only compare to another Board object")
 
         fields = [self.board[x][y] for x in range(len(self.board)) for y in range(len(self.board[0]))
                   if self.board[x][y] != other.board[x][y]]
         return fields
@@ -223,66 +197,70 @@
     def contains(self, field: Field) -> bool:
         """
         Checks if the board contains the given field.
 
         :param field: The field to check for.
         :return: True if the board contains the field, False otherwise.
         """
-        for row in self.board:
-            if field in row:
-                return True
-        return False
+        return any(field in row for row in self.board)
 
     def contains_all(self, fields: List[Field]) -> bool:
         """
         Checks if the board contains all the given fields.
 
         :param fields: The fields to check for.
         :return: True if the board contains all the given fields, False otherwise.
         """
         if not fields:
             return False
 
-        for field in fields:
-            if not self.contains(field):
-                return False
-        return True
+        return all(self.contains(field) for field in fields)
 
     def get_moves_in_direction(self, origin: HexCoordinate, direction: Vector, team_enum: Optional[TeamEnum] = None) \
             -> List[Move]:
         """
         Gets all moves in the given direction from the given origin.
-
         Args:
             origin: The origin of the move.
             direction: The direction of the move.
             team_enum: Team to make moves for.
-
         Returns:
                 List[Move]: List of moves that can be made in the given direction from the given index,
                             for the given team_enum
         """
-        if team_enum is None:
-            team_enum = self.get_field(origin).penguin.team_enum
+        team_enum = team_enum or self.get_field(origin).penguin.team_enum
         if not self.get_field(origin).penguin or self.get_field(origin).penguin.team_enum != team_enum:
             return []
 
-        moves = []
-        for i in range(1, self.width()):
+        def valid_destination(i):
             destination = origin.add_vector(direction.scalar_product(i))
-            if self._is_destination_valid(destination):
-                moves.append(Move(team_enum=team_enum, from_value=origin, to_value=destination))
-            else:
-                break
+            return self.is_destination_valid(destination)
+
+        moves = [Move(team_enum=team_enum, from_value=origin, to_value=origin.add_vector(direction.scalar_product(i)))
+                 for i in takewhile(valid_destination, range(1, self.width()))]
+
         return moves
 
-    def _is_destination_valid(self, field: HexCoordinate) -> bool:
+    def is_destination_valid(self, field: HexCoordinate) -> bool:
+        """
+        Checks if the given field is a valid destination for a move.
+        It checks if the destination is on the board, if it is not occupied and if it is not empty.
+
+        Args:
+            field: The field to check for.
+
+        Returns:
+            bool: True if the field is a valid destination, False otherwise.
+        """
         return self.is_valid(field) and not self.is_occupied(field) and not \
             self.get_field(field).is_empty()
 
+    def _is_destination_valid(self, field: HexCoordinate) -> bool:
+        return self.is_destination_valid(field)
+
     def possible_moves_from(self, position: HexCoordinate, team_enum: Optional[TeamEnum] = None) -> List[Move]:
         """
         Returns a list of all possible moves from the given position. That are all moves in all hexagonal directions.
 
         Args:
             position: The position to start from.
             team_enum: A list of all possible moves from the given position.
@@ -312,34 +290,27 @@
     def get_teams_penguins(self, team: TeamEnum) -> List[Penguin]:
         """
         Searches the board for all penguins of the given team_enum.
 
         :param team: The team_enum to search for.
         :return: A list of all coordinates that are occupied by a penguin of the given team_enum.
         """
-        penguins = []
-        for row in self.board:
-            for field in row:
-                if field.penguin and field.penguin.team_enum == team:
-                    penguins.append(field.penguin)
-        return penguins
+        penguins = filter(lambda field: field.penguin and field.penguin.team_enum == team,
+                          (field for row in self.board for field in row))
+        return list(map(attrgetter('penguin'), penguins))
 
     def get_most_fish(self) -> List[Field]:
         """
         Returns a list of all fields with the most fish.
 
         :return: A list of Fields.
         """
-
-        fields = list(filter(lambda field_x: not field_x.is_occupied(), self.get_all_fields()))
-        fields.sort(key=lambda field_x: field_x.get_fish(), reverse=True)
-        for i, field in enumerate(fields):
-            if field.get_fish() < fields[0].get_fish():
-                fields = fields[:i]
-        return fields
+        fields = [field for field in self.get_all_fields() if not field.is_occupied()]
+        max_fish = max(fields, key=lambda field: field.get_fish()).get_fish()
+        return list(filter(lambda field: field.get_fish() == max_fish, fields))
 
     def get_board_intersection(self, other: 'Board') -> List[Field]:
         """
         Returns a list of all fields that are in both boards.
 
         :param other: The other board to compare to.
         :return: A list of Fields.
@@ -351,57 +322,91 @@
         Returns a list of all fields that are in both list of Fields.
 
         :param other: The other list of Fields to compare to.
         :return: A list of Fields.
         """
         return [field for field in self.get_all_fields() if field in other]
 
-    def _move(self, move: Move) -> 'Board':
-        warnings.warn("'_move' is deprecated and will be removed in a future version. Use 'move' instead.",
-                      DeprecationWarning)
-        return self.move(move)
+    def get_neighbor_fields(self, field: Field) -> Iterator[Field]:
+        """
+        Returns a generator of all neighbor fields of the given field.
+
+        Args:
+            field: The field to get the neighbors of.
+
+        Returns:
+            Generator[Field, None, None]: A generator of all neighbor fields of the given field.
+        """
+        return (self.get_field(each) for each in field.coordinate.get_neighbors() if self.is_valid(each))
+
+    def get_neighbor_fields_coordinate(self, coordinate: HexCoordinate) -> Iterator[Field]:
+        """
+        Returns a generator of all neighbor fields of the given coordinate.
+
+        Args:
+            coordinate: The coordinate to get the neighbors of.
+
+        Returns:
+            Generator[Field, None, None]: A generator of all neighbor fields of the given coordinate.
+        """
+        return (self.get_field(each) for each in coordinate.get_neighbors() if self.is_valid(each))
+
+    def get_valid_neighbor_fields(self, field: Field) -> Iterator[Field]:
+        """
+        Returns a generator of all neighbor fields of the given field.
+
+        Args:
+            field: The field to get the neighbors of.
+
+        Returns:
+            Generator[Field, None, None]: A generator of all neighbor fields of the given field.
+        """
+        return (self.get_field(each) for each in field.coordinate.get_neighbors() if self.is_destination_valid(each))
+
+    def get_valid_neighbor_fields_coordinate(self, coordinate: HexCoordinate) -> Iterator[Field]:
+        """
+        Returns a generator of all neighbor fields of the given coordinate.
+
+        Args:
+            coordinate: The coordinate to get the neighbors of.
+
+        Returns:
+            Generator[Field, None, None]: A generator of all neighbor fields of the given coordinate.
+        """
+        return (self.get_field(each) for each in coordinate.get_neighbors() if self.is_destination_valid(each))
 
     def move(self, move: Move) -> 'Board':
         """
         Moves the penguin from the origin to the destination.
         **Please make sure that the move is correct, because this method will not check that.**
         If there is no Penguin to move, than this method will return the current state unchanged.
 
         :param move: The move to execute.
         :return: The new board with the moved penguin.
         """
         board_state = pickle.loads(pickle.dumps(self.board, protocol=-1))
-        updated_board = Board(board_state)
         moving_penguin = Penguin(team_enum=move.team_enum, coordinate=move.to_value)
         if move.from_value:
             if not self.get_field(move.from_value).penguin:
                 logging.error(f"There is no penguin to move. Origin was: {self.get_field(move.from_value)}")
                 return self
             origin_field_coordinate = move.from_value.to_cartesian()
             moving_penguin = board_state[origin_field_coordinate.y][origin_field_coordinate.x].penguin
-            moving_penguin.coordinate = move.to_value
+            moving_penguin = dataclasses.replace(moving_penguin, coordinate=move.to_value)
             board_state[origin_field_coordinate.y][origin_field_coordinate.x] = Field(coordinate=move.from_value,
                                                                                       penguin=None, fish=0)
-        destination_field = updated_board.get_field(move.to_value)
-        destination_field.penguin = moving_penguin
-        destination_field.fish = 0
-        return updated_board
+
+        destination_field = Field(coordinate=move.to_value, penguin=moving_penguin, fish=0)
+        board_state[move.to_value.to_cartesian().y][move.to_value.to_cartesian().x] = destination_field
+        return Board(board_state)
 
     def pretty_print(self):
         print()
         for i, row in enumerate(self.board):
+            row_str = ""
             if (i + 1) % 2 == 0:
-                print(" ", end="")
-            for field in row:
-                if field.is_empty():
-                    print("~", end=" ")
-                elif field.is_occupied():
-                    print(field.get_team().value[0], end=" ")
-                else:
-                    print(field.get_fish(), end=" ")
-            print()
+                row_str += " "
+            row_str += " ".join(["~" if field.is_empty() else field.get_team().value[0] if field.is_occupied() else str(
+                field.get_fish())
+                                 for field in row])
+            print(row_str)
         print()
-
-    def __eq__(self, other):
-        if isinstance(other, self.__class__):
-            return self.board == other.board
-        return False
```

### Comparing `socha-1.0.7/socha/api/plugin/penguins/coordinate.py` & `socha-1.0.8/socha/api/plugin/penguins/coordinate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 import math
+from dataclasses import dataclass
 from typing import List, Optional
 
 
+@dataclass(frozen=True, order=True, unsafe_hash=True)
 class Vector:
     """
     Represents a vector in the hexagonal grid. It can calculate various vector operations.
     """
-
-    def __init__(self, d_x: int = 0, d_y: int = 0):
-        """
-        Constructor for the Vector class.
-
-        :param d_x: The x-coordinate of the vector.
-        :param d_y: The y-coordinate of the vector.
-        """
-        self.d_x = d_x
-        self.d_y = d_y
+    d_x: int = 0
+    d_y: int = 0
 
     def magnitude(self) -> float:
         """
         Calculates the length of the vector.
 
         :return: The length of the vector.
         """
@@ -116,38 +110,19 @@
         """
         Checks if the vector points to a hexagonal field that is a direct neighbor.
 
         :return: True if the vector is a one hex move, false otherwise.
         """
         return abs(self.d_x) == abs(self.d_y) or (self.d_x % 2 == 0 and self.d_y == 0)
 
-    def __repr__(self) -> str:
-        """
-        Returns the string representation of the vector.
-
-        :return: The string representation of the vector.
-        """
-        return f"Vector({self.d_x}, {self.d_y})"
-
-    def __eq__(self, other):
-        """
-        Overrides the default equality operator to check if two Vector objects are equal.
-
-        :param other: The other Vector object to compare to.
-        :return: True if the two Vector objects are equal, False otherwise.
-        """
-        if isinstance(other, Vector):
-            return self.d_x == other.d_x and self.d_y == other.d_y
-        return False
-
 
+@dataclass(frozen=True, order=True, unsafe_hash=True)
 class Coordinate:
-    def __init__(self, x: int, y: int):
-        self.x = x
-        self.y = y
+    x: int
+    y: int
 
     def to_vector(self) -> Vector:
         """
         Converts the coordinate to a vector.
         """
         return Vector(d_x=self.x, d_y=self.y)
 
@@ -161,14 +136,15 @@
         return self.to_vector().subtraction(other.to_vector()).magnitude()
 
     def add_vector(self, vector: Vector): ...
 
     def subtract_vector(self, vector: Vector): ...
 
 
+@dataclass(frozen=True, order=True, unsafe_hash=True)
 class CartesianCoordinate(Coordinate):
     """
     Represents a coordinate in a normal cartesian coordinate system, that has been taught in school.
     This class is used to translate and represent a hexagonal coordinate in a cartesian and with that a 2D-Array.
     """
 
     def add_vector(self, vector: Vector) -> 'CartesianCoordinate':
@@ -225,21 +201,16 @@
         """
         if index < 0 or index >= width * height:
             raise IndexError(f"Index out of range. The index has to be 0 <= {index} < {width * height}")
         x = index % width
         y = index // width
         return CartesianCoordinate(x, y)
 
-    def __repr__(self) -> str:
-        return f"CartesianCoordinate({self.x}, {self.y})"
-
-    def __eq__(self, other: object) -> bool:
-        return isinstance(other, CartesianCoordinate) and self.x == other.x and self.y == other.y
-
 
+@dataclass(frozen=True, order=True, unsafe_hash=True)
 class HexCoordinate(Coordinate):
     """
     Represents a coordinate in a hexagonal coordinate system, that differs from the normal cartesian one.
     This class is used to represent the hexagonal game board.
     """
 
     def to_cartesian(self) -> CartesianCoordinate:
@@ -273,13 +244,7 @@
     def get_neighbors(self) -> List['HexCoordinate']:
         """
         Returns a list of all neighbors of the hex coordinate.
 
         :return: The list of neighbors.
         """
         return [self.add_vector(vector) for vector in self.to_vector().directions]
-
-    def __repr__(self) -> str:
-        return f"HexCoordinate({self.x}, {self.y})"
-
-    def __eq__(self, other: object) -> bool:
-        return isinstance(other, HexCoordinate) and self.x == other.x and self.y == other.y
```

### Comparing `socha-1.0.7/socha/api/plugin/penguins/game_state.py` & `socha-1.0.8/socha/api/plugin/penguins/game_state.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import _pickle as pickle
 import logging
 from dataclasses import dataclass
 from typing import List, Optional
 
 from socha.api.plugin.penguins.board import Board
 from socha.api.plugin.penguins.coordinate import CartesianCoordinate
-from socha.api.plugin.penguins.team import TeamEnum, Team, Move
+from socha.api.plugin.penguins.team import TeamEnum, Team, Move, Penguin
 
 
+@dataclass(frozen=True, order=True, unsafe_hash=True)
 class GameState:
     """
        A `GameState` contains all information, that describes the game state at a given time, that is, between two game
        moves.
 
        This includes:
             - the board
@@ -27,30 +28,23 @@
             - a method to calculate available moves
             - a method to perform a move for simulating future game states
 
        The game server sends a new copy of the `GameState` to both participating players after each completed move,
        describing the then current state.
        """
 
-    def __init__(self, board: Board, turn: int, first_team: Team, second_team: Team, last_move: Optional[Move]):
-        """
-        Creates a new `GameState` with the given parameters.
+    board: Board
+    turn: int
+    first_team: Team
+    second_team: Team
+    last_move: Optional[Move]
 
-        Args:
-            board: The board of the game.
-            turn: The turn number of the game.
-            first_team: The team_enum that has the first turn.
-            second_team: The team_enum that has the second turn.
-            last_move: The last move made.
-        """
-        self.board = board
-        self.turn = turn
-        self.first_team = first_team
-        self.second_team = second_team
-        self.last_move = last_move
+    @property
+    def possible_moves(self):
+        return self._get_possible_moves(self.current_team)
 
     @property
     def round(self):
         return int((self.turn + 1) / 2)
 
     @property
     def current_team(self):
@@ -60,44 +54,39 @@
     def other_team(self):
         return self.current_team.opponent
 
     @property
     def current_pieces(self):
         return self.current_team.get_penguins()
 
-    @property
-    def possible_moves(self):
-        return self._get_possible_moves(self.current_team)
-
     def _get_possible_moves(self, current_team: Optional[Team]) -> List[Move]:
         """
         Gets all possible moves for the current team.
         That includes all possible moves from all Fields that are not occupied by a penguin from that team.
 
         :param current_team: The team to get the possible moves for.
         :return: A list of all possible moves from the current player's turn.
         """
         current_team = current_team or self.current_team
-        moves = []
-
         if not current_team:
-            return moves
+            return []
 
-        if len(self.board.get_teams_penguins(current_team.name)) < 4:
-            for x in range(self.board.width()):
-                for y in range(self.board.height()):
-                    field = self.board.get_field(CartesianCoordinate(x, y).to_hex())
-                    if not field.is_occupied() and field.get_fish() == 1:
-                        moves.append(
-                            Move(team_enum=current_team.name, from_value=None,
-                                 to_value=CartesianCoordinate(x, y).to_hex()))
+        if self.turn < 8:
+            moves = [(x, y) for x in range(self.board.width()) for y in range(self.board.height())]
+            moves = filter(lambda pos: not self.board.get_field(
+                CartesianCoordinate(*pos).to_hex()).is_occupied() and self.board.get_field(
+                CartesianCoordinate(*pos).to_hex()).get_fish() == 1, moves)
+            moves = map(lambda pos: Move(team_enum=current_team.name, from_value=None,
+                                         to_value=CartesianCoordinate(*pos).to_hex()), moves)
+            return list(moves)
         else:
-            for piece in self.board.get_teams_penguins(current_team.name):
-                moves.extend(self.board.possible_moves_from(piece.coordinate, current_team.name))
-        return moves
+            pieces = self.board.get_teams_penguins(current_team.name)
+            moves = map(lambda piece: self.board.possible_moves_from(piece.coordinate, current_team.name), pieces)
+            moves = [item for sublist in moves for item in sublist]
+            return moves
 
     def current_team_from_turn(self, turn: int) -> Team:
         """
         Calculates the current team from the turn number and available moves.
 
         :return: The team that has the current turn.
         """
@@ -119,45 +108,41 @@
             GameState: The new state of the game after the move.
         """
         if self.is_valid_move(move) and self.current_team.name == move.team_enum:
             new_board = self.board.move(move)
             new_first_team: Team = pickle.loads(pickle.dumps(self.first_team, protocol=-1))
             new_second_team: Team = pickle.loads(pickle.dumps(self.second_team, protocol=-1))
             if self.current_team.name == TeamEnum.ONE:
-                self._update_team(new_first_team, move, new_board)
+                new_first_team = self._update_team(new_first_team, move, new_board)
             else:
-                self._update_team(new_second_team, move, new_board)
+                new_second_team = self._update_team(new_second_team, move, new_board)
             new_first_team.opponent = new_second_team
             new_second_team.opponent = new_first_team
             new_turn = self.turn + 1
             new_last_move = move
             return GameState(board=new_board, turn=new_turn, first_team=new_first_team, second_team=new_second_team,
                              last_move=new_last_move)
         else:
             logging.error(f"Performed invalid move while simulating: {move}")
             raise ValueError(f"Invalid move attempted: {move}")
 
-    def _update_team(self, team: Team, move: Move, new_board: Board) -> None:
+    def _update_team(self, team: Team, move: Move, new_board: Board) -> Team:
         """
         Helper function to update the given team when a move is performed.
 
         Args:
             team: The team that will be updated.
             move: The move that was performed.
             new_board: The updated board.
         """
-        team.moves.append(move)
-        adding_fish = self.board.get_field(move.to_value).get_fish()
-        new_penguin = new_board.get_field(move.to_value).penguin
-        teams_penguin = next(filter(lambda x: x.coordinate == move.from_value, team.penguins), None)
-        if teams_penguin:
-            teams_penguin.coordinate = new_penguin.coordinate
-        else:
-            team.penguins.append(new_penguin)
-        team.fish += adding_fish
+        new_moves: List[Move] = team.moves + [move]
+        new_fish: int = team.fish + self.board.get_field(move.to_value).get_fish()
+        new_penguins: List[Penguin] = list(filter(lambda x: x.coordinate != move.from_value, team.penguins)) + [
+            new_board.get_field(move.to_value).penguin]
+        return Team(name=team.name, fish=new_fish, penguins=new_penguins, moves=new_moves, opponent=team.opponent)
 
     def is_valid_move(self, move: Move) -> bool:
         """
         Checks if the given move is valid.
 
         :param move: The move to check.
         :return: True if the move is valid, False otherwise.
@@ -169,11 +154,7 @@
         Returns the opponent team of the current team.
 
         Returns:
             Team: The team which is the opponent of the current team.
         """
         team = team or self.current_team
         return team.opponent
-
-    def __repr__(self):
-        return f"GameState(turn={self.turn}, round={self.round}, first_team={self.first_team}, " \
-               f"second_team={self.second_team}, last_move={self.last_move}, current_team={self.current_team})"
```

### Comparing `socha-1.0.7/socha/api/plugin/penguins/team.py` & `socha-1.0.8/socha/api/plugin/penguins/team.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,28 @@
+from dataclasses import dataclass
 from enum import Enum
 from typing import List, Optional
 
 from socha.api.plugin.penguins.coordinate import HexCoordinate, Vector
 
 
 class TeamEnum(Enum):
     ONE = "ONE"
     TWO = "TWO"
 
 
+@dataclass(frozen=True, order=True, unsafe_hash=True)
 class Move:
     """
     Represents a move in the game.
     """
 
-    def __init__(self, team_enum: TeamEnum, to_value: HexCoordinate, from_value: Optional[HexCoordinate]):
-        """
-        Args:
-            team_enum: The team_enum that performs the move.
-            to_value: The destination of the move.
-            from_value: The origin of the move.
-        """
-        self.team_enum = team_enum
-        self.from_value = from_value
-        self.to_value = to_value
+    team_enum: TeamEnum
+    from_value: Optional[HexCoordinate]
+    to_value: HexCoordinate
 
     def get_delta(self) -> float:
         """
         This method calculates and returns the difference in distance between the to_value and from_value properties
         of the Move object. If the from_value is not initialized, the distance is calculated between the to_value and
         itself.
 
@@ -41,35 +36,23 @@
         If the current Move object is not initialized with a from_value, the method returns the current object.
 
         :return: The reversed move or the current move.
         """
         return self if not self.from_value else Move(team_enum=self.team_enum, to_value=self.from_value,
                                                      from_value=self.to_value)
 
-    def __repr__(self):
-        return f"Move(team={self.team_enum.value}, from={self.from_value}, to={self.to_value})"
-
-    def __eq__(self, __o: object) -> bool:
-        return isinstance(__o, Move) and self.to_value == __o.to_value and \
-               (self.from_value is None or self.from_value == __o.from_value)
-
 
+@dataclass(frozen=True, order=True, unsafe_hash=True)
 class Penguin:
     """
        The Penguin class represents a penguin object with a coordinate and a team_enum.
     """
 
-    def __init__(self, coordinate: HexCoordinate, team_enum: TeamEnum):
-        """
-        Args:
-           coordinate (HexCoordinate): The coordinate of the penguin on the game board.
-           team_enum (TeamEnum): The team_enum that the penguin belongs to.
-        """
-        self.coordinate = coordinate
-        self.team_enum = team_enum
+    coordinate: HexCoordinate
+    team_enum: TeamEnum
 
     def get_distance(self, destination: HexCoordinate) -> float:
         """
         Calculates the distance from the current position to the given destination.
 
         Args:
             destination: The destination to calculate the distance to.
@@ -87,36 +70,27 @@
             destination: The destination coordinate.
 
         Returns:
             Vector: The direction of the move.
         """
         return destination.subtract_vector(self.coordinate.to_vector()).to_vector()
 
-    def __eq__(self, other):
-        if not isinstance(other, Penguin):
-            return False
-        return self.coordinate == other.coordinate and self.team_enum == other.team_enum
-
-    def __repr__(self):
-        return f'Penguin({self.coordinate}, {self.team_enum.value})'
-
 
+@dataclass(order=True, unsafe_hash=True)
 class Team:
     """
     The Team class is useful for storing and manipulating information about teams in the game. It allows you to
     easily create objects for each team_enum, keep track of their attributes, and compare them to their opponents.
     """
 
-    def __init__(self, name: TeamEnum, fish: int, penguins: List[Penguin], moves: List[Move],
-                 opponent: Optional['Team'] = None):
-        self.name = name
-        self.fish = fish
-        self.penguins = penguins
-        self.moves = moves
-        self.opponent = opponent
+    name: TeamEnum
+    fish: int
+    penguins: List[Penguin]
+    moves: List[Move]
+    opponent: Optional['Team'] = None
 
     def team(self) -> TeamEnum:
         """
         :return: The team_enum object.
         """
         return self.name
 
@@ -132,14 +106,9 @@
         """
         if self.name == TeamEnum.ONE:
             return TeamEnum.ONE.value
         else:
             return TeamEnum.TWO.value
 
     def __repr__(self) -> str:
-        return f"Team(name={self.name}, fish={self.fish}, penguins={len(self.penguins)}, moves={len(self.moves)})"
-
-    def __eq__(self, other):
-        if isinstance(other, self.__class__):
-            return self.name == other.name and self.fish == other.fish and self.penguins == other.penguins and \
-                   self.moves == other.moves
-        return False
+        return f'Team(name={self.name.value}, fish={self.fish}, penguins={len(self.penguins)}, ' \
+               f'moves={len(self.moves)}, opponent={None if not self.opponent else self.opponent.name})'
```

### Comparing `socha-1.0.7/socha/api/protocol/protocol.py` & `socha-1.0.8/socha/api/protocol/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         }
     )
 
 
 @dataclass
 class Left(ProtocolPacket):
     """
-    If the game is over the server will _send this message to the clients and closes the connection afterwards.
+    If the game is over the server will _send this message to the clients and closes the connection afterward.
     """
 
     class Meta:
         name = "left"
 
     room_id: Optional[str] = field(
         default=None,
@@ -119,15 +119,15 @@
             "name": "roomId",
             "type": "Attribute",
         }
     )
 
 
 @dataclass
-class JoinedGameRoom(ResponsePacket):
+class JoinedGameRoom(ObservableRoomMessage):
     """
     Sent to all administrative clients after a player joined a GameRoom via a JoinRoomRequest.
     """
 
     class Meta:
         name = "joinedGameRoom"
 
@@ -186,15 +186,15 @@
         metadata={
             "type": "Attribute",
         }
     )
 
 
 @dataclass
-class Slot(ProtocolPacket):
+class Slot(RoomOrchestrationMessage):
     """
     Slots for a game which contains the player's name and its attributes.
     """
 
     class Meta:
         name = "slot"
 
@@ -217,15 +217,15 @@
         metadata={
             "type": "Attribute",
         }
     )
 
 
 @dataclass
-class Step(AdminLobbyRequest):
+class Step(RoomOrchestrationMessage):
     """
     When the client is authenticated as administrator,
     it can _send this step request to the server to advance the game for one move.
     This is not possible if the game is not paused.
     """
 
     class Meta:
@@ -237,15 +237,15 @@
             "name": "roomId",
             "type": "Attribute",
         }
     )
 
 
 @dataclass
-class Prepare(AdminLobbyRequest):
+class Prepare(RoomOrchestrationMessage):
     """
     When the client is authenticated as administrator,
     it can _send this request to prepare the room for the game.
     """
 
     class Meta:
         name = "prepare"
@@ -518,15 +518,15 @@
     )
 
 
 @dataclass
 class Board:
     """
     The protocol representation of a board.
-    It contains a list of list of fields, which size is 7x7.
+    It contains a list of fields, which size is 7x7.
     """
 
     class Meta:
         name = "board"
 
     list_value: List[ListType] = field(
         default_factory=list,
@@ -671,15 +671,15 @@
     )
 
 
 @dataclass
 class OriginalMessage:
     """
     The original message that was sent by the client.
-    Is sent by the server if a error occurs.
+    Is sent by the server if an error occurs.
     """
 
     class Meta:
         name = "originalMessage"
 
     class_value: Optional[str] = field(
         default=None,
@@ -826,26 +826,60 @@
     scores: Scores
     winner: Winner
 
 
 @dataclass
 class Error:
     """
-    This sends the server when the client sent a erroneous message.
+    This sends the server when the client sent an erroneous message.
     """
     message: str
     originalMessage: OriginalMessage
 
 
 @dataclass
+class Prepared(RoomOrchestrationMessage):
+    class Meta:
+        name = "prepared"
+
+    room_id: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "roomId",
+            "type": "Attribute",
+        }
+    )
+    reservation: List[str] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+
+
+@dataclass
+class Observed(RoomOrchestrationMessage):
+    class Meta:
+        name = "observed"
+
+    room_id: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "roomId",
+            "type": "Attribute",
+        }
+    )
+
+
+@dataclass
 class Protocol:
     """
     This is the root element of the protocol.
     Even it's in here it will never be called,
-    because the children of this root element have to be handelt separately.
+    because the children of this root element have to be handled separately.
     """
 
     class Meta:
         name = "protocol"
 
     authenticate: Optional[Authenticate] = field(
         default=None,
@@ -905,7 +939,21 @@
     room: List[Room] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
 
     )
+
+    prepared: Optional[Prepared] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+
+    observed: Optional[Observed] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
```

### Comparing `socha-1.0.7/socha/utils/package_builder.py` & `socha-1.0.8/socha/utils/package_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,22 +109,28 @@
     def _copy_modules(self):
         """
         Recursively searches for the given python file in the current working directory and its subdirectories,
         and copies all python files with their directory structure to the target_folder.
         """
         logging.info(f'Copying python files to {self.package_name}')
         source_folder = os.getcwd()
-        main_modules = self._get_modules()  # Get the set of module names
+        main_modules = self._get_modules()
         for root, dirs, files in os.walk(source_folder):
+            if "socha_builds" in dirs:
+                dirs.remove("socha_builds")
             for file in files:
                 if file.endswith('.py'):
                     source_file_path = os.path.join(root, file)
                     target_file_path = os.path.join(self.build_dir, self.package_name,
                                                     os.path.relpath(source_file_path, source_folder))
-                    if source_file_path in main_modules:  # Only copy files that were imported in the main script
+                    if file in sys.argv[0]:
+                        os.makedirs(os.path.dirname(target_file_path), exist_ok=True)
+                        shutil.copy2(source_file_path, target_file_path)
+                        logging.info(f'Copying {source_file_path} to {target_file_path}')
+                    if source_file_path in main_modules:
                         os.makedirs(os.path.dirname(target_file_path), exist_ok=True)
                         shutil.copy2(source_file_path, target_file_path)
                         logging.info(f'Copying {source_file_path} to {target_file_path}')
 
     def _create_shell_script(self):
         logging.info(f'Creating shell script {self.package_name}/start.sh')
         with open(f'{self.build_dir}/{self.package_name}/start.sh', 'w', newline='\n') as f:
```

### Comparing `socha-1.0.7/.gitignore` & `socha-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `socha-1.0.7/LICENSE` & `socha-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `socha-1.0.7/README.md` & `socha-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `socha-1.0.7/pyproject.toml` & `socha-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "socha"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
     { name = "FalconsSky", email = "stu222782@mail.uni-kiel.de" },
 ]
 description = "This is the package for the Software-Challenge Germany 2023. This Season the game will be 'Hey, danke für den Fisch' a.k.a. 'Penguins' in short."
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

### Comparing `socha-1.0.7/PKG-INFO` & `socha-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socha
-Version: 1.0.7
+Version: 1.0.8
 Summary: This is the package for the Software-Challenge Germany 2023. This Season the game will be 'Hey, danke für den Fisch' a.k.a. 'Penguins' in short.
 Project-URL: Bug Tracker, https://github.com/FalconsSky/Software-Challenge-Python-Client/issues
 Author-email: FalconsSky <stu222782@mail.uni-kiel.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

