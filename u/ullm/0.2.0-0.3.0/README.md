# Comparing `tmp/ullm-0.2.0.tar.gz` & `tmp/ullm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ullm-0.2.0.tar", last modified: Wed May 15 03:05:51 2024, max compression
+gzip compressed data, was "ullm-0.3.0.tar", last modified: Tue May 28 06:35:17 2024, max compression
```

## Comparing `ullm-0.2.0.tar` & `ullm-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:05:51.079203 ullm-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-05-15 03:05:51.079203 ullm-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-05-15 03:05:47.000000 ullm-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-15 03:05:47.000000 ullm-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 03:05:51.079203 ullm-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:05:51.071203 ullm-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-15 03:05:47.000000 ullm-0.2.0/tests/test_openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:05:51.079203 ullm-0.2.0/ullm/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/alibaba.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/baichuan.py
--rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)    19678 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/deepseek.py
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/iflytek.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/minimax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/moonshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)    14332 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     8432 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/skywork.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/stepfun.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/together.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/zero_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/zhipu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:05:51.079203 ullm-0.2.0/ullm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-05-15 03:05:51.000000 ullm-0.2.0/ullm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-15 03:05:51.000000 ullm-0.2.0/ullm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 03:05:51.000000 ullm-0.2.0/ullm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 03:05:51.000000 ullm-0.2.0/ullm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 03:05:51.000000 ullm-0.2.0/ullm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 03:05:51.000000 ullm-0.2.0/ullm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:35:17.681209 ullm-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-05-28 06:35:17.681209 ullm-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17551 2024-05-28 06:35:12.000000 ullm-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-28 06:35:12.000000 ullm-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 06:35:17.681209 ullm-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:35:17.677209 ullm-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-28 06:35:12.000000 ullm-0.3.0/tests/test_openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:35:17.681209 ullm-0.3.0/ullm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/baichuan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24252 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20213 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/deepseek.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/iflytek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/minimax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/moonshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14310 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/skywork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/stepfun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/zero_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/zhipu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:35:17.681209 ullm-0.3.0/ullm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-05-28 06:35:17.000000 ullm-0.3.0/ullm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-28 06:35:17.000000 ullm-0.3.0/ullm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:35:17.000000 ullm-0.3.0/ullm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 06:35:17.000000 ullm-0.3.0/ullm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-28 06:35:17.000000 ullm-0.3.0/ullm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 06:35:17.000000 ullm-0.3.0/ullm.egg-info/top_level.txt
```

### Comparing `ullm-0.2.0/PKG-INFO` & `ullm-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ullm
-Version: 0.2.0
+Version: 0.3.0
 Summary: A unified interface for local Large Language Model(LLM) models and online LLM providers.
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/monsternlp/ullm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -90,33 +90,33 @@
 
 TBD
 
 ### 在线服务
 
 | 平台 | Provider ID            | 模型数量 | 视觉模型数量 | 支持工具调用的模型数量 | 联网模型数量 |
 |------|-------------------|----------|--------------|------------------------|--------------|
-| [零一万物](https://platform.lingyiwanwu.com/docs)     | 01ai              |        3 |            1 |                      0 |            0 |
-| [阿里巴巴](https://help.aliyun.com/zh/dashscope/developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT)      | alibaba           |       44 |            4 |                      6 |            6 |
+| [零一万物](https://platform.lingyiwanwu.com/docs)     | 01ai              |        9 |            1 |                      0 |            2 |
+| [阿里巴巴](https://help.aliyun.com/zh/dashscope/developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT)      | alibaba           |       46 |            4 |                      7 |            7 |
 | [Anthropic](https://docs.anthropic.com/claude/reference/getting-started-with-the-api)     | anthropic         |        3 |            3 |                      3 |            0 |
 | [Azure OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/reference#chat-completions)     | azure-openai      |       20 |            4 |                     11 |            0 |
-| [百川智能](https://platform.baichuan-ai.com/docs/api)     | baichuan          |        4 |            0 |                      0 |            2 |
-| [百度](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu)     | baidu             |       46 |            0 |                     24 |           12 |
+| [百川智能](https://platform.baichuan-ai.com/docs/api)     | baichuan          |        10 |            0 |                      3 |            5 |
+| [百度](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu)     | baidu             |       51 |            0 |                     28 |           14 |
 | [Cloudflare Workers AI](https://developers.cloudflare.com/workers-ai/get-started/rest-api/) | cloudflare        |       35 |               0 |             0 |               0 |
 | [Cohere](https://docs.cohere.com/reference/about)     | cohere            |       12 |            0 |                      4 |            6 |
 | [DeepSeek](https://platform.deepseek.com/docs)     | deepseek          |        2 |            0 |                      0 |            0 |
-| [Google](https://ai.google.dev/gemini-api/docs)     | google            |        3 |            2 |                      2 |            0 |
+| [Google](https://ai.google.dev/gemini-api/docs)     | google            |        13 |            9 |                      2 |            0 |
 | [Groq](https://console.groq.com/docs/quickstart)     | groq              |        4 |            0 |                      4 |            0 |
 | [科大讯飞](https://www.xfyun.cn/doc/spark/%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E.html)     | iflytek           |        4 |            0 |                      2 |            0 |
-| [MiniMax](https://www.minimaxi.com/document/algorithm-concept?id=6433f37594878d408fc8295d)     | minimax           |        5 |            0 |                      5 |            0 |
+| [MiniMax](https://www.minimaxi.com/document/algorithm-concept?id=6433f37594878d408fc8295d)     | minimax           |        6 |            0 |                      6 |            0 |
 | [Moonshot](https://platform.moonshot.cn/docs/api/chat#%E5%9F%BA%E6%9C%AC%E4%BF%A1%E6%81%AF)     | moonshot          |        3 |            0 |                      3 |            0 |
-| [OpenAI](https://platform.openai.com/docs/api-reference/chat)      | openai            |       20 |            4 |                     11 |            0 |
-| [OpenRouter](https://openrouter.ai/docs)     | openrouter        |      127 |           13 |                    127 |            4 |
+| [OpenAI](https://platform.openai.com/docs/api-reference/chat)      | openai            |       21 |            5 |                     12 |            0 |
+| [OpenRouter](https://openrouter.ai/docs)     | openrouter        |      158 |           16 |                    158 |            2 |
 | [Perplexity](https://docs.perplexity.ai/docs/getting-started)     | perplexity        |        7 |            0 |                      0 |            2 |
 | [天工](https://model-platform.tiangong.cn/api-reference) | skywork           |        1 |               0 |             0 |               0 |
-| [阶跃星辰](https://platform.stepfun.com/docs/Chat/chat-completion-create)     | stepfun           |        3 |            1 |                      0 |            0 |
+| [阶跃星辰](https://platform.stepfun.com/docs/Chat/chat-completion-create)     | stepfun           |        6 |            2 |                      0 |            0 |
 | [Together AI](https://docs.together.ai/docs/quickstart) | together          |       58 |               0 |            58 |               0 |
 | [智谱](https://open.bigmodel.cn/dev/api)     | zhipu             |        5 |            1 |                      4 |            2 |
 | OpenAI 接口兼容的服务     | openai-compatible |          |              |                        |              |
 | Ollama API     | ollama            |          |              |                        |              |
 
 
 ## 安装
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ullm Version: 0.2.0 Summary: A unified interface
+Metadata-Version: 2.1 Name: ullm Version: 0.3.0 Summary: A unified interface
 for local Large Language Model(LLM) models and online LLM providers. Author-
 email: Linusp
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/monsternlp/
 ullm Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist: pydantic
 Requires-Dist: arrow Requires-Dist: websocket-client Requires-Dist: requests
@@ -39,40 +39,40 @@
 tokenizerï¼ä»¥è·å¾ tokens æ°éè§£å³æäº remote model ä¸è¿å tokens
 æ°éçé®é¢ - [ ] æ¨¡åéç½®çç®¡ç - [ ] å¤æ¨¡åè·¯ç± - [ ]
 ååæµè¯ - [ ] å®åææ¡£ - [ ] å®ç°æµå¼æ¥å£ ## æ¯ææ¨¡å ###
 æ¬å°æ¨¡å TBD ### å¨çº¿æå¡ | å¹³å° | Provider ID | æ¨¡åæ°é |
 è§è§æ¨¡åæ°é | æ¯æå·¥å·è°ç¨çæ¨¡åæ°é | èç½æ¨¡åæ°é |
 |------|-------------------|----------|--------------|------------------------
 |--------------| | [é¶ä¸ä¸ç©](https://platform.lingyiwanwu.com/docs) | 01ai
-| 3 | 1 | 0 | 0 | | [é¿éå·´å·´](https://help.aliyun.com/zh/dashscope/
+| 9 | 1 | 0 | 2 | | [é¿éå·´å·´](https://help.aliyun.com/zh/dashscope/
 developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT) |
-alibaba | 44 | 4 | 6 | 6 | | [Anthropic](https://docs.anthropic.com/claude/
+alibaba | 46 | 4 | 7 | 7 | | [Anthropic](https://docs.anthropic.com/claude/
 reference/getting-started-with-the-api) | anthropic | 3 | 3 | 3 | 0 | | [Azure
 OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/
 reference#chat-completions) | azure-openai | 20 | 4 | 11 | 0 | | [ç¾å·æºè½]
-(https://platform.baichuan-ai.com/docs/api) | baichuan | 4 | 0 | 0 | 2 | |
-[ç¾åº¦](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu) | baidu | 46 |
-0 | 24 | 12 | | [Cloudflare Workers AI](https://developers.cloudflare.com/
+(https://platform.baichuan-ai.com/docs/api) | baichuan | 10 | 0 | 3 | 5 | |
+[ç¾åº¦](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu) | baidu | 51 |
+0 | 28 | 14 | | [Cloudflare Workers AI](https://developers.cloudflare.com/
 workers-ai/get-started/rest-api/) | cloudflare | 35 | 0 | 0 | 0 | | [Cohere]
 (https://docs.cohere.com/reference/about) | cohere | 12 | 0 | 4 | 6 | |
 [DeepSeek](https://platform.deepseek.com/docs) | deepseek | 2 | 0 | 0 | 0 | |
-[Google](https://ai.google.dev/gemini-api/docs) | google | 3 | 2 | 2 | 0 | |
+[Google](https://ai.google.dev/gemini-api/docs) | google | 13 | 9 | 2 | 0 | |
 [Groq](https://console.groq.com/docs/quickstart) | groq | 4 | 0 | 4 | 0 | |
 [ç§å¤§è®¯é£](https://www.xfyun.cn/doc/spark/
 %E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E.html) | iflytek | 4 | 0 | 2 | 0 | |
 [MiniMax](https://www.minimaxi.com/document/algorithm-
-concept?id=6433f37594878d408fc8295d) | minimax | 5 | 0 | 5 | 0 | | [Moonshot]
+concept?id=6433f37594878d408fc8295d) | minimax | 6 | 0 | 6 | 0 | | [Moonshot]
 (https://platform.moonshot.cn/docs/api/
 chat#%E5%9F%BA%E6%9C%AC%E4%BF%A1%E6%81%AF) | moonshot | 3 | 0 | 3 | 0 | |
-[OpenAI](https://platform.openai.com/docs/api-reference/chat) | openai | 20 | 4
-| 11 | 0 | | [OpenRouter](https://openrouter.ai/docs) | openrouter | 127 | 13 |
-127 | 4 | | [Perplexity](https://docs.perplexity.ai/docs/getting-started) |
+[OpenAI](https://platform.openai.com/docs/api-reference/chat) | openai | 21 | 5
+| 12 | 0 | | [OpenRouter](https://openrouter.ai/docs) | openrouter | 158 | 16 |
+158 | 2 | | [Perplexity](https://docs.perplexity.ai/docs/getting-started) |
 perplexity | 7 | 0 | 0 | 2 | | [å¤©å·¥](https://model-platform.tiangong.cn/api-
 reference) | skywork | 1 | 0 | 0 | 0 | | [é¶è·æè¾°](https://
-platform.stepfun.com/docs/Chat/chat-completion-create) | stepfun | 3 | 1 | 0 |
+platform.stepfun.com/docs/Chat/chat-completion-create) | stepfun | 6 | 2 | 0 |
 0 | | [Together AI](https://docs.together.ai/docs/quickstart) | together | 58 |
 0 | 58 | 0 | | [æºè°±](https://open.bigmodel.cn/dev/api) | zhipu | 5 | 1 | 4 |
 2 | | OpenAI æ¥å£å¼å®¹çæå¡ | openai-compatible | | | | | | Ollama API |
 ollama | | | | | ## å®è£ ```shell pip install ullm ``` ## ä½¿ç¨ ###
 åå»ºæ¨¡åéç½® ç¤ºä¾: ```python model_config = { # required fields "type":
 'remote', "model": 'gpt-3.5-turbo', "provider": 'openai', "api_key": 'sk-
 ************************************************', # optional fields
```

### Comparing `ullm-0.2.0/README.md` & `ullm-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,33 +65,33 @@
 
 TBD
 
 ### 在线服务
 
 | 平台 | Provider ID            | 模型数量 | 视觉模型数量 | 支持工具调用的模型数量 | 联网模型数量 |
 |------|-------------------|----------|--------------|------------------------|--------------|
-| [零一万物](https://platform.lingyiwanwu.com/docs)     | 01ai              |        3 |            1 |                      0 |            0 |
-| [阿里巴巴](https://help.aliyun.com/zh/dashscope/developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT)      | alibaba           |       44 |            4 |                      6 |            6 |
+| [零一万物](https://platform.lingyiwanwu.com/docs)     | 01ai              |        9 |            1 |                      0 |            2 |
+| [阿里巴巴](https://help.aliyun.com/zh/dashscope/developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT)      | alibaba           |       46 |            4 |                      7 |            7 |
 | [Anthropic](https://docs.anthropic.com/claude/reference/getting-started-with-the-api)     | anthropic         |        3 |            3 |                      3 |            0 |
 | [Azure OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/reference#chat-completions)     | azure-openai      |       20 |            4 |                     11 |            0 |
-| [百川智能](https://platform.baichuan-ai.com/docs/api)     | baichuan          |        4 |            0 |                      0 |            2 |
-| [百度](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu)     | baidu             |       46 |            0 |                     24 |           12 |
+| [百川智能](https://platform.baichuan-ai.com/docs/api)     | baichuan          |        10 |            0 |                      3 |            5 |
+| [百度](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu)     | baidu             |       51 |            0 |                     28 |           14 |
 | [Cloudflare Workers AI](https://developers.cloudflare.com/workers-ai/get-started/rest-api/) | cloudflare        |       35 |               0 |             0 |               0 |
 | [Cohere](https://docs.cohere.com/reference/about)     | cohere            |       12 |            0 |                      4 |            6 |
 | [DeepSeek](https://platform.deepseek.com/docs)     | deepseek          |        2 |            0 |                      0 |            0 |
-| [Google](https://ai.google.dev/gemini-api/docs)     | google            |        3 |            2 |                      2 |            0 |
+| [Google](https://ai.google.dev/gemini-api/docs)     | google            |        13 |            9 |                      2 |            0 |
 | [Groq](https://console.groq.com/docs/quickstart)     | groq              |        4 |            0 |                      4 |            0 |
 | [科大讯飞](https://www.xfyun.cn/doc/spark/%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E.html)     | iflytek           |        4 |            0 |                      2 |            0 |
-| [MiniMax](https://www.minimaxi.com/document/algorithm-concept?id=6433f37594878d408fc8295d)     | minimax           |        5 |            0 |                      5 |            0 |
+| [MiniMax](https://www.minimaxi.com/document/algorithm-concept?id=6433f37594878d408fc8295d)     | minimax           |        6 |            0 |                      6 |            0 |
 | [Moonshot](https://platform.moonshot.cn/docs/api/chat#%E5%9F%BA%E6%9C%AC%E4%BF%A1%E6%81%AF)     | moonshot          |        3 |            0 |                      3 |            0 |
-| [OpenAI](https://platform.openai.com/docs/api-reference/chat)      | openai            |       20 |            4 |                     11 |            0 |
-| [OpenRouter](https://openrouter.ai/docs)     | openrouter        |      127 |           13 |                    127 |            4 |
+| [OpenAI](https://platform.openai.com/docs/api-reference/chat)      | openai            |       21 |            5 |                     12 |            0 |
+| [OpenRouter](https://openrouter.ai/docs)     | openrouter        |      158 |           16 |                    158 |            2 |
 | [Perplexity](https://docs.perplexity.ai/docs/getting-started)     | perplexity        |        7 |            0 |                      0 |            2 |
 | [天工](https://model-platform.tiangong.cn/api-reference) | skywork           |        1 |               0 |             0 |               0 |
-| [阶跃星辰](https://platform.stepfun.com/docs/Chat/chat-completion-create)     | stepfun           |        3 |            1 |                      0 |            0 |
+| [阶跃星辰](https://platform.stepfun.com/docs/Chat/chat-completion-create)     | stepfun           |        6 |            2 |                      0 |            0 |
 | [Together AI](https://docs.together.ai/docs/quickstart) | together          |       58 |               0 |            58 |               0 |
 | [智谱](https://open.bigmodel.cn/dev/api)     | zhipu             |        5 |            1 |                      4 |            2 |
 | OpenAI 接口兼容的服务     | openai-compatible |          |              |                        |              |
 | Ollama API     | ollama            |          |              |                        |              |
 
 
 ## 安装
```

#### html2text {}

```diff
@@ -27,40 +27,40 @@
 tokenizerï¼ä»¥è·å¾ tokens æ°éè§£å³æäº remote model ä¸è¿å tokens
 æ°éçé®é¢ - [ ] æ¨¡åéç½®çç®¡ç - [ ] å¤æ¨¡åè·¯ç± - [ ]
 ååæµè¯ - [ ] å®åææ¡£ - [ ] å®ç°æµå¼æ¥å£ ## æ¯ææ¨¡å ###
 æ¬å°æ¨¡å TBD ### å¨çº¿æå¡ | å¹³å° | Provider ID | æ¨¡åæ°é |
 è§è§æ¨¡åæ°é | æ¯æå·¥å·è°ç¨çæ¨¡åæ°é | èç½æ¨¡åæ°é |
 |------|-------------------|----------|--------------|------------------------
 |--------------| | [é¶ä¸ä¸ç©](https://platform.lingyiwanwu.com/docs) | 01ai
-| 3 | 1 | 0 | 0 | | [é¿éå·´å·´](https://help.aliyun.com/zh/dashscope/
+| 9 | 1 | 0 | 2 | | [é¿éå·´å·´](https://help.aliyun.com/zh/dashscope/
 developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT) |
-alibaba | 44 | 4 | 6 | 6 | | [Anthropic](https://docs.anthropic.com/claude/
+alibaba | 46 | 4 | 7 | 7 | | [Anthropic](https://docs.anthropic.com/claude/
 reference/getting-started-with-the-api) | anthropic | 3 | 3 | 3 | 0 | | [Azure
 OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/
 reference#chat-completions) | azure-openai | 20 | 4 | 11 | 0 | | [ç¾å·æºè½]
-(https://platform.baichuan-ai.com/docs/api) | baichuan | 4 | 0 | 0 | 2 | |
-[ç¾åº¦](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu) | baidu | 46 |
-0 | 24 | 12 | | [Cloudflare Workers AI](https://developers.cloudflare.com/
+(https://platform.baichuan-ai.com/docs/api) | baichuan | 10 | 0 | 3 | 5 | |
+[ç¾åº¦](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu) | baidu | 51 |
+0 | 28 | 14 | | [Cloudflare Workers AI](https://developers.cloudflare.com/
 workers-ai/get-started/rest-api/) | cloudflare | 35 | 0 | 0 | 0 | | [Cohere]
 (https://docs.cohere.com/reference/about) | cohere | 12 | 0 | 4 | 6 | |
 [DeepSeek](https://platform.deepseek.com/docs) | deepseek | 2 | 0 | 0 | 0 | |
-[Google](https://ai.google.dev/gemini-api/docs) | google | 3 | 2 | 2 | 0 | |
+[Google](https://ai.google.dev/gemini-api/docs) | google | 13 | 9 | 2 | 0 | |
 [Groq](https://console.groq.com/docs/quickstart) | groq | 4 | 0 | 4 | 0 | |
 [ç§å¤§è®¯é£](https://www.xfyun.cn/doc/spark/
 %E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E.html) | iflytek | 4 | 0 | 2 | 0 | |
 [MiniMax](https://www.minimaxi.com/document/algorithm-
-concept?id=6433f37594878d408fc8295d) | minimax | 5 | 0 | 5 | 0 | | [Moonshot]
+concept?id=6433f37594878d408fc8295d) | minimax | 6 | 0 | 6 | 0 | | [Moonshot]
 (https://platform.moonshot.cn/docs/api/
 chat#%E5%9F%BA%E6%9C%AC%E4%BF%A1%E6%81%AF) | moonshot | 3 | 0 | 3 | 0 | |
-[OpenAI](https://platform.openai.com/docs/api-reference/chat) | openai | 20 | 4
-| 11 | 0 | | [OpenRouter](https://openrouter.ai/docs) | openrouter | 127 | 13 |
-127 | 4 | | [Perplexity](https://docs.perplexity.ai/docs/getting-started) |
+[OpenAI](https://platform.openai.com/docs/api-reference/chat) | openai | 21 | 5
+| 12 | 0 | | [OpenRouter](https://openrouter.ai/docs) | openrouter | 158 | 16 |
+158 | 2 | | [Perplexity](https://docs.perplexity.ai/docs/getting-started) |
 perplexity | 7 | 0 | 0 | 2 | | [å¤©å·¥](https://model-platform.tiangong.cn/api-
 reference) | skywork | 1 | 0 | 0 | 0 | | [é¶è·æè¾°](https://
-platform.stepfun.com/docs/Chat/chat-completion-create) | stepfun | 3 | 1 | 0 |
+platform.stepfun.com/docs/Chat/chat-completion-create) | stepfun | 6 | 2 | 0 |
 0 | | [Together AI](https://docs.together.ai/docs/quickstart) | together | 58 |
 0 | 58 | 0 | | [æºè°±](https://open.bigmodel.cn/dev/api) | zhipu | 5 | 1 | 4 |
 2 | | OpenAI æ¥å£å¼å®¹çæå¡ | openai-compatible | | | | | | Ollama API |
 ollama | | | | | ## å®è£ ```shell pip install ullm ``` ## ä½¿ç¨ ###
 åå»ºæ¨¡åéç½® ç¤ºä¾: ```python model_config = { # required fields "type":
 'remote', "model": 'gpt-3.5-turbo', "provider": 'openai', "api_key": 'sk-
 ************************************************', # optional fields
```

### Comparing `ullm-0.2.0/pyproject.toml` & `ullm-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ullm"
-version = "0.2.0"
+version = "0.3.0"
 description = "A unified interface for local Large Language Model(LLM) models and online LLM providers."
 authors = [
     {name = "Linusp", email = "linusp1024@gmail.com"},
 ]
 dependencies = [
     "pydantic",
     "arrow",
```

### Comparing `ullm-0.2.0/tests/test_openai.py` & `ullm-0.3.0/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/__init__.py` & `ullm-0.3.0/ullm/__init__.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/alibaba.py` & `ullm-0.3.0/ullm/alibaba.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,20 +183,22 @@
     _BASE_URL = "https://dashscope.aliyuncs.com/api/v1/services/aigc"
     META = RemoteLanguageModelMetaInfo(
         language_models=[
             # noqa: https://help.aliyun.com/zh/dashscope/developer-reference/api-details?spm=a2c4g.11186623.0.0.4070e0f6LPgURw#b8ebf6b25eul6
             "qwen-turbo",
             "qwen-plus",
             "qwen-max",
+            "qwen-max-0428",
             "qwen-max-0403",
             "qwen-max-0107",
             "qwen-max-longcontext",
             "qwen-turbo-online",
             "qwen-plus-online",
             "qwen-max-online",
+            "qwen-max-0428-online",
             "qwen-max-0403-online",
             "qwen-max-0107-online",
             "qwen-max-longcontext-online",
             # noqa: https://help.aliyun.com/zh/dashscope/developer-reference/api-details-11?spm=a2c4g.11186623.0.0.7d4d23edoHHGiM#8f79b5d0f8ker
             "llama2-7b-chat-v2",
             "llama2-13b-chat-v2",
             "llama3-8b-instruct",
@@ -240,22 +242,24 @@
             "qwen-vl-v1",
             "qwen-vl-chat-v1",
         ],
         tool_models=[
             "qwen-turbo",
             "qwen-plus",
             "qwen-max",
+            "qwen-max-0428",
             "qwen-max-0403",
             "qwen-max-0107",
             "qwen-max-longcontext",
         ],
         online_models=[
             "qwen-turbo-online",
             "qwen-plus-online",
             "qwen-max-online",
+            "qwen-max-0428-online",
             "qwen-max-0403-online",
             "qwen-max-0107-online",
             "qwen-max-longcontext-online",
         ],
         required_config_fields=["api_key"],
     )
     REQUEST_BODY_CLS = AlibabaRequestBody
```

### Comparing `ullm-0.2.0/ullm/anthropic.py` & `ullm-0.3.0/ullm/anthropic.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/baichuan.py` & `ullm-0.3.0/ullm/baichuan.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,109 +5,137 @@
 from .base import (
     AssistantMessage,
     ChatMessage,
     GenerateConfig,
     RemoteLanguageModel,
     RemoteLanguageModelMetaInfo,
     TextPart,
+    Tool,
+    ToolChoice,
     ToolMessage,
     UserMessage,
 )
 from .openai import (
     OpenAICompatibleModel,
+    OpenAIFunctionObject,
     OpenAIRequestBody,
+    OpenAIToolCall,
 )
 
 
 class BaichuanChatMessage(BaseModel):
-    role: Literal["user", "assistant"]
+    role: Literal["system", "user", "assistant", "tool"]
     content: str
+    # NOTE: https://platform.baichuan-ai.com/docs/api#12 文档上说 tool_calls 是 string 类型
+    #       但将 tool_calls json.dumps 后调用 API 会报错，按 OpenAI 的形式传入则正常
+    tool_calls: Optional[List[OpenAIToolCall]] = None
+    tool_call_id: Optional[str] = None
 
     @classmethod
     def from_standard(cls, message: ChatMessage):
         if isinstance(message, AssistantMessage):
             content = message.content
-            if message.tool_calls:  # NOTE: API 文档中未定义相关行为
-                content = ""
+            tool_calls = None
+            if message.tool_calls:
+                content, tool_calls = "", []
                 for tool_call in message.tool_calls:
-                    content += (
-                        f"You should call the function `{tool_call.function.name}` with arguments: "
-                        f"{tool_call.function.arguments}\n"
-                    )
+                    tool_calls.append(OpenAIToolCall.from_standard(tool_call))
 
-            return BaichuanChatMessage(role="assistant", content=content.strip())
+            return cls(role="assistant", content=content.strip(), tool_calls=tool_calls)
 
         if isinstance(message, UserMessage):
             content = ""
             for part in message.content:
                 if isinstance(part, TextPart):
                     content += part.text + "\n"
                 else:
                     pass
 
-            return BaichuanChatMessage(role="user", content=content.strip())
+            return cls(role="user", content=content.strip())
 
         if isinstance(message, ToolMessage):
-            content = (
-                f"I called the function `{message.tool_name}` and "
-                f"the response of that function is: {message.tool_result}"
-            )
-            return cls(role="user", content=content)
+            return cls(role="tool", content=message.tool_result, tool_call_id=message.tool_call_id)
 
 
 class BaichuanRetrievalObject(BaseModel):
     kb_ids: List[str]
     answer_mode: Optional[Literal["knowledge-base-only"]] = None
 
 
+class BaichuanWebSearchObject(BaseModel):
+    enable: Optional[bool] = False
+    search_mode: Optional[Literal["performance_first", "quality_first"]] = "performance_first"
+
+
+BaichuanFunctionObject = OpenAIFunctionObject
+
+
 class BaichuanTool(BaseModel):
-    type: Literal["retrieval"] = "retrieval"
-    retrieval: BaichuanRetrievalObject
+    type: Optional[Literal["web_search", "retrieval", "function"]] = None
+    retrieval: Optional[BaichuanRetrievalObject] = None
+    web_search: Optional[BaichuanRetrievalObject] = None
+    function: Optional[BaichuanFunctionObject] = None
+
+    @classmethod
+    def from_standard(cls, tool: Tool):
+        return cls(type=tool.type, function=BaichuanFunctionObject.from_standard(tool.function))
 
 
 class BaichuanRequestBody(OpenAIRequestBody):
     # reference: https://platform.baichuan-ai.com/docs/api#12
     ## excluded parameters
     frequency_penalty: Optional[Any] = Field(None, exclude=True)
     logit_bias: Optional[Any] = Field(None, exclude=True)
     logprobs: Optional[Any] = Field(None, exclude=True)
     top_logprobs: Optional[Any] = Field(None, exclude=True)
     n: Optional[Any] = Field(None, exclude=True)
     presence_penalty: Optional[Any] = Field(None, exclude=True)
     response_format: Optional[Any] = Field(None, exclude=True)
     seed: Optional[Any] = Field(None, exclude=True)
     stop: Optional[Any] = Field(None, exclude=True)
-    tool_choice: Optional[Any] = Field(None, exclude=True)
     user: Optional[Any] = Field(None, exclude=True)
 
     ## different parameters
     messages: conlist(BaichuanChatMessage, min_length=1)
     tools: Optional[List[BaichuanTool]] = None
+    tool_choice: Optional[Literal["auto", "none"]] = None
 
     ## Baichuan-specific parameters
     top_k: Optional[conint(ge=0, le=20)] = None
-    with_search_enhance: Optional[bool] = False
 
 
 @RemoteLanguageModel.register("baichuan")
 class BaichuanModel(OpenAICompatibleModel):
     # reference: https://platform.baichuan-ai.com/docs/api
     META = RemoteLanguageModelMetaInfo(
         api_url="https://api.baichuan-ai.com/v1/chat/completions",
         language_models=[
             "Baichuan2-Turbo",
             "Baichuan2-Turbo-192k",
             "Baichuan2-Turbo-online",
             "Baichuan2-Turbo-192k-online",
+            "Baichuan3-Turbo",
+            "Baichuan3-Turbo-128k",
+            "Baichuan3-Turbo-online",
+            "Baichuan3-Turbo-128k-online",
+            "Baichuan4",
+            "Baichuan4-online",
         ],
         visual_language_models=[],
-        tool_models=[],
+        tool_models=[
+            "Baichuan3-Turbo",
+            "Baichuan3-Turbo-128k",
+            "Baichuan4",
+        ],
         online_models=[
             "Baichuan2-Turbo-online",
             "Baichuan2-Turbo-192k-online",
+            "Baichuan3-Turbo-online",
+            "Baichuan3-Turbo-128k-online",
+            "Baichuan4-online",
         ],
         required_config_fields=["api_key"],
     )
     REQUEST_BODY_CLS = BaichuanRequestBody
 
     @classmethod
     @validate_call
@@ -118,24 +146,41 @@
     def _convert_messages(
         self,
         messages: conlist(ChatMessage, min_length=1),
         system: Optional[str] = None,
     ) -> Dict[str, Any]:
         messages = [self._convert_message(message) for message in messages]
         if system:
-            # NOTE: 百川不支持 system 参数
-            messages = [BaichuanChatMessage(role="user", content=system)] + messages
+            messages = [BaichuanChatMessage(role="system", content=system)] + messages
 
         return {"messages": messages}
 
+    @validate_call
+    def _convert_tools(
+        self, tools: Optional[List[Tool]] = None, tool_choice: Optional[ToolChoice] = None
+    ) -> Dict[str, Any]:
+        if tools:
+            tools = [BaichuanTool.from_standard(tool) for tool in tools]
+
+        baichuan_tool_choice = None
+        if tools and tool_choice is not None:
+            baichuan_tool_choice = tool_choice.mode
+            if baichuan_tool_choice == "any":
+                baichuan_tool_choice = "auto"
+
+        return {"tools": tools, "tool_choice": baichuan_tool_choice}
+
     def _convert_generation_config(
         self, config: GenerateConfig, system: Optional[str] = None
     ) -> Dict[str, Any]:
-        return {
+        generation_config = {
             "model": self.model.replace("-online", ""),
             "max_tokens": config.max_output_tokens or self.config.max_output_tokens,
             "stop": config.stop_sequences or self.config.stop_sequences,
             "temperature": config.temperature or self.config.temperature,
             "top_p": config.top_p or self.config.top_p,
             "top_k": config.top_k or self.config.top_k,
-            "with_search_enhance": self.is_online_model(),
         }
+        if self.is_online_model():
+            generation_config["tools"] = [{"type": "web_search", "web_search": {"enable": True}}]
+
+        return generation_config
```

### Comparing `ullm-0.2.0/ullm/baidu.py` & `ullm-0.3.0/ullm/baidu.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,21 +224,23 @@
     META = RemoteLanguageModelMetaInfo(
         model_api_url_mappings={
             "ERNIE-4.0-8K": f"{_BASE_URL}/chat/completions_pro",
             "ERNIE-4.0-8K-Preemptible": f"{_BASE_URL}/chat/completions_pro_preemptible",
             "ERNIE-4.0-8K-Preview": f"{_BASE_URL}/chat/ernie-4.0-8k-preview",
             "ERNIE-4.0-8K-0329": f"{_BASE_URL}/chat/ernie-4.0-8k-0329",
             "ERNIE-4.0-8K-0104": f"{_BASE_URL}/chat/ernie-4.0-8k-0104",
+            "ERNIE-4.0-8K-Preview-0518": f"{_BASE_URL}/chat/completions_adv_pro",
             "ERNIE-3.5-8K": f"{_BASE_URL}/chat/completions",
             "ERNIE-3.5-8K-0329": f"{_BASE_URL}/chat/ernie-3.5-8k-0329",
             "ERNIE-3.5-8K-0205": f"{_BASE_URL}/chat/ernie-3.5-8k-0205",
             "ERNIE-3.5-8K-1222": f"{_BASE_URL}/chat/ernie-3.5-8k-1222",
             "ERNIE-3.5-4K-0205": f"{_BASE_URL}/chat/ernie-3.5-4k-0205",
             "ERNIE-3.5-8K-Preemptible": f"{_BASE_URL}/chat/completions_preemptible",
             "ERNIE-3.5-8K-Preview": f"{_BASE_URL}/chat/ernie-3.5-8k-preview",
+            "ERNIE-3.5-128K": f"{_BASE_URL}/chat/ernie-3.5-128k",
             "ERNIE-Speed-8K": f"{_BASE_URL}/chat/ernie_speed",
             "ERNIE-Speed-128K": f"{_BASE_URL}/chat/ernie-speed-128k",
             "ERNIE-Lite-8K-0922": f"{_BASE_URL}/chat/eb-instant",
             "ERNIE-Lite-8K-0308": f"{_BASE_URL}/chat/ernie-lite-8k",
             # ERNIE-Lite-8K-0725/ERNIE-Lite-4K-0704/ERNIE-Lite-4K-0516/ERNIE-Lite-128K-0419
             # 需要用户自己部署
             "ERNIE-Tiny-8K": f"{_BASE_URL}/chat/ernie-tiny-8k",
@@ -249,14 +251,15 @@
             "Gemma-7B-it": f"{_BASE_URL}/chat/gemma_7b_it",
             "Yi-34B-Chat": f"{_BASE_URL}/chat/yi_34b_chat",
             "Mixtral-8x7B-Instruct": f"{_BASE_URL}/chat/mixtral_8x7b_instruct",
             # Mistral-7B-Instruct 需要用户自己部署
             # Qianfan-Chinese-Llama-2-7B-32K, Qianfan-Chinese-Llama-2-13B-v2 需要用户自己部署
             "Qianfan-Chinese-Llama-2-7B": f"{_BASE_URL}/chat/qianfan_chinese_llama_2_7b",
             "Qianfan-Chinese-Llama-2-13B-v1": f"{_BASE_URL}/chat/qianfan_chinese_llama_2_13b",
+            "Qianfan_Chinese_Llama_2-70B": f"{_BASE_URL}/chat/qianfan_chinese_llama_2_70b",
             # Qianfan-Chinese-Llama-2-70B/Qianfan-Chinese-Llama-2-1.3B 需要用户自己部署
             # Qianfan-Llama-2-70B-compressed 需要用户自己部署
             # Linly-Chinese-LLaMA-2-7B, Linly-Chinese-LLaMA-2-13B 需要用户自己部署
             "Llama-2-7b-chat": f"{_BASE_URL}/chat/llama_2_7b",
             "Llama-2-13b-chat": f"{_BASE_URL}/chat/llama_2_13b",
             "Llama-2-70b-chat": f"{_BASE_URL}/chat/llama_2_70b",
             "Meta-Llama-3-8B-Instruct": f"{_BASE_URL}/chat/llama_3_8b",
@@ -281,45 +284,50 @@
         },
         language_models=[
             "ERNIE-4.0-8K",
             "ERNIE-4.0-8K-Preemptible",
             "ERNIE-4.0-8K-Preview",
             "ERNIE-4.0-8K-0329",
             "ERNIE-4.0-8K-0104",
+            "ERNIE-4.0-8K-Preview-0518",
             "ERNIE-4.0-8K-online",
             "ERNIE-4.0-8K-Preemptible-online",
             "ERNIE-4.0-8K-Preview-online",
             "ERNIE-4.0-8K-0329-online",
             "ERNIE-4.0-8K-0104-online",
+            "ERNIE-4.0-8K-Preview-0518-online",
             "ERNIE-3.5-8K",
             "ERNIE-3.5-8K-0329",
             "ERNIE-3.5-8K-0205",
             "ERNIE-3.5-8K-1222",
             "ERNIE-3.5-4K-0205",
             "ERNIE-3.5-8K-Preemptible",
             "ERNIE-3.5-8K-Preview",
+            "ERNIE-3.5-128K",
             "ERNIE-3.5-8K-online",
             "ERNIE-3.5-8K-0329-online",
             "ERNIE-3.5-8K-0205-online",
             "ERNIE-3.5-8K-1222-online",
             "ERNIE-3.5-4K-0205-online",
             "ERNIE-3.5-8K-Preemptible-online",
             "ERNIE-3.5-8K-Preview-online",
+            "ERNIE-3.5-128K-online",
             "ERNIE-Speed-8K",
             "ERNIE-Speed-128K",
             "ERNIE-Lite-8K-0922",
             "ERNIE-Lite-8K-0308",
             "ERNIE-Tiny-8K",
             "ERNIE-Character-8K-0321",
             "ERNIE-Functions-8K",
             "Gemma-7B-it",
             "Yi-34B-Chat",
             "Mixtral-8x7B-Instruct",
             "Qianfan-Chinese-Llama-2-7B",
             "Qianfan-Chinese-Llama-2-13B-v1",
+            "Qianfan_Chinese_Llama_2-70B",
             "Llama-2-7b-chat",
             "Llama-2-13b-chat",
             "Llama-2-70b-chat",
             "Meta-Llama-3-8B-Instruct",
             "Meta-Llama-3-70B-Instruct",
             "ChatGLM2-6B-32K",
             "XuanYuan-70B-Chat-4bit",
@@ -332,68 +340,76 @@
             # NOTE: ERNIE-4.0 模型的 API 文档中没有写支持 functions 参数，
             #       但实际测试传入 functions 参数后会起作用
             "ERNIE-4.0-8K",
             "ERNIE-4.0-8K-Preemptible",
             "ERNIE-4.0-8K-Preview",
             "ERNIE-4.0-8K-0329",
             "ERNIE-4.0-8K-0104",
+            "ERNIE-4.0-8K-Preview-0518",
             "ERNIE-4.0-8K-online",
             "ERNIE-4.0-8K-Preemptible-online",
             "ERNIE-4.0-8K-Preview-online",
             "ERNIE-4.0-8K-0329-online",
             "ERNIE-4.0-8K-0104-online",
+            "ERNIE-4.0-8K-Preview-0518-online",
             "ERNIE-3.5-8K",
             "ERNIE-3.5-8K-0329",
             "ERNIE-3.5-8K-0205",
             "ERNIE-3.5-8K-1222",
             "ERNIE-3.5-4K-0205",
             "ERNIE-3.5-8K-Preemptible",
             "ERNIE-3.5-8K-Preview",
+            "ERNIE-3.5-128K",
             "ERNIE-3.5-8K-online",
             "ERNIE-3.5-8K-0329-online",
             "ERNIE-3.5-8K-0205-online",
             "ERNIE-3.5-8K-1222-online",
             "ERNIE-3.5-4K-0205-online",
             "ERNIE-3.5-8K-Preemptible-online",
             "ERNIE-3.5-8K-Preview-online",
+            "ERNIE-3.5-128K-online",
             # NOTE: ERNIE-Functions-8K 简介里说说适合外部工具使用，但文档中无 functions 参数，
             #       传入 functions 后也无作用
         ],
         online_models=[
             "ERNIE-4.0-8K-online",
             "ERNIE-4.0-8K-Preemptible-online",
             "ERNIE-4.0-8K-Preview-online",
             "ERNIE-4.0-8K-0329-online",
             "ERNIE-4.0-8K-0104-online",
+            "ERNIE-4.0-8K-Preview-0518-online",
             "ERNIE-3.5-8K-online",
             "ERNIE-3.5-8K-0329-online",
             "ERNIE-3.5-8K-0205-online",
             "ERNIE-3.5-8K-1222-online",
             "ERNIE-3.5-4K-0205-online",
             "ERNIE-3.5-8K-Preemptible-online",
             "ERNIE-3.5-8K-Preview-online",
+            "ERNIE-3.5-128K-online",
         ],
         required_config_fields=["api_key", "secret_key"],
     )
     REQUEST_BODY_CLS = BaiduRequestBody
     RESPONSE_BODY_CLS = BaiduResponseBody
     _AUTH_URL = "https://aip.baidubce.com/oauth/2.0/token"
     _MODEL_EXCLUDE_REQUEST_KEYS = {
         "ERNIE-4.0-8K": ["top_k"],
         "ERNIE-4.0-8K-Preemptible": ["top_k"],
         "ERNIE-4.0-8K-Preview": ["top_k"],
         "ERNIE-4.0-8K-0329": ["top_k"],
         "ERNIE-4.0-8K-0104": ["top_k"],
+        "ERNIE-4.0-8K-Preview-0518": ["top_k"],
         "ERNIE-3.5-4K-0205": ["top_k"],
         "ERNIE-3.5-8K": ["top_k"],
         "ERNIE-3.5-8K-0205": ["top_k"],
         "ERNIE-3.5-8K-0329": ["top_k"],
         "ERNIE-3.5-8K-1222": ["top_k"],
         "ERNIE-3.5-8K-Preemptible": ["top_k"],
         "ERNIE-3.5-8K-Preview": ["top_k"],
+        "ERNIE-3.5-128K": ["top_k"],
         "ERNIE-Speed-8K": [
             "top_k",
             "response_format",
             "disable_search",
             "enable_citation",
             "enable_trace",
         ],
@@ -491,14 +507,22 @@
             "response_format",
             "max_output_tokens",
             "system",
             "disable_search",
             "enable_citation",
             "enable_trace",
         ],
+        "Qianfan-Chinese-Llama-2-70B": [
+            "response_format",
+            "max_output_tokens",
+            "system",
+            "disable_search",
+            "enable_citation",
+            "enable_trace",
+        ],
         "Llama-2-70b-chat": [
             "response_format",
             "max_output_tokens",
             "system",
             "disable_search",
             "enable_citation",
             "enable_trace",
```

### Comparing `ullm-0.2.0/ullm/base.py` & `ullm-0.3.0/ullm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,57 +236,83 @@
         raise NotImplementedError
 
 
 class RemoteLanguageModelConfig(ModelConfig):
     provider: str = Field(..., description="模型提供方名称")
     model: str = Field(..., description="模型名称")
     is_visual_model: Optional[bool] = Field(
-        False, description="该模型是否支持视觉理解，用于自定义服务", examples=[True, False]
+        False,
+        description="该模型是否支持视觉理解，用于自定义服务",
+        examples=[True, False],
+        json_schema_extra={"providers": ["openai-compatible"]},
     )
     is_tool_model: Optional[bool] = Field(
-        False, description="是否支持工具，用于自定义服务", examples=[True, False]
+        False,
+        description="是否支持工具，用于自定义服务",
+        examples=[True, False],
+        json_schema_extra={"providers": ["openai-compatible"]},
     )
     is_online_model: Optional[bool] = Field(
-        False, description="是否支持联网，用于自定义服务", examples=[True, False]
+        False,
+        description="是否支持联网，用于自定义服务",
+        examples=[True, False],
+        json_schema_extra={"providers": ["openai-compatible"]},
     )
     api_url: Optional[HttpUrl] = Field(
         None,
         description="有的 provider 并无公开的固定 URL 需要自己指定，如自己部署的 API 代理服务",
         examples=["http://example.com/api/v1/chat/completion"],
+        json_schema_extra={"providers": ["openai-compatible"]},
     )
     api_key: Optional[SecretStr] = Field(
         "", examples=["sk-************************************************"]
     )
     secret_key: Optional[SecretStr] = Field(
         "",
         description="讯飞星火 api_secret, 文心一言 secret key",
         examples=["c5ff5142b0b248d5885bac25352364eb"],
+        json_schema_extra={"providers": ["iflytek", "baidu"]},
     )
     azure_endpoint: Optional[str] = Field(
-        "", description="用于 Azure OpenAI", examples=["https://example-endpoint.openai.azure.com/"]
+        "",
+        description="用于 Azure OpenAI",
+        examples=["https://example-endpoint.openai.azure.com/"],
+        json_schema_extra={"providers": ["azure-openai"]},
     )
     azure_deployment_name: Optional[str] = Field(
-        "", description="用于 Azure OpenAI", examples=["gpt-35-turbo"]
+        "",
+        description="用于 Azure OpenAI",
+        examples=["gpt-35-turbo"],
+        json_schema_extra={"providers": ["azure-openai"]},
     )
     azure_api_version: Optional[str] = Field(
-        "2024-02-01", description="用于 Azure OpenAI", examples=["2024-02-01"]
+        "2024-02-01",
+        description="用于 Azure OpenAI",
+        examples=["2024-02-01"],
+        json_schema_extra={"providers": ["azure-openai"]},
+    )
+    app_id: Optional[str] = Field(
+        "",
+        description="讯飞星火需要",
+        examples=["404abcde"],
+        json_schema_extra={"providers": ["iflytek"]},
     )
-    app_id: Optional[str] = Field("", description="讯飞星火需要", examples=["404abcde"])
     max_tokens: Optional[PositiveInt] = Field(None, examples=[4096, 8192])
     max_input_tokens: Optional[PositiveInt] = Field(None, examples=[1024, 2048])
     max_output_tokens: Optional[PositiveInt] = Field(None, examples=[1024, 4096])
     temperature: Optional[NonNegativeFloat] = Field(None, examples=[0.7, 0.8])
     top_p: Optional[NonNegativeFloat] = Field(None, le=1.0, examples=[1.0])
     top_k: Optional[NonNegativeInt] = Field(None, examples=[50, 100])
     stop_sequences: Optional[List[str]] = Field(None, examples=[["stop1", "stop2"]])
     http_proxy: Optional[HttpUrl] = Field(None, examples=["https://example-proxy.com"])
     cf_account_id: Optional[SecretStr] = Field(
         None,
         description="Cloudflare Account ID",
         examples=["fe18f2a883e6401c9ee72ab358714088"],
+        json_schema_extra={"providers": ["cloudflare"]},
     )
 
 
 class RemoteLanguageModelMetaInfo(BaseModel):
     model_config = ConfigDict(protected_namespaces=())
 
     api_url: Optional[AnyUrl] = Field("", description="TODO")
@@ -377,28 +403,20 @@
         required_config = {"type": "remote", "model": example_model, "provider": provider}
         for field in meta.required_config_fields:
             required_config[field] = random.choice(
                 RemoteLanguageModelConfig.model_fields[field].examples
             )
 
         optional_config = {}
-        ignored_fields = [
-            "is_visual_model",
-            "is_online_model",
-            "is_tool_model",
-            "api_url",
-            "api_key",
-            "secret_key",
-            "app_id",
-            "azure_endpoint",
-            "azure_api_version",
-            "azure_deployment_name",
-        ]
         for field, field_info in RemoteLanguageModelConfig.model_fields.items():
-            if field in required_config or field in ignored_fields:
+            if field in required_config:
+                continue
+
+            extra = field_info.json_schema_extra
+            if extra and provider not in extra.get("providers", []):
                 continue
 
             optional_config[field] = random.choice(field_info.examples)
 
         return required_config, optional_config
 
     @classmethod
```

### Comparing `ullm-0.2.0/ullm/cli.py` & `ullm-0.3.0/ullm/cli.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/cloudflare.py` & `ullm-0.3.0/ullm/cloudflare.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/cohere.py` & `ullm-0.3.0/ullm/cohere.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/deepseek.py` & `ullm-0.3.0/ullm/deepseek.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/google.py` & `ullm-0.3.0/ullm/google.py`

 * *Files 7% similar despite different names*

```diff
@@ -332,17 +332,30 @@
 )
 
 
 @RemoteLanguageModel.register("google")
 class GoogleModel(HttpServiceModel):
     # https://ai.google.dev/gemini-api/docs/models/gemini
     _LANGUAGE_MODELS = [
+        "gemini-1.0-pro",
+        "gemini-1.0-pro-001",
+        "gemini-1.0-pro-latest",
         "gemini-pro",
     ]
-    _VISUAL_LANGUAGE_MODELS = ["gemini-pro-vision", "gemini-1.5-pro-latest"]
+    _VISUAL_LANGUAGE_MODELS = [
+        "gemini-1.0-pro-vision",
+        "gemini-1.0-pro-vision-latest",
+        "gemini-pro-vision",
+        "gemini-1.5-flash",
+        "gemini-1.5-flash-001",
+        "gemini-1.5-flash-latest",
+        "gemini-1.5-pro",
+        "gemini-1.5-pro-001",
+        "gemini-1.5-pro-latest",
+    ]
 
     META = RemoteLanguageModelMetaInfo(
         model_api_url_mappings={
             model: GOOGLE_API_URL_TEMPLATE.format(model=model)
             for model in _LANGUAGE_MODELS + _VISUAL_LANGUAGE_MODELS
         },
         language_models=_LANGUAGE_MODELS,
```

### Comparing `ullm-0.2.0/ullm/groq.py` & `ullm-0.3.0/ullm/groq.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/iflytek.py` & `ullm-0.3.0/ullm/iflytek.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/minimax.py` & `ullm-0.3.0/ullm/minimax.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,22 +107,24 @@
 @RemoteLanguageModel.register("minimax")
 class MiniMaxModel(OpenAICompatibleModel):
     META = RemoteLanguageModelMetaInfo(
         api_url="https://api.minimax.chat/v1/text/chatcompletion_v2",
         language_models=[
             "abab6.5-chat",
             "abab6.5s-chat",
+            "abab6.5g-chat",
             "abab6-chat",
             "abab5.5-chat",
             "abab5.5s-chat",
         ],
         visual_language_models=[],
         tool_models=[
             "abab6.5-chat",
             "abab6.5s-chat",
+            "abab6.5g-chat",
             "abab6-chat",
             "abab5.5-chat",
             "abab5.5s-chat",
         ],
         required_config_fields=["api_key"],
     )
     REQUEST_BODY_CLS = MiniMaxRequestBody
```

### Comparing `ullm-0.2.0/ullm/moonshot.py` & `ullm-0.3.0/ullm/moonshot.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/ollama.py` & `ullm-0.3.0/ullm/ollama.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/openai.py` & `ullm-0.3.0/ullm/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,14 @@
             "gpt-4-0613",
             "gpt-4-1106-preview",
             "gpt-4-32k",
             "gpt-4-32k-0613",
             "gpt-4-turbo",
             "gpt-4-turbo-2024-04-09",
             "gpt-4-turbo-preview",
-            "gpt-4o",
         ],
         visual_language_models=[
             "gpt-4-vision-preview",
             "gpt-4-1106-vision-preview",
             "gpt-4-turbo",
             "gpt-4-turbo-2024-04-09",
             "gpt-4o",
```

### Comparing `ullm-0.2.0/ullm/openrouter.py` & `ullm-0.3.0/ullm/openrouter.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,37 +76,45 @@
 @RemoteLanguageModel.register("openrouter")
 class OpenRouterModel(OpenAICompatibleModel):
     # https://openrouter.ai/api/v1/models
     _FULL_SUPPORTED_MODELS = [
         "01-ai/yi-34b",
         "01-ai/yi-34b-chat",
         "01-ai/yi-6b",
+        "allenai/olmo-7b-instruct",
         "alpindale/goliath-120b",
+        "anthropic/claude-1",
+        "anthropic/claude-1.2",
         "anthropic/claude-2",
         "anthropic/claude-2.0",
         "anthropic/claude-2.0:beta",
         "anthropic/claude-2.1",
         "anthropic/claude-2.1:beta",
         "anthropic/claude-2:beta",
         "anthropic/claude-3-haiku",
         "anthropic/claude-3-haiku:beta",
         "anthropic/claude-3-opus",
         "anthropic/claude-3-opus:beta",
         "anthropic/claude-3-sonnet",
         "anthropic/claude-3-sonnet:beta",
         "anthropic/claude-instant-1",
+        "anthropic/claude-instant-1.0",
+        "anthropic/claude-instant-1.1",
         "anthropic/claude-instant-1:beta",
         "austism/chronos-hermes-13b",
         "codellama/codellama-70b-instruct",
         "cognitivecomputations/dolphin-mixtral-8x7b",
         "cohere/command",
         "cohere/command-r",
         "cohere/command-r-plus",
         "databricks/dbrx-instruct",
+        "deepseek/deepseek-chat",
+        "deepseek/deepseek-coder",
         "fireworks/firellava-13b",
+        "google/gemini-flash-1.5",
         "google/gemini-pro",
         "google/gemini-pro-1.5",
         "google/gemini-pro-vision",
         "google/gemma-7b-it",
         "google/gemma-7b-it:free",
         "google/gemma-7b-it:nitro",
         "google/palm-2-chat-bison",
@@ -114,85 +122,107 @@
         "google/palm-2-codechat-bison",
         "google/palm-2-codechat-bison-32k",
         "gryphe/mythomax-l2-13b",
         "gryphe/mythomax-l2-13b:extended",
         "gryphe/mythomax-l2-13b:nitro",
         "gryphe/mythomist-7b",
         "gryphe/mythomist-7b:free",
-        "haotian-liu/llava-13b",
+        "huggingfaceh4/zephyr-7b-beta",
         "huggingfaceh4/zephyr-7b-beta:free",
         "intel/neural-chat-7b",
+        "jebcarter/psyfighter-13b",
         "jondurbin/airoboros-l2-70b",
+        "jondurbin/bagel-34b",
         "koboldai/psyfighter-13b-2",
+        "liuhaotian/llava-13b",
+        "liuhaotian/llava-yi-34b",
         "lizpreciatior/lzlv-70b-fp16-hf",
         "lynn/soliloquy-l3",
         "mancer/weaver",
         "meta-llama/codellama-34b-instruct",
         "meta-llama/llama-2-13b-chat",
         "meta-llama/llama-2-70b-chat",
         "meta-llama/llama-2-70b-chat:nitro",
+        "meta-llama/llama-3-70b",
         "meta-llama/llama-3-70b-instruct",
         "meta-llama/llama-3-70b-instruct:nitro",
+        "meta-llama/llama-3-8b",
         "meta-llama/llama-3-8b-instruct",
         "meta-llama/llama-3-8b-instruct:extended",
+        "meta-llama/llama-3-8b-instruct:free",
         "meta-llama/llama-3-8b-instruct:nitro",
+        "meta-llama/llama-guard-2-8b",
+        "microsoft/phi-3-medium-128k-instruct",
+        "microsoft/phi-3-medium-128k-instruct:free",
+        "microsoft/phi-3-mini-128k-instruct",
+        "microsoft/phi-3-mini-128k-instruct:free",
         "microsoft/wizardlm-2-7b",
         "microsoft/wizardlm-2-8x22b",
-        "microsoft/wizardlm-2-8x22b:nitro",
         "mistralai/mistral-7b-instruct",
         "mistralai/mistral-7b-instruct:free",
         "mistralai/mistral-7b-instruct:nitro",
         "mistralai/mistral-large",
         "mistralai/mistral-medium",
         "mistralai/mistral-small",
         "mistralai/mistral-tiny",
         "mistralai/mixtral-8x22b",
         "mistralai/mixtral-8x22b-instruct",
         "mistralai/mixtral-8x7b",
         "mistralai/mixtral-8x7b-instruct",
         "mistralai/mixtral-8x7b-instruct:nitro",
+        "neversleep/llama-3-lumimaid-70b",
         "neversleep/llama-3-lumimaid-8b",
         "neversleep/llama-3-lumimaid-8b:extended",
         "neversleep/noromaid-20b",
         "neversleep/noromaid-mixtral-8x7b-instruct",
+        "nousresearch/hermes-2-pro-llama-3-8b",
         "nousresearch/nous-capybara-34b",
         "nousresearch/nous-capybara-7b",
         "nousresearch/nous-capybara-7b:free",
         "nousresearch/nous-hermes-2-mistral-7b-dpo",
         "nousresearch/nous-hermes-2-mixtral-8x7b-dpo",
         "nousresearch/nous-hermes-2-mixtral-8x7b-sft",
         "nousresearch/nous-hermes-2-vision-7b",
         "nousresearch/nous-hermes-llama2-13b",
         "nousresearch/nous-hermes-yi-34b",
         "open-orca/mistral-7b-openorca",
         "openai/gpt-3.5-turbo",
         "openai/gpt-3.5-turbo-0125",
+        "openai/gpt-3.5-turbo-0301",
+        "openai/gpt-3.5-turbo-0613",
+        "openai/gpt-3.5-turbo-1106",
         "openai/gpt-3.5-turbo-16k",
         "openai/gpt-3.5-turbo-instruct",
         "openai/gpt-4",
+        "openai/gpt-4-0314",
+        "openai/gpt-4-1106-preview",
         "openai/gpt-4-32k",
+        "openai/gpt-4-32k-0314",
         "openai/gpt-4-turbo",
         "openai/gpt-4-turbo-preview",
         "openai/gpt-4-vision-preview",
         "openai/gpt-4o",
+        "openai/gpt-4o-2024-05-13",
         "openchat/openchat-7b",
         "openchat/openchat-7b:free",
         "openrouter/auto",
         "openrouter/cinematika-7b",
         "openrouter/cinematika-7b:free",
-        "perplexity/pplx-70b-chat",
-        "perplexity/pplx-70b-online",
-        "perplexity/pplx-7b-chat",
-        "perplexity/pplx-7b-online",
-        "perplexity/sonar-medium-chat",
-        "perplexity/sonar-medium-online",
-        "perplexity/sonar-small-chat",
-        "perplexity/sonar-small-online",
+        "perplexity/llama-3-sonar-large-32k-chat",
+        "perplexity/llama-3-sonar-large-32k-online",
+        "perplexity/llama-3-sonar-small-32k-chat",
+        "perplexity/llama-3-sonar-small-32k-online",
         "phind/phind-codellama-34b",
         "pygmalionai/mythalion-13b",
+        "qwen/qwen-110b-chat",
+        "qwen/qwen-14b-chat",
+        "qwen/qwen-32b-chat",
+        "qwen/qwen-4b-chat",
+        "qwen/qwen-72b-chat",
+        "qwen/qwen-7b-chat",
         "recursal/eagle-7b",
         "recursal/rwkv-5-3b-ai-town",
         "rwkv/rwkv-5-world-3b",
         "sao10k/fimbulvetr-11b-v2",
         "snowflake/snowflake-arctic-instruct",
         "sophosympatheia/midnight-rose-70b",
         "teknium/openhermes-2-mistral-7b",
@@ -215,29 +245,29 @@
         "claude-3-haiku:beta",
         "claude-3-opus",
         "claude-3-opus:beta",
         "claude-3-sonnet",
         "claude-3-sonnet:beta",
         "firellava-13b",  # https://openrouter.ai/models/fireworks/firellava-13b
         "gemini-pro-vision",
+        "gemini-flash-1.5",
         "gemini-pro-1.5",
         "gpt-4-turbo",
         "gpt-4-vision-preview",
         "gpt-4o",
         "llava-13b",  # https://openrouter.ai/models/haotian-liu/llava-13b
+        "llava-yi-34b",
         "nous-hermes-2-vision-7b",  # https://openrouter.ai/models/nousresearch/nous-hermes-2-vision-7b
     ]
     META = RemoteLanguageModelMetaInfo(
         api_url="https://openrouter.ai/api/v1/chat/completions",
         required_config_fields=["api_key"],
         language_models=set(_SUPPORTED_MODELS) - set(_VISUAL_MODELS),
         visual_language_models=_VISUAL_MODELS,
         tool_models=_SUPPORTED_MODELS,
         online_models=[
-            "pplx-70b-online",
-            "pplx-7b-online",
-            "sonar-medium-online",
-            "sonar-small-online",
+            "llama-3-sonar-large-32k-online",
+            "llama-3-sonar-small-32k-online",
         ],
     )
     REQUEST_BODY_CLS = OpenRouterRequestBody
     RESPONSE_BODY_CLS = OpenRouterResponseBody
```

### Comparing `ullm-0.2.0/ullm/perplexity.py` & `ullm-0.3.0/ullm/perplexity.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/skywork.py` & `ullm-0.3.0/ullm/skywork.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/stepfun.py` & `ullm-0.3.0/ullm/stepfun.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,21 @@
 
 @RemoteLanguageModel.register("stepfun")
 class StepFunModel(OpenAICompatibleModel):
     # reference: https://platform.openai.com/docs/models/overview
     META = RemoteLanguageModelMetaInfo(
         api_url="https://api.stepfun.com/v1/chat/completions",
         language_models=[
+            "step-1-8k",
             "step-1-32k",
-            "step-1-200k",
+            "step-1-128k",
+            "step-1-256k",
         ],
         visual_language_models=[
+            "step-1v-8k",
             "step-1v-32k",
         ],
         tool_models=[],
         online_models=[],
         required_config_fields=["api_key"],
     )
     REQUEST_BODY_CLS = StepFunRequestBody
```

### Comparing `ullm-0.2.0/ullm/together.py` & `ullm-0.3.0/ullm/together.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm/zhipu.py` & `ullm-0.3.0/ullm/zhipu.py`

 * *Files identical despite different names*

### Comparing `ullm-0.2.0/ullm.egg-info/PKG-INFO` & `ullm-0.3.0/ullm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ullm
-Version: 0.2.0
+Version: 0.3.0
 Summary: A unified interface for local Large Language Model(LLM) models and online LLM providers.
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/monsternlp/ullm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -90,33 +90,33 @@
 
 TBD
 
 ### 在线服务
 
 | 平台 | Provider ID            | 模型数量 | 视觉模型数量 | 支持工具调用的模型数量 | 联网模型数量 |
 |------|-------------------|----------|--------------|------------------------|--------------|
-| [零一万物](https://platform.lingyiwanwu.com/docs)     | 01ai              |        3 |            1 |                      0 |            0 |
-| [阿里巴巴](https://help.aliyun.com/zh/dashscope/developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT)      | alibaba           |       44 |            4 |                      6 |            6 |
+| [零一万物](https://platform.lingyiwanwu.com/docs)     | 01ai              |        9 |            1 |                      0 |            2 |
+| [阿里巴巴](https://help.aliyun.com/zh/dashscope/developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT)      | alibaba           |       46 |            4 |                      7 |            7 |
 | [Anthropic](https://docs.anthropic.com/claude/reference/getting-started-with-the-api)     | anthropic         |        3 |            3 |                      3 |            0 |
 | [Azure OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/reference#chat-completions)     | azure-openai      |       20 |            4 |                     11 |            0 |
-| [百川智能](https://platform.baichuan-ai.com/docs/api)     | baichuan          |        4 |            0 |                      0 |            2 |
-| [百度](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu)     | baidu             |       46 |            0 |                     24 |           12 |
+| [百川智能](https://platform.baichuan-ai.com/docs/api)     | baichuan          |        10 |            0 |                      3 |            5 |
+| [百度](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu)     | baidu             |       51 |            0 |                     28 |           14 |
 | [Cloudflare Workers AI](https://developers.cloudflare.com/workers-ai/get-started/rest-api/) | cloudflare        |       35 |               0 |             0 |               0 |
 | [Cohere](https://docs.cohere.com/reference/about)     | cohere            |       12 |            0 |                      4 |            6 |
 | [DeepSeek](https://platform.deepseek.com/docs)     | deepseek          |        2 |            0 |                      0 |            0 |
-| [Google](https://ai.google.dev/gemini-api/docs)     | google            |        3 |            2 |                      2 |            0 |
+| [Google](https://ai.google.dev/gemini-api/docs)     | google            |        13 |            9 |                      2 |            0 |
 | [Groq](https://console.groq.com/docs/quickstart)     | groq              |        4 |            0 |                      4 |            0 |
 | [科大讯飞](https://www.xfyun.cn/doc/spark/%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E.html)     | iflytek           |        4 |            0 |                      2 |            0 |
-| [MiniMax](https://www.minimaxi.com/document/algorithm-concept?id=6433f37594878d408fc8295d)     | minimax           |        5 |            0 |                      5 |            0 |
+| [MiniMax](https://www.minimaxi.com/document/algorithm-concept?id=6433f37594878d408fc8295d)     | minimax           |        6 |            0 |                      6 |            0 |
 | [Moonshot](https://platform.moonshot.cn/docs/api/chat#%E5%9F%BA%E6%9C%AC%E4%BF%A1%E6%81%AF)     | moonshot          |        3 |            0 |                      3 |            0 |
-| [OpenAI](https://platform.openai.com/docs/api-reference/chat)      | openai            |       20 |            4 |                     11 |            0 |
-| [OpenRouter](https://openrouter.ai/docs)     | openrouter        |      127 |           13 |                    127 |            4 |
+| [OpenAI](https://platform.openai.com/docs/api-reference/chat)      | openai            |       21 |            5 |                     12 |            0 |
+| [OpenRouter](https://openrouter.ai/docs)     | openrouter        |      158 |           16 |                    158 |            2 |
 | [Perplexity](https://docs.perplexity.ai/docs/getting-started)     | perplexity        |        7 |            0 |                      0 |            2 |
 | [天工](https://model-platform.tiangong.cn/api-reference) | skywork           |        1 |               0 |             0 |               0 |
-| [阶跃星辰](https://platform.stepfun.com/docs/Chat/chat-completion-create)     | stepfun           |        3 |            1 |                      0 |            0 |
+| [阶跃星辰](https://platform.stepfun.com/docs/Chat/chat-completion-create)     | stepfun           |        6 |            2 |                      0 |            0 |
 | [Together AI](https://docs.together.ai/docs/quickstart) | together          |       58 |               0 |            58 |               0 |
 | [智谱](https://open.bigmodel.cn/dev/api)     | zhipu             |        5 |            1 |                      4 |            2 |
 | OpenAI 接口兼容的服务     | openai-compatible |          |              |                        |              |
 | Ollama API     | ollama            |          |              |                        |              |
 
 
 ## 安装
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ullm Version: 0.2.0 Summary: A unified interface
+Metadata-Version: 2.1 Name: ullm Version: 0.3.0 Summary: A unified interface
 for local Large Language Model(LLM) models and online LLM providers. Author-
 email: Linusp
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/monsternlp/
 ullm Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist: pydantic
 Requires-Dist: arrow Requires-Dist: websocket-client Requires-Dist: requests
@@ -39,40 +39,40 @@
 tokenizerï¼ä»¥è·å¾ tokens æ°éè§£å³æäº remote model ä¸è¿å tokens
 æ°éçé®é¢ - [ ] æ¨¡åéç½®çç®¡ç - [ ] å¤æ¨¡åè·¯ç± - [ ]
 ååæµè¯ - [ ] å®åææ¡£ - [ ] å®ç°æµå¼æ¥å£ ## æ¯ææ¨¡å ###
 æ¬å°æ¨¡å TBD ### å¨çº¿æå¡ | å¹³å° | Provider ID | æ¨¡åæ°é |
 è§è§æ¨¡åæ°é | æ¯æå·¥å·è°ç¨çæ¨¡åæ°é | èç½æ¨¡åæ°é |
 |------|-------------------|----------|--------------|------------------------
 |--------------| | [é¶ä¸ä¸ç©](https://platform.lingyiwanwu.com/docs) | 01ai
-| 3 | 1 | 0 | 0 | | [é¿éå·´å·´](https://help.aliyun.com/zh/dashscope/
+| 9 | 1 | 0 | 2 | | [é¿éå·´å·´](https://help.aliyun.com/zh/dashscope/
 developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT) |
-alibaba | 44 | 4 | 6 | 6 | | [Anthropic](https://docs.anthropic.com/claude/
+alibaba | 46 | 4 | 7 | 7 | | [Anthropic](https://docs.anthropic.com/claude/
 reference/getting-started-with-the-api) | anthropic | 3 | 3 | 3 | 0 | | [Azure
 OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/
 reference#chat-completions) | azure-openai | 20 | 4 | 11 | 0 | | [ç¾å·æºè½]
-(https://platform.baichuan-ai.com/docs/api) | baichuan | 4 | 0 | 0 | 2 | |
-[ç¾åº¦](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu) | baidu | 46 |
-0 | 24 | 12 | | [Cloudflare Workers AI](https://developers.cloudflare.com/
+(https://platform.baichuan-ai.com/docs/api) | baichuan | 10 | 0 | 3 | 5 | |
+[ç¾åº¦](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu) | baidu | 51 |
+0 | 28 | 14 | | [Cloudflare Workers AI](https://developers.cloudflare.com/
 workers-ai/get-started/rest-api/) | cloudflare | 35 | 0 | 0 | 0 | | [Cohere]
 (https://docs.cohere.com/reference/about) | cohere | 12 | 0 | 4 | 6 | |
 [DeepSeek](https://platform.deepseek.com/docs) | deepseek | 2 | 0 | 0 | 0 | |
-[Google](https://ai.google.dev/gemini-api/docs) | google | 3 | 2 | 2 | 0 | |
+[Google](https://ai.google.dev/gemini-api/docs) | google | 13 | 9 | 2 | 0 | |
 [Groq](https://console.groq.com/docs/quickstart) | groq | 4 | 0 | 4 | 0 | |
 [ç§å¤§è®¯é£](https://www.xfyun.cn/doc/spark/
 %E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E.html) | iflytek | 4 | 0 | 2 | 0 | |
 [MiniMax](https://www.minimaxi.com/document/algorithm-
-concept?id=6433f37594878d408fc8295d) | minimax | 5 | 0 | 5 | 0 | | [Moonshot]
+concept?id=6433f37594878d408fc8295d) | minimax | 6 | 0 | 6 | 0 | | [Moonshot]
 (https://platform.moonshot.cn/docs/api/
 chat#%E5%9F%BA%E6%9C%AC%E4%BF%A1%E6%81%AF) | moonshot | 3 | 0 | 3 | 0 | |
-[OpenAI](https://platform.openai.com/docs/api-reference/chat) | openai | 20 | 4
-| 11 | 0 | | [OpenRouter](https://openrouter.ai/docs) | openrouter | 127 | 13 |
-127 | 4 | | [Perplexity](https://docs.perplexity.ai/docs/getting-started) |
+[OpenAI](https://platform.openai.com/docs/api-reference/chat) | openai | 21 | 5
+| 12 | 0 | | [OpenRouter](https://openrouter.ai/docs) | openrouter | 158 | 16 |
+158 | 2 | | [Perplexity](https://docs.perplexity.ai/docs/getting-started) |
 perplexity | 7 | 0 | 0 | 2 | | [å¤©å·¥](https://model-platform.tiangong.cn/api-
 reference) | skywork | 1 | 0 | 0 | 0 | | [é¶è·æè¾°](https://
-platform.stepfun.com/docs/Chat/chat-completion-create) | stepfun | 3 | 1 | 0 |
+platform.stepfun.com/docs/Chat/chat-completion-create) | stepfun | 6 | 2 | 0 |
 0 | | [Together AI](https://docs.together.ai/docs/quickstart) | together | 58 |
 0 | 58 | 0 | | [æºè°±](https://open.bigmodel.cn/dev/api) | zhipu | 5 | 1 | 4 |
 2 | | OpenAI æ¥å£å¼å®¹çæå¡ | openai-compatible | | | | | | Ollama API |
 ollama | | | | | ## å®è£ ```shell pip install ullm ``` ## ä½¿ç¨ ###
 åå»ºæ¨¡åéç½® ç¤ºä¾: ```python model_config = { # required fields "type":
 'remote', "model": 'gpt-3.5-turbo', "provider": 'openai', "api_key": 'sk-
 ************************************************', # optional fields
```

### Comparing `ullm-0.2.0/ullm.egg-info/SOURCES.txt` & `ullm-0.3.0/ullm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

