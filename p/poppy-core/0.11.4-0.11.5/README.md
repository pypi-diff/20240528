# Comparing `tmp/poppy-core-0.11.4.tar.gz` & `tmp/poppy_core-0.11.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poppy-core-0.11.4.tar", max compression
+gzip compressed data, was "poppy_core-0.11.5.tar", max compression
```

## Comparing `poppy-core-0.11.4.tar` & `poppy_core-0.11.5.tar`

### file list

```diff
@@ -1,85 +1,84 @@
--rw-r--r--   0        0        0    21863 2022-12-06 17:18:33.679073 poppy-core-0.11.4/LICENSE
--rw-r--r--   0        0        0     1320 2022-12-06 17:18:33.679073 poppy-core-0.11.4/README.md
--rw-r--r--   0        0        0       64 2022-12-06 17:18:33.679073 poppy-core-0.11.4/poppy/__init__.py
--rw-r--r--   0        0        0      307 2022-12-06 17:18:33.679073 poppy-core-0.11.4/poppy/core/__init__.py
--rw-r--r--   0        0        0    11002 2022-12-06 17:18:33.679073 poppy-core-0.11.4/poppy/core/command.py
--rw-r--r--   0        0        0     1316 2022-12-06 17:18:33.679073 poppy-core-0.11.4/poppy/core/conf/__init__.py
--rw-r--r--   0        0        0      478 2022-12-06 17:18:33.679073 poppy-core-0.11.4/poppy/core/conf/default_settings.py
--rw-r--r--   0        0        0     3170 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/conf/logger.json
--rw-r--r--   0        0        0     5375 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/configuration.py
--rw-r--r--   0        0        0        0 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/db/__init__.py
--rw-r--r--   0        0        0      258 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/db/base.py
--rw-r--r--   0        0        0     4693 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/db/connector.py
--rw-r--r--   0        0        0    15019 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/db/database.py
--rw-r--r--   0        0        0     1554 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/db/dry_runner.py
--rw-r--r--   0        0        0     7975 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/db/handlers.py
--rw-r--r--   0        0        0        0 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/db/models/__init__.py
--rw-r--r--   0        0        0     2549 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/db/non_null_column.py
--rw-r--r--   0        0        0        0 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/generic/__init__.py
--rw-r--r--   0        0        0      968 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/generic/cache.py
--rw-r--r--   0        0        0     3612 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/generic/dot_dict.py
--rw-r--r--   0        0        0     1639 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/generic/graph.py
--rw-r--r--   0        0        0     3706 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/generic/manager.py
--rw-r--r--   0        0        0     2866 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/generic/metaclasses.py
--rw-r--r--   0        0        0     2478 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/generic/paths.py
--rw-r--r--   0        0        0      730 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/generic/requests.py
--rw-r--r--   0        0        0     1812 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/generic/signals.py
--rw-r--r--   0        0        0     1428 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/generic/timer.py
--rw-r--r--   0        0        0      333 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/logger.py
--rw-r--r--   0        0        0    12434 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/loop.py
--rw-r--r--   0        0        0        0 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/__init__.py
--rw-r--r--   0        0        0    11481 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/commands.py
--rw-r--r--   0        0        0      882 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/pipeline_template/config.json-tpl
--rw-r--r--   0        0        0     1566 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/pipeline_template/descriptor.json-tpl
--rw-r--r--   0        0        0      898 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/pipeline_template/manage.py
--rw-r--r--   0        0        0      202 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/pipeline_template/requirements.txt
--rw-r--r--   0        0        0      617 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/pipeline_template/settings.py-tpl
--rw-r--r--   0        0        0       84 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/MANIFEST.in-tpl
--rw-r--r--   0        0        0      593 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/README.rst-tpl
--rw-r--r--   0        0        0       64 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/__init__.py-tpl
--rw-r--r--   0        0        0        0 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/__init__.py-tpl
--rw-r--r--   0        0        0     1285 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/commands.py-tpl
--rw-r--r--   0        0        0      698 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/descriptor.json-tpl
--rw-r--r--   0        0        0      732 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/models/__init__.py-tpl
--rw-r--r--   0        0        0      196 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/models/versions/README.rst
--rw-r--r--   0        0        0      637 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/tasks.py-tpl
--rw-r--r--   0        0        0     1684 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/tests.py-tpl
--rw-r--r--   0        0        0        0 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/requirements.txt
--rw-r--r--   0        0        0     1342 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/setup.py-tpl
--rw-r--r--   0        0        0        0 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/management/templates/plugin_template/system_reqs.ini
--rw-r--r--   0        0        0    23542 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/pipeline.py
--rw-r--r--   0        0        0     7125 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/plugin.py
--rw-r--r--   0        0        0     1486 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/properties.py
--rw-r--r--   0        0        0      116 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/target/__init__.py
--rw-r--r--   0        0        0     8627 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/target/base_target.py
--rw-r--r--   0        0        0     6977 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/target/file_target.py
--rw-r--r--   0        0        0     2056 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/target/py_object_target.py
--rw-r--r--   0        0        0      131 2022-12-06 17:18:33.683073 poppy-core-0.11.4/poppy/core/task/__init__.py
--rw-r--r--   0        0        0    11785 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/task/base_task.py
--rw-r--r--   0        0        0     5168 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/task/task.py
--rw-r--r--   0        0        0     9533 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/test.py
--rw-r--r--   0        0        0       49 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/__init__.py
--rw-r--r--   0        0        0     1097 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/appdirs/LICENSE.txt
--rw-r--r--   0        0        0     4272 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/appdirs/README.rst
--rw-r--r--   0        0        0       47 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/appdirs/__init__.py
--rw-r--r--   0        0        0    22475 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/appdirs/appdirs.py
--rw-r--r--   0        0        0       87 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/cdf/__init__.py
--rw-r--r--   0        0        0   176499 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/cdf/cdf.py
--rw-r--r--   0        0        0    15202 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/cdf/const.py
--rw-r--r--   0        0        0     3337 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/exceptions.py
--rw-r--r--   0        0        0      331 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/hashfile.py
--rw-r--r--   0        0        0      423 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/imports.py
--rw-r--r--   0        0        0     2350 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/lock.py
--rw-r--r--   0        0        0     1885 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/poppy_argparse.py
--rw-r--r--   0        0        0     1150 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/poppy_logging/TerminalColorFormatter.py
--rw-r--r--   0        0        0      169 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/poppy_logging/__init__.py
--rw-r--r--   0        0        0     1327 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/poppy_logging/rotating_file_handler.py
--rw-r--r--   0        0        0       69 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/test/__init__.py
--rw-r--r--   0        0        0      585 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/text.py
--rw-r--r--   0        0        0     1042 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/xml.py
--rw-r--r--   0        0        0     1085 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/xmltodict/LICENSE.txt
--rw-r--r--   0        0        0       93 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/xmltodict/__init__.py
--rw-r--r--   0        0        0    12585 2022-12-06 17:18:33.687073 poppy-core-0.11.4/poppy/core/tools/xmltodict/xmltodict.py
--rw-r--r--   0        0        0     1059 2022-12-06 17:18:33.687073 poppy-core-0.11.4/pyproject.toml
--rw-r--r--   0        0        0     3076 2022-12-06 17:19:01.792997 poppy-core-0.11.4/setup.py
--rw-r--r--   0        0        0     2108 2022-12-06 17:19:01.793514 poppy-core-0.11.4/PKG-INFO
+-rw-r--r--   0        0        0    21863 2024-05-28 13:20:37.917591 poppy_core-0.11.5/LICENSE
+-rw-r--r--   0        0        0     1320 2024-05-28 13:20:37.921591 poppy_core-0.11.5/README.md
+-rw-r--r--   0        0        0       64 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/__init__.py
+-rw-r--r--   0        0        0      307 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/__init__.py
+-rw-r--r--   0        0        0    10982 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/command.py
+-rw-r--r--   0        0        0     1316 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/conf/__init__.py
+-rw-r--r--   0        0        0      478 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/conf/default_settings.py
+-rw-r--r--   0        0        0     3170 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/conf/logger.json
+-rw-r--r--   0        0        0     5375 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/configuration.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:24:38.029967 poppy_core-0.11.5/poppy/core/db/__init__.py
+-rw-r--r--   0        0        0      258 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/db/base.py
+-rw-r--r--   0        0        0     4693 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/db/connector.py
+-rw-r--r--   0        0        0    15020 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/db/database.py
+-rw-r--r--   0        0        0     1554 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/db/dry_runner.py
+-rw-r--r--   0        0        0     7975 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/db/handlers.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:24:38.029967 poppy_core-0.11.5/poppy/core/db/models/__init__.py
+-rw-r--r--   0        0        0     2633 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/db/non_null_column.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:24:38.029967 poppy_core-0.11.5/poppy/core/generic/__init__.py
+-rw-r--r--   0        0        0      968 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/generic/cache.py
+-rw-r--r--   0        0        0     3612 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/generic/dot_dict.py
+-rw-r--r--   0        0        0     1639 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/generic/graph.py
+-rw-r--r--   0        0        0     3706 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/generic/manager.py
+-rw-r--r--   0        0        0     2866 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/generic/metaclasses.py
+-rw-r--r--   0        0        0     2478 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/generic/paths.py
+-rw-r--r--   0        0        0      730 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/generic/requests.py
+-rw-r--r--   0        0        0     1812 2024-05-28 13:20:37.921591 poppy_core-0.11.5/poppy/core/generic/signals.py
+-rw-r--r--   0        0        0     1428 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/generic/timer.py
+-rw-r--r--   0        0        0      333 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/logger.py
+-rw-r--r--   0        0        0    12434 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/loop.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:24:38.029967 poppy_core-0.11.5/poppy/core/management/__init__.py
+-rw-r--r--   0        0        0    11481 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/commands.py
+-rw-r--r--   0        0        0      882 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/pipeline_template/config.json-tpl
+-rw-r--r--   0        0        0     1566 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/pipeline_template/descriptor.json-tpl
+-rw-r--r--   0        0        0      898 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/pipeline_template/manage.py
+-rw-r--r--   0        0        0      202 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/pipeline_template/requirements.txt
+-rw-r--r--   0        0        0      617 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/pipeline_template/settings.py-tpl
+-rw-r--r--   0        0        0       84 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/MANIFEST.in-tpl
+-rw-r--r--   0        0        0      593 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/README.rst-tpl
+-rw-r--r--   0        0        0       64 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2024-05-28 13:24:38.029967 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/__init__.py-tpl
+-rw-r--r--   0        0        0     1285 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/commands.py-tpl
+-rw-r--r--   0        0        0      698 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/descriptor.json-tpl
+-rw-r--r--   0        0        0      732 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/models/__init__.py-tpl
+-rw-r--r--   0        0        0      196 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/models/versions/README.rst
+-rw-r--r--   0        0        0      637 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/tasks.py-tpl
+-rw-r--r--   0        0        0     1684 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/tests.py-tpl
+-rw-r--r--   0        0        0        0 2024-05-28 13:24:38.033967 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/requirements.txt
+-rw-r--r--   0        0        0     1342 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/setup.py-tpl
+-rw-r--r--   0        0        0        0 2024-05-28 13:24:38.033967 poppy_core-0.11.5/poppy/core/management/templates/plugin_template/system_reqs.ini
+-rw-r--r--   0        0        0    23542 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/pipeline.py
+-rw-r--r--   0        0        0     7125 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/plugin.py
+-rw-r--r--   0        0        0     1486 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/properties.py
+-rw-r--r--   0        0        0      116 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/target/__init__.py
+-rw-r--r--   0        0        0     8627 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/target/base_target.py
+-rw-r--r--   0        0        0     6977 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/target/file_target.py
+-rw-r--r--   0        0        0     2056 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/target/py_object_target.py
+-rw-r--r--   0        0        0      131 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/task/__init__.py
+-rw-r--r--   0        0        0    11785 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/task/base_task.py
+-rw-r--r--   0        0        0     5168 2024-05-28 13:20:37.925591 poppy_core-0.11.5/poppy/core/task/task.py
+-rw-r--r--   0        0        0     9533 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/test.py
+-rw-r--r--   0        0        0       49 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/__init__.py
+-rw-r--r--   0        0        0     1097 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/appdirs/LICENSE.txt
+-rw-r--r--   0        0        0     4272 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/appdirs/README.rst
+-rw-r--r--   0        0        0       47 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/appdirs/__init__.py
+-rw-r--r--   0        0        0    22475 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/appdirs/appdirs.py
+-rw-r--r--   0        0        0       87 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/cdf/__init__.py
+-rw-r--r--   0        0        0   176499 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/cdf/cdf.py
+-rw-r--r--   0        0        0    15202 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/cdf/const.py
+-rw-r--r--   0        0        0     3337 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/exceptions.py
+-rw-r--r--   0        0        0      331 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/hashfile.py
+-rw-r--r--   0        0        0      423 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/imports.py
+-rw-r--r--   0        0        0     2350 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/lock.py
+-rw-r--r--   0        0        0     1885 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/poppy_argparse.py
+-rw-r--r--   0        0        0     1150 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/poppy_logging/TerminalColorFormatter.py
+-rw-r--r--   0        0        0      169 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/poppy_logging/__init__.py
+-rw-r--r--   0        0        0     1327 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/poppy_logging/rotating_file_handler.py
+-rw-r--r--   0        0        0       69 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/test/__init__.py
+-rw-r--r--   0        0        0      585 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/text.py
+-rw-r--r--   0        0        0     1042 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/xml.py
+-rw-r--r--   0        0        0     1085 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/xmltodict/LICENSE.txt
+-rw-r--r--   0        0        0       93 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/xmltodict/__init__.py
+-rw-r--r--   0        0        0    12585 2024-05-28 13:20:37.929591 poppy_core-0.11.5/poppy/core/tools/xmltodict/xmltodict.py
+-rw-r--r--   0        0        0     1016 2024-05-28 13:20:37.933591 poppy_core-0.11.5/pyproject.toml
+-rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 poppy_core-0.11.5/PKG-INFO
```

### Comparing `poppy-core-0.11.4/LICENSE` & `poppy_core-0.11.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/README.md` & `poppy_core-0.11.5/README.md`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/command.py` & `poppy_core-0.11.5/poppy/core/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 import collections
 from poppy.core.logger import logger
 
 from poppy.core.generic.signals import Signal
 from poppy.core.tools.poppy_argparse import argparse
 from poppy.core.generic.metaclasses import ManagerMeta
 from poppy.core.pipeline import Pipeline
-__all__ = ["Command"]
+__all__ = ['Command']
 
 
 def after_creation(cls, name):
     """
     Some extra things to do after the creation of command classes (and not
     instances, this is not an error).
     """
     # check that the class has the good attributes
-    if not hasattr(cls, "__command__"):
+    if not hasattr(cls, '__command__'):
         logger.error(
-            "The class {0} has no attribute __command__".format(name)
+            'The class {0} has no attribute __command__'.format(name)
         )
         return
-    if not hasattr(cls, "__parent__"):
+    if not hasattr(cls, '__parent__'):
         logger.error(
-            "The class {0} has no attribute __parent__".format(name)
+            'The class {0} has no attribute __parent__'.format(name)
         )
         return
 
 
 class CommandManager(object):
     """
     A class to manage the available defined commands by the user through the
@@ -71,30 +71,30 @@
         self.run_end = Signal()
 
     def add(self, name, cls):
         """
         Adds the command and its class to the manager.
         """
         # register
-        logger.debug("Register the command {0}".format(name))
+        logger.debug('Register the command {0}'.format(name))
         self.commands[cls.__command__] = cls
 
         # add its dependence in the tree (none parent is the root tree)
         self.tree[cls.__parent__].append(cls.__command__)
 
         # send a signal of a new definition
         self.added(name, cls)
 
     def create(self, instance):
         """
         Register the instances of the commands by their name.
         """
         # register
         logger.debug(
-            "Register command instance {0}".format(instance.__command__)
+            'Register command instance {0}'.format(instance.__command__)
         )
         self.instancesByCommand[instance.__command__] = instance
 
         # send the signal of a new instantiation
         self.created(instance)
 
     def generate(self, options):
@@ -102,15 +102,15 @@
         Given a first base subparser and the parents parser, generate the
         parsers for children commands recursively.
         """
         # send signal that the generation is starting
         self.generation_start(options)
 
         # generate commands
-        logger.debug("Generating commands hierarchy")
+        logger.debug('Generating commands hierarchy')
         self._generate()
 
         # send signal that the generation stopped
         self.generation_stop(options)
 
     def _generate(self, subparser=None, start=None, parsers=None):
         # keep trace of the parsers generated by commands
@@ -120,15 +120,15 @@
         # loop over children
         for command in self.tree[start]:
             # create an instance of the command
             instance = self.commands[command]()
 
             # generate the list of parent parsers used by the command if
             # provided by the user
-            if hasattr(instance, "__parent_arguments__"):
+            if hasattr(instance, '__parent_arguments__'):
                 parents = [
                     self.parsers[name]
                     for name in instance.__parent_arguments__
                 ]
             else:
                 parents = []
 
@@ -184,20 +184,20 @@
         """
         # first check that the number of commands linked to the root that does
         # nothing is not greater than one. If it is not the case, several
         # parsers are defined and thus we are unable to define which one to
         # use.
         if len(self.tree[None]) > 1:
             logger.error(
-                "Multiple parsers are defined for the commands. Cannot " +
-                "decide which one to use."
+                'Multiple parsers are defined for the commands. Cannot ' +
+                'decide which one to use.'
             )
             raise SystemExit(-1)
         elif len(self.tree[None]) <= 0:
-            logger.error("No commands defined for the root command.")
+            logger.error('No commands defined for the root command.')
             raise SystemExit(-1)
 
         # else parse the root parser
         return self.parsers[self.tree[None][0]].parse_known_args(args=argv)
 
     def preprocess_args(self, argv):
         """
@@ -263,35 +263,35 @@
         use. Take as argument the subparser from the parent parser.
         """
         return subparser.add_parser(
             self.__command_name__,
             help=self.__help__,
             parents=parents,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-            conflict_handler="resolve",
+            conflict_handler='resolve',
         )
 
     def add_arguments(self, parser):
         """
         Used by the user to add arguments associated to the given parser.
         """
         pass
 
     def subparser(self, parser):
         """
         Should return a subparser for this command. Not always called, just
         when the command has possibly subcommands to generate.
         """
-        if hasattr(self, "__command_name__"):
+        if hasattr(self, '__command_name__'):
             command = self.__command_name__
         else:
             command = self.__command__
 
         return parser.add_subparsers(
-            help="Sub-commands available for command {0}".format(command),
+            help='Sub-commands available for command {0}'.format(command),
         )
 
     def has_children(self):
         """
         To know if the command has subcommands.
         """
         # check that the command has subcommands
@@ -336,21 +336,19 @@
         Used to add a parser with its options and be able to refer from a
         command, since the conflict handler of argparse is not well done, as
         many other things.
         """
         # check that the parser with this name is not already present
         if name in cls.manager.parsers:
             logger.error(
-                "Trying to add parser with name {0} while already defined"
+                'Trying to add parser with name {0} while already defined'
             )
             raise SystemExit(-1)
 
         # add the parser to the collection
         cls.manager.parsers[name] = parser
 
     def __repr__(self):
-        return "Command {0}".format(self.__command__)
+        return 'Command {0}'.format(self.__command__)
 
     def __str__(self):
         return self.__command__
-
-# vim: set tw=79 :
```

### Comparing `poppy-core-0.11.4/poppy/core/conf/__init__.py` & `poppy_core-0.11.5/poppy/core/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/conf/logger.json` & `poppy_core-0.11.5/poppy/core/conf/logger.json`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/configuration.py` & `poppy_core-0.11.5/poppy/core/configuration.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/db/connector.py` & `poppy_core-0.11.5/poppy/core/db/connector.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/db/database.py` & `poppy_core-0.11.5/poppy/core/db/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,14 +286,15 @@
             # Make sure that special characters are well passed in URL
             user, password = self.parameters['user'].split(':')
             port = self.parameters.get('port', None)
             if port:
                 address = self.parameters['address'] + ':' + port
             else:
                 address = self.parameters['address']
+
             return '{0}://{1}@{2}/{3}'.format(
                 vendor, quote_plus(user) + ':' + quote_plus(password),
                 address, self.parameters['database']
             )
 
     def generate_url_admin(self):
         """
```

### Comparing `poppy-core-0.11.4/poppy/core/db/dry_runner.py` & `poppy_core-0.11.5/poppy/core/db/dry_runner.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/db/handlers.py` & `poppy_core-0.11.5/poppy/core/db/handlers.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/db/non_null_column.py` & `poppy_core-0.11.5/poppy/core/db/non_null_column.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,20 +29,21 @@
         of sqlalchemy.Column.
         """
 
         self.descr = descr
         self.doc_comment = comment
         self.priority = None
 
-        self.sql_type = list(args).pop(0)
+        self.sql_type = kwargs.get('type_', None)
+        if self.sql_type is None:
+            self.sql_type = list(args).pop(0)
 
         if self.sql_type.__class__ == ENUM:
             self.sql_type = 'ENUM'
 
-
         try:
             if kwargs['primary_key']:
                 self.priority = 'PK'
         except KeyError:
             if nullable:
                 self.priority = 'N'
             else:
@@ -50,15 +51,14 @@
 
         if self.priority == 'PK':
             self.descr = 'Primary key'
 
         if unique:
             self.doc_comment = f'Must be unique. {self.doc_comment}'
 
-
         # if column is a foreign key, generate the corresponding description
         try:
             fk = list(args).pop(1)
             if fk.__class__ == ForeignKey:
                 column = fk._colspec.split('.')
                 self.descr = f'FK reference to {column[2]} in the {column[0]}.{column[1]} table'
         except IndexError:
@@ -86,9 +86,7 @@
         return {
             'name': f'{self.key}',
             'sql_type': f'{self.sql_type}',
             'description': f'{self.descr}',
             'priority': f'{self.priority}',
             'comment': f'{self.doc_comment}'
         }
-
-
```

### Comparing `poppy-core-0.11.4/poppy/core/generic/cache.py` & `poppy_core-0.11.5/poppy/core/generic/cache.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/generic/dot_dict.py` & `poppy_core-0.11.5/poppy/core/generic/dot_dict.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/generic/graph.py` & `poppy_core-0.11.5/poppy/core/generic/graph.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/generic/manager.py` & `poppy_core-0.11.5/poppy/core/generic/manager.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/generic/metaclasses.py` & `poppy_core-0.11.5/poppy/core/generic/metaclasses.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/generic/paths.py` & `poppy_core-0.11.5/poppy/core/generic/paths.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/generic/requests.py` & `poppy_core-0.11.5/poppy/core/generic/requests.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/generic/signals.py` & `poppy_core-0.11.5/poppy/core/generic/signals.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/generic/timer.py` & `poppy_core-0.11.5/poppy/core/generic/timer.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/loop.py` & `poppy_core-0.11.5/poppy/core/loop.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/management/commands.py` & `poppy_core-0.11.5/poppy/core/management/commands.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/management/templates/pipeline_template/config.json-tpl` & `poppy_core-0.11.5/poppy/core/management/templates/pipeline_template/config.json-tpl`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/management/templates/pipeline_template/descriptor.json-tpl` & `poppy_core-0.11.5/poppy/core/management/templates/pipeline_template/descriptor.json-tpl`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/management/templates/pipeline_template/manage.py` & `poppy_core-0.11.5/poppy/core/management/templates/pipeline_template/manage.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/management/templates/pipeline_template/settings.py-tpl` & `poppy_core-0.11.5/poppy/core/management/templates/pipeline_template/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/management/templates/plugin_template/README.rst-tpl` & `poppy_core-0.11.5/poppy/core/management/templates/plugin_template/README.rst-tpl`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/commands.py-tpl` & `poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/commands.py-tpl`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/descriptor.json-tpl` & `poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/descriptor.json-tpl`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/models/__init__.py-tpl` & `poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/models/__init__.py-tpl`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/tasks.py-tpl` & `poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/tasks.py-tpl`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/tests.py-tpl` & `poppy_core-0.11.5/poppy/core/management/templates/plugin_template/plugin_namespace/plugin_name/tests.py-tpl`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/management/templates/plugin_template/setup.py-tpl` & `poppy_core-0.11.5/poppy/core/management/templates/plugin_template/setup.py-tpl`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/pipeline.py` & `poppy_core-0.11.5/poppy/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/plugin.py` & `poppy_core-0.11.5/poppy/core/plugin.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/properties.py` & `poppy_core-0.11.5/poppy/core/properties.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/target/base_target.py` & `poppy_core-0.11.5/poppy/core/target/base_target.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/target/file_target.py` & `poppy_core-0.11.5/poppy/core/target/file_target.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/target/py_object_target.py` & `poppy_core-0.11.5/poppy/core/target/py_object_target.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/task/base_task.py` & `poppy_core-0.11.5/poppy/core/task/base_task.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/task/task.py` & `poppy_core-0.11.5/poppy/core/task/task.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/test.py` & `poppy_core-0.11.5/poppy/core/test.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/appdirs/LICENSE.txt` & `poppy_core-0.11.5/poppy/core/tools/appdirs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/appdirs/README.rst` & `poppy_core-0.11.5/poppy/core/tools/appdirs/README.rst`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/appdirs/appdirs.py` & `poppy_core-0.11.5/poppy/core/tools/appdirs/appdirs.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/cdf/cdf.py` & `poppy_core-0.11.5/poppy/core/tools/cdf/cdf.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/cdf/const.py` & `poppy_core-0.11.5/poppy/core/tools/cdf/const.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/exceptions.py` & `poppy_core-0.11.5/poppy/core/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/lock.py` & `poppy_core-0.11.5/poppy/core/tools/lock.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/poppy_argparse.py` & `poppy_core-0.11.5/poppy/core/tools/poppy_argparse.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/poppy_logging/TerminalColorFormatter.py` & `poppy_core-0.11.5/poppy/core/tools/poppy_logging/TerminalColorFormatter.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/poppy_logging/rotating_file_handler.py` & `poppy_core-0.11.5/poppy/core/tools/poppy_logging/rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/text.py` & `poppy_core-0.11.5/poppy/core/tools/text.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/xml.py` & `poppy_core-0.11.5/poppy/core/tools/xml.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/xmltodict/LICENSE.txt` & `poppy_core-0.11.5/poppy/core/tools/xmltodict/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/poppy/core/tools/xmltodict/xmltodict.py` & `poppy_core-0.11.5/poppy/core/tools/xmltodict/xmltodict.py`

 * *Files identical despite different names*

### Comparing `poppy-core-0.11.4/pyproject.toml` & `poppy_core-0.11.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 skip-string-normalization = true
 line-length = 79
 include = "\\.pyi?$"
 exclude = "/(\n    \\.git\n  | \\.hg\n  | \\.mypy_cache\n  | \\.tox\n  | \\.venv\n  | _build\n  | buck-out\n  | build\n  | dist\n)/\n"
 
 [tool.poetry]
 name = "poppy-core"
-version = "0.11.4"
+version = "0.11.5"
 readme = "README.md"
 license = "CeCILL-C"
 repository = "https://gitlab.obspm.fr/POPPy/POPPyCore"
 description = "POPPy: Plugin-Oriented Pipeline for Python"
-authors = [ "Xavier Bonnin <xavier.bonnin@obspm.fr>", "ROC Team <roc.support@sympa.obspm.fr>",]
+authors = [ "ROC Team <roc.support@sympa.obspm.fr>"]
 exclude = [ "bump_version.py",]
 [[tool.poetry.packages]]
 include = "poppy"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 psycopg2-binary = "^2.8.4"
```

### Comparing `poppy-core-0.11.4/PKG-INFO` & `poppy_core-0.11.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: poppy-core
-Version: 0.11.4
+Version: 0.11.5
 Summary: POPPy: Plugin-Oriented Pipeline for Python
 Home-page: https://gitlab.obspm.fr/POPPy/POPPyCore
 License: CECILL-C
-Author: Xavier Bonnin
-Author-email: xavier.bonnin@obspm.fr
+Author: ROC Team
+Author-email: roc.support@sympa.obspm.fr
 Requires-Python: >=3.8,<4
 Classifier: License :: CeCILL-C Free Software License Agreement (CECILL-C)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: SQLAlchemy (>=1.3,<2.0)
 Requires-Dist: alembic (>=1.4,<2.0)
 Requires-Dist: declic (>=1.0,<2.0)
 Requires-Dist: jsonschema (>=4.0,<5.0)
 Requires-Dist: psycopg2-binary (>=2.8.4,<3.0.0)
 Project-URL: Repository, https://gitlab.obspm.fr/POPPy/POPPyCore
 Description-Content-Type: text/markdown
```

