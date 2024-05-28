# Comparing `tmp/flet_page_manager-0.1.9-py312-none-any.whl.zip` & `tmp/flet_page_manager-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 3703 bytes, number of entries: 10
+Zip file size: 4317 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        2 b- defN 16-Jan-01 00:00 .gitignore
--rw-r--r--  2.0 unx      426 b- defN 16-Jan-01 00:00 flet_page_manager-0.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 16-Jan-01 00:00 flet_page_manager-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx      220 b- defN 16-Jan-01 00:00 page_manager/__init__.py
--rw-r--r--  2.0 unx       84 b- defN 16-Jan-01 00:00 page_manager/exception.py
--rw-r--r--  2.0 unx     2804 b- defN 16-Jan-01 00:00 page_manager/manager.py
+-rw-r--r--  2.0 unx      534 b- defN 16-Jan-01 00:00 flet_page_manager-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 flet_page_manager-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      138 b- defN 16-Jan-01 00:00 page_manager/__init__.py
+-rw-r--r--  2.0 unx      121 b- defN 16-Jan-01 00:00 page_manager/exception.py
+-rw-r--r--  2.0 unx     3837 b- defN 16-Jan-01 00:00 page_manager/manager.py
 -rw-r--r--  2.0 unx       51 b- defN 16-Jan-01 00:00 page_manager/pages/__init__.py
--rw-r--r--  2.0 unx      603 b- defN 16-Jan-01 00:00 page_manager/pages/base.py
--rw-r--r--  2.0 unx      234 b- defN 16-Jan-01 00:00 page_manager/state.py
-?rw-------  2.0 unx      783 b- defN 16-Jan-01 00:00 flet_page_manager-0.1.9.dist-info/RECORD
-10 files, 5299 bytes uncompressed, 2361 bytes compressed:  55.4%
+-rw-r--r--  2.0 unx      728 b- defN 16-Jan-01 00:00 page_manager/pages/base.py
+-rw-r--r--  2.0 unx      215 b- defN 16-Jan-01 00:00 page_manager/state.py
+-rw-r--r--  2.0 unx      211 b- defN 16-Jan-01 00:00 page_manager/utils.py
+?rw-------  2.0 unx      861 b- defN 16-Jan-01 00:00 flet_page_manager-0.2.0.dist-info/RECORD
+11 files, 6788 bytes uncompressed, 2857 bytes compressed:  57.9%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
 Filename: .gitignore
 Comment: 
 
-Filename: flet_page_manager-0.1.9.dist-info/METADATA
+Filename: flet_page_manager-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: flet_page_manager-0.1.9.dist-info/WHEEL
+Filename: flet_page_manager-0.2.0.dist-info/WHEEL
 Comment: 
 
 Filename: page_manager/__init__.py
 Comment: 
 
 Filename: page_manager/exception.py
 Comment: 
@@ -21,11 +21,14 @@
 
 Filename: page_manager/pages/base.py
 Comment: 
 
 Filename: page_manager/state.py
 Comment: 
 
-Filename: flet_page_manager-0.1.9.dist-info/RECORD
+Filename: page_manager/utils.py
+Comment: 
+
+Filename: flet_page_manager-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## page_manager/__init__.py

```diff
@@ -1,6 +1,4 @@
+from .exception import PageCrash, PageException
 from .manager import PageManager
 from .pages import PageBase
-from .exception import PageException, PageCrash
 from .state import StateBase
-
-__all__ = ["PageManager", "PageBase", "PageException", "PageCrash", "StateBase"]
```

## page_manager/exception.py

```diff
@@ -1,6 +1,9 @@
+from __future__ import annotations
+
+
 class PageException(Exception):
     pass
 
 
 class PageCrash(PageException):
     pass
```

## page_manager/manager.py

```diff
@@ -1,22 +1,27 @@
 from __future__ import annotations
+
+import asyncio
+import sys
+from functools import partial
+
 import flet as ft
 from flet import AppView
-import asyncio
-from typing import TYPE_CHECKING, TypeVar
 from loguru import logger
-import sys
-from .exception import PageException
-from .state import StateBase
+
 from .pages import PageBase
+from .state import StateBase
+from .utils import get_free_port
+from typing import Generic, TypeVar
 
+__PageManager_StateT = TypeVar("__PageManager_StateT", bound = StateBase)
 
-class PageManager[StateT: StateBase]:
-    logger = logger
 
+class PageManager(Generic[__PageManager_StateT]):
+    logger = logger
     page_mapping: dict[str, type[PageBase]] = {}
 
     @staticmethod
     def register_page(name: str | None = None):
         def _register_page(page_cls: type[PageBase]):
             PageManager.page_mapping[name or page_cls.__name__] = page_cls
             return page_cls
@@ -26,27 +31,40 @@
     @staticmethod
     def set_level(level: str | int):
         logger.remove(0)
         logger.add(sys.stdout, level=level)
 
     def __init__(
         self,
-        state: StateT,
+        state: __PageManager_StateT,
         *,
         view: AppView = AppView.FLET_APP,
         assets_dir: str = "public",
     ) -> None:
         self.state = state
         self.page_count: int = 0
         self.page_tasks: list[asyncio.Task] = []
         self.background_tasks: list[asyncio.Task] = []
 
-        self.view: AppView = view
+        self.view = view
         self.assets_dir = assets_dir
 
+    async def cancel_tasks(self, tasks: list[asyncio.Task]):
+        for task in tasks:
+            if not task.done():
+                try:
+                    task.cancel()
+                    try:
+                        await task
+                    except asyncio.CancelledError:
+                        pass
+                    self.logger.info("PageManager: Task canceled")
+                except Exception as e:
+                    self.logger.error("PageManager: Error canceling task - {:}".format(e))
+
     async def run(self, name: str, *, port: int = 0):
         self.open_page(name, port=port)
         while self.page_count > 0:
             try:
                 await asyncio.sleep(0.1)
                 for task in self.page_tasks:
                     if task.done():
@@ -56,38 +74,50 @@
 
                 for task in self.background_tasks:
                     if task.done():
                         self.background_tasks.remove(task)
                         await task
 
             except KeyboardInterrupt:
-                for task in self.page_tasks:
-                    task.cancel()
-                    self.logger.info("PageManager: Page task canceled")
                 break
 
-        for task in self.background_tasks:
-            task.cancel()
-            self.logger.info("PageManager: Background task canceled")
-
-    async def close(self):
-        for p in self.state.running_pages:
-            await p.window_destroy_async()
+        await self.cancel_tasks(self.page_tasks)
+        await self.cancel_tasks(self.background_tasks)
+        self.logger.info("PageManager: All tasks have been canceled, exiting...")
 
     def open_page(self, name: str, *, port: int = 0):
         if name not in PageManager.page_mapping:
-            raise PageException(f"Page {name} not found")
+            logger.error("Page `{:}` not found".format(name))
+            return
+        if port == 0:
+            port = get_free_port()
+        logger.info("PageManager: Opening page `{:}` on port {:}".format(name, port))
         page_obj = PageManager.page_mapping[name]()
         self.page_count += 1
 
-        async def _page_func_async(page: ft.Page):
-            await page_obj(page, self)
-
         task = asyncio.create_task(
             ft.app_async(
-                target=_page_func_async,
+                target=partial(page_obj, pm=self),
                 view=self.view,
                 port=port,
                 assets_dir=self.assets_dir,
             )
         )
         self.page_tasks.append(task)
+
+    async def restart(self, name: str, *, port: int = 0):
+        # TODO
+        await self.cancel_tasks(self.page_tasks)
+        await self.cancel_tasks(self.background_tasks)
+        self.page_count = 0
+        self.page_tasks = []
+        self.background_tasks = []
+        await self.run(name, port=port)
+
+    async def start(self, name: str, *, port: int = 0):
+        # TODO
+        await self.run(name, port=port)
+
+    async def close(self):
+        # TODO
+        for p in self.state.running_pages:
+            p.window_destroy()
```

## page_manager/pages/base.py

```diff
@@ -1,20 +1,24 @@
 from __future__ import annotations
+
+from typing import Generic, TypeVar, TYPE_CHECKING
+
 import flet as ft
-from typing import TYPE_CHECKING
+
 from ..state import StateBase
 
 if TYPE_CHECKING:
     from ..manager import PageManager
+__PageBase_StateT = TypeVar("__PageBase_StateT", bound = StateBase)
 
 
-class PageBase[StateT: StateBase]:
-    async def init(self, page: ft.Page, pm: PageManager[StateT]):
+class PageBase(Generic[__PageBase_StateT]):
+    def init(self, page: ft.Page, pm: PageManager[__PageBase_StateT]):
         pm.state.running_pages.append(page)
-        await page.window_center_async()
+        page.window_center()
 
-    async def build(self, page: ft.Page, pm: PageManager[StateT]):
-        raise NotImplementedError
+    def build(self, page: ft.Page, pm: PageManager[__PageBase_StateT]):
+        raise NotImplementedError("Page must implement build method")
 
-    async def __call__(self, page: ft.Page, pm: PageManager[StateT]):
-        await self.init(page, pm)
-        await self.build(page, pm)
+    def __call__(self, page: ft.Page, pm: PageManager[__PageBase_StateT]):
+        self.init(page, pm)
+        self.build(page, pm)
```

## page_manager/state.py

```diff
@@ -1,11 +1,8 @@
-from pydantic import dataclasses
-import flet as ft
-
+from __future__ import annotations
 
-class Config:
-    arbitrary_types_allowed = True
+import flet as ft
+from pydantic import BaseModel, Field
 
 
-@dataclasses.dataclass(config=Config)
-class StateBase:
-    running_pages: list[ft.Page] = dataclasses.Field(default_factory=list)
+class StateBase(BaseModel, arbitrary_types_allowed=True):
+    running_pages: list[ft.Page] = Field(default_factory=list)
```

## Comparing `flet_page_manager-0.1.9.dist-info/RECORD` & `flet_page_manager-0.2.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore,sha256=zbyuFRBda3geYggTx5x-hodA1OnMU85vX8u8Ejh630s,2
-flet_page_manager-0.1.9.dist-info/METADATA,sha256=dQMW02_bA-zzf-4DQbKXgLly-6UTwET_ApABOHPCtdU,426
-flet_page_manager-0.1.9.dist-info/WHEEL,sha256=RAm9eBVxRjmgO3tnpFsael8h4-AWXbeb2dUwFLZOlSo,92
-page_manager/__init__.py,sha256=eMRgZHNIgHqVzgPRpmtEcmTwO1uBYkH0aKxAZypEBTo,220
-page_manager/exception.py,sha256=gcpmT_pGcgXbEkW5hIzaLyBJMqieBqLXstEUooGcVlg,84
-page_manager/manager.py,sha256=GkY0Dna901vKTq2hsLQS4JvJKxO_b1N8UjdXvoAreu0,2804
+flet_page_manager-0.2.0.dist-info/METADATA,sha256=oyV7GMm1_9YN5eCA5sslupfD06EQf1eWB3VxzbR3Fpg,534
+flet_page_manager-0.2.0.dist-info/WHEEL,sha256=vnE8JVcI2Wz7GRKorsPArnBdnW2SWKWGow5gu5tHlRU,90
+page_manager/__init__.py,sha256=lqt5D9DQrhxPO2vX2ARNC6FU_Z9ABJd8_wibRLwJvXQ,138
+page_manager/exception.py,sha256=fKn5YosQLNXgCjMWq5HeNFCf3qiqXlDb7oD4OdDlip4,121
+page_manager/manager.py,sha256=woRRVDQhT_E9EqY4VWIMTWE__0JcmlW0yQEYIYMUqn8,3837
 page_manager/pages/__init__.py,sha256=otvgMgIQu5PAV7N5UAV4NUdde0qGqTIM5shRiOTimhY,51
-page_manager/pages/base.py,sha256=cqhe8q3YITk0hsS5oKBdMmJjivlDu_r5g3--se4eZbs,603
-page_manager/state.py,sha256=7YbxsadthpIwIsGFf2kPpFVrV2AJUbqmrlbnTKskegY,234
-flet_page_manager-0.1.9.dist-info/RECORD,,
+page_manager/pages/base.py,sha256=fPB280CoBc1GggvnYwytsZjmRDVsX2UuRKhFPnifKZc,728
+page_manager/state.py,sha256=TzNfIwKLe7PY09F4YEvjkpoepewhsR6yyG2F3nSlXKU,215
+page_manager/utils.py,sha256=Oej3zKL1sYFWCwaAueFwtXeuBUrh22j1qAtgcDGcRB4,211
+flet_page_manager-0.2.0.dist-info/RECORD,,
```

