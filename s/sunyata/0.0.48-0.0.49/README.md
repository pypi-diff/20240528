# Comparing `tmp/sunyata-0.0.48.tar.gz` & `tmp/sunyata-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunyata-0.0.48.tar", last modified: Tue May 28 08:55:10 2024, max compression
+gzip compressed data, was "sunyata-0.0.49.tar", last modified: Tue May 28 09:11:44 2024, max compression
```

## Comparing `sunyata-0.0.48.tar` & `sunyata-0.0.49.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:55:09.998650 sunyata-0.0.48/
--rw-r--r--   0 root         (0) staff       (20)     1087 2023-02-28 12:29:05.000000 sunyata-0.0.48/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      526 2024-05-28 08:55:09.998000 sunyata-0.0.48/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)    12510 2023-08-17 08:05:55.000000 sunyata-0.0.48/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2024-05-28 08:55:09.998885 sunyata-0.0.48/setup.cfg
--rwxr-xr-x   0 root         (0) staff       (20)     1134 2024-05-28 08:54:52.000000 sunyata-0.0.48/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:55:09.850007 sunyata-0.0.48/sunyata/
--rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.48/sunyata/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:55:09.940854 sunyata-0.0.48/sunyata/algorithm/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.48/sunyata/algorithm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.48/sunyata/algorithm/avlsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.48/sunyata/algorithm/avltree.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.48/sunyata/algorithm/binsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.48/sunyata/algorithm/bintree.py
--rw-r--r--   0 root         (0) staff       (20)     1083 2023-09-25 12:45:23.000000 sunyata-0.0.48/sunyata/algorithm/bloomfilter.py
--rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.48/sunyata/algorithm/bplustree.py
--rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.48/sunyata/algorithm/btree.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.48/sunyata/algorithm/hashtable.py
--rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.48/sunyata/algorithm/lru.py
--rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.48/sunyata/algorithm/rbtree.py
--rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.48/sunyata/algorithm/trie.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2024-05-22 12:15:19.000000 sunyata-0.0.48/sunyata/cache_wrap.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:55:09.949441 sunyata-0.0.48/sunyata/cli/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.48/sunyata/cli/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.48/sunyata/cli/cli.py
--rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.48/sunyata/cli/entry.py
--rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.48/sunyata/compress.py
--rw-r--r--   0 root         (0) staff       (20)      242 2024-05-22 12:12:16.000000 sunyata-0.0.48/sunyata/concurrent.py
--rw-r--r--   0 root         (0) staff       (20)     3599 2023-04-25 07:31:21.000000 sunyata-0.0.48/sunyata/consul.py
--rw-r--r--   0 root         (0) staff       (20)    13615 2023-08-08 02:12:19.000000 sunyata-0.0.48/sunyata/db.py
--rw-r--r--   0 root         (0) staff       (20)     2233 2023-04-25 07:31:21.000000 sunyata-0.0.48/sunyata/etcd.py
--rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.48/sunyata/eventloop.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:55:09.972748 sunyata-0.0.48/sunyata/http/
--rw-r--r--   0 root         (0) staff       (20)       68 2023-04-13 06:36:26.000000 sunyata-0.0.48/sunyata/http/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.48/sunyata/http/factory.py
--rw-r--r--   0 root         (0) staff       (20)      536 2023-08-17 07:56:55.000000 sunyata-0.0.48/sunyata/http/middleware.py
--rw-r--r--   0 root         (0) staff       (20)     3952 2024-05-28 08:27:23.000000 sunyata-0.0.48/sunyata/http/rawserver.py
--rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.48/sunyata/http/request.py
--rw-r--r--   0 root         (0) staff       (20)      182 2023-04-25 07:23:36.000000 sunyata-0.0.48/sunyata/http/request_stream.py
--rw-r--r--   0 root         (0) staff       (20)     1639 2023-04-14 10:00:43.000000 sunyata-0.0.48/sunyata/http/response.py
--rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.48/sunyata/http/router.py
--rw-r--r--   0 root         (0) staff       (20)     3701 2023-11-30 08:11:39.000000 sunyata-0.0.48/sunyata/http/server.py
--rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.48/sunyata/http/status.py
--rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.48/sunyata/http/transport.py
--rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.48/sunyata/log.py
--rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.48/sunyata/orm.py
--rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.48/sunyata/redislock.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:55:09.996357 sunyata-0.0.48/sunyata/rpc/
--rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.48/sunyata/rpc/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8159 2023-04-25 07:31:21.000000 sunyata-0.0.48/sunyata/rpc/client.py
--rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.48/sunyata/rpc/compress.py
--rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.48/sunyata/rpc/const.py
--rw-r--r--   0 root         (0) staff       (20)     2474 2023-05-06 03:27:50.000000 sunyata-0.0.48/sunyata/rpc/discovery.py
--rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.48/sunyata/rpc/encrypt.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.48/sunyata/rpc/exception.py
--rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.48/sunyata/rpc/method.py
--rw-r--r--   0 root         (0) staff       (20)     2840 2023-04-13 06:02:14.000000 sunyata-0.0.48/sunyata/rpc/protocal.py
--rw-r--r--   0 root         (0) staff       (20)      702 2023-04-20 03:17:34.000000 sunyata-0.0.48/sunyata/rpc/serialize.py
--rw-r--r--   0 root         (0) staff       (20)    13094 2024-05-28 08:27:25.000000 sunyata-0.0.48/sunyata/rpc/server.py
--rw-r--r--   0 root         (0) staff       (20)     7774 2023-04-25 07:31:21.000000 sunyata-0.0.48/sunyata/rpc/transport.py
--rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.48/sunyata/table_writer.py
--rw-r--r--   0 root         (0) staff       (20)      497 2023-04-20 03:17:34.000000 sunyata-0.0.48/sunyata/util.py
--rw-r--r--   0 root         (0) staff       (20)     4081 2023-08-22 12:18:48.000000 sunyata-0.0.48/sunyata/wrap.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 08:55:09.872182 sunyata-0.0.48/sunyata.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      526 2024-05-28 08:55:09.000000 sunyata-0.0.48/sunyata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1456 2024-05-28 08:55:09.000000 sunyata-0.0.48/sunyata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-05-28 08:55:09.000000 sunyata-0.0.48/sunyata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       52 2024-05-28 08:55:09.000000 sunyata-0.0.48/sunyata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       71 2024-05-28 08:55:09.000000 sunyata-0.0.48/sunyata.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       63 2024-05-28 08:55:09.000000 sunyata-0.0.48/sunyata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 09:11:44.229972 sunyata-0.0.49/
+-rw-r--r--   0 root         (0) staff       (20)     1087 2023-02-28 12:29:05.000000 sunyata-0.0.49/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      526 2024-05-28 09:11:44.228658 sunyata-0.0.49/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)    12510 2023-08-17 08:05:55.000000 sunyata-0.0.49/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-28 09:11:44.230293 sunyata-0.0.49/setup.cfg
+-rwxr-xr-x   0 root         (0) staff       (20)     1134 2024-05-28 09:10:48.000000 sunyata-0.0.49/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 09:11:44.103257 sunyata-0.0.49/sunyata/
+-rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.49/sunyata/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 09:11:44.153708 sunyata-0.0.49/sunyata/algorithm/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.49/sunyata/algorithm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.49/sunyata/algorithm/avlsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.49/sunyata/algorithm/avltree.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.49/sunyata/algorithm/binsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.49/sunyata/algorithm/bintree.py
+-rw-r--r--   0 root         (0) staff       (20)     1083 2023-09-25 12:45:23.000000 sunyata-0.0.49/sunyata/algorithm/bloomfilter.py
+-rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.49/sunyata/algorithm/bplustree.py
+-rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.49/sunyata/algorithm/btree.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.49/sunyata/algorithm/hashtable.py
+-rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.49/sunyata/algorithm/lru.py
+-rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.49/sunyata/algorithm/rbtree.py
+-rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.49/sunyata/algorithm/trie.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2024-05-22 12:15:19.000000 sunyata-0.0.49/sunyata/cache_wrap.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 09:11:44.158735 sunyata-0.0.49/sunyata/cli/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.49/sunyata/cli/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.49/sunyata/cli/cli.py
+-rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.49/sunyata/cli/entry.py
+-rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.49/sunyata/compress.py
+-rw-r--r--   0 root         (0) staff       (20)      242 2024-05-22 12:12:16.000000 sunyata-0.0.49/sunyata/concurrent.py
+-rw-r--r--   0 root         (0) staff       (20)     3599 2023-04-25 07:31:21.000000 sunyata-0.0.49/sunyata/consul.py
+-rw-r--r--   0 root         (0) staff       (20)    13615 2023-08-08 02:12:19.000000 sunyata-0.0.49/sunyata/db.py
+-rw-r--r--   0 root         (0) staff       (20)     2233 2023-04-25 07:31:21.000000 sunyata-0.0.49/sunyata/etcd.py
+-rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.49/sunyata/eventloop.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 09:11:44.193852 sunyata-0.0.49/sunyata/http/
+-rw-r--r--   0 root         (0) staff       (20)       68 2023-04-13 06:36:26.000000 sunyata-0.0.49/sunyata/http/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.49/sunyata/http/factory.py
+-rw-r--r--   0 root         (0) staff       (20)      536 2023-08-17 07:56:55.000000 sunyata-0.0.49/sunyata/http/middleware.py
+-rw-r--r--   0 root         (0) staff       (20)     3984 2024-05-28 09:06:07.000000 sunyata-0.0.49/sunyata/http/rawserver.py
+-rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.49/sunyata/http/request.py
+-rw-r--r--   0 root         (0) staff       (20)      182 2023-04-25 07:23:36.000000 sunyata-0.0.49/sunyata/http/request_stream.py
+-rw-r--r--   0 root         (0) staff       (20)     1639 2023-04-14 10:00:43.000000 sunyata-0.0.49/sunyata/http/response.py
+-rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.49/sunyata/http/router.py
+-rw-r--r--   0 root         (0) staff       (20)     3701 2023-11-30 08:11:39.000000 sunyata-0.0.49/sunyata/http/server.py
+-rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.49/sunyata/http/status.py
+-rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.49/sunyata/http/transport.py
+-rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.49/sunyata/log.py
+-rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.49/sunyata/orm.py
+-rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.49/sunyata/redislock.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 09:11:44.226629 sunyata-0.0.49/sunyata/rpc/
+-rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.49/sunyata/rpc/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8223 2024-05-28 09:09:50.000000 sunyata-0.0.49/sunyata/rpc/client.py
+-rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.49/sunyata/rpc/compress.py
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.49/sunyata/rpc/const.py
+-rw-r--r--   0 root         (0) staff       (20)     2474 2023-05-06 03:27:50.000000 sunyata-0.0.49/sunyata/rpc/discovery.py
+-rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.49/sunyata/rpc/encrypt.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.49/sunyata/rpc/exception.py
+-rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.49/sunyata/rpc/method.py
+-rw-r--r--   0 root         (0) staff       (20)     2840 2023-04-13 06:02:14.000000 sunyata-0.0.49/sunyata/rpc/protocal.py
+-rw-r--r--   0 root         (0) staff       (20)      702 2023-04-20 03:17:34.000000 sunyata-0.0.49/sunyata/rpc/serialize.py
+-rw-r--r--   0 root         (0) staff       (20)    13158 2024-05-28 09:06:35.000000 sunyata-0.0.49/sunyata/rpc/server.py
+-rw-r--r--   0 root         (0) staff       (20)     7774 2023-04-25 07:31:21.000000 sunyata-0.0.49/sunyata/rpc/transport.py
+-rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.49/sunyata/table_writer.py
+-rw-r--r--   0 root         (0) staff       (20)      497 2023-04-20 03:17:34.000000 sunyata-0.0.49/sunyata/util.py
+-rw-r--r--   0 root         (0) staff       (20)     4081 2023-08-22 12:18:48.000000 sunyata-0.0.49/sunyata/wrap.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-28 09:11:44.117153 sunyata-0.0.49/sunyata.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      526 2024-05-28 09:11:43.000000 sunyata-0.0.49/sunyata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1456 2024-05-28 09:11:43.000000 sunyata-0.0.49/sunyata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-28 09:11:43.000000 sunyata-0.0.49/sunyata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       52 2024-05-28 09:11:43.000000 sunyata-0.0.49/sunyata.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       71 2024-05-28 09:11:43.000000 sunyata-0.0.49/sunyata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       63 2024-05-28 09:11:43.000000 sunyata-0.0.49/sunyata.egg-info/top_level.txt
```

### Comparing `sunyata-0.0.48/LICENSE` & `sunyata-0.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/PKG-INFO` & `sunyata-0.0.49/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunyata
-Version: 0.0.48
+Version: 0.0.49
 Summary: Light, simple, asynchronous RPC framework for Python
 Home-page: UNKNOWN
 Author: tank
 License: MIT
 Keywords: sunyata
 Platform: any
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `sunyata-0.0.48/README.md` & `sunyata-0.0.49/README.md`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/setup.py` & `sunyata-0.0.49/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DEFINE_VERSION = '0.0.48'
+DEFINE_VERSION = '0.0.49'
 from setuptools import setup
 
 requireList = [
     'lz4==3.1.3',
     'ujson==1.35',
     'uvicorn==0.17.0',
     'aiohttp==3.8.0',
```

### Comparing `sunyata-0.0.48/sunyata/algorithm/bloomfilter.py` & `sunyata-0.0.49/sunyata/algorithm/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/algorithm/hashtable.py` & `sunyata-0.0.49/sunyata/algorithm/hashtable.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/algorithm/lru.py` & `sunyata-0.0.49/sunyata/algorithm/lru.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/algorithm/trie.py` & `sunyata-0.0.49/sunyata/algorithm/trie.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/cache_wrap.py` & `sunyata-0.0.49/sunyata/cache_wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/cli/cli.py` & `sunyata-0.0.49/sunyata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/consul.py` & `sunyata-0.0.49/sunyata/consul.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/db.py` & `sunyata-0.0.49/sunyata/db.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/etcd.py` & `sunyata-0.0.49/sunyata/etcd.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/http/factory.py` & `sunyata-0.0.49/sunyata/http/factory.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/http/middleware.py` & `sunyata-0.0.49/sunyata/http/middleware.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/http/rawserver.py` & `sunyata-0.0.49/sunyata/http/rawserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         server = await asyncio.start_server(self.acceptStream, self.bind, self.port)
         tasklist.append(server.serve_forever())
         for task in tasklist:
             await task
 
     def serve(self):
         print('http running on http://%s:%s' % (self.bind, self.port) )
-        asyncio.run(self.listenAndServe())
+        asyncio.get_event_loop().run_until_complete(self.listenAndServe())
 
     @classmethod
     def route(cls, path, methods = None):
         def wrapper(func):
             cls.addRoute(path, func, methods)
             return func
         return wrapper
```

### Comparing `sunyata-0.0.48/sunyata/http/request.py` & `sunyata-0.0.49/sunyata/http/request.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/http/response.py` & `sunyata-0.0.49/sunyata/http/response.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/http/server.py` & `sunyata-0.0.49/sunyata/http/server.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/http/status.py` & `sunyata-0.0.49/sunyata/http/status.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/http/transport.py` & `sunyata-0.0.49/sunyata/http/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/log.py` & `sunyata-0.0.49/sunyata/log.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/orm.py` & `sunyata-0.0.49/sunyata/orm.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/redislock.py` & `sunyata-0.0.49/sunyata/redislock.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/rpc/client.py` & `sunyata-0.0.49/sunyata/rpc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         self.serversCount = len(self.servers)
         self.serversProtocalMap = {}
         self.serverIndex = 0
         self.lastServer = ''
         self.timeout = 10
 
     def getInstance(self):
-        instanceList = asyncio.run(self.discovery.getInstanceList(self.discoveryConfig.serviceName))
+        instanceList = asyncio.get_event_loop().run_until_complete(self.discovery.getInstanceList(self.discoveryConfig.serviceName))
         instanceLength  = len(instanceList)
         if instanceLength == 0:
             raise Exception('no instance found')
         index = self.instanceIndex % instanceLength
         self.instanceIndex = self.instanceIndex + 1
         return instanceList[index]
 
@@ -211,15 +211,15 @@
         self.beforeCall()
         package = {
             'func' : func,
             'args' : args,
             'kwargs' : kwargs,
         }
         msg = self.protocal.serialize(package)
-        respmsg = asyncio.run(self.protocal.transport.send(msg))
+        respmsg = asyncio.new_event_loop().run_until_complete(self.protocal.transport.send(msg))
         resp = self.protocal.unserialize(respmsg)
         if isinstance(resp, FuncNotFoundException):
             raise resp
         return resp
 
     def getProtocalInstance(self, instance):
         key = "%s:%s:%s" % (instance.service, instance.address, instance.port)
```

### Comparing `sunyata-0.0.48/sunyata/rpc/discovery.py` & `sunyata-0.0.49/sunyata/rpc/discovery.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/rpc/method.py` & `sunyata-0.0.49/sunyata/rpc/method.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/rpc/protocal.py` & `sunyata-0.0.49/sunyata/rpc/protocal.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/rpc/serialize.py` & `sunyata-0.0.49/sunyata/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/rpc/server.py` & `sunyata-0.0.49/sunyata/rpc/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             registTask = asyncio.create_task(self.discovery.asyncRegist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True))
             tasks.append(registTask)
         await asyncio.wait(tasks)
 
     def serve(self):
         print('http rpc running on http://%s:%s' % (self.host, self.port) )
         self.dumpRpcFuncs()
-        asyncio.run(self.asyncServe())
+        asyncio.get_event_loop().run_until_complete(self.asyncServe())
 
 
 class TcpRpcServer(BlockTcpRpcServer):
 
     def __init__(self, host, port):
         BlockTcpRpcServer.__init__(self, host, port)
         self.host = host
@@ -342,11 +342,11 @@
         server = rs[-1]
         # Close the server
         server.close()
         loop.run_until_complete(server.wait_closed())
         loop.close()
     
     def serve(self):
-        asyncio.run(self.asyncServe())
+        asyncio.get_event_loop().run_until_complete(self.asyncServe())
 
 
 rpc = RpcServer.rpc
```

### Comparing `sunyata-0.0.48/sunyata/rpc/transport.py` & `sunyata-0.0.49/sunyata/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/table_writer.py` & `sunyata-0.0.49/sunyata/table_writer.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata/wrap.py` & `sunyata-0.0.49/sunyata/wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.48/sunyata.egg-info/PKG-INFO` & `sunyata-0.0.49/sunyata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunyata
-Version: 0.0.48
+Version: 0.0.49
 Summary: Light, simple, asynchronous RPC framework for Python
 Home-page: UNKNOWN
 Author: tank
 License: MIT
 Keywords: sunyata
 Platform: any
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `sunyata-0.0.48/sunyata.egg-info/SOURCES.txt` & `sunyata-0.0.49/sunyata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

