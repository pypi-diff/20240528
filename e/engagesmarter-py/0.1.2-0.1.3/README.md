# Comparing `tmp/engagesmarter_py-0.1.2.tar.gz` & `tmp/engagesmarter_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "engagesmarter_py-0.1.2.tar", max compression
+gzip compressed data, was "engagesmarter_py-0.1.3.tar", max compression
```

## Comparing `engagesmarter_py-0.1.2.tar` & `engagesmarter_py-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1066 2024-03-10 20:50:59.873990 engagesmarter_py-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      980 2024-03-11 10:34:57.352983 engagesmarter_py-0.1.2/README.md
--rw-r--r--   0        0        0     1044 2024-03-04 20:41:07.389626 engagesmarter_py-0.1.2/engagesmarter/__init__.py
--rw-r--r--   0        0        0     3333 2024-03-10 20:50:59.881310 engagesmarter_py-0.1.2/engagesmarter/_auth_client.py
--rw-r--r--   0        0        0     3408 2024-03-12 08:17:59.289630 engagesmarter_py-0.1.2/engagesmarter/client.py
--rw-r--r--   0        0        0      156 2024-03-04 20:41:07.433450 engagesmarter_py-0.1.2/engagesmarter/constants.py
--rw-r--r--   0        0        0     1470 2024-03-04 20:41:07.445974 engagesmarter_py-0.1.2/engagesmarter/errors.py
--rw-r--r--   0        0        0     1762 2024-03-04 20:41:07.453235 engagesmarter_py-0.1.2/engagesmarter/errors_handler.py
--rw-r--r--   0        0        0        0 2024-03-04 20:41:07.454828 engagesmarter_py-0.1.2/engagesmarter/py.typed
--rw-r--r--   0        0        0      146 2024-03-04 20:41:07.466281 engagesmarter_py-0.1.2/engagesmarter/resources/__init__.py
--rw-r--r--   0        0        0      787 2024-03-12 08:23:21.461477 engagesmarter_py-0.1.2/engagesmarter/resources/agents.py
--rw-r--r--   0        0        0      154 2024-03-04 20:41:07.485995 engagesmarter_py-0.1.2/engagesmarter/resources/base.py
--rw-r--r--   0        0        0    13454 2024-03-11 12:59:23.043377 engagesmarter_py-0.1.2/engagesmarter/resources/conversations.py
--rw-r--r--   0        0        0     7482 2024-03-12 10:45:56.734976 engagesmarter_py-0.1.2/engagesmarter/resources/runs.py
--rw-r--r--   0        0        0     3979 2024-03-04 20:41:07.512356 engagesmarter_py-0.1.2/engagesmarter/resources/tags.py
--rw-r--r--   0        0        0        0 2024-03-04 20:41:07.514368 engagesmarter_py-0.1.2/engagesmarter/schemas/__init__.py
--rw-r--r--   0        0        0      867 2024-03-12 08:25:12.234934 engagesmarter_py-0.1.2/engagesmarter/schemas/agents.py
--rw-r--r--   0        0        0       77 2024-03-04 20:41:07.528314 engagesmarter_py-0.1.2/engagesmarter/schemas/base.py
--rw-r--r--   0        0        0      330 2024-03-04 20:41:07.536363 engagesmarter_py-0.1.2/engagesmarter/schemas/conversations.py
--rw-r--r--   0        0        0      385 2024-03-04 20:41:07.546338 engagesmarter_py-0.1.2/engagesmarter/schemas/feedback.py
--rw-r--r--   0        0        0     1219 2024-03-04 20:41:07.554379 engagesmarter_py-0.1.2/engagesmarter/schemas/messages.py
--rw-r--r--   0        0        0      195 2024-03-04 20:41:07.566449 engagesmarter_py-0.1.2/engagesmarter/schemas/runs.py
--rw-r--r--   0        0        0      257 2024-03-04 20:41:07.577946 engagesmarter_py-0.1.2/engagesmarter/schemas/tags.py
--rw-r--r--   0        0        0       44 2024-03-04 20:41:07.616203 engagesmarter_py-0.1.2/engagesmarter/utils/__init__.py
--rw-r--r--   0        0        0      722 2024-03-04 20:41:07.627123 engagesmarter_py-0.1.2/engagesmarter/utils/content.py
--rw-r--r--   0        0        0      272 2024-03-04 20:41:07.637823 engagesmarter_py-0.1.2/engagesmarter/utils/pydantic.py
--rw-r--r--   0        0        0     3267 2024-03-04 20:41:07.652438 engagesmarter_py-0.1.2/engagesmarter/utils/streaming.py
--rw-r--r--   0        0        0      170 2024-03-04 20:41:07.660672 engagesmarter_py-0.1.2/engagesmarter/utils/utils.py
--rw-r--r--   0        0        0      569 2024-03-12 11:12:51.145770 engagesmarter_py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 engagesmarter_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 17:46:59.008766 engagesmarter_py-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0      980 2024-03-19 17:46:59.016408 engagesmarter_py-0.1.3/README.md
+-rw-r--r--   0        0        0     1126 2024-04-23 10:53:01.429062 engagesmarter_py-0.1.3/engagesmarter/__init__.py
+-rw-r--r--   0        0        0     3333 2024-03-19 17:46:59.050573 engagesmarter_py-0.1.3/engagesmarter/_auth_client.py
+-rw-r--r--   0        0        0     3408 2024-03-19 17:46:59.058353 engagesmarter_py-0.1.3/engagesmarter/client.py
+-rw-r--r--   0        0        0      156 2024-03-19 17:46:59.061707 engagesmarter_py-0.1.3/engagesmarter/constants.py
+-rw-r--r--   0        0        0     1470 2024-03-19 17:46:59.066487 engagesmarter_py-0.1.3/engagesmarter/errors.py
+-rw-r--r--   0        0        0     1762 2024-03-19 17:46:59.070715 engagesmarter_py-0.1.3/engagesmarter/errors_handler.py
+-rw-r--r--   0        0        0        0 2024-03-19 17:46:59.072185 engagesmarter_py-0.1.3/engagesmarter/py.typed
+-rw-r--r--   0        0        0      221 2024-04-23 10:53:01.437885 engagesmarter_py-0.1.3/engagesmarter/resources/__init__.py
+-rw-r--r--   0        0        0      787 2024-03-19 17:46:59.085134 engagesmarter_py-0.1.3/engagesmarter/resources/agents.py
+-rw-r--r--   0        0        0      154 2024-03-19 17:46:59.088579 engagesmarter_py-0.1.3/engagesmarter/resources/base.py
+-rw-r--r--   0        0        0    14984 2024-04-23 10:53:01.443356 engagesmarter_py-0.1.3/engagesmarter/resources/conversations.py
+-rw-r--r--   0        0        0     7482 2024-03-19 17:46:59.120590 engagesmarter_py-0.1.3/engagesmarter/resources/runs.py
+-rw-r--r--   0        0        0     4475 2024-04-23 10:53:01.448297 engagesmarter_py-0.1.3/engagesmarter/resources/tags.py
+-rw-r--r--   0        0        0        0 2024-03-19 17:46:59.124821 engagesmarter_py-0.1.3/engagesmarter/schemas/__init__.py
+-rw-r--r--   0        0        0     1202 2024-03-19 17:46:59.133817 engagesmarter_py-0.1.3/engagesmarter/schemas/agents.py
+-rw-r--r--   0        0        0       77 2024-03-19 17:46:59.138437 engagesmarter_py-0.1.3/engagesmarter/schemas/base.py
+-rw-r--r--   0        0        0     1481 2024-04-23 10:53:01.453710 engagesmarter_py-0.1.3/engagesmarter/schemas/conversations.py
+-rw-r--r--   0        0        0     1760 2024-04-23 10:53:01.458561 engagesmarter_py-0.1.3/engagesmarter/schemas/feedback.py
+-rw-r--r--   0        0        0     1231 2024-04-23 10:53:01.463287 engagesmarter_py-0.1.3/engagesmarter/schemas/messages.py
+-rw-r--r--   0        0        0      421 2024-04-23 10:53:01.468501 engagesmarter_py-0.1.3/engagesmarter/schemas/runs.py
+-rw-r--r--   0        0        0      257 2024-03-19 17:46:59.160007 engagesmarter_py-0.1.3/engagesmarter/schemas/tags.py
+-rw-r--r--   0        0        0       44 2024-03-19 17:46:59.163096 engagesmarter_py-0.1.3/engagesmarter/utils/__init__.py
+-rw-r--r--   0        0        0      722 2024-03-19 17:46:59.172080 engagesmarter_py-0.1.3/engagesmarter/utils/content.py
+-rw-r--r--   0        0        0      272 2024-03-19 17:46:59.174767 engagesmarter_py-0.1.3/engagesmarter/utils/pydantic.py
+-rw-r--r--   0        0        0     3267 2024-03-19 17:46:59.178196 engagesmarter_py-0.1.3/engagesmarter/utils/streaming.py
+-rw-r--r--   0        0        0      170 2024-03-19 17:46:59.181242 engagesmarter_py-0.1.3/engagesmarter/utils/utils.py
+-rw-r--r--   0        0        0      597 2024-05-28 17:32:28.224272 engagesmarter_py-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1719 1970-01-01 00:00:00.000000 engagesmarter_py-0.1.3/PKG-INFO
```

### Comparing `engagesmarter_py-0.1.2/LICENSE.md` & `engagesmarter_py-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `engagesmarter_py-0.1.2/README.md` & `engagesmarter_py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `engagesmarter_py-0.1.2/engagesmarter/__init__.py` & `engagesmarter_py-0.1.3/engagesmarter/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,40 +8,43 @@
 
 from .client import Client
 from .schemas.agents import AgentMetadata
 from .schemas.base import Success
 from .schemas.conversations import (
     ConversationCreate,
     ConversationRead,
+    ConversationReadFull,
     ConversationUpdate,
 )
 from .schemas.feedback import FeedbackRead, FeedbackUpsert
 from .schemas.messages import (
     AgentMessage,
     InfoMessage,
     MessageBasic,
     MessageRead,
     StatusMessage,
     UserMessage,
 )
-from .schemas.runs import RunRead
+from .schemas.runs import RunRead, RunReadFull
 from .schemas.tags import TagCreate, TagRead, TagUpdate
 
 __all__ = [
     Client,
     AgentMessage,
     AgentMetadata,
     ConversationCreate,
     ConversationRead,
+    ConversationReadFull,
     ConversationUpdate,
     FeedbackRead,
     FeedbackUpsert,
     MessageBasic,
     MessageRead,
     RunRead,
+    RunReadFull,
     Success,
     TagCreate,
     TagRead,
     TagUpdate,
     UserMessage,
     InfoMessage,
     StatusMessage,
```

### Comparing `engagesmarter_py-0.1.2/engagesmarter/_auth_client.py` & `engagesmarter_py-0.1.3/engagesmarter/_auth_client.py`

 * *Files identical despite different names*

### Comparing `engagesmarter_py-0.1.2/engagesmarter/client.py` & `engagesmarter_py-0.1.3/engagesmarter/client.py`

 * *Files identical despite different names*

### Comparing `engagesmarter_py-0.1.2/engagesmarter/errors.py` & `engagesmarter_py-0.1.3/engagesmarter/errors.py`

 * *Files identical despite different names*

### Comparing `engagesmarter_py-0.1.2/engagesmarter/errors_handler.py` & `engagesmarter_py-0.1.3/engagesmarter/errors_handler.py`

 * *Files identical despite different names*

### Comparing `engagesmarter_py-0.1.2/engagesmarter/resources/agents.py` & `engagesmarter_py-0.1.3/engagesmarter/resources/agents.py`

 * *Files identical despite different names*

### Comparing `engagesmarter_py-0.1.2/engagesmarter/resources/conversations.py` & `engagesmarter_py-0.1.3/engagesmarter/resources/conversations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,87 @@
 from __future__ import annotations
 
 from typing import Generator
 
 from ..constants import API_VERSION
-from ..schemas.base import Success
 from ..schemas.conversations import (
     ConversationCreate,
     ConversationRead,
+    ConversationReadFull,
     ConversationUpdate,
 )
 from ..schemas.feedback import FeedbackRead
 from ..schemas.messages import AgentMessage, MessageRead, UserMessage
 from ..schemas.runs import RunRead
 from ..schemas.tags import TagRead
 from .base import BaseResource
 
 
 class ConversationsResource(BaseResource):
     _API_PREFIX: str = f"/{API_VERSION}/conversations"
 
     def create(
         self, *, conversation: ConversationCreate | None = None
-    ) -> ConversationRead:
+    ) -> ConversationReadFull:
         """
-        Creates a new conversation and get new conversation read object,
+        Creates a new conversation and get new conversation read full object,
         including the conversation_id.
 
         Args:
-          conversation: If specified, any data included in the `data` field will be included as
-              metadata within the conversation. We recommend structuring this metadata as a JSON
-              encodable dictionary.
+          conversation: This can be useful for including additional context about the conversation.
 
-              This can be useful for including additional context about the conversation.
+              If specified, any data included in the `data` field will be included as metadata within
+              the conversation. We recommend structuring this metadata as a JSONencodable dictionary.
+
+              If specified, the `source` field can be used as the source of the conversation.
+              For instance, a particular chat widget.
         """
         if conversation is None:
             conversation = ConversationCreate()
         response = self.client.post(self._API_PREFIX, content=conversation)
-        return ConversationRead(**response)
+        return ConversationReadFull(**response)
 
     def clone_conversation(
         self,
         *,
         message_id: str,
         conversation: ConversationUpdate | None = None,
-    ) -> ConversationRead:
+    ) -> ConversationReadFull:
         """
         Clones a new conversation from a full or partial existing conversation. This works by
         cloning an existing conversation up to and including the message with the specified
         `message_id`. The new conversation will have a new `conversation_id`, which is different
         from the existing one.
 
         Args:
           message_id: The ID of the agent message up to which to clone an existing conversation.
               The system uses the agent message ID to identify a particular run step in the
               conversation.
 
-          conversation: If specified, any data included in the `data` field will be included as
+          conversation: This can be useful for including additional context about the conversation.
+
+              If specified, any data included in the `data` field will be included as
               metadata within the new conversation and will replace any metadata on the cloned
               conversation. We recommend structuring this metadata as a JSON encodable dictionary.
 
-              If not specified or set to None, and the cloned conversation already has metadata,
-              then that metadata will be carried over to the new conversation.
+              If specified, the `source` field can be used as the source of the conversation.
+              For instance, a particular chat widget.
 
-              This can be useful for including additional context about the conversation.
+              If `conversation` is not specified or set to None, and the cloned conversation
+              already has metadata, then that metadata will be carried over to the new conversation.
         """
         if conversation is None:
             conversation = ConversationUpdate()
         query_params = {"message_id": message_id}
         response = self.client.post(
             f"{self._API_PREFIX}/clone",
             content=conversation,
             params=query_params,
         )
-        return ConversationRead(**response)
+        return ConversationReadFull(**response)
 
     def search_own_conversations(
         self,
         *,
         tag_id: str | None = None,
         reversed: bool = True,
         limit: int = 20,
@@ -106,14 +111,48 @@
             "offset": offset,
         }
         if tag_id:
             query_params["tag_id"] = tag_id
         response = self.client.get(f"{self._API_PREFIX}/me", params=query_params)
         return [ConversationRead(**conversation_dict) for conversation_dict in response]
 
+    def search_current_org_conversations(
+        self,
+        *,
+        tag_id: str | None = None,
+        reversed: bool = True,
+        limit: int = 20,
+        offset: int = 0,
+    ) -> list[ConversationRead]:
+        """
+        Fetches metadata on all past conversations within the organization.
+
+        By default, it returns the most recent conversations first. It can additionally be
+        filtered by `tag_id`.
+
+        Args:
+          tag_id: If specified, only conversations with the specified tag will be returned.
+
+          reversed: If True, returns the most recent conversations first. Otherwise, returns the
+              oldest conversations first.
+
+          limit: Number of conversations to return.
+
+          offset: Number of conversations to skip.
+        """
+        query_params = {
+            "reversed": reversed,
+            "limit": limit,
+            "offset": offset,
+        }
+        if tag_id:
+            query_params["tag_id"] = tag_id
+        response = self.client.get(f"{self._API_PREFIX}/org", params=query_params)
+        return [ConversationRead(**conversation_dict) for conversation_dict in response]
+
     def search_saved_conversations(
         self, *, reversed: bool = True, limit: int = 20, offset: int = 0
     ) -> list[ConversationRead]:
         """
         Fetches metadata on user's saved conversations within the organization. Saved conversations
         can be any conversations carried out within the organization, not only the user's own.
 
@@ -131,64 +170,66 @@
             "reversed": reversed,
             "limit": limit,
             "offset": offset,
         }
         response = self.client.get(f"{self._API_PREFIX}/saved", params=query_params)
         return [ConversationRead(**conversation_dict) for conversation_dict in response]
 
-    def get_conversation_metadata(self, *, conversation_id: str) -> ConversationRead:
+    def get_conversation_metadata(
+        self, *, conversation_id: str
+    ) -> ConversationReadFull:
         """
         Fetches metadata on a specified conversation.
 
         Args:
           conversation_id: The ID of the conversation for which to get the metadata.
         """
         response = self.client.get(f"{self._API_PREFIX}/{conversation_id}")
-        return ConversationRead(**response)
+        return ConversationReadFull(**response)
 
     def update_conversation_metadata(
         self, *, conversation_id: str, conversation: ConversationUpdate
-    ) -> ConversationRead:
+    ) -> ConversationReadFull:
         """
         Updates metadata on a specified conversation.
 
         Args:
           conversation_id: The ID of the conversation for which to update the metadata.
 
           conversation: The updated conversation metadata.
         """
         response = self.client.patch(
             f"{self._API_PREFIX}/{conversation_id}",
             content=conversation,
         )
-        return ConversationRead(**response)
+        return ConversationReadFull(**response)
 
-    def save_conversation(self, *, conversation_id: str) -> ConversationRead:
+    def save_conversation(self, *, conversation_id: str) -> ConversationReadFull:
         """
         Adds a specified conversation to user's saved conversations list. The conversation can
         be any conversation carried out within the organization, not only the user's own. The
         user is identified based on the API key being used.
 
         Args:
           conversation_id: The ID of the conversation to save.
         """
         response = self.client.post(f"{self._API_PREFIX}/{conversation_id}/saved")
-        return ConversationRead(**response)
+        return ConversationReadFull(**response)
 
-    def unsave_conversation(self, *, conversation_id: str) -> Success:
+    def unsave_conversation(self, *, conversation_id: str) -> ConversationReadFull:
         """
         Removes a specified conversation from user's saved conversations list.
         This does not delete the underlying conversation and only removes a reference
         to it in the user's list. The user is identified based on the API key being used.
 
         Args:
           conversation_id: The ID of the conversation to remove.
         """
         response = self.client.delete(f"{self._API_PREFIX}/{conversation_id}/saved")
-        return Success(**response)
+        return ConversationReadFull(**response)
 
     def add_messages_to_conversation_history(
         self, *, conversation_id: str, messages: list[UserMessage | AgentMessage]
     ) -> list[MessageRead]:
         """
         Adds messages to a specified conversation's message history without triggering an agent
         response. Messages are added in the order in which they are provided.
```

### Comparing `engagesmarter_py-0.1.2/engagesmarter/resources/runs.py` & `engagesmarter_py-0.1.3/engagesmarter/resources/runs.py`

 * *Files identical despite different names*

### Comparing `engagesmarter_py-0.1.2/engagesmarter/resources/tags.py` & `engagesmarter_py-0.1.3/engagesmarter/resources/tags.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,30 +6,42 @@
 from .base import BaseResource
 
 
 class TagsResource(BaseResource):
     _API_PREFIX: str = f"/{API_VERSION}/tags"
 
     def search(
-        self, *, search: str = "", limit: int = 20, offset: int = 0
+        self,
+        *,
+        search: str = "",
+        reversed: bool = True,
+        limit: int = 20,
+        offset: int = 0,
     ) -> list[TagRead]:
         """
         Searches for tags with names or descriptions matching the given search string.
         Only searches for tags available within the current organization.
 
         Args:
+          reversed: If True, get most recently created tag first. True by default.
+
           search: A search string to search for among tag names and descriptions.
 
           limit: The maximum number of tags to return.
 
           offset: The number of tags to skip before returning results.
         """
         response = self.client.get(
             f"{self._API_PREFIX}",
-            params={"search": search, "limit": limit, "offset": offset},
+            params={
+                "search": search,
+                "limit": limit,
+                "offset": offset,
+                "reversed": reversed,
+            },
         )
         return [TagRead(**tag_dict) for tag_dict in response]
 
     def create(self, *, name: str, description: str = "") -> TagRead:
         """
         Creates a new tag in the current organization.
 
@@ -72,43 +84,47 @@
         Args:
           tag_id: The ID of the tag to delete.
         """
         response = self.client.delete(f"{self._API_PREFIX}/{tag_id}")
         return Success(**response)
 
     def get_tagged_conversations(
-        self, *, tag_id: str, limit: int = 20, offset: int = 0
+        self, *, reversed: bool = True, tag_id: str, limit: int = 20, offset: int = 0
     ) -> list[ConversationRead]:
         """
         Fetches a list of metadata objects for conversations that have been linked to a given tag.
 
         Args:
+          reversed: If True, get most recent conversation first. True by default.
+
           tag_id: The ID of the tag to fetch conversations for.
 
           limit: The maximum number of conversations to return.
 
           offset: The number of conversations to skip before returning results.
         """
         response = self.client.get(
             f"{self._API_PREFIX}/{tag_id}/conversations",
-            params={"limit": limit, "offset": offset},
+            params={"limit": limit, "offset": offset, "reversed": reversed},
         )
         return [ConversationRead(**conversation) for conversation in response]
 
     def get_tagged_runs(
-        self, *, tag_id: str, limit: int = 20, offset: int = 0
+        self, *, reversed: bool = True, tag_id: str, limit: int = 20, offset: int = 0
     ) -> list[RunRead]:
         """
         Fetches a list of metadata objects for runs that have been linked to a given tag.
 
         Args:
+          reversed: If True, get most recent run first. True by default.
+
           tag_id: The ID of the tag to fetch runs for.
 
           limit: The maximum number of runs to return.
 
           offset: The number of runs to skip before returning results.
         """
         response = self.client.get(
             f"{self._API_PREFIX}/{tag_id}/runs",
-            params={"limit": limit, "offset": offset},
+            params={"limit": limit, "offset": offset, "reversed": reversed},
         )
         return [RunRead(**run) for run in response]
```

### Comparing `engagesmarter_py-0.1.2/engagesmarter/schemas/messages.py` & `engagesmarter_py-0.1.3/engagesmarter/schemas/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
     id: str
     org_id: str
     conversation_id: str
     run_id: str
     role: str
     content: str
-    created: datetime
     name: str | None = None
     user_id: str | None = None
+    created: datetime
 
 
 class MessageBasic(BaseModel):
-    """A message with just the basic fields"""
+    """Message with the basic fields - Not from the API"""
 
     role: str
     content: str
     name: str | None = None
 
 
 class UserMessage(MessageBasic):
```

### Comparing `engagesmarter_py-0.1.2/engagesmarter/utils/content.py` & `engagesmarter_py-0.1.3/engagesmarter/utils/content.py`

 * *Files identical despite different names*

### Comparing `engagesmarter_py-0.1.2/engagesmarter/utils/streaming.py` & `engagesmarter_py-0.1.3/engagesmarter/utils/streaming.py`

 * *Files identical despite different names*

### Comparing `engagesmarter_py-0.1.2/pyproject.toml` & `engagesmarter_py-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "engagesmarter-py"
-version = "0.1.2"
+version = "0.1.3"
 description = "Engage Smarter AI Platform Python client."
 authors = ["Tom Dorrington Ward <tom@engagesmarter.ai>"]
 maintainers = ["Tom Dorrington Ward <tom@engagesmarter.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://docs.engagesmarter.ai"
 packages = [
     { include = "engagesmarter" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 httpx = ">=0.19.0"
+pydantic = ">=1.0.0,<3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `engagesmarter_py-0.1.2/PKG-INFO` & `engagesmarter_py-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: engagesmarter-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Engage Smarter AI Platform Python client.
 Home-page: https://docs.engagesmarter.ai
 License: MIT
 Author: Tom Dorrington Ward
 Author-email: tom@engagesmarter.ai
 Maintainer: Tom Dorrington Ward
 Maintainer-email: tom@engagesmarter.ai
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.19.0)
+Requires-Dist: pydantic (>=1.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://docs.engagesmarter.ai/"><img width="350" height="208" src="https://raw.githubusercontent.com/engagesmarter/engagesmarter-py/master/docs/img/es_logo.jpg" alt='Engage Smarter AI'></a>
 </p>
 
 <h1 align="center"><strong>Engage Smarter AI Platform Python Client</strong></h1>
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: engagesmarter-py Version: 0.1.2 Summary: Engage
+Metadata-Version: 2.1 Name: engagesmarter-py Version: 0.1.3 Summary: Engage
 Smarter AI Platform Python client. Home-page: https://docs.engagesmarter.ai
 License: MIT Author: Tom Dorrington Ward Author-email: tom@engagesmarter.ai
 Maintainer: Tom Dorrington Ward Maintainer-email: tom@engagesmarter.ai
 Requires-Python: >=3.9 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: httpx
-(>=0.19.0) Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Dist: httpx (>=0.19.0) Requires-Dist:
+pydantic (>=1.0.0,<3.0.0) Description-Content-Type: text/markdown
                               _[_E_n_g_a_g_e_ _S_m_a_r_t_e_r_ _A_I_]
             ************ EEnnggaaggee SSmmaarrtteerr AAII PPllaattffoorrmm PPyytthhoonn CClliieenntt ************
                                _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
 The Engage Smarter AI Platform Python Client provides a simple way to interact
 with the Engage Smarter AI Platform from Python. For more information on how to
 interact with the Engage Smarter AI Platform API, please visit the Engage
 Smarter AI Platform [developer docs](https://docs.engagesmarter.ai/).
```

