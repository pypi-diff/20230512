# Comparing `tmp/mktrader-0.0.2.tar.gz` & `tmp/mktrader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktrader-0.0.2.tar", last modified: Thu May 11 23:37:17 2023, max compression
+gzip compressed data, was "mktrader-0.0.3.tar", last modified: Fri May 12 04:02:34 2023, max compression
```

## Comparing `mktrader-0.0.2.tar` & `mktrader-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mmurphy  (433907835) 1133555842        0 2023-05-11 23:37:17.221936 mktrader-0.0.2/
--rw-r--r--   0 mmurphy  (433907835) 1133555842     1068 2023-05-11 23:09:55.000000 mktrader-0.0.2/LICENSE
--rw-r--r--   0 mmurphy  (433907835) 1133555842      642 2023-05-11 23:37:17.221670 mktrader-0.0.2/PKG-INFO
--rw-r--r--   0 mmurphy  (433907835) 1133555842      213 2023-05-11 23:10:15.000000 mktrader-0.0.2/README.md
-drwxr-xr-x   0 mmurphy  (433907835) 1133555842        0 2023-05-11 23:37:17.220589 mktrader-0.0.2/mktrader/
--rw-r--r--   0 mmurphy  (433907835) 1133555842      185 2023-05-11 23:10:15.000000 mktrader-0.0.2/mktrader/__init__.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     3890 2023-05-11 23:10:15.000000 mktrader-0.0.2/mktrader/brokers.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     4236 2023-05-11 23:10:15.000000 mktrader-0.0.2/mktrader/engines.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     5477 2023-05-11 23:10:15.000000 mktrader-0.0.2/mktrader/feeds.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     4045 2023-05-11 23:10:15.000000 mktrader-0.0.2/mktrader/helpers.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     4754 2023-05-11 23:10:15.000000 mktrader-0.0.2/mktrader/indicators.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     1244 2023-05-11 23:10:15.000000 mktrader-0.0.2/mktrader/logger.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     7290 2023-05-11 23:29:10.000000 mktrader-0.0.2/mktrader/models.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     1027 2023-05-11 23:10:15.000000 mktrader-0.0.2/mktrader/strategies.py
-drwxr-xr-x   0 mmurphy  (433907835) 1133555842        0 2023-05-11 23:37:17.221407 mktrader-0.0.2/mktrader.egg-info/
--rw-r--r--   0 mmurphy  (433907835) 1133555842      642 2023-05-11 23:37:17.000000 mktrader-0.0.2/mktrader.egg-info/PKG-INFO
--rw-r--r--   0 mmurphy  (433907835) 1133555842      368 2023-05-11 23:37:17.000000 mktrader-0.0.2/mktrader.egg-info/SOURCES.txt
--rw-r--r--   0 mmurphy  (433907835) 1133555842        1 2023-05-11 23:37:17.000000 mktrader-0.0.2/mktrader.egg-info/dependency_links.txt
--rw-r--r--   0 mmurphy  (433907835) 1133555842       26 2023-05-11 23:37:17.000000 mktrader-0.0.2/mktrader.egg-info/requires.txt
--rw-r--r--   0 mmurphy  (433907835) 1133555842        9 2023-05-11 23:37:17.000000 mktrader-0.0.2/mktrader.egg-info/top_level.txt
--rw-r--r--   0 mmurphy  (433907835) 1133555842       38 2023-05-11 23:37:17.221993 mktrader-0.0.2/setup.cfg
--rw-r--r--   0 mmurphy  (433907835) 1133555842      960 2023-05-11 23:30:12.000000 mktrader-0.0.2/setup.py
+drwxr-xr-x   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)        0 2023-05-12 04:02:34.987712 mktrader-0.0.3/
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     1068 2023-05-11 23:09:55.000000 mktrader-0.0.3/LICENSE
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)      699 2023-05-12 04:02:34.987549 mktrader-0.0.3/PKG-INFO
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)      213 2023-05-11 23:10:15.000000 mktrader-0.0.3/README.md
+drwxr-xr-x   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)        0 2023-05-12 04:02:34.986477 mktrader-0.0.3/mktrader/
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)      185 2023-05-11 23:10:15.000000 mktrader-0.0.3/mktrader/__init__.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     3893 2023-05-12 03:48:43.000000 mktrader-0.0.3/mktrader/brokers.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     4300 2023-05-12 03:52:25.000000 mktrader-0.0.3/mktrader/engines.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     5510 2023-05-12 03:56:07.000000 mktrader-0.0.3/mktrader/feeds.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     3894 2023-05-12 03:57:48.000000 mktrader-0.0.3/mktrader/helpers.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     4754 2023-05-11 23:10:15.000000 mktrader-0.0.3/mktrader/indicators.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     1244 2023-05-11 23:10:15.000000 mktrader-0.0.3/mktrader/logger.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     7290 2023-05-12 03:40:29.000000 mktrader-0.0.3/mktrader/models.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     1055 2023-05-12 03:59:20.000000 mktrader-0.0.3/mktrader/strategies.py
+drwxr-xr-x   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)        0 2023-05-12 04:02:34.987338 mktrader-0.0.3/mktrader.egg-info/
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)      699 2023-05-12 04:02:34.000000 mktrader-0.0.3/mktrader.egg-info/PKG-INFO
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)      368 2023-05-12 04:02:34.000000 mktrader-0.0.3/mktrader.egg-info/SOURCES.txt
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)        1 2023-05-12 04:02:34.000000 mktrader-0.0.3/mktrader.egg-info/dependency_links.txt
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)       26 2023-05-12 04:02:34.000000 mktrader-0.0.3/mktrader.egg-info/requires.txt
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)        9 2023-05-12 04:02:34.000000 mktrader-0.0.3/mktrader.egg-info/top_level.txt
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)       38 2023-05-12 04:02:34.987764 mktrader-0.0.3/setup.cfg
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     1017 2023-05-12 03:45:07.000000 mktrader-0.0.3/setup.py
```

### Comparing `mktrader-0.0.2/LICENSE` & `mktrader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mktrader-0.0.2/PKG-INFO` & `mktrader-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: mktrader
-Version: 0.0.2
+Version: 0.0.3
 Summary: Stock Market Trading Framework
+Home-page: https://github.com/matthewkurtis/mktrader.git
 Author: Matthew K Murphy (MatthewKurtis)
 Author-email: <mkmurphy526@gmail.com>
 Keywords: python,trading,stock,market
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `mktrader-0.0.2/mktrader/brokers.py` & `mktrader-0.0.3/mktrader/brokers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
 import requests
-from .models import *
+from typing import Optional
+from .models import Broker, BracketOrder
 from .logger import logger
 
 
 class Alpaca(Broker):
-    def __init__(self, api_key, api_secret, paper:Optional[bool]=False):
+    def __init__(self, api_key, api_secret, paper: Optional[bool] = False):
         self.api_key = api_key
         self.api_secret = api_secret
         self.paper = paper
 
-        ALPACA_TRADE_API_URL_PAPER = "https:/paper-api.alpaca.markets"   
+        ALPACA_TRADE_API_URL_PAPER = "https:/paper-api.alpaca.markets"
         ALPACA_TRADE_API_URL_LIVE = "https://api.alpaca.markets"
 
-        if self.paper == True:
+        if self.paper is True:
             self.api_url = ALPACA_TRADE_API_URL_PAPER
         else:
             self.api_url = ALPACA_TRADE_API_URL_LIVE
 
         self.headers = {
             'APCA-API-KEY-ID': self.api_key,
             'APCA-API-SECRET-KEY': self.api_secret
@@ -76,26 +77,26 @@
         logger.info("Checking Pending Orders..")
         orders = []
         if len(json_response) == 0:
             logger.info("No Orders Found")
         else:
             for order in json_response:
                 if order['symbol'] == ticker:
-                    logger.info(f"PENDING ORDER FOUND WITH ID: {order['client_order_id']} ({order['id']}) - {order['symbol']} {order['side']} {order['qty']}") 
+                    logger.info(f"PENDING ORDER FOUND WITH ID: {order['client_order_id']} ({order['id']}) - {order['symbol']} {order['side']} {order['qty']}")
                     logger.info(order)
                     orders.append(order['id'])
-        return orders 
-            
-    def submit_order(self, order:BracketOrder) -> dict:
+        return orders
+
+    def submit_order(self, order: BracketOrder) -> dict:
         endpoint = '/v2/orders'
         url = self.api_url + endpoint
-        order = order.asAlpacaOrder() #:dict
-        logger.info(f"ORDER TO SUBMIT:\n{json.dumps(order)}\n") #:str
-        response = requests.post(url=url, headers=self.headers, data=json.dumps(order))#:str
-        json_response = response.json() #:dict
+        order = order.asAlpacaOrder()
+        logger.info(f"ORDER TO SUBMIT:\n{json.dumps(order)}\n")
+        response = requests.post(url=url, headers=self.headers, data=json.dumps(order))
+        json_response = response.json()
         logger.info(f"ORDER RESPONSE:\n{json_response}\n")
-        return json_response #:dict
+        return json_response
 
-    def cancel_order(self, order_id:str) -> None:
+    def cancel_order(self, order_id: str) -> None:
         endpoint = f'/v2/orders/{order_id}'
         url = self.api_url + endpoint
         requests.delete(url=url, headers=self.headers)
```

### Comparing `mktrader-0.0.2/mktrader/engines.py` & `mktrader-0.0.3/mktrader/engines.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,91 +1,97 @@
-from .models import *
+from .models import Engine, Candle
 from .logger import logger
 from . import indicators, helpers
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from collections import deque
 
 
 @dataclass
 class Live_Websocket(Engine):
     """
     Websocket function.
-    
+
     - requests history of bars in proper timeframe
     - Listens to 1 minute websocket connection.
     - Stores incoming bars and resamples to the required timeframe
     - Appends new candle to candles list
     ---
     - applies indicators from strategy
     - pulls out latest candle
     - passes candle to strategy.onData function
     """
-    
+
     previous_bar = None
     candles = []
     minute_candle_deque = deque([])
 
-    def on_candle(self, candle:Candle):
+    def on_candle(self, candle: Candle):
         self.minute_candle_deque.append(candle)
         next_candle_start = helpers.get_next_run_time(date_time=candle.date, num=self.strategy.time_int, period=self.strategy.time_period)
-        
+
         last_current_candle_bar = next_candle_start - timedelta(minutes=1)
         if candle.date == last_current_candle_bar:
             open = self.minute_candle_deque[0].open
             high = max(c.high for c in self.minute_candle_deque)
             low = min(c.low for c in self.minute_candle_deque)
             close = self.minute_candle_deque[-1].close
             volume = sum(c.volume for c in self.minute_candle_deque)
-            
+
             new_candle = Candle(self.minute_candle_deque[0].ticker, self.minute_candle_deque[0].date, open, high, low, close, volume)
 
             logger.info(new_candle)
             self.candles.append(new_candle)
             # remove the used candles from the deque
             self.minute_candle_deque.clear()
 
             # INDICATORS
-            indicated_candles = indicators.add_indicators(self.strategy, self.candles) 
+            indicated_candles = indicators.add_indicators(self.strategy, self.candles)
             # PROCESS
             latest_candle = indicated_candles[-1]
             if not self.broker.market_is_open(latest_candle):
-                if self.strategy.extended_hours == False:
+                if self.strategy.extended_hours is False:
                     logger.info("Market Closed..")
                     return
-                elif self.strategy.extended_hours == True:
+                elif self.strategy.extended_hours is True:
                     logger.info("Extended Hours Session..")
             if self.previous_bar is None or latest_candle.date > self.previous_bar.date:
                 helpers.log_candle_info(candle=latest_candle)
                 self.strategy.onData(candle=latest_candle, broker=self.broker)
                 self.previous_bar = latest_candle
             else:
                 logger.debug("BAR EXISTS, SKIPPING")
 
-
     def run(self):
         self.candles = self.datasource.get_candles()
         logger.debug(self.candles)
 
-        # We may have an incomplete current candle. We need to scrap it from the history if it exists and grab any missing data needed to fill the minute_candle_deque so our new candle calculations will be complete.
-        next_candle_start = helpers.get_next_run_time(date_time=datetime.utcnow(), num=self.strategy.time_int, period=self.strategy.time_period)
+        """We may have an incomplete current candle. We need to scrap it from
+        the history if it exists and grab any missing data needed to fill the
+        minute_candle_deque so our new candle calculations will be complete."""
+
+        next_candle_start = helpers.get_next_run_time(
+                date_time=datetime.utcnow(),
+                num=self.strategy.time_int,
+                period=self.strategy.time_period)
         if self.strategy.time_period == "min":
-            in_process_candle_start = next_candle_start - timedelta(minutes=self.strategy.time_int) 
+            in_process_candle_start = next_candle_start - timedelta(minutes=self.strategy.time_int)
         elif self.strategy.time_period == "hour":
             in_process_candle_start = next_candle_start - timedelta(hours=self.strategy.time_int)
         logger.debug(f"IN PROCESS CANDLE TO DELETE [TIME]: {in_process_candle_start}")
         for candle in self.candles:
             if candle.date >= in_process_candle_start:
                 del self.candles[self.candles.index(candle)]
         logger.debug("LIST UPDATED TO REMOVE ANY IN-PROCESS CANDLES:")
         logger.debug(self.candles)
 
-        # Now we need to get 1-minute candles and pass them to the minute_candle_list before we start getting real-time 1-minute candles
-        catch_up_minute_candles = self.datasource.get_candles(minute_catch_up=in_process_candle_start) 
+        """Now we need to get 1-minute candles and pass them to the minute_candle_list
+        before we start getting real-time 1-minute candles"""
+
+        catch_up_minute_candles = self.datasource.get_candles(minute_catch_up=in_process_candle_start)
         logger.debug("CATCH UP MINUTE CANDLES:")
         logger.debug(catch_up_minute_candles)
         # Add them to the deque to be processed
         for catch_up_candle in catch_up_minute_candles:
             self.minute_candle_deque.append(catch_up_candle)
         # Now start getting live candles
         self.datasource.get_live_candles()
-
```

### Comparing `mktrader-0.0.2/mktrader/feeds.py` & `mktrader-0.0.3/mktrader/feeds.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from .models import *
+from .models import DataFeed, Candle
 from .logger import logger
 from typing import Optional, List
 from datetime import datetime
 import requests
 import websocket
 import json
 
 
 class Alpaca_Historical_Bars(DataFeed):
-    def __init__(self, engine, api_key:str, api_secret:str, sip:Optional[bool]=False):
+    ALPACA_DATA_API_URL = "https://data.alpaca.markets"
+
+    def __init__(self, engine, api_key: str, api_secret: str, sip: Optional[bool] = False):
         super().__init__(engine)
         self.api_key = api_key
         self.api_secret = api_secret
         self.sip = sip
 
-        self.ALPACA_DATA_API_URL = "https://data.alpaca.markets"
-
-
-    def get_candles(self, minute_catch_up:Optional[datetime]=None) -> List[Candle]:
+    def get_candles(self, minute_catch_up: Optional[datetime] = None) -> List[Candle]:
         time_period = self.engine.strategy.time_period
         time_int = self.engine.strategy.time_int
 
         if minute_catch_up is not None:
             time_int = 1
             time_period = "min"
 
@@ -52,89 +51,87 @@
         candles = []
         if self.engine.asset.asset_class == "us_equity":
             bars_list = json_response["bars"]
         elif self.engine.asset.asset_class == "crypto":
             bars_list = json_response["bars"][self.engine.asset.symbol]
         for bar in bars_list:
             candle = Candle(
-                ticker=self.engine.asset.symbol, 
+                ticker=self.engine.asset.symbol,
                 date=datetime.strptime(bar['t'], "%Y-%m-%dT%H:%M:%SZ"),
                 open=bar["o"],
                 high=bar["h"],
                 low=bar["l"],
                 close=bar["c"],
                 volume=bar["v"]
             )
             candles.append(candle)
-        
+
         if minute_catch_up is not None:
             print(f"MINUTE CATCH UP: {minute_catch_up}")
             minute_candles = [candle for candle in candles if candle.date >= minute_catch_up]
             for minute_candle in minute_candles:
                 if minute_candle.date.minute == datetime.utcnow().minute:
                     print(f"IN PROCESS, REMOVING: {minute_candle}")
                     del minute_candles[minute_candles.index(minute_candle)]
             return minute_candles
         else:
             return candles
 
 
+class Alpaca_Live_Bars(DataFeed):
+    ALPACA_STREAM_API_URL_IEX = "wss://stream.data.alpaca.markets/v2/iex"
+    ALPACA_STREAM_API_URL_SIP = "wss://stream.data.alpaca.markets/v2/sip"
+    ALPACA_STREAM_API_URL_CRYPTO = "wss://stream.data.alpaca.markets/v1beta2/crypto"
+    ALPACA_DATA_API_URL = "https://data.alpaca.markets"
 
-class Alpaca_Live_Bars(DataFeed):  
-    def __init__(self, engine, api_key:str, api_secret:str, sip:Optional[bool]=False):
+    def __init__(self, engine, api_key: str, api_secret: str, sip: Optional[bool] = False):
         super().__init__(engine)
         self.api_key = api_key
         self.api_secret = api_secret
         self.sip = sip
 
-        self.ALPACA_STREAM_API_URL_IEX = "wss://stream.data.alpaca.markets/v2/iex"
-        self.ALPACA_STREAM_API_URL_SIP = "wss://stream.data.alpaca.markets/v2/sip"
-        self.ALPACA_STREAM_API_URL_CRYPTO = "wss://stream.data.alpaca.markets/v1beta2/crypto"
-
-        if self.sip == True:
+        if self.sip is True:
             self.api_stream_url = self.ALPACA_STREAM_API_URL_SIP
         else:
             self.api_stream_url = self.ALPACA_STREAM_API_URL_IEX
 
-    def get_candles(self, minute_catch_up:Optional[datetime]=None):
+    def get_candles(self, minute_catch_up: Optional[datetime] = None):
         return Alpaca_Historical_Bars.get_candles(self, minute_catch_up)
 
-
     def get_live_candles(self) -> List[Candle]:
         if self.engine.asset.asset_class == "us_equity":
             socket_url = self.api_stream_url
         elif self.engine.asset.asset_class == "crypto":
             socket_url = self.ALPACA_STREAM_API_URL_CRYPTO
         logger.debug(f"SOCKET URL: {socket_url}")
 
         def on_open(ws):
             auth_message = {"action": "auth", "key": self.api_key, "secret": self.api_secret}
             ws.send(json.dumps(auth_message))
-            subscribe_message = {"action":"subscribe","bars":[self.engine.asset.symbol]}
+            subscribe_message = {"action": "subscribe", "bars": [self.engine.asset.symbol]}
             ws.send(json.dumps(subscribe_message))
 
         def on_message(ws, message):
             json_data = json.loads(message)
             for item in json_data:
                 if item['T'] == 'b':
                     candle = Candle(
-                        ticker=item['S'], 
-                        date=datetime.strptime(item['t'], "%Y-%m-%dT%H:%M:%SZ"), 
-                        open=float(item['o']), 
-                        high=float(item['h']), 
-                        low=float(item['l']), 
-                        close=float(item['c']), 
+                        ticker=item['S'],
+                        date=datetime.strptime(item['t'], "%Y-%m-%dT%H:%M:%SZ"),
+                        open=float(item['o']),
+                        high=float(item['h']),
+                        low=float(item['l']),
+                        close=float(item['c']),
                         volume=float(item['v'])
                     )
                     logger.debug(candle)
                     self.engine.on_candle(candle)
-                else: 
+                else:
                     logger.info(item)
 
         def on_close(ws):
             logger.info("Websocket Connection Closed..")
 
 
         # Connect to the WebSocket
-        ws = websocket.WebSocketApp(socket_url,on_open=on_open, on_message=on_message, on_close=on_close)
+        ws = websocket.WebSocketApp(socket_url, on_open=on_open, on_message=on_message, on_close=on_close)
         ws.run_forever()
-
```

### Comparing `mktrader-0.0.2/mktrader/helpers.py` & `mktrader-0.0.3/mktrader/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from .logger import logger
 from .models import Order, Candle
 from datetime import datetime, timedelta
 from typing import List
 import copy
 
 
-
-
-def get_next_run_time(date_time:datetime, num: int, period: str) -> datetime:
+def get_next_run_time(date_time: datetime, num: int, period: str) -> datetime:
     """
     Calculates the next run time based on the given time period and number.
     Args:
         num (int): Number to be used to calculate the next run time.
         period (str): Time period for which the next run time needs to be calculated. Valid values are 'min' and 'hour'.
     Returns:
         datetime: The next run time.
@@ -49,59 +47,56 @@
     else:
         logger.debug("Invalid Time Period...")
         return None
     logger.info("\n--------------------------------------")
     return dt
 
 
-def orderDict_to_Order(orders_dict:dict) -> List[Order]:
+def orderDict_to_Order(orders_dict: dict) -> List[Order]:
     """
     Convert dict (order) to Order object using dictionary comprehension for matching keys
     """
-    orders=[]
+    orders = []
     for order_item in orders_dict:
         logger.debug(f"ORDER-DICT: {order_item}")
         order_kwargs = {k: v for k, v in order_item.items() if k in Order.__annotations__}
         # Use the unpacking operator to pass the order_kwargs dictionary as keyword arguments to create a new Order object
         order = Order(**order_kwargs)
         logger.debug(f"ORDER OBJECT CREATED: {vars(order)}")
         orders.append(order)
     logger.debug(f"ORDER OBJECTS LIST FINALIZED: {orders}")
     return orders
 
 
-def process_orders(message:dict) -> List[Order]:
+def process_orders(message: dict) -> List[Order]:
     """
     This takes alpaca API order response as a dict and processes it into a list of Order objects
     Helpful for inserting into DB for tracking orders.
     """
     logger.debug(f"ORDER TO PROCESS: {message}")
     logger.debug(f"ORDER TO PROCESS TYPE = {type(message)}")
-    
+
     orders = []
-    
-    if "legs" in message and isinstance(message["legs"], (list, dict)): #This checks if "legs" is a key in message and if its value is either a list or dictionary, which are indexable objects in Python.
+
+    if "legs" in message and isinstance(message["legs"], (list, dict)):
         logger.debug("MESSAGE HAS LEGS, PROCESSING...")
         for leg in message["legs"]:
             orders.append(leg)
-            logger.debug("APPENDING LEGS TO ORDERS") 
-            
+            logger.debug("APPENDING LEGS TO ORDERS")
+
         # Create a copy of the message and remove the legs from the copy
         message_copy = copy.deepcopy(message)
         message_copy["legs"] = None
         orders.append(message_copy)
     else:
         orders.append(message)
     logger.debug(f"ORDERS LIST: {orders}")
 
     order_objects = orderDict_to_Order(orders)
     logger.debug(f"ORDER OBJECTS PROCESSED: {order_objects}")
     return order_objects
 
 
-def log_candle_info(candle:Candle):
+def log_candle_info(candle: Candle):
     logger.info("\n--------------------------------------")
     logger.info(f"Candle Time: {candle.date}")
     logger.info(f"NEW CANDLE ---> {candle.ticker} O:{candle.open:.2f} H:{candle.high:.2f} L:{candle.low:.2f} C:{candle.close:.2f} - Stop:{candle.recent_low:.2f} - BarsDN:{candle.bars_dn}")
-
-
-
```

### Comparing `mktrader-0.0.2/mktrader/indicators.py` & `mktrader-0.0.3/mktrader/indicators.py`

 * *Files identical despite different names*

### Comparing `mktrader-0.0.2/mktrader/logger.py` & `mktrader-0.0.3/mktrader/logger.py`

 * *Files identical despite different names*

### Comparing `mktrader-0.0.2/mktrader/models.py` & `mktrader-0.0.3/mktrader/models.py`

 * *Files identical despite different names*

### Comparing `mktrader-0.0.2/mktrader/strategies.py` & `mktrader-0.0.3/mktrader/strategies.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-from .models import *
+from .models import Strategy, Candle, Engine
 from .logger import logger
 from typing import Optional
 from datetime import datetime
 
 
 class PrintStrategy(Strategy):
-    def __init__(self, engine:Engine, time_int:int, time_period:str, start:Optional[datetime] = None, end:Optional[datetime] = None, limit:Optional[int] = None):
+    def __init__(self, engine: Engine, time_int: int, time_period: str, start: Optional[datetime] = None, end: Optional[datetime] = None, limit: Optional[int] = None):
         super().__init__(engine)
         self.time_int = time_int
         self.time_period = time_period
         self.start = start
         self.end = end
         self.limit = limit
 
         self.indicators = [
             "heikin_ashi",
             "bars_down"
-        ] 
+        ]
 
-    def onData(self, candle:Candle):
+    def onData(self, candle: Candle):
         """
         This function is called by run.py on every new candle to DB
         Timeframe is determined by config above
         """
         logger.debug("---- SYMBOL:")
         logger.debug(self.engine.asset.symbol)
         logger.debug("---- BROKER:")
         logger.debug(self.engine.broker)
         logger.debug("---- CANDLE:")
         logger.debug(candle)
         logger.debug("--------------------")
-
```

### Comparing `mktrader-0.0.2/mktrader.egg-info/PKG-INFO` & `mktrader-0.0.3/mktrader.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: mktrader
-Version: 0.0.2
+Version: 0.0.3
 Summary: Stock Market Trading Framework
+Home-page: https://github.com/matthewkurtis/mktrader.git
 Author: Matthew K Murphy (MatthewKurtis)
 Author-email: <mkmurphy526@gmail.com>
 Keywords: python,trading,stock,market
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `mktrader-0.0.2/setup.py` & `mktrader-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Stock Market Trading Framework'
 LONG_DESCRIPTION = 'A Framework for simple creation and deployment of trading strategies.'
 
 # Setting up
 setup(
     name="mktrader",
     version=VERSION,
     author="Matthew K Murphy (MatthewKurtis)",
     author_email="<mkmurphy526@gmail.com>",
+    url="https://github.com/matthewkurtis/mktrader.git",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[
         'websocket-client',
         'requests'
```

