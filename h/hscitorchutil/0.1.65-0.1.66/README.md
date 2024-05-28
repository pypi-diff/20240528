# Comparing `tmp/hscitorchutil-0.1.65.tar.gz` & `tmp/hscitorchutil-0.1.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscitorchutil-0.1.65.tar", max compression
+gzip compressed data, was "hscitorchutil-0.1.66.tar", max compression
```

## Comparing `hscitorchutil-0.1.65.tar` & `hscitorchutil-0.1.66.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-10-26 13:56:57.077205 hscitorchutil-0.1.65/README.md
--rw-r--r--   0        0        0     2961 2024-01-19 12:53:41.148969 hscitorchutil-0.1.65/hscitorchutil/callbacks.py
--rw-r--r--   0        0        0     9043 2024-05-27 04:59:35.199538 hscitorchutil-0.1.65/hscitorchutil/dataset.py
--rw-r--r--   0        0        0    12723 2023-12-19 12:19:49.447156 hscitorchutil-0.1.65/hscitorchutil/fsspec.py
--rw-r--r--   0        0        0      847 2023-12-11 20:57:21.481430 hscitorchutil-0.1.65/hscitorchutil/processlocal.py
--rw-r--r--   0        0        0     8676 2024-04-18 13:19:14.770983 hscitorchutil-0.1.65/hscitorchutil/sqlite.py
--rw-r--r--   0        0        0      908 2024-05-27 05:05:57.824030 hscitorchutil-0.1.65/pyproject.toml
--rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 hscitorchutil-0.1.65/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-10-26 13:56:57.077205 hscitorchutil-0.1.66/README.md
+-rw-r--r--   0        0        0     2961 2024-01-19 12:53:41.148969 hscitorchutil-0.1.66/hscitorchutil/callbacks.py
+-rw-r--r--   0        0        0     9043 2024-05-27 04:59:35.199538 hscitorchutil-0.1.66/hscitorchutil/dataset.py
+-rw-r--r--   0        0        0    13146 2024-05-28 21:10:07.909175 hscitorchutil-0.1.66/hscitorchutil/fsspec.py
+-rw-r--r--   0        0        0      847 2023-12-11 20:57:21.481430 hscitorchutil-0.1.66/hscitorchutil/processlocal.py
+-rw-r--r--   0        0        0     8676 2024-04-18 13:19:14.770983 hscitorchutil-0.1.66/hscitorchutil/sqlite.py
+-rw-r--r--   0        0        0      908 2024-05-28 21:10:15.798578 hscitorchutil-0.1.66/pyproject.toml
+-rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 hscitorchutil-0.1.66/PKG-INFO
```

### Comparing `hscitorchutil-0.1.65/hscitorchutil/callbacks.py` & `hscitorchutil-0.1.66/hscitorchutil/callbacks.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.65/hscitorchutil/dataset.py` & `hscitorchutil-0.1.66/hscitorchutil/dataset.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.65/hscitorchutil/fsspec.py` & `hscitorchutil-0.1.66/hscitorchutil/fsspec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,40 @@
+from fsspec.asyn import AsyncFileSystem
+from hscitorchutil.processlocal import ProcessLocal
+import yaml
+import multiprocessing_utils
 import asyncio
 from concurrent import futures
 import datetime
 import functools
 import mmap
 import os
 import time
 from typing import Any, Awaitable, Callable, Iterable, Tuple, Coroutine
 import fsspec
 import fsspec.implementations.local
 import fsspec.asyn
-from fsspec.asyn import AsyncFileSystem
 from fsspec.callbacks import TqdmCallback
 from fsspec.implementations.cached import SimpleCacheFileSystem
 from fsspec.implementations.cache_mapper import AbstractCacheMapper
 from fsspec.caching import Fetcher, MMapCache, register_cache, caches
-from morefs.asyn_local import AsyncLocalFileSystem
-import multiprocessing_utils
-import yaml
+import fsspec.implementations.local
+
+# The below patches LocalFileSystem to have the removed mv_file method that current AsyncLocalFileSystem version needs
+
+
+class PatchedLocalFileSystem(fsspec.implementations.local.LocalFileSystem):
+    def mv_file(self, src: str, dst: str, **kwargs) -> None:
+        self.mv(src, dst, **kwargs)
+
+
+fsspec.implementations.local.LocalFileSystem = PatchedLocalFileSystem
+
+from morefs.asyn_local import AsyncLocalFileSystem  # noqa
 
-from hscitorchutil.processlocal import ProcessLocal
 
 # without this, fsspec hangs in a multiprocessing fork context when it has been already used in the parent process
 os.register_at_fork(
     after_in_child=fsspec.asyn.reset_lock,
 )
 
 # Async Maps (start, end) to bytes
@@ -132,15 +144,15 @@
             self._wait(waiting, need)
         return self.cache[start:end]
 
     async def _afetch(self, start: int | None, end: int | None) -> bytes:
         need = self._get_need(start, end)
         while need:
             to_fetch, waiting = self._get_to_fetch(need)
-            datas = await asyncio.gather(*[self.afetcher(sstart, send) for sstart, send, _ in to_fetch]) # type: ignore # noqa
+            datas = await asyncio.gather(*[self.afetcher(sstart, send) for sstart, send, _ in to_fetch])  # type: ignore # noqa
             for (sstart, send, cis), data in zip(to_fetch, datas):
                 self.cache[sstart:send] = data
                 for i in cis:
                     self._index[i] = 2
             await self._await(waiting, need)
         return self.cache[start:end]
 
@@ -172,19 +184,21 @@
         urlpath, storage_options=storage_options)
     if isinstance(fs, fsspec.implementations.local.LocalFileSystem):
         fs = AsyncLocalFileSystem()
     if not fs.async_impl:
         raise ValueError("Unsupported non-async filesystem: %s" % fs)
     return fs
 
+
 def get_cache(fs: AsyncFileSystem, urlpath: str, size: int, cache_dir: str, blocksize: int, parallel_timeout: int, cache_mapper: AbstractCacheMapper) -> SharedMMapCache:
     if not os.path.exists(cache_dir):
         os.makedirs(cache_dir, exist_ok=True)
+
     def _cat_file_fetcher(fs: AsyncFileSystem, urlpath: str, start: int, end: int) -> bytes:
-        return fs.cat_file(urlpath, start=start, end=end) # type: ignore
+        return fs.cat_file(urlpath, start=start, end=end)  # type: ignore
 
     async def _cat_file_afetcher(_, urlpath: str, start: int, end: int) -> bytes:
         return await fs._cat_file(urlpath, start=start, end=end)
 
     return SharedMMapCache(
         blocksize,
         functools.partial(_cat_file_fetcher, fs, urlpath),
@@ -196,27 +210,28 @@
 
 
 def prefetch_if_remote(urlpath: str, size: int, cache_dir: str, storage_options: dict[str, Any] | None = None, blocksize: int = 65536, parallel_timeout: int = 30, cache_mapper: AbstractCacheMapper = PathCacheMapper()) -> futures.Future[None]:
     fs = get_async_filesystem(urlpath, storage_options=storage_options)
     if getattr(fs, "local_file", False):
         ret = asyncio.Future()
         ret.set_result(None)
-        return ret # type: ignore
+        return ret  # type: ignore
     cache = get_cache(fs, urlpath, size, cache_dir,
                       blocksize, parallel_timeout, cache_mapper)
 
     async def _a_fill_cache():
         f = await fs.open_async(urlpath, "rb")
         while f.loc < size:
             loc = f.loc
             data = await f.read(block_size*2**4*5)  # type: ignore
             cache.fill(loc, data)
         cache._index[-1] = 2
-        await f.close() # type: ignore
-    return asyncio.run_coroutine_threadsafe(_a_fill_cache(), fs.loop) # type: ignore
+        await f.close()  # type: ignore
+    # type: ignore
+    return asyncio.run_coroutine_threadsafe(_a_fill_cache(), fs.loop)
 
 
 def _get_afetcher(urlpath: str, size: int, storage_options: dict[str, Any] | None = None, parallel_timeout=30, cache_dir: str | None = None, blocksize: int = 65536, cache_mapper: AbstractCacheMapper = PathCacheMapper()):
     fs = get_async_filesystem(urlpath, storage_options=storage_options)
     if cache_dir is None or getattr(fs, "local_file", False):
         return functools.partial(fs._cat_file, urlpath)
     else:
@@ -264,15 +279,15 @@
         raise ValueError(
             "If you want to use a non-local filesystem, you need to specify a cache_dir")
     if not os.path.exists(cache_dir):
         os.makedirs(cache_dir, exist_ok=True)
     lpath = os.path.join(
         cache_dir, cache_mapper(urlpath))
     if not os.path.exists(lpath):
-        fs.get_file(urlpath, lpath, callback=callback) # type: ignore
+        fs.get_file(urlpath, lpath, callback=callback)  # type: ignore
     return lpath
 
 
 def get_as_locally_cached_filesystem_if_remote(urlpath: str, storage_options: dict[str, Any] | None = None, cache_dir: str | None = None, cache_mapper: AbstractCacheMapper = PathCacheMapper()):
     fs = get_async_filesystem(urlpath, storage_options=storage_options)
     if getattr(fs, "local_file", False):
         return fs
```

### Comparing `hscitorchutil-0.1.65/hscitorchutil/processlocal.py` & `hscitorchutil-0.1.66/hscitorchutil/processlocal.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.65/hscitorchutil/sqlite.py` & `hscitorchutil-0.1.66/hscitorchutil/sqlite.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.65/pyproject.toml` & `hscitorchutil-0.1.66/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hscitorchutil"
-version = "0.1.65"
+version = "0.1.66"
 description = "HSCI research group utilities for pytorch (lightning)"
 authors = ["Eetu Mäkelä <eetu.makela@helsinki.fi>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/hsci-r/hscitorchutil"
 keywords = [
     "pytorch",
```

### Comparing `hscitorchutil-0.1.65/PKG-INFO` & `hscitorchutil-0.1.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hscitorchutil
-Version: 0.1.65
+Version: 0.1.66
 Summary: HSCI research group utilities for pytorch (lightning)
 Home-page: https://github.com/hsci-r/hscitorchutil
 License: MIT
 Keywords: pytorch,dataset
 Author: Eetu Mäkelä
 Author-email: eetu.makela@helsinki.fi
 Requires-Python: >=3.10,<3.12
```

