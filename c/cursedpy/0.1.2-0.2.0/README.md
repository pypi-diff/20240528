# Comparing `tmp/cursedpy-0.1.2.tar.gz` & `tmp/cursedpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursedpy-0.1.2.tar", max compression
+gzip compressed data, was "cursedpy-0.2.0.tar", max compression
```

## Comparing `cursedpy-0.1.2.tar` & `cursedpy-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      846 2024-05-21 20:42:41.769295 cursedpy-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-21 19:19:35.064570 cursedpy-0.1.2/cursedpy/__init__.py
--rw-r--r--   0        0        0    13777 2024-05-21 14:44:17.972681 cursedpy-0.1.2/cursedpy/cursed.py
--rw-r--r--   0        0        0        0 2024-05-21 11:32:26.515522 cursedpy-0.1.2/cursedpy/tools/__init__.py
--rw-r--r--   0        0        0      146 2024-05-21 12:49:22.682508 cursedpy-0.1.2/cursedpy/tools/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    21424 2024-05-21 12:49:22.689175 cursedpy-0.1.2/cursedpy/tools/__pycache__/types.cpython-312.pyc
--rw-r--r--   0        0        0    11166 2024-05-21 11:32:26.515522 cursedpy-0.1.2/cursedpy/tools/types.py
--rw-r--r--   0        0        0      375 2024-05-21 21:51:37.883969 cursedpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1304 1970-01-01 00:00:00.000000 cursedpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1916 2024-05-27 23:09:55.542558 cursedpy-0.2.0/README.md
+-rw-r--r--   0        0        0      511 2024-05-27 21:20:56.206746 cursedpy-0.2.0/cursedpy/__init__.py
+-rw-r--r--   0        0        0    13289 2024-05-27 21:20:56.210080 cursedpy-0.2.0/cursedpy/cursed.py
+-rw-r--r--   0        0        0       61 2024-05-27 21:20:56.210080 cursedpy-0.2.0/cursedpy/http/__init__.py
+-rw-r--r--   0        0        0      946 2024-05-27 21:20:56.210080 cursedpy-0.2.0/cursedpy/http/abc.py
+-rw-r--r--   0        0        0     1390 2024-05-27 21:20:56.210080 cursedpy-0.2.0/cursedpy/http/aiohttp_client.py
+-rw-r--r--   0        0        0     2188 2024-05-27 21:20:56.210080 cursedpy-0.2.0/cursedpy/http/cursed_client.py
+-rw-r--r--   0        0        0    11388 2024-05-27 21:20:56.210080 cursedpy-0.2.0/cursedpy/types.py
+-rw-r--r--   0        0        0      394 2024-05-27 23:05:58.500749 cursedpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2414 1970-01-01 00:00:00.000000 cursedpy-0.2.0/PKG-INFO
```

### Comparing `cursedpy-0.1.2/cursedpy/cursed.py` & `cursedpy-0.2.0/cursedpy/cursed.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,132 +1,76 @@
-#!/bin/python3
-import argparse
-import requests
-from dataclasses import dataclass
-from enum import Enum
-from pathlib import Path
 import json
-from typing import Any, Optional, List
+from typing import Any, Optional
 from urllib.parse import urlencode
-from functools import wraps
 from dataclass_wizard import fromdict, asdict
-import colorama
 
-from tools.types import *
+import asyncio
 
-DEBUG = False
-REQUEST = True
+from .http import CurseHTTP
+from .types import *
 
-#Test API token used by official curseforge apps
-import base64
-CFApiKey = base64.b64decode("JDJhJDEwJGJMNGJJTDVwVVdxZmNPN0tRdG5NUmVha3d0ZkhiTktoNnYxdVRwS2x6aHdvdWVFSlFuUG5t").decode('utf-8')
-
-class CFAPI:
-    """
-    Base class for CurseForge API
-    """
-    def __init__(self, api_key):
-        self.api_key = api_key
-    def cf_get(self, endpoint_url: str):
-        if DEBUG: print(f'GET: {base_url+endpoint_url}')
-        return requests.get(url=base_url+endpoint_url, headers={
-            'Accept': 'application/json',
-            'x-api-key': self.api_key})
-    def cf_post(self, endpoint_url, data):
-        if DEBUG: print(f'POST: {base_url+endpoint_url}\nDATA: {data}')
-        return requests.post(url=base_url+endpoint_url, headers={
-            'Accept': 'application/json',
-            'Content-Type': 'application/json',
-            'x-api-key': self.api_key}, data=data)
-    def cf_api(self, endpoint: endpoint, data: Optional[object] = None, params: Optional[dict] = None, query: Optional[dict] = None):
-        """
-        Call to curseforge API
-        :param endpoint:  Endpoint class with `endpoint` string, request method and endpoint description inside it. Predefined in `endpoints` variable.
-        :param data: Data sent to server, POST only. (cf_post)
-        :param params: `!!MANDATORY!!` Params to substitute in endpoint string
-        :param query: Url query
-        """
-        method = endpoint.method
-        if data: data = json.dumps(data)
-        if query: 
-            query = urlencode(query)
-        else:
-            query = ""
-        endpoint_url = str(endpoint.endpoint)+query
-        if DEBUG:
-            d_str = 'endpoint: {endpoint_url}\napi_key:{api_key}\ndata:{data}\nparams:{params}\nquery:{query}'.format(
-                endpoint_url = endpoint_url,
-                api_key = self.api_key,
-                data = data,
-                params = params,
-                query = query
-            )
-            print(d_str)
-        if REQUEST:
-            if params:
-                endpoint_url = endpoint_url.format(**params)
-            if method == GET:
-                return(self.cf_get(endpoint_url))
-            if method == POST:
-                return(self.cf_post(endpoint_url, data))
-
-class CFGames(CFAPI):
-    #!! Add apgination parameters
-    def games(self) -> tuple[list[Game], Pagination]:
+class CFGames(CurseHTTP):
+    async def games(self, index: Optional[int] = None, pageSize: Optional[int] = None) -> tuple[list[Game], Pagination]:
         """
         Get all games that are available to the provided API key.
         """
-        response = json.loads(self.cf_api(endpoints["games"]).text)
+        query = {}
+        if pageSize: query['pageSize'] = pageSize
+        if index: query['index'] = index
+        response = await self.api(endpoints["games"], query=query)
         pagination = Pagination(**response['pagination'])
         data = [fromdict(Game, game) for game in response['data']]
         return(data, pagination)
-    def game(self, gameId) -> Game:
+
+    async def game(self, gameId) -> Game:
         """
         Get a single game.
         A private game is only accessible by its respective API key.
         """
-        response = json.loads(self.cf_api(endpoints["game"], params={"gameId":gameId}).text)
+        response = await self.api(endpoints["game"], params={"gameId":gameId})
         print(response)
         data = fromdict(Game, response['data'])
         return(data)
-    def versions(self, gameId) -> list[GameVersionsByType]:
+
+    async def versions(self, gameId: int) -> list[GameVersionsByType]:
         """
         Get all available versions for each known version type of the specified game.
         A private game is only accessible to its respective API key.
         """
-        response = json.loads(self.cf_api(endpoints["versions"], params={"gameId":gameId}).text)
+        response = await self.api(endpoints["versions"], params={"gameId":gameId})
         data = [fromdict(GameVersionsByType, vbt) for vbt in response['data']]
         return(data)
-    def version_types(self, gameId) -> list[GameVersionType]:
+
+    async def version_types(self, gameId: int) -> list[GameVersionType]:
         """
-        Get all available version types of the specified game.
-        A private game is only accessible to its respective API key.
         Currently, when creating games via the CurseForge for Studios Console, you are limited to a single game version type.
         This means that this endpoint is probably not useful in most cases and is relevant mostly when handling existing games that have multiple game versions such as World of Warcraft and Minecraft (e.g. 517 for wow_retail).
         """
-        response = json.loads(self.cf_api(endpoints["version_types"], params={"gameId":gameId}).text)
+        response = await self.api(endpoints["version_types"], params={"gameId":gameId})
         data = [fromdict(GameVersionType, gvt) for gvt in response['data']]
         return(data)
 
-class CFCategories(CFAPI):
-    def categories(self, gameId: int, classId: Optional[int] = None, classesOnly: Optional[bool] = None) -> list[Category]:
+    # Add version types V2
+
+class CFCategories(CurseHTTP):
+    async def categories(self, gameId: int, classId: Optional[int] = None, classesOnly: Optional[bool] = None) -> list[Category]:
         """
         Get all available classes and categories of the specified game.
         Specify a game id for a list of all game categories, or a class id for a list of categories under that class.
         Specifiy the classes Only flag to just get the classes for a given game.
         """
         query = {"gameId":gameId}
         if classId: query['classId'] = classId
         if classesOnly: query['classesOnly'] = classesOnly
-        response = json.loads(self.cf_api(endpoints["categories"],query=query).text)
+        response = await self.api(endpoints["categories"],query=query)
         data = [fromdict(Category, category) for category in response['data']]
         return(data)
 
-class CFMods(CFAPI):
-    def search_mods(
+class CFMods(CurseHTTP):
+    async def search_mods(
         self, gameId: int, classId: Optional[int]=None,
         categoryId: Optional[int]=None, categoryIds: Optional[str]=None,
         gameVersion: Optional[str]=None, gameVersions: Optional[str]=None,
         searchFilter: Optional[str]=None, sortField: Optional[ModsSearchSortField]=None,
         sortOrder: Optional[SortOrder]=None, modLoaderType: Optional[ModLoaderType]=None,
         modLoaderTypes: Optional[str]=None, gameVersionTypeId: Optional[int]=None,
         authorId: Optional[int]=None, primaryAuthorId: Optional[int]=None,
@@ -149,159 +93,194 @@
         if gameVersionTypeId: query['gameVersionTypeId'] = gameVersionTypeId
         if authorId: query['authorId'] = authorId
         if primaryAuthorId: query['primaryAuthorId'] = primaryAuthorId
         if slug: query['slug'] = slug
         if index: query['index'] = index
         if pageSize: query['pageSize'] = pageSize
         # Call curseforge api
-        response = json.loads(self.cf_api(endpoints['search_mods'], query=query).text)
+        response = await self.api(endpoints['search_mods'], query=query)
         pagination = Pagination(**response['pagination'])
         data = [fromdict(Mod, moddata) for moddata in response['data']]
         return(data, pagination)
 
-    def get_mod(self, modId: int) -> Mod:
+    async def get_mod(self, modId: int) -> Mod:
         """
         Get a single mod.
         """
-        response = json.loads(self.cf_api(endpoints['get_mod'], params={'modId':modId}).text)
+        response = await self.api(endpoints['get_mod'], params={'modId':modId})
         data = fromdict(Mod, response['data'])
         return(data)
 
-    def get_mods(self, modIds: list[int], filterPCOnly: Optional[bool] = True) -> list[Mod]:
+    async def get_mods(self, modIds: list[int], filterPCOnly: Optional[bool] = True) -> list[Mod]:
         """
         Get a list of mods belonging the the same game.
         """
         body = {"modIds":modIds}
         if filterPCOnly: body["filterPCOnly"] = filterPCOnly
-        response = json.loads(self.cf_api(endpoints['get_mods'], data=body).text)
+        response = await self.api(endpoints['get_mods'], data=body)
         data = [fromdict(Mod, moddata) for moddata in response['data']]
         return(data)
 
-    def get_featured_mods(self, gameId: int, excludedModIds: Optional[List] = None, gameVersionTypeId: Optional[int] = None) -> FeaturedModsResponse:
+    async def get_featured_mods(self, gameId: int, excludedModIds: Optional[list] = None, gameVersionTypeId: Optional[int] = None) -> FeaturedModsResponse:
         """
         Get a list of featured, popular and recently updated mods.
         """
         body = {"gameId":gameId}
         if excludedModIds: body['excludedModIds'] = excludedModIds
         if gameVersionTypeId: body['gameVersionTypeId'] = gameVersionTypeId
-        response = json.loads(self.cf_api(endpoints['get_featured_mods'],data=body).text)
+        response = await self.api(endpoints['get_featured_mods'],data=body)
         data = fromdict(FeaturedModsResponse, response['data'])
         return(data)
 
-    def get_mod_description(self, modId: int, raw: Optional[bool] = None, stripped: Optional[bool] = None, markup: Optional[bool] = None) -> str:
+    async def get_mod_description(self, modId: int, raw: Optional[bool] = None, stripped: Optional[bool] = None, markup: Optional[bool] = None) -> str:
         """
         Get the full description of a mod in HTML format.
         """
         query = {"modId":modId}
         if raw: query['raw'] = raw
         if stripped: query['stripped'] = stripped
         if markup: query['markup'] = markup
-        response = json.loads(self.cf_api(endpoints['get_mod_description'], query=query).text)
+        response = await self.api(endpoints['get_mod_description'], query=query)
         data = response['data']
         return(data)
 
-class CFFiles(CFAPI):
-    def get_mod_file(self, modId: int, fileId: int) -> File:
+class CFFiles(CurseHTTP):
+    async def get_mod_file(self, modId: int, fileId: int) -> File:
         """
         Get a single file of the specified mod.
         """
-        response = json.loads(self.cf_api(endpoints['get_mod_file'], params={'modId':modId, 'fileId':fileId}).text)
+        response = await self.api(endpoints['get_mod_file'], params={'modId':modId, 'fileId':fileId})
         data = fromdict(Mod, response['data'])
         return(data)
 
-    def get_mod_files(
+    async def get_mod_files(
         self, modId: int, gameVersion: Optional[str] = None,
         modLoaderType: Optional[ModLoaderType] = None, gameVersionTypeId: Optional[int] = None,
         index: Optional[int] = None, pageSize: Optional[int] = None) -> tuple[list[File], Pagination]:
         """
         Get all files of the specified mod.
         """
         query={}
         if gameVersion: query['gameVersion'] = gameVersion
         if modLoaderType: query['modLoaderType'] = modLoaderType
         if gameVersionTypeId: query['gameVersionTypeId'] = gameVersionTypeId
         if index: query['index'] = index
         if pageSize: query['pageSize'] = pageSize
-        response = json.loads(self.cf_api(endpoints['get_mod_files'],params={'modId':modId}, query=query).text)
+        response = await self.api(endpoints['get_mod_files'],params={'modId':modId}, query=query)
         pagination = Pagination(**response['pagination'])
         data = [fromdict(File, f) for f in response['data']]
         return(data, pagination)
 
-    def get_files(self, fileIds: list) -> list[File]:
+    async def get_files(self, fileIds: list) -> list[File]:
         """
         Get a list of files.
         """
         body = {"fileIds":fileIds}
-        response = json.loads(self.cf_api(endpoints['get_files'], data=body).text)
+        response = await self.api(endpoints['get_files'], data=body)
         data = [fromdict(File, f) for f in response['data']]
         return(data)
 
-    def get_mod_file_changelog(self, modId: int, fileId: int) -> str:
+    async def get_mod_file_changelog(self, modId: int, fileId: int) -> str:
         """
         Get the changelog of a file in HTML format.
         """
-        respone = json.loads(self.cf_api(endpoints['get_mod_file_changelog'], params={'modId':modId, 'fileId':fileId}).text)
+        respone = await self.api(endpoints['get_mod_file_changelog'], params={'modId':modId, 'fileId':fileId})
         data = response['data']
         return(data)
 
-    def get_mod_file_download_url(self, modId: int, fileId: int) -> str:
+    async def get_mod_file_download_url(self, modId: int, fileId: int) -> str:
         """
         Get a download url for a specific file.
         """
-        response = json.loads(self.cf_api(endpoints['get_mod_file_download_url'], params={'modId':modId, 'fileId':fileId}).text)
+        response = await self.api(endpoints['get_mod_file_download_url'], params={'modId':modId, 'fileId':fileId})
         data = response['data']
         return(data)
 
-class CFMinecraft(CFAPI):
-    def get_minecraft_versions(self, sortDescending: Optional[bool] = None) -> list[MinecraftGameVersion]:
+class CFMinecraft(CurseHTTP):
+    async def get_minecraft_versions(self, sortDescending: Optional[bool] = None) -> list[MinecraftGameVersion]:
         """
         Get all Minecraft versions.
         """
         query = {}
         if sortDescending: query['sortDescending'] = sortDescending
-        response = json.loads(self.cf_api(endpoints['get_minecraft_versions'], query=query).text)
+        response = await self.api(endpoints['get_minecraft_versions'], query=query)
         data = [MinecraftGameVersion(**mc_gv) for mc_gv in response['data']]
         data = [fromdict(MinecraftGameVersion, mc_gv) for mc_gv in response['data']]
         return(data)
 
-    def get_specific_minecraft_version(self, gameVersionString: str) -> MinecraftGameVersion:
+    async def get_specific_minecraft_version(self, gameVersionString: str) -> MinecraftGameVersion:
         """
         Get information about specific Minecraft version.
         """
-        response = json.loads(self.cf_api(endpoints['get_specific_minecraft_version'], params={'gameVersionString':gameVersionString}).text)
+        response = self.api(await endpoints['get_specific_minecraft_version'], params={'gameVersionString':gameVersionString})
         data = fromdict(MinecraftGameVersion, response['data'])
         return(data)
 
-    def get_minecraft_modloaders(self, version: Optional[str] = None, includeAll: Optional[bool] = None) -> list[MinecraftModLoaderIndex]:
+    async def get_minecraft_modloaders(self, version: Optional[str] = None, includeAll: Optional[bool] = None) -> list[MinecraftModLoaderIndex]:
         """
         Get list of all Minecraft modloaders.
         """
         query={}
         if version: query['version'] = version
         if includeAll: query['includeAll'] = includeAll
-        response = json.loads(self.cf_api(endpoints['get_minecraft_modloaders'], query=query).text)
+        response = await self.api(endpoints['get_minecraft_modloaders'], query=query)
         data = [fromdict(MinecraftModLoaderIndex, ml_idx) for ml_idx in response['data']]
         return(data)
 
-    def get_specific_minecraft_modloader(self, modLoaderName: str) -> MinecraftModLoaderVersion:
+    async def get_specific_minecraft_modloader(self, modLoaderName: str) -> MinecraftModLoaderVersion:
         """
         Get everything about specific Minecraft modloader version.
         """
-        response = json.loads(self.cf_api(endpoints['get_specific_minecraft_modloader'],params={'modLoaderName':modLoaderName}).text)
+        response = await self.api(endpoints['get_specific_minecraft_modloader'],params={'modLoaderName':modLoaderName})
         data = fromdict(MinecraftModLoaderVersion, response['data'])
         return(data)
 
-class CFFingerprints(CFAPI):
-    """
-    NOT IMPLEMENTED
-    """
-    pass
+class CFFingerprints(CurseHTTP):
+    async def get_fingerprints_matches_by_game_id(self, gameId: int, fingerprints: list[int]) -> FingerprintsMatchesResult:
+        """
+        Get mod files that match a list of fingerprints for a given game id.
+        """
+        response = await self.api(endpoint['get_fingerprints_matches_by_game_id'],data={"fingerprints":fingerprints},params={"gameId":gameId})
+        data = fromdict(FingerprintsMatchesResult, response['data'])
+        return(data)
+    
+    async def get_fingerprints_matches(self, fingerprint: list[int]) -> FingerprintsMatchesResult:
+        """
+        Get mod files that match a list of fingerprints.
+        """
+        response = await self.api(endpoint['get_fingerprints_matches'],data={"fingerprints":fingerprints})
+        data = fromdict(FingerprintsMatchesResult, response['data'])
+        return(data)
+
+    async def get_fingerprints_fuzzy_matches_by_game_id(self, gameId: int, fingerprints: list[FolderFingerprint]) -> FingerprintFuzzyMatchResult:
+        """
+        Get mod files that match a list of fingerprints using fuzzy matching.
+        """
+        response = await self.api(endpoint['get_fingerprints_fuzzy_matches_by_game_id'], data={"gameId": gameId, "fingerprints":fingerprints}, params={"gameId": gameId})
+        data = fromdict(FingerprintFuzzyMatchResult, response['data'])
+        return(data)
+
+    async def get_fingerprints_fuzzy_matches(self, fingerprints: list[FolderFingerprint]) -> FingerprintFuzzyMatchResult:
+        """
+        Get mod files that match a list of fingerprints using fuzzy matching.
+        """
+        response = await self.api(endpoint['get_fingerprints_fuzzy_matches'], data={"gameId": gameId, "fingerprints":fingerprints})
+        data = fromdict(FingerprintFuzzyMatchResult, response['data'])
+        return(data)
 
 class CFClient:
     def __init__(self, api_key):
         self.api_key = api_key
         self.Games = CFGames(self.api_key)
         self.Categories = CFCategories(self.api_key)
         self.Mods = CFMods(self.api_key)
         self.Files = CFFiles(self.api_key)
         self.Minecraft = CFMinecraft(self.api_key)
-        self.Fingerprints = CFFingerprints(self.api_key)
+        self.Fingerprints = CFFingerprints(self.api_key)
+
+    async def close(self):
+        await self.Games.close()
+        await self.Categories.close()
+        await self.Mods.close()
+        await self.Files.close()
+        await self.Minecraft.close()
+        await self.Fingerprints.close()
```

### Comparing `cursedpy-0.1.2/cursedpy/tools/types.py` & `cursedpy-0.2.0/cursedpy/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,107 @@
 import argparse
-import requests
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 import json
-from typing import Any, Optional, List
-from urllib.parse import urlencode
-from functools import wraps
+from typing import Any, Optional
 import datetime
 import json
-from types import SimpleNamespace
-
-base_url = "https://api.curseforge.com"
-
-def JsonToType(data):
-    """
-    Transform API response to python type
-    """
-    return(json.loads(data, object_hook=lambda d: SimpleNamespace(**d)))
 
 class req_method(Enum):
     GET = 0
     POST = 1
+    DOWNLOAD = 2
 
 GET = req_method.GET
 POST = req_method.POST
+DOWNLOAD = req_method.DOWNLOAD
 
 @dataclass
 class endpoint:
     method: req_method
     endpoint: Path
-    description: Optional[str] = None
 
 endpoints = {
-    #Games
-    "games":endpoint(GET, '/v1/games', 'Get all games that are available to the provided API key.'),
-    "game":endpoint(GET, '/v1/games/{gameId}', 'Get a single game. A private game is only accessible by its respective API key.'),
-    "versions":endpoint(GET, '/v2/games/{gameId}/versions', 'Get all available versions for each known version type of the specified game. A private game is only accessible to its respective API key.'),
-    "version_types":endpoint(GET,'/v1/games/{gameId}/version-types','Get all available version types of the specified game.'),
-    #Categories
-    "categories":endpoint(GET, '/v1/categories?', "Get all available classes and categories of the specified game. Specify a game id for a list of all game categories, or a class id for a list of categories under that class. specifiy the classes Only flag to just get the classes for a given game."),
-    #Mods
-    "search_mods":endpoint(GET, '/v1/mods/search?','Get all mods that match the search criteria.'),
-    "get_mod":endpoint(GET, '/v1/mods/{modId}', 'Get a single mod.'),
-    "get_mods":endpoint(POST, '/v1/mods', 'Get a list of mods belonging the the same game.'),
-    "get_featured_mods":endpoint(POST, '/v1/mods/featured', 'Get a list of featured, popular and recently updated mods.'),
-    "get_mod_description":endpoint(GET, '/v1/mods/{modId}/description', 'Get the full description of a mod in HTML format.'),
-    #Files
-    "get_mod_file":endpoint(GET,'/v1/mods/{modId}/files/{fileId}','Get a single file of the specified mod.'),
-    "get_mod_files":endpoint(GET,'/v1/mods/{modId}/files','Get all files of the specified mod.'),
-    "get_files":endpoint(POST, '/v1/mods/files', 'Get a list of files.'),
-    "get_mod_file_changelog":endpoint(GET, '/v1/mods/{modId}/files/{fileId}/changelog', 'Get the changelog of a file in HTML format.'),
-    "get_mod_file_download_url":endpoint(GET, '/v1/mods/{modId}/files/{fileId}/download-url', 'Get a download url for a specific file.'),
-    #Minecraft
-    "get_minecraft_versions":endpoint(GET,'/v1/minecraft/version',''),
-    "get_specific_minecraft_version":endpoint(GET,'/v1/minecraft/version/{gameVersionString}',''),
-    "get_minecraft_modloaders":endpoint(GET,'/v1/minecraft/modloader',''),
-    "get_specific_minecraft_modloader":endpoint(GET,'/v1/minecraft/modloader/{modLoaderName}','')
-    #Fingerprints ???
-}
+        # Games
+    # Get all games that are available to the provided API key.
+    "games":endpoint(GET, '/v1/games?'),
 
-@dataclass
-class ApiResponseOf:
-    data: Any
-GetResponse = ApiResponseOf # Alias
+    # Get a single game. A private game is only accessible by its respective API key.
+    "game":endpoint(GET, '/v1/games/{gameId}'),
+
+    # Get all available versions for each known version type of the specified game. A private game is only accessible to its respective API key.
+    "versions":endpoint(GET, '/v2/games/{gameId}/versions'),
+
+    # Get all available version types of the specified game.
+    "version_types":endpoint(GET,'/v1/games/{gameId}/version-types'),
+
+        # Categories
+    # Get all available classes and categories of the specified game. Specify a game id for a list of all game categories, or a class id for a list of categories under that class. specifiy the classes Only flag to just get the classes for a given game.
+    "categories":endpoint(GET, '/v1/categories?'),
+
+        # Mods
+    # Get all mods that match the search criteria.
+    "search_mods":endpoint(GET, '/v1/mods/search?'),
+
+    # Get a single mod.
+    "get_mod":endpoint(GET, '/v1/mods/{modId}'),
+
+    # Get a list of mods belonging the the same game.
+    "get_mods":endpoint(POST, '/v1/mods'),
+
+    # Get a list of featured, popular and recently updated mods.
+    "get_featured_mods":endpoint(POST, '/v1/mods/featured'),
+
+    # Get the full description of a mod in HTML format.
+    "get_mod_description":endpoint(GET, '/v1/mods/{modId}/description'),
+
+        # Files
+    # Get a single file of the specified mod.
+    "get_mod_file":endpoint(GET,'/v1/mods/{modId}/files/{fileId}'),
+
+    # Get all files of the specified mod.
+    "get_mod_files":endpoint(GET,'/v1/mods/{modId}/files'),
+
+    # Get a list of files.
+    "get_files":endpoint(POST, '/v1/mods/files'),
+
+    # Get the changelog of a file in HTML format.
+    "get_mod_file_changelog":endpoint(GET, '/v1/mods/{modId}/files/{fileId}/changelog'),
+
+    # Get a download url for a specific file.
+    "get_mod_file_download_url":endpoint(GET, '/v1/mods/{modId}/files/{fileId}/download-url'),
+
+        # Minecraft
+    "get_minecraft_versions":endpoint(GET,'/v1/minecraft/version'),
+    "get_specific_minecraft_version":endpoint(GET,'/v1/minecraft/version/{gameVersionString}'),
+    "get_minecraft_modloaders":endpoint(GET,'/v1/minecraft/modloader'),
+    "get_specific_minecraft_modloader":endpoint(GET,'/v1/minecraft/modloader/{modLoaderName}'),
+
+        # Fingerprints
+    # Get mod files that match a list of fingerprints for a given game id.
+    "get_fingerprints_matches_by_game_id":endpoint(POST,'v1/fingerprints/{gameId}'),
+
+    # Get mod files that match a list of fingerprints.
+    "get_fingerprints_matches":endpoint(POST, '/v1/fingerprints'),
+
+    # Get mod files that match a list of fingerprints using fuzzy matching.
+    "get_fingerprints_fuzzy_matches_by_game_id":endpoint(POST, '/v1/fingerprints/fuzzy/{gameId}'),
+
+    # Get mod files that match a list of fingerprints using fuzzy matching.
+    "get_fingerprints_fuzzy_matches":endpoint(POST, '/v1/fingerprints/fuzzy')
+}
 
 @dataclass
 class Pagination:
     index: int
     pageSize: int
     resultCount: int
     totalCount: int
 
-@dataclass
-class GetResponseWithPagination:
-    data: Any
-    pagination: Pagination
-
 class ModsSearchSortField(Enum):
     Featured = 1
     Popularity = 2
     LastUpdated = 3
     Name = 4
     Author = 5
     TotalDownloads = 6
```

