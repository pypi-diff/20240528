# Comparing `tmp/nestipy-0.3.5.tar.gz` & `tmp/nestipy-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy-0.3.5.tar", max compression
+gzip compressed data, was "nestipy-0.3.7.tar", max compression
```

## Comparing `nestipy-0.3.5.tar` & `nestipy-0.3.7.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0     1054 2024-05-25 05:58:23.876165 nestipy-0.3.5/LICENSE
--rw-r--r--   0        0        0     1906 2024-05-25 05:58:23.876165 nestipy-0.3.5/README.md
--rw-r--r--   0        0        0      681 2024-05-25 05:58:33.348290 nestipy-0.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/__init__.py
--rw-r--r--   0        0        0     1251 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/__init__.py
--rw-r--r--   0        0        0     1489 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      652 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
--rw-r--r--   0        0        0     1005 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/config/__init__.py
--rw-r--r--   0        0        0      246 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/decorator/__init__.py
--rw-r--r--   0        0        0     2957 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/decorator/class_.py
--rw-r--r--   0        0        0     1204 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/decorator/method.py
--rw-r--r--   0        0        0      367 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/exception/__init__.py
--rw-r--r--   0        0        0      732 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/exception/decorator.py
--rw-r--r--   0        0        0      433 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/exception/http.py
--rw-r--r--   0        0        0      364 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/exception/interface.py
--rw-r--r--   0        0        0     2531 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/exception/message.py
--rw-r--r--   0        0        0      113 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/exception/meta.py
--rw-r--r--   0        0        0     1686 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/exception/status.py
--rw-r--r--   0        0        0      164 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/guards/__init__.py
--rw-r--r--   0        0        0      326 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/guards/can_activate.py
--rw-r--r--   0        0        0      332 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/guards/decorator.py
--rw-r--r--   0        0        0       45 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/guards/meta.py
--rw-r--r--   0        0        0      719 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/helpers/__init__.py
--rw-r--r--   0        0        0      208 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/http_/__init__.py
--rw-r--r--   0        0        0     4503 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/http_/multipart.py
--rw-r--r--   0        0        0     5299 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/http_/request.py
--rw-r--r--   0        0        0     5321 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/http_/response.py
--rw-r--r--   0        0        0      478 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/http_/test.py
--rw-r--r--   0        0        0     1403 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/http_/upload_file.py
--rw-r--r--   0        0        0      303 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/http_/websocket.py
--rw-r--r--   0        0        0      199 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/interceptor/__init__.py
--rw-r--r--   0        0        0      489 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/interceptor/decorator.py
--rw-r--r--   0        0        0      352 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/interceptor/interface.py
--rw-r--r--   0        0        0       52 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/interceptor/meta.py
--rw-r--r--   0        0        0       54 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/logger.py
--rw-r--r--   0        0        0      248 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/middleware/__init__.py
--rw-r--r--   0        0        0      695 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/middleware/cors.py
--rw-r--r--   0        0        0      323 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/middleware/interface.py
--rw-r--r--   0        0        0      100 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/middleware/meta.py
--rw-r--r--   0        0        0     3276 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/middleware/session.py
--rw-r--r--   0        0        0      167 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/template/__init__.py
--rw-r--r--   0        0        0      274 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/template/decorator.py
--rw-r--r--   0        0        0      627 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/template/interface.py
--rw-r--r--   0        0        0      109 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/template/meta.py
--rw-r--r--   0        0        0     1590 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/common/utils.py
--rw-r--r--   0        0        0      933 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/__init__.py
--rw-r--r--   0        0        0     1179 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16492 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
--rw-r--r--   0        0        0     1929 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/__pycache__/factory.cpython-311.pyc
--rw-r--r--   0        0        0     1567 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0      212 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/adapter/__init__.py
--rw-r--r--   0        0        0     4224 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/adapter/blacksheep_adapter.py
--rw-r--r--   0        0        0     3803 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/adapter/fastapi_adapter.py
--rw-r--r--   0        0        0     5666 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/adapter/http_adapter.py
--rw-r--r--   0        0        0      418 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/constant.py
--rw-r--r--   0        0        0        0 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/context/__init__.py
--rw-r--r--   0        0        0     1741 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/context/argument_host.py
--rw-r--r--   0        0        0     1613 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/context/execution_context.py
--rw-r--r--   0        0        0      526 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/context/graphql_argument_host.py
--rw-r--r--   0        0        0      369 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/context/http_argument_host.py
--rw-r--r--   0        0        0      556 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/context/websocket_argument_host.py
--rw-r--r--   0        0        0      730 2024-05-25 05:58:23.908166 nestipy-0.3.5/src/nestipy/core/discover.py
--rw-r--r--   0        0        0       90 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/exception/__init__.py
--rw-r--r--   0        0        0     4040 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/exception/processor.py
--rw-r--r--   0        0        0       75 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/guards/__init__.py
--rw-r--r--   0        0        0     2164 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/guards/processor.py
--rw-r--r--   0        0        0     4528 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/instance_loader.py
--rw-r--r--   0        0        0       82 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/interceptor/__init__.py
--rw-r--r--   0        0        0     2569 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/interceptor/processor.py
--rw-r--r--   0        0        0        0 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/meta/__init__.py
--rw-r--r--   0        0        0      380 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/meta/controller_metadata_creator.py
--rw-r--r--   0        0        0     4040 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/meta/metadata_creator.py
--rw-r--r--   0        0        0      771 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/meta/module_metadata_creator.py
--rw-r--r--   0        0        0      374 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/meta/provider_metadata_creator.py
--rw-r--r--   0        0        0      162 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/middleware/__init__.py
--rw-r--r--   0        0        0     3973 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/middleware/executor.py
--rw-r--r--   0        0        0     8913 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/nestipy_application.py
--rw-r--r--   0        0        0     1317 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/nestipy_factory.py
--rw-r--r--   0        0        0       64 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/on_destroy.py
--rw-r--r--   0        0        0       60 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/on_init.py
--rw-r--r--   0        0        0       89 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/platform/__init__.py
--rw-r--r--   0        0        0      608 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3199 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
--rw-r--r--   0        0        0     7185 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
--rw-r--r--   0        0        0     7397 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/router/__init__.py
--rw-r--r--   0        0        0     2879 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/router/route_explorer.py
--rw-r--r--   0        0        0      510 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/router/route_extractor.py
--rw-r--r--   0        0        0     7355 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/router/router_proxy.py
--rw-r--r--   0        0        0      184 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/template/__init__.py
--rw-r--r--   0        0        0     1004 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/template/minimal_jinja.py
--rw-r--r--   0        0        0     1457 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/core/template/processor.py
--rw-r--r--   0        0        0      231 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/dynamic_module/__init__.py
--rw-r--r--   0        0        0     3512 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/dynamic_module/builder.py
--rw-r--r--   0        0        0      139 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/dynamic_module/module/__init__.py
--rw-r--r--   0        0        0      517 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/dynamic_module/module/consumer.py
--rw-r--r--   0        0        0      251 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/dynamic_module/module/interface.py
--rw-r--r--   0        0        0      282 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/__init__.py
--rw-r--r--   0        0        0     1533 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/decorator.py
--rw-r--r--   0        0        0     2244 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/graphql_adapter.py
--rw-r--r--   0        0        0     1768 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/graphql_asgi.py
--rw-r--r--   0        0        0     1871 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/graphql_explorer.py
--rw-r--r--   0        0        0      584 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/graphql_module.py
--rw-r--r--   0        0        0     4392 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/graphql_proxy.py
--rw-r--r--   0        0        0      289 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/meta.py
--rw-r--r--   0        0        0     1531 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/playground/graphql-playground-default.html
--rw-r--r--   0        0        0     3486 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/playground/graphql-playground-graphiql.html
--rw-r--r--   0        0        0      704 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/pubsub.py
--rw-r--r--   0        0        0      648 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/strawberry/__init__.py
--rw-r--r--   0        0        0     2103 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/strawberry/strawberry_adapter.py
--rw-r--r--   0        0        0     1588 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/strawberry/strawberry_asgi.py
--rw-r--r--   0        0        0      110 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/graphql/test.py
--rw-r--r--   0        0        0      848 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/ioc/__init__.py
--rw-r--r--   0        0        0      444 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/ioc/annotation.py
--rw-r--r--   0        0        0    10995 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/ioc/container.py
--rw-r--r--   0        0        0     1029 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/ioc/context_container.py
--rw-r--r--   0        0        0     5504 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/ioc/dependency.py
--rw-r--r--   0        0        0      602 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/ioc/meta.py
--rw-r--r--   0        0        0     3013 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/ioc/middleware.py
--rw-r--r--   0        0        0      877 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/ioc/provider.py
--rw-r--r--   0        0        0       57 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/ioc/utils.py
--rw-r--r--   0        0        0      458 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/metadata/__init__.py
--rw-r--r--   0        0        0     1673 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/metadata/class_.py
--rw-r--r--   0        0        0      508 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/metadata/container.py
--rw-r--r--   0        0        0      710 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/metadata/decorator.py
--rw-r--r--   0        0        0     1004 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/metadata/dependency.py
--rw-r--r--   0        0        0      236 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/metadata/module.py
--rw-r--r--   0        0        0       88 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/metadata/provider_token.py
--rw-r--r--   0        0        0      688 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/metadata/reflect.py
--rw-r--r--   0        0        0      107 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/metadata/route.py
--rw-r--r--   0        0        0     1105 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/__init__.py
--rw-r--r--   0        0        0       49 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/constant.py
--rw-r--r--   0        0        0     3145 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/decorator.py
--rw-r--r--   0        0        0     1587 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/document_builder.py
--rw-r--r--   0        0        0      423 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/explorer.py
--rw-r--r--   0        0        0       44 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/__init__.py
--rw-r--r--   0        0        0     4684 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/common.py
--rw-r--r--   0        0        0     1325 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/__init__.py
--rw-r--r--   0        0        0     1757 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/common.py
--rw-r--r--   0        0        0     1855 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/contents.py
--rw-r--r--   0        0        0      633 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/generate.py
--rw-r--r--   0        0        0     3196 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/jinja.py
--rw-r--r--   0        0        0     1894 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/md.py
--rw-r--r--   0        0        0     3065 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/texts.py
--rw-r--r--   0        0        0    21375 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py
--rw-r--r--   0        0        0     4250 2024-05-25 05:58:23.912166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/examples.py
--rw-r--r--   0        0        0      103 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/README.md
--rw-r--r--   0        0        0        0 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/__init__.py
--rw-r--r--   0        0        0      890 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html
--rw-r--r--   0        0        0      610 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html
--rw-r--r--   0        0        0      730 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html
--rw-r--r--   0        0        0      135 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-schemas.html
--rw-r--r--   0        0        0      322 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-security-schemes.html
--rw-r--r--   0        0        0      284 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/content-examples.html
--rw-r--r--   0        0        0      207 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/external-docs.html
--rw-r--r--   0        0        0      571 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html
--rw-r--r--   0        0        0      873 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html
--rw-r--r--   0        0        0        0 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-auth.html
--rw-r--r--   0        0        0      480 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-body.html
--rw-r--r--   0        0        0      492 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-parameters.html
--rw-r--r--   0        0        0     1335 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html
--rw-r--r--   0        0        0      929 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html
--rw-r--r--   0        0        0      224 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/servers.html
--rw-r--r--   0        0        0      227 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/tags.html
--rw-r--r--   0        0        0      429 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/type.html
--rw-r--r--   0        0        0      286 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/README.md
--rw-r--r--   0        0        0        0 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/__init__.py
--rw-r--r--   0        0        0      889 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html
--rw-r--r--   0        0        0      933 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html
--rw-r--r--   0        0        0      843 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html
--rw-r--r--   0        0        0      135 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-schemas.html
--rw-r--r--   0        0        0      561 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html
--rw-r--r--   0        0        0      383 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/content-examples.html
--rw-r--r--   0        0        0      326 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/external-docs.html
--rw-r--r--   0        0        0      817 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html
--rw-r--r--   0        0        0     1007 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html
--rw-r--r--   0        0        0        0 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-auth.html
--rw-r--r--   0        0        0      616 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html
--rw-r--r--   0        0        0      857 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html
--rw-r--r--   0        0        0     2250 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html
--rw-r--r--   0        0        0     1155 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html
--rw-r--r--   0        0        0      475 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/servers.html
--rw-r--r--   0        0        0      227 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/tags.html
--rw-r--r--   0        0        0      638 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html
--rw-r--r--   0        0        0      170 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/README.md
--rw-r--r--   0        0        0      548 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html
--rw-r--r--   0        0        0      670 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html
--rw-r--r--   0        0        0      156 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/README.md
--rw-r--r--   0        0        0      754 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html
--rw-r--r--   0        0        0      670 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
--rw-r--r--   0        0        0        0 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/utils/__init__.py
--rw-r--r--   0        0        0     2844 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/utils/source.py
--rw-r--r--   0        0        0      878 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/utils/web.py
--rw-r--r--   0        0        0     9579 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/v2.py
--rw-r--r--   0        0        0     9667 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/openapi_docs/v3.py
--rw-r--r--   0        0        0     1323 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/swagger.html
--rw-r--r--   0        0        0     2707 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/swagger_module.py
--rw-r--r--   0        0        0     2676 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/openapi/test.py
--rw-r--r--   0        0        0      220 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/types_/__init__.py
--rw-r--r--   0        0        0      393 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/types_/handler.py
--rw-r--r--   0        0        0      123 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/types_/http.py
--rw-r--r--   0        0        0      309 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/websocket/__init__.py
--rw-r--r--   0        0        0     3323 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/websocket/adapter.py
--rw-r--r--   0        0        0      716 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/websocket/decorator.py
--rw-r--r--   0        0        0     4611 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/websocket/proxy.py
--rw-r--r--   0        0        0      316 2024-05-25 05:58:23.916166 nestipy-0.3.5/src/nestipy/websocket/socket_request.py
--rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 nestipy-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-05-28 13:14:17.462167 nestipy-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1906 2024-05-28 13:14:17.462167 nestipy-0.3.7/README.md
+-rw-r--r--   0        0        0      681 2024-05-28 13:14:27.866151 nestipy-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/__init__.py
+-rw-r--r--   0        0        0     1489 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      652 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
+-rw-r--r--   0        0        0     1005 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/config/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/decorator/__init__.py
+-rw-r--r--   0        0        0     2957 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/decorator/class_.py
+-rw-r--r--   0        0        0     1204 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/decorator/method.py
+-rw-r--r--   0        0        0      367 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/decorator.py
+-rw-r--r--   0        0        0      433 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/http.py
+-rw-r--r--   0        0        0      364 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/interface.py
+-rw-r--r--   0        0        0     2531 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/message.py
+-rw-r--r--   0        0        0      113 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/meta.py
+-rw-r--r--   0        0        0     1686 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/status.py
+-rw-r--r--   0        0        0      164 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/guards/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/guards/can_activate.py
+-rw-r--r--   0        0        0      332 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/guards/decorator.py
+-rw-r--r--   0        0        0       45 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/guards/meta.py
+-rw-r--r--   0        0        0      971 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/helpers/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/__init__.py
+-rw-r--r--   0        0        0     4503 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/multipart.py
+-rw-r--r--   0        0        0     5299 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/request.py
+-rw-r--r--   0        0        0     5321 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/response.py
+-rw-r--r--   0        0        0      478 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/test.py
+-rw-r--r--   0        0        0     1403 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/upload_file.py
+-rw-r--r--   0        0        0      303 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/websocket.py
+-rw-r--r--   0        0        0      199 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/interceptor/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/interceptor/decorator.py
+-rw-r--r--   0        0        0      352 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/interceptor/interface.py
+-rw-r--r--   0        0        0       52 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/interceptor/meta.py
+-rw-r--r--   0        0        0       54 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/logger.py
+-rw-r--r--   0        0        0      248 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/middleware/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/middleware/cors.py
+-rw-r--r--   0        0        0      323 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/middleware/interface.py
+-rw-r--r--   0        0        0      100 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/middleware/meta.py
+-rw-r--r--   0        0        0     3276 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/middleware/session.py
+-rw-r--r--   0        0        0      167 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/template/__init__.py
+-rw-r--r--   0        0        0      274 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/template/decorator.py
+-rw-r--r--   0        0        0      627 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/template/interface.py
+-rw-r--r--   0        0        0      109 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/template/meta.py
+-rw-r--r--   0        0        0     1590 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/utils.py
+-rw-r--r--   0        0        0      933 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/__init__.py
+-rw-r--r--   0        0        0     1179 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16492 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
+-rw-r--r--   0        0        0     1929 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     1567 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0      212 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/adapter/__init__.py
+-rw-r--r--   0        0        0     4224 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/adapter/blacksheep_adapter.py
+-rw-r--r--   0        0        0     3803 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/adapter/fastapi_adapter.py
+-rw-r--r--   0        0        0     5666 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/adapter/http_adapter.py
+-rw-r--r--   0        0        0      418 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/constant.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/context/__init__.py
+-rw-r--r--   0        0        0     1741 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/context/argument_host.py
+-rw-r--r--   0        0        0     1613 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/context/execution_context.py
+-rw-r--r--   0        0        0      526 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/context/graphql_argument_host.py
+-rw-r--r--   0        0        0      369 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/context/http_argument_host.py
+-rw-r--r--   0        0        0      556 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/context/websocket_argument_host.py
+-rw-r--r--   0        0        0      730 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/discover.py
+-rw-r--r--   0        0        0       90 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/exception/__init__.py
+-rw-r--r--   0        0        0     4040 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/exception/processor.py
+-rw-r--r--   0        0        0       75 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/guards/__init__.py
+-rw-r--r--   0        0        0     2164 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/guards/processor.py
+-rw-r--r--   0        0        0     4566 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/instance_loader.py
+-rw-r--r--   0        0        0       82 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/interceptor/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/interceptor/processor.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/meta/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/meta/controller_metadata_creator.py
+-rw-r--r--   0        0        0     4040 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/meta/metadata_creator.py
+-rw-r--r--   0        0        0      771 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/meta/module_metadata_creator.py
+-rw-r--r--   0        0        0      374 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/meta/provider_metadata_creator.py
+-rw-r--r--   0        0        0      162 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/middleware/__init__.py
+-rw-r--r--   0        0        0     3973 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/middleware/executor.py
+-rw-r--r--   0        0        0     8913 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/nestipy_application.py
+-rw-r--r--   0        0        0     1317 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/nestipy_factory.py
+-rw-r--r--   0        0        0       64 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/on_destroy.py
+-rw-r--r--   0        0        0       60 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/on_init.py
+-rw-r--r--   0        0        0       89 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/platform/__init__.py
+-rw-r--r--   0        0        0      608 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3199 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
+-rw-r--r--   0        0        0     7185 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
+-rw-r--r--   0        0        0     7397 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/router/__init__.py
+-rw-r--r--   0        0        0     2879 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/router/route_explorer.py
+-rw-r--r--   0        0        0      510 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/router/route_extractor.py
+-rw-r--r--   0        0        0     7389 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/router/router_proxy.py
+-rw-r--r--   0        0        0      184 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/template/__init__.py
+-rw-r--r--   0        0        0     1004 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/template/minimal_jinja.py
+-rw-r--r--   0        0        0     1457 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/template/processor.py
+-rw-r--r--   0        0        0      231 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/dynamic_module/__init__.py
+-rw-r--r--   0        0        0     3512 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/dynamic_module/builder.py
+-rw-r--r--   0        0        0      139 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/dynamic_module/module/__init__.py
+-rw-r--r--   0        0        0      517 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/dynamic_module/module/consumer.py
+-rw-r--r--   0        0        0      251 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/dynamic_module/module/interface.py
+-rw-r--r--   0        0        0      282 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/__init__.py
+-rw-r--r--   0        0        0     1533 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/decorator.py
+-rw-r--r--   0        0        0     2244 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/graphql_adapter.py
+-rw-r--r--   0        0        0     1768 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/graphql_asgi.py
+-rw-r--r--   0        0        0     1871 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/graphql_explorer.py
+-rw-r--r--   0        0        0      584 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/graphql_module.py
+-rw-r--r--   0        0        0     4315 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/graphql_proxy.py
+-rw-r--r--   0        0        0      289 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/meta.py
+-rw-r--r--   0        0        0     1531 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/playground/graphql-playground-default.html
+-rw-r--r--   0        0        0     3486 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/playground/graphql-playground-graphiql.html
+-rw-r--r--   0        0        0      704 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/pubsub.py
+-rw-r--r--   0        0        0      648 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/strawberry/__init__.py
+-rw-r--r--   0        0        0     2103 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/strawberry/strawberry_adapter.py
+-rw-r--r--   0        0        0     1588 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/strawberry/strawberry_asgi.py
+-rw-r--r--   0        0        0      110 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/test.py
+-rw-r--r--   0        0        0      848 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/__init__.py
+-rw-r--r--   0        0        0      449 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/annotation.py
+-rw-r--r--   0        0        0    10665 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/container.py
+-rw-r--r--   0        0        0      831 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/context_container.py
+-rw-r--r--   0        0        0     5679 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/dependency.py
+-rw-r--r--   0        0        0      602 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/meta.py
+-rw-r--r--   0        0        0     3013 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/middleware.py
+-rw-r--r--   0        0        0      877 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/provider.py
+-rw-r--r--   0        0        0       57 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/utils.py
+-rw-r--r--   0        0        0      458 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/__init__.py
+-rw-r--r--   0        0        0     1748 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/class_.py
+-rw-r--r--   0        0        0      508 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/container.py
+-rw-r--r--   0        0        0      710 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/decorator.py
+-rw-r--r--   0        0        0     1004 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/dependency.py
+-rw-r--r--   0        0        0      236 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/module.py
+-rw-r--r--   0        0        0       88 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/provider_token.py
+-rw-r--r--   0        0        0      688 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/reflect.py
+-rw-r--r--   0        0        0      107 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/route.py
+-rw-r--r--   0        0        0     1133 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/constant.py
+-rw-r--r--   0        0        0     3227 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/decorator.py
+-rw-r--r--   0        0        0     1587 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/document_builder.py
+-rw-r--r--   0        0        0      424 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/explorer.py
+-rw-r--r--   0        0        0       44 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/__init__.py
+-rw-r--r--   0        0        0     4684 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/common.py
+-rw-r--r--   0        0        0     1325 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/__init__.py
+-rw-r--r--   0        0        0     1757 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/common.py
+-rw-r--r--   0        0        0     1855 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/contents.py
+-rw-r--r--   0        0        0      633 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/generate.py
+-rw-r--r--   0        0        0     3196 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/jinja.py
+-rw-r--r--   0        0        0     1894 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/md.py
+-rw-r--r--   0        0        0     3065 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/texts.py
+-rw-r--r--   0        0        0    21375 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py
+-rw-r--r--   0        0        0     4250 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/examples.py
+-rw-r--r--   0        0        0      103 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/__init__.py
+-rw-r--r--   0        0        0      890 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html
+-rw-r--r--   0        0        0      610 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html
+-rw-r--r--   0        0        0      730 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-schemas.html
+-rw-r--r--   0        0        0      322 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      284 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/content-examples.html
+-rw-r--r--   0        0        0      207 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/external-docs.html
+-rw-r--r--   0        0        0      571 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html
+-rw-r--r--   0        0        0      873 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html
+-rw-r--r--   0        0        0        0 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-auth.html
+-rw-r--r--   0        0        0      480 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-body.html
+-rw-r--r--   0        0        0      492 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-parameters.html
+-rw-r--r--   0        0        0     1335 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html
+-rw-r--r--   0        0        0      929 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html
+-rw-r--r--   0        0        0      224 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/servers.html
+-rw-r--r--   0        0        0      227 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/tags.html
+-rw-r--r--   0        0        0      429 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/type.html
+-rw-r--r--   0        0        0      286 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/__init__.py
+-rw-r--r--   0        0        0      889 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html
+-rw-r--r--   0        0        0      933 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html
+-rw-r--r--   0        0        0      843 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-schemas.html
+-rw-r--r--   0        0        0      561 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      383 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/content-examples.html
+-rw-r--r--   0        0        0      326 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/external-docs.html
+-rw-r--r--   0        0        0      817 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html
+-rw-r--r--   0        0        0     1007 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html
+-rw-r--r--   0        0        0        0 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-auth.html
+-rw-r--r--   0        0        0      616 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html
+-rw-r--r--   0        0        0      857 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html
+-rw-r--r--   0        0        0     2250 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html
+-rw-r--r--   0        0        0     1155 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html
+-rw-r--r--   0        0        0      475 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/servers.html
+-rw-r--r--   0        0        0      227 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/tags.html
+-rw-r--r--   0        0        0      638 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html
+-rw-r--r--   0        0        0      170 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/README.md
+-rw-r--r--   0        0        0      548 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html
+-rw-r--r--   0        0        0      670 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html
+-rw-r--r--   0        0        0      156 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/README.md
+-rw-r--r--   0        0        0      754 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html
+-rw-r--r--   0        0        0      670 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
+-rw-r--r--   0        0        0        0 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/utils/__init__.py
+-rw-r--r--   0        0        0     2844 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/utils/source.py
+-rw-r--r--   0        0        0      878 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/utils/web.py
+-rw-r--r--   0        0        0     9579 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/v2.py
+-rw-r--r--   0        0        0     9667 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/v3.py
+-rw-r--r--   0        0        0     1323 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/swagger.html
+-rw-r--r--   0        0        0     2707 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/swagger_module.py
+-rw-r--r--   0        0        0     2676 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/test.py
+-rw-r--r--   0        0        0      220 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/types_/__init__.py
+-rw-r--r--   0        0        0      393 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/types_/handler.py
+-rw-r--r--   0        0        0      123 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/types_/http.py
+-rw-r--r--   0        0        0      309 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/websocket/__init__.py
+-rw-r--r--   0        0        0     3323 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/websocket/adapter.py
+-rw-r--r--   0        0        0      716 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/websocket/decorator.py
+-rw-r--r--   0        0        0     4556 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/websocket/proxy.py
+-rw-r--r--   0        0        0      316 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/websocket/socket_request.py
+-rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 nestipy-0.3.7/PKG-INFO
```

### Comparing `nestipy-0.3.5/LICENSE` & `nestipy-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/README.md` & `nestipy-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/pyproject.toml` & `nestipy-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nestipy"
-version = "0.3.5"
+version = "0.3.7"
 description = "Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS"
 authors = ["tsiresymila <tsiresymila@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "nestipy", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nestipy-0.3.5/src/nestipy/common/__init__.py` & `nestipy-0.3.7/src/nestipy/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.7/src/nestipy/common/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/__pycache__/http_method.cpython-311.pyc` & `nestipy-0.3.7/src/nestipy/common/__pycache__/http_method.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/config/__init__.py` & `nestipy-0.3.7/src/nestipy/common/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/decorator/class_.py` & `nestipy-0.3.7/src/nestipy/common/decorator/class_.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/decorator/method.py` & `nestipy-0.3.7/src/nestipy/common/decorator/method.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/exception/decorator.py` & `nestipy-0.3.7/src/nestipy/common/exception/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/exception/message.py` & `nestipy-0.3.7/src/nestipy/common/exception/message.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/exception/status.py` & `nestipy-0.3.7/src/nestipy/common/exception/status.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/helpers/__init__.py` & `nestipy-0.3.7/src/nestipy/common/helpers/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from typing import Type
 
 from nestipy.ioc import ModuleProviderDict
-from nestipy.metadata import ModuleMetadata, Reflect
+from nestipy.metadata import Reflect, ClassMetadata, ModuleMetadata
 
 
 class SpecialProviderExtractor:
 
     @classmethod
     def extract_special_providers(
             cls,
             module_class: Type,
             subclass: Type,
             key: str
     ) -> list[Type]:
         providers = []
-        for p in Reflect.get_metadata(module_class, ModuleMetadata.Providers, []):
+        class_providers = Reflect.get_metadata(module_class, ModuleMetadata.Providers, [])
+        metadata: ClassMetadata = Reflect.get_metadata(module_class, ClassMetadata.Metadata, None)
+        if metadata is not None:
+            class_providers += metadata.get_global_providers()
+        for p in class_providers:
             if (isinstance(p, ModuleProviderDict) and
                     isinstance(p.token, str) and p.token.startswith(key) and p.use_class is not None):
                 if issubclass(p.use_class, subclass):
                     providers.append(p.use_class)
         return providers
```

### Comparing `nestipy-0.3.5/src/nestipy/common/http_/multipart.py` & `nestipy-0.3.7/src/nestipy/common/http_/multipart.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/http_/request.py` & `nestipy-0.3.7/src/nestipy/common/http_/request.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/http_/response.py` & `nestipy-0.3.7/src/nestipy/common/http_/response.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/http_/upload_file.py` & `nestipy-0.3.7/src/nestipy/common/http_/upload_file.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/middleware/cors.py` & `nestipy-0.3.7/src/nestipy/common/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/middleware/session.py` & `nestipy-0.3.7/src/nestipy/common/middleware/session.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/template/interface.py` & `nestipy-0.3.7/src/nestipy/common/template/interface.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/common/utils.py` & `nestipy-0.3.7/src/nestipy/common/utils.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/__init__.py` & `nestipy-0.3.7/src/nestipy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.7/src/nestipy/core/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/__pycache__/app_context.cpython-311.pyc` & `nestipy-0.3.7/src/nestipy/core/__pycache__/app_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/__pycache__/factory.cpython-311.pyc` & `nestipy-0.3.7/src/nestipy/core/__pycache__/factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/__pycache__/utils.cpython-311.pyc` & `nestipy-0.3.7/src/nestipy/core/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/adapter/blacksheep_adapter.py` & `nestipy-0.3.7/src/nestipy/core/adapter/blacksheep_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/adapter/fastapi_adapter.py` & `nestipy-0.3.7/src/nestipy/core/adapter/fastapi_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/adapter/http_adapter.py` & `nestipy-0.3.7/src/nestipy/core/adapter/http_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/context/argument_host.py` & `nestipy-0.3.7/src/nestipy/core/context/argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/context/execution_context.py` & `nestipy-0.3.7/src/nestipy/core/context/execution_context.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/context/graphql_argument_host.py` & `nestipy-0.3.7/src/nestipy/core/context/graphql_argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/context/websocket_argument_host.py` & `nestipy-0.3.7/src/nestipy/core/context/websocket_argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/discover.py` & `nestipy-0.3.7/src/nestipy/core/discover.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/exception/processor.py` & `nestipy-0.3.7/src/nestipy/core/exception/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/guards/processor.py` & `nestipy-0.3.7/src/nestipy/core/guards/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/instance_loader.py` & `nestipy-0.3.7/src/nestipy/core/instance_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+import inspect
 import typing
 from typing import Type, Any
 
 from nestipy.dynamic_module import DynamicModule, MiddlewareConsumer, NestipyModule
 from nestipy.ioc import NestipyContainer, ModuleProviderDict
 from nestipy.metadata import ModuleMetadata, Reflect
 
@@ -49,15 +50,15 @@
                 self.graphql_instance = instance
             imports = Reflect.get_metadata(module, ModuleMetadata.Imports, [])
             await self.create_instances(imports)
         # Create  NestipyInterceptor, CanActivate, NestipyMiddleware,ExceptionFilter without scope
         container = NestipyContainer.get_instance()
         all_services = container.get_all_services()
         for service in [
-            s for s in all_services if issubclass(s, (
+            s for s in all_services if inspect.isclass(s) and issubclass(s, (
                     NestipyInterceptor,
                     CanActivate,
                     NestipyMiddleware,
                     ExceptionFilter
             ))
         ]:
             await self.create_instance(service, with_scope=False)
```

### Comparing `nestipy-0.3.5/src/nestipy/core/interceptor/processor.py` & `nestipy-0.3.7/src/nestipy/core/interceptor/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/meta/metadata_creator.py` & `nestipy-0.3.7/src/nestipy/core/meta/metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/meta/module_metadata_creator.py` & `nestipy-0.3.7/src/nestipy/core/meta/module_metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/middleware/executor.py` & `nestipy-0.3.7/src/nestipy/core/middleware/executor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/nestipy_application.py` & `nestipy-0.3.7/src/nestipy/core/nestipy_application.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/nestipy_factory.py` & `nestipy-0.3.7/src/nestipy/core/nestipy_factory.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.7/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc` & `nestipy-0.3.7/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc` & `nestipy-0.3.7/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc` & `nestipy-0.3.7/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/router/route_explorer.py` & `nestipy-0.3.7/src/nestipy/core/router/route_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/router/router_proxy.py` & `nestipy-0.3.7/src/nestipy/core/router/router_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,21 @@
                     # OPEN API REGISTER
                     if path in json_paths.keys():
                         route_path = json_paths[path]
                     else:
                         route_path = {}
                     if "responses" not in route['openapi'].keys():
                         continue
-                    route_path[method.lower()] = Operation(
-                        **route['openapi'],
-                        summary=snakecase_to_camelcase(method_name)
-                    )
-                    json_paths[path] = route_path
+
+                    if 'no_swagger' not in route['openapi'].keys():
+                        route_path[method.lower()] = Operation(
+                            **route['openapi'],
+                            summary=snakecase_to_camelcase(method_name)
+                        )
+                        json_paths[path] = route_path
         paths = {}
         for path, op in json_paths.items():
             paths[path] = PathItem(**op)
         return paths
 
     def create_request_handler(
             self,
@@ -81,15 +83,14 @@
                 self.router,
                 module_ref,
                 controller,
                 controller_method_handler,
                 req,
                 res
             )
-            context_container.set_container(container)
             context_container.set_execution_context(execution_context)
             handler_response: Response
             try:
                 # TODO : Refactor
                 guard_processor: GuardProcessor = await NestipyContainer.get_instance().get(GuardProcessor)
                 can_activate = await guard_processor.process(execution_context)
                 if not can_activate[0]:
```

### Comparing `nestipy-0.3.5/src/nestipy/core/template/minimal_jinja.py` & `nestipy-0.3.7/src/nestipy/core/template/minimal_jinja.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/core/template/processor.py` & `nestipy-0.3.7/src/nestipy/core/template/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/dynamic_module/builder.py` & `nestipy-0.3.7/src/nestipy/dynamic_module/builder.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/dynamic_module/module/consumer.py` & `nestipy-0.3.7/src/nestipy/dynamic_module/module/consumer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/graphql/decorator.py` & `nestipy-0.3.7/src/nestipy/graphql/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/graphql/graphql_adapter.py` & `nestipy-0.3.7/src/nestipy/graphql/graphql_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/graphql/graphql_asgi.py` & `nestipy-0.3.7/src/nestipy/graphql/graphql_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/graphql/graphql_explorer.py` & `nestipy-0.3.7/src/nestipy/graphql/graphql_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/graphql/graphql_module.py` & `nestipy-0.3.7/src/nestipy/graphql/graphql_module.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/graphql/graphql_proxy.py` & `nestipy-0.3.7/src/nestipy/graphql/graphql_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,14 @@
                 getattr(resolver, method_name),
                 None,
                 None,
                 kwargs,
                 None
 
             )
-            context_container.set_container(NestipyContainer.get_instance())
             context_container.set_execution_context(execution_context)
             try:
                 # TODO: Refactor with routerProxy
                 # create execution context
 
                 #  apply guards
                 guard_processor: GuardProcessor = await self.container.get(GuardProcessor)
```

### Comparing `nestipy-0.3.5/src/nestipy/graphql/playground/graphql-playground-default.html` & `nestipy-0.3.7/src/nestipy/graphql/playground/graphql-playground-default.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/graphql/playground/graphql-playground-graphiql.html` & `nestipy-0.3.7/src/nestipy/graphql/playground/graphql-playground-graphiql.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/graphql/pubsub.py` & `nestipy-0.3.7/src/nestipy/graphql/pubsub.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/graphql/strawberry/__init__.py` & `nestipy-0.3.7/src/nestipy/graphql/strawberry/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/graphql/strawberry/strawberry_adapter.py` & `nestipy-0.3.7/src/nestipy/graphql/strawberry/strawberry_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/graphql/strawberry/strawberry_asgi.py` & `nestipy-0.3.7/src/nestipy/graphql/strawberry/strawberry_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/ioc/__init__.py` & `nestipy-0.3.7/src/nestipy/ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/ioc/container.py` & `nestipy-0.3.7/src/nestipy/ioc/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,29 +79,21 @@
                 else:
                     uniq_providers.append(m)
             return uniq(uniq_providers)
         # raise ValueError(f"Dependency Metadata not found  for {service.__name__} service ")
         return []
 
     @classmethod
-    def _data_to_typed(cls, annotation: Union[Type, Any], data: Union[dict, list, str, int, tuple, set, Any]):
-        if dataclasses.is_dataclass(annotation) or issubclass(annotation, BaseModel):
-            return annotation(**data)
-        elif annotation in (dict, list, str, int, tuple, set, Any):
-            return data
-        return None
-
-    @classmethod
-    async def _resolve_context_service(cls, dep_key: TypeAnnotated, annotation: Union[Type, Any]):
+    async def _resolve_context_service(cls, name: str, dep_key: TypeAnnotated, annotation: Union[Type, Any]):
         context_container = RequestContextContainer.get_instance()
         callback = dep_key.metadata.callback
         if inspect.iscoroutinefunction(callback):
-            return await callback(dep_key.metadata.token, annotation, context_container)
+            return await callback(name, dep_key.metadata.token, annotation, context_container)
         else:
-            return callback(dep_key.metadata.token, annotation, context_container)
+            return callback(name, dep_key.metadata.token, annotation, context_container)
 
     async def _resolve_module_provider_dict(self, instance: "ModuleProviderDict", search_scope: list):
         if instance.value:
             return instance.value
         elif instance.existing:
             if isinstance(instance.existing, ProviderToken):
                 return await self.get(instance.existing.key)
@@ -124,15 +116,15 @@
         if key in self._singleton_instances:
             instance = self._singleton_instances[key]
             # to keep improve
             if isinstance(instance, ModuleProviderDict):
                 search_scope = self.get_dependency_metadata(instance)
                 if instance.token in search_scope:
                     value = await self._resolve_module_provider_dict(instance, search_scope=search_scope)
-                    # update singleton instance to have the async valur from ModuleProviderDict
+                    # update singleton instance to have the async value from ModuleProviderDict
                     self._singleton_instances[key] = value
                     return value
                 else:
                     raise ValueError(
                         f"Service {instance.__class__.__name__} "
                         f"not found in scope")
             else:
@@ -157,15 +149,15 @@
         search_scope = self.get_dependency_metadata(service)
         origin.add(service)
         annotations: dict = getattr(service, '__annotations__', {})
         for name, param_annotation in annotations.items():
             annotation, dep_key = self.helper.get_type_from_annotation(param_annotation)
             if dep_key.metadata.key in CtxDepKey.to_list():
                 if dep_key.metadata.key is not CtxDepKey.Service:
-                    dependency = await self._resolve_context_service(dep_key, annotation)
+                    dependency = await self._resolve_context_service(name, dep_key, annotation)
                     setattr(service, name, dependency)
                 elif dep_key.metadata.token in search_scope or annotation in search_scope or disable_scope:
                     dependency = await self.get(dep_key.metadata.token or annotation)
                     setattr(service, name, dependency)
                 else:
                     _name: str = annotation.__name__ if not isinstance(annotation, str) else annotation
                     raise ValueError(
@@ -179,15 +171,15 @@
     async def _get_method_dependency(self, method_to_resolve: Callable, search_scope: list, origin: list):
         params = inspect.signature(method_to_resolve).parameters
         args = {}
         for name, param in params.items():
             if name != 'self' and param.annotation is not inspect.Parameter.empty:
                 annotation, dep_key = self.helper.get_type_from_annotation(param.annotation)
                 if dep_key.metadata.key in CtxDepKey.to_list() and dep_key.metadata.key is not CtxDepKey.Service:
-                    dependency = await self._resolve_context_service(dep_key, annotation)
+                    dependency = await self._resolve_context_service(name, dep_key, annotation)
                     args[name] = dependency
                 elif annotation in search_scope:
                     dependency = await self.get(annotation, origin=origin)
                     args[name] = dependency
                 else:
                     _name: str = annotation.__name__ if not isinstance(annotation, str) else annotation
                     raise ValueError(f"Service {_name} not found in scope {search_scope}")
```

### Comparing `nestipy-0.3.5/src/nestipy/ioc/context_container.py` & `nestipy-0.3.7/src/nestipy/ioc/context_container.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,30 +4,24 @@
     from nestipy.core import ExecutionContext
     from nestipy.ioc import NestipyContainer
 
 
 class RequestContextContainer:
     _instance: Union["RequestContextContainer", None] = None
     execution_context: Union["ExecutionContext", None] = None
-    container: Union["NestipyContainer", None] = None
 
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super(RequestContextContainer, cls).__new__(cls, *args, **kwargs)
         return cls._instance
 
     @classmethod
     def set_execution_context(cls, context: "ExecutionContext"):
         ins = cls.get_instance()
         ins.execution_context = context
 
     @classmethod
-    def set_container(cls, container: "NestipyContainer"):
-        ins = cls.get_instance()
-        ins.container = container
-
-    @classmethod
     def get_instance(cls, *args, **kwargs):
         return RequestContextContainer(*args, **kwargs)
 
     def destroy(self):
         self._instance = None
```

### Comparing `nestipy-0.3.5/src/nestipy/ioc/dependency.py` & `nestipy-0.3.7/src/nestipy/ioc/dependency.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,105 +17,106 @@
         return TypeAnnotated(ParamAnnotation(self.metadata.callback, self.metadata.key, token))
 
 
 def create_type_annotated(callback: TypeAnnotatedCallable, key: str) -> TypeAnnotated:
     return TypeAnnotated(ParamAnnotation(callback, key))
 
 
-def inject_callback(token: Optional[str], type_ref: Type, _request_context: RequestContextContainer):
-    return _request_context.container.get(token or type_ref)
+def inject_callback(_name: str, _token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+    return None
 
 
-def instance_callback(_token: Optional[str], type_ref: Type, _request_context: RequestContextContainer):
-    return _request_context.container.get(type_ref)
+def instance_callback(_name: str, _token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+    return None
 
 
-def req_callback(token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def req_callback(_name: str, _token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
     return _request_context.execution_context.get_request()
 
 
-def res_callback(token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def res_callback(_name: str, _token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
     return _request_context.execution_context.get_response()
 
 
-def to_validate_value(value: Any, _type_ref: Type):
+def to_valid_value(value: Any, _type_ref: Type):
     if is_dataclass(_type_ref):
         return _type_ref(**value)
     elif issubclass(_type_ref, BaseModel):
         return _type_ref.model_validate(value)
     return value
 
 
-async def body_callback(token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+async def body_callback(_name: str, _token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
     req = _request_context.execution_context.get_request()
     form_data = await req.form()
     if form_data is not None:
-        return to_validate_value(form_data, _type_ref)
+        return to_valid_value(form_data, _type_ref)
     else:
-        return to_validate_value(await req.json(), _type_ref)
+        return to_valid_value(await req.json(), _type_ref)
 
 
 def _get_request_param_value(
         key: str,
         _type_ref: Type, _request_context: RequestContextContainer,
         token: Optional[str] = None
 ):
     req = _request_context.execution_context.get_request()
     value: dict = getattr(req, key)
     if token:
         return value.get(token)
     else:
-        return to_validate_value(value, _type_ref)
+        return to_valid_value(value, _type_ref)
 
 
-def session_callback(token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def session_callback(_name: str, token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
     return _get_request_param_value('session', _type_ref, _request_context, token)
 
 
-def cookie_callback(token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def cookie_callback(_name: str, token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
     return _get_request_param_value('cookies', _type_ref, _request_context, token)
 
 
-def query_callback(token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def query_callback(_name: str, token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
     return _get_request_param_value('query_params', _type_ref, _request_context, token)
 
 
-def params_callback(token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def params_callback(_name: str, token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
     return _get_request_param_value('path_params', _type_ref, _request_context, token)
 
 
-def headers_callback(token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def headers_callback(_name: str, token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
     return _get_request_param_value('headers', _type_ref, _request_context, token)
 
 
-def args_callback(token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def args_callback(_name: str, _token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
     args = _request_context.execution_context.switch_to_graphql().get_args()
-    if token:
-        return args.get(token)
-    else:
-        return args
+    return args.get(_name)
 
 
-def context_callback(_token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def context_callback(_name: str, _token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
     return _request_context
 
 
-def graphql_context_callback(_token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def graphql_context_callback(_name: str, _token: Optional[str], _type_ref: Type,
+                             _request_context: RequestContextContainer):
     return _request_context.execution_context.switch_to_graphql().get_context()
 
 
-def websocket_server_callback(_token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def websocket_server_callback(_name: str, _token: Optional[str], _type_ref: Type,
+                              _request_context: RequestContextContainer):
     return _request_context.execution_context.switch_to_websocket().get_server()
 
 
-def websocket_client_callback(_token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def websocket_client_callback(_name: str, _token: Optional[str], _type_ref: Type,
+                              _request_context: RequestContextContainer):
     return _request_context.execution_context.switch_to_websocket().get_client()
 
 
-def websocket_data_callback(_token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+def websocket_data_callback(_name: str, _token: Optional[str], _type_ref: Type,
+                            _request_context: RequestContextContainer):
     return _request_context.execution_context.switch_to_websocket().get_data()
 
 
 Instance = create_type_annotated(instance_callback, 'instance')
 Inject = create_type_annotated(inject_callback, CtxDepKey.Service)
 Req = create_type_annotated(req_callback, CtxDepKey.Request)
 Res = create_type_annotated(res_callback, CtxDepKey.Response)
```

### Comparing `nestipy-0.3.5/src/nestipy/ioc/meta.py` & `nestipy-0.3.7/src/nestipy/ioc/meta.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/ioc/middleware.py` & `nestipy-0.3.7/src/nestipy/ioc/middleware.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/ioc/provider.py` & `nestipy-0.3.7/src/nestipy/ioc/provider.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/metadata/class_.py` & `nestipy-0.3.7/src/nestipy/metadata/class_.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     def __init__(self, module: Callable, global_providers: list = None):
         self._module = module
         self._global_providers = global_providers or []
 
     def get_module(self):
         return self._module
 
+    def get_global_providers(self):
+        return self._global_providers
+
     def get_service_providers(self):
         providers = Reflect.get_metadata(self._module, ModuleMetadata.Providers, [])
         import_providers_form_exports = []
         # Only not a root module need to get import_providers to share
         # if not Reflect.get_metadata(self._module, ModuleMetadata.Root, False):
         for im in Reflect.get_metadata(self._module, ModuleMetadata.Imports, []):
             exports = Reflect.get_metadata(im.module if hasattr(im, 'module') else im, ModuleMetadata.Exports, [])
```

### Comparing `nestipy-0.3.5/src/nestipy/metadata/decorator.py` & `nestipy-0.3.7/src/nestipy/metadata/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/metadata/dependency.py` & `nestipy-0.3.7/src/nestipy/metadata/dependency.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/metadata/reflect.py` & `nestipy-0.3.7/src/nestipy/metadata/reflect.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/__init__.py` & `nestipy-0.3.7/src/nestipy/openapi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 
 from pydantic import create_model
 
-from .decorator import ApiBearerAuth, ApiBasicAuth, ApiSecurity
+from .decorator import ApiBearerAuth, ApiBasicAuth, ApiSecurity, NoSwagger
 from .decorator import ApiResponse, ApiCreatedResponse, ApiOkResponse, ApiNotFoundResponse
 from .decorator import ApiTags, ApiId, ApiBody, ApiParameter
 from .document_builder import DocumentBuilder
 from .swagger_module import SwaggerModule
 
 
 def ApiSchema(cls):
@@ -41,9 +41,10 @@
     "ApiNotFoundResponse",
     "ApiTags",
     "ApiId",
     "ApiBody",
     "ApiParameter",
     "ApiBearerAuth",
     "ApiBasicAuth",
-    "ApiSecurity"
+    "ApiSecurity",
+    "NoSwagger"
 ]
```

### Comparing `nestipy-0.3.5/src/nestipy/openapi/decorator.py` & `nestipy-0.3.7/src/nestipy/openapi/decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     return SetMetadata(key='__openapi__request_body', data=body)
 
 
 def ApiResponse(status: int, response: Response):
     return SetMetadata(key='__openapi__responses', data={status: response}, as_dict=True)
 
 
+def NoSwagger():
+    return SetMetadata(key='__openapi__no_swagger', data=True)
+
+
 def ApiOkResponse(description: Optional[str] = None, schema: Schema = None, example: Any = None):
     return ApiResponse(
         status=200,
         response=Response(
             description or 'Success response',
             content={
                 'application/json': MediaType(
```

### Comparing `nestipy-0.3.5/src/nestipy/openapi/document_builder.py` & `nestipy-0.3.7/src/nestipy/openapi/document_builder.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/common.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/common.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/__init__.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/common.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/common.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/contents.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/contents.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/generate.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/generate.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/jinja.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/jinja.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/md.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/md.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/texts.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/texts.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/examples.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/examples.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/utils/source.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/utils/source.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/utils/web.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/utils/web.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/v2.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/v2.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/openapi_docs/v3.py` & `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/v3.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/swagger.html` & `nestipy-0.3.7/src/nestipy/openapi/swagger.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/swagger_module.py` & `nestipy-0.3.7/src/nestipy/openapi/swagger_module.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/openapi/test.py` & `nestipy-0.3.7/src/nestipy/openapi/test.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/websocket/adapter.py` & `nestipy-0.3.7/src/nestipy/websocket/adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/websocket/decorator.py` & `nestipy-0.3.7/src/nestipy/websocket/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.5/src/nestipy/websocket/proxy.py` & `nestipy-0.3.7/src/nestipy/websocket/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,14 @@
                 None,
                 None,
                 io_adapter,
                 client,
                 data
             )
             context_container.set_execution_context(execution_context)
-            context_container.set_container(container)
             try:
                 result = await container.get(gateway, method_name)
                 if result is not None:
                     # get success event from handler
                     success_event = Reflect.get_metadata(gateway, SUCCESS_EVENT_KEY, None)
                     # send response to websocket
                     await self.call_handler(io_adapter.emit, {
```

### Comparing `nestipy-0.3.5/PKG-INFO` & `nestipy-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestipy
-Version: 0.3.5
+Version: 0.3.7
 Summary: Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nestipy Version: 0.3.5 Summary: Nestipy is a Python
+Metadata-Version: 2.1 Name: nestipy Version: 0.3.7 Summary: Nestipy is a Python
 framework built on top of BlackSheep that follows the modular architecture of
 NestJS Author: tsiresymila Author-email: tsiresymila@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: blacksheep (>=2.0.7,<3.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: minijinja
```

