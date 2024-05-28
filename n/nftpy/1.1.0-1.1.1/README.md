# Comparing `tmp/nftpy-1.1.0.tar.gz` & `tmp/nftpy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nftpy-1.1.0.tar", max compression
+gzip compressed data, was "nftpy-1.1.1.tar", max compression
```

## Comparing `nftpy-1.1.0.tar` & `nftpy-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1091 2024-05-27 01:41:06.348086 nftpy-1.1.0/LICENSE
--rw-r--r--   0        0        0      267 2024-05-27 21:04:09.914588 nftpy-1.1.0/nftpy/__init__.py
--rw-r--r--   0        0        0     2669 2024-05-28 05:51:30.861326 nftpy-1.1.0/nftpy/errors.py
--rw-r--r--   0        0        0      152 2024-05-27 20:44:18.057168 nftpy-1.1.0/nftpy/EVM/__init__.py
--rw-r--r--   0        0        0    14009 2024-05-28 06:40:00.392465 nftpy-1.1.0/nftpy/EVM/abi.py
--rw-r--r--   0        0        0     3142 2024-05-28 06:06:15.680338 nftpy-1.1.0/nftpy/EVM/chains.py
--rw-r--r--   0        0        0     6286 2024-05-28 05:48:12.511059 nftpy-1.1.0/nftpy/EVM/nft.py
--rw-r--r--   0        0        0     7437 2024-05-28 07:12:35.726905 nftpy-1.1.0/nftpy/EVM/wallet.py
--rw-r--r--   0        0        0     8626 2024-05-28 05:47:40.676820 nftpy-1.1.0/nftpy/opensea.py
--rw-r--r--   0        0        0      570 2024-05-27 21:04:09.909587 nftpy-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    12107 2024-05-28 07:41:41.952834 nftpy-1.1.0/README.md
--rw-r--r--   0        0        0    12482 1970-01-01 00:00:00.000000 nftpy-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-27 01:41:06.348086 nftpy-1.1.1/LICENSE
+-rw-r--r--   0        0        0      269 2024-05-28 08:15:32.289802 nftpy-1.1.1/nftpy/__init__.py
+-rw-r--r--   0        0        0     2669 2024-05-28 05:51:30.861326 nftpy-1.1.1/nftpy/errors.py
+-rw-r--r--   0        0        0      152 2024-05-27 20:44:18.057168 nftpy-1.1.1/nftpy/EVM/__init__.py
+-rw-r--r--   0        0        0    14009 2024-05-28 06:40:00.392465 nftpy-1.1.1/nftpy/EVM/abi.py
+-rw-r--r--   0        0        0     3142 2024-05-28 06:06:15.680338 nftpy-1.1.1/nftpy/EVM/chains.py
+-rw-r--r--   0        0        0     6286 2024-05-28 05:48:12.511059 nftpy-1.1.1/nftpy/EVM/nft.py
+-rw-r--r--   0        0        0     7534 2024-05-28 08:10:02.369569 nftpy-1.1.1/nftpy/EVM/wallet.py
+-rw-r--r--   0        0        0     8626 2024-05-28 05:47:40.676820 nftpy-1.1.1/nftpy/opensea.py
+-rw-r--r--   0        0        0      570 2024-05-28 08:12:47.554479 nftpy-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12704 2024-05-28 08:20:29.669317 nftpy-1.1.1/README.md
+-rw-r--r--   0        0        0    13069 1970-01-01 00:00:00.000000 nftpy-1.1.1/PKG-INFO
```

### Comparing `nftpy-1.1.0/LICENSE` & `nftpy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.0/nftpy/errors.py` & `nftpy-1.1.1/nftpy/errors.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.0/nftpy/EVM/abi.py` & `nftpy-1.1.1/nftpy/EVM/abi.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.0/nftpy/EVM/chains.py` & `nftpy-1.1.1/nftpy/EVM/chains.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.0/nftpy/EVM/nft.py` & `nftpy-1.1.1/nftpy/EVM/nft.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.0/nftpy/EVM/wallet.py` & `nftpy-1.1.1/nftpy/EVM/wallet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+import time
+
 from web3 import Web3
+from web3.exceptions import TransactionNotFound
+
 from .abi import ABI
 from .chains import Chains
 from ..errors import *
 
 class NFTWallet:
     def __init__(self, private_key: str = None, address: str = None, chains: list[Chains] = None, rpc_url: str = None):
         if not private_key and not address:
@@ -129,15 +133,15 @@
         elif abi_str is not None:
             contract_abi = abi_str
         else:
             raise ValueError("Either abi or abi_str must be provided.")
 
         contract = conn.eth.contract(address=contract_address, abi=contract_abi)
 
-        nonce = conn.eth.getTransactionCount(self._address)
+        nonce = conn.eth.get_transaction_count(self._address)
         tx = {
             'nonce': nonce,
             'to': contract_address,
             'value': 0,
             'gas': gas_limit,
             'gasPrice': gas_price,
             'data': contract.functions.safeTransferFrom(self._address, to, token_id, amount, b'').build_transaction({
@@ -158,22 +162,23 @@
             if 'gas' in str(e):
                 raise TransactionGasError()
             elif 'balance' in str(e):
                 raise TransactionBalanceError()
             else:
                 raise e
 
-        signed_tx = conn.eth.account.sign_transaction(tx, private_key=self._private_key)
+    def wait_until_transaction_processes(self, tx_hash, chain: Chains) -> bool:
+        if isinstance(tx_hash, str):
+            tx_hash = Web3.to_bytes(hexstr=tx_hash)
 
-        try:
-            tx_hash = conn.eth.send_raw_transaction(signed_tx.rawTransaction)
-            return {
-                'transaction_hash': tx_hash.hex(),
-                'explorer_url': f"{chain.explorer_url}/tx/{tx_hash.hex()}"
-            }
-        except ValueError as e:
-            if 'gas' in str(e):
-                raise TransactionGasError()
-            elif 'balance' in str(e):
-                raise TransactionBalanceError()
-            else:
-                raise e
+        conn = Web3(Web3.HTTPProvider(chain.rpc_url))
+        if not conn.is_connected():
+            raise InvalidRPCURL(chain.rpc_url, chain.name)
+
+        while True:
+            try:
+                receipt = conn.eth.get_transaction_receipt(tx_hash)
+                if receipt is not None and receipt.status == 1:
+                    return True
+            except TransactionNotFound:
+                pass
+            time.sleep(1)
```

### Comparing `nftpy-1.1.0/nftpy/opensea.py` & `nftpy-1.1.1/nftpy/opensea.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.0/pyproject.toml` & `nftpy-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nftpy"
-version = "1.1.0"
+version = "1.1.1"
 description = "A NFT specific Python library for easy NFT integration in Python"
 authors = ["CoulterStutz <coultercash@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/coulterstutz/nftpy"
 repository = "https://github.com/coulterstutz/nftpy"
```

### Comparing `nftpy-1.1.0/README.md` & `nftpy-1.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # NFTPy
-[![PyPi](https://img.shields.io/badge/PyPi-1.1-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.1.1-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
 [![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
 
 A Python package designed to facilitate the integration and adoption of NFT (ERC721, ERC1155) tokens in software applications.
 
 ## Features
 
 #### EVM Interaction with NFT Tokens
@@ -26,14 +26,15 @@
 
 **Wallet Features:**
 - **get_balance**: Retrieve the balance of NFTs for a given address in Ether.
 - **get_balance_wei**: Retrieve the balance of NFTs for a given address in Wei.
 - **get_gas_price_wei**: Fetch the current gas price in Wei.
 - **get_gas_price_gwei**: Fetch the current gas price in Gwei.
 - **transfer_nft**: Transfer an NFT from the wallet to another address.
+- **wait_until_transaction_processes**: Delays the program until the transaction has fully processed in the blockchain
 
 #### Built-in OpenSea Interface
 ![OpenSea Support](https://img.shields.io/badge/OpenSea-%232081E2.svg?style=for-the-badge&logo=opensea&logoColor=white)
 
 NFTPy includes a built-in interface for interacting with OpenSea via an API key. This allows for in-package queries to OpenSea, enabling access to pricing information and other OpenSea-specific data. The OpenSea interface can be configured to focus on a single collection or query multiple collections. The available methods include:
 
 - **get_collection_stats**: Obtain statistics for a collection.
@@ -115,50 +116,59 @@
 
 # Check if an address is approved for all tokens (ERC1155)
 is_approved_erc1155 = erc1155_nft.is_approved_for_all_erc1155(wallet_address, '0xOperatorAddress')
 print(f'Is Approved For All (ERC1155): {is_approved_erc1155}')
 ```
 
 ### Interacting with a Wallet | NFTPy.NFTWallet
-#### Sending a Transaction with Private Key
+
 Creating an instance of `NFTWallet` requires either a private key for full access or just an address for read-only access. You can also specify multiple chains to connect to different networks simultaneously.
 
 ```python
 from nftpy import *
 
 # Initialize the wallet with a private key and specify chains
-wallet = NFTWallet(private_key="your_private_key", chains=[Chains.ETH_SEPOLIA])
+wallet = NFTWallet(private_key="0x9015a0eb4c1ceab5f5544ac6e0a75eabb37d7dec26f1dfcb09adb43632330736", chains=[Chains.ETH_SEPOLIA])
 
 # Get the balance of the wallet in Ether
 print(wallet.get_balance()) 
-# Output: {"Balances": {'Sepolia Testnet': Decimal('1.234567890123456789')}}
+# Output: {"Balances": {'Sepolia Testnet': Decimal('0.8341469847291797')}}
 
 # Get the balance of the wallet in Wei
 print(wallet.get_balance_wei()) 
-# Output: {"Balances": {'Sepolia Testnet': 1234567890123456789}}
+# Output: {"Balances": {'Sepolia Testnet': 834146984729179700}}
 
 # Get the current gas price in Wei
 print(wallet.get_gas_price_wei()) 
-# Output: {'Sepolia Testnet': 30000000000}
+# Output: {'Sepolia Testnet': 20000000000}
 
 # Get the current gas price in Gwei
 print(wallet.get_gas_price_gwei()) 
-# Output: {'Sepolia Testnet': Decimal('30')}
+# Output: {'Sepolia Testnet': Decimal('20')}
 
 # Transfer an NFT to another wallet
-to_wallet = "0xb1234567890abcdef1234567890abcdef1234567"
-contract = "0xabcdefabcdefabcdefabcdefabcdefabcdefabcdef"
+to_wallet = "0xa693190103733280E23055BE70C838d9b6708b9a"
+contract = "0x725Ea5eEA79F1515e34A921b83D4307b325cC8b9"
 gas_price = wallet.get_gas_price_gwei()["Sepolia Testnet"]
-gas_limit = 70000   # Disclaimer! Gas Limit set for Sepolia, WILL fail on other networks
+gas_limit = 65000   # Disclaimer! Gas Limit set for Sepolia, WILL fail on other networks
 
 # Transfer the NFT and get the transaction hash and explorer URL
 print(wallet.transfer_nft(to=to_wallet, contract_address=contract, amount=1, gas_limit=gas_limit,
                           gas_price_gwei=gas_price, abi=ABI.OPENSEA_ERC1155, token_id=1))
-# Output: {'transaction_hash': '0xabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdef', 'explorer_url': 'https://sepolia.etherscan.io/tx/0xabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdef'}
+# Output: {'transaction_hash': '0x18a076a4a30c1cc014b1620aa907db06a04e8a709bda47e9beed2233a23f532f', 'explorer_url': 'https://sepolia.etherscan.io/tx/0x18a076a4a30c1cc014b1620aa907db06a04e8a709bda47e9beed2233a23f532f'}
+```
+#### Waiting For The Transaction To Process
+After we get the transaction hash, we can have the program delay until the transaction processes on the blockchain.
+```python
+# Wait until the transaction is processed
+transaction_hash = "0xcd74c93bbf42cae24f329c45da995bde7e1c89ea848855d04db516c6460eda02"
+print(wallet.wait_until_transaction_processes(transaction_hash, chain=Chains.ETH_SEPOLIA))
+# Output: True | When the transaction fully processes on the blockchain
 ```
+
 #### Read-Only Wallets
 When using a read-only address (i.e., only providing an address and not a private key), you can still interact with the blockchain to query information, but you will not be able to perform transactions. This is useful for monitoring wallets and retrieving data without the need for sensitive credentials.
 ```python
 from nftpy import *
 
 # Initialize the wallet with an address and specify chains
 readonly_wallet = NFTWallet(address="0xYourReadOnlyWalletAddress", chains=[Chains.ETH_SEPOLIA])
```

### Comparing `nftpy-1.1.0/PKG-INFO` & `nftpy-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nftpy
-Version: 1.1.0
+Version: 1.1.1
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
-[![PyPi](https://img.shields.io/badge/PyPi-1.1-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.1.1-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
 [![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
 
 A Python package designed to facilitate the integration and adoption of NFT (ERC721, ERC1155) tokens in software applications.
 
 ## Features
 
 #### EVM Interaction with NFT Tokens
@@ -43,14 +43,15 @@
 
 **Wallet Features:**
 - **get_balance**: Retrieve the balance of NFTs for a given address in Ether.
 - **get_balance_wei**: Retrieve the balance of NFTs for a given address in Wei.
 - **get_gas_price_wei**: Fetch the current gas price in Wei.
 - **get_gas_price_gwei**: Fetch the current gas price in Gwei.
 - **transfer_nft**: Transfer an NFT from the wallet to another address.
+- **wait_until_transaction_processes**: Delays the program until the transaction has fully processed in the blockchain
 
 #### Built-in OpenSea Interface
 ![OpenSea Support](https://img.shields.io/badge/OpenSea-%232081E2.svg?style=for-the-badge&logo=opensea&logoColor=white)
 
 NFTPy includes a built-in interface for interacting with OpenSea via an API key. This allows for in-package queries to OpenSea, enabling access to pricing information and other OpenSea-specific data. The OpenSea interface can be configured to focus on a single collection or query multiple collections. The available methods include:
 
 - **get_collection_stats**: Obtain statistics for a collection.
@@ -132,50 +133,59 @@
 
 # Check if an address is approved for all tokens (ERC1155)
 is_approved_erc1155 = erc1155_nft.is_approved_for_all_erc1155(wallet_address, '0xOperatorAddress')
 print(f'Is Approved For All (ERC1155): {is_approved_erc1155}')
 ```
 
 ### Interacting with a Wallet | NFTPy.NFTWallet
-#### Sending a Transaction with Private Key
+
 Creating an instance of `NFTWallet` requires either a private key for full access or just an address for read-only access. You can also specify multiple chains to connect to different networks simultaneously.
 
 ```python
 from nftpy import *
 
 # Initialize the wallet with a private key and specify chains
-wallet = NFTWallet(private_key="your_private_key", chains=[Chains.ETH_SEPOLIA])
+wallet = NFTWallet(private_key="0x9015a0eb4c1ceab5f5544ac6e0a75eabb37d7dec26f1dfcb09adb43632330736", chains=[Chains.ETH_SEPOLIA])
 
 # Get the balance of the wallet in Ether
 print(wallet.get_balance()) 
-# Output: {"Balances": {'Sepolia Testnet': Decimal('1.234567890123456789')}}
+# Output: {"Balances": {'Sepolia Testnet': Decimal('0.8341469847291797')}}
 
 # Get the balance of the wallet in Wei
 print(wallet.get_balance_wei()) 
-# Output: {"Balances": {'Sepolia Testnet': 1234567890123456789}}
+# Output: {"Balances": {'Sepolia Testnet': 834146984729179700}}
 
 # Get the current gas price in Wei
 print(wallet.get_gas_price_wei()) 
-# Output: {'Sepolia Testnet': 30000000000}
+# Output: {'Sepolia Testnet': 20000000000}
 
 # Get the current gas price in Gwei
 print(wallet.get_gas_price_gwei()) 
-# Output: {'Sepolia Testnet': Decimal('30')}
+# Output: {'Sepolia Testnet': Decimal('20')}
 
 # Transfer an NFT to another wallet
-to_wallet = "0xb1234567890abcdef1234567890abcdef1234567"
-contract = "0xabcdefabcdefabcdefabcdefabcdefabcdefabcdef"
+to_wallet = "0xa693190103733280E23055BE70C838d9b6708b9a"
+contract = "0x725Ea5eEA79F1515e34A921b83D4307b325cC8b9"
 gas_price = wallet.get_gas_price_gwei()["Sepolia Testnet"]
-gas_limit = 70000   # Disclaimer! Gas Limit set for Sepolia, WILL fail on other networks
+gas_limit = 65000   # Disclaimer! Gas Limit set for Sepolia, WILL fail on other networks
 
 # Transfer the NFT and get the transaction hash and explorer URL
 print(wallet.transfer_nft(to=to_wallet, contract_address=contract, amount=1, gas_limit=gas_limit,
                           gas_price_gwei=gas_price, abi=ABI.OPENSEA_ERC1155, token_id=1))
-# Output: {'transaction_hash': '0xabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdef', 'explorer_url': 'https://sepolia.etherscan.io/tx/0xabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdefabcdef'}
+# Output: {'transaction_hash': '0x18a076a4a30c1cc014b1620aa907db06a04e8a709bda47e9beed2233a23f532f', 'explorer_url': 'https://sepolia.etherscan.io/tx/0x18a076a4a30c1cc014b1620aa907db06a04e8a709bda47e9beed2233a23f532f'}
+```
+#### Waiting For The Transaction To Process
+After we get the transaction hash, we can have the program delay until the transaction processes on the blockchain.
+```python
+# Wait until the transaction is processed
+transaction_hash = "0xcd74c93bbf42cae24f329c45da995bde7e1c89ea848855d04db516c6460eda02"
+print(wallet.wait_until_transaction_processes(transaction_hash, chain=Chains.ETH_SEPOLIA))
+# Output: True | When the transaction fully processes on the blockchain
 ```
+
 #### Read-Only Wallets
 When using a read-only address (i.e., only providing an address and not a private key), you can still interact with the blockchain to query information, but you will not be able to perform transactions. This is useful for monitoring wallets and retrieving data without the need for sensitive credentials.
 ```python
 from nftpy import *
 
 # Initialize the wallet with an address and specify chains
 readonly_wallet = NFTWallet(address="0xYourReadOnlyWalletAddress", chains=[Chains.ETH_SEPOLIA])
```

