# Comparing `tmp/ai21-2.3.1.tar.gz` & `tmp/ai21-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-2.3.1.tar", max compression
+gzip compressed data, was "ai21-2.4.0.tar", max compression
```

## Comparing `ai21-2.3.1.tar` & `ai21-2.4.0.tar`

### file list

```diff
@@ -1,105 +1,107 @@
--rw-r--r--   0        0        0    11357 2024-05-22 18:06:40.054503 ai21-2.3.1/LICENSE
--rw-r--r--   0        0        0    13215 2024-05-22 18:06:40.058503 ai21-2.3.1/README.md
--rw-r--r--   0        0        0     1575 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/__init__.py
--rw-r--r--   0        0        0     2516 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/ai21_env_config.py
--rw-r--r--   0        0        0     2703 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/ai21_http_client.py
--rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/__init__.py
--rw-r--r--   0        0        0      844 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/ai21_bedrock_client.py
--rw-r--r--   0        0        0       92 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/bedrock_model_id.py
--rw-r--r--   0        0        0     2414 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/bedrock_session.py
--rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/resources/__init__.py
--rw-r--r--   0        0        0     1996 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/resources/bedrock_completion.py
--rw-r--r--   0        0        0      522 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/resources/bedrock_resource.py
--rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/__init__.py
--rw-r--r--   0        0        0      857 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/answer_base.py
--rw-r--r--   0        0        0     3594 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/chat_base.py
--rw-r--r--   0        0        0     4081 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/completion_base.py
--rw-r--r--   0        0        0     1496 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/custom_model_base.py
--rw-r--r--   0        0        0     1723 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/dataset_base.py
--rw-r--r--   0        0        0      770 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/embed_base.py
--rw-r--r--   0        0        0      577 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/gec_base.py
--rw-r--r--   0        0        0      639 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/improvements_base.py
--rw-r--r--   0        0        0     1478 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/paraphrase_base.py
--rw-r--r--   0        0        0      674 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/segmentation_base.py
--rw-r--r--   0        0        0     1217 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/summarize_base.py
--rw-r--r--   0        0        0      999 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/summarize_by_segment_base.py
--rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/__init__.py
--rw-r--r--   0        0        0     1545 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/ai21_sagemaker_client.py
--rw-r--r--   0        0        0      154 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/constants.py
--rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/__init__.py
--rw-r--r--   0        0        0      498 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_answer.py
--rw-r--r--   0        0        0     3194 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_completion.py
--rw-r--r--   0        0        0      399 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_gec.py
--rw-r--r--   0        0        0      789 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py
--rw-r--r--   0        0        0      484 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_resource.py
--rw-r--r--   0        0        0      810 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_summarize.py
--rw-r--r--   0        0        0     2522 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/sagemaker_session.py
--rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/__init__.py
--rw-r--r--   0        0        0     3496 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/ai21_client.py
--rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/__init__.py
--rw-r--r--   0        0        0      101 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/chat/__init__.py
--rw-r--r--   0        0        0     3647 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/chat/chat_completions.py
--rw-r--r--   0        0        0      550 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_answer.py
--rw-r--r--   0        0        0     2036 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_chat.py
--rw-r--r--   0        0        0     2006 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_completion.py
--rw-r--r--   0        0        0     1301 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_custom_model.py
--rw-r--r--   0        0        0     1455 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_dataset.py
--rw-r--r--   0        0        0      560 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_embed.py
--rw-r--r--   0        0        0      446 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_gec.py
--rw-r--r--   0        0        0      722 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_improvements.py
--rw-r--r--   0        0        0     4100 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_library.py
--rw-r--r--   0        0        0      854 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_paraphrase.py
--rw-r--r--   0        0        0     2808 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_resource.py
--rw-r--r--   0        0        0      587 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_segmentation.py
--rw-r--r--   0        0        0      871 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_summarize.py
--rw-r--r--   0        0        0      772 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_summarize_by_segment.py
--rw-r--r--   0        0        0       64 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/constants.py
--rw-r--r--   0        0        0     2821 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/errors.py
--rw-r--r--   0        0        0     5373 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/http_client.py
--rw-r--r--   0        0        0      484 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/logger.py
--rw-r--r--   0        0        0     2633 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/__init__.py
--rw-r--r--   0        0        0      262 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/ai21_base_model_mixin.py
--rw-r--r--   0        0        0      510 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/chat/__init__.py
--rw-r--r--   0        0        0      651 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      592 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/chat/chat_completion_response.py
--rw-r--r--   0        0        0      219 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/chat/chat_message.py
--rw-r--r--   0        0        0       97 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/chat/role_type.py
--rw-r--r--   0        0        0      233 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/chat_message.py
--rw-r--r--   0        0        0       89 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/document_type.py
--rw-r--r--   0        0        0       96 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/embed_type.py
--rw-r--r--   0        0        0      286 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/improvement_type.py
--rw-r--r--   0        0        0      410 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/logprobs.py
--rw-r--r--   0        0        0      168 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/paraphrase_style_type.py
--rw-r--r--   0        0        0      503 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/penalty.py
--rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/__init__.py
--rw-r--r--   0        0        0      273 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/answer_response.py
--rw-r--r--   0        0        0      518 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/chat_response.py
--rw-r--r--   0        0        0      786 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/completion_response.py
--rw-r--r--   0        0        0      713 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/custom_model_response.py
--rw-r--r--   0        0        0      376 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/dataset_response.py
--rw-r--r--   0        0        0      300 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/embed_response.py
--rw-r--r--   0        0        0      550 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/file_response.py
--rw-r--r--   0        0        0      635 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/gec_response.py
--rw-r--r--   0        0        0      401 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/improvement_response.py
--rw-r--r--   0        0        0      469 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/library_answer_response.py
--rw-r--r--   0        0        0      450 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/library_search_response.py
--rw-r--r--   0        0        0      294 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/paraphrase_response.py
--rw-r--r--   0        0        0      317 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/segmentation_response.py
--rw-r--r--   0        0        0      564 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/summarize_by_segment_response.py
--rw-r--r--   0        0        0      187 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/summarize_response.py
--rw-r--r--   0        0        0      139 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/summary_method.py
--rw-r--r--   0        0        0      222 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/usage_info.py
--rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/py.typed
--rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/services/__init__.py
--rw-r--r--   0        0        0     2310 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/services/sagemaker.py
--rw-r--r--   0        0        0     2105 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/stream.py
--rw-r--r--   0        0        0      123 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/tokenizers/__init__.py
--rw-r--r--   0        0        0      608 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/tokenizers/ai21_tokenizer.py
--rw-r--r--   0        0        0      628 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/tokenizers/factory.py
--rw-r--r--   0        0        0     1074 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/types.py
--rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/utils/__init__.py
--rw-r--r--   0        0        0      989 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/utils/typing.py
--rw-r--r--   0        0        0       18 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/version.py
--rw-r--r--   0        0        0     2286 2024-05-22 18:06:40.062503 ai21-2.3.1/pyproject.toml
--rw-r--r--   0        0        0    13966 1970-01-01 00:00:00.000000 ai21-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 12:38:37.065813 ai21-2.4.0/LICENSE
+-rw-r--r--   0        0        0    13215 2024-05-28 12:38:37.065813 ai21-2.4.0/README.md
+-rw-r--r--   0        0        0     1575 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/__init__.py
+-rw-r--r--   0        0        0     2516 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/ai21_env_config.py
+-rw-r--r--   0        0        0     2703 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/ai21_http_client.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/bedrock/__init__.py
+-rw-r--r--   0        0        0      844 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/bedrock/ai21_bedrock_client.py
+-rw-r--r--   0        0        0       92 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/bedrock/bedrock_model_id.py
+-rw-r--r--   0        0        0     2414 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/bedrock/bedrock_session.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/bedrock/resources/__init__.py
+-rw-r--r--   0        0        0     1996 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/bedrock/resources/bedrock_completion.py
+-rw-r--r--   0        0        0      522 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/bedrock/resources/bedrock_resource.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/answer_base.py
+-rw-r--r--   0        0        0     3594 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/chat_base.py
+-rw-r--r--   0        0        0     4081 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/completion_base.py
+-rw-r--r--   0        0        0     1496 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/custom_model_base.py
+-rw-r--r--   0        0        0     1723 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/dataset_base.py
+-rw-r--r--   0        0        0      770 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/embed_base.py
+-rw-r--r--   0        0        0      577 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/gec_base.py
+-rw-r--r--   0        0        0      639 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/improvements_base.py
+-rw-r--r--   0        0        0     1478 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/paraphrase_base.py
+-rw-r--r--   0        0        0      674 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/segmentation_base.py
+-rw-r--r--   0        0        0     1217 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/summarize_base.py
+-rw-r--r--   0        0        0      999 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/common/summarize_by_segment_base.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/sagemaker/__init__.py
+-rw-r--r--   0        0        0     1545 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/sagemaker/ai21_sagemaker_client.py
+-rw-r--r--   0        0        0      154 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/sagemaker/constants.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/sagemaker/resources/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/sagemaker/resources/sagemaker_answer.py
+-rw-r--r--   0        0        0     3194 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/sagemaker/resources/sagemaker_completion.py
+-rw-r--r--   0        0        0      399 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/sagemaker/resources/sagemaker_gec.py
+-rw-r--r--   0        0        0      789 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py
+-rw-r--r--   0        0        0      484 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/sagemaker/resources/sagemaker_resource.py
+-rw-r--r--   0        0        0      810 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/sagemaker/resources/sagemaker_summarize.py
+-rw-r--r--   0        0        0     2522 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/sagemaker/sagemaker_session.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/__init__.py
+-rw-r--r--   0        0        0     3597 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/ai21_client.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/beta/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/beta/beta.py
+-rw-r--r--   0        0        0      101 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/chat/__init__.py
+-rw-r--r--   0        0        0     3647 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/chat/chat_completions.py
+-rw-r--r--   0        0        0      550 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_answer.py
+-rw-r--r--   0        0        0     2036 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_chat.py
+-rw-r--r--   0        0        0     2006 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_completion.py
+-rw-r--r--   0        0        0     1301 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_custom_model.py
+-rw-r--r--   0        0        0     1455 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_dataset.py
+-rw-r--r--   0        0        0      560 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_embed.py
+-rw-r--r--   0        0        0      446 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_gec.py
+-rw-r--r--   0        0        0      722 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_improvements.py
+-rw-r--r--   0        0        0     4100 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_library.py
+-rw-r--r--   0        0        0      854 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_paraphrase.py
+-rw-r--r--   0        0        0     2808 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_resource.py
+-rw-r--r--   0        0        0      587 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_segmentation.py
+-rw-r--r--   0        0        0      871 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_summarize.py
+-rw-r--r--   0        0        0      772 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/clients/studio/resources/studio_summarize_by_segment.py
+-rw-r--r--   0        0        0       64 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/constants.py
+-rw-r--r--   0        0        0     2821 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/errors.py
+-rw-r--r--   0        0        0     5373 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/http_client.py
+-rw-r--r--   0        0        0      484 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/logger.py
+-rw-r--r--   0        0        0     2633 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/__init__.py
+-rw-r--r--   0        0        0      262 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/ai21_base_model_mixin.py
+-rw-r--r--   0        0        0      510 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/chat/__init__.py
+-rw-r--r--   0        0        0      651 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      592 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/chat/chat_completion_response.py
+-rw-r--r--   0        0        0      219 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/chat/chat_message.py
+-rw-r--r--   0        0        0       97 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/chat/role_type.py
+-rw-r--r--   0        0        0      233 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/chat_message.py
+-rw-r--r--   0        0        0       89 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/document_type.py
+-rw-r--r--   0        0        0       96 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/embed_type.py
+-rw-r--r--   0        0        0      286 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/improvement_type.py
+-rw-r--r--   0        0        0      410 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/logprobs.py
+-rw-r--r--   0        0        0      168 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/paraphrase_style_type.py
+-rw-r--r--   0        0        0      503 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/penalty.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/responses/__init__.py
+-rw-r--r--   0        0        0      273 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/responses/answer_response.py
+-rw-r--r--   0        0        0      518 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/responses/chat_response.py
+-rw-r--r--   0        0        0      786 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/responses/completion_response.py
+-rw-r--r--   0        0        0      713 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/responses/custom_model_response.py
+-rw-r--r--   0        0        0      376 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/responses/dataset_response.py
+-rw-r--r--   0        0        0      300 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/responses/embed_response.py
+-rw-r--r--   0        0        0      550 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/responses/file_response.py
+-rw-r--r--   0        0        0      635 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/responses/gec_response.py
+-rw-r--r--   0        0        0      401 2024-05-28 12:38:37.065813 ai21-2.4.0/ai21/models/responses/improvement_response.py
+-rw-r--r--   0        0        0      469 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/models/responses/library_answer_response.py
+-rw-r--r--   0        0        0      482 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/models/responses/library_search_response.py
+-rw-r--r--   0        0        0      294 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/models/responses/paraphrase_response.py
+-rw-r--r--   0        0        0      317 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/models/responses/segmentation_response.py
+-rw-r--r--   0        0        0      564 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/models/responses/summarize_by_segment_response.py
+-rw-r--r--   0        0        0      187 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/models/responses/summarize_response.py
+-rw-r--r--   0        0        0      139 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/models/summary_method.py
+-rw-r--r--   0        0        0      222 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/models/usage_info.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/py.typed
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/services/__init__.py
+-rw-r--r--   0        0        0     2310 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/services/sagemaker.py
+-rw-r--r--   0        0        0     2105 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/stream.py
+-rw-r--r--   0        0        0      123 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/tokenizers/__init__.py
+-rw-r--r--   0        0        0      608 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/tokenizers/ai21_tokenizer.py
+-rw-r--r--   0        0        0      628 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/tokenizers/factory.py
+-rw-r--r--   0        0        0     1074 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/types.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/utils/__init__.py
+-rw-r--r--   0        0        0      989 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/utils/typing.py
+-rw-r--r--   0        0        0       18 2024-05-28 12:38:37.069813 ai21-2.4.0/ai21/version.py
+-rw-r--r--   0        0        0     2286 2024-05-28 12:38:37.069813 ai21-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13966 1970-01-01 00:00:00.000000 ai21-2.4.0/PKG-INFO
```

### Comparing `ai21-2.3.1/LICENSE` & `ai21-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/README.md` & `ai21-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/__init__.py` & `ai21-2.4.0/ai21/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/ai21_env_config.py` & `ai21-2.4.0/ai21/ai21_env_config.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/ai21_http_client.py` & `ai21-2.4.0/ai21/ai21_http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/bedrock/ai21_bedrock_client.py` & `ai21-2.4.0/ai21/clients/bedrock/ai21_bedrock_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/bedrock/bedrock_session.py` & `ai21-2.4.0/ai21/clients/bedrock/bedrock_session.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/bedrock/resources/bedrock_completion.py` & `ai21-2.4.0/ai21/clients/bedrock/resources/bedrock_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/bedrock/resources/bedrock_resource.py` & `ai21-2.4.0/ai21/clients/bedrock/resources/bedrock_resource.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/common/answer_base.py` & `ai21-2.4.0/ai21/clients/common/answer_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/common/chat_base.py` & `ai21-2.4.0/ai21/clients/common/chat_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/common/completion_base.py` & `ai21-2.4.0/ai21/clients/common/completion_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/common/custom_model_base.py` & `ai21-2.4.0/ai21/clients/common/custom_model_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/common/dataset_base.py` & `ai21-2.4.0/ai21/clients/common/dataset_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/common/embed_base.py` & `ai21-2.4.0/ai21/clients/common/embed_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/common/gec_base.py` & `ai21-2.4.0/ai21/clients/common/gec_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/common/improvements_base.py` & `ai21-2.4.0/ai21/clients/common/improvements_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/common/paraphrase_base.py` & `ai21-2.4.0/ai21/clients/common/paraphrase_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/common/segmentation_base.py` & `ai21-2.4.0/ai21/clients/common/segmentation_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/common/summarize_base.py` & `ai21-2.4.0/ai21/clients/common/summarize_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/common/summarize_by_segment_base.py` & `ai21-2.4.0/ai21/clients/common/summarize_by_segment_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/sagemaker/ai21_sagemaker_client.py` & `ai21-2.4.0/ai21/clients/sagemaker/ai21_sagemaker_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_completion.py` & `ai21-2.4.0/ai21/clients/sagemaker/resources/sagemaker_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py` & `ai21-2.4.0/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_summarize.py` & `ai21-2.4.0/ai21/clients/sagemaker/resources/sagemaker_summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/sagemaker/sagemaker_session.py` & `ai21-2.4.0/ai21/clients/sagemaker/sagemaker_session.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/ai21_client.py` & `ai21-2.4.0/ai21/clients/studio/ai21_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import warnings
 from typing import Optional, Any, Dict
 
 from ai21_tokenizer import PreTrainedTokenizers
 
 from ai21.ai21_env_config import _AI21EnvConfig, AI21EnvConfig
 from ai21.ai21_http_client import AI21HTTPClient
+from ai21.clients.studio.resources.beta.beta import Beta
 from ai21.clients.studio.resources.studio_answer import StudioAnswer
 from ai21.clients.studio.resources.studio_chat import StudioChat
 from ai21.clients.studio.resources.studio_completion import StudioCompletion
 from ai21.clients.studio.resources.studio_custom_model import StudioCustomModel
 from ai21.clients.studio.resources.studio_dataset import StudioDataset
 from ai21.clients.studio.resources.studio_embed import StudioEmbed
 from ai21.clients.studio.resources.studio_gec import StudioGEC
@@ -61,14 +62,15 @@
         self.paraphrase = StudioParaphrase(self._http_client)
         self.summarize_by_segment = StudioSummarizeBySegment(self._http_client)
         self.custom_model = StudioCustomModel(self._http_client)
         self.dataset = StudioDataset(self._http_client)
         self.answer = StudioAnswer(self._http_client)
         self.library = StudioLibrary(self._http_client)
         self.segmentation = StudioSegmentation(self._http_client)
+        self.beta = Beta(self._http_client)
 
     def count_tokens(self, text: str, tokenizer_name: str = PreTrainedTokenizers.J2_TOKENIZER) -> int:
         warnings.warn(
             "Please use the global get_tokenizer() method directly instead of the AI21Client().count_tokens() method.",
             DeprecationWarning,
         )
```

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/chat/chat_completions.py` & `ai21-2.4.0/ai21/clients/studio/resources/chat/chat_completions.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_answer.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_answer.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_chat.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_chat.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_completion.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_custom_model.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_dataset.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_dataset.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_embed.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_embed.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_improvements.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_improvements.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_library.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_library.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_paraphrase.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_resource.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_resource.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_segmentation.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_segmentation.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_summarize.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/clients/studio/resources/studio_summarize_by_segment.py` & `ai21-2.4.0/ai21/clients/studio/resources/studio_summarize_by_segment.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/errors.py` & `ai21-2.4.0/ai21/errors.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/http_client.py` & `ai21-2.4.0/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/models/__init__.py` & `ai21-2.4.0/ai21/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/models/chat/chat_completion_chunk.py` & `ai21-2.4.0/ai21/models/chat/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/models/chat/chat_completion_response.py` & `ai21-2.4.0/ai21/models/chat/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/models/responses/chat_response.py` & `ai21-2.4.0/ai21/models/responses/chat_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/models/responses/completion_response.py` & `ai21-2.4.0/ai21/models/responses/completion_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/models/responses/custom_model_response.py` & `ai21-2.4.0/ai21/models/responses/custom_model_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/models/responses/file_response.py` & `ai21-2.4.0/ai21/models/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/models/responses/gec_response.py` & `ai21-2.4.0/ai21/models/responses/gec_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/models/responses/summarize_by_segment_response.py` & `ai21-2.4.0/ai21/models/responses/summarize_by_segment_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/services/sagemaker.py` & `ai21-2.4.0/ai21/services/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/stream.py` & `ai21-2.4.0/ai21/stream.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/tokenizers/ai21_tokenizer.py` & `ai21-2.4.0/ai21/tokenizers/ai21_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/tokenizers/factory.py` & `ai21-2.4.0/ai21/tokenizers/factory.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/types.py` & `ai21-2.4.0/ai21/types.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/ai21/utils/typing.py` & `ai21-2.4.0/ai21/utils/typing.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.1/pyproject.toml` & `ai21-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
   "if typing.TYPE_CHECKING:"
 ]
 
 [tool.poetry]
 name = "ai21"
-version = "2.3.1"
+version = "2.4.0"
 description = ""
 authors = ["AI21 Labs"]
 readme = "README.md"
 packages = [
     { include = "ai21" }
 ]
```

### Comparing `ai21-2.3.1/PKG-INFO` & `ai21-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 2.3.1
+Version: 2.4.0
 Summary: 
 Author: AI21 Labs
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ai21 Version: 2.3.1 Summary: Author: AI21 Labs
+Metadata-Version: 2.1 Name: ai21 Version: 2.4.0 Summary: Author: AI21 Labs
 Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Provides-Extra: aws Requires-Dist: ai21-tokenizer
 (>=0.9.1,<1.0.0) Requires-Dist: boto3 (>=1.28.82,<2.0.0) ; extra == "aws"
 Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0) Requires-Dist: httpx
```

