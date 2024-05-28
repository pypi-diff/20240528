# Comparing `tmp/lavague_drivers_playwright-0.1.1.tar.gz` & `tmp/lavague_drivers_playwright-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_drivers_playwright-0.1.1.tar", max compression
+gzip compressed data, was "lavague_drivers_playwright-0.1.2.tar", max compression
```

## Comparing `lavague_drivers_playwright-0.1.1.tar` & `lavague_drivers_playwright-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       36 2024-05-15 19:17:05.222186 lavague_drivers_playwright-0.1.1/README.md
--rw-r--r--   0        0        0       61 2024-05-15 19:17:05.222186 lavague_drivers_playwright-0.1.1/lavague/drivers/playwright/__init__.py
--rw-r--r--   0        0        0     7063 2024-05-15 19:17:05.222186 lavague_drivers_playwright-0.1.1/lavague/drivers/playwright/base.py
--rw-r--r--   0        0        0      984 2024-05-15 21:18:20.756384 lavague_drivers_playwright-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 lavague_drivers_playwright-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       36 2024-05-28 08:59:04.857202 lavague_drivers_playwright-0.1.2/README.md
+-rw-r--r--   0        0        0       61 2024-05-28 08:59:04.857383 lavague_drivers_playwright-0.1.2/lavague/drivers/playwright/__init__.py
+-rw-r--r--   0        0        0     7215 2024-05-28 14:40:14.793562 lavague_drivers_playwright-0.1.2/lavague/drivers/playwright/base.py
+-rw-r--r--   0        0        0      984 2024-05-28 14:47:32.619177 lavague_drivers_playwright-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 lavague_drivers_playwright-0.1.2/PKG-INFO
```

### Comparing `lavague_drivers_playwright-0.1.1/lavague/drivers/playwright/base.py` & `lavague_drivers_playwright-0.1.2/lavague/drivers/playwright/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import Callable, Optional
 from playwright.sync_api import Page
 from lavague.core.base_driver import BaseDriver
 
 
 class PlaywrightDriver(BaseDriver):
     driver: Page
@@ -25,14 +26,20 @@
         browser = p.chromium.launch()
         page = browser.new_page()
         return page
 
     def get_driver(self) -> Page:
         return self.driver
 
+    def get_current_screenshot_folder(self) -> Path:
+        pass
+
+    def get_screenshot_as_png(self) -> bytes:
+        pass
+
     def resize_driver(self, width, height) -> None:
         self.driver.set_viewport_size({"width": width, "height": height})
 
     def get_url(self) -> Optional[str]:
         if self.driver.url == "about:blank":
             return None
         return self.driver.url
```

### Comparing `lavague_drivers_playwright-0.1.1/pyproject.toml` & `lavague_drivers_playwright-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-drivers-playwright"
-version = "0.1.1"
+version = "0.1.2"
 description = "Playwright integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_drivers_playwright-0.1.1/PKG-INFO` & `lavague_drivers_playwright-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-drivers-playwright
-Version: 0.1.1
+Version: 0.1.2
 Summary: Playwright integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

