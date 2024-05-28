# Comparing `tmp/postfinancex-0.0.8.tar.gz` & `tmp/postfinancex-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postfinancex-0.0.8.tar", max compression
+gzip compressed data, was "postfinancex-0.0.9.tar", max compression
```

## Comparing `postfinancex-0.0.8.tar` & `postfinancex-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1494 2024-04-12 16:26:18.496679 postfinancex-0.0.8/LICENSE
--rw-r--r--   0        0        0     1406 2024-05-27 00:32:46.191007 postfinancex-0.0.8/README.md
--rw-r--r--   0        0        0      389 2024-05-27 04:37:44.026260 postfinancex-0.0.8/postfinance/__init__.py
--rw-r--r--   0        0        0     3152 2024-05-27 13:05:44.264495 postfinancex-0.0.8/postfinance/agent.py
--rw-r--r--   0        0        0    10672 2024-05-27 13:38:09.376879 postfinancex-0.0.8/postfinance/annotate.py
--rw-r--r--   0        0        0     4317 2024-05-27 12:54:10.868842 postfinancex-0.0.8/postfinance/settings.py
--rw-r--r--   0        0        0     1446 2024-05-27 04:36:04.514673 postfinancex-0.0.8/postfinance/storage.py
--rw-r--r--   0        0        0        0 2024-05-26 22:24:54.394886 postfinancex-0.0.8/postfinance/tools/__init__.py
--rw-r--r--   0        0        0     7272 2024-05-27 04:24:45.593360 postfinancex-0.0.8/postfinance/tools/graph_qa_tool.py
--rw-r--r--   0        0        0     2171 2024-05-27 13:18:47.801553 postfinancex-0.0.8/postfinance/tools/summarization_tool.py
--rw-r--r--   0        0        0     1633 2024-05-26 23:50:41.315057 postfinancex-0.0.8/postfinance/tools/translation_tool.py
--rw-r--r--   0        0        0     2132 2024-05-27 13:16:53.528257 postfinancex-0.0.8/postfinance/tools/vector_search_tool.py
--rw-r--r--   0        0        0    11299 2024-05-27 13:38:20.213406 postfinancex-0.0.8/postfinance/translate.py
--rw-r--r--   0        0        0      805 2024-05-27 12:38:09.662664 postfinancex-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 postfinancex-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1494 2024-04-12 16:26:18.496679 postfinancex-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2690 2024-05-28 13:20:38.807028 postfinancex-0.0.9/README.md
+-rw-r--r--   0        0        0      499 2024-05-28 11:57:16.753945 postfinancex-0.0.9/postfinance/__init__.py
+-rw-r--r--   0        0        0     3422 2024-05-28 12:55:13.046354 postfinancex-0.0.9/postfinance/agent.py
+-rw-r--r--   0        0        0    10672 2024-05-27 13:38:09.376879 postfinancex-0.0.9/postfinance/annotate.py
+-rw-r--r--   0        0        0     4317 2024-05-27 12:54:10.868842 postfinancex-0.0.9/postfinance/settings.py
+-rw-r--r--   0        0        0     1446 2024-05-27 04:36:04.514673 postfinancex-0.0.9/postfinance/storage.py
+-rw-r--r--   0        0        0        0 2024-05-26 22:24:54.394886 postfinancex-0.0.9/postfinance/tools/__init__.py
+-rw-r--r--   0        0        0     7272 2024-05-27 04:24:45.593360 postfinancex-0.0.9/postfinance/tools/graph_qa_tool.py
+-rw-r--r--   0        0        0     2171 2024-05-27 13:18:47.801553 postfinancex-0.0.9/postfinance/tools/summarization_tool.py
+-rw-r--r--   0        0        0     1633 2024-05-26 23:50:41.315057 postfinancex-0.0.9/postfinance/tools/translation_tool.py
+-rw-r--r--   0        0        0     2132 2024-05-27 13:16:53.528257 postfinancex-0.0.9/postfinance/tools/vector_search_tool.py
+-rw-r--r--   0        0        0    11299 2024-05-27 13:38:20.213406 postfinancex-0.0.9/postfinance/translate.py
+-rw-r--r--   0        0        0      805 2024-05-28 13:09:51.816390 postfinancex-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 postfinancex-0.0.9/PKG-INFO
```

### Comparing `postfinancex-0.0.8/LICENSE` & `postfinancex-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.8/postfinance/agent.py` & `postfinancex-0.0.9/postfinance/agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,35 @@
+from typing import Optional
+
 from langchain.agents import AgentExecutor, create_react_agent
 from langchain.chains.conversation.memory import ConversationBufferWindowMemory
 from langchain.prompts import PromptTemplate
+from langchain_community.callbacks.streamlit import StreamlitCallbackHandler
 from langchain_ibm import WatsonxLLM
 
 from .settings import Settings
 from .tools.graph_qa_tool import get_graph_qa_tool
 from .tools.summarization_tool import get_summarization_tool
 from .tools.translation_tool import get_translation_tool
 from .tools.vector_search_tool import get_vector_search_tool
 
-REACT_AGENT_PROMPT_TEMPLATE = """You are a call-center employee at PostFinance, able to have normal interactions with the customer.
+REACT_AGENT_PROMPT_TEMPLATE = """You are a call-center employee at PostFinance, able to have normal interactions with humans.
 
 Be as helpful as possible and return as much information as possible.
 
-But, do NOT answer any questions using your pre-trained knowledge, only use the information provided in the context. If the provided context is irrelevant or insufficient, just say that you don't know the answer, you need to check with your colleagues.
+But, do NOT answer any questions using your pre-trained knowledge, only use the information provided in the context. If the provided context is irrelevant or insufficient, just say that you don't know the answer.
 
 TOOLS:
 ------
 
 You have access to the following tools:
 
 {tools}
 
-You must use one of tools above to answer the question.
+You must use at least one of tools above to answer the question.
 
 To use a tool, please use the following format:
 
 ```
 Thought: Do I need to use a tool? Yes
 Action: the action to take, should be one of [{tool_names}]
 Action Input: the input to the action
@@ -65,23 +68,23 @@
         import json
 
         llm_params = json.dumps(llm.params, indent=4, ensure_ascii=False)
         print(f"Model parameters:\n{llm_params}")
 
     # tools
     _tools = {
-        "translate": get_translation_tool(settings),
-        "graph_qa": get_graph_qa_tool(settings),
-        "vector_search": get_vector_search_tool(settings),
-        "summarize": get_summarization_tool(settings),
+        "translate": get_translation_tool,
+        "graph_qa": get_graph_qa_tool,
+        "vector_search": get_vector_search_tool,
+        "summarize": get_summarization_tool,
     }
 
     tool_names = settings.tools.to_list()
 
-    tools = [_tools[t] for t in tool_names]
+    tools = [_tools[t](settings) for t in tool_names]
 
     if settings.verbose:
         tool_names = ", ".join(tool_names)
         print(f"Tools:\n{tool_names}")
 
     # memory
     memory = ConversationBufferWindowMemory(
@@ -103,9 +106,17 @@
         handle_parsing_errors=True,
         verbose=settings.verbose,
     )
 
     return agent_executor
 
 
-def chat(agent_executor: AgentExecutor, message: str) -> str:
-    return agent_executor.invoke({"input": message})["output"]
+def chat(
+    agent_executor: AgentExecutor,
+    message: str,
+    streamlit_callback: Optional[StreamlitCallbackHandler] = None,
+) -> str:
+    if streamlit_callback is None:
+        return agent_executor.invoke({"input": message})["output"]
+    return agent_executor.invoke(
+        {"input": message}, {"callbacks": [streamlit_callback]}
+    )["output"]
```

### Comparing `postfinancex-0.0.8/postfinance/annotate.py` & `postfinancex-0.0.9/postfinance/annotate.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.8/postfinance/settings.py` & `postfinancex-0.0.9/postfinance/settings.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.8/postfinance/storage.py` & `postfinancex-0.0.9/postfinance/storage.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.8/postfinance/tools/graph_qa_tool.py` & `postfinancex-0.0.9/postfinance/tools/graph_qa_tool.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.8/postfinance/tools/summarization_tool.py` & `postfinancex-0.0.9/postfinance/tools/summarization_tool.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.8/postfinance/tools/translation_tool.py` & `postfinancex-0.0.9/postfinance/tools/translation_tool.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.8/postfinance/tools/vector_search_tool.py` & `postfinancex-0.0.9/postfinance/tools/vector_search_tool.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.8/postfinance/translate.py` & `postfinancex-0.0.9/postfinance/translate.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.8/pyproject.toml` & `postfinancex-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postfinancex"
-version = "0.0.8"
+version = "0.0.9"
 description = "PostFinanceX Virtual Assistant powered by IBM watsonx.ai ✨ PostFinance X IBM watsonx.ai"
 packages = [
     {include = "postfinance"}
 ]
 authors = ["Yi ZHANG <yizhang.dev@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
```

