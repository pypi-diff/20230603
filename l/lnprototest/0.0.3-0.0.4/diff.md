# Comparing `tmp/lnprototest-0.0.3.tar.gz` & `tmp/lnprototest-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnprototest-0.0.3.tar", max compression
+gzip compressed data, was "lnprototest-0.0.4.tar", max compression
```

## Comparing `lnprototest-0.0.3.tar` & `lnprototest-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     2418 2023-03-01 18:25:00.167598 lnprototest-0.0.3/README.md
--rw-r--r--   0        0        0     3368 2023-03-01 18:25:00.167598 lnprototest-0.0.3/lnprototest/__init__.py
--rw-r--r--   0        0        0       95 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/backend/__init__.py
--rw-r--r--   0        0        0      554 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/backend/backend.py
--rw-r--r--   0        0        0     6496 2023-03-01 18:25:00.167598 lnprototest-0.0.3/lnprototest/backend/bitcoind.py
--rw-r--r--   0        0        0     1114 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/bitfield.py
--rw-r--r--   0        0        0      645 2023-03-01 18:25:00.167598 lnprototest-0.0.3/lnprototest/clightning/__init__.py
--rw-r--r--   0        0        0    19081 2023-03-15 15:14:56.510646 lnprototest-0.0.3/lnprototest/clightning/clightning.py
--rw-r--r--   0        0        0       12 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/clightning/requirements.txt
--rw-r--r--   0        0        0   150826 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/commit_tx.py
--rw-r--r--   0        0        0     6922 2023-02-28 10:32:56.588103 lnprototest-0.0.3/lnprototest/dummyrunner.py
--rw-r--r--   0        0        0      849 2023-03-01 18:25:00.170931 lnprototest-0.0.3/lnprototest/errors.py
--rw-r--r--   0        0        0    23341 2023-03-15 15:14:31.716348 lnprototest-0.0.3/lnprototest/event.py
--rw-r--r--   0        0        0    31511 2023-03-01 18:25:00.170931 lnprototest-0.0.3/lnprototest/funding.py
--rw-r--r--   0        0        0     6123 2023-03-01 18:25:00.170931 lnprototest-0.0.3/lnprototest/keyset.py
--rwxr-xr-x   0        0        0     1013 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/namespace.py
--rw-r--r--   0        0        0     4619 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/proposals.py
--rw-r--r--   0        0        0     9918 2023-03-01 18:25:00.170931 lnprototest-0.0.3/lnprototest/runner.py
--rwxr-xr-x   0        0        0     5570 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/signature.py
--rw-r--r--   0        0        0     1175 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/stash/__init__.py
--rw-r--r--   0        0        0     8599 2023-03-01 18:25:00.170931 lnprototest-0.0.3/lnprototest/stash/stash.py
--rw-r--r--   0        0        0     9117 2023-02-27 21:38:00.613217 lnprototest-0.0.3/lnprototest/structure.py
--rw-r--r--   0        0        0      169 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/utils/__init__.py
--rw-r--r--   0        0        0     1806 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/utils/bitcoin_utils.py
--rw-r--r--   0        0        0     1536 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/utils/ln_spec_utils.py
--rw-r--r--   0        0        0     1362 2023-02-14 10:36:29.511225 lnprototest-0.0.3/lnprototest/utils/utils.py
--rw-r--r--   0        0        0      896 2023-04-26 20:57:43.777515 lnprototest-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 lnprototest-0.0.3/setup.py
--rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 lnprototest-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2418 2023-03-01 18:25:00.167598 lnprototest-0.0.4/README.md
+-rw-r--r--   0        0        0     3353 2023-06-01 22:01:01.582905 lnprototest-0.0.4/lnprototest/__init__.py
+-rw-r--r--   0        0        0       95 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/backend/__init__.py
+-rw-r--r--   0        0        0      554 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/backend/backend.py
+-rw-r--r--   0        0        0     6496 2023-03-01 18:25:00.167598 lnprototest-0.0.4/lnprototest/backend/bitcoind.py
+-rw-r--r--   0        0        0     1114 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/bitfield.py
+-rw-r--r--   0        0        0      645 2023-03-01 18:25:00.167598 lnprototest-0.0.4/lnprototest/clightning/__init__.py
+-rw-r--r--   0        0        0    19098 2023-06-01 23:07:19.594928 lnprototest-0.0.4/lnprototest/clightning/clightning.py
+-rw-r--r--   0        0        0       12 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/clightning/requirements.txt
+-rw-r--r--   0        0        0   150826 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/commit_tx.py
+-rw-r--r--   0        0        0     6948 2023-06-01 22:43:33.042532 lnprototest-0.0.4/lnprototest/dummyrunner.py
+-rw-r--r--   0        0        0      849 2023-03-01 18:25:00.170931 lnprototest-0.0.4/lnprototest/errors.py
+-rw-r--r--   0        0        0    23405 2023-06-03 15:19:03.207606 lnprototest-0.0.4/lnprototest/event.py
+-rw-r--r--   0        0        0    31655 2023-06-01 22:00:10.587565 lnprototest-0.0.4/lnprototest/funding.py
+-rw-r--r--   0        0        0     6133 2023-06-01 22:35:32.610636 lnprototest-0.0.4/lnprototest/keyset.py
+-rwxr-xr-x   0        0        0     1013 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/namespace.py
+-rw-r--r--   0        0        0     4619 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/proposals.py
+-rw-r--r--   0        0        0     9918 2023-03-01 18:25:00.170931 lnprototest-0.0.4/lnprototest/runner.py
+-rwxr-xr-x   0        0        0     5570 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/signature.py
+-rw-r--r--   0        0        0      817 2023-06-01 20:30:01.524336 lnprototest-0.0.4/lnprototest/stash/__init__.py
+-rw-r--r--   0        0        0     9145 2023-06-03 15:25:28.179410 lnprototest-0.0.4/lnprototest/stash/stash.py
+-rw-r--r--   0        0        0     9117 2023-02-27 21:38:00.613217 lnprototest-0.0.4/lnprototest/structure.py
+-rw-r--r--   0        0        0      480 2023-06-01 22:36:58.710620 lnprototest-0.0.4/lnprototest/utils/__init__.py
+-rw-r--r--   0        0        0     8530 2023-06-01 21:57:15.467339 lnprototest-0.0.4/lnprototest/utils/bitcoin_utils.py
+-rw-r--r--   0        0        0     8585 2023-06-03 15:25:28.156076 lnprototest-0.0.4/lnprototest/utils/ln_spec_utils.py
+-rw-r--r--   0        0        0     3058 2023-06-01 22:46:52.836969 lnprototest-0.0.4/lnprototest/utils/utils.py
+-rw-r--r--   0        0        0      896 2023-06-03 15:40:36.775497 lnprototest-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 lnprototest-0.0.4/PKG-INFO
```

### Comparing `lnprototest-0.0.3/README.md` & `lnprototest-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.3/lnprototest/__init__.py` & `lnprototest-0.0.4/lnprototest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 the tests themselves, and clightning.Runner.
 
 The documentation for the classes themselves should cover much of the
 reference material, and the tutorial should get you started.
 
 """
 from .errors import EventError, SpecFileError
+
 from .event import (
     Event,
     Connect,
     Disconnect,
     Msg,
     RawMsg,
     ExpectMsg,
@@ -34,15 +35,17 @@
     msat,
     negotiated,
     DualFundAccept,
     Wait,
     CloseChannel,
     ExpectDisconnect,
 )
+
 from .structure import Sequence, OneOf, AnyOrder, TryAll
+
 from .runner import (
     Runner,
     Conn,
     remote_revocation_basepoint,
     remote_payment_basepoint,
     remote_delayed_payment_basepoint,
     remote_htlc_basepoint,
@@ -60,15 +63,14 @@
 )
 from .bitfield import bitfield, has_bit, bitfield_len
 from .signature import SigType, Sig
 from .keyset import KeySet
 from .commit_tx import Commit, HTLC, UpdateCommit
 from .utils import (
     Side,
-    regtest_hash,
     privkey_expand,
     wait_for,
     LightningUtils,
     ScriptType,
     BitcoinUtils,
 )
 from .funding import (
```

### Comparing `lnprototest-0.0.3/lnprototest/backend/backend.py` & `lnprototest-0.0.4/lnprototest/backend/backend.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.3/lnprototest/backend/bitcoind.py` & `lnprototest-0.0.4/lnprototest/backend/bitcoind.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.3/lnprototest/bitfield.py` & `lnprototest-0.0.4/lnprototest/bitfield.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.3/lnprototest/clightning/__init__.py` & `lnprototest-0.0.4/lnprototest/clightning/__init__.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.3/lnprototest/clightning/clightning.py` & `lnprototest-0.0.4/lnprototest/clightning/clightning.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     Conn,
     namespace,
     MustNotMsg,
 )
 from lnprototest import wait_for
 from typing import Dict, Any, Callable, List, Optional, cast
 
-TIMEOUT = int(os.getenv("TIMEOUT", "30"))
+TIMEOUT = int(os.getenv("TIMEOUT", "60"))
 LIGHTNING_SRC = os.path.join(os.getcwd(), os.getenv("LIGHTNING_SRC", "../lightning/"))
 
 
 class CLightningConn(lnprototest.Conn):
     def __init__(self, connprivkey: str, port: int):
         super().__init__(connprivkey)
         # FIXME: pyln.proto.wire should just use coincurve PrivateKey!
@@ -171,15 +171,15 @@
             try:
                 rpc.getinfo()
                 return True
             except Exception as ex:
                 logging.debug(f"waiting for core-lightning: Exception received {ex}")
                 return False
 
-        wait_for(lambda: node_ready(self.rpc))
+        wait_for(lambda: node_ready(self.rpc), timeout=TIMEOUT)
         logging.debug("Waited for core-lightning")
 
         # Make sure that we see any funds that come to our wallet
         for i in range(5):
             self.rpc.newaddr()
 
     def shutdown(self, also_bitcoind: bool = True) -> None:
```

### Comparing `lnprototest-0.0.3/lnprototest/commit_tx.py` & `lnprototest-0.0.4/lnprototest/commit_tx.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.3/lnprototest/dummyrunner.py` & `lnprototest-0.0.4/lnprototest/dummyrunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def has_option(self, optname: str) -> Optional[str]:
         return None
 
     def start(self) -> None:
         self.blockheight = 102
 
-    def stop(self) -> None:
+    def stop(self, print_logs: bool = False) -> None:
         pass
 
     def restart(self) -> None:
         super().restart()
         if self.config.getoption("verbose"):
             print("[RESTART]")
         self.blockheight = 102
```

### Comparing `lnprototest-0.0.3/lnprototest/errors.py` & `lnprototest-0.0.4/lnprototest/errors.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.3/lnprototest/event.py` & `lnprototest-0.0.4/lnprototest/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 import traceback
 import collections
 import os.path
 import io
 import struct
 import time
 import json
+
 from typing import Optional, Dict, Union, Callable, Any, List, TYPE_CHECKING, overload
+
 from pyln.proto.message import Message
+
 from .errors import SpecFileError, EventError
 from .namespace import namespace
-from .utils import check_hex
 from .signature import Sig
 from .bitfield import has_bit
+from .utils import check_hex
+
 from bitcoin.core import CTransaction
 
 if TYPE_CHECKING:
     # Otherwise a circular dependency
     from .runner import Runner, Conn
 
 
@@ -342,14 +346,15 @@
                     raise EventError(
                         self, "Got msg banned by {}: {}".format(e, binmsg.hex())
                     )
             logging.debug(f"raw msg {binmsg}")
             # Might be completely unknown to namespace.
             try:
                 msg = Message.read(namespace(), io.BytesIO(binmsg))
+                runner.add_stash(msg.messagetype.name, msg)
             except ValueError as ve:
                 raise EventError(
                     self, "Runner gave bad msg {}: {}".format(binmsg.hex(), ve)
                 )
             logging.debug(f"decoded msg {msg.to_str()}")
             # Ignore function may tell us to respond.
             response = self.ignore(msg)
```

### Comparing `lnprototest-0.0.3/lnprototest/funding.py` & `lnprototest-0.0.4/lnprototest/funding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 # Support for funding txs.
+import coincurve
+import io
+import logging
+
 from typing import Tuple, Any, Optional, Union, Callable, Dict, List
-from .utils import Side, privkey_expand, regtest_hash
+
+from hashlib import sha256
+from pyln.proto.message import Message
+
+from .utils.bitcoin_utils import BitcoinUtils
+from .utils import Side, privkey_expand
 from .event import Event, ResolvableInt, ResolvableStr
 from .namespace import namespace
 from .runner import Runner
 from .signature import Sig
-from pyln.proto.message import Message
-from hashlib import sha256
-import coincurve
-import io
-import logging
+
+import bitcoin.core.script as script
 from bitcoin.core import (
     COutPoint,
     CScript,
     CTxIn,
     CTxOut,
     CMutableTransaction,
     CTxWitness,
     CTxInWitness,
     CScriptWitness,
     Hash160,
     CTransaction,
 )
-import bitcoin.core.script as script
 from bitcoin.wallet import P2WPKHBitcoinAddress
 
 ResolvableFunding = Union["Funding", Callable[["Runner", "Event", str], "Funding"]]
 
 
 def txid_raw(tx: str) -> str:
     """Helper to get the txid of a tx: note this is in wire protocol order, not bitcoin order!"""
@@ -39,15 +44,15 @@
         funding_txid: str,
         funding_output_index: int,
         funding_amount: int,
         local_node_privkey: str,
         local_funding_privkey: str,
         remote_node_privkey: str,
         remote_funding_privkey: str,
-        chain_hash: str = regtest_hash,
+        chain_hash: str = BitcoinUtils.blockchain_hash(),
         locktime: int = 0,
     ):
         self.chain_hash = chain_hash
         self.txid = funding_txid
         self.output_index = funding_output_index
         self.amount = funding_amount
         self.bitcoin_privkeys = [
@@ -133,15 +138,15 @@
     def start(
         local_node_privkey: str,
         local_funding_privkey: str,
         remote_node_privkey: str,
         remote_funding_privkey: str,
         funding_sats: int,
         locktime: int,
-        chain_hash: str = regtest_hash,
+        chain_hash: str = BitcoinUtils.blockchain_hash(),
     ) -> "Funding":
         # Create dummy one to start: we will fill in txid at the end
         return Funding(
             "",
             0,
             funding_sats,
             local_node_privkey,
@@ -301,15 +306,15 @@
         sats: int,
         privkey: str,
         fee: int,
         local_node_privkey: str,
         local_funding_privkey: str,
         remote_node_privkey: str,
         remote_funding_privkey: str,
-        chain_hash: str = regtest_hash,
+        chain_hash: str = BitcoinUtils.blockchain_hash(),
     ) -> Tuple["Funding", str]:
         """Make a funding transaction by spending this utxo using privkey: return Funding, tx."""
 
         # Create dummy one to start: we will fill in txid at the end.
         funding = Funding(
             "",
             0,
@@ -650,15 +655,15 @@
         funding_txid: ResolvableStr,
         funding_output_index: ResolvableInt,
         funding_amount: ResolvableInt,
         local_node_privkey: ResolvableStr,
         local_funding_privkey: ResolvableStr,
         remote_node_privkey: ResolvableStr,
         remote_funding_privkey: ResolvableStr,
-        chain_hash: str = regtest_hash,
+        chain_hash: str = BitcoinUtils.blockchain_hash(),
     ):
         super().__init__()
         self.funding_txid = funding_txid
         self.funding_output_index = funding_output_index
         self.funding_amount = funding_amount
         self.local_node_privkey = local_node_privkey
         self.local_funding_privkey = local_funding_privkey
@@ -698,15 +703,15 @@
         sats_in: int,
         spending_privkey: str,
         fee: int,
         local_node_privkey: ResolvableStr,
         local_funding_privkey: ResolvableStr,
         remote_node_privkey: ResolvableStr,
         remote_funding_privkey: ResolvableStr,
-        chain_hash: str = regtest_hash,
+        chain_hash: str = BitcoinUtils.blockchain_hash(),
     ):
         super().__init__()
         self.txid_in = txid_in
         self.tx_index_in = tx_index_in
         self.sats_in = sats_in
         self.spending_privkey = spending_privkey
         self.fee = fee
@@ -750,15 +755,15 @@
         fee: int,
         funding_sats: ResolvableInt,
         locktime: ResolvableInt,
         local_node_privkey: str,
         local_funding_privkey: str,
         remote_node_privkey: str,
         remote_funding_privkey: ResolvableStr,
-        chain_hash: str = regtest_hash,
+        chain_hash: str = BitcoinUtils.blockchain_hash(),
     ):
         super().__init__()
 
         self.funding_sats = funding_sats
         self.locktime = locktime
         self.local_node_privkey = local_node_privkey
         self.local_funding_privkey = local_funding_privkey
```

### Comparing `lnprototest-0.0.3/lnprototest/keyset.py` & `lnprototest-0.0.4/lnprototest/keyset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #! /usr/bin/python3
 # FIXME: clean this up for use as pyln.proto.tx
 import coincurve
 import hashlib
-from .utils import privkey_expand, check_hex
 
 
 class KeySet(object):
     def __init__(
         self,
         revocation_base_secret: str,
         payment_base_secret: str,
         htlc_base_secret: str,
         delayed_payment_base_secret: str,
         shachain_seed: str,
     ):
+
+        from .utils import privkey_expand, check_hex
+
         self.revocation_base_secret = privkey_expand(revocation_base_secret)
         self.payment_base_secret = privkey_expand(payment_base_secret)
         self.htlc_base_secret = privkey_expand(htlc_base_secret)
         self.delayed_payment_base_secret = privkey_expand(delayed_payment_base_secret)
         self.shachain_seed = bytes.fromhex(check_hex(shachain_seed, 64))
 
     def raw_payment_basepoint(self) -> coincurve.PublicKey:
```

### Comparing `lnprototest-0.0.3/lnprototest/namespace.py` & `lnprototest-0.0.4/lnprototest/namespace.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.3/lnprototest/proposals.py` & `lnprototest-0.0.4/lnprototest/proposals.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.3/lnprototest/runner.py` & `lnprototest-0.0.4/lnprototest/runner.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.3/lnprototest/signature.py` & `lnprototest-0.0.4/lnprototest/signature.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.3/lnprototest/stash/stash.py` & `lnprototest-0.0.4/lnprototest/stash/stash.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from lnprototest import Runner, Event, Side, SpecFileError, Funding
-from typing import Callable, Optional, Any
-from pyln.proto.message import Message
 import functools
 import time
 import coincurve
 
+from typing import Callable, Optional, Any
+from pyln.proto.message import Message
+
+from lnprototest import Runner, Event, Side, SpecFileError, Funding
+
 
 def commitsig_to_send() -> Callable[[Runner, Event, str], str]:
     """Get the appropriate signature for the local side to send to the remote"""
 
     def _commitsig_to_send(runner: Runner, event: Event, field: str) -> str:
         tx = runner.get_stash(event, "Commit").remote_unsigned_tx()
         return runner.get_stash(event, "Commit").local_sig(tx)
@@ -269,7 +271,21 @@
 
 
 def funding_close_tx() -> Callable[[Runner, Event, str], str]:
     def _funding_close_tx(runner: Runner, event: Event, field: str) -> str:
         return runner.get_stash(event, "Funding").close_tx()
 
     return _funding_close_tx
+
+
+def stash_field_from_event(
+    stash_key: str, field_name: Optional[str] = None, dummy_val: Optional[Any] = None
+) -> Callable[[Runner, Event, str], str]:
+    """Generic stash function to get the information back from a previous event"""
+
+    def _stash_field_from_event(runner: Runner, event: Event, field: str) -> str:
+        if runner._is_dummy():
+            return dummy_val
+        field = field if field_name is None else field_name
+        return runner.get_stash(event, stash_key).fields[field]
+
+    return _stash_field_from_event
```

### Comparing `lnprototest-0.0.3/lnprototest/structure.py` & `lnprototest-0.0.4/lnprototest/structure.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.3/pyproject.toml` & `lnprototest-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lnprototest"
-version = "0.0.3"
+version = "0.0.4"
 description = "Spec protocol tests for lightning network implementations"
 authors = ["Rusty Russell <rusty@blockstream.com>", "Vincenzo Palazzo <vincenzopalazzodev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `lnprototest-0.0.3/PKG-INFO` & `lnprototest-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnprototest
-Version: 0.0.3
+Version: 0.0.4
 Summary: Spec protocol tests for lightning network implementations
 License: MIT
 Author: Rusty Russell
 Author-email: rusty@blockstream.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lnprototest Version: 0.0.3 Summary: Spec protocol
+Metadata-Version: 2.1 Name: lnprototest Version: 0.0.4 Summary: Spec protocol
 tests for lightning network implementations License: MIT Author: Rusty Russell
 Author-email: rusty@blockstream.com Requires-Python: >=3.7,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: crc32c (>=2.2.post0,<3.0)
```

