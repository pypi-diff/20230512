# Comparing `tmp/dxsp-2.2.2.tar.gz` & `tmp/dxsp-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.2.2.tar", max compression
+gzip compressed data, was "dxsp-2.2.3.tar", max compression
```

## Comparing `dxsp-2.2.2.tar` & `dxsp-2.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-10 11:05:15.055733 dxsp-2.2.2/LICENSE
--rw-r--r--   0        0        0     2605 2023-05-10 11:05:15.055733 dxsp-2.2.2/README.md
--rw-r--r--   0        0        0       86 2023-05-10 11:05:15.703731 dxsp-2.2.2/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-10 11:05:15.055733 dxsp-2.2.2/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-10 11:05:15.055733 dxsp-2.2.2/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-10 11:05:15.055733 dxsp-2.2.2/dxsp/config.py
--rw-r--r--   0        0        0     3432 2023-05-10 11:05:15.055733 dxsp-2.2.2/dxsp/default_settings.toml
--rw-r--r--   0        0        0    29162 2023-05-10 11:05:15.055733 dxsp-2.2.2/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-10 11:05:15.703731 dxsp-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 dxsp-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-12 05:31:33.453496 dxsp-2.2.3/LICENSE
+-rw-r--r--   0        0        0     2605 2023-05-12 05:31:33.453496 dxsp-2.2.3/README.md
+-rw-r--r--   0        0        0       86 2023-05-12 05:31:34.301524 dxsp-2.2.3/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-12 05:31:33.453496 dxsp-2.2.3/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-12 05:31:33.453496 dxsp-2.2.3/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-12 05:31:33.453496 dxsp-2.2.3/dxsp/config.py
+-rw-r--r--   0        0        0     3139 2023-05-12 05:31:33.453496 dxsp-2.2.3/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    29260 2023-05-12 05:31:33.453496 dxsp-2.2.3/dxsp/main.py
+-rw-r--r--   0        0        0     1811 2023-05-12 05:31:34.301524 dxsp-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 dxsp-2.2.3/PKG-INFO
```

### Comparing `dxsp-2.2.2/LICENSE` & `dxsp-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.2/README.md` & `dxsp-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.2/dxsp/assets/blockchains.py` & `dxsp-2.2.3/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.2/dxsp/default_settings.toml` & `dxsp-2.2.3/dxsp/default_settings.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 [default]
 loglevel = "INFO"
-#📝tokenlist
-#headers = '{"User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.4 Safari/605.1.15"}'
-#headers = '{"accept": "application/json, text/plain, */*", "content-type": "application/json"}'
-#headers = '{"User-Agent": "Mozilla/5.0"}'
 headers = {User-Agent= 'Mozilla/5.0'}
-
+#📝tokenlist
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 #📝trading setup
 trading_quote_ccy = "USDT"
 trading_risk_amount = 10 # 10% of the position
 dex_trading_slippage = 2 # 2 % slippage
 #user settings
 dex_wallet_address = "0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE" #this is an example
 dex_private_key = "0x111111111117dc0aaaaaa0fa6a738034aaaa302" #this is an example
-dex_block_explorer_api =  "798437294880920392"  #this is an example
 #chain_1 #see below for other chain ids or use https://chainlist.org to overwrite settings
 dex_chain_id = 1
 dex_protocol_type = "uniswap_v2" #0x | 1inch | uniswap_v3
-
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_block_explorer_url = "https://api.etherscan.io/api?"
+dex_block_explorer_api =  "798437294880920392"  #this is an example
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D" 
 
 #protocol specific
 #🦄1inch
 dex_1inch_url = "https://api.1inch.exchange/v5.0/"
 dex_1inch_limit_url = "https://limit-orders.1inch.io/v3.0/"
 #0️⃣0x
 dex_0x_url = "https://api.0x.org/mainnet/"
 dex_0x_api_key = "" 
-
 #🪐apollo
 dex_apollo_url = "https://fapi.apollox.finance/"
 dex_apollo_spot_api_key = ""
 dex_apollo_spot_api_secret = ""
 dex_apollo_future_api_key = ""
 dex_apollo_future_api_secret = ""
 
-
 [chain_1]
 dex_chain_id = 1
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_block_explorer_url = "https://api.etherscan.io/api?"
 dex_protocol_type = "uniswap_v2"
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
 dex_0x_url = "https://api.0x.org/mainnet/"
```

### Comparing `dxsp-2.2.2/dxsp/main.py` & `dxsp-2.2.3/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
  DEX SWAP Main
 """
 
 import logging
 
 import requests
+from uniswap import Uniswap
 from dxsp import __version__
 from dxsp.config import settings
 
 from pycoingecko import CoinGeckoAPI
 from web3 import Web3
 
 
@@ -30,14 +31,23 @@
 
         self.protocol_type = settings.dex_protocol_type
         self.chain_id = settings.dex_chain_id
         # USER
         self.wallet_address = settings.dex_wallet_address
         self.private_key = settings.dex_private_key
 
+        # UNISWAP 🦄
+        if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
+            self.uniswap = Uniswap(
+                address=self.wallet_address,
+                private_key=self.private_key,
+                version=2 if self.protocol_type == "uniswap_v2" else 3,
+                web3=self.w3,
+                default_slippage=settings.slippage)
+
         # COINGECKO 🦎
         try:
             self.cg = CoinGeckoAPI()
             assetplatform = self.cg.get_asset_platforms()
             output_dict = [x for x in assetplatform if x['chain_identifier']
                            == int(self.chain_id)]
             self.cg_platform = output_dict[0]['id']
@@ -58,31 +68,28 @@
             return
         try:
             if self.protocol_type in ["1inch", "1inch_limit"]:
                 self.logger.debug("1inch getquote")
                 await self.get_quote_1inch(
                     asset_in_address,
                     asset_out_address)
-            if self.protocol_type == "uniswap_v2":
-                self.logger.debug("uniswap_v2 getquote")
-                await self.get_quote_uniswap_v2(
+            if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
+                self.logger.debug("uniswap getquote")
+                await self.get_quote_uniswap(
                     asset_in_address,
                     asset_out_address)
             if self.protocol_type == "0x":
                 self.logger.debug("0x getquote")
                 await self.get_quote_0x(
                     symbol,
                     asset_out_symbol,)
             if self.protocol_type == "apollo":
                 self.logger.debug("apollo getquote")
                 await self.get_quote_apollo()
-            if self.protocol_type == "uniswap_v3":
-                await self.get_quote_uniswap_v3(
-                    asset_in_address,
-                    asset_out_address)
+
         except Exception as e:
             self.logger.error("get_quote %s", e)
             return
 
     async def get_swap(
                 self,
                 asset_out_symbol: str,
@@ -124,16 +131,16 @@
             self.logger.debug("order_amount %s", order_amount)
 
             # VERIFY IF ASSET OUT IS APPROVED otherwise get it approved
             if (await self.get_approve(asset_out_address)) is None:
                 return
 
             # UNISWAP V2
-            if self.protocol_type in ["uniswap_v2"]:
-                swap_order = await self.get_swap_uniswap_v2(
+            if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
+                swap_order = await self.get_swap_uniswap(
                     asset_out_address,
                     asset_in_address,
                     order_amount)
             # 0x
             if self.protocol_type == "0x":
                 swap_order = await self.get_quote_0x(
                     asset_in_symbol,
@@ -142,17 +149,14 @@
 
             # 1INCH
             if self.protocol_type in ["1inch"]:
                 swap_order = await self.get_swap_1inch(
                     asset_out_address,
                     asset_in_address,
                     order_amount)
-            # UNISWAP V3
-            if self.protocol_type in ['uniswap_v3']:
-                swap_order = await self.get_swap_uniswap_v3()
 
             if swap_order:
                 self.logger.debug("swap_order %s", swap_order)
                 signed_order = await self.get_sign(swap_order)
                 order_hash = str(self.w3.to_hex(signed_order))
                 order_hash_details = self.w3.wait_for_transaction_receipt(
                                         order_hash,
@@ -265,15 +269,15 @@
                         token)
                     if token_contract is None:
                         token_contract = await self.search_cg_contract(
                             token)
             if token_contract is not None:
                 self.logger.info("token_contract found %s", token_contract)
                 return self.w3.to_checksum_address(token_contract)
-            self.logger.info("no contract found for %s", token)
+            return f"no contract found for {token}"
         except Exception as e:
             self.logger.error("search_contract %s", e)
             return
 
     async def search_cg(self, token):
         """search coingecko"""
         try:
@@ -339,15 +343,14 @@
         try:
             self.logger.debug("url: %s", url)
             self.logger.debug("_header: %s", settings.headers)
             response = requests.get(
                 url,
                 params=params,
                 headers=headers,
-                # headers={'User-Agent': 'Mozilla/5.0'},
                 timeout=10)
             self.logger.debug("_response: %s", response)
             if response:
                 # self.logger.debug("_json: %s", response.json())
                 return response.json()
 
         except Exception as e:
@@ -539,31 +542,35 @@
             return
         except Exception as e:
             self.logger.error("get_account_position: %s", e)
             return 0
 
 # PROTOCOL SPECIFIC
 # uniswap v2 🦄
-    async def get_quote_uniswap_v2(
+    async def get_quote_uniswap(
         self,
         asset_in_address,
         asset_out_address,
         amount=1
     ):
-        self.logger.debug("get_quote_uniswap_v2")
+        self.logger.debug("get_quote_uniswap")
         try:
-            order_path_dex = [asset_out_address, asset_in_address]
-            router_instance = await self.router()
-            get_amount = router_instance.functions.getAmountsOut(
-                amount,
-                order_path_dex).call()
-            self.logger.debug("get_amount: %s", get_amount)
-            return get_amount[1]
+            # order_path_dex = [asset_out_address, asset_in_address]
+            # router_instance = await self.router()
+            # get_amount = router_instance.functions.getAmountsIn(
+            #     amount,
+            #     order_path_dex).call()
+            # self.logger.debug("get_amount: %s", get_amount)
+            # return get_amount[0]
+            self.uniswap.get_price_output(
+                token0=asset_out_address,
+                token1=asset_in_address,
+                qty=amount)
         except Exception as e:
-            self.logger.error("get_quote_uniswap_v2 %s", e)
+            self.logger.error("get_quote_uniswap %s", e)
             return
 
     async def get_approve_uniswap(self, asset_out_address):
 
         try:
             asset_out_abi = await self.get_abi(asset_out_address)
             asset_out_contract = self.w3.eth.contract(
@@ -590,47 +597,39 @@
                         timeout=120,
                         poll_latency=0.1))
                 return approval_txHash_complete
         except Exception as e:
             self.logger.error("get_approve_uniswap %s", e)
             return None
 
-    async def get_swap_uniswap_v2(
+    async def get_swap_uniswap(
         self,
         asset_out_address,
         asset_in_address,
         amount
     ):
-        order_path_dex = [asset_out_address, asset_in_address]
-
-        deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
-        order_min_amount = self.get_quote_uniswap_v2(
-            asset_in_address,
-            asset_out_address)
-        router_instance = await self.router()
-        swap_order = router_instance.functions.swapExactTokensForTokens(
-                        amount,
-                        order_min_amount,
-                        order_path_dex,
-                        self.wallet_address,
-                        deadline)
-        return swap_order
-
-# uniswap v3 🦄
-    async def get_quote_uniswap_v3(
-        self,
-        asset_in_address,
-        asset_out_address,
-        amount=1
-    ):
-        return
-
-    async def get_swap_uniswap_v3(self):
-        self.logger.warning("Not available")
-        return
+        return self.uniswap(
+            input_token=asset_in_address,
+            output_token=asset_out_address,
+            qty=amount
+        )
+        # order_path_dex = [asset_out_address, asset_in_address]
+
+        # deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
+        # order_min_amount = self.get_quote_uniswap_v2(
+        #     asset_in_address,
+        #     asset_out_address)
+        # router_instance = await self.router()
+        # swap_order = router_instance.functions.swapExactTokensForTokens(
+        #                 amount,
+        #                 order_min_amount,
+        #                 order_path_dex,
+        #                 self.wallet_address,
+        #                 deadline)
+        # return swap_order
 
 # 0️⃣x
     async def get_quote_0x(
         self,
         asset_in_address,
         asset_out_address,
         amount=1
```

### Comparing `dxsp-2.2.2/pyproject.toml` & `dxsp-2.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.2.2"
+version = "2.2.3"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
@@ -14,14 +14,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 asyncio = "*"
 dynaconf = "*"
 web3 = ">=6.0.0"
 pycoingecko = "*"
+uniswap-python = "*"
 
 #web3-ethereum-defi = "*"
 # web3client = ">=1.1.8"
 # # many-abis = ">=0.1.7"
 # apollox-connector-python = "*"
```

### Comparing `dxsp-2.2.2/PKG-INFO` & `dxsp-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.2.2
+Version: 2.2.3
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: asyncio
 Requires-Dist: dynaconf
 Requires-Dist: pycoingecko
+Requires-Dist: uniswap-python
 Requires-Dist: web3 (>=6.0.0)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
 
 # DXSP (DeX SwaP)
```

