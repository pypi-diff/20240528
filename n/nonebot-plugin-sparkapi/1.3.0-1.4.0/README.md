# Comparing `tmp/nonebot_plugin_sparkapi-1.3.0.tar.gz` & `tmp/nonebot_plugin_sparkapi-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sparkapi-1.3.0.tar", last modified: Tue May 28 18:06:12 2024, max compression
+gzip compressed data, was "nonebot_plugin_sparkapi-1.4.0.tar", last modified: Tue May 28 21:31:28 2024, max compression
```

## Comparing `nonebot_plugin_sparkapi-1.3.0.tar` & `nonebot_plugin_sparkapi-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:12.616462 nonebot_plugin_sparkapi-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-28 18:06:12.616462 nonebot_plugin_sparkapi-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:12.612462 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/SparkApi.py
--rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:12.612462 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-28 18:06:12.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-28 18:06:12.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:06:12.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 18:06:12.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 18:06:12.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:06:12.616462 nonebot_plugin_sparkapi-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:31:28.355968 nonebot_plugin_sparkapi-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-28 21:31:24.000000 nonebot_plugin_sparkapi-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-28 21:31:28.355968 nonebot_plugin_sparkapi-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-28 21:31:24.000000 nonebot_plugin_sparkapi-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:31:28.351968 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-28 21:31:24.000000 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/ImgGenApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-28 21:31:24.000000 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/SparkApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15808 2024-05-28 21:31:24.000000 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-28 21:31:24.000000 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-28 21:31:24.000000 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-28 21:31:24.000000 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-28 21:31:24.000000 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:31:28.355968 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-28 21:31:28.000000 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-28 21:31:28.000000 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:31:28.000000 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 21:31:28.000000 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 21:31:28.000000 nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-28 21:31:24.000000 nonebot_plugin_sparkapi-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:31:28.355968 nonebot_plugin_sparkapi-1.4.0/setup.cfg
```

### Comparing `nonebot_plugin_sparkapi-1.3.0/LICENSE` & `nonebot_plugin_sparkapi-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.3.0/PKG-INFO` & `nonebot_plugin_sparkapi-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.3.0
+Version: 1.4.0
 Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,14 +27,16 @@
         
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
 Requires-Dist: websockets<13.0,>=12.0
+Requires-Dist: httpx<1.0.0,>=0.19.0
+Requires-Dist: pillow<11.0.0,>=10.0.0
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
@@ -60,20 +62,21 @@
 
 适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设等功能
 
 ### 💬 功能
 - [x] 支持AI对话
 - [x] 支持上下文关联记忆（可设置记忆文本长度）
 - [x] 用户鉴别（每个用户的历史记录独立）
-- [x] 支持用户自定义、更改、切换预设（prompt）
+- [x] 支持用户自定义、更改、切换预设（Prompt）
 - [x] 自动生成人物预设菜单、帮助列表，无需重写
 - [x] 基于pickle的历史记录持久化
 - [x] 完善的配置项（有其他需求请发issue）
+- [x] 支持AI绘图（AI Image Generation）
 - [ ] 用户权限与功能区分（超级用户、普通用户）
-- [ ] 支持图片生成（ImageGeneration）
+- [ ] PPT生成（PPT Generation）
 
 ### 📦 项目地址
 - Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
 - 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
 
 ## 💿 安装
 
@@ -134,38 +137,43 @@
 | SPARKAPI_PRIORITY | 否 | 80 | 该值越小，事件越先被触发。本插件建议设置较大的值。可选值：1~97<br>若触发本插件事件，所有插件中优先级大于此值的事件都将被阻断。<br>本插件中事件的优先级顺序：私聊阻断（=priority）< 功能（=priority+1）< 对话（=priority+2） |
 | SPARKAPI_COMMANDS__CHAT | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空：COMMAND_START = [""]） |
 | SPARKAPI_FL_NOTICE | 否 | True | 收到请求时是否提示“已收到请求” |
 | SPARKAPI_FL_SETPRESET_CLEAR | 否 | True | 切换人物预设时是否清除当前对话上下文 |
 | SPARKAPI_FL_PRIVATE_CHAT | 否 | True | 是否允许私聊使用 |
 | SPARKAPI_FL_GROUP_PUBLIC | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
 | SPARKAPI_FL_GROUP_AT | 否 | True | 群聊回复消息时是否需要@提问者 |
+| SPARKAPI_FL_IMGGEN | 否 | True | 是否启用AI绘图功能 |
 | SPARKAPI_BOT_NAME | 否 | "" | 机器人的名字 |
 
 以下配置项请查看`/.venv/Lib/nonebot_plugin_sparkapi/config.py`修改：
 1. sparkapi_commands：指令表（允许单个字符串或字符串列表）
 2. sparkapi_commands_info：指令表说明（用于生成帮助信息）
 3. sparkapi_message_blockprivate：阻断私聊时的提示信息
+4. sparkapi_message_blockimggen：阻断AI绘图时的提示信息
 
 ## 🎉 使用
 ### 指令表（默认）
 以下所有指令均可在config.py中修改，且无需重写菜单/指令生成函数
 
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | SPARKAPI_COMMAND_CHAT（若不为空） + 对话内容 | 是 | 私聊/群聊 | 与机器人进行对话 |
 | help/帮助 | 是 | 私聊/群聊 | 显示帮助信息 |
 | preset/人物预设 | 是 | 私聊/群聊 | 显示人物预设菜单和当前预设 |
-| set/切换预设 | 是 | 私聊/群聊 | 显示人物预设菜单，选择并切换 |
+| set/切换预设 | 是 | 私聊/群聊 | 显示人物预设菜单，选择人物预设并切换 |
 | set/切换预设 + 人物名 | 是 | 私聊/群聊 | 切换人物预设 |
 | create/创建预设 | 是 | 私聊/群聊 | 创建自定义的人物预设 |
 | delete/删除预设 | 是 | 私聊/群聊 | 删除自定义的人物预设 |
-| delete/删除预设 + 人物名 | 是 | 私聊/群聊 | 显示自定义人物预设菜单, 选择并删除 |
+| delete/删除预设 + 人物名 | 是 | 私聊/群聊 | 显示自定义人物预设菜单, 选择人物预设并删除 |
 | clear/清空对话 | 是 | 私聊/群聊 | 清除当前对话上下文 |
 | save/保存对话 | 是 | 私聊/群聊 | 保存当前对话记录 |
 | load/加载对话 | 是 | 私聊/群聊 | 加载上次保存的对话记录 |
+| imggen/AI绘图 + 描述 | 是 | 私聊/群聊 | AI根据描述生成图片 |
+| imggen/AI绘图 | 是 | 私聊/群聊 | 下一句给出描述，AI根据描述生成图片 |
 
 ### 人物预设
 1. 智能助手（默认）
 2. 心理咨询师
+3. 李白
 
 ### 效果图
 ![demo](https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.4.0 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -14,33 +14,35 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Requires-Python: >=3.10 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: nonebot-adapter-
 onebot<3.0.0,>=2.2.1 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3 Requires-Dist:
-websockets<13.0,>=12.0
+websockets<13.0,>=12.0 Requires-Dist: httpx<1.0.0,>=0.19.0 Requires-Dist:
+pillow<11.0.0,>=10.0.0
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                         # nonebot-plugin-sparkapi _â¨
  ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIèå¤©æºå¨äºº â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð ä»ç»
 åºäºNonebot2å¹³å°ï¼è°ç¨ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIçAIèå¤©æºå¨äººæä»¶
 éç¨äºæææ¨¡åçæ¬ï¼é»è®¤å½åææ°ï¼v3.5ï¼ï¼ï¼æ¯æä¸ä¸æå³èãäººç©é¢è®¾ç­åè½
 ### ð¬ åè½ - [x] æ¯æAIå¯¹è¯ - [x]
 æ¯æä¸ä¸æå³èè®°å¿ï¼å¯è®¾ç½®è®°å¿ææ¬é¿åº¦ï¼ - [x]
 ç¨æ·é´å«ï¼æ¯ä¸ªç¨æ·çåå²è®°å½ç¬ç«ï¼ - [x]
-æ¯æç¨æ·èªå®ä¹ãæ´æ¹ãåæ¢é¢è®¾ï¼promptï¼ - [x]
+æ¯æç¨æ·èªå®ä¹ãæ´æ¹ãåæ¢é¢è®¾ï¼Promptï¼ - [x]
 èªå¨çæäººç©é¢è®¾èåãå¸®å©åè¡¨ï¼æ ééå - [x]
 åºäºpickleçåå²è®°å½æä¹å - [x]
-å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [ ]
+å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [x] æ¯æAIç»å¾ï¼AI
+Image Generationï¼ - [ ]
 ç¨æ·æéä¸åè½åºåï¼è¶çº§ç¨æ·ãæ®éç¨æ·ï¼ - [ ]
-æ¯æå¾ççæï¼ImageGenerationï¼ ### ð¦ é¡¹ç®å°å - Githubï¼https:
-//github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
+PPTçæï¼PPT Generationï¼ ### ð¦ é¡¹ç®å°å - Githubï¼https://
+github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
 Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-sparkapi ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-sparkapi pdm pdm add
 nonebot-plugin-sparkapi poetry poetry add nonebot-plugin-sparkapi conda conda
 install nonebot-plugin-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
@@ -73,31 +75,36 @@
 æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | |
 SPARKAPI_FL_SETPRESET_CLEAR | å¦ | True |
 åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | |
 SPARKAPI_FL_PRIVATE_CHAT | å¦ | True | æ¯å¦åè®¸ç§èä½¿ç¨ | |
 SPARKAPI_FL_GROUP_PUBLIC | å¦ | False | ç¾¤èå¯ç¨å¬å±ä¼è¯
 Trueï¼ææäººå±äº«åä¸ä¼è¯
 Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | SPARKAPI_FL_GROUP_AT | å¦ | True |
-ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_BOT_NAME | å¦ | "" |
+ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_FL_IMGGEN | å¦ | True
+| æ¯å¦å¯ç¨AIç»å¾åè½ | | SPARKAPI_BOT_NAME | å¦ | "" |
 æºå¨äººçåå­ | ä»¥ä¸éç½®é¡¹è¯·æ¥ç`/.venv/Lib/
 nonebot_plugin_sparkapi/config.py`ä¿®æ¹ï¼ 1.
 sparkapi_commandsï¼æä»¤è¡¨ï¼åè®¸åä¸ªå­ç¬¦ä¸²æå­ç¬¦ä¸²åè¡¨ï¼ 2.
 sparkapi_commands_infoï¼æä»¤è¡¨è¯´æï¼ç¨äºçæå¸®å©ä¿¡æ¯ï¼ 3.
-sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
+sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ 4.
+sparkapi_message_blockimggenï¼é»æ­AIç»å¾æ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
 ### æä»¤è¡¨ï¼é»è®¤ï¼
 ä»¥ä¸æææä»¤åå¯å¨config.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
 æä»¤çæå½æ° | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:| | SPARKAPI_COMMAND_CHATï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ |
 ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help/å¸®å© | æ¯ | ç§è/ç¾¤è
 | æ¾ç¤ºå¸®å©ä¿¡æ¯ | | preset/äººç©é¢è®¾ | æ¯ | ç§è/ç¾¤è |
 æ¾ç¤ºäººç©é¢è®¾èååå½åé¢è®¾ | | set/åæ¢é¢è®¾ | æ¯ | ç§è/
-ç¾¤è | æ¾ç¤ºäººç©é¢è®¾èåï¼éæ©å¹¶åæ¢ | | set/åæ¢é¢è®¾ +
-äººç©å | æ¯ | ç§è/ç¾¤è | åæ¢äººç©é¢è®¾ | | create/åå»ºé¢è®¾ |
-æ¯ | ç§è/ç¾¤è | åå»ºèªå®ä¹çäººç©é¢è®¾ | | delete/å é¤é¢è®¾ |
-æ¯ | ç§è/ç¾¤è | å é¤èªå®ä¹çäººç©é¢è®¾ | | delete/å é¤é¢è®¾ +
-äººç©å | æ¯ | ç§è/ç¾¤è | æ¾ç¤ºèªå®ä¹äººç©é¢è®¾èå,
-éæ©å¹¶å é¤ | | clear/æ¸ç©ºå¯¹è¯ | æ¯ | ç§è/ç¾¤è |
-æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | save/ä¿å­å¯¹è¯ | æ¯ | ç§è/ç¾¤è |
-ä¿å­å½åå¯¹è¯è®°å½ | | load/å è½½å¯¹è¯ | æ¯ | ç§è/ç¾¤è |
-å è½½ä¸æ¬¡ä¿å­çå¯¹è¯è®°å½ | ### äººç©é¢è®¾ 1.
-æºè½å©æï¼é»è®¤ï¼ 2. å¿çå¨è¯¢å¸ ### ææå¾ ![demo](https://
-github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
+ç¾¤è | æ¾ç¤ºäººç©é¢è®¾èåï¼éæ©äººç©é¢è®¾å¹¶åæ¢ | | set/
+åæ¢é¢è®¾ + äººç©å | æ¯ | ç§è/ç¾¤è | åæ¢äººç©é¢è®¾ | | create/
+åå»ºé¢è®¾ | æ¯ | ç§è/ç¾¤è | åå»ºèªå®ä¹çäººç©é¢è®¾ | | delete/
+å é¤é¢è®¾ | æ¯ | ç§è/ç¾¤è | å é¤èªå®ä¹çäººç©é¢è®¾ | | delete/
+å é¤é¢è®¾ + äººç©å | æ¯ | ç§è/ç¾¤è |
+æ¾ç¤ºèªå®ä¹äººç©é¢è®¾èå, éæ©äººç©é¢è®¾å¹¶å é¤ | | clear/
+æ¸ç©ºå¯¹è¯ | æ¯ | ç§è/ç¾¤è | æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | save/
+ä¿å­å¯¹è¯ | æ¯ | ç§è/ç¾¤è | ä¿å­å½åå¯¹è¯è®°å½ | | load/
+å è½½å¯¹è¯ | æ¯ | ç§è/ç¾¤è | å è½½ä¸æ¬¡ä¿å­çå¯¹è¯è®°å½ | |
+imggen/AIç»å¾ + æè¿° | æ¯ | ç§è/ç¾¤è | AIæ ¹æ®æè¿°çæå¾ç | |
+imggen/AIç»å¾ | æ¯ | ç§è/ç¾¤è |
+ä¸ä¸å¥ç»åºæè¿°ï¼AIæ ¹æ®æè¿°çæå¾ç | ### äººç©é¢è®¾ 1.
+æºè½å©æï¼é»è®¤ï¼ 2. å¿çå¨è¯¢å¸ 3. æç½ ### ææå¾ ![demo]
+(https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

### Comparing `nonebot_plugin_sparkapi-1.3.0/README.md` & `nonebot_plugin_sparkapi-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,20 +26,21 @@
 
 适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设等功能
 
 ### 💬 功能
 - [x] 支持AI对话
 - [x] 支持上下文关联记忆（可设置记忆文本长度）
 - [x] 用户鉴别（每个用户的历史记录独立）
-- [x] 支持用户自定义、更改、切换预设（prompt）
+- [x] 支持用户自定义、更改、切换预设（Prompt）
 - [x] 自动生成人物预设菜单、帮助列表，无需重写
 - [x] 基于pickle的历史记录持久化
 - [x] 完善的配置项（有其他需求请发issue）
+- [x] 支持AI绘图（AI Image Generation）
 - [ ] 用户权限与功能区分（超级用户、普通用户）
-- [ ] 支持图片生成（ImageGeneration）
+- [ ] PPT生成（PPT Generation）
 
 ### 📦 项目地址
 - Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
 - 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
 
 ## 💿 安装
 
@@ -100,38 +101,43 @@
 | SPARKAPI_PRIORITY | 否 | 80 | 该值越小，事件越先被触发。本插件建议设置较大的值。可选值：1~97<br>若触发本插件事件，所有插件中优先级大于此值的事件都将被阻断。<br>本插件中事件的优先级顺序：私聊阻断（=priority）< 功能（=priority+1）< 对话（=priority+2） |
 | SPARKAPI_COMMANDS__CHAT | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空：COMMAND_START = [""]） |
 | SPARKAPI_FL_NOTICE | 否 | True | 收到请求时是否提示“已收到请求” |
 | SPARKAPI_FL_SETPRESET_CLEAR | 否 | True | 切换人物预设时是否清除当前对话上下文 |
 | SPARKAPI_FL_PRIVATE_CHAT | 否 | True | 是否允许私聊使用 |
 | SPARKAPI_FL_GROUP_PUBLIC | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
 | SPARKAPI_FL_GROUP_AT | 否 | True | 群聊回复消息时是否需要@提问者 |
+| SPARKAPI_FL_IMGGEN | 否 | True | 是否启用AI绘图功能 |
 | SPARKAPI_BOT_NAME | 否 | "" | 机器人的名字 |
 
 以下配置项请查看`/.venv/Lib/nonebot_plugin_sparkapi/config.py`修改：
 1. sparkapi_commands：指令表（允许单个字符串或字符串列表）
 2. sparkapi_commands_info：指令表说明（用于生成帮助信息）
 3. sparkapi_message_blockprivate：阻断私聊时的提示信息
+4. sparkapi_message_blockimggen：阻断AI绘图时的提示信息
 
 ## 🎉 使用
 ### 指令表（默认）
 以下所有指令均可在config.py中修改，且无需重写菜单/指令生成函数
 
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | SPARKAPI_COMMAND_CHAT（若不为空） + 对话内容 | 是 | 私聊/群聊 | 与机器人进行对话 |
 | help/帮助 | 是 | 私聊/群聊 | 显示帮助信息 |
 | preset/人物预设 | 是 | 私聊/群聊 | 显示人物预设菜单和当前预设 |
-| set/切换预设 | 是 | 私聊/群聊 | 显示人物预设菜单，选择并切换 |
+| set/切换预设 | 是 | 私聊/群聊 | 显示人物预设菜单，选择人物预设并切换 |
 | set/切换预设 + 人物名 | 是 | 私聊/群聊 | 切换人物预设 |
 | create/创建预设 | 是 | 私聊/群聊 | 创建自定义的人物预设 |
 | delete/删除预设 | 是 | 私聊/群聊 | 删除自定义的人物预设 |
-| delete/删除预设 + 人物名 | 是 | 私聊/群聊 | 显示自定义人物预设菜单, 选择并删除 |
+| delete/删除预设 + 人物名 | 是 | 私聊/群聊 | 显示自定义人物预设菜单, 选择人物预设并删除 |
 | clear/清空对话 | 是 | 私聊/群聊 | 清除当前对话上下文 |
 | save/保存对话 | 是 | 私聊/群聊 | 保存当前对话记录 |
 | load/加载对话 | 是 | 私聊/群聊 | 加载上次保存的对话记录 |
+| imggen/AI绘图 + 描述 | 是 | 私聊/群聊 | AI根据描述生成图片 |
+| imggen/AI绘图 | 是 | 私聊/群聊 | 下一句给出描述，AI根据描述生成图片 |
 
 ### 人物预设
 1. 智能助手（默认）
 2. 心理咨询师
+3. 李白
 
 ### 效果图
 ![demo](https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

#### html2text {}

```diff
@@ -5,21 +5,22 @@
                                    [python]
 ## ð ä»ç»
 åºäºNonebot2å¹³å°ï¼è°ç¨ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIçAIèå¤©æºå¨äººæä»¶
 éç¨äºæææ¨¡åçæ¬ï¼é»è®¤å½åææ°ï¼v3.5ï¼ï¼ï¼æ¯æä¸ä¸æå³èãäººç©é¢è®¾ç­åè½
 ### ð¬ åè½ - [x] æ¯æAIå¯¹è¯ - [x]
 æ¯æä¸ä¸æå³èè®°å¿ï¼å¯è®¾ç½®è®°å¿ææ¬é¿åº¦ï¼ - [x]
 ç¨æ·é´å«ï¼æ¯ä¸ªç¨æ·çåå²è®°å½ç¬ç«ï¼ - [x]
-æ¯æç¨æ·èªå®ä¹ãæ´æ¹ãåæ¢é¢è®¾ï¼promptï¼ - [x]
+æ¯æç¨æ·èªå®ä¹ãæ´æ¹ãåæ¢é¢è®¾ï¼Promptï¼ - [x]
 èªå¨çæäººç©é¢è®¾èåãå¸®å©åè¡¨ï¼æ ééå - [x]
 åºäºpickleçåå²è®°å½æä¹å - [x]
-å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [ ]
+å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [x] æ¯æAIç»å¾ï¼AI
+Image Generationï¼ - [ ]
 ç¨æ·æéä¸åè½åºåï¼è¶çº§ç¨æ·ãæ®éç¨æ·ï¼ - [ ]
-æ¯æå¾ççæï¼ImageGenerationï¼ ### ð¦ é¡¹ç®å°å - Githubï¼https:
-//github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
+PPTçæï¼PPT Generationï¼ ### ð¦ é¡¹ç®å°å - Githubï¼https://
+github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
 Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-sparkapi ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-sparkapi pdm pdm add
 nonebot-plugin-sparkapi poetry poetry add nonebot-plugin-sparkapi conda conda
 install nonebot-plugin-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
@@ -52,31 +53,36 @@
 æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | |
 SPARKAPI_FL_SETPRESET_CLEAR | å¦ | True |
 åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | |
 SPARKAPI_FL_PRIVATE_CHAT | å¦ | True | æ¯å¦åè®¸ç§èä½¿ç¨ | |
 SPARKAPI_FL_GROUP_PUBLIC | å¦ | False | ç¾¤èå¯ç¨å¬å±ä¼è¯
 Trueï¼ææäººå±äº«åä¸ä¼è¯
 Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | SPARKAPI_FL_GROUP_AT | å¦ | True |
-ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_BOT_NAME | å¦ | "" |
+ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_FL_IMGGEN | å¦ | True
+| æ¯å¦å¯ç¨AIç»å¾åè½ | | SPARKAPI_BOT_NAME | å¦ | "" |
 æºå¨äººçåå­ | ä»¥ä¸éç½®é¡¹è¯·æ¥ç`/.venv/Lib/
 nonebot_plugin_sparkapi/config.py`ä¿®æ¹ï¼ 1.
 sparkapi_commandsï¼æä»¤è¡¨ï¼åè®¸åä¸ªå­ç¬¦ä¸²æå­ç¬¦ä¸²åè¡¨ï¼ 2.
 sparkapi_commands_infoï¼æä»¤è¡¨è¯´æï¼ç¨äºçæå¸®å©ä¿¡æ¯ï¼ 3.
-sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
+sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ 4.
+sparkapi_message_blockimggenï¼é»æ­AIç»å¾æ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
 ### æä»¤è¡¨ï¼é»è®¤ï¼
 ä»¥ä¸æææä»¤åå¯å¨config.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
 æä»¤çæå½æ° | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:| | SPARKAPI_COMMAND_CHATï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ |
 ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help/å¸®å© | æ¯ | ç§è/ç¾¤è
 | æ¾ç¤ºå¸®å©ä¿¡æ¯ | | preset/äººç©é¢è®¾ | æ¯ | ç§è/ç¾¤è |
 æ¾ç¤ºäººç©é¢è®¾èååå½åé¢è®¾ | | set/åæ¢é¢è®¾ | æ¯ | ç§è/
-ç¾¤è | æ¾ç¤ºäººç©é¢è®¾èåï¼éæ©å¹¶åæ¢ | | set/åæ¢é¢è®¾ +
-äººç©å | æ¯ | ç§è/ç¾¤è | åæ¢äººç©é¢è®¾ | | create/åå»ºé¢è®¾ |
-æ¯ | ç§è/ç¾¤è | åå»ºèªå®ä¹çäººç©é¢è®¾ | | delete/å é¤é¢è®¾ |
-æ¯ | ç§è/ç¾¤è | å é¤èªå®ä¹çäººç©é¢è®¾ | | delete/å é¤é¢è®¾ +
-äººç©å | æ¯ | ç§è/ç¾¤è | æ¾ç¤ºèªå®ä¹äººç©é¢è®¾èå,
-éæ©å¹¶å é¤ | | clear/æ¸ç©ºå¯¹è¯ | æ¯ | ç§è/ç¾¤è |
-æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | save/ä¿å­å¯¹è¯ | æ¯ | ç§è/ç¾¤è |
-ä¿å­å½åå¯¹è¯è®°å½ | | load/å è½½å¯¹è¯ | æ¯ | ç§è/ç¾¤è |
-å è½½ä¸æ¬¡ä¿å­çå¯¹è¯è®°å½ | ### äººç©é¢è®¾ 1.
-æºè½å©æï¼é»è®¤ï¼ 2. å¿çå¨è¯¢å¸ ### ææå¾ ![demo](https://
-github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
+ç¾¤è | æ¾ç¤ºäººç©é¢è®¾èåï¼éæ©äººç©é¢è®¾å¹¶åæ¢ | | set/
+åæ¢é¢è®¾ + äººç©å | æ¯ | ç§è/ç¾¤è | åæ¢äººç©é¢è®¾ | | create/
+åå»ºé¢è®¾ | æ¯ | ç§è/ç¾¤è | åå»ºèªå®ä¹çäººç©é¢è®¾ | | delete/
+å é¤é¢è®¾ | æ¯ | ç§è/ç¾¤è | å é¤èªå®ä¹çäººç©é¢è®¾ | | delete/
+å é¤é¢è®¾ + äººç©å | æ¯ | ç§è/ç¾¤è |
+æ¾ç¤ºèªå®ä¹äººç©é¢è®¾èå, éæ©äººç©é¢è®¾å¹¶å é¤ | | clear/
+æ¸ç©ºå¯¹è¯ | æ¯ | ç§è/ç¾¤è | æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | save/
+ä¿å­å¯¹è¯ | æ¯ | ç§è/ç¾¤è | ä¿å­å½åå¯¹è¯è®°å½ | | load/
+å è½½å¯¹è¯ | æ¯ | ç§è/ç¾¤è | å è½½ä¸æ¬¡ä¿å­çå¯¹è¯è®°å½ | |
+imggen/AIç»å¾ + æè¿° | æ¯ | ç§è/ç¾¤è | AIæ ¹æ®æè¿°çæå¾ç | |
+imggen/AIç»å¾ | æ¯ | ç§è/ç¾¤è |
+ä¸ä¸å¥ç»åºæè¿°ï¼AIæ ¹æ®æè¿°çæå¾ç | ### äººç©é¢è®¾ 1.
+æºè½å©æï¼é»è®¤ï¼ 2. å¿çå¨è¯¢å¸ 3. æç½ ### ææå¾ ![demo]
+(https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

### Comparing `nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/SparkApi.py` & `nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/SparkApi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/__init__.py` & `nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from nonebot.adapters.onebot.v11 import MessageEvent as ME,PrivateMessageEvent as PME # type: ignore
 from nonebot.adapters.onebot.v11 import Message , MessageSegment as MS # type: ignore
 
 import nonebot
 from nonebot.plugin import PluginMetadata
 from nonebot.plugin.on import on_message
 from nonebot.params import CommandArg
-from nonebot.rule import Rule,to_me,is_type
+from nonebot.rule import to_me,is_type,command
 from nonebot.params import ArgPlainText
 # from nonebot.permission import SUPERUSER
 
 from copy import deepcopy
 
-from . import SparkApi,funcs,info,storage
+from . import SparkApi,ImgGenApi,funcs,info,storage
 from .config import Config
 
 # ---------------------------Configurations---------------------------
 # 插件元数据
 __plugin_meta__ = PluginMetadata(
     name="科大讯飞星火大语言模型官方API聊天机器人插件",
     description="调用科大讯飞星火大语言模型官方API的聊天机器人插件。适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设",
@@ -38,56 +38,55 @@
 api_key = conf.sparkapi_api_key
 
 # 获取优先级设置
 priority_blockprivate = conf.sparkapi_priority
 priority_function = priority_blockprivate + 1
 priority_chat = priority_blockprivate + 2
 
-# if not appid or not api_secret or not api_key:
-#     raise ConfigError("请设置API信息,可前往 https://console.xfyun.cn/ 获取")
-
 commands = conf.sparkapi_commands
-fl_private_chat = conf.sparkapi_fl_private_chat
 fl_group_at = conf.sparkapi_fl_group_at
 fl_notice = conf.sparkapi_fl_notice
 fl_setpreset_clear = conf.sparkapi_fl_setpreset_clear
+fl_imggen = conf.sparkapi_fl_imggen
 maxlength = conf.sparkpai_model_maxlength
 priority = conf.sparkapi_priority
 
 sessions = {} # 会话记录
 spname = {} # 选取的prompt
 presets = {} # 人物预设列表
 
+# if not appid or not api_secret or not api_key:
+#     raise ConfigError("请设置API信息,可前往 https://console.xfyun.cn/ 获取")
+
 # ---------------------------Tests---------------------------
-# print(unify_commands(commands["chat"]))
-# print(unify_commands(commands["help"]))
-# print(*unify_commands(commands["help"]))
 
 # ---------------------------Matchers---------------------------
 # 事件响应器：私聊阻断
 async def fl_blockprivate() -> bool:
     return not conf.sparkapi_fl_private_chat
 rule_blockprivate = is_type(PME) & fl_blockprivate
 matcher_blockprivate = on_message(
     rule = rule_blockprivate,
     priority = priority_blockprivate,
     block = True
 )
+
 @matcher_blockprivate.handle()
 async def blockprivate_handle_function():
     await matcher_blockprivate.finish(MS.text(conf.sparkapi_message_blockprivate))
 
 
 # 事件响应器：带上下文的对话
 rule_chat = to_me() & funcs.trans_command(commands["chat"])
 matcher_chat = on_message(
     rule = rule_chat,
     priority = priority_chat,
     block = True
 )
+
 @matcher_chat.handle()
 async def chat_handle_function(event: ME, msg: Message = CommandArg()):
     content = msg.extract_plain_text().strip()
     if not content:
         await matcher_chat.finish(MS.text("请输入文字！"))
 
     if len(content) > maxlength//2:
@@ -132,32 +131,35 @@
 # 事件响应器：显示帮助信息
 rule_help = to_me() & funcs.trans_command(commands["help"])
 matcher_help = on_message(
     rule = rule_help,
     priority = priority_function,
     block = True
 )
+
 @matcher_help.handle()
 async def sparkhelp_handle_function():
     await matcher_help.finish(MS.text(info.help_info))
 
 
 # 事件响应器：创建人物预设
 rule_preset_create = to_me() & funcs.trans_command(commands["preset_create"])
 matcher_preset_create = on_message(
     rule = rule_preset_create,
     priority = priority_function,
     block=True
 )
+
 @matcher_preset_create.got("pname",prompt="请输入预设名称\n回复“取消”退出")
 async def preset_create_got_check(event: ME, pname: str= ArgPlainText()):
     if pname=="取消":
         await matcher_preset_create.finish(MS.text("操作已取消"))
 
     session_id = funcs.get_session_id(event)
+    
     check = storage.f_preset_check(pname, session_id) or (pname in info.presets_default)
     if check:
         await matcher_preset_create.finish(MS.text(f'已存在名为"{pname}"的预设'))
 
 @matcher_preset_create.got("prompt",prompt="请输入预设内容\n回复“取消”退出")
 async def preset_create_got_function(event: ME, pname: str = ArgPlainText(), prompt: str = ArgPlainText()):
     if prompt=="取消":
@@ -182,14 +184,15 @@
 # 事件响应器：删除人物预设
 rule_preset_delete = to_me() & funcs.trans_command(commands["preset_delete"])
 matcher_preset_delete = on_message(
     rule = rule_preset_delete,
     priority = priority_function,
     block = True
 )
+
 @matcher_preset_delete.handle()
 async def preset_delete_handle_function(event: ME, msg: Message = CommandArg()):
     pname = msg.extract_plain_text().strip()
     session_id = funcs.get_session_id(event)
     custom_presets = storage.f_preset_load(funcs.get_session_id(event))
 
     if custom_presets:
@@ -199,17 +202,17 @@
 
     if len(custom_presets) == 0:
         await matcher_preset_delete.finish(MS.text("无自定义预设！"))
 
     if pname:
         await preset_delete_function(event, pname)
         
-    msg = info.get_preset_lst({},custom_presets)
-    msg = msg+"\n请输入名称以删除人物预设，回复“取消”退出"
-    await matcher_preset_delete.send(MS.text(msg))
+    ret = info.get_preset_lst({},custom_presets)
+    ret = ret+"\n请输入名称以删除人物预设，回复“取消”退出"
+    await matcher_preset_delete.send(MS.text(ret))
 
 @matcher_preset_delete.got("pname")
 async def preset_delete_got_function(event: ME, pname: str = ArgPlainText()):
     if pname=="取消":
         await matcher_preset_delete.finish(MS.text("操作已取消"))
 
     await preset_delete_function(event, pname)
@@ -231,14 +234,15 @@
 # 事件响应器：显示人物预设
 rule_preset_show = to_me() & funcs.trans_command(commands["preset_show"])
 matcher_preset_show = on_message(
     rule = rule_preset_show,
     priority = priority_function,
     block = True
 )
+
 @matcher_preset_show.handle()
 async def preset_show_handle_function(event:ME):
     session_id = funcs.get_session_id(event)
     custom_presets = storage.f_preset_load(session_id)
 
     msg = info.get_preset_lst(info.presets_default,custom_presets)
     msg += f"\n当前预设为：{spname.get(session_id,'智能助手')}"
@@ -248,31 +252,32 @@
 # 事件响应器：切换人物预设
 rule_preset_set = to_me() & funcs.trans_command(commands["preset_set"])
 matcher_preset_set = on_message(
     rule = rule_preset_set,
     priority=priority_function,
     block=True
 )
+
 @matcher_preset_set.handle()
 async def preset_set_handle_function(event: ME, msg: Message = CommandArg()):
     pname = msg.extract_plain_text().strip()
     session_id = funcs.get_session_id(event)
     custom_presets = storage.f_preset_load(funcs.get_session_id(event))
 
     if custom_presets:
         presets[session_id] = funcs.merge_dict(info.presets_default,custom_presets)
     else:
         presets[session_id] = info.presets_default
 
     if pname:
         await preset_set_function(event, pname)
 
-    msg = info.get_preset_lst(info.presets_default,custom_presets)
-    msg = msg+"\n请输入名称以选择人物预设，回复“取消”退出"
-    await matcher_preset_set.send(MS.text(msg))
+    ret = info.get_preset_lst(info.presets_default,custom_presets)
+    ret = ret+"\n请输入名称以选择人物预设，回复“取消”退出"
+    await matcher_preset_set.send(MS.text(ret))
 
 @matcher_preset_set.got("pname")
 async def preset_set_got_function(event: ME, pname: str = ArgPlainText()):
     if pname=="取消":
         await matcher_preset_set.finish(MS.text("操作已取消"))
     await preset_set_function(event, pname)
 
@@ -316,14 +321,15 @@
 # 事件响应器：清空对话
 rule_session_clear = to_me() & funcs.trans_command(commands["session_clear"])
 matcher_session_clear = on_message(
     rule = rule_session_clear,
     priority=priority_function,
     block=True
 )
+
 @matcher_session_clear.handle()
 async def session_clear_handle_function(event: ME):
     session_id = funcs.get_session_id(event)
 
     if session_id in sessions:
         del sessions[session_id]
         del spname[session_id]
@@ -335,14 +341,15 @@
 # 事件响应器：保存对话记录
 rule_session_save = to_me() & funcs.trans_command(commands["session_save"])
 matcher_session_save = on_message(
     rule = rule_session_save,
     priority=priority_function,
     block=True
 )
+
 @matcher_session_save.handle()
 async def session_save_handle_function(event: ME):
     session_id = funcs.get_session_id(event)
 
     if session_id in sessions:
         storage.f_session_save(sessions[session_id], spname[session_id], session_id)
         await matcher_session_save.finish(MS.text("当前对话记录已保存！"))
@@ -353,33 +360,80 @@
 # 事件响应器：加载对话记录
 rule_session_load = to_me() & funcs.trans_command(commands["session_load"])
 matcher_session_load = on_message(
     rule = rule_session_load,
     priority=priority_function,
     block=True
 )
+
 @matcher_session_load.handle()
 async def session_load_handle_function(event: ME):
     session_id = funcs.get_session_id(event)
     session, pname = storage.f_session_load(session_id)
 
     if session:
         sessions[session_id] = session
         spname[session_id] = pname
         await matcher_session_load.finish(MS.text("已加载上次保存的对话记录！"))
     else:
         await matcher_session_load.finish(MS.text("未保存对话记录"))
 
 
+# 事件响应器：AI绘图
+rule_imggen = to_me() & funcs.trans_command(commands["image_generation"])
+matcher_imggen = on_message(
+    rule = rule_imggen,
+    priority = priority_function,
+    block = True
+)
+
+@matcher_imggen.handle()
+async def imggen_handle_function(event: ME, msg: Message = CommandArg()):
+    if not fl_imggen:
+        await matcher_imggen.finish(MS.text(conf.sparkapi_message_blockimggen))
+    
+    content = msg.extract_plain_text().strip()
+    session_id = funcs.get_session_id(event)
+
+    if content : 
+        if len(content) > maxlength:
+            await matcher_imggen.finish(MS.text(f"输入文字过长：请不要超过{maxlength}字节！"))
+        ret = await request_IG(content)
+        path = storage.f_image_base64_save(ret, f"{session_id}.png")
+        await matcher_imggen.finish(MS.image(path))
+
+@matcher_imggen.got("content",prompt="请输入文字描述\n回复“取消”退出")
+async def imggen_got_function(event: ME, content: str = ArgPlainText()):
+    if content=="取消":
+        await matcher_imggen.finish(MS.text("操作已取消"))
+    if len(content) > maxlength:
+        await matcher_imggen.finish(MS.text(f"输入文字过长：请不要超过{maxlength}字节！"))
+    
+    session_id = funcs.get_session_id(event)
+
+    ret = await request_IG(content)
+    path = storage.f_image_base64_save(ret, f"{session_id}.png")
+    await matcher_imggen.finish(MS.image(path))
+
+
 # ---------------------------API Request---------------------------
 model_version = funcs.unify_model_version(conf.sparkapi_model_version)
 Spark_url = funcs.get_Spark_url(model_version)
 domain = funcs.get_domain(model_version)
 
 async def request(history, sid, session_id, pname):
     history = deepcopy(history)
     history.insert(0, presets[session_id][pname])
     history = funcs.checklen(history)
     print("request:", history)
     SparkApi.answer = ""
     await SparkApi.main(appid,api_key,api_secret,Spark_url,domain,history,sid)
-    return SparkApi.answer
+    return SparkApi.answer
+
+IG_url = "http://spark-api.cn-huabei-1.xf-yun.com/v2.1/tti"
+IG_domain = "general"
+
+async def request_IG(content):
+    ImgGenApi.res = ""
+    ImgGenApi.duration = 0
+    await ImgGenApi.main(appid,api_key,api_secret,IG_url,IG_domain,content)
+    return ImgGenApi.res
```

### Comparing `nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/config.py` & `nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,31 +24,40 @@
         "preset_show" : ["preset","人物预设"], # 显示人物预设
         "preset_set" : ["set","切换预设"], # 切换人物预设
         "preset_create" : ["create","创建预设"], # 创建人物预设
         "preset_delete" : ["delete","删除预设"], # 删除人物预设
         "session_clear" : ["clear","清空对话"], # 清空对话
         "session_save" : ["save","保存对话"], # 保存对话记录
         "session_load" : ["load","加载对话"],  # 加载对话记录
+        "image_generation" : ["imggen","AI绘图"],  # AI绘图
     }
     sparkapi_commands_info: dict[str, str] = { # 命令说明，用于生成帮助信息
         "chat" : "与机器人进行对话",
         "help" : "显示帮助信息",
         "preset_show" : "显示人物预设菜单和当前预设",
         "preset_set" : "切换人物预设",
         "preset_create" : "创建人物预设",
         "preset_delete" : "删除人物预设",
         "session_clear" : "清空当前对话上下文",
         "session_save" : "保存本次对话记录",
         "session_load" : "加载上次保存的对话记录",
+        "image_generation" : "AI根据文字描述绘制一张图片",
     }
 
     # 聊天设置
     sparkapi_fl_notice: bool = True # 收到请求时是否提示已收到请求
     sparkapi_fl_setpreset_clear: bool = True # 切换人物预设时是否清空上下文
+
     # 私聊设置
     sparkapi_fl_private_chat: bool = True # 允许私聊
     sparkapi_message_blockprivate: str = "私聊功能已关闭！如有需要，请联系管理员。" # 阻断私聊时的提示信息
+    
     # 群聊设置
     sparkapi_fl_group_public: bool = False # 群聊启用公共会话：True：所有人共享同一会话；False：每个人的会话各自独立
     sparkapi_fl_group_at: bool = True # 群聊中，回复时是否需要@提问者
+    
+    # 图片生成功能，API信息一般与AI对话API一致
+    sparkapi_fl_imggen : bool = True # 启用图片生成功能
+    sparkapi_message_blockimggen : str = "图片生成功能已关闭！如有需要，请联系管理员。" # 阻断图片生成功能时的提示信息
 
+    # 机器人名字
     sparkapi_bot_name: str = "" # 机器人名字
```

### Comparing `nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/funcs.py` & `nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/funcs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/info.py` & `nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         'role': 'system', 
         'content': prompt_assistant
     },
     "心理咨询师":{
         'role': 'system',
         'content': prompt_psychological_counselor
     },
-    # "李白":{
-    #     'role': 'system',
-    #     'content': prompt_libai
-    # }
+    "李白":{
+        'role': 'system',
+        'content': prompt_libai
+    }
 }
 
 # 生成人物预设列表
 def get_preset_lst(presets:dict,costom_presets:dict)->str:
     presets_lst = "【人物预设】\n"
     for i, preset in enumerate(presets.keys(),start=1):
         presets_lst += f"{i}. {preset}\n"
```

### Comparing `nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/PKG-INFO` & `nonebot_plugin_sparkapi-1.4.0/nonebot_plugin_sparkapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.3.0
+Version: 1.4.0
 Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,14 +27,16 @@
         
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
 Requires-Dist: websockets<13.0,>=12.0
+Requires-Dist: httpx<1.0.0,>=0.19.0
+Requires-Dist: pillow<11.0.0,>=10.0.0
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
@@ -60,20 +62,21 @@
 
 适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设等功能
 
 ### 💬 功能
 - [x] 支持AI对话
 - [x] 支持上下文关联记忆（可设置记忆文本长度）
 - [x] 用户鉴别（每个用户的历史记录独立）
-- [x] 支持用户自定义、更改、切换预设（prompt）
+- [x] 支持用户自定义、更改、切换预设（Prompt）
 - [x] 自动生成人物预设菜单、帮助列表，无需重写
 - [x] 基于pickle的历史记录持久化
 - [x] 完善的配置项（有其他需求请发issue）
+- [x] 支持AI绘图（AI Image Generation）
 - [ ] 用户权限与功能区分（超级用户、普通用户）
-- [ ] 支持图片生成（ImageGeneration）
+- [ ] PPT生成（PPT Generation）
 
 ### 📦 项目地址
 - Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
 - 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
 
 ## 💿 安装
 
@@ -134,38 +137,43 @@
 | SPARKAPI_PRIORITY | 否 | 80 | 该值越小，事件越先被触发。本插件建议设置较大的值。可选值：1~97<br>若触发本插件事件，所有插件中优先级大于此值的事件都将被阻断。<br>本插件中事件的优先级顺序：私聊阻断（=priority）< 功能（=priority+1）< 对话（=priority+2） |
 | SPARKAPI_COMMANDS__CHAT | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空：COMMAND_START = [""]） |
 | SPARKAPI_FL_NOTICE | 否 | True | 收到请求时是否提示“已收到请求” |
 | SPARKAPI_FL_SETPRESET_CLEAR | 否 | True | 切换人物预设时是否清除当前对话上下文 |
 | SPARKAPI_FL_PRIVATE_CHAT | 否 | True | 是否允许私聊使用 |
 | SPARKAPI_FL_GROUP_PUBLIC | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
 | SPARKAPI_FL_GROUP_AT | 否 | True | 群聊回复消息时是否需要@提问者 |
+| SPARKAPI_FL_IMGGEN | 否 | True | 是否启用AI绘图功能 |
 | SPARKAPI_BOT_NAME | 否 | "" | 机器人的名字 |
 
 以下配置项请查看`/.venv/Lib/nonebot_plugin_sparkapi/config.py`修改：
 1. sparkapi_commands：指令表（允许单个字符串或字符串列表）
 2. sparkapi_commands_info：指令表说明（用于生成帮助信息）
 3. sparkapi_message_blockprivate：阻断私聊时的提示信息
+4. sparkapi_message_blockimggen：阻断AI绘图时的提示信息
 
 ## 🎉 使用
 ### 指令表（默认）
 以下所有指令均可在config.py中修改，且无需重写菜单/指令生成函数
 
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | SPARKAPI_COMMAND_CHAT（若不为空） + 对话内容 | 是 | 私聊/群聊 | 与机器人进行对话 |
 | help/帮助 | 是 | 私聊/群聊 | 显示帮助信息 |
 | preset/人物预设 | 是 | 私聊/群聊 | 显示人物预设菜单和当前预设 |
-| set/切换预设 | 是 | 私聊/群聊 | 显示人物预设菜单，选择并切换 |
+| set/切换预设 | 是 | 私聊/群聊 | 显示人物预设菜单，选择人物预设并切换 |
 | set/切换预设 + 人物名 | 是 | 私聊/群聊 | 切换人物预设 |
 | create/创建预设 | 是 | 私聊/群聊 | 创建自定义的人物预设 |
 | delete/删除预设 | 是 | 私聊/群聊 | 删除自定义的人物预设 |
-| delete/删除预设 + 人物名 | 是 | 私聊/群聊 | 显示自定义人物预设菜单, 选择并删除 |
+| delete/删除预设 + 人物名 | 是 | 私聊/群聊 | 显示自定义人物预设菜单, 选择人物预设并删除 |
 | clear/清空对话 | 是 | 私聊/群聊 | 清除当前对话上下文 |
 | save/保存对话 | 是 | 私聊/群聊 | 保存当前对话记录 |
 | load/加载对话 | 是 | 私聊/群聊 | 加载上次保存的对话记录 |
+| imggen/AI绘图 + 描述 | 是 | 私聊/群聊 | AI根据描述生成图片 |
+| imggen/AI绘图 | 是 | 私聊/群聊 | 下一句给出描述，AI根据描述生成图片 |
 
 ### 人物预设
 1. 智能助手（默认）
 2. 心理咨询师
+3. 李白
 
 ### 效果图
 ![demo](https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.4.0 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -14,33 +14,35 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Requires-Python: >=3.10 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: nonebot-adapter-
 onebot<3.0.0,>=2.2.1 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3 Requires-Dist:
-websockets<13.0,>=12.0
+websockets<13.0,>=12.0 Requires-Dist: httpx<1.0.0,>=0.19.0 Requires-Dist:
+pillow<11.0.0,>=10.0.0
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                         # nonebot-plugin-sparkapi _â¨
  ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIèå¤©æºå¨äºº â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð ä»ç»
 åºäºNonebot2å¹³å°ï¼è°ç¨ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIçAIèå¤©æºå¨äººæä»¶
 éç¨äºæææ¨¡åçæ¬ï¼é»è®¤å½åææ°ï¼v3.5ï¼ï¼ï¼æ¯æä¸ä¸æå³èãäººç©é¢è®¾ç­åè½
 ### ð¬ åè½ - [x] æ¯æAIå¯¹è¯ - [x]
 æ¯æä¸ä¸æå³èè®°å¿ï¼å¯è®¾ç½®è®°å¿ææ¬é¿åº¦ï¼ - [x]
 ç¨æ·é´å«ï¼æ¯ä¸ªç¨æ·çåå²è®°å½ç¬ç«ï¼ - [x]
-æ¯æç¨æ·èªå®ä¹ãæ´æ¹ãåæ¢é¢è®¾ï¼promptï¼ - [x]
+æ¯æç¨æ·èªå®ä¹ãæ´æ¹ãåæ¢é¢è®¾ï¼Promptï¼ - [x]
 èªå¨çæäººç©é¢è®¾èåãå¸®å©åè¡¨ï¼æ ééå - [x]
 åºäºpickleçåå²è®°å½æä¹å - [x]
-å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [ ]
+å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [x] æ¯æAIç»å¾ï¼AI
+Image Generationï¼ - [ ]
 ç¨æ·æéä¸åè½åºåï¼è¶çº§ç¨æ·ãæ®éç¨æ·ï¼ - [ ]
-æ¯æå¾ççæï¼ImageGenerationï¼ ### ð¦ é¡¹ç®å°å - Githubï¼https:
-//github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
+PPTçæï¼PPT Generationï¼ ### ð¦ é¡¹ç®å°å - Githubï¼https://
+github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
 Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-sparkapi ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-sparkapi pdm pdm add
 nonebot-plugin-sparkapi poetry poetry add nonebot-plugin-sparkapi conda conda
 install nonebot-plugin-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
@@ -73,31 +75,36 @@
 æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | |
 SPARKAPI_FL_SETPRESET_CLEAR | å¦ | True |
 åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | |
 SPARKAPI_FL_PRIVATE_CHAT | å¦ | True | æ¯å¦åè®¸ç§èä½¿ç¨ | |
 SPARKAPI_FL_GROUP_PUBLIC | å¦ | False | ç¾¤èå¯ç¨å¬å±ä¼è¯
 Trueï¼ææäººå±äº«åä¸ä¼è¯
 Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | SPARKAPI_FL_GROUP_AT | å¦ | True |
-ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_BOT_NAME | å¦ | "" |
+ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_FL_IMGGEN | å¦ | True
+| æ¯å¦å¯ç¨AIç»å¾åè½ | | SPARKAPI_BOT_NAME | å¦ | "" |
 æºå¨äººçåå­ | ä»¥ä¸éç½®é¡¹è¯·æ¥ç`/.venv/Lib/
 nonebot_plugin_sparkapi/config.py`ä¿®æ¹ï¼ 1.
 sparkapi_commandsï¼æä»¤è¡¨ï¼åè®¸åä¸ªå­ç¬¦ä¸²æå­ç¬¦ä¸²åè¡¨ï¼ 2.
 sparkapi_commands_infoï¼æä»¤è¡¨è¯´æï¼ç¨äºçæå¸®å©ä¿¡æ¯ï¼ 3.
-sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
+sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ 4.
+sparkapi_message_blockimggenï¼é»æ­AIç»å¾æ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
 ### æä»¤è¡¨ï¼é»è®¤ï¼
 ä»¥ä¸æææä»¤åå¯å¨config.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
 æä»¤çæå½æ° | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:| | SPARKAPI_COMMAND_CHATï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ |
 ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help/å¸®å© | æ¯ | ç§è/ç¾¤è
 | æ¾ç¤ºå¸®å©ä¿¡æ¯ | | preset/äººç©é¢è®¾ | æ¯ | ç§è/ç¾¤è |
 æ¾ç¤ºäººç©é¢è®¾èååå½åé¢è®¾ | | set/åæ¢é¢è®¾ | æ¯ | ç§è/
-ç¾¤è | æ¾ç¤ºäººç©é¢è®¾èåï¼éæ©å¹¶åæ¢ | | set/åæ¢é¢è®¾ +
-äººç©å | æ¯ | ç§è/ç¾¤è | åæ¢äººç©é¢è®¾ | | create/åå»ºé¢è®¾ |
-æ¯ | ç§è/ç¾¤è | åå»ºèªå®ä¹çäººç©é¢è®¾ | | delete/å é¤é¢è®¾ |
-æ¯ | ç§è/ç¾¤è | å é¤èªå®ä¹çäººç©é¢è®¾ | | delete/å é¤é¢è®¾ +
-äººç©å | æ¯ | ç§è/ç¾¤è | æ¾ç¤ºèªå®ä¹äººç©é¢è®¾èå,
-éæ©å¹¶å é¤ | | clear/æ¸ç©ºå¯¹è¯ | æ¯ | ç§è/ç¾¤è |
-æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | save/ä¿å­å¯¹è¯ | æ¯ | ç§è/ç¾¤è |
-ä¿å­å½åå¯¹è¯è®°å½ | | load/å è½½å¯¹è¯ | æ¯ | ç§è/ç¾¤è |
-å è½½ä¸æ¬¡ä¿å­çå¯¹è¯è®°å½ | ### äººç©é¢è®¾ 1.
-æºè½å©æï¼é»è®¤ï¼ 2. å¿çå¨è¯¢å¸ ### ææå¾ ![demo](https://
-github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
+ç¾¤è | æ¾ç¤ºäººç©é¢è®¾èåï¼éæ©äººç©é¢è®¾å¹¶åæ¢ | | set/
+åæ¢é¢è®¾ + äººç©å | æ¯ | ç§è/ç¾¤è | åæ¢äººç©é¢è®¾ | | create/
+åå»ºé¢è®¾ | æ¯ | ç§è/ç¾¤è | åå»ºèªå®ä¹çäººç©é¢è®¾ | | delete/
+å é¤é¢è®¾ | æ¯ | ç§è/ç¾¤è | å é¤èªå®ä¹çäººç©é¢è®¾ | | delete/
+å é¤é¢è®¾ + äººç©å | æ¯ | ç§è/ç¾¤è |
+æ¾ç¤ºèªå®ä¹äººç©é¢è®¾èå, éæ©äººç©é¢è®¾å¹¶å é¤ | | clear/
+æ¸ç©ºå¯¹è¯ | æ¯ | ç§è/ç¾¤è | æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | save/
+ä¿å­å¯¹è¯ | æ¯ | ç§è/ç¾¤è | ä¿å­å½åå¯¹è¯è®°å½ | | load/
+å è½½å¯¹è¯ | æ¯ | ç§è/ç¾¤è | å è½½ä¸æ¬¡ä¿å­çå¯¹è¯è®°å½ | |
+imggen/AIç»å¾ + æè¿° | æ¯ | ç§è/ç¾¤è | AIæ ¹æ®æè¿°çæå¾ç | |
+imggen/AIç»å¾ | æ¯ | ç§è/ç¾¤è |
+ä¸ä¸å¥ç»åºæè¿°ï¼AIæ ¹æ®æè¿°çæå¾ç | ### äººç©é¢è®¾ 1.
+æºè½å©æï¼é»è®¤ï¼ 2. å¿çå¨è¯¢å¸ 3. æç½ ### ææå¾ ![demo]
+(https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

### Comparing `nonebot_plugin_sparkapi-1.3.0/pyproject.toml` & `nonebot_plugin_sparkapi-1.4.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [project]
 name = "nonebot_plugin_sparkapi"
-version = "1.3.0"
+version = "1.4.0"
 description = "Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)"
 authors = [
     { name = "CCLMSY", email = "2502408581@qq.com" }
 ]
 dependencies = [
     "nonebot-adapter-onebot >=2.2.1, <3.0.0",
     "nonebot2 >=2.0.0rc3, <3.0.0",
-    "websockets >=12.0, <13.0"
+    "websockets >=12.0, <13.0",
+    "httpx >=0.19.0, <1.0.0",
+    "pillow >=10.0.0, <11.0.0",
 ]
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 readme = { file = "README.md", content-type = "text/markdown" }
 
 [build-system]
 requires = ["setuptools>=42", "wheel"]
```

