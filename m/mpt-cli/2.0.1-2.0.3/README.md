# Comparing `tmp/mpt_cli-2.0.1.tar.gz` & `tmp/mpt_cli-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpt_cli-2.0.1.tar", max compression
+gzip compressed data, was "mpt_cli-2.0.3.tar", max compression
```

## Comparing `mpt_cli-2.0.1.tar` & `mpt_cli-2.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2024-04-11 14:13:39.969985 mpt_cli-2.0.1/LICENSE
--rw-r--r--   0        0        0      775 2024-04-11 15:21:09.368351 mpt_cli-2.0.1/README.md
--rw-r--r--   0        0        0     2873 2024-05-28 10:33:41.507793 mpt_cli-2.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 15:21:09.371045 mpt_cli-2.0.1/swo/__init__.py
--rw-r--r--   0        0        0       29 2024-04-19 13:58:48.870093 mpt_cli-2.0.1/swo/mpt/cli/core/accounts/__init__.py
--rw-r--r--   0        0        0     7174 2024-05-27 10:55:09.537193 mpt_cli-2.0.1/swo/mpt/cli/core/accounts/app.py
--rw-r--r--   0        0        0     3082 2024-05-27 10:55:09.537707 mpt_cli-2.0.1/swo/mpt/cli/core/accounts/flows.py
--rw-r--r--   0        0        0      163 2024-05-27 10:55:09.538191 mpt_cli-2.0.1/swo/mpt/cli/core/accounts/models.py
--rw-r--r--   0        0        0      854 2024-04-19 13:58:48.871054 mpt_cli-2.0.1/swo/mpt/cli/core/alias_group.py
--rw-r--r--   0        0        0     1791 2024-04-30 09:32:19.164668 mpt_cli-2.0.1/swo/mpt/cli/core/console.py
--rw-r--r--   0        0        0     2024 2024-05-16 12:08:01.747697 mpt_cli-2.0.1/swo/mpt/cli/core/errors.py
--rw-r--r--   0        0        0      301 2024-05-09 15:53:42.884533 mpt_cli-2.0.1/swo/mpt/cli/core/icons/fake-icon.png
--rw-r--r--   0        0        0        0 2024-04-19 13:58:48.871507 mpt_cli-2.0.1/swo/mpt/cli/core/mpt/__init__.py
--rw-r--r--   0        0        0     1515 2024-05-27 10:55:09.538682 mpt_cli-2.0.1/swo/mpt/cli/core/mpt/client.py
--rw-r--r--   0        0        0     6592 2024-05-27 10:55:09.539216 mpt_cli-2.0.1/swo/mpt/cli/core/mpt/flows.py
--rw-r--r--   0        0        0      965 2024-05-23 13:02:42.929732 mpt_cli-2.0.1/swo/mpt/cli/core/mpt/models.py
--rw-r--r--   0        0        0       29 2024-05-23 13:02:42.930189 mpt_cli-2.0.1/swo/mpt/cli/core/pricelists/__init__.py
--rw-r--r--   0        0        0     3834 2024-05-27 10:55:09.540050 mpt_cli-2.0.1/swo/mpt/cli/core/pricelists/app.py
--rw-r--r--   0        0        0     2192 2024-05-23 13:02:42.930865 mpt_cli-2.0.1/swo/mpt/cli/core/pricelists/constants.py
--rw-r--r--   0        0        0     5900 2024-05-27 10:55:09.540700 mpt_cli-2.0.1/swo/mpt/cli/core/pricelists/flows.py
--rw-r--r--   0        0        0       29 2024-04-22 13:13:18.239354 mpt_cli-2.0.1/swo/mpt/cli/core/products/__init__.py
--rw-r--r--   0        0        0     7001 2024-05-16 12:08:01.748684 mpt_cli-2.0.1/swo/mpt/cli/core/products/app.py
--rw-r--r--   0        0        0     8438 2024-05-10 15:33:21.643754 mpt_cli-2.0.1/swo/mpt/cli/core/products/constants.py
--rw-r--r--   0        0        0    27905 2024-05-27 10:55:09.541114 mpt_cli-2.0.1/swo/mpt/cli/core/products/flows.py
--rw-r--r--   0        0        0     3665 2024-05-23 13:02:42.932153 mpt_cli-2.0.1/swo/mpt/cli/core/stats.py
--rw-r--r--   0        0        0     4367 2024-05-27 10:55:09.541474 mpt_cli-2.0.1/swo/mpt/cli/core/utils.py
--rw-r--r--   0        0        0     1157 2024-05-23 13:02:42.932860 mpt_cli-2.0.1/swo/mpt/cli/swocli.py
--rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 mpt_cli-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/LICENSE
+-rw-r--r--   0        0        0      861 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/README.md
+-rw-r--r--   0        0        0     2873 2024-05-28 10:53:19.702954 mpt_cli-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/accounts/__init__.py
+-rw-r--r--   0        0        0     7402 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/accounts/app.py
+-rw-r--r--   0        0        0     3093 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/accounts/flows.py
+-rw-r--r--   0        0        0      181 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/accounts/models.py
+-rw-r--r--   0        0        0      854 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/alias_group.py
+-rw-r--r--   0        0        0     1791 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/console.py
+-rw-r--r--   0        0        0     2024 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/errors.py
+-rw-r--r--   0        0        0      301 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/icons/fake-icon.png
+-rw-r--r--   0        0        0        0 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/mpt/__init__.py
+-rw-r--r--   0        0        0     1481 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/mpt/client.py
+-rw-r--r--   0        0        0     6574 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/mpt/flows.py
+-rw-r--r--   0        0        0      965 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/mpt/models.py
+-rw-r--r--   0        0        0       29 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/pricelists/__init__.py
+-rw-r--r--   0        0        0     3930 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/pricelists/app.py
+-rw-r--r--   0        0        0     2192 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/pricelists/constants.py
+-rw-r--r--   0        0        0     6663 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/pricelists/flows.py
+-rw-r--r--   0        0        0       29 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/products/__init__.py
+-rw-r--r--   0        0        0     7001 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/products/app.py
+-rw-r--r--   0        0        0     8438 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/products/constants.py
+-rw-r--r--   0        0        0    27565 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/products/flows.py
+-rw-r--r--   0        0        0     3665 2024-05-28 10:53:10.310815 mpt_cli-2.0.3/swo/mpt/cli/core/stats.py
+-rw-r--r--   0        0        0     4747 2024-05-28 10:53:10.314815 mpt_cli-2.0.3/swo/mpt/cli/core/utils.py
+-rw-r--r--   0        0        0     1157 2024-05-28 10:53:10.314815 mpt_cli-2.0.3/swo/mpt/cli/swocli.py
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 mpt_cli-2.0.3/PKG-INFO
```

### Comparing `mpt_cli-2.0.1/LICENSE` & `mpt_cli-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.0.1/README.md` & `mpt_cli-2.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -6,7 +6,15 @@
 Command line utility for SoftwareOne Marketplace Platform
 
 # Run tests
 ```
 $ docker-compose build app_test
 $ docker-compose run --service-ports app_test
 ```
+
+# Command Line Interface
+To list all available commands use
+
+
+```
+mpt-cli --help
+```
```

### Comparing `mpt_cli-2.0.1/pyproject.toml` & `mpt_cli-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpt-cli"
-version = "2.0.1"
+version = "2.0.3"
 description = "Command line utility for SoftwareOne Marketplace Platform"
 authors = ["SoftwareOne AG"]
 license = "Apache-2.0 license"
 packages = [
     { include = "swo" }
 ]
 readme = "README.md"
@@ -27,15 +27,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.12,<4"
 openpyxl = "3.1.*"
 pydantic = "2.7.*"
 pyfiglet = "1.0.*"
-requests = "2.31.*"
+requests = "2.32.*"
 requests-toolbelt = "1.0.*"
 typer = "0.12.*"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "0.13.*"
 ipython = "8.*"
 mypy = "1.8.*"
```

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/accounts/app.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/accounts/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,19 +211,28 @@
     def _wrap_active(is_active: bool) -> str:  # pragma: no cover
         if is_active:
             return "[red bold]\u2714"
         else:
             return ""
 
     def _wrap_token(account: Account, to_wrap_secret: bool) -> str:
-        token_id, token = account.token.split(":")
+        is_new_token = "idt:TKN-" in account.token
+
+        if is_new_token:
+            token = account.token
+        else:
+            token = f"{account.token_id}:{account.token}"
+
         if to_wrap_secret:
-            token = f"{token[0:][:4]}*****{token[:4]}"
+            if is_new_token:
+                token = f"{token[0:][:22]}*****{token[:4]}"
+            else:
+                token = f"{token[0:][:4]}*****{token[:4]}"
 
-        return f"{token_id}:{token}"
+        return token
 
     for account in accounts:
         table.add_row(
             account.id,
             account.name,
             _wrap_account_type(account.type),
             _wrap_token(account, wrap_secret),
```

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/accounts/flows.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/accounts/flows.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     """
     Extracts Account from the MPT Token
     """
     return Account(
         id=token.account.id,
         name=token.account.name,
         type=token.account.type,
-        token=f"{token.id}:{token.token}",
+        token=token.token,
+        token_id=token.id,
         environment=environment,
         is_active=True,
     )
 
 
 def from_file(accounts_file_path: Path) -> list[Account]:
     """
```

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/alias_group.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/alias_group.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/console.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/console.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/errors.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/mpt/client.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/mpt/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,9 +35,8 @@
 
     def join_url(self, url: str) -> str:
         url = url[1:] if url[0] == "/" else url
         return urljoin(self.base_url, url, allow_fragments=True)
 
 
 def client_from_account(account: Account) -> MPTClient:
-    _, secret = account.token.split(":")
-    return MPTClient(account.environment, secret)
+    return MPTClient(account.environment, account.token)
```

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/mpt/flows.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/mpt/flows.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     )
     response.raise_for_status()
 
     return Parameter.model_validate(response.json())
 
 
 @wrap_http_error
-def create_item(mpt_client: MPTClient, product: Product, item_json: dict) -> Item:
+def create_item(mpt_client: MPTClient, item_json: dict) -> Item:
     response = mpt_client.post("/items", json=item_json)
     response.raise_for_status()
 
     return Item.model_validate(response.json())
 
 
 @wrap_http_error
```

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/mpt/models.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/mpt/models.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/pricelists/app.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/pricelists/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,26 +25,27 @@
     pricelists_paths: Annotated[
         list[str],
         typer.Argument(
             help="Path to Price lists definition files", metavar="PRICELISTS-PATHS"
         ),
     ],
 ):
-    file_paths = []
-    for pricelist_path in pricelists_paths:
-        path = Path(pricelist_path)
+    with console.status("Fetching pricelist files..."):
+        file_paths = []
+        for pricelist_path in pricelists_paths:
+            path = Path(pricelist_path)
 
-        if path.is_file():
-            file_paths.append(pricelist_path)
-        elif path.is_dir():
-            file_paths.extend(glob(str(path / "*")))
-        else:
-            file_paths.extend(glob(pricelist_path))
+            if path.is_file():
+                file_paths.append(pricelist_path)
+            elif path.is_dir():
+                file_paths.extend(glob(str(path / "*")))
+            else:
+                file_paths.extend(glob(pricelist_path))
 
-    file_paths = list(filter(lambda p: p.endswith(".xlsx"), file_paths))
+        file_paths = list(filter(lambda p: p.endswith(".xlsx"), file_paths))
 
     if not len(file_paths):
         console.print(
             f"No files found for provided paths {', '.join(pricelists_paths)}"
         )
         raise typer.Exit(code=3)
```

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/pricelists/constants.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/pricelists/constants.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/pricelists/flows.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/pricelists/flows.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from swo.mpt.cli.core.stats import PricelistStatsCollector
 from swo.mpt.cli.core.utils import (
     SheetValue,
     add_or_create_error,
     find_value_for,
     get_values_for_general,
     get_values_for_table,
+    status_step_text,
 )
 
 
 class PricelistAction(enum.Enum):
     CREATE = "create"
     UPDATE = "update"
 
@@ -75,41 +76,42 @@
     mpt_client: MPTClient,
     wb: Workbook,
     action: PricelistAction,
     active_account: Account,
     stats: PricelistStatsCollector,
     console: Console,
 ) -> tuple[PricelistStatsCollector, Optional[Pricelist]]:
-    general_ws = wb[constants.TAB_GENERAL]
-    general_values = get_values_for_general(general_ws, constants.GENERAL_FIELDS)
+    with console.status("Sync Pricelist..."):
+        general_ws = wb[constants.TAB_GENERAL]
+        general_values = get_values_for_general(general_ws, constants.GENERAL_FIELDS)
 
-    if active_account.type == "Operations":
-        pricelist_json = to_operations_pricelist_json(general_values)
-    else:
-        pricelist_json = to_vendor_pricelist_json(general_values)
-
-    try:
-        if action == PricelistAction.CREATE:
-            pricelist = create_pricelist(
-                mpt_client,
-                pricelist_json,
-            )
+        if active_account.type == "Operations":
+            pricelist_json = to_operations_pricelist_json(general_values)
         else:
-            pricelist_id = find_value_for(
-                constants.GENERAL_PRICELIST_ID, general_values
-            )[2]
-            pricelist = update_pricelist(
-                mpt_client,
-                pricelist_id,
-                pricelist_json,
-            )
-    except Exception as e:
-        add_or_create_error(general_ws, general_values, e)
-        stats.add_error(constants.TAB_GENERAL)
-        return stats, None
+            pricelist_json = to_vendor_pricelist_json(general_values)
+
+        try:
+            if action == PricelistAction.CREATE:
+                pricelist = create_pricelist(
+                    mpt_client,
+                    pricelist_json,
+                )
+            else:
+                pricelist_id = find_value_for(
+                    constants.GENERAL_PRICELIST_ID, general_values
+                )[2]
+                pricelist = update_pricelist(
+                    mpt_client,
+                    pricelist_id,
+                    pricelist_json,
+                )
+        except Exception as e:
+            add_or_create_error(general_ws, general_values, e)
+            stats.add_error(constants.TAB_GENERAL)
+            return stats, None
 
     index, _, _ = find_value_for(constants.GENERAL_PRICELIST_ID, general_values)
     general_ws[index] = pricelist.id
     stats.add_synced(constants.TAB_GENERAL)
 
     stats = sync_pricelist_items(
         mpt_client,
@@ -123,17 +125,22 @@
     return stats, pricelist
 
 
 def to_operations_priceitem_json(values: list[SheetValue]) -> dict:
     status = find_value_for(constants.PRICELIST_ITEMS_STATUS, values)[2]
     priceitem_json = {
         "markup": find_value_for(constants.PRICELIST_ITEMS_MARKUP, values)[2],
-        "unitSP": find_value_for(constants.PRICELIST_ITEMS_UNIT_SP, values)[2],
+        "unitLP": find_value_for(constants.PRICELIST_ITEMS_UNIT_LP, values)[2],
+        "unitPP": find_value_for(constants.PRICELIST_ITEMS_UNIT_PP, values)[2],
     }
 
+    unit_sp = find_value_for(constants.PRICELIST_ITEMS_UNIT_SP, values)
+    if unit_sp and unit_sp[2] is not None:
+        priceitem_json["unitSP"] = unit_sp[2]
+
     if status != "Draft":
         priceitem_json["status"] = status
 
     return priceitem_json
 
 
 def to_vendor_priceitem_json(values: list[SheetValue]) -> dict:
@@ -148,41 +155,47 @@
     mpt_client: MPTClient,
     ws: Worksheet,
     pricelist_id: str,
     active_account: Account,
     stats: PricelistStatsCollector,
     console: Console,
 ) -> PricelistStatsCollector:
-    values = get_values_for_table(ws, constants.PRICELIST_ITEMS_FIELDS)
-
-    for sheet_value in values:
-        try:
-            action = PricelistItemAction(
-                find_value_for(constants.PRICELIST_ITEMS_ACTION, sheet_value)[2]
-            )
-
-            if action != PricelistItemAction.UPDATE:
-                stats.add_skipped(constants.TAB_PRICE_ITEMS)
-                continue
-
-            vendor_id = find_value_for(
-                constants.PRICELIST_ITEMS_ITEM_VENDOR_ID, sheet_value
-            )[2]
-            pricelist_item = get_pricelist_item(mpt_client, pricelist_id, vendor_id)
+    with console.status("Sync Pricelist Items...") as status:
+        values = get_values_for_table(ws, constants.PRICELIST_ITEMS_FIELDS)
 
-            if active_account.type == "Operations":
-                pricelist_item_json = to_operations_priceitem_json(sheet_value)
-            else:
-                pricelist_item_json = to_vendor_priceitem_json(sheet_value)
-
-            pricelist_item = update_pricelist_item(
-                mpt_client, pricelist_id, pricelist_item.id, pricelist_item_json
-            )
-
-            index_id, _, _ = find_value_for(constants.PRICELIST_ITEMS_ID, sheet_value)
-            ws[index_id] = pricelist_item.id
-            stats.add_synced(constants.TAB_PRICE_ITEMS)
-        except Exception as e:
-            add_or_create_error(ws, sheet_value, e)
-            stats.add_error(constants.TAB_PRICE_ITEMS)
+        for sheet_value in values:
+            try:
+                action = PricelistItemAction(
+                    find_value_for(constants.PRICELIST_ITEMS_ACTION, sheet_value)[2]
+                )
+
+                if action != PricelistItemAction.UPDATE:
+                    stats.add_skipped(constants.TAB_PRICE_ITEMS)
+                    continue
+
+                vendor_id = find_value_for(
+                    constants.PRICELIST_ITEMS_ITEM_VENDOR_ID, sheet_value
+                )[2]
+                pricelist_item = get_pricelist_item(mpt_client, pricelist_id, vendor_id)
+
+                if active_account.type == "Operations":
+                    pricelist_item_json = to_operations_priceitem_json(sheet_value)
+                else:
+                    pricelist_item_json = to_vendor_priceitem_json(sheet_value)
+
+                pricelist_item = update_pricelist_item(
+                    mpt_client, pricelist_id, pricelist_item.id, pricelist_item_json
+                )
+
+                index_id, _, _ = find_value_for(
+                    constants.PRICELIST_ITEMS_ID, sheet_value
+                )
+                ws[index_id] = pricelist_item.id
+                stats.add_synced(constants.TAB_PRICE_ITEMS)
+            except Exception as e:
+                add_or_create_error(ws, sheet_value, e)
+                stats.add_error(constants.TAB_PRICE_ITEMS)
+            finally:
+                step_text = status_step_text(stats, ws.title)
+                status.update(f"Syncing {ws.title}: {step_text}")
 
     return stats
```

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/products/app.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/products/app.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/products/constants.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/products/constants.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/products/flows.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/products/flows.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     find_value_for,
     find_values_by_pattern,
     get_values_for_dynamic_table,
     get_values_for_general,
     get_values_for_table,
     set_dict_value,
     set_value,
+    status_step_text,
 )
 
 T = TypeVar("T")
 SyncResult: TypeAlias = tuple[Worksheet, dict[str, T]]
 
 
 class ProductAction(enum.Enum):
@@ -353,25 +354,14 @@
         "name": find_value_for(constants.TEMPLATES_NAME, values)[2],
         "type": find_value_for(constants.TEMPLATES_TYPE, values)[2],
         "content": find_value_for(constants.TEMPLATES_CONTENT, values)[2],
         "default": find_value_for(constants.TEMPLATES_DEFAULT, values)[2] == "True",
     }
 
 
-def status_step_text(stats: ProductStatsCollector, tab_name: str) -> str:
-    results = stats.tabs[tab_name]
-
-    return (
-        f"[green]{results['synced']}[/green] / "
-        f"[red bold]{results['error']}[/red bold] / "
-        f"[white bold]{results['skipped']}[/white bold] / "
-        f"[blue]{results['total']}[/blue]"
-    )
-
-
 def sync_product_definition(
     mpt_client: MPTClient,
     definition_path: Path,
     action: ProductAction,
     active_account: Account,
     stats: ProductStatsCollector,
     status: Status,
@@ -765,15 +755,14 @@
     id_mapping = {}
 
     for sheet_value in values:
         try:
             sheet_value = setup_unit_of_measure(mpt_client, sheet_value)
             item = create_item(
                 mpt_client,
-                product,
                 to_item_create_json(
                     product.id,
                     items_groups_mapping,
                     item_parameters_id_mapping,
                     sheet_value,
                 ),
             )
```

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/stats.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/stats.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/core/utils.py` & `mpt_cli-2.0.3/swo/mpt/cli/core/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from typing import Any, Generator, Pattern, TypeAlias
 
 from openpyxl.utils import get_column_letter  # type: ignore
 from openpyxl.utils.cell import coordinate_from_string  # type: ignore
 from openpyxl.worksheet.worksheet import Worksheet  # type: ignore
+from swo.mpt.cli.core.stats import StatsCollector
 
 SheetValue: TypeAlias = tuple[str, str, Any]
 SheetValueGenerator: TypeAlias = Generator[list[SheetValue], None, None]
 
 
 # TODO: add typehints here
 def find_first(func, iterable, default=None):
@@ -152,7 +153,18 @@
         ws[f"{column_letter}1"] = "Error"
 
     index, _, _ = sheet_value[0]
     row_number = coordinate_from_string(index)[1]
     ws[f"{column_letter}{row_number}"] = str(exception)
 
     return ws
+
+
+def status_step_text(stats: StatsCollector, tab_name: str) -> str:
+    results = stats.tabs[tab_name]
+
+    return (
+        f"[green]{results['synced']}[/green] / "
+        f"[red bold]{results['error']}[/red bold] / "
+        f"[white bold]{results['skipped']}[/white bold] / "
+        f"[blue]{results['total']}[/blue]"
+    )
```

### Comparing `mpt_cli-2.0.1/swo/mpt/cli/swocli.py` & `mpt_cli-2.0.3/swo/mpt/cli/swocli.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.0.1/PKG-INFO` & `mpt_cli-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpt-cli
-Version: 2.0.1
+Version: 2.0.3
 Summary: Command line utility for SoftwareOne Marketplace Platform
 License: Apache-2.0 license
 Keywords: fulfillment,command,line,interface,utility,cli,softwareone,marketplace
 Author: SoftwareOne AG
 Requires-Python: >=3.12,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -12,15 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: openpyxl (==3.1.*)
 Requires-Dist: pydantic (==2.7.*)
 Requires-Dist: pyfiglet (==1.0.*)
-Requires-Dist: requests (==2.31.*)
+Requires-Dist: requests (==2.32.*)
 Requires-Dist: requests-toolbelt (==1.0.*)
 Requires-Dist: typer (==0.12.*)
 Description-Content-Type: text/markdown
 
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=softwareone-platform_swo-marketplace-cli&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=softwareone-platform_swo-marketplace-cli) [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=softwareone-platform_swo-marketplace-cli&metric=coverage)](https://sonarcloud.io/summary/new_code?id=softwareone-platform_swo-marketplace-cli)
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
@@ -30,7 +30,15 @@
 
 # Run tests
 ```
 $ docker-compose build app_test
 $ docker-compose run --service-ports app_test
 ```
 
+# Command Line Interface
+To list all available commands use
+
+
+```
+mpt-cli --help
+```
+
```

