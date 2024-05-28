# Comparing `tmp/pyneople-0.3.9.tar.gz` & `tmp/pyneople-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.3.9.tar", last modified: Wed May  8 09:15:21 2024, max compression
+gzip compressed data, was "pyneople-0.4.0.tar", last modified: Tue May 28 13:57:47 2024, max compression
```

## Comparing `pyneople-0.3.9.tar` & `pyneople-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:15:21.209385 pyneople-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-08 09:15:05.000000 pyneople-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 09:15:21.209385 pyneople-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-08 09:15:05.000000 pyneople-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 09:15:05.000000 pyneople-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:15:21.209385 pyneople-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-08 09:15:05.000000 pyneople-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:15:21.205385 pyneople-0.3.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:15:21.209385 pyneople-0.3.9/src/pyneople/
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-08 09:15:05.000000 pyneople-0.3.9/src/pyneople/METADATA.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 09:15:05.000000 pyneople-0.3.9/src/pyneople/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37562 2024-05-08 09:15:05.000000 pyneople-0.3.9/src/pyneople/character.py
--rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-05-08 09:15:05.000000 pyneople-0.3.9/src/pyneople/database_connecter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-08 09:15:05.000000 pyneople-0.3.9/src/pyneople/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:15:21.209385 pyneople-0.3.9/src/pyneople.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 09:15:21.000000 pyneople-0.3.9/src/pyneople.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 09:15:21.000000 pyneople-0.3.9/src/pyneople.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:15:21.000000 pyneople-0.3.9/src/pyneople.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 09:15:21.000000 pyneople-0.3.9/src/pyneople.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:57:47.477291 pyneople-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 13:57:35.000000 pyneople-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-05-28 13:57:47.477291 pyneople-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-05-28 13:57:35.000000 pyneople-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 13:57:35.000000 pyneople-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:57:47.477291 pyneople-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-28 13:57:35.000000 pyneople-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:57:47.473291 pyneople-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:57:47.473291 pyneople-0.4.0/src/pyneople/
+-rw-r--r--   0 runner    (1001) docker     (127)     8787 2024-05-28 13:57:35.000000 pyneople-0.4.0/src/pyneople/METADATA.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 13:57:35.000000 pyneople-0.4.0/src/pyneople/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42491 2024-05-28 13:57:35.000000 pyneople-0.4.0/src/pyneople/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23498 2024-05-28 13:57:35.000000 pyneople-0.4.0/src/pyneople/database_connecter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-05-28 13:57:35.000000 pyneople-0.4.0/src/pyneople/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:57:47.473291 pyneople-0.4.0/src/pyneople.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-05-28 13:57:47.000000 pyneople-0.4.0/src/pyneople.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 13:57:47.000000 pyneople-0.4.0/src/pyneople.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:57:47.000000 pyneople-0.4.0/src/pyneople.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 13:57:47.000000 pyneople-0.4.0/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.3.9/LICENSE` & `pyneople-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.3.9/setup.py` & `pyneople-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.3.9",
+    version="0.4.0",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/pyneople",
     project_urls={
```

### Comparing `pyneople-0.3.9/src/pyneople/METADATA.py` & `pyneople-0.4.0/src/pyneople/METADATA.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,28 @@
     "프레이" : "prey",
     "시로코" : "siroco"
     }
 
 # 서버 ID 가 key NAME 이 value
 SERVER_ID_2_NAME = {v : k for k , v in SERVER_NAME_2_ID.items()}
 
+# 서버 ID 가 total_id에 저장되는 값
+SERVER_ID_2_TOTAL_ID = {
+    'anton': 'a',
+    'bakal': 'b',
+    'cain': 'c',
+    'casillas': 'k',
+    'diregie': 'd',
+    'hilder': 'h',
+    'prey': 'p',
+    'siroco': 's'
+    }
+
+TOTAL_ID_2_SERVER_ID = {v : k for k , v in SERVER_ID_2_TOTAL_ID.items()}
+
 # 서버 ID 문자열 길이의 최대값
 SERVERLENGTH = max(list(map(lambda x : len(x), list(SERVER_NAME_2_ID.values()))))
 
 # 직업명
 JOBCLASS = {
     "귀검사(남)" : ["웨펀마스터", "버서커", "소울브링어", "아수라", "검귀"],
     "격투가(남)" : ["넨마스터", "스트리트파이터", "그래플러", "스트라이커"],
@@ -49,18 +63,18 @@
 
 # 직업명 문자열 길이의 최대값
 JOB_NAME_LENGTH = max(list(map(lambda x : len(x), list(JOBCLASS.keys()))))
 
 del jobclass_list
 
 # 착용가능 장비
-EQUIPMENT_LIST = ['weapon', 'title', 'jacket', 'shoulder', 'pants', 'shoes', 'waist', 'amulet', 'wrist', 'ring', 'support', 'magic_ston', 'earring', 'set_item_info']
+EQUIPMENT_LIST = ['total_id', 'weapon', 'title', 'jacket', 'shoulder', 'pants', 'shoes', 'waist', 'amulet', 'wrist', 'ring', 'support', 'magic_ston', 'earring', 'set_item_info']
 
 # 착용가능 아바타
-AVATAR_LIST = ['headgear', 'hair', 'face', 'jacket', 'pants', 'shoes', 'breast', 'waist', 'skin', 'aurora', 'weapon']
+AVATAR_LIST = ['total_id', 'headgear', 'hair', 'face', 'jacket', 'pants', 'shoes', 'breast', 'waist', 'skin', 'aurora', 'weapon']
 
 # 플래티넘 엠블렘 착용 가능 부위
 PLATINUM_AVATAR_LIST = ['jacket', 'pants']
 
 # CharacterSearch 에서 선택 가능한 변수
 CHARACTER_SEARCH_NAME = {
     'server_id': 'serverId',
@@ -72,26 +86,28 @@
     'job_name': 'jobName',
     'job_grow_name': 'jobGrowName',
     'fame': 'fame',
 }
 
 # CharacterInformation 에서 선택 가능한 변수
 CHARACTER_INFORMATION_NAME = {
+    'total_id' : 'total_id',
     'character_id': 'characterId',
     'character_name': 'characterName',
     'level': 'level',
     'job_name': 'jobName',
     'job_grow_name': 'jobGrowName',
     'adventure_name': 'adventureName',
     'guild_id': 'guildId',
     'guild_name': 'guildName'
 }
 
 # Status 에서 선택 가능한 변수
 STATUS_NAME = {
+    'total_id' : 'total_id',
     'character_id': 'characterId',
     'character_name': 'characterName',
     'level': 'level',
     'job_name': 'jobName',
     'job_grow_name': 'jobGrowName',
     'adventure_name': 'adventureName',
     'guild_id': 'guildId',
```

### Comparing `pyneople-0.3.9/src/pyneople/character.py` & `pyneople-0.4.0/src/pyneople/character.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
-character
+Neople Open API 에서 Character를 기반으로 한 정보를 다루는 모듈입니다.
 """
-
+import asyncio
 import datetime
 import urllib.parse
-from typing import Iterable, Union
-from .functions import get_request, explain_enchant
+from typing import Union
+from .functions import get_request, async_get_request, explain_enchant, NeopleOpenAPIError
 from .METADATA import SERVER_NAME_2_ID, CHARACTER_SEARCH_NAME, \
                     CHARACTER_INFORMATION_NAME, STATUS_NAME, EQUIPMENT_LIST, AVATAR_LIST, PLATINUM_AVATAR_LIST, \
-                    BASE_EQUIPMENT_NAME, EQUIPMENT_NAME, WEAPON_NAME, AVATAR_NAME, PLATINUM_AVATAR_NAME, GROWINFO_NAME
+                    BASE_EQUIPMENT_NAME, EQUIPMENT_NAME, WEAPON_NAME, AVATAR_NAME, PLATINUM_AVATAR_NAME, GROWINFO_NAME, SERVER_ID_2_TOTAL_ID
 
 __all__ = [
     "CharacterSearch",
     "CharacterInformation",
     "Timeline",
     "Status",
     "Equipments",
@@ -28,157 +28,191 @@
 
 class PyNeople():
     """
     부모 Class로 사용
     """
     def __init__(self, arg_api_key : str):
         """
-        클래스 생성 시 Neople Open API key를 입력받는다
-            Args :
-                arg_api_key(str) : Neople Open API key
+        클래스 생성 시 Neople Open API key를 입력받는다  
+            Args :  
+                arg_api_key(str) : Neople Open API key  
         """        
         self._api_key = arg_api_key
 
 class PyNeopleAttributeSetter(PyNeople):
     """
     하위 Attribute를 설정 할 수 있는 PyNeople Class 의 부모 Class
     """
-
+    default_sub_attribute_list = []
+    
     @classmethod
     def set_sub_attributes(cls, arg_new_attribute_list : list[str]):
         for new_attribute_name in arg_new_attribute_list:
             if not new_attribute_name in cls.default_sub_attribute_list:
                 raise ValueError("사용할 수 없는 attribute 입니다.")
         cls.sub_attribute_list = arg_new_attribute_list
 
+    @classmethod
+    def delete_sub_attributes(cls, arg_delete_attribute_list : list[str]):
+        for new_attribute_name in arg_delete_attribute_list:
+            if not new_attribute_name in cls.default_sub_attribute_list:
+                raise ValueError("제거 할 수 없는 attribute 입니다.")
+        cls.sub_attribute_list = [sub_attr for sub_attr in cls.default_sub_attribute_list if sub_attr not in arg_delete_attribute_list]
+
     @classmethod        
     def init_sub_attributes(cls):
         cls.sub_attribute_list = cls.default_sub_attribute_list
 
+class PyneopleCharacter(PyNeopleAttributeSetter):
+    
+    def get_data(self, arg_server_id : str, arg_character_id : str):
+        url = self.get_url(arg_server_id, arg_character_id)
+        data = asyncio.run(async_get_request(url))
+        print("처리")
+        data['total_id'] = f"{SERVER_ID_2_TOTAL_ID[arg_server_id]}{arg_character_id}"
+        return data
+    
+    def parse_data(self, arg_data : dict):
+        self.total_id = arg_data.get('total_id')
+                
 class CharacterSearch(PyNeopleAttributeSetter):
     """
     Neople Open API 02. 캐릭터 검색
     """
     default_sub_attribute_list = CHARACTER_SEARCH_NAME.keys()
     sub_attribute_list = default_sub_attribute_list
 
-    def get_data(self, arg_server_name : str, arg_character_name : str):
-        """
-        서버 이름과 캐릭터 이름을 검색하면 기본 정보를 반환
-            Args : 
-                arg_server_name(str) : 서버 이름  ex) 디레지에, diregie
-                
-                arg_character_name(str) : 캐릭터 이름 ex) 홍길동
-        """
-        
-        # 한글 서버명을 영문 서버명으로 변환, 영문 서버명은 그대로 입력, 그 외의 입력은 에러 발생
+    def get_url(self, arg_server_name : str, arg_character_name : str):
         if arg_server_name in SERVER_NAME_2_ID.keys():
             arg_server_name = SERVER_NAME_2_ID[arg_server_name]
         elif arg_server_name in SERVER_NAME_2_ID.values():
             pass
         else:
             raise ValueError("서버 이름을 확인하시오")
         self._server_id = arg_server_name
-        url = f"https://api.neople.co.kr/df/servers/{arg_server_name}/characters?characterName={urllib.parse.quote(arg_character_name)}&limit=1&apikey={self._api_key}"
-        
+        return f"https://api.neople.co.kr/df/servers/{arg_server_name}/characters?characterName={urllib.parse.quote(arg_character_name)}&limit=1&apikey={self._api_key}"
+    
+    def get_data(self, arg_server_name : str, arg_character_name : str):
+        """
+        서버 이름과 캐릭터 이름을 검색하면 기본 정보를 반환
+            Args : 
+                arg_server_name(str) : 서버 이름  ex) 디레지에, cain  
+                
+                arg_character_name(str) : 캐릭터 이름 ex) 홍길동
+        """
+        url = self.get_url(arg_server_name, arg_character_name)
         # parse_data에 매개변수로 사용 될 것을 생각해서 dict를 받을 수 있도록 정보 다듬어서 제공
         try:
-            return get_request(url).get("rows")[0]
+            data = asyncio.run(async_get_request(url)).get("rows")
+            if data:
+                return data[0]
+            else:
+                raise NeopleOpenAPIError("{'status': 404, 'code': 'DNF001', 'message': 'NOT_FOUND_CHARACTER'}")
         except IndexError:
             return dict()
 
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 속성에 저장
             Args :
-                arg_data(dict) : Neople Open API 를 통해 받은 data
+                arg_data(dict) : Neople Open API 를 통해 받은 data  
+                
                 attribute_list(iterable of str) : 원하는 하위 속성 명
         """
         # 하위 속성에 데이터 할당
         for attribute_name in CharacterSearch.sub_attribute_list:            
             setattr(self, attribute_name, arg_data.get(CHARACTER_SEARCH_NAME[attribute_name]))
 
 
-class CharacterInformation(PyNeopleAttributeSetter):
+class CharacterInformation(PyneopleCharacter):
     """
     Neople Open API 03. 캐릭터 '기본정보' 조회
     """
     default_sub_attribute_list = CHARACTER_INFORMATION_NAME.keys()
     sub_attribute_list = default_sub_attribute_list
-    def get_data(self, arg_server_id : str, arg_character_id : str):
-        """
-        영문 서버 이름과 캐릭터 ID 를 검색하면 기본 정보를 반환
-            Args : 
-                arg_server_id(str) : 영문 서버 이름  ex) diregie
-                
-                arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
-        """    
-        self._total_id = f"{arg_server_id} {arg_character_id}"
-        url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}?apikey={self._api_key}"
-        return get_request(url)
 
-    def parse_data(self, arg_data : dict):
+    def get_url(self, arg_server_id : str, arg_character_id : str):
+        return f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}?apikey={self._api_key}"
 
+    # def get_data(self, arg_server_id : str, arg_character_id : str):
+    #     """
+    #     영문 서버 이름과 캐릭터 ID 를 검색하면 기본 정보를 반환
+    #         Args : 
+    #             arg_server_id(str) : 영문 서버 이름  ex) cain  
+                
+    #             arg_character_name(str) : 캐릭터 ID ex) d018e5f7e7519e34b8ef21db0c40fd98
+    #     """    
+    #     # self._total_id = f"{arg_server_id} {arg_character_id}"
+        
+    #     url = self.get_url(arg_server_id, arg_character_id)
+    #     data = get_request(url)
+    #     data['total_id'] = f"{arg_server_id}{arg_character_id}"
+    #     return data
+
+    def parse_data(self, arg_data : dict):
+        super().parse_data()
         """
         데이터를 정리해서 하위 속성에 저장
             Args :
-                arg_data(dict) : Neople Open API 를 통해 받은 data
-                attribute_list(iterable of str) : 원하는 하위 속성 명
+                arg_data(dict) : Neople Open API 를 통해 받은 data  
+                
+                attribute_list(iterable of str) : 원하는 하위 속성 명  
         """
         # 하위 속성에 데이터 할당
         for attribute_name in CharacterInformation.sub_attribute_list:
             setattr(self, attribute_name, arg_data.get(CHARACTER_INFORMATION_NAME[attribute_name]))
 
 
 class Timeline(PyNeople):
     """
     Neople Open API 04. 캐릭터 '타임라인 정보' 조회
-    """  
-    def get_data(self, 
+    """
+    def get_data(self,  
                  arg_server_id : str, 
                  arg_character_id : str, 
                  arg_end_date : str, 
                  arg_last_end_date : str = "2017-09-21 00:00", 
                  arg_last_end_data : Union[dict, None] = None, 
                  arg_limit : int = 100, 
                  arg_code : Union[int, str] = "",
                  arg_print_log : bool = False):
         """
         서버ID와 캐릭터ID 원하는 수집시간(arg_end_date)을 입력받으면 타임라인데이터를 반환한다.
             Args :
-                arg_server_id(str) : 서버ID ex) cain
+                arg_server_id(str) : 서버ID ex) cain  
                 
-                arg_character_id(str) : 캐릭터ID ex) 80d9189c86147ab9a7b8c1481be85d95
+                arg_character_id(str) : 캐릭터ID ex) d018e5f7e7519e34b8ef21db0c40fd98
                 
-                arg_end_date(str) : 이 시간까지 수집을 한다 ex) 2023-03-03 15:57
+                arg_end_date(str) : 이 시간까지 수집을 한다 ex) 2023-03-03 15:57  
                 
-                arg_last_end_date(str) : 이 시간부터 수집을 한다 ex) 2018-03-03 15:57
+                arg_last_end_date(str) : 이 시간부터 수집을 한다 ex) 2018-03-03 15:57  
                 
-                arg_last_end_data(dict) : 지금까지 수집한 해당 캐릭터의 마지막 타임라인 데이터
+                arg_last_end_data(dict) : 지금까지 수집한 해당 캐릭터의 마지막 타임라인 데이터  
                 
-                arg_limit(int) : 한번 request할 때 수집 할 타임라인 데이터의 개수
+                arg_limit(int) : 한번 request할 때 수집 할 타임라인 데이터의 개수  
                 
-                arg_code(int) : 수집하고 싶은 타임라인 코드 ex)201, 202 참조) https://developers.neople.co.kr/contents/guide/pages/all 
+                arg_code(int) : 수집하고 싶은 타임라인 코드 ex)201, 202 참조) https://developers.neople.co.kr/contents/guide/pages/all  
                 
-                arg_print_log(boolean) : 데이터 수집의 과정의 print 여부
+                arg_print_log(boolean) : 데이터 수집의 과정의 print 여부  
         """
         self._total_id = f"{arg_server_id} {arg_character_id}"
         timeline = []
         
         end_date = datetime.datetime.strptime(arg_end_date, '%Y-%m-%d %H:%M')
         start_date = end_date - datetime.timedelta(days=90)
         if start_date < datetime.datetime.strptime(arg_last_end_date, '%Y-%m-%d %H:%M'):
             start_date = datetime.datetime.strptime(arg_last_end_date, '%Y-%m-%d %H:%M')
         next = ""
         while start_date < end_date:
             stop = False
             url = f"""https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/timeline?limit={arg_limit}&code={arg_code}&startDate={start_date.strftime('%Y-%m-%d %H:%M')}&endDate={end_date.strftime('%Y-%m-%d %H:%M')}&next={next}&apikey={self._api_key}"""
             if arg_print_log:
                 print(f"서버 = {arg_server_id}, 캐릭터 = {arg_character_id} 시작 = {start_date.strftime('%Y-%m-%d %H:%M')}, 끝 = {end_date.strftime('%Y-%m-%d %H:%M')}")
-            data = get_request(url)
+            data = asyncio.run(async_get_request(url))
+            # data = get_request(url)
             next = data['timeline']['next']
 
             # 데이터가 있다면
             if data['timeline']['rows']:                 
                 for log in data['timeline']['rows']:
                     if log == arg_last_end_data:
                         stop = True
@@ -203,38 +237,49 @@
                 start_date = end_date - datetime.timedelta(days=90)
                 if start_date < datetime.datetime.strptime(arg_last_end_date, '%Y-%m-%d %H:%M'):
                     start_date = datetime.datetime.strptime(arg_last_end_date, '%Y-%m-%d %H:%M')
                 next = ""    
                 continue
         return {'timeline' : timeline} 
 
-class Status(PyNeopleAttributeSetter):
+class Status(PyneopleCharacter):
     """
-    Neople Open API 05. 캐릭터 '능력치 정보' 조회
+    Neople Open API 05. 캐릭터 '능력치 정보' 조회  
     """    
     default_sub_attribute_list = STATUS_NAME.keys()
     sub_attribute_list = default_sub_attribute_list    
-    
-    def get_data(self, arg_server_id : str, arg_character_id : str):
+
+    def get_url(self, arg_server_id : str, arg_character_id : str):
         """
         캐릭터의 모험단명부터 명성 등 정보를 반환한다
             Args:
-                arg_server_id(str) :  서버 ID
+                arg_server_id(str) :  서버 ID  
                 
-                arg_character_id(str) : 캐릭터 ID
+                arg_character_id(str) : 캐릭터 ID  
         """
-        self._total_id = f"{arg_server_id} {arg_character_id}"
-        url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/status?apikey={self._api_key}'
-        return get_request(url)
+        return f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/status?apikey={self._api_key}' 
+
+    # def get_data(self, arg_server_id : str, arg_character_id : str):
+    #     """
+    #     캐릭터의 모험단명부터 명성 등 정보를 반환한다
+    #         Args:
+    #             arg_server_id(str) :  서버 ID  
+                
+    #             arg_character_id(str) : 캐릭터 ID  
+    #     """
+    #     self._total_id = f"{arg_server_id} {arg_character_id}"
+    #     url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/status?apikey={self._api_key}'
+    #     return get_request(url)
 
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
+
                 attribute_list(iterable of str) : 원하는 하위 속성 명
         """
         
         # 모험단, 길드 버프 정리
         if arg_data.get('buff'):
             for buff in arg_data['buff']:
                 if buff.get('name') == '모험단 버프':
@@ -280,15 +325,15 @@
                         if option.get('transfer'):
                             setattr(self, 'transfer', i+1)
             else:   
                 setattr(self, sub_attribute_name, arg_grow_info_dict.get(GROWINFO_NAME[sub_attribute_name])) 
 
 class BaseEquipment(PyNeopleAttributeSetter):
     """
-    Equipments를 위해 사용되는 Class
+    Equipments를 위해 사용되는 Class  
     가장 기초적인 장비 정보를 담으며 다른 장비에 부모클래스로 이용된다.
     """    
     default_sub_attribute_list = BASE_EQUIPMENT_NAME.keys()
     sub_attribute_list = default_sub_attribute_list
     
     def __init__(self):
         for sub_attribute in BaseEquipment.sub_attribute_list:
@@ -300,15 +345,15 @@
             if sub_attribute == 'enchant':
                 setattr(self, sub_attribute, explain_enchant(arg_equipment_dict.get('enchant')))
             else:    
                 setattr(self, sub_attribute, arg_equipment_dict.get(BASE_EQUIPMENT_NAME[sub_attribute]))
 
 class Equipment(BaseEquipment):
     """
-    Equipments를 위해 사용되는 Class
+    Equipments를 위해 사용되는 Class  
     """ 
     default_sub_attribute_list = EQUIPMENT_NAME.keys()
     sub_attribute_list = default_sub_attribute_list
     def __init__(self):
         super().__init__()
         for sub_attribute in Equipment.sub_attribute_list:
             if sub_attribute == 'grow_info':
@@ -389,48 +434,54 @@
                 pass    
 
     def get_equipment_data(self, arg_equipment_dict):
         super().get_equipment_data(arg_equipment_dict)
         for sub_attribute in Weapon.sub_attribute_list:
             getattr(self, sub_attribute).get_info_data(arg_equipment_dict.get(WEAPON_NAME[sub_attribute], dict()))
             
-class Equipments(PyNeopleAttributeSetter):
+class Equipments(PyneopleCharacter):
     """
     Neople Open API 06. 캐릭터 '장착 장비' 조회
     """    
     default_sub_attribute_list = EQUIPMENT_LIST
     sub_attribute_list = default_sub_attribute_list
-    
-    def get_data(self, arg_server_id : str, arg_character_id : str):
-        """
-        영문 서버 이름과 캐릭터 ID 를 검색하면 장착 장비 정보를 반환
-            Args : 
-                arg_server_id(str) : 영문 서버 이름  ex) diregie
-                
-                arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
-        """        
-        self._total_id = f"{arg_server_id} {arg_character_id}"
+
+    def get_url(self, arg_server_id : str, arg_character_id : str):
         url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/equipment?apikey={self._api_key}'
-        return get_request(url)
+        return url
+
+    # def get_data(self, arg_server_id : str, arg_character_id : str):
+    #     """
+    #     영문 서버 이름과 캐릭터 ID 를 검색하면 장착 장비 정보를 반환
+    #         Args : 
+    #             arg_server_id(str) : 영문 서버 이름  ex) cain  
+                
+    #             arg_character_name(str) : 캐릭터 ID ex) d018e5f7e7519e34b8ef21db0c40fd98
+    #     """        
+    #     self._total_id = f"{arg_server_id} {arg_character_id}"
+    #     url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/equipment?apikey={self._api_key}'
+    #     return get_request(url)
     
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
         """
         # 하위 속성 생성
-        
+        self.total_id = arg_data.get("total_id")
         for equipment in Equipments.sub_attribute_list:
             if equipment == 'weapon':
                 setattr(self, equipment, Weapon())
             elif equipment == 'title':
                 setattr(self, equipment, BaseEquipment())
             elif equipment == 'set_item_info':
                 setattr(self, equipment, None)
+            elif equipment == 'total_id':
+                setattr(self, equipment, None)
             else:
                 setattr(self, equipment, Equipment())
                 
         # 장착 장비 정보 할당        
         for equipment in arg_data.get('equipment', list()):
             if equipment['slotId'].lower() in Equipments.sub_attribute_list:
                 getattr(self, equipment['slotId'].lower()).get_equipment_data(equipment)
@@ -500,100 +551,110 @@
             elif sub_attribute == "platinum_emblem":
                 for emblem in arg_avatar_dict.get(PLATINUM_AVATAR_NAME[sub_attribute], dict()):
                     if emblem.get('slotColor') == '플래티넘':
                         setattr(self, sub_attribute, emblem.get('itemName'))
             else:    
                 setattr(self, sub_attribute, arg_avatar_dict.get(AVATAR_NAME[sub_attribute]))
 
-class Avatars(PyNeopleAttributeSetter):
+class Avatars(PyneopleCharacter):
     """
     Neople Open API 07. 캐릭터 '장착 아바타' 조회
     """       
     default_sub_attribute_list = AVATAR_LIST
     sub_attribute_list = default_sub_attribute_list
 
-    def get_data(self, arg_server_id: str, arg_character_id : str):    
-        """
-        영문 서버 이름과 캐릭터 ID 를 검색하면 장착 아바타 정보를 반환
-            Args : 
-                arg_server_id(str) : 영문 서버 이름  ex) diregie
-                
-                arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
-        """        
-        self._total_id = f"{arg_server_id} {arg_character_id}"
-        url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/avatar?apikey={self._api_key}'
-        return get_request(url)
+    def get_url(self, arg_server_id: str, arg_character_id : str):    
+        return f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/avatar?apikey={self._api_key}' 
+
+    # def get_data(self, arg_server_id: str, arg_character_id : str):    
+    #     """
+    #     영문 서버 이름과 캐릭터 ID 를 검색하면 장착 아바타 정보를 반환
+    #         Args : 
+    #             arg_server_id(str) : 영문 서버 이름  ex) cain
+                
+    #             arg_character_name(str) : 캐릭터 ID ex) d018e5f7e7519e34b8ef21db0c40fd98
+    #     """
+    #     self._total_id = f"{arg_server_id} {arg_character_id}"
+    #     url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/avatar?apikey={self._api_key}'
+    #     return get_request(url)
 
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
         """        
+        self.total_id = arg_data.get("total_id")
         # 하위 속성 생성
         for avatar in Avatars.sub_attribute_list:
             if avatar in PLATINUM_AVATAR_LIST:
                 setattr(self, avatar, PlatinumAvatar())    
             else:
                 setattr(self, avatar, Avatar())
         
         # 하위 속성에 데이터 할당
         for avatar in arg_data.get('avatar', list()):
             if avatar["slotId"].lower() in Avatars.sub_attribute_list:
                 getattr(self, f'{avatar["slotId"].lower()}').get_avatar_data(avatar)
 
 
-class Creature(PyNeople):
+class Creature(PyneopleCharacter):
     """
     Neople Open API 08. 캐릭터 '장착 크리쳐' 조회
     """
-        
-    def get_data(self, arg_server_id : str, arg_character_id : str):
-        """
-        영문 서버 이름과 캐릭터 ID 를 검색하면 장착 크리쳐 정보를 반환
-            Args : 
-                arg_server_id(str) : 영문 서버 이름  ex) diregie
-                
-                arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
-        """
-        self._total_id = f"{arg_server_id} {arg_character_id}"
-        url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/creature?apikey={self._api_key}"
-        return get_request(url)
+    def get_url(self, arg_server_id : str, arg_character_id : str):
+        return f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/creature?apikey={self._api_key}"
+
+    # def get_data(self, arg_server_id : str, arg_character_id : str):
+    #     """
+    #     영문 서버 이름과 캐릭터 ID 를 검색하면 장착 크리쳐 정보를 반환
+    #         Args : 
+    #             arg_server_id(str) : 영문 서버 이름  ex) cain
+                
+    #             arg_character_name(str) : 캐릭터 ID ex) d018e5f7e7519e34b8ef21db0c40fd98
+    #     """
+    #     self._total_id = f"{arg_server_id} {arg_character_id}"
+    #     url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/creature?apikey={self._api_key}"
+    #     return get_request(url)
     
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
-        """        
+        """
+        self.total_id = arg_data.get("total_id")
         self.creature = arg_data.get('creature', dict()).get('itemName')
         
-class Flag(PyNeople):
+class Flag(PyneopleCharacter):
     """
     Neople Open API 09. 캐릭터 '장착 휘장' 조회
     """
-    
-    def get_data(self, arg_server_id : str, arg_character_id : str):
-        """
-        영문 서버 이름과 캐릭터 ID 를 검색하면 장착 휘장 정보를 반환
-            Args : 
-                arg_server_id(str) : 영문 서버 이름  ex) diregie
-                
-                arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
-        """        
-        self._total_id = f"{arg_server_id} {arg_character_id}"
-        url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/flag?apikey={self._api_key}"
-        return get_request(url)
+    def get_url(self, arg_server_id : str, arg_character_id : str):
+        return f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/flag?apikey={self._api_key}"
+
+    # def get_data(self, arg_server_id : str, arg_character_id : str):
+    #     """
+    #     영문 서버 이름과 캐릭터 ID 를 검색하면 장착 휘장 정보를 반환
+    #         Args : 
+    #             arg_server_id(str) : 영문 서버 이름  ex) cain
+                
+    #             arg_character_name(str) : 캐릭터 ID ex) d018e5f7e7519e34b8ef21db0c40fd98
+    #     """        
+    #     self._total_id = f"{arg_server_id} {arg_character_id}"
+    #     url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/flag?apikey={self._api_key}"
+    #     return get_request(url)
     
     def parse_data(self, arg_data):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
         """        
+        self.total_id = arg_data.get("total_id")
         self.gem_1 = None       # 젬1 레어도
         self.gem_2 = None       # 젬2 레어도
         self.gem_3 = None       # 젬3 레어도
         self.gem_4 = None       # 젬4 레어도
         self.item_rarity = arg_data.get('flag', dict()).get('itemRarity')   # 휘장 레어도
         self.reinforce = arg_data.get('flag', dict()).get('reinforce')      # 휘장 강화 수치
         for i, gem in enumerate(arg_data.get('flag', dict()).get('gems', list())):
@@ -605,110 +666,119 @@
     """
 
     def __init__(self):
         self.item_name = None
         self.rune_1 = None
         self.rune_2 = None
         self.rune_3 = None   
+    
     def get_talisman_data(self, arg_talisman_data):
         self.item_name = arg_talisman_data.get('talisman', dict()).get('itemName')
         for i, rune in enumerate(arg_talisman_data.get('runes', list())):
             setattr(self, f'rune_{i+1}', rune.get('itemName'))        
 
-class Talismans(PyNeople):
+class Talismans(PyneopleCharacter):
     """
     Neople Open API 10. 캐릭터 '장착 탈리스만' 조회
     """ 
 
-    def get_data(self, arg_server_id : str, arg_character_id : str):
-        """
-        영문 서버 이름과 캐릭터 ID 를 검색하면 장착 탈리스만 정보를 반환
-            Args : 
-                arg_server_id(str) : 영문 서버 이름  ex) diregie
-                
-                arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
-        """                
-        self._total_id = f"{arg_server_id} {arg_character_id}"
-        url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/talisman?apikey={self._api_key}"         
-        return get_request(url)
+    def get_url(self, arg_server_id : str, arg_character_id : str):
+        return f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/talisman?apikey={self._api_key}"
+
+    # def get_data(self, arg_server_id : str, arg_character_id : str):
+    #     """
+    #     영문 서버 이름과 캐릭터 ID 를 검색하면 장착 탈리스만 정보를 반환
+    #         Args : 
+    #             arg_server_id(str) : 영문 서버 이름  ex) cain
+                
+    #             arg_character_name(str) : 캐릭터 ID ex) d018e5f7e7519e34b8ef21db0c40fd98
+    #     """                
+    #     self._total_id = f"{arg_server_id} {arg_character_id}"
+    #     url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/talisman?apikey={self._api_key}"         
+    #     return get_request(url)
     
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
         """        
+        self.total_id = arg_data.get("total_id")
         for i, talisman in enumerate(arg_data.get("talismans", list())):
             setattr(self, f"talisman_{i+1}", Talisman())
             getattr(self, f"talisman_{i+1}").get_talisman_data(talisman)        
 
 
-class EquipmentTrait(PyNeople):
+class EquipmentTrait(PyneopleCharacter):
     """
     Neople Open API 11. 캐릭터 '장비 특성' 조회
     """ 
 
-    def get_data(self, arg_server_id : str, arg_character_id : str):
-        """
-        영문 서버 이름과 캐릭터 ID 를 검색하면 장비 특성 정보를 반환
-            Args : 
-                arg_server_id(str) : 영문 서버 이름  ex) diregie
-                
-                arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
-        """                
-        self._total_id = f"{arg_server_id} {arg_character_id}"
-        url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/equipment-trait?apikey={self._api_key}"
-        return get_request(url)
+    def get_url(self, arg_server_id : str, arg_character_id : str):
+        return f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/equipment-trait?apikey={self._api_key}" 
+
+    # def get_data(self, arg_server_id : str, arg_character_id : str):
+    #     """
+    #     영문 서버 이름과 캐릭터 ID 를 검색하면 장비 특성 정보를 반환
+    #         Args : 
+    #             arg_server_id(str) : 영문 서버 이름  ex) cain
+                
+    #             arg_character_name(str) : 캐릭터 ID ex) d018e5f7e7519e34b8ef21db0c40fd98
+    #     """                
+    #     self._total_id = f"{arg_server_id} {arg_character_id}"
+    #     url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/equipment-trait?apikey={self._api_key}"
+    #     return get_request(url)
     
     def parse_data(self, arg_data : dict):
         """
-        데이터를 정리해서 하위 attribute에 저장
-        강력한 일격과 명상의 레벨만 확인
+        데이터를 정리해서 하위 attribute에 저장 강력한 일격과 명상의 레벨만 확인
             Args :
-                arg_data(dict) : Neople Open API 를 통해 받은 data
+                arg_data(dict) : Neople Open API 를 통해 받은 data  
         """
-
+        self.total_id = arg_data.get("total_id")
         self.total_point = arg_data.get("equipmentTrait", dict()).get("total", dict()).get("point")
         self.category_name = arg_data.get("equipmentTrait", dict()).get("category", dict()).get("name")
         self.strong_hit_level = 0
         self.meditation_level = 0
         option_list = arg_data.get("equipmentTrait", dict()).get("options", list())
         option_list = list(filter(lambda x : x.get("name") in ["[강력한 일격]", "[명상]"], option_list))
         for option in option_list:
             if option.get("name") == "[강력한 일격]":
                 self.strong_hit_level = option.get("level")
             else:
                 self.meditation_level = option.get("level")
 
 
-class SkillStyle(PyNeople):
+class SkillStyle(PyneopleCharacter):
     """
     Neople Open API 12. 캐릭터 '스킬 스타일' 조회
     """ 
 
-    def get_data(self, arg_server_id : str, arg_character_id : str):
-        """
-        영문 서버 이름과 캐릭터 ID 를 검색하면 스킬 스타일 정보를 반환
-            Args : 
-                arg_server_id(str) : 영문 서버 이름  ex) diregie
-                
-                arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
-        """                
-        self._total_id = f"{arg_server_id} {arg_character_id}"
-        url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/style?apikey={self._api_key}"
-        return get_request(url)
+    def get_url(self, arg_server_id : str, arg_character_id : str):
+        return f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/style?apikey={self._api_key}" 
+
+    # def get_data(self, arg_server_id : str, arg_character_id : str):
+    #     """
+    #     영문 서버 이름과 캐릭터 ID 를 검색하면 스킬 스타일 정보를 반환
+    #         Args : 
+    #             arg_server_id(str) : 영문 서버 이름  ex) cain
+                
+    #             arg_character_name(str) : 캐릭터 ID ex) d018e5f7e7519e34b8ef21db0c40fd98
+    #     """                
+    #     self._total_id = f"{arg_server_id} {arg_character_id}"
+    #     url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/style?apikey={self._api_key}"
+    #     return get_request(url)
 
     def parse_data(self, arg_data : dict):
         """
-        데이터를 정리해서 하위 attribute에 저장
-        스킬 코드만 구현 완료 나머지 추후 개발
+        데이터를 정리해서 하위 attribute에 저장 스킬 코드만 구현 완료 나머지 추후 개발
             Args :
-                arg_data(dict) : Neople Open API 를 통해 받은 data
+                arg_data(dict) : Neople Open API 를 통해 받은 data  
         """        
-
+        self.total_id = arg_data.get("total_id")
         self.skill_code = arg_data.get("skill", dict()).get("hash")
 
 class BuffAvatar():
     """
     Buff를 위해 사용되는 Class
     """
     def __init__(self):
@@ -744,48 +814,57 @@
     Neople Open API 15. 캐릭터 "버프 스킬 강화 장착 크리쳐" 조회
     """
          
     def get_data(self, arg_server_id : str, arg_character_id : str):
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 버프 강화(장비, 아바타, 크리쳐) 정보를 반환
             Args : 
-                arg_server_id(str) : 영문 서버 이름  ex) diregie
+                arg_server_id(str) : 영문 서버 이름  ex) cain
                 
-                arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
+                arg_character_name(str) : 캐릭터 ID ex) d018e5f7e7519e34b8ef21db0c40fd98
         """   
-        self._total_id = f"{arg_server_id} {arg_character_id}"
+        # self._total_id = f"{arg_server_id} {arg_character_id}"
         buff_info_dict = {}     
-        buff_equipment_data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/equipment?apikey={self._api_key}")
-        buff_avatar_data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/avatar?apikey={self._api_key}")
-        buff_creature_data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/creature?apikey={self._api_key}")
+        
+        buff_equipment_data = asyncio.run(async_get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/equipment?apikey={self._api_key}"))
+        buff_avatar_data = asyncio.run(async_get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/avatar?apikey={self._api_key}"))
+        buff_creature_data = asyncio.run(async_get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/creature?apikey={self._api_key}"))
+        # buff_avatar_data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/avatar?apikey={self._api_key}")
+        # buff_creature_data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/creature?apikey={self._api_key}")
         buff_info_dict["equipment"] = buff_equipment_data
         buff_info_dict["avatar"] = buff_avatar_data
         buff_info_dict["creature"] = buff_creature_data
+        buff_info_dict['total_id'] = f"{SERVER_ID_2_TOTAL_ID[arg_server_id]}{arg_character_id}"
         return buff_info_dict
 
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
         """         
         # 하위 속성 생성
+        self.total_id = arg_data.get('total_id')
         self.buff_level = None
         self.buff_desc = None
         for equipment in EQUIPMENT_LIST:
-            setattr(self, f"self.buff_equipment_{equipment}", None)
+            if equipment == 'total_id':
+                continue
+            else:
+                setattr(self, f"equipment_{equipment}", None)
         for avatar in list(set(AVATAR_LIST) - set(PLATINUM_AVATAR_LIST)):
-            setattr(self, f"self.buff_avatar_{avatar}", BuffAvatar())
+            setattr(self, f"avatar_{avatar}", BuffAvatar())
         for avatar in PLATINUM_AVATAR_LIST:
-            setattr(self, f"self.buff_avatar_{avatar}", BuffPlatimun())
-        self.buff_creature = None  
+            # print(avatar)
+            setattr(self, f"avatar_{avatar}", BuffPlatimun())
         
-        arg_data["equipment"] = arg_buff_equipment_data
-        arg_data["avatar"] = arg_buff_avatar_data
-        arg_data["creature"] = arg_buff_creature_data
+        self.buff_creature = None  
+        arg_buff_equipment_data = arg_data["equipment"]
+        arg_buff_avatar_data = arg_data["avatar"]
+        arg_buff_creature_data = arg_data["creature"]
 
         if arg_buff_equipment_data.get("skill", dict()).get('buff'):
             arg_buff_equipment_data = arg_buff_equipment_data.get("skill", dict()).get('buff')
             # 버프 강화 장비
             if arg_buff_equipment_data.get("equipment"):
                 for buff_equipment in arg_buff_equipment_data.get("equipment"):
                     setattr(self, f'equipment_{buff_equipment.get("slotId").lower()}', buff_equipment.get('itemName'))
@@ -832,18 +911,25 @@
                   arg_is_buff : bool = "", 
                   arg_server_id : str = "all",
                   arg_limit : int = 200):
         """
         해당 명성 구간의 캐릭터 정보를 원소로 가지는 list를 반환함
             Args : 
                 arg_min_fame(int) : 명성 구간 최소값(최대 명성과의 차이가 2000이상이면 최대명성 - 2000 으로 입력됨)
+                
                 arg_max_fame(int) : 명성 구간 최대값
+                
                 arg_job_id(str) : 캐릭터 직업 고유 코드
+                
                 arg_job_grow_id(str) : 캐릭터 전직 직업 고유 코드(jobId 필요)
+                
                 arg_is_all_job_grow(bool) : jobGrowId 입력 시 연계되는 전체 전직 포함 조회 ex) 검성 -> 웨펀마스터, 검성, 검신, 眞웨펀마스터
+                
                 arg_is_buff(bool) : 버퍼만 조회(true), 딜러만 조회(false), 전체 조회(미 입력)	
+                
                 arg_server_id(str) : 서버 아이디
+                
                 arg_limit(int) : 반환 Row 수
         """
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters-fame?minFame={arg_min_fame}&maxFame={arg_max_fame}&jobId={arg_job_id}&jobGrowId={arg_job_grow_id}&isAllJobGrow={arg_is_all_job_grow}&isBuff={arg_is_buff}&limit={arg_limit}&apikey={self._api_key}"
-        return get_request(url)
+        return asyncio.run(async_get_request(url))
```

### Comparing `pyneople-0.3.9/src/pyneople/database_connecter.py` & `pyneople-0.4.0/src/pyneople/database_connecter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-database connecter
+데이터베이스와 상호작용하는 모듈입니다.
 """
 
 from .functions import get_request, ServerMaintenanceError, attr_flatten
 from .character import CharacterFame, CharacterSearch, Timeline
 from multiprocessing import Process, Queue, Value
 from pymongo import MongoClient
 from typing import Callable
@@ -20,23 +20,30 @@
 ]
 
 def store_fame_data_to_mongodb(
         arg_mongo_client_instance : MongoClient,
         arg_database_name : str,
         arg_collection_name : str,
         arg_api_key_list : list[str],
-        arg_max_fame : int = 100000):
+        arg_max_fame : int = 100000,
+        arg_min_fame : int = 0):
     """
     최근 90일 이내 접속한 110 레벨 이상 캐릭터 전체를 MongoDB에 저장하는 함수
         Args :
-            arg_mongo_client_instance(MongoClient) : 저장하려는 MongoDB의 pymongo MongoClient 객체 
-            arg_database_name(str) : 저장하려는 MongoDB의 database name
-            arg_collection_name(str) : 저장하려는 MongoDB의 collection name
-            arg_api_key_list(list[str]) : Neople Open API 에서 발급된 api key를 원소로 가지는 list
+            arg_mongo_client_instance(MongoClient) : 저장하려는 MongoDB의 pymongo MongoClient 객체  
+            
+            arg_database_name(str) : 저장하려는 MongoDB의 database name  
+            
+            arg_collection_name(str) : 저장하려는 MongoDB의 collection name  
+            
+            arg_api_key_list(list[str]) : Neople Open API 에서 발급된 api key를 원소로 가지는 list  
+            
             arg_max_fame(int) : 조회 하려는 최대 명성
+
+            arg_min_fame(int) : 조회 하려는 최소 명성  
     """
     def task_get_request(character_fame_instance, args_queue, data_queue, completed_tasks_count, tasks_to_be_completed_count):
         """
         args_queue에서 인자 정보를 get하고 데이터를 Neople Open API 에서 가져와서 data_queue에 저장
         """
         while completed_tasks_count.value != tasks_to_be_completed_count:
             if not args_queue.empty():
@@ -76,24 +83,24 @@
                     print(f"max = {max_fame}, min = {min_fame}, 직업 = {character_search_instance.job_grow_name}", end="\r")
                     
                     # 모든 캐릭터의 명성이 같다면
                     if max_fame == min_fame:
                         # 최대명성을 1만 내림
                         min_fame = max_fame - 1
 
-                    # 명성이 최소값이 0보다 작거나 같으면
-                    if min_fame <= 0:
+                    # 명성이 최소값이 arg_min_fame보다 작거나 같으면
+                    if min_fame <= arg_min_fame:
                         # 해당 직업 완료
                         completed_tasks_count.value += 1
                         print(f"완료된 직업 개수 {completed_tasks_count.value}", end="\r")
                         continue       
                     
                     # 인자정보 args queue에 저장
                     args_dict = {
-                        'arg_min_fame' : 0,
+                        'arg_min_fame' : arg_min_fame,
                         'arg_max_fame' : min_fame,
                         'arg_job_id' : character_search_instance.job_id,
                         'arg_job_grow_id' : character_search_instance.job_grow_id,
                         'arg_is_all_job_grow' : True
                     }
                     args_queue.put(args_dict)
                 # 데이터가 없다면
@@ -129,15 +136,15 @@
     for process in processes:
         process.start()
     
     # arg_queue에 인자 정보 투입
     for job_id , job_grow_id in job_id_list:
         max_fame = arg_max_fame
         args_dict = {
-            'arg_min_fame' : 0,
+            'arg_min_fame' : arg_min_fame,
             'arg_max_fame' : max_fame,
             'arg_job_id' : job_id,
             'arg_job_grow_id' : job_grow_id,
             'arg_is_all_job_grow' : True
         }
         args_queue.put(args_dict)
     
@@ -151,58 +158,66 @@
         arg_collection_name : str,
         arg_api_key_list : list[str],
         arg_pyneople_character_class_list : list,
         arg_total_id_list : list):
     """
     character data를 MongoDB에 저장하는 함수
         Args :
-            arg_mongo_client_instance(MongoClient) : 저장하려는 MongoDB의 pymongo MongoClient 객체 
-            arg_database_name(str) : 저장하려는 MongoDB의 database name
-            arg_collection_name(str) : 저장하려는 MongoDB의 collection name
-            arg_api_key_list(list[str]) : Neople Open API 에서 발급된 api key를 원소로 가지는 list
-            arg_pyneople_character_class_list(list) : pyneopl.character 객체를 원소로 가지는 list
-            arg_total_id_list : "server_id character_id"로 이루어진 total_id
+            arg_mongo_client_instance(MongoClient) : 저장하려는 MongoDB의 pymongo MongoClient 객체   
+            
+            arg_database_name(str) : 저장하려는 MongoDB의 database name  
+            
+            arg_collection_name(str) : 저장하려는 MongoDB의 collection name  
+            
+            arg_api_key_list(list[str]) : Neople Open API 에서 발급된 api key를 원소로 가지는 list  
+            
+            arg_pyneople_character_class_list(list) : pyneopl.character 객체를 원소로 가지는 list  
+            
+            arg_total_id_list : "server_id character_id"로 이루어진 total_id  
     """    
-    def task_get_request(pyneople_instance_list, args_queue, data_queue, completed_tasks_count, tasks_to_be_completed_count, fail_queue):
+    def task_get_request(pyneople_instance_list, args_queue, data_queue, completed_tasks_count, tasks_to_be_completed_count):
         while completed_tasks_count.value != tasks_to_be_completed_count:
             if not args_queue.empty():
                 args_dict = args_queue.get()
-                completed_tasks_count.value += 1
-                print(f"{completed_tasks_count.value}/{tasks_to_be_completed_count}", end="\r")
                 try:
                     for pyneople_instance in pyneople_instance_list:
                         data = pyneople_instance.get_data(**args_dict)
                         data['total_id'] = pyneople_instance._total_id
                         data_queue.put(data)
                 except ServerMaintenanceError:
                     raise Exception("서버점검중")
                 except:
-                    fail_queue.put(args_dict)
+                    data_queue.put({"pyneople_fail" : args_dict})
 
-    def task_store_data(data_queue, mongo_collection, completed_tasks_count, tasks_to_be_completed_count):
+    def task_store_data(data_queue, mongo_collection, completed_tasks_count, tasks_to_be_completed_count, fail_queue):
         while completed_tasks_count.value != tasks_to_be_completed_count:
             if not data_queue.empty():
                 data = data_queue.get()
-                mongo_collection.insert_one(data)
+                completed_tasks_count.value += 1
+                print(f"{completed_tasks_count.value}/{tasks_to_be_completed_count}", end="\r")
+                if data.get("pyneople_fail"):
+                    fail_queue.put(data.get("pyneople_fail"))
+                else:
+                    mongo_collection.insert_one(data)
     
     mongo_database = arg_mongo_client_instance[arg_database_name]
     collection = mongo_database[arg_collection_name]    
     tasks_to_be_completed_count = len(arg_total_id_list)
     completed_tasks_count = Value("i", 0)
     data_queue = Queue()
     args_queue = Queue()
     fail_queue = Queue()
     process_list = []
     for api_key in arg_api_key_list:
         pyneople_instance_list = []
         for pyneople_character_class in arg_pyneople_character_class_list:
             pyneople_instance_list.append(pyneople_character_class(api_key))
-        process = Process(target=task_get_request, args=(pyneople_instance_list, args_queue, data_queue, completed_tasks_count, tasks_to_be_completed_count, fail_queue))
+        process = Process(target=task_get_request, args=(pyneople_instance_list, args_queue, data_queue, completed_tasks_count, tasks_to_be_completed_count))
         process_list.append(process)
-    process = Process(target=task_store_data, args=(data_queue, collection, completed_tasks_count, tasks_to_be_completed_count))
+    process = Process(target=task_store_data, args=(data_queue, collection, completed_tasks_count, tasks_to_be_completed_count, fail_queue))
     process_list.append(process)
 
     for process in process_list:
         process.start()    
 
     for total_id in arg_total_id_list:
         server_id, character_id = total_id.split()
@@ -229,58 +244,69 @@
         arg_end_time: str,
         arg_start_time: str = "2017-09-21 00:00",
         arg_code : Union[int, str] = ""):
     
     """
     timeline data를 MongoDB에 저장하는 함수
         Args :
-            arg_mongo_client_instance(MongoClient) : 저장하려는 MongoDB의 pymongo MongoClient 객체 
-            arg_database_name(str) : 저장하려는 MongoDB의 database name
-            arg_collection_name(str) : 저장하려는 MongoDB의 collection name
-            arg_api_key_list(list[str]) : Neople Open API 에서 발급된 api key를 원소로 가지는 list
-            arg_end_time(str) : 타임라인 데이터 마지막 수집 시간 ex) "2024-05-02 05:30",
-            arg_start_time(str) : 타임라인 데이터 첫 수집 시간 ex) "2024-04-25 12:00",            
-            arg_code(int) : 수집하고 싶은 타임라인 코드 ex)201, 202 참조) https://developers.neople.co.kr/contents/guide/pages/all
-            arg_total_id_list : "server_id character_id"로 이루어진 total_id
+            arg_mongo_client_instance(MongoClient) : 저장하려는 MongoDB의 pymongo MongoClient 객체  
+            
+            arg_database_name(str) : 저장하려는 MongoDB의 database name  
+            
+            arg_collection_name(str) : 저장하려는 MongoDB의 collection name  
+            
+            arg_api_key_list(list[str]) : Neople Open API 에서 발급된 api key를 원소로 가지는 list  
+            
+            arg_end_time(str) : 타임라인 데이터 마지막 수집 시간 ex) "2024-05-02 05:30",  
+            
+            arg_start_time(str) : 타임라인 데이터 첫 수집 시간 ex) "2024-04-25 12:00",              
+            
+            arg_code(int) : 수집하고 싶은 타임라인 코드 ex)201, 202 참조) https://developers.neople.co.kr/contents/guide/pages/all  
+            
+            arg_total_id_list : "server_id character_id"로 이루어진 total_id  
     """     
-    def task_get_request(pyneople_instance, args_queue, data_queue, completed_tasks_count, tasks_to_be_completed_count, fail_queue):
+    def task_get_request(pyneople_instance, args_queue, data_queue, completed_tasks_count, tasks_to_be_completed_count):
         while completed_tasks_count.value != tasks_to_be_completed_count:
             if not args_queue.empty():
                 args_dict = args_queue.get()
-                completed_tasks_count.value += 1
-                print(f"{completed_tasks_count.value}/{tasks_to_be_completed_count}", end="\r")
                 try:
                     data = pyneople_instance.get_data(**args_dict)
                     data['total_id'] = pyneople_instance._total_id
                     data_queue.put(data)
                 except ServerMaintenanceError:
                     raise Exception("서버점검중")
                 except :
-                    fail_queue.put(args_dict)
+                    data_queue.put({"pyneople_fail" : args_dict})
 
-    def task_store_data(data_queue, mongo_collection, completed_tasks_count, tasks_to_be_completed_count):
+
+    def task_store_data(data_queue, mongo_collection, completed_tasks_count, tasks_to_be_completed_count, fail_queue):
         while completed_tasks_count.value != tasks_to_be_completed_count:
             if not data_queue.empty():
                 data = data_queue.get()
-                mongo_collection.insert_one(data)
+                completed_tasks_count.value += 1
+                print(f"{completed_tasks_count.value}/{tasks_to_be_completed_count}", end="\r")
+                if data.get("pyneople_fail"):
+                    fail_queue.put(data.get("pyneople_fail"))
+                else:
+                    mongo_collection.insert_one(data)
     
     mongo_database = arg_mongo_client_instance[arg_database_name]
     collection = mongo_database[arg_collection_name]    
     tasks_to_be_completed_count = len(arg_total_id_list)
     completed_tasks_count = Value("i", 0)
     data_queue = Queue()
     args_queue = Queue()
     fail_queue = Queue()
     process_list = []
     
     for api_key in arg_api_key_list:
         pyneople_instance = Timeline(api_key)
-        process = Process(target=task_get_request, args=(pyneople_instance, args_queue, data_queue, completed_tasks_count, tasks_to_be_completed_count, fail_queue))
+        process = Process(target=task_get_request, args=(pyneople_instance, args_queue, data_queue, completed_tasks_count, tasks_to_be_completed_count))
         process_list.append(process)
-    process = Process(target=task_store_data, args=(data_queue, collection, completed_tasks_count, tasks_to_be_completed_count))
+    process = Process(target=task_store_data, args=(data_queue, collection, completed_tasks_count, tasks_to_be_completed_count, fail_queue))
     process_list.append(process)
 
     for process in process_list:
         process.start()    
     
     for total_id in arg_total_id_list:
         print(total_id)
@@ -336,17 +362,19 @@
             cursor.execute(arg_query)
             return cursor.fetchall()
 
     def create_table_query(self, arg_pyneople_instance, arg_data_types : list, arg_constraint_options : str = None):
         """
         PostgreSQLConnecter.create_table 메소드의 arg_columns 매개변수로 사용될 값을 반환하는 함수
             Args:
-                arg_pyneople_instance : pyneople instance 혹은 pyneople instance를 원소로 가지는 list
-                arg_data_type(list) : VARCHAR(32) PRIMARY KEY 같은 제약 조건을 담은 list
-                arg_constraint_options(str) : 해당 테이블의 제약조건 ex) "PRIMARY KEY(characterid, server)"
+                arg_pyneople_instance : pyneople instance 혹은 pyneople instance를 원소로 가지는 list  
+                
+                arg_data_type(list) : VARCHAR(32) PRIMARY KEY 같은 제약 조건을 담은 list  
+                
+                arg_constraint_options(str) : 해당 테이블의 제약조건 ex) "PRIMARY KEY(characterid, server)"  
         """
         colnames = []
         if isinstance(arg_pyneople_instance ,list):
             for pyneople_instance in arg_pyneople_instance:
                 colnames += attr_flatten(pyneople_instance)
         else:
             colnames = attr_flatten(arg_pyneople_instance)
@@ -362,16 +390,15 @@
         """
         table을 만드는 함수
             Args:
                 arg_table_name(str) : 생성하려는 table name
                 
                 arg_columns(list) : CREATE TABLE {table_name} (); 안에들어가는 문자열 list ex ["characterId VARCHAR(32) PRIMARY KEY", "serverId VARCHAR(32) NOT NULL"]
                 
-                arg_drop(bool) : {False : 이미 동일한 이름의 table이 있으면 에러발생(default), 
-                                True : 이미 동일한 이름의 table이 있으면 삭제하고 만든다}
+                arg_drop(bool) : {False : 이미 동일한 이름의 table이 있으면 에러발생(default), True : 이미 동일한 이름의 table이 있으면 삭제하고 만든다}
         """    
         columns_str = ', '.join(arg_columns)
         if arg_drop :
             self.execute(f"DROP TABLE IF EXISTS {arg_table_name};")
             self.execute(f"CREATE TABLE {arg_table_name} ({columns_str});")
         else :
             self.execute(f"CREATE TABLE {arg_table_name} ({columns_str});")
@@ -407,26 +434,25 @@
         )            
         table_name_list = [table_name[0].split(".")[1] for table_name in data]
         return table_name_list
 
 
     def insert_into_table(self, arg_cursor , arg_table_name : str, arg_columns : list, arg_data : list, arg_ignore_duplication : bool = True):
         """
-        table에 데이터를 삽입하는 함수
+        table에 데이터를 삽입하는 함수, 주의사항 : 해당 함수는 connectiom.commit() 을 실행하지 않음
             Args:
-                arg_cursor(cursor) : psycopg2 cursor 객체
-                arg_table_name(str) : 데이터를 삽입하려는 table name
-                arg_columns(list) : 데이터를 삽입하려는 column들의 list ex) ["characterId", "serverId", "jobName"]
-                arg_data(list) : ex [('f2baddf4a296490a4d463cb512a83789', 'anton', '총검사'),
-                                    ('87cbd3e834ae89c567a22a98bb2c9911', 'anton', '총검사')]
-                                    or
-                                    [('f2baddf4a296490a4d463cb512a83789', 'anton', '총검사')] <- data 1개여도 이런식으로 삽입
-                arg_ignore_duplication(bool) : {True : 중복되는게 있으면 해당 항목만 넘어가고 계속 저장해라, False : 중복되는게 있으면 에러를 발생시켜라}
-
-        주의사항 : 해당 함수는 connectiom.commit() 을 실행하지 않음
+                arg_cursor(cursor) : psycopg2 cursor 객체  
+                
+                arg_table_name(str) : 데이터를 삽입하려는 table name  
+                
+                arg_columns(list) : 데이터를 삽입하려는 column들의 list ex) ["characterId", "serverId", "jobName"]  
+                
+                arg_data(list) : [('f2baddf4a296490a4d463cb512a83789', 'anton', '총검사')] <- data 1개여도 이런식으로 삽입  
+                
+                arg_ignore_duplication(bool) : {True : 중복되는게 있으면 해당 항목만 넘어가고 계속 저장해라, False : 중복되는게 있으면 에러를 발생시켜라}  
         """
         insert_query = sql.SQL("INSERT INTO {} ({}) VALUES {}").format(
             sql.Identifier(arg_table_name),
             sql.SQL(', ').join(map(sql.Identifier, arg_columns)),
             sql.SQL(', ').join(map(sql.Literal, arg_data))
             )
         if arg_ignore_duplication:
@@ -439,21 +465,27 @@
                           arg_mongo_database_name : str,
                           arg_mongo_collection_name : str,
                           arg_preprocess_function : Callable, 
                           arg_batch_size : int = 100):
     """
     MomgoDB collection 에 저장된 데이터를 Postgresql로 전처리 후 batch_size씩 저장하는 함수
         Args :
-            arg_postgresql_connecter(PostgreSQLConnecter) : pyneople database connecter
-            arg_postgresql_table_name(str) :  저장하려는 PostgreSQL table name
-            arg_mongo_client(MongoClient) : pymongo 의 MongoClient 객체
-            arg_mongo_database_name(str) : MongoDB의 database name
-            arg_mongo_collection_name(str) : MongoDB의 collection name
-            arg_preprocess_function(Callable) : 전처리 함수(input으로 MongoDB의 document가 들어가며 tuple 또는 tuple로 이루어진 list를 반환해야 한다.)
-            arg_batch_size(int) : 한번에 조회, 저장하는 document 개수
+            arg_postgresql_connecter(PostgreSQLConnecter) : pyneople database connecter  
+            
+            arg_postgresql_table_name(str) :  저장하려는 PostgreSQL table name  
+            
+            arg_mongo_client(MongoClient) : pymongo 의 MongoClient 객체  
+            
+            arg_mongo_database_name(str) : MongoDB의 database name  
+            
+            arg_mongo_collection_name(str) : MongoDB의 collection name  
+            
+            arg_preprocess_function(Callable) : 전처리 함수(input으로 MongoDB의 document가 들어가며 tuple 또는 tuple로 이루어진 list를 반환해야 한다.)  
+            
+            arg_batch_size(int) : 한번에 조회, 저장하는 document 개수  
     """
     postgresql_columns = arg_postgresql_connecter.get_column_names(arg_postgresql_table_name)
     postgresql_cursor = arg_postgresql_connecter.connection.cursor()
 
     mongo_database = arg_mongo_client[arg_mongo_database_name]
     mongo_collection = mongo_database[arg_mongo_collection_name]
     
@@ -481,11 +513,8 @@
         arg_postgresql_connecter.connection.commit()
         count += arg_batch_size
         print(f"{count}/{total_data_count}", end="\r")
 
     # 연결 종료
     arg_mongo_client.close()
     postgresql_cursor.close()
-    arg_postgresql_connecter.connection.close()
-    print("done")    
-
-            
+    print("done")
```

### Comparing `pyneople-0.3.9/src/pyneople/functions.py` & `pyneople-0.4.0/src/pyneople/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
-functions
+pyneople에서 사용되는 함수와 클래스입니다.
 """
 
 import time
 import json
+import aiohttp
+import asyncio  
 import requests
-from .METADATA import JOBCLASS
-from .METADATA import SETTINGS
+from .METADATA import JOBCLASS, SETTINGS, TOTAL_ID_2_SERVER_ID
 
-__all__ = ['change_settings', 'get_request', 'jobname_equalize', 'get_job_info', 'system_maintenance', 'NeopleOpenAPIError', 'ServerMaintenanceError', 'value_flatten', 'attr_flatten']
+__all__ = ['change_settings', 'get_request', 'jobname_equalize', 'get_job_info', 'NeopleOpenAPIError', 'ServerMaintenanceError', 'value_flatten', 'attr_flatten']
 
 class NeopleOpenAPIError(Exception):
     """
     Error 핸들링을 위한 Class
     """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
@@ -54,29 +55,50 @@
         else:
             raise NeopleOpenAPIError(data.get("error"))
     elapsed_time = time.time() - start_time
     if elapsed_time < SETTINGS['request_time_sleep']:
         time.sleep(SETTINGS['request_time_sleep'] - elapsed_time)
     return data
 
+async def async_get_request(arg_url : str):
+    """
+    url 입력시 data 가져오는 함수
+        Args :
+            arg_url(str) : 원하는 url 주소
+    """
+    async with aiohttp.ClientSession(timeout = aiohttp.ClientTimeout(total=SETTINGS['request_time_out'])) as session:
+        print(f"요청{time.time()}")
+        async with session.get(arg_url) as response:
+            await asyncio.sleep(SETTINGS['request_time_sleep'])
+            data = await response.json()
+            if data.get("error"):
+                if data.get("error").get('status') == 503:
+                    raise ServerMaintenanceError
+                else:
+                    raise NeopleOpenAPIError(data.get("error"))
+            return data
+
 def _next(arg_dict : dict, arg_list : list):
     """
     get_job_info 함수를 위해 쓰이는 함수
     """
     if 'next' in arg_dict.keys():
         arg_list.append(arg_dict["jobGrowName"])
         return _next(arg_dict['next'], arg_list)
     else :
         arg_list.append(arg_dict["jobGrowName"])
         return arg_dict["jobGrowName"]
 
+def split_total_id(arg_total_id):
+    return TOTAL_ID_2_SERVER_ID[arg_total_id[:1]], arg_total_id[1:]
 
 def get_job_info(arg_api_key : str):
     """
     직업 정보를 받아오는 함수
+
     전직명(각성명)을 1차 전직명으로 통일시키는 jobname_equalize 함수에 매개변수로 사용되는 객체를 반환함
         Args :
             arg_api_key(str) : Neople Open API key
         Retruns :
             jobname_equalize 함수에 매개변수로 사용되는 객체
     """
     data = get_request(f"https://api.neople.co.kr/df/jobs?apikey={arg_api_key}")
@@ -110,34 +132,14 @@
         for job in arg_job_info[arg_job_name]:
             if arg_job_grow_name in job:
                 output = job
                 break
         output = output[0]
     return output
 
-def system_maintenance(arg_api_key: str):
-    """
-    현재 Neople Open API 서버가 점검중인지 확인하는 함수\\
-    서버가 점검중이면 TRUE를 반환한다
-        Args :
-            arg_api_key : Neople Open API key
-        Retruns : 
-            boolean
-    """
-    try:
-        data = requests.get(f"https://api.neople.co.kr/df/servers?apikey={arg_api_key}", timeout = SETTINGS['request_time_out'])
-        time.sleep(SETTINGS['request_time_sleep'])
-        data = json.loads(data.text)
-    except:
-        return False    
-    if (list(data.keys())[0] == 'error') and (data['error']['status'] == 503): 
-        return True
-    else:
-        return False
-
 def explain_enchant(arg_enchant_dict : dict):
     """
     마법부여 정보를 정리해주는 함수
         Args :
             arg_enchant_dict(dict) : 마법부여 정보 dict
     """
     if arg_enchant_dict == {} or arg_enchant_dict == None:
```

