# Comparing `tmp/nonebot_plugin_waiter-0.6.0.tar.gz` & `tmp/nonebot_plugin_waiter-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_waiter-0.6.0.tar", last modified: Fri May 24 15:56:00 2024, max compression
+gzip compressed data, was "nonebot_plugin_waiter-0.6.1.tar", last modified: Tue May 28 15:55:49 2024, max compression
```

## Comparing `nonebot_plugin_waiter-0.6.0.tar` & `nonebot_plugin_waiter-0.6.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     5579 2024-05-24 15:53:38.054026 nonebot_plugin_waiter-0.6.0/README.md
--rw-r--r--   0        0        0     1387 2024-05-24 15:56:00.844773 nonebot_plugin_waiter-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    15740 2024-05-24 15:53:01.881729 nonebot_plugin_waiter-0.6.0/src/nonebot_plugin_waiter/__init__.py
--rw-r--r--   0        0        0      741 2024-05-24 15:25:29.887357 nonebot_plugin_waiter-0.6.0/src/nonebot_plugin_waiter/config.py
--rw-r--r--   0        0        0     5645 1970-01-01 00:00:00.000000 nonebot_plugin_waiter-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     5579 2024-05-24 15:53:38.054026 nonebot_plugin_waiter-0.6.1/README.md
+-rw-r--r--   0        0        0     1387 2024-05-28 15:55:49.132867 nonebot_plugin_waiter-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    16128 2024-05-28 15:53:59.968871 nonebot_plugin_waiter-0.6.1/src/nonebot_plugin_waiter/__init__.py
+-rw-r--r--   0        0        0      741 2024-05-24 15:25:29.887357 nonebot_plugin_waiter-0.6.1/src/nonebot_plugin_waiter/config.py
+-rw-r--r--   0        0        0     5645 1970-01-01 00:00:00.000000 nonebot_plugin_waiter-0.6.1/PKG-INFO
```

### Comparing `nonebot_plugin_waiter-0.6.0/README.md` & `nonebot_plugin_waiter-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_waiter-0.6.0/pyproject.toml` & `nonebot_plugin_waiter-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-waiter"
-version = "0.6.0"
+version = "0.6.1"
 description = "An alternative for got-and-reject in Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "3165388245@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.3.0",
 ]
```

### Comparing `nonebot_plugin_waiter-0.6.0/src/nonebot_plugin_waiter/__init__.py` & `nonebot_plugin_waiter-0.6.1/src/nonebot_plugin_waiter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from nonebot.internal.permission import User, Permission
 from nonebot.utils import run_sync, is_coroutine_callable
 from nonebot.internal.matcher import current_event, current_matcher
 from nonebot.internal.adapter import Bot, Event, Message, MessageSegment, MessageTemplate
 
 from .config import Config
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 __plugin_meta__ = PluginMetadata(
     name="Waiter 插件",
     description="提供一个 got-and-reject 会话控制的替代方案，可自由控制超时时间",
     usage="@waiter(waits: list[type[Event] | str], matcher: type[Matcher] | Matcher, parameterless: Iterable[Any] | None, keep_session: bool = False)",  # noqa: E501
     homepage="https://github.com/RF-Tar-Railt/nonebot-plugin-waiter",
     type="library",
@@ -300,14 +300,15 @@
     handler: _DependentCallable[R] | None = None,
     timeout: float = plugin_config.waiter_timeout,
 ):
     """等待用户输入并返回结果
 
     参数:
         message: 提示消息
+        handler: 处理函数
         timeout: 等待超时时间
     返回值:
         符合条件的用户输入
     """
 
     async def wrapper(event: Event):
         return event.get_message()
@@ -331,14 +332,15 @@
 
 @overload
 async def prompt_until(
     message: str | Message | MessageSegment | MessageTemplate,
     checker: Callable[[Message], bool],
     *,
     matcher: type[Matcher] | Matcher | None = None,
+    finish: bool = False,
     timeout: float = plugin_config.waiter_timeout,
     retry: int = 5,
     retry_prompt: str | Message | MessageSegment | MessageTemplate = plugin_config.waiter_retry_prompt,
     timeout_prompt: str | Message | MessageSegment | MessageTemplate = plugin_config.waiter_timeout_prompt,
     limited_prompt: str | Message | MessageSegment | MessageTemplate = plugin_config.waiter_limited_prompt,
 ) -> Message | None: ...
 
@@ -346,45 +348,49 @@
 @overload
 async def prompt_until(
     message: str | Message | MessageSegment | MessageTemplate,
     checker: Callable[[R], bool],
     handler: _DependentCallable[R],
     *,
     matcher: type[Matcher] | Matcher | None = None,
+    finish: bool = False,
     timeout: float = plugin_config.waiter_timeout,
     retry: int = 5,
     retry_prompt: str | Message | MessageSegment | MessageTemplate = plugin_config.waiter_retry_prompt,
     timeout_prompt: str | Message | MessageSegment | MessageTemplate = plugin_config.waiter_timeout_prompt,
     limited_prompt: str | Message | MessageSegment | MessageTemplate = plugin_config.waiter_limited_prompt,
 ) -> R | None: ...
 
 
 async def prompt_until(
     message: str | Message | MessageSegment | MessageTemplate,
     checker: Callable[..., bool],
     handler: _DependentCallable[R] | None = None,
     *,
     matcher: type[Matcher] | Matcher | None = None,
+    finish: bool = False,
     timeout: float = plugin_config.waiter_timeout,
     retry: int = 5,
     retry_prompt: str | Message | MessageSegment | MessageTemplate = plugin_config.waiter_retry_prompt,
     timeout_prompt: str | Message | MessageSegment | MessageTemplate = plugin_config.waiter_timeout_prompt,
     limited_prompt: str | Message | MessageSegment | MessageTemplate = plugin_config.waiter_limited_prompt,
 ):
     """等待用户输入并返回结果
 
     参数:
-        before: 提示消息
+        message: 提示消息
+        checker: 检查函数
+        handler: 处理函数
         matcher: 匹配器
+        finish: 超时或重试过多时是否结束会话
         timeout: 等待超时时间
         retry: 重试次数
         retry_prompt: 重试时的提示信息
         timeout_prompt: 等待超时时的提示信息
         limited_prompt: 重试次数用尽时的提示信息
-        rule: 验证输入的规则
     返回值:
         符合条件的用户输入
     """
     if not matcher:
         try:
             matcher = current_matcher.get()
         except LookupError:
@@ -400,21 +406,27 @@
     if handler is None:
         wait = waiter(waits=["message"], keep_session=True, matcher=matcher)(wrapper)
     else:
         wait = waiter(waits=["message"], keep_session=True, matcher=matcher)(handler)
 
     async for data in wait(timeout=timeout, retry=retry, prompt=retry_prompt):
         if data is None:
-            await matcher.send(timeout_prompt)
+            if finish:
+                await matcher.finish(timeout_prompt)
+            else:
+                await matcher.send(timeout_prompt)
             return
         if not checker(data):
             continue
         return data  # type: ignore
     else:
-        await matcher.send(limited_prompt)
+        if finish:
+            await matcher.finish(limited_prompt)
+        else:
+            await matcher.send(limited_prompt)
 
 
 async def suggest(
     message: str | Message | MessageSegment | MessageTemplate,
     expect: list[str],
     timeout: float = plugin_config.waiter_timeout,
     retry: int = 5,
```

### Comparing `nonebot_plugin_waiter-0.6.0/src/nonebot_plugin_waiter/config.py` & `nonebot_plugin_waiter-0.6.1/src/nonebot_plugin_waiter/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_waiter-0.6.0/PKG-INFO` & `nonebot_plugin_waiter-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-waiter
-Version: 0.6.0
+Version: 0.6.1
 Summary: An alternative for got-and-reject in Nonebot
 Author-Email: RF-Tar-Railt <3165388245@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: nonebot2>=2.3.0
 Description-Content-Type: text/markdown
```

