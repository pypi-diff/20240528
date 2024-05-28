# Comparing `tmp/cobib-5.0.1.tar.gz` & `tmp/cobib-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobib-5.0.1.tar", last modified: Wed May  1 13:46:22 2024, max compression
+gzip compressed data, was "cobib-5.1.0.tar", last modified: Tue May 28 18:15:39 2024, max compression
```

## Comparing `cobib-5.0.1.tar` & `cobib-5.1.0.tar`

### file list

```diff
@@ -1,97 +1,99 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.433230 cobib-5.0.1/
--rw-r--r--   0 max       (1000) max       (1000)    42185 2024-05-01 13:44:24.000000 cobib-5.0.1/CHANGELOG.md
--rw-r--r--   0 max       (1000) max       (1000)     1076 2024-01-18 21:03:08.000000 cobib-5.0.1/LICENSE.txt
--rw-r--r--   0 max       (1000) max       (1000)      100 2023-06-12 19:22:05.000000 cobib-5.0.1/MANIFEST.in
--rw-r--r--   0 max       (1000) max       (1000)    51602 2024-05-01 13:46:22.433230 cobib-5.0.1/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     8035 2024-03-17 16:27:49.000000 cobib-5.0.1/README.md
--rw-r--r--   0 max       (1000) max       (1000)    35143 2024-05-01 13:43:45.000000 cobib-5.0.1/cobib.1
--rw-r--r--   0 max       (1000) max       (1000)     4580 2024-04-28 11:19:47.000000 cobib-5.0.1/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)      135 2024-02-03 16:58:09.000000 cobib-5.0.1/requirements.txt
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-01 13:46:22.436564 cobib-5.0.1/setup.cfg
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.399897 cobib-5.0.1/src/
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.403231 cobib-5.0.1/src/cobib/
--rw-r--r--   0 max       (1000) max       (1000)      474 2024-05-01 13:43:53.000000 cobib-5.0.1/src/cobib/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      445 2024-03-17 16:27:49.000000 cobib-5.0.1/src/cobib/__main__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.413231 cobib-5.0.1/src/cobib/commands/
--rw-r--r--   0 max       (1000) max       (1000)     1108 2024-03-17 16:27:49.000000 cobib-5.0.1/src/cobib/commands/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    23338 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/add.py
--rw-r--r--   0 max       (1000) max       (1000)     7015 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/base_command.py
--rw-r--r--   0 max       (1000) max       (1000)     4633 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/delete.py
--rw-r--r--   0 max       (1000) max       (1000)     8699 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/edit.py
--rw-r--r--   0 max       (1000) max       (1000)     7477 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/export.py
--rw-r--r--   0 max       (1000) max       (1000)     3179 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/git.py
--rw-r--r--   0 max       (1000) max       (1000)     7264 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/import_.py
--rw-r--r--   0 max       (1000) max       (1000)     4548 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/init.py
--rw-r--r--   0 max       (1000) max       (1000)     4607 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/lint.py
--rw-r--r--   0 max       (1000) max       (1000)    14510 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/list_.py
--rw-r--r--   0 max       (1000) max       (1000)    21161 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/modify.py
--rw-r--r--   0 max       (1000) max       (1000)    10356 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/open.py
--rw-r--r--   0 max       (1000) max       (1000)     4578 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/redo.py
--rw-r--r--   0 max       (1000) max       (1000)    19498 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/review.py
--rw-r--r--   0 max       (1000) max       (1000)    11513 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/search.py
--rw-r--r--   0 max       (1000) max       (1000)     2211 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/show.py
--rw-r--r--   0 max       (1000) max       (1000)     5275 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/undo.py
--rw-r--r--   0 max       (1000) max       (1000)     2578 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/unify_labels.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.413231 cobib-5.0.1/src/cobib/config/
--rw-r--r--   0 max       (1000) max       (1000)     1302 2023-11-12 10:49:04.000000 cobib-5.0.1/src/cobib/config/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1521 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/config/command.py
--rw-r--r--   0 max       (1000) max       (1000)    42794 2024-05-01 13:42:08.000000 cobib-5.0.1/src/cobib/config/config.py
--rw-r--r--   0 max       (1000) max       (1000)    31459 2024-01-21 19:11:03.000000 cobib-5.0.1/src/cobib/config/event.py
--rw-r--r--   0 max       (1000) max       (1000)    11469 2023-12-12 08:31:55.000000 cobib-5.0.1/src/cobib/config/example.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.416564 cobib-5.0.1/src/cobib/database/
--rw-r--r--   0 max       (1000) max       (1000)     1413 2023-11-13 21:18:22.000000 cobib-5.0.1/src/cobib/database/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     4164 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/database/author.py
--rw-r--r--   0 max       (1000) max       (1000)    18110 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/database/database.py
--rw-r--r--   0 max       (1000) max       (1000)    24383 2024-01-21 19:11:03.000000 cobib-5.0.1/src/cobib/database/entry.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.419897 cobib-5.0.1/src/cobib/importers/
--rw-r--r--   0 max       (1000) max       (1000)      275 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/importers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     3051 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/importers/base_importer.py
--rw-r--r--   0 max       (1000) max       (1000)    12895 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/importers/zotero.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.423231 cobib-5.0.1/src/cobib/parsers/
--rw-r--r--   0 max       (1000) max       (1000)      520 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/parsers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5317 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/parsers/arxiv.py
--rw-r--r--   0 max       (1000) max       (1000)     2034 2023-08-27 11:42:15.000000 cobib-5.0.1/src/cobib/parsers/base_parser.py
--rw-r--r--   0 max       (1000) max       (1000)     3522 2023-11-12 10:49:04.000000 cobib-5.0.1/src/cobib/parsers/bibtex.py
--rw-r--r--   0 max       (1000) max       (1000)     3815 2023-08-27 11:42:15.000000 cobib-5.0.1/src/cobib/parsers/doi.py
--rw-r--r--   0 max       (1000) max       (1000)     4731 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/parsers/isbn.py
--rw-r--r--   0 max       (1000) max       (1000)     3593 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/parsers/url.py
--rw-r--r--   0 max       (1000) max       (1000)     3852 2024-01-21 19:11:03.000000 cobib-5.0.1/src/cobib/parsers/yaml.py
--rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/py.typed
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.426564 cobib-5.0.1/src/cobib/ui/
--rw-r--r--   0 max       (1000) max       (1000)      236 2024-03-17 16:27:49.000000 cobib-5.0.1/src/cobib/ui/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     4094 2024-03-17 16:27:49.000000 cobib-5.0.1/src/cobib/ui/cli.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.429897 cobib-5.0.1/src/cobib/ui/components/
--rw-r--r--   0 max       (1000) max       (1000)     1043 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/ui/components/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1911 2024-03-17 16:27:49.000000 cobib-5.0.1/src/cobib/ui/components/entry_points.py
--rw-r--r--   0 max       (1000) max       (1000)      705 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/ui/components/entry_view.py
--rw-r--r--   0 max       (1000) max       (1000)     3287 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/ui/components/help_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     2566 2024-01-14 16:13:13.000000 cobib-5.0.1/src/cobib/ui/components/input_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     4649 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/ui/components/list_view.py
--rw-r--r--   0 max       (1000) max       (1000)     1564 2024-01-14 16:13:13.000000 cobib-5.0.1/src/cobib/ui/components/log_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     2257 2024-01-21 19:11:03.000000 cobib-5.0.1/src/cobib/ui/components/logging_handler.py
--rw-r--r--   0 max       (1000) max       (1000)     2891 2023-12-11 20:47:52.000000 cobib-5.0.1/src/cobib/ui/components/main_content.py
--rw-r--r--   0 max       (1000) max       (1000)      565 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/ui/components/motion_key.py
--rw-r--r--   0 max       (1000) max       (1000)     2731 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/ui/components/preset_filter_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     3908 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/ui/components/search_view.py
--rw-r--r--   0 max       (1000) max       (1000)     1373 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/ui/components/selection_filter.py
--rw-r--r--   0 max       (1000) max       (1000)    21173 2024-03-17 16:27:49.000000 cobib-5.0.1/src/cobib/ui/tui.py
--rw-r--r--   0 max       (1000) max       (1000)     4311 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/ui/ui.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.433230 cobib-5.0.1/src/cobib/utils/
--rw-r--r--   0 max       (1000) max       (1000)      242 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/utils/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      460 2024-01-21 19:11:03.000000 cobib-5.0.1/src/cobib/utils/context.py
--rw-r--r--   0 max       (1000) max       (1000)     6731 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/utils/diff_renderer.py
--rw-r--r--   0 max       (1000) max       (1000)     7574 2024-04-28 11:21:44.000000 cobib-5.0.1/src/cobib/utils/file_downloader.py
--rw-r--r--   0 max       (1000) max       (1000)     4615 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/utils/journal_abbreviations.py
--rw-r--r--   0 max       (1000) max       (1000)     4776 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/utils/logging.py
--rw-r--r--   0 max       (1000) max       (1000)     2998 2024-01-21 19:11:03.000000 cobib-5.0.1/src/cobib/utils/progress.py
--rw-r--r--   0 max       (1000) max       (1000)     9017 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/utils/prompt.py
--rw-r--r--   0 max       (1000) max       (1000)     1860 2023-08-27 11:42:15.000000 cobib-5.0.1/src/cobib/utils/rel_path.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.433230 cobib-5.0.1/src/cobib.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)    51602 2024-05-01 13:46:22.000000 cobib-5.0.1/src/cobib.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     2366 2024-05-01 13:46:22.000000 cobib-5.0.1/src/cobib.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-01 13:46:22.000000 cobib-5.0.1/src/cobib.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)     1151 2024-05-01 13:46:22.000000 cobib-5.0.1/src/cobib.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)      135 2024-05-01 13:46:22.000000 cobib-5.0.1/src/cobib.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        6 2024-05-01 13:46:22.000000 cobib-5.0.1/src/cobib.egg-info/top_level.txt
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.433230 cobib-5.0.1/tests/
--rw-r--r--   0 max       (1000) max       (1000)     4314 2024-04-28 11:19:47.000000 cobib-5.0.1/tests/test_main.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:39.007002 cobib-5.1.0/
+-rw-r--r--   0 max       (1000) max       (1000)    43831 2024-05-28 18:14:52.000000 cobib-5.1.0/CHANGELOG.md
+-rw-r--r--   0 max       (1000) max       (1000)     1076 2024-01-18 21:03:08.000000 cobib-5.1.0/LICENSE.txt
+-rw-r--r--   0 max       (1000) max       (1000)      100 2023-06-12 19:22:05.000000 cobib-5.1.0/MANIFEST.in
+-rw-r--r--   0 max       (1000) max       (1000)    53373 2024-05-28 18:15:39.003669 cobib-5.1.0/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     8035 2024-03-17 16:27:49.000000 cobib-5.1.0/README.md
+-rw-r--r--   0 max       (1000) max       (1000)    37891 2024-05-28 18:13:54.000000 cobib-5.1.0/cobib.1
+-rw-r--r--   0 max       (1000) max       (1000)     4654 2024-05-25 07:44:16.000000 cobib-5.1.0/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)      135 2024-02-03 16:58:09.000000 cobib-5.1.0/requirements.txt
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-28 18:15:39.007002 cobib-5.1.0/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:38.967002 cobib-5.1.0/src/
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:38.973669 cobib-5.1.0/src/cobib/
+-rw-r--r--   0 max       (1000) max       (1000)      474 2024-05-28 18:13:59.000000 cobib-5.1.0/src/cobib/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      445 2024-03-17 16:27:49.000000 cobib-5.1.0/src/cobib/__main__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:38.983669 cobib-5.1.0/src/cobib/commands/
+-rw-r--r--   0 max       (1000) max       (1000)     1108 2024-03-17 16:27:49.000000 cobib-5.1.0/src/cobib/commands/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    23338 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/add.py
+-rw-r--r--   0 max       (1000) max       (1000)     7015 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/base_command.py
+-rw-r--r--   0 max       (1000) max       (1000)     4633 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/delete.py
+-rw-r--r--   0 max       (1000) max       (1000)     8699 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/edit.py
+-rw-r--r--   0 max       (1000) max       (1000)     7477 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/export.py
+-rw-r--r--   0 max       (1000) max       (1000)     3179 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/git.py
+-rw-r--r--   0 max       (1000) max       (1000)     7264 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/import_.py
+-rw-r--r--   0 max       (1000) max       (1000)     4548 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/init.py
+-rw-r--r--   0 max       (1000) max       (1000)     4607 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/lint.py
+-rw-r--r--   0 max       (1000) max       (1000)    20559 2024-05-25 13:12:31.000000 cobib-5.1.0/src/cobib/commands/list_.py
+-rw-r--r--   0 max       (1000) max       (1000)    21161 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/modify.py
+-rw-r--r--   0 max       (1000) max       (1000)    10356 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/open.py
+-rw-r--r--   0 max       (1000) max       (1000)     4578 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/redo.py
+-rw-r--r--   0 max       (1000) max       (1000)    19498 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/review.py
+-rw-r--r--   0 max       (1000) max       (1000)    16225 2024-05-25 13:12:23.000000 cobib-5.1.0/src/cobib/commands/search.py
+-rw-r--r--   0 max       (1000) max       (1000)     2211 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/show.py
+-rw-r--r--   0 max       (1000) max       (1000)     5275 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/undo.py
+-rw-r--r--   0 max       (1000) max       (1000)     2578 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/commands/unify_labels.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:38.987002 cobib-5.1.0/src/cobib/config/
+-rw-r--r--   0 max       (1000) max       (1000)     1302 2023-11-12 10:49:04.000000 cobib-5.1.0/src/cobib/config/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1521 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/config/command.py
+-rw-r--r--   0 max       (1000) max       (1000)    45259 2024-05-25 07:44:16.000000 cobib-5.1.0/src/cobib/config/config.py
+-rw-r--r--   0 max       (1000) max       (1000)    31459 2024-01-21 19:11:03.000000 cobib-5.1.0/src/cobib/config/event.py
+-rw-r--r--   0 max       (1000) max       (1000)    13120 2024-05-25 07:44:16.000000 cobib-5.1.0/src/cobib/config/example.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:38.987002 cobib-5.1.0/src/cobib/database/
+-rw-r--r--   0 max       (1000) max       (1000)     1413 2023-11-13 21:18:22.000000 cobib-5.1.0/src/cobib/database/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     4164 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/database/author.py
+-rw-r--r--   0 max       (1000) max       (1000)    18110 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/database/database.py
+-rw-r--r--   0 max       (1000) max       (1000)    28457 2024-05-25 07:44:16.000000 cobib-5.1.0/src/cobib/database/entry.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:38.990336 cobib-5.1.0/src/cobib/importers/
+-rw-r--r--   0 max       (1000) max       (1000)      275 2023-06-12 19:22:05.000000 cobib-5.1.0/src/cobib/importers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3051 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/importers/base_importer.py
+-rw-r--r--   0 max       (1000) max       (1000)    12895 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/importers/zotero.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:38.993669 cobib-5.1.0/src/cobib/parsers/
+-rw-r--r--   0 max       (1000) max       (1000)      520 2023-06-12 19:22:05.000000 cobib-5.1.0/src/cobib/parsers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     5317 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/parsers/arxiv.py
+-rw-r--r--   0 max       (1000) max       (1000)     2034 2023-08-27 11:42:15.000000 cobib-5.1.0/src/cobib/parsers/base_parser.py
+-rw-r--r--   0 max       (1000) max       (1000)     3522 2023-11-12 10:49:04.000000 cobib-5.1.0/src/cobib/parsers/bibtex.py
+-rw-r--r--   0 max       (1000) max       (1000)     3815 2023-08-27 11:42:15.000000 cobib-5.1.0/src/cobib/parsers/doi.py
+-rw-r--r--   0 max       (1000) max       (1000)     4731 2023-12-17 17:15:09.000000 cobib-5.1.0/src/cobib/parsers/isbn.py
+-rw-r--r--   0 max       (1000) max       (1000)     3593 2023-12-17 17:15:09.000000 cobib-5.1.0/src/cobib/parsers/url.py
+-rw-r--r--   0 max       (1000) max       (1000)     3852 2024-01-21 19:11:03.000000 cobib-5.1.0/src/cobib/parsers/yaml.py
+-rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-12 19:22:05.000000 cobib-5.1.0/src/cobib/py.typed
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:38.993669 cobib-5.1.0/src/cobib/ui/
+-rw-r--r--   0 max       (1000) max       (1000)      236 2024-03-17 16:27:49.000000 cobib-5.1.0/src/cobib/ui/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     4094 2024-03-17 16:27:49.000000 cobib-5.1.0/src/cobib/ui/cli.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:38.997002 cobib-5.1.0/src/cobib/ui/components/
+-rw-r--r--   0 max       (1000) max       (1000)     1043 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/ui/components/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1911 2024-03-17 16:27:49.000000 cobib-5.1.0/src/cobib/ui/components/entry_points.py
+-rw-r--r--   0 max       (1000) max       (1000)      705 2023-06-12 19:22:05.000000 cobib-5.1.0/src/cobib/ui/components/entry_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     3287 2023-12-17 17:15:09.000000 cobib-5.1.0/src/cobib/ui/components/help_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     2566 2024-01-14 16:13:13.000000 cobib-5.1.0/src/cobib/ui/components/input_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     4649 2023-12-17 17:15:09.000000 cobib-5.1.0/src/cobib/ui/components/list_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     1564 2024-01-14 16:13:13.000000 cobib-5.1.0/src/cobib/ui/components/log_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     2257 2024-01-21 19:11:03.000000 cobib-5.1.0/src/cobib/ui/components/logging_handler.py
+-rw-r--r--   0 max       (1000) max       (1000)     2891 2023-12-11 20:47:52.000000 cobib-5.1.0/src/cobib/ui/components/main_content.py
+-rw-r--r--   0 max       (1000) max       (1000)      565 2023-06-12 19:22:05.000000 cobib-5.1.0/src/cobib/ui/components/motion_key.py
+-rw-r--r--   0 max       (1000) max       (1000)     2731 2023-12-17 17:15:09.000000 cobib-5.1.0/src/cobib/ui/components/preset_filter_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     3908 2023-12-17 17:15:09.000000 cobib-5.1.0/src/cobib/ui/components/search_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     1373 2023-12-17 17:15:09.000000 cobib-5.1.0/src/cobib/ui/components/selection_filter.py
+-rw-r--r--   0 max       (1000) max       (1000)    21173 2024-03-17 16:27:49.000000 cobib-5.1.0/src/cobib/ui/tui.py
+-rw-r--r--   0 max       (1000) max       (1000)     4311 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/ui/ui.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:39.003669 cobib-5.1.0/src/cobib/utils/
+-rw-r--r--   0 max       (1000) max       (1000)      242 2023-06-12 19:22:05.000000 cobib-5.1.0/src/cobib/utils/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      460 2024-01-21 19:11:03.000000 cobib-5.1.0/src/cobib/utils/context.py
+-rw-r--r--   0 max       (1000) max       (1000)     6731 2023-06-12 19:22:05.000000 cobib-5.1.0/src/cobib/utils/diff_renderer.py
+-rw-r--r--   0 max       (1000) max       (1000)     7574 2024-04-28 11:21:44.000000 cobib-5.1.0/src/cobib/utils/file_downloader.py
+-rw-r--r--   0 max       (1000) max       (1000)     4615 2023-12-17 17:15:09.000000 cobib-5.1.0/src/cobib/utils/journal_abbreviations.py
+-rw-r--r--   0 max       (1000) max       (1000)     4776 2023-12-17 17:15:09.000000 cobib-5.1.0/src/cobib/utils/logging.py
+-rw-r--r--   0 max       (1000) max       (1000)     1015 2024-05-25 07:44:16.000000 cobib-5.1.0/src/cobib/utils/match.py
+-rw-r--r--   0 max       (1000) max       (1000)     2998 2024-01-21 19:11:03.000000 cobib-5.1.0/src/cobib/utils/progress.py
+-rw-r--r--   0 max       (1000) max       (1000)     9017 2024-04-28 11:19:47.000000 cobib-5.1.0/src/cobib/utils/prompt.py
+-rw-r--r--   0 max       (1000) max       (1000)      781 2024-05-25 07:44:16.000000 cobib-5.1.0/src/cobib/utils/regex.py
+-rw-r--r--   0 max       (1000) max       (1000)     1860 2023-08-27 11:42:15.000000 cobib-5.1.0/src/cobib/utils/rel_path.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:39.003669 cobib-5.1.0/src/cobib.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)    53373 2024-05-28 18:15:38.000000 cobib-5.1.0/src/cobib.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     2416 2024-05-28 18:15:38.000000 cobib-5.1.0/src/cobib.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-28 18:15:38.000000 cobib-5.1.0/src/cobib.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)     1151 2024-05-28 18:15:38.000000 cobib-5.1.0/src/cobib.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)      170 2024-05-28 18:15:38.000000 cobib-5.1.0/src/cobib.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        6 2024-05-28 18:15:38.000000 cobib-5.1.0/src/cobib.egg-info/top_level.txt
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-28 18:15:39.003669 cobib-5.1.0/tests/
+-rw-r--r--   0 max       (1000) max       (1000)     4314 2024-04-28 11:19:47.000000 cobib-5.1.0/tests/test_main.py
```

### Comparing `cobib-5.0.1/CHANGELOG.md` & `cobib-5.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,47 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [5.1.0] - 2024-05-28
+
+Pypi: https://pypi.org/project/cobib/5.1.0/
+
+### Prelude
+
+Check out my blog post to learn more about the features of this new release:
+https://mrossinek.gitlab.io/programming/cobib-becomes-fuzzy/
+
+### Added
+- approximate (or fuzzy) filter matching and search functionality (#107,#130,!177)
+  - the `list` and `search` commands now support the following features to
+    perform approximate filter matching and searching, respectively:
+    - LaTeX sequences can be decoded to Unicode characters:
+      - using `--decode-latex` from the command-line
+      - setting `config.commands.list_.decode_latex = True`
+      - setting `config.commands.search.decode_latex = True`
+    - Unicode characters can be converted to a close ASCII equivalent:
+      - using `--decode-unicode` from the command-line
+      - setting `config.commands.list_.decode_unicode = True`
+      - setting `config.commands.search.decode_unicode = True`
+    - a number of fuzzy errors can be set (this requires the optional dependency
+      [`regex`](https://pypi.org/project/regex/) to be installed):
+      - using `--fuzziness <int>` from the command-line
+      - setting `config.commands.list_.fuzzines` to some integer
+      - setting `config.commands.search.fuzzines` to some integer
+- (DEV) the following method arguments have been converted to be accepted only
+  as keyword arguments:
+  - in `cobib.database.Entry.matches`: `ignore_case`
+  - in `cobib.database.Entry.search`: `context`, `ignore_case`, and `skip_files`
+- (DEV) the return-type of `cobib.database.Entry.search` has been changed
+
+
 ## [5.0.1] - 2024-05-01
 
 Pypi: https://pypi.org/project/cobib/5.0.1/
 
 ### Fixed
 - the ability to use an empty string as the separator in `config.database.format.label_suffix` (#138)
 
@@ -996,15 +1029,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.0.1...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.1.0...master
+[5.1.0]: https://gitlab.com/cobib/cobib/-/tags/v5.1.0
 [5.0.1]: https://gitlab.com/cobib/cobib/-/tags/v5.0.1
 [5.0.0]: https://gitlab.com/cobib/cobib/-/tags/v5.0.0
 [4.5.0]: https://gitlab.com/cobib/cobib/-/tags/v4.5.0
 [4.4.0]: https://gitlab.com/cobib/cobib/-/tags/v4.4.0
 [4.3.1]: https://gitlab.com/cobib/cobib/-/tags/v4.3.1
 [4.3.0]: https://gitlab.com/cobib/cobib/-/tags/v4.3.0
 [4.2.0]: https://gitlab.com/cobib/cobib/-/tags/v4.2.0
```

### Comparing `cobib-5.0.1/LICENSE.txt` & `cobib-5.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/PKG-INFO` & `cobib-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 5.0.1
+Version: 5.1.0
 Summary: Console Bibliography
 Author-email: Max Rossmannek <max@rossmannek.de>
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/cobib/cobib
 Project-URL: Documentation, https://cobib.gitlab.io/cobib/cobib.html
 Project-URL: Repository, https://gitlab.com/cobib/cobib
 Project-URL: Issues, https://gitlab.com/cobib/cobib/-/issues
@@ -29,14 +29,18 @@
 Requires-Dist: requests
 Requires-Dist: requests_oauthlib
 Requires-Dist: rich
 Requires-Dist: ruamel.yaml
 Requires-Dist: textual>=0.48
 Requires-Dist: typing_extensions
 Requires-Dist: text-unidecode
+Provides-Extra: all
+Requires-Dist: cobib[fuzzy]; extra == "all"
+Provides-Extra: fuzzy
+Requires-Dist: regex; extra == "fuzzy"
 
 [![coBib](https://gitlab.com/cobib/cobib/-/raw/master/logo/cobib_logo.svg)](https://cobib.gitlab.io/cobib/cobib.html)
 
 # coBib
 
 [![pipeline](https://gitlab.com/cobib/cobib/badges/master/pipeline.svg)](https://gitlab.com/cobib/cobib/-/pipelines)
 [![coverage](https://gitlab.com/cobib/cobib/badges/master/coverage.svg)](https://gitlab.com/cobib/cobib/-/graphs/master/charts)
@@ -307,14 +311,47 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [5.1.0] - 2024-05-28
+
+Pypi: https://pypi.org/project/cobib/5.1.0/
+
+### Prelude
+
+Check out my blog post to learn more about the features of this new release:
+https://mrossinek.gitlab.io/programming/cobib-becomes-fuzzy/
+
+### Added
+- approximate (or fuzzy) filter matching and search functionality (#107,#130,!177)
+  - the `list` and `search` commands now support the following features to
+    perform approximate filter matching and searching, respectively:
+    - LaTeX sequences can be decoded to Unicode characters:
+      - using `--decode-latex` from the command-line
+      - setting `config.commands.list_.decode_latex = True`
+      - setting `config.commands.search.decode_latex = True`
+    - Unicode characters can be converted to a close ASCII equivalent:
+      - using `--decode-unicode` from the command-line
+      - setting `config.commands.list_.decode_unicode = True`
+      - setting `config.commands.search.decode_unicode = True`
+    - a number of fuzzy errors can be set (this requires the optional dependency
+      [`regex`](https://pypi.org/project/regex/) to be installed):
+      - using `--fuzziness <int>` from the command-line
+      - setting `config.commands.list_.fuzzines` to some integer
+      - setting `config.commands.search.fuzzines` to some integer
+- (DEV) the following method arguments have been converted to be accepted only
+  as keyword arguments:
+  - in `cobib.database.Entry.matches`: `ignore_case`
+  - in `cobib.database.Entry.search`: `context`, `ignore_case`, and `skip_files`
+- (DEV) the return-type of `cobib.database.Entry.search` has been changed
+
+
 ## [5.0.1] - 2024-05-01
 
 Pypi: https://pypi.org/project/cobib/5.0.1/
 
 ### Fixed
 - the ability to use an empty string as the separator in `config.database.format.label_suffix` (#138)
 
@@ -1300,15 +1337,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.0.1...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.1.0...master
+[5.1.0]: https://gitlab.com/cobib/cobib/-/tags/v5.1.0
 [5.0.1]: https://gitlab.com/cobib/cobib/-/tags/v5.0.1
 [5.0.0]: https://gitlab.com/cobib/cobib/-/tags/v5.0.0
 [4.5.0]: https://gitlab.com/cobib/cobib/-/tags/v4.5.0
 [4.4.0]: https://gitlab.com/cobib/cobib/-/tags/v4.4.0
 [4.3.1]: https://gitlab.com/cobib/cobib/-/tags/v4.3.1
 [4.3.0]: https://gitlab.com/cobib/cobib/-/tags/v4.3.0
 [4.2.0]: https://gitlab.com/cobib/cobib/-/tags/v4.2.0
```

### Comparing `cobib-5.0.1/README.md` & `cobib-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/cobib.1` & `cobib-5.1.0/cobib.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH COBIB 1 2024-05-01 v5.0.1
+.TH COBIB 1 2024-05-28 v5.1.0
 .SH NAME
 coBib \- Console-based Bibliography Management
 .SH SYNOPSIS
 .B cobib
 [\fB\-\-version\fR]
 [\fB\-h\fR|\fB\-\-help\fR]
 [\fB\-v\fR|\fB\-\-verbose\fR]
@@ -405,14 +405,47 @@
 .in +8n
 .BR \-I ", " \-\-no\-ignore\-case
 .in +4n
 Makes the entry matching case-sensitive.
 This takes precedence over the \fIconfig.commands.list_.ignore_case\fR setting.
 .PP
 .in +8n
+.BR \-\-decode\-latex
+.in +4n
+Makes the entry matching decode all LaTeX sequences.
+This takes precedence over the \fIconfig.commands.list_.decode_latex\fR setting.
+.PP
+.in +8n
+.BR \-\-no\-decode\-latex
+.in +4n
+Makes the entry matching preserve all LaTeX sequences.
+This takes precedence over the \fIconfig.commands.list_.decode_latex\fR setting.
+.PP
+.in +8n
+.BR \-\-decode\-unicode
+.in +4n
+Makes the entry matching decode all Unicode characters.
+This takes precedence over the \fIconfig.commands.list_.decode_unicode\fR
+setting.
+.PP
+.in +8n
+.BR \-\-no\-decode\-unicode
+.in +4n
+Makes the entry matching preserve all Unicode characters.
+This takes precedence over the \fIconfig.commands.list_.decode_unicode\fR
+setting.
+.PP
+.in +8n
+.BR \-z ", " \-\-fuzziness " " \fI<int>\fI
+.in +4n
+Specifies how many fuzzy errors to allow during entry matching.
+The default value is 0 but can be configured via
+\fIconfig.commands.list_.fuzziness\fR.
+.PP
+.in +8n
 .BR \-x ", " \-\-or
 .in +4n
 Concatenate the filters using logical \fIOR\fR rather than the default
 \fIAND\fR.
 .TP
 .B cobib search \fI<query>\fR \fI<args>\fR ...
 Searches the database recursively (i.e. including any associated files) for the
@@ -434,15 +467,50 @@
 Makes the search case-insensitive.
 This takes precedence over the \fIconfig.commands.search.ignore_case\fR setting.
 .PP
 .in +8n
 .BR \-I ", " \-\-no\-ignore\-case
 .in +4n
 Makes the search case-insensitive.
-This takes precedence over the \fIconfig.commands.list_.ignore_case\fR setting.
+This takes precedence over the \fIconfig.commands.search.ignore_case\fR setting.
+.PP
+.in +8n
+.BR \-l ", " \-\-decode\-latex
+.in +4n
+Makes the search decode all LaTeX sequences.
+This takes precedence over the \fIconfig.commands.search.decode_latex\fR
+setting.
+.PP
+.in +8n
+.BR \-L ", " \-\-no\-decode\-latex
+.in +4n
+Makes the search preserve all LaTeX sequences.
+This takes precedence over the \fIconfig.commands.search.decode_latex\fR
+setting.
+.PP
+.in +8n
+.BR \-u ", " \-\-decode\-unicode
+.in +4n
+Makes the search decode all Unicode characters.
+This takes precedence over the \fIconfig.commands.search.decode_unicode\fR
+setting.
+.PP
+.in +8n
+.BR \-U ", " \-\-no\-decode\-unicode
+.in +4n
+Makes the search preserve all Unicode characters.
+This takes precedence over the \fIconfig.commands.search.decode_unicode\fR
+setting.
+.PP
+.in +8n
+.BR \-z ", " \-\-fuzziness " " \fI<int>\fI
+.in +4n
+Specifies how many fuzzy errors to allow during search.
+The default value is 0 but can be configured via
+\fIconfig.commands.search.fuzziness\fR.
 .PP
 .in +8n
 .BR \-\-skip\-files
 .in +4n
 Skips searching the associated files.
 .TP
 .B cobib export \fI<args>\fR ...
@@ -742,14 +810,24 @@
 .TP
 .IR config.commands.list_.default_columns = ['label',\ 'title']
 Specifies the default columns displayed during the \fIlist\fR command.
 .TP
 .IR config.commands.list_.ignore_case = False
 Specifies whether filter matching should be performed case-insensitive.
 .TP
+.IR config.commands.list_.decode_unicode = False
+Specifies whether filter matching should decode all Unicode characters.
+.TP
+.IR config.commands.list_.decode_latex = False
+Specifies whether filter matching should decode all LaTeX sequences.
+.TP
+.IR config.commands.list_.fuzziness = 0
+Specifies the amount of fuzzy errors to allow for filter matching. Using this
+feature requires the optional \fIregex\fR dependency to be installed.
+.TP
 .IR config.commands.modify.preserve_files = False
 Specifies whether associates files should be preserved during renaming.
 .TP
 .IR config.commands.open.command = 'xdg-open' " (on Linux); " 'open' " (on Mac OS)"
 Specifies the program used to open associated files.
 .TP
 .IR config.commands.open.fields = ['file',\ 'url']
@@ -765,14 +843,24 @@
 .TP
 .IR config.commands.search.grep_args = []
 Allows the specification of additional arguments for the \fIgrep\fR command.
 .TP
 .IR config.commands.search.ignore_case = False
 This boolean setting indicates whether search defaults to be case-insensitive.
 .TP
+.IR config.commands.search.decode_unicode = False
+Specifies whether searches should decode all Unicode characters.
+.TP
+.IR config.commands.search.decode_latex = False
+Specifies whether searches should decode all LaTeX sequences.
+.TP
+.IR config.commands.search.fuzziness = 0
+Specifies the amount of fuzzy errors to allow for searches. Using this feature
+requires the optional \fIregex\fR dependency to be installed.
+.TP
 .IR config.commands.show.encode_latex = True
 This boolean setting indicates whether non-ASCII characters should be encoded
 using LaTeX sequences during rendering via the \fIshow\fR command.
 .PP
 .BR DATABASE
 .TP
 .IR config.database.file = '~/.local/share/cobib/literature.yaml'
```

### Comparing `cobib-5.0.1/pyproject.toml` & `cobib-5.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,18 @@
 isbn = "cobib.parsers.isbn:ISBNParser"
 url = "cobib.parsers.url:URLParser"
 yaml = "cobib.parsers.yaml:YAMLParser"
 
 [project.scripts]
 cobib = "cobib.__main__:_main"
 
+[project.optional-dependencies]
+all = ["cobib[fuzzy]"]
+fuzzy = ["regex"]
+
 [project.urls]
 Homepage = "https://gitlab.com/cobib/cobib"
 Documentation = "https://cobib.gitlab.io/cobib/cobib.html"
 Repository = "https://gitlab.com/cobib/cobib"
 Issues = "https://gitlab.com/cobib/cobib/-/issues"
 Changelog = "https://gitlab.com/cobib/cobib/-/blob/master/CHANGELOG.md"
```

### Comparing `cobib-5.0.1/src/cobib/commands/__init__.py` & `cobib-5.1.0/src/cobib/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/add.py` & `cobib-5.1.0/src/cobib/commands/add.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/base_command.py` & `cobib-5.1.0/src/cobib/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/delete.py` & `cobib-5.1.0/src/cobib/commands/delete.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/edit.py` & `cobib-5.1.0/src/cobib/commands/edit.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/export.py` & `cobib-5.1.0/src/cobib/commands/export.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/git.py` & `cobib-5.1.0/src/cobib/commands/git.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/import_.py` & `cobib-5.1.0/src/cobib/commands/import_.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/init.py` & `cobib-5.1.0/src/cobib/commands/init.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/lint.py` & `cobib-5.1.0/src/cobib/commands/lint.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/list_.py` & `cobib-5.1.0/src/cobib/commands/list_.py`

 * *Files 26% similar despite different names*

```diff
@@ -87,34 +87,76 @@
 cobib list --ignore-case ++author rossmannek
 ```
 And the following will *always* be sensitive to case:
 ```
 cobib list --no-ignore-case ++author rossmannek
 ```
 
+
+### Approximate matching
+
 .. note::
-   For more information on the filtering mechanisms see also `cobib.database.Entry.matches`.
+   New in version v5.1.0
+
+Besides case-insensitive filter matching (see above), coBib now also provides more means to perform
+approximate matching of your filters.
+
+The `--decode-latex` argument will convert LaTeX sequences to Unicode characters (where possible).
+For example, a LaTeX-encoded Umlaut like `\"o` will become `ö`. This can significantly simplify your
+match query, for example:
+```
+cobib list --decode-latex ++title Körper
+```
+will match entries whose title contains `K{\"o}rper`.
+You can enable this behavior by default by setting `config.commands.list_.decode_latex = True`.
+If you have enabled this setting, you can temporarily overwrite it from the command-line with the
+`--no-decode-latex` argument.
+
+Additionally, you can convert Unicode characters to a close ASCII equivalent with `--decode-unicode`
+which can simplify your search further. Reusing the example above, you can now match titles
+containing `K{\"o}rper` as follows:
+```
+cobib list --decode-latex --decode-unicode ++title Korper
+```
+You can enable this behavior by default by setting `config.commands.list_.decode_unicode = True`.
+If you have enabled this setting, you can temporarily overwrite it from the command-line with the
+`--no-decode-unicode` argument.
+
+Finally, if you install the optional [`regex`](https://pypi.org/project/regex/) dependency you can
+even perform fuzzy matching. For example, you can specify the amount of fuzzy errors to allow via
+the `--fuzziness` (`-z` for short) argument. Reusing the sample example again, you can allow for
+typos in your filter like so:
+```
+cobib list --decode-latex --decode-unicode --fuzziness 2 ++title Koprer
+```
+You can specify a default amount of fuzzy errors by setting `config.commands.list_.fuzziness` to the
+desired value.
+
+
+.. note::
+   For more information on the filtering mechanisms see also `cobib.database.entry.Entry.matches`.
 """
 
 from __future__ import annotations
 
 import argparse
 import logging
 from collections import defaultdict
 from copy import copy
-from typing import Any
+from typing import Any, Final, Literal, get_args
 
 from rich.console import ConsoleRenderable
 from rich.table import Table
 from rich.text import Text
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database, Entry
 from cobib.ui.components import ListView
+from cobib.utils.regex import HAS_OPTIONAL_REGEX
 
 from .base_command import Command
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
@@ -134,23 +176,49 @@
         * `-l`, `--limit`: you can specify a maximum number of entries to be returned in order to
           limit the amount of matches to be displayed. (Note, that as of now, this is purely a
           post-processing step and, thus, does not yield faster results.)
         * `-i`, `--ignore-case`: if specified, the entry matching will be case-**in**sensitive. This
           overwrites the `cobib.config.config.ListCommandConfig.ignore_case` setting.
         * `-I`, `--no-ignore-case`: if specified, the entry matching will be case-sensitive. This
           overwrites the `cobib.config.config.ListCommandConfig.ignore_case` setting.
+        * `--decode-latex`: if specified, all LaTeX sequences will be decoded before matching. This
+          overwrites the `cobib.config.config.ListCommandConfig.decode_latex` setting.
+        * `--no-decode-latex`: if specified, LaTeX sequences will be left unchanged before matching.
+          This overwrites the `cobib.config.config.ListCommandConfig.decode_latex` setting.
+        * `--decode-unicode`: if specified, all Unicode characters will be decoded before matching.
+          This overwrites the `cobib.config.config.ListCommandConfig.decode_unicode` setting.
+        * `--no-decode-unicode`: if specified, Unicode characters will be left unchanged before
+          matching. This overwrites the `cobib.config.config.ListCommandConfig.decode_unicode`
+          setting.
+        * `-z`, `--fuzziness`: you can specify the number of fuzzy errors to allow for entry
+          matching. This requires the optional `regex` dependency to be installed.
         * `-x`, `--or`: if specified, multiple filters will be combined with logical OR rather than
           the default logical AND.
         * in addition to the options above, [Filter keyword arguments](#filters) are registered at
           runtime based on the fields available in the database. Please refer that section or the
           output of `cobib list --help` for more information.
     """
 
     name = "list"
 
+    _RESERVED_FIELDS = Final[
+        Literal[
+            "OR",
+            "sort",
+            "reverse",
+            "limit",
+            "ignore_case",
+            "decode_latex",
+            "decode_unicode",
+            "fuzziness",
+        ]
+    ]
+    """These fields are reserved because they correspond to the names of the command-line arguments.
+    This list of values is used when constructing the filter during `filter_entries`."""
+
     @override
     def __init__(self, *args: str) -> None:
         super().__init__(*args)
 
         self.entries: list[Entry] = []
         """A list of entries, filtered and sorted according to the provided command arguments."""
 
@@ -183,14 +251,52 @@
             "-I",
             "--no-ignore-case",
             dest="ignore_case",
             action="store_false",
             default=None,
             help="do NOT ignore case for entry matching",
         )
+        latex_group = parser.add_mutually_exclusive_group()
+        latex_group.add_argument(
+            "--decode-latex",
+            action="store_true",
+            default=None,
+            help="decode LaTeX sequences for entry matching",
+        )
+        latex_group.add_argument(
+            "--no-decode-latex",
+            dest="decode_latex",
+            action="store_false",
+            default=None,
+            help="do NOT decode LaTeX sequences for entry matching",
+        )
+        unicode_group = parser.add_mutually_exclusive_group()
+        unicode_group.add_argument(
+            "--decode-unicode",
+            action="store_true",
+            default=None,
+            help="decode Unicode characters for entry matching",
+        )
+        unicode_group.add_argument(
+            "--no-decode-unicode",
+            dest="decode_unicode",
+            action="store_false",
+            default=None,
+            help="do NOT decode Unicode characters for entry matching",
+        )
+        parser.add_argument(
+            "-z",
+            "--fuzziness",
+            type=int,
+            default=config.commands.list_.fuzziness,
+            help=(
+                "how many fuzzy errors to allow for entry matching. This requires the optional "
+                "`regex` dependency to be installed."
+            ),
+        )
         parser.add_argument(
             "-x",
             "--or",
             dest="OR",
             action="store_true",
             help="concatenate filters with OR instead of AND",
         )
@@ -209,15 +315,24 @@
         cls.argparser = parser
 
     @override
     @classmethod
     def _parse_args(cls, args: tuple[str, ...]) -> argparse.Namespace:
         args = tuple(arg for arg in args if arg != "--")
 
-        return super()._parse_args(args)
+        largs = super()._parse_args(args)
+
+        if largs.fuzziness > 0 and not HAS_OPTIONAL_REGEX:  # pragma: no branch
+            LOGGER.warning(  # pragma: no cover
+                "Using the `--fuzziness` argument requires the optional `regex` dependency to be "
+                "installed! Falling back to `fuzziness=0`."
+            )
+            largs.fuzziness = 0  # pragma: no cover
+
+        return largs
 
     @override
     def execute(self) -> None:
         LOGGER.debug("Starting List command.")
 
         Event.PreListCommand.fire(self)
 
@@ -271,15 +386,18 @@
         """
         LOGGER.debug("Constructing filter.")
 
         filtered_keys: set[str] = set()
         _filter: dict[tuple[str, bool], list[Any]] = defaultdict(list)
 
         for key, val in self.largs.__dict__.items():
-            if key in ["OR", "sort", "reverse", "limit", "ignore_case"] or val is None:
+            # we use get_args twice:
+            #  1. to extract the args from `Final`
+            #  2. and then to extract the args from the `Literal` stored in the first arg of `Final`
+            if key in get_args(get_args(self._RESERVED_FIELDS)[0]) or val is None:
                 # ignore special arguments
                 continue
 
             # track the keys being filtered to display these columns later
             filtered_keys.add(key)
 
             if not isinstance(val, list):
@@ -302,20 +420,42 @@
         ignore_case = config.commands.list_.ignore_case
         if self.largs.ignore_case is not None:
             ignore_case = self.largs.ignore_case
         LOGGER.debug(
             "The entry matching will be performed case %ssensitive", "in" if ignore_case else ""
         )
 
+        decode_latex = config.commands.list_.decode_latex
+        if self.largs.decode_latex is not None:
+            decode_latex = self.largs.decode_latex
+        LOGGER.debug(
+            "The entry matching will%s decode all LaTeX sequences", "" if decode_latex else " NOT"
+        )
+
+        decode_unicode = config.commands.list_.decode_unicode
+        if self.largs.decode_unicode is not None:
+            decode_unicode = self.largs.decode_unicode
+        LOGGER.debug(
+            "The entry matching will%s decode all Unicode characters",
+            "" if decode_unicode else " NOT",
+        )
+
         if len(filtered_keys) == 0:
             # bypassing the unnecessary calls to `Entry.matches` when no filter was provided
             self.entries = list(Database().values())
         else:
             for key, entry in Database().items():
-                if entry.matches(_filter, self.largs.OR, ignore_case):
+                if entry.matches(
+                    _filter,
+                    self.largs.OR,
+                    ignore_case=ignore_case,
+                    decode_latex=decode_latex,
+                    decode_unicode=decode_unicode,
+                    fuzziness=self.largs.fuzziness,
+                ):
                     LOGGER.debug('Entry "%s" matches the filter.', key)
                     self.entries.append(entry)
 
         return self.entries, filtered_keys
 
     def sort_entries(self) -> list[Entry]:
         """The sorting method.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cobib-5.0.1/src/cobib/commands/modify.py` & `cobib-5.1.0/src/cobib/commands/modify.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/open.py` & `cobib-5.1.0/src/cobib/commands/open.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/redo.py` & `cobib-5.1.0/src/cobib/commands/redo.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/review.py` & `cobib-5.1.0/src/cobib/commands/review.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/show.py` & `cobib-5.1.0/src/cobib/commands/show.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/undo.py` & `cobib-5.1.0/src/cobib/commands/undo.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/commands/unify_labels.py` & `cobib-5.1.0/src/cobib/commands/unify_labels.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/config/__init__.py` & `cobib-5.1.0/src/cobib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/config/command.py` & `cobib-5.1.0/src/cobib/config/command.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/config/config.py` & `cobib-5.1.0/src/cobib/config/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, NamedTuple, TextIO
 
 from rich.style import Style
 from rich.theme import Theme
 from typing_extensions import override
 
+from cobib.utils.regex import HAS_OPTIONAL_REGEX
 from cobib.utils.rel_path import RelPath
 
 if TYPE_CHECKING:
     import rich
 
     from .event import Event
 
@@ -347,26 +348,51 @@
 class ListCommandConfig(_ConfigBase):
     """The `config.commands.list_` section."""
 
     default_columns: list[str] = field(default_factory=lambda: ["label", "title"])
     """Specifies the default columns shown during the `list` command."""
     ignore_case: bool = False
     """Specifies whether filter matching should be performed case-insensitive."""
+    decode_unicode: bool = False
+    """Specifies whether filter matching should decode all Unicode characters."""
+    decode_latex: bool = False
+    """Specifies whether filter matching should decode all LaTeX sequences."""
+    fuzziness: int = 0
+    """The amount of fuzzy errors to allow for filter matching. Using this feature requires the
+    optional `regex` dependency to be installed."""
 
     @override
     def validate(self) -> None:
         LOGGER.debug("Validating the COMMANDS.LIST configuration section.")
         self._assert(
             isinstance(self.default_columns, list),
             "config.commands.list_.default_columns should be a list.",
         )
         self._assert(
             isinstance(self.ignore_case, bool),
             "config.commands.list_.ignore_case should be a boolean.",
         )
+        self._assert(
+            isinstance(self.decode_unicode, bool),
+            "config.commands.list_.decode_unicode should be a boolean.",
+        )
+        self._assert(
+            isinstance(self.decode_latex, bool),
+            "config.commands.list_.decode_latex should be a boolean.",
+        )
+        self._assert(
+            isinstance(self.fuzziness, int) and self.fuzziness >= 0,
+            "config.commands.list_.fuzziness should be a non-negative integer.",
+        )
+        if self.fuzziness > 0 and not HAS_OPTIONAL_REGEX:  # pragma: no branch
+            LOGGER.warning(  # pragma: no cover
+                "Using `config.commands.list_.fuzziness` requires the optional `regex` "
+                "dependency to be installed! Falling back to `fuzziness=0`."
+            )
+            self.fuzziness = 0  # pragma: no cover
 
 
 @dataclass
 class ModifyCommandConfig(_ConfigBase):
     """The `config.commands.modify` section."""
 
     preserve_files: bool = False
@@ -416,14 +442,21 @@
     default tool (`grep`) will not provide results for attached PDFs but other tools such as
     [ripgrep-all](https://github.com/phiresky/ripgrep-all) will."""
     grep_args: list[str] = field(default_factory=list)
     """Specifies additional arguments for your grep command. Note, that GNU's grep understands
     extended regex patterns even without specifying `-E`."""
     ignore_case: bool = False
     """Specifies whether searches should be performed case-insensitive."""
+    decode_unicode: bool = False
+    """Specifies whether searches should decode all Unicode characters."""
+    decode_latex: bool = False
+    """Specifies whether searches should decode all LaTeX sequences."""
+    fuzziness: int = 0
+    """The amount of fuzzy errors to allow for search matches. Using this feature requires the
+    optional `regex` dependency to be installed."""
 
     @property
     def highlights(self) -> SearchHighlightConfig:
         """**DEPRECATED** Use `config.theme.search` instead!
 
         The nested section for highlights used when displaying search results.
         """
@@ -449,14 +482,32 @@
             isinstance(self.grep_args, list),
             "config.commands.search.grep_args should be a list.",
         )
         self._assert(
             isinstance(self.ignore_case, bool),
             "config.commands.search.ignore_case should be a boolean.",
         )
+        self._assert(
+            isinstance(self.decode_unicode, bool),
+            "config.commands.search.decode_unicode should be a boolean.",
+        )
+        self._assert(
+            isinstance(self.decode_latex, bool),
+            "config.commands.search.decode_latex should be a boolean.",
+        )
+        self._assert(
+            isinstance(self.fuzziness, int) and self.fuzziness >= 0,
+            "config.commands.search.fuzziness should be a non-negative integer.",
+        )
+        if self.fuzziness > 0 and not HAS_OPTIONAL_REGEX:
+            LOGGER.warning(
+                "Using `config.commands.search.fuzziness` requires the optional `regex` "
+                "dependency to be installed! Falling back to `fuzziness=0`."
+            )
+            self.fuzziness = 0
 
 
 @dataclass
 class ShowCommandConfig(_ConfigBase):
     """The `config.commands.show` section."""
 
     encode_latex: bool = True
```

### Comparing `cobib-5.0.1/src/cobib/config/event.py` & `cobib-5.1.0/src/cobib/config/event.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/config/example.py` & `cobib-5.1.0/src/cobib/config/example.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """
 
 # Generally, you won't need these, but the default configuration relies on them.
 import os
 import sys
 
 # To get started you must import coBib's configuration.
-from cobib.config import LabelSuffix, TagMarkup, config
+from cobib.config import AuthorFormat, LabelSuffix, TagMarkup, config
 
 # Now, you are all set to apply your own settings.
 
 
 # LOGGING
 # You can specify the default cache location.
 config.logging.cache = "~/.cache/cobib/cache"
@@ -53,14 +53,21 @@
 # You can specify whether downloading of attachments inside the imported library should be skipped.
 config.commands.import_.skip_download = False
 
 # You can configure the default columns displayed during the list command.
 config.commands.list_.default_columns = ["label", "title"]
 # You can specify whether filter matching should be performed case-insensitive.
 config.commands.list_.ignore_case = False
+# You can specify whether filter matching should decode all Unicode characters.
+config.commands.list_.decode_unicode = False
+# You can specify whether filter matching should decode all LaTeX sequences.
+config.commands.list_.decode_latex = False
+# You can specify the amount of fuzzy errors to allow for filter matching. Using this feature
+# requires the optional `regex` dependency to be installed.
+config.commands.list_.fuzziness = 0
 
 # You can specify whether associated files should be preserved when renaming during modifying.
 config.commands.modify.preserve_files = False
 
 # You can specify a custom command which will be used to `open` files associated with your entries.
 config.commands.open.command = "xdg-open" if sys.platform.lower() == "linux" else "open"
 # You can specify the names of the data fields which are to be checked for openable URLs.
@@ -73,17 +80,26 @@
 # associated files. The default tool (`grep`) will not provide results for attached PDFs but other
 # tools such as [ripgrep-all](https://github.com/phiresky/ripgrep-all) will.
 config.commands.search.grep = "grep"
 # If you want to specify additional arguments for your grep command, you can specify them as a list
 # of strings in the following setting. Note, that GNU's grep understands extended regex patterns
 # even without specifying `-E`.
 config.commands.search.grep_args = []
-
 # You can specify whether searches should be performed case-insensitive.
 config.commands.search.ignore_case = False
+# You can specify whether searches should decode all Unicode characters.
+config.commands.search.decode_unicode = False
+# You can specify whether searches should decode all LaTeX sequences.
+config.commands.search.decode_latex = False
+# You can specify the amount of fuzzy errors to allow for searches. Using this feature requires the
+# optional `regex` dependency to be installed.
+config.commands.search.fuzziness = 0
+
+# You can specify whether non-ASCII characters should be encoded using LaTeX sequences.
+config.commands.show.encode_latex = True
 
 
 # DATABASE
 # These settings affect the database in general.
 
 # You can specify the path to the database YAML file. You can use a `~` to represent your `$HOME`
 # directory.
@@ -99,14 +115,22 @@
 # Warning: Before enabling this setting you must ensure that you have set up git properly by setting
 # your name and email address.
 config.database.git = False
 
 # DATABASE.FORMAT
 # You can also specify some aspects about the format of the database.
 
+# You can specify how the `author` fields should be stored. The available options are provided by
+# the `AuthorFormat` Enum.
+#   - `AuthorFormat.YAML` (the default): this will split the author information into a list of
+#     author objects for which the first and last names as well as titles will each have their own
+#     field.
+#   - `AuthorField.BIBLATEX`: this will keep the author information as plain LaTeX.
+config.database.format.author_format = AuthorFormat.YAML
+
 # You can specify a default label format which will be used for the database entry keys. The format
 # of this option follows the f-string like formatting of modifications (see also the documentation
 # of the [ModifyCommand](https://cobib.gitlab.io/cobib/cobib/commands/modify.html)). The default
 # configuration value passes the originally provided label through
 # [text-unidecode](https://pypi.org/project/text-unidecode/) which replaces all Unicode symbols with
 # pure ASCII ones. A more useful example is
 #     `"{unidecode(author[0].last)}{year}"`
@@ -119,14 +143,18 @@
 # label from the enumerator and the second one is one of the enumerators provided in the
 # `config.LabelSuffix` object. The available enumerators are:
 #   - ALPHA: a, b, ...
 #   - CAPITAL: A, B, ...
 #   - NUMERIC: 1, 2, ...
 config.database.format.label_suffix = ("_", LabelSuffix.ALPHA)
 
+# You can specify which fields should be left verbatim and, thus, remain unaffected by any special
+# character conversions.
+config.database.format.verbatim_fields = ["file", "url"]
+
 # You can specify whether latex warnings should not be ignored during the escaping of special
 # characters. This is a simple option which gets passed on to the internally used `pylatexenc`
 # library.
 config.database.format.suppress_latex_warnings = True
 
 # DATABASE.STRINGIFY
 # You can customize the functions which convert non-string fields.
```

### Comparing `cobib-5.0.1/src/cobib/database/__init__.py` & `cobib-5.1.0/src/cobib/database/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/database/author.py` & `cobib-5.1.0/src/cobib/database/author.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/database/database.py` & `cobib-5.1.0/src/cobib/database/database.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/database/entry.py` & `cobib-5.1.0/src/cobib/database/entry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """coBib's Entry class."""
 
 from __future__ import annotations
 
 import logging
-import re
 import subprocess
+from itertools import accumulate
 from typing import TYPE_CHECKING, Any, List, Optional, cast
 
 from pylatexenc.latex2text import LatexNodes2Text
 from pylatexenc.latexencode import UnicodeToLatexEncoder
+from text_unidecode import unidecode
 
 from cobib.config import AuthorFormat, config
+from cobib.utils.match import Match, Span
+from cobib.utils.regex import HAS_OPTIONAL_REGEX, regex
 from cobib.utils.rel_path import RelPath
 
 from .author import Author
 
 if TYPE_CHECKING:
     import cobib.parsers
 
@@ -453,15 +456,22 @@
         if parser is None:
             from cobib.parsers.yaml import YAMLParser
 
             parser = YAMLParser()
         return parser.dump(formatted_entry) or ""  # `dump` may return `None`
 
     def matches(
-        self, filter_: dict[tuple[str, bool], list[str]], or_: bool, ignore_case: bool = False
+        self,
+        filter_: dict[tuple[str, bool], list[str]],
+        or_: bool,
+        *,
+        ignore_case: bool = False,
+        decode_unicode: bool = False,
+        decode_latex: bool = False,
+        fuzziness: int = 0,
     ) -> bool:
         """Check whether this entry matches the supplied filter.
 
         coBib provides an extensive filtering implementation. The filter is specified in the form
         of a dictionary whose keys consist of pairs of `(str, bool)` entries where the string
         indicates the field to match against and the boolean whether a positive (`true`) or negative
         (`false`) match is required. The values of the dictionary must be a `list[str]`. This means
@@ -480,87 +490,185 @@
         | `{('year', False): ['2020', '2021']}` | False    | `year` contains neither 2020 nor 2021 |
 
         Args:
             filter_: dictionary describing the filter as explained above.
             or_ : boolean indicating whether logical OR (`true`) or AND (`false`) is used to combine
                 multiple filter items.
             ignore_case: if True, the matching will be case-*in*sensitive.
+            decode_unicode: if True, all Unicode characters will be decoded before matching.
+            decode_latex: if True, all LaTeX sequences will be decoded before matching.
+            fuzziness: the amount of fuzzy errors to allow for matches. Using this feature requires
+                the optional `regex` dependency to be installed.
 
         Returns:
             Boolean indicating whether this entry matches the filter.
         """
         LOGGER.debug("Checking whether entry %s matches.", self.label)
-        re_flags = re.IGNORECASE if ignore_case else 0
+
+        if decode_latex:
+            dec = self._get_latex_to_text_decoder()
+
+        re_flags = regex.IGNORECASE if ignore_case else 0
+
         match_list = []
         stringified_data = self.stringify(encode_latex=False)
+
         for key, values in filter_.items():
             if key[0] not in stringified_data:
                 match_list.append(not key[1])
                 continue
+
+            field_data = stringified_data[key[0]]
+
+            if decode_latex:
+                field_data = dec.latex_to_text(field_data)
+
+            if decode_unicode:
+                field_data = unidecode(field_data)
+
             for val in values:
-                if re.search(rf"{val}", stringified_data[key[0]], flags=re_flags):
+                if fuzziness:
+                    re_compiled = regex.compile(rf"({val}){{e<={fuzziness}}}", flags=re_flags)
+                else:
+                    re_compiled = regex.compile(rf"{val}", flags=re_flags)
+
+                if re_compiled.search(field_data):
                     match_list.append(key[1])
                 else:
                     match_list.append(not key[1])
         if or_:
             return any(m for m in match_list)
         return all(m for m in match_list)
 
-    def search(
+    def search(  # noqa: PLR0912
         self,
         query: list[str],
+        *,
         context: int = 1,
-        ignore_case: bool = False,
         skip_files: bool = False,
-    ) -> list[list[str]]:
+        ignore_case: bool = False,
+        decode_unicode: bool = False,
+        decode_latex: bool = False,
+        fuzziness: int = 0,
+    ) -> list[Match]:
         """Search entry contents for the query strings.
 
         The entry will *always* be converted to a searchable string using the
-        `cobib.parsers.BibtexParser.dump` method. This text will then be search for each item in
-        `query` and will interpret these as regex patterns.
+        `cobib.parsers.BibtexParser.dump` method.
+
+        .. note::
+           Setting `decode_latex=True` and/or `decode_unicode=True` does *NOT* affect the output of
+           the above in order to ensure that the printed search results still include the original
+           LaTeX sequences and/or Unicode characters. Instead, only the internally searched string
+           will be decoded.
+
+        This text will then be search for each item in `query` and will interpret these as regex
+        patterns.
         If a `file` is associated with this entry, the search will try its best to recursively query
         its contents, too. However, the success of this depends highly on the configured search
         tool, `cobib.config.config.SearchCommandConfig.grep`.
 
         Args:
             query: the list of regex patterns to search for.
             context: the number of context lines to provide for each match. This behaves similarly
                 to the *Context Line Control* available for the UNIX `grep` command (`--context`).
-            ignore_case: if True, the search will be case-*in*sensitive.
             skip_files: if True, associated files will *not* be searched.
+            ignore_case: if True, the search will be case-*in*sensitive.
+            decode_unicode: if True, all Unicode characters will be decoded before search.
+            decode_latex: if True, all LaTeX sequences will be decoded before search.
+            fuzziness: the amount of fuzzy errors to allow for search matches. Using this feature
+                requires the optional `regex` dependency to be installed.
 
         Returns:
             A list of lists containing the context for each match associated with this entry.
         """
+        if fuzziness > 0 and not HAS_OPTIONAL_REGEX:  # pragma: no branch
+            LOGGER.warning(  # pragma: no cover
+                "Using the `fuzziness` option requires the optional `regex` dependency to be "
+                "installed! Falling back to `fuzziness=0`."
+            )
+
         LOGGER.debug("Searching entry %s.", self.label)
-        matches: list[list[str]] = []
+        matches: list[Match] = []
 
         from cobib.parsers.bibtex import BibtexParser
 
-        bibtex = BibtexParser(encode_latex=False).dump(self).split("\n")
-        re_flags = re.IGNORECASE if ignore_case else 0
+        # get searchable text
+        bibtex_raw = BibtexParser(encode_latex=False).dump(self)
+
+        # split into lines and compute their lengths and offsets
+        lines = bibtex_raw.split("\n")
+        line_lengths = [len(line) + 1 for line in lines]  # + 1 to account for the newline character
+        line_offsets = list(accumulate(line_lengths))
+
+        if decode_latex:
+            dec = self._get_latex_to_text_decoder()
+            bibtex_raw = dec.latex_to_text(bibtex_raw)
+
+        if decode_unicode:
+            bibtex_raw = unidecode(bibtex_raw)
+
+        re_flags = regex.IGNORECASE if ignore_case else 0
         for query_str in query:
-            re_compiled = re.compile(rf"{query_str}", flags=re_flags)
-            for idx, line in enumerate(bibtex):
-                if re_compiled.search(line):
-                    # add new match
-                    matches.append([])
-                    # upper context; (we iterate in reverse in order to ensure that we abort on the
-                    # first previous occurrence of the query pattern)
-                    for string in reversed(bibtex[max(idx - context, 0) : min(idx, len(bibtex))]):
-                        if re_compiled.search(string):
-                            break
-                        matches[-1].insert(0, string)
-                    # matching line itself
-                    matches[-1].append(line)
-                    # lower context
-                    for string in bibtex[max(idx + 1, 0) : min(idx + context + 1, len(bibtex))]:
-                        if re_compiled.search(string):
-                            break
-                        matches[-1].append(string)
+            if fuzziness:
+                re_compiled = regex.compile(rf"({query_str}){{e<={fuzziness}}}", flags=re_flags)
+            else:
+                re_compiled = regex.compile(rf"{query_str}", flags=re_flags)
+
+            # find all query matches
+            re_matches = list(re_compiled.finditer(bibtex_raw))
+
+            # determine line index for each match
+            matched_line_indices = []
+            for match_ in re_matches:
+                end = match_.span()[1]
+                for line_idx, offset in enumerate(line_offsets):
+                    if offset > end:
+                        matched_line_indices.append(line_idx)
+                        break
+
+            matched_line_indices_set = set(matched_line_indices)
+            prev_idx = 0
+            for idx, (match_, line_idx) in enumerate(zip(re_matches, matched_line_indices)):
+                try:
+                    next_idx = matched_line_indices[idx + 1]
+                except IndexError:
+                    next_idx = len(lines)
+
+                start = line_idx
+                # NOTE: we iterate in reverse in order to ensure that we abort on the first previous
+                # occurrence of the query pattern
+                for idx2 in reversed(
+                    range(
+                        max(line_idx - context, prev_idx),
+                        min(line_idx, next_idx),
+                    )
+                ):
+                    if idx2 in matched_line_indices_set:
+                        break
+                    start -= 1
+
+                stop = line_idx + 1
+                for idx2 in range(
+                    max(line_idx + 1, prev_idx),
+                    min(line_idx + context + 1, next_idx),
+                ):
+                    if idx2 in matched_line_indices_set:
+                        break
+                    stop += 1
+
+                offset = line_offsets[start - 1] if start > 0 else 0
+                matches.append(
+                    Match(
+                        "\n".join(lines[start:stop]),
+                        [Span(match_.start() - offset, match_.end() - offset)],
+                    )
+                )
+
+                prev_idx = line_idx
 
             if skip_files:
                 LOGGER.debug("Skipping the search in associated files of %s", self.label)
                 continue
 
             for file_ in self.file:
                 grep_prog = config.commands.search.grep
@@ -580,15 +688,19 @@
                         query_str,
                         RelPath(file_).path,
                     ],
                     stdout=subprocess.PIPE,
                 ) as grep:
                     if grep.stdout is None:
                         continue
-                    stdout = grep.stdout
-                    # extract results
-                    results = stdout.read().decode().split("\n--\n")
-                for match in results:
-                    if match:
-                        matches.append([line.strip() for line in match.split("\n") if line.strip()])
+                    stdout = grep.stdout.read().decode()
+                    if not stdout:
+                        continue
+
+                for file_match in stdout.split("\n--\n"):
+                    stripped = file_match.strip()
+                    file_matches = list(re_compiled.finditer(stripped))
+                    matches.append(
+                        Match(stripped, [Span(m.start(), m.end()) for m in file_matches])
+                    )
 
         return matches
```

### Comparing `cobib-5.0.1/src/cobib/importers/base_importer.py` & `cobib-5.1.0/src/cobib/importers/base_importer.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/importers/zotero.py` & `cobib-5.1.0/src/cobib/importers/zotero.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/parsers/__init__.py` & `cobib-5.1.0/src/cobib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/parsers/arxiv.py` & `cobib-5.1.0/src/cobib/parsers/arxiv.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/parsers/base_parser.py` & `cobib-5.1.0/src/cobib/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/parsers/bibtex.py` & `cobib-5.1.0/src/cobib/parsers/bibtex.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/parsers/doi.py` & `cobib-5.1.0/src/cobib/parsers/doi.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/parsers/isbn.py` & `cobib-5.1.0/src/cobib/parsers/isbn.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/parsers/url.py` & `cobib-5.1.0/src/cobib/parsers/url.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/parsers/yaml.py` & `cobib-5.1.0/src/cobib/parsers/yaml.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/cli.py` & `cobib-5.1.0/src/cobib/ui/cli.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/__init__.py` & `cobib-5.1.0/src/cobib/ui/components/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/entry_points.py` & `cobib-5.1.0/src/cobib/ui/components/entry_points.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/entry_view.py` & `cobib-5.1.0/src/cobib/ui/components/entry_view.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/help_screen.py` & `cobib-5.1.0/src/cobib/ui/components/help_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/input_screen.py` & `cobib-5.1.0/src/cobib/ui/components/input_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/list_view.py` & `cobib-5.1.0/src/cobib/ui/components/list_view.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/log_screen.py` & `cobib-5.1.0/src/cobib/ui/components/log_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/logging_handler.py` & `cobib-5.1.0/src/cobib/ui/components/logging_handler.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/main_content.py` & `cobib-5.1.0/src/cobib/ui/components/main_content.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/motion_key.py` & `cobib-5.1.0/src/cobib/ui/components/motion_key.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/preset_filter_screen.py` & `cobib-5.1.0/src/cobib/ui/components/preset_filter_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/search_view.py` & `cobib-5.1.0/src/cobib/ui/components/search_view.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/components/selection_filter.py` & `cobib-5.1.0/src/cobib/ui/components/selection_filter.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/tui.py` & `cobib-5.1.0/src/cobib/ui/tui.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/ui/ui.py` & `cobib-5.1.0/src/cobib/ui/ui.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/utils/diff_renderer.py` & `cobib-5.1.0/src/cobib/utils/diff_renderer.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/utils/file_downloader.py` & `cobib-5.1.0/src/cobib/utils/file_downloader.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/utils/journal_abbreviations.py` & `cobib-5.1.0/src/cobib/utils/journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/utils/logging.py` & `cobib-5.1.0/src/cobib/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/utils/progress.py` & `cobib-5.1.0/src/cobib/utils/progress.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/utils/prompt.py` & `cobib-5.1.0/src/cobib/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib/utils/rel_path.py` & `cobib-5.1.0/src/cobib/utils/rel_path.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/src/cobib.egg-info/PKG-INFO` & `cobib-5.1.0/src/cobib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 5.0.1
+Version: 5.1.0
 Summary: Console Bibliography
 Author-email: Max Rossmannek <max@rossmannek.de>
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/cobib/cobib
 Project-URL: Documentation, https://cobib.gitlab.io/cobib/cobib.html
 Project-URL: Repository, https://gitlab.com/cobib/cobib
 Project-URL: Issues, https://gitlab.com/cobib/cobib/-/issues
@@ -29,14 +29,18 @@
 Requires-Dist: requests
 Requires-Dist: requests_oauthlib
 Requires-Dist: rich
 Requires-Dist: ruamel.yaml
 Requires-Dist: textual>=0.48
 Requires-Dist: typing_extensions
 Requires-Dist: text-unidecode
+Provides-Extra: all
+Requires-Dist: cobib[fuzzy]; extra == "all"
+Provides-Extra: fuzzy
+Requires-Dist: regex; extra == "fuzzy"
 
 [![coBib](https://gitlab.com/cobib/cobib/-/raw/master/logo/cobib_logo.svg)](https://cobib.gitlab.io/cobib/cobib.html)
 
 # coBib
 
 [![pipeline](https://gitlab.com/cobib/cobib/badges/master/pipeline.svg)](https://gitlab.com/cobib/cobib/-/pipelines)
 [![coverage](https://gitlab.com/cobib/cobib/badges/master/coverage.svg)](https://gitlab.com/cobib/cobib/-/graphs/master/charts)
@@ -307,14 +311,47 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [5.1.0] - 2024-05-28
+
+Pypi: https://pypi.org/project/cobib/5.1.0/
+
+### Prelude
+
+Check out my blog post to learn more about the features of this new release:
+https://mrossinek.gitlab.io/programming/cobib-becomes-fuzzy/
+
+### Added
+- approximate (or fuzzy) filter matching and search functionality (#107,#130,!177)
+  - the `list` and `search` commands now support the following features to
+    perform approximate filter matching and searching, respectively:
+    - LaTeX sequences can be decoded to Unicode characters:
+      - using `--decode-latex` from the command-line
+      - setting `config.commands.list_.decode_latex = True`
+      - setting `config.commands.search.decode_latex = True`
+    - Unicode characters can be converted to a close ASCII equivalent:
+      - using `--decode-unicode` from the command-line
+      - setting `config.commands.list_.decode_unicode = True`
+      - setting `config.commands.search.decode_unicode = True`
+    - a number of fuzzy errors can be set (this requires the optional dependency
+      [`regex`](https://pypi.org/project/regex/) to be installed):
+      - using `--fuzziness <int>` from the command-line
+      - setting `config.commands.list_.fuzzines` to some integer
+      - setting `config.commands.search.fuzzines` to some integer
+- (DEV) the following method arguments have been converted to be accepted only
+  as keyword arguments:
+  - in `cobib.database.Entry.matches`: `ignore_case`
+  - in `cobib.database.Entry.search`: `context`, `ignore_case`, and `skip_files`
+- (DEV) the return-type of `cobib.database.Entry.search` has been changed
+
+
 ## [5.0.1] - 2024-05-01
 
 Pypi: https://pypi.org/project/cobib/5.0.1/
 
 ### Fixed
 - the ability to use an empty string as the separator in `config.database.format.label_suffix` (#138)
 
@@ -1300,15 +1337,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.0.1...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.1.0...master
+[5.1.0]: https://gitlab.com/cobib/cobib/-/tags/v5.1.0
 [5.0.1]: https://gitlab.com/cobib/cobib/-/tags/v5.0.1
 [5.0.0]: https://gitlab.com/cobib/cobib/-/tags/v5.0.0
 [4.5.0]: https://gitlab.com/cobib/cobib/-/tags/v4.5.0
 [4.4.0]: https://gitlab.com/cobib/cobib/-/tags/v4.4.0
 [4.3.1]: https://gitlab.com/cobib/cobib/-/tags/v4.3.1
 [4.3.0]: https://gitlab.com/cobib/cobib/-/tags/v4.3.0
 [4.2.0]: https://gitlab.com/cobib/cobib/-/tags/v4.2.0
```

### Comparing `cobib-5.0.1/src/cobib.egg-info/SOURCES.txt` & `cobib-5.1.0/src/cobib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -72,11 +72,13 @@
 src/cobib/ui/components/selection_filter.py
 src/cobib/utils/__init__.py
 src/cobib/utils/context.py
 src/cobib/utils/diff_renderer.py
 src/cobib/utils/file_downloader.py
 src/cobib/utils/journal_abbreviations.py
 src/cobib/utils/logging.py
+src/cobib/utils/match.py
 src/cobib/utils/progress.py
 src/cobib/utils/prompt.py
+src/cobib/utils/regex.py
 src/cobib/utils/rel_path.py
 tests/test_main.py
```

### Comparing `cobib-5.0.1/src/cobib.egg-info/entry_points.txt` & `cobib-5.1.0/src/cobib.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cobib-5.0.1/tests/test_main.py` & `cobib-5.1.0/tests/test_main.py`

 * *Files identical despite different names*

