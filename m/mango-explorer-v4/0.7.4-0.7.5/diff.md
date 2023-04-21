# Comparing `tmp/mango_explorer_v4-0.7.4.tar.gz` & `tmp/mango_explorer_v4-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango_explorer_v4-0.7.4.tar", max compression
+gzip compressed data, was "mango_explorer_v4-0.7.5.tar", max compression
```

## Comparing `mango_explorer_v4-0.7.4.tar` & `mango_explorer_v4-0.7.5.tar`

### file list

```diff
@@ -1,167 +1,167 @@
--rw-r--r--   0        0        0     4953 2023-04-20 16:58:32.323371 mango_explorer_v4-0.7.4/README.md
--rw-r--r--   0        0        0        0 2023-03-28 18:28:14.167650 mango_explorer_v4-0.7.4/mango_explorer_v4/__init__.py
--rw-r--r--   0        0        0      554 2023-03-28 18:28:17.281077 mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/__init__.py
--rw-r--r--   0        0        0    16687 2023-03-28 18:28:17.406595 mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/bank.py
--rw-r--r--   0        0        0     4431 2023-03-28 18:28:17.687970 mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/book_side.py
--rw-r--r--   0        0        0     3535 2023-03-28 18:28:17.718250 mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/event_queue.py
--rw-r--r--   0        0        0     7560 2023-03-28 18:28:17.467721 mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/group.py
--rw-r--r--   0        0        0    10935 2023-04-16 05:06:36.568051 mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/mango_account.py
--rw-r--r--   0        0        0     4692 2023-03-28 18:28:17.620541 mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/mint_info.py
--rw-r--r--   0        0        0    17113 2023-03-28 18:28:17.848827 mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/perp_market.py
--rw-r--r--   0        0        0     5365 2023-03-28 18:28:17.931443 mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/serum3_market.py
--rw-r--r--   0        0        0     3300 2023-03-28 18:28:17.963516 mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/serum3_market_index_reservation.py
--rw-r--r--   0        0        0     3581 2023-03-28 18:28:17.650502 mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/stub_oracle.py
--rw-r--r--   0        0        0      246 2023-03-28 18:34:34.292405 mango_explorer_v4-0.7.4/mango_explorer_v4/constants.py
--rw-r--r--   0        0        0     6479 2023-04-15 00:21:51.949900 mango_explorer_v4-0.7.4/mango_explorer_v4/constructs/book_side_items.py
--rw-r--r--   0        0        0      167 2023-04-14 17:52:03.356866 mango_explorer_v4-0.7.4/mango_explorer_v4/constructs/serum3_reserved.py
--rw-r--r--   0        0        0      898 2023-03-28 18:28:14.175668 mango_explorer_v4-0.7.4/mango_explorer_v4/errors/__init__.py
--rw-r--r--   0        0        0    16298 2023-03-28 18:28:14.355123 mango_explorer_v4-0.7.4/mango_explorer_v4/errors/anchor.py
--rw-r--r--   0        0        0    14036 2023-03-28 18:28:14.277382 mango_explorer_v4-0.7.4/mango_explorer_v4/errors/custom.py
--rw-r--r--   0        0        0     1920 2023-04-20 15:32:44.142637 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/atomic_cancel_replace.py
--rw-r--r--   0        0        0      697 2023-04-20 15:31:27.015090 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/balances.py
--rw-r--r--   0        0        0     1032 2023-04-20 16:52:01.107323 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/cancel_all_orders.py
--rw-r--r--   0        0        0      518 2023-04-20 15:32:44.158502 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/equity.py
--rw-r--r--   0        0        0      564 2023-04-20 15:32:44.168217 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/fills.py
--rw-r--r--   0        0        0      422 2023-04-20 15:32:44.170198 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/funding_rate.py
--rw-r--r--   0        0        0      530 2023-04-20 15:32:44.150802 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/get_all_mango_accounts.py
--rw-r--r--   0        0        0      524 2023-04-20 15:32:44.172487 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/health_ratio.py
--rw-r--r--   0        0        0      587 2023-04-20 15:32:44.144683 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/incremental_fills.py
--rw-r--r--   0        0        0      571 2023-04-20 15:32:44.139058 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/incremental_orderbook_l2.py
--rw-r--r--   0        0        0     3131 2023-04-20 15:32:44.155377 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/market_maker.py
--rw-r--r--   0        0        0      493 2023-04-20 16:23:20.963674 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/orderbook_l2.py
--rw-r--r--   0        0        0     1309 2023-04-20 15:32:44.133923 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/place_order.py
--rw-r--r--   0        0        0     1419 2023-04-20 15:32:44.162483 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/place_perp_pegged_order.py
--rw-r--r--   0        0        0      175 2023-04-20 15:32:44.165157 mango_explorer_v4-0.7.4/mango_explorer_v4/examples/symbols.py
--rw-r--r--   0        0        0     1413 2023-04-10 21:52:09.976405 mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/bank.py
--rw-r--r--   0        0        0      466 2023-04-06 00:29:25.402431 mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/health_cache.py
--rw-r--r--   0        0        0      212 2023-04-03 18:14:47.577912 mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/i80f48.py
--rw-r--r--   0        0        0     1256 2023-04-13 20:59:03.364741 mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/mango_account.py
--rw-r--r--   0        0        0     2735 2023-04-14 23:04:00.006151 mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/perp_info.py
--rw-r--r--   0        0        0     1537 2023-04-04 23:44:46.310604 mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/perp_market.py
--rw-r--r--   0        0        0     4177 2023-04-15 15:05:04.789702 mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/perp_position.py
--rw-r--r--   0        0        0      794 2023-04-14 17:48:58.107793 mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/prices.py
--rw-r--r--   0        0        0     3205 2023-04-14 23:08:16.454262 mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/serum3_info.py
--rw-r--r--   0        0        0      194 2023-04-10 23:35:25.100335 mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/serum3_orders.py
--rw-r--r--   0        0        0     1684 2023-04-14 17:48:58.111335 mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/token_info.py
--rw-r--r--   0        0        0      637 2023-04-14 03:47:22.462530 mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/token_position.py
--rw-r--r--   0        0        0    14743 2023-04-14 23:52:07.526634 mango_explorer_v4-0.7.4/mango_explorer_v4/ids.json
--rw-r--r--   0        0        0     6531 2023-03-28 18:28:14.375260 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/__init__.py
--rw-r--r--   0        0        0     1930 2023-03-28 18:28:14.676966 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/account_buyback_fees_with_mngo.py
--rw-r--r--   0        0        0     1566 2023-03-28 18:28:14.661654 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/account_close.py
--rw-r--r--   0        0        0     2010 2023-03-28 18:28:14.608556 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/account_create.py
--rw-r--r--   0        0        0     1502 2023-03-28 18:28:14.637306 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/account_edit.py
--rw-r--r--   0        0        0     1835 2023-03-28 18:28:14.624285 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/account_expand.py
--rw-r--r--   0        0        0     1306 2023-03-28 18:28:14.648229 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/account_toggle_freeze.py
--rw-r--r--   0        0        0     1627 2023-03-28 18:28:15.474785 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/alt_extend.py
--rw-r--r--   0        0        0     1274 2023-03-28 18:28:15.460423 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/alt_set.py
--rw-r--r--   0        0        0      614 2023-03-28 18:28:15.489839 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/benchmark.py
--rw-r--r--   0        0        0      938 2023-03-28 18:28:15.483244 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/compute_account_data.py
--rw-r--r--   0        0        0     1538 2023-03-28 18:28:14.794315 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/flash_loan_begin.py
--rw-r--r--   0        0        0     1429 2023-03-28 18:28:14.804993 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/flash_loan_end.py
--rw-r--r--   0        0        0     1324 2023-03-28 18:28:14.443285 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/group_close.py
--rw-r--r--   0        0        0     2115 2023-03-28 18:28:14.399946 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/group_create.py
--rw-r--r--   0        0        0     3076 2023-03-28 18:28:14.421704 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/group_edit.py
--rw-r--r--   0        0        0     1077 2023-03-28 18:28:14.815212 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/health_region_begin.py
--rw-r--r--   0        0        0      829 2023-03-28 18:28:14.822399 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/health_region_end.py
--rw-r--r--   0        0        0     1151 2023-03-28 18:28:14.432548 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/ix_gate_set.py
--rw-r--r--   0        0        0     2055 2023-03-28 18:28:15.093469 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/liq_token_bankruptcy.py
--rw-r--r--   0        0        0     1776 2023-03-28 18:28:15.077328 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/liq_token_with_token.py
--rw-r--r--   0        0        0     1620 2023-03-28 18:28:15.333487 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_cancel_all_orders.py
--rw-r--r--   0        0        0     1944 2023-03-28 18:28:15.348888 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_cancel_all_orders_by_side.py
--rw-r--r--   0        0        0     1614 2023-03-28 18:28:15.305606 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_cancel_order.py
--rw-r--r--   0        0        0     1713 2023-03-28 18:28:15.319507 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_cancel_order_by_client_order_id.py
--rw-r--r--   0        0        0     1647 2023-03-28 18:28:15.217101 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_close_market.py
--rw-r--r--   0        0        0     1307 2023-03-28 18:28:15.360369 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_consume_events.py
--rw-r--r--   0        0        0     5504 2023-03-28 18:28:15.159726 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_create_market.py
--rw-r--r--   0        0        0     1180 2023-03-28 18:28:15.227828 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_deactivate_position.py
--rw-r--r--   0        0        0     6963 2023-03-28 18:28:15.203662 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_edit_market.py
--rw-r--r--   0        0        0     2232 2023-03-11 18:54:48.805388 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_liq_bankruptcy.py
--rw-r--r--   0        0        0     2198 2023-03-28 18:28:15.417269 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_liq_base_or_positive_pnl.py
--rw-r--r--   0        0        0     1684 2023-03-11 18:54:48.805559 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_liq_base_position.py
--rw-r--r--   0        0        0     1543 2023-03-28 18:28:15.430728 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_liq_force_cancel_orders.py
--rw-r--r--   0        0        0     2391 2023-03-28 18:28:15.449251 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_liq_negative_pnl_or_bankruptcy.py
--rw-r--r--   0        0        0     2780 2023-03-28 18:28:15.250130 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_place_order.py
--rw-r--r--   0        0        0     3085 2023-03-28 18:28:15.292058 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_place_order_pegged.py
--rw-r--r--   0        0        0     1701 2023-03-28 18:28:15.400012 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_settle_fees.py
--rw-r--r--   0        0        0     1770 2023-03-28 18:28:15.385969 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_settle_pnl.py
--rw-r--r--   0        0        0     1259 2023-03-28 18:28:15.371009 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_update_funding.py
--rw-r--r--   0        0        0     2255 2023-03-28 18:28:14.960915 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_cancel_all_orders.py
--rw-r--r--   0        0        0     2380 2023-03-28 18:28:14.942897 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_cancel_order.py
--rw-r--r--   0        0        0     1759 2023-03-28 18:28:14.893159 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_close_open_orders.py
--rw-r--r--   0        0        0     1971 2023-03-28 18:28:14.879402 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_create_open_orders.py
--rw-r--r--   0        0        0     1498 2023-03-28 18:28:14.864079 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_deregister_market.py
--rw-r--r--   0        0        0     1348 2023-03-28 18:28:14.851764 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_edit_market.py
--rw-r--r--   0        0        0     3200 2023-03-28 18:28:15.053755 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_liq_force_cancel_orders.py
--rw-r--r--   0        0        0     4442 2023-03-28 18:28:14.924805 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_place_order.py
--rw-r--r--   0        0        0     2319 2023-03-28 18:28:14.840620 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_register_market.py
--rw-r--r--   0        0        0     2625 2023-03-28 18:28:14.981269 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_settle_funds.py
--rw-r--r--   0        0        0     4061 2023-03-28 18:28:15.029678 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_settle_funds_v2.py
--rw-r--r--   0        0        0     1306 2023-03-28 18:28:14.702678 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/stub_oracle_close.py
--rw-r--r--   0        0        0     1682 2023-03-28 18:28:14.691197 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/stub_oracle_create.py
--rw-r--r--   0        0        0     1334 2023-03-28 18:28:14.713847 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/stub_oracle_set.py
--rw-r--r--   0        0        0     2319 2023-03-28 18:28:14.570011 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_add_bank.py
--rw-r--r--   0        0        0     2087 2023-03-28 18:28:14.749718 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_deposit.py
--rw-r--r--   0        0        0     2050 2023-03-28 18:28:14.766192 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_deposit_into_existing.py
--rw-r--r--   0        0        0     1423 2023-03-28 18:28:14.581550 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_deregister.py
--rw-r--r--   0        0        0     6232 2023-03-28 18:28:14.550748 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_edit.py
--rw-r--r--   0        0        0     2055 2023-03-28 18:28:15.123057 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_liq_bankruptcy.py
--rw-r--r--   0        0        0     1767 2023-03-28 18:28:15.107116 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_liq_with_token.py
--rw-r--r--   0        0        0     4198 2023-03-28 18:28:14.493969 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_register.py
--rw-r--r--   0        0        0     2309 2023-03-28 18:28:14.511980 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_register_trustless.py
--rw-r--r--   0        0        0     1212 2023-03-28 18:28:14.592362 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_update_index_and_rate.py
--rw-r--r--   0        0        0     1951 2023-03-28 18:28:14.781609 mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_withdraw.py
--rw-r--r--   0        0        0    60101 2023-04-20 17:11:14.302273 mango_explorer_v4-0.7.4/mango_explorer_v4/mango_client.py
--rw-r--r--   0        0        0     2088 2023-03-21 21:21:46.412623 mango_explorer_v4-0.7.4/mango_explorer_v4/oracles/pyth/__init__.py
--rw-r--r--   0        0        0      111 2023-03-28 18:28:14.169964 mango_explorer_v4-0.7.4/mango_explorer_v4/program_id.py
--rw-r--r--   0        0        0     4384 2023-03-28 18:28:15.506038 mango_explorer_v4-0.7.4/mango_explorer_v4/types/__init__.py
--rw-r--r--   0        0        0      940 2023-03-28 18:28:16.175465 mango_explorer_v4-0.7.4/mango_explorer_v4/types/any_event.py
--rw-r--r--   0        0        0      810 2023-03-28 18:28:16.072770 mango_explorer_v4-0.7.4/mango_explorer_v4/types/any_node.py
--rw-r--r--   0        0        0     1779 2023-03-28 18:28:16.921053 mango_explorer_v4-0.7.4/mango_explorer_v4/types/book_side_order_tree.py
--rw-r--r--   0        0        0     1916 2023-03-28 18:28:15.577643 mango_explorer_v4-0.7.4/mango_explorer_v4/types/equity.py
--rw-r--r--   0        0        0     1037 2023-03-28 18:28:16.159321 mango_explorer_v4-0.7.4/mango_explorer_v4/types/event_queue_header.py
--rw-r--r--   0        0        0     2192 2023-03-28 18:28:17.277076 mango_explorer_v4-0.7.4/mango_explorer_v4/types/event_type.py
--rw-r--r--   0        0        0     5576 2023-03-30 05:30:28.975854 mango_explorer_v4-0.7.4/mango_explorer_v4/types/fill_event.py
--rw-r--r--   0        0        0     2478 2023-03-28 18:28:15.773789 mango_explorer_v4-0.7.4/mango_explorer_v4/types/flash_loan_token_detail.py
--rw-r--r--   0        0        0     1669 2023-03-28 18:28:16.354508 mango_explorer_v4-0.7.4/mango_explorer_v4/types/flash_loan_type.py
--rw-r--r--   0        0        0     3215 2023-03-28 18:28:15.750874 mango_explorer_v4-0.7.4/mango_explorer_v4/types/health_cache.py
--rw-r--r--   0        0        0     2311 2023-03-28 18:28:16.477476 mango_explorer_v4-0.7.4/mango_explorer_v4/types/health_type.py
--rw-r--r--   0        0        0      968 2023-04-10 19:08:32.062957 mango_explorer_v4-0.7.4/mango_explorer_v4/types/i80f48.py
--rw-r--r--   0        0        0     2267 2023-03-28 18:28:16.025863 mango_explorer_v4-0.7.4/mango_explorer_v4/types/inner_node.py
--rw-r--r--   0        0        0     1990 2023-03-28 18:28:15.557136 mango_explorer_v4-0.7.4/mango_explorer_v4/types/interest_rate_params.py
--rw-r--r--   0        0        0    36314 2023-03-28 18:28:16.838780 mango_explorer_v4-0.7.4/mango_explorer_v4/types/ix_gate.py
--rw-r--r--   0        0        0     3669 2023-03-28 18:28:16.060268 mango_explorer_v4-0.7.4/mango_explorer_v4/types/leaf_node.py
--rw-r--r--   0        0        0     5704 2023-03-28 18:28:16.528320 mango_explorer_v4-0.7.4/mango_explorer_v4/types/loan_origination_fee_instruction.py
--rw-r--r--   0        0        0     5792 2023-03-28 18:28:15.974169 mango_explorer_v4-0.7.4/mango_explorer_v4/types/mango_account_fixed.py
--rw-r--r--   0        0        0     3639 2023-03-28 18:28:16.994291 mango_explorer_v4-0.7.4/mango_explorer_v4/types/node_tag.py
--rw-r--r--   0        0        0     1618 2023-03-28 18:28:15.991006 mango_explorer_v4-0.7.4/mango_explorer_v4/types/oracle_config.py
--rw-r--r--   0        0        0     1307 2023-03-28 18:28:16.003608 mango_explorer_v4-0.7.4/mango_explorer_v4/types/oracle_config_params.py
--rw-r--r--   0        0        0     2942 2023-03-28 18:28:16.873563 mango_explorer_v4-0.7.4/mango_explorer_v4/types/oracle_type.py
--rw-r--r--   0        0        0     6976 2023-03-28 18:28:17.168960 mango_explorer_v4-0.7.4/mango_explorer_v4/types/order_params.py
--rw-r--r--   0        0        0     2242 2023-03-28 18:28:16.900291 mango_explorer_v4-0.7.4/mango_explorer_v4/types/order_state.py
--rw-r--r--   0        0        0     2757 2023-03-28 18:28:16.144048 mango_explorer_v4-0.7.4/mango_explorer_v4/types/order_tree_nodes.py
--rw-r--r--   0        0        0      988 2023-03-28 18:28:16.086195 mango_explorer_v4-0.7.4/mango_explorer_v4/types/order_tree_root.py
--rw-r--r--   0        0        0     1624 2023-03-28 18:28:17.209042 mango_explorer_v4-0.7.4/mango_explorer_v4/types/order_tree_type.py
--rw-r--r--   0        0        0     2702 2023-03-28 18:28:16.255737 mango_explorer_v4-0.7.4/mango_explorer_v4/types/out_event.py
--rw-r--r--   0        0        0     1275 2023-03-28 18:28:15.603747 mango_explorer_v4-0.7.4/mango_explorer_v4/types/perp_equity.py
--rw-r--r--   0        0        0     6548 2023-03-28 18:28:15.721472 mango_explorer_v4-0.7.4/mango_explorer_v4/types/perp_info.py
--rw-r--r--   0        0        0      724 2023-03-28 18:28:16.322105 mango_explorer_v4-0.7.4/mango_explorer_v4/types/perp_market_index.py
--rw-r--r--   0        0        0     2209 2023-03-28 18:28:15.932238 mango_explorer_v4-0.7.4/mango_explorer_v4/types/perp_open_order.py
--rw-r--r--   0        0        0    10131 2023-03-28 18:28:15.907755 mango_explorer_v4-0.7.4/mango_explorer_v4/types/perp_position.py
--rw-r--r--   0        0        0     3665 2023-03-28 18:28:17.028677 mango_explorer_v4-0.7.4/mango_explorer_v4/types/place_order_type.py
--rw-r--r--   0        0        0     2371 2023-03-28 18:28:17.052275 mango_explorer_v4-0.7.4/mango_explorer_v4/types/post_order_type.py
--rw-r--r--   0        0        0     1219 2023-04-10 19:56:01.619718 mango_explorer_v4-0.7.4/mango_explorer_v4/types/prices.py
--rw-r--r--   0        0        0     2496 2023-03-28 18:28:15.674841 mango_explorer_v4-0.7.4/mango_explorer_v4/types/serum3_info.py
--rw-r--r--   0        0        0      736 2023-03-28 18:28:16.311360 mango_explorer_v4-0.7.4/mango_explorer_v4/types/serum3_market_index.py
--rw-r--r--   0        0        0     2441 2023-03-28 18:28:16.404196 mango_explorer_v4-0.7.4/mango_explorer_v4/types/serum3_order_type.py
--rw-r--r--   0        0        0     3158 2023-03-28 18:28:15.847071 mango_explorer_v4-0.7.4/mango_explorer_v4/types/serum3_orders.py
--rw-r--r--   0        0        0     2673 2023-03-28 18:28:16.378634 mango_explorer_v4-0.7.4/mango_explorer_v4/types/serum3_self_trade_behavior.py
--rw-r--r--   0        0        0     1579 2023-03-28 18:28:16.448940 mango_explorer_v4-0.7.4/mango_explorer_v4/types/serum3_side.py
--rw-r--r--   0        0        0     1549 2023-03-28 18:28:17.071688 mango_explorer_v4-0.7.4/mango_explorer_v4/types/side.py
--rw-r--r--   0        0        0     3164 2023-03-28 18:28:17.103353 mango_explorer_v4-0.7.4/mango_explorer_v4/types/side_and_order_tree.py
--rw-r--r--   0        0        0     4257 2023-03-28 18:28:16.288411 mango_explorer_v4-0.7.4/mango_explorer_v4/types/stable_price_model.py
--rw-r--r--   0        0        0     1119 2023-03-28 18:28:15.589905 mango_explorer_v4-0.7.4/mango_explorer_v4/types/token_equity.py
--rw-r--r--   0        0        0      694 2023-03-28 18:28:16.299159 mango_explorer_v4-0.7.4/mango_explorer_v4/types/token_index.py
--rw-r--r--   0        0        0     4482 2023-03-28 18:28:15.651474 mango_explorer_v4-0.7.4/mango_explorer_v4/types/token_info.py
--rw-r--r--   0        0        0     3327 2023-03-28 18:28:15.800167 mango_explorer_v4-0.7.4/mango_explorer_v4/types/token_position.py
--rw-r--r--   0        0        0     2008 2023-04-20 17:12:03.936822 mango_explorer_v4-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     8291 1970-01-01 00:00:00.000000 mango_explorer_v4-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     4862 2023-04-21 15:08:15.630944 mango_explorer_v4-0.7.5/README.md
+-rw-r--r--   0        0        0        0 2023-03-28 18:28:14.167650 mango_explorer_v4-0.7.5/mango_explorer_v4/__init__.py
+-rw-r--r--   0        0        0      554 2023-03-28 18:28:17.281077 mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/__init__.py
+-rw-r--r--   0        0        0    16687 2023-03-28 18:28:17.406595 mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/bank.py
+-rw-r--r--   0        0        0     4431 2023-03-28 18:28:17.687970 mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/book_side.py
+-rw-r--r--   0        0        0     3535 2023-03-28 18:28:17.718250 mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/event_queue.py
+-rw-r--r--   0        0        0     7560 2023-03-28 18:28:17.467721 mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/group.py
+-rw-r--r--   0        0        0    10935 2023-04-16 05:06:36.568051 mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/mango_account.py
+-rw-r--r--   0        0        0     4692 2023-03-28 18:28:17.620541 mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/mint_info.py
+-rw-r--r--   0        0        0    17113 2023-03-28 18:28:17.848827 mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/perp_market.py
+-rw-r--r--   0        0        0     5365 2023-03-28 18:28:17.931443 mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/serum3_market.py
+-rw-r--r--   0        0        0     3300 2023-03-28 18:28:17.963516 mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/serum3_market_index_reservation.py
+-rw-r--r--   0        0        0     3581 2023-03-28 18:28:17.650502 mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/stub_oracle.py
+-rw-r--r--   0        0        0      246 2023-03-28 18:34:34.292405 mango_explorer_v4-0.7.5/mango_explorer_v4/constants.py
+-rw-r--r--   0        0        0     6479 2023-04-15 00:21:51.949900 mango_explorer_v4-0.7.5/mango_explorer_v4/constructs/book_side_items.py
+-rw-r--r--   0        0        0      167 2023-04-14 17:52:03.356866 mango_explorer_v4-0.7.5/mango_explorer_v4/constructs/serum3_reserved.py
+-rw-r--r--   0        0        0      898 2023-03-28 18:28:14.175668 mango_explorer_v4-0.7.5/mango_explorer_v4/errors/__init__.py
+-rw-r--r--   0        0        0    16298 2023-03-28 18:28:14.355123 mango_explorer_v4-0.7.5/mango_explorer_v4/errors/anchor.py
+-rw-r--r--   0        0        0    14036 2023-03-28 18:28:14.277382 mango_explorer_v4-0.7.5/mango_explorer_v4/errors/custom.py
+-rw-r--r--   0        0        0     1920 2023-04-20 15:32:44.142637 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/atomic_cancel_replace.py
+-rw-r--r--   0        0        0      697 2023-04-20 15:31:27.015090 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/balances.py
+-rw-r--r--   0        0        0     1032 2023-04-20 16:52:01.107323 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/cancel_all_orders.py
+-rw-r--r--   0        0        0      518 2023-04-20 15:32:44.158502 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/equity.py
+-rw-r--r--   0        0        0      564 2023-04-20 15:32:44.168217 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/fills.py
+-rw-r--r--   0        0        0      422 2023-04-20 15:32:44.170198 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/funding_rate.py
+-rw-r--r--   0        0        0      530 2023-04-20 15:32:44.150802 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/get_all_mango_accounts.py
+-rw-r--r--   0        0        0      524 2023-04-20 15:32:44.172487 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/health_ratio.py
+-rw-r--r--   0        0        0      587 2023-04-20 15:32:44.144683 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/incremental_fills.py
+-rw-r--r--   0        0        0      571 2023-04-20 15:32:44.139058 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/incremental_orderbook_l2.py
+-rw-r--r--   0        0        0     3131 2023-04-20 15:32:44.155377 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/market_maker.py
+-rw-r--r--   0        0        0      493 2023-04-20 16:23:20.963674 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/orderbook_l2.py
+-rw-r--r--   0        0        0     1309 2023-04-20 15:32:44.133923 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/place_order.py
+-rw-r--r--   0        0        0     1419 2023-04-20 15:32:44.162483 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/place_perp_pegged_order.py
+-rw-r--r--   0        0        0      175 2023-04-20 15:32:44.165157 mango_explorer_v4-0.7.5/mango_explorer_v4/examples/symbols.py
+-rw-r--r--   0        0        0     1413 2023-04-10 21:52:09.976405 mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/bank.py
+-rw-r--r--   0        0        0      466 2023-04-06 00:29:25.402431 mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/health_cache.py
+-rw-r--r--   0        0        0      212 2023-04-03 18:14:47.577912 mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/i80f48.py
+-rw-r--r--   0        0        0     1256 2023-04-13 20:59:03.364741 mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/mango_account.py
+-rw-r--r--   0        0        0     2735 2023-04-14 23:04:00.006151 mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/perp_info.py
+-rw-r--r--   0        0        0     1537 2023-04-04 23:44:46.310604 mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/perp_market.py
+-rw-r--r--   0        0        0     4177 2023-04-15 15:05:04.789702 mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/perp_position.py
+-rw-r--r--   0        0        0      794 2023-04-14 17:48:58.107793 mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/prices.py
+-rw-r--r--   0        0        0     3205 2023-04-14 23:08:16.454262 mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/serum3_info.py
+-rw-r--r--   0        0        0      194 2023-04-10 23:35:25.100335 mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/serum3_orders.py
+-rw-r--r--   0        0        0     1684 2023-04-14 17:48:58.111335 mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/token_info.py
+-rw-r--r--   0        0        0      637 2023-04-14 03:47:22.462530 mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/token_position.py
+-rw-r--r--   0        0        0    14743 2023-04-14 23:52:07.526634 mango_explorer_v4-0.7.5/mango_explorer_v4/ids.json
+-rw-r--r--   0        0        0     6531 2023-03-28 18:28:14.375260 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/__init__.py
+-rw-r--r--   0        0        0     1930 2023-03-28 18:28:14.676966 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/account_buyback_fees_with_mngo.py
+-rw-r--r--   0        0        0     1566 2023-03-28 18:28:14.661654 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/account_close.py
+-rw-r--r--   0        0        0     2010 2023-03-28 18:28:14.608556 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/account_create.py
+-rw-r--r--   0        0        0     1502 2023-03-28 18:28:14.637306 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/account_edit.py
+-rw-r--r--   0        0        0     1835 2023-03-28 18:28:14.624285 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/account_expand.py
+-rw-r--r--   0        0        0     1306 2023-03-28 18:28:14.648229 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/account_toggle_freeze.py
+-rw-r--r--   0        0        0     1627 2023-03-28 18:28:15.474785 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/alt_extend.py
+-rw-r--r--   0        0        0     1274 2023-03-28 18:28:15.460423 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/alt_set.py
+-rw-r--r--   0        0        0      614 2023-03-28 18:28:15.489839 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/benchmark.py
+-rw-r--r--   0        0        0      938 2023-03-28 18:28:15.483244 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/compute_account_data.py
+-rw-r--r--   0        0        0     1538 2023-03-28 18:28:14.794315 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/flash_loan_begin.py
+-rw-r--r--   0        0        0     1429 2023-03-28 18:28:14.804993 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/flash_loan_end.py
+-rw-r--r--   0        0        0     1324 2023-03-28 18:28:14.443285 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/group_close.py
+-rw-r--r--   0        0        0     2115 2023-03-28 18:28:14.399946 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/group_create.py
+-rw-r--r--   0        0        0     3076 2023-03-28 18:28:14.421704 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/group_edit.py
+-rw-r--r--   0        0        0     1077 2023-03-28 18:28:14.815212 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/health_region_begin.py
+-rw-r--r--   0        0        0      829 2023-03-28 18:28:14.822399 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/health_region_end.py
+-rw-r--r--   0        0        0     1151 2023-03-28 18:28:14.432548 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/ix_gate_set.py
+-rw-r--r--   0        0        0     2055 2023-03-28 18:28:15.093469 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/liq_token_bankruptcy.py
+-rw-r--r--   0        0        0     1776 2023-03-28 18:28:15.077328 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/liq_token_with_token.py
+-rw-r--r--   0        0        0     1620 2023-03-28 18:28:15.333487 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_cancel_all_orders.py
+-rw-r--r--   0        0        0     1944 2023-03-28 18:28:15.348888 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_cancel_all_orders_by_side.py
+-rw-r--r--   0        0        0     1614 2023-03-28 18:28:15.305606 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_cancel_order.py
+-rw-r--r--   0        0        0     1713 2023-03-28 18:28:15.319507 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_cancel_order_by_client_order_id.py
+-rw-r--r--   0        0        0     1647 2023-03-28 18:28:15.217101 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_close_market.py
+-rw-r--r--   0        0        0     1307 2023-03-28 18:28:15.360369 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_consume_events.py
+-rw-r--r--   0        0        0     5504 2023-03-28 18:28:15.159726 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_create_market.py
+-rw-r--r--   0        0        0     1180 2023-03-28 18:28:15.227828 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_deactivate_position.py
+-rw-r--r--   0        0        0     6963 2023-03-28 18:28:15.203662 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_edit_market.py
+-rw-r--r--   0        0        0     2232 2023-03-11 18:54:48.805388 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_liq_bankruptcy.py
+-rw-r--r--   0        0        0     2198 2023-03-28 18:28:15.417269 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_liq_base_or_positive_pnl.py
+-rw-r--r--   0        0        0     1684 2023-03-11 18:54:48.805559 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_liq_base_position.py
+-rw-r--r--   0        0        0     1543 2023-03-28 18:28:15.430728 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_liq_force_cancel_orders.py
+-rw-r--r--   0        0        0     2391 2023-03-28 18:28:15.449251 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_liq_negative_pnl_or_bankruptcy.py
+-rw-r--r--   0        0        0     2780 2023-03-28 18:28:15.250130 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_place_order.py
+-rw-r--r--   0        0        0     3085 2023-03-28 18:28:15.292058 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_place_order_pegged.py
+-rw-r--r--   0        0        0     1701 2023-03-28 18:28:15.400012 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_settle_fees.py
+-rw-r--r--   0        0        0     1770 2023-03-28 18:28:15.385969 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_settle_pnl.py
+-rw-r--r--   0        0        0     1259 2023-03-28 18:28:15.371009 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_update_funding.py
+-rw-r--r--   0        0        0     2255 2023-03-28 18:28:14.960915 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_cancel_all_orders.py
+-rw-r--r--   0        0        0     2380 2023-03-28 18:28:14.942897 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_cancel_order.py
+-rw-r--r--   0        0        0     1759 2023-03-28 18:28:14.893159 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_close_open_orders.py
+-rw-r--r--   0        0        0     1971 2023-03-28 18:28:14.879402 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_create_open_orders.py
+-rw-r--r--   0        0        0     1498 2023-03-28 18:28:14.864079 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_deregister_market.py
+-rw-r--r--   0        0        0     1348 2023-03-28 18:28:14.851764 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_edit_market.py
+-rw-r--r--   0        0        0     3200 2023-03-28 18:28:15.053755 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_liq_force_cancel_orders.py
+-rw-r--r--   0        0        0     4442 2023-03-28 18:28:14.924805 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_place_order.py
+-rw-r--r--   0        0        0     2319 2023-03-28 18:28:14.840620 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_register_market.py
+-rw-r--r--   0        0        0     2625 2023-03-28 18:28:14.981269 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_settle_funds.py
+-rw-r--r--   0        0        0     4061 2023-03-28 18:28:15.029678 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_settle_funds_v2.py
+-rw-r--r--   0        0        0     1306 2023-03-28 18:28:14.702678 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/stub_oracle_close.py
+-rw-r--r--   0        0        0     1682 2023-03-28 18:28:14.691197 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/stub_oracle_create.py
+-rw-r--r--   0        0        0     1334 2023-03-28 18:28:14.713847 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/stub_oracle_set.py
+-rw-r--r--   0        0        0     2319 2023-03-28 18:28:14.570011 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_add_bank.py
+-rw-r--r--   0        0        0     2087 2023-03-28 18:28:14.749718 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_deposit.py
+-rw-r--r--   0        0        0     2050 2023-03-28 18:28:14.766192 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_deposit_into_existing.py
+-rw-r--r--   0        0        0     1423 2023-03-28 18:28:14.581550 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_deregister.py
+-rw-r--r--   0        0        0     6232 2023-03-28 18:28:14.550748 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_edit.py
+-rw-r--r--   0        0        0     2055 2023-03-28 18:28:15.123057 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_liq_bankruptcy.py
+-rw-r--r--   0        0        0     1767 2023-03-28 18:28:15.107116 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_liq_with_token.py
+-rw-r--r--   0        0        0     4198 2023-03-28 18:28:14.493969 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_register.py
+-rw-r--r--   0        0        0     2309 2023-03-28 18:28:14.511980 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_register_trustless.py
+-rw-r--r--   0        0        0     1212 2023-03-28 18:28:14.592362 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_update_index_and_rate.py
+-rw-r--r--   0        0        0     1951 2023-03-28 18:28:14.781609 mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_withdraw.py
+-rw-r--r--   0        0        0    59963 2023-04-21 17:36:46.535930 mango_explorer_v4-0.7.5/mango_explorer_v4/mango_client.py
+-rw-r--r--   0        0        0     2088 2023-03-21 21:21:46.412623 mango_explorer_v4-0.7.5/mango_explorer_v4/oracles/pyth/__init__.py
+-rw-r--r--   0        0        0      111 2023-03-28 18:28:14.169964 mango_explorer_v4-0.7.5/mango_explorer_v4/program_id.py
+-rw-r--r--   0        0        0     4384 2023-03-28 18:28:15.506038 mango_explorer_v4-0.7.5/mango_explorer_v4/types/__init__.py
+-rw-r--r--   0        0        0      940 2023-03-28 18:28:16.175465 mango_explorer_v4-0.7.5/mango_explorer_v4/types/any_event.py
+-rw-r--r--   0        0        0      810 2023-03-28 18:28:16.072770 mango_explorer_v4-0.7.5/mango_explorer_v4/types/any_node.py
+-rw-r--r--   0        0        0     1779 2023-03-28 18:28:16.921053 mango_explorer_v4-0.7.5/mango_explorer_v4/types/book_side_order_tree.py
+-rw-r--r--   0        0        0     1916 2023-03-28 18:28:15.577643 mango_explorer_v4-0.7.5/mango_explorer_v4/types/equity.py
+-rw-r--r--   0        0        0     1037 2023-03-28 18:28:16.159321 mango_explorer_v4-0.7.5/mango_explorer_v4/types/event_queue_header.py
+-rw-r--r--   0        0        0     2192 2023-03-28 18:28:17.277076 mango_explorer_v4-0.7.5/mango_explorer_v4/types/event_type.py
+-rw-r--r--   0        0        0     5576 2023-03-30 05:30:28.975854 mango_explorer_v4-0.7.5/mango_explorer_v4/types/fill_event.py
+-rw-r--r--   0        0        0     2478 2023-03-28 18:28:15.773789 mango_explorer_v4-0.7.5/mango_explorer_v4/types/flash_loan_token_detail.py
+-rw-r--r--   0        0        0     1669 2023-03-28 18:28:16.354508 mango_explorer_v4-0.7.5/mango_explorer_v4/types/flash_loan_type.py
+-rw-r--r--   0        0        0     3215 2023-03-28 18:28:15.750874 mango_explorer_v4-0.7.5/mango_explorer_v4/types/health_cache.py
+-rw-r--r--   0        0        0     2311 2023-03-28 18:28:16.477476 mango_explorer_v4-0.7.5/mango_explorer_v4/types/health_type.py
+-rw-r--r--   0        0        0      968 2023-04-10 19:08:32.062957 mango_explorer_v4-0.7.5/mango_explorer_v4/types/i80f48.py
+-rw-r--r--   0        0        0     2267 2023-03-28 18:28:16.025863 mango_explorer_v4-0.7.5/mango_explorer_v4/types/inner_node.py
+-rw-r--r--   0        0        0     1990 2023-03-28 18:28:15.557136 mango_explorer_v4-0.7.5/mango_explorer_v4/types/interest_rate_params.py
+-rw-r--r--   0        0        0    36314 2023-03-28 18:28:16.838780 mango_explorer_v4-0.7.5/mango_explorer_v4/types/ix_gate.py
+-rw-r--r--   0        0        0     3669 2023-03-28 18:28:16.060268 mango_explorer_v4-0.7.5/mango_explorer_v4/types/leaf_node.py
+-rw-r--r--   0        0        0     5704 2023-03-28 18:28:16.528320 mango_explorer_v4-0.7.5/mango_explorer_v4/types/loan_origination_fee_instruction.py
+-rw-r--r--   0        0        0     5792 2023-03-28 18:28:15.974169 mango_explorer_v4-0.7.5/mango_explorer_v4/types/mango_account_fixed.py
+-rw-r--r--   0        0        0     3639 2023-03-28 18:28:16.994291 mango_explorer_v4-0.7.5/mango_explorer_v4/types/node_tag.py
+-rw-r--r--   0        0        0     1618 2023-03-28 18:28:15.991006 mango_explorer_v4-0.7.5/mango_explorer_v4/types/oracle_config.py
+-rw-r--r--   0        0        0     1307 2023-03-28 18:28:16.003608 mango_explorer_v4-0.7.5/mango_explorer_v4/types/oracle_config_params.py
+-rw-r--r--   0        0        0     2942 2023-03-28 18:28:16.873563 mango_explorer_v4-0.7.5/mango_explorer_v4/types/oracle_type.py
+-rw-r--r--   0        0        0     6976 2023-03-28 18:28:17.168960 mango_explorer_v4-0.7.5/mango_explorer_v4/types/order_params.py
+-rw-r--r--   0        0        0     2242 2023-03-28 18:28:16.900291 mango_explorer_v4-0.7.5/mango_explorer_v4/types/order_state.py
+-rw-r--r--   0        0        0     2757 2023-03-28 18:28:16.144048 mango_explorer_v4-0.7.5/mango_explorer_v4/types/order_tree_nodes.py
+-rw-r--r--   0        0        0      988 2023-03-28 18:28:16.086195 mango_explorer_v4-0.7.5/mango_explorer_v4/types/order_tree_root.py
+-rw-r--r--   0        0        0     1624 2023-03-28 18:28:17.209042 mango_explorer_v4-0.7.5/mango_explorer_v4/types/order_tree_type.py
+-rw-r--r--   0        0        0     2702 2023-03-28 18:28:16.255737 mango_explorer_v4-0.7.5/mango_explorer_v4/types/out_event.py
+-rw-r--r--   0        0        0     1275 2023-03-28 18:28:15.603747 mango_explorer_v4-0.7.5/mango_explorer_v4/types/perp_equity.py
+-rw-r--r--   0        0        0     6548 2023-03-28 18:28:15.721472 mango_explorer_v4-0.7.5/mango_explorer_v4/types/perp_info.py
+-rw-r--r--   0        0        0      724 2023-03-28 18:28:16.322105 mango_explorer_v4-0.7.5/mango_explorer_v4/types/perp_market_index.py
+-rw-r--r--   0        0        0     2209 2023-03-28 18:28:15.932238 mango_explorer_v4-0.7.5/mango_explorer_v4/types/perp_open_order.py
+-rw-r--r--   0        0        0    10131 2023-03-28 18:28:15.907755 mango_explorer_v4-0.7.5/mango_explorer_v4/types/perp_position.py
+-rw-r--r--   0        0        0     3665 2023-03-28 18:28:17.028677 mango_explorer_v4-0.7.5/mango_explorer_v4/types/place_order_type.py
+-rw-r--r--   0        0        0     2371 2023-03-28 18:28:17.052275 mango_explorer_v4-0.7.5/mango_explorer_v4/types/post_order_type.py
+-rw-r--r--   0        0        0     1219 2023-04-10 19:56:01.619718 mango_explorer_v4-0.7.5/mango_explorer_v4/types/prices.py
+-rw-r--r--   0        0        0     2496 2023-03-28 18:28:15.674841 mango_explorer_v4-0.7.5/mango_explorer_v4/types/serum3_info.py
+-rw-r--r--   0        0        0      736 2023-03-28 18:28:16.311360 mango_explorer_v4-0.7.5/mango_explorer_v4/types/serum3_market_index.py
+-rw-r--r--   0        0        0     2441 2023-03-28 18:28:16.404196 mango_explorer_v4-0.7.5/mango_explorer_v4/types/serum3_order_type.py
+-rw-r--r--   0        0        0     3158 2023-03-28 18:28:15.847071 mango_explorer_v4-0.7.5/mango_explorer_v4/types/serum3_orders.py
+-rw-r--r--   0        0        0     2673 2023-03-28 18:28:16.378634 mango_explorer_v4-0.7.5/mango_explorer_v4/types/serum3_self_trade_behavior.py
+-rw-r--r--   0        0        0     1579 2023-03-28 18:28:16.448940 mango_explorer_v4-0.7.5/mango_explorer_v4/types/serum3_side.py
+-rw-r--r--   0        0        0     1549 2023-03-28 18:28:17.071688 mango_explorer_v4-0.7.5/mango_explorer_v4/types/side.py
+-rw-r--r--   0        0        0     3164 2023-03-28 18:28:17.103353 mango_explorer_v4-0.7.5/mango_explorer_v4/types/side_and_order_tree.py
+-rw-r--r--   0        0        0     4257 2023-03-28 18:28:16.288411 mango_explorer_v4-0.7.5/mango_explorer_v4/types/stable_price_model.py
+-rw-r--r--   0        0        0     1119 2023-03-28 18:28:15.589905 mango_explorer_v4-0.7.5/mango_explorer_v4/types/token_equity.py
+-rw-r--r--   0        0        0      694 2023-03-28 18:28:16.299159 mango_explorer_v4-0.7.5/mango_explorer_v4/types/token_index.py
+-rw-r--r--   0        0        0     4482 2023-03-28 18:28:15.651474 mango_explorer_v4-0.7.5/mango_explorer_v4/types/token_info.py
+-rw-r--r--   0        0        0     3327 2023-03-28 18:28:15.800167 mango_explorer_v4-0.7.5/mango_explorer_v4/types/token_position.py
+-rw-r--r--   0        0        0     2008 2023-04-21 17:37:12.476453 mango_explorer_v4-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     8200 1970-01-01 00:00:00.000000 mango_explorer_v4-0.7.5/PKG-INFO
```

### Comparing `mango_explorer_v4-0.7.4/README.md` & `mango_explorer_v4-0.7.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -97,32 +97,30 @@
 # ]
 ```
 
 Examples may take arguments, which are specified in their source files. The [equity function](https://github.com/blockworks-foundation/mango-explorer-v4/blob/master/mango_explorer_v4/examples/equity.py) for example, takes a Mango account primary key, whilst the [order book retrieval](https://github.com/blockworks-foundation/mango-explorer-v4/blob/master/mango_explorer_v4/examples/orderbook_l2.py) takes a symbol & (optional) depth. These can be specified in the shell like this:
 
 ```shell
 python -m mango_explorer_v4.examples.equity --mango-account 9XJt2tvSZghsMAhWto1VuPBrwXsiimPtsTR8XwGgDxK2
-# Output the Account Balance at https://app.mango.markets/?address=9XJt2tvSZghsMAhWto1VuPBrwXsiimPtsTR8XwGgDxK2
+# Outputs the Account Balance at https://app.mango.markets/?address=9XJt2tvSZghsMAhWto1VuPBrwXsiimPtsTR8XwGgDxK2
 
 python -m mango_explorer_v4.examples.orderbook_l2 --symbol SOL-PERP --depth 5
 # Outputs the first 5 orders in the book at https://app.mango.markets/trade?name=SOL-PERP
 ```
 
 Some transactions, like order placement, require a keypair. On [Phantom wallet](https://phantom.app/) it can be fetched as follows:
 
 https://user-images.githubusercontent.com/28162761/233431861-5db448c1-fdf9-4dd0-8df9-156b131dfd71.mov
 
 With the keypair at hand you can place orders using:
 
 ```shell
 python -m mango_explorer_v4.examples.place_order \
     --keypair [KEYPAIR] \
-    # ^ Replace with your keypair
     --mango-account [MANGO_ACCOUNT] \
-    # ^ Replace with a Mango account owned by the keypair
     --symbol SOL-PERP \
     --side bids \
     --price 1 \
     --size 0.1
 ```
 
 And cancel them later as:
```

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/__init__.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/bank.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/bank.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/book_side.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/book_side.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/event_queue.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/event_queue.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/group.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/group.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/mango_account.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/mango_account.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/mint_info.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/mint_info.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/perp_market.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/perp_market.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/serum3_market.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/serum3_market.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/serum3_market_index_reservation.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/serum3_market_index_reservation.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/accounts/stub_oracle.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/accounts/stub_oracle.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/constructs/book_side_items.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/constructs/book_side_items.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/errors/__init__.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/errors/anchor.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/errors/anchor.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/errors/custom.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/errors/custom.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/examples/atomic_cancel_replace.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/examples/atomic_cancel_replace.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/examples/balances.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/examples/balances.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/examples/cancel_all_orders.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/examples/cancel_all_orders.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/examples/equity.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/examples/equity.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/examples/fills.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/examples/fills.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/examples/get_all_mango_accounts.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/examples/get_all_mango_accounts.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/examples/health_ratio.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/examples/health_ratio.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/examples/incremental_fills.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/examples/incremental_fills.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/examples/incremental_orderbook_l2.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/examples/incremental_orderbook_l2.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/examples/market_maker.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/examples/market_maker.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/examples/place_order.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/examples/place_order.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/examples/place_perp_pegged_order.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/examples/place_perp_pegged_order.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/bank.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/bank.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/mango_account.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/mango_account.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/perp_info.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/perp_info.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/perp_market.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/perp_market.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/perp_position.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/perp_position.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/prices.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/prices.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/serum3_info.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/serum3_info.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/token_info.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/token_info.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/helpers/token_position.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/helpers/token_position.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/ids.json` & `mango_explorer_v4-0.7.5/mango_explorer_v4/ids.json`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/__init__.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/account_buyback_fees_with_mngo.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/account_buyback_fees_with_mngo.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/account_close.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/account_close.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/account_create.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/account_create.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/account_edit.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/account_edit.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/account_expand.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/account_expand.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/account_toggle_freeze.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/account_toggle_freeze.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/alt_extend.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/alt_extend.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/alt_set.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/alt_set.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/benchmark.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/benchmark.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/compute_account_data.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/compute_account_data.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/flash_loan_begin.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/flash_loan_begin.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/flash_loan_end.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/flash_loan_end.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/group_close.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/group_close.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/group_create.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/group_create.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/group_edit.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/group_edit.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/health_region_begin.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/health_region_begin.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/health_region_end.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/health_region_end.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/ix_gate_set.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/ix_gate_set.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/liq_token_bankruptcy.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/liq_token_bankruptcy.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/liq_token_with_token.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/liq_token_with_token.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_cancel_all_orders.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_cancel_all_orders.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_cancel_all_orders_by_side.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_cancel_all_orders_by_side.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_cancel_order.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_cancel_order.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_cancel_order_by_client_order_id.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_cancel_order_by_client_order_id.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_close_market.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_close_market.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_consume_events.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_consume_events.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_create_market.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_create_market.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_deactivate_position.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_deactivate_position.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_edit_market.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_edit_market.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_liq_bankruptcy.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_liq_bankruptcy.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_liq_base_or_positive_pnl.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_liq_base_or_positive_pnl.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_liq_base_position.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_liq_base_position.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_liq_force_cancel_orders.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_liq_force_cancel_orders.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_liq_negative_pnl_or_bankruptcy.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_liq_negative_pnl_or_bankruptcy.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_place_order.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_place_order.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_place_order_pegged.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_place_order_pegged.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_settle_fees.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_settle_fees.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_settle_pnl.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_settle_pnl.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/perp_update_funding.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/perp_update_funding.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_cancel_all_orders.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_cancel_all_orders.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_cancel_order.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_cancel_order.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_close_open_orders.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_close_open_orders.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_create_open_orders.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_create_open_orders.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_deregister_market.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_deregister_market.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_edit_market.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_edit_market.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_liq_force_cancel_orders.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_liq_force_cancel_orders.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_place_order.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_place_order.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_register_market.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_register_market.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_settle_funds.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_settle_funds.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/serum3_settle_funds_v2.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/serum3_settle_funds_v2.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/stub_oracle_close.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/stub_oracle_close.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/stub_oracle_create.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/stub_oracle_create.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/stub_oracle_set.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/stub_oracle_set.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_add_bank.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_add_bank.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_deposit.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_deposit.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_deposit_into_existing.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_deposit_into_existing.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_deregister.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_deregister.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_edit.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_edit.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_liq_bankruptcy.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_liq_bankruptcy.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_liq_with_token.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_liq_with_token.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_register.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_register.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_register_trustless.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_register_trustless.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_update_index_and_rate.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_update_index_and_rate.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/instructions/token_withdraw.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/instructions/token_withdraw.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/mango_client.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/mango_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -559,46 +559,44 @@
     ) -> [AccountMeta]:
         health_remaining_account_pks = []
 
         match retriever:
             case 'fixed':
                 token_indices = [token.token_index for token in mango_account.tokens]
 
-                if len(banks) > 0:
-                    for bank in banks:
-                        if bank.token_index not in token_indices:
-                            index = [
-                                idx for idx, token in enumerate(mango_account.tokens)
-                                if token.token_index == 65535
-                                if token_indices[idx] == 65535
-                            ][0]
+                for bank in banks:
+                    if bank.token_index not in token_indices:
+                        index = [
+                            idx for idx, token in enumerate(mango_account.tokens)
+                            if token.token_index == 65535
+                            if token_indices[idx] == 65535
+                        ][0]
 
-                            token_indices[index] = bank.token_index
+                        token_indices[index] = bank.token_index
 
                 mint_infos = [
-                    mint_info for mint_info in self.mint_infos
-                    if mint_info.token_index in [token_index for token_index in token_indices if token_index != 65535]
+                    [mint_info for mint_info in self.mint_infos if mint_info.token_index == token_index][0]
+                    for token_index in token_indices if token_index != 65535
                 ]
 
                 health_remaining_account_pks.extend([mint_info.banks[0] for mint_info in mint_infos])
 
                 health_remaining_account_pks.extend([mint_info.oracle for mint_info in mint_infos])
 
                 perp_market_indices = [perp.market_index for perp in mango_account.perps]
 
-                if len(perp_markets) > 0:
-                    for perp_market in perp_markets:
-                        if perp_market.perp_market_index not in perp_market_indices:
-                            index = [
-                                idx for idx, perp in enumerate(mango_account.perps)
-                                if perp.market_index == 65535
-                                if perp_market_indices[idx] == 65535
-                            ][0] = perp_market.perp_market_index
+                for perp_market in perp_markets:
+                    if perp_market.perp_market_index not in perp_market_indices:
+                        index = [
+                            idx for idx, perp in enumerate(mango_account.perps)
+                            if perp.market_index == 65535
+                            if perp_market_indices[idx] == 65535
+                        ][0] = perp_market.perp_market_index
 
-                            perp_market_indices[index] = perp_market.perp_market_index
+                        perp_market_indices[index] = perp_market.perp_market_index
 
                 perp_markets = [
                     perp_market for perp_market in self.perp_markets
                     if perp_market.perp_market_index in [perp_index for perp_index in perp_market_indices if perp_index != 65535]
                 ]
 
                 perp_market_pks = [
```

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/oracles/pyth/__init__.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/oracles/pyth/__init__.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/__init__.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/any_event.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/any_event.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/any_node.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/any_node.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/book_side_order_tree.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/book_side_order_tree.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/equity.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/equity.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/event_queue_header.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/event_queue_header.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/event_type.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/event_type.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/fill_event.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/fill_event.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/flash_loan_token_detail.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/flash_loan_token_detail.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/flash_loan_type.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/flash_loan_type.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/health_cache.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/health_cache.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/health_type.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/health_type.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/i80f48.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/i80f48.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/inner_node.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/inner_node.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/interest_rate_params.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/interest_rate_params.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/ix_gate.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/ix_gate.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/leaf_node.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/leaf_node.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/loan_origination_fee_instruction.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/loan_origination_fee_instruction.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/mango_account_fixed.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/mango_account_fixed.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/node_tag.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/node_tag.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/oracle_config.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/oracle_config.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/oracle_config_params.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/oracle_config_params.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/oracle_type.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/oracle_type.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/order_params.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/order_params.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/order_state.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/order_state.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/order_tree_nodes.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/order_tree_nodes.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/order_tree_root.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/order_tree_root.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/order_tree_type.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/order_tree_type.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/out_event.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/out_event.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/perp_equity.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/perp_equity.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/perp_info.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/perp_info.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/perp_market_index.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/perp_market_index.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/perp_open_order.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/perp_open_order.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/perp_position.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/perp_position.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/place_order_type.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/place_order_type.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/post_order_type.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/post_order_type.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/prices.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/prices.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/serum3_info.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/serum3_info.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/serum3_market_index.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/serum3_market_index.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/serum3_order_type.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/serum3_order_type.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/serum3_orders.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/serum3_orders.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/serum3_self_trade_behavior.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/serum3_self_trade_behavior.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/serum3_side.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/serum3_side.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/side.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/side.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/side_and_order_tree.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/side_and_order_tree.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/stable_price_model.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/stable_price_model.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/token_equity.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/token_equity.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/token_index.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/token_index.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/token_info.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/token_info.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/mango_explorer_v4/types/token_position.py` & `mango_explorer_v4-0.7.5/mango_explorer_v4/types/token_position.py`

 * *Files identical despite different names*

### Comparing `mango_explorer_v4-0.7.4/pyproject.toml` & `mango_explorer_v4-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mango-explorer-v4"
-version = "0.7.4"
+version = "0.7.5"
 description = ""
 authors = ["waterquarks <waterquarks@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "mango_explorer_v4" }
 ]
```

### Comparing `mango_explorer_v4-0.7.4/PKG-INFO` & `mango_explorer_v4-0.7.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-explorer-v4
-Version: 0.7.4
+Version: 0.7.5
 Summary: 
 Author: waterquarks
 Author-email: waterquarks@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -193,32 +193,30 @@
 # ]
 ```
 
 Examples may take arguments, which are specified in their source files. The [equity function](https://github.com/blockworks-foundation/mango-explorer-v4/blob/master/mango_explorer_v4/examples/equity.py) for example, takes a Mango account primary key, whilst the [order book retrieval](https://github.com/blockworks-foundation/mango-explorer-v4/blob/master/mango_explorer_v4/examples/orderbook_l2.py) takes a symbol & (optional) depth. These can be specified in the shell like this:
 
 ```shell
 python -m mango_explorer_v4.examples.equity --mango-account 9XJt2tvSZghsMAhWto1VuPBrwXsiimPtsTR8XwGgDxK2
-# Output the Account Balance at https://app.mango.markets/?address=9XJt2tvSZghsMAhWto1VuPBrwXsiimPtsTR8XwGgDxK2
+# Outputs the Account Balance at https://app.mango.markets/?address=9XJt2tvSZghsMAhWto1VuPBrwXsiimPtsTR8XwGgDxK2
 
 python -m mango_explorer_v4.examples.orderbook_l2 --symbol SOL-PERP --depth 5
 # Outputs the first 5 orders in the book at https://app.mango.markets/trade?name=SOL-PERP
 ```
 
 Some transactions, like order placement, require a keypair. On [Phantom wallet](https://phantom.app/) it can be fetched as follows:
 
 https://user-images.githubusercontent.com/28162761/233431861-5db448c1-fdf9-4dd0-8df9-156b131dfd71.mov
 
 With the keypair at hand you can place orders using:
 
 ```shell
 python -m mango_explorer_v4.examples.place_order \
     --keypair [KEYPAIR] \
-    # ^ Replace with your keypair
     --mango-account [MANGO_ACCOUNT] \
-    # ^ Replace with a Mango account owned by the keypair
     --symbol SOL-PERP \
     --side bids \
     --price 1 \
     --size 0.1
 ```
 
 And cancel them later as:
```

