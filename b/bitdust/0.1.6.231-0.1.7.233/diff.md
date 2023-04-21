# Comparing `tmp/bitdust-0.1.6.231.tar.gz` & `tmp/bitdust-0.1.7.233.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitdust-0.1.6.231.tar", last modified: Sun Jan 29 11:48:56 2023, max compression
+gzip compressed data, was "dist/bitdust-0.1.7.233.tar", last modified: Fri Apr 21 14:01:38 2023, max compression
```

## Comparing `bitdust-0.1.6.231.tar` & `bitdust-0.1.7.233.tar`

### file list

```diff
@@ -1,468 +1,482 @@
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.588984 bitdust-0.1.6.231/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9005 2023-01-29 11:48:56.588984 bitdust-0.1.6.231/PKG-INFO
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6011 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/README.txt
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.528984 bitdust-0.1.6.231/bitdust/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1803 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/__init__.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.532984 bitdust-0.1.6.231/bitdust/access/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      882 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/access/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8145 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/access/group_access_donor.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    69935 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/access/group_member.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    27158 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/access/groups.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    35302 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/access/key_ring.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    45703 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/access/shared_access_coordinator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    16003 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/access/shared_access_donor.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.532984 bitdust-0.1.6.231/bitdust/automats/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/automats/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    28621 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/automats/automat.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4035 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/automats/global_state.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.532984 bitdust-0.1.6.231/bitdust/blockchain/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      882 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/blockchain/__init__.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.532984 bitdust-0.1.6.231/bitdust/broadcast/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/broadcast/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7494 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/broadcast/broadcast_listener.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4803 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/broadcast/broadcast_service.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14662 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/broadcast/broadcaster_node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10000 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/broadcast/broadcasters_finder.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.536984 bitdust-0.1.6.231/bitdust/chat/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      876 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/chat/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3306 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/chat/kbhit.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    29641 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/chat/message_database.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5675 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/chat/message_keeper.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11276 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/chat/nickname_holder.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11315 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/chat/nickname_observer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10358 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/chat/terminal_chat.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.536984 bitdust-0.1.6.231/bitdust/coins/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      877 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    16133 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/accountant_node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10172 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/accountants_finder.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13995 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/coins_db.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7339 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/coins_index.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6480 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/coins_io.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17260 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/coins_miner.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10287 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/contract_chain_consumer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7023 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/contract_chain_node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10444 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/customer_contract_executor.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6104 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/mine_old.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5311 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/miner_old.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11275 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/coins/supplier_contract_executor.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.536984 bitdust-0.1.6.231/bitdust/contacts/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      884 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/contacts/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    38445 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/contacts/contactsdb.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3829 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/contacts/friends.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    21012 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/contacts/identitycache.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14809 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/contacts/identitydb.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.536984 bitdust-0.1.6.231/bitdust/crypt/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      877 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/crypt/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5835 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/crypt/certificate.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4029 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/crypt/cipher.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11851 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/crypt/encrypted.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3253 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/crypt/hashes.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13081 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/crypt/key.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    39203 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/crypt/my_keys.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2799 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/crypt/number.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8811 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/crypt/rsa_key.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17628 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/crypt/signed.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.536984 bitdust-0.1.6.231/bitdust/currency/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/currency/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7434 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/currency/geth_service.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.536984 bitdust-0.1.6.231/bitdust/customer/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/customer/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    41073 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/customer/fire_hire.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13849 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/customer/list_files_orator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    26487 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/customer/supplier_connector.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13424 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/customer/supplier_finder.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.540984 bitdust-0.1.6.231/bitdust/dht/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      954 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/dht/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10289 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/dht/dht_records.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14437 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/dht/dht_relations.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    62442 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/dht/dht_service.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4098 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/dht/known_nodes.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.540984 bitdust-0.1.6.231/bitdust/interface/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/interface/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)   237997 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/interface/api.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    53720 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/interface/api_rest_http_server.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11461 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/interface/api_web_socket.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    57996 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/interface/cmd_line_json.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7069 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/interface/cmd_line_json_templates.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    22207 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/interface/ftp_server.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.540984 bitdust-0.1.6.231/bitdust/lib/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      969 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7701 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/diskspace.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2799 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/getsizeof.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10243 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/jsn.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    40342 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/jsontemplate.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11193 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/maths.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    31961 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/misc.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8488 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/nameurl.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    30816 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/net_misc.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    16067 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/packetid.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    15989 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/schedule.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3508 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/serialization.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2760 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/strng.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    23049 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/txws.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10343 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/udp.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2382 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/utime.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13150 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/lib/websock.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.544984 bitdust-0.1.6.231/bitdust/logs/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/logs/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    25603 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/logs/lg.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3211 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/logs/measure_it.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1890 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/logs/memdebug.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8227 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/logs/weblog.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10403 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/logs/webtraffic.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.544984 bitdust-0.1.6.231/bitdust/main/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      949 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    34314 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/bpmain.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14187 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/bptester.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    20957 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/config.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    12982 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/config_defaults.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    24970 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/config_details.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10719 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/config_types.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1712 2023-01-29 11:48:56.000000 bitdust-0.1.6.231/bitdust/main/default_network.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9443 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/events.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9615 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/help.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    20782 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/initializer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5089 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/install_wizard.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    15084 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/installer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6602 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/listeners.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2368 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/network_config.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    60580 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/settings.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11845 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/main/shutdowner.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.548984 bitdust-0.1.6.231/bitdust/p2p/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      925 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8983 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/commands.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17986 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/handshaker.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    28281 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/id_rotator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    22021 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/lookup.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    23837 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/network_connector.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11849 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/network_service.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    29615 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/online_status.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    27694 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/p2p_connector.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    37669 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/p2p_service.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17410 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/p2p_service_seeker.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4556 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/p2p_stats.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    19004 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/propagate.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8730 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/p2p/ratings.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.548984 bitdust-0.1.6.231/bitdust/raid/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      933 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/raid/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    24733 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/raid/eccmap.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5943 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/raid/make.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    20051 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/raid/raid_worker.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2059 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/raid/raidutils.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8614 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/raid/read.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9178 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/raid/rebuild.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5262 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/raid/worker.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.556984 bitdust-0.1.6.231/bitdust/services/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      884 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    26507 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/driver.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17419 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/local_service.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4424 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_accountant.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1974 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_backup_db.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6595 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_backups.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1486 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_blockchain.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9792 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_broadcasting.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2897 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_contract_chain.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5591 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_customer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2618 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_customer_contracts.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11976 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_customer_family.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2318 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_customer_patrol.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4913 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_customer_support.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1618 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_data_disintegration.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5001 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_data_motion.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9743 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_employer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8193 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_entangled_dht.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2511 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_gateway.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2009 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_http_connections.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4091 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_http_transport.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5346 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_identity_propagate.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1991 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_identity_server.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2390 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_ip_port_responder.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3298 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_keys_registry.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11261 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_keys_storage.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3253 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_list_files.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8420 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_message_broker.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4261 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_message_history.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2127 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_miner.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4100 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_my_data.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2935 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_my_ip_port.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4938 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_network.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2033 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_nodes_lookup.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10155 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_p2p_hookups.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7449 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_p2p_notifications.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3981 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_personal_messages.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4318 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_private_groups.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4827 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_private_messages.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4590 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_proxy_server.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11284 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_proxy_transport.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1577 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_rebuilding.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1565 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_restores.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3397 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_shared_data.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17790 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_supplier.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2452 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_supplier_contracts.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1994 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_tcp_connections.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4431 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_tcp_transport.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2962 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_udp_datagrams.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5040 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/services/service_udp_transport.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.556984 bitdust-0.1.6.231/bitdust/storage/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      958 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    12346 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/accounting.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    21394 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/archive_reader.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    15001 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/archive_writer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    22868 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/backup.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    39792 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/backup_control.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    77837 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/backup_fs.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    75581 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/backup_matrix.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    16663 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/backup_monitor.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    32245 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/backup_rebuilder.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    12919 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/backup_schedule.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8127 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/backup_tar.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    20832 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/index_synchronizer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    16012 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/keys_synchronizer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9592 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/restore_monitor.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    33981 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/restore_worker.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11181 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/storage/tar_file.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.560984 bitdust-0.1.6.231/bitdust/stream/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      882 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stream/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    34695 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stream/broker_negotiator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4688 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stream/data_receiver.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    20254 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stream/data_sender.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11841 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stream/file_down.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    12865 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stream/file_up.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    38717 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stream/io_throttle.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    29553 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stream/message.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    91952 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stream/message_peddler.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    19432 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stream/message_producer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    43379 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stream/p2p_queue.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    35334 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stream/queue_keeper.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.560984 bitdust-0.1.6.231/bitdust/stun/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1223 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stun/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    23168 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stun/stun_client.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6390 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/stun/stun_server.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.560984 bitdust-0.1.6.231/bitdust/supplier/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/supplier/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8236 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/supplier/customer_assistant.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    35366 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/supplier/customer_space.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8818 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/supplier/customers_rejector.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    51966 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/supplier/family_member.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10878 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/supplier/list_files.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6955 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/supplier/local_tester.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.560984 bitdust-0.1.6.231/bitdust/system/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      961 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/system/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    37730 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/system/bpio.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6797 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/system/child_process.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14441 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/system/deploy.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4405 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/system/dirsize.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6550 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/system/diskusage.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6110 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/system/local_fs.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8609 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/system/nonblocking.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11747 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/system/run_upnpc.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11571 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/system/tmpfile.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8526 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/system/tray_icon.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.560984 bitdust-0.1.6.231/bitdust/transport/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1161 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9653 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/bandwidth.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13659 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/callback.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    45667 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/gateway.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.564984 bitdust-0.1.6.231/bitdust/transport/http/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/http/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8974 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/http/http_interface.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14059 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/http/http_node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      842 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/http/sum_client.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      633 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/http/sum_server.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)    12360 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/http/transport_http_old.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2216 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/http/twisted-web-ssl.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10153 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/network_transport.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    21546 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/packet_in.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    55997 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/packet_out.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.564984 bitdust-0.1.6.231/bitdust/transport/proxy/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/proxy/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13162 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/proxy/proxy_interface.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    40557 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/proxy/proxy_receiver.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    68687 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/proxy/proxy_router.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    24428 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/proxy/proxy_sender.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.564984 bitdust-0.1.6.231/bitdust/transport/tcp/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      879 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/tcp/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    18570 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/tcp/tcp_connection.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13313 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/tcp/tcp_interface.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    15160 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/tcp/tcp_node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    22333 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/tcp/tcp_stream.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.568984 bitdust-0.1.6.231/bitdust/transport/udp/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      879 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/udp/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11284 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/udp/udp_connector.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    24562 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/udp/udp_file_queue.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13917 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/udp/udp_interface.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    19322 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/udp/udp_node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    26324 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/udp/udp_session.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    57234 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/transport/udp/udp_stream.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.568984 bitdust-0.1.6.231/bitdust/updates/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      879 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/updates/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    12033 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/updates/git_proc.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.568984 bitdust-0.1.6.231/bitdust/userid/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      877 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/userid/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    15285 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/userid/global_id.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    25972 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/userid/id_registrator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    15375 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/userid/id_restorer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    18020 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/userid/id_server.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    39959 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/userid/id_url.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    39644 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/userid/identity.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4119 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/userid/known_servers.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    22377 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust/userid/my_id.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.528984 bitdust-0.1.6.231/bitdust.egg-info/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9005 2023-01-29 11:48:56.000000 bitdust-0.1.6.231/bitdust.egg-info/PKG-INFO
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14386 2023-01-29 11:48:56.000000 bitdust-0.1.6.231/bitdust.egg-info/SOURCES.txt
--rw-r--r--   0 veselin   (1000) veselin   (1001)        1 2023-01-29 11:48:56.000000 bitdust-0.1.6.231/bitdust.egg-info/dependency_links.txt
--rw-r--r--   0 veselin   (1000) veselin   (1001)      120 2023-01-29 11:48:56.000000 bitdust-0.1.6.231/bitdust.egg-info/requires.txt
--rw-r--r--   0 veselin   (1000) veselin   (1001)       22 2023-01-29 11:48:56.000000 bitdust-0.1.6.231/bitdust.egg-info/top_level.txt
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.568984 bitdust-0.1.6.231/bitdust_forks/
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.576984 bitdust-0.1.6.231/bitdust_forks/Bismuth/
--rw-r--r--   0 veselin   (1000) veselin   (1001)        0 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1699 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/aliases.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1567 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/aliasesv2.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    37606 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/apihandler.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      116 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/application_directories.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      846 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/balance_nogui.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2403 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/check_tx.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1034 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/cmd_addpeers.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      906 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/cmd_hn_last_block_ts.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1086 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/cmd_hn_reg_round.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14518 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/commands.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3421 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/connectionmanager.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4748 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/connections.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    18284 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/dbhandler.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1310 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/demo_getaddresssince.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1426 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/demo_getstatus.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4399 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/difficulty.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    26736 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/digest.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11146 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/essentials.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2255 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/fork.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9427 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/genesis.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      790 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/hmac_drbg.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      715 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/hyperlane.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1114 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/hyperlane_asyncio.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9049 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/ledger_explorer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1764 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/log.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    32179 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/mempool.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2362 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/mining.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7396 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/mining_heavy3.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)   116112 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      561 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/node_stop.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6116 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/optiexplorer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8203 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/optihash.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6014 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/options.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    25033 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/optipoolware.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    24519 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/peershandler.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6820 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/plugins.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      537 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/process_search.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      700 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/quantizer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8159 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/regnet.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      636 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/rewards_reindex.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      446 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/rewards_test.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5812 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/rpcconnections.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2014 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/send_csv.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4611 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/send_nogui_noconf.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5625 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/simplecrypt.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9408 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/staking.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9526 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/tokensv2.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1164 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/wallet_keys.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11108 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/wallet_server.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6998 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/wallet_websocket.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14984 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/Bismuth/worker.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.576984 bitdust-0.1.6.231/bitdust_forks/CodernityDB/
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)      700 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/__init__.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)    42787 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/database.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     1037 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/database_gevent.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     8184 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/database_safe_shared.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3992 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/database_super_thread_safe.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1170 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/database_thread_safe.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7835 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/debug_stuff.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      764 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/env.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)    33960 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/hash_index.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     4814 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/index.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    25578 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/indexcreator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4860 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/lfu_cache.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5547 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/lfu_cache_with_lock.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1370 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/migrate.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1011 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/misc.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     2851 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/patch.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     3756 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/rr_cache.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4115 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/rr_cache_with_lock.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     5125 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/sharded_hash.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     3863 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/sharded_index.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     3806 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/storage.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)   107565 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB/tree_index.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.580984 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      700 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    43644 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/database.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1040 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/database_gevent.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8236 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/database_safe_shared.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3973 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/database_super_thread_safe.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1170 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/database_thread_safe.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7915 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/debug_stuff.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      764 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/env.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    40383 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/hash_index.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4958 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/index.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    25451 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/indexcreator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5435 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/lfu_cache.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6221 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/lfu_cache_with_lock.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1371 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/migrate.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1010 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/misc.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2852 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/patch.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4376 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/rr_cache.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4639 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/rr_cache_with_lock.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6030 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/sharded_hash.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3714 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/sharded_index.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4261 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/storage.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)   111785 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/CodernityDB3/tree_index.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1803 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/__init__.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.580984 bitdust-0.1.6.231/bitdust_forks/entangled/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1474 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    25438 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/dtuple.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.584984 bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2008 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2181 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/constants.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3401 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/contact.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    12393 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/datastore.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8793 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/encoding.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5867 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/kbucket.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6548 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/msgformat.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3471 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/msgtypes.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    89776 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    33799 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/protocol.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    22400 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/routingtable.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13052 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/entangled/node.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.584984 bitdust-0.1.6.231/bitdust_forks/parallelp/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      885 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/parallelp/__init__.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.584984 bitdust-0.1.6.231/bitdust_forks/parallelp/pp/
--rw-r--r--   0 veselin   (1000) veselin   (1001)    36502 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/parallelp/pp/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4764 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/parallelp/pp/ppauto.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11913 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/parallelp/pp/ppserver.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6981 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/parallelp/pp/pptransport.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5046 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/parallelp/pp/ppworker.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.584984 bitdust-0.1.6.231/bitdust_forks/txrestapi/
--rw-r--r--   0 veselin   (1000) veselin   (1001)        2 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/txrestapi/__init__.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.584984 bitdust-0.1.6.231/bitdust_forks/txrestapi/txrestapi/
--rw-r--r--   0 veselin   (1000) veselin   (1001)        2 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/txrestapi/txrestapi/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7447 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/txrestapi/txrestapi/json_resource.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1472 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/txrestapi/txrestapi/methods.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2941 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/txrestapi/txrestapi/resource.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      169 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/txrestapi/txrestapi/service.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9470 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/txrestapi/txrestapi/tests.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.584984 bitdust-0.1.6.231/bitdust_forks/websocket/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1022 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13641 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/_abnf.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13508 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/_app.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1758 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/_cookiejar.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17675 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/_core.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2404 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/_exceptions.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6436 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/_handshake.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10842 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/_http.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2156 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/_logging.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4757 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/_socket.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1797 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/_ssl_compat.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4707 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/_url.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6951 2023-01-27 15:47:05.000000 bitdust-0.1.6.231/bitdust_forks/websocket/_utils.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-01-29 11:48:56.584984 bitdust-0.1.6.231/scripts/
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     1918 2023-01-29 11:48:56.000000 bitdust-0.1.6.231/scripts/bitdust
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     1833 2023-01-29 11:48:56.000000 bitdust-0.1.6.231/scripts/bitdust_worker
--rw-r--r--   0 veselin   (1000) veselin   (1001)       38 2023-01-29 11:48:56.588984 bitdust-0.1.6.231/setup.cfg
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5284 2023-01-29 11:48:56.000000 bitdust-0.1.6.231/setup.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.258923 bitdust-0.1.7.233/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    34520 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/LICENSE.txt
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7712 2023-04-21 14:01:38.258923 bitdust-0.1.7.233/PKG-INFO
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6011 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/README.txt
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.190921 bitdust-0.1.7.233/bitdust/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1803 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/__init__.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.190921 bitdust-0.1.7.233/bitdust/access/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      882 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8145 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/group_access_donor.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    69935 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/group_member.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    27158 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/groups.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    35302 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/key_ring.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    46155 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/shared_access_coordinator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    16003 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/shared_access_donor.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.194921 bitdust-0.1.7.233/bitdust/automats/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/automats/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    28621 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/automats/automat.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4035 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/automats/global_state.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.194921 bitdust-0.1.7.233/bitdust/blockchain/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      882 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/blockchain/__init__.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.194921 bitdust-0.1.7.233/bitdust/broadcast/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/broadcast/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7494 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/broadcast/broadcast_listener.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4803 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/broadcast/broadcast_service.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14662 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/broadcast/broadcaster_node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10000 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/broadcast/broadcasters_finder.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.194921 bitdust-0.1.7.233/bitdust/chat/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      876 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3306 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/kbhit.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    29641 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/message_database.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5675 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/message_keeper.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11276 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/nickname_holder.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11315 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/nickname_observer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10358 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/terminal_chat.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.198921 bitdust-0.1.7.233/bitdust/coins/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      877 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    16133 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/accountant_node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10172 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/accountants_finder.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13995 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/coins_db.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7339 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/coins_index.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6480 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/coins_io.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17260 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/coins_miner.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10287 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/contract_chain_consumer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7023 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/contract_chain_node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10444 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/customer_contract_executor.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6104 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/mine_old.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5311 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/miner_old.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11275 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/supplier_contract_executor.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.198921 bitdust-0.1.7.233/bitdust/contacts/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      884 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/contacts/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    38445 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/contacts/contactsdb.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3829 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/contacts/friends.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    21012 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/contacts/identitycache.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14809 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/contacts/identitydb.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.198921 bitdust-0.1.7.233/bitdust/crypt/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      877 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5835 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/certificate.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4029 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/cipher.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11851 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/encrypted.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3253 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/hashes.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13081 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/key.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    39203 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/my_keys.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2799 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/number.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8811 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/rsa_key.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17628 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/signed.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.198921 bitdust-0.1.7.233/bitdust/currency/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/currency/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7434 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/currency/geth_service.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.198921 bitdust-0.1.7.233/bitdust/customer/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/customer/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    41073 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/customer/fire_hire.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13849 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/customer/list_files_orator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    26487 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/customer/supplier_connector.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13424 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/customer/supplier_finder.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.202921 bitdust-0.1.7.233/bitdust/dht/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      954 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/dht/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10289 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/dht/dht_records.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14437 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/dht/dht_relations.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    62442 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/dht/dht_service.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4098 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/dht/known_nodes.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.202921 bitdust-0.1.7.233/bitdust/interface/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)   238439 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/api.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    53720 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/api_rest_http_server.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11461 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/api_web_socket.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    57996 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/cmd_line_json.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7069 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/cmd_line_json_templates.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    22207 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/ftp_server.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.202921 bitdust-0.1.7.233/bitdust/lib/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      969 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7701 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/diskspace.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2799 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/getsizeof.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10243 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/jsn.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    40342 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/jsontemplate.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11193 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/maths.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    31961 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/misc.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8488 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/nameurl.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    31041 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/net_misc.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    16067 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/packetid.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    15989 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/schedule.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3508 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/serialization.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2760 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/strng.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    23049 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/txws.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10343 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/udp.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2382 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/utime.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13150 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/websock.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.206921 bitdust-0.1.7.233/bitdust/logs/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/logs/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    25640 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/logs/lg.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3211 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/logs/measure_it.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1890 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/logs/memdebug.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8227 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/logs/weblog.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10403 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/logs/webtraffic.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.206921 bitdust-0.1.7.233/bitdust/main/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      949 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    34709 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/bpmain.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14262 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/bptester.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    20957 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/config.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    12982 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/config_defaults.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    24970 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/config_details.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10719 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/config_types.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1712 2023-04-21 14:01:37.000000 bitdust-0.1.7.233/bitdust/main/default_network.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9443 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/events.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9615 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/help.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    20827 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/initializer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5089 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/install_wizard.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    15084 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/installer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6602 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/listeners.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2368 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/network_config.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    60704 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/settings.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11845 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/shutdowner.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.210922 bitdust-0.1.7.233/bitdust/p2p/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      925 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8983 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/commands.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17986 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/handshaker.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    28281 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/id_rotator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    22021 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/lookup.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    23837 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/network_connector.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11849 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/network_service.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    29615 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/online_status.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    27694 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/p2p_connector.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    37669 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/p2p_service.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17410 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/p2p_service_seeker.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4556 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/p2p_stats.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    19004 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/propagate.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8730 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/ratings.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.210922 bitdust-0.1.7.233/bitdust/raid/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      933 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    24733 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/eccmap.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5943 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/make.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    20051 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/raid_worker.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2059 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/raidutils.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8614 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/read.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9178 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/rebuild.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5395 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/worker.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.218922 bitdust-0.1.7.233/bitdust/services/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      884 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    26507 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/driver.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17419 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/local_service.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4424 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_accountant.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1974 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_backup_db.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6595 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_backups.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1486 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_blockchain.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9792 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_broadcasting.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2897 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_contract_chain.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5591 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_customer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2618 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_customer_contracts.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11976 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_customer_family.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2318 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_customer_patrol.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4913 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_customer_support.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1618 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_data_disintegration.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5001 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_data_motion.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9743 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_employer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8193 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_entangled_dht.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2511 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_gateway.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2009 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_http_connections.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4091 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_http_transport.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5346 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_identity_propagate.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1991 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_identity_server.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2390 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_ip_port_responder.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3298 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_keys_registry.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11261 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_keys_storage.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3253 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_list_files.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8420 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_message_broker.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4261 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_message_history.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2127 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_miner.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4100 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_my_data.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2935 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_my_ip_port.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4938 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_network.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2033 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_nodes_lookup.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10155 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_p2p_hookups.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7449 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_p2p_notifications.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3981 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_personal_messages.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4318 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_private_groups.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4827 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_private_messages.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4590 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_proxy_server.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11284 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_proxy_transport.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1577 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_rebuilding.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1565 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_restores.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3397 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_shared_data.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17790 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_supplier.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2452 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_supplier_contracts.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1994 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_tcp_connections.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4431 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_tcp_transport.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2962 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_udp_datagrams.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5040 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_udp_transport.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.222922 bitdust-0.1.7.233/bitdust/storage/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      958 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    12346 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/accounting.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    21358 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/archive_reader.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14921 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/archive_writer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    22859 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    39695 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_control.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    77837 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_fs.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    75581 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_matrix.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    16663 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_monitor.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    32245 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_rebuilder.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    12919 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_schedule.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8285 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_tar.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    20832 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/index_synchronizer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    16189 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/keys_synchronizer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9662 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/restore_monitor.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    33963 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/restore_worker.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11658 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/tar_file.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.222922 bitdust-0.1.7.233/bitdust/stream/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      882 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    34695 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/broker_negotiator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4688 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/data_receiver.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    20254 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/data_sender.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11841 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/file_down.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    12865 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/file_up.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    38717 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/io_throttle.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    29553 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/message.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    91952 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/message_peddler.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    19432 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/message_producer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    43379 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/p2p_queue.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    35334 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/queue_keeper.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.222922 bitdust-0.1.7.233/bitdust/stun/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1223 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stun/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    23168 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stun/stun_client.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6390 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stun/stun_server.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.226922 bitdust-0.1.7.233/bitdust/supplier/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8236 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/customer_assistant.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    35366 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/customer_space.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8938 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/customers_rejector.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    51966 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/family_member.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10878 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/list_files.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6955 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/local_tester.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.226922 bitdust-0.1.7.233/bitdust/system/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      961 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    37906 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/bpio.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6797 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/child_process.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14220 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/deploy.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4405 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/dirsize.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6550 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/diskusage.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6110 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/local_fs.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8609 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/nonblocking.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11747 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/run_upnpc.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11571 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/tmpfile.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8526 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/tray_icon.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.226922 bitdust-0.1.7.233/bitdust/transport/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1161 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9653 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/bandwidth.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13659 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/callback.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    45667 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/gateway.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.230922 bitdust-0.1.7.233/bitdust/transport/http/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8974 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/http_interface.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14059 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/http_node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      842 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/sum_client.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      633 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/sum_server.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)    12360 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/transport_http_old.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2216 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/twisted-web-ssl.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10153 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/network_transport.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    21546 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/packet_in.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    55997 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/packet_out.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.230922 bitdust-0.1.7.233/bitdust/transport/proxy/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/proxy/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13162 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/proxy/proxy_interface.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    40557 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/proxy/proxy_receiver.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    68687 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/proxy/proxy_router.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    24428 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/proxy/proxy_sender.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.230922 bitdust-0.1.7.233/bitdust/transport/tcp/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      879 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/tcp/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    18570 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/tcp/tcp_connection.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13313 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/tcp/tcp_interface.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    15160 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/tcp/tcp_node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    22333 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/tcp/tcp_stream.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.230922 bitdust-0.1.7.233/bitdust/transport/udp/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      879 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11284 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/udp_connector.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    24562 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/udp_file_queue.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13917 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/udp_interface.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    19322 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/udp_node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    26324 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/udp_session.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    57234 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/udp_stream.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.230922 bitdust-0.1.7.233/bitdust/updates/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      879 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/updates/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    12033 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/updates/git_proc.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.234922 bitdust-0.1.7.233/bitdust/userid/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      877 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    15285 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/global_id.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    25972 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/id_registrator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    15375 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/id_restorer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    18020 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/id_server.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    39959 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/id_url.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    39644 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/identity.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4119 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/known_servers.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    22377 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/my_id.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.190921 bitdust-0.1.7.233/bitdust.egg-info/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7712 2023-04-21 14:01:38.000000 bitdust-0.1.7.233/bitdust.egg-info/PKG-INFO
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14699 2023-04-21 14:01:38.000000 bitdust-0.1.7.233/bitdust.egg-info/SOURCES.txt
+-rw-r--r--   0 veselin   (1000) veselin   (1001)        1 2023-04-21 14:01:38.000000 bitdust-0.1.7.233/bitdust.egg-info/dependency_links.txt
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      120 2023-04-21 14:01:38.000000 bitdust-0.1.7.233/bitdust.egg-info/requires.txt
+-rw-r--r--   0 veselin   (1000) veselin   (1001)       22 2023-04-21 14:01:38.000000 bitdust-0.1.7.233/bitdust.egg-info/top_level.txt
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.234922 bitdust-0.1.7.233/bitdust_forks/
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.242922 bitdust-0.1.7.233/bitdust_forks/Bismuth/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)        0 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1699 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/aliases.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1567 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/aliasesv2.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    37606 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/apihandler.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      116 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/application_directories.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      846 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/balance_nogui.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2403 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/check_tx.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1034 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/cmd_addpeers.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      906 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/cmd_hn_last_block_ts.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1086 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/cmd_hn_reg_round.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14518 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/commands.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3421 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/connectionmanager.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4748 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/connections.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    18284 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/dbhandler.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1310 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/demo_getaddresssince.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1426 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/demo_getstatus.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4399 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/difficulty.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    26736 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/digest.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11146 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/essentials.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2255 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/fork.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9427 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/genesis.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      790 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/hmac_drbg.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      715 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/hyperlane.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1114 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/hyperlane_asyncio.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9049 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/ledger_explorer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1764 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/log.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    32179 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/mempool.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2362 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/mining.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7396 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/mining_heavy3.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)   116112 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      561 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/node_stop.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6116 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/optiexplorer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8203 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/optihash.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6014 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/options.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    25033 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/optipoolware.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    24519 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/peershandler.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6820 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/plugins.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      537 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/process_search.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      700 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/quantizer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8159 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/regnet.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      636 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/rewards_reindex.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      446 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/rewards_test.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5812 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/rpcconnections.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2014 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/send_csv.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4611 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/send_nogui_noconf.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5625 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/simplecrypt.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9408 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/staking.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9526 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/tokensv2.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1164 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/wallet_keys.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11108 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/wallet_server.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6998 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/wallet_websocket.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14984 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/worker.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.246923 bitdust-0.1.7.233/bitdust_forks/CodernityDB/
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)      700 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/__init__.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)    42787 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/database.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     1037 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_gevent.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     8184 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_safe_shared.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3992 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_super_thread_safe.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1170 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_thread_safe.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7835 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/debug_stuff.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      764 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/env.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)    33960 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/hash_index.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     4814 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/index.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    25578 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/indexcreator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4860 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/lfu_cache.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5547 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/lfu_cache_with_lock.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1370 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/migrate.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1011 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/misc.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     2851 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/patch.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     3756 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/rr_cache.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4115 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/rr_cache_with_lock.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     5125 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/sharded_hash.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     3863 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/sharded_index.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     3806 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/storage.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)   107565 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/tree_index.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.246923 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      700 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    43644 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1040 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_gevent.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8236 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_safe_shared.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3973 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_super_thread_safe.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1170 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_thread_safe.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7915 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/debug_stuff.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      764 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/env.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    40383 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/hash_index.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4958 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/index.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    25451 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/indexcreator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5435 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/lfu_cache.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6221 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/lfu_cache_with_lock.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1371 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/migrate.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1010 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/misc.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2852 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/patch.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4376 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/rr_cache.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4639 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/rr_cache_with_lock.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6030 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/sharded_hash.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3714 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/sharded_index.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4261 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/storage.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)   111785 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/tree_index.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1803 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/__init__.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.250923 bitdust-0.1.7.233/bitdust_forks/entangled/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1474 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    25438 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/dtuple.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.250923 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2008 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2181 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/constants.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3401 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/contact.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    12393 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/datastore.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8793 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/encoding.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5867 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/kbucket.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6548 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/msgformat.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3471 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/msgtypes.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    89776 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    33799 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/protocol.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    22400 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/routingtable.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13052 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/node.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.250923 bitdust-0.1.7.233/bitdust_forks/parallelp/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      885 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/parallelp/__init__.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.250923 bitdust-0.1.7.233/bitdust_forks/parallelp/pp/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    36502 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/parallelp/pp/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4764 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/parallelp/pp/ppauto.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11913 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/parallelp/pp/ppserver.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6981 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/parallelp/pp/pptransport.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5046 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/parallelp/pp/ppworker.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.250923 bitdust-0.1.7.233/bitdust_forks/txrestapi/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)        2 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/__init__.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.254923 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)        2 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7447 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/json_resource.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1472 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/methods.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2941 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/resource.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      169 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/service.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9470 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/tests.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.254923 bitdust-0.1.7.233/bitdust_forks/websocket/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1022 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13641 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_abnf.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13508 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_app.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1758 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_cookiejar.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17675 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_core.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2404 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_exceptions.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6436 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_handshake.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10842 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_http.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2156 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_logging.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4757 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_socket.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1797 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_ssl_compat.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4707 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_url.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6951 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_utils.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.254923 bitdust-0.1.7.233/scripts/
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     1918 2023-04-21 14:01:37.000000 bitdust-0.1.7.233/scripts/bitdust
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     1833 2023-04-21 14:01:37.000000 bitdust-0.1.7.233/scripts/bitdust_worker
+-rw-r--r--   0 veselin   (1000) veselin   (1001)       38 2023-04-21 14:01:38.258923 bitdust-0.1.7.233/setup.cfg
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5284 2023-04-21 14:01:37.000000 bitdust-0.1.7.233/setup.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.254923 bitdust-0.1.7.233/tests/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7089 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_backup_fs.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7938 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_backup_restore.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4064 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_codernity_db.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8271 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_crypt_signed.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    35543 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_id_url.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4942 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_identity.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7730 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_my_keys.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3024 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_raid_make_read.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3560 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_raid_manager.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13735 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_raid_worker.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2299 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_rsa_key.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6347 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_serialize.py
```

### Comparing `bitdust-0.1.6.231/PKG-INFO` & `bitdust-0.1.7.233/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,182 +1,19 @@
 Metadata-Version: 2.1
 Name: bitdust
-Version: 0.1.6.231
+Version: 0.1.7.233
 Summary: p2p secure distributed storage and communication engine
 Home-page: https://bitdust.io
+Download-URL: https://bitdust.io
 Author: Veselin Penev, BitDust
 Author-email: bitdust.io@gmail.com
 Maintainer: Veselin Penev, BitDust
 Maintainer-email: veselin@bitdust.io
 License: Copyright (C) 2008 Veselin Penev, https://bitdust.io
-Download-URL: https://bitdust.io
-Description: BitDust
-        =======
-        
-        BitDust is a peer to peer online backup utility.
-        
-        This is a distributed network for backup data storage. Each participant of the network provides a portion of his hard drive for other users. In exchange, he is able to store his data on other peers.
-        
-        The redundancy in backup makes it so if someone loses your data, you can rebuild what was lost and give it to someone else to hold. And all of this happens without you having to do a thing - the software keeps your data in safe.
-        
-        All your data is encrypted before it leaves your computer with a private key your computer generates. No one else can read your data, even BitDust Team! Recover data is only one way - download the necessary pieces from computers of other peers and decrypt them with your private key.
-        
-        BitDust is written in Python using pure Twisted framework and published under GNU AGPLv3.
-        
-        https://bitdust.io
-        
-        
-        
-        Current status
-        ==============
-        
-        Current project stage is about to only research opportunities of
-        building a holistic eco-system that protects your privacy in the network
-        by establishing p2p communications of users and maximize distribution of
-        information flows in the network.
-        
-        At the moment exists a very limited alpha version of the BitDust software.
-        We decided to publish those earlier works to verify/test/share our ideas and experiments with other people.
-        
-        
-        
-        Install BitDust software
-        ========================
-        
-        
-        1. Install software dependencies
-        
-        Seems like in Ubuntu (probably most other distros) you can install all dependencies in that way:
-        
-                sudo apt-get install git gcc python3-dev python3-virtualenv
-        
-        
-        Optionally, you can also install [miniupnpc](http://miniupnp.tuxfamily.org/) tool if you want BitDust automatically deal with UPnPc configuration of your network router so it can also accept incomming connections from other nodes.:
-        
-                sudo apt-get install miniupnpc
-        
-        
-        On MacOSX platform you can install requirements in that way:
-        
-                brew install git python3
-        
-        And use pip to get all required packages:
-        
-                pip install --upgrade --user
-                pip install --upgrade pip --user
-                pip install virtualenv --user
-        
-        
-        2. Get BitDust to your local machine
-        
-        Second step is to get the BitDust sources. To have a full control over BitDust process running on your local machine you better make a fork of the Public BitDist repository on GitHub at https://github.com/bitdust-io/public and clone it on your local machine:
-        
-                git clone https://github.com/<your GitHub username>/<name of BitDust fork>.git bitdust
-        
-        
-        The software will periodically run `git fetch` and `git rebase` to check for recent commits in the repo. This way we make sure that everyone is running the latest version of the program. Once you made a fork, you will have to update your Fork manually and pull commits from Public BitDust repository if you trust them.
-        
-        However if you just trust BitDust contributors you can simply clone the Public repository directly and software will be up to date with the "official" public code base:
-        
-                git clone https://github.com/bitdust-io/public.git bitdust
-        
-        
-        3. Building virtual environment
-        
-        Then you need to build virtual environment with all required Python dependencies, BitDust software will run fully isolated.
-        
-        Single command should make it for you, all required files will be generated in `~/.bitdust/venv/` sub-folder:
-        
-                cd bitdust
-                python3 bitdust.py install
-        
-        
-        Last step to make BitDust software ready is to make a short alias in your OS, then you can just type `bitdust` in command line to fast access the program:
-        
-                sudo ln -s -f /home/<user>/.bitdust/bitdust /usr/local/bin/bitdust
-        
-        
-        4. Run BitDust
-        
-        Start using the software by creating an identity for your device in BitDust network:
-        
-                bitdust id create <some nick name>
-        
-        
-        I recommend you to create another copy of your Private Key in a safe place to be able to recover your data in the future. You can do it with such command:
-        
-                bitdust key copy <nickname>.bitdust.key
-        
-        
-        Your settings and local files are located in that folder: ~/.bitdust
-        
-        Type this command to read more info about BitDust commands:
-        
-                bitdust help
-        
-        
-        To run the software type:
-        
-                bitdust
-        
-        
-        Start as background process:
-        
-                bitdust detach
-        
-        
-        To get some more insights or just to know how to start playing with software
-        you can visit [BitDust Commands](https://bitdust.io/commands.html) page.
-        
-        To get more info about API methods available go to [BitDust API](https://bitdust.io/api.html) page.
-        
-        
-        5. Binary Dependencies
-        
-        If you are installing BitDust on Windows platforms, you may require some binary packages already compiled and packaged for Microsoft Windows platforms, you can check following locations and download needed binaries and libraries:
-        
-        * cygwin: [cygwin.com](https://cygwin.com/install.html)
-        * git: [git-scm.com](https://git-scm.com/download/win)
-        * python2.7 or python3: [python.org](http://python.org/download/releases)
-        * twisted: [twistedmatrix.com](http://twistedmatrix.com)
-        * pyasn1: [pyasn1.sourceforge.net](http://pyasn1.sourceforge.net)
-        * miniupnpc: [miniupnp.tuxfamily.org](http://miniupnp.tuxfamily.org/)
-        
-        
-        
-        Docker Hub container image
-        ==========================
-        
-        You can also run bitdust inside Docker. We prepared a container which have BitDust installed and easy to run. You will have to SSH into the running container after start it and manually configure bitdust as you wish and run it:
-        
-                docker run -d -P --name bdnode bitdust/app1
-                docker port bdnode 22
-                0.0.0.0:32771  <-  learn which SSH port was opened on your host
-        
-        
-        Now you can ssh to the container, password is `bitdust`:
-        
-                ssh root@localhost -p 32771
-                password: bitdust
-        
-        
-        Inside the container you will have BitDust installed and ready to use, so you can run it directly:
-        
-                root@1ef6a46c3042:~# bitdust
-        
-        
-        
-        Feedback
-        ========
-        
-        You can contact [BitDust contributors](https://github.com/bitdust-io) on GitHub if you have any questions or ideas.
-        Welcome to the future!
-        
 Keywords: p2p,peer to peer,backup,restore,storage,data,recover,distributed,online,python,twisted,messaging,websocket,encryption,crypto,protection
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Twisted
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -194,7 +31,170 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+BitDust
+=======
+
+BitDust is a peer to peer online backup utility.
+
+This is a distributed network for backup data storage. Each participant of the network provides a portion of his hard drive for other users. In exchange, he is able to store his data on other peers.
+
+The redundancy in backup makes it so if someone loses your data, you can rebuild what was lost and give it to someone else to hold. And all of this happens without you having to do a thing - the software keeps your data in safe.
+
+All your data is encrypted before it leaves your computer with a private key your computer generates. No one else can read your data, even BitDust Team! Recover data is only one way - download the necessary pieces from computers of other peers and decrypt them with your private key.
+
+BitDust is written in Python using pure Twisted framework and published under GNU AGPLv3.
+
+https://bitdust.io
+
+
+
+Current status
+==============
+
+Current project stage is about to only research opportunities of
+building a holistic eco-system that protects your privacy in the network
+by establishing p2p communications of users and maximize distribution of
+information flows in the network.
+
+At the moment exists a very limited alpha version of the BitDust software.
+We decided to publish those earlier works to verify/test/share our ideas and experiments with other people.
+
+
+
+Install BitDust software
+========================
+
+
+1. Install software dependencies
+
+Seems like in Ubuntu (probably most other distros) you can install all dependencies in that way:
+
+        sudo apt-get install git gcc python3-dev python3-virtualenv
+
+
+Optionally, you can also install [miniupnpc](http://miniupnp.tuxfamily.org/) tool if you want BitDust automatically deal with UPnPc configuration of your network router so it can also accept incomming connections from other nodes.:
+
+        sudo apt-get install miniupnpc
+
+
+On MacOSX platform you can install requirements in that way:
+
+        brew install git python3
+
+And use pip to get all required packages:
+
+        pip install --upgrade --user
+        pip install --upgrade pip --user
+        pip install virtualenv --user
+
+
+2. Get BitDust to your local machine
+
+Second step is to get the BitDust sources. To have a full control over BitDust process running on your local machine you better make a fork of the Public BitDist repository on GitHub at https://github.com/bitdust-io/public and clone it on your local machine:
+
+        git clone https://github.com/<your GitHub username>/<name of BitDust fork>.git bitdust
+
+
+The software will periodically run `git fetch` and `git rebase` to check for recent commits in the repo. This way we make sure that everyone is running the latest version of the program. Once you made a fork, you will have to update your Fork manually and pull commits from Public BitDust repository if you trust them.
+
+However if you just trust BitDust contributors you can simply clone the Public repository directly and software will be up to date with the "official" public code base:
+
+        git clone https://github.com/bitdust-io/public.git bitdust
+
+
+3. Building virtual environment
+
+Then you need to build virtual environment with all required Python dependencies, BitDust software will run fully isolated.
+
+Single command should make it for you, all required files will be generated in `~/.bitdust/venv/` sub-folder:
+
+        cd bitdust
+        python3 bitdust.py install
+
+
+Last step to make BitDust software ready is to make a short alias in your OS, then you can just type `bitdust` in command line to fast access the program:
+
+        sudo ln -s -f /home/<user>/.bitdust/bitdust /usr/local/bin/bitdust
+
+
+4. Run BitDust
+
+Start using the software by creating an identity for your device in BitDust network:
+
+        bitdust id create <some nick name>
+
+
+I recommend you to create another copy of your Private Key in a safe place to be able to recover your data in the future. You can do it with such command:
+
+        bitdust key copy <nickname>.bitdust.key
+
+
+Your settings and local files are located in that folder: ~/.bitdust
+
+Type this command to read more info about BitDust commands:
+
+        bitdust help
+
+
+To run the software type:
+
+        bitdust
+
+
+Start as background process:
+
+        bitdust detach
+
+
+To get some more insights or just to know how to start playing with software
+you can visit [BitDust Commands](https://bitdust.io/commands.html) page.
+
+To get more info about API methods available go to [BitDust API](https://bitdust.io/api.html) page.
+
+
+5. Binary Dependencies
+
+If you are installing BitDust on Windows platforms, you may require some binary packages already compiled and packaged for Microsoft Windows platforms, you can check following locations and download needed binaries and libraries:
+
+* cygwin: [cygwin.com](https://cygwin.com/install.html)
+* git: [git-scm.com](https://git-scm.com/download/win)
+* python2.7 or python3: [python.org](http://python.org/download/releases)
+* twisted: [twistedmatrix.com](http://twistedmatrix.com)
+* pyasn1: [pyasn1.sourceforge.net](http://pyasn1.sourceforge.net)
+* miniupnpc: [miniupnp.tuxfamily.org](http://miniupnp.tuxfamily.org/)
+
+
+
+Docker Hub container image
+==========================
+
+You can also run bitdust inside Docker. We prepared a container which have BitDust installed and easy to run. You will have to SSH into the running container after start it and manually configure bitdust as you wish and run it:
+
+        docker run -d -P --name bdnode bitdust/app1
+        docker port bdnode 22
+        0.0.0.0:32771  <-  learn which SSH port was opened on your host
+
+
+Now you can ssh to the container, password is `bitdust`:
+
+        ssh root@localhost -p 32771
+        password: bitdust
+
+
+Inside the container you will have BitDust installed and ready to use, so you can run it directly:
+
+        root@1ef6a46c3042:~# bitdust
+
+
+
+Feedback
+========
+
+You can contact [BitDust contributors](https://github.com/bitdust-io) on GitHub if you have any questions or ideas.
+Welcome to the future!
```

### Comparing `bitdust-0.1.6.231/README.txt` & `bitdust-0.1.7.233/README.txt`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/__init__.py` & `bitdust-0.1.7.233/bitdust/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/access/__init__.py` & `bitdust-0.1.7.233/bitdust/access/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/access/group_access_donor.py` & `bitdust-0.1.7.233/bitdust/access/group_access_donor.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/access/group_member.py` & `bitdust-0.1.7.233/bitdust/access/group_member.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/access/groups.py` & `bitdust-0.1.7.233/bitdust/access/groups.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/access/key_ring.py` & `bitdust-0.1.7.233/bitdust/access/key_ring.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/access/shared_access_coordinator.py` & `bitdust-0.1.7.233/bitdust/access/shared_access_coordinator.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,21 +304,31 @@
         return
     active_share = get_active_share(evt.data['key_id'])
     if _Debug:
         lg.args(_DebugLevel, e=evt, active_share=active_share)
     if active_share:
         active_share.automat('new-private-key-registered')
         return
-    new_share = SharedAccessCoordinator(
-        evt.data['key_id'],
-        log_events=True,
-        publish_events=False,
-    )
-    new_share.add_connected_callback('key_registered' + strng.to_text(time.time()), lambda _id, _result: on_share_first_connected(evt.data['key_id'], _id, _result))
-    new_share.automat('new-private-key-registered')
+
+    def _run_coordinator():
+        new_share = SharedAccessCoordinator(
+            key_id=evt.data['key_id'],
+            log_events=True,
+            publish_events=False,
+        )
+        new_share.add_connected_callback('key_registered' + strng.to_text(time.time()), lambda _id, _result: on_share_first_connected(evt.data['key_id'], _id, _result))
+        new_share.automat('new-private-key-registered')
+
+    glob_id = global_id.NormalizeGlobalID(evt.data['key_id'])
+    if id_url.is_cached(glob_id['idurl']):
+        _run_coordinator()
+    else:
+        d = identitycache.immediatelyCaching(glob_id['idurl'])
+        d.addErrback(lg.errback, debug=_Debug, debug_level=_DebugLevel, method='shared_access_coordinator.on_key_registered')
+        d.addCallback(lambda *args: _run_coordinator())
 
 
 def on_key_erased(evt):
     if not evt.data['key_id'].startswith('share_'):
         return
     from bitdust.access import shared_access_coordinator
     active_share = shared_access_coordinator.get_active_share(evt.data['key_id'])
```

### Comparing `bitdust-0.1.6.231/bitdust/access/shared_access_donor.py` & `bitdust-0.1.7.233/bitdust/access/shared_access_donor.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/automats/__init__.py` & `bitdust-0.1.7.233/bitdust/automats/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/automats/automat.py` & `bitdust-0.1.7.233/bitdust/automats/automat.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/automats/global_state.py` & `bitdust-0.1.7.233/bitdust/automats/global_state.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/blockchain/__init__.py` & `bitdust-0.1.7.233/bitdust/blockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/broadcast/__init__.py` & `bitdust-0.1.7.233/bitdust/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/broadcast/broadcast_listener.py` & `bitdust-0.1.7.233/bitdust/broadcast/broadcast_listener.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/broadcast/broadcast_service.py` & `bitdust-0.1.7.233/bitdust/broadcast/broadcast_service.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/broadcast/broadcaster_node.py` & `bitdust-0.1.7.233/bitdust/broadcast/broadcaster_node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/broadcast/broadcasters_finder.py` & `bitdust-0.1.7.233/bitdust/broadcast/broadcasters_finder.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/chat/__init__.py` & `bitdust-0.1.7.233/bitdust/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/chat/kbhit.py` & `bitdust-0.1.7.233/bitdust/chat/kbhit.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/chat/message_database.py` & `bitdust-0.1.7.233/bitdust/chat/message_database.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/chat/message_keeper.py` & `bitdust-0.1.7.233/bitdust/chat/message_keeper.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/chat/nickname_holder.py` & `bitdust-0.1.7.233/bitdust/chat/nickname_holder.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/chat/nickname_observer.py` & `bitdust-0.1.7.233/bitdust/chat/nickname_observer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/chat/terminal_chat.py` & `bitdust-0.1.7.233/bitdust/chat/terminal_chat.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/__init__.py` & `bitdust-0.1.7.233/bitdust/coins/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/accountant_node.py` & `bitdust-0.1.7.233/bitdust/coins/accountant_node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/accountants_finder.py` & `bitdust-0.1.7.233/bitdust/coins/accountants_finder.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/coins_db.py` & `bitdust-0.1.7.233/bitdust/coins/coins_db.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/coins_index.py` & `bitdust-0.1.7.233/bitdust/coins/coins_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/coins_io.py` & `bitdust-0.1.7.233/bitdust/coins/coins_io.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/coins_miner.py` & `bitdust-0.1.7.233/bitdust/coins/coins_miner.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/contract_chain_consumer.py` & `bitdust-0.1.7.233/bitdust/coins/contract_chain_consumer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/contract_chain_node.py` & `bitdust-0.1.7.233/bitdust/coins/contract_chain_node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/customer_contract_executor.py` & `bitdust-0.1.7.233/bitdust/coins/customer_contract_executor.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/mine_old.py` & `bitdust-0.1.7.233/bitdust/coins/mine_old.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/miner_old.py` & `bitdust-0.1.7.233/bitdust/coins/miner_old.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/coins/supplier_contract_executor.py` & `bitdust-0.1.7.233/bitdust/coins/supplier_contract_executor.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/contacts/__init__.py` & `bitdust-0.1.7.233/bitdust/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/contacts/contactsdb.py` & `bitdust-0.1.7.233/bitdust/contacts/contactsdb.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/contacts/friends.py` & `bitdust-0.1.7.233/bitdust/contacts/friends.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/contacts/identitycache.py` & `bitdust-0.1.7.233/bitdust/contacts/identitycache.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/contacts/identitydb.py` & `bitdust-0.1.7.233/bitdust/contacts/identitydb.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/crypt/__init__.py` & `bitdust-0.1.7.233/bitdust/crypt/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/crypt/certificate.py` & `bitdust-0.1.7.233/bitdust/crypt/certificate.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/crypt/cipher.py` & `bitdust-0.1.7.233/bitdust/crypt/cipher.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/crypt/encrypted.py` & `bitdust-0.1.7.233/bitdust/crypt/encrypted.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/crypt/hashes.py` & `bitdust-0.1.7.233/bitdust/crypt/hashes.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/crypt/key.py` & `bitdust-0.1.7.233/bitdust/crypt/key.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/crypt/my_keys.py` & `bitdust-0.1.7.233/bitdust/crypt/my_keys.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/crypt/number.py` & `bitdust-0.1.7.233/bitdust/crypt/number.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/crypt/rsa_key.py` & `bitdust-0.1.7.233/bitdust/crypt/rsa_key.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/crypt/signed.py` & `bitdust-0.1.7.233/bitdust/crypt/signed.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/currency/__init__.py` & `bitdust-0.1.7.233/bitdust/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/currency/geth_service.py` & `bitdust-0.1.7.233/bitdust/currency/geth_service.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/customer/__init__.py` & `bitdust-0.1.7.233/bitdust/customer/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/customer/fire_hire.py` & `bitdust-0.1.7.233/bitdust/customer/fire_hire.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/customer/list_files_orator.py` & `bitdust-0.1.7.233/bitdust/customer/list_files_orator.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/customer/supplier_connector.py` & `bitdust-0.1.7.233/bitdust/customer/supplier_connector.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/customer/supplier_finder.py` & `bitdust-0.1.7.233/bitdust/customer/supplier_finder.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/dht/__init__.py` & `bitdust-0.1.7.233/bitdust/dht/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/dht/dht_records.py` & `bitdust-0.1.7.233/bitdust/dht/dht_records.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/dht/dht_relations.py` & `bitdust-0.1.7.233/bitdust/dht/dht_relations.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/dht/dht_service.py` & `bitdust-0.1.7.233/bitdust/dht/dht_service.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/dht/known_nodes.py` & `bitdust-0.1.7.233/bitdust/dht/known_nodes.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/interface/__init__.py` & `bitdust-0.1.7.233/bitdust/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/interface/api.py` & `bitdust-0.1.7.233/bitdust/interface/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1730,14 +1730,15 @@
         curl -X GET 'localhost:8180/file/list/v1?remote_path=abcd1234$alice@server-a.com:pictures/cats/'
 
     ###### WebSocket
         websocket.send('{"command": "api_call", "method": "files_list", "kwargs": {"remote_path": "abcd1234$alice@server-a.com:pictures/cats/"} }');
     """
     if not driver.is_on('service_backup_db'):
         return ERROR('service_backup_db() is not started')
+    from bitdust.main import settings
     from bitdust.storage import backup_fs
     from bitdust.storage import backup_control
     from bitdust.system import bpio
     from bitdust.lib import misc
     from bitdust.userid import global_id
     from bitdust.crypt import my_keys
     result = []
@@ -1793,14 +1794,15 @@
                 iterID=backup_fs.fsID(customer_idurl, key_alias),
                 backup_info_callback=backup_info_callback,
             )
     if not isinstance(lookup, list):
         return ERROR(lookup)
     if _Debug:
         lg.out(_DebugLevel, '    lookup with %d items' % len(lookup))
+    local_dir = settings.getRestoreDir()
     for i in lookup:
         if i['path_id'] == 'index':
             continue
         if key_id is not None and key_id != i['item']['k']:
             continue
         if key_id is None and norm_path['key_alias'] and i['item']['k']:
             if i['item']['k'] != my_keys.make_key_id(alias=norm_path['key_alias'], creator_glob_id=norm_path['customer']):
@@ -1841,14 +1843,15 @@
             'childs': i['childs'],
             'versions': i['versions'],
             'uploads': {
                 'running': [],
                 'pending': [],
             },
             'downloads': [],
+            'local_path': os.path.join(local_dir, i['name']),
         }
         if include_uploads:
             backup_control.tasks()
             running = []
             for backupID in backup_control.FindRunningBackup(pathID=full_glob_id):
                 j = backup_control.jobs().get(backupID)
                 if j:
@@ -1980,14 +1983,15 @@
     ###### WebSocket
         websocket.send('{"command": "api_call", "method": "file_info", "kwargs": {"remote_path": "abcd1234$alice@server-a.com:pictures/dogs/bobby.jpeg"} }');
     """
     if not driver.is_on('service_backup_db'):
         return ERROR('service_backup_db() is not started')
     if _Debug:
         lg.out(_DebugLevel, 'api.file_info remote_path=%s include_uploads=%s include_downloads=%s' % (remote_path, include_uploads, include_downloads))
+    from bitdust.main import settings
     from bitdust.storage import backup_fs
     from bitdust.storage import backup_control
     from bitdust.lib import misc
     from bitdust.system import bpio
     from bitdust.userid import global_id
     norm_path = global_id.NormalizeGlobalID(remote_path)
     remotePath = bpio.remotePath(norm_path['path'])
@@ -2030,14 +2034,15 @@
         'key_id': item.key_id,
         'versions': versions,
         'uploads': {
             'running': [],
             'pending': [],
         },
         'downloads': [],
+        'local_path': os.path.join(settings.getRestoreDir(), item.name()),
     }
     if include_uploads:
         backup_control.tasks()
         running = []
         for backupID in backup_control.FindRunningBackup(pathID=pathID):
             j = backup_control.jobs().get(backupID)
             if j:
@@ -2911,19 +2916,22 @@
     """
     if not driver.is_on('service_shared_data'):
         return ERROR('service_shared_data() is not started')
     from bitdust.access import shared_access_coordinator
     from bitdust.storage import backup_fs
     from bitdust.crypt import my_keys
     from bitdust.userid import global_id
+    from bitdust.userid import id_url
     from bitdust.userid import my_id
     results = []
     if only_active:
         for key_id in shared_access_coordinator.list_active_shares():
             _glob_id = global_id.ParseGlobalID(key_id)
+            if not id_url.is_cached(_glob_id['idurl']):
+                continue
             to_be_listed = False
             if include_mine and _glob_id['idurl'] == my_id.getIDURL():
                 to_be_listed = True
             if include_granted and _glob_id['idurl'] != my_id.getIDURL():
                 to_be_listed = True
             if not to_be_listed:
                 continue
@@ -2933,14 +2941,16 @@
                 continue
             results.append(cur_share.to_json())
         return RESULT(results)
     for key_id in my_keys.known_keys():
         if not key_id.startswith('share_'):
             continue
         key_alias, creator_idurl = my_keys.split_key_id(key_id)
+        if not id_url.is_cached(creator_idurl):
+            continue
         to_be_listed = False
         if include_mine and creator_idurl == my_id.getIDURL():
             to_be_listed = True
         if include_granted and creator_idurl != my_id.getIDURL():
             to_be_listed = True
         if not to_be_listed:
             continue
```

### Comparing `bitdust-0.1.6.231/bitdust/interface/api_rest_http_server.py` & `bitdust-0.1.7.233/bitdust/interface/api_rest_http_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/interface/api_web_socket.py` & `bitdust-0.1.7.233/bitdust/interface/api_web_socket.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/interface/cmd_line_json.py` & `bitdust-0.1.7.233/bitdust/interface/cmd_line_json.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/interface/cmd_line_json_templates.py` & `bitdust-0.1.7.233/bitdust/interface/cmd_line_json_templates.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/interface/ftp_server.py` & `bitdust-0.1.7.233/bitdust/interface/ftp_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/__init__.py` & `bitdust-0.1.7.233/bitdust/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/diskspace.py` & `bitdust-0.1.7.233/bitdust/lib/diskspace.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/getsizeof.py` & `bitdust-0.1.7.233/bitdust/lib/getsizeof.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/jsn.py` & `bitdust-0.1.7.233/bitdust/lib/jsn.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/jsontemplate.py` & `bitdust-0.1.7.233/bitdust/lib/jsontemplate.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/maths.py` & `bitdust-0.1.7.233/bitdust/lib/maths.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/misc.py` & `bitdust-0.1.7.233/bitdust/lib/misc.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/nameurl.py` & `bitdust-0.1.7.233/bitdust/lib/nameurl.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/net_misc.py` & `bitdust-0.1.7.233/bitdust/lib/net_misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -928,14 +928,20 @@
             ips = []
             for ip in ips_unicode:
                 ips.append(str(ip))
             del ips_unicode
             return ips
 
     elif plat == 'Linux':
+        if sys.executable == 'android_python' or ('ANDROID_ARGUMENT' in os.environ or 'ANDROID_ROOT' in os.environ):
+            # fake nw interface on Android
+            return [
+                '127.0.0.1',
+            ]
+
         try:
             pipe = os.popen('`which ip` -f inet a')
         except IOError:
             return []
         try:
             rawtxt = six.text_type(pipe.read())
             lines = rawtxt.splitlines()
```

### Comparing `bitdust-0.1.6.231/bitdust/lib/packetid.py` & `bitdust-0.1.7.233/bitdust/lib/packetid.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/schedule.py` & `bitdust-0.1.7.233/bitdust/lib/schedule.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/serialization.py` & `bitdust-0.1.7.233/bitdust/lib/serialization.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/strng.py` & `bitdust-0.1.7.233/bitdust/lib/strng.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/txws.py` & `bitdust-0.1.7.233/bitdust/lib/txws.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/udp.py` & `bitdust-0.1.7.233/bitdust/lib/udp.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/utime.py` & `bitdust-0.1.7.233/bitdust/lib/utime.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/lib/websock.py` & `bitdust-0.1.7.233/bitdust/lib/websock.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/logs/__init__.py` & `bitdust-0.1.7.233/bitdust/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/logs/lg.py` & `bitdust-0.1.7.233/bitdust/logs/lg.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     if level < 0:
         level = 0
     if level % 2:
         level -= 1
     if level:
         s = ' '*level + s
     if _IsAndroid is None:
-        _IsAndroid = (sys.executable == 'android_python' or ('ANDROID_ARGUMENT' in os.environ))
+        _IsAndroid = (sys.executable == 'android_python' or ('ANDROID_ARGUMENT' in os.environ or 'ANDROID_ROOT' in os.environ))
     if (_ShowTime and level > 0) or showtime:
         tm_string = time.strftime('%H:%M:%S')
         if _LifeBeginsTime != 0:
             dt = time.time() - _LifeBeginsTime
             mn = dt // 60
             sc = dt - mn*60
             if _GlobalDebugLevel >= 6:
@@ -474,15 +474,15 @@
     We will use ``level`` 2-6 for most important things and 10 for really
     minor stuff.
 
     Level 14 and higher is for things we don't think we want to see
     again. Can set ``level`` to 0 for no debug messages at all.
     """
     global _GlobalDebugLevel
-    _GlobalDebugLevel = level
+    _GlobalDebugLevel = int(level)
 
 
 def get_debug_level():
     """
     Returns currently set debug level.
     """
     global _GlobalDebugLevel
```

### Comparing `bitdust-0.1.6.231/bitdust/logs/measure_it.py` & `bitdust-0.1.7.233/bitdust/logs/measure_it.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/logs/memdebug.py` & `bitdust-0.1.7.233/bitdust/logs/memdebug.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/logs/weblog.py` & `bitdust-0.1.7.233/bitdust/logs/weblog.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/logs/webtraffic.py` & `bitdust-0.1.7.233/bitdust/logs/webtraffic.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/__init__.py` & `bitdust-0.1.7.233/bitdust/main/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/bpmain.py` & `bitdust-0.1.7.233/bitdust/main/bpmain.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,23 +591,32 @@
     """
     Prints the copyright string.
     """
     print('Copyright (C) 2008 Veselin Penev, https://bitdust.io')
 
 
 #--- THE ENTRY POINT
-def main(executable_path=None, start_reactor=True):
+def main(executable_path=None, start_reactor=True, appdir=None):
     """
     THE ENTRY POINT
     """
     global _AppDataDir
 
+    if _Debug:
+        print_text('ENTRY POINT: executable_path=%s appdir=%s' % (
+            executable_path,
+            appdir,
+        ))
+
     pars = parser()
     (opts, args) = pars.parse_args()
 
+    if not appdir:
+        appdir = opts.appdir
+
     if opts.coverage:
         import coverage  # @UnresolvedImport
         cov = coverage.Coverage(config_file=opts.coverage_config)
         cov.start()
 
     overDict = override_options(opts, args)
 
@@ -663,16 +672,16 @@
         src += '# Run:\n'
         src += '#     python3 bitdust.py alias > /usr/local/bin/bitdust\n'
         src += '#     chmod +x /usr/local/bin/bitdust\n'
         src += '%s %s/bitdust.py "$@"\n' % (python_path, curpath)
         print_text(src)
         return 0
 
-    if opts.appdir:
-        appdata = opts.appdir
+    if appdir:
+        appdata = appdir
         _AppDataDir = appdata
 
     else:
         curdir = os.getcwd()
         appdatafile = os.path.join(curdir, 'appdata')
         defaultappdata = deploy.default_base_dir_portable()
         appdata = defaultappdata
@@ -681,28 +690,33 @@
                 appdata = os.path.abspath(open(appdatafile, 'rb').read().strip())
             except:
                 appdata = defaultappdata
             if not os.path.isdir(appdata):
                 appdata = defaultappdata
         _AppDataDir = appdata
 
+    if _Debug:
+        print_text('_AppDataDir: %s' % _AppDataDir)
+        print_text('default_base_dir_portable(): %s' % deploy.default_base_dir_portable())
+
     #---BitDust Home
     deploy.init_base_dir(base_dir=_AppDataDir)
 
     from bitdust.logs import lg
 
     #---init IO module
     from bitdust.system import bpio
     bpio.init()
 
     appList = bpio.find_main_process(pid_file_path=os.path.join(appdata, 'processid'))
 
     if bpio.Android():
         lg.close_intercepted_log_file()
-        lg.open_intercepted_log_file('/storage/emulated/0/Android/data/org.bitdust_io.bitdust1/files/Documents/.bitdust/logs/android.log')
+        from android.storage import app_storage_path  # @UnresolvedImport
+        lg.open_intercepted_log_file(os.path.join(app_storage_path(), '.bitdust', 'logs', 'android.log'))
 
     # sys.excepthook = lg.exception_hook
 
     #---init logging
     from twisted.internet.defer import setDebugging
     if _Debug:
         if bpio.isFrozen():
```

### Comparing `bitdust-0.1.6.231/bitdust/main/bptester.py` & `bitdust-0.1.7.233/bitdust/main/bptester.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,17 @@
             try:
                 appdata = os.path.abspath(open(os.path.join(curdir, 'appdata'), 'r').read().strip())
             except:
                 appdata = os.path.join(os.path.expanduser('~'), '.bitdust')
             if not os.path.isdir(appdata):
                 appdata = os.path.join(os.path.expanduser('~'), '.bitdust')
         else:
-            if sys.executable == 'android_python' or ('ANDROID_ARGUMENT' in os.environ):
-                appdata = '/storage/emulated/0/Android/data/org.bitdust_io.bitdust1/files/Documents/.bitdust'
+            if sys.executable == 'android_python' or ('ANDROID_ARGUMENT' in os.environ or 'ANDROID_ROOT' in os.environ):
+                from android.storage import app_storage_path  # @UnresolvedImport
+                appdata = os.path.join(app_storage_path(), '.bitdust')
             else:
                 appdata = os.path.join(os.path.expanduser('~'), '.bitdust')
         AppData = appdata
     if not CurrentNetwork:
         try:
             cur_network = open(os.path.join(AppData, 'current_network'), 'r').read().strip()
         except:
```

### Comparing `bitdust-0.1.6.231/bitdust/main/config.py` & `bitdust-0.1.7.233/bitdust/main/config.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/config_defaults.py` & `bitdust-0.1.7.233/bitdust/main/config_defaults.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/config_details.py` & `bitdust-0.1.7.233/bitdust/main/config_details.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/config_types.py` & `bitdust-0.1.7.233/bitdust/main/config_types.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/default_network.py` & `bitdust-0.1.7.233/bitdust/main/default_network.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/events.py` & `bitdust-0.1.7.233/bitdust/main/events.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/help.py` & `bitdust-0.1.7.233/bitdust/main/help.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/initializer.py` & `bitdust-0.1.7.233/bitdust/main/initializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,16 @@
 
     def doInitServices(self, *args, **kwargs):
         """
         Action method.
         """
         if bpio.Android():
             lg.close_intercepted_log_file()
-            lg.open_intercepted_log_file('/storage/emulated/0/Android/data/org.bitdust_io.bitdust1/files/Documents/.bitdust/logs/android.log', mode='a')
+            from android.storage import app_storage_path  # @UnresolvedImport
+            lg.open_intercepted_log_file(os.path.join(app_storage_path(), '.bitdust', 'logs', 'android.log'), mode='a')
             if _Debug:
                 lg.dbg(_DebugLevel, 'log file "android.log" re-opened')
         if _Debug:
             lg.out(_DebugLevel, 'initializer.doInitServices')
         d = init_services()
         d.addBoth(lambda x: self.automat('init-services-done'))
```

### Comparing `bitdust-0.1.6.231/bitdust/main/install_wizard.py` & `bitdust-0.1.7.233/bitdust/main/install_wizard.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/installer.py` & `bitdust-0.1.7.233/bitdust/main/installer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/listeners.py` & `bitdust-0.1.7.233/bitdust/main/listeners.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/network_config.py` & `bitdust-0.1.7.233/bitdust/main/network_config.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/main/settings.py` & `bitdust-0.1.7.233/bitdust/main/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -630,16 +630,19 @@
     return os.path.join(bpio.getExecutableDir(), 'appdata')
 
 
 def DefaultRestoreDir():
     """
     Default location to place restored files and folders.
     """
-    if sys.executable == 'android_python' or ('ANDROID_ARGUMENT' in os.environ):
-        return '/storage/emulated/0/Android/data/org.bitdust_io.bitdust1/files/Downloads'
+    if bpio.Android():
+        # from android.storage import primary_external_storage_path  # @UnresolvedImport
+        # return os.path.join(primary_external_storage_path(), 'Download')
+        from android.storage import app_storage_path  # @UnresolvedImport
+        return app_storage_path()
     return os.path.expanduser('~')
 
 
 def MetaDataDir():
     """
     Return current location of the "metadata" folder - most important config files is here.
     """
```

### Comparing `bitdust-0.1.6.231/bitdust/main/shutdowner.py` & `bitdust-0.1.7.233/bitdust/main/shutdowner.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/__init__.py` & `bitdust-0.1.7.233/bitdust/p2p/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/commands.py` & `bitdust-0.1.7.233/bitdust/p2p/commands.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/handshaker.py` & `bitdust-0.1.7.233/bitdust/p2p/handshaker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/id_rotator.py` & `bitdust-0.1.7.233/bitdust/p2p/id_rotator.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/lookup.py` & `bitdust-0.1.7.233/bitdust/p2p/lookup.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/network_connector.py` & `bitdust-0.1.7.233/bitdust/p2p/network_connector.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/network_service.py` & `bitdust-0.1.7.233/bitdust/p2p/network_service.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/online_status.py` & `bitdust-0.1.7.233/bitdust/p2p/online_status.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/p2p_connector.py` & `bitdust-0.1.7.233/bitdust/p2p/p2p_connector.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/p2p_service.py` & `bitdust-0.1.7.233/bitdust/p2p/p2p_service.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/p2p_service_seeker.py` & `bitdust-0.1.7.233/bitdust/p2p/p2p_service_seeker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/p2p_stats.py` & `bitdust-0.1.7.233/bitdust/p2p/p2p_stats.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/propagate.py` & `bitdust-0.1.7.233/bitdust/p2p/propagate.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/p2p/ratings.py` & `bitdust-0.1.7.233/bitdust/p2p/ratings.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/raid/__init__.py` & `bitdust-0.1.7.233/bitdust/raid/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/raid/eccmap.py` & `bitdust-0.1.7.233/bitdust/raid/eccmap.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/raid/make.py` & `bitdust-0.1.7.233/bitdust/raid/make.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/raid/raid_worker.py` & `bitdust-0.1.7.233/bitdust/raid/raid_worker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/raid/raidutils.py` & `bitdust-0.1.7.233/bitdust/raid/raidutils.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/raid/read.py` & `bitdust-0.1.7.233/bitdust/raid/read.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/raid/rebuild.py` & `bitdust-0.1.7.233/bitdust/raid/rebuild.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/raid/worker.py` & `bitdust-0.1.7.233/bitdust/raid/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,17 @@
                 print('worker got Exception in queue -- exiting')
 
         return res
 
 
 def func_thread(tasks, pool):
     while True:
+        if _Debug:
+            lg.out(_DebugLevel, 'raid.worker.func_thread tasks: %d' % len(tasks))
+
         try:
             _WorkerQueue.get()
         except (EOFError, OSError, IOError):
             print('publisher got EOFError or OSError or IOError -- exiting')
             break
 
         with _WorkerLock:
@@ -89,15 +92,15 @@
                 task = tasks.popitem(last=False)
             except KeyError:
                 task = None
 
         if task:
             func, params, callback, error_callback, task_id = task[1]
             if _Debug:
-                lg.out(_DebugLevel, 'raid.worker.func_thread is going to apply task %s' % task_id)
+                lg.out(_DebugLevel, 'raid.worker.func_thread is going to apply task %s with callback %r' % (task_id, callback, ))
             if six.PY3:
                 pool.apply_async(func=func, args=params + (task_id, ), callback=callback, error_callback=error_callback)
             else:
                 pool.apply_async(func=func, args=params + (task_id, ), callback=callback)
         else:
             try:
                 _WorkerQueue.put(1)
```

### Comparing `bitdust-0.1.6.231/bitdust/services/__init__.py` & `bitdust-0.1.7.233/bitdust/services/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/driver.py` & `bitdust-0.1.7.233/bitdust/services/driver.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/local_service.py` & `bitdust-0.1.7.233/bitdust/services/local_service.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_accountant.py` & `bitdust-0.1.7.233/bitdust/services/service_accountant.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_backup_db.py` & `bitdust-0.1.7.233/bitdust/services/service_backup_db.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_backups.py` & `bitdust-0.1.7.233/bitdust/services/service_backups.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_blockchain.py` & `bitdust-0.1.7.233/bitdust/services/service_blockchain.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_broadcasting.py` & `bitdust-0.1.7.233/bitdust/services/service_broadcasting.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_contract_chain.py` & `bitdust-0.1.7.233/bitdust/services/service_contract_chain.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_customer.py` & `bitdust-0.1.7.233/bitdust/services/service_customer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_customer_contracts.py` & `bitdust-0.1.7.233/bitdust/services/service_customer_contracts.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_customer_family.py` & `bitdust-0.1.7.233/bitdust/services/service_customer_family.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_customer_patrol.py` & `bitdust-0.1.7.233/bitdust/services/service_customer_patrol.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_customer_support.py` & `bitdust-0.1.7.233/bitdust/services/service_customer_support.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_data_disintegration.py` & `bitdust-0.1.7.233/bitdust/services/service_data_disintegration.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_data_motion.py` & `bitdust-0.1.7.233/bitdust/services/service_data_motion.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_employer.py` & `bitdust-0.1.7.233/bitdust/services/service_employer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_entangled_dht.py` & `bitdust-0.1.7.233/bitdust/services/service_entangled_dht.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_gateway.py` & `bitdust-0.1.7.233/bitdust/services/service_gateway.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_http_connections.py` & `bitdust-0.1.7.233/bitdust/services/service_http_connections.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_http_transport.py` & `bitdust-0.1.7.233/bitdust/services/service_http_transport.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_identity_propagate.py` & `bitdust-0.1.7.233/bitdust/services/service_identity_propagate.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_identity_server.py` & `bitdust-0.1.7.233/bitdust/services/service_identity_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_ip_port_responder.py` & `bitdust-0.1.7.233/bitdust/services/service_ip_port_responder.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_keys_registry.py` & `bitdust-0.1.7.233/bitdust/services/service_keys_registry.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_keys_storage.py` & `bitdust-0.1.7.233/bitdust/services/service_keys_storage.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_list_files.py` & `bitdust-0.1.7.233/bitdust/services/service_list_files.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_message_broker.py` & `bitdust-0.1.7.233/bitdust/services/service_message_broker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_message_history.py` & `bitdust-0.1.7.233/bitdust/services/service_message_history.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_miner.py` & `bitdust-0.1.7.233/bitdust/services/service_miner.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_my_data.py` & `bitdust-0.1.7.233/bitdust/services/service_my_data.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_my_ip_port.py` & `bitdust-0.1.7.233/bitdust/services/service_my_ip_port.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_network.py` & `bitdust-0.1.7.233/bitdust/services/service_network.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_nodes_lookup.py` & `bitdust-0.1.7.233/bitdust/services/service_nodes_lookup.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_p2p_hookups.py` & `bitdust-0.1.7.233/bitdust/services/service_p2p_hookups.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_p2p_notifications.py` & `bitdust-0.1.7.233/bitdust/services/service_p2p_notifications.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_personal_messages.py` & `bitdust-0.1.7.233/bitdust/services/service_personal_messages.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_private_groups.py` & `bitdust-0.1.7.233/bitdust/services/service_private_groups.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_private_messages.py` & `bitdust-0.1.7.233/bitdust/services/service_private_messages.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_proxy_server.py` & `bitdust-0.1.7.233/bitdust/services/service_proxy_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_proxy_transport.py` & `bitdust-0.1.7.233/bitdust/services/service_proxy_transport.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_rebuilding.py` & `bitdust-0.1.7.233/bitdust/services/service_rebuilding.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_restores.py` & `bitdust-0.1.7.233/bitdust/services/service_restores.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_shared_data.py` & `bitdust-0.1.7.233/bitdust/services/service_shared_data.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_supplier.py` & `bitdust-0.1.7.233/bitdust/services/service_supplier.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_supplier_contracts.py` & `bitdust-0.1.7.233/bitdust/services/service_supplier_contracts.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_tcp_connections.py` & `bitdust-0.1.7.233/bitdust/services/service_tcp_connections.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_tcp_transport.py` & `bitdust-0.1.7.233/bitdust/services/service_tcp_transport.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_udp_datagrams.py` & `bitdust-0.1.7.233/bitdust/services/service_udp_datagrams.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/services/service_udp_transport.py` & `bitdust-0.1.7.233/bitdust/services/service_udp_transport.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/storage/__init__.py` & `bitdust-0.1.7.233/bitdust/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/storage/accounting.py` & `bitdust-0.1.7.233/bitdust/storage/accounting.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/storage/archive_reader.py` & `bitdust-0.1.7.233/bitdust/storage/archive_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,18 +340,19 @@
         if _Debug:
             lg.args(_DebugLevel, backup_index=backup_index, selected_backups=len(self.selected_backups))
         if backup_index >= len(self.selected_backups):
             lg.info('all selected backups are processed')
             self.automat('extract-all-done', self.extracted_messages)
             return
         backup_id = self.selected_backups[backup_index]
+        alias = backup_id.split('$')[0]
         outfd, outfilename = tmpfile.make(
             'restore',
             extension='.tar.gz',
-            prefix=backup_id.replace('@', '_').replace('.', '_').replace('/', '_').replace(':', '_') + '_',
+            prefix=alias + '_',
         )
         rw = restore_worker.RestoreWorker(backup_id, outfd, KeyID=self.group_key_id)
         rw.MyDeferred.addCallback(self._on_restore_done, backup_id, outfd, outfilename, backup_index)
         rw.MyDeferred.addErrback(lg.errback, debug=_Debug, debug_level=_DebugLevel, method='archive_reader.doStartRestoreWorker')
         rw.MyDeferred.addErrback(self._on_restore_failed, backup_id, outfd, outfilename, backup_index)
         rw.automat('init')
```

### Comparing `bitdust-0.1.6.231/bitdust/storage/archive_writer.py` & `bitdust-0.1.7.233/bitdust/storage/archive_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,18 +276,15 @@
         backup_id = packetid.MakeBackupID(
             customer=self.queue_owner_id,
             path_id=supplier_path_id,
             key_alias=self.queue_alias,
             version=dataID,
         )
         backup_fs.MakeLocalDir(settings.getLocalBackupsDir(), backup_id)
-        if bpio.Android():
-            compress_mode = 'none'
-        else:
-            compress_mode = 'bz2'
+        compress_mode = 'bz2'
         arcname = os.path.basename(local_path)
         backupPipe = backup_tar.backuptarfile_thread(local_path, arcname=arcname, compress=compress_mode)
         self.backup_job = backup.backup(
             backupID=backup_id,
             pipe=backupPipe,
             blockResultCallback=self._on_archive_backup_block_result,
             finishCallback=self._on_archive_backup_done,
```

### Comparing `bitdust-0.1.6.231/bitdust/storage/backup.py` & `bitdust-0.1.7.233/bitdust/storage/backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,15 +577,15 @@
     automat.LifeBegins(lg.when_life_begins())
     automat.OpenLogFile(settings.AutomatsLog())
 
     key.InitMyKey()
     my_id.init()
 
     sourcePath = sys.argv[1]
-    compress_mode = 'none'  # 'gz'
+    compress_mode = 'bz2'
     backupID = sys.argv[2]
     raid_worker.A('init')
 
     if bpio.pathIsDir(sourcePath):
         backupPipe = backup_tar.backuptardir_thread(sourcePath, compress=compress_mode)
     else:
         backupPipe = backup_tar.backuptarfile_thread(sourcePath, compress=compress_mode)
```

### Comparing `bitdust-0.1.6.231/bitdust/storage/backup_control.py` & `bitdust-0.1.7.233/bitdust/storage/backup_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -618,18 +618,15 @@
             backup_fs.MakeLocalDir(settings.getLocalBackupsDir(), self.backupID)
         except:
             lg.exc()
             if _Debug:
                 lg.out(_DebugLevel, 'backup_control.Task.run ERROR creating destination folder for %s' % self.pathID)
             err = 'failed creating destination folder for "%s"' % self.backupID
             return OnTaskFailed(self.backupID, err)
-        if bpio.Android():
-            compress_mode = 'none'
-        else:
-            compress_mode = 'bz2'  # 'none' # 'gz'
+        compress_mode = 'bz2'
         arcname = os.path.basename(sourcePath)
         from bitdust.storage import backup_tar
         if bpio.pathIsDir(self.localPath):
             backupPipe = backup_tar.backuptardir_thread(self.localPath, arcname=arcname, compress=compress_mode)
         else:
             backupPipe = backup_tar.backuptarfile_thread(self.localPath, arcname=arcname, compress=compress_mode)
         job = backup.backup(
```

### Comparing `bitdust-0.1.6.231/bitdust/storage/backup_fs.py` & `bitdust-0.1.7.233/bitdust/storage/backup_fs.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/storage/backup_matrix.py` & `bitdust-0.1.7.233/bitdust/storage/backup_matrix.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/storage/backup_monitor.py` & `bitdust-0.1.7.233/bitdust/storage/backup_monitor.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/storage/backup_rebuilder.py` & `bitdust-0.1.7.233/bitdust/storage/backup_rebuilder.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/storage/backup_schedule.py` & `bitdust-0.1.7.233/bitdust/storage/backup_schedule.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/storage/backup_tar.py` & `bitdust-0.1.7.233/bitdust/storage/backup_tar.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,15 @@
             lg.out(_DebugLevel, 'backup_tar.backuptarfile_thread writetar() finished')
         return ret
 
     reactor.callInThread(_run)  # @UndefinedVariable
     return p
 
 
-def backuptardir_thread(directorypath, arcname=None, recursive_subfolders=True, compress=None):
+def backuptardir_thread(directorypath, arcname=None, recursive_subfolders=True, compress='bz2'):
     """
     Makes tar archive of a single file inside a thread.
     Returns `BytesLoop` object instance which can be used to read produced data in parallel.
     """
     if not bpio.pathIsDir(directorypath):
         lg.err('folder %s not found' % directorypath)
         return None
@@ -216,31 +216,35 @@
             lg.out(_DebugLevel, 'backup_tar.backuptardir_thread writetar() finished')
         return ret
 
     reactor.callInThread(_run)  # @UndefinedVariable
     return p
 
 
-def extracttar_thread(tarfile, outdir):
+def extracttar_thread(tarfile, outdir, mode='r:bz2'):
     """
     Opposite method, extract files and folders from ".tar" file inside a thread.
     """
     if not os.path.isfile(tarfile):
         lg.err('path %s not found' % tarfile)
         return None
     if _Debug:
-        lg.out(_DebugLevel, 'backup_tar.extracttar_thread %s %s' % (tarfile, outdir))
+        lg.out(_DebugLevel, 'backup_tar.extracttar_thread tarfile=%s' % tarfile)
 
     def _run():
+        if _Debug:
+            lg.out(_DebugLevel, 'backup_tar.extracttar_thread._run outdir=%s' % outdir)
         from bitdust.storage import tar_file
-        return tar_file.readtar(
+        ret = tar_file.readtar(
             archivepath=tarfile,
             outputdir=outdir,
             encoding='utf-8',
+            mode=mode,
         )
+        return ret
 
     return threads.deferToThread(_run)  # @UndefinedVariable
 
 
 #------------------------------------------------------------------------------
```

### Comparing `bitdust-0.1.6.231/bitdust/storage/index_synchronizer.py` & `bitdust-0.1.7.233/bitdust/storage/index_synchronizer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/storage/keys_synchronizer.py` & `bitdust-0.1.7.233/bitdust/storage/keys_synchronizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,17 @@
             for i in lookup:
                 if i['path'].endswith('.public'):
                     stored_key_id = i['path'].replace('.public', '').replace('.keys/', '')
                     is_private = False
                 else:
                     stored_key_id = i['path'].replace('.private', '').replace('.keys/', '')
                     is_private = True
+                if not my_keys.is_valid_key_id(stored_key_id):
+                    lg.warn('not able to recognize stored key_id from item: %r' % i)
+                    continue
                 stored_key_id = my_keys.latest_key_id(stored_key_id)
                 is_reliable = False
                 for v in i['versions']:
                     try:
                         reliable = float(v['reliable'].replace('%', ''))
                     except:
                         lg.exc()
```

### Comparing `bitdust-0.1.6.231/bitdust/storage/restore_monitor.py` & `bitdust-0.1.7.233/bitdust/storage/restore_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,16 @@
     return err
 
 
 def restore_done(result, backupID, outfd, tarfilename, outputlocation, callback_method):
     global _WorkingBackupIDs
     global _WorkingRestoreProgress
     global OnRestoreDoneFunc
+    if _Debug:
+        lg.args(_DebugLevel, result=result, bid=backupID, tar=tarfilename, out=outputlocation)
     if result == 'done':
         lg.info('restore success of %s with result=%s' % (backupID, result))
     else:
         lg.err('restore failed of %s with result=%s' % (backupID, result))
     try:
         os.close(outfd)
     except:
@@ -183,18 +185,19 @@
 def Start(backupID, outputLocation, callback=None, keyID=None):
     if _Debug:
         lg.out(_DebugLevel, 'restore_monitor.Start %s to %s' % (backupID, outputLocation))
     global _WorkingBackupIDs
     global _WorkingRestoreProgress
     if backupID in list(_WorkingBackupIDs.keys()):
         return _WorkingBackupIDs[backupID]
+    alias = backupID.split('$')[0]
     outfd, outfilename = tmpfile.make(
         'restore',
         extension='.tar.gz',
-        prefix=backupID.replace('@', '_').replace('.', '_').replace('/', '_').replace(':', '_') + '_',
+        prefix=alias + '_',
     )
     from bitdust.storage import restore_worker
     r = restore_worker.RestoreWorker(backupID, outfd, KeyID=keyID)
     r.MyDeferred.addCallback(restore_done, backupID, outfd, outfilename, outputLocation, callback)
     r.set_block_restored_callback(block_restored_callback)
     r.set_packet_in_callback(packet_in_callback)
     _WorkingBackupIDs[backupID] = r
```

### Comparing `bitdust-0.1.6.231/bitdust/storage/restore_worker.py` & `bitdust-0.1.7.233/bitdust/storage/restore_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,18 +486,19 @@
         if _Debug:
             lg.out(_DebugLevel, 'restore_worker.doSavePacket %s saved to %s' % (packetID, filename))
 
     def doReadRaid(self, *args, **kwargs):
         """
         Action method.
         """
+        alias = self.backup_id.split('$')[0]
         _, outfilename = tmpfile.make(
             'restore',
             extension='.raid',
-            prefix=self.backup_id.replace(':', '_').replace('@', '_').replace('/', '_') + '_' + str(self.block_number) + '_',
+            prefix=alias + '_' + str(self.block_number) + '_',
             close_fd=True,
         )
         inputpath = os.path.join(settings.getLocalBackupsDir(), self.customer_id, self.path_id)
         task_params = (outfilename, self.EccMap.name, self.version, self.block_number, inputpath)
         raid_worker.add_task('read', task_params, lambda cmd, params, result: self._on_block_restored(result, outfilename))
 
     def doRemoveTempFile(self, *args, **kwargs):
```

### Comparing `bitdust-0.1.6.231/bitdust/storage/tar_file.py` & `bitdust-0.1.7.233/bitdust/storage/tar_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,16 +131,17 @@
             try:
                 appdata = os.path.abspath(open(os.path.join(curdir, 'appdata'), 'rb').read().strip())
             except:
                 appdata = os.path.join(os.path.expanduser('~'), '.bitdust')
             if not os.path.isdir(appdata):
                 appdata = os.path.join(os.path.expanduser('~'), '.bitdust')
         else:
-            if sys.executable == 'android_python' or ('ANDROID_ARGUMENT' in os.environ):
-                appdata = '/storage/emulated/0/Android/data/org.bitdust_io.bitdust1/files/Documents/.bitdust'
+            if sys.executable == 'android_python' or ('ANDROID_ARGUMENT' in os.environ or 'ANDROID_ROOT' in os.environ):
+                from android.storage import app_storage_path  # @UnresolvedImport
+                appdata = os.path.join(app_storage_path(), '.bitdust')
             else:
                 appdata = os.path.join(os.path.expanduser('~'), '.bitdust')
         AppData = appdata
     return os.path.join(AppData, subdir, filename)
 
 
 def logfilepath():
@@ -238,66 +239,74 @@
         return None
     return tarinfo
 
 
 #------------------------------------------------------------------------------
 
 
-def writetar(sourcepath, arcname=None, subdirs=True, compression='none', encoding=None, fileobj=None):
+def writetar(sourcepath, arcname=None, subdirs=True, compression='none', encoding=None, fileobj=None, mode=None):
     """
     Create a tar archive from given ``sourcepath`` location.
     """
     global _ExcludeFunction
     if _Debug:
         printlog('WRITE: %s arcname=%s, subdirs=%s, compression=%s, encoding=%s\n' % (sourcepath, arcname, subdirs, compression, encoding))
     if not fileobj:
         fileobj = sys.stdout
-    mode = 'w|'
-    if compression != 'none':
-        mode += compression
+    if not mode:
+        if compression != 'none':
+            mode = 'w|' + compression
+        else:
+            mode = 'w|tar'
     _, filename = os.path.split(sourcepath)
     if arcname is None:
         arcname = to_text(filename)
     else:
         arcname = to_text(arcname)
     # DEBUG: tar = tarfile.open('', mode, fileobj=open('out.tar', 'wb'), encoding=encoding)
+    if _Debug:
+        printlog('OPEN: mode=%s fileobj=%r\n' % (mode, fileobj))
     tar = tarfile.open('', mode, fileobj=fileobj, encoding=encoding, bufsize=1024*1024)
+    if _Debug:
+        printlog('ADD: name=%s arcname=%r\n' % (sourcepath, arcname))
     tar.add(
         name=sourcepath,
         arcname=arcname,
         recursive=subdirs,
         filter=lambda tarinfo: writetar_filter(tarinfo, sourcepath),
     )
     if not subdirs and os.path.isdir(sourcepath):
         # the True is for recursive, if we wanted to just do the immediate directory set to False
         for subfile in os.listdir(sourcepath):
             subpath = os.path.join(sourcepath, subfile)
             if not os.path.isdir(subpath):
+                arcname = to_text(os.path.join(arcname, subfile))
+                if _Debug:
+                    printlog('ADD: name=%s arcname=%r\n' % (subpath, arcname))
                 tar.add(
                     name=subpath,
-                    arcname=to_text(os.path.join(arcname, subfile)),
+                    arcname=arcname,
                     recursive=False,
                     filter=lambda tarinfo: writetar_filter(tarinfo, subpath),
                 )
     tar.close()
     return True
 
 
 #------------------------------------------------------------------------------
 
 
-def readtar(archivepath, outputdir, encoding=None):
+def readtar(archivepath, outputdir, encoding=None, mode='r:*'):
     """
     Extract tar file from ``archivepath`` location into local ``outputdir``
     folder.
     """
     if _Debug:
-        printlog('READ: %s to %s, encoding=%s\n' % (archivepath, outputdir, encoding))
-    mode = 'r:*'
-    tar = tarfile.open(archivepath, mode, encoding=encoding)
+        printlog('READ: mode=%s name=%s outputdir=%s encoding=%s\n' % (mode, archivepath, outputdir, encoding))
+    tar = tarfile.open(name=archivepath, mode=mode, encoding=encoding)
     tar.extractall(outputdir)
     tar.close()
     return True
 
 
 #------------------------------------------------------------------------------
```

### Comparing `bitdust-0.1.6.231/bitdust/stream/__init__.py` & `bitdust-0.1.7.233/bitdust/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stream/broker_negotiator.py` & `bitdust-0.1.7.233/bitdust/stream/broker_negotiator.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stream/data_receiver.py` & `bitdust-0.1.7.233/bitdust/stream/data_receiver.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stream/data_sender.py` & `bitdust-0.1.7.233/bitdust/stream/data_sender.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stream/file_down.py` & `bitdust-0.1.7.233/bitdust/stream/file_down.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stream/file_up.py` & `bitdust-0.1.7.233/bitdust/stream/file_up.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stream/io_throttle.py` & `bitdust-0.1.7.233/bitdust/stream/io_throttle.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stream/message.py` & `bitdust-0.1.7.233/bitdust/stream/message.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stream/message_peddler.py` & `bitdust-0.1.7.233/bitdust/stream/message_peddler.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stream/message_producer.py` & `bitdust-0.1.7.233/bitdust/stream/message_producer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stream/p2p_queue.py` & `bitdust-0.1.7.233/bitdust/stream/p2p_queue.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stream/queue_keeper.py` & `bitdust-0.1.7.233/bitdust/stream/queue_keeper.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stun/__init__.py` & `bitdust-0.1.7.233/bitdust/stun/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stun/stun_client.py` & `bitdust-0.1.7.233/bitdust/stun/stun_client.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/stun/stun_server.py` & `bitdust-0.1.7.233/bitdust/stun/stun_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/supplier/__init__.py` & `bitdust-0.1.7.233/bitdust/supplier/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/supplier/customer_assistant.py` & `bitdust-0.1.7.233/bitdust/supplier/customer_assistant.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/supplier/customer_space.py` & `bitdust-0.1.7.233/bitdust/supplier/customer_space.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/supplier/customers_rejector.py` & `bitdust-0.1.7.233/bitdust/supplier/customers_rejector.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 
 #------------------------------------------------------------------------------
 
 from bitdust.logs import lg
 
 from bitdust.automats import automat
 
+from bitdust.system import bpio
+
 from bitdust.main import settings
 from bitdust.main import config
 
 from bitdust.interface import api
 
 from bitdust.contacts import contactsdb
 
@@ -153,14 +155,17 @@
         + consumed_bytes : how many space was taken from you by other users
         + free_bytes = donated_bytes - consumed_bytes : not yet allocated space
         + used_bytes : size of all files, which you store on your disk for your customers
         + ratio : currently used space compared to consumed space
         """
         if _Debug:
             lg.out(_DebugLevel, 'customers_rejector.doTestMyCapacity')
+        if bpio.Android():
+            self.automat('space-enough')
+            return
         failed_customers = set()
         current_customers = contactsdb.customers()
         donated_bytes = settings.getDonatedBytes()
         space_dict, free_space = accounting.read_customers_quotas()
         used_dict = accounting.read_customers_usage()
         unknown_customers, unused_quotas = accounting.validate_customers_quotas(space_dict, free_space)
         failed_customers.update(unknown_customers)
```

### Comparing `bitdust-0.1.6.231/bitdust/supplier/family_member.py` & `bitdust-0.1.7.233/bitdust/supplier/family_member.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/supplier/list_files.py` & `bitdust-0.1.7.233/bitdust/supplier/list_files.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/supplier/local_tester.py` & `bitdust-0.1.7.233/bitdust/supplier/local_tester.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/system/__init__.py` & `bitdust-0.1.7.233/bitdust/system/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/system/bpio.py` & `bitdust-0.1.7.233/bitdust/system/bpio.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 def ostype():
     """
     Return current platform: "Linux", "Windows", "Darwin".
     """
     global PlatformInfo
     if PlatformInfo is None:
         PlatformInfo = list(platform.uname())
-        if sys.executable == 'android_python' or ('ANDROID_ARGUMENT' in os.environ):
+        if sys.executable == 'android_python' or ('ANDROID_ARGUMENT' in os.environ or 'ANDROID_ROOT' in os.environ):
             PlatformInfo[0] = 'Android'
     return PlatformInfo[0]
 
 
 def osversion():
     """
     Return something like: "2.6.32.9-rscloud" or "XP".
@@ -236,14 +236,16 @@
     """
     Return True if output can be sent to console.
     """
     if getExecutableFilename().count('pythonw.exe'):
         return False
     if getExecutableFilename().count('bitdust-node.exe'):
         return False
+    if getExecutableFilename().count('BitDust-node'):
+        return False
     if not sys.stdout:
         return False
     return True
 
 
 #-------------------------------------------------------------------------------
 
@@ -1275,14 +1277,16 @@
         return []
     q = [
         'bitdust-node.exe',
         'bitdust-console.exe',
         'bitdustnode.exe',
         'BitDustNode.exe',
         'BitDustConsole.exe',  # 'bitdust.py',
+        'BitDust-node',
+        'bpmain.py',
     ]
     if os.environ.get('BITDUST_IN_DOCKER') == '1':
         q.extend([
             'regexp:^.*python.*bitdust.py.*?$',
         ])
     else:
         q.extend([
@@ -1318,14 +1322,15 @@
 def lookup_main_process():
     q = [
         'bitdust-node.exe',
         'bitdust-console.exe',
         'bitdustnode.exe',
         'BitDustNode.exe',
         'BitDustConsole.exe',
+        'BitDust-node',
         'bpmain.py',
     ]
     if os.environ.get('BITDUST_IN_DOCKER') == '1':
         q.extend([
             'regexp:^.*python.*bitdust.py.*?$',
         ])
     else:
```

### Comparing `bitdust-0.1.6.231/bitdust/system/child_process.py` & `bitdust-0.1.7.233/bitdust/system/child_process.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/system/deploy.py` & `bitdust-0.1.7.233/bitdust/system/deploy.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,32 +105,30 @@
 
 
 def default_base_dir_portable():
     """
     A portable method to get the default data folder location.
     """
     if platform.uname()[0] == 'Windows':
-        # TODO: move somewhere on Win10 ...
         return os.path.join(os.path.expanduser('~'), '.bitdust')
 
     elif platform.uname()[0] == 'Linux':
-        if 'ANDROID_ARGUMENT' in os.environ:
-            # We are on Android, it must be in /storage/emulated/0/.bitdust/
-            # I also tried /data/user/0/org.kivy.bitdust/files/app/.bitdust/ but then I can't browse files from other apps
-            # return os.path.join(os.environ.get('ANDROID_APP_PATH'), '.bitdust')
-            return '/storage/emulated/0/Android/data/org.bitdust_io.bitdust1/files/Documents/.bitdust'
+        if 'ANDROID_ARGUMENT' in os.environ or 'ANDROID_ROOT' in os.environ:
+            from android.storage import app_storage_path  # @UnresolvedImport
+            return os.path.join(app_storage_path(), '.bitdust')
 
-        # This should be okay : /home/veselin/.bitdust/
         return os.path.join(os.path.expanduser('~'), '.bitdust')
 
     elif platform.uname()[0] == 'Darwin':
-        # This should be okay : /Users/veselin/.bitdust/
         return os.path.join(os.path.expanduser('~'), '.bitdust')
 
-    # otherwise just default : ".bitdust/" in user root folder
+    elif 'ANDROID_ARGUMENT' in os.environ or 'ANDROID_ROOT' in os.environ:
+        from android.storage import app_storage_path  # @UnresolvedImport
+        return os.path.join(app_storage_path(), '.bitdust')
+
     return os.path.join(os.path.expanduser('~'), '.bitdust')
 
 
 def init_current_network(name=None, base_dir=None):
     global _CurrentNetwork
     base_dir = base_dir or current_base_dir()
     if name:
```

### Comparing `bitdust-0.1.6.231/bitdust/system/dirsize.py` & `bitdust-0.1.7.233/bitdust/system/dirsize.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/system/diskusage.py` & `bitdust-0.1.7.233/bitdust/system/diskusage.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/system/local_fs.py` & `bitdust-0.1.7.233/bitdust/system/local_fs.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/system/nonblocking.py` & `bitdust-0.1.7.233/bitdust/system/nonblocking.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/system/run_upnpc.py` & `bitdust-0.1.7.233/bitdust/system/run_upnpc.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/system/tmpfile.py` & `bitdust-0.1.7.233/bitdust/system/tmpfile.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/system/tray_icon.py` & `bitdust-0.1.7.233/bitdust/system/tray_icon.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/__init__.py` & `bitdust-0.1.7.233/bitdust/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/bandwidth.py` & `bitdust-0.1.7.233/bitdust/transport/bandwidth.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/callback.py` & `bitdust-0.1.7.233/bitdust/transport/callback.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/gateway.py` & `bitdust-0.1.7.233/bitdust/transport/gateway.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/http/__init__.py` & `bitdust-0.1.7.233/bitdust/transport/http/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/http/http_interface.py` & `bitdust-0.1.7.233/bitdust/transport/http/http_interface.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/http/http_node.py` & `bitdust-0.1.7.233/bitdust/transport/http/http_node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/http/sum_client.py` & `bitdust-0.1.7.233/bitdust/transport/http/sum_client.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/http/sum_server.py` & `bitdust-0.1.7.233/bitdust/transport/http/sum_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/http/transport_http_old.py` & `bitdust-0.1.7.233/bitdust/transport/http/transport_http_old.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/http/twisted-web-ssl.py` & `bitdust-0.1.7.233/bitdust/transport/http/twisted-web-ssl.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/network_transport.py` & `bitdust-0.1.7.233/bitdust/transport/network_transport.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/packet_in.py` & `bitdust-0.1.7.233/bitdust/transport/packet_in.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/packet_out.py` & `bitdust-0.1.7.233/bitdust/transport/packet_out.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/proxy/__init__.py` & `bitdust-0.1.7.233/bitdust/transport/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/proxy/proxy_interface.py` & `bitdust-0.1.7.233/bitdust/transport/proxy/proxy_interface.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/proxy/proxy_receiver.py` & `bitdust-0.1.7.233/bitdust/transport/proxy/proxy_receiver.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/proxy/proxy_router.py` & `bitdust-0.1.7.233/bitdust/transport/proxy/proxy_router.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/proxy/proxy_sender.py` & `bitdust-0.1.7.233/bitdust/transport/proxy/proxy_sender.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/tcp/__init__.py` & `bitdust-0.1.7.233/bitdust/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/tcp/tcp_connection.py` & `bitdust-0.1.7.233/bitdust/transport/tcp/tcp_connection.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/tcp/tcp_interface.py` & `bitdust-0.1.7.233/bitdust/transport/tcp/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/tcp/tcp_node.py` & `bitdust-0.1.7.233/bitdust/transport/tcp/tcp_node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/tcp/tcp_stream.py` & `bitdust-0.1.7.233/bitdust/transport/tcp/tcp_stream.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/udp/__init__.py` & `bitdust-0.1.7.233/bitdust/transport/udp/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/udp/udp_connector.py` & `bitdust-0.1.7.233/bitdust/transport/udp/udp_connector.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/udp/udp_file_queue.py` & `bitdust-0.1.7.233/bitdust/transport/udp/udp_file_queue.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/udp/udp_interface.py` & `bitdust-0.1.7.233/bitdust/transport/udp/udp_interface.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/udp/udp_node.py` & `bitdust-0.1.7.233/bitdust/transport/udp/udp_node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/udp/udp_session.py` & `bitdust-0.1.7.233/bitdust/transport/udp/udp_session.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/transport/udp/udp_stream.py` & `bitdust-0.1.7.233/bitdust/transport/udp/udp_stream.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/updates/__init__.py` & `bitdust-0.1.7.233/bitdust/updates/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/updates/git_proc.py` & `bitdust-0.1.7.233/bitdust/updates/git_proc.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/userid/__init__.py` & `bitdust-0.1.7.233/bitdust/userid/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/userid/global_id.py` & `bitdust-0.1.7.233/bitdust/userid/global_id.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/userid/id_registrator.py` & `bitdust-0.1.7.233/bitdust/userid/id_registrator.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/userid/id_restorer.py` & `bitdust-0.1.7.233/bitdust/userid/id_restorer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/userid/id_server.py` & `bitdust-0.1.7.233/bitdust/userid/id_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/userid/id_url.py` & `bitdust-0.1.7.233/bitdust/userid/id_url.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/userid/identity.py` & `bitdust-0.1.7.233/bitdust/userid/identity.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/userid/known_servers.py` & `bitdust-0.1.7.233/bitdust/userid/known_servers.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust/userid/my_id.py` & `bitdust-0.1.7.233/bitdust/userid/my_id.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust.egg-info/PKG-INFO` & `bitdust-0.1.7.233/bitdust.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,182 +1,19 @@
 Metadata-Version: 2.1
 Name: bitdust
-Version: 0.1.6.231
+Version: 0.1.7.233
 Summary: p2p secure distributed storage and communication engine
 Home-page: https://bitdust.io
+Download-URL: https://bitdust.io
 Author: Veselin Penev, BitDust
 Author-email: bitdust.io@gmail.com
 Maintainer: Veselin Penev, BitDust
 Maintainer-email: veselin@bitdust.io
 License: Copyright (C) 2008 Veselin Penev, https://bitdust.io
-Download-URL: https://bitdust.io
-Description: BitDust
-        =======
-        
-        BitDust is a peer to peer online backup utility.
-        
-        This is a distributed network for backup data storage. Each participant of the network provides a portion of his hard drive for other users. In exchange, he is able to store his data on other peers.
-        
-        The redundancy in backup makes it so if someone loses your data, you can rebuild what was lost and give it to someone else to hold. And all of this happens without you having to do a thing - the software keeps your data in safe.
-        
-        All your data is encrypted before it leaves your computer with a private key your computer generates. No one else can read your data, even BitDust Team! Recover data is only one way - download the necessary pieces from computers of other peers and decrypt them with your private key.
-        
-        BitDust is written in Python using pure Twisted framework and published under GNU AGPLv3.
-        
-        https://bitdust.io
-        
-        
-        
-        Current status
-        ==============
-        
-        Current project stage is about to only research opportunities of
-        building a holistic eco-system that protects your privacy in the network
-        by establishing p2p communications of users and maximize distribution of
-        information flows in the network.
-        
-        At the moment exists a very limited alpha version of the BitDust software.
-        We decided to publish those earlier works to verify/test/share our ideas and experiments with other people.
-        
-        
-        
-        Install BitDust software
-        ========================
-        
-        
-        1. Install software dependencies
-        
-        Seems like in Ubuntu (probably most other distros) you can install all dependencies in that way:
-        
-                sudo apt-get install git gcc python3-dev python3-virtualenv
-        
-        
-        Optionally, you can also install [miniupnpc](http://miniupnp.tuxfamily.org/) tool if you want BitDust automatically deal with UPnPc configuration of your network router so it can also accept incomming connections from other nodes.:
-        
-                sudo apt-get install miniupnpc
-        
-        
-        On MacOSX platform you can install requirements in that way:
-        
-                brew install git python3
-        
-        And use pip to get all required packages:
-        
-                pip install --upgrade --user
-                pip install --upgrade pip --user
-                pip install virtualenv --user
-        
-        
-        2. Get BitDust to your local machine
-        
-        Second step is to get the BitDust sources. To have a full control over BitDust process running on your local machine you better make a fork of the Public BitDist repository on GitHub at https://github.com/bitdust-io/public and clone it on your local machine:
-        
-                git clone https://github.com/<your GitHub username>/<name of BitDust fork>.git bitdust
-        
-        
-        The software will periodically run `git fetch` and `git rebase` to check for recent commits in the repo. This way we make sure that everyone is running the latest version of the program. Once you made a fork, you will have to update your Fork manually and pull commits from Public BitDust repository if you trust them.
-        
-        However if you just trust BitDust contributors you can simply clone the Public repository directly and software will be up to date with the "official" public code base:
-        
-                git clone https://github.com/bitdust-io/public.git bitdust
-        
-        
-        3. Building virtual environment
-        
-        Then you need to build virtual environment with all required Python dependencies, BitDust software will run fully isolated.
-        
-        Single command should make it for you, all required files will be generated in `~/.bitdust/venv/` sub-folder:
-        
-                cd bitdust
-                python3 bitdust.py install
-        
-        
-        Last step to make BitDust software ready is to make a short alias in your OS, then you can just type `bitdust` in command line to fast access the program:
-        
-                sudo ln -s -f /home/<user>/.bitdust/bitdust /usr/local/bin/bitdust
-        
-        
-        4. Run BitDust
-        
-        Start using the software by creating an identity for your device in BitDust network:
-        
-                bitdust id create <some nick name>
-        
-        
-        I recommend you to create another copy of your Private Key in a safe place to be able to recover your data in the future. You can do it with such command:
-        
-                bitdust key copy <nickname>.bitdust.key
-        
-        
-        Your settings and local files are located in that folder: ~/.bitdust
-        
-        Type this command to read more info about BitDust commands:
-        
-                bitdust help
-        
-        
-        To run the software type:
-        
-                bitdust
-        
-        
-        Start as background process:
-        
-                bitdust detach
-        
-        
-        To get some more insights or just to know how to start playing with software
-        you can visit [BitDust Commands](https://bitdust.io/commands.html) page.
-        
-        To get more info about API methods available go to [BitDust API](https://bitdust.io/api.html) page.
-        
-        
-        5. Binary Dependencies
-        
-        If you are installing BitDust on Windows platforms, you may require some binary packages already compiled and packaged for Microsoft Windows platforms, you can check following locations and download needed binaries and libraries:
-        
-        * cygwin: [cygwin.com](https://cygwin.com/install.html)
-        * git: [git-scm.com](https://git-scm.com/download/win)
-        * python2.7 or python3: [python.org](http://python.org/download/releases)
-        * twisted: [twistedmatrix.com](http://twistedmatrix.com)
-        * pyasn1: [pyasn1.sourceforge.net](http://pyasn1.sourceforge.net)
-        * miniupnpc: [miniupnp.tuxfamily.org](http://miniupnp.tuxfamily.org/)
-        
-        
-        
-        Docker Hub container image
-        ==========================
-        
-        You can also run bitdust inside Docker. We prepared a container which have BitDust installed and easy to run. You will have to SSH into the running container after start it and manually configure bitdust as you wish and run it:
-        
-                docker run -d -P --name bdnode bitdust/app1
-                docker port bdnode 22
-                0.0.0.0:32771  <-  learn which SSH port was opened on your host
-        
-        
-        Now you can ssh to the container, password is `bitdust`:
-        
-                ssh root@localhost -p 32771
-                password: bitdust
-        
-        
-        Inside the container you will have BitDust installed and ready to use, so you can run it directly:
-        
-                root@1ef6a46c3042:~# bitdust
-        
-        
-        
-        Feedback
-        ========
-        
-        You can contact [BitDust contributors](https://github.com/bitdust-io) on GitHub if you have any questions or ideas.
-        Welcome to the future!
-        
 Keywords: p2p,peer to peer,backup,restore,storage,data,recover,distributed,online,python,twisted,messaging,websocket,encryption,crypto,protection
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Twisted
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -194,7 +31,170 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+BitDust
+=======
+
+BitDust is a peer to peer online backup utility.
+
+This is a distributed network for backup data storage. Each participant of the network provides a portion of his hard drive for other users. In exchange, he is able to store his data on other peers.
+
+The redundancy in backup makes it so if someone loses your data, you can rebuild what was lost and give it to someone else to hold. And all of this happens without you having to do a thing - the software keeps your data in safe.
+
+All your data is encrypted before it leaves your computer with a private key your computer generates. No one else can read your data, even BitDust Team! Recover data is only one way - download the necessary pieces from computers of other peers and decrypt them with your private key.
+
+BitDust is written in Python using pure Twisted framework and published under GNU AGPLv3.
+
+https://bitdust.io
+
+
+
+Current status
+==============
+
+Current project stage is about to only research opportunities of
+building a holistic eco-system that protects your privacy in the network
+by establishing p2p communications of users and maximize distribution of
+information flows in the network.
+
+At the moment exists a very limited alpha version of the BitDust software.
+We decided to publish those earlier works to verify/test/share our ideas and experiments with other people.
+
+
+
+Install BitDust software
+========================
+
+
+1. Install software dependencies
+
+Seems like in Ubuntu (probably most other distros) you can install all dependencies in that way:
+
+        sudo apt-get install git gcc python3-dev python3-virtualenv
+
+
+Optionally, you can also install [miniupnpc](http://miniupnp.tuxfamily.org/) tool if you want BitDust automatically deal with UPnPc configuration of your network router so it can also accept incomming connections from other nodes.:
+
+        sudo apt-get install miniupnpc
+
+
+On MacOSX platform you can install requirements in that way:
+
+        brew install git python3
+
+And use pip to get all required packages:
+
+        pip install --upgrade --user
+        pip install --upgrade pip --user
+        pip install virtualenv --user
+
+
+2. Get BitDust to your local machine
+
+Second step is to get the BitDust sources. To have a full control over BitDust process running on your local machine you better make a fork of the Public BitDist repository on GitHub at https://github.com/bitdust-io/public and clone it on your local machine:
+
+        git clone https://github.com/<your GitHub username>/<name of BitDust fork>.git bitdust
+
+
+The software will periodically run `git fetch` and `git rebase` to check for recent commits in the repo. This way we make sure that everyone is running the latest version of the program. Once you made a fork, you will have to update your Fork manually and pull commits from Public BitDust repository if you trust them.
+
+However if you just trust BitDust contributors you can simply clone the Public repository directly and software will be up to date with the "official" public code base:
+
+        git clone https://github.com/bitdust-io/public.git bitdust
+
+
+3. Building virtual environment
+
+Then you need to build virtual environment with all required Python dependencies, BitDust software will run fully isolated.
+
+Single command should make it for you, all required files will be generated in `~/.bitdust/venv/` sub-folder:
+
+        cd bitdust
+        python3 bitdust.py install
+
+
+Last step to make BitDust software ready is to make a short alias in your OS, then you can just type `bitdust` in command line to fast access the program:
+
+        sudo ln -s -f /home/<user>/.bitdust/bitdust /usr/local/bin/bitdust
+
+
+4. Run BitDust
+
+Start using the software by creating an identity for your device in BitDust network:
+
+        bitdust id create <some nick name>
+
+
+I recommend you to create another copy of your Private Key in a safe place to be able to recover your data in the future. You can do it with such command:
+
+        bitdust key copy <nickname>.bitdust.key
+
+
+Your settings and local files are located in that folder: ~/.bitdust
+
+Type this command to read more info about BitDust commands:
+
+        bitdust help
+
+
+To run the software type:
+
+        bitdust
+
+
+Start as background process:
+
+        bitdust detach
+
+
+To get some more insights or just to know how to start playing with software
+you can visit [BitDust Commands](https://bitdust.io/commands.html) page.
+
+To get more info about API methods available go to [BitDust API](https://bitdust.io/api.html) page.
+
+
+5. Binary Dependencies
+
+If you are installing BitDust on Windows platforms, you may require some binary packages already compiled and packaged for Microsoft Windows platforms, you can check following locations and download needed binaries and libraries:
+
+* cygwin: [cygwin.com](https://cygwin.com/install.html)
+* git: [git-scm.com](https://git-scm.com/download/win)
+* python2.7 or python3: [python.org](http://python.org/download/releases)
+* twisted: [twistedmatrix.com](http://twistedmatrix.com)
+* pyasn1: [pyasn1.sourceforge.net](http://pyasn1.sourceforge.net)
+* miniupnpc: [miniupnp.tuxfamily.org](http://miniupnp.tuxfamily.org/)
+
+
+
+Docker Hub container image
+==========================
+
+You can also run bitdust inside Docker. We prepared a container which have BitDust installed and easy to run. You will have to SSH into the running container after start it and manually configure bitdust as you wish and run it:
+
+        docker run -d -P --name bdnode bitdust/app1
+        docker port bdnode 22
+        0.0.0.0:32771  <-  learn which SSH port was opened on your host
+
+
+Now you can ssh to the container, password is `bitdust`:
+
+        ssh root@localhost -p 32771
+        password: bitdust
+
+
+Inside the container you will have BitDust installed and ready to use, so you can run it directly:
+
+        root@1ef6a46c3042:~# bitdust
+
+
+
+Feedback
+========
+
+You can contact [BitDust contributors](https://github.com/bitdust-io) on GitHub if you have any questions or ideas.
+Welcome to the future!
```

### Comparing `bitdust-0.1.6.231/bitdust.egg-info/SOURCES.txt` & `bitdust-0.1.7.233/bitdust.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.txt
 setup.py
 bitdust/__init__.py
 bitdust.egg-info/PKG-INFO
 bitdust.egg-info/SOURCES.txt
 bitdust.egg-info/dependency_links.txt
 bitdust.egg-info/requires.txt
@@ -414,8 +415,20 @@
 bitdust_forks/websocket/_http.py
 bitdust_forks/websocket/_logging.py
 bitdust_forks/websocket/_socket.py
 bitdust_forks/websocket/_ssl_compat.py
 bitdust_forks/websocket/_url.py
 bitdust_forks/websocket/_utils.py
 scripts/bitdust
-scripts/bitdust_worker
+scripts/bitdust_worker
+tests/test_backup_fs.py
+tests/test_backup_restore.py
+tests/test_codernity_db.py
+tests/test_crypt_signed.py
+tests/test_id_url.py
+tests/test_identity.py
+tests/test_my_keys.py
+tests/test_raid_make_read.py
+tests/test_raid_manager.py
+tests/test_raid_worker.py
+tests/test_rsa_key.py
+tests/test_serialize.py
```

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/aliases.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/aliases.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/aliasesv2.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/aliasesv2.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/apihandler.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/apihandler.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/balance_nogui.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/balance_nogui.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/check_tx.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/check_tx.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/cmd_addpeers.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/cmd_addpeers.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/cmd_hn_last_block_ts.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/cmd_hn_last_block_ts.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/cmd_hn_reg_round.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/cmd_hn_reg_round.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/commands.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/commands.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/connectionmanager.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/connectionmanager.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/connections.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/connections.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/dbhandler.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/dbhandler.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/demo_getaddresssince.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/demo_getaddresssince.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/demo_getstatus.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/demo_getstatus.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/difficulty.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/difficulty.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/digest.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/digest.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/essentials.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/essentials.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/fork.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/fork.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/genesis.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/genesis.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/hmac_drbg.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/hmac_drbg.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/hyperlane.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/hyperlane.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/hyperlane_asyncio.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/hyperlane_asyncio.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/ledger_explorer.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/ledger_explorer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/log.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/log.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/mempool.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/mempool.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/mining.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/mining.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/mining_heavy3.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/mining_heavy3.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/node.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/node_stop.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/node_stop.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/optiexplorer.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/optiexplorer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/optihash.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/optihash.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/options.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/options.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/optipoolware.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/optipoolware.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/peershandler.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/peershandler.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/plugins.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/plugins.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/process_search.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/process_search.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/quantizer.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/quantizer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/regnet.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/regnet.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/rewards_reindex.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/rewards_reindex.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/rpcconnections.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/rpcconnections.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/send_csv.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/send_csv.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/send_nogui_noconf.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/send_nogui_noconf.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/simplecrypt.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/simplecrypt.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/staking.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/staking.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/tokensv2.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/tokensv2.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/wallet_keys.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/wallet_keys.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/wallet_server.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/wallet_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/wallet_websocket.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/wallet_websocket.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/Bismuth/worker.py` & `bitdust-0.1.7.233/bitdust_forks/Bismuth/worker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/__init__.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/database.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/database.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/database_gevent.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_gevent.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/database_safe_shared.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_safe_shared.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/database_super_thread_safe.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_super_thread_safe.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/database_thread_safe.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_thread_safe.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/debug_stuff.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/debug_stuff.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/env.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/env.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/hash_index.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/hash_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/index.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/indexcreator.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/indexcreator.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/lfu_cache.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/lfu_cache.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/lfu_cache_with_lock.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/lfu_cache_with_lock.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/migrate.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/migrate.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/misc.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/misc.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/patch.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/patch.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/rr_cache.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/rr_cache.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/rr_cache_with_lock.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/rr_cache_with_lock.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/sharded_hash.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/sharded_hash.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/sharded_index.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/sharded_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/storage.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/storage.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB/tree_index.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB/tree_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/__init__.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/database.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/database_gevent.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_gevent.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/database_safe_shared.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_safe_shared.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/database_super_thread_safe.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_super_thread_safe.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/database_thread_safe.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_thread_safe.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/debug_stuff.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/debug_stuff.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/env.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/env.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/hash_index.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/hash_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/index.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/indexcreator.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/indexcreator.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/lfu_cache.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/lfu_cache.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/lfu_cache_with_lock.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/lfu_cache_with_lock.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/migrate.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/migrate.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/misc.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/misc.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/patch.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/patch.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/rr_cache.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/rr_cache.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/rr_cache_with_lock.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/rr_cache_with_lock.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/sharded_hash.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/sharded_hash.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/sharded_index.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/sharded_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/storage.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/storage.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/CodernityDB3/tree_index.py` & `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/tree_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/__init__.py` & `bitdust-0.1.7.233/bitdust_forks/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/__init__.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/dtuple.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/dtuple.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/__init__.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/constants.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/constants.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/contact.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/contact.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/datastore.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/datastore.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/encoding.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/encoding.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/kbucket.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/kbucket.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/msgformat.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/msgformat.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/msgtypes.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/msgtypes.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/node.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/protocol.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/protocol.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/kademlia/routingtable.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/routingtable.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/entangled/node.py` & `bitdust-0.1.7.233/bitdust_forks/entangled/node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/parallelp/__init__.py` & `bitdust-0.1.7.233/bitdust_forks/parallelp/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/parallelp/pp/__init__.py` & `bitdust-0.1.7.233/bitdust_forks/parallelp/pp/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/parallelp/pp/ppauto.py` & `bitdust-0.1.7.233/bitdust_forks/parallelp/pp/ppauto.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/parallelp/pp/ppserver.py` & `bitdust-0.1.7.233/bitdust_forks/parallelp/pp/ppserver.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/parallelp/pp/pptransport.py` & `bitdust-0.1.7.233/bitdust_forks/parallelp/pp/pptransport.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/parallelp/pp/ppworker.py` & `bitdust-0.1.7.233/bitdust_forks/parallelp/pp/ppworker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/txrestapi/txrestapi/json_resource.py` & `bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/json_resource.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/txrestapi/txrestapi/methods.py` & `bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/methods.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/txrestapi/txrestapi/resource.py` & `bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/resource.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/txrestapi/txrestapi/tests.py` & `bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/tests.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/__init__.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/_abnf.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/_app.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/_cookiejar.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/_cookiejar.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/_core.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/_exceptions.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/_handshake.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/_http.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/_logging.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/_socket.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/_ssl_compat.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/_url.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/bitdust_forks/websocket/_utils.py` & `bitdust-0.1.7.233/bitdust_forks/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/scripts/bitdust` & `bitdust-0.1.7.233/scripts/bitdust`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/scripts/bitdust_worker` & `bitdust-0.1.7.233/scripts/bitdust_worker`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.6.231/setup.py` & `bitdust-0.1.7.233/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #
 # Please contact us if you have any questions at bitdust.io@gmail.com
 from __future__ import absolute_import
 from setuptools import setup
 
 setup(
     name='bitdust',
-    version='0.1.6.231',
+    version='0.1.7.233',
     author='Veselin Penev, BitDust',
     author_email='bitdust.io@gmail.com',
     maintainer='Veselin Penev, BitDust',
     maintainer_email='veselin@bitdust.io',
     url='https://bitdust.io',
     description='p2p secure distributed storage and communication engine',
     long_description=open('README.txt', 'r').read(),
```

