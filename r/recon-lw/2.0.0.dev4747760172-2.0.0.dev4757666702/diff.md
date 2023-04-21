# Comparing `tmp/recon_lw-2.0.0.dev4747760172.tar.gz` & `tmp/recon_lw-2.0.0.dev4757666702.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4747760172.tar", last modified: Wed Apr 19 20:46:22 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4757666702.tar", last modified: Fri Apr 21 06:18:15 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4747760172.tar` & `recon_lw-2.0.0.dev4757666702.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:46:22.000000 recon_lw-2.0.0.dev4747760172/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-19 20:46:03.000000 recon_lw-2.0.0.dev4747760172/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-19 20:46:22.000000 recon_lw-2.0.0.dev4747760172/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-19 20:46:03.000000 recon_lw-2.0.0.dev4747760172/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-19 20:46:10.000000 recon_lw-2.0.0.dev4747760172/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:46:22.000000 recon_lw-2.0.0.dev4747760172/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-04-19 20:46:03.000000 recon_lw-2.0.0.dev4747760172/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-19 20:46:03.000000 recon_lw-2.0.0.dev4747760172/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-19 20:46:03.000000 recon_lw-2.0.0.dev4747760172/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    16442 2023-04-19 20:46:03.000000 recon_lw-2.0.0.dev4747760172/recon_lw/recon_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:46:22.000000 recon_lw-2.0.0.dev4747760172/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-19 20:46:22.000000 recon_lw-2.0.0.dev4747760172/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-19 20:46:22.000000 recon_lw-2.0.0.dev4747760172/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 20:46:22.000000 recon_lw-2.0.0.dev4747760172/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-19 20:46:22.000000 recon_lw-2.0.0.dev4747760172/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-19 20:46:22.000000 recon_lw-2.0.0.dev4747760172/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-19 20:46:03.000000 recon_lw-2.0.0.dev4747760172/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 20:46:22.000000 recon_lw-2.0.0.dev4747760172/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-19 20:46:03.000000 recon_lw-2.0.0.dev4747760172/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-21 06:17:57.000000 recon_lw-2.0.0.dev4757666702/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19652 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/recon_lw/recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/setup.py
```

### Comparing `recon_lw-2.0.0.dev4747760172/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4757666702/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4747760172/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4757666702/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4747760172/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4757666702/recon_lw/recon_ob.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 def flush_sequence_clear_cache(processed_len, sequence_cache):
     sequence = sequence_cache["sequence"]
     for i in range(0, processed_len):
         sequence.pop(0)
 
 
 def process_market_data_update(mess, events,  books_cache, get_book_id_func ,update_book_rule,
-                               check_book_rule, event_sequence, parent_event, initial_book_params):
+                               check_book_rule, event_sequence, parent_event, initial_book_params, log_books_filter):
     book_id, result = get_book_id_func(mess)
     if result is not None:
         book_id_event = recon_lw.create_event("GetBookEroor:" + parent_event["eventName"], "GetBookEroor", event_sequence,
                                               ok=False,
                                               body=result,
                                               parentId=parent_event["eventId"])
         book_id_event["attachedMessageIds"] = [mess["messageId"]]
@@ -84,57 +84,75 @@
         if operations is None:
             return
         
         for operation, parameters in operations:
             initial_book = copy.deepcopy(book)
             initial_parameters = copy.copy(parameters)
             parameters["order_book"] = book
-            result = operation(**parameters)
+            result, log_entries = operation(**parameters)
             if len(result) > 0:
                 result["operation"] = operation.__name__
                 result["operation_params"] = initial_parameters
                 result["initial_book"] = initial_book
                 result["book_id"] = book_id
                 update_event = recon_lw.create_event("UpdateBookError:" + parent_event["eventName"], "UpdateBookError",
                                                      event_sequence,
                                                      ok=False,
                                                      body=result,
                                                      parentId=parent_event["eventId"])
                 update_event["attachedMessageIds"] = [mess["messageId"]]
                 events.append(update_event)
+            if log_entries is not None:
+                for log_book in log_entries:
+                    log_book["sessionId"] = mess["sessionId"]
+                    log_book["book_id"] = book_id
+                    log_book["operation"] = operation.__name__
+                    log_book["operation_params"] = initial_parameters
+                    if log_books_filter is not None and log_books_filter(log_book):
+                        log_event = recon_lw.create_event("OrderBook:" + mess["sessionId"],
+                                                          "OrderBook",
+                                                          event_sequence,
+                                                          ok=True,
+                                                          body=log_book,
+                                                          parentId=parent_event["eventId"])
+                        log_event["attachedMessageIds"] = [mess["messageId"]]
+                        events.append(log_event)
+
             results = check_book_rule(book, event_sequence)
             if results is not None:
                 for r in results:
                     if not r["successful"]:
                         r["body"]["operation_params"] = initial_parameters
                         r["body"]["initial_book"] = initial_book
                     r["body"]["operation"] = operation.__name__
                     r["body"]["book_id"] = book_id
                     r["parentEventId"] = parent_event["eventId"]
                     r["attachedMessageIds"] = [mess["messageId"]]
                     events.append(r)
 
 
 def process_ob_rules(sequenced_batch, books_cache, get_book_id_func ,update_book_rule,
-                     check_book_rule, event_sequence, send_events_func, parent_event, initial_book_params):
+                     check_book_rule, event_sequence, send_events_func, parent_event, initial_book_params,
+                     log_books_filter):
     events = []
     n_processed = 0
     for m in sequenced_batch:
         seq = m[0]
         mess = m[1]
         #process gaps
         if "gap" in mess:
             gap_event = recon_lw.create_event("SeqGap:" + parent_event["eventName"],"SeqGap",event_sequence,ok=False,
                                               body={"seq_num": seq} ,parentId=parent_event["eventId"])
             events.append(gap_event)
             continue
         chunk = message_utils.expand_message(mess)
         for m_upd in chunk:
             process_market_data_update(m_upd, events, books_cache, get_book_id_func, update_book_rule,
-                                       check_book_rule, event_sequence, parent_event, initial_book_params)
+                                       check_book_rule, event_sequence, parent_event, initial_book_params,
+                                       log_books_filter)
         n_processed += 1
 
     send_events_func(events)
     return n_processed
 
 
 def init_ob_stream(rule_settings):
@@ -162,15 +180,16 @@
                                    rule_settings["books_cache"],
                                    rule_settings["get_book_id"],
                                    rule_settings["update_book_rule"],
                                    rule_settings["check_book_rule"],
                                    event_sequence,
                                    save_events_func,
                                    rule_settings["rule_root_event"],
-                                   rule_settings["initial_book_params"])
+                                   rule_settings["initial_book_params"],
+                                   rule_settings["log_books_filter"] if "log_books_filter" in rule_settings else None)
     ## Process duplicated
     duplicates = rule_settings["sequence_cache"]["duplicates"]
     n_dupl = len(duplicates)
     dupl_events = []
     for i in range(0,n_dupl):
         item = duplicates.pop(0)
         d_ev = recon_lw.create_event("Duplicate:" + rule_settings["rule_root_event"]["eventName"],"Duplicate",
@@ -202,119 +221,135 @@
 
 def ob_add_order(order_id, price, size, side, order_book):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
 
     if find_order_position(order_id, order_book)[0] is not None:
-        return {"error": order_id + " already exists"}
+        return {"error": order_id + " already exists"}, []
     if price not in order_book[side]:
         order_book[side][price] = {order_id: size}
     else:
         order_book[side][price][order_id] = size
 
     reflect_price_update_in_version(side, price, order_book)
-    return {}
+    return {}, [copy.deepcopy(order_book)]
 
 
 def ob_update_order(order_id, price, size, order_book):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
 
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     if old_side is None:
-        return {"error": order_id + " not found"}
+        return {"error": order_id + " not found"}, []
 
+    log = []
     if price == old_price:
         order_book[old_side][old_price][order_id] = size
         reflect_price_update_in_version(old_side, old_price, order_book)
+        log.append(copy.deepcopy(order_book))
     else:
         # should no get here but will monitor
         reflect_price_update_in_version(old_side, old_price, order_book)
         order_book[old_side][old_price].pop(order_id)
         if len(order_book[old_side][old_price]) == 0:
             order_book[old_side].pop(old_price)
+        log.append(copy.deepcopy(order_book))
         if price not in order_book[old_side]:
             order_book[old_side][price] = {}
         order_book[old_side][price][order_id] = size
         reflect_price_update_in_version(old_side, price, order_book)
+        log.append(copy.deepcopy(order_book))
 
-    return {}
+    return {}, log
 
 
 def ob_delete_order(order_id, order_book):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
 
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     if old_side is None:
-        return {"error": order_id + " not found"}
+        return {"error": order_id + " not found"}, []
 
+    log = []
     reflect_price_update_in_version(old_side, old_price, order_book)
     order_book[old_side][old_price].pop(order_id)
     if len(order_book[old_side][old_price]) == 0:
         order_book[old_side].pop(old_price)
+        log.append(copy.deepcopy(order_book))
         max_levels = order_book["aggr_max_levels"]
         if len(order_book[old_side]) >= max_levels and order_book["aggr_seq"]["limit_delta"] == 1:
             #back from horizon update
             order_book["aggr_seq"]["limit_delta"] = 2
             order_book["aggr_seq"]["limit_v"] += 1
+            log.append(copy.deepcopy(order_book))
+    else:
+        log.append(copy.deepcopy(order_book))
 
-    return {}
+    return {}, log
 
 
 def ob_trade_order(order_id, traded_size ,order_book):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     old_side, old_price, old_size = find_order_position(order_id, order_book)
+    log = []
     if old_side is None:
-        return {"error": order_id + " not found"}
+        return {"error": order_id + " not found"}, []
     if traded_size > old_size:
-        return {"error": "traded size > resting size"}
+        return {"error": "traded size > resting size"}, []
     elif traded_size == old_size:
         reflect_price_update_in_version(old_side, old_price, order_book)
         order_book[old_side][old_price].pop(order_id)
         if len(order_book[old_side][old_price]) == 0:
             order_book[old_side].pop(old_price)
+            log.append(copy.deepcopy(order_book))
+            max_levels = order_book["aggr_max_levels"]
             if len(order_book[old_side]) >= max_levels and order_book["aggr_seq"]["limit_delta"] == 1:
                 # back from horizon update
                 order_book["aggr_seq"]["limit_delta"] = 2
                 order_book["aggr_seq"]["limit_v"] += 1
+                log.append(copy.deepcopy(order_book))
+        else:
+            log.append(copy.deepcopy(order_book))
     else:
         reflect_price_update_in_version(old_side, old_price, order_book)
         order_book[old_side][old_price][order_id] -= traded_size
-    return {}
+        log.append(copy.deepcopy(order_book))
+    return {}, log
 
 
 def ob_clean_book(order_book):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     for side_key in ["ask", "bid"]:
         if side_key in order_book:
             order_book[side_key].clear()
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     order_book["aggr_seq"]["top_delta"] = 1
     order_book["aggr_seq"]["top_v"] += 1
-    return {}
+    return {}, [copy.deepcopy(order_book)]
 
 
 def ob_change_status(new_status, order_book):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["status"] = new_status
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     order_book["aggr_seq"]["top_delta"] = 1
     order_book["aggr_seq"]["top_v"] += 1
-    return {}
+    return {}, [copy.deepcopy(order_book)]
 
 
 def find_order_position(order_id, order_book):
     for side in ["ask", "bid"]:
         for pr,orders in order_book[side].items():
             if order_id in orders:
                 return side, pr, orders[order_id]
@@ -327,76 +362,101 @@
         return -1
     levels = list(order_book[side].keys())
     levels.sort()
     return levels.index(p)+1 if side == "ask" else len(levels)-levels.index(p)
 
 
 def ob_aggr_add_level(side, level, price, real_qty, real_num_orders, impl_qty, impl_num_orders, order_book):
+    if "aggr_seq" not in order_book:
+        init_aggr_seq(order_book)
+    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side+"_aggr"
     new_index = level - 1
     if not 0 <= new_index <= len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
-        return result_body
+        return result_body,[]
 
     new_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders, "impl_qty": impl_qty,
                  "impl_num_orders": impl_num_orders}
     order_book[side_key].insert(new_index, new_level)
     if len(order_book[side_key]) == max_levels+1:
         order_book[side_key].pop()
+    order_book["aggr_seq"]["limit_delta"] = 1
+    order_book["aggr_seq"]["limit_v"] += 1
 
-    return {}
+    return {}, [copy.deepcopy(order_book)]
 
 
 def ob_aggr_delete_level(side, level, order_book):
+    if "aggr_seq" not in order_book:
+        init_aggr_seq(order_book)
+    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     result_body = {}
     side_key = side+"_aggr"
     del_index = level - 1
     if not 0 <= del_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
-        return result_body
+        return result_body, []
 
     order_book[side_key].pop(del_index)
 
-    return {}
+    order_book["aggr_seq"]["limit_delta"] = 1
+    order_book["aggr_seq"]["limit_v"] += 1
+    return {}, [copy.deepcopy(order_book)]
 
 
 def ob_aggr_update_level(side, level, price, real_qty, real_num_orders, impl_qty, impl_num_orders, order_book):
+    if "aggr_seq" not in order_book:
+        init_aggr_seq(order_book)
+    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side+"_aggr"
     update_index = level - 1
     if not 0 <= update_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
-        return result_body
+        return result_body, []
 
     upd_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders, 
                  "impl_qty" : impl_qty, "impl_num_orders": impl_num_orders}
     order_book[side_key][update_index].update(upd_level)
+    order_book["aggr_seq"]["limit_delta"] = 1
+    order_book["aggr_seq"]["limit_v"] += 1
 
-    return {}
+    return {}, [copy.deepcopy(order_book)]
 
 
 def ob_aggr_clean_book(order_book):
+    if "aggr_seq" not in order_book:
+        init_aggr_seq(order_book)
+    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     for side_key in ["ask_aggr", "bid_aggr"]:
         if side_key in order_book:
             order_book[side_key].clear()
-    return {}
+    order_book["aggr_seq"]["limit_delta"] = 1
+    order_book["aggr_seq"]["limit_v"] += 1
+    return {}, [copy.deepcopy(order_book)]
 
 
 def ob_top_update(ask_price, ask_real_qty, ask_impl_qty, ask_real_n_orders, ask_impl_n_orders,
                   bid_price, bid_real_qty, bid_impl_qty, bid_real_n_orders, bid_impl_n_orders,
                   order_book):
+    if "aggr_seq" not in order_book:
+        init_aggr_seq(order_book)
     order_book["ask_price"] = ask_price
     order_book["ask_real_qty"] = ask_real_qty
     order_book["ask_impl_qty"] = ask_impl_qty
     order_book["ask_real_n_orders"] = ask_real_n_orders
     order_book["ask_impl_n_orders"] = ask_impl_n_orders
     order_book["bid_price"] = bid_price
     order_book["bid_real_qty"] = bid_real_qty
     order_book["bid_impl_qty"] = bid_impl_qty
     order_book["bid_real_n_orders"] = bid_real_n_orders
     order_book["bid_impl_n_orders"] = bid_impl_n_orders
 
-    return {}
+    order_book["aggr_seq"]["top_delta"] = 1
+    order_book["aggr_seq"]["top_v"] += 1
+
+    return {}, [copy.deepcopy(order_book)]
```

### Comparing `recon_lw-2.0.0.dev4747760172/setup.py` & `recon_lw-2.0.0.dev4757666702/setup.py`

 * *Files identical despite different names*

