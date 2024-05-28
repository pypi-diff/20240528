# Comparing `tmp/friendli_client-1.3.4.tar.gz` & `tmp/friendli_client-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "friendli_client-1.3.4.tar", max compression
+gzip compressed data, was "friendli_client-1.3.5.tar", max compression
```

## Comparing `friendli_client-1.3.4.tar` & `friendli_client-1.3.5.tar`

### file list

```diff
@@ -1,143 +1,146 @@
--rw-r--r--   0        0        0    10173 2024-04-02 02:48:33.811614 friendli_client-1.3.4/LICENSE
--rw-r--r--   0        0        0     6417 2024-04-02 02:48:33.811690 friendli_client-1.3.4/README.md
--rw-r--r--   0        0        0      615 2024-04-02 02:48:33.811781 friendli_client-1.3.4/friendli/__init__.py
--rw-r--r--   0        0        0     5840 2024-04-02 02:48:33.811867 friendli_client-1.3.4/friendli/auth.py
--rw-r--r--   0        0        0      188 2024-04-02 02:48:33.811963 friendli_client-1.3.4/friendli/cli/__init__.py
--rw-r--r--   0        0        0      628 2024-04-02 02:48:33.812042 friendli_client-1.3.4/friendli/cli/api/__init__.py
--rw-r--r--   0        0        0     5374 2024-04-02 02:48:33.812163 friendli_client-1.3.4/friendli/cli/api/chat_completions.py
--rw-r--r--   0        0        0     4513 2024-04-02 02:48:33.812254 friendli_client-1.3.4/friendli/cli/api/completions.py
--rw-r--r--   0        0        0     3058 2024-04-02 02:48:33.812352 friendli_client-1.3.4/friendli/cli/api/text_to_image.py
--rw-r--r--   0        0        0     4424 2024-04-02 02:48:33.812456 friendli_client-1.3.4/friendli/cli/endpoint.py
--rw-r--r--   0        0        0     3572 2024-04-02 02:48:33.812528 friendli_client-1.3.4/friendli/cli/login.py
--rw-r--r--   0        0        0     5150 2024-04-02 02:48:33.812599 friendli_client-1.3.4/friendli/cli/main.py
--rw-r--r--   0        0        0    13525 2024-04-02 03:20:05.465045 friendli_client-1.3.4/friendli/cli/model.py
--rw-r--r--   0        0        0     2727 2024-04-02 02:48:33.812754 friendli_client-1.3.4/friendli/cli/project.py
--rw-r--r--   0        0        0     2074 2024-04-02 02:48:33.812829 friendli_client-1.3.4/friendli/cli/team.py
--rw-r--r--   0        0        0      125 2024-04-02 02:48:33.812930 friendli_client-1.3.4/friendli/client/__init__.py
--rw-r--r--   0        0        0      133 2024-04-02 02:48:33.813027 friendli_client-1.3.4/friendli/client/graphql/__init__.py
--rw-r--r--   0        0        0     4089 2024-04-02 02:48:33.813084 friendli_client-1.3.4/friendli/client/graphql/base.py
--rw-r--r--   0        0        0     6510 2024-04-02 02:48:33.813155 friendli_client-1.3.4/friendli/client/graphql/endpoint.py
--rw-r--r--   0        0        0      791 2024-04-02 02:48:33.813247 friendli_client-1.3.4/friendli/client/graphql/model.py
--rw-r--r--   0        0        0     1014 2024-04-02 02:48:33.813437 friendli_client-1.3.4/friendli/client/graphql/team.py
--rw-r--r--   0        0        0     1914 2024-04-02 02:48:33.813534 friendli_client-1.3.4/friendli/client/graphql/user.py
--rw-r--r--   0        0        0       88 2024-04-02 02:48:33.813643 friendli_client-1.3.4/friendli/client/http/__init__.py
--rw-r--r--   0        0        0    14158 2024-04-02 02:48:33.813750 friendli_client-1.3.4/friendli/client/http/base.py
--rw-r--r--   0        0        0      977 2024-04-02 02:48:33.813870 friendli_client-1.3.4/friendli/client/http/login.py
--rw-r--r--   0        0        0     1567 2024-04-02 02:48:33.813946 friendli_client-1.3.4/friendli/context.py
--rw-r--r--   0        0        0      104 2024-04-02 02:48:33.814074 friendli_client-1.3.4/friendli/di/__init__.py
--rw-r--r--   0        0        0     1507 2024-04-02 02:48:33.814149 friendli_client-1.3.4/friendli/di/injector.py
--rw-r--r--   0        0        0      620 2024-04-02 02:48:33.814218 friendli_client-1.3.4/friendli/di/modules.py
--rw-r--r--   0        0        0     1132 2024-04-02 02:48:33.814282 friendli_client-1.3.4/friendli/enums.py
--rw-r--r--   0        0        0     6853 2024-04-02 02:48:33.814354 friendli_client-1.3.4/friendli/errors.py
--rw-r--r--   0        0        0     9607 2024-04-02 02:48:33.814426 friendli_client-1.3.4/friendli/formatter.py
--rw-r--r--   0        0        0     1728 2024-04-02 02:48:33.814495 friendli_client-1.3.4/friendli/logging.py
--rw-r--r--   0        0        0       92 2024-04-02 02:48:33.814585 friendli_client-1.3.4/friendli/modules/__init__.py
--rw-r--r--   0        0        0      100 2024-04-02 02:48:33.814672 friendli_client-1.3.4/friendli/modules/converter/__init__.py
--rw-r--r--   0        0        0    19733 2024-04-02 02:48:33.814763 friendli_client-1.3.4/friendli/modules/converter/base.py
--rw-r--r--   0        0        0     9671 2024-04-02 03:20:05.465257 friendli_client-1.3.4/friendli/modules/converter/convert.py
--rw-r--r--   0        0        0     5642 2024-04-02 02:48:33.814912 friendli_client-1.3.4/friendli/modules/converter/interface.py
--rw-r--r--   0        0        0     5154 2024-04-02 02:48:33.814984 friendli_client-1.3.4/friendli/modules/converter/maps.py
--rw-r--r--   0        0        0    21332 2024-04-02 02:48:33.815139 friendli_client-1.3.4/friendli/modules/converter/models/blenderbot.py
--rw-r--r--   0        0        0    11658 2024-04-02 02:48:33.815310 friendli_client-1.3.4/friendli/modules/converter/models/bloom.py
--rw-r--r--   0        0        0    10057 2024-04-02 02:48:33.815391 friendli_client-1.3.4/friendli/modules/converter/models/codegen.py
--rw-r--r--   0        0        0    12677 2024-04-02 02:48:33.815479 friendli_client-1.3.4/friendli/modules/converter/models/falcon.py
--rw-r--r--   0        0        0    10036 2024-04-02 02:48:33.815575 friendli_client-1.3.4/friendli/modules/converter/models/gpt2.py
--rw-r--r--   0        0        0    13562 2024-04-02 02:48:33.815649 friendli_client-1.3.4/friendli/modules/converter/models/gpt_neox.py
--rw-r--r--   0        0        0    17772 2024-04-02 02:48:33.815747 friendli_client-1.3.4/friendli/modules/converter/models/gptj.py
--rw-r--r--   0        0        0    21030 2024-04-02 02:48:33.815852 friendli_client-1.3.4/friendli/modules/converter/models/llama.py
--rw-r--r--   0        0        0     4497 2024-04-02 02:48:33.815929 friendli_client-1.3.4/friendli/modules/converter/models/mistral.py
--rw-r--r--   0        0        0     9076 2024-04-02 02:48:33.816002 friendli_client-1.3.4/friendli/modules/converter/models/mixtral.py
--rw-r--r--   0        0        0    16219 2024-04-02 02:48:33.816074 friendli_client-1.3.4/friendli/modules/converter/models/mpt.py
--rw-r--r--   0        0        0    12005 2024-04-02 02:48:33.816146 friendli_client-1.3.4/friendli/modules/converter/models/opt.py
--rw-r--r--   0        0        0    14295 2024-04-02 02:48:33.816216 friendli_client-1.3.4/friendli/modules/converter/models/phi_msft.py
--rw-r--r--   0        0        0    18719 2024-04-02 02:48:33.816290 friendli_client-1.3.4/friendli/modules/converter/models/t5.py
--rw-r--r--   0        0        0     8800 2024-04-02 03:20:05.465458 friendli_client-1.3.4/friendli/modules/converter/saver.py
--rw-r--r--   0        0        0      897 2024-04-02 02:48:33.816450 friendli_client-1.3.4/friendli/modules/converter/schema.py
--rw-r--r--   0        0        0     8858 2024-04-02 03:20:05.465654 friendli_client-1.3.4/friendli/modules/converter/utils.py
--rw-r--r--   0        0        0      100 2024-04-02 02:48:33.816595 friendli_client-1.3.4/friendli/modules/quantizer/__init__.py
--rw-r--r--   0        0        0      104 2024-04-02 02:48:33.816695 friendli_client-1.3.4/friendli/modules/quantizer/awq/__init__.py
--rw-r--r--   0        0        0    19257 2024-04-02 02:48:33.816791 friendli_client-1.3.4/friendli/modules/quantizer/awq/base.py
--rw-r--r--   0        0        0     7090 2024-04-02 02:48:33.816891 friendli_client-1.3.4/friendli/modules/quantizer/awq/models/gpt_neox.py
--rw-r--r--   0        0        0     5917 2024-04-02 02:48:33.816955 friendli_client-1.3.4/friendli/modules/quantizer/awq/models/gptj.py
--rw-r--r--   0        0        0    10738 2024-04-02 02:48:33.817034 friendli_client-1.3.4/friendli/modules/quantizer/awq/models/llama.py
--rw-r--r--   0        0        0     6606 2024-04-02 02:48:33.817101 friendli_client-1.3.4/friendli/modules/quantizer/awq/models/mpt.py
--rw-r--r--   0        0        0     7764 2024-04-02 02:48:33.817162 friendli_client-1.3.4/friendli/modules/quantizer/awq/utils.py
--rw-r--r--   0        0        0    17760 2024-04-02 02:48:33.817232 friendli_client-1.3.4/friendli/modules/quantizer/base.py
--rw-r--r--   0        0        0     3410 2024-04-02 02:48:33.817304 friendli_client-1.3.4/friendli/modules/quantizer/layers.py
--rw-r--r--   0        0        0     4317 2024-04-02 02:48:33.817360 friendli_client-1.3.4/friendli/modules/quantizer/maps.py
--rw-r--r--   0        0        0     3043 2024-04-02 02:48:33.817444 friendli_client-1.3.4/friendli/modules/quantizer/models/llama.py
--rw-r--r--   0        0        0     3212 2024-04-02 02:48:33.817517 friendli_client-1.3.4/friendli/modules/quantizer/models/mixtral.py
--rw-r--r--   0        0        0     2734 2024-04-02 02:48:33.817567 friendli_client-1.3.4/friendli/modules/quantizer/models/mpt.py
--rw-r--r--   0        0        0      107 2024-04-02 02:48:33.817642 friendli_client-1.3.4/friendli/modules/quantizer/schema/__init__.py
--rw-r--r--   0        0        0     2270 2024-04-02 02:48:33.817712 friendli_client-1.3.4/friendli/modules/quantizer/schema/config.py
--rw-r--r--   0        0        0     2798 2024-04-02 02:48:33.817762 friendli_client-1.3.4/friendli/modules/quantizer/schema/data.py
--rw-r--r--   0        0        0      112 2024-04-02 02:48:33.817836 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/__init__.py
--rw-r--r--   0        0        0    24897 2024-04-02 02:48:33.817896 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/base.py
--rw-r--r--   0        0        0     7496 2024-04-02 02:48:33.818011 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/bloom.py
--rw-r--r--   0        0        0     8777 2024-04-02 02:48:33.818086 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/codegen.py
--rw-r--r--   0        0        0    10437 2024-04-02 02:48:33.818138 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/falcon.py
--rw-r--r--   0        0        0     5466 2024-04-02 02:48:33.818193 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/gpt2.py
--rw-r--r--   0        0        0     9062 2024-04-02 02:48:33.818263 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/gpt_neox.py
--rw-r--r--   0        0        0     6961 2024-04-02 02:48:33.818328 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/gptj.py
--rw-r--r--   0        0        0     9431 2024-04-02 02:48:33.818404 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/llama.py
--rw-r--r--   0        0        0     5290 2024-04-02 02:48:33.818545 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/mpt.py
--rw-r--r--   0        0        0     5231 2024-04-02 02:48:33.818597 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/opt.py
--rw-r--r--   0        0        0    16812 2024-04-02 02:48:33.818673 friendli_client-1.3.4/friendli/modules/quantizer/utils.py
--rw-r--r--   0        0        0        0 2024-04-02 02:48:33.818734 friendli_client-1.3.4/friendli/py.typed
--rw-r--r--   0        0        0       92 2024-04-02 02:48:33.818949 friendli_client-1.3.4/friendli/schema/__init__.py
--rw-r--r--   0        0        0       96 2024-04-02 02:48:33.819059 friendli_client-1.3.4/friendli/schema/api/__init__.py
--rw-r--r--   0        0        0       99 2024-04-02 02:48:33.819140 friendli_client-1.3.4/friendli/schema/api/v1/__init__.py
--rw-r--r--   0        0        0      104 2024-04-02 02:48:33.819223 friendli_client-1.3.4/friendli/schema/api/v1/chat/__init__.py
--rw-r--r--   0        0        0     1296 2024-04-02 02:48:33.819279 friendli_client-1.3.4/friendli/schema/api/v1/chat/completions.py
--rw-r--r--   0        0        0      114 2024-04-02 02:48:33.819350 friendli_client-1.3.4/friendli/schema/api/v1/codegen/__init__.py
--rw-r--r--   0        0        0     2208 2024-04-02 02:48:33.819433 friendli_client-1.3.4/friendli/schema/api/v1/codegen/chat_completions_pb2.py
--rw-r--r--   0        0        0     2566 2024-04-02 02:48:33.819560 friendli_client-1.3.4/friendli/schema/api/v1/codegen/chat_completions_pb2.pyi
--rw-r--r--   0        0        0     4490 2024-04-02 02:48:33.819650 friendli_client-1.3.4/friendli/schema/api/v1/codegen/completions_pb2.py
--rw-r--r--   0        0        0     7473 2024-04-02 02:48:33.819710 friendli_client-1.3.4/friendli/schema/api/v1/codegen/completions_pb2.pyi
--rw-r--r--   0        0        0     1738 2024-04-02 02:48:33.819776 friendli_client-1.3.4/friendli/schema/api/v1/codegen/text_to_image_pb2.py
--rw-r--r--   0        0        0     1515 2024-04-02 02:48:33.819906 friendli_client-1.3.4/friendli/schema/api/v1/codegen/text_to_image_pb2.pyi
--rw-r--r--   0        0        0     1027 2024-04-02 02:48:33.819978 friendli_client-1.3.4/friendli/schema/api/v1/completions.py
--rw-r--r--   0        0        0      106 2024-04-02 02:48:33.820119 friendli_client-1.3.4/friendli/schema/api/v1/images/__init__.py
--rw-r--r--   0        0        0      809 2024-04-02 02:48:33.820203 friendli_client-1.3.4/friendli/schema/api/v1/images/image.py
--rw-r--r--   0        0        0      599 2024-04-02 02:48:33.820303 friendli_client-1.3.4/friendli/schema/api/v1/proto/chat_completions.proto
--rw-r--r--   0        0        0     1885 2024-04-02 02:48:33.820359 friendli_client-1.3.4/friendli/schema/api/v1/proto/completions.proto
--rw-r--r--   0        0        0      413 2024-04-02 02:48:33.820415 friendli_client-1.3.4/friendli/schema/api/v1/proto/text_to_image.proto
--rw-r--r--   0        0        0       92 2024-04-02 02:48:33.820516 friendli_client-1.3.4/friendli/schema/config/__init__.py
--rw-r--r--   0        0        0      503 2024-04-02 02:48:33.820569 friendli_client-1.3.4/friendli/schema/config/endpoint.py
--rw-r--r--   0        0        0      101 2024-04-02 02:48:33.820645 friendli_client-1.3.4/friendli/schema/resource/__init__.py
--rw-r--r--   0        0        0      104 2024-04-02 02:48:33.820721 friendli_client-1.3.4/friendli/schema/resource/v1/__init__.py
--rw-r--r--   0        0        0     5476 2024-04-02 02:48:33.820787 friendli_client-1.3.4/friendli/schema/resource/v1/attributes.py
--rw-r--r--   0        0        0      332 2024-04-02 02:48:33.820845 friendli_client-1.3.4/friendli/schema/resource/v1/common.py
--rw-r--r--   0        0        0     1147 2024-04-02 02:48:33.820909 friendli_client-1.3.4/friendli/schema/resource/v1/endpoint.py
--rw-r--r--   0        0        0      243 2024-04-02 02:48:33.820971 friendli_client-1.3.4/friendli/schema/resource/v1/model.py
--rw-r--r--   0        0        0      753 2024-04-02 02:48:33.821026 friendli_client-1.3.4/friendli/schema/resource/v1/transfer.py
--rw-r--r--   0        0        0       88 2024-04-02 02:48:33.821101 friendli_client-1.3.4/friendli/sdk/__init__.py
--rw-r--r--   0        0        0      102 2024-04-02 02:48:33.821171 friendli_client-1.3.4/friendli/sdk/api/__init__.py
--rw-r--r--   0        0        0     8240 2024-04-02 02:48:33.821245 friendli_client-1.3.4/friendli/sdk/api/base.py
--rw-r--r--   0        0        0       93 2024-04-02 02:48:33.821329 friendli_client-1.3.4/friendli/sdk/api/chat/__init__.py
--rw-r--r--   0        0        0     1241 2024-04-02 02:48:33.821390 friendli_client-1.3.4/friendli/sdk/api/chat/chat.py
--rw-r--r--   0        0        0    14282 2024-04-02 02:48:33.821480 friendli_client-1.3.4/friendli/sdk/api/chat/completions.py
--rw-r--r--   0        0        0    51810 2024-04-02 02:48:33.821608 friendli_client-1.3.4/friendli/sdk/api/completions.py
--rw-r--r--   0        0        0       95 2024-04-02 02:48:33.821724 friendli_client-1.3.4/friendli/sdk/api/images/__init__.py
--rw-r--r--   0        0        0     1060 2024-04-02 02:48:33.821774 friendli_client-1.3.4/friendli/sdk/api/images/images.py
--rw-r--r--   0        0        0     5861 2024-04-02 02:48:33.821830 friendli_client-1.3.4/friendli/sdk/api/images/text_to_image.py
--rw-r--r--   0        0        0     3839 2024-04-02 02:48:33.821876 friendli_client-1.3.4/friendli/sdk/client.py
--rw-r--r--   0        0        0      112 2024-04-02 02:48:33.821942 friendli_client-1.3.4/friendli/sdk/resource/__init__.py
--rw-r--r--   0        0        0     2520 2024-04-02 02:48:33.821994 friendli_client-1.3.4/friendli/sdk/resource/base.py
--rw-r--r--   0        0        0     1836 2024-04-02 02:48:33.822044 friendli_client-1.3.4/friendli/sdk/resource/endpoint.py
--rw-r--r--   0        0        0     1033 2024-04-02 02:48:33.822099 friendli_client-1.3.4/friendli/sdk/resource/model.py
--rw-r--r--   0        0        0      706 2024-04-02 02:48:33.822146 friendli_client-1.3.4/friendli/settings.py
--rw-r--r--   0        0        0       97 2024-04-02 02:48:33.822213 friendli_client-1.3.4/friendli/utils/__init__.py
--rw-r--r--   0        0        0     1076 2024-04-02 02:48:33.822265 friendli_client-1.3.4/friendli/utils/compat.py
--rw-r--r--   0        0        0     1294 2024-04-02 02:48:33.822319 friendli_client-1.3.4/friendli/utils/decorator.py
--rw-r--r--   0        0        0     3868 2024-04-02 02:48:33.822376 friendli_client-1.3.4/friendli/utils/format.py
--rw-r--r--   0        0        0     2340 2024-04-02 02:48:33.822424 friendli_client-1.3.4/friendli/utils/fs.py
--rw-r--r--   0        0        0      666 2024-04-02 02:48:33.822474 friendli_client-1.3.4/friendli/utils/prompt.py
--rw-r--r--   0        0        0     1408 2024-04-02 02:48:33.822531 friendli_client-1.3.4/friendli/utils/request.py
--rw-r--r--   0        0        0     1384 2024-04-02 02:48:33.822580 friendli_client-1.3.4/friendli/utils/testing.py
--rw-r--r--   0        0        0    19793 2024-04-02 02:48:33.822653 friendli_client-1.3.4/friendli/utils/transfer.py
--rw-r--r--   0        0        0     3575 2024-04-02 02:48:33.822730 friendli_client-1.3.4/friendli/utils/url.py
--rw-r--r--   0        0        0     3323 2024-04-02 02:48:33.822785 friendli_client-1.3.4/friendli/utils/validate.py
--rw-r--r--   0        0        0     1513 2024-04-02 02:48:33.822833 friendli_client-1.3.4/friendli/utils/version.py
--rw-r--r--   0        0        0     3406 2024-04-02 03:20:05.471738 friendli_client-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     8172 1970-01-01 00:00:00.000000 friendli_client-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-04-02 02:48:33.811614 friendli_client-1.3.5/LICENSE
+-rw-r--r--   0        0        0     6417 2024-04-02 02:48:33.811690 friendli_client-1.3.5/README.md
+-rw-r--r--   0        0        0      615 2024-04-02 02:48:33.811781 friendli_client-1.3.5/friendli/__init__.py
+-rw-r--r--   0        0        0     5840 2024-04-02 02:48:33.811867 friendli_client-1.3.5/friendli/auth.py
+-rw-r--r--   0        0        0      188 2024-04-02 02:48:33.811963 friendli_client-1.3.5/friendli/cli/__init__.py
+-rw-r--r--   0        0        0      628 2024-04-02 02:48:33.812042 friendli_client-1.3.5/friendli/cli/api/__init__.py
+-rw-r--r--   0        0        0     5374 2024-04-02 02:48:33.812163 friendli_client-1.3.5/friendli/cli/api/chat_completions.py
+-rw-r--r--   0        0        0     4513 2024-04-02 02:48:33.812254 friendli_client-1.3.5/friendli/cli/api/completions.py
+-rw-r--r--   0        0        0     3058 2024-04-02 02:48:33.812352 friendli_client-1.3.5/friendli/cli/api/text_to_image.py
+-rw-r--r--   0        0        0     4424 2024-04-02 02:48:33.812456 friendli_client-1.3.5/friendli/cli/endpoint.py
+-rw-r--r--   0        0        0     3572 2024-04-02 02:48:33.812528 friendli_client-1.3.5/friendli/cli/login.py
+-rw-r--r--   0        0        0     5150 2024-04-30 09:30:24.213978 friendli_client-1.3.5/friendli/cli/main.py
+-rw-r--r--   0        0        0    13525 2024-04-08 07:26:04.885159 friendli_client-1.3.5/friendli/cli/model.py
+-rw-r--r--   0        0        0     2727 2024-04-02 02:48:33.812754 friendli_client-1.3.5/friendli/cli/project.py
+-rw-r--r--   0        0        0     2074 2024-04-02 02:48:33.812829 friendli_client-1.3.5/friendli/cli/team.py
+-rw-r--r--   0        0        0      125 2024-04-02 02:48:33.812930 friendli_client-1.3.5/friendli/client/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-02 02:48:33.813027 friendli_client-1.3.5/friendli/client/graphql/__init__.py
+-rw-r--r--   0        0        0     4089 2024-04-02 02:48:33.813084 friendli_client-1.3.5/friendli/client/graphql/base.py
+-rw-r--r--   0        0        0     6510 2024-04-02 02:48:33.813155 friendli_client-1.3.5/friendli/client/graphql/endpoint.py
+-rw-r--r--   0        0        0      791 2024-04-02 02:48:33.813247 friendli_client-1.3.5/friendli/client/graphql/model.py
+-rw-r--r--   0        0        0     1014 2024-04-02 02:48:33.813437 friendli_client-1.3.5/friendli/client/graphql/team.py
+-rw-r--r--   0        0        0     1914 2024-04-02 02:48:33.813534 friendli_client-1.3.5/friendli/client/graphql/user.py
+-rw-r--r--   0        0        0       88 2024-04-02 02:48:33.813643 friendli_client-1.3.5/friendli/client/http/__init__.py
+-rw-r--r--   0        0        0    14158 2024-04-02 02:48:33.813750 friendli_client-1.3.5/friendli/client/http/base.py
+-rw-r--r--   0        0        0      977 2024-04-02 02:48:33.813870 friendli_client-1.3.5/friendli/client/http/login.py
+-rw-r--r--   0        0        0     1567 2024-04-02 02:48:33.813946 friendli_client-1.3.5/friendli/context.py
+-rw-r--r--   0        0        0      104 2024-04-02 02:48:33.814074 friendli_client-1.3.5/friendli/di/__init__.py
+-rw-r--r--   0        0        0     1507 2024-04-02 02:48:33.814149 friendli_client-1.3.5/friendli/di/injector.py
+-rw-r--r--   0        0        0      620 2024-04-02 02:48:33.814218 friendli_client-1.3.5/friendli/di/modules.py
+-rw-r--r--   0        0        0     1132 2024-04-02 02:48:33.814282 friendli_client-1.3.5/friendli/enums.py
+-rw-r--r--   0        0        0     6853 2024-04-02 02:48:33.814354 friendli_client-1.3.5/friendli/errors.py
+-rw-r--r--   0        0        0     9607 2024-04-02 02:48:33.814426 friendli_client-1.3.5/friendli/formatter.py
+-rw-r--r--   0        0        0     1728 2024-04-02 02:48:33.814495 friendli_client-1.3.5/friendli/logging.py
+-rw-r--r--   0        0        0       92 2024-04-02 02:48:33.814585 friendli_client-1.3.5/friendli/modules/__init__.py
+-rw-r--r--   0        0        0      100 2024-04-02 02:48:33.814672 friendli_client-1.3.5/friendli/modules/converter/__init__.py
+-rw-r--r--   0        0        0    20474 2024-04-17 07:52:41.833234 friendli_client-1.3.5/friendli/modules/converter/base.py
+-rw-r--r--   0        0        0     9671 2024-04-30 09:30:24.214259 friendli_client-1.3.5/friendli/modules/converter/convert.py
+-rw-r--r--   0        0        0     5642 2024-04-02 02:48:33.814912 friendli_client-1.3.5/friendli/modules/converter/interface.py
+-rw-r--r--   0        0        0     5496 2024-05-25 04:02:47.656046 friendli_client-1.3.5/friendli/modules/converter/maps.py
+-rw-r--r--   0        0        0    21332 2024-04-02 02:48:33.815139 friendli_client-1.3.5/friendli/modules/converter/models/blenderbot.py
+-rw-r--r--   0        0        0    11658 2024-04-02 02:48:33.815310 friendli_client-1.3.5/friendli/modules/converter/models/bloom.py
+-rw-r--r--   0        0        0    10057 2024-04-02 02:48:33.815391 friendli_client-1.3.5/friendli/modules/converter/models/codegen.py
+-rw-r--r--   0        0        0     3237 2024-04-17 07:52:41.834113 friendli_client-1.3.5/friendli/modules/converter/models/cohere.py
+-rw-r--r--   0        0        0     3521 2024-05-25 04:02:47.656272 friendli_client-1.3.5/friendli/modules/converter/models/dbrx.py
+-rw-r--r--   0        0        0    12677 2024-04-02 02:48:33.815479 friendli_client-1.3.5/friendli/modules/converter/models/falcon.py
+-rw-r--r--   0        0        0    10036 2024-04-02 02:48:33.815575 friendli_client-1.3.5/friendli/modules/converter/models/gpt2.py
+-rw-r--r--   0        0        0    13562 2024-04-02 02:48:33.815649 friendli_client-1.3.5/friendli/modules/converter/models/gpt_neox.py
+-rw-r--r--   0        0        0    17772 2024-04-02 02:48:33.815747 friendli_client-1.3.5/friendli/modules/converter/models/gptj.py
+-rw-r--r--   0        0        0    21029 2024-04-17 07:52:41.834407 friendli_client-1.3.5/friendli/modules/converter/models/llama.py
+-rw-r--r--   0        0        0     4497 2024-04-02 02:48:33.815929 friendli_client-1.3.5/friendli/modules/converter/models/mistral.py
+-rw-r--r--   0        0        0     9076 2024-04-02 02:48:33.816002 friendli_client-1.3.5/friendli/modules/converter/models/mixtral.py
+-rw-r--r--   0        0        0    16219 2024-04-02 02:48:33.816074 friendli_client-1.3.5/friendli/modules/converter/models/mpt.py
+-rw-r--r--   0        0        0    12005 2024-04-02 02:48:33.816146 friendli_client-1.3.5/friendli/modules/converter/models/opt.py
+-rw-r--r--   0        0        0    14295 2024-04-02 02:48:33.816216 friendli_client-1.3.5/friendli/modules/converter/models/phi_msft.py
+-rw-r--r--   0        0        0    18719 2024-04-02 02:48:33.816290 friendli_client-1.3.5/friendli/modules/converter/models/t5.py
+-rw-r--r--   0        0        0     8800 2024-04-02 03:20:05.465458 friendli_client-1.3.5/friendli/modules/converter/saver.py
+-rw-r--r--   0        0        0      897 2024-04-02 02:48:33.816450 friendli_client-1.3.5/friendli/modules/converter/schema.py
+-rw-r--r--   0        0        0     8858 2024-04-02 03:20:05.465654 friendli_client-1.3.5/friendli/modules/converter/utils.py
+-rw-r--r--   0        0        0      100 2024-04-02 02:48:33.816595 friendli_client-1.3.5/friendli/modules/quantizer/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-02 02:48:33.816695 friendli_client-1.3.5/friendli/modules/quantizer/awq/__init__.py
+-rw-r--r--   0        0        0    19257 2024-04-02 02:48:33.816791 friendli_client-1.3.5/friendli/modules/quantizer/awq/base.py
+-rw-r--r--   0        0        0     7090 2024-04-02 02:48:33.816891 friendli_client-1.3.5/friendli/modules/quantizer/awq/models/gpt_neox.py
+-rw-r--r--   0        0        0     5917 2024-04-02 02:48:33.816955 friendli_client-1.3.5/friendli/modules/quantizer/awq/models/gptj.py
+-rw-r--r--   0        0        0    10738 2024-04-02 02:48:33.817034 friendli_client-1.3.5/friendli/modules/quantizer/awq/models/llama.py
+-rw-r--r--   0        0        0     6606 2024-04-02 02:48:33.817101 friendli_client-1.3.5/friendli/modules/quantizer/awq/models/mpt.py
+-rw-r--r--   0        0        0     7764 2024-04-02 02:48:33.817162 friendli_client-1.3.5/friendli/modules/quantizer/awq/utils.py
+-rw-r--r--   0        0        0    18976 2024-05-25 04:02:47.664564 friendli_client-1.3.5/friendli/modules/quantizer/base.py
+-rw-r--r--   0        0        0     3204 2024-05-25 04:02:47.656854 friendli_client-1.3.5/friendli/modules/quantizer/layers.py
+-rw-r--r--   0        0        0     4440 2024-05-25 04:02:47.657091 friendli_client-1.3.5/friendli/modules/quantizer/maps.py
+-rw-r--r--   0        0        0     9730 2024-05-25 04:02:47.657305 friendli_client-1.3.5/friendli/modules/quantizer/models/dbrx.py
+-rw-r--r--   0        0        0     3040 2024-04-17 07:52:41.835946 friendli_client-1.3.5/friendli/modules/quantizer/models/llama.py
+-rw-r--r--   0        0        0     3514 2024-05-25 04:02:47.657785 friendli_client-1.3.5/friendli/modules/quantizer/models/mixtral.py
+-rw-r--r--   0        0        0     2697 2024-05-25 04:02:47.658012 friendli_client-1.3.5/friendli/modules/quantizer/models/mpt.py
+-rw-r--r--   0        0        0      107 2024-04-02 02:48:33.817642 friendli_client-1.3.5/friendli/modules/quantizer/schema/__init__.py
+-rw-r--r--   0        0        0     2285 2024-05-25 04:02:47.658245 friendli_client-1.3.5/friendli/modules/quantizer/schema/config.py
+-rw-r--r--   0        0        0     2798 2024-04-02 02:48:33.817762 friendli_client-1.3.5/friendli/modules/quantizer/schema/data.py
+-rw-r--r--   0        0        0      112 2024-04-02 02:48:33.817836 friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/__init__.py
+-rw-r--r--   0        0        0    24897 2024-04-02 02:48:33.817896 friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/base.py
+-rw-r--r--   0        0        0     7496 2024-04-02 02:48:33.818011 friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/bloom.py
+-rw-r--r--   0        0        0     8777 2024-04-02 02:48:33.818086 friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/codegen.py
+-rw-r--r--   0        0        0    10437 2024-04-02 02:48:33.818138 friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/falcon.py
+-rw-r--r--   0        0        0     5466 2024-04-02 02:48:33.818193 friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/gpt2.py
+-rw-r--r--   0        0        0     9062 2024-04-02 02:48:33.818263 friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/gpt_neox.py
+-rw-r--r--   0        0        0     6961 2024-04-02 02:48:33.818328 friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/gptj.py
+-rw-r--r--   0        0        0     9431 2024-04-02 02:48:33.818404 friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/llama.py
+-rw-r--r--   0        0        0     5290 2024-04-02 02:48:33.818545 friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/mpt.py
+-rw-r--r--   0        0        0     5231 2024-04-02 02:48:33.818597 friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/opt.py
+-rw-r--r--   0        0        0    16812 2024-04-02 02:48:33.818673 friendli_client-1.3.5/friendli/modules/quantizer/utils.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:48:33.818734 friendli_client-1.3.5/friendli/py.typed
+-rw-r--r--   0        0        0       92 2024-04-02 02:48:33.818949 friendli_client-1.3.5/friendli/schema/__init__.py
+-rw-r--r--   0        0        0       96 2024-04-02 02:48:33.819059 friendli_client-1.3.5/friendli/schema/api/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-02 02:48:33.819140 friendli_client-1.3.5/friendli/schema/api/v1/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-02 02:48:33.819223 friendli_client-1.3.5/friendli/schema/api/v1/chat/__init__.py
+-rw-r--r--   0        0        0     1296 2024-04-02 02:48:33.819279 friendli_client-1.3.5/friendli/schema/api/v1/chat/completions.py
+-rw-r--r--   0        0        0      114 2024-04-02 02:48:33.819350 friendli_client-1.3.5/friendli/schema/api/v1/codegen/__init__.py
+-rw-r--r--   0        0        0     2208 2024-04-02 02:48:33.819433 friendli_client-1.3.5/friendli/schema/api/v1/codegen/chat_completions_pb2.py
+-rw-r--r--   0        0        0     2566 2024-04-02 02:48:33.819560 friendli_client-1.3.5/friendli/schema/api/v1/codegen/chat_completions_pb2.pyi
+-rw-r--r--   0        0        0     4490 2024-04-02 02:48:33.819650 friendli_client-1.3.5/friendli/schema/api/v1/codegen/completions_pb2.py
+-rw-r--r--   0        0        0     7473 2024-04-02 02:48:33.819710 friendli_client-1.3.5/friendli/schema/api/v1/codegen/completions_pb2.pyi
+-rw-r--r--   0        0        0     1738 2024-04-02 02:48:33.819776 friendli_client-1.3.5/friendli/schema/api/v1/codegen/text_to_image_pb2.py
+-rw-r--r--   0        0        0     1515 2024-04-02 02:48:33.819906 friendli_client-1.3.5/friendli/schema/api/v1/codegen/text_to_image_pb2.pyi
+-rw-r--r--   0        0        0     1027 2024-04-02 02:48:33.819978 friendli_client-1.3.5/friendli/schema/api/v1/completions.py
+-rw-r--r--   0        0        0      106 2024-04-02 02:48:33.820119 friendli_client-1.3.5/friendli/schema/api/v1/images/__init__.py
+-rw-r--r--   0        0        0      809 2024-04-02 02:48:33.820203 friendli_client-1.3.5/friendli/schema/api/v1/images/image.py
+-rw-r--r--   0        0        0      599 2024-04-02 02:48:33.820303 friendli_client-1.3.5/friendli/schema/api/v1/proto/chat_completions.proto
+-rw-r--r--   0        0        0     1885 2024-04-02 02:48:33.820359 friendli_client-1.3.5/friendli/schema/api/v1/proto/completions.proto
+-rw-r--r--   0        0        0      413 2024-04-02 02:48:33.820415 friendli_client-1.3.5/friendli/schema/api/v1/proto/text_to_image.proto
+-rw-r--r--   0        0        0       92 2024-04-02 02:48:33.820516 friendli_client-1.3.5/friendli/schema/config/__init__.py
+-rw-r--r--   0        0        0      503 2024-04-02 02:48:33.820569 friendli_client-1.3.5/friendli/schema/config/endpoint.py
+-rw-r--r--   0        0        0      101 2024-04-02 02:48:33.820645 friendli_client-1.3.5/friendli/schema/resource/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-02 02:48:33.820721 friendli_client-1.3.5/friendli/schema/resource/v1/__init__.py
+-rw-r--r--   0        0        0     5476 2024-04-02 02:48:33.820787 friendli_client-1.3.5/friendli/schema/resource/v1/attributes.py
+-rw-r--r--   0        0        0      332 2024-04-02 02:48:33.820845 friendli_client-1.3.5/friendli/schema/resource/v1/common.py
+-rw-r--r--   0        0        0     1147 2024-04-02 02:48:33.820909 friendli_client-1.3.5/friendli/schema/resource/v1/endpoint.py
+-rw-r--r--   0        0        0      243 2024-04-02 02:48:33.820971 friendli_client-1.3.5/friendli/schema/resource/v1/model.py
+-rw-r--r--   0        0        0      753 2024-04-02 02:48:33.821026 friendli_client-1.3.5/friendli/schema/resource/v1/transfer.py
+-rw-r--r--   0        0        0       88 2024-04-02 02:48:33.821101 friendli_client-1.3.5/friendli/sdk/__init__.py
+-rw-r--r--   0        0        0      102 2024-04-02 02:48:33.821171 friendli_client-1.3.5/friendli/sdk/api/__init__.py
+-rw-r--r--   0        0        0     8240 2024-04-02 02:48:33.821245 friendli_client-1.3.5/friendli/sdk/api/base.py
+-rw-r--r--   0        0        0       93 2024-04-02 02:48:33.821329 friendli_client-1.3.5/friendli/sdk/api/chat/__init__.py
+-rw-r--r--   0        0        0     1241 2024-04-02 02:48:33.821390 friendli_client-1.3.5/friendli/sdk/api/chat/chat.py
+-rw-r--r--   0        0        0    14282 2024-04-30 09:43:26.458999 friendli_client-1.3.5/friendli/sdk/api/chat/completions.py
+-rw-r--r--   0        0        0    51810 2024-04-02 02:48:33.821608 friendli_client-1.3.5/friendli/sdk/api/completions.py
+-rw-r--r--   0        0        0       95 2024-04-02 02:48:33.821724 friendli_client-1.3.5/friendli/sdk/api/images/__init__.py
+-rw-r--r--   0        0        0     1060 2024-04-02 02:48:33.821774 friendli_client-1.3.5/friendli/sdk/api/images/images.py
+-rw-r--r--   0        0        0     5861 2024-04-02 02:48:33.821830 friendli_client-1.3.5/friendli/sdk/api/images/text_to_image.py
+-rw-r--r--   0        0        0     3839 2024-04-30 09:30:24.214718 friendli_client-1.3.5/friendli/sdk/client.py
+-rw-r--r--   0        0        0      112 2024-04-02 02:48:33.821942 friendli_client-1.3.5/friendli/sdk/resource/__init__.py
+-rw-r--r--   0        0        0     2520 2024-04-02 02:48:33.821994 friendli_client-1.3.5/friendli/sdk/resource/base.py
+-rw-r--r--   0        0        0     1836 2024-04-02 02:48:33.822044 friendli_client-1.3.5/friendli/sdk/resource/endpoint.py
+-rw-r--r--   0        0        0     1033 2024-04-02 02:48:33.822099 friendli_client-1.3.5/friendli/sdk/resource/model.py
+-rw-r--r--   0        0        0      706 2024-04-02 02:48:33.822146 friendli_client-1.3.5/friendli/settings.py
+-rw-r--r--   0        0        0       97 2024-04-02 02:48:33.822213 friendli_client-1.3.5/friendli/utils/__init__.py
+-rw-r--r--   0        0        0     1076 2024-04-02 02:48:33.822265 friendli_client-1.3.5/friendli/utils/compat.py
+-rw-r--r--   0        0        0     1294 2024-04-02 02:48:33.822319 friendli_client-1.3.5/friendli/utils/decorator.py
+-rw-r--r--   0        0        0     3868 2024-04-08 07:21:54.077241 friendli_client-1.3.5/friendli/utils/format.py
+-rw-r--r--   0        0        0     2340 2024-04-02 02:48:33.822424 friendli_client-1.3.5/friendli/utils/fs.py
+-rw-r--r--   0        0        0      666 2024-04-02 02:48:33.822474 friendli_client-1.3.5/friendli/utils/prompt.py
+-rw-r--r--   0        0        0     1408 2024-04-02 02:48:33.822531 friendli_client-1.3.5/friendli/utils/request.py
+-rw-r--r--   0        0        0     1384 2024-04-02 02:48:33.822580 friendli_client-1.3.5/friendli/utils/testing.py
+-rw-r--r--   0        0        0    19793 2024-04-02 02:48:33.822653 friendli_client-1.3.5/friendli/utils/transfer.py
+-rw-r--r--   0        0        0     3575 2024-04-02 02:48:33.822730 friendli_client-1.3.5/friendli/utils/url.py
+-rw-r--r--   0        0        0     3323 2024-04-02 02:48:33.822785 friendli_client-1.3.5/friendli/utils/validate.py
+-rw-r--r--   0        0        0     1513 2024-04-02 02:48:33.822833 friendli_client-1.3.5/friendli/utils/version.py
+-rw-r--r--   0        0        0     3406 2024-05-28 02:47:23.499127 friendli_client-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     8172 1970-01-01 00:00:00.000000 friendli_client-1.3.5/PKG-INFO
```

### Comparing `friendli_client-1.3.4/LICENSE` & `friendli_client-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/README.md` & `friendli_client-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/__init__.py` & `friendli_client-1.3.5/friendli/__init__.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/auth.py` & `friendli_client-1.3.5/friendli/auth.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/cli/api/__init__.py` & `friendli_client-1.3.5/friendli/cli/api/__init__.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/cli/api/chat_completions.py` & `friendli_client-1.3.5/friendli/cli/api/chat_completions.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/cli/api/completions.py` & `friendli_client-1.3.5/friendli/cli/api/completions.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/cli/api/text_to_image.py` & `friendli_client-1.3.5/friendli/cli/api/text_to_image.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/cli/endpoint.py` & `friendli_client-1.3.5/friendli/cli/endpoint.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/cli/login.py` & `friendli_client-1.3.5/friendli/cli/login.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/cli/main.py` & `friendli_client-1.3.5/friendli/cli/main.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/cli/model.py` & `friendli_client-1.3.5/friendli/cli/model.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/cli/project.py` & `friendli_client-1.3.5/friendli/cli/project.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/cli/team.py` & `friendli_client-1.3.5/friendli/cli/team.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/client/graphql/base.py` & `friendli_client-1.3.5/friendli/client/graphql/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/client/graphql/endpoint.py` & `friendli_client-1.3.5/friendli/client/graphql/endpoint.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/client/graphql/model.py` & `friendli_client-1.3.5/friendli/client/graphql/model.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/client/graphql/team.py` & `friendli_client-1.3.5/friendli/client/graphql/team.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/client/graphql/user.py` & `friendli_client-1.3.5/friendli/client/graphql/user.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/client/http/base.py` & `friendli_client-1.3.5/friendli/client/http/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/client/http/login.py` & `friendli_client-1.3.5/friendli/client/http/login.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/context.py` & `friendli_client-1.3.5/friendli/context.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/di/injector.py` & `friendli_client-1.3.5/friendli/di/injector.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/di/modules.py` & `friendli_client-1.3.5/friendli/di/modules.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/enums.py` & `friendli_client-1.3.5/friendli/enums.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/errors.py` & `friendli_client-1.3.5/friendli/errors.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/formatter.py` & `friendli_client-1.3.5/friendli/formatter.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/logging.py` & `friendli_client-1.3.5/friendli/logging.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/base.py` & `friendli_client-1.3.5/friendli/modules/converter/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,7 +531,29 @@
         self,
     ) -> List[ConvertInfo]:
         """Return the list of conversion informations for LoRA modules of the model."""
 
 
 OneOfAdapterConverter = DecoderOnlyLoraConverter
 OneOfConverter = Union[EncoderDecoderConverter, DecoderOnlyConverter]
+
+
+class FP8OnlyConverter(DecoderOnlyConverter):
+    """FP8Only Architectures Converter Class."""
+
+    def get_attributes(self) -> Dict[str, Any]:
+        """Get checkpoint attributes."""
+        raise NotImplementedError("Not supported in FP8 Conversion.")
+
+    @property
+    def decoder_convert_info_list(
+        self,
+    ) -> List[ConvertInfo]:
+        """The list of conversion informations for transformer blocks."""
+        raise NotImplementedError("Not supported in FP8 Conversion.")
+
+    @property
+    def non_transformer_convert_info_list(
+        self,
+    ) -> List[ConvertInfo]:
+        """The list of conversion informations for non-transformer blocks."""
+        raise NotImplementedError("Not supported in FP8 Conversion.")
```

### Comparing `friendli_client-1.3.4/friendli/modules/converter/convert.py` & `friendli_client-1.3.5/friendli/modules/converter/convert.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/interface.py` & `friendli_client-1.3.5/friendli/modules/converter/interface.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/maps.py` & `friendli_client-1.3.5/friendli/modules/converter/maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from typing import Dict, Tuple, Type, Union
 
 from transformers import (  # type: ignore[import]
     AutoModelForCausalLM,
     BlenderbotForConditionalGeneration,
     BloomForCausalLM,
     CodeGenForCausalLM,
+    CohereForCausalLM,
+    DbrxForCausalLM,
     FalconForCausalLM,
     GPT2LMHeadModel,
     GPTJForCausalLM,
     GPTNeoXForCausalLM,
     LlamaForCausalLM,
     MistralForCausalLM,
     MixtralForCausalLM,
@@ -25,14 +27,16 @@
 )
 
 from friendli.errors import NotSupportedCheckpointError
 from friendli.modules.converter.base import OneOfAdapterConverter, OneOfConverter
 from friendli.modules.converter.models.blenderbot import BlenderbotConverter
 from friendli.modules.converter.models.bloom import BloomForCausalLMConverter
 from friendli.modules.converter.models.codegen import CodegenForCausalLMConverter
+from friendli.modules.converter.models.cohere import CohereForCausalLMConverter
+from friendli.modules.converter.models.dbrx import DbrxForCausalLMConverter
 from friendli.modules.converter.models.falcon import FalconForCausalLMConverter
 from friendli.modules.converter.models.gpt2 import GPT2LMHeadModelConverter
 from friendli.modules.converter.models.gpt_neox import GPTNeoXForCausalLMConverter
 from friendli.modules.converter.models.gptj import (
     GPTJForCausalLMConverter,
     GPTJForCausalLMLoraConverter,
 )
@@ -70,14 +74,16 @@
     "LLaMAForCausalLM": (LlamaForCausalLM, LlamaForCausalLMConverter),
     "MistralForCausalLM": (MistralForCausalLM, MistralForCausalLMConverter),
     "MixtralForCausalLM": (MixtralForCausalLM, MixtralForCausalLMConverter),
     "MPTForCausalLM": (MptForCausalLM, MPTForCausalLMConverter),
     "OPTForCausalLM": (OPTForCausalLM, OPTForCausalLMConverter),
     "T5ForConditionalGeneration": (T5ForConditionalGeneration, T5Converter),
     "PhiForCausalLM": (AutoModelForCausalLM, PhiForCausalLMConverter),
+    "CohereForCausalLM": (CohereForCausalLM, CohereForCausalLMConverter),
+    "DbrxForCausalLM": (DbrxForCausalLM, DbrxForCausalLMConverter),
 }
 
 MODEL_ARCH_ADAPTER_CONVERTER_MAP: Dict[
     str,
     Type[OneOfAdapterConverter],
 ] = {
     "GPTJForCausalLM": GPTJForCausalLMLoraConverter,
```

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/blenderbot.py` & `friendli_client-1.3.5/friendli/modules/converter/models/blenderbot.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/bloom.py` & `friendli_client-1.3.5/friendli/modules/converter/models/bloom.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/codegen.py` & `friendli_client-1.3.5/friendli/modules/converter/models/codegen.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/falcon.py` & `friendli_client-1.3.5/friendli/modules/converter/models/falcon.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/gpt2.py` & `friendli_client-1.3.5/friendli/modules/converter/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/gpt_neox.py` & `friendli_client-1.3.5/friendli/modules/converter/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/gptj.py` & `friendli_client-1.3.5/friendli/modules/converter/models/gptj.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/llama.py` & `friendli_client-1.3.5/friendli/modules/converter/models/llama.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) 2022-present, FriendliAI Inc. All rights reserved.
 
-"""Friendli LLaMAa Checkpoint Converter."""
+"""Friendli LLaMA Checkpoint Converter."""
 
 
 from __future__ import annotations
 
 from typing import Any, Dict, Iterable, List, Set, cast
 
 import torch
```

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/mistral.py` & `friendli_client-1.3.5/friendli/modules/converter/models/mistral.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/mixtral.py` & `friendli_client-1.3.5/friendli/modules/converter/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/mpt.py` & `friendli_client-1.3.5/friendli/modules/converter/models/mpt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/opt.py` & `friendli_client-1.3.5/friendli/modules/converter/models/opt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/phi_msft.py` & `friendli_client-1.3.5/friendli/modules/converter/models/phi_msft.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/models/t5.py` & `friendli_client-1.3.5/friendli/modules/converter/models/t5.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/saver.py` & `friendli_client-1.3.5/friendli/modules/converter/saver.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/schema.py` & `friendli_client-1.3.5/friendli/modules/converter/schema.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/converter/utils.py` & `friendli_client-1.3.5/friendli/modules/converter/utils.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/awq/base.py` & `friendli_client-1.3.5/friendli/modules/quantizer/awq/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/awq/models/gpt_neox.py` & `friendli_client-1.3.5/friendli/modules/quantizer/awq/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/awq/models/gptj.py` & `friendli_client-1.3.5/friendli/modules/quantizer/awq/models/gptj.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/awq/models/llama.py` & `friendli_client-1.3.5/friendli/modules/quantizer/awq/models/llama.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/awq/models/mpt.py` & `friendli_client-1.3.5/friendli/modules/quantizer/awq/models/mpt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/awq/utils.py` & `friendli_client-1.3.5/friendli/modules/quantizer/awq/utils.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/base.py` & `friendli_client-1.3.5/friendli/modules/quantizer/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -244,20 +244,49 @@
         model = self.quantize(model)
         yield from self.converter.convert(model, convert_info_list)
 
 
 class FP8QuantHook(AbstractQuantHook):
     """Quantization Hook for FP8Quantizer."""
 
+    def pre_quantize(self, model: Module) -> torch.nn.Module:  # type: ignore[]
+        """Pre-procedure that should be called before quantize() is called in FP8Quantizer."""
+        return model
+
+    def post_quantize(self, model: Module) -> torch.nn.Module:
+        """Post-procedure that should be called after quantize() is called in FP8Quantizer."""
+        return model
+
     def get_quant_result(
         self, quant_inputs: TFQuantInputs, **kwargs: Any
     ) -> TFQuantResults:
         """Returns the quantization result of the layer."""
         raise NotImplementedError
 
+    def get_quantized_param_names(self, model: torch.nn.Module) -> List[str]:
+        """Return the parameter names of quantized layers."""
+        quantized_param_names = []
+        for tf_quant_input in self.iter_tf_quant_inputs(model):
+            assert isinstance(tf_quant_input, HFTFQuantInputs)
+            for quant_input in tf_quant_input.quant_inputs:
+                for target_name in quant_input.target_names:
+                    quantized_param_names.append(f"{target_name}.weight")
+        return quantized_param_names
+
+    def get_quantized_param_scale_names(self, model):
+        """Return the parameter scale names of quantized layers."""
+        quantized_param_scale_names = []
+        for tf_quant_input in self.iter_tf_quant_inputs(model):
+            assert isinstance(tf_quant_input, HFTFQuantInputs)
+            for quant_input in tf_quant_input.quant_inputs:
+                for target_name in quant_input.target_names:
+                    quantized_param_scale_names.append(f"{target_name}.weight_scale")
+                    quantized_param_scale_names.append(f"{target_name}.in_scale")
+        return quantized_param_scale_names
+
     @property
     def quantized_convert_info_list(
         self,
     ) -> List[ConvertInfo]:
         """Return the list of conversion informations for quantized layers."""
         raise NotImplementedError
 
@@ -266,15 +295,15 @@
         self,
     ) -> List[ConvertInfo]:
         """Return the list of conversion informations for modified layers."""
         raise NotImplementedError
 
 
 class FP8Quantizer(CommonQuantizer):
-    """Common Quantizer for huggingface format.
+    """FP8Quantizer for huggingface format.
 
     This quantizer supports per-tensor weight-activation quantization by
     using calibration dataset. It adds quantization scale, and quantized
     parameter to the checkpoint, while preserves parameter shape, and name
     in huggingface checkpoint.
     """
 
@@ -324,15 +353,21 @@
         target_weights = [model.get_submodule(name).weight for name in names]
         target_weight = torch.concat(target_weights)
 
         act_scale = float(input_max.detach().abs().max().item()) / float(max_val)
         weight_scale = float(target_weight.detach().abs().max().item()) / float(max_val)
 
         q_weights = [
-            ((weight.detach().float() / weight_scale).clip(min_val, max_val).to("cpu"))
+            (
+                (weight.detach().float() / weight_scale)
+                .clip(min_val, max_val)
+                .to(torch.float8_e4m3fn)
+                .view(torch.int8)
+                .to("cpu")
+            )
             for weight in target_weights
         ]
         return [
             WeightActQuantResult(
                 name,
                 quant_dtype=self.quant_config.quant_dtype,
                 act_scale=torch.tensor(act_scale, dtype=torch.float32),
@@ -359,25 +394,30 @@
                 self.quant_config.device,
                 dataset,
                 cast(FP8QuantHook, self.hook).get_linear_layer_types(),
                 percentile=self.quant_config.percentile,
                 tqdm_desc="Collecting stats for Static Quantization.",
                 batch_size=32,
             )
-            for tf_quant_input in self.hook.iter_tf_quant_inputs(model):
+            for tf_quant_input in tqdm(
+                self.hook.iter_tf_quant_inputs(model),
+                total=len(self.hook.get_tf_blocks(model)),
+                desc="Qunatize",
+                unit="layer",
+            ):
                 assert isinstance(tf_quant_input, HFTFQuantInputs)
                 for quant_input in tf_quant_input.quant_inputs:
                     parent_module, local_names, names = (
                         quant_input.parent_module,
                         quant_input.local_names,
                         quant_input.target_names,
                     )
+
                     if isinstance(parent_module, torch.nn.ModuleList):
-                        # for MoE model
-                        # all module share same weight scale & act scale
+                        # For MoE models with seperate expert layers
                         parent_modules_w_local_name = []
                         for p_module in parent_module:
                             for local_name in local_names:
                                 parent_modules_w_local_name.append(
                                     (p_module, local_name)
                                 )
 
@@ -434,35 +474,25 @@
             model (torch.nn.Module): Huggingface model.
             state_dict (Dict[str, torch.Tensor]):
                 Dictionary of mapping of tensor name to tensor
             convert_info_list (List[ConvertInfo]):
                 Dictionary of mapping converted params name to conversion functions.
                 It will be depreciated.
         """
-        quantized_param_names = []
-        quantized_param_scale_names = []
-        for tf_quant_input in self.hook.iter_tf_quant_inputs(model):
-            assert isinstance(tf_quant_input, HFTFQuantInputs)
-            for quant_input in tf_quant_input.quant_inputs:
-                for target_name in quant_input.target_names:
-                    quantized_param_names.append(f"{target_name}.weight")
-                    quantized_param_scale_names.append(f"{target_name}.weight_scale")
-                    quantized_param_scale_names.append(f"{target_name}.in_scale")
-
-        self.pre_quantize(model)
+        model = cast(FP8QuantHook, self.hook).pre_quantize(model)
         model = self.quantize(model)
+        model = cast(FP8QuantHook, self.hook).post_quantize(model)
         state_dict: Dict[str, torch.Tensor] = model.state_dict()
 
+        quantized_param_names = cast(FP8QuantHook, self.hook).get_quantized_param_names(
+            model
+        )
+        quantized_param_names.extend(
+            cast(FP8QuantHook, self.hook).get_quantized_param_scale_names(model)
+        )
+
         with tqdm(total=len(state_dict), desc="Converting", unit="tensor") as pbar:
             for param_name, param in state_dict.items():
-                param = param.to("cpu").detach()
-                if param_name in quantized_param_names:
-                    converted_param = param.to(torch.float8_e4m3fn).view(torch.int8)
-                elif param_name in quantized_param_scale_names:
-                    converted_param = param.to(torch.float32)
-                else:
-                    converted_param = param.to(
-                        get_torch_data_type(self.converter.data_type)
-                    )
-
-                yield param_name, converted_param
+                if param_name not in quantized_param_names:
+                    param = param.to(get_torch_data_type(self.converter.data_type))
+                yield param_name, param
                 pbar.update()
```

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/layers.py` & `friendli_client-1.3.5/friendli/modules/quantizer/layers.py`

 * *Files 17% similar despite different names*

```diff
@@ -57,41 +57,35 @@
 
 
 class WeightActQuantizedLinearLayer(torch.nn.Module):
     """Linear Layer with weight-act quantization."""
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        in_features: int,
-        out_features: int,
         q_weight: torch.Tensor,
         weight_scale: torch.Tensor,
         act_scale: torch.Tensor,
         bias: Optional[torch.nn.Parameter] = None,
     ):
         """Initialize the Weight Only Quantized Linear Layer."""
         super().__init__()
-        self.in_features = in_features
-        self.out_features = out_features
         self.in_scale = torch.nn.Parameter(act_scale)
         self.weight_scale = torch.nn.Parameter(weight_scale)
         self.weight = torch.nn.Parameter(q_weight, requires_grad=False)
         self.register_parameter("bias", bias)
 
     @staticmethod
     def from_layer(
         layer: torch.nn.Module, quant_result: CommonQuantResult
     ) -> torch.nn.Module:
         """Returns the quantized layer from the original layer."""
         q_result = cast(WeightActQuantResult, quant_result)
         return WeightActQuantizedLinearLayer(
-            cast(torch.nn.Linear, layer).in_features,
-            cast(torch.nn.Linear, layer).out_features,
             q_result.q_weight,
             q_result.weight_scale,
             q_result.act_scale,
-            cast(torch.nn.Linear, layer).bias,
+            cast(torch.nn.Linear, layer).bias if hasattr(layer, "bias") else None,
         )
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """Forward pass with fake quantization. Not used in conversion."""
         raise NotImplementedError("Not used in conversion.")
```

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/maps.py` & `friendli_client-1.3.5/friendli/modules/quantizer/maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from friendli.modules.converter.utils import get_model_arch
 from friendli.modules.quantizer.awq.base import AWQHook, AWQQuantizer
 from friendli.modules.quantizer.awq.models.gpt_neox import AWQGPTNeoXHook
 from friendli.modules.quantizer.awq.models.gptj import AWQGPTJHook
 from friendli.modules.quantizer.awq.models.llama import AWQLlamaHook
 from friendli.modules.quantizer.awq.models.mpt import AWQMPTHook
 from friendli.modules.quantizer.base import CommonQuantizer, FP8QuantHook, FP8Quantizer
+from friendli.modules.quantizer.models.dbrx import DbrxHook
 from friendli.modules.quantizer.models.llama import LlamaHook
 from friendli.modules.quantizer.models.mixtral import MixtralHook
 from friendli.modules.quantizer.models.mpt import MPTHook
 from friendli.modules.quantizer.schema.config import OneOfQuantConfig
 from friendli.modules.quantizer.smoothquant.base import (
     SmoothQuantHook,
     SmoothQuantQuantizer,
@@ -52,30 +53,32 @@
     "GPTJForCausalLM": AWQGPTJHook,
     "GPTNeoXForCausalLM": AWQGPTNeoXHook,
     "LlamaForCausalLM": AWQLlamaHook,
     "MPTForCausalLM": AWQMPTHook,
     "MistralForCausalLM": AWQLlamaHook,
 }
 
-model_arch_common_hook_map: Dict[str, type[FP8QuantHook]] = {
+model_arch_fp8_hook_map: Dict[str, type[FP8QuantHook]] = {
     "LlamaForCausalLM": LlamaHook,
     "MistralForCausalLM": LlamaHook,
     "MixtralForCausalLM": MixtralHook,
     "MPTForCausalLM": MPTHook,
+    "CohereForCausalLM": LlamaHook,
+    "DbrxForCausalLM": DbrxHook,
 }
 
 
 def get_quanthook_map(quant_mode: QuantMode) -> Dict[str, Any]:
     """Get quantizer map."""
     if quant_mode == QuantMode.SMOOTH_QUANT:
         return model_arch_smoothquant_hook_map
     if quant_mode == QuantMode.AWQ:
         return model_arch_awq_hook_map
     if quant_mode == QuantMode.FP8:
-        return model_arch_common_hook_map
+        return model_arch_fp8_hook_map
     raise NotSupportedQuantModeError(
         invalid_option=quant_mode,
         valid_options=[e.value for e in QuantMode],
     )
 
 
 def get_quantizer_class(quant_mode: QuantMode) -> Type[CommonQuantizer]:
```

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/models/llama.py` & `friendli_client-1.3.5/friendli/modules/quantizer/models/llama.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     HFQuantInput,
     HFTFQuantInputs,
     TFQuantInputs,
 )
 
 
 class LlamaHook(FP8QuantHook):
-    """CommonQuantHook for LlamaForCausalLM."""
+    """FP8QuantHook for LlamaForCausalLM."""
 
     def get_tf_blocks(self, model: torch.nn.Module) -> List[torch.nn.Module]:
         """Returns the transformer blocks in LlamaForCausalLM."""
         return model.model.layers
 
     def get_linear_layer_types(self) -> Tuple[Type[torch.nn.Module]]:
         """Returns the linear layer types in LlamaForCausalLM."""
```

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/models/mixtral.py` & `friendli_client-1.3.5/friendli/modules/quantizer/models/mixtral.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Copyright (c) 2024-present, FriendliAI Inc. All rights reserved.
 
-"""Friendli LlamaForCausalLM QuantizerHook."""
+"""Friendli MixtralForCausalLM QuantizerHook."""
 
 # mypy: ignore-errors
 
 from __future__ import annotations
 
-from dataclasses import dataclass
-from typing import Iterator, List, Tuple, Type
+from typing import Iterator, List
 
 import torch
 
 from friendli.modules.quantizer.models.llama import LlamaHook
 from friendli.modules.quantizer.schema.data import (
     HFQuantInput,
     HFTFQuantInputs,
@@ -21,15 +20,15 @@
 
 class MixtralHook(LlamaHook):
     """FP8QuantHook for MixtralForCausalLM."""
 
     def iter_tf_quant_inputs(
         self, model: torch.nn.Module
     ) -> Iterator[TFQuantInputs] | Iterator[HFTFQuantInputs]:
-        """Returns the layers which should be quantized in transformer block of LlamaForCausalLM."""
+        """Returns the layers which should be quantized in transformer block of MixtralForCausalLM."""
         for index, decoder_layer in enumerate(
             self.get_tf_blocks(model)  # type: ignore[union-attr, arg-type]
         ):
             self_attn = decoder_layer.self_attn
             block_sparse_moe = decoder_layer.block_sparse_moe
             moe_ff1_ff_gate_target_names = []
             for expert_idx in range(self.converter.num_experts):
@@ -58,14 +57,22 @@
                         target_names=[
                             f"{self.quantized_layer_prefix}{index}.self_attn.o_proj",
                         ],
                         local_names=[
                             "o_proj",
                         ],
                     ),
+                    # router
+                    HFQuantInput(
+                        parent_module=block_sparse_moe,
+                        target_names=[
+                            f"{self.quantized_layer_prefix}{index}.block_sparse_moe.gate",
+                        ],
+                        local_names=["gate"],
+                    ),
                     # ff1, ff_gate in each moe
                     HFQuantInput(
                         parent_module=block_sparse_moe.experts,
                         target_names=moe_ff1_ff_gate_target_names,
                         local_names=["w1", "w3"],
                     ),
                     # ff2 in each moe
```

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/models/mpt.py` & `friendli_client-1.3.5/friendli/modules/quantizer/models/mpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 
 """Friendli MPTForCausalLM QuantizerHook."""
 
 # mypy: ignore-errors
 
 from __future__ import annotations
 
-from dataclasses import dataclass
 from typing import Iterator, List, Tuple, Type
 
 import torch
 
 from friendli.modules.quantizer.base import FP8QuantHook
 from friendli.modules.quantizer.schema.data import (
     HFQuantInput,
     HFTFQuantInputs,
     TFQuantInputs,
 )
 
 
 class MPTHook(FP8QuantHook):
-    """CommonQuantHook for MPTForCausalLM."""
+    """FP8QuantHook for MPTForCausalLM."""
 
     def get_tf_blocks(self, model: torch.nn.Module) -> List[torch.nn.Module]:
         """Returns the transformer blocks in MPTForCausalLM."""
         return model.transformer.blocks
 
     def get_linear_layer_types(self) -> Tuple[Type[torch.nn.Module]]:
         """Returns the linear layer types in MPTForCausalLM."""
```

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/schema/config.py` & `friendli_client-1.3.5/friendli/modules/quantizer/schema/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 from friendli.enums import ModelDataType, QuantDatasetFormat, QuantMode
 
 
 class CalibrationDatasetConfig(BaseModel):
     """Calibration dataset config."""
 
-    path_or_name: str = "lambada"
+    path_or_name: str = "cnn_dailymail:3.0.0"
     format: QuantDatasetFormat = QuantDatasetFormat.JSON
     split: str = "validation"
-    lookup_column_name: str = "text"
-    num_samples: int = 128
+    lookup_column_name: str = "article"
+    num_samples: int = 512
     max_length: int = 512
 
 
 class AbstractQuantConfig(BaseModel):
     """Abstract quantization config."""
 
     mode: QuantMode
```

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/schema/data.py` & `friendli_client-1.3.5/friendli/modules/quantizer/schema/data.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/base.py` & `friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/bloom.py` & `friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/bloom.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/codegen.py` & `friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/codegen.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/falcon.py` & `friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/falcon.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/gpt2.py` & `friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/gpt_neox.py` & `friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/gptj.py` & `friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/gptj.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/llama.py` & `friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/llama.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/mpt.py` & `friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/mpt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/opt.py` & `friendli_client-1.3.5/friendli/modules/quantizer/smoothquant/models/opt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/modules/quantizer/utils.py` & `friendli_client-1.3.5/friendli/modules/quantizer/utils.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/api/v1/chat/completions.py` & `friendli_client-1.3.5/friendli/schema/api/v1/chat/completions.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/api/v1/codegen/chat_completions_pb2.py` & `friendli_client-1.3.5/friendli/schema/api/v1/codegen/chat_completions_pb2.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/api/v1/codegen/chat_completions_pb2.pyi` & `friendli_client-1.3.5/friendli/schema/api/v1/codegen/chat_completions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/api/v1/codegen/completions_pb2.py` & `friendli_client-1.3.5/friendli/schema/api/v1/codegen/completions_pb2.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/api/v1/codegen/completions_pb2.pyi` & `friendli_client-1.3.5/friendli/schema/api/v1/codegen/completions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/api/v1/codegen/text_to_image_pb2.py` & `friendli_client-1.3.5/friendli/schema/api/v1/codegen/text_to_image_pb2.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/api/v1/codegen/text_to_image_pb2.pyi` & `friendli_client-1.3.5/friendli/schema/api/v1/codegen/text_to_image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/api/v1/completions.py` & `friendli_client-1.3.5/friendli/schema/api/v1/completions.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/api/v1/images/image.py` & `friendli_client-1.3.5/friendli/schema/api/v1/images/image.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/api/v1/proto/chat_completions.proto` & `friendli_client-1.3.5/friendli/schema/api/v1/proto/chat_completions.proto`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/api/v1/proto/completions.proto` & `friendli_client-1.3.5/friendli/schema/api/v1/proto/completions.proto`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/resource/v1/attributes.py` & `friendli_client-1.3.5/friendli/schema/resource/v1/attributes.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/resource/v1/endpoint.py` & `friendli_client-1.3.5/friendli/schema/resource/v1/endpoint.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/schema/resource/v1/transfer.py` & `friendli_client-1.3.5/friendli/schema/resource/v1/transfer.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/sdk/api/base.py` & `friendli_client-1.3.5/friendli/sdk/api/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/sdk/api/chat/chat.py` & `friendli_client-1.3.5/friendli/sdk/api/chat/chat.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/sdk/api/chat/completions.py` & `friendli_client-1.3.5/friendli/sdk/api/chat/completions.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/sdk/api/completions.py` & `friendli_client-1.3.5/friendli/sdk/api/completions.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/sdk/api/images/images.py` & `friendli_client-1.3.5/friendli/sdk/api/images/images.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/sdk/api/images/text_to_image.py` & `friendli_client-1.3.5/friendli/sdk/api/images/text_to_image.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/sdk/client.py` & `friendli_client-1.3.5/friendli/sdk/client.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/sdk/resource/base.py` & `friendli_client-1.3.5/friendli/sdk/resource/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/sdk/resource/endpoint.py` & `friendli_client-1.3.5/friendli/sdk/resource/endpoint.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/sdk/resource/model.py` & `friendli_client-1.3.5/friendli/sdk/resource/model.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/settings.py` & `friendli_client-1.3.5/friendli/settings.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/utils/compat.py` & `friendli_client-1.3.5/friendli/utils/compat.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/utils/decorator.py` & `friendli_client-1.3.5/friendli/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/utils/format.py` & `friendli_client-1.3.5/friendli/utils/format.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/utils/fs.py` & `friendli_client-1.3.5/friendli/utils/fs.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/utils/prompt.py` & `friendli_client-1.3.5/friendli/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/utils/request.py` & `friendli_client-1.3.5/friendli/utils/request.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/utils/testing.py` & `friendli_client-1.3.5/friendli/utils/testing.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/utils/transfer.py` & `friendli_client-1.3.5/friendli/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/utils/url.py` & `friendli_client-1.3.5/friendli/utils/url.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/utils/validate.py` & `friendli_client-1.3.5/friendli/utils/validate.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/friendli/utils/version.py` & `friendli_client-1.3.5/friendli/utils/version.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.4/pyproject.toml` & `friendli_client-1.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "friendli-client"
-version = "1.3.4"
+version = "1.3.5"
 description = "Client of Friendli Suite."
 license = "Apache-2.0"
 authors = ["FriendliAI teams <eng@friendli.ai>"]
 packages = [
     { include = "friendli" },
 ]
 include = ["friendli/py.typed"]
@@ -30,24 +30,24 @@
 requests = "^2"
 PyYaml = "^6.0.1"
 typer = "^0.9.0"
 rich = "^12.2.0"
 jsonschema = "^4.17.3"
 tqdm = "^4.48.0"
 pydantic = {extras = ["email"], version = ">=1.9.0, <3"}
-transformers = { version = "4.36.2", optional = true }
+transformers = { version = "4.40.0", optional = true }
 h5py = { version = "^3.9.0", optional = true }
 einops = { version = "^0.6.1", optional = true }
 accelerate = { version = "0.21.0", optional = true }
 datasets = { version = "2.16.0", optional = true }
 injector = "^0.21.0"
 protobuf = "^4.24.2"
 types-protobuf = "^4.24.0.1"
 peft = { version = "0.6.0", optional = true }
-safetensors = { version = "0.3.2", optional = true }
+safetensors = { version = "0.4.1", optional = true }
 httpx = "^0.24.1"
 fastapi = "^0.104.0"
 uvicorn = "^0.23.2"
 gql = "^3.4.1"
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `friendli_client-1.3.4/PKG-INFO` & `friendli_client-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: friendli-client
-Version: 1.3.4
+Version: 1.3.5
 Summary: Client of Friendli Suite.
 Home-page: https://friendli.ai/
 License: Apache-2.0
 Keywords: generative-ai,serving,llm,inference,finetuning
 Author: FriendliAI teams
 Author-email: eng@friendli.ai
 Requires-Python: >=3.8.1,<4.0.0
@@ -26,17 +26,17 @@
 Requires-Dist: injector (>=0.21.0,<0.22.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: peft (==0.6.0) ; extra == "mllib"
 Requires-Dist: protobuf (>=4.24.2,<5.0.0)
 Requires-Dist: pydantic[email] (>=1.9.0,<3)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: rich (>=12.2.0,<13.0.0)
-Requires-Dist: safetensors (==0.3.2) ; extra == "mllib"
+Requires-Dist: safetensors (==0.4.1) ; extra == "mllib"
 Requires-Dist: tqdm (>=4.48.0,<5.0.0)
-Requires-Dist: transformers (==4.36.2) ; extra == "mllib"
+Requires-Dist: transformers (==4.40.0) ; extra == "mllib"
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: types-protobuf (>=4.24.0.1,<5.0.0.0)
 Requires-Dist: uvicorn (>=0.23.2,<0.24.0)
 Project-URL: Documentation, https://docs.friendli.ai/
 Project-URL: Repository, https://github.com/friendliai/friendli-client
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: friendli-client Version: 1.3.4 Summary: Client of
+Metadata-Version: 2.1 Name: friendli-client Version: 1.3.5 Summary: Client of
 Friendli Suite. Home-page: https://friendli.ai/ License: Apache-2.0 Keywords:
 generative-ai,serving,llm,inference,finetuning Author: FriendliAI teams Author-
 email: eng@friendli.ai Requires-Python: >=3.8.1,<4.0.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Provides-
@@ -11,16 +11,16 @@
 "mllib" Requires-Dist: einops (>=0.6.1,<0.7.0) ; extra == "mllib" Requires-
 Dist: fastapi (>=0.104.0,<0.105.0) Requires-Dist: gql (>=3.4.1,<4.0.0)
 Requires-Dist: h5py (>=3.9.0,<4.0.0) ; extra == "mllib" Requires-Dist: httpx
 (>=0.24.1,<0.25.0) Requires-Dist: injector (>=0.21.0,<0.22.0) Requires-Dist:
 jsonschema (>=4.17.3,<5.0.0) Requires-Dist: peft (==0.6.0) ; extra == "mllib"
 Requires-Dist: protobuf (>=4.24.2,<5.0.0) Requires-Dist: pydantic[email]
 (>=1.9.0,<3) Requires-Dist: requests (>=2,<3) Requires-Dist: rich
-(>=12.2.0,<13.0.0) Requires-Dist: safetensors (==0.3.2) ; extra == "mllib"
-Requires-Dist: tqdm (>=4.48.0,<5.0.0) Requires-Dist: transformers (==4.36.2) ;
+(>=12.2.0,<13.0.0) Requires-Dist: safetensors (==0.4.1) ; extra == "mllib"
+Requires-Dist: tqdm (>=4.48.0,<5.0.0) Requires-Dist: transformers (==4.40.0) ;
 extra == "mllib" Requires-Dist: typer (>=0.9.0,<0.10.0) Requires-Dist: types-
 protobuf (>=4.24.0.1,<5.0.0.0) Requires-Dist: uvicorn (>=0.23.2,<0.24.0)
 Project-URL: Documentation, https://docs.friendli.ai/ Project-URL: Repository,
 https://github.com/friendliai/friendli-client Description-Content-Type: text/
 markdown
                                 [Friendli Logo]
 ********** SSuuppeerrcchhaarrggee GGeenneerraattiivvee AAII SSeerrvviinngg wwiitthh FFrriieennddllii ?ð??? **********
```

