# Comparing `tmp/vanguard_api-0.1.2.tar.gz` & `tmp/vanguard_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanguard_api-0.1.2.tar", last modified: Wed May 22 16:54:54 2024, max compression
+gzip compressed data, was "vanguard_api-0.1.4.tar", last modified: Tue May 28 02:12:50 2024, max compression
```

## Comparing `vanguard_api-0.1.2.tar` & `vanguard_api-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:54:54.958423 vanguard_api-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-22 16:54:50.000000 vanguard_api-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-22 16:54:54.958423 vanguard_api-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-22 16:54:50.000000 vanguard_api-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:54:54.958423 vanguard_api-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-22 16:54:50.000000 vanguard_api-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:54:54.954424 vanguard_api-0.1.2/vanguard/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 16:54:50.000000 vanguard_api-0.1.2/vanguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-05-22 16:54:50.000000 vanguard_api-0.1.2/vanguard/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    13291 2024-05-22 16:54:50.000000 vanguard_api-0.1.2/vanguard/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-22 16:54:50.000000 vanguard_api-0.1.2/vanguard/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-22 16:54:50.000000 vanguard_api-0.1.2/vanguard/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:54:54.958423 vanguard_api-0.1.2/vanguard_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-22 16:54:54.000000 vanguard_api-0.1.2/vanguard_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-22 16:54:54.000000 vanguard_api-0.1.2/vanguard_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:54:54.000000 vanguard_api-0.1.2/vanguard_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 16:54:54.000000 vanguard_api-0.1.2/vanguard_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 16:54:54.000000 vanguard_api-0.1.2/vanguard_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:12:50.530397 vanguard_api-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-28 02:12:46.000000 vanguard_api-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-28 02:12:50.530397 vanguard_api-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-28 02:12:46.000000 vanguard_api-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 02:12:50.530397 vanguard_api-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-28 02:12:46.000000 vanguard_api-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:12:50.530397 vanguard_api-0.1.4/vanguard/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 02:12:46.000000 vanguard_api-0.1.4/vanguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-05-28 02:12:46.000000 vanguard_api-0.1.4/vanguard/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13772 2024-05-28 02:12:46.000000 vanguard_api-0.1.4/vanguard/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-28 02:12:46.000000 vanguard_api-0.1.4/vanguard/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 02:12:46.000000 vanguard_api-0.1.4/vanguard/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:12:50.530397 vanguard_api-0.1.4/vanguard_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-28 02:12:50.000000 vanguard_api-0.1.4/vanguard_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-28 02:12:50.000000 vanguard_api-0.1.4/vanguard_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 02:12:50.000000 vanguard_api-0.1.4/vanguard_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 02:12:50.000000 vanguard_api-0.1.4/vanguard_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 02:12:50.000000 vanguard_api-0.1.4/vanguard_api.egg-info/top_level.txt
```

### Comparing `vanguard_api-0.1.2/LICENSE` & `vanguard_api-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.1.2/PKG-INFO` & `vanguard_api-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.1.2
+Version: 0.1.4
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.4.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

### Comparing `vanguard_api-0.1.2/README.md` & `vanguard_api-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.1.2/setup.py` & `vanguard_api-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="vanguard-api",
-    version="0.1.2",
+    version="0.1.4",
     author="MaxxRK",
     author_email="maxxrk@pm.me",
     description="An unofficial API for Vanguard Invest",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/MaxxRK/vanguard-api",
-    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.2.tar.gz",
+    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.4.tar.gz",
     keywords=["VANGUARD", "API"],
     install_requires=["playwright", "playwright-stealth"],
     packages=["vanguard"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP :: Session",
```

### Comparing `vanguard_api-0.1.2/vanguard/account.py` & `vanguard_api-0.1.4/vanguard/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         Args:
             selector (ElementHandle): The selector from which to retrieve the account ID.
 
         Returns:
            string: account_id
         """
         account_id = selector.query_selector("span > span > span > span").inner_text()
-        if len(account_fields := account_id.split("—")) == 3:
+        if len(account_fields := account_id.split("—")) == 3 and ("brokerage" in account_fields[1].lower()):
             return account_fields[2].strip().replace("*", "")
         return None
 
     def _parse_rows(self, table_rows, account_id):
         """
         Parses the rows of a table to extract holdings information.
 
@@ -146,20 +146,26 @@
 
         This method navigates to the account holdings page, waits for the account numbers to load, and then retrieves the account numbers from the page.
 
         Returns:
             bool: True if the account numbers were successfully retrieved, False otherwise.
         """
         try:
-            self.session.go_url(holdings_page())
-            self.session.page.wait_for_selector(
-                '//span[contains(text(), "Expand all accounts")]', timeout=120000
-            ).click()
-            self.session.page.wait_for_selector("#overflow-override")
-            all_selectors = self.session.page.query_selector_all("#overflow-override")
+            
+            for _ in range(5):
+                try:
+                    self.session.go_url(holdings_page())
+                    self.session.page.wait_for_selector(
+                        '//span[contains(text(), "Expand all accounts")]', timeout=10000
+                    ).click()
+                    self.session.page.wait_for_selector("#overflow-override")
+                    all_selectors = self.session.page.query_selector_all("#overflow-override")
+                    break
+                except PlaywrightTimeoutError:
+                    continue
             for i, selector in enumerate(all_selectors):
                 account_id = self._get_account_id(selector)
                 if not account_id:
                     continue
                 self.account_numbers.append(account_id)
                 table_wrapper = selector.wait_for_selector(f"#self_managed_table_{i}")
                 table_entries = table_wrapper.query_selector_all("tbody")
```

### Comparing `vanguard_api-0.1.2/vanguard/order.py` & `vanguard_api-0.1.4/vanguard/order.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,15 +132,22 @@
         if quote_price != "$—":
             order_messages["ORDER INVALID"] = "Order page loaded correctly."
         else:
             order_messages["ORDER INVALID"] = "Quote did not load correctly."
 
         if order_messages["ORDER INVALID"] != "Order page loaded correctly.":
             return order_messages
-
+        try:
+            self.session.page.wait_for_selector(
+                "twe-trade-cannot-be-completed-modal tds-modal .modal__content",
+                timeout=3000
+            )
+            self.session.page.locator("xpath=//button[contains(text(), 'OK')]").click()
+        except PlaywrightTimeoutError:
+            pass
         if order_type == "BUY":
             buy_btn = self.session.page.wait_for_selector("xpath=//label[text()='Buy']")
             buy_btn.click()
         elif order_type == "SELL":
             sell_btn = self.session.page.wait_for_selector(
                 "xpath=//label[text()='Sell']"
             )
@@ -185,21 +192,25 @@
         try:
             if duration == "DAY":
                 self.session.page.click("xpath=//label[text()='Day']")
             elif duration == "GOOD_TILL_CANCELLED":
                 self.session.page.click("xpath=//label[text()='60-day (GTC)']")
             if order_type == "SELL":
                 self.session.page.wait_for_selector(
-                    "body > twe-root > main > twe-trade > form > div > div.row > div:nth-child(1) > twe-cost-basis-control > twe-cost-basis-modal > tds-modal > div.modal.visible > div > div.modal__content",
-                    timeout=10000,
-                )
+                    "twe-cost-basis-modal tds-checkbox .tds-checkbox__indicator.tds-checkbox--blue",
+                    timeout=3000
+                ).click()
                 self.session.page.wait_for_selector(
-                    "//button[text()=' Continue ']",
+                    "//button[contains(text(), ' Continue ')]",
                     timeout=10000,
                 ).click()
+                self.session.page.wait_for_selector(
+                    "body > twe-root > main > twe-trade > form > div > div.row > div:nth-child(1) > twe-cost-basis-control > twe-cost-basis-modal > tds-modal > div.modal.visible > div > div.modal__content",
+                    timeout=10000,
+                )
         except PlaywrightTimeoutError:
             pass
         try:
             self.session.page.wait_for_selector(
                 "body > twe-root > vg-vgn-nav > div > main > twe-trade > form > div > div.row > div.col-lg-6.col-xxl-4.tds-mb-9.d-none.d-xxl-block > twe-trade-detail > tds-card > div > tds-card-body > div.twe-flex-button-wrap > button:nth-child(2)",
                 timeout=5000,
             ).click()
@@ -213,15 +224,15 @@
                     timeout=5000,
                 ).click()
             except PlaywrightTimeoutError:
                 pass
 
         try:
             warning = self.session.page.wait_for_selector(
-                "body > twe-root > main > twe-trade > form > div > div.row > div.col-lg-6.col-xxl-4.tds-mb-9.d-none.d-xxl-block > twe-trade-detail > tds-card > div > tds-card-body > div:nth-child(3) > div > tds-card > div > tds-card-body",
+                "div.col-lg-6:nth-child(3) > twe-trade-detail:nth-child(2) > tds-card:nth-child(1) > div:nth-child(1) > tds-card-body:nth-child(1) > div:nth-child(3)",
                 timeout=5000,
             )
             warning_header_selector = warning.query_selector("p")
             warning_header = warning_header_selector.text_content()
             warning_items = warning.query_selector_all("li")
             warning_text = {warning_header: []}
             for item in warning_items:
```

### Comparing `vanguard_api-0.1.2/vanguard/session.py` & `vanguard_api-0.1.4/vanguard/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import traceback
 from time import sleep
 
 from playwright.sync_api import TimeoutError as PlaywrightTimeoutError
 from playwright.sync_api import sync_playwright
 from playwright_stealth import stealth_sync
 
-from .urls import landing_page
+from .urls import login_page, landing_page
 
 
 class VanguardSession:
     """
     A class to manage a session with Vanguard.
 
     This class provides methods to initialize a WebDriver with the necessary options, log into Vanguard, and perform other actions on the Chase website.
@@ -86,15 +86,16 @@
         else:
             self.browser = self.playwright.firefox.launch(headless=False)
         self.context = self.browser.new_context(
             viewport={"width": 1920, "height": 1080},
             storage_state=self.profile_path if self.title is not None else None,
         )
         self.page = self.context.new_page()
-        stealth_sync(self.page)
+        #testing without playwright-stealth for a bit
+        #stealth_sync(self.page)
         if self.debug:
             self.context.tracing.start(
                 name="vanguard_trace", screenshots=True, snapshots=True
             )
 
     def save_storage_state(self):
         """
@@ -122,14 +123,43 @@
     def go_url(self, url):
         """Navigates to the specified URL."""
         try:
             self.page.goto(url)
         except Exception as e:
             if "NS_BINDING_ABORTED" not in str(e):
                 raise e
+    
+    def find_login_state(self):
+        for _ in range(120):
+            try:
+                if "challenges.web.vanguard.com" in self.page.url:
+                    mode = 1
+                    return mode
+                if self.page.url == landing_page():
+                    self.page.wait_for_selector(
+                        "//h2[contains(text(), 'Accounts')]",
+                        timeout=1000,
+                    )
+                    mode = 1
+                    return mode
+                selector = self.page.wait_for_selector(
+                    "#username-password-submit-btn-1", timeout=500
+                )
+                if selector is not None:
+                    mode = 2
+                    return mode
+                selector = self.page.wait_for_selector("#CODE", timeout=500)
+                if selector is not None:
+                    mode = 3
+                    return mode 
+            except PlaywrightTimeoutError:
+                pass
+        mode = 0
+        return mode
+        
 
     def login(self, username, password, last_four):
         """
         Logs into the website with the provided username and password.
 
         This method navigates to the login page, enters the provided username and password into the appropriate fields,
         and submits the form. If the login is successful, the WebDriver will be redirected to the user's account page.
@@ -140,67 +170,61 @@
             last_four (int): The last four digits of the user's phone number.
 
         Raises:
             Exception: If there is an error during the login process in step one.
         """
         try:
             self.password = password
-            self.go_url(landing_page())
-            for _ in range(30):
+            self.go_url(login_page())
+            login_state = self.find_login_state()
+            if login_state == 0:
+                raise Exception("Failed to find login state")
+            elif login_state == 1:
+                return False
+            elif login_state == 2:
+                try:
+                    username_box = self.page.wait_for_selector("#USER", timeout=10000)
+                    username_box.type(username, delay=random.randint(50, 500))
+                    username_box.press("Tab")
+                    password_box = self.page.query_selector("#PASSWORD-blocked")
+                    password_box.type(password, delay=random.randint(50, 500))
+                    sleep(random.uniform(1, 3))
+                    self.page.query_selector("#username-password-submit-btn-1").click()
+                except PlaywrightTimeoutError:
+                    pass
+                try:
+                    self.page.wait_for_selector(
+                        "button.col-md:nth-child(2) > div:nth-child(1)", timeout=5000
+                    ).click()
+                except PlaywrightTimeoutError:
+                    pass
                 try:
-                    if self.page.url == landing_page():
-                        self.page.wait_for_selector(
-                            "//h2[contains(text(), 'Accounts')]",
-                            timeout=1000,
-                        )
-                        return False
                     self.page.wait_for_selector(
-                        "#username-password-submit-btn-1", timeout=1000
+                        "xpath=//div[contains(text(), '***-***-')]", timeout=5000
                     )
-                    break
+                    otp_cards = self.page.query_selector_all(
+                        "xpath=//div[contains(text(), '***-***-')]"
+                    )
+                    for otp_card in otp_cards:
+                        if otp_card.inner_text() == f"***-***-{last_four}":
+                            otp_card.click()
+                            break
                 except PlaywrightTimeoutError:
-                    continue
-            try:
-                username_box = self.page.wait_for_selector("#USER", timeout=10000)
-                username_box.type(username, delay=random.randint(50, 500))
-                username_box.press("Tab")
-                password_box = self.page.query_selector("#PASSWORD-blocked")
-                password_box.type(password, delay=random.randint(50, 500))
-                sleep(random.uniform(1, 3))
-                self.page.query_selector("#username-password-submit-btn-1").click()
-            except PlaywrightTimeoutError:
-                pass
-            try:
-                self.page.wait_for_selector(
-                    "button.col-md:nth-child(2) > div:nth-child(1)", timeout=5000
-                ).click()
-            except PlaywrightTimeoutError:
-                pass
-            try:
-                self.page.wait_for_selector(
-                    "xpath=//div[contains(text(), '***-***-')]", timeout=5000
-                )
-                otp_cards = self.page.query_selector_all(
-                    "xpath=//div[contains(text(), '***-***-')]"
-                )
-                for otp_card in otp_cards:
-                    if otp_card.inner_text() == f"***-***-{last_four}":
-                        otp_card.click()
-                        break
-            except PlaywrightTimeoutError:
-                pass
-            try:
-                self.page.wait_for_selector(
-                    "xpath=//div[contains(text(), 'Text')]", timeout=5000
-                ).click()
+                    pass
+                try:
+                    self.page.wait_for_selector(
+                        "xpath=//div[contains(text(), 'Text')]", timeout=5000
+                    ).click()
+                    return True
+                except PlaywrightTimeoutError:
+                    if self.title is not None:
+                        self.save_storage_state()
+                    return False
+            elif login_state == 3:
                 return True
-            except PlaywrightTimeoutError:
-                if self.title is not None:
-                    self.save_storage_state()
-                return False
         except Exception as e:
             self.close_browser()
             traceback.print_exc()
             raise Exception(f"Error in first step of login into Vanguard: {e}")
 
     def login_two(self, code):
         """
```

### Comparing `vanguard_api-0.1.2/vanguard_api.egg-info/PKG-INFO` & `vanguard_api-0.1.4/vanguard_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.1.2
+Version: 0.1.4
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.4.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

