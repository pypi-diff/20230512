# Comparing `tmp/pyln_testing-23.2.tar.gz` & `tmp/pyln-testing-23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyln_testing-23.2.tar", max compression
+gzip compressed data, was "pyln-testing-23.5.tar", max compression
```

## Comparing `pyln_testing-23.2.tar` & `pyln-testing-23.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1138 2023-03-03 15:54:49.825873 pyln_testing-23.2/README.md
--rw-r--r--   0        0        0       56 2023-03-03 15:54:49.825873 pyln_testing-23.2/pyln/testing/__init__.py
--rw-r--r--   0        0        0     4005 2023-03-03 15:54:49.825873 pyln_testing-23.2/pyln/testing/btcproxy.py
--rw-r--r--   0        0        0     7452 2023-03-03 15:54:49.825873 pyln_testing-23.2/pyln/testing/db.py
--rw-r--r--   0        0        0    21397 2023-03-03 15:54:49.825873 pyln_testing-23.2/pyln/testing/fixtures.py
--rw-r--r--   0        0        0    13033 2023-03-03 15:54:49.825873 pyln_testing-23.2/pyln/testing/gossip.py
--rw-r--r--   0        0        0    10117 2023-03-03 15:54:49.825873 pyln_testing-23.2/pyln/testing/grpc.py
--rw-r--r--   0        0        0    44640 2023-03-03 15:54:49.825873 pyln_testing-23.2/pyln/testing/grpc2py.py
--rw-r--r--   0        0        0   128401 2023-03-03 15:54:49.825873 pyln_testing-23.2/pyln/testing/node_pb2.py
--rw-r--r--   0        0        0    73128 2023-03-03 15:54:49.825873 pyln_testing-23.2/pyln/testing/node_pb2_grpc.py
--rw-r--r--   0        0        0     8060 2023-03-03 15:54:49.825873 pyln_testing-23.2/pyln/testing/primitives_pb2.py
--rw-r--r--   0        0        0    60159 2023-03-03 15:54:49.825873 pyln_testing-23.2/pyln/testing/utils.py
--rw-r--r--   0        0        0      764 2023-03-03 15:54:49.825873 pyln_testing-23.2/pyproject.toml
--rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 pyln_testing-23.2/setup.py
--rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 pyln_testing-23.2/PKG-INFO
+-rw-r--r--   0        0        0     1138 2023-05-11 17:43:49.805160 pyln-testing-23.5/README.md
+-rw-r--r--   0        0        0       56 2023-05-11 17:43:49.805160 pyln-testing-23.5/pyln/testing/__init__.py
+-rw-r--r--   0        0        0     4005 2023-05-11 17:43:49.805160 pyln-testing-23.5/pyln/testing/btcproxy.py
+-rw-r--r--   0        0        0     7452 2023-05-11 17:43:49.805160 pyln-testing-23.5/pyln/testing/db.py
+-rw-r--r--   0        0        0    21280 2023-05-11 17:43:49.805160 pyln-testing-23.5/pyln/testing/fixtures.py
+-rw-r--r--   0        0        0    13033 2023-05-11 17:43:49.805160 pyln-testing-23.5/pyln/testing/gossip.py
+-rw-r--r--   0        0        0    10117 2023-05-11 17:43:49.805160 pyln-testing-23.5/pyln/testing/grpc.py
+-rw-r--r--   0        0        0    71164 2023-05-11 17:55:35.731224 pyln-testing-23.5/pyln/testing/grpc2py.py
+-rw-r--r--   0        0        0   164092 2023-05-11 17:43:49.805160 pyln-testing-23.5/pyln/testing/node_pb2.py
+-rw-r--r--   0        0        0    79161 2023-05-11 17:43:49.805160 pyln-testing-23.5/pyln/testing/node_pb2_grpc.py
+-rw-r--r--   0        0        0     8941 2023-05-11 17:43:49.805160 pyln-testing-23.5/pyln/testing/primitives_pb2.py
+-rw-r--r--   0        0        0    62390 2023-05-11 17:43:49.805160 pyln-testing-23.5/pyln/testing/utils.py
+-rw-r--r--   0        0        0      764 2023-05-11 17:43:49.805160 pyln-testing-23.5/pyproject.toml
+-rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 pyln-testing-23.5/setup.py
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 pyln-testing-23.5/PKG-INFO
```

### Comparing `pyln_testing-23.2/README.md` & `pyln-testing-23.5/README.md`

 * *Files identical despite different names*

### Comparing `pyln_testing-23.2/pyln/testing/btcproxy.py` & `pyln-testing-23.5/pyln/testing/btcproxy.py`

 * *Files identical despite different names*

### Comparing `pyln_testing-23.2/pyln/testing/db.py` & `pyln-testing-23.5/pyln/testing/db.py`

 * *Files identical despite different names*

### Comparing `pyln_testing-23.2/pyln/testing/fixtures.py` & `pyln-testing-23.5/pyln/testing/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from concurrent import futures
 from pyln.testing.db import SqliteDbProvider, PostgresDbProvider
-from pyln.testing.utils import NodeFactory, BitcoinD, ElementsD, env, DEVELOPER, LightningNode, TEST_DEBUG, Throttler
+from pyln.testing.utils import NodeFactory, BitcoinD, ElementsD, env, DEVELOPER, LightningNode, TEST_DEBUG
 from pyln.client import Millisatoshi
 from typing import Dict
 
 import json
 import jsonschema  # type: ignore
 import logging
 import os
@@ -202,19 +202,14 @@
 
     if errors.has_errors():
         # Format a nice list of everything that went wrong and raise an exception
         request.node.has_errors = True
         raise ValueError(str(errors))
 
 
-@pytest.fixture
-def throttler(test_base_dir):
-    yield Throttler(test_base_dir)
-
-
 def _extra_validator(is_request: bool):
     """JSON Schema validator with additions for our specialized types"""
     def is_hex(checker, instance):
         """Hex string"""
         if not checker.is_type(instance, "string"):
             return False
         return all(c in string.hexdigits for c in instance)
@@ -296,15 +291,15 @@
 
     def is_feerate(checker, instance):
         """feerate string or number (optionally ending in perkw/perkb)"""
         if checker.is_type(instance, "integer"):
             return True
         if not checker.is_type(instance, "string"):
             return False
-        if instance in ("urgent", "normal", "slow"):
+        if instance in ("urgent", "normal", "slow", "minimum"):
             return True
         if instance in ("opening", "mutual_close", "unilateral_close", "delayed_to_us", "htlc_resolution", "penalty", "min_acceptable", "max_acceptable"):
             return True
         if not instance.endswith("perkw") and not instance.endswith("perkb"):
             return False
 
         try:
@@ -349,15 +344,15 @@
         try:
             Millisatoshi(instance)
             return True
         except TypeError:
             return False
 
     def is_msat_response(checker, instance):
-        """String number ending in msat (deprecated) or integer"""
+        """An integer, but we convert to Millisatoshi in JSON parsing"""
         return type(instance) is Millisatoshi
 
     def is_txid(checker, instance):
         """Bitcoin transaction ID"""
         if not checker.is_type(instance, "hex"):
             return False
         return len(instance) == 64
@@ -447,24 +442,23 @@
             schemas[base] = [None, None]
         schemas[base][index] = _load_schema(os.path.join('doc/schemas', fname),
                                             is_request)
     return schemas
 
 
 @pytest.fixture
-def node_factory(request, directory, test_name, bitcoind, executor, db_provider, teardown_checks, node_cls, throttler, jsonschemas):
+def node_factory(request, directory, test_name, bitcoind, executor, db_provider, teardown_checks, node_cls, jsonschemas):
     nf = NodeFactory(
         request,
         test_name,
         bitcoind,
         executor,
         directory=directory,
         db_provider=db_provider,
         node_cls=node_cls,
-        throttler=throttler,
         jsonschemas=jsonschemas,
     )
 
     yield nf
     ok, errs = nf.killall([not n.may_fail for n in nf.nodes])
 
     for e in errs:
```

### Comparing `pyln_testing-23.2/pyln/testing/gossip.py` & `pyln-testing-23.5/pyln/testing/gossip.py`

 * *Files identical despite different names*

### Comparing `pyln_testing-23.2/pyln/testing/grpc.py` & `pyln-testing-23.5/pyln/testing/grpc.py`

 * *Files identical despite different names*

### Comparing `pyln_testing-23.2/pyln/testing/grpc2py.py` & `pyln-testing-23.5/pyln/testing/grpc2py.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 
 import json
 
 
 def hexlify(b):
     return b if b is None else b.hex()
 
+
 def amount2msat(a):
     return a.msat
 
-def amount_or_all2msat(a):
-    breakpoint()
-
 
 def remove_default(d):
     # grpc is really not good at empty values, they get replaced with the type's default value...
     return {k: v for k, v in d.items() if v is not None and v != ""}
 
 
 def getinfo_our_features2py(m):
@@ -55,15 +53,14 @@
         "num_pending_channels": m.num_pending_channels,  # PrimitiveField in generate_composite
         "num_active_channels": m.num_active_channels,  # PrimitiveField in generate_composite
         "num_inactive_channels": m.num_inactive_channels,  # PrimitiveField in generate_composite
         "version": m.version,  # PrimitiveField in generate_composite
         "lightning_dir": m.lightning_dir,  # PrimitiveField in generate_composite
         "blockheight": m.blockheight,  # PrimitiveField in generate_composite
         "network": m.network,  # PrimitiveField in generate_composite
-        "msatoshi_fees_collected": m.msatoshi_fees_collected,  # PrimitiveField in generate_composite
         "fees_collected_msat": amount2msat(m.fees_collected_msat),  # PrimitiveField in generate_composite
         "address": [getinfo_address2py(i) for i in m.address],  # ArrayField[composite] in generate_composite
         "binding": [getinfo_binding2py(i) for i in m.binding],  # ArrayField[composite] in generate_composite
         "warning_bitcoind_sync": m.warning_bitcoind_sync,  # PrimitiveField in generate_composite
         "warning_lightningd_sync": m.warning_lightningd_sync,  # PrimitiveField in generate_composite
     })
 
@@ -96,16 +93,14 @@
         "our_funding_msat": amount2msat(m.our_funding_msat),  # PrimitiveField in generate_composite
         "scratch_txid": hexlify(m.scratch_txid),  # PrimitiveField in generate_composite
     })
 
 
 def listpeers_peers_channels_funding2py(m):
     return remove_default({
-        "local_msat": amount2msat(m.local_msat),  # PrimitiveField in generate_composite
-        "remote_msat": amount2msat(m.remote_msat),  # PrimitiveField in generate_composite
         "pushed_msat": amount2msat(m.pushed_msat),  # PrimitiveField in generate_composite
         "local_funds_msat": amount2msat(m.local_funds_msat),  # PrimitiveField in generate_composite
         "remote_funds_msat": amount2msat(m.remote_funds_msat),  # PrimitiveField in generate_composite
         "fee_paid_msat": amount2msat(m.fee_paid_msat),  # PrimitiveField in generate_composite
         "fee_rcvd_msat": amount2msat(m.fee_rcvd_msat),  # PrimitiveField in generate_composite
     })
 
@@ -219,14 +214,15 @@
         "peer_id": hexlify(m.peer_id),  # PrimitiveField in generate_composite
         "our_amount_msat": amount2msat(m.our_amount_msat),  # PrimitiveField in generate_composite
         "amount_msat": amount2msat(m.amount_msat),  # PrimitiveField in generate_composite
         "funding_txid": hexlify(m.funding_txid),  # PrimitiveField in generate_composite
         "funding_output": m.funding_output,  # PrimitiveField in generate_composite
         "connected": m.connected,  # PrimitiveField in generate_composite
         "state": str(m.state),  # EnumField in generate_composite
+        "channel_id": hexlify(m.channel_id),  # PrimitiveField in generate_composite
         "short_channel_id": m.short_channel_id,  # PrimitiveField in generate_composite
     })
 
 
 def listfunds2py(m):
     return remove_default({
         "outputs": [listfunds_outputs2py(i) for i in m.outputs],  # ArrayField[composite] in generate_composite
@@ -722,36 +718,473 @@
     return remove_default({
         "psbt": m.psbt,  # PrimitiveField in generate_composite
         "tx": hexlify(m.tx),  # PrimitiveField in generate_composite
         "txid": hexlify(m.txid),  # PrimitiveField in generate_composite
     })
 
 
+def listpeerchannels_channels_channel_type2py(m):
+    return remove_default({
+        "bits": [m.bits for i in m.bits], # ArrayField[primitive] in generate_composite
+        "names": [str(i) for i in m.names],  # ArrayField[composite] in generate_composite
+    })
+
+
+def listpeerchannels_channels_feerate2py(m):
+    return remove_default({
+        "perkw": m.perkw,  # PrimitiveField in generate_composite
+        "perkb": m.perkb,  # PrimitiveField in generate_composite
+    })
+
+
+def listpeerchannels_channels_inflight2py(m):
+    return remove_default({
+        "funding_txid": hexlify(m.funding_txid),  # PrimitiveField in generate_composite
+        "funding_outnum": m.funding_outnum,  # PrimitiveField in generate_composite
+        "feerate": m.feerate,  # PrimitiveField in generate_composite
+        "total_funding_msat": amount2msat(m.total_funding_msat),  # PrimitiveField in generate_composite
+        "our_funding_msat": amount2msat(m.our_funding_msat),  # PrimitiveField in generate_composite
+        "scratch_txid": hexlify(m.scratch_txid),  # PrimitiveField in generate_composite
+    })
+
+
+def listpeerchannels_channels_funding2py(m):
+    return remove_default({
+        "pushed_msat": amount2msat(m.pushed_msat),  # PrimitiveField in generate_composite
+        "local_funds_msat": amount2msat(m.local_funds_msat),  # PrimitiveField in generate_composite
+        "remote_funds_msat": amount2msat(m.remote_funds_msat),  # PrimitiveField in generate_composite
+        "fee_paid_msat": amount2msat(m.fee_paid_msat),  # PrimitiveField in generate_composite
+        "fee_rcvd_msat": amount2msat(m.fee_rcvd_msat),  # PrimitiveField in generate_composite
+    })
+
+
+def listpeerchannels_channels_alias2py(m):
+    return remove_default({
+        "local": m.local,  # PrimitiveField in generate_composite
+        "remote": m.remote,  # PrimitiveField in generate_composite
+    })
+
+
+def listpeerchannels_channels_state_changes2py(m):
+    return remove_default({
+        "timestamp": m.timestamp,  # PrimitiveField in generate_composite
+        "old_state": str(m.old_state),  # EnumField in generate_composite
+        "new_state": str(m.new_state),  # EnumField in generate_composite
+        "cause": str(m.cause),  # EnumField in generate_composite
+        "message": m.message,  # PrimitiveField in generate_composite
+    })
+
+
+def listpeerchannels_channels_htlcs2py(m):
+    return remove_default({
+        "direction": str(m.direction),  # EnumField in generate_composite
+        "id": m.id,  # PrimitiveField in generate_composite
+        "amount_msat": amount2msat(m.amount_msat),  # PrimitiveField in generate_composite
+        "expiry": m.expiry,  # PrimitiveField in generate_composite
+        "payment_hash": hexlify(m.payment_hash),  # PrimitiveField in generate_composite
+        "local_trimmed": m.local_trimmed,  # PrimitiveField in generate_composite
+        "status": m.status,  # PrimitiveField in generate_composite
+        "state": str(m.state),  # EnumField in generate_composite
+    })
+
+
+def listpeerchannels_channels2py(m):
+    return remove_default({
+        "peer_id": hexlify(m.peer_id),  # PrimitiveField in generate_composite
+        "peer_connected": m.peer_connected,  # PrimitiveField in generate_composite
+        "state": str(m.state),  # EnumField in generate_composite
+        "scratch_txid": hexlify(m.scratch_txid),  # PrimitiveField in generate_composite
+        "owner": m.owner,  # PrimitiveField in generate_composite
+        "short_channel_id": m.short_channel_id,  # PrimitiveField in generate_composite
+        "channel_id": hexlify(m.channel_id),  # PrimitiveField in generate_composite
+        "funding_txid": hexlify(m.funding_txid),  # PrimitiveField in generate_composite
+        "funding_outnum": m.funding_outnum,  # PrimitiveField in generate_composite
+        "initial_feerate": m.initial_feerate,  # PrimitiveField in generate_composite
+        "last_feerate": m.last_feerate,  # PrimitiveField in generate_composite
+        "next_feerate": m.next_feerate,  # PrimitiveField in generate_composite
+        "next_fee_step": m.next_fee_step,  # PrimitiveField in generate_composite
+        "inflight": [listpeerchannels_channels_inflight2py(i) for i in m.inflight],  # ArrayField[composite] in generate_composite
+        "close_to": hexlify(m.close_to),  # PrimitiveField in generate_composite
+        "private": m.private,  # PrimitiveField in generate_composite
+        "opener": str(m.opener),  # EnumField in generate_composite
+        "closer": str(m.closer),  # EnumField in generate_composite
+        "features": [str(i) for i in m.features],  # ArrayField[composite] in generate_composite
+        "to_us_msat": amount2msat(m.to_us_msat),  # PrimitiveField in generate_composite
+        "min_to_us_msat": amount2msat(m.min_to_us_msat),  # PrimitiveField in generate_composite
+        "max_to_us_msat": amount2msat(m.max_to_us_msat),  # PrimitiveField in generate_composite
+        "total_msat": amount2msat(m.total_msat),  # PrimitiveField in generate_composite
+        "fee_base_msat": amount2msat(m.fee_base_msat),  # PrimitiveField in generate_composite
+        "fee_proportional_millionths": m.fee_proportional_millionths,  # PrimitiveField in generate_composite
+        "dust_limit_msat": amount2msat(m.dust_limit_msat),  # PrimitiveField in generate_composite
+        "max_total_htlc_in_msat": amount2msat(m.max_total_htlc_in_msat),  # PrimitiveField in generate_composite
+        "their_reserve_msat": amount2msat(m.their_reserve_msat),  # PrimitiveField in generate_composite
+        "our_reserve_msat": amount2msat(m.our_reserve_msat),  # PrimitiveField in generate_composite
+        "spendable_msat": amount2msat(m.spendable_msat),  # PrimitiveField in generate_composite
+        "receivable_msat": amount2msat(m.receivable_msat),  # PrimitiveField in generate_composite
+        "minimum_htlc_in_msat": amount2msat(m.minimum_htlc_in_msat),  # PrimitiveField in generate_composite
+        "minimum_htlc_out_msat": amount2msat(m.minimum_htlc_out_msat),  # PrimitiveField in generate_composite
+        "maximum_htlc_out_msat": amount2msat(m.maximum_htlc_out_msat),  # PrimitiveField in generate_composite
+        "their_to_self_delay": m.their_to_self_delay,  # PrimitiveField in generate_composite
+        "our_to_self_delay": m.our_to_self_delay,  # PrimitiveField in generate_composite
+        "max_accepted_htlcs": m.max_accepted_htlcs,  # PrimitiveField in generate_composite
+        "state_changes": [listpeerchannels_channels_state_changes2py(i) for i in m.state_changes],  # ArrayField[composite] in generate_composite
+        "status": [m.status for i in m.status], # ArrayField[primitive] in generate_composite
+        "in_payments_offered": m.in_payments_offered,  # PrimitiveField in generate_composite
+        "in_offered_msat": amount2msat(m.in_offered_msat),  # PrimitiveField in generate_composite
+        "in_payments_fulfilled": m.in_payments_fulfilled,  # PrimitiveField in generate_composite
+        "in_fulfilled_msat": amount2msat(m.in_fulfilled_msat),  # PrimitiveField in generate_composite
+        "out_payments_offered": m.out_payments_offered,  # PrimitiveField in generate_composite
+        "out_offered_msat": amount2msat(m.out_offered_msat),  # PrimitiveField in generate_composite
+        "out_payments_fulfilled": m.out_payments_fulfilled,  # PrimitiveField in generate_composite
+        "out_fulfilled_msat": amount2msat(m.out_fulfilled_msat),  # PrimitiveField in generate_composite
+        "htlcs": [listpeerchannels_channels_htlcs2py(i) for i in m.htlcs],  # ArrayField[composite] in generate_composite
+        "close_to_addr": m.close_to_addr,  # PrimitiveField in generate_composite
+    })
+
+
+def listpeerchannels2py(m):
+    return remove_default({
+        "channels": [listpeerchannels_channels2py(i) for i in m.channels],  # ArrayField[composite] in generate_composite
+    })
+
+
+def listclosedchannels_closedchannels_alias2py(m):
+    return remove_default({
+        "local": m.local,  # PrimitiveField in generate_composite
+        "remote": m.remote,  # PrimitiveField in generate_composite
+    })
+
+
+def listclosedchannels_closedchannels_channel_type2py(m):
+    return remove_default({
+        "bits": [m.bits for i in m.bits], # ArrayField[primitive] in generate_composite
+        "names": [str(i) for i in m.names],  # ArrayField[composite] in generate_composite
+    })
+
+
+def listclosedchannels_closedchannels2py(m):
+    return remove_default({
+        "peer_id": hexlify(m.peer_id),  # PrimitiveField in generate_composite
+        "channel_id": hexlify(m.channel_id),  # PrimitiveField in generate_composite
+        "short_channel_id": m.short_channel_id,  # PrimitiveField in generate_composite
+        "opener": str(m.opener),  # EnumField in generate_composite
+        "closer": str(m.closer),  # EnumField in generate_composite
+        "private": m.private,  # PrimitiveField in generate_composite
+        "total_local_commitments": m.total_local_commitments,  # PrimitiveField in generate_composite
+        "total_remote_commitments": m.total_remote_commitments,  # PrimitiveField in generate_composite
+        "total_htlcs_sent": m.total_htlcs_sent,  # PrimitiveField in generate_composite
+        "funding_txid": hexlify(m.funding_txid),  # PrimitiveField in generate_composite
+        "funding_outnum": m.funding_outnum,  # PrimitiveField in generate_composite
+        "leased": m.leased,  # PrimitiveField in generate_composite
+        "funding_fee_paid_msat": amount2msat(m.funding_fee_paid_msat),  # PrimitiveField in generate_composite
+        "funding_fee_rcvd_msat": amount2msat(m.funding_fee_rcvd_msat),  # PrimitiveField in generate_composite
+        "funding_pushed_msat": amount2msat(m.funding_pushed_msat),  # PrimitiveField in generate_composite
+        "total_msat": amount2msat(m.total_msat),  # PrimitiveField in generate_composite
+        "final_to_us_msat": amount2msat(m.final_to_us_msat),  # PrimitiveField in generate_composite
+        "min_to_us_msat": amount2msat(m.min_to_us_msat),  # PrimitiveField in generate_composite
+        "max_to_us_msat": amount2msat(m.max_to_us_msat),  # PrimitiveField in generate_composite
+        "last_commitment_txid": hexlify(m.last_commitment_txid),  # PrimitiveField in generate_composite
+        "last_commitment_fee_msat": amount2msat(m.last_commitment_fee_msat),  # PrimitiveField in generate_composite
+        "close_cause": str(m.close_cause),  # EnumField in generate_composite
+    })
+
+
+def listclosedchannels2py(m):
+    return remove_default({
+        "closedchannels": [listclosedchannels_closedchannels2py(i) for i in m.closedchannels],  # ArrayField[composite] in generate_composite
+    })
+
+
+def decodepay_fallbacks2py(m):
+    return remove_default({
+        "type": str(m.item_type),  # EnumField in generate_composite
+        "addr": m.addr,  # PrimitiveField in generate_composite
+        "hex": hexlify(m.hex),  # PrimitiveField in generate_composite
+    })
+
+
+def decodepay_routes2py(m):
+    return remove_default({
+        "pubkey": hexlify(m.pubkey),  # PrimitiveField in generate_composite
+        "short_channel_id": m.short_channel_id,  # PrimitiveField in generate_composite
+        "fee_base_msat": amount2msat(m.fee_base_msat),  # PrimitiveField in generate_composite
+        "fee_proportional_millionths": m.fee_proportional_millionths,  # PrimitiveField in generate_composite
+        "cltv_expiry_delta": m.cltv_expiry_delta,  # PrimitiveField in generate_composite
+    })
+
+
+def decodepay_extra2py(m):
+    return remove_default({
+        "tag": m.tag,  # PrimitiveField in generate_composite
+        "data": m.data,  # PrimitiveField in generate_composite
+    })
+
+
+def decodepay2py(m):
+    return remove_default({
+        "currency": m.currency,  # PrimitiveField in generate_composite
+        "created_at": m.created_at,  # PrimitiveField in generate_composite
+        "expiry": m.expiry,  # PrimitiveField in generate_composite
+        "payee": hexlify(m.payee),  # PrimitiveField in generate_composite
+        "amount_msat": amount2msat(m.amount_msat),  # PrimitiveField in generate_composite
+        "payment_hash": hexlify(m.payment_hash),  # PrimitiveField in generate_composite
+        "signature": hexlify(m.signature),  # PrimitiveField in generate_composite
+        "description": m.description,  # PrimitiveField in generate_composite
+        "description_hash": hexlify(m.description_hash),  # PrimitiveField in generate_composite
+        "min_final_cltv_expiry": m.min_final_cltv_expiry,  # PrimitiveField in generate_composite
+        "payment_secret": hexlify(m.payment_secret),  # PrimitiveField in generate_composite
+        "features": hexlify(m.features),  # PrimitiveField in generate_composite
+        "payment_metadata": hexlify(m.payment_metadata),  # PrimitiveField in generate_composite
+        "fallbacks": [decodepay_fallbacks2py(i) for i in m.fallbacks],  # ArrayField[composite] in generate_composite
+        "routes": [decodepay_routes2py(i) for i in m.routes],  # ArrayField[composite] in generate_composite
+        "extra": [decodepay_extra2py(i) for i in m.extra],  # ArrayField[composite] in generate_composite
+    })
+
+
+def decode_offer_paths_path2py(m):
+    return remove_default({
+        "blinded_node_id": hexlify(m.blinded_node_id),  # PrimitiveField in generate_composite
+        "encrypted_recipient_data": hexlify(m.encrypted_recipient_data),  # PrimitiveField in generate_composite
+    })
+
+
+def decode_offer_paths2py(m):
+    return remove_default({
+        "first_node_id": hexlify(m.first_node_id),  # PrimitiveField in generate_composite
+        "blinding": hexlify(m.blinding),  # PrimitiveField in generate_composite
+        "path": [decode_offer_paths_path2py(i) for i in m.path],  # ArrayField[composite] in generate_composite
+    })
+
+
+def decode_offer_recurrence_paywindow2py(m):
+    return remove_default({
+        "seconds_before": m.seconds_before,  # PrimitiveField in generate_composite
+        "seconds_after": m.seconds_after,  # PrimitiveField in generate_composite
+        "proportional_amount": m.proportional_amount,  # PrimitiveField in generate_composite
+    })
+
+
+def decode_offer_recurrence2py(m):
+    return remove_default({
+        "time_unit": m.time_unit,  # PrimitiveField in generate_composite
+        "time_unit_name": m.time_unit_name,  # PrimitiveField in generate_composite
+        "period": m.period,  # PrimitiveField in generate_composite
+        "basetime": m.basetime,  # PrimitiveField in generate_composite
+        "start_any_period": m.start_any_period,  # PrimitiveField in generate_composite
+        "limit": m.limit,  # PrimitiveField in generate_composite
+    })
+
+
+def decode_unknown_offer_tlvs2py(m):
+    return remove_default({
+        "item_type": m.type,  # PrimitiveField in generate_composite
+        "length": m.length,  # PrimitiveField in generate_composite
+        "value": hexlify(m.value),  # PrimitiveField in generate_composite
+    })
+
+
+def decode_unknown_invoice_request_tlvs2py(m):
+    return remove_default({
+        "item_type": m.type,  # PrimitiveField in generate_composite
+        "length": m.length,  # PrimitiveField in generate_composite
+        "value": hexlify(m.value),  # PrimitiveField in generate_composite
+    })
+
+
+def decode_invoice_paths_payinfo2py(m):
+    return remove_default({
+        "fee_base_msat": amount2msat(m.fee_base_msat),  # PrimitiveField in generate_composite
+        "fee_proportional_millionths": m.fee_proportional_millionths,  # PrimitiveField in generate_composite
+        "cltv_expiry_delta": m.cltv_expiry_delta,  # PrimitiveField in generate_composite
+        "features": hexlify(m.features),  # PrimitiveField in generate_composite
+    })
+
+
+def decode_invoice_paths_path2py(m):
+    return remove_default({
+        "blinded_node_id": hexlify(m.blinded_node_id),  # PrimitiveField in generate_composite
+        "encrypted_recipient_data": hexlify(m.encrypted_recipient_data),  # PrimitiveField in generate_composite
+    })
+
+
+def decode_invoice_paths2py(m):
+    return remove_default({
+        "first_node_id": hexlify(m.first_node_id),  # PrimitiveField in generate_composite
+        "blinding": hexlify(m.blinding),  # PrimitiveField in generate_composite
+        "path": [decode_invoice_paths_path2py(i) for i in m.path],  # ArrayField[composite] in generate_composite
+    })
+
+
+def decode_invoice_fallbacks2py(m):
+    return remove_default({
+        "version": m.version,  # PrimitiveField in generate_composite
+        "hex": hexlify(m.hex),  # PrimitiveField in generate_composite
+        "address": m.address,  # PrimitiveField in generate_composite
+    })
+
+
+def decode_unknown_invoice_tlvs2py(m):
+    return remove_default({
+        "item_type": m.type,  # PrimitiveField in generate_composite
+        "length": m.length,  # PrimitiveField in generate_composite
+        "value": hexlify(m.value),  # PrimitiveField in generate_composite
+    })
+
+
+def decode_fallbacks2py(m):
+    return remove_default({
+        "warning_invoice_fallbacks_version_invalid": m.warning_invoice_fallbacks_version_invalid,  # PrimitiveField in generate_composite
+    })
+
+
+def decode_routes2py(m):
+    return remove_default({
+        "pubkey": hexlify(m.pubkey),  # PrimitiveField in generate_composite
+        "short_channel_id": m.short_channel_id,  # PrimitiveField in generate_composite
+        "fee_base_msat": amount2msat(m.fee_base_msat),  # PrimitiveField in generate_composite
+        "fee_proportional_millionths": m.fee_proportional_millionths,  # PrimitiveField in generate_composite
+        "cltv_expiry_delta": m.cltv_expiry_delta,  # PrimitiveField in generate_composite
+    })
+
+
+def decode_extra2py(m):
+    return remove_default({
+        "tag": m.tag,  # PrimitiveField in generate_composite
+        "data": m.data,  # PrimitiveField in generate_composite
+    })
+
+
+def decode_restrictions2py(m):
+    return remove_default({
+        "alternatives": [m.alternatives for i in m.alternatives], # ArrayField[primitive] in generate_composite
+        "summary": m.summary,  # PrimitiveField in generate_composite
+    })
+
+
+def decode2py(m):
+    return remove_default({
+        "type": str(m.item_type),  # EnumField in generate_composite
+        "valid": m.valid,  # PrimitiveField in generate_composite
+        "offer_id": hexlify(m.offer_id),  # PrimitiveField in generate_composite
+        "offer_chains": [hexlify(m.offer_chains) for i in hexlify(m.offer_chains)], # ArrayField[primitive] in generate_composite
+        "offer_metadata": hexlify(m.offer_metadata),  # PrimitiveField in generate_composite
+        "offer_currency": m.offer_currency,  # PrimitiveField in generate_composite
+        "warning_unknown_offer_currency": m.warning_unknown_offer_currency,  # PrimitiveField in generate_composite
+        "currency_minor_unit": m.currency_minor_unit,  # PrimitiveField in generate_composite
+        "offer_amount": m.offer_amount,  # PrimitiveField in generate_composite
+        "offer_amount_msat": amount2msat(m.offer_amount_msat),  # PrimitiveField in generate_composite
+        "offer_description": m.offer_description,  # PrimitiveField in generate_composite
+        "offer_issuer": m.offer_issuer,  # PrimitiveField in generate_composite
+        "offer_features": hexlify(m.offer_features),  # PrimitiveField in generate_composite
+        "offer_absolute_expiry": m.offer_absolute_expiry,  # PrimitiveField in generate_composite
+        "offer_quantity_max": m.offer_quantity_max,  # PrimitiveField in generate_composite
+        "offer_paths": [decode_offer_paths2py(i) for i in m.offer_paths],  # ArrayField[composite] in generate_composite
+        "offer_node_id": hexlify(m.offer_node_id),  # PrimitiveField in generate_composite
+        "unknown_offer_tlvs": [decode_unknown_offer_tlvs2py(i) for i in m.unknown_offer_tlvs],  # ArrayField[composite] in generate_composite
+        "warning_missing_offer_node_id": m.warning_missing_offer_node_id,  # PrimitiveField in generate_composite
+        "warning_invalid_offer_description": m.warning_invalid_offer_description,  # PrimitiveField in generate_composite
+        "warning_missing_offer_description": m.warning_missing_offer_description,  # PrimitiveField in generate_composite
+        "warning_invalid_offer_currency": m.warning_invalid_offer_currency,  # PrimitiveField in generate_composite
+        "warning_invalid_offer_issuer": m.warning_invalid_offer_issuer,  # PrimitiveField in generate_composite
+        "invreq_metadata": hexlify(m.invreq_metadata),  # PrimitiveField in generate_composite
+        "invreq_payer_id": hexlify(m.invreq_payer_id),  # PrimitiveField in generate_composite
+        "invreq_chain": hexlify(m.invreq_chain),  # PrimitiveField in generate_composite
+        "invreq_amount_msat": amount2msat(m.invreq_amount_msat),  # PrimitiveField in generate_composite
+        "invreq_features": hexlify(m.invreq_features),  # PrimitiveField in generate_composite
+        "invreq_quantity": m.invreq_quantity,  # PrimitiveField in generate_composite
+        "invreq_payer_note": m.invreq_payer_note,  # PrimitiveField in generate_composite
+        "invreq_recurrence_counter": m.invreq_recurrence_counter,  # PrimitiveField in generate_composite
+        "invreq_recurrence_start": m.invreq_recurrence_start,  # PrimitiveField in generate_composite
+        "unknown_invoice_request_tlvs": [decode_unknown_invoice_request_tlvs2py(i) for i in m.unknown_invoice_request_tlvs],  # ArrayField[composite] in generate_composite
+        "warning_missing_invreq_metadata": m.warning_missing_invreq_metadata,  # PrimitiveField in generate_composite
+        "warning_missing_invreq_payer_id": m.warning_missing_invreq_payer_id,  # PrimitiveField in generate_composite
+        "warning_invalid_invreq_payer_note": m.warning_invalid_invreq_payer_note,  # PrimitiveField in generate_composite
+        "warning_missing_invoice_request_signature": m.warning_missing_invoice_request_signature,  # PrimitiveField in generate_composite
+        "warning_invalid_invoice_request_signature": m.warning_invalid_invoice_request_signature,  # PrimitiveField in generate_composite
+        "invoice_paths": [decode_invoice_paths2py(i) for i in m.invoice_paths],  # ArrayField[composite] in generate_composite
+        "invoice_created_at": m.invoice_created_at,  # PrimitiveField in generate_composite
+        "invoice_relative_expiry": m.invoice_relative_expiry,  # PrimitiveField in generate_composite
+        "invoice_payment_hash": hexlify(m.invoice_payment_hash),  # PrimitiveField in generate_composite
+        "invoice_amount_msat": amount2msat(m.invoice_amount_msat),  # PrimitiveField in generate_composite
+        "invoice_fallbacks": [decode_invoice_fallbacks2py(i) for i in m.invoice_fallbacks],  # ArrayField[composite] in generate_composite
+        "invoice_features": hexlify(m.invoice_features),  # PrimitiveField in generate_composite
+        "invoice_node_id": hexlify(m.invoice_node_id),  # PrimitiveField in generate_composite
+        "invoice_recurrence_basetime": m.invoice_recurrence_basetime,  # PrimitiveField in generate_composite
+        "unknown_invoice_tlvs": [decode_unknown_invoice_tlvs2py(i) for i in m.unknown_invoice_tlvs],  # ArrayField[composite] in generate_composite
+        "warning_missing_invoice_paths": m.warning_missing_invoice_paths,  # PrimitiveField in generate_composite
+        "warning_missing_invoice_blindedpay": m.warning_missing_invoice_blindedpay,  # PrimitiveField in generate_composite
+        "warning_missing_invoice_created_at": m.warning_missing_invoice_created_at,  # PrimitiveField in generate_composite
+        "warning_missing_invoice_payment_hash": m.warning_missing_invoice_payment_hash,  # PrimitiveField in generate_composite
+        "warning_missing_invoice_amount": m.warning_missing_invoice_amount,  # PrimitiveField in generate_composite
+        "warning_missing_invoice_recurrence_basetime": m.warning_missing_invoice_recurrence_basetime,  # PrimitiveField in generate_composite
+        "warning_missing_invoice_node_id": m.warning_missing_invoice_node_id,  # PrimitiveField in generate_composite
+        "warning_missing_invoice_signature": m.warning_missing_invoice_signature,  # PrimitiveField in generate_composite
+        "warning_invalid_invoice_signature": m.warning_invalid_invoice_signature,  # PrimitiveField in generate_composite
+        "fallbacks": [decode_fallbacks2py(i) for i in m.fallbacks],  # ArrayField[composite] in generate_composite
+        "created_at": m.created_at,  # PrimitiveField in generate_composite
+        "expiry": m.expiry,  # PrimitiveField in generate_composite
+        "payee": hexlify(m.payee),  # PrimitiveField in generate_composite
+        "payment_hash": hexlify(m.payment_hash),  # PrimitiveField in generate_composite
+        "description_hash": hexlify(m.description_hash),  # PrimitiveField in generate_composite
+        "min_final_cltv_expiry": m.min_final_cltv_expiry,  # PrimitiveField in generate_composite
+        "payment_secret": hexlify(m.payment_secret),  # PrimitiveField in generate_composite
+        "payment_metadata": hexlify(m.payment_metadata),  # PrimitiveField in generate_composite
+        "routes": [decode_routes2py(i) for i in m.routes],  # ArrayField[composite] in generate_composite
+        "extra": [decode_extra2py(i) for i in m.extra],  # ArrayField[composite] in generate_composite
+        "unique_id": m.unique_id,  # PrimitiveField in generate_composite
+        "version": m.version,  # PrimitiveField in generate_composite
+        "string": m.string,  # PrimitiveField in generate_composite
+        "restrictions": [decode_restrictions2py(i) for i in m.restrictions],  # ArrayField[composite] in generate_composite
+        "warning_rune_invalid_utf8": m.warning_rune_invalid_utf8,  # PrimitiveField in generate_composite
+        "hex": hexlify(m.hex),  # PrimitiveField in generate_composite
+    })
+
+
 def disconnect2py(m):
     return remove_default({
     })
 
 
+def feerates_perkb_estimates2py(m):
+    return remove_default({
+        "blockcount": m.blockcount,  # PrimitiveField in generate_composite
+        "feerate": m.feerate,  # PrimitiveField in generate_composite
+        "smoothed_feerate": m.smoothed_feerate,  # PrimitiveField in generate_composite
+    })
+
+
 def feerates_perkb2py(m):
     return remove_default({
         "min_acceptable": m.min_acceptable,  # PrimitiveField in generate_composite
         "max_acceptable": m.max_acceptable,  # PrimitiveField in generate_composite
+        "floor": m.floor,  # PrimitiveField in generate_composite
+        "estimates": [feerates_perkb_estimates2py(i) for i in m.estimates],  # ArrayField[composite] in generate_composite
         "opening": m.opening,  # PrimitiveField in generate_composite
         "mutual_close": m.mutual_close,  # PrimitiveField in generate_composite
         "unilateral_close": m.unilateral_close,  # PrimitiveField in generate_composite
         "delayed_to_us": m.delayed_to_us,  # PrimitiveField in generate_composite
         "htlc_resolution": m.htlc_resolution,  # PrimitiveField in generate_composite
         "penalty": m.penalty,  # PrimitiveField in generate_composite
     })
 
 
+def feerates_perkw_estimates2py(m):
+    return remove_default({
+        "blockcount": m.blockcount,  # PrimitiveField in generate_composite
+        "feerate": m.feerate,  # PrimitiveField in generate_composite
+        "smoothed_feerate": m.smoothed_feerate,  # PrimitiveField in generate_composite
+    })
+
+
 def feerates_perkw2py(m):
     return remove_default({
         "min_acceptable": m.min_acceptable,  # PrimitiveField in generate_composite
         "max_acceptable": m.max_acceptable,  # PrimitiveField in generate_composite
+        "floor": m.floor,  # PrimitiveField in generate_composite
+        "estimates": [feerates_perkw_estimates2py(i) for i in m.estimates],  # ArrayField[composite] in generate_composite
         "opening": m.opening,  # PrimitiveField in generate_composite
         "mutual_close": m.mutual_close,  # PrimitiveField in generate_composite
         "unilateral_close": m.unilateral_close,  # PrimitiveField in generate_composite
         "delayed_to_us": m.delayed_to_us,  # PrimitiveField in generate_composite
         "htlc_resolution": m.htlc_resolution,  # PrimitiveField in generate_composite
         "penalty": m.penalty,  # PrimitiveField in generate_composite
     })
@@ -785,15 +1218,14 @@
 
 
 def getroute_route2py(m):
     return remove_default({
         "id": hexlify(m.id),  # PrimitiveField in generate_composite
         "channel": m.channel,  # PrimitiveField in generate_composite
         "direction": m.direction,  # PrimitiveField in generate_composite
-        "msatoshi": m.msatoshi,  # PrimitiveField in generate_composite
         "amount_msat": amount2msat(m.amount_msat),  # PrimitiveField in generate_composite
         "delay": m.delay,  # PrimitiveField in generate_composite
         "style": str(m.style),  # EnumField in generate_composite
     })
 
 
 def getroute2py(m):
```

### Comparing `pyln_testing-23.2/pyln/testing/node_pb2.py` & `pyln-testing-23.5/pyln/testing/node_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import primitives_pb2 as primitives__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nnode.proto\x12\x03\x63ln\x1a\x10primitives.proto\"\x10\n\x0eGetinfoRequest\"\xf4\x04\n\x0fGetinfoResponse\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\x0c\x12\x11\n\tnum_peers\x18\x04 \x01(\r\x12\x1c\n\x14num_pending_channels\x18\x05 \x01(\r\x12\x1b\n\x13num_active_channels\x18\x06 \x01(\r\x12\x1d\n\x15num_inactive_channels\x18\x07 \x01(\r\x12\x0f\n\x07version\x18\x08 \x01(\t\x12\x15\n\rlightning_dir\x18\t \x01(\t\x12\x33\n\x0cour_features\x18\n \x01(\x0b\x32\x18.cln.GetinfoOur_featuresH\x00\x88\x01\x01\x12\x13\n\x0b\x62lockheight\x18\x0b \x01(\r\x12\x0f\n\x07network\x18\x0c \x01(\t\x12$\n\x17msatoshi_fees_collected\x18\x12 \x01(\x04H\x01\x88\x01\x01\x12(\n\x13\x66\x65\x65s_collected_msat\x18\r \x01(\x0b\x32\x0b.cln.Amount\x12$\n\x07\x61\x64\x64ress\x18\x0e \x03(\x0b\x32\x13.cln.GetinfoAddress\x12$\n\x07\x62inding\x18\x0f \x03(\x0b\x32\x13.cln.GetinfoBinding\x12\"\n\x15warning_bitcoind_sync\x18\x10 \x01(\tH\x02\x88\x01\x01\x12$\n\x17warning_lightningd_sync\x18\x11 \x01(\tH\x03\x88\x01\x01\x42\x0f\n\r_our_featuresB\x1a\n\x18_msatoshi_fees_collectedB\x18\n\x16_warning_bitcoind_syncB\x1a\n\x18_warning_lightningd_sync\"S\n\x13GetinfoOur_features\x12\x0c\n\x04init\x18\x01 \x01(\x0c\x12\x0c\n\x04node\x18\x02 \x01(\x0c\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\x0c\x12\x0f\n\x07invoice\x18\x04 \x01(\x0c\"\xd3\x01\n\x0eGetinfoAddress\x12\x39\n\titem_type\x18\x01 \x01(\x0e\x32&.cln.GetinfoAddress.GetinfoAddressType\x12\x0c\n\x04port\x18\x02 \x01(\r\x12\x14\n\x07\x61\x64\x64ress\x18\x03 \x01(\tH\x00\x88\x01\x01\"V\n\x12GetinfoAddressType\x12\x07\n\x03\x44NS\x10\x00\x12\x08\n\x04IPV4\x10\x01\x12\x08\n\x04IPV6\x10\x02\x12\t\n\x05TORV2\x10\x03\x12\t\n\x05TORV3\x10\x04\x12\r\n\tWEBSOCKET\x10\x05\x42\n\n\x08_address\"\xfb\x01\n\x0eGetinfoBinding\x12\x39\n\titem_type\x18\x01 \x01(\x0e\x32&.cln.GetinfoBinding.GetinfoBindingType\x12\x14\n\x07\x61\x64\x64ress\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\x04port\x18\x03 \x01(\rH\x01\x88\x01\x01\x12\x13\n\x06socket\x18\x04 \x01(\tH\x02\x88\x01\x01\"P\n\x12GetinfoBindingType\x12\x10\n\x0cLOCAL_SOCKET\x10\x00\x12\x08\n\x04IPV4\x10\x01\x12\x08\n\x04IPV6\x10\x02\x12\t\n\x05TORV2\x10\x03\x12\t\n\x05TORV3\x10\x04\x42\n\n\x08_addressB\x07\n\x05_portB\t\n\x07_socket\"H\n\x10ListpeersRequest\x12\x0f\n\x02id\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05level\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x05\n\x03_idB\x08\n\x06_level\"7\n\x11ListpeersResponse\x12\"\n\x05peers\x18\x01 \x03(\x0b\x32\x13.cln.ListpeersPeers\"\xf8\x01\n\x0eListpeersPeers\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x11\n\tconnected\x18\x02 \x01(\x08\x12\x14\n\x0cnum_channels\x18\x08 \x01(\r\x12#\n\x03log\x18\x03 \x03(\x0b\x32\x16.cln.ListpeersPeersLog\x12-\n\x08\x63hannels\x18\x04 \x03(\x0b\x32\x1b.cln.ListpeersPeersChannels\x12\x0f\n\x07netaddr\x18\x05 \x03(\t\x12\x18\n\x0bremote_addr\x18\x07 \x01(\tH\x00\x88\x01\x01\x12\x15\n\x08\x66\x65\x61tures\x18\x06 \x01(\x0cH\x01\x88\x01\x01\x42\x0e\n\x0c_remote_addrB\x0b\n\t_features\"\xfd\x02\n\x11ListpeersPeersLog\x12?\n\titem_type\x18\x01 \x01(\x0e\x32,.cln.ListpeersPeersLog.ListpeersPeersLogType\x12\x18\n\x0bnum_skipped\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x11\n\x04time\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x06source\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x10\n\x03log\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x14\n\x07node_id\x18\x06 \x01(\x0cH\x04\x88\x01\x01\x12\x11\n\x04\x64\x61ta\x18\x07 \x01(\x0cH\x05\x88\x01\x01\"i\n\x15ListpeersPeersLogType\x12\x0b\n\x07SKIPPED\x10\x00\x12\n\n\x06\x42ROKEN\x10\x01\x12\x0b\n\x07UNUSUAL\x10\x02\x12\x08\n\x04INFO\x10\x03\x12\t\n\x05\x44\x45\x42UG\x10\x04\x12\t\n\x05IO_IN\x10\x05\x12\n\n\x06IO_OUT\x10\x06\x42\x0e\n\x0c_num_skippedB\x07\n\x05_timeB\t\n\x07_sourceB\x06\n\x04_logB\n\n\x08_node_idB\x07\n\x05_data\"\xd6\x17\n\x16ListpeersPeersChannels\x12\x46\n\x05state\x18\x01 \x01(\x0e\x32\x37.cln.ListpeersPeersChannels.ListpeersPeersChannelsState\x12\x19\n\x0cscratch_txid\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x12\x38\n\x07\x66\x65\x65rate\x18\x03 \x01(\x0b\x32\".cln.ListpeersPeersChannelsFeerateH\x01\x88\x01\x01\x12\x12\n\x05owner\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x1d\n\x10short_channel_id\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x17\n\nchannel_id\x18\x06 \x01(\x0cH\x04\x88\x01\x01\x12\x19\n\x0c\x66unding_txid\x18\x07 \x01(\x0cH\x05\x88\x01\x01\x12\x1b\n\x0e\x66unding_outnum\x18\x08 \x01(\rH\x06\x88\x01\x01\x12\x1c\n\x0finitial_feerate\x18\t \x01(\tH\x07\x88\x01\x01\x12\x19\n\x0clast_feerate\x18\n \x01(\tH\x08\x88\x01\x01\x12\x19\n\x0cnext_feerate\x18\x0b \x01(\tH\t\x88\x01\x01\x12\x1a\n\rnext_fee_step\x18\x0c \x01(\rH\n\x88\x01\x01\x12\x35\n\x08inflight\x18\r \x03(\x0b\x32#.cln.ListpeersPeersChannelsInflight\x12\x15\n\x08\x63lose_to\x18\x0e \x01(\x0cH\x0b\x88\x01\x01\x12\x14\n\x07private\x18\x0f \x01(\x08H\x0c\x88\x01\x01\x12 \n\x06opener\x18\x10 \x01(\x0e\x32\x10.cln.ChannelSide\x12%\n\x06\x63loser\x18\x11 \x01(\x0e\x32\x10.cln.ChannelSideH\r\x88\x01\x01\x12\x10\n\x08\x66\x65\x61tures\x18\x12 \x03(\t\x12\x38\n\x07\x66unding\x18\x13 \x01(\x0b\x32\".cln.ListpeersPeersChannelsFundingH\x0e\x88\x01\x01\x12$\n\nto_us_msat\x18\x14 \x01(\x0b\x32\x0b.cln.AmountH\x0f\x88\x01\x01\x12(\n\x0emin_to_us_msat\x18\x15 \x01(\x0b\x32\x0b.cln.AmountH\x10\x88\x01\x01\x12(\n\x0emax_to_us_msat\x18\x16 \x01(\x0b\x32\x0b.cln.AmountH\x11\x88\x01\x01\x12$\n\ntotal_msat\x18\x17 \x01(\x0b\x32\x0b.cln.AmountH\x12\x88\x01\x01\x12\'\n\rfee_base_msat\x18\x18 \x01(\x0b\x32\x0b.cln.AmountH\x13\x88\x01\x01\x12(\n\x1b\x66\x65\x65_proportional_millionths\x18\x19 \x01(\rH\x14\x88\x01\x01\x12)\n\x0f\x64ust_limit_msat\x18\x1a \x01(\x0b\x32\x0b.cln.AmountH\x15\x88\x01\x01\x12\x30\n\x16max_total_htlc_in_msat\x18\x1b \x01(\x0b\x32\x0b.cln.AmountH\x16\x88\x01\x01\x12,\n\x12their_reserve_msat\x18\x1c \x01(\x0b\x32\x0b.cln.AmountH\x17\x88\x01\x01\x12*\n\x10our_reserve_msat\x18\x1d \x01(\x0b\x32\x0b.cln.AmountH\x18\x88\x01\x01\x12(\n\x0espendable_msat\x18\x1e \x01(\x0b\x32\x0b.cln.AmountH\x19\x88\x01\x01\x12)\n\x0freceivable_msat\x18\x1f \x01(\x0b\x32\x0b.cln.AmountH\x1a\x88\x01\x01\x12.\n\x14minimum_htlc_in_msat\x18  \x01(\x0b\x32\x0b.cln.AmountH\x1b\x88\x01\x01\x12/\n\x15minimum_htlc_out_msat\x18\x30 \x01(\x0b\x32\x0b.cln.AmountH\x1c\x88\x01\x01\x12/\n\x15maximum_htlc_out_msat\x18\x31 \x01(\x0b\x32\x0b.cln.AmountH\x1d\x88\x01\x01\x12 \n\x13their_to_self_delay\x18! \x01(\rH\x1e\x88\x01\x01\x12\x1e\n\x11our_to_self_delay\x18\" \x01(\rH\x1f\x88\x01\x01\x12\x1f\n\x12max_accepted_htlcs\x18# \x01(\rH \x88\x01\x01\x12\x34\n\x05\x61lias\x18\x32 \x01(\x0b\x32 .cln.ListpeersPeersChannelsAliasH!\x88\x01\x01\x12\x0e\n\x06status\x18% \x03(\t\x12 \n\x13in_payments_offered\x18& \x01(\x04H\"\x88\x01\x01\x12)\n\x0fin_offered_msat\x18\' \x01(\x0b\x32\x0b.cln.AmountH#\x88\x01\x01\x12\"\n\x15in_payments_fulfilled\x18( \x01(\x04H$\x88\x01\x01\x12+\n\x11in_fulfilled_msat\x18) \x01(\x0b\x32\x0b.cln.AmountH%\x88\x01\x01\x12!\n\x14out_payments_offered\x18* \x01(\x04H&\x88\x01\x01\x12*\n\x10out_offered_msat\x18+ \x01(\x0b\x32\x0b.cln.AmountH\'\x88\x01\x01\x12#\n\x16out_payments_fulfilled\x18, \x01(\x04H(\x88\x01\x01\x12,\n\x12out_fulfilled_msat\x18- \x01(\x0b\x32\x0b.cln.AmountH)\x88\x01\x01\x12/\n\x05htlcs\x18. \x03(\x0b\x32 .cln.ListpeersPeersChannelsHtlcs\x12\x1a\n\rclose_to_addr\x18/ \x01(\tH*\x88\x01\x01\"\xa1\x02\n\x1bListpeersPeersChannelsState\x12\x0c\n\x08OPENINGD\x10\x00\x12\x1c\n\x18\x43HANNELD_AWAITING_LOCKIN\x10\x01\x12\x13\n\x0f\x43HANNELD_NORMAL\x10\x02\x12\x1a\n\x16\x43HANNELD_SHUTTING_DOWN\x10\x03\x12\x18\n\x14\x43LOSINGD_SIGEXCHANGE\x10\x04\x12\x15\n\x11\x43LOSINGD_COMPLETE\x10\x05\x12\x17\n\x13\x41WAITING_UNILATERAL\x10\x06\x12\x16\n\x12\x46UNDING_SPEND_SEEN\x10\x07\x12\x0b\n\x07ONCHAIN\x10\x08\x12\x17\n\x13\x44UALOPEND_OPEN_INIT\x10\t\x12\x1d\n\x19\x44UALOPEND_AWAITING_LOCKIN\x10\nB\x0f\n\r_scratch_txidB\n\n\x08_feerateB\x08\n\x06_ownerB\x13\n\x11_short_channel_idB\r\n\x0b_channel_idB\x0f\n\r_funding_txidB\x11\n\x0f_funding_outnumB\x12\n\x10_initial_feerateB\x0f\n\r_last_feerateB\x0f\n\r_next_feerateB\x10\n\x0e_next_fee_stepB\x0b\n\t_close_toB\n\n\x08_privateB\t\n\x07_closerB\n\n\x08_fundingB\r\n\x0b_to_us_msatB\x11\n\x0f_min_to_us_msatB\x11\n\x0f_max_to_us_msatB\r\n\x0b_total_msatB\x10\n\x0e_fee_base_msatB\x1e\n\x1c_fee_proportional_millionthsB\x12\n\x10_dust_limit_msatB\x19\n\x17_max_total_htlc_in_msatB\x15\n\x13_their_reserve_msatB\x13\n\x11_our_reserve_msatB\x11\n\x0f_spendable_msatB\x12\n\x10_receivable_msatB\x17\n\x15_minimum_htlc_in_msatB\x18\n\x16_minimum_htlc_out_msatB\x18\n\x16_maximum_htlc_out_msatB\x16\n\x14_their_to_self_delayB\x14\n\x12_our_to_self_delayB\x15\n\x13_max_accepted_htlcsB\x08\n\x06_aliasB\x16\n\x14_in_payments_offeredB\x12\n\x10_in_offered_msatB\x18\n\x16_in_payments_fulfilledB\x14\n\x12_in_fulfilled_msatB\x17\n\x15_out_payments_offeredB\x13\n\x11_out_offered_msatB\x19\n\x17_out_payments_fulfilledB\x15\n\x13_out_fulfilled_msatB\x10\n\x0e_close_to_addr\"=\n\x1dListpeersPeersChannelsFeerate\x12\r\n\x05perkw\x18\x01 \x01(\r\x12\r\n\x05perkb\x18\x02 \x01(\r\"\xc5\x01\n\x1eListpeersPeersChannelsInflight\x12\x14\n\x0c\x66unding_txid\x18\x01 \x01(\x0c\x12\x16\n\x0e\x66unding_outnum\x18\x02 \x01(\r\x12\x0f\n\x07\x66\x65\x65rate\x18\x03 \x01(\t\x12\'\n\x12total_funding_msat\x18\x04 \x01(\x0b\x32\x0b.cln.Amount\x12%\n\x10our_funding_msat\x18\x05 \x01(\x0b\x32\x0b.cln.Amount\x12\x14\n\x0cscratch_txid\x18\x06 \x01(\x0c\"\x87\x03\n\x1dListpeersPeersChannelsFunding\x12$\n\nlocal_msat\x18\x01 \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12%\n\x0bremote_msat\x18\x02 \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12%\n\x0bpushed_msat\x18\x03 \x01(\x0b\x32\x0b.cln.AmountH\x02\x88\x01\x01\x12%\n\x10local_funds_msat\x18\x04 \x01(\x0b\x32\x0b.cln.Amount\x12&\n\x11remote_funds_msat\x18\x07 \x01(\x0b\x32\x0b.cln.Amount\x12\'\n\rfee_paid_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x03\x88\x01\x01\x12\'\n\rfee_rcvd_msat\x18\x06 \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x42\r\n\x0b_local_msatB\x0e\n\x0c_remote_msatB\x0e\n\x0c_pushed_msatB\x10\n\x0e_fee_paid_msatB\x10\n\x0e_fee_rcvd_msat\"[\n\x1bListpeersPeersChannelsAlias\x12\x12\n\x05local\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06remote\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x08\n\x06_localB\t\n\x07_remote\"\xd2\x02\n\x1bListpeersPeersChannelsHtlcs\x12X\n\tdirection\x18\x01 \x01(\x0e\x32\x45.cln.ListpeersPeersChannelsHtlcs.ListpeersPeersChannelsHtlcsDirection\x12\n\n\x02id\x18\x02 \x01(\x04\x12 \n\x0b\x61mount_msat\x18\x03 \x01(\x0b\x32\x0b.cln.Amount\x12\x0e\n\x06\x65xpiry\x18\x04 \x01(\r\x12\x14\n\x0cpayment_hash\x18\x05 \x01(\x0c\x12\x1a\n\rlocal_trimmed\x18\x06 \x01(\x08H\x00\x88\x01\x01\x12\x13\n\x06status\x18\x07 \x01(\tH\x01\x88\x01\x01\"7\n$ListpeersPeersChannelsHtlcsDirection\x12\x06\n\x02IN\x10\x00\x12\x07\n\x03OUT\x10\x01\x42\x10\n\x0e_local_trimmedB\t\n\x07_status\"0\n\x10ListfundsRequest\x12\x12\n\x05spent\x18\x01 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_spent\"e\n\x11ListfundsResponse\x12&\n\x07outputs\x18\x01 \x03(\x0b\x32\x15.cln.ListfundsOutputs\x12(\n\x08\x63hannels\x18\x02 \x03(\x0b\x32\x16.cln.ListfundsChannels\"\x83\x03\n\x10ListfundsOutputs\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\x12\x0e\n\x06output\x18\x02 \x01(\r\x12 \n\x0b\x61mount_msat\x18\x03 \x01(\x0b\x32\x0b.cln.Amount\x12\x14\n\x0cscriptpubkey\x18\x04 \x01(\x0c\x12\x14\n\x07\x61\x64\x64ress\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x19\n\x0credeemscript\x18\x06 \x01(\x0cH\x01\x88\x01\x01\x12<\n\x06status\x18\x07 \x01(\x0e\x32,.cln.ListfundsOutputs.ListfundsOutputsStatus\x12\x10\n\x08reserved\x18\t \x01(\x08\x12\x18\n\x0b\x62lockheight\x18\x08 \x01(\rH\x02\x88\x01\x01\"Q\n\x16ListfundsOutputsStatus\x12\x0f\n\x0bUNCONFIRMED\x10\x00\x12\r\n\tCONFIRMED\x10\x01\x12\t\n\x05SPENT\x10\x02\x12\x0c\n\x08IMMATURE\x10\x03\x42\n\n\x08_addressB\x0f\n\r_redeemscriptB\x0e\n\x0c_blockheight\"\x83\x02\n\x11ListfundsChannels\x12\x0f\n\x07peer_id\x18\x01 \x01(\x0c\x12$\n\x0four_amount_msat\x18\x02 \x01(\x0b\x32\x0b.cln.Amount\x12 \n\x0b\x61mount_msat\x18\x03 \x01(\x0b\x32\x0b.cln.Amount\x12\x14\n\x0c\x66unding_txid\x18\x04 \x01(\x0c\x12\x16\n\x0e\x66unding_output\x18\x05 \x01(\r\x12\x11\n\tconnected\x18\x06 \x01(\x08\x12 \n\x05state\x18\x07 \x01(\x0e\x32\x11.cln.ChannelState\x12\x1d\n\x10short_channel_id\x18\x08 \x01(\tH\x00\x88\x01\x01\x42\x13\n\x11_short_channel_id\"\xdd\x02\n\x0eSendpayRequest\x12 \n\x05route\x18\x01 \x03(\x0b\x32\x11.cln.SendpayRoute\x12\x14\n\x0cpayment_hash\x18\x02 \x01(\x0c\x12\x12\n\x05label\x18\x03 \x01(\tH\x00\x88\x01\x01\x12%\n\x0b\x61mount_msat\x18\n \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x05 \x01(\tH\x02\x88\x01\x01\x12\x1b\n\x0epayment_secret\x18\x06 \x01(\x0cH\x03\x88\x01\x01\x12\x13\n\x06partid\x18\x07 \x01(\rH\x04\x88\x01\x01\x12\x1a\n\rlocalinvreqid\x18\x0b \x01(\x0cH\x05\x88\x01\x01\x12\x14\n\x07groupid\x18\t \x01(\x04H\x06\x88\x01\x01\x42\x08\n\x06_labelB\x0e\n\x0c_amount_msatB\t\n\x07_bolt11B\x11\n\x0f_payment_secretB\t\n\x07_partidB\x10\n\x0e_localinvreqidB\n\n\x08_groupid\"\xd1\x04\n\x0fSendpayResponse\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x14\n\x07groupid\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12\x32\n\x06status\x18\x04 \x01(\x0e\x32\".cln.SendpayResponse.SendpayStatus\x12%\n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\x06 \x01(\x0cH\x02\x88\x01\x01\x12\x12\n\ncreated_at\x18\x07 \x01(\x04\x12\x19\n\x0c\x63ompleted_at\x18\x0f \x01(\x04H\x03\x88\x01\x01\x12%\n\x10\x61mount_sent_msat\x18\x08 \x01(\x0b\x32\x0b.cln.Amount\x12\x12\n\x05label\x18\t \x01(\tH\x04\x88\x01\x01\x12\x13\n\x06partid\x18\n \x01(\x04H\x05\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x0b \x01(\tH\x06\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\r \x01(\x0cH\x08\x88\x01\x01\x12\x14\n\x07message\x18\x0e \x01(\tH\t\x88\x01\x01\"*\n\rSendpayStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x43OMPLETE\x10\x01\x42\n\n\x08_groupidB\x0e\n\x0c_amount_msatB\x0e\n\x0c_destinationB\x0f\n\r_completed_atB\x08\n\x06_labelB\t\n\x07_partidB\t\n\x07_bolt11B\t\n\x07_bolt12B\x13\n\x11_payment_preimageB\n\n\x08_message\"\\\n\x0cSendpayRoute\x12 \n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.Amount\x12\n\n\x02id\x18\x02 \x01(\x0c\x12\r\n\x05\x64\x65lay\x18\x03 \x01(\r\x12\x0f\n\x07\x63hannel\x18\x04 \x01(\t\"\x93\x01\n\x13ListchannelsRequest\x12\x1d\n\x10short_channel_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06source\x18\x02 \x01(\x0cH\x01\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\x03 \x01(\x0cH\x02\x88\x01\x01\x42\x13\n\x11_short_channel_idB\t\n\x07_sourceB\x0e\n\x0c_destination\"C\n\x14ListchannelsResponse\x12+\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x19.cln.ListchannelsChannels\"\xb3\x03\n\x14ListchannelsChannels\x12\x0e\n\x06source\x18\x01 \x01(\x0c\x12\x13\n\x0b\x64\x65stination\x18\x02 \x01(\x0c\x12\x18\n\x10short_channel_id\x18\x03 \x01(\t\x12\x11\n\tdirection\x18\x10 \x01(\r\x12\x0e\n\x06public\x18\x04 \x01(\x08\x12 \n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.Amount\x12\x15\n\rmessage_flags\x18\x06 \x01(\r\x12\x15\n\rchannel_flags\x18\x07 \x01(\r\x12\x0e\n\x06\x61\x63tive\x18\x08 \x01(\x08\x12\x13\n\x0blast_update\x18\t \x01(\r\x12\x1d\n\x15\x62\x61se_fee_millisatoshi\x18\n \x01(\r\x12\x19\n\x11\x66\x65\x65_per_millionth\x18\x0b \x01(\r\x12\r\n\x05\x64\x65lay\x18\x0c \x01(\r\x12&\n\x11htlc_minimum_msat\x18\r \x01(\x0b\x32\x0b.cln.Amount\x12+\n\x11htlc_maximum_msat\x18\x0e \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x10\n\x08\x66\x65\x61tures\x18\x0f \x01(\x0c\x42\x14\n\x12_htlc_maximum_msat\"#\n\x10\x41\x64\x64gossipRequest\x12\x0f\n\x07message\x18\x01 \x01(\x0c\"\x13\n\x11\x41\x64\x64gossipResponse\"o\n\x17\x41utocleaninvoiceRequest\x12\x17\n\nexpired_by\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x1a\n\rcycle_seconds\x18\x02 \x01(\x04H\x01\x88\x01\x01\x42\r\n\x0b_expired_byB\x10\n\x0e_cycle_seconds\"\x81\x01\n\x18\x41utocleaninvoiceResponse\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\nexpired_by\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x1a\n\rcycle_seconds\x18\x03 \x01(\x04H\x01\x88\x01\x01\x42\r\n\x0b_expired_byB\x10\n\x0e_cycle_seconds\"U\n\x13\x43heckmessageRequest\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\r\n\x05zbase\x18\x02 \x01(\t\x12\x13\n\x06pubkey\x18\x03 \x01(\x0cH\x00\x88\x01\x01\x42\t\n\x07_pubkey\"8\n\x14\x43heckmessageResponse\x12\x10\n\x08verified\x18\x01 \x01(\x08\x12\x0e\n\x06pubkey\x18\x02 \x01(\x0c\"\xcb\x02\n\x0c\x43loseRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1e\n\x11unilateraltimeout\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\x03 \x01(\tH\x01\x88\x01\x01\x12!\n\x14\x66\x65\x65_negotiation_step\x18\x04 \x01(\tH\x02\x88\x01\x01\x12)\n\rwrong_funding\x18\x05 \x01(\x0b\x32\r.cln.OutpointH\x03\x88\x01\x01\x12\x1f\n\x12\x66orce_lease_closed\x18\x06 \x01(\x08H\x04\x88\x01\x01\x12\x1e\n\x08\x66\x65\x65range\x18\x07 \x03(\x0b\x32\x0c.cln.FeerateB\x14\n\x12_unilateraltimeoutB\x0e\n\x0c_destinationB\x17\n\x15_fee_negotiation_stepB\x10\n\x0e_wrong_fundingB\x15\n\x13_force_lease_closed\"\xab\x01\n\rCloseResponse\x12/\n\titem_type\x18\x01 \x01(\x0e\x32\x1c.cln.CloseResponse.CloseType\x12\x0f\n\x02tx\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x12\x11\n\x04txid\x18\x03 \x01(\x0cH\x01\x88\x01\x01\"5\n\tCloseType\x12\n\n\x06MUTUAL\x10\x00\x12\x0e\n\nUNILATERAL\x10\x01\x12\x0c\n\x08UNOPENED\x10\x02\x42\x05\n\x03_txB\x07\n\x05_txid\"T\n\x0e\x43onnectRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\x04host\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\x04port\x18\x03 \x01(\rH\x01\x88\x01\x01\x42\x07\n\x05_hostB\x07\n\x05_port\"\xb4\x01\n\x0f\x43onnectResponse\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x10\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0c\x12\x38\n\tdirection\x18\x03 \x01(\x0e\x32%.cln.ConnectResponse.ConnectDirection\x12$\n\x07\x61\x64\x64ress\x18\x04 \x01(\x0b\x32\x13.cln.ConnectAddress\"#\n\x10\x43onnectDirection\x12\x06\n\x02IN\x10\x00\x12\x07\n\x03OUT\x10\x01\"\xfb\x01\n\x0e\x43onnectAddress\x12\x39\n\titem_type\x18\x01 \x01(\x0e\x32&.cln.ConnectAddress.ConnectAddressType\x12\x13\n\x06socket\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x07\x61\x64\x64ress\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04port\x18\x04 \x01(\rH\x02\x88\x01\x01\"P\n\x12\x43onnectAddressType\x12\x10\n\x0cLOCAL_SOCKET\x10\x00\x12\x08\n\x04IPV4\x10\x01\x12\x08\n\x04IPV6\x10\x02\x12\t\n\x05TORV2\x10\x03\x12\t\n\x05TORV3\x10\x04\x42\t\n\x07_socketB\n\n\x08_addressB\x07\n\x05_port\"J\n\x14\x43reateinvoiceRequest\x12\x11\n\tinvstring\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x10\n\x08preimage\x18\x03 \x01(\x0c\"\x81\x05\n\x15\x43reateinvoiceResponse\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x06\x62olt11\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x04 \x01(\x0c\x12%\n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x02\x88\x01\x01\x12>\n\x06status\x18\x06 \x01(\x0e\x32..cln.CreateinvoiceResponse.CreateinvoiceStatus\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x12\n\nexpires_at\x18\x08 \x01(\x04\x12\x16\n\tpay_index\x18\t \x01(\x04H\x03\x88\x01\x01\x12.\n\x14\x61mount_received_msat\x18\n \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x12\x14\n\x07paid_at\x18\x0b \x01(\x04H\x05\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\x0c \x01(\x0cH\x06\x88\x01\x01\x12\x1b\n\x0elocal_offer_id\x18\r \x01(\x0cH\x07\x88\x01\x01\x12\x1e\n\x11invreq_payer_note\x18\x0f \x01(\tH\x08\x88\x01\x01\"8\n\x13\x43reateinvoiceStatus\x12\x08\n\x04PAID\x10\x00\x12\x0b\n\x07\x45XPIRED\x10\x01\x12\n\n\x06UNPAID\x10\x02\x42\t\n\x07_bolt11B\t\n\x07_bolt12B\x0e\n\x0c_amount_msatB\x0c\n\n_pay_indexB\x17\n\x15_amount_received_msatB\n\n\x08_paid_atB\x13\n\x11_payment_preimageB\x11\n\x0f_local_offer_idB\x14\n\x12_invreq_payer_note\"\xb4\x02\n\x10\x44\x61tastoreRequest\x12\x0b\n\x03key\x18\x05 \x03(\t\x12\x13\n\x06string\x18\x06 \x01(\tH\x00\x88\x01\x01\x12\x10\n\x03hex\x18\x02 \x01(\x0cH\x01\x88\x01\x01\x12\x36\n\x04mode\x18\x03 \x01(\x0e\x32#.cln.DatastoreRequest.DatastoreModeH\x02\x88\x01\x01\x12\x17\n\ngeneration\x18\x04 \x01(\x04H\x03\x88\x01\x01\"p\n\rDatastoreMode\x12\x0f\n\x0bMUST_CREATE\x10\x00\x12\x10\n\x0cMUST_REPLACE\x10\x01\x12\x15\n\x11\x43REATE_OR_REPLACE\x10\x02\x12\x0f\n\x0bMUST_APPEND\x10\x03\x12\x14\n\x10\x43REATE_OR_APPEND\x10\x04\x42\t\n\x07_stringB\x06\n\x04_hexB\x07\n\x05_modeB\r\n\x0b_generation\"\x82\x01\n\x11\x44\x61tastoreResponse\x12\x0b\n\x03key\x18\x05 \x03(\t\x12\x17\n\ngeneration\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x10\n\x03hex\x18\x03 \x01(\x0cH\x01\x88\x01\x01\x12\x13\n\x06string\x18\x04 \x01(\tH\x02\x88\x01\x01\x42\r\n\x0b_generationB\x06\n\x04_hexB\t\n\x07_string\"\x9d\x01\n\x12\x43reateonionRequest\x12\"\n\x04hops\x18\x01 \x03(\x0b\x32\x14.cln.CreateonionHops\x12\x11\n\tassocdata\x18\x02 \x01(\x0c\x12\x18\n\x0bsession_key\x18\x03 \x01(\x0cH\x00\x88\x01\x01\x12\x17\n\nonion_size\x18\x04 \x01(\rH\x01\x88\x01\x01\x42\x0e\n\x0c_session_keyB\r\n\x0b_onion_size\"<\n\x13\x43reateonionResponse\x12\r\n\x05onion\x18\x01 \x01(\x0c\x12\x16\n\x0eshared_secrets\x18\x02 \x03(\x0c\"2\n\x0f\x43reateonionHops\x12\x0e\n\x06pubkey\x18\x01 \x01(\x0c\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\"J\n\x13\x44\x65ldatastoreRequest\x12\x0b\n\x03key\x18\x03 \x03(\t\x12\x17\n\ngeneration\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\r\n\x0b_generation\"\x85\x01\n\x14\x44\x65ldatastoreResponse\x12\x0b\n\x03key\x18\x05 \x03(\t\x12\x17\n\ngeneration\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x10\n\x03hex\x18\x03 \x01(\x0cH\x01\x88\x01\x01\x12\x13\n\x06string\x18\x04 \x01(\tH\x02\x88\x01\x01\x42\r\n\x0b_generationB\x06\n\x04_hexB\t\n\x07_string\"H\n\x18\x44\x65lexpiredinvoiceRequest\x12\x1a\n\rmaxexpirytime\x18\x01 \x01(\x04H\x00\x88\x01\x01\x42\x10\n\x0e_maxexpirytime\"\x1b\n\x19\x44\x65lexpiredinvoiceResponse\"\xb6\x01\n\x11\x44\x65linvoiceRequest\x12\r\n\x05label\x18\x01 \x01(\t\x12\x37\n\x06status\x18\x02 \x01(\x0e\x32\'.cln.DelinvoiceRequest.DelinvoiceStatus\x12\x15\n\x08\x64\x65sconly\x18\x03 \x01(\x08H\x00\x88\x01\x01\"5\n\x10\x44\x65linvoiceStatus\x12\x08\n\x04PAID\x10\x00\x12\x0b\n\x07\x45XPIRED\x10\x01\x12\n\n\x06UNPAID\x10\x02\x42\x0b\n\t_desconly\"\xc5\x03\n\x12\x44\x65linvoiceResponse\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x06\x62olt11\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x03 \x01(\tH\x01\x88\x01\x01\x12%\n\x0b\x61mount_msat\x18\x04 \x01(\x0b\x32\x0b.cln.AmountH\x02\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x06 \x01(\x0c\x12\x38\n\x06status\x18\x07 \x01(\x0e\x32(.cln.DelinvoiceResponse.DelinvoiceStatus\x12\x12\n\nexpires_at\x18\x08 \x01(\x04\x12\x1b\n\x0elocal_offer_id\x18\t \x01(\x0cH\x04\x88\x01\x01\x12\x1e\n\x11invreq_payer_note\x18\x0b \x01(\tH\x05\x88\x01\x01\"5\n\x10\x44\x65linvoiceStatus\x12\x08\n\x04PAID\x10\x00\x12\x0b\n\x07\x45XPIRED\x10\x01\x12\n\n\x06UNPAID\x10\x02\x42\t\n\x07_bolt11B\t\n\x07_bolt12B\x0e\n\x0c_amount_msatB\x0e\n\x0c_descriptionB\x11\n\x0f_local_offer_idB\x14\n\x12_invreq_payer_note\"\xb8\x02\n\x0eInvoiceRequest\x12%\n\x0b\x61mount_msat\x18\n \x01(\x0b\x32\x10.cln.AmountOrAny\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05label\x18\x03 \x01(\t\x12\x13\n\x06\x65xpiry\x18\x07 \x01(\x04H\x00\x88\x01\x01\x12\x11\n\tfallbacks\x18\x04 \x03(\t\x12\x15\n\x08preimage\x18\x05 \x01(\x0cH\x01\x88\x01\x01\x12\"\n\x15\x65xposeprivatechannels\x18\x08 \x01(\x08H\x02\x88\x01\x01\x12\x11\n\x04\x63ltv\x18\x06 \x01(\rH\x03\x88\x01\x01\x12\x19\n\x0c\x64\x65schashonly\x18\t \x01(\x08H\x04\x88\x01\x01\x42\t\n\x07_expiryB\x0b\n\t_preimageB\x18\n\x16_exposeprivatechannelsB\x07\n\x05_cltvB\x0f\n\r_deschashonly\"\xe7\x02\n\x0fInvoiceResponse\x12\x0e\n\x06\x62olt11\x18\x01 \x01(\t\x12\x14\n\x0cpayment_hash\x18\x02 \x01(\x0c\x12\x16\n\x0epayment_secret\x18\x03 \x01(\x0c\x12\x12\n\nexpires_at\x18\x04 \x01(\x04\x12\x1d\n\x10warning_capacity\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x1c\n\x0fwarning_offline\x18\x06 \x01(\tH\x01\x88\x01\x01\x12\x1d\n\x10warning_deadends\x18\x07 \x01(\tH\x02\x88\x01\x01\x12#\n\x16warning_private_unused\x18\x08 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0bwarning_mpp\x18\t \x01(\tH\x04\x88\x01\x01\x42\x13\n\x11_warning_capacityB\x12\n\x10_warning_offlineB\x13\n\x11_warning_deadendsB\x19\n\x17_warning_private_unusedB\x0e\n\x0c_warning_mpp\"#\n\x14ListdatastoreRequest\x12\x0b\n\x03key\x18\x02 \x03(\t\"G\n\x15ListdatastoreResponse\x12.\n\tdatastore\x18\x01 \x03(\x0b\x32\x1b.cln.ListdatastoreDatastore\"\x87\x01\n\x16ListdatastoreDatastore\x12\x0b\n\x03key\x18\x01 \x03(\t\x12\x17\n\ngeneration\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x10\n\x03hex\x18\x03 \x01(\x0cH\x01\x88\x01\x01\x12\x13\n\x06string\x18\x04 \x01(\tH\x02\x88\x01\x01\x42\r\n\x0b_generationB\x06\n\x04_hexB\t\n\x07_string\"\xa9\x01\n\x13ListinvoicesRequest\x12\x12\n\x05label\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x16\n\tinvstring\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x19\n\x0cpayment_hash\x18\x03 \x01(\x0cH\x02\x88\x01\x01\x12\x15\n\x08offer_id\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\x08\n\x06_labelB\x0c\n\n_invstringB\x0f\n\r_payment_hashB\x0b\n\t_offer_id\"C\n\x14ListinvoicesResponse\x12+\n\x08invoices\x18\x01 \x03(\x0b\x32\x19.cln.ListinvoicesInvoices\"\xa2\x05\n\x14ListinvoicesInvoices\x12\r\n\x05label\x18\x01 \x01(\t\x12\x18\n\x0b\x64\x65scription\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12\x44\n\x06status\x18\x04 \x01(\x0e\x32\x34.cln.ListinvoicesInvoices.ListinvoicesInvoicesStatus\x12\x12\n\nexpires_at\x18\x05 \x01(\x04\x12%\n\x0b\x61mount_msat\x18\x06 \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x07 \x01(\tH\x02\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x08 \x01(\tH\x03\x88\x01\x01\x12\x1b\n\x0elocal_offer_id\x18\t \x01(\x0cH\x04\x88\x01\x01\x12\x1e\n\x11invreq_payer_note\x18\x0f \x01(\tH\x05\x88\x01\x01\x12\x16\n\tpay_index\x18\x0b \x01(\x04H\x06\x88\x01\x01\x12.\n\x14\x61mount_received_msat\x18\x0c \x01(\x0b\x32\x0b.cln.AmountH\x07\x88\x01\x01\x12\x14\n\x07paid_at\x18\r \x01(\x04H\x08\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\x0e \x01(\x0cH\t\x88\x01\x01\"?\n\x1aListinvoicesInvoicesStatus\x12\n\n\x06UNPAID\x10\x00\x12\x08\n\x04PAID\x10\x01\x12\x0b\n\x07\x45XPIRED\x10\x02\x42\x0e\n\x0c_descriptionB\x0e\n\x0c_amount_msatB\t\n\x07_bolt11B\t\n\x07_bolt12B\x11\n\x0f_local_offer_idB\x14\n\x12_invreq_payer_noteB\x0c\n\n_pay_indexB\x17\n\x15_amount_received_msatB\n\n\x08_paid_atB\x13\n\x11_payment_preimage\"\x8a\x03\n\x10SendonionRequest\x12\r\n\x05onion\x18\x01 \x01(\x0c\x12*\n\tfirst_hop\x18\x02 \x01(\x0b\x32\x17.cln.SendonionFirst_hop\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12\x12\n\x05label\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x16\n\x0eshared_secrets\x18\x05 \x03(\x0c\x12\x13\n\x06partid\x18\x06 \x01(\rH\x01\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x07 \x01(\tH\x02\x88\x01\x01\x12%\n\x0b\x61mount_msat\x18\x0c \x01(\x0b\x32\x0b.cln.AmountH\x03\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\t \x01(\x0cH\x04\x88\x01\x01\x12\x1a\n\rlocalinvreqid\x18\r \x01(\x0cH\x05\x88\x01\x01\x12\x14\n\x07groupid\x18\x0b \x01(\x04H\x06\x88\x01\x01\x42\x08\n\x06_labelB\t\n\x07_partidB\t\n\x07_bolt11B\x0e\n\x0c_amount_msatB\x0e\n\x0c_destinationB\x10\n\x0e_localinvreqidB\n\n\x08_groupid\"\x8b\x04\n\x11SendonionResponse\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x14\n\x0cpayment_hash\x18\x02 \x01(\x0c\x12\x36\n\x06status\x18\x03 \x01(\x0e\x32&.cln.SendonionResponse.SendonionStatus\x12%\n\x0b\x61mount_msat\x18\x04 \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\x05 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\ncreated_at\x18\x06 \x01(\x04\x12%\n\x10\x61mount_sent_msat\x18\x07 \x01(\x0b\x32\x0b.cln.Amount\x12\x12\n\x05label\x18\x08 \x01(\tH\x02\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\t \x01(\tH\x03\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\n \x01(\tH\x04\x88\x01\x01\x12\x13\n\x06partid\x18\r \x01(\x04H\x05\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\x0b \x01(\x0cH\x06\x88\x01\x01\x12\x14\n\x07message\x18\x0c \x01(\tH\x07\x88\x01\x01\",\n\x0fSendonionStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x43OMPLETE\x10\x01\x42\x0e\n\x0c_amount_msatB\x0e\n\x0c_destinationB\x08\n\x06_labelB\t\n\x07_bolt11B\t\n\x07_bolt12B\t\n\x07_partidB\x13\n\x11_payment_preimageB\n\n\x08_message\"Q\n\x12SendonionFirst_hop\x12\n\n\x02id\x18\x01 \x01(\x0c\x12 \n\x0b\x61mount_msat\x18\x02 \x01(\x0b\x32\x0b.cln.Amount\x12\r\n\x05\x64\x65lay\x18\x03 \x01(\r\"\xeb\x01\n\x13ListsendpaysRequest\x12\x13\n\x06\x62olt11\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x19\n\x0cpayment_hash\x18\x02 \x01(\x0cH\x01\x88\x01\x01\x12@\n\x06status\x18\x03 \x01(\x0e\x32+.cln.ListsendpaysRequest.ListsendpaysStatusH\x02\x88\x01\x01\";\n\x12ListsendpaysStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x43OMPLETE\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x42\t\n\x07_bolt11B\x0f\n\r_payment_hashB\t\n\x07_status\"C\n\x14ListsendpaysResponse\x12+\n\x08payments\x18\x01 \x03(\x0b\x32\x19.cln.ListsendpaysPayments\"\xf4\x04\n\x14ListsendpaysPayments\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x0f\n\x07groupid\x18\x02 \x01(\x04\x12\x13\n\x06partid\x18\x0f \x01(\x04H\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12\x44\n\x06status\x18\x04 \x01(\x0e\x32\x34.cln.ListsendpaysPayments.ListsendpaysPaymentsStatus\x12%\n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\x06 \x01(\x0cH\x02\x88\x01\x01\x12\x12\n\ncreated_at\x18\x07 \x01(\x04\x12%\n\x10\x61mount_sent_msat\x18\x08 \x01(\x0b\x32\x0b.cln.Amount\x12\x12\n\x05label\x18\t \x01(\tH\x03\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\n \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0e \x01(\tH\x05\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x0b \x01(\tH\x06\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\x0c \x01(\x0cH\x07\x88\x01\x01\x12\x17\n\nerroronion\x18\r \x01(\x0cH\x08\x88\x01\x01\"C\n\x1aListsendpaysPaymentsStatus\x12\x0b\n\x07PENDING\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x12\x0c\n\x08\x43OMPLETE\x10\x02\x42\t\n\x07_partidB\x0e\n\x0c_amount_msatB\x0e\n\x0c_destinationB\x08\n\x06_labelB\t\n\x07_bolt11B\x0e\n\x0c_descriptionB\t\n\x07_bolt12B\x13\n\x11_payment_preimageB\r\n\x0b_erroronion\"\x19\n\x17ListtransactionsRequest\"S\n\x18ListtransactionsResponse\x12\x37\n\x0ctransactions\x18\x01 \x03(\x0b\x32!.cln.ListtransactionsTransactions\"\xf8\x01\n\x1cListtransactionsTransactions\x12\x0c\n\x04hash\x18\x01 \x01(\x0c\x12\r\n\x05rawtx\x18\x02 \x01(\x0c\x12\x13\n\x0b\x62lockheight\x18\x03 \x01(\r\x12\x0f\n\x07txindex\x18\x04 \x01(\r\x12\x10\n\x08locktime\x18\x07 \x01(\r\x12\x0f\n\x07version\x18\x08 \x01(\r\x12\x37\n\x06inputs\x18\t \x03(\x0b\x32\'.cln.ListtransactionsTransactionsInputs\x12\x39\n\x07outputs\x18\n \x03(\x0b\x32(.cln.ListtransactionsTransactionsOutputs\"\x84\x04\n\"ListtransactionsTransactionsInputs\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\x12\r\n\x05index\x18\x02 \x01(\r\x12\x10\n\x08sequence\x18\x03 \x01(\r\x12\x66\n\titem_type\x18\x04 \x01(\x0e\x32N.cln.ListtransactionsTransactionsInputs.ListtransactionsTransactionsInputsTypeH\x00\x88\x01\x01\x12\x14\n\x07\x63hannel\x18\x05 \x01(\tH\x01\x88\x01\x01\"\x96\x02\n&ListtransactionsTransactionsInputsType\x12\n\n\x06THEIRS\x10\x00\x12\x0b\n\x07\x44\x45POSIT\x10\x01\x12\x0c\n\x08WITHDRAW\x10\x02\x12\x13\n\x0f\x43HANNEL_FUNDING\x10\x03\x12\x18\n\x14\x43HANNEL_MUTUAL_CLOSE\x10\x04\x12\x1c\n\x18\x43HANNEL_UNILATERAL_CLOSE\x10\x05\x12\x11\n\rCHANNEL_SWEEP\x10\x06\x12\x18\n\x14\x43HANNEL_HTLC_SUCCESS\x10\x07\x12\x18\n\x14\x43HANNEL_HTLC_TIMEOUT\x10\x08\x12\x13\n\x0f\x43HANNEL_PENALTY\x10\t\x12\x1c\n\x18\x43HANNEL_UNILATERAL_CHEAT\x10\nB\x0c\n\n_item_typeB\n\n\x08_channel\"\xa0\x04\n#ListtransactionsTransactionsOutputs\x12\r\n\x05index\x18\x01 \x01(\r\x12 \n\x0b\x61mount_msat\x18\x06 \x01(\x0b\x32\x0b.cln.Amount\x12\x14\n\x0cscriptPubKey\x18\x03 \x01(\x0c\x12h\n\titem_type\x18\x04 \x01(\x0e\x32P.cln.ListtransactionsTransactionsOutputs.ListtransactionsTransactionsOutputsTypeH\x00\x88\x01\x01\x12\x14\n\x07\x63hannel\x18\x05 \x01(\tH\x01\x88\x01\x01\"\x97\x02\n\'ListtransactionsTransactionsOutputsType\x12\n\n\x06THEIRS\x10\x00\x12\x0b\n\x07\x44\x45POSIT\x10\x01\x12\x0c\n\x08WITHDRAW\x10\x02\x12\x13\n\x0f\x43HANNEL_FUNDING\x10\x03\x12\x18\n\x14\x43HANNEL_MUTUAL_CLOSE\x10\x04\x12\x1c\n\x18\x43HANNEL_UNILATERAL_CLOSE\x10\x05\x12\x11\n\rCHANNEL_SWEEP\x10\x06\x12\x18\n\x14\x43HANNEL_HTLC_SUCCESS\x10\x07\x12\x18\n\x14\x43HANNEL_HTLC_TIMEOUT\x10\x08\x12\x13\n\x0f\x43HANNEL_PENALTY\x10\t\x12\x1c\n\x18\x43HANNEL_UNILATERAL_CHEAT\x10\nB\x0c\n\n_item_typeB\n\n\x08_channel\"\xda\x03\n\nPayRequest\x12\x0e\n\x06\x62olt11\x18\x01 \x01(\t\x12%\n\x0b\x61mount_msat\x18\r \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x12\n\x05label\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x17\n\nriskfactor\x18\x08 \x01(\x01H\x02\x88\x01\x01\x12\x1a\n\rmaxfeepercent\x18\x04 \x01(\x01H\x03\x88\x01\x01\x12\x16\n\tretry_for\x18\x05 \x01(\rH\x04\x88\x01\x01\x12\x15\n\x08maxdelay\x18\x06 \x01(\rH\x05\x88\x01\x01\x12#\n\texemptfee\x18\x07 \x01(\x0b\x32\x0b.cln.AmountH\x06\x88\x01\x01\x12\x1a\n\rlocalinvreqid\x18\x0e \x01(\x0cH\x07\x88\x01\x01\x12\x0f\n\x07\x65xclude\x18\n \x03(\t\x12 \n\x06maxfee\x18\x0b \x01(\x0b\x32\x0b.cln.AmountH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0c \x01(\tH\t\x88\x01\x01\x42\x0e\n\x0c_amount_msatB\x08\n\x06_labelB\r\n\x0b_riskfactorB\x10\n\x0e_maxfeepercentB\x0c\n\n_retry_forB\x0b\n\t_maxdelayB\x0c\n\n_exemptfeeB\x10\n\x0e_localinvreqidB\t\n\x07_maxfeeB\x0e\n\x0c_description\"\xfb\x02\n\x0bPayResponse\x12\x18\n\x10payment_preimage\x18\x01 \x01(\x0c\x12\x18\n\x0b\x64\x65stination\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12\x12\n\ncreated_at\x18\x04 \x01(\x01\x12\r\n\x05parts\x18\x05 \x01(\r\x12 \n\x0b\x61mount_msat\x18\x06 \x01(\x0b\x32\x0b.cln.Amount\x12%\n\x10\x61mount_sent_msat\x18\x07 \x01(\x0b\x32\x0b.cln.Amount\x12\'\n\x1awarning_partial_completion\x18\x08 \x01(\tH\x01\x88\x01\x01\x12*\n\x06status\x18\t \x01(\x0e\x32\x1a.cln.PayResponse.PayStatus\"2\n\tPayStatus\x12\x0c\n\x08\x43OMPLETE\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x42\x0e\n\x0c_destinationB\x1d\n\x1b_warning_partial_completion\"*\n\x10ListnodesRequest\x12\x0f\n\x02id\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x42\x05\n\x03_id\"7\n\x11ListnodesResponse\x12\"\n\x05nodes\x18\x01 \x03(\x0b\x32\x13.cln.ListnodesNodes\"\xe1\x01\n\x0eListnodesNodes\x12\x0e\n\x06nodeid\x18\x01 \x01(\x0c\x12\x1b\n\x0elast_timestamp\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x12\n\x05\x61lias\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x12\n\x05\x63olor\x18\x04 \x01(\x0cH\x02\x88\x01\x01\x12\x15\n\x08\x66\x65\x61tures\x18\x05 \x01(\x0cH\x03\x88\x01\x01\x12/\n\taddresses\x18\x06 \x03(\x0b\x32\x1c.cln.ListnodesNodesAddressesB\x11\n\x0f_last_timestampB\x08\n\x06_aliasB\x08\n\x06_colorB\x0b\n\t_features\"\xf7\x01\n\x17ListnodesNodesAddresses\x12K\n\titem_type\x18\x01 \x01(\x0e\x32\x38.cln.ListnodesNodesAddresses.ListnodesNodesAddressesType\x12\x0c\n\x04port\x18\x02 \x01(\r\x12\x14\n\x07\x61\x64\x64ress\x18\x03 \x01(\tH\x00\x88\x01\x01\"_\n\x1bListnodesNodesAddressesType\x12\x07\n\x03\x44NS\x10\x00\x12\x08\n\x04IPV4\x10\x01\x12\x08\n\x04IPV6\x10\x02\x12\t\n\x05TORV2\x10\x03\x12\t\n\x05TORV3\x10\x04\x12\r\n\tWEBSOCKET\x10\x05\x42\n\n\x08_address\"g\n\x15WaitanyinvoiceRequest\x12\x1a\n\rlastpay_index\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x14\n\x07timeout\x18\x02 \x01(\x04H\x01\x88\x01\x01\x42\x10\n\x0e_lastpay_indexB\n\n\x08_timeout\"\x93\x04\n\x16WaitanyinvoiceResponse\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12@\n\x06status\x18\x04 \x01(\x0e\x32\x30.cln.WaitanyinvoiceResponse.WaitanyinvoiceStatus\x12\x12\n\nexpires_at\x18\x05 \x01(\x04\x12%\n\x0b\x61mount_msat\x18\x06 \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x07 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x08 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tpay_index\x18\t \x01(\x04H\x03\x88\x01\x01\x12.\n\x14\x61mount_received_msat\x18\n \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x12\x14\n\x07paid_at\x18\x0b \x01(\x04H\x05\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\x0c \x01(\x0cH\x06\x88\x01\x01\"-\n\x14WaitanyinvoiceStatus\x12\x08\n\x04PAID\x10\x00\x12\x0b\n\x07\x45XPIRED\x10\x01\x42\x0e\n\x0c_amount_msatB\t\n\x07_bolt11B\t\n\x07_bolt12B\x0c\n\n_pay_indexB\x17\n\x15_amount_received_msatB\n\n\x08_paid_atB\x13\n\x11_payment_preimage\"#\n\x12WaitinvoiceRequest\x12\r\n\x05label\x18\x01 \x01(\t\"\x87\x04\n\x13WaitinvoiceResponse\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12:\n\x06status\x18\x04 \x01(\x0e\x32*.cln.WaitinvoiceResponse.WaitinvoiceStatus\x12\x12\n\nexpires_at\x18\x05 \x01(\x04\x12%\n\x0b\x61mount_msat\x18\x06 \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x07 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x08 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tpay_index\x18\t \x01(\x04H\x03\x88\x01\x01\x12.\n\x14\x61mount_received_msat\x18\n \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x12\x14\n\x07paid_at\x18\x0b \x01(\x04H\x05\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\x0c \x01(\x0cH\x06\x88\x01\x01\"*\n\x11WaitinvoiceStatus\x12\x08\n\x04PAID\x10\x00\x12\x0b\n\x07\x45XPIRED\x10\x01\x42\x0e\n\x0c_amount_msatB\t\n\x07_bolt11B\t\n\x07_bolt12B\x0c\n\n_pay_indexB\x17\n\x15_amount_received_msatB\n\n\x08_paid_atB\x13\n\x11_payment_preimage\"\x8e\x01\n\x12WaitsendpayRequest\x12\x14\n\x0cpayment_hash\x18\x01 \x01(\x0c\x12\x14\n\x07timeout\x18\x03 \x01(\rH\x00\x88\x01\x01\x12\x13\n\x06partid\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x14\n\x07groupid\x18\x04 \x01(\x04H\x02\x88\x01\x01\x42\n\n\x08_timeoutB\t\n\x07_partidB\n\n\x08_groupid\"\xb2\x04\n\x13WaitsendpayResponse\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x14\n\x07groupid\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12:\n\x06status\x18\x04 \x01(\x0e\x32*.cln.WaitsendpayResponse.WaitsendpayStatus\x12%\n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\x06 \x01(\x0cH\x02\x88\x01\x01\x12\x12\n\ncreated_at\x18\x07 \x01(\x04\x12\x19\n\x0c\x63ompleted_at\x18\x0e \x01(\x01H\x03\x88\x01\x01\x12%\n\x10\x61mount_sent_msat\x18\x08 \x01(\x0b\x32\x0b.cln.Amount\x12\x12\n\x05label\x18\t \x01(\tH\x04\x88\x01\x01\x12\x13\n\x06partid\x18\n \x01(\x04H\x05\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x0b \x01(\tH\x06\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\r \x01(\x0cH\x08\x88\x01\x01\"!\n\x11WaitsendpayStatus\x12\x0c\n\x08\x43OMPLETE\x10\x00\x42\n\n\x08_groupidB\x0e\n\x0c_amount_msatB\x0e\n\x0c_destinationB\x0f\n\r_completed_atB\x08\n\x06_labelB\t\n\x07_partidB\t\n\x07_bolt11B\t\n\x07_bolt12B\x13\n\x11_payment_preimage\"\x8d\x01\n\x0eNewaddrRequest\x12@\n\x0b\x61\x64\x64resstype\x18\x01 \x01(\x0e\x32&.cln.NewaddrRequest.NewaddrAddresstypeH\x00\x88\x01\x01\")\n\x12NewaddrAddresstype\x12\n\n\x06\x42\x45\x43H32\x10\x00\x12\x07\n\x03\x41LL\x10\x02\x42\x0e\n\x0c_addresstype\"[\n\x0fNewaddrResponse\x12\x13\n\x06\x62\x65\x63h32\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0bp2sh_segwit\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\t\n\x07_bech32B\x0e\n\x0c_p2sh_segwit\"\xca\x01\n\x0fWithdrawRequest\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\t\x12&\n\x07satoshi\x18\x02 \x01(\x0b\x32\x10.cln.AmountOrAllH\x00\x88\x01\x01\x12\"\n\x07\x66\x65\x65rate\x18\x05 \x01(\x0b\x32\x0c.cln.FeerateH\x01\x88\x01\x01\x12\x14\n\x07minconf\x18\x03 \x01(\rH\x02\x88\x01\x01\x12\x1c\n\x05utxos\x18\x04 \x03(\x0b\x32\r.cln.OutpointB\n\n\x08_satoshiB\n\n\x08_feerateB\n\n\x08_minconf\":\n\x10WithdrawResponse\x12\n\n\x02tx\x18\x01 \x01(\x0c\x12\x0c\n\x04txid\x18\x02 \x01(\x0c\x12\x0c\n\x04psbt\x18\x03 \x01(\t\"\x82\x03\n\x0eKeysendRequest\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\x0c\x12 \n\x0b\x61mount_msat\x18\n \x01(\x0b\x32\x0b.cln.Amount\x12\x12\n\x05label\x18\x03 \x01(\tH\x00\x88\x01\x01\x12\x1a\n\rmaxfeepercent\x18\x04 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\tretry_for\x18\x05 \x01(\rH\x02\x88\x01\x01\x12\x15\n\x08maxdelay\x18\x06 \x01(\rH\x03\x88\x01\x01\x12#\n\texemptfee\x18\x07 \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x12+\n\nroutehints\x18\x08 \x01(\x0b\x32\x12.cln.RoutehintListH\x05\x88\x01\x01\x12&\n\textratlvs\x18\t \x01(\x0b\x32\x0e.cln.TlvStreamH\x06\x88\x01\x01\x42\x08\n\x06_labelB\x10\n\x0e_maxfeepercentB\x0c\n\n_retry_forB\x0b\n\t_maxdelayB\x0c\n\n_exemptfeeB\r\n\x0b_routehintsB\x0c\n\n_extratlvs\"\xf2\x02\n\x0fKeysendResponse\x12\x18\n\x10payment_preimage\x18\x01 \x01(\x0c\x12\x18\n\x0b\x64\x65stination\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12\x12\n\ncreated_at\x18\x04 \x01(\x01\x12\r\n\x05parts\x18\x05 \x01(\r\x12 \n\x0b\x61mount_msat\x18\x06 \x01(\x0b\x32\x0b.cln.Amount\x12%\n\x10\x61mount_sent_msat\x18\x07 \x01(\x0b\x32\x0b.cln.Amount\x12\'\n\x1awarning_partial_completion\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x32\n\x06status\x18\t \x01(\x0e\x32\".cln.KeysendResponse.KeysendStatus\"\x1d\n\rKeysendStatus\x12\x0c\n\x08\x43OMPLETE\x10\x00\x42\x0e\n\x0c_destinationB\x1d\n\x1b_warning_partial_completion\"\xbc\x02\n\x0f\x46undpsbtRequest\x12!\n\x07satoshi\x18\x01 \x01(\x0b\x32\x10.cln.AmountOrAll\x12\x1d\n\x07\x66\x65\x65rate\x18\x02 \x01(\x0b\x32\x0c.cln.Feerate\x12\x13\n\x0bstartweight\x18\x03 \x01(\r\x12\x14\n\x07minconf\x18\x04 \x01(\rH\x00\x88\x01\x01\x12\x14\n\x07reserve\x18\x05 \x01(\rH\x01\x88\x01\x01\x12\x15\n\x08locktime\x18\x06 \x01(\rH\x02\x88\x01\x01\x12\x1f\n\x12min_witness_weight\x18\x07 \x01(\rH\x03\x88\x01\x01\x12\x1d\n\x10\x65xcess_as_change\x18\x08 \x01(\x08H\x04\x88\x01\x01\x42\n\n\x08_minconfB\n\n\x08_reserveB\x0b\n\t_locktimeB\x15\n\x13_min_witness_weightB\x13\n\x11_excess_as_change\"\xd9\x01\n\x10\x46undpsbtResponse\x12\x0c\n\x04psbt\x18\x01 \x01(\t\x12\x16\n\x0e\x66\x65\x65rate_per_kw\x18\x02 \x01(\r\x12\x1e\n\x16\x65stimated_final_weight\x18\x03 \x01(\r\x12 \n\x0b\x65xcess_msat\x18\x04 \x01(\x0b\x32\x0b.cln.Amount\x12\x1a\n\rchange_outnum\x18\x05 \x01(\rH\x00\x88\x01\x01\x12/\n\x0creservations\x18\x06 \x03(\x0b\x32\x19.cln.FundpsbtReservationsB\x10\n\x0e_change_outnum\"u\n\x14\x46undpsbtReservations\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\x12\x0c\n\x04vout\x18\x02 \x01(\r\x12\x14\n\x0cwas_reserved\x18\x03 \x01(\x08\x12\x10\n\x08reserved\x18\x04 \x01(\x08\x12\x19\n\x11reserved_to_block\x18\x05 \x01(\r\"A\n\x0fSendpsbtRequest\x12\x0c\n\x04psbt\x18\x01 \x01(\t\x12\x14\n\x07reserve\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\n\n\x08_reserve\",\n\x10SendpsbtResponse\x12\n\n\x02tx\x18\x01 \x01(\x0c\x12\x0c\n\x04txid\x18\x02 \x01(\x0c\"1\n\x0fSignpsbtRequest\x12\x0c\n\x04psbt\x18\x01 \x01(\t\x12\x10\n\x08signonly\x18\x02 \x03(\r\"\'\n\x10SignpsbtResponse\x12\x13\n\x0bsigned_psbt\x18\x01 \x01(\t\"\xdb\x02\n\x0fUtxopsbtRequest\x12\x1c\n\x07satoshi\x18\x01 \x01(\x0b\x32\x0b.cln.Amount\x12\x1d\n\x07\x66\x65\x65rate\x18\x02 \x01(\x0b\x32\x0c.cln.Feerate\x12\x13\n\x0bstartweight\x18\x03 \x01(\r\x12\x1c\n\x05utxos\x18\x04 \x03(\x0b\x32\r.cln.Outpoint\x12\x14\n\x07reserve\x18\x05 \x01(\rH\x00\x88\x01\x01\x12\x17\n\nreservedok\x18\x08 \x01(\x08H\x01\x88\x01\x01\x12\x15\n\x08locktime\x18\x06 \x01(\rH\x02\x88\x01\x01\x12\x1f\n\x12min_witness_weight\x18\x07 \x01(\rH\x03\x88\x01\x01\x12\x1d\n\x10\x65xcess_as_change\x18\t \x01(\x08H\x04\x88\x01\x01\x42\n\n\x08_reserveB\r\n\x0b_reservedokB\x0b\n\t_locktimeB\x15\n\x13_min_witness_weightB\x13\n\x11_excess_as_change\"\xd9\x01\n\x10UtxopsbtResponse\x12\x0c\n\x04psbt\x18\x01 \x01(\t\x12\x16\n\x0e\x66\x65\x65rate_per_kw\x18\x02 \x01(\r\x12\x1e\n\x16\x65stimated_final_weight\x18\x03 \x01(\r\x12 \n\x0b\x65xcess_msat\x18\x04 \x01(\x0b\x32\x0b.cln.Amount\x12\x1a\n\rchange_outnum\x18\x05 \x01(\rH\x00\x88\x01\x01\x12/\n\x0creservations\x18\x06 \x03(\x0b\x32\x19.cln.UtxopsbtReservationsB\x10\n\x0e_change_outnum\"u\n\x14UtxopsbtReservations\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\x12\x0c\n\x04vout\x18\x02 \x01(\r\x12\x14\n\x0cwas_reserved\x18\x03 \x01(\x08\x12\x10\n\x08reserved\x18\x04 \x01(\x08\x12\x19\n\x11reserved_to_block\x18\x05 \x01(\r\" \n\x10TxdiscardRequest\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\"6\n\x11TxdiscardResponse\x12\x13\n\x0bunsigned_tx\x18\x01 \x01(\x0c\x12\x0c\n\x04txid\x18\x02 \x01(\x0c\"\xa4\x01\n\x10TxprepareRequest\x12 \n\x07outputs\x18\x05 \x03(\x0b\x32\x0f.cln.OutputDesc\x12\"\n\x07\x66\x65\x65rate\x18\x02 \x01(\x0b\x32\x0c.cln.FeerateH\x00\x88\x01\x01\x12\x14\n\x07minconf\x18\x03 \x01(\rH\x01\x88\x01\x01\x12\x1c\n\x05utxos\x18\x04 \x03(\x0b\x32\r.cln.OutpointB\n\n\x08_feerateB\n\n\x08_minconf\"D\n\x11TxprepareResponse\x12\x0c\n\x04psbt\x18\x01 \x01(\t\x12\x13\n\x0bunsigned_tx\x18\x02 \x01(\x0c\x12\x0c\n\x04txid\x18\x03 \x01(\x0c\"\x1d\n\rTxsendRequest\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\"8\n\x0eTxsendResponse\x12\x0c\n\x04psbt\x18\x01 \x01(\t\x12\n\n\x02tx\x18\x02 \x01(\x0c\x12\x0c\n\x04txid\x18\x03 \x01(\x0c\"=\n\x11\x44isconnectRequest\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x12\n\x05\x66orce\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_force\"\x14\n\x12\x44isconnectResponse\"k\n\x0f\x46\x65\x65ratesRequest\x12\x31\n\x05style\x18\x01 \x01(\x0e\x32\".cln.FeeratesRequest.FeeratesStyle\"%\n\rFeeratesStyle\x12\t\n\x05PERKB\x10\x00\x12\t\n\x05PERKW\x10\x01\"\x9c\x02\n\x10\x46\x65\x65ratesResponse\x12%\n\x18warning_missing_feerates\x18\x01 \x01(\tH\x00\x88\x01\x01\x12&\n\x05perkb\x18\x02 \x01(\x0b\x32\x12.cln.FeeratesPerkbH\x01\x88\x01\x01\x12&\n\x05perkw\x18\x03 \x01(\x0b\x32\x12.cln.FeeratesPerkwH\x02\x88\x01\x01\x12\x46\n\x15onchain_fee_estimates\x18\x04 \x01(\x0b\x32\".cln.FeeratesOnchain_fee_estimatesH\x03\x88\x01\x01\x42\x1b\n\x19_warning_missing_feeratesB\x08\n\x06_perkbB\x08\n\x06_perkwB\x18\n\x16_onchain_fee_estimates\"\xc3\x02\n\rFeeratesPerkb\x12\x16\n\x0emin_acceptable\x18\x01 \x01(\r\x12\x16\n\x0emax_acceptable\x18\x02 \x01(\r\x12\x14\n\x07opening\x18\x03 \x01(\rH\x00\x88\x01\x01\x12\x19\n\x0cmutual_close\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x1d\n\x10unilateral_close\x18\x05 \x01(\rH\x02\x88\x01\x01\x12\x1a\n\rdelayed_to_us\x18\x06 \x01(\rH\x03\x88\x01\x01\x12\x1c\n\x0fhtlc_resolution\x18\x07 \x01(\rH\x04\x88\x01\x01\x12\x14\n\x07penalty\x18\x08 \x01(\rH\x05\x88\x01\x01\x42\n\n\x08_openingB\x0f\n\r_mutual_closeB\x13\n\x11_unilateral_closeB\x10\n\x0e_delayed_to_usB\x12\n\x10_htlc_resolutionB\n\n\x08_penalty\"\xc3\x02\n\rFeeratesPerkw\x12\x16\n\x0emin_acceptable\x18\x01 \x01(\r\x12\x16\n\x0emax_acceptable\x18\x02 \x01(\r\x12\x14\n\x07opening\x18\x03 \x01(\rH\x00\x88\x01\x01\x12\x19\n\x0cmutual_close\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x1d\n\x10unilateral_close\x18\x05 \x01(\rH\x02\x88\x01\x01\x12\x1a\n\rdelayed_to_us\x18\x06 \x01(\rH\x03\x88\x01\x01\x12\x1c\n\x0fhtlc_resolution\x18\x07 \x01(\rH\x04\x88\x01\x01\x12\x14\n\x07penalty\x18\x08 \x01(\rH\x05\x88\x01\x01\x42\n\n\x08_openingB\x0f\n\r_mutual_closeB\x13\n\x11_unilateral_closeB\x10\n\x0e_delayed_to_usB\x12\n\x10_htlc_resolutionB\n\n\x08_penalty\"\xc1\x01\n\x1d\x46\x65\x65ratesOnchain_fee_estimates\x12 \n\x18opening_channel_satoshis\x18\x01 \x01(\x04\x12\x1d\n\x15mutual_close_satoshis\x18\x02 \x01(\x04\x12!\n\x19unilateral_close_satoshis\x18\x03 \x01(\x04\x12\x1d\n\x15htlc_timeout_satoshis\x18\x04 \x01(\x04\x12\x1d\n\x15htlc_success_satoshis\x18\x05 \x01(\x04\"\xe5\x03\n\x12\x46undchannelRequest\x12\n\n\x02id\x18\t \x01(\x0c\x12 \n\x06\x61mount\x18\x01 \x01(\x0b\x32\x10.cln.AmountOrAll\x12\"\n\x07\x66\x65\x65rate\x18\x02 \x01(\x0b\x32\x0c.cln.FeerateH\x00\x88\x01\x01\x12\x15\n\x08\x61nnounce\x18\x03 \x01(\x08H\x01\x88\x01\x01\x12\x14\n\x07minconf\x18\n \x01(\rH\x02\x88\x01\x01\x12#\n\tpush_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x03\x88\x01\x01\x12\x15\n\x08\x63lose_to\x18\x06 \x01(\tH\x04\x88\x01\x01\x12%\n\x0brequest_amt\x18\x07 \x01(\x0b\x32\x0b.cln.AmountH\x05\x88\x01\x01\x12\x1a\n\rcompact_lease\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x1c\n\x05utxos\x18\x0b \x03(\x0b\x32\r.cln.Outpoint\x12\x15\n\x08mindepth\x18\x0c \x01(\rH\x07\x88\x01\x01\x12!\n\x07reserve\x18\r \x01(\x0b\x32\x0b.cln.AmountH\x08\x88\x01\x01\x42\n\n\x08_feerateB\x0b\n\t_announceB\n\n\x08_minconfB\x0c\n\n_push_msatB\x0b\n\t_close_toB\x0e\n\x0c_request_amtB\x10\n\x0e_compact_leaseB\x0b\n\t_mindepthB\n\n\x08_reserve\"\x9b\x01\n\x13\x46undchannelResponse\x12\n\n\x02tx\x18\x01 \x01(\x0c\x12\x0c\n\x04txid\x18\x02 \x01(\x0c\x12\x0e\n\x06outnum\x18\x03 \x01(\r\x12\x12\n\nchannel_id\x18\x04 \x01(\x0c\x12\x15\n\x08\x63lose_to\x18\x05 \x01(\x0cH\x00\x88\x01\x01\x12\x15\n\x08mindepth\x18\x06 \x01(\rH\x01\x88\x01\x01\x42\x0b\n\t_close_toB\x0b\n\t_mindepth\"\xec\x01\n\x0fGetrouteRequest\x12\n\n\x02id\x18\x01 \x01(\x0c\x12 \n\x0b\x61mount_msat\x18\t \x01(\x0b\x32\x0b.cln.Amount\x12\x12\n\nriskfactor\x18\x03 \x01(\x04\x12\x11\n\x04\x63ltv\x18\x04 \x01(\x01H\x00\x88\x01\x01\x12\x13\n\x06\x66romid\x18\x05 \x01(\x0cH\x01\x88\x01\x01\x12\x18\n\x0b\x66uzzpercent\x18\x06 \x01(\rH\x02\x88\x01\x01\x12\x0f\n\x07\x65xclude\x18\x07 \x03(\t\x12\x14\n\x07maxhops\x18\x08 \x01(\rH\x03\x88\x01\x01\x42\x07\n\x05_cltvB\t\n\x07_fromidB\x0e\n\x0c_fuzzpercentB\n\n\x08_maxhops\"5\n\x10GetrouteResponse\x12!\n\x05route\x18\x01 \x03(\x0b\x32\x12.cln.GetrouteRoute\"\xe9\x01\n\rGetrouteRoute\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\t\x12\x11\n\tdirection\x18\x03 \x01(\r\x12\x15\n\x08msatoshi\x18\x07 \x01(\x04H\x00\x88\x01\x01\x12 \n\x0b\x61mount_msat\x18\x04 \x01(\x0b\x32\x0b.cln.Amount\x12\r\n\x05\x64\x65lay\x18\x05 \x01(\r\x12\x34\n\x05style\x18\x06 \x01(\x0e\x32%.cln.GetrouteRoute.GetrouteRouteStyle\"\x1d\n\x12GetrouteRouteStyle\x12\x07\n\x03TLV\x10\x00\x42\x0b\n\t_msatoshi\"\x82\x02\n\x13ListforwardsRequest\x12@\n\x06status\x18\x01 \x01(\x0e\x32+.cln.ListforwardsRequest.ListforwardsStatusH\x00\x88\x01\x01\x12\x17\n\nin_channel\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x0bout_channel\x18\x03 \x01(\tH\x02\x88\x01\x01\"L\n\x12ListforwardsStatus\x12\x0b\n\x07OFFERED\x10\x00\x12\x0b\n\x07SETTLED\x10\x01\x12\x10\n\x0cLOCAL_FAILED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x42\t\n\x07_statusB\r\n\x0b_in_channelB\x0e\n\x0c_out_channel\"C\n\x14ListforwardsResponse\x12+\n\x08\x66orwards\x18\x01 \x03(\x0b\x32\x19.cln.ListforwardsForwards\"\xde\x04\n\x14ListforwardsForwards\x12\x12\n\nin_channel\x18\x01 \x01(\t\x12\x17\n\nin_htlc_id\x18\n \x01(\x04H\x00\x88\x01\x01\x12\x1c\n\x07in_msat\x18\x02 \x01(\x0b\x32\x0b.cln.Amount\x12\x44\n\x06status\x18\x03 \x01(\x0e\x32\x34.cln.ListforwardsForwards.ListforwardsForwardsStatus\x12\x15\n\rreceived_time\x18\x04 \x01(\x01\x12\x18\n\x0bout_channel\x18\x05 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x0bout_htlc_id\x18\x0b \x01(\x04H\x02\x88\x01\x01\x12G\n\x05style\x18\t \x01(\x0e\x32\x33.cln.ListforwardsForwards.ListforwardsForwardsStyleH\x03\x88\x01\x01\x12\"\n\x08\x66\x65\x65_msat\x18\x07 \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x12\"\n\x08out_msat\x18\x08 \x01(\x0b\x32\x0b.cln.AmountH\x05\x88\x01\x01\"T\n\x1aListforwardsForwardsStatus\x12\x0b\n\x07OFFERED\x10\x00\x12\x0b\n\x07SETTLED\x10\x01\x12\x10\n\x0cLOCAL_FAILED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\"0\n\x19ListforwardsForwardsStyle\x12\n\n\x06LEGACY\x10\x00\x12\x07\n\x03TLV\x10\x01\x42\r\n\x0b_in_htlc_idB\x0e\n\x0c_out_channelB\x0e\n\x0c_out_htlc_idB\x08\n\x06_styleB\x0b\n\t_fee_msatB\x0b\n\t_out_msat\"\xdb\x01\n\x0fListpaysRequest\x12\x13\n\x06\x62olt11\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x19\n\x0cpayment_hash\x18\x02 \x01(\x0cH\x01\x88\x01\x01\x12\x38\n\x06status\x18\x03 \x01(\x0e\x32#.cln.ListpaysRequest.ListpaysStatusH\x02\x88\x01\x01\"7\n\x0eListpaysStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x43OMPLETE\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x42\t\n\x07_bolt11B\x0f\n\r_payment_hashB\t\n\x07_status\"3\n\x10ListpaysResponse\x12\x1f\n\x04pays\x18\x01 \x03(\x0b\x32\x11.cln.ListpaysPays\"\x87\x04\n\x0cListpaysPays\x12\x14\n\x0cpayment_hash\x18\x01 \x01(\x0c\x12\x34\n\x06status\x18\x02 \x01(\x0e\x32$.cln.ListpaysPays.ListpaysPaysStatus\x12\x18\n\x0b\x64\x65stination\x18\x03 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\ncreated_at\x18\x04 \x01(\x04\x12\x19\n\x0c\x63ompleted_at\x18\x0c \x01(\x04H\x01\x88\x01\x01\x12\x12\n\x05label\x18\x05 \x01(\tH\x02\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x06 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0b \x01(\tH\x04\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x07 \x01(\tH\x05\x88\x01\x01\x12\x15\n\x08preimage\x18\r \x01(\x0cH\x06\x88\x01\x01\x12\x1c\n\x0fnumber_of_parts\x18\x0e \x01(\x04H\x07\x88\x01\x01\x12\x17\n\nerroronion\x18\n \x01(\x0cH\x08\x88\x01\x01\";\n\x12ListpaysPaysStatus\x12\x0b\n\x07PENDING\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x12\x0c\n\x08\x43OMPLETE\x10\x02\x42\x0e\n\x0c_destinationB\x0f\n\r_completed_atB\x08\n\x06_labelB\t\n\x07_bolt11B\x0e\n\x0c_descriptionB\t\n\x07_bolt12B\x0b\n\t_preimageB\x12\n\x10_number_of_partsB\r\n\x0b_erroronion\"Y\n\x0bPingRequest\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x10\n\x03len\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x16\n\tpongbytes\x18\x03 \x01(\rH\x01\x88\x01\x01\x42\x06\n\x04_lenB\x0c\n\n_pongbytes\"\x1e\n\x0cPingResponse\x12\x0e\n\x06totlen\x18\x01 \x01(\r\"4\n\x14SendcustommsgRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12\x0b\n\x03msg\x18\x02 \x01(\x0c\"\'\n\x15SendcustommsgResponse\x12\x0e\n\x06status\x18\x01 \x01(\t\"\xf8\x01\n\x11SetchannelRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12!\n\x07\x66\x65\x65\x62\x61se\x18\x02 \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x13\n\x06\x66\x65\x65ppm\x18\x03 \x01(\rH\x01\x88\x01\x01\x12!\n\x07htlcmin\x18\x04 \x01(\x0b\x32\x0b.cln.AmountH\x02\x88\x01\x01\x12!\n\x07htlcmax\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x03\x88\x01\x01\x12\x19\n\x0c\x65nforcedelay\x18\x06 \x01(\rH\x04\x88\x01\x01\x42\n\n\x08_feebaseB\t\n\x07_feeppmB\n\n\x08_htlcminB\n\n\x08_htlcmaxB\x0f\n\r_enforcedelay\"?\n\x12SetchannelResponse\x12)\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x17.cln.SetchannelChannels\"\x94\x03\n\x12SetchannelChannels\x12\x0f\n\x07peer_id\x18\x01 \x01(\x0c\x12\x12\n\nchannel_id\x18\x02 \x01(\x0c\x12\x1d\n\x10short_channel_id\x18\x03 \x01(\tH\x00\x88\x01\x01\x12\"\n\rfee_base_msat\x18\x04 \x01(\x0b\x32\x0b.cln.Amount\x12#\n\x1b\x66\x65\x65_proportional_millionths\x18\x05 \x01(\r\x12*\n\x15minimum_htlc_out_msat\x18\x06 \x01(\x0b\x32\x0b.cln.Amount\x12$\n\x17warning_htlcmin_too_low\x18\x07 \x01(\tH\x01\x88\x01\x01\x12*\n\x15maximum_htlc_out_msat\x18\x08 \x01(\x0b\x32\x0b.cln.Amount\x12%\n\x18warning_htlcmax_too_high\x18\t \x01(\tH\x02\x88\x01\x01\x42\x13\n\x11_short_channel_idB\x1a\n\x18_warning_htlcmin_too_lowB\x1b\n\x19_warning_htlcmax_too_high\"\'\n\x12SigninvoiceRequest\x12\x11\n\tinvstring\x18\x01 \x01(\t\"%\n\x13SigninvoiceResponse\x12\x0e\n\x06\x62olt11\x18\x01 \x01(\t\"%\n\x12SignmessageRequest\x12\x0f\n\x07message\x18\x01 \x01(\t\"F\n\x13SignmessageResponse\x12\x11\n\tsignature\x18\x01 \x01(\x0c\x12\r\n\x05recid\x18\x02 \x01(\x0c\x12\r\n\x05zbase\x18\x03 \x01(\t\"\r\n\x0bStopRequest\"\x0e\n\x0cStopResponse2\xbf\x18\n\x04Node\x12\x36\n\x07Getinfo\x12\x13.cln.GetinfoRequest\x1a\x14.cln.GetinfoResponse\"\x00\x12<\n\tListPeers\x12\x15.cln.ListpeersRequest\x1a\x16.cln.ListpeersResponse\"\x00\x12<\n\tListFunds\x12\x15.cln.ListfundsRequest\x1a\x16.cln.ListfundsResponse\"\x00\x12\x36\n\x07SendPay\x12\x13.cln.SendpayRequest\x1a\x14.cln.SendpayResponse\"\x00\x12\x45\n\x0cListChannels\x12\x18.cln.ListchannelsRequest\x1a\x19.cln.ListchannelsResponse\"\x00\x12<\n\tAddGossip\x12\x15.cln.AddgossipRequest\x1a\x16.cln.AddgossipResponse\"\x00\x12Q\n\x10\x41utoCleanInvoice\x12\x1c.cln.AutocleaninvoiceRequest\x1a\x1d.cln.AutocleaninvoiceResponse\"\x00\x12\x45\n\x0c\x43heckMessage\x12\x18.cln.CheckmessageRequest\x1a\x19.cln.CheckmessageResponse\"\x00\x12\x30\n\x05\x43lose\x12\x11.cln.CloseRequest\x1a\x12.cln.CloseResponse\"\x00\x12:\n\x0b\x43onnectPeer\x12\x13.cln.ConnectRequest\x1a\x14.cln.ConnectResponse\"\x00\x12H\n\rCreateInvoice\x12\x19.cln.CreateinvoiceRequest\x1a\x1a.cln.CreateinvoiceResponse\"\x00\x12<\n\tDatastore\x12\x15.cln.DatastoreRequest\x1a\x16.cln.DatastoreResponse\"\x00\x12\x42\n\x0b\x43reateOnion\x12\x17.cln.CreateonionRequest\x1a\x18.cln.CreateonionResponse\"\x00\x12\x45\n\x0c\x44\x65lDatastore\x12\x18.cln.DeldatastoreRequest\x1a\x19.cln.DeldatastoreResponse\"\x00\x12T\n\x11\x44\x65lExpiredInvoice\x12\x1d.cln.DelexpiredinvoiceRequest\x1a\x1e.cln.DelexpiredinvoiceResponse\"\x00\x12?\n\nDelInvoice\x12\x16.cln.DelinvoiceRequest\x1a\x17.cln.DelinvoiceResponse\"\x00\x12\x36\n\x07Invoice\x12\x13.cln.InvoiceRequest\x1a\x14.cln.InvoiceResponse\"\x00\x12H\n\rListDatastore\x12\x19.cln.ListdatastoreRequest\x1a\x1a.cln.ListdatastoreResponse\"\x00\x12\x45\n\x0cListInvoices\x12\x18.cln.ListinvoicesRequest\x1a\x19.cln.ListinvoicesResponse\"\x00\x12<\n\tSendOnion\x12\x15.cln.SendonionRequest\x1a\x16.cln.SendonionResponse\"\x00\x12\x45\n\x0cListSendPays\x12\x18.cln.ListsendpaysRequest\x1a\x19.cln.ListsendpaysResponse\"\x00\x12Q\n\x10ListTransactions\x12\x1c.cln.ListtransactionsRequest\x1a\x1d.cln.ListtransactionsResponse\"\x00\x12*\n\x03Pay\x12\x0f.cln.PayRequest\x1a\x10.cln.PayResponse\"\x00\x12<\n\tListNodes\x12\x15.cln.ListnodesRequest\x1a\x16.cln.ListnodesResponse\"\x00\x12K\n\x0eWaitAnyInvoice\x12\x1a.cln.WaitanyinvoiceRequest\x1a\x1b.cln.WaitanyinvoiceResponse\"\x00\x12\x42\n\x0bWaitInvoice\x12\x17.cln.WaitinvoiceRequest\x1a\x18.cln.WaitinvoiceResponse\"\x00\x12\x42\n\x0bWaitSendPay\x12\x17.cln.WaitsendpayRequest\x1a\x18.cln.WaitsendpayResponse\"\x00\x12\x36\n\x07NewAddr\x12\x13.cln.NewaddrRequest\x1a\x14.cln.NewaddrResponse\"\x00\x12\x39\n\x08Withdraw\x12\x14.cln.WithdrawRequest\x1a\x15.cln.WithdrawResponse\"\x00\x12\x36\n\x07KeySend\x12\x13.cln.KeysendRequest\x1a\x14.cln.KeysendResponse\"\x00\x12\x39\n\x08\x46undPsbt\x12\x14.cln.FundpsbtRequest\x1a\x15.cln.FundpsbtResponse\"\x00\x12\x39\n\x08SendPsbt\x12\x14.cln.SendpsbtRequest\x1a\x15.cln.SendpsbtResponse\"\x00\x12\x39\n\x08SignPsbt\x12\x14.cln.SignpsbtRequest\x1a\x15.cln.SignpsbtResponse\"\x00\x12\x39\n\x08UtxoPsbt\x12\x14.cln.UtxopsbtRequest\x1a\x15.cln.UtxopsbtResponse\"\x00\x12<\n\tTxDiscard\x12\x15.cln.TxdiscardRequest\x1a\x16.cln.TxdiscardResponse\"\x00\x12<\n\tTxPrepare\x12\x15.cln.TxprepareRequest\x1a\x16.cln.TxprepareResponse\"\x00\x12\x33\n\x06TxSend\x12\x12.cln.TxsendRequest\x1a\x13.cln.TxsendResponse\"\x00\x12?\n\nDisconnect\x12\x16.cln.DisconnectRequest\x1a\x17.cln.DisconnectResponse\"\x00\x12\x39\n\x08\x46\x65\x65rates\x12\x14.cln.FeeratesRequest\x1a\x15.cln.FeeratesResponse\"\x00\x12\x42\n\x0b\x46undChannel\x12\x17.cln.FundchannelRequest\x1a\x18.cln.FundchannelResponse\"\x00\x12\x39\n\x08GetRoute\x12\x14.cln.GetrouteRequest\x1a\x15.cln.GetrouteResponse\"\x00\x12\x45\n\x0cListForwards\x12\x18.cln.ListforwardsRequest\x1a\x19.cln.ListforwardsResponse\"\x00\x12\x39\n\x08ListPays\x12\x14.cln.ListpaysRequest\x1a\x15.cln.ListpaysResponse\"\x00\x12-\n\x04Ping\x12\x10.cln.PingRequest\x1a\x11.cln.PingResponse\"\x00\x12H\n\rSendCustomMsg\x12\x19.cln.SendcustommsgRequest\x1a\x1a.cln.SendcustommsgResponse\"\x00\x12?\n\nSetChannel\x12\x16.cln.SetchannelRequest\x1a\x17.cln.SetchannelResponse\"\x00\x12\x42\n\x0bSignInvoice\x12\x17.cln.SigninvoiceRequest\x1a\x18.cln.SigninvoiceResponse\"\x00\x12\x42\n\x0bSignMessage\x12\x17.cln.SignmessageRequest\x1a\x18.cln.SignmessageResponse\"\x00\x12-\n\x04Stop\x12\x10.cln.StopRequest\x1a\x11.cln.StopResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nnode.proto\x12\x03\x63ln\x1a\x10primitives.proto\"\x10\n\x0eGetinfoRequest\"\xb2\x04\n\x0fGetinfoResponse\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\x0c\x12\x11\n\tnum_peers\x18\x04 \x01(\r\x12\x1c\n\x14num_pending_channels\x18\x05 \x01(\r\x12\x1b\n\x13num_active_channels\x18\x06 \x01(\r\x12\x1d\n\x15num_inactive_channels\x18\x07 \x01(\r\x12\x0f\n\x07version\x18\x08 \x01(\t\x12\x15\n\rlightning_dir\x18\t \x01(\t\x12\x33\n\x0cour_features\x18\n \x01(\x0b\x32\x18.cln.GetinfoOur_featuresH\x00\x88\x01\x01\x12\x13\n\x0b\x62lockheight\x18\x0b \x01(\r\x12\x0f\n\x07network\x18\x0c \x01(\t\x12(\n\x13\x66\x65\x65s_collected_msat\x18\r \x01(\x0b\x32\x0b.cln.Amount\x12$\n\x07\x61\x64\x64ress\x18\x0e \x03(\x0b\x32\x13.cln.GetinfoAddress\x12$\n\x07\x62inding\x18\x0f \x03(\x0b\x32\x13.cln.GetinfoBinding\x12\"\n\x15warning_bitcoind_sync\x18\x10 \x01(\tH\x01\x88\x01\x01\x12$\n\x17warning_lightningd_sync\x18\x11 \x01(\tH\x02\x88\x01\x01\x42\x0f\n\r_our_featuresB\x18\n\x16_warning_bitcoind_syncB\x1a\n\x18_warning_lightningd_sync\"S\n\x13GetinfoOur_features\x12\x0c\n\x04init\x18\x01 \x01(\x0c\x12\x0c\n\x04node\x18\x02 \x01(\x0c\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\x0c\x12\x0f\n\x07invoice\x18\x04 \x01(\x0c\"\xd3\x01\n\x0eGetinfoAddress\x12\x39\n\titem_type\x18\x01 \x01(\x0e\x32&.cln.GetinfoAddress.GetinfoAddressType\x12\x0c\n\x04port\x18\x02 \x01(\r\x12\x14\n\x07\x61\x64\x64ress\x18\x03 \x01(\tH\x00\x88\x01\x01\"V\n\x12GetinfoAddressType\x12\x07\n\x03\x44NS\x10\x00\x12\x08\n\x04IPV4\x10\x01\x12\x08\n\x04IPV6\x10\x02\x12\t\n\x05TORV2\x10\x03\x12\t\n\x05TORV3\x10\x04\x12\r\n\tWEBSOCKET\x10\x05\x42\n\n\x08_address\"\xfb\x01\n\x0eGetinfoBinding\x12\x39\n\titem_type\x18\x01 \x01(\x0e\x32&.cln.GetinfoBinding.GetinfoBindingType\x12\x14\n\x07\x61\x64\x64ress\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\x04port\x18\x03 \x01(\rH\x01\x88\x01\x01\x12\x13\n\x06socket\x18\x04 \x01(\tH\x02\x88\x01\x01\"P\n\x12GetinfoBindingType\x12\x10\n\x0cLOCAL_SOCKET\x10\x00\x12\x08\n\x04IPV4\x10\x01\x12\x08\n\x04IPV6\x10\x02\x12\t\n\x05TORV2\x10\x03\x12\t\n\x05TORV3\x10\x04\x42\n\n\x08_addressB\x07\n\x05_portB\t\n\x07_socket\"H\n\x10ListpeersRequest\x12\x0f\n\x02id\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05level\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x05\n\x03_idB\x08\n\x06_level\"7\n\x11ListpeersResponse\x12\"\n\x05peers\x18\x01 \x03(\x0b\x32\x13.cln.ListpeersPeers\"\x8e\x02\n\x0eListpeersPeers\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x11\n\tconnected\x18\x02 \x01(\x08\x12\x19\n\x0cnum_channels\x18\x08 \x01(\rH\x00\x88\x01\x01\x12#\n\x03log\x18\x03 \x03(\x0b\x32\x16.cln.ListpeersPeersLog\x12-\n\x08\x63hannels\x18\x04 \x03(\x0b\x32\x1b.cln.ListpeersPeersChannels\x12\x0f\n\x07netaddr\x18\x05 \x03(\t\x12\x18\n\x0bremote_addr\x18\x07 \x01(\tH\x01\x88\x01\x01\x12\x15\n\x08\x66\x65\x61tures\x18\x06 \x01(\x0cH\x02\x88\x01\x01\x42\x0f\n\r_num_channelsB\x0e\n\x0c_remote_addrB\x0b\n\t_features\"\xfd\x02\n\x11ListpeersPeersLog\x12?\n\titem_type\x18\x01 \x01(\x0e\x32,.cln.ListpeersPeersLog.ListpeersPeersLogType\x12\x18\n\x0bnum_skipped\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x11\n\x04time\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x06source\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x10\n\x03log\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x14\n\x07node_id\x18\x06 \x01(\x0cH\x04\x88\x01\x01\x12\x11\n\x04\x64\x61ta\x18\x07 \x01(\x0cH\x05\x88\x01\x01\"i\n\x15ListpeersPeersLogType\x12\x0b\n\x07SKIPPED\x10\x00\x12\n\n\x06\x42ROKEN\x10\x01\x12\x0b\n\x07UNUSUAL\x10\x02\x12\x08\n\x04INFO\x10\x03\x12\t\n\x05\x44\x45\x42UG\x10\x04\x12\t\n\x05IO_IN\x10\x05\x12\n\n\x06IO_OUT\x10\x06\x42\x0e\n\x0c_num_skippedB\x07\n\x05_timeB\t\n\x07_sourceB\x06\n\x04_logB\n\n\x08_node_idB\x07\n\x05_data\"\xd6\x17\n\x16ListpeersPeersChannels\x12\x46\n\x05state\x18\x01 \x01(\x0e\x32\x37.cln.ListpeersPeersChannels.ListpeersPeersChannelsState\x12\x19\n\x0cscratch_txid\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x12\x38\n\x07\x66\x65\x65rate\x18\x03 \x01(\x0b\x32\".cln.ListpeersPeersChannelsFeerateH\x01\x88\x01\x01\x12\x12\n\x05owner\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x1d\n\x10short_channel_id\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x17\n\nchannel_id\x18\x06 \x01(\x0cH\x04\x88\x01\x01\x12\x19\n\x0c\x66unding_txid\x18\x07 \x01(\x0cH\x05\x88\x01\x01\x12\x1b\n\x0e\x66unding_outnum\x18\x08 \x01(\rH\x06\x88\x01\x01\x12\x1c\n\x0finitial_feerate\x18\t \x01(\tH\x07\x88\x01\x01\x12\x19\n\x0clast_feerate\x18\n \x01(\tH\x08\x88\x01\x01\x12\x19\n\x0cnext_feerate\x18\x0b \x01(\tH\t\x88\x01\x01\x12\x1a\n\rnext_fee_step\x18\x0c \x01(\rH\n\x88\x01\x01\x12\x35\n\x08inflight\x18\r \x03(\x0b\x32#.cln.ListpeersPeersChannelsInflight\x12\x15\n\x08\x63lose_to\x18\x0e \x01(\x0cH\x0b\x88\x01\x01\x12\x14\n\x07private\x18\x0f \x01(\x08H\x0c\x88\x01\x01\x12 \n\x06opener\x18\x10 \x01(\x0e\x32\x10.cln.ChannelSide\x12%\n\x06\x63loser\x18\x11 \x01(\x0e\x32\x10.cln.ChannelSideH\r\x88\x01\x01\x12\x10\n\x08\x66\x65\x61tures\x18\x12 \x03(\t\x12\x38\n\x07\x66unding\x18\x13 \x01(\x0b\x32\".cln.ListpeersPeersChannelsFundingH\x0e\x88\x01\x01\x12$\n\nto_us_msat\x18\x14 \x01(\x0b\x32\x0b.cln.AmountH\x0f\x88\x01\x01\x12(\n\x0emin_to_us_msat\x18\x15 \x01(\x0b\x32\x0b.cln.AmountH\x10\x88\x01\x01\x12(\n\x0emax_to_us_msat\x18\x16 \x01(\x0b\x32\x0b.cln.AmountH\x11\x88\x01\x01\x12$\n\ntotal_msat\x18\x17 \x01(\x0b\x32\x0b.cln.AmountH\x12\x88\x01\x01\x12\'\n\rfee_base_msat\x18\x18 \x01(\x0b\x32\x0b.cln.AmountH\x13\x88\x01\x01\x12(\n\x1b\x66\x65\x65_proportional_millionths\x18\x19 \x01(\rH\x14\x88\x01\x01\x12)\n\x0f\x64ust_limit_msat\x18\x1a \x01(\x0b\x32\x0b.cln.AmountH\x15\x88\x01\x01\x12\x30\n\x16max_total_htlc_in_msat\x18\x1b \x01(\x0b\x32\x0b.cln.AmountH\x16\x88\x01\x01\x12,\n\x12their_reserve_msat\x18\x1c \x01(\x0b\x32\x0b.cln.AmountH\x17\x88\x01\x01\x12*\n\x10our_reserve_msat\x18\x1d \x01(\x0b\x32\x0b.cln.AmountH\x18\x88\x01\x01\x12(\n\x0espendable_msat\x18\x1e \x01(\x0b\x32\x0b.cln.AmountH\x19\x88\x01\x01\x12)\n\x0freceivable_msat\x18\x1f \x01(\x0b\x32\x0b.cln.AmountH\x1a\x88\x01\x01\x12.\n\x14minimum_htlc_in_msat\x18  \x01(\x0b\x32\x0b.cln.AmountH\x1b\x88\x01\x01\x12/\n\x15minimum_htlc_out_msat\x18\x30 \x01(\x0b\x32\x0b.cln.AmountH\x1c\x88\x01\x01\x12/\n\x15maximum_htlc_out_msat\x18\x31 \x01(\x0b\x32\x0b.cln.AmountH\x1d\x88\x01\x01\x12 \n\x13their_to_self_delay\x18! \x01(\rH\x1e\x88\x01\x01\x12\x1e\n\x11our_to_self_delay\x18\" \x01(\rH\x1f\x88\x01\x01\x12\x1f\n\x12max_accepted_htlcs\x18# \x01(\rH \x88\x01\x01\x12\x34\n\x05\x61lias\x18\x32 \x01(\x0b\x32 .cln.ListpeersPeersChannelsAliasH!\x88\x01\x01\x12\x0e\n\x06status\x18% \x03(\t\x12 \n\x13in_payments_offered\x18& \x01(\x04H\"\x88\x01\x01\x12)\n\x0fin_offered_msat\x18\' \x01(\x0b\x32\x0b.cln.AmountH#\x88\x01\x01\x12\"\n\x15in_payments_fulfilled\x18( \x01(\x04H$\x88\x01\x01\x12+\n\x11in_fulfilled_msat\x18) \x01(\x0b\x32\x0b.cln.AmountH%\x88\x01\x01\x12!\n\x14out_payments_offered\x18* \x01(\x04H&\x88\x01\x01\x12*\n\x10out_offered_msat\x18+ \x01(\x0b\x32\x0b.cln.AmountH\'\x88\x01\x01\x12#\n\x16out_payments_fulfilled\x18, \x01(\x04H(\x88\x01\x01\x12,\n\x12out_fulfilled_msat\x18- \x01(\x0b\x32\x0b.cln.AmountH)\x88\x01\x01\x12/\n\x05htlcs\x18. \x03(\x0b\x32 .cln.ListpeersPeersChannelsHtlcs\x12\x1a\n\rclose_to_addr\x18/ \x01(\tH*\x88\x01\x01\"\xa1\x02\n\x1bListpeersPeersChannelsState\x12\x0c\n\x08OPENINGD\x10\x00\x12\x1c\n\x18\x43HANNELD_AWAITING_LOCKIN\x10\x01\x12\x13\n\x0f\x43HANNELD_NORMAL\x10\x02\x12\x1a\n\x16\x43HANNELD_SHUTTING_DOWN\x10\x03\x12\x18\n\x14\x43LOSINGD_SIGEXCHANGE\x10\x04\x12\x15\n\x11\x43LOSINGD_COMPLETE\x10\x05\x12\x17\n\x13\x41WAITING_UNILATERAL\x10\x06\x12\x16\n\x12\x46UNDING_SPEND_SEEN\x10\x07\x12\x0b\n\x07ONCHAIN\x10\x08\x12\x17\n\x13\x44UALOPEND_OPEN_INIT\x10\t\x12\x1d\n\x19\x44UALOPEND_AWAITING_LOCKIN\x10\nB\x0f\n\r_scratch_txidB\n\n\x08_feerateB\x08\n\x06_ownerB\x13\n\x11_short_channel_idB\r\n\x0b_channel_idB\x0f\n\r_funding_txidB\x11\n\x0f_funding_outnumB\x12\n\x10_initial_feerateB\x0f\n\r_last_feerateB\x0f\n\r_next_feerateB\x10\n\x0e_next_fee_stepB\x0b\n\t_close_toB\n\n\x08_privateB\t\n\x07_closerB\n\n\x08_fundingB\r\n\x0b_to_us_msatB\x11\n\x0f_min_to_us_msatB\x11\n\x0f_max_to_us_msatB\r\n\x0b_total_msatB\x10\n\x0e_fee_base_msatB\x1e\n\x1c_fee_proportional_millionthsB\x12\n\x10_dust_limit_msatB\x19\n\x17_max_total_htlc_in_msatB\x15\n\x13_their_reserve_msatB\x13\n\x11_our_reserve_msatB\x11\n\x0f_spendable_msatB\x12\n\x10_receivable_msatB\x17\n\x15_minimum_htlc_in_msatB\x18\n\x16_minimum_htlc_out_msatB\x18\n\x16_maximum_htlc_out_msatB\x16\n\x14_their_to_self_delayB\x14\n\x12_our_to_self_delayB\x15\n\x13_max_accepted_htlcsB\x08\n\x06_aliasB\x16\n\x14_in_payments_offeredB\x12\n\x10_in_offered_msatB\x18\n\x16_in_payments_fulfilledB\x14\n\x12_in_fulfilled_msatB\x17\n\x15_out_payments_offeredB\x13\n\x11_out_offered_msatB\x19\n\x17_out_payments_fulfilledB\x15\n\x13_out_fulfilled_msatB\x10\n\x0e_close_to_addr\"=\n\x1dListpeersPeersChannelsFeerate\x12\r\n\x05perkw\x18\x01 \x01(\r\x12\r\n\x05perkb\x18\x02 \x01(\r\"\xc5\x01\n\x1eListpeersPeersChannelsInflight\x12\x14\n\x0c\x66unding_txid\x18\x01 \x01(\x0c\x12\x16\n\x0e\x66unding_outnum\x18\x02 \x01(\r\x12\x0f\n\x07\x66\x65\x65rate\x18\x03 \x01(\t\x12\'\n\x12total_funding_msat\x18\x04 \x01(\x0b\x32\x0b.cln.Amount\x12%\n\x10our_funding_msat\x18\x05 \x01(\x0b\x32\x0b.cln.Amount\x12\x14\n\x0cscratch_txid\x18\x06 \x01(\x0c\"\x9b\x02\n\x1dListpeersPeersChannelsFunding\x12%\n\x0bpushed_msat\x18\x03 \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12%\n\x10local_funds_msat\x18\x04 \x01(\x0b\x32\x0b.cln.Amount\x12&\n\x11remote_funds_msat\x18\x07 \x01(\x0b\x32\x0b.cln.Amount\x12\'\n\rfee_paid_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12\'\n\rfee_rcvd_msat\x18\x06 \x01(\x0b\x32\x0b.cln.AmountH\x02\x88\x01\x01\x42\x0e\n\x0c_pushed_msatB\x10\n\x0e_fee_paid_msatB\x10\n\x0e_fee_rcvd_msat\"[\n\x1bListpeersPeersChannelsAlias\x12\x12\n\x05local\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06remote\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x08\n\x06_localB\t\n\x07_remote\"\xf1\x02\n\x1bListpeersPeersChannelsHtlcs\x12X\n\tdirection\x18\x01 \x01(\x0e\x32\x45.cln.ListpeersPeersChannelsHtlcs.ListpeersPeersChannelsHtlcsDirection\x12\n\n\x02id\x18\x02 \x01(\x04\x12 \n\x0b\x61mount_msat\x18\x03 \x01(\x0b\x32\x0b.cln.Amount\x12\x0e\n\x06\x65xpiry\x18\x04 \x01(\r\x12\x14\n\x0cpayment_hash\x18\x05 \x01(\x0c\x12\x1a\n\rlocal_trimmed\x18\x06 \x01(\x08H\x00\x88\x01\x01\x12\x13\n\x06status\x18\x07 \x01(\tH\x01\x88\x01\x01\x12\x1d\n\x05state\x18\x08 \x01(\x0e\x32\x0e.cln.HtlcState\"7\n$ListpeersPeersChannelsHtlcsDirection\x12\x06\n\x02IN\x10\x00\x12\x07\n\x03OUT\x10\x01\x42\x10\n\x0e_local_trimmedB\t\n\x07_status\"0\n\x10ListfundsRequest\x12\x12\n\x05spent\x18\x01 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_spent\"e\n\x11ListfundsResponse\x12&\n\x07outputs\x18\x01 \x03(\x0b\x32\x15.cln.ListfundsOutputs\x12(\n\x08\x63hannels\x18\x02 \x03(\x0b\x32\x16.cln.ListfundsChannels\"\x83\x03\n\x10ListfundsOutputs\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\x12\x0e\n\x06output\x18\x02 \x01(\r\x12 \n\x0b\x61mount_msat\x18\x03 \x01(\x0b\x32\x0b.cln.Amount\x12\x14\n\x0cscriptpubkey\x18\x04 \x01(\x0c\x12\x14\n\x07\x61\x64\x64ress\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x19\n\x0credeemscript\x18\x06 \x01(\x0cH\x01\x88\x01\x01\x12<\n\x06status\x18\x07 \x01(\x0e\x32,.cln.ListfundsOutputs.ListfundsOutputsStatus\x12\x10\n\x08reserved\x18\t \x01(\x08\x12\x18\n\x0b\x62lockheight\x18\x08 \x01(\rH\x02\x88\x01\x01\"Q\n\x16ListfundsOutputsStatus\x12\x0f\n\x0bUNCONFIRMED\x10\x00\x12\r\n\tCONFIRMED\x10\x01\x12\t\n\x05SPENT\x10\x02\x12\x0c\n\x08IMMATURE\x10\x03\x42\n\n\x08_addressB\x0f\n\r_redeemscriptB\x0e\n\x0c_blockheight\"\xab\x02\n\x11ListfundsChannels\x12\x0f\n\x07peer_id\x18\x01 \x01(\x0c\x12$\n\x0four_amount_msat\x18\x02 \x01(\x0b\x32\x0b.cln.Amount\x12 \n\x0b\x61mount_msat\x18\x03 \x01(\x0b\x32\x0b.cln.Amount\x12\x14\n\x0c\x66unding_txid\x18\x04 \x01(\x0c\x12\x16\n\x0e\x66unding_output\x18\x05 \x01(\r\x12\x11\n\tconnected\x18\x06 \x01(\x08\x12 \n\x05state\x18\x07 \x01(\x0e\x32\x11.cln.ChannelState\x12\x17\n\nchannel_id\x18\t \x01(\x0cH\x00\x88\x01\x01\x12\x1d\n\x10short_channel_id\x18\x08 \x01(\tH\x01\x88\x01\x01\x42\r\n\x0b_channel_idB\x13\n\x11_short_channel_id\"\xdd\x02\n\x0eSendpayRequest\x12 \n\x05route\x18\x01 \x03(\x0b\x32\x11.cln.SendpayRoute\x12\x14\n\x0cpayment_hash\x18\x02 \x01(\x0c\x12\x12\n\x05label\x18\x03 \x01(\tH\x00\x88\x01\x01\x12%\n\x0b\x61mount_msat\x18\n \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x05 \x01(\tH\x02\x88\x01\x01\x12\x1b\n\x0epayment_secret\x18\x06 \x01(\x0cH\x03\x88\x01\x01\x12\x13\n\x06partid\x18\x07 \x01(\rH\x04\x88\x01\x01\x12\x1a\n\rlocalinvreqid\x18\x0b \x01(\x0cH\x05\x88\x01\x01\x12\x14\n\x07groupid\x18\t \x01(\x04H\x06\x88\x01\x01\x42\x08\n\x06_labelB\x0e\n\x0c_amount_msatB\t\n\x07_bolt11B\x11\n\x0f_payment_secretB\t\n\x07_partidB\x10\n\x0e_localinvreqidB\n\n\x08_groupid\"\xd1\x04\n\x0fSendpayResponse\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x14\n\x07groupid\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12\x32\n\x06status\x18\x04 \x01(\x0e\x32\".cln.SendpayResponse.SendpayStatus\x12%\n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\x06 \x01(\x0cH\x02\x88\x01\x01\x12\x12\n\ncreated_at\x18\x07 \x01(\x04\x12\x19\n\x0c\x63ompleted_at\x18\x0f \x01(\x04H\x03\x88\x01\x01\x12%\n\x10\x61mount_sent_msat\x18\x08 \x01(\x0b\x32\x0b.cln.Amount\x12\x12\n\x05label\x18\t \x01(\tH\x04\x88\x01\x01\x12\x13\n\x06partid\x18\n \x01(\x04H\x05\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x0b \x01(\tH\x06\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\r \x01(\x0cH\x08\x88\x01\x01\x12\x14\n\x07message\x18\x0e \x01(\tH\t\x88\x01\x01\"*\n\rSendpayStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x43OMPLETE\x10\x01\x42\n\n\x08_groupidB\x0e\n\x0c_amount_msatB\x0e\n\x0c_destinationB\x0f\n\r_completed_atB\x08\n\x06_labelB\t\n\x07_partidB\t\n\x07_bolt11B\t\n\x07_bolt12B\x13\n\x11_payment_preimageB\n\n\x08_message\"\\\n\x0cSendpayRoute\x12 \n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.Amount\x12\n\n\x02id\x18\x02 \x01(\x0c\x12\r\n\x05\x64\x65lay\x18\x03 \x01(\r\x12\x0f\n\x07\x63hannel\x18\x04 \x01(\t\"\x93\x01\n\x13ListchannelsRequest\x12\x1d\n\x10short_channel_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06source\x18\x02 \x01(\x0cH\x01\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\x03 \x01(\x0cH\x02\x88\x01\x01\x42\x13\n\x11_short_channel_idB\t\n\x07_sourceB\x0e\n\x0c_destination\"C\n\x14ListchannelsResponse\x12+\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x19.cln.ListchannelsChannels\"\xb3\x03\n\x14ListchannelsChannels\x12\x0e\n\x06source\x18\x01 \x01(\x0c\x12\x13\n\x0b\x64\x65stination\x18\x02 \x01(\x0c\x12\x18\n\x10short_channel_id\x18\x03 \x01(\t\x12\x11\n\tdirection\x18\x10 \x01(\r\x12\x0e\n\x06public\x18\x04 \x01(\x08\x12 \n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.Amount\x12\x15\n\rmessage_flags\x18\x06 \x01(\r\x12\x15\n\rchannel_flags\x18\x07 \x01(\r\x12\x0e\n\x06\x61\x63tive\x18\x08 \x01(\x08\x12\x13\n\x0blast_update\x18\t \x01(\r\x12\x1d\n\x15\x62\x61se_fee_millisatoshi\x18\n \x01(\r\x12\x19\n\x11\x66\x65\x65_per_millionth\x18\x0b \x01(\r\x12\r\n\x05\x64\x65lay\x18\x0c \x01(\r\x12&\n\x11htlc_minimum_msat\x18\r \x01(\x0b\x32\x0b.cln.Amount\x12+\n\x11htlc_maximum_msat\x18\x0e \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x10\n\x08\x66\x65\x61tures\x18\x0f \x01(\x0c\x42\x14\n\x12_htlc_maximum_msat\"#\n\x10\x41\x64\x64gossipRequest\x12\x0f\n\x07message\x18\x01 \x01(\x0c\"\x13\n\x11\x41\x64\x64gossipResponse\"o\n\x17\x41utocleaninvoiceRequest\x12\x17\n\nexpired_by\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x1a\n\rcycle_seconds\x18\x02 \x01(\x04H\x01\x88\x01\x01\x42\r\n\x0b_expired_byB\x10\n\x0e_cycle_seconds\"\x81\x01\n\x18\x41utocleaninvoiceResponse\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\nexpired_by\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x1a\n\rcycle_seconds\x18\x03 \x01(\x04H\x01\x88\x01\x01\x42\r\n\x0b_expired_byB\x10\n\x0e_cycle_seconds\"U\n\x13\x43heckmessageRequest\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\r\n\x05zbase\x18\x02 \x01(\t\x12\x13\n\x06pubkey\x18\x03 \x01(\x0cH\x00\x88\x01\x01\x42\t\n\x07_pubkey\"8\n\x14\x43heckmessageResponse\x12\x10\n\x08verified\x18\x01 \x01(\x08\x12\x0e\n\x06pubkey\x18\x02 \x01(\x0c\"\xcb\x02\n\x0c\x43loseRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1e\n\x11unilateraltimeout\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\x03 \x01(\tH\x01\x88\x01\x01\x12!\n\x14\x66\x65\x65_negotiation_step\x18\x04 \x01(\tH\x02\x88\x01\x01\x12)\n\rwrong_funding\x18\x05 \x01(\x0b\x32\r.cln.OutpointH\x03\x88\x01\x01\x12\x1f\n\x12\x66orce_lease_closed\x18\x06 \x01(\x08H\x04\x88\x01\x01\x12\x1e\n\x08\x66\x65\x65range\x18\x07 \x03(\x0b\x32\x0c.cln.FeerateB\x14\n\x12_unilateraltimeoutB\x0e\n\x0c_destinationB\x17\n\x15_fee_negotiation_stepB\x10\n\x0e_wrong_fundingB\x15\n\x13_force_lease_closed\"\xab\x01\n\rCloseResponse\x12/\n\titem_type\x18\x01 \x01(\x0e\x32\x1c.cln.CloseResponse.CloseType\x12\x0f\n\x02tx\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x12\x11\n\x04txid\x18\x03 \x01(\x0cH\x01\x88\x01\x01\"5\n\tCloseType\x12\n\n\x06MUTUAL\x10\x00\x12\x0e\n\nUNILATERAL\x10\x01\x12\x0c\n\x08UNOPENED\x10\x02\x42\x05\n\x03_txB\x07\n\x05_txid\"T\n\x0e\x43onnectRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\x04host\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\x04port\x18\x03 \x01(\rH\x01\x88\x01\x01\x42\x07\n\x05_hostB\x07\n\x05_port\"\xb4\x01\n\x0f\x43onnectResponse\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x10\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0c\x12\x38\n\tdirection\x18\x03 \x01(\x0e\x32%.cln.ConnectResponse.ConnectDirection\x12$\n\x07\x61\x64\x64ress\x18\x04 \x01(\x0b\x32\x13.cln.ConnectAddress\"#\n\x10\x43onnectDirection\x12\x06\n\x02IN\x10\x00\x12\x07\n\x03OUT\x10\x01\"\xfb\x01\n\x0e\x43onnectAddress\x12\x39\n\titem_type\x18\x01 \x01(\x0e\x32&.cln.ConnectAddress.ConnectAddressType\x12\x13\n\x06socket\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x07\x61\x64\x64ress\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04port\x18\x04 \x01(\rH\x02\x88\x01\x01\"P\n\x12\x43onnectAddressType\x12\x10\n\x0cLOCAL_SOCKET\x10\x00\x12\x08\n\x04IPV4\x10\x01\x12\x08\n\x04IPV6\x10\x02\x12\t\n\x05TORV2\x10\x03\x12\t\n\x05TORV3\x10\x04\x42\t\n\x07_socketB\n\n\x08_addressB\x07\n\x05_port\"J\n\x14\x43reateinvoiceRequest\x12\x11\n\tinvstring\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x10\n\x08preimage\x18\x03 \x01(\x0c\"\x81\x05\n\x15\x43reateinvoiceResponse\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x06\x62olt11\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x04 \x01(\x0c\x12%\n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x02\x88\x01\x01\x12>\n\x06status\x18\x06 \x01(\x0e\x32..cln.CreateinvoiceResponse.CreateinvoiceStatus\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x12\n\nexpires_at\x18\x08 \x01(\x04\x12\x16\n\tpay_index\x18\t \x01(\x04H\x03\x88\x01\x01\x12.\n\x14\x61mount_received_msat\x18\n \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x12\x14\n\x07paid_at\x18\x0b \x01(\x04H\x05\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\x0c \x01(\x0cH\x06\x88\x01\x01\x12\x1b\n\x0elocal_offer_id\x18\r \x01(\x0cH\x07\x88\x01\x01\x12\x1e\n\x11invreq_payer_note\x18\x0f \x01(\tH\x08\x88\x01\x01\"8\n\x13\x43reateinvoiceStatus\x12\x08\n\x04PAID\x10\x00\x12\x0b\n\x07\x45XPIRED\x10\x01\x12\n\n\x06UNPAID\x10\x02\x42\t\n\x07_bolt11B\t\n\x07_bolt12B\x0e\n\x0c_amount_msatB\x0c\n\n_pay_indexB\x17\n\x15_amount_received_msatB\n\n\x08_paid_atB\x13\n\x11_payment_preimageB\x11\n\x0f_local_offer_idB\x14\n\x12_invreq_payer_note\"\xb4\x02\n\x10\x44\x61tastoreRequest\x12\x0b\n\x03key\x18\x05 \x03(\t\x12\x13\n\x06string\x18\x06 \x01(\tH\x00\x88\x01\x01\x12\x10\n\x03hex\x18\x02 \x01(\x0cH\x01\x88\x01\x01\x12\x36\n\x04mode\x18\x03 \x01(\x0e\x32#.cln.DatastoreRequest.DatastoreModeH\x02\x88\x01\x01\x12\x17\n\ngeneration\x18\x04 \x01(\x04H\x03\x88\x01\x01\"p\n\rDatastoreMode\x12\x0f\n\x0bMUST_CREATE\x10\x00\x12\x10\n\x0cMUST_REPLACE\x10\x01\x12\x15\n\x11\x43REATE_OR_REPLACE\x10\x02\x12\x0f\n\x0bMUST_APPEND\x10\x03\x12\x14\n\x10\x43REATE_OR_APPEND\x10\x04\x42\t\n\x07_stringB\x06\n\x04_hexB\x07\n\x05_modeB\r\n\x0b_generation\"\x82\x01\n\x11\x44\x61tastoreResponse\x12\x0b\n\x03key\x18\x05 \x03(\t\x12\x17\n\ngeneration\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x10\n\x03hex\x18\x03 \x01(\x0cH\x01\x88\x01\x01\x12\x13\n\x06string\x18\x04 \x01(\tH\x02\x88\x01\x01\x42\r\n\x0b_generationB\x06\n\x04_hexB\t\n\x07_string\"\x9d\x01\n\x12\x43reateonionRequest\x12\"\n\x04hops\x18\x01 \x03(\x0b\x32\x14.cln.CreateonionHops\x12\x11\n\tassocdata\x18\x02 \x01(\x0c\x12\x18\n\x0bsession_key\x18\x03 \x01(\x0cH\x00\x88\x01\x01\x12\x17\n\nonion_size\x18\x04 \x01(\rH\x01\x88\x01\x01\x42\x0e\n\x0c_session_keyB\r\n\x0b_onion_size\"<\n\x13\x43reateonionResponse\x12\r\n\x05onion\x18\x01 \x01(\x0c\x12\x16\n\x0eshared_secrets\x18\x02 \x03(\x0c\"2\n\x0f\x43reateonionHops\x12\x0e\n\x06pubkey\x18\x01 \x01(\x0c\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\"J\n\x13\x44\x65ldatastoreRequest\x12\x0b\n\x03key\x18\x03 \x03(\t\x12\x17\n\ngeneration\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\r\n\x0b_generation\"\x85\x01\n\x14\x44\x65ldatastoreResponse\x12\x0b\n\x03key\x18\x05 \x03(\t\x12\x17\n\ngeneration\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x10\n\x03hex\x18\x03 \x01(\x0cH\x01\x88\x01\x01\x12\x13\n\x06string\x18\x04 \x01(\tH\x02\x88\x01\x01\x42\r\n\x0b_generationB\x06\n\x04_hexB\t\n\x07_string\"H\n\x18\x44\x65lexpiredinvoiceRequest\x12\x1a\n\rmaxexpirytime\x18\x01 \x01(\x04H\x00\x88\x01\x01\x42\x10\n\x0e_maxexpirytime\"\x1b\n\x19\x44\x65lexpiredinvoiceResponse\"\xb6\x01\n\x11\x44\x65linvoiceRequest\x12\r\n\x05label\x18\x01 \x01(\t\x12\x37\n\x06status\x18\x02 \x01(\x0e\x32\'.cln.DelinvoiceRequest.DelinvoiceStatus\x12\x15\n\x08\x64\x65sconly\x18\x03 \x01(\x08H\x00\x88\x01\x01\"5\n\x10\x44\x65linvoiceStatus\x12\x08\n\x04PAID\x10\x00\x12\x0b\n\x07\x45XPIRED\x10\x01\x12\n\n\x06UNPAID\x10\x02\x42\x0b\n\t_desconly\"\xc5\x03\n\x12\x44\x65linvoiceResponse\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x06\x62olt11\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x03 \x01(\tH\x01\x88\x01\x01\x12%\n\x0b\x61mount_msat\x18\x04 \x01(\x0b\x32\x0b.cln.AmountH\x02\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x06 \x01(\x0c\x12\x38\n\x06status\x18\x07 \x01(\x0e\x32(.cln.DelinvoiceResponse.DelinvoiceStatus\x12\x12\n\nexpires_at\x18\x08 \x01(\x04\x12\x1b\n\x0elocal_offer_id\x18\t \x01(\x0cH\x04\x88\x01\x01\x12\x1e\n\x11invreq_payer_note\x18\x0b \x01(\tH\x05\x88\x01\x01\"5\n\x10\x44\x65linvoiceStatus\x12\x08\n\x04PAID\x10\x00\x12\x0b\n\x07\x45XPIRED\x10\x01\x12\n\n\x06UNPAID\x10\x02\x42\t\n\x07_bolt11B\t\n\x07_bolt12B\x0e\n\x0c_amount_msatB\x0e\n\x0c_descriptionB\x11\n\x0f_local_offer_idB\x14\n\x12_invreq_payer_note\"\xfa\x01\n\x0eInvoiceRequest\x12%\n\x0b\x61mount_msat\x18\n \x01(\x0b\x32\x10.cln.AmountOrAny\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05label\x18\x03 \x01(\t\x12\x13\n\x06\x65xpiry\x18\x07 \x01(\x04H\x00\x88\x01\x01\x12\x11\n\tfallbacks\x18\x04 \x03(\t\x12\x15\n\x08preimage\x18\x05 \x01(\x0cH\x01\x88\x01\x01\x12\x11\n\x04\x63ltv\x18\x06 \x01(\rH\x02\x88\x01\x01\x12\x19\n\x0c\x64\x65schashonly\x18\t \x01(\x08H\x03\x88\x01\x01\x42\t\n\x07_expiryB\x0b\n\t_preimageB\x07\n\x05_cltvB\x0f\n\r_deschashonly\"\xe7\x02\n\x0fInvoiceResponse\x12\x0e\n\x06\x62olt11\x18\x01 \x01(\t\x12\x14\n\x0cpayment_hash\x18\x02 \x01(\x0c\x12\x16\n\x0epayment_secret\x18\x03 \x01(\x0c\x12\x12\n\nexpires_at\x18\x04 \x01(\x04\x12\x1d\n\x10warning_capacity\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x1c\n\x0fwarning_offline\x18\x06 \x01(\tH\x01\x88\x01\x01\x12\x1d\n\x10warning_deadends\x18\x07 \x01(\tH\x02\x88\x01\x01\x12#\n\x16warning_private_unused\x18\x08 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0bwarning_mpp\x18\t \x01(\tH\x04\x88\x01\x01\x42\x13\n\x11_warning_capacityB\x12\n\x10_warning_offlineB\x13\n\x11_warning_deadendsB\x19\n\x17_warning_private_unusedB\x0e\n\x0c_warning_mpp\"#\n\x14ListdatastoreRequest\x12\x0b\n\x03key\x18\x02 \x03(\t\"G\n\x15ListdatastoreResponse\x12.\n\tdatastore\x18\x01 \x03(\x0b\x32\x1b.cln.ListdatastoreDatastore\"\x87\x01\n\x16ListdatastoreDatastore\x12\x0b\n\x03key\x18\x01 \x03(\t\x12\x17\n\ngeneration\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x10\n\x03hex\x18\x03 \x01(\x0cH\x01\x88\x01\x01\x12\x13\n\x06string\x18\x04 \x01(\tH\x02\x88\x01\x01\x42\r\n\x0b_generationB\x06\n\x04_hexB\t\n\x07_string\"\xa9\x01\n\x13ListinvoicesRequest\x12\x12\n\x05label\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x16\n\tinvstring\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x19\n\x0cpayment_hash\x18\x03 \x01(\x0cH\x02\x88\x01\x01\x12\x15\n\x08offer_id\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\x08\n\x06_labelB\x0c\n\n_invstringB\x0f\n\r_payment_hashB\x0b\n\t_offer_id\"C\n\x14ListinvoicesResponse\x12+\n\x08invoices\x18\x01 \x03(\x0b\x32\x19.cln.ListinvoicesInvoices\"\xa2\x05\n\x14ListinvoicesInvoices\x12\r\n\x05label\x18\x01 \x01(\t\x12\x18\n\x0b\x64\x65scription\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12\x44\n\x06status\x18\x04 \x01(\x0e\x32\x34.cln.ListinvoicesInvoices.ListinvoicesInvoicesStatus\x12\x12\n\nexpires_at\x18\x05 \x01(\x04\x12%\n\x0b\x61mount_msat\x18\x06 \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x07 \x01(\tH\x02\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x08 \x01(\tH\x03\x88\x01\x01\x12\x1b\n\x0elocal_offer_id\x18\t \x01(\x0cH\x04\x88\x01\x01\x12\x1e\n\x11invreq_payer_note\x18\x0f \x01(\tH\x05\x88\x01\x01\x12\x16\n\tpay_index\x18\x0b \x01(\x04H\x06\x88\x01\x01\x12.\n\x14\x61mount_received_msat\x18\x0c \x01(\x0b\x32\x0b.cln.AmountH\x07\x88\x01\x01\x12\x14\n\x07paid_at\x18\r \x01(\x04H\x08\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\x0e \x01(\x0cH\t\x88\x01\x01\"?\n\x1aListinvoicesInvoicesStatus\x12\n\n\x06UNPAID\x10\x00\x12\x08\n\x04PAID\x10\x01\x12\x0b\n\x07\x45XPIRED\x10\x02\x42\x0e\n\x0c_descriptionB\x0e\n\x0c_amount_msatB\t\n\x07_bolt11B\t\n\x07_bolt12B\x11\n\x0f_local_offer_idB\x14\n\x12_invreq_payer_noteB\x0c\n\n_pay_indexB\x17\n\x15_amount_received_msatB\n\n\x08_paid_atB\x13\n\x11_payment_preimage\"\x8a\x03\n\x10SendonionRequest\x12\r\n\x05onion\x18\x01 \x01(\x0c\x12*\n\tfirst_hop\x18\x02 \x01(\x0b\x32\x17.cln.SendonionFirst_hop\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12\x12\n\x05label\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x16\n\x0eshared_secrets\x18\x05 \x03(\x0c\x12\x13\n\x06partid\x18\x06 \x01(\rH\x01\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x07 \x01(\tH\x02\x88\x01\x01\x12%\n\x0b\x61mount_msat\x18\x0c \x01(\x0b\x32\x0b.cln.AmountH\x03\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\t \x01(\x0cH\x04\x88\x01\x01\x12\x1a\n\rlocalinvreqid\x18\r \x01(\x0cH\x05\x88\x01\x01\x12\x14\n\x07groupid\x18\x0b \x01(\x04H\x06\x88\x01\x01\x42\x08\n\x06_labelB\t\n\x07_partidB\t\n\x07_bolt11B\x0e\n\x0c_amount_msatB\x0e\n\x0c_destinationB\x10\n\x0e_localinvreqidB\n\n\x08_groupid\"\x8b\x04\n\x11SendonionResponse\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x14\n\x0cpayment_hash\x18\x02 \x01(\x0c\x12\x36\n\x06status\x18\x03 \x01(\x0e\x32&.cln.SendonionResponse.SendonionStatus\x12%\n\x0b\x61mount_msat\x18\x04 \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\x05 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\ncreated_at\x18\x06 \x01(\x04\x12%\n\x10\x61mount_sent_msat\x18\x07 \x01(\x0b\x32\x0b.cln.Amount\x12\x12\n\x05label\x18\x08 \x01(\tH\x02\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\t \x01(\tH\x03\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\n \x01(\tH\x04\x88\x01\x01\x12\x13\n\x06partid\x18\r \x01(\x04H\x05\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\x0b \x01(\x0cH\x06\x88\x01\x01\x12\x14\n\x07message\x18\x0c \x01(\tH\x07\x88\x01\x01\",\n\x0fSendonionStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x43OMPLETE\x10\x01\x42\x0e\n\x0c_amount_msatB\x0e\n\x0c_destinationB\x08\n\x06_labelB\t\n\x07_bolt11B\t\n\x07_bolt12B\t\n\x07_partidB\x13\n\x11_payment_preimageB\n\n\x08_message\"Q\n\x12SendonionFirst_hop\x12\n\n\x02id\x18\x01 \x01(\x0c\x12 \n\x0b\x61mount_msat\x18\x02 \x01(\x0b\x32\x0b.cln.Amount\x12\r\n\x05\x64\x65lay\x18\x03 \x01(\r\"\xeb\x01\n\x13ListsendpaysRequest\x12\x13\n\x06\x62olt11\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x19\n\x0cpayment_hash\x18\x02 \x01(\x0cH\x01\x88\x01\x01\x12@\n\x06status\x18\x03 \x01(\x0e\x32+.cln.ListsendpaysRequest.ListsendpaysStatusH\x02\x88\x01\x01\";\n\x12ListsendpaysStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x43OMPLETE\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x42\t\n\x07_bolt11B\x0f\n\r_payment_hashB\t\n\x07_status\"C\n\x14ListsendpaysResponse\x12+\n\x08payments\x18\x01 \x03(\x0b\x32\x19.cln.ListsendpaysPayments\"\xf4\x04\n\x14ListsendpaysPayments\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x0f\n\x07groupid\x18\x02 \x01(\x04\x12\x13\n\x06partid\x18\x0f \x01(\x04H\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12\x44\n\x06status\x18\x04 \x01(\x0e\x32\x34.cln.ListsendpaysPayments.ListsendpaysPaymentsStatus\x12%\n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\x06 \x01(\x0cH\x02\x88\x01\x01\x12\x12\n\ncreated_at\x18\x07 \x01(\x04\x12%\n\x10\x61mount_sent_msat\x18\x08 \x01(\x0b\x32\x0b.cln.Amount\x12\x12\n\x05label\x18\t \x01(\tH\x03\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\n \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0e \x01(\tH\x05\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x0b \x01(\tH\x06\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\x0c \x01(\x0cH\x07\x88\x01\x01\x12\x17\n\nerroronion\x18\r \x01(\x0cH\x08\x88\x01\x01\"C\n\x1aListsendpaysPaymentsStatus\x12\x0b\n\x07PENDING\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x12\x0c\n\x08\x43OMPLETE\x10\x02\x42\t\n\x07_partidB\x0e\n\x0c_amount_msatB\x0e\n\x0c_destinationB\x08\n\x06_labelB\t\n\x07_bolt11B\x0e\n\x0c_descriptionB\t\n\x07_bolt12B\x13\n\x11_payment_preimageB\r\n\x0b_erroronion\"\x19\n\x17ListtransactionsRequest\"S\n\x18ListtransactionsResponse\x12\x37\n\x0ctransactions\x18\x01 \x03(\x0b\x32!.cln.ListtransactionsTransactions\"\xf8\x01\n\x1cListtransactionsTransactions\x12\x0c\n\x04hash\x18\x01 \x01(\x0c\x12\r\n\x05rawtx\x18\x02 \x01(\x0c\x12\x13\n\x0b\x62lockheight\x18\x03 \x01(\r\x12\x0f\n\x07txindex\x18\x04 \x01(\r\x12\x10\n\x08locktime\x18\x07 \x01(\r\x12\x0f\n\x07version\x18\x08 \x01(\r\x12\x37\n\x06inputs\x18\t \x03(\x0b\x32\'.cln.ListtransactionsTransactionsInputs\x12\x39\n\x07outputs\x18\n \x03(\x0b\x32(.cln.ListtransactionsTransactionsOutputs\"\x84\x04\n\"ListtransactionsTransactionsInputs\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\x12\r\n\x05index\x18\x02 \x01(\r\x12\x10\n\x08sequence\x18\x03 \x01(\r\x12\x66\n\titem_type\x18\x04 \x01(\x0e\x32N.cln.ListtransactionsTransactionsInputs.ListtransactionsTransactionsInputsTypeH\x00\x88\x01\x01\x12\x14\n\x07\x63hannel\x18\x05 \x01(\tH\x01\x88\x01\x01\"\x96\x02\n&ListtransactionsTransactionsInputsType\x12\n\n\x06THEIRS\x10\x00\x12\x0b\n\x07\x44\x45POSIT\x10\x01\x12\x0c\n\x08WITHDRAW\x10\x02\x12\x13\n\x0f\x43HANNEL_FUNDING\x10\x03\x12\x18\n\x14\x43HANNEL_MUTUAL_CLOSE\x10\x04\x12\x1c\n\x18\x43HANNEL_UNILATERAL_CLOSE\x10\x05\x12\x11\n\rCHANNEL_SWEEP\x10\x06\x12\x18\n\x14\x43HANNEL_HTLC_SUCCESS\x10\x07\x12\x18\n\x14\x43HANNEL_HTLC_TIMEOUT\x10\x08\x12\x13\n\x0f\x43HANNEL_PENALTY\x10\t\x12\x1c\n\x18\x43HANNEL_UNILATERAL_CHEAT\x10\nB\x0c\n\n_item_typeB\n\n\x08_channel\"\xa0\x04\n#ListtransactionsTransactionsOutputs\x12\r\n\x05index\x18\x01 \x01(\r\x12 \n\x0b\x61mount_msat\x18\x06 \x01(\x0b\x32\x0b.cln.Amount\x12\x14\n\x0cscriptPubKey\x18\x03 \x01(\x0c\x12h\n\titem_type\x18\x04 \x01(\x0e\x32P.cln.ListtransactionsTransactionsOutputs.ListtransactionsTransactionsOutputsTypeH\x00\x88\x01\x01\x12\x14\n\x07\x63hannel\x18\x05 \x01(\tH\x01\x88\x01\x01\"\x97\x02\n\'ListtransactionsTransactionsOutputsType\x12\n\n\x06THEIRS\x10\x00\x12\x0b\n\x07\x44\x45POSIT\x10\x01\x12\x0c\n\x08WITHDRAW\x10\x02\x12\x13\n\x0f\x43HANNEL_FUNDING\x10\x03\x12\x18\n\x14\x43HANNEL_MUTUAL_CLOSE\x10\x04\x12\x1c\n\x18\x43HANNEL_UNILATERAL_CLOSE\x10\x05\x12\x11\n\rCHANNEL_SWEEP\x10\x06\x12\x18\n\x14\x43HANNEL_HTLC_SUCCESS\x10\x07\x12\x18\n\x14\x43HANNEL_HTLC_TIMEOUT\x10\x08\x12\x13\n\x0f\x43HANNEL_PENALTY\x10\t\x12\x1c\n\x18\x43HANNEL_UNILATERAL_CHEAT\x10\nB\x0c\n\n_item_typeB\n\n\x08_channel\"\xda\x03\n\nPayRequest\x12\x0e\n\x06\x62olt11\x18\x01 \x01(\t\x12%\n\x0b\x61mount_msat\x18\r \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x12\n\x05label\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x17\n\nriskfactor\x18\x08 \x01(\x01H\x02\x88\x01\x01\x12\x1a\n\rmaxfeepercent\x18\x04 \x01(\x01H\x03\x88\x01\x01\x12\x16\n\tretry_for\x18\x05 \x01(\rH\x04\x88\x01\x01\x12\x15\n\x08maxdelay\x18\x06 \x01(\rH\x05\x88\x01\x01\x12#\n\texemptfee\x18\x07 \x01(\x0b\x32\x0b.cln.AmountH\x06\x88\x01\x01\x12\x1a\n\rlocalinvreqid\x18\x0e \x01(\x0cH\x07\x88\x01\x01\x12\x0f\n\x07\x65xclude\x18\n \x03(\t\x12 \n\x06maxfee\x18\x0b \x01(\x0b\x32\x0b.cln.AmountH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0c \x01(\tH\t\x88\x01\x01\x42\x0e\n\x0c_amount_msatB\x08\n\x06_labelB\r\n\x0b_riskfactorB\x10\n\x0e_maxfeepercentB\x0c\n\n_retry_forB\x0b\n\t_maxdelayB\x0c\n\n_exemptfeeB\x10\n\x0e_localinvreqidB\t\n\x07_maxfeeB\x0e\n\x0c_description\"\xfb\x02\n\x0bPayResponse\x12\x18\n\x10payment_preimage\x18\x01 \x01(\x0c\x12\x18\n\x0b\x64\x65stination\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12\x12\n\ncreated_at\x18\x04 \x01(\x01\x12\r\n\x05parts\x18\x05 \x01(\r\x12 \n\x0b\x61mount_msat\x18\x06 \x01(\x0b\x32\x0b.cln.Amount\x12%\n\x10\x61mount_sent_msat\x18\x07 \x01(\x0b\x32\x0b.cln.Amount\x12\'\n\x1awarning_partial_completion\x18\x08 \x01(\tH\x01\x88\x01\x01\x12*\n\x06status\x18\t \x01(\x0e\x32\x1a.cln.PayResponse.PayStatus\"2\n\tPayStatus\x12\x0c\n\x08\x43OMPLETE\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x42\x0e\n\x0c_destinationB\x1d\n\x1b_warning_partial_completion\"*\n\x10ListnodesRequest\x12\x0f\n\x02id\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x42\x05\n\x03_id\"7\n\x11ListnodesResponse\x12\"\n\x05nodes\x18\x01 \x03(\x0b\x32\x13.cln.ListnodesNodes\"\xe1\x01\n\x0eListnodesNodes\x12\x0e\n\x06nodeid\x18\x01 \x01(\x0c\x12\x1b\n\x0elast_timestamp\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x12\n\x05\x61lias\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x12\n\x05\x63olor\x18\x04 \x01(\x0cH\x02\x88\x01\x01\x12\x15\n\x08\x66\x65\x61tures\x18\x05 \x01(\x0cH\x03\x88\x01\x01\x12/\n\taddresses\x18\x06 \x03(\x0b\x32\x1c.cln.ListnodesNodesAddressesB\x11\n\x0f_last_timestampB\x08\n\x06_aliasB\x08\n\x06_colorB\x0b\n\t_features\"\xf7\x01\n\x17ListnodesNodesAddresses\x12K\n\titem_type\x18\x01 \x01(\x0e\x32\x38.cln.ListnodesNodesAddresses.ListnodesNodesAddressesType\x12\x0c\n\x04port\x18\x02 \x01(\r\x12\x14\n\x07\x61\x64\x64ress\x18\x03 \x01(\tH\x00\x88\x01\x01\"_\n\x1bListnodesNodesAddressesType\x12\x07\n\x03\x44NS\x10\x00\x12\x08\n\x04IPV4\x10\x01\x12\x08\n\x04IPV6\x10\x02\x12\t\n\x05TORV2\x10\x03\x12\t\n\x05TORV3\x10\x04\x12\r\n\tWEBSOCKET\x10\x05\x42\n\n\x08_address\"g\n\x15WaitanyinvoiceRequest\x12\x1a\n\rlastpay_index\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x14\n\x07timeout\x18\x02 \x01(\x04H\x01\x88\x01\x01\x42\x10\n\x0e_lastpay_indexB\n\n\x08_timeout\"\x93\x04\n\x16WaitanyinvoiceResponse\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12@\n\x06status\x18\x04 \x01(\x0e\x32\x30.cln.WaitanyinvoiceResponse.WaitanyinvoiceStatus\x12\x12\n\nexpires_at\x18\x05 \x01(\x04\x12%\n\x0b\x61mount_msat\x18\x06 \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x07 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x08 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tpay_index\x18\t \x01(\x04H\x03\x88\x01\x01\x12.\n\x14\x61mount_received_msat\x18\n \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x12\x14\n\x07paid_at\x18\x0b \x01(\x04H\x05\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\x0c \x01(\x0cH\x06\x88\x01\x01\"-\n\x14WaitanyinvoiceStatus\x12\x08\n\x04PAID\x10\x00\x12\x0b\n\x07\x45XPIRED\x10\x01\x42\x0e\n\x0c_amount_msatB\t\n\x07_bolt11B\t\n\x07_bolt12B\x0c\n\n_pay_indexB\x17\n\x15_amount_received_msatB\n\n\x08_paid_atB\x13\n\x11_payment_preimage\"#\n\x12WaitinvoiceRequest\x12\r\n\x05label\x18\x01 \x01(\t\"\x87\x04\n\x13WaitinvoiceResponse\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12:\n\x06status\x18\x04 \x01(\x0e\x32*.cln.WaitinvoiceResponse.WaitinvoiceStatus\x12\x12\n\nexpires_at\x18\x05 \x01(\x04\x12%\n\x0b\x61mount_msat\x18\x06 \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x07 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x08 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tpay_index\x18\t \x01(\x04H\x03\x88\x01\x01\x12.\n\x14\x61mount_received_msat\x18\n \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x12\x14\n\x07paid_at\x18\x0b \x01(\x04H\x05\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\x0c \x01(\x0cH\x06\x88\x01\x01\"*\n\x11WaitinvoiceStatus\x12\x08\n\x04PAID\x10\x00\x12\x0b\n\x07\x45XPIRED\x10\x01\x42\x0e\n\x0c_amount_msatB\t\n\x07_bolt11B\t\n\x07_bolt12B\x0c\n\n_pay_indexB\x17\n\x15_amount_received_msatB\n\n\x08_paid_atB\x13\n\x11_payment_preimage\"\x8e\x01\n\x12WaitsendpayRequest\x12\x14\n\x0cpayment_hash\x18\x01 \x01(\x0c\x12\x14\n\x07timeout\x18\x03 \x01(\rH\x00\x88\x01\x01\x12\x13\n\x06partid\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x14\n\x07groupid\x18\x04 \x01(\x04H\x02\x88\x01\x01\x42\n\n\x08_timeoutB\t\n\x07_partidB\n\n\x08_groupid\"\xb2\x04\n\x13WaitsendpayResponse\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x14\n\x07groupid\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12:\n\x06status\x18\x04 \x01(\x0e\x32*.cln.WaitsendpayResponse.WaitsendpayStatus\x12%\n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12\x18\n\x0b\x64\x65stination\x18\x06 \x01(\x0cH\x02\x88\x01\x01\x12\x12\n\ncreated_at\x18\x07 \x01(\x04\x12\x19\n\x0c\x63ompleted_at\x18\x0e \x01(\x01H\x03\x88\x01\x01\x12%\n\x10\x61mount_sent_msat\x18\x08 \x01(\x0b\x32\x0b.cln.Amount\x12\x12\n\x05label\x18\t \x01(\tH\x04\x88\x01\x01\x12\x13\n\x06partid\x18\n \x01(\x04H\x05\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x0b \x01(\tH\x06\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x1d\n\x10payment_preimage\x18\r \x01(\x0cH\x08\x88\x01\x01\"!\n\x11WaitsendpayStatus\x12\x0c\n\x08\x43OMPLETE\x10\x00\x42\n\n\x08_groupidB\x0e\n\x0c_amount_msatB\x0e\n\x0c_destinationB\x0f\n\r_completed_atB\x08\n\x06_labelB\t\n\x07_partidB\t\n\x07_bolt11B\t\n\x07_bolt12B\x13\n\x11_payment_preimage\"\x8d\x01\n\x0eNewaddrRequest\x12@\n\x0b\x61\x64\x64resstype\x18\x01 \x01(\x0e\x32&.cln.NewaddrRequest.NewaddrAddresstypeH\x00\x88\x01\x01\")\n\x12NewaddrAddresstype\x12\n\n\x06\x42\x45\x43H32\x10\x00\x12\x07\n\x03\x41LL\x10\x02\x42\x0e\n\x0c_addresstype\"[\n\x0fNewaddrResponse\x12\x13\n\x06\x62\x65\x63h32\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0bp2sh_segwit\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\t\n\x07_bech32B\x0e\n\x0c_p2sh_segwit\"\xca\x01\n\x0fWithdrawRequest\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\t\x12&\n\x07satoshi\x18\x02 \x01(\x0b\x32\x10.cln.AmountOrAllH\x00\x88\x01\x01\x12\"\n\x07\x66\x65\x65rate\x18\x05 \x01(\x0b\x32\x0c.cln.FeerateH\x01\x88\x01\x01\x12\x14\n\x07minconf\x18\x03 \x01(\rH\x02\x88\x01\x01\x12\x1c\n\x05utxos\x18\x04 \x03(\x0b\x32\r.cln.OutpointB\n\n\x08_satoshiB\n\n\x08_feerateB\n\n\x08_minconf\":\n\x10WithdrawResponse\x12\n\n\x02tx\x18\x01 \x01(\x0c\x12\x0c\n\x04txid\x18\x02 \x01(\x0c\x12\x0c\n\x04psbt\x18\x03 \x01(\t\"\x82\x03\n\x0eKeysendRequest\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\x0c\x12 \n\x0b\x61mount_msat\x18\n \x01(\x0b\x32\x0b.cln.Amount\x12\x12\n\x05label\x18\x03 \x01(\tH\x00\x88\x01\x01\x12\x1a\n\rmaxfeepercent\x18\x04 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\tretry_for\x18\x05 \x01(\rH\x02\x88\x01\x01\x12\x15\n\x08maxdelay\x18\x06 \x01(\rH\x03\x88\x01\x01\x12#\n\texemptfee\x18\x07 \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x12+\n\nroutehints\x18\x08 \x01(\x0b\x32\x12.cln.RoutehintListH\x05\x88\x01\x01\x12&\n\textratlvs\x18\t \x01(\x0b\x32\x0e.cln.TlvStreamH\x06\x88\x01\x01\x42\x08\n\x06_labelB\x10\n\x0e_maxfeepercentB\x0c\n\n_retry_forB\x0b\n\t_maxdelayB\x0c\n\n_exemptfeeB\r\n\x0b_routehintsB\x0c\n\n_extratlvs\"\xf2\x02\n\x0fKeysendResponse\x12\x18\n\x10payment_preimage\x18\x01 \x01(\x0c\x12\x18\n\x0b\x64\x65stination\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x03 \x01(\x0c\x12\x12\n\ncreated_at\x18\x04 \x01(\x01\x12\r\n\x05parts\x18\x05 \x01(\r\x12 \n\x0b\x61mount_msat\x18\x06 \x01(\x0b\x32\x0b.cln.Amount\x12%\n\x10\x61mount_sent_msat\x18\x07 \x01(\x0b\x32\x0b.cln.Amount\x12\'\n\x1awarning_partial_completion\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x32\n\x06status\x18\t \x01(\x0e\x32\".cln.KeysendResponse.KeysendStatus\"\x1d\n\rKeysendStatus\x12\x0c\n\x08\x43OMPLETE\x10\x00\x42\x0e\n\x0c_destinationB\x1d\n\x1b_warning_partial_completion\"\xbc\x02\n\x0f\x46undpsbtRequest\x12!\n\x07satoshi\x18\x01 \x01(\x0b\x32\x10.cln.AmountOrAll\x12\x1d\n\x07\x66\x65\x65rate\x18\x02 \x01(\x0b\x32\x0c.cln.Feerate\x12\x13\n\x0bstartweight\x18\x03 \x01(\r\x12\x14\n\x07minconf\x18\x04 \x01(\rH\x00\x88\x01\x01\x12\x14\n\x07reserve\x18\x05 \x01(\rH\x01\x88\x01\x01\x12\x15\n\x08locktime\x18\x06 \x01(\rH\x02\x88\x01\x01\x12\x1f\n\x12min_witness_weight\x18\x07 \x01(\rH\x03\x88\x01\x01\x12\x1d\n\x10\x65xcess_as_change\x18\x08 \x01(\x08H\x04\x88\x01\x01\x42\n\n\x08_minconfB\n\n\x08_reserveB\x0b\n\t_locktimeB\x15\n\x13_min_witness_weightB\x13\n\x11_excess_as_change\"\xd9\x01\n\x10\x46undpsbtResponse\x12\x0c\n\x04psbt\x18\x01 \x01(\t\x12\x16\n\x0e\x66\x65\x65rate_per_kw\x18\x02 \x01(\r\x12\x1e\n\x16\x65stimated_final_weight\x18\x03 \x01(\r\x12 \n\x0b\x65xcess_msat\x18\x04 \x01(\x0b\x32\x0b.cln.Amount\x12\x1a\n\rchange_outnum\x18\x05 \x01(\rH\x00\x88\x01\x01\x12/\n\x0creservations\x18\x06 \x03(\x0b\x32\x19.cln.FundpsbtReservationsB\x10\n\x0e_change_outnum\"u\n\x14\x46undpsbtReservations\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\x12\x0c\n\x04vout\x18\x02 \x01(\r\x12\x14\n\x0cwas_reserved\x18\x03 \x01(\x08\x12\x10\n\x08reserved\x18\x04 \x01(\x08\x12\x19\n\x11reserved_to_block\x18\x05 \x01(\r\"A\n\x0fSendpsbtRequest\x12\x0c\n\x04psbt\x18\x01 \x01(\t\x12\x14\n\x07reserve\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\n\n\x08_reserve\",\n\x10SendpsbtResponse\x12\n\n\x02tx\x18\x01 \x01(\x0c\x12\x0c\n\x04txid\x18\x02 \x01(\x0c\"1\n\x0fSignpsbtRequest\x12\x0c\n\x04psbt\x18\x01 \x01(\t\x12\x10\n\x08signonly\x18\x02 \x03(\r\"\'\n\x10SignpsbtResponse\x12\x13\n\x0bsigned_psbt\x18\x01 \x01(\t\"\xdb\x02\n\x0fUtxopsbtRequest\x12\x1c\n\x07satoshi\x18\x01 \x01(\x0b\x32\x0b.cln.Amount\x12\x1d\n\x07\x66\x65\x65rate\x18\x02 \x01(\x0b\x32\x0c.cln.Feerate\x12\x13\n\x0bstartweight\x18\x03 \x01(\r\x12\x1c\n\x05utxos\x18\x04 \x03(\x0b\x32\r.cln.Outpoint\x12\x14\n\x07reserve\x18\x05 \x01(\rH\x00\x88\x01\x01\x12\x17\n\nreservedok\x18\x08 \x01(\x08H\x01\x88\x01\x01\x12\x15\n\x08locktime\x18\x06 \x01(\rH\x02\x88\x01\x01\x12\x1f\n\x12min_witness_weight\x18\x07 \x01(\rH\x03\x88\x01\x01\x12\x1d\n\x10\x65xcess_as_change\x18\t \x01(\x08H\x04\x88\x01\x01\x42\n\n\x08_reserveB\r\n\x0b_reservedokB\x0b\n\t_locktimeB\x15\n\x13_min_witness_weightB\x13\n\x11_excess_as_change\"\xd9\x01\n\x10UtxopsbtResponse\x12\x0c\n\x04psbt\x18\x01 \x01(\t\x12\x16\n\x0e\x66\x65\x65rate_per_kw\x18\x02 \x01(\r\x12\x1e\n\x16\x65stimated_final_weight\x18\x03 \x01(\r\x12 \n\x0b\x65xcess_msat\x18\x04 \x01(\x0b\x32\x0b.cln.Amount\x12\x1a\n\rchange_outnum\x18\x05 \x01(\rH\x00\x88\x01\x01\x12/\n\x0creservations\x18\x06 \x03(\x0b\x32\x19.cln.UtxopsbtReservationsB\x10\n\x0e_change_outnum\"u\n\x14UtxopsbtReservations\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\x12\x0c\n\x04vout\x18\x02 \x01(\r\x12\x14\n\x0cwas_reserved\x18\x03 \x01(\x08\x12\x10\n\x08reserved\x18\x04 \x01(\x08\x12\x19\n\x11reserved_to_block\x18\x05 \x01(\r\" \n\x10TxdiscardRequest\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\"6\n\x11TxdiscardResponse\x12\x13\n\x0bunsigned_tx\x18\x01 \x01(\x0c\x12\x0c\n\x04txid\x18\x02 \x01(\x0c\"\xa4\x01\n\x10TxprepareRequest\x12 \n\x07outputs\x18\x05 \x03(\x0b\x32\x0f.cln.OutputDesc\x12\"\n\x07\x66\x65\x65rate\x18\x02 \x01(\x0b\x32\x0c.cln.FeerateH\x00\x88\x01\x01\x12\x14\n\x07minconf\x18\x03 \x01(\rH\x01\x88\x01\x01\x12\x1c\n\x05utxos\x18\x04 \x03(\x0b\x32\r.cln.OutpointB\n\n\x08_feerateB\n\n\x08_minconf\"D\n\x11TxprepareResponse\x12\x0c\n\x04psbt\x18\x01 \x01(\t\x12\x13\n\x0bunsigned_tx\x18\x02 \x01(\x0c\x12\x0c\n\x04txid\x18\x03 \x01(\x0c\"\x1d\n\rTxsendRequest\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\"8\n\x0eTxsendResponse\x12\x0c\n\x04psbt\x18\x01 \x01(\t\x12\n\n\x02tx\x18\x02 \x01(\x0c\x12\x0c\n\x04txid\x18\x03 \x01(\x0c\"1\n\x17ListpeerchannelsRequest\x12\x0f\n\x02id\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x42\x05\n\x03_id\"K\n\x18ListpeerchannelsResponse\x12/\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x1d.cln.ListpeerchannelsChannels\"\xc7\x18\n\x18ListpeerchannelsChannels\x12\x14\n\x07peer_id\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x1b\n\x0epeer_connected\x18\x02 \x01(\x08H\x01\x88\x01\x01\x12O\n\x05state\x18\x03 \x01(\x0e\x32;.cln.ListpeerchannelsChannels.ListpeerchannelsChannelsStateH\x02\x88\x01\x01\x12\x19\n\x0cscratch_txid\x18\x04 \x01(\x0cH\x03\x88\x01\x01\x12:\n\x07\x66\x65\x65rate\x18\x06 \x01(\x0b\x32$.cln.ListpeerchannelsChannelsFeerateH\x04\x88\x01\x01\x12\x12\n\x05owner\x18\x07 \x01(\tH\x05\x88\x01\x01\x12\x1d\n\x10short_channel_id\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x17\n\nchannel_id\x18\t \x01(\x0cH\x07\x88\x01\x01\x12\x19\n\x0c\x66unding_txid\x18\n \x01(\x0cH\x08\x88\x01\x01\x12\x1b\n\x0e\x66unding_outnum\x18\x0b \x01(\rH\t\x88\x01\x01\x12\x1c\n\x0finitial_feerate\x18\x0c \x01(\tH\n\x88\x01\x01\x12\x19\n\x0clast_feerate\x18\r \x01(\tH\x0b\x88\x01\x01\x12\x19\n\x0cnext_feerate\x18\x0e \x01(\tH\x0c\x88\x01\x01\x12\x1a\n\rnext_fee_step\x18\x0f \x01(\rH\r\x88\x01\x01\x12\x37\n\x08inflight\x18\x10 \x03(\x0b\x32%.cln.ListpeerchannelsChannelsInflight\x12\x15\n\x08\x63lose_to\x18\x11 \x01(\x0cH\x0e\x88\x01\x01\x12\x14\n\x07private\x18\x12 \x01(\x08H\x0f\x88\x01\x01\x12%\n\x06opener\x18\x13 \x01(\x0e\x32\x10.cln.ChannelSideH\x10\x88\x01\x01\x12%\n\x06\x63loser\x18\x14 \x01(\x0e\x32\x10.cln.ChannelSideH\x11\x88\x01\x01\x12:\n\x07\x66unding\x18\x16 \x01(\x0b\x32$.cln.ListpeerchannelsChannelsFundingH\x12\x88\x01\x01\x12$\n\nto_us_msat\x18\x17 \x01(\x0b\x32\x0b.cln.AmountH\x13\x88\x01\x01\x12(\n\x0emin_to_us_msat\x18\x18 \x01(\x0b\x32\x0b.cln.AmountH\x14\x88\x01\x01\x12(\n\x0emax_to_us_msat\x18\x19 \x01(\x0b\x32\x0b.cln.AmountH\x15\x88\x01\x01\x12$\n\ntotal_msat\x18\x1a \x01(\x0b\x32\x0b.cln.AmountH\x16\x88\x01\x01\x12\'\n\rfee_base_msat\x18\x1b \x01(\x0b\x32\x0b.cln.AmountH\x17\x88\x01\x01\x12(\n\x1b\x66\x65\x65_proportional_millionths\x18\x1c \x01(\rH\x18\x88\x01\x01\x12)\n\x0f\x64ust_limit_msat\x18\x1d \x01(\x0b\x32\x0b.cln.AmountH\x19\x88\x01\x01\x12\x30\n\x16max_total_htlc_in_msat\x18\x1e \x01(\x0b\x32\x0b.cln.AmountH\x1a\x88\x01\x01\x12,\n\x12their_reserve_msat\x18\x1f \x01(\x0b\x32\x0b.cln.AmountH\x1b\x88\x01\x01\x12*\n\x10our_reserve_msat\x18  \x01(\x0b\x32\x0b.cln.AmountH\x1c\x88\x01\x01\x12(\n\x0espendable_msat\x18! \x01(\x0b\x32\x0b.cln.AmountH\x1d\x88\x01\x01\x12)\n\x0freceivable_msat\x18\" \x01(\x0b\x32\x0b.cln.AmountH\x1e\x88\x01\x01\x12.\n\x14minimum_htlc_in_msat\x18# \x01(\x0b\x32\x0b.cln.AmountH\x1f\x88\x01\x01\x12/\n\x15minimum_htlc_out_msat\x18$ \x01(\x0b\x32\x0b.cln.AmountH \x88\x01\x01\x12/\n\x15maximum_htlc_out_msat\x18% \x01(\x0b\x32\x0b.cln.AmountH!\x88\x01\x01\x12 \n\x13their_to_self_delay\x18& \x01(\rH\"\x88\x01\x01\x12\x1e\n\x11our_to_self_delay\x18\' \x01(\rH#\x88\x01\x01\x12\x1f\n\x12max_accepted_htlcs\x18( \x01(\rH$\x88\x01\x01\x12\x36\n\x05\x61lias\x18) \x01(\x0b\x32\".cln.ListpeerchannelsChannelsAliasH%\x88\x01\x01\x12\x0e\n\x06status\x18+ \x03(\t\x12 \n\x13in_payments_offered\x18, \x01(\x04H&\x88\x01\x01\x12)\n\x0fin_offered_msat\x18- \x01(\x0b\x32\x0b.cln.AmountH\'\x88\x01\x01\x12\"\n\x15in_payments_fulfilled\x18. \x01(\x04H(\x88\x01\x01\x12+\n\x11in_fulfilled_msat\x18/ \x01(\x0b\x32\x0b.cln.AmountH)\x88\x01\x01\x12!\n\x14out_payments_offered\x18\x30 \x01(\x04H*\x88\x01\x01\x12*\n\x10out_offered_msat\x18\x31 \x01(\x0b\x32\x0b.cln.AmountH+\x88\x01\x01\x12#\n\x16out_payments_fulfilled\x18\x32 \x01(\x04H,\x88\x01\x01\x12,\n\x12out_fulfilled_msat\x18\x33 \x01(\x0b\x32\x0b.cln.AmountH-\x88\x01\x01\x12\x31\n\x05htlcs\x18\x34 \x03(\x0b\x32\".cln.ListpeerchannelsChannelsHtlcs\x12\x1a\n\rclose_to_addr\x18\x35 \x01(\tH.\x88\x01\x01\"\xa3\x02\n\x1dListpeerchannelsChannelsState\x12\x0c\n\x08OPENINGD\x10\x00\x12\x1c\n\x18\x43HANNELD_AWAITING_LOCKIN\x10\x01\x12\x13\n\x0f\x43HANNELD_NORMAL\x10\x02\x12\x1a\n\x16\x43HANNELD_SHUTTING_DOWN\x10\x03\x12\x18\n\x14\x43LOSINGD_SIGEXCHANGE\x10\x04\x12\x15\n\x11\x43LOSINGD_COMPLETE\x10\x05\x12\x17\n\x13\x41WAITING_UNILATERAL\x10\x06\x12\x16\n\x12\x46UNDING_SPEND_SEEN\x10\x07\x12\x0b\n\x07ONCHAIN\x10\x08\x12\x17\n\x13\x44UALOPEND_OPEN_INIT\x10\t\x12\x1d\n\x19\x44UALOPEND_AWAITING_LOCKIN\x10\nB\n\n\x08_peer_idB\x11\n\x0f_peer_connectedB\x08\n\x06_stateB\x0f\n\r_scratch_txidB\n\n\x08_feerateB\x08\n\x06_ownerB\x13\n\x11_short_channel_idB\r\n\x0b_channel_idB\x0f\n\r_funding_txidB\x11\n\x0f_funding_outnumB\x12\n\x10_initial_feerateB\x0f\n\r_last_feerateB\x0f\n\r_next_feerateB\x10\n\x0e_next_fee_stepB\x0b\n\t_close_toB\n\n\x08_privateB\t\n\x07_openerB\t\n\x07_closerB\n\n\x08_fundingB\r\n\x0b_to_us_msatB\x11\n\x0f_min_to_us_msatB\x11\n\x0f_max_to_us_msatB\r\n\x0b_total_msatB\x10\n\x0e_fee_base_msatB\x1e\n\x1c_fee_proportional_millionthsB\x12\n\x10_dust_limit_msatB\x19\n\x17_max_total_htlc_in_msatB\x15\n\x13_their_reserve_msatB\x13\n\x11_our_reserve_msatB\x11\n\x0f_spendable_msatB\x12\n\x10_receivable_msatB\x17\n\x15_minimum_htlc_in_msatB\x18\n\x16_minimum_htlc_out_msatB\x18\n\x16_maximum_htlc_out_msatB\x16\n\x14_their_to_self_delayB\x14\n\x12_our_to_self_delayB\x15\n\x13_max_accepted_htlcsB\x08\n\x06_aliasB\x16\n\x14_in_payments_offeredB\x12\n\x10_in_offered_msatB\x18\n\x16_in_payments_fulfilledB\x14\n\x12_in_fulfilled_msatB\x17\n\x15_out_payments_offeredB\x13\n\x11_out_offered_msatB\x19\n\x17_out_payments_fulfilledB\x15\n\x13_out_fulfilled_msatB\x10\n\x0e_close_to_addr\"]\n\x1fListpeerchannelsChannelsFeerate\x12\x12\n\x05perkw\x18\x01 \x01(\rH\x00\x88\x01\x01\x12\x12\n\x05perkb\x18\x02 \x01(\rH\x01\x88\x01\x01\x42\x08\n\x06_perkwB\x08\n\x06_perkb\"\xd2\x02\n ListpeerchannelsChannelsInflight\x12\x19\n\x0c\x66unding_txid\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x1b\n\x0e\x66unding_outnum\x18\x02 \x01(\rH\x01\x88\x01\x01\x12\x14\n\x07\x66\x65\x65rate\x18\x03 \x01(\tH\x02\x88\x01\x01\x12,\n\x12total_funding_msat\x18\x04 \x01(\x0b\x32\x0b.cln.AmountH\x03\x88\x01\x01\x12*\n\x10our_funding_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x12\x19\n\x0cscratch_txid\x18\x06 \x01(\x0cH\x05\x88\x01\x01\x42\x0f\n\r_funding_txidB\x11\n\x0f_funding_outnumB\n\n\x08_feerateB\x15\n\x13_total_funding_msatB\x13\n\x11_our_funding_msatB\x0f\n\r_scratch_txid\"\xd2\x02\n\x1fListpeerchannelsChannelsFunding\x12%\n\x0bpushed_msat\x18\x01 \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12*\n\x10local_funds_msat\x18\x02 \x01(\x0b\x32\x0b.cln.AmountH\x01\x88\x01\x01\x12+\n\x11remote_funds_msat\x18\x03 \x01(\x0b\x32\x0b.cln.AmountH\x02\x88\x01\x01\x12\'\n\rfee_paid_msat\x18\x04 \x01(\x0b\x32\x0b.cln.AmountH\x03\x88\x01\x01\x12\'\n\rfee_rcvd_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x42\x0e\n\x0c_pushed_msatB\x13\n\x11_local_funds_msatB\x14\n\x12_remote_funds_msatB\x10\n\x0e_fee_paid_msatB\x10\n\x0e_fee_rcvd_msat\"]\n\x1dListpeerchannelsChannelsAlias\x12\x12\n\x05local\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06remote\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x08\n\x06_localB\t\n\x07_remote\"\xe2\x03\n\x1dListpeerchannelsChannelsHtlcs\x12\x61\n\tdirection\x18\x01 \x01(\x0e\x32I.cln.ListpeerchannelsChannelsHtlcs.ListpeerchannelsChannelsHtlcsDirectionH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12%\n\x0b\x61mount_msat\x18\x03 \x01(\x0b\x32\x0b.cln.AmountH\x02\x88\x01\x01\x12\x13\n\x06\x65xpiry\x18\x04 \x01(\rH\x03\x88\x01\x01\x12\x19\n\x0cpayment_hash\x18\x05 \x01(\x0cH\x04\x88\x01\x01\x12\x1a\n\rlocal_trimmed\x18\x06 \x01(\x08H\x05\x88\x01\x01\x12\x13\n\x06status\x18\x07 \x01(\tH\x06\x88\x01\x01\x12\"\n\x05state\x18\x08 \x01(\x0e\x32\x0e.cln.HtlcStateH\x07\x88\x01\x01\"9\n&ListpeerchannelsChannelsHtlcsDirection\x12\x06\n\x02IN\x10\x00\x12\x07\n\x03OUT\x10\x01\x42\x0c\n\n_directionB\x05\n\x03_idB\x0e\n\x0c_amount_msatB\t\n\x07_expiryB\x0f\n\r_payment_hashB\x10\n\x0e_local_trimmedB\t\n\x07_statusB\x08\n\x06_state\"3\n\x19ListclosedchannelsRequest\x12\x0f\n\x02id\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x42\x05\n\x03_id\"[\n\x1aListclosedchannelsResponse\x12=\n\x0e\x63losedchannels\x18\x01 \x03(\x0b\x32%.cln.ListclosedchannelsClosedchannels\"\xb2\t\n ListclosedchannelsClosedchannels\x12\x14\n\x07peer_id\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\nchannel_id\x18\x02 \x01(\x0c\x12\x1d\n\x10short_channel_id\x18\x03 \x01(\tH\x01\x88\x01\x01\x12>\n\x05\x61lias\x18\x04 \x01(\x0b\x32*.cln.ListclosedchannelsClosedchannelsAliasH\x02\x88\x01\x01\x12 \n\x06opener\x18\x05 \x01(\x0e\x32\x10.cln.ChannelSide\x12%\n\x06\x63loser\x18\x06 \x01(\x0e\x32\x10.cln.ChannelSideH\x03\x88\x01\x01\x12\x0f\n\x07private\x18\x07 \x01(\x08\x12\x1f\n\x17total_local_commitments\x18\t \x01(\x04\x12 \n\x18total_remote_commitments\x18\n \x01(\x04\x12\x18\n\x10total_htlcs_sent\x18\x0b \x01(\x04\x12\x14\n\x0c\x66unding_txid\x18\x0c \x01(\x0c\x12\x16\n\x0e\x66unding_outnum\x18\r \x01(\r\x12\x0e\n\x06leased\x18\x0e \x01(\x08\x12/\n\x15\x66unding_fee_paid_msat\x18\x0f \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x12/\n\x15\x66unding_fee_rcvd_msat\x18\x10 \x01(\x0b\x32\x0b.cln.AmountH\x05\x88\x01\x01\x12-\n\x13\x66unding_pushed_msat\x18\x11 \x01(\x0b\x32\x0b.cln.AmountH\x06\x88\x01\x01\x12\x1f\n\ntotal_msat\x18\x12 \x01(\x0b\x32\x0b.cln.Amount\x12%\n\x10\x66inal_to_us_msat\x18\x13 \x01(\x0b\x32\x0b.cln.Amount\x12#\n\x0emin_to_us_msat\x18\x14 \x01(\x0b\x32\x0b.cln.Amount\x12#\n\x0emax_to_us_msat\x18\x15 \x01(\x0b\x32\x0b.cln.Amount\x12!\n\x14last_commitment_txid\x18\x16 \x01(\x0cH\x07\x88\x01\x01\x12\x32\n\x18last_commitment_fee_msat\x18\x17 \x01(\x0b\x32\x0b.cln.AmountH\x08\x88\x01\x01\x12\x66\n\x0b\x63lose_cause\x18\x18 \x01(\x0e\x32Q.cln.ListclosedchannelsClosedchannels.ListclosedchannelsClosedchannelsClose_cause\"v\n+ListclosedchannelsClosedchannelsClose_cause\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05LOCAL\x10\x01\x12\x08\n\x04USER\x10\x02\x12\n\n\x06REMOTE\x10\x03\x12\x0c\n\x08PROTOCOL\x10\x04\x12\x0b\n\x07ONCHAIN\x10\x05\x42\n\n\x08_peer_idB\x13\n\x11_short_channel_idB\x08\n\x06_aliasB\t\n\x07_closerB\x18\n\x16_funding_fee_paid_msatB\x18\n\x16_funding_fee_rcvd_msatB\x16\n\x14_funding_pushed_msatB\x17\n\x15_last_commitment_txidB\x1b\n\x19_last_commitment_fee_msat\"e\n%ListclosedchannelsClosedchannelsAlias\x12\x12\n\x05local\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06remote\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x08\n\x06_localB\t\n\x07_remote\"L\n\x10\x44\x65\x63odepayRequest\x12\x0e\n\x06\x62olt11\x18\x01 \x01(\t\x12\x18\n\x0b\x64\x65scription\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_description\"\x8d\x04\n\x11\x44\x65\x63odepayResponse\x12\x10\n\x08\x63urrency\x18\x01 \x01(\t\x12\x12\n\ncreated_at\x18\x02 \x01(\x04\x12\x0e\n\x06\x65xpiry\x18\x03 \x01(\x04\x12\r\n\x05payee\x18\x04 \x01(\x0c\x12%\n\x0b\x61mount_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x14\n\x0cpayment_hash\x18\x06 \x01(\x0c\x12\x11\n\tsignature\x18\x07 \x01(\t\x12\x18\n\x0b\x64\x65scription\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x1d\n\x10\x64\x65scription_hash\x18\t \x01(\x0cH\x02\x88\x01\x01\x12\x1d\n\x15min_final_cltv_expiry\x18\n \x01(\r\x12\x1b\n\x0epayment_secret\x18\x0b \x01(\x0cH\x03\x88\x01\x01\x12\x15\n\x08\x66\x65\x61tures\x18\x0c \x01(\x0cH\x04\x88\x01\x01\x12\x1d\n\x10payment_metadata\x18\r \x01(\x0cH\x05\x88\x01\x01\x12*\n\tfallbacks\x18\x0e \x03(\x0b\x32\x17.cln.DecodepayFallbacks\x12\"\n\x05\x65xtra\x18\x10 \x03(\x0b\x32\x13.cln.DecodepayExtraB\x0e\n\x0c_amount_msatB\x0e\n\x0c_descriptionB\x13\n\x11_description_hashB\x11\n\x0f_payment_secretB\x0b\n\t_featuresB\x13\n\x11_payment_metadata\"\xc6\x01\n\x12\x44\x65\x63odepayFallbacks\x12\x41\n\titem_type\x18\x01 \x01(\x0e\x32..cln.DecodepayFallbacks.DecodepayFallbacksType\x12\x11\n\x04\x61\x64\x64r\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x0b\n\x03hex\x18\x03 \x01(\x0c\"D\n\x16\x44\x65\x63odepayFallbacksType\x12\t\n\x05P2PKH\x10\x00\x12\x08\n\x04P2SH\x10\x01\x12\n\n\x06P2WPKH\x10\x02\x12\t\n\x05P2WSH\x10\x03\x42\x07\n\x05_addr\"+\n\x0e\x44\x65\x63odepayExtra\x12\x0b\n\x03tag\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\"\x1f\n\rDecodeRequest\x12\x0e\n\x06string\x18\x01 \x01(\t\"\xaa!\n\x0e\x44\x65\x63odeResponse\x12\x31\n\titem_type\x18\x01 \x01(\x0e\x32\x1e.cln.DecodeResponse.DecodeType\x12\r\n\x05valid\x18\x02 \x01(\x08\x12\x15\n\x08offer_id\x18\x03 \x01(\x0cH\x00\x88\x01\x01\x12\x14\n\x0coffer_chains\x18\x04 \x03(\x0c\x12\x1b\n\x0eoffer_metadata\x18\x05 \x01(\x0cH\x01\x88\x01\x01\x12\x1b\n\x0eoffer_currency\x18\x06 \x01(\tH\x02\x88\x01\x01\x12+\n\x1ewarning_unknown_offer_currency\x18\x07 \x01(\tH\x03\x88\x01\x01\x12 \n\x13\x63urrency_minor_unit\x18\x08 \x01(\rH\x04\x88\x01\x01\x12\x19\n\x0coffer_amount\x18\t \x01(\x04H\x05\x88\x01\x01\x12+\n\x11offer_amount_msat\x18\n \x01(\x0b\x32\x0b.cln.AmountH\x06\x88\x01\x01\x12\x1e\n\x11offer_description\x18\x0b \x01(\tH\x07\x88\x01\x01\x12\x19\n\x0coffer_issuer\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x1b\n\x0eoffer_features\x18\r \x01(\x0cH\t\x88\x01\x01\x12\"\n\x15offer_absolute_expiry\x18\x0e \x01(\x04H\n\x88\x01\x01\x12\x1f\n\x12offer_quantity_max\x18\x0f \x01(\x04H\x0b\x88\x01\x01\x12+\n\x0boffer_paths\x18\x10 \x03(\x0b\x32\x16.cln.DecodeOffer_paths\x12\x1a\n\roffer_node_id\x18\x11 \x01(\x0cH\x0c\x88\x01\x01\x12*\n\x1dwarning_missing_offer_node_id\x18\x14 \x01(\tH\r\x88\x01\x01\x12.\n!warning_invalid_offer_description\x18\x15 \x01(\tH\x0e\x88\x01\x01\x12.\n!warning_missing_offer_description\x18\x16 \x01(\tH\x0f\x88\x01\x01\x12+\n\x1ewarning_invalid_offer_currency\x18\x17 \x01(\tH\x10\x88\x01\x01\x12)\n\x1cwarning_invalid_offer_issuer\x18\x18 \x01(\tH\x11\x88\x01\x01\x12\x1c\n\x0finvreq_metadata\x18\x19 \x01(\x0cH\x12\x88\x01\x01\x12\x1c\n\x0finvreq_payer_id\x18\x1a \x01(\x0cH\x13\x88\x01\x01\x12\x19\n\x0cinvreq_chain\x18\x1b \x01(\x0cH\x14\x88\x01\x01\x12,\n\x12invreq_amount_msat\x18\x1c \x01(\x0b\x32\x0b.cln.AmountH\x15\x88\x01\x01\x12\x1c\n\x0finvreq_features\x18\x1d \x01(\x0cH\x16\x88\x01\x01\x12\x1c\n\x0finvreq_quantity\x18\x1e \x01(\x04H\x17\x88\x01\x01\x12\x1e\n\x11invreq_payer_note\x18\x1f \x01(\tH\x18\x88\x01\x01\x12&\n\x19invreq_recurrence_counter\x18  \x01(\rH\x19\x88\x01\x01\x12$\n\x17invreq_recurrence_start\x18! \x01(\rH\x1a\x88\x01\x01\x12,\n\x1fwarning_missing_invreq_metadata\x18# \x01(\tH\x1b\x88\x01\x01\x12,\n\x1fwarning_missing_invreq_payer_id\x18$ \x01(\tH\x1c\x88\x01\x01\x12.\n!warning_invalid_invreq_payer_note\x18% \x01(\tH\x1d\x88\x01\x01\x12\x36\n)warning_missing_invoice_request_signature\x18& \x01(\tH\x1e\x88\x01\x01\x12\x36\n)warning_invalid_invoice_request_signature\x18\' \x01(\tH\x1f\x88\x01\x01\x12\x1f\n\x12invoice_created_at\x18) \x01(\x04H \x88\x01\x01\x12$\n\x17invoice_relative_expiry\x18* \x01(\rH!\x88\x01\x01\x12!\n\x14invoice_payment_hash\x18+ \x01(\x0cH\"\x88\x01\x01\x12-\n\x13invoice_amount_msat\x18, \x01(\x0b\x32\x0b.cln.AmountH#\x88\x01\x01\x12\x37\n\x11invoice_fallbacks\x18- \x03(\x0b\x32\x1c.cln.DecodeInvoice_fallbacks\x12\x1d\n\x10invoice_features\x18. \x01(\x0cH$\x88\x01\x01\x12\x1c\n\x0finvoice_node_id\x18/ \x01(\x0cH%\x88\x01\x01\x12(\n\x1binvoice_recurrence_basetime\x18\x30 \x01(\x04H&\x88\x01\x01\x12*\n\x1dwarning_missing_invoice_paths\x18\x32 \x01(\tH\'\x88\x01\x01\x12/\n\"warning_missing_invoice_blindedpay\x18\x33 \x01(\tH(\x88\x01\x01\x12/\n\"warning_missing_invoice_created_at\x18\x34 \x01(\tH)\x88\x01\x01\x12\x31\n$warning_missing_invoice_payment_hash\x18\x35 \x01(\tH*\x88\x01\x01\x12+\n\x1ewarning_missing_invoice_amount\x18\x36 \x01(\tH+\x88\x01\x01\x12\x38\n+warning_missing_invoice_recurrence_basetime\x18\x37 \x01(\tH,\x88\x01\x01\x12,\n\x1fwarning_missing_invoice_node_id\x18\x38 \x01(\tH-\x88\x01\x01\x12.\n!warning_missing_invoice_signature\x18\x39 \x01(\tH.\x88\x01\x01\x12.\n!warning_invalid_invoice_signature\x18: \x01(\tH/\x88\x01\x01\x12\'\n\tfallbacks\x18; \x03(\x0b\x32\x14.cln.DecodeFallbacks\x12\x17\n\ncreated_at\x18< \x01(\x04H0\x88\x01\x01\x12\x13\n\x06\x65xpiry\x18= \x01(\x04H1\x88\x01\x01\x12\x12\n\x05payee\x18> \x01(\x0cH2\x88\x01\x01\x12\x19\n\x0cpayment_hash\x18? \x01(\x0cH3\x88\x01\x01\x12\x1d\n\x10\x64\x65scription_hash\x18@ \x01(\x0cH4\x88\x01\x01\x12\"\n\x15min_final_cltv_expiry\x18\x41 \x01(\rH5\x88\x01\x01\x12\x1b\n\x0epayment_secret\x18\x42 \x01(\x0cH6\x88\x01\x01\x12\x1d\n\x10payment_metadata\x18\x43 \x01(\x0cH7\x88\x01\x01\x12\x1f\n\x05\x65xtra\x18\x45 \x03(\x0b\x32\x10.cln.DecodeExtra\x12\x16\n\tunique_id\x18\x46 \x01(\tH8\x88\x01\x01\x12\x14\n\x07version\x18G \x01(\tH9\x88\x01\x01\x12\x13\n\x06string\x18H \x01(\tH:\x88\x01\x01\x12-\n\x0crestrictions\x18I \x03(\x0b\x32\x17.cln.DecodeRestrictions\x12&\n\x19warning_rune_invalid_utf8\x18J \x01(\tH;\x88\x01\x01\x12\x10\n\x03hex\x18K \x01(\x0cH<\x88\x01\x01\"l\n\nDecodeType\x12\x10\n\x0c\x42OLT12_OFFER\x10\x00\x12\x12\n\x0e\x42OLT12_INVOICE\x10\x01\x12\x1a\n\x16\x42OLT12_INVOICE_REQUEST\x10\x02\x12\x12\n\x0e\x42OLT11_INVOICE\x10\x03\x12\x08\n\x04RUNE\x10\x04\x42\x0b\n\t_offer_idB\x11\n\x0f_offer_metadataB\x11\n\x0f_offer_currencyB!\n\x1f_warning_unknown_offer_currencyB\x16\n\x14_currency_minor_unitB\x0f\n\r_offer_amountB\x14\n\x12_offer_amount_msatB\x14\n\x12_offer_descriptionB\x0f\n\r_offer_issuerB\x11\n\x0f_offer_featuresB\x18\n\x16_offer_absolute_expiryB\x15\n\x13_offer_quantity_maxB\x10\n\x0e_offer_node_idB \n\x1e_warning_missing_offer_node_idB$\n\"_warning_invalid_offer_descriptionB$\n\"_warning_missing_offer_descriptionB!\n\x1f_warning_invalid_offer_currencyB\x1f\n\x1d_warning_invalid_offer_issuerB\x12\n\x10_invreq_metadataB\x12\n\x10_invreq_payer_idB\x0f\n\r_invreq_chainB\x15\n\x13_invreq_amount_msatB\x12\n\x10_invreq_featuresB\x12\n\x10_invreq_quantityB\x14\n\x12_invreq_payer_noteB\x1c\n\x1a_invreq_recurrence_counterB\x1a\n\x18_invreq_recurrence_startB\"\n _warning_missing_invreq_metadataB\"\n _warning_missing_invreq_payer_idB$\n\"_warning_invalid_invreq_payer_noteB,\n*_warning_missing_invoice_request_signatureB,\n*_warning_invalid_invoice_request_signatureB\x15\n\x13_invoice_created_atB\x1a\n\x18_invoice_relative_expiryB\x17\n\x15_invoice_payment_hashB\x16\n\x14_invoice_amount_msatB\x13\n\x11_invoice_featuresB\x12\n\x10_invoice_node_idB\x1e\n\x1c_invoice_recurrence_basetimeB \n\x1e_warning_missing_invoice_pathsB%\n#_warning_missing_invoice_blindedpayB%\n#_warning_missing_invoice_created_atB\'\n%_warning_missing_invoice_payment_hashB!\n\x1f_warning_missing_invoice_amountB.\n,_warning_missing_invoice_recurrence_basetimeB\"\n _warning_missing_invoice_node_idB$\n\"_warning_missing_invoice_signatureB$\n\"_warning_invalid_invoice_signatureB\r\n\x0b_created_atB\t\n\x07_expiryB\x08\n\x06_payeeB\x0f\n\r_payment_hashB\x13\n\x11_description_hashB\x18\n\x16_min_final_cltv_expiryB\x11\n\x0f_payment_secretB\x13\n\x11_payment_metadataB\x0c\n\n_unique_idB\n\n\x08_versionB\t\n\x07_stringB\x1c\n\x1a_warning_rune_invalid_utf8B\x06\n\x04_hex\"<\n\x11\x44\x65\x63odeOffer_paths\x12\x15\n\rfirst_node_id\x18\x01 \x01(\x0c\x12\x10\n\x08\x62linding\x18\x02 \x01(\x0c\"\x8a\x01\n\x1f\x44\x65\x63odeOffer_recurrencePaywindow\x12\x16\n\x0eseconds_before\x18\x01 \x01(\r\x12\x15\n\rseconds_after\x18\x02 \x01(\r\x12 \n\x13proportional_amount\x18\x03 \x01(\x08H\x00\x88\x01\x01\x42\x16\n\x14_proportional_amount\"T\n\x17\x44\x65\x63odeInvoice_pathsPath\x12\x17\n\x0f\x62linded_node_id\x18\x01 \x01(\x0c\x12 \n\x18\x65ncrypted_recipient_data\x18\x02 \x01(\x0c\"Y\n\x17\x44\x65\x63odeInvoice_fallbacks\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x0b\n\x03hex\x18\x02 \x01(\x0c\x12\x14\n\x07\x61\x64\x64ress\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\n\n\x08_address\"w\n\x0f\x44\x65\x63odeFallbacks\x12\x36\n)warning_invoice_fallbacks_version_invalid\x18\x01 \x01(\tH\x00\x88\x01\x01\x42,\n*_warning_invoice_fallbacks_version_invalid\"(\n\x0b\x44\x65\x63odeExtra\x12\x0b\n\x03tag\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\";\n\x12\x44\x65\x63odeRestrictions\x12\x14\n\x0c\x61lternatives\x18\x01 \x03(\t\x12\x0f\n\x07summary\x18\x02 \x01(\t\"=\n\x11\x44isconnectRequest\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x12\n\x05\x66orce\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_force\"\x14\n\x12\x44isconnectResponse\"k\n\x0f\x46\x65\x65ratesRequest\x12\x31\n\x05style\x18\x01 \x01(\x0e\x32\".cln.FeeratesRequest.FeeratesStyle\"%\n\rFeeratesStyle\x12\t\n\x05PERKB\x10\x00\x12\t\n\x05PERKW\x10\x01\"\x9c\x02\n\x10\x46\x65\x65ratesResponse\x12%\n\x18warning_missing_feerates\x18\x01 \x01(\tH\x00\x88\x01\x01\x12&\n\x05perkb\x18\x02 \x01(\x0b\x32\x12.cln.FeeratesPerkbH\x01\x88\x01\x01\x12&\n\x05perkw\x18\x03 \x01(\x0b\x32\x12.cln.FeeratesPerkwH\x02\x88\x01\x01\x12\x46\n\x15onchain_fee_estimates\x18\x04 \x01(\x0b\x32\".cln.FeeratesOnchain_fee_estimatesH\x03\x88\x01\x01\x42\x1b\n\x19_warning_missing_feeratesB\x08\n\x06_perkbB\x08\n\x06_perkwB\x18\n\x16_onchain_fee_estimates\"\x91\x03\n\rFeeratesPerkb\x12\x16\n\x0emin_acceptable\x18\x01 \x01(\r\x12\x16\n\x0emax_acceptable\x18\x02 \x01(\r\x12\x12\n\x05\x66loor\x18\n \x01(\rH\x00\x88\x01\x01\x12.\n\testimates\x18\t \x03(\x0b\x32\x1b.cln.FeeratesPerkbEstimates\x12\x14\n\x07opening\x18\x03 \x01(\rH\x01\x88\x01\x01\x12\x19\n\x0cmutual_close\x18\x04 \x01(\rH\x02\x88\x01\x01\x12\x1d\n\x10unilateral_close\x18\x05 \x01(\rH\x03\x88\x01\x01\x12\x1a\n\rdelayed_to_us\x18\x06 \x01(\rH\x04\x88\x01\x01\x12\x1c\n\x0fhtlc_resolution\x18\x07 \x01(\rH\x05\x88\x01\x01\x12\x14\n\x07penalty\x18\x08 \x01(\rH\x06\x88\x01\x01\x42\x08\n\x06_floorB\n\n\x08_openingB\x0f\n\r_mutual_closeB\x13\n\x11_unilateral_closeB\x10\n\x0e_delayed_to_usB\x12\n\x10_htlc_resolutionB\n\n\x08_penalty\"\x96\x01\n\x16\x46\x65\x65ratesPerkbEstimates\x12\x17\n\nblockcount\x18\x01 \x01(\rH\x00\x88\x01\x01\x12\x14\n\x07\x66\x65\x65rate\x18\x02 \x01(\rH\x01\x88\x01\x01\x12\x1d\n\x10smoothed_feerate\x18\x03 \x01(\rH\x02\x88\x01\x01\x42\r\n\x0b_blockcountB\n\n\x08_feerateB\x13\n\x11_smoothed_feerate\"\x91\x03\n\rFeeratesPerkw\x12\x16\n\x0emin_acceptable\x18\x01 \x01(\r\x12\x16\n\x0emax_acceptable\x18\x02 \x01(\r\x12\x12\n\x05\x66loor\x18\n \x01(\rH\x00\x88\x01\x01\x12.\n\testimates\x18\t \x03(\x0b\x32\x1b.cln.FeeratesPerkwEstimates\x12\x14\n\x07opening\x18\x03 \x01(\rH\x01\x88\x01\x01\x12\x19\n\x0cmutual_close\x18\x04 \x01(\rH\x02\x88\x01\x01\x12\x1d\n\x10unilateral_close\x18\x05 \x01(\rH\x03\x88\x01\x01\x12\x1a\n\rdelayed_to_us\x18\x06 \x01(\rH\x04\x88\x01\x01\x12\x1c\n\x0fhtlc_resolution\x18\x07 \x01(\rH\x05\x88\x01\x01\x12\x14\n\x07penalty\x18\x08 \x01(\rH\x06\x88\x01\x01\x42\x08\n\x06_floorB\n\n\x08_openingB\x0f\n\r_mutual_closeB\x13\n\x11_unilateral_closeB\x10\n\x0e_delayed_to_usB\x12\n\x10_htlc_resolutionB\n\n\x08_penalty\"\x96\x01\n\x16\x46\x65\x65ratesPerkwEstimates\x12\x17\n\nblockcount\x18\x01 \x01(\rH\x00\x88\x01\x01\x12\x14\n\x07\x66\x65\x65rate\x18\x02 \x01(\rH\x01\x88\x01\x01\x12\x1d\n\x10smoothed_feerate\x18\x03 \x01(\rH\x02\x88\x01\x01\x42\r\n\x0b_blockcountB\n\n\x08_feerateB\x13\n\x11_smoothed_feerate\"\xc1\x01\n\x1d\x46\x65\x65ratesOnchain_fee_estimates\x12 \n\x18opening_channel_satoshis\x18\x01 \x01(\x04\x12\x1d\n\x15mutual_close_satoshis\x18\x02 \x01(\x04\x12!\n\x19unilateral_close_satoshis\x18\x03 \x01(\x04\x12\x1d\n\x15htlc_timeout_satoshis\x18\x04 \x01(\x04\x12\x1d\n\x15htlc_success_satoshis\x18\x05 \x01(\x04\"\xe5\x03\n\x12\x46undchannelRequest\x12\n\n\x02id\x18\t \x01(\x0c\x12 \n\x06\x61mount\x18\x01 \x01(\x0b\x32\x10.cln.AmountOrAll\x12\"\n\x07\x66\x65\x65rate\x18\x02 \x01(\x0b\x32\x0c.cln.FeerateH\x00\x88\x01\x01\x12\x15\n\x08\x61nnounce\x18\x03 \x01(\x08H\x01\x88\x01\x01\x12\x14\n\x07minconf\x18\n \x01(\rH\x02\x88\x01\x01\x12#\n\tpush_msat\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x03\x88\x01\x01\x12\x15\n\x08\x63lose_to\x18\x06 \x01(\tH\x04\x88\x01\x01\x12%\n\x0brequest_amt\x18\x07 \x01(\x0b\x32\x0b.cln.AmountH\x05\x88\x01\x01\x12\x1a\n\rcompact_lease\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x1c\n\x05utxos\x18\x0b \x03(\x0b\x32\r.cln.Outpoint\x12\x15\n\x08mindepth\x18\x0c \x01(\rH\x07\x88\x01\x01\x12!\n\x07reserve\x18\r \x01(\x0b\x32\x0b.cln.AmountH\x08\x88\x01\x01\x42\n\n\x08_feerateB\x0b\n\t_announceB\n\n\x08_minconfB\x0c\n\n_push_msatB\x0b\n\t_close_toB\x0e\n\x0c_request_amtB\x10\n\x0e_compact_leaseB\x0b\n\t_mindepthB\n\n\x08_reserve\"\x9b\x01\n\x13\x46undchannelResponse\x12\n\n\x02tx\x18\x01 \x01(\x0c\x12\x0c\n\x04txid\x18\x02 \x01(\x0c\x12\x0e\n\x06outnum\x18\x03 \x01(\r\x12\x12\n\nchannel_id\x18\x04 \x01(\x0c\x12\x15\n\x08\x63lose_to\x18\x05 \x01(\x0cH\x00\x88\x01\x01\x12\x15\n\x08mindepth\x18\x06 \x01(\rH\x01\x88\x01\x01\x42\x0b\n\t_close_toB\x0b\n\t_mindepth\"\xec\x01\n\x0fGetrouteRequest\x12\n\n\x02id\x18\x01 \x01(\x0c\x12 \n\x0b\x61mount_msat\x18\t \x01(\x0b\x32\x0b.cln.Amount\x12\x12\n\nriskfactor\x18\x03 \x01(\x04\x12\x11\n\x04\x63ltv\x18\x04 \x01(\x01H\x00\x88\x01\x01\x12\x13\n\x06\x66romid\x18\x05 \x01(\x0cH\x01\x88\x01\x01\x12\x18\n\x0b\x66uzzpercent\x18\x06 \x01(\rH\x02\x88\x01\x01\x12\x0f\n\x07\x65xclude\x18\x07 \x03(\t\x12\x14\n\x07maxhops\x18\x08 \x01(\rH\x03\x88\x01\x01\x42\x07\n\x05_cltvB\t\n\x07_fromidB\x0e\n\x0c_fuzzpercentB\n\n\x08_maxhops\"5\n\x10GetrouteResponse\x12!\n\x05route\x18\x01 \x03(\x0b\x32\x12.cln.GetrouteRoute\"\xc5\x01\n\rGetrouteRoute\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\t\x12\x11\n\tdirection\x18\x03 \x01(\r\x12 \n\x0b\x61mount_msat\x18\x04 \x01(\x0b\x32\x0b.cln.Amount\x12\r\n\x05\x64\x65lay\x18\x05 \x01(\r\x12\x34\n\x05style\x18\x06 \x01(\x0e\x32%.cln.GetrouteRoute.GetrouteRouteStyle\"\x1d\n\x12GetrouteRouteStyle\x12\x07\n\x03TLV\x10\x00\"\x82\x02\n\x13ListforwardsRequest\x12@\n\x06status\x18\x01 \x01(\x0e\x32+.cln.ListforwardsRequest.ListforwardsStatusH\x00\x88\x01\x01\x12\x17\n\nin_channel\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x0bout_channel\x18\x03 \x01(\tH\x02\x88\x01\x01\"L\n\x12ListforwardsStatus\x12\x0b\n\x07OFFERED\x10\x00\x12\x0b\n\x07SETTLED\x10\x01\x12\x10\n\x0cLOCAL_FAILED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x42\t\n\x07_statusB\r\n\x0b_in_channelB\x0e\n\x0c_out_channel\"C\n\x14ListforwardsResponse\x12+\n\x08\x66orwards\x18\x01 \x03(\x0b\x32\x19.cln.ListforwardsForwards\"\xde\x04\n\x14ListforwardsForwards\x12\x12\n\nin_channel\x18\x01 \x01(\t\x12\x17\n\nin_htlc_id\x18\n \x01(\x04H\x00\x88\x01\x01\x12\x1c\n\x07in_msat\x18\x02 \x01(\x0b\x32\x0b.cln.Amount\x12\x44\n\x06status\x18\x03 \x01(\x0e\x32\x34.cln.ListforwardsForwards.ListforwardsForwardsStatus\x12\x15\n\rreceived_time\x18\x04 \x01(\x01\x12\x18\n\x0bout_channel\x18\x05 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x0bout_htlc_id\x18\x0b \x01(\x04H\x02\x88\x01\x01\x12G\n\x05style\x18\t \x01(\x0e\x32\x33.cln.ListforwardsForwards.ListforwardsForwardsStyleH\x03\x88\x01\x01\x12\"\n\x08\x66\x65\x65_msat\x18\x07 \x01(\x0b\x32\x0b.cln.AmountH\x04\x88\x01\x01\x12\"\n\x08out_msat\x18\x08 \x01(\x0b\x32\x0b.cln.AmountH\x05\x88\x01\x01\"T\n\x1aListforwardsForwardsStatus\x12\x0b\n\x07OFFERED\x10\x00\x12\x0b\n\x07SETTLED\x10\x01\x12\x10\n\x0cLOCAL_FAILED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\"0\n\x19ListforwardsForwardsStyle\x12\n\n\x06LEGACY\x10\x00\x12\x07\n\x03TLV\x10\x01\x42\r\n\x0b_in_htlc_idB\x0e\n\x0c_out_channelB\x0e\n\x0c_out_htlc_idB\x08\n\x06_styleB\x0b\n\t_fee_msatB\x0b\n\t_out_msat\"\xdb\x01\n\x0fListpaysRequest\x12\x13\n\x06\x62olt11\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x19\n\x0cpayment_hash\x18\x02 \x01(\x0cH\x01\x88\x01\x01\x12\x38\n\x06status\x18\x03 \x01(\x0e\x32#.cln.ListpaysRequest.ListpaysStatusH\x02\x88\x01\x01\"7\n\x0eListpaysStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x43OMPLETE\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x42\t\n\x07_bolt11B\x0f\n\r_payment_hashB\t\n\x07_status\"3\n\x10ListpaysResponse\x12\x1f\n\x04pays\x18\x01 \x03(\x0b\x32\x11.cln.ListpaysPays\"\x87\x04\n\x0cListpaysPays\x12\x14\n\x0cpayment_hash\x18\x01 \x01(\x0c\x12\x34\n\x06status\x18\x02 \x01(\x0e\x32$.cln.ListpaysPays.ListpaysPaysStatus\x12\x18\n\x0b\x64\x65stination\x18\x03 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\ncreated_at\x18\x04 \x01(\x04\x12\x19\n\x0c\x63ompleted_at\x18\x0c \x01(\x04H\x01\x88\x01\x01\x12\x12\n\x05label\x18\x05 \x01(\tH\x02\x88\x01\x01\x12\x13\n\x06\x62olt11\x18\x06 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0b \x01(\tH\x04\x88\x01\x01\x12\x13\n\x06\x62olt12\x18\x07 \x01(\tH\x05\x88\x01\x01\x12\x15\n\x08preimage\x18\r \x01(\x0cH\x06\x88\x01\x01\x12\x1c\n\x0fnumber_of_parts\x18\x0e \x01(\x04H\x07\x88\x01\x01\x12\x17\n\nerroronion\x18\n \x01(\x0cH\x08\x88\x01\x01\";\n\x12ListpaysPaysStatus\x12\x0b\n\x07PENDING\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x12\x0c\n\x08\x43OMPLETE\x10\x02\x42\x0e\n\x0c_destinationB\x0f\n\r_completed_atB\x08\n\x06_labelB\t\n\x07_bolt11B\x0e\n\x0c_descriptionB\t\n\x07_bolt12B\x0b\n\t_preimageB\x12\n\x10_number_of_partsB\r\n\x0b_erroronion\"Y\n\x0bPingRequest\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x10\n\x03len\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x16\n\tpongbytes\x18\x03 \x01(\rH\x01\x88\x01\x01\x42\x06\n\x04_lenB\x0c\n\n_pongbytes\"\x1e\n\x0cPingResponse\x12\x0e\n\x06totlen\x18\x01 \x01(\r\"4\n\x14SendcustommsgRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12\x0b\n\x03msg\x18\x02 \x01(\x0c\"\'\n\x15SendcustommsgResponse\x12\x0e\n\x06status\x18\x01 \x01(\t\"\xf8\x01\n\x11SetchannelRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12!\n\x07\x66\x65\x65\x62\x61se\x18\x02 \x01(\x0b\x32\x0b.cln.AmountH\x00\x88\x01\x01\x12\x13\n\x06\x66\x65\x65ppm\x18\x03 \x01(\rH\x01\x88\x01\x01\x12!\n\x07htlcmin\x18\x04 \x01(\x0b\x32\x0b.cln.AmountH\x02\x88\x01\x01\x12!\n\x07htlcmax\x18\x05 \x01(\x0b\x32\x0b.cln.AmountH\x03\x88\x01\x01\x12\x19\n\x0c\x65nforcedelay\x18\x06 \x01(\rH\x04\x88\x01\x01\x42\n\n\x08_feebaseB\t\n\x07_feeppmB\n\n\x08_htlcminB\n\n\x08_htlcmaxB\x0f\n\r_enforcedelay\"?\n\x12SetchannelResponse\x12)\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x17.cln.SetchannelChannels\"\x94\x03\n\x12SetchannelChannels\x12\x0f\n\x07peer_id\x18\x01 \x01(\x0c\x12\x12\n\nchannel_id\x18\x02 \x01(\x0c\x12\x1d\n\x10short_channel_id\x18\x03 \x01(\tH\x00\x88\x01\x01\x12\"\n\rfee_base_msat\x18\x04 \x01(\x0b\x32\x0b.cln.Amount\x12#\n\x1b\x66\x65\x65_proportional_millionths\x18\x05 \x01(\r\x12*\n\x15minimum_htlc_out_msat\x18\x06 \x01(\x0b\x32\x0b.cln.Amount\x12$\n\x17warning_htlcmin_too_low\x18\x07 \x01(\tH\x01\x88\x01\x01\x12*\n\x15maximum_htlc_out_msat\x18\x08 \x01(\x0b\x32\x0b.cln.Amount\x12%\n\x18warning_htlcmax_too_high\x18\t \x01(\tH\x02\x88\x01\x01\x42\x13\n\x11_short_channel_idB\x1a\n\x18_warning_htlcmin_too_lowB\x1b\n\x19_warning_htlcmax_too_high\"\'\n\x12SigninvoiceRequest\x12\x11\n\tinvstring\x18\x01 \x01(\t\"%\n\x13SigninvoiceResponse\x12\x0e\n\x06\x62olt11\x18\x01 \x01(\t\"%\n\x12SignmessageRequest\x12\x0f\n\x07message\x18\x01 \x01(\t\"F\n\x13SignmessageResponse\x12\x11\n\tsignature\x18\x01 \x01(\x0c\x12\r\n\x05recid\x18\x02 \x01(\x0c\x12\r\n\x05zbase\x18\x03 \x01(\t\"\r\n\x0bStopRequest\"\x0e\n\x0cStopResponse2\xde\x1a\n\x04Node\x12\x36\n\x07Getinfo\x12\x13.cln.GetinfoRequest\x1a\x14.cln.GetinfoResponse\"\x00\x12<\n\tListPeers\x12\x15.cln.ListpeersRequest\x1a\x16.cln.ListpeersResponse\"\x00\x12<\n\tListFunds\x12\x15.cln.ListfundsRequest\x1a\x16.cln.ListfundsResponse\"\x00\x12\x36\n\x07SendPay\x12\x13.cln.SendpayRequest\x1a\x14.cln.SendpayResponse\"\x00\x12\x45\n\x0cListChannels\x12\x18.cln.ListchannelsRequest\x1a\x19.cln.ListchannelsResponse\"\x00\x12<\n\tAddGossip\x12\x15.cln.AddgossipRequest\x1a\x16.cln.AddgossipResponse\"\x00\x12Q\n\x10\x41utoCleanInvoice\x12\x1c.cln.AutocleaninvoiceRequest\x1a\x1d.cln.AutocleaninvoiceResponse\"\x00\x12\x45\n\x0c\x43heckMessage\x12\x18.cln.CheckmessageRequest\x1a\x19.cln.CheckmessageResponse\"\x00\x12\x30\n\x05\x43lose\x12\x11.cln.CloseRequest\x1a\x12.cln.CloseResponse\"\x00\x12:\n\x0b\x43onnectPeer\x12\x13.cln.ConnectRequest\x1a\x14.cln.ConnectResponse\"\x00\x12H\n\rCreateInvoice\x12\x19.cln.CreateinvoiceRequest\x1a\x1a.cln.CreateinvoiceResponse\"\x00\x12<\n\tDatastore\x12\x15.cln.DatastoreRequest\x1a\x16.cln.DatastoreResponse\"\x00\x12\x42\n\x0b\x43reateOnion\x12\x17.cln.CreateonionRequest\x1a\x18.cln.CreateonionResponse\"\x00\x12\x45\n\x0c\x44\x65lDatastore\x12\x18.cln.DeldatastoreRequest\x1a\x19.cln.DeldatastoreResponse\"\x00\x12T\n\x11\x44\x65lExpiredInvoice\x12\x1d.cln.DelexpiredinvoiceRequest\x1a\x1e.cln.DelexpiredinvoiceResponse\"\x00\x12?\n\nDelInvoice\x12\x16.cln.DelinvoiceRequest\x1a\x17.cln.DelinvoiceResponse\"\x00\x12\x36\n\x07Invoice\x12\x13.cln.InvoiceRequest\x1a\x14.cln.InvoiceResponse\"\x00\x12H\n\rListDatastore\x12\x19.cln.ListdatastoreRequest\x1a\x1a.cln.ListdatastoreResponse\"\x00\x12\x45\n\x0cListInvoices\x12\x18.cln.ListinvoicesRequest\x1a\x19.cln.ListinvoicesResponse\"\x00\x12<\n\tSendOnion\x12\x15.cln.SendonionRequest\x1a\x16.cln.SendonionResponse\"\x00\x12\x45\n\x0cListSendPays\x12\x18.cln.ListsendpaysRequest\x1a\x19.cln.ListsendpaysResponse\"\x00\x12Q\n\x10ListTransactions\x12\x1c.cln.ListtransactionsRequest\x1a\x1d.cln.ListtransactionsResponse\"\x00\x12*\n\x03Pay\x12\x0f.cln.PayRequest\x1a\x10.cln.PayResponse\"\x00\x12<\n\tListNodes\x12\x15.cln.ListnodesRequest\x1a\x16.cln.ListnodesResponse\"\x00\x12K\n\x0eWaitAnyInvoice\x12\x1a.cln.WaitanyinvoiceRequest\x1a\x1b.cln.WaitanyinvoiceResponse\"\x00\x12\x42\n\x0bWaitInvoice\x12\x17.cln.WaitinvoiceRequest\x1a\x18.cln.WaitinvoiceResponse\"\x00\x12\x42\n\x0bWaitSendPay\x12\x17.cln.WaitsendpayRequest\x1a\x18.cln.WaitsendpayResponse\"\x00\x12\x36\n\x07NewAddr\x12\x13.cln.NewaddrRequest\x1a\x14.cln.NewaddrResponse\"\x00\x12\x39\n\x08Withdraw\x12\x14.cln.WithdrawRequest\x1a\x15.cln.WithdrawResponse\"\x00\x12\x36\n\x07KeySend\x12\x13.cln.KeysendRequest\x1a\x14.cln.KeysendResponse\"\x00\x12\x39\n\x08\x46undPsbt\x12\x14.cln.FundpsbtRequest\x1a\x15.cln.FundpsbtResponse\"\x00\x12\x39\n\x08SendPsbt\x12\x14.cln.SendpsbtRequest\x1a\x15.cln.SendpsbtResponse\"\x00\x12\x39\n\x08SignPsbt\x12\x14.cln.SignpsbtRequest\x1a\x15.cln.SignpsbtResponse\"\x00\x12\x39\n\x08UtxoPsbt\x12\x14.cln.UtxopsbtRequest\x1a\x15.cln.UtxopsbtResponse\"\x00\x12<\n\tTxDiscard\x12\x15.cln.TxdiscardRequest\x1a\x16.cln.TxdiscardResponse\"\x00\x12<\n\tTxPrepare\x12\x15.cln.TxprepareRequest\x1a\x16.cln.TxprepareResponse\"\x00\x12\x33\n\x06TxSend\x12\x12.cln.TxsendRequest\x1a\x13.cln.TxsendResponse\"\x00\x12Q\n\x10ListPeerChannels\x12\x1c.cln.ListpeerchannelsRequest\x1a\x1d.cln.ListpeerchannelsResponse\"\x00\x12W\n\x12ListClosedChannels\x12\x1e.cln.ListclosedchannelsRequest\x1a\x1f.cln.ListclosedchannelsResponse\"\x00\x12<\n\tDecodePay\x12\x15.cln.DecodepayRequest\x1a\x16.cln.DecodepayResponse\"\x00\x12\x33\n\x06\x44\x65\x63ode\x12\x12.cln.DecodeRequest\x1a\x13.cln.DecodeResponse\"\x00\x12?\n\nDisconnect\x12\x16.cln.DisconnectRequest\x1a\x17.cln.DisconnectResponse\"\x00\x12\x39\n\x08\x46\x65\x65rates\x12\x14.cln.FeeratesRequest\x1a\x15.cln.FeeratesResponse\"\x00\x12\x42\n\x0b\x46undChannel\x12\x17.cln.FundchannelRequest\x1a\x18.cln.FundchannelResponse\"\x00\x12\x39\n\x08GetRoute\x12\x14.cln.GetrouteRequest\x1a\x15.cln.GetrouteResponse\"\x00\x12\x45\n\x0cListForwards\x12\x18.cln.ListforwardsRequest\x1a\x19.cln.ListforwardsResponse\"\x00\x12\x39\n\x08ListPays\x12\x14.cln.ListpaysRequest\x1a\x15.cln.ListpaysResponse\"\x00\x12-\n\x04Ping\x12\x10.cln.PingRequest\x1a\x11.cln.PingResponse\"\x00\x12H\n\rSendCustomMsg\x12\x19.cln.SendcustommsgRequest\x1a\x1a.cln.SendcustommsgResponse\"\x00\x12?\n\nSetChannel\x12\x16.cln.SetchannelRequest\x1a\x17.cln.SetchannelResponse\"\x00\x12\x42\n\x0bSignInvoice\x12\x17.cln.SigninvoiceRequest\x1a\x18.cln.SigninvoiceResponse\"\x00\x12\x42\n\x0bSignMessage\x12\x17.cln.SignmessageRequest\x1a\x18.cln.SignmessageResponse\"\x00\x12-\n\x04Stop\x12\x10.cln.StopRequest\x1a\x11.cln.StopResponse\"\x00\x62\x06proto3')
 
 
 
 _GETINFOREQUEST = DESCRIPTOR.message_types_by_name['GetinfoRequest']
 _GETINFORESPONSE = DESCRIPTOR.message_types_by_name['GetinfoResponse']
 _GETINFOOUR_FEATURES = DESCRIPTOR.message_types_by_name['GetinfoOur_features']
 _GETINFOADDRESS = DESCRIPTOR.message_types_by_name['GetinfoAddress']
@@ -117,20 +117,47 @@
 _UTXOPSBTRESERVATIONS = DESCRIPTOR.message_types_by_name['UtxopsbtReservations']
 _TXDISCARDREQUEST = DESCRIPTOR.message_types_by_name['TxdiscardRequest']
 _TXDISCARDRESPONSE = DESCRIPTOR.message_types_by_name['TxdiscardResponse']
 _TXPREPAREREQUEST = DESCRIPTOR.message_types_by_name['TxprepareRequest']
 _TXPREPARERESPONSE = DESCRIPTOR.message_types_by_name['TxprepareResponse']
 _TXSENDREQUEST = DESCRIPTOR.message_types_by_name['TxsendRequest']
 _TXSENDRESPONSE = DESCRIPTOR.message_types_by_name['TxsendResponse']
+_LISTPEERCHANNELSREQUEST = DESCRIPTOR.message_types_by_name['ListpeerchannelsRequest']
+_LISTPEERCHANNELSRESPONSE = DESCRIPTOR.message_types_by_name['ListpeerchannelsResponse']
+_LISTPEERCHANNELSCHANNELS = DESCRIPTOR.message_types_by_name['ListpeerchannelsChannels']
+_LISTPEERCHANNELSCHANNELSFEERATE = DESCRIPTOR.message_types_by_name['ListpeerchannelsChannelsFeerate']
+_LISTPEERCHANNELSCHANNELSINFLIGHT = DESCRIPTOR.message_types_by_name['ListpeerchannelsChannelsInflight']
+_LISTPEERCHANNELSCHANNELSFUNDING = DESCRIPTOR.message_types_by_name['ListpeerchannelsChannelsFunding']
+_LISTPEERCHANNELSCHANNELSALIAS = DESCRIPTOR.message_types_by_name['ListpeerchannelsChannelsAlias']
+_LISTPEERCHANNELSCHANNELSHTLCS = DESCRIPTOR.message_types_by_name['ListpeerchannelsChannelsHtlcs']
+_LISTCLOSEDCHANNELSREQUEST = DESCRIPTOR.message_types_by_name['ListclosedchannelsRequest']
+_LISTCLOSEDCHANNELSRESPONSE = DESCRIPTOR.message_types_by_name['ListclosedchannelsResponse']
+_LISTCLOSEDCHANNELSCLOSEDCHANNELS = DESCRIPTOR.message_types_by_name['ListclosedchannelsClosedchannels']
+_LISTCLOSEDCHANNELSCLOSEDCHANNELSALIAS = DESCRIPTOR.message_types_by_name['ListclosedchannelsClosedchannelsAlias']
+_DECODEPAYREQUEST = DESCRIPTOR.message_types_by_name['DecodepayRequest']
+_DECODEPAYRESPONSE = DESCRIPTOR.message_types_by_name['DecodepayResponse']
+_DECODEPAYFALLBACKS = DESCRIPTOR.message_types_by_name['DecodepayFallbacks']
+_DECODEPAYEXTRA = DESCRIPTOR.message_types_by_name['DecodepayExtra']
+_DECODEREQUEST = DESCRIPTOR.message_types_by_name['DecodeRequest']
+_DECODERESPONSE = DESCRIPTOR.message_types_by_name['DecodeResponse']
+_DECODEOFFER_PATHS = DESCRIPTOR.message_types_by_name['DecodeOffer_paths']
+_DECODEOFFER_RECURRENCEPAYWINDOW = DESCRIPTOR.message_types_by_name['DecodeOffer_recurrencePaywindow']
+_DECODEINVOICE_PATHSPATH = DESCRIPTOR.message_types_by_name['DecodeInvoice_pathsPath']
+_DECODEINVOICE_FALLBACKS = DESCRIPTOR.message_types_by_name['DecodeInvoice_fallbacks']
+_DECODEFALLBACKS = DESCRIPTOR.message_types_by_name['DecodeFallbacks']
+_DECODEEXTRA = DESCRIPTOR.message_types_by_name['DecodeExtra']
+_DECODERESTRICTIONS = DESCRIPTOR.message_types_by_name['DecodeRestrictions']
 _DISCONNECTREQUEST = DESCRIPTOR.message_types_by_name['DisconnectRequest']
 _DISCONNECTRESPONSE = DESCRIPTOR.message_types_by_name['DisconnectResponse']
 _FEERATESREQUEST = DESCRIPTOR.message_types_by_name['FeeratesRequest']
 _FEERATESRESPONSE = DESCRIPTOR.message_types_by_name['FeeratesResponse']
 _FEERATESPERKB = DESCRIPTOR.message_types_by_name['FeeratesPerkb']
+_FEERATESPERKBESTIMATES = DESCRIPTOR.message_types_by_name['FeeratesPerkbEstimates']
 _FEERATESPERKW = DESCRIPTOR.message_types_by_name['FeeratesPerkw']
+_FEERATESPERKWESTIMATES = DESCRIPTOR.message_types_by_name['FeeratesPerkwEstimates']
 _FEERATESONCHAIN_FEE_ESTIMATES = DESCRIPTOR.message_types_by_name['FeeratesOnchain_fee_estimates']
 _FUNDCHANNELREQUEST = DESCRIPTOR.message_types_by_name['FundchannelRequest']
 _FUNDCHANNELRESPONSE = DESCRIPTOR.message_types_by_name['FundchannelResponse']
 _GETROUTEREQUEST = DESCRIPTOR.message_types_by_name['GetrouteRequest']
 _GETROUTERESPONSE = DESCRIPTOR.message_types_by_name['GetrouteResponse']
 _GETROUTEROUTE = DESCRIPTOR.message_types_by_name['GetrouteRoute']
 _LISTFORWARDSREQUEST = DESCRIPTOR.message_types_by_name['ListforwardsRequest']
@@ -175,14 +202,19 @@
 _PAYRESPONSE_PAYSTATUS = _PAYRESPONSE.enum_types_by_name['PayStatus']
 _LISTNODESNODESADDRESSES_LISTNODESNODESADDRESSESTYPE = _LISTNODESNODESADDRESSES.enum_types_by_name['ListnodesNodesAddressesType']
 _WAITANYINVOICERESPONSE_WAITANYINVOICESTATUS = _WAITANYINVOICERESPONSE.enum_types_by_name['WaitanyinvoiceStatus']
 _WAITINVOICERESPONSE_WAITINVOICESTATUS = _WAITINVOICERESPONSE.enum_types_by_name['WaitinvoiceStatus']
 _WAITSENDPAYRESPONSE_WAITSENDPAYSTATUS = _WAITSENDPAYRESPONSE.enum_types_by_name['WaitsendpayStatus']
 _NEWADDRREQUEST_NEWADDRADDRESSTYPE = _NEWADDRREQUEST.enum_types_by_name['NewaddrAddresstype']
 _KEYSENDRESPONSE_KEYSENDSTATUS = _KEYSENDRESPONSE.enum_types_by_name['KeysendStatus']
+_LISTPEERCHANNELSCHANNELS_LISTPEERCHANNELSCHANNELSSTATE = _LISTPEERCHANNELSCHANNELS.enum_types_by_name['ListpeerchannelsChannelsState']
+_LISTPEERCHANNELSCHANNELSHTLCS_LISTPEERCHANNELSCHANNELSHTLCSDIRECTION = _LISTPEERCHANNELSCHANNELSHTLCS.enum_types_by_name['ListpeerchannelsChannelsHtlcsDirection']
+_LISTCLOSEDCHANNELSCLOSEDCHANNELS_LISTCLOSEDCHANNELSCLOSEDCHANNELSCLOSE_CAUSE = _LISTCLOSEDCHANNELSCLOSEDCHANNELS.enum_types_by_name['ListclosedchannelsClosedchannelsClose_cause']
+_DECODEPAYFALLBACKS_DECODEPAYFALLBACKSTYPE = _DECODEPAYFALLBACKS.enum_types_by_name['DecodepayFallbacksType']
+_DECODERESPONSE_DECODETYPE = _DECODERESPONSE.enum_types_by_name['DecodeType']
 _FEERATESREQUEST_FEERATESSTYLE = _FEERATESREQUEST.enum_types_by_name['FeeratesStyle']
 _GETROUTEROUTE_GETROUTEROUTESTYLE = _GETROUTEROUTE.enum_types_by_name['GetrouteRouteStyle']
 _LISTFORWARDSREQUEST_LISTFORWARDSSTATUS = _LISTFORWARDSREQUEST.enum_types_by_name['ListforwardsStatus']
 _LISTFORWARDSFORWARDS_LISTFORWARDSFORWARDSSTATUS = _LISTFORWARDSFORWARDS.enum_types_by_name['ListforwardsForwardsStatus']
 _LISTFORWARDSFORWARDS_LISTFORWARDSFORWARDSSTYLE = _LISTFORWARDSFORWARDS.enum_types_by_name['ListforwardsForwardsStyle']
 _LISTPAYSREQUEST_LISTPAYSSTATUS = _LISTPAYSREQUEST.enum_types_by_name['ListpaysStatus']
 _LISTPAYSPAYS_LISTPAYSPAYSSTATUS = _LISTPAYSPAYS.enum_types_by_name['ListpaysPaysStatus']
@@ -896,14 +928,189 @@
 TxsendResponse = _reflection.GeneratedProtocolMessageType('TxsendResponse', (_message.Message,), {
   'DESCRIPTOR' : _TXSENDRESPONSE,
   '__module__' : 'node_pb2'
   # @@protoc_insertion_point(class_scope:cln.TxsendResponse)
   })
 _sym_db.RegisterMessage(TxsendResponse)
 
+ListpeerchannelsRequest = _reflection.GeneratedProtocolMessageType('ListpeerchannelsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _LISTPEERCHANNELSREQUEST,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.ListpeerchannelsRequest)
+  })
+_sym_db.RegisterMessage(ListpeerchannelsRequest)
+
+ListpeerchannelsResponse = _reflection.GeneratedProtocolMessageType('ListpeerchannelsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _LISTPEERCHANNELSRESPONSE,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.ListpeerchannelsResponse)
+  })
+_sym_db.RegisterMessage(ListpeerchannelsResponse)
+
+ListpeerchannelsChannels = _reflection.GeneratedProtocolMessageType('ListpeerchannelsChannels', (_message.Message,), {
+  'DESCRIPTOR' : _LISTPEERCHANNELSCHANNELS,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.ListpeerchannelsChannels)
+  })
+_sym_db.RegisterMessage(ListpeerchannelsChannels)
+
+ListpeerchannelsChannelsFeerate = _reflection.GeneratedProtocolMessageType('ListpeerchannelsChannelsFeerate', (_message.Message,), {
+  'DESCRIPTOR' : _LISTPEERCHANNELSCHANNELSFEERATE,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.ListpeerchannelsChannelsFeerate)
+  })
+_sym_db.RegisterMessage(ListpeerchannelsChannelsFeerate)
+
+ListpeerchannelsChannelsInflight = _reflection.GeneratedProtocolMessageType('ListpeerchannelsChannelsInflight', (_message.Message,), {
+  'DESCRIPTOR' : _LISTPEERCHANNELSCHANNELSINFLIGHT,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.ListpeerchannelsChannelsInflight)
+  })
+_sym_db.RegisterMessage(ListpeerchannelsChannelsInflight)
+
+ListpeerchannelsChannelsFunding = _reflection.GeneratedProtocolMessageType('ListpeerchannelsChannelsFunding', (_message.Message,), {
+  'DESCRIPTOR' : _LISTPEERCHANNELSCHANNELSFUNDING,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.ListpeerchannelsChannelsFunding)
+  })
+_sym_db.RegisterMessage(ListpeerchannelsChannelsFunding)
+
+ListpeerchannelsChannelsAlias = _reflection.GeneratedProtocolMessageType('ListpeerchannelsChannelsAlias', (_message.Message,), {
+  'DESCRIPTOR' : _LISTPEERCHANNELSCHANNELSALIAS,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.ListpeerchannelsChannelsAlias)
+  })
+_sym_db.RegisterMessage(ListpeerchannelsChannelsAlias)
+
+ListpeerchannelsChannelsHtlcs = _reflection.GeneratedProtocolMessageType('ListpeerchannelsChannelsHtlcs', (_message.Message,), {
+  'DESCRIPTOR' : _LISTPEERCHANNELSCHANNELSHTLCS,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.ListpeerchannelsChannelsHtlcs)
+  })
+_sym_db.RegisterMessage(ListpeerchannelsChannelsHtlcs)
+
+ListclosedchannelsRequest = _reflection.GeneratedProtocolMessageType('ListclosedchannelsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _LISTCLOSEDCHANNELSREQUEST,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.ListclosedchannelsRequest)
+  })
+_sym_db.RegisterMessage(ListclosedchannelsRequest)
+
+ListclosedchannelsResponse = _reflection.GeneratedProtocolMessageType('ListclosedchannelsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _LISTCLOSEDCHANNELSRESPONSE,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.ListclosedchannelsResponse)
+  })
+_sym_db.RegisterMessage(ListclosedchannelsResponse)
+
+ListclosedchannelsClosedchannels = _reflection.GeneratedProtocolMessageType('ListclosedchannelsClosedchannels', (_message.Message,), {
+  'DESCRIPTOR' : _LISTCLOSEDCHANNELSCLOSEDCHANNELS,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.ListclosedchannelsClosedchannels)
+  })
+_sym_db.RegisterMessage(ListclosedchannelsClosedchannels)
+
+ListclosedchannelsClosedchannelsAlias = _reflection.GeneratedProtocolMessageType('ListclosedchannelsClosedchannelsAlias', (_message.Message,), {
+  'DESCRIPTOR' : _LISTCLOSEDCHANNELSCLOSEDCHANNELSALIAS,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.ListclosedchannelsClosedchannelsAlias)
+  })
+_sym_db.RegisterMessage(ListclosedchannelsClosedchannelsAlias)
+
+DecodepayRequest = _reflection.GeneratedProtocolMessageType('DecodepayRequest', (_message.Message,), {
+  'DESCRIPTOR' : _DECODEPAYREQUEST,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodepayRequest)
+  })
+_sym_db.RegisterMessage(DecodepayRequest)
+
+DecodepayResponse = _reflection.GeneratedProtocolMessageType('DecodepayResponse', (_message.Message,), {
+  'DESCRIPTOR' : _DECODEPAYRESPONSE,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodepayResponse)
+  })
+_sym_db.RegisterMessage(DecodepayResponse)
+
+DecodepayFallbacks = _reflection.GeneratedProtocolMessageType('DecodepayFallbacks', (_message.Message,), {
+  'DESCRIPTOR' : _DECODEPAYFALLBACKS,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodepayFallbacks)
+  })
+_sym_db.RegisterMessage(DecodepayFallbacks)
+
+DecodepayExtra = _reflection.GeneratedProtocolMessageType('DecodepayExtra', (_message.Message,), {
+  'DESCRIPTOR' : _DECODEPAYEXTRA,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodepayExtra)
+  })
+_sym_db.RegisterMessage(DecodepayExtra)
+
+DecodeRequest = _reflection.GeneratedProtocolMessageType('DecodeRequest', (_message.Message,), {
+  'DESCRIPTOR' : _DECODEREQUEST,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodeRequest)
+  })
+_sym_db.RegisterMessage(DecodeRequest)
+
+DecodeResponse = _reflection.GeneratedProtocolMessageType('DecodeResponse', (_message.Message,), {
+  'DESCRIPTOR' : _DECODERESPONSE,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodeResponse)
+  })
+_sym_db.RegisterMessage(DecodeResponse)
+
+DecodeOffer_paths = _reflection.GeneratedProtocolMessageType('DecodeOffer_paths', (_message.Message,), {
+  'DESCRIPTOR' : _DECODEOFFER_PATHS,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodeOffer_paths)
+  })
+_sym_db.RegisterMessage(DecodeOffer_paths)
+
+DecodeOffer_recurrencePaywindow = _reflection.GeneratedProtocolMessageType('DecodeOffer_recurrencePaywindow', (_message.Message,), {
+  'DESCRIPTOR' : _DECODEOFFER_RECURRENCEPAYWINDOW,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodeOffer_recurrencePaywindow)
+  })
+_sym_db.RegisterMessage(DecodeOffer_recurrencePaywindow)
+
+DecodeInvoice_pathsPath = _reflection.GeneratedProtocolMessageType('DecodeInvoice_pathsPath', (_message.Message,), {
+  'DESCRIPTOR' : _DECODEINVOICE_PATHSPATH,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodeInvoice_pathsPath)
+  })
+_sym_db.RegisterMessage(DecodeInvoice_pathsPath)
+
+DecodeInvoice_fallbacks = _reflection.GeneratedProtocolMessageType('DecodeInvoice_fallbacks', (_message.Message,), {
+  'DESCRIPTOR' : _DECODEINVOICE_FALLBACKS,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodeInvoice_fallbacks)
+  })
+_sym_db.RegisterMessage(DecodeInvoice_fallbacks)
+
+DecodeFallbacks = _reflection.GeneratedProtocolMessageType('DecodeFallbacks', (_message.Message,), {
+  'DESCRIPTOR' : _DECODEFALLBACKS,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodeFallbacks)
+  })
+_sym_db.RegisterMessage(DecodeFallbacks)
+
+DecodeExtra = _reflection.GeneratedProtocolMessageType('DecodeExtra', (_message.Message,), {
+  'DESCRIPTOR' : _DECODEEXTRA,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodeExtra)
+  })
+_sym_db.RegisterMessage(DecodeExtra)
+
+DecodeRestrictions = _reflection.GeneratedProtocolMessageType('DecodeRestrictions', (_message.Message,), {
+  'DESCRIPTOR' : _DECODERESTRICTIONS,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.DecodeRestrictions)
+  })
+_sym_db.RegisterMessage(DecodeRestrictions)
+
 DisconnectRequest = _reflection.GeneratedProtocolMessageType('DisconnectRequest', (_message.Message,), {
   'DESCRIPTOR' : _DISCONNECTREQUEST,
   '__module__' : 'node_pb2'
   # @@protoc_insertion_point(class_scope:cln.DisconnectRequest)
   })
 _sym_db.RegisterMessage(DisconnectRequest)
 
@@ -931,21 +1138,35 @@
 FeeratesPerkb = _reflection.GeneratedProtocolMessageType('FeeratesPerkb', (_message.Message,), {
   'DESCRIPTOR' : _FEERATESPERKB,
   '__module__' : 'node_pb2'
   # @@protoc_insertion_point(class_scope:cln.FeeratesPerkb)
   })
 _sym_db.RegisterMessage(FeeratesPerkb)
 
+FeeratesPerkbEstimates = _reflection.GeneratedProtocolMessageType('FeeratesPerkbEstimates', (_message.Message,), {
+  'DESCRIPTOR' : _FEERATESPERKBESTIMATES,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.FeeratesPerkbEstimates)
+  })
+_sym_db.RegisterMessage(FeeratesPerkbEstimates)
+
 FeeratesPerkw = _reflection.GeneratedProtocolMessageType('FeeratesPerkw', (_message.Message,), {
   'DESCRIPTOR' : _FEERATESPERKW,
   '__module__' : 'node_pb2'
   # @@protoc_insertion_point(class_scope:cln.FeeratesPerkw)
   })
 _sym_db.RegisterMessage(FeeratesPerkw)
 
+FeeratesPerkwEstimates = _reflection.GeneratedProtocolMessageType('FeeratesPerkwEstimates', (_message.Message,), {
+  'DESCRIPTOR' : _FEERATESPERKWESTIMATES,
+  '__module__' : 'node_pb2'
+  # @@protoc_insertion_point(class_scope:cln.FeeratesPerkwEstimates)
+  })
+_sym_db.RegisterMessage(FeeratesPerkwEstimates)
+
 FeeratesOnchain_fee_estimates = _reflection.GeneratedProtocolMessageType('FeeratesOnchain_fee_estimates', (_message.Message,), {
   'DESCRIPTOR' : _FEERATESONCHAIN_FEE_ESTIMATES,
   '__module__' : 'node_pb2'
   # @@protoc_insertion_point(class_scope:cln.FeeratesOnchain_fee_estimates)
   })
 _sym_db.RegisterMessage(FeeratesOnchain_fee_estimates)
 
@@ -1120,341 +1341,405 @@
 _NODE = DESCRIPTOR.services_by_name['Node']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _GETINFOREQUEST._serialized_start=37
   _GETINFOREQUEST._serialized_end=53
   _GETINFORESPONSE._serialized_start=56
-  _GETINFORESPONSE._serialized_end=684
-  _GETINFOOUR_FEATURES._serialized_start=686
-  _GETINFOOUR_FEATURES._serialized_end=769
-  _GETINFOADDRESS._serialized_start=772
-  _GETINFOADDRESS._serialized_end=983
-  _GETINFOADDRESS_GETINFOADDRESSTYPE._serialized_start=885
-  _GETINFOADDRESS_GETINFOADDRESSTYPE._serialized_end=971
-  _GETINFOBINDING._serialized_start=986
-  _GETINFOBINDING._serialized_end=1237
-  _GETINFOBINDING_GETINFOBINDINGTYPE._serialized_start=1125
-  _GETINFOBINDING_GETINFOBINDINGTYPE._serialized_end=1205
-  _LISTPEERSREQUEST._serialized_start=1239
-  _LISTPEERSREQUEST._serialized_end=1311
-  _LISTPEERSRESPONSE._serialized_start=1313
-  _LISTPEERSRESPONSE._serialized_end=1368
-  _LISTPEERSPEERS._serialized_start=1371
-  _LISTPEERSPEERS._serialized_end=1619
-  _LISTPEERSPEERSLOG._serialized_start=1622
-  _LISTPEERSPEERSLOG._serialized_end=2003
-  _LISTPEERSPEERSLOG_LISTPEERSPEERSLOGTYPE._serialized_start=1833
-  _LISTPEERSPEERSLOG_LISTPEERSPEERSLOGTYPE._serialized_end=1938
-  _LISTPEERSPEERSCHANNELS._serialized_start=2006
-  _LISTPEERSPEERSCHANNELS._serialized_end=5036
-  _LISTPEERSPEERSCHANNELS_LISTPEERSPEERSCHANNELSSTATE._serialized_start=3906
-  _LISTPEERSPEERSCHANNELS_LISTPEERSPEERSCHANNELSSTATE._serialized_end=4195
-  _LISTPEERSPEERSCHANNELSFEERATE._serialized_start=5038
-  _LISTPEERSPEERSCHANNELSFEERATE._serialized_end=5099
-  _LISTPEERSPEERSCHANNELSINFLIGHT._serialized_start=5102
-  _LISTPEERSPEERSCHANNELSINFLIGHT._serialized_end=5299
-  _LISTPEERSPEERSCHANNELSFUNDING._serialized_start=5302
-  _LISTPEERSPEERSCHANNELSFUNDING._serialized_end=5693
-  _LISTPEERSPEERSCHANNELSALIAS._serialized_start=5695
-  _LISTPEERSPEERSCHANNELSALIAS._serialized_end=5786
-  _LISTPEERSPEERSCHANNELSHTLCS._serialized_start=5789
-  _LISTPEERSPEERSCHANNELSHTLCS._serialized_end=6127
-  _LISTPEERSPEERSCHANNELSHTLCS_LISTPEERSPEERSCHANNELSHTLCSDIRECTION._serialized_start=6043
-  _LISTPEERSPEERSCHANNELSHTLCS_LISTPEERSPEERSCHANNELSHTLCSDIRECTION._serialized_end=6098
-  _LISTFUNDSREQUEST._serialized_start=6129
-  _LISTFUNDSREQUEST._serialized_end=6177
-  _LISTFUNDSRESPONSE._serialized_start=6179
-  _LISTFUNDSRESPONSE._serialized_end=6280
-  _LISTFUNDSOUTPUTS._serialized_start=6283
-  _LISTFUNDSOUTPUTS._serialized_end=6670
-  _LISTFUNDSOUTPUTS_LISTFUNDSOUTPUTSSTATUS._serialized_start=6544
-  _LISTFUNDSOUTPUTS_LISTFUNDSOUTPUTSSTATUS._serialized_end=6625
-  _LISTFUNDSCHANNELS._serialized_start=6673
-  _LISTFUNDSCHANNELS._serialized_end=6932
-  _SENDPAYREQUEST._serialized_start=6935
-  _SENDPAYREQUEST._serialized_end=7284
-  _SENDPAYRESPONSE._serialized_start=7287
-  _SENDPAYRESPONSE._serialized_end=7880
-  _SENDPAYRESPONSE_SENDPAYSTATUS._serialized_start=7701
-  _SENDPAYRESPONSE_SENDPAYSTATUS._serialized_end=7743
-  _SENDPAYROUTE._serialized_start=7882
-  _SENDPAYROUTE._serialized_end=7974
-  _LISTCHANNELSREQUEST._serialized_start=7977
-  _LISTCHANNELSREQUEST._serialized_end=8124
-  _LISTCHANNELSRESPONSE._serialized_start=8126
-  _LISTCHANNELSRESPONSE._serialized_end=8193
-  _LISTCHANNELSCHANNELS._serialized_start=8196
-  _LISTCHANNELSCHANNELS._serialized_end=8631
-  _ADDGOSSIPREQUEST._serialized_start=8633
-  _ADDGOSSIPREQUEST._serialized_end=8668
-  _ADDGOSSIPRESPONSE._serialized_start=8670
-  _ADDGOSSIPRESPONSE._serialized_end=8689
-  _AUTOCLEANINVOICEREQUEST._serialized_start=8691
-  _AUTOCLEANINVOICEREQUEST._serialized_end=8802
-  _AUTOCLEANINVOICERESPONSE._serialized_start=8805
-  _AUTOCLEANINVOICERESPONSE._serialized_end=8934
-  _CHECKMESSAGEREQUEST._serialized_start=8936
-  _CHECKMESSAGEREQUEST._serialized_end=9021
-  _CHECKMESSAGERESPONSE._serialized_start=9023
-  _CHECKMESSAGERESPONSE._serialized_end=9079
-  _CLOSEREQUEST._serialized_start=9082
-  _CLOSEREQUEST._serialized_end=9413
-  _CLOSERESPONSE._serialized_start=9416
-  _CLOSERESPONSE._serialized_end=9587
-  _CLOSERESPONSE_CLOSETYPE._serialized_start=9518
-  _CLOSERESPONSE_CLOSETYPE._serialized_end=9571
-  _CONNECTREQUEST._serialized_start=9589
-  _CONNECTREQUEST._serialized_end=9673
-  _CONNECTRESPONSE._serialized_start=9676
-  _CONNECTRESPONSE._serialized_end=9856
-  _CONNECTRESPONSE_CONNECTDIRECTION._serialized_start=9821
-  _CONNECTRESPONSE_CONNECTDIRECTION._serialized_end=9856
-  _CONNECTADDRESS._serialized_start=9859
-  _CONNECTADDRESS._serialized_end=10110
-  _CONNECTADDRESS_CONNECTADDRESSTYPE._serialized_start=9998
-  _CONNECTADDRESS_CONNECTADDRESSTYPE._serialized_end=10078
-  _CREATEINVOICEREQUEST._serialized_start=10112
-  _CREATEINVOICEREQUEST._serialized_end=10186
-  _CREATEINVOICERESPONSE._serialized_start=10189
-  _CREATEINVOICERESPONSE._serialized_end=10830
-  _CREATEINVOICERESPONSE_CREATEINVOICESTATUS._serialized_start=10623
-  _CREATEINVOICERESPONSE_CREATEINVOICESTATUS._serialized_end=10679
-  _DATASTOREREQUEST._serialized_start=10833
-  _DATASTOREREQUEST._serialized_end=11141
-  _DATASTOREREQUEST_DATASTOREMODE._serialized_start=10986
-  _DATASTOREREQUEST_DATASTOREMODE._serialized_end=11098
-  _DATASTORERESPONSE._serialized_start=11144
-  _DATASTORERESPONSE._serialized_end=11274
-  _CREATEONIONREQUEST._serialized_start=11277
-  _CREATEONIONREQUEST._serialized_end=11434
-  _CREATEONIONRESPONSE._serialized_start=11436
-  _CREATEONIONRESPONSE._serialized_end=11496
-  _CREATEONIONHOPS._serialized_start=11498
-  _CREATEONIONHOPS._serialized_end=11548
-  _DELDATASTOREREQUEST._serialized_start=11550
-  _DELDATASTOREREQUEST._serialized_end=11624
-  _DELDATASTORERESPONSE._serialized_start=11627
-  _DELDATASTORERESPONSE._serialized_end=11760
-  _DELEXPIREDINVOICEREQUEST._serialized_start=11762
-  _DELEXPIREDINVOICEREQUEST._serialized_end=11834
-  _DELEXPIREDINVOICERESPONSE._serialized_start=11836
-  _DELEXPIREDINVOICERESPONSE._serialized_end=11863
-  _DELINVOICEREQUEST._serialized_start=11866
-  _DELINVOICEREQUEST._serialized_end=12048
-  _DELINVOICEREQUEST_DELINVOICESTATUS._serialized_start=11982
-  _DELINVOICEREQUEST_DELINVOICESTATUS._serialized_end=12035
-  _DELINVOICERESPONSE._serialized_start=12051
-  _DELINVOICERESPONSE._serialized_end=12504
-  _DELINVOICERESPONSE_DELINVOICESTATUS._serialized_start=11982
-  _DELINVOICERESPONSE_DELINVOICESTATUS._serialized_end=12035
-  _INVOICEREQUEST._serialized_start=12507
-  _INVOICEREQUEST._serialized_end=12819
-  _INVOICERESPONSE._serialized_start=12822
-  _INVOICERESPONSE._serialized_end=13181
-  _LISTDATASTOREREQUEST._serialized_start=13183
-  _LISTDATASTOREREQUEST._serialized_end=13218
-  _LISTDATASTORERESPONSE._serialized_start=13220
-  _LISTDATASTORERESPONSE._serialized_end=13291
-  _LISTDATASTOREDATASTORE._serialized_start=13294
-  _LISTDATASTOREDATASTORE._serialized_end=13429
-  _LISTINVOICESREQUEST._serialized_start=13432
-  _LISTINVOICESREQUEST._serialized_end=13601
-  _LISTINVOICESRESPONSE._serialized_start=13603
-  _LISTINVOICESRESPONSE._serialized_end=13670
-  _LISTINVOICESINVOICES._serialized_start=13673
-  _LISTINVOICESINVOICES._serialized_end=14347
-  _LISTINVOICESINVOICES_LISTINVOICESINVOICESSTATUS._serialized_start=14117
-  _LISTINVOICESINVOICES_LISTINVOICESINVOICESSTATUS._serialized_end=14180
-  _SENDONIONREQUEST._serialized_start=14350
-  _SENDONIONREQUEST._serialized_end=14744
-  _SENDONIONRESPONSE._serialized_start=14747
-  _SENDONIONRESPONSE._serialized_end=15270
-  _SENDONIONRESPONSE_SENDONIONSTATUS._serialized_start=15118
-  _SENDONIONRESPONSE_SENDONIONSTATUS._serialized_end=15162
-  _SENDONIONFIRST_HOP._serialized_start=15272
-  _SENDONIONFIRST_HOP._serialized_end=15353
-  _LISTSENDPAYSREQUEST._serialized_start=15356
-  _LISTSENDPAYSREQUEST._serialized_end=15591
-  _LISTSENDPAYSREQUEST_LISTSENDPAYSSTATUS._serialized_start=15493
-  _LISTSENDPAYSREQUEST_LISTSENDPAYSSTATUS._serialized_end=15552
-  _LISTSENDPAYSRESPONSE._serialized_start=15593
-  _LISTSENDPAYSRESPONSE._serialized_end=15660
-  _LISTSENDPAYSPAYMENTS._serialized_start=15663
-  _LISTSENDPAYSPAYMENTS._serialized_end=16291
-  _LISTSENDPAYSPAYMENTS_LISTSENDPAYSPAYMENTSSTATUS._serialized_start=16097
-  _LISTSENDPAYSPAYMENTS_LISTSENDPAYSPAYMENTSSTATUS._serialized_end=16164
-  _LISTTRANSACTIONSREQUEST._serialized_start=16293
-  _LISTTRANSACTIONSREQUEST._serialized_end=16318
-  _LISTTRANSACTIONSRESPONSE._serialized_start=16320
-  _LISTTRANSACTIONSRESPONSE._serialized_end=16403
-  _LISTTRANSACTIONSTRANSACTIONS._serialized_start=16406
-  _LISTTRANSACTIONSTRANSACTIONS._serialized_end=16654
-  _LISTTRANSACTIONSTRANSACTIONSINPUTS._serialized_start=16657
-  _LISTTRANSACTIONSTRANSACTIONSINPUTS._serialized_end=17173
-  _LISTTRANSACTIONSTRANSACTIONSINPUTS_LISTTRANSACTIONSTRANSACTIONSINPUTSTYPE._serialized_start=16869
-  _LISTTRANSACTIONSTRANSACTIONSINPUTS_LISTTRANSACTIONSTRANSACTIONSINPUTSTYPE._serialized_end=17147
-  _LISTTRANSACTIONSTRANSACTIONSOUTPUTS._serialized_start=17176
-  _LISTTRANSACTIONSTRANSACTIONSOUTPUTS._serialized_end=17720
-  _LISTTRANSACTIONSTRANSACTIONSOUTPUTS_LISTTRANSACTIONSTRANSACTIONSOUTPUTSTYPE._serialized_start=17415
-  _LISTTRANSACTIONSTRANSACTIONSOUTPUTS_LISTTRANSACTIONSTRANSACTIONSOUTPUTSTYPE._serialized_end=17694
-  _PAYREQUEST._serialized_start=17723
-  _PAYREQUEST._serialized_end=18197
-  _PAYRESPONSE._serialized_start=18200
-  _PAYRESPONSE._serialized_end=18579
-  _PAYRESPONSE_PAYSTATUS._serialized_start=18482
-  _PAYRESPONSE_PAYSTATUS._serialized_end=18532
-  _LISTNODESREQUEST._serialized_start=18581
-  _LISTNODESREQUEST._serialized_end=18623
-  _LISTNODESRESPONSE._serialized_start=18625
-  _LISTNODESRESPONSE._serialized_end=18680
-  _LISTNODESNODES._serialized_start=18683
-  _LISTNODESNODES._serialized_end=18908
-  _LISTNODESNODESADDRESSES._serialized_start=18911
-  _LISTNODESNODESADDRESSES._serialized_end=19158
-  _LISTNODESNODESADDRESSES_LISTNODESNODESADDRESSESTYPE._serialized_start=19051
-  _LISTNODESNODESADDRESSES_LISTNODESNODESADDRESSESTYPE._serialized_end=19146
-  _WAITANYINVOICEREQUEST._serialized_start=19160
-  _WAITANYINVOICEREQUEST._serialized_end=19263
-  _WAITANYINVOICERESPONSE._serialized_start=19266
-  _WAITANYINVOICERESPONSE._serialized_end=19797
-  _WAITANYINVOICERESPONSE_WAITANYINVOICESTATUS._serialized_start=19642
-  _WAITANYINVOICERESPONSE_WAITANYINVOICESTATUS._serialized_end=19687
-  _WAITINVOICEREQUEST._serialized_start=19799
-  _WAITINVOICEREQUEST._serialized_end=19834
-  _WAITINVOICERESPONSE._serialized_start=19837
-  _WAITINVOICERESPONSE._serialized_end=20356
-  _WAITINVOICERESPONSE_WAITINVOICESTATUS._serialized_start=20204
-  _WAITINVOICERESPONSE_WAITINVOICESTATUS._serialized_end=20246
-  _WAITSENDPAYREQUEST._serialized_start=20359
-  _WAITSENDPAYREQUEST._serialized_end=20501
-  _WAITSENDPAYRESPONSE._serialized_start=20504
-  _WAITSENDPAYRESPONSE._serialized_end=21066
-  _WAITSENDPAYRESPONSE_WAITSENDPAYSTATUS._serialized_start=20908
-  _WAITSENDPAYRESPONSE_WAITSENDPAYSTATUS._serialized_end=20941
-  _NEWADDRREQUEST._serialized_start=21069
-  _NEWADDRREQUEST._serialized_end=21210
-  _NEWADDRREQUEST_NEWADDRADDRESSTYPE._serialized_start=21153
-  _NEWADDRREQUEST_NEWADDRADDRESSTYPE._serialized_end=21194
-  _NEWADDRRESPONSE._serialized_start=21212
-  _NEWADDRRESPONSE._serialized_end=21303
-  _WITHDRAWREQUEST._serialized_start=21306
-  _WITHDRAWREQUEST._serialized_end=21508
-  _WITHDRAWRESPONSE._serialized_start=21510
-  _WITHDRAWRESPONSE._serialized_end=21568
-  _KEYSENDREQUEST._serialized_start=21571
-  _KEYSENDREQUEST._serialized_end=21957
-  _KEYSENDRESPONSE._serialized_start=21960
-  _KEYSENDRESPONSE._serialized_end=22330
-  _KEYSENDRESPONSE_KEYSENDSTATUS._serialized_start=22254
-  _KEYSENDRESPONSE_KEYSENDSTATUS._serialized_end=22283
-  _FUNDPSBTREQUEST._serialized_start=22333
-  _FUNDPSBTREQUEST._serialized_end=22649
-  _FUNDPSBTRESPONSE._serialized_start=22652
-  _FUNDPSBTRESPONSE._serialized_end=22869
-  _FUNDPSBTRESERVATIONS._serialized_start=22871
-  _FUNDPSBTRESERVATIONS._serialized_end=22988
-  _SENDPSBTREQUEST._serialized_start=22990
-  _SENDPSBTREQUEST._serialized_end=23055
-  _SENDPSBTRESPONSE._serialized_start=23057
-  _SENDPSBTRESPONSE._serialized_end=23101
-  _SIGNPSBTREQUEST._serialized_start=23103
-  _SIGNPSBTREQUEST._serialized_end=23152
-  _SIGNPSBTRESPONSE._serialized_start=23154
-  _SIGNPSBTRESPONSE._serialized_end=23193
-  _UTXOPSBTREQUEST._serialized_start=23196
-  _UTXOPSBTREQUEST._serialized_end=23543
-  _UTXOPSBTRESPONSE._serialized_start=23546
-  _UTXOPSBTRESPONSE._serialized_end=23763
-  _UTXOPSBTRESERVATIONS._serialized_start=23765
-  _UTXOPSBTRESERVATIONS._serialized_end=23882
-  _TXDISCARDREQUEST._serialized_start=23884
-  _TXDISCARDREQUEST._serialized_end=23916
-  _TXDISCARDRESPONSE._serialized_start=23918
-  _TXDISCARDRESPONSE._serialized_end=23972
-  _TXPREPAREREQUEST._serialized_start=23975
-  _TXPREPAREREQUEST._serialized_end=24139
-  _TXPREPARERESPONSE._serialized_start=24141
-  _TXPREPARERESPONSE._serialized_end=24209
-  _TXSENDREQUEST._serialized_start=24211
-  _TXSENDREQUEST._serialized_end=24240
-  _TXSENDRESPONSE._serialized_start=24242
-  _TXSENDRESPONSE._serialized_end=24298
-  _DISCONNECTREQUEST._serialized_start=24300
-  _DISCONNECTREQUEST._serialized_end=24361
-  _DISCONNECTRESPONSE._serialized_start=24363
-  _DISCONNECTRESPONSE._serialized_end=24383
-  _FEERATESREQUEST._serialized_start=24385
-  _FEERATESREQUEST._serialized_end=24492
-  _FEERATESREQUEST_FEERATESSTYLE._serialized_start=24455
-  _FEERATESREQUEST_FEERATESSTYLE._serialized_end=24492
-  _FEERATESRESPONSE._serialized_start=24495
-  _FEERATESRESPONSE._serialized_end=24779
-  _FEERATESPERKB._serialized_start=24782
-  _FEERATESPERKB._serialized_end=25105
-  _FEERATESPERKW._serialized_start=25108
-  _FEERATESPERKW._serialized_end=25431
-  _FEERATESONCHAIN_FEE_ESTIMATES._serialized_start=25434
-  _FEERATESONCHAIN_FEE_ESTIMATES._serialized_end=25627
-  _FUNDCHANNELREQUEST._serialized_start=25630
-  _FUNDCHANNELREQUEST._serialized_end=26115
-  _FUNDCHANNELRESPONSE._serialized_start=26118
-  _FUNDCHANNELRESPONSE._serialized_end=26273
-  _GETROUTEREQUEST._serialized_start=26276
-  _GETROUTEREQUEST._serialized_end=26512
-  _GETROUTERESPONSE._serialized_start=26514
-  _GETROUTERESPONSE._serialized_end=26567
-  _GETROUTEROUTE._serialized_start=26570
-  _GETROUTEROUTE._serialized_end=26803
-  _GETROUTEROUTE_GETROUTEROUTESTYLE._serialized_start=26761
-  _GETROUTEROUTE_GETROUTEROUTESTYLE._serialized_end=26790
-  _LISTFORWARDSREQUEST._serialized_start=26806
-  _LISTFORWARDSREQUEST._serialized_end=27064
-  _LISTFORWARDSREQUEST_LISTFORWARDSSTATUS._serialized_start=26946
-  _LISTFORWARDSREQUEST_LISTFORWARDSSTATUS._serialized_end=27022
-  _LISTFORWARDSRESPONSE._serialized_start=27066
-  _LISTFORWARDSRESPONSE._serialized_end=27133
-  _LISTFORWARDSFORWARDS._serialized_start=27136
-  _LISTFORWARDSFORWARDS._serialized_end=27742
-  _LISTFORWARDSFORWARDS_LISTFORWARDSFORWARDSSTATUS._serialized_start=27525
-  _LISTFORWARDSFORWARDS_LISTFORWARDSFORWARDSSTATUS._serialized_end=27609
-  _LISTFORWARDSFORWARDS_LISTFORWARDSFORWARDSSTYLE._serialized_start=27611
-  _LISTFORWARDSFORWARDS_LISTFORWARDSFORWARDSSTYLE._serialized_end=27659
-  _LISTPAYSREQUEST._serialized_start=27745
-  _LISTPAYSREQUEST._serialized_end=27964
-  _LISTPAYSREQUEST_LISTPAYSSTATUS._serialized_start=27870
-  _LISTPAYSREQUEST_LISTPAYSSTATUS._serialized_end=27925
-  _LISTPAYSRESPONSE._serialized_start=27966
-  _LISTPAYSRESPONSE._serialized_end=28017
-  _LISTPAYSPAYS._serialized_start=28020
-  _LISTPAYSPAYS._serialized_end=28539
-  _LISTPAYSPAYS_LISTPAYSPAYSSTATUS._serialized_start=28351
-  _LISTPAYSPAYS_LISTPAYSPAYSSTATUS._serialized_end=28410
-  _PINGREQUEST._serialized_start=28541
-  _PINGREQUEST._serialized_end=28630
-  _PINGRESPONSE._serialized_start=28632
-  _PINGRESPONSE._serialized_end=28662
-  _SENDCUSTOMMSGREQUEST._serialized_start=28664
-  _SENDCUSTOMMSGREQUEST._serialized_end=28716
-  _SENDCUSTOMMSGRESPONSE._serialized_start=28718
-  _SENDCUSTOMMSGRESPONSE._serialized_end=28757
-  _SETCHANNELREQUEST._serialized_start=28760
-  _SETCHANNELREQUEST._serialized_end=29008
-  _SETCHANNELRESPONSE._serialized_start=29010
-  _SETCHANNELRESPONSE._serialized_end=29073
-  _SETCHANNELCHANNELS._serialized_start=29076
-  _SETCHANNELCHANNELS._serialized_end=29480
-  _SIGNINVOICEREQUEST._serialized_start=29482
-  _SIGNINVOICEREQUEST._serialized_end=29521
-  _SIGNINVOICERESPONSE._serialized_start=29523
-  _SIGNINVOICERESPONSE._serialized_end=29560
-  _SIGNMESSAGEREQUEST._serialized_start=29562
-  _SIGNMESSAGEREQUEST._serialized_end=29599
-  _SIGNMESSAGERESPONSE._serialized_start=29601
-  _SIGNMESSAGERESPONSE._serialized_end=29671
-  _STOPREQUEST._serialized_start=29673
-  _STOPREQUEST._serialized_end=29686
-  _STOPRESPONSE._serialized_start=29688
-  _STOPRESPONSE._serialized_end=29702
-  _NODE._serialized_start=29705
-  _NODE._serialized_end=32840
+  _GETINFORESPONSE._serialized_end=618
+  _GETINFOOUR_FEATURES._serialized_start=620
+  _GETINFOOUR_FEATURES._serialized_end=703
+  _GETINFOADDRESS._serialized_start=706
+  _GETINFOADDRESS._serialized_end=917
+  _GETINFOADDRESS_GETINFOADDRESSTYPE._serialized_start=819
+  _GETINFOADDRESS_GETINFOADDRESSTYPE._serialized_end=905
+  _GETINFOBINDING._serialized_start=920
+  _GETINFOBINDING._serialized_end=1171
+  _GETINFOBINDING_GETINFOBINDINGTYPE._serialized_start=1059
+  _GETINFOBINDING_GETINFOBINDINGTYPE._serialized_end=1139
+  _LISTPEERSREQUEST._serialized_start=1173
+  _LISTPEERSREQUEST._serialized_end=1245
+  _LISTPEERSRESPONSE._serialized_start=1247
+  _LISTPEERSRESPONSE._serialized_end=1302
+  _LISTPEERSPEERS._serialized_start=1305
+  _LISTPEERSPEERS._serialized_end=1575
+  _LISTPEERSPEERSLOG._serialized_start=1578
+  _LISTPEERSPEERSLOG._serialized_end=1959
+  _LISTPEERSPEERSLOG_LISTPEERSPEERSLOGTYPE._serialized_start=1789
+  _LISTPEERSPEERSLOG_LISTPEERSPEERSLOGTYPE._serialized_end=1894
+  _LISTPEERSPEERSCHANNELS._serialized_start=1962
+  _LISTPEERSPEERSCHANNELS._serialized_end=4992
+  _LISTPEERSPEERSCHANNELS_LISTPEERSPEERSCHANNELSSTATE._serialized_start=3862
+  _LISTPEERSPEERSCHANNELS_LISTPEERSPEERSCHANNELSSTATE._serialized_end=4151
+  _LISTPEERSPEERSCHANNELSFEERATE._serialized_start=4994
+  _LISTPEERSPEERSCHANNELSFEERATE._serialized_end=5055
+  _LISTPEERSPEERSCHANNELSINFLIGHT._serialized_start=5058
+  _LISTPEERSPEERSCHANNELSINFLIGHT._serialized_end=5255
+  _LISTPEERSPEERSCHANNELSFUNDING._serialized_start=5258
+  _LISTPEERSPEERSCHANNELSFUNDING._serialized_end=5541
+  _LISTPEERSPEERSCHANNELSALIAS._serialized_start=5543
+  _LISTPEERSPEERSCHANNELSALIAS._serialized_end=5634
+  _LISTPEERSPEERSCHANNELSHTLCS._serialized_start=5637
+  _LISTPEERSPEERSCHANNELSHTLCS._serialized_end=6006
+  _LISTPEERSPEERSCHANNELSHTLCS_LISTPEERSPEERSCHANNELSHTLCSDIRECTION._serialized_start=5922
+  _LISTPEERSPEERSCHANNELSHTLCS_LISTPEERSPEERSCHANNELSHTLCSDIRECTION._serialized_end=5977
+  _LISTFUNDSREQUEST._serialized_start=6008
+  _LISTFUNDSREQUEST._serialized_end=6056
+  _LISTFUNDSRESPONSE._serialized_start=6058
+  _LISTFUNDSRESPONSE._serialized_end=6159
+  _LISTFUNDSOUTPUTS._serialized_start=6162
+  _LISTFUNDSOUTPUTS._serialized_end=6549
+  _LISTFUNDSOUTPUTS_LISTFUNDSOUTPUTSSTATUS._serialized_start=6423
+  _LISTFUNDSOUTPUTS_LISTFUNDSOUTPUTSSTATUS._serialized_end=6504
+  _LISTFUNDSCHANNELS._serialized_start=6552
+  _LISTFUNDSCHANNELS._serialized_end=6851
+  _SENDPAYREQUEST._serialized_start=6854
+  _SENDPAYREQUEST._serialized_end=7203
+  _SENDPAYRESPONSE._serialized_start=7206
+  _SENDPAYRESPONSE._serialized_end=7799
+  _SENDPAYRESPONSE_SENDPAYSTATUS._serialized_start=7620
+  _SENDPAYRESPONSE_SENDPAYSTATUS._serialized_end=7662
+  _SENDPAYROUTE._serialized_start=7801
+  _SENDPAYROUTE._serialized_end=7893
+  _LISTCHANNELSREQUEST._serialized_start=7896
+  _LISTCHANNELSREQUEST._serialized_end=8043
+  _LISTCHANNELSRESPONSE._serialized_start=8045
+  _LISTCHANNELSRESPONSE._serialized_end=8112
+  _LISTCHANNELSCHANNELS._serialized_start=8115
+  _LISTCHANNELSCHANNELS._serialized_end=8550
+  _ADDGOSSIPREQUEST._serialized_start=8552
+  _ADDGOSSIPREQUEST._serialized_end=8587
+  _ADDGOSSIPRESPONSE._serialized_start=8589
+  _ADDGOSSIPRESPONSE._serialized_end=8608
+  _AUTOCLEANINVOICEREQUEST._serialized_start=8610
+  _AUTOCLEANINVOICEREQUEST._serialized_end=8721
+  _AUTOCLEANINVOICERESPONSE._serialized_start=8724
+  _AUTOCLEANINVOICERESPONSE._serialized_end=8853
+  _CHECKMESSAGEREQUEST._serialized_start=8855
+  _CHECKMESSAGEREQUEST._serialized_end=8940
+  _CHECKMESSAGERESPONSE._serialized_start=8942
+  _CHECKMESSAGERESPONSE._serialized_end=8998
+  _CLOSEREQUEST._serialized_start=9001
+  _CLOSEREQUEST._serialized_end=9332
+  _CLOSERESPONSE._serialized_start=9335
+  _CLOSERESPONSE._serialized_end=9506
+  _CLOSERESPONSE_CLOSETYPE._serialized_start=9437
+  _CLOSERESPONSE_CLOSETYPE._serialized_end=9490
+  _CONNECTREQUEST._serialized_start=9508
+  _CONNECTREQUEST._serialized_end=9592
+  _CONNECTRESPONSE._serialized_start=9595
+  _CONNECTRESPONSE._serialized_end=9775
+  _CONNECTRESPONSE_CONNECTDIRECTION._serialized_start=9740
+  _CONNECTRESPONSE_CONNECTDIRECTION._serialized_end=9775
+  _CONNECTADDRESS._serialized_start=9778
+  _CONNECTADDRESS._serialized_end=10029
+  _CONNECTADDRESS_CONNECTADDRESSTYPE._serialized_start=9917
+  _CONNECTADDRESS_CONNECTADDRESSTYPE._serialized_end=9997
+  _CREATEINVOICEREQUEST._serialized_start=10031
+  _CREATEINVOICEREQUEST._serialized_end=10105
+  _CREATEINVOICERESPONSE._serialized_start=10108
+  _CREATEINVOICERESPONSE._serialized_end=10749
+  _CREATEINVOICERESPONSE_CREATEINVOICESTATUS._serialized_start=10542
+  _CREATEINVOICERESPONSE_CREATEINVOICESTATUS._serialized_end=10598
+  _DATASTOREREQUEST._serialized_start=10752
+  _DATASTOREREQUEST._serialized_end=11060
+  _DATASTOREREQUEST_DATASTOREMODE._serialized_start=10905
+  _DATASTOREREQUEST_DATASTOREMODE._serialized_end=11017
+  _DATASTORERESPONSE._serialized_start=11063
+  _DATASTORERESPONSE._serialized_end=11193
+  _CREATEONIONREQUEST._serialized_start=11196
+  _CREATEONIONREQUEST._serialized_end=11353
+  _CREATEONIONRESPONSE._serialized_start=11355
+  _CREATEONIONRESPONSE._serialized_end=11415
+  _CREATEONIONHOPS._serialized_start=11417
+  _CREATEONIONHOPS._serialized_end=11467
+  _DELDATASTOREREQUEST._serialized_start=11469
+  _DELDATASTOREREQUEST._serialized_end=11543
+  _DELDATASTORERESPONSE._serialized_start=11546
+  _DELDATASTORERESPONSE._serialized_end=11679
+  _DELEXPIREDINVOICEREQUEST._serialized_start=11681
+  _DELEXPIREDINVOICEREQUEST._serialized_end=11753
+  _DELEXPIREDINVOICERESPONSE._serialized_start=11755
+  _DELEXPIREDINVOICERESPONSE._serialized_end=11782
+  _DELINVOICEREQUEST._serialized_start=11785
+  _DELINVOICEREQUEST._serialized_end=11967
+  _DELINVOICEREQUEST_DELINVOICESTATUS._serialized_start=11901
+  _DELINVOICEREQUEST_DELINVOICESTATUS._serialized_end=11954
+  _DELINVOICERESPONSE._serialized_start=11970
+  _DELINVOICERESPONSE._serialized_end=12423
+  _DELINVOICERESPONSE_DELINVOICESTATUS._serialized_start=11901
+  _DELINVOICERESPONSE_DELINVOICESTATUS._serialized_end=11954
+  _INVOICEREQUEST._serialized_start=12426
+  _INVOICEREQUEST._serialized_end=12676
+  _INVOICERESPONSE._serialized_start=12679
+  _INVOICERESPONSE._serialized_end=13038
+  _LISTDATASTOREREQUEST._serialized_start=13040
+  _LISTDATASTOREREQUEST._serialized_end=13075
+  _LISTDATASTORERESPONSE._serialized_start=13077
+  _LISTDATASTORERESPONSE._serialized_end=13148
+  _LISTDATASTOREDATASTORE._serialized_start=13151
+  _LISTDATASTOREDATASTORE._serialized_end=13286
+  _LISTINVOICESREQUEST._serialized_start=13289
+  _LISTINVOICESREQUEST._serialized_end=13458
+  _LISTINVOICESRESPONSE._serialized_start=13460
+  _LISTINVOICESRESPONSE._serialized_end=13527
+  _LISTINVOICESINVOICES._serialized_start=13530
+  _LISTINVOICESINVOICES._serialized_end=14204
+  _LISTINVOICESINVOICES_LISTINVOICESINVOICESSTATUS._serialized_start=13974
+  _LISTINVOICESINVOICES_LISTINVOICESINVOICESSTATUS._serialized_end=14037
+  _SENDONIONREQUEST._serialized_start=14207
+  _SENDONIONREQUEST._serialized_end=14601
+  _SENDONIONRESPONSE._serialized_start=14604
+  _SENDONIONRESPONSE._serialized_end=15127
+  _SENDONIONRESPONSE_SENDONIONSTATUS._serialized_start=14975
+  _SENDONIONRESPONSE_SENDONIONSTATUS._serialized_end=15019
+  _SENDONIONFIRST_HOP._serialized_start=15129
+  _SENDONIONFIRST_HOP._serialized_end=15210
+  _LISTSENDPAYSREQUEST._serialized_start=15213
+  _LISTSENDPAYSREQUEST._serialized_end=15448
+  _LISTSENDPAYSREQUEST_LISTSENDPAYSSTATUS._serialized_start=15350
+  _LISTSENDPAYSREQUEST_LISTSENDPAYSSTATUS._serialized_end=15409
+  _LISTSENDPAYSRESPONSE._serialized_start=15450
+  _LISTSENDPAYSRESPONSE._serialized_end=15517
+  _LISTSENDPAYSPAYMENTS._serialized_start=15520
+  _LISTSENDPAYSPAYMENTS._serialized_end=16148
+  _LISTSENDPAYSPAYMENTS_LISTSENDPAYSPAYMENTSSTATUS._serialized_start=15954
+  _LISTSENDPAYSPAYMENTS_LISTSENDPAYSPAYMENTSSTATUS._serialized_end=16021
+  _LISTTRANSACTIONSREQUEST._serialized_start=16150
+  _LISTTRANSACTIONSREQUEST._serialized_end=16175
+  _LISTTRANSACTIONSRESPONSE._serialized_start=16177
+  _LISTTRANSACTIONSRESPONSE._serialized_end=16260
+  _LISTTRANSACTIONSTRANSACTIONS._serialized_start=16263
+  _LISTTRANSACTIONSTRANSACTIONS._serialized_end=16511
+  _LISTTRANSACTIONSTRANSACTIONSINPUTS._serialized_start=16514
+  _LISTTRANSACTIONSTRANSACTIONSINPUTS._serialized_end=17030
+  _LISTTRANSACTIONSTRANSACTIONSINPUTS_LISTTRANSACTIONSTRANSACTIONSINPUTSTYPE._serialized_start=16726
+  _LISTTRANSACTIONSTRANSACTIONSINPUTS_LISTTRANSACTIONSTRANSACTIONSINPUTSTYPE._serialized_end=17004
+  _LISTTRANSACTIONSTRANSACTIONSOUTPUTS._serialized_start=17033
+  _LISTTRANSACTIONSTRANSACTIONSOUTPUTS._serialized_end=17577
+  _LISTTRANSACTIONSTRANSACTIONSOUTPUTS_LISTTRANSACTIONSTRANSACTIONSOUTPUTSTYPE._serialized_start=17272
+  _LISTTRANSACTIONSTRANSACTIONSOUTPUTS_LISTTRANSACTIONSTRANSACTIONSOUTPUTSTYPE._serialized_end=17551
+  _PAYREQUEST._serialized_start=17580
+  _PAYREQUEST._serialized_end=18054
+  _PAYRESPONSE._serialized_start=18057
+  _PAYRESPONSE._serialized_end=18436
+  _PAYRESPONSE_PAYSTATUS._serialized_start=18339
+  _PAYRESPONSE_PAYSTATUS._serialized_end=18389
+  _LISTNODESREQUEST._serialized_start=18438
+  _LISTNODESREQUEST._serialized_end=18480
+  _LISTNODESRESPONSE._serialized_start=18482
+  _LISTNODESRESPONSE._serialized_end=18537
+  _LISTNODESNODES._serialized_start=18540
+  _LISTNODESNODES._serialized_end=18765
+  _LISTNODESNODESADDRESSES._serialized_start=18768
+  _LISTNODESNODESADDRESSES._serialized_end=19015
+  _LISTNODESNODESADDRESSES_LISTNODESNODESADDRESSESTYPE._serialized_start=18908
+  _LISTNODESNODESADDRESSES_LISTNODESNODESADDRESSESTYPE._serialized_end=19003
+  _WAITANYINVOICEREQUEST._serialized_start=19017
+  _WAITANYINVOICEREQUEST._serialized_end=19120
+  _WAITANYINVOICERESPONSE._serialized_start=19123
+  _WAITANYINVOICERESPONSE._serialized_end=19654
+  _WAITANYINVOICERESPONSE_WAITANYINVOICESTATUS._serialized_start=19499
+  _WAITANYINVOICERESPONSE_WAITANYINVOICESTATUS._serialized_end=19544
+  _WAITINVOICEREQUEST._serialized_start=19656
+  _WAITINVOICEREQUEST._serialized_end=19691
+  _WAITINVOICERESPONSE._serialized_start=19694
+  _WAITINVOICERESPONSE._serialized_end=20213
+  _WAITINVOICERESPONSE_WAITINVOICESTATUS._serialized_start=20061
+  _WAITINVOICERESPONSE_WAITINVOICESTATUS._serialized_end=20103
+  _WAITSENDPAYREQUEST._serialized_start=20216
+  _WAITSENDPAYREQUEST._serialized_end=20358
+  _WAITSENDPAYRESPONSE._serialized_start=20361
+  _WAITSENDPAYRESPONSE._serialized_end=20923
+  _WAITSENDPAYRESPONSE_WAITSENDPAYSTATUS._serialized_start=20765
+  _WAITSENDPAYRESPONSE_WAITSENDPAYSTATUS._serialized_end=20798
+  _NEWADDRREQUEST._serialized_start=20926
+  _NEWADDRREQUEST._serialized_end=21067
+  _NEWADDRREQUEST_NEWADDRADDRESSTYPE._serialized_start=21010
+  _NEWADDRREQUEST_NEWADDRADDRESSTYPE._serialized_end=21051
+  _NEWADDRRESPONSE._serialized_start=21069
+  _NEWADDRRESPONSE._serialized_end=21160
+  _WITHDRAWREQUEST._serialized_start=21163
+  _WITHDRAWREQUEST._serialized_end=21365
+  _WITHDRAWRESPONSE._serialized_start=21367
+  _WITHDRAWRESPONSE._serialized_end=21425
+  _KEYSENDREQUEST._serialized_start=21428
+  _KEYSENDREQUEST._serialized_end=21814
+  _KEYSENDRESPONSE._serialized_start=21817
+  _KEYSENDRESPONSE._serialized_end=22187
+  _KEYSENDRESPONSE_KEYSENDSTATUS._serialized_start=22111
+  _KEYSENDRESPONSE_KEYSENDSTATUS._serialized_end=22140
+  _FUNDPSBTREQUEST._serialized_start=22190
+  _FUNDPSBTREQUEST._serialized_end=22506
+  _FUNDPSBTRESPONSE._serialized_start=22509
+  _FUNDPSBTRESPONSE._serialized_end=22726
+  _FUNDPSBTRESERVATIONS._serialized_start=22728
+  _FUNDPSBTRESERVATIONS._serialized_end=22845
+  _SENDPSBTREQUEST._serialized_start=22847
+  _SENDPSBTREQUEST._serialized_end=22912
+  _SENDPSBTRESPONSE._serialized_start=22914
+  _SENDPSBTRESPONSE._serialized_end=22958
+  _SIGNPSBTREQUEST._serialized_start=22960
+  _SIGNPSBTREQUEST._serialized_end=23009
+  _SIGNPSBTRESPONSE._serialized_start=23011
+  _SIGNPSBTRESPONSE._serialized_end=23050
+  _UTXOPSBTREQUEST._serialized_start=23053
+  _UTXOPSBTREQUEST._serialized_end=23400
+  _UTXOPSBTRESPONSE._serialized_start=23403
+  _UTXOPSBTRESPONSE._serialized_end=23620
+  _UTXOPSBTRESERVATIONS._serialized_start=23622
+  _UTXOPSBTRESERVATIONS._serialized_end=23739
+  _TXDISCARDREQUEST._serialized_start=23741
+  _TXDISCARDREQUEST._serialized_end=23773
+  _TXDISCARDRESPONSE._serialized_start=23775
+  _TXDISCARDRESPONSE._serialized_end=23829
+  _TXPREPAREREQUEST._serialized_start=23832
+  _TXPREPAREREQUEST._serialized_end=23996
+  _TXPREPARERESPONSE._serialized_start=23998
+  _TXPREPARERESPONSE._serialized_end=24066
+  _TXSENDREQUEST._serialized_start=24068
+  _TXSENDREQUEST._serialized_end=24097
+  _TXSENDRESPONSE._serialized_start=24099
+  _TXSENDRESPONSE._serialized_end=24155
+  _LISTPEERCHANNELSREQUEST._serialized_start=24157
+  _LISTPEERCHANNELSREQUEST._serialized_end=24206
+  _LISTPEERCHANNELSRESPONSE._serialized_start=24208
+  _LISTPEERCHANNELSRESPONSE._serialized_end=24283
+  _LISTPEERCHANNELSCHANNELS._serialized_start=24286
+  _LISTPEERCHANNELSCHANNELS._serialized_end=27429
+  _LISTPEERCHANNELSCHANNELS_LISTPEERCHANNELSCHANNELSSTATE._serialized_start=26245
+  _LISTPEERCHANNELSCHANNELS_LISTPEERCHANNELSCHANNELSSTATE._serialized_end=26536
+  _LISTPEERCHANNELSCHANNELSFEERATE._serialized_start=27431
+  _LISTPEERCHANNELSCHANNELSFEERATE._serialized_end=27524
+  _LISTPEERCHANNELSCHANNELSINFLIGHT._serialized_start=27527
+  _LISTPEERCHANNELSCHANNELSINFLIGHT._serialized_end=27865
+  _LISTPEERCHANNELSCHANNELSFUNDING._serialized_start=27868
+  _LISTPEERCHANNELSCHANNELSFUNDING._serialized_end=28206
+  _LISTPEERCHANNELSCHANNELSALIAS._serialized_start=28208
+  _LISTPEERCHANNELSCHANNELSALIAS._serialized_end=28301
+  _LISTPEERCHANNELSCHANNELSHTLCS._serialized_start=28304
+  _LISTPEERCHANNELSCHANNELSHTLCS._serialized_end=28786
+  _LISTPEERCHANNELSCHANNELSHTLCS_LISTPEERCHANNELSCHANNELSHTLCSDIRECTION._serialized_start=28625
+  _LISTPEERCHANNELSCHANNELSHTLCS_LISTPEERCHANNELSCHANNELSHTLCSDIRECTION._serialized_end=28682
+  _LISTCLOSEDCHANNELSREQUEST._serialized_start=28788
+  _LISTCLOSEDCHANNELSREQUEST._serialized_end=28839
+  _LISTCLOSEDCHANNELSRESPONSE._serialized_start=28841
+  _LISTCLOSEDCHANNELSRESPONSE._serialized_end=28932
+  _LISTCLOSEDCHANNELSCLOSEDCHANNELS._serialized_start=28935
+  _LISTCLOSEDCHANNELSCLOSEDCHANNELS._serialized_end=30137
+  _LISTCLOSEDCHANNELSCLOSEDCHANNELS_LISTCLOSEDCHANNELSCLOSEDCHANNELSCLOSE_CAUSE._serialized_start=29835
+  _LISTCLOSEDCHANNELSCLOSEDCHANNELS_LISTCLOSEDCHANNELSCLOSEDCHANNELSCLOSE_CAUSE._serialized_end=29953
+  _LISTCLOSEDCHANNELSCLOSEDCHANNELSALIAS._serialized_start=30139
+  _LISTCLOSEDCHANNELSCLOSEDCHANNELSALIAS._serialized_end=30240
+  _DECODEPAYREQUEST._serialized_start=30242
+  _DECODEPAYREQUEST._serialized_end=30318
+  _DECODEPAYRESPONSE._serialized_start=30321
+  _DECODEPAYRESPONSE._serialized_end=30846
+  _DECODEPAYFALLBACKS._serialized_start=30849
+  _DECODEPAYFALLBACKS._serialized_end=31047
+  _DECODEPAYFALLBACKS_DECODEPAYFALLBACKSTYPE._serialized_start=30970
+  _DECODEPAYFALLBACKS_DECODEPAYFALLBACKSTYPE._serialized_end=31038
+  _DECODEPAYEXTRA._serialized_start=31049
+  _DECODEPAYEXTRA._serialized_end=31092
+  _DECODEREQUEST._serialized_start=31094
+  _DECODEREQUEST._serialized_end=31125
+  _DECODERESPONSE._serialized_start=31128
+  _DECODERESPONSE._serialized_end=35394
+  _DECODERESPONSE_DECODETYPE._serialized_start=33696
+  _DECODERESPONSE_DECODETYPE._serialized_end=33804
+  _DECODEOFFER_PATHS._serialized_start=35396
+  _DECODEOFFER_PATHS._serialized_end=35456
+  _DECODEOFFER_RECURRENCEPAYWINDOW._serialized_start=35459
+  _DECODEOFFER_RECURRENCEPAYWINDOW._serialized_end=35597
+  _DECODEINVOICE_PATHSPATH._serialized_start=35599
+  _DECODEINVOICE_PATHSPATH._serialized_end=35683
+  _DECODEINVOICE_FALLBACKS._serialized_start=35685
+  _DECODEINVOICE_FALLBACKS._serialized_end=35774
+  _DECODEFALLBACKS._serialized_start=35776
+  _DECODEFALLBACKS._serialized_end=35895
+  _DECODEEXTRA._serialized_start=35897
+  _DECODEEXTRA._serialized_end=35937
+  _DECODERESTRICTIONS._serialized_start=35939
+  _DECODERESTRICTIONS._serialized_end=35998
+  _DISCONNECTREQUEST._serialized_start=36000
+  _DISCONNECTREQUEST._serialized_end=36061
+  _DISCONNECTRESPONSE._serialized_start=36063
+  _DISCONNECTRESPONSE._serialized_end=36083
+  _FEERATESREQUEST._serialized_start=36085
+  _FEERATESREQUEST._serialized_end=36192
+  _FEERATESREQUEST_FEERATESSTYLE._serialized_start=36155
+  _FEERATESREQUEST_FEERATESSTYLE._serialized_end=36192
+  _FEERATESRESPONSE._serialized_start=36195
+  _FEERATESRESPONSE._serialized_end=36479
+  _FEERATESPERKB._serialized_start=36482
+  _FEERATESPERKB._serialized_end=36883
+  _FEERATESPERKBESTIMATES._serialized_start=36886
+  _FEERATESPERKBESTIMATES._serialized_end=37036
+  _FEERATESPERKW._serialized_start=37039
+  _FEERATESPERKW._serialized_end=37440
+  _FEERATESPERKWESTIMATES._serialized_start=37443
+  _FEERATESPERKWESTIMATES._serialized_end=37593
+  _FEERATESONCHAIN_FEE_ESTIMATES._serialized_start=37596
+  _FEERATESONCHAIN_FEE_ESTIMATES._serialized_end=37789
+  _FUNDCHANNELREQUEST._serialized_start=37792
+  _FUNDCHANNELREQUEST._serialized_end=38277
+  _FUNDCHANNELRESPONSE._serialized_start=38280
+  _FUNDCHANNELRESPONSE._serialized_end=38435
+  _GETROUTEREQUEST._serialized_start=38438
+  _GETROUTEREQUEST._serialized_end=38674
+  _GETROUTERESPONSE._serialized_start=38676
+  _GETROUTERESPONSE._serialized_end=38729
+  _GETROUTEROUTE._serialized_start=38732
+  _GETROUTEROUTE._serialized_end=38929
+  _GETROUTEROUTE_GETROUTEROUTESTYLE._serialized_start=38900
+  _GETROUTEROUTE_GETROUTEROUTESTYLE._serialized_end=38929
+  _LISTFORWARDSREQUEST._serialized_start=38932
+  _LISTFORWARDSREQUEST._serialized_end=39190
+  _LISTFORWARDSREQUEST_LISTFORWARDSSTATUS._serialized_start=39072
+  _LISTFORWARDSREQUEST_LISTFORWARDSSTATUS._serialized_end=39148
+  _LISTFORWARDSRESPONSE._serialized_start=39192
+  _LISTFORWARDSRESPONSE._serialized_end=39259
+  _LISTFORWARDSFORWARDS._serialized_start=39262
+  _LISTFORWARDSFORWARDS._serialized_end=39868
+  _LISTFORWARDSFORWARDS_LISTFORWARDSFORWARDSSTATUS._serialized_start=39651
+  _LISTFORWARDSFORWARDS_LISTFORWARDSFORWARDSSTATUS._serialized_end=39735
+  _LISTFORWARDSFORWARDS_LISTFORWARDSFORWARDSSTYLE._serialized_start=39737
+  _LISTFORWARDSFORWARDS_LISTFORWARDSFORWARDSSTYLE._serialized_end=39785
+  _LISTPAYSREQUEST._serialized_start=39871
+  _LISTPAYSREQUEST._serialized_end=40090
+  _LISTPAYSREQUEST_LISTPAYSSTATUS._serialized_start=39996
+  _LISTPAYSREQUEST_LISTPAYSSTATUS._serialized_end=40051
+  _LISTPAYSRESPONSE._serialized_start=40092
+  _LISTPAYSRESPONSE._serialized_end=40143
+  _LISTPAYSPAYS._serialized_start=40146
+  _LISTPAYSPAYS._serialized_end=40665
+  _LISTPAYSPAYS_LISTPAYSPAYSSTATUS._serialized_start=40477
+  _LISTPAYSPAYS_LISTPAYSPAYSSTATUS._serialized_end=40536
+  _PINGREQUEST._serialized_start=40667
+  _PINGREQUEST._serialized_end=40756
+  _PINGRESPONSE._serialized_start=40758
+  _PINGRESPONSE._serialized_end=40788
+  _SENDCUSTOMMSGREQUEST._serialized_start=40790
+  _SENDCUSTOMMSGREQUEST._serialized_end=40842
+  _SENDCUSTOMMSGRESPONSE._serialized_start=40844
+  _SENDCUSTOMMSGRESPONSE._serialized_end=40883
+  _SETCHANNELREQUEST._serialized_start=40886
+  _SETCHANNELREQUEST._serialized_end=41134
+  _SETCHANNELRESPONSE._serialized_start=41136
+  _SETCHANNELRESPONSE._serialized_end=41199
+  _SETCHANNELCHANNELS._serialized_start=41202
+  _SETCHANNELCHANNELS._serialized_end=41606
+  _SIGNINVOICEREQUEST._serialized_start=41608
+  _SIGNINVOICEREQUEST._serialized_end=41647
+  _SIGNINVOICERESPONSE._serialized_start=41649
+  _SIGNINVOICERESPONSE._serialized_end=41686
+  _SIGNMESSAGEREQUEST._serialized_start=41688
+  _SIGNMESSAGEREQUEST._serialized_end=41725
+  _SIGNMESSAGERESPONSE._serialized_start=41727
+  _SIGNMESSAGERESPONSE._serialized_end=41797
+  _STOPREQUEST._serialized_start=41799
+  _STOPREQUEST._serialized_end=41812
+  _STOPRESPONSE._serialized_start=41814
+  _STOPRESPONSE._serialized_end=41828
+  _NODE._serialized_start=41831
+  _NODE._serialized_end=45253
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyln_testing-23.2/pyln/testing/node_pb2_grpc.py` & `pyln-testing-23.5/pyln/testing/node_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,34 @@
                 response_deserializer=node__pb2.TxprepareResponse.FromString,
                 )
         self.TxSend = channel.unary_unary(
                 '/cln.Node/TxSend',
                 request_serializer=node__pb2.TxsendRequest.SerializeToString,
                 response_deserializer=node__pb2.TxsendResponse.FromString,
                 )
+        self.ListPeerChannels = channel.unary_unary(
+                '/cln.Node/ListPeerChannels',
+                request_serializer=node__pb2.ListpeerchannelsRequest.SerializeToString,
+                response_deserializer=node__pb2.ListpeerchannelsResponse.FromString,
+                )
+        self.ListClosedChannels = channel.unary_unary(
+                '/cln.Node/ListClosedChannels',
+                request_serializer=node__pb2.ListclosedchannelsRequest.SerializeToString,
+                response_deserializer=node__pb2.ListclosedchannelsResponse.FromString,
+                )
+        self.DecodePay = channel.unary_unary(
+                '/cln.Node/DecodePay',
+                request_serializer=node__pb2.DecodepayRequest.SerializeToString,
+                response_deserializer=node__pb2.DecodepayResponse.FromString,
+                )
+        self.Decode = channel.unary_unary(
+                '/cln.Node/Decode',
+                request_serializer=node__pb2.DecodeRequest.SerializeToString,
+                response_deserializer=node__pb2.DecodeResponse.FromString,
+                )
         self.Disconnect = channel.unary_unary(
                 '/cln.Node/Disconnect',
                 request_serializer=node__pb2.DisconnectRequest.SerializeToString,
                 response_deserializer=node__pb2.DisconnectResponse.FromString,
                 )
         self.Feerates = channel.unary_unary(
                 '/cln.Node/Feerates',
@@ -482,14 +502,38 @@
 
     def TxSend(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ListPeerChannels(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ListClosedChannels(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DecodePay(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Decode(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def Disconnect(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Feerates(self, request, context):
@@ -742,14 +786,34 @@
                     response_serializer=node__pb2.TxprepareResponse.SerializeToString,
             ),
             'TxSend': grpc.unary_unary_rpc_method_handler(
                     servicer.TxSend,
                     request_deserializer=node__pb2.TxsendRequest.FromString,
                     response_serializer=node__pb2.TxsendResponse.SerializeToString,
             ),
+            'ListPeerChannels': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListPeerChannels,
+                    request_deserializer=node__pb2.ListpeerchannelsRequest.FromString,
+                    response_serializer=node__pb2.ListpeerchannelsResponse.SerializeToString,
+            ),
+            'ListClosedChannels': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListClosedChannels,
+                    request_deserializer=node__pb2.ListclosedchannelsRequest.FromString,
+                    response_serializer=node__pb2.ListclosedchannelsResponse.SerializeToString,
+            ),
+            'DecodePay': grpc.unary_unary_rpc_method_handler(
+                    servicer.DecodePay,
+                    request_deserializer=node__pb2.DecodepayRequest.FromString,
+                    response_serializer=node__pb2.DecodepayResponse.SerializeToString,
+            ),
+            'Decode': grpc.unary_unary_rpc_method_handler(
+                    servicer.Decode,
+                    request_deserializer=node__pb2.DecodeRequest.FromString,
+                    response_serializer=node__pb2.DecodeResponse.SerializeToString,
+            ),
             'Disconnect': grpc.unary_unary_rpc_method_handler(
                     servicer.Disconnect,
                     request_deserializer=node__pb2.DisconnectRequest.FromString,
                     response_serializer=node__pb2.DisconnectResponse.SerializeToString,
             ),
             'Feerates': grpc.unary_unary_rpc_method_handler(
                     servicer.Feerates,
@@ -1442,14 +1506,82 @@
         return grpc.experimental.unary_unary(request, target, '/cln.Node/TxSend',
             node__pb2.TxsendRequest.SerializeToString,
             node__pb2.TxsendResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def ListPeerChannels(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/cln.Node/ListPeerChannels',
+            node__pb2.ListpeerchannelsRequest.SerializeToString,
+            node__pb2.ListpeerchannelsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListClosedChannels(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/cln.Node/ListClosedChannels',
+            node__pb2.ListclosedchannelsRequest.SerializeToString,
+            node__pb2.ListclosedchannelsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DecodePay(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/cln.Node/DecodePay',
+            node__pb2.DecodepayRequest.SerializeToString,
+            node__pb2.DecodepayResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Decode(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/cln.Node/Decode',
+            node__pb2.DecodeRequest.SerializeToString,
+            node__pb2.DecodeResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def Disconnect(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `pyln_testing-23.2/pyln/testing/primitives_pb2.py` & `pyln-testing-23.5/pyln/testing/primitives_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,33 +11,46 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10primitives.proto\x12\x03\x63ln\"\x16\n\x06\x41mount\x12\x0c\n\x04msat\x18\x01 \x01(\x04\"D\n\x0b\x41mountOrAll\x12\x1d\n\x06\x61mount\x18\x01 \x01(\x0b\x32\x0b.cln.AmountH\x00\x12\r\n\x03\x61ll\x18\x02 \x01(\x08H\x00\x42\x07\n\x05value\"D\n\x0b\x41mountOrAny\x12\x1d\n\x06\x61mount\x18\x01 \x01(\x0b\x32\x0b.cln.AmountH\x00\x12\r\n\x03\x61ny\x18\x02 \x01(\x08H\x00\x42\x07\n\x05value\"\x19\n\x17\x43hannelStateChangeCause\"(\n\x08Outpoint\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\x12\x0e\n\x06outnum\x18\x02 \x01(\r\"h\n\x07\x46\x65\x65rate\x12\x0e\n\x04slow\x18\x01 \x01(\x08H\x00\x12\x10\n\x06normal\x18\x02 \x01(\x08H\x00\x12\x10\n\x06urgent\x18\x03 \x01(\x08H\x00\x12\x0f\n\x05perkb\x18\x04 \x01(\rH\x00\x12\x0f\n\x05perkw\x18\x05 \x01(\rH\x00\x42\x07\n\x05style\":\n\nOutputDesc\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x1b\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x0b.cln.Amount\"t\n\x08RouteHop\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x18\n\x10short_channel_id\x18\x02 \x01(\t\x12\x1c\n\x07\x66\x65\x65\x62\x61se\x18\x03 \x01(\x0b\x32\x0b.cln.Amount\x12\x0f\n\x07\x66\x65\x65prop\x18\x04 \x01(\r\x12\x13\n\x0b\x65xpirydelta\x18\x05 \x01(\r\"(\n\tRoutehint\x12\x1b\n\x04hops\x18\x01 \x03(\x0b\x32\r.cln.RouteHop\".\n\rRoutehintList\x12\x1d\n\x05hints\x18\x02 \x03(\x0b\x32\x0e.cln.Routehint\"\'\n\x08TlvEntry\x12\x0c\n\x04type\x18\x01 \x01(\x04\x12\r\n\x05value\x18\x02 \x01(\x0c\"+\n\tTlvStream\x12\x1e\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\r.cln.TlvEntry*\x1e\n\x0b\x43hannelSide\x12\x06\n\x02IN\x10\x00\x12\x07\n\x03OUT\x10\x01*\x84\x02\n\x0c\x43hannelState\x12\x0c\n\x08Openingd\x10\x00\x12\x1a\n\x16\x43hanneldAwaitingLockin\x10\x01\x12\x12\n\x0e\x43hanneldNormal\x10\x02\x12\x18\n\x14\x43hanneldShuttingDown\x10\x03\x12\x17\n\x13\x43losingdSigexchange\x10\x04\x12\x14\n\x10\x43losingdComplete\x10\x05\x12\x16\n\x12\x41waitingUnilateral\x10\x06\x12\x14\n\x10\x46undingSpendSeen\x10\x07\x12\x0b\n\x07Onchain\x10\x08\x12\x15\n\x11\x44ualopendOpenInit\x10\t\x12\x1b\n\x17\x44ualopendAwaitingLockin\x10\nb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10primitives.proto\x12\x03\x63ln\"\x16\n\x06\x41mount\x12\x0c\n\x04msat\x18\x01 \x01(\x04\"D\n\x0b\x41mountOrAll\x12\x1d\n\x06\x61mount\x18\x01 \x01(\x0b\x32\x0b.cln.AmountH\x00\x12\r\n\x03\x61ll\x18\x02 \x01(\x08H\x00\x42\x07\n\x05value\"D\n\x0b\x41mountOrAny\x12\x1d\n\x06\x61mount\x18\x01 \x01(\x0b\x32\x0b.cln.AmountH\x00\x12\r\n\x03\x61ny\x18\x02 \x01(\x08H\x00\x42\x07\n\x05value\"\x19\n\x17\x43hannelStateChangeCause\"(\n\x08Outpoint\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\x12\x0e\n\x06outnum\x18\x02 \x01(\r\"h\n\x07\x46\x65\x65rate\x12\x0e\n\x04slow\x18\x01 \x01(\x08H\x00\x12\x10\n\x06normal\x18\x02 \x01(\x08H\x00\x12\x10\n\x06urgent\x18\x03 \x01(\x08H\x00\x12\x0f\n\x05perkb\x18\x04 \x01(\rH\x00\x12\x0f\n\x05perkw\x18\x05 \x01(\rH\x00\x42\x07\n\x05style\":\n\nOutputDesc\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x1b\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x0b.cln.Amount\"t\n\x08RouteHop\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x18\n\x10short_channel_id\x18\x02 \x01(\t\x12\x1c\n\x07\x66\x65\x65\x62\x61se\x18\x03 \x01(\x0b\x32\x0b.cln.Amount\x12\x0f\n\x07\x66\x65\x65prop\x18\x04 \x01(\r\x12\x13\n\x0b\x65xpirydelta\x18\x05 \x01(\r\"(\n\tRoutehint\x12\x1b\n\x04hops\x18\x01 \x03(\x0b\x32\r.cln.RouteHop\".\n\rRoutehintList\x12\x1d\n\x05hints\x18\x02 \x03(\x0b\x32\x0e.cln.Routehint\"\'\n\x08TlvEntry\x12\x0c\n\x04type\x18\x01 \x01(\x04\x12\r\n\x05value\x18\x02 \x01(\x0c\"+\n\tTlvStream\x12\x1e\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\r.cln.TlvEntry*$\n\x0b\x43hannelSide\x12\t\n\x05LOCAL\x10\x00\x12\n\n\x06REMOTE\x10\x01*\x84\x02\n\x0c\x43hannelState\x12\x0c\n\x08Openingd\x10\x00\x12\x1a\n\x16\x43hanneldAwaitingLockin\x10\x01\x12\x12\n\x0e\x43hanneldNormal\x10\x02\x12\x18\n\x14\x43hanneldShuttingDown\x10\x03\x12\x17\n\x13\x43losingdSigexchange\x10\x04\x12\x14\n\x10\x43losingdComplete\x10\x05\x12\x16\n\x12\x41waitingUnilateral\x10\x06\x12\x14\n\x10\x46undingSpendSeen\x10\x07\x12\x0b\n\x07Onchain\x10\x08\x12\x15\n\x11\x44ualopendOpenInit\x10\t\x12\x1b\n\x17\x44ualopendAwaitingLockin\x10\n*\x8a\x02\n\tHtlcState\x12\x0f\n\x0bSentAddHtlc\x10\x00\x12\x11\n\rSentAddCommit\x10\x01\x12\x15\n\x11RcvdAddRevocation\x10\x02\x12\x14\n\x10RcvdAddAckCommit\x10\x03\x12\x18\n\x14SentAddAckRevocation\x10\x04\x12\x18\n\x14RcvdAddAckRevocation\x10\x05\x12\x12\n\x0eRcvdRemoveHtlc\x10\x06\x12\x14\n\x10RcvdRemoveCommit\x10\x07\x12\x18\n\x14SentRemoveRevocation\x10\x08\x12\x17\n\x13SentRemoveAckCommit\x10\t\x12\x1b\n\x17RcvdRemoveAckRevocation\x10\nb\x06proto3')
 
 _CHANNELSIDE = DESCRIPTOR.enum_types_by_name['ChannelSide']
 ChannelSide = enum_type_wrapper.EnumTypeWrapper(_CHANNELSIDE)
 _CHANNELSTATE = DESCRIPTOR.enum_types_by_name['ChannelState']
 ChannelState = enum_type_wrapper.EnumTypeWrapper(_CHANNELSTATE)
-IN = 0
-OUT = 1
+_HTLCSTATE = DESCRIPTOR.enum_types_by_name['HtlcState']
+HtlcState = enum_type_wrapper.EnumTypeWrapper(_HTLCSTATE)
+LOCAL = 0
+REMOTE = 1
 Openingd = 0
 ChanneldAwaitingLockin = 1
 ChanneldNormal = 2
 ChanneldShuttingDown = 3
 ClosingdSigexchange = 4
 ClosingdComplete = 5
 AwaitingUnilateral = 6
 FundingSpendSeen = 7
 Onchain = 8
 DualopendOpenInit = 9
 DualopendAwaitingLockin = 10
+SentAddHtlc = 0
+SentAddCommit = 1
+RcvdAddRevocation = 2
+RcvdAddAckCommit = 3
+SentAddAckRevocation = 4
+RcvdAddAckRevocation = 5
+RcvdRemoveHtlc = 6
+RcvdRemoveCommit = 7
+SentRemoveRevocation = 8
+SentRemoveAckCommit = 9
+RcvdRemoveAckRevocation = 10
 
 
 _AMOUNT = DESCRIPTOR.message_types_by_name['Amount']
 _AMOUNTORALL = DESCRIPTOR.message_types_by_name['AmountOrAll']
 _AMOUNTORANY = DESCRIPTOR.message_types_by_name['AmountOrAny']
 _CHANNELSTATECHANGECAUSE = DESCRIPTOR.message_types_by_name['ChannelStateChangeCause']
 _OUTPOINT = DESCRIPTOR.message_types_by_name['Outpoint']
@@ -132,17 +145,19 @@
   })
 _sym_db.RegisterMessage(TlvStream)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _CHANNELSIDE._serialized_start=718
-  _CHANNELSIDE._serialized_end=748
-  _CHANNELSTATE._serialized_start=751
-  _CHANNELSTATE._serialized_end=1011
+  _CHANNELSIDE._serialized_end=754
+  _CHANNELSTATE._serialized_start=757
+  _CHANNELSTATE._serialized_end=1017
+  _HTLCSTATE._serialized_start=1020
+  _HTLCSTATE._serialized_end=1286
   _AMOUNT._serialized_start=25
   _AMOUNT._serialized_end=47
   _AMOUNTORALL._serialized_start=49
   _AMOUNTORALL._serialized_end=117
   _AMOUNTORANY._serialized_start=119
   _AMOUNTORANY._serialized_end=187
   _CHANNELSTATECHANGECAUSE._serialized_start=189
```

### Comparing `pyln_testing-23.2/pyln/testing/utils.py` & `pyln-testing-23.5/pyln/testing/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 import ephemeral_port_reserve  # type: ignore
 import json
 import logging
 import lzma
 import math
 import os
-import psutil  # type: ignore
 import random
 import re
 import shutil
 import sqlite3
 import string
 import struct
 import subprocess
@@ -456,33 +455,48 @@
         return proxy
 
     # wait_for_mempool can be used to wait for the mempool before generating blocks:
     # True := wait for at least 1 transation
     # int > 0 := wait for at least N transactions
     # 'tx_id' := wait for one transaction id given as a string
     # ['tx_id1', 'tx_id2'] := wait until all of the specified transaction IDs
-    def generate_block(self, numblocks=1, wait_for_mempool=0, to_addr=None):
+    def generate_block(self, numblocks=1, wait_for_mempool=0, to_addr=None, needfeerate=None):
         if wait_for_mempool:
             if isinstance(wait_for_mempool, str):
                 wait_for_mempool = [wait_for_mempool]
             if isinstance(wait_for_mempool, list):
                 wait_for(lambda: all(txid in self.rpc.getrawmempool() for txid in wait_for_mempool))
             else:
                 wait_for(lambda: len(self.rpc.getrawmempool()) >= wait_for_mempool)
 
-        mempool = self.rpc.getrawmempool()
+        mempool = self.rpc.getrawmempool(True)
         logging.debug("Generating {numblocks}, confirming {lenmempool} transactions: {mempool}".format(
             numblocks=numblocks,
             mempool=mempool,
             lenmempool=len(mempool),
         ))
 
         # As of 0.16, generate() is removed; use generatetoaddress.
         if to_addr is None:
             to_addr = self.rpc.getnewaddress()
+
+        # We assume all-or-nothing.
+        if needfeerate is not None:
+            assert numblocks == 1
+            # If any tx including ancestors is above the given feerate, mine all.
+            for txid, details in mempool.items():
+                feerate = float(details['fees']['ancestor']) * 100_000_000 / (float(details['ancestorsize']) * 4 / 1000)
+                if feerate >= needfeerate:
+                    return self.rpc.generatetoaddress(numblocks, to_addr)
+                else:
+                    print(f"Feerate {feerate} for {txid} below {needfeerate}")
+
+            # Otherwise, mine none.
+            return self.rpc.generateblock(to_addr, [])
+
         return self.rpc.generatetoaddress(numblocks, to_addr)
 
     def simple_reorg(self, height, shift=0):
         """
         Reorganize chain by creating a fork at height=[height] and re-mine all mempool
         transactions into [height + shift], where shift >= 0. Returns hashes of generated
         blocks.
@@ -543,14 +557,15 @@
             '-printtoconsole',
             '-server',
             '-logtimestamps',
             '-nolisten',
             '-nowallet',
             '-validatepegin=0',
             '-con_blocksubsidy=5000000000',
+            '-acceptnonstdtxn=1',  # FIXME Issues such as dust limit interacting with anchors
         ]
         conf_file = os.path.join(bitcoin_dir, 'elements.conf')
         config['rpcport'] = self.rpcport
         BITCOIND_REGTEST = {'rpcport': self.rpcport}
         write_config(conf_file, config, BITCOIND_REGTEST, section_name='liquid-regtest')
         self.conf_file = conf_file
         self.rpc = SimpleBitcoinProxy(btc_conf_file=self.conf_file)
@@ -579,15 +594,15 @@
         self.executable = 'lightningd'
         self.lightning_dir = lightning_dir
         self.port = port
         self.cmd_prefix = []
         self.disconnect_file = None
 
         self.rpcproxy = bitcoindproxy
-        self.env['CLN_PLUGIN_LOG'] = "gl_plugin=trace,gl_rpc=trace,gl_grpc=trace,debug"
+        self.env['CLN_PLUGIN_LOG'] = "cln_plugin=trace,cln_rpc=trace,cln_grpc=trace,debug"
 
         self.opts = LIGHTNINGD_CONFIG.copy()
         opts = {
             'lightning-dir': lightning_dir,
             'addr': '127.0.0.1:{}'.format(port),
             'allow-deprecated-apis': '{}'.format("true" if DEPRECATED_APIS
                                                  else "false"),
@@ -776,15 +791,15 @@
 
         if options is not None:
             self.daemon.opts.update(options)
         dsn = db.get_dsn()
         if dsn is not None:
             self.daemon.opts['wallet'] = dsn
         if valgrind:
-            trace_skip_pattern = '*python*,*bitcoin-cli*,*elements-cli*,*cln-grpc'
+            trace_skip_pattern = '*python*,*bitcoin-cli*,*elements-cli*,*cln-*'
             if not valgrind_plugins:
                 trace_skip_pattern += ',*plugins*'
             self.daemon.cmd_prefix = [
                 'valgrind',
                 '-q',
                 '--trace-children=yes',
                 '--trace-children-skip={}'.format(trace_skip_pattern),
@@ -832,23 +847,57 @@
 
         self.rpc = PrettyPrintingLightningRpc(
             str(socket_path),
             self.executor,
             jsonschemas=jsonschemas
         )
 
+    @property
+    def grpc(self):
+        """Tiny helper to return a grpc stub if grpc was configured.
+        """
+        # Before doing anything let's see if we have a grpc-port at all
+        try:
+            grpc_port = int(filter(
+                lambda v: v[0] == 'grpc-port',
+                self.daemon.opts.items()
+            ).__next__()[1])
+        except Exception:
+            raise ValueError("grpc-port is not specified, can't connect over grpc")
+
+        import grpc
+        p = Path(self.daemon.lightning_dir) / TEST_NETWORK
+        cert, key, ca = [f.open('rb').read() for f in [
+            p / 'client.pem',
+            p / 'client-key.pem',
+            p / "ca.pem"]]
+        creds = grpc.ssl_channel_credentials(
+            root_certificates=ca,
+            private_key=key,
+            certificate_chain=cert,
+        )
+
+        channel = grpc.secure_channel(
+            f"localhost:{grpc_port}",
+            creds,
+            options=(('grpc.ssl_target_name_override', 'cln'),)
+        )
+        from pyln.testing import node_pb2_grpc as nodegrpc
+        return nodegrpc.NodeStub(channel)
+
     def connect(self, remote_node):
-        self.rpc.connect(remote_node.info['id'], '127.0.0.1', remote_node.daemon.port)
+        self.rpc.connect(remote_node.info['id'], '127.0.0.1', remote_node.port)
 
     def is_connected(self, remote_node):
         return remote_node.info['id'] in [p['id'] for p in self.rpc.listpeers()['peers']]
 
     def openchannel(self, remote_node, capacity=FUNDAMOUNT, addrtype="bech32", confirm=True, wait_for_announce=True, connect=True):
         addr, wallettxid = self.fundwallet(10 * capacity, addrtype)
 
+        # connect if necessary
         if connect and not self.is_connected(remote_node):
             self.connect(remote_node)
 
         res = self.rpc.fundchannel(remote_node.info['id'], capacity)
 
         if confirm or wait_for_announce:
             self.bitcoin.generate_block(1, wait_for_mempool=res['txid'])
@@ -863,15 +912,15 @@
         addr = self.rpc.newaddr(addrtype)[addrtype]
         txid = self.bitcoin.rpc.sendtoaddress(addr, sats / 10**8)
         if mine_block:
             self.bitcoin.generate_block(1)
             self.daemon.wait_for_log('Owning output .* txid {} CONFIRMED'.format(txid))
         return addr, txid
 
-    def fundbalancedchannel(self, remote_node, total_capacity, announce=True):
+    def fundbalancedchannel(self, remote_node, total_capacity=FUNDAMOUNT, announce=True):
         '''
         Creates a perfectly-balanced channel, as all things should be.
         '''
         if isinstance(total_capacity, Millisatoshi):
             total_capacity = int(total_capacity.to_satoshi())
         else:
             total_capacity = int(total_capacity)
@@ -887,15 +936,17 @@
             # Tell the node to equally dual-fund the channel
             remote_node.rpc.call('funderupdate', {'policy': 'match',
                                                   'policy_mod': 100,
                                                   'fuzz_percent': 0})
         else:
             chan_capacity = total_capacity
 
-        self.rpc.connect(remote_node.info['id'], 'localhost', remote_node.port)
+        # connect if necessary
+        if not self.is_connected(remote_node):
+            self.connect(remote_node)
 
         res = self.rpc.fundchannel(remote_node.info['id'], chan_capacity, feerate='slow', minconf=0, announce=announce, push_msat=Millisatoshi(chan_capacity * 500))
         blockid = self.bitcoin.generate_block(1, wait_for_mempool=res['txid'])[0]
 
         # Generate the scid.
         for i, txid in enumerate(self.bitcoin.rpc.getblock(blockid)['tx']):
             if txid == res['txid']:
@@ -968,19 +1019,14 @@
         if clean:
             self.stop(timeout)
         else:
             self.daemon.stop()
 
         self.start()
 
-    def fund_channel(self, l2, amount, wait_for_active=True, announce_channel=True):
-        warnings.warn("LightningNode.fund_channel is deprecated in favor of "
-                      "LightningNode.fundchannel", category=DeprecationWarning)
-        return self.fundchannel(l2, amount, wait_for_active, announce_channel)
-
     def fundchannel(self, l2, amount=FUNDAMOUNT, wait_for_active=True,
                     announce_channel=True, **kwargs):
         # Give yourself some funds to work with
         addr = self.rpc.newaddr()['bech32']
 
         def has_funds_on_addr(addr):
             """Check if the given address has funds in the internal wallet.
@@ -994,14 +1040,18 @@
 
         self.bitcoin.rpc.sendtoaddress(addr, (amount + 1000000) / 10**8)
         self.bitcoin.generate_block(1)
 
         # Now we should.
         wait_for(lambda: has_funds_on_addr(addr))
 
+        # connect if necessary
+        if not self.is_connected(l2):
+            self.connect(l2)
+
         # Now go ahead and open a channel
         res = self.rpc.fundchannel(l2.info['id'], amount,
                                    announce=announce_channel,
                                    **kwargs)
         blockid = self.bitcoin.generate_block(1, wait_for_mempool=res['txid'])[0]
 
         for i, txid in enumerate(self.bitcoin.rpc.getblock(blockid)['tx']):
@@ -1185,28 +1235,75 @@
                 'result': {
                     'feerate': Decimal(feerate) / 10**8
                 },
             }
         self.daemon.rpcproxy.mock_rpc('estimatesmartfee', mock_estimatesmartfee)
 
         # Technically, this waits until it's called, not until it's processed.
-        # We wait until all three levels have been called.
+        # We wait until all four levels have been called.
         if wait_for_effect:
             wait_for(lambda:
                      self.daemon.rpcproxy.mock_counts['estimatesmartfee'] >= 4)
 
     # force new feerates by restarting and thus skipping slow smoothed process
     # Note: testnode must be created with: opts={'may_reconnect': True}
     def force_feerates(self, rate):
         assert(self.may_reconnect)
         self.set_feerates([rate] * 4, False)
         self.restart()
         self.daemon.wait_for_log('peer_out WIRE_UPDATE_FEE')
         assert(self.rpc.feerates('perkw')['perkw']['opening'] == rate)
 
+    def wait_for_onchaind_txs(self, *args):
+        """Wait for onchaind to ask lightningd to create one or more txs.  Each arg is a pair of typename, resolvename.  Returns tuples of the rawtx, txid and number of blocks delay for each pair.
+        """
+        # Could happen in any order.
+        needle = self.daemon.logsearch_start
+        ret = ()
+        for (name, resolve) in args:
+            self.daemon.logsearch_start = needle
+            r = self.daemon.wait_for_log('Telling lightningd about {} to resolve {}'
+                                         .format(name, resolve))
+            blocks = int(re.search(r'\(([-0-9]*) more blocks\)', r).group(1))
+
+            # The next 'Broadcast for onchaind' will be the tx.
+            # Now grab the corresponding broadcast lightningd did, to get actual tx:
+            r = self.daemon.wait_for_log('Broadcast for onchaind tx')
+            rawtx = re.search(r'.* tx ([0-9a-fA-F]*)', r).group(1)
+            txid = self.bitcoin.rpc.decoderawtransaction(rawtx, True)['txid']
+            ret = ret + ((rawtx, txid, blocks),)
+        return ret
+
+    def wait_for_onchaind_tx(self, name, resolve):
+        return self.wait_for_onchaind_txs((name, resolve))[0]
+
+    def mine_txid_or_rbf(self, txid, numblocks=1):
+        """Wait for a txid to be broadcast, or an rbf.  Return the one actually mined"""
+        # Hack so we can mutate the txid: pass it in a list
+        def rbf_or_txid_broadcast(txids):
+            # RBF onchain txid d4b597505b543a4b8b42ab4d481fd7a533febb7e7df150ca70689e6d046612f7 (fee 6564sat) with txid 979878b8f855d3895d1cd29bd75a60b21492c4842e38099186a8e649bee02c7c (fee 8205sat)
+            line = self.daemon.is_in_log("RBF onchain txid {}".format(txids[-1]))
+            if line is not None:
+                newtxid = re.search(r'with txid ([0-9a-fA-F]*)', line).group(1)
+                txids.append(newtxid)
+            mempool = self.bitcoin.rpc.getrawmempool()
+            return any([t in mempool for t in txids])
+
+        txids = [txid]
+        wait_for(lambda: rbf_or_txid_broadcast(txids))
+        blocks = self.bitcoin.generate_block(numblocks)
+
+        # It might have snuck an RBF in at the last minute!
+        rbf_or_txid_broadcast(txids)
+
+        for tx in self.bitcoin.rpc.getblock(blocks[0])['tx']:
+            if tx in txids:
+                return tx
+        raise ValueError("None of the rbf txs were mined?")
+
     def wait_for_onchaind_broadcast(self, name, resolve=None):
         """Wait for onchaind to drop tx name to resolve (if any)"""
         if resolve:
             r = self.daemon.wait_for_log('Broadcasting {} .* to resolve {}'
                                          .format(name, resolve))
         else:
             r = self.daemon.wait_for_log('Broadcasting {} .* to resolve '
@@ -1323,80 +1420,33 @@
     # We can continue
     yield fname
 
     # Remove our file, so the next one can go ahead.
     fname.unlink()
 
 
-class Throttler(object):
-    """Throttles the creation of system-processes to avoid overload.
-
-    There is no reason to overload the system with too many processes
-    being spawned or run at the same time. It causes timeouts by
-    aggressively preempting processes and swapping if the memory limit is
-    reached. In order to reduce this loss of performance we provide a
-    `wait()` method which will serialize the creation of processes, but
-    also delay if the system load is too high.
-
-    Notice that technically we are throttling too late, i.e., we react
-    to an overload, but chances are pretty good that some other
-    already running process is about to terminate, and so the overload
-    is short-lived. We throttle when the process object is first
-    created, not when restarted, in order to avoid delaying running
-    tests, which could cause more timeouts.
-
-    """
-    def __init__(self, directory: str, target: float = 90):
-        """If specified we try to stick to a load of target (in percent).
-        """
-        self.target = target
-        self.current_load = self.target  # Start slow
-        psutil.cpu_percent()  # Prime the internal load metric
-        self.directory = directory
-
-    def wait(self):
-        start_time = time.time()
-        with flock(self.directory):
-            # We just got the lock, assume someone else just released it
-            self.current_load = 100
-            while self.load() >= self.target:
-                time.sleep(1)
-
-            self.current_load = 100  # Back off slightly to avoid triggering right away
-        print("Throttler delayed startup for {} seconds".format(time.time() - start_time))
-
-    def load(self):
-        """An exponential moving average of the load
-        """
-        decay = 0.5
-        load = psutil.cpu_percent()
-        self.current_load = decay * load + (1 - decay) * self.current_load
-        return self.current_load
-
-
 class NodeFactory(object):
     """A factory to setup and start `lightningd` daemons.
     """
     def __init__(self, request, testname, bitcoind, executor, directory,
-                 db_provider, node_cls, throttler, jsonschemas):
+                 db_provider, node_cls, jsonschemas):
         if request.node.get_closest_marker("slow_test") and SLOW_MACHINE:
             self.valgrind = False
         else:
             self.valgrind = VALGRIND
         self.testname = testname
         self.next_id = 1
         self.nodes = []
         self.reserved_ports = []
         self.executor = executor
         self.bitcoind = bitcoind
         self.directory = directory
         self.lock = threading.Lock()
         self.db_provider = db_provider
         self.node_cls = node_cls
-        self.throttler = throttler
         self.jsonschemas = jsonschemas
 
     def split_options(self, opts):
         """Split node options from cli options
 
         Some options are used to instrument the node wrapper and some are passed
         to the daemon on the command line. Split them so we know where to use
@@ -1456,15 +1506,14 @@
 
         return [j.result() for j in jobs]
 
     def get_node(self, node_id=None, options=None, dbfile=None,
                  bkpr_dbfile=None, feerates=(15000, 11000, 7500, 3750),
                  start=True, wait_for_bitcoind_sync=True, may_fail=False,
                  expect_fail=False, cleandir=True, **kwargs):
-        self.throttler.wait()
         node_id = self.get_node_id() if not node_id else node_id
         port = reserve_unused_port()
 
         lightning_dir = os.path.join(
             self.directory, "lightning-{}/".format(node_id))
 
         if cleandir and os.path.exists(lightning_dir):
@@ -1573,20 +1622,22 @@
 
     def killall(self, expected_successes):
         """Returns true if every node we expected to succeed actually succeeded"""
         unexpected_fail = False
         err_msgs = []
         for i in range(len(self.nodes)):
             leaks = None
-            # leak detection upsets VALGRIND by reading uninitialized mem.
+            # leak detection upsets VALGRIND by reading uninitialized mem,
+            # and valgrind adds extra fds.
             # If it's dead, we'll catch it below.
             if not self.valgrind and DEVELOPER:
                 try:
                     # This also puts leaks in log.
                     leaks = self.nodes[i].rpc.dev_memleak()['leaks']
+                    self.nodes[i].rpc.dev_report_fds()
                 except Exception:
                     pass
 
             try:
                 self.nodes[i].stop()
             except Exception:
                 if expected_successes[i]:
```

### Comparing `pyln_testing-23.2/pyproject.toml` & `pyln-testing-23.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyln-testing"
-version = "23.02"
+version = "23.05"
 description = "Test your Core Lightning integration, plugins or whatever you want"
 authors = ["Christian Decker <decker.christian@gmail.com>"]
 license = "BSD-MIT"
 readme = "README.md"
 
 packages = [
   { include = "pyln/testing" },
```

### Comparing `pyln_testing-23.2/setup.py` & `pyln-testing-23.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'psycopg2-binary>=2.9.3,<3.0.0',
  'pyln-client>=0.12.1',
  'pytest>=7.0.1,<8.0.0',
  'python-bitcoinlib>=0.11.0,<0.12.0']
 
 setup_kwargs = {
     'name': 'pyln-testing',
-    'version': '23.2',
+    'version': '23.5',
     'description': 'Test your Core Lightning integration, plugins or whatever you want',
     'long_description': '# pyln-testing: A library to write tests against Core Lightning\n\nThis library implements a number of utilities that help building tests for\nCore Lightning nodes. In particular it provides a number of pytest fixtures that\nallow the management of a test network of a given topology and then execute a\ntest scenarion.\n\n`pyln-testing` is used by Core Lightning for its internal tests, and by the\ncommunity plugin directory to exercise the plugins.\n\n## Installation\n\n`pyln-testing` is available on `pip`:\n\n```bash\npip install pyln-testing\n```\n\nAlternatively you can also install the development version to get access to\ncurrently unreleased features by checking out the Core Lightning source code and\ninstalling into your python3 environment:\n\n```bash\ngit clone https://github.com/ElementsProject/lightning.git\ncd lightning/contrib/pyln-testing\npoetry install\n```\n\nThis will add links to the library into your environment so changing the\nchecked out source code will also result in the environment picking up these\nchanges. Notice however that unreleased versions may change API without\nwarning, so test thoroughly with the released version.\n\n',
     'author': 'Christian Decker',
     'author_email': 'decker.christian@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pyln_testing-23.2/PKG-INFO` & `pyln-testing-23.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pyln-testing
-Version: 23.2
+Version: 23.5
 Summary: Test your Core Lightning integration, plugins or whatever you want
 License: BSD-MIT
 Author: Christian Decker
 Author-email: decker.christian@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask (>=2.0.3,<3.0.0)
 Requires-Dist: cheroot (>=8.6.0,<9.0.0)
 Requires-Dist: ephemeral-port-reserve (>=1.1.4,<2.0.0)
 Requires-Dist: grpcio (>=1.47)
 Requires-Dist: jsonschema (>=4.4.0,<5.0.0)
 Requires-Dist: protobuf (>=3.20.3,<4)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
```

