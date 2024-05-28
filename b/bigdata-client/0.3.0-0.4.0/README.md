# Comparing `tmp/bigdata_client-0.3.0.tar.gz` & `tmp/bigdata_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigdata_client-0.3.0.tar", max compression
+gzip compressed data, was "bigdata_client-0.4.0.tar", max compression
```

## Comparing `bigdata_client-0.3.0.tar` & `bigdata_client-0.4.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
--rw-r--r--   0        0        0      358 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/README.md
--rw-r--r--   0        0        0      155 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/__init__.py
--rw-r--r--   0        0        0     6556 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/advanced_search_query.py
--rw-r--r--   0        0        0        0 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/api/__init__.py
--rw-r--r--   0        0        0      888 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/api/knowledge_graph.py
--rw-r--r--   0        0        0     8970 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/api/search.py
--rw-r--r--   0        0        0     2985 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/api/uploads.py
--rw-r--r--   0        0        0      975 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/api/watchlist.py
--rw-r--r--   0        0        0     6464 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/auth.py
--rw-r--r--   0        0        0        0 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/authenticators/__init__.py
--rw-r--r--   0        0        0     2256 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/authenticators/base_instance.py
--rw-r--r--   0        0        0     4166 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/authenticators/dev_instance.py
--rw-r--r--   0        0        0     3650 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/authenticators/production_instance.py
--rw-r--r--   0        0        0      853 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/exceptions.py
--rw-r--r--   0        0        0      245 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/models.py
--rw-r--r--   0        0        0        0 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/sign_in_strategies/__init__.py
--rw-r--r--   0        0        0      243 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/sign_in_strategies/base.py
--rw-r--r--   0        0        0     1008 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/sign_in_strategies/password.py
--rw-r--r--   0        0        0     2510 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/token_manager.py
--rw-r--r--   0        0        0     2040 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/token_manager_factory.py
--rw-r--r--   0        0        0    14138 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/connection.py
--rw-r--r--   0        0        0      475 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/connection_protocol.py
--rw-r--r--   0        0        0      154 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/constants.py
--rw-r--r--   0        0        0     4501 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/daterange.py
--rw-r--r--   0        0        0     1234 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/entity_types.py
--rw-r--r--   0        0        0      664 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/enum_utils.py
--rw-r--r--   0        0        0       82 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/errors.py
--rw-r--r--   0        0        0      196 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/file_status.py
--rw-r--r--   0        0        0      513 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/jwt.py
--rw-r--r--   0        0        0        0 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/__init__.py
--rw-r--r--   0        0        0    33261 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/advanced_search_query.py
--rw-r--r--   0        0        0     1181 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/comentions.py
--rw-r--r--   0        0        0     5961 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/entities.py
--rw-r--r--   0        0        0     1094 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/languages.py
--rw-r--r--   0        0        0     3841 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/parse.py
--rw-r--r--   0        0        0     3513 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/search.py
--rw-r--r--   0        0        0     2280 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/sources.py
--rw-r--r--   0        0        0      897 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/story.py
--rw-r--r--   0        0        0     2180 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/topics.py
--rw-r--r--   0        0        0     6902 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/uploads.py
--rw-r--r--   0        0        0     2820 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/watchlists.py
--rw-r--r--   0        0        0     4773 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/old_auth.py
--rw-r--r--   0        0        0      177 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/pdf_utils.py
--rw-r--r--   0        0        0     1296 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/query.py
--rw-r--r--   0        0        0      251 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/query_type.py
--rw-r--r--   0        0        0     9523 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/search.py
--rw-r--r--   0        0        0    14376 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/services.py
--rw-r--r--   0        0        0     1086 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/settings.py
--rw-r--r--   0        0        0     2146 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/story.py
--rw-r--r--   0        0        0      465 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/user_agent.py
--rw-r--r--   0        0        0     1359 2024-05-10 15:57:33.966220 bigdata_client-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 bigdata_client-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      358 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/README.md
+-rw-r--r--   0        0        0      154 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/__init__.py
+-rw-r--r--   0        0        0     6536 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/advanced_search_query.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/api/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/api/knowledge_graph.py
+-rw-r--r--   0        0        0     9039 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/api/search.py
+-rw-r--r--   0        0        0     2985 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/api/uploads.py
+-rw-r--r--   0        0        0      975 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/api/watchlist.py
+-rw-r--r--   0        0        0     6464 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/auth.py
+-rw-r--r--   0        0        0     1874 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/bigdata.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/clerk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/clerk/authenticators/__init__.py
+-rw-r--r--   0        0        0     2256 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/clerk/authenticators/base_instance.py
+-rw-r--r--   0        0        0     4166 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/clerk/authenticators/dev_instance.py
+-rw-r--r--   0        0        0     3650 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/clerk/authenticators/production_instance.py
+-rw-r--r--   0        0        0      853 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/clerk/exceptions.py
+-rw-r--r--   0        0        0      245 2024-05-28 14:44:46.404251 bigdata_client-0.4.0/bigdata/clerk/models.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/clerk/sign_in_strategies/__init__.py
+-rw-r--r--   0        0        0      243 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/clerk/sign_in_strategies/base.py
+-rw-r--r--   0        0        0     1008 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/clerk/sign_in_strategies/password.py
+-rw-r--r--   0        0        0     2510 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/clerk/token_manager.py
+-rw-r--r--   0        0        0     2040 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/clerk/token_manager_factory.py
+-rw-r--r--   0        0        0    14138 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/connection.py
+-rw-r--r--   0        0        0      475 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/connection_protocol.py
+-rw-r--r--   0        0        0      154 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/constants.py
+-rw-r--r--   0        0        0     4501 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/daterange.py
+-rw-r--r--   0        0        0     2209 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/document.py
+-rw-r--r--   0        0        0     1234 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/entity_types.py
+-rw-r--r--   0        0        0      664 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/enum_utils.py
+-rw-r--r--   0        0        0      196 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/file_status.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/models/__init__.py
+-rw-r--r--   0        0        0    36167 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/models/advanced_search_query.py
+-rw-r--r--   0        0        0     2028 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/models/comentions.py
+-rw-r--r--   0        0        0      901 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/models/document.py
+-rw-r--r--   0        0        0     6291 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/models/entities.py
+-rw-r--r--   0        0        0     1137 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/models/languages.py
+-rw-r--r--   0        0        0     3841 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/models/parse.py
+-rw-r--r--   0        0        0     2249 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/models/search.py
+-rw-r--r--   0        0        0     2313 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/models/sources.py
+-rw-r--r--   0        0        0     2213 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/models/topics.py
+-rw-r--r--   0        0        0     6902 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/models/uploads.py
+-rw-r--r--   0        0        0     2820 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/models/watchlists.py
+-rw-r--r--   0        0        0      177 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/pdf_utils.py
+-rw-r--r--   0        0        0     1376 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/query.py
+-rw-r--r--   0        0        0      251 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/query_type.py
+-rw-r--r--   0        0        0     9723 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/search.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/services/__init__.py
+-rw-r--r--   0        0        0     2558 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/services/content_search.py
+-rw-r--r--   0        0        0     8048 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/services/knowledge_graph.py
+-rw-r--r--   0        0        0     4126 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/services/uploads.py
+-rw-r--r--   0        0        0     2959 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/services/watchlists.py
+-rw-r--r--   0        0        0      804 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/settings.py
+-rw-r--r--   0        0        0      465 2024-05-28 14:44:46.408251 bigdata_client-0.4.0/bigdata/user_agent.py
+-rw-r--r--   0        0        0     1359 2024-05-28 14:44:46.412251 bigdata_client-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 bigdata_client-0.4.0/PKG-INFO
```

### Comparing `bigdata_client-0.3.0/bigdata/advanced_search_query.py` & `bigdata_client-0.4.0/bigdata/advanced_search_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from bigdata.constants import SEARCH_PAGE_SIZE
 from bigdata.daterange import AbsoluteDateRange, RollingDateRange
 from bigdata.models.advanced_search_query import (
     QueryComponent,
     _expression_to_query_component,
 )
 from bigdata.models.search import (
+    DocumentType,
     Expression,
     ExpressionTypes,
-    FileType,
     SearchPagination,
     SortBy,
 )
 from bigdata.settings import settings
 
 
 @dataclass
@@ -29,20 +29,20 @@
     """
     A class to hold the query with the date range and sort by
     """
 
     query: QueryComponent
     date_range: Optional[Union[AbsoluteDateRange, RollingDateRange]] = None
     sortby: SortBy = SortBy.RELEVANCE
-    scope: FileType = FileType.ALL
+    scope: DocumentType = DocumentType.ALL
 
     def make_copy(self) -> "AdvancedSearchQuery":
         return AdvancedSearchQuery(
             date_range=self.date_range,
-            query=self.query.make_copy(),  # TODO: make copy of this too?
+            query=self.query.make_copy(),
             sortby=self.sortby,
             scope=self.scope,
         )
 
     def to_query_clusters_api_request(self, page: int) -> QueryClustersRequest:
         """
         Used when composing the request to perform a search using the
```

### Comparing `bigdata_client-0.3.0/bigdata/api/knowledge_graph.py` & `bigdata_client-0.4.0/bigdata/api/knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/api/search.py` & `bigdata_client-0.4.0/bigdata/api/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,49 +5,50 @@
 
 import datetime
 from typing import Literal, Optional, Union
 
 from pydantic import BaseModel, Field
 
 from bigdata.constants import SEARCH_PAGE_SIZE
+from bigdata.models.document import DocType
 from bigdata.models.entities import (
     Company,
     Concept,
     Facility,
     Landmark,
     Organization,
     OrganizationType,
+    Person,
     Place,
     Product,
     ProductType,
 )
 from bigdata.models.languages import Language
 from bigdata.models.search import (
+    DocumentType,
     Expression,
-    FileType,
     Ranking,
     SearchChain,
     SearchPagination,
     SearchSharePermission,
     SortBy,
 )
 from bigdata.models.sources import Source
-from bigdata.models.story import StoryType
 from bigdata.models.topics import Topic
 from bigdata.query_type import QueryType
 from bigdata.settings import settings
 
 # Save a search
 
 
 class SaveSearchQueryRequest(BaseModel):
     """Model to represent the "query" attribute of a request to save a search"""
 
     expression: Expression
-    scope: FileType = Field(default=FileType.ALL)
+    scope: DocumentType = Field(default=DocumentType.ALL)
     sort: SortBy = Field(default=SortBy.RELEVANCE)
     ranking: Ranking = Field(default=settings.LLM.RANKING)
     search_chain: Optional[SearchChain] = Field(alias="searchChain", default=None)
     hybrid: bool = settings.LLM.USE_HYBRID
     # The date expression neds a type=ExpressionTypes.DATE
     # the value is coming from date_range.to_expression()
     date: Optional[list[Expression]] = None
@@ -94,18 +95,17 @@
 class SavedSearchQueryResponse(BaseModel):
     """
     Model to represent the "query" attribute of a response from getting a saved
     search.
     """
 
     expression: Expression
-    scope: FileType = Field(default=FileType.ALL)
+    scope: DocumentType = Field(default=DocumentType.ALL)
     sort: SortBy = Field(default=SortBy.RELEVANCE)
     ranking: Ranking = Field(default=settings.LLM.RANKING)
-    search_chain: Optional[SearchChain] = Field(alias="searchChain", default=None)
     hybrid: bool = settings.LLM.USE_HYBRID
     date: Optional[list[Expression]] = None
 
 
 class SavedSearchResponse(BaseModel):
     """Model to represent the response from getting a saved search"""
 
@@ -156,143 +156,143 @@
 # Run a search
 
 
 class QueryClustersRequest(BaseModel):
     """Model to represent a request to run a search"""
 
     expression: Expression
-    scope: FileType = Field(default=FileType.ALL)
+    scope: DocumentType = Field(default=DocumentType.ALL)
     sort: SortBy = Field(default=SortBy.RELEVANCE)
     ranking: Ranking = Field(default=settings.LLM.RANKING)
     pagination: SearchPagination = Field(
         default=SearchPagination(limit=SEARCH_PAGE_SIZE, cursor=1)
     )
     search_chain: Optional[SearchChain] = Field(alias="searchChain", default=None)
     hybrid: bool = settings.LLM.USE_HYBRID
 
 
 class QueryChunksRequest(BaseModel):
     """Model to represent a request to run a search"""
 
     expression: Expression
-    scope: FileType = Field(default=FileType.ALL)
+    scope: DocumentType = Field(default=DocumentType.ALL)
     sort: SortBy = Field(default=SortBy.RELEVANCE)
     ranking: Ranking = Field(default=settings.LLM.RANKING)
     pagination: SearchPagination = Field(
         default=SearchPagination(limit=SEARCH_PAGE_SIZE, cursor=1)
     )
     search_chain: Optional[SearchChain] = Field(alias="searchChain", default=None)
     hybrid: bool = settings.LLM.USE_HYBRID
 
 
-class ClusteredStoryResponse(BaseModel):
+class ClusteredDocumentResponse(BaseModel):
     """
     Helper class to parse the response from the API.
     It should be used only internally to parse the JSON response from the API,
     and not passed around.
     """
 
     headline: str = Field(validation_alias="hd")
     id: str
     sentiment: float = Field(validation_alias="sent")
-    story_type: StoryType = Field(validation_alias="doctype")
+    doc_type: DocType = Field(validation_alias="doctype")
     timestamp: datetime.datetime = Field(validation_alias="ts")
 
     source_key: str = Field(validation_alias="srcKey")
     source_name: str = Field(validation_alias="srcName")
     source_rank: int
     language: str
 
-    class StoryResponseSentence(BaseModel):
+    class DocumentResponseSentence(BaseModel):
         text: str
         pnum: int
         snum: int
 
-        class StoryResponseEntity(BaseModel):
+        class DocumentResponseEntity(BaseModel):
             key: str
             start: int
             end: int
             queryType: QueryType
 
-        entities: list[StoryResponseEntity]
+        entities: list[DocumentResponseEntity]
 
-    sentences: list[StoryResponseSentence]
+    sentences: list[DocumentResponseSentence]
 
 
-class ChunkedStoryResponse(BaseModel):
+class ChunkedDocumentResponse(BaseModel):
     """
     Helper class to parse the response from the API.
     It should be used only internally to parse the JSON response from the API,
     and not passed around.
     """
 
     headline: str = Field(validation_alias="hd")
     id: str
     sentiment: float = Field(validation_alias="sent")
-    story_type: StoryType = Field(validation_alias="doctype")
+    doc_type: DocType = Field(validation_alias="doctype")
     timestamp: datetime.datetime = Field(validation_alias="ts")
 
     source_key: str = Field(validation_alias="srcKey")
     source_name: str = Field(validation_alias="srcName")
     source_rank: int
     language: str
 
-    class ChunkedStoryResponseSentence(BaseModel):
+    class ChunkedDocumentResponseSentence(BaseModel):
         text: str
         cnum: int
         relevance: float
         sentiment: float
 
-        class StoryResponseEntity(BaseModel):
+        class DocumentResponseEntity(BaseModel):
             key: str
             start: int
             end: int
             queryType: QueryType
 
-        entities: list[StoryResponseEntity]
+        entities: list[DocumentResponseEntity]
 
-        class StoryResponseSentence(BaseModel):
+        class DocumentResponseSentence(BaseModel):
             pnum: int
             snum: int
 
-        sentences: list[StoryResponseSentence]
+        sentences: list[DocumentResponseSentence]
 
-    chunks: list[ChunkedStoryResponseSentence]
+    chunks: list[ChunkedDocumentResponseSentence]
 
 
 class QueryClustersResponse(BaseModel):
-    """Model to represent the response from running a search"""
+    """Model to represent the backend response from running a search"""
 
     count: int
     document_count: int = Field(alias="documentCount")
     coverage: dict  # Not worth to model this yet
     timing: dict  # Not worth to model this yet
-    stories: list[ClusteredStoryResponse]
+    stories: list[ClusteredDocumentResponse]
     next_cursor: Optional[int] = Field(alias="nextCursor", default=None)
 
 
 class QueryChunksResponse(BaseModel):
-    """Model to represent the response from running a search"""
+    """Model to represent the Backend response from running a search"""
 
     count: int
     document_count: int = Field(alias="documentCount")
     coverage: dict  # Not worth to model this yet
     timing: dict  # Not worth to model this yet
-    stories: list[ChunkedStoryResponse]
+    stories: list[ChunkedDocumentResponse]
     next_cursor: Optional[int] = Field(alias="nextCursor", default=None)
 
 
 # Comentions
 
 
 class DiscoveryPanelRequest(BaseModel):
     """Model to represent a request to get comentions"""
 
     expression: Expression
-    scope: FileType = Field(default=FileType.ALL)
+    scope: DocumentType = Field(default=DocumentType.ALL)
     sort: SortBy = Field(default=SortBy.RELEVANCE)
     ranking: Ranking = Field(default=settings.LLM.RANKING)
     search_chain: Optional[SearchChain] = Field(alias="searchChain", default=None)
     hybrid: bool = settings.LLM.USE_HYBRID
 
 
 class DiscoveryPanelResponse(BaseModel):
@@ -302,7 +302,8 @@
     concepts: list[Concept] = Field(default=[])
     languages: list[Language] = Field(default=[])
     organizations: list[Union[Organization, OrganizationType]] = Field(default=[])
     places: list[Union[Place, Facility, Landmark]] = Field(default=[])
     products: list[Union[Product, ProductType]] = Field(default=[])
     sources: list[Source] = Field(default=[])
     topics: list[Topic] = Field(default=[])
+    people: list[Person] = Field(default=[])
```

### Comparing `bigdata_client-0.3.0/bigdata/api/uploads.py` & `bigdata_client-0.4.0/bigdata/api/uploads.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/api/watchlist.py` & `bigdata_client-0.4.0/bigdata/api/watchlist.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/auth.py` & `bigdata_client-0.4.0/bigdata/auth.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/clerk/authenticators/base_instance.py` & `bigdata_client-0.4.0/bigdata/clerk/authenticators/base_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/clerk/authenticators/dev_instance.py` & `bigdata_client-0.4.0/bigdata/clerk/authenticators/dev_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/clerk/authenticators/production_instance.py` & `bigdata_client-0.4.0/bigdata/clerk/authenticators/production_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/clerk/exceptions.py` & `bigdata_client-0.4.0/bigdata/clerk/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/clerk/sign_in_strategies/password.py` & `bigdata_client-0.4.0/bigdata/clerk/sign_in_strategies/password.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/clerk/token_manager.py` & `bigdata_client-0.4.0/bigdata/clerk/token_manager.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/clerk/token_manager_factory.py` & `bigdata_client-0.4.0/bigdata/clerk/token_manager_factory.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/connection.py` & `bigdata_client-0.4.0/bigdata/connection.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/daterange.py` & `bigdata_client-0.4.0/bigdata/daterange.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/entity_types.py` & `bigdata_client-0.4.0/bigdata/entity_types.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/enum_utils.py` & `bigdata_client-0.4.0/bigdata/enum_utils.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/models/advanced_search_query.py` & `bigdata_client-0.4.0/bigdata/models/advanced_search_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from abc import ABC, ABCMeta, abstractmethod
 from typing import Optional, Protocol, Union, runtime_checkable
 
+from bigdata.enum_utils import StrEnum
 from bigdata.models.search import (
-    DocumentTypes,
     Expression,
     ExpressionOperation,
     ExpressionTypes,
     FiscalQuarterValidator,
     FiscalYearValidator,
-    SectionTypes,
 )
 
 
 # Decorated with runtime_checkable to allow isinstance checks
 @runtime_checkable
 class QueryComponent(Protocol):
     """
@@ -27,14 +26,16 @@
 
     def __and__(self, other: "QueryComponent") -> "QueryComponent": ...
 
     def __or__(self, other: "QueryComponent") -> "QueryComponent": ...
 
     def __invert__(self) -> "QueryComponent": ...
 
+    def to_dict(self) -> dict: ...
+
 
 class BaseQueryComponent(ABC):
     """
     An abstract component that implements the common basic logic of the query
     components, like the AND, OR, and NOT operators.
     """
 
@@ -367,14 +368,24 @@
 
     def _quote(self, item: str) -> str:
         if item[0] == '"' and item[-1] == '"':
             return item
         return f'"{item}"'
 
 
+class Document(ListQueryComponent):
+    def __init__(
+        self, *items: str, operation: ExpressionOperation = ExpressionOperation.IN
+    ):
+        super().__init__(*items, operation=operation)
+
+    def get_expression_type(self) -> ExpressionTypes:
+        return ExpressionTypes.DOCUMENT
+
+
 class Similarity(ListQueryComponent):
     def __init__(
         self, *items: str, operation: ExpressionOperation = ExpressionOperation.ALL
     ):
         if operation == ExpressionOperation.IN:
             raise ValueError("Similarity does not support `|` (OR) operator")
         super().__init__(*items, operation=operation)
@@ -465,51 +476,86 @@
 
 
 class Source(ListQueryComponent):
     def get_expression_type(self) -> ExpressionTypes:
         return ExpressionTypes.SOURCE
 
 
-class SectionMetadata(BaseQueryComponent):
+class MetaBaseQueryComponentAndStrEnum(type(BaseQueryComponent), type(StrEnum)):
+    """Metaclass magic"""
+
 
-    def __init__(self, section_id: SectionTypes):
-        self.section_id = str(section_id)
+class SectionMetadata(
+    BaseQueryComponent, StrEnum, metaclass=MetaBaseQueryComponentAndStrEnum
+):
+    MANAGEMENT_DISCUSSION = "Management Discussion Section"
+    """Management Discussion Section"""
+    QA = "qa"
+    """QA"""
+    QUESTION = "question"
+    """question"""
+    ANSWER = "answer"
+    """answer"""
 
     def to_expression(self) -> Expression:
         return Expression(
             type=ExpressionTypes.SECTION_METADATA,
             operation=ExpressionOperation.IN,
-            value=[self.section_id],
+            value=[self.value],
         )
 
     def __repr__(self):
-        return f"SectionMetadata({self.section_id})"
+        return f"SectionMetadata({self.value})"
 
     def make_copy(self) -> QueryComponent:
         """Make a deep copy of the query component"""
-        return SectionMetadata(section_id=SectionTypes(self.section_id))
+        return SectionMetadata(self.value)
 
 
-class DocumentType(BaseQueryComponent):
-    def __init__(self, doc_type_id: DocumentTypes):
-        self.doc_type_id = str(doc_type_id)
+class TranscriptTypes(
+    BaseQueryComponent, StrEnum, metaclass=MetaBaseQueryComponentAndStrEnum
+):
+    ANALYST_INVESTOR_SHAREHOLDER_MEETING = "Analyst, Investor and Shareholder meeting"
+    """Analyst, Investor and Shareholder meeting"""
+    CONFERENCE_CALL = "General Conference Call"
+    """General Conference Call"""
+    GENERAL_PRESENTATION = "General Presentation"
+    """General Presentation"""
+    EARNINGS_CALL = "Earnings Call"
+    """Earnings Call"""
+    EARNINGS_RELEASE = "Earnings Release"
+    """Earnings Release"""
+    GUIDANCE_CALL = "Guidance Call"
+    """Guidance Call"""
+    SALES_REVENUE_CALL = "Sales and Revenue Call"
+    """Sales and Revenue Call"""
+    SALES_REVENUE_RELEASE = "Sales and Revenue Release"
+    """Sales and Revenue Release"""
+    SPECIAL_SITUATION_MA = "Special Situation, M&A and Other"
+    """Special Situation, M&A and Other"""
+    SHAREHOLDERS_MEETING = "Shareholders Meeting"
+    """Shareholders Meeting"""
+    MANAGEMENT_PLAN_ANNOUNCEMENT = "Management Plan Announcement"
+    """Management Plan Announcement"""
+    INVESTOR_CONFERENCE_CALL = "Investor Conference Call"
+    """Investor Conference Call"""
 
     def to_expression(self) -> Expression:
         return Expression(
             type=ExpressionTypes.DOCUMENT_TYPE,
             operation=ExpressionOperation.IN,
-            value=[self.doc_type_id],
+            value=[self.value],
         )
 
     def __repr__(self):
-        return f"DocumentType({self.doc_type_id})"
+        return f"TranscriptTypes('{self.value}')"
 
     def make_copy(self) -> QueryComponent:
         """Make a deep copy of the query component"""
-        return DocumentType(doc_type_id=DocumentTypes(self.doc_type_id))
+        return TranscriptTypes(self.value)
 
 
 class FiscalYear(ListQueryComponent):
     def __init__(
         self, *items: int, operation: ExpressionOperation = ExpressionOperation.IN
     ):
         # Validate the items but keep them stored raw, this is so FiscalYear can operate with itself
@@ -664,14 +710,37 @@
         self,
         fiscal_year: Optional[FiscalYear] = None,
         fiscal_quarter: Optional[FiscalQuarter] = None,
     ):
         self.fiscal_year = fiscal_year
         self.fiscal_quarter = fiscal_quarter
 
+    @staticmethod
+    def from_values(values: list[str]) -> "FiscalYearQuarterAggregate":
+        fiscal_years = []
+        fiscal_quarters = []
+        for value in values:
+            if value.endswith("FY"):
+                fiscal_years.append(int(value[:-2]))
+            elif value.startswith("FQ"):
+                fiscal_quarters.append(int(value[2:]))
+            else:
+                raise ValueError(
+                    f"Could not process {values} into FiscalYear and FiscalQuarter"
+                )
+        return FiscalYearQuarterAggregate(
+            fiscal_year=FiscalYear(*fiscal_years),
+            fiscal_quarter=FiscalQuarter(*fiscal_quarters),
+        )
+
+    def make_copy(self):
+        return FiscalYearQuarterAggregate(
+            fiscal_year=self.fiscal_year, fiscal_quarter=self.fiscal_quarter
+        )
+
 
 class ReportingPeriodWrapper(ListQueryComponent):
     """
     This is an class that will be used when the user combines FiscalYear and FiscalQuarter so that when the expression
     is generated elements from FiscalYear and FiscalQuarter are combined into the same values array.
     E.g:
     >>> (FiscalYear(2099) & FiscalQuarter(2) & FiscalQuarter(3)).to_dict()
@@ -692,16 +761,15 @@
             type=self.get_expression_type(),
             operation=self.operation,
             value=fiscal_quarters + fiscal_years,
         )
 
     def make_copy(self) -> QueryComponent:
         return ReportingPeriodWrapper(
-            fiscal_year=self.fiscal_year.make_copy(),
-            fiscal_quarter=self.fiscal_quarter.make_copy(),
+            *[item.make_copy() for item in self.items],
             operation=self.operation,
         )
 
     def get_expression_type(self) -> ExpressionTypes:
         return ExpressionTypes.REPORTING_PERIOD
 
     def _get_items_as_string(self) -> tuple[list[str]]:
@@ -982,7 +1050,18 @@
         if isinstance(expression.value, list):
             return AbsoluteDateRangeQuery(*expression.value)
         return RollingDateRangeQuery(expression.value)
     if expression.type == ExpressionTypes.CONTENT_TYPE:
         return ContentType(*expression.value, operation=expression.operation)
     if expression.type == ExpressionTypes.SENTIMENT:
         return Sentiment(expression.value, operation=expression.operation)
+    if expression.type == ExpressionTypes.REPORTING_PERIOD:
+        return ReportingPeriodWrapper(
+            FiscalYearQuarterAggregate.from_values(expression.value),
+            operation=expression.operation,
+        )
+    if expression.type == ExpressionTypes.SECTION_METADATA:
+        return SectionMetadata(expression.value[0])
+    if expression.type == ExpressionTypes.DOCUMENT_TYPE:
+        return TranscriptTypes(expression.value[0])
+    if expression.type == ExpressionTypes.DOCUMENT:
+        return Document(*expression.value, operation=expression.operation)
```

### Comparing `bigdata_client-0.3.0/bigdata/models/entities.py` & `bigdata_client-0.4.0/bigdata/models/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     Represents an entity in RavenPack's dataset.
     """
 
     model_config = ConfigDict(populate_by_name=True)
 
     id: str = Field(validation_alias="key")
     name: str
+    volume: Optional[int] = None
     # TODO: Add description to all entities
     # description: str
     entity_type: Literal["COMP"] = Field(default="COMP", validation_alias="entityType")
     company_type: Optional[str] = Field(validation_alias="group1", default=None)
     country: Optional[str] = Field(validation_alias="group2", default=None)
     sector: Optional[str] = Field(validation_alias="group3", default=None)
     industry_group: Optional[str] = Field(validation_alias="group4", default=None)
@@ -51,97 +52,106 @@
     ticker: Optional[str] = Field(validation_alias="metadata1", default=None)
 
 
 class Product(_AbstractEntity):
     model_config = ConfigDict(populate_by_name=True)
     id: str = Field(validation_alias="key")
     name: str
+    volume: Optional[int] = None
     entity_type: Literal["PROD"] = Field(default="PROD", validation_alias="entityType")
     product_type: str = Field(validation_alias="group1")
     product_owner: Optional[str] = Field(validation_alias="group2", default=None)
 
 
 class ProductType(_AbstractEntity):
     model_config = ConfigDict(populate_by_name=True)
     id: str = Field(validation_alias="key")
     name: str
+    volume: Optional[int] = None
     entity_type: Literal["PRDT"] = Field(default="PRDT", validation_alias="entityType")
 
 
 class Organization(_AbstractEntity):
     model_config = ConfigDict(populate_by_name=True)
     id: str = Field(validation_alias="key")
     name: str
+    volume: Optional[int] = None
     entity_type: Literal["ORGA"] = Field(default="ORGA", validation_alias="entityType")
     organization_type: Optional[str] = Field(validation_alias="group1", default=None)
     country: Optional[str] = Field(validation_alias="group2", default=None)
 
 
 class OrganizationType(_AbstractEntity):
     model_config = ConfigDict(populate_by_name=True)
     id: str = Field(validation_alias="key")
     name: str
+    volume: Optional[int] = None
     entity_type: Literal["ORGT"] = Field(default="ORGT", validation_alias="entityType")
 
 
 class Person(_AbstractEntity):
     """A person"""
 
     model_config = ConfigDict(populate_by_name=True)
     id: str = Field(validation_alias="key")
     name: str
+    volume: Optional[int] = None
     entity_type: Literal["PEOP"] = Field(default="PEOP", validation_alias="entityType")
     # Disabled but enabled for watchlists?
     position: Optional[str] = Field(validation_alias="group1", default=None)
     employer: Optional[str] = Field(validation_alias="group2", default=None)
     nationality: Optional[str] = Field(validation_alias="group3", default=None)
     gender: Optional[str] = Field(validation_alias="group4", default=None)
 
 
 class Place(_AbstractEntity):
     """A place. E.g. a country, city, etc."""
 
     model_config = ConfigDict(populate_by_name=True)
     id: str = Field(validation_alias="key")
     name: str
+    volume: Optional[int] = None
     entity_type: Literal["PLCE"] = Field(default="PLCE", validation_alias="entityType")
     place_type: str = Field(validation_alias="group2")
     country: Optional[str] = Field(validation_alias="group4", default=None)
     region: Optional[str] = Field(validation_alias="group5", default=None)
 
 
 class Facility(_AbstractEntity):
     """A facility. E.g. a factory, a mine, etc."""
 
     model_config = ConfigDict(populate_by_name=True)
     id: str = Field(validation_alias="key")
     name: str
+    volume: Optional[int] = None
     entity_type: Literal["FCTY"] = Field(default="FCTY", validation_alias="entityType")
     country: Optional[str] = Field(validation_alias="group4", default=None)
     region: Optional[str] = Field(validation_alias="group5", default=None)
 
 
 class Landmark(_AbstractEntity):
     """A landmark. E.g. a mountain, a lake, etc."""
 
     model_config = ConfigDict(populate_by_name=True)
     id: str = Field(validation_alias="key")
     name: str
+    volume: Optional[int] = None
     entity_type: Literal["LAND"] = Field(default="LAND", validation_alias="entityType")
     landmark_type: str = Field(validation_alias="group2")
     country: Optional[str] = Field(validation_alias="group4", default=None)
     region: Optional[str] = Field(validation_alias="group5", default=None)
 
 
 class Concept(_AbstractEntity):
     """Basically everything else"""
 
     model_config = ConfigDict(populate_by_name=True)
     id: str = Field(validation_alias="key")
     name: str
+    volume: Optional[int] = None
     entity_type: str = Field(
         validation_alias="entityType"
     )  # Should belong in EntityType
     entity_type_name: str = Field(validation_alias="group1")
     concept_level_2: Optional[str] = Field(validation_alias="group2", default=None)
     concept_level_3: Optional[str] = Field(validation_alias="group3", default=None)
     concept_level_4: Optional[str] = Field(validation_alias="group4", default=None)
```

### Comparing `bigdata_client-0.3.0/bigdata/models/languages.py` & `bigdata_client-0.4.0/bigdata/models/languages.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Literal
+from typing import Literal, Optional
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from bigdata.models.advanced_search_query import Language as LanguageQuery
 from bigdata.models.advanced_search_query import QueryComponent
 from bigdata.models.search import Expression
 
 
 class Language(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     id: str = Field(validation_alias="key")
     name: str
+    volume: Optional[int] = None
     query_type: Literal["language"] = Field(
         default="language", validation_alias="queryType"
     )
 
     # QueryComponent methods
 
     @property
```

### Comparing `bigdata_client-0.3.0/bigdata/models/parse.py` & `bigdata_client-0.4.0/bigdata/models/parse.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/models/sources.py` & `bigdata_client-0.4.0/bigdata/models/sources.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 class Source(BaseModel):
     """A source of news and information for RavenPack"""
 
     model_config = ConfigDict(populate_by_name=True, alias_generator=to_camel)
     id: str
     name: str
+    volume: Optional[int] = None
     entity_type: Literal["SRCE"] = Field(default="SRCE")
     publication_type: str
     language: Optional[str] = Field(default=None)
     country: str
     source_rank: Optional[str] = Field(default=None)
     provider_id: str
     url: str
```

### Comparing `bigdata_client-0.3.0/bigdata/models/story.py` & `bigdata_client-0.4.0/bigdata/models/document.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 from dataclasses import dataclass
 from enum import Enum
 
 from bigdata.query_type import QueryType
 
 
 @dataclass
-class StorySource:
-    """The source of a story"""
+class DocumentSource:
+    """The source of a document"""
 
     key: str
     name: str
     rank: int
 
 
-class StoryType(Enum):
+class DocType(Enum):
     """
-    The type of the story. A news, a transcript or an uploaded file.
+    The type of the document.
     """
 
     NEWS = "news"
+    FILINGS = "filings"
     TRANSCRIPTS = "transcripts"
     FILES = "files"
 
 
 @dataclass
-class StorySentenceEntity:
+class DocumentSentenceEntity:
     """
     A detection instance of an entity in a sentence
     """
 
     key: str
     start: int
     end: int
     query_type: QueryType
 
 
 @dataclass
-class StorySentence:
+class DocumentSentence:
     paragraph: int
     sentence: int
 
 
 @dataclass
-class StoryChunk:
+class DocumentChunk:
     """
     A chunk of text representing a contextual unit within the document
     """
 
     text: str
     chunk: int
-    entities: list[StorySentenceEntity]
-    sentences: list[StorySentence]
+    entities: list[DocumentSentenceEntity]
+    sentences: list[DocumentSentence]
     relevance: float
     sentiment: float
```

### Comparing `bigdata_client-0.3.0/bigdata/models/topics.py` & `bigdata_client-0.4.0/bigdata/models/topics.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from bigdata.models.search import Expression
 
 
 class Topic(BaseModel):
     model_config = ConfigDict(populate_by_name=True, alias_generator=to_camel)
     id: str
     name: str
+    volume: Optional[int] = None
     # Disabled, but enabled for watchlists?
     topic: Optional[str]
     topic_group: Optional[str]
     entity_type: Literal["TOPC"] = Field(default="TOPC")
     # Disabled fields.
     # topic_type: str = Field(validation_alias="group3")
     # topic_subtype: str = Field(validation_alias="group4")
```

### Comparing `bigdata_client-0.3.0/bigdata/models/uploads.py` & `bigdata_client-0.4.0/bigdata/models/uploads.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/models/watchlists.py` & `bigdata_client-0.4.0/bigdata/models/watchlists.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.3.0/bigdata/query.py` & `bigdata_client-0.4.0/bigdata/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 This is for the user to import
 """
 
 # Coming soon:
 # from bigdata.models.advanced_search_query import ContentType  # pyright: ignore
 # from bigdata.models.advanced_search_query import Sentiment  # pyright: ignore
 
-from bigdata.models.advanced_search_query import DocumentType  # pyright: ignore
+from bigdata.models.advanced_search_query import Document  # pyright: ignore
 from bigdata.models.advanced_search_query import Entity  # pyright: ignore
 from bigdata.models.advanced_search_query import FiscalQuarter  # pyright: ignore
 from bigdata.models.advanced_search_query import FiscalYear  # pyright: ignore
 from bigdata.models.advanced_search_query import Keyword  # pyright: ignore
 from bigdata.models.advanced_search_query import Language  # pyright: ignore
 from bigdata.models.advanced_search_query import SectionMetadata  # pyright: ignore
 from bigdata.models.advanced_search_query import Similarity  # pyright: ignore
 from bigdata.models.advanced_search_query import Source  # pyright: ignore
 from bigdata.models.advanced_search_query import Topic  # pyright: ignore
+from bigdata.models.advanced_search_query import TranscriptTypes  # pyright: ignore
 from bigdata.models.advanced_search_query import Watchlist  # pyright: ignore
 from bigdata.models.advanced_search_query import all_  # pyright: ignore
 from bigdata.models.advanced_search_query import any_  # pyright: ignore
```

### Comparing `bigdata_client-0.3.0/bigdata/search.py` & `bigdata_client-0.4.0/bigdata/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,24 @@
     ShareSavedSearchRequest,
     UpdateSearchRequest,
     UserQueryShareCompanyContext,
 )
 from bigdata.connection import BigdataConnection
 from bigdata.constants import MAX_SEARCH_PAGES
 from bigdata.daterange import AbsoluteDateRange, RollingDateRange
+from bigdata.document import Document
 from bigdata.models.advanced_search_query import QueryComponent
 from bigdata.models.comentions import Comentions
-from bigdata.models.search import FileType, SearchSharePermission, SortBy
-from bigdata.story import Story
+from bigdata.models.search import DocumentType, SearchSharePermission, SortBy
 
 
 class Search:
     """
     Class representing a search, saved or not.
-    It allows you to perform searches in bigdata, getting stories, or get the
+    It allows you to perform searches in bigdata, getting documents, or get the
     co-mentions for that search.
     It also allows you to save, update, delete and share the search.
     """
 
     def __init__(
         self,
         api: BigdataConnection,
@@ -45,15 +45,15 @@
     @classmethod
     def from_query(
         cls,
         api: "BigdataConnection",
         query: QueryComponent,
         date_range: Optional[Union[AbsoluteDateRange, RollingDateRange]] = None,
         sortby: SortBy = SortBy.RELEVANCE,
-        scope: FileType = FileType.ALL,
+        scope: DocumentType = DocumentType.ALL,
     ) -> "Search":
         """
         Create a search object given a query, a date range, a scope filter and sort by
         """
         rpx_query = AdvancedSearchQuery(
             date_range=date_range, query=query, sortby=sortby, scope=scope
         )
@@ -75,19 +75,23 @@
             id=response.id,
             name=response.name,
             company_shared_permission=company_permission,
             # TODO: Add the rest of the parameters like created_at, updated_at,
             # owner, etc.
         )
 
-    def limit_stories(self, limit: int) -> Iterable[Story]:
-        """Limit the number of stories returned by this search"""
+    def limit_documents(self, limit: int) -> Iterable[Document]:
+        """Return the first `limit` documents of the search as a generator"""
         new = self.make_copy()
         return SearchResults(new, limit=limit)
 
+    def run(self, limit: int) -> list[Document]:
+        """Return the first `limit` documents of the search as a list"""
+        return list(self.limit_documents(limit))
+
     def get_comentions(self) -> Comentions:
         """Get the comentions of the search"""
         if self._api is None:
             raise ValueError("The search object must have an API to get comentions.")
         request = self.query.to_discovery_panel_api_request()
         response = self._api.query_discovery_panel(request)
         return Comentions.from_response(response)
@@ -183,24 +187,24 @@
         return self._company_shared_permission
 
 
 # To be changed. It shouldn't be a dataclass, but for now it's fine
 @dataclass
 class SearchResults:
     """
-    A search with a limit. It allows you to get the count of stories, and/or get
+    A search with a limit. It allows you to get the count of documents, and/or get
     an iterator over the results.
     """
 
     def __init__(self, search: Search, limit: int):
         self.search = search
         self._first_page: Optional[QueryClustersResponse] = None
         if limit <= 0:
             raise ValueError("The limit must be a positive number.")
-        self._limit_stories = limit
+        self._limit_documents = limit
 
     @property
     def _sentence_count(self) -> int:
         """
         INTERNAL!!
         Do not rely on this because it may not mean what you think it means, and
         could change.
@@ -218,48 +222,48 @@
         return first_page.document_count
 
     def _ensure_first_page(self) -> QueryClustersResponse:
         if self._first_page is None:
             self._first_page = self.search.get_page()
         return self._first_page
 
-    def __iter__(self) -> Iterable[Story]:
+    def __iter__(self) -> Iterable[Document]:
         return iter(
             SearchResultsPaginatorIterator(
-                self.search, self._limit_stories, self._first_page
+                self.search, self._limit_documents, self._first_page
             )
         )
 
 
 class SearchResultsPaginatorIterator:
     """
-    Helper to iterate over the stories in all the pages.
+    Helper to iterate over the documents in all the pages.
     Optionally, it can skip the first request and use the first_page parameter.
     """
 
     def __init__(
         self,
         search: Search,
-        limit_stories: int,
+        limit: int,
         first_page: Optional[QueryClustersResponse],
     ):
         self.search = search
         self.current_page = first_page or None
-        self._limit_stories = limit_stories
+        self._limit = limit
         self._page_num = 0
 
-    def __iter__(self) -> Iterator[Story]:
+    def __iter__(self) -> Iterator[Document]:
         # The first page may have been provided, if the user asked for the count first
         if self.current_page is None:
             self.current_page = self.search.get_page()
         items = 0
         for _ in range(MAX_SEARCH_PAGES):  # Effectively a while(True), but safer
-            for story in self.current_page.stories:
-                if items >= self._limit_stories:
+            for document in self.current_page.stories:
+                if items >= self._limit:
                     return
                 items += 1
-                yield Story.from_response(story)
+                yield Document.from_response(document)
             next_page = self.current_page.next_cursor
             if not next_page:
                 break
             self._page_num = next_page
             self.current_page = self.search.get_page(self._page_num)
```

### Comparing `bigdata_client-0.3.0/bigdata/settings.py` & `bigdata_client-0.4.0/bigdata/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,32 +7,24 @@
 
 
 class ClerkInstanceType(str, Enum):
     DEV = "DEV"
     PROD = "PROD"
 
 
-class BigdataAuthType(str, Enum):
-    CLERK = "CLERK"
-    OLD = "OLD"
-
-
 class LLMSettings(BaseSettings):
     USE_HYBRID: bool = True
     RANKING: Ranking = Ranking.STABLE
 
 
 class Settings(
     BaseSettings
 ):  # FIXME OLD AUTH remove Clerk config when old auth is removed
     PACKAGE_NAME: str = "bigdata-client"  # The name of the python package
     BIGDATA_API_URL: HttpUrl = "https://api.bigdata.com"
     UPLOAD_API_URL: HttpUrl = "https://upload.ravenpack.com/1.0/"
-    BIGDATA_AUTH_TYPE: BigdataAuthType = BigdataAuthType.CLERK
     CLERK_INSTANCE_TYPE: ClerkInstanceType = ClerkInstanceType.PROD
-    # TODO: Change to another endpoint as we need the refresh token
-    AUTH_LOGIN_FORM_ENDPOINT: HttpUrl = "https://auth.ravenpack.com/2.0/login"
     CLERK_FRONTEND_URL: HttpUrl = "https://clerk.bigdata.com/v1"
     LLM: LLMSettings = LLMSettings()
 
 
 settings = Settings()
```

### Comparing `bigdata_client-0.3.0/pyproject.toml` & `bigdata_client-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "bigdata-client"
 packages = [
     { include = "bigdata" },
 ]
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = [
     "Bigdata Team <support@bigdata.com>"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `bigdata_client-0.3.0/PKG-INFO` & `bigdata_client-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigdata-client
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: Bigdata Team
 Author-email: support@bigdata.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

