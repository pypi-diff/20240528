# Comparing `tmp/sunyata-0.0.46.tar.gz` & `tmp/sunyata-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sunyata-0.0.46.tar", last modified: Thu Nov 30 08:52:40 2023, max compression
+gzip compressed data, was "sunyata-0.0.47.tar", last modified: Tue May 28 08:48:59 2024, max compression
```

## Comparing `sunyata-0.0.46.tar` & `sunyata-0.0.47.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-11-30 08:52:40.000000 sunyata-0.0.46/
--rw-r--r--   0 root         (0) staff       (20)      537 2023-11-30 08:52:40.000000 sunyata-0.0.46/PKG-INFO
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-11-30 08:52:40.000000 sunyata-0.0.46/sunyata.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      537 2023-11-30 08:52:40.000000 sunyata-0.0.46/sunyata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1448 2023-11-30 08:52:40.000000 sunyata-0.0.46/sunyata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)       52 2023-11-30 08:52:40.000000 sunyata-0.0.46/sunyata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       86 2023-11-30 08:52:40.000000 sunyata-0.0.46/sunyata.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       63 2023-11-30 08:52:40.000000 sunyata-0.0.46/sunyata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-11-30 08:52:40.000000 sunyata-0.0.46/sunyata.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-11-30 08:52:40.000000 sunyata-0.0.46/sunyata/
--rw-r--r--   0 root         (0) staff       (20)    13615 2023-08-08 02:12:19.000000 sunyata-0.0.46/sunyata/db.py
--rw-r--r--   0 root         (0) staff       (20)      306 2023-07-05 07:23:02.000000 sunyata-0.0.46/sunyata/concurrent.py
--rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.46/sunyata/log.py
--rw-r--r--   0 root         (0) staff       (20)      497 2023-04-20 03:17:34.000000 sunyata-0.0.46/sunyata/util.py
--rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.46/sunyata/orm.py
--rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.46/sunyata/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.46/sunyata/eventloop.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-11-30 08:52:40.000000 sunyata-0.0.46/sunyata/cli/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.46/sunyata/cli/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.46/sunyata/cli/cli.py
--rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.46/sunyata/cli/entry.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-11-30 08:52:40.000000 sunyata-0.0.46/sunyata/algorithm/
--rw-r--r--   0 root         (0) staff       (20)     1083 2023-09-25 12:45:23.000000 sunyata-0.0.46/sunyata/algorithm/bloomfilter.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.46/sunyata/algorithm/binsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.46/sunyata/algorithm/rbtree.py
--rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.46/sunyata/algorithm/avltree.py
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.46/sunyata/algorithm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.46/sunyata/algorithm/bplustree.py
--rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.46/sunyata/algorithm/btree.py
--rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.46/sunyata/algorithm/bintree.py
--rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.46/sunyata/algorithm/lru.py
--rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.46/sunyata/algorithm/trie.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.46/sunyata/algorithm/hashtable.py
--rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.46/sunyata/algorithm/avlsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.46/sunyata/redislock.py
--rw-r--r--   0 root         (0) staff       (20)     2233 2023-04-25 07:31:21.000000 sunyata-0.0.46/sunyata/etcd.py
--rw-r--r--   0 root         (0) staff       (20)     3599 2023-04-25 07:31:21.000000 sunyata-0.0.46/sunyata/consul.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-11-30 08:52:40.000000 sunyata-0.0.46/sunyata/http/
--rw-r--r--   0 root         (0) staff       (20)     3701 2023-11-30 08:11:39.000000 sunyata-0.0.46/sunyata/http/server.py
--rw-r--r--   0 root         (0) staff       (20)      182 2023-04-25 07:23:36.000000 sunyata-0.0.46/sunyata/http/request_stream.py
--rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.46/sunyata/http/transport.py
--rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.46/sunyata/http/request.py
--rw-r--r--   0 root         (0) staff       (20)       68 2023-04-13 06:36:26.000000 sunyata-0.0.46/sunyata/http/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1639 2023-04-14 10:00:43.000000 sunyata-0.0.46/sunyata/http/response.py
--rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.46/sunyata/http/factory.py
--rw-r--r--   0 root         (0) staff       (20)     3950 2023-08-17 07:57:30.000000 sunyata-0.0.46/sunyata/http/rawserver.py
--rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.46/sunyata/http/router.py
--rw-r--r--   0 root         (0) staff       (20)      536 2023-08-17 07:56:55.000000 sunyata-0.0.46/sunyata/http/middleware.py
--rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.46/sunyata/http/status.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.46/sunyata/cache_wrap.py
--rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.46/sunyata/compress.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-11-30 08:52:40.000000 sunyata-0.0.46/sunyata/rpc/
--rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.46/sunyata/rpc/encrypt.py
--rw-r--r--   0 root         (0) staff       (20)      702 2023-04-20 03:17:34.000000 sunyata-0.0.46/sunyata/rpc/serialize.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.46/sunyata/rpc/exception.py
--rw-r--r--   0 root         (0) staff       (20)    13092 2023-11-30 08:12:33.000000 sunyata-0.0.46/sunyata/rpc/server.py
--rw-r--r--   0 root         (0) staff       (20)     2474 2023-05-06 03:27:50.000000 sunyata-0.0.46/sunyata/rpc/discovery.py
--rw-r--r--   0 root         (0) staff       (20)     7774 2023-04-25 07:31:21.000000 sunyata-0.0.46/sunyata/rpc/transport.py
--rw-r--r--   0 root         (0) staff       (20)     8159 2023-04-25 07:31:21.000000 sunyata-0.0.46/sunyata/rpc/client.py
--rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.46/sunyata/rpc/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.46/sunyata/rpc/compress.py
--rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.46/sunyata/rpc/method.py
--rw-r--r--   0 root         (0) staff       (20)     2840 2023-04-13 06:02:14.000000 sunyata-0.0.46/sunyata/rpc/protocal.py
--rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.46/sunyata/rpc/const.py
--rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.46/sunyata/table_writer.py
--rw-r--r--   0 root         (0) staff       (20)     4081 2023-08-22 12:18:48.000000 sunyata-0.0.46/sunyata/wrap.py
--rw-r--r--   0 root         (0) staff       (20)    12510 2023-08-17 08:05:55.000000 sunyata-0.0.46/README.md
--rwxr-xr-x   0 root         (0) staff       (20)     1134 2023-11-30 08:50:55.000000 sunyata-0.0.46/setup.py
--rw-r--r--   0 root         (0) staff       (20)       38 2023-11-30 08:52:40.000000 sunyata-0.0.46/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:48:59.564510 sunyata-0.0.47/
+-rw-r--r--   0 root         (0) staff       (20)     1087 2023-02-28 12:29:05.000000 sunyata-0.0.47/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      526 2024-05-28 08:48:59.564188 sunyata-0.0.47/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)    12510 2023-08-17 08:05:55.000000 sunyata-0.0.47/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-28 08:48:59.564616 sunyata-0.0.47/setup.cfg
+-rwxr-xr-x   0 root         (0) staff       (20)     1134 2024-05-28 08:44:45.000000 sunyata-0.0.47/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:48:59.494349 sunyata-0.0.47/sunyata/
+-rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.47/sunyata/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:48:59.522887 sunyata-0.0.47/sunyata/algorithm/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.47/sunyata/algorithm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.47/sunyata/algorithm/avlsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.47/sunyata/algorithm/avltree.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.47/sunyata/algorithm/binsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.47/sunyata/algorithm/bintree.py
+-rw-r--r--   0 root         (0) staff       (20)     1083 2023-09-25 12:45:23.000000 sunyata-0.0.47/sunyata/algorithm/bloomfilter.py
+-rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.47/sunyata/algorithm/bplustree.py
+-rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.47/sunyata/algorithm/btree.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.47/sunyata/algorithm/hashtable.py
+-rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.47/sunyata/algorithm/lru.py
+-rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.47/sunyata/algorithm/rbtree.py
+-rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.47/sunyata/algorithm/trie.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2024-05-22 12:15:19.000000 sunyata-0.0.47/sunyata/cache_wrap.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:48:59.526623 sunyata-0.0.47/sunyata/cli/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.47/sunyata/cli/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.47/sunyata/cli/cli.py
+-rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.47/sunyata/cli/entry.py
+-rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.47/sunyata/compress.py
+-rw-r--r--   0 root         (0) staff       (20)      242 2024-05-22 12:12:16.000000 sunyata-0.0.47/sunyata/concurrent.py
+-rw-r--r--   0 root         (0) staff       (20)     3599 2023-04-25 07:31:21.000000 sunyata-0.0.47/sunyata/consul.py
+-rw-r--r--   0 root         (0) staff       (20)    13615 2023-08-08 02:12:19.000000 sunyata-0.0.47/sunyata/db.py
+-rw-r--r--   0 root         (0) staff       (20)     2233 2023-04-25 07:31:21.000000 sunyata-0.0.47/sunyata/etcd.py
+-rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.47/sunyata/eventloop.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:48:59.541678 sunyata-0.0.47/sunyata/http/
+-rw-r--r--   0 root         (0) staff       (20)       68 2023-04-13 06:36:26.000000 sunyata-0.0.47/sunyata/http/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.47/sunyata/http/factory.py
+-rw-r--r--   0 root         (0) staff       (20)      536 2023-08-17 07:56:55.000000 sunyata-0.0.47/sunyata/http/middleware.py
+-rw-r--r--   0 root         (0) staff       (20)     3952 2024-05-28 08:27:23.000000 sunyata-0.0.47/sunyata/http/rawserver.py
+-rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.47/sunyata/http/request.py
+-rw-r--r--   0 root         (0) staff       (20)      182 2023-04-25 07:23:36.000000 sunyata-0.0.47/sunyata/http/request_stream.py
+-rw-r--r--   0 root         (0) staff       (20)     1639 2023-04-14 10:00:43.000000 sunyata-0.0.47/sunyata/http/response.py
+-rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.47/sunyata/http/router.py
+-rw-r--r--   0 root         (0) staff       (20)     3701 2023-11-30 08:11:39.000000 sunyata-0.0.47/sunyata/http/server.py
+-rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.47/sunyata/http/status.py
+-rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.47/sunyata/http/transport.py
+-rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.47/sunyata/log.py
+-rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.47/sunyata/orm.py
+-rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.47/sunyata/redislock.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:48:59.563480 sunyata-0.0.47/sunyata/rpc/
+-rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.47/sunyata/rpc/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8159 2023-04-25 07:31:21.000000 sunyata-0.0.47/sunyata/rpc/client.py
+-rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.47/sunyata/rpc/compress.py
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.47/sunyata/rpc/const.py
+-rw-r--r--   0 root         (0) staff       (20)     2474 2023-05-06 03:27:50.000000 sunyata-0.0.47/sunyata/rpc/discovery.py
+-rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.47/sunyata/rpc/encrypt.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.47/sunyata/rpc/exception.py
+-rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.47/sunyata/rpc/method.py
+-rw-r--r--   0 root         (0) staff       (20)     2840 2023-04-13 06:02:14.000000 sunyata-0.0.47/sunyata/rpc/protocal.py
+-rw-r--r--   0 root         (0) staff       (20)      702 2023-04-20 03:17:34.000000 sunyata-0.0.47/sunyata/rpc/serialize.py
+-rw-r--r--   0 root         (0) staff       (20)    13094 2024-05-28 08:27:25.000000 sunyata-0.0.47/sunyata/rpc/server.py
+-rw-r--r--   0 root         (0) staff       (20)     7774 2023-04-25 07:31:21.000000 sunyata-0.0.47/sunyata/rpc/transport.py
+-rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.47/sunyata/table_writer.py
+-rw-r--r--   0 root         (0) staff       (20)      497 2023-04-20 03:17:34.000000 sunyata-0.0.47/sunyata/util.py
+-rw-r--r--   0 root         (0) staff       (20)     4081 2023-08-22 12:18:48.000000 sunyata-0.0.47/sunyata/wrap.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:48:59.503372 sunyata-0.0.47/sunyata.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      526 2024-05-28 08:48:59.000000 sunyata-0.0.47/sunyata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1456 2024-05-28 08:48:59.000000 sunyata-0.0.47/sunyata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-28 08:48:59.000000 sunyata-0.0.47/sunyata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       52 2024-05-28 08:48:59.000000 sunyata-0.0.47/sunyata.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       71 2024-05-28 08:48:59.000000 sunyata-0.0.47/sunyata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       63 2024-05-28 08:48:59.000000 sunyata-0.0.47/sunyata.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sunyata-0.0.46/PKG-INFO` & `sunyata-0.0.47/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sunyata
-Version: 0.0.46
+Version: 0.0.47
 Summary: Light, simple, asynchronous RPC framework for Python
 Home-page: UNKNOWN
 Author: tank
-Author-email: UNKNOWN
 License: MIT
-Description: UNKNOWN
 Keywords: sunyata
 Platform: any
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `sunyata-0.0.46/sunyata.egg-info/PKG-INFO` & `sunyata-0.0.47/sunyata.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sunyata
-Version: 0.0.46
+Version: 0.0.47
 Summary: Light, simple, asynchronous RPC framework for Python
 Home-page: UNKNOWN
 Author: tank
-Author-email: UNKNOWN
 License: MIT
-Description: UNKNOWN
 Keywords: sunyata
 Platform: any
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `sunyata-0.0.46/sunyata.egg-info/SOURCES.txt` & `sunyata-0.0.47/sunyata.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 sunyata/__init__.py
 sunyata/cache_wrap.py
 sunyata/compress.py
 sunyata/concurrent.py
 sunyata/consul.py
```

### Comparing `sunyata-0.0.46/sunyata/db.py` & `sunyata-0.0.47/sunyata/db.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/log.py` & `sunyata-0.0.47/sunyata/log.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/orm.py` & `sunyata-0.0.47/sunyata/orm.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/cli/cli.py` & `sunyata-0.0.47/sunyata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/algorithm/bloomfilter.py` & `sunyata-0.0.47/sunyata/algorithm/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/algorithm/lru.py` & `sunyata-0.0.47/sunyata/algorithm/lru.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/algorithm/trie.py` & `sunyata-0.0.47/sunyata/algorithm/trie.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/algorithm/hashtable.py` & `sunyata-0.0.47/sunyata/algorithm/hashtable.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/redislock.py` & `sunyata-0.0.47/sunyata/redislock.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/etcd.py` & `sunyata-0.0.47/sunyata/etcd.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/consul.py` & `sunyata-0.0.47/sunyata/consul.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/http/server.py` & `sunyata-0.0.47/sunyata/http/server.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/http/transport.py` & `sunyata-0.0.47/sunyata/http/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/http/request.py` & `sunyata-0.0.47/sunyata/http/request.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/http/response.py` & `sunyata-0.0.47/sunyata/http/response.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/http/factory.py` & `sunyata-0.0.47/sunyata/http/factory.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/http/rawserver.py` & `sunyata-0.0.47/sunyata/http/rawserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from sunyata.http.status import *
 from sunyata.http.request_stream import RequestStream
 from sunyata.http.response import HttpResponse
 from sunyata.table_writer import TableWriter
 from traceback import format_exc
 from types import MethodType,FunctionType
 import asyncio
-import uvloop
+#import uvloop
 import inspect
-asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+#asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
 
 class RawHttpServer(object):
 
     routerMap = {}
     responseTypeConvertMap = {
         set: HttpResponse.responseConvertSetToJson,
```

### Comparing `sunyata-0.0.46/sunyata/http/middleware.py` & `sunyata-0.0.47/sunyata/http/middleware.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/http/status.py` & `sunyata-0.0.47/sunyata/http/status.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/cache_wrap.py` & `sunyata-0.0.47/sunyata/cache_wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/rpc/serialize.py` & `sunyata-0.0.47/sunyata/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/rpc/server.py` & `sunyata-0.0.47/sunyata/rpc/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 import socket
 from sunyata.rpc.discovery import DiscoveryConfig, RpcDiscovery
 import struct
 from sunyata.rpc.compress import RpcCompress
 from types import FunctionType
 from sunyata.rpc.method import RpcMethod
 import asyncio
-import uvloop
+#import uvloop
 import inspect
 from sunyata.http.server import HttpServer
 from sunyata.table_writer import TableWriter
 import time
-asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+#asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
 
 class RpcServer(object):
 
     funcMap = {}
     funcList = []
```

### Comparing `sunyata-0.0.46/sunyata/rpc/discovery.py` & `sunyata-0.0.47/sunyata/rpc/discovery.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/rpc/transport.py` & `sunyata-0.0.47/sunyata/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/rpc/client.py` & `sunyata-0.0.47/sunyata/rpc/client.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/rpc/method.py` & `sunyata-0.0.47/sunyata/rpc/method.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/rpc/protocal.py` & `sunyata-0.0.47/sunyata/rpc/protocal.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/table_writer.py` & `sunyata-0.0.47/sunyata/table_writer.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/sunyata/wrap.py` & `sunyata-0.0.47/sunyata/wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/README.md` & `sunyata-0.0.47/README.md`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.46/setup.py` & `sunyata-0.0.47/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-DEFINE_VERSION = '0.0.46'
+DEFINE_VERSION = '0.0.47'
 from setuptools import setup
 
 requireList = [
     'lz4==3.1.3',
     'ujson==1.35',
-    'uvloop==0.17.0',
     'uvicorn==0.18.0',
     'aiohttp==3.8.4',
     'requests==2.30.0',
     #'PyMySQL==0.10.1',
     #'DBUtils==1.3',
-     #'dataclasses-json==0.5.13',
+    #'dataclasses-json==0.5.13',
+    #'uvloop==0.17.0',
 ]
 
 setup(
     name='sunyata',
     version=DEFINE_VERSION,
     description='Light, simple, asynchronous RPC framework for Python',
     author='tank',
```

