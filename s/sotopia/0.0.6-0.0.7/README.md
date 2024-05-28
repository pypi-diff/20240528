# Comparing `tmp/sotopia-0.0.6.tar.gz` & `tmp/sotopia-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotopia-0.0.6.tar", max compression
+gzip compressed data, was "sotopia-0.0.7.tar", max compression
```

## Comparing `sotopia-0.0.6.tar` & `sotopia-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0     4500 2023-12-30 20:43:30.649963 sotopia-0.0.6/README.md
--rw-r--r--   0        0        0     1218 2023-12-30 20:54:33.475718 sotopia-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-04 20:26:33.392970 sotopia-0.0.6/sotopia/__init__.py
--rw-r--r--   0        0        0      494 2023-12-30 20:43:34.344519 sotopia-0.0.6/sotopia/agents/__init__.py
--rw-r--r--   0        0        0     1862 2023-12-29 22:08:48.369468 sotopia-0.0.6/sotopia/agents/base_agent.py
--rw-r--r--   0        0        0     2932 2023-12-29 22:08:48.369766 sotopia-0.0.6/sotopia/agents/generate_agent_background.py
--rw-r--r--   0        0        0     7912 2023-12-30 20:43:34.344884 sotopia-0.0.6/sotopia/agents/llm_agent.py
--rw-r--r--   0        0        0     6649 2023-12-30 20:43:30.665752 sotopia-0.0.6/sotopia/agents/redis_agent.py
--rw-r--r--   0        0        0      703 2023-12-30 20:43:30.666133 sotopia-0.0.6/sotopia/database/__init__.py
--rw-r--r--   0        0        0      212 2023-12-30 20:43:30.666361 sotopia-0.0.6/sotopia/database/annotators.py
--rw-r--r--   0        0        0      315 2023-12-30 20:43:30.666575 sotopia-0.0.6/sotopia/database/auto_expires_mixin.py
--rw-r--r--   0        0        0      248 2023-12-30 20:43:30.666776 sotopia-0.0.6/sotopia/database/env_agent_combo_storage.py
--rw-r--r--   0        0        0        8 2023-12-30 20:43:30.667045 sotopia-0.0.6/sotopia/database/handshake.py
--rw-r--r--   0        0        0     3591 2023-12-30 20:43:30.667228 sotopia-0.0.6/sotopia/database/logs.py
--rw-r--r--   0        0        0     5253 2023-12-30 20:43:30.667631 sotopia-0.0.6/sotopia/database/persistent_profile.py
--rw-r--r--   0        0        0     1512 2023-12-30 20:43:30.667845 sotopia-0.0.6/sotopia/database/session_transaction.py
--rw-r--r--   0        0        0      406 2023-12-30 20:43:30.668206 sotopia-0.0.6/sotopia/database/waiting_room.py
--rw-r--r--   0        0        0       75 2023-12-29 22:08:48.371676 sotopia-0.0.6/sotopia/envs/__init__.py
--rw-r--r--   0        0        0    30392 2023-12-30 20:43:34.345450 sotopia-0.0.6/sotopia/envs/evaluators.py
--rw-r--r--   0        0        0    23446 2023-12-30 20:43:34.345942 sotopia-0.0.6/sotopia/envs/parallel.py
--rw-r--r--   0        0        0      253 2023-12-30 20:43:30.670813 sotopia-0.0.6/sotopia/generation_utils/__init__.py
--rw-r--r--   0        0        0    36226 2023-12-30 20:43:34.346685 sotopia-0.0.6/sotopia/generation_utils/generate.py
--rw-r--r--   0        0        0     5623 2023-12-30 20:43:30.671664 sotopia-0.0.6/sotopia/generation_utils/generate_specific_envs.py
--rw-r--r--   0        0        0     1476 2023-12-30 20:43:30.672050 sotopia-0.0.6/sotopia/generation_utils/langchain_callback_handler.py
--rw-r--r--   0        0        0     6893 2023-12-30 20:43:34.347402 sotopia-0.0.6/sotopia/generation_utils/llama2.py
--rw-r--r--   0        0        0      392 2023-12-29 22:08:48.375048 sotopia-0.0.6/sotopia/messages/__init__.py
--rw-r--r--   0        0        0    13089 2023-12-30 20:43:34.348061 sotopia-0.0.6/sotopia/messages/message_classes.py
--rw-r--r--   0        0        0      325 2023-12-29 22:08:48.375606 sotopia-0.0.6/sotopia/messages/messenger.py
--rw-r--r--   0        0        0        0 2023-04-04 20:26:33.393688 sotopia-0.0.6/sotopia/py.typed
--rw-r--r--   0        0        0      144 2023-12-30 20:43:30.675455 sotopia-0.0.6/sotopia/renderers/__init__.py
--rw-r--r--   0        0        0     1422 2023-12-30 20:43:30.675711 sotopia-0.0.6/sotopia/renderers/base.py
--rw-r--r--   0        0        0     2917 2023-12-30 20:43:34.348531 sotopia-0.0.6/sotopia/renderers/xml_renderer.py
--rw-r--r--   0        0        0      265 2023-12-30 20:43:30.676362 sotopia-0.0.6/sotopia/samplers/__init__.py
--rw-r--r--   0        0        0     1992 2023-12-30 20:43:30.677050 sotopia-0.0.6/sotopia/samplers/base_sampler.py
--rw-r--r--   0        0        0     6695 2023-12-30 20:43:30.677506 sotopia-0.0.6/sotopia/samplers/constraint_based_sampler.py
--rw-r--r--   0        0        0     4195 2023-12-30 20:43:30.677993 sotopia-0.0.6/sotopia/samplers/uniform_sampler.py
--rw-r--r--   0        0        0    17049 2023-12-30 20:43:34.349090 sotopia-0.0.6/sotopia/server.py
--rw-r--r--   0        0        0      167 2023-12-29 22:08:48.381467 sotopia-0.0.6/sotopia/utils.py
--rw-r--r--   0        0        0     5764 1970-01-01 00:00:00.000000 sotopia-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-28 19:13:02.448295 sotopia-0.0.7/LICENSE
+-rw-r--r--   0        0        0     9151 2024-05-28 19:13:02.448295 sotopia-0.0.7/README.md
+-rw-r--r--   0        0        0     1951 2024-05-28 19:13:02.460296 sotopia-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/__init__.py
+-rw-r--r--   0        0        0      494 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/agents/__init__.py
+-rw-r--r--   0        0        0     1709 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/agents/base_agent.py
+-rw-r--r--   0        0        0     2914 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/agents/generate_agent_background.py
+-rw-r--r--   0        0        0     8021 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/agents/llm_agent.py
+-rw-r--r--   0        0        0     6764 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/agents/redis_agent.py
+-rw-r--r--   0        0        0     1854 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/__init__.py
+-rw-r--r--   0        0        0     4284 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/aggregate_annotations.py
+-rw-r--r--   0        0        0      187 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/annotators.py
+-rw-r--r--   0        0        0      315 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/auto_expires_mixin.py
+-rw-r--r--   0        0        0      248 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/env_agent_combo_storage.py
+-rw-r--r--   0        0        0        8 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/handshake.py
+-rw-r--r--   0        0        0     3358 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/logs.py
+-rw-r--r--   0        0        0     5262 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/persistent_profile.py
+-rw-r--r--   0        0        0    21934 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/serialization.py
+-rw-r--r--   0        0        0     1398 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/session_transaction.py
+-rw-r--r--   0        0        0      406 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/waiting_room.py
+-rw-r--r--   0        0        0       75 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/envs/__init__.py
+-rw-r--r--   0        0        0    30043 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/envs/evaluators.py
+-rw-r--r--   0        0        0    22614 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/envs/parallel.py
+-rw-r--r--   0        0        0      253 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/generation_utils/__init__.py
+-rw-r--r--   0        0        0    35603 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/generation_utils/generate.py
+-rw-r--r--   0        0        0     1476 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/generation_utils/langchain_callback_handler.py
+-rw-r--r--   0        0        0     6567 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/generation_utils/llama2.py
+-rw-r--r--   0        0        0      392 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/messages/__init__.py
+-rw-r--r--   0        0        0    13319 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/messages/message_classes.py
+-rw-r--r--   0        0        0      325 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/messages/messenger.py
+-rw-r--r--   0        0        0        0 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/py.typed
+-rw-r--r--   0        0        0      144 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/renderers/__init__.py
+-rw-r--r--   0        0        0     1408 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/renderers/base.py
+-rw-r--r--   0        0        0     2822 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/renderers/xml_renderer.py
+-rw-r--r--   0        0        0      265 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/samplers/__init__.py
+-rw-r--r--   0        0        0     1986 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/samplers/base_sampler.py
+-rw-r--r--   0        0        0     6560 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/samplers/constraint_based_sampler.py
+-rw-r--r--   0        0        0     4095 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/samplers/uniform_sampler.py
+-rw-r--r--   0        0        0    16553 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/server.py
+-rw-r--r--   0        0        0      167 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/utils.py
+-rw-r--r--   0        0        0    11094 1970-01-01 00:00:00.000000 sotopia-0.0.7/PKG-INFO
```

### Comparing `sotopia-0.0.6/sotopia/agents/base_agent.py` & `sotopia-0.0.7/sotopia/agents/base_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import uuid
-from typing import Generic, TypeVar, cast
+from typing import Generic, TypeVar
 
 from redis_om.model.model import NotFoundError
 
 from sotopia.database import AgentProfile
-from sotopia.messages import Message, MessengerMixin
+from sotopia.messages import MessengerMixin
 
 ObsType = TypeVar("ObsType")
 ActType = TypeVar("ActType")
 
 
 class BaseAgent(Generic[ObsType, ActType], MessengerMixin):
     def __init__(
@@ -16,41 +15,33 @@
         agent_name: str | None = None,
         uuid_str: str | None = None,
         agent_profile: AgentProfile | None = None,
     ) -> None:
         MessengerMixin.__init__(self)
         if agent_profile is not None:
             self.profile = agent_profile
-            self.agent_name = (
-                self.profile.first_name + " " + self.profile.last_name
-            )
+            self.agent_name = self.profile.first_name + " " + self.profile.last_name
         elif uuid_str is not None:
             # try retrieving profile from database
             try:
                 self.profile = AgentProfile.get(pk=uuid_str)
             except NotFoundError:
-                raise ValueError(
-                    f"Agent with uuid {uuid_str} not found in database"
-                )
-            self.agent_name = (
-                self.profile.first_name + " " + self.profile.last_name
-            )
+                raise ValueError(f"Agent with uuid {uuid_str} not found in database")
+            self.agent_name = self.profile.first_name + " " + self.profile.last_name
         else:
             assert (
                 agent_name is not None
             ), "Either agent_name or uuid_str must be provided"
             self.agent_name = agent_name
 
         self._goal: str | None = None
 
     @property
     def goal(self) -> str:
-        assert (
-            self._goal is not None
-        ), "attribute goal has to be set before use"
+        assert self._goal is not None, "attribute goal has to be set before use"
         return self._goal
 
     @goal.setter
     def goal(self, goal: str) -> None:
         self._goal = goal
 
     def act(self, obs: ObsType) -> ActType:
```

### Comparing `sotopia-0.0.6/sotopia/agents/generate_agent_background.py` & `sotopia-0.0.7/sotopia/agents/generate_agent_background.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import os
 from typing import Callable
 
 from sotopia.generation_utils.generate import (
-    LLM_Name,
     convert_narratives,
     generate_init_profile,
 )
 from sotopia.messages import Message, ScriptBackground
 
 
 def generate_background(
@@ -46,15 +45,15 @@
     seed: dict[str, str],
     basic_info: dict[str, str],
     initial_profile: str,
     profile: str,
     background_json_file: str,
     run_sync_server: Callable[..., list[tuple[str, str, Message]]],
 ) -> tuple[list[tuple[str, str, Message]], ScriptBackground]:
-    scenario, topic, role, q_goal, a_goal = (
+    scenario, _topic, role, q_goal, a_goal = (
         seed["scenario"],
         seed["topic"],
         seed["role"],
         seed["q_goal"],
         seed["a_goal"],
     )
     background = ScriptBackground(
@@ -66,15 +65,15 @@
         p1_goal=q_goal,
         p2_goal=a_goal,
     )
     with open(background_json_file, "w") as f:
         background_dict = json.loads(background.json())
         json.dump(background_dict, f, indent=4)
 
-    model_names: dict[str, LLM_Name] = {
+    model_names: dict[str, str] = {
         "env": "gpt-3.5-turbo",
         "agent2": "gpt-3.5-turbo",
         "agent1": "gpt-4",
     }
 
     agents_info: dict[str, dict[str, str]] = {
         "env": {"mode": "all"},
```

### Comparing `sotopia-0.0.6/sotopia/agents/llm_agent.py` & `sotopia-0.0.7/sotopia/agents/llm_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
-from typing import Callable
+from typing import Callable, cast
 
 from sotopia.agents import BaseAgent
 from sotopia.database import AgentProfile
 from sotopia.generation_utils.generate import (
-    LLM_Name,
     agenerate_action,
     agenerate_script,
     generate_action,
     generate_action_speak,
     generate_goal,
 )
-from sotopia.messages import AgentAction, Message, Observation
+from sotopia.messages import AgentAction, Observation
 from sotopia.messages.message_classes import ScriptBackground
 
 
 async def ainput(prompt: str = "") -> str:
     with ThreadPoolExecutor(1, "ainput") as executor:
         return (
-            await asyncio.get_event_loop().run_in_executor(
-                executor, input, prompt
-            )
+            await asyncio.get_event_loop().run_in_executor(executor, input, prompt)
         ).rstrip()
 
 
 class LLMAgent(BaseAgent[Observation, AgentAction]):
     def __init__(
         self,
         agent_name: str | None = None,
         uuid_str: str | None = None,
         agent_profile: AgentProfile | None = None,
-        model_name: LLM_Name = "gpt-3.5-turbo",
+        model_name: str = "gpt-3.5-turbo",
         script_like: bool = False,
     ) -> None:
         super().__init__(
             agent_name=agent_name,
             uuid_str=uuid_str,
             agent_profile=agent_profile,
         )
@@ -69,17 +66,15 @@
         self.recv_message("Environment", obs)
 
         if len(obs.available_actions) == 1 and "none" in obs.available_actions:
             return AgentAction(action_type="none", argument="")
         else:
             action = gen_func(
                 self.model_name,
-                history="\n".join(
-                    f"{y.to_natural_language()}" for x, y in self.inbox
-                ),
+                history="\n".join(f"{y.to_natural_language()}" for x, y in self.inbox),
                 turn_number=obs.turn_number,
                 action_types=obs.available_actions,
                 agent=self.agent_name,
                 goal=self.goal,
             )
             return action
 
@@ -87,36 +82,43 @@
         self.recv_message("Environment", obs)
 
         if len(obs.available_actions) == 1 and "none" in obs.available_actions:
             return AgentAction(action_type="none", argument="")
         else:
             action, prompt = await agenerate_action(
                 self.model_name,
-                history="\n".join(
-                    f"{y.to_natural_language()}" for x, y in self.inbox
-                ),
+                history="\n".join(f"{y.to_natural_language()}" for x, y in self.inbox),
                 turn_number=obs.turn_number,
                 action_types=obs.available_actions,
                 agent=self.agent_name,
                 goal=self.goal,
                 script_like=self.script_like,
             )
-            return action
-
+            # Temporary fix for mixtral-moe model for incorrect generation format
+            if "Mixtral-8x7B-Instruct-v0.1" in self.model_name:
+                current_agent = self.agent_name
+                if f"{current_agent}:" in action.argument:
+                    print("Fixing Mixtral's generation format")
+                    action.argument = action.argument.replace(f"{current_agent}: ", "")
+                elif f"{current_agent} said:" in action.argument:
+                    print("Fixing Mixtral's generation format")
+                    action.argument = action.argument.replace(
+                        f"{current_agent} said: ", ""
+                    )
 
-from typing import cast
+            return action
 
 
 class ScriptWritingAgent(LLMAgent):
     def __init__(
         self,
         agent_name: str | None = None,
         uuid_str: str | None = None,
         agent_profile: AgentProfile | None = None,
-        model_name: LLM_Name = "gpt-3.5-turbo",
+        model_name: str = "gpt-3.5-turbo",
         agent_names: list[str] = [],
         background: ScriptBackground | None = None,
     ) -> None:
         super().__init__(
             agent_name=agent_name,
             uuid_str=uuid_str,
             agent_profile=agent_profile,
@@ -124,40 +126,27 @@
         self.model_name = model_name
         self.agent_names = agent_names
         assert background is not None, "background cannot be None"
         self.background = background
 
     async def aact(self, obs: Observation) -> AgentAction:
         self.recv_message("Environment", obs)
-        message_to_compose = [
-            y for idx, (x, y) in enumerate(self.inbox) if idx != 0
-        ]
+        message_to_compose = [y for idx, (x, y) in enumerate(self.inbox) if idx != 0]
 
-        history = "\n".join(
-            f"{y.to_natural_language()}" for y in message_to_compose
-        )
-        print("Current agent: ", self.agent_name)
-        print("Composed history: ", history)
+        history = "\n".join(f"{y.to_natural_language()}" for y in message_to_compose)
 
         action, prompt = await agenerate_script(
             model_name=self.model_name,
             background=self.background,
             agent_names=self.agent_names,
             history=history,
             agent_name=self.agent_name,
             single_step=True,
         )
-        # action: tuple[
-        #     list[list[tuple[str, str, Message]]], list[tuple[str, Message]]
-        # ]
         returned_action = cast(AgentAction, action[1][0][1])
-        print("Action: ", returned_action, type(returned_action))
-        # print("Action: ", action)
-        # exit(0)
-
         return returned_action
 
 
 class SpeakAgent(LLMAgent):
     def act(
         self,
         obs: Observation,
@@ -215,23 +204,21 @@
 
         if obs.available_actions != ["none"]:
             action_type_number = await ainput(
                 "Action type (Please only input the number): "
             )
             try:
                 action_type_number = int(action_type_number)  # type: ignore
-            except:
+            except TypeError:
                 print("Please input a number.")
                 action_type_number = await ainput(
                     "Action type (Please only input the number): "
                 )
                 action_type_number = int(action_type_number)  # type: ignore
-            assert isinstance(
-                action_type_number, int
-            ), "Please input a number."
+            assert isinstance(action_type_number, int), "Please input a number."
             action_type = obs.available_actions[action_type_number]
         else:
             action_type = "none"
         if action_type in ["speak", "non-verbal communication"]:
             argument = await ainput("Argument: ")
         else:
             argument = ""
@@ -242,10 +229,9 @@
 class Agents(dict[str, BaseAgent[Observation, AgentAction]]):
     def reset(self) -> None:
         for agent in self.values():
             agent.reset()
 
     def act(self, obs: dict[str, Observation]) -> dict[str, AgentAction]:
         return {
-            agent_name: agent.act(obs[agent_name])
-            for agent_name, agent in self.items()
+            agent_name: agent.act(obs[agent_name]) for agent_name, agent in self.items()
         }
```

### Comparing `sotopia-0.0.6/sotopia/agents/redis_agent.py` & `sotopia-0.0.7/sotopia/agents/redis_agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 import asyncio
 import logging
 import os
-import time
-from datetime import datetime
 from uuid import uuid4
 
 import aiohttp
 import pydantic
-import redis
-import redis.asyncio as aredis
 import requests
 
 from sotopia.agents import BaseAgent
 from sotopia.database import AgentProfile, MessageTransaction
 from sotopia.messages import AgentAction, Observation
 
-_URL = "http://tiger.lti.cs.cmu.edu:8000"
-
 
 class RedisAgent(BaseAgent[Observation, AgentAction]):
     """An agent use redis as a message broker."""
 
     def __init__(
         self,
         agent_name: str | None = None,
@@ -32,16 +26,23 @@
             agent_name=agent_name,
             uuid_str=uuid_str,
             agent_profile=agent_profile,
         )
         # super().__init__(agent_name=agent_name, uuid_str=uuid_str)
         self.session_id = session_id or str(uuid4())
         self.sender_id = str(uuid4())
+        print(f"session id: {self.session_id}")
+        print("step 1: connect to the server")
+        assert (
+            "FASTAPI_URL" in os.environ
+        ), "To use redis agent, you have to launch a FastAPI server and set FASTAPI_URL"
+        self._URL = os.environ["FASTAPI_URL"]
         response = requests.request(
-            "POST", f"{_URL}/connect/{self.session_id}/server/{self.sender_id}"
+            "POST",
+            f"{self._URL}/connect/{self.session_id}/server/{self.sender_id}",
         )
         assert (
             response.status_code == 200 and response.text == "[]"
         ), "Failed to connect to the server"
         logging.info(f"Session ID: {self.session_id}")
         # logging.info(f"Sender ID: {self.sender_id}")
 
@@ -56,36 +57,35 @@
         obs: Observation,
     ) -> AgentAction:
         self.recv_message("Environment", obs)
 
         if len(obs.available_actions) == 1 and "none" in obs.available_actions:
             if obs.turn_number == 0:
                 async with aiohttp.ClientSession() as session:
+                    print("step 2: post observation to the message list")
                     response = await session.request(
                         "POST",
-                        f"{_URL}/send/{self.session_id}/{self.sender_id}",
+                        f"{self._URL}/send/{self.session_id}/{self.sender_id}",
                         data=obs.to_natural_language(),
                     )
                     assert response.status == 200, response
                     sorted_message_list: list[tuple[float, str, str]] = list(
                         map(
-                            lambda x: MessageTransaction.parse_obj(
-                                x
-                            ).to_tuple(),
+                            lambda x: MessageTransaction.parse_obj(x).to_tuple(),
                             await response.json(),
                         )
                     )
                     last_timestamp = sorted_message_list[-1][0]
             return AgentAction(action_type="none", argument="")
         else:
             async with aiohttp.ClientSession() as session:
                 # 1. post observation to the message list
                 response = await session.request(
                     "POST",
-                    f"{_URL}/send/{self.session_id}/{self.sender_id}",
+                    f"{self._URL}/send/{self.session_id}/{self.sender_id}",
                     data=obs.to_natural_language(),
                 )
                 assert response.status == 200, response
                 sorted_message_list = list(
                     map(
                         lambda x: MessageTransaction.parse_obj(x).to_tuple(),
                         await response.json(),
@@ -93,57 +93,53 @@
                 )
                 last_timestamp = sorted_message_list[-1][0]
 
                 print("step 2: unlock the server for the client")
                 # 2. unlock the server for the client
                 response = await session.request(
                     "PUT",
-                    f"{_URL}/lock/{self.session_id}/{self.sender_id}/action",
+                    f"{self._URL}/lock/{self.session_id}/{self.sender_id}/action",
                 )
                 assert response.status == 200, response
 
                 print("step 3: wait for the client to post their message")
                 # 3. wait for the client to post their message
                 for _ in range(300):
                     response = await session.request(
                         "GET",
-                        f"{_URL}/get/{self.session_id}",
+                        f"{self._URL}/get/{self.session_id}",
                     )
                     # print(f"get response: {response}")
                     assert response.status == 200, response
                     sorted_message_list = list(
                         map(
-                            lambda x: MessageTransaction.parse_obj(
-                                x
-                            ).to_tuple(),
+                            lambda x: MessageTransaction.parse_obj(x).to_tuple(),
                             await response.json(),
                         )
                     )
                     if (
                         sorted_message_list[-1][0] > last_timestamp
                         and sorted_message_list[-1][1] == "client"
                     ):
                         # 3.a if the client has posted their message, lock the server for the client
                         response = await session.request(
                             "PUT",
-                            f"{_URL}/lock/{self.session_id}/{self.sender_id}/no%20action",
+                            f"{self._URL}/lock/{self.session_id}/{self.sender_id}/no%20action",
                         )
                         assert response.status == 200, response
                         break
                     else:
                         # 3.b if the client has not posted their message, wait for 0.1 second and retry
                         await asyncio.sleep(1)
                 else:
                     response = await session.request(
                         "PUT",
-                        f"{_URL}/lock/{self.session_id}/{self.sender_id}/no%20action",
-                    )
-                    self.reset(
-                        "Someone has left or the conversation is too long."
+                        f"{self._URL}/lock/{self.session_id}/{self.sender_id}/no%20action",
                     )
+                    self.reset("Someone has left or the conversation is too long.")
                     return AgentAction(action_type="leave", argument="")
             action_string = sorted_message_list[-1][2]
             try:
                 action = AgentAction.parse_raw(action_string)
                 return action
             except pydantic.error_wrappers.ValidationError:
                 logging.warn(
@@ -160,14 +156,14 @@
         reset_reason: str = "",
     ) -> None:
         super().reset()
         try:
             if reset_reason != "":
                 response = requests.request(
                     "POST",
-                    f"{_URL}/send/{self.session_id}/{self.sender_id}",
+                    f"{self._URL}/send/{self.session_id}/{self.sender_id}",
                     json=reset_reason,
                 )
                 assert response.status_code == 200
 
         except Exception as e:
             logging.error(f"Failed to reset RedisAgent {self.sender_id}: {e}")
```

### Comparing `sotopia-0.0.6/sotopia/database/logs.py` & `sotopia-0.0.7/sotopia/database/logs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-from typing import Any, cast
+from typing import Any
 
-from pydantic import ConstrainedList, conlist, root_validator
-from redis_om import HashModel, JsonModel
+from pydantic import root_validator
+from redis_om import JsonModel
 from redis_om.model.model import Field
 
 from sotopia.database.persistent_profile import AgentProfile
-from sotopia.messages import Message
 
 
 class EpisodeLog(JsonModel):
     # Note that we did not validate the following constraints:
     # 1. The number of turns in messages and rewards should be the same or off by 1
     # 2. The agents in the messages are the same as the agetns
 
     environment: str = Field(index=True)
     agents: list[str] = Field(index=True)
     tag: str | None = Field(index=True)
     models: list[str] | None = Field(index=True)
     messages: list[list[tuple[str, str, str]]]  # Messages arranged by turn
     reasoning: str
-    rewards: list[
-        tuple[float, dict[str, float]] | float
-    ]  # Rewards arranged by turn
+    rewards: list[tuple[float, dict[str, float]] | float]  # Rewards arranged by turn
     rewards_prompt: str
 
-    @root_validator
+    @root_validator(skip_on_failure=True)
     def agent_number_message_number_reward_number_turn_number_match(
         cls, values: Any
     ) -> Any:
-        agents, _, reasoning, rewards = (
+        agents, _, _reasoning, rewards = (
             values.get("agents"),
             values.get("messages"),
             values.get("reasoning"),
             values.get("rewards"),
         )
         agent_number = len(agents)
 
@@ -44,17 +41,15 @@
     def render_for_humans(self) -> tuple[list[AgentProfile], list[str]]:
         """Generate a human readable version of the episode log.
 
         Returns:
             A tuple of (a list of agent_profiles, a list of str): The agent profiles, and the messages and rewards in each turn.
         """
 
-        agent_profiles = [
-            AgentProfile.get(pk=uuid_str) for uuid_str in self.agents
-        ]
+        agent_profiles = [AgentProfile.get(pk=uuid_str) for uuid_str in self.agents]
         messages_and_rewards = []
         for idx, turn in enumerate(self.messages):
             messages_in_this_turn = []
             if idx == 0:
                 assert (
                     len(turn) >= 2
                 ), "The first turn should have at least environemnt messages"
@@ -63,21 +58,17 @@
             for sender, receiver, message in turn:
                 if receiver == "Environment":
                     if sender != "Environment":
                         if "did nothing" in message:
                             continue
                         else:
                             if "said:" in message:
-                                messages_in_this_turn.append(
-                                    f"{sender} {message}"
-                                )
+                                messages_in_this_turn.append(f"{sender} {message}")
                             else:
-                                messages_in_this_turn.append(
-                                    f"{sender}: {message}"
-                                )
+                                messages_in_this_turn.append(f"{sender}: {message}")
                     else:
                         messages_in_this_turn.append(message)
             messages_and_rewards.append("\n".join(messages_in_this_turn))
         messages_and_rewards.append(f"The reasoning is:\n{self.reasoning}")
         messages_and_rewards.append(
             f"The rewards are:\nAgent 1: {self.rewards[0]}\nAgent 2: {self.rewards[1]}"
         )
```

### Comparing `sotopia-0.0.6/sotopia/database/persistent_profile.py` & `sotopia-0.0.7/sotopia/database/persistent_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import uuid
 from enum import IntEnum
-from typing import Any, cast
+from typing import Any
 
-from pydantic import root_validator, validator
+from pydantic import root_validator
 from redis_om import JsonModel
 from redis_om.model.model import Field
 
 
 class RelationshipType(IntEnum):
     stranger = 0
     know_by_name = 1
@@ -22,21 +21,20 @@
     age: int = Field(index=True, default_factory=lambda: 0)
     occupation: str = Field(index=True, default_factory=lambda: "")
     gender: str = Field(index=True, default_factory=lambda: "")
     gender_pronoun: str = Field(index=True, default_factory=lambda: "")
     public_info: str = Field(index=True, default_factory=lambda: "")
     big_five: str = Field(index=True, default_factory=lambda: "")
     moral_values: list[str] = Field(index=False, default_factory=lambda: [])
-    schwartz_personal_values: list[str] = Field(
-        index=False, default_factory=lambda: []
-    )
+    schwartz_personal_values: list[str] = Field(index=False, default_factory=lambda: [])
     personality_and_values: str = Field(index=True, default_factory=lambda: "")
     decision_making_style: str = Field(index=True, default_factory=lambda: "")
     secret: str = Field(default_factory=lambda: "")
     model_id: str = Field(default_factory=lambda: "")
+    mbti: str = Field(default_factory=lambda: "")
 
 
 class EnvironmentProfile(JsonModel):
     codename: str = Field(
         index=True,
         default_factory=lambda: "",
         description="The codename of the environment",
@@ -93,11 +91,11 @@
     def the_length_agent_index_matches_environments(cls, values: Any) -> Any:
         environments, agent_index = (
             values.get("environments"),
             values.get("agent_index"),
         )
         if agent_index is None:
             return values
-        assert len(environments) == len(
-            agent_index
+        assert (
+            len(environments) == len(agent_index)
         ), f"Number of environments {len(environments)} and agent_index {len(agent_index)} do not match"
         return values
```

### Comparing `sotopia-0.0.6/sotopia/database/session_transaction.py` & `sotopia-0.0.7/sotopia/database/session_transaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-from pydantic import Field as PydanticField
 from pydantic import validator
 from redis_om import EmbeddedJsonModel, JsonModel
 from redis_om.model.model import Field
 
-from sotopia.messages import AgentAction, Observation, SimpleMessage
-
 from .auto_expires_mixin import AutoExpireMixin
 
 
 class MessageTransaction(EmbeddedJsonModel):
     timestamp_str: str = Field(index=True)
     sender: str = Field(index=True)
     message: str
```

### Comparing `sotopia-0.0.6/sotopia/envs/evaluators.py` & `sotopia-0.0.7/sotopia/envs/evaluators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 import abc
 import logging
 from collections import defaultdict
-from typing import Generic, Type, Union
 
 import gin
 from beartype import beartype
 from langchain.output_parsers import PydanticOutputParser
-from langchain.schema import BaseOutputParser
 from pydantic import BaseModel, Field, validator
 
-from sotopia.generation_utils.generate import (
-    EnvResponsePydanticOutputParser,
-    ListOfIntOutputParser,
-    LLM_Name,
-    agenerate,
-    generate,
-)
+from sotopia.generation_utils.generate import agenerate
 from sotopia.messages import (
     AgentAction,
     Message,
     ScriptEnvironmentResponse,
 )
 
 log = logging.getLogger("evaluators")
@@ -74,24 +66,20 @@
 
     @validator("believability", "knowledge", "goal")
     def zero_to_ten_validator(cls, v: tuple[str, int]) -> tuple[str, int]:
         assert v[1] >= 0 and v[1] <= 10
         return v
 
     @validator("relationship", "financial_and_material_benefits")
-    def minus_five_to_five_validator(
-        cls, v: tuple[str, int]
-    ) -> tuple[str, int]:
+    def minus_five_to_five_validator(cls, v: tuple[str, int]) -> tuple[str, int]:
         assert v[1] >= -5 and v[1] <= 5
         return v
 
     @validator("secret", "social_rules")
-    def minus_ten_to_zero_validator(
-        cls, v: tuple[str, int]
-    ) -> tuple[str, int]:
+    def minus_ten_to_zero_validator(cls, v: tuple[str, int]) -> tuple[str, int]:
         assert v[1] >= -10 and v[1] <= 0
         return v
 
 
 class EvaluationBySocialDimensionsPlus(BaseModel):
     believability: tuple[str, int] = Field(
         ...,
@@ -141,24 +129,20 @@
 
     @validator("believability", "knowledge", "goal")
     def zero_to_ten_validator(cls, v: tuple[str, int]) -> tuple[str, int]:
         assert v[1] >= 0 and v[1] <= 10
         return v
 
     @validator("relationship", "financial_and_material_benefits")
-    def minus_five_to_five_validator(
-        cls, v: tuple[str, int]
-    ) -> tuple[str, int]:
+    def minus_five_to_five_validator(cls, v: tuple[str, int]) -> tuple[str, int]:
         assert v[1] >= -5 and v[1] <= 5
         return v
 
     @validator("secret", "social_rules")
-    def minus_ten_to_zero_validator(
-        cls, v: tuple[str, int]
-    ) -> tuple[str, int]:
+    def minus_ten_to_zero_validator(cls, v: tuple[str, int]) -> tuple[str, int]:
         assert v[1] >= -10 and v[1] <= 0
         return v
 
 
 class EnvResponse(BaseModel):
     agent_1_evaluation: EvaluationBySocialDimensions
     agent_2_evaluation: EvaluationBySocialDimensions
@@ -184,17 +168,15 @@
         self, turn_number: int, messages: list[tuple[str, Message]]
     ) -> list[tuple[str, tuple[tuple[str, int | float | bool], str]]]:
         raise NotImplementedError
 
 
 @beartype
 class RuleBasedTerminatedEvaluator(Evaluator):
-    def __init__(
-        self, max_turn_number: int = 20, max_stale_turn: int = 2
-    ) -> None:
+    def __init__(self, max_turn_number: int = 20, max_stale_turn: int = 2) -> None:
         self.max_turn_number = max_turn_number
         self.max_stale_turn = max_stale_turn
 
     def __call__(
         self, turn_number: int, messages: list[tuple[str, Message]]
     ) -> list[tuple[str, tuple[tuple[str, int | float | bool], str]]]:
         # Rule 1: If the conversation is too long, terminate the conversation
@@ -219,17 +201,15 @@
             if message[1].action_type == "none":
                 stale_count += 1
             else:
                 break
             if stale_count > self.max_stale_turn:
                 break
         stale_too_long = stale_count > self.max_stale_turn
-        terminated = (
-            conversation_too_long or p1_leaving or p2_leaving or stale_too_long
-        )
+        terminated = conversation_too_long or p1_leaving or p2_leaving or stale_too_long
         reasons_for_termination = (
             f"{'The conversation is too long; ' if conversation_too_long else ''}"
             f"{'Agent 1 is leaving; ' if p1_leaving else ''}"
             f"{'Agent 2 is leaving; ' if p2_leaving else ''}"
             f"{'The conversation stales for too long; ' if stale_too_long else ''}"
         )
         return [
@@ -243,17 +223,15 @@
         self, turn_number: int, messages: list[tuple[str, Message]]
     ) -> list[tuple[str, tuple[tuple[str, int | float | bool], str]]]:
         return self(turn_number, messages)
 
 
 class ReachGoalLLMEvaluator(Evaluator):
     @beartype
-    def __init__(
-        self, model_name: LLM_Name, response_format: str = "basic"
-    ) -> None:
+    def __init__(self, model_name: str, response_format: str = "basic") -> None:
         self.model_name = model_name
         self.prompt = ""
         self.response_format = response_format
 
     def __call__(
         self, turn_number: int, messages: list[tuple[str, Message]]
     ) -> list[tuple[str, tuple[tuple[str, int | float | bool], str]]]:
@@ -275,80 +253,80 @@
             messages_filtered = [
                 (x, y)
                 for x, y in messages
                 if "did nothing" not in y.to_natural_language()
             ]
             history = "\n".join(
                 [
-                    f"{x} {y.to_natural_language()}"
-                    if x != "Environment"
-                    else y.to_natural_language()
+                    (
+                        f"{x} {y.to_natural_language()}"
+                        if x != "Environment"
+                        else y.to_natural_language()
+                    )
                     for x, y in messages_filtered
                 ]
             )
         response_format_class = (
             EnvResponsePlus if self.response_format == "plus" else EnvResponse
         )
 
         try:
-            response: EnvResponsePlus | EnvResponse  # fix type error from langchain 0.0.264. we don't need this line for langchain 0.0.263
+            response: (
+                EnvResponsePlus | EnvResponse
+            )  # fix type error from langchain 0.0.264. we don't need this line for langchain 0.0.263
             response, prompt = await agenerate(
                 model_name=self.model_name,
                 template="""{history},
                     Based on previous interactions, evaluate how well participants achieve their goals.
                     Please following the format:
                     {format_instructions}
                 """,
                 input_values=dict(history=history),
-                output_parser=PydanticOutputParser[
-                    EnvResponsePlus | EnvResponse
-                ](pydantic_object=response_format_class),
+                output_parser=PydanticOutputParser[EnvResponsePlus | EnvResponse](
+                    pydantic_object=response_format_class
+                ),
                 temperature=temperature,
             )
             self.prompt = prompt
             response_list = []
             # TODO: multiple agents
             for dimension in response.agent_1_evaluation.dict().keys():
                 response_list.append(
                     (
                         "agent_1",
                         (
                             (
                                 dimension,
-                                response.agent_1_evaluation.dict()[dimension][
-                                    1
-                                ],
+                                response.agent_1_evaluation.dict()[dimension][1],
                             ),
                             response.agent_1_evaluation.dict()[dimension][0],
                         ),
                     )
                 )
                 response_list.append(
                     (
                         "agent_2",
                         (
                             (
                                 dimension,
-                                response.agent_2_evaluation.dict()[dimension][
-                                    1
-                                ],
+                                response.agent_2_evaluation.dict()[dimension][1],
                             ),
                             response.agent_2_evaluation.dict()[dimension][0],
                         ),
                     )
                 )
             return response_list
         except Exception as e:
             log.debug(f"[red] Failed to generate environment response. {e}")
             return []
 
 
 @beartype
 def _reduce(
-    responses_per_reducer: list[tuple[tuple[str, float | int | bool], str]]
+    responses_per_reducer: list[tuple[tuple[str, float | int | bool], str]],
 ) -> tuple[dict[str, float | int | bool], str]:
     responses_dict = defaultdict(list)
     comments_dict: dict[str, str] = defaultdict(str)
     reduced_dict: dict[str, float | int | bool] = {}
     for response, reasoning in responses_per_reducer:
         responses_dict[response[0]].append(response[1])
         comments_dict[response[0]] += reasoning
@@ -357,15 +335,15 @@
         if k == "terminated":
             assert all([isinstance(x, bool) for x in v])
             reduced_dict[k] = any(v)
         else:
             assert all([isinstance(x, (float, int)) for x in v])
             reduced_dict[k] = sum(v) / len(v)
             scores.append(reduced_dict[k])
-    if len(scores) and not "overall_score" in responses_dict:
+    if len(scores) and "overall_score" not in responses_dict:
         scores = [x for x in scores if x is not None]
         reduced_dict["overall_score"] = sum(scores) / len(scores)
     comments = "\n".join([f"{k}: {v}" for k, v in comments_dict.items()])
     return reduced_dict, comments
 
 
 @beartype
@@ -375,17 +353,17 @@
     """
     Aggregate the responses from the environment
 
     Args:
         responses (list[tuple[str, tuple[tuple[str, int | bool], str]]]): list of responses from the environment
         Each response is a tuple of (agent_name/environment, (response, reasoning))
     """
-    responses_dict: dict[
-        str, list[tuple[tuple[str, int | float | bool], str]]
-    ] = defaultdict(list)
+    responses_dict: dict[str, list[tuple[tuple[str, int | float | bool], str]]] = (
+        defaultdict(list)
+    )
     for response in responses:
         assert response[0] == "environment" or response[0].startswith("agent")
         responses_dict[response[0]].append(response[1])
 
     environment_responses: tuple[dict[str, float | int | bool], str] = ({}, "")
     agent_1_responses: tuple[dict[str, float | int | bool], str] = ({}, "")
     agent_2_responses: tuple[dict[str, float | int | bool], str] = ({}, "")
```

### Comparing `sotopia-0.0.6/sotopia/envs/parallel.py` & `sotopia-0.0.7/sotopia/envs/parallel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import asyncio
 import copy
 import itertools
-import json
-import logging
 import random
-import uuid
-from copy import deepcopy
-from pathlib import Path
-from typing import Any, Literal, TypedDict, cast
+from typing import Any, Literal
 
 from beartype import beartype
 from gin import configurable
 from gymnasium.spaces.dict import Dict
 from gymnasium.spaces.discrete import Discrete
 from gymnasium.spaces.text import Text
 from pettingzoo.utils.env import ParallelEnv
@@ -19,32 +14,25 @@
 
 from sotopia.agents.llm_agent import Agents
 from sotopia.database import EnvironmentProfile
 from sotopia.database.persistent_profile import (
     AgentProfile,
     RelationshipType,
 )
-from sotopia.generation_utils import LLM_Name
 from sotopia.messages import (
     ActionType,
     AgentAction,
-    Message,
     MessengerMixin,
     Observation,
     ScriptBackground,
     SimpleMessage,
 )
 from sotopia.renderers import RenderContext, XMLRenderer
 
-from .evaluators import (
-    Evaluator,
-    ReachGoalLLMEvaluator,
-    RuleBasedTerminatedEvaluator,
-    unweighted_aggregate_evaluate,
-)
+from .evaluators import Evaluator, unweighted_aggregate_evaluate
 
 
 def _actions_to_natural_language(actions: dict[str, AgentAction]) -> str:
     action_str = ""
     for agent, action in actions.items():
         # Only record actions that did something
         if action.action_type != "none":
@@ -62,52 +50,46 @@
     }
     if gender:
         return gender_to_adj[gender]
     else:
         return ""
 
 
-def _agent_profile_to_stranger_self(
-    profile: AgentProfile, agent_id: int
-) -> str:
+def _agent_profile_to_stranger_self(profile: AgentProfile, agent_id: int) -> str:
     return f"<root><p viewer='agent_{agent_id}'>{profile.first_name} {profile.last_name} is a {profile.age}-year-old {_map_gender_to_adj(profile.gender)} {profile.occupation.lower()}. {profile.gender_pronoun} pronouns. {profile.public_info} Personality and values description: {profile.personality_and_values} {profile.first_name}'s secrets: {profile.secret}</p></root>"
 
 
 def _agent_profile_to_name_self(profile: AgentProfile, agent_id: int) -> str:
     return f"{profile.first_name} {profile.last_name} <p viewer='agent_{agent_id}'>is a {profile.age}-year-old {_map_gender_to_adj(profile.gender)} {profile.occupation.lower()}. {profile.gender_pronoun} pronouns. {profile.public_info} Personality and values description: {profile.personality_and_values} {profile.first_name}'s secrets: {profile.secret}</p>"
 
 
-def _agent_profile_to_aquaintance_self(
-    profile: AgentProfile, agent_id: int
-) -> str:
+def _agent_profile_to_aquaintance_self(profile: AgentProfile, agent_id: int) -> str:
     return f"{profile.first_name} {profile.last_name} is a {profile.age}-year-old {_map_gender_to_adj(profile.gender)} {profile.occupation.lower()}. {profile.gender_pronoun} pronouns. {profile.public_info} <p viewer='agent_{agent_id}'>Personality and values description: {profile.personality_and_values} {profile.first_name}'s secrets: {profile.secret}</p>"
 
 
-def _agent_profile_to_friendabove_self(
-    profile: AgentProfile, agent_id: int
-) -> str:
+def _agent_profile_to_friendabove_self(profile: AgentProfile, agent_id: int) -> str:
     return f"{profile.first_name} {profile.last_name} is a {profile.age}-year-old {_map_gender_to_adj(profile.gender)} {profile.occupation.lower()}. {profile.gender_pronoun} pronouns. {profile.public_info} Personality and values description: {profile.personality_and_values} <p viewer='agent_{agent_id}'>{profile.first_name}'s secrets: {profile.secret}</p>"
 
 
 def get_bio(
     relationship: RelationshipType, profile: AgentProfile, agent_id: int
 ) -> str:
     match relationship:
         case RelationshipType.stranger:
             return _agent_profile_to_stranger_self(profile, agent_id=agent_id)
         case RelationshipType.know_by_name:
             return _agent_profile_to_name_self(profile, agent_id=agent_id)
         case RelationshipType.acquaintance:
-            return _agent_profile_to_aquaintance_self(
-                profile, agent_id=agent_id
-            )
-        case RelationshipType.friend | RelationshipType.romantic_relationship | RelationshipType.family_member:
-            return _agent_profile_to_friendabove_self(
-                profile, agent_id=agent_id
-            )
+            return _agent_profile_to_aquaintance_self(profile, agent_id=agent_id)
+        case (
+            RelationshipType.friend
+            | RelationshipType.romantic_relationship
+            | RelationshipType.family_member
+        ):
+            return _agent_profile_to_friendabove_self(profile, agent_id=agent_id)
         case _:
             raise ValueError(f"Unknown relationship {relationship}")
 
 
 @configurable
 def render_text_for_agent(
     raw_text: str,
@@ -116,17 +98,15 @@
         "extra_info",
         "clarification_hint",
         "strategy_hint",
     ],
 ) -> str:
     return XMLRenderer()(
         raw_text,
-        RenderContext(
-            viewer=f"agent_{agent_id}", tags_to_render=tags_to_render
-        ),
+        RenderContext(viewer=f"agent_{agent_id}", tags_to_render=tags_to_render),
     )
 
 
 @configurable
 def render_text_for_environment(
     raw_text: str,
     tags_to_render: list[str] = [
@@ -137,37 +117,33 @@
 ) -> str:
     return XMLRenderer()(
         raw_text,
         RenderContext(viewer="environment", tags_to_render=tags_to_render),
     )
 
 
-class ParallelSotopiaEnv(
-    ParallelEnv[str, Observation, AgentAction], MessengerMixin
-):
+class ParallelSotopiaEnv(ParallelEnv[str, Observation, AgentAction], MessengerMixin):
     def __init__(
         self,
         available_action_types: set[ActionType] = set(
             ["none", "speak", "non-verbal communication", "action", "leave"]
         ),
-        action_order: Literal[
-            "simutaneous", "round-robin", "random"
-        ] = "simutaneous",
-        model_name: LLM_Name = "gpt-3.5-turbo",
+        action_order: Literal["simutaneous", "round-robin", "random"] = "simutaneous",
+        model_name: str = "gpt-3.5-turbo",
         evaluators: list[Evaluator] = [],
         terminal_evaluators: list[Evaluator] = [],
         uuid_str: str | None = None,
         env_profile: EnvironmentProfile | None = None,
     ) -> None:
         """A sotopia environment for parallel agents.
 
         Args:
             available_action_types (set[ActionType], optional): The action types that are available to the agents. Defaults to set(["none", "speak", "non-verbal communication", "action"]).
             action_order (Literal["simutaneous", "round-robin", "random"], optional): The order in which the agents take actions. Defaults to "simutaneous".
-            model_name (LLM_Name, optional): The name of the language model to use. Defaults to "gpt-3.5-turbo".
+            model_name (str, optional): The name of the language model to use. Defaults to "gpt-3.5-turbo".
         """
         super().__init__()
         self.model_name = model_name
         self.background = ScriptBackground(
             scenario="",
             p1_background="",
             p2_background="",
@@ -193,17 +169,15 @@
             self.profile = env_profile
         # if a uuid is provided, try to load the environment profile from the database
         elif uuid_str is not None:
             # try retrieving profile from database
             try:
                 self.profile = EnvironmentProfile.get(pk=uuid_str)
             except NotFoundError:
-                raise ValueError(
-                    f"Agent with uuid {uuid_str} not found in database"
-                )
+                raise ValueError(f"Agent with uuid {uuid_str} not found in database")
 
     @configurable
     def reset(
         self,
         seed: int | None = None,
         options: dict[str, str] | None = None,
         agents: Agents | None = None,
@@ -219,25 +193,23 @@
                 "full_background_file" (str): Path to a json file which need to contain a ScriptBackground object. The backgound must be completed (no "unknown" for missing parts).
             omniscient (bool, optional): Whether the agents know the other agent's goal. Defaults to False.
         """
         super().__init__()
         MessengerMixin.reset_inbox(self)
         assert (
             not options
-            or not ("partial_background_file" in options)
-            and not ("full_background_file" in options)
+            or "partial_background_file" not in options
+            and "full_background_file" not in options
         ), "partial_background_file and full_background_file are not supported anymore"
         if agents is not None:
             assert agents, "agents must be provided"
             assert len(agents) == 2, "Only supporting two agents right now"
             agent_names = list(agents.keys())
             agent_goals = self.profile.agent_goals
-            assert (
-                len(agent_goals) == 2
-            ), "Only supporting two agents right now"
+            assert len(agent_goals) == 2, "Only supporting two agents right now"
 
             raw_background = ScriptBackground(
                 scenario=self.profile.scenario,
                 p1_background=get_bio(
                     self.profile.relationship,
                     agents[agent_names[0]].profile,
                     agent_id=0,
@@ -255,20 +227,16 @@
 
             if lite:
                 raw_background.p1_background = ""
                 raw_background.p2_background = ""
 
             self.background = ScriptBackground(
                 scenario=render_text_for_environment(raw_background.scenario),
-                p1_background=render_text_for_environment(
-                    raw_background.p1_background
-                ),
-                p2_background=render_text_for_environment(
-                    raw_background.p2_background
-                ),
+                p1_background=render_text_for_environment(raw_background.p1_background),
+                p2_background=render_text_for_environment(raw_background.p2_background),
                 p1_goal=render_text_for_environment(raw_background.p1_goal),
                 p2_goal=render_text_for_environment(raw_background.p2_goal),
                 p1_name=raw_background.p1_name,
                 p2_name=raw_background.p2_name,
             )
         else:
             raise ValueError("agents must be provided")
@@ -278,29 +246,23 @@
         if omniscient:
             for i in range(self.num_agents):
                 agent_backgrounds.append(copy.deepcopy(self.background))
         else:
             for i in range(self.num_agents):
                 agent_backgrounds.append(
                     ScriptBackground(
-                        scenario=render_text_for_agent(
-                            raw_background.scenario, i
-                        ),
+                        scenario=render_text_for_agent(raw_background.scenario, i),
                         p1_background=render_text_for_agent(
                             raw_background.p1_background, i
                         ),
                         p2_background=render_text_for_agent(
                             raw_background.p2_background, i
                         ),
-                        p1_goal=render_text_for_agent(
-                            raw_background.p1_goal, i
-                        ),
-                        p2_goal=render_text_for_agent(
-                            raw_background.p2_goal, i
-                        ),
+                        p1_goal=render_text_for_agent(raw_background.p1_goal, i),
+                        p2_goal=render_text_for_agent(raw_background.p2_goal, i),
                         p1_name=raw_background.p1_name,
                         p2_name=raw_background.p2_name,
                     )
                 )
         background_for_a = agent_backgrounds[0]
         background_for_b = agent_backgrounds[1]
 
@@ -319,17 +281,15 @@
             for agent in self.agents
         }
         self.turn_number = 0
         self.action_mask = [False for _ in self.agents]
         if self.action_order == "round-robin":
             self.action_mask[0] = True
         elif self.action_order == "random":
-            self.action_mask[
-                random.randint(0, len(self.action_mask) - 1)
-            ] = True
+            self.action_mask[random.randint(0, len(self.action_mask) - 1)] = True
         else:
             self.action_mask = [True for _ in self.agents]
 
         self.recv_message("Environment", self.background)
 
         return {
             self.background.p1_name: Observation(
@@ -372,44 +332,38 @@
                     int(action["action_type"])
                 ]
                 complied_actions[key] = AgentAction.parse_obj(action)
 
         # Masking actions from agent that are in turn
         for idx, agent in enumerate(self.agents):
             if not self.action_mask[idx]:
-                complied_actions[agent] = AgentAction(
-                    action_type="none", argument=""
-                )
+                complied_actions[agent] = AgentAction(action_type="none", argument="")
 
         self.recv_message(
             "Environment", SimpleMessage(message=f"Turn #{self.turn_number}")
         )
         for agent, action in complied_actions.items():
             self.recv_message(agent, action)
 
         response = unweighted_aggregate_evaluate(
             list(
                 itertools.chain(
                     *(
-                        evaluator(
-                            turn_number=self.turn_number, messages=self.inbox
-                        )
+                        evaluator(turn_number=self.turn_number, messages=self.inbox)
                         for evaluator in self.evaluators
                     )
                 )
             )
         )
 
         self.action_mask = [False for _ in self.agents]
         if self.action_order == "round-robin":
             self.action_mask[self.turn_number % len(self.action_mask)] = True
         elif self.action_order == "random":
-            self.action_mask[
-                random.randint(0, len(self.action_mask) - 1)
-            ] = True
+            self.action_mask[random.randint(0, len(self.action_mask) - 1)] = True
         else:
             self.action_mask = [True for _ in self.agents]
         obs = _actions_to_natural_language(complied_actions)
         return (
             {
                 self.background.p1_name: Observation(
                     last_turn=render_text_for_agent(obs, agent_id=0),
@@ -486,17 +440,15 @@
                     int(action["action_type"])
                 ]
                 complied_actions[key] = AgentAction.parse_obj(action)
 
         # Masking actions from agent that are in turn
         for idx, agent in enumerate(self.agents):
             if not self.action_mask[idx]:
-                complied_actions[agent] = AgentAction(
-                    action_type="none", argument=""
-                )
+                complied_actions[agent] = AgentAction(action_type="none", argument="")
 
         self.recv_message(
             "Environment", SimpleMessage(message=f"Turn #{self.turn_number}")
         )
         for agent, action in complied_actions.items():
             self.recv_message(agent, action)
 
@@ -540,32 +492,32 @@
             elif terminal_response.comments:
                 response.comments = terminal_response.comments
 
         self.action_mask = [False for _ in self.agents]
         if self.action_order == "round-robin":
             self.action_mask[self.turn_number % len(self.action_mask)] = True
         elif self.action_order == "random":
-            self.action_mask[
-                random.randint(0, len(self.action_mask) - 1)
-            ] = True
+            self.action_mask[random.randint(0, len(self.action_mask) - 1)] = True
         else:
             self.action_mask = [True for _ in self.agents]
         obs = _actions_to_natural_language(complied_actions)
         info = {
             self.background.p1_name: {
                 "comments": response.comments or "",
                 "complete_rating": response.p1_rate or 0,
             },
             self.background.p2_name: {
                 "comments": response.comments or "",
                 "complete_rating": response.p2_rate or 0,
             },
         }
         if response.terminated:
-            info["rewards_prompt"] = {"overall_prompt": self.terminal_evaluators[0].prompt}  # type: ignore
+            info["rewards_prompt"] = {
+                "overall_prompt": self.terminal_evaluators[0].prompt  # type: ignore
+            }
 
         return (
             {
                 self.background.p1_name: Observation(
                     last_turn=render_text_for_agent(obs, agent_id=0),
                     turn_number=self.turn_number,
                     available_actions=list(self.available_action_types)
```

### Comparing `sotopia-0.0.6/sotopia/generation_utils/generate.py` & `sotopia-0.0.7/sotopia/generation_utils/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,79 +1,92 @@
 import logging
 import re
-from typing import TypeVar, cast
+from typing import Any, TypeVar
 
 import gin
 from beartype import beartype
 from beartype.typing import Type
-from langchain.callbacks import StdOutCallbackHandler
 from langchain.chains import LLMChain
-from langchain.chat_models import ChatOpenAI
-from langchain.llms import OpenAI
 from langchain.output_parsers import PydanticOutputParser
 from langchain.prompts import (
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
     PromptTemplate,
 )
-from langchain.schema import (
-    BaseOutputParser,
-    HumanMessage,
-    OutputParserException,
-)
-from pydantic import BaseModel, Field, validator
+from langchain.schema import BaseOutputParser, OutputParserException
+from langchain_community.chat_models import ChatLiteLLM
+from pydantic import BaseModel, Field
 from rich import print
-from rich.logging import RichHandler
 from typing_extensions import Literal
 
 from sotopia.database import EnvironmentProfile, RelationshipProfile
-from sotopia.messages import (
-    ActionType,
-    AgentAction,
-    ScriptBackground,
-    ScriptEnvironmentResponse,
-)
+from sotopia.messages import ActionType, AgentAction, ScriptBackground
 from sotopia.messages.message_classes import (
     ScriptInteraction,
     ScriptInteractionReturnType,
-    SimpleMessage,
 )
 from sotopia.utils import format_docstring
 
 from .langchain_callback_handler import LoggingCallbackHandler
-from .llama2 import Llama2
 
 log = logging.getLogger("generate")
 logging_handler = LoggingCallbackHandler("langchain")
 
 LLM_Name = Literal[
     "togethercomputer/llama-2-7b-chat",
     "togethercomputer/llama-2-70b-chat",
     "togethercomputer/mpt-30b-chat",
     "gpt-3.5-turbo",
+    "gpt-3.5-turbo-finetuned",
+    "gpt-3.5-turbo-ft-MF",
     "text-davinci-003",
     "gpt-4",
     "gpt-4-turbo",
     "human",
     "redis",
+    "mistralai/Mixtral-8x7B-Instruct-v0.1",
+    "together_ai/togethercomputer/llama-2-7b-chat",
+    "together_ai/togethercomputer/falcon-7b-instruct",
+    "groq/llama3-70b-8192",
 ]
 
 OutputType = TypeVar("OutputType", bound=object)
 
 
+class PatchedChatLiteLLM(ChatLiteLLM):
+    max_tokens: int | None = None  # type: ignore
+
+    @property
+    def _default_params(self) -> dict[str, Any]:
+        """Get the default parameters for calling OpenAI API."""
+        set_model_value = self.model
+        if self.model_name is not None:
+            set_model_value = self.model_name
+
+        params = {
+            "model": set_model_value,
+            "force_timeout": self.request_timeout,
+            "stream": self.streaming,
+            "n": self.n,
+            "temperature": self.temperature,
+            "custom_llm_provider": self.custom_llm_provider,
+            **self.model_kwargs,
+        }
+        if self.max_tokens is not None:
+            params["max_tokens"] = self.max_tokens
+
+        return params
+
+
 class EnvResponse(BaseModel):
     reasoning: str = Field(
         description="first reiterate agents' social goals and then reason about what agents say/do and whether that aligns with their goals."
     )
-    p1_rate: int = Field(
-        description="rating of participant 1, on the scale of 0 to 9"
-    )
-    p2_rate: int = Field(
-        description="rating of participant 2, on the scale of 0 to 9"
-    )
+    p1_rate: int = Field(description="rating of participant 1, on the scale of 0 to 9")
+    p2_rate: int = Field(description="rating of participant 2, on the scale of 0 to 9")
 
 
 class EnvResponsePydanticOutputParser(PydanticOutputParser[EnvResponse]):
     def __init__(self, pydantic_object: Type[BaseModel] = EnvResponse) -> None:
         super(EnvResponsePydanticOutputParser, self).__init__(
             pydantic_object=pydantic_object
         )
@@ -115,17 +128,15 @@
 
     def parse(self, output: str) -> list[int]:
         try:
             if ":" in output:
                 output = output.split(":")[1]
             result = [int(x) for x in output.split(" ") if x]
             if self.number_of_int and len(result) != self.number_of_int:
-                msg = (
-                    f"Expect {self.number_of_int} integers, got {len(result)}"
-                )
+                msg = f"Expect {self.number_of_int} integers, got {len(result)}"
                 raise OutputParserException(msg)
             if self.range_of_int:
                 for x in result:
                     if x < self.range_of_int[0] or x > self.range_of_int[1]:
                         msg = f"Expect integers within the range of {self.range_of_int}, got {result}"
                         raise OutputParserException(msg)
             return result
@@ -199,17 +210,15 @@
 
 
 class ScriptOutputParser(BaseOutputParser[ScriptInteractionReturnType]):
     agent_names: list[str] = Field(
         description="The names of the two agents in the conversation"
     )
     background: str = Field(description="The background of the conversation")
-    single_turn: bool = Field(
-        description="Whether the output is a single turn"
-    )
+    single_turn: bool = Field(description="Whether the output is a single turn")
 
     def get_format_instructions(self) -> str:
         if self.single_turn:
             return r"""For one turn, only write the next step of this agent. You should follow the structure. The format looks like this: Turn #0 \n[participant's name] [action].
 This means you can only generate two lines in one turn.
 
 You can use different types of actions in the [action] part, but PLEASE follows the rule STRICTLY. Remember to include the square brackets when doing an action as stated in the instructions.
@@ -262,115 +271,84 @@
         try:
             # try to parse the output
             parsed_interaction = interaction.parse(
                 agent_names=agent_names, background=self.background
             )
             return parsed_interaction
         except Exception as e:
-            print(
-                f"Exception {e}: the output format is not correct. Reformatting "
-            )
+            print(f"Exception {e}: the output format is not correct. Reformatting ")
             reformat_parsed_result = format_bad_output_for_script(
                 ill_formed_output=output,
                 format_instructions=self.get_format_instructions(),
                 agents=agent_names,
             )
             print("Reformatted output: ", reformat_parsed_result)
-            interaction = ScriptInteraction(
-                interactions=reformat_parsed_result
-            )
+            interaction = ScriptInteraction(interactions=reformat_parsed_result)
             parsed_interaction = interaction.parse(
                 agent_names=agent_names, background=self.background
             )
             return parsed_interaction
 
     @property
     def _type(self) -> str:
         """Return the type key."""
         return "str"
 
 
-def _return_fixed_model_version(
-    model_name: Literal["gpt-3.5-turbo", "gpt-4", "gpt-4-turbo"]
-) -> str:
-    return {
-        "gpt-3.5-turbo": "gpt-3.5-turbo-0613",
-        "gpt-4": "gpt-4-0613",
-        "gpt-4-turbo": "gpt-4-1106-preview",
-    }[model_name]
+def _return_fixed_model_version(model_name: str) -> str:
+    if model_name in [
+        "gpt-3.5-turbo",
+        "gpt-3.5-turbo-finetuned",
+        "gpt-3.5-turbo-ft-MF",
+        "gpt-4",
+        "gpt-4-turbo",
+    ]:
+        return {
+            "gpt-3.5-turbo": "gpt-3.5-turbo-0613",
+            "gpt-3.5-turbo-finetuned": "ft:gpt-3.5-turbo-0613:academicscmu::8nY2zgdt",
+            "gpt-3.5-turbo-ft-MF": "ft:gpt-3.5-turbo-0613:academicscmu::8nuER4bO",
+            "gpt-4": "gpt-4-0613",
+            "gpt-4-turbo": "gpt-4-1106-preview",
+        }[model_name]
+    else:
+        return model_name
 
 
 @gin.configurable
 @beartype
 def obtain_chain(
-    model_name: LLM_Name,
+    model_name: str,
     template: str,
     input_variables: list[str],
     temperature: float = 0.7,
     max_retries: int = 6,
 ) -> LLMChain:
     """
     Using langchain to sample profiles for participants
     """
-    match model_name:
-        case "gpt-3.5-turbo" | "gpt-4" | "gpt-4-turbo":
-            human_message_prompt = HumanMessagePromptTemplate(
-                prompt=PromptTemplate(
-                    template=template,
-                    input_variables=input_variables,
-                )
-            )
-            chat_prompt_template = ChatPromptTemplate.from_messages(
-                [human_message_prompt]
-            )
-            chat = ChatOpenAI(
-                model_name=_return_fixed_model_version(model_name),
-                temperature=temperature,
-                max_retries=max_retries,
-            )
-            chain = LLMChain(llm=chat, prompt=chat_prompt_template)
-            return chain
-        case "text-davinci-003":
-            # Warning: no interactive mode for 003
-            llm = OpenAI(
-                model_name=model_name,
-                temperature=temperature,
-                max_retries=max_retries,
-            )
-            prompt = PromptTemplate(
-                input_variables=input_variables,
-                template=template,
-            )
-            chain = LLMChain(llm=llm, prompt=prompt)
-            return chain
-        case "togethercomputer/llama-2-7b-chat" | "togethercomputer/llama-2-70b-chat" | "togethercomputer/mpt-30b-chat":
-            human_message_prompt = HumanMessagePromptTemplate(
-                prompt=PromptTemplate(
-                    template=template,
-                    input_variables=input_variables,
-                )
-            )
-            chat_prompt_template = ChatPromptTemplate.from_messages(
-                [human_message_prompt]
-            )
-            together_llm = Llama2(
-                model_name=model_name, temperature=temperature
-            )
-            chain = LLMChain(llm=together_llm, prompt=chat_prompt_template)
-            return chain
-        case _:
-            raise ValueError(f"Invalid model name: {model_name}")
+    model_name = _return_fixed_model_version(model_name)
+    chat = PatchedChatLiteLLM(
+        model=model_name,
+        temperature=temperature,
+        max_retries=max_retries,
+    )
+    human_message_prompt = HumanMessagePromptTemplate(
+        prompt=PromptTemplate(template=template, input_variables=input_variables)
+    )
+    chat_prompt_template = ChatPromptTemplate.from_messages([human_message_prompt])
+    chain = LLMChain(llm=chat, prompt=chat_prompt_template)
+    return chain
 
 
 @beartype
 def format_bad_output_for_script(
     ill_formed_output: str,
     format_instructions: str,
     agents: list[str],
-    model_name: LLM_Name = "gpt-3.5-turbo",
+    model_name: str = "gpt-3.5-turbo",
 ) -> str:
     template = """
     Given the string that can not be parsed by a parser, reformat it to a string that can be parsed by the parser which uses the following format instructions. Do not add or delete any information.
     Small tip: for every round of conversation, first determine the name and the case, and whether this line contains errors. Correct it if necessary.
 
     Format instructions: {format_instructions}
 
@@ -396,15 +374,15 @@
     return reformat
 
 
 @beartype
 def format_bad_output(
     ill_formed_output: str,
     format_instructions: str,
-    model_name: LLM_Name = "gpt-3.5-turbo",
+    model_name: str = "gpt-3.5-turbo",
 ) -> str:
     template = """
     Given the string that can not be parsed by json parser, reformat it to a string that can be parsed by json parser.
     Original string: {ill_formed_output}
 
     Format instructions: {format_instructions}
 
@@ -422,38 +400,35 @@
     reformat = chain.predict([logging_handler], **input_values)
     log.info(f"Reformated output: {reformat}")
     return reformat
 
 
 @beartype
 def generate(
-    model_name: LLM_Name,
+    model_name: str,
     template: str,
     input_values: dict[str, str],
     output_parser: BaseOutputParser[OutputType],
     temperature: float = 0.7,
 ) -> OutputType:
     input_variables = re.findall(r"{(.*?)}", template)
-    assert set(input_variables) == set(
-        list(input_values.keys()) + ["format_instructions"]
-    ) or set(input_variables) == set(
-        list(input_values.keys())
+    assert (
+        set(input_variables) == set(list(input_values.keys()) + ["format_instructions"])
+        or set(input_variables) == set(list(input_values.keys()))
     ), f"The variables in the template must match input_values except for format_instructions. Got {sorted(input_values.keys())}, expect {sorted(input_variables)}"
     # process template
     template = format_docstring(template)
     chain = obtain_chain(
         model_name=model_name,
         template=template,
         input_variables=input_variables,
         temperature=temperature,
     )
     if "format_instructions" not in input_values:
-        input_values[
-            "format_instructions"
-        ] = output_parser.get_format_instructions()
+        input_values["format_instructions"] = output_parser.get_format_instructions()
     result = chain.predict([logging_handler], **input_values)
     try:
         parsed_result = output_parser.parse(result)
     except KeyboardInterrupt:
         raise KeyboardInterrupt
     except Exception as e:
         log.debug(
@@ -467,38 +442,35 @@
     log.info(f"Generated result: {parsed_result}")
     return parsed_result
 
 
 @gin.configurable
 @beartype
 async def agenerate(
-    model_name: LLM_Name,
+    model_name: str,
     template: str,
     input_values: dict[str, str],
     output_parser: BaseOutputParser[OutputType],
     temperature: float = 0.7,
 ) -> tuple[OutputType, str]:
     input_variables = re.findall(r"{(.*?)}", template)
-    assert set(input_variables) == set(
-        list(input_values.keys()) + ["format_instructions"]
-    ) or set(input_variables) == set(
-        list(input_values.keys())
+    assert (
+        set(input_variables) == set(list(input_values.keys()) + ["format_instructions"])
+        or set(input_variables) == set(list(input_values.keys()))
     ), f"The variables in the template must match input_values except for format_instructions. Got {sorted(input_values.keys())}, expect {sorted(input_variables)}"
     # process template
     template = format_docstring(template)
     chain = obtain_chain(
         model_name=model_name,
         template=template,
         input_variables=input_variables,
         temperature=temperature,
     )
     if "format_instructions" not in input_values:
-        input_values[
-            "format_instructions"
-        ] = output_parser.get_format_instructions()
+        input_values["format_instructions"] = output_parser.get_format_instructions()
     result = await chain.apredict([logging_handler], **input_values)
     prompt = logging_handler.retrive_prompt()
     try:
         parsed_result = output_parser.parse(result)
     except Exception as e:
         if isinstance(output_parser, ScriptOutputParser):
             raise e  # the problem has been handled in the parser
@@ -513,15 +485,15 @@
     log.info(f"Generated result: {parsed_result}")
     return parsed_result, prompt
 
 
 # deprecated function
 @beartype
 def generate_episode(
-    model_name: LLM_Name,
+    model_name: str,
     participants: str = "Jack (a greedy person), Rose",
     topic: str = "lawsuit",
     extra_info: str = "",
 ) -> EnvResponse:
     """
     Using langchain to generate an example episode
     """
@@ -542,15 +514,15 @@
         output_parser=EnvResponsePydanticOutputParser(),
     )
 
 
 @gin.configurable
 @beartype
 async def agenerate_env_profile(
-    model_name: LLM_Name,
+    model_name: str,
     inspiration_prompt: str = "asking my boyfriend to stop being friends with his ex",
     examples: str = "",
     temperature: float = 0.7,
 ) -> tuple[EnvironmentProfile, str]:
     """
     Using langchain to generate the background
     """
@@ -570,15 +542,15 @@
         output_parser=PydanticOutputParser(pydantic_object=EnvironmentProfile),
         temperature=temperature,
     )
 
 
 @beartype
 async def agenerate_relationship_profile(
-    model_name: LLM_Name,
+    model_name: str,
     agents_profiles: list[str],
 ) -> tuple[RelationshipProfile, str]:
     """
     Using langchain to generate the background
     """
     agent_profile = "\n".join(agents_profiles)
     return await agenerate(
@@ -587,23 +559,21 @@
         {agent_profile}
         Please use the following format:
         {format_instructions}
         """,
         input_values=dict(
             agent_profile=agent_profile,
         ),
-        output_parser=PydanticOutputParser(
-            pydantic_object=RelationshipProfile
-        ),
+        output_parser=PydanticOutputParser(pydantic_object=RelationshipProfile),
     )
 
 
 @beartype
 async def agenerate_enviroment_profile(
-    model_name: LLM_Name,
+    model_name: str,
     inspiration_prompt: str = "asking my boyfriend to stop being friends with his ex",
     examples: str = "",
 ) -> tuple[EnvironmentProfile, str]:
     """
     Using langchain to generate the background
     """
     return await agenerate(
@@ -621,15 +591,15 @@
         ),
         output_parser=PydanticOutputParser(pydantic_object=EnvironmentProfile),
     )
 
 
 @beartype
 def fill_in_background(
-    model_name: LLM_Name,
+    model_name: str,
     partial_background: ScriptBackground,
 ) -> ScriptBackground:
     """
     Fill in the missing information of the background
     """
     return generate(
         model_name=model_name,
@@ -643,15 +613,15 @@
         ),
         output_parser=PydanticOutputParser(pydantic_object=ScriptBackground),
     )
 
 
 @beartype
 def generate_action(
-    model_name: LLM_Name,
+    model_name: str,
     history: str,
     turn_number: int,
     action_types: list[ActionType],
     agent: str,
     goal: str,
 ) -> AgentAction:
     """
@@ -678,21 +648,21 @@
                 history=history,
                 action_list=" ".join(action_types),
             ),
             output_parser=PydanticOutputParser(pydantic_object=AgentAction),
         )
     except KeyboardInterrupt:
         raise KeyboardInterrupt
-    except:
+    except Exception:
         return AgentAction(action_type="none", argument="")
 
 
 @beartype
 def generate_action_speak(
-    model_name: LLM_Name,
+    model_name: str,
     history: str,
     turn_number: int,
     action_types: list[ActionType],
     agent: str,
     goal: str,
 ) -> AgentAction:
     """
@@ -723,22 +693,22 @@
         utterance = utterance.replace(f"{agent} said:", "")
         utterance = utterance.replace(f"Turn #{turn_number}:", "")
         utterance = utterance.strip()
         utterance = utterance.replace('"', "")
         return AgentAction(action_type="speak", argument=utterance)
     except KeyboardInterrupt:
         raise KeyboardInterrupt
-    except:
+    except Exception:
         return AgentAction(action_type="none", argument="")
 
 
 @gin.configurable
 @beartype
 async def agenerate_action(
-    model_name: LLM_Name,
+    model_name: str,
     history: str,
     turn_number: int,
     action_types: list[ActionType],
     agent: str,
     goal: str,
     temperature: float = 0.7,
     script_like: bool = False,
@@ -776,35 +746,34 @@
                 {action_list}.
                 Note: You can "leave" this conversation if 1. you have achieved your social goals, 2. this conversation makes you uncomfortable, 3. you find it uninteresting/you lose your patience, 4. or for other reasons you want to leave.
 
                 Please only generate a JSON string including the action type and the argument.
                 Your action should follow the given format:
                 {format_instructions}
             """
-
         return await agenerate(
             model_name=model_name,
             template=template,
             input_values=dict(
                 agent=agent,
                 turn_number=str(turn_number),
                 history=history,
                 action_list=" ".join(action_types),
             ),
             output_parser=PydanticOutputParser(pydantic_object=AgentAction),
             temperature=temperature,
         )
-    except:
+    except Exception:
         return AgentAction(action_type="none", argument=""), ""
 
 
 @gin.configurable
 @beartype
 async def agenerate_script(
-    model_name: LLM_Name,
+    model_name: str,
     background: ScriptBackground,
     temperature: float = 0.7,
     agent_names: list[str] = [],
     agent_name: str = "",
     history: str = "",
     single_step: bool = False,
 ) -> tuple[ScriptInteractionReturnType, str]:
@@ -870,15 +839,15 @@
             ScriptInteraction.default_value_for_return_type()
         )
         return (return_default_value, "")
 
 
 @beartype
 def process_history(
-    script: ScriptBackground | EnvResponse | dict[str, AgentAction]
+    script: ScriptBackground | EnvResponse | dict[str, AgentAction],
 ) -> str:
     """
     Format the script background
     """
     result = ""
     if isinstance(script, ScriptBackground | EnvResponse):
         script = script.dict()
@@ -886,17 +855,15 @@
     for key, value in script.items():
         if value:
             result += f"{key}: {value} \n"
     return result
 
 
 @beartype
-def generate_init_profile(
-    model_name: LLM_Name, basic_info: dict[str, str]
-) -> str:
+def generate_init_profile(model_name: str, basic_info: dict[str, str]) -> str:
     """
     Using langchain to generate the background
     """
     return generate(
         model_name=model_name,
         template="""Please expand a fictional background for {name}. Here is the basic information:
             {name}'s age: {age}
@@ -926,15 +893,15 @@
             secret=basic_info["secret"],
         ),
         output_parser=StrOutputParser(),
     )
 
 
 @beartype
-def convert_narratives(model_name: LLM_Name, narrative: str, text: str) -> str:
+def convert_narratives(model_name: str, narrative: str, text: str) -> str:
     if narrative == "first":
         return generate(
             model_name=model_name,
             template="""Please convert the following text into a first-person narrative.
             e.g, replace name, he, she, him, her, his, and hers with I, me, my, and mine.
             {text}""",
             input_values=dict(text=text),
@@ -950,15 +917,15 @@
             output_parser=StrOutputParser(),
         )
     else:
         raise ValueError(f"Narrative {narrative} is not supported.")
 
 
 @beartype
-def generate_goal(model_name: LLM_Name, background: str) -> str:
+def generate_goal(model_name: str, background: str) -> str:
     """
     Using langchain to generate the background
     """
     return generate(
         model_name=model_name,
         template="""Please generate your goal based on the background:
             {background}
```

### Comparing `sotopia-0.0.6/sotopia/generation_utils/langchain_callback_handler.py` & `sotopia-0.0.7/sotopia/generation_utils/langchain_callback_handler.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.6/sotopia/generation_utils/llama2.py` & `sotopia-0.0.7/sotopia/generation_utils/llama2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 from __future__ import annotations
 
 import logging
-import os
-import sys
-from typing import (
-    Any,
-    Callable,
-    Coroutine,
-    Dict,
-    List,
-    Mapping,
-    Optional,
-    Tuple,
-    Union,
-    cast,
-)
+from typing import Any, Dict, List, Mapping, Optional, Tuple, cast
 
 import together
 from langchain.callbacks.manager import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain.chat_models.base import BaseChatModel
@@ -28,22 +15,15 @@
     ChatGeneration,
     ChatMessage,
     ChatResult,
     HumanMessage,
     SystemMessage,
 )
 from langchain.utils import get_from_dict_or_env
-from pydantic import Extra, Field, root_validator
-from tenacity import (
-    before_sleep_log,
-    retry,
-    retry_if_exception_type,
-    stop_after_attempt,
-    wait_exponential,
-)
+from pydantic import Extra, root_validator
 
 
 def _convert_message_to_dict(message: BaseMessage) -> dict[str, Any]:
     if isinstance(message, ChatMessage):
         message_dict = {"role": message.role, "content": message.content}
     elif isinstance(message, HumanMessage):
         message_dict = {"role": "user", "content": message.content}
@@ -76,17 +56,15 @@
     tag_sep = ": "
     conv_sep = "\n"
 
     if dialog[0]["role"] == "system":
         dialog = [
             {
                 "role": dialog[1]["role"],
-                "content": dialog[0]["content"]
-                + conv_sep
-                + dialog[1]["content"],
+                "content": dialog[0]["content"] + conv_sep + dialog[1]["content"],
             }
         ] + dialog[2:]
     assert all([msg["role"] == "user" for msg in dialog[::2]]) and all(
         [msg["role"] == "assistant" for msg in dialog[1::2]]
     ), (
         "model only supports 'system', 'user' and 'assistant' roles, "
         "starting with 'system', then 'user' and alternating (u/a/u/a/u...)"
@@ -123,17 +101,15 @@
         """Configuration for this pydantic object."""
 
         extra = Extra.ignore
 
     @root_validator(pre=True)
     def build_extra(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Build extra kwargs from additional params that were passed in."""
-        all_required_field_names = {
-            field.alias for field in cls.__fields__.values()
-        }
+        all_required_field_names = {field.alias for field in cls.__fields__.values()}
 
         extra = values.get("model_kwargs", {})
         for field_name in list(values):
             if field_name not in all_required_field_names:
                 if field_name in extra:
                     raise ValueError(f"Found {field_name} supplied twice.")
                 extra[field_name] = values.pop(field_name)
@@ -178,17 +154,15 @@
     ) -> Tuple[str, Dict[str, Any]]:
         params: Dict[str, Any] = {
             **{"model": self.model_name},
             **self._default_params,
         }
         if stop is not None:
             if "stop" in params:
-                raise ValueError(
-                    "`stop` found in both the input and default params."
-                )
+                raise ValueError("`stop` found in both the input and default params.")
             params["stop"] = stop
         message_dicts = [_convert_message_to_dict(m) for m in messages]
         message_prompt = _make_prompt_from_dict(message_dicts)
         return message_prompt, params
 
     def _create_chat_result(self, response: Mapping[str, Any]) -> ChatResult:
         generations = []
```

### Comparing `sotopia-0.0.6/sotopia/messages/message_classes.py` & `sotopia-0.0.7/sotopia/messages/message_classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import re
 from typing import Literal, cast
 
 from pydantic import BaseModel, Field
 
 from sotopia.utils import format_docstring
 
-ActionType = Literal[
-    "none", "speak", "non-verbal communication", "action", "leave"
-]
+ActionType = Literal["none", "speak", "non-verbal communication", "action", "leave"]
 
 
 class Message(BaseModel):
     """
     An interface for messages.
     There is only one required method: to_natural_language
     """
@@ -30,17 +28,15 @@
     def to_natural_language(self) -> str:
         return self.message
 
 
 class Observation(Message):
     last_turn: str = Field(description="the last turn of the conversation")
     turn_number: int = Field(description="the turn number of the conversation")
-    available_actions: list[ActionType] = Field(
-        description="the available actions"
-    )
+    available_actions: list[ActionType] = Field(description="the available actions")
 
     def to_natural_language(self) -> str:
         if self.turn_number == 0:
             return f"\n{self.last_turn}\nConversation Starts:\n"
         else:
             return f"Turn #{self.turn_number-1}: {self.last_turn}\n"
 
@@ -51,21 +47,24 @@
     p2_name: str = Field(description="name of participant 2")
     p1_background: str = Field(description="background of participant 1")
     p2_background: str = Field(description="background of participant 2")
     p1_goal: str = Field(description="goal of participant 1")
     p2_goal: str = Field(description="goal of participant 2")
 
     def to_natural_language(self) -> str:
-        if self.p1_background and self.p2_background:
+        if self.p1_background or self.p2_background:
+            p1_background = self.p1_background if self.p1_background else "Unknown"
+            p2_background = self.p2_background if self.p2_background else "Unknown"
+            # Not using AND, since in stranger relation the background is not visible
             return format_docstring(
                 f"""Here is the context of this interaction:
             Scenario: {self.scenario}
             Participants: {self.p1_name} and {self.p2_name}
-            {self.p1_name}'s background: {self.p1_background}
-            {self.p2_name}'s background: {self.p2_background}
+            {self.p1_name}'s background: {p1_background}
+            {self.p2_name}'s background: {p2_background}
             {self.p1_name}'s goal: {self.p1_goal}
             {self.p2_name}'s goal: {self.p2_goal}
             """
             )
         else:
             return format_docstring(
                 f"""Here is the context of this interaction:
@@ -177,17 +176,15 @@
     )
 
     def to_natural_language(self) -> str:
         return self.interactions
 
     def parse(
         self, agent_names: list[str], background: str
-    ) -> tuple[
-        list[list[tuple[str, str, Message]]], list[tuple[str, Message]]
-    ]:
+    ) -> tuple[list[list[tuple[str, str, Message]]], list[tuple[str, Message]]]:
         interaction = self.interactions
         # print("Interaction: ", interaction)
         lines = self.split_by_turn(interaction)
 
         agent_results = []
         results: list[list[tuple[str, str, Message]]] = [
             [
@@ -205,20 +202,18 @@
         ]
 
         for line_idx, line in enumerate(lines):
             try:
                 res = self.parse_single_dialogue(line)
                 action: AgentAction = cast(AgentAction, res["action"])
                 argument: str = cast(str, res["argument"])
-                turn: int = cast(int, res["turn"])
+                cast(int, res["turn"])
                 name: str = cast(str, res["name"])
 
-                parsed_action = AgentAction(
-                    action_type=action, argument=argument
-                )
+                parsed_action = AgentAction(action_type=action, argument=argument)
                 if name not in agent_names:
                     print(
                         f"The name of the agent, {name}, is not in the list of agent names, {agent_names}"
                     )
                     name = agent_names[
                         line_idx % 2
                     ]  # TODO Not sure what name to be set here
@@ -247,17 +242,15 @@
                     for name in agent_names
                 ]
                 + [
                     (name, "Environment", parsed_action),
                     (
                         inactive_agent_name,
                         "Environment",
-                        AgentAction(
-                            action_type="none", argument="did nothing"
-                        ),
+                        AgentAction(action_type="none", argument="did nothing"),
                     ),
                 ]
             )
 
             agent_results.append((name, parsed_action))
         # print("Parsed agent results: ", agent_results)
         return (results, agent_results)  # type: ignore
@@ -272,17 +265,15 @@
             r"Turn #?(\d+):?\s*\n((?:[A-Z]['a-z]* ?)+)", dialogue
         )
 
         if not match_turn_name:
             raise ValueError(
                 f"The dialogue does not match the expected format: {dialogue}"
             )
-            return (
-                None  # TODO Which should we use, return None or raise error?
-            )
+            return None  # TODO Which should we use, return None or raise error?
 
         turn, name = match_turn_name.groups()
         action_content = dialogue[
             len(match_turn_name.group(0)) :
         ].strip()  # Extract the action content
 
         # Check for different action types
@@ -313,25 +304,25 @@
         return parsed_item
 
     def split_by_turn(self, input_string: str) -> list[str]:
         """Split the input dialogue string by turn and return a list of dialogues."""
         # Split using 'Turn #' as delimiter, but keep the delimiter in the results
         dialogues = re.split(r"(?=Turn #?\d+)", input_string)
         # Remove any empty strings and strip whitespace
-        dialogues = [
-            dialogue.strip() for dialogue in dialogues if dialogue.strip()
-        ]
-        dialogues = [
-            dialogue for dialogue in dialogues if dialogue.startswith("Turn")
-        ]
+        dialogues = [dialogue.strip() for dialogue in dialogues if dialogue.strip()]
+        dialogues = [dialogue for dialogue in dialogues if dialogue.startswith("Turn")]
         # Change from Turn #x to Turn (#)x (# is optional)
         dialogues[-1] = "\n".join(
             dialogues[-1].split("\n")[:2]
         )  # Discard further input in the last turn
-        # print("Dialogues: ", dialogues)
+
+        for dialogue in dialogues:
+            # TODO this is current workaround for the issue of multiple agents in one turn
+            if len(dialogue.split("\n")) >= 3:
+                raise ValueError("Only one agent can act per turn.")
         return dialogues
 
     @staticmethod
     def default_value_for_return_type() -> ScriptInteractionReturnType:
         results_1: list[list[tuple[str, str, Message]]] = [
             [
                 (
```

### Comparing `sotopia-0.0.6/sotopia/renderers/base.py` & `sotopia-0.0.7/sotopia/renderers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Any
-
 from pydantic import BaseModel, Field, validator
 
 
 class RenderContext(BaseModel):
     viewer: str = Field(
         default="human",
         description="The viewer of the rendered string."
@@ -21,15 +19,15 @@
 
     @validator("viewer")
     def viewer_must_be_valid(cls, v: str) -> str:
         if v.startswith("agent_"):
             try:
                 agent_idx = int(v.split("_")[1])
                 assert agent_idx >= 0
-            except:
+            except Exception:
                 raise ValueError(
                     "If viewer is an agent, it must be of the form agent_i, where i is a non-negative integer."
                 )
         elif v not in ["human", "environment"]:
             raise ValueError(
                 "Viewer must be one of ['human', 'environment', 'agent_i']"
                 "where i is a non-negative integer, the index of the agent in the episode log."
```

### Comparing `sotopia-0.0.6/sotopia/renderers/xml_renderer.py` & `sotopia-0.0.7/sotopia/renderers/xml_renderer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-"""XML Renderer for background, goal, observation, etc.
-"""
+"""XML Renderer for background, goal, observation, etc."""
+
 from io import StringIO
 from typing import cast
 
 from beartype.door import is_bearable
 from lxml import etree
 
 from .base import BaseRenderer, RenderContext
 
 
 def _render_xml(xml_node: etree._Element | str, context: RenderContext) -> str:
     if isinstance(xml_node, str):
         return xml_node
     else:
-        if (
-            xml_node.tag in ["root", "p"]
-            or xml_node.tag in context.tags_to_render
-        ):
+        if xml_node.tag in ["root", "p"] or xml_node.tag in context.tags_to_render:
             if context.viewer.startswith("agent_"):
                 # For each agent, we only render the messages viewable by that agent
                 all_visible_children = xml_node.xpath(
                     f"./node()[@viewer='{context.viewer}'] | ./node()[not(@viewer)]"
                 )
-                assert is_bearable(
-                    all_visible_children, list[etree._Element | str]
-                )
+                assert is_bearable(all_visible_children, list[etree._Element | str])
                 cast(list[etree._Element | str], all_visible_children)
                 return "".join(
-                    _render_xml(child, context) for child in all_visible_children  # type: ignore[attr-defined]
+                    _render_xml(child, context)
+                    for child in all_visible_children  # type: ignore[attr-defined]
                 )
             elif context.viewer == "human":
                 # For human, we render the raw xml
-                return etree.tostring(xml_node, pretty_print=True).decode(
-                    "utf-8"
-                )
+                return etree.tostring(xml_node, pretty_print=True).decode("utf-8")
             elif context.viewer == "environment":
                 # For environment, we render all text
                 all_text = xml_node.xpath("//text()")
                 return "".join(cast(list[str], all_text))
         # Add return statement for the case where none of the conditions are met
         return ""
 
@@ -63,17 +57,16 @@
                 table = str.maketrans(
                     {
                         "&": "&amp;",
                     }
                 )
                 try:
                     root = etree.parse(
-                        StringIO(
-                            f"<root>{xml_string.translate(table)}</root>"
-                        ),
+                        StringIO(f"<root>{xml_string.translate(table)}</root>"),
                         self.parser,
                     ).getroot()
                 except etree.XMLSyntaxError as e:
-                    e.add_note(f"The xml_string is {xml_string}")
-                    raise e
+                    raise etree.XMLSyntaxError(
+                        f"Failed to parse xml_string: {xml_string}"
+                    ) from e
 
         return _render_xml(root, context)
```

### Comparing `sotopia-0.0.6/sotopia/samplers/base_sampler.py` & `sotopia-0.0.7/sotopia/samplers/base_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,15 @@
     EnvironmentProfile,
 )
 from sotopia.envs.parallel import ParallelSotopiaEnv
 
 ObsType = TypeVar("ObsType")
 ActType = TypeVar("ActType")
 
-EnvAgentCombo = tuple[
-    ParallelSotopiaEnv, Sequence[BaseAgent[ObsType, ActType]]
-]
+EnvAgentCombo = tuple[ParallelSotopiaEnv, Sequence[BaseAgent[ObsType, ActType]]]
 
 
 class BaseSampler(Generic[ObsType, ActType]):
     def __init__(
         self,
         env_candidates: Sequence[EnvironmentProfile | str] | None = None,
         agent_candidates: Sequence[AgentProfile | str] | None = None,
```

### Comparing `sotopia-0.0.6/sotopia/samplers/constraint_based_sampler.py` & `sotopia-0.0.7/sotopia/samplers/constraint_based_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Any, Generator, Type, TypeVar
 
 from sotopia.agents.base_agent import BaseAgent
 from sotopia.database import (
     AgentProfile,
     EnvironmentProfile,
     RelationshipProfile,
-    RelationshipType,
 )
 from sotopia.envs.parallel import ParallelSotopiaEnv
 
 from .base_sampler import BaseSampler, EnvAgentCombo
 
 ObsType = TypeVar("ObsType")
 ActType = TypeVar("ActType")
@@ -59,28 +58,27 @@
 class ConstraintBasedSampler(BaseSampler[ObsType, ActType]):
     def sample(
         self,
         agent_classes: Type[BaseAgent[ObsType, ActType]]
         | list[Type[BaseAgent[ObsType, ActType]]],
         n_agent: int = 2,
         replacement: bool = True,
-        size: int = 10,
+        size: int = 5,
         env_params: dict[str, Any] = {},
         agents_params: list[dict[str, Any]] = [{}, {}],
     ) -> Generator[EnvAgentCombo[ObsType, ActType], None, None]:
         """
         Sample an environment and a list of agents based on the constraints of the environment.
 
         Note: Sampling without replacement is only restricted to single env candidate.
         This is due to the fact that the number of possible combinations of env and agents is huge.
         Please sample for each env separately if you want to sample without replacement.
         """
         assert (
-            not isinstance(agent_classes, list)
-            or len(agent_classes) == n_agent
+            not isinstance(agent_classes, list) or len(agent_classes) == n_agent
         ), f"agent_classes should be a list of length {n_agent} or a single agent class"
 
         if not isinstance(agent_classes, list):
             agent_classes = [agent_classes] * n_agent
         assert (
             len(agents_params) == n_agent
         ), f"agents_params should be a list of length {n_agent}"
@@ -123,41 +121,35 @@
         else:
             for _ in range(size):
                 if self.env_candidates:
                     env_profile = random.choice(self.env_candidates)
                     if isinstance(env_profile, str):
                         env_profile = EnvironmentProfile.get(env_profile)
                 else:
-                    env_profile_id = random.choice(
-                        list(EnvironmentProfile.all_pks())
-                    )
+                    env_profile_id = random.choice(list(EnvironmentProfile.all_pks()))
                     env_profile = EnvironmentProfile.get(env_profile_id)
                 env_profiles.append(env_profile)
                 env_profile_id = env_profile.pk
                 assert env_profile_id, "Env candidate must have an id"
                 agents_which_fit_scenario.append(
-                    _get_fit_agents_for_one_env(
-                        env_profile_id, agent_candidate_ids, 1
-                    )[0]
+                    _get_fit_agents_for_one_env(env_profile_id, agent_candidate_ids, 1)[
+                        0
+                    ]
                 )
 
-        assert (
-            len(env_profiles) == size
-        ), "Number of env_profiles is not equal to size"
+        assert len(env_profiles) == size, "Number of env_profiles is not equal to size"
         assert (
             len(agents_which_fit_scenario) == size
         ), "Number of agents_which_fit_scenario is not equal to size"
 
         for env_profile, agent_profile_id_list in zip(
             env_profiles, agents_which_fit_scenario
         ):
             env = ParallelSotopiaEnv(env_profile=env_profile, **env_params)
-            agent_profiles = [
-                AgentProfile.get(id) for id in agent_profile_id_list
-            ]
+            agent_profiles = [AgentProfile.get(id) for id in agent_profile_id_list]
 
             agents = [
                 agent_class(agent_profile=agent_profile, **agent_params)
                 for agent_class, agent_profile, agent_params in zip(
                     agent_classes, agent_profiles, agents_params
                 )
             ]
```

### Comparing `sotopia-0.0.6/sotopia/samplers/uniform_sampler.py` & `sotopia-0.0.7/sotopia/samplers/uniform_sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-from typing import Any, Generator, Type, TypeVar, cast
+from typing import Any, Generator, Type, TypeVar
 
 from sotopia.agents.base_agent import BaseAgent
 from sotopia.database import AgentProfile, EnvironmentProfile
 from sotopia.envs.parallel import ParallelSotopiaEnv
 
 from .base_sampler import BaseSampler, EnvAgentCombo
 
@@ -31,37 +31,32 @@
 
         Note: Currently, uniform sampling without replacement is not supported.
         This is due to the difficulty of sequentially sampling environment and agents.
         In theory, we can reject samples that have been sampled before, but this is not efficient.
         Please open an issue if you need this feature.
         """
         assert (
-            not isinstance(agent_classes, list)
-            or len(agent_classes) == n_agent
+            not isinstance(agent_classes, list) or len(agent_classes) == n_agent
         ), f"agent_classes should be a list of length {n_agent} or a single agent class"
 
         if not isinstance(agent_classes, list):
             agent_classes = [agent_classes] * n_agent
         assert (
             len(agents_params) == n_agent
         ), f"agents_params should be a list of length {n_agent}"
 
-        assert (
-            replacement
-        ), "Uniform sampling without replacement is not supported yet"
+        assert replacement, "Uniform sampling without replacement is not supported yet"
 
         for _ in range(size):
             if self.env_candidates:
                 env_profile = random.choice(self.env_candidates)
                 if isinstance(env_profile, str):
                     env_profile = EnvironmentProfile.get(env_profile)
             else:
-                env_profile_id = random.choice(
-                    list(EnvironmentProfile.all_pks())
-                )
+                env_profile_id = random.choice(list(EnvironmentProfile.all_pks()))
                 env_profile = EnvironmentProfile.get(env_profile_id)
             env = ParallelSotopiaEnv(env_profile=env_profile, **env_params)
 
             if self.agent_candidates:
                 agent_profile_candidates = self.agent_candidates
                 if len(agent_profile_candidates) < n_agent:
                     raise ValueError(
@@ -70,16 +65,15 @@
             else:
                 agent_profile_candidates_keys = list(AgentProfile.all_pks())
                 if len(agent_profile_candidates_keys) < n_agent:
                     raise ValueError(
                         f"Number of agent profile candidates ({len(agent_profile_candidates_keys)}) in database is less than number of agents ({n_agent})"
                     )
                 agent_profile_candidates = [
-                    AgentProfile.get(pk=pk)
-                    for pk in agent_profile_candidates_keys
+                    AgentProfile.get(pk=pk) for pk in agent_profile_candidates_keys
                 ]
 
             if len(agent_profile_candidates) == n_agent:
                 agent_profiles_maybe_id = agent_profile_candidates
             else:
                 agent_profiles_maybe_id = random.sample(
                     agent_profile_candidates, n_agent
```

### Comparing `sotopia-0.0.6/sotopia/server.py` & `sotopia-0.0.7/sotopia/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,51 @@
 import asyncio
-import functools
 import itertools
 import logging
-from typing import Callable, Literal, Sequence, Type, cast
+from typing import Literal, Sequence, Type, cast
 
 import gin
 import rich
 from beartype import beartype
 from tqdm.asyncio import tqdm_asyncio
 
 from sotopia.agents import (
     Agents,
     HumanAgent,
     LLMAgent,
+    RedisAgent,
     ScriptWritingAgent,
     SpeakAgent,
 )
 from sotopia.agents.base_agent import BaseAgent
 from sotopia.database import EpisodeLog
-from sotopia.database.persistent_profile import (
-    AgentProfile,
-    EnvironmentProfile,
-)
 from sotopia.envs import ParallelSotopiaEnv
 from sotopia.envs.evaluators import (
     ReachGoalLLMEvaluator,
     RuleBasedTerminatedEvaluator,
     unweighted_aggregate_evaluate,
 )
 from sotopia.generation_utils.generate import LLM_Name, agenerate_script
 from sotopia.messages import AgentAction, Message, Observation
 from sotopia.messages.message_classes import (
     ScriptBackground,
     ScriptEnvironmentResponse,
-    ScriptInteraction,
-)
-from sotopia.samplers import (
-    BaseSampler,
-    ConstraintBasedSampler,
-    EnvAgentCombo,
-    UniformSampler,
 )
+from sotopia.samplers import BaseSampler, EnvAgentCombo
 
 
 @beartype
 def run_sync_server(
     model_name_dict: dict[str, LLM_Name],
     action_order: Literal["simutaneous", "round-robin", "random"],
     agents_info: dict[str, dict[str, str]] | None = None,
     partial_background_file: str | None = None,
     full_background_file: str | None = None,
     mode: str | None = None,
 ) -> list[tuple[str, str, Message]]:
-
     # Create Environment and agents
     # This step will be moved to outside this function
 
     env = ParallelSotopiaEnv(
         model_name=model_name_dict["env"],
         action_order=action_order,
         evaluators=[
@@ -85,35 +74,29 @@
     agents.reset()
 
     messages: list[tuple[str, str, Message]] = []
 
     # Main Event Loop
     done = False
     for agent_name in env.agents:
-        messages.append(
-            ("Environment", agent_name, environment_messages[agent_name])
-        )
+        messages.append(("Environment", agent_name, environment_messages[agent_name]))
 
     while not done:
         # gather agent messages
         agent_messages: dict[str, AgentAction] = dict()
         for agent_name in env.agents:
             if agents_info is not None:
                 agents[agent_name].goal = agents_info[agent_name]["goal"]
             agent_messages[agent_name] = agents[agent_name].act(
                 environment_messages[agent_name]
             )
-            messages.append(
-                (agent_name, "Environment", agent_messages[agent_name])
-            )
+            messages.append((agent_name, "Environment", agent_messages[agent_name]))
 
         # send agent messages to environment
-        environment_messages, _, terminated, ___, ____ = env.step(
-            agent_messages
-        )
+        environment_messages, _, terminated, ___, ____ = env.step(agent_messages)
         for agent_name in env.agents:
             messages.append(
                 ("Environment", agent_name, environment_messages[agent_name])
             )
         done = all(terminated.values())
 
     return messages
@@ -132,14 +115,16 @@
 ) -> list[tuple[str, str, Message]]:
     agents = Agents({agent.agent_name: agent for agent in agent_list})
     environment_messages = env.reset(agents=agents, omniscient=omniscient)
     agents_model_names = [model_dict["agent1"], model_dict["agent2"]]
     for agent_name, agent_model in zip(env.agents, agents_model_names):
         if agent_model == "human":
             agents[agent_name] = HumanAgent(agent_name)
+        elif agent_model == "redis":
+            agents[agent_name] = RedisAgent(agent_name)
         elif script_like and not json_in_script:
             agents[agent_name] = ScriptWritingAgent(
                 agent_name,
                 model_name=agent_model,
                 background=env.background,
                 agent_names=env.agents,
             )
@@ -184,17 +169,15 @@
                 else:
                     print("Current action taken: ", actions[idx])
 
         # actions = cast(list[AgentAction], actions)
         for idx, agent_name in enumerate(env.agents):
             agent_messages[agent_name] = actions[idx]
 
-            messages[-1].append(
-                (agent_name, "Environment", agent_messages[agent_name])
-            )
+            messages[-1].append((agent_name, "Environment", agent_messages[agent_name]))
 
         # send agent messages to environment
         (
             environment_messages,
             rewards_in_turn,
             terminated,
             ___,
@@ -204,39 +187,32 @@
             [
                 ("Environment", agent_name, environment_messages[agent_name])
                 for agent_name in env.agents
             ]
         )
         # print("Environment message: ", environment_messages)
         # exit(0)
-        rewards.append(
-            [rewards_in_turn[agent_name] for agent_name in env.agents]
-        )
+        rewards.append([rewards_in_turn[agent_name] for agent_name in env.agents])
         reasons.append(
             " ".join(info[agent_name]["comments"] for agent_name in env.agents)
         )
         done = all(terminated.values())
 
     # TODO: clean up this part
     epilog = EpisodeLog(
         environment=env.profile.pk,
         agents=[agent.profile.pk for agent in agent_list],
         tag=tag,
         models=[model_dict["env"], model_dict["agent1"], model_dict["agent2"]],
         messages=[
-            [
-                (m[0], m[1], m[2].to_natural_language())
-                for m in messages_in_turn
-            ]
+            [(m[0], m[1], m[2].to_natural_language()) for m in messages_in_turn]
             for messages_in_turn in messages
         ],
         reasoning=info[env.agents[0]]["comments"],
-        rewards=[
-            info[agent_name]["complete_rating"] for agent_name in env.agents
-        ],
+        rewards=[info[agent_name]["complete_rating"] for agent_name in env.agents],
         rewards_prompt=info["rewards_prompt"]["overall_prompt"],
     )
     rich.print(epilog.rewards_prompt)
     agent_profiles, conversation = epilog.render_for_humans()
     for agent_profile in agent_profiles:
         rich.print(agent_profile)
     for message in conversation:
@@ -252,17 +228,15 @@
 
 
 @gin.configurable
 @beartype
 async def run_async_server(
     model_dict: dict[str, LLM_Name],
     sampler: BaseSampler[Observation, AgentAction] = BaseSampler(),
-    action_order: Literal[
-        "simutaneous", "round-robin", "random"
-    ] = "round-robin",
+    action_order: Literal["simutaneous", "round-robin", "random"] = "round-robin",
     env_agent_combo_list: list[EnvAgentCombo[Observation, AgentAction]] = [],
     omniscient: bool = False,
     script_like: bool = False,
     json_in_script: bool = False,
     tag: str | None = None,
     push_to_db: bool = False,
     using_async: bool = True,
@@ -275,17 +249,15 @@
         script_like (bool): Whether we generate the turn in script like manner, default to False
         json_in_script (bool): Whether we requires the script generator to return json (Only valid when script_like is True), default to False
 
     Note: env_agent_combo_list is optional. When it defaults to [], sampler is used
     else the sampler is not used. Please pass in BaseSampler or simply not specify it when using this option.
     """
 
-    assert not (
-        push_to_db and tag is None
-    ), "please provide a tag when push to db"
+    assert not (push_to_db and tag is None), "please provide a tag when push to db"
 
     # Create Environment and agents
     # This step will be moved to outside this function
 
     env_params = {
         "model_name": model_dict["env"],
         "action_order": action_order,
@@ -310,21 +282,20 @@
             return ScriptWritingAgent
         else:
             return LLMAgent
 
     if env_agent_combo_list:
         assert (
             type(sampler) is BaseSampler
-        ), "No sampler should be used when `env_agent_combo_list` is empty"
+        ), "No sampler should be used when `env_agent_combo_list` is not empty"
         env_agent_combo_iter = iter(env_agent_combo_list)
     else:
         env_agent_combo_iter = sampler.sample(
             agent_classes=[
-                get_agent_class(model_name)
-                for model_name in agents_model_dict.values()
+                get_agent_class(model_name) for model_name in agents_model_dict.values()
             ],
             n_agent=len(agents_model_dict),
             env_params=env_params,
             agents_params=[
                 {"model_name": model_name} if model_name != "human" else {}
                 for model_name in agents_model_dict.values()
             ],
@@ -366,17 +337,15 @@
         omniscient (bool): Whether the agent knows the goal of the other
     """
 
     agents = Agents({agent.agent_name: agent for agent in agent_list})
     env.reset(agents=agents, omniscient=omniscient)
 
     agent_names = [agent.agent_name for agent in agent_list]
-    assert (
-        len(agent_names) == 2
-    ), f"only support 2 agents, current: {agent_names}"
+    assert len(agent_names) == 2, f"only support 2 agents, current: {agent_names}"
 
     script_background = env.inbox[0][1]
     assert isinstance(script_background, ScriptBackground)
     story, prompt = await agenerate_script(
         model_name=model_dict["env"],
         background=script_background,
         agent_names=agent_names,
@@ -397,17 +366,15 @@
                         )
                         for sing_evaluator in [evaluator]
                     ]
                 )
             )
         )
     )
-    info: dict[
-        str, dict[str, str | ScriptEnvironmentResponse | float | None]
-    ] = {
+    info: dict[str, dict[str, str | ScriptEnvironmentResponse | float | None]] = {
         script_background.p1_name: {
             "comments": response.comments or "",
             "complete_rating": response.p1_rate or 0,  # type: ignore
         },
         script_background.p2_name: {
             "comments": response.comments or "",
             "complete_rating": response.p2_rate or 0,  # type: ignore
@@ -416,25 +383,20 @@
     }
     epilog = EpisodeLog(
         environment=env.profile.pk,
         agents=[agent.profile.pk for agent in agent_list],
         tag=tag,
         models=[model_dict["env"], model_dict["agent1"], model_dict["agent2"]],
         messages=[
-            [
-                (m[0], m[1], m[2].to_natural_language())
-                for m in messages_in_turn
-            ]
+            [(m[0], m[1], m[2].to_natural_language()) for m in messages_in_turn]
             for messages_in_turn in messages
         ],
         reasoning=str(info[env.agents[0]]["comments"])
         + str(info[env.agents[1]]["comments"]),
-        rewards=[
-            info[agent_name]["complete_rating"] for agent_name in env.agents
-        ],
+        rewards=[info[agent_name]["complete_rating"] for agent_name in env.agents],
         rewards_prompt=info["rewards_prompt"]["overall_prompt"],
     )
     print("Reward prompt: ")
     rich.print(epilog.rewards_prompt)
     agent_profiles, conversation = epilog.render_for_humans()
     print("Agent profiles: ")
     for agent_profile in agent_profiles:
@@ -449,24 +411,22 @@
             logging.error(f"Failed to save episode log: {e}")
     # flatten nested list messages
     return list(itertools.chain(*messages))
 
 
 async def aevaluate_one_episode(
     episode: EpisodeLog,
-    model: LLM_Name = "gpt-4",
+    model: str = "gpt-4",
     tag: str | None = None,
     push_to_db: bool = False,
 ) -> None:
-    history = episode.rewards_prompt.replace(
-        "Prompt after formatting:", ""
-    ).split(",\nBased on previous interactions")[0]
-    evaluator = ReachGoalLLMEvaluator(
-        model_name=model, response_format="basic"
-    )
+    history = episode.rewards_prompt.replace("Prompt after formatting:", "").split(
+        ",\nBased on previous interactions"
+    )[0]
+    evaluator = ReachGoalLLMEvaluator(model_name=model, response_format="basic")
     response = unweighted_aggregate_evaluate(
         list(
             itertools.chain(
                 *await asyncio.gather(
                     *[
                         sing_evaluator.__acall__(
                             turn_number=-1,
@@ -475,17 +435,15 @@
                         )
                         for sing_evaluator in [evaluator]
                     ]
                 )
             )
         )
     )
-    info: dict[
-        str, dict[str, str | ScriptEnvironmentResponse | float | None]
-    ] = {
+    info: dict[str, dict[str, str | ScriptEnvironmentResponse | float | None]] = {
         episode.agents[0]: {
             "comments": response.comments or "",
             "complete_rating": response.p1_rate or 0,  # type: ignore
         },
         episode.agents[1]: {
             "comments": response.comments or "",
             "complete_rating": response.p2_rate or 0,  # type: ignore
@@ -496,18 +454,15 @@
         environment=episode.environment,
         agents=episode.agents,
         tag=tag,
         models=[model, episode.models[1], episode.models[2]],
         messages=episode.messages,
         reasoning=str(info[episode.agents[0]]["comments"])
         + str(info[episode.agents[1]]["comments"]),
-        rewards=[
-            info[agent_name]["complete_rating"]
-            for agent_name in episode.agents
-        ],
+        rewards=[info[agent_name]["complete_rating"] for agent_name in episode.agents],
         rewards_prompt="TBD",
     )
     # rich.print(history)
     # rich.print(epilog.rewards)
 
     if push_to_db:
         try:
```

