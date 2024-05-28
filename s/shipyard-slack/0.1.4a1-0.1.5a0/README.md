# Comparing `tmp/shipyard_slack-0.1.4a1.tar.gz` & `tmp/shipyard_slack-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_slack-0.1.4a1.tar", max compression
+gzip compressed data, was "shipyard_slack-0.1.5a0.tar", max compression
```

## Comparing `shipyard_slack-0.1.4a1.tar` & `shipyard_slack-0.1.5a0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.842181 shipyard_slack-0.1.4a1/README.md
--rw-r--r--   0        0        0      494 2024-04-02 03:18:14.819226 shipyard_slack-0.1.4a1/pyproject.toml
--rw-r--r--   0        0        0       31 2023-05-12 18:48:21.842512 shipyard_slack-0.1.4a1/shipyard_slack/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.764117 shipyard_slack-0.1.4a1/shipyard_slack/cli/__init__.py
--rw-r--r--   0        0        0      182 2024-01-11 03:34:57.764385 shipyard_slack-0.1.4a1/shipyard_slack/cli/authtest.py
--rw-r--r--   0        0        0     7054 2024-04-02 02:35:20.023020 shipyard_slack-0.1.4a1/shipyard_slack/cli/send_conditional_message.py
--rw-r--r--   0        0        0     4564 2024-04-02 02:35:20.034021 shipyard_slack-0.1.4a1/shipyard_slack/cli/send_message.py
--rw-r--r--   0        0        0     5384 2024-04-02 03:18:00.189089 shipyard_slack-0.1.4a1/shipyard_slack/cli/send_message_with_file.py
--rw-r--r--   0        0        0    10409 2024-03-06 20:41:14.967938 shipyard_slack-0.1.4a1/shipyard_slack/slack.py
--rw-r--r--   0        0        0     5860 2024-02-19 16:47:11.187471 shipyard_slack-0.1.4a1/shipyard_slack/slack_utils.py
--rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 shipyard_slack-0.1.4a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.842181 shipyard_slack-0.1.5a0/README.md
+-rw-r--r--   0        0        0      578 2024-05-28 20:33:35.928417 shipyard_slack-0.1.5a0/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-05-12 18:48:21.842512 shipyard_slack-0.1.5a0/shipyard_slack/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.764117 shipyard_slack-0.1.5a0/shipyard_slack/cli/__init__.py
+-rw-r--r--   0        0        0      182 2024-05-20 15:32:22.130853 shipyard_slack-0.1.5a0/shipyard_slack/cli/authtest.py
+-rw-r--r--   0        0        0     4873 2024-05-28 20:27:01.185961 shipyard_slack-0.1.5a0/shipyard_slack/cli/johnathanrodriguez-artifacts/slack-blueprints/responses/send_message_with_file.json
+-rw-r--r--   0        0        0     7054 2024-04-18 20:05:24.213000 shipyard_slack-0.1.5a0/shipyard_slack/cli/send_conditional_message.py
+-rw-r--r--   0        0        0     4564 2024-04-18 20:05:24.213294 shipyard_slack-0.1.5a0/shipyard_slack/cli/send_message.py
+-rw-r--r--   0        0        0     5384 2024-05-28 20:27:50.647863 shipyard_slack-0.1.5a0/shipyard_slack/cli/send_message_with_file.py
+-rw-r--r--   0        0        0    10654 2024-05-28 20:36:29.109483 shipyard_slack-0.1.5a0/shipyard_slack/slack.py
+-rw-r--r--   0        0        0     5884 2024-05-28 20:24:11.442020 shipyard_slack-0.1.5a0/shipyard_slack/slack_utils.py
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 shipyard_slack-0.1.5a0/PKG-INFO
```

### Comparing `shipyard_slack-0.1.4a1/shipyard_slack/cli/send_conditional_message.py` & `shipyard_slack-0.1.5a0/shipyard_slack/cli/send_conditional_message.py`

 * *Files identical despite different names*

### Comparing `shipyard_slack-0.1.4a1/shipyard_slack/cli/send_message.py` & `shipyard_slack-0.1.5a0/shipyard_slack/cli/send_message.py`

 * *Files identical despite different names*

### Comparing `shipyard_slack-0.1.4a1/shipyard_slack/cli/send_message_with_file.py` & `shipyard_slack-0.1.5a0/shipyard_slack/cli/send_message_with_file.py`

 * *Files identical despite different names*

### Comparing `shipyard_slack-0.1.4a1/shipyard_slack/slack.py` & `shipyard_slack-0.1.5a0/shipyard_slack/slack.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from typing import Any, Optional, Dict
+from typing import Optional, Dict
+
+from shipyard_templates import Messaging, ShipyardLogger, ExitCodeException
 from slack_sdk import WebClient
-from slack_sdk.web import SlackResponse
 from slack_sdk.errors import SlackApiError
+from slack_sdk.web import SlackResponse
+
 from shipyard_slack.slack_utils import _create_blocks
-from shipyard_templates import Messaging, ShipyardLogger, ExitCodeException
 
 logger = ShipyardLogger().get_logger()
 
 
 class SlackClient(Messaging):
     """
     A client for interacting with Slack using the Slack SDK, providing functionalities such as sending messages,
@@ -25,14 +27,19 @@
 
         Args:
             slack_token (str): The token used for authenticating with the Slack API.
         """
         self.slack_token = slack_token
         self.web_client = WebClient(token=self.slack_token, timeout=self.TIMEOUT)
 
+        from slack_sdk.http_retry.builtin_handlers import RateLimitErrorRetryHandler
+        rate_limit_handler = RateLimitErrorRetryHandler(max_retry_count=1)
+
+        self.web_client.retry_handlers.append(rate_limit_handler)
+
     def _handle_slack_error(self, slack_error: SlackApiError) -> None:
         """
         Handles errors returned by the Slack API.
 
         Args:
             slack_error (SlackApiError): The error raised by a Slack API call.
 
@@ -80,15 +87,15 @@
                     f"Failed to validate credentials. Response from Slack servers: {e}"
                 )
             return 1
         else:
             return 0
 
     def send_message(
-        self, message: str, channel_name: str, download_link: str = ""
+            self, message: str, channel_name: str, download_link: str = ""
     ) -> SlackResponse:
         """
         Sends a message to a specified Slack channel.
 
         Args:
         message (str): The message content to send.
         channel_name (str): The name of the channel to send the message to.
@@ -216,15 +223,15 @@
                 f"User {display_name} not found", self.EXIT_CODE_USER_NOT_FOUND
             )
 
         except SlackApiError as e:
             self._handle_slack_error(e)
 
     def update_message(
-        self, message: str, channel_id: str, timestamp: str, download_link: str = ""
+            self, message: str, channel_id: str, timestamp: str, download_link: str = ""
     ) -> SlackResponse:
         """
         Updates a previously sent Slack message.
 
         Args:
             message (str): The new message content to update.
             channel_id (str): The channel ID where the message was originally sent.
@@ -248,30 +255,30 @@
             )
             logger.debug("Your message was updated")
             return response
         except SlackApiError as e:
             self._handle_slack_error(e)
 
     def upload_file(
-        self, filename: str, channels: str, thread_ts: Optional[str] = None
+            self, filename: str, channels: str, thread_ts: Optional[str] = None
     ) -> SlackResponse:
         """
         Uploads a file to a Slack channel, optionally in a thread.
 
         Args:
             filename (str): The path to the file to upload.
             channels (str): The channel IDs where the file should be uploaded, separated by commas.
             thread_ts (Optional[str]): The thread timestamp to upload the file into, if any.
 
         Returns:
         SlackResponse: The response from the Slack API after uploading the file.
         """
         logger.debug(f"Attempting to upload file {filename} to Slack...")
         try:
+            message_args = {"file": filename, "channels": channels}
             if thread_ts:
-                return self.web_client.files_upload(
-                    file=filename, channels=channels, thread_ts=thread_ts
-                )
-            else:
-                return self.web_client.files_upload(file=filename, channels=channels)
+                message_args[thread_ts] = thread_ts
+            logger.debug(f"Uploading file to channel(s) {channels}")
+            return self.web_client.files_upload_v2(**message_args)
+
         except SlackApiError as e:
             self._handle_slack_error(e)
```

### Comparing `shipyard_slack-0.1.4a1/shipyard_slack/slack_utils.py` & `shipyard_slack-0.1.5a0/shipyard_slack/slack_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,17 @@
 
     Returns:
         SlackResponse: The response from the Slack API after sending the message and file.
     """
     logger.debug(f"Attempting to send message with file to {channel}...")
     if not include_in_thread:
         logger.debug("Sending message without file in thread...")
-        slack_client.send_message(message, channel)
-        return slack_client.upload_file(file, channel)
+        response = slack_client.send_message(message, channel)
+
+        return slack_client.upload_file(file, response["channel"])
 
     logger.debug("Sending message with file in thread...")
     message_with_file_status = message + "\n\n _(File is currently uploading...)_"
     response = slack_client.send_message(message_with_file_status, channel)
     channel_id = response["channel"]
     timestamp = response["ts"]
```

### Comparing `shipyard_slack-0.1.4a1/PKG-INFO` & `shipyard_slack-0.1.5a0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: shipyard-slack
-Version: 0.1.4a1
+Version: 0.1.5a0
 Summary: A local client for connecting and working with Slack
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: requests (>=2.32.2,<3.0.0)
 Requires-Dist: shipyard-bp-utils (>=1.0.2,<2.0.0)
 Requires-Dist: shipyard-templates (>=0.6.2,<0.7.0)
 Requires-Dist: slack-sdk (>=3.26.2,<4.0.0)
 Description-Content-Type: text/markdown
```

