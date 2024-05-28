# Comparing `tmp/nonebot_plugin_daily_task-0.1.4.tar.gz` & `tmp/nonebot_plugin_daily_task-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_daily_task-0.1.4.tar", last modified: Mon May 27 12:38:37 2024, max compression
+gzip compressed data, was "nonebot_plugin_daily_task-0.1.5.tar", last modified: Mon May 27 12:48:39 2024, max compression
```

## Comparing `nonebot_plugin_daily_task-0.1.4.tar` & `nonebot_plugin_daily_task-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2024-05-27 12:38:27.514226 nonebot_plugin_daily_task-0.1.4/LICENSE
--rw-r--r--   0        0        0     2418 2024-05-27 12:38:27.514226 nonebot_plugin_daily_task-0.1.4/README.md
--rw-r--r--   0        0        0    14915 2024-05-27 12:38:27.514226 nonebot_plugin_daily_task-0.1.4/nonebot_plugin_daily_task/__init__.py
--rw-r--r--   0        0        0      546 2024-05-27 12:38:27.514226 nonebot_plugin_daily_task-0.1.4/nonebot_plugin_daily_task/config.py
--rw-r--r--   0        0        0      402 2024-05-27 12:38:37.018224 nonebot_plugin_daily_task-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 nonebot_plugin_daily_task-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-27 12:48:30.798864 nonebot_plugin_daily_task-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2418 2024-05-27 12:48:30.798864 nonebot_plugin_daily_task-0.1.5/README.md
+-rw-r--r--   0        0        0    15047 2024-05-27 12:48:30.798864 nonebot_plugin_daily_task-0.1.5/nonebot_plugin_daily_task/__init__.py
+-rw-r--r--   0        0        0      546 2024-05-27 12:48:30.798864 nonebot_plugin_daily_task-0.1.5/nonebot_plugin_daily_task/config.py
+-rw-r--r--   0        0        0      402 2024-05-27 12:48:39.922917 nonebot_plugin_daily_task-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 nonebot_plugin_daily_task-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_daily_task-0.1.4/LICENSE` & `nonebot_plugin_daily_task-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_daily_task-0.1.4/README.md` & `nonebot_plugin_daily_task-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_daily_task-0.1.4/nonebot_plugin_daily_task/__init__.py` & `nonebot_plugin_daily_task-0.1.5/nonebot_plugin_daily_task/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,16 @@
     """
     # 构建帮助信息
     message = MessageSegment.text("添加任务: daily.add/a\n"
                                   "删除任务: daily.del/d\n"
                                   "完成任务: daily.finish/f\n"
                                   "修改任务: daily.modify/m\n"
                                   "查询任务: daily.query/q status/task\n"
+                                  "启用插件: daily.start/s\n"
+                                  "停用插件: daily.stop/st\n"
                                   "帮助: daily.help/h")
     await daily_help.finish(message=message)
 
 
 # daily.add -- 向数据库中添加任务
 @daily_add.handle()
 async def add_task(event: Event, args: Message = CommandArg()):
```

### Comparing `nonebot_plugin_daily_task-0.1.4/nonebot_plugin_daily_task/config.py` & `nonebot_plugin_daily_task-0.1.5/nonebot_plugin_daily_task/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_daily_task-0.1.4/PKG-INFO` & `nonebot_plugin_daily_task-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_daily_task
-Version: 0.1.4
+Version: 0.1.5
 Summary: 适用于Nonebot2的每日任务提醒插件
 Author-Email: WMGray <1466787434@qq.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD041 -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_daily_task Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_daily_task Version: 0.1.5 Summary:
 éç¨äºNonebot2çæ¯æ¥ä»»å¡æéæä»¶ Author-Email: WMGray
 <1466787434@qq.com> License: MIT Requires-Python: >=3.10 Description-Content-
 Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
 # nonebot-plugin-daily-task _â¨ NoneBot æ¯æ¥ä»»å¡æä»¶ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ nb plugin install nonebot-plugin-daily-task
```

