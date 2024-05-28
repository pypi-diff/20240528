# Comparing `tmp/popoll_backend-0.0.57.tar.gz` & `tmp/popoll_backend-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popoll_backend-0.0.57.tar", last modified: Mon May 27 08:53:21 2024, max compression
+gzip compressed data, was "popoll_backend-0.0.58.tar", last modified: Tue May 28 11:20:59 2024, max compression
```

## Comparing `popoll_backend-0.0.57.tar` & `popoll_backend-0.0.58.tar`

### file list

```diff
@@ -1,86 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.953738 popoll_backend-0.0.57/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-27 08:53:21.953738 popoll_backend-0.0.57/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.936738 popoll_backend-0.0.57/popoll_backend/
--rw-rw-rw-   0 root         (0) root         (0)     7908 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.938738 popoll_backend-0.0.57/popoll_backend/model/
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.939738 popoll_backend-0.0.57/popoll_backend/model/db/
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/answer.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/date.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/option.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/session.py
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/user.py
--rw-rw-rw-   0 root         (0) root         (0)      736 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/user_instruments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.942738 popoll_backend-0.0.57/popoll_backend/model/payload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/date_details.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/dates.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/empty.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/history.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/id_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/user_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/user_with_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/users.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/users_payload_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.948738 popoll_backend-0.0.57/popoll_backend/query/
--rw-rw-rw-   0 root         (0) root         (0)     2226 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1017 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/create_date.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/create_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/create_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1860 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/create_user.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/delete_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_all_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1459 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_date_details.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      519 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1028 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_user_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1048 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_user_with_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/update_date.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1934 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/update_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.953738 popoll_backend-0.0.57/popoll_backend.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-27 08:53:21.000000 popoll_backend-0.0.57/popoll_backend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2687 2024-05-27 08:53:21.000000 popoll_backend-0.0.57/popoll_backend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 08:53:21.000000 popoll_backend-0.0.57/popoll_backend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-27 08:53:21.000000 popoll_backend-0.0.57/popoll_backend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-27 08:53:21.000000 popoll_backend-0.0.57/popoll_backend.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-27 08:53:16.000000 popoll_backend-0.0.57/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 08:53:21.954738 popoll_backend-0.0.57/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.952738 popoll_backend-0.0.57/tests/
--rw-rw-rw-   0 root         (0) root         (0)      803 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_01_get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1102 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_02_create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_03_update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_04_get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_08_get_users.py
--rw-rw-rw-   0 root         (0) root         (0)     2054 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_09_create_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_10_get_user.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_11_update_user.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_12_delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_13_get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_14_create_date.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_15_get_date.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_16_update_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_17_delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_18_create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_19_update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_20_delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_21_get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_22_get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      572 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_23_get_create_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:20:59.350417 popoll_backend-0.0.58/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-28 11:20:59.350417 popoll_backend-0.0.58/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:20:59.333416 popoll_backend-0.0.58/popoll_backend/
+-rw-rw-rw-   0 root         (0) root         (0)     8225 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:20:59.334416 popoll_backend-0.0.58/popoll_backend/model/
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:20:59.336417 popoll_backend-0.0.58/popoll_backend/model/db/
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/db/answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/db/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/db/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/db/option.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/db/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/db/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      736 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/db/user_instruments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:20:59.338417 popoll_backend-0.0.58/popoll_backend/model/payload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/payload/date_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/payload/dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/payload/empty.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/payload/history.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/payload/id_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/payload/instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/payload/polls.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/payload/user_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/payload/user_with_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/payload/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/model/payload/users_payload_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:20:59.345417 popoll_backend-0.0.58/popoll_backend/query/
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/create_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)     2402 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      894 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      665 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/delete_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_all_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      756 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_all_sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_date_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_user_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_user_with_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/popoll_backend/query/update_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:20:59.350417 popoll_backend-0.0.58/popoll_backend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-28 11:20:59.000000 popoll_backend-0.0.58/popoll_backend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2799 2024-05-28 11:20:59.000000 popoll_backend-0.0.58/popoll_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 11:20:59.000000 popoll_backend-0.0.58/popoll_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-28 11:20:59.000000 popoll_backend-0.0.58/popoll_backend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-28 11:20:59.000000 popoll_backend-0.0.58/popoll_backend.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-28 11:20:53.000000 popoll_backend-0.0.58/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 11:20:59.350417 popoll_backend-0.0.58/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:20:59.349417 popoll_backend-0.0.58/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_01_get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_02_create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_03_update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_04_get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_08_get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_09_create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_10_get_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_11_update_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_12_delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_13_get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_14_create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_15_get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_16_update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_17_delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_18_create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_19_update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_20_delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_21_get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_22_get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      572 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_23_get_create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-28 11:20:38.000000 popoll_backend-0.0.58/tests/test_24_get_all_session.py
```

### Comparing `popoll_backend-0.0.57/PKG-INFO` & `popoll_backend-0.0.58/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.57
+Version: 0.0.58
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `popoll_backend-0.0.57/popoll_backend/__main__.py` & `popoll_backend-0.0.58/popoll_backend/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from popoll_backend.query.create_poll import CreatePoll
 from popoll_backend.query.create_user import CreateUser
 from popoll_backend.query.delete_answer import DeleteAnswer
 from popoll_backend.query.delete_date import DeleteDate
 from popoll_backend.query.delete_instrument import DeleteInstrument
 from popoll_backend.query.delete_user import DeleteUser
 from popoll_backend.query.get_all_instruments import GetAllInstruments
+from popoll_backend.query.get_all_sessions import GetAllSession
 from popoll_backend.query.get_answer import GetAnswer
 from popoll_backend.query.get_date import GetDate
 from popoll_backend.query.get_date_details import GetDateDetails
 from popoll_backend.query.get_dates import GetDates
 from popoll_backend.query.get_instrument import GetInstrument
 from popoll_backend.query.get_instruments import GetInstruments
 from popoll_backend.query.get_poll import GetPoll
@@ -71,49 +72,49 @@
         return res
     return decorated
 
 
 
 
 
-class PollEndpoint(Resource):
+class PollPollEndpoint(Resource):
     def get(self, poll: str) -> str: return GetPoll(poll).run().toJSON()
     
     @history
     def post(self, poll:str) -> str: return CreatePoll(poll, body(flask.request, 'name', mandatory=False, default=poll), body(flask.request, 'instruments', mandatory=False, default=[]), body(flask.request, 'color', mandatory=False, default="#000000")).run().toJSON()
     
     @history
     def put(self, poll:str) -> str: return UpdatePoll(poll, body(flask.request, 'name'), body(flask.request, 'color')).run().toJSON()
     
     
     
 
-class InstrumentsEndpoint(Resource):
+class PollInstrumentsEndpoint(Resource):
     def get(self, poll: str) -> str: 
         if queryParam(flask.request, 'used_only'):
             return GetInstruments(poll).run().toJSON()
         else:
             return GetAllInstruments(poll).run().toJSON()
     
     
 
 
 
 
 
 
-class UsersEndpoint(Resource):
+class PollUsersEndpoint(Resource):
     def get(self, poll: str) -> str: return GetUsers(poll).run().toJSON()
     
     @history
     def post(self, poll: str) -> str: return CreateUser(poll, body(flask.request, 'user')['name'], body(flask.request, 'main_instrument')['id'], [i['id'] for i in body(flask.request, 'instruments')]).run().toJSON()
 
 
 
-class UserEndpoint(Resource):
+class PollUserEndpoint(Resource):
     def get(self, poll: str, id:int) -> str: 
         if queryParam(flask.request, 'details'):
             return GetUserDetails(poll, id).run().toJSON()
         else:
             return GetUserWithInstruments(poll, id).run().toJSON()
     
     @history
@@ -124,23 +125,23 @@
 
 
 
 
 
 
 
-class DatesEndpoint(Resource):
+class PollDatesEndpoint(Resource):
     def get(self, poll: str) -> str: return GetDates(poll).run().toJSON()
     
     @history
     def post(self, poll: str) -> str: return CreateDate(poll, body(flask.request, 'title'), body(flask.request, 'date'), body(flask.request, 'time', mandatory=False), body(flask.request, 'end_time', mandatory=False)).run().toJSON()
 
 
 
-class DateEndpoint(Resource):
+class PollDateEndpoint(Resource):
     def get(self, poll: str, id:int) -> str:
         if queryParam(flask.request, 'details'):
             return GetDateDetails(poll, id).run().toJSON()
         else:
             return GetDate(poll, id).run().toJSON()
     
     @history
@@ -151,53 +152,63 @@
 
 
 
 
 
 
 
-class AnswersEndpoint(Resource):
+class PollAnswersEndpoint(Resource):
     
     @history
     def post(self, poll: str) -> str: return CreateAnswer(poll, body(flask.request, 'user_id'), body(flask.request, 'date_id')).run().toJSON()
 
 
-class AnswerEndpoint(Resource):
+class PollAnswerEndpoint(Resource):
     
     def get(self, poll: str, id:int) -> str: return GetAnswer(poll, id).run().toJSON()
     
     @history
     def put(self, poll: str, id: int) -> str: return UpdateAnswer(poll, id, body(flask.request, 'response')).run().toJSON()
     
     @history
     def delete(self, poll: str, id: int) -> str: return DeleteAnswer(poll, id).run().toJSON()
 
-class GetAnswerEndpoint(Resource):
+class PollGetAnswerEndpoint(Resource):
     def get(self, poll: str, userId: int, dateId: int) -> str: return GetSearchAnswer(poll, userId, dateId).run().toJSON()
 
 
-class SessionEndpoint(Resource):
+class PollSessionEndpoint(Resource):
     def get(self, poll: str, id: str) -> str: return GetSession(poll, id).run().toJSON()
     
     @history
     def post(self, poll: str, id: str) -> str: return CreateSession(poll, id, body(flask.request, 'user_id')).run().toJSON()
 
 
 
 
-api.add_resource(PollEndpoint, '/<string:poll>')
-api.add_resource(InstrumentsEndpoint, '/<string:poll>/instrument')
-api.add_resource(UsersEndpoint, '/<string:poll>/user')
-api.add_resource(UserEndpoint, '/<string:poll>/user/<int:id>')
-api.add_resource(DatesEndpoint, '/<string:poll>/date')
-api.add_resource(DateEndpoint, '/<string:poll>/date/<int:id>')
-api.add_resource(AnswersEndpoint, '/<string:poll>/answer')
-api.add_resource(AnswerEndpoint, '/<string:poll>/answer/<int:id>')
-api.add_resource(GetAnswerEndpoint, '/<string:poll>/answer/<int:userId>/<int:dateId>')
-api.add_resource(SessionEndpoint, '/<string:poll>/session/<string:id>')
+class SessionEndpoint(Resource):
+    def get(self, id: str) -> str: return GetAllSession(id).run().toJSON()
+
+
+
+
+
+api.add_resource(SessionEndpoint, '/session/<string:id>')
+
+api.add_resource(PollPollEndpoint, '/<string:poll>')
+api.add_resource(PollInstrumentsEndpoint, '/<string:poll>/instrument')
+api.add_resource(PollUsersEndpoint, '/<string:poll>/user')
+api.add_resource(PollUserEndpoint, '/<string:poll>/user/<int:id>')
+api.add_resource(PollDatesEndpoint, '/<string:poll>/date')
+api.add_resource(PollDateEndpoint, '/<string:poll>/date/<int:id>')
+api.add_resource(PollAnswersEndpoint, '/<string:poll>/answer')
+api.add_resource(PollAnswerEndpoint, '/<string:poll>/answer/<int:id>')
+api.add_resource(PollGetAnswerEndpoint, '/<string:poll>/answer/<int:userId>/<int:dateId>')
+api.add_resource(PollSessionEndpoint, '/<string:poll>/session/<string:id>')
+
 
 def get_options():
     parser = argparse.ArgumentParser()
     parser.add_argument('--host', help='the hostname to listen on', default='0.0.0.0')
     parser.add_argument('--port', help='the port of the webserver', default=4444)
     parser.add_argument('--debug', help='Enable debugging', action='store_true')
     return parser
```

### Comparing `popoll_backend-0.0.57/popoll_backend/model/db/answer.py` & `popoll_backend-0.0.58/popoll_backend/model/db/answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/popoll_backend/model/db/date.py` & `popoll_backend-0.0.58/popoll_backend/model/db/date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/popoll_backend/model/db/session.py` & `popoll_backend-0.0.58/popoll_backend/model/db/session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/popoll_backend/model/db/user.py` & `popoll_backend-0.0.58/popoll_backend/model/db/user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/popoll_backend/model/db/user_instruments.py` & `popoll_backend-0.0.58/popoll_backend/model/db/user_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/popoll_backend/model/payload/date_details.py` & `popoll_backend-0.0.58/popoll_backend/model/payload/date_details.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/popoll_backend/model/payload/history.py` & `popoll_backend-0.0.58/popoll_backend/model/payload/history.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/popoll_backend/model/payload/user_details.py` & `popoll_backend-0.0.58/popoll_backend/model/payload/user_details.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/popoll_backend/model/payload/user_with_instruments.py` & `popoll_backend-0.0.58/popoll_backend/model/payload/user_with_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/popoll_backend/query/__init__.py` & `popoll_backend-0.0.58/popoll_backend/query/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import flask
 import os
 import sqlite3
 
-from typing import List, Type, Optional
+from typing import List, Optional
 
 from popoll_backend.model import Payload
 
 class Query:
     
+    def run(self) -> Payload:
+        raise NotImplementedError()
+
+class PollQuery(Query):
+    
     fail_if_db_exists: bool = False
     fail_if_db_not_exists: bool = True
     
     def __init__(self, poll: str):
         self.poll = poll
         self.db_file = f'{poll}.db'
         if self.fail_if_db_exists and os.path.exists(self.db_file):
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/create_answer.py` & `popoll_backend-0.0.58/popoll_backend/query/create_answer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sqlite3
 
 import flask
 
 from popoll_backend.model.db.answer import Answer
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class CreateAnswer(Query):
+class CreateAnswer(PollQuery):
     
     user_id: int
     date_id: int
     
     id: int
     
     def __init__(self, poll:str, user_id: int, date_id: int):
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/create_date.py` & `popoll_backend-0.0.58/popoll_backend/query/create_date.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import sqlite3
 from typing import Optional
 
 from popoll_backend.model.db.date import Date
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class CreateDate(Query):
+class CreateDate(PollQuery):
     
     title: str
     date: datetime.date
     time: Optional[datetime.time]
     end_time: Optional[datetime.time]
     
     id: int
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/create_instrument.py` & `popoll_backend-0.0.58/popoll_backend/query/create_instrument.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sqlite3
 
 from popoll_backend.model.db.instrument import Instrument
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class CreateInstrument(Query):
+class CreateInstrument(PollQuery):
     
     name: str
     rank: int
     
     instrument_id: int
     
     def __init__(self, poll: str, name: str, rank: int):
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/create_poll.py` & `popoll_backend-0.0.58/popoll_backend/query/create_poll.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from popoll_backend.model.db.date import Date
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.option import Option
 from popoll_backend.model.db.session import Session
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.id_payload import IdPayload
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class CreatePoll(Query):
+class CreatePoll(PollQuery):
     
     fail_if_db_exists: bool = True
     fail_if_db_not_exists: bool = False
     
     name: str
     instruments: List[str]
     color: str
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/create_session.py` & `popoll_backend-0.0.58/popoll_backend/query/create_session.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import sqlite3
 
 from popoll_backend.model.db.session import Session
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class CreateSession(Query):
+class CreateSession(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: str, user_id: int):
         super().__init__(poll)
         self.id = id
         self.user_id = user_id
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/create_user.py` & `popoll_backend-0.0.58/popoll_backend/query/create_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from typing import List
 
 from popoll_backend.model import Payload
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class CreateUser(Query):
+class CreateUser(PollQuery):
     
     name: str
     main_instrument: int
     instruments: List[int]
     
     id: int
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/delete_answer.py` & `popoll_backend-0.0.58/popoll_backend/query/delete_answer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sqlite3
 from popoll_backend.model import Payload
 from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.id_payload import IdPayload
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class DeleteAnswer(Query):
+class DeleteAnswer(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/delete_date.py` & `popoll_backend-0.0.58/popoll_backend/query/delete_date.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sqlite3
 from popoll_backend.model import Payload
 from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.id_payload import IdPayload
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class DeleteDate(Query):
+class DeleteDate(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/delete_instrument.py` & `popoll_backend-0.0.58/popoll_backend/query/delete_instrument.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sqlite3
 from popoll_backend.model import Payload
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.id_payload import IdPayload
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class DeleteInstrument(Query):
+class DeleteInstrument(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/delete_user.py` & `popoll_backend-0.0.58/popoll_backend/query/delete_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sqlite3
 from popoll_backend.model import Payload
 from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.id_payload import IdPayload
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class DeleteUser(Query):
+class DeleteUser(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/get_all_instruments.py` & `popoll_backend-0.0.58/popoll_backend/query/get_all_instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sqlite3
 from typing import List
 
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.payload.instruments import Instruments
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class GetAllInstruments(Query):
+class GetAllInstruments(PollQuery):
     
     instruments: List[Instrument]
     
     def __init__(self, poll: str):
         super().__init__(poll)
 
     def process(self, cursor: sqlite3.Cursor) -> None:
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/get_date.py` & `popoll_backend-0.0.58/popoll_backend/query/get_date.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sqlite3
 
 from popoll_backend.model import Payload
 from popoll_backend.model.db.date import Date
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class GetDate(Query):
+class GetDate(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/get_date_details.py` & `popoll_backend-0.0.58/popoll_backend/query/get_date_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from popoll_backend.model.db.answer import Answer
 from popoll_backend.model.db.date import Date
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.date_details import DateDetails
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class GetDateDetails(Query):
+class GetDateDetails(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/get_dates.py` & `popoll_backend-0.0.58/popoll_backend/query/get_dates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sqlite3
 from typing import List
 
 from popoll_backend.model.db.date import Date
 from popoll_backend.model.payload.dates import Dates
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class GetDates(Query):
+class GetDates(PollQuery):
     
     dates: List[Date]
     
     def __init__(self, poll: str):
         super().__init__(poll)
 
     def process(self, cursor: sqlite3.Cursor):
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/get_instrument.py` & `popoll_backend-0.0.58/popoll_backend/query/get_instrument.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sqlite3
 
 from popoll_backend.model.db.instrument import Instrument
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class GetInstrument(Query):
+class GetInstrument(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/get_instruments.py` & `popoll_backend-0.0.58/popoll_backend/query/get_instruments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sqlite3
 from typing import List
 
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.payload.instruments import Instruments
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class GetInstruments(Query):
+class GetInstruments(PollQuery):
     
     instruments: List[Instrument]
     
     def __init__(self, poll: str):
         super().__init__(poll)
 
     def process(self, cursor: sqlite3.Cursor) -> None:
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/get_search_answer.py` & `popoll_backend-0.0.58/popoll_backend/query/get_search_answer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sqlite3
 
 import flask
 
 from popoll_backend.model.db.answer import Answer
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class GetSearchAnswer(Query):
+class GetSearchAnswer(PollQuery):
     
     userId: int
     dateId: int
     
     def __init__(self, poll: str, userId: int, dateId: int):
         super().__init__(poll)
         self.userId = userId
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/get_session.py` & `popoll_backend-0.0.58/popoll_backend/query/get_session.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sqlite3
 
 from popoll_backend.model.db.session import Session
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class GetSession(Query):
+class GetSession(PollQuery):
     
     id: int
     session: Session
     
     def __init__(self, poll: str, id: str):
         super().__init__(poll)
         self.id = id
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/get_user_details.py` & `popoll_backend-0.0.58/popoll_backend/query/get_user_details.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sqlite3
 
 from popoll_backend.model.db.answer import Answer
 from popoll_backend.model.db.date import Date
 from popoll_backend.model.db.user import User
 from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
 from popoll_backend.model.payload.user_details import UserDetails
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class GetUserDetails(Query):
+class GetUserDetails(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/get_user_with_instruments.py` & `popoll_backend-0.0.58/popoll_backend/query/get_user_with_instruments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import sqlite3
 
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class GetUserWithInstruments(Query):
+class GetUserWithInstruments(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/get_users.py` & `popoll_backend-0.0.58/popoll_backend/query/get_users.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sqlite3
 from typing import List
 
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.users import Users
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class GetUsers(Query):
+class GetUsers(PollQuery):
     
     def __init__(self, poll: str):
         super().__init__(poll)
     
     def process(self, cursor: sqlite3.Cursor) -> None:
         pass
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/update_answer.py` & `popoll_backend-0.0.58/popoll_backend/query/update_answer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import sqlite3
 from typing import Optional
 
 from popoll_backend.model import Payload
 from popoll_backend.model.db.answer import Answer
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 from popoll_backend.query.get_answer import GetAnswer
 
 
-class UpdateAnswer(Query):
+class UpdateAnswer(PollQuery):
     
     id: int
     response: Optional[bool]
     
     def __init__(self, poll:str, id: int, response: Optional[bool]):
         super().__init__(poll)
         self.id = id
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/update_date.py` & `popoll_backend-0.0.58/popoll_backend/query/update_date.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import sqlite3
 from typing import Optional
 
 from popoll_backend.model.db.date import Date
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class UpdateDate(Query):
+class UpdateDate(PollQuery):
     
     id: int
     title: str
     date: datetime.date
     time: Optional[datetime.time]
     end_time: Optional[datetime.time]
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/update_poll.py` & `popoll_backend-0.0.58/popoll_backend/query/update_poll.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sqlite3
 
 from popoll_backend.model.db.option import Option
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class UpdatePoll(Query):
+class UpdatePoll(PollQuery):
     
     name: str
     color: str
     
     def __init__(self, poll: str, name: str, color: str):
         super().__init__(poll)
         self.name = name
```

### Comparing `popoll_backend-0.0.57/popoll_backend/query/update_user.py` & `popoll_backend-0.0.58/popoll_backend/query/update_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import flask
 
 from popoll_backend.model import Payload
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
-from popoll_backend.query import Query
+from popoll_backend.query import PollQuery
 
 
-class UpdateUser(Query):
+class UpdateUser(PollQuery):
     
     id: int
     name: str
     main_instrument: int
     instruments: List[int]
     
     def __init__(self, poll, id, name, main_instrument, instruments):
```

### Comparing `popoll_backend-0.0.57/popoll_backend.egg-info/PKG-INFO` & `popoll_backend-0.0.58/popoll_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.57
+Version: 0.0.58
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `popoll_backend-0.0.57/popoll_backend.egg-info/SOURCES.txt` & `popoll_backend-0.0.58/popoll_backend.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 popoll_backend/model/payload/__init__.py
 popoll_backend/model/payload/date_details.py
 popoll_backend/model/payload/dates.py
 popoll_backend/model/payload/empty.py
 popoll_backend/model/payload/history.py
 popoll_backend/model/payload/id_payload.py
 popoll_backend/model/payload/instruments.py
+popoll_backend/model/payload/polls.py
 popoll_backend/model/payload/user_details.py
 popoll_backend/model/payload/user_with_instruments.py
 popoll_backend/model/payload/users.py
 popoll_backend/model/payload/users_payload_details.py
 popoll_backend/query/__init__.py
 popoll_backend/query/create_answer.py
 popoll_backend/query/create_date.py
@@ -34,14 +35,15 @@
 popoll_backend/query/create_session.py
 popoll_backend/query/create_user.py
 popoll_backend/query/delete_answer.py
 popoll_backend/query/delete_date.py
 popoll_backend/query/delete_instrument.py
 popoll_backend/query/delete_user.py
 popoll_backend/query/get_all_instruments.py
+popoll_backend/query/get_all_sessions.py
 popoll_backend/query/get_answer.py
 popoll_backend/query/get_date.py
 popoll_backend/query/get_date_details.py
 popoll_backend/query/get_dates.py
 popoll_backend/query/get_instrument.py
 popoll_backend/query/get_instruments.py
 popoll_backend/query/get_poll.py
@@ -69,8 +71,9 @@
 tests/test_16_update_date.py
 tests/test_17_delete_date.py
 tests/test_18_create_answer.py
 tests/test_19_update_answer.py
 tests/test_20_delete_answer.py
 tests/test_21_get_answer.py
 tests/test_22_get_search_answer.py
-tests/test_23_get_create_session.py
+tests/test_23_get_create_session.py
+tests/test_24_get_all_session.py
```

### Comparing `popoll_backend-0.0.57/pyproject.toml` & `popoll_backend-0.0.58/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", 'wheel', 'flask', 'flask_cors', 'flask-restful', 'jsonpickle', 'sqlalchemy', 'sqlalchemy-utils', 'psycopg2-binary', 'pyyaml', 'pyopenssl']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "popoll_backend"
-version = "0.0.57"
+version = "0.0.58"
 authors = [
   { name="vivi5421", email="pypi@villard.me" },
 ]
 description = "A small example package"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
```

### Comparing `popoll_backend-0.0.57/tests/test_01_get_poll.py` & `popoll_backend-0.0.58/tests/test_01_get_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_02_create_poll.py` & `popoll_backend-0.0.58/tests/test_02_create_poll.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import contextlib
 import os
-from tests import IntegrationTest
+from tests import DB_NAME, IntegrationTest
 
 class TestCreatePoll(IntegrationTest):
     
+    DB_NAME_2 = 'DB2'
+    
     def test_db_creation(self):
         _json = self.get_instruments(False)
         
         self.assertEqual(self.instru1_id, _json['instruments'][0]['id'])
         self.assertEqual(self.INSTRU1, _json['instruments'][0]['name'])
         self.assertEqual(self.instru2_id, _json['instruments'][1]['id'])
         self.assertEqual(self.INSTRU2, _json['instruments'][1]['name'])
         self.assertEqual(self.instru3_id, _json['instruments'][2]['id'])
         self.assertEqual(self.INSTRU3, _json['instruments'][2]['name'])
         
     def test_can_create_another_db(self):
-        _json = self.create_poll(f'{self.db_name}2', f'/{self.db_name}2', '#ff8b00')
+        _json = self.create_poll(self.DB_NAME_2, self.DB_NAME_2, '#ff8b00')
         self.assertEqual(0, _json['id'])
 
     def test_no_duplicate_poll_id(self):
-        rs = self.create_poll(f'{self.db_name}', f'/{self.db_name}2', '#ff8b00', fail=True)
+        rs = self.create_poll(DB_NAME, self.DB_NAME_2, '#ff8b00', fail=True)
         self.assertEqual(409, rs.status_code)
         
     def tearDown(self):
-        with contextlib.suppress(FileNotFoundError): os.remove(f'{self.db_name}2.db')
+        self.tearDown_db(self.DB_NAME_2)
```

### Comparing `popoll_backend-0.0.57/tests/test_04_get_instruments.py` & `popoll_backend-0.0.58/tests/test_04_get_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_08_get_users.py` & `popoll_backend-0.0.58/tests/test_08_get_users.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_09_create_user.py` & `popoll_backend-0.0.58/tests/test_09_create_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_10_get_user.py` & `popoll_backend-0.0.58/tests/test_10_get_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_11_update_user.py` & `popoll_backend-0.0.58/tests/test_11_update_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_12_delete_user.py` & `popoll_backend-0.0.58/tests/test_12_delete_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_13_get_dates.py` & `popoll_backend-0.0.58/tests/test_13_get_dates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_14_create_date.py` & `popoll_backend-0.0.58/tests/test_14_create_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_15_get_date.py` & `popoll_backend-0.0.58/tests/test_15_get_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_16_update_date.py` & `popoll_backend-0.0.58/tests/test_16_update_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_17_delete_date.py` & `popoll_backend-0.0.58/tests/test_17_delete_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_18_create_answer.py` & `popoll_backend-0.0.58/tests/test_18_create_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_19_update_answer.py` & `popoll_backend-0.0.58/tests/test_19_update_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_20_delete_answer.py` & `popoll_backend-0.0.58/tests/test_20_delete_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_21_get_answer.py` & `popoll_backend-0.0.58/tests/test_21_get_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_22_get_search_answer.py` & `popoll_backend-0.0.58/tests/test_22_get_search_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.57/tests/test_23_get_create_session.py` & `popoll_backend-0.0.58/tests/test_23_get_create_session.py`

 * *Files identical despite different names*

