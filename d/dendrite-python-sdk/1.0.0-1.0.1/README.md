# Comparing `tmp/dendrite_python_sdk-1.0.0.tar.gz` & `tmp/dendrite_python_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dendrite_python_sdk-1.0.0.tar", max compression
+gzip compressed data, was "dendrite_python_sdk-1.0.1.tar", max compression
```

## Comparing `dendrite_python_sdk-1.0.0.tar` & `dendrite_python_sdk-1.0.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     1074 2024-02-02 14:20:43.049218 dendrite_python_sdk-1.0.0/LICENSE
--rw-r--r--   0        0        0     6707 2024-05-26 16:58:56.466954 dendrite_python_sdk-1.0.0/README.md
--rw-r--r--   0        0        0       62 2024-05-15 17:53:47.139877 dendrite_python_sdk-1.0.0/dendrite_python_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 08:59:27.558957 dendrite_python_sdk-1.0.0/dendrite_python_sdk/ai_util/__init__.py
--rw-r--r--   0        0        0      196 2024-05-20 09:08:52.601223 dendrite_python_sdk-1.0.0/dendrite_python_sdk/ai_util/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4434 2024-05-26 16:15:03.183234 dendrite_python_sdk-1.0.0/dendrite_python_sdk/ai_util/__pycache__/generate_text.cpython-312.pyc
--rw-r--r--   0        0        0     2898 2024-05-26 16:15:03.183642 dendrite_python_sdk-1.0.0/dendrite_python_sdk/ai_util/generate_text.py
--rw-r--r--   0        0        0     2361 2024-05-17 11:11:36.767261 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/ActivePageManager.py
--rw-r--r--   0        0        0     4580 2024-05-26 16:15:03.184074 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/DendriteBrowser.py
--rw-r--r--   0        0        0     4849 2024-05-17 11:39:53.139850 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/DendriteLocator.py
--rw-r--r--   0        0        0     6384 2024-05-26 16:58:56.468040 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/DendritePage.py
--rw-r--r--   0        0        0     1620 2024-05-26 16:15:03.184385 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/ScreenshotManager.py
--rw-r--r--   0        0        0     4301 2024-05-17 11:13:52.699998 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/ActivePageManager.cpython-312.pyc
--rw-r--r--   0        0        0     1748 2024-05-04 14:41:16.918373 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupBrowser.cpython-310.pyc
--rw-r--r--   0        0        0     3509 2024-05-15 11:35:02.885586 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupBrowser.cpython-312.pyc
--rw-r--r--   0        0        0     2767 2024-05-04 14:41:16.919019 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupPage.cpython-310.pyc
--rw-r--r--   0        0        0     5965 2024-05-15 17:42:22.652233 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupPage.cpython-312.pyc
--rw-r--r--   0        0        0     7400 2024-05-26 16:58:56.468580 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/DendriteBrowser.cpython-312.pyc
--rw-r--r--   0        0        0     7192 2024-05-17 11:39:57.460426 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/DendriteLocator.cpython-312.pyc
--rw-r--r--   0        0        0     9365 2024-05-26 17:08:20.406737 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/DendritePage.cpython-312.pyc
--rw-r--r--   0        0        0     3222 2024-05-26 16:58:56.469429 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/ScreenshotManager.cpython-312.pyc
--rw-r--r--   0        0        0     2919 2024-05-04 14:41:16.985071 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     3778 2024-05-26 17:08:20.551411 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/utils.cpython-312.pyc
--rw-r--r--   0        0        0      301 2024-05-16 06:48:31.744669 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/common/__pycache__/status.cpython-312.pyc
--rw-r--r--   0        0        0       67 2024-05-16 06:25:40.442424 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/common/status.py
--rw-r--r--   0        0        0     2732 2024-05-26 16:58:56.470225 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/utils.py
--rw-r--r--   0        0        0      280 2024-05-05 13:50:00.924479 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/GetInteractionDTO.py
--rw-r--r--   0        0        0      386 2024-05-16 16:51:31.204276 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/GoogleSearchDTO.py
--rw-r--r--   0        0        0      507 2024-05-15 11:04:30.884398 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/MakeInteractionDTO.py
--rw-r--r--   0        0        0      382 2024-05-16 06:52:15.213330 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/ScrapePageDTO.py
--rw-r--r--   0        0        0      661 2024-05-05 13:42:28.637321 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/GetInteractionDTO.cpython-310.pyc
--rw-r--r--   0        0        0      702 2024-05-05 13:50:13.259879 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/GetInteractionDTO.cpython-312.pyc
--rw-r--r--   0        0        0      853 2024-05-16 16:55:29.849995 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/GoogleSearchDTO.cpython-312.pyc
--rw-r--r--   0        0        0      465 2024-05-05 13:42:28.638500 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/LLMConfig.cpython-312.pyc
--rw-r--r--   0        0        0      441 2024-05-05 13:42:28.639036 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/LLMConfigDTO.cpython-310.pyc
--rw-r--r--   0        0        0      471 2024-05-05 13:42:28.639549 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/LLMConfigDTO.cpython-312.pyc
--rw-r--r--   0        0        0      992 2024-05-15 12:50:08.193062 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/MakeInteractionDTO.cpython-312.pyc
--rw-r--r--   0        0        0      909 2024-05-05 13:42:28.639943 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/PageInformation.cpython-312.pyc
--rw-r--r--   0        0        0      816 2024-05-05 13:42:28.640332 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/PageInformationDTO.cpython-310.pyc
--rw-r--r--   0        0        0      915 2024-05-05 13:42:28.640720 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/PageInformationDTO.cpython-312.pyc
--rw-r--r--   0        0        0      847 2024-05-16 06:52:50.171794 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/ScrapePageDTO.cpython-312.pyc
--rw-r--r--   0        0        0     2916 2024-02-04 16:42:27.331461 dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/__pycache__/agent.cpython-310.pyc
--rw-r--r--   0        0        0      784 2024-05-26 16:15:03.185863 dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/get_steam_reviews.py
--rw-r--r--   0        0        0     3028 2024-05-26 16:15:03.186113 dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/review_sentiment.py
--rw-r--r--   0        0        0     1426 2024-05-26 17:16:58.148127 dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/send_discord_message.py
--rw-r--r--   0        0        0      843 2024-05-26 16:58:56.470925 dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/simple_example.py
--rw-r--r--   0        0        0     1449 2024-05-24 13:38:38.546988 dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/yc.py
--rw-r--r--   0        0        0     1244 2024-05-17 11:21:44.603429 dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/DendriteException.py
--rw-r--r--   0        0        0      142 2024-05-14 09:02:04.165589 dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/IncorrectOutcomeException.py
--rw-r--r--   0        0        0        0 2024-05-14 09:02:01.998750 dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0     2526 2024-05-17 11:32:52.852813 dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/__pycache__/DendriteException.cpython-312.pyc
--rw-r--r--   0        0        0      504 2024-05-17 11:02:51.328702 dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/__pycache__/IncorrectOutcomeException.cpython-312.pyc
--rw-r--r--   0        0        0      199 2024-05-17 11:02:51.327921 dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0       85 2024-05-05 13:42:28.647626 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/LLMConfig.py
--rw-r--r--   0        0        0      208 2024-05-05 13:50:08.291916 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/PageDeltaInformation.py
--rw-r--r--   0        0        0      329 2024-05-05 13:49:28.012120 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/PageInformation.py
--rw-r--r--   0        0        0        0 2024-05-05 13:42:28.648634 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/__init__.py
--rw-r--r--   0        0        0      472 2024-05-05 13:49:39.105411 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/__pycache__/LLMConfig.cpython-312.pyc
--rw-r--r--   0        0        0      602 2024-05-15 11:35:03.288900 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/__pycache__/PageDeltaInformation.cpython-312.pyc
--rw-r--r--   0        0        0      934 2024-05-05 13:49:39.042358 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/__pycache__/PageInformation.cpython-312.pyc
--rw-r--r--   0        0        0      195 2024-05-05 13:49:39.041818 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      219 2024-02-04 09:02:32.807278 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models.py
--rw-r--r--   0        0        0     2405 2024-05-26 16:15:03.186638 dendrite_python_sdk-1.0.0/dendrite_python_sdk/request_handler.py
--rw-r--r--   0        0        0      210 2024-05-16 14:47:58.502176 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/GoogleSearchResponse.py
--rw-r--r--   0        0        0      205 2024-05-16 06:26:28.003675 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/InteractionResponse.py
--rw-r--r--   0        0        0      219 2024-05-16 07:41:52.278090 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/ScrapePageResponse.py
--rw-r--r--   0        0        0        0 2024-05-14 09:26:48.741213 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__init__.py
--rw-r--r--   0        0        0      782 2024-05-16 16:55:29.851232 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__pycache__/GoogleSearchResponse.cpython-312.pyc
--rw-r--r--   0        0        0      636 2024-05-16 06:48:31.795856 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__pycache__/InteractionResponse.cpython-312.pyc
--rw-r--r--   0        0        0      661 2024-05-16 07:43:56.074864 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__pycache__/ScrapePageResponse.cpython-312.pyc
--rw-r--r--   0        0        0      198 2024-05-15 12:50:08.234795 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      694 2024-05-26 18:07:19.190359 dendrite_python_sdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7414 1970-01-01 00:00:00.000000 dendrite_python_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-02-02 14:20:43.049218 dendrite_python_sdk-1.0.1/LICENSE
+-rw-r--r--   0        0        0     7059 2024-05-28 08:38:01.567597 dendrite_python_sdk-1.0.1/README.md
+-rw-r--r--   0        0        0       62 2024-05-15 17:53:47.139877 dendrite_python_sdk-1.0.1/dendrite_python_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 08:59:27.558957 dendrite_python_sdk-1.0.1/dendrite_python_sdk/ai_util/__init__.py
+-rw-r--r--   0        0        0      196 2024-05-20 09:08:52.601223 dendrite_python_sdk-1.0.1/dendrite_python_sdk/ai_util/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4434 2024-05-27 08:43:51.060967 dendrite_python_sdk-1.0.1/dendrite_python_sdk/ai_util/__pycache__/generate_text.cpython-312.pyc
+-rw-r--r--   0        0        0     2898 2024-05-26 16:15:03.183642 dendrite_python_sdk-1.0.1/dendrite_python_sdk/ai_util/generate_text.py
+-rw-r--r--   0        0        0     2361 2024-05-17 11:11:36.767261 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/ActivePageManager.py
+-rw-r--r--   0        0        0     4580 2024-05-26 16:15:03.184074 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/DendriteBrowser.py
+-rw-r--r--   0        0        0     4792 2024-05-28 08:18:19.728971 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/DendriteLocator.py
+-rw-r--r--   0        0        0     6380 2024-05-28 07:39:20.439252 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/DendritePage.py
+-rw-r--r--   0        0        0     1620 2024-05-26 16:15:03.184385 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/ScreenshotManager.py
+-rw-r--r--   0        0        0     4301 2024-05-17 11:13:52.699998 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/ActivePageManager.cpython-312.pyc
+-rw-r--r--   0        0        0     1748 2024-05-04 14:41:16.918373 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupBrowser.cpython-310.pyc
+-rw-r--r--   0        0        0     3509 2024-05-15 11:35:02.885586 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupBrowser.cpython-312.pyc
+-rw-r--r--   0        0        0     2767 2024-05-04 14:41:16.919019 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupPage.cpython-310.pyc
+-rw-r--r--   0        0        0     5965 2024-05-15 17:42:22.652233 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupPage.cpython-312.pyc
+-rw-r--r--   0        0        0     7400 2024-05-26 16:58:56.468580 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/DendriteBrowser.cpython-312.pyc
+-rw-r--r--   0        0        0     7105 2024-05-28 08:20:27.104574 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/DendriteLocator.cpython-312.pyc
+-rw-r--r--   0        0        0     9314 2024-05-28 08:17:31.736428 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/DendritePage.cpython-312.pyc
+-rw-r--r--   0        0        0     3222 2024-05-26 16:58:56.469429 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/ScreenshotManager.cpython-312.pyc
+-rw-r--r--   0        0        0     2919 2024-05-04 14:41:16.985071 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     3778 2024-05-26 17:08:20.551411 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/utils.cpython-312.pyc
+-rw-r--r--   0        0        0      301 2024-05-16 06:48:31.744669 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/common/__pycache__/status.cpython-312.pyc
+-rw-r--r--   0        0        0       67 2024-05-16 06:25:40.442424 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/common/status.py
+-rw-r--r--   0        0        0     2732 2024-05-26 16:58:56.470225 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/utils.py
+-rw-r--r--   0        0        0      280 2024-05-05 13:50:00.924479 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/GetInteractionDTO.py
+-rw-r--r--   0        0        0      386 2024-05-16 16:51:31.204276 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/GoogleSearchDTO.py
+-rw-r--r--   0        0        0      507 2024-05-15 11:04:30.884398 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/MakeInteractionDTO.py
+-rw-r--r--   0        0        0      382 2024-05-16 06:52:15.213330 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/ScrapePageDTO.py
+-rw-r--r--   0        0        0      661 2024-05-05 13:42:28.637321 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/GetInteractionDTO.cpython-310.pyc
+-rw-r--r--   0        0        0      702 2024-05-05 13:50:13.259879 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/GetInteractionDTO.cpython-312.pyc
+-rw-r--r--   0        0        0      853 2024-05-16 16:55:29.849995 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/GoogleSearchDTO.cpython-312.pyc
+-rw-r--r--   0        0        0      465 2024-05-05 13:42:28.638500 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/LLMConfig.cpython-312.pyc
+-rw-r--r--   0        0        0      441 2024-05-05 13:42:28.639036 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/LLMConfigDTO.cpython-310.pyc
+-rw-r--r--   0        0        0      471 2024-05-05 13:42:28.639549 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/LLMConfigDTO.cpython-312.pyc
+-rw-r--r--   0        0        0      992 2024-05-15 12:50:08.193062 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/MakeInteractionDTO.cpython-312.pyc
+-rw-r--r--   0        0        0      909 2024-05-05 13:42:28.639943 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/PageInformation.cpython-312.pyc
+-rw-r--r--   0        0        0      816 2024-05-05 13:42:28.640332 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/PageInformationDTO.cpython-310.pyc
+-rw-r--r--   0        0        0      915 2024-05-05 13:42:28.640720 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/PageInformationDTO.cpython-312.pyc
+-rw-r--r--   0        0        0      847 2024-05-16 06:52:50.171794 dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/ScrapePageDTO.cpython-312.pyc
+-rw-r--r--   0        0        0     2916 2024-02-04 16:42:27.331461 dendrite_python_sdk-1.0.1/dendrite_python_sdk/examples/__pycache__/agent.cpython-310.pyc
+-rw-r--r--   0        0        0      784 2024-05-26 16:15:03.185863 dendrite_python_sdk-1.0.1/dendrite_python_sdk/examples/get_steam_reviews.py
+-rw-r--r--   0        0        0     3028 2024-05-27 10:00:22.735320 dendrite_python_sdk-1.0.1/dendrite_python_sdk/examples/review_sentiment.py
+-rw-r--r--   0        0        0     1426 2024-05-26 17:16:58.148127 dendrite_python_sdk-1.0.1/dendrite_python_sdk/examples/send_discord_message.py
+-rw-r--r--   0        0        0     1129 2024-05-28 06:13:51.494297 dendrite_python_sdk-1.0.1/dendrite_python_sdk/examples/simple_example.py
+-rw-r--r--   0        0        0     1449 2024-05-24 13:38:38.546988 dendrite_python_sdk-1.0.1/dendrite_python_sdk/examples/yc.py
+-rw-r--r--   0        0        0     1246 2024-05-28 07:40:14.288359 dendrite_python_sdk-1.0.1/dendrite_python_sdk/exceptions/DendriteException.py
+-rw-r--r--   0        0        0      142 2024-05-14 09:02:04.165589 dendrite_python_sdk-1.0.1/dendrite_python_sdk/exceptions/IncorrectOutcomeException.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:02:01.998750 dendrite_python_sdk-1.0.1/dendrite_python_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     2473 2024-05-28 08:17:31.910171 dendrite_python_sdk-1.0.1/dendrite_python_sdk/exceptions/__pycache__/DendriteException.cpython-312.pyc
+-rw-r--r--   0        0        0      504 2024-05-17 11:02:51.328702 dendrite_python_sdk-1.0.1/dendrite_python_sdk/exceptions/__pycache__/IncorrectOutcomeException.cpython-312.pyc
+-rw-r--r--   0        0        0      199 2024-05-17 11:02:51.327921 dendrite_python_sdk-1.0.1/dendrite_python_sdk/exceptions/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0       85 2024-05-05 13:42:28.647626 dendrite_python_sdk-1.0.1/dendrite_python_sdk/models/LLMConfig.py
+-rw-r--r--   0        0        0      208 2024-05-05 13:50:08.291916 dendrite_python_sdk-1.0.1/dendrite_python_sdk/models/PageDeltaInformation.py
+-rw-r--r--   0        0        0      329 2024-05-05 13:49:28.012120 dendrite_python_sdk-1.0.1/dendrite_python_sdk/models/PageInformation.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:42:28.648634 dendrite_python_sdk-1.0.1/dendrite_python_sdk/models/__init__.py
+-rw-r--r--   0        0        0      472 2024-05-05 13:49:39.105411 dendrite_python_sdk-1.0.1/dendrite_python_sdk/models/__pycache__/LLMConfig.cpython-312.pyc
+-rw-r--r--   0        0        0      602 2024-05-15 11:35:03.288900 dendrite_python_sdk-1.0.1/dendrite_python_sdk/models/__pycache__/PageDeltaInformation.cpython-312.pyc
+-rw-r--r--   0        0        0      934 2024-05-05 13:49:39.042358 dendrite_python_sdk-1.0.1/dendrite_python_sdk/models/__pycache__/PageInformation.cpython-312.pyc
+-rw-r--r--   0        0        0      195 2024-05-05 13:49:39.041818 dendrite_python_sdk-1.0.1/dendrite_python_sdk/models/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      219 2024-02-04 09:02:32.807278 dendrite_python_sdk-1.0.1/dendrite_python_sdk/models.py
+-rw-r--r--   0        0        0     2810 2024-05-28 08:36:16.273120 dendrite_python_sdk-1.0.1/dendrite_python_sdk/request_handler.py
+-rw-r--r--   0        0        0      210 2024-05-16 14:47:58.502176 dendrite_python_sdk-1.0.1/dendrite_python_sdk/responses/GoogleSearchResponse.py
+-rw-r--r--   0        0        0      205 2024-05-16 06:26:28.003675 dendrite_python_sdk-1.0.1/dendrite_python_sdk/responses/InteractionResponse.py
+-rw-r--r--   0        0        0      219 2024-05-16 07:41:52.278090 dendrite_python_sdk-1.0.1/dendrite_python_sdk/responses/ScrapePageResponse.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:26:48.741213 dendrite_python_sdk-1.0.1/dendrite_python_sdk/responses/__init__.py
+-rw-r--r--   0        0        0      782 2024-05-16 16:55:29.851232 dendrite_python_sdk-1.0.1/dendrite_python_sdk/responses/__pycache__/GoogleSearchResponse.cpython-312.pyc
+-rw-r--r--   0        0        0      636 2024-05-16 06:48:31.795856 dendrite_python_sdk-1.0.1/dendrite_python_sdk/responses/__pycache__/InteractionResponse.cpython-312.pyc
+-rw-r--r--   0        0        0      661 2024-05-16 07:43:56.074864 dendrite_python_sdk-1.0.1/dendrite_python_sdk/responses/__pycache__/ScrapePageResponse.cpython-312.pyc
+-rw-r--r--   0        0        0      198 2024-05-15 12:50:08.234795 dendrite_python_sdk-1.0.1/dendrite_python_sdk/responses/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      694 2024-05-28 08:37:17.920758 dendrite_python_sdk-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7766 1970-01-01 00:00:00.000000 dendrite_python_sdk-1.0.1/PKG-INFO
```

### Comparing `dendrite_python_sdk-1.0.0/LICENSE` & `dendrite_python_sdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/README.md` & `dendrite_python_sdk-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,61 @@
 # Dendrite
 
-Dendrite is a developer tool that makes it very easy to interact with and scrape websites using AI.
+Dendrite is an SDK that makes it easy to interact with and scrape websites using prompts.
 
-This project is still in it's infancy and is susceptible to many changes in the coming weeks. 
+```python
+# Extracting data from a page is as simple as doing page.scrape(prompt)
+startup_urls = await page.scrape("Extract a list of valid urls for each listed startup's YC page")
+```
 
-If you want to chat with us developers, give feedback and report bugs, our discord is the place to be! [Invite link](https://discord.gg/ETPBdXU3kx)
+Join our discord to give feedback and report bugs! [Invite link](https://discord.gg/ETPBdXU3kx)
 
 
 ## Installation:
 
 ```
 pip install dendrite-python-sdk && playwright install
 ```
 
 ## Quick start:
 
-Here is a very simple example of how to use Dendrite. In the example we go to google.com, close the cookie popup, find the search bar and enter 'hello world' into it.
+Here is a very simple example of how to use Dendrite.
 
-To do this we install dendrite and asyncio like so: `pip install asyncio dendrite-python-sdk && playwright install` and we then create a file called `main.py` which we can run with `python main.py` from the terminal.
+Install dendrite and asyncio like so: `pip install asyncio dendrite-python-sdk && playwright install` and create a file called `main.py`. Use the code below and run it with `python main.py` from the terminal.
 
 `main.py`
 ```python
 from dendrite_python_sdk import DendriteBrowser
 import asyncio
 
 async def main():
-    dendrite_browser = DendriteBrowser(openai_api_key=...) # Use your own OpenAI API key here
+    # Launch browser locally
+    dendrite_browser = DendriteBrowser(openai_api_key=...) # Use your OpenAI key here
+
+    # Go to google.com
     page = await dendrite_browser.goto("https://google.com")
+
+    # Get the reject cookies button
     close_cookies = await page.get_interactable_element("reject cookies popup button")
+
+    # Click the button, returns IncorrectOutcomeException if the popup wasn't closed
     await close_cookies.click(expected_outcome="That the cookies popup closed.")
+
+    # Get the search bar
     search_bar = await page.get_interactable_element("Return the search bar")
-    await search_bar.fill("hello world")
+
+    # Enter "hello world" into it.
+    await search_bar.fill(
+        "hello world", expected_outcome="The words 'hello world' to have been entered"
+    )
+
+    # Use the Playwright page to press enter.
+    await page.get_playwright_page().keyboard.press("Enter")
+
+    await asyncio.sleep(2)
     await dendrite_browser.close()
 
 
 asyncio.run(main())
 ```
 
 ## More Advanced Example:
```

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/ai_util/__pycache__/generate_text.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/ai_util/__pycache__/generate_text.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Fri May 24 15:30:35 2024 UTC, .py size: 2898 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 9bb2 5066 520b 0000  ..........PfR...
+00000000: cb0d 0d0a 0000 0000 0760 5366 520b 0000  .........`SfR...
 00000010: e300 0000 0000 0000 0000 0000 0008 0000  ................
 00000020: 0000 0000 00f3 4601 0000 9700 6400 6401  ......F.....d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6402  l.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 0100 6400 6401  l.m.Z.m.Z...d.d.
 00000050: 6c05 5a05 6400 6401 6c06 5a06 6400 6403  l.Z.d.d.l.Z.d.d.
 00000060: 6c07 6d08 5a08 0100 6400 6404 6c09 6d0a  l.m.Z...d.d.l.m.
 00000070: 5a0a 6d0b 5a0b 0100 6400 6405 6c0c 6d0d  Z.m.Z...d.d.l.m.
```

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/ai_util/generate_text.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/ai_util/generate_text.py`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/ActivePageManager.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/ActivePageManager.py`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/DendriteBrowser.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/DendriteBrowser.py`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/DendriteLocator.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/DendriteLocator.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,14 @@
             os.path.join(os.getcwd(), "exceptions"), name="after"
         )
 
         page_delta_information = PageDeltaInformation(
             page_before=page_before_info, page_after=page_after_info
         )
 
-        print("page_after_info: ", page_after_info.url)
-
         dto = MakeInteractionDTO(
             url=page_before.url,
             dendrite_id=self.dendrite_id,
             interaction_type="click",
             expected_outcome=expected_outcome,
             page_delta_information=page_delta_information,
             llm_config=llm_config,
```

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/DendritePage.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/DendritePage.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
         if pydantic_return_model:
             return pydantic_return_model.parse_obj(res.json_data)
 
         return res.json_data
 
     async def scroll_to_bottom(self):
+        # TODO: add timeout
         i = 0
         last_scroll_position = 0
         start_time = time.time()
 
         while True:
             current_scroll_position = await self.page.evaluate("window.scrollY")
 
@@ -163,15 +164,14 @@
             page_information = await self.get_page_information()
 
             dto = GetInteractionDTO(
                 page_information=page_information, llm_config=llm_config, prompt=prompt
             )
 
             res = await get_interaction(dto)
-            print("res: ", res)
             if res and res["dendrite_id"] != "":
                 locator = await self.get_element_from_dendrite_id(res["dendrite_id"])
                 dendrite_locator = DendriteLocator(
                     res["dendrite_id"], locator, self.dendrite_browser
                 )
                 return dendrite_locator
             num_attempts += 1
```

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/ScreenshotManager.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/ScreenshotManager.py`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/ActivePageManager.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/ActivePageManager.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupBrowser.cpython-310.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupBrowser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupBrowser.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupBrowser.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupPage.cpython-310.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupPage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupPage.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupPage.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/DendriteBrowser.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/DendriteBrowser.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/DendriteLocator.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/DendriteLocator.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Fri May 17 11:39:53 2024 UTC, .py size: 4849 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 0942 4766 f112 0000  .........BGf....
+00000000: cb0d 0d0a 0000 0000 4b93 5566 b812 0000  ........K.Uf....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 ac00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6403 6c05 6d06 5a06 0100 6400 6404  d.d.l.m.Z...d.d.
 00000060: 6c07 6d08 5a08 0100 6400 6405 6c09 6d0a  l.m.Z...d.d.l.m.
 00000070: 5a0a 0100 6400 6406 6c0b 6d0c 5a0c 0100  Z...d.d.l.m.Z...
@@ -106,15 +106,15 @@
 00000690: 1224 d70c 24d0 0c24 f409 000f 138f 6989  .$..$..$......i.
 000006a0: 698b 6b98 4ad1 0e26 a827 d30e 31f0 0a00  i.k.J..&.'..1...
 000006b0: 1015 f009 0014 4101 f8f0 0600 0d25 fa73  ......A......%.s
 000006c0: 2a00 0000 8241 0c42 2001 c10e 0142 1c04  *....A.B ....B..
 000006d0: c10f 2c42 2001 c13b 0142 1e04 c13c 1e42  ..,B ..;.B...<.B
 000006e0: 2001 c21b 0242 2001 c21e 0142 2001 6302   ....B ....B .c.
 000006f0: 0000 0000 0000 0000 0000 0008 0000 008f  ................
-00000700: 0000 01f3 1006 0000 4b00 0100 9700 7c00  ........K.....|.
+00000700: 0000 01f3 e405 0000 4b00 0100 9700 7c00  ........K.....|.
 00000710: 6a00 0000 0000 0000 0000 0000 0000 0000  j...............
 00000720: 0000 0000 6a03 0000 0000 0000 0000 0000  ....j...........
 00000730: 0000 0000 0000 0000 ab00 0000 0000 0000  ................
 00000740: 7d04 7c00 6a00 0000 0000 0000 0000 0000  }.|.j...........
 00000750: 0000 0000 0000 0000 6a05 0000 0000 0000  ........j.......
 00000760: 0000 0000 0000 0000 0000 0000 ab00 0000  ................
 00000770: 0000 0000 8300 6400 7b03 0000 9602 9703  ......d.{.......
@@ -168,283 +168,278 @@
 00000a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a80: 7421 0000 0000 0000 0000 6a26 0000 0000  t!........j&....
 00000a90: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
 00000aa0: 0000 0000 0000 640c ab02 0000 0000 0000  ......d.........
 00000ab0: 640f ac0e ab02 0000 0000 0000 0100 7429  d.............t)
 00000ac0: 0000 0000 0000 0000 7c06 7c0b ac10 ab02  ........|.|.....
 00000ad0: 0000 0000 0000 7d0c 742b 0000 0000 0000  ......}.t+......
-00000ae0: 0000 6411 7c0b 6a14 0000 0000 0000 0000  ..d.|.j.........
-00000af0: 0000 0000 0000 0000 0000 ab02 0000 0000  ................
-00000b00: 0000 0100 742d 0000 0000 0000 0000 7c05  ....t-........|.
-00000b10: 6a14 0000 0000 0000 0000 0000 0000 0000  j...............
-00000b20: 0000 0000 7c00 6a2e 0000 0000 0000 0000  ....|.j.........
-00000b30: 0000 0000 0000 0000 0000 6407 7c01 7c0c  ..........d.|.|.
-00000b40: 7c04 ac12 ab06 0000 0000 0000 7d0d 7431  |...........}.t1
-00000b50: 0000 0000 0000 0000 7c0d ab01 0000 0000  ........|.......
-00000b60: 0000 8300 6400 7b03 0000 9602 9703 8605  ....d.{.........
-00000b70: 0500 7d0e 7c0e 6a32 0000 0000 0000 0000  ..}.|.j2........
-00000b80: 0000 0000 0000 0000 0000 6413 6b28 0000  ..........d.k(..
-00000b90: 722b 7435 0000 0000 0000 0000 7c0e 6a36  r+t5........|.j6
+00000ae0: 0000 7c05 6a14 0000 0000 0000 0000 0000  ..|.j...........
+00000af0: 0000 0000 0000 0000 7c00 6a2c 0000 0000  ........|.j,....
+00000b00: 0000 0000 0000 0000 0000 0000 0000 6407  ..............d.
+00000b10: 7c01 7c0c 7c04 ac11 ab06 0000 0000 0000  |.|.|...........
+00000b20: 7d0d 742f 0000 0000 0000 0000 7c0d ab01  }.t/........|...
+00000b30: 0000 0000 0000 8300 6400 7b03 0000 9602  ........d.{.....
+00000b40: 9703 8605 0500 7d0e 7c0e 6a30 0000 0000  ......}.|.j0....
+00000b50: 0000 0000 0000 0000 0000 0000 0000 6412  ..............d.
+00000b60: 6b28 0000 722b 7433 0000 0000 0000 0000  k(..r+t3........
+00000b70: 7c0e 6a34 0000 0000 0000 0000 0000 0000  |.j4............
+00000b80: 0000 0000 0000 7c0c 6a36 0000 0000 0000  ......|.j6......
+00000b90: 0000 0000 0000 0000 0000 0000 6a1c 0000  ............j...
 00000ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bb0: 0000 7c0c 6a38 0000 0000 0000 0000 0000  ..|.j8..........
-00000bc0: 0000 0000 0000 0000 6a1c 0000 0000 0000  ........j.......
-00000bd0: 0000 0000 0000 0000 0000 0000 ac0b ab02  ................
-00000be0: 0000 0000 0000 8201 7c0e 5300 3700 9002  ........|.S.7...
-00000bf0: 8c38 3700 9002 8c23 3700 9001 8cda 2300  .87....#7.....#.
-00000c00: 740e 0000 0000 0000 0000 2400 7271 7d09  t.........$.rq}.
-00000c10: 0900 0200 7c00 6a0a 0000 0000 0000 0000  ....|.j.........
-00000c20: 0000 0000 0000 0000 0000 6a0c 0000 0000  ..........j.....
-00000c30: 0000 0000 0000 0000 0000 0000 0000 7c02  ..............|.
-00000c40: 6402 6406 6405 9c02 7c03 a401 8e01 8300  d.d.d...|.......
-00000c50: 6400 7b04 0000 9605 9703 8605 3700 0500  d.{.........7...
-00000c60: 0100 6e3c 2300 740e 0000 0000 0000 0000  ..n<#.t.........
-00000c70: 2400 7230 7d09 7c00 6a0a 0000 0000 0000  $.r0}.|.j.......
-00000c80: 0000 0000 0000 0000 0000 0000 6a11 0000  ............j...
-00000c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ca0: 6407 6402 ac08 ab02 0000 0000 0000 8300  d.d.............
-00000cb0: 6400 7b04 0000 9606 9703 8605 3700 0500  d.{.........7...
-00000cc0: 0100 5900 6400 7d09 7e09 6e08 6400 7d09  ..Y.d.}.~.n.d.}.
-00000cd0: 7e09 7701 7700 7803 5900 7701 5900 6400  ~.w.w.x.Y.w.Y.d.
-00000ce0: 7d09 7e09 9002 8c4d 6400 7d09 7e09 7701  }.~....Md.}.~.w.
-00000cf0: 7700 7803 5900 7701 3700 9002 8c37 3700  w.x.Y.w.7....77.
-00000d00: 9002 8c18 3700 9001 8cf4 3700 9001 8cdf  ....7.....7.....
-00000d10: 3700 8cd2 ad03 7701 2914 4e72 2100 0000  7.....w.).Nr!...
-00000d20: e9d0 0700 00da 0566 6f72 6365 4629 0272  .......forceF).r
-00000d30: 2100 0000 7227 0000 0054 da05 636c 6963  !...r'...T..clic
-00000d40: 6b29 0172 2100 0000 da04 6c6f 6164 da00  k).r!.....load..
-00000d50: 2902 da07 6d65 7373 6167 65da 1173 6372  )...message..scr
-00000d60: 6565 6e73 686f 745f 6261 7365 3634 da0a  eenshot_base64..
-00000d70: 6578 6365 7074 696f 6e73 da06 6265 666f  exceptions..befo
-00000d80: 7265 2901 da04 6e61 6d65 da05 6166 7465  re)...name..afte
-00000d90: 72a9 02da 0b70 6167 655f 6265 666f 7265  r....page_before
-00000da0: da0a 7061 6765 5f61 6674 6572 7a11 7061  ..page_afterz.pa
-00000db0: 6765 5f61 6674 6572 5f69 6e66 6f3a 20a9  ge_after_info: .
-00000dc0: 0672 1d00 0000 7211 0000 00da 1069 6e74  .r....r......int
-00000dd0: 6572 6163 7469 6f6e 5f74 7970 65da 1065  eraction_type..e
-00000de0: 7870 6563 7465 645f 6f75 7463 6f6d 65da  xpected_outcome.
-00000df0: 1670 6167 655f 6465 6c74 615f 696e 666f  .page_delta_info
-00000e00: 726d 6174 696f 6eda 0a6c 6c6d 5f63 6f6e  rmation..llm_con
-00000e10: 6669 67da 0666 6169 6c65 6429 1d72 1300  fig..failed).r..
-00000e20: 0000 da0e 6765 745f 6c6c 6d5f 636f 6e66  ....get_llm_conf
-00000e30: 6967 721c 0000 00da 1467 6574 5f70 6167  igr......get_pag
-00000e40: 655f 696e 666f 726d 6174 696f 6eda 0370  e_information..p
-00000e50: 6f70 7212 0000 0072 2800 0000 da09 4578  opr....r(.....Ex
-00000e60: 6365 7074 696f 6eda 0e64 6973 7061 7463  ception..dispatc
-00000e70: 685f 6576 656e 7472 2400 0000 721d 0000  h_eventr$...r...
-00000e80: 00da 1367 6574 5f70 6c61 7977 7269 6768  ...get_playwrigh
-00000e90: 745f 7061 6765 da13 7761 6974 5f66 6f72  t_page..wait_for
-00000ea0: 5f6c 6f61 645f 7374 6174 6572 0600 0000  _load_stater....
-00000eb0: 722c 0000 00da 1a73 746f 7265 5f65 7863  r,.....store_exc
-00000ec0: 6570 7469 6f6e 5f73 6372 6565 6e73 686f  eption_screensho
-00000ed0: 74da 026f 73da 0470 6174 68da 046a 6f69  t..os..path..joi
-00000ee0: 6eda 0667 6574 6377 6472 0a00 0000 da05  n..getcwdr......
-00000ef0: 7072 696e 7472 0900 0000 7211 0000 0072  printr....r....r
-00000f00: 0b00 0000 da06 7374 6174 7573 7207 0000  ......statusr...
-00000f10: 0072 2b00 0000 7233 0000 0029 0f72 1400  .r+...r3...).r..
-00000f20: 0000 7236 0000 00da 0461 7267 73da 066b  ..r6.....args..k
-00000f30: 7761 7267 7372 3800 0000 7232 0000 00da  wargsr8...r2....
-00000f40: 1070 6167 655f 6265 666f 7265 5f69 6e66  .page_before_inf
-00000f50: 6f72 2100 0000 7227 0000 00da 0165 7233  or!...r'.....er3
-00000f60: 0000 00da 0f70 6167 655f 6166 7465 725f  .....page_after_
-00000f70: 696e 666f 7237 0000 00da 0364 746f da03  infor7.....dto..
-00000f80: 7265 7373 0f00 0000 2020 2020 2020 2020  ress....        
-00000f90: 2020 2020 2020 2072 1500 0000 7228 0000         r....r(..
-00000fa0: 007a 1544 656e 6472 6974 654c 6f63 6174  .z.DendriteLocat
-00000fb0: 6f72 2e63 6c69 636b 2c00 0000 7399 0200  or.click,...s...
-00000fc0: 00e8 00f8 8000 d815 19d7 152a d115 2ad7  ...........*..*.
-00000fd0: 1539 d115 39d3 153b 880a e01c 20d7 1c31  .9..9..;.... ..1
-00000fe0: d11c 31d7 1c41 d11c 41d3 1c43 d716 4388  ..1..A..A..C..C.
-00000ff0: 0bd8 212c d721 41d1 2141 d321 43d7 1b43  ..!,.!A.!A.!C..C
-00001000: d008 18e0 1218 972a 912a 9859 a804 d312  .......*.*.Y....
-00001010: 2d88 07d8 1016 970a 910a 9837 a045 d310  -..........7.E..
-00001020: 2a88 05f0 0406 0949 01d8 1224 9024 972c  *......I...$.$.,
-00001030: 912c d712 24d1 1224 c044 a857 b845 d112  .,..$..$.D.W.E..
-00001040: 53c8 46d1 1253 d70c 53d0 0c53 f00e 000f  S.F..S..S..S....
-00001050: 13d7 0e28 d10e 28a8 1baf 1fa9 1fd3 0e39  ...(..(........9
-00001060: d708 39d0 0839 e01b 1fd7 1b30 d11b 30d7  ..9..9.....0..0.
-00001070: 1b40 d11b 40d3 1b42 d715 4288 0ad8 0e18  .@..@..B..B.....
-00001080: d70e 2cd1 0e2c d30e 2ed7 0e42 d10e 42c0  ..,..,.....B..B.
-00001090: 36d3 0e4a d708 4ad0 084a d820 2ad7 203f  6..J..J..J. *. ?
-000010a0: d120 3fd3 2041 d71a 4188 0fe4 0c1d d814  . ?. A..A.......
-000010b0: 16d0 2a3a d72a 4cd1 2a4c f403 020d 0a88  ..*:.*L.*L......
+00000bb0: ac0b ab02 0000 0000 0000 8201 7c0e 5300  ............|.S.
+00000bc0: 3700 9002 8c22 3700 9002 8c0d 3700 9001  7...."7.....7...
+00000bd0: 8cc4 2300 740e 0000 0000 0000 0000 2400  ..#.t.........$.
+00000be0: 7271 7d09 0900 0200 7c00 6a0a 0000 0000  rq}.....|.j.....
+00000bf0: 0000 0000 0000 0000 0000 0000 0000 6a0c  ..............j.
+00000c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000c10: 0000 7c02 6402 6406 6405 9c02 7c03 a401  ..|.d.d.d...|...
+00000c20: 8e01 8300 6400 7b04 0000 9605 9703 8605  ....d.{.........
+00000c30: 3700 0500 0100 6e3c 2300 740e 0000 0000  7.....n<#.t.....
+00000c40: 0000 0000 2400 7230 7d09 7c00 6a0a 0000  ....$.r0}.|.j...
+00000c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000c60: 6a11 0000 0000 0000 0000 0000 0000 0000  j...............
+00000c70: 0000 0000 6407 6402 ac08 ab02 0000 0000  ....d.d.........
+00000c80: 0000 8300 6400 7b04 0000 9606 9703 8605  ....d.{.........
+00000c90: 3700 0500 0100 5900 6400 7d09 7e09 6e08  7.....Y.d.}.~.n.
+00000ca0: 6400 7d09 7e09 7701 7700 7803 5900 7701  d.}.~.w.w.x.Y.w.
+00000cb0: 5900 6400 7d09 7e09 9002 8c37 6400 7d09  Y.d.}.~....7d.}.
+00000cc0: 7e09 7701 7700 7803 5900 7701 3700 9002  ~.w.w.x.Y.w.7...
+00000cd0: 8c21 3700 9002 8c02 3700 9001 8cde 3700  .!7.....7.....7.
+00000ce0: 9001 8cc9 3700 8cd2 ad03 7701 2913 4e72  ....7.....w.).Nr
+00000cf0: 2100 0000 e9d0 0700 00da 0566 6f72 6365  !..........force
+00000d00: 4629 0272 2100 0000 7227 0000 0054 da05  F).r!...r'...T..
+00000d10: 636c 6963 6b29 0172 2100 0000 da04 6c6f  click).r!.....lo
+00000d20: 6164 da00 2902 da07 6d65 7373 6167 65da  ad..)...message.
+00000d30: 1173 6372 6565 6e73 686f 745f 6261 7365  .screenshot_base
+00000d40: 3634 da0a 6578 6365 7074 696f 6e73 da06  64..exceptions..
+00000d50: 6265 666f 7265 2901 da04 6e61 6d65 da05  before)...name..
+00000d60: 6166 7465 72a9 02da 0b70 6167 655f 6265  after....page_be
+00000d70: 666f 7265 da0a 7061 6765 5f61 6674 6572  fore..page_after
+00000d80: a906 721d 0000 0072 1100 0000 da10 696e  ..r....r......in
+00000d90: 7465 7261 6374 696f 6e5f 7479 7065 da10  teraction_type..
+00000da0: 6578 7065 6374 6564 5f6f 7574 636f 6d65  expected_outcome
+00000db0: da16 7061 6765 5f64 656c 7461 5f69 6e66  ..page_delta_inf
+00000dc0: 6f72 6d61 7469 6f6e da0a 6c6c 6d5f 636f  ormation..llm_co
+00000dd0: 6e66 6967 da06 6661 696c 6564 291c 7213  nfig..failed).r.
+00000de0: 0000 00da 0e67 6574 5f6c 6c6d 5f63 6f6e  .....get_llm_con
+00000df0: 6669 6772 1c00 0000 da14 6765 745f 7061  figr......get_pa
+00000e00: 6765 5f69 6e66 6f72 6d61 7469 6f6e da03  ge_information..
+00000e10: 706f 7072 1200 0000 7228 0000 00da 0945  popr....r(.....E
+00000e20: 7863 6570 7469 6f6e da0e 6469 7370 6174  xception..dispat
+00000e30: 6368 5f65 7665 6e74 7224 0000 0072 1d00  ch_eventr$...r..
+00000e40: 0000 da13 6765 745f 706c 6179 7772 6967  ....get_playwrig
+00000e50: 6874 5f70 6167 65da 1377 6169 745f 666f  ht_page..wait_fo
+00000e60: 725f 6c6f 6164 5f73 7461 7465 7206 0000  r_load_stater...
+00000e70: 0072 2c00 0000 da1a 7374 6f72 655f 6578  .r,.....store_ex
+00000e80: 6365 7074 696f 6e5f 7363 7265 656e 7368  ception_screensh
+00000e90: 6f74 da02 6f73 da04 7061 7468 da04 6a6f  ot..os..path..jo
+00000ea0: 696e da06 6765 7463 7764 720a 0000 0072  in..getcwdr....r
+00000eb0: 0900 0000 7211 0000 0072 0b00 0000 da06  ....r....r......
+00000ec0: 7374 6174 7573 7207 0000 0072 2b00 0000  statusr....r+...
+00000ed0: 7233 0000 0029 0f72 1400 0000 7236 0000  r3...).r....r6..
+00000ee0: 00da 0461 7267 73da 066b 7761 7267 7372  ...args..kwargsr
+00000ef0: 3800 0000 7232 0000 00da 1070 6167 655f  8...r2.....page_
+00000f00: 6265 666f 7265 5f69 6e66 6f72 2100 0000  before_infor!...
+00000f10: 7227 0000 00da 0165 7233 0000 00da 0f70  r'.....er3.....p
+00000f20: 6167 655f 6166 7465 725f 696e 666f 7237  age_after_infor7
+00000f30: 0000 00da 0364 746f da03 7265 7373 0f00  .....dto..ress..
+00000f40: 0000 2020 2020 2020 2020 2020 2020 2020  ..              
+00000f50: 2072 1500 0000 7228 0000 007a 1544 656e   r....r(...z.Den
+00000f60: 6472 6974 654c 6f63 6174 6f72 2e63 6c69  driteLocator.cli
+00000f70: 636b 2c00 0000 7388 0200 00e8 00f8 8000  ck,...s.........
+00000f80: d815 19d7 152a d115 2ad7 1539 d115 39d3  .....*..*..9..9.
+00000f90: 153b 880a e01c 20d7 1c31 d11c 31d7 1c41  .;.... ..1..1..A
+00000fa0: d11c 41d3 1c43 d716 4388 0bd8 212c d721  ..A..C..C...!,.!
+00000fb0: 41d1 2141 d321 43d7 1b43 d008 18e0 1218  A.!A.!C..C......
+00000fc0: 972a 912a 9859 a804 d312 2d88 07d8 1016  .*.*.Y....-.....
+00000fd0: 970a 910a 9837 a045 d310 2a88 05f0 0406  .....7.E..*.....
+00000fe0: 0949 01d8 1224 9024 972c 912c d712 24d1  .I...$.$.,.,..$.
+00000ff0: 1224 c044 a857 b845 d112 53c8 46d1 1253  .$.D.W.E..S.F..S
+00001000: d70c 53d0 0c53 f00e 000f 13d7 0e28 d10e  ..S..S.......(..
+00001010: 28a8 1baf 1fa9 1fd3 0e39 d708 39d0 0839  (........9..9..9
+00001020: e01b 1fd7 1b30 d11b 30d7 1b40 d11b 40d3  .....0..0..@..@.
+00001030: 1b42 d715 4288 0ad8 0e18 d70e 2cd1 0e2c  .B..B.......,..,
+00001040: d30e 2ed7 0e42 d10e 42c0 36d3 0e4a d708  .....B..B.6..J..
+00001050: 4ad0 084a d820 2ad7 203f d120 3fd3 2041  J..J. *. ?. ?. A
+00001060: d71a 4188 0fe4 0c1d d814 16d0 2a3a d72a  ..A.........*:.*
+00001070: 4cd1 2a4c f403 020d 0a88 01f0 0600 090a  L.*L............
+00001080: d708 24d1 0824 dc0c 0e8f 4789 478f 4c89  ..$..$....G.G.L.
+00001090: 4c9c 129f 1999 199b 1ba0 6cd3 0c33 b828  L.........l..3.(
+000010a0: f003 0009 25f4 0002 090a f408 000d 1ed8  ....%...........
+000010b0: 1416 a82f d72a 4bd1 2a4b f403 020d 0a88  .../.*K.*K......
 000010c0: 01f0 0600 090a d708 24d1 0824 dc0c 0e8f  ........$..$....
 000010d0: 4789 478f 4c89 4c9c 129f 1999 199b 1ba0  G.G.L.L.........
-000010e0: 6cd3 0c33 b828 f003 0009 25f4 0002 090a  l..3.(....%.....
-000010f0: f408 000d 1ed8 1416 a82f d72a 4bd1 2a4b  ........./.*K.*K
-00001100: f403 020d 0a88 01f0 0600 090a d708 24d1  ..............$.
-00001110: 0824 dc0c 0e8f 4789 478f 4c89 4c9c 129f  .$....G.G.L.L...
-00001120: 1999 199b 1ba0 6cd3 0c33 b827 f003 0009  ......l..3.'....
-00001130: 25f4 0002 090a f408 0022 36d8 1828 b05f  %........"6..(._
-00001140: f403 0222 0ad0 081e f408 0009 0ed0 0e21  ..."...........!
-00001150: a03f d723 36d1 2336 d408 37e4 0e20 d810  .?.#6.#6..7.. ..
-00001160: 1b97 0f91 0fd8 181c d718 28d1 1828 d81d  ..........(..(..
-00001170: 24d8 1d2d d823 39d8 1721 f40d 070f 0a88  $..-.#9..!......
-00001180: 03f4 1000 1525 a053 d314 29d7 0e29 8803  .....%.S..)..)..
-00001190: e00b 0e8f 3a89 3a98 18d2 0b21 dc12 2bd8  ....:.:....!..+.
-000011a0: 181b 9f0b 990b d822 38d7 2243 d122 43d7  ......."8."C."C.
-000011b0: 2255 d122 55f4 0503 130e f000 030d 0ef0  "U."U...........
-000011c0: 0a00 1013 880a f071 0100 1744 01f9 d81b  .......q...D....
-000011d0: 43f9 f00c 000d 5401 fadc 0f18 f200 0409  C.....T.........
-000011e0: 4901 f002 030d 4901 d816 2890 6497 6c91  I.....I...(.d.l.
-000011f0: 6cd7 1628 d116 28c0 44b0 14b8 54d1 1653  l..(..(.D...T..S
-00001200: c846 d116 53d7 1053 d210 53f8 dc13 1cf2  .F..S..S..S.....
-00001210: 0001 0d49 01d8 161a 976c 916c d716 31d1  ...I.....l.l..1.
-00001220: 1631 b027 c034 d016 31d3 1648 d710 48d6  .1.'.4..1..H..H.
-00001230: 1048 fbf0 0301 0d49 01ff fcf0 0704 0949  .H.....I.......I
-00001240: 01fa f00c 0009 3af9 e015 42f9 d808 4af9  ......:...B...J.
-00001250: d81a 41f9 f03c 000f 2afa 73ef 0000 0082  ..A..<..*.s.....
-00001260: 384c 0601 ba01 4932 04bb 174c 0601 c112  8L....I2...L....
-00001270: 0149 3504 c113 284c 0601 c13c 2249 3b00  .I5...(L...<"I;.
-00001280: c21e 0149 3804 c21f 0449 3b00 c223 1e4c  ...I8....I;..#.L
-00001290: 0601 c301 014b 3804 c302 214c 0601 c323  .....K8...!L...#
-000012a0: 014b 3b04 c324 264c 0601 c40a 014b 3e04  .K;..$&L.....K>.
-000012b0: c40b 174c 0601 c422 014c 0104 c423 440e  ...L...".L...#D.
-000012c0: 4c06 01c8 3101 4c04 04c8 3241 014c 0601  L...1.L...2A.L..
-000012d0: c935 014c 0601 c938 0149 3b00 c93b 094b  .5.L...8.I;..;.K
-000012e0: 3503 ca05 224a 2e02 ca27 014a 2a06 ca28  5..."J...'.J*..(
-000012f0: 054a 2e02 ca2d 014b 3003 ca2e 094b 2705  .J...-.K0....K'.
-00001300: ca37 204b 2205 cb17 014b 1a08 cb18 054b  .7 K"....K.....K
-00001310: 2205 cb1d 054b 3003 cb22 054b 2705 cb27  "....K0..".K'..'
-00001320: 034b 3003 cb2a 064c 0601 cb30 054b 3503  .K0..*.L...0.K5.
-00001330: cb35 044c 0601 cb3b 014c 0601 cb3e 014c  .5.L...;.L...>.L
-00001340: 0601 cc01 014c 0601 cc04 014c 0601 6303  .....L.....L..c.
-00001350: 0000 0000 0000 0000 0000 0008 0000 008f  ................
-00001360: 0000 01f3 a402 0000 4b00 0100 9700 7c02  ........K.....|.
-00001370: 6401 6b28 0000 7206 6402 7c01 9b00 6403  d.k(..r.d.|...d.
-00001380: 9d03 7d02 7c00 6a00 0000 0000 0000 0000  ..}.|.j.........
-00001390: 0000 0000 0000 0000 0000 6a03 0000 0000  ..........j.....
-000013a0: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
-000013b0: 0000 0000 0000 7d05 7c00 6a00 0000 0000  ......}.|.j.....
-000013c0: 0000 0000 0000 0000 0000 0000 0000 6a05  ..............j.
-000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000013e0: 0000 ab00 0000 0000 0000 8300 6400 7b03  ............d.{.
-000013f0: 0000 9602 9703 8605 0500 7d06 7c06 6a07  ..........}.|.j.
+000010e0: 6cd3 0c33 b827 f003 0009 25f4 0002 090a  l..3.'....%.....
+000010f0: f408 0022 36d8 1828 b05f f403 0222 0ad0  ..."6..(._..."..
+00001100: 081e f408 000f 21d8 101b 970f 910f d818  ......!.........
+00001110: 1cd7 1828 d118 28d8 1d24 d81d 2dd8 2339  ...(..(..$..-.#9
+00001120: d817 21f4 0d07 0f0a 8803 f410 0015 25a0  ..!...........%.
+00001130: 53d3 1429 d70e 2988 03e0 0b0e 8f3a 893a  S..)..)......:.:
+00001140: 9818 d20b 21dc 122b d818 1b9f 0b99 0bd8  ....!..+........
+00001150: 2238 d722 43d1 2243 d722 55d1 2255 f405  "8."C."C."U."U..
+00001160: 0313 0ef0 0003 0d0e f00a 0010 1388 0af0  ................
+00001170: 6d01 0017 4401 f9d8 1b43 f9f0 0c00 0d54  m...D....C.....T
+00001180: 01fa dc0f 18f2 0004 0949 01f0 0203 0d49  .........I.....I
+00001190: 01d8 1628 9064 976c 916c d716 28d1 1628  ...(.d.l.l..(..(
+000011a0: c044 b014 b854 d116 53c8 46d1 1653 d710  .D...T..S.F..S..
+000011b0: 53d2 1053 f8dc 131c f200 010d 4901 d816  S..S........I...
+000011c0: 1a97 6c91 6cd7 1631 d116 31b0 27c0 34d0  ..l.l..1..1.'.4.
+000011d0: 1631 d316 48d7 1048 d610 48fb f003 010d  .1..H..H..H.....
+000011e0: 4901 fffc f007 0409 4901 faf0 0c00 093a  I.......I......:
+000011f0: f9e0 1542 f9d8 084a f9d8 1a41 f9f0 3800  ...B...J...A..8.
+00001200: 0f2a fa73 ef00 0000 8238 4b30 01ba 0149  .*.s.....8K0...I
+00001210: 1c04 bb17 4b30 01c1 1201 491f 04c1 1328  ....K0....I....(
+00001220: 4b30 01c1 3c22 4925 00c2 1e01 4922 04c2  K0..<"I%....I"..
+00001230: 1f04 4925 00c2 231e 4b30 01c3 0101 4b22  ..I%..#.K0....K"
+00001240: 04c3 0221 4b30 01c3 2301 4b25 04c3 2426  ...!K0..#.K%..$&
+00001250: 4b30 01c4 0a01 4b28 04c4 0b17 4b30 01c4  K0....K(....K0..
+00001260: 2201 4b2b 04c4 2343 384b 3001 c81b 014b  ".K+..#C8K0....K
+00001270: 2e04 c81c 4101 4b30 01c9 1f01 4b30 01c9  ....A.K0....K0..
+00001280: 2201 4925 00c9 2509 4b1f 03c9 2f22 4a18  ".I%..%.K.../"J.
+00001290: 02ca 1101 4a14 06ca 1205 4a18 02ca 1701  ....J.....J.....
+000012a0: 4b1a 03ca 1809 4b11 05ca 2120 4b0c 05cb  K.....K...! K...
+000012b0: 0101 4b04 08cb 0205 4b0c 05cb 0705 4b1a  ..K.....K.....K.
+000012c0: 03cb 0c05 4b11 05cb 1103 4b1a 03cb 1406  ....K.....K.....
+000012d0: 4b30 01cb 1a05 4b1f 03cb 1f04 4b30 01cb  K0....K.....K0..
+000012e0: 2501 4b30 01cb 2801 4b30 01cb 2b01 4b30  %.K0..(.K0..+.K0
+000012f0: 01cb 2e01 4b30 0163 0300 0000 0000 0000  ....K0.c........
+00001300: 0000 0000 0800 0000 8f00 0001 f3a4 0200  ................
+00001310: 004b 0001 0097 007c 0264 016b 2800 0072  .K.....|.d.k(..r
+00001320: 0664 027c 019b 0064 039d 037d 027c 006a  .d.|...d...}.|.j
+00001330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001340: 0000 006a 0300 0000 0000 0000 0000 0000  ...j............
+00001350: 0000 0000 0000 00ab 0000 0000 0000 007d  ...............}
+00001360: 057c 006a 0000 0000 0000 0000 0000 0000  .|.j............
+00001370: 0000 0000 0000 006a 0500 0000 0000 0000  .......j........
+00001380: 0000 0000 0000 0000 0000 00ab 0000 0000  ................
+00001390: 0000 0083 0064 007b 0300 0096 0297 0386  .....d.{........
+000013a0: 0505 007d 067c 066a 0700 0000 0000 0000  ...}.|.j........
+000013b0: 0000 0000 0000 0000 0000 00ab 0000 0000  ................
+000013c0: 0000 0083 0064 007b 0300 0096 0297 0386  .....d.{........
+000013d0: 0505 007d 077c 046a 0900 0000 0000 0000  ...}.|.j........
+000013e0: 0000 0000 0000 0000 0000 0064 0464 05ab  ...........d.d..
+000013f0: 0200 0000 0000 007d 0802 007c 006a 0a00  .......}...|.j..
 00001400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001410: 0000 ab00 0000 0000 0000 8300 6400 7b03  ............d.{.
-00001420: 0000 9602 9703 8605 0500 7d07 7c04 6a09  ..........}.|.j.
-00001430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001440: 0000 6404 6405 ab02 0000 0000 0000 7d08  ..d.d.........}.
-00001450: 0200 7c00 6a0a 0000 0000 0000 0000 0000  ..|.j...........
-00001460: 0000 0000 0000 0000 6a0c 0000 0000 0000  ........j.......
-00001470: 0000 0000 0000 0000 0000 0000 7c01 6701  ............|.g.
-00001480: 7c03 a201 ad06 6404 7c08 6901 7c04 a401  |.....d.|.i.|...
-00001490: 8e01 8300 6400 7b03 0000 9602 9703 8605  ....d.{.........
-000014a0: 0500 0100 7c00 6a0f 0000 0000 0000 0000  ....|.j.........
-000014b0: 0000 0000 0000 0000 0000 7c06 6a10 0000  ..........|.j...
-000014c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000014d0: ab01 0000 0000 0000 8300 6400 7b03 0000  ..........d.{...
-000014e0: 9602 9703 8605 0500 0100 7c00 6a00 0000  ..........|.j...
-000014f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001500: 6a05 0000 0000 0000 0000 0000 0000 0000  j...............
-00001510: 0000 0000 ab00 0000 0000 0000 8300 6400  ..............d.
-00001520: 7b03 0000 9602 9703 8605 0500 7d09 7c09  {...........}.|.
-00001530: 6a07 0000 0000 0000 0000 0000 0000 0000  j...............
-00001540: 0000 0000 ab00 0000 0000 0000 8300 6400  ..............d.
-00001550: 7b03 0000 9602 9703 8605 0500 7d0a 7413  {...........}.t.
-00001560: 0000 0000 0000 0000 7c07 7c0a ac06 ab02  ........|.|.....
-00001570: 0000 0000 0000 7d0b 7415 0000 0000 0000  ......}.t.......
-00001580: 0000 7c06 6a10 0000 0000 0000 0000 0000  ..|.j...........
-00001590: 0000 0000 0000 0000 7c00 6a16 0000 0000  ........|.j.....
-000015a0: 0000 0000 0000 0000 0000 0000 0000 6407  ..............d.
-000015b0: 7c02 7c0b 7c05 ac08 ab06 0000 0000 0000  |.|.|...........
-000015c0: 7d0c 7419 0000 0000 0000 0000 7c0c ab01  }.t.........|...
-000015d0: 0000 0000 0000 8300 6400 7b03 0000 9602  ........d.{.....
-000015e0: 9703 8605 0500 7d0d 7c0d 5300 3700 8cfc  ......}.|.S.7...
-000015f0: 3700 8ce6 3700 8cac 3700 8c8b 3700 8c6b  7...7...7...7..k
-00001600: 3700 8c55 3700 8c12 ad03 7701 2909 4e72  7..U7.....w.).Nr
-00001610: 2a00 0000 7a0f 5468 6174 2074 6865 2074  *...z.That the t
-00001620: 6578 7420 277a 2627 2069 7320 6669 6c6c  ext 'z&' is fill
-00001630: 6564 2069 6e74 6f20 7468 6520 7461 7267  ed into the targ
-00001640: 6574 6564 2065 6c65 6d65 6e74 2e72 2100  eted element.r!.
-00001650: 0000 7226 0000 0072 3100 0000 da04 6669  ..r&...r1.....fi
-00001660: 6c6c 7234 0000 0029 0d72 1300 0000 723a  llr4...).r....r:
-00001670: 0000 0072 1c00 0000 723b 0000 0072 3c00  ...r....r;...r<.
-00001680: 0000 7212 0000 0072 5000 0000 7224 0000  ..r....rP...r$..
-00001690: 0072 1d00 0000 720a 0000 0072 0900 0000  .r....r....r....
-000016a0: 7211 0000 0072 0b00 0000 290e 7214 0000  r....r....).r...
-000016b0: 00da 0576 616c 7565 7236 0000 0072 4800  ...valuer6...rH.
-000016c0: 0000 7249 0000 0072 3800 0000 7232 0000  ..rI...r8...r2..
-000016d0: 0072 4a00 0000 7221 0000 0072 3300 0000  .rJ...r!...r3...
-000016e0: 724c 0000 0072 3700 0000 724d 0000 0072  rL...r7...rM...r
-000016f0: 4e00 0000 730e 0000 0020 2020 2020 2020  N...s....       
-00001700: 2020 2020 2020 2072 1500 0000 7250 0000         r....rP..
-00001710: 007a 1444 656e 6472 6974 654c 6f63 6174  .z.DendriteLocat
-00001720: 6f72 2e66 696c 6c69 0000 0073 4701 0000  or.filli...sG...
-00001730: e800 f880 00d8 0b1b 9872 d20b 21e0 1221  .........r..!..!
-00001740: a025 a017 d028 4ed0 104f f003 000d 1df0  .%...(N..O......
-00001750: 0800 161a d715 2ad1 152a d715 39d1 1539  ......*..*..9..9
-00001760: d315 3b88 0ae0 1c20 d71c 31d1 1c31 d71c  ..;.... ..1..1..
-00001770: 41d1 1c41 d31c 43d7 1643 880b d821 2cd7  A..A..C..C...!,.
-00001780: 2141 d121 41d3 2143 d71b 43d0 0818 e012  !A.!A.!C..C.....
-00001790: 1897 2a91 2a98 59a8 04d3 122d 8807 d80e  ..*.*.Y....-....
-000017a0: 1f88 648f 6c89 6cd7 0e1f d10e 1fa0 05d0  ..d.l.l.........
-000017b0: 0e48 b814 d20e 48a8 77d0 0e48 c016 d10e  .H....H.w..H....
-000017c0: 48d7 0848 d008 48e0 0e12 d70e 28d1 0e28  H..H..H.....(..(
-000017d0: a81b af1f a91f d30e 39d7 0839 d008 39e0  ........9..9..9.
-000017e0: 1b1f d71b 30d1 1b30 d71b 40d1 1b40 d31b  ....0..0..@..@..
-000017f0: 42d7 1542 880a d820 2ad7 203f d120 3fd3  B..B... *. ?. ?.
-00001800: 2041 d71a 4188 0fdc 2135 d818 28b0 5ff4   A..A...!5..(._.
-00001810: 0302 220a d008 1ef4 0800 0f21 d810 1b97  .."........!....
-00001820: 0f91 0fd8 181c d718 28d1 1828 d81d 23d8  ........(..(..#.
-00001830: 1d2d d823 39d8 1721 f40d 070f 0a88 03f4  .-.#9..!........
-00001840: 1000 1525 a053 d314 29d7 0e29 8803 d80f  ...%.S..)..)....
-00001850: 1288 0af0 2f00 1744 01f8 d81b 43f8 f006  ..../..D....C...
-00001860: 0009 4901 f8e0 0839 f8e0 1542 f8d8 1a41  ..I....9...B...A
-00001870: f8f0 1a00 0f2a fa73 7f00 0000 8241 0345  .....*.s.....A.E
-00001880: 1001 c105 0145 0204 c106 1745 1001 c11d  .....E.....E....
-00001890: 0145 0404 c11e 3b45 1001 c219 0145 0604  .E....;E.....E..
-000018a0: c21a 2245 1001 c23c 0145 0804 c23d 2145  .."E...<.E...=!E
-000018b0: 1001 c31e 0145 0a04 c31f 1745 1001 c336  .....E.....E...6
-000018c0: 0145 0c04 c337 4104 4510 01c4 3b01 450e  .E...7A.E...;.E.
-000018d0: 04c4 3c07 4510 01c5 0401 4510 01c5 0601  ..<.E.....E.....
-000018e0: 4510 01c5 0801 4510 01c5 0a01 4510 01c5  E.....E.....E...
-000018f0: 0c01 4510 01c5 0e01 4510 014e 2906 7211  ..E.....E..N).r.
-00001900: 0000 00da 0373 7472 7212 0000 0072 0400  .....strr....r..
-00001910: 0000 7213 0000 0072 0800 0000 2902 da06  ..r....r....)...
-00001920: 7265 7475 726e 7204 0000 0029 01e9 0200  returnr....)....
-00001930: 0000 2904 7220 0000 0072 5200 0000 7221  ..).r ...rR...r!
-00001940: 0000 00da 0566 6c6f 6174 2901 722a 0000  .....float).r*..
-00001950: 0029 0272 5300 0000 720c 0000 0029 0272  .).rS...r....).r
-00001960: 5100 0000 7252 0000 0029 08da 085f 5f6e  Q...rR...)...__n
-00001970: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00001980: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00001990: 1600 0000 7219 0000 0072 2400 0000 7228  ....r....r$...r(
-000019a0: 0000 0072 5000 0000 a900 7217 0000 0072  ...rP.....r....r
-000019b0: 1500 0000 720e 0000 0072 0e00 0000 1800  ....r....r......
-000019c0: 0000 7334 0000 0084 00f0 0205 0531 d81b  ..s4.........1..
-000019d0: 1ef0 0305 0531 d829 30f0 0305 0531 d844  .....1.)0....1.D
-000019e0: 53f3 0305 0531 f30e 0105 1cf4 0607 0515  S....1..........
-000019f0: f412 3b05 13f5 7a01 1f05 1372 1700 0000  ..;...z....r....
-00001a00: 720e 0000 0029 18da 0a5f 5f66 7574 7572  r....)...__futur
-00001a10: 655f 5f72 0300 0000 721e 0000 0072 4200  e__r....r....rB.
-00001a20: 0000 721b 0000 00da 1470 6c61 7977 7269  ..r......playwri
-00001a30: 6768 742e 6173 796e 635f 6170 6972 0400  ght.async_apir..
-00001a40: 0000 da06 7479 7069 6e67 7205 0000 00da  ....typingr.....
-00001a50: 3064 656e 6472 6974 655f 7079 7468 6f6e  0dendrite_python
-00001a60: 5f73 646b 2e65 7863 6570 7469 6f6e 732e  _sdk.exceptions.
-00001a70: 4465 6e64 7269 7465 4578 6365 7074 696f  DendriteExceptio
-00001a80: 6e72 0600 0000 da38 6465 6e64 7269 7465  nr.....8dendrite
-00001a90: 5f70 7974 686f 6e5f 7364 6b2e 6578 6365  _python_sdk.exce
-00001aa0: 7074 696f 6e73 2e49 6e63 6f72 7265 6374  ptions.Incorrect
-00001ab0: 4f75 7463 6f6d 6545 7863 6570 7469 6f6e  OutcomeException
-00001ac0: 7207 0000 00da 1364 656e 6472 6974 655f  r......dendrite_
-00001ad0: 7079 7468 6f6e 5f73 646b 7208 0000 00da  python_sdkr.....
-00001ae0: 2a64 656e 6472 6974 655f 7079 7468 6f6e  *dendrite_python
-00001af0: 5f73 646b 2e64 746f 2e4d 616b 6549 6e74  _sdk.dto.MakeInt
-00001b00: 6572 6163 7469 6f6e 4454 4f72 0900 0000  eractionDTOr....
-00001b10: da2f 6465 6e64 7269 7465 5f70 7974 686f  ./dendrite_pytho
-00001b20: 6e5f 7364 6b2e 6d6f 6465 6c73 2e50 6167  n_sdk.models.Pag
-00001b30: 6544 656c 7461 496e 666f 726d 6174 696f  eDeltaInformatio
-00001b40: 6e72 0a00 0000 da23 6465 6e64 7269 7465  nr.....#dendrite
-00001b50: 5f70 7974 686f 6e5f 7364 6b2e 7265 7175  _python_sdk.requ
-00001b60: 6573 745f 6861 6e64 6c65 7272 0b00 0000  est_handlerr....
-00001b70: da31 6465 6e64 7269 7465 5f70 7974 686f  .1dendrite_pytho
-00001b80: 6e5f 7364 6b2e 7265 7370 6f6e 7365 732e  n_sdk.responses.
-00001b90: 496e 7465 7261 6374 696f 6e52 6573 706f  InteractionRespo
-00001ba0: 6e73 6572 0c00 0000 720e 0000 0072 5900  nser....r....rY.
-00001bb0: 0000 7217 0000 0072 1500 0000 fa08 3c6d  ..r....r......<m
-00001bc0: 6f64 756c 653e 7264 0000 0001 0000 0073  odule>rd.......s
-00001bd0: 3f00 0000 f003 0101 01dd 0022 db00 0edb  ?.........."....
-00001be0: 0009 db00 0be5 0028 e500 20e5 004e f502  .......(.. ..N..
-00001bf0: 0201 02f1 0800 0411 dd04 33e5 0049 dd00  ..........3..I..
-00001c00: 50dd 0040 dd00 51f7 0670 0101 13f2 0070  P..@..Q..p.....p
-00001c10: 0101 1372 1700 0000                      ...r....
+00001410: 006a 0c00 0000 0000 0000 0000 0000 0000  .j..............
+00001420: 0000 0000 007c 0167 017c 03a2 01ad 0664  .....|.g.|.....d
+00001430: 047c 0869 017c 04a4 018e 0183 0064 007b  .|.i.|.......d.{
+00001440: 0300 0096 0297 0386 0505 0001 007c 006a  .............|.j
+00001450: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
+00001460: 0000 007c 066a 1000 0000 0000 0000 0000  ...|.j..........
+00001470: 0000 0000 0000 0000 00ab 0100 0000 0000  ................
+00001480: 0083 0064 007b 0300 0096 0297 0386 0505  ...d.{..........
+00001490: 0001 007c 006a 0000 0000 0000 0000 0000  ...|.j..........
+000014a0: 0000 0000 0000 0000 006a 0500 0000 0000  .........j......
+000014b0: 0000 0000 0000 0000 0000 0000 00ab 0000  ................
+000014c0: 0000 0000 0083 0064 007b 0300 0096 0297  .......d.{......
+000014d0: 0386 0505 007d 097c 096a 0700 0000 0000  .....}.|.j......
+000014e0: 0000 0000 0000 0000 0000 0000 00ab 0000  ................
+000014f0: 0000 0000 0083 0064 007b 0300 0096 0297  .......d.{......
+00001500: 0386 0505 007d 0a74 1300 0000 0000 0000  .....}.t........
+00001510: 007c 077c 0aac 06ab 0200 0000 0000 007d  .|.|...........}
+00001520: 0b74 1500 0000 0000 0000 007c 066a 1000  .t.........|.j..
+00001530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001540: 007c 006a 1600 0000 0000 0000 0000 0000  .|.j............
+00001550: 0000 0000 0000 0064 077c 027c 0b7c 05ac  .......d.|.|.|..
+00001560: 08ab 0600 0000 0000 007d 0c74 1900 0000  .........}.t....
+00001570: 0000 0000 007c 0cab 0100 0000 0000 0083  .....|..........
+00001580: 0064 007b 0300 0096 0297 0386 0505 007d  .d.{...........}
+00001590: 0d7c 0d53 0037 008c fc37 008c e637 008c  .|.S.7...7...7..
+000015a0: ac37 008c 8b37 008c 6b37 008c 5537 008c  .7...7..k7..U7..
+000015b0: 12ad 0377 0129 094e 722a 0000 007a 0f54  ...w.).Nr*...z.T
+000015c0: 6861 7420 7468 6520 7465 7874 2027 7a26  hat the text 'z&
+000015d0: 2720 6973 2066 696c 6c65 6420 696e 746f  ' is filled into
+000015e0: 2074 6865 2074 6172 6765 7465 6420 656c   the targeted el
+000015f0: 656d 656e 742e 7221 0000 0072 2600 0000  ement.r!...r&...
+00001600: 7231 0000 00da 0466 696c 6c72 3400 0000  r1.....fillr4...
+00001610: 290d 7213 0000 0072 3a00 0000 721c 0000  ).r....r:...r...
+00001620: 0072 3b00 0000 723c 0000 0072 1200 0000  .r;...r<...r....
+00001630: 724f 0000 0072 2400 0000 721d 0000 0072  rO...r$...r....r
+00001640: 0a00 0000 7209 0000 0072 1100 0000 720b  ....r....r....r.
+00001650: 0000 0029 0e72 1400 0000 da05 7661 6c75  ...).r......valu
+00001660: 6572 3600 0000 7247 0000 0072 4800 0000  er6...rG...rH...
+00001670: 7238 0000 0072 3200 0000 7249 0000 0072  r8...r2...rI...r
+00001680: 2100 0000 7233 0000 0072 4b00 0000 7237  !...r3...rK...r7
+00001690: 0000 0072 4c00 0000 724d 0000 0073 0e00  ...rL...rM...s..
+000016a0: 0000 2020 2020 2020 2020 2020 2020 2020  ..              
+000016b0: 7215 0000 0072 4f00 0000 7a14 4465 6e64  r....rO...z.Dend
+000016c0: 7269 7465 4c6f 6361 746f 722e 6669 6c6c  riteLocator.fill
+000016d0: 6700 0000 7347 0100 00e8 00f8 8000 d80b  g...sG..........
+000016e0: 1b98 72d2 0b21 e012 21a0 25a0 17d0 284e  ..r..!..!.%...(N
+000016f0: d010 4ff0 0300 0d1d f008 0016 1ad7 152a  ..O............*
+00001700: d115 2ad7 1539 d115 39d3 153b 880a e01c  ..*..9..9..;....
+00001710: 20d7 1c31 d11c 31d7 1c41 d11c 41d3 1c43   ..1..1..A..A..C
+00001720: d716 4388 0bd8 212c d721 41d1 2141 d321  ..C...!,.!A.!A.!
+00001730: 43d7 1b43 d008 18e0 1218 972a 912a 9859  C..C.......*.*.Y
+00001740: a804 d312 2d88 07d8 0e1f 8864 8f6c 896c  ....-......d.l.l
+00001750: d70e 1fd1 0e1f a005 d00e 48b8 14d2 0e48  ..........H....H
+00001760: a877 d00e 48c0 16d1 0e48 d708 48d0 0848  .w..H....H..H..H
+00001770: e00e 12d7 0e28 d10e 28a8 1baf 1fa9 1fd3  .....(..(.......
+00001780: 0e39 d708 39d0 0839 e01b 1fd7 1b30 d11b  .9..9..9.....0..
+00001790: 30d7 1b40 d11b 40d3 1b42 d715 4288 0ad8  0..@..@..B..B...
+000017a0: 202a d720 3fd1 203f d320 41d7 1a41 880f   *. ?. ?. A..A..
+000017b0: dc21 35d8 1828 b05f f403 0222 0ad0 081e  .!5..(._..."....
+000017c0: f408 000f 21d8 101b 970f 910f d818 1cd7  ....!...........
+000017d0: 1828 d118 28d8 1d23 d81d 2dd8 2339 d817  .(..(..#..-.#9..
+000017e0: 21f4 0d07 0f0a 8803 f410 0015 25a0 53d3  !...........%.S.
+000017f0: 1429 d70e 2988 03d8 0f12 880a f02f 0017  .)..)......../..
+00001800: 4401 f8d8 1b43 f8f0 0600 0949 01f8 e008  D....C.....I....
+00001810: 39f8 e015 42f8 d81a 41f8 f01a 000f 2afa  9...B...A.....*.
+00001820: 737f 0000 0082 4103 4510 01c1 0501 4502  s.....A.E.....E.
+00001830: 04c1 0617 4510 01c1 1d01 4504 04c1 1e3b  ....E.....E....;
+00001840: 4510 01c2 1901 4506 04c2 1a22 4510 01c2  E.....E...."E...
+00001850: 3c01 4508 04c2 3d21 4510 01c3 1e01 450a  <.E...=!E.....E.
+00001860: 04c3 1f17 4510 01c3 3601 450c 04c3 3741  ....E...6.E...7A
+00001870: 0445 1001 c43b 0145 0e04 c43c 0745 1001  .E...;.E...<.E..
+00001880: c504 0145 1001 c506 0145 1001 c508 0145  ...E.....E.....E
+00001890: 1001 c50a 0145 1001 c50c 0145 1001 c50e  .....E.....E....
+000018a0: 0145 1001 4e29 0672 1100 0000 da03 7374  .E..N).r......st
+000018b0: 7272 1200 0000 7204 0000 0072 1300 0000  rr....r....r....
+000018c0: 7208 0000 0029 02da 0672 6574 7572 6e72  r....)...returnr
+000018d0: 0400 0000 2901 e902 0000 0029 0472 2000  ....)......).r .
+000018e0: 0000 7251 0000 0072 2100 0000 da05 666c  ..rQ...r!.....fl
+000018f0: 6f61 7429 0172 2a00 0000 2902 7252 0000  oat).r*...).rR..
+00001900: 0072 0c00 0000 2902 7250 0000 0072 5100  .r....).rP...rQ.
+00001910: 0000 2908 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+00001920: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00001930: 616c 6e61 6d65 5f5f 7216 0000 0072 1900  alname__r....r..
+00001940: 0000 7224 0000 0072 2800 0000 724f 0000  ..r$...r(...rO..
+00001950: 00a9 0072 1700 0000 7215 0000 0072 0e00  ...r....r....r..
+00001960: 0000 720e 0000 0018 0000 0073 3400 0000  ..r........s4...
+00001970: 8400 f002 0505 31d8 1b1e f003 0505 31d8  ......1.......1.
+00001980: 2930 f003 0505 31d8 4453 f303 0505 31f3  )0....1.DS....1.
+00001990: 0e01 051c f406 0705 15f4 1239 0513 f576  ...........9...v
+000019a0: 011f 0513 7217 0000 0072 0e00 0000 2918  ....r....r....).
+000019b0: da0a 5f5f 6675 7475 7265 5f5f 7203 0000  ..__future__r...
+000019c0: 0072 1e00 0000 7242 0000 0072 1b00 0000  .r....rB...r....
+000019d0: da14 706c 6179 7772 6967 6874 2e61 7379  ..playwright.asy
+000019e0: 6e63 5f61 7069 7204 0000 00da 0674 7970  nc_apir......typ
+000019f0: 696e 6772 0500 0000 da30 6465 6e64 7269  ingr.....0dendri
+00001a00: 7465 5f70 7974 686f 6e5f 7364 6b2e 6578  te_python_sdk.ex
+00001a10: 6365 7074 696f 6e73 2e44 656e 6472 6974  ceptions.Dendrit
+00001a20: 6545 7863 6570 7469 6f6e 7206 0000 00da  eExceptionr.....
+00001a30: 3864 656e 6472 6974 655f 7079 7468 6f6e  8dendrite_python
+00001a40: 5f73 646b 2e65 7863 6570 7469 6f6e 732e  _sdk.exceptions.
+00001a50: 496e 636f 7272 6563 744f 7574 636f 6d65  IncorrectOutcome
+00001a60: 4578 6365 7074 696f 6e72 0700 0000 da13  Exceptionr......
+00001a70: 6465 6e64 7269 7465 5f70 7974 686f 6e5f  dendrite_python_
+00001a80: 7364 6b72 0800 0000 da2a 6465 6e64 7269  sdkr.....*dendri
+00001a90: 7465 5f70 7974 686f 6e5f 7364 6b2e 6474  te_python_sdk.dt
+00001aa0: 6f2e 4d61 6b65 496e 7465 7261 6374 696f  o.MakeInteractio
+00001ab0: 6e44 544f 7209 0000 00da 2f64 656e 6472  nDTOr...../dendr
+00001ac0: 6974 655f 7079 7468 6f6e 5f73 646b 2e6d  ite_python_sdk.m
+00001ad0: 6f64 656c 732e 5061 6765 4465 6c74 6149  odels.PageDeltaI
+00001ae0: 6e66 6f72 6d61 7469 6f6e 720a 0000 00da  nformationr.....
+00001af0: 2364 656e 6472 6974 655f 7079 7468 6f6e  #dendrite_python
+00001b00: 5f73 646b 2e72 6571 7565 7374 5f68 616e  _sdk.request_han
+00001b10: 646c 6572 720b 0000 00da 3164 656e 6472  dlerr.....1dendr
+00001b20: 6974 655f 7079 7468 6f6e 5f73 646b 2e72  ite_python_sdk.r
+00001b30: 6573 706f 6e73 6573 2e49 6e74 6572 6163  esponses.Interac
+00001b40: 7469 6f6e 5265 7370 6f6e 7365 720c 0000  tionResponser...
+00001b50: 0072 0e00 0000 7258 0000 0072 1700 0000  .r....rX...r....
+00001b60: 7215 0000 00fa 083c 6d6f 6475 6c65 3e72  r......<module>r
+00001b70: 6300 0000 0100 0000 733f 0000 00f0 0301  c.......s?......
+00001b80: 0101 dd00 22db 000e db00 09db 000b e500  ...."...........
+00001b90: 28e5 0020 e500 4ef5 0202 0102 f108 0004  (.. ..N.........
+00001ba0: 11dd 0433 e500 49dd 0050 dd00 40dd 0051  ...3..I..P..@..Q
+00001bb0: f706 6e01 0113 f200 6e01 0113 7217 0000  ..n.....n...r...
+00001bc0: 00                                       .
```

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/DendritePage.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/DendritePage.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun May 26 16:58:56 2024 UTC, .py size: 6384 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 506a 5366 f018 0000  ........PjSf....
+00000000: cb0d 0d0a 0000 0000 288a 5566 ec18 0000  ........(.Uf....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 fc00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6403 6c05 6d06 5a06 6d07 5a07 0100  d.d.l.m.Z.m.Z...
 00000060: 6400 6404 6c08 6d09 5a09 0100 6400 6405  d.d.l.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  l.m.Z.m.Z.m.Z.m.
@@ -186,15 +186,15 @@
 00000b90: 6c5f 706f 7369 7469 6f6e da0a 7374 6172  l_position..star
 00000ba0: 745f 7469 6d65 da17 6375 7272 656e 745f  t_time..current_
 00000bb0: 7363 726f 6c6c 5f70 6f73 6974 696f 6e73  scroll_positions
 00000bc0: 0500 0000 2020 2020 2072 1f00 0000 da10  ....     r......
 00000bd0: 7363 726f 6c6c 5f74 6f5f 626f 7474 6f6d  scroll_to_bottom
 00000be0: 7a1d 4465 6e64 7269 7465 5061 6765 2e73  z.DendritePage.s
 00000bf0: 6372 6f6c 6c5f 746f 5f62 6f74 746f 6d45  croll_to_bottomE
-00000c00: 0000 0073 bc00 0000 e800 f880 00d8 0c0d  ...s............
+00000c00: 0000 0073 bc00 0000 e800 f880 00e0 0c0d  ...s............
 00000c10: 8801 d81f 20d0 081c dc15 1997 5991 5993  .... .......Y.Y.
 00000c20: 5b88 0ae0 0e12 d82c 30af 49a9 49d7 2c3e  [......,0.I.I.,>
 00000c30: d12c 3ed0 3f4f d32c 50d7 2650 d00c 23e0  .,>.?O.,P.&P..#.
 00000c40: 1216 9729 9129 d712 24d1 1224 d027 3ab8  ...).)..$..$.':.
 00000c50: 31b8 23b8 51d0 253f d312 40d7 0c40 d00c  1.#.Q.%?..@..@..
 00000c60: 40d8 0c0d 9015 894a 8841 e40f 138f 7989  @......J.A....y.
 00000c70: 798b 7b98 5ad1 0f27 a821 d20f 2bd8 1015  y.{.Z..'.!..+...
@@ -237,15 +237,15 @@
 00000ec0: 721e 0000 00da 0b64 656e 6472 6974 655f  r......dendrite_
 00000ed0: 6964 da02 656c da01 6573 0400 0000 2020  id..el..es....  
 00000ee0: 2020 721f 0000 00da 1c67 6574 5f65 6c65    r......get_ele
 00000ef0: 6d65 6e74 5f66 726f 6d5f 6465 6e64 7269  ment_from_dendri
 00000f00: 7465 5f69 647a 2944 656e 6472 6974 6550  te_idz)DendriteP
 00000f10: 6167 652e 6765 745f 656c 656d 656e 745f  age.get_element_
 00000f20: 6672 6f6d 5f64 656e 6472 6974 655f 6964  from_dendrite_id
-00000f30: 5a00 0000 7387 0000 00e8 00f8 8000 f002  Z...s...........
+00000f30: 5b00 0000 7387 0000 00e8 00f8 8000 f002  [...s...........
 00000f40: 0809 0ed8 1216 d712 2cd1 122c d312 2ed7  ........,..,....
 00000f50: 0c2e d00c 2ed8 1115 9719 9119 d711 22d1  ..............".
 00000f60: 1122 d025 36b0 7bb0 6dc0 32d0 2346 d311  .".%6.{.m.2.#F..
 00000f70: 4788 42d8 1214 972b 912b a063 902b d312  G.B....+.+.c.+..
 00000f80: 2ad7 0c2a d00c 2ad8 1315 9738 9138 884f  *..*..*....8.8.O
 00000f90: f007 000d 2ff8 e00c 2af9 e40f 18f2 0003  ..../...*.......
 00000fa0: 090e dc12 1bd8 123e b87b b86d d010 4cf3  .......>.{.m..L.
@@ -286,15 +286,15 @@
 000011d0: 6f74 7213 0000 0072 2300 0000 da03 7374  otr....r#.....st
 000011e0: 7229 0472 1e00 0000 da04 736f 7570 da15  r).r......soup..
 000011f0: 696e 7465 7261 6374 6162 6c65 5f65 6c65  interactable_ele
 00001200: 6d65 6e74 73da 0662 6173 6536 3473 0400  ments..base64s..
 00001210: 0000 2020 2020 721f 0000 0072 3000 0000  ..    r....r0...
 00001220: 7a21 4465 6e64 7269 7465 5061 6765 2e67  z!DendritePage.g
 00001230: 6574 5f70 6167 655f 696e 666f 726d 6174  et_page_informat
-00001240: 696f 6e65 0000 0073 8100 0000 e800 f880  ione...s........
+00001240: 696f 6e66 0000 0073 8100 0000 e800 f880  ionf...s........
 00001250: 00d8 1519 975d 915d 935f d70f 2488 04dc  .....].]._..$...
 00001260: 264e d80c 108f 4989 49f3 0302 270a f700  &N....I.I...'...
 00001270: 0221 0ad0 081d f006 0018 1cd7 172e d117  .!..............
 00001280: 2ed7 1747 d117 47c8 04cf 09c9 09d3 1752  ...G..G........R
 00001290: d711 5288 06e4 0f1e d810 1497 0991 0997  ..R.............
 000012a0: 0d91 0ddc 1518 9814 9359 d826 3bd8 1e24  .........Y.&;..$
 000012b0: f409 0510 0af0 0005 090a f00d 0010 25f8  ..............%.
@@ -371,216 +371,213 @@
 00001720: 4174 7472 6962 7574 6528 2764 2d69 6427  Attribute('d-id'
 00001730: 2c20 756e 6971 7565 4964 293b 0a7d 293b  , uniqueId);.});
 00001740: 0a0a 2902 721b 0000 0072 3e00 0000 2902  ..).r....r>...).
 00001750: 721e 0000 00da 0673 6372 6970 7473 0200  r......scripts..
 00001760: 0000 2020 721f 0000 0072 4800 0000 7a22  ..  r....rH...z"
 00001770: 4465 6e64 7269 7465 5061 6765 2e67 656e  DendritePage.gen
 00001780: 6572 6174 655f 6465 6e64 7269 7465 5f69  erate_dendrite_i
-00001790: 6473 7300 0000 7328 0000 00e8 00f8 8000  dss...s(........
+00001790: 6473 7400 0000 7328 0000 00e8 00f8 8000  dst...s(........
 000017a0: f002 1e12 0488 06f0 4001 000f 138f 6989  ........@.....i.
 000017b0: 69d7 0e20 d10e 20a0 16d3 0e28 d708 28d2  i.. .. ....(..(.
 000017c0: 0828 fa73 0c00 0000 8221 2b01 a301 2904  .(.s.....!+...).
 000017d0: a406 2b01 6301 0000 0000 0000 0000 0000  ..+.c...........
 000017e0: 0003 0000 0083 0000 01f3 4000 0000 4b00  ..........@...K.
 000017f0: 0100 9700 7c00 6a01 0000 0000 0000 0000  ....|.j.........
 00001800: 0000 0000 0000 0000 0000 ab00 0000 0000  ................
 00001810: 0000 8300 6400 7b03 0000 9602 9703 8605  ....d.{.........
 00001820: 0500 0100 7900 3700 8c05 ad03 7701 721a  ....y.7.....w.r.
 00001830: 0000 0029 0172 4500 0000 7224 0000 0073  ...).rE...r$...s
 00001840: 0100 0000 2072 1f00 0000 da1a 7363 726f  .... r......scro
 00001850: 6c6c 5f74 6872 6f75 6768 5f65 6e74 6972  ll_through_entir
 00001860: 655f 7061 6765 7a27 4465 6e64 7269 7465  e_pagez'Dendrite
 00001870: 5061 6765 2e73 6372 6f6c 6c5f 7468 726f  Page.scroll_thro
-00001880: 7567 685f 656e 7469 7265 5f70 6167 6596  ugh_entire_page.
+00001880: 7567 685f 656e 7469 7265 5f70 6167 6597  ugh_entire_page.
 00001890: 0000 0073 1800 0000 e800 f880 00d8 0e12  ...s............
 000018a0: d70e 23d1 0e23 d30e 25d7 0825 d208 25fa  ..#..#..%..%..%.
 000018b0: 730c 0000 0082 141e 0196 011c 0497 061e  s...............
 000018c0: 0163 0400 0000 0000 0000 0000 0000 0500  .c..............
-000018d0: 0000 8300 0001 f31c 0200 004b 0001 0097  ...........K....
+000018d0: 0000 8300 0001 f304 0200 004b 0001 0097  ...........K....
 000018e0: 007c 006a 0000 0000 0000 0000 0000 0000  .|.j............
 000018f0: 0000 0000 0000 006a 0300 0000 0000 0000  .......j........
 00001900: 0000 0000 0000 0000 0000 00ab 0000 0000  ................
 00001910: 0000 007d 0464 017d 057c 057c 036b 0200  ...}.d.}.|.|.k..
-00001920: 0072 af7c 006a 0500 0000 0000 0000 0000  .r.|.j..........
+00001920: 0072 a37c 006a 0500 0000 0000 0000 0000  .r.|.j..........
 00001930: 0000 0000 0000 0000 00ab 0000 0000 0000  ................
 00001940: 0083 0064 007b 0300 0096 0297 0386 0505  ...d.{..........
 00001950: 007d 0674 0700 0000 0000 0000 007c 067c  .}.t.........|.|
 00001960: 047c 01ac 02ab 0300 0000 0000 007d 0774  .|...........}.t
 00001970: 0900 0000 0000 0000 007c 07ab 0100 0000  .........|......
 00001980: 0000 0083 0064 007b 0300 0096 0297 0386  .....d.{........
-00001990: 0505 007d 0874 0b00 0000 0000 0000 0064  ...}.t.........d
-000019a0: 037c 08ab 0200 0000 0000 0001 007c 0872  .|...........|.r
-000019b0: 407c 0864 0419 0000 0064 056b 3700 0072  @|.d.....d.k7..r
-000019c0: 387c 006a 0d00 0000 0000 0000 0000 0000  8|.j............
-000019d0: 0000 0000 0000 007c 0864 0419 0000 00ab  .......|.d......
-000019e0: 0100 0000 0000 0083 0064 007b 0300 0096  .........d.{....
-000019f0: 0297 0386 0505 007d 0974 0f00 0000 0000  .......}.t......
-00001a00: 0000 007c 0864 0419 0000 007c 097c 006a  ...|.d.....|.|.j
-00001a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001a20: 0000 00ab 0300 0000 0000 007d 0a7c 0a53  ...........}.|.S
-00001a30: 007c 0564 067a 0d00 007d 0574 1100 0000  .|.d.z...}.t....
-00001a40: 0000 0000 006a 1200 0000 0000 0000 0000  .....j..........
-00001a50: 0000 0000 0000 0000 007c 02ab 0100 0000  .........|......
-00001a60: 0000 0083 0064 007b 0300 0096 0297 0386  .....d.{........
-00001a70: 0505 0001 007c 057c 036b 0200 0072 018c  .....|.|.k...r..
-00001a80: af7c 006a 0500 0000 0000 0000 0000 0000  .|.j............
-00001a90: 0000 0000 0000 00ab 0000 0000 0000 0083  ................
-00001aa0: 0064 007b 0300 0096 0297 0386 0505 007d  .d.{...........}
-00001ab0: 0674 1500 0000 0000 0000 0064 077c 066a  .t.........d.|.j
-00001ac0: 1600 0000 0000 0000 0000 0000 0000 0000  ................
-00001ad0: 0000 00ac 08ab 0200 0000 0000 0082 0137  ...............7
-00001ae0: 008c ca37 008c ab37 008c 7b37 008c 3f37  ...7...7..{7..?7
-00001af0: 008c 23ad 0377 0129 094e 7202 0000 0029  ..#..w.).Nr....)
-00001b00: 0372 2800 0000 7229 0000 0072 2a00 0000  .r(...r)...r*...
-00001b10: 7a05 7265 733a 2072 4d00 0000 da00 e901  z.res: rM.......
-00001b20: 0000 007a 2c43 6f75 6c64 206e 6f74 2066  ...z,Could not f
-00001b30: 696e 6420 7375 6974 6162 6c65 2065 6c65  ind suitable ele
-00001b40: 6d65 6e74 206f 6e20 7468 6520 7061 6765  ment on the page
-00001b50: 2e29 02da 076d 6573 7361 6765 7254 0000  .)...messagerT..
-00001b60: 0029 0c72 1d00 0000 7231 0000 0072 3000  .).r....r1...r0.
-00001b70: 0000 7212 0000 0072 1500 0000 da05 7072  ..r....r......pr
-00001b80: 696e 7472 5000 0000 7214 0000 0072 3f00  intrP...r....r?.
-00001b90: 0000 7240 0000 0072 0d00 0000 7254 0000  ..r@...r....rT..
-00001ba0: 0029 0b72 1e00 0000 722a 0000 0072 4700  .).r....r*...rG.
-00001bb0: 0000 da0b 6d61 785f 7265 7472 6965 7372  ....max_retriesr
-00001bc0: 2900 0000 da0c 6e75 6d5f 6174 7465 6d70  ).....num_attemp
-00001bd0: 7473 7228 0000 0072 3600 0000 7237 0000  tsr(...r6...r7..
-00001be0: 0072 4900 0000 da10 6465 6e64 7269 7465  .rI.....dendrite
-00001bf0: 5f6c 6f63 6174 6f72 730b 0000 0020 2020  _locators....   
-00001c00: 2020 2020 2020 2020 721f 0000 00da 1867          r......g
-00001c10: 6574 5f69 6e74 6572 6163 7461 626c 655f  et_interactable_
-00001c20: 656c 656d 656e 747a 2544 656e 6472 6974  elementz%Dendrit
-00001c30: 6550 6167 652e 6765 745f 696e 7465 7261  ePage.get_intera
-00001c40: 6374 6162 6c65 5f65 6c65 6d65 6e74 9900  ctable_element..
-00001c50: 0000 7322 0100 00e8 00f8 8000 f00c 0016  ..s"............
-00001c60: 1ad7 152a d115 2ad7 1539 d115 39d3 153b  ...*..*..9..9..;
-00001c70: 880a e017 1888 0cd8 0e1a 985b d20e 28d8  ...........[..(.
-00001c80: 2529 d725 3ed1 253e d325 40d7 1f40 d00c  %).%>.%>.%@..@..
-00001c90: 1ce4 1223 d821 31b8 6ad0 5157 f403 0213  ...#.!1.j.QW....
-00001ca0: 0e88 43f4 0800 1928 a803 d318 2cd7 122c  ..C....(....,..,
-00001cb0: 8843 dc0c 1190 2798 33d4 0c1f d90f 1290  .C....'.3.......
-00001cc0: 7398 3dd1 1729 a852 d217 2fd8 2024 d720  s.=..).R../. $. 
-00001cd0: 41d1 2041 c023 c06d d142 54d3 2055 d71a  A. A.#.m.BT. U..
-00001ce0: 5590 07dc 2332 d814 1798 0dd1 1426 a807  U...#2.......&..
-00001cf0: b014 d731 46d1 3146 f303 0224 12d0 1020  ...1F.1F...$... 
-00001d00: f006 0018 28d0 1027 d80c 1898 41d1 0c1d  ....(..'....A...
-00001d10: 884c dc12 1997 2d91 2da0 07d3 1228 d70c  .L....-.-....(..
-00001d20: 28d0 0c28 f021 000f 1b98 5bd3 0e28 f024  (..(.!....[..(.$
-00001d30: 0022 26d7 213a d121 3ad3 213c d71b 3cd0  ."&.!:.!:.!<..<.
-00001d40: 0818 dc0e 1fd8 1442 d81e 2ed7 1e40 d11e  .......B.....@..
-00001d50: 40f4 0503 0f0a f000 0309 0af0 2500 2041  @...........%. A
-00001d60: 01f8 f00c 0013 2df8 f006 001b 5601 f8f0  ......-.....V...
-00001d70: 0c00 0d29 f8e0 1b3c fa73 5d00 0000 8235  ...)...<.s]....5
-00001d80: 440c 01b7 0144 0204 b820 440c 01c1 1801  D....D... D.....
-00001d90: 4404 04c1 1931 440c 01c2 0a01 4406 04c2  D....1D.....D...
-00001da0: 0b3d 440c 01c3 0801 4408 04c3 0909 440c  .=D.....D.....D.
-00001db0: 01c3 1313 440c 01c3 2601 440a 04c3 271c  ....D...&.D...'.
-00001dc0: 440c 01c4 0401 440c 01c4 0601 440c 01c4  D.....D.....D...
-00001dd0: 0801 440c 01c4 0a01 440c 0163 0100 0000  ..D.....D..c....
-00001de0: 0000 0000 0000 0000 0400 0000 8300 0001  ................
-00001df0: f3a2 0000 004b 0001 0097 007c 006a 0100  .....K.....|.j..
-00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e10: 00ab 0000 0000 0000 0083 0064 007b 0300  ...........d.{..
-00001e20: 0096 0297 0386 0505 0001 007c 006a 0200  ...........|.j..
-00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e40: 006a 0500 0000 0000 0000 0000 0000 0000  .j..............
-00001e50: 0000 0000 00ab 0000 0000 0000 0083 0064  ...............d
-00001e60: 007b 0300 0096 0297 0386 0505 007d 0174  .{...........}.t
-00001e70: 0700 0000 0000 0000 007c 0164 01ab 0200  .........|.d....
-00001e80: 0000 0000 007d 027c 0253 0037 008c 3437  .....}.|.S.7..47
-00001e90: 008c 14ad 0377 0129 024e da04 6c78 6d6c  .....w.).N..lxml
-00001ea0: 2904 7248 0000 0072 1b00 0000 da07 636f  ).rH...r......co
-00001eb0: 6e74 656e 7472 0600 0000 2903 721e 0000  ntentr....).r...
-00001ec0: 00da 0b70 6167 655f 736f 7572 6365 7258  ...page_sourcerX
-00001ed0: 0000 0073 0300 0000 2020 2072 1f00 0000  ...s....   r....
-00001ee0: 7255 0000 007a 1544 656e 6472 6974 6550  rU...z.DendriteP
-00001ef0: 6167 652e 6765 745f 736f 7570 ba00 0000  age.get_soup....
-00001f00: 7347 0000 00e8 00f8 8000 d80e 12d7 0e28  sG.............(
-00001f10: d10e 28d3 0e2a d708 2ad0 082a d81c 209f  ..(..*..*..*.. .
-00001f20: 4999 49d7 1c2d d11c 2dd3 1c2f d716 2f88  I.I..-..-../../.
-00001f30: 0bdc 0f1c 985b a826 d30f 3188 04d8 0f13  .....[.&..1.....
-00001f40: 880b f007 0009 2bf8 d816 2ffa 731f 0000  ......+.../.s...
-00001f50: 0082 1441 0f01 9601 410b 0497 2141 0f01  ...A....A...!A..
-00001f60: b801 410d 04b9 1341 0f01 c10d 0141 0f01  ..A....A.....A..
-00001f70: 2904 721b 0000 0072 0400 0000 721d 0000  ).r....r....r...
-00001f80: 0072 0f00 0000 2902 da06 7265 7475 726e  .r....)...return
-00001f90: 7204 0000 0029 034e 4e4e 290a 722a 0000  r....).NNN).r*..
-00001fa0: 0072 5700 0000 722b 0000 007a 0d4f 7074  .rW...r+...z.Opt
-00001fb0: 696f 6e61 6c5b 7374 725d 722c 0000 007a  ional[str]r,...z
-00001fc0: 0d4f 7074 696f 6e61 6c5b 416e 795d 7234  .Optional[Any]r4
-00001fd0: 0000 007a 194f 7074 696f 6e61 6c5b 5479  ...z.Optional[Ty
-00001fe0: 7065 5b42 6173 654d 6f64 656c 5d5d 726c  pe[BaseModel]]rl
-00001ff0: 0000 0072 0800 0000 2904 724d 0000 0072  ...r....).rM...r
-00002000: 5700 0000 726c 0000 0072 0500 0000 2902  W...rl...r....).
-00002010: 726c 0000 0072 1300 0000 2902 726c 0000  rl...r....).rl..
-00002020: 00da 044e 6f6e 6529 0272 3c00 0000 e903  ...None).r<.....
-00002030: 0000 0029 0872 2a00 0000 7257 0000 0072  ...).r*...rW...r
-00002040: 4700 0000 da05 666c 6f61 7472 6400 0000  G.....floatrd...
-00002050: da03 696e 7472 6c00 0000 7214 0000 0029  ..intrl...r....)
-00002060: 0272 6c00 0000 7206 0000 0029 0fda 085f  .rl...r....)..._
-00002070: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00002080: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00002090: 5f72 2000 0000 da08 7072 6f70 6572 7479  _r .....property
-000020a0: 7223 0000 0072 2600 0000 7238 0000 0072  r#...r&...r8...r
-000020b0: 4500 0000 7250 0000 0072 3000 0000 7248  E...rP...r0...rH
-000020c0: 0000 0072 5e00 0000 7267 0000 0072 5500  ...r^...rg...rU.
-000020d0: 0000 a900 7221 0000 0072 1f00 0000 7218  ....r!...r....r.
-000020e0: 0000 0072 1800 0000 1d00 0000 73b3 0000  ...r........s...
-000020f0: 0084 00f3 0203 0531 f00a 0006 0ef1 0201  .......1........
-00002100: 051d f303 0006 0ef0 0201 051d f306 0105  ................
-00002110: 19f0 0c00 2f33 d831 35d8 3b3f f00b 1905  ..../3.15.;?....
-00002120: 1de0 1013 f005 1905 1df0 0600 1f2c f007  .............,..
-00002130: 1905 1df0 0800 222f f009 1905 1df0 0a00  ......"/........
-00002140: 2039 f00b 1905 1df0 0c00 0a0d f30d 1905   9..............
-00002150: 1df2 3613 0525 f32a 0905 0ef3 160c 050a  ..6..%.*........
-00002160: f21c 2105 29f3 4601 0105 26f0 0c00 1a1d  ..!.).F...&.....
-00002170: d81b 1cf0 091f 050a e010 13f0 051f 050a  ................
-00002180: f006 0012 17f0 071f 050a f008 0016 19f0  ................
-00002190: 091f 050a f00a 000a 19f3 0b1f 050a f442  ...............B
-000021a0: 0104 0514 7221 0000 0072 1800 0000 2927  ....r!...r....)'
-000021b0: da0a 5f5f 6675 7475 7265 5f5f 7203 0000  ..__future__r...
-000021c0: 0072 3f00 0000 722d 0000 0072 3d00 0000  .r?...r-...r=...
-000021d0: da14 706c 6179 7772 6967 6874 2e61 7379  ..playwright.asy
-000021e0: 6e63 5f61 7069 7204 0000 0072 0500 0000  nc_apir....r....
-000021f0: da03 6273 3472 0600 0000 da06 7479 7069  ..bs4r......typi
-00002200: 6e67 7207 0000 0072 0800 0000 7209 0000  ngr....r....r...
-00002210: 0072 0a00 0000 da08 7079 6461 6e74 6963  .r......pydantic
-00002220: 720b 0000 00da 2564 656e 6472 6974 655f  r.....%dendrite_
-00002230: 7079 7468 6f6e 5f73 646b 2e64 746f 2e53  python_sdk.dto.S
-00002240: 6372 6170 6550 6167 6544 544f 720c 0000  crapePageDTOr...
-00002250: 00da 3064 656e 6472 6974 655f 7079 7468  ..0dendrite_pyth
-00002260: 6f6e 5f73 646b 2e65 7863 6570 7469 6f6e  on_sdk.exception
-00002270: 732e 4465 6e64 7269 7465 4578 6365 7074  s.DendriteExcept
-00002280: 696f 6e72 0d00 0000 da30 6465 6e64 7269  ionr.....0dendri
-00002290: 7465 5f70 7974 686f 6e5f 7364 6b2e 7265  te_python_sdk.re
-000022a0: 7370 6f6e 7365 732e 5363 7261 7065 5061  sponses.ScrapePa
-000022b0: 6765 5265 7370 6f6e 7365 720e 0000 00da  geResponser.....
-000022c0: 1364 656e 6472 6974 655f 7079 7468 6f6e  .dendrite_python
-000022d0: 5f73 646b 720f 0000 00da 3664 656e 6472  _sdkr.....6dendr
-000022e0: 6974 655f 7079 7468 6f6e 5f73 646b 2e64  ite_python_sdk.d
-000022f0: 656e 6472 6974 655f 6272 6f77 7365 722e  endrite_browser.
-00002300: 5363 7265 656e 7368 6f74 4d61 6e61 6765  ScreenshotManage
-00002310: 7272 1000 0000 da2a 6465 6e64 7269 7465  rr.....*dendrite
-00002320: 5f70 7974 686f 6e5f 7364 6b2e 6465 6e64  _python_sdk.dend
-00002330: 7269 7465 5f62 726f 7773 6572 2e75 7469  rite_browser.uti
-00002340: 6c73 7211 0000 00da 2964 656e 6472 6974  lsr.....)dendrit
-00002350: 655f 7079 7468 6f6e 5f73 646b 2e64 746f  e_python_sdk.dto
-00002360: 2e47 6574 496e 7465 7261 6374 696f 6e44  .GetInteractionD
-00002370: 544f 7212 0000 00da 2a64 656e 6472 6974  TOr.....*dendrit
-00002380: 655f 7079 7468 6f6e 5f73 646b 2e6d 6f64  e_python_sdk.mod
-00002390: 656c 732e 5061 6765 496e 666f 726d 6174  els.PageInformat
-000023a0: 696f 6e72 1300 0000 da34 6465 6e64 7269  ionr.....4dendri
-000023b0: 7465 5f70 7974 686f 6e5f 7364 6b2e 6465  te_python_sdk.de
-000023c0: 6e64 7269 7465 5f62 726f 7773 6572 2e44  ndrite_browser.D
-000023d0: 656e 6472 6974 654c 6f63 6174 6f72 7214  endriteLocatorr.
-000023e0: 0000 00da 2364 656e 6472 6974 655f 7079  ....#dendrite_py
-000023f0: 7468 6f6e 5f73 646b 2e72 6571 7565 7374  thon_sdk.request
-00002400: 5f68 616e 646c 6572 7215 0000 0072 1600  _handlerr....r..
-00002410: 0000 7218 0000 0072 7500 0000 7221 0000  ..r....ru...r!..
-00002420: 0072 1f00 0000 fa08 3c6d 6f64 756c 653e  .r......<module>
-00002430: 7285 0000 0001 0000 0073 5200 0000 f003  r........sR.....
-00002440: 0101 01dd 0022 db00 0edb 000b db00 0be7  ....."..........
-00002450: 002e dd00 1de7 0035 d300 35dd 001e e500  .......5..5.....
-00002460: 3fdd 004e dd00 4fe1 0310 dd04 33e5 0054  ?..N..O.....3..T
-00002470: f502 0201 02f5 0600 0148 01dd 0046 dd00  .........H...F..
-00002480: 50df 004c f706 6102 0114 f200 6102 0114  P..L..a.....a...
-00002490: 7221 0000 00                             r!...
+00001990: 0505 007d 087c 0872 407c 0864 0319 0000  ...}.|.r@|.d....
+000019a0: 0064 046b 3700 0072 387c 006a 0b00 0000  .d.k7..r8|.j....
+000019b0: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
+000019c0: 0864 0319 0000 00ab 0100 0000 0000 0083  .d..............
+000019d0: 0064 007b 0300 0096 0297 0386 0505 007d  .d.{...........}
+000019e0: 0974 0d00 0000 0000 0000 007c 0864 0319  .t.........|.d..
+000019f0: 0000 007c 097c 006a 0000 0000 0000 0000  ...|.|.j........
+00001a00: 0000 0000 0000 0000 0000 00ab 0300 0000  ................
+00001a10: 0000 007d 0a7c 0a53 007c 0564 057a 0d00  ...}.|.S.|.d.z..
+00001a20: 007d 0574 0f00 0000 0000 0000 006a 1000  .}.t.........j..
+00001a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a40: 007c 02ab 0100 0000 0000 0083 0064 007b  .|...........d.{
+00001a50: 0300 0096 0297 0386 0505 0001 007c 057c  .............|.|
+00001a60: 036b 0200 0072 018c a37c 006a 0500 0000  .k...r...|.j....
+00001a70: 0000 0000 0000 0000 0000 0000 0000 00ab  ................
+00001a80: 0000 0000 0000 0083 0064 007b 0300 0096  .........d.{....
+00001a90: 0297 0386 0505 007d 0674 1300 0000 0000  .......}.t......
+00001aa0: 0000 0064 067c 066a 1400 0000 0000 0000  ...d.|.j........
+00001ab0: 0000 0000 0000 0000 0000 00ac 07ab 0200  ................
+00001ac0: 0000 0000 0082 0137 008c be37 008c 9f37  .......7...7...7
+00001ad0: 008c 7b37 008c 3f37 008c 23ad 0377 0129  ..{7..?7..#..w.)
+00001ae0: 084e 7202 0000 0029 0372 2800 0000 7229  .Nr....).r(...r)
+00001af0: 0000 0072 2a00 0000 724d 0000 00da 00e9  ...r*...rM......
+00001b00: 0100 0000 7a2c 436f 756c 6420 6e6f 7420  ....z,Could not 
+00001b10: 6669 6e64 2073 7569 7461 626c 6520 656c  find suitable el
+00001b20: 656d 656e 7420 6f6e 2074 6865 2070 6167  ement on the pag
+00001b30: 652e 2902 da07 6d65 7373 6167 6572 5400  e.)...messagerT.
+00001b40: 0000 290b 721d 0000 0072 3100 0000 7230  ..).r....r1...r0
+00001b50: 0000 0072 1200 0000 7215 0000 0072 5000  ...r....r....rP.
+00001b60: 0000 7214 0000 0072 3f00 0000 7240 0000  ..r....r?...r@..
+00001b70: 0072 0d00 0000 7254 0000 0029 0b72 1e00  .r....rT...).r..
+00001b80: 0000 722a 0000 0072 4700 0000 da0b 6d61  ..r*...rG.....ma
+00001b90: 785f 7265 7472 6965 7372 2900 0000 da0c  x_retriesr).....
+00001ba0: 6e75 6d5f 6174 7465 6d70 7473 7228 0000  num_attemptsr(..
+00001bb0: 0072 3600 0000 7237 0000 0072 4900 0000  .r6...r7...rI...
+00001bc0: da10 6465 6e64 7269 7465 5f6c 6f63 6174  ..dendrite_locat
+00001bd0: 6f72 730b 0000 0020 2020 2020 2020 2020  ors....         
+00001be0: 2020 721f 0000 00da 1867 6574 5f69 6e74    r......get_int
+00001bf0: 6572 6163 7461 626c 655f 656c 656d 656e  eractable_elemen
+00001c00: 747a 2544 656e 6472 6974 6550 6167 652e  tz%DendritePage.
+00001c10: 6765 745f 696e 7465 7261 6374 6162 6c65  get_interactable
+00001c20: 5f65 6c65 6d65 6e74 9a00 0000 7315 0100  _element....s...
+00001c30: 00e8 00f8 8000 f00c 0016 1ad7 152a d115  .............*..
+00001c40: 2ad7 1539 d115 39d3 153b 880a e017 1888  *..9..9..;......
+00001c50: 0cd8 0e1a 985b d20e 28d8 2529 d725 3ed1  .....[..(.%).%>.
+00001c60: 253e d325 40d7 1f40 d00c 1ce4 1223 d821  %>.%@..@.....#.!
+00001c70: 31b8 6ad0 5157 f403 0213 0e88 43f4 0800  1.j.QW......C...
+00001c80: 1928 a803 d318 2cd7 122c 8843 d90f 1290  .(....,..,.C....
+00001c90: 7398 3dd1 1729 a852 d217 2fd8 2024 d720  s.=..).R../. $. 
+00001ca0: 41d1 2041 c023 c06d d142 54d3 2055 d71a  A. A.#.m.BT. U..
+00001cb0: 5590 07dc 2332 d814 1798 0dd1 1426 a807  U...#2.......&..
+00001cc0: b014 d731 46d1 3146 f303 0224 12d0 1020  ...1F.1F...$... 
+00001cd0: f006 0018 28d0 1027 d80c 1898 41d1 0c1d  ....(..'....A...
+00001ce0: 884c dc12 1997 2d91 2da0 07d3 1228 d70c  .L....-.-....(..
+00001cf0: 28d0 0c28 f01f 000f 1b98 5bd3 0e28 f022  (..(......[..(."
+00001d00: 0022 26d7 213a d121 3ad3 213c d71b 3cd0  ."&.!:.!:.!<..<.
+00001d10: 0818 dc0e 1fd8 1442 d81e 2ed7 1e40 d11e  .......B.....@..
+00001d20: 40f4 0503 0f0a f000 0309 0af0 2300 2041  @...........#. A
+00001d30: 01f8 f00c 0013 2df8 e01a 55f8 f00c 000d  ......-...U.....
+00001d40: 29f8 e01b 3cfa 735d 0000 0082 3544 0001  )...<.s]....5D..
+00001d50: b701 4336 04b8 2044 0001 c118 0143 3804  ..C6.. D.....C8.
+00001d60: c119 2544 0001 c13e 0143 3a04 c13f 3d44  ..%D...>.C:..?=D
+00001d70: 0001 c23c 0143 3c04 c23d 0944 0001 c307  ...<.C<..=.D....
+00001d80: 1344 0001 c31a 0143 3e04 c31b 1c44 0001  .D.....C>....D..
+00001d90: c338 0144 0001 c33a 0144 0001 c33c 0144  .8.D...:.D...<.D
+00001da0: 0001 c33e 0144 0001 6301 0000 0000 0000  ...>.D..c.......
+00001db0: 0000 0000 0004 0000 0083 0000 01f3 a200  ................
+00001dc0: 0000 4b00 0100 9700 7c00 6a01 0000 0000  ..K.....|.j.....
+00001dd0: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
+00001de0: 0000 0000 0000 8300 6400 7b03 0000 9602  ........d.{.....
+00001df0: 9703 8605 0500 0100 7c00 6a02 0000 0000  ........|.j.....
+00001e00: 0000 0000 0000 0000 0000 0000 0000 6a05  ..............j.
+00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e20: 0000 ab00 0000 0000 0000 8300 6400 7b03  ............d.{.
+00001e30: 0000 9602 9703 8605 0500 7d01 7407 0000  ..........}.t...
+00001e40: 0000 0000 0000 7c01 6401 ab02 0000 0000  ......|.d.......
+00001e50: 0000 7d02 7c02 5300 3700 8c34 3700 8c14  ..}.|.S.7..47...
+00001e60: ad03 7701 2902 4eda 046c 786d 6c29 0472  ..w.).N..lxml).r
+00001e70: 4800 0000 721b 0000 00da 0763 6f6e 7465  H...r......conte
+00001e80: 6e74 7206 0000 0029 0372 1e00 0000 da0b  ntr....).r......
+00001e90: 7061 6765 5f73 6f75 7263 6572 5800 0000  page_sourcerX...
+00001ea0: 7303 0000 0020 2020 721f 0000 0072 5500  s....   r....rU.
+00001eb0: 0000 7a15 4465 6e64 7269 7465 5061 6765  ..z.DendritePage
+00001ec0: 2e67 6574 5f73 6f75 70ba 0000 0073 4700  .get_soup....sG.
+00001ed0: 0000 e800 f880 00d8 0e12 d70e 28d1 0e28  ............(..(
+00001ee0: d30e 2ad7 082a d008 2ad8 1c20 9f49 9949  ..*..*..*.. .I.I
+00001ef0: d71c 2dd1 1c2d d31c 2fd7 162f 880b dc0f  ..-..-../../....
+00001f00: 1c98 5ba8 26d3 0f31 8804 d80f 1388 0bf0  ..[.&..1........
+00001f10: 0700 092b f8d8 162f fa73 1f00 0000 8214  ...+.../.s......
+00001f20: 410f 0196 0141 0b04 9721 410f 01b8 0141  A....A...!A....A
+00001f30: 0d04 b913 410f 01c1 0d01 410f 0129 0472  ....A.....A..).r
+00001f40: 1b00 0000 7204 0000 0072 1d00 0000 720f  ....r....r....r.
+00001f50: 0000 0029 02da 0672 6574 7572 6e72 0400  ...)...returnr..
+00001f60: 0000 2903 4e4e 4e29 0a72 2a00 0000 7257  ..).NNN).r*...rW
+00001f70: 0000 0072 2b00 0000 7a0d 4f70 7469 6f6e  ...r+...z.Option
+00001f80: 616c 5b73 7472 5d72 2c00 0000 7a0d 4f70  al[str]r,...z.Op
+00001f90: 7469 6f6e 616c 5b41 6e79 5d72 3400 0000  tional[Any]r4...
+00001fa0: 7a19 4f70 7469 6f6e 616c 5b54 7970 655b  z.Optional[Type[
+00001fb0: 4261 7365 4d6f 6465 6c5d 5d72 6b00 0000  BaseModel]]rk...
+00001fc0: 7208 0000 0029 0472 4d00 0000 7257 0000  r....).rM...rW..
+00001fd0: 0072 6b00 0000 7205 0000 0029 0272 6b00  .rk...r....).rk.
+00001fe0: 0000 7213 0000 0029 0272 6b00 0000 da04  ..r....).rk.....
+00001ff0: 4e6f 6e65 2902 723c 0000 00e9 0300 0000  None).r<........
+00002000: 2908 722a 0000 0072 5700 0000 7247 0000  ).r*...rW...rG..
+00002010: 00da 0566 6c6f 6174 7263 0000 00da 0369  ...floatrc.....i
+00002020: 6e74 726b 0000 0072 1400 0000 2902 726b  ntrk...r....).rk
+00002030: 0000 0072 0600 0000 290f da08 5f5f 6e61  ...r....)...__na
+00002040: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00002050: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7220  ..__qualname__r 
+00002060: 0000 00da 0870 726f 7065 7274 7972 2300  .....propertyr#.
+00002070: 0000 7226 0000 0072 3800 0000 7245 0000  ..r&...r8...rE..
+00002080: 0072 5000 0000 7230 0000 0072 4800 0000  .rP...r0...rH...
+00002090: 725e 0000 0072 6600 0000 7255 0000 00a9  r^...rf...rU....
+000020a0: 0072 2100 0000 721f 0000 0072 1800 0000  .r!...r....r....
+000020b0: 7218 0000 001d 0000 0073 b300 0000 8400  r........s......
+000020c0: f302 0305 31f0 0a00 060e f102 0105 1df3  ....1...........
+000020d0: 0300 060e f002 0105 1df3 0601 0519 f00c  ................
+000020e0: 002f 33d8 3135 d83b 3ff0 0b19 051d e010  ./3.15.;?.......
+000020f0: 13f0 0519 051d f006 001f 2cf0 0719 051d  ..........,.....
+00002100: f008 0022 2ff0 0919 051d f00a 0020 39f0  ..."/........ 9.
+00002110: 0b19 051d f00c 000a 0df3 0d19 051d f236  ...............6
+00002120: 1405 25f3 2c09 050e f316 0c05 0af2 1c21  ..%.,..........!
+00002130: 0529 f346 0101 0526 f00c 001a 1dd8 1b1c  .).F...&........
+00002140: f009 1e05 0ae0 1013 f005 1e05 0af0 0600  ................
+00002150: 1217 f007 1e05 0af0 0800 1619 f009 1e05  ................
+00002160: 0af0 0a00 0a19 f30b 1e05 0af4 4001 0405  ............@...
+00002170: 1472 2100 0000 7218 0000 0029 27da 0a5f  .r!...r....)'.._
+00002180: 5f66 7574 7572 655f 5f72 0300 0000 723f  _future__r....r?
+00002190: 0000 0072 2d00 0000 723d 0000 00da 1470  ...r-...r=.....p
+000021a0: 6c61 7977 7269 6768 742e 6173 796e 635f  laywright.async_
+000021b0: 6170 6972 0400 0000 7205 0000 00da 0362  apir....r......b
+000021c0: 7334 7206 0000 00da 0674 7970 696e 6772  s4r......typingr
+000021d0: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
+000021e0: 0000 00da 0870 7964 616e 7469 6372 0b00  .....pydanticr..
+000021f0: 0000 da25 6465 6e64 7269 7465 5f70 7974  ...%dendrite_pyt
+00002200: 686f 6e5f 7364 6b2e 6474 6f2e 5363 7261  hon_sdk.dto.Scra
+00002210: 7065 5061 6765 4454 4f72 0c00 0000 da30  pePageDTOr.....0
+00002220: 6465 6e64 7269 7465 5f70 7974 686f 6e5f  dendrite_python_
+00002230: 7364 6b2e 6578 6365 7074 696f 6e73 2e44  sdk.exceptions.D
+00002240: 656e 6472 6974 6545 7863 6570 7469 6f6e  endriteException
+00002250: 720d 0000 00da 3064 656e 6472 6974 655f  r.....0dendrite_
+00002260: 7079 7468 6f6e 5f73 646b 2e72 6573 706f  python_sdk.respo
+00002270: 6e73 6573 2e53 6372 6170 6550 6167 6552  nses.ScrapePageR
+00002280: 6573 706f 6e73 6572 0e00 0000 da13 6465  esponser......de
+00002290: 6e64 7269 7465 5f70 7974 686f 6e5f 7364  ndrite_python_sd
+000022a0: 6b72 0f00 0000 da36 6465 6e64 7269 7465  kr.....6dendrite
+000022b0: 5f70 7974 686f 6e5f 7364 6b2e 6465 6e64  _python_sdk.dend
+000022c0: 7269 7465 5f62 726f 7773 6572 2e53 6372  rite_browser.Scr
+000022d0: 6565 6e73 686f 744d 616e 6167 6572 7210  eenshotManagerr.
+000022e0: 0000 00da 2a64 656e 6472 6974 655f 7079  ....*dendrite_py
+000022f0: 7468 6f6e 5f73 646b 2e64 656e 6472 6974  thon_sdk.dendrit
+00002300: 655f 6272 6f77 7365 722e 7574 696c 7372  e_browser.utilsr
+00002310: 1100 0000 da29 6465 6e64 7269 7465 5f70  .....)dendrite_p
+00002320: 7974 686f 6e5f 7364 6b2e 6474 6f2e 4765  ython_sdk.dto.Ge
+00002330: 7449 6e74 6572 6163 7469 6f6e 4454 4f72  tInteractionDTOr
+00002340: 1200 0000 da2a 6465 6e64 7269 7465 5f70  .....*dendrite_p
+00002350: 7974 686f 6e5f 7364 6b2e 6d6f 6465 6c73  ython_sdk.models
+00002360: 2e50 6167 6549 6e66 6f72 6d61 7469 6f6e  .PageInformation
+00002370: 7213 0000 00da 3464 656e 6472 6974 655f  r.....4dendrite_
+00002380: 7079 7468 6f6e 5f73 646b 2e64 656e 6472  python_sdk.dendr
+00002390: 6974 655f 6272 6f77 7365 722e 4465 6e64  ite_browser.Dend
+000023a0: 7269 7465 4c6f 6361 746f 7272 1400 0000  riteLocatorr....
+000023b0: da23 6465 6e64 7269 7465 5f70 7974 686f  .#dendrite_pytho
+000023c0: 6e5f 7364 6b2e 7265 7175 6573 745f 6861  n_sdk.request_ha
+000023d0: 6e64 6c65 7272 1500 0000 7216 0000 0072  ndlerr....r....r
+000023e0: 1800 0000 7274 0000 0072 2100 0000 721f  ....rt...r!...r.
+000023f0: 0000 00fa 083c 6d6f 6475 6c65 3e72 8400  .....<module>r..
+00002400: 0000 0100 0000 7352 0000 00f0 0301 0101  ......sR........
+00002410: dd00 22db 000e db00 0bdb 000b e700 2edd  ..".............
+00002420: 001d e700 35d3 0035 dd00 1ee5 003f dd00  ....5..5.....?..
+00002430: 4edd 004f e103 10dd 0433 e500 54f5 0202  N..O.....3..T...
+00002440: 0102 f506 0001 4801 dd00 46dd 0050 df00  ......H...F..P..
+00002450: 4cf7 0661 0201 14f2 0061 0201 1472 2100  L..a.....a...r!.
+00002460: 0000                                     ..
```

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/ScreenshotManager.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/ScreenshotManager.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/utils.cpython-310.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/utils.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/__pycache__/utils.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/utils.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dendrite_browser/utils.py`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/GetInteractionDTO.cpython-310.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/GetInteractionDTO.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/GetInteractionDTO.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/GetInteractionDTO.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/GoogleSearchDTO.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/GoogleSearchDTO.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/MakeInteractionDTO.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/MakeInteractionDTO.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/PageInformation.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/PageInformation.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/PageInformationDTO.cpython-310.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/PageInformationDTO.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/PageInformationDTO.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/PageInformationDTO.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/ScrapePageDTO.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/dto/__pycache__/ScrapePageDTO.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/__pycache__/agent.cpython-310.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/examples/__pycache__/agent.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/get_steam_reviews.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/examples/get_steam_reviews.py`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/review_sentiment.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/examples/review_sentiment.py`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/send_discord_message.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/examples/send_discord_message.py`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/simple_example.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/examples/simple_example.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,23 +3,37 @@
 import asyncio
 from dotenv import load_dotenv, find_dotenv
 
 load_dotenv(find_dotenv())
 
 
 async def main():
+    # Launch browser locally
     dendrite_browser = DendriteBrowser(
         openai_api_key=os.environ.get("OPENAI_API_KEY", "")
     )
+
+    # Go to google.com
     page = await dendrite_browser.goto("https://google.com")
+
+    # Get the reject cookies button
     close_cookies = await page.get_interactable_element("reject cookies popup button")
+
+    # Click the button, returns IncorrectOutcomeException if the popup wasn't closed
     await close_cookies.click(expected_outcome="That the cookies popup closed.")
+
+    # Get the search bar
     search_bar = await page.get_interactable_element("Return the search bar")
+
+    # Enter "hello world" into it.
     await search_bar.fill(
         "hello world", expected_outcome="The words 'hello world' to have been entered"
     )
+
+    # Use the Playwright page to press enter.
     await page.get_playwright_page().keyboard.press("Enter")
+
     await asyncio.sleep(2)
     await dendrite_browser.close()
 
 
 asyncio.run(main())
```

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/yc.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/examples/yc.py`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/DendriteException.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/exceptions/DendriteException.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def store_exception_screenshot(self, path: str, name: str = "") -> str:
         if not name:
             name = str(uuid4())
 
         # Create the full file path
         filepath = os.path.join(path, f"{name}.png")
 
-        print("filepath: ", filepath)
+        # print("filepath: ", filepath)
 
         # Ensure the directory exists
         os.makedirs(os.path.dirname(filepath), exist_ok=True)
 
         # Decode the Base64 string
         screenshot_data = base64.b64decode(self._screenshot_base64)
```

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/__pycache__/DendriteException.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/exceptions/__pycache__/DendriteException.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Fri May 17 11:21:44 2024 UTC, .py size: 1244 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 c83d 4766 dc04 0000  .........=Gf....
+00000000: cb0d 0d0a 0000 0000 5e8a 5566 de04 0000  ........^.Uf....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 00f3 4200 0000 9700 6400 6401  ......B.....d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6402  l.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 0100 6400 6403 6c04 6d05  l.m.Z...d.d.l.m.
 00000050: 5a05 0100 0200 4700 6404 8400 6405 6506  Z.....G.d...d.e.
 00000060: ab03 0000 0000 0000 5a07 7901 2906 e900  ........Z.y.)...
 00000070: 0000 004e 2901 da08 4f70 7469 6f6e 616c  ...N)...Optional
@@ -71,88 +71,85 @@
 00000460: 0072 0b00 0000 2901 720f 0000 0072 1700  .r....).r....r..
 00000470: 0000 7301 0000 0020 7214 0000 00da 0573  ..s.... r......s
 00000480: 7461 636b 7a17 4465 6e64 7269 7465 4578  tackz.DendriteEx
 00000490: 6365 7074 696f 6e2e 7374 6163 6b17 0000  ception.stack...
 000004a0: 0073 0c00 0000 8000 e00f 138f 7b89 7bd0  .s..........{.{.
 000004b0: 081a 7215 0000 00da 0470 6174 6872 1900  ..r......pathr..
 000004c0: 0000 6303 0000 0000 0000 0000 0000 0006  ..c.............
-000004d0: 0000 0003 0000 00f3 9a01 0000 9700 7c02  ..............|.
+000004d0: 0000 0003 0000 00f3 8201 0000 9700 7c02  ..............|.
 000004e0: 7313 7401 0000 0000 0000 0000 7403 0000  s.t.........t...
 000004f0: 0000 0000 0000 ab00 0000 0000 0000 ab01  ................
 00000500: 0000 0000 0000 7d02 7404 0000 0000 0000  ......}.t.......
 00000510: 0000 6a06 0000 0000 0000 0000 0000 0000  ..j.............
 00000520: 0000 0000 0000 6a09 0000 0000 0000 0000  ......j.........
 00000530: 0000 0000 0000 0000 0000 7c01 7c02 9b00  ..........|.|...
-00000540: 6401 9d02 ab02 0000 0000 0000 7d03 740b  d...........}.t.
-00000550: 0000 0000 0000 0000 6402 7c03 ab02 0000  ........d.|.....
-00000560: 0000 0000 0100 7405 0000 0000 0000 0000  ......t.........
-00000570: 6a0c 0000 0000 0000 0000 0000 0000 0000  j...............
-00000580: 0000 0000 7404 0000 0000 0000 0000 6a06  ....t.........j.
-00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005a0: 0000 6a0f 0000 0000 0000 0000 0000 0000  ..j.............
-000005b0: 0000 0000 0000 7c03 ab01 0000 0000 0000  ......|.........
-000005c0: 6403 ac04 ab02 0000 0000 0000 0100 7411  d.............t.
-000005d0: 0000 0000 0000 0000 6a12 0000 0000 0000  ........j.......
-000005e0: 0000 0000 0000 0000 0000 0000 7c00 6a14  ............|.j.
-000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000600: 0000 ab01 0000 0000 0000 7d04 7417 0000  ..........}.t...
-00000610: 0000 0000 0000 7c03 6405 ab02 0000 0000  ......|.d.......
-00000620: 0000 3500 7d05 7c05 6a19 0000 0000 0000  ..5.}.|.j.......
-00000630: 0000 0000 0000 0000 0000 0000 7c04 ab01  ............|...
-00000640: 0000 0000 0000 0100 6400 6400 6400 ab02  ........d.d.d...
-00000650: 0000 0000 0000 0100 7c03 5300 2300 3100  ........|.S.#.1.
-00000660: 7301 7702 0100 5900 0100 0100 7c03 5300  s.w...Y.....|.S.
-00000670: 7803 5900 7701 2906 4e7a 042e 706e 677a  x.Y.w.).Nz..pngz
-00000680: 0a66 696c 6570 6174 683a 2054 2901 da08  .filepath: T)...
-00000690: 6578 6973 745f 6f6b da02 7762 290d da03  exist_ok..wb)...
-000006a0: 7374 7272 0400 0000 da02 6f73 721c 0000  strr......osr...
-000006b0: 00da 046a 6f69 6eda 0570 7269 6e74 da08  ...join..print..
-000006c0: 6d61 6b65 6469 7273 da07 6469 726e 616d  makedirs..dirnam
-000006d0: 65da 0662 6173 6536 34da 0962 3634 6465  e..base64..b64de
-000006e0: 636f 6465 720d 0000 00da 046f 7065 6eda  coder......open.
-000006f0: 0577 7269 7465 2906 7212 0000 0072 1c00  .write).r....r..
-00000700: 0000 7219 0000 00da 0866 696c 6570 6174  ..r......filepat
-00000710: 68da 0f73 6372 6565 6e73 686f 745f 6461  h..screenshot_da
-00000720: 7461 da04 6669 6c65 7306 0000 0020 2020  ta..files....   
-00000730: 2020 2072 1400 0000 da1a 7374 6f72 655f     r......store_
-00000740: 6578 6365 7074 696f 6e5f 7363 7265 656e  exception_screen
-00000750: 7368 6f74 7a2c 4465 6e64 7269 7465 4578  shotz,DendriteEx
-00000760: 6365 7074 696f 6e2e 7374 6f72 655f 6578  ception.store_ex
-00000770: 6365 7074 696f 6e5f 7363 7265 656e 7368  ception_screensh
-00000780: 6f74 1b00 0000 73a3 0000 0080 00d9 0f13  ot....s.........
-00000790: dc13 1694 7593 7793 3c88 44f4 0600 1416  ....u.w.<.D.....
-000007a0: 9737 9137 973c 913c a004 a814 a806 a864  .7.7.<.<.......d
-000007b0: a06d d313 3488 08e4 080d 886c 9848 d408  .m..4......l.H..
-000007c0: 25f4 0600 090b 8f0b 890b 9442 9747 9147  %..........B.G.G
-000007d0: 974f 914f a048 d314 2db8 04d5 083d f406  .O.O.H..-....=..
-000007e0: 001b 21d7 1a2a d11a 2aa8 34d7 2b42 d12b  ..!..*..*.4.+B.+
-000007f0: 42d3 1a43 880f f406 000e 1290 2898 44d3  B..C........(.D.
-00000800: 0d21 f000 0109 28a0 54d8 0c10 8f4a 894a  .!....(.T....J.J
-00000810: 907f d40c 27f7 0301 0928 f006 0010 1888  ....'....(......
-00000820: 0ff7 0701 0928 f006 0010 1888 0ffa 730c  .....(........s.
-00000830: 0000 00c2 2412 4300 03c3 0005 430a 0729  ....$.C.....C..)
-00000840: 01da 0029 0cda 085f 5f6e 616d 655f 5fda  ...)...__name__.
-00000850: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000860: 7561 6c6e 616d 655f 5f72 2000 0000 7211  ualname__r ...r.
-00000870: 0000 00da 0870 726f 7065 7274 7972 0700  .....propertyr..
-00000880: 0000 7203 0000 0072 1900 0000 721b 0000  ..r....r....r...
-00000890: 0072 2d00 0000 da0d 5f5f 636c 6173 7363  .r-.....__classc
-000008a0: 656c 6c5f 5f29 0172 1300 0000 7301 0000  ell__).r....s...
-000008b0: 0040 7214 0000 0072 0600 0000 7206 0000  .@r....r....r...
-000008c0: 0007 0000 0073 9000 0000 f884 00f0 0205  .....s..........
-000008d0: 0522 a003 f000 0505 22b8 03f0 0005 0522  ."......"......"
-000008e0: c004 f500 0505 22f0 0e00 060e f002 0105  ......".........
-000008f0: 1d98 13f2 0001 051d f303 0006 0ef0 0201  ................
-00000900: 051d f006 0006 0ef0 0201 051a 9068 9873  .............h.s
-00000910: 916d f200 0105 1af3 0300 060e f002 0105  .m..............
-00000920: 1af0 0600 060e f002 0105 1b90 78a0 0391  ............x...
-00000930: 7df2 0001 051b f303 0006 0ef0 0201 051b  }...............
-00000940: f106 1305 18a8 73f0 0013 0518 b823 f000  ......s......#..
-00000950: 1305 18c0 73f7 0013 0518 7215 0000 0072  ....s.....r....r
-00000960: 0600 0000 2908 7226 0000 0072 2100 0000  ....).r&...r!...
-00000970: da06 7479 7069 6e67 7203 0000 00da 0475  ..typingr......u
-00000980: 7569 6472 0400 0000 da09 4578 6365 7074  uidr......Except
-00000990: 696f 6e72 0600 0000 a900 7215 0000 0072  ionr......r....r
-000009a0: 1400 0000 fa08 3c6d 6f64 756c 653e 7238  ......<module>r8
-000009b0: 0000 0001 0000 0073 1d00 0000 f003 0101  .......s........
-000009c0: 01db 000d db00 09dd 001b dd00 16f4 0627  ...............'
-000009d0: 0118 9809 f500 2701 1872 1500 0000       ......'..r....
+00000540: 6401 9d02 ab02 0000 0000 0000 7d03 7405  d...........}.t.
+00000550: 0000 0000 0000 0000 6a0a 0000 0000 0000  ........j.......
+00000560: 0000 0000 0000 0000 0000 0000 7404 0000  ............t...
+00000570: 0000 0000 0000 6a06 0000 0000 0000 0000  ......j.........
+00000580: 0000 0000 0000 0000 0000 6a0d 0000 0000  ..........j.....
+00000590: 0000 0000 0000 0000 0000 0000 0000 7c03  ..............|.
+000005a0: ab01 0000 0000 0000 6402 ac03 ab02 0000  ........d.......
+000005b0: 0000 0000 0100 740f 0000 0000 0000 0000  ......t.........
+000005c0: 6a10 0000 0000 0000 0000 0000 0000 0000  j...............
+000005d0: 0000 0000 7c00 6a12 0000 0000 0000 0000  ....|.j.........
+000005e0: 0000 0000 0000 0000 0000 ab01 0000 0000  ................
+000005f0: 0000 7d04 7415 0000 0000 0000 0000 7c03  ..}.t.........|.
+00000600: 6404 ab02 0000 0000 0000 3500 7d05 7c05  d.........5.}.|.
+00000610: 6a17 0000 0000 0000 0000 0000 0000 0000  j...............
+00000620: 0000 0000 7c04 ab01 0000 0000 0000 0100  ....|...........
+00000630: 6400 6400 6400 ab02 0000 0000 0000 0100  d.d.d...........
+00000640: 7c03 5300 2300 3100 7301 7702 0100 5900  |.S.#.1.s.w...Y.
+00000650: 0100 0100 7c03 5300 7803 5900 7701 2905  ....|.S.x.Y.w.).
+00000660: 4e7a 042e 706e 6754 2901 da08 6578 6973  Nz..pngT)...exis
+00000670: 745f 6f6b da02 7762 290c da03 7374 7272  t_ok..wb)...strr
+00000680: 0400 0000 da02 6f73 721c 0000 00da 046a  ......osr......j
+00000690: 6f69 6eda 086d 616b 6564 6972 73da 0764  oin..makedirs..d
+000006a0: 6972 6e61 6d65 da06 6261 7365 3634 da09  irname..base64..
+000006b0: 6236 3464 6563 6f64 6572 0d00 0000 da04  b64decoder......
+000006c0: 6f70 656e da05 7772 6974 6529 0672 1200  open..write).r..
+000006d0: 0000 721c 0000 0072 1900 0000 da08 6669  ..r....r......fi
+000006e0: 6c65 7061 7468 da0f 7363 7265 656e 7368  lepath..screensh
+000006f0: 6f74 5f64 6174 61da 0466 696c 6573 0600  ot_data..files..
+00000700: 0000 2020 2020 2020 7214 0000 00da 1a73  ..      r......s
+00000710: 746f 7265 5f65 7863 6570 7469 6f6e 5f73  tore_exception_s
+00000720: 6372 6565 6e73 686f 747a 2c44 656e 6472  creenshotz,Dendr
+00000730: 6974 6545 7863 6570 7469 6f6e 2e73 746f  iteException.sto
+00000740: 7265 5f65 7863 6570 7469 6f6e 5f73 6372  re_exception_scr
+00000750: 6565 6e73 686f 741b 0000 0073 9900 0000  eenshot....s....
+00000760: 8000 d90f 13dc 1316 9475 9377 933c 8844  .........u.w.<.D
+00000770: f406 0014 1697 3791 3797 3c91 3ca0 04a8  ......7.7.<.<...
+00000780: 14a8 06a8 64a0 6dd3 1334 8808 f40a 0009  ....d.m..4......
+00000790: 0b8f 0b89 0b94 4297 4791 4797 4f91 4fa0  ......B.G.G.O.O.
+000007a0: 48d3 142d b804 d508 3df4 0600 1b21 d71a  H..-....=....!..
+000007b0: 2ad1 1a2a a834 d72b 42d1 2b42 d31a 4388  *..*.4.+B.+B..C.
+000007c0: 0ff4 0600 0e12 9028 9844 d30d 21f0 0001  .......(.D..!...
+000007d0: 0928 a054 d80c 108f 4a89 4a90 7fd4 0c27  .(.T....J.J....'
+000007e0: f703 0109 28f0 0600 1018 880f f707 0109  ....(...........
+000007f0: 28f0 0600 1018 880f fa73 0c00 0000 c218  (........s......
+00000800: 1242 3403 c234 0542 3e07 2901 da00 290c  .B4..4.B>.)...).
+00000810: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000820: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000830: 6d65 5f5f 7220 0000 0072 1100 0000 da08  me__r ...r......
+00000840: 7072 6f70 6572 7479 7207 0000 0072 0300  propertyr....r..
+00000850: 0000 7219 0000 0072 1b00 0000 722c 0000  ..r....r....r,..
+00000860: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00000870: 2901 7213 0000 0073 0100 0000 4072 1400  ).r....s....@r..
+00000880: 0000 7206 0000 0072 0600 0000 0700 0000  ..r....r........
+00000890: 7390 0000 00f8 8400 f002 0505 22a0 03f0  s..........."...
+000008a0: 0005 0522 b803 f000 0505 22c0 04f5 0005  ..."......".....
+000008b0: 0522 f00e 0006 0ef0 0201 051d 9813 f200  ."..............
+000008c0: 0105 1df3 0300 060e f002 0105 1df0 0600  ................
+000008d0: 060e f002 0105 1a90 6898 7391 6df2 0001  ........h.s.m...
+000008e0: 051a f303 0006 0ef0 0201 051a f006 0006  ................
+000008f0: 0ef0 0201 051b 9078 a003 917d f200 0105  .......x...}....
+00000900: 1bf3 0300 060e f002 0105 1bf1 0613 0518  ................
+00000910: a873 f000 1305 18b8 23f0 0013 0518 c073  .s......#......s
+00000920: f700 1305 1872 1500 0000 7206 0000 0029  .....r....r....)
+00000930: 0872 2500 0000 7221 0000 00da 0674 7970  .r%...r!.....typ
+00000940: 696e 6772 0300 0000 da04 7575 6964 7204  ingr......uuidr.
+00000950: 0000 00da 0945 7863 6570 7469 6f6e 7206  .....Exceptionr.
+00000960: 0000 00a9 0072 1500 0000 7214 0000 00fa  .....r....r.....
+00000970: 083c 6d6f 6475 6c65 3e72 3700 0000 0100  .<module>r7.....
+00000980: 0000 731d 0000 00f0 0301 0101 db00 0ddb  ..s.............
+00000990: 0009 dd00 1bdd 0016 f406 2701 1898 09f5  ..........'.....
+000009a0: 0027 0118 7215 0000 00                   .'..r....
```

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/__pycache__/PageDeltaInformation.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/models/__pycache__/PageDeltaInformation.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/__pycache__/PageInformation.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/models/__pycache__/PageInformation.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/request_handler.py` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/request_handler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 import json
 import sys
 import httpx
-from dendrite_python_sdk.dto.MakeInteractionDTO import (
-    MakeInteractionDTO,
-)
+from dendrite_python_sdk.dto.MakeInteractionDTO import MakeInteractionDTO
 from dendrite_python_sdk.dto.GetInteractionDTO import GetInteractionDTO
 from dendrite_python_sdk.dto.ScrapePageDTO import ScrapePageDTO
 from dendrite_python_sdk.dto.GoogleSearchDTO import GoogleSearchDTO
 from dendrite_python_sdk.responses.GoogleSearchResponse import GoogleSearchResponse
 from dendrite_python_sdk.responses.InteractionResponse import InteractionResponse
 from dendrite_python_sdk.responses.ScrapePageResponse import ScrapePageResponse
-from dendrite_python_sdk.responses.ScrapePageResponse import ScrapePageResponse
 
 config = {"dendrite_api_key": ""}
 dev_mode = True if "--dev" in sys.argv else False
 
 
 async def send_request(
-    endpoint,
-    params=None,
-    data: dict | None = None,
-    headers=None,
-    method="GET",
+    endpoint, params=None, data: dict | None = None, headers=None, method="GET"
 ):
     base_url = (
         "http://localhost:8000/api/v1"
         if dev_mode
         else "https://dendrite-server.azurewebsites.net/api/v1"
     )
     url = f"{base_url}/{endpoint}"
     headers = headers or {}
     headers["Content-Type"] = "application/json"
     if config["dendrite_api_key"] != "":
         headers["Authorization"] = f"Bearer {config['dendrite_api_key']}"
 
     async with httpx.AsyncClient(timeout=300) as client:
-        response = await client.request(
-            method, url, params=params, json=data, headers=headers
-        )
-        response.raise_for_status()
-        return response.json()
+        try:
+            response = await client.request(
+                method, url, params=params, json=data, headers=headers
+            )
+            response.raise_for_status()
+            return response.json()
+        except httpx.HTTPStatusError as http_err:
+            detail = http_err.response.json()
+            print(
+                f"HTTP error occurred: {http_err.response.status_code}: {detail['detail']}"
+            )
+            raise http_err
+        except httpx.RequestError as req_err:
+            print(f"Request error occurred: {req_err}")
+            raise req_err
+        except Exception as err:
+            print(f"An error occurred: {err}")
+            raise err
 
 
 async def get_interaction(dto: GetInteractionDTO) -> dict:
     res = await send_request("actions/get-interaction", data=dto.dict(), method="POST")
     return res
```

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__pycache__/GoogleSearchResponse.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/responses/__pycache__/GoogleSearchResponse.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__pycache__/InteractionResponse.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/responses/__pycache__/InteractionResponse.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__pycache__/ScrapePageResponse.cpython-312.pyc` & `dendrite_python_sdk-1.0.1/dendrite_python_sdk/responses/__pycache__/ScrapePageResponse.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-1.0.0/pyproject.toml` & `dendrite_python_sdk-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dendrite-python-sdk"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["Charles Maddock <charles@dendrite.se>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 requests = "^2.31.0"
```

### Comparing `dendrite_python_sdk-1.0.0/PKG-INFO` & `dendrite_python_sdk-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dendrite-python-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: Charles Maddock
 Author-email: charles@dendrite.se
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
@@ -17,45 +17,66 @@
 Requires-Dist: pydantic (>=2.6.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Dendrite
 
-Dendrite is a developer tool that makes it very easy to interact with and scrape websites using AI.
+Dendrite is an SDK that makes it easy to interact with and scrape websites using prompts.
 
-This project is still in it's infancy and is susceptible to many changes in the coming weeks. 
+```python
+# Extracting data from a page is as simple as doing page.scrape(prompt)
+startup_urls = await page.scrape("Extract a list of valid urls for each listed startup's YC page")
+```
 
-If you want to chat with us developers, give feedback and report bugs, our discord is the place to be! [Invite link](https://discord.gg/ETPBdXU3kx)
+Join our discord to give feedback and report bugs! [Invite link](https://discord.gg/ETPBdXU3kx)
 
 
 ## Installation:
 
 ```
 pip install dendrite-python-sdk && playwright install
 ```
 
 ## Quick start:
 
-Here is a very simple example of how to use Dendrite. In the example we go to google.com, close the cookie popup, find the search bar and enter 'hello world' into it.
+Here is a very simple example of how to use Dendrite.
 
-To do this we install dendrite and asyncio like so: `pip install asyncio dendrite-python-sdk && playwright install` and we then create a file called `main.py` which we can run with `python main.py` from the terminal.
+Install dendrite and asyncio like so: `pip install asyncio dendrite-python-sdk && playwright install` and create a file called `main.py`. Use the code below and run it with `python main.py` from the terminal.
 
 `main.py`
 ```python
 from dendrite_python_sdk import DendriteBrowser
 import asyncio
 
 async def main():
-    dendrite_browser = DendriteBrowser(openai_api_key=...) # Use your own OpenAI API key here
+    # Launch browser locally
+    dendrite_browser = DendriteBrowser(openai_api_key=...) # Use your OpenAI key here
+
+    # Go to google.com
     page = await dendrite_browser.goto("https://google.com")
+
+    # Get the reject cookies button
     close_cookies = await page.get_interactable_element("reject cookies popup button")
+
+    # Click the button, returns IncorrectOutcomeException if the popup wasn't closed
     await close_cookies.click(expected_outcome="That the cookies popup closed.")
+
+    # Get the search bar
     search_bar = await page.get_interactable_element("Return the search bar")
-    await search_bar.fill("hello world")
+
+    # Enter "hello world" into it.
+    await search_bar.fill(
+        "hello world", expected_outcome="The words 'hello world' to have been entered"
+    )
+
+    # Use the Playwright page to press enter.
+    await page.get_playwright_page().keyboard.press("Enter")
+
+    await asyncio.sleep(2)
     await dendrite_browser.close()
 
 
 asyncio.run(main())
 ```
 
 ## More Advanced Example:
```

