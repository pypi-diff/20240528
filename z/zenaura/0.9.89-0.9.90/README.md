# Comparing `tmp/zenaura-0.9.89.tar.gz` & `tmp/zenaura-0.9.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.89.tar", last modified: Mon May 27 20:30:38 2024, max compression
+gzip compressed data, was "zenaura-0.9.90.tar", last modified: Mon May 27 20:49:47 2024, max compression
```

## Comparing `zenaura-0.9.89.tar` & `zenaura-0.9.90.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.834869 zenaura-0.9.89/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.89/LICENSE
--rw-rw-rw-   0        0        0     2028 2024-05-27 20:30:38.834369 zenaura-0.9.89/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.89/README.md
--rw-rw-rw-   0        0        0       42 2024-05-27 20:30:38.834869 zenaura-0.9.89/setup.cfg
--rw-rw-rw-   0        0        0     1135 2024-05-27 20:30:14.000000 zenaura-0.9.89/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.807349 zenaura-0.9.89/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.89/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6595 2024-05-27 20:30:05.000000 zenaura-0.9.89/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.89/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.89/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.89/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.89/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.89/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.89/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0     1201 2024-05-27 20:12:21.000000 zenaura-0.9.89/tests/test_server.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.89/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.89/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.89/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.808353 zenaura-0.9.89/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-26 19:08:09.000000 zenaura-0.9.89/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.816858 zenaura-0.9.89/zenaura/client/
--rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.89/zenaura/client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.819363 zenaura-0.9.89/zenaura/client/algorithm/
--rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/algorithm/__init__.py
--rw-rw-rw-   0        0        0      193 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/algorithm/algorithm.py
--rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/algorithm/operations.py
--rw-rw-rw-   0        0        0     7166 2024-05-26 18:57:08.000000 zenaura-0.9.89/zenaura/client/algorithm/searcher.py
--rw-rw-rw-   0        0        0     2772 2024-05-26 18:57:08.000000 zenaura-0.9.89/zenaura/client/algorithm/updater.py
--rw-rw-rw-   0        0        0    10263 2024-05-27 19:32:29.000000 zenaura-0.9.89/zenaura/client/app.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.821362 zenaura-0.9.89/zenaura/client/compiler/
--rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/compiler/__init__.py
--rw-rw-rw-   0        0        0     1403 2024-05-26 18:57:08.000000 zenaura-0.9.89/zenaura/client/compiler/attribute.py
--rw-rw-rw-   0        0        0     3471 2024-05-26 18:57:08.000000 zenaura-0.9.89/zenaura/client/compiler/compiler.py
--rw-rw-rw-   0        0        0     1132 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/compiler/sanitize.py
--rw-rw-rw-   0        0        0     4093 2024-05-26 18:57:08.000000 zenaura-0.9.89/zenaura/client/component.py
--rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/config.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.823362 zenaura-0.9.89/zenaura/client/dom/
--rw-rw-rw-   0        0        0       43 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/dom/__init__.py
--rw-rw-rw-   0        0        0      280 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/dom/dom.py
--rw-rw-rw-   0        0        0     1803 2024-05-26 18:57:08.000000 zenaura-0.9.89/zenaura/client/dom/error.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.824863 zenaura-0.9.89/zenaura/client/dom/lifecycles/
--rw-rw-rw-   0        0        0      449 2024-05-27 19:25:39.000000 zenaura-0.9.89/zenaura/client/dom/lifecycles/mount.py
--rw-rw-rw-   0        0        0      804 2024-05-27 19:26:03.000000 zenaura-0.9.89/zenaura/client/dom/lifecycles/render.py
--rw-rw-rw-   0        0        0     1488 2024-05-27 19:25:23.000000 zenaura-0.9.89/zenaura/client/dom/mount.py
--rw-rw-rw-   0        0        0     1883 2024-05-26 21:17:10.000000 zenaura-0.9.89/zenaura/client/dom/render.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.828366 zenaura-0.9.89/zenaura/client/hydrator/
--rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/hydrator/__init__.py
--rw-rw-rw-   0        0        0     1895 2024-05-26 18:57:08.000000 zenaura-0.9.89/zenaura/client/hydrator/compiler_adapter.py
--rw-rw-rw-   0        0        0     1236 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/hydrator/hydrator.py
--rw-rw-rw-   0        0        0     1346 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/hydrator/lookup.py
--rw-rw-rw-   0        0        0     7089 2024-05-27 19:20:18.000000 zenaura-0.9.89/zenaura/client/hydrator/real_dom_adapter.py
--rw-rw-rw-   0        0        0     2264 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/hydrator/tasker.py
--rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.89/zenaura/client/hydrator/virtual_dom_adapter.py
--rw-rw-rw-   0        0        0     2631 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/mocks.py
--rw-rw-rw-   0        0        0      896 2024-05-26 18:57:08.000000 zenaura-0.9.89/zenaura/client/mutator.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.829369 zenaura-0.9.89/zenaura/client/observer/
--rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/observer/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/observer/observer.py
--rw-rw-rw-   0        0        0     1609 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/observer/subject.py
--rw-rw-rw-   0        0        0     2009 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/observer.py
--rw-rw-rw-   0        0        0      735 2024-05-27 20:29:15.000000 zenaura-0.9.89/zenaura/client/page.py
--rw-rw-rw-   0        0        0     2212 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/persistance.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.832370 zenaura-0.9.89/zenaura/client/tags/
--rw-rw-rw-   0        0        0      165 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/tags/__init__.py
--rw-rw-rw-   0        0        0      429 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/tags/attribute.py
--rw-rw-rw-   0        0        0     4666 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/tags/builder.py
--rw-rw-rw-   0        0        0      418 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/tags/data.py
--rw-rw-rw-   0        0        0      473 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/tags/html.py
--rw-rw-rw-   0        0        0    10231 2024-05-26 17:44:57.000000 zenaura-0.9.89/zenaura/client/tags/node.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.833370 zenaura-0.9.89/zenaura/server/
--rw-rw-rw-   0        0        0       33 2024-05-26 19:08:17.000000 zenaura-0.9.89/zenaura/server/__init__.py
--rw-rw-rw-   0        0        0     3316 2024-05-27 20:10:51.000000 zenaura-0.9.89/zenaura/server/server.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:30:38.833869 zenaura-0.9.89/zenaura.egg-info/
--rw-rw-rw-   0        0        0     2028 2024-05-27 20:30:38.000000 zenaura-0.9.89/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1888 2024-05-27 20:30:38.000000 zenaura-0.9.89/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 20:30:38.000000 zenaura-0.9.89/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-27 20:30:38.000000 zenaura-0.9.89/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-27 20:30:38.000000 zenaura-0.9.89/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.468117 zenaura-0.9.90/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.90/LICENSE
+-rw-rw-rw-   0        0        0     2028 2024-05-27 20:49:47.467116 zenaura-0.9.90/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.90/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 20:49:47.468117 zenaura-0.9.90/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2024-05-27 20:49:10.000000 zenaura-0.9.90/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.430661 zenaura-0.9.90/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.90/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6595 2024-05-27 20:30:05.000000 zenaura-0.9.90/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.90/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.90/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.90/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.90/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.90/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.90/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0     1201 2024-05-27 20:12:21.000000 zenaura-0.9.90/tests/test_server.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.90/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.90/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.90/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.431162 zenaura-0.9.90/zenaura/
+-rw-rw-rw-   0        0        0        0 2024-05-26 19:08:09.000000 zenaura-0.9.90/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.446165 zenaura-0.9.90/zenaura/client/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.90/zenaura/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.448956 zenaura-0.9.90/zenaura/client/algorithm/
+-rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/algorithm/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/algorithm/algorithm.py
+-rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/algorithm/operations.py
+-rw-rw-rw-   0        0        0     7166 2024-05-26 18:57:08.000000 zenaura-0.9.90/zenaura/client/algorithm/searcher.py
+-rw-rw-rw-   0        0        0     2772 2024-05-26 18:57:08.000000 zenaura-0.9.90/zenaura/client/algorithm/updater.py
+-rw-rw-rw-   0        0        0    10334 2024-05-27 20:43:18.000000 zenaura-0.9.90/zenaura/client/app.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.450960 zenaura-0.9.90/zenaura/client/compiler/
+-rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/compiler/__init__.py
+-rw-rw-rw-   0        0        0     1403 2024-05-26 18:57:08.000000 zenaura-0.9.90/zenaura/client/compiler/attribute.py
+-rw-rw-rw-   0        0        0     3471 2024-05-26 18:57:08.000000 zenaura-0.9.90/zenaura/client/compiler/compiler.py
+-rw-rw-rw-   0        0        0     1132 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/compiler/sanitize.py
+-rw-rw-rw-   0        0        0     4093 2024-05-26 18:57:08.000000 zenaura-0.9.90/zenaura/client/component.py
+-rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/config.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.454460 zenaura-0.9.90/zenaura/client/dom/
+-rw-rw-rw-   0        0        0       43 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/dom/__init__.py
+-rw-rw-rw-   0        0        0      280 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/dom/dom.py
+-rw-rw-rw-   0        0        0     1803 2024-05-26 18:57:08.000000 zenaura-0.9.90/zenaura/client/dom/error.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.455460 zenaura-0.9.90/zenaura/client/dom/lifecycles/
+-rw-rw-rw-   0        0        0      449 2024-05-27 19:25:39.000000 zenaura-0.9.90/zenaura/client/dom/lifecycles/mount.py
+-rw-rw-rw-   0        0        0      804 2024-05-27 19:26:03.000000 zenaura-0.9.90/zenaura/client/dom/lifecycles/render.py
+-rw-rw-rw-   0        0        0     1488 2024-05-27 19:25:23.000000 zenaura-0.9.90/zenaura/client/dom/mount.py
+-rw-rw-rw-   0        0        0     1895 2024-05-27 20:46:41.000000 zenaura-0.9.90/zenaura/client/dom/render.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.460465 zenaura-0.9.90/zenaura/client/hydrator/
+-rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/hydrator/__init__.py
+-rw-rw-rw-   0        0        0     1895 2024-05-26 18:57:08.000000 zenaura-0.9.90/zenaura/client/hydrator/compiler_adapter.py
+-rw-rw-rw-   0        0        0     1236 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/hydrator/hydrator.py
+-rw-rw-rw-   0        0        0     1346 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/hydrator/lookup.py
+-rw-rw-rw-   0        0        0     7085 2024-05-27 20:48:57.000000 zenaura-0.9.90/zenaura/client/hydrator/real_dom_adapter.py
+-rw-rw-rw-   0        0        0     2264 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/hydrator/tasker.py
+-rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.90/zenaura/client/hydrator/virtual_dom_adapter.py
+-rw-rw-rw-   0        0        0     2631 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/mocks.py
+-rw-rw-rw-   0        0        0      896 2024-05-26 18:57:08.000000 zenaura-0.9.90/zenaura/client/mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.461618 zenaura-0.9.90/zenaura/client/observer/
+-rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/observer/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/observer/observer.py
+-rw-rw-rw-   0        0        0     1609 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/observer/subject.py
+-rw-rw-rw-   0        0        0     2009 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/observer.py
+-rw-rw-rw-   0        0        0      735 2024-05-27 20:29:15.000000 zenaura-0.9.90/zenaura/client/page.py
+-rw-rw-rw-   0        0        0     2212 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/persistance.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.465617 zenaura-0.9.90/zenaura/client/tags/
+-rw-rw-rw-   0        0        0      165 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/tags/__init__.py
+-rw-rw-rw-   0        0        0      429 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/tags/attribute.py
+-rw-rw-rw-   0        0        0     4666 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/tags/builder.py
+-rw-rw-rw-   0        0        0      418 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/tags/data.py
+-rw-rw-rw-   0        0        0      473 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/tags/html.py
+-rw-rw-rw-   0        0        0    10231 2024-05-26 17:44:57.000000 zenaura-0.9.90/zenaura/client/tags/node.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.466117 zenaura-0.9.90/zenaura/server/
+-rw-rw-rw-   0        0        0       33 2024-05-26 19:08:17.000000 zenaura-0.9.90/zenaura/server/__init__.py
+-rw-rw-rw-   0        0        0     3316 2024-05-27 20:10:51.000000 zenaura-0.9.90/zenaura/server/server.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:49:47.466616 zenaura-0.9.90/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     2028 2024-05-27 20:49:47.000000 zenaura-0.9.90/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1888 2024-05-27 20:49:47.000000 zenaura-0.9.90/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 20:49:47.000000 zenaura-0.9.90/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-27 20:49:47.000000 zenaura-0.9.90/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 20:49:47.000000 zenaura-0.9.90/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.89/LICENSE` & `zenaura-0.9.90/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/PKG-INFO` & `zenaura-0.9.90/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.89
+Version: 0.9.90
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.89/README.md` & `zenaura-0.9.90/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/setup.py` & `zenaura-0.9.90/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.89',
+    version='0.9.90',
     description="Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
     packages=['zenaura', 'zenaura.server', 'zenaura.client', 'zenaura.client.algorithm', 'zenaura.client.compiler', 'zenaura.client.hydrator', 'zenaura.client.observer', 'zenaura.client.tags', 'zenaura.client.dom', 'zenaura.client.dom.lifecycles'],
     install_requires=[
         'bleach'
     ],
```

### Comparing `zenaura-0.9.89/tests/test_algorithm.py` & `zenaura-0.9.90/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/tests/test_app.py` & `zenaura-0.9.90/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/tests/test_compiler.py` & `zenaura-0.9.90/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/tests/test_component_e2e.py` & `zenaura-0.9.90/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/tests/test_component_unit.py` & `zenaura-0.9.90/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/tests/test_node_properties.py` & `zenaura-0.9.90/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/tests/test_observer.py` & `zenaura-0.9.90/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/tests/test_rdom_adapter.py` & `zenaura-0.9.90/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/tests/test_server.py` & `zenaura-0.9.90/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/tests/test_tags.py` & `zenaura-0.9.90/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/tests/test_tasker.py` & `zenaura-0.9.90/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/tests/test_zenaura_dom.py` & `zenaura-0.9.90/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/algorithm/operations.py` & `zenaura-0.9.90/zenaura/client/algorithm/operations.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/algorithm/searcher.py` & `zenaura-0.9.90/zenaura/client/algorithm/searcher.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/algorithm/updater.py` & `zenaura-0.9.90/zenaura/client/algorithm/updater.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/app.py` & `zenaura-0.9.90/zenaura/client/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,16 @@
             await self.not_found()
             return
         [page, title, middleware, ssr] = self.routes[path]
         window.history.pushState(path, title, path) # Update browser history
         if callable(middleware):
             await middleware()
         if not ssr: # ignore mount step for server side rendering pages.
-            rdom_hyd.hyd_rdom_toggle_pages_visibilty(page, self.history.current.page)
+            if not self.history.current.page: # self.history.current is intially Nonde
+                rdom_hyd.hyd_rdom_toggle_pages_visibilty(page, page)
             await zenaura_dom.mount(page)  # trigger attached lifecycle for each component within the page.
         else: # trigger attached lifecycle method for the component.
             await zenaura_dom.mount(page)
         # TODO handle ssr in mount. 
         self.history.visit(page)
         document.title = title
```

### Comparing `zenaura-0.9.89/zenaura/client/compiler/attribute.py` & `zenaura-0.9.90/zenaura/client/compiler/attribute.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/compiler/compiler.py` & `zenaura-0.9.90/zenaura/client/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/compiler/sanitize.py` & `zenaura-0.9.90/zenaura/client/compiler/sanitize.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/component.py` & `zenaura-0.9.90/zenaura/client/component.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/config.py` & `zenaura-0.9.90/zenaura/client/config.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/dom/error.py` & `zenaura-0.9.90/zenaura/client/dom/error.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/dom/lifecycles/render.py` & `zenaura-0.9.90/zenaura/client/dom/lifecycles/render.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/dom/mount.py` & `zenaura-0.9.90/zenaura/client/dom/mount.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/dom/render.py` & `zenaura-0.9.90/zenaura/client/dom/render.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             Returns:
             None
         """
         try:
 
             # update steps 1-3: on_mutation -> update -> on_settled
             # update 1: lifecycle method to be called before updating
-            self.on_mutation(comp)
+            await self.on_mutation(comp)
             comp_id = comp.id            
             prev_tree = self.zen_dom_table[comp_id]
             new_tree = comp.render()
 
             # create task queue for component
             task_que = self.hyd_tsk_get_or_create_task_queue(comp_id)
 
@@ -45,11 +45,11 @@
                     task = self.hyd_tsk_dequeue_task(comp_id)
                     await task()
 
                 
             self.hyd_vdom_update(comp)
 
             # update 3  : on_settled method to be called after updating
-            self.on_settled(comp)
+            await self.on_settled(comp)
 
         except Exception as e:
             self.componentDidCatchError(comp, traceback.format_exc())
```

### Comparing `zenaura-0.9.89/zenaura/client/hydrator/compiler_adapter.py` & `zenaura-0.9.90/zenaura/client/hydrator/compiler_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/hydrator/hydrator.py` & `zenaura-0.9.90/zenaura/client/hydrator/hydrator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/hydrator/lookup.py` & `zenaura-0.9.90/zenaura/client/hydrator/lookup.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/hydrator/real_dom_adapter.py` & `zenaura-0.9.90/zenaura/client/hydrator/real_dom_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,11 +177,11 @@
             if document.readyState=="complete":
                 break
         
 
     def hyd_rdom_toggle_pages_visibilty(self, current_page : Page , previous_page : Page):
         p_page = document.querySelector(f'[{ZENAURA_DOM_ATTRIBUTE}="{previous_page.id}"]')
         if p_page:
-            p_page.setAttribute("hidden", "true")
+            p_page.setAttribute("hidden", True)
         curr_page = document.querySelector(f'[{ZENAURA_DOM_ATTRIBUTE}="{current_page.id}"]')
         if curr_page:
-            curr_page.setAttribute("hidden", "false") # Update the title
+            curr_page.setAttribute("hidden", False) # Update the title
```

### Comparing `zenaura-0.9.89/zenaura/client/hydrator/tasker.py` & `zenaura-0.9.90/zenaura/client/hydrator/tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/hydrator/virtual_dom_adapter.py` & `zenaura-0.9.90/zenaura/client/hydrator/virtual_dom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/mocks.py` & `zenaura-0.9.90/zenaura/client/mocks.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/mutator.py` & `zenaura-0.9.90/zenaura/client/mutator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/observer/subject.py` & `zenaura-0.9.90/zenaura/client/observer/subject.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/observer.py` & `zenaura-0.9.90/zenaura/client/observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/page.py` & `zenaura-0.9.90/zenaura/client/page.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/persistance.py` & `zenaura-0.9.90/zenaura/client/persistance.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/tags/builder.py` & `zenaura-0.9.90/zenaura/client/tags/builder.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/client/tags/node.py` & `zenaura-0.9.90/zenaura/client/tags/node.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura/server/server.py` & `zenaura-0.9.90/zenaura/server/server.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.89/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.90/zenaura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.89
+Version: 0.9.90
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.89/zenaura.egg-info/SOURCES.txt` & `zenaura-0.9.90/zenaura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

