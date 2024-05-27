# Comparing `tmp/cli-chess-1.1.1.tar.gz` & `tmp/cli_chess-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-chess-1.1.1.tar", last modified: Sat Nov  4 22:09:57 2023, max compression
+gzip compressed data, was "cli_chess-1.2.0.tar", last modified: Mon May 27 23:27:31 2024, max compression
```

## Comparing `cli-chess-1.1.1.tar` & `cli_chess-1.2.0.tar`

### file list

```diff
@@ -1,171 +1,176 @@
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.283502 cli-chess-1.1.1/
--rw-r--r--   0 trevor    (1000) trevor    (1000)    35823 2023-11-04 22:08:06.000000 cli-chess-1.1.1/LICENSE
--rw-r--r--   0 trevor    (1000) trevor    (1000)      118 2023-11-04 22:08:06.000000 cli-chess-1.1.1/MANIFEST.in
--rw-r--r--   0 trevor    (1000) trevor    (1000)     7635 2023-11-04 22:09:57.283502 cli-chess-1.1.1/PKG-INFO
--rw-r--r--   0 trevor    (1000) trevor    (1000)     6420 2023-11-04 22:08:06.000000 cli-chess-1.1.1/README.md
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1243 2023-11-04 22:09:57.283502 cli-chess-1.1.1/setup.cfg
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1723 2023-11-04 22:08:06.000000 cli-chess-1.1.1/setup.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.273502 cli-chess-1.1.1/src/
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.273502 cli-chess-1.1.1/src/cli_chess/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      334 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)      886 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/__main__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)      981 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/__metadata__.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.273502 cli-chess-1.1.1/src/cli_chess/core/
--rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/__init__.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.273502 cli-chess-1.1.1/src/cli_chess/core/api/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      212 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/api/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1815 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/api/api_manager.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     4847 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/api/game_state_dispatcher.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     3737 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/api/incoming_event_manger.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.273502 cli-chess-1.1.1/src/cli_chess/core/game/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      340 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     5262 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/game_model_base.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     5173 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/game_options.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     5224 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/game_presenter_base.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     7365 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/game_view_base.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.273502 cli-chess-1.1.1/src/cli_chess/core/game/offline_game/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      153 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/offline_game/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     5868 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/offline_game/offline_game_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     6855 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/offline_game/offline_game_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2082 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/offline_game/offline_game_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.273502 cli-chess-1.1.1/src/cli_chess/core/game/online_game/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      147 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/online_game/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)    15699 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/online_game/online_game_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     5512 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/online_game/online_game_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2130 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/online_game/online_game_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.273502 cli-chess-1.1.1/src/cli_chess/core/game/online_game/watch_tv/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      148 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/online_game/watch_tv/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)    12487 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/online_game/watch_tv/watch_tv_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2092 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/online_game/watch_tv/watch_tv_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     3454 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/game/online_game/watch_tv/watch_tv_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/core/main/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      108 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/main/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1583 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/main/main_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2173 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/main/main_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     7279 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/core/main/main_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/menus/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      398 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/__init__.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/menus/main_menu/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      152 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/main_menu/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1572 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/main_menu/main_menu_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1878 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/main_menu/main_menu_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     6506 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/main_menu/main_menu_view.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2964 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/menu_common.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1729 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/menu_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     3790 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/menu_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     6996 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/menu_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/menus/offline_games_menu/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      211 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/offline_games_menu/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1296 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/offline_games_menu/offline_games_menu_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1459 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/offline_games_menu/offline_games_menu_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     3007 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/offline_games_menu/offline_games_menu_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/menus/online_games_menu/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      204 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/online_games_menu/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1606 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/online_games_menu/online_games_menu_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1769 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/online_games_menu/online_games_menu_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     4611 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/online_games_menu/online_games_menu_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/menus/program_settings_menu/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      204 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/program_settings_menu/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     4318 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/program_settings_menu/program_settings_menu_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2173 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/program_settings_menu/program_settings_menu_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1150 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/program_settings_menu/program_settings_menu_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/menus/settings_menu/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      180 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/settings_menu/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1514 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/settings_menu/settings_menu_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1648 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/settings_menu/settings_menu_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     3285 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/settings_menu/settings_menu_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/menus/tv_channel_menu/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      190 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/tv_channel_menu/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2660 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1392 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2517 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/menus/versus_menus/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      272 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/versus_menus/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     4932 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/versus_menus/versus_menu_models.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     4356 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/versus_menus/versus_menu_presenters.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1950 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/menus/versus_menus/versus_menu_views.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/modules/
--rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/__init__.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/modules/about/
--rw-r--r--   0 trevor    (1000) trevor    (1000)       78 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/about/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1377 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/about/about_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     3834 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/about/about_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/modules/board/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      114 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/board/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)    14280 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/board/board_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     8009 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/board/board_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2807 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/board/board_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/modules/clock/
--rw-r--r--   0 trevor    (1000) trevor    (1000)       78 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/clock/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2500 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/clock/clock_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1601 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/clock/clock_view.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1261 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/common.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.276836 cli-chess-1.1.1/src/cli_chess/modules/engine/
--rw-r--r--   0 trevor    (1000) trevor    (1000)       84 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/engine/__init__.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.280169 cli-chess-1.1.1/src/cli_chess/modules/engine/binaries/
--rwxr-xr-x   0 trevor    (1000) trevor    (1000)   697544 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_arm64_macos
--rwxr-xr-x   0 trevor    (1000) trevor    (1000)   797928 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_linux
--rwxr-xr-x   0 trevor    (1000) trevor    (1000)   761256 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_macos
--rwxr-xr-x   0 trevor    (1000) trevor    (1000)  1916430 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_windows.exe
--rw-r--r--   0 trevor    (1000) trevor    (1000)     4496 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/engine/engine_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1395 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/engine/engine_presenter.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.280169 cli-chess-1.1.1/src/cli_chess/modules/material_difference/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      195 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/material_difference/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     6343 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/material_difference/material_difference_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     4246 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/material_difference/material_difference_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2506 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/material_difference/material_difference_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.280169 cli-chess-1.1.1/src/cli_chess/modules/move_list/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      135 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/move_list/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     3214 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/move_list/move_list_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     3345 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/move_list/move_list_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     3680 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/move_list/move_list_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.280169 cli-chess-1.1.1/src/cli_chess/modules/player_info/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      100 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/player_info/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1864 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/player_info/player_info_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     4083 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/player_info/player_info_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.283502 cli-chess-1.1.1/src/cli_chess/modules/token_manager/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      159 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/token_manager/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     5371 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/token_manager/token_manager_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2060 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/token_manager/token_manager_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     4844 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/modules/token_manager/token_manager_view.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.283502 cli-chess-1.1.1/src/cli_chess/tests/
--rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/__init__.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.283502 cli-chess-1.1.1/src/cli_chess/tests/modules/
--rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/__init__.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.283502 cli-chess-1.1.1/src/cli_chess/tests/modules/board/
--rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/board/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)    14892 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/board/test_board_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)    11841 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/board/test_board_presenter.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.283502 cli-chess-1.1.1/src/cli_chess/tests/modules/material_difference/
--rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/material_difference/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     6963 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/material_difference/test_material_difference_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     5369 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/material_difference/test_material_difference_presenter.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.283502 cli-chess-1.1.1/src/cli_chess/tests/modules/move_list/
--rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/move_list/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     4431 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/move_list/test_move_list_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     5772 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/move_list/test_move_list_presenter.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1333 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/test_common.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.283502 cli-chess-1.1.1/src/cli_chess/tests/modules/token_manager/
--rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/token_manager/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     4407 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/token_manager/test_token_manager_model.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     1974 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/modules/token_manager/test_token_manager_presenter.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.283502 cli-chess-1.1.1/src/cli_chess/tests/utils/
--rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/utils/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     4421 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/tests/utils/test_event.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.283502 cli-chess-1.1.1/src/cli_chess/utils/
--rw-r--r--   0 trevor    (1000) trevor    (1000)      395 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/utils/__init__.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2906 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/utils/argparse.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     3931 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/utils/common.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)    14905 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/utils/config.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2804 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/utils/event.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2191 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/utils/logging.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     2804 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/utils/styles.py
--rw-r--r--   0 trevor    (1000) trevor    (1000)     6549 2023-11-04 22:08:06.000000 cli-chess-1.1.1/src/cli_chess/utils/ui_common.py
-drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2023-11-04 22:09:57.273502 cli-chess-1.1.1/src/cli_chess.egg-info/
--rw-r--r--   0 trevor    (1000) trevor    (1000)     7635 2023-11-04 22:09:57.000000 cli-chess-1.1.1/src/cli_chess.egg-info/PKG-INFO
--rw-r--r--   0 trevor    (1000) trevor    (1000)     6424 2023-11-04 22:09:57.000000 cli-chess-1.1.1/src/cli_chess.egg-info/SOURCES.txt
--rw-r--r--   0 trevor    (1000) trevor    (1000)        1 2023-11-04 22:09:57.000000 cli-chess-1.1.1/src/cli_chess.egg-info/dependency_links.txt
--rw-r--r--   0 trevor    (1000) trevor    (1000)       54 2023-11-04 22:09:57.000000 cli-chess-1.1.1/src/cli_chess.egg-info/entry_points.txt
--rw-r--r--   0 trevor    (1000) trevor    (1000)        1 2023-11-04 22:09:57.000000 cli-chess-1.1.1/src/cli_chess.egg-info/not-zip-safe
--rw-r--r--   0 trevor    (1000) trevor    (1000)      187 2023-11-04 22:09:57.000000 cli-chess-1.1.1/src/cli_chess.egg-info/requires.txt
--rw-r--r--   0 trevor    (1000) trevor    (1000)       10 2023-11-04 22:09:57.000000 cli-chess-1.1.1/src/cli_chess.egg-info/top_level.txt
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.416803 cli_chess-1.2.0/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)    35823 2023-08-21 16:39:29.000000 cli_chess-1.2.0/LICENSE
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      118 2023-08-21 16:39:29.000000 cli_chess-1.2.0/MANIFEST.in
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     8015 2024-05-27 23:27:31.416803 cli_chess-1.2.0/PKG-INFO
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     6420 2023-09-01 17:06:39.000000 cli_chess-1.2.0/README.md
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1243 2024-05-27 23:27:31.416803 cli_chess-1.2.0/setup.cfg
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1723 2024-05-27 23:14:22.000000 cli_chess-1.2.0/setup.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.403470 cli_chess-1.2.0/src/
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.406803 cli_chess-1.2.0/src/cli_chess/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      334 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      886 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/__main__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      981 2024-05-27 23:12:56.000000 cli_chess-1.2.0/src/cli_chess/__metadata__.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.406803 cli_chess-1.2.0/src/cli_chess/core/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/__init__.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.406803 cli_chess-1.2.0/src/cli_chess/core/api/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      212 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/api/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1815 2023-09-01 15:55:57.000000 cli_chess-1.2.0/src/cli_chess/core/api/api_manager.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     4847 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/api/game_state_dispatcher.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     3737 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/api/incoming_event_manger.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.406803 cli_chess-1.2.0/src/cli_chess/core/game/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      340 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/game/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     5520 2024-05-27 23:03:36.000000 cli_chess-1.2.0/src/cli_chess/core/game/game_model_base.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     5173 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/game/game_options.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     5749 2024-05-27 23:03:36.000000 cli_chess-1.2.0/src/cli_chess/core/game/game_presenter_base.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     9423 2024-05-27 23:03:36.000000 cli_chess-1.2.0/src/cli_chess/core/game/game_view_base.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.406803 cli_chess-1.2.0/src/cli_chess/core/game/offline_game/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      153 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/game/offline_game/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     5986 2024-05-27 23:03:36.000000 cli_chess-1.2.0/src/cli_chess/core/game/offline_game/offline_game_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     7268 2024-05-27 23:03:36.000000 cli_chess-1.2.0/src/cli_chess/core/game/offline_game/offline_game_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2122 2024-05-24 22:15:23.000000 cli_chess-1.2.0/src/cli_chess/core/game/offline_game/offline_game_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.406803 cli_chess-1.2.0/src/cli_chess/core/game/online_game/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      147 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/game/online_game/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)    16407 2024-05-27 23:03:36.000000 cli_chess-1.2.0/src/cli_chess/core/game/online_game/online_game_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     5701 2024-05-27 23:03:36.000000 cli_chess-1.2.0/src/cli_chess/core/game/online_game/online_game_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2170 2024-05-26 18:24:12.000000 cli_chess-1.2.0/src/cli_chess/core/game/online_game/online_game_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.406803 cli_chess-1.2.0/src/cli_chess/core/game/online_game/watch_tv/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      148 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/game/online_game/watch_tv/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)    12487 2023-08-29 20:52:44.000000 cli_chess-1.2.0/src/cli_chess/core/game/online_game/watch_tv/watch_tv_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2092 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/game/online_game/watch_tv/watch_tv_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2233 2024-05-26 18:24:18.000000 cli_chess-1.2.0/src/cli_chess/core/game/online_game/watch_tv/watch_tv_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.406803 cli_chess-1.2.0/src/cli_chess/core/main/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      108 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/main/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1583 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/main/main_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2173 2023-09-01 16:40:54.000000 cli_chess-1.2.0/src/cli_chess/core/main/main_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     7279 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/core/main/main_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.406803 cli_chess-1.2.0/src/cli_chess/menus/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      398 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/__init__.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.406803 cli_chess-1.2.0/src/cli_chess/menus/main_menu/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      152 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/main_menu/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1572 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/main_menu/main_menu_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1878 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/main_menu/main_menu_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     6506 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/main_menu/main_menu_view.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2964 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/menu_common.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1729 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/menu_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     3790 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/menu_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     6996 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/menu_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.410137 cli_chess-1.2.0/src/cli_chess/menus/offline_games_menu/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      211 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/offline_games_menu/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1296 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/offline_games_menu/offline_games_menu_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1459 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/offline_games_menu/offline_games_menu_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     3007 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/offline_games_menu/offline_games_menu_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.410137 cli_chess-1.2.0/src/cli_chess/menus/online_games_menu/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      204 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/online_games_menu/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1606 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/online_games_menu/online_games_menu_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1769 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/online_games_menu/online_games_menu_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     4611 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/online_games_menu/online_games_menu_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.410137 cli_chess-1.2.0/src/cli_chess/menus/program_settings_menu/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      204 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/program_settings_menu/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     4318 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/program_settings_menu/program_settings_menu_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2173 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/program_settings_menu/program_settings_menu_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1150 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/program_settings_menu/program_settings_menu_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.410137 cli_chess-1.2.0/src/cli_chess/menus/settings_menu/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      180 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/settings_menu/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1514 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/settings_menu/settings_menu_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1648 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/settings_menu/settings_menu_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     3285 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/settings_menu/settings_menu_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.410137 cli_chess-1.2.0/src/cli_chess/menus/tv_channel_menu/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      190 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/tv_channel_menu/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2660 2023-08-29 20:54:07.000000 cli_chess-1.2.0/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1392 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2517 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.410137 cli_chess-1.2.0/src/cli_chess/menus/versus_menus/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      272 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/versus_menus/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     4932 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/versus_menus/versus_menu_models.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     4356 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/versus_menus/versus_menu_presenters.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1950 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/menus/versus_menus/versus_menu_views.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.410137 cli_chess-1.2.0/src/cli_chess/modules/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/__init__.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.410137 cli_chess-1.2.0/src/cli_chess/modules/about/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)       78 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/about/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1377 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/about/about_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     3834 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/about/about_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.410137 cli_chess-1.2.0/src/cli_chess/modules/board/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      114 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/board/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)    15117 2024-05-27 23:03:36.000000 cli_chess-1.2.0/src/cli_chess/modules/board/board_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     8244 2024-05-27 23:03:36.000000 cli_chess-1.2.0/src/cli_chess/modules/board/board_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2807 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/board/board_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.410137 cli_chess-1.2.0/src/cli_chess/modules/clock/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)       78 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/clock/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2500 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/clock/clock_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1601 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/clock/clock_view.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1261 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/common.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.410137 cli_chess-1.2.0/src/cli_chess/modules/engine/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)       84 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/engine/__init__.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.413470 cli_chess-1.2.0/src/cli_chess/modules/engine/binaries/
+-rwxr-xr-x   0 trevor    (1000) trevor    (1000)   697544 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_arm64_macos
+-rwxr-xr-x   0 trevor    (1000) trevor    (1000)   797928 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_linux
+-rwxr-xr-x   0 trevor    (1000) trevor    (1000)   761256 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_macos
+-rwxr-xr-x   0 trevor    (1000) trevor    (1000)  1916430 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_windows.exe
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     4496 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/engine/engine_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1395 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/engine/engine_presenter.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.413470 cli_chess-1.2.0/src/cli_chess/modules/material_difference/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      195 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/material_difference/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     6343 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/material_difference/material_difference_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     4246 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/material_difference/material_difference_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2506 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/material_difference/material_difference_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.413470 cli_chess-1.2.0/src/cli_chess/modules/move_list/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      135 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/move_list/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     3214 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/move_list/move_list_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     3345 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/move_list/move_list_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     3442 2024-05-24 21:29:11.000000 cli_chess-1.2.0/src/cli_chess/modules/move_list/move_list_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.413470 cli_chess-1.2.0/src/cli_chess/modules/player_info/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      100 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/player_info/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1864 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/player_info/player_info_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     4083 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/player_info/player_info_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.413470 cli_chess-1.2.0/src/cli_chess/modules/premove/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      126 2024-05-27 23:03:36.000000 cli_chess-1.2.0/src/cli_chess/modules/premove/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     3855 2024-05-27 23:03:36.000000 cli_chess-1.2.0/src/cli_chess/modules/premove/premove_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1698 2024-05-27 23:03:36.000000 cli_chess-1.2.0/src/cli_chess/modules/premove/premove_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2197 2024-05-26 18:30:22.000000 cli_chess-1.2.0/src/cli_chess/modules/premove/premove_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.413470 cli_chess-1.2.0/src/cli_chess/modules/token_manager/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      159 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/token_manager/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     5371 2023-09-01 16:46:48.000000 cli_chess-1.2.0/src/cli_chess/modules/token_manager/token_manager_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2060 2023-09-01 15:43:27.000000 cli_chess-1.2.0/src/cli_chess/modules/token_manager/token_manager_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     4844 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/modules/token_manager/token_manager_view.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.413470 cli_chess-1.2.0/src/cli_chess/tests/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/__init__.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.413470 cli_chess-1.2.0/src/cli_chess/tests/modules/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/__init__.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.413470 cli_chess-1.2.0/src/cli_chess/tests/modules/board/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/board/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)    14892 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/board/test_board_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)    11841 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/board/test_board_presenter.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.413470 cli_chess-1.2.0/src/cli_chess/tests/modules/material_difference/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/material_difference/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     6963 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/material_difference/test_material_difference_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     5369 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/material_difference/test_material_difference_presenter.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.416803 cli_chess-1.2.0/src/cli_chess/tests/modules/move_list/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/move_list/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     4431 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/move_list/test_move_list_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     5772 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/move_list/test_move_list_presenter.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1333 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/test_common.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.416803 cli_chess-1.2.0/src/cli_chess/tests/modules/token_manager/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/token_manager/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     4407 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/token_manager/test_token_manager_model.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     1974 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/modules/token_manager/test_token_manager_presenter.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.416803 cli_chess-1.2.0/src/cli_chess/tests/utils/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)        0 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/utils/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     4421 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/tests/utils/test_event.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.416803 cli_chess-1.2.0/src/cli_chess/utils/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      395 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/utils/__init__.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2906 2023-09-01 16:48:17.000000 cli_chess-1.2.0/src/cli_chess/utils/argparse.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     3931 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/utils/common.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)    14905 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/utils/config.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2804 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/utils/event.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2191 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/utils/logging.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     2946 2024-05-22 20:52:29.000000 cli_chess-1.2.0/src/cli_chess/utils/styles.py
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     6549 2023-08-21 16:39:29.000000 cli_chess-1.2.0/src/cli_chess/utils/ui_common.py
+drwxr-xr-x   0 trevor    (1000) trevor    (1000)        0 2024-05-27 23:27:31.416803 cli_chess-1.2.0/src/cli_chess.egg-info/
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     8015 2024-05-27 23:27:31.000000 cli_chess-1.2.0/src/cli_chess.egg-info/PKG-INFO
+-rw-r--r--   0 trevor    (1000) trevor    (1000)     6610 2024-05-27 23:27:31.000000 cli_chess-1.2.0/src/cli_chess.egg-info/SOURCES.txt
+-rw-r--r--   0 trevor    (1000) trevor    (1000)        1 2024-05-27 23:27:31.000000 cli_chess-1.2.0/src/cli_chess.egg-info/dependency_links.txt
+-rw-r--r--   0 trevor    (1000) trevor    (1000)       54 2024-05-27 23:27:31.000000 cli_chess-1.2.0/src/cli_chess.egg-info/entry_points.txt
+-rw-r--r--   0 trevor    (1000) trevor    (1000)        1 2023-08-21 16:42:22.000000 cli_chess-1.2.0/src/cli_chess.egg-info/not-zip-safe
+-rw-r--r--   0 trevor    (1000) trevor    (1000)      187 2024-05-27 23:27:31.000000 cli_chess-1.2.0/src/cli_chess.egg-info/requires.txt
+-rw-r--r--   0 trevor    (1000) trevor    (1000)       10 2024-05-27 23:27:31.000000 cli_chess-1.2.0/src/cli_chess.egg-info/top_level.txt
```

### Comparing `cli-chess-1.1.1/LICENSE` & `cli_chess-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/PKG-INFO` & `cli_chess-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-chess
-Version: 1.1.1
+Version: 1.2.0
 Summary: A highly customizable way to play chess in your terminal
 Home-page: https://github.com/trevorbayless/cli-chess
 Author: Trevor Bayless
 Author-email: trevorbayless1@gmail.com
 License: GPL-3.0+
 Keywords: chess,terminal,fairy-stockfish,stockfish,lichess,lichess.org,cli,san,uci
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -20,16 +20,24 @@
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: chess<2.0.0,>=1.9.4
+Requires-Dist: berserk<0.14.0,>=0.13.1
+Requires-Dist: prompt-toolkit==3.0.44
+Provides-Extra: dev
+Requires-Dist: pytest<8.0.0,>=7.2.1; extra == "dev"
+Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == "dev"
+Requires-Dist: pytest-socket<1.0.0,>=0.6.0; extra == "dev"
+Requires-Dist: flake8<7.0.0,>=5.0.4; extra == "dev"
+Requires-Dist: vulture<3.0,>=2.7; extra == "dev"
 
 <p align="center">
   <a href="#"><img src="https://user-images.githubusercontent.com/3620552/214357735-53c2174c-5ada-45a2-97cb-6a25b5ca9c0c.png"/></a>
 </p>
 
 <p align="center">
 A highly customizable way to play chess in your terminal. Supports playing online (via Lichess.org) and
```

#### html2text {}

```diff
@@ -1,24 +1,29 @@
-Metadata-Version: 2.1 Name: cli-chess Version: 1.1.1 Summary: A highly
+Metadata-Version: 2.1 Name: cli-chess Version: 1.2.0 Summary: A highly
 customizable way to play chess in your terminal Home-page: https://github.com/
 trevorbayless/cli-chess Author: Trevor Bayless Author-email:
 trevorbayless1@gmail.com License: GPL-3.0+ Keywords: chess,terminal,fairy-
 stockfish,stockfish,lichess,lichess.org,cli,san,uci Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: Microsoft ::
 Windows Classifier: Operating System :: MacOS Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Games/Entertainment
 :: Board Games Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Requires-Python:
->=3.8 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE
+>=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: chess<2.0.0,>=1.9.4 Requires-Dist: berserk<0.14.0,>=0.13.1 Requires-Dist:
+prompt-toolkit==3.0.44 Provides-Extra: dev Requires-Dist: pytest<8.0.0,>=7.2.1;
+extra == "dev" Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == "dev"
+Requires-Dist: pytest-socket<1.0.0,>=0.6.0; extra == "dev" Requires-Dist:
+flake8<7.0.0,>=5.0.4; extra == "dev" Requires-Dist: vulture<3.0,>=2.7; extra ==
+"dev"
   _[_h_t_t_p_s_:_/_/_u_s_e_r_-_i_m_a_g_e_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_3_6_2_0_5_5_2_/_2_1_4_3_5_7_7_3_5_-_5_3_c_2_1_7_4_c_-_5_a_d_a_-
                           _4_5_a_2_-_9_7_c_b_-_6_a_2_5_b_5_c_a_9_c_0_c_._p_n_g_]
   A highly customizable way to play chess in your terminal. Supports playing
  online (via Lichess.org) and offline against the Fairy-Stockfish engine. All
                         Lichess variants are supported.
                           _[_C_I_ _W_o_r_k_f_l_o_w_]_[_P_y_P_I_]_[_P_y_t_h_o_n_]
 Demo Offline against Fairy-Stockfish | Watching Lichess Bullet TV :------------
```

### Comparing `cli-chess-1.1.1/README.md` & `cli_chess-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/setup.cfg` & `cli_chess-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/setup.py` & `cli_chess-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2024 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -18,15 +18,15 @@
 
 metadata_file = open("src/cli_chess/__metadata__.py").read()
 metadata = dict(findall(r'__(\w*)__\s*=\s*"([^"]+)"', metadata_file))
 
 dependencies = [
     "chess>=1.9.4,<2.0.0",
     "berserk>=0.13.1,<0.14.0",
-    "prompt-toolkit==3.0.39"  # pin as breaking changes have been
+    "prompt-toolkit==3.0.44"  # pin as breaking changes have been
                               # introduced in previous patch versions
                               # read PT changelog before bumping
 ]
 
 dev_dependencies = {
     'dev': [
         'pytest>=7.2.1,<8.0.0',
```

### Comparing `cli-chess-1.1.1/src/cli_chess/__main__.py` & `cli_chess-1.2.0/src/cli_chess/__main__.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/__metadata__.py` & `cli_chess-1.2.0/src/cli_chess/__metadata__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2024 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,13 +10,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 __name__ = "cli-chess"
-__version__ = "1.1.1"
+__version__ = "1.2.0"
 __description__ = "A highly customizable way to play chess in your terminal"
 __url__ = "https://github.com/trevorbayless/cli-chess"
 __author__ = "Trevor Bayless"
 __author_email__ = "trevorbayless1@gmail.com"
 __license__ = "GPL-3.0+"
```

### Comparing `cli-chess-1.1.1/src/cli_chess/core/api/api_manager.py` & `cli_chess-1.2.0/src/cli_chess/core/api/api_manager.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/core/api/game_state_dispatcher.py` & `cli_chess-1.2.0/src/cli_chess/core/api/game_state_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/core/api/incoming_event_manger.py` & `cli_chess-1.2.0/src/cli_chess/core/api/incoming_event_manger.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/core/game/game_model_base.py` & `cli_chess-1.2.0/src/cli_chess/core/game/game_model_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2024 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,14 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from cli_chess.modules.board import BoardModel
 from cli_chess.modules.move_list import MoveListModel
 from cli_chess.modules.material_difference import MaterialDifferenceModel
+from cli_chess.modules.premove import PremoveModel
 from cli_chess.utils import EventManager, log
 from chess import Color, WHITE, COLOR_NAMES
 from random import getrandbits
 from abc import ABC, abstractmethod
 
 
 class GameModelBase:
@@ -105,15 +106,18 @@
         }
 
 
 class PlayableGameModelBase(GameModelBase, ABC):
     def __init__(self, play_as_color: str, variant="standard", fen=""):
         self.my_color = self._get_side_to_play_as(play_as_color)
         self.game_in_progress = False
+
         super().__init__(orientation=self.my_color, variant=variant, fen=fen)
+        self.premove_model = PremoveModel(self.board_model)
+        self._assoc_models = self._assoc_models + [self.premove_model]
 
     def is_my_turn(self) -> bool:
         """Return True if it's our turn"""
         return self.board_model.get_turn() == self.my_color
 
     @staticmethod
     def _get_side_to_play_as(color: str) -> Color:
@@ -126,14 +130,18 @@
             return Color(getrandbits(1))
 
     @abstractmethod
     def make_move(self, move: str) -> None:
         pass
 
     @abstractmethod
+    def set_premove(self, move) -> None:
+        pass
+
+    @abstractmethod
     def propose_takeback(self) -> None:
         pass
 
     @abstractmethod
     def offer_draw(self) -> None:
         pass
```

### Comparing `cli-chess-1.1.1/src/cli_chess/core/game/game_options.py` & `cli_chess-1.2.0/src/cli_chess/core/game/game_options.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/core/game/game_presenter_base.py` & `cli_chess-1.2.0/src/cli_chess/core/game/game_presenter_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2024 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -16,14 +16,15 @@
 from __future__ import annotations
 from cli_chess.core.game import GameViewBase, PlayableGameViewBase
 from cli_chess.modules.board import BoardPresenter
 from cli_chess.modules.move_list import MoveListPresenter
 from cli_chess.modules.material_difference import MaterialDifferencePresenter
 from cli_chess.modules.player_info import PlayerInfoPresenter
 from cli_chess.modules.clock import ClockPresenter
+from cli_chess.modules.premove import PremovePresenter
 from cli_chess.utils import log, AlertType, RequestSuccessfullySent
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from cli_chess.core.game import GameModelBase, PlayableGameModelBase
 
 
@@ -61,40 +62,53 @@
         log.debug("Exiting game presenter")
         self.model.cleanup()
         self.view.exit()
 
 
 class PlayableGamePresenterBase(GamePresenterBase, ABC):
     def __init__(self, model: PlayableGameModelBase):
+        self.premove_presenter = PremovePresenter(model.premove_model)
         super().__init__(model)
         self.model = model
 
     @abstractmethod
     def _get_view(self) -> PlayableGameViewBase:
         """Returns the view to use for this presenter"""
         return PlayableGameViewBase(self)
 
+    @abstractmethod
+    def is_vs_ai(self) -> bool:
+        """Inheriting classes must specify if the game
+           is versus AI (offline engine or Lichess)
+        """
+        pass
+
     def update(self, **kwargs) -> None:
         """Update method called on game model updates. Overrides base."""
         if "successfulMoveMade" in kwargs:
             self.view.alert.clear_alert()
 
     def user_input_received(self, inpt: str) -> None:
         """Respond to the users input. This input can either be the
            move input, or game actions (such as resign)
         """
-        inpt_lower = inpt.lower()
-        if inpt_lower == "resign" or inpt_lower == "quit" or inpt_lower == "exit":
-            self.resign()
-        elif inpt_lower == "draw" or inpt_lower == "offer draw":
-            self.offer_draw()
-        elif inpt_lower == "takeback" or inpt_lower == "back" or inpt_lower == "undo":
-            self.propose_takeback()
-        else:
-            self.make_move(inpt)
+        try:
+            inpt_lower = inpt.lower()
+            if inpt_lower == "resign" or inpt_lower == "quit" or inpt_lower == "exit":
+                self.resign()
+            elif inpt_lower == "draw" or inpt_lower == "offer draw":
+                self.offer_draw()
+            elif inpt_lower == "takeback" or inpt_lower == "back" or inpt_lower == "undo":
+                self.propose_takeback()
+            elif self.model.is_my_turn():
+                self.make_move(inpt)
+            else:
+                self.model.set_premove(inpt)
+        except Exception as e:
+            self.view.alert.show_alert(str(e))
 
     def make_move(self, move: str) -> None:
         """Make the passed in move on the board"""
         try:
             move = move.strip()
             if move:
                 self.model.make_move(move)
```

### Comparing `cli-chess-1.1.1/src/cli_chess/core/game/offline_game/offline_game_model.py` & `cli_chess-1.2.0/src/cli_chess/core/game/offline_game/offline_game_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2024 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -46,38 +46,41 @@
                 if self.board_model.board.is_game_over():
                     self.game_in_progress = False
                     raise Warning("Game has already ended")
 
                 if not self.is_my_turn():
                     raise Warning("Not your turn")
 
-                move = move.strip()
-                if not move:
-                    raise Warning("No move specified")
+                self.board_model.make_move(move.strip())
+                self.premove_model.clear_premove()
 
-                self.board_model.make_move(move)
             except Exception:
                 raise
         else:
             log.warning("Attempted to make a move in a game that's not in progress")
             raise Warning("Game has already ended")
 
+    def set_premove(self, move: str) -> None:
+        """Sets the premove"""
+        self.premove_model.set_premove(move)
+
     def propose_takeback(self) -> None:
         """Take back the previous move"""
         try:
             if self.board_model.board.is_game_over():
                 raise Warning("Game has already ended")
 
+            self.premove_model.clear_premove()
             self.board_model.takeback(self.my_color)
         except Exception as e:
             log.error(f"Takeback failed - {e}")
             raise
 
     def offer_draw(self) -> None:
-        raise Warning("Engines do not accept draw offers")
+        raise Warning("Offline engine does not accept draw offers")
 
     def resign(self) -> None:
         """Handles resigning the game"""
         if self.game_in_progress:
             try:
                 self.board_model.handle_resignation(self.my_color)
             except Exception:
```

### Comparing `cli-chess-1.1.1/src/cli_chess/core/game/offline_game/offline_game_presenter.py` & `cli_chess-1.2.0/src/cli_chess/core/game/offline_game/offline_game_presenter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2024 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -45,20 +45,24 @@
         return OfflineGameView(self)
 
     def update(self, **kwargs) -> None:
         """Update method called on game model updates. Overrides base."""
         super().update(**kwargs)
         if "offlineGameOver" in kwargs:
             self._parse_and_present_game_over()
+            self.premove_presenter.clear_premove()
 
     def make_move(self, move: str) -> None:
         """Make the users move on the board"""
         try:
-            self.model.make_move(move)
-            self.make_engine_move()
+            if self.model.is_my_turn() and move:
+                self.model.make_move(move)
+                self.make_engine_move()
+            else:
+                self.premove_presenter.set_premove(move)
         except Exception as e:
             self.view.alert.show_alert(str(e))
 
     @threaded
     def make_engine_move(self) -> None:
         """Get the best move from the engine and make it"""
         try:
@@ -68,17 +72,20 @@
                 log.debug("Sending resignation on behalf of the engine")
                 self.board_presenter.handle_resignation(not self.model.my_color)
 
             elif engine_move.move:
                 move = engine_move.move.uci()
                 log.debug(f"Received move ({move}) from engine.")
                 self.board_presenter.make_move(move)
+
+                # After the engine moves, make the premove if set
+                self.make_move(self.premove_presenter.pop_premove())
         except Exception as e:
-            log.error(f"Engine error {e}")
-            self.view.alert.show_alert(f"Engine error: {e}")
+            log.error(e)
+            self.view.alert.show_alert(str(e))
 
     def _parse_and_present_game_over(self) -> None:
         """Triages game over status for parsing and sending to the view for display"""
         if not self.is_game_in_progress():
             status: Termination = self.model.game_metadata['state']['status']
             winner_str: str = self.model.game_metadata['state']['winner']
 
@@ -143,14 +150,18 @@
                 output = output + "• Seventy-five-move rule"
         else:
             log.debug(f"Received game over with uncaught status: {status}")
             output = "Game over • Draw"
 
         self.view.alert.show_alert(output, AlertType.NEUTRAL)
 
+    def is_vs_ai(self) -> bool:
+        """Returns True if the game is being played against an engine"""
+        return True
+
     def exit(self) -> None:
         """Exit current presenter/view"""
         try:
             super().exit()
             self.engine_presenter.quit_engine()
         except Exception as e:
             log.error(f"Error caught while exiting: {e}")
```

### Comparing `cli-chess-1.1.1/src/cli_chess/core/game/offline_game/offline_game_view.py` & `cli_chess-1.2.0/src/cli_chess/core/game/offline_game/offline_game_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2024 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -37,14 +37,15 @@
                         self.material_diff_upper_container,
                         self.move_list_container,
                         self.material_diff_lower_container,
                         self.player_info_lower_container,
                     ]), padding=0, padding_top=1)
                 ]),
                 self.input_field_container,
+                self.premove_container,
                 self.alert,
             ]),
             padding=0
         )
         function_bar = HSplit([
             self._create_function_bar()
         ], align=VerticalAlign.BOTTOM)
```

### Comparing `cli-chess-1.1.1/src/cli_chess/core/game/online_game/online_game_model.py` & `cli_chess-1.2.0/src/cli_chess/core/game/online_game/online_game_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2024 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -21,39 +21,38 @@
 from typing import Optional
 
 
 class OnlineGameModel(PlayableGameModelBase):
     """This model must only be used for games owned by the linked lichess user.
        Games not owned by this account must directly use the base model instead.
     """
-    def __init__(self, game_parameters: dict):
+    def __init__(self, game_parameters: dict, is_vs_ai: bool):
         super().__init__(play_as_color=game_parameters[GameOption.COLOR], variant=game_parameters[GameOption.VARIANT], fen=None)
         self._save_game_metadata(game_parameters=game_parameters)
 
         self.game_state_dispatcher = Optional[GameStateDispatcher]
         self.playing_game_id = None
         self.searching = False
-        self.vs_ai = False
+        self.vs_ai = is_vs_ai
 
         try:
             from cli_chess.core.api.api_manager import api_client, api_iem
             self.api_iem = api_iem
             self.api_client = api_client
         except ImportError:
             # TODO: Clean this up so the error is displayed on the main screen
             log.error("Failed to import api_iem and api_client")
             raise ImportError("API client not setup. Do you have an API token linked?")
 
     @threaded
-    def create_a_game(self, is_vs_ai: bool) -> None:
+    def create_game(self) -> None:
         """Sends a request to lichess to start an AI challenge using the selected game parameters"""
         # Note: Only subscribe to IEM events right before creating challenge to lessen chance of grabbing another game
         self.api_iem.subscribe_to_events(self.handle_iem_event)
         self._notify_game_model_updated(searchingForOpponent=True)
-        self.vs_ai = is_vs_ai
         self.searching = True
 
         if self.vs_ai:  # Challenge Lichess AI (stockfish)
             self.api_client.challenges.create_ai(level=self.game_metadata['ai_level'],
                                                  clock_limit=self.game_metadata['clock']['white']['time'],
                                                  clock_increment=self.game_metadata['clock']['white']['increment'],
                                                  color=self.game_metadata['my_color_str'],
@@ -119,14 +118,25 @@
 
             # TODO: Take some time measurements to see how much of an impact this approach is
             # Resetting and replaying the moves guarantees the game between lichess
             # and our local board are in sync (eg. takebacks, moves played on website, etc)
             self.board_model.reset(notify=False)
             self.board_model.make_moves_from_list(event.get('moves', []).split())
 
+            if self.is_my_turn():
+                premove = self.premove_model.pop_premove()
+                try:
+                    if premove:
+                        self.make_move(premove)
+                except Exception as e:
+                    if isinstance(e, ValueError):
+                        log.debug(f"The premove set was invalid in the new context, skipping: {e}")
+                    else:
+                        log.exception(e)
+
             if kwargs['gameOver']:
                 self._report_game_over(status=event.get('status'), winner=event.get('winner', ""))
 
         elif 'chatLine' in kwargs:
             event = kwargs['chatLine']
             self._save_game_metadata(gsd_chatLine=event)
 
@@ -138,41 +148,46 @@
     def make_move(self, move: str):
         """Sends the move to the board model for a validity check. If valid this
            function will pass the move over to the game state dispatcher to be sent
            Raises an exception on move or API errors.
         """
         if self.game_in_progress:
             try:
-                if not self.is_my_turn():
-                    raise Warning("Not your turn")
-
-                move = move.strip()
                 if not move:
                     raise Warning("No move specified")
 
                 if move == "0000":
                     raise Warning("Null moves are not supported in online games")
 
-                move = self.board_model.verify_move(move)
+                move = self.board_model.verify_move(move.strip())
                 self.game_state_dispatcher.make_move(move)
             except Exception:
                 raise
         else:
             log.warning("Attempted to make a move in a game that's not in progress")
             if self.searching:
                 raise Warning("Still searching for opponent")
             else:
                 raise Warning("Game has already ended")
 
+    def set_premove(self, move: str) -> None:
+        """Sets the premove. Raises an exception on an invalid premove"""
+        if self.game_in_progress and move and not self.is_my_turn():
+            if move == "0000":
+                raise Warning("Null moves are not supported in online games")
+            self.premove_model.set_premove(move)
+
     def propose_takeback(self) -> None:
         """Notifies the game state dispatcher to propose a takeback"""
         if self.game_in_progress:
             try:
                 if len(self.board_model.get_move_stack()) < 2:
                     raise Warning("Cannot send takeback with less than two moves")
+
+                self.premove_model.clear_premove()
                 self.game_state_dispatcher.send_takeback_request()
 
                 if not self.vs_ai:
                     raise RequestSuccessfullySent("Takeback request sent")
             except Exception:
                 raise
         else:
@@ -182,15 +197,15 @@
             else:
                 raise Warning("Game has already ended")
 
     def offer_draw(self) -> None:
         """Notifies the game state dispatcher to offer a draw"""
         if self.game_in_progress:
             if self.vs_ai:
-                raise Warning("AI does not accept draw offers")
+                raise Warning("Lichess AI does not accept draw offers")
 
             try:
                 self.game_state_dispatcher.send_draw_offer()
                 raise RequestSuccessfullySent("Draw offer sent")
             except Exception:
                 raise
         else:
```

### Comparing `cli-chess-1.1.1/src/cli_chess/core/game/online_game/online_game_presenter.py` & `cli_chess-1.2.0/src/cli_chess/core/game/online_game/online_game_presenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2024 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -20,18 +20,18 @@
 from chess import Color, COLOR_NAMES
 
 
 def start_online_game(game_parameters: dict, is_vs_ai: bool) -> None:
     """Start an online game. If `is_vs_ai` is True a challenge will be sent to
        the Lichess AI (stockfish). Otherwise, a seek vs a random opponent will be created
     """
-    model = OnlineGameModel(game_parameters)
+    model = OnlineGameModel(game_parameters, is_vs_ai)
     presenter = OnlineGamePresenter(model)
     change_views(presenter.view, presenter.view.input_field_container) # noqa
-    model.create_a_game(is_vs_ai)
+    model.create_game()
 
 
 class OnlineGamePresenter(PlayableGamePresenterBase):
     def __init__(self, model: OnlineGameModel):
         self.model = model
         super().__init__(model)
 
@@ -44,14 +44,15 @@
         super().update(**kwargs)
         if 'searchingForOpponent' in kwargs:
             self.view.alert.show_alert("Searching for opponent...", AlertType.NEUTRAL)
         if 'opponentFound' in kwargs:
             self.view.alert.clear_alert()
         if 'onlineGameOver' in kwargs:
             self._parse_and_present_game_over()
+            self.premove_presenter.clear_premove()
 
     def _parse_and_present_game_over(self) -> None:
         """Triages game over status for parsing and sending to the view for display"""
         if not self.is_game_in_progress():
             status: str = self.model.game_metadata['state']['status']
             winner_str = self.model.game_metadata['state']['winner']
 
@@ -117,7 +118,11 @@
                 output = "Game over • Draw"
             elif status == "stalemate":
                 output = "Draw • Stalemate"
         else:
             log.debug(f"Received game over with uncaught status: {status}")
 
         self.view.alert.show_alert(output, AlertType.NEUTRAL)
+
+    def is_vs_ai(self) -> bool:
+        """Returns true if the game being played is versus lichess AI"""
+        return self.model.vs_ai
```

### Comparing `cli-chess-1.1.1/src/cli_chess/core/game/online_game/online_game_view.py` & `cli_chess-1.2.0/src/cli_chess/core/game/online_game/online_game_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2024 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -39,14 +39,15 @@
                         self.move_list_container,
                         self.material_diff_lower_container,
                         self.player_info_lower_container,
                         self.clock_lower
                     ])
                 ]),
                 self.input_field_container,
+                self.premove_container,
                 self.alert,
             ]),
             padding=0
         )
         function_bar = HSplit([
             self._create_function_bar()
         ], align=VerticalAlign.BOTTOM)
```

### Comparing `cli-chess-1.1.1/src/cli_chess/core/game/online_game/watch_tv/watch_tv_model.py` & `cli_chess-1.2.0/src/cli_chess/core/game/online_game/watch_tv/watch_tv_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/core/game/online_game/watch_tv/watch_tv_presenter.py` & `cli_chess-1.2.0/src/cli_chess/core/game/online_game/watch_tv/watch_tv_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/core/game/online_game/watch_tv/watch_tv_view.py` & `cli_chess-1.2.0/src/cli_chess/core/game/online_game/watch_tv/watch_tv_view.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2024 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -11,20 +11,16 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 from cli_chess.core.game import GameViewBase
-from cli_chess.utils.ui_common import handle_mouse_click
-from prompt_toolkit.layout import Container, Window, FormattedTextControl, VSplit, HSplit, VerticalAlign, D
+from prompt_toolkit.layout import Container, Window, VSplit, HSplit, VerticalAlign, D
 from prompt_toolkit.widgets import Box
-from prompt_toolkit.formatted_text import StyleAndTextTuples
-from prompt_toolkit.key_binding import KeyBindings, merge_key_bindings
-from prompt_toolkit.keys import Keys
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from cli_chess.core.game.online_game.watch_tv import WatchTVPresenter
 
 
 class WatchTVView(GameViewBase):
     def __init__(self, presenter: WatchTVPresenter):
@@ -53,31 +49,7 @@
             padding=0
         )
         function_bar = HSplit([
             self._create_function_bar()
         ], align=VerticalAlign.BOTTOM)
 
         return HSplit([main_content, function_bar], key_bindings=self.get_key_bindings())
-
-    def _create_function_bar(self) -> VSplit:
-        """Create the conditional function bar"""
-        def _get_function_bar_fragments() -> StyleAndTextTuples:
-            fragments = self._base_function_bar_fragments()
-            fragments.extend([
-                ("class:function-bar.key", "F8", handle_mouse_click(self.presenter.exit)),
-                ("class:function-bar.label", f"{'Exit':<14}", handle_mouse_click(self.presenter.exit))
-            ])
-            return fragments
-
-        return VSplit([
-            Window(FormattedTextControl(_get_function_bar_fragments)),
-        ], height=D(max=1, preferred=1))
-
-    def get_key_bindings(self) -> "_MergedKeyBindings":  # noqa: F821:
-        """Returns the key bindings for this container"""
-        bindings = KeyBindings()
-
-        @bindings.add(Keys.F8, eager=True)
-        def _(event): # noqa
-            self.presenter.exit()
-
-        return merge_key_bindings([bindings, super().get_key_bindings()])
```

### Comparing `cli-chess-1.1.1/src/cli_chess/core/main/main_model.py` & `cli_chess-1.2.0/src/cli_chess/core/main/main_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/core/main/main_presenter.py` & `cli_chess-1.2.0/src/cli_chess/core/main/main_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/core/main/main_view.py` & `cli_chess-1.2.0/src/cli_chess/core/main/main_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/main_menu/main_menu_model.py` & `cli_chess-1.2.0/src/cli_chess/menus/main_menu/main_menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/main_menu/main_menu_presenter.py` & `cli_chess-1.2.0/src/cli_chess/menus/main_menu/main_menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/main_menu/main_menu_view.py` & `cli_chess-1.2.0/src/cli_chess/menus/main_menu/main_menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/menu_common.py` & `cli_chess-1.2.0/src/cli_chess/menus/menu_common.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/menu_model.py` & `cli_chess-1.2.0/src/cli_chess/menus/menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/menu_presenter.py` & `cli_chess-1.2.0/src/cli_chess/menus/menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/menu_view.py` & `cli_chess-1.2.0/src/cli_chess/menus/menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/offline_games_menu/offline_games_menu_model.py` & `cli_chess-1.2.0/src/cli_chess/menus/offline_games_menu/offline_games_menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/offline_games_menu/offline_games_menu_presenter.py` & `cli_chess-1.2.0/src/cli_chess/menus/offline_games_menu/offline_games_menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/offline_games_menu/offline_games_menu_view.py` & `cli_chess-1.2.0/src/cli_chess/menus/offline_games_menu/offline_games_menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/online_games_menu/online_games_menu_model.py` & `cli_chess-1.2.0/src/cli_chess/menus/online_games_menu/online_games_menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/online_games_menu/online_games_menu_presenter.py` & `cli_chess-1.2.0/src/cli_chess/menus/online_games_menu/online_games_menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/online_games_menu/online_games_menu_view.py` & `cli_chess-1.2.0/src/cli_chess/menus/online_games_menu/online_games_menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/program_settings_menu/program_settings_menu_model.py` & `cli_chess-1.2.0/src/cli_chess/menus/program_settings_menu/program_settings_menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/program_settings_menu/program_settings_menu_presenter.py` & `cli_chess-1.2.0/src/cli_chess/menus/program_settings_menu/program_settings_menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/program_settings_menu/program_settings_menu_view.py` & `cli_chess-1.2.0/src/cli_chess/menus/program_settings_menu/program_settings_menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/settings_menu/settings_menu_model.py` & `cli_chess-1.2.0/src/cli_chess/menus/settings_menu/settings_menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/settings_menu/settings_menu_presenter.py` & `cli_chess-1.2.0/src/cli_chess/menus/settings_menu/settings_menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/settings_menu/settings_menu_view.py` & `cli_chess-1.2.0/src/cli_chess/menus/settings_menu/settings_menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_model.py` & `cli_chess-1.2.0/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_presenter.py` & `cli_chess-1.2.0/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_view.py` & `cli_chess-1.2.0/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/versus_menus/versus_menu_models.py` & `cli_chess-1.2.0/src/cli_chess/menus/versus_menus/versus_menu_models.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/versus_menus/versus_menu_presenters.py` & `cli_chess-1.2.0/src/cli_chess/menus/versus_menus/versus_menu_presenters.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/menus/versus_menus/versus_menu_views.py` & `cli_chess-1.2.0/src/cli_chess/menus/versus_menus/versus_menu_views.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/about/about_presenter.py` & `cli_chess-1.2.0/src/cli_chess/modules/about/about_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/about/about_view.py` & `cli_chess-1.2.0/src/cli_chess/modules/about/about_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/board/board_model.py` & `cli_chess-1.2.0/src/cli_chess/modules/board/board_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2024 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -23,14 +23,15 @@
 
 class BoardModel:
     def __init__(self, orientation: chess.Color = chess.WHITE, variant="standard", fen="") -> None:
         self.board = self._initialize_board(variant, fen)
         self.initial_fen = self.board.fen()
         self.orientation = chess.WHITE if variant.lower() == "racingkings" else orientation
         self.highlight_move = chess.Move.null()
+        self.premove_highlight = chess.Move.null()
         self._game_over_result: Optional[chess.Outcome] = None
         self._log_init_info()
 
         self._event_manager = EventManager()
         self.e_board_model_updated = self._event_manager.create_event()
 
     @staticmethod
@@ -270,15 +271,15 @@
 
     @staticmethod
     def get_rank_label(rank_index: int) -> str:
         """Returns the rank label at the index passed in"""
         return chess.RANK_NAMES[rank_index]
 
     def is_square_in_check(self, square: chess.Square) -> bool:
-        """Returns True if a king whose turn it is
+        """Returns True if a king whose turn it
            is in check at the passed in square
         """
         king_square = self.board.king(self.board.turn)
         if square == king_square and self.board.is_check():
             return True
         return False
 
@@ -324,14 +325,31 @@
         """Handle marking the game as ended by resignation. The color
            passed in is the side resigning. Sends out a notification to
            listeners that the game is over.
         """
         self._game_over_result = chess.Outcome("resignation", not color_resigning)  # noqa
         self._notify_board_model_updated(isGameOver=True)
 
+    def set_premove_highlight(self, move: chess.Move) -> None:
+        """Sets the move that should be highlighted on the board.
+           indicating a premove. The board model itself does not
+           manage premoves but instead should be handled by an outside
+           class and passes to the board model for updating. This move
+           should never be popped from the board as it is a future
+           (possible) move.
+        """
+        if bool(move):
+            self.premove_highlight = move
+            self._notify_board_model_updated(premoveHighlightSet=True)
+
+    def clear_premove_highlight(self):
+        """Clears the set premove highlight"""
+        self.premove_highlight = chess.Move.null()
+        self._notify_board_model_updated(premoveHighlightCleared=True)
+
     def cleanup(self) -> None:
         """Handles model cleanup tasks. This should only ever
            be run when this model is no longer needed.
         """
         self._event_manager.purge_all_events()
 
     def _notify_board_model_updated(self, **kwargs) -> None:
```

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/board/board_presenter.py` & `cli_chess-1.2.0/src/cli_chess/modules/board/board_presenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,19 +166,23 @@
         if self.model.is_light_square(square):
             square_color = "light-square"
         else:
             square_color = "dark-square"
 
         show_board_highlights = self.game_config_values[game_config.Keys.SHOW_BOARD_HIGHLIGHTS]
         if show_board_highlights:
+            # TODO: Lighten last move square color if on light square
             try:
                 last_move = self.model.get_highlight_move()
                 if bool(last_move) and (square == last_move.to_square or square == last_move.from_square):
                     square_color = "last-move"
-                    # TODO: Lighten last move square color if on light square
+
+                premove_highlight = self.model.premove_highlight
+                if bool(premove_highlight) and (square == premove_highlight.from_square or square == premove_highlight.to_square):
+                    square_color = "pre-move"
             except IndexError:
                 pass
 
             if self.model.is_square_in_check(square):
                 square_color = "in-check"
 
         return square_color
```

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/board/board_view.py` & `cli_chess-1.2.0/src/cli_chess/modules/board/board_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/clock/clock_presenter.py` & `cli_chess-1.2.0/src/cli_chess/modules/clock/clock_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/clock/clock_view.py` & `cli_chess-1.2.0/src/cli_chess/modules/clock/clock_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/common.py` & `cli_chess-1.2.0/src/cli_chess/modules/common.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_arm64_macos` & `cli_chess-1.2.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_arm64_macos`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_linux` & `cli_chess-1.2.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_linux`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_macos` & `cli_chess-1.2.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_macos`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_windows.exe` & `cli_chess-1.2.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_windows.exe`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/engine/engine_model.py` & `cli_chess-1.2.0/src/cli_chess/modules/engine/engine_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/engine/engine_presenter.py` & `cli_chess-1.2.0/src/cli_chess/modules/engine/engine_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/material_difference/material_difference_model.py` & `cli_chess-1.2.0/src/cli_chess/modules/material_difference/material_difference_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/material_difference/material_difference_presenter.py` & `cli_chess-1.2.0/src/cli_chess/modules/material_difference/material_difference_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/material_difference/material_difference_view.py` & `cli_chess-1.2.0/src/cli_chess/modules/material_difference/material_difference_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/move_list/move_list_model.py` & `cli_chess-1.2.0/src/cli_chess/modules/move_list/move_list_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/move_list/move_list_presenter.py` & `cli_chess-1.2.0/src/cli_chess/modules/move_list/move_list_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/move_list/move_list_view.py` & `cli_chess-1.2.0/src/cli_chess/modules/move_list/move_list_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,17 +41,14 @@
         """Create the move list container"""
         return Box(self._move_list_output, height=D(max=4), padding=0)
 
     def update(self, formatted_move_list: List[str]):
         """Loops through the passed in move list
            and updates the move list display
         """
-        # TODO: When the move list is displayed as unicode, frequently the
-        #       moves do not line up. Need to rework how the container handles
-        #       the text with (hopefully) not losing the ability to scroll the list
         output = ""
         for i, move in enumerate(formatted_move_list):
             if i % 2 == 0 and i != 0:
                 output += "\n"
             output += move.ljust(8)
 
         self._move_list_output.text = output if output else "No moves..."
```

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/player_info/player_info_presenter.py` & `cli_chess-1.2.0/src/cli_chess/modules/player_info/player_info_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/player_info/player_info_view.py` & `cli_chess-1.2.0/src/cli_chess/modules/player_info/player_info_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/token_manager/token_manager_model.py` & `cli_chess-1.2.0/src/cli_chess/modules/token_manager/token_manager_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/token_manager/token_manager_presenter.py` & `cli_chess-1.2.0/src/cli_chess/modules/token_manager/token_manager_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/modules/token_manager/token_manager_view.py` & `cli_chess-1.2.0/src/cli_chess/modules/token_manager/token_manager_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/tests/modules/board/test_board_model.py` & `cli_chess-1.2.0/src/cli_chess/tests/modules/board/test_board_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/tests/modules/board/test_board_presenter.py` & `cli_chess-1.2.0/src/cli_chess/tests/modules/board/test_board_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/tests/modules/material_difference/test_material_difference_model.py` & `cli_chess-1.2.0/src/cli_chess/tests/modules/material_difference/test_material_difference_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/tests/modules/material_difference/test_material_difference_presenter.py` & `cli_chess-1.2.0/src/cli_chess/tests/modules/material_difference/test_material_difference_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/tests/modules/move_list/test_move_list_model.py` & `cli_chess-1.2.0/src/cli_chess/tests/modules/move_list/test_move_list_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/tests/modules/move_list/test_move_list_presenter.py` & `cli_chess-1.2.0/src/cli_chess/tests/modules/move_list/test_move_list_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/tests/modules/test_common.py` & `cli_chess-1.2.0/src/cli_chess/tests/modules/test_common.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/tests/modules/token_manager/test_token_manager_model.py` & `cli_chess-1.2.0/src/cli_chess/tests/modules/token_manager/test_token_manager_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/tests/modules/token_manager/test_token_manager_presenter.py` & `cli_chess-1.2.0/src/cli_chess/tests/modules/token_manager/test_token_manager_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/tests/utils/test_event.py` & `cli_chess-1.2.0/src/cli_chess/tests/utils/test_event.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/utils/argparse.py` & `cli_chess-1.2.0/src/cli_chess/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/utils/common.py` & `cli_chess-1.2.0/src/cli_chess/utils/common.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/utils/config.py` & `cli_chess-1.2.0/src/cli_chess/utils/config.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/utils/event.py` & `cli_chess-1.2.0/src/cli_chess/utils/event.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/utils/logging.py` & `cli_chess-1.2.0/src/cli_chess/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess/utils/styles.py` & `cli_chess-1.2.0/src/cli_chess/utils/styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     "dark-square.light-piece": f"fg:{light_piece_color}",
     "dark-square.dark-piece": f"fg:{dark_piece_color}",
 
     "last-move": "bg:yellowgreen",
     "last-move.light-piece": f"fg:{light_piece_color}",
     "last-move.dark-piece": f"fg:{dark_piece_color}",
 
+    "pre-move": "bg:darkorange",
+    "pre-move.light-piece": f"fg:{light_piece_color}",
+    "pre-move.dark-piece": f"fg:{dark_piece_color}",
+
     "in-check": "bg:red",
     "in-check.light-piece": f"fg:{light_piece_color}",
     "in-check.dark-piece": f"fg:{dark_piece_color}",
 
     "material-difference": "fg:gray",
     "move-list": "fg:gray",
     "move-input": "fg:white bold",
```

### Comparing `cli-chess-1.1.1/src/cli_chess/utils/ui_common.py` & `cli_chess-1.2.0/src/cli_chess/utils/ui_common.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.1.1/src/cli_chess.egg-info/PKG-INFO` & `cli_chess-1.2.0/src/cli_chess.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-chess
-Version: 1.1.1
+Version: 1.2.0
 Summary: A highly customizable way to play chess in your terminal
 Home-page: https://github.com/trevorbayless/cli-chess
 Author: Trevor Bayless
 Author-email: trevorbayless1@gmail.com
 License: GPL-3.0+
 Keywords: chess,terminal,fairy-stockfish,stockfish,lichess,lichess.org,cli,san,uci
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -20,16 +20,24 @@
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: chess<2.0.0,>=1.9.4
+Requires-Dist: berserk<0.14.0,>=0.13.1
+Requires-Dist: prompt-toolkit==3.0.44
+Provides-Extra: dev
+Requires-Dist: pytest<8.0.0,>=7.2.1; extra == "dev"
+Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == "dev"
+Requires-Dist: pytest-socket<1.0.0,>=0.6.0; extra == "dev"
+Requires-Dist: flake8<7.0.0,>=5.0.4; extra == "dev"
+Requires-Dist: vulture<3.0,>=2.7; extra == "dev"
 
 <p align="center">
   <a href="#"><img src="https://user-images.githubusercontent.com/3620552/214357735-53c2174c-5ada-45a2-97cb-6a25b5ca9c0c.png"/></a>
 </p>
 
 <p align="center">
 A highly customizable way to play chess in your terminal. Supports playing online (via Lichess.org) and
```

#### html2text {}

```diff
@@ -1,24 +1,29 @@
-Metadata-Version: 2.1 Name: cli-chess Version: 1.1.1 Summary: A highly
+Metadata-Version: 2.1 Name: cli-chess Version: 1.2.0 Summary: A highly
 customizable way to play chess in your terminal Home-page: https://github.com/
 trevorbayless/cli-chess Author: Trevor Bayless Author-email:
 trevorbayless1@gmail.com License: GPL-3.0+ Keywords: chess,terminal,fairy-
 stockfish,stockfish,lichess,lichess.org,cli,san,uci Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: Microsoft ::
 Windows Classifier: Operating System :: MacOS Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Games/Entertainment
 :: Board Games Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Requires-Python:
->=3.8 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE
+>=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: chess<2.0.0,>=1.9.4 Requires-Dist: berserk<0.14.0,>=0.13.1 Requires-Dist:
+prompt-toolkit==3.0.44 Provides-Extra: dev Requires-Dist: pytest<8.0.0,>=7.2.1;
+extra == "dev" Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == "dev"
+Requires-Dist: pytest-socket<1.0.0,>=0.6.0; extra == "dev" Requires-Dist:
+flake8<7.0.0,>=5.0.4; extra == "dev" Requires-Dist: vulture<3.0,>=2.7; extra ==
+"dev"
   _[_h_t_t_p_s_:_/_/_u_s_e_r_-_i_m_a_g_e_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_3_6_2_0_5_5_2_/_2_1_4_3_5_7_7_3_5_-_5_3_c_2_1_7_4_c_-_5_a_d_a_-
                           _4_5_a_2_-_9_7_c_b_-_6_a_2_5_b_5_c_a_9_c_0_c_._p_n_g_]
   A highly customizable way to play chess in your terminal. Supports playing
  online (via Lichess.org) and offline against the Fairy-Stockfish engine. All
                         Lichess variants are supported.
                           _[_C_I_ _W_o_r_k_f_l_o_w_]_[_P_y_P_I_]_[_P_y_t_h_o_n_]
 Demo Offline against Fairy-Stockfish | Watching Lichess Bullet TV :------------
```

### Comparing `cli-chess-1.1.1/src/cli_chess.egg-info/SOURCES.txt` & `cli_chess-1.2.0/src/cli_chess.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,18 @@
 src/cli_chess/modules/move_list/__init__.py
 src/cli_chess/modules/move_list/move_list_model.py
 src/cli_chess/modules/move_list/move_list_presenter.py
 src/cli_chess/modules/move_list/move_list_view.py
 src/cli_chess/modules/player_info/__init__.py
 src/cli_chess/modules/player_info/player_info_presenter.py
 src/cli_chess/modules/player_info/player_info_view.py
+src/cli_chess/modules/premove/__init__.py
+src/cli_chess/modules/premove/premove_model.py
+src/cli_chess/modules/premove/premove_presenter.py
+src/cli_chess/modules/premove/premove_view.py
 src/cli_chess/modules/token_manager/__init__.py
 src/cli_chess/modules/token_manager/token_manager_model.py
 src/cli_chess/modules/token_manager/token_manager_presenter.py
 src/cli_chess/modules/token_manager/token_manager_view.py
 src/cli_chess/tests/__init__.py
 src/cli_chess/tests/modules/__init__.py
 src/cli_chess/tests/modules/test_common.py
```

