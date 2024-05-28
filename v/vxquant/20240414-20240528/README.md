# Comparing `tmp/vxquant-20240414.tar.gz` & `tmp/vxquant-20240528.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vxquant-20240414.tar", max compression
+gzip compressed data, was "vxquant-20240528.tar", max compression
```

## Comparing `vxquant-20240414.tar` & `vxquant-20240528.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1877 2024-04-24 04:34:07.271188 vxquant-20240414/pyproject.toml
--rw-r--r--   0        0        0        9 2024-03-09 11:57:35.000000 vxquant-20240414/README.md
--rw-r--r--   0        0        0        0 2024-03-21 01:51:48.150714 vxquant-20240414/src/vxcollector/__init__.py
--rw-r--r--   0        0        0     2296 2024-03-21 03:01:25.422696 vxquant-20240414/src/vxcollector/__main__.py
--rw-r--r--   0        0        0        0 2024-03-21 02:48:35.252540 vxquant-20240414/src/vxcollector/init_mod/__init__.py
--rw-r--r--   0        0        0     7018 2024-03-31 05:46:55.667301 vxquant-20240414/src/vxcollector/init_mod/start_up.py
--rw-r--r--   0        0        0        0 2024-03-21 02:43:31.789778 vxquant-20240414/src/vxcollector/mod/__init__.py
--rw-r--r--   0        0        0      407 2024-03-21 02:48:11.599024 vxquant-20240414/src/vxcollector/mod/start_up.py
--rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxquant-20240414/src/vxcollector/py.typed
--rw-r--r--   0        0        0        0 2024-03-01 13:26:50.522744 vxquant-20240414/src/vxquant/__init__.py
--rw-r--r--   0        0        0     5322 2024-04-14 08:25:39.535966 vxquant-20240414/src/vxquant/__main__.py
--rw-r--r--   0        0        0     1026 2024-03-02 03:35:54.729169 vxquant-20240414/src/vxquant/exceptions.py
--rw-r--r--   0        0        0     7563 2024-04-14 07:10:13.802634 vxquant-20240414/src/vxquant/mdapi.py
--rw-r--r--   0        0        0        1 2024-03-09 14:37:11.000000 vxquant-20240414/src/vxquant/models/__init__.py
--rw-r--r--   0        0        0    11484 2024-04-25 07:03:19.266835 vxquant-20240414/src/vxquant/models/base.py
--rw-r--r--   0        0        0     3910 2024-03-09 12:41:00.040710 vxquant-20240414/src/vxquant/models/constants.py
--rw-r--r--   0        0        0     3736 2024-03-19 06:26:36.698404 vxquant-20240414/src/vxquant/models/industry.py
--rw-r--r--   0        0        0    11658 2024-03-20 05:53:35.455372 vxquant-20240414/src/vxquant/models/instruments.py
--rw-r--r--   0        0        0     3042 2024-04-30 06:06:01.702259 vxquant-20240414/src/vxquant/models/nomalize.py
--rw-r--r--   0        0        0    12548 2024-04-30 06:09:51.332634 vxquant-20240414/src/vxquant/models/preset.py
--rw-r--r--   0        0        0        0 2024-03-09 12:47:51.000000 vxquant-20240414/src/vxquant/providers/__init__.py
--rw-r--r--   0        0        0     2997 2024-03-20 06:09:46.192349 vxquant-20240414/src/vxquant/providers/bsproviders.py
--rw-r--r--   0        0        0        0 2024-04-15 01:28:38.285351 vxquant-20240414/src/vxquant/providers/miniqmt/__init__.py
--rw-r--r--   0        0        0     7312 2024-04-25 06:59:35.557211 vxquant-20240414/src/vxquant/providers/miniqmt/adapters.py
--rw-r--r--   0        0        0    10228 2024-04-30 06:35:35.543215 vxquant-20240414/src/vxquant/providers/miniqmt/base.py
--rw-r--r--   0        0        0     1948 2024-03-31 06:22:33.395459 vxquant-20240414/src/vxquant/providers/spiders.py
--rw-r--r--   0        0        0        0 2024-03-31 06:20:15.881547 vxquant-20240414/src/vxquant/providers/tsproviders.py
--rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxquant-20240414/src/vxquant/py.typed
--rw-r--r--   0        0        0     7194 2024-04-26 03:17:05.458452 vxquant-20240414/src/vxquant/tdapi.py
--rw-r--r--   0        0        0     8518 2024-04-07 01:35:53.845511 vxquant-20240414/src/vxquant/teller.py
--rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 vxquant-20240414/PKG-INFO
+-rw-r--r--   0        0        0     1877 2024-05-28 05:28:11.273207 vxquant-20240528/pyproject.toml
+-rw-r--r--   0        0        0        9 2024-03-09 11:57:35.000000 vxquant-20240528/README.md
+-rw-r--r--   0        0        0        0 2024-03-21 01:51:48.150714 vxquant-20240528/src/vxcollector/__init__.py
+-rw-r--r--   0        0        0     2296 2024-03-21 03:01:25.422696 vxquant-20240528/src/vxcollector/__main__.py
+-rw-r--r--   0        0        0        0 2024-03-21 02:48:35.252540 vxquant-20240528/src/vxcollector/init_mod/__init__.py
+-rw-r--r--   0        0        0     7018 2024-03-31 05:46:55.667301 vxquant-20240528/src/vxcollector/init_mod/start_up.py
+-rw-r--r--   0        0        0        0 2024-03-21 02:43:31.789778 vxquant-20240528/src/vxcollector/mod/__init__.py
+-rw-r--r--   0        0        0      407 2024-03-21 02:48:11.599024 vxquant-20240528/src/vxcollector/mod/start_up.py
+-rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxquant-20240528/src/vxcollector/py.typed
+-rw-r--r--   0        0        0        0 2024-03-01 13:26:50.522744 vxquant-20240528/src/vxquant/__init__.py
+-rw-r--r--   0        0        0     5322 2024-04-14 08:25:39.535966 vxquant-20240528/src/vxquant/__main__.py
+-rw-r--r--   0        0        0     1026 2024-03-02 03:35:54.729169 vxquant-20240528/src/vxquant/exceptions.py
+-rw-r--r--   0        0        0     7563 2024-04-14 07:10:13.802634 vxquant-20240528/src/vxquant/mdapi.py
+-rw-r--r--   0        0        0        1 2024-03-09 14:37:11.000000 vxquant-20240528/src/vxquant/models/__init__.py
+-rw-r--r--   0        0        0    11586 2024-05-28 05:27:34.819002 vxquant-20240528/src/vxquant/models/base.py
+-rw-r--r--   0        0        0     3910 2024-03-09 12:41:00.040710 vxquant-20240528/src/vxquant/models/constants.py
+-rw-r--r--   0        0        0     3736 2024-03-19 06:26:36.698404 vxquant-20240528/src/vxquant/models/industry.py
+-rw-r--r--   0        0        0    11658 2024-03-20 05:53:35.455372 vxquant-20240528/src/vxquant/models/instruments.py
+-rw-r--r--   0        0        0     3042 2024-04-30 06:06:01.702259 vxquant-20240528/src/vxquant/models/nomalize.py
+-rw-r--r--   0        0        0    12548 2024-04-30 06:09:51.332634 vxquant-20240528/src/vxquant/models/preset.py
+-rw-r--r--   0        0        0        0 2024-03-09 12:47:51.000000 vxquant-20240528/src/vxquant/providers/__init__.py
+-rw-r--r--   0        0        0     2997 2024-03-20 06:09:46.192349 vxquant-20240528/src/vxquant/providers/bsproviders.py
+-rw-r--r--   0        0        0        0 2024-04-15 01:28:38.285351 vxquant-20240528/src/vxquant/providers/miniqmt/__init__.py
+-rw-r--r--   0        0        0     7328 2024-05-27 10:45:56.449478 vxquant-20240528/src/vxquant/providers/miniqmt/adapters.py
+-rw-r--r--   0        0        0    10910 2024-05-10 01:30:57.690333 vxquant-20240528/src/vxquant/providers/miniqmt/base.py
+-rw-r--r--   0        0        0     1948 2024-03-31 06:22:33.395459 vxquant-20240528/src/vxquant/providers/spiders.py
+-rw-r--r--   0        0        0        0 2024-03-31 06:20:15.881547 vxquant-20240528/src/vxquant/providers/tsproviders.py
+-rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxquant-20240528/src/vxquant/py.typed
+-rw-r--r--   0        0        0     6924 2024-05-27 10:43:38.590147 vxquant-20240528/src/vxquant/tdapi.py
+-rw-r--r--   0        0        0     8518 2024-04-07 01:35:53.845511 vxquant-20240528/src/vxquant/teller.py
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 vxquant-20240528/PKG-INFO
```

### Comparing `vxquant-20240414/pyproject.toml` & `vxquant-20240528/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vxquant"
-version = "20240414"
+version = "20240528"
 description = "一个简单、易用、面向中国股市实盘的python量化交易框架"
 license = "MIT"
 authors = ["vex1023 <vex1023@qq.com>"]
 homepage = "https://gitee.com/vxquant/vxquant"
 keywords = ["quant", "tools"]
 readme = "README.md"
```

### Comparing `vxquant-20240414/src/vxcollector/__main__.py` & `vxquant-20240528/src/vxcollector/__main__.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/src/vxcollector/init_mod/start_up.py` & `vxquant-20240528/src/vxcollector/init_mod/start_up.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/src/vxquant/__main__.py` & `vxquant-20240528/src/vxquant/__main__.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/src/vxquant/exceptions.py` & `vxquant-20240528/src/vxquant/exceptions.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/src/vxquant/mdapi.py` & `vxquant-20240528/src/vxquant/mdapi.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/src/vxquant/models/base.py` & `vxquant-20240528/src/vxquant/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,19 @@
                 if self.allow_t0
                 else self.volume_his - self.frozen
             ),
         )
 
     @computed_field(title="VWAP", description="持仓均价")
     def vwap(self) -> float:
-        return self.cost / (self.volume_today + self.volume_his)
+        return (
+            self.cost / (self.volume_today + self.volume_his)
+            if (self.volume_today + self.volume_his) > 0
+            else 0.0
+        )
 
     @computed_field(title="PnL", description="浮动盈亏")
     def fpnl(self) -> float:
         return self.lasttrade * (self.volume_today + self.volume_his) - self.cost
 
 
 class VXCashInfo(VXDataModel):
```

### Comparing `vxquant-20240414/src/vxquant/models/constants.py` & `vxquant-20240528/src/vxquant/models/constants.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/src/vxquant/models/industry.py` & `vxquant-20240528/src/vxquant/models/industry.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/src/vxquant/models/instruments.py` & `vxquant-20240528/src/vxquant/models/instruments.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/src/vxquant/models/nomalize.py` & `vxquant-20240528/src/vxquant/models/nomalize.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/src/vxquant/models/preset.py` & `vxquant-20240528/src/vxquant/models/preset.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/src/vxquant/providers/bsproviders.py` & `vxquant-20240528/src/vxquant/providers/bsproviders.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/src/vxquant/providers/miniqmt/adapters.py` & `vxquant-20240528/src/vxquant/providers/miniqmt/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 if __name__ == "__main__":
 
     import time
     from xtquant.xttrader import XtQuantTrader, XtQuantTraderCallback
     from xtquant.xttype import StockAccount
     from xtquant import xtconstant
 
-    path = "D:\\兴业证券SMT-Q\\userdata_mini"
+    path = """D:\\兴业证券SMT-Q实盘交易\\userdata_mini"""
     session_id = int(time.time())
     xt_trader = XtQuantTrader(path, session_id)
     acc = StockAccount("20061359")
     xt_trader.start()
     connect_result = xt_trader.connect()
     print(connect_result)
     subscribe_result = xt_trader.subscribe(acc)
```

### Comparing `vxquant-20240414/src/vxquant/providers/miniqmt/base.py` & `vxquant-20240528/src/vxquant/providers/miniqmt/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,29 @@
         for xt_order in xt_orders:
             order = miniqmt_order_adapter(xt_order)
             self._context["orders"][order.order_id] = order
 
         return list(self._context["orders"].values())
 
 
+class VXMiniQMTGetExecRptProvider(VXGetExecRptProvider):
+    def __call__(
+        self,
+        *,
+        account_id: str = "default",
+        df: bool = False,
+    ) -> Union[List[VXOrder], pl.DataFrame]:
+        xt_execrpts = self._context.xt_trader.query_stock_trades()
+        execrpts = [miniqmt_execrpt_adapter(xt_execrpt) for xt_execrpt in xt_execrpts]
+        if df:
+            return pl.DataFrame([execrpt.model_dump() for execrpt in execrpts])
+        else:
+            return execrpts
+
+
 class XtQuantAccountType(Enum):
     FUTURE_ACCOUNT = xtconstant.FUTURE_ACCOUNT
     SECURITY_ACCOUNT = xtconstant.SECURITY_ACCOUNT
     CREDIT_ACCOUNT = xtconstant.CREDIT_ACCOUNT
     FUTURE_OPTION_ACCOUNT = xtconstant.FUTURE_OPTION_ACCOUNT
     STOCK_OPTION_ACCOUNT = xtconstant.STOCK_OPTION_ACCOUNT
     HUGANGTONG_ACCOUNT = xtconstant.HUGANGTONG_ACCOUNT
@@ -215,14 +230,18 @@
             "mod_path": "vxquant.providers.miniqmt.base.VXMiniQMTGetPositionProvider",
             "params": {},
         },
         "get_account": {
             "mod_path": "vxquant.providers.miniqmt.base.VXMiniQMTGetAccountProvider",
             "params": {},
         },
+        "get_order": {
+            "mod_path": "vxquant.providers.miniqmt.base.VXMiniQMTGetOrderProvider",
+            "params": {},
+        },
     }
 
     def __init__(
         self,
         miniqmt_path: str,
         account_id: str,
         account_type: Literal[
@@ -253,19 +272,19 @@
         super().__init__(context=context)
 
 
 if __name__ == "__main__":
     loggerConfig("INFO")
     context = VXContext()
     trader = VXMiniQMTTdAPI(
-        miniqmt_path="D:\\兴业证券SMT-Q\\userdata_mini", account_id="20061359"
+        miniqmt_path="D:\\兴业证券SMT-Q实盘交易\\userdata_mini", account_id="2660007522"
     )
-    positions = trader.get_positions(account_id="20061359", df=True)
+    positions = trader.get_positions(account_id="2660007522", df=True)
     print(positions)
-    accountinfo = trader.get_account(account_id="20061359")
+    accountinfo = trader.get_account(account_id="2660007522")
     print(accountinfo)
     ticks = trader.current(["399001.SZ", "399905.SZ", "000001.SZ", "000002.SZ"])
     positions = positions.select(["symbol", "market_value", "available"])
     ticks = ticks.select(["symbol", "lasttrade", "yclose"])
     print(positions.join(ticks, on="symbol", how="left"))
     print(ticks.join(positions, on="symbol", how="left").fill_null(0))
```

### Comparing `vxquant-20240414/src/vxquant/providers/spiders.py` & `vxquant-20240528/src/vxquant/providers/spiders.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/src/vxquant/tdapi.py` & `vxquant-20240528/src/vxquant/tdapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """tdapi"""
 
 import polars as pl
 from typing import Any, Dict, Optional, Union, List
 from multiprocessing import Lock
 from vxutils import VXContext
-from vxutils.provider import AbstractProvider, AbstractProviderCollection
+from vxutils.provider import (
+    AbstractProvider,
+    AbstractProviderCollection,
+    ProviderConfig,
+)
 from vxquant.models.base import VXTick
 from vxquant.models.base import VXOrder, VXCashInfo, VXPosition, VXExecRpt
 from vxquant.models.preset import VXMarketPreset
 from vxquant.models.nomalize import to_symbol
 
 __all__ = [
     "VXTdAPI",
@@ -37,21 +41,26 @@
             "params": {},
         },
         "get_account": {
             "mod_path": "vxquant.tdapi.VXGetAccountProvider",
             "params": {},
         },
     }
+    current: "VXHQCallBackProvider"
+    order_batch: "VXOrderBatchProvider"
+    get_positions: "VXGetPositionProvider"
+    get_orders: "VXGetOrderProvider"
+    get_execrpts: "VXGetExecRptProvider"
+    get_account: "VXGetAccountProvider"
 
     def order_volume(
         self,
         symbol: str,
         volume: int,
         price: Optional[float] = None,
-        account_id: Optional[str] = None,
     ) -> VXOrder:
         """下单函数
 
         Arguments:
             symbol {str} -- 证券代码
             volume {int} -- 下单数量，正数为买，负数为卖
             price {Optional[float]} -- 委托价格 (default: {None})
@@ -65,18 +74,18 @@
             "Market"
             if price is None
             and VXMarketPreset(symbol=symbol).security_type.name == "BOND_CONVERTIBLE"
             else "Limit"
         )
         if price is None:
             ticks = self.current(symbol).filter(pl.col("symbol") == symbol)
-            price = ticks["ask1"][0] if order_side == "Buy" else ticks["bid1"][0]
+            price = ticks["ask1_p"][0] if order_side == "Buy" else ticks["bid1"][0]
 
         order = VXOrder(
-            account_id=account_id or "default",
+            account_id=self.context.account_id,
             symbol=symbol,
             volume=abs(volume),
             price=price,
             order_side=order_side,
             order_type=order_type,
         )
         return self.order_batch([order], df=False).values()[0]
@@ -89,23 +98,28 @@
         """启动函数"""
         super().start_up(context)
 
         data: Dict[str, List[Any]] = {col: [] for col in VXTick.model_fields.keys()}
         self._ticks = pl.DataFrame(data)
         self._lock = Lock()
 
-    def __call__(self, *symbols: List[str]) -> pl.DataFrame:
+    def __call__(
+        self, *symbols: str, df: bool = False
+    ) -> Union[pl.DataFrame, Dict[str, VXTick]]:
         """行情回调函数"""
         if len(symbols) == 1 and isinstance(symbols[0], list):
             symbols = symbols[0]
 
         with self._lock:
-            return self._ticks.filter(pl.col("symbol").is_in(symbols))
+            ticks = self._ticks.filter(pl.col("symbol").is_in(symbols))
+            if df:
+                return ticks
+            return {row["symbol"]: VXTick(**row) for row in ticks.rows(named=True)}
 
-    def on_tick(self, ticks: pl.DataFrame) -> None:
+    def on_price_change(self, ticks: pl.DataFrame) -> None:
         """行情回调函数"""
         if ticks.shape[0] == 0:
             return
 
         with self._lock:
             self._ticks = pl.concat(
                 [
@@ -126,62 +140,49 @@
         Arguments:
             orders {List[VXOrder]} -- 订单列表
             df {bool} -- 是否返回DataFrame (default: {False})
 
         Returns:
             Union[VXOrder, pl.DataFrame]  -- 委托订单信息
         """
-        ret_orders = self._place_order(orders)
-        return (
-            pl.DataFrame([order.model_dump() for order in ret_orders.values()])
-            if df
-            else ret_orders
-        )
-
-    def _place_order(self, orders: List[VXOrder]) -> Dict[str, VXOrder]:
-        """实际下单函数"""
         raise NotImplementedError
 
 
 class VXOrderCancelProvider(AbstractProvider):
-    def __call__(self, order_id: str) -> VXOrder:
+    def __call__(self, order_id: str) -> str:
         """撤单函数
 
         Arguments:
             order_id {str} -- 订单ID
 
         Returns:
-            VXOrder -- 返回撤单订单信息
+            str -- 返回撤单订单id
         """
         raise NotImplementedError
 
 
 class VXGetAccountProvider(AbstractProvider):
     """获取账户信息接口"""
 
-    def __call__(self, account_id: str = "default") -> VXCashInfo:
+    def __call__(self) -> VXCashInfo:
         """获取账户信息
 
-        Keyword Arguments:
-            account_id {str} -- 账户ID (default: {"default"})
-
         Returns:
             Any -- 账户信息
         """
         raise NotImplementedError
 
 
 class VXGetOrderProvider(AbstractProvider):
     """获取订单信息接口"""
 
     def __call__(
         self,
         order_id: str = "",
         *,
-        account_id: str = "default",
         is_finished: bool = False,
         df: bool = False,
     ) -> Union[List[VXOrder], pl.DataFrame]:
         """获取订单信息
 
         Keyword Arguments:
             order_id: str -- 订单ID (default: {""})
@@ -195,38 +196,34 @@
         raise NotImplementedError
 
 
 class VXGetPositionProvider(AbstractProvider):
     """获取持仓信息接口"""
 
     def __call__(
-        self, account_id: str = "default", account_type: str = "STOCK", df: bool = False
+        self, symbol: Optional[str] = None, df: bool = False
     ) -> Union[Dict[str, VXPosition], pl.DataFrame]:
         """获取持仓信息
 
-        Keyword Arguments:
-            account_id {str} -- 账户ID (default: {"default"})
-
         Returns:
             Union[List[VXPosition],pl.DataFrame] -- 持仓信息
         """
         raise NotImplementedError
 
 
 class VXGetExecRptProvider(AbstractProvider):
     """获取成交信息接口"""
 
     def __call__(
-        self, execrpt_id: str = "", *, account_id: str = "default", df: bool = False
+        self, execrpt_id: str = "", *, df: bool = False
     ) -> Union[List[VXExecRpt], pl.DataFrame]:
         """获取成交信息
 
         Keyword Arguments:
             execrpt_id {str} -- 成交信息订单号 (default: {""})
-            account_id {str} -- 账户id (default: {"default"})
             df {bool} -- 是否返回dataframe格式 (default: {False})
 
         Returns:
             Union[List[VXExecRpt], pl.DataFrame] -- 成交信息
         """
         raise NotImplementedError
```

### Comparing `vxquant-20240414/src/vxquant/teller.py` & `vxquant-20240528/src/vxquant/teller.py`

 * *Files identical despite different names*

### Comparing `vxquant-20240414/PKG-INFO` & `vxquant-20240528/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vxquant
-Version: 20240414
+Version: 20240528
 Summary: 一个简单、易用、面向中国股市实盘的python量化交易框架
 Home-page: https://gitee.com/vxquant/vxquant
 License: MIT
 Keywords: quant,tools
 Author: vex1023
 Author-email: vex1023@qq.com
 Requires-Python: >=3.8,<4.0
```

