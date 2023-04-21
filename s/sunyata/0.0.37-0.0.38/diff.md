# Comparing `tmp/sunyata-0.0.37.tar.gz` & `tmp/sunyata-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sunyata-0.0.37.tar", last modified: Thu Apr 20 03:19:06 2023, max compression
+gzip compressed data, was "dist/sunyata-0.0.38.tar", last modified: Fri Apr 21 02:51:42 2023, max compression
```

## Comparing `sunyata-0.0.37.tar` & `sunyata-0.0.38.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-20 03:19:06.000000 sunyata-0.0.37/
--rw-r--r--   0 root         (0) staff       (20)      486 2023-04-20 03:19:06.000000 sunyata-0.0.37/PKG-INFO
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-20 03:19:06.000000 sunyata-0.0.37/sunyata.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      486 2023-04-20 03:19:05.000000 sunyata-0.0.37/sunyata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1399 2023-04-20 03:19:05.000000 sunyata-0.0.37/sunyata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)       52 2023-04-20 03:19:05.000000 sunyata-0.0.37/sunyata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       70 2023-04-20 03:19:05.000000 sunyata-0.0.37/sunyata.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       63 2023-04-20 03:19:05.000000 sunyata-0.0.37/sunyata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-04-20 03:19:05.000000 sunyata-0.0.37/sunyata.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-20 03:19:06.000000 sunyata-0.0.37/sunyata/
--rw-r--r--   0 root         (0) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.37/sunyata/db.py
--rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.37/sunyata/log.py
--rw-r--r--   0 root         (0) staff       (20)      497 2023-04-20 03:17:34.000000 sunyata-0.0.37/sunyata/util.py
--rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.37/sunyata/orm.py
--rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.37/sunyata/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.37/sunyata/eventloop.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-20 03:19:06.000000 sunyata-0.0.37/sunyata/cli/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.37/sunyata/cli/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.37/sunyata/cli/cli.py
--rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.37/sunyata/cli/entry.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-20 03:19:06.000000 sunyata-0.0.37/sunyata/algorithm/
--rw-r--r--   0 root         (0) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.37/sunyata/algorithm/bloomfilter.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.37/sunyata/algorithm/binsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.37/sunyata/algorithm/rbtree.py
--rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.37/sunyata/algorithm/avltree.py
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.37/sunyata/algorithm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.37/sunyata/algorithm/bplustree.py
--rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.37/sunyata/algorithm/btree.py
--rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.37/sunyata/algorithm/bintree.py
--rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.37/sunyata/algorithm/lru.py
--rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.37/sunyata/algorithm/trie.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.37/sunyata/algorithm/hashtable.py
--rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.37/sunyata/algorithm/avlsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.37/sunyata/redislock.py
--rw-r--r--   0 root         (0) staff       (20)     1761 2023-04-20 03:17:34.000000 sunyata-0.0.37/sunyata/etcd.py
--rw-r--r--   0 root         (0) staff       (20)     3718 2023-04-20 03:17:34.000000 sunyata-0.0.37/sunyata/consul.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-20 03:19:06.000000 sunyata-0.0.37/sunyata/http/
--rw-r--r--   0 root         (0) staff       (20)     3103 2023-04-14 09:55:44.000000 sunyata-0.0.37/sunyata/http/server.py
--rw-r--r--   0 root         (0) staff       (20)      182 2023-04-12 02:31:22.000000 sunyata-0.0.37/sunyata/http/request_stream.py
--rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.37/sunyata/http/transport.py
--rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.37/sunyata/http/request.py
--rw-r--r--   0 root         (0) staff       (20)       68 2023-04-13 06:36:26.000000 sunyata-0.0.37/sunyata/http/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1639 2023-04-14 10:00:43.000000 sunyata-0.0.37/sunyata/http/response.py
--rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.37/sunyata/http/factory.py
--rw-r--r--   0 root         (0) staff       (20)     3394 2023-04-20 03:05:05.000000 sunyata-0.0.37/sunyata/http/rawserver.py
--rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.37/sunyata/http/router.py
--rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.37/sunyata/http/status.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.37/sunyata/cache_wrap.py
--rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.37/sunyata/compress.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-20 03:19:06.000000 sunyata-0.0.37/sunyata/rpc/
--rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.37/sunyata/rpc/encrypt.py
--rw-r--r--   0 root         (0) staff       (20)      702 2023-04-20 03:17:34.000000 sunyata-0.0.37/sunyata/rpc/serialize.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.37/sunyata/rpc/exception.py
--rw-r--r--   0 root         (0) staff       (20)    11783 2023-04-20 03:17:34.000000 sunyata-0.0.37/sunyata/rpc/server.py
--rw-r--r--   0 root         (0) staff       (20)     2437 2023-04-20 03:17:34.000000 sunyata-0.0.37/sunyata/rpc/discovery.py
--rw-r--r--   0 root         (0) staff       (20)     8307 2023-04-12 02:48:07.000000 sunyata-0.0.37/sunyata/rpc/transport.py
--rw-r--r--   0 root         (0) staff       (20)     8117 2023-04-20 03:17:34.000000 sunyata-0.0.37/sunyata/rpc/client.py
--rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.37/sunyata/rpc/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.37/sunyata/rpc/compress.py
--rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.37/sunyata/rpc/method.py
--rw-r--r--   0 root         (0) staff       (20)     2840 2023-04-13 06:02:14.000000 sunyata-0.0.37/sunyata/rpc/protocal.py
--rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.37/sunyata/rpc/const.py
--rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.37/sunyata/table_writer.py
--rw-r--r--   0 root         (0) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.37/sunyata/wrap.py
--rw-r--r--   0 root         (0) staff       (20)    10354 2023-04-20 03:17:34.000000 sunyata-0.0.37/README.md
--rwxr-xr-x   0 root         (0) staff       (20)     1026 2023-04-20 03:17:34.000000 sunyata-0.0.37/setup.py
--rw-r--r--   0 root         (0) staff       (20)       38 2023-04-20 03:19:06.000000 sunyata-0.0.37/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/
+-rw-r--r--   0 root         (0) staff       (20)      486 2023-04-21 02:51:42.000000 sunyata-0.0.38/PKG-INFO
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      486 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1399 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)       52 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       70 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       63 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata/
+-rw-r--r--   0 root         (0) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/db.py
+-rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/log.py
+-rw-r--r--   0 root         (0) staff       (20)      497 2023-04-20 03:17:34.000000 sunyata-0.0.38/sunyata/util.py
+-rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/orm.py
+-rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/eventloop.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata/cli/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/cli/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/cli/cli.py
+-rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/cli/entry.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata/algorithm/
+-rw-r--r--   0 root         (0) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/algorithm/bloomfilter.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.38/sunyata/algorithm/binsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.38/sunyata/algorithm/rbtree.py
+-rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.38/sunyata/algorithm/avltree.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/algorithm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.38/sunyata/algorithm/bplustree.py
+-rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.38/sunyata/algorithm/btree.py
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.38/sunyata/algorithm/bintree.py
+-rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/algorithm/lru.py
+-rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/algorithm/trie.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/algorithm/hashtable.py
+-rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.38/sunyata/algorithm/avlsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/redislock.py
+-rw-r--r--   0 root         (0) staff       (20)     1724 2023-04-20 12:48:28.000000 sunyata-0.0.38/sunyata/etcd.py
+-rw-r--r--   0 root         (0) staff       (20)     3718 2023-04-20 03:17:34.000000 sunyata-0.0.38/sunyata/consul.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata/http/
+-rw-r--r--   0 root         (0) staff       (20)     3251 2023-04-20 08:32:35.000000 sunyata-0.0.38/sunyata/http/server.py
+-rw-r--r--   0 root         (0) staff       (20)      182 2023-04-12 02:31:22.000000 sunyata-0.0.38/sunyata/http/request_stream.py
+-rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.38/sunyata/http/transport.py
+-rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.38/sunyata/http/request.py
+-rw-r--r--   0 root         (0) staff       (20)       68 2023-04-13 06:36:26.000000 sunyata-0.0.38/sunyata/http/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1639 2023-04-14 10:00:43.000000 sunyata-0.0.38/sunyata/http/response.py
+-rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.38/sunyata/http/factory.py
+-rw-r--r--   0 root         (0) staff       (20)     3394 2023-04-20 03:05:05.000000 sunyata-0.0.38/sunyata/http/rawserver.py
+-rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.38/sunyata/http/router.py
+-rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.38/sunyata/http/status.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/cache_wrap.py
+-rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/compress.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata/rpc/
+-rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/rpc/encrypt.py
+-rw-r--r--   0 root         (0) staff       (20)      702 2023-04-20 03:17:34.000000 sunyata-0.0.38/sunyata/rpc/serialize.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/rpc/exception.py
+-rw-r--r--   0 root         (0) staff       (20)    12146 2023-04-20 08:39:54.000000 sunyata-0.0.38/sunyata/rpc/server.py
+-rw-r--r--   0 root         (0) staff       (20)     2437 2023-04-20 06:50:23.000000 sunyata-0.0.38/sunyata/rpc/discovery.py
+-rw-r--r--   0 root         (0) staff       (20)     8307 2023-04-12 02:48:07.000000 sunyata-0.0.38/sunyata/rpc/transport.py
+-rw-r--r--   0 root         (0) staff       (20)     8117 2023-04-21 02:49:05.000000 sunyata-0.0.38/sunyata/rpc/client.py
+-rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/rpc/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/rpc/compress.py
+-rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/rpc/method.py
+-rw-r--r--   0 root         (0) staff       (20)     2840 2023-04-13 06:02:14.000000 sunyata-0.0.38/sunyata/rpc/protocal.py
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/rpc/const.py
+-rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/table_writer.py
+-rw-r--r--   0 root         (0) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/wrap.py
+-rw-r--r--   0 root         (0) staff       (20)    10444 2023-04-21 02:46:28.000000 sunyata-0.0.38/README.md
+-rwxr-xr-x   0 root         (0) staff       (20)     1026 2023-04-21 02:50:58.000000 sunyata-0.0.38/setup.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-04-21 02:51:42.000000 sunyata-0.0.38/setup.cfg
```

### Comparing `sunyata-0.0.37/sunyata.egg-info/SOURCES.txt` & `sunyata-0.0.38/sunyata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/db.py` & `sunyata-0.0.38/sunyata/db.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/log.py` & `sunyata-0.0.38/sunyata/log.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/orm.py` & `sunyata-0.0.38/sunyata/orm.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/cli/cli.py` & `sunyata-0.0.38/sunyata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/algorithm/bloomfilter.py` & `sunyata-0.0.38/sunyata/algorithm/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/algorithm/lru.py` & `sunyata-0.0.38/sunyata/algorithm/lru.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/algorithm/trie.py` & `sunyata-0.0.38/sunyata/algorithm/trie.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/algorithm/hashtable.py` & `sunyata-0.0.38/sunyata/algorithm/hashtable.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/redislock.py` & `sunyata-0.0.38/sunyata/redislock.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/etcd.py` & `sunyata-0.0.38/sunyata/etcd.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
         r = requests.put(url, timeout=self.timeout, headers=self.headers)
         print(r.text, r.status_code)
 
     def getServiceInstanceList(self, serviceName: str) -> list:
         url = self.baseUrl + '/v2/keys/sunyata-services/%s' % serviceName
         r = requests.get(url, timeout=self.timeout, headers=self.headers)
         dic = ujson.loads(r.text)
-        print(r.status_code, r.text)
         nodes = dic.get('node').get('nodes', [])
         instanceList = []
         for node in nodes:
             value = node.get('value')
             ip, port = value.split(':')
             instance = Instance(
                 service=serviceName,
```

### Comparing `sunyata-0.0.37/sunyata/consul.py` & `sunyata-0.0.38/sunyata/consul.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/http/server.py` & `sunyata-0.0.38/sunyata/http/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,19 @@
         RawHttpServer.__init__(self, bind=bind, port=port)
         self.config = uvicorn.Config("sunyata.http.server:HttpServer", host=self.bind, port=self.port, log_level=log_level)
 
     def serve(self):
         server = uvicorn.Server(self.config)
         print('http running on http://%s:%s' % (self.bind, self.port) )
         server.run()
+
+    async def asyncServe(self):
+        server = uvicorn.Server(self.config)
+        server.config.setup_event_loop()
+        await server.serve()
     
     async def genHttpRequest(self, scheme, httpVersion, method, path, queryString, headers, body, clientTuple):
         httpRequest = HttpRequest()
         httpRequest.scheme = scheme
         httpRequest.httpVersion = httpVersion
         httpRequest.method = method
         httpRequest.uri = path
```

### Comparing `sunyata-0.0.37/sunyata/http/transport.py` & `sunyata-0.0.38/sunyata/http/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/http/request.py` & `sunyata-0.0.38/sunyata/http/request.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/http/response.py` & `sunyata-0.0.38/sunyata/http/response.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/http/factory.py` & `sunyata-0.0.38/sunyata/http/factory.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/http/rawserver.py` & `sunyata-0.0.38/sunyata/http/rawserver.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/http/status.py` & `sunyata-0.0.38/sunyata/http/status.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/cache_wrap.py` & `sunyata-0.0.38/sunyata/cache_wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/rpc/serialize.py` & `sunyata-0.0.38/sunyata/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/rpc/server.py` & `sunyata-0.0.38/sunyata/rpc/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,18 @@
 import inspect
 from sunyata.http.server import HttpServer
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
 
 class RpcServer(object):
 
-    __slots__ = ('discoveryConfig', 'discovery', 'protocal')
-
     funcMap = {}
     funcList = []
 
     def __init__(self):
-        #self.funcMap = {}
-        #self.funcList = []
         self.discoveryConfig = None
         self.discovery = None
         self.protocal = RpcProtocal()
 
     @classmethod
     def regist(cls, func):
         if isinstance(func, FunctionType):
@@ -157,22 +153,33 @@
         if isEnableCompress == b'1':
             msg = RpcCompress.decompress(msg)
         request = self.protocal.unserialize(msg)
         func, args, kwargs = self.protocal.parseRequest(request)
         resp = self.run(func, args, kwargs)
         resp = self.protocal.serialize(resp)
         return resp
+    
+    async def asyncServe(self):
+        tasks = []
+        tasks.append(self.app.asyncServe())
+        if self.discovery and self.discoveryConfig:
+            registTask = asyncio.create_task(self.discovery.asyncRegist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True))
+            tasks.append(registTask)
+        await asyncio.wait(tasks)
 
     def serve(self):
+        asyncio.run(self.asyncServe())
+        """
         tRegist = None
         if self.discovery and self.discoveryConfig:
             self.discovery.regist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
         self.printLogo()
         print('http rpc running on http://%s:%s' % (self.host, self.port) )
         self.app.serve()
+        """
 
 
 class TcpRpcServer(BlockTcpRpcServer):
 
     def __init__(self, host, port):
         BlockTcpRpcServer.__init__(self, host, port)
         self.host = host
```

### Comparing `sunyata-0.0.37/sunyata/rpc/discovery.py` & `sunyata-0.0.38/sunyata/rpc/discovery.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/rpc/transport.py` & `sunyata-0.0.38/sunyata/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/rpc/client.py` & `sunyata-0.0.38/sunyata/rpc/client.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/rpc/method.py` & `sunyata-0.0.38/sunyata/rpc/method.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/rpc/protocal.py` & `sunyata-0.0.38/sunyata/rpc/protocal.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/table_writer.py` & `sunyata-0.0.38/sunyata/table_writer.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/sunyata/wrap.py` & `sunyata-0.0.38/sunyata/wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.37/README.md` & `sunyata-0.0.38/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 
 ## 简介
 sunyata是一个Python3 RPC框架，client和server既可以直连，也可以通过Consul或ETCD做服务注册发现。
 
 ## 特性
 - 像本地函数一样调用
 - 使用简单，用户只需要关注业务即可
-- HTTP/UDP/TCP 全协议支持
-- 支持异步 async/await
-- 支持服务注册、发现
+- 支持HTTP/UDP/TCP协议
+- 支持异步async/await
+- 支持通过consul或etcd的服务注册发现
+- 支持所有数据类型，包括自定义的类对象等都可作为参数
 
 ## 安装
 Python 版本 >= 3.6
 ```
 pip install sunyata
 ```
 
@@ -156,15 +157,15 @@
 cli = UdpRpcClient('127.0.0.1', 9988)
 resp = cli.call('sayHello', name = 'xiaoming' )
 print(resp)
 ```
 
 ## 服务发现
 除了客户端与服务端直连，也支持服务注册发现（客户端与服务端直连的例子，请参考上面的TcpRpcServer部分）。
-目前仅支持基于Consul的服务发现，未来计划支持etcd。下面的例子以TCP为例。
+目前支持基于Consul 或 etcd 进行服务注册发现， 下面的例子先以Consul为例。
 
 
 ### 基于Consul的服务注册发现
 基于Consul的Check机制，服务注册后，自动添加一个定期的检查任务。默认为TCP端口检查，支持TCP/HTTP RPC服务端，UDP服务端暂不支持。一旦服务进程挂掉，那么客户端会请求到其他健康的服务端节点上。
 
 ### 快速开始
 - 第一步，你需要定义一个DiscoverConfig对象。
```

### Comparing `sunyata-0.0.37/setup.py` & `sunyata-0.0.38/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DEFINE_VERSION = '0.0.37'
+DEFINE_VERSION = '0.0.38'
 from setuptools import setup
 
 requireList = [
     'lz4==3.1.3',
     'requests==2.25.1',
     'ujson==1.35',
     'uvloop==0.19.0'
```

