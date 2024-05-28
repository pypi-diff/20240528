# Comparing `tmp/gpt_computer_assistant-0.1.2.tar.gz` & `tmp/gpt_computer_assistant-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_computer_assistant-0.1.2.tar", last modified: Mon May 27 12:21:42 2024, max compression
+gzip compressed data, was "gpt_computer_assistant-0.2.0.tar", last modified: Mon May 27 19:32:17 2024, max compression
```

## Comparing `gpt_computer_assistant-0.1.2.tar` & `gpt_computer_assistant-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:21:42.942747 gpt_computer_assistant-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-27 12:21:42.942747 gpt_computer_assistant-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:21:42.938748 gpt_computer_assistant-0.1.2/gpt_computer_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:21:42.942747 gpt_computer_assistant-0.1.2/gpt_computer_assistant/agent/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/agent/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/agent/background.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/agent/chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/agent/proccess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:21:42.942747 gpt_computer_assistant-0.1.2/gpt_computer_assistant/audio/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/audio/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/audio/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/gpt_computer_assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:21:42.942747 gpt_computer_assistant-0.1.2/gpt_computer_assistant/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/gui/button.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/gui/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:21:42.942747 gpt_computer_assistant-0.1.2/gpt_computer_assistant/screen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/screen/shot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:21:42.942747 gpt_computer_assistant-0.1.2/gpt_computer_assistant/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant/utils/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:21:42.942747 gpt_computer_assistant-0.1.2/gpt_computer_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-27 12:21:42.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-27 12:21:42.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:21:42.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-27 12:21:42.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:21:42.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 12:21:42.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 12:21:42.000000 gpt_computer_assistant-0.1.2/gpt_computer_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:21:42.942747 gpt_computer_assistant-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-27 12:21:33.000000 gpt_computer_assistant-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.061683 gpt_computer_assistant-0.2.0/gpt_computer_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/proccess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/gpt_computer_assistant/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/audio/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/audio/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/gpt_computer_assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/gpt_computer_assistant/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/gui/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/gui/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/gpt_computer_assistant/screen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/screen/shot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/gpt_computer_assistant/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/utils/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-27 19:32:16.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-27 19:32:17.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:32:16.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-27 19:32:16.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:32:16.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 19:32:16.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 19:32:16.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/setup.py
```

### Comparing `gpt_computer_assistant-0.1.2/LICENSE` & `gpt_computer_assistant-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.2/gpt_computer_assistant/agent/agent.py` & `gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,23 @@
 tools = Tiger()
 tools.enable_auto_requirements = False
 tools = tools.langchain()
 
 
 from langgraph.checkpoint.sqlite import SqliteSaver
 
-from ..utils.db import memory_db
 
-memory = SqliteSaver.from_conn_string(memory_db)
 
 
 
 from langgraph.prebuilt import chat_agent_executor
 
 
 def get_agent_executor():
-    return chat_agent_executor.create_tool_calling_executor(get_model(), tools, checkpointer=memory)
+    return chat_agent_executor.create_tool_calling_executor(get_model(), tools)
 
 
 
 """
 from langchain.agents import Tool
 from langchain_experimental.utilities import PythonREPL
 python_repl = PythonREPL()
@@ -30,9 +28,9 @@
 repl_tool = Tool(
     name="python_repl",
     description="A Python shell. Use this to execute python commands. Input should be a valid python command. If you want to see the output of a value, you should print it out with `print(...)`.",
     func=python_repl.run,
 )
 
 from langgraph.prebuilt import chat_agent_executor
-agent_executor = chat_agent_executor.create_tool_calling_executor(model, [repl_tool], checkpointer=memory)
+agent_executor = chat_agent_executor.create_tool_calling_executor(model, [repl_tool])
 """
```

### Comparing `gpt_computer_assistant-0.1.2/gpt_computer_assistant/agent/assistant.py` & `gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/assistant.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.2/gpt_computer_assistant/agent/background.py` & `gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/background.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from langchain_core.messages import HumanMessage, SystemMessage, AIMessage
+from .chat_history import *
 
-llm_history = [
+
+llm_history_oiginal = [
     SystemMessage(
         content=[
             {"type": "text", "text": "You are an helpful and intelligent assistant. But converting your text to the speech process can be long so please make short your answers as possible."},
             {"type": "text", "text": "Answer with maximum 3 sentences. Also please feel free to use tools."},
             {"type": "text", "text": "If you want to make a long answer using clipboard tool. And say i just copied the answer. Use this way for codes, text fixes."},
             {"type": "text", "text": "If the user wantt to take a action just make the action and say ok. Like copy to clipboard."}
                  ]
                  )
     ]
-
-
```

### Comparing `gpt_computer_assistant-0.1.2/gpt_computer_assistant/agent/proccess.py` & `gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/proccess.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 
 from ..utils.db import system_sound_location, mic_record_location, just_screenshot_path, screenshot_path
 
 
 def process_audio(take_screenshot=True, take_system_audio=False):
-    global audio_data, llm_history
+    global audio_data
 
     
 
     audio_file = open(mic_record_location, "rb")
     transcription = get_client().audio.transcriptions.create(
         model="whisper-1",
         file=audio_file
@@ -44,21 +44,19 @@
 
     
     llm_input = "USER: "+transcription.text
 
     if take_system_audio:
         llm_input += " \n Other of USER: "+transcription2.text
 
-    llm_output = assistant(llm_input, llm_history, get_client(), screenshot_path=screenshot_path if take_screenshot else None)
+    llm_output = assistant(llm_input, chat_message_history.messages, get_client(), screenshot_path=screenshot_path if take_screenshot else None)
 
 
 
 
-    llm_history = llm_output
-
 
     chat_message_history.add_message(llm_output[-1])
     llm_output = llm_output[-1].content
 
 
     response_path = text_to_speech(llm_output)
 
@@ -75,25 +73,25 @@
     
     playback_thread = threading.Thread(target=play_audio)
     playback_thread.start()
 
 
 
 def process_screenshot():
-    global llm_history
+
 
     
     llm_input = "USER: "+"I just take a screenshot. for you to remember. Just say ok."
     print("LLM INPUT (just screenshot)", llm_input)
 
-    llm_output = assistant(llm_input, llm_history, get_client(), screenshot_path=just_screenshot_path)
+    llm_output = assistant(llm_input, chat_message_history.messages, get_client(), screenshot_path=just_screenshot_path)
+
 
 
 
-    llm_history = llm_output
 
 
     chat_message_history.add_message(llm_output[-1])
     llm_output = llm_output[-1].content
```

### Comparing `gpt_computer_assistant-0.1.2/gpt_computer_assistant/audio/record.py` & `gpt_computer_assistant-0.2.0/gpt_computer_assistant/audio/record.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.2/gpt_computer_assistant/audio/tts.py` & `gpt_computer_assistant-0.2.0/gpt_computer_assistant/audio/tts.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.2/gpt_computer_assistant/gpt_computer_assistant.py` & `gpt_computer_assistant-0.2.0/gpt_computer_assistant/gpt_computer_assistant.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.2/gpt_computer_assistant/gui/button.py` & `gpt_computer_assistant-0.2.0/gpt_computer_assistant/gui/button.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from ..audio.record import *
 
 from ..screen.shot import *
 
 from ..agent.proccess import *
 
+from ..agent.chat_history import clear_chat_history
+
 import pyautogui
 recording_thread = None
 
 
 from ..utils.db import screenshot_path, save_api_key, load_api_key
 from ..screen.shot import take_screenshot
 
@@ -105,10 +107,17 @@
         api_key_input = QLineEdit()
         api_key = load_api_key()
         api_key_input.setText(api_key)
         settings_dialog.layout().addWidget(api_key_input)
         save_button = QPushButton("Save")
         save_button.clicked.connect(lambda: save_api_key(api_key_input.text()))
         settings_dialog.layout().addWidget(save_button)
+
+        # Add another button to reset memory
+        reset_memory_button = QPushButton("Reset Memory")
+        reset_memory_button.clicked.connect(clear_chat_history)
+        settings_dialog.layout().addWidget(reset_memory_button)
+
+
         settings_dialog.exec_()
         settings_dialog.show()
```

### Comparing `gpt_computer_assistant-0.1.2/gpt_computer_assistant/utils/db.py` & `gpt_computer_assistant-0.2.0/gpt_computer_assistant/utils/db.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 just_screenshot_path = os.path.join(artifacts_dir, "screenshot.png")
 screenshot_path = os.path.join(artifacts_dir, "screenshot_with_text.png")
 
 
 
-memory_db = os.path.join(artifacts_dir, "memory.db")
+
 history_db = os.path.join(artifacts_dir, "history.db")
 
 openaikey = os.path.join(artifacts_dir, "openaikey.db")
 
 
 def save_api_key(api_key):
         with open(openaikey, 'w') as f:
```

### Comparing `gpt_computer_assistant-0.1.2/gpt_computer_assistant.egg-info/SOURCES.txt` & `gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.2/setup.py` & `gpt_computer_assistant-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 with open('requirements.txt') as fp:
     install_requires = fp.read()
 setup(
     name="gpt_computer_assistant",
-    version="0.1.2",
+    version="0.2.0",
     description="""GPT""",
     long_description="".join(open("README.md", encoding="utf-8").readlines()),
     long_description_content_type="text/markdown",
     url="https://github.com/onuratakan/gpt-computer-assistant",
     author="Onur Atakan ULUSOY",
     author_email="atadogan06@gmail.com",
     license="MIT",
```

