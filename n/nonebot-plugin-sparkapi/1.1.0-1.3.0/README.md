# Comparing `tmp/nonebot_plugin_sparkapi-1.1.0.tar.gz` & `tmp/nonebot_plugin_sparkapi-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sparkapi-1.1.0.tar", last modified: Fri May 17 12:45:02 2024, max compression
+gzip compressed data, was "nonebot_plugin_sparkapi-1.3.0.tar", last modified: Tue May 28 18:06:12 2024, max compression
```

## Comparing `nonebot_plugin_sparkapi-1.1.0.tar` & `nonebot_plugin_sparkapi-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:45:02.436154 nonebot_plugin_sparkapi-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-17 12:44:57.000000 nonebot_plugin_sparkapi-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-05-17 12:45:02.436154 nonebot_plugin_sparkapi-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-05-17 12:44:57.000000 nonebot_plugin_sparkapi-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:45:02.436154 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi/
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-17 12:44:57.000000 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi/SparkApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-17 12:44:57.000000 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-17 12:44:57.000000 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-17 12:44:57.000000 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi/funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-17 12:44:57.000000 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-17 12:44:57.000000 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi/slsessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:45:02.436154 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-05-17 12:45:02.000000 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-17 12:45:02.000000 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:45:02.000000 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-17 12:45:02.000000 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 12:45:02.000000 nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 12:44:57.000000 nonebot_plugin_sparkapi-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 12:45:02.436154 nonebot_plugin_sparkapi-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:12.616462 nonebot_plugin_sparkapi-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-28 18:06:12.616462 nonebot_plugin_sparkapi-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:12.612462 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/SparkApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:12.612462 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-28 18:06:12.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-28 18:06:12.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:06:12.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 18:06:12.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 18:06:12.000000 nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-28 18:06:08.000000 nonebot_plugin_sparkapi-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:06:12.616462 nonebot_plugin_sparkapi-1.3.0/setup.cfg
```

### Comparing `nonebot_plugin_sparkapi-1.1.0/LICENSE` & `nonebot_plugin_sparkapi-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.1.0/PKG-INFO` & `nonebot_plugin_sparkapi-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.1.0
+Version: 1.3.0
 Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,15 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
 Requires-Dist: websockets<13.0,>=12.0
 
 <div align="center">
@@ -60,23 +60,20 @@
 
 适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设等功能
 
 ### 💬 功能
 - [x] 支持AI对话
 - [x] 支持上下文关联记忆（可设置记忆文本长度）
 - [x] 用户鉴别（每个用户的历史记录独立）
-- [x] 支持使用、切换人物预设（prompt）
-- [x] 人物预设菜单自动生成，更改无需重写
-- [x] 功能菜单自动生成，更改无需重写
+- [x] 支持用户自定义、更改、切换预设（prompt）
+- [x] 自动生成人物预设菜单、帮助列表，无需重写
+- [x] 基于pickle的历史记录持久化
 - [x] 完善的配置项（有其他需求请发issue）
-- [x] 历史记录持久化
-- [ ] 实用功能列表（查天气、查快递等）
 - [ ] 用户权限与功能区分（超级用户、普通用户）
-- [ ] 支持星火助手API
-- [ ] 支持用户自定义、更改预设
+- [ ] 支持图片生成（ImageGeneration）
 
 ### 📦 项目地址
 - Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
 - 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
 
 ## 💿 安装
 
@@ -129,39 +126,46 @@
 |:-----:|:----:|:----:|:----:|
 | SPARKAPI_APP_ID | 是 | "" | APPID |
 | SPARKAPI_API_SECRET | 是 | "" | APISecret |
 | SPARKAPI_API_KEY | 是 | "" | APIKey |
 | SPARKAPI_MODEL_VERSION | 否 | "" | 星火大模型的版本，默认为当前最新。<br>可选值：v3.5, v3.0, v2.0, v1.5 |
 | SPARKAPI_MODEL_TOP_K | 否 | 4 | 平衡生成文本的质量和多样性。<br>较小的 k 值会减少随机性，使得输出更加稳定；<br>而较大的 k 值会增加随机性，产生更多新颖的输出。<br>取值范围[1, 6] |
 | SPARKAPI_MODEL_TEMPERATURE | 否 | 0.5 | 控制结果随机性，取值越高随机性越强，即相同的问题得到的不同答案的可能性越高。<br>取值范围 (0，1] |
-| SPARKAPI_COMMAND_CHAT | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空<br>COMMAND_START = [""]） |
-| SPARKAPI_PRIVATE_CHAT | 否 | True | 是否允许私聊使用 |
-| SPARKAPI_GROUP_PUBLIC | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
-| SPARKAPI_GROUP_AT | 否 | True | 群聊回复消息时是否需要@提问者 |
-| SPARKAPI_FNOTICE | 否 | True | 收到请求时是否提示“已收到请求” |
-| SPARKAPI_PRIORITY | 否 | 90 | 聊天事件响应器优先级，[1,99]，数字越小优先级越高 |
-| SPARKPAI_MAX_LENGTH | 否 | 8000 | 上下文最大长度，[1,8000]<br>单次发送和回复的消息不能超过该项的一半 |
-| SPARKAPI_SETPRESET_CLEAR | 否 | True | 切换人物预设时是否清除当前对话上下文 |
+| SPARKAPI_MODEL_MAXKLENGTH | 否 | 8000 | 上下文最大长度，[1,8000]<br>单次发送和回复的消息不能超过该项的一半 |
+| SPARKAPI_PRIORITY | 否 | 80 | 该值越小，事件越先被触发。本插件建议设置较大的值。可选值：1~97<br>若触发本插件事件，所有插件中优先级大于此值的事件都将被阻断。<br>本插件中事件的优先级顺序：私聊阻断（=priority）< 功能（=priority+1）< 对话（=priority+2） |
+| SPARKAPI_COMMANDS__CHAT | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空：COMMAND_START = [""]） |
+| SPARKAPI_FL_NOTICE | 否 | True | 收到请求时是否提示“已收到请求” |
+| SPARKAPI_FL_SETPRESET_CLEAR | 否 | True | 切换人物预设时是否清除当前对话上下文 |
+| SPARKAPI_FL_PRIVATE_CHAT | 否 | True | 是否允许私聊使用 |
+| SPARKAPI_FL_GROUP_PUBLIC | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
+| SPARKAPI_FL_GROUP_AT | 否 | True | 群聊回复消息时是否需要@提问者 |
 | SPARKAPI_BOT_NAME | 否 | "" | 机器人的名字 |
 
+以下配置项请查看`/.venv/Lib/nonebot_plugin_sparkapi/config.py`修改：
+1. sparkapi_commands：指令表（允许单个字符串或字符串列表）
+2. sparkapi_commands_info：指令表说明（用于生成帮助信息）
+3. sparkapi_message_blockprivate：阻断私聊时的提示信息
 
 ## 🎉 使用
-### 指令表
-所有指令均可在config.py中修改，且无需重写菜单/指令生成函数
+### 指令表（默认）
+以下所有指令均可在config.py中修改，且无需重写菜单/指令生成函数
 
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | SPARKAPI_COMMAND_CHAT（若不为空） + 对话内容 | 是 | 私聊/群聊 | 与机器人进行对话 |
-| help | 是 | 私聊/群聊 | 查看帮助信息 |
-| presets | 是 | 私聊/群聊 | 查看当前可选的人物预设 |
-| set | 是 | 私聊/群聊 | 查看当前可选的人物预设<br>回复编号以进行切换 |
-| set + 人物预设编号 | 是 | 私聊/群聊 | 切换到编号对应的人物预设 |
-| save | 是 | 私聊/群聊 | 保存当前对话上下文 |
-| load | 是 | 私聊/群聊 | 加载之前保存的对话上下文 |
-| clear | 是 | 私聊/群聊 | 清除当前对话上下文 |
+| help/帮助 | 是 | 私聊/群聊 | 显示帮助信息 |
+| preset/人物预设 | 是 | 私聊/群聊 | 显示人物预设菜单和当前预设 |
+| set/切换预设 | 是 | 私聊/群聊 | 显示人物预设菜单，选择并切换 |
+| set/切换预设 + 人物名 | 是 | 私聊/群聊 | 切换人物预设 |
+| create/创建预设 | 是 | 私聊/群聊 | 创建自定义的人物预设 |
+| delete/删除预设 | 是 | 私聊/群聊 | 删除自定义的人物预设 |
+| delete/删除预设 + 人物名 | 是 | 私聊/群聊 | 显示自定义人物预设菜单, 选择并删除 |
+| clear/清空对话 | 是 | 私聊/群聊 | 清除当前对话上下文 |
+| save/保存对话 | 是 | 私聊/群聊 | 保存当前对话记录 |
+| load/加载对话 | 是 | 私聊/群聊 | 加载上次保存的对话记录 |
 
 ### 人物预设
 1. 智能助手（默认）
 2. 心理咨询师
 
 ### 效果图
 ![demo](https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.3.0 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -11,83 +11,93 @@
 permission notice shall be included in all copies or substantial portions of
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Requires-Python: >=3.8 Description-Content-Type:
+DEALINGS IN THE SOFTWARE. Requires-Python: >=3.10 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: nonebot-adapter-
 onebot<3.0.0,>=2.2.1 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3 Requires-Dist:
 websockets<13.0,>=12.0
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
-æ¯æä½¿ç¨ãåæ¢äººç©é¢è®¾ï¼promptï¼ - [x]
-äººç©é¢è®¾èåèªå¨çæï¼æ´æ¹æ ééå - [x]
-åè½èåèªå¨çæï¼æ´æ¹æ ééå - [x]
-å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [x] åå²è®°å½æä¹å
-- [ ] å®ç¨åè½åè¡¨ï¼æ¥å¤©æ°ãæ¥å¿«éç­ï¼ - [ ]
+æ¯æç¨æ·èªå®ä¹ãæ´æ¹ãåæ¢é¢è®¾ï¼promptï¼ - [x]
+èªå¨çæäººç©é¢è®¾èåãå¸®å©åè¡¨ï¼æ ééå - [x]
+åºäºpickleçåå²è®°å½æä¹å - [x]
+å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [ ]
 ç¨æ·æéä¸åè½åºåï¼è¶çº§ç¨æ·ãæ®éç¨æ·ï¼ - [ ]
-æ¯ææç«å©æAPI - [ ] æ¯æç¨æ·èªå®ä¹ãæ´æ¹é¢è®¾ ### ð¦
-é¡¹ç®å°å - Githubï¼https://github.com/CCLMSY/nonebot-plugin-sparkapi -
-è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-
-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-sparkapi
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip pip install nonebot-plugin-sparkapi pdm pdm add nonebot-plugin-sparkapi
-poetry poetry add nonebot-plugin-sparkapi conda conda install nonebot-plugin-
-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
-[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_sparkapi"] ##
-âï¸ éç½® å¨ nonebot2
+æ¯æå¾ççæï¼ImageGenerationï¼ ### ð¦ é¡¹ç®å°å - Githubï¼https:
+//github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
+Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
+install nonebot-plugin-sparkapi ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
+é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
+è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-sparkapi pdm pdm add
+nonebot-plugin-sparkapi poetry poetry add nonebot-plugin-sparkapi conda conda
+install nonebot-plugin-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
+`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
+["nonebot_plugin_sparkapi"] ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
 å¶ä¸­ï¼æå¡æ¥å£è®¤è¯ä¿¡æ¯ app_id, api_secret, api_key è¯·åå¾
 [è®¯é£å¼æ¾å¹³å°æ§å¶å°](https://console.xfyun.cn/) è·å | éç½®é¡¹ |
 å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | SPARKAPI_APP_ID
 | æ¯ | "" | APPID | | SPARKAPI_API_SECRET | æ¯ | "" | APISecret | |
 SPARKAPI_API_KEY | æ¯ | "" | APIKey | | SPARKAPI_MODEL_VERSION | å¦ | "" |
 æç«å¤§æ¨¡åççæ¬ï¼é»è®¤ä¸ºå½åææ°ã
 å¯éå¼ï¼v3.5, v3.0, v2.0, v1.5 | | SPARKAPI_MODEL_TOP_K | å¦ | 4 |
 å¹³è¡¡çæææ¬çè´¨éåå¤æ ·æ§ã
 è¾å°ç k å¼ä¼åå°éæºæ§ï¼ä½¿å¾è¾åºæ´å ç¨³å®ï¼
 èè¾å¤§ç k å¼ä¼å¢å éæºæ§ï¼äº§çæ´å¤æ°é¢çè¾åºã
 åå¼èå´[1, 6] | | SPARKAPI_MODEL_TEMPERATURE | å¦ | 0.5 |
 æ§å¶ç»æéæºæ§ï¼åå¼è¶é«éæºæ§è¶å¼ºï¼å³ç¸åçé®é¢å¾å°çä¸åç­æ¡çå¯è½æ§è¶é«ã
-åå¼èå´ (0ï¼1] | | SPARKAPI_COMMAND_CHAT | å¦ | "" |
-æºå¨äººå¯¹è¯æä»¤ï¼é»è®¤ä¸ºç©ºå¯ç´æ¥å¯¹è¯
-ï¼éè¦åæ¶å¨`.env`ä¸­éç½®å½ä»¤èµ·å§å­ç¬¦ä¸ºç©º
-COMMAND_START = [""]ï¼ | | SPARKAPI_PRIVATE_CHAT | å¦ | True |
-æ¯å¦åè®¸ç§èä½¿ç¨ | | SPARKAPI_GROUP_PUBLIC | å¦ | False |
-ç¾¤èå¯ç¨å¬å±ä¼è¯
+åå¼èå´ (0ï¼1] | | SPARKAPI_MODEL_MAXKLENGTH | å¦ | 8000 |
+ä¸ä¸ææå¤§é¿åº¦ï¼[1,8000]
+åæ¬¡åéååå¤çæ¶æ¯ä¸è½è¶è¿è¯¥é¡¹çä¸å | | SPARKAPI_PRIORITY
+| å¦ | 80 |
+è¯¥å¼è¶å°ï¼äºä»¶è¶åè¢«è§¦åãæ¬æä»¶å»ºè®®è®¾ç½®è¾å¤§çå¼ãå¯éå¼ï¼1~97
+è¥è§¦åæ¬æä»¶äºä»¶ï¼æææä»¶ä¸­ä¼åçº§å¤§äºæ­¤å¼çäºä»¶é½å°è¢«é»æ­ã
+æ¬æä»¶ä¸­äºä»¶çä¼åçº§é¡ºåºï¼ç§èé»æ­ï¼=priorityï¼<
+åè½ï¼=priority+1ï¼< å¯¹è¯ï¼=priority+2ï¼ | | SPARKAPI_COMMANDS__CHAT |
+å¦ | "" | æºå¨äººå¯¹è¯æä»¤ï¼é»è®¤ä¸ºç©ºå¯ç´æ¥å¯¹è¯
+ï¼éè¦åæ¶å¨`.env`ä¸­éç½®å½ä»¤èµ·å§å­ç¬¦ä¸ºç©ºï¼COMMAND_START =
+[""]ï¼ | | SPARKAPI_FL_NOTICE | å¦ | True |
+æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | |
+SPARKAPI_FL_SETPRESET_CLEAR | å¦ | True |
+åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | |
+SPARKAPI_FL_PRIVATE_CHAT | å¦ | True | æ¯å¦åè®¸ç§èä½¿ç¨ | |
+SPARKAPI_FL_GROUP_PUBLIC | å¦ | False | ç¾¤èå¯ç¨å¬å±ä¼è¯
 Trueï¼ææäººå±äº«åä¸ä¼è¯
-Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | SPARKAPI_GROUP_AT | å¦ | True |
-ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_FNOTICE | å¦ | True |
-æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | | SPARKAPI_PRIORITY | å¦ |
-90 | èå¤©äºä»¶ååºå¨ä¼åçº§ï¼[1,99]ï¼æ°å­è¶å°ä¼åçº§è¶é« | |
-SPARKPAI_MAX_LENGTH | å¦ | 8000 | ä¸ä¸ææå¤§é¿åº¦ï¼[1,8000]
-åæ¬¡åéååå¤çæ¶æ¯ä¸è½è¶è¿è¯¥é¡¹çä¸å | |
-SPARKAPI_SETPRESET_CLEAR | å¦ | True |
-åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | SPARKAPI_BOT_NAME |
-å¦ | "" | æºå¨äººçåå­ | ## ð ä½¿ç¨ ### æä»¤è¡¨
-æææä»¤åå¯å¨config.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
+Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | SPARKAPI_FL_GROUP_AT | å¦ | True |
+ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_BOT_NAME | å¦ | "" |
+æºå¨äººçåå­ | ä»¥ä¸éç½®é¡¹è¯·æ¥ç`/.venv/Lib/
+nonebot_plugin_sparkapi/config.py`ä¿®æ¹ï¼ 1.
+sparkapi_commandsï¼æä»¤è¡¨ï¼åè®¸åä¸ªå­ç¬¦ä¸²æå­ç¬¦ä¸²åè¡¨ï¼ 2.
+sparkapi_commands_infoï¼æä»¤è¡¨è¯´æï¼ç¨äºçæå¸®å©ä¿¡æ¯ï¼ 3.
+sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
+### æä»¤è¡¨ï¼é»è®¤ï¼
+ä»¥ä¸æææä»¤åå¯å¨config.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
 æä»¤çæå½æ° | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:| | SPARKAPI_COMMAND_CHATï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ |
-ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help | æ¯ | ç§è/ç¾¤è |
-æ¥çå¸®å©ä¿¡æ¯ | | presets | æ¯ | ç§è/ç¾¤è |
-æ¥çå½åå¯éçäººç©é¢è®¾ | | set | æ¯ | ç§è/ç¾¤è |
-æ¥çå½åå¯éçäººç©é¢è®¾
-åå¤ç¼å·ä»¥è¿è¡åæ¢ | | set + äººç©é¢è®¾ç¼å· | æ¯ | ç§è/ç¾¤è
-| åæ¢å°ç¼å·å¯¹åºçäººç©é¢è®¾ | | save | æ¯ | ç§è/ç¾¤è |
-ä¿å­å½åå¯¹è¯ä¸ä¸æ | | load | æ¯ | ç§è/ç¾¤è |
-å è½½ä¹åä¿å­çå¯¹è¯ä¸ä¸æ | | clear | æ¯ | ç§è/ç¾¤è |
-æ¸é¤å½åå¯¹è¯ä¸ä¸æ | ### äººç©é¢è®¾ 1. æºè½å©æï¼é»è®¤ï¼ 2.
-å¿çå¨è¯¢å¸ ### ææå¾ ![demo](https://github.com/CCLMSY/nonebot-plugin-
-sparkapi/blob/resources/demo.jpg)
+ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help/å¸®å© | æ¯ | ç§è/ç¾¤è
+| æ¾ç¤ºå¸®å©ä¿¡æ¯ | | preset/äººç©é¢è®¾ | æ¯ | ç§è/ç¾¤è |
+æ¾ç¤ºäººç©é¢è®¾èååå½åé¢è®¾ | | set/åæ¢é¢è®¾ | æ¯ | ç§è/
+ç¾¤è | æ¾ç¤ºäººç©é¢è®¾èåï¼éæ©å¹¶åæ¢ | | set/åæ¢é¢è®¾ +
+äººç©å | æ¯ | ç§è/ç¾¤è | åæ¢äººç©é¢è®¾ | | create/åå»ºé¢è®¾ |
+æ¯ | ç§è/ç¾¤è | åå»ºèªå®ä¹çäººç©é¢è®¾ | | delete/å é¤é¢è®¾ |
+æ¯ | ç§è/ç¾¤è | å é¤èªå®ä¹çäººç©é¢è®¾ | | delete/å é¤é¢è®¾ +
+äººç©å | æ¯ | ç§è/ç¾¤è | æ¾ç¤ºèªå®ä¹äººç©é¢è®¾èå,
+éæ©å¹¶å é¤ | | clear/æ¸ç©ºå¯¹è¯ | æ¯ | ç§è/ç¾¤è |
+æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | save/ä¿å­å¯¹è¯ | æ¯ | ç§è/ç¾¤è |
+ä¿å­å½åå¯¹è¯è®°å½ | | load/å è½½å¯¹è¯ | æ¯ | ç§è/ç¾¤è |
+å è½½ä¸æ¬¡ä¿å­çå¯¹è¯è®°å½ | ### äººç©é¢è®¾ 1.
+æºè½å©æï¼é»è®¤ï¼ 2. å¿çå¨è¯¢å¸ ### ææå¾ ![demo](https://
+github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

### Comparing `nonebot_plugin_sparkapi-1.1.0/README.md` & `nonebot_plugin_sparkapi-1.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -26,23 +26,20 @@
 
 适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设等功能
 
 ### 💬 功能
 - [x] 支持AI对话
 - [x] 支持上下文关联记忆（可设置记忆文本长度）
 - [x] 用户鉴别（每个用户的历史记录独立）
-- [x] 支持使用、切换人物预设（prompt）
-- [x] 人物预设菜单自动生成，更改无需重写
-- [x] 功能菜单自动生成，更改无需重写
+- [x] 支持用户自定义、更改、切换预设（prompt）
+- [x] 自动生成人物预设菜单、帮助列表，无需重写
+- [x] 基于pickle的历史记录持久化
 - [x] 完善的配置项（有其他需求请发issue）
-- [x] 历史记录持久化
-- [ ] 实用功能列表（查天气、查快递等）
 - [ ] 用户权限与功能区分（超级用户、普通用户）
-- [ ] 支持星火助手API
-- [ ] 支持用户自定义、更改预设
+- [ ] 支持图片生成（ImageGeneration）
 
 ### 📦 项目地址
 - Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
 - 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
 
 ## 💿 安装
 
@@ -95,39 +92,46 @@
 |:-----:|:----:|:----:|:----:|
 | SPARKAPI_APP_ID | 是 | "" | APPID |
 | SPARKAPI_API_SECRET | 是 | "" | APISecret |
 | SPARKAPI_API_KEY | 是 | "" | APIKey |
 | SPARKAPI_MODEL_VERSION | 否 | "" | 星火大模型的版本，默认为当前最新。<br>可选值：v3.5, v3.0, v2.0, v1.5 |
 | SPARKAPI_MODEL_TOP_K | 否 | 4 | 平衡生成文本的质量和多样性。<br>较小的 k 值会减少随机性，使得输出更加稳定；<br>而较大的 k 值会增加随机性，产生更多新颖的输出。<br>取值范围[1, 6] |
 | SPARKAPI_MODEL_TEMPERATURE | 否 | 0.5 | 控制结果随机性，取值越高随机性越强，即相同的问题得到的不同答案的可能性越高。<br>取值范围 (0，1] |
-| SPARKAPI_COMMAND_CHAT | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空<br>COMMAND_START = [""]） |
-| SPARKAPI_PRIVATE_CHAT | 否 | True | 是否允许私聊使用 |
-| SPARKAPI_GROUP_PUBLIC | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
-| SPARKAPI_GROUP_AT | 否 | True | 群聊回复消息时是否需要@提问者 |
-| SPARKAPI_FNOTICE | 否 | True | 收到请求时是否提示“已收到请求” |
-| SPARKAPI_PRIORITY | 否 | 90 | 聊天事件响应器优先级，[1,99]，数字越小优先级越高 |
-| SPARKPAI_MAX_LENGTH | 否 | 8000 | 上下文最大长度，[1,8000]<br>单次发送和回复的消息不能超过该项的一半 |
-| SPARKAPI_SETPRESET_CLEAR | 否 | True | 切换人物预设时是否清除当前对话上下文 |
+| SPARKAPI_MODEL_MAXKLENGTH | 否 | 8000 | 上下文最大长度，[1,8000]<br>单次发送和回复的消息不能超过该项的一半 |
+| SPARKAPI_PRIORITY | 否 | 80 | 该值越小，事件越先被触发。本插件建议设置较大的值。可选值：1~97<br>若触发本插件事件，所有插件中优先级大于此值的事件都将被阻断。<br>本插件中事件的优先级顺序：私聊阻断（=priority）< 功能（=priority+1）< 对话（=priority+2） |
+| SPARKAPI_COMMANDS__CHAT | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空：COMMAND_START = [""]） |
+| SPARKAPI_FL_NOTICE | 否 | True | 收到请求时是否提示“已收到请求” |
+| SPARKAPI_FL_SETPRESET_CLEAR | 否 | True | 切换人物预设时是否清除当前对话上下文 |
+| SPARKAPI_FL_PRIVATE_CHAT | 否 | True | 是否允许私聊使用 |
+| SPARKAPI_FL_GROUP_PUBLIC | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
+| SPARKAPI_FL_GROUP_AT | 否 | True | 群聊回复消息时是否需要@提问者 |
 | SPARKAPI_BOT_NAME | 否 | "" | 机器人的名字 |
 
+以下配置项请查看`/.venv/Lib/nonebot_plugin_sparkapi/config.py`修改：
+1. sparkapi_commands：指令表（允许单个字符串或字符串列表）
+2. sparkapi_commands_info：指令表说明（用于生成帮助信息）
+3. sparkapi_message_blockprivate：阻断私聊时的提示信息
 
 ## 🎉 使用
-### 指令表
-所有指令均可在config.py中修改，且无需重写菜单/指令生成函数
+### 指令表（默认）
+以下所有指令均可在config.py中修改，且无需重写菜单/指令生成函数
 
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | SPARKAPI_COMMAND_CHAT（若不为空） + 对话内容 | 是 | 私聊/群聊 | 与机器人进行对话 |
-| help | 是 | 私聊/群聊 | 查看帮助信息 |
-| presets | 是 | 私聊/群聊 | 查看当前可选的人物预设 |
-| set | 是 | 私聊/群聊 | 查看当前可选的人物预设<br>回复编号以进行切换 |
-| set + 人物预设编号 | 是 | 私聊/群聊 | 切换到编号对应的人物预设 |
-| save | 是 | 私聊/群聊 | 保存当前对话上下文 |
-| load | 是 | 私聊/群聊 | 加载之前保存的对话上下文 |
-| clear | 是 | 私聊/群聊 | 清除当前对话上下文 |
+| help/帮助 | 是 | 私聊/群聊 | 显示帮助信息 |
+| preset/人物预设 | 是 | 私聊/群聊 | 显示人物预设菜单和当前预设 |
+| set/切换预设 | 是 | 私聊/群聊 | 显示人物预设菜单，选择并切换 |
+| set/切换预设 + 人物名 | 是 | 私聊/群聊 | 切换人物预设 |
+| create/创建预设 | 是 | 私聊/群聊 | 创建自定义的人物预设 |
+| delete/删除预设 | 是 | 私聊/群聊 | 删除自定义的人物预设 |
+| delete/删除预设 + 人物名 | 是 | 私聊/群聊 | 显示自定义人物预设菜单, 选择并删除 |
+| clear/清空对话 | 是 | 私聊/群聊 | 清除当前对话上下文 |
+| save/保存对话 | 是 | 私聊/群聊 | 保存当前对话记录 |
+| load/加载对话 | 是 | 私聊/群聊 | 加载上次保存的对话记录 |
 
 ### 人物预设
 1. 智能助手（默认）
 2. 心理咨询师
 
 ### 效果图
 ![demo](https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

#### html2text {}

```diff
@@ -5,68 +5,78 @@
                                    [python]
 ## ð ä»ç»
 åºäºNonebot2å¹³å°ï¼è°ç¨ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIçAIèå¤©æºå¨äººæä»¶
 éç¨äºæææ¨¡åçæ¬ï¼é»è®¤å½åææ°ï¼v3.5ï¼ï¼ï¼æ¯æä¸ä¸æå³èãäººç©é¢è®¾ç­åè½
 ### ð¬ åè½ - [x] æ¯æAIå¯¹è¯ - [x]
 æ¯æä¸ä¸æå³èè®°å¿ï¼å¯è®¾ç½®è®°å¿ææ¬é¿åº¦ï¼ - [x]
 ç¨æ·é´å«ï¼æ¯ä¸ªç¨æ·çåå²è®°å½ç¬ç«ï¼ - [x]
-æ¯æä½¿ç¨ãåæ¢äººç©é¢è®¾ï¼promptï¼ - [x]
-äººç©é¢è®¾èåèªå¨çæï¼æ´æ¹æ ééå - [x]
-åè½èåèªå¨çæï¼æ´æ¹æ ééå - [x]
-å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [x] åå²è®°å½æä¹å
-- [ ] å®ç¨åè½åè¡¨ï¼æ¥å¤©æ°ãæ¥å¿«éç­ï¼ - [ ]
+æ¯æç¨æ·èªå®ä¹ãæ´æ¹ãåæ¢é¢è®¾ï¼promptï¼ - [x]
+èªå¨çæäººç©é¢è®¾èåãå¸®å©åè¡¨ï¼æ ééå - [x]
+åºäºpickleçåå²è®°å½æä¹å - [x]
+å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [ ]
 ç¨æ·æéä¸åè½åºåï¼è¶çº§ç¨æ·ãæ®éç¨æ·ï¼ - [ ]
-æ¯ææç«å©æAPI - [ ] æ¯æç¨æ·èªå®ä¹ãæ´æ¹é¢è®¾ ### ð¦
-é¡¹ç®å°å - Githubï¼https://github.com/CCLMSY/nonebot-plugin-sparkapi -
-è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-
-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-sparkapi
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip pip install nonebot-plugin-sparkapi pdm pdm add nonebot-plugin-sparkapi
-poetry poetry add nonebot-plugin-sparkapi conda conda install nonebot-plugin-
-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
-[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_sparkapi"] ##
-âï¸ éç½® å¨ nonebot2
+æ¯æå¾ççæï¼ImageGenerationï¼ ### ð¦ é¡¹ç®å°å - Githubï¼https:
+//github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
+Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
+install nonebot-plugin-sparkapi ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
+é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
+è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-sparkapi pdm pdm add
+nonebot-plugin-sparkapi poetry poetry add nonebot-plugin-sparkapi conda conda
+install nonebot-plugin-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
+`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
+["nonebot_plugin_sparkapi"] ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
 å¶ä¸­ï¼æå¡æ¥å£è®¤è¯ä¿¡æ¯ app_id, api_secret, api_key è¯·åå¾
 [è®¯é£å¼æ¾å¹³å°æ§å¶å°](https://console.xfyun.cn/) è·å | éç½®é¡¹ |
 å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | SPARKAPI_APP_ID
 | æ¯ | "" | APPID | | SPARKAPI_API_SECRET | æ¯ | "" | APISecret | |
 SPARKAPI_API_KEY | æ¯ | "" | APIKey | | SPARKAPI_MODEL_VERSION | å¦ | "" |
 æç«å¤§æ¨¡åççæ¬ï¼é»è®¤ä¸ºå½åææ°ã
 å¯éå¼ï¼v3.5, v3.0, v2.0, v1.5 | | SPARKAPI_MODEL_TOP_K | å¦ | 4 |
 å¹³è¡¡çæææ¬çè´¨éåå¤æ ·æ§ã
 è¾å°ç k å¼ä¼åå°éæºæ§ï¼ä½¿å¾è¾åºæ´å ç¨³å®ï¼
 èè¾å¤§ç k å¼ä¼å¢å éæºæ§ï¼äº§çæ´å¤æ°é¢çè¾åºã
 åå¼èå´[1, 6] | | SPARKAPI_MODEL_TEMPERATURE | å¦ | 0.5 |
 æ§å¶ç»æéæºæ§ï¼åå¼è¶é«éæºæ§è¶å¼ºï¼å³ç¸åçé®é¢å¾å°çä¸åç­æ¡çå¯è½æ§è¶é«ã
-åå¼èå´ (0ï¼1] | | SPARKAPI_COMMAND_CHAT | å¦ | "" |
-æºå¨äººå¯¹è¯æä»¤ï¼é»è®¤ä¸ºç©ºå¯ç´æ¥å¯¹è¯
-ï¼éè¦åæ¶å¨`.env`ä¸­éç½®å½ä»¤èµ·å§å­ç¬¦ä¸ºç©º
-COMMAND_START = [""]ï¼ | | SPARKAPI_PRIVATE_CHAT | å¦ | True |
-æ¯å¦åè®¸ç§èä½¿ç¨ | | SPARKAPI_GROUP_PUBLIC | å¦ | False |
-ç¾¤èå¯ç¨å¬å±ä¼è¯
+åå¼èå´ (0ï¼1] | | SPARKAPI_MODEL_MAXKLENGTH | å¦ | 8000 |
+ä¸ä¸ææå¤§é¿åº¦ï¼[1,8000]
+åæ¬¡åéååå¤çæ¶æ¯ä¸è½è¶è¿è¯¥é¡¹çä¸å | | SPARKAPI_PRIORITY
+| å¦ | 80 |
+è¯¥å¼è¶å°ï¼äºä»¶è¶åè¢«è§¦åãæ¬æä»¶å»ºè®®è®¾ç½®è¾å¤§çå¼ãå¯éå¼ï¼1~97
+è¥è§¦åæ¬æä»¶äºä»¶ï¼æææä»¶ä¸­ä¼åçº§å¤§äºæ­¤å¼çäºä»¶é½å°è¢«é»æ­ã
+æ¬æä»¶ä¸­äºä»¶çä¼åçº§é¡ºåºï¼ç§èé»æ­ï¼=priorityï¼<
+åè½ï¼=priority+1ï¼< å¯¹è¯ï¼=priority+2ï¼ | | SPARKAPI_COMMANDS__CHAT |
+å¦ | "" | æºå¨äººå¯¹è¯æä»¤ï¼é»è®¤ä¸ºç©ºå¯ç´æ¥å¯¹è¯
+ï¼éè¦åæ¶å¨`.env`ä¸­éç½®å½ä»¤èµ·å§å­ç¬¦ä¸ºç©ºï¼COMMAND_START =
+[""]ï¼ | | SPARKAPI_FL_NOTICE | å¦ | True |
+æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | |
+SPARKAPI_FL_SETPRESET_CLEAR | å¦ | True |
+åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | |
+SPARKAPI_FL_PRIVATE_CHAT | å¦ | True | æ¯å¦åè®¸ç§èä½¿ç¨ | |
+SPARKAPI_FL_GROUP_PUBLIC | å¦ | False | ç¾¤èå¯ç¨å¬å±ä¼è¯
 Trueï¼ææäººå±äº«åä¸ä¼è¯
-Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | SPARKAPI_GROUP_AT | å¦ | True |
-ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_FNOTICE | å¦ | True |
-æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | | SPARKAPI_PRIORITY | å¦ |
-90 | èå¤©äºä»¶ååºå¨ä¼åçº§ï¼[1,99]ï¼æ°å­è¶å°ä¼åçº§è¶é« | |
-SPARKPAI_MAX_LENGTH | å¦ | 8000 | ä¸ä¸ææå¤§é¿åº¦ï¼[1,8000]
-åæ¬¡åéååå¤çæ¶æ¯ä¸è½è¶è¿è¯¥é¡¹çä¸å | |
-SPARKAPI_SETPRESET_CLEAR | å¦ | True |
-åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | SPARKAPI_BOT_NAME |
-å¦ | "" | æºå¨äººçåå­ | ## ð ä½¿ç¨ ### æä»¤è¡¨
-æææä»¤åå¯å¨config.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
+Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | SPARKAPI_FL_GROUP_AT | å¦ | True |
+ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_BOT_NAME | å¦ | "" |
+æºå¨äººçåå­ | ä»¥ä¸éç½®é¡¹è¯·æ¥ç`/.venv/Lib/
+nonebot_plugin_sparkapi/config.py`ä¿®æ¹ï¼ 1.
+sparkapi_commandsï¼æä»¤è¡¨ï¼åè®¸åä¸ªå­ç¬¦ä¸²æå­ç¬¦ä¸²åè¡¨ï¼ 2.
+sparkapi_commands_infoï¼æä»¤è¡¨è¯´æï¼ç¨äºçæå¸®å©ä¿¡æ¯ï¼ 3.
+sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
+### æä»¤è¡¨ï¼é»è®¤ï¼
+ä»¥ä¸æææä»¤åå¯å¨config.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
 æä»¤çæå½æ° | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:| | SPARKAPI_COMMAND_CHATï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ |
-ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help | æ¯ | ç§è/ç¾¤è |
-æ¥çå¸®å©ä¿¡æ¯ | | presets | æ¯ | ç§è/ç¾¤è |
-æ¥çå½åå¯éçäººç©é¢è®¾ | | set | æ¯ | ç§è/ç¾¤è |
-æ¥çå½åå¯éçäººç©é¢è®¾
-åå¤ç¼å·ä»¥è¿è¡åæ¢ | | set + äººç©é¢è®¾ç¼å· | æ¯ | ç§è/ç¾¤è
-| åæ¢å°ç¼å·å¯¹åºçäººç©é¢è®¾ | | save | æ¯ | ç§è/ç¾¤è |
-ä¿å­å½åå¯¹è¯ä¸ä¸æ | | load | æ¯ | ç§è/ç¾¤è |
-å è½½ä¹åä¿å­çå¯¹è¯ä¸ä¸æ | | clear | æ¯ | ç§è/ç¾¤è |
-æ¸é¤å½åå¯¹è¯ä¸ä¸æ | ### äººç©é¢è®¾ 1. æºè½å©æï¼é»è®¤ï¼ 2.
-å¿çå¨è¯¢å¸ ### ææå¾ ![demo](https://github.com/CCLMSY/nonebot-plugin-
-sparkapi/blob/resources/demo.jpg)
+ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help/å¸®å© | æ¯ | ç§è/ç¾¤è
+| æ¾ç¤ºå¸®å©ä¿¡æ¯ | | preset/äººç©é¢è®¾ | æ¯ | ç§è/ç¾¤è |
+æ¾ç¤ºäººç©é¢è®¾èååå½åé¢è®¾ | | set/åæ¢é¢è®¾ | æ¯ | ç§è/
+ç¾¤è | æ¾ç¤ºäººç©é¢è®¾èåï¼éæ©å¹¶åæ¢ | | set/åæ¢é¢è®¾ +
+äººç©å | æ¯ | ç§è/ç¾¤è | åæ¢äººç©é¢è®¾ | | create/åå»ºé¢è®¾ |
+æ¯ | ç§è/ç¾¤è | åå»ºèªå®ä¹çäººç©é¢è®¾ | | delete/å é¤é¢è®¾ |
+æ¯ | ç§è/ç¾¤è | å é¤èªå®ä¹çäººç©é¢è®¾ | | delete/å é¤é¢è®¾ +
+äººç©å | æ¯ | ç§è/ç¾¤è | æ¾ç¤ºèªå®ä¹äººç©é¢è®¾èå,
+éæ©å¹¶å é¤ | | clear/æ¸ç©ºå¯¹è¯ | æ¯ | ç§è/ç¾¤è |
+æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | save/ä¿å­å¯¹è¯ | æ¯ | ç§è/ç¾¤è |
+ä¿å­å½åå¯¹è¯è®°å½ | | load/å è½½å¯¹è¯ | æ¯ | ç§è/ç¾¤è |
+å è½½ä¸æ¬¡ä¿å­çå¯¹è¯è®°å½ | ### äººç©é¢è®¾ 1.
+æºè½å©æï¼é»è®¤ï¼ 2. å¿çå¨è¯¢å¸ ### ææå¾ ![demo](https://
+github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

### Comparing `nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi/SparkApi.py` & `nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/SparkApi.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,23 @@
 from time import mktime
 from wsgiref.handlers import format_date_time
 from urllib.parse import urlparse, urlencode
 
 import hmac
 import hashlib
 import base64
-
 import json
 import websockets
 
 from .config import Config
-from nonebot import get_driver
-
-conf = Config.parse_obj(get_driver().config.dict())
-
+from nonebot import get_plugin_config
+conf = get_plugin_config(Config)
 model_top_k = conf.sparkapi_model_top_k
 model_temperature = conf.sparkapi_model_temperature
-max_length = conf.sparkpai_max_length
+maxlength = conf.sparkpai_model_maxlength
 
 answer = ""
 
 class Ws_Param(object):
     # 初始化
     def __init__(self, APPID, APIKey, APISecret, Spark_url):
         self.APPID = APPID
@@ -60,15 +57,14 @@
         url = self.Spark_url + '?' + urlencode(v)
 
         # print("APPID: " + self.APPID)
         # print("APIKey: " + self.APIKey)
         # print("APISecret: " + self.APISecret)
         # print("signature_origin: " + signature_origin)
         # print(url)
-        # 此处打印出建立连接时候的url,参考本demo的时候可取消上方打印的注释，比对相同参数时生成的url与自己代码生成的url是否一致
         return url
 
 # 收到websockets消息的处理
 async def on_message(ws, message):
     # print(message)
     data = json.loads(message)
     code = data['header']['code']
@@ -88,17 +84,14 @@
         # print(1)
         if status == 2:
             await ws.close()
 
 async def connect_ws(appid, api_key, api_secret, Spark_url, domain, question, sid):
     wsParam = Ws_Param(appid, api_key, api_secret, Spark_url)
     ws_url = wsParam.create_url()
-    # ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
-    # ssl_context.check_hostname = False
-    # ssl_context.verify_mode = ssl.CERT_NONE
 
     async with websockets.connect(ws_url) as ws:
         ws.appid = appid
         ws.question = question
         ws.domain = domain
         ws.sid = sid
         await ws.send(json.dumps(gen_params(appid, domain, question)))
@@ -111,15 +104,15 @@
             "app_id": appid,
             "uid": "1234"
         },
         "parameter": {
             "chat": {
                 "domain": domain,
                 "temperature": model_temperature,
-                "max_tokens": max_length // 2,
+                "max_tokens": maxlength // 2,
                 "top_k": model_top_k,
                 "auditing": "default"
             }
         },
         "payload": {
             "message": {
                 "text": question
```

### Comparing `nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi/config.py` & `nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 from pydantic import BaseModel
-from typing import Optional
 
 class Config(BaseModel):
-    # 讯飞开放平台控制台中的 服务接口认证信息
-    sparkapi_app_id: Optional[str] = "" # APP ID
-    sparkapi_api_secret: Optional[str] = "" # API Secret
-    sparkapi_api_key: Optional[str] = "" # API Key
+    # API信息：讯飞开放平台控制台（https://console.xfyun.cn/）中的“服务接口认证信息”
+    sparkapi_app_id: str = "" # APP ID
+    sparkapi_api_secret: str = "" # API Secret
+    sparkapi_api_key: str = "" # API Key
 
+    # 模型设置
     sparkapi_model_version: str = "" # 星火大模型的版本，默认为当前最新。可选值：v3.5, v3.0, v2.0, v1.5
     sparkapi_model_top_k: int = 4 # 平衡生成文本的质量和多样性。较小的 k 值会减少随机性，使得输出更加稳定；而较大的 k 值会增加随机性，产生更多新颖的输出。取值范围[1, 6]，默认为4
     sparkapi_model_temperature : float = 0.5 # 控制结果随机性，取值越高随机性越强，即相同的问题得到的不同答案的可能性越高。取值范围 (0，1]，默认为0.5
-
-    sparkapi_command_chat :str = "" # 机器人对话指令，默认为空可直接对话（需要同时在`.env`中配置命令起始字符为空：COMMAND_START = [""]）
-    sparkapi_private_chat: bool = True # 允许私聊
-    sparkapi_group_public: bool = False # 群聊启用公共会话：True：所有人共享同一会话；False：每个人的会话各自独立
-    sparkapi_group_at: bool = True # 群聊回复时是否需要@提问者
-    sparkapi_fnotice:bool = True # 收到请求时是否提示已收到请求
-
-    sparkapi_priority: int = 90 # 聊天事件响应器优先级，[1,99]，数字越小优先级越高
-    sparkpai_max_length: int = 8000 # 单次上下文最大长度 越大，对话历史记录保留越长，消耗token上限越高
-
-    sparkapi_setpreset_clear: bool = True # 切换人物预设时是否清空上下文
+    sparkpai_model_maxlength: int = 8000 # 单次上下文最大长度 越大，对话历史记录保留越长，消耗token上限越高
+    
+    # 优先级：该值越小，事件越先被触发。本插件建议设置较大的值。可选值：1~97
+    # 若触发本插件事件，所有插件中优先级大于此值的事件都将被阻断。
+    # 本插件中事件的优先级顺序：私聊阻断（=priority）< 功能（=priority+1）< 对话（=priority+2）
+    sparkapi_priority: int = 80 # 优先级
+    
+    # 命令设置
+    sparkapi_commands : dict[str, str|list[str]] = { # 命令
+        "chat" : "", # 机器人对话指令（默认：为""且同时在`.env`中配置命令起始字符为空：COMMAND_START = [""]，即可直接对话）
+        "help" : ["help","帮助"], # 显示帮助信息
+        "preset_show" : ["preset","人物预设"], # 显示人物预设
+        "preset_set" : ["set","切换预设"], # 切换人物预设
+        "preset_create" : ["create","创建预设"], # 创建人物预设
+        "preset_delete" : ["delete","删除预设"], # 删除人物预设
+        "session_clear" : ["clear","清空对话"], # 清空对话
+        "session_save" : ["save","保存对话"], # 保存对话记录
+        "session_load" : ["load","加载对话"],  # 加载对话记录
+    }
+    sparkapi_commands_info: dict[str, str] = { # 命令说明，用于生成帮助信息
+        "chat" : "与机器人进行对话",
+        "help" : "显示帮助信息",
+        "preset_show" : "显示人物预设菜单和当前预设",
+        "preset_set" : "切换人物预设",
+        "preset_create" : "创建人物预设",
+        "preset_delete" : "删除人物预设",
+        "session_clear" : "清空当前对话上下文",
+        "session_save" : "保存本次对话记录",
+        "session_load" : "加载上次保存的对话记录",
+    }
+
+    # 聊天设置
+    sparkapi_fl_notice: bool = True # 收到请求时是否提示已收到请求
+    sparkapi_fl_setpreset_clear: bool = True # 切换人物预设时是否清空上下文
+    # 私聊设置
+    sparkapi_fl_private_chat: bool = True # 允许私聊
+    sparkapi_message_blockprivate: str = "私聊功能已关闭！如有需要，请联系管理员。" # 阻断私聊时的提示信息
+    # 群聊设置
+    sparkapi_fl_group_public: bool = False # 群聊启用公共会话：True：所有人共享同一会话；False：每个人的会话各自独立
+    sparkapi_fl_group_at: bool = True # 群聊中，回复时是否需要@提问者
 
     sparkapi_bot_name: str = "" # 机器人名字
-
-commands = {
-    "chat" : "chat", # 此处chat项只是为了保持代码一致性，在此处修改不生效，需要修改该命令请参阅插件文档
-    "help" : "help", # 显示帮助信息
-    "showpresets" : "presets", # 显示人物预设
-    "setpreset" : "set", # 更改人物预设
-    "clear" : "clear", # 清空对话
-    "savesession" : "save", # 保存对话记录
-    "loadsession" : "load"  # 加载对话记录
-}
-commands_lst = {
-    f"{commands['chat'] + ' + ' if commands['chat'] else '直接发送'}对话内容" : "与机器人进行对话",
-    commands["help"] : "显示帮助信息",
-    commands["showpresets"] : "显示人物预设",
-    commands["setpreset"] : "更改人物预设",
-    f"{commands['setpreset']} + 序号" : "选择人物预设",
-    commands["savesession"] : "保存当前对话记录",
-    commands["loadsession"] : "加载上次保存的对话记录",
-    commands["clear"] : "清除对话"
-}
```

### Comparing `nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi/funcs.py` & `nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi/funcs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,96 @@
 import hashlib
-from nonebot.adapters.onebot.v11 import PrivateMessageEvent
-from .config import Config, commands_lst
-from nonebot import get_driver
-conf = Config.parse_obj(get_driver().config.dict())
 
-group_public = conf.sparkapi_group_public
-max_length = conf.sparkpai_max_length
+from nonebot.adapters.onebot.v11 import PrivateMessageEvent as PME # type: ignore
+from nonebot.rule import command
 
+from .config import Config
+from nonebot import get_plugin_config
+conf = get_plugin_config(Config)
+
+group_public = conf.sparkapi_fl_group_public
+max_length = conf.sparkpai_model_maxlength
+
+# 统一模型版本，获取Spark URL、Domain
 def unify_model_version(model_version : str):
     version : str
     if model_version in ["v3.5","3.5","","default"]:
         version = "v3.5"
-    elif model_version in ["v3.0","3.0","v3.1","3.1","v3","3"]:
+    elif model_version in ["v3.0","3.0","v3.1","3.1","v3","3","Pro","pro"]:
         version = "v3.0"
     elif model_version in ["v2.0","2.0","v2.1","2.1","v2","2"]:
         version = "v2.0"
-    elif model_version in ["v1.0","1.0","v1.1","1.1","v1.5","1.5","v1","1"]:
+    elif model_version in ["v1.0","1.0","v1.1","1.1","v1.5","1.5","v1","1", "Lite","lite"]:
         version = "v1.5"
     return version
-
 def get_Spark_url(model_version : str):
     if model_version == "v3.5":
         return "wss://spark-api.xf-yun.com/v3.5/chat"
     if model_version == "v3.0":
         return "wss://spark-api.xf-yun.com/v3.1/chat"
     if model_version == "v2.0":
         return "wss://spark-api.xf-yun.com/v2.1/chat"
     if model_version == "v1.5":
         return "wss://spark-api.xf-yun.com/v1.1/chat"
-
 def get_domain(model_version : str):
     if model_version == "v3.5":
         return "generalv3.5"
     if model_version == "v3.0":
         return "generalv3"
     if model_version == "v2.0":
         return "generalv2"
     if model_version == "v1.5":
         return "general"
     
 def gethash(data:str) -> str: 
     return hashlib.md5(data.encode()).hexdigest()
+def get_sid(data:str) -> str:
+    return gethash(data)[-20:]
 
 def appendText(role, content, text):
     # "role": "system","user","assistant"
     # text: [{"role": "system", "content": ""},...]
     # 将对话内容追加到text列表中
     jsoncon = {}
     jsoncon["role"] = role
     jsoncon["content"] = content
     text.append(jsoncon)
     return text
 
-def getlength(text): # 获取对话长度
-    length = 0
-    for content in text:
-        temp = content["content"]
-        leng = len(temp)
-        length += leng
-    return length
+def checklen(text): # 修理对话长度
+    def getlength(text): # 获取对话长度
+        length = 0
+        for content in text:
+            temp = content["content"]
+            leng = len(temp)
+            length += leng
+        return length
+    while (getlength(text) > max_length):
+        del text[1]
+    return text
 
 # 根据消息类型创建会话ID
 def get_session_id(event):
-    if isinstance(event, PrivateMessageEvent):
+    if isinstance(event, PME):
         return "private_" + str(event.user_id)
     if group_public:
         return event.get_session_id().replace(str(event.user_id), "public")
     else:
         return event.get_session_id()
-    
-def checklen(text): # 修理对话长度
-    while (getlength(text) > max_length):
-        del text[1]
-    return text
-
-
-help_info = "【帮助信息】\n"
-
-for id, (command, description) in enumerate(commands_lst.items(), start=1):
-    help_info += f"{id}. {command}：{description}\n"
 
-help_info += "\n群聊中需要@bot + 指令/对话内容"
+# 将命令列表转化为Rule
+def trans_command(cmds: str|list[str]):
+    if(isinstance(cmds, str)): 
+        cmds = [cmds]
+    return command(*cmds)
+
+# 将预设转化为标准dict格式
+def trans_preset(prompt: str):
+    ret = {
+        'role': 'system',
+        'content': prompt
+    }
+    return ret
+
+# 合并两个dict
+def merge_dict(dict1, dict2):
+    return {**dict1, **dict2}
```

### Comparing `nonebot_plugin_sparkapi-1.1.0/nonebot_plugin_sparkapi.egg-info/PKG-INFO` & `nonebot_plugin_sparkapi-1.3.0/nonebot_plugin_sparkapi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.1.0
+Version: 1.3.0
 Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,15 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
 Requires-Dist: websockets<13.0,>=12.0
 
 <div align="center">
@@ -60,23 +60,20 @@
 
 适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设等功能
 
 ### 💬 功能
 - [x] 支持AI对话
 - [x] 支持上下文关联记忆（可设置记忆文本长度）
 - [x] 用户鉴别（每个用户的历史记录独立）
-- [x] 支持使用、切换人物预设（prompt）
-- [x] 人物预设菜单自动生成，更改无需重写
-- [x] 功能菜单自动生成，更改无需重写
+- [x] 支持用户自定义、更改、切换预设（prompt）
+- [x] 自动生成人物预设菜单、帮助列表，无需重写
+- [x] 基于pickle的历史记录持久化
 - [x] 完善的配置项（有其他需求请发issue）
-- [x] 历史记录持久化
-- [ ] 实用功能列表（查天气、查快递等）
 - [ ] 用户权限与功能区分（超级用户、普通用户）
-- [ ] 支持星火助手API
-- [ ] 支持用户自定义、更改预设
+- [ ] 支持图片生成（ImageGeneration）
 
 ### 📦 项目地址
 - Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
 - 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
 
 ## 💿 安装
 
@@ -129,39 +126,46 @@
 |:-----:|:----:|:----:|:----:|
 | SPARKAPI_APP_ID | 是 | "" | APPID |
 | SPARKAPI_API_SECRET | 是 | "" | APISecret |
 | SPARKAPI_API_KEY | 是 | "" | APIKey |
 | SPARKAPI_MODEL_VERSION | 否 | "" | 星火大模型的版本，默认为当前最新。<br>可选值：v3.5, v3.0, v2.0, v1.5 |
 | SPARKAPI_MODEL_TOP_K | 否 | 4 | 平衡生成文本的质量和多样性。<br>较小的 k 值会减少随机性，使得输出更加稳定；<br>而较大的 k 值会增加随机性，产生更多新颖的输出。<br>取值范围[1, 6] |
 | SPARKAPI_MODEL_TEMPERATURE | 否 | 0.5 | 控制结果随机性，取值越高随机性越强，即相同的问题得到的不同答案的可能性越高。<br>取值范围 (0，1] |
-| SPARKAPI_COMMAND_CHAT | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空<br>COMMAND_START = [""]） |
-| SPARKAPI_PRIVATE_CHAT | 否 | True | 是否允许私聊使用 |
-| SPARKAPI_GROUP_PUBLIC | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
-| SPARKAPI_GROUP_AT | 否 | True | 群聊回复消息时是否需要@提问者 |
-| SPARKAPI_FNOTICE | 否 | True | 收到请求时是否提示“已收到请求” |
-| SPARKAPI_PRIORITY | 否 | 90 | 聊天事件响应器优先级，[1,99]，数字越小优先级越高 |
-| SPARKPAI_MAX_LENGTH | 否 | 8000 | 上下文最大长度，[1,8000]<br>单次发送和回复的消息不能超过该项的一半 |
-| SPARKAPI_SETPRESET_CLEAR | 否 | True | 切换人物预设时是否清除当前对话上下文 |
+| SPARKAPI_MODEL_MAXKLENGTH | 否 | 8000 | 上下文最大长度，[1,8000]<br>单次发送和回复的消息不能超过该项的一半 |
+| SPARKAPI_PRIORITY | 否 | 80 | 该值越小，事件越先被触发。本插件建议设置较大的值。可选值：1~97<br>若触发本插件事件，所有插件中优先级大于此值的事件都将被阻断。<br>本插件中事件的优先级顺序：私聊阻断（=priority）< 功能（=priority+1）< 对话（=priority+2） |
+| SPARKAPI_COMMANDS__CHAT | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空：COMMAND_START = [""]） |
+| SPARKAPI_FL_NOTICE | 否 | True | 收到请求时是否提示“已收到请求” |
+| SPARKAPI_FL_SETPRESET_CLEAR | 否 | True | 切换人物预设时是否清除当前对话上下文 |
+| SPARKAPI_FL_PRIVATE_CHAT | 否 | True | 是否允许私聊使用 |
+| SPARKAPI_FL_GROUP_PUBLIC | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
+| SPARKAPI_FL_GROUP_AT | 否 | True | 群聊回复消息时是否需要@提问者 |
 | SPARKAPI_BOT_NAME | 否 | "" | 机器人的名字 |
 
+以下配置项请查看`/.venv/Lib/nonebot_plugin_sparkapi/config.py`修改：
+1. sparkapi_commands：指令表（允许单个字符串或字符串列表）
+2. sparkapi_commands_info：指令表说明（用于生成帮助信息）
+3. sparkapi_message_blockprivate：阻断私聊时的提示信息
 
 ## 🎉 使用
-### 指令表
-所有指令均可在config.py中修改，且无需重写菜单/指令生成函数
+### 指令表（默认）
+以下所有指令均可在config.py中修改，且无需重写菜单/指令生成函数
 
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | SPARKAPI_COMMAND_CHAT（若不为空） + 对话内容 | 是 | 私聊/群聊 | 与机器人进行对话 |
-| help | 是 | 私聊/群聊 | 查看帮助信息 |
-| presets | 是 | 私聊/群聊 | 查看当前可选的人物预设 |
-| set | 是 | 私聊/群聊 | 查看当前可选的人物预设<br>回复编号以进行切换 |
-| set + 人物预设编号 | 是 | 私聊/群聊 | 切换到编号对应的人物预设 |
-| save | 是 | 私聊/群聊 | 保存当前对话上下文 |
-| load | 是 | 私聊/群聊 | 加载之前保存的对话上下文 |
-| clear | 是 | 私聊/群聊 | 清除当前对话上下文 |
+| help/帮助 | 是 | 私聊/群聊 | 显示帮助信息 |
+| preset/人物预设 | 是 | 私聊/群聊 | 显示人物预设菜单和当前预设 |
+| set/切换预设 | 是 | 私聊/群聊 | 显示人物预设菜单，选择并切换 |
+| set/切换预设 + 人物名 | 是 | 私聊/群聊 | 切换人物预设 |
+| create/创建预设 | 是 | 私聊/群聊 | 创建自定义的人物预设 |
+| delete/删除预设 | 是 | 私聊/群聊 | 删除自定义的人物预设 |
+| delete/删除预设 + 人物名 | 是 | 私聊/群聊 | 显示自定义人物预设菜单, 选择并删除 |
+| clear/清空对话 | 是 | 私聊/群聊 | 清除当前对话上下文 |
+| save/保存对话 | 是 | 私聊/群聊 | 保存当前对话记录 |
+| load/加载对话 | 是 | 私聊/群聊 | 加载上次保存的对话记录 |
 
 ### 人物预设
 1. 智能助手（默认）
 2. 心理咨询师
 
 ### 效果图
 ![demo](https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.3.0 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -11,83 +11,93 @@
 permission notice shall be included in all copies or substantial portions of
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Requires-Python: >=3.8 Description-Content-Type:
+DEALINGS IN THE SOFTWARE. Requires-Python: >=3.10 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: nonebot-adapter-
 onebot<3.0.0,>=2.2.1 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3 Requires-Dist:
 websockets<13.0,>=12.0
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
-æ¯æä½¿ç¨ãåæ¢äººç©é¢è®¾ï¼promptï¼ - [x]
-äººç©é¢è®¾èåèªå¨çæï¼æ´æ¹æ ééå - [x]
-åè½èåèªå¨çæï¼æ´æ¹æ ééå - [x]
-å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [x] åå²è®°å½æä¹å
-- [ ] å®ç¨åè½åè¡¨ï¼æ¥å¤©æ°ãæ¥å¿«éç­ï¼ - [ ]
+æ¯æç¨æ·èªå®ä¹ãæ´æ¹ãåæ¢é¢è®¾ï¼promptï¼ - [x]
+èªå¨çæäººç©é¢è®¾èåãå¸®å©åè¡¨ï¼æ ééå - [x]
+åºäºpickleçåå²è®°å½æä¹å - [x]
+å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [ ]
 ç¨æ·æéä¸åè½åºåï¼è¶çº§ç¨æ·ãæ®éç¨æ·ï¼ - [ ]
-æ¯ææç«å©æAPI - [ ] æ¯æç¨æ·èªå®ä¹ãæ´æ¹é¢è®¾ ### ð¦
-é¡¹ç®å°å - Githubï¼https://github.com/CCLMSY/nonebot-plugin-sparkapi -
-è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-
-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-sparkapi
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip pip install nonebot-plugin-sparkapi pdm pdm add nonebot-plugin-sparkapi
-poetry poetry add nonebot-plugin-sparkapi conda conda install nonebot-plugin-
-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
-[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_sparkapi"] ##
-âï¸ éç½® å¨ nonebot2
+æ¯æå¾ççæï¼ImageGenerationï¼ ### ð¦ é¡¹ç®å°å - Githubï¼https:
+//github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
+Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
+install nonebot-plugin-sparkapi ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
+é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
+è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-sparkapi pdm pdm add
+nonebot-plugin-sparkapi poetry poetry add nonebot-plugin-sparkapi conda conda
+install nonebot-plugin-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
+`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
+["nonebot_plugin_sparkapi"] ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
 å¶ä¸­ï¼æå¡æ¥å£è®¤è¯ä¿¡æ¯ app_id, api_secret, api_key è¯·åå¾
 [è®¯é£å¼æ¾å¹³å°æ§å¶å°](https://console.xfyun.cn/) è·å | éç½®é¡¹ |
 å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | SPARKAPI_APP_ID
 | æ¯ | "" | APPID | | SPARKAPI_API_SECRET | æ¯ | "" | APISecret | |
 SPARKAPI_API_KEY | æ¯ | "" | APIKey | | SPARKAPI_MODEL_VERSION | å¦ | "" |
 æç«å¤§æ¨¡åççæ¬ï¼é»è®¤ä¸ºå½åææ°ã
 å¯éå¼ï¼v3.5, v3.0, v2.0, v1.5 | | SPARKAPI_MODEL_TOP_K | å¦ | 4 |
 å¹³è¡¡çæææ¬çè´¨éåå¤æ ·æ§ã
 è¾å°ç k å¼ä¼åå°éæºæ§ï¼ä½¿å¾è¾åºæ´å ç¨³å®ï¼
 èè¾å¤§ç k å¼ä¼å¢å éæºæ§ï¼äº§çæ´å¤æ°é¢çè¾åºã
 åå¼èå´[1, 6] | | SPARKAPI_MODEL_TEMPERATURE | å¦ | 0.5 |
 æ§å¶ç»æéæºæ§ï¼åå¼è¶é«éæºæ§è¶å¼ºï¼å³ç¸åçé®é¢å¾å°çä¸åç­æ¡çå¯è½æ§è¶é«ã
-åå¼èå´ (0ï¼1] | | SPARKAPI_COMMAND_CHAT | å¦ | "" |
-æºå¨äººå¯¹è¯æä»¤ï¼é»è®¤ä¸ºç©ºå¯ç´æ¥å¯¹è¯
-ï¼éè¦åæ¶å¨`.env`ä¸­éç½®å½ä»¤èµ·å§å­ç¬¦ä¸ºç©º
-COMMAND_START = [""]ï¼ | | SPARKAPI_PRIVATE_CHAT | å¦ | True |
-æ¯å¦åè®¸ç§èä½¿ç¨ | | SPARKAPI_GROUP_PUBLIC | å¦ | False |
-ç¾¤èå¯ç¨å¬å±ä¼è¯
+åå¼èå´ (0ï¼1] | | SPARKAPI_MODEL_MAXKLENGTH | å¦ | 8000 |
+ä¸ä¸ææå¤§é¿åº¦ï¼[1,8000]
+åæ¬¡åéååå¤çæ¶æ¯ä¸è½è¶è¿è¯¥é¡¹çä¸å | | SPARKAPI_PRIORITY
+| å¦ | 80 |
+è¯¥å¼è¶å°ï¼äºä»¶è¶åè¢«è§¦åãæ¬æä»¶å»ºè®®è®¾ç½®è¾å¤§çå¼ãå¯éå¼ï¼1~97
+è¥è§¦åæ¬æä»¶äºä»¶ï¼æææä»¶ä¸­ä¼åçº§å¤§äºæ­¤å¼çäºä»¶é½å°è¢«é»æ­ã
+æ¬æä»¶ä¸­äºä»¶çä¼åçº§é¡ºåºï¼ç§èé»æ­ï¼=priorityï¼<
+åè½ï¼=priority+1ï¼< å¯¹è¯ï¼=priority+2ï¼ | | SPARKAPI_COMMANDS__CHAT |
+å¦ | "" | æºå¨äººå¯¹è¯æä»¤ï¼é»è®¤ä¸ºç©ºå¯ç´æ¥å¯¹è¯
+ï¼éè¦åæ¶å¨`.env`ä¸­éç½®å½ä»¤èµ·å§å­ç¬¦ä¸ºç©ºï¼COMMAND_START =
+[""]ï¼ | | SPARKAPI_FL_NOTICE | å¦ | True |
+æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | |
+SPARKAPI_FL_SETPRESET_CLEAR | å¦ | True |
+åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | |
+SPARKAPI_FL_PRIVATE_CHAT | å¦ | True | æ¯å¦åè®¸ç§èä½¿ç¨ | |
+SPARKAPI_FL_GROUP_PUBLIC | å¦ | False | ç¾¤èå¯ç¨å¬å±ä¼è¯
 Trueï¼ææäººå±äº«åä¸ä¼è¯
-Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | SPARKAPI_GROUP_AT | å¦ | True |
-ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_FNOTICE | å¦ | True |
-æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | | SPARKAPI_PRIORITY | å¦ |
-90 | èå¤©äºä»¶ååºå¨ä¼åçº§ï¼[1,99]ï¼æ°å­è¶å°ä¼åçº§è¶é« | |
-SPARKPAI_MAX_LENGTH | å¦ | 8000 | ä¸ä¸ææå¤§é¿åº¦ï¼[1,8000]
-åæ¬¡åéååå¤çæ¶æ¯ä¸è½è¶è¿è¯¥é¡¹çä¸å | |
-SPARKAPI_SETPRESET_CLEAR | å¦ | True |
-åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | SPARKAPI_BOT_NAME |
-å¦ | "" | æºå¨äººçåå­ | ## ð ä½¿ç¨ ### æä»¤è¡¨
-æææä»¤åå¯å¨config.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
+Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | SPARKAPI_FL_GROUP_AT | å¦ | True |
+ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_BOT_NAME | å¦ | "" |
+æºå¨äººçåå­ | ä»¥ä¸éç½®é¡¹è¯·æ¥ç`/.venv/Lib/
+nonebot_plugin_sparkapi/config.py`ä¿®æ¹ï¼ 1.
+sparkapi_commandsï¼æä»¤è¡¨ï¼åè®¸åä¸ªå­ç¬¦ä¸²æå­ç¬¦ä¸²åè¡¨ï¼ 2.
+sparkapi_commands_infoï¼æä»¤è¡¨è¯´æï¼ç¨äºçæå¸®å©ä¿¡æ¯ï¼ 3.
+sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
+### æä»¤è¡¨ï¼é»è®¤ï¼
+ä»¥ä¸æææä»¤åå¯å¨config.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
 æä»¤çæå½æ° | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:| | SPARKAPI_COMMAND_CHATï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ |
-ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help | æ¯ | ç§è/ç¾¤è |
-æ¥çå¸®å©ä¿¡æ¯ | | presets | æ¯ | ç§è/ç¾¤è |
-æ¥çå½åå¯éçäººç©é¢è®¾ | | set | æ¯ | ç§è/ç¾¤è |
-æ¥çå½åå¯éçäººç©é¢è®¾
-åå¤ç¼å·ä»¥è¿è¡åæ¢ | | set + äººç©é¢è®¾ç¼å· | æ¯ | ç§è/ç¾¤è
-| åæ¢å°ç¼å·å¯¹åºçäººç©é¢è®¾ | | save | æ¯ | ç§è/ç¾¤è |
-ä¿å­å½åå¯¹è¯ä¸ä¸æ | | load | æ¯ | ç§è/ç¾¤è |
-å è½½ä¹åä¿å­çå¯¹è¯ä¸ä¸æ | | clear | æ¯ | ç§è/ç¾¤è |
-æ¸é¤å½åå¯¹è¯ä¸ä¸æ | ### äººç©é¢è®¾ 1. æºè½å©æï¼é»è®¤ï¼ 2.
-å¿çå¨è¯¢å¸ ### ææå¾ ![demo](https://github.com/CCLMSY/nonebot-plugin-
-sparkapi/blob/resources/demo.jpg)
+ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help/å¸®å© | æ¯ | ç§è/ç¾¤è
+| æ¾ç¤ºå¸®å©ä¿¡æ¯ | | preset/äººç©é¢è®¾ | æ¯ | ç§è/ç¾¤è |
+æ¾ç¤ºäººç©é¢è®¾èååå½åé¢è®¾ | | set/åæ¢é¢è®¾ | æ¯ | ç§è/
+ç¾¤è | æ¾ç¤ºäººç©é¢è®¾èåï¼éæ©å¹¶åæ¢ | | set/åæ¢é¢è®¾ +
+äººç©å | æ¯ | ç§è/ç¾¤è | åæ¢äººç©é¢è®¾ | | create/åå»ºé¢è®¾ |
+æ¯ | ç§è/ç¾¤è | åå»ºèªå®ä¹çäººç©é¢è®¾ | | delete/å é¤é¢è®¾ |
+æ¯ | ç§è/ç¾¤è | å é¤èªå®ä¹çäººç©é¢è®¾ | | delete/å é¤é¢è®¾ +
+äººç©å | æ¯ | ç§è/ç¾¤è | æ¾ç¤ºèªå®ä¹äººç©é¢è®¾èå,
+éæ©å¹¶å é¤ | | clear/æ¸ç©ºå¯¹è¯ | æ¯ | ç§è/ç¾¤è |
+æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | save/ä¿å­å¯¹è¯ | æ¯ | ç§è/ç¾¤è |
+ä¿å­å½åå¯¹è¯è®°å½ | | load/å è½½å¯¹è¯ | æ¯ | ç§è/ç¾¤è |
+å è½½ä¸æ¬¡ä¿å­çå¯¹è¯è®°å½ | ### äººç©é¢è®¾ 1.
+æºè½å©æï¼é»è®¤ï¼ 2. å¿çå¨è¯¢å¸ ### ææå¾ ![demo](https://
+github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

### Comparing `nonebot_plugin_sparkapi-1.1.0/pyproject.toml` & `nonebot_plugin_sparkapi-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "nonebot_plugin_sparkapi"
-version = "1.1.0"
+version = "1.3.0"
 description = "Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)"
 authors = [
     { name = "CCLMSY", email = "2502408581@qq.com" }
 ]
 dependencies = [
     "nonebot-adapter-onebot >=2.2.1, <3.0.0",
     "nonebot2 >=2.0.0rc3, <3.0.0",
     "websockets >=12.0, <13.0"
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 license = { file = "LICENSE" }
 readme = { file = "README.md", content-type = "text/markdown" }
 
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
```

