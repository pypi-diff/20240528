# Comparing `tmp/bitcoin-utils-0.6.6.tar.gz` & `tmp/bitcoin-utils-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin-utils-0.6.6.tar", last modified: Wed Mar 13 12:42:10 2024, max compression
+gzip compressed data, was "bitcoin-utils-0.6.8.tar", last modified: Tue May 28 07:02:16 2024, max compression
```

## Comparing `bitcoin-utils-0.6.6.tar` & `bitcoin-utils-0.6.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2024-03-13 12:42:10.665978 bitcoin-utils-0.6.6/
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     1097 2023-01-06 11:32:26.000000 bitcoin-utils-0.6.6/LICENSE
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     8208 2024-03-13 12:42:10.665978 bitcoin-utils-0.6.6/PKG-INFO
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     7892 2024-03-04 09:02:12.000000 bitcoin-utils-0.6.6/README.rst
-drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2024-03-13 12:42:10.665978 bitcoin-utils-0.6.6/bitcoin_utils.egg-info/
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     8208 2024-03-13 12:42:10.000000 bitcoin-utils-0.6.6/bitcoin_utils.egg-info/PKG-INFO
--rw-rw-r--   0 kostas   (30000) kostas   (30003)      535 2024-03-13 12:42:10.000000 bitcoin-utils-0.6.6/bitcoin_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 kostas   (30000) kostas   (30003)        1 2024-03-13 12:42:10.000000 bitcoin-utils-0.6.6/bitcoin_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 kostas   (30000) kostas   (30003)        1 2023-01-10 09:09:10.000000 bitcoin-utils-0.6.6/bitcoin_utils.egg-info/not-zip-safe
--rw-rw-r--   0 kostas   (30000) kostas   (30003)       98 2024-03-13 12:42:10.000000 bitcoin-utils-0.6.6/bitcoin_utils.egg-info/requires.txt
--rw-rw-r--   0 kostas   (30000) kostas   (30003)       13 2024-03-13 12:42:10.000000 bitcoin-utils-0.6.6/bitcoin_utils.egg-info/top_level.txt
-drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2024-03-13 12:42:10.665978 bitcoin-utils-0.6.6/bitcoinutils/
--rw-rw-r--   0 kostas   (30000) kostas   (30003)       22 2024-01-23 12:17:48.000000 bitcoin-utils-0.6.6/bitcoinutils/__init__.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     5122 2023-09-06 10:50:56.000000 bitcoin-utils-0.6.6/bitcoinutils/bech32.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     1843 2023-09-03 11:44:59.000000 bitcoin-utils-0.6.6/bitcoinutils/constants.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     2405 2023-11-30 07:25:37.000000 bitcoin-utils-0.6.6/bitcoinutils/hdwallet.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)    46009 2024-03-13 12:30:27.000000 bitcoin-utils-0.6.6/bitcoinutils/keys.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     2002 2023-09-05 08:48:23.000000 bitcoin-utils-0.6.6/bitcoinutils/proxy.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     5345 2023-05-30 16:59:52.000000 bitcoin-utils-0.6.6/bitcoinutils/ripemd160.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     6474 2023-09-06 09:01:04.000000 bitcoin-utils-0.6.6/bitcoinutils/schnorr.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)    13537 2024-03-06 09:33:22.000000 bitcoin-utils-0.6.6/bitcoinutils/script.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     1019 2023-09-03 23:05:48.000000 bitcoin-utils-0.6.6/bitcoinutils/setup.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)    40174 2024-01-23 11:31:52.000000 bitcoin-utils-0.6.6/bitcoinutils/transactions.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)    14695 2024-03-13 12:30:27.000000 bitcoin-utils-0.6.6/bitcoinutils/utils.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)       38 2024-03-13 12:42:10.665978 bitcoin-utils-0.6.6/setup.cfg
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     1074 2023-06-01 15:38:14.000000 bitcoin-utils-0.6.6/setup.py
+drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2024-05-28 07:02:16.075261 bitcoin-utils-0.6.8/
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     1097 2024-04-19 12:45:45.000000 bitcoin-utils-0.6.8/LICENSE
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     8208 2024-05-28 07:02:16.075261 bitcoin-utils-0.6.8/PKG-INFO
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     7892 2024-04-17 07:25:31.000000 bitcoin-utils-0.6.8/README.rst
+drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2024-05-28 07:02:16.075261 bitcoin-utils-0.6.8/bitcoin_utils.egg-info/
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     8208 2024-05-28 07:02:16.000000 bitcoin-utils-0.6.8/bitcoin_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)      535 2024-05-28 07:02:16.000000 bitcoin-utils-0.6.8/bitcoin_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)        1 2024-05-28 07:02:16.000000 bitcoin-utils-0.6.8/bitcoin_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)        1 2023-01-10 09:09:10.000000 bitcoin-utils-0.6.8/bitcoin_utils.egg-info/not-zip-safe
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)       98 2024-05-28 07:02:16.000000 bitcoin-utils-0.6.8/bitcoin_utils.egg-info/requires.txt
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)       13 2024-05-28 07:02:16.000000 bitcoin-utils-0.6.8/bitcoin_utils.egg-info/top_level.txt
+drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2024-05-28 07:02:16.075261 bitcoin-utils-0.6.8/bitcoinutils/
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)       22 2024-04-17 07:27:12.000000 bitcoin-utils-0.6.8/bitcoinutils/__init__.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     5122 2024-04-19 12:45:45.000000 bitcoin-utils-0.6.8/bitcoinutils/bech32.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     2001 2024-04-19 12:45:45.000000 bitcoin-utils-0.6.8/bitcoinutils/constants.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     2544 2024-04-19 12:45:45.000000 bitcoin-utils-0.6.8/bitcoinutils/hdwallet.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)    46145 2024-04-19 12:45:45.000000 bitcoin-utils-0.6.8/bitcoinutils/keys.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     2002 2024-04-19 12:45:45.000000 bitcoin-utils-0.6.8/bitcoinutils/proxy.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     5350 2024-04-19 12:45:45.000000 bitcoin-utils-0.6.8/bitcoinutils/ripemd160.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     6474 2023-09-06 09:01:04.000000 bitcoin-utils-0.6.8/bitcoinutils/schnorr.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)    13731 2024-04-19 12:49:00.000000 bitcoin-utils-0.6.8/bitcoinutils/script.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     1019 2024-04-19 12:45:45.000000 bitcoin-utils-0.6.8/bitcoinutils/setup.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)    39820 2024-04-19 12:45:45.000000 bitcoin-utils-0.6.8/bitcoinutils/transactions.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)    14903 2024-04-19 12:45:45.000000 bitcoin-utils-0.6.8/bitcoinutils/utils.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)       38 2024-05-28 07:02:16.075261 bitcoin-utils-0.6.8/setup.cfg
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     1074 2024-05-28 06:57:55.000000 bitcoin-utils-0.6.8/setup.py
```

### Comparing `bitcoin-utils-0.6.6/LICENSE` & `bitcoin-utils-0.6.8/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2020 The python-bitcoin-utils developers
+Copyright (c) 2018-2024 The python-bitcoin-utils developers
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `bitcoin-utils-0.6.6/PKG-INFO` & `bitcoin-utils-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: bitcoin-utils
-Version: 0.6.6
+Version: 0.6.8
 Summary: Bitcoin utility functions
 Home-page: https://github.com/karask/python-bitcoin-utils
 Author: Konstantinos Karasavvas
 Author-email: kkarasavvas@gmail.com
 License: MIT
 Keywords: bitcoin library utilities tools
 Platform: UNKNOWN
 License-File: LICENSE
 
 python-bitcoin-utils
 ====================
 
 This is a bitcoin library that provides tools/utilities to interact with the Bitcoin network. One of the primary goals of the library is to explain the low-level details of Bitcoin. The code is easy to read and properly documented explaining in detail all the thorny aspects of the implementation. It is a low-level library which assumes some high-level understanding of how Bitcoin works. In the future this might change.
 
-This is an early version of the library (v0.6.6) and currently, it supports private/public keys, all type of addresses and creation of any transaction, incl. segwit and taproot, with all SIGHASH types. All script op codes are included. Extra functionality will be added continuously and the documentation will be improved as the work progresses.
+This is an early version of the library (v0.6.8) and currently, it supports private/public keys, all type of addresses and creation of any transaction, incl. segwit and taproot, with all SIGHASH types. All script op codes are included. Extra functionality will be added continuously and the documentation will be improved as the work progresses.
 
 The API documentation can be build with Sphinx but is also available as a PDF for convenience. One can currently use the library for experimenting and learning the inner workings of Bitcoin. It is not meant for production yet and parts of the API might be updated with new versions.
 
 Complementary to this library is a CC BY-SA 4.0 licensed `Bitcoin programming book <https://github.com/karask/bitcoin-textbook>`_.
 
 
 Notes
```

### Comparing `bitcoin-utils-0.6.6/README.rst` & `bitcoin-utils-0.6.8/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 python-bitcoin-utils
 ====================
 
 This is a bitcoin library that provides tools/utilities to interact with the Bitcoin network. One of the primary goals of the library is to explain the low-level details of Bitcoin. The code is easy to read and properly documented explaining in detail all the thorny aspects of the implementation. It is a low-level library which assumes some high-level understanding of how Bitcoin works. In the future this might change.
 
-This is an early version of the library (v0.6.6) and currently, it supports private/public keys, all type of addresses and creation of any transaction, incl. segwit and taproot, with all SIGHASH types. All script op codes are included. Extra functionality will be added continuously and the documentation will be improved as the work progresses.
+This is an early version of the library (v0.6.8) and currently, it supports private/public keys, all type of addresses and creation of any transaction, incl. segwit and taproot, with all SIGHASH types. All script op codes are included. Extra functionality will be added continuously and the documentation will be improved as the work progresses.
 
 The API documentation can be build with Sphinx but is also available as a PDF for convenience. One can currently use the library for experimenting and learning the inner workings of Bitcoin. It is not meant for production yet and parts of the API might be updated with new versions.
 
 Complementary to this library is a CC BY-SA 4.0 licensed `Bitcoin programming book <https://github.com/karask/bitcoin-textbook>`_.
 
 
 Notes
```

### Comparing `bitcoin-utils-0.6.6/bitcoin_utils.egg-info/PKG-INFO` & `bitcoin-utils-0.6.8/bitcoin_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: bitcoin-utils
-Version: 0.6.6
+Version: 0.6.8
 Summary: Bitcoin utility functions
 Home-page: https://github.com/karask/python-bitcoin-utils
 Author: Konstantinos Karasavvas
 Author-email: kkarasavvas@gmail.com
 License: MIT
 Keywords: bitcoin library utilities tools
 Platform: UNKNOWN
 License-File: LICENSE
 
 python-bitcoin-utils
 ====================
 
 This is a bitcoin library that provides tools/utilities to interact with the Bitcoin network. One of the primary goals of the library is to explain the low-level details of Bitcoin. The code is easy to read and properly documented explaining in detail all the thorny aspects of the implementation. It is a low-level library which assumes some high-level understanding of how Bitcoin works. In the future this might change.
 
-This is an early version of the library (v0.6.6) and currently, it supports private/public keys, all type of addresses and creation of any transaction, incl. segwit and taproot, with all SIGHASH types. All script op codes are included. Extra functionality will be added continuously and the documentation will be improved as the work progresses.
+This is an early version of the library (v0.6.8) and currently, it supports private/public keys, all type of addresses and creation of any transaction, incl. segwit and taproot, with all SIGHASH types. All script op codes are included. Extra functionality will be added continuously and the documentation will be improved as the work progresses.
 
 The API documentation can be build with Sphinx but is also available as a PDF for convenience. One can currently use the library for experimenting and learning the inner workings of Bitcoin. It is not meant for production yet and parts of the API might be updated with new versions.
 
 Complementary to this library is a CC BY-SA 4.0 licensed `Bitcoin programming book <https://github.com/karask/bitcoin-textbook>`_.
 
 
 Notes
```

### Comparing `bitcoin-utils-0.6.6/bitcoin_utils.egg-info/SOURCES.txt` & `bitcoin-utils-0.6.8/bitcoin_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.6.6/bitcoinutils/bech32.py` & `bitcoin-utils-0.6.8/bitcoinutils/bech32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017, 2020 Pieter Wuille
+# Copyright (c) 2017, 2024 Pieter Wuille
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `bitcoin-utils-0.6.6/bitcoinutils/constants.py` & `bitcoin-utils-0.6.8/bitcoinutils/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-# Copyright (C) 2018-2022 The python-bitcoin-utils developers
+# Copyright (C) 2018-2024 The python-bitcoin-utils developers
 #
 # This file is part of python-bitcoin-utils
 #
 # It is subject to the license terms in the LICENSE file found in the top-level
 # directory of this distribution.
 #
 # No part of python-bitcoin-utils, including this file, may be copied, modified,
 # propagated, or distributed except according to the terms contained in the
 # LICENSE file.
 
-# TODO organise constants in sections
-
 NETWORK_DEFAULT_PORTS = {
     "mainnet": 8332,
     "signet": 38332,
     "testnet": 18332,
     "regtest": 18443,
 }
 
@@ -42,39 +40,50 @@
 NETWORK_SEGWIT_PREFIXES = {
     "mainnet": "bc",
     "signet": "tb",
     "testnet": "tb",
     "regtest": "bcrt",
 }
 
+
+# Constants for address types
 P2PKH_ADDRESS = "p2pkh"
 P2SH_ADDRESS = "p2sh"
 P2WPKH_ADDRESS_V0 = "p2wpkhv0"
 P2WSH_ADDRESS_V0 = "p2wshv0"
 P2TR_ADDRESS_V1 = "p2trv1"
 
+
+# Constants related to transaction signature types
 TAPROOT_SIGHASH_ALL = 0x00
 SIGHASH_ALL = 0x01
 SIGHASH_NONE = 0x02
 SIGHASH_SINGLE = 0x03
 SIGHASH_ANYONECANPAY = 0x80
 
+
+# Constants for time lock and RB
 TYPE_ABSOLUTE_TIMELOCK = 0x101
 TYPE_RELATIVE_TIMELOCK = 0x201
 TYPE_REPLACE_BY_FEE = 0x301
 
 DEFAULT_TX_LOCKTIME = b"\x00\x00\x00\x00"
 
 EMPTY_TX_SEQUENCE = b"\x00\x00\x00\x00"
 DEFAULT_TX_SEQUENCE = b"\xff\xff\xff\xff"
 ABSOLUTE_TIMELOCK_SEQUENCE = b"\xfe\xff\xff\xff"
 
 REPLACE_BY_FEE_SEQUENCE = b"\x01\x00\x00\x00"
 
+
+# Constants related to transaction versions and scripts
 LEAF_VERSION_TAPSCRIPT = 0xC0
 
+
 # TX version 2 was introduced in BIP-68 with relative locktime -- tx v1
 # does not support relative locktime
 DEFAULT_TX_VERSION = b"\x02\x00\x00\x00"
 
+
+# Monetary constants
 SATOSHIS_PER_BITCOIN = 100000000
 NEGATIVE_SATOSHI = -1
```

### Comparing `bitcoin-utils-0.6.6/bitcoinutils/hdwallet.py` & `bitcoin-utils-0.6.8/bitcoinutils/hdwallet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2023 The python-bitcoin-utils developers
+# Copyright (C) 2018-2024 The python-bitcoin-utils developers
 #
 # This file is part of python-bitcoin-utils
 #
 # It is subject to the license terms in the LICENSE file found in the top-level
 # directory of this distribution.
 #
 # No part of python-bitcoin-utils, including this file, may be copied, modified,
@@ -45,34 +45,33 @@
             symbol = BTC
         else:
             symbol = BTCTEST
 
         self.hdw = ext_HDWallet(symbol)
 
         if mnemonic:
-            self.from_mnemonic(mnemonic)
+            self.hdw.from_mnemonic(mnemonic=mnemonic)
 
-        if xprivate_key:
-            assert path is not None
-            self.from_xprivate_key(xprivate_key, path)
-
-    # TODO make this a class method, return cls(mnemonic=)
-    def from_mnemonic(self, mnemonic: str):
-        """Set a mnemonic code for the HD Wallet"""
-
-        self.hdw.from_mnemonic(mnemonic=mnemonic)
-
-    # TODO make this a class method, return cls(xprivate_key=, path=)
-    def from_xprivate_key(self, xprivate_key: str, path: Optional[str] = None):
-        """Set an extended private key and optionally the path for the HD Wallet"""
-
-        self.hdw.from_xprivate_key(xprivate_key=xprivate_key)
-        if path:
+        if xprivate_key and path:
+            self.hdw.from_xprivate_key(xprivate_key=xprivate_key)
             self.hdw.from_path(path=path)
 
+    @classmethod
+    def from_mnemonic(cls, mnemonic: str):
+        """Class method to instantiate from a mnemonic code for the HD Wallet"""
+        return cls(mnemonic=mnemonic)
+
+    @classmethod
+    def from_xprivate_key(cls, xprivate_key: str, path: Optional[str] = None):
+        """Class method to instantiate from an extended private key and optionally the path for the HD Wallet"""
+        # Assert to ensure path is not None if xprivate_key is provided
+        assert path is not None, "Path must be provided with xprivate key"
+        # Create an instance directly using the xprivate key and path
+        return cls(xprivate_key=xprivate_key, path=path)
+
     def from_path(self, path: str):
         """Set/update the path"""
 
         self.hdw.clean_derivation()  # type: ignore
         self.hdw.from_path(path=path)
 
     def get_private_key(self):
```

### Comparing `bitcoin-utils-0.6.6/bitcoinutils/keys.py` & `bitcoin-utils-0.6.8/bitcoinutils/keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2022 The python-bitcoin-utils developers
+# Copyright (C) 2018-2024 The python-bitcoin-utils developers
 #
 # This file is part of python-bitcoin-utils
 #
 # It is subject to the license terms in the LICENSE file found in the top-level
 # directory of this distribution.
 #
 # No part of python-bitcoin-utils, including this file, may be copied, modified,
@@ -46,17 +46,16 @@
     TAPROOT_SIGHASH_ALL,
 )
 from bitcoinutils.setup import get_network
 from bitcoinutils.ripemd160 import ripemd160
 from bitcoinutils.schnorr import schnorr_sign
 from bitcoinutils.transactions import Transaction
 from bitcoinutils.utils import (
-    EcdsaParams,
+    Secp256k1Params,
     calculate_tweak,
-    bytes32_from_int,
     add_magic_prefix,
     h_to_i,
     b_to_h,
     h_to_b,
     b_to_i,
     i_to_b32,
     tweak_taproot_pubkey,
@@ -149,15 +148,16 @@
         """Creates key from WIFC or WIF format key"""
 
         return cls(b=b)
 
     def _from_bytes(self, b: bytes):
         """Creates a key directly from 32 raw bytes"""
 
-        # TODO check if b is len 32 and raise error
+        if len(b) != 32:
+            raise ValueError("Invalid key length: must be exactly 32 bytes.")
         self.key = SigningKey.from_string(b, curve=SECP256k1)
 
     # expects wif in hex string
     def _from_wif(self, wif: str):
         """Creates key from WIFC or WIF format key
 
         Check to_wif for the detailed process. From WIF is the reverse.
@@ -362,15 +362,15 @@
         # if high R re-sign until we get a low R value
         # if high R then its size will be 33 bytes to include the sign
         attempt = 1
         length_r = signature[3]
         while length_r == 33:
             signature = self.key.sign_digest_deterministic(
                 tx_digest,
-                extra_entropy=bytes32_from_int(attempt),
+                extra_entropy=i_to_b32(attempt),
                 sigencode=sigencode_der,
                 hashfunc=hashlib.sha256,
             )
             attempt += 1
             length_r = signature[3]
 
         # make sure that signature complies with Low S standardness rule of
@@ -403,15 +403,15 @@
         S = signature[5 + length_r + 1 :]
         S_as_bigint = b_to_i(S)
 
         # update S -- Low S standardness rule
 
         # if length is 33 bytes then it contains a sign and thus is high S
         if length_s == 33:
-            new_S_as_bigint = EcdsaParams._order - S_as_bigint
+            new_S_as_bigint = Secp256k1Params._order - S_as_bigint
             # convert bigint to bytes
             # new_S = h_to_b(i_to_h64(new_S_as_bigint))
             new_S = i_to_b32(new_S_as_bigint)
             # new value should be 32 bytes
             assert len(new_S) == 0x20
             # reduce appropriate lengths
             length_s -= 1
@@ -537,44 +537,47 @@
 
         Raises
         ------
         TypeError
             If first byte of public key (corresponding to SEC format) is
             invalid.
         """
-        # TODO accepts hex str in any format and handle here!
+        hex_str = hex_str.strip()
+
+        # Normalize hex string by removing '0x' prefix and any whitespace
+        if hex_str.lower().startswith('0x'):
+            hex_str = hex_str[2:]
 
         # expects key as hex string - SEC format
         first_byte_in_hex = hex_str[:2]  # 2 hex chars = 1 byte
         hex_bytes = h_to_b(hex_str)
 
-        # TODO needed?? - see flag below
         taproot = False
 
         # check if compressed or not
         if len(hex_bytes) > 33:
             # uncompressed - SEC format: 0x04 + x + y coordinates (x,y are 32 byte
             # numbers)
 
             # remove first byte and instantiate ecdsa key
             self.key = VerifyingKey.from_string(hex_bytes[1:], curve=SECP256k1)
         elif len(hex_bytes) > 31:
             # key is either compressed or in x-only taproot format
 
-            # taproot is 32 bytes and it should always be prefixed with 0x02
+            # taproot public keys are exactly 32 bytes
             if len(hex_bytes) == 32:
                 taproot = True
 
             # compressed - SEC FORMAT: 0x02|0x03 + x coordinate (if 02 then y
             # is even else y is odd. Calculate y and then instantiate the ecdsa key
             x_coord = int(hex_str[2:], 16)
 
             # y = modulo_square_root( (x**3 + 7) mod p ) -- there will be 2 y values
             y_values = sqrt_mod(
-                (x_coord**3 + 7) % EcdsaParams._p, EcdsaParams._p, True
+                (x_coord**3 + 7) % Secp256k1Params._p, Secp256k1Params._p, True
             )
 
             assert y_values is not None
             # check SEC format's first byte to determine which of the 2 values to use
             if first_byte_in_hex == "02" or taproot:
                 # y is the even value
                 if y_values[0] % 2 == 0:  # type: ignore
@@ -713,38 +716,38 @@
         message_digest = hashlib.sha256(hashlib.sha256(message_magic).digest()).digest()
 
         #
         # use recid, r and s to get the point in the curve
         #
 
         # get signature's r and s
-        r, s = sigdecode_string(sig[1:], EcdsaParams._order)
+        r, s = sigdecode_string(sig[1:], Secp256k1Params._order)
 
         # ger R's x coordinate
-        x = r + (recid // 2) * EcdsaParams._order
+        x = r + (recid // 2) * Secp256k1Params._order
 
         # get R's y coordinate (y**2 = x**3 + 7)
-        y_values = sqrt_mod((x**3 + 7) % EcdsaParams._p, EcdsaParams._p, True)
+        y_values = sqrt_mod((x**3 + 7) % Secp256k1Params._p, Secp256k1Params._p, True)
         if (y_values[0] - recid) % 2 == 0:  # type: ignore
             y = y_values[0]  # type: ignore
         else:
             y = y_values[1]  # type: ignore
 
         # get R (recovered ephemeral key) from x,y
-        R = ellipticcurve.Point(EcdsaParams._curve, x, y, EcdsaParams._order)
+        R = ellipticcurve.Point(Secp256k1Params._curve, x, y, Secp256k1Params._order)
 
         # get e (encoded message hash as big integer)
         e = b_to_i(message_digest)
 
         # compute public key Q = r^-1 (sR - eG)
         # because Point substraction is not defined we will instead use:
         # Q = r^-1 (sR + (-eG) )
-        minus_e = -e % EcdsaParams._order
-        inv_r = numbertheory.inverse_mod(r, EcdsaParams._order)
-        Q = inv_r * (s * R + minus_e * EcdsaParams._G)
+        minus_e = -e % Secp256k1Params._order
+        inv_r = numbertheory.inverse_mod(r, Secp256k1Params._order)
+        Q = inv_r * (s * R + minus_e * Secp256k1Params._G)
 
         # instantiate the public key and verify message
         public_key = VerifyingKey.from_public_point(Q, curve=SECP256k1)
         key_hex = b_to_h(public_key.to_string())
         pubkey = PublicKey.from_hex("04" + key_hex)
         if not pubkey.verify(signature, message):
             return False
```

### Comparing `bitcoin-utils-0.6.6/bitcoinutils/proxy.py` & `bitcoin-utils-0.6.8/bitcoinutils/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2022 The python-bitcoin-utils developers
+# Copyright (C) 2018-2024 The python-bitcoin-utils developers
 #
 # This file is part of python-bitcoin-utils
 #
 # It is subject to the license terms in the LICENSE file found in the top-level
 # directory of this distribution.
 #
 # No part of python-bitcoin-utils, including this file, may be copied, modified,
```

### Comparing `bitcoin-utils-0.6.6/bitcoinutils/ripemd160.py` & `bitcoin-utils-0.6.8/bitcoinutils/ripemd160.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021 Pieter Wuille
+# Copyright (c) 2021-2024 Pieter Wuille
 # Distributed under the MIT software license, see the accompanying
 # file COPYING or http://www.opensource.org/licenses/mit-license.php.
 """Test-only pure Python RIPEMD160 implementation."""
 
 # This is required because new verions of openssl do not allow for using
 # ripemd160 unless you manually configure openssl accordinly. To solve we
 # use a pure python ripemd implementation that was added to Bitcoin Core
```

### Comparing `bitcoin-utils-0.6.6/bitcoinutils/schnorr.py` & `bitcoin-utils-0.6.8/bitcoinutils/schnorr.py`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.6.6/bitcoinutils/script.py` & `bitcoin-utils-0.6.8/bitcoinutils/script.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2022 The python-bitcoin-utils developers
+# Copyright (C) 2018-2024 The python-bitcoin-utils developers
 #
 # This file is part of python-bitcoin-utils
 #
 # It is subject to the license terms in the LICENSE file found in the top-level
 # directory of this distribution.
 #
 # No part of python-bitcoin-utils, including this file, may be copied, modified,
@@ -11,15 +11,15 @@
 
 import copy
 import hashlib
 import struct
 from typing import Any
 
 from bitcoinutils.ripemd160 import ripemd160
-from bitcoinutils.utils import b_to_h, h_to_b, to_bytes, vi_to_int
+from bitcoinutils.utils import b_to_h, h_to_b, vi_to_int
 
 # import bitcoinutils.keys
 
 
 # Bitcoin's op codes. Complete list at: https://en.bitcoin.it/wiki/Script
 OP_CODES = {
     # constants
@@ -286,19 +286,16 @@
         0x4c-0xff           -> OP_PUSHDATA1 plus 1-byte-length plus data bytes
         0x0100-0xffff       -> OP_PUSHDATA2 plus 2-byte-length plus data bytes
         0x010000-0xffffffff -> OP_PUSHDATA4 plus 4-byte-length plus data bytes
 
         Also note that according to standarardness rules (BIP-62) the minimum
         possible PUSHDATA operator must be used!
         """
-
-        # expects data in hexadecimal characters and converts appropriately
-        # TODO maybe, for convenience, also accept objects for public keys,
-        # addresses, etc. and use isinstance and convert manually
-        data_bytes = h_to_b(data)
+        
+        data_bytes = h_to_b(data) # Assuming string is hexadecimal
 
         if len(data_bytes) < 0x4C:
             return bytes([len(data_bytes)]) + data_bytes
         elif len(data_bytes) < 0xFF:
             return b"\x4c" + bytes([len(data_bytes)]) + data_bytes
         elif len(data_bytes) < 0xFFFF:
             return b"\x4d" + struct.pack("<H", len(data_bytes)) + data_bytes
@@ -365,40 +362,51 @@
             Attributes
             ----------
             txinputraw : string (hex)
                 The hexadecimal raw string representing the Script commands
             has_segwit : boolean
                 Is the Tx Input segwit or not
         """
-        scriptraw = to_bytes(scriptrawhex)
+        scriptraw = h_to_b(scriptrawhex)
         commands = []
         index = 0
 
         while index < len(scriptraw):
             byte = scriptraw[index]
             if bytes([byte]) in CODE_OPS:
-                commands.append(CODE_OPS[bytes([byte])])
+                if (
+                    bytes([byte]) != b"\x4c"
+                    and bytes([byte]) != b"\x4d"
+                    and bytes([byte]) != b"\x4e"
+                ):
+                    commands.append(CODE_OPS[bytes([byte])])
                 index = index + 1
                 # handle the 3 special bytes 0x4c,0x4d,0x4e if the transaction is
                 # not segwit type
-            elif has_segwit is False and bytes([byte]) == b"\x4c":
-                bytes_to_read = int.from_bytes(scriptraw[index : index + 1], "little")
-                index = index + 1
-                commands.append(scriptraw[index : index + bytes_to_read].hex())
-                index = index + bytes_to_read
-            elif has_segwit is False and bytes([byte]) == b"\x4d":
-                bytes_to_read = int.from_bytes(scriptraw[index : index + 2], "little")
-                index = index + 2
-                commands.append(scriptraw[index : index + bytes_to_read].hex())
-                index = index + bytes_to_read
-            elif has_segwit is False and bytes([byte]) == b"\x4e":
-                bytes_to_read = int.from_bytes(scriptraw[index : index + 4], "little")
-                index = index + 4
-                commands.append(scriptraw[index : index + bytes_to_read].hex())
-                index = index + bytes_to_read
+                if has_segwit is False and bytes([byte]) == b"\x4c":
+                    bytes_to_read = int.from_bytes(
+                        scriptraw[index : index + 1], "little"
+                    )
+                    index = index + 1
+                    commands.append(scriptraw[index : index + bytes_to_read].hex())
+                    index = index + bytes_to_read
+                elif has_segwit is False and bytes([byte]) == b"\x4d":
+                    bytes_to_read = int.from_bytes(
+                        scriptraw[index : index + 2], "little"
+                    )
+                    index = index + 2
+                    commands.append(scriptraw[index : index + bytes_to_read].hex())
+                    index = index + bytes_to_read
+                elif has_segwit is False and bytes([byte]) == b"\x4e":
+                    bytes_to_read = int.from_bytes(
+                        scriptraw[index : index + 4], "little"
+                    )
+                    index = index + 4
+                    commands.append(scriptraw[index : index + bytes_to_read].hex())
+                    index = index + bytes_to_read
             else:
                 data_size, size = vi_to_int(scriptraw[index : index + 8])
                 commands.append(
                     scriptraw[index + size : index + size + data_size].hex()
                 )
                 index = index + data_size + size
```

### Comparing `bitcoin-utils-0.6.6/bitcoinutils/setup.py` & `bitcoin-utils-0.6.8/bitcoinutils/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2022 The python-bitcoin-utils developers
+# Copyright (C) 2018-2024 The python-bitcoin-utils developers
 #
 # This file is part of python-bitcoin-utils
 #
 # It is subject to the license terms in the LICENSE file found in the top-level
 # directory of this distribution.
 #
 # No part of python-bitcoin-utils, including this file, may be copied, modified,
```

### Comparing `bitcoin-utils-0.6.6/bitcoinutils/transactions.py` & `bitcoin-utils-0.6.8/bitcoinutils/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2022 The python-bitcoin-utils developers
+# Copyright (C) 2018-2024 The python-bitcoin-utils developers
 #
 # This file is part of python-bitcoin-utils
 #
 # It is subject to the license terms in the LICENSE file found in the top-level
 # directory of this distribution.
 #
 # No part of python-bitcoin-utils, including this file, may be copied, modified,
@@ -30,22 +30,20 @@
     REPLACE_BY_FEE_SEQUENCE,
     TYPE_ABSOLUTE_TIMELOCK,
     TYPE_RELATIVE_TIMELOCK,
     TYPE_REPLACE_BY_FEE,
 )
 from bitcoinutils.script import Script
 from bitcoinutils.utils import (
-    to_bytes,
     vi_to_int,
     encode_varint,
     tagged_hash,
-    prepend_varint,
+    prepend_compact_size,
     h_to_b,
     b_to_h,
-    i_to_b,
 )
 
 
 class TxInput:
     """Represents a transaction input.
 
     A transaction input requires a transaction id of a UTXO and the index of
@@ -151,15 +149,15 @@
         txinputrawhex : string (hex)
             The hexadecimal raw string of the Transaction
         cursor : int
             The cursor of which the algorithm will start to read the data
         has_segwit : boolean
             Is the Tx Input segwit or not
         """
-        txinputraw = to_bytes(txinputrawhex)
+        txinputraw = h_to_b(txinputrawhex)
 
         # read the 32 bytes of TxInput ID
         inp_hash = txinputraw[cursor : cursor + 32][::-1]
 
         if not len(inp_hash):
             raise Exception(
                 "Input transaction hash not found. Probably malformed raw transaction"
@@ -232,15 +230,15 @@
         self.stack = stack
 
     def to_bytes(self) -> bytes:
         """Converts to bytes"""
         stack_bytes = b""
         for item in self.stack:
             # witness items can only be data items (hex str)
-            item_bytes = prepend_varint(h_to_b(item))
+            item_bytes = prepend_compact_size(h_to_b(item))
             stack_bytes += item_bytes
 
         return stack_bytes
 
     @classmethod
     def copy(cls, txwin: "TxWitnessInput") -> "TxWitnessInput":
         """Deep copy of TxWitnessInput"""
@@ -308,15 +306,15 @@
         txoutputrawhex : string (hex)
             The hexadecimal raw string of the Transaction
         cursor : int
             The cursor of which the algorithm will start to read the data
         has_segwit : boolean
             Is the Tx Output segwit or not
         """
-        txoutputraw = to_bytes(txoutputrawhex)
+        txoutputraw = h_to_b(txoutputrawhex)
 
         # read the amount of the TxOutput
         value = int.from_bytes(txoutputraw[cursor : cursor + 8][::-1], "big")
         cursor += 8
 
         # read the size (bytes length) of the integer representing the size of the
         # locking Script's raw data and the size of the locking Script's raw data
@@ -539,15 +537,15 @@
         Imports a Transaction from hexadecimal data
 
         Attributes
         ----------
         rawtxhex : string (hex)
             The hexadecimal raw string of the Transaction
         """
-        rawtx = to_bytes(rawtxhex)
+        rawtx = h_to_b(rawtxhex)
 
         # read version
         version = rawtx[0:4]
         flag = None
         has_segwit = False
         cursor = 4
         if rawtx[4:5] == b"\0":
@@ -765,19 +763,14 @@
              amount : int/float/Decimal
                  The amount of the UTXO to spend is included in the
                  signature for segwit (in satoshis)
              sighash : int
                  The type of the signature hash to be created
         """
 
-        # clone transaction to modify without messing up the real transaction
-        # TODO tmp_tx is not really used for its to_bytes() - we can access
-        # self directly
-        tmp_tx = Transaction.copy(self)
-
         # defaults for BIP143
         hash_prevouts = b"\x00" * 32
         hash_sequence = b"\x00" * 32
         hash_outputs = b"\x00" * 32
 
         # acquiring the signature type
         basic_sig_hash_type = sighash & 0x1F
@@ -785,48 +778,47 @@
         sign_all = (basic_sig_hash_type != SIGHASH_SINGLE) and (
             basic_sig_hash_type != SIGHASH_NONE
         )
 
         # Hash all input
         if not anyone_can_pay:
             hash_prevouts = b""
-            for txin in tmp_tx.inputs:
-                # TODO ? <L is 8 bytes, should be 4 bytes <I instead
+            for txin in self.inputs:
                 hash_prevouts += h_to_b(txin.txid)[::-1] + struct.pack(
-                    "<L",
-                    txin.txout_index,
+                    "<I", txin.txout_index
                 )
+
             hash_prevouts = hashlib.sha256(
                 hashlib.sha256(hash_prevouts).digest()
             ).digest()
 
         # Hash all input sequence
         if not anyone_can_pay and sign_all:
             hash_sequence = b""
-            for txin in tmp_tx.inputs:
+            for txin in self.inputs:
                 hash_sequence += txin.sequence
             hash_sequence = hashlib.sha256(
                 hashlib.sha256(hash_sequence).digest()
             ).digest()
 
         if sign_all:
             # Hash all output
             hash_outputs = b""
-            for txout in tmp_tx.outputs:
+            for txout in self.outputs:
                 amount_bytes = struct.pack("<q", txout.amount)
                 script_bytes = txout.script_pubkey.to_bytes()
                 hash_outputs += (
                     amount_bytes + struct.pack("B", len(script_bytes)) + script_bytes
                 )
             hash_outputs = hashlib.sha256(
                 hashlib.sha256(hash_outputs).digest()
             ).digest()
-        elif basic_sig_hash_type == SIGHASH_SINGLE and txin_index < len(tmp_tx.outputs):
+        elif basic_sig_hash_type == SIGHASH_SINGLE and txin_index < len(self.outputs):
             # Hash one output
-            txout = tmp_tx.outputs[txin_index]
+            txout = self.outputs[txin_index]
             amount_bytes = struct.pack("<q", txout.amount)
             script_bytes = txout.script_pubkey.to_bytes()
             hash_outputs = (
                 amount_bytes + struct.pack("B", len(script_bytes)) + script_bytes
             )
             hash_outputs = hashlib.sha256(
                 hashlib.sha256(hash_outputs).digest()
@@ -835,20 +827,17 @@
         # add sighash version
         tx_for_signing = self.version
 
         # add hash_prevouts and hash_sequence
         tx_for_signing += hash_prevouts + hash_sequence
 
         # add tx outpoint (utxo txid + index)
-        # TODO <L is 8 bytes, should be 4 bytes <I instead
+        # Correcting the struct.pack usage from "<L" to "<I" for explicit 4-byte packing
         txin = self.inputs[txin_index]
-        tx_for_signing += h_to_b(txin.txid)[::-1] + struct.pack(
-            "<L",
-            txin.txout_index,
-        )
+        tx_for_signing += h_to_b(txin.txid)[::-1] + struct.pack("<I", txin.txout_index)
 
         # add tx script code
         tx_for_signing += struct.pack("B", len(script.to_bytes()))
         tx_for_signing += script.to_bytes()
 
         # add txin amount
         tx_for_signing += struct.pack("<q", amount)
@@ -1007,15 +996,15 @@
 
             tx_for_signing += txin.sequence
         else:
             # print('4')
             tx_for_signing += txin_index.to_bytes(4, "little")
 
         # TODO if annex is present it should be added here
-        # length of annex should use prepend_varint (compact_size)
+        # length of annex should use compact_size
 
         # Data about this output
         if sighash_single:
             # print('5')
             txout = tmp_tx.outputs[txin_index]
             amount_bytes = struct.pack("<Q", txout.amount)
             script_bytes = txout.script_pubkey.to_bytes()
@@ -1027,15 +1016,15 @@
         if ext_flag == 1:  # script spending path (Signature Message Extension BIP-342)
             # committing the tapleaf hash - makes it safe to reuse keys for separate
             # scripts in the same output
             leaf_ver = (
                 LEAF_VERSION_TAPSCRIPT  # pass as a parameter if a new version comes
             )
             tx_for_signing += tagged_hash(
-                bytes([leaf_ver]) + prepend_varint(script.to_bytes()), "TapLeaf"
+                bytes([leaf_ver]) + prepend_compact_size(script.to_bytes()), "TapLeaf"
             )
 
             # key version - type of public key used for this signature, currently only 0
             tx_for_signing += bytes([0])
 
             # code separator position - records position of when the last
             # OP_CODESEPARATOR was executed; not supported for now, we always
```

### Comparing `bitcoin-utils-0.6.6/bitcoinutils/utils.py` & `bitcoin-utils-0.6.8/bitcoinutils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2022 The python-bitcoin-utils developers
+# Copyright (C) 2018-2024 The python-bitcoin-utils developers
 #
 # This file is part of python-bitcoin-utils
 #
 # It is subject to the license terms in the LICENSE file found in the top-level
 # directory of this distribution.
 #
 # No part of python-bitcoin-utils, including this file, may be copied, modified,
@@ -19,17 +19,16 @@
     from typing import Tuple
 
 import hashlib
 from ecdsa import ellipticcurve  # type: ignore
 from bitcoinutils.constants import SATOSHIS_PER_BITCOIN, LEAF_VERSION_TAPSCRIPT
 from bitcoinutils.schnorr import full_pubkey_gen, point_add, point_mul, G
 
-
-# TODO rename to Secp256k1Params and clean whatever is not used!
-class EcdsaParams:
+# clean whatever is not used!
+class Secp256k1Params:
     # ECDSA curve using secp256k1 is defined by: y**2 = x**3 + 7
     # This is done modulo p which (secp256k1) is:
     # p is the finite field prime number and is equal to:
     # 2^256 - 2^32 - 2^9 - 2^8 - 2^7 - 2^6 - 2^4 - 1
     # Note that we could also get that from ecdsa lib from the curve, e.g.:
     # SECP256k1.__dict__['curve'].__dict__['_CurveFp__p']
     _p = 0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFEFFFFFC2F
@@ -59,78 +58,97 @@
 class ControlBlock:
     """Represents a control block for spending a taproot script path
 
     Attributes
     ----------
     pubkey : PublicKey
         the internal public key object
-    script_to_spend : Script
-        the tapscript leaf that we want to spend
     scripts : list[ list[Script] ]
         a list of list of Scripts describing the merkle tree of scripts to commit
+    merkle_path : bytes
+        the pre-calculated merkle path
 
     Methods
     -------
     to_bytes()
         returns the control block as bytes
     to_hex()
         returns the control block as a hexadecimal string
     """
 
-    # TODO TEMP scripts is just the top root th_branch manually calculated!
-    def __init__(self, pubkey: PublicKey, script_to_spend=None, scripts=None, is_odd = False):
+    def __init__(self, pubkey: PublicKey, scripts: None | list[list[Script]], index: int, is_odd=False):
         """
         Parameters
         ----------
         pubkey : PublicKey
             the internal public key object
-        script_to_spend : Script (ignored for now)
-            the tapscript leaf that we want to spend
-        scripts : bytes
-            concatenated path (leafs/branches) hashes in bytes
+        scripts : list[list[Script]]
+            a list of list of Scripts describing the merkle tree of scripts to commit
+        index : int
+            the index of the leaf taproot using which to execute the transaction
         """
         self.pubkey = pubkey
-        # script_to_spend is ignored for now - needed for automatically
-        # constructing the merkle path
-        self.script_to_spend = script_to_spend
         self.scripts = scripts
+        self.merkle_path = b"".join(_generate_merkle_path(scripts, index))
         self.is_odd = is_odd
 
     def to_bytes(self) -> bytes:
-        leaf_version = bytes([ (1 if self.is_odd else 0) + LEAF_VERSION_TAPSCRIPT])
-
+        leaf_version = bytes([(1 if self.is_odd else 0) + LEAF_VERSION_TAPSCRIPT])
         # x-only public key is required
         pub_key = bytes.fromhex(self.pubkey.to_x_only_hex())
-
-        merkle_path = b""
-
-        # get merkle path from scripts, if any
-        # TODO currently the manually constructed merkle path is passed
-        if self.scripts:
-            merkle_path = self.scripts  # manually constructed path
-
-        return leaf_version + pub_key + merkle_path
+        return leaf_version + pub_key + self.merkle_path
 
     def to_hex(self):
         """Converts object to hexadecimal string"""
-
         return b_to_h(self.to_bytes())
+    
+def _generate_merkle_path(all_leafs, target_leaf_index):
+    """Generate the merkle path for spending a taproot path.
 
+    Parameters
+    ----------
+    all_leafs : list
+        List of all taproot leaf scripts. Can be nested.
+    target_leaf_index : int
+        Index of the target leaf script for which to generate the merkle path.
+
+    Returns
+    ----------
+    merkle_path : list
+        List of tagged hashes representing the merkle path.
+    """
+    merkle_path = []
+    traversed = 0
+    
+    def traverse_level(level):
+        nonlocal traversed
+        for leaf in level:
+            if isinstance(leaf, list):
+                traverse_level(leaf)
+            else:
+                if traversed == target_leaf_index:
+                    traversed += 1
+                    continue
+                tagged_hash = tapleaf_tagged_hash(leaf)
+                merkle_path.append(tagged_hash)
+                traversed += 1
+    
+    traverse_level(all_leafs)
+    
+    return merkle_path
 
 def get_tag_hashed_merkle_root(
     scripts: None | Script | list[Script] | list[list[Script]],
 ) -> bytes:
     """Tag hashed merkle root of all scripts - tag hashes tapleafs and branches
     as needed.
 
     Scripts is a list of list of Scripts describing the merkle tree of scripts to commit
     Example of scripts' list:  [ [A, B], C ]
     """
-    # TODO raise errors
-
     # empty scripts or empty list
     if not scripts:
         return b""
     # print('1')
     # if not list return tapleaf_hash of Script
     if not isinstance(scripts, list):
         # print('2')
@@ -145,28 +163,28 @@
             return get_tag_hashed_merkle_root(scripts[0])
         elif len(scripts) == 2:
             # print('5')
             left = get_tag_hashed_merkle_root(scripts[0])
             right = get_tag_hashed_merkle_root(scripts[1])
             return tapbranch_tagged_hash(left, right)
         else:
-            # TODO throw exception
-            exit("List cannot have more than 2 branches.")
+            # Raise an error if a branch node contains more than two elements
+            raise ValueError("Invalid Merkle branch: List cannot have more than 2 branches.")
 
 
 def to_satoshis(num: int | float | Decimal):
     """
     Converts from any number type (int/float/Decimal) to satoshis (int)
     """
     # we need to round because of how floats are stored internally:
     # e.g. 0.29 * 100000000 = 28999999.999999996
     return int(round(num * SATOSHIS_PER_BITCOIN))
 
 
-def prepend_varint(data: bytes) -> bytes:
+def prepend_compact_size(data: bytes) -> bytes:
     """
     Counts bytes and returns them with their varint (or compact size) prepended.
     """
     varint_bytes = encode_varint(len(data))
     return varint_bytes + data
 
 
@@ -188,21 +206,31 @@
     else:
         raise ValueError("Integer is too large: %d" % i)
 
 
 def is_address_bech32(address: str) -> bool:
     """
     Returns if an address (string) is bech32 or not
-    TODO improve by checking if valid, etc.
     """
-    if address.startswith("bc") or address.startswith("tb"):
-        return True
-
-    return False
-
+    if not address:
+        return False
+    
+    CHARSET = "qpzry9x8gf2tvdw0s3jn54khce6mua7l"
+    # Check if the string has valid characters
+    for char in address:
+        if char.lower() not in CHARSET:
+            return False
+    try:
+        hrp, data = address.lower().split("1")
+    except ValueError:
+        return False
+    # Check if the human-readable part (hrp) and data part are of appropriate lengths
+    if len(hrp) < 1 or len(data) < 6:
+        return False
+    return True
 
 def vi_to_int(byteint: bytes) -> Tuple[int, int]:
     """
     Converts varint bytes to int
     """
     if not isinstance(byteint, (bytes)):
         raise Exception("Byteint must be a list or defined as bytes")
@@ -212,54 +240,17 @@
         return ni, 1
     if ni == 253:  # integer of 2 bytes
         size = 2
     elif ni == 254:  # integer of 4 bytes
         size = 4
     else:  # integer of 8 bytes
         size = 8
-
     return int.from_bytes(byteint[1 : 1 + size][::-1], "big"), size + 1
 
 
-# TODO name hex_to_bytes ??
-def to_bytes(string: str, unhexlify: bool = True) -> bytes:
-    """
-    Converts a hex string to bytes
-    """
-    if not string:
-        return b""
-    if unhexlify:
-        try:
-            if isinstance(string, bytes):
-                string = string.decode()
-            s = bytes.fromhex(string)
-            return s
-        except (TypeError, ValueError):
-            pass
-    if isinstance(string, bytes):
-        return string
-    else:
-        return bytes(string, "utf8")
-
-
-def bytes32_from_int(x: int) -> bytes:
-    """
-    Converts int to 32 big-endian bytes
-    """
-    return x.to_bytes(32, byteorder="big")
-
-
-# TODO REMOVE --- NOT USED
-# def int_from_bytes(b: bytes) -> int:
-#    '''
-#    Converts int to bytes
-#    '''
-#    return int.from_bytes(b, byteorder="big")
-
-
 def add_magic_prefix(message: str) -> bytes:
     """
     Required prefix when signing a message
     """
     magic_prefix = b"\x18Bitcoin Signed Message:\n"
     # need to use varint for big messages
     # note that previously big-endian was used but varint uses little-endian
@@ -307,15 +298,15 @@
     tweak_int = b_to_i(tweak)
 
     return tweak_int
 
 
 def tapleaf_tagged_hash(script: Script) -> bytes:
     """Calculates the tagged hash for a tapleaf"""
-    script_part = bytes([LEAF_VERSION_TAPSCRIPT]) + prepend_varint(script.to_bytes())
+    script_part = bytes([LEAF_VERSION_TAPSCRIPT]) + prepend_compact_size(script.to_bytes())
     return tagged_hash(script_part, "TapLeaf")
 
 
 def tapbranch_tagged_hash(thashed_a: bytes, thashed_b: bytes) -> bytes:
     """Calculates the tagged hash for a tapbranch"""
     # order - smaller left side
     if thashed_a < thashed_b:
@@ -333,29 +324,29 @@
 
     # negate private key if necessary
     if int(pubkey_hex[64:], 16) % 2 == 0:
         negated_key = h_to_i(key.hex())
     else:
         key_secret_exponent = h_to_i(key.hex())
         # negate private key
-        negated_key = EcdsaParams._order - key_secret_exponent
+        negated_key = Secp256k1Params._order - key_secret_exponent
 
     return f"{negated_key:064x}"
 
 
 # def negate_pubkey(key: bytes) -> str:
 #    '''Negate public key, if necessary'''
 #
 #    # convert public key bytes to tuple Point
 #    x = h_to_i( key[:32].hex() )
 #    y = h_to_i( key[32:].hex() )
 #
 #    # negate public key if necessary
 #    if y % 2 != 0:
-#        y = EcdsaParams._field - y
+#        y = Secp256k1Params._field - y
 #
 #    return f'{x:064x}{y:064x}'
 
 
 def tweak_taproot_pubkey(internal_pubkey: bytes, tweak: int) -> Tuple[bytes, bool]:
     """
     Tweaks the public key with the specified tweak. Required to create the
@@ -368,27 +359,27 @@
     # convert public key bytes to tuple Point
     x = h_to_i(internal_pubkey[:32].hex())
     y = h_to_i(internal_pubkey[32:].hex())
 
     # if y is odd then negate y (effectively P) to make it even and equivalent
     # to a 02 compressed pk
     if y % 2 != 0:
-        y = EcdsaParams._field - y
+        y = Secp256k1Params._field - y
     P = (x, y)
 
     # apply tweak to public key (Q = P + th*G)
     Q = point_add(P, (point_mul(G, tweak)))
 
     # stores if it's odd to correct the control block bit
     is_odd = False
 
     # negate Q as well before returning ?!?
     if Q[1] % 2 != 0:  # type: ignore
         is_odd = True
-        Q = (Q[0], EcdsaParams._field - Q[1])  # type: ignore
+        Q = (Q[0], Secp256k1Params._field - Q[1])  # type: ignore
 
     # print(f'Tweaked Public Key: {Q[0]:064x}{Q[1]:064x}')
     return bytes.fromhex(f"{Q[0]:064x}{Q[1]:064x}"), is_odd # type: ignore
 
 
 def tweak_taproot_privkey(privkey: bytes, tweak: int) -> bytes:
     """
@@ -408,15 +399,15 @@
         negated_key = privkey.hex()
     else:
         negated_key = negate_privkey(privkey)
 
     # The tweaked private key can be computed by d + hash(P || S)
     # where d is the normal private key, P is the normal public key
     # and S is the alt script, if any (empty script, if none?? TODO)
-    tweaked_privkey_int = (h_to_i(negated_key) + tweak) % EcdsaParams._order
+    tweaked_privkey_int = (h_to_i(negated_key) + tweak) % Secp256k1Params._order
 
     # print(f'Tweaked Private Key:', hex(tweaked_privkey_int)[2:])
     return bytes.fromhex(f"{tweaked_privkey_int:064x}")
 
 
 #
 # Basic conversions between bytes (b), hexadecimal (h) and integer (i)
@@ -448,22 +439,18 @@
 
 
 # to convert hashes to ints we need byteorder BIG...
 def b_to_i(b: bytes) -> int:
     """Converts a bytes to a number"""
     return int.from_bytes(b, byteorder="big")
 
-
 def i_to_b32(i: int) -> bytes:
     """Converts a integer to bytes"""
     return i.to_bytes(32, byteorder="big")
 
-
 def i_to_b(i: int) -> bytes:
     """Converts a integer to bytes"""
-
     # determine the number of bytes required to represent the integer
     byte_length = (i.bit_length() + 7) // 8
     return i.to_bytes(byte_length, "big")
 
-
 # TODO are these required - maybe bytestoint and inttobytes are only required?!?
```

### Comparing `bitcoin-utils-0.6.6/setup.py` & `bitcoin-utils-0.6.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       author='Konstantinos Karasavvas',
       author_email='kkarasavvas@gmail.com',
       url='https://github.com/karask/python-bitcoin-utils',
       license='MIT',
       keywords='bitcoin library utilities tools',
       install_requires=[
           'base58check>=1.0.2,<2.0',
-          'ecdsa==0.17.0',
+          'ecdsa==0.18.0',
           'sympy>=1.2,<2.0',
           'python-bitcoinrpc>=1.0,<2.0',
           'hdwallet==2.2.1'
       ],
       packages=['bitcoinutils'],
       #package_data={
       #    'bitcoinutils': ['requirements.txt']
```

