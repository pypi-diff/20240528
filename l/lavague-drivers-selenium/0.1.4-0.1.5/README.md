# Comparing `tmp/lavague_drivers_selenium-0.1.4.tar.gz` & `tmp/lavague_drivers_selenium-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_drivers_selenium-0.1.4.tar", max compression
+gzip compressed data, was "lavague_drivers_selenium-0.1.5.tar", max compression
```

## Comparing `lavague_drivers_selenium-0.1.4.tar` & `lavague_drivers_selenium-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       34 2024-05-22 18:18:44.475195 lavague_drivers_selenium-0.1.4/README.md
--rw-r--r--   0        0        0       57 2024-05-22 18:18:44.475375 lavague_drivers_selenium-0.1.4/lavague/drivers/selenium/__init__.py
--rw-r--r--   0        0        0    25991 2024-05-25 13:34:21.297084 lavague_drivers_selenium-0.1.4/lavague/drivers/selenium/base.py
--rw-r--r--   0        0        0      976 2024-05-25 13:39:34.180343 lavague_drivers_selenium-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-05-28 08:59:04.857656 lavague_drivers_selenium-0.1.5/README.md
+-rw-r--r--   0        0        0       57 2024-05-28 08:59:04.858191 lavague_drivers_selenium-0.1.5/lavague/drivers/selenium/__init__.py
+-rw-r--r--   0        0        0    28288 2024-05-28 12:38:02.777250 lavague_drivers_selenium-0.1.5/lavague/drivers/selenium/base.py
+-rw-r--r--   0        0        0      976 2024-05-28 14:48:36.161430 lavague_drivers_selenium-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.1.5/PKG-INFO
```

### Comparing `lavague_drivers_selenium-0.1.4/lavague/drivers/selenium/base.py` & `lavague_drivers_selenium-0.1.5/lavague/drivers/selenium/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+from datetime import datetime
+import hashlib
+import os
+from pathlib import Path
+import time
 from typing import Any, Optional, Callable
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.common.by import By
 from lavague.core.base_driver import BaseDriver
 from PIL import Image
 from io import BytesIO
 
+
 class SeleniumDriver(BaseDriver):
     driver: WebDriver
 
     def __init__(
         self,
         url: Optional[str] = None,
         get_selenium_driver: Optional[Callable[[], WebDriver]] = None,
@@ -58,33 +64,87 @@
         return f'driver.get("{url}")'
 
     def goto(self, url: str) -> None:
         self.driver.get(url)
 
     def get_html(self) -> str:
         return self.driver.page_source
-    
+
+    def compute_hash(self, screenshot: bytes) -> str:
+        """Computes hash of a file."""
+        hasher = hashlib.md5()
+        hasher.update(screenshot)
+        return hasher.hexdigest()
+
+    def save_screenshot(self, current_screenshot_folder: Path) -> str:
+        """Save the screenshot data to a file and return the path. If the screenshot already exists, return the path. If not save it to the folder."""
+
+        new_screenshot = self.get_screenshot_as_png()
+        new_hash = self.compute_hash(new_screenshot)
+        new_screenshot_name = f"{new_hash}.png"
+        new_screenshot_full_path = current_screenshot_folder / new_screenshot_name
+
+        # If the screenshot does not exist, save it
+        if not new_screenshot_full_path.exists():
+            with open(new_screenshot_full_path, "wb") as f:
+                f.write(new_screenshot)
+        return str(new_screenshot_full_path)
+
     def get_obs(self) -> dict:
-        driver = self.driver
-        
-        html = driver.page_source
-        
-        screenshot = driver.get_screenshot_as_png()
-        screenshot = BytesIO(screenshot)
-        screenshot = Image.open(screenshot)
+        current_screenshot_folder = self.get_current_screenshot_folder()
+        # We take a screenshot and computes its hash to see if it already exists
+        self.save_screenshot(current_screenshot_folder)
 
+        url = self.get_url()
+        html = self.get_html()
         obs = {
             "html": html,
-            "screenshot": screenshot
+            "screenshots_path": str(current_screenshot_folder),
+            "url": url,
+            "date": datetime.now().isoformat(),
         }
-        
+
         return obs
 
-    def save_screenshot(self, filename: str) -> None:
-        self.driver.save_screenshot(filename)
+    def is_bottom_of_page(self) -> bool:
+        return self.driver.execute_script(
+            "return (window.innerHeight + window.scrollY) >= document.body.scrollHeight;"
+        )
+
+    def get_current_screenshot_folder(self) -> Path:
+        url = self.get_url()
+        screenshots_path = Path("./screenshots")
+        screenshots_path.mkdir(exist_ok=True)
+
+        current_screenshot_folder = screenshots_path / url.replace("://", "_").replace(
+            "/", "_"
+        )
+        current_screenshot_folder.mkdir(exist_ok=True)
+        return current_screenshot_folder
+
+    def get_screenshots_whole_page(self) -> list[str]:
+        screenshot_paths = []
+
+        current_screenshot_folder = self.get_current_screenshot_folder()
+
+        while True:
+            # Saves a screenshot
+            screenshot_path = self.save_screenshot(current_screenshot_folder)
+            screenshot_paths.append(screenshot_path)
+            self.driver.execute_script(
+                "window.scrollBy(0, (window.innerHeight / 1.5));"
+            )
+            time.sleep(0.5)
+
+            if self.is_bottom_of_page():
+                break
+        return screenshot_paths
+
+    def get_screenshot_as_png(self) -> bytes:
+        return self.driver.get_screenshot_as_png()
 
     def get_dummy_code(self) -> str:
         return 'driver.execute_script("window.scrollBy(0, 500)")'
 
     def destroy(self) -> None:
         self.driver.quit()
 
@@ -108,16 +168,17 @@
         viewport_height = self.driver.execute_script("return window.innerHeight;")
 
         height_difference = targeted_height - viewport_height
         self.driver.set_window_size(width, targeted_height + height_difference)
 
     def get_capability(self) -> str:
         return SELENIUM_PROMPT_TEMPLATE
-    
-SELENIUM_PROMPT_TEMPLATE = '''
+
+
+SELENIUM_PROMPT_TEMPLATE = """
 You are a Selenium expert in writing code to interact with web pages. You have been given a series of HTML snippets and queries.
 Your goal is to write Selenium code to answer queries. Your answer must be a Python markdown only.
 Always target elements by XPATH.
 
 Provide high level explanations about why you think this element is the right one.
 Your answer must be short and concise. 
 
@@ -238,8 +299,8 @@
 # Next, we locate the time selector. It is also inside a div element with specific class and data-test attributes.
 # The time selector is found at the following XPath:
 time_selector = driver.find_element(By.XPATH, "/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[2]/div")
 
 # Click on the time selector to open the time selection dropdown
 time_selector.click()
 ```python
-'''
+"""
```

### Comparing `lavague_drivers_selenium-0.1.4/pyproject.toml` & `lavague_drivers_selenium-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-drivers-selenium"
-version = "0.1.4"
+version = "0.1.5"
 description = "Selenium integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_drivers_selenium-0.1.4/PKG-INFO` & `lavague_drivers_selenium-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-drivers-selenium
-Version: 0.1.4
+Version: 0.1.5
 Summary: Selenium integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,selenium
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

