# Comparing `tmp/myfans_client-0.0.2.tar.gz` & `tmp/myfans_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myfans_client-0.0.2.tar", max compression
+gzip compressed data, was "myfans_client-0.0.3.tar", max compression
```

## Comparing `myfans_client-0.0.2.tar` & `myfans_client-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2024-05-26 16:26:00.361578 myfans_client-0.0.2/LICENSE
--rw-r--r--   0        0        0       47 2024-05-26 16:26:00.361578 myfans_client-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-05-26 16:26:00.361578 myfans_client-0.0.2/myfans_client/__init__.py
--rw-r--r--   0        0        0     6475 2024-05-26 16:26:00.361578 myfans_client-0.0.2/myfans_client/client.py
--rw-r--r--   0        0        0       86 2024-05-26 16:26:00.361578 myfans_client-0.0.2/myfans_client/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-26 16:26:00.361578 myfans_client-0.0.2/myfans_client/models/__init__.py
--rw-r--r--   0        0        0      311 2024-05-26 16:26:00.361578 myfans_client-0.0.2/myfans_client/models/follow.py
--rw-r--r--   0        0        0     1160 2024-05-26 16:26:00.361578 myfans_client-0.0.2/myfans_client/models/user.py
--rw-r--r--   0        0        0      806 2024-05-26 16:26:16.921711 myfans_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 myfans_client-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-28 15:04:50.936416 myfans_client-0.0.3/LICENSE
+-rw-r--r--   0        0        0       47 2024-05-28 15:04:50.936416 myfans_client-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 15:04:50.936416 myfans_client-0.0.3/myfans_client/__init__.py
+-rw-r--r--   0        0        0     6494 2024-05-28 15:04:50.936416 myfans_client-0.0.3/myfans_client/client.py
+-rw-r--r--   0        0        0       86 2024-05-28 15:04:50.936416 myfans_client-0.0.3/myfans_client/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:04:50.936416 myfans_client-0.0.3/myfans_client/models/__init__.py
+-rw-r--r--   0        0        0      311 2024-05-28 15:04:50.936416 myfans_client-0.0.3/myfans_client/models/follow.py
+-rw-r--r--   0        0        0     1527 2024-05-28 15:04:50.936416 myfans_client-0.0.3/myfans_client/models/user.py
+-rw-r--r--   0        0        0      806 2024-05-28 15:05:08.448670 myfans_client-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 myfans_client-0.0.3/PKG-INFO
```

### Comparing `myfans_client-0.0.2/LICENSE` & `myfans_client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `myfans_client-0.0.2/myfans_client/client.py` & `myfans_client-0.0.3/myfans_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         """
         GET https://api.myfans.jp/api/v2/users/show_by_username?username=USERNAME
         """
         res = self._get(
             f'api/v2/users/show_by_username?username={username}',
             headers=self.header,
         )
+        print(res)
         return UserProfile(**res)
 
     def get_users(self, user_code: str) -> UserProfile:
         """
         GET https://api.myfans.jp/api/v1/users/USER_CODE
         """
         res = self._get(
```

### Comparing `myfans_client-0.0.2/myfans_client/models/user.py` & `myfans_client-0.0.3/myfans_client/models/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 from typing import Optional
 from pydantic import BaseModel
 
 
+class Plan(BaseModel):
+    id: str
+    product_name: str
+    monthly_price: int
+    status: str
+    is_limited_access: bool
+    disallow_new_subscriber: bool
+    active_discount: Optional[str] = None
+    description: str
+    posts_count: int
+    is_back_number: bool
+    flag: Optional[str] = None
+    welcome_message: str
+    plan_discounts: Optional[str] = None
+
+
 class UserProfile(BaseModel):
     about: Optional[str] = None
     active: bool
     avatar_url: str
     back_number_post_images_count: int
     back_number_post_videos_count: int
     banner_url: str
     cant_receive_message: bool
-    current_back_number_plan: Optional[str] = None
+    current_back_number_plan: Optional[Plan] = None
     followers_count: int
     followings_count: int
     has_approved_user_identification: bool
     id: str
     is_bought_back_number: bool
     is_followed: bool
     is_following: bool
```

### Comparing `myfans_client-0.0.2/pyproject.toml` & `myfans_client-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "myfans-client"
-version = "0.0.2"  # using poetry-dynamic-versioning
+version = "0.0.3"  # using poetry-dynamic-versioning
 description = ""
 authors = ["komanushi <155377273+komanushi@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/komanushi/myfans-client"
 repository = "https://github.com/komanushi/myfans-client"
 keywords = ["API"]
```

### Comparing `myfans_client-0.0.2/PKG-INFO` & `myfans_client-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfans-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Home-page: https://github.com/komanushi/myfans-client
 License: MIT
 Keywords: API
 Author: komanushi
 Author-email: 155377273+komanushi@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

