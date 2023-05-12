# Comparing `tmp/netpackAIO-0.0.5.tar.gz` & `tmp/netpackAIO-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpackAIO-0.0.5.tar", last modified: Tue Apr 25 18:36:58 2023, max compression
+gzip compressed data, was "netpackAIO-0.0.8.tar", last modified: Fri May 12 03:14:17 2023, max compression
```

## Comparing `netpackAIO-0.0.5.tar` & `netpackAIO-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 18:36:58.071283 netpackAIO-0.0.5/
--rw-rw-rw-   0        0        0     1089 2023-04-14 20:36:26.000000 netpackAIO-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3405 2023-04-25 18:36:58.072286 netpackAIO-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2894 2023-04-20 20:36:34.000000 netpackAIO-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 18:36:58.035286 netpackAIO-0.0.5/netpack/
--rw-rw-rw-   0        0        0        0 2023-04-12 17:33:48.000000 netpackAIO-0.0.5/netpack/__init__.py
--rw-rw-rw-   0        0        0    11570 2023-04-25 17:06:55.000000 netpackAIO-0.0.5/netpack/func.py
--rw-rw-rw-   0        0        0      877 2023-04-25 17:10:17.000000 netpackAIO-0.0.5/netpack/test.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:36:58.069281 netpackAIO-0.0.5/netpackAIO.egg-info/
--rw-rw-rw-   0        0        0     3405 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-25 18:36:58.078282 netpackAIO-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-04-25 18:36:55.000000 netpackAIO-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:14:17.852909 netpackAIO-0.0.8/
+-rw-rw-rw-   0        0        0     1089 2023-04-14 20:36:26.000000 netpackAIO-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3538 2023-05-12 03:14:17.852909 netpackAIO-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3027 2023-05-12 03:10:59.000000 netpackAIO-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 03:14:17.815909 netpackAIO-0.0.8/netpack/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:33:48.000000 netpackAIO-0.0.8/netpack/__init__.py
+-rw-rw-rw-   0        0        0    13641 2023-05-12 03:11:35.000000 netpackAIO-0.0.8/netpack/func.py
+-rw-rw-rw-   0        0        0      289 2023-05-12 00:39:21.000000 netpackAIO-0.0.8/netpack/test.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:14:17.850908 netpackAIO-0.0.8/netpackAIO.egg-info/
+-rw-rw-rw-   0        0        0     3538 2023-05-12 03:14:17.000000 netpackAIO-0.0.8/netpackAIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-12 03:14:17.000000 netpackAIO-0.0.8/netpackAIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 03:14:17.000000 netpackAIO-0.0.8/netpackAIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-12 03:14:17.000000 netpackAIO-0.0.8/netpackAIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 03:14:17.000000 netpackAIO-0.0.8/netpackAIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-12 03:14:17.858916 netpackAIO-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-05-12 03:14:13.000000 netpackAIO-0.0.8/setup.py
```

### Comparing `netpackAIO-0.0.5/LICENSE` & `netpackAIO-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `netpackAIO-0.0.5/PKG-INFO` & `netpackAIO-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpackAIO
-Version: 0.0.5
+Version: 0.0.8
 Summary: A Python package for performing network-related tasks
 Home-page: https://github.com/crusaderay/netpack
 Author: Dongjie Zhang
 Author-email: crusade.ray@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -29,40 +29,41 @@
 print(response)
 ```
 
 ### Classes and Methods
 The NetPack package contains the following classes and methods:
 
 
-#### NetPack.inr(server: str, ipv4v6: str, query_flags: str = None) -> str
+#### func.NetPack.inr(server: str, ipv4v6: str, query_flags: str = None) -> str
 * This is a static method that takes the following parameters, and return the check result from the INR whois server:
     * server: The whois server address
       * ##### Pre-set NetPack.ServerLocation
           * AFRINIC: The AFRINIC whois server address
           * ARIN: The ARIN whois server address
           * APNIC: The APNIC whois server address
           * LACNIC: The LACNIC whois server address
           * RIPE_NCC: The RIPE NCC whois server address
           * IANA: The IANA whois server address
           * RADB: The RADB website URL
     * ipv4v6: The IP address or CIDR range
     * query_flags: Optional parameter that specifies query flags for certain whois servers
     * (The method returns the response received from the whois server as a string.)
 
-#### NetPack.radb(ip: str) -> str
+#### func.NetPack.radb(ip: str) -> str
 * This is a static method that takes an IPv4 address as an input and return the result from RADB
 
-#### NetPack.ping(host, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> tuple
+#### func.NetPack.ping(host, packet_size=64, ping_type="os", protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> tuple
 * The ping() method can be used to ping a single host:
     * Arguments
         * host: the hostname or IP address of the host to ping.
         * packet_size: the size of the packets to send (in bytes). Default is 64.
+        * ping_type: using socket to initiate the ping or using inherit from OS
         * protocol: the protocol to use for the ping test. Must be either "icmp" or "tcp". Default is "icmp".
         * interval: the time (in seconds) to wait between sending each packet. Default is 0.2.
         * timeout: the time (in seconds) to wait for a response before considering the packet lost. Default is 1.
         * packet_num: the number of packets to send. Default is 5.
 
-#### NetPack.multiple_ping(hosts, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> dict
+#### func.NetPack.multiple_ping(hosts, packet_size=64, ping_type="os", protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> dict
 * The multiple_ping() method can be used to ping multiple hosts in parallel, This will return a dictionary where each key is a host from the hosts list and each value is a dictionary containing the average latency and success rate of the ping test.
     * Arguments
         * The arguments for multiple_ping() are the same as for ping(), except that they are used for all hosts in the hosts list.
```

### Comparing `netpackAIO-0.0.5/README.md` & `netpackAIO-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,39 +13,40 @@
 print(response)
 ```
 
 ### Classes and Methods
 The NetPack package contains the following classes and methods:
 
 
-#### NetPack.inr(server: str, ipv4v6: str, query_flags: str = None) -> str
+#### func.NetPack.inr(server: str, ipv4v6: str, query_flags: str = None) -> str
 * This is a static method that takes the following parameters, and return the check result from the INR whois server:
     * server: The whois server address
       * ##### Pre-set NetPack.ServerLocation
           * AFRINIC: The AFRINIC whois server address
           * ARIN: The ARIN whois server address
           * APNIC: The APNIC whois server address
           * LACNIC: The LACNIC whois server address
           * RIPE_NCC: The RIPE NCC whois server address
           * IANA: The IANA whois server address
           * RADB: The RADB website URL
     * ipv4v6: The IP address or CIDR range
     * query_flags: Optional parameter that specifies query flags for certain whois servers
     * (The method returns the response received from the whois server as a string.)
 
-#### NetPack.radb(ip: str) -> str
+#### func.NetPack.radb(ip: str) -> str
 * This is a static method that takes an IPv4 address as an input and return the result from RADB
 
-#### NetPack.ping(host, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> tuple
+#### func.NetPack.ping(host, packet_size=64, ping_type="os", protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> tuple
 * The ping() method can be used to ping a single host:
     * Arguments
         * host: the hostname or IP address of the host to ping.
         * packet_size: the size of the packets to send (in bytes). Default is 64.
+        * ping_type: using socket to initiate the ping or using inherit from OS
         * protocol: the protocol to use for the ping test. Must be either "icmp" or "tcp". Default is "icmp".
         * interval: the time (in seconds) to wait between sending each packet. Default is 0.2.
         * timeout: the time (in seconds) to wait for a response before considering the packet lost. Default is 1.
         * packet_num: the number of packets to send. Default is 5.
 
-#### NetPack.multiple_ping(hosts, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> dict
+#### func.NetPack.multiple_ping(hosts, packet_size=64, ping_type="os", protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> dict
 * The multiple_ping() method can be used to ping multiple hosts in parallel, This will return a dictionary where each key is a host from the hosts list and each value is a dictionary containing the average latency and success rate of the ping test.
     * Arguments
         * The arguments for multiple_ping() are the same as for ping(), except that they are used for all hosts in the hosts list.
```

### Comparing `netpackAIO-0.0.5/netpack/func.py` & `netpackAIO-0.0.8/netpack/func.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import threading
-
 from bs4 import BeautifulSoup
 import requests
 import ipaddress
 import socket
-import time
 import struct
 import random
 from contextlib import closing
-import concurrent.futures
+import platform
+import subprocess
+import re
+import time
 
 
 class NetPack(object):
     class ServerLocation(object):
         AFRINIC = 'whois.afrinic.net'
         ARIN = 'whois.arin.net'
         APNIC = 'whois.apnic.net'
@@ -132,15 +133,60 @@
         answer = ~total
         # Ensure the answer doesn't exceed 16 bits
         answer &= 0xffff
 
         return answer
 
     @staticmethod
-    def _icmp_ping(host, packet_size, interval, timeout, packet_num):
+    def _icmp_ping_os(host, packet_size, interval, timeout, packet_num):
+        # Sends ICMP echo requests to the specified host and returns the average latency and success rate as a tuple
+
+        # Determine the operating system
+        system = platform.system()
+
+        if system == 'Windows':
+            # For Windows
+            command = ['ping', '-n', str(packet_num), '-l', str(packet_size), '-w', str(int(timeout * 1000)), host]
+            output = subprocess.run(command, capture_output=True, text=True)
+            result = output.stdout
+        elif system == 'Darwin':
+            # For macOS
+            command = ['ping', '-c', str(packet_num), '-s', str(packet_size), '-i', str(interval), '-t', str(timeout),
+                       host]
+            output = subprocess.run(command, capture_output=True, text=True)
+            result = output.stdout
+        elif system == 'Linux':
+            # For Linux
+            command = ['ping', '-c', str(packet_num), '-s', str(packet_size), '-i', str(interval), '-W', str(timeout),
+                       host]
+            output = subprocess.run(command, capture_output=True, text=True)
+            result = output.stdout
+        else:
+            raise OSError(f"Unsupported operating system: {system}")
+
+        # Parse the ping result to calculate average latency and success rate
+        latency_sum = 0
+        received_count = 0
+        lines = result.split('\n')
+        for line in lines:
+            if 'time=' in line:
+                try:
+                    latency = float(re.search(r'time=([0-9.]+)', line).group(1))
+                    latency_sum += latency
+                    received_count += 1
+                except (ValueError, AttributeError):
+                    pass
+
+        average_latency = (latency_sum / received_count) if received_count > 0 else None
+        success_rate = (received_count / packet_num) * 100
+
+        return average_latency, success_rate
+
+    @staticmethod
+    def _icmp_ping_sock(host, packet_size, interval, timeout, packet_num):
         # Sends ICMP echo requests to the specified host and returns the average latency and success rate as a tuple
         if packet_size < 8:
             packet_size = 8
         payload = b'\x00' * (packet_size-8)
         icmp_protocol = socket.getprotobyname("icmp")
         icmp_echo = 8
         packet_id = random.randint(1, 0xffff)
@@ -233,47 +279,47 @@
                 # Wait for the specified interval time before sending the next packet
                 time.sleep(max(0, interval - (time.time() - start_time)))
 
         # Calculate the average latency and packet loss percentage and return as a tuple
         return (total_latency / received_count) * 1000 if received_count > 0 else None, received_count / sent_count * 100
 
     @staticmethod
-    def ping(host, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5):
+    def ping(host, ping_type='os', packet_size=64, protocol="icmp", interval=0.5, timeout=1, packet_num=5):
         # Try to get address information for the given host
         try:
             socket.getaddrinfo(host, None, socket.AF_INET6)
             address_family = socket.AF_INET6  # Use IPv6 address family if available
         except socket.gaierror:
             address_family = socket.AF_INET  # Otherwise, use IPv4 address family
 
         # Depending on the protocol, call the corresponding ping function
         if protocol.lower() == "icmp":
             # ICMP protocol is only supported for IPv4
             if address_family == socket.AF_INET6:
                 raise ValueError("ICMP is not supported for IPv6 addresses in this implementation.")
-            return NetPack._icmp_ping(host, packet_size, interval, timeout, packet_num)
+            if ping_type == 'sock':
+                return NetPack._icmp_ping_sock(host, packet_size, interval, timeout, packet_num)
+            else:
+                return NetPack._icmp_ping_os(host, packet_size, interval, timeout, packet_num)
         elif protocol.lower() == "tcp":
             # Use TCP protocol for both IPv4 and IPv6
             return NetPack._tcp_ping(host, packet_size, interval, timeout, packet_num)
         else:
             # Raise an error if an unsupported protocol is given
             raise ValueError("Unsupported protocol. Please use 'icmp' or 'tcp'.")
 
     @staticmethod
-    def multiple_ping(hosts, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5):
+    def multiple_ping(hosts, ping_type='os', packet_size=64, protocol="icmp", interval=0.5, timeout=1, packet_num=5):
         multiping_results = {}
 
         # Define a function to ping a host and store the result in the results dictionary
-        def ping_host(host):
-            try:
-                latency, success_rate = NetPack.ping(host, packet_size, protocol, interval, timeout, packet_num)
-                multiping_results[host] = {'success_rate': success_rate, 'latency': latency}
-            except Exception as e:
-                print(e)
-                multiping_results[host] = {'success_rate': 0, 'latency': None}
+        def ping_host(ip):
+
+            latency, success_rate = NetPack.ping(ip, ping_type, packet_size, protocol, interval, timeout, packet_num)
+            multiping_results[ip] = {'success_rate': success_rate, 'latency': latency}
 
         # Create a thread for each host and start them all simultaneously
         threads = []
         for host in hosts:
             t = threading.Thread(target=ping_host, args=(host,))
             threads.append(t)
             t.start()
```

### Comparing `netpackAIO-0.0.5/netpackAIO.egg-info/PKG-INFO` & `netpackAIO-0.0.8/netpackAIO.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpackAIO
-Version: 0.0.5
+Version: 0.0.8
 Summary: A Python package for performing network-related tasks
 Home-page: https://github.com/crusaderay/netpack
 Author: Dongjie Zhang
 Author-email: crusade.ray@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -29,40 +29,41 @@
 print(response)
 ```
 
 ### Classes and Methods
 The NetPack package contains the following classes and methods:
 
 
-#### NetPack.inr(server: str, ipv4v6: str, query_flags: str = None) -> str
+#### func.NetPack.inr(server: str, ipv4v6: str, query_flags: str = None) -> str
 * This is a static method that takes the following parameters, and return the check result from the INR whois server:
     * server: The whois server address
       * ##### Pre-set NetPack.ServerLocation
           * AFRINIC: The AFRINIC whois server address
           * ARIN: The ARIN whois server address
           * APNIC: The APNIC whois server address
           * LACNIC: The LACNIC whois server address
           * RIPE_NCC: The RIPE NCC whois server address
           * IANA: The IANA whois server address
           * RADB: The RADB website URL
     * ipv4v6: The IP address or CIDR range
     * query_flags: Optional parameter that specifies query flags for certain whois servers
     * (The method returns the response received from the whois server as a string.)
 
-#### NetPack.radb(ip: str) -> str
+#### func.NetPack.radb(ip: str) -> str
 * This is a static method that takes an IPv4 address as an input and return the result from RADB
 
-#### NetPack.ping(host, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> tuple
+#### func.NetPack.ping(host, packet_size=64, ping_type="os", protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> tuple
 * The ping() method can be used to ping a single host:
     * Arguments
         * host: the hostname or IP address of the host to ping.
         * packet_size: the size of the packets to send (in bytes). Default is 64.
+        * ping_type: using socket to initiate the ping or using inherit from OS
         * protocol: the protocol to use for the ping test. Must be either "icmp" or "tcp". Default is "icmp".
         * interval: the time (in seconds) to wait between sending each packet. Default is 0.2.
         * timeout: the time (in seconds) to wait for a response before considering the packet lost. Default is 1.
         * packet_num: the number of packets to send. Default is 5.
 
-#### NetPack.multiple_ping(hosts, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> dict
+#### func.NetPack.multiple_ping(hosts, packet_size=64, ping_type="os", protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> dict
 * The multiple_ping() method can be used to ping multiple hosts in parallel, This will return a dictionary where each key is a host from the hosts list and each value is a dictionary containing the average latency and success rate of the ping test.
     * Arguments
         * The arguments for multiple_ping() are the same as for ping(), except that they are used for all hosts in the hosts list.
```

### Comparing `netpackAIO-0.0.5/setup.py` & `netpackAIO-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='netpackAIO',
-    version='0.0.5',
+    version='0.0.8',
     description='A Python package for performing network-related tasks',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Dongjie Zhang',
     author_email='crusade.ray@gmail.com',
     url='https://github.com/crusaderay/netpack',
     packages=find_packages(),
```

