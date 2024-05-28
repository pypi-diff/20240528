# Comparing `tmp/tehzor-0.0.5.tar.gz` & `tmp/tehzor-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tehzor-0.0.5.tar", last modified: Fri Apr 26 15:46:41 2024, max compression
+gzip compressed data, was "tehzor-0.0.6.tar", last modified: Tue May 28 14:26:50 2024, max compression
```

## Comparing `tehzor-0.0.5.tar` & `tehzor-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 15:46:41.923295 tehzor-0.0.5/
--rw-rw-rw-   0        0        0     1082 2024-04-12 09:32:26.000000 tehzor-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     1955 2024-04-26 15:46:41.923295 tehzor-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1180 2024-04-17 06:48:00.000000 tehzor-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 15:46:41.923295 tehzor-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1028 2024-04-26 15:46:10.000000 tehzor-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:46:41.915470 tehzor-0.0.5/tehzor/
--rw-rw-rw-   0        0        0       77 2024-04-17 06:33:50.000000 tehzor-0.0.5/tehzor/__init__.py
--rw-rw-rw-   0        0        0     7727 2024-04-18 10:07:43.000000 tehzor-0.0.5/tehzor/api.py
--rw-rw-rw-   0        0        0      748 2024-04-17 06:33:50.000000 tehzor-0.0.5/tehzor/constants.py
--rw-rw-rw-   0        0        0     6119 2024-04-26 15:31:14.000000 tehzor-0.0.5/tehzor/models.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:46:41.923295 tehzor-0.0.5/tehzor.egg-info/
--rw-rw-rw-   0        0        0     1955 2024-04-26 15:46:41.000000 tehzor-0.0.5/tehzor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2024-04-26 15:46:41.000000 tehzor-0.0.5/tehzor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 15:46:41.000000 tehzor-0.0.5/tehzor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-26 15:46:41.000000 tehzor-0.0.5/tehzor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-26 15:46:41.000000 tehzor-0.0.5/tehzor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 15:46:41.923295 tehzor-0.0.5/tests/
--rw-rw-rw-   0        0        0      531 2024-04-17 06:33:50.000000 tehzor-0.0.5/tests/test_api_create.py
--rw-rw-rw-   0        0        0      927 2024-04-17 06:33:50.000000 tehzor-0.0.5/tests/test_get_problem_id.py
--rw-rw-rw-   0        0        0      915 2024-04-17 13:10:00.000000 tehzor-0.0.5/tests/test_get_space_id.py
--rw-rw-rw-   0        0        0     1399 2024-04-17 15:55:44.000000 tehzor-0.0.5/tests/test_get_space_meters.py
--rw-rw-rw-   0        0        0      975 2024-04-17 06:33:50.000000 tehzor-0.0.5/tests/test_get_work_acceptance.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:26:50.735417 tehzor-0.0.6/
+-rw-rw-rw-   0        0        0     1082 2024-04-12 09:32:26.000000 tehzor-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     1955 2024-05-28 14:26:50.735417 tehzor-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1180 2024-04-17 06:48:00.000000 tehzor-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 14:26:50.735417 tehzor-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1028 2024-05-28 14:21:52.000000 tehzor-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:26:50.719779 tehzor-0.0.6/tehzor/
+-rw-rw-rw-   0        0        0       77 2024-04-17 06:33:50.000000 tehzor-0.0.6/tehzor/__init__.py
+-rw-rw-rw-   0        0        0     7697 2024-05-28 14:12:11.000000 tehzor-0.0.6/tehzor/api.py
+-rw-rw-rw-   0        0        0      748 2024-04-17 06:33:50.000000 tehzor-0.0.6/tehzor/constants.py
+-rw-rw-rw-   0        0        0     6119 2024-04-26 15:31:14.000000 tehzor-0.0.6/tehzor/models.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:26:50.735417 tehzor-0.0.6/tehzor.egg-info/
+-rw-rw-rw-   0        0        0     1955 2024-05-28 14:26:50.000000 tehzor-0.0.6/tehzor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-05-28 14:26:50.000000 tehzor-0.0.6/tehzor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 14:26:50.000000 tehzor-0.0.6/tehzor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-28 14:26:50.000000 tehzor-0.0.6/tehzor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 14:26:50.000000 tehzor-0.0.6/tehzor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 14:26:50.719779 tehzor-0.0.6/tests/
+-rw-rw-rw-   0        0        0      531 2024-04-17 06:33:50.000000 tehzor-0.0.6/tests/test_api_create.py
+-rw-rw-rw-   0        0        0      927 2024-04-17 06:33:50.000000 tehzor-0.0.6/tests/test_get_problem_id.py
+-rw-rw-rw-   0        0        0      915 2024-04-17 13:10:00.000000 tehzor-0.0.6/tests/test_get_space_id.py
+-rw-rw-rw-   0        0        0     1399 2024-04-17 15:55:44.000000 tehzor-0.0.6/tests/test_get_space_meters.py
+-rw-rw-rw-   0        0        0      975 2024-05-28 14:12:40.000000 tehzor-0.0.6/tests/test_get_work_acceptance.py
```

### Comparing `tehzor-0.0.5/LICENSE.txt` & `tehzor-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.5/PKG-INFO` & `tehzor-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tehzor
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python API wrapper for Tehzor API
 Home-page: https://github.com/gritsyuk/tehzor
 Download-URL: https://github.com/gritsyuk/tehzor/archive/refs/heads/develop.zip
 Author: Igor Gritsyuk
 Author-email: gritsyuk.igor@gmail.com
 Project-URL: GitHub, https://github.com/gritsyuk/tehzor
 Keywords: tehzor api tehzorapi construction supervision operation inspections constarctionsite building management
```

### Comparing `tehzor-0.0.5/README.md` & `tehzor-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.5/setup.py` & `tehzor-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
   
 
 setup(
   name='tehzor',
-  version='0.0.5',
+  version='0.0.6',
   author='Igor Gritsyuk',
   author_email='gritsyuk.igor@gmail.com',
   description='A Python API wrapper for Tehzor API',
   download_url='https://github.com/gritsyuk/tehzor/archive/refs/heads/develop.zip',
   long_description=long_description,
   long_description_content_type='text/markdown',
   url='https://github.com/gritsyuk/tehzor',
```

### Comparing `tehzor-0.0.5/tehzor/api.py` & `tehzor-0.0.6/tehzor/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from aiohttp import ClientSession, ClientResponse
 from asyncio import Semaphore
 from typing import List, AsyncGenerator, Optional
-from .models import (ProblemFilter, 
-                     Problem, 
-                     WorkAcceptances, 
-                     Space, 
+from .models import (ProblemFilter,
+                     Problem,
+                     WorkAcceptances,
+                     Space,
                      SpaceMeters)
 
 
 class TehzorAPIError(Exception):
     pass
 
 
@@ -68,78 +68,78 @@
                                     verify_ssl=False) as r:
             await self._handle_response(r)
             res_json = await r.json()
 
             return Problem.model_validate(res_json)
 
     async def get_problems(self,
-                           user_id: str = None,  
+                           user_id: str = None,
                            limit: int = 50000,
-                           offset: int = 0, 
+                           offset: int = 0,
                            filter: Optional[ProblemFilter] = None) -> AsyncGenerator[Problem, None]:
         url = r"/problems"
         if not user_id and self.user_id:
             user_id = self.user_id
         params = dict(userId=user_id,
-                      limit=limit, 
+                      limit=limit,
                       offset=offset)
         filter_json = filter.model_dump() if filter else None
-        async with self.session.get(url, 
-                                    params=params, 
-                                    proxy=self.proxy, 
+        async with self.session.get(url,
+                                    params=params,
+                                    proxy=self.proxy,
                                     json=filter_json) as r:
             await self._handle_response(r)
             res_json = await r.json()
             for data in res_json:
                 yield Problem.model_validate(data)
-    
+
     async def get_work_acceptance(self, id: str) -> WorkAcceptances:
         url = f"/work-acceptances/{id}"
         async with self.session.get(url,
                                     proxy=self.proxy,
                                     verify_ssl=False) as r:
             await self._handle_response(r)
             res_json = await r.json()
             return WorkAcceptances.model_validate(res_json)
 
     async def get_work_acceptances(self,
-                                   object_id: str= "",
+                                   object_id: str = "",
                                    limit: int = 50000,
                                    offset: int = 0,
                                    ) -> AsyncGenerator[WorkAcceptances, None]:
-        url = "/work-acceptances"
+        url = "/work-acceptances/get-work-acceptances"
         params = dict(objectId=object_id,
-                      limit=limit, 
+                      limit=limit,
                       offset=offset)
-        async with self.session.get(url,
-                                    params=params,
-                                    proxy=self.proxy,
-                                    verify_ssl=False) as r:
+        async with self.session.post(url,
+                                     params=params,
+                                     proxy=self.proxy,
+                                     verify_ssl=False) as r:
             await self._handle_response(r)
             res_json = await r.json()
             for data in res_json:
                 yield WorkAcceptances.model_validate(data)
 
     async def update_problem(self, id: str, data: dict):
         url = fr"/problems/{id}"
         async with self.session.post(url,
                                      data=data,
                                      proxy=self.proxy,
                                      verify_ssl=False) as r:
             assert r.status == 201
             return await r.json()
-    
+
     # async def create_problem(self, data: ProblemNew) -> Problem:
     #     url = fr"/problems"
     #     async with self.session.post(url,
     #                                  data=data,
     #                                  proxy=self.proxy,
     #                                  verify_ssl=False) as r:
-            # assert r.status == 201
-            # return await r.json()
+    # assert r.status == 201
+    # return await r.json()
 
     async def get_contract_forms(self) -> dict:
         url = r"/contract-forms"
         async with self.session.get(url,
                                     proxy=self.proxy,
                                     verify_ssl=False) as r:
             assert r.status == 200
@@ -149,37 +149,37 @@
         url = fr"/space-owners"
         async with self.semaphore:
             async with self.session.post(url,
                                          data=data,
                                          proxy=self.proxy,
                                          verify_ssl=False) as r:
                 assert r.status == 201
-    
+
     async def get_space(self, id: str) -> Space:
         url = f"/spaces/{id}"
         async with self.session.get(url,
                                     proxy=self.proxy,
                                     verify_ssl=False) as r:
             await self._handle_response(r)
             res_json = await r.json()
             return Space.model_validate(res_json)
-        
+
     async def get_space_meters(self, id: str) -> List[SpaceMeters]:
         url = f"/spaces/{id}/meters"
         async with self.session.get(url,
                                     proxy=self.proxy,
                                     verify_ssl=False) as r:
             await self._handle_response(r)
             res_json = await r.json()
             space_meters_list = []
             for data in res_json:
                 space_meters_list.append(SpaceMeters.model_validate(data))
 
             return space_meters_list
-        
+
     async def update_spaces(self, id: str, data: dict):
         url = fr"/spaces/{id}"
         async with self.semaphore:
             async with self.session.post(url,
                                          data=data,
                                          proxy=self.proxy,
                                          verify_ssl=False) as r:
```

### Comparing `tehzor-0.0.5/tehzor/constants.py` & `tehzor-0.0.6/tehzor/constants.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.5/tehzor/models.py` & `tehzor-0.0.6/tehzor/models.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.5/tehzor.egg-info/PKG-INFO` & `tehzor-0.0.6/tehzor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tehzor
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python API wrapper for Tehzor API
 Home-page: https://github.com/gritsyuk/tehzor
 Download-URL: https://github.com/gritsyuk/tehzor/archive/refs/heads/develop.zip
 Author: Igor Gritsyuk
 Author-email: gritsyuk.igor@gmail.com
 Project-URL: GitHub, https://github.com/gritsyuk/tehzor
 Keywords: tehzor api tehzorapi construction supervision operation inspections constarctionsite building management
```

### Comparing `tehzor-0.0.5/tests/test_api_create.py` & `tehzor-0.0.6/tests/test_api_create.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.5/tests/test_get_problem_id.py` & `tehzor-0.0.6/tests/test_get_problem_id.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.5/tests/test_get_space_id.py` & `tehzor-0.0.6/tests/test_get_space_id.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.5/tests/test_get_space_meters.py` & `tehzor-0.0.6/tests/test_get_space_meters.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.5/tests/test_get_work_acceptance.py` & `tehzor-0.0.6/tests/test_get_work_acceptance.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 @pytest.mark.asyncio
 async def test_get_work_acceptance_success():
     thz = await TehzorAPI.create(api_key=API_KEY,
                                  user_id=USER_ID
                                  )
     try:
-        res = await thz.get_work_acceptance("661a261d5d3aea11af15b08f")
+        res = await thz.get_work_acceptance("6655bb0bfc1f87d4ec04d167")
         assert isinstance(res, WorkAcceptances)
     finally:
         await thz.session_close()
 
 
 @pytest.mark.asyncio
 async def test_get_work_acceptance_nonexistent_id():
```

