# Comparing `tmp/dexie_rewards-0.0.2.tar.gz` & `tmp/dexie_rewards-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexie_rewards-0.0.2.tar", max compression
+gzip compressed data, was "dexie_rewards-0.0.3.tar", max compression
```

## Comparing `dexie_rewards-0.0.2.tar` & `dexie_rewards-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-0.0.2/LICENSE
--rw-r--r--   0        0        0     9721 2023-05-04 04:25:10.558427 dexie_rewards-0.0.2/README.md
--rw-r--r--   0        0        0      643 2023-05-04 04:23:49.780610 dexie_rewards-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-0.0.2/src/dexie_rewards/__init__.py
--rw-r--r--   0        0        0     1048 2023-05-02 08:44:23.928205 dexie_rewards-0.0.2/src/dexie_rewards/config.py
--rw-r--r--   0        0        0     1133 2023-05-02 08:44:23.929217 dexie_rewards-0.0.2/src/dexie_rewards/decorators/with_wallet_rpc_client.py
--rw-r--r--   0        0        0      272 2023-05-04 04:08:54.737867 dexie_rewards-0.0.2/src/dexie_rewards/main.py
--rw-r--r--   0        0        0     2866 2023-05-02 08:44:23.931726 dexie_rewards-0.0.2/src/dexie_rewards/rewards/claim.py
--rw-r--r--   0        0        0     1122 2023-05-02 08:44:23.929570 dexie_rewards-0.0.2/src/dexie_rewards/rewards/list.py
--rw-r--r--   0        0        0      310 2023-05-02 08:44:23.932210 dexie_rewards-0.0.2/src/dexie_rewards/rewards/main.py
--rw-r--r--   0        0        0     2596 2023-05-02 08:44:23.931954 dexie_rewards-0.0.2/src/dexie_rewards/rewards/utils.py
--rw-r--r--   0        0        0     2329 2023-05-02 08:44:23.936658 dexie_rewards-0.0.2/src/dexie_rewards/services/dexie_api.py
--rw-r--r--   0        0        0     1224 2023-05-02 08:44:23.935671 dexie_rewards-0.0.2/src/dexie_rewards/services/wallet_rpc_client.py
--rw-r--r--   0        0        0     1606 2023-05-02 08:44:23.935051 dexie_rewards-0.0.2/src/dexie_rewards/utils.py
--rw-r--r--   0        0        0    10432 1970-01-01 00:00:00.000000 dexie_rewards-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-0.0.3/LICENSE
+-rw-r--r--   0        0        0    11174 2023-05-09 13:47:59.047352 dexie_rewards-0.0.3/README.md
+-rw-r--r--   0        0        0      768 2023-05-12 08:42:06.871508 dexie_rewards-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-0.0.3/src/dexie_rewards/__init__.py
+-rw-r--r--   0        0        0     1111 2023-05-09 06:30:09.411906 dexie_rewards-0.0.3/src/dexie_rewards/config.py
+-rw-r--r--   0        0        0      636 2023-05-11 04:08:59.600900 dexie_rewards-0.0.3/src/dexie_rewards/decorators/with_db_connection.py
+-rw-r--r--   0        0        0     1207 2023-05-11 04:12:56.210275 dexie_rewards-0.0.3/src/dexie_rewards/decorators/with_wallet_rpc_client.py
+-rw-r--r--   0        0        0      234 2023-05-08 10:51:08.009870 dexie_rewards-0.0.3/src/dexie_rewards/main.py
+-rw-r--r--   0        0        0     3190 2023-05-12 08:22:12.370698 dexie_rewards-0.0.3/src/dexie_rewards/rewards/claim.py
+-rw-r--r--   0        0        0     1260 2023-05-09 13:38:34.024504 dexie_rewards-0.0.3/src/dexie_rewards/rewards/list.py
+-rw-r--r--   0        0        0      272 2023-05-08 10:18:31.545940 dexie_rewards-0.0.3/src/dexie_rewards/rewards/main.py
+-rw-r--r--   0        0        0     4500 2023-05-12 08:41:27.306106 dexie_rewards-0.0.3/src/dexie_rewards/rewards/utils.py
+-rw-r--r--   0        0        0     2292 2023-05-09 13:07:18.656197 dexie_rewards-0.0.3/src/dexie_rewards/services/dexie_api.py
+-rw-r--r--   0        0        0     4530 2023-05-12 08:20:37.855585 dexie_rewards-0.0.3/src/dexie_rewards/services/dexie_db.py
+-rw-r--r--   0        0        0     1713 2023-05-11 04:36:56.173403 dexie_rewards-0.0.3/src/dexie_rewards/services/wallet_rpc_client.py
+-rw-r--r--   0        0        0      911 2023-05-09 07:34:28.541774 dexie_rewards-0.0.3/src/dexie_rewards/types/offer_reward.py
+-rw-r--r--   0        0        0      229 2023-05-09 11:06:14.984159 dexie_rewards-0.0.3/src/dexie_rewards/types/utils.py
+-rw-r--r--   0        0        0     1863 2023-05-09 13:39:30.466958 dexie_rewards-0.0.3/src/dexie_rewards/utils.py
+-rw-r--r--   0        0        0    11929 1970-01-01 00:00:00.000000 dexie_rewards-0.0.3/PKG-INFO
```

### Comparing `dexie_rewards-0.0.2/LICENSE` & `dexie_rewards-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.2/pyproject.toml` & `dexie_rewards-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 [tool.poetry]
 name = "dexie-rewards"
-version = "0.0.2"
+version = "0.0.3"
 description = "An open source Python tool which runs locally and will automatically claim rewards for all your created offers on dexie."
 authors = ["Dexie Contributors <pypi@dexie.space>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "dexie_rewards", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 rich-click = "^1.6.1"
 aiomisc = "^17.0.9"
 aiohttp = "^3.8.4"
 based58 = "^0.1.1"
 chia-blockchain = "1.8.*"
+aiosqlite = "^0.17.0"
 
 [tool.poetry.scripts]
 dexie = "dexie_rewards.main:dexie_cmd"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+mypy = "^1.2.0"
+types-setuptools = "^67.7.0.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dexie_rewards-0.0.2/src/dexie_rewards/config.py` & `dexie_rewards-0.0.3/src/dexie_rewards/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,7 +28,9 @@
 dexie_api_testnet = "https://api-testnet.dexie.space/v1"
 dexie_api_local = "http://localhost:3001/v1"
 
 dexie_api_url = os.environ.get(
     "DEXIE_API_URL",
     dexie_api_mainnet if selected_network == "mainnet" else dexie_api_testnet,
 )
+
+dexie_db_path = os.environ.get("DEXIE_DB_PATH", "./dexie.db")
```

### Comparing `dexie_rewards-0.0.2/src/dexie_rewards/decorators/with_wallet_rpc_client.py` & `dexie_rewards-0.0.3/src/dexie_rewards/decorators/with_wallet_rpc_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,35 +3,33 @@
 import sys
 from typing import Any, Dict
 
 from chia.util.ints import uint16
 from chia.rpc.wallet_rpc_client import WalletRpcClient
 
 
-async def run_rpc(rpc_client, f, *args, **kwargs):
+async def run_rpc(rpc_client, f, *args, **kwargs):  # type: ignore
     try:
         result = await f(rpc_client, *args, **kwargs)
     except Exception:
         raise
     finally:
         rpc_client.close()
         await rpc_client.await_closed()
     return result
 
 
-def with_wallet_rpc_client(
-    self_hostname: str, rpc_port: uint16, chia_root: Path, chia_config: Dict[str, Any]
-):
-    def _with_wallet_rpc_client(f):
-        async def with_rpc_client(*args, **kwargs):
+def with_wallet_rpc_client(self_hostname: str, rpc_port: uint16, chia_root: Path, chia_config: Dict[str, Any]):  # type: ignore
+    def _with_wallet_rpc_client(f):  # type: ignore
+        async def with_rpc_client(*args, **kwargs):  # type: ignore
             try:
                 rpc_client = await WalletRpcClient.create(
                     self_hostname, rpc_port, chia_root, chia_config
                 )
-                return await run_rpc(rpc_client, f, *args, **kwargs)
+                return await run_rpc(rpc_client, f, *args, **kwargs)  # type: ignore
             except Exception:
                 Console(stderr=True, style="bold red").print(
                     "Unable to connect to wallet"
                 )
                 sys.exit(1)
 
         return with_rpc_client
```

### Comparing `dexie_rewards-0.0.2/src/dexie_rewards/rewards/list.py` & `dexie_rewards-0.0.3/src/dexie_rewards/rewards/list.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import asyncio
 import json
 import rich_click as click
 
 from rich.console import Console
 
+from typing import Optional
+
+from ..services.dexie_db import create_db
+from ..types.offer_reward import OfferReward
 from ..utils import wait_for_synced_wallet
 from .utils import display_rewards, get_offers_with_claimable_rewards
 
 console = Console()
 
 
 @click.command("list", short_help="List all offers with dexie rewards")
 @click.option(
     "-f",
     "--fingerprint",
-    required=True,
+    required=False,
     help="Set the fingerprint to specify which wallet to use",
     type=int,
 )
 @click.option(
     "-j",
     "--json",
     "as_json",
     help="Displays offers as JSON",
     is_flag=True,
     default=False,
     show_default=True,
 )
-@click.pass_context
-def list_cmds(ctx: click.Context, fingerprint, as_json):
+def list_cmds(fingerprint: Optional[int], as_json: bool) -> None:
     asyncio.run(list_cmds_async(fingerprint, as_json))
 
 
-async def list_cmds_async(fingerprint, as_json):
-    await wait_for_synced_wallet(fingerprint)
+async def list_cmds_async(fingerprint: Optional[int], as_json: bool) -> None:
+    await create_db()
+
+    await wait_for_synced_wallet(fingerprint, as_json)
 
-    offers_rewards = await get_offers_with_claimable_rewards()
+    offers_rewards_dict = await get_offers_with_claimable_rewards()
     if as_json:
-        click.echo(json.dumps(offers_rewards))
+        click.echo(json.dumps(offers_rewards_dict))
     else:
-        if len(offers_rewards) == 0:
-            console.print("No rewards to claim", style="bold red")
-            return
+        offers_rewards = list(map(OfferReward.from_json_dict, offers_rewards_dict))
         display_rewards(offers_rewards)
```

### Comparing `dexie_rewards-0.0.2/src/dexie_rewards/services/dexie_api.py` & `dexie_rewards-0.0.3/src/dexie_rewards/services/dexie_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import aiohttp
 import based58
 import dataclasses
 import hashlib
+from typing import Any, Dict, Optional
 
 from chia.wallet.trading.offer import Offer
 
 
-# https://github.com/dexie-space/dexie-api/blob/036d6af21e33afe807534fab9668dfe66f08d594/src/offers/utils.ts#L16
 def get_dexie_bs58_offer_hash(offer: Offer) -> str:
     m = hashlib.sha256()
     m.update(bytes(offer.to_bech32(), "utf-8"))
     offer_hash = m.hexdigest()
     offer_hash_bs58 = based58.b58encode(bytes.fromhex(offer_hash))
     return offer_hash_bs58.decode("utf-8")
 
@@ -46,27 +46,27 @@
         ):
             if not rep.ok:
                 raise RuntimeError(rep.reason)
             return await rep.json()
 
     async def get_offers_with_claimable_rewards(
         self, offer_ids: list[str]
-    ) -> list[Offer]:
+    ) -> Dict[str, Any]:
         async with (
             aiohttp.ClientSession() as session,
             session.post(
                 f"{self.base_url}/checkRewards", json={"ids": offer_ids}
             ) as rep,
         ):
             if not rep.ok:
                 raise RuntimeError(rep.reason)
             return await rep.json()
 
     # claim rewards
-    async def claim_rewards(self, claims_payload):
+    async def claim_rewards(self, claims_payload: Dict[str, Any]) -> Dict[str, Any]:
         async with (
             aiohttp.ClientSession() as session,
             session.post(f"{self.base_url}/claimRewards", json=claims_payload) as rep,
         ):
             if not rep.ok:
                 raise RuntimeError(rep.reason)
             return await rep.json()
```

### Comparing `dexie_rewards-0.0.2/src/dexie_rewards/services/wallet_rpc_client.py` & `dexie_rewards-0.0.3/src/dexie_rewards/services/wallet_rpc_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,47 @@
+from typing import List, Tuple
+
+from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.rpc.wallet_rpc_client import WalletRpcClient
 from chia.util.bech32m import encode_puzzle_hash
-
+from chia.wallet.trade_record import TradeRecord
 
 from ..config import (
     address_prefix,
     chia_config,
     chia_root,
     self_hostname,
     wallet_rpc_port,
 )
 from ..decorators.with_wallet_rpc_client import with_wallet_rpc_client
 
 
 @with_wallet_rpc_client(self_hostname, wallet_rpc_port, chia_root, chia_config)
-async def log_in(wallet_rpc_client: WalletRpcClient, fingerprint):
-    return await wallet_rpc_client.log_in(fingerprint)
+async def get_logged_in_fingerprint(
+    wallet_rpc_client: WalletRpcClient,
+) -> int:
+    return await wallet_rpc_client.get_logged_in_fingerprint()
+
+
+@with_wallet_rpc_client(self_hostname, wallet_rpc_port, chia_root, chia_config)
+async def log_in(wallet_rpc_client: WalletRpcClient, fingerprint: int) -> None:
+    await wallet_rpc_client.log_in(fingerprint)
 
 
 @with_wallet_rpc_client(self_hostname, wallet_rpc_port, chia_root, chia_config)
-async def get_synced(wallet_rpc_client: WalletRpcClient):
+async def get_synced(wallet_rpc_client: WalletRpcClient) -> bool:
     return await wallet_rpc_client.get_synced()
 
 
 @with_wallet_rpc_client(self_hostname, wallet_rpc_port, chia_root, chia_config)
-async def get_all_offers(wallet_rpc_client: WalletRpcClient):
-    return await wallet_rpc_client.get_all_offers(file_contents=True)
+async def get_all_offers(wallet_rpc_client: WalletRpcClient) -> List[TradeRecord]:
+    return await wallet_rpc_client.get_all_offers(
+        include_completed=True, file_contents=True
+    )
 
 
 @with_wallet_rpc_client(self_hostname, wallet_rpc_port, chia_root, chia_config)
 async def sign_message_by_puzzle_hash(
-    wallet_rpc_client: WalletRpcClient, puzzle_hash, message
-):
-    address = encode_puzzle_hash(puzzle_hash, address_prefix)
+    wallet_rpc_client: WalletRpcClient, puzzle_hash: bytes32, message: str
+) -> Tuple[str, str, str]:
+    address: str = encode_puzzle_hash(puzzle_hash, address_prefix)
     return await wallet_rpc_client.sign_message_by_address(address, message)
```

### Comparing `dexie_rewards-0.0.2/src/dexie_rewards/utils.py` & `dexie_rewards-0.0.3/src/dexie_rewards/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from rich.console import Console
 from rich.progress import (
-    Column,
     Progress,
     SpinnerColumn,
     TextColumn,
     TimeElapsedColumn,
 )
 import time
 
@@ -24,25 +23,32 @@
     calculate_synthetic_secret_key,
     DEFAULT_HIDDEN_PUZZLE_HASH,
 )
 
 from .services import wallet_rpc_client as wallet_rpc_client
 
 
-async def is_wallet_synced(fingerprint):
+async def is_wallet_synced(fingerprint: int) -> bool:
     await wallet_rpc_client.log_in(fingerprint)
 
     is_synced = await wallet_rpc_client.get_synced()
     if is_synced:
         return True
 
     return False
 
 
-async def wait_for_synced_wallet(fingerprint):
+async def wait_for_synced_wallet(
+    fingerprint: Optional[int], as_json: bool = False
+) -> None:
+    if fingerprint is None:
+        fingerprint = await wallet_rpc_client.get_logged_in_fingerprint()
+        if not as_json:
+            Console().print(f"Using wallet with fingerprint: {fingerprint}")
+
     await wallet_rpc_client.log_in(fingerprint)
     syncing_wallet_progress = Progress(
         TextColumn("{task.description}"),
         SpinnerColumn("dots8Bit"),
         TimeElapsedColumn(),
         transient=True,
     )
```

### Comparing `dexie_rewards-0.0.2/PKG-INFO` & `dexie_rewards-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dexie-rewards
-Version: 0.0.2
+Version: 0.0.3
 Summary: An open source Python tool which runs locally and will automatically claim rewards for all your created offers on dexie.
 License: Apache-2.0
 Author: Dexie Contributors
 Author-email: pypi@dexie.space
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: aiomisc (>=17.0.9,<18.0.0)
+Requires-Dist: aiosqlite (>=0.17.0,<0.18.0)
 Requires-Dist: based58 (>=0.1.1,<0.2.0)
 Requires-Dist: chia-blockchain (>=1.8.0,<1.9.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 ## Overview
 
@@ -76,20 +77,19 @@
 ```sh
 ❯ dexie --help
 
  Usage: dexie [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ─────────────────────────────────────────────────────────────────────────────────────╮
 │ --version      Show the version and exit.                                                     │
-│ --help      Show this message and exit.                                                       │
+│ --help         Show this message and exit.                                                    │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ────────────────────────────────────────────────────────────────────────────────────╮
 │ rewards           Manage your dexie rewards for offers                                        │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────╯
-
 ```
 
 ### Rewards
 
 ```sh
 ❯ dexie rewards --help
 
@@ -98,106 +98,124 @@
 ╭─ Options ─────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                       │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ────────────────────────────────────────────────────────────────────────────────────╮
 │ claim          Claim all offers with dexie rewards                                            │
 │ list           List all offers with dexie rewards                                             │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────╯
-
 ```
 
 #### list
 
 ```sh
 ❯ dexie rewards list --help
 
  Usage: dexie rewards list [OPTIONS]
 
 ╭─ Options ─────────────────────────────────────────────────────────────────────────────────────╮
-│ *  --fingerprint  -f  INTEGER  Set the fingerprint to specify which wallet to use [required]  │
-│    --json         -j           Displays offers as JSON                                        │
-│    --help                      Show this message and exit.                                    │
+│ --fingerprint  -f  INTEGER  Set the fingerprint to specify which wallet to use                │
+│ --json         -j           Displays offers as JSON                                           │
+│ --help                      Show this message and exit.                                       │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────╯
 
+❯ dexie rewards list
+Using wallet with fingerprint: 518185849
+╭──────────────────────────────────────────────┬───────────────╮
+│                    Offer                     │ Rewards (DBX) │
+├──────────────────────────────────────────────┼───────────────┤
+│ CWkZDUURQioPtKjF2zWUHqf6vxEQDhjEnCk6TJqoTpPe │         0.864 │
+│ J12qwA7fAC2jFm7AjNB2H7DKRzZ2ajfbMBygnRrhjrVM │         0.126 │
+│ 5gkKdAg93TbnUSSJLbhCEhWw9zHXWMxggWQmshQiKUuP │         0.805 │
+├──────────────────────────────────────────────┼───────────────┤
+│      Found 3 offers with total rewards       │         1.795 │
+╰──────────────────────────────────────────────┴───────────────╯
 
-❯ dexie rewards list -f 2149823282 --json | jq
+❯ dexie rewards list -f 518185849 --json | jq
 [
   {
-    "id": "9D1P2oTKhLveYosRiksTczSjX9pW6okAvNL5XVQEwHsD",
+    "id": "CWkZDUURQioPtKjF2zWUHqf6vxEQDhjEnCk6TJqoTpPe",
     "status": 0,
-    "date_found": "2023-04-22T03:38:50.363Z",
-    "date_rewards_since": "2023-04-24T08:52:48.366Z",
-    "maker_puzzle_hash": "0x1aa36967f74dfc0b85996e9adbe2e646c507b34644c1e17501d790b3838dbdd4",
-    "claimable_rewards": 0.669
+    "date_found": "2023-05-08T13:31:49.033Z",
+    "date_rewards_since": "2023-05-08T13:32:24.623Z",
+    "maker_puzzle_hash": "0xe762f668c631ec2bd6f909cfdfc42d56a281e5e5be03bd8a021900ecb6917d78",
+    "claimable_rewards": 0.864
   },
   {
-    "id": "BSqJs63Pf1DV4kBc2hTv8G9ZFgytMbWWtkoLnCmzu1LV",
-    "status": 0,
-    "date_found": "2023-04-22T03:38:19.712Z",
-    "date_rewards_since": "2023-04-24T08:52:48.366Z",
-    "maker_puzzle_hash": "0x1aa36967f74dfc0b85996e9adbe2e646c507b34644c1e17501d790b3838dbdd4",
-    "claimable_rewards": 0.9
+    "id": "J12qwA7fAC2jFm7AjNB2H7DKRzZ2ajfbMBygnRrhjrVM",
+    "status": 4,
+    "date_found": "2023-05-08T10:26:28.083Z",
+    "date_rewards_since": "2023-05-08T10:33:05.237Z",
+    "maker_puzzle_hash": "0xe762f668c631ec2bd6f909cfdfc42d56a281e5e5be03bd8a021900ecb6917d78",
+    "claimable_rewards": 0.126
+  },
+  {
+    "id": "5gkKdAg93TbnUSSJLbhCEhWw9zHXWMxggWQmshQiKUuP",
+    "status": 4,
+    "date_found": "2023-05-08T10:24:42.258Z",
+    "date_rewards_since": "2023-05-08T10:25:05.167Z",
+    "maker_puzzle_hash": "0xe762f668c631ec2bd6f909cfdfc42d56a281e5e5be03bd8a021900ecb6917d78",
+    "claimable_rewards": 0.805
   }
 ]
-
-❯ dexie rewards list -f 2149823282
-╭──────────────────────────────────────────────┬───────────────╮
-│                    Offer                     │ Rewards (DBX) │
-├──────────────────────────────────────────────┼───────────────┤
-│ 9D1P2oTKhLveYosRiksTczSjX9pW6okAvNL5XVQEwHsD │         0.669 │
-│ BSqJs63Pf1DV4kBc2hTv8G9ZFgytMbWWtkoLnCmzu1LV │         0.900 │
-╰──────────────────────────────────────────────┴───────────────╯
 ```
 
 #### claim
 
 ```sh
 ❯ dexie rewards claim --help
 
  Usage: dexie rewards claim [OPTIONS]
 
 ╭─ Options ─────────────────────────────────────────────────────────────────────────────────────╮
-│ *  --fingerprint  -f   INTEGER  Set the fingerprint to specify which wallet to use [required] │
-│    --verify-only  -vo           Only verify the claim, don't actually claim                   │
-│    --yes          -y            Skip claim confirmation                                       │
-│    --verbose      -v            Display verbose output                                        │
-│    --help                       Show this message and exit.                                   │
+│ --fingerprint  -f   INTEGER  Set the fingerprint to specify which wallet to use               │
+│ --verify-only  -vo           Only verify the claim, don't actually claim                      │
+│ --yes          -y            Skip claim confirmation                                          │
+│ --verbose      -v            Display verbose output                                           │
+│ --help                       Show this message and exit.                                      │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────╯
 
-
-
-❯ dexie rewards claim -f 2149823282 --verbose
+❯ dexie rewards claim -f 518185849 --verbose
 ╭──────────────────────────────────────────────┬───────────────╮
 │                    Offer                     │ Rewards (DBX) │
 ├──────────────────────────────────────────────┼───────────────┤
-│ 9D1P2oTKhLveYosRiksTczSjX9pW6okAvNL5XVQEwHsD │         0.669 │
-│ BSqJs63Pf1DV4kBc2hTv8G9ZFgytMbWWtkoLnCmzu1LV │         0.900 │
+│ CWkZDUURQioPtKjF2zWUHqf6vxEQDhjEnCk6TJqoTpPe │         0.864 │
+│ J12qwA7fAC2jFm7AjNB2H7DKRzZ2ajfbMBygnRrhjrVM │         0.126 │
+│ 5gkKdAg93TbnUSSJLbhCEhWw9zHXWMxggWQmshQiKUuP │         0.805 │
+├──────────────────────────────────────────────┼───────────────┤
+│      Found 3 offers with total rewards       │         1.795 │
 ╰──────────────────────────────────────────────┴───────────────╯
-Total Rewards: 1.569 DBX
 Claim all? [y/n]: y
 
 claims request payload:
 {
   "claims": [
     {
-      "offer_id": "9D1P2oTKhLveYosRiksTczSjX9pW6okAvNL5XVQEwHsD",
-      "signature": "a911020f0d60082bda371c0237f4d81797ac868ca8f6fcf71b5477857802543f9aba7b85f7a8240ba2afaf60c3449c66105f33b7a5511b3fb75296aa33f33c517aed9ce8544e513235745818597d10d8889b103307a5c507d1638e724bad0ce5",
-      "public_key": "b9ea173a4a26f6bd5b372ac9a559ede742a44578d8f17a7ca631f1a9a1e5257b0ba4a78ec4edb65532b949c1a0d3866d"
+      "offer_id": "CWkZDUURQioPtKjF2zWUHqf6vxEQDhjEnCk6TJqoTpPe",
+      "signature": "8c46a42998ad7089a50d3b92bb194a4d3ded1d3f9ae7911949ae561e48076d05eb11817e65984dec9c746d9bb17da1c714c0138a7fa36a057388e5df247d3309723ec28e3e0b84bde6f927f1ead77e5bdae0ecf855ffd838798ef74dc06f1d46",
+      "public_key": "b3406aa1620c09fa9c653019c1f071c330a69829d3adfd4eb735e4518ca9717e9f47e66902e06fa9beb9d3d026acb042"
+    },
+    {
+      "offer_id": "J12qwA7fAC2jFm7AjNB2H7DKRzZ2ajfbMBygnRrhjrVM",
+      "signature": "abf567d26a5332461daf404c6482c9214b5f6955b87cffaad1290a96d7bb0184317e8963a5b44a19ca9b159a6c80137502bf2f83531adec8b1a5d22b118624b3ba06a676f0f2fa05d3cd533eb3d74c097b6cf9cd4e4d515fa1160b6dc565e817",
+      "public_key": "b3406aa1620c09fa9c653019c1f071c330a69829d3adfd4eb735e4518ca9717e9f47e66902e06fa9beb9d3d026acb042"
     },
     {
-      "offer_id": "BSqJs63Pf1DV4kBc2hTv8G9ZFgytMbWWtkoLnCmzu1LV",
-      "signature": "80ef07c8156b07731bd4dd647b32de47ad0831581765963eaff619f5bdf7b2a05666db7d8da742c24b6d3055f9555f9f07ad51b4ac6ddc75d6644d4f5854195e7c45f0e42aba45033ea2257a528ed60e61084598e1513eba074c39e831832236",
-      "public_key": "b9ea173a4a26f6bd5b372ac9a559ede742a44578d8f17a7ca631f1a9a1e5257b0ba4a78ec4edb65532b949c1a0d3866d"
+      "offer_id": "5gkKdAg93TbnUSSJLbhCEhWw9zHXWMxggWQmshQiKUuP",
+      "signature": "a17eedb2d8f0ad31c1ad93de4a288bcb85241c952d2b0fb2d1d583aec6d1f8b858858055c4893a3b6d23283e590dc9a302fac5e434e5e0800337c872f3efd50542f1140298e8e4e29e80b1100d164f33248a38d2efbe53f124d3772205160d72",
+      "public_key": "b3406aa1620c09fa9c653019c1f071c330a69829d3adfd4eb735e4518ca9717e9f47e66902e06fa9beb9d3d026acb042"
     }
   ]
 }
 
 claims result:
 {
   "success": true,
   "verified_amount": {
-    "9D1P2oTKhLveYosRiksTczSjX9pW6okAvNL5XVQEwHsD": 0.669,
-    "BSqJs63Pf1DV4kBc2hTv8G9ZFgytMbWWtkoLnCmzu1LV": 0.9
+    "CWkZDUURQioPtKjF2zWUHqf6vxEQDhjEnCk6TJqoTpPe": 0.864,
+    "J12qwA7fAC2jFm7AjNB2H7DKRzZ2ajfbMBygnRrhjrVM": 0.126,
+    "5gkKdAg93TbnUSSJLbhCEhWw9zHXWMxggWQmshQiKUuP": 0.805
   }
 }
+
+
 ```
```

