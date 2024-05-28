# Comparing `tmp/ithaca_py-0.2.8.tar.gz` & `tmp/ithaca_py-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ithaca_py-0.2.8.tar", max compression
+gzip compressed data, was "ithaca_py-0.2.9.tar", max compression
```

## Comparing `ithaca_py-0.2.8.tar` & `ithaca_py-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      983 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/README.md
--rw-r--r--   0        0        0     5147 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/__init__.py
--rw-r--r--   0        0        0     3870 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/analytics.py
--rw-r--r--   0        0        0    10809 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/auth.py
--rw-r--r--   0        0        0     5589 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/calculation.py
--rw-r--r--   0        0        0     3668 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/client.py
--rw-r--r--   0        0        0     1846 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/constants.py
--rw-r--r--   0        0        0    12592 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/fundlock.py
--rw-r--r--   0        0        0      603 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/market.py
--rw-r--r--   0        0        0     7370 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/orders.py
--rw-r--r--   0        0        0     1513 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/protocol.py
--rw-r--r--   0        0        0     2406 2024-05-24 04:27:54.192906 ithaca_py-0.2.8/ithaca/socket.py
--rw-r--r--   0        0        0      929 2024-05-24 04:27:54.192906 ithaca_py-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      983 2024-05-28 16:30:13.278639 ithaca_py-0.2.9/README.md
+-rw-r--r--   0        0        0     5147 2024-05-28 16:30:13.278639 ithaca_py-0.2.9/ithaca/__init__.py
+-rw-r--r--   0        0        0     3870 2024-05-28 16:30:13.278639 ithaca_py-0.2.9/ithaca/analytics.py
+-rw-r--r--   0        0        0    10809 2024-05-28 16:30:13.278639 ithaca_py-0.2.9/ithaca/auth.py
+-rw-r--r--   0        0        0     6412 2024-05-28 16:30:13.278639 ithaca_py-0.2.9/ithaca/calculation.py
+-rw-r--r--   0        0        0     3668 2024-05-28 16:30:13.278639 ithaca_py-0.2.9/ithaca/client.py
+-rw-r--r--   0        0        0     1846 2024-05-28 16:30:13.278639 ithaca_py-0.2.9/ithaca/constants.py
+-rw-r--r--   0        0        0    12592 2024-05-28 16:30:13.278639 ithaca_py-0.2.9/ithaca/fundlock.py
+-rw-r--r--   0        0        0      603 2024-05-28 16:30:13.278639 ithaca_py-0.2.9/ithaca/market.py
+-rw-r--r--   0        0        0     7370 2024-05-28 16:30:13.278639 ithaca_py-0.2.9/ithaca/orders.py
+-rw-r--r--   0        0        0     1513 2024-05-28 16:30:13.278639 ithaca_py-0.2.9/ithaca/protocol.py
+-rw-r--r--   0        0        0     2406 2024-05-28 16:30:13.278639 ithaca_py-0.2.9/ithaca/socket.py
+-rw-r--r--   0        0        0      929 2024-05-28 16:30:13.282639 ithaca_py-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.9/PKG-INFO
```

### Comparing `ithaca_py-0.2.8/README.md` & `ithaca_py-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.8/ithaca/__init__.py` & `ithaca_py-0.2.9/ithaca/__init__.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.8/ithaca/analytics.py` & `ithaca_py-0.2.9/ithaca/analytics.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.8/ithaca/auth.py` & `ithaca_py-0.2.9/ithaca/auth.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.8/ithaca/calculation.py` & `ithaca_py-0.2.9/ithaca/calculation.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,14 +48,37 @@
             "legs": legs,
             "orderType": order_type,
             "timeInForce": time_in_force,
             "clientEthAddress": self.parent.account.address.lower(),
         }
         return self.parent.post("/clientapi/estimateOrderLock", json=order)
 
+
+    def estimate_multi_order_lock(
+        self, orders_array, order_type="LIMIT", time_in_force="GOOD_TILL_CANCEL"
+    ):
+        """Estimate lock for array of orders."""
+        payload = []
+        for legs, price in orders_array:
+            legs = [
+                {"contractId": contract_id, "quantity": qty, "side": side}
+                for contract_id, side, qty in legs
+            ]
+            order = {
+                "clientOrderId": 1,
+                "totalNetPrice": price,
+                "legs": legs,
+                "orderType": order_type,
+                "timeInForce": time_in_force,
+                "clientEthAddress": self.parent.account.address.lower(),
+            }
+            payload.append(order)
+        return self.parent.post("/clientapi/estimatePositionedOrdersLock", json=payload)
+
+
     def estimate_order_fees(
         self, legs, price, order_type="LIMIT", time_in_force="GOOD_TILL_CANCEL"
     ):
         """Estimate order fees.
 
         Args:
             legs ([type]): [description]
```

### Comparing `ithaca_py-0.2.8/ithaca/client.py` & `ithaca_py-0.2.9/ithaca/client.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.8/ithaca/constants.py` & `ithaca_py-0.2.9/ithaca/constants.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.8/ithaca/fundlock.py` & `ithaca_py-0.2.9/ithaca/fundlock.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.8/ithaca/market.py` & `ithaca_py-0.2.9/ithaca/market.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.8/ithaca/orders.py` & `ithaca_py-0.2.9/ithaca/orders.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.8/ithaca/protocol.py` & `ithaca_py-0.2.9/ithaca/protocol.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.8/ithaca/socket.py` & `ithaca_py-0.2.9/ithaca/socket.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.8/pyproject.toml` & `ithaca_py-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ithaca_py"
-version = "0.2.8"
+version = "0.2.9"
 description = "Ithaca Protocol SDK"
 authors = ["nhaga <nhaga5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ithaca"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ithaca_py-0.2.8/PKG-INFO` & `ithaca_py-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ithaca_py
-Version: 0.2.8
+Version: 0.2.9
 Summary: Ithaca Protocol SDK
 Author: nhaga
 Author-email: nhaga5@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

