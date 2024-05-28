# Comparing `tmp/contextooor-0.9.9.9.tar.gz` & `tmp/contextooor-0.9.9.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contextooor-0.9.9.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "contextooor-0.9.9.92.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `contextooor-0.9.9.9.tar` & `contextooor-0.9.9.92.tar`

### file list

```diff
@@ -1,33 +1,22 @@
--rw-r--r--   0        0        0       72 2024-05-27 17:04:45.134848 contextooor-0.9.9.9/.gitignore
--rw-r--r--   0        0        0    71515 2024-03-14 15:04:16.974143 contextooor-0.9.9.9/Cargo.lock
--rw-r--r--   0        0        0      334 2024-03-14 15:07:01.741088 contextooor-0.9.9.9/Cargo.toml
--rw-r--r--   0        0        0    10457 2024-01-31 18:27:21.928630 contextooor-0.9.9.9/btc_sanctioned_addresses.parquet
--rw-r--r--   0        0        0    51376 2024-05-06 20:31:27.436460 contextooor-0.9.9.9/coingecko.parquet
-drwxr-xr-x   0        0        0        0 2024-05-27 17:07:21.907443 contextooor-0.9.9.9/contextooor/
--rw-r--r--   0        0        0     4552 2024-03-12 15:15:26.385216 contextooor-0.9.9.9/contextooor/README.md
--rw-r--r--   0        0        0       95 2024-05-27 16:52:39.962528 contextooor-0.9.9.9/contextooor/__init__.py
--rw-r--r--   0        0        0     6285 2024-02-15 15:30:15.619991 contextooor-0.9.9.9/contextooor/btc.py
--rw-r--r--   0        0        0     2055 2024-05-27 17:07:21.906738 contextooor-0.9.9.9/contextooor/core/Chainalysis/chainalysis_ofac_api.py
--rw-r--r--   0        0        0    29738 2023-12-23 03:26:26.687369 contextooor-0.9.9.9/contextooor/core/V2_router/V2_router.py
--rw-r--r--   0        0        0    28278 2023-12-23 03:26:26.691166 contextooor-0.9.9.9/contextooor/core/V3_router/V3_router.py
--rw-r--r--   0        0        0     1497 2023-12-23 03:26:26.694388 contextooor-0.9.9.9/contextooor/core/safe_math.py
--rw-r--r--   0        0        0    13969 2023-12-23 03:26:26.695305 contextooor-0.9.9.9/contextooor/core/universal_router/V2_universal_router.py
--rw-r--r--   0        0        0    17995 2023-12-23 03:26:26.696171 contextooor-0.9.9.9/contextooor/core/universal_router/V3_universal_router.py
--rw-r--r--   0        0        0     7534 2023-12-23 03:26:26.699278 contextooor-0.9.9.9/contextooor/core/universal_router/data.py
--rw-r--r--   0        0        0     5400 2023-12-23 03:26:26.699936 contextooor-0.9.9.9/contextooor/core/universal_router/policies.py
--rw-r--r--   0        0        0    21057 2024-05-27 17:07:21.907599 contextooor-0.9.9.9/contextooor/eth.py
--rw-r--r--   0        0        0    24125 2024-02-15 15:31:50.362363 contextooor-0.9.9.9/contextooor/eth_uniswap.py
--rw-r--r--   0        0        0     2302 2024-02-15 15:32:16.690084 contextooor-0.9.9.9/contextooor/etherscan_testing.py
--rw-r--r--   0        0        0      476 2024-03-12 16:19:03.385043 contextooor-0.9.9.9/contextooor/near.py
--rw-r--r--   0        0        0     2030 2024-01-31 18:53:43.352487 contextooor-0.9.9.9/contextooor/ofac_btc_cronjob.py
--rw-r--r--   0        0        0     1460 2024-03-12 15:29:50.972039 contextooor-0.9.9.9/contextooor/sol.py
--rw-r--r--   0        0        0      629 2024-03-14 15:36:17.343067 contextooor-0.9.9.9/decode_near.js
--rw-r--r--   0        0        0        0 2024-03-14 14:44:04.200505 contextooor-0.9.9.9/decode_near.rs
--rw-r--r--   0        0        0     2446 2024-03-13 18:45:11.465827 contextooor-0.9.9.9/encode_near.js
-lrwxr-xr-x   0        0        0        0 2024-03-13 13:55:58.946196 contextooor-0.9.9.9/node_modules/.bin/mustache -> ../mustache/bin/mustache
--rw-r--r--   0        0        0    20111 2024-03-14 15:31:21.934951 contextooor-0.9.9.9/node_modules/.package-lock.json
--rw-r--r--   0        0        0    20279 2024-03-14 15:31:21.931456 contextooor-0.9.9.9/package-lock.json
--rw-r--r--   0        0        0      131 2024-03-14 15:31:21.924015 contextooor-0.9.9.9/package.json
--rw-r--r--   0        0        0      600 2024-05-13 23:45:38.948684 contextooor-0.9.9.9/pyproject.toml
--rw-r--r--   0        0        0     2313 2024-02-15 15:31:40.253535 contextooor-0.9.9.9/test.py
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 contextooor-0.9.9.9/PKG-INFO
+-rw-r--r--   0        0        0      131 2024-05-27 18:11:37.919815 contextooor-0.9.9.92/.gitignore
+-rw-r--r--   0        0        0     4769 2024-05-27 20:53:31.413183 contextooor-0.9.9.92/README.md
+-rw-r--r--   0        0        0       34 2024-05-27 16:52:20.937569 contextooor-0.9.9.92/contextooor/.env.example
+-rw-r--r--   0        0        0       51 2024-05-27 16:52:20.938399 contextooor-0.9.9.92/contextooor/.gitignore
+-rw-r--r--   0        0        0       96 2024-05-28 20:19:05.898998 contextooor-0.9.9.92/contextooor/__init__.py
+-rw-r--r--   0        0        0     6285 2024-02-15 15:30:15.619991 contextooor-0.9.9.92/contextooor/btc.py
+-rw-r--r--   0        0        0     2055 2024-05-27 17:07:21.906738 contextooor-0.9.9.92/contextooor/core/Chainalysis/chainalysis_ofac_api.py
+-rw-r--r--   0        0        0    29734 2024-05-28 20:16:41.680039 contextooor-0.9.9.92/contextooor/core/V2_router/V2_router.py
+-rw-r--r--   0        0        0    28285 2024-05-28 20:16:46.711300 contextooor-0.9.9.92/contextooor/core/V3_router/V3_router.py
+-rw-r--r--   0        0        0     1724 2024-05-28 20:15:36.479992 contextooor-0.9.9.92/contextooor/core/safe_math.py
+-rw-r--r--   0        0        0    13969 2023-12-23 03:26:26.695305 contextooor-0.9.9.92/contextooor/core/universal_router/V2_universal_router.py
+-rw-r--r--   0        0        0    17995 2023-12-23 03:26:26.696171 contextooor-0.9.9.92/contextooor/core/universal_router/V3_universal_router.py
+-rw-r--r--   0        0        0     7534 2023-12-23 03:26:26.699278 contextooor-0.9.9.92/contextooor/core/universal_router/data.py
+-rw-r--r--   0        0        0     5400 2023-12-23 03:26:26.699936 contextooor-0.9.9.92/contextooor/core/universal_router/policies.py
+-rw-r--r--   0        0        0    21059 2024-05-27 18:35:11.595877 contextooor-0.9.9.92/contextooor/eth.py
+-rw-r--r--   0        0        0    25841 2024-05-27 20:45:13.212666 contextooor-0.9.9.92/contextooor/eth_uniswap.py
+-rw-r--r--   0        0        0     2302 2024-02-15 15:32:16.690084 contextooor-0.9.9.92/contextooor/etherscan_testing.py
+-rw-r--r--   0        0        0      476 2024-03-12 16:19:03.385043 contextooor-0.9.9.92/contextooor/near.py
+-rw-r--r--   0        0        0     2030 2024-01-31 18:53:43.352487 contextooor-0.9.9.92/contextooor/ofac_btc_cronjob.py
+-rw-r--r--   0        0        0     1460 2024-03-12 15:29:50.972039 contextooor-0.9.9.92/contextooor/sol.py
+-rw-r--r--   0        0        0      592 2024-05-28 20:17:14.651865 contextooor-0.9.9.92/pyproject.toml
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 contextooor-0.9.9.92/PKG-INFO
```

### Comparing `contextooor-0.9.9.9/contextooor/README.md` & `contextooor-0.9.9.92/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,57 @@
 # Contextooor
 A library to gather more data from your transaction before broadcasting.
 
 ``` pip install contextooor ```
 
+## For local development
+1. Fork repo
+2. Clone fork
+``` git clone https://your-fork-url.com ```
+3. Set up venv
+``` python3.11 -m venv env
+    source env/bin/activate
+    pip install flit
+    flit install
+```
+4. Publishing
+Bump the version in __init__.py, then run
+```
+    flit build
+    flit publish
+```
+
 ## eth_uniswap:
-    - Universal router supports execute, but missing support for the second execute method
-    - Volatility and slippage on all swap methods on V2 router
-    - Other than multicall, slippage and volatility on all swap methods on V3 router
-    - TODO: Transactions directly to pairs, multicall on V3, second execute method on universal router, volatility on universal router, fee accounting on universal router
+- Universal router supports execute, but missing support for the second execute method
+- Volatility and slippage on all swap methods on V2 router
+- Other than multicall, slippage and volatility on all swap methods on V3 router
+- TODO: Transactions directly to pairs, multicall on V3, second execute method on universal router, volatility on universal router, fee accounting on universal router
 
 ## Ethereum:
-    - Converting to USD
-    - Concurrent approvals on a specific token
-    - Concurrent approvals on all tokens
-    - Total amount approved on a specific token (usd or token value)
-    - Total amount approved on all tokens (usd)
-    - Using Forta's attack detector feed labels, is the address a known attacker?
-    - On the fly audits using slither and slitherin detectors
-    - Moooore 
+- Converting to USD
+- Concurrent approvals on a specific token
+- Concurrent approvals on all tokens
+- Total amount approved on a specific token (usd or token value)
+- Total amount approved on all tokens (usd)
+- Using Forta's attack detector feed labels, is the address a known attacker?
+- On the fly audits using slither and slitherin detectors
+- Moooore 
 
 ## Bitcoin:
-    - Decoding to transaction object
-    - Polars dataframe of recipient and their value (aggregated by recipient)
-    - Total value of transaction
-    - Value sent to a specified address
-    - Recipient is in OFAC Sanction list
-    - Largest individual amount sent
-    - Number of recipients
-    - Arbitrary rich contexting with parquet files
+- Decoding to transaction object
+- Polars dataframe of recipient and their value (aggregated by recipient)
+- Total value of transaction
+- Value sent to a specified address
+- Recipient is in OFAC Sanction list
+- Largest individual amount sent
+- Number of recipients
+- Arbitrary rich contexting with parquet files
 ## Solana:
-    - Decoding Base64
-    - Native Value Transfers (lamports/sol/usd)
+- Decoding Base64
+- Native Value Transfers (lamports/sol/usd)
 
 ## How 2 context
 ### EVM Contexting
 ```Python
 from contextooor.eth_uniswap import Snippets
 from contextooor.eth import Snippets
 from web3 import Web3
```

### Comparing `contextooor-0.9.9.9/contextooor/btc.py` & `contextooor-0.9.9.92/contextooor/btc.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.9/contextooor/core/Chainalysis/chainalysis_ofac_api.py` & `contextooor-0.9.9.92/contextooor/core/Chainalysis/chainalysis_ofac_api.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.9/contextooor/core/V2_router/V2_router.py` & `contextooor-0.9.9.92/contextooor/core/V2_router/V2_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from web3 import Web3
 import requests
 import math
-import numpy as np
 from contextooor.core.safe_math import SafeMath
 
 class uniswapV2_router:
 
     def __init__(self,w3=Web3(Web3.HTTPProvider("https://cloudflare-eth.com/")),block='latest'):
         self.web3=w3
         self.block=block
@@ -108,15 +107,15 @@
                 reserves=contract.call(block_identifier=block)
                 optimal_rate=(reserves[1]/reserves[0])
                 if str(block) in prices.keys():
                     prices[str(block)]=prices[str(block)]*optimal_rate
                 else:
                     prices[str(block)]=optimal_rate
         log_returns = [math.log(price / list(prices.values())[i - 1]) for i, price in enumerate(list(prices.values()))]
-        return np.std(log_returns)
+        return SafeMath.standard_dev(log_returns)
 
     def getSlippage(self,input_data,value=None):
         method=input_data[0:10]
         if method not in self.SUPPORTED_METHODS:
             raise ValueError(f'Method ID {method} not currently supported.')
         method_data=self.SUPPORTED_METHODS[method]
         function=method_data['slippage']
```

### Comparing `contextooor-0.9.9.9/contextooor/core/V3_router/V3_router.py` & `contextooor-0.9.9.92/contextooor/core/V3_router/V3_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from web3 import Web3
 import math
-import numpy as np
 from contextooor.core.safe_math import SafeMath
 
 class uniswapV3_router:
 
     def __init__(self,w3=Web3(Web3.HTTPProvider("https://cloudflare-eth.com/")),block='latest'):
         self.block=block
         self.web3=w3
@@ -76,15 +75,15 @@
         latest_block = self.web3.eth.block_number
 
         for block in range(latest_block - (block_depth-1), latest_block):
             price = self.getRate(token0,token1,fee,block)
             prices.append(price)
 
         log_returns = [math.log(price / prices[i - 1]) for i, price in enumerate(prices)]
-        return np.std(log_returns)
+        return SafeMath.standard_dev(log_returns)
     
     def full_decode(self,input_data):
         partially_decoded=self.router_contract.decode_function_input(input_data)
         decoded=partially_decoded[1]['params']
         path=self.decode_path(decoded['path'])
         decoded['path']=path
         return decoded
@@ -97,24 +96,24 @@
             addr1=path[0+base]
             fee=path[1+base]
             addr2=path[2+base]
             token0,token1,inverse=self.align_tokens_inverse(addr1,addr2)
             optimal_rate=SafeMath().safe_exponent(self.getRate(token0,token1,fee,block),inverse)
             running_rate=running_rate*optimal_rate*(1-(fee/1000000))
         return running_rate
-    
+
     def get_path_volatility(self,input_data,block_depth=100):
         prices=[]
         decoded=self.full_decode(input_data)
         latest_block = self.web3.eth.block_number
         for block in range(latest_block - (block_depth-1), latest_block):
             actual_rate=self.get_optimal_path_rate(decoded["path"],block)
             prices.append(actual_rate)
         log_returns = [math.log(price / prices[i - 1]) for i, price in enumerate(prices)]
-        return np.std(log_returns)
+        return SafeMath.standard_dev(log_returns)
 
     def getSlippage_path_input(self,input_data):
         decoded=self.full_decode(input_data)
         executed_rate=self.safe_division(decoded['amountIn'],decoded['amountOutMinimum'])
         actual_rate=self.get_optimal_path_rate(decoded["path"])
         return 1-self.safe_division(executed_rate,actual_rate)
```

### Comparing `contextooor-0.9.9.9/contextooor/core/universal_router/V2_universal_router.py` & `contextooor-0.9.9.92/contextooor/core/universal_router/V2_universal_router.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.9/contextooor/core/universal_router/V3_universal_router.py` & `contextooor-0.9.9.92/contextooor/core/universal_router/V3_universal_router.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.9/contextooor/core/universal_router/data.py` & `contextooor-0.9.9.92/contextooor/core/universal_router/data.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.9/contextooor/core/universal_router/policies.py` & `contextooor-0.9.9.92/contextooor/core/universal_router/policies.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.9/contextooor/eth.py` & `contextooor-0.9.9.92/contextooor/eth.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
     def is_poisonned_address(self,from_address,to_address, first_n=4, last_n=4, current_block_number=99999999):
         from_address=from_address.lower()
         to_address=to_address.lower()
         df=self.get_tx_history(from_address,current_block_number)
         matchbook=self.find_matches(df,from_address,to_address,first_n,last_n)
         return self.parse_results(matchbook,to_address)
     
-def test_snippets():
+def test_chainalysis():
     api_key = os.getenv('CHAINALYSIS_API_KEY')
     if api_key is None:
         raise ValueError("CHAINALYSIS_API_KEY is not set")
 
     chainalysis = Chainalysis(api_key)
     for address in DEMO_SANCTIONED_ADDRESSES:
       is_sanctioned = chainalysis.is_sanctioned(address)
@@ -282,8 +282,7 @@
       
     for address in DEMO_NON_SANCTIONED_ADDRESSES:
       is_sanctioned = chainalysis.is_sanctioned(address)
       assert is_sanctioned == False
 
       sanction_data = chainalysis.get_sanctioned_address_data(address)
       assert len(sanction_data) == 0
-
```

### Comparing `contextooor-0.9.9.9/contextooor/eth_uniswap.py` & `contextooor-0.9.9.92/contextooor/eth_uniswap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from contextooor.core.universal_router.policies import universal_router
 from contextooor.core.V3_router.V3_router import uniswapV3_router
 from contextooor.core.V2_router.V2_router import uniswapV2_router
 from web3 import Web3
+import requests
 
 class Snippets:
 
     def __init__(self,w3=Web3(Web3.HTTPProvider("https://eth.public-rpc.com")),block='latest',suppress_errors=True):
         self.web3=w3
         try:
             self.web3.eth.get_block_number()
@@ -62,10 +63,33 @@
             return {'success':function(input_data,block_depth)}
         except ValueError as e:
             if self.suppress_errors:
                 return {"error":e.args}
             else: 
                 raise ValueError(e.args)
 
-        
 
-    
+def get_transaction(tx_hash):
+    url = f"https://api.etherscan.io/api?module=proxy&action=eth_getTransactionByHash&txhash={tx_hash}&apikey=VP84ZNW3VHQ2S9JHE92VYXV96NX9E5U3VU"
+    response = requests.get(url)
+    if response.status_code == 200:
+        return response.json()
+    else:
+        raise Exception("Failed to fetch transaction data")
+
+def test_slippage():
+    test_transactions=[{"test":"universal-pass","tx_hash":"0xec0e8702b4b47eb8ffd00e6bebcd4fc49407940bd0b8c706b07b2d428b858f2a","expected_result":{'success': 0.018734462880736102}},
+                       {"test":"v3-router-pass","tx_hash":"0xba403decf1e1c2fd5a2e4b05fe2b7d627e417f302240f54f838781b4c09b32ae","expected_result":{'success': 0.005573769978890364}},
+                       {"test":"v3-router-unsupported-method","tx_hash":"0x1d553a00265241c469ee4c13816e0a1d44eda59064e9151fc0255aabe2e30e4d","expected_result":{'error': ('Method ID 0xac9650d8 not currently supported',)}},
+                       {"test":"v2-router-pass","tx_hash":"0x8c1b8a2a725732ed3c25d59b75d9341be4cfdc28290a586af4d14a2b0c98bfd3","expected_result":{'success': 0.004669577023805327}},
+                       {"test":"v2-router-pass_low_liquidity","tx_hash":"0xc663a7077093e802530625ed7aa7ea8786aa843b3830d8dbbe8d2435f4d07429","expected_result":{'success': -3093319975.3551455}}]
+    for case in test_transactions:
+        hash=case['tx_hash']
+        tx=get_transaction(hash)['result']
+        block_number=int(tx['blockNumber'],16)
+        value=int(tx['blockNumber'],16)
+        sn=Snippets(block=block_number-1)
+        slip=sn.getSlippage(to_address=tx['to'],input_data=tx['input'],value=value)
+        print(slip)
+        assert slip==case['expected_result']
+
+
```

### Comparing `contextooor-0.9.9.9/contextooor/etherscan_testing.py` & `contextooor-0.9.9.92/contextooor/etherscan_testing.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.9/contextooor/ofac_btc_cronjob.py` & `contextooor-0.9.9.92/contextooor/ofac_btc_cronjob.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.9/contextooor/sol.py` & `contextooor-0.9.9.92/contextooor/sol.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.9/pyproject.toml` & `contextooor-0.9.9.92/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "contextooor"
 authors = [
     {name = "David Desjardins", email = "david.thegardens@gmail.com"},
 ]
 dynamic = ["version", "description"]
 dependencies = [
   "web3>=6.11.4",
-  "numpy>=1.26.2",
   "uniswap_universal_router_decoder",
   "python_bitcoinlib",
   "polars",
   "slither-analyzer",
   "slitherin",
   "solc-select",
+  "pytest"
 ]
```

