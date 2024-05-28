# Comparing `tmp/nftpy-1.0.2.tar.gz` & `tmp/nftpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nftpy-1.0.2.tar", max compression
+gzip compressed data, was "nftpy-1.1.0.tar", max compression
```

## Comparing `nftpy-1.0.2.tar` & `nftpy-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1091 2024-05-27 01:41:06.348086 nftpy-1.0.2/LICENSE
--rw-r--r--   0        0        0      228 2024-05-27 01:42:48.914058 nftpy-1.0.2/nftpy/__init__.py
--rw-r--r--   0        0        0     1361 2024-05-27 01:41:06.351086 nftpy-1.0.2/nftpy/errors.py
--rw-r--r--   0        0        0      108 2024-05-27 01:41:06.349086 nftpy-1.0.2/nftpy/EVM/__init__.py
--rw-r--r--   0        0        0     9518 2024-05-27 01:41:06.350086 nftpy-1.0.2/nftpy/EVM/abi.py
--rw-r--r--   0        0        0     4346 2024-05-27 01:41:06.350086 nftpy-1.0.2/nftpy/EVM/chains.py
--rw-r--r--   0        0        0     6241 2024-05-27 01:41:06.350086 nftpy-1.0.2/nftpy/EVM/nft.py
--rw-r--r--   0        0        0     8490 2024-05-27 01:41:06.351086 nftpy-1.0.2/nftpy/opensea.py
--rw-r--r--   0        0        0      570 2024-05-27 01:57:09.605403 nftpy-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     8483 2024-05-27 01:41:06.349086 nftpy-1.0.2/README.md
--rw-r--r--   0        0        0     8931 1970-01-01 00:00:00.000000 nftpy-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-27 01:41:06.348086 nftpy-1.1.0/LICENSE
+-rw-r--r--   0        0        0      267 2024-05-27 21:04:09.914588 nftpy-1.1.0/nftpy/__init__.py
+-rw-r--r--   0        0        0     2669 2024-05-28 05:51:30.861326 nftpy-1.1.0/nftpy/errors.py
+-rw-r--r--   0        0        0      152 2024-05-27 20:44:18.057168 nftpy-1.1.0/nftpy/EVM/__init__.py
+-rw-r--r--   0        0        0    14009 2024-05-28 06:40:00.392465 nftpy-1.1.0/nftpy/EVM/abi.py
+-rw-r--r--   0        0        0     3142 2024-05-28 06:06:15.680338 nftpy-1.1.0/nftpy/EVM/chains.py
+-rw-r--r--   0        0        0     6286 2024-05-28 05:48:12.511059 nftpy-1.1.0/nftpy/EVM/nft.py
+-rw-r--r--   0        0        0     7437 2024-05-28 07:12:35.726905 nftpy-1.1.0/nftpy/EVM/wallet.py
+-rw-r--r--   0        0        0     8626 2024-05-28 05:47:40.676820 nftpy-1.1.0/nftpy/opensea.py
+-rw-r--r--   0        0        0      570 2024-05-27 21:04:09.909587 nftpy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12107 2024-05-28 07:41:41.952834 nftpy-1.1.0/README.md
+-rw-r--r--   0        0        0    12482 1970-01-01 00:00:00.000000 nftpy-1.1.0/PKG-INFO
```

### Comparing `nftpy-1.0.2/LICENSE` & `nftpy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nftpy-1.0.2/nftpy/EVM/abi.py` & `nftpy-1.1.0/nftpy/EVM/abi.py`

 * *Files 13% similar despite different names*

```diff
@@ -264,8 +264,132 @@
             "inputs": [
                 {"indexed": False, "name": "value", "type": "uint256"},
                 {"indexed": True, "name": "id", "type": "uint256"}
             ],
             "name": "URI",
             "type": "event"
         }
+    ],
+
+    OPENSEA_ERC1155 = [
+        {
+            "constant": True,
+            "inputs": [
+                {"name": "_owner", "type": "address"},
+                {"name": "_id", "type": "uint256"}
+            ],
+            "name": "balanceOf",
+            "outputs": [{"name": "balance", "type": "uint256"}],
+            "payable": False,
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "constant": True,
+            "inputs": [
+                {"name": "_owners", "type": "address[]"},
+                {"name": "_ids", "type": "uint256[]"}
+            ],
+            "name": "balanceOfBatch",
+            "outputs": [{"name": "balances", "type": "uint256[]"}],
+            "payable": False,
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "constant": False,
+            "inputs": [
+                {"name": "_from", "type": "address"},
+                {"name": "_to", "type": "address"},
+                {"name": "_id", "type": "uint256"},
+                {"name": "_value", "type": "uint256"},
+                {"name": "_data", "type": "bytes"}
+            ],
+            "name": "safeTransferFrom",
+            "outputs": [],
+            "payable": False,
+            "stateMutability": "nonpayable",
+            "type": "function"
+        },
+        {
+            "constant": False,
+            "inputs": [
+                {"name": "_from", "type": "address"},
+                {"name": "_to", "type": "address"},
+                {"name": "_ids", "type": "uint256[]"},
+                {"name": "_values", "type": "uint256[]"},
+                {"name": "_data", "type": "bytes"}
+            ],
+            "name": "safeBatchTransferFrom",
+            "outputs": [],
+            "payable": False,
+            "stateMutability": "nonpayable",
+            "type": "function"
+        },
+        {
+            "constant": False,
+            "inputs": [
+                {"name": "_operator", "type": "address"},
+                {"name": "_approved", "type": "bool"}
+            ],
+            "name": "setApprovalForAll",
+            "outputs": [],
+            "payable": False,
+            "stateMutability": "nonpayable",
+            "type": "function"
+        },
+        {
+            "constant": True,
+            "inputs": [
+                {"name": "_owner", "type": "address"},
+                {"name": "_operator", "type": "address"}
+            ],
+            "name": "isApprovedForAll",
+            "outputs": [{"name": "approved", "type": "bool"}],
+            "payable": False,
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "anonymous": False,
+            "inputs": [
+                {"indexed": True, "name": "operator", "type": "address"},
+                {"indexed": True, "name": "from", "type": "address"},
+                {"indexed": True, "name": "to", "type": "address"},
+                {"indexed": True, "name": "id", "type": "uint256"},
+                {"indexed": False, "name": "value", "type": "uint256"}
+            ],
+            "name": "TransferSingle",
+            "type": "event"
+        },
+        {
+            "anonymous": False,
+            "inputs": [
+                {"indexed": True, "name": "operator", "type": "address"},
+                {"indexed": True, "name": "from", "type": "address"},
+                {"indexed": True, "name": "to", "type": "address"},
+                {"indexed": True, "name": "ids", "type": "uint256[]"},
+                {"indexed": False, "name": "values", "type": "uint256[]"}
+            ],
+            "name": "TransferBatch",
+            "type": "event"
+        },
+        {
+            "anonymous": False,
+            "inputs": [
+                {"indexed": True, "name": "account", "type": "address"},
+                {"indexed": True, "name": "operator", "type": "address"},
+                {"indexed": False, "name": "approved", "type": "bool"}
+            ],
+            "name": "ApprovalForAll",
+            "type": "event"
+        },
+        {
+            "anonymous": False,
+            "inputs": [
+                {"indexed": False, "name": "value", "type": "uint256"},
+                {"indexed": True, "name": "id", "type": "uint256"}
+            ],
+            "name": "URI",
+            "type": "event"
+        }
     ]
```

### Comparing `nftpy-1.0.2/nftpy/EVM/chains.py` & `nftpy-1.1.0/nftpy/EVM/chains.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,32 +45,20 @@
     }
     MOONBEAM = {
         "chain_id": 1284,
         "name": "Moonbeam",
         "rpc_url": "https://rpc.api.moonbeam.network",
         "explorer_url": "https://moonscan.io"
     }
-    KLAYTN = {
-        "chain_id": 8217,
-        "name": "Klaytn",
-        "rpc_url": "https://public-node-api.klaytnapi.com/v1/cypress",
-        "explorer_url": "https://scope.klaytn.com"
-    }
     CELO = {
         "chain_id": 42220,
         "name": "Celo",
         "rpc_url": "https://forno.celo.org",
         "explorer_url": "https://explorer.celo.org"
     }
-    HECO = {
-        "chain_id": 128,
-        "name": "Huobi ECO Chain",
-        "rpc_url": "https://http-mainnet.hecochain.com",
-        "explorer_url": "https://hecoinfo.com"
-    }
     CRONOS = {
         "chain_id": 25,
         "name": "Cronos",
         "rpc_url": "https://evm-cronos.crypto.org",
         "explorer_url": "https://cronoscan.com"
     }
     METIS = {
@@ -87,53 +75,27 @@
     }
     RSK = {
         "chain_id": 30,
         "name": "Rootstock (RSK)",
         "rpc_url": "https://public-node.rsk.co",
         "explorer_url": "https://explorer.rsk.co"
     }
-    XDAI = {
-        "chain_id": 100,
-        "name": "Gnosis Chain (formerly xDai)",
-        "rpc_url": "https://rpc.xdaichain.com/",
-        "explorer_url": "https://blockscout.com/xdai/mainnet"
-    }
-    MUMBAI = {
-        "chain_id": 80001,
-        "name": "Mumbai",
-        "rpc_url": "https://rpc-mumbai.maticvigil.com",
-        "explorer_url": "https://mumbai.polygonscan.com"
-    }
-    GOERLI = {
-        "chain_id": 5,
-        "name": "Goerli",
-        "rpc_url": "https://rpc.goerli.mudit.blog",
-        "explorer_url": "https://goerli.etherscan.io"
-    }
     BASE = {
         "chain_id": 8453,
         "name": "Base",
         "rpc_url": "https://mainnet.base.org",
         "explorer_url": "https://basescan.org"
     }
-    BNB = {
-        "chain_id": 97,
-        "name": "BNB",
-        "rpc_url": "https://data-seed-prebsc-1-s1.binance.org:8545/",
-        "explorer_url": "https://testnet.bscscan.com"
-    }
-    SCROLL_ALPHA = {
-        "chain_id": 534353,
-        "name": "Scroll Alpha",
-        "rpc_url": "https://alpha-rpc.scroll.io/l2",
-        "explorer_url": "https://blockscout.scroll.io"
+    ETH_SEPOLIA = {
+        "chain_id": 11155111,
+        "name": "Sepolia Testnet",
+        "rpc_url": "https://rpc.sepolia.org",
+        "explorer_url": "https://sepolia.etherscan.io"
     }
 
-    # ADD CUSTOM CHAINS HERE
-
     @property
     def chain_id(self):
         return self.value["chain_id"]
 
     @property
     def name(self):
         return self.value["name"]
```

### Comparing `nftpy-1.0.2/nftpy/EVM/nft.py` & `nftpy-1.1.0/nftpy/EVM/nft.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,60 +36,60 @@
 
         Returns:
             int: The balance of tokens.
         """
         try:
             return self.contract.functions.balanceOf(wallet_address).call()
         except Exception as e:
-            raise ContractFunctionFailed('balanceOf') from e
+            raise ContractFunctionFailedError('balanceOf') from e
 
     def get_token_uri(self, token_id: int) -> str:
         """
         Get the URI of a specific token.
 
         Args:
             token_id (int): The ID of the token.
 
         Returns:
             str: The URI of the token.
         """
         try:
             return self.contract.functions.tokenURI(token_id).call()
         except Exception as e:
-            raise ContractFunctionFailed('tokenURI') from e
+            raise ContractFunctionFailedError('tokenURI') from e
 
     def get_owner(self, token_id: int) -> str:
         """
         Get the owner of a specific token.
 
         Args:
             token_id (int): The ID of the token.
 
         Returns:
             str: The address of the owner.
         """
         try:
             return self.contract.functions.ownerOf(token_id).call()
         except Exception as e:
-            raise ContractFunctionFailed('ownerOf') from e
+            raise ContractFunctionFailedError('ownerOf') from e
 
     def get_approved(self, token_id: int) -> str:
         """
         Get the approved address for a specific ERC721 token.
 
         Args:
             token_id (int): The ID of the token.
 
         Returns:
             str: The address that is approved for the token.
         """
         try:
             return self.contract.functions.getApproved(token_id).call()
         except Exception as e:
-            raise ContractFunctionFailed('getApproved') from e
+            raise ContractFunctionFailedError('getApproved') from e
 
     def is_approved_for_all(self, owner_address: str, operator_address: str) -> bool:
         """
         Check if an address is approved for all tokens owned by another address (ERC721).
 
         Args:
             owner_address (str): The address of the token owner.
@@ -97,15 +97,15 @@
 
         Returns:
             bool: True if the operator is approved for all tokens, False otherwise.
         """
         try:
             return self.contract.functions.isApprovedForAll(owner_address, operator_address).call()
         except Exception as e:
-            raise ContractFunctionFailed('isApprovedForAll') from e
+            raise ContractFunctionFailedError('isApprovedForAll') from e
 
     def get_token_metadata(self, token_id: int) -> dict:
         """
         Get the metadata for a specific ERC721 token.
         This assumes the tokenURI returns a URL that points to a JSON metadata file.
 
         Args:
@@ -115,15 +115,15 @@
             dict: The metadata of the token.
         """
         try:
             token_uri = self.get_token_uri(token_id)
             response = requests.get(token_uri)
             return response.json()
         except Exception as e:
-            raise ContractFunctionFailed('get_token_metadata') from e
+            raise ContractFunctionFailedError('get_token_metadata') from e
 
     def get_tokens_balance(self, wallet_address: str, token_ids: list) -> dict:
         """
         Get the balance of multiple ERC1155 tokens for a specific wallet address.
 
         Args:
             wallet_address (str): The address of the wallet.
@@ -132,15 +132,15 @@
         Returns:
             dict: A dictionary where the key is the token ID and the value is the balance.
         """
         try:
             balances = self.contract.functions.balanceOfBatch([wallet_address] * len(token_ids), token_ids).call()
             return {token_id: balance for token_id, balance in zip(token_ids, balances)}
         except Exception as e:
-            raise ContractFunctionFailed('balanceOfBatch') from e
+            raise ContractFunctionFailedError('balanceOfBatch') from e
 
     def is_approved_for_all_erc1155(self, owner_address: str, operator_address: str) -> bool:
         """
         Check if an address is approved for all tokens owned by another address (ERC1155).
 
         Args:
             owner_address (str): The address of the token owner.
@@ -148,15 +148,15 @@
 
         Returns:
             bool: True if the operator is approved for all tokens, False otherwise.
         """
         try:
             return self.contract.functions.isApprovedForAll(owner_address, operator_address).call()
         except Exception as e:
-            raise ContractFunctionFailed('isApprovedForAll') from e
+            raise ContractFunctionFailedError('isApprovedForAll') from e
 
     def get_token_balance(self, wallet_address: str, token_id: int) -> int:
         """
         Get the balance of a specific ERC1155 token for a specific wallet address.
 
         Args:
             wallet_address (str): The address of the wallet.
@@ -164,8 +164,8 @@
 
         Returns:
             int: The balance of the token.
         """
         try:
             return self.contract.functions.balanceOf(wallet_address, token_id).call()
         except Exception as e:
-            raise ContractFunctionFailed('balanceOf') from e
+            raise ContractFunctionFailedError('balanceOf') from e
```

### Comparing `nftpy-1.0.2/nftpy/opensea.py` & `nftpy-1.1.0/nftpy/opensea.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 from enum import Enum
-from errors import APIRequestFailed, MissingChain, MissingSlug
+from .errors import APIRequestFailedError, MissingChainError, MissingSlugError
 
 class OpenSeaChain(Enum):
     ETHEREUM = "ethereum"
     POLYGON = "polygon"
     KLAYTN = "klaytn"
     MUMBAI = "mumbai"
     GOERLI = "goerli"
@@ -20,30 +20,30 @@
         self.chain = chain
         self.collection_slug = collection_slug
         self.base_url = "https://api.opensea.io/api/v2"
 
     def get_collection_stats(self, collection_slug: str = None):
         collection_slug = collection_slug or self.collection_slug
         if collection_slug is None:
-            raise MissingSlug()
+            raise MissingSlugError()
         url = f"{self.base_url}/collection/{collection_slug}/stats"
         headers = {
             "Accept": "application/json",
             "X-API-KEY": self.api_key
         }
         response = requests.get(url, headers=headers)
         if response.status_code == 200:
             return response.json()
         else:
-            raise APIRequestFailed(response.status_code)
+            raise APIRequestFailedError(response.status_code)
 
     def list_events_by_nft(self, address: str, token_id: str, chain: OpenSeaChain = None, event_type: str = None, only_opensea: bool = False, auction_type: str = None, occurred_before: str = None, occurred_after: str = None, cursor: str = None, limit: int = 50):
         chain = chain or self.chain
         if chain is None:
-            raise MissingChain()
+            raise MissingChainError()
         url = f"{self.base_url}/events/chain/{chain.value}/contract/{address}/nfts/{token_id}"
         headers = {
             "Accept": "application/json",
             "X-API-KEY": self.api_key
         }
         params = {
             "event_type": event_type,
@@ -54,165 +54,165 @@
             "cursor": cursor,
             "limit": limit
         }
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:
             return response.json()
         else:
-            raise APIRequestFailed(response.status_code)
+            raise APIRequestFailedError(response.status_code)
 
     def get_collection(self, collection_slug: str = None):
         collection_slug = collection_slug or self.collection_slug
         if collection_slug is None:
-            raise MissingSlug()
+            raise MissingSlugError()
         url = f"{self.base_url}/collection/{collection_slug}"
         headers = {
             "Accept": "application/json",
             "X-API-KEY": self.api_key
         }
         response = requests.get(url, headers=headers)
         if response.status_code == 200:
             return response.json()
         else:
-            raise APIRequestFailed(response.status_code)
+            raise APIRequestFailedError(response.status_code)
 
     def get_contract(self, address: str, chain: OpenSeaChain = None):
         chain = chain or self.chain
         if chain is None:
-            raise MissingChain()
+            raise MissingChainError()
         url = f"{self.base_url}/chain/{chain.value}/contract/{address}"
         headers = {
             "Accept": "application/json",
             "X-API-KEY": self.api_key
         }
         response = requests.get(url, headers=headers)
         if response.status_code == 200:
             return response.json()
         else:
-            raise APIRequestFailed(response.status_code)
+            raise APIRequestFailedError(response.status_code)
 
     def get_nft(self, address: str, token_id: str, chain: OpenSeaChain = None):
         chain = chain or self.chain
         if chain is None:
-            raise MissingChain()
+            raise MissingChainError()
         url = f"{self.base_url}/chain/{chain.value}/contract/{address}/nfts/{token_id}"
         headers = {
             "Accept": "application/json",
             "X-API-KEY": self.api_key
         }
         response = requests.get(url, headers=headers)
         if response.status_code == 200:
             return response.json()
         else:
-            raise APIRequestFailed(response.status_code)
+            raise APIRequestFailedError(response.status_code)
 
     def list_nfts_by_account(self, address: str, chain: OpenSeaChain = None, cursor: str = None, limit: int = 50):
         chain = chain or self.chain
         if chain is None:
-            raise MissingChain()
+            raise MissingChainError()
         url = f"{self.base_url}/chain/{chain.value}/account/{address}/nfts"
         headers = {
             "Accept": "application/json",
             "X-API-KEY": self.api_key
         }
         params = {
             "cursor": cursor,
             "limit": limit
         }
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:
             return response.json()
         else:
-            raise APIRequestFailed(response.status_code)
+            raise APIRequestFailedError(response.status_code)
 
     def list_nfts_by_collection(self, collection_slug: str = None, chain: OpenSeaChain = None, cursor: str = None, limit: int = 50):
         collection_slug = collection_slug or self.collection_slug
         chain = chain or self.chain
         if collection_slug is None:
-            raise MissingSlug()
+            raise MissingSlugError()
         if chain is None:
-            raise MissingChain()
+            raise MissingChainError()
         url = f"{self.base_url}/chain/{chain.value}/collection/{collection_slug}/nfts"
         headers = {
             "Accept": "application/json",
             "X-API-KEY": self.api_key
         }
         params = {
             "cursor": cursor,
             "limit": limit
         }
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:
             return response.json()
         else:
-            raise APIRequestFailed(response.status_code)
+            raise APIRequestFailedError(response.status_code)
 
     def list_nfts_by_contract(self, contract_address: str, chain: OpenSeaChain = None, cursor: str = None, limit: int = 50):
         chain = chain or self.chain
         if chain is None:
-            raise MissingChain()
+            raise MissingChainError()
         url = f"{self.base_url}/chain/{chain.value}/contract/{contract_address}/nfts"
         headers = {
             "Accept": "application/json",
             "X-API-KEY": self.api_key
         }
         params = {
             "cursor": cursor,
             "limit": limit
         }
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:
             return response.json()
         else:
-            raise APIRequestFailed(response.status_code)
+            raise APIRequestFailedError(response.status_code)
 
     def get_payment_token(self, address: str, chain: OpenSeaChain = None):
         chain = chain or self.chain
         if chain is None:
-            raise MissingChain()
+            raise MissingChainError()
         url = f"{self.base_url}/chain/{chain.value}/payment_token/{address}"
         headers = {
             "Accept": "application/json",
             "X-API-KEY": self.api_key
         }
         response = requests.get(url, headers=headers)
         if response.status_code == 200:
             return response.json()
         else:
-            raise APIRequestFailed(response.status_code)
+            raise APIRequestFailedError(response.status_code)
 
     def get_traits(self, collection_slug: str = None):
         collection_slug = collection_slug or self.collection_slug
         if collection_slug is None:
-            raise MissingSlug()
+            raise MissingSlugError()
         url = f"{self.base_url}/collection/{collection_slug}/traits"
         headers = {
             "Accept": "application/json",
             "X-API-KEY": self.api_key
         }
         response = requests.get(url, headers=headers)
         if response.status_code == 200:
             return response.json()
         else:
-            raise APIRequestFailed(response.status_code)
+            raise APIRequestFailedError(response.status_code)
 
     def get_all_listings_on_collection(self, collection_slug: str = None, chain: OpenSeaChain = None, cursor: str = None, limit: int = 50):
         collection_slug = collection_slug or self.collection_slug
         chain = chain or self.chain
         if collection_slug is None:
-            raise MissingSlug()
+            raise MissingSlugError()
         if chain is None:
-            raise MissingChain()
+            raise MissingChainError()
         url = f"{self.base_url}/chain/{chain.value}/collection/{collection_slug}/listings"
         headers = {
             "Accept": "application/json",
             "X-API-KEY": self.api_key
         }
         params = {
             "cursor": cursor,
             "limit": limit
         }
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:
             return response.json()
         else:
-            raise APIRequestFailed(response.status_code)
+            raise APIRequestFailedError(response.status_code)
```

### Comparing `nftpy-1.0.2/pyproject.toml` & `nftpy-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nftpy"
-version = "1.0.2"
+version = "1.1.0"
 description = "A NFT specific Python library for easy NFT integration in Python"
 authors = ["CoulterStutz <coultercash@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/coulterstutz/nftpy"
 repository = "https://github.com/coulterstutz/nftpy"
```

### Comparing `nftpy-1.0.2/PKG-INFO` & `nftpy-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nftpy
-Version: 1.0.2
+Version: 1.1.0
 Summary: A NFT specific Python library for easy NFT integration in Python
 Home-page: https://github.com/coulterstutz/nftpy
 License: MIT
 Author: CoulterStutz
 Author-email: coultercash@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: web3 (>=6.2.0,<7.0.0)
 Project-URL: Repository, https://github.com/coulterstutz/nftpy
 Description-Content-Type: text/markdown
 
 # NFTPy
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.0-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.1-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
 [![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
 
 A Python package designed to facilitate the integration and adoption of NFT (ERC721, ERC1155) tokens in software applications.
 
 ## Features
 
 #### EVM Interaction with NFT Tokens
@@ -34,27 +34,41 @@
 - **get_approved**: Get the approved address for a specific ERC721 token.
 - **is_approved_for_all**: Check if an address is approved for all tokens owned by another address (ERC721).
 - **get_token_metadata**: Get the metadata for a specific ERC721 token.
 - **get_token_balance**: Get the balance of a specific ERC1155 token for a specific wallet address.
 - **get_tokens_balance**: Gets the balance of a specific list of tokens.
 - **is_approved_for_all_erc1155**: Check if an address is approved for all tokens owned by another address (ERC1155).
 
+#### EVM Wallet Interaction
+NFTPy includes comprehensive features for interacting with Ethereum wallets, including querying balances, fetching gas prices, and transferring NFTs. The wallet interface supports both read-only and transactional operations.
+
+**Wallet Features:**
+- **get_balance**: Retrieve the balance of NFTs for a given address in Ether.
+- **get_balance_wei**: Retrieve the balance of NFTs for a given address in Wei.
+- **get_gas_price_wei**: Fetch the current gas price in Wei.
+- **get_gas_price_gwei**: Fetch the current gas price in Gwei.
+- **transfer_nft**: Transfer an NFT from the wallet to another address.
+
 #### Built-in OpenSea Interface
 ![OpenSea Support](https://img.shields.io/badge/OpenSea-%232081E2.svg?style=for-the-badge&logo=opensea&logoColor=white)
 
 NFTPy includes a built-in interface for interacting with OpenSea via an API key. This allows for in-package queries to OpenSea, enabling access to pricing information and other OpenSea-specific data. The OpenSea interface can be configured to focus on a single collection or query multiple collections. The available methods include:
 
+- **get_collection_stats**: Obtain statistics for a collection.
+- **list_events_by_nft**: List events related to a specific NFT.
 - **get_collection**: Fetch details of a specific collection.
 - **get_contract**: Retrieve details of a specific contract.
 - **get_nft**: Get details of a specific NFT.
-- **get_collection_stats**: Obtain statistics for a collection.
-- **list_events_by_nft**: List events related to a specific NFT.
 - **list_nfts_by_account**: List NFTs owned by a specific account.
 - **list_nfts_by_collection**: List NFTs in a specific collection.
 - **list_nfts_by_contract**: List NFTs under a specific contract.
+- **get_payment_token**: Get details of a specific payment token.
+- **get_traits**: Get traits of a specific collection.
+- **get_all_listings_on_collection**: Get all listings of a specific collection.
+
 
 # Example Usage
 ### Interacting on-chain with a collection | NFTPy.EVM.NFT
 Using NFTPy.EVM.NFT we are going to be querying the Pixelmon NFT collection on Ethereum mainnet!
 We will first start off by creating our class. We are going to define our class with three arguments:
 - contract_address: The address of the contract you are trying to query.
 - abi: The ABI of the contract you are trying to query. The EVM.ABI class provides presets for our ABI. You can also paste an ABI into the field.
@@ -116,14 +130,73 @@
 tokens_balance = erc1155_nft.get_tokens(wallet_address, token_ids)
 print(f'Tokens Balance: {tokens_balance}')
 
 # Check if an address is approved for all tokens (ERC1155)
 is_approved_erc1155 = erc1155_nft.is_approved_for_all_erc1155(wallet_address, '0xOperatorAddress')
 print(f'Is Approved For All (ERC1155): {is_approved_erc1155}')
 ```
+
+### Interacting with a Wallet | NFTPy.NFTWallet
+#### Sending a Transaction with Private Key
+Creating an instance of `NFTWallet` requires either a private key for full access or just an address for read-only access. You can also specify multiple chains to connect to different networks simultaneously.
+
+```python
+from nftpy import *
+
+# Initialize the wallet with a private key and specify chains
+wallet = NFTWallet(private_key="your_private_key", chains=[Chains.ETH_SEPOLIA])
+
+# Get the balance of the wallet in Ether
+print(wallet.get_balance()) 
+# Output: {"Balances": {'Sepolia Testnet': Decimal('1.234567890123456789')}}
+
+# Get the balance of the wallet in Wei
+print(wallet.get_balance_wei()) 
+# Output: {"Balances": {'Sepolia Testnet': 1234567890123456789}}
+
+# Get the current gas price in Wei
+print(wallet.get_gas_price_wei()) 
+# Output: {'Sepolia Testnet': 30000000000}
+
+# Get the current gas price in Gwei
+print(wallet.get_gas_price_gwei()) 
+# Output: {'Sepolia Testnet': Decimal('30')}
+
+# Transfer an NFT to another wallet
+to_wallet = "0xb1234567890abcdef1234567890abcdef1234567"
+contract = "0xabcdefabcdefabcdefabcdefabcdefabcdefabcdef"
+gas_price = wallet.get_gas_price_gwei()["Sepolia Testnet"]
+gas_limit = 70000   # Disclaimer! Gas Limit set for Sepolia, WILL fail on other networks
+
+# Transfer the NFT and get the transaction hash and explorer URL
+print(wallet.transfer_nft(to=to_wallet, contract_address=contract, amount=1, gas_limit=gas_limit,
+                          gas_price_gwei=gas_price, abi=ABI.OPENSEA_ERC1155, token_id=1))
+# Output: {'transaction_hash': '0xabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdef', 'explorer_url': 'https://sepolia.etherscan.io/tx/0xabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdef'}
+```
+#### Read-Only Wallets
+When using a read-only address (i.e., only providing an address and not a private key), you can still interact with the blockchain to query information, but you will not be able to perform transactions. This is useful for monitoring wallets and retrieving data without the need for sensitive credentials.
+```python
+from nftpy import *
+
+# Initialize the wallet with an address and specify chains
+readonly_wallet = NFTWallet(address="0xYourReadOnlyWalletAddress", chains=[Chains.ETH_SEPOLIA])
+
+# Get the balance of the wallet in Ether
+print(readonly_wallet.get_balance()) 
+# Output: {"Balances": {'Sepolia Testnet': Decimal('0.123456789012345678')}}
+
+# Get the balance of the wallet in Wei
+print(readonly_wallet.get_balance_wei()) 
+# Output: {"Balances": {'Sepolia Testnet': 123456789012345678}}
+
+# Get the current gas price in Wei
+print(readonly_wallet.get_gas_price_wei()) 
+# Output: {'Sepolia Testnet': 20000000000}
+```
+
 ### Interacting with OpenSea API | NFTPy.OpenSea
 We will first start by creating our class with the following arguments:
 - api_key: Your OpenSea API key.
 - chain: The blockchain network (e.g., Ethereum, Polygon).
 - collection_slug: The slug of the collection you want to query (the last part of the url when browsing the collection on opensea) This assigns the interface to a specific collection. If you are using the interface to view multiple collections then you should leave this blank
 
 **Please Note**: When defining the chain, it should be done with NFTPy.OpenSea.Chain as the api requires a special format for chain definition
```

