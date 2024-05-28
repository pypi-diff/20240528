# Comparing `tmp/bootwrap-1.0.1.tar.gz` & `tmp/bootwrap-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootwrap-1.0.1.tar", last modified: Mon May 27 19:59:16 2024, max compression
+gzip compressed data, was "bootwrap-1.0.2.tar", last modified: Tue May 28 20:56:40 2024, max compression
```

## Comparing `bootwrap-1.0.1.tar` & `bootwrap-1.0.2.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.653569 bootwrap-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.621569 bootwrap-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.629569 bootwrap-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-27 19:59:11.000000 bootwrap-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-27 19:59:11.000000 bootwrap-1.0.1/.github/workflows/pre-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-27 19:59:11.000000 bootwrap-1.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-27 19:59:11.000000 bootwrap-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-27 19:59:11.000000 bootwrap-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-27 19:59:11.000000 bootwrap-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-27 19:59:16.653569 bootwrap-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-27 19:59:11.000000 bootwrap-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.629569 bootwrap-1.0.1/bootwrap/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.637569 bootwrap-1.0.1/bootwrap/components/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/anchor.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/badge.py
--rw-r--r--   0 runner    (1001) docker     (127)    17817 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/deck.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    14694 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/icon.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/link.py
--rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/panel.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/separator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/generic.css
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/generic.js
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.653569 bootwrap-1.0.1/bootwrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-27 19:59:16.000000 bootwrap-1.0.1/bootwrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-27 19:59:16.000000 bootwrap-1.0.1/bootwrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:59:16.000000 bootwrap-1.0.1/bootwrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 19:59:16.000000 bootwrap-1.0.1/bootwrap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.641569 bootwrap-1.0.1/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48411 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/aapl-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    59453 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/account-screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)   115095 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/activity-screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/amzn-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   284519 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/background.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    39185 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/bank.png
--rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/cash.png
--rw-r--r--   0 runner    (1001) docker     (127)   458319 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/collage.png
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/demo.md
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/demo_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/demo_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/demo_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/demo_user.py
--rw-r--r--   0 runner    (1001) docker     (127)   117258 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/discovery-screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    16363 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/googl-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    36084 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/hard-work.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/lnkd-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    38559 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/login-screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)    45146 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/nvda-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/party.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    75442 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/piggybank-title.png
--rw-r--r--   0 runner    (1001) docker     (127)   108158 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/portfolio-screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/stock.png
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/tsla-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.645569 bootwrap-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/amazon-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   112499 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/base.html
--rw-r--r--   0 runner    (1001) docker     (127)    28291 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/bootwrap-equation.png
--rw-r--r--   0 runner    (1001) docker     (127)   297611 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/components.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.649569 bootwrap-1.0.1/docs/config/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/config/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/config/components.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/config/home.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/config/layout.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17454 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/doc_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/doc_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    52572 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/flash.png
--rw-r--r--   0 runner    (1001) docker     (127)    16363 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/google-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/layout.png
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/linkedin-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/menu.png
--rw-r--r--   0 runner    (1001) docker     (127)    32506 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/multi-pages-app.png
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/page.png
--rw-r--r--   0 runner    (1001) docker     (127)    17798 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/single-page-app.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2886 2024-05-27 19:59:11.000000 bootwrap-1.0.1/helper.sh
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-27 19:59:11.000000 bootwrap-1.0.1/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-27 19:59:11.000000 bootwrap-1.0.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 19:59:11.000000 bootwrap-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:59:16.653569 bootwrap-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 19:59:11.000000 bootwrap-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.653569 bootwrap-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_anchor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_badge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_deck.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    15690 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_separator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:56:40.912176 bootwrap-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:56:40.880175 bootwrap-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:56:40.888176 bootwrap-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-28 20:56:31.000000 bootwrap-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-28 20:56:31.000000 bootwrap-1.0.2/.github/workflows/pre-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-28 20:56:31.000000 bootwrap-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-28 20:56:31.000000 bootwrap-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-28 20:56:31.000000 bootwrap-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 20:56:31.000000 bootwrap-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-28 20:56:40.912176 bootwrap-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-28 20:56:31.000000 bootwrap-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:56:40.888176 bootwrap-1.0.2/bootwrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:56:40.892176 bootwrap-1.0.2/bootwrap/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17817 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/deck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14694 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/separator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/components/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/generic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/generic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-28 20:56:31.000000 bootwrap-1.0.2/bootwrap/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:56:40.908176 bootwrap-1.0.2/bootwrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-28 20:56:40.000000 bootwrap-1.0.2/bootwrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-28 20:56:40.000000 bootwrap-1.0.2/bootwrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:56:40.000000 bootwrap-1.0.2/bootwrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 20:56:40.000000 bootwrap-1.0.2/bootwrap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:56:40.900176 bootwrap-1.0.2/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48411 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/aapl-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59453 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/account-screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   115095 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/activity-screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/amzn-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   284519 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/background.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    39185 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/bank.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/cash.png
+-rw-r--r--   0 runner    (1001) docker     (127)   458319 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/collage.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/demo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/demo_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/demo_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/demo_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/demo_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117258 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/discovery-screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    16363 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/googl-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36084 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/hard-work.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/lnkd-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38559 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/login-screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45146 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/nvda-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/party.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    75442 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/piggybank-title.png
+-rw-r--r--   0 runner    (1001) docker     (127)   108158 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/portfolio-screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/stock.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-28 20:56:31.000000 bootwrap-1.0.2/demo/tsla-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:56:40.904176 bootwrap-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/amazon-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   112499 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28291 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/bootwrap-equation.png
+-rw-r--r--   0 runner    (1001) docker     (127)   297611 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/components.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:56:40.904176 bootwrap-1.0.2/docs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/config/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/config/components.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/config/home.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/config/layout.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17454 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/doc_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/doc_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    52572 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/flash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16363 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/google-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/layout.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/linkedin-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/menu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32506 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/multi-pages-app.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/page.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17798 2024-05-28 20:56:31.000000 bootwrap-1.0.2/docs/single-page-app.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2886 2024-05-28 20:56:31.000000 bootwrap-1.0.2/helper.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-28 20:56:31.000000 bootwrap-1.0.2/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-28 20:56:31.000000 bootwrap-1.0.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 20:56:31.000000 bootwrap-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 20:56:40.912176 bootwrap-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-28 20:56:31.000000 bootwrap-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:56:40.908176 bootwrap-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_deck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15690 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_separator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-28 20:56:31.000000 bootwrap-1.0.2/tests/test_utils.py
```

### Comparing `bootwrap-1.0.1/.github/workflows/ci.yml` & `bootwrap-1.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/.github/workflows/pre-release.yml` & `bootwrap-1.0.2/.github/workflows/pre-release.yml`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/.github/workflows/release.yml` & `bootwrap-1.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/.gitignore` & `bootwrap-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/CONTRIBUTING.md` & `bootwrap-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/LICENSE` & `bootwrap-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/PKG-INFO` & `bootwrap-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootwrap
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for rapid development of web-based user interfaces.
 Home-page: https://github.com/mmgalushka/bootwrap
 Author: Mykola Galushka
 Author-email: mm.galushka@gmail.com
 Project-URL: Bug Tracker, https://github.com/mmgalushka/bootwrap/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bootwrap-1.0.1/README.md` & `bootwrap-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/auth.py` & `bootwrap-1.0.2/bootwrap/auth.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/__init__.py` & `bootwrap-1.0.2/bootwrap/components/__init__.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/anchor.py` & `bootwrap-1.0.2/bootwrap/components/anchor.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/badge.py` & `bootwrap-1.0.2/bootwrap/components/badge.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/base.py` & `bootwrap-1.0.2/bootwrap/components/base.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/button.py` & `bootwrap-1.0.2/bootwrap/components/button.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/deck.py` & `bootwrap-1.0.2/bootwrap/components/deck.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/dialog.py` & `bootwrap-1.0.2/bootwrap/components/dialog.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/form.py` & `bootwrap-1.0.2/bootwrap/components/form.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/icon.py` & `bootwrap-1.0.2/bootwrap/components/icon.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/image.py` & `bootwrap-1.0.2/bootwrap/components/image.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/javascript.py` & `bootwrap-1.0.2/bootwrap/components/javascript.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/link.py` & `bootwrap-1.0.2/bootwrap/components/link.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/list.py` & `bootwrap-1.0.2/bootwrap/components/list.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/navigation.py` & `bootwrap-1.0.2/bootwrap/components/navigation.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/panel.py` & `bootwrap-1.0.2/bootwrap/components/panel.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/table.py` & `bootwrap-1.0.2/bootwrap/components/table.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/text.py` & `bootwrap-1.0.2/bootwrap/components/text.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/components/utils.py` & `bootwrap-1.0.2/bootwrap/components/utils.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/generic.css` & `bootwrap-1.0.2/bootwrap/generic.css`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/menu.py` & `bootwrap-1.0.2/bootwrap/menu.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap/page.py` & `bootwrap-1.0.2/bootwrap/page.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/bootwrap.egg-info/PKG-INFO` & `bootwrap-1.0.2/bootwrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootwrap
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for rapid development of web-based user interfaces.
 Home-page: https://github.com/mmgalushka/bootwrap
 Author: Mykola Galushka
 Author-email: mm.galushka@gmail.com
 Project-URL: Bug Tracker, https://github.com/mmgalushka/bootwrap/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bootwrap-1.0.1/bootwrap.egg-info/SOURCES.txt` & `bootwrap-1.0.2/bootwrap.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 helper.sh
 main.py
 pytest.ini
 requirements.txt
 setup.py
 ./bootwrap/__init__.py
 ./bootwrap/auth.py
+./bootwrap/generic.css
+./bootwrap/generic.js
 ./bootwrap/menu.py
 ./bootwrap/page.py
 ./bootwrap/components/__init__.py
 ./bootwrap/components/anchor.py
 ./bootwrap/components/badge.py
 ./bootwrap/components/base.py
 ./bootwrap/components/button.py
```

### Comparing `bootwrap-1.0.1/demo/aapl-logo.png` & `bootwrap-1.0.2/demo/aapl-logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/account-screenshot.png` & `bootwrap-1.0.2/demo/account-screenshot.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/activity-screenshot.png` & `bootwrap-1.0.2/demo/activity-screenshot.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/amzn-logo.png` & `bootwrap-1.0.2/demo/amzn-logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/background.jpg` & `bootwrap-1.0.2/demo/background.jpg`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/bank.png` & `bootwrap-1.0.2/demo/bank.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/cash.png` & `bootwrap-1.0.2/demo/cash.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/collage.png` & `bootwrap-1.0.2/demo/collage.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/demo.md` & `bootwrap-1.0.2/demo/demo.md`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/demo_app.py` & `bootwrap-1.0.2/demo/demo_app.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/demo_components.py` & `bootwrap-1.0.2/demo/demo_components.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/demo_stock.py` & `bootwrap-1.0.2/demo/demo_stock.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/demo_user.py` & `bootwrap-1.0.2/demo/demo_user.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/discovery-screenshot.png` & `bootwrap-1.0.2/demo/discovery-screenshot.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/favicon.ico` & `bootwrap-1.0.2/demo/favicon.ico`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/googl-logo.png` & `bootwrap-1.0.2/demo/googl-logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/hard-work.jpg` & `bootwrap-1.0.2/demo/hard-work.jpg`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/lnkd-logo.png` & `bootwrap-1.0.2/demo/lnkd-logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/login-screenshot.png` & `bootwrap-1.0.2/demo/login-screenshot.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/logo.png` & `bootwrap-1.0.2/demo/logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/nvda-logo.png` & `bootwrap-1.0.2/demo/nvda-logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/party.jpg` & `bootwrap-1.0.2/demo/party.jpg`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/piggybank-title.png` & `bootwrap-1.0.2/demo/piggybank-title.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/portfolio-screenshot.png` & `bootwrap-1.0.2/demo/portfolio-screenshot.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/stock.png` & `bootwrap-1.0.2/demo/stock.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/demo/tsla-logo.png` & `bootwrap-1.0.2/demo/tsla-logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/amazon-logo.png` & `bootwrap-1.0.2/docs/amazon-logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/base.html` & `bootwrap-1.0.2/docs/base.html`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/bootwrap-equation.png` & `bootwrap-1.0.2/docs/bootwrap-equation.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/components.html` & `bootwrap-1.0.2/docs/components.html`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/config/base.yaml` & `bootwrap-1.0.2/docs/config/base.yaml`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/config/components.yaml` & `bootwrap-1.0.2/docs/config/components.yaml`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/config/home.yaml` & `bootwrap-1.0.2/docs/config/home.yaml`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/config/layout.yaml` & `bootwrap-1.0.2/docs/config/layout.yaml`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/doc_app.py` & `bootwrap-1.0.2/docs/doc_app.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/doc_generator.py` & `bootwrap-1.0.2/docs/doc_generator.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/favicon.ico` & `bootwrap-1.0.2/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/flash.png` & `bootwrap-1.0.2/docs/flash.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/google-logo.png` & `bootwrap-1.0.2/docs/google-logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/index.html` & `bootwrap-1.0.2/docs/index.html`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/layout.html` & `bootwrap-1.0.2/docs/layout.html`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/layout.png` & `bootwrap-1.0.2/docs/layout.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/linkedin-logo.png` & `bootwrap-1.0.2/docs/linkedin-logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/logo.png` & `bootwrap-1.0.2/docs/logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/menu.png` & `bootwrap-1.0.2/docs/menu.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/multi-pages-app.png` & `bootwrap-1.0.2/docs/multi-pages-app.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/page.png` & `bootwrap-1.0.2/docs/page.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/docs/single-page-app.png` & `bootwrap-1.0.2/docs/single-page-app.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/helper.sh` & `bootwrap-1.0.2/helper.sh`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/main.py` & `bootwrap-1.0.2/main.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/pytest.ini` & `bootwrap-1.0.2/pytest.ini`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/setup.py` & `bootwrap-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,11 +26,13 @@
         'Intended Audience :: Developers',
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
     ],
     package_dir={"": "."},
     packages=setuptools.find_packages(where=".", exclude=["tests"]),
+    package_data={"bootwrap": ["*.css", "*.js"]},
+    include_package_data=True,    
     python_requires=">=3.6",
     use_scm_version=True,
-    setup_requires=['setuptools_scm']
+    setup_requires=['setuptools_scm'],
 )
```

### Comparing `bootwrap-1.0.1/tests/helper.py` & `bootwrap-1.0.2/tests/helper.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_anchor.py` & `bootwrap-1.0.2/tests/test_anchor.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_auth.py` & `bootwrap-1.0.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_base.py` & `bootwrap-1.0.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_button.py` & `bootwrap-1.0.2/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_deck.py` & `bootwrap-1.0.2/tests/test_deck.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_dialog.py` & `bootwrap-1.0.2/tests/test_dialog.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_form.py` & `bootwrap-1.0.2/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_helper.py` & `bootwrap-1.0.2/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_icon.py` & `bootwrap-1.0.2/tests/test_icon.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_image.py` & `bootwrap-1.0.2/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_javascript.py` & `bootwrap-1.0.2/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_link.py` & `bootwrap-1.0.2/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_list.py` & `bootwrap-1.0.2/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_menu.py` & `bootwrap-1.0.2/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_navigation.py` & `bootwrap-1.0.2/tests/test_navigation.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_page.py` & `bootwrap-1.0.2/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_panel.py` & `bootwrap-1.0.2/tests/test_panel.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_table.py` & `bootwrap-1.0.2/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_text.py` & `bootwrap-1.0.2/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.1/tests/test_utils.py` & `bootwrap-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

