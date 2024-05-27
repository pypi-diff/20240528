# Comparing `tmp/zenaura-0.9.91.tar.gz` & `tmp/zenaura-0.9.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.91.tar", last modified: Mon May 27 22:10:08 2024, max compression
+gzip compressed data, was "zenaura-0.9.92.tar", last modified: Mon May 27 22:31:16 2024, max compression
```

## Comparing `zenaura-0.9.91.tar` & `zenaura-0.9.92.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.360395 zenaura-0.9.91/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.91/LICENSE
--rw-rw-rw-   0        0        0     2028 2024-05-27 22:10:08.359895 zenaura-0.9.91/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.91/README.md
--rw-rw-rw-   0        0        0       42 2024-05-27 22:10:08.360395 zenaura-0.9.91/setup.cfg
--rw-rw-rw-   0        0        0     1135 2024-05-27 22:07:41.000000 zenaura-0.9.91/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.320026 zenaura-0.9.91/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.91/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6595 2024-05-27 20:30:05.000000 zenaura-0.9.91/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.91/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.91/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.91/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.91/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.91/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.91/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0     1201 2024-05-27 20:12:21.000000 zenaura-0.9.91/tests/test_server.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.91/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.91/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.91/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.320526 zenaura-0.9.91/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-26 19:08:09.000000 zenaura-0.9.91/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.340008 zenaura-0.9.91/zenaura/client/
--rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.91/zenaura/client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.342583 zenaura-0.9.91/zenaura/client/algorithm/
--rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/algorithm/__init__.py
--rw-rw-rw-   0        0        0      193 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/algorithm/algorithm.py
--rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/algorithm/operations.py
--rw-rw-rw-   0        0        0     7166 2024-05-26 18:57:08.000000 zenaura-0.9.91/zenaura/client/algorithm/searcher.py
--rw-rw-rw-   0        0        0     2772 2024-05-26 18:57:08.000000 zenaura-0.9.91/zenaura/client/algorithm/updater.py
--rw-rw-rw-   0        0        0    10403 2024-05-27 22:09:46.000000 zenaura-0.9.91/zenaura/client/app.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.344083 zenaura-0.9.91/zenaura/client/compiler/
--rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/compiler/__init__.py
--rw-rw-rw-   0        0        0     1403 2024-05-26 18:57:08.000000 zenaura-0.9.91/zenaura/client/compiler/attribute.py
--rw-rw-rw-   0        0        0     3471 2024-05-26 18:57:08.000000 zenaura-0.9.91/zenaura/client/compiler/compiler.py
--rw-rw-rw-   0        0        0     1132 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/compiler/sanitize.py
--rw-rw-rw-   0        0        0     4093 2024-05-26 18:57:08.000000 zenaura-0.9.91/zenaura/client/component.py
--rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/config.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.347205 zenaura-0.9.91/zenaura/client/dom/
--rw-rw-rw-   0        0        0       43 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/dom/__init__.py
--rw-rw-rw-   0        0        0      280 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/dom/dom.py
--rw-rw-rw-   0        0        0     1803 2024-05-26 18:57:08.000000 zenaura-0.9.91/zenaura/client/dom/error.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.348204 zenaura-0.9.91/zenaura/client/dom/lifecycles/
--rw-rw-rw-   0        0        0      449 2024-05-27 19:25:39.000000 zenaura-0.9.91/zenaura/client/dom/lifecycles/mount.py
--rw-rw-rw-   0        0        0      804 2024-05-27 19:26:03.000000 zenaura-0.9.91/zenaura/client/dom/lifecycles/render.py
--rw-rw-rw-   0        0        0     1488 2024-05-27 19:25:23.000000 zenaura-0.9.91/zenaura/client/dom/mount.py
--rw-rw-rw-   0        0        0     1895 2024-05-27 20:46:41.000000 zenaura-0.9.91/zenaura/client/dom/render.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.351708 zenaura-0.9.91/zenaura/client/hydrator/
--rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/hydrator/__init__.py
--rw-rw-rw-   0        0        0     1895 2024-05-26 18:57:08.000000 zenaura-0.9.91/zenaura/client/hydrator/compiler_adapter.py
--rw-rw-rw-   0        0        0     1236 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/hydrator/hydrator.py
--rw-rw-rw-   0        0        0     1346 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/hydrator/lookup.py
--rw-rw-rw-   0        0        0     7033 2024-05-27 22:07:22.000000 zenaura-0.9.91/zenaura/client/hydrator/real_dom_adapter.py
--rw-rw-rw-   0        0        0     2264 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/hydrator/tasker.py
--rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.91/zenaura/client/hydrator/virtual_dom_adapter.py
--rw-rw-rw-   0        0        0     2631 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/mocks.py
--rw-rw-rw-   0        0        0      896 2024-05-26 18:57:08.000000 zenaura-0.9.91/zenaura/client/mutator.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.353917 zenaura-0.9.91/zenaura/client/observer/
--rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/observer/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/observer/observer.py
--rw-rw-rw-   0        0        0     1609 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/observer/subject.py
--rw-rw-rw-   0        0        0     2009 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/observer.py
--rw-rw-rw-   0        0        0      735 2024-05-27 20:29:15.000000 zenaura-0.9.91/zenaura/client/page.py
--rw-rw-rw-   0        0        0     2212 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/persistance.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.356917 zenaura-0.9.91/zenaura/client/tags/
--rw-rw-rw-   0        0        0      165 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/tags/__init__.py
--rw-rw-rw-   0        0        0      429 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/tags/attribute.py
--rw-rw-rw-   0        0        0     4666 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/tags/builder.py
--rw-rw-rw-   0        0        0      418 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/tags/data.py
--rw-rw-rw-   0        0        0      473 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/tags/html.py
--rw-rw-rw-   0        0        0    10231 2024-05-26 17:44:57.000000 zenaura-0.9.91/zenaura/client/tags/node.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.358417 zenaura-0.9.91/zenaura/server/
--rw-rw-rw-   0        0        0       33 2024-05-26 19:08:17.000000 zenaura-0.9.91/zenaura/server/__init__.py
--rw-rw-rw-   0        0        0     3294 2024-05-27 21:23:25.000000 zenaura-0.9.91/zenaura/server/server.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:10:08.358417 zenaura-0.9.91/zenaura.egg-info/
--rw-rw-rw-   0        0        0     2028 2024-05-27 22:10:08.000000 zenaura-0.9.91/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1888 2024-05-27 22:10:08.000000 zenaura-0.9.91/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 22:10:08.000000 zenaura-0.9.91/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-27 22:10:08.000000 zenaura-0.9.91/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-27 22:10:08.000000 zenaura-0.9.91/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.058856 zenaura-0.9.92/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.92/LICENSE
+-rw-rw-rw-   0        0        0     2028 2024-05-27 22:31:16.058356 zenaura-0.9.92/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.92/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 22:31:16.059357 zenaura-0.9.92/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2024-05-27 22:29:39.000000 zenaura-0.9.92/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.025857 zenaura-0.9.92/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.92/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6595 2024-05-27 20:30:05.000000 zenaura-0.9.92/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.92/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.92/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.92/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.92/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.92/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.92/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0     1201 2024-05-27 20:12:21.000000 zenaura-0.9.92/tests/test_server.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.92/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.92/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.92/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.026357 zenaura-0.9.92/zenaura/
+-rw-rw-rw-   0        0        0        0 2024-05-26 19:08:09.000000 zenaura-0.9.92/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.034856 zenaura-0.9.92/zenaura/client/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.92/zenaura/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.037358 zenaura-0.9.92/zenaura/client/algorithm/
+-rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/algorithm/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/algorithm/algorithm.py
+-rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/algorithm/operations.py
+-rw-rw-rw-   0        0        0     7166 2024-05-26 18:57:08.000000 zenaura-0.9.92/zenaura/client/algorithm/searcher.py
+-rw-rw-rw-   0        0        0     2772 2024-05-26 18:57:08.000000 zenaura-0.9.92/zenaura/client/algorithm/updater.py
+-rw-rw-rw-   0        0        0    10403 2024-05-27 22:09:46.000000 zenaura-0.9.92/zenaura/client/app.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.039357 zenaura-0.9.92/zenaura/client/compiler/
+-rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/compiler/__init__.py
+-rw-rw-rw-   0        0        0     1403 2024-05-26 18:57:08.000000 zenaura-0.9.92/zenaura/client/compiler/attribute.py
+-rw-rw-rw-   0        0        0     3471 2024-05-26 18:57:08.000000 zenaura-0.9.92/zenaura/client/compiler/compiler.py
+-rw-rw-rw-   0        0        0     1132 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/compiler/sanitize.py
+-rw-rw-rw-   0        0        0     4093 2024-05-26 18:57:08.000000 zenaura-0.9.92/zenaura/client/component.py
+-rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/config.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.042358 zenaura-0.9.92/zenaura/client/dom/
+-rw-rw-rw-   0        0        0       43 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/dom/__init__.py
+-rw-rw-rw-   0        0        0      280 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/dom/dom.py
+-rw-rw-rw-   0        0        0     1803 2024-05-26 18:57:08.000000 zenaura-0.9.92/zenaura/client/dom/error.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.043357 zenaura-0.9.92/zenaura/client/dom/lifecycles/
+-rw-rw-rw-   0        0        0      449 2024-05-27 19:25:39.000000 zenaura-0.9.92/zenaura/client/dom/lifecycles/mount.py
+-rw-rw-rw-   0        0        0      804 2024-05-27 19:26:03.000000 zenaura-0.9.92/zenaura/client/dom/lifecycles/render.py
+-rw-rw-rw-   0        0        0     1488 2024-05-27 19:25:23.000000 zenaura-0.9.92/zenaura/client/dom/mount.py
+-rw-rw-rw-   0        0        0     1895 2024-05-27 20:46:41.000000 zenaura-0.9.92/zenaura/client/dom/render.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.048857 zenaura-0.9.92/zenaura/client/hydrator/
+-rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/hydrator/__init__.py
+-rw-rw-rw-   0        0        0     1895 2024-05-26 18:57:08.000000 zenaura-0.9.92/zenaura/client/hydrator/compiler_adapter.py
+-rw-rw-rw-   0        0        0     1236 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/hydrator/hydrator.py
+-rw-rw-rw-   0        0        0     1346 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/hydrator/lookup.py
+-rw-rw-rw-   0        0        0     7033 2024-05-27 22:07:22.000000 zenaura-0.9.92/zenaura/client/hydrator/real_dom_adapter.py
+-rw-rw-rw-   0        0        0     2264 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/hydrator/tasker.py
+-rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.92/zenaura/client/hydrator/virtual_dom_adapter.py
+-rw-rw-rw-   0        0        0     2631 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/mocks.py
+-rw-rw-rw-   0        0        0      896 2024-05-26 18:57:08.000000 zenaura-0.9.92/zenaura/client/mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.051358 zenaura-0.9.92/zenaura/client/observer/
+-rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/observer/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/observer/observer.py
+-rw-rw-rw-   0        0        0     1609 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/observer/subject.py
+-rw-rw-rw-   0        0        0     2009 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/observer.py
+-rw-rw-rw-   0        0        0      735 2024-05-27 20:29:15.000000 zenaura-0.9.92/zenaura/client/page.py
+-rw-rw-rw-   0        0        0     2212 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/persistance.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.055858 zenaura-0.9.92/zenaura/client/tags/
+-rw-rw-rw-   0        0        0      165 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/tags/__init__.py
+-rw-rw-rw-   0        0        0      429 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/tags/attribute.py
+-rw-rw-rw-   0        0        0     4666 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/tags/builder.py
+-rw-rw-rw-   0        0        0      418 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/tags/data.py
+-rw-rw-rw-   0        0        0      473 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/tags/html.py
+-rw-rw-rw-   0        0        0    10231 2024-05-26 17:44:57.000000 zenaura-0.9.92/zenaura/client/tags/node.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.057357 zenaura-0.9.92/zenaura/server/
+-rw-rw-rw-   0        0        0       33 2024-05-26 19:08:17.000000 zenaura-0.9.92/zenaura/server/__init__.py
+-rw-rw-rw-   0        0        0     3292 2024-05-27 22:29:34.000000 zenaura-0.9.92/zenaura/server/server.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:31:16.057857 zenaura-0.9.92/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     2028 2024-05-27 22:31:15.000000 zenaura-0.9.92/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1888 2024-05-27 22:31:16.000000 zenaura-0.9.92/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 22:31:15.000000 zenaura-0.9.92/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-27 22:31:15.000000 zenaura-0.9.92/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 22:31:15.000000 zenaura-0.9.92/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.91/LICENSE` & `zenaura-0.9.92/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/PKG-INFO` & `zenaura-0.9.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.91
+Version: 0.9.92
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.91/README.md` & `zenaura-0.9.92/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/setup.py` & `zenaura-0.9.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.91',
+    version='0.9.92',
     description="Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
     packages=['zenaura', 'zenaura.server', 'zenaura.client', 'zenaura.client.algorithm', 'zenaura.client.compiler', 'zenaura.client.hydrator', 'zenaura.client.observer', 'zenaura.client.tags', 'zenaura.client.dom', 'zenaura.client.dom.lifecycles'],
     install_requires=[
         'bleach'
     ],
```

### Comparing `zenaura-0.9.91/tests/test_algorithm.py` & `zenaura-0.9.92/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/tests/test_app.py` & `zenaura-0.9.92/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/tests/test_compiler.py` & `zenaura-0.9.92/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/tests/test_component_e2e.py` & `zenaura-0.9.92/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/tests/test_component_unit.py` & `zenaura-0.9.92/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/tests/test_node_properties.py` & `zenaura-0.9.92/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/tests/test_observer.py` & `zenaura-0.9.92/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/tests/test_rdom_adapter.py` & `zenaura-0.9.92/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/tests/test_server.py` & `zenaura-0.9.92/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/tests/test_tags.py` & `zenaura-0.9.92/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/tests/test_tasker.py` & `zenaura-0.9.92/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/tests/test_zenaura_dom.py` & `zenaura-0.9.92/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/algorithm/operations.py` & `zenaura-0.9.92/zenaura/client/algorithm/operations.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/algorithm/searcher.py` & `zenaura-0.9.92/zenaura/client/algorithm/searcher.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/algorithm/updater.py` & `zenaura-0.9.92/zenaura/client/algorithm/updater.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/app.py` & `zenaura-0.9.92/zenaura/client/app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/compiler/attribute.py` & `zenaura-0.9.92/zenaura/client/compiler/attribute.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/compiler/compiler.py` & `zenaura-0.9.92/zenaura/client/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/compiler/sanitize.py` & `zenaura-0.9.92/zenaura/client/compiler/sanitize.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/component.py` & `zenaura-0.9.92/zenaura/client/component.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/config.py` & `zenaura-0.9.92/zenaura/client/config.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/dom/error.py` & `zenaura-0.9.92/zenaura/client/dom/error.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/dom/lifecycles/render.py` & `zenaura-0.9.92/zenaura/client/dom/lifecycles/render.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/dom/mount.py` & `zenaura-0.9.92/zenaura/client/dom/mount.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/dom/render.py` & `zenaura-0.9.92/zenaura/client/dom/render.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/hydrator/compiler_adapter.py` & `zenaura-0.9.92/zenaura/client/hydrator/compiler_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/hydrator/hydrator.py` & `zenaura-0.9.92/zenaura/client/hydrator/hydrator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/hydrator/lookup.py` & `zenaura-0.9.92/zenaura/client/hydrator/lookup.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/hydrator/real_dom_adapter.py` & `zenaura-0.9.92/zenaura/client/hydrator/real_dom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/hydrator/tasker.py` & `zenaura-0.9.92/zenaura/client/hydrator/tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/hydrator/virtual_dom_adapter.py` & `zenaura-0.9.92/zenaura/client/hydrator/virtual_dom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/mocks.py` & `zenaura-0.9.92/zenaura/client/mocks.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/mutator.py` & `zenaura-0.9.92/zenaura/client/mutator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/observer/subject.py` & `zenaura-0.9.92/zenaura/client/observer/subject.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/observer.py` & `zenaura-0.9.92/zenaura/client/observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/page.py` & `zenaura-0.9.92/zenaura/client/page.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/persistance.py` & `zenaura-0.9.92/zenaura/client/persistance.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/tags/builder.py` & `zenaura-0.9.92/zenaura/client/tags/builder.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/client/tags/node.py` & `zenaura-0.9.92/zenaura/client/tags/node.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.91/zenaura/server/server.py` & `zenaura-0.9.92/zenaura/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
           icon: favorite.ico
           pydide : is pydide build script url.
       """
       pages = io.StringIO()
 
       # render pages 
       for path, route in app.routes.items():
-          page, _, path, ssr = route 
+          page, _, _ , ssr = route 
           if ssr: # ignore SSR pages
               continue 
           if path == "/" : # set / route to visible 
               page_div = lambda comps : f'<div data-zenaura="{page.id}">{comps}</div>'
               pages.write(page_div(compiler_adapter.hyd_comp_compile_page(page)))
               continue
           # pages other than / are set to hidden
```

#### html2text {}

```diff
@@ -14,16 +14,16 @@
 (page),meta_description, title, icon, pydide) @staticmethod def hydrate_app(app
 :App, title="zenaura", meta_description="this app created with zenaura",
 icon="./public/favicon.ico", pydide="https://pyscript.net/releases/2024.1.1/
 core.js"): """ render pages on app run, set page with path / to visible, rest
 to hidden then compile index.html on server run. params : app - zenaura app.
 title - html meta tag for title text meta_description : html meta description
 for website icon: favorite.ico pydide : is pydide build script url. """ pages =
-io.StringIO() # render pages for path, route in app.routes.items(): page, _,
-path, ssr = route if ssr: # ignore SSR pages continue if path == "/" : # set /
+io.StringIO() # render pages for path, route in app.routes.items(): page, _, _
+, ssr = route if ssr: # ignore SSR pages continue if path == "/" : # set /
 route to visible page_div = lambda comps : f'
 {comps}
 ' pages.write(page_div(compiler_adapter.hyd_comp_compile_page(page))) continue
 # pages other than / are set to hidden page_div = lambda comps : f'
 {comps}
 ' pages.write(page_div(compiler_adapter.hyd_comp_compile_page(page))) pages =
 pages.getvalue() # overwrite in public dir with open("./public/index.html",
```

### Comparing `zenaura-0.9.91/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.92/zenaura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.91
+Version: 0.9.92
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.91/zenaura.egg-info/SOURCES.txt` & `zenaura-0.9.92/zenaura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

