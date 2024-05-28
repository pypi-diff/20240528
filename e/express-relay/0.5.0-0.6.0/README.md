# Comparing `tmp/express_relay-0.5.0.tar.gz` & `tmp/express_relay-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express_relay-0.5.0.tar", max compression
+gzip compressed data, was "express_relay-0.6.0.tar", max compression
```

## Comparing `express_relay-0.5.0.tar` & `express_relay-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      949 2024-05-20 18:38:26.401841 express_relay-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-05-20 18:38:26.401841 express_relay-0.5.0/express_relay/__init__.py
--rw-r--r--   0        0        0    17136 2024-05-20 18:38:26.401841 express_relay-0.5.0/express_relay/client.py
--rw-r--r--   0        0        0     9645 2024-05-20 18:38:26.401841 express_relay-0.5.0/express_relay/express_relay_types.py
--rw-r--r--   0        0        0     5184 2024-05-20 18:38:26.401841 express_relay-0.5.0/express_relay/searcher/examples/simple_searcher.py
--rw-r--r--   0        0        0      612 2024-05-20 18:38:26.401841 express_relay-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 express_relay-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      949 2024-05-28 17:42:43.339715 express_relay-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 17:42:43.339715 express_relay-0.6.0/express_relay/__init__.py
+-rw-r--r--   0        0        0    18387 2024-05-28 17:42:43.339715 express_relay-0.6.0/express_relay/client.py
+-rw-r--r--   0        0        0    12204 2024-05-28 17:42:43.339715 express_relay-0.6.0/express_relay/express_relay_types.py
+-rw-r--r--   0        0        0     5488 2024-05-28 17:42:43.339715 express_relay-0.6.0/express_relay/searcher/examples/simple_searcher.py
+-rw-r--r--   0        0        0      612 2024-05-28 17:42:43.339715 express_relay-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 express_relay-0.6.0/PKG-INFO
```

### Comparing `express_relay-0.5.0/README.md` & `express_relay-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `express_relay-0.5.0/express_relay/client.py` & `express_relay-0.6.0/express_relay/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import asyncio
 from asyncio import Task
+from datetime import datetime
 import json
 import urllib.parse
 from typing import Callable, Any
 from collections.abc import Coroutine
 from uuid import UUID
 import httpx
 import websockets
 from websockets.client import WebSocketClientProtocol
 from eth_account.account import Account
 from express_relay.express_relay_types import (
+    BidResponse,
     Opportunity,
     BidStatusUpdate,
     ClientMessage,
-    BidStatus,
     Bid,
     OpportunityBid,
     OpportunityParams,
 )
 
 
 class ExpressRelayClientException(Exception):
     pass
 
 
 class ExpressRelayClient:
     def __init__(
         self,
         server_url: str,
+        api_key: str | None = None,
         opportunity_callback: (
             Callable[[Opportunity], Coroutine[Any, Any, Any]] | None
         ) = None,
         bid_status_callback: (
             Callable[[BidStatusUpdate], Coroutine[Any, Any, Any]] | None
         ) = None,
         timeout_response_secs: int = 10,
@@ -52,14 +54,15 @@
             ws_scheme = "wss"
         elif parsed_url.scheme == "http":
             ws_scheme = "ws"
         else:
             raise ValueError("Invalid server URL")
 
         self.server_url = server_url
+        self.api_key = api_key
         self.ws_endpoint = parsed_url._replace(scheme=ws_scheme, path="/v1/ws").geturl()
         self.ws_msg_counter = 0
         self.ws: WebSocketClientProtocol
         self.ws_lock = asyncio.Lock()
         self.ws_loop: Task[Any]
         self.ws_msg_futures: dict[str, asyncio.Future] = {}
         self.timeout_response_secs = timeout_response_secs
@@ -67,14 +70,22 @@
             ws_options = {}
         self.ws_options = ws_options
         if http_options is None:
             http_options = {}
         self.http_options = http_options
         self.opportunity_callback = opportunity_callback
         self.bid_status_callback = bid_status_callback
+        if self.api_key:
+            authorization_header = f"Bearer {self.api_key}"
+            if "headers" not in self.http_options:
+                self.http_options["headers"] = {}
+            self.http_options["headers"]["Authorization"] = authorization_header
+            if "extra_headers" not in self.ws_options:
+                self.ws_options["extra_headers"] = {}
+            self.ws_options["extra_headers"]["Authorization"] = authorization_header
 
     async def start_ws(self):
         """
         Initializes the websocket connection to the server, if not already connected.
         """
         async with self.ws_lock:
             if not hasattr(self, "ws"):
@@ -314,25 +325,19 @@
                             msg_json["opportunity"]
                         )
                         if opportunity:
                             asyncio.create_task(opportunity_callback(opportunity))
 
                 elif msg_json.get("type") == "bid_status_update":
                     if bid_status_callback is not None:
-                        id = msg_json["status"]["id"]
-                        bid_status = msg_json["status"]["bid_status"]["type"]
-                        result = msg_json["status"]["bid_status"].get("result")
-                        index = msg_json["status"]["bid_status"].get("index")
-                        bid_status_update = BidStatusUpdate(
-                            id=id,
-                            bid_status=BidStatus(bid_status),
-                            result=result,
-                            index=index,
+                        bid_status_update = BidStatusUpdate.process_bid_status_dict(
+                            msg_json["status"]
                         )
-                        asyncio.create_task(bid_status_callback(bid_status_update))
+                        if bid_status_update:
+                            asyncio.create_task(bid_status_callback(bid_status_update))
 
             elif msg_json.get("id"):
                 future = self.ws_msg_futures.pop(msg_json["id"])
                 future.set_result(msg_json)
 
     async def get_opportunities(self, chain_id: str | None = None) -> list[Opportunity]:
         """
@@ -380,14 +385,45 @@
                 ._replace(path="/v1/opportunities")
                 .geturl(),
                 json=opportunity.params.model_dump(),
             )
         resp.raise_for_status()
         return UUID(resp.json()["opportunity_id"])
 
+    async def get_bids(self, from_time: datetime | None = None) -> list[BidResponse]:
+        """
+        Fetches bids for an api key from the server with pagination of 20 bids per page.
+
+        Args:
+            from_time: The datetime to fetch bids from. If None, fetches from the beginning of time.
+        Returns:
+            A list of bids.
+        """
+        async with httpx.AsyncClient(**self.http_options) as client:
+            resp = await client.get(
+                urllib.parse.urlparse(self.server_url)
+                ._replace(path="/v1/bids")
+                .geturl(),
+                params=(
+                    {"from_time": from_time.astimezone().isoformat()}
+                    if from_time
+                    else None
+                ),
+            )
+
+        resp.raise_for_status()
+
+        bids = []
+        for bid in resp.json()["items"]:
+            bid_processed = BidResponse.process_bid_response_dict(bid)
+            if bid_processed:
+                bids.append(bid_processed)
+
+        return bids
+
 
 def sign_bid(
     opportunity: Opportunity,
     bid_amount: int,
     valid_until: int,
     private_key: str,
 ) -> OpportunityBid:
```

### Comparing `express_relay-0.5.0/express_relay/express_relay_types.py` & `express_relay-0.6.0/express_relay/express_relay_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from enum import Enum
 from pydantic import BaseModel, model_validator
 from pydantic.functional_validators import AfterValidator
 from pydantic.functional_serializers import PlainSerializer
 from uuid import UUID
 import web3
 from typing import Union, ClassVar
@@ -140,14 +141,92 @@
             assert self.index is not None, "index must be a valid integer"
         elif self.bid_status == BidStatus("lost"):
             pass
         else:
             assert self.index is None, "index must be None"
         return self
 
+    @classmethod
+    def process_bid_status_dict(cls, bid_status_dict: dict):
+        """
+        Processes a bid status dictionary and converts to a class object.
+
+        Args:
+            bid_status_dict: The bid status dictionary to convert.
+
+        Returns:
+            The bid status as a class object.
+        """
+        try:
+            return cls.model_validate(
+                dict(
+                    id=bid_status_dict.get("id"),
+                    bid_status=bid_status_dict.get("bid_status", {}).pop("type"),
+                    **bid_status_dict.get("bid_status", {}),
+                )
+            )
+        except Exception as e:
+            warnings.warn(str(e))
+            return None
+
+
+class BidResponse(BaseModel):
+    """
+    Attributes:
+        id: The unique id for bid.
+        amount: The amount of the bid in wei.
+        target_calldata: Calldata for the contract call.
+        chain_id: The chain ID to bid on.
+        target_contract: The contract address to call.
+        permission_key: The permission key to bid on.
+        status: The latest status for bid.
+        initiation_time: The time server received the bid formatted in rfc3339.
+        profile_id: The profile id for the bid owner.
+    """
+
+    id: UUIDString
+    bid_amount: IntString
+    target_calldata: HexString
+    chain_id: str
+    target_contract: Address
+    permission_key: HexString
+    status: BidStatusUpdate
+    initiation_time: datetime
+    profile_id: str | None = Field(default=None)
+
+    @classmethod
+    def process_bid_response_dict(cls, bid_response_dict: dict):
+        """
+        Processes a bid response dictionary and converts to a class object.
+
+        Args:
+            bid_response_dict: The bid response dictionary to convert.
+
+        Returns:
+            The bid response as a class object.
+        """
+        try:
+            return cls.model_validate(
+                dict(
+                    status=BidStatusUpdate.process_bid_status_dict(
+                        dict(
+                            id=bid_response_dict.get("id"),
+                            bid_status=bid_response_dict.pop("status"),
+                        )
+                    ),
+                    initiation_time=datetime.fromisoformat(
+                        bid_response_dict.pop("initiation_time")
+                    ),
+                    **bid_response_dict,
+                )
+            )
+        except UnsupportedOpportunityVersionException as e:
+            warnings.warn(str(e))
+            return None
+
 
 class OpportunityBid(BaseModel):
     """
     Attributes:
         opportunity_id: The ID of the opportunity.
         amount: The amount of the bid in wei.
         executor: The address of the executor.
```

### Comparing `express_relay-0.5.0/express_relay/searcher/examples/simple_searcher.py` & `express_relay-0.6.0/express_relay/searcher/examples/simple_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,22 @@
 
 NAIVE_BID = 10
 # Set validity (naively) to max uint256
 VALID_UNTIL_MAX = 2**256 - 1
 
 
 class SimpleSearcher:
-    def __init__(self, server_url: str, private_key: Bytes32):
+    def __init__(
+        self, server_url: str, private_key: Bytes32, api_key: str | None = None
+    ):
         self.client = ExpressRelayClient(
-            server_url, self.opportunity_callback, self.bid_status_callback
+            server_url,
+            api_key,
+            self.opportunity_callback,
+            self.bid_status_callback,
         )
         self.private_key = private_key
         self.public_key = Account.from_key(private_key).address
 
     def assess_opportunity(
         self,
         opp: Opportunity,
@@ -81,15 +86,15 @@
         if bid_status == BidStatus("submitted") or bid_status == BidStatus("won"):
             result_details = f", transaction {result}, index {index} of multicall"
         elif bid_status == BidStatus("lost"):
             if result:
                 result_details = f", transaction {result}"
             if index:
                 result_details += f", index {index} of multicall"
-        logger.error(
+        logger.info(
             f"Bid status for bid {id}: {bid_status.value.replace('_', ' ')}{result_details}"
         )
 
 
 async def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-v", "--verbose", action="count", default=0)
@@ -108,26 +113,32 @@
     )
     parser.add_argument(
         "--server-url",
         type=str,
         required=True,
         help="Server endpoint to use for fetching opportunities and submitting bids",
     )
+    parser.add_argument(
+        "--api-key",
+        type=str,
+        required=False,
+        help="The API key of the searcher to authenticate with the server for fetching and submitting bids",
+    )
     args = parser.parse_args()
 
     logger.setLevel(logging.INFO if args.verbose == 0 else logging.DEBUG)
     log_handler = logging.StreamHandler()
     formatter = logging.Formatter(
         "%(asctime)s %(levelname)s:%(name)s:%(module)s %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
     log_handler.setFormatter(formatter)
     logger.addHandler(log_handler)
 
-    simple_searcher = SimpleSearcher(args.server_url, args.private_key)
+    simple_searcher = SimpleSearcher(args.server_url, args.private_key, args.api_key)
     logger.info("Searcher address: %s", simple_searcher.public_key)
 
     await simple_searcher.client.subscribe_chains(args.chain_ids)
 
     task = await simple_searcher.client.get_ws_loop()
     await task
```

### Comparing `express_relay-0.5.0/pyproject.toml` & `express_relay-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "express-relay"
-version = "0.5.0"
+version = "0.6.0"
 description = "Utilities for searchers and protocols to interact with the Express Relay protocol."
 authors = ["dourolabs"]
 license = "Proprietary"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `express_relay-0.5.0/PKG-INFO` & `express_relay-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-relay
-Version: 0.5.0
+Version: 0.6.0
 Summary: Utilities for searchers and protocols to interact with the Express Relay protocol.
 License: Proprietary
 Author: dourolabs
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

