# Comparing `tmp/ds_fastapi_middleware-2024.2.0-py3-none-any.whl.zip` & `tmp/ds_fastapi_middleware-2024.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 43473 bytes, number of entries: 65
+Zip file size: 43510 bytes, number of entries: 65
 -rw-rw-rw-  2.0 fat      545 b- defN 24-May-27 20:57 ds_fastapi_middleware/__init__.py
 -rw-rw-rw-  2.0 fat       92 b- defN 24-May-27 20:57 ds_fastapi_middleware/config/__init__.py
--rw-rw-rw-  2.0 fat      329 b- defN 24-May-24 13:08 ds_fastapi_middleware/config/config.py
+-rw-rw-rw-  2.0 fat      329 b- defN 24-May-28 09:21 ds_fastapi_middleware/config/config.py
 -rw-rw-rw-  2.0 fat      175 b- defN 24-May-27 20:57 ds_fastapi_middleware/errors/__init__.py
 -rw-rw-rw-  2.0 fat      739 b- defN 24-May-27 19:01 ds_fastapi_middleware/errors/_exceptions.py
 -rw-rw-rw-  2.0 fat     5124 b- defN 24-May-27 20:58 ds_fastapi_middleware/errors/_webapp.py
 -rw-rw-rw-  2.0 fat      400 b- defN 24-May-27 20:57 ds_fastapi_middleware/middlewares/__init__.py
 -rw-rw-rw-  2.0 fat     4529 b- defN 24-May-27 20:57 ds_fastapi_middleware/middlewares/audit.py
 -rw-rw-rw-  2.0 fat     1363 b- defN 24-May-27 20:57 ds_fastapi_middleware/middlewares/ctx.py
 -rw-rw-rw-  2.0 fat     1488 b- defN 24-May-27 20:57 ds_fastapi_middleware/middlewares/timeout.py
@@ -55,13 +55,13 @@
 -rw-rw-rw-  2.0 fat      494 b- defN 24-May-27 19:01 middleware/utils/usage/write.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-23 12:54 tests/__init__.py
 -rw-rw-rw-  2.0 fat     1318 b- defN 24-May-27 20:57 tests/test_middleware_audit.py
 -rw-rw-rw-  2.0 fat      579 b- defN 24-May-27 20:57 tests/test_middleware_ctx.py
 -rw-rw-rw-  2.0 fat     1554 b- defN 24-May-27 20:57 tests/test_middleware_timeout.py
 -rw-rw-rw-  2.0 fat     1616 b- defN 24-May-27 20:57 tests/test_middleware_usage.py
 -rw-rw-rw-  2.0 fat      904 b- defN 24-May-27 20:57 tests/test_utils_log_stdout.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-May-27 21:00 ds_fastapi_middleware-2024.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2202 b- defN 24-May-27 21:00 ds_fastapi_middleware-2024.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-27 21:00 ds_fastapi_middleware-2024.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       28 b- defN 24-May-27 21:00 ds_fastapi_middleware-2024.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6002 b- defN 24-May-27 21:00 ds_fastapi_middleware-2024.2.0.dist-info/RECORD
-65 files, 98098 bytes uncompressed, 33707 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-May-28 09:23 ds_fastapi_middleware-2024.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2202 b- defN 24-May-28 09:23 ds_fastapi_middleware-2024.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 09:23 ds_fastapi_middleware-2024.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       28 b- defN 24-May-28 09:23 ds_fastapi_middleware-2024.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6002 b- defN 24-May-28 09:23 ds_fastapi_middleware-2024.3.0.dist-info/RECORD
+65 files, 98098 bytes uncompressed, 33744 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -174,23 +174,23 @@
 
 Filename: tests/test_middleware_usage.py
 Comment: 
 
 Filename: tests/test_utils_log_stdout.py
 Comment: 
 
-Filename: ds_fastapi_middleware-2024.2.0.dist-info/LICENSE
+Filename: ds_fastapi_middleware-2024.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: ds_fastapi_middleware-2024.2.0.dist-info/METADATA
+Filename: ds_fastapi_middleware-2024.3.0.dist-info/METADATA
 Comment: 
 
-Filename: ds_fastapi_middleware-2024.2.0.dist-info/WHEEL
+Filename: ds_fastapi_middleware-2024.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: ds_fastapi_middleware-2024.2.0.dist-info/top_level.txt
+Filename: ds_fastapi_middleware-2024.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ds_fastapi_middleware-2024.2.0.dist-info/RECORD
+Filename: ds_fastapi_middleware-2024.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ds_fastapi_middleware/config/config.py

```diff
@@ -1,14 +1,14 @@
 import os
 import pathlib
 import yaml
 
 
 def load_config():
-    root = pathlib.Path(__file__).parents[2]
+    root = pathlib.Path(__file__).parents[1]
     file_name = os.getenv("DS_CONFIG_FILE", "default_config.yml")
     file_path = os.path.join(root, file_name)
     with open(file_path, "r") as file:
         return yaml.safe_load(file)
 
 
 config = load_config()
```

## Comparing `ds_fastapi_middleware-2024.2.0.dist-info/LICENSE` & `ds_fastapi_middleware-2024.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ds_fastapi_middleware-2024.2.0.dist-info/METADATA` & `ds_fastapi_middleware-2024.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds-fastapi-middleware
-Version: 2024.2.0
+Version: 2024.3.0
 Summary: A FastAPI middleware project for GraspDP(w)
 Author-email: yuan1989 <yuan@grasplabs.no>, skerve <arve.skjervheim@gmail.com>
 Maintainer-email: skerve <arve.skjervheim@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Grasp labs
```

## Comparing `ds_fastapi_middleware-2024.2.0.dist-info/RECORD` & `ds_fastapi_middleware-2024.3.0.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ds_fastapi_middleware/__init__.py,sha256=JFe2l-fTktNL97fgFwE6Tkr277l6dE5gA_IXIGYnkZI,545
 ds_fastapi_middleware/config/__init__.py,sha256=OKPimsyz91JWoCg1rJ_mHcR7gwQ5tXtEy61tLRZdzR8,92
-ds_fastapi_middleware/config/config.py,sha256=8wjiSrR6D4t2i_NpmSQeV3WUbcaB--K_InpoKgVfujg,329
+ds_fastapi_middleware/config/config.py,sha256=3_iDBZh7zkfNmaAEHZmusmFc4Lv_Mkue3Ik_DfiWndY,329
 ds_fastapi_middleware/errors/__init__.py,sha256=pUaVsDtmgyFGDt6UZ9q_6O-8FjmaYP8SdxuDizwk4Nc,175
 ds_fastapi_middleware/errors/_exceptions.py,sha256=YZTwX_M9H7rzPrSkbHn7GxdjnMaFjnreD-FfYyhMYKA,739
 ds_fastapi_middleware/errors/_webapp.py,sha256=j22P3c78FTkLPCz-Z8cL8Oy80WaLwwA7ByUUtoox1wU,5124
 ds_fastapi_middleware/middlewares/__init__.py,sha256=Zvedjq4WBvEtQWUs6jZninExxLrBAIVIhmiINwnXROg,400
 ds_fastapi_middleware/middlewares/audit.py,sha256=A6M4Wak3BENG8g71H6eGK6uc5Nv0yU2I1oSE5wHrzxI,4529
 ds_fastapi_middleware/middlewares/ctx.py,sha256=7pPbG1Y5Lae6i4tGthRkuflkN0P7NABeuPh6Tjw4oE4,1363
 ds_fastapi_middleware/middlewares/timeout.py,sha256=i1uNdO7AJ-xveg5HO4HHomNGK3Oh8esAsRh5Aua6KCM,1488
@@ -54,12 +54,12 @@
 middleware/utils/usage/write.py,sha256=vnVAt5QbRFwPYfeCmuPHyWD68mvlgo_m-vT9-6oR8HM,494
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_middleware_audit.py,sha256=YtqwHG-7WVFbkOSgIHEivavdyUYlrUCuMqKWeKUwIcM,1318
 tests/test_middleware_ctx.py,sha256=WF1PvLsLIkx3kbzxYD_YoyGOHlPuB9wA1vPsow79VqA,579
 tests/test_middleware_timeout.py,sha256=jVLePzvtEGscNIRa7zgDf6V9lhPmQ_eHidNsRBu4KPA,1554
 tests/test_middleware_usage.py,sha256=8mMQy2CoF57wKi2Ok_OLfM9xsSGrP6p9aHmmRrzMpq0,1616
 tests/test_utils_log_stdout.py,sha256=lUgkDG6gKEbsOXLWKQTt84UYAZlP0drT6G-jyF6xEe4,904
-ds_fastapi_middleware-2024.2.0.dist-info/LICENSE,sha256=KxvR2F9CNeqpe0C2UWp1zlf2OfkWAjE-1C8MUUsgKCQ,1088
-ds_fastapi_middleware-2024.2.0.dist-info/METADATA,sha256=GTyzmQN4D-Z-2uILvyPgRpd-GvnO4a2G3Dbq41DKx8E,2202
-ds_fastapi_middleware-2024.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ds_fastapi_middleware-2024.2.0.dist-info/top_level.txt,sha256=FbZA1HVTVVAO4yXVSCrnxFrescmNA1q4oJvlESrKmcQ,28
-ds_fastapi_middleware-2024.2.0.dist-info/RECORD,,
+ds_fastapi_middleware-2024.3.0.dist-info/LICENSE,sha256=KxvR2F9CNeqpe0C2UWp1zlf2OfkWAjE-1C8MUUsgKCQ,1088
+ds_fastapi_middleware-2024.3.0.dist-info/METADATA,sha256=5uhdedoBDns7CGqApvJXO6JGb7zBdTwBy79nHywYtk0,2202
+ds_fastapi_middleware-2024.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ds_fastapi_middleware-2024.3.0.dist-info/top_level.txt,sha256=FbZA1HVTVVAO4yXVSCrnxFrescmNA1q4oJvlESrKmcQ,28
+ds_fastapi_middleware-2024.3.0.dist-info/RECORD,,
```

