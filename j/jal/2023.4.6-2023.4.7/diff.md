# Comparing `tmp/jal-2023.4.6.tar.gz` & `tmp/jal-2023.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jal-2023.4.6.tar", last modified: Sat Apr 15 14:24:53 2023, max compression
+gzip compressed data, was "jal-2023.4.7.tar", last modified: Fri Apr 21 18:29:44 2023, max compression
```

## Comparing `jal-2023.4.6.tar` & `jal-2023.4.7.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.986407 jal-2023.4.6/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      176 2022-01-13 06:08:45.000000 jal-2023.4.6/MANIFEST.in
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-15 14:24:53.986407 jal-2023.4.6/PKG-INFO
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.943073 jal-2023.4.6/docs/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7580 2023-04-15 14:23:01.000000 jal-2023.4.6/docs/README.md
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.949740 jal-2023.4.6/jal/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       24 2023-04-15 14:19:23.000000 jal-2023.4.6/jal/__init__.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3831 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/constants.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.949740 jal-2023.4.6/jal/data_export/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2022-01-13 15:45:51.000000 jal-2023.4.6/jal/data_export/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19856 2023-04-14 11:26:23.000000 jal-2023.4.6/jal/data_export/dlsg.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.953073 jal-2023.4.6/jal/data_export/tax_reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/data_export/tax_reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      990 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/data_export/tax_reports/portugal.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7089 2023-02-08 10:00:47.000000 jal-2023.4.6/jal/data_export/tax_reports/portugal.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1532 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/data_export/tax_reports/russia.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    38366 2023-04-14 11:26:23.000000 jal-2023.4.6/jal/data_export/tax_reports/russia.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6433 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/data_export/taxes.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5299 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/data_export/taxes_flow.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.956406 jal-2023.4.6/jal/data_export/templates/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-30 08:37:57.000000 jal-2023.4.6/jal/data_export/templates/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1286 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/data_export/templates/tax_prt_dividends.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2594 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/data_export/templates/tax_prt_shares.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6163 2022-01-30 08:37:57.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_bonds.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4792 2022-02-13 11:04:18.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_corporate_actions.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4938 2022-04-30 20:05:13.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_crypto.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4948 2022-04-30 20:05:13.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_derivatives.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3249 2022-02-13 11:04:18.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_dividends.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1450 2022-01-30 08:37:57.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_fees.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1133 2022-06-19 17:39:33.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_flow.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1654 2022-07-20 07:00:10.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_interests.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5303 2022-01-30 08:37:57.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_trades.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10842 2023-02-08 13:35:53.000000 jal-2023.4.6/jal/data_export/xlsx.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.956406 jal-2023.4.6/jal/data_import/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/data_import/__init__.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.959740 jal-2023.4.6/jal/data_import/broker_statements/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-22 16:32:16.000000 jal-2023.4.6/jal/data_import/broker_statements/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    63265 2023-04-14 11:26:23.000000 jal-2023.4.6/jal/data_import/broker_statements/ibkr.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19903 2022-08-21 07:15:06.000000 jal-2023.4.6/jal/data_import/broker_statements/just2trade.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9470 2022-08-21 07:15:06.000000 jal-2023.4.6/jal/data_import/broker_statements/kit.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5857 2023-02-14 12:14:19.000000 jal-2023.4.6/jal/data_import/broker_statements/open_portfolio.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    30709 2023-02-14 12:16:51.000000 jal-2023.4.6/jal/data_import/broker_statements/openbroker.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15460 2022-12-07 21:59:21.000000 jal-2023.4.6/jal/data_import/broker_statements/psb.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    27469 2022-08-21 07:15:06.000000 jal-2023.4.6/jal/data_import/broker_statements/uralsib.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3893 2023-03-05 19:06:08.000000 jal-2023.4.6/jal/data_import/category_recognizer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      543 2021-08-05 15:24:10.000000 jal-2023.4.6/jal/data_import/import_schema.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15598 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/data_import/slips.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13145 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/data_import/slips_tax.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35649 2023-04-14 11:26:23.000000 jal-2023.4.6/jal/data_import/statement.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11314 2023-02-02 08:45:14.000000 jal-2023.4.6/jal/data_import/statement_xls.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6950 2023-04-14 11:26:23.000000 jal-2023.4.6/jal/data_import/statement_xml.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3224 2023-04-08 19:50:05.000000 jal-2023.4.6/jal/data_import/statements.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.959740 jal-2023.4.6/jal/db/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/db/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17607 2023-02-27 16:25:45.000000 jal-2023.4.6/jal/db/account.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21487 2023-04-14 11:26:23.000000 jal-2023.4.6/jal/db/asset.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     6074 2022-12-06 18:30:39.000000 jal-2023.4.6/jal/db/backup_restore.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7360 2023-02-27 17:48:37.000000 jal-2023.4.6/jal/db/balances_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4103 2023-02-27 16:03:46.000000 jal-2023.4.6/jal/db/category.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5218 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/db/closed_trade.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2399 2023-03-08 17:11:23.000000 jal-2023.4.6/jal/db/country.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    18652 2023-04-15 13:39:15.000000 jal-2023.4.6/jal/db/db.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3941 2023-04-12 09:44:25.000000 jal-2023.4.6/jal/db/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15989 2023-04-14 11:27:05.000000 jal-2023.4.6/jal/db/holdings_model.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    16683 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/db/ledger.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    60565 2023-04-07 14:10:37.000000 jal-2023.4.6/jal/db/operations.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7475 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/db/operations_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3379 2023-02-20 16:05:40.000000 jal-2023.4.6/jal/db/peer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15204 2023-04-15 13:54:08.000000 jal-2023.4.6/jal/db/reference_models.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1190 2023-01-06 21:49:49.000000 jal-2023.4.6/jal/db/settings.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      438 2023-02-16 17:12:29.000000 jal-2023.4.6/jal/db/tag.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6777 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/db/tax_estimator.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1458 2023-02-23 19:54:06.000000 jal-2023.4.6/jal/db/view_model.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.963073 jal-2023.4.6/jal/img/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2922 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/accept.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1443 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/add.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2049 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/add_child.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      435 2022-04-25 10:26:48.000000 jal-2023.4.6/jal/img/broom.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4004 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/cancel.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      806 2023-03-08 16:58:09.000000 jal-2023.4.6/jal/img/chart.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      898 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/copy.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2812 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/delete.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      583 2021-03-20 12:52:05.000000 jal-2023.4.6/jal/img/ibkr.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2340 2022-04-29 07:05:21.000000 jal-2023.4.6/jal/img/j2t.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5563 2022-01-13 06:08:45.000000 jal-2023.4.6/jal/img/jal.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1516 2021-03-22 11:20:31.000000 jal-2023.4.6/jal/img/kit.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1163 2022-12-28 10:47:37.000000 jal-2023.4.6/jal/img/list.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      342 2022-04-25 10:26:48.000000 jal-2023.4.6/jal/img/meatballs.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      611 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/new.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1175 2022-07-10 15:39:56.000000 jal-2023.4.6/jal/img/open_portfolio.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15086 2021-08-05 15:24:10.000000 jal-2023.4.6/jal/img/openbroker.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-08-05 15:24:10.000000 jal-2023.4.6/jal/img/psb.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-03-20 12:52:05.000000 jal-2023.4.6/jal/img/quik.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2651 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/reconcile.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      822 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/remove.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1874 2023-03-08 16:53:42.000000 jal-2023.4.6/jal/img/tax.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1406 2021-03-20 12:52:05.000000 jal-2023.4.6/jal/img/uralsib.ico
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     1938 2023-01-19 12:05:21.000000 jal-2023.4.6/jal/jal.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    91499 2023-04-07 14:10:37.000000 jal-2023.4.6/jal/jal_init.sql
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.966406 jal-2023.4.6/jal/languages/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      424 2020-12-21 16:23:10.000000 jal-2023.4.6/jal/languages/en.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    32025 2022-01-13 06:08:45.000000 jal-2023.4.6/jal/languages/en.qm
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      287 2022-04-25 10:26:48.000000 jal-2023.4.6/jal/languages/ru.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    87568 2023-04-15 14:17:53.000000 jal-2023.4.6/jal/languages/ru.qm
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.966406 jal-2023.4.6/jal/net/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2021-08-17 15:15:47.000000 jal-2023.4.6/jal/net/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    24656 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/net/downloader.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2912 2023-01-27 21:53:46.000000 jal-2023.4.6/jal/net/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2040 2023-03-06 11:34:17.000000 jal-2023.4.6/jal/pypi_description.md
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.966406 jal-2023.4.6/jal/reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2967 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/category.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14386 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/deals.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3936 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/holdings.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14756 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/income_spending.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2855 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/peer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8771 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/profit_loss.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3287 2023-02-16 10:22:14.000000 jal-2023.4.6/jal/reports/reports.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2827 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/tag.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.966406 jal-2023.4.6/jal/ui/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/ui/__init__.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.969740 jal-2023.4.6/jal/ui/reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-13 15:45:51.000000 jal-2023.4.6/jal/ui/reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5179 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_category_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4099 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_deals_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4159 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_holdings_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4156 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_income_spending_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5382 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_peer_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4687 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_profit_loss_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5353 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_tag_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4805 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_tax_estimation.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12742 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_asset_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4056 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_flow_export_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14782 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_login_fns_dlg.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     9324 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_main_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14510 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_operations_widget.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     5707 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_rebuild_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7302 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_reference_data_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2903 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_select_account_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3253 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_select_reference_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16301 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_slip_import_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9674 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_tax_export_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4023 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_update_quotes_window.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.983073 jal-2023.4.6/jal/updates/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/updates/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5122 2020-12-21 16:23:10.000000 jal-2023.4.6/jal/updates/jal_delta_10.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12870 2021-08-18 12:53:40.000000 jal-2023.4.6/jal/updates/jal_delta_11.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26116 2021-01-13 17:04:46.000000 jal-2023.4.6/jal/updates/jal_delta_12.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16516 2021-01-30 16:01:43.000000 jal-2023.4.6/jal/updates/jal_delta_13.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    34961 2021-02-27 17:35:02.000000 jal-2023.4.6/jal/updates/jal_delta_14.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2250 2021-02-27 17:35:02.000000 jal-2023.4.6/jal/updates/jal_delta_15.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3630 2021-02-27 17:35:02.000000 jal-2023.4.6/jal/updates/jal_delta_16.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20912 2021-02-27 17:35:02.000000 jal-2023.4.6/jal/updates/jal_delta_17.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      656 2021-03-07 11:58:53.000000 jal-2023.4.6/jal/updates/jal_delta_18.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      686 2021-03-08 13:39:11.000000 jal-2023.4.6/jal/updates/jal_delta_19.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13578 2021-03-12 14:26:01.000000 jal-2023.4.6/jal/updates/jal_delta_20.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1428 2021-03-19 12:24:53.000000 jal-2023.4.6/jal/updates/jal_delta_21.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      949 2021-03-22 11:20:31.000000 jal-2023.4.6/jal/updates/jal_delta_22.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17602 2021-04-08 12:12:36.000000 jal-2023.4.6/jal/updates/jal_delta_23.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      344 2021-04-11 10:57:46.000000 jal-2023.4.6/jal/updates/jal_delta_24.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8270 2021-04-22 04:11:28.000000 jal-2023.4.6/jal/updates/jal_delta_25.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2492 2021-08-12 19:15:12.000000 jal-2023.4.6/jal/updates/jal_delta_26.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26325 2022-01-13 05:57:31.000000 jal-2023.4.6/jal/updates/jal_delta_27.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13276 2022-01-13 06:08:45.000000 jal-2023.4.6/jal/updates/jal_delta_28.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35370 2022-01-13 15:45:51.000000 jal-2023.4.6/jal/updates/jal_delta_29.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8671 2022-02-13 13:11:58.000000 jal-2023.4.6/jal/updates/jal_delta_30.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11413 2022-02-13 11:04:18.000000 jal-2023.4.6/jal/updates/jal_delta_31.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12545 2022-03-31 14:26:11.000000 jal-2023.4.6/jal/updates/jal_delta_32.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4229 2022-03-31 14:26:11.000000 jal-2023.4.6/jal/updates/jal_delta_33.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2287 2022-04-06 14:47:21.000000 jal-2023.4.6/jal/updates/jal_delta_34.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2858 2022-04-30 20:05:13.000000 jal-2023.4.6/jal/updates/jal_delta_35.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3427 2022-06-19 17:39:33.000000 jal-2023.4.6/jal/updates/jal_delta_36.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3755 2022-07-20 07:00:10.000000 jal-2023.4.6/jal/updates/jal_delta_37.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21913 2022-08-21 07:15:06.000000 jal-2023.4.6/jal/updates/jal_delta_38.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      343 2023-01-04 13:14:35.000000 jal-2023.4.6/jal/updates/jal_delta_39.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3055 2023-01-27 21:53:46.000000 jal-2023.4.6/jal/updates/jal_delta_40.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    48157 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/updates/jal_delta_41.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2085 2023-02-20 14:55:36.000000 jal-2023.4.6/jal/updates/jal_delta_42.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2528 2023-03-08 16:23:30.000000 jal-2023.4.6/jal/updates/jal_delta_43.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3020 2023-04-07 14:10:37.000000 jal-2023.4.6/jal/updates/jal_delta_44.sql
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.986407 jal-2023.4.6/jal/widgets/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/widgets/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3912 2023-04-15 09:01:12.000000 jal-2023.4.6/jal/widgets/abstract_operation_details.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6846 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/account_select.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14491 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/asset_dialog.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11302 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/corporate_action_widget.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.986407 jal-2023.4.6/jal/widgets/custom/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-12-24 19:32:40.000000 jal-2023.4.6/jal/widgets/custom/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4441 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/custom/date_range_selector.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2015 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/custom/db_lookup_combobox.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5331 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/widgets/custom/log_viewer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13628 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/delegates.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9289 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/dividend_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8437 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/widgets/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12488 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/income_spending_widget.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    13018 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/widgets/main_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3386 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/mdi.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2854 2022-12-26 13:26:40.000000 jal-2023.4.6/jal/widgets/operations_tabs.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7159 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/widgets/operations_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6013 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/price_chart.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5667 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/qr_scanner.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11244 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/widgets/reference_data.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21856 2023-04-15 13:54:08.000000 jal-2023.4.6/jal/widgets/reference_dialogs.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4779 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/reference_selector.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      632 2022-12-26 08:54:07.000000 jal-2023.4.6/jal/widgets/register_designer_plugins.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3499 2023-04-15 14:14:41.000000 jal-2023.4.6/jal/widgets/selection_dialog.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7862 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/widgets/tax_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6890 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/trade_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10088 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/transfer_widget.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.949740 jal-2023.4.6/jal.egg-info/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-15 14:24:53.000000 jal-2023.4.6/jal.egg-info/PKG-INFO
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5592 2023-04-15 14:24:53.000000 jal-2023.4.6/jal.egg-info/SOURCES.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        1 2023-04-15 14:24:53.000000 jal-2023.4.6/jal.egg-info/dependency_links.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       37 2023-04-15 14:24:53.000000 jal-2023.4.6/jal.egg-info/entry_points.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       67 2023-04-15 14:24:53.000000 jal-2023.4.6/jal.egg-info/requires.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       10 2023-04-15 14:24:53.000000 jal-2023.4.6/jal.egg-info/top_level.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       38 2023-04-15 14:24:53.986407 jal-2023.4.6/setup.cfg
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1756 2023-04-14 18:14:21.000000 jal-2023.4.6/setup.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.020457 jal-2023.4.7/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      176 2022-01-13 06:08:45.000000 jal-2023.4.7/MANIFEST.in
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-21 18:29:44.020457 jal-2023.4.7/PKG-INFO
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.977123 jal-2023.4.7/docs/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7580 2023-04-15 14:23:01.000000 jal-2023.4.7/docs/README.md
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.980456 jal-2023.4.7/jal/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       24 2023-04-21 18:26:09.000000 jal-2023.4.7/jal/__init__.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3831 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/constants.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.980456 jal-2023.4.7/jal/data_export/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2022-01-13 15:45:51.000000 jal-2023.4.7/jal/data_export/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19856 2023-04-14 11:26:23.000000 jal-2023.4.7/jal/data_export/dlsg.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.983790 jal-2023.4.7/jal/data_export/tax_reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/data_export/tax_reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      990 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/data_export/tax_reports/portugal.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7089 2023-02-08 10:00:47.000000 jal-2023.4.7/jal/data_export/tax_reports/portugal.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1532 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/data_export/tax_reports/russia.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    38366 2023-04-14 11:26:23.000000 jal-2023.4.7/jal/data_export/tax_reports/russia.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6433 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/data_export/taxes.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5299 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/data_export/taxes_flow.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.983790 jal-2023.4.7/jal/data_export/templates/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-30 08:37:57.000000 jal-2023.4.7/jal/data_export/templates/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1286 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/data_export/templates/tax_prt_dividends.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2594 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/data_export/templates/tax_prt_shares.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6163 2022-01-30 08:37:57.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_bonds.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4792 2022-02-13 11:04:18.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_corporate_actions.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4938 2022-04-30 20:05:13.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_crypto.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4948 2022-04-30 20:05:13.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_derivatives.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3249 2022-02-13 11:04:18.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_dividends.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1450 2022-01-30 08:37:57.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_fees.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1133 2022-06-19 17:39:33.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_flow.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1654 2022-07-20 07:00:10.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_interests.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5303 2022-01-30 08:37:57.000000 jal-2023.4.7/jal/data_export/templates/tax_rus_trades.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10842 2023-02-08 13:35:53.000000 jal-2023.4.7/jal/data_export/xlsx.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.987123 jal-2023.4.7/jal/data_import/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/data_import/__init__.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.987123 jal-2023.4.7/jal/data_import/broker_statements/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-22 16:32:16.000000 jal-2023.4.7/jal/data_import/broker_statements/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    65337 2023-04-21 18:16:02.000000 jal-2023.4.7/jal/data_import/broker_statements/ibkr.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19903 2022-08-21 07:15:06.000000 jal-2023.4.7/jal/data_import/broker_statements/just2trade.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9470 2022-08-21 07:15:06.000000 jal-2023.4.7/jal/data_import/broker_statements/kit.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5857 2023-02-14 12:14:19.000000 jal-2023.4.7/jal/data_import/broker_statements/open_portfolio.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    31013 2023-04-20 21:42:30.000000 jal-2023.4.7/jal/data_import/broker_statements/openbroker.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15460 2022-12-07 21:59:21.000000 jal-2023.4.7/jal/data_import/broker_statements/psb.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    27485 2023-04-20 18:05:58.000000 jal-2023.4.7/jal/data_import/broker_statements/uralsib.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3893 2023-03-05 19:06:08.000000 jal-2023.4.7/jal/data_import/category_recognizer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      543 2021-08-05 15:24:10.000000 jal-2023.4.7/jal/data_import/import_schema.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15598 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/data_import/slips.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13145 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/data_import/slips_tax.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35722 2023-04-21 16:25:20.000000 jal-2023.4.7/jal/data_import/statement.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11314 2023-02-02 08:45:14.000000 jal-2023.4.7/jal/data_import/statement_xls.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6950 2023-04-14 11:26:23.000000 jal-2023.4.7/jal/data_import/statement_xml.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3224 2023-04-08 19:50:05.000000 jal-2023.4.7/jal/data_import/statements.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.993790 jal-2023.4.7/jal/db/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/db/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17607 2023-02-27 16:25:45.000000 jal-2023.4.7/jal/db/account.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21487 2023-04-14 11:26:23.000000 jal-2023.4.7/jal/db/asset.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     6074 2022-12-06 18:30:39.000000 jal-2023.4.7/jal/db/backup_restore.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7360 2023-02-27 17:48:37.000000 jal-2023.4.7/jal/db/balances_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4103 2023-02-27 16:03:46.000000 jal-2023.4.7/jal/db/category.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5218 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/db/closed_trade.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2399 2023-03-08 17:11:23.000000 jal-2023.4.7/jal/db/country.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    18652 2023-04-15 13:39:15.000000 jal-2023.4.7/jal/db/db.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3941 2023-04-12 09:44:25.000000 jal-2023.4.7/jal/db/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15989 2023-04-14 11:27:05.000000 jal-2023.4.7/jal/db/holdings_model.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    16683 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/db/ledger.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    60565 2023-04-07 14:10:37.000000 jal-2023.4.7/jal/db/operations.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7461 2023-04-20 16:47:43.000000 jal-2023.4.7/jal/db/operations_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3379 2023-02-20 16:05:40.000000 jal-2023.4.7/jal/db/peer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15204 2023-04-15 13:54:08.000000 jal-2023.4.7/jal/db/reference_models.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1190 2023-01-06 21:49:49.000000 jal-2023.4.7/jal/db/settings.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      438 2023-02-16 17:12:29.000000 jal-2023.4.7/jal/db/tag.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6777 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/db/tax_estimator.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1458 2023-02-23 19:54:06.000000 jal-2023.4.7/jal/db/view_model.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.997123 jal-2023.4.7/jal/img/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2922 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/accept.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1443 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/add.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2049 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/add_child.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      435 2022-04-25 10:26:48.000000 jal-2023.4.7/jal/img/broom.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4004 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/cancel.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      806 2023-03-08 16:58:09.000000 jal-2023.4.7/jal/img/chart.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      898 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/copy.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2812 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/delete.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      583 2021-03-20 12:52:05.000000 jal-2023.4.7/jal/img/ibkr.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2340 2022-04-29 07:05:21.000000 jal-2023.4.7/jal/img/j2t.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5563 2022-01-13 06:08:45.000000 jal-2023.4.7/jal/img/jal.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1516 2021-03-22 11:20:31.000000 jal-2023.4.7/jal/img/kit.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1163 2022-12-28 10:47:37.000000 jal-2023.4.7/jal/img/list.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      342 2022-04-25 10:26:48.000000 jal-2023.4.7/jal/img/meatballs.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      611 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/new.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1175 2022-07-10 15:39:56.000000 jal-2023.4.7/jal/img/open_portfolio.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15086 2021-08-05 15:24:10.000000 jal-2023.4.7/jal/img/openbroker.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-08-05 15:24:10.000000 jal-2023.4.7/jal/img/psb.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-03-20 12:52:05.000000 jal-2023.4.7/jal/img/quik.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2651 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/reconcile.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      822 2021-05-26 12:51:46.000000 jal-2023.4.7/jal/img/remove.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1874 2023-03-08 16:53:42.000000 jal-2023.4.7/jal/img/tax.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1406 2021-03-20 12:52:05.000000 jal-2023.4.7/jal/img/uralsib.ico
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     1938 2023-01-19 12:05:21.000000 jal-2023.4.7/jal/jal.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    91499 2023-04-07 14:10:37.000000 jal-2023.4.7/jal/jal_init.sql
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.997123 jal-2023.4.7/jal/languages/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      424 2020-12-21 16:23:10.000000 jal-2023.4.7/jal/languages/en.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    32025 2022-01-13 06:08:45.000000 jal-2023.4.7/jal/languages/en.qm
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      287 2022-04-25 10:26:48.000000 jal-2023.4.7/jal/languages/ru.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    87966 2023-04-20 18:09:17.000000 jal-2023.4.7/jal/languages/ru.qm
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.000456 jal-2023.4.7/jal/net/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2021-08-17 15:15:47.000000 jal-2023.4.7/jal/net/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    24656 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/net/downloader.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2912 2023-01-27 21:53:46.000000 jal-2023.4.7/jal/net/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2040 2023-03-06 11:34:17.000000 jal-2023.4.7/jal/pypi_description.md
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.003790 jal-2023.4.7/jal/reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2967 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/reports/category.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14386 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/reports/deals.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3936 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/reports/holdings.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17557 2023-04-16 16:12:41.000000 jal-2023.4.7/jal/reports/income_spending.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2855 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/reports/peer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8772 2023-04-16 16:04:35.000000 jal-2023.4.7/jal/reports/profit_loss.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3287 2023-02-16 10:22:14.000000 jal-2023.4.7/jal/reports/reports.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2827 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/reports/tag.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.003790 jal-2023.4.7/jal/ui/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/ui/__init__.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.007123 jal-2023.4.7/jal/ui/reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-13 15:45:51.000000 jal-2023.4.7/jal/ui/reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5179 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_category_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4099 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_deals_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4159 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_holdings_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4954 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_income_spending_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5382 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_peer_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4687 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_profit_loss_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5353 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_tag_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4805 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/reports/ui_tax_estimation.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12742 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_asset_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4056 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_flow_export_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14782 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_login_fns_dlg.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     9324 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_main_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14510 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_operations_widget.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     5707 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_rebuild_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7302 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_reference_data_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2903 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_select_account_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3253 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_select_reference_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16301 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_slip_import_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9674 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_tax_export_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4023 2023-04-20 18:08:23.000000 jal-2023.4.7/jal/ui/ui_update_quotes_window.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.017123 jal-2023.4.7/jal/updates/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/updates/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5122 2020-12-21 16:23:10.000000 jal-2023.4.7/jal/updates/jal_delta_10.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12870 2021-08-18 12:53:40.000000 jal-2023.4.7/jal/updates/jal_delta_11.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26116 2021-01-13 17:04:46.000000 jal-2023.4.7/jal/updates/jal_delta_12.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16516 2021-01-30 16:01:43.000000 jal-2023.4.7/jal/updates/jal_delta_13.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    34961 2021-02-27 17:35:02.000000 jal-2023.4.7/jal/updates/jal_delta_14.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2250 2021-02-27 17:35:02.000000 jal-2023.4.7/jal/updates/jal_delta_15.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3630 2021-02-27 17:35:02.000000 jal-2023.4.7/jal/updates/jal_delta_16.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20912 2021-02-27 17:35:02.000000 jal-2023.4.7/jal/updates/jal_delta_17.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      656 2021-03-07 11:58:53.000000 jal-2023.4.7/jal/updates/jal_delta_18.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      686 2021-03-08 13:39:11.000000 jal-2023.4.7/jal/updates/jal_delta_19.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13578 2021-03-12 14:26:01.000000 jal-2023.4.7/jal/updates/jal_delta_20.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1428 2021-03-19 12:24:53.000000 jal-2023.4.7/jal/updates/jal_delta_21.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      949 2021-03-22 11:20:31.000000 jal-2023.4.7/jal/updates/jal_delta_22.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17602 2021-04-08 12:12:36.000000 jal-2023.4.7/jal/updates/jal_delta_23.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      344 2021-04-11 10:57:46.000000 jal-2023.4.7/jal/updates/jal_delta_24.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8270 2021-04-22 04:11:28.000000 jal-2023.4.7/jal/updates/jal_delta_25.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2492 2021-08-12 19:15:12.000000 jal-2023.4.7/jal/updates/jal_delta_26.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26325 2022-01-13 05:57:31.000000 jal-2023.4.7/jal/updates/jal_delta_27.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13276 2022-01-13 06:08:45.000000 jal-2023.4.7/jal/updates/jal_delta_28.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35370 2022-01-13 15:45:51.000000 jal-2023.4.7/jal/updates/jal_delta_29.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8671 2022-02-13 13:11:58.000000 jal-2023.4.7/jal/updates/jal_delta_30.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11413 2022-02-13 11:04:18.000000 jal-2023.4.7/jal/updates/jal_delta_31.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12545 2022-03-31 14:26:11.000000 jal-2023.4.7/jal/updates/jal_delta_32.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4229 2022-03-31 14:26:11.000000 jal-2023.4.7/jal/updates/jal_delta_33.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2287 2022-04-06 14:47:21.000000 jal-2023.4.7/jal/updates/jal_delta_34.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2858 2022-04-30 20:05:13.000000 jal-2023.4.7/jal/updates/jal_delta_35.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3427 2022-06-19 17:39:33.000000 jal-2023.4.7/jal/updates/jal_delta_36.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3755 2022-07-20 07:00:10.000000 jal-2023.4.7/jal/updates/jal_delta_37.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21913 2022-08-21 07:15:06.000000 jal-2023.4.7/jal/updates/jal_delta_38.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      343 2023-01-04 13:14:35.000000 jal-2023.4.7/jal/updates/jal_delta_39.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3055 2023-01-27 21:53:46.000000 jal-2023.4.7/jal/updates/jal_delta_40.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    48157 2023-02-07 18:26:24.000000 jal-2023.4.7/jal/updates/jal_delta_41.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2085 2023-02-20 14:55:36.000000 jal-2023.4.7/jal/updates/jal_delta_42.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2528 2023-03-08 16:23:30.000000 jal-2023.4.7/jal/updates/jal_delta_43.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3020 2023-04-07 14:10:37.000000 jal-2023.4.7/jal/updates/jal_delta_44.sql
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.017123 jal-2023.4.7/jal/widgets/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.7/jal/widgets/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3912 2023-04-15 09:01:12.000000 jal-2023.4.7/jal/widgets/abstract_operation_details.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6846 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/account_select.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14491 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/asset_dialog.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11302 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/corporate_action_widget.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:44.020457 jal-2023.4.7/jal/widgets/custom/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-12-24 19:32:40.000000 jal-2023.4.7/jal/widgets/custom/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4703 2023-04-20 16:58:35.000000 jal-2023.4.7/jal/widgets/custom/date_range_selector.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2015 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/custom/db_lookup_combobox.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5874 2023-04-20 16:38:19.000000 jal-2023.4.7/jal/widgets/custom/log_viewer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13628 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/delegates.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9289 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/dividend_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10438 2023-04-16 16:04:35.000000 jal-2023.4.7/jal/widgets/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12488 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/income_spending_widget.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    13018 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/widgets/main_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3386 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/mdi.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2854 2022-12-26 13:26:40.000000 jal-2023.4.7/jal/widgets/operations_tabs.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7159 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/widgets/operations_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6013 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/price_chart.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5667 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/qr_scanner.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11244 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/widgets/reference_data.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21856 2023-04-15 13:54:08.000000 jal-2023.4.7/jal/widgets/reference_dialogs.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4779 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/reference_selector.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      632 2022-12-26 08:54:07.000000 jal-2023.4.7/jal/widgets/register_designer_plugins.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3499 2023-04-15 14:14:41.000000 jal-2023.4.7/jal/widgets/selection_dialog.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7862 2023-04-14 18:14:21.000000 jal-2023.4.7/jal/widgets/tax_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6890 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/trade_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10088 2023-04-15 14:13:28.000000 jal-2023.4.7/jal/widgets/transfer_widget.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-21 18:29:43.980456 jal-2023.4.7/jal.egg-info/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-21 18:29:43.000000 jal-2023.4.7/jal.egg-info/PKG-INFO
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5592 2023-04-21 18:29:43.000000 jal-2023.4.7/jal.egg-info/SOURCES.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        1 2023-04-21 18:29:43.000000 jal-2023.4.7/jal.egg-info/dependency_links.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       37 2023-04-21 18:29:43.000000 jal-2023.4.7/jal.egg-info/entry_points.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       67 2023-04-21 18:29:43.000000 jal-2023.4.7/jal.egg-info/requires.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       10 2023-04-21 18:29:43.000000 jal-2023.4.7/jal.egg-info/top_level.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       38 2023-04-21 18:29:44.020457 jal-2023.4.7/setup.cfg
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1756 2023-04-14 18:14:21.000000 jal-2023.4.7/setup.py
```

### Comparing `jal-2023.4.6/PKG-INFO` & `jal-2023.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jal
-Version: 2023.4.6
+Version: 2023.4.7
 Summary: Just Another Ledger - project to track personal financial records
 Home-page: https://github.com/titov-vv/jal
 Author-email: jal@gmx.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `jal-2023.4.6/docs/README.md` & `jal-2023.4.7/docs/README.md`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/constants.py` & `jal-2023.4.7/jal/constants.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/dlsg.py` & `jal-2023.4.7/jal/data_export/dlsg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/tax_reports/portugal.json` & `jal-2023.4.7/jal/data_export/tax_reports/portugal.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/tax_reports/portugal.py` & `jal-2023.4.7/jal/data_export/tax_reports/portugal.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/tax_reports/russia.json` & `jal-2023.4.7/jal/data_export/tax_reports/russia.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/tax_reports/russia.py` & `jal-2023.4.7/jal/data_export/tax_reports/russia.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/taxes.py` & `jal-2023.4.7/jal/data_export/taxes.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/taxes_flow.py` & `jal-2023.4.7/jal/data_export/taxes_flow.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/templates/tax_prt_dividends.json` & `jal-2023.4.7/jal/data_export/templates/tax_prt_dividends.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/templates/tax_prt_shares.json` & `jal-2023.4.7/jal/data_export/templates/tax_prt_shares.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/templates/tax_rus_bonds.json` & `jal-2023.4.7/jal/data_export/templates/tax_rus_bonds.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/templates/tax_rus_corporate_actions.json` & `jal-2023.4.7/jal/data_export/templates/tax_rus_corporate_actions.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/templates/tax_rus_crypto.json` & `jal-2023.4.7/jal/data_export/templates/tax_rus_crypto.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/templates/tax_rus_derivatives.json` & `jal-2023.4.7/jal/data_export/templates/tax_rus_derivatives.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/templates/tax_rus_dividends.json` & `jal-2023.4.7/jal/data_export/templates/tax_rus_dividends.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/templates/tax_rus_fees.json` & `jal-2023.4.7/jal/data_export/templates/tax_rus_fees.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/templates/tax_rus_flow.json` & `jal-2023.4.7/jal/data_export/templates/tax_rus_flow.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/templates/tax_rus_interests.json` & `jal-2023.4.7/jal/data_export/templates/tax_rus_interests.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/templates/tax_rus_trades.json` & `jal-2023.4.7/jal/data_export/templates/tax_rus_trades.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_export/xlsx.py` & `jal-2023.4.7/jal/data_export/xlsx.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_import/broker_statements/ibkr.py` & `jal-2023.4.7/jal/data_import/broker_statements/ibkr.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
         'STK': FOF.ASSET_STOCK,
         'ETF': FOF.ASSET_ETF,
         'ADR': FOF.ASSET_ADR,
         'BOND': FOF.ASSET_BOND,
         'OPT': FOF.ASSET_OPTION,
         'FUT': FOF.ASSET_FUTURES,
         'WAR': FOF.ASSET_WARRANT,
-        'RIGHT': FOF.ASSET_RIGHTS
+        'RIGHT': FOF.ASSET_RIGHTS,
+        'CFD': FOF.ASSET_CFD
     }
 
     def __init__(self, asset_type, subtype):
         self.type = self.NotSupported
         try:
             self.type = self._asset_types[asset_type]
         except KeyError:
@@ -125,14 +126,15 @@
     statements_path = '/*/FlexStatement'
     statement_tag = 'FlexStatement'
     level_tag = 'levelOfDetail'
     CancelledFlag = 'Ca'
     ReversalCode = 'Re'
     ReversalSuffix = " - REVERSAL"
     CancelPrefix = "CANCEL "
+    NoAsset = -1
 
     def __init__(self):
         super().__init__()
         self.name = self.tr("Interactive Brokers")
         self.icon_name = "ibkr.png"
         self.filename_filter = self.tr("IBKR flex-query (*.xml)")
 
@@ -253,15 +255,24 @@
                                  'level': 'SUMMARY',
                                  'values': [('accountId', 'account', IBKR_Account, None),
                                             ('symbol', 'symbol', str, None),
                                             ('date', 'timestamp', datetime, None),
                                             ('taxAmount', 'amount', float, None),
                                             ('description', 'description', str, None),
                                             ('taxDescription', 'tax_description', str, None)],
-                                 'loader': self.load_taxes}
+                                 'loader': self.load_taxes},
+            'CFDCharges': {'tag': 'CFDCharge',
+                           'level': '',
+                           'values': [('accountId', 'account', IBKR_Account, None),
+                                      ('symbol', 'asset', IBKR_Asset, self.NoAsset),
+                                      ('date', 'timestamp', datetime, None),
+                                      ('total', 'amount', float, None),
+                                      ('transactionID', 'number', str, ''),
+                                      ('activityDescription', 'description', str, None)],
+                           'loader': self.load_cfd_charges},
         }
 
     def tr(self, text):
         return QApplication.translate("IBKR", text)
 
     # Saves information from XML that is related with a given asset
     def save_debug_info(self, account, asset):
@@ -303,15 +314,15 @@
         return IBKR_AssetType(xml_element.attrib[attr_name], sub_type).type
 
     # Convert attribute 'attr_name' value into JAL corporate action
     def attr_corp_action_type(self, xml_element, attr_name, default_value):
         if attr_name not in xml_element.attrib:
             return default_value
         asset_category = self.attr_asset_type(xml_element, 'assetCategory', None)
-        if asset_category not in [FOF.ASSET_STOCK, FOF.ASSET_BOND, FOF.ASSET_WARRANT]:
+        if asset_category not in [FOF.ASSET_STOCK, FOF.ASSET_BOND, FOF.ASSET_WARRANT, FOF.ASSET_CFD]:
             logging.error(self.tr("Corporate action isn't supported for asset type: ") + f"'{asset_category}'")
             return default_value
         return IBKR_CorpActionType(xml_element.attrib[attr_name]).type
 
     def attr_currency(self, xml_element, attr_name, default_value):
         if attr_name not in xml_element.attrib:
             return default_value
@@ -710,23 +721,23 @@
         action['price'] = format_decimal(Decimal(str(action['value'])) / Decimal(str(action['quantity'])))
         action['tax'] = 0
         self.drop_extra_fields(action, ["quantity", "value", "proceeds", "code", "asset_type", "jal_processed"])
         self._data[FOF.ASSET_PAYMENTS].append(action)
         return 1
 
     def load_split(self, action, parts_b) -> int:
-        SplitPattern = r"^(?P<symbol_old>.*)\((?P<isin_old>\w+)\) +SPLIT +(?P<X>\d+) +FOR +(?P<Y>\d+) +\((?P<symbol>.*), (?P<name>.*), (?P<id>\w+)\)$"
+        SplitPattern = r"^(?P<symbol_old>.*)\((?P<isin_old>\w+)\) +SPLIT +(?P<X>\d+) +FOR +(?P<Y>\d+) +\((?P<symbol>.*), (?P<name>.*), (?P<id>\w+)*\)$"
 
         parts = re.match(SplitPattern, action['description'], re.IGNORECASE)
         if parts is None:
             raise Statement_ImportError(self.tr("Can't parse Split description ") + f"'{action}'")
         split = parts.groupdict()
         if len(split) != SplitPattern.count("(?P<"):  # check that expected number of groups was matched
             raise Statement_ImportError(self.tr("Split description miss some data ") + f"'{action}'")
-        if parts['isin_old'] == parts['id']:  # Simple split without ISIN change
+        if parts['id'] is None or parts['isin_old'] == parts['id']:  # Simple split without ISIN change
             qty_delta = action['quantity']
             qty_old = qty_delta / (int(split['X']) / int(split['Y']) - 1)
             qty_new = qty_old + qty_delta
             action['id'] = max([0] + [x['id'] for x in self._data[FOF.CORP_ACTIONS]]) + 1
             action['outcome'] = [{'asset': action['asset'], 'quantity': qty_new, 'share': 1.0}]
             action['quantity'] = qty_old
             self.drop_extra_fields(action, ["value", "proceeds", "code", "asset_type", "jal_processed"])
@@ -930,14 +941,35 @@
             note = f"{tax['symbol']} ({tax['description']}) - {tax['tax_description']}"
             tax['lines'] = [{'amount': tax['amount'], 'category': -PredefinedCategory.Taxes, 'description': note}]
             self.drop_extra_fields(tax, ["symbol", "amount", "description", "tax_description"])
             self._data[FOF.INCOME_SPENDING].append(tax)
             cnt += 1
         logging.info(self.tr("Taxes loaded: ") + f"{cnt} ({len(taxes)})")
 
+    def load_cfd_charges(self, charges):
+        cnt = 0
+        charges_base = max([0] + [x['id'] for x in self._data[FOF.INCOME_SPENDING]]) + 1
+        for i, charge in enumerate(charges):
+            if charge['asset'] != self.NoAsset and not charge['description'].startswith('CFD BORROW FEE FOR'):
+                # FIXME if asset is present -> put this charge not in Income/Spending but in Asset Payments section
+                logging.warning(self.tr("Unknown CFD charge description: ") + charge['description'])
+                continue
+            if charge['asset'] == self.NoAsset and not (
+                    charge['description'].startswith('LONG CFD INTEREST FOR') or
+                    charge['description'].startswith('SHORT CFD INTEREST FOR')):
+                logging.warning(self.tr("Unknown CFD charge description: ") + charge['description'])
+                continue
+            charge['id'] = charges_base + i
+            charge['peer'] = 0
+            charge['lines'] = [{'amount': charge['amount'], 'category': -PredefinedCategory.Fees, 'description': charge['description']}]
+            self.drop_extra_fields(charge, ["amount", "asset", "description", "number"])
+            self._data[FOF.INCOME_SPENDING].append(charge)
+            cnt += 1
+        logging.info(self.tr("CFD charges loaded: ") + f"{cnt} ({len(charges)})")
+
     # Applies tax to matching dividend:
     # if tax < 0: apply it to dividend without tax
     # otherwise: it is a correction and there should be dividend with exactly the same tax that will be set to 0
     def apply_tax_withheld(self, tax) -> int:
         TaxFullPattern = r"^(?P<description>.*) - (?P<country>\w\w) TAX$"
 
         parts = re.match(TaxFullPattern, tax['description'], re.IGNORECASE)
```

### Comparing `jal-2023.4.6/jal/data_import/broker_statements/just2trade.py` & `jal-2023.4.7/jal/data_import/broker_statements/just2trade.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_import/broker_statements/kit.py` & `jal-2023.4.7/jal/data_import/broker_statements/kit.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_import/broker_statements/open_portfolio.py` & `jal-2023.4.7/jal/data_import/broker_statements/open_portfolio.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_import/broker_statements/openbroker.py` & `jal-2023.4.7/jal/data_import/broker_statements/openbroker.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from PySide6.QtWidgets import QApplication
 from jal.constants import PredefinedCategory, PredefinedAsset
 from jal.db.asset import JalAsset
 from jal.data_import.statement import FOF, Statement_ImportError
 from jal.data_import.statement_xml import StatementXML
 from jal.net.downloader import QuoteDownloader
+from jal.widgets.helpers import dt2ts
 
 JAL_STATEMENT_CLASS = "StatementOpenBroker"
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class OpenBroker_AssetType:
     NotSupported = -1
@@ -328,15 +329,15 @@
             elif "Перевод ЦБ в" in operation['description']:
                 self.load_asset_transfer_out(operation)
             else:
                 raise Statement_ImportError(self.tr("Unknown non-trade operation: ") + operation['description'])
 
     def load_bond_repayment(self, operation):
         # Asset name is stored as alternative symbol and in self.asset_withdrawal[]
-        bond_repayment_pattern = r"^.*Снятие ЦБ с учета\. Погашение облигаций - (?P<asset_name>.*)$"
+        bond_repayment_pattern = r"^Отчет депозитария.*от (?P<report_date>\d\d\.\d\d\.\d\d\d\d)\. Снятие ЦБ с учета\. Погашение облигаций - (?P<asset_name>.*)$"
         parts = re.match(bond_repayment_pattern, operation['description'], re.IGNORECASE)
         if parts is None:
             raise Statement_ImportError(
                 self.tr("Can't parse bond repayment description ") + f"'{operation['description']}'")
         repayment_note = parts.groupdict()
         if len(repayment_note) != bond_repayment_pattern.count("(?P<"):  # check expected number of matches
             raise Statement_ImportError(
@@ -344,17 +345,19 @@
         ticker = self._find_in_list(self._data[FOF.SYMBOLS], 'asset', operation['asset'])
         if ticker['symbol'] != repayment_note['asset_name']:  # Store alternative depositary name
             ticker = ticker.copy()
             ticker['id'] = max([0] + [x['id'] for x in self._data[FOF.SYMBOLS]]) + 1
             ticker['symbol'] = repayment_note['asset_name']
             ticker['broker_symbol'] = True
             self._data[FOF.SYMBOLS].append(ticker)
+        report_date = dt2ts(datetime.strptime(repayment_note['report_date'], "%d.%m.%Y"))
         new_id = max([0] + [x['id'] for x in self.asset_withdrawal]) + 1
-        record = {"id": new_id, "timestamp": operation['timestamp'], "asset": operation['asset'],
-                  "symbol": ticker['symbol'], "quantity": operation['quantity'], "note": operation['description']}
+        record = {"id": new_id, "timestamp": operation['timestamp'], "report_date": report_date,
+                  "asset": operation['asset'], "symbol": ticker['symbol'],
+                  "quantity": operation['quantity'], "note": operation['description']}
         self.asset_withdrawal.append(record)
 
     def load_asset_transfer_out(self, transfer):
         transfer['id'] = max([0] + [x['id'] for x in self._data[FOF.TRANSFERS]]) + 1
         ruble_id = JalAsset(data={'symbol': 'RUB', 'type_id': PredefinedAsset.Money}, search=True, create=False).id()
         transfer['account'] = [ruble_id, 0, 0]   # Assume russian ruble as default for Open Broker
         transfer['asset'] = [transfer['asset'], transfer['asset']]
@@ -486,15 +489,16 @@
         parts = re.match(repayment_pattern, description, re.IGNORECASE)
         if parts is None:
             raise Statement_ImportError(self.tr("Can't parse Bond Mature description ") + f"'{description}'")
         repayment = parts.groupdict()
         if len(repayment) != repayment_pattern.count("(?P<"):  # check expected number of matches
             raise Statement_ImportError(self.tr("Bond repayment description miss some data ")
                                         + f"'{description}'")
-        match = [x for x in self.asset_withdrawal if x['symbol'] == repayment['asset'] and x['timestamp'] == timestamp]
+        match = [x for x in self.asset_withdrawal if
+                 x['symbol'] == repayment['asset'] and (x['timestamp'] == timestamp or x['report_date'] == timestamp)]
         if not match:
             raise Statement_ImportError(self.tr("Can't find asset cancellation record for ")
                                         + f"'{description}'")
         if len(match) != 1:
             raise Statement_ImportError(self.tr("Multiple asset cancellation match for ")
                                         + f"'{description}'")
         asset_cancel = match[0]
```

### Comparing `jal-2023.4.6/jal/data_import/broker_statements/psb.py` & `jal-2023.4.7/jal/data_import/broker_statements/psb.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_import/broker_statements/uralsib.py` & `jal-2023.4.7/jal/data_import/broker_statements/uralsib.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from jal.data_import.statement_xls import StatementXLS
 
 JAL_STATEMENT_CLASS = "StatementUKFU"
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class StatementUKFU(StatementXLS):
-    Header = (2, 0, '  Брокер: ООО "УРАЛСИБ Брокер"')
-    PeriodPattern = (2, 2, r"  за период с (?P<S>\d\d\.\d\d\.\d\d\d\d) по (?P<E>\d\d\.\d\d\.\d\d\d\d)")
-    AccountPattern = (2, 7, None)
+    Header = (0, 0, '  Брокер: ООО "Твой Брокер"')
+    PeriodPattern = (0, 2, r"  за период с (?P<S>\d\d\.\d\d\.\d\d\d\d) по (?P<E>\d\d\.\d\d\.\d\d\d\d)")
+    AccountPattern = (2, 6, None)
     SummaryHeader = "СОСТОЯНИЕ ДЕНЕЖНЫХ СРЕДСТВ НА СЧЕТЕ"
     trade_columns = {
         "number": "Номер сделки",
         "date": "Дата сделки",
         "time": "Время сделки",
         "settlement": "Дата поставки, плановая",
         "isin": "ISIN",
@@ -41,17 +41,17 @@
         "name": "Наименование ЦБ",
         "isin": "ISIN",
         "reg_number": "Номер гос. регистрации / CFI код"
     }
 
     def __init__(self):
         super().__init__()
-        self.name = self.tr("Uralsib Broker")
+        self.name = self.tr("Tvoy Broker (ex. Uralsib Broker)")
         self.icon_name = "uralsib.ico"
-        self.filename_filter = self.tr("Uralsib statement (*.zip)")
+        self.filename_filter = self.tr("Tvoy Broker statement (*.zip)")
         self.asset_withdrawal = []
 
     def _load_deals(self):
         self.load_stock_deals()
         self.load_futures_deals()
         self.load_asset_movements()
```

### Comparing `jal-2023.4.6/jal/data_import/category_recognizer.py` & `jal-2023.4.7/jal/data_import/category_recognizer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_import/import_schema.json` & `jal-2023.4.7/jal/data_import/import_schema.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_import/slips.py` & `jal-2023.4.7/jal/data_import/slips.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_import/slips_tax.py` & `jal-2023.4.7/jal/data_import/slips_tax.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_import/statement.py` & `jal-2023.4.7/jal/data_import/statement.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     ASSET_ETF = "etf"
     ASSET_BOND = "bond"
     ASSET_FUTURES = "futures"
     ASSET_OPTION = "option"
     ASSET_WARRANT = "warrant"
     ASSET_RIGHTS = "right"
     ASSET_CRYPTO = "crypto"
+    ASSET_CFD = "cfd"
 
     ACTION_MERGER = "merger"
     ACTION_SPLIT = "split"
     ACTION_SPINOFF = "spin-off"
     ACTION_SYMBOL_CHANGE = "symbol_change"
     ACTION_BOND_MATURITY = "bond_maturity"    # Isn't used in reality as will be put as ordinary sell operation
     ACTION_DELISTING = "delisting"
@@ -83,14 +84,15 @@
         FOF.ASSET_STOCK: PredefinedAsset.Stock,
         FOF.ASSET_ADR: PredefinedAsset.Stock,
         FOF.ASSET_ETF: PredefinedAsset.ETF,
         FOF.ASSET_BOND: PredefinedAsset.Bond,
         FOF.ASSET_FUTURES: PredefinedAsset.Derivative,
         FOF.ASSET_OPTION: PredefinedAsset.Derivative,
         FOF.ASSET_WARRANT: PredefinedAsset.Derivative,
+        FOF.ASSET_CFD: PredefinedAsset.Derivative,
         FOF.ASSET_CRYPTO: PredefinedAsset.Crypto
     }
     _corp_actions = {
         FOF.ACTION_MERGER: CorporateAction.Merger,
         FOF.ACTION_SPLIT: CorporateAction.Split,
         FOF.ACTION_SPINOFF: CorporateAction.SpinOff,
         FOF.ACTION_SYMBOL_CHANGE: CorporateAction.SymbolChange,
```

### Comparing `jal-2023.4.6/jal/data_import/statement_xls.py` & `jal-2023.4.7/jal/data_import/statement_xls.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_import/statement_xml.py` & `jal-2023.4.7/jal/data_import/statement_xml.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/data_import/statements.py` & `jal-2023.4.7/jal/data_import/statements.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/account.py` & `jal-2023.4.7/jal/db/account.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/asset.py` & `jal-2023.4.7/jal/db/asset.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/backup_restore.py` & `jal-2023.4.7/jal/db/backup_restore.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/balances_model.py` & `jal-2023.4.7/jal/db/balances_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/category.py` & `jal-2023.4.7/jal/db/category.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/closed_trade.py` & `jal-2023.4.7/jal/db/closed_trade.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/country.py` & `jal-2023.4.7/jal/db/country.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/db.py` & `jal-2023.4.7/jal/db/db.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/helpers.py` & `jal-2023.4.7/jal/db/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/holdings_model.py` & `jal-2023.4.7/jal/db/holdings_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/ledger.py` & `jal-2023.4.7/jal/db/ledger.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/operations.py` & `jal-2023.4.7/jal/db/operations.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/operations_model.py` & `jal-2023.4.7/jal/db/operations_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from decimal import Decimal
 from PySide6.QtCore import Qt, Slot, QDate, QAbstractTableModel, QModelIndex
-from PySide6.QtGui import QBrush, QFontDatabase, QFontMetrics
+from PySide6.QtGui import QBrush, QFontDatabase
 from PySide6.QtWidgets import QStyledItemDelegate, QHeaderView
 from jal.constants import CustomColor
 from jal.db.ledger import Ledger
 from jal.db.operations import LedgerTransaction
 from jal.widgets.helpers import ts2dt
```

### Comparing `jal-2023.4.6/jal/db/peer.py` & `jal-2023.4.7/jal/db/peer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/reference_models.py` & `jal-2023.4.7/jal/db/reference_models.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/settings.py` & `jal-2023.4.7/jal/db/settings.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/tax_estimator.py` & `jal-2023.4.7/jal/db/tax_estimator.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/db/view_model.py` & `jal-2023.4.7/jal/db/view_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/accept.png` & `jal-2023.4.7/jal/img/accept.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/add.png` & `jal-2023.4.7/jal/img/add.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/add_child.png` & `jal-2023.4.7/jal/img/add_child.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/cancel.png` & `jal-2023.4.7/jal/img/cancel.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/chart.png` & `jal-2023.4.7/jal/img/chart.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/copy.png` & `jal-2023.4.7/jal/img/copy.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/delete.png` & `jal-2023.4.7/jal/img/delete.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/ibkr.png` & `jal-2023.4.7/jal/img/ibkr.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/j2t.png` & `jal-2023.4.7/jal/img/j2t.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/jal.png` & `jal-2023.4.7/jal/img/jal.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/kit.png` & `jal-2023.4.7/jal/img/kit.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/list.png` & `jal-2023.4.7/jal/img/list.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/new.png` & `jal-2023.4.7/jal/img/new.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/open_portfolio.png` & `jal-2023.4.7/jal/img/open_portfolio.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/openbroker.ico` & `jal-2023.4.7/jal/img/openbroker.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/psb.ico` & `jal-2023.4.7/jal/img/psb.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/quik.ico` & `jal-2023.4.7/jal/img/quik.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/reconcile.png` & `jal-2023.4.7/jal/img/reconcile.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/remove.png` & `jal-2023.4.7/jal/img/remove.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/tax.png` & `jal-2023.4.7/jal/img/tax.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/img/uralsib.ico` & `jal-2023.4.7/jal/img/uralsib.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/jal.py` & `jal-2023.4.7/jal/jal.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/jal_init.sql` & `jal-2023.4.7/jal/jal_init.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/languages/en.qm` & `jal-2023.4.7/jal/languages/en.qm`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/languages/ru.qm` & `jal-2023.4.7/jal/languages/ru.qm`

 * *Files 2% similar despite different names*

```diff
@@ -1,5473 +1,5498 @@
 00000000: 3cb8 6418 caef 9c95 cd21 1cbf 60a1 bddd  <.d......!..`...
-00000010: a700 0000 0572 755f 5255 4200 001a 0000  .....ru_RUB.....
+00000010: a700 0000 0572 755f 5255 4200 001a 3800  .....ru_RUB...8.
 00000020: 0000 2300 001c 2500 0000 2300 0030 1300  ..#...%...#..0..
-00000030: 0000 2300 0130 e500 0000 2300 0135 9500  ..#..0....#..5..
-00000040: 0000 2500 0092 9a00 0004 7300 0005 b700  ..%.......s.....
-00000050: 0005 3b00 0009 4c00 0005 af00 0137 4600  ..;...L......7F.
-00000060: 0031 0e00 007e 3e00 0031 0e00 0124 b900  .1...~>..1...$..
-00000070: 0046 3900 0003 7000 0046 3900 00a3 0500  .F9...p..F9.....
-00000080: 0047 a400 0045 bf00 0048 7200 004e 5200  .G...E...Hr..NR.
-00000090: 0048 7200 0092 c100 0048 b700 004e 8900  .Hr......H...N..
-000000a0: 0048 b700 0093 1c00 004a 7a00 0047 bd00  .H.......Jz..G..
-000000b0: 004a b300 004e c000 004a b300 0093 ca00  .J...N...J......
-000000c0: 004b 1a00 0047 e800 004b 3a00 0048 1300  .K...G...K:..H..
-000000d0: 004c b200 004e f700 004c b200 0094 3600  .L...N...L....6.
-000000e0: 004c b500 0013 bf00 004c b500 0131 e900  .L.......L...1..
-000000f0: 0050 7e00 004f 2e00 0050 7e00 0094 df00  .P~..O...P~.....
-00000100: 0051 3100 001e df00 0051 3100 0031 8400  .Q1......Q1..1..
-00000110: 0051 bc00 004f 6500 0051 bc00 0095 0c00  .Q...Oe..Q......
-00000120: 0051 be00 004f 9c00 0051 be00 0095 3900  .Q...O...Q....9.
-00000130: 0052 ac00 0096 4700 0052 ac00 0098 a000  .R....G..R......
-00000140: 0053 3c00 0015 2300 0053 3c00 0036 c900  .S<...#..S<..6..
-00000150: 0053 8200 004f d300 0053 8200 0095 6600  .S...O...S....f.
-00000160: 0053 8900 0050 0a00 0053 8900 0095 9300  .S...P...S......
-00000170: 0055 6600 0050 4100 0055 6600 0095 ed00  .Uf..PA..Uf.....
-00000180: 0055 a400 0050 7800 0055 a400 0096 1a00  .U...Px..U......
-00000190: 0058 b900 0015 8a00 0058 b900 0020 5e00  .X.......X... ^.
-000001a0: 0058 b900 0037 2800 0058 b900 00aa 1700  .X...7(..X......
-000001b0: 0058 b900 0120 c100 0058 b900 0132 7d00  .X... ...X...2}.
-000001c0: 0059 c000 0050 af00 0059 c000 0097 3e00  .Y...P...Y....>.
-000001d0: 005a 7700 002b cf00 005a 7700 0089 dd00  .Zw..+...Zw.....
-000001e0: 005a 7700 011a c400 005a 8800 0032 f900  .Zw......Z...2..
-000001f0: 005b 2a00 0027 6b00 0070 7c00 005d cd00  .[*..'k..p|..]..
-00000200: 047a 6e00 0005 4000 047a 6e00 0119 a600  .zn...@..zn.....
-00000210: 0498 9800 008f 2800 04a6 7900 0085 6400  ......(...y...d.
-00000220: 04a8 a500 000e 0500 04a8 a500 00a0 2600  ..............&.
-00000230: 04a8 a500 0120 1100 04a8 d300 0091 9900  ..... ..........
-00000240: 04cb c300 0094 6300 04cf 3a00 0035 be00  ......c...:..5..
-00000250: 04d9 5d00 0136 e600 04e3 1a00 0075 b200  ..]..6.......u..
-00000260: 04e7 de00 000b 0d00 04e7 de00 000c 7500  ..............u.
-00000270: 0504 cf00 0078 e500 0528 a400 0035 ee00  .....x...(...5..
-00000280: 0548 3500 0006 1b00 0548 3500 000b 3c00  .H5......H5...<.
-00000290: 0548 3500 0011 c100 0548 3500 008e 5e00  .H5......H5...^.
-000002a0: 0556 a500 0013 f800 0556 a500 001f 1200  .V.......V......
-000002b0: 0556 a500 002b 9a00 0556 a500 0031 f500  .V...+...V...1..
-000002c0: 0556 a500 0055 3700 0556 a500 0132 1c00  .V...U7..V...2..
-000002d0: 0556 a500 0137 0f00 0565 c000 0043 cc00  .V...7...e...C..
-000002e0: 0566 be00 0036 8f00 0566 be00 0120 4300  .f...6...f... C.
-000002f0: 056b c200 0056 e600 05a3 0000 004b d700  .k...V.......K..
-00000300: 05a7 aa00 011b a700 05a7 e300 011d b700  ................
-00000310: 05b3 d800 011e e000 05c0 6500 0021 a300  ..........e..!..
-00000320: 05c0 6500 0033 2900 05db bb00 0027 9a00  ..e..3)......'..
-00000330: 05fb 8200 0027 d000 1530 3000 0012 3a00  .....'...00...:.
-00000340: 18d1 5000 00ee b100 2311 0000 0124 8c00  ..P.....#....$..
-00000350: 26f2 9100 004c 0300 2aa8 a100 0058 9500  &....L..*....X..
-00000360: 2acf 0400 0058 cb00 2b37 fe00 0059 7100  *....X..+7...Yq.
-00000370: 2b76 1e00 0086 3300 2ba7 e300 005b 7500  +v....3.+....[u.
-00000380: 2ec7 e000 0045 5e00 3153 c400 0094 9b00  .....E^.1S......
-00000390: 3d1a 0e00 005d 2800 4182 8900 00ff b000  =....](.A.......
-000003a0: 4796 c400 0078 6600 47af 8000 009c 3500  G....xf.G.....5.
-000003b0: 48a9 c400 0006 db00 48a9 c400 0012 8a00  H.......H.......
-000003c0: 48a9 c400 001c da00 48a9 c400 0029 9400  H.......H....)..
-000003d0: 48a9 c400 0030 6b00 48a9 c400 009f c100  H....0k.H.......
-000003e0: 48a9 c400 00a9 e700 48a9 c400 0131 3700  H.......H....17.
-000003f0: 48a9 c400 0135 ee00 4964 b300 0090 9500  H....5..Id......
-00000400: 4988 b300 008e ee00 4a2b 8200 0046 c700  I.......J+...F..
-00000410: 4a36 9500 002a 4300 4a36 9500 0046 fe00  J6...*C.J6...F..
-00000420: 4a36 9500 0074 be00 4a71 ec00 0025 3100  J6...t..Jq...%1.
-00000430: 4ab8 3300 0028 d400 4b6b 9000 0104 5300  J.3..(..Kk....S.
-00000440: 4d68 c800 0091 c900 4d96 0a00 0025 df00  Mh......M....%..
-00000450: 4dc4 b300 0091 fe00 4e7e 1a00 0008 de00  M.......N~......
-00000460: 522b 5a00 0074 f400 52e9 5500 0014 d900  R+Z..t..R.U.....
-00000470: 5308 d400 0096 aa00 535d fe00 0075 e100  S.......S]...u..
-00000480: 5464 c900 0092 3100 5464 c900 0095 c000  Td....1.Td......
-00000490: 5465 a800 0026 0e00 5483 8a00 0009 0d00  Te...&..T.......
-000004a0: 556a c300 0083 8200 55da be00 0012 0300  Uj......U.......
-000004b0: 56bc 5a00 004a 9200 56bc 5a00 008d 4d00  V.Z..J..V.Z...M.
-000004c0: 56bc 9300 008b 6d00 578f 9500 0032 2c00  V.....m.W....2,.
-000004d0: 578f 9500 0132 5000 57a1 7200 0027 2600  W....2P.W.r..'&.
-000004e0: 5839 2400 006b 2d00 58c6 a500 00a0 5600  X9$..k-.X.....V.
-000004f0: 5948 5c00 0050 e600 5948 5c00 011f 1400  YH\..P..YH\.....
-00000500: 5a73 0400 001a 4a00 5a73 0400 0021 1900  Zs....J.Zs...!..
-00000510: 5a79 2700 011d 8100 5a8a e000 0121 2e00  Zy'.....Z....!..
-00000520: 5a8b c000 002f 6e00 5a8e c300 0097 6b00  Z..../n.Z.....k.
-00000530: 5a8e c300 012d ca00 5b6a 7c00 000d 4600  Z....-..[j|...F.
-00000540: 5b6a 7c00 0097 a000 5c06 8a00 004c 8d00  [j|.....\....L..
-00000550: 5c83 b500 0034 ec00 5c83 b500 0037 9100  \....4..\....7..
-00000560: 5fb8 5a00 0081 5800 5fb8 5a00 012f 2e00  _.Z...X._.Z../..
-00000570: 602e 0a00 0056 8400 67f7 0000 00f8 0000  `....V..g.......
-00000580: 70c5 c000 00c8 8700 80a8 e500 0049 ce00  p............I..
-00000590: 81bc 0000 00ce 7000 918d 3700 003c 4000  ......p...7..<@.
-000005a0: 931f 2000 00d9 df00 9472 3000 0070 6600  .. ......r0..pf.
-000005b0: 9688 5400 00d4 c200 ab81 4000 0117 b900  ..T.......@.....
-000005c0: af00 f000 00b6 4600 af26 4500 0125 1000  ......F..&E..%..
-000005d0: b27d 9f00 0079 7b00 b4d0 c500 0029 d900  .}...y{......)..
-000005e0: b643 0000 00c3 0c00 c9db ba00 0063 2a00  .C...........c*.
-000005f0: cfb0 f400 0031 1100 e1f3 f000 0017 8d00  .....1..........
-00000600: e25b 3000 002c f900 ed2c 2500 0028 0000  .[0..,...,%..(..
-00000610: fbe4 b100 0048 3e00 ff6b fe00 00b3 8401  .....H>..k......
-00000620: 11c0 6000 0139 7e01 1c4b f000 0115 4101  ..`..9~..K....A.
-00000630: 2273 8300 008e 9c01 24a2 9700 003c f701  "s......$....<..
-00000640: 2bca d000 009e aa01 3502 c000 00c4 db01  +.......5.......
-00000650: 473b 2300 0071 5701 5567 7000 00cd c901  G;#..qW.Ugp.....
-00000660: 59b4 9000 001b 0d01 6654 9000 003b 3701  Y.......fT...;7.
-00000670: 7248 d000 0036 2801 776d e000 00d5 e201  rH...6(.wm......
-00000680: 78c3 f500 0031 b001 7e51 ea00 012b 7f01  x....1..~Q...+..
-00000690: 873b 2300 0071 8901 887c d300 005d f901  .;#..q...|...]..
-000006a0: 9687 c000 010b 3c01 98a7 5300 004c bc01  ......<...S..L..
-000006b0: a469 f900 0102 4c01 a885 4000 0134 b901  .i....L...@..4..
-000006c0: aff7 3300 0000 0001 bef6 7000 00d2 e001  ..3.......p.....
-000006d0: c26a 9a00 00a3 3a01 ce0a 1200 008c 5601  .j....:.......V.
-000006e0: d48e 5000 0043 2801 da69 b000 0114 d401  ..P..C(..i......
-000006f0: e128 5000 00c0 1201 e26a 9a00 0004 2801  .(P......j....(.
-00000700: f571 7000 00bd 2102 00dd 0100 0044 6a02  .qp...!......Dj.
-00000710: 01b8 4900 003a 8d02 01b8 4900 0088 9202  ..I..:....I.....
-00000720: 01b8 4900 00a2 c502 01b8 4900 0138 a602  ..I.......I..8..
-00000730: 24d1 2000 00df 9702 2b24 6500 012e 8c02  $. .....+$e.....
-00000740: 36c0 e700 006d 7302 38ab b000 00b0 1502  6....ms.8.......
-00000750: 488e 8300 0127 cb02 5442 2f00 0022 3d02  H....'..TB/.."=.
-00000760: 6b41 b400 012f 5902 705b 1000 0060 7702  kA.../Y.p[...`w.
-00000770: 75ac 0500 00d8 2f02 76e6 2500 0043 fd02  u...../.v.%..C..
-00000780: 80f4 7400 005b ed02 83cb 1900 00ad 1702  ..t..[..........
-00000790: 84df 6000 000d 0b02 86cb d700 00ae a402  ..`.............
-000007a0: 960b 0000 0103 7902 9d24 b400 00bf af02  ......y..$......
-000007b0: a013 f300 00d4 6702 b6bc 9300 0059 eb02  ......g......Y..
-000007c0: b827 6100 00a5 0002 c4de 6000 00c9 1502  .'a.......`.....
-000007d0: d6b9 7000 00e0 7202 d6b9 7000 00ec 5e02  ..p...r...p...^.
-000007e0: d6b9 7000 0102 d002 d6b9 7000 010d 9c02  ..p.......p.....
-000007f0: da2f f000 00bb 4b02 db87 a000 00f2 f102  ./....K.........
-00000800: ddd8 9000 0018 c702 e4ef 0400 0020 9702  ............. ..
-00000810: e60b 0000 0077 e902 ecb9 d000 006e 6f03  .....w.......no.
-00000820: 0055 4a00 012a e803 0ae6 8700 0018 3203  .UJ..*........2.
-00000830: 0ae6 8700 001d ba03 0b8a 5a00 007a f603  ..........Z..z..
-00000840: 1108 9c00 0131 6003 1638 c400 0096 f203  .....1`..8......
-00000850: 1684 be00 001d 0d03 2221 4000 00af 8c03  ........"!@.....
-00000860: 232f f000 00f4 3803 232f f000 0108 d703  #/....8.#/......
-00000870: 3500 5a00 0088 4603 3f3c 8400 0111 4d03  5.Z...F.?<....M.
-00000880: 55cb 1a00 0076 4d03 57fa 2e00 0075 3b03  U....vM.W....u;.
-00000890: 5dae f000 0109 8603 5dce f000 00e4 0b03  ].......].......
-000008a0: 6b8b d900 0126 a603 7321 8300 0110 3103  k....&..s!....1.
-000008b0: 82a1 0000 00e0 a303 8a06 2000 0100 2003  .......... ... .
-000008c0: 8b39 a000 0104 bb03 8b60 e400 003f b803  .9.......`...?..
-000008d0: 8c34 6500 0026 cd03 8f4e c000 0114 0d03  .4e..&...N......
-000008e0: 9100 d000 005f 7f03 97c9 0000 0122 8303  ....._......."..
-000008f0: b023 a000 00b9 fc03 cafd 4000 0083 bb03  .#........@.....
-00000900: d07e 2400 0069 4f03 d1c2 7400 0041 9203  .~$..iO...t..A..
-00000910: d1e5 2200 0005 7103 da9c f300 005b a703  .."...q......[..
-00000920: ec0c f700 003d bd03 f69b 8000 00c7 3504  .....=........5.
-00000930: 0029 e000 0125 f104 09f4 0a00 00bc ad04  .)...%..........
-00000940: 11d2 4900 000d 7704 11d2 a900 0058 0404  ..I...w......X..
-00000950: 1263 4400 00b5 f804 1564 8e00 0029 5a04  .cD......d...)Z.
-00000960: 15b4 7000 0139 f704 195c b000 0119 0f04  ..p..9...\......
-00000970: 2e61 f000 0073 7104 449a c000 012c d804  .a...sq.D....,..
-00000980: 56c0 a000 00b7 d004 62c1 c000 00ff 2504  V.......b.....%.
-00000990: 66ac 6500 0137 a804 7914 8000 00d1 7b04  f.e..7..y.....{.
-000009a0: 7d16 7000 006f 4b04 846c 5400 002b 2e04  }.p..oK..lT..+..
-000009b0: 846c 5400 0082 df04 846c 5400 0089 1604  .lT......lT.....
-000009c0: 846c 5400 0135 bb04 8a9c b300 000a 1404  .lT..5..........
-000009d0: 8a9c b300 0092 ee04 8c2d c700 0065 9504  .........-...e..
-000009e0: 8c2d c700 007c 7404 8e23 4000 0000 c004  .-...|t..#@.....
-000009f0: 8e23 4000 001f e304 8e23 4000 0056 0a04  .#@......#@..V..
-00000a00: 983c 8100 0046 9304 9849 bc00 0008 3504  .<...F...I....5.
-00000a10: 9e16 8200 0102 0d04 9e84 d500 0093 4904  ..............I.
-00000a20: a577 1f00 0067 7c04 a5e2 3000 0099 b404  .w...g|...0.....
-00000a30: ac2c a500 0085 fa04 ac2c a500 00a4 c404  .,.......,......
-00000a40: bebd 0000 00a8 3f04 c840 f000 00e9 dc04  ......?..@......
-00000a50: c840 f000 00ed 1704 c840 f000 010e d404  .@.......@......
-00000a60: cc5c 9400 0028 4e04 cf4d c200 00f8 8704  .\...(N..M......
-00000a70: d5c8 0000 0007 1a04 d7d5 4000 00cb ca04  ..........@.....
-00000a80: dd34 9000 0015 bf04 ee54 4000 010c 3c04  .4.......T@...<.
-00000a90: f6d3 c900 00d4 0005 04e3 1000 0007 9505  ................
-00000aa0: 079c 7300 0123 1105 161e a000 00b5 8305  ..s..#..........
-00000ab0: 2caa 5000 00b3 e105 2cde 2300 00a5 5805  ,.P.....,.#...X.
-00000ac0: 304c 6a00 0049 9805 33ee 2500 0015 5205  0Lj..I..3.%...R.
-00000ad0: 33ee 2500 0036 f405 3c8d c200 0018 7105  3.%..6..<.....q.
-00000ae0: 3c8d c200 001e 8705 3d7b 7000 00e9 7705  <.......={p...w.
-00000af0: 3d7b 7000 00ec b205 3d7b 7000 0103 ee05  ={p.....={p.....
-00000b00: 3d7b 7000 010d f105 49ee 8900 0068 b505  ={p.....I....h..
-00000b10: 4e5b d400 0118 0705 5305 de00 0076 9b05  N[......S....v..
-00000b20: 5316 ce00 0075 7a05 633f 7000 00e5 6505  S....uz.c?p...e.
-00000b30: 6945 5000 00c5 e905 6bc4 2700 008b 2c05  iEP.....k.'...,.
-00000b40: 6bcd a500 00b1 ac05 6c90 5400 0096 7405  k.......l.T...t.
-00000b50: 6ccc 4300 004b 7205 6edf f400 008d e805  l.C..Kr.n.......
-00000b60: 6fe5 c000 00f3 a305 802f 5e00 00b0 e005  o......../^.....
-00000b70: 812d 6000 0101 b005 88a7 e000 0120 f605  .-`.......... ..
-00000b80: 88a8 c000 004d c705 8c6a c300 009f 8405  .....M...j......
-00000b90: 8c6a c300 011a 5005 8cbc 8e00 004b 3c05  .j....P......K<.
-00000ba0: 98ab 6e00 008e 2a05 9ca9 f100 0039 1905  ..n...*......9..
-00000bb0: 9dfd c000 00a7 bf05 9e88 c300 0092 6605  ..............f.
-00000bc0: a661 8700 004d fc05 a661 8700 0051 6905  .a...M...a...Qi.
-00000bd0: a661 8700 0052 1305 a7f1 8700 0054 e105  .a...R.......T..
-00000be0: adfb 2800 00a0 9105 b039 5c00 000b 7b05  ..(......9\...{.
-00000bf0: b039 5c00 011a 8d05 b093 0000 00c7 c305  .9\.............
-00000c00: b247 c400 009b db05 c068 c000 0009 a705  .G.......h......
-00000c10: c1f8 2200 008d 8d05 ced0 2500 00d8 a505  ..".......%.....
-00000c20: d5fa e400 0080 6205 d5fa e400 012b 3805  ......b......+8.
-00000c30: da03 6e00 005d 8805 dce3 0000 00d1 0105  ..n..]..........
-00000c40: dce3 0000 0101 3705 dde3 7900 0060 a105  ......7...y..`..
-00000c50: e1ed 8400 00be 0e05 ecff 1900 00eb ed05  ................
-00000c60: f264 ba00 0047 3305 f662 ea00 00bc 3805  .d...G3..b....8.
-00000c70: facb 8300 0090 d006 0826 4000 00d6 7e06  .........&@...~.
-00000c80: 08e3 9400 007b 8c06 0ab9 9000 00e2 6506  .....{........e.
-00000c90: 129d e000 00df 2606 148d a400 0021 d706  ......&......!..
-00000ca0: 1867 1e00 0099 fe06 215f 7400 0062 d706  .g......!_t..b..
-00000cb0: 2b00 1300 0037 fd06 2b00 1300 0038 8d06  +....7..+....8..
-00000cc0: 2b00 1300 003a 0a06 34af 4a00 0009 d706  +....:..4.J.....
-00000cd0: 3500 0f00 006c 0606 3c17 4000 00dc 7e06  5....l..<.@...~.
-00000ce0: 3c17 4000 00e8 3a06 3c17 4000 00fa 7006  <.@...:.<.@...p.
-00000cf0: 3c17 4000 0113 bd06 3cee 8400 00ab cb06  <.@.....<.......
-00000d00: 468c a000 00b0 7606 4e38 c500 00a1 3206  F.....v.N8....2.
-00000d10: 4f34 c000 0110 af06 53a5 f500 004b 0706  O4......S....K..
-00000d20: 580f ce00 002a 7e06 5a60 a900 00f8 d806  X....*~.Z`......
-00000d30: 6318 9000 00e6 7906 68ee 6400 001c 8b06  c.....y.h.d.....
-00000d40: 69a9 8400 00a3 8306 69b7 0200 012a 3906  i.......i....*9.
-00000d50: 70e2 d000 006f a206 7cd1 c500 004a 2206  p....o..|....J".
-00000d60: 7f33 4700 0032 ad06 8786 ea00 00a2 6406  .3G..2........d.
-00000d70: 88a1 2400 0136 5a06 8f30 5000 011f 4406  ..$..6Z..0P...D.
-00000d80: 9b5a 7700 011b 2606 9bb8 0c00 0038 d406  .Zw...&......8..
-00000d90: 9c50 2000 00c4 2906 9fb2 5300 00fe 5e06  .P ...)...S...^.
-00000da0: a6d5 8300 012d f906 a8dd 9c00 0053 0706  .....-.......S..
-00000db0: aef9 ce00 005a 6a06 afe6 3000 0072 9d06  .....Zj...0..r..
-00000dc0: b017 2200 00a1 d306 b8bb 6000 00a8 c006  ..".......`.....
-00000dd0: c10c 6000 00ce fc06 c215 0a00 0007 ee06  ..`.............
-00000de0: c227 5a00 0029 0b06 c5bd 6a00 0126 7206  .'Z..)....j..&r.
-00000df0: ce8a a100 004c 4406 cf70 9900 0024 f606  .....LD..p...$..
-00000e00: d08b 2a00 00c9 c706 d81c 2e00 00d9 1006  ..*.............
-00000e10: dbaf 2000 00f0 1806 e231 4000 012d 4f06  .. ......1@..-O.
-00000e20: e6c0 4c00 0053 6c07 0120 6600 0020 e707  ..L..Sl.. f.. ..
-00000e30: 0140 6600 0019 e407 0923 2000 0061 e407  .@f......# ..a..
-00000e40: 0ac3 fa00 00a2 2607 0e35 d000 00dc 1e07  ......&..5......
-00000e50: 126c 4400 013a 7807 1d24 9000 0105 d007  .lD..:x..$......
-00000e60: 1db9 0500 0013 7407 3389 e000 00b7 0c07  ......t.3.......
-00000e70: 3c71 f700 000f 6607 449d 1f00 00be 7307  <q....f.D.....s.
-00000e80: 47cf 0400 0040 ba07 4bcf e000 00e8 8a07  G....@..K.......
-00000e90: 5cec 7500 00a0 ee07 62f5 3500 0040 4107  \.u.....b.5..@A.
-00000ea0: 65e8 b400 007f 1007 65e8 b400 0129 9707  e.......e....)..
-00000eb0: 6c21 5400 000b f607 7e9b 0500 00e7 8b07  l!T.....~.......
-00000ec0: 9a56 2000 0070 c107 9a6c 1400 000c a507  .V ..p...l......
-00000ed0: 9a6c 1400 001c 5207 9a6c 1400 0030 3907  .l....R..l...09.
-00000ee0: 9a6c 1400 0052 cf07 9a6c 1400 0082 ac07  .l...R...l......
-00000ef0: 9a6c 1400 0131 0807 9aa9 6000 00cc 6207  .l...1....`...b.
-00000f00: 9db4 9000 00b9 9507 9db4 9000 00fd ea07  ................
-00000f10: 9e2e 7300 0138 4507 a121 8000 0022 ea07  ..s..8E..!..."..
-00000f20: a674 8700 00a3 d607 bdfe de00 002d 9a07  .t...........-..
-00000f30: cf9a 7000 00fc 0a07 d231 3400 0003 9f07  ..p......14.....
-00000f40: daae 0000 0105 6307 dae0 ea00 011e 3507  ......c.......5.
-00000f50: e0a9 5000 000e a107 e0a9 5000 008a 6d07  ..P.......P...m.
-00000f60: e0a9 5000 011c 3d07 ebd7 9e00 00aa ee07  ..P...=.........
-00000f70: ebd7 9e00 00ad d907 ec42 a500 000a c507  .........B......
-00000f80: ed5c 8000 0112 dc07 f3d4 e000 00ca bc07  .\..............
-00000f90: f714 e400 00f9 5908 0291 0000 0081 8908  ......Y.........
-00000fa0: 08a7 9000 00c5 6408 1f02 9000 00b6 ac08  ......d.........
-00000fb0: 283b 1400 00fe b508 284d 4300 0084 d008  (;......(MC.....
-00000fc0: 28e8 e000 00f0 cf08 2a45 4a00 00a4 2108  (.......*EJ...!.
-00000fd0: 2fe7 9000 009e 3208 3267 1100 0008 a008  /.....2.2g......
-00000fe0: 41da 6e00 0086 8808 426e 6000 0116 c208  A.n.....Bn`.....
-00000ff0: 46c5 3a00 0045 f408 4d37 c500 0093 8508  F.:..E..M7......
-00001000: 4e6b 2a00 0047 7b08 4ef9 1500 005c f208  Nk*..G{.N....\..
-00001010: 4fd0 2000 0116 3f08 6186 7000 0071 bb08  O. ...?.a.p..q..
-00001020: 6c71 e200 00ad 7a08 6f32 c000 00da a008  lq....z.o2......
-00001030: 700d f000 00fb 8308 70b2 8b00 0077 2808  p.......p....w(.
-00001040: 7219 0f00 008a a408 7a4a 5000 007a 2208  r.......zJP..z".
-00001050: 8284 d500 000c d608 8284 d500 0083 1308  ................
-00001060: 8599 7200 0137 6f08 8958 2900 012c 7f08  ..r..7o..X)..,..
-00001070: 8b87 0000 00d2 3808 8fa4 9300 0010 9908  ......8.........
-00001080: 8fa4 9300 0086 d608 8fa4 9300 008c d208  ................
-00001090: 8fa4 9300 011a ee08 9a98 b400 001a c808  ................
-000010a0: 9c61 5e00 011e 9008 a1a4 9300 0059 ab08  .a^..........Y..
-000010b0: a63b 3000 010e 5708 aa82 f400 005b 3c08  .;0...W......[<.
-000010c0: abe2 0900 002b 5f08 abe2 0900 0089 4b08  .....+_.......K.
-000010d0: af11 d500 0063 af08 b89a 9200 0026 9208  .....c.......&..
-000010e0: bbfe c500 0002 ac08 bbfe c500 0127 7c08  .............'|.
-000010f0: bd8a 6000 0118 8508 c000 5000 0098 5b08  ..`.......P...[.
-00001100: c000 5000 0099 1e08 c272 0900 0010 d608  ..P......r......
-00001110: c76b 0300 005a b108 cd7c e400 00aa 7e09  .k...Z...|....~.
-00001120: 00f9 a400 0003 e009 162e f000 003b c609  .............;..
-00001130: 1afc d400 003e 7709 1fb9 f500 0076 cd09  .....>w......v..
-00001140: 2254 0000 0122 2409 2e57 df00 00a6 a609  "T..."$..W......
-00001150: 35e6 6000 0049 5509 3b85 e000 006c e509  5.`..IU.;....l..
-00001160: 4459 d000 00e1 d409 4d67 fe00 011a 1009  DY......Mg......
-00001170: 5962 c900 00e7 ca09 5aa4 1000 00ba 9909  Yb......Z.......
-00001180: 5b68 f000 005f 0509 5c07 3000 00ef 6909  [h..._..\.0...i.
-00001190: 5ca2 3000 0132 f009 5d03 9000 0120 8109  \.0..2..].... ..
-000011a0: 6302 2500 0138 1509 667a 9000 00ed a009  c.%..8..fz......
-000011b0: 66cc c900 0034 b109 700b c500 0012 cf09  f....4..p.......
-000011c0: 7a29 6900 0010 1909 8c00 0a00 0051 2309  z)i..........Q#.
-000011d0: 8c81 5e00 003a 4b09 8c81 5e00 0051 c509  ..^..:K...^..Q..
-000011e0: 8c81 5e00 0098 d409 8d04 b300 0090 0709  ..^.............
-000011f0: 95cb c400 00d7 c209 a6af c300 0057 8d09  .............W..
-00001200: a6c1 0a00 0028 9c09 a6c1 0a00 0045 8b09  .....(.......E..
-00001210: a6c1 0a00 0083 fc09 a6c1 0a00 0098 1e09  ................
-00001220: a6c1 0a00 0124 e009 a6c1 c300 0004 6f09  .....$........o.
-00001230: a87a 8000 00fa c709 b56b a200 008d 0b09  .z.......k......
-00001240: b889 ea00 0087 af09 b889 ea00 00a6 0c09  ................
-00001250: cf34 f000 00e1 3f09 d82d 3f00 0084 3309  .4....?..-?...3.
-00001260: dbfe c000 00db 5f0a 074b 5000 0073 040a  ......_..KP..s..
-00001270: 159b 8000 001f 500a 159b 8000 0055 780a  ......P......Ux.
-00001280: 17d3 5000 00cd 200a 20b0 6000 0079 1c0a  ..P... . .`..y..
-00001290: 20fc 9000 00b4 c50a 22d2 d000 00e5 e40a   .......".......
-000012a0: 2aef e000 00fc 950a 2e99 7e00 0057 c50a  *.........~..W..
-000012b0: 30f6 b500 002a d60a 338b 1000 00de a50a  0....*..3.......
-000012c0: 3f0e 9500 0081 110a 3f0e 9500 012c 3e0a  ?.......?....,>.
-000012d0: 4985 3000 0072 290a 4cb2 e000 00b8 500a  I.0..r).L.....P.
-000012e0: 5e50 b000 010b c50a 62cd 3400 0035 6a0a  ^P......b.4..5j.
-000012f0: 64c8 9500 0087 730a 65e3 f000 005e 4a0a  d.....s.e....^J.
-00001300: 6c11 b300 0005 040a 6c5b d900 000a 580a  l.......l[....X.
-00001310: 6c5b d900 000c 3e0a 6c89 9300 0137 d80a  l[....>.l....7..
-00001320: 70ea 0000 0044 f00a 8170 8e00 0133 c70a  p....D...p...3..
-00001330: 84e6 b500 001d 730a 84e6 b500 0030 d10a  ......s......0..
-00001340: 84e6 b500 0053 d80a 84e6 b500 0131 ac0a  .....S.......1..
-00001350: 84e6 b500 0136 1a0a 89ad 3000 00f6 9e0a  .....6....0.....
-00001360: 89ad 3000 010c fe0a 8c5e f000 0066 cd0a  ..0......^...f..
-00001370: 954c 2000 00dc cf0a 9989 6300 0074 6c0a  .L .......c..tl.
-00001380: ac8c c000 00f9 f70a ae3e fa00 0076 130a  .........>...v..
-00001390: b4bc 2e00 002f 9e0a b5ff 6400 00b2 440a  ...../....d...D.
-000013a0: b6d5 d000 00d3 600a ba90 7000 00e8 f80a  ......`...p.....
-000013b0: be20 4a00 0011 1c0a c25d 1400 0042 530a  . J......]...BS.
-000013c0: c945 a000 00b4 380a ca80 7300 0054 1e0a  .E....8...s..T..
-000013d0: cf76 b400 0058 ff0a cfef 4000 0108 430a  .v...X....@...C.
-000013e0: e1b0 da00 00a9 210a e1b4 8000 0115 c60a  ......!.........
-000013f0: e45f d000 00b9 0e0a eb63 2000 0023 870a  ._.......c ..#..
-00001400: ee50 6000 0082 410a f3de 9e00 0085 a10a  .P`...A.........
-00001410: f818 8000 00b8 890a f818 8000 00fd 580b  ..............X.
-00001420: 0396 6300 0009 720b 03f9 7300 008f bd0b  ..c...r...s.....
-00001430: 0476 b400 0059 390b 0ac1 5a00 012b d40b  .v...Y9...Z..+..
-00001440: 139f b500 0087 e70b 19b8 d700 008b ab0b  ................
-00001450: 1b90 b000 0103 000b 1fcd 0500 00a1 8f0b  ................
-00001460: 20ce b000 00c3 970b 2371 ce00 0001 3e0b   .......#q....>.
-00001470: 244d 8300 0107 1f0b 296c c900 0073 fd0b  $M......)l...s..
-00001480: 2d80 be00 000f c70b 2d80 be00 008c 080b  -.......-.......
-00001490: 2d80 be00 011c c40b 2fa8 e400 0132 ac0b  -......./....2..
-000014a0: 4000 a500 0065 120b 440d ae00 005a ea0b  @....e..D....Z..
-000014b0: 47ce c400 00ea d80b 4841 e400 00bd a80b  G.......HA......
-000014c0: 4e26 9900 0011 620b 543a f400 00e3 080b  N&....b.T:......
-000014d0: 5467 9000 002b fd0b 6948 d000 00c6 830b  Tg...+..iH......
-000014e0: 6b4e 3000 005f e80b 6f1b 4500 0062 4d0b  kN0.._..o.E..bM.
-000014f0: 76dd 9d00 0136 a50b 8a1a 2000 00e4 9f0b  v....6.... .....
-00001500: 8a1a 2000 0112 890b 8c6a e300 005a 2c0b  .. ......j...Z,.
-00001510: 9253 4000 0002 280b 94b6 5e00 00d0 490b  .S@...(...^...I.
-00001520: 967b 5400 0032 5c0b a0c9 de00 0006 5c0b  .{T..2\.......\.
-00001530: a3fc 7000 00f2 770b a4a2 2500 0025 690b  ..p...w...%..%i.
-00001540: c474 9000 00dd 6b0b c4a6 f000 0064 9d0b  .t....k......d..
-00001550: c81a a000 00de 0a0b cbf1 c000 00e4 f20b  ................
-00001560: cbf1 c000 00ea 650b cbf1 c000 00f4 ed0b  ......e.........
-00001570: cbf1 c000 010a c80b db2b b200 0026 430b  .........+...&C.
-00001580: def4 0000 012f f50b e203 8700 000f 1f0b  ...../..........
-00001590: e217 6300 000e dc0b e4a0 3000 0016 c50b  ..c.......0.....
-000015a0: f39a 4000 003a ce0b f39a 4000 0081 d20b  ..@..:....@.....
-000015b0: f39a 4000 00ca 4a0b fc32 3300 0046 290c  ..@...J..23..F).
-000015c0: 04fe c500 0014 360c 0c17 6300 0058 530c  ......6...c..XS.
-000015d0: 0ce3 2300 008f 670c 0dec 5a00 0080 af0c  ..#...g...Z.....
-000015e0: 1cdb 4200 010f 5e0c 1d95 4000 00c1 c40c  ..B...^...@.....
-000015f0: 3834 1400 000e 3b0c 3834 1400 008a 0b0c  84....;.84......
-00001600: 3834 1400 011b db0c 5256 ae00 0034 730c  84......RV...4s.
-00001610: 5bd6 a000 0008 670c 61ce a500 0035 240c  [.....g.a....5$.
-00001620: 63ce a500 000b b00c 6dca b800 0038 3e0c  c.......m....8>.
-00001630: 808a a300 00a5 b20c 83b7 b000 0037 c40c  .............7..
-00001640: 8910 0000 0006 9a0c 89ed e500 004a cf0c  .............J..
-00001650: 98c0 0900 0005 e20c 98c0 0900 000a 8e0c  ................
-00001660: 98c0 0900 000d c70c 98c0 0900 0083 4a0c  ..............J.
-00001670: 98c0 0900 0088 d50c 98c0 0900 009f ee0c  ................
-00001680: 98c0 0900 0119 d70c 9fa9 6000 0121 670c  ..........`..!g.
-00001690: b106 9a00 011d e60c b195 2700 007f b80c  ..........'.....
-000016a0: b1a8 e500 0031 4c0c ba9f 2400 0112 0a0c  .....1L...$.....
-000016b0: c1c5 c300 0091 560c c4e1 d500 0014 7f0c  ......V.........
-000016c0: c5f7 d500 007d ad0c c7ee 6000 009c db0c  .....}....`.....
-000016d0: c8e8 6400 0030 970c c9a0 2e00 007e 0c0c  ..d..0.......~..
-000016e0: cba2 d500 00eb ad0c db0c 0400 00b5 350c  ..............5.
-000016f0: dda2 6e00 00b2 b20c e3ed a900 0091 0b0c  ..n.............
-00001700: f3b0 8500 0013 190c fb0f b300 0093 f70d  ................
-00001710: 0027 2000 00c0 970d 09a5 6000 011f 9c0d  .' .......`.....
-00001720: 0a66 ed00 0129 0b0d 0ad7 7300 004d 170d  .f...)....s..M..
-00001730: 0f91 6000 00f1 590d 0f91 6000 0106 840d  ..`...Y...`.....
-00001740: 1201 a400 005c 7b0d 1cec 6700 011d 120d  .....\{...g.....
-00001750: 2d41 7000 00ae f50d 32db 3000 00ed fb0d  -Ap.....2.0.....
-00001760: 35c6 3000 010a 1b0d 3b8c 3900 00ac 750d  5.0.....;.9...u.
-00001770: 48cd 6500 009a cc0d 51bd f000 00f5 670d  H.e.....Q.....g.
-00001780: 69f6 0000 009d 880d 7298 e700 00ae 310d  i.......r.....1.
-00001790: 7c3b 4000 0113 4f0d 80f6 3400 0097 d30d  |;@...O...4.....
-000017a0: 80f6 3400 0099 630d 8344 9300 0090 4d0d  ..4...c..D....M.
-000017b0: 8c46 7500 0004 a70d 8c46 7500 00a6 470d  .Fu......Fu...G.
-000017c0: 96e3 5000 00e0 1e0d 9df1 6500 001a 7d0d  ..P.......e...}.
-000017d0: 9df1 6500 0021 520d 9ee3 5e00 006d 320d  ..e..!R...^..m2.
-000017e0: 9ee3 5e00 0078 a00d 9ee3 5e00 0085 190d  ..^..x....^.....
-000017f0: 9ee3 5e00 00a4 760d 9ee3 5e00 00b7 8c0d  ..^...v...^.....
-00001800: aa4e 9000 00e7 070d c964 7400 00ab 440d  .N.......dt...D.
-00001810: d0e8 e000 00c9 890d ded8 9000 001d ff0d  ................
-00001820: ded8 9000 0054 5a0d eb49 0000 007f f00d  .....TZ..I......
-00001830: ec49 8400 0048 950d f086 4a00 0039 b50d  .I...H....J..9..
-00001840: fcd5 7e00 003f 300d fe0b 6000 0070 060e  ..~..?0...`..p..
-00001850: 00f0 b000 00d5 630e 03af f000 0077 6c0e  ......c......wl.
-00001860: 1bf8 6400 0039 540e 1ddb 6300 0052 6f0e  ..d..9T...c..Ro.
-00001870: 202b 3a00 007e 6b0e 202b 3a00 0128 720e   +:..~k. +:..(r.
-00001880: 20d7 0900 010f ac0e 2511 7400 0060 eb0e   .......%.t..`..
-00001890: 38a0 f000 0107 a40e 5c13 4700 011b 5a0e  8.......\.G...Z.
-000018a0: 6193 e900 0114 7d0e 61d5 0400 00a9 700e  a.....}.a.....p.
-000018b0: 68cb dc00 0057 270e 6ac2 e300 0025 a00e  h....W'.j....%..
-000018c0: 7617 2000 007b dd0e 8347 4400 006a 930e  v. ..{...GD..j..
-000018d0: 887b b500 0037 590e 887b b500 00aa 470e  .{...7Y..{....G.
-000018e0: 9dcc d400 0033 560e a934 c000 0061 6a0e  .....3V..4...aj.
-000018f0: abf5 1300 0068 410e ae34 8000 005e a50e  .....hA..4...^..
-00001900: b4a5 0a00 0064 380e b5c2 8000 009b 2e0e  .....d8.........
-00001910: b803 9900 006e f60e b82d 1000 00f5 fb0e  .....n...-......
-00001920: c28b b000 0003 0c0e d945 de00 002e 560e  .........E....V.
-00001930: e77d 7000 0123 db0e f7f8 4000 00f1 fa0f  .}p..#....@.....
-00001940: 09fd b000 00d7 270f 0cc4 c000 00fd 050f  ......'.........
-00001950: 105e a000 00bb cd0f 11be 6000 00c1 0c0f  .^........`.....
-00001960: 1d28 1000 0100 c70f 201d 8500 0089 8a0f  .(...... .......
-00001970: 20f1 3000 00d9 670f 4321 f500 0134 5e0f   .0...g.C!...4^.
-00001980: 4a90 4000 00b4 7c0f 5e00 1000 00cb 450f  J.@...|.^.....E.
-00001990: 8e7b e000 00cf a70f 9222 7c00 00ac 350f  .{......."|...5.
-000019a0: 9450 0000 0117 2e0f 9ebd c400 0048 ed0f  .P...........H..
-000019b0: 9fbc 6000 0138 e80f a262 9000 013b 5f0f  ..`..8...b...;_.
-000019c0: a44f 0300 0000 5f0f bd5e e700 011c 740f  .O...._..^....t.
-000019d0: cb15 5200 006a 470f cf80 f000 00f7 420f  ..R..jG.......B.
-000019e0: d19a 7000 00c2 7d0f dfeb 7000 009f 190f  ..p...}...p.....
-000019f0: e7f7 9000 013a ed0f ea8a 0900 007e b00f  .....:.......~..
-00001a00: ea8a 0900 00a7 670f ea8a 0900 0128 b10f  ......g......(..
-00001a10: f87c e000 0024 6d0f fe37 0300 0087 1569  .|...$m..7.....i
-00001a20: 0001 3bda 0300 0000 2404 1e04 4204 3c04  ..;.....$...B.<.
-00001a30: 3504 3d04 3804 4204 4c00 2004 3804 3704  5.=.8.B.L. .8.7.
-00001a40: 3c04 3504 3d04 3504 3d04 3804 4f08 0000  <.5.=.5.=.8.O...
-00001a50: 0000 0600 0000 0e43 616e 6365 6c20 6368  .......Cancel ch
-00001a60: 616e 6765 7307 0000 0018 4162 7374 7261  anges.....Abstra
-00001a70: 6374 4f70 6572 6174 696f 6e44 6574 6169  ctOperationDetai
-00001a80: 6c73 0103 0000 0026 0421 043e 0445 0440  ls.....&.!.>.E.@
-00001a90: 0430 043d 0438 0442 044c 0020 0438 0437  .0.=.8.B.L. .8.7
-00001aa0: 043c 0435 043d 0435 043d 0438 044f 0800  .<.5.=.5.=.8.O..
-00001ab0: 0000 0006 0000 000e 436f 6d6d 6974 2063  ........Commit c
-00001ac0: 6861 6e67 6573 0700 0000 1841 6273 7472  hanges.....Abstr
-00001ad0: 6163 744f 7065 7261 7469 6f6e 4465 7461  actOperationDeta
-00001ae0: 696c 7301 0300 0000 3804 1e04 4804 3804  ils.....8...H.8.
-00001af0: 3104 3a04 3000 2004 3f04 4004 3800 2004  1.:.0. .?.@.8. .
-00001b00: 3704 3004 3f04 3804 4104 3800 2004 3e04  7.0.?.8.A.8. .>.
-00001b10: 3f04 3504 4004 3004 4604 3804 3800 3a00  ?.5.@.0.F.8.8.:.
-00001b20: 2008 0000 0000 0600 0000 194f 7065 7261   ..........Opera
-00001b30: 7469 6f6e 2073 7562 6d69 7420 6661 696c  tion submit fail
-00001b40: 6564 3a20 0700 0000 1841 6273 7472 6163  ed: .....Abstrac
-00001b50: 744f 7065 7261 7469 6f6e 4465 7461 696c  tOperationDetail
-00001b60: 7301 0300 0000 8804 1d04 3504 4104 3e04  s.........5.A.>.
-00001b70: 4504 4004 3004 3d04 5104 3d04 3d04 4b04  E.@.0.=.Q.=.=.K.
-00001b80: 3500 2004 3804 3704 3c04 3504 3d04 3504  5. .8.7.<.5.=.5.
-00001b90: 3d04 3804 4f00 2004 3104 4b04 3b04 3800  =.8.O. .1.K.;.8.
-00001ba0: 2004 3e04 4204 3c04 3504 3d04 3504 3d04   .>.B.<.5.=.5.=.
-00001bb0: 4b00 2004 3f04 3504 4004 3504 3400 2004  K. .?.5.@.5.4. .
-00001bc0: 4104 3e04 3704 3404 3004 3d04 3804 3504  A.>.7.4.0.=.8.5.
-00001bd0: 3c00 2004 3d04 3e04 3204 3e04 3900 2004  <. .=.>.2.>.9. .
-00001be0: 3e04 3f04 3504 4004 3004 4604 3804 3808  >.?.5.@.0.F.8.8.
-00001bf0: 0000 0000 0600 0000 3555 6e73 6176 6564  ........5Unsaved
-00001c00: 2063 6861 6e67 6573 2077 6572 6520 7265   changes were re
-00001c10: 7665 7274 6564 2074 6f20 6372 6561 7465  verted to create
-00001c20: 206e 6577 206f 7065 7261 7469 6f6e 0700   new operation..
-00001c30: 0000 1841 6273 7472 6163 744f 7065 7261  ...AbstractOpera
-00001c40: 7469 6f6e 4465 7461 696c 7301 0300 0000  tionDetails.....
-00001c50: 3a04 1d04 3504 3204 3504 4004 3d04 3e04  :...5.2.5.@.=.>.
-00001c60: 3500 2004 3704 3d04 3004 4704 3504 3d04  5. .7.=.0.G.5.=.
-00001c70: 3804 3500 2004 3200 2004 4104 4204 3e04  8.5. .2. .A.B.>.
-00001c80: 3b04 3104 4604 3500 3a00 2008 0000 0000  ;.1.F.5.:. .....
-00001c90: 0600 0000 1b43 6f6c 756d 6e20 6861 7320  .....Column has 
-00001ca0: 6e6f 2076 616c 6964 2076 616c 7565 3a20  no valid value: 
-00001cb0: 0700 0000 1a41 6273 7472 6163 7452 6566  .....AbstractRef
-00001cc0: 6572 656e 6365 4c69 7374 4d6f 6465 6c01  erenceListModel.
-00001cd0: 0300 0000 1e04 1d04 3504 3f04 3e04 3b04  ........5.?.>.;.
-00001ce0: 3d04 4b04 3500 2004 3404 3004 3d04 3d04  =.K.5. .4.0.=.=.
-00001cf0: 4b04 3508 0000 0000 0600 0000 1344 6174  K.5..........Dat
-00001d00: 6120 6172 6520 696e 636f 6d70 6c65 7465  a are incomplete
-00001d10: 0700 0000 1a41 6273 7472 6163 7452 6566  .....AbstractRef
-00001d20: 6572 656e 6365 4c69 7374 4d6f 6465 6c01  erenceListModel.
-00001d30: 0300 0000 2604 1e04 4804 3804 3104 3a04  ....&...H.8.1.:.
-00001d40: 3000 2004 4104 3e04 4504 4004 3004 3d04  0. .A.>.E.@.0.=.
-00001d50: 3504 3d04 3804 4f00 3a00 2008 0000 0000  5.=.8.O.:. .....
-00001d60: 0600 0000 0f53 7562 6d69 7420 6661 696c  .....Submit fail
-00001d70: 6564 3a20 0700 0000 1a41 6273 7472 6163  ed: .....Abstrac
-00001d80: 7452 6566 6572 656e 6365 4c69 7374 4d6f  tReferenceListMo
-00001d90: 6465 6c01 0300 0000 0a04 1b04 4e04 3104  del.........N.1.
-00001da0: 3e04 3908 0000 0000 0600 0000 0341 4e59  >.9..........ANY
-00001db0: 0700 0000 0d41 6363 6f75 6e74 4275 7474  .....AccountButt
-00001dc0: 6f6e 0103 0000 0014 041b 044e 0431 043e  on.........N.1.>
-00001dd0: 0439 0020 0441 0447 0435 0442 0800 0000  .9. .A.G.5.B....
-00001de0: 0006 0000 000b 416e 7920 6163 636f 756e  ......Any accoun
-00001df0: 7407 0000 000d 4163 636f 756e 7442 7574  t.....AccountBut
-00001e00: 746f 6e01 0300 0000 1804 1204 4b04 3104  ton.........K.1.
-00001e10: 4004 3004 4204 4c00 2004 4104 4704 3504  @.0.B.L. .A.G.5.
-00001e20: 4208 0000 0000 0600 0000 0e43 686f 6f73  B..........Choos
-00001e30: 6520 6163 636f 756e 7407 0000 000d 4163  e account.....Ac
-00001e40: 636f 756e 7442 7574 746f 6e01 0300 0000  countButton.....
-00001e50: 1404 2204 3804 3f00 2004 4104 4704 3504  ..".8.?. .A.G.5.
-00001e60: 4204 3000 3a08 0000 0000 0600 0000 0d41  B.0.:..........A
-00001e70: 6363 6f75 6e74 2074 7970 653a 0700 0000  ccount type:....
-00001e80: 1141 6363 6f75 6e74 4c69 7374 4469 616c  .AccountListDial
-00001e90: 6f67 0103 0000 000a 0421 0447 0435 0442  og.......!.G.5.B
-00001ea0: 0430 0800 0000 0006 0000 0008 4163 636f  .0..........Acco
-00001eb0: 756e 7473 0700 0000 1141 6363 6f75 6e74  unts.....Account
-00001ec0: 4c69 7374 4469 616c 6f67 0103 0000 002a  ListDialog.....*
-00001ed0: 041f 043e 043a 0430 0437 044b 0432 0430  ...>.:.0.7.K.2.0
-00001ee0: 0442 044c 0020 043d 0435 0430 043a 0442  .B.L. .=.5.0.:.B
-00001ef0: 0438 0432 043d 044b 0435 0800 0000 0006  .8.2.=.K.5......
-00001f00: 0000 000d 5368 6f77 2069 6e61 6374 6976  ....Show inactiv
-00001f10: 6507 0000 0011 4163 636f 756e 744c 6973  e.....AccountLis
-00001f20: 7444 6961 6c6f 6701 0300 0000 0e21 1600  tDialog......!..
-00001f30: 2004 4104 4704 3504 4204 3008 0000 0000   .A.G.5.B.0.....
-00001f40: 0600 0000 0941 6363 6f75 6e74 2023 0700  .....Account #..
-00001f50: 0000 1041 6363 6f75 6e74 4c69 7374 4d6f  ...AccountListMo
-00001f60: 6465 6c01 0300 0000 0804 1004 3a04 4200  del.........:.B.
-00001f70: 2e08 0000 0000 0600 0000 0441 6374 2e07  ...........Act..
-00001f80: 0000 0010 4163 636f 756e 744c 6973 744d  ....AccountListM
-00001f90: 6f64 656c 0103 0000 0016 0411 0430 043d  odel.........0.=
-00001fa0: 043a 002f 0411 0440 043e 043a 0435 0440  .:./...@.>.:.5.@
-00001fb0: 0800 0000 0006 0000 000b 4261 6e6b 2f42  ..........Bank/B
-00001fc0: 726f 6b65 7207 0000 0010 4163 636f 756e  roker.....Accoun
-00001fd0: 744c 6973 744d 6f64 656c 0103 0000 0004  tListModel......
-00001fe0: 041a 0421 0800 0000 0006 0000 0002 4343  ...!..........CC
-00001ff0: 0700 0000 1041 6363 6f75 6e74 4c69 7374  .....AccountList
-00002000: 4d6f 6465 6c01 0300 0000 0c04 1204 3004  Model.........0.
-00002010: 3b04 4e04 4204 3008 0000 0000 0600 0000  ;.N.B.0.........
-00002020: 0843 7572 7265 6e63 7907 0000 0010 4163  .Currency.....Ac
-00002030: 636f 756e 744c 6973 744d 6f64 656c 0103  countListModel..
-00002040: 0000 0018 041d 0430 0438 043c 0435 043d  .......0.8.<.5.=
-00002050: 043e 0432 0430 043d 0438 0435 0800 0000  .>.2.0.=.8.5....
-00002060: 0006 0000 0004 4e61 6d65 0700 0000 1041  ......Name.....A
-00002070: 6363 6f75 6e74 4c69 7374 4d6f 6465 6c01  ccountListModel.
-00002080: 0300 0000 1004 2204 3e04 4704 3d04 3e04  ......".>.G.=.>.
-00002090: 4104 4204 4c08 0000 0000 0600 0000 0950  A.B.L..........P
-000020a0: 7265 6369 7369 6f6e 0700 0000 1041 6363  recision.....Acc
-000020b0: 6f75 6e74 4c69 7374 4d6f 6465 6c01 0300  ountListModel...
-000020c0: 0000 1004 2104 3204 3504 4004 3504 3d00  ....!.2.5.@.5.=.
-000020d0: 2000 4008 0000 0000 0600 0000 0c52 6563   .@..........Rec
-000020e0: 6f6e 6369 6c65 6420 4007 0000 0010 4163  onciled @.....Ac
-000020f0: 636f 756e 744c 6973 744d 6f64 656c 0103  countListModel..
-00002100: 0000 001a 0426 0435 043d 043d 0430 044f  .....&.5.=.=.0.O
-00002110: 0020 0431 0443 043c 0430 0433 0430 0800  . .1.C.<.0.3.0..
-00002120: 0000 0006 0000 0005 4173 7365 7407 0000  ........Asset...
-00002130: 000b 4173 7365 7444 6961 6c6f 6701 0300  ..AssetDialog...
-00002140: 0000 3e04 1e04 4804 3804 3104 3a04 3000  ..>...H.8.1.:.0.
-00002150: 2004 3704 3004 3f04 3804 4104 3800 2004   .7.0.?.8.A.8. .
-00002160: 3804 3d04 4404 3e04 4004 3c04 3004 4604  8.=.D.>.@.<.0.F.
-00002170: 3804 3800 2004 3e00 2004 2604 1100 3a00  8.8. .>. .&...:.
-00002180: 2008 0000 0000 0600 0000 1d41 7373 6574   ..........Asset
-00002190: 2064 6574 6169 6c73 2073 7562 6d69 7420   details submit 
-000021a0: 6661 696c 6564 3a20 0700 0000 0b41 7373  failed: .....Ass
-000021b0: 6574 4469 616c 6f67 0103 0000 0024 041e  etDialog.....$..
-000021c0: 0448 0438 0431 043a 0430 0020 0437 0430  .H.8.1.:.0. .7.0
-000021d0: 043f 0438 0441 0438 0020 0426 0415 003a  .?.8.A.8. .&...:
-000021e0: 0020 0800 0000 0006 0000 0015 4173 7365  . ..........Asse
-000021f0: 7420 7375 626d 6974 2066 6169 6c65 643a  t submit failed:
-00002200: 2007 0000 000b 4173 7365 7444 6961 6c6f   .....AssetDialo
-00002210: 6701 0300 0000 1c04 1104 3004 3704 3e04  g.........0.7.>.
-00002220: 3204 4b04 3900 2004 3004 3a04 4204 3804  2.K.9. .0.:.B.8.
-00002230: 3200 3a08 0000 0000 0600 0000 0b42 6173  2.:..........Bas
-00002240: 6520 6173 7365 743a 0700 0000 0b41 7373  e asset:.....Ass
-00002250: 6574 4469 616c 6f67 0103 0000 000c 041e  etDialog........
-00002260: 0442 043c 0435 043d 0430 0800 0000 0006  .B.<.5.=.0......
-00002270: 0000 0006 4361 6e63 656c 0700 0000 0b41  ....Cancel.....A
-00002280: 7373 6574 4469 616c 6f67 0103 0000 0010  ssetDialog......
-00002290: 0421 0442 0440 0430 043d 0430 003a 0020  .!.B.@.0.=.0.:. 
-000022a0: 0800 0000 0006 0000 0009 436f 756e 7472  ..........Countr
-000022b0: 793a 2007 0000 000b 4173 7365 7444 6961  y: .....AssetDia
-000022c0: 6c6f 6701 0300 0000 1404 1404 3e04 3f00  log.........>.?.
-000022d0: 2e04 3404 3004 3d04 3d04 4b04 3508 0000  ..4.0.=.=.K.5...
-000022e0: 0000 0600 0000 0a45 7874 7261 2064 6174  .......Extra dat
-000022f0: 6107 0000 000b 4173 7365 7444 6961 6c6f  a.....AssetDialo
-00002300: 6701 0300 0000 0a00 4900 5300 4900 4e00  g.......I.S.I.N.
-00002310: 3a08 0000 0000 0600 0000 0549 5349 4e3a  :..........ISIN:
-00002320: 0700 0000 0b41 7373 6574 4469 616c 6f67  .....AssetDialog
-00002330: 0103 0000 001a 041d 0430 0438 043c 0435  .........0.8.<.5
-00002340: 043d 043e 0432 0430 043d 0438 0435 003a  .=.>.2.0.=.8.5.:
-00002350: 0800 0000 0006 0000 0005 4e61 6d65 3a07  ..........Name:.
-00002360: 0000 000b 4173 7365 7444 6961 6c6f 6701  ....AssetDialog.
-00002370: 0300 0000 0404 1e04 1a08 0000 0000 0600  ................
-00002380: 0000 024f 4b07 0000 000b 4173 7365 7444  ...OK.....AssetD
-00002390: 6961 6c6f 6701 0300 0000 0e04 2104 3804  ialog.......!.8.
-000023a0: 3c04 3204 3e04 3b04 4b08 0000 0000 0600  <.2.>.;.K.......
-000023b0: 0000 0753 796d 626f 6c73 0700 0000 0b41  ...Symbols.....A
-000023c0: 7373 6574 4469 616c 6f67 0103 0000 000a  ssetDialog......
-000023d0: 0422 0438 043f 003a 0020 0800 0000 0006  .".8.?.:. ......
-000023e0: 0000 0006 5479 7065 3a20 0700 0000 0b41  ....Type: .....A
-000023f0: 7373 6574 4469 616c 6f67 0103 0000 000e  ssetDialog......
-00002400: 0422 0438 043f 0020 0426 0411 003a 0800  .".8.?. .&...:..
-00002410: 0000 0006 0000 000b 4173 7365 7420 7479  ........Asset ty
-00002420: 7065 3a07 0000 000f 4173 7365 744c 6973  pe:.....AssetLis
-00002430: 7444 6961 6c6f 6701 0300 0000 1a04 2604  tDialog.......&.
-00002440: 3504 3d04 3d04 4b04 3500 2004 3104 4304  5.=.=.K.5. .1.C.
-00002450: 3c04 3004 3304 3808 0000 0000 0600 0000  <.0.3.8.........
-00002460: 0641 7373 6574 7307 0000 000f 4173 7365  .Assets.....Asse
-00002470: 744c 6973 7444 6961 6c6f 6701 0300 0000  tListDialog.....
-00002480: 0c04 2104 4204 4004 3004 3d04 3008 0000  ..!.B.@.0.=.0...
-00002490: 0000 0600 0000 0743 6f75 6e74 7279 0700  .......Country..
-000024a0: 0000 0e41 7373 6574 4c69 7374 4d6f 6465  ...AssetListMode
-000024b0: 6c01 0300 0000 0c04 1204 3004 3b04 4e04  l.........0.;.N.
-000024c0: 4204 3008 0000 0000 0600 0000 0843 7572  B.0..........Cur
-000024d0: 7265 6e63 7907 0000 000e 4173 7365 744c  rency.....AssetL
-000024e0: 6973 744d 6f64 656c 0103 0000 001a 0418  istModel........
-000024f0: 0441 0442 002e 043a 043e 0442 0438 0440  .A.B...:.>.B.8.@
-00002500: 043e 0432 043e 043a 0800 0000 0006 0000  .>.2.>.:........
-00002510: 000b 4461 7461 2073 6f75 7263 6507 0000  ..Data source...
-00002520: 000e 4173 7365 744c 6973 744d 6f64 656c  ..AssetListModel
-00002530: 0103 0000 0008 0049 0053 0049 004e 0800  .......I.S.I.N..
-00002540: 0000 0006 0000 0004 4953 494e 0700 0000  ........ISIN....
-00002550: 0e41 7373 6574 4c69 7374 4d6f 6465 6c01  .AssetListModel.
-00002560: 0300 0000 1804 1d04 3004 3804 3c04 3504  ........0.8.<.5.
-00002570: 3d04 3e04 3204 3004 3d04 3804 3508 0000  =.>.2.0.=.8.5...
-00002580: 0000 0600 0000 044e 616d 6507 0000 000e  .......Name.....
-00002590: 4173 7365 744c 6973 744d 6f64 656c 0103  AssetListModel..
-000025a0: 0000 000c 0421 0438 043c 0432 043e 043b  .....!.8.<.2.>.;
-000025b0: 0800 0000 0006 0000 0006 5379 6d62 6f6c  ..........Symbol
-000025c0: 0700 0000 0e41 7373 6574 4c69 7374 4d6f  .....AssetListMo
-000025d0: 6465 6c01 0300 0000 1804 1d04 3004 3804  del.........0.8.
-000025e0: 3c04 3504 3d04 3e04 3204 3004 3d04 3804  <.5.=.>.2.0.=.8.
-000025f0: 3508 0000 0000 0600 0000 0a41 7373 6574  5..........Asset
-00002600: 206e 616d 6507 0000 000f 4173 7365 7473   name.....Assets
-00002610: 4c69 7374 4d6f 6465 6c01 0300 0000 1a04  ListModel.......
-00002620: 1104 3004 3704 3e04 3204 4b04 3900 2004  ..0.7.>.2.K.9. .
-00002630: 3004 3a04 4204 3804 3208 0000 0000 0600  0.:.B.8.2.......
-00002640: 0000 0a42 6173 6520 6173 7365 7407 0000  ...Base asset...
-00002650: 000f 4173 7365 7473 4c69 7374 4d6f 6465  ..AssetsListMode
-00002660: 6c01 0300 0000 0c04 2104 4204 4004 3004  l.......!.B.@.0.
-00002670: 3d04 3008 0000 0000 0600 0000 0743 6f75  =.0..........Cou
-00002680: 6e74 7279 0700 0000 0f41 7373 6574 734c  ntry.....AssetsL
-00002690: 6973 744d 6f64 656c 0103 0000 0008 0049  istModel.......I
-000026a0: 0053 0049 004e 0800 0000 0006 0000 0004  .S.I.N..........
-000026b0: 4953 494e 0700 0000 0f41 7373 6574 734c  ISIN.....AssetsL
-000026c0: 6973 744d 6f64 656c 0103 0000 0008 0421  istModel.......!
-000026d0: 0447 0435 0442 0800 0000 0006 0000 0007  .G.5.B..........
-000026e0: 4163 636f 756e 7407 0000 000d 4261 6c61  Account.....Bala
-000026f0: 6e63 6573 4d6f 6465 6c01 0300 0000 0c04  ncesModel.......
-00002700: 1104 3004 3b04 3004 3d04 4108 0000 0000  ..0.;.0.=.A.....
-00002710: 0600 0000 0742 616c 616e 6365 0700 0000  .....Balance....
-00002720: 0d42 616c 616e 6365 734d 6f64 656c 0103  .BalancesModel..
-00002730: 0000 0010 0411 0430 043b 0430 043d 0441  .......0.;.0.=.A
-00002740: 002c 0020 0800 0000 0006 0000 0009 4261  .,. ..........Ba
-00002750: 6c61 6e63 652c 2007 0000 000d 4261 6c61  lance, .....Bala
-00002760: 6e63 6573 4d6f 6465 6c01 0300 0000 0a04  ncesModel.......
-00002770: 1804 4204 3e04 3304 3e08 0000 0000 0600  ..B.>.3.>.......
-00002780: 0000 0554 6f74 616c 0700 0000 0d42 616c  ...Total.....Bal
-00002790: 616e 6365 734d 6f64 656c 0103 0000 001c  ancesModel......
-000027a0: 0411 0430 0437 043e 0432 0430 044f 0020  ...0.7.>.2.0.O. 
-000027b0: 0432 0430 043b 044e 0442 0430 0800 0000  .2.0.;.N.B.0....
-000027c0: 0006 0000 000d 4261 7365 2063 7572 7265  ......Base curre
-000027d0: 6e63 7907 0000 0012 4261 7365 4375 7272  ncy.....BaseCurr
-000027e0: 656e 6379 4469 616c 6f67 0103 0000 000c  encyDialog......
-000027f0: 0412 0430 043b 044e 0442 0430 0800 0000  ...0.;.N.B.0....
-00002800: 0006 0000 0008 4375 7272 656e 6379 0700  ......Currency..
-00002810: 0000 1542 6173 6543 7572 7265 6e63 794c  ...BaseCurrencyL
-00002820: 6973 744d 6f64 656c 0103 0000 0008 0414  istModel........
-00002830: 0430 0442 0430 0800 0000 0006 0000 0004  .0.B.0..........
-00002840: 4461 7465 0700 0000 1542 6173 6543 7572  Date.....BaseCur
-00002850: 7265 6e63 794c 6973 744d 6f64 656c 0103  rencyListModel..
-00002860: 0000 0024 0027 0020 0437 0430 043c 0435  ...$.'. .7.0.<.5
-00002870: 043d 0435 043d 0430 0020 0443 0441 043f  .=.5.=.0. .C.A.?
-00002880: 0435 0448 043d 043e 0800 0000 0006 0000  .5.H.=.>........
-00002890: 001b 2720 7761 7320 7375 6363 6573 7366  ..' was successf
-000028a0: 756c 6c79 2072 6570 6c61 6365 6407 0000  ully replaced...
-000028b0: 0012 4361 7465 676f 7279 4c69 7374 4469  ..CategoryListDi
-000028c0: 616c 6f67 0103 0000 000c 0027 0020 043d  alog.......'. .=
-000028d0: 0430 003a 0020 0800 0000 0006 0000 0008  .0.:. ..........
-000028e0: 2720 7769 7468 3a20 0700 0000 1243 6174  ' with: .....Cat
-000028f0: 6567 6f72 794c 6973 7444 6961 6c6f 6701  egoryListDialog.
-00002900: 0300 0000 1204 1a04 3004 4204 3504 3304  ........0.B.5.3.
-00002910: 3e04 4004 3804 3808 0000 0000 0600 0000  >.@.8.8.........
-00002920: 0a43 6174 6567 6f72 6965 7307 0000 0012  .Categories.....
-00002930: 4361 7465 676f 7279 4c69 7374 4469 616c  CategoryListDial
-00002940: 6f67 0103 0000 0016 041a 0430 0442 0435  og.........0.B.5
-00002950: 0433 043e 0440 0438 044f 0020 0027 0800  .3.>.@.8.O. .'..
-00002960: 0000 0006 0000 000a 4361 7465 676f 7279  ........Category
-00002970: 2027 0700 0000 1243 6174 6567 6f72 794c   '.....CategoryL
-00002980: 6973 7444 6961 6c6f 6701 0300 0000 2804  istDialog.....(.
-00002990: 1704 3004 3c04 3504 3d04 3804 4204 4c00  ..0.<.5.=.8.B.L.
-000029a0: 2004 3a04 3004 4204 3504 3304 3e04 4004   .:.0.B.5.3.>.@.
-000029b0: 3804 4e00 2000 2708 0000 0000 0600 0000  8.N. .'.........
-000029c0: 1252 6570 6c61 6365 2063 6174 6567 6f72  .Replace categor
-000029d0: 7920 2707 0000 0012 4361 7465 676f 7279  y '.....Category
-000029e0: 4c69 7374 4469 616c 6f67 0103 0000 001c  ListDialog......
-000029f0: 0417 0430 043c 0435 043d 0438 0442 044c  ...0.<.5.=.8.B.L
-00002a00: 0020 043d 0430 002e 002e 002e 0800 0000  . .=.0..........
-00002a10: 0006 0000 000f 5265 706c 6163 6520 7769  ......Replace wi
-00002a20: 7468 2e2e 2e07 0000 0012 4361 7465 676f  th........Catego
-00002a30: 7279 4c69 7374 4469 616c 6f67 0103 0000  ryListDialog....
-00002a40: 003c 041f 043e 043a 0430 0437 0430 0442  .<...>.:.0.7.0.B
-00002a50: 044c 0020 043e 043f 0435 0440 0430 0446  .L. .>.?.5.@.0.F
-00002a60: 0438 0438 0020 0441 0020 041a 0430 0442  .8.8. .A. ...0.B
-00002a70: 0435 0433 043e 0440 0438 0435 0439 0800  .5.3.>.@.8.5.9..
-00002a80: 0000 0006 0000 001d 5368 6f77 206f 7065  ........Show ope
-00002a90: 7261 7469 6f6e 7320 7769 7468 2043 6174  rations with Cat
-00002aa0: 6567 6f72 7907 0000 0012 4361 7465 676f  egory.....Catego
-00002ab0: 7279 4c69 7374 4469 616c 6f67 0103 0000  ryListDialog....
-00002ac0: 0010 041e 043f 0435 0440 0430 0446 0438  .....?.5.@.0.F.8
-00002ad0: 0438 0800 0000 0006 0000 000a 4f70 6572  .8..........Oper
-00002ae0: 6174 696f 6e73 0700 0000 0e43 6174 6567  ations.....Categ
-00002af0: 6f72 7952 6570 6f72 7401 0300 0000 1804  oryReport.......
-00002b00: 3f04 3e00 2004 1a04 3004 4204 3504 3304  ?.>. ...0.B.5.3.
-00002b10: 3e04 4004 3804 3808 0000 0000 0600 0000  >.@.8.8.........
-00002b20: 0b62 7920 4361 7465 676f 7279 0700 0000  .by Category....
-00002b30: 0e43 6174 6567 6f72 7952 6570 6f72 7401  .CategoryReport.
-00002b40: 0300 0000 1404 1a04 3004 4204 3504 3304  ........0.B.5.3.
-00002b50: 3e04 4004 3804 4f00 3a08 0000 0000 0600  >.@.8.O.:.......
-00002b60: 0000 0943 6174 6567 6f72 793a 0700 0000  ...Category:....
-00002b70: 1443 6174 6567 6f72 7952 6570 6f72 7457  .CategoryReportW
-00002b80: 6964 6765 7401 0300 0000 2404 1e04 4204  idget.....$...B.
-00002b90: 4704 5104 4200 2004 3f04 3e00 2004 3a04  G.Q.B. .?.>. .:.
-00002ba0: 3004 4204 3504 3304 3e04 4004 3804 3808  0.B.5.3.>.@.8.8.
-00002bb0: 0000 0000 0600 0000 1252 6570 6f72 7420  .........Report 
-00002bc0: 6279 2063 6174 6567 6f72 7907 0000 0014  by category.....
-00002bd0: 4361 7465 676f 7279 5265 706f 7274 5769  CategoryReportWi
-00002be0: 6467 6574 0103 0000 0018 041d 0430 0438  dget.........0.8
-00002bf0: 043c 0435 043d 043e 0432 0430 043d 0438  .<.5.=.>.2.0.=.8
-00002c00: 0435 0800 0000 0006 0000 0004 4e61 6d65  .5..........Name
-00002c10: 0700 0000 1143 6174 6567 6f72 7954 7265  .....CategoryTre
-00002c20: 654d 6f64 656c 0103 0000 000c 0427 0430  eModel.......'.0
-00002c30: 0441 0442 0430 044f 0800 0000 0006 0000  .A.B.0.O........
-00002c40: 0005 4f66 7465 6e07 0000 0011 4361 7465  ..Often.....Cate
-00002c50: 676f 7279 5472 6565 4d6f 6465 6c01 0300  goryTreeModel...
-00002c60: 0000 2004 1304 4004 3004 4404 3804 3a00  .. ...@.0.D.8.:.
-00002c70: 2004 4604 3504 3d04 4b00 2004 3404 3b04   .F.5.=.K. .4.;.
-00002c80: 4f00 2008 0000 0000 0600 0000 1050 7269  O. ..........Pri
-00002c90: 6365 2063 6861 7274 2066 6f72 2007 0000  ce chart for ...
-00002ca0: 000b 4368 6172 7457 696e 646f 7701 0300  ..ChartWindow...
-00002cb0: 0000 1a04 2604 3504 3d04 3d04 3004 4f00  ....&.5.=.=.0.O.
-00002cc0: 2004 3104 4304 3c04 3004 3304 3008 0000   .1.C.<.0.3.0...
-00002cd0: 0000 0600 0000 0541 7373 6574 0700 0000  .......Asset....
-00002ce0: 1143 6c6f 7365 6454 7261 6465 734d 6f64  .ClosedTradesMod
-00002cf0: 656c 0103 0000 001a 0414 0430 0442 0430  el.........0.B.0
-00002d00: 0020 0437 0430 043a 0440 044b 0442 0438  . .7.0.:.@.K.B.8
-00002d10: 044f 0800 0000 0006 0000 000a 436c 6f73  .O..........Clos
-00002d20: 6520 4461 7465 0700 0000 1143 6c6f 7365  e Date.....Close
-00002d30: 6454 7261 6465 734d 6f64 656c 0103 0000  dTradesModel....
-00002d40: 0026 0414 0430 0442 0430 002f 0432 0440  .&...0.B.0./.2.@
-00002d50: 0435 043c 044f 0020 0437 0430 043a 0440  .5.<.O. .7.0.:.@
-00002d60: 044b 0442 0438 044f 0800 0000 0006 0000  .K.B.8.O........
-00002d70: 000f 436c 6f73 6520 4461 7465 2f54 696d  ..Close Date/Tim
-00002d80: 6507 0000 0011 436c 6f73 6564 5472 6164  e.....ClosedTrad
-00002d90: 6573 4d6f 6465 6c01 0300 0000 1a04 2604  esModel.......&.
-00002da0: 3504 3d04 3000 2004 3704 3004 3a04 4004  5.=.0. .7.0.:.@.
-00002db0: 4b04 4204 3804 4f08 0000 0000 0600 0000  K.B.8.O.........
-00002dc0: 0b43 6c6f 7365 2050 7269 6365 0700 0000  .Close Price....
-00002dd0: 1143 6c6f 7365 6454 7261 6465 734d 6f64  .ClosedTradesMod
-00002de0: 656c 0103 0000 0010 041a 043e 043c 0438  el.........>.<.8
-00002df0: 0441 0441 0438 044f 0800 0000 0006 0000  .A.A.8.O........
-00002e00: 0003 4665 6507 0000 0011 436c 6f73 6564  ..Fee.....Closed
-00002e10: 5472 6164 6573 4d6f 6465 6c01 0300 0000  TradesModel.....
-00002e20: 1404 1f04 4004 3804 3c04 3504 4704 3004  ....@.8.<.5.G.0.
-00002e30: 3d04 3804 3508 0000 0000 0600 0000 044e  =.8.5..........N
-00002e40: 6f74 6507 0000 0011 436c 6f73 6564 5472  ote.....ClosedTr
-00002e50: 6164 6573 4d6f 6465 6c01 0300 0000 1a04  adesModel.......
-00002e60: 1404 3004 4204 3000 2004 3e04 4204 3a04  ..0.B.0. .>.B.:.
-00002e70: 4004 4b04 4204 3804 4f08 0000 0000 0600  @.K.B.8.O.......
-00002e80: 0000 094f 7065 6e20 4461 7465 0700 0000  ...Open Date....
-00002e90: 1143 6c6f 7365 6454 7261 6465 734d 6f64  .ClosedTradesMod
-00002ea0: 656c 0103 0000 0026 0414 0430 0442 0430  el.....&...0.B.0
-00002eb0: 002f 0412 0440 0435 043c 044f 0020 043e  ./...@.5.<.O. .>
-00002ec0: 0442 043a 0440 044b 0442 0438 044f 0800  .B.:.@.K.B.8.O..
-00002ed0: 0000 0006 0000 000e 4f70 656e 2044 6174  ........Open Dat
-00002ee0: 652f 5469 6d65 0700 0000 1143 6c6f 7365  e/Time.....Close
-00002ef0: 6454 7261 6465 734d 6f64 656c 0103 0000  dTradesModel....
-00002f00: 001a 0426 0435 043d 0430 0020 043e 0442  ...&.5.=.0. .>.B
-00002f10: 043a 0440 044b 0442 0438 044f 0800 0000  .:.@.K.B.8.O....
-00002f20: 0006 0000 000a 4f70 656e 2050 7269 6365  ......Open Price
-00002f30: 0700 0000 1143 6c6f 7365 6454 7261 6465  .....ClosedTrade
-00002f40: 734d 6f64 656c 0103 0000 0006 041f 0438  sModel.........8
-00002f50: 0423 0800 0000 0006 0000 0003 502f 4c07  .#..........P/L.
-00002f60: 0000 0011 436c 6f73 6564 5472 6164 6573  ....ClosedTrades
-00002f70: 4d6f 6465 6c01 0300 0000 0c04 1f04 3804  Model.........8.
-00002f80: 2300 2c00 2000 2508 0000 0000 0600 0000  #.,. .%.........
-00002f90: 0650 2f4c 2c20 2507 0000 0011 436c 6f73  .P/L, %.....Clos
+00000030: 0000 2300 0132 3b00 0000 2300 0136 eb00  ..#..2;...#..6..
+00000040: 0000 2500 0091 9500 0004 7300 0005 b700  ..%.......s.....
+00000050: 0005 3b00 0009 4c00 0005 af00 0138 9c00  ..;...L......8..
+00000060: 0007 db00 00a8 7200 0031 0e00 007d 3900  ......r..1...}9.
+00000070: 0031 0e00 0126 0f00 0046 3900 0003 7000  .1...&...F9...p.
+00000080: 0046 3900 00a2 0000 0047 a400 0045 bf00  .F9......G...E..
+00000090: 0048 7200 0091 bc00 0048 7200 00a6 6200  .Hr......Hr...b.
+000000a0: 0048 b700 0092 1700 0048 b700 00a6 8e00  .H.......H......
+000000b0: 004a 7a00 0047 bd00 004a b300 0092 c500  .Jz..G...J......
+000000c0: 004a b300 00a6 ba00 004b 1a00 0047 e800  .J.......K...G..
+000000d0: 004b 3a00 0048 1300 004c b200 0093 3100  .K:..H...L....1.
+000000e0: 004c b200 00a6 e600 004c b500 0013 bf00  .L.......L......
+000000f0: 004c b500 0133 3f00 0050 7e00 0093 da00  .L...3?..P~.....
+00000100: 0050 7e00 00a7 1200 0051 3100 001e df00  .P~......Q1.....
+00000110: 0051 3100 0031 8400 0051 bc00 0094 0700  .Q1..1...Q......
+00000120: 0051 bc00 00a7 3e00 0051 be00 0094 3400  .Q....>..Q....4.
+00000130: 0051 be00 00a7 6a00 0052 ac00 0095 4200  .Q....j..R....B.
+00000140: 0052 ac00 0097 9b00 0053 3c00 0015 2300  .R.......S<...#.
+00000150: 0053 3c00 0036 c900 0053 8200 0094 6100  .S<..6...S....a.
+00000160: 0053 8200 00a7 9600 0053 8900 0094 8e00  .S.......S......
+00000170: 0053 8900 00a7 c200 0055 6600 0094 e800  .S.......Uf.....
+00000180: 0055 6600 00a7 ee00 0055 a400 0095 1500  .Uf......U......
+00000190: 0055 a400 00a8 1a00 0058 b900 0015 8a00  .U.......X......
+000001a0: 0058 b900 0020 5e00 0058 b900 0037 2800  .X... ^..X...7(.
+000001b0: 0058 b900 00ab 4d00 0058 b900 0122 1700  .X....M..X..."..
+000001c0: 0058 b900 0133 d300 0059 c000 0096 3900  .X...3...Y....9.
+000001d0: 0059 c000 00a8 4600 005a 7700 002b cf00  .Y....F..Zw..+..
+000001e0: 005a 7700 0088 d800 005a 7700 011c 1a00  .Zw......Zw.....
+000001f0: 005a 8800 0032 f900 005b 2a00 0027 6b00  .Z...2...[*..'k.
+00000200: 0070 7c00 005c 2100 047a 6e00 0005 4000  .p|..\!..zn...@.
+00000210: 047a 6e00 011a fc00 0498 9800 008e 2300  .zn...........#.
+00000220: 04a6 7900 006f 4800 04a6 7900 0084 5f00  ..y..oH...y..._.
+00000230: 04a8 a500 000e 0500 04a8 a500 009f 2100  ..............!.
+00000240: 04a8 a500 0121 6700 04a8 d300 0090 9400  .....!g.........
+00000250: 04cb c300 0093 5e00 04cf 3a00 0035 be00  ......^...:..5..
+00000260: 04d9 5d00 0138 3c00 04e3 1a00 0074 ad00  ..]..8<......t..
+00000270: 04e7 de00 000b 0d00 04e7 de00 000c 7500  ..............u.
+00000280: 0504 cf00 0077 e000 0528 a400 0035 ee00  .....w...(...5..
+00000290: 0548 3500 0006 1b00 0548 3500 000b 3c00  .H5......H5...<.
+000002a0: 0548 3500 0011 c100 0548 3500 008d 5900  .H5......H5...Y.
+000002b0: 0556 a500 0013 f800 0556 a500 001f 1200  .V.......V......
+000002c0: 0556 a500 002b 9a00 0556 a500 0031 f500  .V...+...V...1..
+000002d0: 0556 a500 0053 8b00 0556 a500 0133 7200  .V...S...V...3r.
+000002e0: 0556 a500 0138 6500 0565 c000 0043 cc00  .V...8e..e...C..
+000002f0: 0566 be00 0036 8f00 0566 be00 0121 9900  .f...6...f...!..
+00000300: 056b c200 0055 3a00 05a3 0000 004b d700  .k...U:......K..
+00000310: 05a7 aa00 011c fd00 05a7 e300 011f 0d00  ................
+00000320: 05b3 d800 0120 3600 05c0 6500 0021 a300  ..... 6...e..!..
+00000330: 05c0 6500 0033 2900 05db bb00 0027 9a00  ..e..3)......'..
+00000340: 05fb 8200 0027 d000 1530 3000 0012 3a00  .....'...00...:.
+00000350: 18d1 5000 00ef e700 2311 0000 0125 e200  ..P.....#....%..
+00000360: 26f2 9100 004c 0300 2aa8 a100 0056 e900  &....L..*....V..
+00000370: 2acf 0400 0057 1f00 2b37 fe00 0057 c500  *....W..+7...W..
+00000380: 2b76 1e00 0085 2e00 2ba7 e300 0059 c900  +v......+....Y..
+00000390: 2ec7 e000 0045 5e00 3153 c400 0093 9600  .....E^.1S......
+000003a0: 3d1a 0e00 005b 7c00 4182 8900 0100 e600  =....[|.A.......
+000003b0: 4796 c400 0077 6100 47af 8000 009b 3000  G....wa.G.....0.
+000003c0: 48a9 c400 0006 db00 48a9 c400 0012 8a00  H.......H.......
+000003d0: 48a9 c400 001c da00 48a9 c400 0029 9400  H.......H....)..
+000003e0: 48a9 c400 0030 6b00 48a9 c400 009e bc00  H....0k.H.......
+000003f0: 48a9 c400 00ab 1d00 48a9 c400 0132 8d00  H.......H....2..
+00000400: 48a9 c400 0137 4400 4964 b300 008f 9000  H....7D.Id......
+00000410: 4988 b300 008d e900 4a2b 8200 0046 c700  I.......J+...F..
+00000420: 4a2b 8200 006f 1500 4a36 9500 002a 4300  J+...o..J6...*C.
+00000430: 4a36 9500 0046 fe00 4a36 9500 0073 b900  J6...F..J6...s..
+00000440: 4a71 ec00 0025 3100 4ab8 3300 0028 d400  Jq...%1.J.3..(..
+00000450: 4b6b 9000 0105 8900 4d68 c800 0090 c400  Kk......Mh......
+00000460: 4d96 0a00 0025 df00 4dc4 b300 0090 f900  M....%..M.......
+00000470: 4e7e 1a00 0008 de00 522b 5a00 0073 ef00  N~......R+Z..s..
+00000480: 52e9 5500 0014 d900 5308 d400 0095 a500  R.U.....S.......
+00000490: 535d fe00 0074 dc00 5464 c900 0091 2c00  S]...t..Td....,.
+000004a0: 5464 c900 0094 bb00 5465 a800 0026 0e00  Td......Te...&..
+000004b0: 5483 8a00 0009 0d00 556a c300 0082 7d00  T.......Uj....}.
+000004c0: 55da be00 0012 0300 56bc 5a00 004a 9200  U.......V.Z..J..
+000004d0: 56bc 5a00 008c 4800 56bc 9300 008a 6800  V.Z...H.V.....h.
+000004e0: 578f 9500 0032 2c00 578f 9500 0133 a600  W....2,.W....3..
+000004f0: 57a1 7200 0027 2600 5839 2400 0069 8100  W.r..'&.X9$..i..
+00000500: 58c6 a500 009f 5100 5948 5c00 004e 5200  X.....Q.YH\..NR.
+00000510: 5948 5c00 0120 6a00 5a73 0400 001a 4a00  YH\.. j.Zs....J.
+00000520: 5a73 0400 0021 1900 5a79 2700 011e d700  Zs...!..Zy'.....
+00000530: 5a8a e000 0122 8400 5a8b c000 002f 6e00  Z...."..Z..../n.
+00000540: 5a8e c300 0096 6600 5a8e c300 012f 2000  Z.....f.Z..../ .
+00000550: 5b6a 7c00 000d 4600 5b6a 7c00 0096 9b00  [j|...F.[j|.....
+00000560: 5c06 8a00 004c 8d00 5c83 b500 0034 ec00  \....L..\....4..
+00000570: 5c83 b500 0037 9100 5fb8 5a00 0080 5300  \....7.._.Z...S.
+00000580: 5fb8 5a00 0130 8400 602e 0a00 0054 d800  _.Z..0..`....T..
+00000590: 67f7 0000 00f9 3600 70c5 c000 00c9 bd00  g.....6.p.......
+000005a0: 80a8 e500 0049 ce00 81bc 0000 00cf a600  .....I..........
+000005b0: 918d 3700 003c 4000 931f 2000 00db 1500  ..7..<@... .....
+000005c0: 9472 3000 006e ba00 9688 5400 00d5 f800  .r0..n....T.....
+000005d0: ab81 4000 0119 0f00 af00 f000 00b7 7c00  ..@...........|.
+000005e0: af26 4500 0126 6600 b27d 9f00 0078 7600  .&E..&f..}...xv.
+000005f0: b4d0 c500 0029 d900 b643 0000 00c4 4200  .....)...C....B.
+00000600: c9db ba00 0061 7e00 cfb0 f400 0031 1100  .....a~......1..
+00000610: e1f3 f000 0017 8d00 e25b 3000 002c f900  .........[0..,..
+00000620: ed2c 2500 0028 0000 fbe4 b100 0048 3e00  .,%..(.......H>.
+00000630: ff6b fe00 00b4 ba01 11c0 6000 013a d401  .k........`..:..
+00000640: 1c4b f000 0116 9701 2273 8300 008d 9701  .K......"s......
+00000650: 24a2 9700 003c f701 2bca d000 009d a501  $....<..+.......
+00000660: 3502 c000 00c6 1101 473b 2300 0070 5201  5.......G;#..pR.
+00000670: 5567 7000 00ce ff01 59b4 9000 001b 0d01  Ugp.....Y.......
+00000680: 6654 9000 003b 3701 7248 d000 0036 2801  fT...;7.rH...6(.
+00000690: 776d e000 00d7 1801 78c3 f500 0031 b001  wm......x....1..
+000006a0: 7e51 ea00 012c d501 873b 2300 0070 8401  ~Q...,...;#..p..
+000006b0: 887c d300 005c 4d01 9687 c000 010c 7201  .|...\M.......r.
+000006c0: 98a7 5300 004c bc01 a469 f900 0103 8201  ..S..L...i......
+000006d0: a885 4000 0136 0f01 aff7 3300 0000 0001  ..@..6....3.....
+000006e0: bef6 7000 00d4 1601 c26a 9a00 00a2 3501  ..p......j....5.
+000006f0: ce0a 1200 008b 5101 d48e 5000 0043 2801  ......Q...P..C(.
+00000700: da69 b000 0116 2a01 e128 5000 00c1 4801  .i....*..(P...H.
+00000710: e26a 9a00 0004 2801 f571 7000 00be 5702  .j....(..qp...W.
+00000720: 00dd 0100 0044 6a02 01b8 4900 003a 8d02  .....Dj...I..:..
+00000730: 01b8 4900 0087 8d02 01b8 4900 00a1 c002  ..I.......I.....
+00000740: 01b8 4900 0139 fc02 24d1 2000 00e0 cd02  ..I..9..$. .....
+00000750: 2b24 6500 012f e202 36c0 e700 006b c702  +$e../..6....k..
+00000760: 38ab b000 00b1 4b02 488e 8300 0129 2102  8.....K.H....)!.
+00000770: 5442 2f00 0022 3d02 6b41 b400 0130 af02  TB/.."=.kA...0..
+00000780: 705b 1000 005e cb02 75ac 0500 00d9 6502  p[...^..u.....e.
+00000790: 76e6 2500 0043 fd02 80f4 7400 005a 4102  v.%..C....t..ZA.
+000007a0: 83cb 1900 00ae 4d02 84df 6000 000d 0b02  ......M...`.....
+000007b0: 86cb d700 00af da02 960b 0000 0104 af02  ................
+000007c0: 9d24 b400 00c0 e502 a013 f300 00d5 9d02  .$..............
+000007d0: b6bc 9300 0058 3f02 b827 6100 00a3 fb02  .....X?..'a.....
+000007e0: c4de 6000 00ca 4b02 d6b9 7000 00e1 a802  ..`...K...p.....
+000007f0: d6b9 7000 00ed 9402 d6b9 7000 0104 0602  ..p.......p.....
+00000800: d6b9 7000 010e d202 da2f f000 00bc 8102  ..p....../......
+00000810: db87 a000 00f4 2702 ddd8 9000 0018 c702  ......'.........
+00000820: e4ef 0400 0020 9702 e60b 0000 0076 e402  ..... .......v..
+00000830: ecb9 d000 006c c303 0055 4a00 012c 3e03  .....l...UJ..,>.
+00000840: 0ae6 8700 0018 3203 0ae6 8700 001d ba03  ......2.........
+00000850: 0b8a 5a00 0079 f103 1108 9c00 0132 b603  ..Z..y.......2..
+00000860: 1638 c400 0095 ed03 1684 be00 001d 0d03  .8..............
+00000870: 2221 4000 00b0 c203 232f f000 00f5 6e03  "!@.....#/....n.
+00000880: 232f f000 010a 0d03 3500 5a00 0087 4103  #/......5.Z...A.
+00000890: 3f3c 8400 0112 a303 55cb 1a00 0075 4803  ?<......U....uH.
+000008a0: 57fa 2e00 0074 3603 5dae f000 010a bc03  W....t6.].......
+000008b0: 5dce f000 00e5 4103 6b8b d900 0127 fc03  ].....A.k....'..
+000008c0: 7321 8300 0111 8703 82a1 0000 00e1 d903  s!..............
+000008d0: 8a06 2000 0101 5603 8b39 a000 0105 f103  .. ...V..9......
+000008e0: 8b60 e400 003f b803 8c34 6500 0026 cd03  .`...?...4e..&..
+000008f0: 8f4e c000 0115 6303 9100 d000 005d d303  .N....c......]..
+00000900: 97c9 0000 0123 d903 b023 a000 00bb 3203  .....#...#....2.
+00000910: cafd 4000 0082 b603 d07e 2400 0067 a303  ..@......~$..g..
+00000920: d1c2 7400 0041 9203 d1e5 2200 0005 7103  ..t..A...."...q.
+00000930: da9c f300 0059 fb03 ec0c f700 003d bd03  .....Y.......=..
+00000940: f69b 8000 00c8 6b04 0029 e000 0127 4704  ......k..)...'G.
+00000950: 09f4 0a00 00bd e304 11d2 4900 000d 7704  ..........I...w.
+00000960: 11d2 a900 0056 5804 1263 4400 00b7 2e04  .....VX..cD.....
+00000970: 1564 8e00 0029 5a04 15b4 7000 013b 4d04  .d...)Z...p..;M.
+00000980: 195c b000 011a 6504 2e61 f000 0072 6c04  .\....e..a...rl.
+00000990: 449a c000 012e 2e04 56c0 a000 00b9 0604  D.......V.......
+000009a0: 62c1 c000 0100 5b04 65af 6900 004f 3104  b.....[.e.i..O1.
+000009b0: 66ac 6500 0138 fe04 7914 8000 00d2 b104  f.e..8..y.......
+000009c0: 7d16 7000 006d 9f04 846c 5400 002b 2e04  }.p..m...lT..+..
+000009d0: 846c 5400 0081 da04 846c 5400 0088 1104  .lT......lT.....
+000009e0: 846c 5400 0137 1104 8a9c b300 000a 1404  .lT..7..........
+000009f0: 8a9c b300 0091 e904 8c2d c700 0063 e904  .........-...c..
+00000a00: 8c2d c700 007b 6f04 8e23 4000 0000 c004  .-...{o..#@.....
+00000a10: 8e23 4000 001f e304 8e23 4000 0054 5e04  .#@......#@..T^.
+00000a20: 983c 8100 0046 9304 9849 bc00 0008 3504  .<...F...I....5.
+00000a30: 9e16 8200 0103 4304 9e84 d500 0092 4404  ......C.......D.
+00000a40: a577 1f00 0065 d004 a5e2 3000 0098 af04  .w...e....0.....
+00000a50: ac2c a500 0084 f504 ac2c a500 00a3 bf04  .,.......,......
+00000a60: bebd 0000 00a9 7504 c840 f000 00eb 1204  ......u..@......
+00000a70: c840 f000 00ee 4d04 c840 f000 0110 fd04  .@....M..@......
+00000a80: cc5c 9400 0028 4e04 cf4d c200 00f9 bd04  .\...(N..M......
+00000a90: d5c8 0000 0007 1a04 d7d5 4000 00cd 0004  ..........@.....
+00000aa0: dd34 9000 0015 bf04 ee54 4000 010d 7204  .4.......T@...r.
+00000ab0: f6d3 c900 00d5 3605 04e3 1000 0007 9505  ......6.........
+00000ac0: 079c 7300 0124 6705 161e a000 00b6 b905  ..s..$g.........
+00000ad0: 2caa 5000 00b5 1705 2cde 2300 00a4 5305  ,.P.....,.#...S.
+00000ae0: 304c 6a00 0049 9805 33ee 2500 0015 5205  0Lj..I..3.%...R.
+00000af0: 33ee 2500 0036 f405 3c8d c200 0018 7105  3.%..6..<.....q.
+00000b00: 3c8d c200 001e 8705 3d7b 7000 00ea ad05  <.......={p.....
+00000b10: 3d7b 7000 00ed e805 3d7b 7000 0105 2405  ={p.....={p...$.
+00000b20: 3d7b 7000 0110 1a05 49ee 8900 0067 0905  ={p.....I....g..
+00000b30: 4e5b d400 0119 5d05 5305 de00 0075 9605  N[....].S....u..
+00000b40: 5316 ce00 0074 7505 633f 7000 00e6 9b05  S....tu.c?p.....
+00000b50: 6945 5000 00c7 1f05 6bc4 2700 008a 2705  iEP.....k.'...'.
+00000b60: 6bcd a500 00b2 e205 6c90 5400 0095 6f05  k.......l.T...o.
+00000b70: 6ccc 4300 004b 7205 6edf f400 008c e305  l.C..Kr.n.......
+00000b80: 6fe5 c000 00f4 d905 802f 5e00 00b2 1605  o......../^.....
+00000b90: 812d 6000 0102 e605 88a7 e000 0122 4c05  .-`.........."L.
+00000ba0: 88a8 c000 004d c705 8c6a c300 009e 7f05  .....M...j......
+00000bb0: 8c6a c300 011b a605 8cbc 8e00 004b 3c05  .j...........K<.
+00000bc0: 98ab 6e00 008d 2505 9ca9 f100 0039 1905  ..n...%......9..
+00000bd0: 9dfd c000 00a8 f505 9e88 c300 0091 6105  ..............a.
+00000be0: a661 8700 004d fc05 a661 8700 004e d505  .a...M...a...N..
+00000bf0: a661 8700 0050 6705 a7f1 8700 0053 3505  .a...Pg......S5.
+00000c00: adfb 2800 009f 8c05 b039 5c00 000b 7b05  ..(......9\...{.
+00000c10: b039 5c00 011b e305 b093 0000 00c8 f905  .9\.............
+00000c20: b247 c400 009a d605 c068 c000 0009 a705  .G.......h......
+00000c30: c1f8 2200 008c 8805 ced0 2500 00d9 db05  ..".......%.....
+00000c40: d5fa e400 007f 5d05 d5fa e400 012c 8e05  ......]......,..
+00000c50: da03 6e00 005b dc05 dbc2 3900 0050 1e05  ..n..[....9..P..
+00000c60: dce3 0000 00d2 3705 dce3 0000 0102 6d05  ......7.......m.
+00000c70: dde3 7900 005e f505 e1ed 8400 00bf 4405  ..y..^........D.
+00000c80: ecff 1900 00ed 2305 f264 ba00 0047 3305  ......#..d...G3.
+00000c90: f662 ea00 00bd 6e05 facb 8300 008f cb06  .b....n.........
+00000ca0: 0826 4000 00d7 b406 08e3 9400 007a 8706  .&@..........z..
+00000cb0: 0ab9 9000 00e3 9b06 129d e000 00e0 5c06  ..............\.
+00000cc0: 148d a400 0021 d706 1867 1e00 0098 f906  .....!...g......
+00000cd0: 215f 7400 0061 2b06 2b00 1300 0037 fd06  !_t..a+.+....7..
+00000ce0: 2b00 1300 0038 8d06 2b00 1300 003a 0a06  +....8..+....:..
+00000cf0: 34af 4a00 0009 d706 3500 0f00 006a 5a06  4.J.....5....jZ.
+00000d00: 3c17 4000 00dd b406 3c17 4000 00e9 7006  <.@.....<.@...p.
+00000d10: 3c17 4000 00fb a606 3c17 4000 0115 1306  <.@.....<.@.....
+00000d20: 3cee 8400 00ad 0106 468c a000 00b1 ac06  <.......F.......
+00000d30: 4e38 c500 00a0 2d06 4f34 c000 0112 0506  N8....-.O4......
+00000d40: 53a5 f500 004b 0706 5479 d900 010f a906  S....K..Ty......
+00000d50: 580f ce00 002a 7e06 5a60 a900 00fa 0e06  X....*~.Z`......
+00000d60: 6318 9000 00e7 af06 68ee 6400 001c 8b06  c.......h.d.....
+00000d70: 69a9 8400 00a2 7e06 69b7 0200 012b 8f06  i.....~.i....+..
+00000d80: 70e2 d000 006d f606 7cd1 c500 004a 2206  p....m..|....J".
+00000d90: 7f33 4700 0032 ad06 8786 ea00 00a1 5f06  .3G..2........_.
+00000da0: 88a1 2400 0137 b006 8f30 5000 0120 9a06  ..$..7...0P.. ..
+00000db0: 9b5a 7700 011c 7c06 9bb8 0c00 0038 d406  .Zw...|......8..
+00000dc0: 9c50 2000 00c5 5f06 9fb2 5300 00ff 9406  .P ..._...S.....
+00000dd0: a6d5 8300 012f 4f06 a8dd 9c00 0051 5b06  ...../O......Q[.
+00000de0: aef9 ce00 0058 be06 afe6 3000 0071 9806  .....X....0..q..
+00000df0: b017 2200 00a0 ce06 b8bb 6000 00a9 f606  ..".......`.....
+00000e00: c10c 6000 00d0 3206 c215 0a00 0007 ee06  ..`...2.........
+00000e10: c227 5a00 0029 0b06 c5bd 6a00 0127 c806  .'Z..)....j..'..
+00000e20: ce8a a100 004c 4406 cf70 9900 0024 f606  .....LD..p...$..
+00000e30: d08b 2a00 00ca fd06 d81c 2e00 00da 4606  ..*...........F.
+00000e40: dbaf 2000 00f1 4e06 e231 4000 012e a506  .. ...N..1@.....
+00000e50: e6c0 4c00 0051 c007 0120 6600 0020 e707  ..L..Q... f.. ..
+00000e60: 0140 6600 0019 e407 0923 2000 0060 3807  .@f......# ..`8.
+00000e70: 0ac3 fa00 00a1 2107 0e35 d000 00dd 5407  ......!..5....T.
+00000e80: 126c 4400 013b ce07 1d24 9000 0107 0607  .lD..;...$......
+00000e90: 1db9 0500 0013 7407 3389 e000 00b8 4207  ......t.3.....B.
+00000ea0: 3c71 f700 000f 6607 449d 1f00 00bf a907  <q....f.D.......
+00000eb0: 47cf 0400 0040 ba07 4bcf e000 00e9 c007  G....@..K.......
+00000ec0: 5cec 7500 009f e907 62f5 3500 0040 4107  \.u.....b.5..@A.
+00000ed0: 65e8 b400 007e 0b07 65e8 b400 012a ed07  e....~..e....*..
+00000ee0: 6c21 5400 000b f607 7e9b 0500 00e8 c107  l!T.....~.......
+00000ef0: 9a56 2000 006f bc07 9a6c 1400 000c a507  .V ..o...l......
+00000f00: 9a6c 1400 001c 5207 9a6c 1400 0030 3907  .l....R..l...09.
+00000f10: 9a6c 1400 0051 2307 9a6c 1400 0081 a707  .l...Q#..l......
+00000f20: 9a6c 1400 0132 5e07 9aa9 6000 00cd 9807  .l...2^...`.....
+00000f30: 9db4 9000 00ba cb07 9db4 9000 00ff 2007  .............. .
+00000f40: 9e2e 7300 0139 9b07 a121 8000 0022 ea07  ..s..9...!..."..
+00000f50: a674 8700 00a2 d107 bdfe de00 002d 9a07  .t...........-..
+00000f60: cf9a 7000 00fd 4007 d231 3400 0003 9f07  ..p...@..14.....
+00000f70: daae 0000 0106 9907 dae0 ea00 011f 8b07  ................
+00000f80: e0a9 5000 000e a107 e0a9 5000 0089 6807  ..P.......P...h.
+00000f90: e0a9 5000 011d 9307 ebd7 9e00 00ac 2407  ..P...........$.
+00000fa0: ebd7 9e00 00af 0f07 ec42 a500 000a c507  .........B......
+00000fb0: ed5c 8000 0114 3207 f3d4 e000 00cb f207  .\....2.........
+00000fc0: f714 e400 00fa 8f08 0291 0000 0080 8408  ................
+00000fd0: 08a7 9000 00c6 9a08 1f02 9000 00b7 e208  ................
+00000fe0: 283b 1400 00ff eb08 284d 4300 0083 cb08  (;......(MC.....
+00000ff0: 28e8 e000 00f2 0508 2a45 4a00 00a3 1c08  (.......*EJ.....
+00001000: 2fe7 9000 009d 2d08 3267 1100 0008 a008  /.....-.2g......
+00001010: 41da 6e00 0085 8308 426e 6000 0118 1808  A.n.....Bn`.....
+00001020: 46c5 3a00 0045 f408 4d37 c500 0092 8008  F.:..E..M7......
+00001030: 4e6b 2a00 0047 7b08 4ef9 1500 005b 4608  Nk*..G{.N....[F.
+00001040: 4fd0 2000 0117 9508 6186 7000 0070 b608  O. .....a.p..p..
+00001050: 6c71 e200 00ae b008 6f32 c000 00db d608  lq......o2......
+00001060: 700d f000 00fc b908 70b2 8b00 0076 2308  p.......p....v#.
+00001070: 7219 0f00 0089 9f08 7a4a 5000 0079 1d08  r.......zJP..y..
+00001080: 8284 d500 000c d608 8284 d500 0082 0e08  ................
+00001090: 8599 7200 0138 c508 8958 2900 012d d508  ..r..8...X)..-..
+000010a0: 8b87 0000 00d3 6e08 8fa4 9300 0010 9908  ......n.........
+000010b0: 8fa4 9300 0085 d108 8fa4 9300 008b cd08  ................
+000010c0: 8fa4 9300 011c 4408 9a98 b400 001a c808  ......D.........
+000010d0: 9c61 5e00 011f e608 a1a4 9300 0057 ff08  .a^..........W..
+000010e0: a63b 3000 0110 8008 aa82 f400 0059 9008  .;0..........Y..
+000010f0: abe2 0900 002b 5f08 abe2 0900 0088 4608  .....+_.......F.
+00001100: af11 d500 0062 0308 b89a 9200 0026 9208  .....b.......&..
+00001110: bbfe c500 0002 ac08 bbfe c500 0128 d208  .............(..
+00001120: bd8a 6000 0119 db08 c000 5000 0097 5608  ..`.......P...V.
+00001130: c000 5000 0098 1908 c272 0900 0010 d608  ..P......r......
+00001140: c76b 0300 0059 0508 cd7c e400 00ab b409  .k...Y...|......
+00001150: 00f9 a400 0003 e009 162e f000 003b c609  .............;..
+00001160: 1afc d400 003e 7709 1fb9 f500 0075 c809  .....>w......u..
+00001170: 2254 0000 0123 7a09 2e57 df00 00a5 a109  "T...#z..W......
+00001180: 35e6 6000 0049 5509 3b85 e000 006b 3909  5.`..IU.;....k9.
+00001190: 4459 d000 00e3 0a09 4d67 fe00 011b 6609  DY......Mg....f.
+000011a0: 5962 c900 00e9 0009 5aa4 1000 00bb cf09  Yb......Z.......
+000011b0: 5b68 f000 005d 5909 5c07 3000 00f0 9f09  [h...]Y.\.0.....
+000011c0: 5ca2 3000 0134 4609 5d03 9000 0121 d709  \.0..4F.]....!..
+000011d0: 6302 2500 0139 6b09 667a 9000 00ee d609  c.%..9k.fz......
+000011e0: 66cc c900 0034 b109 700b c500 0012 cf09  f....4..p.......
+000011f0: 7a29 6900 0010 1909 8c00 0a00 004e 8f09  z)i..........N..
+00001200: 8c81 5e00 003a 4b09 8c81 5e00 004f d009  ..^..:K...^..O..
+00001210: 8c81 5e00 0097 cf09 8d04 b300 008f 0209  ..^.............
+00001220: 95cb c400 00d8 f809 a6af c300 0055 e109  .............U..
+00001230: a6c1 0a00 0028 9c09 a6c1 0a00 0045 8b09  .....(.......E..
+00001240: a6c1 0a00 0082 f709 a6c1 0a00 0097 1909  ................
+00001250: a6c1 0a00 0126 3609 a6c1 c300 0004 6f09  .....&6.......o.
+00001260: a87a 8000 00fb fd09 b56b a200 008c 0609  .z.......k......
+00001270: b889 ea00 0086 aa09 b889 ea00 00a5 0709  ................
+00001280: cf34 f000 00e2 7509 d82d 3f00 0083 2e09  .4....u..-?.....
+00001290: dbfe c000 00dc 950a 074b 5000 0071 ff0a  .........KP..q..
+000012a0: 159b 8000 001f 500a 159b 8000 0053 cc0a  ......P......S..
+000012b0: 17d3 5000 00ce 560a 20b0 6000 0078 170a  ..P...V. .`..x..
+000012c0: 20fc 9000 00b5 fb0a 22d2 d000 00e7 1a0a   .......".......
+000012d0: 2aef e000 00fd cb0a 2e99 7e00 0056 190a  *.........~..V..
+000012e0: 30f6 b500 002a d60a 338b 1000 00df db0a  0....*..3.......
+000012f0: 3f0e 9500 0080 0c0a 3f0e 9500 012d 940a  ?.......?....-..
+00001300: 4985 3000 0071 240a 4cb2 e000 00b9 860a  I.0..q$.L.......
+00001310: 5e50 b000 010c fb0a 62cd 3400 0035 6a0a  ^P......b.4..5j.
+00001320: 64c8 9500 0086 6e0a 65e3 f000 005c 9e0a  d.....n.e....\..
+00001330: 6c11 b300 0005 040a 6c5b d900 000a 580a  l.......l[....X.
+00001340: 6c5b d900 000c 3e0a 6c89 9300 0139 2e0a  l[....>.l....9..
+00001350: 6cba 2900 010f 270a 70ea 0000 0044 f00a  l.)...'.p....D..
+00001360: 8170 8e00 0135 1d0a 84e6 b500 001d 730a  .p...5........s.
+00001370: 84e6 b500 0030 d10a 84e6 b500 0052 2c0a  .....0.......R,.
+00001380: 84e6 b500 0133 020a 84e6 b500 0137 700a  .....3.......7p.
+00001390: 89ad 3000 00f7 d40a 89ad 3000 010e 340a  ..0.......0...4.
+000013a0: 8c5e f000 0065 210a 954c 2000 00de 050a  .^...e!..L .....
+000013b0: 9989 6300 0073 670a ac8c c000 00fb 2d0a  ..c..sg.......-.
+000013c0: ae3e fa00 0075 0e0a b4bc 2e00 002f 9e0a  .>...u......./..
+000013d0: b5ff 6400 00b3 7a0a b6d5 d000 00d4 960a  ..d...z.........
+000013e0: ba90 7000 00ea 2e0a be20 4a00 0011 1c0a  ..p...... J.....
+000013f0: c25d 1400 0042 530a c945 a000 00b5 6e0a  .]...BS..E....n.
+00001400: ca80 7300 0052 720a cf76 b400 0057 530a  ..s..Rr..v...WS.
+00001410: cfef 4000 0109 790a e1b0 da00 00aa 570a  ..@...y.......W.
+00001420: e1b4 8000 0117 1c0a e45f d000 00ba 440a  ........._....D.
+00001430: eb63 2000 0023 870a ee50 6000 0081 3c0a  .c ..#...P`...<.
+00001440: f3de 9e00 0084 9c0a f818 8000 00b9 bf0a  ................
+00001450: f818 8000 00fe 8e0b 0396 6300 0009 720b  ..........c...r.
+00001460: 03f9 7300 008e b80b 0476 b400 0057 8d0b  ..s......v...W..
+00001470: 0ac1 5a00 012d 2a0b 139f b500 0086 e20b  ..Z..-*.........
+00001480: 19b8 d700 008a a60b 1b90 b000 0104 360b  ..............6.
+00001490: 1fcd 0500 00a0 8a0b 20ce b000 00c4 cd0b  ........ .......
+000014a0: 2371 ce00 0001 3e0b 244d 8300 0108 550b  #q....>.$M....U.
+000014b0: 296c c900 0072 f80b 2d80 be00 000f c70b  )l...r..-.......
+000014c0: 2d80 be00 008b 030b 2d80 be00 011e 1a0b  -.......-.......
+000014d0: 2fa8 e400 0134 020b 4000 a500 0063 660b  /....4..@....cf.
+000014e0: 440d ae00 0059 3e0b 47ce c400 00ec 0e0b  D....Y>.G.......
+000014f0: 4841 e400 00be de0b 4e26 9900 0011 620b  HA......N&....b.
+00001500: 543a f400 00e4 3e0b 5467 9000 002b fd0b  T:....>.Tg...+..
+00001510: 6948 d000 00c7 b90b 6b4e 3000 005e 3c0b  iH......kN0..^<.
+00001520: 6f1b 4500 0060 a10b 76dd 9d00 0137 fb0b  o.E..`..v....7..
+00001530: 8a1a 2000 00e5 d50b 8a1a 2000 0113 df0b  .. ....... .....
+00001540: 8c6a e300 0058 800b 9253 4000 0002 280b  .j...X...S@...(.
+00001550: 94b6 5e00 00d1 7f0b 967b 5400 0032 5c0b  ..^......{T..2\.
+00001560: a0c9 de00 0006 5c0b a3fc 0c00 006f 7e0b  ......\......o~.
+00001570: a3fc 7000 00f3 ad0b a4a2 2500 0025 690b  ..p.......%..%i.
+00001580: c474 9000 00de a10b c4a6 f000 0062 f10b  .t...........b..
+00001590: c81a a000 00df 400b cbf1 c000 00e6 280b  ......@.......(.
+000015a0: cbf1 c000 00eb 9b0b cbf1 c000 00f6 230b  ..............#.
+000015b0: cbf1 c000 010b fe0b db2b b200 0026 430b  .........+...&C.
+000015c0: def4 0000 0131 4b0b e203 8700 000f 1f0b  .....1K.........
+000015d0: e217 6300 000e dc0b e4a0 3000 0016 c50b  ..c.......0.....
+000015e0: f39a 4000 003a ce0b f39a 4000 0080 cd0b  ..@..:....@.....
+000015f0: f39a 4000 00cb 800b fc32 3300 0046 290c  ..@......23..F).
+00001600: 04fe c500 0014 360c 0c17 6300 0056 a70c  ......6...c..V..
+00001610: 0ce3 2300 008e 620c 0dec 5a00 007f aa0c  ..#...b...Z.....
+00001620: 1d95 4000 00c2 fa0c 3834 1400 000e 3b0c  ..@.....84....;.
+00001630: 3834 1400 0089 060c 3834 1400 011d 310c  84......84....1.
+00001640: 5256 ae00 0034 730c 5bd6 a000 0008 670c  RV...4s.[.....g.
+00001650: 61ce a500 0035 240c 63ce a500 000b b00c  a....5$.c.......
+00001660: 6dca b800 0038 3e0c 808a a300 00a4 ad0c  m....8>.........
+00001670: 83b7 b000 0037 c40c 8910 0000 0006 9a0c  .....7..........
+00001680: 89ed e500 004a cf0c 98c0 0900 0005 e20c  .....J..........
+00001690: 98c0 0900 000a 8e0c 98c0 0900 000d c70c  ................
+000016a0: 98c0 0900 0082 450c 98c0 0900 0087 d00c  ......E.........
+000016b0: 98c0 0900 009e e90c 98c0 0900 011b 2d0c  ..............-.
+000016c0: 9fa9 6000 0122 bd0c b106 9a00 011f 3c0c  ..`.."........<.
+000016d0: b195 2700 007e b30c b1a8 e500 0031 4c0c  ..'..~.......1L.
+000016e0: ba9f 2400 0113 600c c1c5 c300 0090 510c  ..$...`.......Q.
+000016f0: c4e1 d500 0014 7f0c c5f7 d500 007c a80c  .............|..
+00001700: c7ee 6000 009b d60c c8e8 6400 0030 970c  ..`.......d..0..
+00001710: c9a0 2e00 007d 070c cba2 d500 00ec e30c  .....}..........
+00001720: db0c 0400 00b6 6b0c dda2 6e00 00b3 e80c  ......k...n.....
+00001730: e3ed a900 0090 060c f3b0 8500 0013 190c  ................
+00001740: fb0f b300 0092 f20d 0027 2000 00c1 cd0d  .........' .....
+00001750: 09a5 6000 0120 f20d 0a66 ed00 012a 610d  ..`.. ...f...*a.
+00001760: 0ad7 7300 004d 170d 0f91 6000 00f2 8f0d  ..s..M....`.....
+00001770: 0f91 6000 0107 ba0d 1201 a400 005a cf0d  ..`..........Z..
+00001780: 1cec 6700 011e 680d 2d41 7000 00b0 2b0d  ..g...h.-Ap...+.
+00001790: 32db 3000 00ef 310d 35c6 3000 010b 510d  2.0...1.5.0...Q.
+000017a0: 3b8c 3900 00ad ab0d 48cd 6500 0099 c70d  ;.9.....H.e.....
+000017b0: 51bd f000 00f6 9d0d 69f6 0000 009c 830d  Q.......i.......
+000017c0: 7298 e700 00af 670d 7c3b 4000 0114 a50d  r.....g.|;@.....
+000017d0: 80f6 3400 0096 ce0d 80f6 3400 0098 5e0d  ..4.......4...^.
+000017e0: 8344 9300 008f 480d 8c46 7500 0004 a70d  .D....H..Fu.....
+000017f0: 8c46 7500 00a5 420d 96e3 5000 00e1 540d  .Fu...B...P...T.
+00001800: 9df1 6500 001a 7d0d 9df1 6500 0021 520d  ..e...}...e..!R.
+00001810: 9ee3 5e00 006b 860d 9ee3 5e00 0077 9b0d  ..^..k....^..w..
+00001820: 9ee3 5e00 0084 140d 9ee3 5e00 00a3 710d  ..^.......^...q.
+00001830: 9ee3 5e00 00b8 c20d aa4e 9000 00e8 3d0d  ..^......N....=.
+00001840: c964 7400 00ac 7a0d d0e8 e000 00ca bf0d  .dt...z.........
+00001850: ded8 9000 001d ff0d ded8 9000 0052 ae0d  .............R..
+00001860: eb49 0000 007e eb0d ec49 8400 0048 950d  .I...~...I...H..
+00001870: f086 4a00 0039 b50d fcd5 7e00 003f 300d  ..J..9....~..?0.
+00001880: fe0b 6000 006e 5a0e 00f0 b000 00d6 990e  ..`..nZ.........
+00001890: 03af f000 0076 670e 1bf8 6400 0039 540e  .....vg...d..9T.
+000018a0: 1ddb 6300 0050 c30e 202b 3a00 007d 660e  ..c..P.. +:..}f.
+000018b0: 202b 3a00 0129 c80e 2511 7400 005f 3f0e   +:..)..%.t.._?.
+000018c0: 38a0 f000 0108 da0e 5c13 4700 011c b00e  8.......\.G.....
+000018d0: 6193 e900 0115 d30e 61d5 0400 00aa a60e  a.......a.......
+000018e0: 68cb dc00 0055 7b0e 6ac2 e300 0025 a00e  h....U{.j....%..
+000018f0: 7617 2000 007a d80e 8347 4400 0068 e70e  v. ..z...GD..h..
+00001900: 887b b500 0037 590e 887b b500 00ab 7d0e  .{...7Y..{....}.
+00001910: 9dcc d400 0033 560e a934 c000 005f be0e  .....3V..4..._..
+00001920: abf5 1300 0066 950e ae34 8000 005c f90e  .....f...4...\..
+00001930: b4a5 0a00 0062 8c0e b5c2 8000 009a 290e  .....b........).
+00001940: b803 9900 006d 4a0e b82d 1000 00f7 310e  .....mJ..-....1.
+00001950: c28b b000 0003 0c0e d945 de00 002e 560e  .........E....V.
+00001960: e77d 7000 0125 310e f7f8 4000 00f3 300f  .}p..%1...@...0.
+00001970: 09fd b000 00d8 5d0f 0cc4 c000 00fe 3b0f  ......].......;.
+00001980: 105e a000 00bd 030f 11be 6000 00c2 420f  .^........`...B.
+00001990: 1d28 1000 0101 fd0f 201d 8500 0088 850f  .(...... .......
+000019a0: 20f1 3000 00da 9d0f 4321 f500 0135 b40f   .0.....C!...5..
+000019b0: 4a90 4000 00b5 b20f 5e00 1000 00cc 7b0f  J.@.....^.....{.
+000019c0: 8e7b e000 00d0 dd0f 9222 7c00 00ad 6b0f  .{......."|...k.
+000019d0: 9450 0000 0118 840f 969b 9a00 004f 790f  .P...........Oy.
+000019e0: 9ebd c400 0048 ed0f 9fbc 6000 013a 3e0f  .....H....`..:>.
+000019f0: a262 9000 013c b50f a44f 0300 0000 5f0f  .b...<...O...._.
+00001a00: bd5e e700 011d ca0f cb15 5200 0068 9b0f  .^........R..h..
+00001a10: cf80 f000 00f8 780f d19a 7000 00c3 b30f  ......x...p.....
+00001a20: dfeb 7000 009e 140f e7f7 9000 013c 430f  ..p..........<C.
+00001a30: ea8a 0900 007d ab0f ea8a 0900 00a8 9d0f  .....}..........
+00001a40: ea8a 0900 012a 070f f87c e000 0024 6d0f  .....*...|...$m.
+00001a50: fe37 0300 0086 1069 0001 3d30 0300 0000  .7.....i..=0....
+00001a60: 2404 1e04 4204 3c04 3504 3d04 3804 4204  $...B.<.5.=.8.B.
+00001a70: 4c00 2004 3804 3704 3c04 3504 3d04 3504  L. .8.7.<.5.=.5.
+00001a80: 3d04 3804 4f08 0000 0000 0600 0000 0e43  =.8.O..........C
+00001a90: 616e 6365 6c20 6368 616e 6765 7307 0000  ancel changes...
+00001aa0: 0018 4162 7374 7261 6374 4f70 6572 6174  ..AbstractOperat
+00001ab0: 696f 6e44 6574 6169 6c73 0103 0000 0026  ionDetails.....&
+00001ac0: 0421 043e 0445 0440 0430 043d 0438 0442  .!.>.E.@.0.=.8.B
+00001ad0: 044c 0020 0438 0437 043c 0435 043d 0435  .L. .8.7.<.5.=.5
+00001ae0: 043d 0438 044f 0800 0000 0006 0000 000e  .=.8.O..........
+00001af0: 436f 6d6d 6974 2063 6861 6e67 6573 0700  Commit changes..
+00001b00: 0000 1841 6273 7472 6163 744f 7065 7261  ...AbstractOpera
+00001b10: 7469 6f6e 4465 7461 696c 7301 0300 0000  tionDetails.....
+00001b20: 3804 1e04 4804 3804 3104 3a04 3000 2004  8...H.8.1.:.0. .
+00001b30: 3f04 4004 3800 2004 3704 3004 3f04 3804  ?.@.8. .7.0.?.8.
+00001b40: 4104 3800 2004 3e04 3f04 3504 4004 3004  A.8. .>.?.5.@.0.
+00001b50: 4604 3804 3800 3a00 2008 0000 0000 0600  F.8.8.:. .......
+00001b60: 0000 194f 7065 7261 7469 6f6e 2073 7562  ...Operation sub
+00001b70: 6d69 7420 6661 696c 6564 3a20 0700 0000  mit failed: ....
+00001b80: 1841 6273 7472 6163 744f 7065 7261 7469  .AbstractOperati
+00001b90: 6f6e 4465 7461 696c 7301 0300 0000 8804  onDetails.......
+00001ba0: 1d04 3504 4104 3e04 4504 4004 3004 3d04  ..5.A.>.E.@.0.=.
+00001bb0: 5104 3d04 3d04 4b04 3500 2004 3804 3704  Q.=.=.K.5. .8.7.
+00001bc0: 3c04 3504 3d04 3504 3d04 3804 4f00 2004  <.5.=.5.=.8.O. .
+00001bd0: 3104 4b04 3b04 3800 2004 3e04 4204 3c04  1.K.;.8. .>.B.<.
+00001be0: 3504 3d04 3504 3d04 4b00 2004 3f04 3504  5.=.5.=.K. .?.5.
+00001bf0: 4004 3504 3400 2004 4104 3e04 3704 3404  @.5.4. .A.>.7.4.
+00001c00: 3004 3d04 3804 3504 3c00 2004 3d04 3e04  0.=.8.5.<. .=.>.
+00001c10: 3204 3e04 3900 2004 3e04 3f04 3504 4004  2.>.9. .>.?.5.@.
+00001c20: 3004 4604 3804 3808 0000 0000 0600 0000  0.F.8.8.........
+00001c30: 3555 6e73 6176 6564 2063 6861 6e67 6573  5Unsaved changes
+00001c40: 2077 6572 6520 7265 7665 7274 6564 2074   were reverted t
+00001c50: 6f20 6372 6561 7465 206e 6577 206f 7065  o create new ope
+00001c60: 7261 7469 6f6e 0700 0000 1841 6273 7472  ration.....Abstr
+00001c70: 6163 744f 7065 7261 7469 6f6e 4465 7461  actOperationDeta
+00001c80: 696c 7301 0300 0000 3a04 1d04 3504 3204  ils.....:...5.2.
+00001c90: 3504 4004 3d04 3e04 3500 2004 3704 3d04  5.@.=.>.5. .7.=.
+00001ca0: 3004 4704 3504 3d04 3804 3500 2004 3200  0.G.5.=.8.5. .2.
+00001cb0: 2004 4104 4204 3e04 3b04 3104 4604 3500   .A.B.>.;.1.F.5.
+00001cc0: 3a00 2008 0000 0000 0600 0000 1b43 6f6c  :. ..........Col
+00001cd0: 756d 6e20 6861 7320 6e6f 2076 616c 6964  umn has no valid
+00001ce0: 2076 616c 7565 3a20 0700 0000 1a41 6273   value: .....Abs
+00001cf0: 7472 6163 7452 6566 6572 656e 6365 4c69  tractReferenceLi
+00001d00: 7374 4d6f 6465 6c01 0300 0000 1e04 1d04  stModel.........
+00001d10: 3504 3f04 3e04 3b04 3d04 4b04 3500 2004  5.?.>.;.=.K.5. .
+00001d20: 3404 3004 3d04 3d04 4b04 3508 0000 0000  4.0.=.=.K.5.....
+00001d30: 0600 0000 1344 6174 6120 6172 6520 696e  .....Data are in
+00001d40: 636f 6d70 6c65 7465 0700 0000 1a41 6273  complete.....Abs
+00001d50: 7472 6163 7452 6566 6572 656e 6365 4c69  tractReferenceLi
+00001d60: 7374 4d6f 6465 6c01 0300 0000 2604 1e04  stModel.....&...
+00001d70: 4804 3804 3104 3a04 3000 2004 4104 3e04  H.8.1.:.0. .A.>.
+00001d80: 4504 4004 3004 3d04 3504 3d04 3804 4f00  E.@.0.=.5.=.8.O.
+00001d90: 3a00 2008 0000 0000 0600 0000 0f53 7562  :. ..........Sub
+00001da0: 6d69 7420 6661 696c 6564 3a20 0700 0000  mit failed: ....
+00001db0: 1a41 6273 7472 6163 7452 6566 6572 656e  .AbstractReferen
+00001dc0: 6365 4c69 7374 4d6f 6465 6c01 0300 0000  ceListModel.....
+00001dd0: 0a04 1b04 4e04 3104 3e04 3908 0000 0000  ....N.1.>.9.....
+00001de0: 0600 0000 0341 4e59 0700 0000 0d41 6363  .....ANY.....Acc
+00001df0: 6f75 6e74 4275 7474 6f6e 0103 0000 0014  ountButton......
+00001e00: 041b 044e 0431 043e 0439 0020 0441 0447  ...N.1.>.9. .A.G
+00001e10: 0435 0442 0800 0000 0006 0000 000b 416e  .5.B..........An
+00001e20: 7920 6163 636f 756e 7407 0000 000d 4163  y account.....Ac
+00001e30: 636f 756e 7442 7574 746f 6e01 0300 0000  countButton.....
+00001e40: 1804 1204 4b04 3104 4004 3004 4204 4c00  ....K.1.@.0.B.L.
+00001e50: 2004 4104 4704 3504 4208 0000 0000 0600   .A.G.5.B.......
+00001e60: 0000 0e43 686f 6f73 6520 6163 636f 756e  ...Choose accoun
+00001e70: 7407 0000 000d 4163 636f 756e 7442 7574  t.....AccountBut
+00001e80: 746f 6e01 0300 0000 1404 2204 3804 3f00  ton.......".8.?.
+00001e90: 2004 4104 4704 3504 4204 3000 3a08 0000   .A.G.5.B.0.:...
+00001ea0: 0000 0600 0000 0d41 6363 6f75 6e74 2074  .......Account t
+00001eb0: 7970 653a 0700 0000 1141 6363 6f75 6e74  ype:.....Account
+00001ec0: 4c69 7374 4469 616c 6f67 0103 0000 000a  ListDialog......
+00001ed0: 0421 0447 0435 0442 0430 0800 0000 0006  .!.G.5.B.0......
+00001ee0: 0000 0008 4163 636f 756e 7473 0700 0000  ....Accounts....
+00001ef0: 1141 6363 6f75 6e74 4c69 7374 4469 616c  .AccountListDial
+00001f00: 6f67 0103 0000 002a 041f 043e 043a 0430  og.....*...>.:.0
+00001f10: 0437 044b 0432 0430 0442 044c 0020 043d  .7.K.2.0.B.L. .=
+00001f20: 0435 0430 043a 0442 0438 0432 043d 044b  .5.0.:.B.8.2.=.K
+00001f30: 0435 0800 0000 0006 0000 000d 5368 6f77  .5..........Show
+00001f40: 2069 6e61 6374 6976 6507 0000 0011 4163   inactive.....Ac
+00001f50: 636f 756e 744c 6973 7444 6961 6c6f 6701  countListDialog.
+00001f60: 0300 0000 0e21 1600 2004 4104 4704 3504  .....!.. .A.G.5.
+00001f70: 4204 3008 0000 0000 0600 0000 0941 6363  B.0..........Acc
+00001f80: 6f75 6e74 2023 0700 0000 1041 6363 6f75  ount #.....Accou
+00001f90: 6e74 4c69 7374 4d6f 6465 6c01 0300 0000  ntListModel.....
+00001fa0: 0804 1004 3a04 4200 2e08 0000 0000 0600  ....:.B.........
+00001fb0: 0000 0441 6374 2e07 0000 0010 4163 636f  ...Act......Acco
+00001fc0: 756e 744c 6973 744d 6f64 656c 0103 0000  untListModel....
+00001fd0: 0016 0411 0430 043d 043a 002f 0411 0440  .....0.=.:./...@
+00001fe0: 043e 043a 0435 0440 0800 0000 0006 0000  .>.:.5.@........
+00001ff0: 000b 4261 6e6b 2f42 726f 6b65 7207 0000  ..Bank/Broker...
+00002000: 0010 4163 636f 756e 744c 6973 744d 6f64  ..AccountListMod
+00002010: 656c 0103 0000 0004 041a 0421 0800 0000  el.........!....
+00002020: 0006 0000 0002 4343 0700 0000 1041 6363  ......CC.....Acc
+00002030: 6f75 6e74 4c69 7374 4d6f 6465 6c01 0300  ountListModel...
+00002040: 0000 0c04 1204 3004 3b04 4e04 4204 3008  ......0.;.N.B.0.
+00002050: 0000 0000 0600 0000 0843 7572 7265 6e63  .........Currenc
+00002060: 7907 0000 0010 4163 636f 756e 744c 6973  y.....AccountLis
+00002070: 744d 6f64 656c 0103 0000 0018 041d 0430  tModel.........0
+00002080: 0438 043c 0435 043d 043e 0432 0430 043d  .8.<.5.=.>.2.0.=
+00002090: 0438 0435 0800 0000 0006 0000 0004 4e61  .8.5..........Na
+000020a0: 6d65 0700 0000 1041 6363 6f75 6e74 4c69  me.....AccountLi
+000020b0: 7374 4d6f 6465 6c01 0300 0000 1004 2204  stModel.......".
+000020c0: 3e04 4704 3d04 3e04 4104 4204 4c08 0000  >.G.=.>.A.B.L...
+000020d0: 0000 0600 0000 0950 7265 6369 7369 6f6e  .......Precision
+000020e0: 0700 0000 1041 6363 6f75 6e74 4c69 7374  .....AccountList
+000020f0: 4d6f 6465 6c01 0300 0000 1004 2104 3204  Model.......!.2.
+00002100: 3504 4004 3504 3d00 2000 4008 0000 0000  5.@.5.=. .@.....
+00002110: 0600 0000 0c52 6563 6f6e 6369 6c65 6420  .....Reconciled 
+00002120: 4007 0000 0010 4163 636f 756e 744c 6973  @.....AccountLis
+00002130: 744d 6f64 656c 0103 0000 001a 0426 0435  tModel.......&.5
+00002140: 043d 043d 0430 044f 0020 0431 0443 043c  .=.=.0.O. .1.C.<
+00002150: 0430 0433 0430 0800 0000 0006 0000 0005  .0.3.0..........
+00002160: 4173 7365 7407 0000 000b 4173 7365 7444  Asset.....AssetD
+00002170: 6961 6c6f 6701 0300 0000 3e04 1e04 4804  ialog.....>...H.
+00002180: 3804 3104 3a04 3000 2004 3704 3004 3f04  8.1.:.0. .7.0.?.
+00002190: 3804 4104 3800 2004 3804 3d04 4404 3e04  8.A.8. .8.=.D.>.
+000021a0: 4004 3c04 3004 4604 3804 3800 2004 3e00  @.<.0.F.8.8. .>.
+000021b0: 2004 2604 1100 3a00 2008 0000 0000 0600   .&...:. .......
+000021c0: 0000 1d41 7373 6574 2064 6574 6169 6c73  ...Asset details
+000021d0: 2073 7562 6d69 7420 6661 696c 6564 3a20   submit failed: 
+000021e0: 0700 0000 0b41 7373 6574 4469 616c 6f67  .....AssetDialog
+000021f0: 0103 0000 0024 041e 0448 0438 0431 043a  .....$...H.8.1.:
+00002200: 0430 0020 0437 0430 043f 0438 0441 0438  .0. .7.0.?.8.A.8
+00002210: 0020 0426 0415 003a 0020 0800 0000 0006  . .&...:. ......
+00002220: 0000 0015 4173 7365 7420 7375 626d 6974  ....Asset submit
+00002230: 2066 6169 6c65 643a 2007 0000 000b 4173   failed: .....As
+00002240: 7365 7444 6961 6c6f 6701 0300 0000 1c04  setDialog.......
+00002250: 1104 3004 3704 3e04 3204 4b04 3900 2004  ..0.7.>.2.K.9. .
+00002260: 3004 3a04 4204 3804 3200 3a08 0000 0000  0.:.B.8.2.:.....
+00002270: 0600 0000 0b42 6173 6520 6173 7365 743a  .....Base asset:
+00002280: 0700 0000 0b41 7373 6574 4469 616c 6f67  .....AssetDialog
+00002290: 0103 0000 000c 041e 0442 043c 0435 043d  .........B.<.5.=
+000022a0: 0430 0800 0000 0006 0000 0006 4361 6e63  .0..........Canc
+000022b0: 656c 0700 0000 0b41 7373 6574 4469 616c  el.....AssetDial
+000022c0: 6f67 0103 0000 0010 0421 0442 0440 0430  og.......!.B.@.0
+000022d0: 043d 0430 003a 0020 0800 0000 0006 0000  .=.0.:. ........
+000022e0: 0009 436f 756e 7472 793a 2007 0000 000b  ..Country: .....
+000022f0: 4173 7365 7444 6961 6c6f 6701 0300 0000  AssetDialog.....
+00002300: 1404 1404 3e04 3f00 2e04 3404 3004 3d04  ....>.?...4.0.=.
+00002310: 3d04 4b04 3508 0000 0000 0600 0000 0a45  =.K.5..........E
+00002320: 7874 7261 2064 6174 6107 0000 000b 4173  xtra data.....As
+00002330: 7365 7444 6961 6c6f 6701 0300 0000 0a00  setDialog.......
+00002340: 4900 5300 4900 4e00 3a08 0000 0000 0600  I.S.I.N.:.......
+00002350: 0000 0549 5349 4e3a 0700 0000 0b41 7373  ...ISIN:.....Ass
+00002360: 6574 4469 616c 6f67 0103 0000 001a 041d  etDialog........
+00002370: 0430 0438 043c 0435 043d 043e 0432 0430  .0.8.<.5.=.>.2.0
+00002380: 043d 0438 0435 003a 0800 0000 0006 0000  .=.8.5.:........
+00002390: 0005 4e61 6d65 3a07 0000 000b 4173 7365  ..Name:.....Asse
+000023a0: 7444 6961 6c6f 6701 0300 0000 0404 1e04  tDialog.........
+000023b0: 1a08 0000 0000 0600 0000 024f 4b07 0000  ...........OK...
+000023c0: 000b 4173 7365 7444 6961 6c6f 6701 0300  ..AssetDialog...
+000023d0: 0000 0e04 2104 3804 3c04 3204 3e04 3b04  ....!.8.<.2.>.;.
+000023e0: 4b08 0000 0000 0600 0000 0753 796d 626f  K..........Symbo
+000023f0: 6c73 0700 0000 0b41 7373 6574 4469 616c  ls.....AssetDial
+00002400: 6f67 0103 0000 000a 0422 0438 043f 003a  og.......".8.?.:
+00002410: 0020 0800 0000 0006 0000 0006 5479 7065  . ..........Type
+00002420: 3a20 0700 0000 0b41 7373 6574 4469 616c  : .....AssetDial
+00002430: 6f67 0103 0000 000e 0422 0438 043f 0020  og.......".8.?. 
+00002440: 0426 0411 003a 0800 0000 0006 0000 000b  .&...:..........
+00002450: 4173 7365 7420 7479 7065 3a07 0000 000f  Asset type:.....
+00002460: 4173 7365 744c 6973 7444 6961 6c6f 6701  AssetListDialog.
+00002470: 0300 0000 1a04 2604 3504 3d04 3d04 4b04  ......&.5.=.=.K.
+00002480: 3500 2004 3104 4304 3c04 3004 3304 3808  5. .1.C.<.0.3.8.
+00002490: 0000 0000 0600 0000 0641 7373 6574 7307  .........Assets.
+000024a0: 0000 000f 4173 7365 744c 6973 7444 6961  ....AssetListDia
+000024b0: 6c6f 6701 0300 0000 0c04 2104 4204 4004  log.......!.B.@.
+000024c0: 3004 3d04 3008 0000 0000 0600 0000 0743  0.=.0..........C
+000024d0: 6f75 6e74 7279 0700 0000 0e41 7373 6574  ountry.....Asset
+000024e0: 4c69 7374 4d6f 6465 6c01 0300 0000 0c04  ListModel.......
+000024f0: 1204 3004 3b04 4e04 4204 3008 0000 0000  ..0.;.N.B.0.....
+00002500: 0600 0000 0843 7572 7265 6e63 7907 0000  .....Currency...
+00002510: 000e 4173 7365 744c 6973 744d 6f64 656c  ..AssetListModel
+00002520: 0103 0000 001a 0418 0441 0442 002e 043a  .........A.B...:
+00002530: 043e 0442 0438 0440 043e 0432 043e 043a  .>.B.8.@.>.2.>.:
+00002540: 0800 0000 0006 0000 000b 4461 7461 2073  ..........Data s
+00002550: 6f75 7263 6507 0000 000e 4173 7365 744c  ource.....AssetL
+00002560: 6973 744d 6f64 656c 0103 0000 0008 0049  istModel.......I
+00002570: 0053 0049 004e 0800 0000 0006 0000 0004  .S.I.N..........
+00002580: 4953 494e 0700 0000 0e41 7373 6574 4c69  ISIN.....AssetLi
+00002590: 7374 4d6f 6465 6c01 0300 0000 1804 1d04  stModel.........
+000025a0: 3004 3804 3c04 3504 3d04 3e04 3204 3004  0.8.<.5.=.>.2.0.
+000025b0: 3d04 3804 3508 0000 0000 0600 0000 044e  =.8.5..........N
+000025c0: 616d 6507 0000 000e 4173 7365 744c 6973  ame.....AssetLis
+000025d0: 744d 6f64 656c 0103 0000 000c 0421 0438  tModel.......!.8
+000025e0: 043c 0432 043e 043b 0800 0000 0006 0000  .<.2.>.;........
+000025f0: 0006 5379 6d62 6f6c 0700 0000 0e41 7373  ..Symbol.....Ass
+00002600: 6574 4c69 7374 4d6f 6465 6c01 0300 0000  etListModel.....
+00002610: 1804 1d04 3004 3804 3c04 3504 3d04 3e04  ....0.8.<.5.=.>.
+00002620: 3204 3004 3d04 3804 3508 0000 0000 0600  2.0.=.8.5.......
+00002630: 0000 0a41 7373 6574 206e 616d 6507 0000  ...Asset name...
+00002640: 000f 4173 7365 7473 4c69 7374 4d6f 6465  ..AssetsListMode
+00002650: 6c01 0300 0000 1a04 1104 3004 3704 3e04  l.........0.7.>.
+00002660: 3204 4b04 3900 2004 3004 3a04 4204 3804  2.K.9. .0.:.B.8.
+00002670: 3208 0000 0000 0600 0000 0a42 6173 6520  2..........Base 
+00002680: 6173 7365 7407 0000 000f 4173 7365 7473  asset.....Assets
+00002690: 4c69 7374 4d6f 6465 6c01 0300 0000 0c04  ListModel.......
+000026a0: 2104 4204 4004 3004 3d04 3008 0000 0000  !.B.@.0.=.0.....
+000026b0: 0600 0000 0743 6f75 6e74 7279 0700 0000  .....Country....
+000026c0: 0f41 7373 6574 734c 6973 744d 6f64 656c  .AssetsListModel
+000026d0: 0103 0000 0008 0049 0053 0049 004e 0800  .......I.S.I.N..
+000026e0: 0000 0006 0000 0004 4953 494e 0700 0000  ........ISIN....
+000026f0: 0f41 7373 6574 734c 6973 744d 6f64 656c  .AssetsListModel
+00002700: 0103 0000 0008 0421 0447 0435 0442 0800  .......!.G.5.B..
+00002710: 0000 0006 0000 0007 4163 636f 756e 7407  ........Account.
+00002720: 0000 000d 4261 6c61 6e63 6573 4d6f 6465  ....BalancesMode
+00002730: 6c01 0300 0000 0c04 1104 3004 3b04 3004  l.........0.;.0.
+00002740: 3d04 4108 0000 0000 0600 0000 0742 616c  =.A..........Bal
+00002750: 616e 6365 0700 0000 0d42 616c 616e 6365  ance.....Balance
+00002760: 734d 6f64 656c 0103 0000 0010 0411 0430  sModel.........0
+00002770: 043b 0430 043d 0441 002c 0020 0800 0000  .;.0.=.A.,. ....
+00002780: 0006 0000 0009 4261 6c61 6e63 652c 2007  ......Balance, .
+00002790: 0000 000d 4261 6c61 6e63 6573 4d6f 6465  ....BalancesMode
+000027a0: 6c01 0300 0000 0a04 1804 4204 3e04 3304  l.........B.>.3.
+000027b0: 3e08 0000 0000 0600 0000 0554 6f74 616c  >..........Total
+000027c0: 0700 0000 0d42 616c 616e 6365 734d 6f64  .....BalancesMod
+000027d0: 656c 0103 0000 001c 0411 0430 0437 043e  el.........0.7.>
+000027e0: 0432 0430 044f 0020 0432 0430 043b 044e  .2.0.O. .2.0.;.N
+000027f0: 0442 0430 0800 0000 0006 0000 000d 4261  .B.0..........Ba
+00002800: 7365 2063 7572 7265 6e63 7907 0000 0012  se currency.....
+00002810: 4261 7365 4375 7272 656e 6379 4469 616c  BaseCurrencyDial
+00002820: 6f67 0103 0000 000c 0412 0430 043b 044e  og.........0.;.N
+00002830: 0442 0430 0800 0000 0006 0000 0008 4375  .B.0..........Cu
+00002840: 7272 656e 6379 0700 0000 1542 6173 6543  rrency.....BaseC
+00002850: 7572 7265 6e63 794c 6973 744d 6f64 656c  urrencyListModel
+00002860: 0103 0000 0008 0414 0430 0442 0430 0800  .........0.B.0..
+00002870: 0000 0006 0000 0004 4461 7465 0700 0000  ........Date....
+00002880: 1542 6173 6543 7572 7265 6e63 794c 6973  .BaseCurrencyLis
+00002890: 744d 6f64 656c 0103 0000 0024 0027 0020  tModel.....$.'. 
+000028a0: 0437 0430 043c 0435 043d 0435 043d 0430  .7.0.<.5.=.5.=.0
+000028b0: 0020 0443 0441 043f 0435 0448 043d 043e  . .C.A.?.5.H.=.>
+000028c0: 0800 0000 0006 0000 001b 2720 7761 7320  ..........' was 
+000028d0: 7375 6363 6573 7366 756c 6c79 2072 6570  successfully rep
+000028e0: 6c61 6365 6407 0000 0012 4361 7465 676f  laced.....Catego
+000028f0: 7279 4c69 7374 4469 616c 6f67 0103 0000  ryListDialog....
+00002900: 000c 0027 0020 043d 0430 003a 0020 0800  ...'. .=.0.:. ..
+00002910: 0000 0006 0000 0008 2720 7769 7468 3a20  ........' with: 
+00002920: 0700 0000 1243 6174 6567 6f72 794c 6973  .....CategoryLis
+00002930: 7444 6961 6c6f 6701 0300 0000 1204 1a04  tDialog.........
+00002940: 3004 4204 3504 3304 3e04 4004 3804 3808  0.B.5.3.>.@.8.8.
+00002950: 0000 0000 0600 0000 0a43 6174 6567 6f72  .........Categor
+00002960: 6965 7307 0000 0012 4361 7465 676f 7279  ies.....Category
+00002970: 4c69 7374 4469 616c 6f67 0103 0000 0016  ListDialog......
+00002980: 041a 0430 0442 0435 0433 043e 0440 0438  ...0.B.5.3.>.@.8
+00002990: 044f 0020 0027 0800 0000 0006 0000 000a  .O. .'..........
+000029a0: 4361 7465 676f 7279 2027 0700 0000 1243  Category '.....C
+000029b0: 6174 6567 6f72 794c 6973 7444 6961 6c6f  ategoryListDialo
+000029c0: 6701 0300 0000 2804 1704 3004 3c04 3504  g.....(...0.<.5.
+000029d0: 3d04 3804 4204 4c00 2004 3a04 3004 4204  =.8.B.L. .:.0.B.
+000029e0: 3504 3304 3e04 4004 3804 4e00 2000 2708  5.3.>.@.8.N. .'.
+000029f0: 0000 0000 0600 0000 1252 6570 6c61 6365  .........Replace
+00002a00: 2063 6174 6567 6f72 7920 2707 0000 0012   category '.....
+00002a10: 4361 7465 676f 7279 4c69 7374 4469 616c  CategoryListDial
+00002a20: 6f67 0103 0000 001c 0417 0430 043c 0435  og.........0.<.5
+00002a30: 043d 0438 0442 044c 0020 043d 0430 002e  .=.8.B.L. .=.0..
+00002a40: 002e 002e 0800 0000 0006 0000 000f 5265  ..............Re
+00002a50: 706c 6163 6520 7769 7468 2e2e 2e07 0000  place with......
+00002a60: 0012 4361 7465 676f 7279 4c69 7374 4469  ..CategoryListDi
+00002a70: 616c 6f67 0103 0000 003c 041f 043e 043a  alog.....<...>.:
+00002a80: 0430 0437 0430 0442 044c 0020 043e 043f  .0.7.0.B.L. .>.?
+00002a90: 0435 0440 0430 0446 0438 0438 0020 0441  .5.@.0.F.8.8. .A
+00002aa0: 0020 041a 0430 0442 0435 0433 043e 0440  . ...0.B.5.3.>.@
+00002ab0: 0438 0435 0439 0800 0000 0006 0000 001d  .8.5.9..........
+00002ac0: 5368 6f77 206f 7065 7261 7469 6f6e 7320  Show operations 
+00002ad0: 7769 7468 2043 6174 6567 6f72 7907 0000  with Category...
+00002ae0: 0012 4361 7465 676f 7279 4c69 7374 4469  ..CategoryListDi
+00002af0: 616c 6f67 0103 0000 0010 041e 043f 0435  alog.........?.5
+00002b00: 0440 0430 0446 0438 0438 0800 0000 0006  .@.0.F.8.8......
+00002b10: 0000 000a 4f70 6572 6174 696f 6e73 0700  ....Operations..
+00002b20: 0000 0e43 6174 6567 6f72 7952 6570 6f72  ...CategoryRepor
+00002b30: 7401 0300 0000 1804 3f04 3e00 2004 1a04  t.......?.>. ...
+00002b40: 3004 4204 3504 3304 3e04 4004 3804 3808  0.B.5.3.>.@.8.8.
+00002b50: 0000 0000 0600 0000 0b62 7920 4361 7465  .........by Cate
+00002b60: 676f 7279 0700 0000 0e43 6174 6567 6f72  gory.....Categor
+00002b70: 7952 6570 6f72 7401 0300 0000 1404 1a04  yReport.........
+00002b80: 3004 4204 3504 3304 3e04 4004 3804 4f00  0.B.5.3.>.@.8.O.
+00002b90: 3a08 0000 0000 0600 0000 0943 6174 6567  :..........Categ
+00002ba0: 6f72 793a 0700 0000 1443 6174 6567 6f72  ory:.....Categor
+00002bb0: 7952 6570 6f72 7457 6964 6765 7401 0300  yReportWidget...
+00002bc0: 0000 2404 1e04 4204 4704 5104 4200 2004  ..$...B.G.Q.B. .
+00002bd0: 3f04 3e00 2004 3a04 3004 4204 3504 3304  ?.>. .:.0.B.5.3.
+00002be0: 3e04 4004 3804 3808 0000 0000 0600 0000  >.@.8.8.........
+00002bf0: 1252 6570 6f72 7420 6279 2063 6174 6567  .Report by categ
+00002c00: 6f72 7907 0000 0014 4361 7465 676f 7279  ory.....Category
+00002c10: 5265 706f 7274 5769 6467 6574 0103 0000  ReportWidget....
+00002c20: 0018 041d 0430 0438 043c 0435 043d 043e  .....0.8.<.5.=.>
+00002c30: 0432 0430 043d 0438 0435 0800 0000 0006  .2.0.=.8.5......
+00002c40: 0000 0004 4e61 6d65 0700 0000 1143 6174  ....Name.....Cat
+00002c50: 6567 6f72 7954 7265 654d 6f64 656c 0103  egoryTreeModel..
+00002c60: 0000 000c 0427 0430 0441 0442 0430 044f  .....'.0.A.B.0.O
+00002c70: 0800 0000 0006 0000 0005 4f66 7465 6e07  ..........Often.
+00002c80: 0000 0011 4361 7465 676f 7279 5472 6565  ....CategoryTree
+00002c90: 4d6f 6465 6c01 0300 0000 2004 1304 4004  Model..... ...@.
+00002ca0: 3004 4404 3804 3a00 2004 4604 3504 3d04  0.D.8.:. .F.5.=.
+00002cb0: 4b00 2004 3404 3b04 4f00 2008 0000 0000  K. .4.;.O. .....
+00002cc0: 0600 0000 1050 7269 6365 2063 6861 7274  .....Price chart
+00002cd0: 2066 6f72 2007 0000 000b 4368 6172 7457   for .....ChartW
+00002ce0: 696e 646f 7701 0300 0000 1a04 2604 3504  indow.......&.5.
+00002cf0: 3d04 3d04 3004 4f00 2004 3104 4304 3c04  =.=.0.O. .1.C.<.
+00002d00: 3004 3304 3008 0000 0000 0600 0000 0541  0.3.0..........A
+00002d10: 7373 6574 0700 0000 1143 6c6f 7365 6454  sset.....ClosedT
+00002d20: 7261 6465 734d 6f64 656c 0103 0000 001a  radesModel......
+00002d30: 0414 0430 0442 0430 0020 0437 0430 043a  ...0.B.0. .7.0.:
+00002d40: 0440 044b 0442 0438 044f 0800 0000 0006  .@.K.B.8.O......
+00002d50: 0000 000a 436c 6f73 6520 4461 7465 0700  ....Close Date..
+00002d60: 0000 1143 6c6f 7365 6454 7261 6465 734d  ...ClosedTradesM
+00002d70: 6f64 656c 0103 0000 0026 0414 0430 0442  odel.....&...0.B
+00002d80: 0430 002f 0432 0440 0435 043c 044f 0020  .0./.2.@.5.<.O. 
+00002d90: 0437 0430 043a 0440 044b 0442 0438 044f  .7.0.:.@.K.B.8.O
+00002da0: 0800 0000 0006 0000 000f 436c 6f73 6520  ..........Close 
+00002db0: 4461 7465 2f54 696d 6507 0000 0011 436c  Date/Time.....Cl
+00002dc0: 6f73 6564 5472 6164 6573 4d6f 6465 6c01  osedTradesModel.
+00002dd0: 0300 0000 1a04 2604 3504 3d04 3000 2004  ......&.5.=.0. .
+00002de0: 3704 3004 3a04 4004 4b04 4204 3804 4f08  7.0.:.@.K.B.8.O.
+00002df0: 0000 0000 0600 0000 0b43 6c6f 7365 2050  .........Close P
+00002e00: 7269 6365 0700 0000 1143 6c6f 7365 6454  rice.....ClosedT
+00002e10: 7261 6465 734d 6f64 656c 0103 0000 0010  radesModel......
+00002e20: 041a 043e 043c 0438 0441 0441 0438 044f  ...>.<.8.A.A.8.O
+00002e30: 0800 0000 0006 0000 0003 4665 6507 0000  ..........Fee...
+00002e40: 0011 436c 6f73 6564 5472 6164 6573 4d6f  ..ClosedTradesMo
+00002e50: 6465 6c01 0300 0000 1404 1f04 4004 3804  del.........@.8.
+00002e60: 3c04 3504 4704 3004 3d04 3804 3508 0000  <.5.G.0.=.8.5...
+00002e70: 0000 0600 0000 044e 6f74 6507 0000 0011  .......Note.....
+00002e80: 436c 6f73 6564 5472 6164 6573 4d6f 6465  ClosedTradesMode
+00002e90: 6c01 0300 0000 1a04 1404 3004 4204 3000  l.........0.B.0.
+00002ea0: 2004 3e04 4204 3a04 4004 4b04 4204 3804   .>.B.:.@.K.B.8.
+00002eb0: 4f08 0000 0000 0600 0000 094f 7065 6e20  O..........Open 
+00002ec0: 4461 7465 0700 0000 1143 6c6f 7365 6454  Date.....ClosedT
+00002ed0: 7261 6465 734d 6f64 656c 0103 0000 0026  radesModel.....&
+00002ee0: 0414 0430 0442 0430 002f 0412 0440 0435  ...0.B.0./...@.5
+00002ef0: 043c 044f 0020 043e 0442 043a 0440 044b  .<.O. .>.B.:.@.K
+00002f00: 0442 0438 044f 0800 0000 0006 0000 000e  .B.8.O..........
+00002f10: 4f70 656e 2044 6174 652f 5469 6d65 0700  Open Date/Time..
+00002f20: 0000 1143 6c6f 7365 6454 7261 6465 734d  ...ClosedTradesM
+00002f30: 6f64 656c 0103 0000 001a 0426 0435 043d  odel.......&.5.=
+00002f40: 0430 0020 043e 0442 043a 0440 044b 0442  .0. .>.B.:.@.K.B
+00002f50: 0438 044f 0800 0000 0006 0000 000a 4f70  .8.O..........Op
+00002f60: 656e 2050 7269 6365 0700 0000 1143 6c6f  en Price.....Clo
+00002f70: 7365 6454 7261 6465 734d 6f64 656c 0103  sedTradesModel..
+00002f80: 0000 0006 041f 0438 0423 0800 0000 0006  .......8.#......
+00002f90: 0000 0003 502f 4c07 0000 0011 436c 6f73  ....P/L.....Clos
 00002fa0: 6564 5472 6164 6573 4d6f 6465 6c01 0300  edTradesModel...
-00002fb0: 0000 0c04 1a04 3e04 3b00 2d04 3204 3e08  ......>.;.-.2.>.
-00002fc0: 0000 0000 0600 0000 0351 7479 0700 0000  .........Qty....
-00002fd0: 1143 6c6f 7365 6454 7261 6465 734d 6f64  .ClosedTradesMod
-00002fe0: 656c 0103 0000 00a0 041a 043e 043b 0438  el.........>.;.8
-00002ff0: 0447 0435 0442 0432 043e 0020 0446 0435  .G.5.B.2.>. .F.5
-00003000: 043d 043d 044b 0445 0020 0431 0443 043c  .=.=.K.E. .1.C.<
-00003010: 0430 0433 0020 043d 0435 0434 043e 0441  .0.3. .=.5.4.>.A
-00003020: 0442 0430 0442 043e 0447 043d 043e 0020  .B.0.B.>.G.=.>. 
-00003030: 0434 043b 044f 0020 043e 0431 0440 0430  .4.;.O. .>.1.@.0
-00003040: 0431 043e 0442 043a 0438 0020 043a 043e  .1.>.B.:.8. .:.>
-00003050: 0440 043f 043e 0440 0430 0442 0438 0432  .@.?.>.@.0.B.8.2
-00003060: 043d 043e 0433 043e 0020 0441 043e 0431  .=.>.3.>. .A.>.1
-00003070: 044b 0442 0438 044f 002e 0020 0414 0430  .K.B.8.O... ...0
-00003080: 0442 0430 003a 0020 0800 0000 0006 0000  .B.0.:. ........
-00003090: 0042 4173 7365 7420 616d 6f75 6e74 2069  .BAsset amount i
-000030a0: 7320 6e6f 7420 656e 6f75 6768 2066 6f72  s not enough for
-000030b0: 2063 6f72 706f 7261 7465 2061 6374 696f   corporate actio
-000030c0: 6e20 7072 6f63 6573 7369 6e67 2e20 4461  n processing. Da
-000030d0: 7465 3a20 0700 0000 0f43 6f72 706f 7261  te: .....Corpora
-000030e0: 7465 4163 7469 6f6e 0103 0000 0074 0426  teAction.....t.&
-000030f0: 0411 0020 043d 0435 0020 044f 0432 043b  ... .=.5. .O.2.;
-00003100: 044f 0435 0442 0441 044f 0020 0447 0430  .O.5.B.A.O. .G.0
-00003110: 0441 0442 044c 044e 0020 0440 0435 0437  .A.B.L.N. .@.5.7
-00003120: 0443 043b 044c 0442 0430 0442 043e 0432  .C.;.L.B.0.B.>.2
-00003130: 0020 043a 043e 0440 043f 043e 0440 0430  . .:.>.@.?.>.@.0
-00003140: 0442 0438 0432 043d 043e 0433 043e 0020  .B.8.2.=.>.3.>. 
-00003150: 0441 043e 0431 044b 0442 0438 044f 003a  .A.>.1.K.B.8.O.:
-00003160: 0020 0800 0000 0006 0000 0030 4173 7365  . .........0Asse
-00003170: 7420 6973 6e27 7420 6120 7061 7274 206f  t isn't a part o
-00003180: 6620 636f 7270 6f72 6174 6520 6163 7469  f corporate acti
-00003190: 6f6e 2072 6573 756c 7473 3a20 0700 0000  on results: ....
-000031a0: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
-000031b0: 0103 0000 0056 041d 0435 0020 0437 0430  .....V...5. .7.0
-000031c0: 0434 0430 043d 0020 0442 0438 043f 0020  .4.0.=. .B.8.?. 
-000031d0: 043a 043e 0440 043f 043e 0440 0430 0442  .:.>.@.?.>.@.0.B
-000031e0: 0438 0432 043d 043e 0433 043e 0020 0441  .8.2.=.>.3.>. .A
-000031f0: 043e 0431 044b 0442 0438 044f 002e 0020  .>.1.K.B.8.O... 
-00003200: 0414 0430 0442 0430 003a 0020 0800 0000  ...0.B.0.:. ....
-00003210: 0006 0000 002b 436f 7270 6f72 6174 6520  .....+Corporate 
-00003220: 6163 7469 6f6e 2074 7970 6520 6973 6e27  action type isn'
-00003230: 7420 6465 6669 6e65 642e 2044 6174 653a  t defined. Date:
-00003240: 2007 0000 000f 436f 7270 6f72 6174 6541   .....CorporateA
-00003250: 6374 696f 6e01 0300 0000 1204 1404 3504  ction.........5.
-00003260: 3b04 3804 4104 4204 3804 3d04 3308 0000  ;.8.A.B.8.=.3...
-00003270: 0000 0600 0000 0944 656c 6973 7469 6e67  .......Delisting
-00003280: 0700 0000 0f43 6f72 706f 7261 7465 4163  .....CorporateAc
-00003290: 7469 6f6e 0103 0000 002c 0420 0435 043e  tion.....,. .5.>
-000032a0: 0440 0433 0430 043d 0438 0437 0430 0446  .@.3.0.=.8.7.0.F
-000032b0: 0438 044f 0020 043a 043e 043c 043f 0430  .8.O. .:.>.<.?.0
-000032c0: 043d 0438 0438 0800 0000 0006 0000 0006  .=.8.8..........
-000032d0: 4d65 7267 6572 0700 0000 0f43 6f72 706f  Merger.....Corpo
-000032e0: 7261 7465 4163 7469 6f6e 0103 0000 00ac  rateAction......
-000032f0: 0420 0435 0437 0443 043b 044c 0442 0430  . .5.7.C.;.L.B.0
-00003300: 0442 044b 0020 043a 043e 0440 043f 043e  .B.K. .:.>.@.?.>
-00003310: 0440 0430 0442 0438 0432 043d 043e 0433  .@.0.B.8.2.=.>.3
-00003320: 043e 0020 0441 043e 0431 044b 0442 0438  .>. .A.>.1.K.B.8
-00003330: 044f 0020 043d 0435 0020 0440 0430 0441  .O. .=.5. .@.0.A
-00003340: 043f 0440 0435 0434 0435 043b 044f 044e  .?.@.5.4.5.;.O.N
-00003350: 0442 0020 0031 0030 0030 0025 0020 0441  .B. .1.0.0.%. .A
-00003360: 0442 043e 0438 043c 043e 0441 0442 0438  .B.>.8.<.>.A.B.8
-00003370: 0020 0438 0437 043d 0430 0447 0430 043b  . .8.7.=.0.G.0.;
-00003380: 044c 043d 043e 0433 043e 0020 0430 043a  .L.=.>.3.>. .0.:
-00003390: 0442 0438 0432 0430 002e 0020 0800 0000  .B.8.2.0... ....
-000033a0: 0006 0000 004d 5265 7375 6c74 7320 7661  .....MResults va
-000033b0: 6c75 6520 6f66 2063 6f72 706f 7261 7465  lue of corporate
-000033c0: 2061 6374 696f 6e20 646f 6573 6e27 7420   action doesn't 
-000033d0: 6d61 7463 6820 3130 3025 206f 6620 696e  match 100% of in
-000033e0: 6974 6961 6c20 6173 7365 7420 7661 6c75  itial asset valu
-000033f0: 652e 2007 0000 000f 436f 7270 6f72 6174  e. .....Corporat
-00003400: 6541 6374 696f 6e01 0300 0000 3a04 1204  eAction.....:...
-00003410: 4b04 3404 3504 3b04 3504 3d04 3804 3500  K.4.5.;.5.=.8.5.
-00003420: 2004 3a04 3e04 3c04 3f04 3004 3d04 3804   .:.>.<.?.0.=.8.
-00003430: 3800 2000 2804 4104 3f04 3804 3d00 2d04  8. .(.A.?.8.=.-.
-00003440: 3e04 4404 4400 2908 0000 0000 0600 0000  >.D.D.).........
-00003450: 0853 7069 6e2d 6f66 6607 0000 000f 436f  .Spin-off.....Co
-00003460: 7270 6f72 6174 6541 6374 696f 6e01 0300  rporateAction...
-00003470: 0000 0a04 2104 3f04 3b04 3804 4208 0000  ....!.?.;.8.B...
-00003480: 0000 0600 0000 0553 706c 6974 0700 0000  .......Split....
-00003490: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
-000034a0: 0103 0000 001a 0421 043c 0435 043d 0430  .......!.<.5.=.0
-000034b0: 0020 0441 0438 043c 0432 043e 043b 0430  . .A.8.<.2.>.;.0
-000034c0: 0800 0000 0006 0000 000d 5379 6d62 6f6c  ..........Symbol
-000034d0: 2063 6861 6e67 6507 0000 000f 436f 7270   change.....Corp
-000034e0: 6f72 6174 6541 6374 696f 6e01 0300 0000  orateAction.....
-000034f0: 1804 1d04 1504 1e04 1f04 2004 1504 1404  .......... .....
-00003500: 1504 1b04 1504 1d04 1e08 0000 0000 0600  ................
-00003510: 0000 0955 4e44 4546 494e 4544 0700 0000  ...UNDEFINED....
-00003520: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
-00003530: 0103 0000 00ae 041d 0435 043f 043e 0434  .........5.?.>.4
-00003540: 0435 0440 0436 0438 0432 0430 0435 043c  .5.@.6.8.2.0.5.<
-00003550: 044b 0439 0020 0441 043b 0443 0447 0430  .K.9. .A.;.C.G.0
-00003560: 0439 003a 0020 041a 043e 0440 043f 043e  .9.:. ...>.@.?.>
-00003570: 0440 0430 0442 0438 0432 043d 043e 0435  .@.0.B.8.2.=.>.5
-00003580: 0020 0441 043e 0431 044b 0442 0438 0435  . .A.>.1.K.B.8.5
-00003590: 0020 043f 043e 043a 0440 044b 0432 0430  . .?.>.:.@.K.2.0
-000035a0: 0435 0442 0020 043d 0435 0020 0432 0441  .5.B. .=.5. .2.A
-000035b0: 044e 0020 043e 0442 043a 0440 044b 0442  .N. .>.B.:.@.K.B
-000035c0: 0443 044e 0020 043f 043e 0437 0438 0446  .C.N. .?.>.7.8.F
-000035d0: 0438 044e 002e 0020 0414 0430 0442 0430  .8.N... ...0.B.0
-000035e0: 003a 0020 0800 0000 0006 0000 0046 556e  .:. .........FUn
-000035f0: 6861 6e64 6c65 6420 6361 7365 3a20 436f  handled case: Co
-00003600: 7270 6f72 6174 6520 6163 7469 6f6e 2063  rporate action c
-00003610: 6f76 6572 7320 6e6f 7420 6675 6c6c 206f  overs not full o
-00003620: 7065 6e20 706f 7369 7469 6f6e 2e20 4461  pen position. Da
-00003630: 7465 3a20 0700 0000 0f43 6f72 706f 7261  te: .....Corpora
-00003640: 7465 4163 7469 6f6e 0103 0000 0002 2116  teAction......!.
-00003650: 0800 0000 0006 0000 0001 2307 0000 0015  ..........#.....
-00003660: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
-00003670: 6964 6765 7401 0300 0000 0804 2104 4704  idget.......!.G.
-00003680: 3504 4208 0000 0000 0600 0000 0741 6363  5.B..........Acc
-00003690: 6f75 6e74 0700 0000 1543 6f72 706f 7261  ount.....Corpora
-000036a0: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
-000036b0: 0000 001c 0414 043e 0431 0430 0432 0438  .......>.1.0.2.8
-000036c0: 0442 044c 0020 0430 043a 0442 0438 0432  .B.L. .0.:.B.8.2
-000036d0: 0800 0000 0006 0000 0009 4164 6420 6173  ..........Add as
-000036e0: 7365 7407 0000 0015 436f 7270 6f72 6174  set.....Corporat
-000036f0: 6541 6374 696f 6e57 6964 6765 7401 0300  eActionWidget...
-00003700: 0000 0404 2604 1108 0000 0000 0600 0000  ....&...........
-00003710: 0541 7373 6574 0700 0000 1543 6f72 706f  .Asset.....Corpo
-00003720: 7261 7465 4163 7469 6f6e 5769 6467 6574  rateActionWidget
-00003730: 0103 0000 002c 041a 043e 0440 043f 043e  .....,...>.@.?.>
-00003740: 0440 0430 0442 0438 0432 043d 043e 0435  .@.0.B.8.2.=.>.5
-00003750: 0020 0434 0435 0439 0441 0442 0432 0438  . .4.5.9.A.B.2.8
-00003760: 0435 0800 0000 0006 0000 0010 436f 7270  .5..........Corp
-00003770: 6f72 6174 6520 4163 7469 6f6e 0700 0000  orate Action....
-00003780: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
-00003790: 5769 6467 6574 0103 0000 0014 0414 0430  Widget.........0
-000037a0: 0442 0430 002f 0412 0440 0435 043c 044f  .B.0./...@.5.<.O
-000037b0: 0800 0000 0006 0000 0009 4461 7465 2f54  ..........Date/T
-000037c0: 696d 6507 0000 0015 436f 7270 6f72 6174  ime.....Corporat
-000037d0: 6541 6374 696f 6e57 6964 6765 7401 0300  eActionWidget...
-000037e0: 0000 1204 1404 3504 3b04 3804 4104 4204  ......5.;.8.A.B.
-000037f0: 3804 3d04 3308 0000 0000 0600 0000 0944  8.=.3..........D
-00003800: 656c 6973 7469 6e67 0700 0000 1543 6f72  elisting.....Cor
-00003810: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
-00003820: 6574 0103 0000 0044 041d 0435 0432 043e  et.....D...5.2.>
-00003830: 0437 043c 043e 0436 043d 043e 0020 0434  .7.<.>.6.=.>. .4
-00003840: 043e 0431 0430 0432 0438 0442 044c 0020  .>.1.0.2.8.B.L. 
-00003850: 043d 043e 0432 0443 044e 0020 0437 0430  .=.>.2.C.N. .7.0
-00003860: 043f 0438 0441 044c 003a 0020 0800 0000  .?.8.A.L.:. ....
-00003870: 0006 0000 001a 4661 696c 6564 2074 6f20  ......Failed to 
-00003880: 6164 6420 6e65 7720 7265 636f 7264 3a20  add new record: 
-00003890: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
-000038a0: 7469 6f6e 5769 6467 6574 0103 0000 0028  tionWidget.....(
-000038b0: 041e 0431 044a 0435 0434 0438 043d 0435  ...1.J.5.4.8.=.5
-000038c0: 043d 0438 0435 0020 043a 043e 043c 043f  .=.8.5. .:.>.<.?
-000038d0: 0430 043d 0438 0438 0800 0000 0006 0000  .0.=.8.8........
-000038e0: 0006 4d65 7267 6572 0700 0000 1543 6f72  ..Merger.....Cor
-000038f0: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
-00003900: 6574 0103 0000 0006 004e 002f 0041 0800  et.......N./.A..
-00003910: 0000 0006 0000 0003 4e2f 4107 0000 0015  ........N/A.....
-00003920: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
-00003930: 6964 6765 7401 0300 0000 1004 1e04 3f04  idget.........?.
-00003940: 3804 4104 3004 3d04 3804 3508 0000 0000  8.A.0.=.8.5.....
-00003950: 0600 0000 044e 6f74 6507 0000 0015 436f  .....Note.....Co
-00003960: 7270 6f72 6174 6541 6374 696f 6e57 6964  rporateActionWid
-00003970: 6765 7401 0300 0000 4804 1e04 4804 3804  get.....H...H.8.
-00003980: 3104 3a04 3000 2004 3f04 4004 3800 2004  1.:.0. .?.@.8. .
-00003990: 3704 3004 3f04 3804 4104 3800 2004 3404  7.0.?.8.A.8. .4.
-000039a0: 3504 4204 3004 3b04 3504 3900 2004 3e04  5.B.0.;.5.9. .>.
-000039b0: 3f04 3504 4004 3004 4604 3804 3800 3a00  ?.5.@.0.F.8.8.:.
-000039c0: 2008 0000 0000 0600 0000 214f 7065 7261   .........!Opera
-000039d0: 7469 6f6e 2064 6574 6169 6c73 2073 7562  tion details sub
-000039e0: 6d69 7420 6661 696c 6564 3a20 0700 0000  mit failed: ....
-000039f0: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
-00003a00: 5769 6467 6574 0103 0000 0038 041e 0448  Widget.....8...H
-00003a10: 0438 0431 043a 0430 0020 043f 0440 0438  .8.1.:.0. .?.@.8
-00003a20: 0020 0437 0430 043f 0438 0441 0438 0020  . .7.0.?.8.A.8. 
-00003a30: 043e 043f 0435 0440 0430 0446 0438 0438  .>.?.5.@.0.F.8.8
-00003a40: 003a 0020 0800 0000 0006 0000 0019 4f70  .:. ..........Op
-00003a50: 6572 6174 696f 6e20 7375 626d 6974 2066  eration submit f
-00003a60: 6169 6c65 643a 2007 0000 0015 436f 7270  ailed: .....Corp
-00003a70: 6f72 6174 6541 6374 696f 6e57 6964 6765  orateActionWidge
-00003a80: 7401 0300 0000 0c04 1a04 3e04 3b00 2d04  t.........>.;.-.
-00003a90: 3204 3e08 0000 0000 0600 0000 0351 7479  2.>..........Qty
-00003aa0: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
-00003ab0: 7469 6f6e 5769 6467 6574 0103 0000 001a  tionWidget......
-00003ac0: 0423 0434 0430 043b 0438 0442 044c 0020  .#.4.0.;.8.B.L. 
-00003ad0: 0430 043a 0442 0438 0432 0800 0000 0006  .0.:.B.8.2......
-00003ae0: 0000 000c 5265 6d6f 7665 2061 7373 6574  ....Remove asset
-00003af0: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
-00003b00: 7469 6f6e 5769 6467 6574 0103 ffff ffff  tionWidget......
-00003b10: 0800 0000 0006 0000 0008 5370 696e 2d4f  ..........Spin-O
-00003b20: 6666 0700 0000 1543 6f72 706f 7261 7465  ff.....Corporate
-00003b30: 4163 7469 6f6e 5769 6467 6574 0103 0000  ActionWidget....
-00003b40: 000a 0421 043f 043b 0438 0442 0800 0000  ...!.?.;.8.B....
-00003b50: 0006 0000 0005 5370 6c69 7407 0000 0015  ......Split.....
-00003b60: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
-00003b70: 6964 6765 7401 0300 0000 1a04 2104 3c04  idget.......!.<.
-00003b80: 3504 3d04 3000 2004 4104 3804 3c04 3204  5.=.0. .A.8.<.2.
-00003b90: 3e04 3b04 3008 0000 0000 0600 0000 0d53  >.;.0..........S
-00003ba0: 796d 626f 6c20 6368 616e 6765 0700 0000  ymbol change....
-00003bb0: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
-00003bc0: 5769 6467 6574 0103 0000 0006 0422 0438  Widget.......".8
-00003bd0: 043f 0800 0000 0006 0000 0004 5479 7065  .?..........Type
-00003be0: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
-00003bf0: 7469 6f6e 5769 6467 6574 0103 0000 0034  tionWidget.....4
-00003c00: 0424 043e 0440 043c 0430 0442 0020 0431  .$.>.@.<.0.B. .1
-00003c10: 0430 0437 044b 0020 0434 0430 043d 043d  .0.7.K. .4.0.=.=
-00003c20: 044b 0445 0020 0443 0441 0442 0430 0440  .K.E. .C.A.B.0.@
-00003c30: 0435 043b 0800 0000 0006 0000 001b 4461  .5.;..........Da
-00003c40: 7461 6261 7365 2066 6f72 6d61 7420 6973  tabase format is
-00003c50: 206f 7574 6461 7465 6407 0000 0002 4442   outdated.....DB
-00003c60: 0103 0000 0064 0412 044b 0020 0441 043e  .....d...K. .A.>
-00003c70: 0433 043b 0430 0441 043d 044b 0020 0441  .3.;.0.A.=.K. .A
-00003c80: 043a 043e 043d 0432 0435 0440 0442 0438  .:.>.=.2.5.@.B.8
-00003c90: 0440 043e 0432 0430 0442 044c 0020 0434  .@.>.2.0.B.L. .4
-00003ca0: 0430 043d 043d 044b 0435 0020 0432 0020  .0.=.=.K.5. .2. 
-00003cb0: 043d 043e 0432 044b 0439 0020 0444 043e  .=.>.2.K.9. .D.>
-00003cc0: 0440 043c 0430 0442 003f 0800 0000 0006  .@.<.0.B.?......
-00003cd0: 0000 0032 446f 2079 6f75 2061 6772 6565  ...2Do you agree
-00003ce0: 2074 6f20 7570 6772 6164 6520 796f 7572   to upgrade your
-00003cf0: 2064 6174 6120 746f 206e 6577 6572 2066   data to newer f
-00003d00: 6f72 6d61 743f 0700 0000 0244 4201 0300  ormat?.....DB...
-00003d10: 0000 5e04 2404 3e04 4004 3c04 3000 2000  ..^.$.>.@.<.0. .
-00003d20: 3300 2d04 1d04 1404 2404 1b00 2004 3404  3.-.....$... .4.
-00003d30: 3b04 4f00 2004 4d04 4204 3e04 3304 3e00  ;.O. .M.B.>.3.>.
-00003d40: 2004 3304 3e04 3404 3000 2004 3d04 3500   .3.>.4.0. .=.5.
-00003d50: 2004 3f04 3e04 3404 3404 3504 4004 3604   .?.>.4.4.5.@.6.
-00003d60: 3804 3204 3004 3504 4204 4104 4f00 3a00  8.2.0.5.B.A.O.:.
-00003d70: 2008 0000 0000 0600 0000 2633 2d4e 4446   .........&3-NDF
-00003d80: 4c20 666f 726d 2069 736e 2774 2073 7570  L form isn't sup
-00003d90: 6f6f 7274 6564 2066 6f72 2079 6561 723a  oorted for year:
-00003da0: 2007 0000 0004 444c 5347 0103 0000 0086   .....DLSG......
-00003db0: 0421 0442 0440 0430 043d 0430 0020 0426  .!.B.@.0.=.0. .&
-00003dc0: 0411 0020 043d 0435 0020 0437 0430 0434  ... .=.5. .7.0.4
-00003dd0: 0430 043d 0430 002c 0020 0434 0438 0432  .0.=.0.,. .4.8.2
-00003de0: 0438 0434 0435 043d 0434 0020 043d 0435  .8.4.5.=.4. .=.5
-00003df0: 0020 0431 0443 0434 0435 0442 0020 0432  . .1.C.4.5.B. .2
-00003e00: 043a 043b 044e 0447 0451 043d 0020 0432  .:.;.N.G.Q.=. .2
-00003e10: 0020 0434 0435 043a 043b 0430 0440 0430  . .4.5.:.;.0.@.0
-00003e20: 0446 0438 044e 0020 0033 002d 041d 0424  .F.8.N. .3.-...$
-00003e30: 0414 041b 0020 0800 0000 0006 0000 0047  ..... .........G
-00003e40: 4163 636f 756e 7420 636f 756e 7472 7920  Account country 
-00003e50: 6973 206e 6f74 2073 6574 2066 6f72 2061  is not set for a
-00003e60: 7373 6574 2c20 6469 7669 6465 6e64 2069  sset, dividend i
-00003e70: 736e 2774 2069 6e63 6c75 6465 2069 6e20  sn't include in 
-00003e80: 332d 4e44 464c 2007 0000 0004 444c 5347  3-NDFL .....DLSG
-00003e90: 0103 0000 004a 0412 0430 043b 044e 0442  .....J...0.;.N.B
-00003ea0: 0430 0020 043d 0435 0020 043f 043e 0434  .0. .=.5. .?.>.4
-00003eb0: 0434 0435 0440 0436 0438 0432 0430 0435  .4.5.@.6.8.2.0.5
-00003ec0: 0442 0441 044f 0020 0434 043b 044f 0020  .B.A.O. .4.;.O. 
-00003ed0: 0033 002d 041d 0414 0424 041b 003a 0020  .3.-.....$...:. 
-00003ee0: 0800 0000 0006 0000 0026 4375 7272 656e  .........&Curren
-00003ef0: 6379 2069 7320 6e6f 7420 7375 7070 6f72  cy is not suppor
-00003f00: 7465 6420 666f 7220 332d 4e44 464c 3a20  ted for 3-NDFL: 
-00003f10: 0700 0000 0444 4c53 4701 0300 0000 1404  .....DLSG.......
-00003f20: 4d04 3a04 4104 3f04 3804 4004 3004 4604  M.:.A.?.8.@.0.F.
-00003f30: 3804 4f08 0000 0000 0600 0000 0665 7870  8.O..........exp
-00003f40: 6972 7907 0000 000c 4461 7461 4465 6c65  iry.....DataDele
-00003f50: 6761 7465 0103 0000 000e 043d 043e 043c  gate.......=.>.<
-00003f60: 0438 043d 0430 043b 0800 0000 0006 0000  .8.=.0.;........
-00003f70: 0009 7072 696e 6369 7061 6c07 0000 000c  ..principal.....
+00002fb0: 0000 0c04 1f04 3804 2300 2c00 2000 2508  ......8.#.,. .%.
+00002fc0: 0000 0000 0600 0000 0650 2f4c 2c20 2507  .........P/L, %.
+00002fd0: 0000 0011 436c 6f73 6564 5472 6164 6573  ....ClosedTrades
+00002fe0: 4d6f 6465 6c01 0300 0000 0c04 1a04 3e04  Model.........>.
+00002ff0: 3b00 2d04 3204 3e08 0000 0000 0600 0000  ;.-.2.>.........
+00003000: 0351 7479 0700 0000 1143 6c6f 7365 6454  .Qty.....ClosedT
+00003010: 7261 6465 734d 6f64 656c 0103 0000 00a0  radesModel......
+00003020: 041a 043e 043b 0438 0447 0435 0442 0432  ...>.;.8.G.5.B.2
+00003030: 043e 0020 0446 0435 043d 043d 044b 0445  .>. .F.5.=.=.K.E
+00003040: 0020 0431 0443 043c 0430 0433 0020 043d  . .1.C.<.0.3. .=
+00003050: 0435 0434 043e 0441 0442 0430 0442 043e  .5.4.>.A.B.0.B.>
+00003060: 0447 043d 043e 0020 0434 043b 044f 0020  .G.=.>. .4.;.O. 
+00003070: 043e 0431 0440 0430 0431 043e 0442 043a  .>.1.@.0.1.>.B.:
+00003080: 0438 0020 043a 043e 0440 043f 043e 0440  .8. .:.>.@.?.>.@
+00003090: 0430 0442 0438 0432 043d 043e 0433 043e  .0.B.8.2.=.>.3.>
+000030a0: 0020 0441 043e 0431 044b 0442 0438 044f  . .A.>.1.K.B.8.O
+000030b0: 002e 0020 0414 0430 0442 0430 003a 0020  ... ...0.B.0.:. 
+000030c0: 0800 0000 0006 0000 0042 4173 7365 7420  .........BAsset 
+000030d0: 616d 6f75 6e74 2069 7320 6e6f 7420 656e  amount is not en
+000030e0: 6f75 6768 2066 6f72 2063 6f72 706f 7261  ough for corpora
+000030f0: 7465 2061 6374 696f 6e20 7072 6f63 6573  te action proces
+00003100: 7369 6e67 2e20 4461 7465 3a20 0700 0000  sing. Date: ....
+00003110: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+00003120: 0103 0000 0074 0426 0411 0020 043d 0435  .....t.&... .=.5
+00003130: 0020 044f 0432 043b 044f 0435 0442 0441  . .O.2.;.O.5.B.A
+00003140: 044f 0020 0447 0430 0441 0442 044c 044e  .O. .G.0.A.B.L.N
+00003150: 0020 0440 0435 0437 0443 043b 044c 0442  . .@.5.7.C.;.L.B
+00003160: 0430 0442 043e 0432 0020 043a 043e 0440  .0.B.>.2. .:.>.@
+00003170: 043f 043e 0440 0430 0442 0438 0432 043d  .?.>.@.0.B.8.2.=
+00003180: 043e 0433 043e 0020 0441 043e 0431 044b  .>.3.>. .A.>.1.K
+00003190: 0442 0438 044f 003a 0020 0800 0000 0006  .B.8.O.:. ......
+000031a0: 0000 0030 4173 7365 7420 6973 6e27 7420  ...0Asset isn't 
+000031b0: 6120 7061 7274 206f 6620 636f 7270 6f72  a part of corpor
+000031c0: 6174 6520 6163 7469 6f6e 2072 6573 756c  ate action resul
+000031d0: 7473 3a20 0700 0000 0f43 6f72 706f 7261  ts: .....Corpora
+000031e0: 7465 4163 7469 6f6e 0103 0000 0056 041d  teAction.....V..
+000031f0: 0435 0020 0437 0430 0434 0430 043d 0020  .5. .7.0.4.0.=. 
+00003200: 0442 0438 043f 0020 043a 043e 0440 043f  .B.8.?. .:.>.@.?
+00003210: 043e 0440 0430 0442 0438 0432 043d 043e  .>.@.0.B.8.2.=.>
+00003220: 0433 043e 0020 0441 043e 0431 044b 0442  .3.>. .A.>.1.K.B
+00003230: 0438 044f 002e 0020 0414 0430 0442 0430  .8.O... ...0.B.0
+00003240: 003a 0020 0800 0000 0006 0000 002b 436f  .:. .........+Co
+00003250: 7270 6f72 6174 6520 6163 7469 6f6e 2074  rporate action t
+00003260: 7970 6520 6973 6e27 7420 6465 6669 6e65  ype isn't define
+00003270: 642e 2044 6174 653a 2007 0000 000f 436f  d. Date: .....Co
+00003280: 7270 6f72 6174 6541 6374 696f 6e01 0300  rporateAction...
+00003290: 0000 1204 1404 3504 3b04 3804 4104 4204  ......5.;.8.A.B.
+000032a0: 3804 3d04 3308 0000 0000 0600 0000 0944  8.=.3..........D
+000032b0: 656c 6973 7469 6e67 0700 0000 0f43 6f72  elisting.....Cor
+000032c0: 706f 7261 7465 4163 7469 6f6e 0103 0000  porateAction....
+000032d0: 002c 0420 0435 043e 0440 0433 0430 043d  .,. .5.>.@.3.0.=
+000032e0: 0438 0437 0430 0446 0438 044f 0020 043a  .8.7.0.F.8.O. .:
+000032f0: 043e 043c 043f 0430 043d 0438 0438 0800  .>.<.?.0.=.8.8..
+00003300: 0000 0006 0000 0006 4d65 7267 6572 0700  ........Merger..
+00003310: 0000 0f43 6f72 706f 7261 7465 4163 7469  ...CorporateActi
+00003320: 6f6e 0103 0000 00ac 0420 0435 0437 0443  on....... .5.7.C
+00003330: 043b 044c 0442 0430 0442 044b 0020 043a  .;.L.B.0.B.K. .:
+00003340: 043e 0440 043f 043e 0440 0430 0442 0438  .>.@.?.>.@.0.B.8
+00003350: 0432 043d 043e 0433 043e 0020 0441 043e  .2.=.>.3.>. .A.>
+00003360: 0431 044b 0442 0438 044f 0020 043d 0435  .1.K.B.8.O. .=.5
+00003370: 0020 0440 0430 0441 043f 0440 0435 0434  . .@.0.A.?.@.5.4
+00003380: 0435 043b 044f 044e 0442 0020 0031 0030  .5.;.O.N.B. .1.0
+00003390: 0030 0025 0020 0441 0442 043e 0438 043c  .0.%. .A.B.>.8.<
+000033a0: 043e 0441 0442 0438 0020 0438 0437 043d  .>.A.B.8. .8.7.=
+000033b0: 0430 0447 0430 043b 044c 043d 043e 0433  .0.G.0.;.L.=.>.3
+000033c0: 043e 0020 0430 043a 0442 0438 0432 0430  .>. .0.:.B.8.2.0
+000033d0: 002e 0020 0800 0000 0006 0000 004d 5265  ... .........MRe
+000033e0: 7375 6c74 7320 7661 6c75 6520 6f66 2063  sults value of c
+000033f0: 6f72 706f 7261 7465 2061 6374 696f 6e20  orporate action 
+00003400: 646f 6573 6e27 7420 6d61 7463 6820 3130  doesn't match 10
+00003410: 3025 206f 6620 696e 6974 6961 6c20 6173  0% of initial as
+00003420: 7365 7420 7661 6c75 652e 2007 0000 000f  set value. .....
+00003430: 436f 7270 6f72 6174 6541 6374 696f 6e01  CorporateAction.
+00003440: 0300 0000 3a04 1204 4b04 3404 3504 3b04  ....:...K.4.5.;.
+00003450: 3504 3d04 3804 3500 2004 3a04 3e04 3c04  5.=.8.5. .:.>.<.
+00003460: 3f04 3004 3d04 3804 3800 2000 2804 4104  ?.0.=.8.8. .(.A.
+00003470: 3f04 3804 3d00 2d04 3e04 4404 4400 2908  ?.8.=.-.>.D.D.).
+00003480: 0000 0000 0600 0000 0853 7069 6e2d 6f66  .........Spin-of
+00003490: 6607 0000 000f 436f 7270 6f72 6174 6541  f.....CorporateA
+000034a0: 6374 696f 6e01 0300 0000 0a04 2104 3f04  ction.......!.?.
+000034b0: 3b04 3804 4208 0000 0000 0600 0000 0553  ;.8.B..........S
+000034c0: 706c 6974 0700 0000 0f43 6f72 706f 7261  plit.....Corpora
+000034d0: 7465 4163 7469 6f6e 0103 0000 001a 0421  teAction.......!
+000034e0: 043c 0435 043d 0430 0020 0441 0438 043c  .<.5.=.0. .A.8.<
+000034f0: 0432 043e 043b 0430 0800 0000 0006 0000  .2.>.;.0........
+00003500: 000d 5379 6d62 6f6c 2063 6861 6e67 6507  ..Symbol change.
+00003510: 0000 000f 436f 7270 6f72 6174 6541 6374  ....CorporateAct
+00003520: 696f 6e01 0300 0000 1804 1d04 1504 1e04  ion.............
+00003530: 1f04 2004 1504 1404 1504 1b04 1504 1d04  .. .............
+00003540: 1e08 0000 0000 0600 0000 0955 4e44 4546  ...........UNDEF
+00003550: 494e 4544 0700 0000 0f43 6f72 706f 7261  INED.....Corpora
+00003560: 7465 4163 7469 6f6e 0103 0000 00ae 041d  teAction........
+00003570: 0435 043f 043e 0434 0435 0440 0436 0438  .5.?.>.4.5.@.6.8
+00003580: 0432 0430 0435 043c 044b 0439 0020 0441  .2.0.5.<.K.9. .A
+00003590: 043b 0443 0447 0430 0439 003a 0020 041a  .;.C.G.0.9.:. ..
+000035a0: 043e 0440 043f 043e 0440 0430 0442 0438  .>.@.?.>.@.0.B.8
+000035b0: 0432 043d 043e 0435 0020 0441 043e 0431  .2.=.>.5. .A.>.1
+000035c0: 044b 0442 0438 0435 0020 043f 043e 043a  .K.B.8.5. .?.>.:
+000035d0: 0440 044b 0432 0430 0435 0442 0020 043d  .@.K.2.0.5.B. .=
+000035e0: 0435 0020 0432 0441 044e 0020 043e 0442  .5. .2.A.N. .>.B
+000035f0: 043a 0440 044b 0442 0443 044e 0020 043f  .:.@.K.B.C.N. .?
+00003600: 043e 0437 0438 0446 0438 044e 002e 0020  .>.7.8.F.8.N... 
+00003610: 0414 0430 0442 0430 003a 0020 0800 0000  ...0.B.0.:. ....
+00003620: 0006 0000 0046 556e 6861 6e64 6c65 6420  .....FUnhandled 
+00003630: 6361 7365 3a20 436f 7270 6f72 6174 6520  case: Corporate 
+00003640: 6163 7469 6f6e 2063 6f76 6572 7320 6e6f  action covers no
+00003650: 7420 6675 6c6c 206f 7065 6e20 706f 7369  t full open posi
+00003660: 7469 6f6e 2e20 4461 7465 3a20 0700 0000  tion. Date: ....
+00003670: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+00003680: 0103 0000 0002 2116 0800 0000 0006 0000  ......!.........
+00003690: 0001 2307 0000 0015 436f 7270 6f72 6174  ..#.....Corporat
+000036a0: 6541 6374 696f 6e57 6964 6765 7401 0300  eActionWidget...
+000036b0: 0000 0804 2104 4704 3504 4208 0000 0000  ....!.G.5.B.....
+000036c0: 0600 0000 0741 6363 6f75 6e74 0700 0000  .....Account....
+000036d0: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+000036e0: 5769 6467 6574 0103 0000 001c 0414 043e  Widget.........>
+000036f0: 0431 0430 0432 0438 0442 044c 0020 0430  .1.0.2.8.B.L. .0
+00003700: 043a 0442 0438 0432 0800 0000 0006 0000  .:.B.8.2........
+00003710: 0009 4164 6420 6173 7365 7407 0000 0015  ..Add asset.....
+00003720: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
+00003730: 6964 6765 7401 0300 0000 0404 2604 1108  idget.......&...
+00003740: 0000 0000 0600 0000 0541 7373 6574 0700  .........Asset..
+00003750: 0000 1543 6f72 706f 7261 7465 4163 7469  ...CorporateActi
+00003760: 6f6e 5769 6467 6574 0103 0000 002c 041a  onWidget.....,..
+00003770: 043e 0440 043f 043e 0440 0430 0442 0438  .>.@.?.>.@.0.B.8
+00003780: 0432 043d 043e 0435 0020 0434 0435 0439  .2.=.>.5. .4.5.9
+00003790: 0441 0442 0432 0438 0435 0800 0000 0006  .A.B.2.8.5......
+000037a0: 0000 0010 436f 7270 6f72 6174 6520 4163  ....Corporate Ac
+000037b0: 7469 6f6e 0700 0000 1543 6f72 706f 7261  tion.....Corpora
+000037c0: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
+000037d0: 0000 0014 0414 0430 0442 0430 002f 0412  .......0.B.0./..
+000037e0: 0440 0435 043c 044f 0800 0000 0006 0000  .@.5.<.O........
+000037f0: 0009 4461 7465 2f54 696d 6507 0000 0015  ..Date/Time.....
+00003800: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
+00003810: 6964 6765 7401 0300 0000 1204 1404 3504  idget.........5.
+00003820: 3b04 3804 4104 4204 3804 3d04 3308 0000  ;.8.A.B.8.=.3...
+00003830: 0000 0600 0000 0944 656c 6973 7469 6e67  .......Delisting
+00003840: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
+00003850: 7469 6f6e 5769 6467 6574 0103 0000 0044  tionWidget.....D
+00003860: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+00003870: 043d 043e 0020 0434 043e 0431 0430 0432  .=.>. .4.>.1.0.2
+00003880: 0438 0442 044c 0020 043d 043e 0432 0443  .8.B.L. .=.>.2.C
+00003890: 044e 0020 0437 0430 043f 0438 0441 044c  .N. .7.0.?.8.A.L
+000038a0: 003a 0020 0800 0000 0006 0000 001a 4661  .:. ..........Fa
+000038b0: 696c 6564 2074 6f20 6164 6420 6e65 7720  iled to add new 
+000038c0: 7265 636f 7264 3a20 0700 0000 1543 6f72  record: .....Cor
+000038d0: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
+000038e0: 6574 0103 0000 0028 041e 0431 044a 0435  et.....(...1.J.5
+000038f0: 0434 0438 043d 0435 043d 0438 0435 0020  .4.8.=.5.=.8.5. 
+00003900: 043a 043e 043c 043f 0430 043d 0438 0438  .:.>.<.?.0.=.8.8
+00003910: 0800 0000 0006 0000 0006 4d65 7267 6572  ..........Merger
+00003920: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
+00003930: 7469 6f6e 5769 6467 6574 0103 0000 0006  tionWidget......
+00003940: 004e 002f 0041 0800 0000 0006 0000 0003  .N./.A..........
+00003950: 4e2f 4107 0000 0015 436f 7270 6f72 6174  N/A.....Corporat
+00003960: 6541 6374 696f 6e57 6964 6765 7401 0300  eActionWidget...
+00003970: 0000 1004 1e04 3f04 3804 4104 3004 3d04  ......?.8.A.0.=.
+00003980: 3804 3508 0000 0000 0600 0000 044e 6f74  8.5..........Not
+00003990: 6507 0000 0015 436f 7270 6f72 6174 6541  e.....CorporateA
+000039a0: 6374 696f 6e57 6964 6765 7401 0300 0000  ctionWidget.....
+000039b0: 4804 1e04 4804 3804 3104 3a04 3000 2004  H...H.8.1.:.0. .
+000039c0: 3f04 4004 3800 2004 3704 3004 3f04 3804  ?.@.8. .7.0.?.8.
+000039d0: 4104 3800 2004 3404 3504 4204 3004 3b04  A.8. .4.5.B.0.;.
+000039e0: 3504 3900 2004 3e04 3f04 3504 4004 3004  5.9. .>.?.5.@.0.
+000039f0: 4604 3804 3800 3a00 2008 0000 0000 0600  F.8.8.:. .......
+00003a00: 0000 214f 7065 7261 7469 6f6e 2064 6574  ..!Operation det
+00003a10: 6169 6c73 2073 7562 6d69 7420 6661 696c  ails submit fail
+00003a20: 6564 3a20 0700 0000 1543 6f72 706f 7261  ed: .....Corpora
+00003a30: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
+00003a40: 0000 0038 041e 0448 0438 0431 043a 0430  ...8...H.8.1.:.0
+00003a50: 0020 043f 0440 0438 0020 0437 0430 043f  . .?.@.8. .7.0.?
+00003a60: 0438 0441 0438 0020 043e 043f 0435 0440  .8.A.8. .>.?.5.@
+00003a70: 0430 0446 0438 0438 003a 0020 0800 0000  .0.F.8.8.:. ....
+00003a80: 0006 0000 0019 4f70 6572 6174 696f 6e20  ......Operation 
+00003a90: 7375 626d 6974 2066 6169 6c65 643a 2007  submit failed: .
+00003aa0: 0000 0015 436f 7270 6f72 6174 6541 6374  ....CorporateAct
+00003ab0: 696f 6e57 6964 6765 7401 0300 0000 0c04  ionWidget.......
+00003ac0: 1a04 3e04 3b00 2d04 3204 3e08 0000 0000  ..>.;.-.2.>.....
+00003ad0: 0600 0000 0351 7479 0700 0000 1543 6f72  .....Qty.....Cor
+00003ae0: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
+00003af0: 6574 0103 0000 001a 0423 0434 0430 043b  et.......#.4.0.;
+00003b00: 0438 0442 044c 0020 0430 043a 0442 0438  .8.B.L. .0.:.B.8
+00003b10: 0432 0800 0000 0006 0000 000c 5265 6d6f  .2..........Remo
+00003b20: 7665 2061 7373 6574 0700 0000 1543 6f72  ve asset.....Cor
+00003b30: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
+00003b40: 6574 0103 ffff ffff 0800 0000 0006 0000  et..............
+00003b50: 0008 5370 696e 2d4f 6666 0700 0000 1543  ..Spin-Off.....C
+00003b60: 6f72 706f 7261 7465 4163 7469 6f6e 5769  orporateActionWi
+00003b70: 6467 6574 0103 0000 000a 0421 043f 043b  dget.......!.?.;
+00003b80: 0438 0442 0800 0000 0006 0000 0005 5370  .8.B..........Sp
+00003b90: 6c69 7407 0000 0015 436f 7270 6f72 6174  lit.....Corporat
+00003ba0: 6541 6374 696f 6e57 6964 6765 7401 0300  eActionWidget...
+00003bb0: 0000 1a04 2104 3c04 3504 3d04 3000 2004  ....!.<.5.=.0. .
+00003bc0: 4104 3804 3c04 3204 3e04 3b04 3008 0000  A.8.<.2.>.;.0...
+00003bd0: 0000 0600 0000 0d53 796d 626f 6c20 6368  .......Symbol ch
+00003be0: 616e 6765 0700 0000 1543 6f72 706f 7261  ange.....Corpora
+00003bf0: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
+00003c00: 0000 0006 0422 0438 043f 0800 0000 0006  .....".8.?......
+00003c10: 0000 0004 5479 7065 0700 0000 1543 6f72  ....Type.....Cor
+00003c20: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
+00003c30: 6574 0103 0000 0034 0424 043e 0440 043c  et.....4.$.>.@.<
+00003c40: 0430 0442 0020 0431 0430 0437 044b 0020  .0.B. .1.0.7.K. 
+00003c50: 0434 0430 043d 043d 044b 0445 0020 0443  .4.0.=.=.K.E. .C
+00003c60: 0441 0442 0430 0440 0435 043b 0800 0000  .A.B.0.@.5.;....
+00003c70: 0006 0000 001b 4461 7461 6261 7365 2066  ......Database f
+00003c80: 6f72 6d61 7420 6973 206f 7574 6461 7465  ormat is outdate
+00003c90: 6407 0000 0002 4442 0103 0000 0064 0412  d.....DB.....d..
+00003ca0: 044b 0020 0441 043e 0433 043b 0430 0441  .K. .A.>.3.;.0.A
+00003cb0: 043d 044b 0020 0441 043a 043e 043d 0432  .=.K. .A.:.>.=.2
+00003cc0: 0435 0440 0442 0438 0440 043e 0432 0430  .5.@.B.8.@.>.2.0
+00003cd0: 0442 044c 0020 0434 0430 043d 043d 044b  .B.L. .4.0.=.=.K
+00003ce0: 0435 0020 0432 0020 043d 043e 0432 044b  .5. .2. .=.>.2.K
+00003cf0: 0439 0020 0444 043e 0440 043c 0430 0442  .9. .D.>.@.<.0.B
+00003d00: 003f 0800 0000 0006 0000 0032 446f 2079  .?.........2Do y
+00003d10: 6f75 2061 6772 6565 2074 6f20 7570 6772  ou agree to upgr
+00003d20: 6164 6520 796f 7572 2064 6174 6120 746f  ade your data to
+00003d30: 206e 6577 6572 2066 6f72 6d61 743f 0700   newer format?..
+00003d40: 0000 0244 4201 0300 0000 5e04 2404 3e04  ...DB.....^.$.>.
+00003d50: 4004 3c04 3000 2000 3300 2d04 1d04 1404  @.<.0. .3.-.....
+00003d60: 2404 1b00 2004 3404 3b04 4f00 2004 4d04  $... .4.;.O. .M.
+00003d70: 4204 3e04 3304 3e00 2004 3304 3e04 3404  B.>.3.>. .3.>.4.
+00003d80: 3000 2004 3d04 3500 2004 3f04 3e04 3404  0. .=.5. .?.>.4.
+00003d90: 3404 3504 4004 3604 3804 3204 3004 3504  4.5.@.6.8.2.0.5.
+00003da0: 4204 4104 4f00 3a00 2008 0000 0000 0600  B.A.O.:. .......
+00003db0: 0000 2633 2d4e 4446 4c20 666f 726d 2069  ..&3-NDFL form i
+00003dc0: 736e 2774 2073 7570 6f6f 7274 6564 2066  sn't supoorted f
+00003dd0: 6f72 2079 6561 723a 2007 0000 0004 444c  or year: .....DL
+00003de0: 5347 0103 0000 0086 0421 0442 0440 0430  SG.......!.B.@.0
+00003df0: 043d 0430 0020 0426 0411 0020 043d 0435  .=.0. .&... .=.5
+00003e00: 0020 0437 0430 0434 0430 043d 0430 002c  . .7.0.4.0.=.0.,
+00003e10: 0020 0434 0438 0432 0438 0434 0435 043d  . .4.8.2.8.4.5.=
+00003e20: 0434 0020 043d 0435 0020 0431 0443 0434  .4. .=.5. .1.C.4
+00003e30: 0435 0442 0020 0432 043a 043b 044e 0447  .5.B. .2.:.;.N.G
+00003e40: 0451 043d 0020 0432 0020 0434 0435 043a  .Q.=. .2. .4.5.:
+00003e50: 043b 0430 0440 0430 0446 0438 044e 0020  .;.0.@.0.F.8.N. 
+00003e60: 0033 002d 041d 0424 0414 041b 0020 0800  .3.-...$..... ..
+00003e70: 0000 0006 0000 0047 4163 636f 756e 7420  .......GAccount 
+00003e80: 636f 756e 7472 7920 6973 206e 6f74 2073  country is not s
+00003e90: 6574 2066 6f72 2061 7373 6574 2c20 6469  et for asset, di
+00003ea0: 7669 6465 6e64 2069 736e 2774 2069 6e63  vidend isn't inc
+00003eb0: 6c75 6465 2069 6e20 332d 4e44 464c 2007  lude in 3-NDFL .
+00003ec0: 0000 0004 444c 5347 0103 0000 004a 0412  ....DLSG.....J..
+00003ed0: 0430 043b 044e 0442 0430 0020 043d 0435  .0.;.N.B.0. .=.5
+00003ee0: 0020 043f 043e 0434 0434 0435 0440 0436  . .?.>.4.4.5.@.6
+00003ef0: 0438 0432 0430 0435 0442 0441 044f 0020  .8.2.0.5.B.A.O. 
+00003f00: 0434 043b 044f 0020 0033 002d 041d 0414  .4.;.O. .3.-....
+00003f10: 0424 041b 003a 0020 0800 0000 0006 0000  .$...:. ........
+00003f20: 0026 4375 7272 656e 6379 2069 7320 6e6f  .&Currency is no
+00003f30: 7420 7375 7070 6f72 7465 6420 666f 7220  t supported for 
+00003f40: 332d 4e44 464c 3a20 0700 0000 0444 4c53  3-NDFL: .....DLS
+00003f50: 4701 0300 0000 1404 4d04 3a04 4104 3f04  G.......M.:.A.?.
+00003f60: 3804 4004 3004 4604 3804 4f08 0000 0000  8.@.0.F.8.O.....
+00003f70: 0600 0000 0665 7870 6972 7907 0000 000c  .....expiry.....
 00003f80: 4461 7461 4465 6c65 6761 7465 0103 0000  DataDelegate....
-00003f90: 000e 0440 0435 0433 002e 043a 043e 0434  ...@.5.3...:.>.4
-00003fa0: 0800 0000 0006 0000 0008 7265 672e 636f  ..........reg.co
-00003fb0: 6465 0700 0000 0c44 6174 6144 656c 6567  de.....DataDeleg
-00003fc0: 6174 6501 0300 0000 1004 1204 4104 3500  ate.........A.5.
-00003fd0: 2004 3404 3004 4204 4b08 0000 0000 0600   .4.0.B.K.......
-00003fe0: 0000 0941 6c6c 2064 6174 6573 0700 0000  ...All dates....
-00003ff0: 1144 6174 6552 616e 6765 5365 6c65 6374  .DateRangeSelect
-00004000: 6f72 0103 0000 0004 0421 003a 0800 0000  or.......!.:....
-00004010: 0006 0000 0005 4672 6f6d 3a07 0000 0011  ......From:.....
-00004020: 4461 7465 5261 6e67 6553 656c 6563 746f  DateRangeSelecto
-00004030: 7201 0300 0000 0a04 1c04 3504 4104 4f04  r.........5.A.O.
-00004040: 4608 0000 0000 0600 0000 054d 6f6e 7468  F..........Month
-00004050: 0700 0000 1144 6174 6552 616e 6765 5365  .....DateRangeSe
-00004060: 6c65 6374 6f72 0103 0000 001c 041f 0440  lector.........@
-00004070: 0435 0434 044b 0434 0443 0449 0438 0439  .5.4.K.4.C.I.8.9
-00004080: 0020 0433 043e 0434 0800 0000 0006 0000  . .3.>.4........
-00004090: 000d 5072 6576 696f 7573 2079 6561 7207  ..Previous year.
-000040a0: 0000 0011 4461 7465 5261 6e67 6553 656c  ....DateRangeSel
-000040b0: 6563 746f 7201 0300 0000 0e04 1a04 3204  ector.........2.
-000040c0: 3004 4004 4204 3004 3b08 0000 0000 0600  0.@.B.0.;.......
-000040d0: 0000 0751 7561 7274 6572 0700 0000 1144  ...Quarter.....D
-000040e0: 6174 6552 616e 6765 5365 6c65 6374 6f72  ateRangeSelector
-000040f0: 0103 0000 0024 0422 0435 043a 0443 0449  .....$.".5.:.C.I
-00004100: 0438 0439 0020 0434 043e 0020 0441 0435  .8.9. .4.>. .A.5
-00004110: 0433 043e 0434 043d 044f 0800 0000 0006  .3.>.4.=.O......
-00004120: 0000 000f 5175 6172 7465 7220 746f 2064  ....Quarter to d
-00004130: 6174 6507 0000 0011 4461 7465 5261 6e67  ate.....DateRang
-00004140: 6553 656c 6563 746f 7201 0300 0000 1604  eSelector.......
-00004150: 2204 3504 3a04 4304 4904 3804 3900 2004  ".5.:.C.I.8.9. .
-00004160: 3304 3e04 3408 0000 0000 0600 0000 0954  3.>.4..........T
-00004170: 6869 7320 7965 6172 0700 0000 1144 6174  his year.....Dat
-00004180: 6552 616e 6765 5365 6c65 6374 6f72 0103  eRangeSelector..
-00004190: 0000 0006 0414 043e 003a 0800 0000 0006  .......>.:......
-000041a0: 0000 0003 546f 3a07 0000 0011 4461 7465  ....To:.....Date
-000041b0: 5261 6e67 6553 656c 6563 746f 7201 0300  RangeSelector...
-000041c0: 0000 0c04 1d04 3504 3404 3504 3b04 4f08  ......5.4.5.;.O.
-000041d0: 0000 0000 0600 0000 0457 6565 6b07 0000  .........Week...
-000041e0: 0011 4461 7465 5261 6e67 6553 656c 6563  ..DateRangeSelec
-000041f0: 746f 7201 0300 0000 0604 1304 3e04 3408  tor.........>.4.
-00004200: 0000 0000 0600 0000 0459 6561 7207 0000  .........Year...
-00004210: 0011 4461 7465 5261 6e67 6553 656c 6563  ..DateRangeSelec
-00004220: 746f 7201 0300 0000 1c04 1304 3e04 3400  tor.........>.4.
-00004230: 2004 3404 3e00 2004 4104 3504 3304 3e04   .4.>. .A.5.3.>.
-00004240: 3404 3d04 4f08 0000 0000 0600 0000 0c59  4.=.O..........Y
-00004250: 6561 7220 746f 2064 6174 6507 0000 0011  ear to date.....
-00004260: 4461 7465 5261 6e67 6553 656c 6563 746f  DateRangeSelecto
-00004270: 7201 0300 0000 1e04 2104 3404 3504 3b04  r.......!.4.5.;.
-00004280: 3a04 3800 2004 3f04 3e00 2004 4104 4704  :.8. .?.>. .A.G.
-00004290: 3504 4204 4308 0000 0000 0600 0000 1044  5.B.C..........D
-000042a0: 6561 6c73 2062 7920 4163 636f 756e 7407  eals by Account.
-000042b0: 0000 000b 4465 616c 7352 6570 6f72 7401  ....DealsReport.
-000042c0: 0300 0000 0a04 2104 4704 3504 4200 3a08  ......!.G.5.B.:.
-000042d0: 0000 0000 0600 0000 0841 6363 6f75 6e74  .........Account
-000042e0: 3a07 0000 0011 4465 616c 7352 6570 6f72  :.....DealsRepor
-000042f0: 7457 6964 6765 7401 0300 0000 0c04 2104  tWidget.......!.
-00004300: 3404 3504 3b04 3a04 3808 0000 0000 0600  4.5.;.:.8.......
-00004310: 0000 0544 6561 6c73 0700 0000 1144 6561  ...Deals.....Dea
-00004320: 6c73 5265 706f 7274 5769 6467 6574 0103  lsReportWidget..
-00004330: 0000 0020 0413 0440 0443 043f 043f 0438  ... ...@.C.?.?.8
-00004340: 0440 043e 0432 0430 0442 044c 0020 043f  .@.>.2.0.B.L. .?
-00004350: 043e 003a 0800 0000 0006 0000 0009 4772  .>.:..........Gr
-00004360: 6f75 7020 6279 3a07 0000 0011 4465 616c  oup by:.....Deal
-00004370: 7352 6570 6f72 7457 6964 6765 7401 0300  sReportWidget...
-00004380: 0000 0e00 3c04 1f04 4304 4104 4204 3e00  ....<...C.A.B.>.
-00004390: 3e08 0000 0000 0600 0000 063c 4e6f 6e65  >..........<None
-000043a0: 3e07 0000 0011 4465 616c 7352 6570 6f72  >.....DealsRepor
-000043b0: 7457 696e 646f 7701 0300 0000 1a04 2604  tWindow.......&.
-000043c0: 3504 3d04 3d04 3004 4f00 2004 3104 4304  5.=.=.0.O. .1.C.
-000043d0: 3c04 3004 3304 3008 0000 0000 0600 0000  <.0.3.0.........
-000043e0: 0541 7373 6574 0700 0000 1144 6561 6c73  .Asset.....Deals
-000043f0: 5265 706f 7274 5769 6e64 6f77 0103 0000  ReportWindow....
-00004400: 0030 0426 0411 0020 002d 0020 041e 0442  .0.&... .-. ...B
-00004410: 043a 0440 044b 0442 0438 0435 0020 002d  .:.@.K.B.8.5. .-
-00004420: 0020 0417 0430 043a 0440 044b 0442 0438  . ...0.:.@.K.B.8
-00004430: 0435 0800 0000 0006 0000 0014 4173 7365  .5..........Asse
-00004440: 7420 2d20 4f70 656e 202d 2043 6c6f 7365  t - Open - Close
-00004450: 0700 0000 1144 6561 6c73 5265 706f 7274  .....DealsReport
-00004460: 5769 6e64 6f77 0103 0000 0010 0417 0430  Window.........0
-00004470: 043a 0440 044b 0442 0438 0435 0800 0000  .:.@.K.B.8.5....
-00004480: 0006 0000 0005 436c 6f73 6507 0000 0011  ......Close.....
-00004490: 4465 616c 7352 6570 6f72 7457 696e 646f  DealsReportWindo
-000044a0: 7701 0300 0000 2604 1704 3004 3a04 4004  w.....&...0.:.@.
-000044b0: 4b04 4204 3804 3500 2000 2d00 2004 1e04  K.B.8.5. .-. ...
-000044c0: 4204 3a04 4004 4b04 4204 3804 3508 0000  B.:.@.K.B.8.5...
-000044d0: 0000 0600 0000 0c43 6c6f 7365 202d 204f  .......Close - O
-000044e0: 7065 6e07 0000 0011 4465 616c 7352 6570  pen.....DealsRep
-000044f0: 6f72 7457 696e 646f 7701 0300 0000 2604  ortWindow.....&.
-00004500: 1e04 4204 3a04 4004 4b04 4204 3804 3500  ..B.:.@.K.B.8.5.
-00004510: 2000 2d00 2004 1704 3004 3a04 4004 4b04   .-. ...0.:.@.K.
-00004520: 4204 3804 3508 0000 0000 0600 0000 0c4f  B.8.5..........O
-00004530: 7065 6e20 2d20 436c 6f73 6507 0000 0011  pen - Close.....
-00004540: 4465 616c 7352 6570 6f72 7457 696e 646f  DealsReportWindo
-00004550: 7701 0300 0000 0a04 2104 4304 3c04 3c04  w.......!.C.<.<.
-00004560: 3008 0000 0000 0600 0000 0641 6d6f 756e  0..........Amoun
-00004570: 7407 0000 000c 4465 7461 696c 734d 6f64  t.....DetailsMod
-00004580: 656c 0103 0000 0012 041a 0430 0442 0435  el.........0.B.5
-00004590: 0433 043e 0440 0438 044f 0800 0000 0006  .3.>.@.8.O......
-000045a0: 0000 0008 4361 7465 676f 7279 0700 0000  ....Category....
-000045b0: 0c44 6574 6169 6c73 4d6f 6465 6c01 0300  .DetailsModel...
-000045c0: 0000 1004 1e04 3f04 3804 4104 3004 3d04  ......?.8.A.0.=.
-000045d0: 3804 3508 0000 0000 0600 0000 044e 6f74  8.5..........Not
-000045e0: 6507 0000 000c 4465 7461 696c 734d 6f64  e.....DetailsMod
-000045f0: 656c 0103 0000 000a 041c 0435 0442 043a  el.........5.B.:
-00004600: 0430 0800 0000 0006 0000 0003 5461 6707  .0..........Tag.
-00004610: 0000 000c 4465 7461 696c 734d 6f64 656c  ....DetailsModel
-00004620: 0103 0000 009e 041d 0435 0432 043e 0437  .........5.2.>.7
-00004630: 043c 043e 0436 043d 043e 0020 043e 0431  .<.>.6.=.>. .>.1
-00004640: 0440 0430 0431 043e 0442 0430 0442 044c  .@.0.1.>.B.0.B.L
-00004650: 0020 0434 0438 0432 0438 0434 0435 043d  . .4.8.2.8.4.5.=
-00004660: 0434 002c 0020 0442 002e 043a 002e 0020  .4.,. .B...:... 
-00004670: 043d 0435 0020 0443 043a 0430 0437 0430  .=.5. .C.:.0.7.0
-00004680: 043d 0020 0431 0430 043d 043a 0020 0434  .=. .1.0.=.:. .4
-00004690: 043b 044f 0020 0438 043d 0432 0435 0441  .;.O. .8.=.2.5.A
-000046a0: 0442 0438 0446 0438 043e 043d 043d 043e  .B.8.F.8.>.=.=.>
-000046b0: 0433 043e 0020 0441 0447 0451 0442 0430  .3.>. .A.G.Q.B.0
-000046c0: 003a 0020 0800 0000 0006 0000 0041 4361  .:. .........ACa
-000046d0: 6e27 7420 7072 6f63 6573 7320 6469 7669  n't process divi
-000046e0: 6465 6e64 2061 7320 6261 6e6b 2069 736e  dend as bank isn
-000046f0: 2774 2073 6574 2066 6f72 2069 6e76 6573  't set for inves
-00004700: 746d 656e 7420 6163 636f 756e 743a 2007  tment account: .
-00004710: 0000 0008 4469 7669 6465 6e64 0103 0000  ....Dividend....
-00004720: 005a 041d 0435 0020 0437 0430 0434 0430  .Z...5. .7.0.4.0
-00004730: 043d 0430 0020 0446 0435 043d 0430 0020  .=.0. .F.5.=.0. 
-00004740: 0434 043b 044f 0020 0432 044b 043f 043b  .4.;.O. .2.K.?.;
-00004750: 0430 0442 044b 0020 0446 0435 043d 043d  .0.B.K. .F.5.=.=
-00004760: 044b 043c 0438 0020 0431 0443 043c 0430  .K.<.8. .1.C.<.0
-00004770: 0433 0430 043c 0438 003a 0020 0800 0000  .3.0.<.8.:. ....
-00004780: 0006 0000 002a 4e6f 2070 7269 6365 2064  .....*No price d
-00004790: 6174 6120 666f 7220 7374 6f63 6b20 6469  ata for stock di
-000047a0: 7669 6465 6e64 2f76 6573 7469 6e67 3a20  vidend/vesting: 
-000047b0: 0700 0000 0844 6976 6964 656e 6401 0300  .....Dividend...
-000047c0: 0000 7204 1d04 3504 4200 2004 3a04 3e04  ..r...5.B. .:.>.
-000047d0: 4204 3804 4004 3e04 3204 3a04 3800 2004  B.8.@.>.2.:.8. .
-000047e0: 3404 3b04 4f00 2004 3404 3804 3204 3804  4.;.O. .4.8.2.8.
-000047f0: 3404 3504 3d04 3404 3000 2004 3004 3a04  4.5.=.4.0. .0.:.
-00004800: 4604 3804 4f04 3c04 3800 2004 3804 3b04  F.8.O.<.8. .8.;.
-00004810: 3800 2004 3704 3004 4704 3804 4104 3b04  8. .7.0.G.8.A.;.
-00004820: 3504 3d04 3804 4f00 2004 3004 3a04 4604  5.=.8.O. .0.:.F.
-00004830: 3804 3900 2e08 0000 0000 0600 0000 2d4e  8.9...........-N
-00004840: 6f20 7374 6f63 6b20 7175 6f74 6520 666f  o stock quote fo
-00004850: 7220 7374 6f63 6b20 6469 7669 6465 6e64  r stock dividend
-00004860: 206f 7220 7665 7374 696e 672e 0700 0000   or vesting.....
-00004870: 0844 6976 6964 656e 6401 0300 0000 b804  .Dividend.......
-00004880: 1d04 3504 3f04 3e04 3404 3404 3504 4004  ..5.?.>.4.4.5.@.
-00004890: 3604 3804 3204 3004 3504 3c04 3e04 3500  6.8.2.0.5.<.>.5.
-000048a0: 2004 3404 3504 3904 4104 4204 3204 3804   .4.5.9.A.B.2.8.
-000048b0: 3500 3a00 2004 3404 3804 3204 3804 3404  5.:. .4.8.2.8.4.
-000048c0: 3504 3d04 3400 2004 3004 3a04 4604 3804  5.=.4. .0.:.F.8.
-000048d0: 4f04 3c04 3800 2004 3804 3b04 3800 2004  O.<.8. .8.;.8. .
-000048e0: 3704 3004 4704 3804 4104 3b04 3504 3d04  7.0.G.8.A.;.5.=.
-000048f0: 3804 3500 2004 3004 3a04 4604 3804 3900  8.5. .0.:.F.8.9.
-00004900: 2004 3704 3004 3a04 4004 4b04 3204 3004   .7.0.:.@.K.2.0.
-00004910: 3504 4200 2004 3a04 3e04 4004 3e04 4204  5.B. .:.>.@.>.B.
-00004920: 3a04 4304 4e00 2004 3f04 3e04 3704 3804  :.C.N. .?.>.7.8.
-00004930: 4604 3804 4e00 2e08 0000 0000 0600 0000  F.8.N...........
-00004940: 434e 6f74 2073 7570 706f 7274 6564 2061  CNot supported a
-00004950: 6374 696f 6e3a 2073 746f 636b 2064 6976  ction: stock div
-00004960: 6964 656e 6420 6f72 2076 6573 7469 6e67  idend or vesting
-00004970: 2063 6c6f 7365 7320 7368 6f72 7420 7472   closes short tr
-00004980: 6164 652e 0700 0000 0844 6976 6964 656e  ade......Dividen
-00004990: 6401 0300 0000 0e04 1d04 3004 3b04 3e04  d.........0.;.>.
-000049a0: 3300 3a00 2008 0000 0000 0600 0000 0554  3.:. ..........T
-000049b0: 6178 3a20 0700 0000 0844 6976 6964 656e  ax: .....Dividen
-000049c0: 6401 0300 0000 3e04 1d04 3504 3f04 3e04  d.....>...5.?.>.
-000049d0: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
-000049e0: 3504 3c04 4b04 3900 2004 4204 3804 3f00  5.<.K.9. .B.8.?.
-000049f0: 2004 3404 3804 3204 3804 3404 3504 3d04   .4.8.2.8.4.5.=.
-00004a00: 3404 3000 2e08 0000 0000 0600 0000 1a55  4.0............U
-00004a10: 6e73 7570 706f 7274 6564 2064 6976 6964  nsupported divid
-00004a20: 656e 6420 7479 7065 2e07 0000 0008 4469  end type......Di
-00004a30: 7669 6465 6e64 0103 0000 0002 2116 0800  vidend......!...
-00004a40: 0000 0006 0000 0001 2307 0000 000e 4469  ........#.....Di
-00004a50: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
-00004a60: 0008 0421 0447 0435 0442 0800 0000 0006  ...!.G.5.B......
-00004a70: 0000 0007 4163 636f 756e 7407 0000 000e  ....Account.....
-00004a80: 4469 7669 6465 6e64 5769 6467 6574 0103  DividendWidget..
-00004a90: 0000 0004 0426 0411 0800 0000 0006 0000  .....&..........
-00004aa0: 0005 4173 7365 7407 0000 000e 4469 7669  ..Asset.....Divi
-00004ab0: 6465 6e64 5769 6467 6574 0103 0000 000a  dendWidget......
-00004ac0: 041a 0443 043f 043e 043d 0800 0000 0006  ...C.?.>.=......
-00004ad0: 0000 000d 426f 6e64 2049 6e74 6572 6573  ....Bond Interes
-00004ae0: 7407 0000 000e 4469 7669 6465 6e64 5769  t.....DividendWi
-00004af0: 6467 6574 0103 0000 0014 0414 0430 0442  dget.........0.B
-00004b00: 0430 002f 0412 0440 0435 043c 044f 0800  .0./...@.5.<.O..
-00004b10: 0000 0006 0000 0009 4461 7465 2f54 696d  ........Date/Tim
-00004b20: 6507 0000 000e 4469 7669 6465 6e64 5769  e.....DividendWi
-00004b30: 6467 6574 0103 0000 0010 0414 0438 0432  dget.........8.2
-00004b40: 0438 0434 0435 043d 0434 0800 0000 0006  .8.4.5.=.4......
-00004b50: 0000 0008 4469 7669 6465 6e64 0700 0000  ....Dividend....
-00004b60: 0e44 6976 6964 656e 6457 6964 6765 7401  .DividendWidget.
-00004b70: 0300 0000 0e04 1e04 4204 4104 3504 4704  ........B.A.5.G.
-00004b80: 3a04 3008 0000 0000 0600 0000 0745 782d  :.0..........Ex-
-00004b90: 4461 7465 0700 0000 0e44 6976 6964 656e  Date.....Dividen
-00004ba0: 6457 6964 6765 7401 0300 0000 0600 4e00  dWidget.......N.
-00004bb0: 2f00 4108 0000 0000 0600 0000 034e 2f41  /.A..........N/A
-00004bc0: 0700 0000 0e44 6976 6964 656e 6457 6964  .....DividendWid
-00004bd0: 6765 7401 0300 0000 1a04 1d04 3504 4200  get.........5.B.
-00004be0: 2004 3a04 3e04 4204 3804 4004 3e04 3204   .:.>.B.8.@.>.2.
-00004bf0: 3a04 3808 0000 0000 0600 0000 084e 6f20  :.8..........No 
-00004c00: 7175 6f74 6507 0000 000e 4469 7669 6465  quote.....Divide
-00004c10: 6e64 5769 6467 6574 0103 0000 0010 041e  ndWidget........
-00004c20: 043f 0438 0441 0430 043d 0438 0435 0800  .?.8.A.0.=.8.5..
-00004c30: 0000 0006 0000 0004 4e6f 7465 0700 0000  ........Note....
-00004c40: 0e44 6976 6964 656e 6457 6964 6765 7401  .DividendWidget.
-00004c50: 0300 0000 0804 2604 3504 3d04 3008 0000  ......&.5.=.0...
-00004c60: 0000 0600 0000 0550 7269 6365 0700 0000  .......Price....
-00004c70: 0e44 6976 6964 656e 6457 6964 6765 7401  .DividendWidget.
-00004c80: 0300 0000 2004 1404 3804 3204 3804 3404  .... ...8.2.8.4.
-00004c90: 3504 3d04 3400 2004 3004 3a04 4604 3804  5.=.4. .0.:.F.8.
-00004ca0: 4f04 3c04 3808 0000 0000 0600 0000 0e53  O.<.8..........S
-00004cb0: 746f 636b 2044 6976 6964 656e 6407 0000  tock Dividend...
-00004cc0: 000e 4469 7669 6465 6e64 5769 6467 6574  ..DividendWidget
-00004cd0: 0103 0000 001c 041f 0435 0440 0435 0434  .........5.@.5.4
-00004ce0: 0430 0447 0430 0020 0430 043a 0446 0438  .0.G.0. .0.:.F.8
-00004cf0: 0439 0800 0000 0006 0000 000d 5374 6f63  .9..........Stoc
-00004d00: 6b20 5665 7374 696e 6707 0000 000e 4469  k Vesting.....Di
-00004d10: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
-00004d20: 000a 041d 0430 043b 043e 0433 0800 0000  .....0.;.>.3....
-00004d30: 0006 0000 0003 5461 7807 0000 000e 4469  ......Tax.....Di
-00004d40: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
-00004d50: 0006 0422 0438 043f 0800 0000 0006 0000  ...".8.?........
-00004d60: 0004 5479 7065 0700 0000 0e44 6976 6964  ..Type.....Divid
-00004d70: 656e 6457 6964 6765 7401 0300 0000 b204  endWidget.......
-00004d80: 1d04 4304 3604 3d04 3e00 2004 4304 4104  ..C.6.=.>. .C.A.
-00004d90: 4204 3004 3d04 3e04 3204 3804 4204 4c00  B.0.=.>.2.8.B.L.
-00004da0: 2004 3a04 3e04 4204 3804 4004 3e04 3204   .:.>.B.8.@.>.2.
-00004db0: 3a04 4300 2004 3104 4304 3c04 3004 3304  :.C. .1.C.<.0.3.
-00004dc0: 3800 2004 3404 3b04 4f00 2004 1404 3004  8. .4.;.O. ...0.
-00004dd0: 4204 4b00 2f04 1204 4004 3504 3c04 3504  B.K./...@.5.<.5.
-00004de0: 3d04 3800 2004 3404 3804 3204 3804 3404  =.8. .4.8.2.8.4.
-00004df0: 3504 3d04 3404 3000 2004 4704 3504 4004  5.=.4.0. .G.5.@.
-00004e00: 3504 3700 2004 3c04 3504 3d04 4e00 2004  5.7. .<.5.=.N. .
-00004e10: 1404 3004 3d04 3d04 4b04 3500 2d00 3e04  ..0.=.=.K.5.-.>.
-00004e20: 1a04 3e04 4204 3804 4004 3e04 3204 3a04  ..>.B.8.@.>.2.:.
-00004e30: 3808 0000 0000 0600 0000 4859 6f75 2073  8.........HYou s
-00004e40: 686f 756c 6420 7365 7420 7175 6f74 6520  hould set quote 
-00004e50: 7669 6120 4461 7461 2d3e 5175 6f74 6573  via Data->Quotes
-00004e60: 206d 656e 7520 666f 7220 4461 7465 2f54   menu for Date/T
-00004e70: 696d 6520 6f66 2074 6865 2064 6976 6964  ime of the divid
-00004e80: 656e 6407 0000 000e 4469 7669 6465 6e64  end.....Dividend
-00004e90: 5769 6467 6574 0103 0000 0014 043d 0435  Widget.......=.5
-00004ea0: 0438 0437 0432 0435 0441 0442 043d 043e  .8.7.2.5.A.B.=.>
-00004eb0: 0800 0000 0006 0000 0007 756e 6b6e 6f77  ..........unknow
-00004ec0: 6e07 0000 000e 4469 7669 6465 6e64 5769  n.....DividendWi
-00004ed0: 6467 6574 0103 0000 0010 0421 0432 043e  dget.......!.2.>
-00004ee0: 0439 0441 0442 0432 043e 0800 0000 0006  .9.A.B.2.>......
-00004ef0: 0000 0008 5072 6f70 6572 7479 0700 0000  ....Property....
-00004f00: 0e45 7874 7261 4461 7461 4d6f 6465 6c01  .ExtraDataModel.
-00004f10: 0300 0000 1004 1704 3d04 3004 4704 3504  ........=.0.G.5.
-00004f20: 3d04 3804 3508 0000 0000 0600 0000 0556  =.8.5..........V
-00004f30: 616c 7565 0700 0000 0e45 7874 7261 4461  alue.....ExtraDa
-00004f40: 7461 4d6f 6465 6c01 0300 0000 1a04 2604  taModel.......&.
-00004f50: 3504 3d04 3d04 3004 4f00 2004 3104 4304  5.=.=.0.O. .1.C.
-00004f60: 3c04 3004 3304 3008 0000 0000 0600 0000  <.0.3.0.........
-00004f70: 0a41 7373 6574 204e 616d 6507 0000 000d  .Asset Name.....
-00004f80: 486f 6c64 696e 6773 4d6f 6465 6c01 0300  HoldingsModel...
-00004f90: 0000 1c04 1204 3004 3b04 4e04 4204 3000  ......0.;.N.B.0.
-00004fa0: 2f04 2104 4704 5104 4200 2f04 2604 1108  /.!.G.Q.B./.&...
-00004fb0: 0000 0000 0600 0000 1643 7572 7265 6e63  .........Currenc
-00004fc0: 792f 4163 636f 756e 742f 4173 7365 7407  y/Account/Asset.
-00004fd0: 0000 000d 486f 6c64 696e 6773 4d6f 6465  ....HoldingsMode
-00004fe0: 6c01 0300 0000 0a04 2d04 3a04 4104 3f00  l.......-.:.A.?.
-00004ff0: 3a08 0000 0000 0600 0000 0445 7870 3a07  :..........Exp:.
-00005000: 0000 000d 486f 6c64 696e 6773 4d6f 6465  ....HoldingsMode
-00005010: 6c01 0300 0000 1404 2604 3504 3d04 3000  l.......&.5.=.0.
-00005020: 2004 3704 3004 3a04 4000 2e08 0000 0000   .7.0.:.@.......
-00005030: 0600 0000 044c 6173 7407 0000 000d 486f  .....Last.....Ho
-00005040: 6c64 696e 6773 4d6f 6465 6c01 0300 0000  ldingsModel.....
-00005050: 3404 1404 3004 4204 3000 2004 3f04 3e04  4...0.B.0. .?.>.
-00005060: 4104 3b04 3504 3404 3d04 3504 3900 2004  A.;.5.4.=.5.9. .
-00005070: 3a04 3e04 4204 3804 4004 3e04 3204 3a04  :.>.B.8.@.>.2.:.
-00005080: 3800 3a00 2008 0000 0000 0600 0000 114c  8.:. ..........L
-00005090: 6173 7420 7175 6f74 6520 6461 7465 3a20  ast quote date: 
-000050a0: 0700 0000 0d48 6f6c 6469 6e67 734d 6f64  .....HoldingsMod
-000050b0: 656c 0103 0000 0014 0426 0435 043d 0430  el.......&.5.=.0
-000050c0: 0020 043e 0442 043a 0440 002e 0800 0000  . .>.B.:.@......
-000050d0: 0006 0000 0004 4f70 656e 0700 0000 0d48  ......Open.....H
-000050e0: 6f6c 6469 6e67 734d 6f64 656c 0103 0000  oldingsModel....
-000050f0: 0006 041f 0438 0423 0800 0000 0006 0000  .....8.#........
-00005100: 0003 502f 4c07 0000 000d 486f 6c64 696e  ..P/L.....Holdin
-00005110: 6773 4d6f 6465 6c01 0300 0000 0c04 1f04  gsModel.........
-00005120: 3804 2300 2c00 2000 2508 0000 0000 0600  8.#.,. .%.......
-00005130: 0000 0650 2f4c 2c20 2507 0000 000d 486f  ...P/L, %.....Ho
-00005140: 6c64 696e 6773 4d6f 6465 6c01 0300 0000  ldingsModel.....
-00005150: 0c04 1a04 3e04 3b00 2d04 3204 3e08 0000  ....>.;.-.2.>...
-00005160: 0000 0600 0000 0351 7479 0700 0000 0d48  .......Qty.....H
-00005170: 6f6c 6469 6e67 734d 6f64 656c 0103 0000  oldingsModel....
-00005180: 000e 0414 043e 043b 044f 002c 0020 0025  .....>.;.O.,. .%
-00005190: 0800 0000 0006 0000 0008 5368 6172 652c  ..........Share,
-000051a0: 2025 0700 0000 0d48 6f6c 6469 6e67 734d   %.....HoldingsM
-000051b0: 6f64 656c 0103 0000 000c 041e 0446 0435  odel.........F.5
-000051c0: 043d 043a 0430 0800 0000 0006 0000 0005  .=.:.0..........
-000051d0: 5661 6c75 6507 0000 000d 486f 6c64 696e  Value.....Holdin
-000051e0: 6773 4d6f 6465 6c01 0300 0000 1004 1e04  gsModel.........
-000051f0: 4604 3504 3d04 3a04 3000 2c00 2008 0000  F.5.=.:.0.,. ...
-00005200: 0000 0600 0000 0756 616c 7565 2c20 0700  .......Value, ..
-00005210: 0000 0d48 6f6c 6469 6e67 734d 6f64 656c  ...HoldingsModel
-00005220: 0103 0000 0016 041f 043e 0440 0442 0444  .........>.@.B.D
-00005230: 0435 043b 044c 0020 0426 0411 0800 0000  .5.;.L. .&......
-00005240: 0006 0000 0008 486f 6c64 696e 6773 0700  ......Holdings..
-00005250: 0000 0e48 6f6c 6469 6e67 7352 6570 6f72  ...HoldingsRepor
-00005260: 7401 0300 0000 1a04 1e04 4604 3504 3d04  t.........F.5.=.
-00005270: 3804 4204 4c00 2004 3d04 3004 3b04 3e04  8.B.L. .=.0.;.>.
-00005280: 3308 0000 0000 0600 0000 0c45 7374 696d  3..........Estim
-00005290: 6174 6520 7461 7807 0000 0014 486f 6c64  ate tax.....Hold
-000052a0: 696e 6773 5265 706f 7274 5769 6e64 6f77  ingsReportWindow
-000052b0: 0103 0000 0016 041f 043e 0440 0442 0444  .........>.@.B.D
-000052c0: 0435 043b 044c 0020 0426 0411 0800 0000  .5.;.L. .&......
-000052d0: 0006 0000 0008 486f 6c64 696e 6773 0700  ......Holdings..
-000052e0: 0000 1448 6f6c 6469 6e67 7352 6570 6f72  ...HoldingsRepor
-000052f0: 7457 696e 646f 7701 0300 0000 1404 1f04  tWindow.........
-00005300: 3e04 4004 4204 4304 3304 3004 3b04 3804  >.@.B.C.3.0.;.8.
-00005310: 4f08 0000 0000 0600 0000 0850 6f72 7475  O..........Portu
-00005320: 6761 6c07 0000 0014 486f 6c64 696e 6773  gal.....Holdings
-00005330: 5265 706f 7274 5769 6e64 6f77 0103 0000  ReportWindow....
-00005340: 000c 0420 043e 0441 0441 0438 044f 0800  ... .>.A.A.8.O..
-00005350: 0000 0006 0000 0006 5275 7373 6961 0700  ........Russia..
-00005360: 0000 1448 6f6c 6469 6e67 7352 6570 6f72  ...HoldingsRepor
-00005370: 7457 696e 646f 7701 0300 0000 2804 1f04  tWindow.....(...
-00005380: 3e04 3a04 3004 3704 3004 4204 4c00 2004  >.:.0.7.0.B.L. .
-00005390: 3304 4004 3004 4404 3804 3a00 2004 4604  3.@.0.D.8.:. .F.
-000053a0: 3504 3d04 4b08 0000 0000 0600 0000 1053  5.=.K..........S
-000053b0: 686f 7720 5072 6963 6520 4368 6172 7407  how Price Chart.
-000053c0: 0000 0014 486f 6c64 696e 6773 5265 706f  ....HoldingsRepo
-000053d0: 7274 5769 6e64 6f77 0103 0000 0022 0412  rtWindow....."..
-000053e0: 0430 043b 044e 0442 0430 0020 043f 0435  .0.;.N.B.0. .?.5
-000053f0: 0440 0435 0441 0447 0451 0442 0430 003a  .@.5.A.G.Q.B.0.:
-00005400: 0800 0000 0006 0000 0010 436f 6d6d 6f6e  ..........Common
-00005410: 2063 7572 7265 6e63 793a 0700 0000 0e48   currency:.....H
-00005420: 6f6c 6469 6e67 7357 6964 6765 7401 0300  oldingsWidget...
-00005430: 0000 1604 1f04 3e04 4004 4204 4404 3504  ......>.@.B.D.5.
-00005440: 3b04 4c00 2004 2604 1108 0000 0000 0600  ;.L. .&.........
-00005450: 0000 0848 6f6c 6469 6e67 7307 0000 000e  ...Holdings.....
-00005460: 486f 6c64 696e 6773 5769 6467 6574 0103  HoldingsWidget..
-00005470: 0000 0018 0421 043e 0445 0440 0430 043d  .....!.>.E.@.0.=
-00005480: 0438 0442 044c 002e 002e 002e 0800 0000  .8.B.L..........
-00005490: 0006 0000 0007 5361 7665 2e2e 2e07 0000  ......Save......
-000054a0: 000e 486f 6c64 696e 6773 5769 6467 6574  ..HoldingsWidget
-000054b0: 0103 0000 0014 0064 0064 002f 004d 004d  .......d.d./.M.M
-000054c0: 002f 0079 0079 0079 0079 0800 0000 0006  ./.y.y.y.y......
-000054d0: 0000 000a 6464 2f4d 4d2f 7979 7979 0700  ....dd/MM/yyyy..
-000054e0: 0000 0e48 6f6c 6469 6e67 7357 6964 6765  ...HoldingsWidge
-000054f0: 7401 0300 0000 3404 2204 3804 3f00 2004  t.....4.".8.?. .
-00005500: 2604 1100 2004 3d04 3500 2004 3f04 3e04  &... .=.5. .?.>.
-00005510: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
-00005520: 3504 4204 4104 4f00 3a00 2008 0000 0000  5.B.A.O.:. .....
-00005530: 0600 0000 1c41 7373 6574 2074 7970 6520  .....Asset type 
-00005540: 6973 6e27 7420 7375 7070 6f72 7465 643a  isn't supported:
-00005550: 2007 0000 0004 4942 4b52 0103 0000 0054   .....IBKR.....T
-00005560: 041a 043e 0440 043f 043e 0440 0430 0442  ...>.@.?.>.@.0.B
-00005570: 0438 0432 043d 043e 0435 0020 0434 0435  .8.2.=.>.5. .4.5
-00005580: 0439 0441 0442 0432 0438 0435 0020 043d  .9.A.B.2.8.5. .=
-00005590: 0435 0020 043f 043e 0434 0434 0435 0440  .5. .?.>.4.4.5.@
-000055a0: 0436 0438 0432 0430 0435 0442 0441 044f  .6.8.2.0.5.B.A.O
-000055b0: 003a 0020 0800 0000 0006 0000 0022 436f  .:. ........."Co
-000055c0: 7270 6f72 6174 6520 6163 7469 6f6e 2069  rporate action i
-000055d0: 736e 2774 2073 7570 706f 7274 6564 3a20  sn't supported: 
-000055e0: 0700 0000 0449 424b 5201 0300 0000 4604  .....IBKR.....F.
-000055f0: 1d04 3504 3e04 3404 3d04 3e04 3704 3d04  ..5.>.4.=.>.7.=.
-00005600: 3004 4704 3d04 3e04 3500 2004 4104 3e04  0.G.=.>.5. .A.>.
-00005610: 3204 3f04 3004 3404 3504 3d04 3804 3500  2.?.0.4.5.=.8.5.
-00005620: 2004 4104 4704 5104 4204 3000 2004 3404   .A.G.Q.B.0. .4.
-00005630: 3b04 4f00 2008 0000 0000 0600 0000 1b4d  ;.O. ..........M
-00005640: 756c 7469 706c 6520 6163 636f 756e 7420  ultiple account 
-00005650: 6d61 7463 6820 666f 7220 0700 0000 0449  match for .....I
-00005660: 424b 5201 0300 0000 6800 4a00 5300 4f00  BKR.....h.J.S.O.
-00005670: 4e00 2004 4204 4d04 3300 2000 2700 6400  N. .B.M.3. .'.d.
-00005680: 6f00 6300 7500 6d00 6500 6e00 7400 2700  o.c.u.m.e.n.t.'.
-00005690: 2004 3e04 4204 4104 4304 4204 4104 4204   .>.B.A.C.B.A.B.
-000056a0: 3204 4304 3504 4200 2004 3204 3d04 4304  2.C.5.B. .2.=.C.
-000056b0: 4204 4004 3800 2004 4204 4d04 3304 3000  B.@.8. .B.M.3.0.
-000056c0: 2000 2700 7400 6900 6300 6b00 6500 7400   .'.t.i.c.k.e.t.
-000056d0: 2708 0000 0000 0600 0000 2a43 616e 2774  '.........*Can't
-000056e0: 2066 696e 6420 2764 6f63 756d 656e 7427   find 'document'
-000056f0: 2074 6167 2069 6e20 6a73 6f6e 2027 7469   tag in json 'ti
-00005700: 636b 6574 2707 0000 0010 496d 706f 7274  cket'.....Import
-00005710: 536c 6970 4469 616c 6f67 0103 0000 0072  SlipDialog.....r
-00005720: 004a 0053 004f 004e 0020 0442 044d 0433  .J.S.O.N. .B.M.3
-00005730: 0020 0027 006f 0070 0065 0072 0061 0074  . .'.o.p.e.r.a.t
-00005740: 0069 006f 006e 0054 0079 0070 0065 0027  .i.o.n.T.y.p.e.'
-00005750: 0020 043e 0442 0441 0443 0442 0441 0442  . .>.B.A.C.B.A.B
-00005760: 0432 0443 0435 0442 0020 0432 043d 0443  .2.C.5.B. .2.=.C
-00005770: 0442 0440 0438 0020 0442 044d 0433 0430  .B.@.8. .B.M.3.0
-00005780: 0020 0027 0074 0069 0063 006b 0065 0074  . .'.t.i.c.k.e.t
-00005790: 0027 0800 0000 0006 0000 002f 4361 6e27  .'........./Can'
-000057a0: 7420 6669 6e64 2027 6f70 6572 6174 696f  t find 'operatio
-000057b0: 6e54 7970 6527 2074 6167 2069 6e20 6a73  nType' tag in js
-000057c0: 6f6e 2027 7469 636b 6574 2707 0000 0010  on 'ticket'.....
-000057d0: 496d 706f 7274 536c 6970 4469 616c 6f67  ImportSlipDialog
-000057e0: 0103 0000 006a 004a 0053 004f 004e 0020  .....j.J.S.O.N. 
-000057f0: 0442 044d 0433 0020 0027 0072 0065 0063  .B.M.3. .'.r.e.c
-00005800: 0065 0069 0070 0074 0027 0020 043e 0442  .e.i.p.t.'. .>.B
-00005810: 0441 0443 0442 0441 0442 0432 0443 0435  .A.C.B.A.B.2.C.5
-00005820: 0442 0020 0432 043d 0443 0442 0440 0438  .B. .2.=.C.B.@.8
-00005830: 0020 0442 044d 0433 0430 0020 0027 0064  . .B.M.3.0. .'.d
-00005840: 006f 0063 0075 006d 0065 006e 0074 0027  .o.c.u.m.e.n.t.'
-00005850: 0800 0000 0006 0000 002b 4361 6e27 7420  .........+Can't 
-00005860: 6669 6e64 2027 7265 6365 6970 7427 2074  find 'receipt' t
-00005870: 6167 2069 6e20 6a73 6f6e 2027 646f 6375  ag in json 'docu
-00005880: 6d65 6e74 2707 0000 0010 496d 706f 7274  ment'.....Import
-00005890: 536c 6970 4469 616c 6f67 0103 0000 005e  SlipDialog.....^
-000058a0: 041a 0430 0442 0435 0433 043e 0440 0438  ...0.B.5.3.>.@.8
-000058b0: 0438 0020 043d 0435 0020 0440 0430 0441  .8. .=.5. .@.0.A
-000058c0: 043f 043e 0437 043d 0430 043d 044b 003a  .?.>.7.=.0.=.K.:
-000058d0: 0020 0054 0065 006e 0073 006f 0072 006c  . .T.e.n.s.o.r.l
-000058e0: 006f 0077 0020 043d 0435 0020 043e 0431  .o.w. .=.5. .>.1
-000058f0: 043d 0430 0440 0443 0436 0435 043d 0800  .=.0.@.C.6.5.=..
-00005900: 0000 0006 0000 0036 4361 7465 676f 7269  .......6Categori
-00005910: 6573 2061 7265 206e 6f74 2072 6563 6f67  es are not recog
-00005920: 6e69 7a65 643a 2054 656e 736f 7266 6c6f  nized: Tensorflo
-00005930: 7720 6973 206e 6f74 2066 6f75 6e64 0700  w is not found..
-00005940: 0000 1049 6d70 6f72 7453 6c69 7044 6961  ...ImportSlipDia
-00005950: 6c6f 6701 0300 0000 4a04 1f04 4004 3504  log.....J...@.5.
-00005960: 3204 4b04 4804 3504 3d04 3e00 2004 3c04  2.K.H.5.=.>. .<.
-00005970: 3004 3a04 4104 3804 3c04 3004 3b04 4c04  0.:.A.8.<.0.;.L.
-00005980: 3d04 3e04 3500 2004 4704 3804 4104 3b04  =.>.5. .G.8.A.;.
-00005990: 3e00 2004 3f04 3e04 3f04 4b04 4204 3e04  >. .?.>.?.K.B.>.
-000059a0: 3a00 2e08 0000 0000 0600 0000 194d 6178  :............Max
-000059b0: 2072 6574 7279 2063 6f75 6e74 2065 7863   retry count exc
-000059c0: 6565 6465 642e 0700 0000 1049 6d70 6f72  eeded......Impor
-000059d0: 7453 6c69 7044 6961 6c6f 6701 0300 0000  tSlipDialog.....
-000059e0: 4600 5100 5200 2004 3a04 3e04 3400 2004  F.Q.R. .:.>.4. .
-000059f0: 3d04 3500 2004 3e04 3104 3d04 3004 4004  =.5. .>.1.=.0.@.
-00005a00: 4304 3604 3504 3d00 2004 3200 2004 3104  C.6.5.=. .2. .1.
-00005a10: 4304 4404 3504 4004 3500 2004 3e04 3104  C.D.5.@.5. .>.1.
-00005a20: 3c04 3504 3d04 3008 0000 0000 0600 0000  <.5.=.0.........
-00005a30: 1e4e 6f20 5152 2063 6f64 6573 2066 6f75  .No QR codes fou
-00005a40: 6e64 2069 6e20 636c 6970 626f 6172 6407  nd in clipboard.
-00005a50: 0000 0010 496d 706f 7274 536c 6970 4469  ....ImportSlipDi
-00005a60: 616c 6f67 0103 0000 0036 0051 0052 002d  alog.....6.Q.R.-
-00005a70: 043a 043e 0434 0020 0432 0020 0444 0430  .:.>.4. .2. .D.0
-00005a80: 0439 043b 0435 0020 043d 0435 0020 043e  .9.;.5. .=.5. .>
-00005a90: 0431 043d 0430 0440 0443 0436 0435 043d  .1.=.0.@.C.6.5.=
-00005aa0: 0800 0000 0006 0000 001e 4e6f 2051 5220  ..........No QR 
-00005ab0: 636f 6465 7320 7765 7265 2066 6f75 6e64  codes were found
-00005ac0: 2069 6e20 6669 6c65 0700 0000 1049 6d70   in file.....Imp
-00005ad0: 6f72 7453 6c69 7044 6961 6c6f 6701 0300  ortSlipDialog...
-00005ae0: 0000 7204 1d04 3504 3204 3e04 3704 3c04  ..r...5.2.>.7.<.
-00005af0: 3e04 3604 3d04 3e00 2004 3404 3e04 3104  >.6.=.>. .4.>.1.
-00005b00: 3004 3204 3804 4204 4c00 2004 4704 3504  0.2.8.B.L. .G.5.
-00005b10: 3a00 3a00 2004 3d04 3500 2004 4304 3a04  :.:. .=.5. .C.:.
-00005b20: 3004 3704 3004 3d00 2004 3a04 3e04 3d04  0.7.0.=. .:.>.=.
-00005b30: 4204 4004 3004 3304 3504 3d04 4200 2004  B.@.0.3.5.=.B. .
-00005b40: 3404 3b04 4f00 2004 3804 3c04 3f04 3e04  4.;.O. .8.<.?.>.
-00005b50: 4004 4204 3008 0000 0000 0600 0000 414e  @.B.0.........AN
-00005b60: 6f74 2070 6f73 7369 626c 6520 746f 2069  ot possible to i
-00005b70: 6d70 6f72 7420 736c 6970 3a20 6361 6e27  mport slip: can'
-00005b80: 7420 696d 706f 7274 3a20 6e6f 2070 6565  t import: no pee
-00005b90: 7220 7365 7420 666f 7220 696d 706f 7274  r set for import
-00005ba0: 0700 0000 1049 6d70 6f72 7453 6c69 7044  .....ImportSlipD
-00005bb0: 6961 6c6f 6701 0300 0000 6604 1d04 3504  ialog.....f...5.
-00005bc0: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
-00005bd0: 2004 3404 3e04 3104 3004 3204 3804 4204   .4.>.1.0.2.8.B.
-00005be0: 4c00 2004 4704 3504 3a00 3a00 2004 3d04  L. .G.5.:.:. .=.
-00005bf0: 3500 2004 4304 3a04 3004 3704 3004 3d00  5. .C.:.0.7.0.=.
-00005c00: 2004 4104 4704 3504 4200 2004 3404 3b04   .A.G.5.B. .4.;.
-00005c10: 4f00 2004 3804 3c04 3f04 3e04 4004 4204  O. .8.<.?.>.@.B.
-00005c20: 3008 0000 0000 0600 0000 364e 6f74 2070  0.........6Not p
-00005c30: 6f73 7369 626c 6520 746f 2069 6d70 6f72  ossible to impor
-00005c40: 7420 736c 6970 3a20 6e6f 2061 6363 6f75  t slip: no accou
-00005c50: 6e74 2073 6574 2066 6f72 2069 6d70 6f72  nt set for impor
-00005c60: 7407 0000 0010 496d 706f 7274 536c 6970  t.....ImportSlip
-00005c70: 4469 616c 6f67 0103 0000 0078 041d 0435  Dialog.....x...5
-00005c80: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
-00005c90: 0020 0434 043e 0431 0430 0432 0438 0442  . .4.>.1.0.2.8.B
-00005ca0: 044c 0020 0447 0435 043a 003a 0020 043a  .L. .G.5.:.:. .:
-00005cb0: 0430 0442 0435 0433 043e 0440 0438 0438  .0.B.5.3.>.@.8.8
-00005cc0: 0020 0443 043a 0430 0437 0430 043d 044b  . .C.:.0.7.0.=.K
-00005cd0: 0020 043d 0435 0020 0434 043b 044f 0020  . .=.5. .4.;.O. 
-00005ce0: 0432 0441 0435 0445 0020 0441 0442 0440  .2.A.5.E. .A.B.@
-00005cf0: 043e 043a 0800 0000 0006 0000 0038 4e6f  .>.:.........8No
-00005d00: 7420 706f 7373 6962 6c65 2074 6f20 696d  t possible to im
-00005d10: 706f 7274 2073 6c69 703a 2073 6f6d 6520  port slip: some 
-00005d20: 6361 7465 676f 7269 6573 2061 7265 206e  categories are n
-00005d30: 6f74 2073 6574 0700 0000 1049 6d70 6f72  ot set.....Impor
-00005d40: 7453 6c69 7044 6961 6c6f 6701 0300 0000  tSlipDialog.....
-00005d50: 5404 1d04 3504 3204 3e04 3704 3c04 3e04  T...5.2.>.7.<.>.
-00005d60: 3604 3d04 3e00 2004 4004 3004 4104 3f04  6.=.>. .@.0.A.?.
-00005d70: 3e04 3704 3d04 3004 4204 4c00 2004 3f04  >.7.=.0.B.L. .?.
-00005d80: 4004 3e04 4704 3804 4204 3004 3d04 3d04  @.>.G.8.B.0.=.=.
-00005d90: 4b04 3900 2000 5100 5200 2d04 3a04 3e04  K.9. .Q.R.-.:.>.
-00005da0: 3400 3a00 2008 0000 0000 0600 0000 2b51  4.:. .........+Q
-00005db0: 5220 6176 6169 6c61 626c 6520 6275 7420  R available but 
-00005dc0: 7061 7474 6572 6e20 6973 6e27 7420 7265  pattern isn't re
-00005dd0: 636f 676e 697a 6564 3a20 0700 0000 1049  cognized: .....I
-00005de0: 6d70 6f72 7453 6c69 7044 6961 6c6f 6701  mportSlipDialog.
-00005df0: 0300 0000 0800 5100 5200 3a00 2008 0000  ......Q.R.:. ...
-00005e00: 0000 0600 0000 0451 523a 2007 0000 0010  .......QR: .....
-00005e10: 496d 706f 7274 536c 6970 4469 616c 6f67  ImportSlipDialog
-00005e20: 0103 0000 0030 0412 044b 0431 0435 0440  .....0...K.1.5.@
-00005e30: 0438 0442 0435 0020 0444 0430 0439 043b  .8.B.5. .D.0.9.;
-00005e40: 0020 0441 0020 0051 0052 002d 043a 043e  . .A. .Q.R.-.:.>
-00005e50: 0434 043e 043c 0800 0000 0006 0000 0018  .4.>.<..........
-00005e60: 5365 6c65 6374 2066 696c 6520 7769 7468  Select file with
-00005e70: 2051 5220 636f 6465 0700 0000 1049 6d70   QR code.....Imp
-00005e80: 6f72 7453 6c69 7044 6961 6c6f 6701 0300  ortSlipDialog...
-00005e90: 0000 4204 1204 4b04 3104 3504 4004 3804  ..B...K.1.5.@.8.
-00005ea0: 4204 3500 2004 4404 3004 3904 3b00 2004  B.5. .D.0.9.;. .
-00005eb0: 4100 2000 4a00 5300 4f00 4e00 2d04 3404  A. .J.S.O.N.-.4.
-00005ec0: 3004 3d04 3d04 4b04 3c04 3800 2004 4704  0.=.=.K.<.8. .G.
-00005ed0: 3504 3a04 3008 0000 0000 0600 0000 1f53  5.:.0..........S
-00005ee0: 656c 6563 7420 6669 6c65 2077 6974 6820  elect file with 
-00005ef0: 736c 6970 204a 534f 4e20 6461 7461 0700  slip JSON data..
-00005f00: 0000 1049 6d70 6f72 7453 6c69 7044 6961  ...ImportSlipDia
-00005f10: 6c6f 6701 0300 0000 3204 1d04 3504 3804  log.....2...5.8.
-00005f20: 3704 3204 3504 4104 4204 3d04 4b04 3900  7.2.5.A.B.=.K.9.
-00005f30: 2004 4204 3804 3f00 2004 3e04 3f04 3504   .B.8.?. .>.?.5.
-00005f40: 4004 3004 4604 3804 3800 2008 0000 0000  @.0.F.8.8. .....
-00005f50: 0600 0000 1755 6e6b 6e6f 776e 206f 7065  .....Unknown ope
-00005f60: 7261 7469 6f6e 2074 7970 6520 0700 0000  ration type ....
-00005f70: 1049 6d70 6f72 7453 6c69 7044 6961 6c6f  .ImportSlipDialo
-00005f80: 6701 0300 0000 0600 2027 9c00 2008 0000  g....... '.. ...
-00005f90: 0000 0600 0000 0520 e29e 9c20 0700 0000  ....... ... ....
-00005fa0: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
-00005fb0: 0000 000a 0421 0447 0435 0442 003a 0800  .....!.G.5.B.:..
-00005fc0: 0000 0006 0000 0008 4163 636f 756e 743a  ........Account:
-00005fd0: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
-00005fe0: 6c67 0103 0000 0010 0414 043e 0431 0430  lg.........>.1.0
-00005ff0: 0432 0438 0442 044c 0800 0000 0006 0000  .2.8.B.L........
-00006000: 0003 4164 6407 0000 000d 496d 706f 7274  ..Add.....Import
-00006010: 536c 6970 446c 6701 0300 0000 0c04 2104  SlipDlg.......!.
-00006020: 4304 3c04 3c04 3000 3a08 0000 0000 0600  C.<.<.0.:.......
-00006030: 0000 0741 6d6f 756e 743a 0700 0000 0d49  ...Amount:.....I
-00006040: 6d70 6f72 7453 6c69 7044 6c67 0103 0000  mportSlipDlg....
-00006050: 0032 0410 0432 0442 043e 002d 043d 0430  .2...2.B.>.-.=.0
-00006060: 0437 043d 0430 0447 0435 043d 0438 0435  .7.=.0.G.5.=.8.5
-00006070: 0020 043a 0430 0442 0435 0433 043e 0440  . .:.0.B.5.3.>.@
-00006080: 0438 0439 0800 0000 0006 0000 0016 4175  .8.9..........Au
-00006090: 746f 2d61 7373 6967 6e20 6361 7465 676f  to-assign catego
-000060a0: 7269 6573 0700 0000 0d49 6d70 6f72 7453  ries.....ImportS
-000060b0: 6c69 7044 6c67 0103 0000 000c 041a 0430  lipDlg.........0
-000060c0: 043c 0435 0440 0430 0800 0000 0006 0000  .<.5.@.0........
-000060d0: 0006 4361 6d65 7261 0700 0000 0d49 6d70  ..Camera.....Imp
-000060e0: 6f72 7453 6c69 7044 6c67 0103 0000 0010  ortSlipDlg......
-000060f0: 041e 0447 0438 0441 0442 0438 0442 044c  ...G.8.A.B.8.B.L
-00006100: 0800 0000 0006 0000 0005 436c 6561 7207  ..........Clear.
-00006110: 0000 000d 496d 706f 7274 536c 6970 446c  ....ImportSlipDl
-00006120: 6701 0300 0000 0e04 1704 3004 3a04 4004  g.........0.:.@.
-00006130: 4b04 4204 4c08 0000 0000 0600 0000 0543  K.B.L..........C
-00006140: 6c6f 7365 0700 0000 0d49 6d70 6f72 7453  lose.....ImportS
-00006150: 6c69 7044 6c67 0103 0000 001a 0414 0430  lipDlg.........0
-00006160: 0442 0430 0020 002f 0020 0412 0440 0435  .B.0. ./. ...@.5
-00006170: 043c 044f 003a 0800 0000 0006 0000 000c  .<.O.:..........
-00006180: 4461 7465 202f 2054 696d 653a 0700 0000  Date / Time:....
-00006190: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
-000061a0: 0000 0016 0414 0430 0442 0430 002f 0412  .......0.B.0./..
-000061b0: 0440 0435 043c 044f 003a 0800 0000 0006  .@.5.<.O.:......
-000061c0: 0000 000a 4461 7465 2f54 696d 653a 0700  ....Date/Time:..
-000061d0: 0000 0d49 6d70 6f72 7453 6c69 7044 6c67  ...ImportSlipDlg
-000061e0: 0103 0000 0006 0424 0414 003a 0800 0000  .......$...:....
-000061f0: 0006 0000 0003 4644 3a07 0000 000d 496d  ......FD:.....Im
-00006200: 706f 7274 536c 6970 446c 6701 0300 0000  portSlipDlg.....
-00006210: 0604 2404 1d00 3a08 0000 0000 0600 0000  ..$...:.........
-00006220: 0346 4e3a 0700 0000 0d49 6d70 6f72 7453  .FN:.....ImportS
-00006230: 6c69 7044 6c67 0103 0000 0006 0424 041f  lipDlg.......$..
-00006240: 003a 0800 0000 0006 0000 0003 4650 3a07  .:..........FP:.
-00006250: 0000 000d 496d 706f 7274 536c 6970 446c  ....ImportSlipDl
-00006260: 6701 0300 0000 2604 2104 3a04 3004 3d04  g.....&.!.:.0.=.
-00006270: 3804 4004 3e04 3204 3004 4204 4c00 2004  8.@.>.2.0.B.L. .
-00006280: 3a04 3004 3c04 3504 4004 3e04 3908 0000  :.0.<.5.@.>.9...
-00006290: 0000 0600 0000 0f47 6574 2066 726f 6d20  .......Get from 
-000062a0: 6361 6d65 7261 0700 0000 0d49 6d70 6f72  camera.....Impor
-000062b0: 7453 6c69 7044 6c67 0103 0000 0024 041f  tSlipDlg.....$..
-000062c0: 043e 043b 0443 0447 0438 0442 044c 0020  .>.;.C.G.8.B.L. 
-000062d0: 0438 0437 0020 0431 0443 0444 0435 0440  .8.7. .1.C.D.5.@
-000062e0: 0430 0800 0000 0006 0000 0012 4765 7420  .0..........Get 
-000062f0: 6672 6f6d 2063 6c69 7062 6f61 7264 0700  from clipboard..
-00006300: 0000 0d49 6d70 6f72 7453 6c69 7044 6c67  ...ImportSlipDlg
-00006310: 0103 0000 0030 041f 043e 043b 0443 0447  .....0...>.;.C.G
-00006320: 0438 0442 044c 0020 0447 0435 043a 0020  .8.B.L. .G.5.:. 
-00006330: 0441 0020 0441 0430 0439 0442 0430 0020  .A. .A.0.9.B.0. 
-00006340: 0424 041d 0421 0800 0000 0006 0000 0016  .$...!..........
-00006350: 4765 7420 736c 6970 2066 726f 6d20 696e  Get slip from in
-00006360: 7465 726e 6574 0700 0000 0d49 6d70 6f72  ternet.....Impor
-00006370: 7453 6c69 7044 6c67 0103 0000 0016 0418  tSlipDlg........
-00006380: 043c 043f 043e 0440 0442 0020 0447 0435  .<.?.>.@.B. .G.5
-00006390: 043a 0430 0800 0000 0006 0000 000b 496d  .:.0..........Im
-000063a0: 706f 7274 2053 6c69 7007 0000 000d 496d  port Slip.....Im
-000063b0: 706f 7274 536c 6970 446c 6701 0300 0000  portSlipDlg.....
-000063c0: 0e04 2104 4204 4004 3e04 3a04 3800 3a08  ..!.B.@.>.:.8.:.
-000063d0: 0000 0000 0600 0000 064c 696e 6573 3a07  .........Lines:.
-000063e0: 0000 000d 496d 706f 7274 536c 6970 446c  ....ImportSlipDl
-000063f0: 6701 0300 0000 2404 1704 3004 3304 4004  g.....$...0.3.@.
-00006400: 4304 3704 3804 4204 4c00 2004 3804 3700  C.7.8.B.L. .8.7.
-00006410: 2004 4404 3004 3904 3b04 3008 0000 0000   .D.0.9.;.0.....
-00006420: 0600 0000 0e4c 6f61 6420 6672 6f6d 2066  .....Load from f
-00006430: 696c 6507 0000 000d 496d 706f 7274 536c  ile.....ImportSl
-00006440: 6970 446c 6701 0300 0000 3604 1704 3004  ipDlg.....6...0.
-00006450: 3304 4304 3704 3804 4204 4c00 2004 4704  3.C.7.8.B.L. .G.
-00006460: 3504 3a04 3000 2004 3804 3700 2000 4a00  5.:.0. .8.7. .J.
-00006470: 5300 4f00 4e00 2d04 4404 3004 3904 3b04  S.O.N.-.D.0.9.;.
-00006480: 3008 0000 0000 0600 0000 184c 6f61 6420  0..........Load 
-00006490: 736c 6970 2066 726f 6d20 4a53 4f4e 2066  slip from JSON f
-000064a0: 696c 6507 0000 000d 496d 706f 7274 536c  ile.....ImportSl
-000064b0: 6970 446c 6701 0300 0000 1604 1a04 3e04  ipDlg.........>.
-000064c0: 3d04 4204 4004 3004 3304 3504 3d04 4200  =.B.@.0.3.5.=.B.
-000064d0: 3a08 0000 0000 0600 0000 0550 6565 723a  :..........Peer:
-000064e0: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
-000064f0: 6c67 0103 0000 000e 041f 043e 043a 0443  lg.........>.:.C
-00006500: 043f 043a 0430 0800 0000 0006 0000 0008  .?.:.0..........
-00006510: 5075 7263 6861 7365 0700 0000 0d49 6d70  Purchase.....Imp
-00006520: 6f72 7453 6c69 7044 6c67 0103 0000 000c  ortSlipDlg......
-00006530: 0051 0052 002d 043a 043e 0434 0800 0000  .Q.R.-.:.>.4....
-00006540: 0006 0000 0007 5152 2d63 6f64 6507 0000  ......QR-code...
-00006550: 000d 496d 706f 7274 536c 6970 446c 6701  ..ImportSlipDlg.
-00006560: 0300 0000 0e04 1204 3e04 3704 3204 4004  ........>.7.2.@.
-00006570: 3004 4208 0000 0000 0600 0000 0652 6574  0.B..........Ret
-00006580: 7572 6e07 0000 000d 496d 706f 7274 536c  urn.....ImportSl
-00006590: 6970 446c 6701 0300 0000 2e04 2304 4104  ipDlg.......#.A.
-000065a0: 4204 3004 3d04 3e04 3204 3804 4204 4c00  B.0.=.>.2.8.B.L.
-000065b0: 2004 4204 4d04 3300 2004 3404 3b04 4f00   .B.M.3. .4.;.O.
-000065c0: 2004 3204 4104 3504 4508 0000 0000 0600   .2.A.5.E.......
-000065d0: 0000 1553 6574 2054 6167 2066 6f72 2061  ...Set Tag for a
-000065e0: 6c6c 206c 696e 6573 0700 0000 0d49 6d70  ll lines.....Imp
-000065f0: 6f72 7453 6c69 7044 6c67 0103 0000 0006  ortSlipDlg......
-00006600: 0427 0435 043a 0800 0000 0006 0000 0004  .'.5.:..........
-00006610: 536c 6970 0700 0000 0d49 6d70 6f72 7453  Slip.....ImportS
-00006620: 6c69 7044 6c67 0103 0000 0016 0414 0430  lipDlg.........0
-00006630: 043d 043d 044b 0435 0020 0447 0435 043a  .=.=.K.5. .G.5.:
-00006640: 0430 0800 0000 0006 0000 0009 536c 6970  .0..........Slip
-00006650: 2064 6174 6107 0000 000d 496d 706f 7274   data.....Import
-00006660: 536c 6970 446c 6701 0300 0000 1c04 1704  SlipDlg.........
-00006670: 3004 3a04 4004 4b04 4204 4c00 2004 3a04  0.:.@.K.B.L. .:.
-00006680: 3004 3c04 3504 4004 4308 0000 0000 0600  0.<.5.@.C.......
-00006690: 0000 0b53 746f 7020 6361 6d65 7261 0700  ...Stop camera..
-000066a0: 0000 0d49 6d70 6f72 7453 6c69 7044 6c67  ...ImportSlipDlg
-000066b0: 0103 0000 0008 0422 0438 043f 003a 0800  .......".8.?.:..
-000066c0: 0000 0006 0000 0005 5479 7065 3a07 0000  ........Type:...
-000066d0: 000d 496d 706f 7274 536c 6970 446c 6701  ..ImportSlipDlg.
-000066e0: 0300 0000 2600 6400 6400 2f00 4d00 4d00  ....&.d.d./.M.M.
-000066f0: 2f00 7900 7900 7900 7900 2000 6800 6800  /.y.y.y.y. .h.h.
-00006700: 3a00 6d00 6d00 3a00 7300 7308 0000 0000  :.m.m.:.s.s.....
-00006710: 0600 0000 1364 642f 4d4d 2f79 7979 7920  .....dd/MM/yyyy 
-00006720: 6868 3a6d 6d3a 7373 0700 0000 0d49 6d70  hh:mm:ss.....Imp
-00006730: 6f72 7453 6c69 7044 6c67 0103 0000 0066  ortSlipDlg.....f
-00006740: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-00006750: 043d 043e 0020 043e 0431 0440 0430 0431  .=.>. .>.1.@.0.1
-00006760: 043e 0442 0430 0442 044c 0020 043e 043f  .>.B.0.B.L. .>.?
-00006770: 0435 0440 0430 0446 0438 044e 0020 0431  .5.@.0.F.8.N. .1
-00006780: 0435 0437 0020 0434 0435 0442 0430 043b  .5.7. .4.5.B.0.;
-00006790: 044c 043d 044b 0445 0020 0434 0430 043d  .L.=.K.E. .4.0.=
-000067a0: 043d 044b 0445 0800 0000 0006 0000 0027  .=.K.E.........'
-000067b0: 4361 6e27 7420 7072 6f63 6573 7320 6f70  Can't process op
-000067c0: 6572 6174 696f 6e20 7769 7468 6f75 7420  eration without 
-000067d0: 6465 7461 696c 7307 0000 000e 496e 636f  details.....Inco
-000067e0: 6d65 5370 656e 6469 6e67 0103 0000 000c  meSpending......
-000067f0: 041a 0443 0440 0441 003a 0020 0800 0000  ...C.@.A.:. ....
-00006800: 0006 0000 0006 5261 7465 3a20 0700 0000  ......Rate: ....
-00006810: 0e49 6e63 6f6d 6553 7065 6e64 696e 6701  .IncomeSpending.
-00006820: 0300 0000 1c04 1404 3e04 4504 3e04 3404  ........>.E.>.4.
-00006830: 4b00 2004 3800 2004 2204 4004 3004 4204  K. .8. .".@.0.B.
-00006840: 4b08 0000 0000 0600 0000 1149 6e63 6f6d  K..........Incom
-00006850: 6520 2620 5370 656e 6469 6e67 0700 0000  e & Spending....
-00006860: 1449 6e63 6f6d 6553 7065 6e64 696e 6752  .IncomeSpendingR
-00006870: 6570 6f72 7401 0300 0000 0604 1004 3f04  eport.........?.
-00006880: 4008 0000 0000 0600 0000 0341 7072 0700  @..........Apr..
-00006890: 0000 1949 6e63 6f6d 6553 7065 6e64 696e  ...IncomeSpendin
-000068a0: 6752 6570 6f72 744d 6f64 656c 0103 0000  gReportModel....
-000068b0: 0006 0410 0432 0433 0800 0000 0006 0000  .....2.3........
-000068c0: 0003 4175 6707 0000 0019 496e 636f 6d65  ..Aug.....Income
-000068d0: 5370 656e 6469 6e67 5265 706f 7274 4d6f  SpendingReportMo
-000068e0: 6465 6c01 0300 0000 0604 1404 3504 3a08  del.........5.:.
-000068f0: 0000 0000 0600 0000 0344 6563 0700 0000  .........Dec....
-00006900: 1949 6e63 6f6d 6553 7065 6e64 696e 6752  .IncomeSpendingR
-00006910: 6570 6f72 744d 6f64 656c 0103 0000 0006  eportModel......
-00006920: 0424 0435 0432 0800 0000 0006 0000 0003  .$.5.2..........
-00006930: 4665 6207 0000 0019 496e 636f 6d65 5370  Feb.....IncomeSp
-00006940: 656e 6469 6e67 5265 706f 7274 4d6f 6465  endingReportMode
-00006950: 6c01 0300 0000 0604 2f04 3d04 3208 0000  l......./.=.2...
-00006960: 0000 0600 0000 034a 616e 0700 0000 1949  .......Jan.....I
-00006970: 6e63 6f6d 6553 7065 6e64 696e 6752 6570  ncomeSpendingRep
-00006980: 6f72 744d 6f64 656c 0103 0000 0006 0418  ortModel........
-00006990: 044e 043b 0800 0000 0006 0000 0003 4a75  .N.;..........Ju
-000069a0: 6c07 0000 0019 496e 636f 6d65 5370 656e  l.....IncomeSpen
-000069b0: 6469 6e67 5265 706f 7274 4d6f 6465 6c01  dingReportModel.
-000069c0: 0300 0000 0604 1804 4e04 3d08 0000 0000  ........N.=.....
-000069d0: 0600 0000 034a 756e 0700 0000 1949 6e63  .....Jun.....Inc
-000069e0: 6f6d 6553 7065 6e64 696e 6752 6570 6f72  omeSpendingRepor
-000069f0: 744d 6f64 656c 0103 0000 0006 041c 0430  tModel.........0
-00006a00: 0440 0800 0000 0006 0000 0003 4d61 7207  .@..........Mar.
-00006a10: 0000 0019 496e 636f 6d65 5370 656e 6469  ....IncomeSpendi
-00006a20: 6e67 5265 706f 7274 4d6f 6465 6c01 0300  ngReportModel...
-00006a30: 0000 0604 1c04 3004 3908 0000 0000 0600  ......0.9.......
-00006a40: 0000 034d 6179 0700 0000 1949 6e63 6f6d  ...May.....Incom
-00006a50: 6553 7065 6e64 696e 6752 6570 6f72 744d  eSpendingReportM
-00006a60: 6f64 656c 0103 0000 0006 041d 043e 044f  odel.........>.O
-00006a70: 0800 0000 0006 0000 0003 4e6f 7607 0000  ..........Nov...
-00006a80: 0019 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
-00006a90: 5265 706f 7274 4d6f 6465 6c01 0300 0000  ReportModel.....
-00006aa0: 0604 1e04 3a04 4208 0000 0000 0600 0000  ....:.B.........
-00006ab0: 034f 6374 0700 0000 1949 6e63 6f6d 6553  .Oct.....IncomeS
-00006ac0: 7065 6e64 696e 6752 6570 6f72 744d 6f64  pendingReportMod
-00006ad0: 656c 0103 0000 0006 0421 0435 043d 0800  el.......!.5.=..
-00006ae0: 0000 0006 0000 0003 5365 7007 0000 0019  ........Sep.....
-00006af0: 496e 636f 6d65 5370 656e 6469 6e67 5265  IncomeSpendingRe
-00006b00: 706f 7274 4d6f 6465 6c01 0300 0000 0a04  portModel.......
-00006b10: 1804 2204 1e04 1304 1e08 0000 0000 0600  ..".............
-00006b20: 0000 0554 4f54 414c 0700 0000 1949 6e63  ...TOTAL.....Inc
-00006b30: 6f6d 6553 7065 6e64 696e 6752 6570 6f72  omeSpendingRepor
-00006b40: 744d 6f64 656c 0103 0000 000e 0412 0430  tModel.........0
-00006b50: 043b 044e 0442 0430 003a 0800 0000 0006  .;.N.B.0.:......
-00006b60: 0000 0009 4375 7272 656e 6379 3a07 0000  ....Currency:...
-00006b70: 001a 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
-00006b80: 5265 706f 7274 5769 6467 6574 0103 0000  ReportWidget....
-00006b90: 001c 0414 043e 0445 043e 0434 044b 0020  .....>.E.>.4.K. 
-00006ba0: 0438 0020 0422 0440 0430 0442 044b 0800  .8. .".@.0.B.K..
-00006bb0: 0000 0006 0000 0011 496e 636f 6d65 2026  ........Income &
-00006bc0: 2053 7065 6e64 696e 6707 0000 001a 496e   Spending.....In
-00006bd0: 636f 6d65 5370 656e 6469 6e67 5265 706f  comeSpendingRepo
-00006be0: 7274 5769 6467 6574 0103 0000 0018 0421  rtWidget.......!
-00006bf0: 043e 0445 0440 0430 043d 0438 0442 044c  .>.E.@.0.=.8.B.L
-00006c00: 002e 002e 002e 0800 0000 0006 0000 0007  ................
-00006c10: 5361 7665 2e2e 2e07 0000 001a 496e 636f  Save........Inco
-00006c20: 6d65 5370 656e 6469 6e67 5265 706f 7274  meSpendingReport
-00006c30: 5769 6467 6574 0103 0000 001c 0414 043e  Widget.........>
-00006c40: 0445 043e 0434 044b 0020 0438 0020 0422  .E.>.4.K. .8. ."
-00006c50: 0440 0430 0442 044b 0800 0000 0006 0000  .@.0.B.K........
-00006c60: 0011 496e 636f 6d65 2026 2053 7065 6e64  ..Income & Spend
-00006c70: 696e 6707 0000 001a 496e 636f 6d65 5370  ing.....IncomeSp
-00006c80: 656e 6469 6e67 5265 706f 7274 5769 6e64  endingReportWind
-00006c90: 6f77 0103 0000 0022 041f 043e 043a 0430  ow....."...>.:.0
-00006ca0: 0437 0430 0442 044c 0020 043e 043f 0435  .7.0.B.L. .>.?.5
-00006cb0: 0440 0430 0446 0438 0438 0800 0000 0006  .@.0.F.8.8......
-00006cc0: 0000 000f 5368 6f77 206f 7065 7261 7469  ....Show operati
-00006cd0: 6f6e 7307 0000 001a 496e 636f 6d65 5370  ons.....IncomeSp
-00006ce0: 656e 6469 6e67 5265 706f 7274 5769 6e64  endingReportWind
-00006cf0: 6f77 0103 0000 0008 0421 0447 0435 0442  ow.......!.G.5.B
-00006d00: 0800 0000 0006 0000 0007 4163 636f 756e  ..........Accoun
-00006d10: 7407 0000 0014 496e 636f 6d65 5370 656e  t.....IncomeSpen
-00006d20: 6469 6e67 5769 6467 6574 0103 0000 0032  dingWidget.....2
-00006d30: 0414 043e 0431 0430 0432 0438 0442 044c  ...>.1.0.2.8.B.L
-00006d40: 0020 0434 0435 0442 0430 043b 044c 043d  . .4.5.B.0.;.L.=
-00006d50: 0443 044e 0020 0437 0430 043f 0438 0441  .C.N. .7.0.?.8.A
-00006d60: 044c 0800 0000 0006 0000 000a 4164 6420  .L..........Add 
-00006d70: 6465 7461 696c 0700 0000 1449 6e63 6f6d  detail.....Incom
-00006d80: 6553 7065 6e64 696e 6757 6964 6765 7401  eSpendingWidget.
-00006d90: 0300 0000 3804 2104 3a04 3e04 3f04 3804  ....8.!.:.>.?.8.
-00006da0: 4004 3e04 3204 3004 4204 4c00 2004 3404  @.>.2.0.B.L. .4.
-00006db0: 3504 4204 3004 3b04 4c04 3d04 4304 4e00  5.B.0.;.L.=.C.N.
-00006dc0: 2004 3704 3004 3f04 3804 4104 4c08 0000   .7.0.?.8.A.L...
-00006dd0: 0000 0600 0000 0b43 6f70 7920 6465 7461  .......Copy deta
-00006de0: 696c 0700 0000 1449 6e63 6f6d 6553 7065  il.....IncomeSpe
-00006df0: 6e64 696e 6757 6964 6765 7401 0300 0000  ndingWidget.....
-00006e00: 1404 1404 3004 4204 3000 2f04 1204 4004  ....0.B.0./...@.
-00006e10: 3504 3c04 4f08 0000 0000 0600 0000 0944  5.<.O..........D
-00006e20: 6174 652f 5469 6d65 0700 0000 1449 6e63  ate/Time.....Inc
-00006e30: 6f6d 6553 7065 6e64 696e 6757 6964 6765  omeSpendingWidge
-00006e40: 7401 0300 0000 0c04 1404 3504 4204 3004  t.........5.B.0.
-00006e50: 3b04 3808 0000 0000 0600 0000 0744 6574  ;.8..........Det
-00006e60: 6169 6c73 0700 0000 1449 6e63 6f6d 6553  ails.....IncomeS
-00006e70: 7065 6e64 696e 6757 6964 6765 7401 0300  pendingWidget...
-00006e80: 0000 4404 1d04 3504 3204 3e04 3704 3c04  ..D...5.2.>.7.<.
-00006e90: 3e04 3604 3d04 3e00 2004 3404 3e04 3104  >.6.=.>. .4.>.1.
-00006ea0: 3004 3204 3804 4204 4c00 2004 3d04 3e04  0.2.8.B.L. .=.>.
-00006eb0: 3204 4304 4e00 2004 3704 3004 3f04 3804  2.C.N. .7.0.?.8.
-00006ec0: 4104 4c00 3a00 2008 0000 0000 0600 0000  A.L.:. .........
-00006ed0: 1a46 6169 6c65 6420 746f 2061 6464 206e  .Failed to add n
-00006ee0: 6577 2072 6563 6f72 643a 2007 0000 0014  ew record: .....
-00006ef0: 496e 636f 6d65 5370 656e 6469 6e67 5769  IncomeSpendingWi
-00006f00: 6467 6574 0103 0000 001c 0414 043e 0445  dget.........>.E
-00006f10: 043e 0434 0020 002f 0020 0420 0430 0441  .>.4. ./. . .0.A
-00006f20: 0445 043e 0434 0800 0000 0006 0000 0011  .E.>.4..........
-00006f30: 496e 636f 6d65 202f 2053 7065 6e64 696e  Income / Spendin
-00006f40: 6707 0000 0014 496e 636f 6d65 5370 656e  g.....IncomeSpen
-00006f50: 6469 6e67 5769 6467 6574 0103 0000 0014  dingWidget......
-00006f60: 041f 0440 0438 043c 0435 0447 0430 043d  ...@.8.<.5.G.0.=
-00006f70: 0438 0435 0800 0000 0006 0000 0004 4e6f  .8.5..........No
-00006f80: 7465 0700 0000 1449 6e63 6f6d 6553 7065  te.....IncomeSpe
-00006f90: 6e64 696e 6757 6964 6765 7401 0300 0000  ndingWidget.....
-00006fa0: 4804 1e04 4804 3804 3104 3a04 3000 2004  H...H.8.1.:.0. .
-00006fb0: 3f04 4004 3800 2004 3704 3004 3f04 3804  ?.@.8. .7.0.?.8.
-00006fc0: 4104 3800 2004 3404 3504 4204 3004 3b04  A.8. .4.5.B.0.;.
-00006fd0: 3504 3900 2004 3e04 3f04 3504 4004 3004  5.9. .>.?.5.@.0.
-00006fe0: 4604 3804 3800 3a00 2008 0000 0000 0600  F.8.8.:. .......
-00006ff0: 0000 214f 7065 7261 7469 6f6e 2064 6574  ..!Operation det
-00007000: 6169 6c73 2073 7562 6d69 7420 6661 696c  ails submit fail
-00007010: 6564 3a20 0700 0000 1449 6e63 6f6d 6553  ed: .....IncomeS
-00007020: 7065 6e64 696e 6757 6964 6765 7401 0300  pendingWidget...
-00007030: 0000 3804 1e04 4804 3804 3104 3a04 3000  ..8...H.8.1.:.0.
-00007040: 2004 3f04 4004 3800 2004 3704 3004 3f04   .?.@.8. .7.0.?.
-00007050: 3804 4104 3800 2004 3e04 3f04 3504 4004  8.A.8. .>.?.5.@.
-00007060: 3004 4604 3804 3800 3a00 2008 0000 0000  0.F.8.8.:. .....
-00007070: 0600 0000 194f 7065 7261 7469 6f6e 2073  .....Operation s
-00007080: 7562 6d69 7420 6661 696c 6564 3a20 0700  ubmit failed: ..
-00007090: 0000 1449 6e63 6f6d 6553 7065 6e64 696e  ...IncomeSpendin
-000070a0: 6757 6964 6765 7401 0300 0000 2004 1e04  gWidget..... ...
-000070b0: 3f04 3b04 3004 4204 3000 2004 3200 2004  ?.;.0.B.0. .2. .
-000070c0: 3204 3004 3b04 4e04 4204 3500 3a08 0000  2.0.;.N.B.5.:...
-000070d0: 0000 0600 0000 1950 6169 6420 696e 2066  .......Paid in f
-000070e0: 6f72 6569 676e 2063 7572 7265 6e63 793a  oreign currency:
-000070f0: 0700 0000 1449 6e63 6f6d 6553 7065 6e64  .....IncomeSpend
-00007100: 696e 6757 6964 6765 7401 0300 0000 1404  ingWidget.......
-00007110: 1a04 3e04 3d04 4204 4004 3004 3304 3504  ..>.=.B.@.0.3.5.
-00007120: 3d04 4208 0000 0000 0600 0000 0450 6565  =.B..........Pee
-00007130: 7207 0000 0014 496e 636f 6d65 5370 656e  r.....IncomeSpen
-00007140: 6469 6e67 5769 6467 6574 0103 0000 0030  dingWidget.....0
-00007150: 0423 0434 0430 043b 0438 0442 044c 0020  .#.4.0.;.8.B.L. 
-00007160: 0434 0435 0442 0430 043b 044c 043d 0443  .4.5.B.0.;.L.=.C
-00007170: 044e 0020 0437 0430 043f 0438 0441 044c  .N. .7.0.?.8.A.L
-00007180: 0800 0000 0006 0000 000d 5265 6d6f 7665  ..........Remove
-00007190: 2064 6574 6169 6c07 0000 0014 496e 636f   detail.....Inco
-000071a0: 6d65 5370 656e 6469 6e67 5769 6467 6574  meSpendingWidget
-000071b0: 0103 0000 000c 0026 0421 0447 0435 0442  .......&.!.G.5.B
-000071c0: 0430 0800 0000 0006 0000 0009 2641 6363  .0..........&Acc
-000071d0: 6f75 6e74 7307 0000 000e 4a41 4c5f 4d61  ounts.....JAL_Ma
-000071e0: 696e 5769 6e64 6f77 0103 0000 0012 0026  inWindow.......&
-000071f0: 0411 044d 043a 0430 043f 002e 002e 002e  ...M.:.0.?......
-00007200: 0800 0000 0006 0000 000a 2642 6163 6b75  ..........&Backu
-00007210: 702e 2e2e 0700 0000 0e4a 414c 5f4d 6169  p........JAL_Mai
-00007220: 6e57 696e 646f 7701 0300 0000 1e00 2604  nWindow.......&.
-00007230: 1104 3004 3704 3e04 3204 3004 4f00 2004  ..0.7.>.2.0.O. .
-00007240: 3204 3004 3b04 4e04 4204 3008 0000 0000  2.0.;.N.B.0.....
-00007250: 0600 0000 0e26 4261 7365 2043 7572 7265  .....&Base Curre
-00007260: 6e63 7907 0000 000e 4a41 4c5f 4d61 696e  ncy.....JAL_Main
-00007270: 5769 6e64 6f77 0103 0000 0014 0026 041a  Window.......&..
-00007280: 0430 0442 0435 0433 043e 0440 0438 0438  .0.B.5.3.>.@.8.8
-00007290: 0800 0000 0006 0000 000b 2643 6174 6567  ..........&Categ
-000072a0: 6f72 6965 7307 0000 000e 4a41 4c5f 4d61  ories.....JAL_Ma
-000072b0: 696e 5769 6e64 6f77 0103 0000 000e 0026  inWindow.......&
-000072c0: 0414 0430 043d 043d 044b 0435 0800 0000  ...0.=.=.K.5....
-000072d0: 0006 0000 0005 2644 6174 6107 0000 000e  ......&Data.....
-000072e0: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
-000072f0: 0000 000c 0026 0412 044b 0445 043e 0434  .....&...K.E.>.4
-00007300: 0800 0000 0006 0000 0005 2645 7869 7407  ..........&Exit.
-00007310: 0000 000e 4a41 4c5f 4d61 696e 5769 6e64  ....JAL_MainWind
-00007320: 6f77 0103 0000 0010 0026 042d 043a 0441  ow.......&.-.:.A
-00007330: 043f 043e 0440 0442 0800 0000 0006 0000  .?.>.@.B........
-00007340: 0007 2645 7870 6f72 7407 0000 000e 4a41  ..&Export.....JA
-00007350: 4c5f 4d61 696e 5769 6e64 6f77 0103 0000  L_MainWindow....
-00007360: 000e 0026 0418 043c 043f 043e 0440 0442  ...&...<.?.>.@.B
-00007370: 0800 0000 0006 0000 0007 2649 6d70 6f72  ..........&Impor
-00007380: 7407 0000 000e 4a41 4c5f 4d61 696e 5769  t.....JAL_MainWi
-00007390: 6e64 6f77 0103 0000 0012 0026 041e 0441  ndow.......&...A
-000073a0: 043d 043e 0432 043d 043e 0435 0800 0000  .=.>.2.=.>.5....
-000073b0: 0006 0000 0005 264d 6169 6e07 0000 000e  ......&Main.....
-000073c0: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
-000073d0: 0000 0012 0026 041e 043f 0435 0440 0430  .....&...?.5.@.0
-000073e0: 0446 0438 0438 0800 0000 0006 0000 000b  .F.8.8..........
-000073f0: 264f 7065 7261 7469 6f6e 7307 0000 000e  &Operations.....
-00007400: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
-00007410: 0000 0018 041a 0026 043e 043d 0442 0440  .......&.>.=.B.@
-00007420: 0430 0433 0435 043d 0442 044b 0800 0000  .0.3.5.=.B.K....
-00007430: 0006 0000 0006 2650 6565 7273 0700 0000  ......&Peers....
-00007440: 0e4a 414c 5f4d 6169 6e57 696e 646f 7701  .JAL_MainWindow.
-00007450: 0300 0000 1400 2604 1a04 3e04 4204 3804  ......&...>.B.8.
-00007460: 4004 3e04 3204 3a04 3808 0000 0000 0600  @.>.2.:.8.......
-00007470: 0000 0726 5175 6f74 6573 0700 0000 0e4a  ...&Quotes.....J
-00007480: 414c 5f4d 6169 6e57 696e 646f 7701 0300  AL_MainWindow...
-00007490: 0000 1a00 2604 1a04 3e04 4204 3804 4004  ....&...>.B.8.@.
-000074a0: 3e04 3204 3a04 3800 2e00 2e00 2e08 0000  >.2.:.8.........
-000074b0: 0000 0600 0000 0a26 5175 6f74 6573 2e2e  .......&Quotes..
-000074c0: 2e07 0000 000e 4a41 4c5f 4d61 696e 5769  ......JAL_MainWi
-000074d0: 6e64 6f77 0103 0000 000e 0026 041e 0442  ndow.......&...B
-000074e0: 0447 0435 0442 044b 0800 0000 0006 0000  .G.5.B.K........
-000074f0: 0008 2652 6570 6f72 7473 0700 0000 0e4a  ..&Reports.....J
-00007500: 414c 5f4d 6169 6e57 696e 646f 7701 0300  AL_MainWindow...
-00007510: 0000 2400 2604 1204 3e04 4104 4104 4204  ..$.&...>.A.A.B.
-00007520: 3004 3d04 3e04 3204 3b04 3504 3d04 3804  0.=.>.2.;.5.=.8.
-00007530: 3500 2e00 2e00 2e08 0000 0000 0600 0000  5...............
-00007540: 0b26 5265 7374 6f72 652e 2e2e 0700 0000  .&Restore.......
-00007550: 0e4a 414c 5f4d 6169 6e57 696e 646f 7701  .JAL_MainWindow.
-00007560: 0300 0000 0c00 2604 1e04 4204 4704 5104  ......&...B.G.Q.
-00007570: 4208 0000 0000 0600 0000 0a26 5374 6174  B..........&Stat
-00007580: 656d 656e 7407 0000 000e 4a41 4c5f 4d61  ement.....JAL_Ma
-00007590: 696e 5769 6e64 6f77 0103 0000 000a 0026  inWindow.......&
-000075a0: 0422 044d 0433 0438 0800 0000 0006 0000  .".M.3.8........
-000075b0: 0005 2654 6167 7307 0000 000e 4a41 4c5f  ..&Tags.....JAL_
-000075c0: 4d61 696e 5769 6e64 6f77 0103 0000 001c  MainWindow......
-000075d0: 0026 0426 0435 043d 043d 044b 0435 0020  .&.&.5.=.=.K.5. 
-000075e0: 0431 0443 043c 0430 0433 0438 0800 0000  .1.C.<.0.3.8....
-000075f0: 0006 0000 0007 4126 7373 6574 7307 0000  ......A&ssets...
-00007600: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
-00007610: 0103 0000 004e 041e 0442 0447 0435 0442  .....N...B.G.5.B
-00007620: 0020 043e 0020 0026 0434 0432 0438 0436  . .>. .&.4.2.8.6
-00007630: 0435 043d 0438 044f 0445 0020 043f 043e  .5.=.8.O.E. .?.>
-00007640: 0020 0437 0430 0440 0443 0431 0435 0436  . .7.0.@.C.1.5.6
-00007650: 043d 044b 043c 0020 0441 0447 0435 0442  .=.K.<. .A.G.5.B
-00007660: 0430 043c 0800 0000 0006 0000 001d 466f  .0.<..........Fo
-00007670: 7265 6967 6e20 6163 636f 756e 7473 2026  reign accounts &
-00007680: 666c 6f77 2072 6570 6f72 7407 0000 000e  flow report.....
-00007690: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
-000076a0: 0000 003e 0418 043d 0432 0435 0441 0442  ...>...=.2.5.A.B
-000076b0: 0438 0446 0438 043e 043d 043d 044b 0439  .8.F.8.>.=.=.K.9
-000076c0: 0020 0026 043d 0430 043b 043e 0433 043e  . .&.=.0.;.>.3.>
-000076d0: 0432 044b 0439 0020 043e 0442 0447 0435  .2.K.9. .>.B.G.5
-000076e0: 0442 0800 0000 0006 0000 0016 496e 7665  .B..........Inve
-000076f0: 7374 6d65 6e74 2026 7461 7820 7265 706f  stment &tax repo
-00007700: 7274 0700 0000 0e4a 414c 5f4d 6169 6e57  rt.....JAL_MainW
-00007710: 696e 646f 7701 0300 0000 0a00 2604 2f04  indow.......&./.
-00007720: 3704 4b04 3a08 0000 0000 0600 0000 094c  7.K.:..........L
-00007730: 2661 6e67 7561 6765 0700 0000 0e4a 414c  &anguage.....JAL
-00007740: 5f4d 6169 6e57 696e 646f 7701 0300 0000  _MainWindow.....
-00007750: 2a04 1f04 3504 4004 3504 4104 4704 3804  *...5.@.5.A.G.8.
-00007760: 4204 3004 4204 4c00 2000 2604 3804 4204  B.0.B.L. .&.8.B.
-00007770: 3e04 3304 3800 2e00 2e00 2e08 0000 0000  >.3.8...........
-00007780: 0600 0000 1352 652d 6275 696c 6420 264c  .....Re-build &L
-00007790: 6564 6765 722e 2e2e 0700 0000 0e4a 414c  edger........JAL
-000077a0: 5f4d 6169 6e57 696e 646f 7701 0300 0000  _MainWindow.....
-000077b0: 1604 2704 3504 3a00 2000 5b00 5200 5500  ..'.5.:. .[.R.U.
-000077c0: 5d00 2e00 2e00 2e08 0000 0000 0600 0000  ]...............
-000077d0: 0c53 6c69 7020 5b52 555d 2e2e 2e07 0000  .Slip [RU]......
-000077e0: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
-000077f0: 0103 0000 0006 006a 0061 006c 0800 0000  .......j.a.l....
-00007800: 0006 0000 0003 6a61 6c07 0000 000e 4a41  ......jal.....JA
-00007810: 4c5f 4d61 696e 5769 6e64 6f77 0103 0000  L_MainWindow....
-00007820: 0020 0411 0430 043d 043a 0020 0434 043b  . ...0.=.:. .4.;
-00007830: 044f 0020 0441 0447 0435 0442 0430 0020  .O. .A.G.5.B.0. 
-00007840: 2116 0800 0000 0006 0000 0012 4261 6e6b  !...........Bank
-00007850: 2066 6f72 2061 6363 6f75 6e74 2023 0700   for account #..
-00007860: 0000 0a4a 616c 4163 636f 756e 7401 0300  ...JalAccount...
-00007870: 0000 2a04 2104 4204 4004 3004 3d04 3000  ..*.!.B.@.0.=.0.
-00007880: 2004 3e04 3104 3d04 3e04 3204 3b04 5104   .>.1.=.>.2.;.Q.
-00007890: 3d04 3000 2004 3404 3b04 4f00 2008 0000  =.0. .4.;.O. ...
-000078a0: 0000 0600 0000 1443 6f75 6e74 7279 2075  .......Country u
-000078b0: 7064 6174 6564 2066 6f72 2007 0000 0008  pdated for .....
-000078c0: 4a61 6c41 7373 6574 0103 0000 002a 041a  JalAsset.....*..
-000078d0: 043e 0442 0438 0440 043e 0432 043a 0438  .>.B.8.@.>.2.:.8
-000078e0: 0020 043e 0431 043d 043e 0432 043b 0435  . .>.1.=.>.2.;.5
-000078f0: 043d 044b 003a 0020 0800 0000 0006 0000  .=.K.:. ........
-00007900: 0019 5175 6f74 6174 696f 6e73 2077 6572  ..Quotations wer
-00007910: 6520 7570 6461 7465 643a 2007 0000 0008  e updated: .....
-00007920: 4a61 6c41 7373 6574 0103 0000 0046 0420  JalAsset.....F. 
-00007930: 0435 0433 0438 0441 0442 0440 0430 0446  .5.3.8.A.B.@.0.F
-00007940: 0438 043e 043d 043d 044b 0439 0020 043d  .8.>.=.=.K.9. .=
-00007950: 043e 043c 0435 0440 0020 043e 0431 043d  .>.<.5.@. .>.1.=
-00007960: 043e 0432 043b 0451 043d 0020 0434 043b  .>.2.;.Q.=. .4.;
-00007970: 044f 0020 0800 0000 0006 0000 0017 5265  .O. ..........Re
-00007980: 672e 6e75 6d62 6572 2075 7064 6174 6564  g.number updated
-00007990: 2066 6f72 2007 0000 0008 4a61 6c41 7373   for .....JalAss
-000079a0: 6574 0103 0000 0030 041d 0435 0442 0020  et.....0...5.B. 
-000079b0: 043a 043e 0442 0438 0440 043e 0432 043a  .:.>.B.8.@.>.2.:
-000079c0: 0438 002f 043a 0443 0440 0441 0430 0020  .8./.:.C.@.A.0. 
-000079d0: 0434 043b 044f 0020 0800 0000 0006 0000  .4.;.O. ........
-000079e0: 001c 5468 6572 6520 6172 6520 6e6f 2071  ..There are no q
-000079f0: 756f 7465 2f72 6174 6520 666f 7220 0700  uote/rate for ..
-00007a00: 0000 084a 616c 4173 7365 7401 0300 0000  ...JalAsset.....
-00007a10: 4c04 1d04 3504 3e04 3604 3804 3404 3004  L...5.>.6.8.4.0.
-00007a20: 3d04 3d04 3004 4f00 2004 3f04 3e04 3f04  =.=.0.O. .?.>.?.
-00007a30: 4b04 4204 3a04 3000 2004 3e04 3104 3d04  K.B.:.0. .>.1.=.
-00007a40: 3e04 3204 3804 4204 4c00 2000 4900 5300  >.2.8.B.L. .I.S.
-00007a50: 4900 4e00 2004 3404 3b04 4f00 2008 0000  I.N. .4.;.O. ...
-00007a60: 0000 0600 0000 2655 6e65 7870 6563 7465  ......&Unexpecte
-00007a70: 6420 6174 7465 6d70 7420 746f 2075 7064  d attempt to upd
-00007a80: 6174 6520 4953 494e 2066 6f72 2007 0000  ate ISIN for ...
-00007a90: 0008 4a61 6c41 7373 6574 0103 0000 0006  ..JalAsset......
-00007aa0: 0020 0432 0020 0800 0000 0006 0000 0006  . .2. ..........
-00007ab0: 2069 6e74 6f20 0700 0000 094a 616c 4261   into .....JalBa
-00007ac0: 636b 7570 0103 0000 001c 0410 0440 0445  ckup.........@.E
-00007ad0: 0438 0432 044b 0020 0028 002a 002e 0074  .8.2.K. .(.*...t
-00007ae0: 0067 007a 0029 0800 0000 0006 0000 0010  .g.z.)..........
-00007af0: 4172 6368 6976 6573 2028 2a2e 7467 7a29  Archives (*.tgz)
-00007b00: 0700 0000 094a 616c 4261 636b 7570 0103  .....JalBackup..
-00007b10: 0000 0046 041d 0435 0020 0440 0430 0441  ...F...5. .@.0.A
-00007b20: 043f 043e 0437 043d 0430 043d 0430 0020  .?.>.7.=.0.=.0. 
-00007b30: 043c 0435 0442 043a 0430 0020 0440 0435  .<.5.B.:.0. .@.5
-00007b40: 0437 0435 0440 0432 043d 043e 0439 0020  .7.5.@.2.=.>.9. 
-00007b50: 043a 043e 043f 0438 0438 0800 0000 0006  .:.>.?.8.8......
-00007b60: 0000 001b 4261 636b 7570 206c 6162 656c  ....Backup label
-00007b70: 206e 6f74 2072 6563 6f67 6e69 7a65 6407   not recognized.
-00007b80: 0000 0009 4a61 6c42 6163 6b75 7001 0300  ....JalBackup...
-00007b90: 0000 4604 2004 3504 3704 3504 4004 3204  ..F. .5.7.5.@.2.
-00007ba0: 3d04 3004 4f00 2004 3a04 3e04 3f04 3804  =.0.O. .:.>.?.8.
-00007bb0: 4f00 2004 3204 3e04 4104 4104 4204 3004  O. .2.>.A.A.B.0.
-00007bc0: 3204 3d04 3e04 3204 3b04 3504 3d04 3000  2.=.>.2.;.5.=.0.
-00007bd0: 2004 3804 3700 3a00 2008 0000 0000 0600   .8.7.:. .......
-00007be0: 0000 1642 6163 6b75 7020 7265 7374 6f72  ...Backup restor
-00007bf0: 6564 2066 726f 6d3a 2007 0000 0009 4a61  ed from: .....Ja
-00007c00: 6c42 6163 6b75 7001 0300 0000 3a04 2004  lBackup.....:. .
-00007c10: 3504 3704 3504 4004 3204 3d04 3004 4f00  5.7.5.@.2.=.0.O.
-00007c20: 2004 3a04 3e04 3f04 3804 4f00 2004 4104   .:.>.?.8.O. .A.
-00007c30: 3e04 4504 4004 3004 3d04 5104 3d04 3000  >.E.@.0.=.Q.=.0.
-00007c40: 2004 3200 3a00 2008 0000 0000 0600 0000   .2.:. .........
-00007c50: 1142 6163 6b75 7020 7361 7665 6420 696e  .Backup saved in
-00007c60: 3a20 0700 0000 094a 616c 4261 636b 7570  : .....JalBackup
-00007c70: 0103 0000 0052 041d 0435 0432 043e 0437  .....R...5.2.>.7
-00007c80: 043c 043e 0436 043d 043e 0020 043f 0440  .<.>.6.=.>. .?.@
-00007c90: 043e 0432 0435 0440 0438 0442 044c 0020  .>.2.5.@.8.B.L. 
-00007ca0: 0434 0430 0442 0443 0020 0440 0435 0437  .4.0.B.C. .@.5.7
-00007cb0: 0435 0440 0432 043d 043e 0439 0020 043a  .5.@.2.=.>.9. .:
-00007cc0: 043e 043f 0438 0438 0800 0000 0006 0000  .>.?.8.8........
-00007cd0: 001a 4361 6e27 7420 7661 6c69 6461 7465  ..Can't validate
-00007ce0: 2062 6163 6b75 7020 6461 7465 0700 0000   backup date....
-00007cf0: 094a 616c 4261 636b 7570 0103 0000 0028  .JalBackup.....(
-00007d00: 0414 0430 043d 043d 044b 0435 0020 0432  ...0.=.=.K.5. .2
-00007d10: 043e 0441 0441 0442 0430 043d 043e 0432  .>.A.A.B.0.=.>.2
-00007d20: 043b 0435 043d 044b 0800 0000 0006 0000  .;.5.=.K........
-00007d30: 000d 4461 7461 2072 6573 746f 7265 6407  ..Data restored.
-00007d40: 0000 0009 4a61 6c42 6163 6b75 7001 0300  ....JalBackup...
-00007d50: 0000 4204 1404 3004 3d04 3d04 4b04 3500  ..B...0.=.=.K.5.
-00007d60: 2004 3104 4b04 3b04 3800 2004 3704 3004   .1.K.;.8. .7.0.
-00007d70: 3304 4004 4304 3604 3504 3d04 4b00 2004  3.@.C.6.5.=.K. .
-00007d80: 3804 3700 2004 3104 4d04 3a04 3004 3f04  8.7. .1.M.:.0.?.
-00007d90: 3000 2e00 0a08 0000 0000 0600 0000 2544  0.............%D
-00007da0: 6174 6162 6173 6520 7761 7320 6c6f 6164  atabase was load
-00007db0: 6564 2066 726f 6d20 7468 6520 6261 636b  ed from the back
-00007dc0: 7570 2e0a 0700 0000 094a 616c 4261 636b  up.......JalBack
-00007dd0: 7570 0103 0000 004e 041d 0435 0020 0443  up.....N...5. .C
-00007de0: 0434 0430 043b 043e 0441 044c 0020 0432  .4.0.;.>.A.L. .2
-00007df0: 043e 0441 0441 0442 0430 043d 043e 0432  .>.A.A.B.0.=.>.2
-00007e00: 0438 0442 044c 0020 0440 0435 0437 0435  .8.B.L. .@.5.7.5
-00007e10: 0440 0432 043d 0443 044e 0020 043a 043e  .@.2.=.C.N. .:.>
-00007e20: 043f 0438 044e 0800 0000 0006 0000 001d  .?.8.N..........
-00007e30: 4661 696c 6564 2074 6f20 7265 7374 6f72  Failed to restor
-00007e40: 6520 6261 636b 7570 2066 696c 6507 0000  e backup file...
-00007e50: 0009 4a61 6c42 6163 6b75 7001 0300 0000  ..JalBackup.....
-00007e60: 3804 2104 3e04 4504 4004 3004 3d04 3804  8.!.>.E.@.0.=.8.
-00007e70: 4204 4c00 2004 4004 3504 3704 3504 4004  B.L. .@.5.7.5.@.
-00007e80: 3204 3d04 4304 4e00 2004 3a04 3e04 3f04  2.=.C.N. .:.>.?.
-00007e90: 3804 4e00 2004 3200 3a08 0000 0000 0600  8.N. .2.:.......
-00007ea0: 0000 0f53 6176 6520 6261 636b 7570 2074  ...Save backup t
-00007eb0: 6f3a 0700 0000 094a 616c 4261 636b 7570  o:.....JalBackup
-00007ec0: 0103 0000 0040 0412 044b 0431 0435 0440  .....@...K.1.5.@
-00007ed0: 0438 0442 0435 0020 0444 0430 0439 043b  .8.B.5. .D.0.9.;
-00007ee0: 0020 0441 0020 0440 0435 0437 0435 0440  . .A. .@.5.7.5.@
-00007ef0: 0432 043d 043e 0439 0020 043a 043e 043f  .2.=.>.9. .:.>.?
-00007f00: 0438 0435 0439 0800 0000 0006 0000 0017  .8.5.9..........
-00007f10: 5365 6c65 6374 2066 696c 6520 7769 7468  Select file with
-00007f20: 2062 6163 6b75 7007 0000 0009 4a61 6c42   backup.....JalB
-00007f30: 6163 6b75 7001 0300 0000 4a04 1d04 3504  ackup.....J...5.
-00007f40: 3204 3504 4004 3d04 4b04 3900 2004 4404  2.5.@.=.K.9. .D.
-00007f50: 3e04 4004 3c04 3004 4200 2004 4404 3004  >.@.<.0.B. .D.0.
-00007f60: 3904 3b04 3000 2004 4004 3504 3704 3504  9.;.0. .@.5.7.5.
-00007f70: 4004 3204 3d04 3e04 3900 2004 3a04 3e04  @.2.=.>.9. .:.>.
-00007f80: 3f04 3804 3808 0000 0000 0600 0000 1b57  ?.8.8..........W
-00007f90: 726f 6e67 2066 6f72 6d61 7420 6f66 2062  rong format of b
-00007fa0: 6163 6b75 7020 6669 6c65 0700 0000 094a  ackup file.....J
-00007fb0: 616c 4261 636b 7570 0103 0000 00c8 0412  alBackup........
-00007fc0: 044b 0020 0434 043e 043b 0436 043d 044b  .K. .4.>.;.6.=.K
-00007fd0: 0020 043f 0435 0440 0435 0437 0430 043f  . .?.5.@.5.7.0.?
-00007fe0: 0443 0441 0442 0438 0442 044c 0020 043f  .C.A.B.8.B.L. .?
-00007ff0: 0440 0438 043b 043e 0436 0435 043d 0438  .@.8.;.>.6.5.=.8
-00008000: 0435 002c 0020 0447 0442 043e 0431 044b  .5.,. .G.B.>.1.K
-00008010: 0020 043f 0440 0438 043c 0435 043d 0438  . .?.@.8.<.5.=.8
-00008020: 0442 044c 0020 0438 0437 043c 0435 043d  .B.L. .8.7.<.5.=
-00008030: 0435 043d 0438 044f 000a 041f 0440 0438  .5.=.8.O.....@.8
-00008040: 043b 043e 0436 0435 043d 0438 0435 0020  .;.>.6.5.=.8.5. 
-00008050: 0441 0435 0439 0447 0430 0441 0020 0437  .A.5.9.G.0.A. .7
-00008060: 0430 0432 0435 0440 0448 0438 0442 0020  .0.2.5.@.H.8.B. 
-00008070: 0441 0432 043e 044e 0020 0440 0430 0431  .A.2.>.N. .@.0.1
-00008080: 043e 0442 0443 0800 0000 0006 0000 0052  .>.B.C.........R
-00008090: 596f 7520 7368 6f75 6c64 2072 6573 7461  You should resta
-000080a0: 7274 2061 7070 6c69 6361 7469 6f6e 2074  rt application t
-000080b0: 6f20 6170 706c 7920 6368 616e 6765 730a  o apply changes.
-000080c0: 4170 706c 6963 6174 696f 6e20 7769 6c6c  Application will
-000080d0: 2062 6520 7465 726d 696e 6174 6564 206e   be terminated n
-000080e0: 6f77 0700 0000 094a 616c 4261 636b 7570  ow.....JalBackup
-000080f0: 0103 0000 0064 041e 043f 0435 0440 0430  .....d...?.5.@.0
-00008100: 0446 0438 044f 0020 0443 0436 0435 0020  .F.8.O. .C.6.5. 
-00008110: 0435 0441 0442 044c 0020 0432 0020 0431  .5.A.B.L. .2. .1
-00008120: 0430 0437 0435 0020 0434 0430 043d 043d  .0.7.5. .4.0.=.=
-00008130: 044b 0445 0020 0438 0020 0431 044b 043b  .K.E. .8. .1.K.;
-00008140: 0430 0020 043f 0440 043e 043f 0443 0449  .0. .?.@.>.?.C.I
-00008150: 0435 043d 0430 003a 0020 0800 0000 0006  .5.=.0.:. ......
-00008160: 0000 0031 4f70 6572 6174 696f 6e20 616c  ...1Operation al
-00008170: 7265 6164 7920 7072 6573 656e 7420 696e  ready present in
-00008180: 2064 6220 616e 6420 7761 7320 736b 6970   db and was skip
-00008190: 7065 643a 2007 0000 0005 4a61 6c44 4201  ped: .....JalDB.
-000081a0: 0300 0000 6e00 2004 3804 3c04 3504 3504  ....n. .8.<.5.5.
-000081b0: 4200 2004 3d04 3504 4104 3e04 4504 4004  B. .=.5.A.>.E.@.
-000081c0: 3004 3d04 5104 3d04 3d04 4b04 3500 2004  0.=.Q.=.=.K.5. .
-000081d0: 3804 3704 3c04 3504 3d04 3504 3d04 3804  8.7.<.5.=.5.=.8.
-000081e0: 4f00 2c00 0a04 3204 4b00 2004 4504 3e04  O.,...2.K. .E.>.
-000081f0: 4204 3804 4204 3500 2004 3804 4500 2004  B.8.B.5. .8.E. .
-00008200: 4104 3e04 4504 4004 3004 3d04 3804 4204  A.>.E.@.0.=.8.B.
-00008210: 4c00 3f08 0000 0000 0600 0000 3120 6861  L.?.........1 ha
-00008220: 7320 756e 636f 6d6d 6974 7465 6420 6368  s uncommitted ch
-00008230: 616e 6765 732c 0a64 6f20 796f 7520 7761  anges,.do you wa
-00008240: 6e74 2074 6f20 7361 7665 2069 743f 0700  nt to save it?..
-00008250: 0000 114a 616c 4f70 6572 6174 696f 6e73  ...JalOperations
-00008260: 5461 6273 0103 0000 0036 0415 0441 0442  Tabs.....6...A.B
-00008270: 044c 0020 043d 0435 0441 043e 0445 0440  .L. .=.5.A.>.E.@
-00008280: 0430 043d 0451 043d 043d 044b 0435 0020  .0.=.Q.=.=.K.5. 
-00008290: 0438 0437 043c 0435 043d 043d 0438 044f  .8.7.<.5.=.=.8.O
-000082a0: 0800 0000 0006 0000 0018 596f 7520 6861  ..........You ha
-000082b0: 7665 2075 6e73 6176 6564 2063 6861 6e67  ve unsaved chang
-000082c0: 6573 0700 0000 114a 616c 4f70 6572 6174  es.....JalOperat
-000082d0: 696f 6e73 5461 6273 0103 0000 005a 041d  ionsTabs.....Z..
-000082e0: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-000082f0: 043e 0020 0443 0434 0430 043b 0438 0442  .>. .C.4.0.;.8.B
-00008300: 044c 0020 043f 0440 0435 0434 043e 043f  .L. .?.@.5.4.>.?
-00008310: 0440 0435 0434 0435 043b 0451 043d 043d  .@.5.4.5.;.Q.=.=
-00008320: 0443 044e 0020 043a 0430 0442 0435 0433  .C.N. .:.0.B.5.3
-00008330: 043e 0440 0438 044e 0800 0000 0006 0000  .>.@.8.N........
-00008340: 0020 4361 6e27 7420 6465 6c65 7465 2070  . Can't delete p
-00008350: 7265 6465 6669 6e65 6420 6361 7465 676f  redefined catego
-00008360: 7279 0700 0000 0b4a 616c 5371 6c45 7272  ry.....JalSqlErr
-00008370: 6f72 0103 0000 009e 042d 0442 0438 0020  or.......-.B.8. 
-00008380: 0434 0430 043d 043d 044b 0435 0020 043d  .4.0.=.=.K.5. .=
-00008390: 0435 0020 043c 043e 0433 0443 0442 0020  .5. .<.>.3.C.B. 
-000083a0: 0431 044b 0442 044c 0020 043c 043e 0434  .1.K.B.L. .<.>.4
-000083b0: 0438 0444 0438 0446 0438 0440 043e 0432  .8.D.8.F.8.@.>.2
-000083c0: 0430 043d 044b 002c 0020 0442 002e 043a  .0.=.K.,. .B...:
-000083d0: 002e 0020 043d 0430 0020 043d 0438 0445  ... .=.0. .=.8.E
-000083e0: 0020 0435 0441 0442 044c 0020 0441 0441  . .5.A.B.L. .A.A
-000083f0: 044b 043b 043a 0430 0020 0432 0020 0434  .K.;.:.0. .2. .4
-00008400: 0440 0443 0433 043e 043c 0020 043c 0435  .@.C.3.>.<. .<.5
-00008410: 0441 0442 0435 0800 0000 0006 0000 003a  .A.B.5.........:
-00008420: 4461 7461 2061 7265 2072 6566 6572 656e  Data are referen
-00008430: 6365 6420 696e 2061 6e6f 7468 6572 2070  ced in another p
-00008440: 6c61 6365 2061 6e64 2063 616e 2774 2062  lace and can't b
-00008450: 6520 6d6f 6469 6669 6564 0700 0000 0b4a  e modified.....J
-00008460: 616c 5371 6c45 7272 6f72 0103 0000 001e  alSqlError......
-00008470: 041e 0448 0438 0431 043a 0430 0020 0432  ...H.8.1.:.0. .2
-00008480: 0020 0434 0430 043d 043d 044b 0445 0800  . .4.0.=.=.K.E..
-00008490: 0000 0006 0000 000e 4461 7461 6261 7365  ........Database
-000084a0: 2065 7272 6f72 0700 0000 0b4a 616c 5371   error.....JalSq
-000084b0: 6c45 7272 6f72 0103 0000 0050 041d 0435  lError.....P...5
-000084c0: 0432 0435 0440 043d 043e 0020 0432 044b  .2.5.@.=.>. .2.K
-000084d0: 0431 0440 0430 043d 0430 0020 0432 0430  .1.@.0.=.0. .2.0
-000084e0: 043b 044e 0442 0430 0020 0434 043b 044f  .;.N.B.0. .4.;.O
-000084f0: 0020 0446 0435 043d 043d 043e 0439 0020  . .F.5.=.=.>.9. 
-00008500: 0431 0443 043c 0430 0433 0438 0800 0000  .1.C.<.0.3.8....
-00008510: 0006 0000 002a 496e 636f 7272 6563 7420  .....*Incorrect 
-00008520: 6375 7272 656e 6379 2061 7373 6967 6e6d  currency assignm
-00008530: 656e 7420 666f 7220 616e 2061 7373 6574  ent for an asset
-00008540: 0700 0000 0b4a 616c 5371 6c45 7272 6f72  .....JalSqlError
-00008550: 0103 0000 0080 041f 043e 043b 0435 0020  .........>.;.5. 
-00008560: 0411 0430 043d 043a 002f 0411 0440 043e  ...0.=.:./...@.>
-00008570: 043a 0435 0440 0020 0434 043e 043b 0436  .:.5.@. .4.>.;.6
-00008580: 043d 043e 0020 0431 044b 0442 044c 0020  .=.>. .1.K.B.L. 
-00008590: 0437 0430 043f 043e 043b 043d 0435 043d  .7.0.?.>.;.=.5.=
-000085a0: 043e 0020 0434 043b 044f 0020 0438 043d  .>. .4.;.O. .8.=
-000085b0: 0432 0435 0441 0442 0438 0446 0438 043e  .2.5.A.B.8.F.8.>
-000085c0: 043d 043d 043e 0433 043e 0020 0441 0447  .=.=.>.3.>. .A.G
-000085d0: 0435 0442 0430 0800 0000 0006 0000 0039  .5.B.0.........9
-000085e0: 496e 7665 7374 6d65 6e74 2061 6363 6f75  Investment accou
-000085f0: 6e74 2073 686f 756c 6420 6861 7665 2061  nt should have a
-00008600: 7373 6f63 6961 7465 6420 6272 6f6b 6572  ssociated broker
-00008610: 2061 7373 6967 6e65 6407 0000 000b 4a61   assigned.....Ja
-00008620: 6c53 716c 4572 726f 7201 0300 0000 8800  lSqlError.......
-00008630: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
-00008640: 3900 2004 4204 4004 3504 3104 4304 4e04  9. .B.@.5.1.C.N.
-00008650: 4200 2004 3f04 3504 4004 3504 4004 3004  B. .?.5.@.5.@.0.
-00008660: 4104 4704 3504 4204 3000 2e00 2004 1204  A.G.5.B.0... ...
-00008670: 4b00 2004 4504 3e04 3404 3804 4204 3500  K. .E.>.4.8.B.5.
-00008680: 2004 3204 4b04 3f04 3e04 3b04 3d04 3804   .2.K.?.>.;.=.8.
-00008690: 4204 4c00 2004 3504 3304 3e00 2004 3f04  B.L. .5.3.>. .?.
-000086a0: 4004 4f04 3c04 3e00 2004 4104 3504 3904  @.O.<.>. .A.5.9.
-000086b0: 4704 3004 4100 3f08 0000 0000 0600 0000  G.0.A.?.........
-000086c0: 3c20 6f70 6572 6174 696f 6e73 2072 6571  < operations req
-000086d0: 7569 7265 2072 6562 7569 6c64 2e20 446f  uire rebuild. Do
-000086e0: 2079 6f75 2077 616e 7420 746f 2064 6f20   you want to do 
-000086f0: 6974 2072 6967 6874 206e 6f77 3f07 0000  it right now?...
-00008700: 0006 4c65 6467 6572 0103 0000 0022 002c  ..Ledger.....".,
-00008710: 0020 043d 043e 0432 0430 044f 0020 0433  . .=.>.2.0.O. .3
-00008720: 0440 0430 043d 0438 0446 0430 003a 0020  .@.0.=.8.F.0.:. 
-00008730: 0800 0000 0006 0000 0010 2c20 6e65 7720  .........., new 
-00008740: 6672 6f6e 7469 6572 3a20 0700 0000 064c  frontier: .....L
-00008750: 6564 6765 7201 0300 0000 1a04 1f04 3e04  edger.........>.
-00008760: 3404 4204 3204 3504 4004 3604 3404 3504  4.B.2.5.@.6.4.5.
-00008770: 3d04 3804 3508 0000 0000 0600 0000 0c43  =.8.5..........C
-00008780: 6f6e 6669 726d 6174 696f 6e07 0000 0006  onfirmation.....
-00008790: 4c65 6467 6572 0103 0000 0094 041f 0440  Ledger.........@
-000087a0: 043e 0438 0437 043e 0448 043b 0430 0020  .>.8.7.>.H.;.0. 
-000087b0: 043e 0448 0438 0431 043a 0430 002e 0020  .>.H.8.1.:.0... 
-000087c0: 0420 0430 0441 0447 0451 0442 0020 0438  . .0.A.G.Q.B. .8
-000087d0: 0442 043e 0433 043e 0432 0020 043d 0435  .B.>.3.>.2. .=.5
-000087e0: 0020 043e 043a 043e 043d 0447 0435 043d  . .>.:.>.=.G.5.=
-000087f0: 002e 0020 041f 0440 043e 0432 0435 0440  ... ...@.>.2.5.@
-00008800: 044c 0442 0435 0020 0441 043e 043e 0431  .L.B.5. .A.>.>.1
-00008810: 0449 0435 043d 0438 044f 0020 043e 0431  .I.5.=.8.O. .>.1
-00008820: 0020 043e 0448 0438 0431 043a 0430 0445  . .>.H.8.1.:.0.E
-00008830: 0800 0000 0006 0000 004d 4578 6365 7074  .........MExcept
-00008840: 696f 6e20 6861 7070 656e 6564 2e20 4c65  ion happened. Le
-00008850: 6467 6572 2069 7320 696e 636f 6d70 6c65  dger is incomple
-00008860: 7465 2e20 506c 6561 7365 2063 6f72 7265  te. Please corre
-00008870: 6374 2065 7272 6f72 7320 6c69 7374 6564  ct errors listed
-00008880: 2069 6e20 6c6f 6707 0000 0006 4c65 6467   in log.....Ledg
-00008890: 6572 0103 0000 004a 0418 0442 043e 0433  er.....J...B.>.3
-000088a0: 0438 0020 0440 0430 0441 0441 0447 0438  .8. .@.0.A.A.G.8
-000088b0: 0442 0430 043d 044b 002e 0020 0417 0430  .B.0.=.K... ...0
-000088c0: 0442 0440 0430 0447 0435 043d 043d 043e  .B.@.0.G.5.=.=.>
-000088d0: 0435 0020 0432 0440 0435 043c 044f 003a  .5. .2.@.5.<.O.:
-000088e0: 0020 0800 0000 0006 0000 0022 4c65 6467  . ........."Ledg
-000088f0: 6572 2069 7320 636f 6d70 6c65 7465 2e20  er is complete. 
-00008900: 456c 6170 7365 6420 7469 6d65 3a20 0700  Elapsed time: ..
-00008910: 0000 064c 6564 6765 7201 0300 0000 2c04  ...Ledger.....,.
-00008920: 2204 4004 3004 3d04 3704 3004 3a04 4604  ".@.0.=.7.0.:.F.
-00008930: 3804 3800 2004 3e04 4204 4104 4304 4204  8.8. .>.B.A.C.B.
-00008940: 4104 4204 3204 4304 4e04 4208 0000 0000  A.B.2.C.N.B.....
-00008950: 0600 0000 0e4c 6567 6572 2069 7320 656d  .....Leger is em
-00008960: 7074 7907 0000 0006 4c65 6467 6572 0103  pty.....Ledger..
-00008970: 0000 0026 041d 0435 0020 0443 043a 0430  ...&...5. .C.:.0
-00008980: 0437 0430 043d 0430 0020 0426 0411 0020  .7.0.=.0. .&... 
-00008990: 0434 043b 044f 003a 0020 0800 0000 0006  .4.;.O.:. ......
-000089a0: 0000 0016 4e6f 2061 7373 6574 2064 6566  ....No asset def
-000089b0: 696e 6564 2066 6f72 3a20 0700 0000 064c  ined for: .....L
-000089c0: 6564 6765 7201 0300 0000 3404 1d04 4300  edger.....4...C.
-000089d0: 2004 4304 3a04 3004 3704 3004 3d04 3000   .C.:.0.7.0.=.0.
-000089e0: 2004 3a04 3004 4204 3504 3304 3e04 4004   .:.0.B.5.3.>.@.
-000089f0: 3804 4f00 2004 3404 3b04 4f00 3a00 2008  8.O. .4.;.O.:. .
-00008a00: 0000 0000 0600 0000 154e 6f20 6361 7465  .........No cate
-00008a10: 676f 7279 2073 6574 2066 6f72 3a20 0700  gory set for: ..
-00008a20: 0000 064c 6564 6765 7201 0300 0000 3404  ...Ledger.....4.
-00008a30: 1d04 3500 2004 4304 3a04 3004 3704 3004  ..5. .C.:.0.7.0.
-00008a40: 3d00 2004 3a04 3e04 3d04 4204 4004 3004  =. .:.>.=.B.@.0.
-00008a50: 3304 3504 3d04 4200 2004 3404 3b04 4f00  3.5.=.B. .4.;.O.
-00008a60: 3a00 2008 0000 0000 0600 0000 114e 6f20  :. ..........No 
-00008a70: 7065 6572 2073 6574 2066 6f72 3a20 0700  peer set for: ..
-00008a80: 0000 064c 6564 6765 7201 0300 0000 2604  ...Ledger.....&.
-00008a90: 1f04 3504 4004 3504 4104 4704 5104 4200  ..5.@.5.A.G.Q.B.
-00008aa0: 2004 3804 4204 3e04 3304 3e04 3200 2004   .8.B.>.3.>.2. .
-00008ab0: 4100 3a00 2008 0000 0000 0600 0000 1a52  A.:. ..........R
-00008ac0: 652d 6275 696c 6469 6e67 206c 6564 6765  e-building ledge
-00008ad0: 7220 7369 6e63 653a 2007 0000 0006 4c65  r since: .....Le
-00008ae0: 6467 6572 0103 0000 0058 041d 0435 0438  dger.....X...5.8
-00008af0: 0437 0432 0435 0441 0442 043d 044b 0439  .7.2.5.A.B.=.K.9
-00008b00: 0020 043f 0430 0440 0430 043c 0435 0442  . .?.0.@.0.<.5.B
-00008b10: 0440 0020 043a 0440 0438 0442 0438 0447  .@. .:.@.8.B.8.G
-00008b20: 043d 043e 0441 0442 0438 0020 0441 043e  .=.>.A.B.8. .A.>
-00008b30: 043e 0431 0449 0435 043d 0438 044f 003a  .>.1.I.5.=.8.O.:
-00008b40: 0020 0800 0000 0006 0000 0020 556e 6b6e  . ......... Unkn
-00008b50: 6f77 6e20 6c6f 6767 696e 6720 6c65 7665  own logging leve
-00008b60: 6c20 7072 6f76 6964 6564 3a20 0700 0000  l provided: ....
-00008b70: 094c 6f67 5669 6577 6572 0103 0000 000c  .LogViewer......
-00008b80: 25b2 0020 006c 006f 0067 0073 0800 0000  %.. .l.o.g.s....
-00008b90: 0006 0000 0008 e296 b220 6c6f 6773 0700  ......... logs..
-00008ba0: 0000 094c 6f67 5669 6577 6572 0103 0000  ...LogViewer....
-00008bb0: 000c 25b6 0020 006c 006f 0067 0073 0800  ..%.. .l.o.g.s..
-00008bc0: 0000 0006 0000 0008 e296 b620 6c6f 6773  ........... logs
-00008bd0: 0700 0000 094c 6f67 5669 6577 6572 0103  .....LogViewer..
-00008be0: 0000 003e 041e 0448 0438 0431 043a 0430  ...>...H.8.1.:.0
-00008bf0: 0020 043b 043e 0433 0438 043d 0430 0020  . .;.>.3.8.=.0. 
-00008c00: 0447 0435 0440 0435 0437 0020 0413 043e  .G.5.@.5.7. ...>
-00008c10: 0441 0443 0441 043b 0443 0433 0438 003a  .A.C.A.;.C.3.8.:
-00008c20: 0020 0800 0000 0006 0000 0013 4553 4941  . ..........ESIA
-00008c30: 206c 6f67 696e 2066 6169 6c65 643a 2007   login failed: .
-00008c40: 0000 0008 4c6f 6769 6e46 4e53 0103 0000  ....LoginFNS....
-00008c50: 0040 0423 0441 043f 0435 0448 043d 044b  .@.#.A.?.5.H.=.K
-00008c60: 0439 0020 043b 043e 0433 0438 043d 0020  .9. .;.>.3.8.=. 
-00008c70: 0447 0435 0440 0435 0437 0020 0413 043e  .G.5.@.5.7. ...>
-00008c80: 0441 0443 0441 043b 0443 0433 0438 003a  .A.C.A.;.C.3.8.:
-00008c90: 0020 0800 0000 0006 0000 0017 4553 4941  . ..........ESIA
-00008ca0: 206c 6f67 696e 2073 7563 6365 7373 6675   login successfu
-00008cb0: 6c3a 2007 0000 0008 4c6f 6769 6e46 4e53  l: .....LoginFNS
-00008cc0: 0103 0000 0038 041e 0448 0438 0431 043a  .....8...H.8.1.:
-00008cd0: 0430 0020 043b 043e 0433 0438 043d 0430  .0. .;.>.3.8.=.0
-00008ce0: 0020 0447 0435 0440 0435 0437 0020 041b  . .G.5.@.5.7. ..
-00008cf0: 041a 0020 0424 041d 0421 003a 0020 0800  ... .$...!.:. ..
-00008d00: 0000 0006 0000 0012 464e 5320 6c6f 6769  ........FNS logi
-00008d10: 6e20 6661 696c 6564 3a20 0700 0000 084c  n failed: .....L
-00008d20: 6f67 696e 464e 5301 0300 0000 3a04 2304  oginFNS.....:.#.
-00008d30: 4104 3f04 3504 4804 3d04 4b04 3900 2004  A.?.5.H.=.K.9. .
-00008d40: 3b04 3e04 3304 3804 3d00 2004 4704 3504  ;.>.3.8.=. .G.5.
-00008d50: 4004 3504 3700 2004 1b04 1a00 2004 2404  @.5.7. ..... .$.
-00008d60: 1d04 2100 3a00 2008 0000 0000 0600 0000  ..!.:. .........
-00008d70: 1646 4e53 206c 6f67 696e 2073 7563 6365  .FNS login succe
-00008d80: 7373 6675 6c3a 2007 0000 0008 4c6f 6769  ssful: .....Logi
-00008d90: 6e46 4e53 0103 0000 005a 041e 0448 0438  nFNS.....Z...H.8
-00008da0: 0431 043a 0430 0020 043f 043e 043b 0443  .1.:.0. .?.>.;.C
-00008db0: 0447 0435 043d 0438 044f 0020 0055 0052  .G.5.=.8.O. .U.R
-00008dc0: 004c 0020 043b 043e 0433 0438 043d 0430  .L. .;.>.3.8.=.0
-00008dd0: 0020 0447 0435 0440 0435 0437 0020 0413  . .G.5.@.5.7. ..
-00008de0: 043e 0441 0443 0441 043b 0443 0433 0438  .>.A.C.A.;.C.3.8
-00008df0: 003a 0020 0800 0000 0006 0000 0015 4765  .:. ..........Ge
-00008e00: 7420 4553 4941 2055 524c 2066 6169 6c65  t ESIA URL faile
-00008e10: 643a 2007 0000 0008 4c6f 6769 6e46 4e53  d: .....LoginFNS
-00008e20: 0103 0000 0034 0053 004d 0053 0020 0431  .....4.S.M.S. .1
-00008e30: 044b 043b 043e 0020 0437 0430 043f 0440  .K.;.>. .7.0.?.@
-00008e40: 043e 0448 0435 043d 043e 0020 0443 0441  .>.H.5.=.>. .C.A
-00008e50: 043f 0435 0448 043d 043e 0800 0000 0006  .?.5.H.=.>......
-00008e60: 0000 001e 534d 5320 7761 7320 7265 7175  ....SMS was requ
-00008e70: 6573 7465 6420 7375 6363 6573 7366 756c  ested successful
-00008e80: 6c79 0700 0000 084c 6f67 696e 464e 5301  ly.....LoginFNS.
-00008e90: 0300 0000 1e04 1004 3204 4204 3e04 4004  ........2.B.>.@.
-00008ea0: 3804 3704 3004 4604 3804 4f00 2004 2404  8.7.0.F.8.O. .$.
-00008eb0: 1d04 2108 0000 0000 0600 0000 1141 7574  ..!..........Aut
-00008ec0: 686f 7269 7a61 7469 6f6e 2046 4e53 0700  horization FNS..
-00008ed0: 0000 0e4c 6f67 696e 464e 5344 6961 6c6f  ...LoginFNSDialo
-00008ee0: 6701 0300 0000 0e04 1704 3004 3a04 4004  g.........0.:.@.
-00008ef0: 4b04 4204 4c08 0000 0000 0600 0000 0543  K.B.L..........C
-00008f00: 6c6f 7365 0700 0000 0e4c 6f67 696e 464e  lose.....LoginFN
-00008f10: 5344 6961 6c6f 6701 0300 0000 1604 1a04  SDialog.........
-00008f20: 3e04 3400 2004 3804 3700 2000 5300 4d00  >.4. .8.7. .S.M.
-00008f30: 5300 3a08 0000 0000 0600 0000 0e43 6f64  S.:..........Cod
-00008f40: 6520 6672 6f6d 2053 4d53 3a07 0000 000e  e from SMS:.....
-00008f50: 4c6f 6769 6e46 4e53 4469 616c 6f67 0103  LoginFNSDialog..
-00008f60: 0000 0012 0413 043e 0441 0443 0441 043b  .......>.A.C.A.;
-00008f70: 0443 0433 0438 0800 0000 0006 0000 000a  .C.3.8..........
-00008f80: 4553 4941 204c 6f67 696e 0700 0000 0e4c  ESIA Login.....L
-00008f90: 6f67 696e 464e 5344 6961 6c6f 6701 0300  oginFNSDialog...
-00008fa0: 0000 0c04 1b04 1a00 2004 2404 1d04 2108  ........ .$...!.
-00008fb0: 0000 0000 0600 0000 0946 4e53 204c 6f67  .........FNS Log
-00008fc0: 696e 0700 0000 0e4c 6f67 696e 464e 5344  in.....LoginFNSD
-00008fd0: 6961 6c6f 6701 0300 0000 0804 1804 1d04  ialog...........
-00008fe0: 1d00 3a08 0000 0000 0600 0000 0449 4e4e  ..:..........INN
-00008ff0: 3a07 0000 000e 4c6f 6769 6e46 4e53 4469  :.....LoginFNSDi
-00009000: 616c 6f67 0103 0000 000a 041b 043e 0433  alog.........>.3
-00009010: 0438 043d 0800 0000 0006 0000 0005 4c6f  .8.=..........Lo
-00009020: 6769 6e07 0000 000e 4c6f 6769 6e46 4e53  gin.....LoginFNS
-00009030: 4469 616c 6f67 0103 0000 000e 041f 0430  Dialog.........0
-00009040: 0440 043e 043b 044c 003a 0800 0000 0006  .@.>.;.L.:......
-00009050: 0000 0009 5061 7373 776f 7264 3a07 0000  ....Password:...
-00009060: 000e 4c6f 6769 6e46 4e53 4469 616c 6f67  ..LoginFNSDialog
-00009070: 0103 0000 001e 041d 043e 043c 0435 0440  .........>.<.5.@
-00009080: 0020 0442 0435 043b 0435 0444 043e 043d  . .B.5.;.5.D.>.=
-00009090: 0430 003a 0800 0000 0006 0000 000d 5068  .0.:..........Ph
-000090a0: 6f6e 6520 6e75 6d62 6572 3a07 0000 000e  one number:.....
-000090b0: 4c6f 6769 6e46 4e53 4469 616c 6f67 0103  LoginFNSDialog..
-000090c0: 0000 0006 0053 004d 0053 0800 0000 0006  .....S.M.S......
-000090d0: 0000 0009 534d 5320 4c6f 6769 6e07 0000  ....SMS Login...
-000090e0: 000e 4c6f 6769 6e46 4e53 4469 616c 6f67  ..LoginFNSDialog
-000090f0: 0103 0000 0026 0412 044b 0441 043b 0430  .....&...K.A.;.0
-00009100: 0442 044c 0020 0053 004d 0053 0020 0441  .B.L. .S.M.S. .A
-00009110: 0020 043a 043e 0434 043e 043c 0800 0000  . .:.>.4.>.<....
-00009120: 0006 0000 0012 5365 6e64 2053 4d53 2077  ......Send SMS w
-00009130: 6974 6820 636f 6465 0700 0000 0e4c 6f67  ith code.....Log
-00009140: 696e 464e 5344 6961 6c6f 6701 0300 0000  inFNSDialog.....
-00009150: 1600 6100 6200 6f00 7500 7400 3a00 6200  ..a.b.o.u.t.:.b.
-00009160: 6c00 6100 6e00 6b08 0000 0000 0600 0000  l.a.n.k.........
-00009170: 0b61 626f 7574 3a62 6c61 6e6b 0700 0000  .about:blank....
-00009180: 0e4c 6f67 696e 464e 5344 6961 6c6f 6701  .LoginFNSDialog.
-00009190: 0300 0000 4404 1d04 3004 3904 3404 3504  ....D...0.9.4.5.
-000091a0: 3d04 3e00 2004 3d04 3504 4104 3a04 3e04  =.>. .=.5.A.:.>.
-000091b0: 3b04 4c04 3a04 3e00 2004 2604 1100 2004  ;.L.:.>. .&... .
-000091c0: 3d04 3000 2000 4d00 4f00 4500 5800 2004  =.0. .M.O.E.X. .
-000091d0: 3404 3b04 4f00 3a00 2008 0000 0000 0600  4.;.O.:. .......
-000091e0: 0000 204d 756c 7469 706c 6520 4d4f 4558  .. Multiple MOEX
-000091f0: 2061 7373 6574 7320 666f 756e 6420 666f   assets found fo
-00009200: 723a 2007 0000 0004 4d4f 4558 0103 0000  r: .....MOEX....
-00009210: 0044 041d 0435 043f 043e 0434 0434 0435  .D...5.?.>.4.4.5
-00009220: 0440 0436 0438 0432 0430 0435 043c 044b  .@.6.8.2.0.5.<.K
-00009230: 0439 0020 0442 0438 043f 0020 0426 0411  .9. .B.8.?. .&..
-00009240: 0020 041c 043e 0441 0411 0438 0440 0436  . ...>.A...8.@.6
-00009250: 0438 003a 0020 0800 0000 0006 0000 0020  .8.:. ......... 
-00009260: 556e 7375 7070 6f72 7465 6420 4d4f 4558  Unsupported MOEX
-00009270: 2073 6563 7572 6974 7920 7479 7065 3a20   security type: 
-00009280: 0700 0000 044d 4f45 5801 0300 0000 1604  .....MOEX.......
-00009290: 1e00 2004 3f04 4004 3e04 3304 4004 3004  .. .?.@.>.3.@.0.
-000092a0: 3c04 3c04 3508 0000 0000 0600 0000 0541  <.<.5..........A
-000092b0: 626f 7574 0700 0000 0a4d 6169 6e57 696e  bout.....MainWin
-000092c0: 646f 7701 0300 0000 1a04 1f04 3e04 3404  dow.........>.4.
-000092d0: 4204 3204 3504 4004 3604 3404 3504 3d04  B.2.5.@.6.4.5.=.
-000092e0: 3804 3508 0000 0000 0600 0000 0c43 6f6e  8.5..........Con
-000092f0: 6669 726d 6174 696f 6e07 0000 000a 4d61  firmation.....Ma
-00009300: 696e 5769 6e64 6f77 0103 0000 0014 0418  inWindow........
-00009310: 043d 0444 043e 0440 043c 0430 0446 0438  .=.D.>.@.<.0.F.8
-00009320: 044f 0800 0000 0006 0000 0004 496e 666f  .O..........Info
-00009330: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-00009340: 0300 0000 2804 2f04 3704 4b04 3a00 2004  ....(./.7.K.:. .
-00009350: 3104 4b04 3b00 2004 3804 3704 3c04 3504  1.K.;. .8.7.<.5.
-00009360: 3d04 5104 3d00 2004 3d04 3000 2008 0000  =.Q.=. .=.0. ...
-00009370: 0000 0600 0000 184c 616e 6775 6167 6520  .......Language 
-00009380: 7761 7320 6368 616e 6765 6420 746f 2007  was changed to .
-00009390: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
-000093a0: 0000 0062 0418 0442 043e 0433 0438 0020  ...b...B.>.3.8. 
-000093b0: 0442 0440 0430 043d 0437 0430 043a 0446  .B.@.0.=.7.0.:.F
-000093c0: 0438 0439 0020 043d 0435 0430 043a 0442  .8.9. .=.5.0.:.B
-000093d0: 0443 0430 043b 044c 043d 044b 002e 0020  .C.0.;.L.=.K... 
-000093e0: 041f 0435 0440 0435 0441 0447 0438 0442  ...5.@.5.A.G.8.B
-000093f0: 0430 0442 044c 0020 0441 0435 0439 0447  .0.B.L. .A.5.9.G
-00009400: 0430 0441 003f 0800 0000 0006 0000 0026  .0.A.?.........&
-00009410: 4c65 6467 6572 2069 736e 2774 2063 6f6d  Ledger isn't com
-00009420: 706c 6574 652e 2052 6562 7569 6c64 2069  plete. Rebuild i
-00009430: 7420 6e6f 773f 0700 0000 0a4d 6169 6e57  t now?.....MainW
-00009440: 696e 646f 7701 0300 0000 8004 1404 3e04  indow.........>.
-00009450: 3f04 3e04 3b04 3d04 3804 4204 3504 3b04  ?.>.;.=.8.B.5.;.
-00009460: 4c04 3d04 3004 4f00 2004 3804 3d04 4404  L.=.0.O. .8.=.D.
-00009470: 3e04 4004 3c04 3004 4604 3804 4f00 2c00  >.@.<.0.F.8.O.,.
-00009480: 2004 3804 3d04 4104 4204 4004 4304 3a04   .8.=.A.B.@.C.:.
-00009490: 4604 3804 3800 2c00 2004 4104 3e04 3e04  F.8.8.,. .A.>.>.
-000094a0: 3104 4904 3504 3d04 3804 4f00 2004 3e00  1.I.5.=.8.O. .>.
-000094b0: 2004 3f04 4004 3e04 3104 3b04 3504 3c04   .?.@.>.1.;.5.<.
-000094c0: 3004 4500 2004 3d04 3000 2008 0000 0000  0.E. .=.0. .....
-000094d0: 0600 0000 354d 6f72 6520 696e 666f 726d  ....5More inform
-000094e0: 6174 696f 6e2c 206d 616e 7561 6c73 2061  ation, manuals a
-000094f0: 6e64 2070 726f 626c 656d 2072 6570 6f72  nd problem repor
-00009500: 7473 2061 7265 2061 7420 0700 0000 0a4d  ts are at .....M
-00009510: 6169 6e57 696e 646f 7701 0300 0000 5004  ainWindow.....P.
-00009520: 1204 3e04 3f04 4004 3e04 4104 4b00 2c00  ..>.?.@.>.A.K.,.
-00009530: 2004 3a04 3e04 3c04 3c04 3504 3d04 4204   .:.>.<.<.5.=.B.
-00009540: 3004 4004 3804 3800 2c00 2004 3f04 3e04  0.@.8.8.,. .?.>.
-00009550: 3c04 3e04 4904 4c00 2004 3804 3b04 3800  <.>.I.L. .8.;.8.
-00009560: 2004 3404 3e04 3d04 3004 4204 4b00 3a08   .4.>.=.0.B.K.:.
-00009570: 0000 0000 0600 0000 2751 7565 7374 696f  ........'Questio
-00009580: 6e73 2c20 636f 6d6d 656e 7473 2c20 6865  ns, comments, he
-00009590: 6c70 206f 7220 646f 6e61 7469 6f6e 733a  lp or donations:
-000095a0: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-000095b0: 0300 0000 2204 2204 4004 3504 3104 4304  ....".".@.5.1.C.
-000095c0: 3504 4204 4104 4f00 2004 4004 3504 4104  5.B.A.O. .@.5.A.
-000095d0: 4204 3004 4004 4208 0000 0000 0600 0000  B.0.@.B.........
-000095e0: 1052 6573 7461 7274 2072 6571 7569 7265  .Restart require
-000095f0: 6407 0000 000a 4d61 696e 5769 6e64 6f77  d.....MainWindow
-00009600: 0103 0000 0050 041a 043e 043d 0435 0447  .....P...>.=.5.G
-00009610: 043d 044b 0439 0020 0431 0430 043b 0430  .=.K.9. .1.0.;.0
-00009620: 043d 0441 0020 043f 043e 0020 043e 0442  .=.A. .?.>. .>.B
-00009630: 0447 0451 0442 0443 0020 043d 0435 0020  .G.Q.B.C. .=.5. 
-00009640: 0441 043e 0432 043f 0430 0434 0430 0435  .A.>.2.?.0.4.0.5
-00009650: 0442 003a 0020 0800 0000 0006 0000 0028  .B.:. .........(
-00009660: 5374 6174 656d 656e 7420 656e 6469 6e67  Statement ending
-00009670: 2062 616c 616e 6365 2064 6f65 736e 2774   balance doesn't
-00009680: 206d 6174 6368 3a20 0700 0000 0a4d 6169   match: .....Mai
-00009690: 6e57 696e 646f 7701 0300 0000 c804 1204  nWindow.........
-000096a0: 4b00 2004 3404 3e04 3b04 3604 3d04 4b00  K. .4.>.;.6.=.K.
-000096b0: 2004 3f04 3504 4004 3504 3704 3004 3f04   .?.5.@.5.7.0.?.
-000096c0: 4304 4104 4204 3804 4204 4c00 2004 3f04  C.A.B.8.B.L. .?.
-000096d0: 4004 3804 3b04 3e04 3604 3504 3d04 3804  @.8.;.>.6.5.=.8.
-000096e0: 3500 2c00 2004 4704 4204 3e04 3104 4b00  5.,. .G.B.>.1.K.
-000096f0: 2004 3f04 4004 3804 3c04 3504 3d04 3804   .?.@.8.<.5.=.8.
-00009700: 4204 4c00 2004 3804 3704 3c04 3504 3d04  B.L. .8.7.<.5.=.
-00009710: 3504 3d04 3804 4f00 0a04 1f04 4004 3804  5.=.8.O.....@.8.
-00009720: 3b04 3e04 3604 3504 3d04 3804 3500 2004  ;.>.6.5.=.8.5. .
-00009730: 4104 3504 3904 4704 3004 4100 2004 3704  A.5.9.G.0.A. .7.
-00009740: 3004 3204 3504 4004 4804 3804 4200 2004  0.2.5.@.H.8.B. .
-00009750: 4104 3204 3e04 4e00 2004 4004 3004 3104  A.2.>.N. .@.0.1.
-00009760: 3e04 4204 4308 0000 0000 0600 0000 5259  >.B.C.........RY
-00009770: 6f75 2073 686f 756c 6420 7265 7374 6172  ou should restar
-00009780: 7420 6170 706c 6963 6174 696f 6e20 746f  t application to
-00009790: 2061 7070 6c79 2063 6861 6e67 6573 0a41   apply changes.A
-000097a0: 7070 6c69 6361 7469 6f6e 2077 696c 6c20  pplication will 
-000097b0: 6265 2074 6572 6d69 6e61 7465 6420 6e6f  be terminated no
-000097c0: 7707 0000 000a 4d61 696e 5769 6e64 6f77  w.....MainWindow
-000097d0: 0103 0000 0030 0434 043e 043c 0430 0448  .....0.4.>.<.0.H
-000097e0: 043d 0435 0439 0020 0441 0442 0440 0430  .=.5.9. .A.B.@.0
-000097f0: 043d 0438 0446 0435 0020 0067 0069 0074  .=.8.F.5. .g.i.t
-00009800: 0068 0075 0062 0800 0000 0006 0000 0010  .h.u.b..........
-00009810: 6769 7468 7562 2068 6f6d 6520 7061 6765  github home page
-00009820: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-00009830: 0300 0000 0c04 3204 3504 4004 4104 3804  ......2.5.@.A.8.
-00009840: 4f08 0000 0000 0600 0000 0776 6572 7369  O..........versi
-00009850: 6f6e 0700 0000 0a4d 6169 6e57 696e 646f  on.....MainWindo
-00009860: 7701 0300 0000 0600 2e00 2e00 2e08 0000  w...............
-00009870: 0000 0600 0000 032e 2e2e 0700 0000 0f4d  ...............M
-00009880: 6f6e 6579 466c 6f77 5769 6467 6574 0103  oneyFlowWidget..
-00009890: 0000 0016 0424 0430 0439 043b 0020 0045  .....$.0.9.;. .E
-000098a0: 0078 0063 0065 006c 003a 0800 0000 0006  .x.c.e.l.:......
-000098b0: 0000 000b 4578 6365 6c20 6669 6c65 3a07  ....Excel file:.
-000098c0: 0000 000f 4d6f 6e65 7946 6c6f 7757 6964  ....MoneyFlowWid
-000098d0: 6765 7401 0300 0000 2804 2404 3004 3904  get.....(.$.0.9.
-000098e0: 3b04 4b00 2000 4500 7800 6300 6500 6c00  ;.K. .E.x.c.e.l.
-000098f0: 2000 2800 2a00 2e00 7800 7300 6c00 7800   .(.*...x.s.l.x.
-00009900: 2908 0000 0000 0600 0000 1445 7863 656c  )..........Excel
-00009910: 2066 696c 6573 2028 2a2e 786c 7378 2907   files (*.xlsx).
-00009920: 0000 000f 4d6f 6e65 7946 6c6f 7757 6964  ....MoneyFlowWid
-00009930: 6765 7401 0300 0000 5604 2404 3004 3904  get.....V.$.0.9.
-00009940: 3b00 2004 3404 3b04 4f00 2004 4104 3e04  ;. .4.;.O. .A.>.
-00009950: 4504 4004 3004 3d04 3504 3d04 3804 4f00  E.@.0.=.5.=.8.O.
-00009960: 2004 4004 3004 4104 4704 5104 4204 3000   .@.0.A.G.Q.B.0.
-00009970: 2004 3200 2004 4404 3e04 4004 3c04 3004   .2. .D.>.@.<.0.
-00009980: 4204 3500 2000 4500 7800 6300 6500 6c08  B.5. .E.x.c.e.l.
-00009990: 0000 0000 0600 0000 2e46 696c 6520 7768  .........File wh
-000099a0: 6572 6520 746f 2073 746f 7265 2074 6178  ere to store tax
-000099b0: 2072 6570 6f72 7420 696e 2045 7863 656c   report in Excel
-000099c0: 2066 6f72 6d61 7407 0000 000f 4d6f 6e65   format.....Mone
-000099d0: 7946 6c6f 7757 6964 6765 7401 0300 0000  yFlowWidget.....
-000099e0: 0a04 1e04 3e04 1404 1404 2108 0000 0000  ....>.....!.....
-000099f0: 0600 0000 0a4d 6f6e 6579 2046 6c6f 7707  .....Money Flow.
-00009a00: 0000 000f 4d6f 6e65 7946 6c6f 7757 6964  ....MoneyFlowWid
-00009a10: 6765 7401 0300 0000 2e04 1e04 3e04 1404  get.........>...
-00009a20: 1404 2100 2004 4104 3e04 4504 4004 3004  ..!. .A.>.E.@.0.
-00009a30: 3d04 5104 3d00 2004 3200 2004 4404 3004  =.Q.=. .2. .D.0.
-00009a40: 3904 3b04 3500 2008 0000 0000 0600 0000  9.;.5. .........
-00009a50: 204d 6f6e 6579 2066 6c6f 7720 7265 706f   Money flow repo
-00009a60: 7274 2073 6176 6564 2074 6f20 6669 6c65  rt saved to file
-00009a70: 2007 0000 000f 4d6f 6e65 7946 6c6f 7757   .....MoneyFlowW
-00009a80: 6964 6765 7401 0300 0000 1e04 2104 3e04  idget.......!.>.
-00009a90: 4504 4004 3004 3d04 3804 4204 4c00 2004  E.@.0.=.8.B.L. .
-00009aa0: 1e04 4204 4704 5104 4208 0000 0000 0600  ..B.G.Q.B.......
-00009ab0: 0000 0b53 6176 6520 5265 706f 7274 0700  ...Save Report..
-00009ac0: 0000 0f4d 6f6e 6579 466c 6f77 5769 6467  ...MoneyFlowWidg
-00009ad0: 6574 0103 0000 0024 0421 043e 0445 0440  et.....$.!.>.E.@
-00009ae0: 0430 043d 0438 0442 044c 0020 041e 043e  .0.=.8.B.L. ...>
-00009af0: 0414 0414 0421 0020 0432 003a 0800 0000  .....!. .2.:....
-00009b00: 0006 0000 001a 5361 7665 206d 6f6e 6579  ......Save money
-00009b10: 2066 6c6f 7720 7265 706f 7274 2074 6f3a   flow report to:
-00009b20: 0700 0000 0f4d 6f6e 6579 466c 6f77 5769  .....MoneyFlowWi
-00009b30: 6467 6574 0103 0000 0018 0412 044b 0431  dget.........K.1
-00009b40: 0435 0440 0438 0442 0020 0444 0430 0439  .5.@.8.B. .D.0.9
-00009b50: 043b 0800 0000 0006 0000 000b 5365 6c65  .;..........Sele
-00009b60: 6374 2066 696c 6507 0000 000f 4d6f 6e65  ct file.....Mone
-00009b70: 7946 6c6f 7757 6964 6765 7401 0300 0000  yFlowWidget.....
-00009b80: 0804 1304 3e04 3400 3a08 0000 0000 0600  ....>.4.:.......
-00009b90: 0000 0559 6561 723a 0700 0000 0f4d 6f6e  ...Year:.....Mon
-00009ba0: 6579 466c 6f77 5769 6467 6574 0103 0000  eyFlowWidget....
-00009bb0: 0028 0020 043d 0435 0443 0441 043f 0435  .(. .=.5.C.A.?.5
-00009bc0: 0448 043d 044b 0439 0020 0437 0430 043f  .H.=.K.9. .7.0.?
-00009bd0: 0440 043e 0441 003a 0020 0800 0000 0006  .@.>.A.:. ......
-00009be0: 0000 0009 2066 6169 6c65 643a 2007 0000  .... failed: ...
-00009bf0: 0003 4e65 7401 0300 0000 3404 2204 3804  ..Net.....4.".8.
-00009c00: 3f00 2004 2604 1100 2004 3d04 3500 2004  ?. .&... .=.5. .
-00009c10: 3f04 3e04 3404 3404 3504 4004 3604 3804  ?.>.4.4.5.@.6.8.
-00009c20: 3204 3004 3504 4204 4104 4f00 3a00 2008  2.0.5.B.A.O.:. .
-00009c30: 0000 0000 0600 0000 1c41 7373 6574 2074  .........Asset t
-00009c40: 7970 6520 6973 6e27 7420 7375 7070 6f72  ype isn't suppor
-00009c50: 7465 643a 2007 0000 000a 4f70 656e 4272  ted: .....OpenBr
-00009c60: 6f6b 6572 0103 0000 0032 0411 0438 0440  oker.....2...8.@
-00009c70: 0436 0430 0020 043d 0435 0020 043f 043e  .6.0. .=.5. .?.>
-00009c80: 0434 0434 0435 0440 0436 0438 0432 0430  .4.4.5.@.6.8.2.0
-00009c90: 0435 0442 0441 044f 003a 0020 0800 0000  .5.B.A.O.:. ....
-00009ca0: 0006 0000 001a 4578 6368 616e 6765 2069  ......Exchange i
-00009cb0: 736e 2774 2073 7570 706f 7274 6564 3a20  sn't supported: 
-00009cc0: 0700 0000 0a4f 7065 6e42 726f 6b65 7201  .....OpenBroker.
-00009cd0: 0300 0000 0804 2104 4704 3504 4208 0000  ......!.G.5.B...
-00009ce0: 0000 0600 0000 0741 6363 6f75 6e74 0700  .......Account..
-00009cf0: 0000 0f4f 7065 7261 7469 6f6e 734d 6f64  ...OperationsMod
-00009d00: 656c 0103 0000 000a 0421 0443 043c 043c  el.......!.C.<.<
-00009d10: 0430 0800 0000 0006 0000 0006 416d 6f75  .0..........Amou
-00009d20: 6e74 0700 0000 0f4f 7065 7261 7469 6f6e  nt.....Operation
-00009d30: 734d 6f64 656c 0103 0000 000c 0411 0430  sModel.........0
-00009d40: 043b 0430 043d 0441 0800 0000 0006 0000  .;.0.=.A........
-00009d50: 0007 4261 6c61 6e63 6507 0000 000f 4f70  ..Balance.....Op
-00009d60: 6572 6174 696f 6e73 4d6f 6465 6c01 0300  erationsModel...
-00009d70: 0000 0c04 1204 3004 3b04 4e04 4204 3008  ......0.;.N.B.0.
-00009d80: 0000 0000 0600 0000 0843 7572 7265 6e63  .........Currenc
-00009d90: 7907 0000 000f 4f70 6572 6174 696f 6e73  y.....Operations
-00009da0: 4d6f 6465 6c01 0300 0000 1004 1e04 3f04  Model.........?.
-00009db0: 3804 4104 3004 3d04 3804 3508 0000 0000  8.A.0.=.8.5.....
-00009dc0: 0600 0000 054e 6f74 6573 0700 0000 0f4f  .....Notes.....O
-00009dd0: 7065 7261 7469 6f6e 734d 6f64 656c 0103  perationsModel..
-00009de0: 0000 0014 0414 0430 0442 0430 002f 0412  .......0.B.0./..
-00009df0: 0440 0435 043c 044f 0800 0000 0006 0000  .@.5.<.O........
-00009e00: 0009 5469 6d65 7374 616d 7007 0000 000f  ..Timestamp.....
-00009e10: 4f70 6572 6174 696f 6e73 4d6f 6465 6c01  OperationsModel.
-00009e20: 0300 0000 0a04 2104 4704 3504 4200 3a08  ......!.G.5.B.:.
-00009e30: 0000 0000 0600 0000 0841 6363 6f75 6e74  .........Account
-00009e40: 3a07 0000 0010 4f70 6572 6174 696f 6e73  :.....Operations
-00009e50: 5769 6467 6574 0103 0000 004a 0412 044b  Widget.....J...K
-00009e60: 0020 0445 043e 0442 0438 0442 0435 0020  . .E.>.B.8.B.5. 
-00009e70: 0443 0434 0430 043b 0438 0442 044c 0020  .C.4.0.;.8.B.L. 
-00009e80: 0432 044b 0431 0440 0430 043d 043d 044b  .2.K.1.@.0.=.=.K
-00009e90: 0435 0020 043e 043f 0435 0440 0430 0446  .5. .>.?.5.@.0.F
-00009ea0: 0438 0438 003f 0800 0000 0006 0000 002e  .8.8.?..........
-00009eb0: 4172 6520 796f 7520 7375 7265 2074 6f20  Are you sure to 
-00009ec0: 6465 6c65 7465 2073 656c 6563 7465 6420  delete selected 
-00009ed0: 7472 616e 7361 6369 6f6e 2873 293f 0700  transacion(s)?..
-00009ee0: 0000 104f 7065 7261 7469 6f6e 7357 6964  ...OperationsWid
-00009ef0: 6765 7401 0300 0000 1c04 1104 3004 3b04  get.........0.;.
-00009f00: 3004 3d04 4104 4b00 2004 4104 4704 3504  0.=.A.K. .A.G.5.
-00009f10: 4204 3e04 3208 0000 0000 0600 0000 0842  B.>.2..........B
-00009f20: 616c 616e 6365 7307 0000 0010 4f70 6572  alances.....Oper
-00009f30: 6174 696f 6e73 5769 6467 6574 0103 0000  ationsWidget....
-00009f40: 001a 041f 043e 0434 0442 0432 0435 0440  .....>.4.B.2.5.@
-00009f50: 0436 0434 0435 043d 0438 0435 0800 0000  .6.4.5.=.8.5....
-00009f60: 0006 0000 000c 436f 6e66 6972 6d61 7469  ......Confirmati
-00009f70: 6f6e 0700 0000 104f 7065 7261 7469 6f6e  on.....Operation
-00009f80: 7357 6964 6765 7401 0300 0000 1404 1a04  sWidget.........
-00009f90: 3e04 3f04 3804 4004 3e04 3204 3004 4204  >.?.8.@.>.2.0.B.
-00009fa0: 4c08 0000 0000 0600 0000 0443 6f70 7907  L..........Copy.
-00009fb0: 0000 0010 4f70 6572 6174 696f 6e73 5769  ....OperationsWi
-00009fc0: 6467 6574 0103 0000 0026 041a 043e 043f  dget.....&...>.?
-00009fd0: 0438 0440 043e 0432 0430 0442 044c 0020  .8.@.>.2.0.B.L. 
-00009fe0: 043e 043f 0435 0440 0430 0446 0438 044e  .>.?.5.@.0.F.8.N
-00009ff0: 0800 0000 0006 0000 000e 436f 7079 206f  ..........Copy o
-0000a000: 7065 7261 7469 6f6e 0700 0000 104f 7065  peration.....Ope
-0000a010: 7261 7469 6f6e 7357 6964 6765 7401 0300  rationsWidget...
-0000a020: 0000 0e04 2304 3404 3004 3b04 3804 4204  ....#.4.0.;.8.B.
-0000a030: 4c08 0000 0000 0600 0000 0644 656c 6574  L..........Delet
-0000a040: 6507 0000 0010 4f70 6572 6174 696f 6e73  e.....Operations
-0000a050: 5769 6467 6574 0103 0000 0020 0423 0434  Widget..... .#.4
-0000a060: 0430 043b 0438 0442 044c 0020 043e 043f  .0.;.8.B.L. .>.?
-0000a070: 0435 0440 0430 0446 0438 044e 0800 0000  .5.@.0.F.8.N....
-0000a080: 0006 0000 0010 4465 6c65 7465 206f 7065  ......Delete ope
-0000a090: 7261 7469 6f6e 0700 0000 104f 7065 7261  ration.....Opera
-0000a0a0: 7469 6f6e 7357 6964 6765 7401 0300 0000  tionsWidget.....
-0000a0b0: 1c04 1d04 3e04 3204 3004 4f00 2004 3e04  ....>.2.0.O. .>.
-0000a0c0: 3f04 3504 4004 3004 4604 3804 4f08 0000  ?.5.@.0.F.8.O...
-0000a0d0: 0000 0600 0000 0d4e 6577 206f 7065 7261  .......New opera
-0000a0e0: 7469 6f6e 0700 0000 104f 7065 7261 7469  tion.....Operati
-0000a0f0: 6f6e 7357 6964 6765 7401 0300 0000 1004  onsWidget.......
-0000a100: 1e04 3f04 3504 4004 3004 4604 3804 3808  ..?.5.@.0.F.8.8.
-0000a110: 0000 0000 0600 0000 0a4f 7065 7261 7469  .........Operati
-0000a120: 6f6e 7307 0000 0010 4f70 6572 6174 696f  ons.....Operatio
-0000a130: 6e73 5769 6467 6574 0103 0000 0024 041e  nsWidget.....$..
-0000a140: 043f 0435 0440 0430 0446 0438 0438 0020  .?.5.@.0.F.8.8. 
-0000a150: 0438 0020 0411 0430 043b 0430 043d 0441  .8. ...0.;.0.=.A
-0000a160: 044b 0800 0000 0006 0000 0015 4f70 6572  .K..........Oper
-0000a170: 6174 696f 6e73 2026 2042 616c 616e 6365  ations & Balance
-0000a180: 7307 0000 0010 4f70 6572 6174 696f 6e73  s.....Operations
-0000a190: 5769 6467 6574 0103 0000 000e 0421 0432  Widget.......!.2
-0000a1a0: 0435 0440 0438 0442 044c 0800 0000 0006  .5.@.8.B.L......
-0000a1b0: 0000 0009 5265 636f 6e63 696c 6507 0000  ....Reconcile...
-0000a1c0: 0010 4f70 6572 6174 696f 6e73 5769 6467  ..OperationsWidg
-0000a1d0: 6574 0103 0000 000c 041f 043e 0438 0441  et.........>.8.A
-0000a1e0: 043a 003a 0800 0000 0006 0000 0007 5365  .:.:..........Se
-0000a1f0: 6172 6368 3a07 0000 0010 4f70 6572 6174  arch:.....Operat
-0000a200: 696f 6e73 5769 6467 6574 0103 0000 002c  ionsWidget.....,
-0000a210: 041f 043e 043a 0430 0437 044b 0432 0430  ...>.:.0.7.K.2.0
-0000a220: 0442 044c 0020 0026 043d 0435 0430 043a  .B.L. .&.=.5.0.:
-0000a230: 0442 0438 0432 043d 044b 0435 0800 0000  .B.8.2.=.K.5....
-0000a240: 0006 0000 000e 5368 6f77 2026 496e 6163  ......Show &Inac
-0000a250: 7469 7665 0700 0000 104f 7065 7261 7469  tive.....Operati
-0000a260: 6f6e 7357 6964 6765 7401 0300 0000 1a04  onsWidget.......
-0000a270: 1204 3004 3b04 4e04 4204 3000 2004 3804  ..0.;.N.B.0. .8.
-0000a280: 4204 3e04 3304 3e00 3a08 0000 0000 0600  B.>.3.>.:.......
-0000a290: 0000 0d53 756d 2043 7572 7265 6e63 793a  ...Sum Currency:
-0000a2a0: 0700 0000 104f 7065 7261 7469 6f6e 7357  .....OperationsW
-0000a2b0: 6964 6765 7401 0300 0000 1400 6400 6400  idget.......d.d.
-0000a2c0: 2f00 4d00 4d00 2f00 7900 7900 7900 7908  /.M.M./.y.y.y.y.
-0000a2d0: 0000 0000 0600 0000 0a64 642f 4d4d 2f79  .........dd/MM/y
-0000a2e0: 7979 7907 0000 0010 4f70 6572 6174 696f  yyy.....Operatio
-0000a2f0: 6e73 5769 6467 6574 0103 0000 000c 0412  nsWidget........
-0000a300: 0430 043b 044e 0442 0430 0800 0000 0006  .0.;.N.B.0......
-0000a310: 0000 0008 4375 7272 656e 6379 0700 0000  ....Currency....
-0000a320: 184f 7074 696f 6e61 6c43 7572 7265 6e63  .OptionalCurrenc
-0000a330: 7943 6f6d 626f 426f 7801 0300 0000 0a04  yComboBox.......
-0000a340: 2104 4304 3c04 3c04 3008 0000 0000 0600  !.C.<.<.0.......
-0000a350: 0000 0641 6d6f 756e 7407 0000 0010 5061  ...Amount.....Pa
-0000a360: 6e64 6173 4c69 6e65 734d 6f64 656c 0103  ndasLinesModel..
-0000a370: 0000 0012 041a 0430 0442 0435 0433 043e  .......0.B.5.3.>
-0000a380: 0440 0438 044f 0800 0000 0006 0000 0008  .@.8.O..........
-0000a390: 4361 7465 676f 7279 0700 0000 1050 616e  Category.....Pan
-0000a3a0: 6461 734c 696e 6573 4d6f 6465 6c01 0300  dasLinesModel...
-0000a3b0: 0000 2204 1d04 3004 3704 3204 3004 3d04  .."...0.7.2.0.=.
-0000a3c0: 3804 3500 2004 3f04 4004 3e04 3404 4304  8.5. .?.@.>.4.C.
-0000a3d0: 3a04 4204 3008 0000 0000 0600 0000 0c50  :.B.0..........P
-0000a3e0: 726f 6475 6374 206e 616d 6507 0000 0010  roduct name.....
-0000a3f0: 5061 6e64 6173 4c69 6e65 734d 6f64 656c  PandasLinesModel
-0000a400: 0103 0000 0006 0422 044d 0433 0800 0000  .......".M.3....
-0000a410: 0006 0000 0003 5461 6707 0000 0010 5061  ......Tag.....Pa
-0000a420: 6e64 6173 4c69 6e65 734d 6f64 656c 0103  ndasLinesModel..
-0000a430: 0000 0024 0027 0020 0437 0430 043c 0435  ...$.'. .7.0.<.5
-0000a440: 043d 0435 043d 0430 0020 0443 0441 043f  .=.5.=.0. .C.A.?
-0000a450: 0435 0448 043d 043e 0800 0000 0006 0000  .5.H.=.>........
-0000a460: 001b 2720 7761 7320 7375 6363 6573 7366  ..' was successf
-0000a470: 756c 6c79 2072 6570 6c61 6365 6407 0000  ully replaced...
-0000a480: 000e 5065 6572 4c69 7374 4469 616c 6f67  ..PeerListDialog
-0000a490: 0103 0000 000c 0027 0020 043d 0430 003a  .......'. .=.0.:
-0000a4a0: 0020 0800 0000 0006 0000 0008 2720 7769  . ..........' wi
-0000a4b0: 7468 3a20 0700 0000 0e50 6565 724c 6973  th: .....PeerLis
-0000a4c0: 7444 6961 6c6f 6701 0300 0000 4e04 2104  tDialog.....N.!.
-0000a4d0: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
-0000a4e0: 2004 4104 4204 3004 4004 3e04 3500 2004   .A.B.0.@.>.5. .
-0000a4f0: 3d04 3004 3704 3204 3004 3d04 3804 3500  =.0.7.2.0.=.8.5.
-0000a500: 2004 3200 2004 3f04 4004 3804 3c04 3504   .2. .?.@.8.<.5.
-0000a510: 4704 3004 3d04 3804 3800 3f08 0000 0000  G.0.=.8.8.?.....
-0000a520: 0600 0000 174b 6565 7020 6f6c 6420 6e61  .....Keep old na
-0000a530: 6d65 2069 6e20 6e6f 7465 733f 0700 0000  me in notes?....
-0000a540: 0e50 6565 724c 6973 7444 6961 6c6f 6701  .PeerListDialog.
-0000a550: 0300 0000 1804 1a04 3e04 3d04 4204 4004  ........>.=.B.@.
-0000a560: 3004 3304 3504 3d04 4200 2000 2708 0000  0.3.5.=.B. .'...
-0000a570: 0000 0600 0000 0650 6565 7220 2707 0000  .......Peer '...
-0000a580: 000e 5065 6572 4c69 7374 4469 616c 6f67  ..PeerListDialog
-0000a590: 0103 0000 0016 041a 043e 043d 0442 0440  .........>.=.B.@
-0000a5a0: 0430 0433 0435 043d 0442 044b 0800 0000  .0.3.5.=.B.K....
-0000a5b0: 0006 0000 0005 5065 6572 7307 0000 000e  ......Peers.....
-0000a5c0: 5065 6572 4c69 7374 4469 616c 6f67 0103  PeerListDialog..
-0000a5d0: 0000 002c 0417 0430 043c 0435 043d 0438  ...,...0.<.5.=.8
-0000a5e0: 0442 044c 0020 043a 043e 043d 0442 0440  .B.L. .:.>.=.B.@
-0000a5f0: 0430 0433 0435 043d 0442 0430 0020 0027  .0.3.5.=.B.0. .'
-0000a600: 0800 0000 0006 0000 000e 5265 706c 6163  ..........Replac
-0000a610: 6520 7065 6572 2027 0700 0000 0e50 6565  e peer '.....Pee
-0000a620: 724c 6973 7444 6961 6c6f 6701 0300 0000  rListDialog.....
-0000a630: 1c04 1704 3004 3c04 3504 3d04 3804 4204  ....0.<.5.=.8.B.
-0000a640: 4c00 2004 3d04 3000 2e00 2e00 2e08 0000  L. .=.0.........
-0000a650: 0000 0600 0000 0f52 6570 6c61 6365 2077  .......Replace w
-0000a660: 6974 682e 2e2e 0700 0000 0e50 6565 724c  ith........PeerL
-0000a670: 6973 7444 6961 6c6f 6701 0300 0000 4004  istDialog.....@.
-0000a680: 1f04 3e04 3a04 3004 3704 3004 4204 4c00  ..>.:.0.7.0.B.L.
-0000a690: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
-0000a6a0: 3800 2004 4100 2004 1a04 3e04 3d04 4204  8. .A. ...>.=.B.
-0000a6b0: 4004 3004 3304 3504 3d04 4204 3e04 3c08  @.0.3.5.=.B.>.<.
-0000a6c0: 0000 0000 0600 0000 1953 686f 7720 6f70  .........Show op
-0000a6d0: 6572 6174 696f 6e73 2077 6974 6820 5065  erations with Pe
-0000a6e0: 6572 0700 0000 0e50 6565 724c 6973 7444  er.....PeerListD
-0000a6f0: 6961 6c6f 6701 0300 0000 1004 1e04 3f04  ialog.........?.
-0000a700: 3504 4004 3004 4604 3804 3808 0000 0000  5.@.0.F.8.8.....
-0000a710: 0600 0000 0a4f 7065 7261 7469 6f6e 7307  .....Operations.
-0000a720: 0000 000a 5065 6572 5265 706f 7274 0103  ....PeerReport..
-0000a730: 0000 001c 043f 043e 0020 041a 043e 043d  .....?.>. ...>.=
-0000a740: 0442 0440 0430 0433 0435 043d 0442 0443  .B.@.0.3.5.=.B.C
-0000a750: 0800 0000 0006 0000 0007 6279 2050 6565  ..........by Pee
-0000a760: 7207 0000 000a 5065 6572 5265 706f 7274  r.....PeerReport
-0000a770: 0103 0000 0016 041a 043e 043d 0442 0440  .........>.=.B.@
-0000a780: 0430 0433 0435 043d 0442 003a 0800 0000  .0.3.5.=.B.:....
-0000a790: 0006 0000 0005 5065 6572 3a07 0000 0010  ......Peer:.....
-0000a7a0: 5065 6572 5265 706f 7274 5769 6467 6574  PeerReportWidget
-0000a7b0: 0103 0000 0028 041e 0442 0447 0435 0442  .....(...B.G.5.B
-0000a7c0: 0020 043f 043e 0020 043a 043e 043d 0442  . .?.>. .:.>.=.B
-0000a7d0: 0440 0430 0433 0435 043d 0442 0443 0800  .@.0.3.5.=.B.C..
-0000a7e0: 0000 0006 0000 000e 5265 706f 7274 2062  ........Report b
-0000a7f0: 7920 7065 6572 0700 0000 1050 6565 7252  y peer.....PeerR
-0000a800: 6570 6f72 7457 6964 6765 7401 0300 0000  eportWidget.....
-0000a810: 1604 1a04 3e04 3b00 2d04 3204 3e00 2004  ....>.;.-.2.>. .
-0000a820: 3404 3e04 3a00 2e08 0000 0000 0600 0000  4.>.:...........
-0000a830: 0a44 6f63 7320 636f 756e 7407 0000 000d  .Docs count.....
-0000a840: 5065 6572 5472 6565 4d6f 6465 6c01 0300  PeerTreeModel...
-0000a850: 0000 0a04 1004 3404 4004 3504 4108 0000  ......4.@.5.A...
-0000a860: 0000 0600 0000 084c 6f63 6174 696f 6e07  .......Location.
-0000a870: 0000 000d 5065 6572 5472 6565 4d6f 6465  ....PeerTreeMode
-0000a880: 6c01 0300 0000 1804 1d04 3004 3804 3c04  l.........0.8.<.
-0000a890: 3504 3d04 3e04 3204 3004 3d04 3804 3508  5.=.>.2.0.=.8.5.
-0000a8a0: 0000 0000 0600 0000 044e 616d 6507 0000  .........Name...
-0000a8b0: 000d 5065 6572 5472 6565 4d6f 6465 6c01  ..PeerTreeModel.
-0000a8c0: 0300 0000 1a04 2104 4704 3504 4204 3000  ......!.G.5.B.0.
-0000a8d0: 2004 3200 2004 3104 3004 3d04 3a04 3508   .2. .1.0.=.:.5.
-0000a8e0: 0000 0000 0600 0000 0d42 616e 6b20 6163  .........Bank ac
-0000a8f0: 636f 756e 7473 0700 0000 1650 7265 6465  counts.....Prede
-0000a900: 6669 6e64 6564 4163 636f 756e 7454 7970  findedAccountTyp
-0000a910: 6501 0300 0000 0a04 1a04 3004 4004 4204  e.........0.@.B.
-0000a920: 4b08 0000 0000 0600 0000 0543 6172 6473  K..........Cards
-0000a930: 0700 0000 1650 7265 6465 6669 6e64 6564  .....Predefinded
-0000a940: 4163 636f 756e 7454 7970 6501 0300 0000  AccountType.....
-0000a950: 1004 1d04 3004 3b04 3804 4704 3d04 4b04  ....0.;.8.G.=.K.
-0000a960: 3508 0000 0000 0600 0000 0443 6173 6807  5..........Cash.
-0000a970: 0000 0016 5072 6564 6566 696e 6465 6441  ....PredefindedA
-0000a980: 6363 6f75 6e74 5479 7065 0103 0000 001e  ccountType......
-0000a990: 041a 0440 0435 0434 0438 0442 044b 0020  ...@.5.4.8.B.K. 
-0000a9a0: 002f 0020 0414 043e 043b 0433 0438 0800  ./. ...>.;.3.8..
-0000a9b0: 0000 0006 0000 000d 4465 6274 7320 2f20  ........Debts / 
-0000a9c0: 4c6f 616e 7307 0000 0016 5072 6564 6566  Loans.....Predef
-0000a9d0: 696e 6465 6441 6363 6f75 6e74 5479 7065  indedAccountType
-0000a9e0: 0103 0000 0014 0418 043d 0432 0435 0441  .........=.2.5.A
-0000a9f0: 0442 0438 0446 0438 0438 0800 0000 0006  .B.8.F.8.8......
-0000aa00: 0000 000b 496e 7665 7374 6d65 6e74 7307  ....Investments.
-0000aa10: 0000 0016 5072 6564 6566 696e 6465 6441  ....PredefindedA
-0000aa20: 6363 6f75 6e74 5479 7065 0103 0000 0014  ccountType......
-0000aa30: 0421 0431 0435 0440 0435 0436 0435 043d  .!.1.5.@.5.6.5.=
-0000aa40: 0438 044f 0800 0000 0006 0000 0007 5361  .8.O..........Sa
-0000aa50: 7669 6e67 7307 0000 0016 5072 6564 6566  vings.....Predef
-0000aa60: 696e 6465 6441 6363 6f75 6e74 5479 7065  indedAccountType
-0000aa70: 0103 0000 0014 0065 002d 041a 043e 0448  .......e.-...>.H
-0000aa80: 0435 043b 044c 043a 0438 0800 0000 0006  .5.;.L.:.8......
-0000aa90: 0000 0009 652d 5761 6c6c 6574 7307 0000  ....e-Wallets...
-0000aaa0: 0016 5072 6564 6566 696e 6465 6441 6363  ..PredefindedAcc
-0000aab0: 6f75 6e74 5479 7065 0103 0000 0012 041e  ountType........
-0000aac0: 0431 043b 0438 0433 0430 0446 0438 0438  .1.;.8.3.0.F.8.8
-0000aad0: 0800 0000 0006 0000 0005 426f 6e64 7307  ..........Bonds.
-0000aae0: 0000 000f 5072 6564 6566 696e 6564 4173  ....PredefinedAs
-0000aaf0: 7365 7401 0300 0000 0c04 2204 3e04 3204  set.......".>.2.
-0000ab00: 3004 4004 4b08 0000 0000 0600 0000 0b43  0.@.K..........C
-0000ab10: 6f6d 6d6f 6469 7469 6573 0700 0000 0f50  ommodities.....P
-0000ab20: 7265 6465 6669 6e65 6441 7373 6574 0103  redefinedAsset..
-0000ab30: 0000 0018 041a 0440 0438 043f 0442 043e  .......@.8.?.B.>
-0000ab40: 0432 0430 043b 044e 0442 044b 0800 0000  .2.0.;.N.B.K....
-0000ab50: 0006 0000 000f 4372 7970 746f 2d63 7572  ......Crypto-cur
-0000ab60: 7265 6e63 7907 0000 000f 5072 6564 6566  rency.....Predef
-0000ab70: 696e 6564 4173 7365 7401 0300 0000 1404  inedAsset.......
-0000ab80: 1404 3504 4004 3804 3204 3004 4204 3804  ..5.@.8.2.0.B.8.
-0000ab90: 3204 4b08 0000 0000 0600 0000 0b44 6572  2.K..........Der
-0000aba0: 6976 6174 6976 6573 0700 0000 0f50 7265  ivatives.....Pre
+00003f90: 000e 043d 043e 043c 0438 043d 0430 043b  ...=.>.<.8.=.0.;
+00003fa0: 0800 0000 0006 0000 0009 7072 696e 6369  ..........princi
+00003fb0: 7061 6c07 0000 000c 4461 7461 4465 6c65  pal.....DataDele
+00003fc0: 6761 7465 0103 0000 000e 0440 0435 0433  gate.......@.5.3
+00003fd0: 002e 043a 043e 0434 0800 0000 0006 0000  ...:.>.4........
+00003fe0: 0008 7265 672e 636f 6465 0700 0000 0c44  ..reg.code.....D
+00003ff0: 6174 6144 656c 6567 6174 6501 0300 0000  ataDelegate.....
+00004000: 1004 1204 4104 3500 2004 3404 3004 4204  ....A.5. .4.0.B.
+00004010: 4b08 0000 0000 0600 0000 0941 6c6c 2064  K..........All d
+00004020: 6174 6573 0700 0000 1144 6174 6552 616e  ates.....DateRan
+00004030: 6765 5365 6c65 6374 6f72 0103 0000 0004  geSelector......
+00004040: 0421 003a 0800 0000 0006 0000 0005 4672  .!.:..........Fr
+00004050: 6f6d 3a07 0000 0011 4461 7465 5261 6e67  om:.....DateRang
+00004060: 6553 656c 6563 746f 7201 0300 0000 0a04  eSelector.......
+00004070: 1c04 3504 4104 4f04 4608 0000 0000 0600  ..5.A.O.F.......
+00004080: 0000 054d 6f6e 7468 0700 0000 1144 6174  ...Month.....Dat
+00004090: 6552 616e 6765 5365 6c65 6374 6f72 0103  eRangeSelector..
+000040a0: 0000 001c 041f 0440 0435 0434 044b 0434  .......@.5.4.K.4
+000040b0: 0443 0449 0438 0439 0020 0433 043e 0434  .C.I.8.9. .3.>.4
+000040c0: 0800 0000 0006 0000 000d 5072 6576 696f  ..........Previo
+000040d0: 7573 2079 6561 7207 0000 0011 4461 7465  us year.....Date
+000040e0: 5261 6e67 6553 656c 6563 746f 7201 0300  RangeSelector...
+000040f0: 0000 0e04 1a04 3204 3004 4004 4204 3004  ......2.0.@.B.0.
+00004100: 3b08 0000 0000 0600 0000 0751 7561 7274  ;..........Quart
+00004110: 6572 0700 0000 1144 6174 6552 616e 6765  er.....DateRange
+00004120: 5365 6c65 6374 6f72 0103 0000 0024 0422  Selector.....$."
+00004130: 0435 043a 0443 0449 0438 0439 0020 0434  .5.:.C.I.8.9. .4
+00004140: 043e 0020 0441 0435 0433 043e 0434 043d  .>. .A.5.3.>.4.=
+00004150: 044f 0800 0000 0006 0000 000f 5175 6172  .O..........Quar
+00004160: 7465 7220 746f 2064 6174 6507 0000 0011  ter to date.....
+00004170: 4461 7465 5261 6e67 6553 656c 6563 746f  DateRangeSelecto
+00004180: 7201 0300 0000 1604 2204 3504 3a04 4304  r.......".5.:.C.
+00004190: 4904 3804 3900 2004 3304 3e04 3408 0000  I.8.9. .3.>.4...
+000041a0: 0000 0600 0000 0954 6869 7320 7965 6172  .......This year
+000041b0: 0700 0000 1144 6174 6552 616e 6765 5365  .....DateRangeSe
+000041c0: 6c65 6374 6f72 0103 0000 0006 0414 043e  lector.........>
+000041d0: 003a 0800 0000 0006 0000 0003 546f 3a07  .:..........To:.
+000041e0: 0000 0011 4461 7465 5261 6e67 6553 656c  ....DateRangeSel
+000041f0: 6563 746f 7201 0300 0000 0c04 1d04 3504  ector.........5.
+00004200: 3404 3504 3b04 4f08 0000 0000 0600 0000  4.5.;.O.........
+00004210: 0457 6565 6b07 0000 0011 4461 7465 5261  .Week.....DateRa
+00004220: 6e67 6553 656c 6563 746f 7201 0300 0000  ngeSelector.....
+00004230: 0604 1304 3e04 3408 0000 0000 0600 0000  ....>.4.........
+00004240: 0459 6561 7207 0000 0011 4461 7465 5261  .Year.....DateRa
+00004250: 6e67 6553 656c 6563 746f 7201 0300 0000  ngeSelector.....
+00004260: 1c04 1304 3e04 3400 2004 3404 3e00 2004  ....>.4. .4.>. .
+00004270: 4104 3504 3304 3e04 3404 3d04 4f08 0000  A.5.3.>.4.=.O...
+00004280: 0000 0600 0000 0c59 6561 7220 746f 2064  .......Year to d
+00004290: 6174 6507 0000 0011 4461 7465 5261 6e67  ate.....DateRang
+000042a0: 6553 656c 6563 746f 7201 0300 0000 1e04  eSelector.......
+000042b0: 2104 3404 3504 3b04 3a04 3800 2004 3f04  !.4.5.;.:.8. .?.
+000042c0: 3e00 2004 4104 4704 3504 4204 4308 0000  >. .A.G.5.B.C...
+000042d0: 0000 0600 0000 1044 6561 6c73 2062 7920  .......Deals by 
+000042e0: 4163 636f 756e 7407 0000 000b 4465 616c  Account.....Deal
+000042f0: 7352 6570 6f72 7401 0300 0000 0a04 2104  sReport.......!.
+00004300: 4704 3504 4200 3a08 0000 0000 0600 0000  G.5.B.:.........
+00004310: 0841 6363 6f75 6e74 3a07 0000 0011 4465  .Account:.....De
+00004320: 616c 7352 6570 6f72 7457 6964 6765 7401  alsReportWidget.
+00004330: 0300 0000 0c04 2104 3404 3504 3b04 3a04  ......!.4.5.;.:.
+00004340: 3808 0000 0000 0600 0000 0544 6561 6c73  8..........Deals
+00004350: 0700 0000 1144 6561 6c73 5265 706f 7274  .....DealsReport
+00004360: 5769 6467 6574 0103 0000 0020 0413 0440  Widget..... ...@
+00004370: 0443 043f 043f 0438 0440 043e 0432 0430  .C.?.?.8.@.>.2.0
+00004380: 0442 044c 0020 043f 043e 003a 0800 0000  .B.L. .?.>.:....
+00004390: 0006 0000 0009 4772 6f75 7020 6279 3a07  ......Group by:.
+000043a0: 0000 0011 4465 616c 7352 6570 6f72 7457  ....DealsReportW
+000043b0: 6964 6765 7401 0300 0000 0e00 3c04 1f04  idget.......<...
+000043c0: 4304 4104 4204 3e00 3e08 0000 0000 0600  C.A.B.>.>.......
+000043d0: 0000 063c 4e6f 6e65 3e07 0000 0011 4465  ...<None>.....De
+000043e0: 616c 7352 6570 6f72 7457 696e 646f 7701  alsReportWindow.
+000043f0: 0300 0000 1a04 2604 3504 3d04 3d04 3004  ......&.5.=.=.0.
+00004400: 4f00 2004 3104 4304 3c04 3004 3304 3008  O. .1.C.<.0.3.0.
+00004410: 0000 0000 0600 0000 0541 7373 6574 0700  .........Asset..
+00004420: 0000 1144 6561 6c73 5265 706f 7274 5769  ...DealsReportWi
+00004430: 6e64 6f77 0103 0000 0030 0426 0411 0020  ndow.....0.&... 
+00004440: 002d 0020 041e 0442 043a 0440 044b 0442  .-. ...B.:.@.K.B
+00004450: 0438 0435 0020 002d 0020 0417 0430 043a  .8.5. .-. ...0.:
+00004460: 0440 044b 0442 0438 0435 0800 0000 0006  .@.K.B.8.5......
+00004470: 0000 0014 4173 7365 7420 2d20 4f70 656e  ....Asset - Open
+00004480: 202d 2043 6c6f 7365 0700 0000 1144 6561   - Close.....Dea
+00004490: 6c73 5265 706f 7274 5769 6e64 6f77 0103  lsReportWindow..
+000044a0: 0000 0010 0417 0430 043a 0440 044b 0442  .......0.:.@.K.B
+000044b0: 0438 0435 0800 0000 0006 0000 0005 436c  .8.5..........Cl
+000044c0: 6f73 6507 0000 0011 4465 616c 7352 6570  ose.....DealsRep
+000044d0: 6f72 7457 696e 646f 7701 0300 0000 2604  ortWindow.....&.
+000044e0: 1704 3004 3a04 4004 4b04 4204 3804 3500  ..0.:.@.K.B.8.5.
+000044f0: 2000 2d00 2004 1e04 4204 3a04 4004 4b04   .-. ...B.:.@.K.
+00004500: 4204 3804 3508 0000 0000 0600 0000 0c43  B.8.5..........C
+00004510: 6c6f 7365 202d 204f 7065 6e07 0000 0011  lose - Open.....
+00004520: 4465 616c 7352 6570 6f72 7457 696e 646f  DealsReportWindo
+00004530: 7701 0300 0000 2604 1e04 4204 3a04 4004  w.....&...B.:.@.
+00004540: 4b04 4204 3804 3500 2000 2d00 2004 1704  K.B.8.5. .-. ...
+00004550: 3004 3a04 4004 4b04 4204 3804 3508 0000  0.:.@.K.B.8.5...
+00004560: 0000 0600 0000 0c4f 7065 6e20 2d20 436c  .......Open - Cl
+00004570: 6f73 6507 0000 0011 4465 616c 7352 6570  ose.....DealsRep
+00004580: 6f72 7457 696e 646f 7701 0300 0000 0a04  ortWindow.......
+00004590: 2104 4304 3c04 3c04 3008 0000 0000 0600  !.C.<.<.0.......
+000045a0: 0000 0641 6d6f 756e 7407 0000 000c 4465  ...Amount.....De
+000045b0: 7461 696c 734d 6f64 656c 0103 0000 0012  tailsModel......
+000045c0: 041a 0430 0442 0435 0433 043e 0440 0438  ...0.B.5.3.>.@.8
+000045d0: 044f 0800 0000 0006 0000 0008 4361 7465  .O..........Cate
+000045e0: 676f 7279 0700 0000 0c44 6574 6169 6c73  gory.....Details
+000045f0: 4d6f 6465 6c01 0300 0000 1004 1e04 3f04  Model.........?.
+00004600: 3804 4104 3004 3d04 3804 3508 0000 0000  8.A.0.=.8.5.....
+00004610: 0600 0000 044e 6f74 6507 0000 000c 4465  .....Note.....De
+00004620: 7461 696c 734d 6f64 656c 0103 0000 000a  tailsModel......
+00004630: 041c 0435 0442 043a 0430 0800 0000 0006  ...5.B.:.0......
+00004640: 0000 0003 5461 6707 0000 000c 4465 7461  ....Tag.....Deta
+00004650: 696c 734d 6f64 656c 0103 0000 009e 041d  ilsModel........
+00004660: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
+00004670: 043e 0020 043e 0431 0440 0430 0431 043e  .>. .>.1.@.0.1.>
+00004680: 0442 0430 0442 044c 0020 0434 0438 0432  .B.0.B.L. .4.8.2
+00004690: 0438 0434 0435 043d 0434 002c 0020 0442  .8.4.5.=.4.,. .B
+000046a0: 002e 043a 002e 0020 043d 0435 0020 0443  ...:... .=.5. .C
+000046b0: 043a 0430 0437 0430 043d 0020 0431 0430  .:.0.7.0.=. .1.0
+000046c0: 043d 043a 0020 0434 043b 044f 0020 0438  .=.:. .4.;.O. .8
+000046d0: 043d 0432 0435 0441 0442 0438 0446 0438  .=.2.5.A.B.8.F.8
+000046e0: 043e 043d 043d 043e 0433 043e 0020 0441  .>.=.=.>.3.>. .A
+000046f0: 0447 0451 0442 0430 003a 0020 0800 0000  .G.Q.B.0.:. ....
+00004700: 0006 0000 0041 4361 6e27 7420 7072 6f63  .....ACan't proc
+00004710: 6573 7320 6469 7669 6465 6e64 2061 7320  ess dividend as 
+00004720: 6261 6e6b 2069 736e 2774 2073 6574 2066  bank isn't set f
+00004730: 6f72 2069 6e76 6573 746d 656e 7420 6163  or investment ac
+00004740: 636f 756e 743a 2007 0000 0008 4469 7669  count: .....Divi
+00004750: 6465 6e64 0103 0000 005a 041d 0435 0020  dend.....Z...5. 
+00004760: 0437 0430 0434 0430 043d 0430 0020 0446  .7.0.4.0.=.0. .F
+00004770: 0435 043d 0430 0020 0434 043b 044f 0020  .5.=.0. .4.;.O. 
+00004780: 0432 044b 043f 043b 0430 0442 044b 0020  .2.K.?.;.0.B.K. 
+00004790: 0446 0435 043d 043d 044b 043c 0438 0020  .F.5.=.=.K.<.8. 
+000047a0: 0431 0443 043c 0430 0433 0430 043c 0438  .1.C.<.0.3.0.<.8
+000047b0: 003a 0020 0800 0000 0006 0000 002a 4e6f  .:. .........*No
+000047c0: 2070 7269 6365 2064 6174 6120 666f 7220   price data for 
+000047d0: 7374 6f63 6b20 6469 7669 6465 6e64 2f76  stock dividend/v
+000047e0: 6573 7469 6e67 3a20 0700 0000 0844 6976  esting: .....Div
+000047f0: 6964 656e 6401 0300 0000 7204 1d04 3504  idend.....r...5.
+00004800: 4200 2004 3a04 3e04 4204 3804 4004 3e04  B. .:.>.B.8.@.>.
+00004810: 3204 3a04 3800 2004 3404 3b04 4f00 2004  2.:.8. .4.;.O. .
+00004820: 3404 3804 3204 3804 3404 3504 3d04 3404  4.8.2.8.4.5.=.4.
+00004830: 3000 2004 3004 3a04 4604 3804 4f04 3c04  0. .0.:.F.8.O.<.
+00004840: 3800 2004 3804 3b04 3800 2004 3704 3004  8. .8.;.8. .7.0.
+00004850: 4704 3804 4104 3b04 3504 3d04 3804 4f00  G.8.A.;.5.=.8.O.
+00004860: 2004 3004 3a04 4604 3804 3900 2e08 0000   .0.:.F.8.9.....
+00004870: 0000 0600 0000 2d4e 6f20 7374 6f63 6b20  ......-No stock 
+00004880: 7175 6f74 6520 666f 7220 7374 6f63 6b20  quote for stock 
+00004890: 6469 7669 6465 6e64 206f 7220 7665 7374  dividend or vest
+000048a0: 696e 672e 0700 0000 0844 6976 6964 656e  ing......Dividen
+000048b0: 6401 0300 0000 b804 1d04 3504 3f04 3e04  d.........5.?.>.
+000048c0: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
+000048d0: 3504 3c04 3e04 3500 2004 3404 3504 3904  5.<.>.5. .4.5.9.
+000048e0: 4104 4204 3204 3804 3500 3a00 2004 3404  A.B.2.8.5.:. .4.
+000048f0: 3804 3204 3804 3404 3504 3d04 3400 2004  8.2.8.4.5.=.4. .
+00004900: 3004 3a04 4604 3804 4f04 3c04 3800 2004  0.:.F.8.O.<.8. .
+00004910: 3804 3b04 3800 2004 3704 3004 4704 3804  8.;.8. .7.0.G.8.
+00004920: 4104 3b04 3504 3d04 3804 3500 2004 3004  A.;.5.=.8.5. .0.
+00004930: 3a04 4604 3804 3900 2004 3704 3004 3a04  :.F.8.9. .7.0.:.
+00004940: 4004 4b04 3204 3004 3504 4200 2004 3a04  @.K.2.0.5.B. .:.
+00004950: 3e04 4004 3e04 4204 3a04 4304 4e00 2004  >.@.>.B.:.C.N. .
+00004960: 3f04 3e04 3704 3804 4604 3804 4e00 2e08  ?.>.7.8.F.8.N...
+00004970: 0000 0000 0600 0000 434e 6f74 2073 7570  ........CNot sup
+00004980: 706f 7274 6564 2061 6374 696f 6e3a 2073  ported action: s
+00004990: 746f 636b 2064 6976 6964 656e 6420 6f72  tock dividend or
+000049a0: 2076 6573 7469 6e67 2063 6c6f 7365 7320   vesting closes 
+000049b0: 7368 6f72 7420 7472 6164 652e 0700 0000  short trade.....
+000049c0: 0844 6976 6964 656e 6401 0300 0000 0e04  .Dividend.......
+000049d0: 1d04 3004 3b04 3e04 3300 3a00 2008 0000  ..0.;.>.3.:. ...
+000049e0: 0000 0600 0000 0554 6178 3a20 0700 0000  .......Tax: ....
+000049f0: 0844 6976 6964 656e 6401 0300 0000 3e04  .Dividend.....>.
+00004a00: 1d04 3504 3f04 3e04 3404 3404 3504 4004  ..5.?.>.4.4.5.@.
+00004a10: 3604 3804 3204 3004 3504 3c04 4b04 3900  6.8.2.0.5.<.K.9.
+00004a20: 2004 4204 3804 3f00 2004 3404 3804 3204   .B.8.?. .4.8.2.
+00004a30: 3804 3404 3504 3d04 3404 3000 2e08 0000  8.4.5.=.4.0.....
+00004a40: 0000 0600 0000 1a55 6e73 7570 706f 7274  .......Unsupport
+00004a50: 6564 2064 6976 6964 656e 6420 7479 7065  ed dividend type
+00004a60: 2e07 0000 0008 4469 7669 6465 6e64 0103  ......Dividend..
+00004a70: 0000 0002 2116 0800 0000 0006 0000 0001  ....!...........
+00004a80: 2307 0000 000e 4469 7669 6465 6e64 5769  #.....DividendWi
+00004a90: 6467 6574 0103 0000 0008 0421 0447 0435  dget.......!.G.5
+00004aa0: 0442 0800 0000 0006 0000 0007 4163 636f  .B..........Acco
+00004ab0: 756e 7407 0000 000e 4469 7669 6465 6e64  unt.....Dividend
+00004ac0: 5769 6467 6574 0103 0000 0004 0426 0411  Widget.......&..
+00004ad0: 0800 0000 0006 0000 0005 4173 7365 7407  ..........Asset.
+00004ae0: 0000 000e 4469 7669 6465 6e64 5769 6467  ....DividendWidg
+00004af0: 6574 0103 0000 000a 041a 0443 043f 043e  et.........C.?.>
+00004b00: 043d 0800 0000 0006 0000 000d 426f 6e64  .=..........Bond
+00004b10: 2049 6e74 6572 6573 7407 0000 000e 4469   Interest.....Di
+00004b20: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
+00004b30: 0014 0414 0430 0442 0430 002f 0412 0440  .....0.B.0./...@
+00004b40: 0435 043c 044f 0800 0000 0006 0000 0009  .5.<.O..........
+00004b50: 4461 7465 2f54 696d 6507 0000 000e 4469  Date/Time.....Di
+00004b60: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
+00004b70: 0010 0414 0438 0432 0438 0434 0435 043d  .....8.2.8.4.5.=
+00004b80: 0434 0800 0000 0006 0000 0008 4469 7669  .4..........Divi
+00004b90: 6465 6e64 0700 0000 0e44 6976 6964 656e  dend.....Dividen
+00004ba0: 6457 6964 6765 7401 0300 0000 0e04 1e04  dWidget.........
+00004bb0: 4204 4104 3504 4704 3a04 3008 0000 0000  B.A.5.G.:.0.....
+00004bc0: 0600 0000 0745 782d 4461 7465 0700 0000  .....Ex-Date....
+00004bd0: 0e44 6976 6964 656e 6457 6964 6765 7401  .DividendWidget.
+00004be0: 0300 0000 0600 4e00 2f00 4108 0000 0000  ......N./.A.....
+00004bf0: 0600 0000 034e 2f41 0700 0000 0e44 6976  .....N/A.....Div
+00004c00: 6964 656e 6457 6964 6765 7401 0300 0000  idendWidget.....
+00004c10: 1a04 1d04 3504 4200 2004 3a04 3e04 4204  ....5.B. .:.>.B.
+00004c20: 3804 4004 3e04 3204 3a04 3808 0000 0000  8.@.>.2.:.8.....
+00004c30: 0600 0000 084e 6f20 7175 6f74 6507 0000  .....No quote...
+00004c40: 000e 4469 7669 6465 6e64 5769 6467 6574  ..DividendWidget
+00004c50: 0103 0000 0010 041e 043f 0438 0441 0430  .........?.8.A.0
+00004c60: 043d 0438 0435 0800 0000 0006 0000 0004  .=.8.5..........
+00004c70: 4e6f 7465 0700 0000 0e44 6976 6964 656e  Note.....Dividen
+00004c80: 6457 6964 6765 7401 0300 0000 0804 2604  dWidget.......&.
+00004c90: 3504 3d04 3008 0000 0000 0600 0000 0550  5.=.0..........P
+00004ca0: 7269 6365 0700 0000 0e44 6976 6964 656e  rice.....Dividen
+00004cb0: 6457 6964 6765 7401 0300 0000 2004 1404  dWidget..... ...
+00004cc0: 3804 3204 3804 3404 3504 3d04 3400 2004  8.2.8.4.5.=.4. .
+00004cd0: 3004 3a04 4604 3804 4f04 3c04 3808 0000  0.:.F.8.O.<.8...
+00004ce0: 0000 0600 0000 0e53 746f 636b 2044 6976  .......Stock Div
+00004cf0: 6964 656e 6407 0000 000e 4469 7669 6465  idend.....Divide
+00004d00: 6e64 5769 6467 6574 0103 0000 001c 041f  ndWidget........
+00004d10: 0435 0440 0435 0434 0430 0447 0430 0020  .5.@.5.4.0.G.0. 
+00004d20: 0430 043a 0446 0438 0439 0800 0000 0006  .0.:.F.8.9......
+00004d30: 0000 000d 5374 6f63 6b20 5665 7374 696e  ....Stock Vestin
+00004d40: 6707 0000 000e 4469 7669 6465 6e64 5769  g.....DividendWi
+00004d50: 6467 6574 0103 0000 000a 041d 0430 043b  dget.........0.;
+00004d60: 043e 0433 0800 0000 0006 0000 0003 5461  .>.3..........Ta
+00004d70: 7807 0000 000e 4469 7669 6465 6e64 5769  x.....DividendWi
+00004d80: 6467 6574 0103 0000 0006 0422 0438 043f  dget.......".8.?
+00004d90: 0800 0000 0006 0000 0004 5479 7065 0700  ..........Type..
+00004da0: 0000 0e44 6976 6964 656e 6457 6964 6765  ...DividendWidge
+00004db0: 7401 0300 0000 b204 1d04 4304 3604 3d04  t.........C.6.=.
+00004dc0: 3e00 2004 4304 4104 4204 3004 3d04 3e04  >. .C.A.B.0.=.>.
+00004dd0: 3204 3804 4204 4c00 2004 3a04 3e04 4204  2.8.B.L. .:.>.B.
+00004de0: 3804 4004 3e04 3204 3a04 4300 2004 3104  8.@.>.2.:.C. .1.
+00004df0: 4304 3c04 3004 3304 3800 2004 3404 3b04  C.<.0.3.8. .4.;.
+00004e00: 4f00 2004 1404 3004 4204 4b00 2f04 1204  O. ...0.B.K./...
+00004e10: 4004 3504 3c04 3504 3d04 3800 2004 3404  @.5.<.5.=.8. .4.
+00004e20: 3804 3204 3804 3404 3504 3d04 3404 3000  8.2.8.4.5.=.4.0.
+00004e30: 2004 4704 3504 4004 3504 3700 2004 3c04   .G.5.@.5.7. .<.
+00004e40: 3504 3d04 4e00 2004 1404 3004 3d04 3d04  5.=.N. ...0.=.=.
+00004e50: 4b04 3500 2d00 3e04 1a04 3e04 4204 3804  K.5.-.>...>.B.8.
+00004e60: 4004 3e04 3204 3a04 3808 0000 0000 0600  @.>.2.:.8.......
+00004e70: 0000 4859 6f75 2073 686f 756c 6420 7365  ..HYou should se
+00004e80: 7420 7175 6f74 6520 7669 6120 4461 7461  t quote via Data
+00004e90: 2d3e 5175 6f74 6573 206d 656e 7520 666f  ->Quotes menu fo
+00004ea0: 7220 4461 7465 2f54 696d 6520 6f66 2074  r Date/Time of t
+00004eb0: 6865 2064 6976 6964 656e 6407 0000 000e  he dividend.....
+00004ec0: 4469 7669 6465 6e64 5769 6467 6574 0103  DividendWidget..
+00004ed0: 0000 0014 043d 0435 0438 0437 0432 0435  .....=.5.8.7.2.5
+00004ee0: 0441 0442 043d 043e 0800 0000 0006 0000  .A.B.=.>........
+00004ef0: 0007 756e 6b6e 6f77 6e07 0000 000e 4469  ..unknown.....Di
+00004f00: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
+00004f10: 0010 0421 0432 043e 0439 0441 0442 0432  ...!.2.>.9.A.B.2
+00004f20: 043e 0800 0000 0006 0000 0008 5072 6f70  .>..........Prop
+00004f30: 6572 7479 0700 0000 0e45 7874 7261 4461  erty.....ExtraDa
+00004f40: 7461 4d6f 6465 6c01 0300 0000 1004 1704  taModel.........
+00004f50: 3d04 3004 4704 3504 3d04 3804 3508 0000  =.0.G.5.=.8.5...
+00004f60: 0000 0600 0000 0556 616c 7565 0700 0000  .......Value....
+00004f70: 0e45 7874 7261 4461 7461 4d6f 6465 6c01  .ExtraDataModel.
+00004f80: 0300 0000 1a04 2604 3504 3d04 3d04 3004  ......&.5.=.=.0.
+00004f90: 4f00 2004 3104 4304 3c04 3004 3304 3008  O. .1.C.<.0.3.0.
+00004fa0: 0000 0000 0600 0000 0a41 7373 6574 204e  .........Asset N
+00004fb0: 616d 6507 0000 000d 486f 6c64 696e 6773  ame.....Holdings
+00004fc0: 4d6f 6465 6c01 0300 0000 1c04 1204 3004  Model.........0.
+00004fd0: 3b04 4e04 4204 3000 2f04 2104 4704 5104  ;.N.B.0./.!.G.Q.
+00004fe0: 4200 2f04 2604 1108 0000 0000 0600 0000  B./.&...........
+00004ff0: 1643 7572 7265 6e63 792f 4163 636f 756e  .Currency/Accoun
+00005000: 742f 4173 7365 7407 0000 000d 486f 6c64  t/Asset.....Hold
+00005010: 696e 6773 4d6f 6465 6c01 0300 0000 0a04  ingsModel.......
+00005020: 2d04 3a04 4104 3f00 3a08 0000 0000 0600  -.:.A.?.:.......
+00005030: 0000 0445 7870 3a07 0000 000d 486f 6c64  ...Exp:.....Hold
+00005040: 696e 6773 4d6f 6465 6c01 0300 0000 1404  ingsModel.......
+00005050: 2604 3504 3d04 3000 2004 3704 3004 3a04  &.5.=.0. .7.0.:.
+00005060: 4000 2e08 0000 0000 0600 0000 044c 6173  @............Las
+00005070: 7407 0000 000d 486f 6c64 696e 6773 4d6f  t.....HoldingsMo
+00005080: 6465 6c01 0300 0000 3404 1404 3004 4204  del.....4...0.B.
+00005090: 3000 2004 3f04 3e04 4104 3b04 3504 3404  0. .?.>.A.;.5.4.
+000050a0: 3d04 3504 3900 2004 3a04 3e04 4204 3804  =.5.9. .:.>.B.8.
+000050b0: 4004 3e04 3204 3a04 3800 3a00 2008 0000  @.>.2.:.8.:. ...
+000050c0: 0000 0600 0000 114c 6173 7420 7175 6f74  .......Last quot
+000050d0: 6520 6461 7465 3a20 0700 0000 0d48 6f6c  e date: .....Hol
+000050e0: 6469 6e67 734d 6f64 656c 0103 0000 0014  dingsModel......
+000050f0: 0426 0435 043d 0430 0020 043e 0442 043a  .&.5.=.0. .>.B.:
+00005100: 0440 002e 0800 0000 0006 0000 0004 4f70  .@............Op
+00005110: 656e 0700 0000 0d48 6f6c 6469 6e67 734d  en.....HoldingsM
+00005120: 6f64 656c 0103 0000 0006 041f 0438 0423  odel.........8.#
+00005130: 0800 0000 0006 0000 0003 502f 4c07 0000  ..........P/L...
+00005140: 000d 486f 6c64 696e 6773 4d6f 6465 6c01  ..HoldingsModel.
+00005150: 0300 0000 0c04 1f04 3804 2300 2c00 2000  ........8.#.,. .
+00005160: 2508 0000 0000 0600 0000 0650 2f4c 2c20  %..........P/L, 
+00005170: 2507 0000 000d 486f 6c64 696e 6773 4d6f  %.....HoldingsMo
+00005180: 6465 6c01 0300 0000 0c04 1a04 3e04 3b00  del.........>.;.
+00005190: 2d04 3204 3e08 0000 0000 0600 0000 0351  -.2.>..........Q
+000051a0: 7479 0700 0000 0d48 6f6c 6469 6e67 734d  ty.....HoldingsM
+000051b0: 6f64 656c 0103 0000 000e 0414 043e 043b  odel.........>.;
+000051c0: 044f 002c 0020 0025 0800 0000 0006 0000  .O.,. .%........
+000051d0: 0008 5368 6172 652c 2025 0700 0000 0d48  ..Share, %.....H
+000051e0: 6f6c 6469 6e67 734d 6f64 656c 0103 0000  oldingsModel....
+000051f0: 000c 041e 0446 0435 043d 043a 0430 0800  .....F.5.=.:.0..
+00005200: 0000 0006 0000 0005 5661 6c75 6507 0000  ........Value...
+00005210: 000d 486f 6c64 696e 6773 4d6f 6465 6c01  ..HoldingsModel.
+00005220: 0300 0000 1004 1e04 4604 3504 3d04 3a04  ........F.5.=.:.
+00005230: 3000 2c00 2008 0000 0000 0600 0000 0756  0.,. ..........V
+00005240: 616c 7565 2c20 0700 0000 0d48 6f6c 6469  alue, .....Holdi
+00005250: 6e67 734d 6f64 656c 0103 0000 0016 041f  ngsModel........
+00005260: 043e 0440 0442 0444 0435 043b 044c 0020  .>.@.B.D.5.;.L. 
+00005270: 0426 0411 0800 0000 0006 0000 0008 486f  .&............Ho
+00005280: 6c64 696e 6773 0700 0000 0e48 6f6c 6469  ldings.....Holdi
+00005290: 6e67 7352 6570 6f72 7401 0300 0000 1a04  ngsReport.......
+000052a0: 1e04 4604 3504 3d04 3804 4204 4c00 2004  ..F.5.=.8.B.L. .
+000052b0: 3d04 3004 3b04 3e04 3308 0000 0000 0600  =.0.;.>.3.......
+000052c0: 0000 0c45 7374 696d 6174 6520 7461 7807  ...Estimate tax.
+000052d0: 0000 0014 486f 6c64 696e 6773 5265 706f  ....HoldingsRepo
+000052e0: 7274 5769 6e64 6f77 0103 0000 0016 041f  rtWindow........
+000052f0: 043e 0440 0442 0444 0435 043b 044c 0020  .>.@.B.D.5.;.L. 
+00005300: 0426 0411 0800 0000 0006 0000 0008 486f  .&............Ho
+00005310: 6c64 696e 6773 0700 0000 1448 6f6c 6469  ldings.....Holdi
+00005320: 6e67 7352 6570 6f72 7457 696e 646f 7701  ngsReportWindow.
+00005330: 0300 0000 1404 1f04 3e04 4004 4204 4304  ........>.@.B.C.
+00005340: 3304 3004 3b04 3804 4f08 0000 0000 0600  3.0.;.8.O.......
+00005350: 0000 0850 6f72 7475 6761 6c07 0000 0014  ...Portugal.....
+00005360: 486f 6c64 696e 6773 5265 706f 7274 5769  HoldingsReportWi
+00005370: 6e64 6f77 0103 0000 000c 0420 043e 0441  ndow....... .>.A
+00005380: 0441 0438 044f 0800 0000 0006 0000 0006  .A.8.O..........
+00005390: 5275 7373 6961 0700 0000 1448 6f6c 6469  Russia.....Holdi
+000053a0: 6e67 7352 6570 6f72 7457 696e 646f 7701  ngsReportWindow.
+000053b0: 0300 0000 2804 1f04 3e04 3a04 3004 3704  ....(...>.:.0.7.
+000053c0: 3004 4204 4c00 2004 3304 4004 3004 4404  0.B.L. .3.@.0.D.
+000053d0: 3804 3a00 2004 4604 3504 3d04 4b08 0000  8.:. .F.5.=.K...
+000053e0: 0000 0600 0000 1053 686f 7720 5072 6963  .......Show Pric
+000053f0: 6520 4368 6172 7407 0000 0014 486f 6c64  e Chart.....Hold
+00005400: 696e 6773 5265 706f 7274 5769 6e64 6f77  ingsReportWindow
+00005410: 0103 0000 0022 0412 0430 043b 044e 0442  ....."...0.;.N.B
+00005420: 0430 0020 043f 0435 0440 0435 0441 0447  .0. .?.5.@.5.A.G
+00005430: 0451 0442 0430 003a 0800 0000 0006 0000  .Q.B.0.:........
+00005440: 0010 436f 6d6d 6f6e 2063 7572 7265 6e63  ..Common currenc
+00005450: 793a 0700 0000 0e48 6f6c 6469 6e67 7357  y:.....HoldingsW
+00005460: 6964 6765 7401 0300 0000 1604 1f04 3e04  idget.........>.
+00005470: 4004 4204 4404 3504 3b04 4c00 2004 2604  @.B.D.5.;.L. .&.
+00005480: 1108 0000 0000 0600 0000 0848 6f6c 6469  ...........Holdi
+00005490: 6e67 7307 0000 000e 486f 6c64 696e 6773  ngs.....Holdings
+000054a0: 5769 6467 6574 0103 0000 0018 0421 043e  Widget.......!.>
+000054b0: 0445 0440 0430 043d 0438 0442 044c 002e  .E.@.0.=.8.B.L..
+000054c0: 002e 002e 0800 0000 0006 0000 0007 5361  ..............Sa
+000054d0: 7665 2e2e 2e07 0000 000e 486f 6c64 696e  ve........Holdin
+000054e0: 6773 5769 6467 6574 0103 0000 0014 0064  gsWidget.......d
+000054f0: 0064 002f 004d 004d 002f 0079 0079 0079  .d./.M.M./.y.y.y
+00005500: 0079 0800 0000 0006 0000 000a 6464 2f4d  .y..........dd/M
+00005510: 4d2f 7979 7979 0700 0000 0e48 6f6c 6469  M/yyyy.....Holdi
+00005520: 6e67 7357 6964 6765 7401 0300 0000 3404  ngsWidget.....4.
+00005530: 2204 3804 3f00 2004 2604 1100 2004 3d04  ".8.?. .&... .=.
+00005540: 3500 2004 3f04 3e04 3404 3404 3504 4004  5. .?.>.4.4.5.@.
+00005550: 3604 3804 3204 3004 3504 4204 4104 4f00  6.8.2.0.5.B.A.O.
+00005560: 3a00 2008 0000 0000 0600 0000 1c41 7373  :. ..........Ass
+00005570: 6574 2074 7970 6520 6973 6e27 7420 7375  et type isn't su
+00005580: 7070 6f72 7465 643a 2007 0000 0004 4942  pported: .....IB
+00005590: 4b52 0103 0000 0054 041a 043e 0440 043f  KR.....T...>.@.?
+000055a0: 043e 0440 0430 0442 0438 0432 043d 043e  .>.@.0.B.8.2.=.>
+000055b0: 0435 0020 0434 0435 0439 0441 0442 0432  .5. .4.5.9.A.B.2
+000055c0: 0438 0435 0020 043d 0435 0020 043f 043e  .8.5. .=.5. .?.>
+000055d0: 0434 0434 0435 0440 0436 0438 0432 0430  .4.4.5.@.6.8.2.0
+000055e0: 0435 0442 0441 044f 003a 0020 0800 0000  .5.B.A.O.:. ....
+000055f0: 0006 0000 0022 436f 7270 6f72 6174 6520  ....."Corporate 
+00005600: 6163 7469 6f6e 2069 736e 2774 2073 7570  action isn't sup
+00005610: 706f 7274 6564 3a20 0700 0000 0449 424b  ported: .....IBK
+00005620: 5201 0300 0000 4604 1d04 3504 3e04 3404  R.....F...5.>.4.
+00005630: 3d04 3e04 3704 3d04 3004 4704 3d04 3e04  =.>.7.=.0.G.=.>.
+00005640: 3500 2004 4104 3e04 3204 3f04 3004 3404  5. .A.>.2.?.0.4.
+00005650: 3504 3d04 3804 3500 2004 4104 4704 5104  5.=.8.5. .A.G.Q.
+00005660: 4204 3000 2004 3404 3b04 4f00 2008 0000  B.0. .4.;.O. ...
+00005670: 0000 0600 0000 1b4d 756c 7469 706c 6520  .......Multiple 
+00005680: 6163 636f 756e 7420 6d61 7463 6820 666f  account match fo
+00005690: 7220 0700 0000 0449 424b 5201 0300 0000  r .....IBKR.....
+000056a0: 6800 4a00 5300 4f00 4e00 2004 4204 4d04  h.J.S.O.N. .B.M.
+000056b0: 3300 2000 2700 6400 6f00 6300 7500 6d00  3. .'.d.o.c.u.m.
+000056c0: 6500 6e00 7400 2700 2004 3e04 4204 4104  e.n.t.'. .>.B.A.
+000056d0: 4304 4204 4104 4204 3204 4304 3504 4200  C.B.A.B.2.C.5.B.
+000056e0: 2004 3204 3d04 4304 4204 4004 3800 2004   .2.=.C.B.@.8. .
+000056f0: 4204 4d04 3304 3000 2000 2700 7400 6900  B.M.3.0. .'.t.i.
+00005700: 6300 6b00 6500 7400 2708 0000 0000 0600  c.k.e.t.'.......
+00005710: 0000 2a43 616e 2774 2066 696e 6420 2764  ..*Can't find 'd
+00005720: 6f63 756d 656e 7427 2074 6167 2069 6e20  ocument' tag in 
+00005730: 6a73 6f6e 2027 7469 636b 6574 2707 0000  json 'ticket'...
+00005740: 0010 496d 706f 7274 536c 6970 4469 616c  ..ImportSlipDial
+00005750: 6f67 0103 0000 0072 004a 0053 004f 004e  og.....r.J.S.O.N
+00005760: 0020 0442 044d 0433 0020 0027 006f 0070  . .B.M.3. .'.o.p
+00005770: 0065 0072 0061 0074 0069 006f 006e 0054  .e.r.a.t.i.o.n.T
+00005780: 0079 0070 0065 0027 0020 043e 0442 0441  .y.p.e.'. .>.B.A
+00005790: 0443 0442 0441 0442 0432 0443 0435 0442  .C.B.A.B.2.C.5.B
+000057a0: 0020 0432 043d 0443 0442 0440 0438 0020  . .2.=.C.B.@.8. 
+000057b0: 0442 044d 0433 0430 0020 0027 0074 0069  .B.M.3.0. .'.t.i
+000057c0: 0063 006b 0065 0074 0027 0800 0000 0006  .c.k.e.t.'......
+000057d0: 0000 002f 4361 6e27 7420 6669 6e64 2027  .../Can't find '
+000057e0: 6f70 6572 6174 696f 6e54 7970 6527 2074  operationType' t
+000057f0: 6167 2069 6e20 6a73 6f6e 2027 7469 636b  ag in json 'tick
+00005800: 6574 2707 0000 0010 496d 706f 7274 536c  et'.....ImportSl
+00005810: 6970 4469 616c 6f67 0103 0000 006a 004a  ipDialog.....j.J
+00005820: 0053 004f 004e 0020 0442 044d 0433 0020  .S.O.N. .B.M.3. 
+00005830: 0027 0072 0065 0063 0065 0069 0070 0074  .'.r.e.c.e.i.p.t
+00005840: 0027 0020 043e 0442 0441 0443 0442 0441  .'. .>.B.A.C.B.A
+00005850: 0442 0432 0443 0435 0442 0020 0432 043d  .B.2.C.5.B. .2.=
+00005860: 0443 0442 0440 0438 0020 0442 044d 0433  .C.B.@.8. .B.M.3
+00005870: 0430 0020 0027 0064 006f 0063 0075 006d  .0. .'.d.o.c.u.m
+00005880: 0065 006e 0074 0027 0800 0000 0006 0000  .e.n.t.'........
+00005890: 002b 4361 6e27 7420 6669 6e64 2027 7265  .+Can't find 're
+000058a0: 6365 6970 7427 2074 6167 2069 6e20 6a73  ceipt' tag in js
+000058b0: 6f6e 2027 646f 6375 6d65 6e74 2707 0000  on 'document'...
+000058c0: 0010 496d 706f 7274 536c 6970 4469 616c  ..ImportSlipDial
+000058d0: 6f67 0103 0000 005e 041a 0430 0442 0435  og.....^...0.B.5
+000058e0: 0433 043e 0440 0438 0438 0020 043d 0435  .3.>.@.8.8. .=.5
+000058f0: 0020 0440 0430 0441 043f 043e 0437 043d  . .@.0.A.?.>.7.=
+00005900: 0430 043d 044b 003a 0020 0054 0065 006e  .0.=.K.:. .T.e.n
+00005910: 0073 006f 0072 006c 006f 0077 0020 043d  .s.o.r.l.o.w. .=
+00005920: 0435 0020 043e 0431 043d 0430 0440 0443  .5. .>.1.=.0.@.C
+00005930: 0436 0435 043d 0800 0000 0006 0000 0036  .6.5.=.........6
+00005940: 4361 7465 676f 7269 6573 2061 7265 206e  Categories are n
+00005950: 6f74 2072 6563 6f67 6e69 7a65 643a 2054  ot recognized: T
+00005960: 656e 736f 7266 6c6f 7720 6973 206e 6f74  ensorflow is not
+00005970: 2066 6f75 6e64 0700 0000 1049 6d70 6f72   found.....Impor
+00005980: 7453 6c69 7044 6961 6c6f 6701 0300 0000  tSlipDialog.....
+00005990: 4a04 1f04 4004 3504 3204 4b04 4804 3504  J...@.5.2.K.H.5.
+000059a0: 3d04 3e00 2004 3c04 3004 3a04 4104 3804  =.>. .<.0.:.A.8.
+000059b0: 3c04 3004 3b04 4c04 3d04 3e04 3500 2004  <.0.;.L.=.>.5. .
+000059c0: 4704 3804 4104 3b04 3e00 2004 3f04 3e04  G.8.A.;.>. .?.>.
+000059d0: 3f04 4b04 4204 3e04 3a00 2e08 0000 0000  ?.K.B.>.:.......
+000059e0: 0600 0000 194d 6178 2072 6574 7279 2063  .....Max retry c
+000059f0: 6f75 6e74 2065 7863 6565 6465 642e 0700  ount exceeded...
+00005a00: 0000 1049 6d70 6f72 7453 6c69 7044 6961  ...ImportSlipDia
+00005a10: 6c6f 6701 0300 0000 4600 5100 5200 2004  log.....F.Q.R. .
+00005a20: 3a04 3e04 3400 2004 3d04 3500 2004 3e04  :.>.4. .=.5. .>.
+00005a30: 3104 3d04 3004 4004 4304 3604 3504 3d00  1.=.0.@.C.6.5.=.
+00005a40: 2004 3200 2004 3104 4304 4404 3504 4004   .2. .1.C.D.5.@.
+00005a50: 3500 2004 3e04 3104 3c04 3504 3d04 3008  5. .>.1.<.5.=.0.
+00005a60: 0000 0000 0600 0000 1e4e 6f20 5152 2063  .........No QR c
+00005a70: 6f64 6573 2066 6f75 6e64 2069 6e20 636c  odes found in cl
+00005a80: 6970 626f 6172 6407 0000 0010 496d 706f  ipboard.....Impo
+00005a90: 7274 536c 6970 4469 616c 6f67 0103 0000  rtSlipDialog....
+00005aa0: 0036 0051 0052 002d 043a 043e 0434 0020  .6.Q.R.-.:.>.4. 
+00005ab0: 0432 0020 0444 0430 0439 043b 0435 0020  .2. .D.0.9.;.5. 
+00005ac0: 043d 0435 0020 043e 0431 043d 0430 0440  .=.5. .>.1.=.0.@
+00005ad0: 0443 0436 0435 043d 0800 0000 0006 0000  .C.6.5.=........
+00005ae0: 001e 4e6f 2051 5220 636f 6465 7320 7765  ..No QR codes we
+00005af0: 7265 2066 6f75 6e64 2069 6e20 6669 6c65  re found in file
+00005b00: 0700 0000 1049 6d70 6f72 7453 6c69 7044  .....ImportSlipD
+00005b10: 6961 6c6f 6701 0300 0000 7204 1d04 3504  ialog.....r...5.
+00005b20: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
+00005b30: 2004 3404 3e04 3104 3004 3204 3804 4204   .4.>.1.0.2.8.B.
+00005b40: 4c00 2004 4704 3504 3a00 3a00 2004 3d04  L. .G.5.:.:. .=.
+00005b50: 3500 2004 4304 3a04 3004 3704 3004 3d00  5. .C.:.0.7.0.=.
+00005b60: 2004 3a04 3e04 3d04 4204 4004 3004 3304   .:.>.=.B.@.0.3.
+00005b70: 3504 3d04 4200 2004 3404 3b04 4f00 2004  5.=.B. .4.;.O. .
+00005b80: 3804 3c04 3f04 3e04 4004 4204 3008 0000  8.<.?.>.@.B.0...
+00005b90: 0000 0600 0000 414e 6f74 2070 6f73 7369  ......ANot possi
+00005ba0: 626c 6520 746f 2069 6d70 6f72 7420 736c  ble to import sl
+00005bb0: 6970 3a20 6361 6e27 7420 696d 706f 7274  ip: can't import
+00005bc0: 3a20 6e6f 2070 6565 7220 7365 7420 666f  : no peer set fo
+00005bd0: 7220 696d 706f 7274 0700 0000 1049 6d70  r import.....Imp
+00005be0: 6f72 7453 6c69 7044 6961 6c6f 6701 0300  ortSlipDialog...
+00005bf0: 0000 6604 1d04 3504 3204 3e04 3704 3c04  ..f...5.2.>.7.<.
+00005c00: 3e04 3604 3d04 3e00 2004 3404 3e04 3104  >.6.=.>. .4.>.1.
+00005c10: 3004 3204 3804 4204 4c00 2004 4704 3504  0.2.8.B.L. .G.5.
+00005c20: 3a00 3a00 2004 3d04 3500 2004 4304 3a04  :.:. .=.5. .C.:.
+00005c30: 3004 3704 3004 3d00 2004 4104 4704 3504  0.7.0.=. .A.G.5.
+00005c40: 4200 2004 3404 3b04 4f00 2004 3804 3c04  B. .4.;.O. .8.<.
+00005c50: 3f04 3e04 4004 4204 3008 0000 0000 0600  ?.>.@.B.0.......
+00005c60: 0000 364e 6f74 2070 6f73 7369 626c 6520  ..6Not possible 
+00005c70: 746f 2069 6d70 6f72 7420 736c 6970 3a20  to import slip: 
+00005c80: 6e6f 2061 6363 6f75 6e74 2073 6574 2066  no account set f
+00005c90: 6f72 2069 6d70 6f72 7407 0000 0010 496d  or import.....Im
+00005ca0: 706f 7274 536c 6970 4469 616c 6f67 0103  portSlipDialog..
+00005cb0: 0000 0078 041d 0435 0432 043e 0437 043c  ...x...5.2.>.7.<
+00005cc0: 043e 0436 043d 043e 0020 0434 043e 0431  .>.6.=.>. .4.>.1
+00005cd0: 0430 0432 0438 0442 044c 0020 0447 0435  .0.2.8.B.L. .G.5
+00005ce0: 043a 003a 0020 043a 0430 0442 0435 0433  .:.:. .:.0.B.5.3
+00005cf0: 043e 0440 0438 0438 0020 0443 043a 0430  .>.@.8.8. .C.:.0
+00005d00: 0437 0430 043d 044b 0020 043d 0435 0020  .7.0.=.K. .=.5. 
+00005d10: 0434 043b 044f 0020 0432 0441 0435 0445  .4.;.O. .2.A.5.E
+00005d20: 0020 0441 0442 0440 043e 043a 0800 0000  . .A.B.@.>.:....
+00005d30: 0006 0000 0038 4e6f 7420 706f 7373 6962  .....8Not possib
+00005d40: 6c65 2074 6f20 696d 706f 7274 2073 6c69  le to import sli
+00005d50: 703a 2073 6f6d 6520 6361 7465 676f 7269  p: some categori
+00005d60: 6573 2061 7265 206e 6f74 2073 6574 0700  es are not set..
+00005d70: 0000 1049 6d70 6f72 7453 6c69 7044 6961  ...ImportSlipDia
+00005d80: 6c6f 6701 0300 0000 5404 1d04 3504 3204  log.....T...5.2.
+00005d90: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
+00005da0: 4004 3004 4104 3f04 3e04 3704 3d04 3004  @.0.A.?.>.7.=.0.
+00005db0: 4204 4c00 2004 3f04 4004 3e04 4704 3804  B.L. .?.@.>.G.8.
+00005dc0: 4204 3004 3d04 3d04 4b04 3900 2000 5100  B.0.=.=.K.9. .Q.
+00005dd0: 5200 2d04 3a04 3e04 3400 3a00 2008 0000  R.-.:.>.4.:. ...
+00005de0: 0000 0600 0000 2b51 5220 6176 6169 6c61  ......+QR availa
+00005df0: 626c 6520 6275 7420 7061 7474 6572 6e20  ble but pattern 
+00005e00: 6973 6e27 7420 7265 636f 676e 697a 6564  isn't recognized
+00005e10: 3a20 0700 0000 1049 6d70 6f72 7453 6c69  : .....ImportSli
+00005e20: 7044 6961 6c6f 6701 0300 0000 0800 5100  pDialog.......Q.
+00005e30: 5200 3a00 2008 0000 0000 0600 0000 0451  R.:. ..........Q
+00005e40: 523a 2007 0000 0010 496d 706f 7274 536c  R: .....ImportSl
+00005e50: 6970 4469 616c 6f67 0103 0000 0030 0412  ipDialog.....0..
+00005e60: 044b 0431 0435 0440 0438 0442 0435 0020  .K.1.5.@.8.B.5. 
+00005e70: 0444 0430 0439 043b 0020 0441 0020 0051  .D.0.9.;. .A. .Q
+00005e80: 0052 002d 043a 043e 0434 043e 043c 0800  .R.-.:.>.4.>.<..
+00005e90: 0000 0006 0000 0018 5365 6c65 6374 2066  ........Select f
+00005ea0: 696c 6520 7769 7468 2051 5220 636f 6465  ile with QR code
+00005eb0: 0700 0000 1049 6d70 6f72 7453 6c69 7044  .....ImportSlipD
+00005ec0: 6961 6c6f 6701 0300 0000 4204 1204 4b04  ialog.....B...K.
+00005ed0: 3104 3504 4004 3804 4204 3500 2004 4404  1.5.@.8.B.5. .D.
+00005ee0: 3004 3904 3b00 2004 4100 2000 4a00 5300  0.9.;. .A. .J.S.
+00005ef0: 4f00 4e00 2d04 3404 3004 3d04 3d04 4b04  O.N.-.4.0.=.=.K.
+00005f00: 3c04 3800 2004 4704 3504 3a04 3008 0000  <.8. .G.5.:.0...
+00005f10: 0000 0600 0000 1f53 656c 6563 7420 6669  .......Select fi
+00005f20: 6c65 2077 6974 6820 736c 6970 204a 534f  le with slip JSO
+00005f30: 4e20 6461 7461 0700 0000 1049 6d70 6f72  N data.....Impor
+00005f40: 7453 6c69 7044 6961 6c6f 6701 0300 0000  tSlipDialog.....
+00005f50: 3204 1d04 3504 3804 3704 3204 3504 4104  2...5.8.7.2.5.A.
+00005f60: 4204 3d04 4b04 3900 2004 4204 3804 3f00  B.=.K.9. .B.8.?.
+00005f70: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
+00005f80: 3800 2008 0000 0000 0600 0000 1755 6e6b  8. ..........Unk
+00005f90: 6e6f 776e 206f 7065 7261 7469 6f6e 2074  nown operation t
+00005fa0: 7970 6520 0700 0000 1049 6d70 6f72 7453  ype .....ImportS
+00005fb0: 6c69 7044 6961 6c6f 6701 0300 0000 0600  lipDialog.......
+00005fc0: 2027 9c00 2008 0000 0000 0600 0000 0520   '.. .......... 
+00005fd0: e29e 9c20 0700 0000 0d49 6d70 6f72 7453  ... .....ImportS
+00005fe0: 6c69 7044 6c67 0103 0000 000a 0421 0447  lipDlg.......!.G
+00005ff0: 0435 0442 003a 0800 0000 0006 0000 0008  .5.B.:..........
+00006000: 4163 636f 756e 743a 0700 0000 0d49 6d70  Account:.....Imp
+00006010: 6f72 7453 6c69 7044 6c67 0103 0000 0010  ortSlipDlg......
+00006020: 0414 043e 0431 0430 0432 0438 0442 044c  ...>.1.0.2.8.B.L
+00006030: 0800 0000 0006 0000 0003 4164 6407 0000  ..........Add...
+00006040: 000d 496d 706f 7274 536c 6970 446c 6701  ..ImportSlipDlg.
+00006050: 0300 0000 0c04 2104 4304 3c04 3c04 3000  ......!.C.<.<.0.
+00006060: 3a08 0000 0000 0600 0000 0741 6d6f 756e  :..........Amoun
+00006070: 743a 0700 0000 0d49 6d70 6f72 7453 6c69  t:.....ImportSli
+00006080: 7044 6c67 0103 0000 0032 0410 0432 0442  pDlg.....2...2.B
+00006090: 043e 002d 043d 0430 0437 043d 0430 0447  .>.-.=.0.7.=.0.G
+000060a0: 0435 043d 0438 0435 0020 043a 0430 0442  .5.=.8.5. .:.0.B
+000060b0: 0435 0433 043e 0440 0438 0439 0800 0000  .5.3.>.@.8.9....
+000060c0: 0006 0000 0016 4175 746f 2d61 7373 6967  ......Auto-assig
+000060d0: 6e20 6361 7465 676f 7269 6573 0700 0000  n categories....
+000060e0: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
+000060f0: 0000 000c 041a 0430 043c 0435 0440 0430  .......0.<.5.@.0
+00006100: 0800 0000 0006 0000 0006 4361 6d65 7261  ..........Camera
+00006110: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
+00006120: 6c67 0103 0000 0010 041e 0447 0438 0441  lg.........G.8.A
+00006130: 0442 0438 0442 044c 0800 0000 0006 0000  .B.8.B.L........
+00006140: 0005 436c 6561 7207 0000 000d 496d 706f  ..Clear.....Impo
+00006150: 7274 536c 6970 446c 6701 0300 0000 0e04  rtSlipDlg.......
+00006160: 1704 3004 3a04 4004 4b04 4204 4c08 0000  ..0.:.@.K.B.L...
+00006170: 0000 0600 0000 0543 6c6f 7365 0700 0000  .......Close....
+00006180: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
+00006190: 0000 001a 0414 0430 0442 0430 0020 002f  .......0.B.0. ./
+000061a0: 0020 0412 0440 0435 043c 044f 003a 0800  . ...@.5.<.O.:..
+000061b0: 0000 0006 0000 000c 4461 7465 202f 2054  ........Date / T
+000061c0: 696d 653a 0700 0000 0d49 6d70 6f72 7453  ime:.....ImportS
+000061d0: 6c69 7044 6c67 0103 0000 0016 0414 0430  lipDlg.........0
+000061e0: 0442 0430 002f 0412 0440 0435 043c 044f  .B.0./...@.5.<.O
+000061f0: 003a 0800 0000 0006 0000 000a 4461 7465  .:..........Date
+00006200: 2f54 696d 653a 0700 0000 0d49 6d70 6f72  /Time:.....Impor
+00006210: 7453 6c69 7044 6c67 0103 0000 0006 0424  tSlipDlg.......$
+00006220: 0414 003a 0800 0000 0006 0000 0003 4644  ...:..........FD
+00006230: 3a07 0000 000d 496d 706f 7274 536c 6970  :.....ImportSlip
+00006240: 446c 6701 0300 0000 0604 2404 1d00 3a08  Dlg.......$...:.
+00006250: 0000 0000 0600 0000 0346 4e3a 0700 0000  .........FN:....
+00006260: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
+00006270: 0000 0006 0424 041f 003a 0800 0000 0006  .....$...:......
+00006280: 0000 0003 4650 3a07 0000 000d 496d 706f  ....FP:.....Impo
+00006290: 7274 536c 6970 446c 6701 0300 0000 2604  rtSlipDlg.....&.
+000062a0: 2104 3a04 3004 3d04 3804 4004 3e04 3204  !.:.0.=.8.@.>.2.
+000062b0: 3004 4204 4c00 2004 3a04 3004 3c04 3504  0.B.L. .:.0.<.5.
+000062c0: 4004 3e04 3908 0000 0000 0600 0000 0f47  @.>.9..........G
+000062d0: 6574 2066 726f 6d20 6361 6d65 7261 0700  et from camera..
+000062e0: 0000 0d49 6d70 6f72 7453 6c69 7044 6c67  ...ImportSlipDlg
+000062f0: 0103 0000 0024 041f 043e 043b 0443 0447  .....$...>.;.C.G
+00006300: 0438 0442 044c 0020 0438 0437 0020 0431  .8.B.L. .8.7. .1
+00006310: 0443 0444 0435 0440 0430 0800 0000 0006  .C.D.5.@.0......
+00006320: 0000 0012 4765 7420 6672 6f6d 2063 6c69  ....Get from cli
+00006330: 7062 6f61 7264 0700 0000 0d49 6d70 6f72  pboard.....Impor
+00006340: 7453 6c69 7044 6c67 0103 0000 0030 041f  tSlipDlg.....0..
+00006350: 043e 043b 0443 0447 0438 0442 044c 0020  .>.;.C.G.8.B.L. 
+00006360: 0447 0435 043a 0020 0441 0020 0441 0430  .G.5.:. .A. .A.0
+00006370: 0439 0442 0430 0020 0424 041d 0421 0800  .9.B.0. .$...!..
+00006380: 0000 0006 0000 0016 4765 7420 736c 6970  ........Get slip
+00006390: 2066 726f 6d20 696e 7465 726e 6574 0700   from internet..
+000063a0: 0000 0d49 6d70 6f72 7453 6c69 7044 6c67  ...ImportSlipDlg
+000063b0: 0103 0000 0016 0418 043c 043f 043e 0440  .........<.?.>.@
+000063c0: 0442 0020 0447 0435 043a 0430 0800 0000  .B. .G.5.:.0....
+000063d0: 0006 0000 000b 496d 706f 7274 2053 6c69  ......Import Sli
+000063e0: 7007 0000 000d 496d 706f 7274 536c 6970  p.....ImportSlip
+000063f0: 446c 6701 0300 0000 0e04 2104 4204 4004  Dlg.......!.B.@.
+00006400: 3e04 3a04 3800 3a08 0000 0000 0600 0000  >.:.8.:.........
+00006410: 064c 696e 6573 3a07 0000 000d 496d 706f  .Lines:.....Impo
+00006420: 7274 536c 6970 446c 6701 0300 0000 2404  rtSlipDlg.....$.
+00006430: 1704 3004 3304 4004 4304 3704 3804 4204  ..0.3.@.C.7.8.B.
+00006440: 4c00 2004 3804 3700 2004 4404 3004 3904  L. .8.7. .D.0.9.
+00006450: 3b04 3008 0000 0000 0600 0000 0e4c 6f61  ;.0..........Loa
+00006460: 6420 6672 6f6d 2066 696c 6507 0000 000d  d from file.....
+00006470: 496d 706f 7274 536c 6970 446c 6701 0300  ImportSlipDlg...
+00006480: 0000 3604 1704 3004 3304 4304 3704 3804  ..6...0.3.C.7.8.
+00006490: 4204 4c00 2004 4704 3504 3a04 3000 2004  B.L. .G.5.:.0. .
+000064a0: 3804 3700 2000 4a00 5300 4f00 4e00 2d04  8.7. .J.S.O.N.-.
+000064b0: 4404 3004 3904 3b04 3008 0000 0000 0600  D.0.9.;.0.......
+000064c0: 0000 184c 6f61 6420 736c 6970 2066 726f  ...Load slip fro
+000064d0: 6d20 4a53 4f4e 2066 696c 6507 0000 000d  m JSON file.....
+000064e0: 496d 706f 7274 536c 6970 446c 6701 0300  ImportSlipDlg...
+000064f0: 0000 1604 1a04 3e04 3d04 4204 4004 3004  ......>.=.B.@.0.
+00006500: 3304 3504 3d04 4200 3a08 0000 0000 0600  3.5.=.B.:.......
+00006510: 0000 0550 6565 723a 0700 0000 0d49 6d70  ...Peer:.....Imp
+00006520: 6f72 7453 6c69 7044 6c67 0103 0000 000e  ortSlipDlg......
+00006530: 041f 043e 043a 0443 043f 043a 0430 0800  ...>.:.C.?.:.0..
+00006540: 0000 0006 0000 0008 5075 7263 6861 7365  ........Purchase
+00006550: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
+00006560: 6c67 0103 0000 000c 0051 0052 002d 043a  lg.......Q.R.-.:
+00006570: 043e 0434 0800 0000 0006 0000 0007 5152  .>.4..........QR
+00006580: 2d63 6f64 6507 0000 000d 496d 706f 7274  -code.....Import
+00006590: 536c 6970 446c 6701 0300 0000 0e04 1204  SlipDlg.........
+000065a0: 3e04 3704 3204 4004 3004 4208 0000 0000  >.7.2.@.0.B.....
+000065b0: 0600 0000 0652 6574 7572 6e07 0000 000d  .....Return.....
+000065c0: 496d 706f 7274 536c 6970 446c 6701 0300  ImportSlipDlg...
+000065d0: 0000 2e04 2304 4104 4204 3004 3d04 3e04  ....#.A.B.0.=.>.
+000065e0: 3204 3804 4204 4c00 2004 4204 4d04 3300  2.8.B.L. .B.M.3.
+000065f0: 2004 3404 3b04 4f00 2004 3204 4104 3504   .4.;.O. .2.A.5.
+00006600: 4508 0000 0000 0600 0000 1553 6574 2054  E..........Set T
+00006610: 6167 2066 6f72 2061 6c6c 206c 696e 6573  ag for all lines
+00006620: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
+00006630: 6c67 0103 0000 0006 0427 0435 043a 0800  lg.......'.5.:..
+00006640: 0000 0006 0000 0004 536c 6970 0700 0000  ........Slip....
+00006650: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
+00006660: 0000 0016 0414 0430 043d 043d 044b 0435  .......0.=.=.K.5
+00006670: 0020 0447 0435 043a 0430 0800 0000 0006  . .G.5.:.0......
+00006680: 0000 0009 536c 6970 2064 6174 6107 0000  ....Slip data...
+00006690: 000d 496d 706f 7274 536c 6970 446c 6701  ..ImportSlipDlg.
+000066a0: 0300 0000 1c04 1704 3004 3a04 4004 4b04  ........0.:.@.K.
+000066b0: 4204 4c00 2004 3a04 3004 3c04 3504 4004  B.L. .:.0.<.5.@.
+000066c0: 4308 0000 0000 0600 0000 0b53 746f 7020  C..........Stop 
+000066d0: 6361 6d65 7261 0700 0000 0d49 6d70 6f72  camera.....Impor
+000066e0: 7453 6c69 7044 6c67 0103 0000 0008 0422  tSlipDlg......."
+000066f0: 0438 043f 003a 0800 0000 0006 0000 0005  .8.?.:..........
+00006700: 5479 7065 3a07 0000 000d 496d 706f 7274  Type:.....Import
+00006710: 536c 6970 446c 6701 0300 0000 2600 6400  SlipDlg.....&.d.
+00006720: 6400 2f00 4d00 4d00 2f00 7900 7900 7900  d./.M.M./.y.y.y.
+00006730: 7900 2000 6800 6800 3a00 6d00 6d00 3a00  y. .h.h.:.m.m.:.
+00006740: 7300 7308 0000 0000 0600 0000 1364 642f  s.s..........dd/
+00006750: 4d4d 2f79 7979 7920 6868 3a6d 6d3a 7373  MM/yyyy hh:mm:ss
+00006760: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
+00006770: 6c67 0103 0000 0066 041d 0435 0432 043e  lg.....f...5.2.>
+00006780: 0437 043c 043e 0436 043d 043e 0020 043e  .7.<.>.6.=.>. .>
+00006790: 0431 0440 0430 0431 043e 0442 0430 0442  .1.@.0.1.>.B.0.B
+000067a0: 044c 0020 043e 043f 0435 0440 0430 0446  .L. .>.?.5.@.0.F
+000067b0: 0438 044e 0020 0431 0435 0437 0020 0434  .8.N. .1.5.7. .4
+000067c0: 0435 0442 0430 043b 044c 043d 044b 0445  .5.B.0.;.L.=.K.E
+000067d0: 0020 0434 0430 043d 043d 044b 0445 0800  . .4.0.=.=.K.E..
+000067e0: 0000 0006 0000 0027 4361 6e27 7420 7072  .......'Can't pr
+000067f0: 6f63 6573 7320 6f70 6572 6174 696f 6e20  ocess operation 
+00006800: 7769 7468 6f75 7420 6465 7461 696c 7307  without details.
+00006810: 0000 000e 496e 636f 6d65 5370 656e 6469  ....IncomeSpendi
+00006820: 6e67 0103 0000 000c 041a 0443 0440 0441  ng.........C.@.A
+00006830: 003a 0020 0800 0000 0006 0000 0006 5261  .:. ..........Ra
+00006840: 7465 3a20 0700 0000 0e49 6e63 6f6d 6553  te: .....IncomeS
+00006850: 7065 6e64 696e 6701 0300 0000 1c04 1404  pending.........
+00006860: 3e04 4504 3e04 3404 4b00 2004 3800 2004  >.E.>.4.K. .8. .
+00006870: 2204 4004 3004 4204 4b08 0000 0000 0600  ".@.0.B.K.......
+00006880: 0000 1149 6e63 6f6d 6520 2620 5370 656e  ...Income & Spen
+00006890: 6469 6e67 0700 0000 1449 6e63 6f6d 6553  ding.....IncomeS
+000068a0: 7065 6e64 696e 6752 6570 6f72 7401 0300  pendingReport...
+000068b0: 0000 0a04 1804 2204 1e04 1304 1e08 0000  ......".........
+000068c0: 0000 0600 0000 0554 4f54 414c 0700 0000  .......TOTAL....
+000068d0: 1949 6e63 6f6d 6553 7065 6e64 696e 6752  .IncomeSpendingR
+000068e0: 6570 6f72 744d 6f64 656c 0103 0000 000e  eportModel......
+000068f0: 0412 0430 043b 044e 0442 0430 003a 0800  ...0.;.N.B.0.:..
+00006900: 0000 0006 0000 0009 4375 7272 656e 6379  ........Currency
+00006910: 3a07 0000 001a 496e 636f 6d65 5370 656e  :.....IncomeSpen
+00006920: 6469 6e67 5265 706f 7274 5769 6467 6574  dingReportWidget
+00006930: 0103 0000 001c 0414 043e 0445 043e 0434  .........>.E.>.4
+00006940: 044b 0020 0438 0020 0422 0440 0430 0442  .K. .8. .".@.0.B
+00006950: 044b 0800 0000 0006 0000 0011 496e 636f  .K..........Inco
+00006960: 6d65 2026 2053 7065 6e64 696e 6707 0000  me & Spending...
+00006970: 001a 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
+00006980: 5265 706f 7274 5769 6467 6574 0103 0000  ReportWidget....
+00006990: 0012 041f 043e 043c 0435 0441 044f 0447  .....>.<.5.A.O.G
+000069a0: 043d 043e 0800 0000 0006 0000 0007 4d6f  .=.>..........Mo
+000069b0: 6e74 686c 7907 0000 001a 496e 636f 6d65  nthly.....Income
+000069c0: 5370 656e 6469 6e67 5265 706f 7274 5769  SpendingReportWi
+000069d0: 6467 6574 0103 0000 001c 041f 0435 0440  dget.........5.@
+000069e0: 0438 043e 0434 0438 0447 043d 043e 0441  .8.>.4.8.G.=.>.A
+000069f0: 0442 044c 003a 0800 0000 0006 0000 000c  .B.L.:..........
+00006a00: 5065 7269 6f64 6963 6974 793a 0700 0000  Periodicity:....
+00006a10: 1a49 6e63 6f6d 6553 7065 6e64 696e 6752  .IncomeSpendingR
+00006a20: 6570 6f72 7457 6964 6765 7401 0300 0000  eportWidget.....
+00006a30: 1804 2104 3e04 4504 4004 3004 3d04 3804  ..!.>.E.@.0.=.8.
+00006a40: 4204 4c00 2e00 2e00 2e08 0000 0000 0600  B.L.............
+00006a50: 0000 0753 6176 652e 2e2e 0700 0000 1a49  ...Save........I
+00006a60: 6e63 6f6d 6553 7065 6e64 696e 6752 6570  ncomeSpendingRep
+00006a70: 6f72 7457 6964 6765 7401 0300 0000 1404  ortWidget.......
+00006a80: 1f04 3e04 3d04 3504 3404 3504 3b04 4c04  ..>.=.5.4.5.;.L.
+00006a90: 3d04 3e08 0000 0000 0600 0000 0657 6565  =.>..........Wee
+00006aa0: 6b6c 7907 0000 001a 496e 636f 6d65 5370  kly.....IncomeSp
+00006ab0: 656e 6469 6e67 5265 706f 7274 5769 6467  endingReportWidg
+00006ac0: 6574 0103 0000 001c 0414 043e 0445 043e  et.........>.E.>
+00006ad0: 0434 044b 0020 0438 0020 0422 0440 0430  .4.K. .8. .".@.0
+00006ae0: 0442 044b 0800 0000 0006 0000 0011 496e  .B.K..........In
+00006af0: 636f 6d65 2026 2053 7065 6e64 696e 6707  come & Spending.
+00006b00: 0000 001a 496e 636f 6d65 5370 656e 6469  ....IncomeSpendi
+00006b10: 6e67 5265 706f 7274 5769 6e64 6f77 0103  ngReportWindow..
+00006b20: 0000 0022 041f 043e 043a 0430 0437 0430  ..."...>.:.0.7.0
+00006b30: 0442 044c 0020 043e 043f 0435 0440 0430  .B.L. .>.?.5.@.0
+00006b40: 0446 0438 0438 0800 0000 0006 0000 000f  .F.8.8..........
+00006b50: 5368 6f77 206f 7065 7261 7469 6f6e 7307  Show operations.
+00006b60: 0000 001a 496e 636f 6d65 5370 656e 6469  ....IncomeSpendi
+00006b70: 6e67 5265 706f 7274 5769 6e64 6f77 0103  ngReportWindow..
+00006b80: 0000 0008 0421 0447 0435 0442 0800 0000  .....!.G.5.B....
+00006b90: 0006 0000 0007 4163 636f 756e 7407 0000  ......Account...
+00006ba0: 0014 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
+00006bb0: 5769 6467 6574 0103 0000 0032 0414 043e  Widget.....2...>
+00006bc0: 0431 0430 0432 0438 0442 044c 0020 0434  .1.0.2.8.B.L. .4
+00006bd0: 0435 0442 0430 043b 044c 043d 0443 044e  .5.B.0.;.L.=.C.N
+00006be0: 0020 0437 0430 043f 0438 0441 044c 0800  . .7.0.?.8.A.L..
+00006bf0: 0000 0006 0000 000a 4164 6420 6465 7461  ........Add deta
+00006c00: 696c 0700 0000 1449 6e63 6f6d 6553 7065  il.....IncomeSpe
+00006c10: 6e64 696e 6757 6964 6765 7401 0300 0000  ndingWidget.....
+00006c20: 3804 2104 3a04 3e04 3f04 3804 4004 3e04  8.!.:.>.?.8.@.>.
+00006c30: 3204 3004 4204 4c00 2004 3404 3504 4204  2.0.B.L. .4.5.B.
+00006c40: 3004 3b04 4c04 3d04 4304 4e00 2004 3704  0.;.L.=.C.N. .7.
+00006c50: 3004 3f04 3804 4104 4c08 0000 0000 0600  0.?.8.A.L.......
+00006c60: 0000 0b43 6f70 7920 6465 7461 696c 0700  ...Copy detail..
+00006c70: 0000 1449 6e63 6f6d 6553 7065 6e64 696e  ...IncomeSpendin
+00006c80: 6757 6964 6765 7401 0300 0000 1404 1404  gWidget.........
+00006c90: 3004 4204 3000 2f04 1204 4004 3504 3c04  0.B.0./...@.5.<.
+00006ca0: 4f08 0000 0000 0600 0000 0944 6174 652f  O..........Date/
+00006cb0: 5469 6d65 0700 0000 1449 6e63 6f6d 6553  Time.....IncomeS
+00006cc0: 7065 6e64 696e 6757 6964 6765 7401 0300  pendingWidget...
+00006cd0: 0000 0c04 1404 3504 4204 3004 3b04 3808  ......5.B.0.;.8.
+00006ce0: 0000 0000 0600 0000 0744 6574 6169 6c73  .........Details
+00006cf0: 0700 0000 1449 6e63 6f6d 6553 7065 6e64  .....IncomeSpend
+00006d00: 696e 6757 6964 6765 7401 0300 0000 4404  ingWidget.....D.
+00006d10: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
+00006d20: 3d04 3e00 2004 3404 3e04 3104 3004 3204  =.>. .4.>.1.0.2.
+00006d30: 3804 4204 4c00 2004 3d04 3e04 3204 4304  8.B.L. .=.>.2.C.
+00006d40: 4e00 2004 3704 3004 3f04 3804 4104 4c00  N. .7.0.?.8.A.L.
+00006d50: 3a00 2008 0000 0000 0600 0000 1a46 6169  :. ..........Fai
+00006d60: 6c65 6420 746f 2061 6464 206e 6577 2072  led to add new r
+00006d70: 6563 6f72 643a 2007 0000 0014 496e 636f  ecord: .....Inco
+00006d80: 6d65 5370 656e 6469 6e67 5769 6467 6574  meSpendingWidget
+00006d90: 0103 0000 001c 0414 043e 0445 043e 0434  .........>.E.>.4
+00006da0: 0020 002f 0020 0420 0430 0441 0445 043e  . ./. . .0.A.E.>
+00006db0: 0434 0800 0000 0006 0000 0011 496e 636f  .4..........Inco
+00006dc0: 6d65 202f 2053 7065 6e64 696e 6707 0000  me / Spending...
+00006dd0: 0014 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
+00006de0: 5769 6467 6574 0103 0000 0014 041f 0440  Widget.........@
+00006df0: 0438 043c 0435 0447 0430 043d 0438 0435  .8.<.5.G.0.=.8.5
+00006e00: 0800 0000 0006 0000 0004 4e6f 7465 0700  ..........Note..
+00006e10: 0000 1449 6e63 6f6d 6553 7065 6e64 696e  ...IncomeSpendin
+00006e20: 6757 6964 6765 7401 0300 0000 4804 1e04  gWidget.....H...
+00006e30: 4804 3804 3104 3a04 3000 2004 3f04 4004  H.8.1.:.0. .?.@.
+00006e40: 3800 2004 3704 3004 3f04 3804 4104 3800  8. .7.0.?.8.A.8.
+00006e50: 2004 3404 3504 4204 3004 3b04 3504 3900   .4.5.B.0.;.5.9.
+00006e60: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
+00006e70: 3800 3a00 2008 0000 0000 0600 0000 214f  8.:. .........!O
+00006e80: 7065 7261 7469 6f6e 2064 6574 6169 6c73  peration details
+00006e90: 2073 7562 6d69 7420 6661 696c 6564 3a20   submit failed: 
+00006ea0: 0700 0000 1449 6e63 6f6d 6553 7065 6e64  .....IncomeSpend
+00006eb0: 696e 6757 6964 6765 7401 0300 0000 3804  ingWidget.....8.
+00006ec0: 1e04 4804 3804 3104 3a04 3000 2004 3f04  ..H.8.1.:.0. .?.
+00006ed0: 4004 3800 2004 3704 3004 3f04 3804 4104  @.8. .7.0.?.8.A.
+00006ee0: 3800 2004 3e04 3f04 3504 4004 3004 4604  8. .>.?.5.@.0.F.
+00006ef0: 3804 3800 3a00 2008 0000 0000 0600 0000  8.8.:. .........
+00006f00: 194f 7065 7261 7469 6f6e 2073 7562 6d69  .Operation submi
+00006f10: 7420 6661 696c 6564 3a20 0700 0000 1449  t failed: .....I
+00006f20: 6e63 6f6d 6553 7065 6e64 696e 6757 6964  ncomeSpendingWid
+00006f30: 6765 7401 0300 0000 2004 1e04 3f04 3b04  get..... ...?.;.
+00006f40: 3004 4204 3000 2004 3200 2004 3204 3004  0.B.0. .2. .2.0.
+00006f50: 3b04 4e04 4204 3500 3a08 0000 0000 0600  ;.N.B.5.:.......
+00006f60: 0000 1950 6169 6420 696e 2066 6f72 6569  ...Paid in forei
+00006f70: 676e 2063 7572 7265 6e63 793a 0700 0000  gn currency:....
+00006f80: 1449 6e63 6f6d 6553 7065 6e64 696e 6757  .IncomeSpendingW
+00006f90: 6964 6765 7401 0300 0000 1404 1a04 3e04  idget.........>.
+00006fa0: 3d04 4204 4004 3004 3304 3504 3d04 4208  =.B.@.0.3.5.=.B.
+00006fb0: 0000 0000 0600 0000 0450 6565 7207 0000  .........Peer...
+00006fc0: 0014 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
+00006fd0: 5769 6467 6574 0103 0000 0030 0423 0434  Widget.....0.#.4
+00006fe0: 0430 043b 0438 0442 044c 0020 0434 0435  .0.;.8.B.L. .4.5
+00006ff0: 0442 0430 043b 044c 043d 0443 044e 0020  .B.0.;.L.=.C.N. 
+00007000: 0437 0430 043f 0438 0441 044c 0800 0000  .7.0.?.8.A.L....
+00007010: 0006 0000 000d 5265 6d6f 7665 2064 6574  ......Remove det
+00007020: 6169 6c07 0000 0014 496e 636f 6d65 5370  ail.....IncomeSp
+00007030: 656e 6469 6e67 5769 6467 6574 0103 0000  endingWidget....
+00007040: 000c 0026 0421 0447 0435 0442 0430 0800  ...&.!.G.5.B.0..
+00007050: 0000 0006 0000 0009 2641 6363 6f75 6e74  ........&Account
+00007060: 7307 0000 000e 4a41 4c5f 4d61 696e 5769  s.....JAL_MainWi
+00007070: 6e64 6f77 0103 0000 0012 0026 0411 044d  ndow.......&...M
+00007080: 043a 0430 043f 002e 002e 002e 0800 0000  .:.0.?..........
+00007090: 0006 0000 000a 2642 6163 6b75 702e 2e2e  ......&Backup...
+000070a0: 0700 0000 0e4a 414c 5f4d 6169 6e57 696e  .....JAL_MainWin
+000070b0: 646f 7701 0300 0000 1e00 2604 1104 3004  dow.......&...0.
+000070c0: 3704 3e04 3204 3004 4f00 2004 3204 3004  7.>.2.0.O. .2.0.
+000070d0: 3b04 4e04 4204 3008 0000 0000 0600 0000  ;.N.B.0.........
+000070e0: 0e26 4261 7365 2043 7572 7265 6e63 7907  .&Base Currency.
+000070f0: 0000 000e 4a41 4c5f 4d61 696e 5769 6e64  ....JAL_MainWind
+00007100: 6f77 0103 0000 0014 0026 041a 0430 0442  ow.......&...0.B
+00007110: 0435 0433 043e 0440 0438 0438 0800 0000  .5.3.>.@.8.8....
+00007120: 0006 0000 000b 2643 6174 6567 6f72 6965  ......&Categorie
+00007130: 7307 0000 000e 4a41 4c5f 4d61 696e 5769  s.....JAL_MainWi
+00007140: 6e64 6f77 0103 0000 000e 0026 0414 0430  ndow.......&...0
+00007150: 043d 043d 044b 0435 0800 0000 0006 0000  .=.=.K.5........
+00007160: 0005 2644 6174 6107 0000 000e 4a41 4c5f  ..&Data.....JAL_
+00007170: 4d61 696e 5769 6e64 6f77 0103 0000 000c  MainWindow......
+00007180: 0026 0412 044b 0445 043e 0434 0800 0000  .&...K.E.>.4....
+00007190: 0006 0000 0005 2645 7869 7407 0000 000e  ......&Exit.....
+000071a0: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
+000071b0: 0000 0010 0026 042d 043a 0441 043f 043e  .....&.-.:.A.?.>
+000071c0: 0440 0442 0800 0000 0006 0000 0007 2645  .@.B..........&E
+000071d0: 7870 6f72 7407 0000 000e 4a41 4c5f 4d61  xport.....JAL_Ma
+000071e0: 696e 5769 6e64 6f77 0103 0000 000e 0026  inWindow.......&
+000071f0: 0418 043c 043f 043e 0440 0442 0800 0000  ...<.?.>.@.B....
+00007200: 0006 0000 0007 2649 6d70 6f72 7407 0000  ......&Import...
+00007210: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
+00007220: 0103 0000 0012 0026 041e 0441 043d 043e  .......&...A.=.>
+00007230: 0432 043d 043e 0435 0800 0000 0006 0000  .2.=.>.5........
+00007240: 0005 264d 6169 6e07 0000 000e 4a41 4c5f  ..&Main.....JAL_
+00007250: 4d61 696e 5769 6e64 6f77 0103 0000 0012  MainWindow......
+00007260: 0026 041e 043f 0435 0440 0430 0446 0438  .&...?.5.@.0.F.8
+00007270: 0438 0800 0000 0006 0000 000b 264f 7065  .8..........&Ope
+00007280: 7261 7469 6f6e 7307 0000 000e 4a41 4c5f  rations.....JAL_
+00007290: 4d61 696e 5769 6e64 6f77 0103 0000 0018  MainWindow......
+000072a0: 041a 0026 043e 043d 0442 0440 0430 0433  ...&.>.=.B.@.0.3
+000072b0: 0435 043d 0442 044b 0800 0000 0006 0000  .5.=.B.K........
+000072c0: 0006 2650 6565 7273 0700 0000 0e4a 414c  ..&Peers.....JAL
+000072d0: 5f4d 6169 6e57 696e 646f 7701 0300 0000  _MainWindow.....
+000072e0: 1400 2604 1a04 3e04 4204 3804 4004 3e04  ..&...>.B.8.@.>.
+000072f0: 3204 3a04 3808 0000 0000 0600 0000 0726  2.:.8..........&
+00007300: 5175 6f74 6573 0700 0000 0e4a 414c 5f4d  Quotes.....JAL_M
+00007310: 6169 6e57 696e 646f 7701 0300 0000 1a00  ainWindow.......
+00007320: 2604 1a04 3e04 4204 3804 4004 3e04 3204  &...>.B.8.@.>.2.
+00007330: 3a04 3800 2e00 2e00 2e08 0000 0000 0600  :.8.............
+00007340: 0000 0a26 5175 6f74 6573 2e2e 2e07 0000  ...&Quotes......
+00007350: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
+00007360: 0103 0000 000e 0026 041e 0442 0447 0435  .......&...B.G.5
+00007370: 0442 044b 0800 0000 0006 0000 0008 2652  .B.K..........&R
+00007380: 6570 6f72 7473 0700 0000 0e4a 414c 5f4d  eports.....JAL_M
+00007390: 6169 6e57 696e 646f 7701 0300 0000 2400  ainWindow.....$.
+000073a0: 2604 1204 3e04 4104 4104 4204 3004 3d04  &...>.A.A.B.0.=.
+000073b0: 3e04 3204 3b04 3504 3d04 3804 3500 2e00  >.2.;.5.=.8.5...
+000073c0: 2e00 2e08 0000 0000 0600 0000 0b26 5265  .............&Re
+000073d0: 7374 6f72 652e 2e2e 0700 0000 0e4a 414c  store........JAL
+000073e0: 5f4d 6169 6e57 696e 646f 7701 0300 0000  _MainWindow.....
+000073f0: 0c00 2604 1e04 4204 4704 5104 4208 0000  ..&...B.G.Q.B...
+00007400: 0000 0600 0000 0a26 5374 6174 656d 656e  .......&Statemen
+00007410: 7407 0000 000e 4a41 4c5f 4d61 696e 5769  t.....JAL_MainWi
+00007420: 6e64 6f77 0103 0000 000a 0026 0422 044d  ndow.......&.".M
+00007430: 0433 0438 0800 0000 0006 0000 0005 2654  .3.8..........&T
+00007440: 6167 7307 0000 000e 4a41 4c5f 4d61 696e  ags.....JAL_Main
+00007450: 5769 6e64 6f77 0103 0000 001c 0026 0426  Window.......&.&
+00007460: 0435 043d 043d 044b 0435 0020 0431 0443  .5.=.=.K.5. .1.C
+00007470: 043c 0430 0433 0438 0800 0000 0006 0000  .<.0.3.8........
+00007480: 0007 4126 7373 6574 7307 0000 000e 4a41  ..A&ssets.....JA
+00007490: 4c5f 4d61 696e 5769 6e64 6f77 0103 0000  L_MainWindow....
+000074a0: 004e 041e 0442 0447 0435 0442 0020 043e  .N...B.G.5.B. .>
+000074b0: 0020 0026 0434 0432 0438 0436 0435 043d  . .&.4.2.8.6.5.=
+000074c0: 0438 044f 0445 0020 043f 043e 0020 0437  .8.O.E. .?.>. .7
+000074d0: 0430 0440 0443 0431 0435 0436 043d 044b  .0.@.C.1.5.6.=.K
+000074e0: 043c 0020 0441 0447 0435 0442 0430 043c  .<. .A.G.5.B.0.<
+000074f0: 0800 0000 0006 0000 001d 466f 7265 6967  ..........Foreig
+00007500: 6e20 6163 636f 756e 7473 2026 666c 6f77  n accounts &flow
+00007510: 2072 6570 6f72 7407 0000 000e 4a41 4c5f   report.....JAL_
+00007520: 4d61 696e 5769 6e64 6f77 0103 0000 003e  MainWindow.....>
+00007530: 0418 043d 0432 0435 0441 0442 0438 0446  ...=.2.5.A.B.8.F
+00007540: 0438 043e 043d 043d 044b 0439 0020 0026  .8.>.=.=.K.9. .&
+00007550: 043d 0430 043b 043e 0433 043e 0432 044b  .=.0.;.>.3.>.2.K
+00007560: 0439 0020 043e 0442 0447 0435 0442 0800  .9. .>.B.G.5.B..
+00007570: 0000 0006 0000 0016 496e 7665 7374 6d65  ........Investme
+00007580: 6e74 2026 7461 7820 7265 706f 7274 0700  nt &tax report..
+00007590: 0000 0e4a 414c 5f4d 6169 6e57 696e 646f  ...JAL_MainWindo
+000075a0: 7701 0300 0000 0a00 2604 2f04 3704 4b04  w.......&./.7.K.
+000075b0: 3a08 0000 0000 0600 0000 094c 2661 6e67  :..........L&ang
+000075c0: 7561 6765 0700 0000 0e4a 414c 5f4d 6169  uage.....JAL_Mai
+000075d0: 6e57 696e 646f 7701 0300 0000 2a04 1f04  nWindow.....*...
+000075e0: 3504 4004 3504 4104 4704 3804 4204 3004  5.@.5.A.G.8.B.0.
+000075f0: 4204 4c00 2000 2604 3804 4204 3e04 3304  B.L. .&.8.B.>.3.
+00007600: 3800 2e00 2e00 2e08 0000 0000 0600 0000  8...............
+00007610: 1352 652d 6275 696c 6420 264c 6564 6765  .Re-build &Ledge
+00007620: 722e 2e2e 0700 0000 0e4a 414c 5f4d 6169  r........JAL_Mai
+00007630: 6e57 696e 646f 7701 0300 0000 1604 2704  nWindow.......'.
+00007640: 3504 3a00 2000 5b00 5200 5500 5d00 2e00  5.:. .[.R.U.]...
+00007650: 2e00 2e08 0000 0000 0600 0000 0c53 6c69  .............Sli
+00007660: 7020 5b52 555d 2e2e 2e07 0000 000e 4a41  p [RU]........JA
+00007670: 4c5f 4d61 696e 5769 6e64 6f77 0103 0000  L_MainWindow....
+00007680: 0006 006a 0061 006c 0800 0000 0006 0000  ...j.a.l........
+00007690: 0003 6a61 6c07 0000 000e 4a41 4c5f 4d61  ..jal.....JAL_Ma
+000076a0: 696e 5769 6e64 6f77 0103 0000 0020 0411  inWindow..... ..
+000076b0: 0430 043d 043a 0020 0434 043b 044f 0020  .0.=.:. .4.;.O. 
+000076c0: 0441 0447 0435 0442 0430 0020 2116 0800  .A.G.5.B.0. !...
+000076d0: 0000 0006 0000 0012 4261 6e6b 2066 6f72  ........Bank for
+000076e0: 2061 6363 6f75 6e74 2023 0700 0000 0a4a   account #.....J
+000076f0: 616c 4163 636f 756e 7401 0300 0000 2a04  alAccount.....*.
+00007700: 2104 4204 4004 3004 3d04 3000 2004 3e04  !.B.@.0.=.0. .>.
+00007710: 3104 3d04 3e04 3204 3b04 5104 3d04 3000  1.=.>.2.;.Q.=.0.
+00007720: 2004 3404 3b04 4f00 2008 0000 0000 0600   .4.;.O. .......
+00007730: 0000 1443 6f75 6e74 7279 2075 7064 6174  ...Country updat
+00007740: 6564 2066 6f72 2007 0000 0008 4a61 6c41  ed for .....JalA
+00007750: 7373 6574 0103 0000 002a 041a 043e 0442  sset.....*...>.B
+00007760: 0438 0440 043e 0432 043a 0438 0020 043e  .8.@.>.2.:.8. .>
+00007770: 0431 043d 043e 0432 043b 0435 043d 044b  .1.=.>.2.;.5.=.K
+00007780: 003a 0020 0800 0000 0006 0000 0019 5175  .:. ..........Qu
+00007790: 6f74 6174 696f 6e73 2077 6572 6520 7570  otations were up
+000077a0: 6461 7465 643a 2007 0000 0008 4a61 6c41  dated: .....JalA
+000077b0: 7373 6574 0103 0000 0046 0420 0435 0433  sset.....F. .5.3
+000077c0: 0438 0441 0442 0440 0430 0446 0438 043e  .8.A.B.@.0.F.8.>
+000077d0: 043d 043d 044b 0439 0020 043d 043e 043c  .=.=.K.9. .=.>.<
+000077e0: 0435 0440 0020 043e 0431 043d 043e 0432  .5.@. .>.1.=.>.2
+000077f0: 043b 0451 043d 0020 0434 043b 044f 0020  .;.Q.=. .4.;.O. 
+00007800: 0800 0000 0006 0000 0017 5265 672e 6e75  ..........Reg.nu
+00007810: 6d62 6572 2075 7064 6174 6564 2066 6f72  mber updated for
+00007820: 2007 0000 0008 4a61 6c41 7373 6574 0103   .....JalAsset..
+00007830: 0000 0030 041d 0435 0442 0020 043a 043e  ...0...5.B. .:.>
+00007840: 0442 0438 0440 043e 0432 043a 0438 002f  .B.8.@.>.2.:.8./
+00007850: 043a 0443 0440 0441 0430 0020 0434 043b  .:.C.@.A.0. .4.;
+00007860: 044f 0020 0800 0000 0006 0000 001c 5468  .O. ..........Th
+00007870: 6572 6520 6172 6520 6e6f 2071 756f 7465  ere are no quote
+00007880: 2f72 6174 6520 666f 7220 0700 0000 084a  /rate for .....J
+00007890: 616c 4173 7365 7401 0300 0000 4c04 1d04  alAsset.....L...
+000078a0: 3504 3e04 3604 3804 3404 3004 3d04 3d04  5.>.6.8.4.0.=.=.
+000078b0: 3004 4f00 2004 3f04 3e04 3f04 4b04 4204  0.O. .?.>.?.K.B.
+000078c0: 3a04 3000 2004 3e04 3104 3d04 3e04 3204  :.0. .>.1.=.>.2.
+000078d0: 3804 4204 4c00 2000 4900 5300 4900 4e00  8.B.L. .I.S.I.N.
+000078e0: 2004 3404 3b04 4f00 2008 0000 0000 0600   .4.;.O. .......
+000078f0: 0000 2655 6e65 7870 6563 7465 6420 6174  ..&Unexpected at
+00007900: 7465 6d70 7420 746f 2075 7064 6174 6520  tempt to update 
+00007910: 4953 494e 2066 6f72 2007 0000 0008 4a61  ISIN for .....Ja
+00007920: 6c41 7373 6574 0103 0000 0006 0020 0432  lAsset....... .2
+00007930: 0020 0800 0000 0006 0000 0006 2069 6e74  . .......... int
+00007940: 6f20 0700 0000 094a 616c 4261 636b 7570  o .....JalBackup
+00007950: 0103 0000 001c 0410 0440 0445 0438 0432  .........@.E.8.2
+00007960: 044b 0020 0028 002a 002e 0074 0067 007a  .K. .(.*...t.g.z
+00007970: 0029 0800 0000 0006 0000 0010 4172 6368  .)..........Arch
+00007980: 6976 6573 2028 2a2e 7467 7a29 0700 0000  ives (*.tgz)....
+00007990: 094a 616c 4261 636b 7570 0103 0000 0046  .JalBackup.....F
+000079a0: 041d 0435 0020 0440 0430 0441 043f 043e  ...5. .@.0.A.?.>
+000079b0: 0437 043d 0430 043d 0430 0020 043c 0435  .7.=.0.=.0. .<.5
+000079c0: 0442 043a 0430 0020 0440 0435 0437 0435  .B.:.0. .@.5.7.5
+000079d0: 0440 0432 043d 043e 0439 0020 043a 043e  .@.2.=.>.9. .:.>
+000079e0: 043f 0438 0438 0800 0000 0006 0000 001b  .?.8.8..........
+000079f0: 4261 636b 7570 206c 6162 656c 206e 6f74  Backup label not
+00007a00: 2072 6563 6f67 6e69 7a65 6407 0000 0009   recognized.....
+00007a10: 4a61 6c42 6163 6b75 7001 0300 0000 4604  JalBackup.....F.
+00007a20: 2004 3504 3704 3504 4004 3204 3d04 3004   .5.7.5.@.2.=.0.
+00007a30: 4f00 2004 3a04 3e04 3f04 3804 4f00 2004  O. .:.>.?.8.O. .
+00007a40: 3204 3e04 4104 4104 4204 3004 3204 3d04  2.>.A.A.B.0.2.=.
+00007a50: 3e04 3204 3b04 3504 3d04 3000 2004 3804  >.2.;.5.=.0. .8.
+00007a60: 3700 3a00 2008 0000 0000 0600 0000 1642  7.:. ..........B
+00007a70: 6163 6b75 7020 7265 7374 6f72 6564 2066  ackup restored f
+00007a80: 726f 6d3a 2007 0000 0009 4a61 6c42 6163  rom: .....JalBac
+00007a90: 6b75 7001 0300 0000 3a04 2004 3504 3704  kup.....:. .5.7.
+00007aa0: 3504 4004 3204 3d04 3004 4f00 2004 3a04  5.@.2.=.0.O. .:.
+00007ab0: 3e04 3f04 3804 4f00 2004 4104 3e04 4504  >.?.8.O. .A.>.E.
+00007ac0: 4004 3004 3d04 5104 3d04 3000 2004 3200  @.0.=.Q.=.0. .2.
+00007ad0: 3a00 2008 0000 0000 0600 0000 1142 6163  :. ..........Bac
+00007ae0: 6b75 7020 7361 7665 6420 696e 3a20 0700  kup saved in: ..
+00007af0: 0000 094a 616c 4261 636b 7570 0103 0000  ...JalBackup....
+00007b00: 0052 041d 0435 0432 043e 0437 043c 043e  .R...5.2.>.7.<.>
+00007b10: 0436 043d 043e 0020 043f 0440 043e 0432  .6.=.>. .?.@.>.2
+00007b20: 0435 0440 0438 0442 044c 0020 0434 0430  .5.@.8.B.L. .4.0
+00007b30: 0442 0443 0020 0440 0435 0437 0435 0440  .B.C. .@.5.7.5.@
+00007b40: 0432 043d 043e 0439 0020 043a 043e 043f  .2.=.>.9. .:.>.?
+00007b50: 0438 0438 0800 0000 0006 0000 001a 4361  .8.8..........Ca
+00007b60: 6e27 7420 7661 6c69 6461 7465 2062 6163  n't validate bac
+00007b70: 6b75 7020 6461 7465 0700 0000 094a 616c  kup date.....Jal
+00007b80: 4261 636b 7570 0103 0000 0028 0414 0430  Backup.....(...0
+00007b90: 043d 043d 044b 0435 0020 0432 043e 0441  .=.=.K.5. .2.>.A
+00007ba0: 0441 0442 0430 043d 043e 0432 043b 0435  .A.B.0.=.>.2.;.5
+00007bb0: 043d 044b 0800 0000 0006 0000 000d 4461  .=.K..........Da
+00007bc0: 7461 2072 6573 746f 7265 6407 0000 0009  ta restored.....
+00007bd0: 4a61 6c42 6163 6b75 7001 0300 0000 4204  JalBackup.....B.
+00007be0: 1404 3004 3d04 3d04 4b04 3500 2004 3104  ..0.=.=.K.5. .1.
+00007bf0: 4b04 3b04 3800 2004 3704 3004 3304 4004  K.;.8. .7.0.3.@.
+00007c00: 4304 3604 3504 3d04 4b00 2004 3804 3700  C.6.5.=.K. .8.7.
+00007c10: 2004 3104 4d04 3a04 3004 3f04 3000 2e00   .1.M.:.0.?.0...
+00007c20: 0a08 0000 0000 0600 0000 2544 6174 6162  ..........%Datab
+00007c30: 6173 6520 7761 7320 6c6f 6164 6564 2066  ase was loaded f
+00007c40: 726f 6d20 7468 6520 6261 636b 7570 2e0a  rom the backup..
+00007c50: 0700 0000 094a 616c 4261 636b 7570 0103  .....JalBackup..
+00007c60: 0000 004e 041d 0435 0020 0443 0434 0430  ...N...5. .C.4.0
+00007c70: 043b 043e 0441 044c 0020 0432 043e 0441  .;.>.A.L. .2.>.A
+00007c80: 0441 0442 0430 043d 043e 0432 0438 0442  .A.B.0.=.>.2.8.B
+00007c90: 044c 0020 0440 0435 0437 0435 0440 0432  .L. .@.5.7.5.@.2
+00007ca0: 043d 0443 044e 0020 043a 043e 043f 0438  .=.C.N. .:.>.?.8
+00007cb0: 044e 0800 0000 0006 0000 001d 4661 696c  .N..........Fail
+00007cc0: 6564 2074 6f20 7265 7374 6f72 6520 6261  ed to restore ba
+00007cd0: 636b 7570 2066 696c 6507 0000 0009 4a61  ckup file.....Ja
+00007ce0: 6c42 6163 6b75 7001 0300 0000 3804 2104  lBackup.....8.!.
+00007cf0: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
+00007d00: 2004 4004 3504 3704 3504 4004 3204 3d04   .@.5.7.5.@.2.=.
+00007d10: 4304 4e00 2004 3a04 3e04 3f04 3804 4e00  C.N. .:.>.?.8.N.
+00007d20: 2004 3200 3a08 0000 0000 0600 0000 0f53   .2.:..........S
+00007d30: 6176 6520 6261 636b 7570 2074 6f3a 0700  ave backup to:..
+00007d40: 0000 094a 616c 4261 636b 7570 0103 0000  ...JalBackup....
+00007d50: 0040 0412 044b 0431 0435 0440 0438 0442  .@...K.1.5.@.8.B
+00007d60: 0435 0020 0444 0430 0439 043b 0020 0441  .5. .D.0.9.;. .A
+00007d70: 0020 0440 0435 0437 0435 0440 0432 043d  . .@.5.7.5.@.2.=
+00007d80: 043e 0439 0020 043a 043e 043f 0438 0435  .>.9. .:.>.?.8.5
+00007d90: 0439 0800 0000 0006 0000 0017 5365 6c65  .9..........Sele
+00007da0: 6374 2066 696c 6520 7769 7468 2062 6163  ct file with bac
+00007db0: 6b75 7007 0000 0009 4a61 6c42 6163 6b75  kup.....JalBacku
+00007dc0: 7001 0300 0000 4a04 1d04 3504 3204 3504  p.....J...5.2.5.
+00007dd0: 4004 3d04 4b04 3900 2004 4404 3e04 4004  @.=.K.9. .D.>.@.
+00007de0: 3c04 3004 4200 2004 4404 3004 3904 3b04  <.0.B. .D.0.9.;.
+00007df0: 3000 2004 4004 3504 3704 3504 4004 3204  0. .@.5.7.5.@.2.
+00007e00: 3d04 3e04 3900 2004 3a04 3e04 3f04 3804  =.>.9. .:.>.?.8.
+00007e10: 3808 0000 0000 0600 0000 1b57 726f 6e67  8..........Wrong
+00007e20: 2066 6f72 6d61 7420 6f66 2062 6163 6b75   format of backu
+00007e30: 7020 6669 6c65 0700 0000 094a 616c 4261  p file.....JalBa
+00007e40: 636b 7570 0103 0000 00c8 0412 044b 0020  ckup.........K. 
+00007e50: 0434 043e 043b 0436 043d 044b 0020 043f  .4.>.;.6.=.K. .?
+00007e60: 0435 0440 0435 0437 0430 043f 0443 0441  .5.@.5.7.0.?.C.A
+00007e70: 0442 0438 0442 044c 0020 043f 0440 0438  .B.8.B.L. .?.@.8
+00007e80: 043b 043e 0436 0435 043d 0438 0435 002c  .;.>.6.5.=.8.5.,
+00007e90: 0020 0447 0442 043e 0431 044b 0020 043f  . .G.B.>.1.K. .?
+00007ea0: 0440 0438 043c 0435 043d 0438 0442 044c  .@.8.<.5.=.8.B.L
+00007eb0: 0020 0438 0437 043c 0435 043d 0435 043d  . .8.7.<.5.=.5.=
+00007ec0: 0438 044f 000a 041f 0440 0438 043b 043e  .8.O.....@.8.;.>
+00007ed0: 0436 0435 043d 0438 0435 0020 0441 0435  .6.5.=.8.5. .A.5
+00007ee0: 0439 0447 0430 0441 0020 0437 0430 0432  .9.G.0.A. .7.0.2
+00007ef0: 0435 0440 0448 0438 0442 0020 0441 0432  .5.@.H.8.B. .A.2
+00007f00: 043e 044e 0020 0440 0430 0431 043e 0442  .>.N. .@.0.1.>.B
+00007f10: 0443 0800 0000 0006 0000 0052 596f 7520  .C.........RYou 
+00007f20: 7368 6f75 6c64 2072 6573 7461 7274 2061  should restart a
+00007f30: 7070 6c69 6361 7469 6f6e 2074 6f20 6170  pplication to ap
+00007f40: 706c 7920 6368 616e 6765 730a 4170 706c  ply changes.Appl
+00007f50: 6963 6174 696f 6e20 7769 6c6c 2062 6520  ication will be 
+00007f60: 7465 726d 696e 6174 6564 206e 6f77 0700  terminated now..
+00007f70: 0000 094a 616c 4261 636b 7570 0103 0000  ...JalBackup....
+00007f80: 0064 041e 043f 0435 0440 0430 0446 0438  .d...?.5.@.0.F.8
+00007f90: 044f 0020 0443 0436 0435 0020 0435 0441  .O. .C.6.5. .5.A
+00007fa0: 0442 044c 0020 0432 0020 0431 0430 0437  .B.L. .2. .1.0.7
+00007fb0: 0435 0020 0434 0430 043d 043d 044b 0445  .5. .4.0.=.=.K.E
+00007fc0: 0020 0438 0020 0431 044b 043b 0430 0020  . .8. .1.K.;.0. 
+00007fd0: 043f 0440 043e 043f 0443 0449 0435 043d  .?.@.>.?.C.I.5.=
+00007fe0: 0430 003a 0020 0800 0000 0006 0000 0031  .0.:. .........1
+00007ff0: 4f70 6572 6174 696f 6e20 616c 7265 6164  Operation alread
+00008000: 7920 7072 6573 656e 7420 696e 2064 6220  y present in db 
+00008010: 616e 6420 7761 7320 736b 6970 7065 643a  and was skipped:
+00008020: 2007 0000 0005 4a61 6c44 4201 0300 0000   .....JalDB.....
+00008030: 6e00 2004 3804 3c04 3504 3504 4200 2004  n. .8.<.5.5.B. .
+00008040: 3d04 3504 4104 3e04 4504 4004 3004 3d04  =.5.A.>.E.@.0.=.
+00008050: 5104 3d04 3d04 4b04 3500 2004 3804 3704  Q.=.=.K.5. .8.7.
+00008060: 3c04 3504 3d04 3504 3d04 3804 4f00 2c00  <.5.=.5.=.8.O.,.
+00008070: 0a04 3204 4b00 2004 4504 3e04 4204 3804  ..2.K. .E.>.B.8.
+00008080: 4204 3500 2004 3804 4500 2004 4104 3e04  B.5. .8.E. .A.>.
+00008090: 4504 4004 3004 3d04 3804 4204 4c00 3f08  E.@.0.=.8.B.L.?.
+000080a0: 0000 0000 0600 0000 3120 6861 7320 756e  ........1 has un
+000080b0: 636f 6d6d 6974 7465 6420 6368 616e 6765  committed change
+000080c0: 732c 0a64 6f20 796f 7520 7761 6e74 2074  s,.do you want t
+000080d0: 6f20 7361 7665 2069 743f 0700 0000 114a  o save it?.....J
+000080e0: 616c 4f70 6572 6174 696f 6e73 5461 6273  alOperationsTabs
+000080f0: 0103 0000 0036 0415 0441 0442 044c 0020  .....6...A.B.L. 
+00008100: 043d 0435 0441 043e 0445 0440 0430 043d  .=.5.A.>.E.@.0.=
+00008110: 0451 043d 043d 044b 0435 0020 0438 0437  .Q.=.=.K.5. .8.7
+00008120: 043c 0435 043d 043d 0438 044f 0800 0000  .<.5.=.=.8.O....
+00008130: 0006 0000 0018 596f 7520 6861 7665 2075  ......You have u
+00008140: 6e73 6176 6564 2063 6861 6e67 6573 0700  nsaved changes..
+00008150: 0000 114a 616c 4f70 6572 6174 696f 6e73  ...JalOperations
+00008160: 5461 6273 0103 0000 005a 041d 0435 0432  Tabs.....Z...5.2
+00008170: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+00008180: 0443 0434 0430 043b 0438 0442 044c 0020  .C.4.0.;.8.B.L. 
+00008190: 043f 0440 0435 0434 043e 043f 0440 0435  .?.@.5.4.>.?.@.5
+000081a0: 0434 0435 043b 0451 043d 043d 0443 044e  .4.5.;.Q.=.=.C.N
+000081b0: 0020 043a 0430 0442 0435 0433 043e 0440  . .:.0.B.5.3.>.@
+000081c0: 0438 044e 0800 0000 0006 0000 0020 4361  .8.N......... Ca
+000081d0: 6e27 7420 6465 6c65 7465 2070 7265 6465  n't delete prede
+000081e0: 6669 6e65 6420 6361 7465 676f 7279 0700  fined category..
+000081f0: 0000 0b4a 616c 5371 6c45 7272 6f72 0103  ...JalSqlError..
+00008200: 0000 009e 042d 0442 0438 0020 0434 0430  .....-.B.8. .4.0
+00008210: 043d 043d 044b 0435 0020 043d 0435 0020  .=.=.K.5. .=.5. 
+00008220: 043c 043e 0433 0443 0442 0020 0431 044b  .<.>.3.C.B. .1.K
+00008230: 0442 044c 0020 043c 043e 0434 0438 0444  .B.L. .<.>.4.8.D
+00008240: 0438 0446 0438 0440 043e 0432 0430 043d  .8.F.8.@.>.2.0.=
+00008250: 044b 002c 0020 0442 002e 043a 002e 0020  .K.,. .B...:... 
+00008260: 043d 0430 0020 043d 0438 0445 0020 0435  .=.0. .=.8.E. .5
+00008270: 0441 0442 044c 0020 0441 0441 044b 043b  .A.B.L. .A.A.K.;
+00008280: 043a 0430 0020 0432 0020 0434 0440 0443  .:.0. .2. .4.@.C
+00008290: 0433 043e 043c 0020 043c 0435 0441 0442  .3.>.<. .<.5.A.B
+000082a0: 0435 0800 0000 0006 0000 003a 4461 7461  .5.........:Data
+000082b0: 2061 7265 2072 6566 6572 656e 6365 6420   are referenced 
+000082c0: 696e 2061 6e6f 7468 6572 2070 6c61 6365  in another place
+000082d0: 2061 6e64 2063 616e 2774 2062 6520 6d6f   and can't be mo
+000082e0: 6469 6669 6564 0700 0000 0b4a 616c 5371  dified.....JalSq
+000082f0: 6c45 7272 6f72 0103 0000 001e 041e 0448  lError.........H
+00008300: 0438 0431 043a 0430 0020 0432 0020 0434  .8.1.:.0. .2. .4
+00008310: 0430 043d 043d 044b 0445 0800 0000 0006  .0.=.=.K.E......
+00008320: 0000 000e 4461 7461 6261 7365 2065 7272  ....Database err
+00008330: 6f72 0700 0000 0b4a 616c 5371 6c45 7272  or.....JalSqlErr
+00008340: 6f72 0103 0000 0050 041d 0435 0432 0435  or.....P...5.2.5
+00008350: 0440 043d 043e 0020 0432 044b 0431 0440  .@.=.>. .2.K.1.@
+00008360: 0430 043d 0430 0020 0432 0430 043b 044e  .0.=.0. .2.0.;.N
+00008370: 0442 0430 0020 0434 043b 044f 0020 0446  .B.0. .4.;.O. .F
+00008380: 0435 043d 043d 043e 0439 0020 0431 0443  .5.=.=.>.9. .1.C
+00008390: 043c 0430 0433 0438 0800 0000 0006 0000  .<.0.3.8........
+000083a0: 002a 496e 636f 7272 6563 7420 6375 7272  .*Incorrect curr
+000083b0: 656e 6379 2061 7373 6967 6e6d 656e 7420  ency assignment 
+000083c0: 666f 7220 616e 2061 7373 6574 0700 0000  for an asset....
+000083d0: 0b4a 616c 5371 6c45 7272 6f72 0103 0000  .JalSqlError....
+000083e0: 0080 041f 043e 043b 0435 0020 0411 0430  .....>.;.5. ...0
+000083f0: 043d 043a 002f 0411 0440 043e 043a 0435  .=.:./...@.>.:.5
+00008400: 0440 0020 0434 043e 043b 0436 043d 043e  .@. .4.>.;.6.=.>
+00008410: 0020 0431 044b 0442 044c 0020 0437 0430  . .1.K.B.L. .7.0
+00008420: 043f 043e 043b 043d 0435 043d 043e 0020  .?.>.;.=.5.=.>. 
+00008430: 0434 043b 044f 0020 0438 043d 0432 0435  .4.;.O. .8.=.2.5
+00008440: 0441 0442 0438 0446 0438 043e 043d 043d  .A.B.8.F.8.>.=.=
+00008450: 043e 0433 043e 0020 0441 0447 0435 0442  .>.3.>. .A.G.5.B
+00008460: 0430 0800 0000 0006 0000 0039 496e 7665  .0.........9Inve
+00008470: 7374 6d65 6e74 2061 6363 6f75 6e74 2073  stment account s
+00008480: 686f 756c 6420 6861 7665 2061 7373 6f63  hould have assoc
+00008490: 6961 7465 6420 6272 6f6b 6572 2061 7373  iated broker ass
+000084a0: 6967 6e65 6407 0000 000b 4a61 6c53 716c  igned.....JalSql
+000084b0: 4572 726f 7201 0300 0000 8800 2004 3e04  Error....... .>.
+000084c0: 3f04 3504 4004 3004 4604 3804 3900 2004  ?.5.@.0.F.8.9. .
+000084d0: 4204 4004 3504 3104 4304 4e04 4200 2004  B.@.5.1.C.N.B. .
+000084e0: 3f04 3504 4004 3504 4004 3004 4104 4704  ?.5.@.5.@.0.A.G.
+000084f0: 3504 4204 3000 2e00 2004 1204 4b00 2004  5.B.0... ...K. .
+00008500: 4504 3e04 3404 3804 4204 3500 2004 3204  E.>.4.8.B.5. .2.
+00008510: 4b04 3f04 3e04 3b04 3d04 3804 4204 4c00  K.?.>.;.=.8.B.L.
+00008520: 2004 3504 3304 3e00 2004 3f04 4004 4f04   .5.3.>. .?.@.O.
+00008530: 3c04 3e00 2004 4104 3504 3904 4704 3004  <.>. .A.5.9.G.0.
+00008540: 4100 3f08 0000 0000 0600 0000 3c20 6f70  A.?.........< op
+00008550: 6572 6174 696f 6e73 2072 6571 7569 7265  erations require
+00008560: 2072 6562 7569 6c64 2e20 446f 2079 6f75   rebuild. Do you
+00008570: 2077 616e 7420 746f 2064 6f20 6974 2072   want to do it r
+00008580: 6967 6874 206e 6f77 3f07 0000 0006 4c65  ight now?.....Le
+00008590: 6467 6572 0103 0000 0022 002c 0020 043d  dger.....".,. .=
+000085a0: 043e 0432 0430 044f 0020 0433 0440 0430  .>.2.0.O. .3.@.0
+000085b0: 043d 0438 0446 0430 003a 0020 0800 0000  .=.8.F.0.:. ....
+000085c0: 0006 0000 0010 2c20 6e65 7720 6672 6f6e  ......, new fron
+000085d0: 7469 6572 3a20 0700 0000 064c 6564 6765  tier: .....Ledge
+000085e0: 7201 0300 0000 1a04 1f04 3e04 3404 4204  r.........>.4.B.
+000085f0: 3204 3504 4004 3604 3404 3504 3d04 3804  2.5.@.6.4.5.=.8.
+00008600: 3508 0000 0000 0600 0000 0c43 6f6e 6669  5..........Confi
+00008610: 726d 6174 696f 6e07 0000 0006 4c65 6467  rmation.....Ledg
+00008620: 6572 0103 0000 0094 041f 0440 043e 0438  er.........@.>.8
+00008630: 0437 043e 0448 043b 0430 0020 043e 0448  .7.>.H.;.0. .>.H
+00008640: 0438 0431 043a 0430 002e 0020 0420 0430  .8.1.:.0... . .0
+00008650: 0441 0447 0451 0442 0020 0438 0442 043e  .A.G.Q.B. .8.B.>
+00008660: 0433 043e 0432 0020 043d 0435 0020 043e  .3.>.2. .=.5. .>
+00008670: 043a 043e 043d 0447 0435 043d 002e 0020  .:.>.=.G.5.=... 
+00008680: 041f 0440 043e 0432 0435 0440 044c 0442  ...@.>.2.5.@.L.B
+00008690: 0435 0020 0441 043e 043e 0431 0449 0435  .5. .A.>.>.1.I.5
+000086a0: 043d 0438 044f 0020 043e 0431 0020 043e  .=.8.O. .>.1. .>
+000086b0: 0448 0438 0431 043a 0430 0445 0800 0000  .H.8.1.:.0.E....
+000086c0: 0006 0000 004d 4578 6365 7074 696f 6e20  .....MException 
+000086d0: 6861 7070 656e 6564 2e20 4c65 6467 6572  happened. Ledger
+000086e0: 2069 7320 696e 636f 6d70 6c65 7465 2e20   is incomplete. 
+000086f0: 506c 6561 7365 2063 6f72 7265 6374 2065  Please correct e
+00008700: 7272 6f72 7320 6c69 7374 6564 2069 6e20  rrors listed in 
+00008710: 6c6f 6707 0000 0006 4c65 6467 6572 0103  log.....Ledger..
+00008720: 0000 004a 0418 0442 043e 0433 0438 0020  ...J...B.>.3.8. 
+00008730: 0440 0430 0441 0441 0447 0438 0442 0430  .@.0.A.A.G.8.B.0
+00008740: 043d 044b 002e 0020 0417 0430 0442 0440  .=.K... ...0.B.@
+00008750: 0430 0447 0435 043d 043d 043e 0435 0020  .0.G.5.=.=.>.5. 
+00008760: 0432 0440 0435 043c 044f 003a 0020 0800  .2.@.5.<.O.:. ..
+00008770: 0000 0006 0000 0022 4c65 6467 6572 2069  ......."Ledger i
+00008780: 7320 636f 6d70 6c65 7465 2e20 456c 6170  s complete. Elap
+00008790: 7365 6420 7469 6d65 3a20 0700 0000 064c  sed time: .....L
+000087a0: 6564 6765 7201 0300 0000 2c04 2204 4004  edger.....,.".@.
+000087b0: 3004 3d04 3704 3004 3a04 4604 3804 3800  0.=.7.0.:.F.8.8.
+000087c0: 2004 3e04 4204 4104 4304 4204 4104 4204   .>.B.A.C.B.A.B.
+000087d0: 3204 4304 4e04 4208 0000 0000 0600 0000  2.C.N.B.........
+000087e0: 0e4c 6567 6572 2069 7320 656d 7074 7907  .Leger is empty.
+000087f0: 0000 0006 4c65 6467 6572 0103 0000 0026  ....Ledger.....&
+00008800: 041d 0435 0020 0443 043a 0430 0437 0430  ...5. .C.:.0.7.0
+00008810: 043d 0430 0020 0426 0411 0020 0434 043b  .=.0. .&... .4.;
+00008820: 044f 003a 0020 0800 0000 0006 0000 0016  .O.:. ..........
+00008830: 4e6f 2061 7373 6574 2064 6566 696e 6564  No asset defined
+00008840: 2066 6f72 3a20 0700 0000 064c 6564 6765   for: .....Ledge
+00008850: 7201 0300 0000 3404 1d04 4300 2004 4304  r.....4...C. .C.
+00008860: 3a04 3004 3704 3004 3d04 3000 2004 3a04  :.0.7.0.=.0. .:.
+00008870: 3004 4204 3504 3304 3e04 4004 3804 4f00  0.B.5.3.>.@.8.O.
+00008880: 2004 3404 3b04 4f00 3a00 2008 0000 0000   .4.;.O.:. .....
+00008890: 0600 0000 154e 6f20 6361 7465 676f 7279  .....No category
+000088a0: 2073 6574 2066 6f72 3a20 0700 0000 064c   set for: .....L
+000088b0: 6564 6765 7201 0300 0000 3404 1d04 3500  edger.....4...5.
+000088c0: 2004 4304 3a04 3004 3704 3004 3d00 2004   .C.:.0.7.0.=. .
+000088d0: 3a04 3e04 3d04 4204 4004 3004 3304 3504  :.>.=.B.@.0.3.5.
+000088e0: 3d04 4200 2004 3404 3b04 4f00 3a00 2008  =.B. .4.;.O.:. .
+000088f0: 0000 0000 0600 0000 114e 6f20 7065 6572  .........No peer
+00008900: 2073 6574 2066 6f72 3a20 0700 0000 064c   set for: .....L
+00008910: 6564 6765 7201 0300 0000 2604 1f04 3504  edger.....&...5.
+00008920: 4004 3504 4104 4704 5104 4200 2004 3804  @.5.A.G.Q.B. .8.
+00008930: 4204 3e04 3304 3e04 3200 2004 4100 3a00  B.>.3.>.2. .A.:.
+00008940: 2008 0000 0000 0600 0000 1a52 652d 6275   ..........Re-bu
+00008950: 696c 6469 6e67 206c 6564 6765 7220 7369  ilding ledger si
+00008960: 6e63 653a 2007 0000 0006 4c65 6467 6572  nce: .....Ledger
+00008970: 0103 0000 0010 041e 0447 0438 0441 0442  .........G.8.A.B
+00008980: 0438 0442 044c 0800 0000 0006 0000 0005  .8.B.L..........
+00008990: 436c 6561 7207 0000 0009 4c6f 6756 6965  Clear.....LogVie
+000089a0: 7765 7201 0300 0000 1404 1a04 3e04 3f04  wer.........>.?.
+000089b0: 3804 4004 3e04 3204 3004 4204 4c08 0000  8.@.>.2.0.B.L...
+000089c0: 0000 0600 0000 0443 6f70 7907 0000 0009  .......Copy.....
+000089d0: 4c6f 6756 6965 7765 7201 0300 0000 1604  LogViewer.......
+000089e0: 1204 4b04 3104 4004 3004 4204 4c00 2004  ..K.1.@.0.B.L. .
+000089f0: 3204 4104 5108 0000 0000 0600 0000 0a53  2.A.Q..........S
+00008a00: 656c 6563 7420 616c 6c07 0000 0009 4c6f  elect all.....Lo
+00008a10: 6756 6965 7765 7201 0300 0000 5804 1d04  gViewer.....X...
+00008a20: 3504 3804 3704 3204 3504 4104 4204 3d04  5.8.7.2.5.A.B.=.
+00008a30: 4b04 3900 2004 3f04 3004 4004 3004 3c04  K.9. .?.0.@.0.<.
+00008a40: 3504 4204 4000 2004 3a04 4004 3804 4204  5.B.@. .:.@.8.B.
+00008a50: 3804 4704 3d04 3e04 4104 4204 3800 2004  8.G.=.>.A.B.8. .
+00008a60: 4104 3e04 3e04 3104 4904 3504 3d04 3804  A.>.>.1.I.5.=.8.
+00008a70: 4f00 3a00 2008 0000 0000 0600 0000 2055  O.:. ......... U
+00008a80: 6e6b 6e6f 776e 206c 6f67 6769 6e67 206c  nknown logging l
+00008a90: 6576 656c 2070 726f 7669 6465 643a 2007  evel provided: .
+00008aa0: 0000 0009 4c6f 6756 6965 7765 7201 0300  ....LogViewer...
+00008ab0: 0000 0c25 b200 2000 6c00 6f00 6700 7308  ...%.. .l.o.g.s.
+00008ac0: 0000 0000 0600 0000 08e2 96b2 206c 6f67  ............ log
+00008ad0: 7307 0000 0009 4c6f 6756 6965 7765 7201  s.....LogViewer.
+00008ae0: 0300 0000 0c25 b600 2000 6c00 6f00 6700  .....%.. .l.o.g.
+00008af0: 7308 0000 0000 0600 0000 08e2 96b6 206c  s............. l
+00008b00: 6f67 7307 0000 0009 4c6f 6756 6965 7765  ogs.....LogViewe
+00008b10: 7201 0300 0000 3e04 1e04 4804 3804 3104  r.....>...H.8.1.
+00008b20: 3a04 3000 2004 3b04 3e04 3304 3804 3d04  :.0. .;.>.3.8.=.
+00008b30: 3000 2004 4704 3504 4004 3504 3700 2004  0. .G.5.@.5.7. .
+00008b40: 1304 3e04 4104 4304 4104 3b04 4304 3304  ..>.A.C.A.;.C.3.
+00008b50: 3800 3a00 2008 0000 0000 0600 0000 1345  8.:. ..........E
+00008b60: 5349 4120 6c6f 6769 6e20 6661 696c 6564  SIA login failed
+00008b70: 3a20 0700 0000 084c 6f67 696e 464e 5301  : .....LoginFNS.
+00008b80: 0300 0000 4004 2304 4104 3f04 3504 4804  ....@.#.A.?.5.H.
+00008b90: 3d04 4b04 3900 2004 3b04 3e04 3304 3804  =.K.9. .;.>.3.8.
+00008ba0: 3d00 2004 4704 3504 4004 3504 3700 2004  =. .G.5.@.5.7. .
+00008bb0: 1304 3e04 4104 4304 4104 3b04 4304 3304  ..>.A.C.A.;.C.3.
+00008bc0: 3800 3a00 2008 0000 0000 0600 0000 1745  8.:. ..........E
+00008bd0: 5349 4120 6c6f 6769 6e20 7375 6363 6573  SIA login succes
+00008be0: 7366 756c 3a20 0700 0000 084c 6f67 696e  sful: .....Login
+00008bf0: 464e 5301 0300 0000 3804 1e04 4804 3804  FNS.....8...H.8.
+00008c00: 3104 3a04 3000 2004 3b04 3e04 3304 3804  1.:.0. .;.>.3.8.
+00008c10: 3d04 3000 2004 4704 3504 4004 3504 3700  =.0. .G.5.@.5.7.
+00008c20: 2004 1b04 1a00 2004 2404 1d04 2100 3a00   ..... .$...!.:.
+00008c30: 2008 0000 0000 0600 0000 1246 4e53 206c   ..........FNS l
+00008c40: 6f67 696e 2066 6169 6c65 643a 2007 0000  ogin failed: ...
+00008c50: 0008 4c6f 6769 6e46 4e53 0103 0000 003a  ..LoginFNS.....:
+00008c60: 0423 0441 043f 0435 0448 043d 044b 0439  .#.A.?.5.H.=.K.9
+00008c70: 0020 043b 043e 0433 0438 043d 0020 0447  . .;.>.3.8.=. .G
+00008c80: 0435 0440 0435 0437 0020 041b 041a 0020  .5.@.5.7. ..... 
+00008c90: 0424 041d 0421 003a 0020 0800 0000 0006  .$...!.:. ......
+00008ca0: 0000 0016 464e 5320 6c6f 6769 6e20 7375  ....FNS login su
+00008cb0: 6363 6573 7366 756c 3a20 0700 0000 084c  ccessful: .....L
+00008cc0: 6f67 696e 464e 5301 0300 0000 5a04 1e04  oginFNS.....Z...
+00008cd0: 4804 3804 3104 3a04 3000 2004 3f04 3e04  H.8.1.:.0. .?.>.
+00008ce0: 3b04 4304 4704 3504 3d04 3804 4f00 2000  ;.C.G.5.=.8.O. .
+00008cf0: 5500 5200 4c00 2004 3b04 3e04 3304 3804  U.R.L. .;.>.3.8.
+00008d00: 3d04 3000 2004 4704 3504 4004 3504 3700  =.0. .G.5.@.5.7.
+00008d10: 2004 1304 3e04 4104 4304 4104 3b04 4304   ...>.A.C.A.;.C.
+00008d20: 3304 3800 3a00 2008 0000 0000 0600 0000  3.8.:. .........
+00008d30: 1547 6574 2045 5349 4120 5552 4c20 6661  .Get ESIA URL fa
+00008d40: 696c 6564 3a20 0700 0000 084c 6f67 696e  iled: .....Login
+00008d50: 464e 5301 0300 0000 3400 5300 4d00 5300  FNS.....4.S.M.S.
+00008d60: 2004 3104 4b04 3b04 3e00 2004 3704 3004   .1.K.;.>. .7.0.
+00008d70: 3f04 4004 3e04 4804 3504 3d04 3e00 2004  ?.@.>.H.5.=.>. .
+00008d80: 4304 4104 3f04 3504 4804 3d04 3e08 0000  C.A.?.5.H.=.>...
+00008d90: 0000 0600 0000 1e53 4d53 2077 6173 2072  .......SMS was r
+00008da0: 6571 7565 7374 6564 2073 7563 6365 7373  equested success
+00008db0: 6675 6c6c 7907 0000 0008 4c6f 6769 6e46  fully.....LoginF
+00008dc0: 4e53 0103 0000 001e 0410 0432 0442 043e  NS.........2.B.>
+00008dd0: 0440 0438 0437 0430 0446 0438 044f 0020  .@.8.7.0.F.8.O. 
+00008de0: 0424 041d 0421 0800 0000 0006 0000 0011  .$...!..........
+00008df0: 4175 7468 6f72 697a 6174 696f 6e20 464e  Authorization FN
+00008e00: 5307 0000 000e 4c6f 6769 6e46 4e53 4469  S.....LoginFNSDi
+00008e10: 616c 6f67 0103 0000 000e 0417 0430 043a  alog.........0.:
+00008e20: 0440 044b 0442 044c 0800 0000 0006 0000  .@.K.B.L........
+00008e30: 0005 436c 6f73 6507 0000 000e 4c6f 6769  ..Close.....Logi
+00008e40: 6e46 4e53 4469 616c 6f67 0103 0000 0016  nFNSDialog......
+00008e50: 041a 043e 0434 0020 0438 0437 0020 0053  ...>.4. .8.7. .S
+00008e60: 004d 0053 003a 0800 0000 0006 0000 000e  .M.S.:..........
+00008e70: 436f 6465 2066 726f 6d20 534d 533a 0700  Code from SMS:..
+00008e80: 0000 0e4c 6f67 696e 464e 5344 6961 6c6f  ...LoginFNSDialo
+00008e90: 6701 0300 0000 1204 1304 3e04 4104 4304  g.........>.A.C.
+00008ea0: 4104 3b04 4304 3304 3808 0000 0000 0600  A.;.C.3.8.......
+00008eb0: 0000 0a45 5349 4120 4c6f 6769 6e07 0000  ...ESIA Login...
+00008ec0: 000e 4c6f 6769 6e46 4e53 4469 616c 6f67  ..LoginFNSDialog
+00008ed0: 0103 0000 000c 041b 041a 0020 0424 041d  ........... .$..
+00008ee0: 0421 0800 0000 0006 0000 0009 464e 5320  .!..........FNS 
+00008ef0: 4c6f 6769 6e07 0000 000e 4c6f 6769 6e46  Login.....LoginF
+00008f00: 4e53 4469 616c 6f67 0103 0000 0008 0418  NSDialog........
+00008f10: 041d 041d 003a 0800 0000 0006 0000 0004  .....:..........
+00008f20: 494e 4e3a 0700 0000 0e4c 6f67 696e 464e  INN:.....LoginFN
+00008f30: 5344 6961 6c6f 6701 0300 0000 0a04 1b04  SDialog.........
+00008f40: 3e04 3304 3804 3d08 0000 0000 0600 0000  >.3.8.=.........
+00008f50: 054c 6f67 696e 0700 0000 0e4c 6f67 696e  .Login.....Login
+00008f60: 464e 5344 6961 6c6f 6701 0300 0000 0e04  FNSDialog.......
+00008f70: 1f04 3004 4004 3e04 3b04 4c00 3a08 0000  ..0.@.>.;.L.:...
+00008f80: 0000 0600 0000 0950 6173 7377 6f72 643a  .......Password:
+00008f90: 0700 0000 0e4c 6f67 696e 464e 5344 6961  .....LoginFNSDia
+00008fa0: 6c6f 6701 0300 0000 1e04 1d04 3e04 3c04  log.........>.<.
+00008fb0: 3504 4000 2004 4204 3504 3b04 3504 4404  5.@. .B.5.;.5.D.
+00008fc0: 3e04 3d04 3000 3a08 0000 0000 0600 0000  >.=.0.:.........
+00008fd0: 0d50 686f 6e65 206e 756d 6265 723a 0700  .Phone number:..
+00008fe0: 0000 0e4c 6f67 696e 464e 5344 6961 6c6f  ...LoginFNSDialo
+00008ff0: 6701 0300 0000 0600 5300 4d00 5308 0000  g.......S.M.S...
+00009000: 0000 0600 0000 0953 4d53 204c 6f67 696e  .......SMS Login
+00009010: 0700 0000 0e4c 6f67 696e 464e 5344 6961  .....LoginFNSDia
+00009020: 6c6f 6701 0300 0000 2604 1204 4b04 4104  log.....&...K.A.
+00009030: 3b04 3004 4204 4c00 2000 5300 4d00 5300  ;.0.B.L. .S.M.S.
+00009040: 2004 4100 2004 3a04 3e04 3404 3e04 3c08   .A. .:.>.4.>.<.
+00009050: 0000 0000 0600 0000 1253 656e 6420 534d  .........Send SM
+00009060: 5320 7769 7468 2063 6f64 6507 0000 000e  S with code.....
+00009070: 4c6f 6769 6e46 4e53 4469 616c 6f67 0103  LoginFNSDialog..
+00009080: 0000 0016 0061 0062 006f 0075 0074 003a  .....a.b.o.u.t.:
+00009090: 0062 006c 0061 006e 006b 0800 0000 0006  .b.l.a.n.k......
+000090a0: 0000 000b 6162 6f75 743a 626c 616e 6b07  ....about:blank.
+000090b0: 0000 000e 4c6f 6769 6e46 4e53 4469 616c  ....LoginFNSDial
+000090c0: 6f67 0103 0000 0044 041d 0430 0439 0434  og.....D...0.9.4
+000090d0: 0435 043d 043e 0020 043d 0435 0441 043a  .5.=.>. .=.5.A.:
+000090e0: 043e 043b 044c 043a 043e 0020 0426 0411  .>.;.L.:.>. .&..
+000090f0: 0020 043d 0430 0020 004d 004f 0045 0058  . .=.0. .M.O.E.X
+00009100: 0020 0434 043b 044f 003a 0020 0800 0000  . .4.;.O.:. ....
+00009110: 0006 0000 0020 4d75 6c74 6970 6c65 204d  ..... Multiple M
+00009120: 4f45 5820 6173 7365 7473 2066 6f75 6e64  OEX assets found
+00009130: 2066 6f72 3a20 0700 0000 044d 4f45 5801   for: .....MOEX.
+00009140: 0300 0000 4404 1d04 3504 3f04 3e04 3404  ....D...5.?.>.4.
+00009150: 3404 3504 4004 3604 3804 3204 3004 3504  4.5.@.6.8.2.0.5.
+00009160: 3c04 4b04 3900 2004 4204 3804 3f00 2004  <.K.9. .B.8.?. .
+00009170: 2604 1100 2004 1c04 3e04 4104 1104 3804  &... ...>.A...8.
+00009180: 4004 3604 3800 3a00 2008 0000 0000 0600  @.6.8.:. .......
+00009190: 0000 2055 6e73 7570 706f 7274 6564 204d  .. Unsupported M
+000091a0: 4f45 5820 7365 6375 7269 7479 2074 7970  OEX security typ
+000091b0: 653a 2007 0000 0004 4d4f 4558 0103 0000  e: .....MOEX....
+000091c0: 0016 041e 0020 043f 0440 043e 0433 0440  ..... .?.@.>.3.@
+000091d0: 0430 043c 043c 0435 0800 0000 0006 0000  .0.<.<.5........
+000091e0: 0005 4162 6f75 7407 0000 000a 4d61 696e  ..About.....Main
+000091f0: 5769 6e64 6f77 0103 0000 001a 041f 043e  Window.........>
+00009200: 0434 0442 0432 0435 0440 0436 0434 0435  .4.B.2.5.@.6.4.5
+00009210: 043d 0438 0435 0800 0000 0006 0000 000c  .=.8.5..........
+00009220: 436f 6e66 6972 6d61 7469 6f6e 0700 0000  Confirmation....
+00009230: 0a4d 6169 6e57 696e 646f 7701 0300 0000  .MainWindow.....
+00009240: 1404 1804 3d04 4404 3e04 4004 3c04 3004  ....=.D.>.@.<.0.
+00009250: 4604 3804 4f08 0000 0000 0600 0000 0449  F.8.O..........I
+00009260: 6e66 6f07 0000 000a 4d61 696e 5769 6e64  nfo.....MainWind
+00009270: 6f77 0103 0000 0028 042f 0437 044b 043a  ow.....(./.7.K.:
+00009280: 0020 0431 044b 043b 0020 0438 0437 043c  . .1.K.;. .8.7.<
+00009290: 0435 043d 0451 043d 0020 043d 0430 0020  .5.=.Q.=. .=.0. 
+000092a0: 0800 0000 0006 0000 0018 4c61 6e67 7561  ..........Langua
+000092b0: 6765 2077 6173 2063 6861 6e67 6564 2074  ge was changed t
+000092c0: 6f20 0700 0000 0a4d 6169 6e57 696e 646f  o .....MainWindo
+000092d0: 7701 0300 0000 6204 1804 4204 3e04 3304  w.....b...B.>.3.
+000092e0: 3800 2004 4204 4004 3004 3d04 3704 3004  8. .B.@.0.=.7.0.
+000092f0: 3a04 4604 3804 3900 2004 3d04 3504 3004  :.F.8.9. .=.5.0.
+00009300: 3a04 4204 4304 3004 3b04 4c04 3d04 4b00  :.B.C.0.;.L.=.K.
+00009310: 2e00 2004 1f04 3504 4004 3504 4104 4704  .. ...5.@.5.A.G.
+00009320: 3804 4204 3004 4204 4c00 2004 4104 3504  8.B.0.B.L. .A.5.
+00009330: 3904 4704 3004 4100 3f08 0000 0000 0600  9.G.0.A.?.......
+00009340: 0000 264c 6564 6765 7220 6973 6e27 7420  ..&Ledger isn't 
+00009350: 636f 6d70 6c65 7465 2e20 5265 6275 696c  complete. Rebuil
+00009360: 6420 6974 206e 6f77 3f07 0000 000a 4d61  d it now?.....Ma
+00009370: 696e 5769 6e64 6f77 0103 0000 0080 0414  inWindow........
+00009380: 043e 043f 043e 043b 043d 0438 0442 0435  .>.?.>.;.=.8.B.5
+00009390: 043b 044c 043d 0430 044f 0020 0438 043d  .;.L.=.0.O. .8.=
+000093a0: 0444 043e 0440 043c 0430 0446 0438 044f  .D.>.@.<.0.F.8.O
+000093b0: 002c 0020 0438 043d 0441 0442 0440 0443  .,. .8.=.A.B.@.C
+000093c0: 043a 0446 0438 0438 002c 0020 0441 043e  .:.F.8.8.,. .A.>
+000093d0: 043e 0431 0449 0435 043d 0438 044f 0020  .>.1.I.5.=.8.O. 
+000093e0: 043e 0020 043f 0440 043e 0431 043b 0435  .>. .?.@.>.1.;.5
+000093f0: 043c 0430 0445 0020 043d 0430 0020 0800  .<.0.E. .=.0. ..
+00009400: 0000 0006 0000 0035 4d6f 7265 2069 6e66  .......5More inf
+00009410: 6f72 6d61 7469 6f6e 2c20 6d61 6e75 616c  ormation, manual
+00009420: 7320 616e 6420 7072 6f62 6c65 6d20 7265  s and problem re
+00009430: 706f 7274 7320 6172 6520 6174 2007 0000  ports are at ...
+00009440: 000a 4d61 696e 5769 6e64 6f77 0103 0000  ..MainWindow....
+00009450: 0050 0412 043e 043f 0440 043e 0441 044b  .P...>.?.@.>.A.K
+00009460: 002c 0020 043a 043e 043c 043c 0435 043d  .,. .:.>.<.<.5.=
+00009470: 0442 0430 0440 0438 0438 002c 0020 043f  .B.0.@.8.8.,. .?
+00009480: 043e 043c 043e 0449 044c 0020 0438 043b  .>.<.>.I.L. .8.;
+00009490: 0438 0020 0434 043e 043d 0430 0442 044b  .8. .4.>.=.0.B.K
+000094a0: 003a 0800 0000 0006 0000 0027 5175 6573  .:.........'Ques
+000094b0: 7469 6f6e 732c 2063 6f6d 6d65 6e74 732c  tions, comments,
+000094c0: 2068 656c 7020 6f72 2064 6f6e 6174 696f   help or donatio
+000094d0: 6e73 3a07 0000 000a 4d61 696e 5769 6e64  ns:.....MainWind
+000094e0: 6f77 0103 0000 0022 0422 0440 0435 0431  ow.....".".@.5.1
+000094f0: 0443 0435 0442 0441 044f 0020 0440 0435  .C.5.B.A.O. .@.5
+00009500: 0441 0442 0430 0440 0442 0800 0000 0006  .A.B.0.@.B......
+00009510: 0000 0010 5265 7374 6172 7420 7265 7175  ....Restart requ
+00009520: 6972 6564 0700 0000 0a4d 6169 6e57 696e  ired.....MainWin
+00009530: 646f 7701 0300 0000 5004 1a04 3e04 3d04  dow.....P...>.=.
+00009540: 3504 4704 3d04 4b04 3900 2004 3104 3004  5.G.=.K.9. .1.0.
+00009550: 3b04 3004 3d04 4100 2004 3f04 3e00 2004  ;.0.=.A. .?.>. .
+00009560: 3e04 4204 4704 5104 4204 4300 2004 3d04  >.B.G.Q.B.C. .=.
+00009570: 3500 2004 4104 3e04 3204 3f04 3004 3404  5. .A.>.2.?.0.4.
+00009580: 3004 3504 4200 3a00 2008 0000 0000 0600  0.5.B.:. .......
+00009590: 0000 2853 7461 7465 6d65 6e74 2065 6e64  ..(Statement end
+000095a0: 696e 6720 6261 6c61 6e63 6520 646f 6573  ing balance does
+000095b0: 6e27 7420 6d61 7463 683a 2007 0000 000a  n't match: .....
+000095c0: 4d61 696e 5769 6e64 6f77 0103 0000 00c8  MainWindow......
+000095d0: 0412 044b 0020 0434 043e 043b 0436 043d  ...K. .4.>.;.6.=
+000095e0: 044b 0020 043f 0435 0440 0435 0437 0430  .K. .?.5.@.5.7.0
+000095f0: 043f 0443 0441 0442 0438 0442 044c 0020  .?.C.A.B.8.B.L. 
+00009600: 043f 0440 0438 043b 043e 0436 0435 043d  .?.@.8.;.>.6.5.=
+00009610: 0438 0435 002c 0020 0447 0442 043e 0431  .8.5.,. .G.B.>.1
+00009620: 044b 0020 043f 0440 0438 043c 0435 043d  .K. .?.@.8.<.5.=
+00009630: 0438 0442 044c 0020 0438 0437 043c 0435  .8.B.L. .8.7.<.5
+00009640: 043d 0435 043d 0438 044f 000a 041f 0440  .=.5.=.8.O.....@
+00009650: 0438 043b 043e 0436 0435 043d 0438 0435  .8.;.>.6.5.=.8.5
+00009660: 0020 0441 0435 0439 0447 0430 0441 0020  . .A.5.9.G.0.A. 
+00009670: 0437 0430 0432 0435 0440 0448 0438 0442  .7.0.2.5.@.H.8.B
+00009680: 0020 0441 0432 043e 044e 0020 0440 0430  . .A.2.>.N. .@.0
+00009690: 0431 043e 0442 0443 0800 0000 0006 0000  .1.>.B.C........
+000096a0: 0052 596f 7520 7368 6f75 6c64 2072 6573  .RYou should res
+000096b0: 7461 7274 2061 7070 6c69 6361 7469 6f6e  tart application
+000096c0: 2074 6f20 6170 706c 7920 6368 616e 6765   to apply change
+000096d0: 730a 4170 706c 6963 6174 696f 6e20 7769  s.Application wi
+000096e0: 6c6c 2062 6520 7465 726d 696e 6174 6564  ll be terminated
+000096f0: 206e 6f77 0700 0000 0a4d 6169 6e57 696e   now.....MainWin
+00009700: 646f 7701 0300 0000 3004 3404 3e04 3c04  dow.....0.4.>.<.
+00009710: 3004 4804 3d04 3504 3900 2004 4104 4204  0.H.=.5.9. .A.B.
+00009720: 4004 3004 3d04 3804 4604 3500 2000 6700  @.0.=.8.F.5. .g.
+00009730: 6900 7400 6800 7500 6208 0000 0000 0600  i.t.h.u.b.......
+00009740: 0000 1067 6974 6875 6220 686f 6d65 2070  ...github home p
+00009750: 6167 6507 0000 000a 4d61 696e 5769 6e64  age.....MainWind
+00009760: 6f77 0103 0000 000c 0432 0435 0440 0441  ow.......2.5.@.A
+00009770: 0438 044f 0800 0000 0006 0000 0007 7665  .8.O..........ve
+00009780: 7273 696f 6e07 0000 000a 4d61 696e 5769  rsion.....MainWi
+00009790: 6e64 6f77 0103 0000 0006 002e 002e 002e  ndow............
+000097a0: 0800 0000 0006 0000 0003 2e2e 2e07 0000  ................
+000097b0: 000f 4d6f 6e65 7946 6c6f 7757 6964 6765  ..MoneyFlowWidge
+000097c0: 7401 0300 0000 1604 2404 3004 3904 3b00  t.......$.0.9.;.
+000097d0: 2000 4500 7800 6300 6500 6c00 3a08 0000   .E.x.c.e.l.:...
+000097e0: 0000 0600 0000 0b45 7863 656c 2066 696c  .......Excel fil
+000097f0: 653a 0700 0000 0f4d 6f6e 6579 466c 6f77  e:.....MoneyFlow
+00009800: 5769 6467 6574 0103 0000 0028 0424 0430  Widget.....(.$.0
+00009810: 0439 043b 044b 0020 0045 0078 0063 0065  .9.;.K. .E.x.c.e
+00009820: 006c 0020 0028 002a 002e 0078 0073 006c  .l. .(.*...x.s.l
+00009830: 0078 0029 0800 0000 0006 0000 0014 4578  .x.)..........Ex
+00009840: 6365 6c20 6669 6c65 7320 282a 2e78 6c73  cel files (*.xls
+00009850: 7829 0700 0000 0f4d 6f6e 6579 466c 6f77  x).....MoneyFlow
+00009860: 5769 6467 6574 0103 0000 0056 0424 0430  Widget.....V.$.0
+00009870: 0439 043b 0020 0434 043b 044f 0020 0441  .9.;. .4.;.O. .A
+00009880: 043e 0445 0440 0430 043d 0435 043d 0438  .>.E.@.0.=.5.=.8
+00009890: 044f 0020 0440 0430 0441 0447 0451 0442  .O. .@.0.A.G.Q.B
+000098a0: 0430 0020 0432 0020 0444 043e 0440 043c  .0. .2. .D.>.@.<
+000098b0: 0430 0442 0435 0020 0045 0078 0063 0065  .0.B.5. .E.x.c.e
+000098c0: 006c 0800 0000 0006 0000 002e 4669 6c65  .l..........File
+000098d0: 2077 6865 7265 2074 6f20 7374 6f72 6520   where to store 
+000098e0: 7461 7820 7265 706f 7274 2069 6e20 4578  tax report in Ex
+000098f0: 6365 6c20 666f 726d 6174 0700 0000 0f4d  cel format.....M
+00009900: 6f6e 6579 466c 6f77 5769 6467 6574 0103  oneyFlowWidget..
+00009910: 0000 000a 041e 043e 0414 0414 0421 0800  .......>.....!..
+00009920: 0000 0006 0000 000a 4d6f 6e65 7920 466c  ........Money Fl
+00009930: 6f77 0700 0000 0f4d 6f6e 6579 466c 6f77  ow.....MoneyFlow
+00009940: 5769 6467 6574 0103 0000 002e 041e 043e  Widget.........>
+00009950: 0414 0414 0421 0020 0441 043e 0445 0440  .....!. .A.>.E.@
+00009960: 0430 043d 0451 043d 0020 0432 0020 0444  .0.=.Q.=. .2. .D
+00009970: 0430 0439 043b 0435 0020 0800 0000 0006  .0.9.;.5. ......
+00009980: 0000 0020 4d6f 6e65 7920 666c 6f77 2072  ... Money flow r
+00009990: 6570 6f72 7420 7361 7665 6420 746f 2066  eport saved to f
+000099a0: 696c 6520 0700 0000 0f4d 6f6e 6579 466c  ile .....MoneyFl
+000099b0: 6f77 5769 6467 6574 0103 0000 001e 0421  owWidget.......!
+000099c0: 043e 0445 0440 0430 043d 0438 0442 044c  .>.E.@.0.=.8.B.L
+000099d0: 0020 041e 0442 0447 0451 0442 0800 0000  . ...B.G.Q.B....
+000099e0: 0006 0000 000b 5361 7665 2052 6570 6f72  ......Save Repor
+000099f0: 7407 0000 000f 4d6f 6e65 7946 6c6f 7757  t.....MoneyFlowW
+00009a00: 6964 6765 7401 0300 0000 2404 2104 3e04  idget.....$.!.>.
+00009a10: 4504 4004 3004 3d04 3804 4204 4c00 2004  E.@.0.=.8.B.L. .
+00009a20: 1e04 3e04 1404 1404 2100 2004 3200 3a08  ..>.....!. .2.:.
+00009a30: 0000 0000 0600 0000 1a53 6176 6520 6d6f  .........Save mo
+00009a40: 6e65 7920 666c 6f77 2072 6570 6f72 7420  ney flow report 
+00009a50: 746f 3a07 0000 000f 4d6f 6e65 7946 6c6f  to:.....MoneyFlo
+00009a60: 7757 6964 6765 7401 0300 0000 1804 1204  wWidget.........
+00009a70: 4b04 3104 3504 4004 3804 4200 2004 4404  K.1.5.@.8.B. .D.
+00009a80: 3004 3904 3b08 0000 0000 0600 0000 0b53  0.9.;..........S
+00009a90: 656c 6563 7420 6669 6c65 0700 0000 0f4d  elect file.....M
+00009aa0: 6f6e 6579 466c 6f77 5769 6467 6574 0103  oneyFlowWidget..
+00009ab0: 0000 0008 0413 043e 0434 003a 0800 0000  .......>.4.:....
+00009ac0: 0006 0000 0005 5965 6172 3a07 0000 000f  ......Year:.....
+00009ad0: 4d6f 6e65 7946 6c6f 7757 6964 6765 7401  MoneyFlowWidget.
+00009ae0: 0300 0000 2800 2004 3d04 3504 4304 4104  ....(. .=.5.C.A.
+00009af0: 3f04 3504 4804 3d04 4b04 3900 2004 3704  ?.5.H.=.K.9. .7.
+00009b00: 3004 3f04 4004 3e04 4100 3a00 2008 0000  0.?.@.>.A.:. ...
+00009b10: 0000 0600 0000 0920 6661 696c 6564 3a20  ....... failed: 
+00009b20: 0700 0000 034e 6574 0103 0000 0034 0422  .....Net.....4."
+00009b30: 0438 043f 0020 0426 0411 0020 043d 0435  .8.?. .&... .=.5
+00009b40: 0020 043f 043e 0434 0434 0435 0440 0436  . .?.>.4.4.5.@.6
+00009b50: 0438 0432 0430 0435 0442 0441 044f 003a  .8.2.0.5.B.A.O.:
+00009b60: 0020 0800 0000 0006 0000 001c 4173 7365  . ..........Asse
+00009b70: 7420 7479 7065 2069 736e 2774 2073 7570  t type isn't sup
+00009b80: 706f 7274 6564 3a20 0700 0000 0a4f 7065  ported: .....Ope
+00009b90: 6e42 726f 6b65 7201 0300 0000 3204 1104  nBroker.....2...
+00009ba0: 3804 4004 3604 3000 2004 3d04 3500 2004  8.@.6.0. .=.5. .
+00009bb0: 3f04 3e04 3404 3404 3504 4004 3604 3804  ?.>.4.4.5.@.6.8.
+00009bc0: 3204 3004 3504 4204 4104 4f00 3a00 2008  2.0.5.B.A.O.:. .
+00009bd0: 0000 0000 0600 0000 1a45 7863 6861 6e67  .........Exchang
+00009be0: 6520 6973 6e27 7420 7375 7070 6f72 7465  e isn't supporte
+00009bf0: 643a 2007 0000 000a 4f70 656e 4272 6f6b  d: .....OpenBrok
+00009c00: 6572 0103 0000 0008 0421 0447 0435 0442  er.......!.G.5.B
+00009c10: 0800 0000 0006 0000 0007 4163 636f 756e  ..........Accoun
+00009c20: 7407 0000 000f 4f70 6572 6174 696f 6e73  t.....Operations
+00009c30: 4d6f 6465 6c01 0300 0000 0a04 2104 4304  Model.......!.C.
+00009c40: 3c04 3c04 3008 0000 0000 0600 0000 0641  <.<.0..........A
+00009c50: 6d6f 756e 7407 0000 000f 4f70 6572 6174  mount.....Operat
+00009c60: 696f 6e73 4d6f 6465 6c01 0300 0000 0c04  ionsModel.......
+00009c70: 1104 3004 3b04 3004 3d04 4108 0000 0000  ..0.;.0.=.A.....
+00009c80: 0600 0000 0742 616c 616e 6365 0700 0000  .....Balance....
+00009c90: 0f4f 7065 7261 7469 6f6e 734d 6f64 656c  .OperationsModel
+00009ca0: 0103 0000 000c 0412 0430 043b 044e 0442  .........0.;.N.B
+00009cb0: 0430 0800 0000 0006 0000 0008 4375 7272  .0..........Curr
+00009cc0: 656e 6379 0700 0000 0f4f 7065 7261 7469  ency.....Operati
+00009cd0: 6f6e 734d 6f64 656c 0103 0000 0010 041e  onsModel........
+00009ce0: 043f 0438 0441 0430 043d 0438 0435 0800  .?.8.A.0.=.8.5..
+00009cf0: 0000 0006 0000 0005 4e6f 7465 7307 0000  ........Notes...
+00009d00: 000f 4f70 6572 6174 696f 6e73 4d6f 6465  ..OperationsMode
+00009d10: 6c01 0300 0000 1404 1404 3004 4204 3000  l.........0.B.0.
+00009d20: 2f04 1204 4004 3504 3c04 4f08 0000 0000  /...@.5.<.O.....
+00009d30: 0600 0000 0954 696d 6573 7461 6d70 0700  .....Timestamp..
+00009d40: 0000 0f4f 7065 7261 7469 6f6e 734d 6f64  ...OperationsMod
+00009d50: 656c 0103 0000 000a 0421 0447 0435 0442  el.......!.G.5.B
+00009d60: 003a 0800 0000 0006 0000 0008 4163 636f  .:..........Acco
+00009d70: 756e 743a 0700 0000 104f 7065 7261 7469  unt:.....Operati
+00009d80: 6f6e 7357 6964 6765 7401 0300 0000 4a04  onsWidget.....J.
+00009d90: 1204 4b00 2004 4504 3e04 4204 3804 4204  ..K. .E.>.B.8.B.
+00009da0: 3500 2004 4304 3404 3004 3b04 3804 4204  5. .C.4.0.;.8.B.
+00009db0: 4c00 2004 3204 4b04 3104 4004 3004 3d04  L. .2.K.1.@.0.=.
+00009dc0: 3d04 4b04 3500 2004 3e04 3f04 3504 4004  =.K.5. .>.?.5.@.
+00009dd0: 3004 4604 3804 3800 3f08 0000 0000 0600  0.F.8.8.?.......
+00009de0: 0000 2e41 7265 2079 6f75 2073 7572 6520  ...Are you sure 
+00009df0: 746f 2064 656c 6574 6520 7365 6c65 6374  to delete select
+00009e00: 6564 2074 7261 6e73 6163 696f 6e28 7329  ed transacion(s)
+00009e10: 3f07 0000 0010 4f70 6572 6174 696f 6e73  ?.....Operations
+00009e20: 5769 6467 6574 0103 0000 001c 0411 0430  Widget.........0
+00009e30: 043b 0430 043d 0441 044b 0020 0441 0447  .;.0.=.A.K. .A.G
+00009e40: 0435 0442 043e 0432 0800 0000 0006 0000  .5.B.>.2........
+00009e50: 0008 4261 6c61 6e63 6573 0700 0000 104f  ..Balances.....O
+00009e60: 7065 7261 7469 6f6e 7357 6964 6765 7401  perationsWidget.
+00009e70: 0300 0000 1a04 1f04 3e04 3404 4204 3204  ........>.4.B.2.
+00009e80: 3504 4004 3604 3404 3504 3d04 3804 3508  5.@.6.4.5.=.8.5.
+00009e90: 0000 0000 0600 0000 0c43 6f6e 6669 726d  .........Confirm
+00009ea0: 6174 696f 6e07 0000 0010 4f70 6572 6174  ation.....Operat
+00009eb0: 696f 6e73 5769 6467 6574 0103 0000 0014  ionsWidget......
+00009ec0: 041a 043e 043f 0438 0440 043e 0432 0430  ...>.?.8.@.>.2.0
+00009ed0: 0442 044c 0800 0000 0006 0000 0004 436f  .B.L..........Co
+00009ee0: 7079 0700 0000 104f 7065 7261 7469 6f6e  py.....Operation
+00009ef0: 7357 6964 6765 7401 0300 0000 2604 1a04  sWidget.....&...
+00009f00: 3e04 3f04 3804 4004 3e04 3204 3004 4204  >.?.8.@.>.2.0.B.
+00009f10: 4c00 2004 3e04 3f04 3504 4004 3004 4604  L. .>.?.5.@.0.F.
+00009f20: 3804 4e08 0000 0000 0600 0000 0e43 6f70  8.N..........Cop
+00009f30: 7920 6f70 6572 6174 696f 6e07 0000 0010  y operation.....
+00009f40: 4f70 6572 6174 696f 6e73 5769 6467 6574  OperationsWidget
+00009f50: 0103 0000 000e 0423 0434 0430 043b 0438  .......#.4.0.;.8
+00009f60: 0442 044c 0800 0000 0006 0000 0006 4465  .B.L..........De
+00009f70: 6c65 7465 0700 0000 104f 7065 7261 7469  lete.....Operati
+00009f80: 6f6e 7357 6964 6765 7401 0300 0000 2004  onsWidget..... .
+00009f90: 2304 3404 3004 3b04 3804 4204 4c00 2004  #.4.0.;.8.B.L. .
+00009fa0: 3e04 3f04 3504 4004 3004 4604 3804 4e08  >.?.5.@.0.F.8.N.
+00009fb0: 0000 0000 0600 0000 1044 656c 6574 6520  .........Delete 
+00009fc0: 6f70 6572 6174 696f 6e07 0000 0010 4f70  operation.....Op
+00009fd0: 6572 6174 696f 6e73 5769 6467 6574 0103  erationsWidget..
+00009fe0: 0000 001c 041d 043e 0432 0430 044f 0020  .......>.2.0.O. 
+00009ff0: 043e 043f 0435 0440 0430 0446 0438 044f  .>.?.5.@.0.F.8.O
+0000a000: 0800 0000 0006 0000 000d 4e65 7720 6f70  ..........New op
+0000a010: 6572 6174 696f 6e07 0000 0010 4f70 6572  eration.....Oper
+0000a020: 6174 696f 6e73 5769 6467 6574 0103 0000  ationsWidget....
+0000a030: 0010 041e 043f 0435 0440 0430 0446 0438  .....?.5.@.0.F.8
+0000a040: 0438 0800 0000 0006 0000 000a 4f70 6572  .8..........Oper
+0000a050: 6174 696f 6e73 0700 0000 104f 7065 7261  ations.....Opera
+0000a060: 7469 6f6e 7357 6964 6765 7401 0300 0000  tionsWidget.....
+0000a070: 2404 1e04 3f04 3504 4004 3004 4604 3804  $...?.5.@.0.F.8.
+0000a080: 3800 2004 3800 2004 1104 3004 3b04 3004  8. .8. ...0.;.0.
+0000a090: 3d04 4104 4b08 0000 0000 0600 0000 154f  =.A.K..........O
+0000a0a0: 7065 7261 7469 6f6e 7320 2620 4261 6c61  perations & Bala
+0000a0b0: 6e63 6573 0700 0000 104f 7065 7261 7469  nces.....Operati
+0000a0c0: 6f6e 7357 6964 6765 7401 0300 0000 0e04  onsWidget.......
+0000a0d0: 2104 3204 3504 4004 3804 4204 4c08 0000  !.2.5.@.8.B.L...
+0000a0e0: 0000 0600 0000 0952 6563 6f6e 6369 6c65  .......Reconcile
+0000a0f0: 0700 0000 104f 7065 7261 7469 6f6e 7357  .....OperationsW
+0000a100: 6964 6765 7401 0300 0000 0c04 1f04 3e04  idget.........>.
+0000a110: 3804 4104 3a00 3a08 0000 0000 0600 0000  8.A.:.:.........
+0000a120: 0753 6561 7263 683a 0700 0000 104f 7065  .Search:.....Ope
+0000a130: 7261 7469 6f6e 7357 6964 6765 7401 0300  rationsWidget...
+0000a140: 0000 2c04 1f04 3e04 3a04 3004 3704 4b04  ..,...>.:.0.7.K.
+0000a150: 3204 3004 4204 4c00 2000 2604 3d04 3504  2.0.B.L. .&.=.5.
+0000a160: 3004 3a04 4204 3804 3204 3d04 4b04 3508  0.:.B.8.2.=.K.5.
+0000a170: 0000 0000 0600 0000 0e53 686f 7720 2649  .........Show &I
+0000a180: 6e61 6374 6976 6507 0000 0010 4f70 6572  nactive.....Oper
+0000a190: 6174 696f 6e73 5769 6467 6574 0103 0000  ationsWidget....
+0000a1a0: 001a 0412 0430 043b 044e 0442 0430 0020  .....0.;.N.B.0. 
+0000a1b0: 0438 0442 043e 0433 043e 003a 0800 0000  .8.B.>.3.>.:....
+0000a1c0: 0006 0000 000d 5375 6d20 4375 7272 656e  ......Sum Curren
+0000a1d0: 6379 3a07 0000 0010 4f70 6572 6174 696f  cy:.....Operatio
+0000a1e0: 6e73 5769 6467 6574 0103 0000 0014 0064  nsWidget.......d
+0000a1f0: 0064 002f 004d 004d 002f 0079 0079 0079  .d./.M.M./.y.y.y
+0000a200: 0079 0800 0000 0006 0000 000a 6464 2f4d  .y..........dd/M
+0000a210: 4d2f 7979 7979 0700 0000 104f 7065 7261  M/yyyy.....Opera
+0000a220: 7469 6f6e 7357 6964 6765 7401 0300 0000  tionsWidget.....
+0000a230: 0c04 1204 3004 3b04 4e04 4204 3008 0000  ....0.;.N.B.0...
+0000a240: 0000 0600 0000 0843 7572 7265 6e63 7907  .......Currency.
+0000a250: 0000 0018 4f70 7469 6f6e 616c 4375 7272  ....OptionalCurr
+0000a260: 656e 6379 436f 6d62 6f42 6f78 0103 0000  encyComboBox....
+0000a270: 000a 0421 0443 043c 043c 0430 0800 0000  ...!.C.<.<.0....
+0000a280: 0006 0000 0006 416d 6f75 6e74 0700 0000  ......Amount....
+0000a290: 1050 616e 6461 734c 696e 6573 4d6f 6465  .PandasLinesMode
+0000a2a0: 6c01 0300 0000 1204 1a04 3004 4204 3504  l.........0.B.5.
+0000a2b0: 3304 3e04 4004 3804 4f08 0000 0000 0600  3.>.@.8.O.......
+0000a2c0: 0000 0843 6174 6567 6f72 7907 0000 0010  ...Category.....
+0000a2d0: 5061 6e64 6173 4c69 6e65 734d 6f64 656c  PandasLinesModel
+0000a2e0: 0103 0000 0022 041d 0430 0437 0432 0430  ....."...0.7.2.0
+0000a2f0: 043d 0438 0435 0020 043f 0440 043e 0434  .=.8.5. .?.@.>.4
+0000a300: 0443 043a 0442 0430 0800 0000 0006 0000  .C.:.B.0........
+0000a310: 000c 5072 6f64 7563 7420 6e61 6d65 0700  ..Product name..
+0000a320: 0000 1050 616e 6461 734c 696e 6573 4d6f  ...PandasLinesMo
+0000a330: 6465 6c01 0300 0000 0604 2204 4d04 3308  del.......".M.3.
+0000a340: 0000 0000 0600 0000 0354 6167 0700 0000  .........Tag....
+0000a350: 1050 616e 6461 734c 696e 6573 4d6f 6465  .PandasLinesMode
+0000a360: 6c01 0300 0000 2400 2700 2004 3704 3004  l.....$.'. .7.0.
+0000a370: 3c04 3504 3d04 3504 3d04 3000 2004 4304  <.5.=.5.=.0. .C.
+0000a380: 4104 3f04 3504 4804 3d04 3e08 0000 0000  A.?.5.H.=.>.....
+0000a390: 0600 0000 1b27 2077 6173 2073 7563 6365  .....' was succe
+0000a3a0: 7373 6675 6c6c 7920 7265 706c 6163 6564  ssfully replaced
+0000a3b0: 0700 0000 0e50 6565 724c 6973 7444 6961  .....PeerListDia
+0000a3c0: 6c6f 6701 0300 0000 0c00 2700 2004 3d04  log.......'. .=.
+0000a3d0: 3000 3a00 2008 0000 0000 0600 0000 0827  0.:. ..........'
+0000a3e0: 2077 6974 683a 2007 0000 000e 5065 6572   with: .....Peer
+0000a3f0: 4c69 7374 4469 616c 6f67 0103 0000 004e  ListDialog.....N
+0000a400: 0421 043e 0445 0440 0430 043d 0438 0442  .!.>.E.@.0.=.8.B
+0000a410: 044c 0020 0441 0442 0430 0440 043e 0435  .L. .A.B.0.@.>.5
+0000a420: 0020 043d 0430 0437 0432 0430 043d 0438  . .=.0.7.2.0.=.8
+0000a430: 0435 0020 0432 0020 043f 0440 0438 043c  .5. .2. .?.@.8.<
+0000a440: 0435 0447 0430 043d 0438 0438 003f 0800  .5.G.0.=.8.8.?..
+0000a450: 0000 0006 0000 0017 4b65 6570 206f 6c64  ........Keep old
+0000a460: 206e 616d 6520 696e 206e 6f74 6573 3f07   name in notes?.
+0000a470: 0000 000e 5065 6572 4c69 7374 4469 616c  ....PeerListDial
+0000a480: 6f67 0103 0000 0018 041a 043e 043d 0442  og.........>.=.B
+0000a490: 0440 0430 0433 0435 043d 0442 0020 0027  .@.0.3.5.=.B. .'
+0000a4a0: 0800 0000 0006 0000 0006 5065 6572 2027  ..........Peer '
+0000a4b0: 0700 0000 0e50 6565 724c 6973 7444 6961  .....PeerListDia
+0000a4c0: 6c6f 6701 0300 0000 1604 1a04 3e04 3d04  log.........>.=.
+0000a4d0: 4204 4004 3004 3304 3504 3d04 4204 4b08  B.@.0.3.5.=.B.K.
+0000a4e0: 0000 0000 0600 0000 0550 6565 7273 0700  .........Peers..
+0000a4f0: 0000 0e50 6565 724c 6973 7444 6961 6c6f  ...PeerListDialo
+0000a500: 6701 0300 0000 2c04 1704 3004 3c04 3504  g.....,...0.<.5.
+0000a510: 3d04 3804 4204 4c00 2004 3a04 3e04 3d04  =.8.B.L. .:.>.=.
+0000a520: 4204 4004 3004 3304 3504 3d04 4204 3000  B.@.0.3.5.=.B.0.
+0000a530: 2000 2708 0000 0000 0600 0000 0e52 6570   .'..........Rep
+0000a540: 6c61 6365 2070 6565 7220 2707 0000 000e  lace peer '.....
+0000a550: 5065 6572 4c69 7374 4469 616c 6f67 0103  PeerListDialog..
+0000a560: 0000 001c 0417 0430 043c 0435 043d 0438  .......0.<.5.=.8
+0000a570: 0442 044c 0020 043d 0430 002e 002e 002e  .B.L. .=.0......
+0000a580: 0800 0000 0006 0000 000f 5265 706c 6163  ..........Replac
+0000a590: 6520 7769 7468 2e2e 2e07 0000 000e 5065  e with........Pe
+0000a5a0: 6572 4c69 7374 4469 616c 6f67 0103 0000  erListDialog....
+0000a5b0: 0040 041f 043e 043a 0430 0437 0430 0442  .@...>.:.0.7.0.B
+0000a5c0: 044c 0020 043e 043f 0435 0440 0430 0446  .L. .>.?.5.@.0.F
+0000a5d0: 0438 0438 0020 0441 0020 041a 043e 043d  .8.8. .A. ...>.=
+0000a5e0: 0442 0440 0430 0433 0435 043d 0442 043e  .B.@.0.3.5.=.B.>
+0000a5f0: 043c 0800 0000 0006 0000 0019 5368 6f77  .<..........Show
+0000a600: 206f 7065 7261 7469 6f6e 7320 7769 7468   operations with
+0000a610: 2050 6565 7207 0000 000e 5065 6572 4c69   Peer.....PeerLi
+0000a620: 7374 4469 616c 6f67 0103 0000 0010 041e  stDialog........
+0000a630: 043f 0435 0440 0430 0446 0438 0438 0800  .?.5.@.0.F.8.8..
+0000a640: 0000 0006 0000 000a 4f70 6572 6174 696f  ........Operatio
+0000a650: 6e73 0700 0000 0a50 6565 7252 6570 6f72  ns.....PeerRepor
+0000a660: 7401 0300 0000 1c04 3f04 3e00 2004 1a04  t.......?.>. ...
+0000a670: 3e04 3d04 4204 4004 3004 3304 3504 3d04  >.=.B.@.0.3.5.=.
+0000a680: 4204 4308 0000 0000 0600 0000 0762 7920  B.C..........by 
+0000a690: 5065 6572 0700 0000 0a50 6565 7252 6570  Peer.....PeerRep
+0000a6a0: 6f72 7401 0300 0000 1604 1a04 3e04 3d04  ort.........>.=.
+0000a6b0: 4204 4004 3004 3304 3504 3d04 4200 3a08  B.@.0.3.5.=.B.:.
+0000a6c0: 0000 0000 0600 0000 0550 6565 723a 0700  .........Peer:..
+0000a6d0: 0000 1050 6565 7252 6570 6f72 7457 6964  ...PeerReportWid
+0000a6e0: 6765 7401 0300 0000 2804 1e04 4204 4704  get.....(...B.G.
+0000a6f0: 3504 4200 2004 3f04 3e00 2004 3a04 3e04  5.B. .?.>. .:.>.
+0000a700: 3d04 4204 4004 3004 3304 3504 3d04 4204  =.B.@.0.3.5.=.B.
+0000a710: 4308 0000 0000 0600 0000 0e52 6570 6f72  C..........Repor
+0000a720: 7420 6279 2070 6565 7207 0000 0010 5065  t by peer.....Pe
+0000a730: 6572 5265 706f 7274 5769 6467 6574 0103  erReportWidget..
+0000a740: 0000 0016 041a 043e 043b 002d 0432 043e  .......>.;.-.2.>
+0000a750: 0020 0434 043e 043a 002e 0800 0000 0006  . .4.>.:........
+0000a760: 0000 000a 446f 6373 2063 6f75 6e74 0700  ....Docs count..
+0000a770: 0000 0d50 6565 7254 7265 654d 6f64 656c  ...PeerTreeModel
+0000a780: 0103 0000 000a 0410 0434 0440 0435 0441  .........4.@.5.A
+0000a790: 0800 0000 0006 0000 0008 4c6f 6361 7469  ..........Locati
+0000a7a0: 6f6e 0700 0000 0d50 6565 7254 7265 654d  on.....PeerTreeM
+0000a7b0: 6f64 656c 0103 0000 0018 041d 0430 0438  odel.........0.8
+0000a7c0: 043c 0435 043d 043e 0432 0430 043d 0438  .<.5.=.>.2.0.=.8
+0000a7d0: 0435 0800 0000 0006 0000 0004 4e61 6d65  .5..........Name
+0000a7e0: 0700 0000 0d50 6565 7254 7265 654d 6f64  .....PeerTreeMod
+0000a7f0: 656c 0103 0000 001a 0421 0447 0435 0442  el.......!.G.5.B
+0000a800: 0430 0020 0432 0020 0431 0430 043d 043a  .0. .2. .1.0.=.:
+0000a810: 0435 0800 0000 0006 0000 000d 4261 6e6b  .5..........Bank
+0000a820: 2061 6363 6f75 6e74 7307 0000 0016 5072   accounts.....Pr
+0000a830: 6564 6566 696e 6465 6441 6363 6f75 6e74  edefindedAccount
+0000a840: 5479 7065 0103 0000 000a 041a 0430 0440  Type.........0.@
+0000a850: 0442 044b 0800 0000 0006 0000 0005 4361  .B.K..........Ca
+0000a860: 7264 7307 0000 0016 5072 6564 6566 696e  rds.....Predefin
+0000a870: 6465 6441 6363 6f75 6e74 5479 7065 0103  dedAccountType..
+0000a880: 0000 0010 041d 0430 043b 0438 0447 043d  .......0.;.8.G.=
+0000a890: 044b 0435 0800 0000 0006 0000 0004 4361  .K.5..........Ca
+0000a8a0: 7368 0700 0000 1650 7265 6465 6669 6e64  sh.....Predefind
+0000a8b0: 6564 4163 636f 756e 7454 7970 6501 0300  edAccountType...
+0000a8c0: 0000 1e04 1a04 4004 3504 3404 3804 4204  ......@.5.4.8.B.
+0000a8d0: 4b00 2000 2f00 2004 1404 3e04 3b04 3304  K. ./. ...>.;.3.
+0000a8e0: 3808 0000 0000 0600 0000 0d44 6562 7473  8..........Debts
+0000a8f0: 202f 204c 6f61 6e73 0700 0000 1650 7265   / Loans.....Pre
+0000a900: 6465 6669 6e64 6564 4163 636f 756e 7454  defindedAccountT
+0000a910: 7970 6501 0300 0000 1404 1804 3d04 3204  ype.........=.2.
+0000a920: 3504 4104 4204 3804 4604 3804 3808 0000  5.A.B.8.F.8.8...
+0000a930: 0000 0600 0000 0b49 6e76 6573 746d 656e  .......Investmen
+0000a940: 7473 0700 0000 1650 7265 6465 6669 6e64  ts.....Predefind
+0000a950: 6564 4163 636f 756e 7454 7970 6501 0300  edAccountType...
+0000a960: 0000 1404 2104 3104 3504 4004 3504 3604  ....!.1.5.@.5.6.
+0000a970: 3504 3d04 3804 4f08 0000 0000 0600 0000  5.=.8.O.........
+0000a980: 0753 6176 696e 6773 0700 0000 1650 7265  .Savings.....Pre
+0000a990: 6465 6669 6e64 6564 4163 636f 756e 7454  defindedAccountT
+0000a9a0: 7970 6501 0300 0000 1400 6500 2d04 1a04  ype.......e.-...
+0000a9b0: 3e04 4804 3504 3b04 4c04 3a04 3808 0000  >.H.5.;.L.:.8...
+0000a9c0: 0000 0600 0000 0965 2d57 616c 6c65 7473  .......e-Wallets
+0000a9d0: 0700 0000 1650 7265 6465 6669 6e64 6564  .....Predefinded
+0000a9e0: 4163 636f 756e 7454 7970 6501 0300 0000  AccountType.....
+0000a9f0: 1204 1e04 3104 3b04 3804 3304 3004 4604  ....1.;.8.3.0.F.
+0000aa00: 3804 3808 0000 0000 0600 0000 0542 6f6e  8.8..........Bon
+0000aa10: 6473 0700 0000 0f50 7265 6465 6669 6e65  ds.....Predefine
+0000aa20: 6441 7373 6574 0103 0000 000c 0422 043e  dAsset.......".>
+0000aa30: 0432 0430 0440 044b 0800 0000 0006 0000  .2.0.@.K........
+0000aa40: 000b 436f 6d6d 6f64 6974 6965 7307 0000  ..Commodities...
+0000aa50: 000f 5072 6564 6566 696e 6564 4173 7365  ..PredefinedAsse
+0000aa60: 7401 0300 0000 1804 1a04 4004 3804 3f04  t.........@.8.?.
+0000aa70: 4204 3e04 3204 3004 3b04 4e04 4204 4b08  B.>.2.0.;.N.B.K.
+0000aa80: 0000 0000 0600 0000 0f43 7279 7074 6f2d  .........Crypto-
+0000aa90: 6375 7272 656e 6379 0700 0000 0f50 7265  currency.....Pre
+0000aaa0: 6465 6669 6e65 6441 7373 6574 0103 0000  definedAsset....
+0000aab0: 0014 0414 0435 0440 0438 0432 0430 0442  .....5.@.8.2.0.B
+0000aac0: 0438 0432 044b 0800 0000 0006 0000 000b  .8.2.K..........
+0000aad0: 4465 7269 7661 7469 7665 7307 0000 000f  Derivatives.....
+0000aae0: 5072 6564 6566 696e 6564 4173 7365 7401  PredefinedAsset.
+0000aaf0: 0300 0000 0804 1104 1f04 1804 2408 0000  ............$...
+0000ab00: 0000 0600 0000 0445 5446 7307 0000 000f  .......ETFs.....
+0000ab10: 5072 6564 6566 696e 6564 4173 7365 7401  PredefinedAsset.
+0000ab20: 0300 0000 0c04 2404 3e04 4004 3504 3a04  ......$.>.@.5.:.
+0000ab30: 4108 0000 0000 0600 0000 0546 6f72 6578  A..........Forex
+0000ab40: 0700 0000 0f50 7265 6465 6669 6e65 6441  .....PredefinedA
+0000ab50: 7373 6574 0103 0000 000a 0424 043e 043d  sset.......$.>.=
+0000ab60: 0434 044b 0800 0000 0006 0000 0005 4675  .4.K..........Fu
+0000ab70: 6e64 7307 0000 000f 5072 6564 6566 696e  nds.....Predefin
+0000ab80: 6564 4173 7365 7401 0300 0000 0c04 1204  edAsset.........
+0000ab90: 3004 3b04 4e04 4204 4b08 0000 0000 0600  0.;.N.B.K.......
+0000aba0: 0000 054d 6f6e 6579 0700 0000 0f50 7265  ...Money.....Pre
 0000abb0: 6465 6669 6e65 6441 7373 6574 0103 0000  definedAsset....
-0000abc0: 0008 0411 041f 0418 0424 0800 0000 0006  .........$......
-0000abd0: 0000 0004 4554 4673 0700 0000 0f50 7265  ....ETFs.....Pre
-0000abe0: 6465 6669 6e65 6441 7373 6574 0103 0000  definedAsset....
-0000abf0: 000c 0424 043e 0440 0435 043a 0441 0800  ...$.>.@.5.:.A..
-0000ac00: 0000 0006 0000 0005 466f 7265 7807 0000  ........Forex...
-0000ac10: 000f 5072 6564 6566 696e 6564 4173 7365  ..PredefinedAsse
-0000ac20: 7401 0300 0000 0a04 2404 3e04 3d04 3404  t.......$.>.=.4.
-0000ac30: 4b08 0000 0000 0600 0000 0546 756e 6473  K..........Funds
-0000ac40: 0700 0000 0f50 7265 6465 6669 6e65 6441  .....PredefinedA
-0000ac50: 7373 6574 0103 0000 000c 0412 0430 043b  sset.........0.;
-0000ac60: 044e 0442 044b 0800 0000 0006 0000 0005  .N.B.K..........
-0000ac70: 4d6f 6e65 7907 0000 000f 5072 6564 6566  Money.....Predef
-0000ac80: 696e 6564 4173 7365 7401 0300 0000 0a04  inedAsset.......
-0000ac90: 1004 3a04 4604 3804 3808 0000 0000 0600  ..:.F.8.8.......
-0000aca0: 0000 0653 6861 7265 7307 0000 000f 5072  ...Shares.....Pr
-0000acb0: 6564 6566 696e 6564 4173 7365 7401 0300  edefinedAsset...
-0000acc0: 0000 0200 2508 0000 0000 0600 0000 0125  ....%..........%
-0000acd0: 0700 0000 0f50 726f 6669 744c 6f73 734d  .....ProfitLossM
-0000ace0: 6f64 656c 0103 0000 0006 0410 043f 0440  odel.........?.@
-0000acf0: 0800 0000 0006 0000 0003 4170 7207 0000  ..........Apr...
-0000ad00: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
-0000ad10: 6c01 0300 0000 0404 2604 1108 0000 0000  l.......&.......
-0000ad20: 0600 0000 0641 7373 6574 7307 0000 000f  .....Assets.....
-0000ad30: 5072 6f66 6974 4c6f 7373 4d6f 6465 6c01  ProfitLossModel.
-0000ad40: 0300 0000 0604 1004 3204 3308 0000 0000  ........2.3.....
-0000ad50: 0600 0000 0341 7567 0700 0000 0f50 726f  .....Aug.....Pro
-0000ad60: 6669 744c 6f73 734d 6f64 656c 0103 0000  fitLossModel....
-0000ad70: 0012 0418 0437 043c 0435 043d 0435 043d  .....7.<.5.=.5.=
-0000ad80: 0438 0435 0800 0000 0006 0000 0006 4368  .8.5..........Ch
-0000ad90: 616e 6765 0700 0000 0f50 726f 6669 744c  ange.....ProfitL
-0000ada0: 6f73 734d 6f64 656c 0103 0000 0018 0418  ossModel........
-0000adb0: 0437 043c 0435 043d 0435 043d 0438 0435  .7.<.5.=.5.=.8.5
-0000adc0: 002c 0020 0025 0800 0000 0006 0000 0009  .,. .%..........
-0000add0: 4368 616e 6765 2c20 2507 0000 000f 5072  Change, %.....Pr
-0000ade0: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
-0000adf0: 0000 0604 1404 3504 3a08 0000 0000 0600  ......5.:.......
-0000ae00: 0000 0344 6563 0700 0000 0f50 726f 6669  ...Dec.....Profi
-0000ae10: 744c 6f73 734d 6f64 656c 0103 0000 0012  tLossModel......
-0000ae20: 0414 0438 0432 0438 0434 0435 043d 0434  ...8.2.8.4.5.=.4
-0000ae30: 044b 0800 0000 0006 0000 0009 4469 7669  .K..........Divi
-0000ae40: 6465 6e64 7307 0000 000f 5072 6f66 6974  dends.....Profit
-0000ae50: 4c6f 7373 4d6f 6465 6c01 0300 0000 0604  LossModel.......
-0000ae60: 2404 3504 3208 0000 0000 0600 0000 0346  $.5.2..........F
-0000ae70: 6562 0700 0000 0f50 726f 6669 744c 6f73  eb.....ProfitLos
-0000ae80: 734d 6f64 656c 0103 0000 0010 041a 043e  sModel.........>
-0000ae90: 043c 0438 0441 0441 0438 0438 0800 0000  .<.8.A.A.8.8....
-0000aea0: 0006 0000 0004 4665 6573 0700 0000 0f50  ......Fees.....P
-0000aeb0: 726f 6669 744c 6f73 734d 6f64 656c 0103  rofitLossModel..
-0000aec0: 0000 0018 0412 0432 043e 0434 0020 002f  .......2.>.4. ./
-0000aed0: 0020 0412 044b 0432 043e 0434 0800 0000  . ...K.2.>.4....
-0000aee0: 0006 0000 0008 496e 202f 204f 7574 0700  ......In / Out..
-0000aef0: 0000 0f50 726f 6669 744c 6f73 734d 6f64  ...ProfitLossMod
-0000af00: 656c 0103 0000 0006 042f 043d 0432 0800  el......./.=.2..
-0000af10: 0000 0006 0000 0003 4a61 6e07 0000 000f  ........Jan.....
-0000af20: 5072 6f66 6974 4c6f 7373 4d6f 6465 6c01  ProfitLossModel.
-0000af30: 0300 0000 0604 1804 4e04 3b08 0000 0000  ........N.;.....
-0000af40: 0600 0000 034a 756c 0700 0000 0f50 726f  .....Jul.....Pro
-0000af50: 6669 744c 6f73 734d 6f64 656c 0103 0000  fitLossModel....
-0000af60: 0006 0418 044e 043d 0800 0000 0006 0000  .....N.=........
-0000af70: 0003 4a75 6e07 0000 000f 5072 6f66 6974  ..Jun.....Profit
-0000af80: 4c6f 7373 4d6f 6465 6c01 0300 0000 0604  LossModel.......
-0000af90: 1c04 3004 4008 0000 0000 0600 0000 034d  ..0.@..........M
-0000afa0: 6172 0700 0000 0f50 726f 6669 744c 6f73  ar.....ProfitLos
-0000afb0: 734d 6f64 656c 0103 0000 0006 041c 0430  sModel.........0
-0000afc0: 0439 0800 0000 0006 0000 0003 4d61 7907  .9..........May.
-0000afd0: 0000 000f 5072 6f66 6974 4c6f 7373 4d6f  ....ProfitLossMo
-0000afe0: 6465 6c01 0300 0000 0404 1404 2108 0000  del.........!...
-0000aff0: 0000 0600 0000 054d 6f6e 6579 0700 0000  .......Money....
-0000b000: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
-0000b010: 0103 0000 0006 041d 043e 044f 0800 0000  .........>.O....
-0000b020: 0006 0000 0003 4e6f 7607 0000 000f 5072  ......Nov.....Pr
-0000b030: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
-0000b040: 0000 0604 1e04 3a04 4208 0000 0000 0600  ......:.B.......
-0000b050: 0000 034f 6374 0700 0000 0f50 726f 6669  ...Oct.....Profi
-0000b060: 744c 6f73 734d 6f64 656c 0103 0000 0006  tLossModel......
-0000b070: 041f 0438 0423 0800 0000 0006 0000 0003  ...8.#..........
-0000b080: 5026 4c07 0000 000f 5072 6f66 6974 4c6f  P&L.....ProfitLo
-0000b090: 7373 4d6f 6465 6c01 0300 0000 0c04 1f04  ssModel.........
-0000b0a0: 3504 4004 3804 3e04 3408 0000 0000 0600  5.@.8.>.4.......
-0000b0b0: 0000 0650 6572 696f 6407 0000 000f 5072  ...Period.....Pr
-0000b0c0: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
-0000b0d0: 0000 1a04 1a04 3e04 3d04 3504 4600 2004  ......>.=.5.F. .
-0000b0e0: 3f04 3504 4004 3804 3e04 3404 3008 0000  ?.5.@.8.>.4.0...
-0000b0f0: 0000 0600 0000 0a50 6572 696f 6420 656e  .......Period en
-0000b100: 6407 0000 000f 5072 6f66 6974 4c6f 7373  d.....ProfitLoss
-0000b110: 4d6f 6465 6c01 0300 0000 1c04 1d04 3004  Model.........0.
-0000b120: 4704 3004 3b04 3e00 2004 3f04 3504 4004  G.0.;.>. .?.5.@.
-0000b130: 3804 3e04 3404 3008 0000 0000 0600 0000  8.>.4.0.........
-0000b140: 0c50 6572 696f 6420 7374 6172 7407 0000  .Period start...
-0000b150: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
-0000b160: 6c01 0300 0000 0604 2104 3504 3d08 0000  l.......!.5.=...
-0000b170: 0000 0600 0000 0353 6570 0700 0000 0f50  .......Sep.....P
-0000b180: 726f 6669 744c 6f73 734d 6f64 656c 0103  rofitLossModel..
-0000b190: 0000 000c 041d 0430 043b 043e 0433 0438  .......0.;.>.3.8
-0000b1a0: 0800 0000 0006 0000 0005 5461 7865 7307  ..........Taxes.
-0000b1b0: 0000 000f 5072 6f66 6974 4c6f 7373 4d6f  ....ProfitLossMo
-0000b1c0: 6465 6c01 0300 0000 0a04 1804 4204 3e04  del.........B.>.
-0000b1d0: 3304 3e08 0000 0000 0600 0000 0554 6f74  3.>..........Tot
-0000b1e0: 616c 0700 0000 0f50 726f 6669 744c 6f73  al.....ProfitLos
-0000b1f0: 734d 6f64 656c 0103 0000 0018 041f 0438  sModel.........8
-0000b200: 0423 0020 043f 043e 0020 0441 0447 0451  .#. .?.>. .A.G.Q
-0000b210: 0442 0443 0800 0000 0006 0000 000e 5026  .B.C..........P&
-0000b220: 4c20 6279 2041 6363 6f75 6e74 0700 0000  L by Account....
-0000b230: 1050 726f 6669 744c 6f73 7352 6570 6f72  .ProfitLossRepor
-0000b240: 7401 0300 0000 0a04 2104 4704 3504 4200  t.......!.G.5.B.
-0000b250: 3a08 0000 0000 0600 0000 0841 6363 6f75  :..........Accou
-0000b260: 6e74 3a07 0000 0016 5072 6f66 6974 4c6f  nt:.....ProfitLo
-0000b270: 7373 5265 706f 7274 5769 6467 6574 0103  ssReportWidget..
-0000b280: 0000 0010 0412 0430 043b 044e 0442 0430  .......0.;.N.B.0
-0000b290: 003a 0020 0800 0000 0006 0000 000a 4375  .:. ..........Cu
-0000b2a0: 7272 656e 6379 3a20 0700 0000 1650 726f  rrency: .....Pro
-0000b2b0: 6669 744c 6f73 7352 6570 6f72 7457 6964  fitLossReportWid
-0000b2c0: 6765 7401 0300 0000 0604 1f04 3804 2308  get.........8.#.
-0000b2d0: 0000 0000 0600 0000 0350 264c 0700 0000  .........P&L....
-0000b2e0: 1650 726f 6669 744c 6f73 7352 6570 6f72  .ProfitLossRepor
-0000b2f0: 7457 6964 6765 7401 0300 0000 1804 2104  tWidget.......!.
-0000b300: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
-0000b310: 2e00 2e00 2e08 0000 0000 0600 0000 0753  ...............S
-0000b320: 6176 652e 2e2e 0700 0000 1650 726f 6669  ave........Profi
-0000b330: 744c 6f73 7352 6570 6f72 7457 6964 6765  tLossReportWidge
-0000b340: 7401 0300 0000 1004 1204 3004 3b04 4e04  t.........0.;.N.
-0000b350: 4204 3000 3a00 2008 0000 0000 0600 0000  B.0.:. .........
-0000b360: 0a43 7572 7265 6e63 793a 2007 0000 0016  .Currency: .....
-0000b370: 5072 6f66 6974 4c6f 7373 5265 706f 7274  ProfitLossReport
-0000b380: 5769 6e64 6f77 0103 0000 0018 041f 0438  Window.........8
-0000b390: 0423 0020 043f 043e 0020 0441 0447 0451  .#. .?.>. .A.G.Q
-0000b3a0: 0442 0443 0800 0000 0006 0000 000e 5026  .B.C..........P&
-0000b3b0: 4c20 6279 2041 6363 6f75 6e74 0700 0000  L by Account....
-0000b3c0: 1650 726f 6669 744c 6f73 7352 6570 6f72  .ProfitLossRepor
-0000b3d0: 7457 696e 646f 7701 0300 0000 1e04 1e04  tWindow.........
-0000b3e0: 4804 3804 3104 3a04 3000 2004 3a04 3004  H.8.1.:.0. .:.0.
-0000b3f0: 3c04 3504 4004 4b00 3a00 2008 0000 0000  <.5.@.K.:. .....
-0000b400: 0600 0000 0e43 616d 6572 6120 6572 726f  .....Camera erro
-0000b410: 723a 2007 0000 0009 5152 5363 616e 6e65  r: .....QRScanne
-0000b420: 7201 0300 0000 8404 1d04 3500 2004 3e04  r.........5. .>.
-0000b430: 3104 3d04 3004 4004 4304 3604 3504 3d00  1.=.0.@.C.6.5.=.
-0000b440: 2004 3f04 3004 3a04 3504 4200 2000 7000   .?.0.:.5.B. .p.
-0000b450: 7900 7a00 6200 6100 7200 2c00 2004 3d04  y.z.b.a.r.,. .=.
-0000b460: 3504 3e04 3104 4504 3e04 3404 3804 3c04  5.>.1.E.>.4.8.<.
-0000b470: 4b04 3900 2004 3404 3b04 4f00 2004 4004  K.9. .4.;.O. .@.
-0000b480: 3004 4104 3f04 3e04 3704 3d04 3004 3204  0.A.?.>.7.=.0.2.
-0000b490: 3004 3d04 3804 4f00 2000 5100 5200 2004  0.=.8.O. .Q.R. .
-0000b4a0: 3a04 3e04 3404 3e04 3200 2e08 0000 0000  :.>.4.>.2.......
-0000b4b0: 0600 0000 2c50 6163 6b61 6765 2070 797a  ....,Package pyz
-0000b4c0: 6261 7220 6e6f 7420 666f 756e 6420 666f  bar not found fo
-0000b4d0: 7220 5152 2072 6563 6f67 6e69 7469 6f6e  r QR recognition
-0000b4e0: 2e07 0000 0009 5152 5363 616e 6e65 7201  ......QRScanner.
-0000b4f0: 0300 0000 2604 1d04 3504 4200 2004 3404  ....&...5.B. .4.
-0000b500: 3e04 4104 4204 4304 3f04 3d04 4b04 4500  >.A.B.C.?.=.K.E.
-0000b510: 2004 3a04 3004 3c04 3504 4008 0000 0000   .:.0.<.5.@.....
-0000b520: 0600 0000 1e54 6865 7265 2061 7265 206e  .....There are n
-0000b530: 6f20 6361 6d65 7261 7320 6176 6169 6c61  o cameras availa
-0000b540: 626c 6507 0000 0009 5152 5363 616e 6e65  ble.....QRScanne
-0000b550: 7201 0300 0000 6804 1d04 3504 3204 3e04  r.....h...5.2.>.
-0000b560: 3704 3c04 3e04 3604 3d04 3e00 2004 3e04  7.<.>.6.=.>. .>.
-0000b570: 3104 4004 3004 3104 3e04 4204 3004 4204  1.@.0.1.>.B.0.B.
-0000b580: 4c00 2004 3404 3004 3d04 3d04 4b04 3500  L. .4.0.=.=.K.5.
-0000b590: 2004 3a04 3e04 4204 3804 4004 3e04 3204   .:.>.B.8.@.>.2.
-0000b5a0: 3e04 3a00 2004 4100 2004 3104 3804 4004  >.:. .A. .1.8.@.
-0000b5b0: 3604 3800 2000 5400 5300 5800 3a00 2008  6.8. .T.S.X.:. .
-0000b5c0: 0000 0000 0600 0000 2143 616e 2774 2070  ........!Can't p
-0000b5d0: 6172 7365 2064 6174 6120 666f 7220 5453  arse data for TS
-0000b5e0: 5820 7175 6f74 6573 3a20 0700 0000 0f51  X quotes: .....Q
-0000b5f0: 756f 7465 446f 776e 6c6f 6164 6572 0103  uoteDownloader..
-0000b600: 0000 0024 0417 0430 0433 0440 0443 0437  ...$...0.3.@.C.7
-0000b610: 043a 0430 0020 0437 0430 0432 0435 0440  .:.0. .7.0.2.5.@
-0000b620: 0448 0435 043d 0430 0800 0000 0006 0000  .H.5.=.0........
-0000b630: 0012 446f 776e 6c6f 6164 2063 6f6d 706c  ..Download compl
-0000b640: 6574 6564 0700 0000 0f51 756f 7465 446f  eted.....QuoteDo
-0000b650: 776e 6c6f 6164 6572 0103 0000 0060 0049  wnloader.....`.I
-0000b660: 0053 0049 004e 0020 0432 0020 0438 0441  .S.I.N. .2. .8.A
-0000b670: 0442 043e 0440 0438 0438 0020 043a 043e  .B.>.@.8.8. .:.>
-0000b680: 0442 0438 0440 043e 0432 043e 043a 0020  .B.8.@.>.2.>.:. 
-0000b690: 0045 0075 0072 006f 006e 0065 0078 0074  .E.u.r.o.n.e.x.t
-0000b6a0: 0020 043d 0435 0020 0441 043e 0432 043f  . .=.5. .A.>.2.?
-0000b6b0: 0430 0434 0430 0435 0442 003a 0020 0800  .0.4.0.5.B.:. ..
-0000b6c0: 0000 0006 0000 0022 4575 726f 6e65 7874  ......."Euronext
-0000b6d0: 2071 756f 7465 7320 4953 494e 206d 6973   quotes ISIN mis
-0000b6e0: 6d61 7463 6820 696e 3a20 0700 0000 0f51  match in: .....Q
-0000b6f0: 756f 7465 446f 776e 6c6f 6164 6572 0103  uoteDownloader..
-0000b700: 0000 0064 0417 0430 0433 043e 043b 043e  ...d...0.3.>.;.>
-0000b710: 0432 043e 043a 0020 0438 0441 0442 043e  .2.>.:. .8.A.B.>
-0000b720: 0440 0438 0438 0020 043a 043e 0442 0438  .@.8.8. .:.>.B.8
-0000b730: 0440 043e 0432 043e 043a 0020 0045 0075  .@.>.2.>.:. .E.u
-0000b740: 0072 006f 006e 0065 0078 0074 0020 043d  .r.o.n.e.x.t. .=
-0000b750: 0435 0020 043d 0430 0439 0434 0435 043d  .5. .=.0.9.4.5.=
-0000b760: 0020 0432 003a 0020 0800 0000 0006 0000  . .2.:. ........
-0000b770: 0025 4575 726f 6e65 7874 2071 756f 7465  .%Euronext quote
-0000b780: 7320 6865 6164 6572 206e 6f74 2066 6f75  s header not fou
-0000b790: 6e64 2069 6e3a 2007 0000 000f 5175 6f74  nd in: .....Quot
-0000b7a0: 6544 6f77 6e6c 6f61 6465 7201 0300 0000  eDownloader.....
-0000b7b0: 5a04 1804 4104 4204 3e04 4004 3804 4f00  Z...A.B.>.@.8.O.
-0000b7c0: 2004 3a04 3e04 4204 3804 4004 3e04 3204   .:.>.B.8.@.>.2.
-0000b7d0: 3e04 3a00 2000 4500 7500 7200 6f00 6e00  >.:. .E.u.r.o.n.
-0000b7e0: 6500 7800 7400 2004 4104 3b04 3804 4804  e.x.t. .A.;.8.H.
-0000b7f0: 3a04 3e04 3c00 2004 3a04 3e04 4004 3e04  :.>.<. .:.>.@.>.
-0000b800: 4204 3a04 3004 4f00 3a00 2008 0000 0000  B.:.0.O.:. .....
-0000b810: 0600 0000 2c45 7572 6f6e 6578 7420 7175  ....,Euronext qu
-0000b820: 6f74 6573 2068 6973 746f 7279 2072 6570  otes history rep
-0000b830: 6c79 2069 7320 746f 6f20 7368 6f72 743a  ly is too short:
-0000b840: 2007 0000 000f 5175 6f74 6544 6f77 6e6c   .....QuoteDownl
-0000b850: 6f61 6465 7201 0300 0000 3604 1d04 3500  oader.....6...5.
-0000b860: 2004 3704 3004 3304 4004 4304 3604 3504   .7.0.3.@.C.6.5.
-0000b870: 3d04 4b00 2004 3a04 3e04 4204 3804 4004  =.K. .:.>.B.8.@.
-0000b880: 3e04 3204 3a04 3800 2004 3404 3b04 4f00  >.2.:.8. .4.;.O.
-0000b890: 2008 0000 0000 0600 0000 1e4e 6f20 7175   ..........No qu
-0000b8a0: 6f74 6573 2077 6572 6520 646f 776e 6c6f  otes were downlo
-0000b8b0: 6164 6564 2066 6f72 2007 0000 000f 5175  aded for .....Qu
-0000b8c0: 6f74 6544 6f77 6e6c 6f61 6465 7201 0300  oteDownloader...
-0000b8d0: 0000 2e04 1d04 3500 2004 3704 3004 3304  ......5. .7.0.3.
-0000b8e0: 4004 4304 3604 3504 3d04 4b00 2004 3a04  @.C.6.5.=.K. .:.
-0000b8f0: 4304 4004 4104 4b00 2004 3404 3b04 4f00  C.@.A.K. .4.;.O.
-0000b900: 2008 0000 0000 0600 0000 1d4e 6f20 7261   ..........No ra
-0000b910: 7465 7320 7765 7265 2064 6f77 6e6c 6f61  tes were downloa
-0000b920: 6465 6420 666f 7220 0700 0000 0f51 756f  ded for .....Quo
-0000b930: 7465 446f 776e 6c6f 6164 6572 0103 0000  teDownloader....
-0000b940: 002c 041d 0435 0442 0020 0434 0430 043d  .,...5.B. .4.0.=
-0000b950: 043d 044b 0445 0020 0426 0411 0020 0420  .=.K.E. .&... . 
-0000b960: 0424 0020 0434 043b 044f 003a 0020 0800  .$. .4.;.O.:. ..
-0000b970: 0000 0006 0000 001b 5468 6572 6520 6172  ........There ar
-0000b980: 6520 6e6f 2043 4252 2064 6174 6120 666f  e no CBR data fo
-0000b990: 723a 2007 0000 000f 5175 6f74 6544 6f77  r: .....QuoteDow
-0000b9a0: 6e6c 6f61 6465 7201 0300 0000 1204 1a04  nloader.........
-0000b9b0: 3e04 4204 3804 4004 3e04 3204 3a04 3808  >.B.8.@.>.2.:.8.
-0000b9c0: 0000 0000 0600 0000 0651 756f 7465 7307  .........Quotes.
-0000b9d0: 0000 0010 5175 6f74 6573 4c69 7374 4469  ....QuotesListDi
-0000b9e0: 616c 6f67 0103 0000 0004 0426 0411 0800  alog.......&....
-0000b9f0: 0000 0006 0000 0005 4173 7365 7407 0000  ........Asset...
-0000ba00: 000f 5175 6f74 6573 4c69 7374 4d6f 6465  ..QuotesListMode
-0000ba10: 6c01 0300 0000 0c04 1204 3004 3b04 4e04  l.........0.;.N.
-0000ba20: 4204 3008 0000 0000 0600 0000 0843 7572  B.0..........Cur
-0000ba30: 7265 6e63 7907 0000 000f 5175 6f74 6573  rency.....Quotes
-0000ba40: 4c69 7374 4d6f 6465 6c01 0300 0000 0804  ListModel.......
-0000ba50: 1404 3004 4204 3008 0000 0000 0600 0000  ..0.B.0.........
-0000ba60: 0444 6174 6507 0000 000f 5175 6f74 6573  .Date.....Quotes
-0000ba70: 4c69 7374 4d6f 6465 6c01 0300 0000 1204  ListModel.......
-0000ba80: 1a04 3e04 4204 3804 4004 3e04 3204 3a04  ..>.B.8.@.>.2.:.
-0000ba90: 3008 0000 0000 0600 0000 0551 756f 7465  0..........Quote
-0000baa0: 0700 0000 0f51 756f 7465 734c 6973 744d  .....QuotesListM
-0000bab0: 6f64 656c 0103 0000 0028 0026 041f 043e  odel.....(.&...>
-0000bac0: 043b 043d 043e 0441 0442 044c 044e 002c  .;.=.>.A.B.L.N.,
-0000bad0: 0020 0441 0020 043d 0430 0447 0430 043b  . .A. .=.0.G.0.;
-0000bae0: 0430 0800 0000 0006 0000 0013 2646 756c  .0..........&Ful
-0000baf0: 6c2c 2066 726f 6d20 7363 7261 7463 6807  l, from scratch.
-0000bb00: 0000 000d 5265 4275 696c 6444 6961 6c6f  ....ReBuildDialo
-0000bb10: 6701 0300 0000 1804 1804 3d04 4204 3504  g.........=.B.5.
-0000bb20: 4004 3204 3004 3b00 2004 3404 3004 4208  @.2.0.;. .4.0.B.
-0000bb30: 0000 0000 0600 0000 0a44 6174 6520 5261  .........Date Ra
-0000bb40: 6e67 6507 0000 000d 5265 4275 696c 6444  nge.....ReBuildD
-0000bb50: 6961 6c6f 6701 0300 0000 2a00 2604 1104  ialog.....*.&...
-0000bb60: 4b04 4104 4204 4004 3e00 2c00 2004 3d04  K.A.B.@.>.,. .=.
-0000bb70: 3e00 2004 3d04 3504 3d04 3004 3404 5104  >. .=.5.=.0.4.Q.
-0000bb80: 3604 3d04 3e08 0000 0000 0600 0000 1146  6.=.>..........F
-0000bb90: 6173 742c 2026 756e 7265 6c69 6162 6c65  ast, &unreliable
-0000bba0: 0700 0000 0d52 6542 7569 6c64 4469 616c  .....ReBuildDial
-0000bbb0: 6f67 0103 0000 0016 0414 0430 0442 0430  og.........0.B.0
-0000bbc0: 0413 0440 0430 043d 0438 0446 044b 0800  ...@.0.=.8.F.K..
-0000bbd0: 0000 0006 0000 000c 4672 6f6e 7469 6572  ........Frontier
-0000bbe0: 4461 7465 0700 0000 0d52 6542 7569 6c64  Date.....ReBuild
-0000bbf0: 4469 616c 6f67 0103 0000 0022 041f 0435  Dialog....."...5
-0000bc00: 0440 0435 0441 0447 0438 0442 0430 0442  .@.5.A.G.8.B.0.B
-0000bc10: 044c 0020 0438 0442 043e 0433 0438 0800  .L. .8.B.>.3.8..
-0000bc20: 0000 0006 0000 000f 5265 2d42 7569 6c64  ........Re-Build
-0000bc30: 204c 6564 6765 7207 0000 000d 5265 4275   Ledger.....ReBu
-0000bc40: 696c 6444 6961 6c6f 6701 0300 0000 1004  ildDialog.......
-0000bc50: 2100 2000 2604 1404 3004 4204 4b00 3a08  !. .&...0.B.K.:.
-0000bc60: 0000 0000 0600 0000 0c53 696e 6365 2026  .........Since &
-0000bc70: 4461 7465 3a07 0000 000d 5265 4275 696c  Date:.....ReBuil
-0000bc80: 6444 6961 6c6f 6701 0300 0000 2c04 2100  dDialog.....,.!.
-0000bc90: 2004 3a04 4004 3004 3904 3d04 3504 3900   .:.@.0.9.=.5.9.
-0000bca0: 2000 2604 3004 3a04 4204 4304 3004 3b04   .&.0.:.B.C.0.;.
-0000bcb0: 4c04 3d04 3e04 3900 3a08 0000 0000 0600  L.=.>.9.:.......
-0000bcc0: 0000 1353 696e 6365 2026 4c61 7374 2061  ...Since &Last a
-0000bcd0: 6374 7561 6c3a 0700 0000 0d52 6542 7569  ctual:.....ReBui
-0000bce0: 6c64 4469 616c 6f67 0103 0000 0014 0064  ldDialog.......d
-0000bcf0: 0064 002f 004d 004d 002f 0079 0079 0079  .d./.M.M./.y.y.y
-0000bd00: 0079 0800 0000 0006 0000 000a 6464 2f4d  .y..........dd/M
-0000bd10: 4d2f 7979 7979 0700 0000 0d52 6542 7569  M/yyyy.....ReBui
-0000bd20: 6c64 4469 616c 6f67 0103 0000 000a 041b  ldDialog........
-0000bd30: 044e 0431 043e 0439 0800 0000 0006 0000  .N.1.>.9........
-0000bd40: 0003 414e 5907 0000 0013 5265 6665 7265  ..ANY.....Refere
-0000bd50: 6e63 6544 6174 6144 6961 6c6f 6701 0300  nceDataDialog...
-0000bd60: 0000 1404 2204 3804 3f00 2004 4104 4704  ....".8.?. .A.G.
-0000bd70: 3504 4204 3000 3a08 0000 0000 0600 0000  5.B.0.:.........
-0000bd80: 0d41 6363 6f75 6e74 2054 7970 653a 0700  .Account Type:..
-0000bd90: 0000 1352 6566 6572 656e 6365 4461 7461  ...ReferenceData
-0000bda0: 4469 616c 6f67 0103 0000 0022 0414 043e  Dialog....."...>
-0000bdb0: 0431 0430 0432 0438 0442 044c 0020 0434  .1.0.2.8.B.L. .4
-0000bdc0: 043e 0447 0435 0440 043d 0438 0439 0800  .>.G.5.@.=.8.9..
-0000bdd0: 0000 0006 0000 0009 4164 6420 6368 696c  ........Add chil
-0000bde0: 6407 0000 0013 5265 6665 7265 6e63 6544  d.....ReferenceD
-0000bdf0: 6174 6144 6961 6c6f 6701 0300 0000 1c04  ataDialog.......
-0000be00: 1404 3e04 3104 3004 3204 3804 4204 4c00  ..>.1.0.2.8.B.L.
-0000be10: 2004 3d04 3e04 3204 4b04 3908 0000 0000   .=.>.2.K.9.....
-0000be20: 0600 0000 0741 6464 206e 6577 0700 0000  .....Add new....
-0000be30: 1352 6566 6572 656e 6365 4461 7461 4469  .ReferenceDataDi
-0000be40: 616c 6f67 0103 0000 001e 0421 043c 0435  alog.......!.<.5
-0000be50: 043d 0438 0442 044c 0020 0442 0438 043f  .=.8.B.L. .B.8.?
-0000be60: 0020 043d 0430 003a 0800 0000 0006 0000  . .=.0.:........
-0000be70: 000f 4368 616e 6765 2074 7970 6520 746f  ..Change type to
-0000be80: 3a07 0000 0013 5265 6665 7265 6e63 6544  :.....ReferenceD
-0000be90: 6174 6144 6961 6c6f 6701 0300 0000 1a04  ataDialog.......
-0000bea0: 1f04 3e04 3404 4204 3204 3504 4004 3604  ..>.4.B.2.5.@.6.
-0000beb0: 3404 3504 3d04 3804 3508 0000 0000 0600  4.5.=.8.5.......
-0000bec0: 0000 0c43 6f6e 6669 726d 6174 696f 6e07  ...Confirmation.
-0000bed0: 0000 0013 5265 6665 7265 6e63 6544 6174  ....ReferenceDat
-0000bee0: 6144 6961 6c6f 6701 0300 0000 0e04 2304  aDialog.......#.
-0000bef0: 3404 3004 3b04 3804 4204 4c08 0000 0000  4.0.;.8.B.L.....
-0000bf00: 0600 0000 0644 656c 6574 6507 0000 0013  .....Delete.....
-0000bf10: 5265 6665 7265 6e63 6544 6174 6144 6961  ReferenceDataDia
-0000bf20: 6c6f 6701 0300 0000 2204 2104 3f04 4004  log.....".!.?.@.
-0000bf30: 3004 3204 3e04 4704 3d04 4b04 3500 2004  0.2.>.G.=.K.5. .
-0000bf40: 3404 3004 3d04 3d04 4b04 3508 0000 0000  4.0.=.=.K.5.....
-0000bf50: 0600 0000 0e52 6566 6572 656e 6365 2044  .....Reference D
-0000bf60: 6174 6107 0000 0013 5265 6665 7265 6e63  ata.....Referenc
-0000bf70: 6544 6174 6144 6961 6c6f 6701 0300 0000  eDataDialog.....
-0000bf80: 2404 1e04 4204 3c04 3504 3d04 3804 4204  $...B.<.5.=.8.B.
-0000bf90: 4c00 2004 3804 3704 3c04 3504 3d04 3504  L. .8.7.<.5.=.5.
-0000bfa0: 3d04 3804 4f08 0000 0000 0600 0000 0e52  =.8.O..........R
-0000bfb0: 6576 6572 7420 6368 616e 6765 7307 0000  evert changes...
-0000bfc0: 0013 5265 6665 7265 6e63 6544 6174 6144  ..ReferenceDataD
-0000bfd0: 6961 6c6f 6701 0300 0000 2604 2104 3e04  ialog.....&.!.>.
-0000bfe0: 4504 4004 3004 3d04 3804 4204 4c00 2004  E.@.0.=.8.B.L. .
-0000bff0: 3804 3704 3c04 3504 3d04 3504 3d04 3804  8.7.<.5.=.5.=.8.
-0000c000: 4f08 0000 0000 0600 0000 0c53 6176 6520  O..........Save 
-0000c010: 6368 616e 6765 7307 0000 0013 5265 6665  changes.....Refe
-0000c020: 7265 6e63 6544 6174 6144 6961 6c6f 6701  renceDataDialog.
-0000c030: 0300 0000 0c04 1f04 3e04 3804 4104 3a00  ........>.8.A.:.
-0000c040: 3a08 0000 0000 0600 0000 0753 6561 7263  :..........Searc
-0000c050: 683a 0700 0000 1352 6566 6572 656e 6365  h:.....Reference
-0000c060: 4461 7461 4469 616c 6f67 0103 0000 002a  DataDialog.....*
-0000c070: 041f 043e 043a 0430 0437 044b 0432 0430  ...>.:.0.7.K.2.0
-0000c080: 0442 044c 0020 043d 0435 0430 043a 0442  .B.L. .=.5.0.:.B
-0000c090: 0438 0432 043d 044b 0435 0800 0000 0006  .8.2.=.K.5......
-0000c0a0: 0000 000d 5368 6f77 2069 6e61 6374 6976  ....Show inactiv
-0000c0b0: 6507 0000 0013 5265 6665 7265 6e63 6544  e.....ReferenceD
-0000c0c0: 6174 6144 6961 6c6f 6701 0300 0000 6604  ataDialog.....f.
-0000c0d0: 2300 2004 3204 3004 4100 2004 3504 4104  #. .2.0.A. .5.A.
-0000c0e0: 4204 4c00 2004 3d04 3504 4104 3e04 4504  B.L. .=.5.A.>.E.
-0000c0f0: 4004 3004 3d04 5104 3d04 3d04 4b04 3500  @.0.=.Q.=.=.K.5.
-0000c100: 2004 3404 3004 3d04 3d04 4b04 3500 2e00   .4.0.=.=.K.5...
-0000c110: 2004 1204 4104 5100 2004 4004 3004 3204   ...A.Q. .@.0.2.
-0000c120: 3d04 3e00 2004 3704 3004 3a04 4004 4b04  =.>. .7.0.:.@.K.
-0000c130: 4204 4c00 3f08 0000 0000 0600 0000 3359  B.L.?.........3Y
-0000c140: 6f75 2068 6176 6520 756e 636f 6d6d 6974  ou have uncommit
-0000c150: 7465 6420 6368 616e 6765 732e 2044 6f20  ted changes. Do 
-0000c160: 796f 7520 7761 6e74 2074 6f20 636c 6f73  you want to clos
-0000c170: 653f 0700 0000 1352 6566 6572 656e 6365  e?.....Reference
-0000c180: 4461 7461 4469 616c 6f67 0103 0000 0028  DataDialog.....(
-0000c190: 0424 0430 0439 043b 044b 0020 0045 0078  .$.0.9.;.K. .E.x
-0000c1a0: 0063 0065 006c 0020 0028 002a 002e 0078  .c.e.l. .(.*...x
-0000c1b0: 0073 006c 0078 0029 0800 0000 0006 0000  .s.l.x.)........
-0000c1c0: 0014 4578 6365 6c20 6669 6c65 7320 282a  ..Excel files (*
-0000c1d0: 2e78 6c73 7829 0700 0000 0752 6570 6f72  .xlsx).....Repor
-0000c1e0: 7473 0103 0000 0046 041d 0435 0432 043e  ts.....F...5.2.>
-0000c1f0: 0437 043c 043e 0436 043d 043e 0020 0437  .7.<.>.6.=.>. .7
-0000c200: 0430 0433 0440 0443 0437 0438 0442 044c  .0.3.@.C.7.8.B.L
-0000c210: 0020 043a 043b 0430 0441 0441 0020 043e  . .:.;.0.A.A. .>
-0000c220: 0442 0447 0451 0442 0430 003a 0020 0800  .B.G.Q.B.0.:. ..
-0000c230: 0000 0006 0000 001e 5265 706f 7274 2063  ........Report c
-0000c240: 6c61 7373 2063 616e 2774 2062 6520 6c6f  lass can't be lo
-0000c250: 6164 6564 3a20 0700 0000 0752 6570 6f72  aded: .....Repor
-0000c260: 7473 0103 0000 0042 041e 0442 0447 0435  ts.....B...B.G.5
-0000c270: 0442 0020 043d 0435 0020 043d 0430 0439  .B. .=.5. .=.0.9
-0000c280: 0434 0435 043d 0020 0434 043b 044f 0020  .4.5.=. .4.;.O. 
-0000c290: 043a 043b 0430 0441 0441 0430 0020 043e  .:.;.0.A.A.0. .>
-0000c2a0: 043a 043d 0430 003a 0020 0800 0000 0006  .:.=.0.:. ......
-0000c2b0: 0000 0023 5265 706f 7274 206e 6f74 2066  ...#Report not f
-0000c2c0: 6f75 6e64 2066 6f72 2077 696e 646f 7720  ound for window 
-0000c2d0: 636c 6173 733a 2007 0000 0007 5265 706f  class: .....Repo
-0000c2e0: 7274 7301 0300 0000 2c04 1e04 4204 4704  rts.....,...B.G.
-0000c2f0: 3504 4200 2004 4104 3e04 4504 4004 3004  5.B. .A.>.E.@.0.
-0000c300: 3d04 5104 3d00 2004 3200 2004 4404 3004  =.Q.=. .2. .D.0.
-0000c310: 3904 3b00 2008 0000 0000 0600 0000 1952  9.;. ..........R
-0000c320: 6570 6f72 7420 7761 7320 7361 7665 6420  eport was saved 
-0000c330: 746f 2066 696c 6520 0700 0000 0752 6570  to file .....Rep
-0000c340: 6f72 7473 0103 0000 0024 0421 043e 0445  orts.....$.!.>.E
-0000c350: 0440 0430 043d 0438 0442 044c 0020 043e  .@.0.=.8.B.L. .>
-0000c360: 0442 0447 0435 0442 0020 0432 003a 0800  .B.G.5.B. .2.:..
-0000c370: 0000 0006 0000 000f 5361 7665 2072 6570  ........Save rep
-0000c380: 6f72 7420 746f 3a07 0000 0007 5265 706f  ort to:.....Repo
-0000c390: 7274 7301 0300 0000 3c04 1b04 3e04 3304  rts.....<...>.3.
-0000c3a0: 3804 3d00 2004 4704 3504 4004 3504 3700  8.=. .G.5.@.5.7.
-0000c3b0: 2004 1304 3e04 4104 4304 4104 3b04 4304   ...>.A.C.A.;.C.
-0000c3c0: 3304 3800 2004 3704 3004 3204 3504 4004  3.8. .7.0.2.5.@.
-0000c3d0: 4804 5104 3d08 0000 0000 0600 0000 1445  H.Q.=..........E
-0000c3e0: 5349 4120 6c6f 6769 6e20 636f 6d70 6c65  SIA login comple
-0000c3f0: 7465 6407 0000 0012 5265 7175 6573 7449  ted.....RequestI
-0000c400: 6e74 6572 6365 7074 6f72 0103 0000 000a  nterceptor......
-0000c410: 0410 043a 0442 0438 0432 0800 0000 0006  ...:.B.8.2......
-0000c420: 0000 0005 4173 7365 7407 0000 000c 5265  ....Asset.....Re
-0000c430: 7375 6c74 734d 6f64 656c 0103 0000 000c  sultsModel......
-0000c440: 041a 043e 043b 002d 0432 043e 0800 0000  ...>.;.-.2.>....
-0000c450: 0006 0000 0003 5174 7907 0000 000c 5265  ......Qty.....Re
-0000c460: 7375 6c74 734d 6f64 656c 0103 0000 000e  sultsModel......
-0000c470: 0414 043e 043b 044f 002c 0020 0025 0800  ...>.;.O.,. .%..
-0000c480: 0000 0006 0000 0008 5368 6172 652c 2025  ........Share, %
-0000c490: 0700 0000 0c52 6573 756c 7473 4d6f 6465  .....ResultsMode
-0000c4a0: 6c01 0300 0000 3004 1204 4b04 3104 4004  l.....0...K.1.@.
-0000c4b0: 3004 3d00 2004 3d04 3504 3a04 3e04 4004  0.=. .=.5.:.>.@.
-0000c4c0: 4004 3504 3a04 4204 3d04 4b04 3900 2004  @.5.:.B.=.K.9. .
-0000c4d0: 4104 4704 5104 4208 0000 0000 0600 0000  A.G.Q.B.........
-0000c4e0: 1849 6e76 616c 6964 2061 6363 6f75 6e74  .Invalid account
-0000c4f0: 2073 656c 6563 7465 6407 0000 0013 5365   selected.....Se
-0000c500: 6c65 6374 4163 636f 756e 7444 6961 6c6f  lectAccountDialo
-0000c510: 6701 0300 0000 2204 1d04 3804 4704 3504  g....."...8.G.5.
-0000c520: 3304 3e00 2004 3d04 3500 2004 3204 4b04  3.>. .=.5. .2.K.
-0000c530: 3104 4004 3004 3d04 3e08 0000 0000 0600  1.@.0.=.>.......
-0000c540: 0000 0c4e 6f20 7365 6c65 6374 696f 6e07  ...No selection.
-0000c550: 0000 0013 5365 6c65 6374 4163 636f 756e  ....SelectAccoun
-0000c560: 7444 6961 6c6f 6701 0300 0000 4004 1f04  tDialog.....@...
-0000c570: 3e04 3604 3004 3b04 4304 3904 4104 4204  >.6.0.;.C.9.A.B.
-0000c580: 3000 2c00 2004 3204 4b04 3104 3504 4004  0.,. .2.K.1.5.@.
-0000c590: 3804 4204 3500 2004 3404 4004 4304 3304  8.B.5. .4.@.C.3.
-0000c5a0: 3e04 3900 2004 4104 4704 5104 4208 0000  >.9. .A.G.Q.B...
-0000c5b0: 0000 0600 0000 1f50 6c65 6173 6520 7365  .......Please se
-0000c5c0: 6c65 6374 2064 6966 6665 7265 6e74 2061  lect different a
-0000c5d0: 6363 6f75 6e74 0700 0000 1353 656c 6563  ccount.....Selec
-0000c5e0: 7441 6363 6f75 6e74 4469 616c 6f67 0103  tAccountDialog..
-0000c5f0: 0000 0030 041f 043e 0436 0430 043b 0443  ...0...>.6.0.;.C
-0000c600: 0439 0441 0442 0430 0020 0432 044b 0431  .9.A.B.0. .2.K.1
-0000c610: 0435 0440 0438 0442 0435 0020 0441 0447  .5.@.8.B.5. .A.G
-0000c620: 0451 0442 0800 0000 0006 0000 0015 506c  .Q.B..........Pl
-0000c630: 6561 7365 2073 656c 6563 7420 6163 636f  ease select acco
-0000c640: 756e 7407 0000 0010 5365 6c65 6374 4163  unt.....SelectAc
-0000c650: 636f 756e 7444 6c67 0103 0000 0012 0421  countDlg.......!
-0000c660: 043e 043e 0431 0449 0435 043d 0438 0435  .>.>.1.I.5.=.8.5
-0000c670: 0800 0000 0006 0000 0009 5465 7874 4c61  ..........TextLa
-0000c680: 6265 6c07 0000 0010 5365 6c65 6374 4163  bel.....SelectAc
-0000c690: 636f 756e 7444 6c67 0103 0000 0056 0418  countDlg.....V..
-0000c6a0: 0441 043f 043e 043b 044c 0437 043e 0432  .A.?.>.;.L.7.>.2
-0000c6b0: 0430 0442 044c 0020 044d 0442 043e 0442  .0.B.L. .M.B.>.B
-0000c6c0: 0020 0436 0435 0020 0441 0447 0451 0442  . .6.5. .A.G.Q.B
-0000c6d0: 0020 0434 043b 044f 0020 0434 0430 043d  . .4.;.O. .4.0.=
-0000c6e0: 043d 043e 0439 0020 0432 0430 043b 044e  .=.>.9. .2.0.;.N
-0000c6f0: 0442 044b 0800 0000 0006 0000 0027 5573  .B.K.........'Us
-0000c700: 6520 7468 6520 7361 6d65 2061 6363 6f75  e the same accou
-0000c710: 6e74 2066 6f72 2067 6976 656e 2063 7572  nt for given cur
-0000c720: 7265 6e63 7907 0000 0010 5365 6c65 6374  rency.....Select
-0000c730: 4163 636f 756e 7444 6c67 0103 0000 0024  AccountDlg.....$
-0000c740: 0412 044b 0431 0435 0440 0438 0442 0435  ...K.1.5.@.8.B.5
-0000c750: 0020 043a 0430 0442 0435 0433 043e 0440  . .:.0.B.5.3.>.@
-0000c760: 0438 044e 0800 0000 0006 0000 0016 506c  .8.N..........Pl
-0000c770: 6561 7365 2073 656c 6563 7420 6361 7465  ease select cate
-0000c780: 676f 7279 0700 0000 1453 656c 6563 7443  gory.....SelectC
-0000c790: 6174 6567 6f72 7944 6961 6c6f 6701 0300  ategoryDialog...
-0000c7a0: 0000 2804 1204 4b04 3104 3504 4004 3804  ..(...K.1.5.@.8.
-0000c7b0: 4204 3500 2004 3a04 3e04 3d04 4204 4004  B.5. .:.>.=.B.@.
-0000c7c0: 3004 3304 3504 3d04 4204 3008 0000 0000  0.3.5.=.B.0.....
-0000c7d0: 0600 0000 1250 6c65 6173 6520 7365 6c65  .....Please sele
-0000c7e0: 6374 2070 6565 7207 0000 0010 5365 6c65  ct peer.....Sele
-0000c7f0: 6374 5065 6572 4469 616c 6f67 0103 0000  ctPeerDialog....
-0000c800: 0022 041d 0438 0447 0435 0433 043e 0020  ."...8.G.5.3.>. 
-0000c810: 043d 0435 0020 0432 044b 0431 0440 0430  .=.5. .2.K.1.@.0
-0000c820: 043d 043e 0800 0000 0006 0000 000c 4e6f  .=.>..........No
-0000c830: 2073 656c 6563 7469 6f6e 0700 0000 1553   selection.....S
-0000c840: 656c 6563 7452 6566 6572 656e 6365 4469  electReferenceDi
-0000c850: 616c 6f67 0103 0000 002e 0412 044b 0020  alog.........K. 
-0000c860: 0434 043e 043b 0436 043d 044b 0020 0441  .4.>.;.6.=.K. .A
-0000c870: 0434 0435 043b 0430 0442 044c 0020 0432  .4.5.;.0.B.L. .2
-0000c880: 044b 0431 043e 0440 0800 0000 0006 0000  .K.1.>.@........
-0000c890: 001b 596f 7520 7368 6f75 6c64 2073 656c  ..You should sel
-0000c8a0: 6563 7420 736f 6d65 7468 696e 6707 0000  ect something...
-0000c8b0: 0015 5365 6c65 6374 5265 6665 7265 6e63  ..SelectReferenc
-0000c8c0: 6544 6961 6c6f 6701 0300 0000 1c04 1204  eDialog.........
-0000c8d0: 4b04 3104 3504 4004 3804 4204 3500 2004  K.1.5.@.8.B.5. .
-0000c8e0: 3c04 3504 4204 3a04 4308 0000 0000 0600  <.5.B.:.C.......
-0000c8f0: 0000 1150 6c65 6173 6520 7365 6c65 6374  ...Please select
-0000c900: 2074 6167 0700 0000 0f53 656c 6563 7454   tag.....SelectT
-0000c910: 6167 4469 616c 6f67 0103 0000 005a 041d  agDialog.....Z..
-0000c920: 0435 0020 0443 0434 0430 043b 043e 0441  .5. .C.4.0.;.>.A
-0000c930: 044c 0020 043f 043e 043b 0443 0447 0438  .L. .?.>.;.C.G.8
-0000c940: 0442 044c 0020 043d 0430 0437 0432 0430  .B.L. .=.0.7.2.0
-0000c950: 043d 0438 0435 0020 043e 0433 0440 0430  .=.8.5. .>.3.@.0
-0000c960: 043d 0438 0437 0430 0446 0438 0438 0020  .=.8.7.0.F.8.8. 
-0000c970: 0438 0437 003a 0020 0800 0000 0006 0000  .8.7.:. ........
-0000c980: 001d 4361 6e27 7420 6765 7420 636f 6d70  ..Can't get comp
-0000c990: 616e 7920 6e61 6d65 2066 726f 6d3a 2007  any name from: .
-0000c9a0: 0000 000b 536c 6970 7354 6178 4150 4901  ....SlipsTaxAPI.
-0000c9b0: 0300 0000 4804 1d04 3504 3204 3e04 3704  ....H...5.2.>.7.
-0000c9c0: 3c04 3e04 3604 3d04 3e00 2004 3e04 3104  <.>.6.=.>. .>.1.
-0000c9d0: 3204 3d04 3e04 3204 3804 4204 4c00 2004  2.=.>.2.8.B.L. .
-0000c9e0: 4104 3504 4104 4104 3804 4e00 2c00 2004  A.5.A.A.8.N.,. .
-0000c9f0: 3e04 4204 3204 3504 4200 3a00 2008 0000  >.B.2.5.B.:. ...
-0000ca00: 0000 0600 0000 2143 616e 2774 2072 6566  ......!Can't ref
-0000ca10: 7265 7368 2073 6573 7369 6f6e 2c20 7265  resh session, re
-0000ca20: 7370 6f6e 7365 3a20 0700 0000 0b53 6c69  sponse: .....Sli
-0000ca30: 7073 5461 7841 5049 0103 0000 002e 041e  psTaxAPI........
-0000ca40: 0448 0438 0431 043a 0430 0020 043f 043e  .H.8.1.:.0. .?.>
-0000ca50: 043b 0443 0447 0435 043d 0438 044f 0020  .;.C.G.5.=.8.O. 
-0000ca60: 0447 0435 043a 0430 003a 0020 0800 0000  .G.5.:.0.:. ....
-0000ca70: 0006 0000 0013 4765 7420 7469 636b 6574  ......Get ticket
-0000ca80: 2066 6169 6c65 643a 2007 0000 000b 536c   failed: .....Sl
-0000ca90: 6970 7354 6178 4150 4901 0300 0000 3404  ipsTaxAPI.....4.
-0000caa0: 1e04 4804 3804 3104 3a04 3000 2004 3f04  ..H.8.1.:.0. .?.
-0000cab0: 3e04 3b04 4304 4704 3504 3d04 3804 4f00  >.;.C.G.5.=.8.O.
-0000cac0: 2000 6900 6400 2004 4704 3504 3a04 3000   .i.d. .G.5.:.0.
-0000cad0: 3a00 2008 0000 0000 0600 0000 1647 6574  :. ..........Get
-0000cae0: 2074 6963 6b65 7420 6964 2066 6169 6c65   ticket id faile
-0000caf0: 643a 2007 0000 000b 536c 6970 7354 6178  d: .....SlipsTax
-0000cb00: 4150 4901 0300 0000 7c04 1d04 3504 3204  API.....|...5.2.
-0000cb10: 3504 4004 3d04 3004 4f00 2004 3404 3b04  5.@.=.0.O. .4.;.
-0000cb20: 3804 3d04 3000 2004 1804 1d04 1d00 2e00  8.=.0. .........
-0000cb30: 2004 1d04 3504 3204 3e04 3704 3c04 3e04   ...5.2.>.7.<.>.
-0000cb40: 3604 3d04 3e00 2004 3f04 3e04 3b04 4304  6.=.>. .?.>.;.C.
-0000cb50: 4704 3804 4204 4c00 2004 3d04 3004 3804  G.8.B.L. .=.0.8.
-0000cb60: 3c04 3504 3d04 3e04 3204 3004 3d04 3804  <.5.=.>.2.0.=.8.
-0000cb70: 3500 2004 3a04 3e04 3c04 3f04 3004 3d04  5. .:.>.<.?.0.=.
-0000cb80: 3804 3800 2e08 0000 0000 0600 0000 3049  8.8...........0I
-0000cb90: 6e63 6f72 7265 6374 206c 656e 6774 6820  ncorrect length 
-0000cba0: 6f66 2049 4e4e 2e20 4361 6e27 7420 6765  of INN. Can't ge
-0000cbb0: 7420 636f 6d70 616e 7920 6e61 6d65 2e07  t company name..
-0000cbc0: 0000 000b 536c 6970 7354 6178 4150 4901  ....SlipsTaxAPI.
-0000cbd0: 0300 0000 5604 1d04 3504 4200 2000 5300  ....V...5.B. .S.
-0000cbe0: 6500 7300 7300 6900 6f00 6e00 4900 6400  e.s.s.i.o.n.I.d.
-0000cbf0: 2004 3404 3b04 4f00 2004 3704 3004 3304   .4.;.O. .7.0.3.
-0000cc00: 4004 4304 3704 3a04 3800 2004 4704 3504  @.C.7.:.8. .G.5.
-0000cc10: 3a04 3000 2004 4100 2004 4104 3004 3904  :.0. .A. .A.0.9.
-0000cc20: 4204 3000 2004 2404 1d04 2108 0000 0000  B.0. .$...!.....
-0000cc30: 0600 0000 224e 6f20 5275 7373 6961 6e20  ...."No Russian 
-0000cc40: 5461 7820 5365 7373 696f 6e49 6420 6176  Tax SessionId av
-0000cc50: 6169 6c61 626c 6507 0000 000b 536c 6970  ailable.....Slip
-0000cc60: 7354 6178 4150 4901 0300 0000 3604 1d04  sTaxAPI.....6...
-0000cc70: 3504 4200 2004 3004 3a04 4204 3804 3204  5.B. .0.:.B.8.2.
-0000cc80: 3d04 3e04 3900 2004 4104 3504 4104 4104  =.>.9. .A.5.A.A.
-0000cc90: 3804 3800 2004 3404 3b04 4f00 2004 2404  8.8. .4.;.O. .$.
-0000cca0: 1d04 2108 0000 0000 0600 0000 184e 6f20  ..!..........No 
-0000ccb0: 7661 6c69 6420 7365 7373 696f 6e20 7072  valid session pr
-0000ccc0: 6573 656e 7407 0000 000b 536c 6970 7354  esent.....SlipsT
-0000ccd0: 6178 4150 4901 0300 0000 7a04 1e04 3f04  axAPI.....z...?.
-0000cce0: 3504 4004 3004 4604 3804 4f00 2004 3e04  5.@.0.F.8.O. .>.
-0000ccf0: 3104 4004 3004 3104 3004 4204 4b04 3204  1.@.0.1.0.B.K.2.
-0000cd00: 3004 3504 4204 4104 4f00 2004 3d04 3000  0.5.B.A.O. .=.0.
-0000cd10: 2004 4104 4204 3e04 4004 3e04 3d04 3500   .A.B.>.@.>.=.5.
-0000cd20: 2004 4104 3504 4004 3204 3504 4004 3000   .A.5.@.2.5.@.0.
-0000cd30: 2e00 2004 1f04 3e04 3204 4204 3e04 4004  .. ...>.2.B.>.@.
-0000cd40: 4f04 4e00 2004 3504 4904 5100 2004 4004  O.N. .5.I.Q. .@.
-0000cd50: 3004 3700 2e08 0000 0000 0600 0000 384f  0.7...........8O
-0000cd60: 7065 7261 7469 6f6e 206d 6967 6874 2062  peration might b
-0000cd70: 6520 7065 6e64 696e 6720 6f6e 2073 6572  e pending on ser
-0000cd80: 7665 7220 7369 6465 2e20 5472 7969 6e67  ver side. Trying
-0000cd90: 2061 6761 696e 2e07 0000 000b 536c 6970   again......Slip
-0000cda0: 7354 6178 4150 4901 0300 0000 2804 1e04  sTaxAPI.....(...
-0000cdb0: 3104 3d04 3e04 3204 3b04 3504 3d04 3804  1.=.>.2.;.5.=.8.
-0000cdc0: 3500 2004 4104 3504 4104 4104 3804 3800  5. .A.5.A.A.8.8.
-0000cdd0: 2e00 2e00 2e08 0000 0000 0600 0000 1552  ...............R
-0000cde0: 6566 7265 7368 696e 6720 7365 7373 696f  efreshing sessio
-0000cdf0: 6e2e 2e2e 0700 0000 0b53 6c69 7073 5461  n........SlipsTa
-0000ce00: 7841 5049 0103 0000 0024 0421 0435 0441  xAPI.....$.!.5.A
-0000ce10: 0441 0438 044f 0020 043e 0431 043d 043e  .A.8.O. .>.1.=.>
-0000ce20: 0432 043b 0435 043d 0430 003a 0020 0800  .2.;.5.=.0.:. ..
-0000ce30: 0000 0006 0000 0013 5365 7373 696f 6e20  ........Session 
-0000ce40: 7265 6672 6573 6865 643a 2007 0000 000b  refreshed: .....
-0000ce50: 536c 6970 7354 6178 4150 4901 0300 0000  SlipsTaxAPI.....
-0000ce60: 1804 2704 3504 3a00 2004 3d04 3004 3904  ..'.5.:. .=.0.9.
-0000ce70: 3404 3504 3d00 3a00 2008 0000 0000 0600  4.5.=.:. .......
-0000ce80: 0000 0c53 6c69 7020 666f 756e 643a 2007  ...Slip found: .
-0000ce90: 0000 000b 536c 6970 7354 6178 4150 4901  ....SlipsTaxAPI.
-0000cea0: 0300 0000 1c04 2704 3504 3a00 2004 3704  ......'.5.:. .7.
-0000ceb0: 3004 3304 4004 4304 3604 3504 3d00 3a00  0.3.@.C.6.5.=.:.
-0000cec0: 2008 0000 0000 0600 0000 0d53 6c69 7020   ..........Slip 
-0000ced0: 6c6f 6164 6564 3a20 0700 0000 0b53 6c69  loaded: .....Sli
-0000cee0: 7073 5461 7841 5049 0103 0000 0036 041d  psTaxAPI.....6..
-0000cef0: 0435 0430 0432 0442 043e 0440 0438 0437  .5.0.2.B.>.@.8.7
-0000cf00: 043e 0432 0430 043d 043e 0020 043f 043e  .>.2.0.=.>. .?.>
-0000cf10: 0020 043f 0440 0438 0447 0438 043d 0435  . .?.@.8.G.8.=.5
-0000cf20: 003a 0020 0800 0000 0006 0000 001a 556e  .:. ..........Un
-0000cf30: 6175 7468 6f72 697a 6564 2077 6974 6820  authorized with 
-0000cf40: 7265 6173 6f6e 3a20 0700 0000 0b53 6c69  reason: .....Sli
-0000cf50: 7073 5461 7841 5049 0103 0000 001c 0421  psTaxAPI.......!
-0000cf60: 0447 0451 0442 0020 043d 0435 0020 0432  .G.Q.B. .=.5. .2
-0000cf70: 044b 0431 0440 0430 043d 0800 0000 0006  .K.1.@.0.=......
-0000cf80: 0000 0014 4163 636f 756e 7420 6e6f 7420  ....Account not 
-0000cf90: 7365 6c65 6374 6564 0700 0000 0953 7461  selected.....Sta
-0000cfa0: 7465 6d65 6e74 0103 0000 0034 0414 0430  tement.....4...0
-0000cfb0: 043d 043d 044b 0435 0020 043d 0435 0020  .=.=.K.5. .=.5. 
-0000cfc0: 043f 0440 0438 0432 044f 0437 0430 043d  .?.@.8.2.O.7.0.=
-0000cfd0: 044b 0020 043a 0020 0426 0411 003a 0020  .K. .:. .&...:. 
-0000cfe0: 0800 0000 0006 0000 0023 4173 7365 7420  .........#Asset 
-0000cff0: 6461 7461 2061 7265 6e27 7420 6c69 6e6b  data aren't link
-0000d000: 6564 2074 6f20 6173 7365 743a 2007 0000  ed to asset: ...
-0000d010: 0009 5374 6174 656d 656e 7401 0300 0000  ..Statement.....
-0000d020: 1e04 2604 1100 2000 6900 6400 2004 3d04  ..&... .i.d. .=.
-0000d030: 3500 2004 3d04 3004 3904 3404 3504 3d08  5. .=.0.9.4.5.=.
-0000d040: 0000 0000 0600 0000 1241 7373 6574 2069  .........Asset i
-0000d050: 6420 6e6f 7420 666f 756e 6407 0000 0009  d not found.....
-0000d060: 5374 6174 656d 656e 7401 0300 0000 3204  Statement.....2.
-0000d070: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
-0000d080: 3d04 3e00 2004 4104 3e04 3704 3404 3004  =.>. .A.>.7.4.0.
-0000d090: 4204 4c00 2004 4104 4704 5104 4200 3a00  B.L. .A.G.Q.B.:.
-0000d0a0: 2008 0000 0000 0600 0000 1643 616e 2774   ..........Can't
-0000d0b0: 2063 7265 6174 6520 6163 636f 756e 743a   create account:
-0000d0c0: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
-0000d0d0: 0300 0000 2e04 1d04 3504 3204 3e04 3704  ........5.2.>.7.
-0000d0e0: 3c04 3e04 3604 3d04 3e00 2004 4104 3e04  <.>.6.=.>. .A.>.
-0000d0f0: 3704 3404 3004 4204 4c00 2004 2604 1100  7.4.0.B.L. .&...
-0000d100: 3a00 2008 0000 0000 0600 0000 1443 616e  :. ..........Can
-0000d110: 2774 2063 7265 6174 6520 6173 7365 743a  't create asset:
-0000d120: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
-0000d130: 0300 0000 3c04 1d04 3504 3204 3e04 3704  ....<...5.2.>.7.
-0000d140: 3c04 3e04 3604 3d04 3e00 2004 3d04 3004  <.>.6.=.>. .=.0.
-0000d150: 3904 4204 3500 2004 2604 1100 2004 3200  9.B.5. .&... .2.
-0000d160: 2004 3e04 4204 4704 5104 4204 3500 3a00   .>.B.G.Q.B.5.:.
-0000d170: 2008 0000 0000 0600 0000 2643 616e 2774   .........&Can't
-0000d180: 206c 6f63 6174 6520 6173 7365 7420 696e   locate asset in
-0000d190: 2073 7461 7465 6d65 6e74 2064 6174 613a   statement data:
-0000d1a0: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
-0000d1b0: 0300 0000 1a04 1f04 3e04 3404 4204 3204  ........>.4.B.2.
-0000d1c0: 3504 4004 3604 3404 3504 3d04 3804 3508  5.@.6.4.5.=.8.5.
-0000d1d0: 0000 0000 0600 0000 0c43 6f6e 6669 726d  .........Confirm
-0000d1e0: 6174 696f 6e07 0000 0009 5374 6174 656d  ation.....Statem
-0000d1f0: 656e 7401 0300 0000 4404 1e04 4204 3b04  ent.....D...B.;.
-0000d200: 3004 3404 3e04 4704 3d04 3004 4f00 2004  0.4.>.G.=.0.O. .
-0000d210: 3804 3d04 4404 3e04 4004 3c04 3004 4604  8.=.D.>.@.<.0.F.
-0000d220: 3804 4f00 2004 4104 3e04 4504 4004 3004  8.O. .A.>.E.@.0.
-0000d230: 3d04 3504 3d04 3000 2004 3200 2008 0000  =.5.=.0. .2. ...
-0000d240: 0000 0600 0000 1e44 6562 7567 2069 6e66  .......Debug inf
-0000d250: 6f72 6d61 7469 6f6e 2069 7320 7361 7665  ormation is save
-0000d260: 6420 696e 2007 0000 0009 5374 6174 656d  d in .....Statem
-0000d270: 656e 7401 0300 0000 1004 1404 3504 3f04  ent.........5.?.
-0000d280: 3e04 3704 3804 4200 2008 0000 0000 0600  >.7.8.B. .......
-0000d290: 0000 0b44 6570 6f73 6974 206f 6620 0700  ...Deposit of ..
-0000d2a0: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
-0000d2b0: 0048 041d 0435 0432 043e 0437 043c 043e  .H...5.2.>.7.<.>
-0000d2c0: 0436 043d 043e 0020 043f 0440 043e 0447  .6.=.>. .?.@.>.G
-0000d2d0: 0438 0442 0430 0442 044c 0020 004a 0053  .8.B.0.B.L. .J.S
-0000d2e0: 004f 004e 0020 0438 0437 0020 0444 0430  .O.N. .8.7. .D.0
-0000d2f0: 0439 043b 0430 003a 0020 0800 0000 0006  .9.;.0.:. ......
-0000d300: 0000 001f 4661 696c 6564 2074 6f20 7265  ....Failed to re
-0000d310: 6164 204a 534f 4e20 6672 6f6d 2066 696c  ad JSON from fil
-0000d320: 653a 2007 0000 0009 5374 6174 656d 656e  e: .....Statemen
-0000d330: 7401 0300 0000 4804 1d04 3500 2004 4304  t.....H...5. .C.
-0000d340: 3404 3004 3b04 3e04 4104 4c00 2004 3f04  4.0.;.>.A.L. .?.
-0000d350: 4004 3e04 4704 3804 4204 3004 4204 4c00  @.>.G.8.B.0.B.L.
-0000d360: 2004 4104 4504 3504 3c04 4300 2000 4a00   .A.E.5.<.C. .J.
-0000d370: 5300 4f00 4e00 2004 3804 3700 3a00 2008  S.O.N. .8.7.:. .
-0000d380: 0000 0000 0600 0000 2146 6169 6c65 6420  ........!Failed 
-0000d390: 746f 2072 6561 6420 4a53 4f4e 2073 6368  to read JSON sch
-0000d3a0: 656d 6120 6672 6f6d 3a20 0700 0000 0953  ema from: .....S
-0000d3b0: 7461 7465 6d65 6e74 0103 0000 0034 041d  tatement.....4..
-0000d3c0: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-0000d3d0: 043e 0020 043f 0440 043e 0447 0435 0441  .>. .?.@.>.G.5.A
-0000d3e0: 0442 044c 0020 0444 0430 0439 043b 003a  .B.L. .D.0.9.;.:
-0000d3f0: 0020 0800 0000 0006 0000 0015 4661 696c  . ..........Fail
-0000d400: 6564 2074 6f20 7265 6164 2066 696c 653a  ed to read file:
-0000d410: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
-0000d420: 0300 0000 5a04 1e04 4804 3804 3104 3a04  ....Z...H.8.1.:.
-0000d430: 3000 2004 3f04 4004 3800 2004 4104 3e04  0. .?.@.8. .A.>.
-0000d440: 4504 4004 3004 3d04 3504 3d04 3804 3800  E.@.0.=.5.=.8.8.
-0000d450: 2004 3e04 4204 3b04 3004 3404 3e04 4704   .>.B.;.0.4.>.G.
-0000d460: 3d04 3e04 3900 2004 3804 3d04 4404 3e04  =.>.9. .8.=.D.>.
-0000d470: 4004 3c04 3004 4604 3804 3800 3a00 2008  @.<.0.F.8.8.:. .
-0000d480: 0000 0000 0600 0000 2546 6169 6c65 6420  ........%Failed 
-0000d490: 746f 2077 7269 7465 2073 7461 7465 6d65  to write stateme
-0000d4a0: 6e74 2064 756d 7020 696e 746f 3a20 0700  nt dump into: ..
-0000d4b0: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
-0000d4c0: 0066 041d 0435 0432 043e 0437 043c 043e  .f...5.2.>.7.<.>
-0000d4d0: 0436 043d 043e 0020 043a 043e 043d 0442  .6.=.>. .:.>.=.B
-0000d4e0: 0432 0435 0440 0442 0438 0440 043e 0432  .2.5.@.B.8.@.>.2
-0000d4f0: 0430 0442 044c 0020 0442 0438 043f 0020  .0.B.L. .B.8.?. 
-0000d500: 0430 043a 0442 0438 0432 0430 0020 0432  .0.:.B.8.2.0. .2
-0000d510: 0020 0442 0440 0430 043d 0441 0444 0435  . .B.@.0.=.A.D.5
-0000d520: 0440 0435 003a 0020 0800 0000 0006 0000  .@.5.:. ........
-0000d530: 002e 496d 706f 7373 6962 6c65 2074 6f20  ..Impossible to 
-0000d540: 636f 6e76 6572 7420 6173 7365 7420 7479  convert asset ty
-0000d550: 7065 2069 6e20 7472 616e 7366 6572 3a20  pe in transfer: 
-0000d560: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
-0000d570: 0000 0048 041d 0435 043e 0434 043d 043e  ...H...5.>.4.=.>
-0000d580: 0437 043d 0430 0447 043d 043e 0435 0020  .7.=.0.G.=.>.5. 
-0000d590: 0441 043e 0432 043f 0430 0434 0435 043d  .A.>.2.?.0.4.5.=
-0000d5a0: 0438 0435 0020 0432 0430 043b 044e 0442  .8.5. .2.0.;.N.B
-0000d5b0: 044b 0020 0434 043b 044f 0020 0800 0000  .K. .4.;.O. ....
-0000d5c0: 0006 0000 001c 4d75 6c74 6970 6c65 2063  ......Multiple c
-0000d5d0: 7572 7265 6e63 7920 6d61 7463 6820 666f  urrency match fo
-0000d5e0: 7220 0700 0000 0953 7461 7465 6d65 6e74  r .....Statement
-0000d5f0: 0103 0000 003a 041d 0435 043e 0434 043d  .....:...5.>.4.=
-0000d600: 043e 0437 043d 0430 0447 043d 043e 0435  .>.7.=.0.G.=.>.5
-0000d610: 0020 0441 043e 0432 043f 0430 0434 0435  . .A.>.2.?.0.4.5
-0000d620: 043d 0438 0435 0020 0434 043b 044f 0020  .=.8.5. .4.;.O. 
-0000d630: 0800 0000 0006 0000 0013 4d75 6c74 6970  ..........Multip
-0000d640: 6c65 206d 6174 6368 2066 6f72 2007 0000  le match for ...
-0000d650: 0009 5374 6174 656d 656e 7401 0300 0000  ..Statement.....
-0000d660: 3a04 1204 4b04 3104 3504 4004 3804 4204  :...K.1.5.@.8.B.
-0000d670: 3500 2004 4104 4704 5104 4200 2004 3404  5. .A.G.Q.B. .4.
-0000d680: 3b04 4f00 2004 3704 3004 4704 3804 4104  ;.O. .7.0.G.8.A.
-0000d690: 3b04 3504 3d04 3804 4f00 3a08 0000 0000  ;.5.=.8.O.:.....
-0000d6a0: 0600 0000 1d53 656c 6563 7420 6163 636f  .....Select acco
-0000d6b0: 756e 7420 746f 2064 6570 6f73 6974 2074  unt to deposit t
-0000d6c0: 6f3a 0700 0000 0953 7461 7465 6d65 6e74  o:.....Statement
-0000d6d0: 0103 0000 0036 0412 044b 0431 0435 0440  .....6...K.1.5.@
-0000d6e0: 0438 0442 0435 0020 0441 0447 0451 0442  .8.B.5. .A.G.Q.B
-0000d6f0: 0020 0434 043b 044f 0020 0441 043f 0438  . .4.;.O. .A.?.8
-0000d700: 0441 0430 043d 0438 044f 003a 0800 0000  .A.0.=.8.O.:....
-0000d710: 0006 0000 0020 5365 6c65 6374 2061 6363  ..... Select acc
-0000d720: 6f75 6e74 2074 6f20 7769 7468 6472 6177  ount to withdraw
-0000d730: 2066 726f 6d3a 0700 0000 0953 7461 7465   from:.....State
-0000d740: 6d65 6e74 0103 0000 0048 041d 0435 043a  ment.....H...5.:
-0000d750: 043e 0442 043e 0440 044b 0435 0020 0441  .>.B.>.@.K.5. .A
-0000d760: 0435 043a 0446 0438 0438 0020 043d 0435  .5.:.F.8.8. .=.5
-0000d770: 0020 043f 043e 0434 0434 0435 0440 0436  . .?.>.4.4.5.@.6
-0000d780: 0438 0432 0430 044e 0442 0441 044f 003a  .8.2.0.N.B.A.O.:
-0000d790: 0020 0800 0000 0006 0000 0021 536f 6d65  . .........!Some
-0000d7a0: 2073 6563 7469 6f6e 7320 6172 6520 6e6f   sections are no
-0000d7b0: 7420 7375 7070 6f72 7465 643a 2007 0000  t supported: ...
-0000d7c0: 0009 5374 6174 656d 656e 7401 0300 0000  ..Statement.....
-0000d7d0: 2a04 1804 3c04 3f04 3e04 4004 4200 2004  *...<.?.>.@.B. .
-0000d7e0: 3e04 4204 4704 5104 4204 3000 2004 3f04  >.B.G.Q.B.0. .?.
-0000d7f0: 4004 3504 4004 3204 3004 3d08 0000 0000  @.5.@.2.0.=.....
-0000d800: 0600 0000 1e53 7461 7465 6d65 6e74 2069  .....Statement i
-0000d810: 6d70 6f72 7420 7761 7320 6361 6e63 656c  mport was cancel
-0000d820: 6c65 6407 0000 0009 5374 6174 656d 656e  led.....Statemen
-0000d830: 7401 0300 0000 2c04 1d04 3504 3204 3504  t.....,...5.2.5.
-0000d840: 4004 3d04 4b04 3900 2004 3f04 3504 4004  @.=.K.9. .?.5.@.
-0000d850: 3804 3e04 3400 2004 3e04 4204 4704 5104  8.>.4. .>.B.G.Q.
-0000d860: 4204 3008 0000 0000 0600 0000 1b53 7461  B.0..........Sta
-0000d870: 7465 6d65 6e74 2070 6572 696f 6420 6973  tement period is
-0000d880: 2069 6e76 616c 6964 0700 0000 0953 7461   invalid.....Sta
-0000d890: 7465 6d65 6e74 0103 0000 00c6 041f 0435  tement.........5
-0000d8a0: 0440 0438 043e 0434 0020 043e 0442 0447  .@.8.>.4. .>.B.G
-0000d8b0: 0451 0442 0430 0020 043d 0430 0447 0438  .Q.B.0. .=.0.G.8
-0000d8c0: 043d 0430 0435 0442 0441 044f 0020 0440  .=.0.5.B.A.O. .@
-0000d8d0: 0430 043d 0435 0435 0020 043f 043e 0441  .0.=.5.5. .?.>.A
-0000d8e0: 043b 0435 0434 043d 0435 0439 0020 043e  .;.5.4.=.5.9. .>
-0000d8f0: 043f 0435 0440 0430 0446 0438 0438 0020  .?.5.@.0.F.8.8. 
-0000d900: 0434 043b 044f 0020 0441 0447 0451 0442  .4.;.O. .A.G.Q.B
-0000d910: 0430 0020 0028 043f 043e 0432 0442 043e  .0. .(.?.>.2.B.>
-0000d920: 0440 043d 044b 0439 0020 0438 043c 043f  .@.=.K.9. .8.<.?
-0000d930: 043e 0440 0442 003f 0029 002e 0020 041f  .>.@.B.?.)... ..
-0000d940: 0440 043e 0434 043e 043b 0436 0438 0442  .@.>.4.>.;.6.8.B
-0000d950: 044c 0020 0438 043c 043f 043e 0440 0442  .L. .8.<.?.>.@.B
-0000d960: 003f 0800 0000 0006 0000 0058 5374 6174  .?.........XStat
-0000d970: 656d 656e 7420 7065 7269 6f64 2073 7461  ement period sta
-0000d980: 7274 7320 6265 666f 7265 206c 6173 7420  rts before last 
-0000d990: 7265 636f 7264 6564 206f 7065 7261 7469  recorded operati
-0000d9a0: 6f6e 2066 6f72 2074 6865 2061 6363 6f75  on for the accou
-0000d9b0: 6e74 2e20 436f 6e74 696e 7565 2069 6d70  nt. Continue imp
-0000d9c0: 6f72 743f 0700 0000 0953 7461 7465 6d65  ort?.....Stateme
-0000d9d0: 6e74 0103 0000 002a 041e 0442 0447 0451  nt.....*...B.G.Q
-0000d9e0: 0442 0020 0441 043e 0434 0435 0440 0436  .B. .A.>.4.5.@.6
-0000d9f0: 0438 0442 0020 043e 0448 0438 0431 043a  .8.B. .>.H.8.1.:
-0000da00: 0438 0800 0000 0006 0000 001b 5374 6174  .8..........Stat
-0000da10: 656d 656e 7420 7661 6c69 6461 7469 6f6e  ement validation
-0000da20: 2066 6169 6c65 6407 0000 0009 5374 6174   failed.....Stat
-0000da30: 656d 656e 7401 0300 0000 4004 2104 3804  ement.....@.!.8.
-0000da40: 3c04 3204 3e04 3b00 2004 3204 3004 3b04  <.2.>.;. .2.0.;.
-0000da50: 4e04 4204 4b00 2004 3d04 3500 2004 3f04  N.B.K. .=.5. .?.
-0000da60: 4004 3804 3204 4f04 3704 3004 3d00 2004  @.8.2.O.7.0.=. .
-0000da70: 3a00 2004 2604 1100 3a00 2008 0000 0000  :. .&...:. .....
-0000da80: 0600 0000 2753 796d 626f 6c20 6375 7272  ....'Symbol curr
-0000da90: 656e 6379 2069 736e 2774 206c 696e 6b65  ency isn't linke
-0000daa0: 6420 746f 2061 7373 6574 3a20 0700 0000  d to asset: ....
-0000dab0: 0953 7461 7465 6d65 6e74 0103 0000 0032  .Statement.....2
-0000dac0: 0421 0438 043c 0432 043e 043b 0020 043d  .!.8.<.2.>.;. .=
-0000dad0: 0435 0020 043f 0440 0438 0432 044f 0437  .5. .?.@.8.2.O.7
-0000dae0: 0430 043d 0020 043a 0020 0426 0411 003a  .0.=. .:. .&...:
-0000daf0: 0020 0800 0000 0006 0000 0025 5379 6d62  . .........%Symb
-0000db00: 6f6c 2074 6963 6b65 7220 6973 6e27 7420  ol ticker isn't 
-0000db10: 6c69 6e6b 6564 2074 6f20 6173 7365 743a  linked to asset:
-0000db20: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
-0000db30: 0300 0000 7204 1d04 3504 3204 3e04 3704  ....r...5.2.>.7.
-0000db40: 3c04 3e04 3604 3d04 3e00 2004 4104 3e04  <.>.6.=.>. .A.>.
-0000db50: 3f04 3e04 4104 4204 3004 3204 3804 4204  ?.>.A.B.0.2.8.B.
-0000db60: 4c00 2004 4104 4704 5104 4200 2004 3404  L. .A.G.Q.B. .4.
-0000db70: 3b04 4f00 2004 3a04 3e04 4004 3f04 3e04  ;.O. .:.>.@.?.>.
-0000db80: 4004 3004 4204 3804 3204 3d04 3e04 3304  @.0.B.8.2.=.>.3.
-0000db90: 3e00 2004 3404 3504 3904 4104 4204 3204  >. .4.5.9.A.B.2.
-0000dba0: 3804 4f00 3a00 2008 0000 0000 0600 0000  8.O.:. .........
-0000dbb0: 2855 6e6d 6174 6368 6564 2061 6363 6f75  (Unmatched accou
-0000dbc0: 6e74 2066 6f72 2063 6f72 706f 7261 7465  nt for corporate
-0000dbd0: 2061 6374 696f 6e3a 2007 0000 0009 5374   action: .....St
-0000dbe0: 6174 656d 656e 7401 0300 0000 7404 1d04  atement.....t...
-0000dbf0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
-0000dc00: 3e00 2004 4104 3e04 3f04 3e04 4104 4204  >. .A.>.?.>.A.B.
-0000dc10: 3004 3204 3804 4204 4c00 2004 4104 4704  0.2.8.B.L. .A.G.
-0000dc20: 5104 4200 2004 3404 3b04 4f00 2004 3e04  Q.B. .4.;.O. .>.
-0000dc30: 3f04 3504 4004 3004 4604 3804 3800 2004  ?.5.@.0.F.8.8. .
-0000dc40: 3f04 4004 3804 4504 3e04 3404 3000 2f04  ?.@.8.E.>.4.0./.
-0000dc50: 4004 3004 4104 4504 3e04 3404 3000 3a00  @.0.A.E.>.4.0.:.
-0000dc60: 2008 0000 0000 0600 0000 2755 6e6d 6174   .........'Unmat
-0000dc70: 6368 6564 2061 6363 6f75 6e74 2066 6f72  ched account for
-0000dc80: 2069 6e63 6f6d 652f 7370 656e 6469 6e67   income/spending
-0000dc90: 3a20 0700 0000 0953 7461 7465 6d65 6e74  : .....Statement
-0000dca0: 0103 0000 0052 041d 0435 0432 043e 0437  .....R...5.2.>.7
-0000dcb0: 043c 043e 0436 043d 043e 0020 0441 043e  .<.>.6.=.>. .A.>
-0000dcc0: 043f 043e 0441 0442 0430 0432 0438 0442  .?.>.A.B.0.2.8.B
-0000dcd0: 044c 0020 0441 0447 0451 0442 0020 0434  .L. .A.G.Q.B. .4
-0000dce0: 043b 044f 0020 0432 044b 043f 043b 0430  .;.O. .2.K.?.;.0
-0000dcf0: 0442 044b 003a 0020 0800 0000 0006 0000  .B.K.:. ........
-0000dd00: 001f 556e 6d61 7463 6865 6420 6163 636f  ..Unmatched acco
-0000dd10: 756e 7420 666f 7220 7061 796d 656e 743a  unt for payment:
-0000dd20: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
-0000dd30: 0300 0000 5004 1d04 3504 3204 3e04 3704  ....P...5.2.>.7.
-0000dd40: 3c04 3e04 3604 3d04 3e00 2004 4104 3e04  <.>.6.=.>. .A.>.
-0000dd50: 3f04 3e04 4104 4204 3004 3204 3804 4204  ?.>.A.B.0.2.8.B.
-0000dd60: 4c00 2004 4104 4704 5104 4200 2004 3404  L. .A.G.Q.B. .4.
-0000dd70: 3b04 4f00 2004 4104 3404 3504 3b04 3a04  ;.O. .A.4.5.;.:.
-0000dd80: 3800 3a00 2008 0000 0000 0600 0000 1d55  8.:. ..........U
-0000dd90: 6e6d 6174 6368 6564 2061 6363 6f75 6e74  nmatched account
-0000dda0: 2066 6f72 2074 7261 6465 3a20 0700 0000   for trade: ....
-0000ddb0: 0953 7461 7465 6d65 6e74 0103 0000 0054  .Statement.....T
-0000ddc0: 041d 0435 0432 0437 043e 043c 043e 0436  ...5.2.7.>.<.>.6
-0000ddd0: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
-0000dde0: 0442 0430 0432 0438 0442 044c 0020 0441  .B.0.2.8.B.L. .A
-0000ddf0: 0447 0451 0442 0020 0434 043b 044f 0020  .G.Q.B. .4.;.O. 
-0000de00: 043f 0435 0440 0435 0432 043e 0434 0430  .?.5.@.5.2.>.4.0
-0000de10: 003a 0020 0800 0000 0006 0000 0020 556e  .:. ......... Un
-0000de20: 6d61 7463 6865 6420 6163 636f 756e 7420  matched account 
-0000de30: 666f 7220 7472 616e 7366 6572 3a20 0700  for transfer: ..
-0000de40: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
-0000de50: 006e 041d 0435 0432 043e 0437 043c 043e  .n...5.2.>.7.<.>
-0000de60: 0436 043d 043e 0020 0441 043e 043f 043e  .6.=.>. .A.>.?.>
-0000de70: 0441 0442 0430 0432 0438 0442 044c 0020  .A.B.0.2.8.B.L. 
-0000de80: 0426 0411 0020 0434 043b 044f 0020 043a  .&... .4.;.O. .:
-0000de90: 043e 0440 043f 043e 0440 0430 0442 0438  .>.@.?.>.@.0.B.8
-0000dea0: 0432 043d 043e 0433 043e 0020 0434 0435  .2.=.>.3.>. .4.5
-0000deb0: 0439 0441 0442 0432 0438 044f 003a 0020  .9.A.B.2.8.O.:. 
-0000dec0: 0800 0000 0006 0000 0026 556e 6d61 7463  .........&Unmatc
-0000ded0: 6865 6420 6173 7365 7420 666f 7220 636f  hed asset for co
-0000dee0: 7270 6f72 6174 6520 6163 7469 6f6e 3a20  rporate action: 
-0000def0: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
-0000df00: 0000 004e 041d 0435 0432 043e 0437 043c  ...N...5.2.>.7.<
-0000df10: 043e 0436 043d 043e 0020 0441 043e 043f  .>.6.=.>. .A.>.?
-0000df20: 043e 0441 0442 0430 0432 0438 0442 044c  .>.A.B.0.2.8.B.L
-0000df30: 0020 0426 0411 0020 0434 043b 044f 0020  . .&... .4.;.O. 
-0000df40: 0432 044b 043f 043b 0430 0442 044b 003a  .2.K.?.;.0.B.K.:
-0000df50: 0020 0800 0000 0006 0000 001d 556e 6d61  . ..........Unma
-0000df60: 7463 6865 6420 6173 7365 7420 666f 7220  tched asset for 
-0000df70: 7061 796d 656e 743a 2007 0000 0009 5374  payment: .....St
-0000df80: 6174 656d 656e 7401 0300 0000 4c04 1d04  atement.....L...
-0000df90: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
-0000dfa0: 3e00 2004 4104 3e04 3f04 3e04 4104 4204  >. .A.>.?.>.A.B.
-0000dfb0: 3004 3204 3804 4204 4c00 2004 2604 1100  0.2.8.B.L. .&...
-0000dfc0: 2004 3404 3b04 4f00 2004 4104 3404 3504   .4.;.O. .A.4.5.
-0000dfd0: 3b04 3a04 3800 3a00 2008 0000 0000 0600  ;.:.8.:. .......
-0000dfe0: 0000 1b55 6e6d 6174 6368 6564 2061 7373  ...Unmatched ass
-0000dff0: 6574 2066 6f72 2074 7261 6465 3a20 0700  et for trade: ..
-0000e000: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
-0000e010: 005e 041d 0435 0432 043e 0437 043c 043e  .^...5.2.>.7.<.>
-0000e020: 0436 043d 043e 0020 0441 043e 043f 043e  .6.=.>. .A.>.?.>
-0000e030: 0441 0442 0430 0432 0438 0442 044c 0020  .A.B.0.2.8.B.L. 
-0000e040: 0426 0411 002f 0432 0430 043b 044e 0442  .&.../.2.0.;.N.B
-0000e050: 0443 0020 0434 043b 044f 0020 043f 0435  .C. .4.;.O. .?.5
-0000e060: 0440 0435 0432 043e 0434 0430 003a 0020  .@.5.2.>.4.0.:. 
-0000e070: 0800 0000 0006 0000 001e 556e 6d61 7463  ..........Unmatc
-0000e080: 6865 6420 6173 7365 7420 666f 7220 7472  hed asset for tr
-0000e090: 616e 7366 6572 3a20 0700 0000 0953 7461  ansfer: .....Sta
-0000e0a0: 7465 6d65 6e74 0103 0000 006c 041d 0435  tement.....l...5
-0000e0b0: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
-0000e0c0: 0020 0441 043e 043f 043e 0441 0442 0430  . .A.>.?.>.A.B.0
-0000e0d0: 0432 0438 0442 044c 0020 043a 0430 0442  .2.8.B.L. .:.0.B
-0000e0e0: 0435 0433 043e 0440 0438 044e 0020 0434  .5.3.>.@.8.N. .4
-0000e0f0: 043b 044f 0020 043f 0440 0438 0445 043e  .;.O. .?.@.8.E.>
-0000e100: 0434 0430 002f 0440 0430 0441 0445 043e  .4.0./.@.0.A.E.>
-0000e110: 0434 0430 003a 0020 0800 0000 0006 0000  .4.0.:. ........
-0000e120: 0028 556e 6d61 7463 6865 6420 6361 7465  .(Unmatched cate
-0000e130: 676f 7279 2066 6f72 2069 6e63 6f6d 652f  gory for income/
-0000e140: 7370 656e 6469 6e67 3a20 0700 0000 0953  spending: .....S
-0000e150: 7461 7465 6d65 6e74 0103 0000 0050 041d  tatement.....P..
-0000e160: 0435 0432 043e 0437 043c 043e 043d 043e  .5.2.>.7.<.>.=.>
-0000e170: 0020 0441 043e 043f 043e 0441 0442 0430  . .A.>.?.>.A.B.0
-0000e180: 0432 0438 0442 044c 0020 0432 0430 043b  .2.8.B.L. .2.0.;
-0000e190: 044e 0442 0443 0020 0434 043b 044f 0020  .N.B.C. .4.;.O. 
-0000e1a0: 0441 0447 0451 0442 0430 003a 0020 0800  .A.G.Q.B.0.:. ..
-0000e1b0: 0000 0006 0000 0020 556e 6d61 7463 6865  ....... Unmatche
-0000e1c0: 6420 6375 7272 656e 6379 2066 6f72 2061  d currency for a
-0000e1d0: 6363 6f75 6e74 3a20 0700 0000 0953 7461  ccount: .....Sta
-0000e1e0: 7465 6d65 6e74 0103 0000 0082 041d 0435  tement.........5
-0000e1f0: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
-0000e200: 0020 0441 043e 043f 043e 0441 0442 0430  . .A.>.?.>.A.B.0
-0000e210: 0432 0438 0442 044c 0020 043a 043e 043d  .2.8.B.L. .:.>.=
-0000e220: 0442 0440 0430 0433 0435 043d 0442 0430  .B.@.0.3.5.=.B.0
-0000e230: 0020 0434 043b 044f 0020 043e 043f 0435  . .4.;.O. .>.?.5
-0000e240: 0440 0430 0446 0438 0438 0020 043f 0440  .@.0.F.8.8. .?.@
-0000e250: 0438 0445 043e 0434 0430 002f 0440 0430  .8.E.>.4.0./.@.0
-0000e260: 0441 0445 043e 0434 0430 003a 0020 0800  .A.E.>.4.0.:. ..
-0000e270: 0000 0006 0000 0024 556e 6d61 7463 6865  .......$Unmatche
-0000e280: 6420 7065 6572 2066 6f72 2069 6e63 6f6d  d peer for incom
-0000e290: 652f 7370 656e 6469 6e67 3a20 0700 0000  e/spending: ....
-0000e2a0: 0953 7461 7465 6d65 6e74 0103 0000 0052  .Statement.....R
-0000e2b0: 041d 0435 043f 043e 0434 0434 0435 0440  ...5.?.>.4.4.5.@
-0000e2c0: 0436 0438 0432 0430 0435 043c 043e 0435  .6.8.2.0.5.<.>.5
-0000e2d0: 0020 043a 043e 0440 043f 043e 0440 0430  . .:.>.@.?.>.@.0
-0000e2e0: 0442 0438 0432 043d 043e 0435 0020 0434  .B.8.2.=.>.5. .4
-0000e2f0: 0435 0439 0441 0442 0432 0438 0435 003a  .5.9.A.B.2.8.5.:
-0000e300: 0020 0800 0000 0006 0000 001e 556e 7375  . ..........Unsu
-0000e310: 7070 6f72 7465 6420 636f 7270 6f72 6174  pported corporat
-0000e320: 6520 6163 7469 6f6e 3a20 0700 0000 0953  e action: .....S
-0000e330: 7461 7465 6d65 6e74 0103 0000 003c 041d  tatement.....<..
-0000e340: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
-0000e350: 0438 0432 0430 0435 043c 044b 0439 0020  .8.2.0.5.<.K.9. 
-0000e360: 0442 0438 043f 0020 0432 044b 043f 043b  .B.8.?. .2.K.?.;
-0000e370: 0430 0442 044b 003a 0020 0800 0000 0006  .0.B.K.:. ......
-0000e380: 0000 001a 556e 7375 7070 6f72 7465 6420  ....Unsupported 
-0000e390: 7061 796d 656e 7420 7479 7065 3a20 0700  payment type: ..
-0000e3a0: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
-0000e3b0: 0012 0421 043f 0438 0441 0430 043d 0438  ...!.?.8.A.0.=.8
-0000e3c0: 0435 0020 0800 0000 0006 0000 000e 5769  .5. ..........Wi
-0000e3d0: 7468 6472 6177 616c 206f 6620 0700 0000  thdrawal of ....
-0000e3e0: 0953 7461 7465 6d65 6e74 0103 0000 0044  .Statement.....D
-0000e3f0: 002a 002a 002a 0020 041d 0415 041e 0411  .*.*.*. ........
-0000e400: 0425 041e 0414 0418 041c 0410 0020 0420  .%........... . 
-0000e410: 0423 0427 041d 0410 042f 0020 041f 0420  .#.'...../. ... 
-0000e420: 041e 0412 0415 0420 041a 0410 0020 002a  ....... ..... .*
-0000e430: 002a 002a 0800 0000 0006 0000 001d 2a2a  .*.*..........**
-0000e440: 2a20 4d41 4e55 414c 2045 4e54 5259 2052  * MANUAL ENTRY R
-0000e450: 4551 5549 5245 4420 2a2a 2a07 0000 000d  EQUIRED ***.....
-0000e460: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
-0000e470: 0000 3404 2204 3804 3f00 2004 2604 1100  ..4.".8.?. .&...
-0000e480: 2004 3d04 3500 2004 3f04 3e04 3404 3404   .=.5. .?.>.4.4.
-0000e490: 3504 4004 3604 3804 3204 3004 3504 4204  5.@.6.8.2.0.5.B.
-0000e4a0: 4104 4f00 3a00 2008 0000 0000 0600 0000  A.O.:. .........
-0000e4b0: 1c41 7373 6574 2074 7970 6520 6973 6e27  .Asset type isn'
-0000e4c0: 7420 7375 7070 6f72 7465 643a 2007 0000  t supported: ...
-0000e4d0: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
-0000e4e0: 0300 0000 4804 1d04 3504 3204 3e04 3704  ....H...5.2.>.7.
-0000e4f0: 3c04 3e04 3604 3d04 3e00 2004 3d04 3004  <.>.6.=.>. .=.0.
-0000e500: 3904 4204 3800 2004 3f04 3b04 3004 4204  9.B.8. .?.;.0.B.
-0000e510: 5104 3600 2004 3404 3b04 4f00 2004 3e04  Q.6. .4.;.O. .>.
-0000e520: 4204 3c04 3504 3d04 4b00 3a00 2008 0000  B.<.5.=.K.:. ...
-0000e530: 0000 0600 0000 1f43 616e 2774 2066 696e  .......Can't fin
-0000e540: 6420 6d61 7463 6820 666f 7220 7265 7665  d match for reve
-0000e550: 7273 616c 3a20 0700 0000 0d53 7461 7465  rsal: .....State
-0000e560: 6d65 6e74 4942 4b52 0103 0000 0046 041d  mentIBKR.....F..
-0000e570: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-0000e580: 043e 0020 043d 0430 0439 0442 0438 0020  .>. .=.0.9.B.8. 
-0000e590: 043f 0430 0440 043d 0443 044e 0020 0437  .?.0.@.=.C.N. .7
-0000e5a0: 0430 043f 0438 0441 044c 0020 0434 043b  .0.?.8.A.L. .4.;
-0000e5b0: 044f 0020 0800 0000 0006 0000 001d 4361  .O. ..........Ca
-0000e5c0: 6e27 7420 6669 6e64 2070 6169 7265 6420  n't find paired 
-0000e5d0: 7265 636f 7264 2066 6f72 2007 0000 000d  record for .....
-0000e5e0: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
-0000e5f0: 0000 4e04 1d04 3504 3204 3e04 3c04 3e04  ..N...5.2.>.<.>.
-0000e600: 3604 3d04 3e00 2004 3e04 3f04 4004 3504  6.=.>. .>.?.@.5.
-0000e610: 3404 3504 3b04 3804 4204 4c00 2004 3204  4.5.;.8.B.L. .2.
-0000e620: 3004 3b04 4e04 4204 4300 2004 3404 3b04  0.;.N.B.C. .4.;.
-0000e630: 4f00 2004 4104 4704 5104 4204 3000 3a00  O. .A.G.Q.B.0.:.
-0000e640: 2008 0000 0000 0600 0000 2843 616e 2774   .........(Can't
-0000e650: 2067 6574 2061 6363 6f75 6e74 2063 7572   get account cur
-0000e660: 7265 6e63 7920 666f 7220 6163 636f 756e  rency for accoun
-0000e670: 743a 2007 0000 000d 5374 6174 656d 656e  t: .....Statemen
-0000e680: 7449 424b 5201 0300 0000 7004 1d04 3504  tIBKR.....p...5.
-0000e690: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
-0000e6a0: 2004 3e04 3f04 4004 3504 3404 3504 3b04   .>.?.@.5.4.5.;.
-0000e6b0: 3804 4204 4c00 2004 3204 3004 3b04 4e04  8.B.L. .2.0.;.N.
-0000e6c0: 4204 4b00 2004 3404 3b04 4f00 2004 3e04  B.K. .4.;.O. .>.
-0000e6d0: 3f04 3504 4004 3004 4604 3804 3800 2004  ?.5.@.0.F.8.8. .
-0000e6e0: 3e04 3104 3c04 3504 3d04 3000 2004 3204  >.1.<.5.=.0. .2.
-0000e6f0: 3004 3b04 4e04 4200 3a00 2008 0000 0000  0.;.N.B.:. .....
-0000e700: 0600 0000 2c43 616e 2774 2067 6574 2063  ....,Can't get c
-0000e710: 7572 7265 6e63 6965 7320 666f 7220 6375  urrencies for cu
-0000e720: 7272 656e 6379 2065 7863 6861 6e67 653a  rrency exchange:
-0000e730: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
-0000e740: 424b 5201 0300 0000 6804 1d04 3504 3204  BKR.....h...5.2.
-0000e750: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
-0000e760: 4004 3004 4104 3f04 3e04 3704 3d04 3004  @.0.A.?.>.7.=.0.
-0000e770: 4204 4c00 2004 3e04 3f04 3804 4104 3004  B.L. .>.?.8.A.0.
-0000e780: 3d04 3804 3500 2004 1e04 3104 4a04 3504  =.8.5. ...1.J.5.
-0000e790: 3404 3804 3d04 3504 3d04 3804 4f00 2004  4.8.=.5.=.8.O. .
-0000e7a0: 3a04 3e04 3c04 3f04 3004 3d04 3804 3900  :.>.<.?.0.=.8.9.
-0000e7b0: 2008 0000 0000 0600 0000 1f43 616e 2774   ..........Can't
-0000e7c0: 2070 6172 7365 204d 6572 6765 7220 6465   parse Merger de
-0000e7d0: 7363 7269 7074 696f 6e20 0700 0000 0d53  scription .....S
-0000e7e0: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
-0000e7f0: 0064 041d 0435 0432 043e 0437 043c 043e  .d...5.2.>.7.<.>
-0000e800: 0436 043d 043e 0020 0440 0430 0441 043f  .6.=.>. .@.0.A.?
-0000e810: 043e 0437 043d 0430 0442 044c 0020 043e  .>.7.=.0.B.L. .>
-0000e820: 043f 0438 0441 0430 043d 0438 0435 0020  .?.8.A.0.=.8.5. 
-0000e830: 0412 044b 0434 0435 043b 0435 043d 0438  ...K.4.5.;.5.=.8
-0000e840: 044f 0020 043a 043e 043c 043f 0430 043d  .O. .:.>.<.?.0.=
-0000e850: 0438 0438 0020 0800 0000 0006 0000 0021  .8.8. .........!
-0000e860: 4361 6e27 7420 7061 7273 6520 5370 696e  Can't parse Spin
-0000e870: 2d6f 6666 2064 6573 6372 6970 7469 6f6e  -off description
-0000e880: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
-0000e890: 424b 5201 0300 0000 4c04 1d04 3504 3204  BKR.....L...5.2.
-0000e8a0: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
-0000e8b0: 4004 3004 4104 3f04 3e04 3704 3d04 3004  @.0.A.?.>.7.=.0.
-0000e8c0: 4204 4c00 2004 3e04 3f04 3804 4104 3004  B.L. .>.?.8.A.0.
-0000e8d0: 3d04 3804 3500 2004 2104 3f04 3b04 3804  =.8.5. .!.?.;.8.
-0000e8e0: 4204 3000 2008 0000 0000 0600 0000 1e43  B.0. ..........C
-0000e8f0: 616e 2774 2070 6172 7365 2053 706c 6974  an't parse Split
-0000e900: 2064 6573 6372 6970 7469 6f6e 2007 0000   description ...
-0000e910: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
-0000e920: 0300 0000 6204 1d04 3504 3204 3e04 3704  ....b...5.2.>.7.
-0000e930: 3c04 3e04 3604 3d04 3e00 2004 4004 3004  <.>.6.=.>. .@.0.
-0000e940: 4104 3f04 3e04 3704 3d04 3004 4204 4c00  A.?.>.7.=.0.B.L.
-0000e950: 2004 3e04 3f04 3804 4104 3004 3d04 3804   .>.?.8.A.0.=.8.
-0000e960: 3500 2004 1404 3804 3204 3804 3404 3504  5. ...8.2.8.4.5.
-0000e970: 3d04 3404 3000 2004 3004 3a04 4604 3804  =.4.0. .0.:.F.8.
-0000e980: 4f04 3c04 3800 2008 0000 0000 0600 0000  O.<.8. .........
-0000e990: 2743 616e 2774 2070 6172 7365 2053 746f  'Can't parse Sto
-0000e9a0: 636b 2044 6976 6964 656e 6420 6465 7363  ck Dividend desc
-0000e9b0: 7269 7074 696f 6e20 0700 0000 0d53 7461  ription .....Sta
-0000e9c0: 7465 6d65 6e74 4942 4b52 0103 0000 005a  tementIBKR.....Z
-0000e9d0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-0000e9e0: 043d 043e 0020 0440 0430 0441 043f 043e  .=.>. .@.0.A.?.>
-0000e9f0: 0437 043d 0430 0442 044c 0020 043e 043f  .7.=.0.B.L. .>.?
-0000ea00: 0438 0441 0430 043d 0438 0435 0020 0421  .8.A.0.=.8.5. .!
-0000ea10: 043c 0435 043d 044b 0020 0441 0438 043c  .<.5.=.K. .A.8.<
-0000ea20: 0432 043e 043b 0430 0020 0800 0000 0006  .2.>.;.0. ......
-0000ea30: 0000 0026 4361 6e27 7420 7061 7273 6520  ...&Can't parse 
-0000ea40: 5379 6d62 6f6c 2043 6861 6e67 6520 6465  Symbol Change de
-0000ea50: 7363 7269 7074 696f 6e20 0700 0000 0d53  scription .....S
-0000ea60: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
-0000ea70: 006e 041d 0435 0432 043e 0437 043c 043e  .n...5.2.>.7.<.>
-0000ea80: 0436 043d 043e 0020 043e 0431 0440 0430  .6.=.>. .>.1.@.0
-0000ea90: 0431 043e 0442 0430 0442 044c 0020 043e  .1.>.B.0.B.L. .>
-0000eaa0: 0442 043c 0435 043d 0451 043d 043d 043e  .B.<.5.=.Q.=.=.>
-0000eab0: 0435 0020 043a 043e 0440 043f 043e 0440  .5. .:.>.@.?.>.@
-0000eac0: 0430 0442 0438 0432 043d 043e 0435 0020  .0.B.8.2.=.>.5. 
-0000ead0: 0434 0435 0439 0441 0442 0432 0438 0435  .4.5.9.A.B.2.8.5
-0000eae0: 0800 0000 0006 0000 0028 4361 6e27 7420  .........(Can't 
-0000eaf0: 7072 6f63 6573 7320 6361 6e63 656c 6c65  process cancelle
-0000eb00: 6420 636f 7270 6f72 6174 6520 6163 7469  d corporate acti
-0000eb10: 6f6e 0700 0000 0d53 7461 7465 6d65 6e74  on.....Statement
-0000eb20: 4942 4b52 0103 0000 003e 0414 0435 043d  IBKR.....>...5.=
-0000eb30: 0435 0436 043d 044b 0435 0020 0442 0440  .5.6.=.K.5. .B.@
-0000eb40: 0430 043d 0437 0430 043a 0446 0438 0438  .0.=.7.0.:.F.8.8
-0000eb50: 0020 0437 0430 0433 0440 0443 0436 0435  . .7.0.3.@.C.6.5
-0000eb60: 043d 044b 003a 0020 0800 0000 0006 0000  .=.K.:. ........
-0000eb70: 001a 4361 7368 2074 7261 6e73 6163 7469  ..Cash transacti
-0000eb80: 6f6e 7320 6c6f 6164 6564 3a20 0700 0000  ons loaded: ....
-0000eb90: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
-0000eba0: 0000 006a 041a 043e 0440 043f 043e 0440  ...j...>.@.?.>.@
-0000ebb0: 0430 0442 0438 0432 043d 043e 0435 0020  .0.B.8.2.=.>.5. 
-0000ebc0: 0441 043e 0431 044b 0442 0438 0435 0020  .A.>.1.K.B.8.5. 
-0000ebd0: 043d 0435 0020 043f 043e 0434 0434 0435  .=.5. .?.>.4.4.5
-0000ebe0: 0440 0436 0438 0432 0430 0435 0442 0441  .@.6.8.2.0.5.B.A
-0000ebf0: 044f 0020 0434 043b 044f 0020 0442 0438  .O. .4.;.O. .B.8
-0000ec00: 043f 0430 0020 0426 0411 003a 0020 0800  .?.0. .&...:. ..
-0000ec10: 0000 0006 0000 0031 436f 7270 6f72 6174  .......1Corporat
-0000ec20: 6520 6163 7469 6f6e 2069 736e 2774 2073  e action isn't s
-0000ec30: 7570 706f 7274 6564 2066 6f72 2061 7373  upported for ass
-0000ec40: 6574 2074 7970 653a 2007 0000 000d 5374  et type: .....St
-0000ec50: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
-0000ec60: 5e04 2204 3804 3f00 2004 3a04 3e04 4004  ^.".8.?. .:.>.@.
-0000ec70: 3f04 3e04 4004 3004 4204 3804 3204 3d04  ?.>.@.0.B.8.2.=.
-0000ec80: 3e04 3304 3e00 2004 3404 3504 3904 4104  >.3.>. .4.5.9.A.
-0000ec90: 4204 3204 3804 4f00 2004 3d04 3500 2004  B.2.8.O. .=.5. .
-0000eca0: 3f04 3e04 3404 3404 3504 4004 3604 3804  ?.>.4.4.5.@.6.8.
-0000ecb0: 3204 3004 3504 4204 4104 4f00 3a00 2008  2.0.5.B.A.O.:. .
-0000ecc0: 0000 0000 0600 0000 2843 6f72 706f 7261  ........(Corpora
-0000ecd0: 7465 2061 6374 696f 6e20 7479 7065 2069  te action type i
-0000ece0: 7320 6e6f 7420 7375 7070 6f72 7465 643a  s not supported:
-0000ecf0: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
-0000ed00: 424b 5201 0300 0000 4404 1a04 3e04 4004  BKR.....D...>.@.
-0000ed10: 3f04 3e04 4004 3004 4204 3804 3204 3d04  ?.>.@.0.B.8.2.=.
-0000ed20: 4b04 3500 2004 3404 3504 3904 4104 4204  K.5. .4.5.9.A.B.
-0000ed30: 3204 3804 4f00 2004 3704 3004 3304 4004  2.8.O. .7.0.3.@.
-0000ed40: 4304 3604 3504 3d04 4b00 3a00 2008 0000  C.6.5.=.K.:. ...
-0000ed50: 0000 0600 0000 1a43 6f72 706f 7261 7465  .......Corporate
-0000ed60: 2061 6374 696f 6e73 206c 6f61 6465 643a   actions loaded:
-0000ed70: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
-0000ed80: 424b 5201 0300 0000 5604 1404 3804 3204  BKR.....V...8.2.
-0000ed90: 3804 3404 3504 3d04 3400 2004 3d04 3500  8.4.5.=.4. .=.5.
-0000eda0: 2004 3d04 3004 3904 3404 3504 3d00 2004   .=.0.9.4.5.=. .
-0000edb0: 3404 3b04 4f00 2004 4304 3404 3504 4004  4.;.O. .C.4.5.@.
-0000edc0: 3604 3004 3d04 3d04 3e04 3304 3e00 2004  6.0.=.=.>.3.>. .
-0000edd0: 3d04 3004 3b04 3e04 3304 3000 3a00 2008  =.0.;.>.3.0.:. .
-0000ede0: 0000 0000 0600 0000 2844 6976 6964 656e  ........(Dividen
-0000edf0: 6420 6e6f 7420 666f 756e 6420 666f 7220  d not found for 
-0000ee00: 7769 7468 686f 6c64 696e 6720 7461 783a  withholding tax:
-0000ee10: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
-0000ee20: 424b 5201 0300 0000 2e00 4900 4200 4b00  BKR.......I.B.K.
-0000ee30: 5200 2000 6600 6c00 6500 7800 2d04 3e04  R. .f.l.e.x.-.>.
-0000ee40: 4204 4704 5104 4200 2000 2800 2a00 2e00  B.G.Q.B. .(.*...
-0000ee50: 7800 6d00 6c00 2908 0000 0000 0600 0000  x.m.l.).........
-0000ee60: 1749 424b 5220 666c 6578 2d71 7565 7279  .IBKR flex-query
-0000ee70: 2028 2a2e 786d 6c29 0700 0000 0d53 7461   (*.xml).....Sta
-0000ee80: 7465 6d65 6e74 4942 4b52 0103 0000 0026  tementIBKR.....&
-0000ee90: 0049 006e 0074 0065 0072 0061 0063 0074  .I.n.t.e.r.a.c.t
-0000eea0: 0069 0076 0065 0020 0042 0072 006f 006b  .i.v.e. .B.r.o.k
-0000eeb0: 0065 0072 0073 0800 0000 0006 0000 0013  .e.r.s..........
-0000eec0: 496e 7465 7261 6374 6976 6520 4272 6f6b  Interactive Brok
-0000eed0: 6572 7307 0000 000d 5374 6174 656d 656e  ers.....Statemen
-0000eee0: 7449 424b 5201 0300 0000 5604 2204 3804  tIBKR.....V.".8.
-0000eef0: 3f00 2004 3e04 4204 4704 5104 4204 3000  ?. .>.B.G.Q.B.0.
-0000ef00: 2000 4900 6e00 7400 6500 7200 6100 6300   .I.n.t.e.r.a.c.
-0000ef10: 7400 6900 7600 6500 2000 4200 7200 6f00  t.i.v.e. .B.r.o.
-0000ef20: 6b00 6500 7200 7300 2004 3d04 3500 2004  k.e.r.s. .=.5. .
-0000ef30: 3e04 3f04 4004 3504 3404 3504 3b04 5104  >.?.@.5.4.5.;.Q.
-0000ef40: 3d08 0000 0000 0600 0000 2949 6e74 6572  =.........)Inter
-0000ef50: 6163 7469 7665 2042 726f 6b65 7273 2072  active Brokers r
-0000ef60: 6570 6f72 7420 7479 7065 206e 6f74 2066  eport type not f
-0000ef70: 6f75 6e64 0700 0000 0d53 7461 7465 6d65  ound.....Stateme
-0000ef80: 6e74 4942 4b52 0103 0000 003a 0417 0430  ntIBKR.....:...0
-0000ef90: 0433 0440 0443 0437 043a 0430 0020 043e  .3.@.C.7.:.0. .>
-0000efa0: 0442 0447 0451 0442 0430 0020 0049 0042  .B.G.Q.B.0. .I.B
-0000efb0: 0020 0434 043b 044f 0020 0441 0447 0451  . .4.;.O. .A.G.Q
-0000efc0: 0442 0430 0020 0800 0000 0006 0000 0023  .B.0. .........#
-0000efd0: 4c6f 6164 2049 4220 466c 6578 2d73 7461  Load IB Flex-sta
-0000efe0: 7465 6d65 6e74 2066 6f72 2061 6363 6f75  tement for accou
-0000eff0: 6e74 2007 0000 000d 5374 6174 656d 656e  nt .....Statemen
-0000f000: 7449 424b 5201 0300 0000 5804 1d04 3504  tIBKR.....X...5.
-0000f010: 3404 3e04 4104 4204 3004 4204 3e04 4704  4.>.A.B.0.B.>.G.
-0000f020: 3d04 3e00 2004 3404 3004 3d04 3d04 4b04  =.>. .4.0.=.=.K.
-0000f030: 4500 2004 3e04 3100 2004 1e04 3104 4a04  E. .>.1. ...1.J.
-0000f040: 3504 3404 3804 3d04 3504 3d04 3804 3800  5.4.8.=.5.=.8.8.
-0000f050: 2004 3a04 3e04 3c04 3f04 3004 3d04 3804   .:.>.<.?.0.=.8.
-0000f060: 3900 2008 0000 0000 0600 0000 224d 6572  9. ........."Mer
-0000f070: 6765 7220 6465 7363 7269 7074 696f 6e20  ger description 
-0000f080: 6d69 7373 2073 6f6d 6520 6461 7461 2007  miss some data .
-0000f090: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000f0a0: 5201 0300 0000 5e04 1d04 3504 3e04 3404  R.....^...5.>.4.
-0000f0b0: 3d04 3e04 3704 3d04 3004 4704 3d04 3e04  =.>.7.=.0.G.=.>.
-0000f0c0: 3500 2004 4104 3e04 3204 3f04 3004 3404  5. .A.>.2.?.0.4.
-0000f0d0: 3504 3d04 3804 3500 2004 4104 3e04 3104  5.=.8.5. .A.>.1.
-0000f0e0: 4b04 4204 3804 3900 2004 4004 3504 3e04  K.B.8.9. .@.5.>.
-0000f0f0: 4004 3304 3004 3d04 3804 3704 3004 4604  @.3.0.=.8.7.0.F.
-0000f100: 3804 3800 2008 0000 0000 0600 0000 294d  8.8. .........)M
-0000f110: 756c 7469 706c 6520 6d65 7267 6572 2072  ultiple merger r
-0000f120: 6563 6f72 6473 2061 6c72 6561 6479 2065  ecords already e
-0000f130: 7869 7374 2061 7420 0700 0000 0d53 7461  xist at .....Sta
-0000f140: 7465 6d65 6e74 4942 4b52 0103 0000 0052  tementIBKR.....R
-0000f150: 0414 0435 0439 0441 0442 0432 0438 0435  ...5.9.A.B.2.8.5
-0000f160: 0020 043d 0435 0020 043f 043e 0434 0434  . .=.5. .?.>.4.4
-0000f170: 0435 0440 0436 0438 0432 0430 0435 0442  .5.@.6.8.2.0.5.B
-0000f180: 0441 044f 0020 0434 043b 044f 0020 043e  .A.O. .4.;.O. .>
-0000f190: 043f 0446 0438 043e 043d 043e 0432 003a  .?.F.8.>.=.>.2.:
-0000f1a0: 0020 0800 0000 0006 0000 0027 4f70 7469  . .........'Opti
-0000f1b0: 6f6e 2045 2641 2645 2061 6374 696f 6e20  on E&A&E action 
-0000f1c0: 6973 6e27 7420 696d 706c 656d 656e 7465  isn't implemente
-0000f1d0: 643a 2007 0000 000d 5374 6174 656d 656e  d: .....Statemen
-0000f1e0: 7449 424b 5201 0300 0000 3a04 1804 4104  tIBKR.....:...A.
-0000f1f0: 3f04 3e04 3b04 3d04 3504 3d04 3804 3500  ?.>.;.=.5.=.8.5.
-0000f200: 2004 3f04 4004 3e04 3404 3004 3d04 3d04   .?.@.>.4.0.=.=.
-0000f210: 3e04 3304 3e00 2004 3e04 3f04 4604 3804  >.3.>. .>.?.F.8.
-0000f220: 3e04 3d04 3008 0000 0000 0600 0000 114f  >.=.0..........O
-0000f230: 7074 696f 6e20 6173 7369 676e 6d65 6e74  ption assignment
-0000f240: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
-0000f250: 4b52 0103 0000 003a 0418 0441 043f 043e  KR.....:...A.?.>
-0000f260: 043b 043d 0435 043d 0438 0435 002f 044d  .;.=.5.=.8.5./.M
-0000f270: 043a 0441 043f 0438 0440 0430 0446 0438  .:.A.?.8.@.0.F.8
-0000f280: 044f 0020 043e 043f 0446 0438 043e 043d  .O. .>.?.F.8.>.=
-0000f290: 0430 0800 0000 0006 0000 001a 4f70 7469  .0..........Opti
-0000f2a0: 6f6e 2061 7373 6967 6e6d 656e 742f 6578  on assignment/ex
-0000f2b0: 6572 6369 7365 0700 0000 0d53 7461 7465  ercise.....State
-0000f2c0: 6d65 6e74 4942 4b52 0103 0000 003a 0418  mentIBKR.....:..
-0000f2d0: 0441 043f 043e 043b 043d 0435 043d 0438  .A.?.>.;.=.5.=.8
-0000f2e0: 0435 0020 043a 0443 043f 043b 0435 043d  .5. .:.C.?.;.5.=
-0000f2f0: 043d 043e 0433 043e 0020 043e 043f 0446  .=.>.3.>. .>.?.F
-0000f300: 0438 043e 043d 0430 0800 0000 0006 0000  .8.>.=.0........
-0000f310: 000f 4f70 7469 6f6e 2065 7865 7263 6973  ..Option exercis
-0000f320: 6507 0000 000d 5374 6174 656d 656e 7449  e.....StatementI
-0000f330: 424b 5201 0300 0000 2404 2d04 3a04 4104  BKR.....$.-.:.A.
-0000f340: 3f04 3804 4004 3004 4604 3804 4f00 2004  ?.8.@.0.F.8.O. .
-0000f350: 3e04 3f04 4604 3804 3e04 3d04 3008 0000  >.?.F.8.>.=.0...
-0000f360: 0000 0600 0000 114f 7074 696f 6e20 6578  .......Option ex
-0000f370: 7069 7261 7469 6f6e 0700 0000 0d53 7461  piration.....Sta
-0000f380: 7465 6d65 6e74 4942 4b52 0103 0000 0040  tementIBKR.....@
-0000f390: 0414 0435 0439 0441 0442 0432 0438 044f  ...5.9.A.B.2.8.O
-0000f3a0: 0020 0441 0020 043e 043f 0446 0438 043e  . .A. .>.?.F.8.>
-0000f3b0: 043d 0430 043c 0438 0020 0437 0430 0433  .=.0.<.8. .7.0.3
-0000f3c0: 0440 0443 0436 0435 043d 044b 003a 0020  .@.C.6.5.=.K.:. 
-0000f3d0: 0800 0000 0006 0000 0016 4f70 7469 6f6e  ..........Option
-0000f3e0: 7320 4526 4126 4520 6c6f 6164 6564 3a20  s E&A&E loaded: 
-0000f3f0: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
-0000f400: 4b52 0103 0000 006a 041d 0435 0020 043d  KR.....j...5. .=
-0000f410: 0430 0439 0434 0435 043d 0430 0020 0441  .0.9.4.5.=.0. .A
-0000f420: 0434 0435 043b 043a 0430 0020 0434 043b  .4.5.;.:.0. .4.;
-0000f430: 044f 0020 0438 0441 043f 043e 043b 043d  .O. .8.A.?.>.;.=
-0000f440: 0435 043d 0438 044f 002f 044d 043a 0441  .5.=.8.O./.M.:.A
-0000f450: 043f 0438 0440 0430 0446 0438 0438 0020  .?.8.@.0.F.8.8. 
-0000f460: 043e 043f 0446 0438 043e 043d 0430 003a  .>.?.F.8.>.=.0.:
-0000f470: 0020 0800 0000 0006 0000 0035 4f72 6967  . .........5Orig
-0000f480: 696e 616c 2074 7261 6465 206e 6f74 2066  inal trade not f
-0000f490: 6f75 6e64 2066 6f72 204f 7074 696f 6e20  ound for Option 
-0000f4a0: 4526 4126 4520 6f70 6572 6174 696f 6e3a  E&A&E operation:
-0000f4b0: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
-0000f4c0: 424b 5201 0300 0000 6c04 1f04 3b04 3004  BKR.....l...;.0.
-0000f4d0: 4204 5104 3600 2004 3104 4b04 3b00 2004  B.Q.6. .1.K.;. .
-0000f4e0: 3e04 4204 3c04 3504 3d04 5104 3d00 2004  >.B.<.5.=.Q.=. .
-0000f4f0: 3f04 3e00 2004 3f04 4004 3804 3c04 3504  ?.>. .?.@.8.<.5.
-0000f500: 4004 3d04 3e04 3c04 4300 2004 4104 3e04  @.=.>.<.C. .A.>.
-0000f510: 3204 3f04 3004 3404 3504 3d04 3804 4e00  2.?.0.4.5.=.8.N.
-0000f520: 2004 3e04 3f04 3804 4104 3004 3d04 3804   .>.?.8.A.0.=.8.
-0000f530: 4f00 3a00 2008 0000 0000 0600 0000 3150  O.:. .........1P
-0000f540: 6179 6d65 6e74 2077 6173 2072 6576 6572  ayment was rever
-0000f550: 7365 6420 6279 2061 7070 726f 7869 6d61  sed by approxima
-0000f560: 7465 2064 6573 6372 6970 7469 6f6e 3a20  te description: 
-0000f570: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
-0000f580: 4b52 0103 0000 006a 041f 043b 0430 0442  KR.....j...;.0.B
-0000f590: 0451 0436 0020 0431 044b 043b 0020 043e  .Q.6. .1.K.;. .>
-0000f5a0: 0442 043c 0435 043d 0451 043d 002c 0020  .B.<.5.=.Q.=.,. 
-0000f5b0: 043d 043e 0020 0441 0020 043d 0435 0441  .=.>. .A. .=.5.A
-0000f5c0: 043e 0432 043f 0430 0434 0430 044e 0449  .>.2.?.0.4.0.N.I
-0000f5d0: 0435 0439 0020 0434 0430 0442 043e 0439  .5.9. .4.0.B.>.9
-0000f5e0: 0020 043e 0442 0447 0451 0442 0430 003a  . .>.B.G.Q.B.0.:
-0000f5f0: 0020 0800 0000 0006 0000 0033 5061 796d  . .........3Paym
-0000f600: 656e 7420 7761 7320 7265 7665 7273 6564  ent was reversed
-0000f610: 2077 6974 6820 6469 6666 6572 656e 7420   with different 
-0000f620: 7265 706f 7274 6564 2064 6174 653a 2007  reported date: .
-0000f630: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000f640: 5201 0300 0000 2804 1f04 3b04 3004 4204  R.....(...;.0.B.
-0000f650: 5104 3600 2004 3104 4b04 3b00 2004 3e04  Q.6. .1.K.;. .>.
-0000f660: 4204 3c04 3504 3d04 5104 3d00 3a00 2008  B.<.5.=.Q.=.:. .
-0000f670: 0000 0000 0600 0000 1650 6179 6d65 6e74  .........Payment
-0000f680: 2077 6173 2072 6576 6572 7365 643a 2007   was reversed: .
-0000f690: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000f6a0: 5201 0300 0000 1c04 2604 1100 2004 3704  R.......&... .7.
-0000f6b0: 3004 3304 4004 4304 3604 3504 3d04 4b00  0.3.@.C.6.5.=.K.
-0000f6c0: 3a00 2008 0000 0000 0600 0000 1353 6563  :. ..........Sec
-0000f6d0: 7572 6974 6965 7320 6c6f 6164 6564 3a20  urities loaded: 
-0000f6e0: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
-0000f6f0: 4b52 0103 0000 0056 041d 0435 0434 043e  KR.....V...5.4.>
-0000f700: 0441 0442 0430 0442 043e 0447 043d 043e  .A.B.0.B.>.G.=.>
-0000f710: 0020 0434 0430 043d 043d 044b 0445 0020  . .4.0.=.=.K.E. 
-0000f720: 0434 043b 044f 0020 0412 044b 0434 0435  .4.;.O. ...K.4.5
-0000f730: 043b 0435 043d 0438 044f 0020 043a 043e  .;.5.=.8.O. .:.>
-0000f740: 043c 043f 0430 043d 0438 0438 0020 0800  .<.?.0.=.8.8. ..
-0000f750: 0000 0006 0000 0024 5370 696e 2d6f 6666  .......$Spin-off
-0000f760: 2064 6573 6372 6970 7469 6f6e 206d 6973   description mis
-0000f770: 7320 736f 6d65 2064 6174 6120 0700 0000  s some data ....
-0000f780: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
-0000f790: 0000 005c 0418 0441 0445 043e 0434 043d  ...\...A.E.>.4.=
-0000f7a0: 0430 044f 0020 0426 0411 0020 0434 043b  .0.O. .&... .4.;
-0000f7b0: 044f 0020 0432 044b 0434 0435 043b 0435  .O. .2.K.4.5.;.5
-0000f7c0: 043d 0438 044f 0020 043a 043e 043c 043f  .=.8.O. .:.>.<.?
-0000f7d0: 0430 043d 0438 0438 0020 043d 0435 0020  .0.=.8.8. .=.5. 
-0000f7e0: 043d 0430 0439 0434 0435 043d 0430 0020  .=.0.9.4.5.=.0. 
-0000f7f0: 0800 0000 0006 0000 0021 5370 696e 2d6f  .........!Spin-o
-0000f800: 6666 2069 6e69 7469 616c 2061 7373 6574  ff initial asset
-0000f810: 206e 6f74 2066 6f75 6e64 2007 0000 000d   not found .....
-0000f820: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
-0000f830: 0000 5604 1e04 4804 3804 3104 3a04 3000  ..V...H.8.1.:.0.
-0000f840: 2004 3e04 3a04 4004 4304 3304 3b04 3504   .>.:.@.C.3.;.5.
-0000f850: 3d04 3804 4f00 2000 5300 7000 6900 6e00  =.8.O. .S.p.i.n.
-0000f860: 2d00 6f00 6600 6600 2004 4104 3b04 3804  -.o.f.f. .A.;.8.
-0000f870: 4804 3a04 3e04 3c00 2004 3104 3e04 3b04  H.:.>.<. .1.>.;.
-0000f880: 4c04 4804 3004 4f00 2008 0000 0000 0600  L.H.0.O. .......
-0000f890: 0000 2353 7069 6e2d 6f66 6620 726f 756e  ..#Spin-off roun
-0000f8a0: 6469 6e67 2065 7272 6f72 2069 7320 746f  ding error is to
-0000f8b0: 6f20 6269 6720 0700 0000 0d53 7461 7465  o big .....State
-0000f8c0: 6d65 6e74 4942 4b52 0103 0000 003e 041d  mentIBKR.....>..
-0000f8d0: 0435 0434 043e 0441 0442 0430 0442 043e  .5.4.>.A.B.0.B.>
-0000f8e0: 0447 043d 043e 0020 0434 0430 043d 043d  .G.=.>. .4.0.=.=
-0000f8f0: 044b 0445 0020 0434 043b 044f 0020 0421  .K.E. .4.;.O. .!
-0000f900: 043f 043b 0438 0442 0430 0020 0800 0000  .?.;.8.B.0. ....
-0000f910: 0006 0000 0021 5370 6c69 7420 6465 7363  .....!Split desc
-0000f920: 7269 7074 696f 6e20 6d69 7373 2073 6f6d  ription miss som
-0000f930: 6520 6461 7461 2007 0000 000d 5374 6174  e data .....Stat
-0000f940: 656d 656e 7449 424b 5201 0300 0000 3804  ementIBKR.....8.
-0000f950: 1704 3004 4704 3804 4104 3b04 3504 3d04  ..0.G.8.A.;.5.=.
-0000f960: 3804 3500 2004 3004 3a04 4604 3804 3900  8.5. .0.:.F.8.9.
-0000f970: 2004 3704 3004 3304 4004 4304 3604 3504   .7.0.3.@.C.6.5.
-0000f980: 3d04 3e00 3a00 2008 0000 0000 0600 0000  =.>.:. .........
-0000f990: 1753 746f 636b 2076 6573 7469 6e67 7320  .Stock vestings 
-0000f9a0: 6c6f 6164 6564 3a20 0700 0000 0d53 7461  loaded: .....Sta
-0000f9b0: 7465 6d65 6e74 4942 4b52 0103 0000 0048  tementIBKR.....H
-0000f9c0: 041a 043e 0440 0440 0435 043a 0442 0438  ...>.@.@.5.:.B.8
-0000f9d0: 0440 043e 0432 043a 0430 0020 043d 0430  .@.>.2.:.0. .=.0
-0000f9e0: 043b 043e 0433 0430 0020 0434 043b 044f  .;.>.3.0. .4.;.O
-0000f9f0: 0020 0434 0438 0432 0438 0434 0435 043d  . .4.8.2.8.4.5.=
-0000fa00: 0434 0430 003a 0020 0800 0000 0006 0000  .4.0.:. ........
-0000fa10: 001d 5461 7820 6164 6a75 7374 6d65 6e74  ..Tax adjustment
-0000fa20: 2066 6f72 2064 6976 6964 656e 643a 2007   for dividend: .
-0000fa30: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000fa40: 5201 0300 0000 2404 1d04 3004 3b04 3e04  R.....$...0.;.>.
-0000fa50: 3304 3800 2004 3704 3004 3304 4004 4304  3.8. .7.0.3.@.C.
-0000fa60: 3604 3504 3d04 4b00 3a00 2008 0000 0000  6.5.=.K.:. .....
-0000fa70: 0600 0000 0e54 6178 6573 206c 6f61 6465  .....Taxes loade
-0000fa80: 643a 2007 0000 000d 5374 6174 656d 656e  d: .....Statemen
-0000fa90: 7449 424b 5201 03ff ffff ff08 0000 0000  tIBKR...........
-0000faa0: 0600 0000 0f54 7261 6465 7320 6c6f 6164  .....Trades load
-0000fab0: 6564 3a20 0700 0000 0d53 7461 7465 6d65  ed: .....Stateme
-0000fac0: 6e74 4942 4b52 0103 0000 0058 041d 0435  ntIBKR.....X...5
-0000fad0: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
-0000fae0: 0432 0430 0435 043c 044b 0439 0020 0444  .2.0.5.<.K.9. .D
-0000faf0: 043e 0440 043c 0430 0442 0020 043e 043f  .>.@.<.0.B. .>.?
-0000fb00: 0438 0441 0430 043d 0438 044f 0020 0434  .8.A.0.=.8.O. .4
-0000fb10: 0438 0432 0438 0434 0435 043d 0434 0430  .8.2.8.4.5.=.4.0
-0000fb20: 003a 0020 0800 0000 0006 0000 0022 556e  .:. ........."Un
-0000fb30: 6861 6e64 6c65 6420 6469 7669 6465 6e64  handled dividend
-0000fb40: 2070 6174 7465 726e 2066 6f75 6e64 3a20   pattern found: 
-0000fb50: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
-0000fb60: 4b52 0103 0000 004e 041d 0435 043f 043e  KR.....N...5.?.>
-0000fb70: 0434 0434 0435 0440 0436 0438 0432 0430  .4.4.5.@.6.8.2.0
-0000fb80: 0435 043c 044b 0439 0020 0444 043e 0440  .5.<.K.9. .D.>.@
-0000fb90: 043c 0430 0442 0020 0441 0442 0440 0430  .<.0.B. .A.B.@.0
-0000fba0: 043d 044b 0020 043d 0430 043b 043e 0433  .=.K. .=.0.;.>.3
-0000fbb0: 0430 003a 0020 0800 0000 0006 0000 0025  .0.:. .........%
-0000fbc0: 556e 6861 6e64 6c65 6420 7461 7820 636f  Unhandled tax co
-0000fbd0: 756e 7472 7920 7061 7474 6572 6e20 666f  untry pattern fo
-0000fbe0: 756e 643a 2007 0000 000d 5374 6174 656d  und: .....Statem
-0000fbf0: 656e 7449 424b 5201 0300 0000 5204 1d04  entIBKR.....R...
-0000fc00: 3504 3f04 3e04 3404 3404 3504 4004 3604  5.?.>.4.4.5.@.6.
-0000fc10: 3804 3204 3004 3504 3c04 4b04 3900 2004  8.2.0.5.<.K.9. .
-0000fc20: 4404 3e04 4004 3c04 3004 4200 2004 3e04  D.>.@.<.0.B. .>.
-0000fc30: 3f04 3804 4104 3004 3d04 3804 4f00 2004  ?.8.A.0.=.8.O. .
-0000fc40: 3d04 3004 3b04 3e04 3304 3000 3a00 2008  =.0.;.>.3.0.:. .
-0000fc50: 0000 0000 0600 0000 1d55 6e68 616e 646c  .........Unhandl
-0000fc60: 6564 2074 6178 2070 6174 7465 726e 2066  ed tax pattern f
-0000fc70: 6f75 6e64 3a20 0700 0000 0d53 7461 7465  ound: .....State
-0000fc80: 6d65 6e74 4942 4b52 0103 0000 0058 041d  mentIBKR.....X..
-0000fc90: 0435 0438 0437 0432 0435 0441 0442 043d  .5.8.7.2.5.A.B.=
-0000fca0: 044b 0439 0020 0442 0438 043f 0020 043e  .K.9. .B.8.?. .>
-0000fcb0: 0442 0447 0451 0442 0430 0020 0049 006e  .B.G.Q.B.0. .I.n
-0000fcc0: 0074 0065 0072 0061 0063 0074 0069 0076  .t.e.r.a.c.t.i.v
-0000fcd0: 0065 0020 0042 0072 006f 006b 0065 0072  .e. .B.r.o.k.e.r
-0000fce0: 0073 003a 0020 0800 0000 0006 0000 0029  .s.:. .........)
-0000fcf0: 556e 6b6e 6f77 6e20 496e 7465 7261 6374  Unknown Interact
-0000fd00: 6976 6520 4272 6f6b 6572 7320 7265 706f  ive Brokers repo
-0000fd10: 7274 2074 7970 653a 2007 0000 000d 5374  rt type: .....St
-0000fd20: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
-0000fd30: a204 1204 4b00 2004 3f04 4b04 4204 3004  ....K. .?.K.B.0.
-0000fd40: 3504 4204 3504 4104 4c00 2004 3704 3004  5.B.5.A.L. .7.0.
-0000fd50: 3304 4004 4304 3704 3804 4204 4c00 2004  3.@.C.7.8.B.L. .
-0000fd60: 3e04 4204 4704 5104 4200 2004 3e00 2004  >.B.G.Q.B. .>. .
-0000fd70: 3f04 3e04 3404 4204 3204 3504 4004 3604  ?.>.4.B.2.5.@.6.
-0000fd80: 3404 5104 3d04 3d04 4b04 4500 2004 4104  4.Q.=.=.K.E. .A.
-0000fd90: 3404 3504 3b04 3a04 3004 4500 2004 3204  4.5.;.:.0.E. .2.
-0000fda0: 3c04 3504 4104 4204 3e00 2004 3e04 4204  <.5.A.B.>. .>.B.
-0000fdb0: 4704 5104 4204 3000 2004 3f04 3e00 2004  G.Q.B.0. .?.>. .
-0000fdc0: 1004 3a04 4204 3804 3204 3d04 3e04 4104  ..:.B.8.2.=.>.A.
-0000fdd0: 4204 3808 0000 0000 0600 0000 3f59 6f75  B.8.........?You
-0000fde0: 2074 7279 2074 6f20 696d 706f 7274 2054   try to import T
-0000fdf0: 7261 6465 2063 6f6e 6669 6d61 7469 6f6e  rade confimation
-0000fe00: 2072 6570 6f72 742c 206e 6f74 2041 6374   report, not Act
-0000fe10: 6976 6974 7920 7265 706f 7274 0700 0000  ivity report....
-0000fe20: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
-0000fe30: 0000 0052 041d 0435 0432 043e 0437 043c  ...R...5.2.>.7.<
-0000fe40: 043e 0436 043d 043e 0020 0440 0430 0441  .>.6.=.>. .@.0.A
-0000fe50: 043f 043e 0437 043d 0430 0442 044c 0020  .?.>.7.=.0.B.L. 
-0000fe60: 043e 043f 0438 0441 0430 043d 0438 0435  .>.?.8.A.0.=.8.5
-0000fe70: 0020 0434 0438 0432 0438 0434 0435 043d  . .4.8.2.8.4.5.=
-0000fe80: 0434 0430 0020 0800 0000 0006 0000 0021  .4.0. .........!
-0000fe90: 4361 6e27 7420 7061 7273 6520 4469 7669  Can't parse Divi
-0000fea0: 6465 6e64 2064 6573 6372 6970 7469 6f6e  dend description
-0000feb0: 2007 0000 000c 5374 6174 656d 656e 744a   .....StatementJ
-0000fec0: 3254 0103 0000 001c 0414 0421 0020 0437  2T.........!. .7
-0000fed0: 0430 0433 0440 0443 0436 0435 043d 044b  .0.3.@.C.6.5.=.K
-0000fee0: 003a 0020 0800 0000 0006 0000 0016 4361  .:. ..........Ca
-0000fef0: 7368 2062 616c 616e 6365 7320 6c6f 6164  sh balances load
-0000ff00: 6564 3a20 0700 0000 0c53 7461 7465 6d65  ed: .....Stateme
-0000ff10: 6e74 4a32 5401 0300 0000 3a04 1404 3504  ntJ2T.....:...5.
-0000ff20: 3d04 3504 3604 3d04 4b04 4500 2004 3e04  =.5.6.=.K.E. .>.
-0000ff30: 3f04 3504 4004 3004 4604 3804 3900 2004  ?.5.@.0.F.8.9. .
-0000ff40: 3704 3004 3304 4004 4304 3604 3504 3d04  7.0.3.@.C.6.5.=.
-0000ff50: 3e00 3a00 2008 0000 0000 0600 0000 1843  >.:. ..........C
-0000ff60: 6173 6820 6f70 6572 6174 696f 6e73 206c  ash operations l
-0000ff70: 6f61 6465 643a 2007 0000 000c 5374 6174  oaded: .....Stat
-0000ff80: 656d 656e 744a 3254 0103 0000 0048 0421  ementJ2T.....H.!
-0000ff90: 0434 0435 043b 043a 0438 0020 0441 0020  .4.5.;.:.8. .A. 
-0000ffa0: 043a 0440 0438 043f 0442 043e 002d 0432  .:.@.8.?.B.>.-.2
-0000ffb0: 0430 043b 044e 0442 0430 043c 0438 0020  .0.;.N.B.0.<.8. 
-0000ffc0: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
-0000ffd0: 044b 003a 0020 0800 0000 0006 0000 0016  .K.:. ..........
-0000ffe0: 4372 7970 746f 2074 7261 6465 7320 6c6f  Crypto trades lo
-0000fff0: 6164 6564 3a20 0700 0000 0c53 7461 7465  aded: .....State
-00010000: 6d65 6e74 4a32 5401 0300 0000 5004 1200  mentJ2T.....P...
-00010010: 2004 3e04 3f04 3804 4104 3004 3d04 3804   .>.?.8.A.0.=.8.
-00010020: 3800 2004 3404 3804 3204 3804 3404 3504  8. .4.8.2.8.4.5.
-00010030: 3d04 3404 3000 2004 3e04 4204 4104 4304  =.4.0. .>.B.A.C.
-00010040: 4204 4104 4204 3204 4304 4e04 4200 2004  B.A.B.2.C.N.B. .
-00010050: 3404 3004 3d04 3d04 4b04 3500 2008 0000  4.0.=.=.K.5. ...
-00010060: 0000 0600 0000 2444 6976 6964 656e 6420  ......$Dividend 
-00010070: 6465 7363 7269 7074 696f 6e20 6d69 7373  description miss
-00010080: 2073 6f6d 6520 6461 7461 2007 0000 000c   some data .....
-00010090: 5374 6174 656d 656e 744a 3254 0103 0000  StatementJ2T....
-000100a0: 004e 0414 0438 0432 0438 0434 0435 043d  .N...8.2.8.4.5.=
-000100b0: 0434 0020 043d 0435 0020 043d 0430 0439  .4. .=.5. .=.0.9
-000100c0: 0434 0435 043d 0020 0434 043b 044f 0020  .4.5.=. .4.;.O. 
-000100d0: 0441 043f 0438 0441 0430 043d 0438 044f  .A.?.8.A.0.=.8.O
-000100e0: 0020 043d 0430 043b 043e 0433 0430 0020  . .=.0.;.>.3.0. 
-000100f0: 0800 0000 0006 0000 001f 4469 7669 6465  ..........Divide
-00010100: 6e64 2066 6f72 2074 6178 2077 6173 206e  nd for tax was n
-00010110: 6f74 2066 6f75 6e64 2007 0000 000c 5374  ot found .....St
-00010120: 6174 656d 656e 744a 3254 0103 0000 0044  atementJ2T.....D
-00010130: 0422 0440 0430 043d 0437 0430 043a 0446  .".@.0.=.7.0.:.F
-00010140: 0438 044f 0020 043f 0440 043e 043f 0443  .8.O. .?.@.>.?.C
-00010150: 0449 0435 043d 0430 0020 043f 0440 0438  .I.5.=.0. .?.@.8
-00010160: 0020 0438 043c 043f 043e 0440 0442 0435  . .8.<.?.>.@.B.5
-00010170: 003a 0020 0800 0000 0006 0000 001f 496d  .:. ..........Im
-00010180: 706f 7274 2073 6b69 7070 6564 206f 6620  port skipped of 
-00010190: 7472 616e 7361 6374 696f 6e3a 2007 0000  transaction: ...
-000101a0: 000c 5374 6174 656d 656e 744a 3254 0103  ..StatementJ2T..
-000101b0: 0000 0014 004a 0075 0073 0074 0032 0054  .....J.u.s.t.2.T
-000101c0: 0072 0061 0064 0065 0800 0000 0006 0000  .r.a.d.e........
-000101d0: 000a 4a75 7374 3254 7261 6465 0700 0000  ..Just2Trade....
-000101e0: 0c53 7461 7465 6d65 6e74 4a32 5401 0300  .StatementJ2T...
-000101f0: 0000 3204 1e04 4204 4704 5104 4200 2000  ..2...B.G.Q.B. .
-00010200: 4a00 7500 7300 7400 3200 5400 7200 6100  J.u.s.t.2.T.r.a.
-00010210: 6400 6500 2000 2800 2a00 2e00 7800 6c00  d.e. .(.*...x.l.
-00010220: 7300 7800 2908 0000 0000 0600 0000 1d4a  s.x.)..........J
-00010230: 7573 7432 5472 6164 6520 7374 6174 656d  ust2Trade statem
-00010240: 656e 7420 282a 2e78 6c73 7829 0700 0000  ent (*.xlsx)....
-00010250: 0c53 7461 7465 6d65 6e74 4a32 5401 0300  .StatementJ2T...
-00010260: 0000 1c04 2604 1100 2004 3704 3004 3304  ....&... .7.0.3.
-00010270: 4004 4304 3604 3504 3d04 4b00 3a00 2008  @.C.6.5.=.K.:. .
-00010280: 0000 0000 0600 0000 1353 6563 7572 6974  .........Securit
-00010290: 6965 7320 6c6f 6164 6564 3a20 0700 0000  ies loaded: ....
-000102a0: 0c53 7461 7465 6d65 6e74 4a32 5401 0300  .StatementJ2T...
-000102b0: 0000 3804 2104 3404 3504 3b04 3a04 3800  ..8.!.4.5.;.:.8.
-000102c0: 2004 4100 2004 3004 3a04 4604 3804 4f04   .A. .0.:.F.8.O.
-000102d0: 3c04 3800 2004 3704 3004 3304 4004 4304  <.8. .7.0.3.@.C.
-000102e0: 3604 3504 3d04 4b00 3a00 2008 0000 0000  6.5.=.K.:. .....
-000102f0: 0600 0000 1553 746f 636b 2074 7261 6465  .....Stock trade
-00010300: 7320 6c6f 6164 6564 3a20 0700 0000 0c53  s loaded: .....S
-00010310: 7461 7465 6d65 6e74 4a32 5401 0300 0000  tatementJ2T.....
-00010320: 4004 1d04 3504 3804 3704 3204 3504 4104  @...5.8.7.2.5.A.
-00010330: 4204 3d04 3004 4f00 2004 3404 3504 3d04  B.=.0.O. .4.5.=.
-00010340: 3504 3604 3d04 3004 4f00 2004 4204 4004  5.6.=.0.O. .B.@.
-00010350: 3004 3d04 3704 3004 3a04 4604 3804 4f00  0.=.7.0.:.F.8.O.
-00010360: 2008 0000 0000 0600 0000 1e55 6e6b 6e6f   ..........Unkno
-00010370: 776e 2063 6173 6820 7472 616e 7361 6374  wn cash transact
-00010380: 696f 6e20 7479 7065 2007 0000 000c 5374  ion type .....St
-00010390: 6174 656d 656e 744a 3254 0103 0000 0030  atementJ2T.....0
-000103a0: 041d 0435 0438 0437 0432 0435 0441 0442  ...5.8.7.2.5.A.B
-000103b0: 043d 044b 0439 0020 0442 0438 043f 0020  .=.K.9. .B.8.?. 
-000103c0: 0441 0434 0435 043b 043a 0438 003a 0020  .A.4.5.;.:.8.:. 
-000103d0: 0800 0000 0006 0000 0014 556e 6b6e 6f77  ..........Unknow
-000103e0: 6e20 7472 6164 6520 7479 7065 3a20 0700  n trade type: ..
-000103f0: 0000 0c53 7461 7465 6d65 6e74 4a32 5401  ...StatementJ2T.
-00010400: 0300 0000 4a04 1d04 3504 3f04 3e04 3404  ....J...5.?.>.4.
-00010410: 3404 3504 4004 3604 3804 3204 3004 3504  4.5.@.6.8.2.0.5.
-00010420: 3c04 3004 4f00 2004 3404 3504 3d04 3504  <.0.O. .4.5.=.5.
-00010430: 3604 3d04 3004 4f00 2004 4204 4004 3004  6.=.0.O. .B.@.0.
-00010440: 3d04 3704 3004 3a04 4604 3804 4f00 2008  =.7.0.:.F.8.O. .
-00010450: 0000 0000 0600 0000 1e55 6e73 7570 7070  .........Unsuppp
-00010460: 6f72 7465 6420 6361 7368 2074 7261 6e73  orted cash trans
-00010470: 6163 7469 6f6e 2007 0000 000c 5374 6174  action .....Stat
-00010480: 656d 656e 744a 3254 0103 0000 003a 0414  ementJ2T.....:..
-00010490: 0435 043d 0435 0436 043d 044b 0445 0020  .5.=.5.6.=.K.E. 
-000104a0: 043e 043f 0435 0440 0430 0446 0438 0439  .>.?.5.@.0.F.8.9
-000104b0: 0020 0437 0430 0433 0440 0443 0436 0435  . .7.0.3.@.C.6.5
-000104c0: 043d 043e 003a 0020 0800 0000 0006 0000  .=.>.:. ........
-000104d0: 0018 4361 7368 206f 7065 7261 7469 6f6e  ..Cash operation
-000104e0: 7320 6c6f 6164 6564 3a20 0700 0000 0c53  s loaded: .....S
-000104f0: 7461 7465 6d65 6e74 4b49 5401 0300 0000  tatementKIT.....
-00010500: 7604 1d04 3004 3b04 3e04 3300 2004 3d04  v...0.;.>.3. .=.
-00010510: 3000 2004 3404 3804 3204 3804 3404 3504  0. .4.8.2.8.4.5.
-00010520: 3d04 3404 4b00 2004 3d04 3500 2004 3f04  =.4.K. .=.5. .?.
-00010530: 3e04 3404 3404 3504 4004 3604 3804 3204  >.4.4.5.@.6.8.2.
-00010540: 3004 3504 4204 4104 4f00 2004 3404 3b04  0.5.B.A.O. .4.;.
-00010550: 4f00 2004 3104 4004 3e04 3a04 3504 4004  O. .1.@.>.:.5.@.
-00010560: 3000 2004 1a04 1804 2200 2d04 4404 3804  0. .....".-.D.8.
-00010570: 3d04 3004 3d04 4108 0000 0000 0600 0000  =.0.=.A.........
-00010580: 3e44 6976 6964 656e 6420 7461 7865 7320  >Dividend taxes 
-00010590: 6172 6520 6e6f 7420 7375 7070 6f72 7465  are not supporte
-000105a0: 6420 666f 7220 4b49 5420 6272 6f6b 6572  d for KIT broker
-000105b0: 2073 7461 7465 6d65 6e74 7320 7965 7407   statements yet.
-000105c0: 0000 000c 5374 6174 656d 656e 744b 4954  ....StatementKIT
-000105d0: 0103 0000 0014 041a 0418 0422 0020 0424  ...........". .$
-000105e0: 0438 043d 0430 043d 0441 0800 0000 0006  .8.=.0.=.A......
-000105f0: 0000 000b 4b49 5420 4669 6e61 6e63 6507  ....KIT Finance.
-00010600: 0000 000c 5374 6174 656d 656e 744b 4954  ....StatementKIT
-00010610: 0103 0000 0032 041e 0442 0447 0451 0442  .....2...B.G.Q.B
-00010620: 0020 041a 0418 0422 0020 0424 0438 043d  . .....". .$.8.=
-00010630: 0430 043d 0441 0020 0028 002a 002e 0078  .0.=.A. .(.*...x
-00010640: 006c 0073 0078 0029 0800 0000 0006 0000  .l.s.x.)........
-00010650: 001e 4b49 5420 4669 6e61 6e63 6520 7374  ..KIT Finance st
-00010660: 6174 656d 656e 7420 282a 2e78 6c73 7829  atement (*.xlsx)
-00010670: 0700 0000 0c53 7461 7465 6d65 6e74 4b49  .....StatementKI
-00010680: 5401 0300 0000 2404 2104 3404 3504 3b04  T.....$.!.4.5.;.
-00010690: 3a04 3800 2004 3704 3004 3304 4004 4304  :.8. .7.0.3.@.C.
-000106a0: 3604 3504 3d04 4b00 3a00 2008 0000 0000  6.5.=.K.:. .....
-000106b0: 0600 0000 0f54 7261 6465 7320 6c6f 6164  .....Trades load
-000106c0: 6564 3a20 0700 0000 0c53 7461 7465 6d65  ed: .....Stateme
-000106d0: 6e74 4b49 5401 0300 0000 3004 1d04 3504  ntKIT.....0...5.
-000106e0: 3804 3704 3204 3504 4104 4204 3d04 4b04  8.7.2.5.A.B.=.K.
-000106f0: 3900 2004 4204 3804 3f00 2004 4104 3404  9. .B.8.?. .A.4.
-00010700: 3504 3b04 3a04 3800 3a00 2008 0000 0000  5.;.:.8.:. .....
-00010710: 0600 0000 1455 6e6b 6e6f 776e 2074 7261  .....Unknown tra
-00010720: 6465 2074 7970 653a 2007 0000 000c 5374  de type: .....St
-00010730: 6174 656d 656e 744b 4954 0103 0000 004a  atementKIT.....J
-00010740: 041d 0435 043f 043e 0434 0434 0435 0440  ...5.?.>.4.4.5.@
-00010750: 0436 0438 0432 0430 0435 043c 0430 044f  .6.8.2.0.5.<.0.O
-00010760: 0020 0434 0435 043d 0435 0436 043d 0430  . .4.5.=.5.6.=.0
-00010770: 044f 0020 0442 0440 0430 043d 0437 0430  .O. .B.@.0.=.7.0
-00010780: 043a 0446 0438 044f 0020 0800 0000 0006  .:.F.8.O. ......
-00010790: 0000 001e 556e 7375 7070 706f 7274 6564  ....Unsuppported
-000107a0: 2063 6173 6820 7472 616e 7361 6374 696f   cash transactio
-000107b0: 6e20 0700 0000 0c53 7461 7465 6d65 6e74  n .....Statement
-000107c0: 4b49 5401 0300 0000 2204 2104 4704 3504  KIT.....".!.G.5.
-000107d0: 4204 3000 2004 3704 3004 3304 4004 4304  B.0. .7.0.3.@.C.
-000107e0: 3604 3504 3d04 4b00 3a00 2008 0000 0000  6.5.=.K.:. .....
-000107f0: 0600 0000 1141 6363 6f75 6e74 7320 6c6f  .....Accounts lo
-00010800: 6164 6564 3a20 0700 0000 1353 7461 7465  aded: .....State
-00010810: 6d65 6e74 4f70 656e 4272 6f6b 6572 0103  mentOpenBroker..
-00010820: 0000 0064 041e 0442 0441 0443 0442 0441  ...d...B.A.C.B.A
-00010830: 0442 0432 0443 044e 0442 0020 0434 0430  .B.2.C.N.B. .4.0
-00010840: 043d 043d 044b 0435 0020 0432 0020 043e  .=.=.K.5. .2. .>
-00010850: 043f 0438 0441 0430 043d 0438 0438 0020  .?.8.A.0.=.8.8. 
-00010860: 043f 043e 0433 0430 0448 0435 043d 0438  .?.>.3.0.H.5.=.8
-00010870: 044f 0020 043e 0431 043b 0438 0433 0430  .O. .>.1.;.8.3.0
-00010880: 0446 0438 0438 0020 0800 0000 0006 0000  .F.8.8. ........
-00010890: 002a 426f 6e64 2072 6570 6179 6d65 6e74  .*Bond repayment
-000108a0: 2064 6573 6372 6970 7469 6f6e 206d 6973   description mis
-000108b0: 7320 736f 6d65 2064 6174 6120 0700 0000  s some data ....
-000108c0: 1353 7461 7465 6d65 6e74 4f70 656e 4272  .StatementOpenBr
-000108d0: 6f6b 6572 0103 0000 0068 041d 0435 0432  oker.....h...5.2
-000108e0: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-000108f0: 0440 0430 0441 043f 043e 0437 043d 0430  .@.0.A.?.>.7.=.0
-00010900: 0442 044c 0020 043d 0430 0437 0432 0430  .B.L. .=.0.7.2.0
-00010910: 043d 0438 0435 0020 043e 0431 043b 0438  .=.8.5. .>.1.;.8
-00010920: 0433 0430 0446 0438 0438 0020 0432 0020  .3.0.F.8.8. .2. 
-00010930: 043e 043f 0438 0441 0430 043d 0438 0438  .>.?.8.A.0.=.8.8
-00010940: 0020 0800 0000 0006 0000 0028 4361 6e27  . .........(Can'
-00010950: 7420 6465 7465 6374 2062 6f6e 6420 6e61  t detect bond na
-00010960: 6d65 2066 726f 6d20 6465 7363 7269 7074  me from descript
-00010970: 696f 6e20 0700 0000 1353 7461 7465 6d65  ion .....Stateme
+0000abc0: 000a 0410 043a 0446 0438 0438 0800 0000  .....:.F.8.8....
+0000abd0: 0006 0000 0006 5368 6172 6573 0700 0000  ......Shares....
+0000abe0: 0f50 7265 6465 6669 6e65 6441 7373 6574  .PredefinedAsset
+0000abf0: 0103 0000 0002 0025 0800 0000 0006 0000  .......%........
+0000ac00: 0001 2507 0000 000f 5072 6f66 6974 4c6f  ..%.....ProfitLo
+0000ac10: 7373 4d6f 6465 6c01 0300 0000 0604 1004  ssModel.........
+0000ac20: 3f04 4008 0000 0000 0600 0000 0341 7072  ?.@..........Apr
+0000ac30: 0700 0000 0f50 726f 6669 744c 6f73 734d  .....ProfitLossM
+0000ac40: 6f64 656c 0103 0000 0004 0426 0411 0800  odel.......&....
+0000ac50: 0000 0006 0000 0006 4173 7365 7473 0700  ........Assets..
+0000ac60: 0000 0f50 726f 6669 744c 6f73 734d 6f64  ...ProfitLossMod
+0000ac70: 656c 0103 0000 0006 0410 0432 0433 0800  el.........2.3..
+0000ac80: 0000 0006 0000 0003 4175 6707 0000 000f  ........Aug.....
+0000ac90: 5072 6f66 6974 4c6f 7373 4d6f 6465 6c01  ProfitLossModel.
+0000aca0: 0300 0000 1204 1804 3704 3c04 3504 3d04  ........7.<.5.=.
+0000acb0: 3504 3d04 3804 3508 0000 0000 0600 0000  5.=.8.5.........
+0000acc0: 0643 6861 6e67 6507 0000 000f 5072 6f66  .Change.....Prof
+0000acd0: 6974 4c6f 7373 4d6f 6465 6c01 0300 0000  itLossModel.....
+0000ace0: 1804 1804 3704 3c04 3504 3d04 3504 3d04  ....7.<.5.=.5.=.
+0000acf0: 3804 3500 2c00 2000 2508 0000 0000 0600  8.5.,. .%.......
+0000ad00: 0000 0943 6861 6e67 652c 2025 0700 0000  ...Change, %....
+0000ad10: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
+0000ad20: 0103 0000 0006 0414 0435 043a 0800 0000  .........5.:....
+0000ad30: 0006 0000 0003 4465 6307 0000 000f 5072  ......Dec.....Pr
+0000ad40: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
+0000ad50: 0000 1204 1404 3804 3204 3804 3404 3504  ......8.2.8.4.5.
+0000ad60: 3d04 3404 4b08 0000 0000 0600 0000 0944  =.4.K..........D
+0000ad70: 6976 6964 656e 6473 0700 0000 0f50 726f  ividends.....Pro
+0000ad80: 6669 744c 6f73 734d 6f64 656c 0103 0000  fitLossModel....
+0000ad90: 0006 0424 0435 0432 0800 0000 0006 0000  ...$.5.2........
+0000ada0: 0003 4665 6207 0000 000f 5072 6f66 6974  ..Feb.....Profit
+0000adb0: 4c6f 7373 4d6f 6465 6c01 0300 0000 1004  LossModel.......
+0000adc0: 1a04 3e04 3c04 3804 4104 4104 3804 3808  ..>.<.8.A.A.8.8.
+0000add0: 0000 0000 0600 0000 0446 6565 7307 0000  .........Fees...
+0000ade0: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
+0000adf0: 6c01 0300 0000 1804 1204 3204 3e04 3400  l.........2.>.4.
+0000ae00: 2000 2f00 2004 1204 4b04 3204 3e04 3408   ./. ...K.2.>.4.
+0000ae10: 0000 0000 0600 0000 0849 6e20 2f20 4f75  .........In / Ou
+0000ae20: 7407 0000 000f 5072 6f66 6974 4c6f 7373  t.....ProfitLoss
+0000ae30: 4d6f 6465 6c01 0300 0000 0604 2f04 3d04  Model......./.=.
+0000ae40: 3208 0000 0000 0600 0000 034a 616e 0700  2..........Jan..
+0000ae50: 0000 0f50 726f 6669 744c 6f73 734d 6f64  ...ProfitLossMod
+0000ae60: 656c 0103 0000 0006 0418 044e 043b 0800  el.........N.;..
+0000ae70: 0000 0006 0000 0003 4a75 6c07 0000 000f  ........Jul.....
+0000ae80: 5072 6f66 6974 4c6f 7373 4d6f 6465 6c01  ProfitLossModel.
+0000ae90: 0300 0000 0604 1804 4e04 3d08 0000 0000  ........N.=.....
+0000aea0: 0600 0000 034a 756e 0700 0000 0f50 726f  .....Jun.....Pro
+0000aeb0: 6669 744c 6f73 734d 6f64 656c 0103 0000  fitLossModel....
+0000aec0: 0006 041c 0430 0440 0800 0000 0006 0000  .....0.@........
+0000aed0: 0003 4d61 7207 0000 000f 5072 6f66 6974  ..Mar.....Profit
+0000aee0: 4c6f 7373 4d6f 6465 6c01 0300 0000 0604  LossModel.......
+0000aef0: 1c04 3004 3908 0000 0000 0600 0000 034d  ..0.9..........M
+0000af00: 6179 0700 0000 0f50 726f 6669 744c 6f73  ay.....ProfitLos
+0000af10: 734d 6f64 656c 0103 0000 0004 0414 0421  sModel.........!
+0000af20: 0800 0000 0006 0000 0005 4d6f 6e65 7907  ..........Money.
+0000af30: 0000 000f 5072 6f66 6974 4c6f 7373 4d6f  ....ProfitLossMo
+0000af40: 6465 6c01 0300 0000 0604 1d04 3e04 4f08  del.........>.O.
+0000af50: 0000 0000 0600 0000 034e 6f76 0700 0000  .........Nov....
+0000af60: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
+0000af70: 0103 0000 0006 041e 043a 0442 0800 0000  .........:.B....
+0000af80: 0006 0000 0003 4f63 7407 0000 000f 5072  ......Oct.....Pr
+0000af90: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
+0000afa0: 0000 0604 1f04 3804 2308 0000 0000 0600  ......8.#.......
+0000afb0: 0000 0350 264c 0700 0000 0f50 726f 6669  ...P&L.....Profi
+0000afc0: 744c 6f73 734d 6f64 656c 0103 0000 000c  tLossModel......
+0000afd0: 041f 0435 0440 0438 043e 0434 0800 0000  ...5.@.8.>.4....
+0000afe0: 0006 0000 0006 5065 7269 6f64 0700 0000  ......Period....
+0000aff0: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
+0000b000: 0103 0000 001a 041a 043e 043d 0435 0446  .........>.=.5.F
+0000b010: 0020 043f 0435 0440 0438 043e 0434 0430  . .?.5.@.8.>.4.0
+0000b020: 0800 0000 0006 0000 000a 5065 7269 6f64  ..........Period
+0000b030: 2065 6e64 0700 0000 0f50 726f 6669 744c   end.....ProfitL
+0000b040: 6f73 734d 6f64 656c 0103 0000 001c 041d  ossModel........
+0000b050: 0430 0447 0430 043b 043e 0020 043f 0435  .0.G.0.;.>. .?.5
+0000b060: 0440 0438 043e 0434 0430 0800 0000 0006  .@.8.>.4.0......
+0000b070: 0000 000c 5065 7269 6f64 2073 7461 7274  ....Period start
+0000b080: 0700 0000 0f50 726f 6669 744c 6f73 734d  .....ProfitLossM
+0000b090: 6f64 656c 0103 0000 0006 0421 0435 043d  odel.......!.5.=
+0000b0a0: 0800 0000 0006 0000 0003 5365 7007 0000  ..........Sep...
+0000b0b0: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
+0000b0c0: 6c01 0300 0000 0c04 1d04 3004 3b04 3e04  l.........0.;.>.
+0000b0d0: 3304 3808 0000 0000 0600 0000 0554 6178  3.8..........Tax
+0000b0e0: 6573 0700 0000 0f50 726f 6669 744c 6f73  es.....ProfitLos
+0000b0f0: 734d 6f64 656c 0103 0000 000a 0418 0442  sModel.........B
+0000b100: 043e 0433 043e 0800 0000 0006 0000 0005  .>.3.>..........
+0000b110: 546f 7461 6c07 0000 000f 5072 6f66 6974  Total.....Profit
+0000b120: 4c6f 7373 4d6f 6465 6c01 0300 0000 1804  LossModel.......
+0000b130: 1f04 3804 2300 2004 3f04 3e00 2004 4104  ..8.#. .?.>. .A.
+0000b140: 4704 5104 4204 4308 0000 0000 0600 0000  G.Q.B.C.........
+0000b150: 0e50 264c 2062 7920 4163 636f 756e 7407  .P&L by Account.
+0000b160: 0000 0010 5072 6f66 6974 4c6f 7373 5265  ....ProfitLossRe
+0000b170: 706f 7274 0103 0000 000a 0421 0447 0435  port.......!.G.5
+0000b180: 0442 003a 0800 0000 0006 0000 0008 4163  .B.:..........Ac
+0000b190: 636f 756e 743a 0700 0000 1650 726f 6669  count:.....Profi
+0000b1a0: 744c 6f73 7352 6570 6f72 7457 6964 6765  tLossReportWidge
+0000b1b0: 7401 0300 0000 1004 1204 3004 3b04 4e04  t.........0.;.N.
+0000b1c0: 4204 3000 3a00 2008 0000 0000 0600 0000  B.0.:. .........
+0000b1d0: 0a43 7572 7265 6e63 793a 2007 0000 0016  .Currency: .....
+0000b1e0: 5072 6f66 6974 4c6f 7373 5265 706f 7274  ProfitLossReport
+0000b1f0: 5769 6467 6574 0103 0000 0006 041f 0438  Widget.........8
+0000b200: 0423 0800 0000 0006 0000 0003 5026 4c07  .#..........P&L.
+0000b210: 0000 0016 5072 6f66 6974 4c6f 7373 5265  ....ProfitLossRe
+0000b220: 706f 7274 5769 6467 6574 0103 0000 0018  portWidget......
+0000b230: 0421 043e 0445 0440 0430 043d 0438 0442  .!.>.E.@.0.=.8.B
+0000b240: 044c 002e 002e 002e 0800 0000 0006 0000  .L..............
+0000b250: 0007 5361 7665 2e2e 2e07 0000 0016 5072  ..Save........Pr
+0000b260: 6f66 6974 4c6f 7373 5265 706f 7274 5769  ofitLossReportWi
+0000b270: 6467 6574 0103 0000 0010 0412 0430 043b  dget.........0.;
+0000b280: 044e 0442 0430 003a 0020 0800 0000 0006  .N.B.0.:. ......
+0000b290: 0000 000a 4375 7272 656e 6379 3a20 0700  ....Currency: ..
+0000b2a0: 0000 1650 726f 6669 744c 6f73 7352 6570  ...ProfitLossRep
+0000b2b0: 6f72 7457 696e 646f 7701 0300 0000 1804  ortWindow.......
+0000b2c0: 1f04 3804 2300 2004 3f04 3e00 2004 4104  ..8.#. .?.>. .A.
+0000b2d0: 4704 5104 4204 4308 0000 0000 0600 0000  G.Q.B.C.........
+0000b2e0: 0e50 264c 2062 7920 4163 636f 756e 7407  .P&L by Account.
+0000b2f0: 0000 0016 5072 6f66 6974 4c6f 7373 5265  ....ProfitLossRe
+0000b300: 706f 7274 5769 6e64 6f77 0103 0000 001e  portWindow......
+0000b310: 041e 0448 0438 0431 043a 0430 0020 043a  ...H.8.1.:.0. .:
+0000b320: 0430 043c 0435 0440 044b 003a 0020 0800  .0.<.5.@.K.:. ..
+0000b330: 0000 0006 0000 000e 4361 6d65 7261 2065  ........Camera e
+0000b340: 7272 6f72 3a20 0700 0000 0951 5253 6361  rror: .....QRSca
+0000b350: 6e6e 6572 0103 0000 0084 041d 0435 0020  nner.........5. 
+0000b360: 043e 0431 043d 0430 0440 0443 0436 0435  .>.1.=.0.@.C.6.5
+0000b370: 043d 0020 043f 0430 043a 0435 0442 0020  .=. .?.0.:.5.B. 
+0000b380: 0070 0079 007a 0062 0061 0072 002c 0020  .p.y.z.b.a.r.,. 
+0000b390: 043d 0435 043e 0431 0445 043e 0434 0438  .=.5.>.1.E.>.4.8
+0000b3a0: 043c 044b 0439 0020 0434 043b 044f 0020  .<.K.9. .4.;.O. 
+0000b3b0: 0440 0430 0441 043f 043e 0437 043d 0430  .@.0.A.?.>.7.=.0
+0000b3c0: 0432 0430 043d 0438 044f 0020 0051 0052  .2.0.=.8.O. .Q.R
+0000b3d0: 0020 043a 043e 0434 043e 0432 002e 0800  . .:.>.4.>.2....
+0000b3e0: 0000 0006 0000 002c 5061 636b 6167 6520  .......,Package 
+0000b3f0: 7079 7a62 6172 206e 6f74 2066 6f75 6e64  pyzbar not found
+0000b400: 2066 6f72 2051 5220 7265 636f 676e 6974   for QR recognit
+0000b410: 696f 6e2e 0700 0000 0951 5253 6361 6e6e  ion......QRScann
+0000b420: 6572 0103 0000 0026 041d 0435 0442 0020  er.....&...5.B. 
+0000b430: 0434 043e 0441 0442 0443 043f 043d 044b  .4.>.A.B.C.?.=.K
+0000b440: 0445 0020 043a 0430 043c 0435 0440 0800  .E. .:.0.<.5.@..
+0000b450: 0000 0006 0000 001e 5468 6572 6520 6172  ........There ar
+0000b460: 6520 6e6f 2063 616d 6572 6173 2061 7661  e no cameras ava
+0000b470: 696c 6162 6c65 0700 0000 0951 5253 6361  ilable.....QRSca
+0000b480: 6e6e 6572 0103 0000 0068 041d 0435 0432  nner.....h...5.2
+0000b490: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+0000b4a0: 043e 0431 0440 0430 0431 043e 0442 0430  .>.1.@.0.1.>.B.0
+0000b4b0: 0442 044c 0020 0434 0430 043d 043d 044b  .B.L. .4.0.=.=.K
+0000b4c0: 0435 0020 043a 043e 0442 0438 0440 043e  .5. .:.>.B.8.@.>
+0000b4d0: 0432 043e 043a 0020 0441 0020 0431 0438  .2.>.:. .A. .1.8
+0000b4e0: 0440 0436 0438 0020 0054 0053 0058 003a  .@.6.8. .T.S.X.:
+0000b4f0: 0020 0800 0000 0006 0000 0021 4361 6e27  . .........!Can'
+0000b500: 7420 7061 7273 6520 6461 7461 2066 6f72  t parse data for
+0000b510: 2054 5358 2071 756f 7465 733a 2007 0000   TSX quotes: ...
+0000b520: 000f 5175 6f74 6544 6f77 6e6c 6f61 6465  ..QuoteDownloade
+0000b530: 7201 0300 0000 2404 1704 3004 3304 4004  r.....$...0.3.@.
+0000b540: 4304 3704 3a04 3000 2004 3704 3004 3204  C.7.:.0. .7.0.2.
+0000b550: 3504 4004 4804 3504 3d04 3008 0000 0000  5.@.H.5.=.0.....
+0000b560: 0600 0000 1244 6f77 6e6c 6f61 6420 636f  .....Download co
+0000b570: 6d70 6c65 7465 6407 0000 000f 5175 6f74  mpleted.....Quot
+0000b580: 6544 6f77 6e6c 6f61 6465 7201 0300 0000  eDownloader.....
+0000b590: 6000 4900 5300 4900 4e00 2004 3200 2004  `.I.S.I.N. .2. .
+0000b5a0: 3804 4104 4204 3e04 4004 3804 3800 2004  8.A.B.>.@.8.8. .
+0000b5b0: 3a04 3e04 4204 3804 4004 3e04 3204 3e04  :.>.B.8.@.>.2.>.
+0000b5c0: 3a00 2000 4500 7500 7200 6f00 6e00 6500  :. .E.u.r.o.n.e.
+0000b5d0: 7800 7400 2004 3d04 3500 2004 4104 3e04  x.t. .=.5. .A.>.
+0000b5e0: 3204 3f04 3004 3404 3004 3504 4200 3a00  2.?.0.4.0.5.B.:.
+0000b5f0: 2008 0000 0000 0600 0000 2245 7572 6f6e   ........."Euron
+0000b600: 6578 7420 7175 6f74 6573 2049 5349 4e20  ext quotes ISIN 
+0000b610: 6d69 736d 6174 6368 2069 6e3a 2007 0000  mismatch in: ...
+0000b620: 000f 5175 6f74 6544 6f77 6e6c 6f61 6465  ..QuoteDownloade
+0000b630: 7201 0300 0000 6404 1704 3004 3304 3e04  r.....d...0.3.>.
+0000b640: 3b04 3e04 3204 3e04 3a00 2004 3804 4104  ;.>.2.>.:. .8.A.
+0000b650: 4204 3e04 4004 3804 3800 2004 3a04 3e04  B.>.@.8.8. .:.>.
+0000b660: 4204 3804 4004 3e04 3204 3e04 3a00 2000  B.8.@.>.2.>.:. .
+0000b670: 4500 7500 7200 6f00 6e00 6500 7800 7400  E.u.r.o.n.e.x.t.
+0000b680: 2004 3d04 3500 2004 3d04 3004 3904 3404   .=.5. .=.0.9.4.
+0000b690: 3504 3d00 2004 3200 3a00 2008 0000 0000  5.=. .2.:. .....
+0000b6a0: 0600 0000 2545 7572 6f6e 6578 7420 7175  ....%Euronext qu
+0000b6b0: 6f74 6573 2068 6561 6465 7220 6e6f 7420  otes header not 
+0000b6c0: 666f 756e 6420 696e 3a20 0700 0000 0f51  found in: .....Q
+0000b6d0: 756f 7465 446f 776e 6c6f 6164 6572 0103  uoteDownloader..
+0000b6e0: 0000 005a 0418 0441 0442 043e 0440 0438  ...Z...A.B.>.@.8
+0000b6f0: 044f 0020 043a 043e 0442 0438 0440 043e  .O. .:.>.B.8.@.>
+0000b700: 0432 043e 043a 0020 0045 0075 0072 006f  .2.>.:. .E.u.r.o
+0000b710: 006e 0065 0078 0074 0020 0441 043b 0438  .n.e.x.t. .A.;.8
+0000b720: 0448 043a 043e 043c 0020 043a 043e 0440  .H.:.>.<. .:.>.@
+0000b730: 043e 0442 043a 0430 044f 003a 0020 0800  .>.B.:.0.O.:. ..
+0000b740: 0000 0006 0000 002c 4575 726f 6e65 7874  .......,Euronext
+0000b750: 2071 756f 7465 7320 6869 7374 6f72 7920   quotes history 
+0000b760: 7265 706c 7920 6973 2074 6f6f 2073 686f  reply is too sho
+0000b770: 7274 3a20 0700 0000 0f51 756f 7465 446f  rt: .....QuoteDo
+0000b780: 776e 6c6f 6164 6572 0103 0000 0036 041d  wnloader.....6..
+0000b790: 0435 0020 0437 0430 0433 0440 0443 0436  .5. .7.0.3.@.C.6
+0000b7a0: 0435 043d 044b 0020 043a 043e 0442 0438  .5.=.K. .:.>.B.8
+0000b7b0: 0440 043e 0432 043a 0438 0020 0434 043b  .@.>.2.:.8. .4.;
+0000b7c0: 044f 0020 0800 0000 0006 0000 001e 4e6f  .O. ..........No
+0000b7d0: 2071 756f 7465 7320 7765 7265 2064 6f77   quotes were dow
+0000b7e0: 6e6c 6f61 6465 6420 666f 7220 0700 0000  nloaded for ....
+0000b7f0: 0f51 756f 7465 446f 776e 6c6f 6164 6572  .QuoteDownloader
+0000b800: 0103 0000 002e 041d 0435 0020 0437 0430  .........5. .7.0
+0000b810: 0433 0440 0443 0436 0435 043d 044b 0020  .3.@.C.6.5.=.K. 
+0000b820: 043a 0443 0440 0441 044b 0020 0434 043b  .:.C.@.A.K. .4.;
+0000b830: 044f 0020 0800 0000 0006 0000 001d 4e6f  .O. ..........No
+0000b840: 2072 6174 6573 2077 6572 6520 646f 776e   rates were down
+0000b850: 6c6f 6164 6564 2066 6f72 2007 0000 000f  loaded for .....
+0000b860: 5175 6f74 6544 6f77 6e6c 6f61 6465 7201  QuoteDownloader.
+0000b870: 0300 0000 2c04 1d04 3504 4200 2004 3404  ....,...5.B. .4.
+0000b880: 3004 3d04 3d04 4b04 4500 2004 2604 1100  0.=.=.K.E. .&...
+0000b890: 2004 2004 2400 2004 3404 3b04 4f00 3a00   . .$. .4.;.O.:.
+0000b8a0: 2008 0000 0000 0600 0000 1b54 6865 7265   ..........There
+0000b8b0: 2061 7265 206e 6f20 4342 5220 6461 7461   are no CBR data
+0000b8c0: 2066 6f72 3a20 0700 0000 0f51 756f 7465   for: .....Quote
+0000b8d0: 446f 776e 6c6f 6164 6572 0103 0000 0012  Downloader......
+0000b8e0: 041a 043e 0442 0438 0440 043e 0432 043a  ...>.B.8.@.>.2.:
+0000b8f0: 0438 0800 0000 0006 0000 0006 5175 6f74  .8..........Quot
+0000b900: 6573 0700 0000 1051 756f 7465 734c 6973  es.....QuotesLis
+0000b910: 7444 6961 6c6f 6701 0300 0000 0404 2604  tDialog.......&.
+0000b920: 1108 0000 0000 0600 0000 0541 7373 6574  ...........Asset
+0000b930: 0700 0000 0f51 756f 7465 734c 6973 744d  .....QuotesListM
+0000b940: 6f64 656c 0103 0000 000c 0412 0430 043b  odel.........0.;
+0000b950: 044e 0442 0430 0800 0000 0006 0000 0008  .N.B.0..........
+0000b960: 4375 7272 656e 6379 0700 0000 0f51 756f  Currency.....Quo
+0000b970: 7465 734c 6973 744d 6f64 656c 0103 0000  tesListModel....
+0000b980: 0008 0414 0430 0442 0430 0800 0000 0006  .....0.B.0......
+0000b990: 0000 0004 4461 7465 0700 0000 0f51 756f  ....Date.....Quo
+0000b9a0: 7465 734c 6973 744d 6f64 656c 0103 0000  tesListModel....
+0000b9b0: 0012 041a 043e 0442 0438 0440 043e 0432  .....>.B.8.@.>.2
+0000b9c0: 043a 0430 0800 0000 0006 0000 0005 5175  .:.0..........Qu
+0000b9d0: 6f74 6507 0000 000f 5175 6f74 6573 4c69  ote.....QuotesLi
+0000b9e0: 7374 4d6f 6465 6c01 0300 0000 2800 2604  stModel.....(.&.
+0000b9f0: 1f04 3e04 3b04 3d04 3e04 4104 4204 4c04  ..>.;.=.>.A.B.L.
+0000ba00: 4e00 2c00 2004 4100 2004 3d04 3004 4704  N.,. .A. .=.0.G.
+0000ba10: 3004 3b04 3008 0000 0000 0600 0000 1326  0.;.0..........&
+0000ba20: 4675 6c6c 2c20 6672 6f6d 2073 6372 6174  Full, from scrat
+0000ba30: 6368 0700 0000 0d52 6542 7569 6c64 4469  ch.....ReBuildDi
+0000ba40: 616c 6f67 0103 0000 0018 0418 043d 0442  alog.........=.B
+0000ba50: 0435 0440 0432 0430 043b 0020 0434 0430  .5.@.2.0.;. .4.0
+0000ba60: 0442 0800 0000 0006 0000 000a 4461 7465  .B..........Date
+0000ba70: 2052 616e 6765 0700 0000 0d52 6542 7569   Range.....ReBui
+0000ba80: 6c64 4469 616c 6f67 0103 0000 002a 0026  ldDialog.....*.&
+0000ba90: 0411 044b 0441 0442 0440 043e 002c 0020  ...K.A.B.@.>.,. 
+0000baa0: 043d 043e 0020 043d 0435 043d 0430 0434  .=.>. .=.5.=.0.4
+0000bab0: 0451 0436 043d 043e 0800 0000 0006 0000  .Q.6.=.>........
+0000bac0: 0011 4661 7374 2c20 2675 6e72 656c 6961  ..Fast, &unrelia
+0000bad0: 626c 6507 0000 000d 5265 4275 696c 6444  ble.....ReBuildD
+0000bae0: 6961 6c6f 6701 0300 0000 1604 1404 3004  ialog.........0.
+0000baf0: 4204 3004 1304 4004 3004 3d04 3804 4604  B.0...@.0.=.8.F.
+0000bb00: 4b08 0000 0000 0600 0000 0c46 726f 6e74  K..........Front
+0000bb10: 6965 7244 6174 6507 0000 000d 5265 4275  ierDate.....ReBu
+0000bb20: 696c 6444 6961 6c6f 6701 0300 0000 2204  ildDialog.....".
+0000bb30: 1f04 3504 4004 3504 4104 4704 3804 4204  ..5.@.5.A.G.8.B.
+0000bb40: 3004 4204 4c00 2004 3804 4204 3e04 3304  0.B.L. .8.B.>.3.
+0000bb50: 3808 0000 0000 0600 0000 0f52 652d 4275  8..........Re-Bu
+0000bb60: 696c 6420 4c65 6467 6572 0700 0000 0d52  ild Ledger.....R
+0000bb70: 6542 7569 6c64 4469 616c 6f67 0103 0000  eBuildDialog....
+0000bb80: 0010 0421 0020 0026 0414 0430 0442 044b  ...!. .&...0.B.K
+0000bb90: 003a 0800 0000 0006 0000 000c 5369 6e63  .:..........Sinc
+0000bba0: 6520 2644 6174 653a 0700 0000 0d52 6542  e &Date:.....ReB
+0000bbb0: 7569 6c64 4469 616c 6f67 0103 0000 002c  uildDialog.....,
+0000bbc0: 0421 0020 043a 0440 0430 0439 043d 0435  .!. .:.@.0.9.=.5
+0000bbd0: 0439 0020 0026 0430 043a 0442 0443 0430  .9. .&.0.:.B.C.0
+0000bbe0: 043b 044c 043d 043e 0439 003a 0800 0000  .;.L.=.>.9.:....
+0000bbf0: 0006 0000 0013 5369 6e63 6520 264c 6173  ......Since &Las
+0000bc00: 7420 6163 7475 616c 3a07 0000 000d 5265  t actual:.....Re
+0000bc10: 4275 696c 6444 6961 6c6f 6701 0300 0000  BuildDialog.....
+0000bc20: 1400 6400 6400 2f00 4d00 4d00 2f00 7900  ..d.d./.M.M./.y.
+0000bc30: 7900 7900 7908 0000 0000 0600 0000 0a64  y.y.y..........d
+0000bc40: 642f 4d4d 2f79 7979 7907 0000 000d 5265  d/MM/yyyy.....Re
+0000bc50: 4275 696c 6444 6961 6c6f 6701 0300 0000  BuildDialog.....
+0000bc60: 0a04 1b04 4e04 3104 3e04 3908 0000 0000  ....N.1.>.9.....
+0000bc70: 0600 0000 0341 4e59 0700 0000 1352 6566  .....ANY.....Ref
+0000bc80: 6572 656e 6365 4461 7461 4469 616c 6f67  erenceDataDialog
+0000bc90: 0103 0000 0014 0422 0438 043f 0020 0441  .......".8.?. .A
+0000bca0: 0447 0435 0442 0430 003a 0800 0000 0006  .G.5.B.0.:......
+0000bcb0: 0000 000d 4163 636f 756e 7420 5479 7065  ....Account Type
+0000bcc0: 3a07 0000 0013 5265 6665 7265 6e63 6544  :.....ReferenceD
+0000bcd0: 6174 6144 6961 6c6f 6701 0300 0000 2204  ataDialog.....".
+0000bce0: 1404 3e04 3104 3004 3204 3804 4204 4c00  ..>.1.0.2.8.B.L.
+0000bcf0: 2004 3404 3e04 4704 3504 4004 3d04 3804   .4.>.G.5.@.=.8.
+0000bd00: 3908 0000 0000 0600 0000 0941 6464 2063  9..........Add c
+0000bd10: 6869 6c64 0700 0000 1352 6566 6572 656e  hild.....Referen
+0000bd20: 6365 4461 7461 4469 616c 6f67 0103 0000  ceDataDialog....
+0000bd30: 001c 0414 043e 0431 0430 0432 0438 0442  .....>.1.0.2.8.B
+0000bd40: 044c 0020 043d 043e 0432 044b 0439 0800  .L. .=.>.2.K.9..
+0000bd50: 0000 0006 0000 0007 4164 6420 6e65 7707  ........Add new.
+0000bd60: 0000 0013 5265 6665 7265 6e63 6544 6174  ....ReferenceDat
+0000bd70: 6144 6961 6c6f 6701 0300 0000 1e04 2104  aDialog.......!.
+0000bd80: 3c04 3504 3d04 3804 4204 4c00 2004 4204  <.5.=.8.B.L. .B.
+0000bd90: 3804 3f00 2004 3d04 3000 3a08 0000 0000  8.?. .=.0.:.....
+0000bda0: 0600 0000 0f43 6861 6e67 6520 7479 7065  .....Change type
+0000bdb0: 2074 6f3a 0700 0000 1352 6566 6572 656e   to:.....Referen
+0000bdc0: 6365 4461 7461 4469 616c 6f67 0103 0000  ceDataDialog....
+0000bdd0: 001a 041f 043e 0434 0442 0432 0435 0440  .....>.4.B.2.5.@
+0000bde0: 0436 0434 0435 043d 0438 0435 0800 0000  .6.4.5.=.8.5....
+0000bdf0: 0006 0000 000c 436f 6e66 6972 6d61 7469  ......Confirmati
+0000be00: 6f6e 0700 0000 1352 6566 6572 656e 6365  on.....Reference
+0000be10: 4461 7461 4469 616c 6f67 0103 0000 000e  DataDialog......
+0000be20: 0423 0434 0430 043b 0438 0442 044c 0800  .#.4.0.;.8.B.L..
+0000be30: 0000 0006 0000 0006 4465 6c65 7465 0700  ........Delete..
+0000be40: 0000 1352 6566 6572 656e 6365 4461 7461  ...ReferenceData
+0000be50: 4469 616c 6f67 0103 0000 0022 0421 043f  Dialog.....".!.?
+0000be60: 0440 0430 0432 043e 0447 043d 044b 0435  .@.0.2.>.G.=.K.5
+0000be70: 0020 0434 0430 043d 043d 044b 0435 0800  . .4.0.=.=.K.5..
+0000be80: 0000 0006 0000 000e 5265 6665 7265 6e63  ........Referenc
+0000be90: 6520 4461 7461 0700 0000 1352 6566 6572  e Data.....Refer
+0000bea0: 656e 6365 4461 7461 4469 616c 6f67 0103  enceDataDialog..
+0000beb0: 0000 0024 041e 0442 043c 0435 043d 0438  ...$...B.<.5.=.8
+0000bec0: 0442 044c 0020 0438 0437 043c 0435 043d  .B.L. .8.7.<.5.=
+0000bed0: 0435 043d 0438 044f 0800 0000 0006 0000  .5.=.8.O........
+0000bee0: 000e 5265 7665 7274 2063 6861 6e67 6573  ..Revert changes
+0000bef0: 0700 0000 1352 6566 6572 656e 6365 4461  .....ReferenceDa
+0000bf00: 7461 4469 616c 6f67 0103 0000 0026 0421  taDialog.....&.!
+0000bf10: 043e 0445 0440 0430 043d 0438 0442 044c  .>.E.@.0.=.8.B.L
+0000bf20: 0020 0438 0437 043c 0435 043d 0435 043d  . .8.7.<.5.=.5.=
+0000bf30: 0438 044f 0800 0000 0006 0000 000c 5361  .8.O..........Sa
+0000bf40: 7665 2063 6861 6e67 6573 0700 0000 1352  ve changes.....R
+0000bf50: 6566 6572 656e 6365 4461 7461 4469 616c  eferenceDataDial
+0000bf60: 6f67 0103 0000 000c 041f 043e 0438 0441  og.........>.8.A
+0000bf70: 043a 003a 0800 0000 0006 0000 0007 5365  .:.:..........Se
+0000bf80: 6172 6368 3a07 0000 0013 5265 6665 7265  arch:.....Refere
+0000bf90: 6e63 6544 6174 6144 6961 6c6f 6701 0300  nceDataDialog...
+0000bfa0: 0000 2a04 1f04 3e04 3a04 3004 3704 4b04  ..*...>.:.0.7.K.
+0000bfb0: 3204 3004 4204 4c00 2004 3d04 3504 3004  2.0.B.L. .=.5.0.
+0000bfc0: 3a04 4204 3804 3204 3d04 4b04 3508 0000  :.B.8.2.=.K.5...
+0000bfd0: 0000 0600 0000 0d53 686f 7720 696e 6163  .......Show inac
+0000bfe0: 7469 7665 0700 0000 1352 6566 6572 656e  tive.....Referen
+0000bff0: 6365 4461 7461 4469 616c 6f67 0103 0000  ceDataDialog....
+0000c000: 0066 0423 0020 0432 0430 0441 0020 0435  .f.#. .2.0.A. .5
+0000c010: 0441 0442 044c 0020 043d 0435 0441 043e  .A.B.L. .=.5.A.>
+0000c020: 0445 0440 0430 043d 0451 043d 043d 044b  .E.@.0.=.Q.=.=.K
+0000c030: 0435 0020 0434 0430 043d 043d 044b 0435  .5. .4.0.=.=.K.5
+0000c040: 002e 0020 0412 0441 0451 0020 0440 0430  ... ...A.Q. .@.0
+0000c050: 0432 043d 043e 0020 0437 0430 043a 0440  .2.=.>. .7.0.:.@
+0000c060: 044b 0442 044c 003f 0800 0000 0006 0000  .K.B.L.?........
+0000c070: 0033 596f 7520 6861 7665 2075 6e63 6f6d  .3You have uncom
+0000c080: 6d69 7474 6564 2063 6861 6e67 6573 2e20  mitted changes. 
+0000c090: 446f 2079 6f75 2077 616e 7420 746f 2063  Do you want to c
+0000c0a0: 6c6f 7365 3f07 0000 0013 5265 6665 7265  lose?.....Refere
+0000c0b0: 6e63 6544 6174 6144 6961 6c6f 6701 0300  nceDataDialog...
+0000c0c0: 0000 0604 1004 3f04 4008 0000 0000 0600  ......?.@.......
+0000c0d0: 0000 0341 7072 0700 0000 0e52 6570 6f72  ...Apr.....Repor
+0000c0e0: 7454 7265 6549 7465 6d01 0300 0000 0604  tTreeItem.......
+0000c0f0: 1004 3204 3308 0000 0000 0600 0000 0341  ..2.3..........A
+0000c100: 7567 0700 0000 0e52 6570 6f72 7454 7265  ug.....ReportTre
+0000c110: 6549 7465 6d01 0300 0000 0604 1404 3504  eItem.........5.
+0000c120: 3a08 0000 0000 0600 0000 0344 6563 0700  :..........Dec..
+0000c130: 0000 0e52 6570 6f72 7454 7265 6549 7465  ...ReportTreeIte
+0000c140: 6d01 0300 0000 0604 2404 3504 3208 0000  m.......$.5.2...
+0000c150: 0000 0600 0000 0346 6562 0700 0000 0e52  .......Feb.....R
+0000c160: 6570 6f72 7454 7265 6549 7465 6d01 0300  eportTreeItem...
+0000c170: 0000 0604 2f04 3d04 3208 0000 0000 0600  ..../.=.2.......
+0000c180: 0000 034a 616e 0700 0000 0e52 6570 6f72  ...Jan.....Repor
+0000c190: 7454 7265 6549 7465 6d01 0300 0000 0604  tTreeItem.......
+0000c1a0: 1804 4e04 3b08 0000 0000 0600 0000 034a  ..N.;..........J
+0000c1b0: 756c 0700 0000 0e52 6570 6f72 7454 7265  ul.....ReportTre
+0000c1c0: 6549 7465 6d01 0300 0000 0604 1804 4e04  eItem.........N.
+0000c1d0: 3d08 0000 0000 0600 0000 034a 756e 0700  =..........Jun..
+0000c1e0: 0000 0e52 6570 6f72 7454 7265 6549 7465  ...ReportTreeIte
+0000c1f0: 6d01 0300 0000 0604 1c04 3004 4008 0000  m.........0.@...
+0000c200: 0000 0600 0000 034d 6172 0700 0000 0e52  .......Mar.....R
+0000c210: 6570 6f72 7454 7265 6549 7465 6d01 0300  eportTreeItem...
+0000c220: 0000 0604 1c04 3004 3908 0000 0000 0600  ......0.9.......
+0000c230: 0000 034d 6179 0700 0000 0e52 6570 6f72  ...May.....Repor
+0000c240: 7454 7265 6549 7465 6d01 0300 0000 0604  tTreeItem.......
+0000c250: 1d04 3e04 4f08 0000 0000 0600 0000 034e  ..>.O..........N
+0000c260: 6f76 0700 0000 0e52 6570 6f72 7454 7265  ov.....ReportTre
+0000c270: 6549 7465 6d01 0300 0000 0604 1e04 3a04  eItem.........:.
+0000c280: 4208 0000 0000 0600 0000 034f 6374 0700  B..........Oct..
+0000c290: 0000 0e52 6570 6f72 7454 7265 6549 7465  ...ReportTreeIte
+0000c2a0: 6d01 0300 0000 0604 2104 3504 3d08 0000  m.......!.5.=...
+0000c2b0: 0000 0600 0000 0353 6570 0700 0000 0e52  .......Sep.....R
+0000c2c0: 6570 6f72 7454 7265 6549 7465 6d01 0300  eportTreeItem...
+0000c2d0: 0000 0604 3d04 3504 3408 0000 0000 0600  ....=.5.4.......
+0000c2e0: 0000 0277 6b07 0000 000e 5265 706f 7274  ...wk.....Report
+0000c2f0: 5472 6565 4974 656d 0103 0000 0028 0424  TreeItem.....(.$
+0000c300: 0430 0439 043b 044b 0020 0045 0078 0063  .0.9.;.K. .E.x.c
+0000c310: 0065 006c 0020 0028 002a 002e 0078 0073  .e.l. .(.*...x.s
+0000c320: 006c 0078 0029 0800 0000 0006 0000 0014  .l.x.)..........
+0000c330: 4578 6365 6c20 6669 6c65 7320 282a 2e78  Excel files (*.x
+0000c340: 6c73 7829 0700 0000 0752 6570 6f72 7473  lsx).....Reports
+0000c350: 0103 0000 0046 041d 0435 0432 043e 0437  .....F...5.2.>.7
+0000c360: 043c 043e 0436 043d 043e 0020 0437 0430  .<.>.6.=.>. .7.0
+0000c370: 0433 0440 0443 0437 0438 0442 044c 0020  .3.@.C.7.8.B.L. 
+0000c380: 043a 043b 0430 0441 0441 0020 043e 0442  .:.;.0.A.A. .>.B
+0000c390: 0447 0451 0442 0430 003a 0020 0800 0000  .G.Q.B.0.:. ....
+0000c3a0: 0006 0000 001e 5265 706f 7274 2063 6c61  ......Report cla
+0000c3b0: 7373 2063 616e 2774 2062 6520 6c6f 6164  ss can't be load
+0000c3c0: 6564 3a20 0700 0000 0752 6570 6f72 7473  ed: .....Reports
+0000c3d0: 0103 0000 0042 041e 0442 0447 0435 0442  .....B...B.G.5.B
+0000c3e0: 0020 043d 0435 0020 043d 0430 0439 0434  . .=.5. .=.0.9.4
+0000c3f0: 0435 043d 0020 0434 043b 044f 0020 043a  .5.=. .4.;.O. .:
+0000c400: 043b 0430 0441 0441 0430 0020 043e 043a  .;.0.A.A.0. .>.:
+0000c410: 043d 0430 003a 0020 0800 0000 0006 0000  .=.0.:. ........
+0000c420: 0023 5265 706f 7274 206e 6f74 2066 6f75  .#Report not fou
+0000c430: 6e64 2066 6f72 2077 696e 646f 7720 636c  nd for window cl
+0000c440: 6173 733a 2007 0000 0007 5265 706f 7274  ass: .....Report
+0000c450: 7301 0300 0000 2c04 1e04 4204 4704 3504  s.....,...B.G.5.
+0000c460: 4200 2004 4104 3e04 4504 4004 3004 3d04  B. .A.>.E.@.0.=.
+0000c470: 5104 3d00 2004 3200 2004 4404 3004 3904  Q.=. .2. .D.0.9.
+0000c480: 3b00 2008 0000 0000 0600 0000 1952 6570  ;. ..........Rep
+0000c490: 6f72 7420 7761 7320 7361 7665 6420 746f  ort was saved to
+0000c4a0: 2066 696c 6520 0700 0000 0752 6570 6f72   file .....Repor
+0000c4b0: 7473 0103 0000 0024 0421 043e 0445 0440  ts.....$.!.>.E.@
+0000c4c0: 0430 043d 0438 0442 044c 0020 043e 0442  .0.=.8.B.L. .>.B
+0000c4d0: 0447 0435 0442 0020 0432 003a 0800 0000  .G.5.B. .2.:....
+0000c4e0: 0006 0000 000f 5361 7665 2072 6570 6f72  ......Save repor
+0000c4f0: 7420 746f 3a07 0000 0007 5265 706f 7274  t to:.....Report
+0000c500: 7301 0300 0000 3c04 1b04 3e04 3304 3804  s.....<...>.3.8.
+0000c510: 3d00 2004 4704 3504 4004 3504 3700 2004  =. .G.5.@.5.7. .
+0000c520: 1304 3e04 4104 4304 4104 3b04 4304 3304  ..>.A.C.A.;.C.3.
+0000c530: 3800 2004 3704 3004 3204 3504 4004 4804  8. .7.0.2.5.@.H.
+0000c540: 5104 3d08 0000 0000 0600 0000 1445 5349  Q.=..........ESI
+0000c550: 4120 6c6f 6769 6e20 636f 6d70 6c65 7465  A login complete
+0000c560: 6407 0000 0012 5265 7175 6573 7449 6e74  d.....RequestInt
+0000c570: 6572 6365 7074 6f72 0103 0000 000a 0410  erceptor........
+0000c580: 043a 0442 0438 0432 0800 0000 0006 0000  .:.B.8.2........
+0000c590: 0005 4173 7365 7407 0000 000c 5265 7375  ..Asset.....Resu
+0000c5a0: 6c74 734d 6f64 656c 0103 0000 000c 041a  ltsModel........
+0000c5b0: 043e 043b 002d 0432 043e 0800 0000 0006  .>.;.-.2.>......
+0000c5c0: 0000 0003 5174 7907 0000 000c 5265 7375  ....Qty.....Resu
+0000c5d0: 6c74 734d 6f64 656c 0103 0000 000e 0414  ltsModel........
+0000c5e0: 043e 043b 044f 002c 0020 0025 0800 0000  .>.;.O.,. .%....
+0000c5f0: 0006 0000 0008 5368 6172 652c 2025 0700  ......Share, %..
+0000c600: 0000 0c52 6573 756c 7473 4d6f 6465 6c01  ...ResultsModel.
+0000c610: 0300 0000 3004 1204 4b04 3104 4004 3004  ....0...K.1.@.0.
+0000c620: 3d00 2004 3d04 3504 3a04 3e04 4004 4004  =. .=.5.:.>.@.@.
+0000c630: 3504 3a04 4204 3d04 4b04 3900 2004 4104  5.:.B.=.K.9. .A.
+0000c640: 4704 5104 4208 0000 0000 0600 0000 1849  G.Q.B..........I
+0000c650: 6e76 616c 6964 2061 6363 6f75 6e74 2073  nvalid account s
+0000c660: 656c 6563 7465 6407 0000 0013 5365 6c65  elected.....Sele
+0000c670: 6374 4163 636f 756e 7444 6961 6c6f 6701  ctAccountDialog.
+0000c680: 0300 0000 2204 1d04 3804 4704 3504 3304  ...."...8.G.5.3.
+0000c690: 3e00 2004 3d04 3500 2004 3204 4b04 3104  >. .=.5. .2.K.1.
+0000c6a0: 4004 3004 3d04 3e08 0000 0000 0600 0000  @.0.=.>.........
+0000c6b0: 0c4e 6f20 7365 6c65 6374 696f 6e07 0000  .No selection...
+0000c6c0: 0013 5365 6c65 6374 4163 636f 756e 7444  ..SelectAccountD
+0000c6d0: 6961 6c6f 6701 0300 0000 4004 1f04 3e04  ialog.....@...>.
+0000c6e0: 3604 3004 3b04 4304 3904 4104 4204 3000  6.0.;.C.9.A.B.0.
+0000c6f0: 2c00 2004 3204 4b04 3104 3504 4004 3804  ,. .2.K.1.5.@.8.
+0000c700: 4204 3500 2004 3404 4004 4304 3304 3e04  B.5. .4.@.C.3.>.
+0000c710: 3900 2004 4104 4704 5104 4208 0000 0000  9. .A.G.Q.B.....
+0000c720: 0600 0000 1f50 6c65 6173 6520 7365 6c65  .....Please sele
+0000c730: 6374 2064 6966 6665 7265 6e74 2061 6363  ct different acc
+0000c740: 6f75 6e74 0700 0000 1353 656c 6563 7441  ount.....SelectA
+0000c750: 6363 6f75 6e74 4469 616c 6f67 0103 0000  ccountDialog....
+0000c760: 0030 041f 043e 0436 0430 043b 0443 0439  .0...>.6.0.;.C.9
+0000c770: 0441 0442 0430 0020 0432 044b 0431 0435  .A.B.0. .2.K.1.5
+0000c780: 0440 0438 0442 0435 0020 0441 0447 0451  .@.8.B.5. .A.G.Q
+0000c790: 0442 0800 0000 0006 0000 0015 506c 6561  .B..........Plea
+0000c7a0: 7365 2073 656c 6563 7420 6163 636f 756e  se select accoun
+0000c7b0: 7407 0000 0010 5365 6c65 6374 4163 636f  t.....SelectAcco
+0000c7c0: 756e 7444 6c67 0103 0000 0012 0421 043e  untDlg.......!.>
+0000c7d0: 043e 0431 0449 0435 043d 0438 0435 0800  .>.1.I.5.=.8.5..
+0000c7e0: 0000 0006 0000 0009 5465 7874 4c61 6265  ........TextLabe
+0000c7f0: 6c07 0000 0010 5365 6c65 6374 4163 636f  l.....SelectAcco
+0000c800: 756e 7444 6c67 0103 0000 0056 0418 0441  untDlg.....V...A
+0000c810: 043f 043e 043b 044c 0437 043e 0432 0430  .?.>.;.L.7.>.2.0
+0000c820: 0442 044c 0020 044d 0442 043e 0442 0020  .B.L. .M.B.>.B. 
+0000c830: 0436 0435 0020 0441 0447 0451 0442 0020  .6.5. .A.G.Q.B. 
+0000c840: 0434 043b 044f 0020 0434 0430 043d 043d  .4.;.O. .4.0.=.=
+0000c850: 043e 0439 0020 0432 0430 043b 044e 0442  .>.9. .2.0.;.N.B
+0000c860: 044b 0800 0000 0006 0000 0027 5573 6520  .K.........'Use 
+0000c870: 7468 6520 7361 6d65 2061 6363 6f75 6e74  the same account
+0000c880: 2066 6f72 2067 6976 656e 2063 7572 7265   for given curre
+0000c890: 6e63 7907 0000 0010 5365 6c65 6374 4163  ncy.....SelectAc
+0000c8a0: 636f 756e 7444 6c67 0103 0000 0024 0412  countDlg.....$..
+0000c8b0: 044b 0431 0435 0440 0438 0442 0435 0020  .K.1.5.@.8.B.5. 
+0000c8c0: 043a 0430 0442 0435 0433 043e 0440 0438  .:.0.B.5.3.>.@.8
+0000c8d0: 044e 0800 0000 0006 0000 0016 506c 6561  .N..........Plea
+0000c8e0: 7365 2073 656c 6563 7420 6361 7465 676f  se select catego
+0000c8f0: 7279 0700 0000 1453 656c 6563 7443 6174  ry.....SelectCat
+0000c900: 6567 6f72 7944 6961 6c6f 6701 0300 0000  egoryDialog.....
+0000c910: 2804 1204 4b04 3104 3504 4004 3804 4204  (...K.1.5.@.8.B.
+0000c920: 3500 2004 3a04 3e04 3d04 4204 4004 3004  5. .:.>.=.B.@.0.
+0000c930: 3304 3504 3d04 4204 3008 0000 0000 0600  3.5.=.B.0.......
+0000c940: 0000 1250 6c65 6173 6520 7365 6c65 6374  ...Please select
+0000c950: 2070 6565 7207 0000 0010 5365 6c65 6374   peer.....Select
+0000c960: 5065 6572 4469 616c 6f67 0103 0000 0022  PeerDialog....."
+0000c970: 041d 0438 0447 0435 0433 043e 0020 043d  ...8.G.5.3.>. .=
+0000c980: 0435 0020 0432 044b 0431 0440 0430 043d  .5. .2.K.1.@.0.=
+0000c990: 043e 0800 0000 0006 0000 000c 4e6f 2073  .>..........No s
+0000c9a0: 656c 6563 7469 6f6e 0700 0000 1553 656c  election.....Sel
+0000c9b0: 6563 7452 6566 6572 656e 6365 4469 616c  ectReferenceDial
+0000c9c0: 6f67 0103 0000 002e 0412 044b 0020 0434  og.........K. .4
+0000c9d0: 043e 043b 0436 043d 044b 0020 0441 0434  .>.;.6.=.K. .A.4
+0000c9e0: 0435 043b 0430 0442 044c 0020 0432 044b  .5.;.0.B.L. .2.K
+0000c9f0: 0431 043e 0440 0800 0000 0006 0000 001b  .1.>.@..........
+0000ca00: 596f 7520 7368 6f75 6c64 2073 656c 6563  You should selec
+0000ca10: 7420 736f 6d65 7468 696e 6707 0000 0015  t something.....
+0000ca20: 5365 6c65 6374 5265 6665 7265 6e63 6544  SelectReferenceD
+0000ca30: 6961 6c6f 6701 0300 0000 1c04 1204 4b04  ialog.........K.
+0000ca40: 3104 3504 4004 3804 4204 3500 2004 3c04  1.5.@.8.B.5. .<.
+0000ca50: 3504 4204 3a04 4308 0000 0000 0600 0000  5.B.:.C.........
+0000ca60: 1150 6c65 6173 6520 7365 6c65 6374 2074  .Please select t
+0000ca70: 6167 0700 0000 0f53 656c 6563 7454 6167  ag.....SelectTag
+0000ca80: 4469 616c 6f67 0103 0000 005a 041d 0435  Dialog.....Z...5
+0000ca90: 0020 0443 0434 0430 043b 043e 0441 044c  . .C.4.0.;.>.A.L
+0000caa0: 0020 043f 043e 043b 0443 0447 0438 0442  . .?.>.;.C.G.8.B
+0000cab0: 044c 0020 043d 0430 0437 0432 0430 043d  .L. .=.0.7.2.0.=
+0000cac0: 0438 0435 0020 043e 0433 0440 0430 043d  .8.5. .>.3.@.0.=
+0000cad0: 0438 0437 0430 0446 0438 0438 0020 0438  .8.7.0.F.8.8. .8
+0000cae0: 0437 003a 0020 0800 0000 0006 0000 001d  .7.:. ..........
+0000caf0: 4361 6e27 7420 6765 7420 636f 6d70 616e  Can't get compan
+0000cb00: 7920 6e61 6d65 2066 726f 6d3a 2007 0000  y name from: ...
+0000cb10: 000b 536c 6970 7354 6178 4150 4901 0300  ..SlipsTaxAPI...
+0000cb20: 0000 4804 1d04 3504 3204 3e04 3704 3c04  ..H...5.2.>.7.<.
+0000cb30: 3e04 3604 3d04 3e00 2004 3e04 3104 3204  >.6.=.>. .>.1.2.
+0000cb40: 3d04 3e04 3204 3804 4204 4c00 2004 4104  =.>.2.8.B.L. .A.
+0000cb50: 3504 4104 4104 3804 4e00 2c00 2004 3e04  5.A.A.8.N.,. .>.
+0000cb60: 4204 3204 3504 4200 3a00 2008 0000 0000  B.2.5.B.:. .....
+0000cb70: 0600 0000 2143 616e 2774 2072 6566 7265  ....!Can't refre
+0000cb80: 7368 2073 6573 7369 6f6e 2c20 7265 7370  sh session, resp
+0000cb90: 6f6e 7365 3a20 0700 0000 0b53 6c69 7073  onse: .....Slips
+0000cba0: 5461 7841 5049 0103 0000 002e 041e 0448  TaxAPI.........H
+0000cbb0: 0438 0431 043a 0430 0020 043f 043e 043b  .8.1.:.0. .?.>.;
+0000cbc0: 0443 0447 0435 043d 0438 044f 0020 0447  .C.G.5.=.8.O. .G
+0000cbd0: 0435 043a 0430 003a 0020 0800 0000 0006  .5.:.0.:. ......
+0000cbe0: 0000 0013 4765 7420 7469 636b 6574 2066  ....Get ticket f
+0000cbf0: 6169 6c65 643a 2007 0000 000b 536c 6970  ailed: .....Slip
+0000cc00: 7354 6178 4150 4901 0300 0000 3404 1e04  sTaxAPI.....4...
+0000cc10: 4804 3804 3104 3a04 3000 2004 3f04 3e04  H.8.1.:.0. .?.>.
+0000cc20: 3b04 4304 4704 3504 3d04 3804 4f00 2000  ;.C.G.5.=.8.O. .
+0000cc30: 6900 6400 2004 4704 3504 3a04 3000 3a00  i.d. .G.5.:.0.:.
+0000cc40: 2008 0000 0000 0600 0000 1647 6574 2074   ..........Get t
+0000cc50: 6963 6b65 7420 6964 2066 6169 6c65 643a  icket id failed:
+0000cc60: 2007 0000 000b 536c 6970 7354 6178 4150   .....SlipsTaxAP
+0000cc70: 4901 0300 0000 7c04 1d04 3504 3204 3504  I.....|...5.2.5.
+0000cc80: 4004 3d04 3004 4f00 2004 3404 3b04 3804  @.=.0.O. .4.;.8.
+0000cc90: 3d04 3000 2004 1804 1d04 1d00 2e00 2004  =.0. ......... .
+0000cca0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
+0000ccb0: 3d04 3e00 2004 3f04 3e04 3b04 4304 4704  =.>. .?.>.;.C.G.
+0000ccc0: 3804 4204 4c00 2004 3d04 3004 3804 3c04  8.B.L. .=.0.8.<.
+0000ccd0: 3504 3d04 3e04 3204 3004 3d04 3804 3500  5.=.>.2.0.=.8.5.
+0000cce0: 2004 3a04 3e04 3c04 3f04 3004 3d04 3804   .:.>.<.?.0.=.8.
+0000ccf0: 3800 2e08 0000 0000 0600 0000 3049 6e63  8...........0Inc
+0000cd00: 6f72 7265 6374 206c 656e 6774 6820 6f66  orrect length of
+0000cd10: 2049 4e4e 2e20 4361 6e27 7420 6765 7420   INN. Can't get 
+0000cd20: 636f 6d70 616e 7920 6e61 6d65 2e07 0000  company name....
+0000cd30: 000b 536c 6970 7354 6178 4150 4901 0300  ..SlipsTaxAPI...
+0000cd40: 0000 5604 1d04 3504 4200 2000 5300 6500  ..V...5.B. .S.e.
+0000cd50: 7300 7300 6900 6f00 6e00 4900 6400 2004  s.s.i.o.n.I.d. .
+0000cd60: 3404 3b04 4f00 2004 3704 3004 3304 4004  4.;.O. .7.0.3.@.
+0000cd70: 4304 3704 3a04 3800 2004 4704 3504 3a04  C.7.:.8. .G.5.:.
+0000cd80: 3000 2004 4100 2004 4104 3004 3904 4204  0. .A. .A.0.9.B.
+0000cd90: 3000 2004 2404 1d04 2108 0000 0000 0600  0. .$...!.......
+0000cda0: 0000 224e 6f20 5275 7373 6961 6e20 5461  .."No Russian Ta
+0000cdb0: 7820 5365 7373 696f 6e49 6420 6176 6169  x SessionId avai
+0000cdc0: 6c61 626c 6507 0000 000b 536c 6970 7354  lable.....SlipsT
+0000cdd0: 6178 4150 4901 0300 0000 3604 1d04 3504  axAPI.....6...5.
+0000cde0: 4200 2004 3004 3a04 4204 3804 3204 3d04  B. .0.:.B.8.2.=.
+0000cdf0: 3e04 3900 2004 4104 3504 4104 4104 3804  >.9. .A.5.A.A.8.
+0000ce00: 3800 2004 3404 3b04 4f00 2004 2404 1d04  8. .4.;.O. .$...
+0000ce10: 2108 0000 0000 0600 0000 184e 6f20 7661  !..........No va
+0000ce20: 6c69 6420 7365 7373 696f 6e20 7072 6573  lid session pres
+0000ce30: 656e 7407 0000 000b 536c 6970 7354 6178  ent.....SlipsTax
+0000ce40: 4150 4901 0300 0000 7a04 1e04 3f04 3504  API.....z...?.5.
+0000ce50: 4004 3004 4604 3804 4f00 2004 3e04 3104  @.0.F.8.O. .>.1.
+0000ce60: 4004 3004 3104 3004 4204 4b04 3204 3004  @.0.1.0.B.K.2.0.
+0000ce70: 3504 4204 4104 4f00 2004 3d04 3000 2004  5.B.A.O. .=.0. .
+0000ce80: 4104 4204 3e04 4004 3e04 3d04 3500 2004  A.B.>.@.>.=.5. .
+0000ce90: 4104 3504 4004 3204 3504 4004 3000 2e00  A.5.@.2.5.@.0...
+0000cea0: 2004 1f04 3e04 3204 4204 3e04 4004 4f04   ...>.2.B.>.@.O.
+0000ceb0: 4e00 2004 3504 4904 5100 2004 4004 3004  N. .5.I.Q. .@.0.
+0000cec0: 3700 2e08 0000 0000 0600 0000 384f 7065  7...........8Ope
+0000ced0: 7261 7469 6f6e 206d 6967 6874 2062 6520  ration might be 
+0000cee0: 7065 6e64 696e 6720 6f6e 2073 6572 7665  pending on serve
+0000cef0: 7220 7369 6465 2e20 5472 7969 6e67 2061  r side. Trying a
+0000cf00: 6761 696e 2e07 0000 000b 536c 6970 7354  gain......SlipsT
+0000cf10: 6178 4150 4901 0300 0000 2804 1e04 3104  axAPI.....(...1.
+0000cf20: 3d04 3e04 3204 3b04 3504 3d04 3804 3500  =.>.2.;.5.=.8.5.
+0000cf30: 2004 4104 3504 4104 4104 3804 3800 2e00   .A.5.A.A.8.8...
+0000cf40: 2e00 2e08 0000 0000 0600 0000 1552 6566  .............Ref
+0000cf50: 7265 7368 696e 6720 7365 7373 696f 6e2e  reshing session.
+0000cf60: 2e2e 0700 0000 0b53 6c69 7073 5461 7841  .......SlipsTaxA
+0000cf70: 5049 0103 0000 0024 0421 0435 0441 0441  PI.....$.!.5.A.A
+0000cf80: 0438 044f 0020 043e 0431 043d 043e 0432  .8.O. .>.1.=.>.2
+0000cf90: 043b 0435 043d 0430 003a 0020 0800 0000  .;.5.=.0.:. ....
+0000cfa0: 0006 0000 0013 5365 7373 696f 6e20 7265  ......Session re
+0000cfb0: 6672 6573 6865 643a 2007 0000 000b 536c  freshed: .....Sl
+0000cfc0: 6970 7354 6178 4150 4901 0300 0000 1804  ipsTaxAPI.......
+0000cfd0: 2704 3504 3a00 2004 3d04 3004 3904 3404  '.5.:. .=.0.9.4.
+0000cfe0: 3504 3d00 3a00 2008 0000 0000 0600 0000  5.=.:. .........
+0000cff0: 0c53 6c69 7020 666f 756e 643a 2007 0000  .Slip found: ...
+0000d000: 000b 536c 6970 7354 6178 4150 4901 0300  ..SlipsTaxAPI...
+0000d010: 0000 1c04 2704 3504 3a00 2004 3704 3004  ....'.5.:. .7.0.
+0000d020: 3304 4004 4304 3604 3504 3d00 3a00 2008  3.@.C.6.5.=.:. .
+0000d030: 0000 0000 0600 0000 0d53 6c69 7020 6c6f  .........Slip lo
+0000d040: 6164 6564 3a20 0700 0000 0b53 6c69 7073  aded: .....Slips
+0000d050: 5461 7841 5049 0103 0000 0036 041d 0435  TaxAPI.....6...5
+0000d060: 0430 0432 0442 043e 0440 0438 0437 043e  .0.2.B.>.@.8.7.>
+0000d070: 0432 0430 043d 043e 0020 043f 043e 0020  .2.0.=.>. .?.>. 
+0000d080: 043f 0440 0438 0447 0438 043d 0435 003a  .?.@.8.G.8.=.5.:
+0000d090: 0020 0800 0000 0006 0000 001a 556e 6175  . ..........Unau
+0000d0a0: 7468 6f72 697a 6564 2077 6974 6820 7265  thorized with re
+0000d0b0: 6173 6f6e 3a20 0700 0000 0b53 6c69 7073  ason: .....Slips
+0000d0c0: 5461 7841 5049 0103 0000 001c 0421 0447  TaxAPI.......!.G
+0000d0d0: 0451 0442 0020 043d 0435 0020 0432 044b  .Q.B. .=.5. .2.K
+0000d0e0: 0431 0440 0430 043d 0800 0000 0006 0000  .1.@.0.=........
+0000d0f0: 0014 4163 636f 756e 7420 6e6f 7420 7365  ..Account not se
+0000d100: 6c65 6374 6564 0700 0000 0953 7461 7465  lected.....State
+0000d110: 6d65 6e74 0103 0000 0034 0414 0430 043d  ment.....4...0.=
+0000d120: 043d 044b 0435 0020 043d 0435 0020 043f  .=.K.5. .=.5. .?
+0000d130: 0440 0438 0432 044f 0437 0430 043d 044b  .@.8.2.O.7.0.=.K
+0000d140: 0020 043a 0020 0426 0411 003a 0020 0800  . .:. .&...:. ..
+0000d150: 0000 0006 0000 0023 4173 7365 7420 6461  .......#Asset da
+0000d160: 7461 2061 7265 6e27 7420 6c69 6e6b 6564  ta aren't linked
+0000d170: 2074 6f20 6173 7365 743a 2007 0000 0009   to asset: .....
+0000d180: 5374 6174 656d 656e 7401 0300 0000 1e04  Statement.......
+0000d190: 2604 1100 2000 6900 6400 2004 3d04 3500  &... .i.d. .=.5.
+0000d1a0: 2004 3d04 3004 3904 3404 3504 3d08 0000   .=.0.9.4.5.=...
+0000d1b0: 0000 0600 0000 1241 7373 6574 2069 6420  .......Asset id 
+0000d1c0: 6e6f 7420 666f 756e 6407 0000 0009 5374  not found.....St
+0000d1d0: 6174 656d 656e 7401 0300 0000 3204 1d04  atement.....2...
+0000d1e0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
+0000d1f0: 3e00 2004 4104 3e04 3704 3404 3004 4204  >. .A.>.7.4.0.B.
+0000d200: 4c00 2004 4104 4704 5104 4200 3a00 2008  L. .A.G.Q.B.:. .
+0000d210: 0000 0000 0600 0000 1643 616e 2774 2063  .........Can't c
+0000d220: 7265 6174 6520 6163 636f 756e 743a 2007  reate account: .
+0000d230: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
+0000d240: 0000 2e04 1d04 3504 3204 3e04 3704 3c04  ......5.2.>.7.<.
+0000d250: 3e04 3604 3d04 3e00 2004 4104 3e04 3704  >.6.=.>. .A.>.7.
+0000d260: 3404 3004 4204 4c00 2004 2604 1100 3a00  4.0.B.L. .&...:.
+0000d270: 2008 0000 0000 0600 0000 1443 616e 2774   ..........Can't
+0000d280: 2063 7265 6174 6520 6173 7365 743a 2007   create asset: .
+0000d290: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
+0000d2a0: 0000 3c04 1d04 3504 3204 3e04 3704 3c04  ..<...5.2.>.7.<.
+0000d2b0: 3e04 3604 3d04 3e00 2004 3d04 3004 3904  >.6.=.>. .=.0.9.
+0000d2c0: 4204 3500 2004 2604 1100 2004 3200 2004  B.5. .&... .2. .
+0000d2d0: 3e04 4204 4704 5104 4204 3500 3a00 2008  >.B.G.Q.B.5.:. .
+0000d2e0: 0000 0000 0600 0000 2643 616e 2774 206c  ........&Can't l
+0000d2f0: 6f63 6174 6520 6173 7365 7420 696e 2073  ocate asset in s
+0000d300: 7461 7465 6d65 6e74 2064 6174 613a 2007  tatement data: .
+0000d310: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
+0000d320: 0000 1a04 1f04 3e04 3404 4204 3204 3504  ......>.4.B.2.5.
+0000d330: 4004 3604 3404 3504 3d04 3804 3508 0000  @.6.4.5.=.8.5...
+0000d340: 0000 0600 0000 0c43 6f6e 6669 726d 6174  .......Confirmat
+0000d350: 696f 6e07 0000 0009 5374 6174 656d 656e  ion.....Statemen
+0000d360: 7401 0300 0000 4404 1e04 4204 3b04 3004  t.....D...B.;.0.
+0000d370: 3404 3e04 4704 3d04 3004 4f00 2004 3804  4.>.G.=.0.O. .8.
+0000d380: 3d04 4404 3e04 4004 3c04 3004 4604 3804  =.D.>.@.<.0.F.8.
+0000d390: 4f00 2004 4104 3e04 4504 4004 3004 3d04  O. .A.>.E.@.0.=.
+0000d3a0: 3504 3d04 3000 2004 3200 2008 0000 0000  5.=.0. .2. .....
+0000d3b0: 0600 0000 1e44 6562 7567 2069 6e66 6f72  .....Debug infor
+0000d3c0: 6d61 7469 6f6e 2069 7320 7361 7665 6420  mation is saved 
+0000d3d0: 696e 2007 0000 0009 5374 6174 656d 656e  in .....Statemen
+0000d3e0: 7401 0300 0000 1004 1404 3504 3f04 3e04  t.........5.?.>.
+0000d3f0: 3704 3804 4200 2008 0000 0000 0600 0000  7.8.B. .........
+0000d400: 0b44 6570 6f73 6974 206f 6620 0700 0000  .Deposit of ....
+0000d410: 0953 7461 7465 6d65 6e74 0103 0000 0048  .Statement.....H
+0000d420: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+0000d430: 043d 043e 0020 043f 0440 043e 0447 0438  .=.>. .?.@.>.G.8
+0000d440: 0442 0430 0442 044c 0020 004a 0053 004f  .B.0.B.L. .J.S.O
+0000d450: 004e 0020 0438 0437 0020 0444 0430 0439  .N. .8.7. .D.0.9
+0000d460: 043b 0430 003a 0020 0800 0000 0006 0000  .;.0.:. ........
+0000d470: 001f 4661 696c 6564 2074 6f20 7265 6164  ..Failed to read
+0000d480: 204a 534f 4e20 6672 6f6d 2066 696c 653a   JSON from file:
+0000d490: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
+0000d4a0: 0300 0000 4804 1d04 3500 2004 4304 3404  ....H...5. .C.4.
+0000d4b0: 3004 3b04 3e04 4104 4c00 2004 3f04 4004  0.;.>.A.L. .?.@.
+0000d4c0: 3e04 4704 3804 4204 3004 4204 4c00 2004  >.G.8.B.0.B.L. .
+0000d4d0: 4104 4504 3504 3c04 4300 2000 4a00 5300  A.E.5.<.C. .J.S.
+0000d4e0: 4f00 4e00 2004 3804 3700 3a00 2008 0000  O.N. .8.7.:. ...
+0000d4f0: 0000 0600 0000 2146 6169 6c65 6420 746f  ......!Failed to
+0000d500: 2072 6561 6420 4a53 4f4e 2073 6368 656d   read JSON schem
+0000d510: 6120 6672 6f6d 3a20 0700 0000 0953 7461  a from: .....Sta
+0000d520: 7465 6d65 6e74 0103 0000 0034 041d 0435  tement.....4...5
+0000d530: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
+0000d540: 0020 043f 0440 043e 0447 0435 0441 0442  . .?.@.>.G.5.A.B
+0000d550: 044c 0020 0444 0430 0439 043b 003a 0020  .L. .D.0.9.;.:. 
+0000d560: 0800 0000 0006 0000 0015 4661 696c 6564  ..........Failed
+0000d570: 2074 6f20 7265 6164 2066 696c 653a 2007   to read file: .
+0000d580: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
+0000d590: 0000 5a04 1e04 4804 3804 3104 3a04 3000  ..Z...H.8.1.:.0.
+0000d5a0: 2004 3f04 4004 3800 2004 4104 3e04 4504   .?.@.8. .A.>.E.
+0000d5b0: 4004 3004 3d04 3504 3d04 3804 3800 2004  @.0.=.5.=.8.8. .
+0000d5c0: 3e04 4204 3b04 3004 3404 3e04 4704 3d04  >.B.;.0.4.>.G.=.
+0000d5d0: 3e04 3900 2004 3804 3d04 4404 3e04 4004  >.9. .8.=.D.>.@.
+0000d5e0: 3c04 3004 4604 3804 3800 3a00 2008 0000  <.0.F.8.8.:. ...
+0000d5f0: 0000 0600 0000 2546 6169 6c65 6420 746f  ......%Failed to
+0000d600: 2077 7269 7465 2073 7461 7465 6d65 6e74   write statement
+0000d610: 2064 756d 7020 696e 746f 3a20 0700 0000   dump into: ....
+0000d620: 0953 7461 7465 6d65 6e74 0103 0000 0066  .Statement.....f
+0000d630: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+0000d640: 043d 043e 0020 043a 043e 043d 0442 0432  .=.>. .:.>.=.B.2
+0000d650: 0435 0440 0442 0438 0440 043e 0432 0430  .5.@.B.8.@.>.2.0
+0000d660: 0442 044c 0020 0442 0438 043f 0020 0430  .B.L. .B.8.?. .0
+0000d670: 043a 0442 0438 0432 0430 0020 0432 0020  .:.B.8.2.0. .2. 
+0000d680: 0442 0440 0430 043d 0441 0444 0435 0440  .B.@.0.=.A.D.5.@
+0000d690: 0435 003a 0020 0800 0000 0006 0000 002e  .5.:. ..........
+0000d6a0: 496d 706f 7373 6962 6c65 2074 6f20 636f  Impossible to co
+0000d6b0: 6e76 6572 7420 6173 7365 7420 7479 7065  nvert asset type
+0000d6c0: 2069 6e20 7472 616e 7366 6572 3a20 0700   in transfer: ..
+0000d6d0: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
+0000d6e0: 0048 041d 0435 043e 0434 043d 043e 0437  .H...5.>.4.=.>.7
+0000d6f0: 043d 0430 0447 043d 043e 0435 0020 0441  .=.0.G.=.>.5. .A
+0000d700: 043e 0432 043f 0430 0434 0435 043d 0438  .>.2.?.0.4.5.=.8
+0000d710: 0435 0020 0432 0430 043b 044e 0442 044b  .5. .2.0.;.N.B.K
+0000d720: 0020 0434 043b 044f 0020 0800 0000 0006  . .4.;.O. ......
+0000d730: 0000 001c 4d75 6c74 6970 6c65 2063 7572  ....Multiple cur
+0000d740: 7265 6e63 7920 6d61 7463 6820 666f 7220  rency match for 
+0000d750: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
+0000d760: 0000 003a 041d 0435 043e 0434 043d 043e  ...:...5.>.4.=.>
+0000d770: 0437 043d 0430 0447 043d 043e 0435 0020  .7.=.0.G.=.>.5. 
+0000d780: 0441 043e 0432 043f 0430 0434 0435 043d  .A.>.2.?.0.4.5.=
+0000d790: 0438 0435 0020 0434 043b 044f 0020 0800  .8.5. .4.;.O. ..
+0000d7a0: 0000 0006 0000 0013 4d75 6c74 6970 6c65  ........Multiple
+0000d7b0: 206d 6174 6368 2066 6f72 2007 0000 0009   match for .....
+0000d7c0: 5374 6174 656d 656e 7401 0300 0000 3a04  Statement.....:.
+0000d7d0: 1204 4b04 3104 3504 4004 3804 4204 3500  ..K.1.5.@.8.B.5.
+0000d7e0: 2004 4104 4704 5104 4200 2004 3404 3b04   .A.G.Q.B. .4.;.
+0000d7f0: 4f00 2004 3704 3004 4704 3804 4104 3b04  O. .7.0.G.8.A.;.
+0000d800: 3504 3d04 3804 4f00 3a08 0000 0000 0600  5.=.8.O.:.......
+0000d810: 0000 1d53 656c 6563 7420 6163 636f 756e  ...Select accoun
+0000d820: 7420 746f 2064 6570 6f73 6974 2074 6f3a  t to deposit to:
+0000d830: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
+0000d840: 0000 0036 0412 044b 0431 0435 0440 0438  ...6...K.1.5.@.8
+0000d850: 0442 0435 0020 0441 0447 0451 0442 0020  .B.5. .A.G.Q.B. 
+0000d860: 0434 043b 044f 0020 0441 043f 0438 0441  .4.;.O. .A.?.8.A
+0000d870: 0430 043d 0438 044f 003a 0800 0000 0006  .0.=.8.O.:......
+0000d880: 0000 0020 5365 6c65 6374 2061 6363 6f75  ... Select accou
+0000d890: 6e74 2074 6f20 7769 7468 6472 6177 2066  nt to withdraw f
+0000d8a0: 726f 6d3a 0700 0000 0953 7461 7465 6d65  rom:.....Stateme
+0000d8b0: 6e74 0103 0000 0048 041d 0435 043a 043e  nt.....H...5.:.>
+0000d8c0: 0442 043e 0440 044b 0435 0020 0441 0435  .B.>.@.K.5. .A.5
+0000d8d0: 043a 0446 0438 0438 0020 043d 0435 0020  .:.F.8.8. .=.5. 
+0000d8e0: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
+0000d8f0: 0432 0430 044e 0442 0441 044f 003a 0020  .2.0.N.B.A.O.:. 
+0000d900: 0800 0000 0006 0000 0021 536f 6d65 2073  .........!Some s
+0000d910: 6563 7469 6f6e 7320 6172 6520 6e6f 7420  ections are not 
+0000d920: 7375 7070 6f72 7465 643a 2007 0000 0009  supported: .....
+0000d930: 5374 6174 656d 656e 7401 0300 0000 2a04  Statement.....*.
+0000d940: 1804 3c04 3f04 3e04 4004 4200 2004 3e04  ..<.?.>.@.B. .>.
+0000d950: 4204 4704 5104 4204 3000 2004 3f04 4004  B.G.Q.B.0. .?.@.
+0000d960: 3504 4004 3204 3004 3d08 0000 0000 0600  5.@.2.0.=.......
+0000d970: 0000 1e53 7461 7465 6d65 6e74 2069 6d70  ...Statement imp
+0000d980: 6f72 7420 7761 7320 6361 6e63 656c 6c65  ort was cancelle
+0000d990: 6407 0000 0009 5374 6174 656d 656e 7401  d.....Statement.
+0000d9a0: 0300 0000 2c04 1d04 3504 3204 3504 4004  ....,...5.2.5.@.
+0000d9b0: 3d04 4b04 3900 2004 3f04 3504 4004 3804  =.K.9. .?.5.@.8.
+0000d9c0: 3e04 3400 2004 3e04 4204 4704 5104 4204  >.4. .>.B.G.Q.B.
+0000d9d0: 3008 0000 0000 0600 0000 1b53 7461 7465  0..........State
+0000d9e0: 6d65 6e74 2070 6572 696f 6420 6973 2069  ment period is i
+0000d9f0: 6e76 616c 6964 0700 0000 0953 7461 7465  nvalid.....State
+0000da00: 6d65 6e74 0103 0000 00c6 041f 0435 0440  ment.........5.@
+0000da10: 0438 043e 0434 0020 043e 0442 0447 0451  .8.>.4. .>.B.G.Q
+0000da20: 0442 0430 0020 043d 0430 0447 0438 043d  .B.0. .=.0.G.8.=
+0000da30: 0430 0435 0442 0441 044f 0020 0440 0430  .0.5.B.A.O. .@.0
+0000da40: 043d 0435 0435 0020 043f 043e 0441 043b  .=.5.5. .?.>.A.;
+0000da50: 0435 0434 043d 0435 0439 0020 043e 043f  .5.4.=.5.9. .>.?
+0000da60: 0435 0440 0430 0446 0438 0438 0020 0434  .5.@.0.F.8.8. .4
+0000da70: 043b 044f 0020 0441 0447 0451 0442 0430  .;.O. .A.G.Q.B.0
+0000da80: 0020 0028 043f 043e 0432 0442 043e 0440  . .(.?.>.2.B.>.@
+0000da90: 043d 044b 0439 0020 0438 043c 043f 043e  .=.K.9. .8.<.?.>
+0000daa0: 0440 0442 003f 0029 002e 0020 041f 0440  .@.B.?.)... ...@
+0000dab0: 043e 0434 043e 043b 0436 0438 0442 044c  .>.4.>.;.6.8.B.L
+0000dac0: 0020 0438 043c 043f 043e 0440 0442 003f  . .8.<.?.>.@.B.?
+0000dad0: 0800 0000 0006 0000 0058 5374 6174 656d  .........XStatem
+0000dae0: 656e 7420 7065 7269 6f64 2073 7461 7274  ent period start
+0000daf0: 7320 6265 666f 7265 206c 6173 7420 7265  s before last re
+0000db00: 636f 7264 6564 206f 7065 7261 7469 6f6e  corded operation
+0000db10: 2066 6f72 2074 6865 2061 6363 6f75 6e74   for the account
+0000db20: 2e20 436f 6e74 696e 7565 2069 6d70 6f72  . Continue impor
+0000db30: 743f 0700 0000 0953 7461 7465 6d65 6e74  t?.....Statement
+0000db40: 0103 0000 002a 041e 0442 0447 0451 0442  .....*...B.G.Q.B
+0000db50: 0020 0441 043e 0434 0435 0440 0436 0438  . .A.>.4.5.@.6.8
+0000db60: 0442 0020 043e 0448 0438 0431 043a 0438  .B. .>.H.8.1.:.8
+0000db70: 0800 0000 0006 0000 001b 5374 6174 656d  ..........Statem
+0000db80: 656e 7420 7661 6c69 6461 7469 6f6e 2066  ent validation f
+0000db90: 6169 6c65 6407 0000 0009 5374 6174 656d  ailed.....Statem
+0000dba0: 656e 7401 0300 0000 4004 2104 3804 3c04  ent.....@.!.8.<.
+0000dbb0: 3204 3e04 3b00 2004 3204 3004 3b04 4e04  2.>.;. .2.0.;.N.
+0000dbc0: 4204 4b00 2004 3d04 3500 2004 3f04 4004  B.K. .=.5. .?.@.
+0000dbd0: 3804 3204 4f04 3704 3004 3d00 2004 3a00  8.2.O.7.0.=. .:.
+0000dbe0: 2004 2604 1100 3a00 2008 0000 0000 0600   .&...:. .......
+0000dbf0: 0000 2753 796d 626f 6c20 6375 7272 656e  ..'Symbol curren
+0000dc00: 6379 2069 736e 2774 206c 696e 6b65 6420  cy isn't linked 
+0000dc10: 746f 2061 7373 6574 3a20 0700 0000 0953  to asset: .....S
+0000dc20: 7461 7465 6d65 6e74 0103 0000 0032 0421  tatement.....2.!
+0000dc30: 0438 043c 0432 043e 043b 0020 043d 0435  .8.<.2.>.;. .=.5
+0000dc40: 0020 043f 0440 0438 0432 044f 0437 0430  . .?.@.8.2.O.7.0
+0000dc50: 043d 0020 043a 0020 0426 0411 003a 0020  .=. .:. .&...:. 
+0000dc60: 0800 0000 0006 0000 0025 5379 6d62 6f6c  .........%Symbol
+0000dc70: 2074 6963 6b65 7220 6973 6e27 7420 6c69   ticker isn't li
+0000dc80: 6e6b 6564 2074 6f20 6173 7365 743a 2007  nked to asset: .
+0000dc90: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
+0000dca0: 0000 7204 1d04 3504 3204 3e04 3704 3c04  ..r...5.2.>.7.<.
+0000dcb0: 3e04 3604 3d04 3e00 2004 4104 3e04 3f04  >.6.=.>. .A.>.?.
+0000dcc0: 3e04 4104 4204 3004 3204 3804 4204 4c00  >.A.B.0.2.8.B.L.
+0000dcd0: 2004 4104 4704 5104 4200 2004 3404 3b04   .A.G.Q.B. .4.;.
+0000dce0: 4f00 2004 3a04 3e04 4004 3f04 3e04 4004  O. .:.>.@.?.>.@.
+0000dcf0: 3004 4204 3804 3204 3d04 3e04 3304 3e00  0.B.8.2.=.>.3.>.
+0000dd00: 2004 3404 3504 3904 4104 4204 3204 3804   .4.5.9.A.B.2.8.
+0000dd10: 4f00 3a00 2008 0000 0000 0600 0000 2855  O.:. .........(U
+0000dd20: 6e6d 6174 6368 6564 2061 6363 6f75 6e74  nmatched account
+0000dd30: 2066 6f72 2063 6f72 706f 7261 7465 2061   for corporate a
+0000dd40: 6374 696f 6e3a 2007 0000 0009 5374 6174  ction: .....Stat
+0000dd50: 656d 656e 7401 0300 0000 7404 1d04 3504  ement.....t...5.
+0000dd60: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
+0000dd70: 2004 4104 3e04 3f04 3e04 4104 4204 3004   .A.>.?.>.A.B.0.
+0000dd80: 3204 3804 4204 4c00 2004 4104 4704 5104  2.8.B.L. .A.G.Q.
+0000dd90: 4200 2004 3404 3b04 4f00 2004 3e04 3f04  B. .4.;.O. .>.?.
+0000dda0: 3504 4004 3004 4604 3804 3800 2004 3f04  5.@.0.F.8.8. .?.
+0000ddb0: 4004 3804 4504 3e04 3404 3000 2f04 4004  @.8.E.>.4.0./.@.
+0000ddc0: 3004 4104 4504 3e04 3404 3000 3a00 2008  0.A.E.>.4.0.:. .
+0000ddd0: 0000 0000 0600 0000 2755 6e6d 6174 6368  ........'Unmatch
+0000dde0: 6564 2061 6363 6f75 6e74 2066 6f72 2069  ed account for i
+0000ddf0: 6e63 6f6d 652f 7370 656e 6469 6e67 3a20  ncome/spending: 
+0000de00: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
+0000de10: 0000 0052 041d 0435 0432 043e 0437 043c  ...R...5.2.>.7.<
+0000de20: 043e 0436 043d 043e 0020 0441 043e 043f  .>.6.=.>. .A.>.?
+0000de30: 043e 0441 0442 0430 0432 0438 0442 044c  .>.A.B.0.2.8.B.L
+0000de40: 0020 0441 0447 0451 0442 0020 0434 043b  . .A.G.Q.B. .4.;
+0000de50: 044f 0020 0432 044b 043f 043b 0430 0442  .O. .2.K.?.;.0.B
+0000de60: 044b 003a 0020 0800 0000 0006 0000 001f  .K.:. ..........
+0000de70: 556e 6d61 7463 6865 6420 6163 636f 756e  Unmatched accoun
+0000de80: 7420 666f 7220 7061 796d 656e 743a 2007  t for payment: .
+0000de90: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
+0000dea0: 0000 5004 1d04 3504 3204 3e04 3704 3c04  ..P...5.2.>.7.<.
+0000deb0: 3e04 3604 3d04 3e00 2004 4104 3e04 3f04  >.6.=.>. .A.>.?.
+0000dec0: 3e04 4104 4204 3004 3204 3804 4204 4c00  >.A.B.0.2.8.B.L.
+0000ded0: 2004 4104 4704 5104 4200 2004 3404 3b04   .A.G.Q.B. .4.;.
+0000dee0: 4f00 2004 4104 3404 3504 3b04 3a04 3800  O. .A.4.5.;.:.8.
+0000def0: 3a00 2008 0000 0000 0600 0000 1d55 6e6d  :. ..........Unm
+0000df00: 6174 6368 6564 2061 6363 6f75 6e74 2066  atched account f
+0000df10: 6f72 2074 7261 6465 3a20 0700 0000 0953  or trade: .....S
+0000df20: 7461 7465 6d65 6e74 0103 0000 0054 041d  tatement.....T..
+0000df30: 0435 0432 0437 043e 043c 043e 0436 043d  .5.2.7.>.<.>.6.=
+0000df40: 043e 0020 0441 043e 043f 043e 0441 0442  .>. .A.>.?.>.A.B
+0000df50: 0430 0432 0438 0442 044c 0020 0441 0447  .0.2.8.B.L. .A.G
+0000df60: 0451 0442 0020 0434 043b 044f 0020 043f  .Q.B. .4.;.O. .?
+0000df70: 0435 0440 0435 0432 043e 0434 0430 003a  .5.@.5.2.>.4.0.:
+0000df80: 0020 0800 0000 0006 0000 0020 556e 6d61  . ......... Unma
+0000df90: 7463 6865 6420 6163 636f 756e 7420 666f  tched account fo
+0000dfa0: 7220 7472 616e 7366 6572 3a20 0700 0000  r transfer: ....
+0000dfb0: 0953 7461 7465 6d65 6e74 0103 0000 006e  .Statement.....n
+0000dfc0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+0000dfd0: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
+0000dfe0: 0442 0430 0432 0438 0442 044c 0020 0426  .B.0.2.8.B.L. .&
+0000dff0: 0411 0020 0434 043b 044f 0020 043a 043e  ... .4.;.O. .:.>
+0000e000: 0440 043f 043e 0440 0430 0442 0438 0432  .@.?.>.@.0.B.8.2
+0000e010: 043d 043e 0433 043e 0020 0434 0435 0439  .=.>.3.>. .4.5.9
+0000e020: 0441 0442 0432 0438 044f 003a 0020 0800  .A.B.2.8.O.:. ..
+0000e030: 0000 0006 0000 0026 556e 6d61 7463 6865  .......&Unmatche
+0000e040: 6420 6173 7365 7420 666f 7220 636f 7270  d asset for corp
+0000e050: 6f72 6174 6520 6163 7469 6f6e 3a20 0700  orate action: ..
+0000e060: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
+0000e070: 004e 041d 0435 0432 043e 0437 043c 043e  .N...5.2.>.7.<.>
+0000e080: 0436 043d 043e 0020 0441 043e 043f 043e  .6.=.>. .A.>.?.>
+0000e090: 0441 0442 0430 0432 0438 0442 044c 0020  .A.B.0.2.8.B.L. 
+0000e0a0: 0426 0411 0020 0434 043b 044f 0020 0432  .&... .4.;.O. .2
+0000e0b0: 044b 043f 043b 0430 0442 044b 003a 0020  .K.?.;.0.B.K.:. 
+0000e0c0: 0800 0000 0006 0000 001d 556e 6d61 7463  ..........Unmatc
+0000e0d0: 6865 6420 6173 7365 7420 666f 7220 7061  hed asset for pa
+0000e0e0: 796d 656e 743a 2007 0000 0009 5374 6174  yment: .....Stat
+0000e0f0: 656d 656e 7401 0300 0000 4c04 1d04 3504  ement.....L...5.
+0000e100: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
+0000e110: 2004 4104 3e04 3f04 3e04 4104 4204 3004   .A.>.?.>.A.B.0.
+0000e120: 3204 3804 4204 4c00 2004 2604 1100 2004  2.8.B.L. .&... .
+0000e130: 3404 3b04 4f00 2004 4104 3404 3504 3b04  4.;.O. .A.4.5.;.
+0000e140: 3a04 3800 3a00 2008 0000 0000 0600 0000  :.8.:. .........
+0000e150: 1b55 6e6d 6174 6368 6564 2061 7373 6574  .Unmatched asset
+0000e160: 2066 6f72 2074 7261 6465 3a20 0700 0000   for trade: ....
+0000e170: 0953 7461 7465 6d65 6e74 0103 0000 005e  .Statement.....^
+0000e180: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+0000e190: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
+0000e1a0: 0442 0430 0432 0438 0442 044c 0020 0426  .B.0.2.8.B.L. .&
+0000e1b0: 0411 002f 0432 0430 043b 044e 0442 0443  .../.2.0.;.N.B.C
+0000e1c0: 0020 0434 043b 044f 0020 043f 0435 0440  . .4.;.O. .?.5.@
+0000e1d0: 0435 0432 043e 0434 0430 003a 0020 0800  .5.2.>.4.0.:. ..
+0000e1e0: 0000 0006 0000 001e 556e 6d61 7463 6865  ........Unmatche
+0000e1f0: 6420 6173 7365 7420 666f 7220 7472 616e  d asset for tran
+0000e200: 7366 6572 3a20 0700 0000 0953 7461 7465  sfer: .....State
+0000e210: 6d65 6e74 0103 0000 006c 041d 0435 0432  ment.....l...5.2
+0000e220: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+0000e230: 0441 043e 043f 043e 0441 0442 0430 0432  .A.>.?.>.A.B.0.2
+0000e240: 0438 0442 044c 0020 043a 0430 0442 0435  .8.B.L. .:.0.B.5
+0000e250: 0433 043e 0440 0438 044e 0020 0434 043b  .3.>.@.8.N. .4.;
+0000e260: 044f 0020 043f 0440 0438 0445 043e 0434  .O. .?.@.8.E.>.4
+0000e270: 0430 002f 0440 0430 0441 0445 043e 0434  .0./.@.0.A.E.>.4
+0000e280: 0430 003a 0020 0800 0000 0006 0000 0028  .0.:. .........(
+0000e290: 556e 6d61 7463 6865 6420 6361 7465 676f  Unmatched catego
+0000e2a0: 7279 2066 6f72 2069 6e63 6f6d 652f 7370  ry for income/sp
+0000e2b0: 656e 6469 6e67 3a20 0700 0000 0953 7461  ending: .....Sta
+0000e2c0: 7465 6d65 6e74 0103 0000 0050 041d 0435  tement.....P...5
+0000e2d0: 0432 043e 0437 043c 043e 043d 043e 0020  .2.>.7.<.>.=.>. 
+0000e2e0: 0441 043e 043f 043e 0441 0442 0430 0432  .A.>.?.>.A.B.0.2
+0000e2f0: 0438 0442 044c 0020 0432 0430 043b 044e  .8.B.L. .2.0.;.N
+0000e300: 0442 0443 0020 0434 043b 044f 0020 0441  .B.C. .4.;.O. .A
+0000e310: 0447 0451 0442 0430 003a 0020 0800 0000  .G.Q.B.0.:. ....
+0000e320: 0006 0000 0020 556e 6d61 7463 6865 6420  ..... Unmatched 
+0000e330: 6375 7272 656e 6379 2066 6f72 2061 6363  currency for acc
+0000e340: 6f75 6e74 3a20 0700 0000 0953 7461 7465  ount: .....State
+0000e350: 6d65 6e74 0103 0000 0082 041d 0435 0432  ment.........5.2
+0000e360: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+0000e370: 0441 043e 043f 043e 0441 0442 0430 0432  .A.>.?.>.A.B.0.2
+0000e380: 0438 0442 044c 0020 043a 043e 043d 0442  .8.B.L. .:.>.=.B
+0000e390: 0440 0430 0433 0435 043d 0442 0430 0020  .@.0.3.5.=.B.0. 
+0000e3a0: 0434 043b 044f 0020 043e 043f 0435 0440  .4.;.O. .>.?.5.@
+0000e3b0: 0430 0446 0438 0438 0020 043f 0440 0438  .0.F.8.8. .?.@.8
+0000e3c0: 0445 043e 0434 0430 002f 0440 0430 0441  .E.>.4.0./.@.0.A
+0000e3d0: 0445 043e 0434 0430 003a 0020 0800 0000  .E.>.4.0.:. ....
+0000e3e0: 0006 0000 0024 556e 6d61 7463 6865 6420  .....$Unmatched 
+0000e3f0: 7065 6572 2066 6f72 2069 6e63 6f6d 652f  peer for income/
+0000e400: 7370 656e 6469 6e67 3a20 0700 0000 0953  spending: .....S
+0000e410: 7461 7465 6d65 6e74 0103 0000 0052 041d  tatement.....R..
+0000e420: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
+0000e430: 0438 0432 0430 0435 043c 043e 0435 0020  .8.2.0.5.<.>.5. 
+0000e440: 043a 043e 0440 043f 043e 0440 0430 0442  .:.>.@.?.>.@.0.B
+0000e450: 0438 0432 043d 043e 0435 0020 0434 0435  .8.2.=.>.5. .4.5
+0000e460: 0439 0441 0442 0432 0438 0435 003a 0020  .9.A.B.2.8.5.:. 
+0000e470: 0800 0000 0006 0000 001e 556e 7375 7070  ..........Unsupp
+0000e480: 6f72 7465 6420 636f 7270 6f72 6174 6520  orted corporate 
+0000e490: 6163 7469 6f6e 3a20 0700 0000 0953 7461  action: .....Sta
+0000e4a0: 7465 6d65 6e74 0103 0000 003c 041d 0435  tement.....<...5
+0000e4b0: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
+0000e4c0: 0432 0430 0435 043c 044b 0439 0020 0442  .2.0.5.<.K.9. .B
+0000e4d0: 0438 043f 0020 0432 044b 043f 043b 0430  .8.?. .2.K.?.;.0
+0000e4e0: 0442 044b 003a 0020 0800 0000 0006 0000  .B.K.:. ........
+0000e4f0: 001a 556e 7375 7070 6f72 7465 6420 7061  ..Unsupported pa
+0000e500: 796d 656e 7420 7479 7065 3a20 0700 0000  yment type: ....
+0000e510: 0953 7461 7465 6d65 6e74 0103 0000 0012  .Statement......
+0000e520: 0421 043f 0438 0441 0430 043d 0438 0435  .!.?.8.A.0.=.8.5
+0000e530: 0020 0800 0000 0006 0000 000e 5769 7468  . ..........With
+0000e540: 6472 6177 616c 206f 6620 0700 0000 0953  drawal of .....S
+0000e550: 7461 7465 6d65 6e74 0103 0000 0044 002a  tatement.....D.*
+0000e560: 002a 002a 0020 041d 0415 041e 0411 0425  .*.*. .........%
+0000e570: 041e 0414 0418 041c 0410 0020 0420 0423  ........... . .#
+0000e580: 0427 041d 0410 042f 0020 041f 0420 041e  .'...../. ... ..
+0000e590: 0412 0415 0420 041a 0410 0020 002a 002a  ..... ..... .*.*
+0000e5a0: 002a 0800 0000 0006 0000 001d 2a2a 2a20  .*..........*** 
+0000e5b0: 4d41 4e55 414c 2045 4e54 5259 2052 4551  MANUAL ENTRY REQ
+0000e5c0: 5549 5245 4420 2a2a 2a07 0000 000d 5374  UIRED ***.....St
+0000e5d0: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
+0000e5e0: 3404 2204 3804 3f00 2004 2604 1100 2004  4.".8.?. .&... .
+0000e5f0: 3d04 3500 2004 3f04 3e04 3404 3404 3504  =.5. .?.>.4.4.5.
+0000e600: 4004 3604 3804 3204 3004 3504 4204 4104  @.6.8.2.0.5.B.A.
+0000e610: 4f00 3a00 2008 0000 0000 0600 0000 1c41  O.:. ..........A
+0000e620: 7373 6574 2074 7970 6520 6973 6e27 7420  sset type isn't 
+0000e630: 7375 7070 6f72 7465 643a 2007 0000 000d  supported: .....
+0000e640: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
+0000e650: 0000 4804 1d04 3504 3204 3e04 3704 3c04  ..H...5.2.>.7.<.
+0000e660: 3e04 3604 3d04 3e00 2004 3d04 3004 3904  >.6.=.>. .=.0.9.
+0000e670: 4204 3800 2004 3f04 3b04 3004 4204 5104  B.8. .?.;.0.B.Q.
+0000e680: 3600 2004 3404 3b04 4f00 2004 3e04 4204  6. .4.;.O. .>.B.
+0000e690: 3c04 3504 3d04 4b00 3a00 2008 0000 0000  <.5.=.K.:. .....
+0000e6a0: 0600 0000 1f43 616e 2774 2066 696e 6420  .....Can't find 
+0000e6b0: 6d61 7463 6820 666f 7220 7265 7665 7273  match for revers
+0000e6c0: 616c 3a20 0700 0000 0d53 7461 7465 6d65  al: .....Stateme
+0000e6d0: 6e74 4942 4b52 0103 0000 0046 041d 0435  ntIBKR.....F...5
+0000e6e0: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
+0000e6f0: 0020 043d 0430 0439 0442 0438 0020 043f  . .=.0.9.B.8. .?
+0000e700: 0430 0440 043d 0443 044e 0020 0437 0430  .0.@.=.C.N. .7.0
+0000e710: 043f 0438 0441 044c 0020 0434 043b 044f  .?.8.A.L. .4.;.O
+0000e720: 0020 0800 0000 0006 0000 001d 4361 6e27  . ..........Can'
+0000e730: 7420 6669 6e64 2070 6169 7265 6420 7265  t find paired re
+0000e740: 636f 7264 2066 6f72 2007 0000 000d 5374  cord for .....St
+0000e750: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
+0000e760: 4e04 1d04 3504 3204 3e04 3c04 3e04 3604  N...5.2.>.<.>.6.
+0000e770: 3d04 3e00 2004 3e04 3f04 4004 3504 3404  =.>. .>.?.@.5.4.
+0000e780: 3504 3b04 3804 4204 4c00 2004 3204 3004  5.;.8.B.L. .2.0.
+0000e790: 3b04 4e04 4204 4300 2004 3404 3b04 4f00  ;.N.B.C. .4.;.O.
+0000e7a0: 2004 4104 4704 5104 4204 3000 3a00 2008   .A.G.Q.B.0.:. .
+0000e7b0: 0000 0000 0600 0000 2843 616e 2774 2067  ........(Can't g
+0000e7c0: 6574 2061 6363 6f75 6e74 2063 7572 7265  et account curre
+0000e7d0: 6e63 7920 666f 7220 6163 636f 756e 743a  ncy for account:
+0000e7e0: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
+0000e7f0: 424b 5201 0300 0000 7004 1d04 3504 3204  BKR.....p...5.2.
+0000e800: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
+0000e810: 3e04 3f04 4004 3504 3404 3504 3b04 3804  >.?.@.5.4.5.;.8.
+0000e820: 4204 4c00 2004 3204 3004 3b04 4e04 4204  B.L. .2.0.;.N.B.
+0000e830: 4b00 2004 3404 3b04 4f00 2004 3e04 3f04  K. .4.;.O. .>.?.
+0000e840: 3504 4004 3004 4604 3804 3800 2004 3e04  5.@.0.F.8.8. .>.
+0000e850: 3104 3c04 3504 3d04 3000 2004 3204 3004  1.<.5.=.0. .2.0.
+0000e860: 3b04 4e04 4200 3a00 2008 0000 0000 0600  ;.N.B.:. .......
+0000e870: 0000 2c43 616e 2774 2067 6574 2063 7572  ..,Can't get cur
+0000e880: 7265 6e63 6965 7320 666f 7220 6375 7272  rencies for curr
+0000e890: 656e 6379 2065 7863 6861 6e67 653a 2007  ency exchange: .
+0000e8a0: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000e8b0: 5201 0300 0000 6804 1d04 3504 3204 3e04  R.....h...5.2.>.
+0000e8c0: 3704 3c04 3e04 3604 3d04 3e00 2004 4004  7.<.>.6.=.>. .@.
+0000e8d0: 3004 4104 3f04 3e04 3704 3d04 3004 4204  0.A.?.>.7.=.0.B.
+0000e8e0: 4c00 2004 3e04 3f04 3804 4104 3004 3d04  L. .>.?.8.A.0.=.
+0000e8f0: 3804 3500 2004 1e04 3104 4a04 3504 3404  8.5. ...1.J.5.4.
+0000e900: 3804 3d04 3504 3d04 3804 4f00 2004 3a04  8.=.5.=.8.O. .:.
+0000e910: 3e04 3c04 3f04 3004 3d04 3804 3900 2008  >.<.?.0.=.8.9. .
+0000e920: 0000 0000 0600 0000 1f43 616e 2774 2070  .........Can't p
+0000e930: 6172 7365 204d 6572 6765 7220 6465 7363  arse Merger desc
+0000e940: 7269 7074 696f 6e20 0700 0000 0d53 7461  ription .....Sta
+0000e950: 7465 6d65 6e74 4942 4b52 0103 0000 0064  tementIBKR.....d
+0000e960: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+0000e970: 043d 043e 0020 0440 0430 0441 043f 043e  .=.>. .@.0.A.?.>
+0000e980: 0437 043d 0430 0442 044c 0020 043e 043f  .7.=.0.B.L. .>.?
+0000e990: 0438 0441 0430 043d 0438 0435 0020 0412  .8.A.0.=.8.5. ..
+0000e9a0: 044b 0434 0435 043b 0435 043d 0438 044f  .K.4.5.;.5.=.8.O
+0000e9b0: 0020 043a 043e 043c 043f 0430 043d 0438  . .:.>.<.?.0.=.8
+0000e9c0: 0438 0020 0800 0000 0006 0000 0021 4361  .8. .........!Ca
+0000e9d0: 6e27 7420 7061 7273 6520 5370 696e 2d6f  n't parse Spin-o
+0000e9e0: 6666 2064 6573 6372 6970 7469 6f6e 2007  ff description .
+0000e9f0: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000ea00: 5201 0300 0000 4c04 1d04 3504 3204 3e04  R.....L...5.2.>.
+0000ea10: 3704 3c04 3e04 3604 3d04 3e00 2004 4004  7.<.>.6.=.>. .@.
+0000ea20: 3004 4104 3f04 3e04 3704 3d04 3004 4204  0.A.?.>.7.=.0.B.
+0000ea30: 4c00 2004 3e04 3f04 3804 4104 3004 3d04  L. .>.?.8.A.0.=.
+0000ea40: 3804 3500 2004 2104 3f04 3b04 3804 4204  8.5. .!.?.;.8.B.
+0000ea50: 3000 2008 0000 0000 0600 0000 1e43 616e  0. ..........Can
+0000ea60: 2774 2070 6172 7365 2053 706c 6974 2064  't parse Split d
+0000ea70: 6573 6372 6970 7469 6f6e 2007 0000 000d  escription .....
+0000ea80: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
+0000ea90: 0000 6204 1d04 3504 3204 3e04 3704 3c04  ..b...5.2.>.7.<.
+0000eaa0: 3e04 3604 3d04 3e00 2004 4004 3004 4104  >.6.=.>. .@.0.A.
+0000eab0: 3f04 3e04 3704 3d04 3004 4204 4c00 2004  ?.>.7.=.0.B.L. .
+0000eac0: 3e04 3f04 3804 4104 3004 3d04 3804 3500  >.?.8.A.0.=.8.5.
+0000ead0: 2004 1404 3804 3204 3804 3404 3504 3d04   ...8.2.8.4.5.=.
+0000eae0: 3404 3000 2004 3004 3a04 4604 3804 4f04  4.0. .0.:.F.8.O.
+0000eaf0: 3c04 3800 2008 0000 0000 0600 0000 2743  <.8. .........'C
+0000eb00: 616e 2774 2070 6172 7365 2053 746f 636b  an't parse Stock
+0000eb10: 2044 6976 6964 656e 6420 6465 7363 7269   Dividend descri
+0000eb20: 7074 696f 6e20 0700 0000 0d53 7461 7465  ption .....State
+0000eb30: 6d65 6e74 4942 4b52 0103 0000 005a 041d  mentIBKR.....Z..
+0000eb40: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
+0000eb50: 043e 0020 0440 0430 0441 043f 043e 0437  .>. .@.0.A.?.>.7
+0000eb60: 043d 0430 0442 044c 0020 043e 043f 0438  .=.0.B.L. .>.?.8
+0000eb70: 0441 0430 043d 0438 0435 0020 0421 043c  .A.0.=.8.5. .!.<
+0000eb80: 0435 043d 044b 0020 0441 0438 043c 0432  .5.=.K. .A.8.<.2
+0000eb90: 043e 043b 0430 0020 0800 0000 0006 0000  .>.;.0. ........
+0000eba0: 0026 4361 6e27 7420 7061 7273 6520 5379  .&Can't parse Sy
+0000ebb0: 6d62 6f6c 2043 6861 6e67 6520 6465 7363  mbol Change desc
+0000ebc0: 7269 7074 696f 6e20 0700 0000 0d53 7461  ription .....Sta
+0000ebd0: 7465 6d65 6e74 4942 4b52 0103 0000 006e  tementIBKR.....n
+0000ebe0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+0000ebf0: 043d 043e 0020 043e 0431 0440 0430 0431  .=.>. .>.1.@.0.1
+0000ec00: 043e 0442 0430 0442 044c 0020 043e 0442  .>.B.0.B.L. .>.B
+0000ec10: 043c 0435 043d 0451 043d 043d 043e 0435  .<.5.=.Q.=.=.>.5
+0000ec20: 0020 043a 043e 0440 043f 043e 0440 0430  . .:.>.@.?.>.@.0
+0000ec30: 0442 0438 0432 043d 043e 0435 0020 0434  .B.8.2.=.>.5. .4
+0000ec40: 0435 0439 0441 0442 0432 0438 0435 0800  .5.9.A.B.2.8.5..
+0000ec50: 0000 0006 0000 0028 4361 6e27 7420 7072  .......(Can't pr
+0000ec60: 6f63 6573 7320 6361 6e63 656c 6c65 6420  ocess cancelled 
+0000ec70: 636f 7270 6f72 6174 6520 6163 7469 6f6e  corporate action
+0000ec80: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
+0000ec90: 4b52 0103 0000 003e 0414 0435 043d 0435  KR.....>...5.=.5
+0000eca0: 0436 043d 044b 0435 0020 0442 0440 0430  .6.=.K.5. .B.@.0
+0000ecb0: 043d 0437 0430 043a 0446 0438 0438 0020  .=.7.0.:.F.8.8. 
+0000ecc0: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
+0000ecd0: 044b 003a 0020 0800 0000 0006 0000 001a  .K.:. ..........
+0000ece0: 4361 7368 2074 7261 6e73 6163 7469 6f6e  Cash transaction
+0000ecf0: 7320 6c6f 6164 6564 3a20 0700 0000 0d53  s loaded: .....S
+0000ed00: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
+0000ed10: 006a 041a 043e 0440 043f 043e 0440 0430  .j...>.@.?.>.@.0
+0000ed20: 0442 0438 0432 043d 043e 0435 0020 0441  .B.8.2.=.>.5. .A
+0000ed30: 043e 0431 044b 0442 0438 0435 0020 043d  .>.1.K.B.8.5. .=
+0000ed40: 0435 0020 043f 043e 0434 0434 0435 0440  .5. .?.>.4.4.5.@
+0000ed50: 0436 0438 0432 0430 0435 0442 0441 044f  .6.8.2.0.5.B.A.O
+0000ed60: 0020 0434 043b 044f 0020 0442 0438 043f  . .4.;.O. .B.8.?
+0000ed70: 0430 0020 0426 0411 003a 0020 0800 0000  .0. .&...:. ....
+0000ed80: 0006 0000 0031 436f 7270 6f72 6174 6520  .....1Corporate 
+0000ed90: 6163 7469 6f6e 2069 736e 2774 2073 7570  action isn't sup
+0000eda0: 706f 7274 6564 2066 6f72 2061 7373 6574  ported for asset
+0000edb0: 2074 7970 653a 2007 0000 000d 5374 6174   type: .....Stat
+0000edc0: 656d 656e 7449 424b 5201 0300 0000 5e04  ementIBKR.....^.
+0000edd0: 2204 3804 3f00 2004 3a04 3e04 4004 3f04  ".8.?. .:.>.@.?.
+0000ede0: 3e04 4004 3004 4204 3804 3204 3d04 3e04  >.@.0.B.8.2.=.>.
+0000edf0: 3304 3e00 2004 3404 3504 3904 4104 4204  3.>. .4.5.9.A.B.
+0000ee00: 3204 3804 4f00 2004 3d04 3500 2004 3f04  2.8.O. .=.5. .?.
+0000ee10: 3e04 3404 3404 3504 4004 3604 3804 3204  >.4.4.5.@.6.8.2.
+0000ee20: 3004 3504 4204 4104 4f00 3a00 2008 0000  0.5.B.A.O.:. ...
+0000ee30: 0000 0600 0000 2843 6f72 706f 7261 7465  ......(Corporate
+0000ee40: 2061 6374 696f 6e20 7479 7065 2069 7320   action type is 
+0000ee50: 6e6f 7420 7375 7070 6f72 7465 643a 2007  not supported: .
+0000ee60: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000ee70: 5201 0300 0000 4404 1a04 3e04 4004 3f04  R.....D...>.@.?.
+0000ee80: 3e04 4004 3004 4204 3804 3204 3d04 4b04  >.@.0.B.8.2.=.K.
+0000ee90: 3500 2004 3404 3504 3904 4104 4204 3204  5. .4.5.9.A.B.2.
+0000eea0: 3804 4f00 2004 3704 3004 3304 4004 4304  8.O. .7.0.3.@.C.
+0000eeb0: 3604 3504 3d04 4b00 3a00 2008 0000 0000  6.5.=.K.:. .....
+0000eec0: 0600 0000 1a43 6f72 706f 7261 7465 2061  .....Corporate a
+0000eed0: 6374 696f 6e73 206c 6f61 6465 643a 2007  ctions loaded: .
+0000eee0: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000eef0: 5201 0300 0000 5604 1404 3804 3204 3804  R.....V...8.2.8.
+0000ef00: 3404 3504 3d04 3400 2004 3d04 3500 2004  4.5.=.4. .=.5. .
+0000ef10: 3d04 3004 3904 3404 3504 3d00 2004 3404  =.0.9.4.5.=. .4.
+0000ef20: 3b04 4f00 2004 4304 3404 3504 4004 3604  ;.O. .C.4.5.@.6.
+0000ef30: 3004 3d04 3d04 3e04 3304 3e00 2004 3d04  0.=.=.>.3.>. .=.
+0000ef40: 3004 3b04 3e04 3304 3000 3a00 2008 0000  0.;.>.3.0.:. ...
+0000ef50: 0000 0600 0000 2844 6976 6964 656e 6420  ......(Dividend 
+0000ef60: 6e6f 7420 666f 756e 6420 666f 7220 7769  not found for wi
+0000ef70: 7468 686f 6c64 696e 6720 7461 783a 2007  thholding tax: .
+0000ef80: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000ef90: 5201 0300 0000 2e00 4900 4200 4b00 5200  R.......I.B.K.R.
+0000efa0: 2000 6600 6c00 6500 7800 2d04 3e04 4204   .f.l.e.x.-.>.B.
+0000efb0: 4704 5104 4200 2000 2800 2a00 2e00 7800  G.Q.B. .(.*...x.
+0000efc0: 6d00 6c00 2908 0000 0000 0600 0000 1749  m.l.)..........I
+0000efd0: 424b 5220 666c 6578 2d71 7565 7279 2028  BKR flex-query (
+0000efe0: 2a2e 786d 6c29 0700 0000 0d53 7461 7465  *.xml).....State
+0000eff0: 6d65 6e74 4942 4b52 0103 0000 0026 0049  mentIBKR.....&.I
+0000f000: 006e 0074 0065 0072 0061 0063 0074 0069  .n.t.e.r.a.c.t.i
+0000f010: 0076 0065 0020 0042 0072 006f 006b 0065  .v.e. .B.r.o.k.e
+0000f020: 0072 0073 0800 0000 0006 0000 0013 496e  .r.s..........In
+0000f030: 7465 7261 6374 6976 6520 4272 6f6b 6572  teractive Broker
+0000f040: 7307 0000 000d 5374 6174 656d 656e 7449  s.....StatementI
+0000f050: 424b 5201 0300 0000 5604 2204 3804 3f00  BKR.....V.".8.?.
+0000f060: 2004 3e04 4204 4704 5104 4204 3000 2000   .>.B.G.Q.B.0. .
+0000f070: 4900 6e00 7400 6500 7200 6100 6300 7400  I.n.t.e.r.a.c.t.
+0000f080: 6900 7600 6500 2000 4200 7200 6f00 6b00  i.v.e. .B.r.o.k.
+0000f090: 6500 7200 7300 2004 3d04 3500 2004 3e04  e.r.s. .=.5. .>.
+0000f0a0: 3f04 4004 3504 3404 3504 3b04 5104 3d08  ?.@.5.4.5.;.Q.=.
+0000f0b0: 0000 0000 0600 0000 2949 6e74 6572 6163  ........)Interac
+0000f0c0: 7469 7665 2042 726f 6b65 7273 2072 6570  tive Brokers rep
+0000f0d0: 6f72 7420 7479 7065 206e 6f74 2066 6f75  ort type not fou
+0000f0e0: 6e64 0700 0000 0d53 7461 7465 6d65 6e74  nd.....Statement
+0000f0f0: 4942 4b52 0103 0000 003a 0417 0430 0433  IBKR.....:...0.3
+0000f100: 0440 0443 0437 043a 0430 0020 043e 0442  .@.C.7.:.0. .>.B
+0000f110: 0447 0451 0442 0430 0020 0049 0042 0020  .G.Q.B.0. .I.B. 
+0000f120: 0434 043b 044f 0020 0441 0447 0451 0442  .4.;.O. .A.G.Q.B
+0000f130: 0430 0020 0800 0000 0006 0000 0023 4c6f  .0. .........#Lo
+0000f140: 6164 2049 4220 466c 6578 2d73 7461 7465  ad IB Flex-state
+0000f150: 6d65 6e74 2066 6f72 2061 6363 6f75 6e74  ment for account
+0000f160: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
+0000f170: 424b 5201 0300 0000 5804 1d04 3504 3404  BKR.....X...5.4.
+0000f180: 3e04 4104 4204 3004 4204 3e04 4704 3d04  >.A.B.0.B.>.G.=.
+0000f190: 3e00 2004 3404 3004 3d04 3d04 4b04 4500  >. .4.0.=.=.K.E.
+0000f1a0: 2004 3e04 3100 2004 1e04 3104 4a04 3504   .>.1. ...1.J.5.
+0000f1b0: 3404 3804 3d04 3504 3d04 3804 3800 2004  4.8.=.5.=.8.8. .
+0000f1c0: 3a04 3e04 3c04 3f04 3004 3d04 3804 3900  :.>.<.?.0.=.8.9.
+0000f1d0: 2008 0000 0000 0600 0000 224d 6572 6765   ........."Merge
+0000f1e0: 7220 6465 7363 7269 7074 696f 6e20 6d69  r description mi
+0000f1f0: 7373 2073 6f6d 6520 6461 7461 2007 0000  ss some data ...
+0000f200: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
+0000f210: 0300 0000 5e04 1d04 3504 3e04 3404 3d04  ....^...5.>.4.=.
+0000f220: 3e04 3704 3d04 3004 4704 3d04 3e04 3500  >.7.=.0.G.=.>.5.
+0000f230: 2004 4104 3e04 3204 3f04 3004 3404 3504   .A.>.2.?.0.4.5.
+0000f240: 3d04 3804 3500 2004 4104 3e04 3104 4b04  =.8.5. .A.>.1.K.
+0000f250: 4204 3804 3900 2004 4004 3504 3e04 4004  B.8.9. .@.5.>.@.
+0000f260: 3304 3004 3d04 3804 3704 3004 4604 3804  3.0.=.8.7.0.F.8.
+0000f270: 3800 2008 0000 0000 0600 0000 294d 756c  8. .........)Mul
+0000f280: 7469 706c 6520 6d65 7267 6572 2072 6563  tiple merger rec
+0000f290: 6f72 6473 2061 6c72 6561 6479 2065 7869  ords already exi
+0000f2a0: 7374 2061 7420 0700 0000 0d53 7461 7465  st at .....State
+0000f2b0: 6d65 6e74 4942 4b52 0103 0000 0052 0414  mentIBKR.....R..
+0000f2c0: 0435 0439 0441 0442 0432 0438 0435 0020  .5.9.A.B.2.8.5. 
+0000f2d0: 043d 0435 0020 043f 043e 0434 0434 0435  .=.5. .?.>.4.4.5
+0000f2e0: 0440 0436 0438 0432 0430 0435 0442 0441  .@.6.8.2.0.5.B.A
+0000f2f0: 044f 0020 0434 043b 044f 0020 043e 043f  .O. .4.;.O. .>.?
+0000f300: 0446 0438 043e 043d 043e 0432 003a 0020  .F.8.>.=.>.2.:. 
+0000f310: 0800 0000 0006 0000 0027 4f70 7469 6f6e  .........'Option
+0000f320: 2045 2641 2645 2061 6374 696f 6e20 6973   E&A&E action is
+0000f330: 6e27 7420 696d 706c 656d 656e 7465 643a  n't implemented:
+0000f340: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
+0000f350: 424b 5201 0300 0000 3a04 1804 4104 3f04  BKR.....:...A.?.
+0000f360: 3e04 3b04 3d04 3504 3d04 3804 3500 2004  >.;.=.5.=.8.5. .
+0000f370: 3f04 4004 3e04 3404 3004 3d04 3d04 3e04  ?.@.>.4.0.=.=.>.
+0000f380: 3304 3e00 2004 3e04 3f04 4604 3804 3e04  3.>. .>.?.F.8.>.
+0000f390: 3d04 3008 0000 0000 0600 0000 114f 7074  =.0..........Opt
+0000f3a0: 696f 6e20 6173 7369 676e 6d65 6e74 0700  ion assignment..
+0000f3b0: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
+0000f3c0: 0103 0000 003a 0418 0441 043f 043e 043b  .....:...A.?.>.;
+0000f3d0: 043d 0435 043d 0438 0435 002f 044d 043a  .=.5.=.8.5./.M.:
+0000f3e0: 0441 043f 0438 0440 0430 0446 0438 044f  .A.?.8.@.0.F.8.O
+0000f3f0: 0020 043e 043f 0446 0438 043e 043d 0430  . .>.?.F.8.>.=.0
+0000f400: 0800 0000 0006 0000 001a 4f70 7469 6f6e  ..........Option
+0000f410: 2061 7373 6967 6e6d 656e 742f 6578 6572   assignment/exer
+0000f420: 6369 7365 0700 0000 0d53 7461 7465 6d65  cise.....Stateme
+0000f430: 6e74 4942 4b52 0103 0000 003a 0418 0441  ntIBKR.....:...A
+0000f440: 043f 043e 043b 043d 0435 043d 0438 0435  .?.>.;.=.5.=.8.5
+0000f450: 0020 043a 0443 043f 043b 0435 043d 043d  . .:.C.?.;.5.=.=
+0000f460: 043e 0433 043e 0020 043e 043f 0446 0438  .>.3.>. .>.?.F.8
+0000f470: 043e 043d 0430 0800 0000 0006 0000 000f  .>.=.0..........
+0000f480: 4f70 7469 6f6e 2065 7865 7263 6973 6507  Option exercise.
+0000f490: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000f4a0: 5201 0300 0000 2404 2d04 3a04 4104 3f04  R.....$.-.:.A.?.
+0000f4b0: 3804 4004 3004 4604 3804 4f00 2004 3e04  8.@.0.F.8.O. .>.
+0000f4c0: 3f04 4604 3804 3e04 3d04 3008 0000 0000  ?.F.8.>.=.0.....
+0000f4d0: 0600 0000 114f 7074 696f 6e20 6578 7069  .....Option expi
+0000f4e0: 7261 7469 6f6e 0700 0000 0d53 7461 7465  ration.....State
+0000f4f0: 6d65 6e74 4942 4b52 0103 0000 0040 0414  mentIBKR.....@..
+0000f500: 0435 0439 0441 0442 0432 0438 044f 0020  .5.9.A.B.2.8.O. 
+0000f510: 0441 0020 043e 043f 0446 0438 043e 043d  .A. .>.?.F.8.>.=
+0000f520: 0430 043c 0438 0020 0437 0430 0433 0440  .0.<.8. .7.0.3.@
+0000f530: 0443 0436 0435 043d 044b 003a 0020 0800  .C.6.5.=.K.:. ..
+0000f540: 0000 0006 0000 0016 4f70 7469 6f6e 7320  ........Options 
+0000f550: 4526 4126 4520 6c6f 6164 6564 3a20 0700  E&A&E loaded: ..
+0000f560: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
+0000f570: 0103 0000 006a 041d 0435 0020 043d 0430  .....j...5. .=.0
+0000f580: 0439 0434 0435 043d 0430 0020 0441 0434  .9.4.5.=.0. .A.4
+0000f590: 0435 043b 043a 0430 0020 0434 043b 044f  .5.;.:.0. .4.;.O
+0000f5a0: 0020 0438 0441 043f 043e 043b 043d 0435  . .8.A.?.>.;.=.5
+0000f5b0: 043d 0438 044f 002f 044d 043a 0441 043f  .=.8.O./.M.:.A.?
+0000f5c0: 0438 0440 0430 0446 0438 0438 0020 043e  .8.@.0.F.8.8. .>
+0000f5d0: 043f 0446 0438 043e 043d 0430 003a 0020  .?.F.8.>.=.0.:. 
+0000f5e0: 0800 0000 0006 0000 0035 4f72 6967 696e  .........5Origin
+0000f5f0: 616c 2074 7261 6465 206e 6f74 2066 6f75  al trade not fou
+0000f600: 6e64 2066 6f72 204f 7074 696f 6e20 4526  nd for Option E&
+0000f610: 4126 4520 6f70 6572 6174 696f 6e3a 2007  A&E operation: .
+0000f620: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000f630: 5201 0300 0000 6c04 1f04 3b04 3004 4204  R.....l...;.0.B.
+0000f640: 5104 3600 2004 3104 4b04 3b00 2004 3e04  Q.6. .1.K.;. .>.
+0000f650: 4204 3c04 3504 3d04 5104 3d00 2004 3f04  B.<.5.=.Q.=. .?.
+0000f660: 3e00 2004 3f04 4004 3804 3c04 3504 4004  >. .?.@.8.<.5.@.
+0000f670: 3d04 3e04 3c04 4300 2004 4104 3e04 3204  =.>.<.C. .A.>.2.
+0000f680: 3f04 3004 3404 3504 3d04 3804 4e00 2004  ?.0.4.5.=.8.N. .
+0000f690: 3e04 3f04 3804 4104 3004 3d04 3804 4f00  >.?.8.A.0.=.8.O.
+0000f6a0: 3a00 2008 0000 0000 0600 0000 3150 6179  :. .........1Pay
+0000f6b0: 6d65 6e74 2077 6173 2072 6576 6572 7365  ment was reverse
+0000f6c0: 6420 6279 2061 7070 726f 7869 6d61 7465  d by approximate
+0000f6d0: 2064 6573 6372 6970 7469 6f6e 3a20 0700   description: ..
+0000f6e0: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
+0000f6f0: 0103 0000 006a 041f 043b 0430 0442 0451  .....j...;.0.B.Q
+0000f700: 0436 0020 0431 044b 043b 0020 043e 0442  .6. .1.K.;. .>.B
+0000f710: 043c 0435 043d 0451 043d 002c 0020 043d  .<.5.=.Q.=.,. .=
+0000f720: 043e 0020 0441 0020 043d 0435 0441 043e  .>. .A. .=.5.A.>
+0000f730: 0432 043f 0430 0434 0430 044e 0449 0435  .2.?.0.4.0.N.I.5
+0000f740: 0439 0020 0434 0430 0442 043e 0439 0020  .9. .4.0.B.>.9. 
+0000f750: 043e 0442 0447 0451 0442 0430 003a 0020  .>.B.G.Q.B.0.:. 
+0000f760: 0800 0000 0006 0000 0033 5061 796d 656e  .........3Paymen
+0000f770: 7420 7761 7320 7265 7665 7273 6564 2077  t was reversed w
+0000f780: 6974 6820 6469 6666 6572 656e 7420 7265  ith different re
+0000f790: 706f 7274 6564 2064 6174 653a 2007 0000  ported date: ...
+0000f7a0: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
+0000f7b0: 0300 0000 2804 1f04 3b04 3004 4204 5104  ....(...;.0.B.Q.
+0000f7c0: 3600 2004 3104 4b04 3b00 2004 3e04 4204  6. .1.K.;. .>.B.
+0000f7d0: 3c04 3504 3d04 5104 3d00 3a00 2008 0000  <.5.=.Q.=.:. ...
+0000f7e0: 0000 0600 0000 1650 6179 6d65 6e74 2077  .......Payment w
+0000f7f0: 6173 2072 6576 6572 7365 643a 2007 0000  as reversed: ...
+0000f800: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
+0000f810: 0300 0000 1c04 2604 1100 2004 3704 3004  ......&... .7.0.
+0000f820: 3304 4004 4304 3604 3504 3d04 4b00 3a00  3.@.C.6.5.=.K.:.
+0000f830: 2008 0000 0000 0600 0000 1353 6563 7572   ..........Secur
+0000f840: 6974 6965 7320 6c6f 6164 6564 3a20 0700  ities loaded: ..
+0000f850: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
+0000f860: 0103 0000 0056 041d 0435 0434 043e 0441  .....V...5.4.>.A
+0000f870: 0442 0430 0442 043e 0447 043d 043e 0020  .B.0.B.>.G.=.>. 
+0000f880: 0434 0430 043d 043d 044b 0445 0020 0434  .4.0.=.=.K.E. .4
+0000f890: 043b 044f 0020 0412 044b 0434 0435 043b  .;.O. ...K.4.5.;
+0000f8a0: 0435 043d 0438 044f 0020 043a 043e 043c  .5.=.8.O. .:.>.<
+0000f8b0: 043f 0430 043d 0438 0438 0020 0800 0000  .?.0.=.8.8. ....
+0000f8c0: 0006 0000 0024 5370 696e 2d6f 6666 2064  .....$Spin-off d
+0000f8d0: 6573 6372 6970 7469 6f6e 206d 6973 7320  escription miss 
+0000f8e0: 736f 6d65 2064 6174 6120 0700 0000 0d53  some data .....S
+0000f8f0: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
+0000f900: 005c 0418 0441 0445 043e 0434 043d 0430  .\...A.E.>.4.=.0
+0000f910: 044f 0020 0426 0411 0020 0434 043b 044f  .O. .&... .4.;.O
+0000f920: 0020 0432 044b 0434 0435 043b 0435 043d  . .2.K.4.5.;.5.=
+0000f930: 0438 044f 0020 043a 043e 043c 043f 0430  .8.O. .:.>.<.?.0
+0000f940: 043d 0438 0438 0020 043d 0435 0020 043d  .=.8.8. .=.5. .=
+0000f950: 0430 0439 0434 0435 043d 0430 0020 0800  .0.9.4.5.=.0. ..
+0000f960: 0000 0006 0000 0021 5370 696e 2d6f 6666  .......!Spin-off
+0000f970: 2069 6e69 7469 616c 2061 7373 6574 206e   initial asset n
+0000f980: 6f74 2066 6f75 6e64 2007 0000 000d 5374  ot found .....St
+0000f990: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
+0000f9a0: 5604 1e04 4804 3804 3104 3a04 3000 2004  V...H.8.1.:.0. .
+0000f9b0: 3e04 3a04 4004 4304 3304 3b04 3504 3d04  >.:.@.C.3.;.5.=.
+0000f9c0: 3804 4f00 2000 5300 7000 6900 6e00 2d00  8.O. .S.p.i.n.-.
+0000f9d0: 6f00 6600 6600 2004 4104 3b04 3804 4804  o.f.f. .A.;.8.H.
+0000f9e0: 3a04 3e04 3c00 2004 3104 3e04 3b04 4c04  :.>.<. .1.>.;.L.
+0000f9f0: 4804 3004 4f00 2008 0000 0000 0600 0000  H.0.O. .........
+0000fa00: 2353 7069 6e2d 6f66 6620 726f 756e 6469  #Spin-off roundi
+0000fa10: 6e67 2065 7272 6f72 2069 7320 746f 6f20  ng error is too 
+0000fa20: 6269 6720 0700 0000 0d53 7461 7465 6d65  big .....Stateme
+0000fa30: 6e74 4942 4b52 0103 0000 003e 041d 0435  ntIBKR.....>...5
+0000fa40: 0434 043e 0441 0442 0430 0442 043e 0447  .4.>.A.B.0.B.>.G
+0000fa50: 043d 043e 0020 0434 0430 043d 043d 044b  .=.>. .4.0.=.=.K
+0000fa60: 0445 0020 0434 043b 044f 0020 0421 043f  .E. .4.;.O. .!.?
+0000fa70: 043b 0438 0442 0430 0020 0800 0000 0006  .;.8.B.0. ......
+0000fa80: 0000 0021 5370 6c69 7420 6465 7363 7269  ...!Split descri
+0000fa90: 7074 696f 6e20 6d69 7373 2073 6f6d 6520  ption miss some 
+0000faa0: 6461 7461 2007 0000 000d 5374 6174 656d  data .....Statem
+0000fab0: 656e 7449 424b 5201 0300 0000 3804 1704  entIBKR.....8...
+0000fac0: 3004 4704 3804 4104 3b04 3504 3d04 3804  0.G.8.A.;.5.=.8.
+0000fad0: 3500 2004 3004 3a04 4604 3804 3900 2004  5. .0.:.F.8.9. .
+0000fae0: 3704 3004 3304 4004 4304 3604 3504 3d04  7.0.3.@.C.6.5.=.
+0000faf0: 3e00 3a00 2008 0000 0000 0600 0000 1753  >.:. ..........S
+0000fb00: 746f 636b 2076 6573 7469 6e67 7320 6c6f  tock vestings lo
+0000fb10: 6164 6564 3a20 0700 0000 0d53 7461 7465  aded: .....State
+0000fb20: 6d65 6e74 4942 4b52 0103 0000 0048 041a  mentIBKR.....H..
+0000fb30: 043e 0440 0440 0435 043a 0442 0438 0440  .>.@.@.5.:.B.8.@
+0000fb40: 043e 0432 043a 0430 0020 043d 0430 043b  .>.2.:.0. .=.0.;
+0000fb50: 043e 0433 0430 0020 0434 043b 044f 0020  .>.3.0. .4.;.O. 
+0000fb60: 0434 0438 0432 0438 0434 0435 043d 0434  .4.8.2.8.4.5.=.4
+0000fb70: 0430 003a 0020 0800 0000 0006 0000 001d  .0.:. ..........
+0000fb80: 5461 7820 6164 6a75 7374 6d65 6e74 2066  Tax adjustment f
+0000fb90: 6f72 2064 6976 6964 656e 643a 2007 0000  or dividend: ...
+0000fba0: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
+0000fbb0: 0300 0000 2404 1d04 3004 3b04 3e04 3304  ....$...0.;.>.3.
+0000fbc0: 3800 2004 3704 3004 3304 4004 4304 3604  8. .7.0.3.@.C.6.
+0000fbd0: 3504 3d04 4b00 3a00 2008 0000 0000 0600  5.=.K.:. .......
+0000fbe0: 0000 0e54 6178 6573 206c 6f61 6465 643a  ...Taxes loaded:
+0000fbf0: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
+0000fc00: 424b 5201 03ff ffff ff08 0000 0000 0600  BKR.............
+0000fc10: 0000 0f54 7261 6465 7320 6c6f 6164 6564  ...Trades loaded
+0000fc20: 3a20 0700 0000 0d53 7461 7465 6d65 6e74  : .....Statement
+0000fc30: 4942 4b52 0103 0000 0058 041d 0435 043f  IBKR.....X...5.?
+0000fc40: 043e 0434 0434 0435 0440 0436 0438 0432  .>.4.4.5.@.6.8.2
+0000fc50: 0430 0435 043c 044b 0439 0020 0444 043e  .0.5.<.K.9. .D.>
+0000fc60: 0440 043c 0430 0442 0020 043e 043f 0438  .@.<.0.B. .>.?.8
+0000fc70: 0441 0430 043d 0438 044f 0020 0434 0438  .A.0.=.8.O. .4.8
+0000fc80: 0432 0438 0434 0435 043d 0434 0430 003a  .2.8.4.5.=.4.0.:
+0000fc90: 0020 0800 0000 0006 0000 0022 556e 6861  . ........."Unha
+0000fca0: 6e64 6c65 6420 6469 7669 6465 6e64 2070  ndled dividend p
+0000fcb0: 6174 7465 726e 2066 6f75 6e64 3a20 0700  attern found: ..
+0000fcc0: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
+0000fcd0: 0103 0000 004e 041d 0435 043f 043e 0434  .....N...5.?.>.4
+0000fce0: 0434 0435 0440 0436 0438 0432 0430 0435  .4.5.@.6.8.2.0.5
+0000fcf0: 043c 044b 0439 0020 0444 043e 0440 043c  .<.K.9. .D.>.@.<
+0000fd00: 0430 0442 0020 0441 0442 0440 0430 043d  .0.B. .A.B.@.0.=
+0000fd10: 044b 0020 043d 0430 043b 043e 0433 0430  .K. .=.0.;.>.3.0
+0000fd20: 003a 0020 0800 0000 0006 0000 0025 556e  .:. .........%Un
+0000fd30: 6861 6e64 6c65 6420 7461 7820 636f 756e  handled tax coun
+0000fd40: 7472 7920 7061 7474 6572 6e20 666f 756e  try pattern foun
+0000fd50: 643a 2007 0000 000d 5374 6174 656d 656e  d: .....Statemen
+0000fd60: 7449 424b 5201 0300 0000 5204 1d04 3504  tIBKR.....R...5.
+0000fd70: 3f04 3e04 3404 3404 3504 4004 3604 3804  ?.>.4.4.5.@.6.8.
+0000fd80: 3204 3004 3504 3c04 4b04 3900 2004 4404  2.0.5.<.K.9. .D.
+0000fd90: 3e04 4004 3c04 3004 4200 2004 3e04 3f04  >.@.<.0.B. .>.?.
+0000fda0: 3804 4104 3004 3d04 3804 4f00 2004 3d04  8.A.0.=.8.O. .=.
+0000fdb0: 3004 3b04 3e04 3304 3000 3a00 2008 0000  0.;.>.3.0.:. ...
+0000fdc0: 0000 0600 0000 1d55 6e68 616e 646c 6564  .......Unhandled
+0000fdd0: 2074 6178 2070 6174 7465 726e 2066 6f75   tax pattern fou
+0000fde0: 6e64 3a20 0700 0000 0d53 7461 7465 6d65  nd: .....Stateme
+0000fdf0: 6e74 4942 4b52 0103 0000 0058 041d 0435  ntIBKR.....X...5
+0000fe00: 0438 0437 0432 0435 0441 0442 043d 044b  .8.7.2.5.A.B.=.K
+0000fe10: 0439 0020 0442 0438 043f 0020 043e 0442  .9. .B.8.?. .>.B
+0000fe20: 0447 0451 0442 0430 0020 0049 006e 0074  .G.Q.B.0. .I.n.t
+0000fe30: 0065 0072 0061 0063 0074 0069 0076 0065  .e.r.a.c.t.i.v.e
+0000fe40: 0020 0042 0072 006f 006b 0065 0072 0073  . .B.r.o.k.e.r.s
+0000fe50: 003a 0020 0800 0000 0006 0000 0029 556e  .:. .........)Un
+0000fe60: 6b6e 6f77 6e20 496e 7465 7261 6374 6976  known Interactiv
+0000fe70: 6520 4272 6f6b 6572 7320 7265 706f 7274  e Brokers report
+0000fe80: 2074 7970 653a 2007 0000 000d 5374 6174   type: .....Stat
+0000fe90: 656d 656e 7449 424b 5201 0300 0000 a204  ementIBKR.......
+0000fea0: 1204 4b00 2004 3f04 4b04 4204 3004 3504  ..K. .?.K.B.0.5.
+0000feb0: 4204 3504 4104 4c00 2004 3704 3004 3304  B.5.A.L. .7.0.3.
+0000fec0: 4004 4304 3704 3804 4204 4c00 2004 3e04  @.C.7.8.B.L. .>.
+0000fed0: 4204 4704 5104 4200 2004 3e00 2004 3f04  B.G.Q.B. .>. .?.
+0000fee0: 3e04 3404 4204 3204 3504 4004 3604 3404  >.4.B.2.5.@.6.4.
+0000fef0: 5104 3d04 3d04 4b04 4500 2004 4104 3404  Q.=.=.K.E. .A.4.
+0000ff00: 3504 3b04 3a04 3004 4500 2004 3204 3c04  5.;.:.0.E. .2.<.
+0000ff10: 3504 4104 4204 3e00 2004 3e04 4204 4704  5.A.B.>. .>.B.G.
+0000ff20: 5104 4204 3000 2004 3f04 3e00 2004 1004  Q.B.0. .?.>. ...
+0000ff30: 3a04 4204 3804 3204 3d04 3e04 4104 4204  :.B.8.2.=.>.A.B.
+0000ff40: 3808 0000 0000 0600 0000 3f59 6f75 2074  8.........?You t
+0000ff50: 7279 2074 6f20 696d 706f 7274 2054 7261  ry to import Tra
+0000ff60: 6465 2063 6f6e 6669 6d61 7469 6f6e 2072  de confimation r
+0000ff70: 6570 6f72 742c 206e 6f74 2041 6374 6976  eport, not Activ
+0000ff80: 6974 7920 7265 706f 7274 0700 0000 0d53  ity report.....S
+0000ff90: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
+0000ffa0: 0052 041d 0435 0432 043e 0437 043c 043e  .R...5.2.>.7.<.>
+0000ffb0: 0436 043d 043e 0020 0440 0430 0441 043f  .6.=.>. .@.0.A.?
+0000ffc0: 043e 0437 043d 0430 0442 044c 0020 043e  .>.7.=.0.B.L. .>
+0000ffd0: 043f 0438 0441 0430 043d 0438 0435 0020  .?.8.A.0.=.8.5. 
+0000ffe0: 0434 0438 0432 0438 0434 0435 043d 0434  .4.8.2.8.4.5.=.4
+0000fff0: 0430 0020 0800 0000 0006 0000 0021 4361  .0. .........!Ca
+00010000: 6e27 7420 7061 7273 6520 4469 7669 6465  n't parse Divide
+00010010: 6e64 2064 6573 6372 6970 7469 6f6e 2007  nd description .
+00010020: 0000 000c 5374 6174 656d 656e 744a 3254  ....StatementJ2T
+00010030: 0103 0000 001c 0414 0421 0020 0437 0430  .........!. .7.0
+00010040: 0433 0440 0443 0436 0435 043d 044b 003a  .3.@.C.6.5.=.K.:
+00010050: 0020 0800 0000 0006 0000 0016 4361 7368  . ..........Cash
+00010060: 2062 616c 616e 6365 7320 6c6f 6164 6564   balances loaded
+00010070: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
+00010080: 4a32 5401 0300 0000 3a04 1404 3504 3d04  J2T.....:...5.=.
+00010090: 3504 3604 3d04 4b04 4500 2004 3e04 3f04  5.6.=.K.E. .>.?.
+000100a0: 3504 4004 3004 4604 3804 3900 2004 3704  5.@.0.F.8.9. .7.
+000100b0: 3004 3304 4004 4304 3604 3504 3d04 3e00  0.3.@.C.6.5.=.>.
+000100c0: 3a00 2008 0000 0000 0600 0000 1843 6173  :. ..........Cas
+000100d0: 6820 6f70 6572 6174 696f 6e73 206c 6f61  h operations loa
+000100e0: 6465 643a 2007 0000 000c 5374 6174 656d  ded: .....Statem
+000100f0: 656e 744a 3254 0103 0000 0048 0421 0434  entJ2T.....H.!.4
+00010100: 0435 043b 043a 0438 0020 0441 0020 043a  .5.;.:.8. .A. .:
+00010110: 0440 0438 043f 0442 043e 002d 0432 0430  .@.8.?.B.>.-.2.0
+00010120: 043b 044e 0442 0430 043c 0438 0020 0437  .;.N.B.0.<.8. .7
+00010130: 0430 0433 0440 0443 0436 0435 043d 044b  .0.3.@.C.6.5.=.K
+00010140: 003a 0020 0800 0000 0006 0000 0016 4372  .:. ..........Cr
+00010150: 7970 746f 2074 7261 6465 7320 6c6f 6164  ypto trades load
+00010160: 6564 3a20 0700 0000 0c53 7461 7465 6d65  ed: .....Stateme
+00010170: 6e74 4a32 5401 0300 0000 5004 1200 2004  ntJ2T.....P... .
+00010180: 3e04 3f04 3804 4104 3004 3d04 3804 3800  >.?.8.A.0.=.8.8.
+00010190: 2004 3404 3804 3204 3804 3404 3504 3d04   .4.8.2.8.4.5.=.
+000101a0: 3404 3000 2004 3e04 4204 4104 4304 4204  4.0. .>.B.A.C.B.
+000101b0: 4104 4204 3204 4304 4e04 4200 2004 3404  A.B.2.C.N.B. .4.
+000101c0: 3004 3d04 3d04 4b04 3500 2008 0000 0000  0.=.=.K.5. .....
+000101d0: 0600 0000 2444 6976 6964 656e 6420 6465  ....$Dividend de
+000101e0: 7363 7269 7074 696f 6e20 6d69 7373 2073  scription miss s
+000101f0: 6f6d 6520 6461 7461 2007 0000 000c 5374  ome data .....St
+00010200: 6174 656d 656e 744a 3254 0103 0000 004e  atementJ2T.....N
+00010210: 0414 0438 0432 0438 0434 0435 043d 0434  ...8.2.8.4.5.=.4
+00010220: 0020 043d 0435 0020 043d 0430 0439 0434  . .=.5. .=.0.9.4
+00010230: 0435 043d 0020 0434 043b 044f 0020 0441  .5.=. .4.;.O. .A
+00010240: 043f 0438 0441 0430 043d 0438 044f 0020  .?.8.A.0.=.8.O. 
+00010250: 043d 0430 043b 043e 0433 0430 0020 0800  .=.0.;.>.3.0. ..
+00010260: 0000 0006 0000 001f 4469 7669 6465 6e64  ........Dividend
+00010270: 2066 6f72 2074 6178 2077 6173 206e 6f74   for tax was not
+00010280: 2066 6f75 6e64 2007 0000 000c 5374 6174   found .....Stat
+00010290: 656d 656e 744a 3254 0103 0000 0044 0422  ementJ2T.....D."
+000102a0: 0440 0430 043d 0437 0430 043a 0446 0438  .@.0.=.7.0.:.F.8
+000102b0: 044f 0020 043f 0440 043e 043f 0443 0449  .O. .?.@.>.?.C.I
+000102c0: 0435 043d 0430 0020 043f 0440 0438 0020  .5.=.0. .?.@.8. 
+000102d0: 0438 043c 043f 043e 0440 0442 0435 003a  .8.<.?.>.@.B.5.:
+000102e0: 0020 0800 0000 0006 0000 001f 496d 706f  . ..........Impo
+000102f0: 7274 2073 6b69 7070 6564 206f 6620 7472  rt skipped of tr
+00010300: 616e 7361 6374 696f 6e3a 2007 0000 000c  ansaction: .....
+00010310: 5374 6174 656d 656e 744a 3254 0103 0000  StatementJ2T....
+00010320: 0014 004a 0075 0073 0074 0032 0054 0072  ...J.u.s.t.2.T.r
+00010330: 0061 0064 0065 0800 0000 0006 0000 000a  .a.d.e..........
+00010340: 4a75 7374 3254 7261 6465 0700 0000 0c53  Just2Trade.....S
+00010350: 7461 7465 6d65 6e74 4a32 5401 0300 0000  tatementJ2T.....
+00010360: 3204 1e04 4204 4704 5104 4200 2000 4a00  2...B.G.Q.B. .J.
+00010370: 7500 7300 7400 3200 5400 7200 6100 6400  u.s.t.2.T.r.a.d.
+00010380: 6500 2000 2800 2a00 2e00 7800 6c00 7300  e. .(.*...x.l.s.
+00010390: 7800 2908 0000 0000 0600 0000 1d4a 7573  x.)..........Jus
+000103a0: 7432 5472 6164 6520 7374 6174 656d 656e  t2Trade statemen
+000103b0: 7420 282a 2e78 6c73 7829 0700 0000 0c53  t (*.xlsx).....S
+000103c0: 7461 7465 6d65 6e74 4a32 5401 0300 0000  tatementJ2T.....
+000103d0: 1c04 2604 1100 2004 3704 3004 3304 4004  ..&... .7.0.3.@.
+000103e0: 4304 3604 3504 3d04 4b00 3a00 2008 0000  C.6.5.=.K.:. ...
+000103f0: 0000 0600 0000 1353 6563 7572 6974 6965  .......Securitie
+00010400: 7320 6c6f 6164 6564 3a20 0700 0000 0c53  s loaded: .....S
+00010410: 7461 7465 6d65 6e74 4a32 5401 0300 0000  tatementJ2T.....
+00010420: 3804 2104 3404 3504 3b04 3a04 3800 2004  8.!.4.5.;.:.8. .
+00010430: 4100 2004 3004 3a04 4604 3804 4f04 3c04  A. .0.:.F.8.O.<.
+00010440: 3800 2004 3704 3004 3304 4004 4304 3604  8. .7.0.3.@.C.6.
+00010450: 3504 3d04 4b00 3a00 2008 0000 0000 0600  5.=.K.:. .......
+00010460: 0000 1553 746f 636b 2074 7261 6465 7320  ...Stock trades 
+00010470: 6c6f 6164 6564 3a20 0700 0000 0c53 7461  loaded: .....Sta
+00010480: 7465 6d65 6e74 4a32 5401 0300 0000 4004  tementJ2T.....@.
+00010490: 1d04 3504 3804 3704 3204 3504 4104 4204  ..5.8.7.2.5.A.B.
+000104a0: 3d04 3004 4f00 2004 3404 3504 3d04 3504  =.0.O. .4.5.=.5.
+000104b0: 3604 3d04 3004 4f00 2004 4204 4004 3004  6.=.0.O. .B.@.0.
+000104c0: 3d04 3704 3004 3a04 4604 3804 4f00 2008  =.7.0.:.F.8.O. .
+000104d0: 0000 0000 0600 0000 1e55 6e6b 6e6f 776e  .........Unknown
+000104e0: 2063 6173 6820 7472 616e 7361 6374 696f   cash transactio
+000104f0: 6e20 7479 7065 2007 0000 000c 5374 6174  n type .....Stat
+00010500: 656d 656e 744a 3254 0103 0000 0030 041d  ementJ2T.....0..
+00010510: 0435 0438 0437 0432 0435 0441 0442 043d  .5.8.7.2.5.A.B.=
+00010520: 044b 0439 0020 0442 0438 043f 0020 0441  .K.9. .B.8.?. .A
+00010530: 0434 0435 043b 043a 0438 003a 0020 0800  .4.5.;.:.8.:. ..
+00010540: 0000 0006 0000 0014 556e 6b6e 6f77 6e20  ........Unknown 
+00010550: 7472 6164 6520 7479 7065 3a20 0700 0000  trade type: ....
+00010560: 0c53 7461 7465 6d65 6e74 4a32 5401 0300  .StatementJ2T...
+00010570: 0000 4a04 1d04 3504 3f04 3e04 3404 3404  ..J...5.?.>.4.4.
+00010580: 3504 4004 3604 3804 3204 3004 3504 3c04  5.@.6.8.2.0.5.<.
+00010590: 3004 4f00 2004 3404 3504 3d04 3504 3604  0.O. .4.5.=.5.6.
+000105a0: 3d04 3004 4f00 2004 4204 4004 3004 3d04  =.0.O. .B.@.0.=.
+000105b0: 3704 3004 3a04 4604 3804 4f00 2008 0000  7.0.:.F.8.O. ...
+000105c0: 0000 0600 0000 1e55 6e73 7570 7070 6f72  .......Unsupppor
+000105d0: 7465 6420 6361 7368 2074 7261 6e73 6163  ted cash transac
+000105e0: 7469 6f6e 2007 0000 000c 5374 6174 656d  tion .....Statem
+000105f0: 656e 744a 3254 0103 0000 003a 0414 0435  entJ2T.....:...5
+00010600: 043d 0435 0436 043d 044b 0445 0020 043e  .=.5.6.=.K.E. .>
+00010610: 043f 0435 0440 0430 0446 0438 0439 0020  .?.5.@.0.F.8.9. 
+00010620: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
+00010630: 043e 003a 0020 0800 0000 0006 0000 0018  .>.:. ..........
+00010640: 4361 7368 206f 7065 7261 7469 6f6e 7320  Cash operations 
+00010650: 6c6f 6164 6564 3a20 0700 0000 0c53 7461  loaded: .....Sta
+00010660: 7465 6d65 6e74 4b49 5401 0300 0000 7604  tementKIT.....v.
+00010670: 1d04 3004 3b04 3e04 3300 2004 3d04 3000  ..0.;.>.3. .=.0.
+00010680: 2004 3404 3804 3204 3804 3404 3504 3d04   .4.8.2.8.4.5.=.
+00010690: 3404 4b00 2004 3d04 3500 2004 3f04 3e04  4.K. .=.5. .?.>.
+000106a0: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
+000106b0: 3504 4204 4104 4f00 2004 3404 3b04 4f00  5.B.A.O. .4.;.O.
+000106c0: 2004 3104 4004 3e04 3a04 3504 4004 3000   .1.@.>.:.5.@.0.
+000106d0: 2004 1a04 1804 2200 2d04 4404 3804 3d04   .....".-.D.8.=.
+000106e0: 3004 3d04 4108 0000 0000 0600 0000 3e44  0.=.A.........>D
+000106f0: 6976 6964 656e 6420 7461 7865 7320 6172  ividend taxes ar
+00010700: 6520 6e6f 7420 7375 7070 6f72 7465 6420  e not supported 
+00010710: 666f 7220 4b49 5420 6272 6f6b 6572 2073  for KIT broker s
+00010720: 7461 7465 6d65 6e74 7320 7965 7407 0000  tatements yet...
+00010730: 000c 5374 6174 656d 656e 744b 4954 0103  ..StatementKIT..
+00010740: 0000 0014 041a 0418 0422 0020 0424 0438  .........". .$.8
+00010750: 043d 0430 043d 0441 0800 0000 0006 0000  .=.0.=.A........
+00010760: 000b 4b49 5420 4669 6e61 6e63 6507 0000  ..KIT Finance...
+00010770: 000c 5374 6174 656d 656e 744b 4954 0103  ..StatementKIT..
+00010780: 0000 0032 041e 0442 0447 0451 0442 0020  ...2...B.G.Q.B. 
+00010790: 041a 0418 0422 0020 0424 0438 043d 0430  .....". .$.8.=.0
+000107a0: 043d 0441 0020 0028 002a 002e 0078 006c  .=.A. .(.*...x.l
+000107b0: 0073 0078 0029 0800 0000 0006 0000 001e  .s.x.)..........
+000107c0: 4b49 5420 4669 6e61 6e63 6520 7374 6174  KIT Finance stat
+000107d0: 656d 656e 7420 282a 2e78 6c73 7829 0700  ement (*.xlsx)..
+000107e0: 0000 0c53 7461 7465 6d65 6e74 4b49 5401  ...StatementKIT.
+000107f0: 0300 0000 2404 2104 3404 3504 3b04 3a04  ....$.!.4.5.;.:.
+00010800: 3800 2004 3704 3004 3304 4004 4304 3604  8. .7.0.3.@.C.6.
+00010810: 3504 3d04 4b00 3a00 2008 0000 0000 0600  5.=.K.:. .......
+00010820: 0000 0f54 7261 6465 7320 6c6f 6164 6564  ...Trades loaded
+00010830: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
+00010840: 4b49 5401 0300 0000 3004 1d04 3504 3804  KIT.....0...5.8.
+00010850: 3704 3204 3504 4104 4204 3d04 4b04 3900  7.2.5.A.B.=.K.9.
+00010860: 2004 4204 3804 3f00 2004 4104 3404 3504   .B.8.?. .A.4.5.
+00010870: 3b04 3a04 3800 3a00 2008 0000 0000 0600  ;.:.8.:. .......
+00010880: 0000 1455 6e6b 6e6f 776e 2074 7261 6465  ...Unknown trade
+00010890: 2074 7970 653a 2007 0000 000c 5374 6174   type: .....Stat
+000108a0: 656d 656e 744b 4954 0103 0000 004a 041d  ementKIT.....J..
+000108b0: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
+000108c0: 0438 0432 0430 0435 043c 0430 044f 0020  .8.2.0.5.<.0.O. 
+000108d0: 0434 0435 043d 0435 0436 043d 0430 044f  .4.5.=.5.6.=.0.O
+000108e0: 0020 0442 0440 0430 043d 0437 0430 043a  . .B.@.0.=.7.0.:
+000108f0: 0446 0438 044f 0020 0800 0000 0006 0000  .F.8.O. ........
+00010900: 001e 556e 7375 7070 706f 7274 6564 2063  ..Unsuppported c
+00010910: 6173 6820 7472 616e 7361 6374 696f 6e20  ash transaction 
+00010920: 0700 0000 0c53 7461 7465 6d65 6e74 4b49  .....StatementKI
+00010930: 5401 0300 0000 2204 2104 4704 3504 4204  T.....".!.G.5.B.
+00010940: 3000 2004 3704 3004 3304 4004 4304 3604  0. .7.0.3.@.C.6.
+00010950: 3504 3d04 4b00 3a00 2008 0000 0000 0600  5.=.K.:. .......
+00010960: 0000 1141 6363 6f75 6e74 7320 6c6f 6164  ...Accounts load
+00010970: 6564 3a20 0700 0000 1353 7461 7465 6d65  ed: .....Stateme
 00010980: 6e74 4f70 656e 4272 6f6b 6572 0103 0000  ntOpenBroker....
-00010990: 0062 041d 0435 0432 043e 0437 043c 043e  .b...5.2.>.7.<.>
-000109a0: 0436 043d 043e 0020 043e 043f 0440 0435  .6.=.>. .>.?.@.5
-000109b0: 0434 0435 043b 0438 0442 044c 0020 0442  .4.5.;.8.B.L. .B
-000109c0: 0438 043f 002f 043a 043e 043b 0438 0447  .8.?./.:.>.;.8.G
-000109d0: 0435 0441 0442 0432 043e 0020 0434 043b  .5.A.B.2.>. .4.;
-000109e0: 044f 0020 0441 0434 0435 043b 043a 0438  .O. .A.4.5.;.:.8
-000109f0: 003a 0020 0800 0000 0006 0000 0025 4361  .:. .........%Ca
-00010a00: 6e27 7420 6465 7465 726d 696e 6520 7472  n't determine tr
-00010a10: 6164 6520 7479 7065 2f71 7561 6e74 6974  ade type/quantit
-00010a20: 793a 2007 0000 0013 5374 6174 656d 656e  y: .....Statemen
-00010a30: 744f 7065 6e42 726f 6b65 7201 0300 0000  tOpenBroker.....
-00010a40: 6804 1d04 3504 3204 3e04 3704 3c04 3e04  h...5.2.>.7.<.>.
-00010a50: 3604 3d04 3e00 2004 3e04 3f04 4004 3504  6.=.>. .>.?.@.5.
-00010a60: 3404 3504 3b04 3804 4204 4c00 2004 4104  4.5.;.8.B.L. .A.
-00010a70: 4704 5104 4200 2004 3404 3b04 4f00 2004  G.Q.B. .4.;.O. .
-00010a80: 3404 3504 3d04 3504 3604 3d04 3e04 3900  4.5.=.5.6.=.>.9.
-00010a90: 2004 4204 4004 3004 3d04 3704 3004 3a04   .B.@.0.=.7.0.:.
-00010aa0: 4604 3804 3800 3a00 2008 0000 0000 0600  F.8.8.:. .......
-00010ab0: 0000 2743 616e 2774 2066 696e 6420 6163  ..'Can't find ac
-00010ac0: 636f 756e 7420 666f 7220 6361 7368 206f  count for cash o
-00010ad0: 7065 7261 7469 6f6e 3a20 0700 0000 1353  peration: .....S
-00010ae0: 7461 7465 6d65 6e74 4f70 656e 4272 6f6b  tatementOpenBrok
-00010af0: 6572 0103 0000 0044 041d 0435 0432 043e  er.....D...5.2.>
-00010b00: 0437 043c 043e 0436 043d 043e 0020 043d  .7.<.>.6.=.>. .=
-00010b10: 0430 0439 0442 0438 0020 0441 0447 0451  .0.9.B.8. .A.G.Q
-00010b20: 0442 0020 0434 043b 044f 0020 0441 0434  .B. .4.;.O. .A.4
-00010b30: 0435 043b 043a 0438 003a 0020 0800 0000  .5.;.:.8.:. ....
-00010b40: 0006 0000 001e 4361 6e27 7420 6669 6e64  ......Can't find
-00010b50: 2061 6363 6f75 6e74 2066 6f72 2074 7261   account for tra
-00010b60: 6465 3a20 0700 0000 1353 7461 7465 6d65  de: .....Stateme
-00010b70: 6e74 4f70 656e 4272 6f6b 6572 0103 0000  ntOpenBroker....
-00010b80: 0050 041d 0435 0432 043e 0437 043c 043e  .P...5.2.>.7.<.>
-00010b90: 0436 043d 043e 0020 043d 0430 0439 0442  .6.=.>. .=.0.9.B
-00010ba0: 0438 0020 0437 0430 043f 0438 0441 044c  .8. .7.0.?.8.A.L
-00010bb0: 0020 0441 043f 0438 0441 0430 043d 0438  . .A.?.8.A.0.=.8
-00010bc0: 044f 0020 0426 0411 0020 0434 043b 044f  .O. .&... .4.;.O
-00010bd0: 0020 0800 0000 0006 0000 0029 4361 6e27  . .........)Can'
-00010be0: 7420 6669 6e64 2061 7373 6574 2063 616e  t find asset can
-00010bf0: 6365 6c6c 6174 696f 6e20 7265 636f 7264  cellation record
-00010c00: 2066 6f72 2007 0000 0013 5374 6174 656d   for .....Statem
-00010c10: 656e 744f 7065 6e42 726f 6b65 7201 0300  entOpenBroker...
-00010c20: 0000 3204 1d04 3500 2004 3d04 3004 3904  ..2...5. .=.0.9.
-00010c30: 3404 3504 3d04 3000 2004 2604 1100 2004  4.5.=.0. .&... .
-00010c40: 3404 3b04 4f00 2004 3a04 4304 3f04 3e04  4.;.O. .:.C.?.>.
-00010c50: 3d04 3000 2008 0000 0000 0600 0000 2343  =.0. .........#C
-00010c60: 616e 2774 2066 696e 6420 6173 7365 7420  an't find asset 
-00010c70: 666f 7220 626f 6e64 2069 6e74 6572 6573  for bond interes
-00010c80: 7420 0700 0000 1353 7461 7465 6d65 6e74  t .....Statement
-00010c90: 4f70 656e 4272 6f6b 6572 0103 0000 003c  OpenBroker.....<
-00010ca0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-00010cb0: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
-00010cc0: 0442 0430 0432 0438 0442 044c 0020 0426  .B.0.2.8.B.L. .&
-00010cd0: 0411 0020 0434 043b 044f 0020 0800 0000  ... .4.;.O. ....
-00010ce0: 0006 0000 0016 4361 6e27 7420 6d61 7463  ......Can't matc
-00010cf0: 6820 6173 7365 7420 666f 7220 0700 0000  h asset for ....
-00010d00: 1353 7461 7465 6d65 6e74 4f70 656e 4272  .StatementOpenBr
-00010d10: 6f6b 6572 0103 0000 0066 041d 0435 0432  oker.....f...5.2
-00010d20: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-00010d30: 0440 0430 0441 043f 043e 0437 043d 0430  .@.0.A.?.>.7.=.0
-00010d40: 0442 044c 0020 043e 043f 0438 0441 0430  .B.L. .>.?.8.A.0
-00010d50: 043d 0438 0435 0020 043f 043e 0433 0430  .=.8.5. .?.>.3.0
-00010d60: 0448 0435 043d 0438 044f 0020 043e 0431  .H.5.=.8.O. .>.1
-00010d70: 043b 0438 0433 0430 0446 0438 0438 0020  .;.8.3.0.F.8.8. 
-00010d80: 0800 0000 0006 0000 0024 4361 6e27 7420  .........$Can't 
-00010d90: 7061 7273 6520 426f 6e64 204d 6174 7572  parse Bond Matur
-00010da0: 6520 6465 7363 7269 7074 696f 6e20 0700  e description ..
-00010db0: 0000 1353 7461 7465 6d65 6e74 4f70 656e  ...StatementOpen
-00010dc0: 4272 6f6b 6572 0103 0000 004c 041d 0435  Broker.....L...5
-00010dd0: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
-00010de0: 0020 0440 0430 0441 043f 043e 0437 043d  . .@.0.A.?.>.7.=
-00010df0: 0430 0442 044c 0020 043e 043f 0438 0441  .0.B.L. .>.?.8.A
-00010e00: 0430 043d 0438 0435 0020 043a 0443 043f  .0.=.8.5. .:.C.?
-00010e10: 043e 043d 0430 0020 0800 0000 0006 0000  .>.=.0. ........
-00010e20: 0021 4361 6e27 7420 7061 7273 6520 496e  .!Can't parse In
-00010e30: 7465 7265 7374 2064 6573 6372 6970 7469  terest descripti
-00010e40: 6f6e 2007 0000 0013 5374 6174 656d 656e  on .....Statemen
-00010e50: 744f 7065 6e42 726f 6b65 7201 0300 0000  tOpenBroker.....
-00010e60: 6604 1d04 3504 3204 3e04 3704 3c04 3e04  f...5.2.>.7.<.>.
-00010e70: 3604 3d04 3e00 2004 4004 3004 4104 3f04  6.=.>. .@.0.A.?.
-00010e80: 3e04 3704 3d04 3004 4204 4c00 2004 3e04  >.7.=.0.B.L. .>.
-00010e90: 3f04 3804 4104 3004 3d04 3804 3500 2004  ?.8.A.0.=.8.5. .
-00010ea0: 3f04 3e04 3304 3004 4804 3504 3d04 3804  ?.>.3.0.H.5.=.8.
-00010eb0: 4f00 2004 3e04 3104 3b04 3804 3304 3004  O. .>.1.;.8.3.0.
-00010ec0: 4604 3804 3800 2008 0000 0000 0600 0000  F.8.8. .........
-00010ed0: 2743 616e 2774 2070 6172 7365 2062 6f6e  'Can't parse bon
-00010ee0: 6420 7265 7061 796d 656e 7420 6465 7363  d repayment desc
-00010ef0: 7269 7074 696f 6e20 0700 0000 1353 7461  ription .....Sta
-00010f00: 7465 6d65 6e74 4f70 656e 4272 6f6b 6572  tementOpenBroker
-00010f10: 0103 0000 003a 0414 0435 043d 0435 0436  .....:...5.=.5.6
-00010f20: 043d 044b 0445 0020 043e 043f 0435 0440  .=.K.E. .>.?.5.@
-00010f30: 0430 0446 0438 0439 0020 0437 0430 0433  .0.F.8.9. .7.0.3
-00010f40: 0440 0443 0436 0435 043d 043e 003a 0020  .@.C.6.5.=.>.:. 
-00010f50: 0800 0000 0006 0000 0018 4361 7368 206f  ..........Cash o
-00010f60: 7065 7261 7469 6f6e 7320 6c6f 6164 6564  perations loaded
-00010f70: 3a20 0700 0000 1353 7461 7465 6d65 6e74  : .....Statement
-00010f80: 4f70 656e 4272 6f6b 6572 0103 0000 0048  OpenBroker.....H
-00010f90: 041e 0442 0441 0443 0442 0441 0442 0432  ...B.A.C.B.A.B.2
-00010fa0: 0443 044e 0442 0020 0434 0430 043d 043d  .C.N.B. .4.0.=.=
-00010fb0: 044b 0435 0020 0432 0020 043e 043f 0438  .K.5. .2. .>.?.8
-00010fc0: 0441 0430 043d 0438 0020 043a 0443 043f  .A.0.=.8. .:.C.?
-00010fd0: 043e 043d 0430 0020 0800 0000 0006 0000  .>.=.0. ........
-00010fe0: 0024 496e 7465 7265 7374 2064 6573 6372  .$Interest descr
-00010ff0: 6970 7469 6f6e 206d 6973 7320 736f 6d65  iption miss some
-00011000: 2064 6174 6120 0700 0000 1353 7461 7465   data .....State
-00011010: 6d65 6e74 4f70 656e 4272 6f6b 6572 0103  mentOpenBroker..
-00011020: 0000 0054 0417 0430 0433 0440 0443 0437  ...T...0.3.@.C.7
-00011030: 043a 0430 0020 043e 0442 0447 0451 0442  .:.0. .>.B.G.Q.B
-00011040: 0430 0020 041e 0442 043a 0440 044b 0442  .0. ...B.:.@.K.B
-00011050: 0438 0435 0020 0431 0440 043e 043a 0435  .8.5. .1.@.>.:.5
-00011060: 0440 0020 0434 043b 044f 0020 0441 0447  .@. .4.;.O. .A.G
-00011070: 0451 0442 0430 0020 0800 0000 0006 0000  .Q.B.0. ........
-00011080: 0027 4c6f 6164 204f 7065 6e20 4272 6f6b  .'Load Open Brok
-00011090: 6572 2073 7461 7465 6d65 6e74 2066 6f72  er statement for
-000110a0: 2061 6363 6f75 6e74 2007 0000 0013 5374   account .....St
-000110b0: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
-000110c0: 7201 0300 0000 5604 1d04 3004 3904 3404  r.....V...0.9.4.
-000110d0: 3504 3d04 4b00 2004 3d04 3504 4104 3a04  5.=.K. .=.5.A.:.
-000110e0: 3e04 3b04 4c04 3a04 3e00 2004 3704 3004  >.;.L.:.>. .7.0.
-000110f0: 3f04 3804 4104 3504 3900 2004 3f04 3e04  ?.8.A.5.9. .?.>.
-00011100: 3304 3004 4804 3504 3d04 3804 4f00 2004  3.0.H.5.=.8.O. .
-00011110: 2604 1100 2004 3404 3b04 4f00 2008 0000  &... .4.;.O. ...
-00011120: 0000 0600 0000 264d 756c 7469 706c 6520  ......&Multiple 
-00011130: 6173 7365 7420 6361 6e63 656c 6c61 7469  asset cancellati
-00011140: 6f6e 206d 6174 6368 2066 6f72 2007 0000  on match for ...
-00011150: 0013 5374 6174 656d 656e 744f 7065 6e42  ..StatementOpenB
-00011160: 726f 6b65 7201 0300 0000 7404 1d04 3504  roker.....t...5.
-00011170: 4104 3a04 3e04 3b04 4c04 3a04 3e00 2004  A.:.>.;.L.:.>. .
-00011180: 4104 3e04 3204 3f04 3004 3404 3504 3d04  A.>.2.?.0.4.5.=.
-00011190: 3804 3900 2004 3404 3b04 4f00 2004 4104  8.9. .4.;.O. .A.
-000111a0: 3804 3c04 3204 3e04 3b04 3000 2c00 2004  8.<.2.>.;.0.,. .
-000111b0: 3804 4104 3f04 3e04 3b04 4c04 3704 4304  8.A.?.>.;.L.7.C.
-000111c0: 3504 3c04 3e04 3304 3e00 2004 3104 4004  5.<.>.3.>. .1.@.
-000111d0: 3e04 3a04 3504 4004 3e04 3c00 3a00 2008  >.:.5.@.>.<.:. .
-000111e0: 0000 0000 0600 0000 224d 756c 7469 706c  ........"Multipl
-000111f0: 6520 6d61 7463 6820 666f 7220 6272 6f6b  e match for brok
-00011200: 6572 2073 796d 626f 6c3a 2007 0000 0013  er symbol: .....
-00011210: 5374 6174 656d 656e 744f 7065 6e42 726f  StatementOpenBro
-00011220: 6b65 7201 0300 0000 4404 1d04 3504 4104  ker.....D...5.A.
-00011230: 3a04 3e04 3b04 4c04 3a04 3e00 2004 4104  :.>.;.L.:.>. .A.
-00011240: 3e04 3204 3f04 3004 3404 3504 3d04 3804  >.2.?.0.4.5.=.8.
-00011250: 3900 2004 3404 3b04 4f00 2004 4104 3804  9. .4.;.O. .A.8.
-00011260: 3c04 3204 3e04 3b04 3000 3a00 2008 0000  <.2.>.;.0.:. ...
-00011270: 0000 0600 0000 1b4d 756c 7469 706c 6520  .......Multiple 
-00011280: 6d61 7463 6820 666f 7220 7379 6d62 6f6c  match for symbol
-00011290: 3a20 0700 0000 1353 7461 7465 6d65 6e74  : .....Statement
-000112a0: 4f70 656e 4272 6f6b 6572 0103 0000 001e  OpenBroker......
-000112b0: 041e 0442 043a 0440 044b 0442 0438 0435  ...B.:.@.K.B.8.5
-000112c0: 0020 0431 0440 043e 043a 0435 0440 0800  . .1.@.>.:.5.@..
-000112d0: 0000 0006 0000 000b 4f70 656e 2042 726f  ........Open Bro
-000112e0: 6b65 7207 0000 0013 5374 6174 656d 656e  ker.....Statemen
-000112f0: 744f 7065 6e42 726f 6b65 7201 0300 0000  tOpenBroker.....
-00011300: 3c04 1e04 4204 4704 5104 4200 2004 3104  <...B.G.Q.B. .1.
-00011310: 4004 3e04 3a04 3504 4004 3000 2004 1e04  @.>.:.5.@.0. ...
-00011320: 4204 3a04 4004 4b04 4204 3804 3500 2000  B.:.@.K.B.8.5. .
-00011330: 2800 2a00 2e00 7800 6d00 6c00 2908 0000  (.*...x.m.l.)...
-00011340: 0000 0600 0000 1d4f 7065 6e20 4272 6f6b  .......Open Brok
-00011350: 6572 2073 7461 7465 6d65 6e74 2028 2a2e  er statement (*.
-00011360: 786d 6c29 0700 0000 1353 7461 7465 6d65  xml).....Stateme
-00011370: 6e74 4f70 656e 4272 6f6b 6572 0103 0000  ntOpenBroker....
-00011380: 0054 0417 0430 0433 043e 043b 043e 0432  .T...0.3.>.;.>.2
-00011390: 043e 043a 0020 043e 0442 0447 0451 0442  .>.:. .>.B.G.Q.B
-000113a0: 0430 0020 041e 0442 043a 0440 044b 0442  .0. ...B.:.@.K.B
-000113b0: 0438 0435 0020 0431 0440 043e 043a 0435  .8.5. .1.@.>.:.5
-000113c0: 0440 0020 043d 0435 0020 043d 0430 0439  .@. .=.5. .=.0.9
-000113d0: 0434 0435 043d 0800 0000 0006 0000 0022  .4.5.=........."
-000113e0: 4f70 656e 2062 726f 6b65 7220 7265 706f  Open broker repo
-000113f0: 7274 2074 6974 6c65 206e 6f74 2066 6f75  rt title not fou
-00011400: 6e64 0700 0000 1353 7461 7465 6d65 6e74  nd.....Statement
-00011410: 4f70 656e 4272 6f6b 6572 0103 0000 0038  OpenBroker.....8
-00011420: 041e 043f 0435 0440 0430 0446 0438 044f  ...?.5.@.0.F.8.O
-00011430: 0020 043d 0435 0020 043f 043e 0434 0434  . .=.5. .?.>.4.4
-00011440: 0435 0440 0436 0438 0432 0430 0435 0442  .5.@.6.8.2.0.5.B
-00011450: 0441 044f 003a 0020 0800 0000 0006 0000  .A.O.:. ........
-00011460: 0019 4f70 6572 6174 696f 6e20 6e6f 7420  ..Operation not 
-00011470: 7375 7070 6f72 7465 643a 2007 0000 0013  supported: .....
-00011480: 5374 6174 656d 656e 744f 7065 6e42 726f  StatementOpenBro
-00011490: 6b65 7201 0300 0000 1c04 2604 1100 2004  ker.......&... .
-000114a0: 3704 3004 3304 4004 4304 3604 3504 3d04  7.0.3.@.C.6.5.=.
-000114b0: 4b00 3a00 2008 0000 0000 0600 0000 1353  K.:. ..........S
-000114c0: 6563 7572 6974 6965 7320 6c6f 6164 6564  ecurities loaded
-000114d0: 3a20 0700 0000 1353 7461 7465 6d65 6e74  : .....Statement
-000114e0: 4f70 656e 4272 6f6b 6572 0103 0000 006e  OpenBroker.....n
-000114f0: 041d 0435 043f 043e 0434 0434 0435 0440  ...5.?.>.4.4.5.@
-00011500: 0436 0438 0432 0430 0435 043c 044b 0439  .6.8.2.0.5.<.K.9
-00011510: 0020 0437 0430 0433 043e 043b 043e 0432  . .7.0.3.>.;.>.2
-00011520: 043e 043a 0020 043e 0442 0447 0451 0442  .>.:. .>.B.G.Q.B
-00011530: 0430 0020 0434 043b 044f 0020 041e 0442  .0. .4.;.O. ...B
-00011540: 043a 0440 044b 0442 0438 0435 0020 0431  .:.@.K.B.8.5. .1
-00011550: 0440 043e 043a 0435 0440 003a 0020 0800  .@.>.:.5.@.:. ..
-00011560: 0000 0006 0000 0026 556e 6578 7065 6374  .......&Unexpect
-00011570: 6564 204f 7065 6e20 6272 6f6b 6572 2072  ed Open broker r
-00011580: 6570 6f72 7420 6865 6164 6572 3a20 0700  eport header: ..
-00011590: 0000 1353 7461 7465 6d65 6e74 4f70 656e  ...StatementOpen
-000115a0: 4272 6f6b 6572 0103 0000 0042 041d 0435  Broker.....B...5
-000115b0: 0438 0437 0432 0435 0441 0442 043d 0430  .8.7.2.5.A.B.=.0
-000115c0: 044f 0020 043d 0435 0442 043e 0440 0433  .O. .=.5.B.>.@.3
-000115d0: 043e 0432 0430 044f 0020 043e 043f 0435  .>.2.0.O. .>.?.5
-000115e0: 0440 0430 0446 0438 044f 003a 0020 0800  .@.0.F.8.O.:. ..
-000115f0: 0000 0006 0000 001d 556e 6b6e 6f77 6e20  ........Unknown 
-00011600: 6e6f 6e2d 7472 6164 6520 6f70 6572 6174  non-trade operat
-00011610: 696f 6e3a 2007 0000 0013 5374 6174 656d  ion: .....Statem
-00011620: 656e 744f 7065 6e42 726f 6b65 7201 0300  entOpenBroker...
-00011630: 0000 4604 1d04 3504 3f04 3e04 3404 3404  ..F...5.?.>.4.4.
-00011640: 3504 4004 3604 3804 3204 3004 3504 3c04  5.@.6.8.2.0.5.<.
-00011650: 3e04 3500 2004 3e04 3f04 3804 4104 3004  >.5. .>.?.8.A.0.
-00011660: 3d04 3804 3500 2004 3f04 3b04 3004 4204  =.8.5. .?.;.0.B.
-00011670: 3504 3604 3000 3a00 2008 0000 0000 0600  5.6.0.:. .......
-00011680: 0000 1d55 6e6b 6e6f 776e 2070 6179 6d65  ...Unknown payme
-00011690: 6e74 2064 6573 6372 6970 7469 6f6e 3a20  nt description: 
-000116a0: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
-000116b0: 656e 4272 6f6b 6572 0103 0000 0032 041d  enBroker.....2..
-000116c0: 0435 0438 0437 0432 0435 0441 0442 043d  .5.8.7.2.5.A.B.=
-000116d0: 044b 0439 0020 0442 0438 043f 0020 043f  .K.9. .B.8.?. .?
-000116e0: 043b 0430 0442 0435 0436 0430 003a 0020  .;.0.B.5.6.0.:. 
-000116f0: 0800 0000 0006 0000 0016 556e 6b6e 6f77  ..........Unknow
-00011700: 6e20 7061 796d 656e 7420 7479 7065 3a20  n payment type: 
-00011710: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
-00011720: 656e 4272 6f6b 6572 0103 0000 0016 0426  enBroker.......&
-00011730: 0411 0020 0431 0435 0437 0020 0069 0064  ... .1.5.7. .i.d
-00011740: 003a 0020 0800 0000 0006 0000 0012 4173  .:. ..........As
-00011750: 7365 7420 7769 7468 6f75 7420 6964 3a20  set without id: 
-00011760: 0700 0000 1653 7461 7465 6d65 6e74 4f70  .....StatementOp
-00011770: 656e 506f 7274 666f 6c69 6f01 0300 0000  enPortfolio.....
-00011780: 4804 1d04 3504 3204 3e04 3704 3c04 3e04  H...5.2.>.7.<.>.
-00011790: 3604 3d04 3e00 2004 3f04 4004 3e04 4704  6.=.>. .?.@.>.G.
-000117a0: 3804 4204 3004 4204 4c00 2000 4a00 5300  8.B.0.B.L. .J.S.
-000117b0: 4f00 4e00 2004 3804 3700 2004 4404 3004  O.N. .8.7. .D.0.
-000117c0: 3904 3b04 3000 3a00 2008 0000 0000 0600  9.;.0.:. .......
-000117d0: 0000 1f46 6169 6c65 6420 746f 2072 6561  ...Failed to rea
-000117e0: 6420 4a53 4f4e 2066 726f 6d20 6669 6c65  d JSON from file
-000117f0: 3a20 0700 0000 1653 7461 7465 6d65 6e74  : .....Statement
-00011800: 4f70 656e 506f 7274 666f 6c69 6f01 0300  OpenPortfolio...
-00011810: 0000 3404 1d04 3504 3204 3e04 3704 3c04  ..4...5.2.>.7.<.
-00011820: 3e04 3604 3d04 3e00 2004 3f04 4004 3e04  >.6.=.>. .?.@.>.
-00011830: 4704 3504 4104 4204 4c00 2004 4404 3004  G.5.A.B.L. .D.0.
-00011840: 3904 3b00 3a00 2008 0000 0000 0600 0000  9.;.:. .........
-00011850: 1546 6169 6c65 6420 746f 2072 6561 6420  .Failed to read 
-00011860: 6669 6c65 3a20 0700 0000 1653 7461 7465  file: .....State
-00011870: 6d65 6e74 4f70 656e 506f 7274 666f 6c69  mentOpenPortfoli
-00011880: 6f01 0300 0000 2204 1804 3c04 3f04 3e04  o....."...<.?.>.
-00011890: 4004 4204 3804 4004 3e04 3204 3004 3d04  @.B.8.@.>.2.0.=.
-000118a0: 3d04 4b04 3900 2021 1608 0000 0000 0600  =.K.9. !........
-000118b0: 0000 0a49 6d70 6f72 7465 6420 2307 0000  ...Imported #...
-000118c0: 0016 5374 6174 656d 656e 744f 7065 6e50  ..StatementOpenP
-000118d0: 6f72 7466 6f6c 696f 0103 0000 002e 0049  ortfolio.......I
-000118e0: 006e 0076 0065 0073 0074 0062 006f 006f  .n.v.e.s.t.b.o.o
-000118f0: 006b 0020 002f 0020 0049 005a 0049 002d  .k. ./. .I.Z.I.-
-00011900: 0069 006e 0076 0065 0073 0074 0800 0000  .i.n.v.e.s.t....
-00011910: 0006 0000 0017 496e 7665 7374 626f 6f6b  ......Investbook
-00011920: 202f 2049 5a49 2d49 6e76 6573 7407 0000   / IZI-Invest...
-00011930: 0016 5374 6174 656d 656e 744f 7065 6e50  ..StatementOpenP
-00011940: 6f72 7466 6f6c 696f 0103 0000 0042 041e  ortfolio.....B..
-00011950: 0431 044f 0437 0430 0442 0435 043b 044c  .1.O.7.0.B.5.;.L
-00011960: 043d 0430 044f 0020 0441 0435 043a 0446  .=.0.O. .A.5.:.F
-00011970: 0438 044f 0020 043e 0442 0441 0443 0442  .8.O. .>.B.A.C.B
-00011980: 0441 0442 0432 0443 0435 0442 003a 0020  .A.B.2.C.5.B.:. 
-00011990: 0800 0000 0006 0000 001e 4d61 6e64 6174  ..........Mandat
-000119a0: 6f72 7920 7365 6374 696f 6e20 6973 206d  ory section is m
-000119b0: 6973 7369 6e67 3a20 0700 0000 1653 7461  issing: .....Sta
-000119c0: 7465 6d65 6e74 4f70 656e 506f 7274 666f  tementOpenPortfo
-000119d0: 6c69 6f01 0300 0000 2e00 4f00 7000 6500  lio.......O.p.e.
-000119e0: 6e00 2000 7000 6f00 7200 7400 6600 6f00  n. .p.o.r.t.f.o.
-000119f0: 6c00 6900 6f00 2000 2800 2a00 2e00 6a00  l.i.o. .(.*...j.
-00011a00: 7300 6f00 6e00 2908 0000 0000 0600 0000  s.o.n.).........
-00011a10: 174f 7065 6e20 706f 7274 666f 6c69 6f20  .Open portfolio 
-00011a20: 282a 2e6a 736f 6e29 0700 0000 1653 7461  (*.json).....Sta
-00011a30: 7465 6d65 6e74 4f70 656e 506f 7274 666f  tementOpenPortfo
-00011a40: 6c69 6f01 0300 0000 4e04 1d04 3504 3f04  lio.....N...5.?.
-00011a50: 3e04 3404 3404 3504 4004 3604 3804 3204  >.4.4.5.@.6.8.2.
-00011a60: 3004 3504 3c04 3004 4f00 2004 3204 3504  0.5.<.0.O. .2.5.
-00011a70: 4004 4104 3804 4f00 2004 4404 3e04 4004  @.A.8.O. .D.>.@.
-00011a80: 3c04 3004 4204 3000 2004 4404 3004 3904  <.0.B.0. .D.0.9.
-00011a90: 3b04 3000 3a00 2008 0000 0000 0600 0000  ;.0.:. .........
-00011aa0: 2e55 6e73 7570 706f 7274 6564 2076 6572  .Unsupported ver
-00011ab0: 7369 6f6e 206f 6620 6f70 656e 2070 6f72  sion of open por
-00011ac0: 7466 6f6c 696f 2066 6f72 6d61 743a 2007  tfolio format: .
-00011ad0: 0000 0016 5374 6174 656d 656e 744f 7065  ....StatementOpe
-00011ae0: 6e50 6f72 7466 6f6c 696f 0103 0000 0038  nPortfolio.....8
-00011af0: 041a 0443 043f 043e 043d 044b 0020 043e  ...C.?.>.=.K. .>
-00011b00: 0431 043b 0438 0433 0430 0446 0438 0439  .1.;.8.3.0.F.8.9
-00011b10: 0020 0437 0430 0433 0440 0443 0436 0435  . .7.0.3.@.C.6.5
-00011b20: 043d 044b 003a 0020 0800 0000 0006 0000  .=.K.:. ........
-00011b30: 0017 426f 6e64 2069 6e74 6572 6573 7473  ..Bond interests
-00011b40: 206c 6f61 6465 643a 2007 0000 000c 5374   loaded: .....St
-00011b50: 6174 656d 656e 7450 5342 0103 0000 003e  atementPSB.....>
-00011b60: 0414 0435 043d 0435 0436 043d 044b 0435  ...5.=.5.6.=.K.5
-00011b70: 0020 0442 0440 0430 043d 0437 0430 043a  . .B.@.0.=.7.0.:
-00011b80: 0446 0438 0438 0020 0437 0430 0433 0440  .F.8.8. .7.0.3.@
-00011b90: 0443 0436 0435 043d 044b 003a 0020 0800  .C.6.5.=.K.:. ..
-00011ba0: 0000 0006 0000 001a 4361 7368 2074 7261  ........Cash tra
-00011bb0: 6e73 6163 7469 6f6e 7320 6c6f 6164 6564  nsactions loaded
-00011bc0: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
-00011bd0: 5053 4201 0300 0000 2a04 1404 3804 3204  PSB.....*...8.2.
-00011be0: 3804 3404 3504 3d04 3404 4b00 2004 3704  8.4.5.=.4.K. .7.
-00011bf0: 3004 3304 4004 4304 3604 3504 3d04 4b00  0.3.@.C.6.5.=.K.
-00011c00: 3a00 2008 0000 0000 0600 0000 1244 6976  :. ..........Div
-00011c10: 6964 656e 6473 206c 6f61 6465 643a 2007  idends loaded: .
-00011c20: 0000 000c 5374 6174 656d 656e 7450 5342  ....StatementPSB
-00011c30: 0103 0000 0014 041f 0421 0411 002d 0431  .........!...-.1
-00011c40: 0440 043e 043a 0435 0440 0800 0000 0006  .@.>.:.5.@......
-00011c50: 0000 000a 5053 4220 4272 6f6b 6572 0700  ....PSB Broker..
-00011c60: 0000 0c53 7461 7465 6d65 6e74 5053 4201  ...StatementPSB.
-00011c70: 0300 0000 4004 1e04 4204 4704 5104 4200  ....@...B.G.Q.B.
-00011c80: 2004 3104 4004 3e04 3a04 3504 4004 3000   .1.@.>.:.5.@.0.
-00011c90: 2004 1f04 2104 1100 2000 2800 2a00 2e00   ...!... .(.*...
-00011ca0: 7800 6c00 7300 7800 2000 2a00 2e00 7800  x.l.s.x. .*...x.
-00011cb0: 6c00 7300 2908 0000 0000 0600 0000 2350  l.s.).........#P
-00011cc0: 5342 2062 726f 6b65 7220 7374 6174 656d  SB broker statem
-00011cd0: 656e 7420 282a 2e78 6c73 7820 2a2e 786c  ent (*.xlsx *.xl
-00011ce0: 7329 0700 0000 0c53 7461 7465 6d65 6e74  s).....Statement
-00011cf0: 5053 4201 03ff ffff ff08 0000 0000 0600  PSB.............
-00011d00: 0000 0f54 7261 6465 7320 6c6f 6164 6564  ...Trades loaded
-00011d10: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
-00011d20: 5053 4201 0300 0000 4004 1d04 3504 3f04  PSB.....@...5.?.
-00011d30: 3e04 3404 3404 3504 4004 3604 3804 3204  >.4.4.5.@.6.8.2.
-00011d40: 3004 3504 3c04 3004 4f00 2004 3e04 3f04  0.5.<.0.O. .>.?.
-00011d50: 3504 4004 3004 4604 3804 4f00 2004 4100  5.@.0.F.8.O. .A.
-00011d60: 2004 1404 2100 3a00 2008 0000 0000 0600   ...!.:. .......
-00011d70: 0000 1855 6e6b 6e6f 776e 2063 6173 6820  ...Unknown cash 
-00011d80: 6f70 6572 6174 696f 6e3a 2007 0000 000c  operation: .....
-00011d90: 5374 6174 656d 656e 7450 5342 0103 0000  StatementPSB....
-00011da0: 003a 041d 0435 0438 0437 0432 0435 0441  .:...5.8.7.2.5.A
-00011db0: 0442 043d 044b 0439 0020 0442 0438 043f  .B.=.K.9. .B.8.?
-00011dc0: 0020 0434 0432 0438 0436 0435 043d 0438  . .4.2.8.6.5.=.8
-00011dd0: 044f 0020 0414 0421 003a 0020 0800 0000  .O. ...!.:. ....
-00011de0: 0006 0000 001a 556e 6b6e 6f77 6e20 6361  ......Unknown ca
-00011df0: 7368 2074 7261 6e73 6163 7469 6f6e 3a20  sh transaction: 
-00011e00: 0700 0000 0c53 7461 7465 6d65 6e74 5053  .....StatementPS
-00011e10: 4201 0300 0000 3004 1d04 3504 3804 3704  B.....0...5.8.7.
-00011e20: 3204 3504 4104 4204 3d04 4b04 3900 2004  2.5.A.B.=.K.9. .
-00011e30: 4204 3804 3f00 2004 4104 3404 3504 3b04  B.8.?. .A.4.5.;.
-00011e40: 3a04 3800 3a00 2008 0000 0000 0600 0000  :.8.:. .........
-00011e50: 1455 6e6b 6e6f 776e 2074 7261 6465 2074  .Unknown trade t
-00011e60: 7970 653a 2007 0000 000c 5374 6174 656d  ype: .....Statem
-00011e70: 656e 7450 5342 0103 0000 0032 041d 0435  entPSB.....2...5
-00011e80: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
-00011e90: 0432 0430 0435 043c 044b 0439 0020 043f  .2.0.5.<.K.9. .?
-00011ea0: 043b 0430 0442 0451 0436 003a 0020 0800  .;.0.B.Q.6.:. ..
-00011eb0: 0000 0006 0000 0015 556e 7375 7070 6f72  ........Unsuppor
-00011ec0: 7465 6420 7061 796d 656e 743a 2007 0000  ted payment: ...
-00011ed0: 000c 5374 6174 656d 656e 7450 5342 0103  ..StatementPSB..
-00011ee0: 0000 005a 0421 0434 0435 043b 043a 0430  ...Z.!.4.5.;.:.0
-00011ef0: 0020 0441 0020 0440 0430 0437 043d 044b  . .A. .@.0.7.=.K
-00011f00: 043c 0438 0020 0432 0430 043b 044e 0442  .<.8. .2.0.;.N.B
-00011f10: 0430 043c 0438 0020 043d 0435 0020 043f  .0.<.8. .=.5. .?
-00011f20: 043e 0434 0434 0435 0440 0436 0438 0432  .>.4.4.5.@.6.8.2
-00011f30: 0430 0435 0442 0441 044f 003a 0020 0800  .0.5.B.A.O.:. ..
-00011f40: 0000 0006 0000 002d 556e 7375 7070 6f72  .......-Unsuppor
-00011f50: 7465 6420 7472 6164 6520 7769 7468 2064  ted trade with d
-00011f60: 6966 6665 7265 6e74 2063 7572 7265 6e63  ifferent currenc
-00011f70: 6965 733a 2007 0000 000c 5374 6174 656d  ies: .....Statem
-00011f80: 656e 7450 5342 0103 0000 0032 041e 043f  entPSB.....2...?
-00011f90: 0435 0440 0430 0446 0438 0438 0020 0441  .5.@.0.F.8.8. .A
-00011fa0: 0020 0426 0411 0020 0437 0430 0433 0440  . .&... .7.0.3.@
-00011fb0: 0443 0436 0435 043d 044b 003a 0020 0800  .C.6.5.=.K.:. ..
-00011fc0: 0000 0006 0000 0019 4173 7365 7420 6f70  ........Asset op
-00011fd0: 6572 6174 696f 6e73 206c 6f61 6465 643a  erations loaded:
-00011fe0: 2007 0000 000d 5374 6174 656d 656e 7455   .....StatementU
-00011ff0: 4b46 5501 0300 0000 6804 1e04 4204 4104  KFU.....h...B.A.
-00012000: 4304 4204 4104 4204 3204 4304 4e04 4200  C.B.A.B.2.C.N.B.
-00012010: 2004 3e04 3604 3804 3404 3004 3504 3c04   .>.6.8.4.0.5.<.
-00012020: 4b04 3500 2004 3404 3004 3d04 3d04 4b04  K.5. .4.0.=.=.K.
-00012030: 3500 2004 3200 2004 3e04 3f04 3804 4104  5. .2. .>.?.8.A.
-00012040: 3004 3d04 3804 3800 2004 3f04 3504 4004  0.=.8.8. .?.5.@.
-00012050: 3504 3204 3e04 3404 3000 2004 2604 1100  5.2.>.4.0. .&...
-00012060: 2008 0000 0000 0600 0000 2a41 7373 6574   .........*Asset
-00012070: 2074 7261 6e73 6665 7220 6465 7363 7269   transfer descri
-00012080: 7074 696f 6e20 6d69 7373 2073 6f6d 6520  ption miss some 
-00012090: 6461 7461 2007 0000 000d 5374 6174 656d  data .....Statem
-000120a0: 656e 7455 4b46 5501 0300 0000 5004 1d04  entUKFU.....P...
-000120b0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
-000120c0: 3e00 2004 3d04 3004 3904 4204 3800 2004  >. .=.0.9.B.8. .
-000120d0: 3704 3004 3f04 3804 4104 4c00 2004 4104  7.0.?.8.A.L. .A.
-000120e0: 3f04 3804 4104 3004 3d04 3804 4f00 2004  ?.8.A.0.=.8.O. .
-000120f0: 2604 1100 2004 3404 3b04 4f00 2008 0000  &... .4.;.O. ...
-00012100: 0000 0600 0000 2943 616e 2774 2066 696e  ......)Can't fin
-00012110: 6420 6173 7365 7420 6361 6e63 656c 6c61  d asset cancella
-00012120: 7469 6f6e 2072 6563 6f72 6420 666f 7220  tion record for 
-00012130: 0700 0000 0d53 7461 7465 6d65 6e74 554b  .....StatementUK
-00012140: 4655 0103 0000 0046 041d 0435 0432 043e  FU.....F...5.2.>
-00012150: 0437 043c 043e 0436 043d 043e 0020 043d  .7.<.>.6.=.>. .=
-00012160: 0430 0439 0442 0438 0020 0437 0430 0433  .0.9.B.8. .7.0.3
-00012170: 043e 043b 043e 0432 043e 043a 0020 043a  .>.;.>.2.>.:. .:
-00012180: 043e 043c 0438 0441 0441 0438 0439 0800  .>.<.8.A.A.8.9..
-00012190: 0000 0006 0000 001d 4361 6e27 7420 6765  ........Can't ge
-000121a0: 7420 6865 6164 6572 2074 6f20 6669 6e64  t header to find
-000121b0: 2066 6565 7307 0000 000d 5374 6174 656d   fees.....Statem
-000121c0: 656e 7455 4b46 5501 0300 0000 5604 1d04  entUKFU.....V...
-000121d0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
-000121e0: 3e00 2004 4004 3004 4104 3f04 3e04 3704  >. .@.0.A.?.>.7.
-000121f0: 3d04 3004 4204 4c00 2004 3e04 3f04 3804  =.0.B.L. .>.?.8.
-00012200: 4104 3004 3d04 3804 3500 2004 3f04 3504  A.0.=.8.5. .?.5.
-00012210: 4004 3504 3204 3e04 3404 3000 2004 2604  @.5.2.>.4.0. .&.
-00012220: 1100 2008 0000 0000 0600 0000 2743 616e  .. .........'Can
-00012230: 2774 2070 6172 7365 2061 7373 6574 2074  't parse asset t
-00012240: 7261 6e73 6665 7220 6465 7363 7269 7074  ransfer descript
-00012250: 696f 6e20 0700 0000 0d53 7461 7465 6d65  ion .....Stateme
-00012260: 6e74 554b 4655 0103 0000 004c 041d 0435  ntUKFU.....L...5
-00012270: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
-00012280: 0020 0440 0430 0441 043f 043e 0437 043d  . .@.0.A.?.>.7.=
-00012290: 0430 0442 044c 0020 043e 043f 0438 0441  .0.B.L. .>.?.8.A
-000122a0: 0430 043d 0438 0435 0020 043a 0443 043f  .0.=.8.5. .:.C.?
-000122b0: 043e 043d 0430 0020 0800 0000 0006 0000  .>.=.0. ........
-000122c0: 0026 4361 6e27 7420 7061 7273 6520 626f  .&Can't parse bo
-000122d0: 6e64 2069 6e74 6572 6573 7420 6465 7363  nd interest desc
-000122e0: 7269 7074 696f 6e20 0700 0000 0d53 7461  ription .....Sta
-000122f0: 7465 6d65 6e74 554b 4655 0103 0000 0066  tementUKFU.....f
-00012300: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-00012310: 043d 043e 0020 0440 0430 0441 043f 043e  .=.>. .@.0.A.?.>
-00012320: 0437 043d 0430 0442 044c 0020 043e 043f  .7.=.0.B.L. .>.?
-00012330: 0438 0441 0430 043d 0438 0435 0020 043f  .8.A.0.=.8.5. .?
-00012340: 043e 0433 0430 0448 0435 043d 0438 044f  .>.3.0.H.5.=.8.O
-00012350: 0020 043e 0431 043b 0438 0433 0430 0446  . .>.1.;.8.3.0.F
-00012360: 0438 0438 0020 0800 0000 0006 0000 0027  .8.8. .........'
-00012370: 4361 6e27 7420 7061 7273 6520 626f 6e64  Can't parse bond
-00012380: 2072 6570 6179 6d65 6e74 2064 6573 6372   repayment descr
-00012390: 6970 7469 6f6e 2007 0000 000d 5374 6174  iption .....Stat
-000123a0: 656d 656e 7455 4b46 5501 0300 0000 5204  ementUKFU.....R.
-000123b0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
-000123c0: 3d04 3e00 2004 4004 3004 4104 3f04 3e04  =.>. .@.0.A.?.>.
-000123d0: 3704 3d04 3004 4204 4c00 2004 3e04 3f04  7.=.0.B.L. .>.?.
-000123e0: 3804 4104 3004 3d04 3804 3500 2004 3404  8.A.0.=.8.5. .4.
-000123f0: 3804 3204 3804 3404 3504 3d04 3404 3000  8.2.8.4.5.=.4.0.
-00012400: 2008 0000 0000 0600 0000 2143 616e 2774   .........!Can't
-00012410: 2070 6172 7365 2064 6976 6964 656e 6420   parse dividend 
-00012420: 6465 7363 7269 7074 696f 6e20 0700 0000  description ....
-00012430: 0d53 7461 7465 6d65 6e74 554b 4655 0103  .StatementUKFU..
-00012440: 0000 0064 041d 0435 0432 043e 0437 043c  ...d...5.2.>.7.<
-00012450: 043e 0436 043d 043e 0020 0440 0430 0441  .>.6.=.>. .@.0.A
-00012460: 043f 043e 0437 043d 0430 0442 044c 0020  .?.>.7.=.0.B.L. 
-00012470: 043e 043f 0438 0441 0430 043d 0438 0435  .>.?.8.A.0.=.8.5
-00012480: 0020 0434 0435 043d 0435 0436 043d 043e  . .4.5.=.5.6.=.>
-00012490: 0433 043e 0020 043f 0435 0440 0435 0432  .3.>. .?.5.@.5.2
-000124a0: 043e 0434 0430 0020 0800 0000 0006 0000  .>.4.0. ........
-000124b0: 0027 4361 6e27 7420 7061 7273 6520 6d6f  .'Can't parse mo
-000124c0: 6e65 7920 7472 616e 7366 6572 2064 6573  ney transfer des
-000124d0: 6372 6970 7469 6f6e 2007 0000 000d 5374  cription .....St
-000124e0: 6174 656d 656e 7455 4b46 5501 0300 0000  atementUKFU.....
-000124f0: 3a04 1404 3504 3d04 3504 3604 3d04 4b04  :...5.=.5.6.=.K.
-00012500: 4500 2004 3e04 3f04 3504 4004 3004 4604  E. .>.?.5.@.0.F.
-00012510: 3804 3900 2004 3704 3004 3304 4004 4304  8.9. .7.0.3.@.C.
-00012520: 3604 3504 3d04 3e00 3a00 2008 0000 0000  6.5.=.>.:. .....
-00012530: 0600 0000 1843 6173 6820 6f70 6572 6174  .....Cash operat
-00012540: 696f 6e73 206c 6f61 6465 643a 2007 0000  ions loaded: ...
-00012550: 000d 5374 6174 656d 656e 7455 4b46 5501  ..StatementUKFU.
-00012560: 0300 0000 4804 1e04 4804 3804 3104 3a04  ....H...H.8.1.:.
-00012570: 3000 2004 3f04 4004 3800 2004 3a04 3e04  0. .?.@.8. .:.>.
-00012580: 3d04 3204 3504 4004 4204 3004 4604 3804  =.2.5.@.B.0.F.8.
-00012590: 3800 2004 4104 4304 3c04 3c04 4b00 2004  8. .A.C.<.<.K. .
-000125a0: 3d04 3004 3b04 3e04 3304 3000 2008 0000  =.0.;.>.3.0. ...
-000125b0: 0000 0600 0000 1f46 6169 6c65 6420 746f  .......Failed to
-000125c0: 2063 6f6e 7665 7274 2064 6976 6964 656e   convert dividen
-000125d0: 6420 7461 7820 0700 0000 0d53 7461 7465  d tax .....State
-000125e0: 6d65 6e74 554b 4655 0103 0000 003e 0421  mentUKFU.....>.!
-000125f0: 0434 0435 043b 043e 043a 0020 0441 0020  .4.5.;.>.:. .A. 
-00012600: 0444 044c 044e 0447 0435 0440 0441 0430  .D.L.N.G.5.@.A.0
-00012610: 043c 0438 0020 0437 0430 0433 0440 0443  .<.8. .7.0.3.@.C
-00012620: 0436 0435 043d 043e 003a 0020 0800 0000  .6.5.=.>.:. ....
-00012630: 0006 0000 0017 4675 7475 7265 7320 7472  ......Futures tr
-00012640: 6164 6573 206c 6f61 6465 643a 2007 0000  ades loaded: ...
-00012650: 000d 5374 6174 656d 656e 7455 4b46 5501  ..StatementUKFU.
-00012660: 0300 0000 7604 1e04 4204 4104 4304 4204  ....v...B.A.C.B.
-00012670: 4104 4204 3204 4304 4e04 4200 2004 3e04  A.B.2.C.N.B. .>.
-00012680: 3604 3804 3404 3004 3504 3c04 4b04 3500  6.8.4.0.5.<.K.5.
-00012690: 2004 3404 3004 3d04 3d04 4b04 3500 2004   .4.0.=.=.K.5. .
-000126a0: 3200 2004 3e04 3f04 3804 4104 3004 3d04  2. .>.?.8.A.0.=.
-000126b0: 3804 3800 2004 3404 3504 3d04 3504 3604  8.8. .4.5.=.5.6.
-000126c0: 3d04 3e04 3304 3e00 2004 3f04 3504 4004  =.>.3.>. .?.5.@.
-000126d0: 3504 3204 3e04 3404 3000 2008 0000 0000  5.2.>.4.0. .....
-000126e0: 0600 0000 2a4d 6f6e 6579 2074 7261 6e73  ....*Money trans
-000126f0: 6665 7220 6465 7363 7269 7074 696f 6e20  fer description 
-00012700: 6d69 7373 2073 6f6d 6520 6461 7461 2007  miss some data .
-00012710: 0000 000d 5374 6174 656d 656e 7455 4b46  ....StatementUKF
-00012720: 5501 0300 0000 5604 1d04 3004 3904 3404  U.....V...0.9.4.
-00012730: 3504 3d04 4b00 2004 3d04 3504 4104 3a04  5.=.K. .=.5.A.:.
-00012740: 3e04 3b04 4c04 3a04 3e00 2004 3704 3004  >.;.L.:.>. .7.0.
-00012750: 3f04 3804 4104 3504 3900 2004 3f04 3e04  ?.8.A.5.9. .?.>.
-00012760: 3304 3004 4804 3504 3d04 3804 4f00 2004  3.0.H.5.=.8.O. .
-00012770: 2604 1100 2004 3404 3b04 4f00 2008 0000  &... .4.;.O. ...
-00012780: 0000 0600 0000 264d 756c 7469 706c 6520  ......&Multiple 
-00012790: 6173 7365 7420 6361 6e63 656c 6c61 7469  asset cancellati
-000127a0: 6f6e 206d 6174 6368 2066 6f72 2007 0000  on match for ...
-000127b0: 000d 5374 6174 656d 656e 7455 4b46 5501  ..StatementUKFU.
-000127c0: 0300 0000 2404 2104 3404 3504 3b04 3e04  ....$.!.4.5.;.>.
-000127d0: 3a00 2004 3704 3004 3304 4004 4304 3604  :. .7.0.3.@.C.6.
-000127e0: 3504 3d04 3e00 3a00 2008 0000 0000 0600  5.=.>.:. .......
-000127f0: 0000 0f54 7261 6465 7320 6c6f 6164 6564  ...Trades loaded
-00012800: 3a20 0700 0000 0d53 7461 7465 6d65 6e74  : .....Statement
-00012810: 554b 4655 0103 0000 0030 041d 0435 0438  UKFU.....0...5.8
-00012820: 0437 0432 0435 0441 0442 043d 044b 0439  .7.2.5.A.B.=.K.9
-00012830: 0020 0442 0438 043f 0020 0441 0434 0435  . .B.8.?. .A.4.5
-00012840: 043b 043a 0438 003a 0020 0800 0000 0006  .;.:.8.:. ......
-00012850: 0000 0014 556e 6b6e 6f77 6e20 7472 6164  ....Unknown trad
-00012860: 6520 7479 7065 3a20 0700 0000 0d53 7461  e type: .....Sta
-00012870: 7465 6d65 6e74 554b 4655 0103 0000 003e  tementUKFU.....>
-00012880: 041d 0435 043f 043e 0434 0434 0435 0440  ...5.?.>.4.4.5.@
-00012890: 0436 0438 0432 0430 0435 043c 0430 044f  .6.8.2.0.5.<.0.O
-000128a0: 0020 043e 043f 0435 0440 0430 0446 0438  . .>.?.5.@.0.F.8
-000128b0: 044f 0020 0441 0020 0426 0411 0020 0800  .O. .A. .&... ..
-000128c0: 0000 0006 0000 001d 556e 7375 7070 706f  ........Unsupppo
-000128d0: 7274 6564 2061 7373 6574 206f 7065 7261  rted asset opera
-000128e0: 7469 6f6e 2007 0000 000d 5374 6174 656d  tion .....Statem
-000128f0: 656e 7455 4b46 5501 0300 0000 4a04 1d04  entUKFU.....J...
-00012900: 3504 3f04 3e04 3404 3404 3504 4004 3604  5.?.>.4.4.5.@.6.
-00012910: 3804 3204 3004 3504 3c04 3004 4f00 2004  8.2.0.5.<.0.O. .
-00012920: 3404 3504 3d04 3504 3604 3d04 3004 4f00  4.5.=.5.6.=.0.O.
-00012930: 2004 4204 4004 3004 3d04 3704 3004 3a04   .B.@.0.=.7.0.:.
-00012940: 4604 3804 4f00 2008 0000 0000 0600 0000  F.8.O. .........
-00012950: 1e55 6e73 7570 7070 6f72 7465 6420 6361  .Unsuppported ca
-00012960: 7368 2074 7261 6e73 6163 7469 6f6e 2007  sh transaction .
-00012970: 0000 000d 5374 6174 656d 656e 7455 4b46  ....StatementUKF
-00012980: 5501 0300 0000 1e04 2304 4004 3004 3b04  U.......#.@.0.;.
-00012990: 4104 3804 3100 2004 1a04 4d04 3f04 3804  A.8.1. ...M.?.8.
-000129a0: 4204 3004 3b08 0000 0000 0600 0000 0e55  B.0.;..........U
-000129b0: 7261 6c73 6962 2042 726f 6b65 7207 0000  ralsib Broker...
-000129c0: 000d 5374 6174 656d 656e 7455 4b46 5501  ..StatementUKFU.
-000129d0: 0300 0000 4a04 1e04 4204 4704 5104 4200  ....J...B.G.Q.B.
-000129e0: 2004 3104 4004 3e04 3a04 3504 4004 3000   .1.@.>.:.5.@.0.
-000129f0: 2004 2304 4004 3004 3b04 4104 3804 3100   .#.@.0.;.A.8.1.
-00012a00: 2004 1a04 4d04 3f04 3804 4204 3004 3b00   ...M.?.8.B.0.;.
-00012a10: 2000 2800 2a00 2e00 7a00 6900 7000 2908   .(.*...z.i.p.).
-00012a20: 0000 0000 0600 0000 1955 7261 6c73 6962  .........Uralsib
-00012a30: 2073 7461 7465 6d65 6e74 2028 2a2e 7a69   statement (*.zi
-00012a40: 7029 0700 0000 0d53 7461 7465 6d65 6e74  p).....Statement
-00012a50: 554b 4655 0103 0000 003e 0410 0440 0445  UKFU.....>...@.E
-00012a60: 0438 0432 0020 0441 043e 0434 0435 0440  .8.2. .A.>.4.5.@
-00012a70: 0436 0438 0442 0020 043d 0435 0441 043a  .6.8.B. .=.5.A.:
-00012a80: 043e 043b 044c 043a 043e 0020 0444 0430  .>.;.L.:.>. .D.0
-00012a90: 0439 043b 043e 0432 0800 0000 0006 0000  .9.;.>.2........
-00012aa0: 001f 4172 6368 6976 6520 636f 6e74 6169  ..Archive contai
-00012ab0: 6e73 206d 756c 7469 706c 6520 6669 6c65  ns multiple file
-00012ac0: 7307 0000 000c 5374 6174 656d 656e 7458  s.....StatementX
-00012ad0: 4c53 0103 0000 005a 041d 0435 0020 0443  LS.....Z...5. .C
-00012ae0: 0434 0430 043b 043e 0441 044c 0020 043d  .4.0.;.>.A.L. .=
-00012af0: 0430 0439 0442 0438 0020 043e 0436 0438  .0.9.B.8. .>.6.8
-00012b00: 0434 0430 0435 043c 044b 0439 0020 0437  .4.0.5.<.K.9. .7
-00012b10: 0430 0433 043e 043b 043e 0432 043e 043a  .0.3.>.;.>.2.>.:
-00012b20: 0020 043e 0442 0447 0451 0442 0430 003a  . .>.B.G.Q.B.0.:
-00012b30: 0020 0800 0000 0006 0000 0023 4361 6e27  . .........#Can'
-00012b40: 7420 6669 6e64 2065 7870 6563 7465 6420  t find expected 
-00012b50: 7265 706f 7274 2068 6561 6465 723a 2007  report header: .
-00012b60: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
-00012b70: 0103 0000 0066 041d 0435 0020 0443 0434  .....f...5. .C.4
-00012b80: 0430 043b 043e 0441 044c 0020 043e 043f  .0.;.>.A.L. .>.?
-00012b90: 0440 0435 0434 0435 043b 0438 0442 044c  .@.5.4.5.;.8.B.L
-00012ba0: 0020 0432 0430 043b 044e 0442 044b 0020  . .2.0.;.N.B.K. 
-00012bb0: 0438 0437 0020 043e 0431 0449 0435 0439  .8.7. .>.1.I.5.9
-00012bc0: 0020 0441 0435 043a 0446 0438 0438 0020  . .A.5.:.F.8.8. 
-00012bd0: 043e 0442 0447 0451 0442 0430 0800 0000  .>.B.G.Q.B.0....
-00012be0: 0006 0000 0036 4361 6e27 7420 6765 7420  .....6Can't get 
-00012bf0: 6375 7272 656e 6369 6573 2066 726f 6d20  currencies from 
-00012c00: 7375 6d6d 6172 7920 7365 6374 696f 6e20  summary section 
-00012c10: 6f66 2073 7461 7465 6d65 6e74 0700 0000  of statement....
-00012c20: 0c53 7461 7465 6d65 6e74 584c 5301 0300  .StatementXLS...
-00012c30: 0000 4604 1d04 3504 3204 3e04 3704 3c04  ..F...5.2.>.7.<.
-00012c40: 3e04 3604 3d04 3e00 2004 3e04 3f04 4004  >.6.=.>. .>.?.@.
-00012c50: 3504 3404 3504 3b04 3804 4204 4c00 2004  5.4.5.;.8.B.L. .
-00012c60: 3f04 3504 4004 3804 3e04 3400 2004 3e04  ?.5.@.8.>.4. .>.
-00012c70: 4204 4704 5104 4204 3008 0000 0000 0600  B.G.Q.B.0.......
-00012c80: 0000 1843 616e 2774 2072 6561 6420 7265  ...Can't read re
-00012c90: 706f 7274 2070 6572 696f 6407 0000 000c  port period.....
-00012ca0: 5374 6174 656d 656e 7458 4c53 0103 0000  StatementXLS....
-00012cb0: 001c 0414 0421 0020 0437 0430 0433 0440  .....!. .7.0.3.@
-00012cc0: 0443 0436 0435 043d 044b 003a 0020 0800  .C.6.5.=.K.:. ..
-00012cd0: 0000 0006 0000 0016 4361 7368 2062 616c  ........Cash bal
-00012ce0: 616e 6365 7320 6c6f 6164 6564 3a20 0700  ances loaded: ..
-00012cf0: 0000 0c53 7461 7465 6d65 6e74 584c 5301  ...StatementXLS.
-00012d00: 0300 0000 3604 2104 4204 3e04 3b04 3104  ....6.!.B.>.;.1.
-00012d10: 3504 4600 2004 3d04 3500 2004 3d04 3004  5.F. .=.5. .=.0.
-00012d20: 3904 3404 3504 3d00 2004 3200 2004 4104  9.4.5.=. .2. .A.
-00012d30: 3504 3a04 4604 3804 3800 2008 0000 0000  5.:.F.8.8. .....
-00012d40: 0600 0000 1c43 6f6c 756d 6e20 6e6f 7420  .....Column not 
-00012d50: 666f 756e 6420 696e 2073 6563 7469 6f6e  found in section
-00012d60: 2007 0000 000c 5374 6174 656d 656e 7458   .....StatementX
-00012d70: 4c53 0103 0000 0034 041d 0435 0441 043a  LS.....4...5.A.:
-00012d80: 043e 043b 044c 043a 043e 0020 0441 0447  .>.;.L.:.>. .A.G
-00012d90: 0435 0442 043e 0432 0020 043d 0430 0439  .5.B.>.2. .=.0.9
-00012da0: 0434 0435 043d 043e 003a 0020 0800 0000  .4.5.=.>.:. ....
-00012db0: 0006 0000 0019 4d75 6c74 6970 6c65 2061  ......Multiple a
-00012dc0: 6363 6f75 6e74 7320 666f 756e 643a 2007  ccounts found: .
-00012dd0: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
-00012de0: 0103 0000 001c 0426 0411 0020 0437 0430  .......&... .7.0
-00012df0: 0433 0440 0443 0436 0435 043d 044b 003a  .3.@.C.6.5.=.K.:
-00012e00: 0020 0800 0000 0006 0000 0013 5365 6375  . ..........Secu
-00012e10: 7269 7469 6573 206c 6f61 6465 643a 2007  rities loaded: .
-00012e20: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
-00012e30: 0103 0000 0030 041e 0442 0447 0451 0442  .....0...B.G.Q.B
-00012e40: 0020 0437 0430 0433 0440 0443 0436 0435  . .7.0.3.@.C.6.5
-00012e50: 043d 0020 0443 0441 043f 0435 0448 043d  .=. .C.A.?.5.H.=
-00012e60: 043e 003a 0020 0800 0000 0006 0000 001f  .>.:. ..........
-00012e70: 5374 6174 656d 656e 7420 6c6f 6164 6564  Statement loaded
-00012e80: 2073 7563 6365 7373 6675 6c6c 793a 2007   successfully: .
-00012e90: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
-00012ea0: 0103 0000 0022 0020 0437 0430 0433 0440  .....". .7.0.3.@
-00012eb0: 0443 0436 0435 043d 0020 0443 0441 043f  .C.6.5.=. .C.A.?
-00012ec0: 0435 0448 043d 043e 0800 0000 0006 0000  .5.H.=.>........
-00012ed0: 0014 206c 6f61 6465 6420 7375 6363 6573  .. loaded succes
-00012ee0: 7366 756c 6c79 0700 0000 0c53 7461 7465  sfully.....State
-00012ef0: 6d65 6e74 584d 4c01 0300 0000 3604 1d04  mentXML.....6...
-00012f00: 3504 3204 3504 4004 3d04 4b04 3900 2004  5.2.5.@.=.K.9. .
-00012f10: 4404 3e04 4004 3c04 3004 4200 2000 5800  D.>.@.<.0.B. .X.
-00012f20: 4d00 4c00 2004 4404 3004 3904 3b04 3000  M.L. .D.0.9.;.0.
-00012f30: 3a00 2008 0000 0000 0600 0000 1643 616e  :. ..........Can
-00012f40: 2774 2070 6172 7365 2058 4d4c 2066 696c  't parse XML fil
-00012f50: 653a 2007 0000 000c 5374 6174 656d 656e  e: .....Statemen
-00012f60: 7458 4d4c 0103 0000 0044 041d 0435 0432  tXML.....D...5.2
-00012f70: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-00012f80: 0437 0430 0433 0440 0443 0437 0438 0442  .7.0.3.@.C.7.8.B
-00012f90: 044c 0020 043e 0442 0447 0451 0442 0020  .L. .>.B.G.Q.B. 
-00012fa0: 043d 043e 043c 0435 0440 003a 0020 0800  .=.>.<.5.@.:. ..
-00012fb0: 0000 0006 0000 0020 4661 696c 6564 2074  ....... Failed t
-00012fc0: 6f20 6669 6e64 2073 7461 7465 6d65 6e74  o find statement
-00012fd0: 2069 6e64 6578 3a20 0700 0000 0c53 7461   index: .....Sta
-00012fe0: 7465 6d65 6e74 584d 4c01 0300 0000 3e04  tementXML.....>.
-00012ff0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
-00013000: 3d04 3e00 2004 3704 3004 3304 4004 4304  =.>. .7.0.3.@.C.
-00013010: 3704 3804 4204 4c00 2004 3004 4204 4204  7.8.B.L. .0.B.B.
-00013020: 4004 3804 3104 4304 4200 3a00 2008 0000  @.8.1.C.B.:. ...
-00013030: 0000 0600 0000 1a46 6169 6c65 6420 746f  .......Failed to
-00013040: 206c 6f61 6420 6174 7472 6962 7574 653a   load attribute:
-00013050: 2007 0000 000c 5374 6174 656d 656e 7458   .....StatementX
-00013060: 4d4c 0103 0000 0042 041e 0442 0447 0451  ML.....B...B.G.Q
-00013070: 0442 0020 0431 0440 043e 043a 0435 0440  .B. .1.@.>.:.5.@
-00013080: 0430 0020 043d 0435 0020 043d 0430 0439  .0. .=.5. .=.0.9
-00013090: 0434 0435 043d 0020 0432 0020 0444 0430  .4.5.=. .2. .D.0
-000130a0: 0439 043b 0435 003a 0020 0800 0000 0006  .9.;.5.:. ......
-000130b0: 0000 0020 4e6f 2073 7461 7465 6d65 6e74  ... No statement
-000130c0: 2077 6173 2066 6f75 6e64 2069 6e20 6669   was found in fi
-000130d0: 6c65 3a20 0700 0000 0c53 7461 7465 6d65  le: .....Stateme
-000130e0: 6e74 584d 4c01 0300 0000 3404 1d04 3504  ntXML.....4...5.
-000130f0: 3804 3704 3204 3504 4104 4204 3d04 3004  8.7.2.5.A.B.=.0.
-00013100: 4f00 2004 3c04 3504 4204 3a04 3000 2004  O. .<.5.B.:.0. .
-00013110: 3e04 4204 4704 5104 4204 3000 3a00 2008  >.B.G.Q.B.0.:. .
-00013120: 0000 0000 0600 0000 1755 6e6b 6e6f 776e  .........Unknown
-00013130: 2073 7461 7465 6d65 6e74 2074 6167 3a20   statement tag: 
-00013140: 0700 0000 0c53 7461 7465 6d65 6e74 584d  .....StatementXM
-00013150: 4c01 0300 0000 4c04 1d04 3504 3f04 3e04  L.....L...5.?.>.
-00013160: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
-00013170: 3504 3c04 4b04 3900 2004 4404 3e04 4004  5.<.K.9. .D.>.@.
-00013180: 3c04 3004 4200 2004 3404 3004 4204 4b00  <.0.B. .4.0.B.K.
-00013190: 2f04 3204 4004 3504 3c04 3504 3d04 3800  /.2.@.5.<.5.=.8.
-000131a0: 3a00 2008 0000 0000 0600 0000 1e55 6e73  :. ..........Uns
-000131b0: 7570 706f 7274 6564 2064 6174 652f 7469  upported date/ti
-000131c0: 6d65 2066 6f72 6d61 743a 2007 0000 000c  me format: .....
-000131d0: 5374 6174 656d 656e 7458 4d4c 0103 0000  StatementXML....
-000131e0: 0020 041e 0448 0438 0431 043a 0430 0020  . ...H.8.1.:.0. 
-000131f0: 0438 043c 043f 043e 0440 0442 0430 003a  .8.<.?.>.@.B.0.:
-00013200: 0020 0800 0000 0006 0000 000f 496d 706f  . ..........Impo
-00013210: 7274 2066 6169 6c65 643a 2007 0000 000a  rt failed: .....
-00013220: 5374 6174 656d 656e 7473 0103 0000 0040  Statements.....@
-00013230: 0412 044b 0431 0435 0440 0438 0442 0435  ...K.1.5.@.8.B.5
-00013240: 0020 0444 0430 0439 043b 0020 043e 0442  . .D.0.9.;. .>.B
-00013250: 0447 0435 0442 0430 0020 0434 043b 044f  .G.5.B.0. .4.;.O
-00013260: 0020 0438 043c 043f 043e 0440 0442 0430  . .8.<.?.>.@.B.0
-00013270: 0800 0000 0006 0000 001f 5365 6c65 6374  ..........Select
-00013280: 2073 7461 7465 6d65 6e74 2066 696c 6520   statement file 
-00013290: 746f 2069 6d70 6f72 7407 0000 000a 5374  to import.....St
-000132a0: 6174 656d 656e 7473 0103 0000 004a 041a  atements.....J..
-000132b0: 043b 0430 0441 0441 0020 043e 0442 0447  .;.0.A.A. .>.B.G
-000132c0: 0451 0442 0430 0020 043d 0435 0020 043c  .Q.B.0. .=.5. .<
-000132d0: 043e 0436 0435 0442 0020 0431 044b 0442  .>.6.5.B. .1.K.B
-000132e0: 044c 0020 0437 0430 0433 0440 0443 0436  .L. .7.0.3.@.C.6
-000132f0: 0435 043d 003a 0020 0800 0000 0006 0000  .5.=.:. ........
-00013300: 0021 5374 6174 656d 656e 7420 636c 6173  .!Statement clas
-00013310: 7320 6361 6e27 7420 6265 206c 6f61 6465  s can't be loade
-00013320: 643a 2007 0000 000a 5374 6174 656d 656e  d: .....Statemen
-00013330: 7473 0103 0000 0054 041c 043e 0434 0443  ts.....T...>.4.C
-00013340: 043b 044c 0020 043e 0442 0447 0451 0442  .;.L. .>.B.G.Q.B
-00013350: 0430 0020 043d 0435 0020 043c 043e 0436  .0. .=.5. .<.>.6
-00013360: 0435 0442 0020 0431 044b 0442 044c 0020  .5.B. .1.K.B.L. 
-00013370: 0438 043c 043f 043e 0440 0442 0438 0440  .8.<.?.>.@.B.8.@
-00013380: 043e 0432 0430 043d 003a 0020 0800 0000  .>.2.0.=.:. ....
-00013390: 0006 0000 0024 5374 6174 656d 656e 7420  .....$Statement 
-000133a0: 6d6f 6475 6c65 2063 616e 2774 2062 6520  module can't be 
-000133b0: 696d 706f 7274 6564 3a20 0700 0000 0a53  imported: .....S
-000133c0: 7461 7465 6d65 6e74 7301 0300 0000 0804  tatements.......
-000133d0: 1004 3a04 4200 2e08 0000 0000 0600 0000  ..:.B...........
-000133e0: 0441 6374 2e07 0000 0010 5379 6d62 6f6c  .Act......Symbol
-000133f0: 734c 6973 744d 6f64 656c 0103 0000 000c  sListModel......
-00013400: 0412 0430 043b 044e 0442 0430 0800 0000  ...0.;.N.B.0....
-00013410: 0006 0000 0008 4375 7272 656e 6379 0700  ......Currency..
-00013420: 0000 1053 796d 626f 6c73 4c69 7374 4d6f  ...SymbolsListMo
-00013430: 6465 6c01 0300 0000 1004 1e04 3f04 3804  del.........?.8.
-00013440: 4104 3004 3d04 3804 3508 0000 0000 0600  A.0.=.8.5.......
-00013450: 0000 0b44 6573 6372 6970 7469 6f6e 0700  ...Description..
-00013460: 0000 1053 796d 626f 6c73 4c69 7374 4d6f  ...SymbolsListMo
-00013470: 6465 6c01 0300 0000 1204 1a04 3e04 4204  del.........>.B.
-00013480: 3804 4004 3e04 3204 3a04 3808 0000 0000  8.@.>.2.:.8.....
-00013490: 0600 0000 0651 756f 7465 7307 0000 0010  .....Quotes.....
-000134a0: 5379 6d62 6f6c 734c 6973 744d 6f64 656c  SymbolsListModel
-000134b0: 0103 0000 000c 0421 0438 043c 0432 043e  .......!.8.<.2.>
-000134c0: 043b 0800 0000 0006 0000 0006 5379 6d62  .;..........Symb
-000134d0: 6f6c 0700 0000 1053 796d 626f 6c73 4c69  ol.....SymbolsLi
-000134e0: 7374 4d6f 6465 6c01 0300 0000 0604 2204  stModel.......".
-000134f0: 4d04 3308 0000 0000 0600 0000 0354 6167  M.3..........Tag
-00013500: 0700 0000 0c54 6167 4c69 7374 4d6f 6465  .....TagListMode
-00013510: 6c01 0300 0000 1004 1e04 3f04 3504 4004  l.........?.5.@.
-00013520: 3004 4604 3804 3808 0000 0000 0600 0000  0.F.8.8.........
-00013530: 0a4f 7065 7261 7469 6f6e 7307 0000 0009  .Operations.....
-00013540: 5461 6752 6570 6f72 7401 0300 0000 1004  TagReport.......
-00013550: 3f04 3e00 2004 1c04 3504 4204 3a04 3508  ?.>. ...5.B.:.5.
-00013560: 0000 0000 0600 0000 0662 7920 5461 6707  .........by Tag.
-00013570: 0000 0009 5461 6752 6570 6f72 7401 0300  ....TagReport...
-00013580: 0000 1c04 1e04 4204 4704 3504 4200 2004  ......B.G.5.B. .
-00013590: 3f04 3e00 2004 3c04 3504 4204 3a04 3508  ?.>. .<.5.B.:.5.
-000135a0: 0000 0000 0600 0000 0d52 6570 6f72 7420  .........Report 
-000135b0: 6279 2074 6167 0700 0000 0f54 6167 5265  by tag.....TagRe
-000135c0: 706f 7274 5769 6467 6574 0103 0000 000c  portWidget......
-000135d0: 041c 0435 0442 043a 0430 003a 0800 0000  ...5.B.:.0.:....
-000135e0: 0006 0000 0004 5461 673a 0700 0000 0f54  ......Tag:.....T
-000135f0: 6167 5265 706f 7274 5769 6467 6574 0103  agReportWidget..
-00013600: 0000 0024 0027 0020 0437 0430 043c 0435  ...$.'. .7.0.<.5
-00013610: 043d 0435 043d 0430 0020 0443 0441 043f  .=.5.=.0. .C.A.?
-00013620: 0435 0448 043d 043e 0800 0000 0006 0000  .5.H.=.>........
-00013630: 001b 2720 7761 7320 7375 6363 6573 7366  ..' was successf
-00013640: 756c 6c79 2072 6570 6c61 6365 6407 0000  ully replaced...
-00013650: 000e 5461 6773 4c69 7374 4469 616c 6f67  ..TagsListDialog
-00013660: 0103 0000 000c 0027 0020 043d 0430 003a  .......'. .=.0.:
-00013670: 0020 0800 0000 0006 0000 0008 2720 7769  . ..........' wi
-00013680: 7468 3a20 0700 0000 0e54 6167 734c 6973  th: .....TagsLis
-00013690: 7444 6961 6c6f 6701 0300 0000 2004 1704  tDialog..... ...
-000136a0: 3004 3c04 3504 3d04 3804 4204 4c00 2004  0.<.5.=.8.B.L. .
-000136b0: 3c04 3504 4204 3a04 4300 2000 2708 0000  <.5.B.:.C. .'...
-000136c0: 0000 0600 0000 0d52 6570 6c61 6365 2074  .......Replace t
-000136d0: 6167 2027 0700 0000 0e54 6167 734c 6973  ag '.....TagsLis
-000136e0: 7444 6961 6c6f 6701 0300 0000 1c04 1704  tDialog.........
-000136f0: 3004 3c04 3504 3d04 3804 4204 4c00 2004  0.<.5.=.8.B.L. .
-00013700: 3d04 3000 2e00 2e00 2e08 0000 0000 0600  =.0.............
-00013710: 0000 0f52 6570 6c61 6365 2077 6974 682e  ...Replace with.
-00013720: 2e2e 0700 0000 0e54 6167 734c 6973 7444  .......TagsListD
-00013730: 6961 6c6f 6701 0300 0000 3404 1f04 3e04  ialog.....4...>.
-00013740: 3a04 3004 3704 3004 4204 4c00 2004 3e04  :.0.7.0.B.L. .>.
-00013750: 3f04 3504 4004 3004 4604 3804 3800 2004  ?.5.@.0.F.8.8. .
-00013760: 4100 2004 1c04 3504 4204 3a04 3e04 3908  A. ...5.B.:.>.9.
-00013770: 0000 0000 0600 0000 1853 686f 7720 6f70  .........Show op
-00013780: 6572 6174 696f 6e73 2077 6974 6820 5461  erations with Ta
-00013790: 6707 0000 000e 5461 6773 4c69 7374 4469  g.....TagsListDi
-000137a0: 616c 6f67 0103 0000 000e 041c 0435 0442  alog.........5.B
-000137b0: 043a 0430 0020 0027 0800 0000 0006 0000  .:.0. .'........
-000137c0: 0005 5461 6720 2707 0000 000e 5461 6773  ..Tag '.....Tags
-000137d0: 4c69 7374 4469 616c 6f67 0103 0000 0008  ListDialog......
-000137e0: 0422 044d 0433 0438 0800 0000 0006 0000  .".M.3.8........
-000137f0: 0004 5461 6773 0700 0000 0e54 6167 734c  ..Tags.....TagsL
-00013800: 6973 7444 6961 6c6f 6701 0300 0000 1a04  istDialog.......
-00013810: 2204 3504 3a04 4304 4904 3804 3900 2004  ".5.:.C.I.8.9. .
-00013820: 3a04 4304 4004 4100 3a08 0000 0000 0600  :.C.@.A.:.......
-00013830: 0000 0d43 7572 7265 6e74 2072 6174 653a  ...Current rate:
-00013840: 0700 0000 1354 6178 4573 7469 6d61 7469  .....TaxEstimati
-00013850: 6f6e 4469 616c 6f67 0103 0000 0028 041f  onDialog.....(..
-00013860: 043e 0441 043b 0435 0434 043d 044f 044f  .>.A.;.5.4.=.O.O
-00013870: 0020 043a 043e 0442 0438 0440 043e 0432  . .:.>.B.8.@.>.2
-00013880: 043a 0430 003a 0800 0000 0006 0000 000b  .:.0.:..........
-00013890: 4c61 7374 2071 756f 7465 3a07 0000 0013  Last quote:.....
-000138a0: 5461 7845 7374 696d 6174 696f 6e44 6961  TaxEstimationDia
-000138b0: 6c6f 6701 0300 0000 1a04 1e04 4604 3504  log.........F.5.
-000138c0: 3d04 3a04 3000 2004 3d04 3004 3b04 3e04  =.:.0. .=.0.;.>.
-000138d0: 3304 3008 0000 0000 0600 0000 0e54 6178  3.0..........Tax
-000138e0: 2045 7374 696d 6174 696f 6e07 0000 0013   Estimation.....
-000138f0: 5461 7845 7374 696d 6174 696f 6e44 6961  TaxEstimationDia
-00013900: 6c6f 6701 0300 0000 0800 5800 2e00 5800  log.......X...X.
-00013910: 5808 0000 0000 0600 0000 0458 2e58 5807  X..........X.XX.
-00013920: 0000 0013 5461 7845 7374 696d 6174 696f  ....TaxEstimatio
-00013930: 6e44 6961 6c6f 6701 0300 0000 0a04 1804  nDialog.........
-00013940: 2204 1e04 1304 1e08 0000 0000 0600 0000  "...............
-00013950: 0554 4f54 414c 0700 0000 0c54 6178 4573  .TOTAL.....TaxEs
-00013960: 7469 6d61 746f 7201 0300 0000 2404 1e04  timator.....$...
-00013970: 4604 3504 3d04 3a04 3000 2004 3d04 3004  F.5.=.:.0. .=.0.
-00013980: 3b04 3e04 3304 3000 2004 3404 3b04 4f00  ;.>.3.0. .4.;.O.
-00013990: 2008 0000 0000 0600 0000 1354 6178 2065   ..........Tax e
-000139a0: 7374 696d 6174 696f 6e20 666f 7220 0700  stimation for ..
-000139b0: 0000 0c54 6178 4573 7469 6d61 746f 7201  ...TaxEstimator.
-000139c0: 0300 0000 3c04 2104 4204 3004 3204 3a04  ....<.!.B.0.2.:.
-000139d0: 3000 2004 3d04 3004 3b04 3e04 3304 3000  0. .=.0.;.>.3.0.
-000139e0: 2004 3d04 3500 2004 3d04 3004 3904 3404   .=.5. .=.0.9.4.
-000139f0: 3504 3d04 3000 2004 3404 3b04 4f00 3a00  5.=.0. .4.;.O.:.
-00013a00: 2008 0000 0000 0600 0000 1854 6178 2072   ..........Tax r
-00013a10: 6174 6520 6e6f 7420 666f 756e 6420 666f  ate not found fo
-00013a20: 723a 2007 0000 000c 5461 7845 7374 696d  r: .....TaxEstim
-00013a30: 6174 6f72 0103 0000 0008 0414 0430 0442  ator.........0.B
-00013a40: 0430 0800 0000 0006 0000 0004 4461 7465  .0..........Date
-00013a50: 0700 0000 1154 6178 4573 7469 6d61 746f  .....TaxEstimato
-00013a60: 724d 6f64 656c 0103 0000 0014 0426 0435  rModel.......&.5
-00013a70: 043d 0430 0020 043e 0442 043a 0440 002e  .=.0. .>.B.:.@..
-00013a80: 0800 0000 0006 0000 0004 4f70 656e 0700  ..........Open..
-00013a90: 0000 1154 6178 4573 7469 6d61 746f 724d  ...TaxEstimatorM
-00013aa0: 6f64 656c 0103 0000 0012 041f 0440 0438  odel.........@.8
-00013ab0: 0431 044b 043b 044c 002c 0020 0800 0000  .1.K.;.L.,. ....
-00013ac0: 0006 0000 0008 5072 6f66 6974 2c20 0700  ......Profit, ..
-00013ad0: 0000 1154 6178 4573 7469 6d61 746f 724d  ...TaxEstimatorM
-00013ae0: 6f64 656c 0103 0000 000c 041a 043e 043b  odel.........>.;
-00013af0: 002d 0432 043e 0800 0000 0006 0000 0003  .-.2.>..........
-00013b00: 5174 7907 0000 0011 5461 7845 7374 696d  Qty.....TaxEstim
-00013b10: 6174 6f72 4d6f 6465 6c01 0300 0000 0c04  atorModel.......
-00013b20: 1a04 4304 4004 4100 2c00 2008 0000 0000  ..C.@.A.,. .....
-00013b30: 0600 0000 0652 6174 652c 2007 0000 0011  .....Rate, .....
-00013b40: 5461 7845 7374 696d 6174 6f72 4d6f 6465  TaxEstimatorMode
-00013b50: 6c01 0300 0000 0e04 1d04 3004 3b04 3e04  l.........0.;.>.
-00013b60: 3300 2c00 2008 0000 0000 0600 0000 0554  3.,. ..........T
-00013b70: 6178 2c20 0700 0000 1154 6178 4573 7469  ax, .....TaxEsti
-00013b80: 6d61 746f 724d 6f64 656c 0103 0000 0074  matorModel.....t
-00013b90: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-00013ba0: 043d 043e 0020 0437 0430 0433 0440 0443  .=.>. .7.0.3.@.C
-00013bb0: 0437 0438 0442 044c 0020 043f 0430 0440  .7.8.B.L. .?.0.@
-00013bc0: 0430 043c 0435 0442 0440 044b 0020 043d  .0.<.5.B.@.K. .=
-00013bd0: 0430 043b 043e 0433 043e 0432 043e 0433  .0.;.>.3.>.2.>.3
-00013be0: 043e 0020 043e 0442 0447 0451 0442 0430  .>. .>.B.G.Q.B.0
-00013bf0: 0020 0438 0437 0020 0444 0430 0439 043b  . .8.7. .D.0.9.;
-00013c00: 0430 0020 0800 0000 0006 0000 002b 4361  .0. .........+Ca
-00013c10: 6e27 7420 6c6f 6164 2074 6178 2072 6570  n't load tax rep
-00013c20: 6f72 7420 7061 7261 6d65 7465 7273 2066  ort parameters f
-00013c30: 726f 6d20 6669 6c65 2007 0000 0009 5461  rom file .....Ta
-00013c40: 7852 6570 6f72 7401 0300 0000 2804 1d04  xReport.....(...
-00013c50: 3504 3804 3704 3204 3504 4104 4204 3d04  5.8.7.2.5.A.B.=.
-00013c60: 3004 4f00 2004 3204 3004 3b04 4e04 4204  0.O. .2.0.;.N.B.
-00013c70: 3000 3a00 2008 0000 0000 0600 0000 1943  0.:. ..........C
-00013c80: 7572 7265 6e63 7920 6973 206e 6f74 2064  urrency is not d
-00013c90: 6566 696e 6564 3a20 0700 0000 0954 6178  efined: .....Tax
-00013ca0: 5265 706f 7274 0103 0000 004a 041d 0435  Report.....J...5
-00013cb0: 0020 0443 043a 0430 0437 0430 043d 0020  . .C.:.0.7.0.=. 
-00013cc0: 0448 0430 0431 043b 043e 043d 0020 043e  .H.0.1.;.>.=. .>
-00013cd0: 0442 0447 0435 0442 0430 0020 0434 043b  .B.G.5.B.0. .4.;
-00013ce0: 044f 0020 0440 0430 0437 0434 0435 043b  .O. .@.0.7.4.5.;
-00013cf0: 0430 003a 0020 0800 0000 0006 0000 0026  .0.:. .........&
-00013d00: 4e6f 2072 6570 6f72 7420 7465 6d70 6c61  No report templa
-00013d10: 7465 2066 6f75 6e64 2066 6f72 2073 6563  te found for sec
-00013d20: 7469 6f6e 3a20 0700 0000 0954 6178 5265  tion: .....TaxRe
-00013d30: 706f 7274 0103 0000 006a 041d 0435 0442  port.....j...5.B
-00013d40: 0020 0438 043d 0444 043e 0440 043c 0430  . .8.=.D.>.@.<.0
-00013d50: 0446 0438 0438 0020 043e 0020 0421 043e  .F.8.8. .>. .!.>
-00013d60: 0418 0414 041d 0020 0432 0020 043f 0430  ....... .2. .?.0
-00013d70: 0440 0430 043c 0435 0442 0440 0430 0445  .@.0.<.5.B.@.0.E
-00013d80: 0020 043d 0430 043b 043e 0433 043e 0432  . .=.0.;.>.3.>.2
-00013d90: 043e 0433 043e 0020 043e 0442 0447 0451  .>.3.>. .>.B.G.Q
-00013da0: 0442 0430 0800 0000 0006 0000 0042 5468  .B.0.........BTh
-00013db0: 6572 6520 6172 6520 6e6f 2069 6e66 6f72  ere are no infor
-00013dc0: 6d61 7469 6f6e 2061 626f 7574 2074 6178  mation about tax
-00013dd0: 2074 7265 6174 7920 696e 2074 6178 2072   treaty in tax r
-00013de0: 6570 6f72 7420 7061 7261 6d65 7465 7273  eport parameters
-00013df0: 0700 0000 0954 6178 5265 706f 7274 0103  .....TaxReport..
-00013e00: 0000 0060 041d 0435 0020 0437 0430 0434  ...`...5. .7.0.4
-00013e10: 0430 043d 044b 0020 043f 0430 0440 0430  .0.=.K. .?.0.@.0
-00013e20: 043c 0435 0442 0440 044b 0020 043d 0430  .<.5.B.@.K. .=.0
-00013e30: 043b 043e 0433 043e 0432 043e 0433 043e  .;.>.3.>.2.>.3.>
-00013e40: 0020 043e 0442 0447 0451 0442 0430 0020  . .>.B.G.Q.B.0. 
-00013e50: 0434 043b 044f 0020 0433 043e 0434 0430  .4.;.O. .3.>.4.0
-00013e60: 003a 0020 0800 0000 0006 0000 0033 5468  .:. .........3Th
-00013e70: 6572 6520 6172 6520 6e6f 2070 6172 616d  ere are no param
-00013e80: 6574 6572 7320 666f 756e 6420 666f 7220  eters found for 
-00013e90: 7461 7820 7265 706f 7274 2079 6561 723a  tax report year:
-00013ea0: 2007 0000 0009 5461 7852 6570 6f72 7401   .....TaxReport.
-00013eb0: 0300 0000 0a00 2000 2e00 2e00 2e00 2008  ...... ....... .
-00013ec0: 0000 0000 0600 0000 0520 2e2e 2e20 0700  ......... ... ..
-00013ed0: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
-00013ee0: 0006 002e 002e 002e 0800 0000 0006 0000  ................
-00013ef0: 0003 2e2e 2e07 0000 0009 5461 7857 6964  ..........TaxWid
-00013f00: 6765 7401 0300 0000 0a04 2104 4704 3504  get.......!.G.5.
-00013f10: 4200 3a08 0000 0000 0600 0000 0841 6363  B.:..........Acc
-00013f20: 6f75 6e74 3a07 0000 0009 5461 7857 6964  ount:.....TaxWid
-00013f30: 6765 7401 0300 0000 9004 1d04 3804 3604  get.........8.6.
-00013f40: 3500 2004 4004 3004 4104 3f04 3e04 3b04  5. .@.0.A.?.>.;.
-00013f50: 3e04 3604 3504 3d04 4b00 2004 4d04 3a04  >.6.5.=.K. .M.:.
-00013f60: 4104 3f04 3504 4004 3804 3c04 3504 3d04  A.?.5.@.8.<.5.=.
-00013f70: 4204 3004 3b04 4c04 3d04 4b04 3500 2004  B.0.;.L.=.K.5. .
-00013f80: 4404 4304 3d04 3a04 4604 3804 3800 2000  D.C.=.:.F.8.8. .
-00013f90: 2d00 2004 3804 4104 3f04 3e04 3b04 4c04  -. .8.A.?.>.;.L.
-00013fa0: 3704 4304 3904 4204 3500 2004 4100 2004  7.C.9.B.5. .A. .
-00013fb0: 3e04 4104 4204 3e04 4004 3e04 3604 3d04  >.A.B.>.@.>.6.=.
-00013fc0: 3e04 4104 4204 4c04 4e08 0000 0000 0600  >.A.B.L.N.......
-00013fd0: 0000 3342 656c 6f77 2066 756e 6374 696f  ..3Below functio
-00013fe0: 6e73 2061 7265 2065 7870 6572 696d 656e  ns are experimen
-00013ff0: 7461 6c20 2d20 7573 6520 6974 2077 6974  tal - use it wit
-00014000: 6820 6361 7265 0700 0000 0954 6178 5769  h care.....TaxWi
-00014010: 6467 6574 0103 0000 0044 041d 0435 0432  dget.....D...5.2
-00014020: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-00014030: 0437 0430 043f 0438 0441 0430 0442 044c  .7.0.?.8.A.0.B.L
-00014040: 0020 0033 002d 041d 0414 0424 041b 0020  . .3.-.....$... 
-00014050: 0432 0020 0444 0430 0439 043b 0020 0800  .2. .D.0.9.;. ..
-00014060: 0000 0006 0000 001f 4361 6e27 7420 7772  ........Can't wr
-00014070: 6974 6520 7461 7820 666f 726d 2069 6e74  ite tax form int
-00014080: 6f20 6669 6c65 2007 0000 0009 5461 7857  o file .....TaxW
-00014090: 6964 6765 7401 0300 0000 0e04 2104 4204  idget.......!.B.
-000140a0: 4004 3004 3d04 3000 3a08 0000 0000 0600  @.0.=.0.:.......
-000140b0: 0000 0843 6f75 6e74 7279 3a07 0000 0009  ...Country:.....
-000140c0: 5461 7857 6964 6765 7401 0300 0000 7804  TaxWidget.....x.
-000140d0: 2104 3e04 3704 3404 3004 4204 4c00 2004  !.>.7.4.0.B.L. .
-000140e0: 4404 3004 3904 3b00 2000 3300 2d04 1d04  D.0.9.;. .3.-...
-000140f0: 2404 1404 1b00 2004 3200 2004 4404 3e04  $..... .2. .D.>.
-00014100: 4004 3c04 3004 4204 3500 2004 3f04 4004  @.<.0.B.5. .?.@.
-00014110: 3e04 3304 4004 3004 3c04 3c04 4b00 2000  >.3.@.0.<.<.K. .
-00014120: 2204 1404 3504 3a04 3b04 3004 4004 3004  "...5.:.;.0.@.0.
-00014130: 4604 3804 4f00 2200 2000 2800 2a00 2e00  F.8.O.". .(.*...
-00014140: 6400 6300 5800 2908 0000 0000 0600 0000  d.c.X.).........
-00014150: 4043 7265 6174 6520 7461 7820 666f 726d  @Create tax form
-00014160: 2069 6e20 22d0 94d0 b5d0 bad0 bbd0 b0d1   in "...........
-00014170: 80d0 b0d1 86d0 b8d1 8f22 2070 726f 6772  ........." progr
-00014180: 616d 2066 6f72 6d61 7420 282a 2e64 6358  am format (*.dcX
-00014190: 2907 0000 0009 5461 7857 6964 6765 7401  ).....TaxWidget.
-000141a0: 0300 0000 1e04 1404 3004 3d04 3d04 4b04  ........0.=.=.K.
-000141b0: 3500 2004 3d04 3504 3f04 3e04 3b04 3d04  5. .=.5.?.>.;.=.
-000141c0: 4b04 3508 0000 0000 0600 0000 1344 6174  K.5..........Dat
-000141d0: 6120 6172 6520 696e 636f 6d70 6c65 7465  a are incomplete
-000141e0: 0700 0000 0954 6178 5769 6467 6574 0103  .....TaxWidget..
-000141f0: 0000 005c 041d 0435 0020 0438 0441 043f  ...\...5. .8.A.?
-00014200: 043e 043b 044c 0437 043e 0432 0430 0442  .>.;.L.7.>.2.0.B
-00014210: 044c 0020 0434 0430 0442 0443 0020 043f  .L. .4.0.B.C. .?
-00014220: 043e 0441 0442 0430 0432 043a 0438 0020  .>.A.B.0.2.:.8. 
-00014230: 0434 043b 044f 0020 043a 0443 0440 0441  .4.;.O. .:.C.@.A
-00014240: 043e 0432 0020 0432 0430 043b 044e 0442  .>.2. .2.0.;.N.B
-00014250: 0800 0000 0006 0000 002d 446f 206e 6f74  .........-Do not
-00014260: 2075 7365 2073 6574 746c 656d 656e 7420   use settlement 
-00014270: 6461 7465 2066 6f72 2063 7572 7265 6e63  date for currenc
-00014280: 7920 7261 7465 7307 0000 0009 5461 7857  y rates.....TaxW
-00014290: 6964 6765 7401 0300 0000 1604 2404 3004  idget.......$.0.
-000142a0: 3904 3b00 2000 4500 7800 6300 6500 6c00  9.;. .E.x.c.e.l.
-000142b0: 3a08 0000 0000 0600 0000 0b45 7863 656c  :..........Excel
-000142c0: 2066 696c 653a 0700 0000 0954 6178 5769   file:.....TaxWi
-000142d0: 6467 6574 0103 0000 0028 0424 0430 0439  dget.....(.$.0.9
-000142e0: 043b 044b 0020 0045 0078 0063 0065 006c  .;.K. .E.x.c.e.l
-000142f0: 0020 0028 002a 002e 0078 0073 006c 0078  . .(.*...x.s.l.x
-00014300: 0029 0800 0000 0006 0000 0014 4578 6365  .)..........Exce
-00014310: 6c20 6669 6c65 7320 282a 2e78 6c73 7829  l files (*.xlsx)
-00014320: 0700 0000 0954 6178 5769 6467 6574 0103  .....TaxWidget..
-00014330: 0000 004a 0424 0430 0439 043b 0020 0434  ...J.$.0.9.;. .4
-00014340: 043b 044f 0020 0441 043e 0445 0440 0430  .;.O. .A.>.E.@.0
-00014350: 043d 0435 043d 0438 044f 0020 0434 0435  .=.5.=.8.O. .4.5
-00014360: 043a 043b 0430 0440 0430 0446 0438 0438  .:.;.0.@.0.F.8.8
-00014370: 0020 0033 002d 041d 0414 0424 041b 0800  . .3.-.....$....
-00014380: 0000 0006 0000 0024 4669 6c65 2077 6865  .......$File whe
-00014390: 7265 2074 6f20 7374 6f72 6520 7275 7373  re to store russ
-000143a0: 6961 6e20 7461 7820 666f 726d 0700 0000  ian tax form....
-000143b0: 0954 6178 5769 6467 6574 0103 0000 0056  .TaxWidget.....V
-000143c0: 0424 0430 0439 043b 0020 0434 043b 044f  .$.0.9.;. .4.;.O
-000143d0: 0020 0441 043e 0445 0440 0430 043d 0435  . .A.>.E.@.0.=.5
-000143e0: 043d 0438 044f 0020 0440 0430 0441 0447  .=.8.O. .@.0.A.G
-000143f0: 0451 0442 0430 0020 0432 0020 0444 043e  .Q.B.0. .2. .D.>
-00014400: 0440 043c 0430 0442 0435 0020 0045 0078  .@.<.0.B.5. .E.x
-00014410: 0063 0065 006c 0800 0000 0006 0000 002e  .c.e.l..........
-00014420: 4669 6c65 2077 6865 7265 2074 6f20 7374  File where to st
-00014430: 6f72 6520 7461 7820 7265 706f 7274 2069  ore tax report i
-00014440: 6e20 4578 6365 6c20 666f 726d 6174 0700  n Excel format..
-00014450: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
-00014460: 0068 0417 0430 0440 0443 0431 0435 0436  .h...0.@.C.1.5.6
-00014470: 043d 044b 0439 0020 0441 0447 0451 0442  .=.K.9. .A.G.Q.B
-00014480: 0020 0434 043b 044f 0020 043a 043e 0442  . .4.;.O. .:.>.B
-00014490: 043e 0440 043e 0433 043e 0020 043d 0443  .>.@.>.3.>. .=.C
-000144a0: 0436 043d 043e 0020 043f 043e 0434 0433  .6.=.>. .?.>.4.3
-000144b0: 043e 0442 043e 0432 0438 0442 044c 0020  .>.B.>.2.8.B.L. 
-000144c0: 043e 0442 0447 0451 0442 0800 0000 0006  .>.B.G.Q.B......
-000144d0: 0000 0029 466f 7265 6967 6e20 6163 636f  ...)Foreign acco
-000144e0: 756e 7420 746f 2070 7265 7061 7265 2074  unt to prepare t
-000144f0: 6178 2072 6570 6f72 7420 666f 7207 0000  ax report for...
-00014500: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
-00014510: 2604 2404 3004 3904 3b00 2004 4100 2004  &.$.0.9.;. .A. .
-00014520: 4004 3504 3704 4304 3b04 4c04 4204 3004  @.5.7.C.;.L.B.0.
-00014530: 4204 3e04 3c00 3a08 0000 0000 0600 0000  B.>.<.:.........
-00014540: 0c4f 7574 7075 7420 6669 6c65 3a07 0000  .Output file:...
-00014550: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
-00014560: 1e04 2104 3e04 4504 4004 3004 3d04 3804  ..!.>.E.@.0.=.8.
-00014570: 4204 4c00 2004 1e04 4204 4704 5104 4208  B.L. ...B.G.Q.B.
-00014580: 0000 0000 0600 0000 0b53 6176 6520 5265  .........Save Re
-00014590: 706f 7274 0700 0000 0954 6178 5769 6467  port.....TaxWidg
-000145a0: 6574 0103 0000 0026 0421 043e 0445 0440  et.....&.!.>.E.@
-000145b0: 0430 043d 0438 0442 044c 0020 0033 002d  .0.=.8.B.L. .3.-
-000145c0: 041d 0414 0424 041b 0020 0432 003a 0800  .....$... .2.:..
-000145d0: 0000 0006 0000 0011 5361 7665 2074 6178  ........Save tax
-000145e0: 2066 6f72 6d20 746f 3a07 0000 0009 5461   form to:.....Ta
-000145f0: 7857 6964 6765 7401 0300 0000 3804 2104  xWidget.....8.!.
-00014600: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
-00014610: 2004 3d04 3004 3b04 3e04 3304 3e04 3204   .=.0.;.>.3.>.2.
-00014620: 4b04 3900 2004 3e04 4204 4704 5104 4200  K.9. .>.B.G.Q.B.
-00014630: 2004 3200 3a08 0000 0000 0600 0000 1453   .2.:..........S
-00014640: 6176 6520 7461 7820 7265 706f 7274 7320  ave tax reports 
-00014650: 746f 3a07 0000 0009 5461 7857 6964 6765  to:.....TaxWidge
-00014660: 7401 0300 0000 1804 1204 4b04 3104 3504  t.........K.1.5.
-00014670: 4004 3804 4200 2004 4404 3004 3904 3b08  @.8.B. .D.0.9.;.
-00014680: 0000 0000 0600 0000 0b53 656c 6563 7420  .........Select 
-00014690: 6669 6c65 0700 0000 0954 6178 5769 6467  file.....TaxWidg
-000146a0: 6574 0103 0000 0028 041d 0430 043b 043e  et.....(...0.;.>
-000146b0: 0433 043e 0432 044b 0439 0020 043e 0442  .3.>.2.K.9. .>.B
-000146c0: 0447 0451 0442 0020 043f 0443 0441 0442  .G.Q.B. .?.C.A.B
-000146d0: 0800 0000 0006 0000 0013 5461 7820 7265  ..........Tax re
-000146e0: 706f 7274 2069 7320 656d 7074 7907 0000  port is empty...
-000146f0: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
-00014700: 4004 1d04 3004 3b04 3e04 3304 3e04 3204  @...0.;.>.3.>.2.
-00014710: 4b04 3900 2004 3e04 4204 4704 5104 4200  K.9. .>.B.G.Q.B.
-00014720: 2004 4104 3e04 4504 4004 3004 3d04 5104   .A.>.E.@.0.=.Q.
-00014730: 3d00 2004 3200 2004 4404 3004 3904 3b00  =. .2. .D.0.9.;.
-00014740: 2008 0000 0000 0600 0000 1954 6178 2072   ..........Tax r
-00014750: 6570 6f72 7420 7361 7665 6420 746f 2066  eport saved to f
-00014760: 696c 6520 0700 0000 0954 6178 5769 6467  ile .....TaxWidg
-00014770: 6574 0103 0000 0040 041d 0430 043b 043e  et.....@...0.;.>
-00014780: 0433 043e 0432 044b 0439 0020 043e 0442  .3.>.2.K.9. .>.B
-00014790: 0447 0451 0442 0020 0441 043e 0445 0440  .G.Q.B. .A.>.E.@
-000147a0: 0430 043d 0451 043d 0020 0432 0020 0444  .0.=.Q.=. .2. .D
-000147b0: 0430 0439 043b 0020 0800 0000 0006 0000  .0.9.;. ........
-000147c0: 001d 5461 7820 7265 706f 7274 2077 6173  ..Tax report was
-000147d0: 2073 6176 6564 2074 6f20 6669 6c65 2007   saved to file .
-000147e0: 0000 0009 5461 7857 6964 6765 7401 0300  ....TaxWidget...
-000147f0: 0000 0c04 1d04 3004 3b04 3e04 3304 3808  ......0.;.>.3.8.
-00014800: 0000 0000 0600 0000 0554 6178 6573 0700  .........Taxes..
-00014810: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
-00014820: 004e 041e 0431 043d 043e 0432 0438 0442  .N...1.=.>.2.8.B
-00014830: 044c 0020 0442 043e 043b 044c 043a 043e  .L. .B.>.;.L.:.>
-00014840: 0020 0438 043d 0444 043e 0440 043c 0430  . .8.=.D.>.@.<.0
-00014850: 0446 0438 044e 0020 043e 0020 0434 0438  .F.8.N. .>. .4.8
-00014860: 0432 0438 0434 0435 043d 0434 0430 0445  .2.8.4.5.=.4.0.E
-00014870: 0800 0000 0006 0000 0027 5570 6461 7465  .........'Update
-00014880: 206f 6e6c 7920 696e 666f 726d 6174 696f   only informatio
-00014890: 6e20 6162 6f75 7420 6469 7669 6465 6e64  n about dividend
-000148a0: 7307 0000 0009 5461 7857 6964 6765 7401  s.....TaxWidget.
-000148b0: 0300 0000 6404 1804 4104 3f04 3e04 3b04  ....d...A.?.>.;.
-000148c0: 4c04 3704 3e04 3204 3004 4204 4c00 2004  L.7.>.2.0.B.L. .
-000148d0: 3d04 3004 3704 3204 3004 3d04 3804 3500  =.0.7.2.0.=.8.5.
-000148e0: 2004 3104 4004 3e04 3a04 3504 4004 3000   .1.@.>.:.5.@.0.
-000148f0: 2004 3a04 3004 3a00 2004 3804 4104 4204   .:.0.:. .8.A.B.
-00014900: 3e04 4704 3d04 3804 3a00 2004 3204 4b04  >.G.=.8.:. .2.K.
-00014910: 3f04 3b04 3004 4204 4b08 0000 0000 0600  ?.;.0.B.K.......
-00014920: 0000 2055 7365 2062 726f 6b65 7220 6e61  .. Use broker na
-00014930: 6d65 2061 7320 696e 636f 6d65 2073 6f75  me as income sou
-00014940: 7263 6507 0000 0009 5461 7857 6964 6765  rce.....TaxWidge
-00014950: 7401 0300 0000 0804 1304 3e04 3400 3a08  t.........>.4.:.
-00014960: 0000 0000 0600 0000 0559 6561 723a 0700  .........Year:..
-00014970: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
-00014980: 0050 0412 044b 0020 043d 0435 0020 0432  .P...K. .=.5. .2
-00014990: 044b 0431 0440 0430 043b 0438 0020 0441  .K.1.@.0.;.8. .A
-000149a0: 0447 0451 0442 0020 0434 043b 044f 0020  .G.Q.B. .4.;.O. 
-000149b0: 043d 0430 043b 043e 0433 043e 0432 043e  .=.0.;.>.3.>.2.>
-000149c0: 0433 043e 0020 043e 0442 0447 0451 0442  .3.>. .>.B.G.Q.B
-000149d0: 0430 0800 0000 0006 0000 002e 596f 7520  .0..........You 
-000149e0: 6861 7665 6e27 7420 7365 6c65 6374 6564  haven't selected
-000149f0: 2061 6e20 6163 636f 756e 7420 666f 7220   an account for 
-00014a00: 7461 7820 7265 706f 7274 0700 0000 0954  tax report.....T
-00014a10: 6178 5769 6467 6574 0103 0000 0098 041d  axWidget........
-00014a20: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-00014a30: 043e 0020 043e 0431 0440 0430 0431 043e  .>. .>.1.@.0.1.>
-00014a40: 0442 0430 0442 044c 0020 0441 0434 0435  .B.0.B.L. .A.4.5
-00014a50: 043b 043a 0443 002c 0020 0442 002e 043a  .;.:.C.,. .B...:
-00014a60: 002e 0020 043d 0435 0020 0437 0430 0434  ... .=.5. .7.0.4
-00014a70: 0430 043d 0020 0431 0430 043d 043a 0020  .0.=. .1.0.=.:. 
-00014a80: 0434 043b 044f 0020 0438 043d 0432 0435  .4.;.O. .8.=.2.5
-00014a90: 0441 0442 0438 0446 0438 043e 043d 043d  .A.B.8.F.8.>.=.=
-00014aa0: 043e 0433 043e 0020 0441 0447 0451 0442  .>.3.>. .A.G.Q.B
-00014ab0: 0430 003a 0020 0800 0000 0006 0000 003e  .0.:. .........>
-00014ac0: 4361 6e27 7420 7072 6f63 6573 7320 7472  Can't process tr
-00014ad0: 6164 6520 6173 2062 616e 6b20 6973 6e27  ade as bank isn'
-00014ae0: 7420 7365 7420 666f 7220 696e 7665 7374  t set for invest
-00014af0: 6d65 6e74 2061 6363 6f75 6e74 3a20 0700  ment account: ..
-00014b00: 0000 0554 7261 6465 0103 0000 0002 2116  ...Trade......!.
-00014b10: 0800 0000 0006 0000 0001 2307 0000 000b  ..........#.....
-00014b20: 5472 6164 6557 6964 6765 7401 0300 0000  TradeWidget.....
-00014b30: 0804 2104 4704 3504 4208 0000 0000 0600  ..!.G.5.B.......
-00014b40: 0000 0741 6363 6f75 6e74 0700 0000 0b54  ...Account.....T
-00014b50: 7261 6465 5769 6467 6574 0103 0000 0004  radeWidget......
-00014b60: 0426 0411 0800 0000 0006 0000 0005 4173  .&............As
-00014b70: 7365 7407 0000 000b 5472 6164 6557 6964  set.....TradeWid
-00014b80: 6765 7401 0300 0000 2204 1f04 3e04 3a04  get....."...>.:.
-00014b90: 4304 3f04 3a04 3000 2000 2f00 2004 1f04  C.?.:.0. ./. ...
-00014ba0: 4004 3e04 3404 3004 3604 3008 0000 0000  @.>.4.0.6.0.....
-00014bb0: 0600 0000 0a42 7579 202f 2053 656c 6c07  .....Buy / Sell.
-00014bc0: 0000 000b 5472 6164 6557 6964 6765 7401  ....TradeWidget.
-00014bd0: 0300 0000 1404 1404 3004 4204 3000 2f04  ........0.B.0./.
-00014be0: 1204 4004 3504 3c04 4f08 0000 0000 0600  ..@.5.<.O.......
-00014bf0: 0000 0944 6174 652f 5469 6d65 0700 0000  ...Date/Time....
-00014c00: 0b54 7261 6465 5769 6467 6574 0103 0000  .TradeWidget....
-00014c10: 0010 041a 043e 043c 0438 0441 0441 0438  .....>.<.8.A.A.8
-00014c20: 044f 0800 0000 0006 0000 0003 4665 6507  .O..........Fee.
-00014c30: 0000 000b 5472 6164 6557 6964 6765 7401  ....TradeWidget.
-00014c40: 0300 0000 1004 1e04 3f04 3804 4104 3004  ........?.8.A.0.
-00014c50: 3d04 3804 3508 0000 0000 0600 0000 044e  =.8.5..........N
-00014c60: 6f74 6507 0000 000b 5472 6164 6557 6964  ote.....TradeWid
-00014c70: 6765 7401 0300 0000 0804 2604 3504 3d04  get.......&.5.=.
-00014c80: 3008 0000 0000 0600 0000 0550 7269 6365  0..........Price
-00014c90: 0700 0000 0b54 7261 6465 5769 6467 6574  .....TradeWidget
-00014ca0: 0103 0000 000c 041a 043e 043b 002d 0432  .........>.;.-.2
-00014cb0: 043e 0800 0000 0006 0000 0003 5174 7907  .>..........Qty.
-00014cc0: 0000 000b 5472 6164 6557 6964 6765 7401  ....TradeWidget.
-00014cd0: 0300 0000 1a04 1404 3004 4204 3000 2004  ........0.B.0. .
-00014ce0: 4004 3004 4104 4704 3504 4204 3e04 3208  @.0.A.G.5.B.>.2.
-00014cf0: 0000 0000 0600 0000 0a53 6574 746c 656d  .........Settlem
-00014d00: 656e 7407 0000 000b 5472 6164 6557 6964  ent.....TradeWid
-00014d10: 6765 7401 0300 0000 7a04 1a04 3e04 3b04  get.....z...>.;.
-00014d20: 3804 4704 3504 4104 4204 3204 3e00 2004  8.G.5.A.B.2.>. .
-00014d30: 3004 3a04 4204 3804 3204 3000 2004 3d04  0.:.B.8.2.0. .=.
-00014d40: 3504 3404 3e04 4104 4204 3004 4204 3e04  5.4.>.A.B.0.B.>.
-00014d50: 4704 3d04 3e00 2004 3404 3b04 4f00 2004  G.=.>. .4.;.O. .
-00014d60: 3e04 3104 4004 3004 3104 3e04 4204 3a04  >.1.@.0.1.>.B.:.
-00014d70: 3800 2004 3f04 3504 4004 3504 3204 3e04  8. .?.5.@.5.2.>.
-00014d80: 3404 3000 2e00 2004 1404 3004 4204 3000  4.0... ...0.B.0.
-00014d90: 3a00 2008 0000 0000 0600 0000 4041 7373  :. .........@Ass
-00014da0: 6574 2061 6d6f 756e 7420 6973 206e 6f74  et amount is not
-00014db0: 2065 6e6f 7567 6820 666f 7220 6173 7365   enough for asse
-00014dc0: 7420 7472 616e 7366 6572 2070 726f 6365  t transfer proce
-00014dd0: 7373 696e 672e 2044 6174 653a 2007 0000  ssing. Date: ...
-00014de0: 0008 5472 616e 7366 6572 0103 0000 0052  ..Transfer.....R
-00014df0: 0421 043f 0438 0441 0430 043d 0438 0435  .!.?.8.A.0.=.8.5
-00014e00: 0020 0430 043a 0442 0438 0432 0430 0020  . .0.:.B.8.2.0. 
-00014e10: 043d 0435 0020 043d 0430 0439 0434 0435  .=.5. .=.0.9.4.5
-00014e20: 043d 043e 0020 0434 043b 044f 0020 0442  .=.>. .4.;.O. .B
-00014e30: 0440 0430 043d 0441 0444 0435 0440 0430  .@.0.=.A.D.5.@.0
-00014e40: 002e 0800 0000 0006 0000 0028 4173 7365  ...........(Asse
-00014e50: 7420 7769 7468 6472 6177 616c 206e 6f74  t withdrawal not
-00014e60: 2066 6f75 6e64 2066 6f72 2074 7261 6e73   found for trans
-00014e70: 6665 722e 0700 0000 0854 7261 6e73 6665  fer......Transfe
-00014e80: 7201 0300 0000 2e04 1e04 4804 3804 3104  r.........H.8.1.
-00014e90: 3a04 3000 2e00 2004 1a04 4304 4004 4100  :.0... ...C.@.A.
-00014ea0: 2004 4004 3004 3204 3504 3d00 2004 3d04   .@.0.2.5.=. .=.
-00014eb0: 4304 3b04 4e08 0000 0000 0600 0000 1045  C.;.N..........E
-00014ec0: 7272 6f72 2e20 5a65 726f 2072 6174 6507  rror. Zero rate.
-00014ed0: 0000 0008 5472 616e 7366 6572 0103 0000  ....Transfer....
-00014ee0: 0084 041e 0431 0440 0430 0431 043e 0442  .....1.@.0.1.>.B
-00014ef0: 0430 043d 043d 043e 0435 0020 043a 043e  .0.=.=.>.5. .:.>
-00014f00: 043b 0438 0447 0435 0441 0442 0432 043e  .;.8.G.5.A.B.2.>
-00014f10: 0020 043c 0435 043d 044c 0448 0435 002c  . .<.5.=.L.H.5.,
-00014f20: 0020 0447 0435 043c 0020 043a 043e 043b  . .G.5.<. .:.>.;
-00014f30: 0438 0447 0435 0441 0442 0432 043e 0020  .8.G.5.A.B.2.>. 
-00014f40: 0432 0020 0442 0440 0430 043d 0441 0444  .2. .B.@.0.=.A.D
-00014f50: 0435 0440 0435 002e 0020 0414 0430 0442  .5.@.5... ...0.B
-00014f60: 0430 003a 0020 0800 0000 0006 0000 003b  .0.:. .........;
-00014f70: 5072 6f63 6573 7365 6420 6173 7365 7420  Processed asset 
-00014f80: 616d 6f75 6e74 2069 7320 6c65 7373 2074  amount is less t
-00014f90: 6861 6e20 7472 616e 7366 6572 2061 6d6f  han transfer amo
-00014fa0: 756e 742e 2044 6174 653a 2007 0000 0008  unt. Date: .....
-00014fb0: 5472 616e 7366 6572 0103 0000 0002 2116  Transfer......!.
-00014fc0: 0800 0000 0006 0000 0001 2307 0000 000e  ..........#.....
-00014fd0: 5472 616e 7366 6572 5769 6467 6574 0103  TransferWidget..
-00014fe0: 0000 000a 0421 0443 043c 043c 0430 0800  .....!.C.<.<.0..
-00014ff0: 0000 0006 0000 0006 416d 6f75 6e74 0700  ........Amount..
-00015000: 0000 0e54 7261 6e73 6665 7257 6964 6765  ...TransferWidge
-00015010: 7401 0300 0000 0404 2604 1108 0000 0000  t.......&.......
-00015020: 0600 0000 0541 7373 6574 0700 0000 0e54  .....Asset.....T
-00015030: 7261 6e73 6665 7257 6964 6765 7401 0300  ransferWidget...
-00015040: 0000 1404 1404 3004 4204 3000 2f04 1204  ......0.B.0./...
-00015050: 4004 3504 3c04 4f08 0000 0000 0600 0000  @.5.<.O.........
-00015060: 0944 6174 652f 5469 6d65 0700 0000 0e54  .Date/Time.....T
-00015070: 7261 6e73 6665 7257 6964 6765 7401 0300  ransferWidget...
-00015080: 0000 1e04 2004 3004 3704 3c04 3504 4000  .... .0.7.<.5.@.
-00015090: 2004 3a04 3e04 3c04 3804 4104 4104 3804   .:.>.<.8.A.A.8.
-000150a0: 3808 0000 0000 0600 0000 0a46 6565 2061  8..........Fee a
-000150b0: 6d6f 756e 7407 0000 000e 5472 616e 7366  mount.....Transf
-000150c0: 6572 5769 6467 6574 0103 0000 0016 041a  erWidget........
-000150d0: 043e 043c 043c 0438 0441 0441 0438 044f  .>.<.<.8.A.A.8.O
-000150e0: 0020 0441 0800 0000 0006 0000 0008 4665  . .A..........Fe
-000150f0: 6520 6672 6f6d 0700 0000 0e54 7261 6e73  e from.....Trans
-00015100: 6665 7257 6964 6765 7401 0300 0000 0204  ferWidget.......
-00015110: 2108 0000 0000 0600 0000 0446 726f 6d07  !..........From.
-00015120: 0000 000e 5472 616e 7366 6572 5769 6467  ....TransferWidg
-00015130: 6574 0103 0000 0010 041e 043f 0438 0441  et.........?.8.A
-00015140: 0430 043d 0438 0435 0800 0000 0006 0000  .0.=.8.5........
-00015150: 0004 4e6f 7465 0700 0000 0e54 7261 6e73  ..Note.....Trans
-00015160: 6665 7257 6964 6765 7401 0300 0000 0404  ferWidget.......
-00015170: 1d04 3008 0000 0000 0600 0000 0254 6f07  ..0..........To.
-00015180: 0000 000e 5472 616e 7366 6572 5769 6467  ....TransferWidg
-00015190: 6574 0103 0000 000e 041f 0435 0440 0435  et.........5.@.5
-000151a0: 0432 043e 0434 0800 0000 0006 0000 0008  .2.>.4..........
-000151b0: 5472 616e 7366 6572 0700 0000 0e54 7261  Transfer.....Tra
+00010990: 0064 041e 0442 0441 0443 0442 0441 0442  .d...B.A.C.B.A.B
+000109a0: 0432 0443 044e 0442 0020 0434 0430 043d  .2.C.N.B. .4.0.=
+000109b0: 043d 044b 0435 0020 0432 0020 043e 043f  .=.K.5. .2. .>.?
+000109c0: 0438 0441 0430 043d 0438 0438 0020 043f  .8.A.0.=.8.8. .?
+000109d0: 043e 0433 0430 0448 0435 043d 0438 044f  .>.3.0.H.5.=.8.O
+000109e0: 0020 043e 0431 043b 0438 0433 0430 0446  . .>.1.;.8.3.0.F
+000109f0: 0438 0438 0020 0800 0000 0006 0000 002a  .8.8. .........*
+00010a00: 426f 6e64 2072 6570 6179 6d65 6e74 2064  Bond repayment d
+00010a10: 6573 6372 6970 7469 6f6e 206d 6973 7320  escription miss 
+00010a20: 736f 6d65 2064 6174 6120 0700 0000 1353  some data .....S
+00010a30: 7461 7465 6d65 6e74 4f70 656e 4272 6f6b  tatementOpenBrok
+00010a40: 6572 0103 0000 0068 041d 0435 0432 043e  er.....h...5.2.>
+00010a50: 0437 043c 043e 0436 043d 043e 0020 0440  .7.<.>.6.=.>. .@
+00010a60: 0430 0441 043f 043e 0437 043d 0430 0442  .0.A.?.>.7.=.0.B
+00010a70: 044c 0020 043d 0430 0437 0432 0430 043d  .L. .=.0.7.2.0.=
+00010a80: 0438 0435 0020 043e 0431 043b 0438 0433  .8.5. .>.1.;.8.3
+00010a90: 0430 0446 0438 0438 0020 0432 0020 043e  .0.F.8.8. .2. .>
+00010aa0: 043f 0438 0441 0430 043d 0438 0438 0020  .?.8.A.0.=.8.8. 
+00010ab0: 0800 0000 0006 0000 0028 4361 6e27 7420  .........(Can't 
+00010ac0: 6465 7465 6374 2062 6f6e 6420 6e61 6d65  detect bond name
+00010ad0: 2066 726f 6d20 6465 7363 7269 7074 696f   from descriptio
+00010ae0: 6e20 0700 0000 1353 7461 7465 6d65 6e74  n .....Statement
+00010af0: 4f70 656e 4272 6f6b 6572 0103 0000 0062  OpenBroker.....b
+00010b00: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+00010b10: 043d 043e 0020 043e 043f 0440 0435 0434  .=.>. .>.?.@.5.4
+00010b20: 0435 043b 0438 0442 044c 0020 0442 0438  .5.;.8.B.L. .B.8
+00010b30: 043f 002f 043a 043e 043b 0438 0447 0435  .?./.:.>.;.8.G.5
+00010b40: 0441 0442 0432 043e 0020 0434 043b 044f  .A.B.2.>. .4.;.O
+00010b50: 0020 0441 0434 0435 043b 043a 0438 003a  . .A.4.5.;.:.8.:
+00010b60: 0020 0800 0000 0006 0000 0025 4361 6e27  . .........%Can'
+00010b70: 7420 6465 7465 726d 696e 6520 7472 6164  t determine trad
+00010b80: 6520 7479 7065 2f71 7561 6e74 6974 793a  e type/quantity:
+00010b90: 2007 0000 0013 5374 6174 656d 656e 744f   .....StatementO
+00010ba0: 7065 6e42 726f 6b65 7201 0300 0000 6804  penBroker.....h.
+00010bb0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
+00010bc0: 3d04 3e00 2004 3e04 3f04 4004 3504 3404  =.>. .>.?.@.5.4.
+00010bd0: 3504 3b04 3804 4204 4c00 2004 4104 4704  5.;.8.B.L. .A.G.
+00010be0: 5104 4200 2004 3404 3b04 4f00 2004 3404  Q.B. .4.;.O. .4.
+00010bf0: 3504 3d04 3504 3604 3d04 3e04 3900 2004  5.=.5.6.=.>.9. .
+00010c00: 4204 4004 3004 3d04 3704 3004 3a04 4604  B.@.0.=.7.0.:.F.
+00010c10: 3804 3800 3a00 2008 0000 0000 0600 0000  8.8.:. .........
+00010c20: 2743 616e 2774 2066 696e 6420 6163 636f  'Can't find acco
+00010c30: 756e 7420 666f 7220 6361 7368 206f 7065  unt for cash ope
+00010c40: 7261 7469 6f6e 3a20 0700 0000 1353 7461  ration: .....Sta
+00010c50: 7465 6d65 6e74 4f70 656e 4272 6f6b 6572  tementOpenBroker
+00010c60: 0103 0000 0044 041d 0435 0432 043e 0437  .....D...5.2.>.7
+00010c70: 043c 043e 0436 043d 043e 0020 043d 0430  .<.>.6.=.>. .=.0
+00010c80: 0439 0442 0438 0020 0441 0447 0451 0442  .9.B.8. .A.G.Q.B
+00010c90: 0020 0434 043b 044f 0020 0441 0434 0435  . .4.;.O. .A.4.5
+00010ca0: 043b 043a 0438 003a 0020 0800 0000 0006  .;.:.8.:. ......
+00010cb0: 0000 001e 4361 6e27 7420 6669 6e64 2061  ....Can't find a
+00010cc0: 6363 6f75 6e74 2066 6f72 2074 7261 6465  ccount for trade
+00010cd0: 3a20 0700 0000 1353 7461 7465 6d65 6e74  : .....Statement
+00010ce0: 4f70 656e 4272 6f6b 6572 0103 0000 0050  OpenBroker.....P
+00010cf0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+00010d00: 043d 043e 0020 043d 0430 0439 0442 0438  .=.>. .=.0.9.B.8
+00010d10: 0020 0437 0430 043f 0438 0441 044c 0020  . .7.0.?.8.A.L. 
+00010d20: 0441 043f 0438 0441 0430 043d 0438 044f  .A.?.8.A.0.=.8.O
+00010d30: 0020 0426 0411 0020 0434 043b 044f 0020  . .&... .4.;.O. 
+00010d40: 0800 0000 0006 0000 0029 4361 6e27 7420  .........)Can't 
+00010d50: 6669 6e64 2061 7373 6574 2063 616e 6365  find asset cance
+00010d60: 6c6c 6174 696f 6e20 7265 636f 7264 2066  llation record f
+00010d70: 6f72 2007 0000 0013 5374 6174 656d 656e  or .....Statemen
+00010d80: 744f 7065 6e42 726f 6b65 7201 0300 0000  tOpenBroker.....
+00010d90: 3204 1d04 3500 2004 3d04 3004 3904 3404  2...5. .=.0.9.4.
+00010da0: 3504 3d04 3000 2004 2604 1100 2004 3404  5.=.0. .&... .4.
+00010db0: 3b04 4f00 2004 3a04 4304 3f04 3e04 3d04  ;.O. .:.C.?.>.=.
+00010dc0: 3000 2008 0000 0000 0600 0000 2343 616e  0. .........#Can
+00010dd0: 2774 2066 696e 6420 6173 7365 7420 666f  't find asset fo
+00010de0: 7220 626f 6e64 2069 6e74 6572 6573 7420  r bond interest 
+00010df0: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
+00010e00: 656e 4272 6f6b 6572 0103 0000 003c 041d  enBroker.....<..
+00010e10: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
+00010e20: 043e 0020 0441 043e 043f 043e 0441 0442  .>. .A.>.?.>.A.B
+00010e30: 0430 0432 0438 0442 044c 0020 0426 0411  .0.2.8.B.L. .&..
+00010e40: 0020 0434 043b 044f 0020 0800 0000 0006  . .4.;.O. ......
+00010e50: 0000 0016 4361 6e27 7420 6d61 7463 6820  ....Can't match 
+00010e60: 6173 7365 7420 666f 7220 0700 0000 1353  asset for .....S
+00010e70: 7461 7465 6d65 6e74 4f70 656e 4272 6f6b  tatementOpenBrok
+00010e80: 6572 0103 0000 0066 041d 0435 0432 043e  er.....f...5.2.>
+00010e90: 0437 043c 043e 0436 043d 043e 0020 0440  .7.<.>.6.=.>. .@
+00010ea0: 0430 0441 043f 043e 0437 043d 0430 0442  .0.A.?.>.7.=.0.B
+00010eb0: 044c 0020 043e 043f 0438 0441 0430 043d  .L. .>.?.8.A.0.=
+00010ec0: 0438 0435 0020 043f 043e 0433 0430 0448  .8.5. .?.>.3.0.H
+00010ed0: 0435 043d 0438 044f 0020 043e 0431 043b  .5.=.8.O. .>.1.;
+00010ee0: 0438 0433 0430 0446 0438 0438 0020 0800  .8.3.0.F.8.8. ..
+00010ef0: 0000 0006 0000 0024 4361 6e27 7420 7061  .......$Can't pa
+00010f00: 7273 6520 426f 6e64 204d 6174 7572 6520  rse Bond Mature 
+00010f10: 6465 7363 7269 7074 696f 6e20 0700 0000  description ....
+00010f20: 1353 7461 7465 6d65 6e74 4f70 656e 4272  .StatementOpenBr
+00010f30: 6f6b 6572 0103 0000 004c 041d 0435 0432  oker.....L...5.2
+00010f40: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+00010f50: 0440 0430 0441 043f 043e 0437 043d 0430  .@.0.A.?.>.7.=.0
+00010f60: 0442 044c 0020 043e 043f 0438 0441 0430  .B.L. .>.?.8.A.0
+00010f70: 043d 0438 0435 0020 043a 0443 043f 043e  .=.8.5. .:.C.?.>
+00010f80: 043d 0430 0020 0800 0000 0006 0000 0021  .=.0. .........!
+00010f90: 4361 6e27 7420 7061 7273 6520 496e 7465  Can't parse Inte
+00010fa0: 7265 7374 2064 6573 6372 6970 7469 6f6e  rest description
+00010fb0: 2007 0000 0013 5374 6174 656d 656e 744f   .....StatementO
+00010fc0: 7065 6e42 726f 6b65 7201 0300 0000 6604  penBroker.....f.
+00010fd0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
+00010fe0: 3d04 3e00 2004 4004 3004 4104 3f04 3e04  =.>. .@.0.A.?.>.
+00010ff0: 3704 3d04 3004 4204 4c00 2004 3e04 3f04  7.=.0.B.L. .>.?.
+00011000: 3804 4104 3004 3d04 3804 3500 2004 3f04  8.A.0.=.8.5. .?.
+00011010: 3e04 3304 3004 4804 3504 3d04 3804 4f00  >.3.0.H.5.=.8.O.
+00011020: 2004 3e04 3104 3b04 3804 3304 3004 4604   .>.1.;.8.3.0.F.
+00011030: 3804 3800 2008 0000 0000 0600 0000 2743  8.8. .........'C
+00011040: 616e 2774 2070 6172 7365 2062 6f6e 6420  an't parse bond 
+00011050: 7265 7061 796d 656e 7420 6465 7363 7269  repayment descri
+00011060: 7074 696f 6e20 0700 0000 1353 7461 7465  ption .....State
+00011070: 6d65 6e74 4f70 656e 4272 6f6b 6572 0103  mentOpenBroker..
+00011080: 0000 003a 0414 0435 043d 0435 0436 043d  ...:...5.=.5.6.=
+00011090: 044b 0445 0020 043e 043f 0435 0440 0430  .K.E. .>.?.5.@.0
+000110a0: 0446 0438 0439 0020 0437 0430 0433 0440  .F.8.9. .7.0.3.@
+000110b0: 0443 0436 0435 043d 043e 003a 0020 0800  .C.6.5.=.>.:. ..
+000110c0: 0000 0006 0000 0018 4361 7368 206f 7065  ........Cash ope
+000110d0: 7261 7469 6f6e 7320 6c6f 6164 6564 3a20  rations loaded: 
+000110e0: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
+000110f0: 656e 4272 6f6b 6572 0103 0000 0048 041e  enBroker.....H..
+00011100: 0442 0441 0443 0442 0441 0442 0432 0443  .B.A.C.B.A.B.2.C
+00011110: 044e 0442 0020 0434 0430 043d 043d 044b  .N.B. .4.0.=.=.K
+00011120: 0435 0020 0432 0020 043e 043f 0438 0441  .5. .2. .>.?.8.A
+00011130: 0430 043d 0438 0020 043a 0443 043f 043e  .0.=.8. .:.C.?.>
+00011140: 043d 0430 0020 0800 0000 0006 0000 0024  .=.0. .........$
+00011150: 496e 7465 7265 7374 2064 6573 6372 6970  Interest descrip
+00011160: 7469 6f6e 206d 6973 7320 736f 6d65 2064  tion miss some d
+00011170: 6174 6120 0700 0000 1353 7461 7465 6d65  ata .....Stateme
+00011180: 6e74 4f70 656e 4272 6f6b 6572 0103 0000  ntOpenBroker....
+00011190: 0054 0417 0430 0433 0440 0443 0437 043a  .T...0.3.@.C.7.:
+000111a0: 0430 0020 043e 0442 0447 0451 0442 0430  .0. .>.B.G.Q.B.0
+000111b0: 0020 041e 0442 043a 0440 044b 0442 0438  . ...B.:.@.K.B.8
+000111c0: 0435 0020 0431 0440 043e 043a 0435 0440  .5. .1.@.>.:.5.@
+000111d0: 0020 0434 043b 044f 0020 0441 0447 0451  . .4.;.O. .A.G.Q
+000111e0: 0442 0430 0020 0800 0000 0006 0000 0027  .B.0. .........'
+000111f0: 4c6f 6164 204f 7065 6e20 4272 6f6b 6572  Load Open Broker
+00011200: 2073 7461 7465 6d65 6e74 2066 6f72 2061   statement for a
+00011210: 6363 6f75 6e74 2007 0000 0013 5374 6174  ccount .....Stat
+00011220: 656d 656e 744f 7065 6e42 726f 6b65 7201  ementOpenBroker.
+00011230: 0300 0000 5604 1d04 3004 3904 3404 3504  ....V...0.9.4.5.
+00011240: 3d04 4b00 2004 3d04 3504 4104 3a04 3e04  =.K. .=.5.A.:.>.
+00011250: 3b04 4c04 3a04 3e00 2004 3704 3004 3f04  ;.L.:.>. .7.0.?.
+00011260: 3804 4104 3504 3900 2004 3f04 3e04 3304  8.A.5.9. .?.>.3.
+00011270: 3004 4804 3504 3d04 3804 4f00 2004 2604  0.H.5.=.8.O. .&.
+00011280: 1100 2004 3404 3b04 4f00 2008 0000 0000  .. .4.;.O. .....
+00011290: 0600 0000 264d 756c 7469 706c 6520 6173  ....&Multiple as
+000112a0: 7365 7420 6361 6e63 656c 6c61 7469 6f6e  set cancellation
+000112b0: 206d 6174 6368 2066 6f72 2007 0000 0013   match for .....
+000112c0: 5374 6174 656d 656e 744f 7065 6e42 726f  StatementOpenBro
+000112d0: 6b65 7201 0300 0000 7404 1d04 3504 4104  ker.....t...5.A.
+000112e0: 3a04 3e04 3b04 4c04 3a04 3e00 2004 4104  :.>.;.L.:.>. .A.
+000112f0: 3e04 3204 3f04 3004 3404 3504 3d04 3804  >.2.?.0.4.5.=.8.
+00011300: 3900 2004 3404 3b04 4f00 2004 4104 3804  9. .4.;.O. .A.8.
+00011310: 3c04 3204 3e04 3b04 3000 2c00 2004 3804  <.2.>.;.0.,. .8.
+00011320: 4104 3f04 3e04 3b04 4c04 3704 4304 3504  A.?.>.;.L.7.C.5.
+00011330: 3c04 3e04 3304 3e00 2004 3104 4004 3e04  <.>.3.>. .1.@.>.
+00011340: 3a04 3504 4004 3e04 3c00 3a00 2008 0000  :.5.@.>.<.:. ...
+00011350: 0000 0600 0000 224d 756c 7469 706c 6520  ......"Multiple 
+00011360: 6d61 7463 6820 666f 7220 6272 6f6b 6572  match for broker
+00011370: 2073 796d 626f 6c3a 2007 0000 0013 5374   symbol: .....St
+00011380: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
+00011390: 7201 0300 0000 4404 1d04 3504 4104 3a04  r.....D...5.A.:.
+000113a0: 3e04 3b04 4c04 3a04 3e00 2004 4104 3e04  >.;.L.:.>. .A.>.
+000113b0: 3204 3f04 3004 3404 3504 3d04 3804 3900  2.?.0.4.5.=.8.9.
+000113c0: 2004 3404 3b04 4f00 2004 4104 3804 3c04   .4.;.O. .A.8.<.
+000113d0: 3204 3e04 3b04 3000 3a00 2008 0000 0000  2.>.;.0.:. .....
+000113e0: 0600 0000 1b4d 756c 7469 706c 6520 6d61  .....Multiple ma
+000113f0: 7463 6820 666f 7220 7379 6d62 6f6c 3a20  tch for symbol: 
+00011400: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
+00011410: 656e 4272 6f6b 6572 0103 0000 001e 041e  enBroker........
+00011420: 0442 043a 0440 044b 0442 0438 0435 0020  .B.:.@.K.B.8.5. 
+00011430: 0431 0440 043e 043a 0435 0440 0800 0000  .1.@.>.:.5.@....
+00011440: 0006 0000 000b 4f70 656e 2042 726f 6b65  ......Open Broke
+00011450: 7207 0000 0013 5374 6174 656d 656e 744f  r.....StatementO
+00011460: 7065 6e42 726f 6b65 7201 0300 0000 3c04  penBroker.....<.
+00011470: 1e04 4204 4704 5104 4200 2004 3104 4004  ..B.G.Q.B. .1.@.
+00011480: 3e04 3a04 3504 4004 3000 2004 1e04 4204  >.:.5.@.0. ...B.
+00011490: 3a04 4004 4b04 4204 3804 3500 2000 2800  :.@.K.B.8.5. .(.
+000114a0: 2a00 2e00 7800 6d00 6c00 2908 0000 0000  *...x.m.l.).....
+000114b0: 0600 0000 1d4f 7065 6e20 4272 6f6b 6572  .....Open Broker
+000114c0: 2073 7461 7465 6d65 6e74 2028 2a2e 786d   statement (*.xm
+000114d0: 6c29 0700 0000 1353 7461 7465 6d65 6e74  l).....Statement
+000114e0: 4f70 656e 4272 6f6b 6572 0103 0000 0054  OpenBroker.....T
+000114f0: 0417 0430 0433 043e 043b 043e 0432 043e  ...0.3.>.;.>.2.>
+00011500: 043a 0020 043e 0442 0447 0451 0442 0430  .:. .>.B.G.Q.B.0
+00011510: 0020 041e 0442 043a 0440 044b 0442 0438  . ...B.:.@.K.B.8
+00011520: 0435 0020 0431 0440 043e 043a 0435 0440  .5. .1.@.>.:.5.@
+00011530: 0020 043d 0435 0020 043d 0430 0439 0434  . .=.5. .=.0.9.4
+00011540: 0435 043d 0800 0000 0006 0000 0022 4f70  .5.=........."Op
+00011550: 656e 2062 726f 6b65 7220 7265 706f 7274  en broker report
+00011560: 2074 6974 6c65 206e 6f74 2066 6f75 6e64   title not found
+00011570: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
+00011580: 656e 4272 6f6b 6572 0103 0000 0038 041e  enBroker.....8..
+00011590: 043f 0435 0440 0430 0446 0438 044f 0020  .?.5.@.0.F.8.O. 
+000115a0: 043d 0435 0020 043f 043e 0434 0434 0435  .=.5. .?.>.4.4.5
+000115b0: 0440 0436 0438 0432 0430 0435 0442 0441  .@.6.8.2.0.5.B.A
+000115c0: 044f 003a 0020 0800 0000 0006 0000 0019  .O.:. ..........
+000115d0: 4f70 6572 6174 696f 6e20 6e6f 7420 7375  Operation not su
+000115e0: 7070 6f72 7465 643a 2007 0000 0013 5374  pported: .....St
+000115f0: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
+00011600: 7201 0300 0000 1c04 2604 1100 2004 3704  r.......&... .7.
+00011610: 3004 3304 4004 4304 3604 3504 3d04 4b00  0.3.@.C.6.5.=.K.
+00011620: 3a00 2008 0000 0000 0600 0000 1353 6563  :. ..........Sec
+00011630: 7572 6974 6965 7320 6c6f 6164 6564 3a20  urities loaded: 
+00011640: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
+00011650: 656e 4272 6f6b 6572 0103 0000 006e 041d  enBroker.....n..
+00011660: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
+00011670: 0438 0432 0430 0435 043c 044b 0439 0020  .8.2.0.5.<.K.9. 
+00011680: 0437 0430 0433 043e 043b 043e 0432 043e  .7.0.3.>.;.>.2.>
+00011690: 043a 0020 043e 0442 0447 0451 0442 0430  .:. .>.B.G.Q.B.0
+000116a0: 0020 0434 043b 044f 0020 041e 0442 043a  . .4.;.O. ...B.:
+000116b0: 0440 044b 0442 0438 0435 0020 0431 0440  .@.K.B.8.5. .1.@
+000116c0: 043e 043a 0435 0440 003a 0020 0800 0000  .>.:.5.@.:. ....
+000116d0: 0006 0000 0026 556e 6578 7065 6374 6564  .....&Unexpected
+000116e0: 204f 7065 6e20 6272 6f6b 6572 2072 6570   Open broker rep
+000116f0: 6f72 7420 6865 6164 6572 3a20 0700 0000  ort header: ....
+00011700: 1353 7461 7465 6d65 6e74 4f70 656e 4272  .StatementOpenBr
+00011710: 6f6b 6572 0103 0000 0042 041d 0435 0438  oker.....B...5.8
+00011720: 0437 0432 0435 0441 0442 043d 0430 044f  .7.2.5.A.B.=.0.O
+00011730: 0020 043d 0435 0442 043e 0440 0433 043e  . .=.5.B.>.@.3.>
+00011740: 0432 0430 044f 0020 043e 043f 0435 0440  .2.0.O. .>.?.5.@
+00011750: 0430 0446 0438 044f 003a 0020 0800 0000  .0.F.8.O.:. ....
+00011760: 0006 0000 001d 556e 6b6e 6f77 6e20 6e6f  ......Unknown no
+00011770: 6e2d 7472 6164 6520 6f70 6572 6174 696f  n-trade operatio
+00011780: 6e3a 2007 0000 0013 5374 6174 656d 656e  n: .....Statemen
+00011790: 744f 7065 6e42 726f 6b65 7201 0300 0000  tOpenBroker.....
+000117a0: 4604 1d04 3504 3f04 3e04 3404 3404 3504  F...5.?.>.4.4.5.
+000117b0: 4004 3604 3804 3204 3004 3504 3c04 3e04  @.6.8.2.0.5.<.>.
+000117c0: 3500 2004 3e04 3f04 3804 4104 3004 3d04  5. .>.?.8.A.0.=.
+000117d0: 3804 3500 2004 3f04 3b04 3004 4204 3504  8.5. .?.;.0.B.5.
+000117e0: 3604 3000 3a00 2008 0000 0000 0600 0000  6.0.:. .........
+000117f0: 1d55 6e6b 6e6f 776e 2070 6179 6d65 6e74  .Unknown payment
+00011800: 2064 6573 6372 6970 7469 6f6e 3a20 0700   description: ..
+00011810: 0000 1353 7461 7465 6d65 6e74 4f70 656e  ...StatementOpen
+00011820: 4272 6f6b 6572 0103 0000 0032 041d 0435  Broker.....2...5
+00011830: 0438 0437 0432 0435 0441 0442 043d 044b  .8.7.2.5.A.B.=.K
+00011840: 0439 0020 0442 0438 043f 0020 043f 043b  .9. .B.8.?. .?.;
+00011850: 0430 0442 0435 0436 0430 003a 0020 0800  .0.B.5.6.0.:. ..
+00011860: 0000 0006 0000 0016 556e 6b6e 6f77 6e20  ........Unknown 
+00011870: 7061 796d 656e 7420 7479 7065 3a20 0700  payment type: ..
+00011880: 0000 1353 7461 7465 6d65 6e74 4f70 656e  ...StatementOpen
+00011890: 4272 6f6b 6572 0103 0000 0016 0426 0411  Broker.......&..
+000118a0: 0020 0431 0435 0437 0020 0069 0064 003a  . .1.5.7. .i.d.:
+000118b0: 0020 0800 0000 0006 0000 0012 4173 7365  . ..........Asse
+000118c0: 7420 7769 7468 6f75 7420 6964 3a20 0700  t without id: ..
+000118d0: 0000 1653 7461 7465 6d65 6e74 4f70 656e  ...StatementOpen
+000118e0: 506f 7274 666f 6c69 6f01 0300 0000 4804  Portfolio.....H.
+000118f0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
+00011900: 3d04 3e00 2004 3f04 4004 3e04 4704 3804  =.>. .?.@.>.G.8.
+00011910: 4204 3004 4204 4c00 2000 4a00 5300 4f00  B.0.B.L. .J.S.O.
+00011920: 4e00 2004 3804 3700 2004 4404 3004 3904  N. .8.7. .D.0.9.
+00011930: 3b04 3000 3a00 2008 0000 0000 0600 0000  ;.0.:. .........
+00011940: 1f46 6169 6c65 6420 746f 2072 6561 6420  .Failed to read 
+00011950: 4a53 4f4e 2066 726f 6d20 6669 6c65 3a20  JSON from file: 
+00011960: 0700 0000 1653 7461 7465 6d65 6e74 4f70  .....StatementOp
+00011970: 656e 506f 7274 666f 6c69 6f01 0300 0000  enPortfolio.....
+00011980: 3404 1d04 3504 3204 3e04 3704 3c04 3e04  4...5.2.>.7.<.>.
+00011990: 3604 3d04 3e00 2004 3f04 4004 3e04 4704  6.=.>. .?.@.>.G.
+000119a0: 3504 4104 4204 4c00 2004 4404 3004 3904  5.A.B.L. .D.0.9.
+000119b0: 3b00 3a00 2008 0000 0000 0600 0000 1546  ;.:. ..........F
+000119c0: 6169 6c65 6420 746f 2072 6561 6420 6669  ailed to read fi
+000119d0: 6c65 3a20 0700 0000 1653 7461 7465 6d65  le: .....Stateme
+000119e0: 6e74 4f70 656e 506f 7274 666f 6c69 6f01  ntOpenPortfolio.
+000119f0: 0300 0000 2204 1804 3c04 3f04 3e04 4004  ...."...<.?.>.@.
+00011a00: 4204 3804 4004 3e04 3204 3004 3d04 3d04  B.8.@.>.2.0.=.=.
+00011a10: 4b04 3900 2021 1608 0000 0000 0600 0000  K.9. !..........
+00011a20: 0a49 6d70 6f72 7465 6420 2307 0000 0016  .Imported #.....
+00011a30: 5374 6174 656d 656e 744f 7065 6e50 6f72  StatementOpenPor
+00011a40: 7466 6f6c 696f 0103 0000 002e 0049 006e  tfolio.......I.n
+00011a50: 0076 0065 0073 0074 0062 006f 006f 006b  .v.e.s.t.b.o.o.k
+00011a60: 0020 002f 0020 0049 005a 0049 002d 0069  . ./. .I.Z.I.-.i
+00011a70: 006e 0076 0065 0073 0074 0800 0000 0006  .n.v.e.s.t......
+00011a80: 0000 0017 496e 7665 7374 626f 6f6b 202f  ....Investbook /
+00011a90: 2049 5a49 2d49 6e76 6573 7407 0000 0016   IZI-Invest.....
+00011aa0: 5374 6174 656d 656e 744f 7065 6e50 6f72  StatementOpenPor
+00011ab0: 7466 6f6c 696f 0103 0000 0042 041e 0431  tfolio.....B...1
+00011ac0: 044f 0437 0430 0442 0435 043b 044c 043d  .O.7.0.B.5.;.L.=
+00011ad0: 0430 044f 0020 0441 0435 043a 0446 0438  .0.O. .A.5.:.F.8
+00011ae0: 044f 0020 043e 0442 0441 0443 0442 0441  .O. .>.B.A.C.B.A
+00011af0: 0442 0432 0443 0435 0442 003a 0020 0800  .B.2.C.5.B.:. ..
+00011b00: 0000 0006 0000 001e 4d61 6e64 6174 6f72  ........Mandator
+00011b10: 7920 7365 6374 696f 6e20 6973 206d 6973  y section is mis
+00011b20: 7369 6e67 3a20 0700 0000 1653 7461 7465  sing: .....State
+00011b30: 6d65 6e74 4f70 656e 506f 7274 666f 6c69  mentOpenPortfoli
+00011b40: 6f01 0300 0000 2e00 4f00 7000 6500 6e00  o.......O.p.e.n.
+00011b50: 2000 7000 6f00 7200 7400 6600 6f00 6c00   .p.o.r.t.f.o.l.
+00011b60: 6900 6f00 2000 2800 2a00 2e00 6a00 7300  i.o. .(.*...j.s.
+00011b70: 6f00 6e00 2908 0000 0000 0600 0000 174f  o.n.)..........O
+00011b80: 7065 6e20 706f 7274 666f 6c69 6f20 282a  pen portfolio (*
+00011b90: 2e6a 736f 6e29 0700 0000 1653 7461 7465  .json).....State
+00011ba0: 6d65 6e74 4f70 656e 506f 7274 666f 6c69  mentOpenPortfoli
+00011bb0: 6f01 0300 0000 4e04 1d04 3504 3f04 3e04  o.....N...5.?.>.
+00011bc0: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
+00011bd0: 3504 3c04 3004 4f00 2004 3204 3504 4004  5.<.0.O. .2.5.@.
+00011be0: 4104 3804 4f00 2004 4404 3e04 4004 3c04  A.8.O. .D.>.@.<.
+00011bf0: 3004 4204 3000 2004 4404 3004 3904 3b04  0.B.0. .D.0.9.;.
+00011c00: 3000 3a00 2008 0000 0000 0600 0000 2e55  0.:. ..........U
+00011c10: 6e73 7570 706f 7274 6564 2076 6572 7369  nsupported versi
+00011c20: 6f6e 206f 6620 6f70 656e 2070 6f72 7466  on of open portf
+00011c30: 6f6c 696f 2066 6f72 6d61 743a 2007 0000  olio format: ...
+00011c40: 0016 5374 6174 656d 656e 744f 7065 6e50  ..StatementOpenP
+00011c50: 6f72 7466 6f6c 696f 0103 0000 0038 041a  ortfolio.....8..
+00011c60: 0443 043f 043e 043d 044b 0020 043e 0431  .C.?.>.=.K. .>.1
+00011c70: 043b 0438 0433 0430 0446 0438 0439 0020  .;.8.3.0.F.8.9. 
+00011c80: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
+00011c90: 044b 003a 0020 0800 0000 0006 0000 0017  .K.:. ..........
+00011ca0: 426f 6e64 2069 6e74 6572 6573 7473 206c  Bond interests l
+00011cb0: 6f61 6465 643a 2007 0000 000c 5374 6174  oaded: .....Stat
+00011cc0: 656d 656e 7450 5342 0103 0000 003e 0414  ementPSB.....>..
+00011cd0: 0435 043d 0435 0436 043d 044b 0435 0020  .5.=.5.6.=.K.5. 
+00011ce0: 0442 0440 0430 043d 0437 0430 043a 0446  .B.@.0.=.7.0.:.F
+00011cf0: 0438 0438 0020 0437 0430 0433 0440 0443  .8.8. .7.0.3.@.C
+00011d00: 0436 0435 043d 044b 003a 0020 0800 0000  .6.5.=.K.:. ....
+00011d10: 0006 0000 001a 4361 7368 2074 7261 6e73  ......Cash trans
+00011d20: 6163 7469 6f6e 7320 6c6f 6164 6564 3a20  actions loaded: 
+00011d30: 0700 0000 0c53 7461 7465 6d65 6e74 5053  .....StatementPS
+00011d40: 4201 0300 0000 2a04 1404 3804 3204 3804  B.....*...8.2.8.
+00011d50: 3404 3504 3d04 3404 4b00 2004 3704 3004  4.5.=.4.K. .7.0.
+00011d60: 3304 4004 4304 3604 3504 3d04 4b00 3a00  3.@.C.6.5.=.K.:.
+00011d70: 2008 0000 0000 0600 0000 1244 6976 6964   ..........Divid
+00011d80: 656e 6473 206c 6f61 6465 643a 2007 0000  ends loaded: ...
+00011d90: 000c 5374 6174 656d 656e 7450 5342 0103  ..StatementPSB..
+00011da0: 0000 0014 041f 0421 0411 002d 0431 0440  .......!...-.1.@
+00011db0: 043e 043a 0435 0440 0800 0000 0006 0000  .>.:.5.@........
+00011dc0: 000a 5053 4220 4272 6f6b 6572 0700 0000  ..PSB Broker....
+00011dd0: 0c53 7461 7465 6d65 6e74 5053 4201 0300  .StatementPSB...
+00011de0: 0000 4004 1e04 4204 4704 5104 4200 2004  ..@...B.G.Q.B. .
+00011df0: 3104 4004 3e04 3a04 3504 4004 3000 2004  1.@.>.:.5.@.0. .
+00011e00: 1f04 2104 1100 2000 2800 2a00 2e00 7800  ..!... .(.*...x.
+00011e10: 6c00 7300 7800 2000 2a00 2e00 7800 6c00  l.s.x. .*...x.l.
+00011e20: 7300 2908 0000 0000 0600 0000 2350 5342  s.).........#PSB
+00011e30: 2062 726f 6b65 7220 7374 6174 656d 656e   broker statemen
+00011e40: 7420 282a 2e78 6c73 7820 2a2e 786c 7329  t (*.xlsx *.xls)
+00011e50: 0700 0000 0c53 7461 7465 6d65 6e74 5053  .....StatementPS
+00011e60: 4201 03ff ffff ff08 0000 0000 0600 0000  B...............
+00011e70: 0f54 7261 6465 7320 6c6f 6164 6564 3a20  .Trades loaded: 
+00011e80: 0700 0000 0c53 7461 7465 6d65 6e74 5053  .....StatementPS
+00011e90: 4201 0300 0000 4004 1d04 3504 3f04 3e04  B.....@...5.?.>.
+00011ea0: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
+00011eb0: 3504 3c04 3004 4f00 2004 3e04 3f04 3504  5.<.0.O. .>.?.5.
+00011ec0: 4004 3004 4604 3804 4f00 2004 4100 2004  @.0.F.8.O. .A. .
+00011ed0: 1404 2100 3a00 2008 0000 0000 0600 0000  ..!.:. .........
+00011ee0: 1855 6e6b 6e6f 776e 2063 6173 6820 6f70  .Unknown cash op
+00011ef0: 6572 6174 696f 6e3a 2007 0000 000c 5374  eration: .....St
+00011f00: 6174 656d 656e 7450 5342 0103 0000 003a  atementPSB.....:
+00011f10: 041d 0435 0438 0437 0432 0435 0441 0442  ...5.8.7.2.5.A.B
+00011f20: 043d 044b 0439 0020 0442 0438 043f 0020  .=.K.9. .B.8.?. 
+00011f30: 0434 0432 0438 0436 0435 043d 0438 044f  .4.2.8.6.5.=.8.O
+00011f40: 0020 0414 0421 003a 0020 0800 0000 0006  . ...!.:. ......
+00011f50: 0000 001a 556e 6b6e 6f77 6e20 6361 7368  ....Unknown cash
+00011f60: 2074 7261 6e73 6163 7469 6f6e 3a20 0700   transaction: ..
+00011f70: 0000 0c53 7461 7465 6d65 6e74 5053 4201  ...StatementPSB.
+00011f80: 0300 0000 3004 1d04 3504 3804 3704 3204  ....0...5.8.7.2.
+00011f90: 3504 4104 4204 3d04 4b04 3900 2004 4204  5.A.B.=.K.9. .B.
+00011fa0: 3804 3f00 2004 4104 3404 3504 3b04 3a04  8.?. .A.4.5.;.:.
+00011fb0: 3800 3a00 2008 0000 0000 0600 0000 1455  8.:. ..........U
+00011fc0: 6e6b 6e6f 776e 2074 7261 6465 2074 7970  nknown trade typ
+00011fd0: 653a 2007 0000 000c 5374 6174 656d 656e  e: .....Statemen
+00011fe0: 7450 5342 0103 0000 0032 041d 0435 043f  tPSB.....2...5.?
+00011ff0: 043e 0434 0434 0435 0440 0436 0438 0432  .>.4.4.5.@.6.8.2
+00012000: 0430 0435 043c 044b 0439 0020 043f 043b  .0.5.<.K.9. .?.;
+00012010: 0430 0442 0451 0436 003a 0020 0800 0000  .0.B.Q.6.:. ....
+00012020: 0006 0000 0015 556e 7375 7070 6f72 7465  ......Unsupporte
+00012030: 6420 7061 796d 656e 743a 2007 0000 000c  d payment: .....
+00012040: 5374 6174 656d 656e 7450 5342 0103 0000  StatementPSB....
+00012050: 005a 0421 0434 0435 043b 043a 0430 0020  .Z.!.4.5.;.:.0. 
+00012060: 0441 0020 0440 0430 0437 043d 044b 043c  .A. .@.0.7.=.K.<
+00012070: 0438 0020 0432 0430 043b 044e 0442 0430  .8. .2.0.;.N.B.0
+00012080: 043c 0438 0020 043d 0435 0020 043f 043e  .<.8. .=.5. .?.>
+00012090: 0434 0434 0435 0440 0436 0438 0432 0430  .4.4.5.@.6.8.2.0
+000120a0: 0435 0442 0441 044f 003a 0020 0800 0000  .5.B.A.O.:. ....
+000120b0: 0006 0000 002d 556e 7375 7070 6f72 7465  .....-Unsupporte
+000120c0: 6420 7472 6164 6520 7769 7468 2064 6966  d trade with dif
+000120d0: 6665 7265 6e74 2063 7572 7265 6e63 6965  ferent currencie
+000120e0: 733a 2007 0000 000c 5374 6174 656d 656e  s: .....Statemen
+000120f0: 7450 5342 0103 0000 0032 041e 043f 0435  tPSB.....2...?.5
+00012100: 0440 0430 0446 0438 0438 0020 0441 0020  .@.0.F.8.8. .A. 
+00012110: 0426 0411 0020 0437 0430 0433 0440 0443  .&... .7.0.3.@.C
+00012120: 0436 0435 043d 044b 003a 0020 0800 0000  .6.5.=.K.:. ....
+00012130: 0006 0000 0019 4173 7365 7420 6f70 6572  ......Asset oper
+00012140: 6174 696f 6e73 206c 6f61 6465 643a 2007  ations loaded: .
+00012150: 0000 000d 5374 6174 656d 656e 7455 4b46  ....StatementUKF
+00012160: 5501 0300 0000 6804 1e04 4204 4104 4304  U.....h...B.A.C.
+00012170: 4204 4104 4204 3204 4304 4e04 4200 2004  B.A.B.2.C.N.B. .
+00012180: 3e04 3604 3804 3404 3004 3504 3c04 4b04  >.6.8.4.0.5.<.K.
+00012190: 3500 2004 3404 3004 3d04 3d04 4b04 3500  5. .4.0.=.=.K.5.
+000121a0: 2004 3200 2004 3e04 3f04 3804 4104 3004   .2. .>.?.8.A.0.
+000121b0: 3d04 3804 3800 2004 3f04 3504 4004 3504  =.8.8. .?.5.@.5.
+000121c0: 3204 3e04 3404 3000 2004 2604 1100 2008  2.>.4.0. .&... .
+000121d0: 0000 0000 0600 0000 2a41 7373 6574 2074  ........*Asset t
+000121e0: 7261 6e73 6665 7220 6465 7363 7269 7074  ransfer descript
+000121f0: 696f 6e20 6d69 7373 2073 6f6d 6520 6461  ion miss some da
+00012200: 7461 2007 0000 000d 5374 6174 656d 656e  ta .....Statemen
+00012210: 7455 4b46 5501 0300 0000 5004 1d04 3504  tUKFU.....P...5.
+00012220: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
+00012230: 2004 3d04 3004 3904 4204 3800 2004 3704   .=.0.9.B.8. .7.
+00012240: 3004 3f04 3804 4104 4c00 2004 4104 3f04  0.?.8.A.L. .A.?.
+00012250: 3804 4104 3004 3d04 3804 4f00 2004 2604  8.A.0.=.8.O. .&.
+00012260: 1100 2004 3404 3b04 4f00 2008 0000 0000  .. .4.;.O. .....
+00012270: 0600 0000 2943 616e 2774 2066 696e 6420  ....)Can't find 
+00012280: 6173 7365 7420 6361 6e63 656c 6c61 7469  asset cancellati
+00012290: 6f6e 2072 6563 6f72 6420 666f 7220 0700  on record for ..
+000122a0: 0000 0d53 7461 7465 6d65 6e74 554b 4655  ...StatementUKFU
+000122b0: 0103 0000 0046 041d 0435 0432 043e 0437  .....F...5.2.>.7
+000122c0: 043c 043e 0436 043d 043e 0020 043d 0430  .<.>.6.=.>. .=.0
+000122d0: 0439 0442 0438 0020 0437 0430 0433 043e  .9.B.8. .7.0.3.>
+000122e0: 043b 043e 0432 043e 043a 0020 043a 043e  .;.>.2.>.:. .:.>
+000122f0: 043c 0438 0441 0441 0438 0439 0800 0000  .<.8.A.A.8.9....
+00012300: 0006 0000 001d 4361 6e27 7420 6765 7420  ......Can't get 
+00012310: 6865 6164 6572 2074 6f20 6669 6e64 2066  header to find f
+00012320: 6565 7307 0000 000d 5374 6174 656d 656e  ees.....Statemen
+00012330: 7455 4b46 5501 0300 0000 5604 1d04 3504  tUKFU.....V...5.
+00012340: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
+00012350: 2004 4004 3004 4104 3f04 3e04 3704 3d04   .@.0.A.?.>.7.=.
+00012360: 3004 4204 4c00 2004 3e04 3f04 3804 4104  0.B.L. .>.?.8.A.
+00012370: 3004 3d04 3804 3500 2004 3f04 3504 4004  0.=.8.5. .?.5.@.
+00012380: 3504 3204 3e04 3404 3000 2004 2604 1100  5.2.>.4.0. .&...
+00012390: 2008 0000 0000 0600 0000 2743 616e 2774   .........'Can't
+000123a0: 2070 6172 7365 2061 7373 6574 2074 7261   parse asset tra
+000123b0: 6e73 6665 7220 6465 7363 7269 7074 696f  nsfer descriptio
+000123c0: 6e20 0700 0000 0d53 7461 7465 6d65 6e74  n .....Statement
+000123d0: 554b 4655 0103 0000 004c 041d 0435 0432  UKFU.....L...5.2
+000123e0: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+000123f0: 0440 0430 0441 043f 043e 0437 043d 0430  .@.0.A.?.>.7.=.0
+00012400: 0442 044c 0020 043e 043f 0438 0441 0430  .B.L. .>.?.8.A.0
+00012410: 043d 0438 0435 0020 043a 0443 043f 043e  .=.8.5. .:.C.?.>
+00012420: 043d 0430 0020 0800 0000 0006 0000 0026  .=.0. .........&
+00012430: 4361 6e27 7420 7061 7273 6520 626f 6e64  Can't parse bond
+00012440: 2069 6e74 6572 6573 7420 6465 7363 7269   interest descri
+00012450: 7074 696f 6e20 0700 0000 0d53 7461 7465  ption .....State
+00012460: 6d65 6e74 554b 4655 0103 0000 0066 041d  mentUKFU.....f..
+00012470: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
+00012480: 043e 0020 0440 0430 0441 043f 043e 0437  .>. .@.0.A.?.>.7
+00012490: 043d 0430 0442 044c 0020 043e 043f 0438  .=.0.B.L. .>.?.8
+000124a0: 0441 0430 043d 0438 0435 0020 043f 043e  .A.0.=.8.5. .?.>
+000124b0: 0433 0430 0448 0435 043d 0438 044f 0020  .3.0.H.5.=.8.O. 
+000124c0: 043e 0431 043b 0438 0433 0430 0446 0438  .>.1.;.8.3.0.F.8
+000124d0: 0438 0020 0800 0000 0006 0000 0027 4361  .8. .........'Ca
+000124e0: 6e27 7420 7061 7273 6520 626f 6e64 2072  n't parse bond r
+000124f0: 6570 6179 6d65 6e74 2064 6573 6372 6970  epayment descrip
+00012500: 7469 6f6e 2007 0000 000d 5374 6174 656d  tion .....Statem
+00012510: 656e 7455 4b46 5501 0300 0000 5204 1d04  entUKFU.....R...
+00012520: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
+00012530: 3e00 2004 4004 3004 4104 3f04 3e04 3704  >. .@.0.A.?.>.7.
+00012540: 3d04 3004 4204 4c00 2004 3e04 3f04 3804  =.0.B.L. .>.?.8.
+00012550: 4104 3004 3d04 3804 3500 2004 3404 3804  A.0.=.8.5. .4.8.
+00012560: 3204 3804 3404 3504 3d04 3404 3000 2008  2.8.4.5.=.4.0. .
+00012570: 0000 0000 0600 0000 2143 616e 2774 2070  ........!Can't p
+00012580: 6172 7365 2064 6976 6964 656e 6420 6465  arse dividend de
+00012590: 7363 7269 7074 696f 6e20 0700 0000 0d53  scription .....S
+000125a0: 7461 7465 6d65 6e74 554b 4655 0103 0000  tatementUKFU....
+000125b0: 0064 041d 0435 0432 043e 0437 043c 043e  .d...5.2.>.7.<.>
+000125c0: 0436 043d 043e 0020 0440 0430 0441 043f  .6.=.>. .@.0.A.?
+000125d0: 043e 0437 043d 0430 0442 044c 0020 043e  .>.7.=.0.B.L. .>
+000125e0: 043f 0438 0441 0430 043d 0438 0435 0020  .?.8.A.0.=.8.5. 
+000125f0: 0434 0435 043d 0435 0436 043d 043e 0433  .4.5.=.5.6.=.>.3
+00012600: 043e 0020 043f 0435 0440 0435 0432 043e  .>. .?.5.@.5.2.>
+00012610: 0434 0430 0020 0800 0000 0006 0000 0027  .4.0. .........'
+00012620: 4361 6e27 7420 7061 7273 6520 6d6f 6e65  Can't parse mone
+00012630: 7920 7472 616e 7366 6572 2064 6573 6372  y transfer descr
+00012640: 6970 7469 6f6e 2007 0000 000d 5374 6174  iption .....Stat
+00012650: 656d 656e 7455 4b46 5501 0300 0000 3a04  ementUKFU.....:.
+00012660: 1404 3504 3d04 3504 3604 3d04 4b04 4500  ..5.=.5.6.=.K.E.
+00012670: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
+00012680: 3900 2004 3704 3004 3304 4004 4304 3604  9. .7.0.3.@.C.6.
+00012690: 3504 3d04 3e00 3a00 2008 0000 0000 0600  5.=.>.:. .......
+000126a0: 0000 1843 6173 6820 6f70 6572 6174 696f  ...Cash operatio
+000126b0: 6e73 206c 6f61 6465 643a 2007 0000 000d  ns loaded: .....
+000126c0: 5374 6174 656d 656e 7455 4b46 5501 0300  StatementUKFU...
+000126d0: 0000 4804 1e04 4804 3804 3104 3a04 3000  ..H...H.8.1.:.0.
+000126e0: 2004 3f04 4004 3800 2004 3a04 3e04 3d04   .?.@.8. .:.>.=.
+000126f0: 3204 3504 4004 4204 3004 4604 3804 3800  2.5.@.B.0.F.8.8.
+00012700: 2004 4104 4304 3c04 3c04 4b00 2004 3d04   .A.C.<.<.K. .=.
+00012710: 3004 3b04 3e04 3304 3000 2008 0000 0000  0.;.>.3.0. .....
+00012720: 0600 0000 1f46 6169 6c65 6420 746f 2063  .....Failed to c
+00012730: 6f6e 7665 7274 2064 6976 6964 656e 6420  onvert dividend 
+00012740: 7461 7820 0700 0000 0d53 7461 7465 6d65  tax .....Stateme
+00012750: 6e74 554b 4655 0103 0000 003e 0421 0434  ntUKFU.....>.!.4
+00012760: 0435 043b 043e 043a 0020 0441 0020 0444  .5.;.>.:. .A. .D
+00012770: 044c 044e 0447 0435 0440 0441 0430 043c  .L.N.G.5.@.A.0.<
+00012780: 0438 0020 0437 0430 0433 0440 0443 0436  .8. .7.0.3.@.C.6
+00012790: 0435 043d 043e 003a 0020 0800 0000 0006  .5.=.>.:. ......
+000127a0: 0000 0017 4675 7475 7265 7320 7472 6164  ....Futures trad
+000127b0: 6573 206c 6f61 6465 643a 2007 0000 000d  es loaded: .....
+000127c0: 5374 6174 656d 656e 7455 4b46 5501 0300  StatementUKFU...
+000127d0: 0000 7604 1e04 4204 4104 4304 4204 4104  ..v...B.A.C.B.A.
+000127e0: 4204 3204 4304 4e04 4200 2004 3e04 3604  B.2.C.N.B. .>.6.
+000127f0: 3804 3404 3004 3504 3c04 4b04 3500 2004  8.4.0.5.<.K.5. .
+00012800: 3404 3004 3d04 3d04 4b04 3500 2004 3200  4.0.=.=.K.5. .2.
+00012810: 2004 3e04 3f04 3804 4104 3004 3d04 3804   .>.?.8.A.0.=.8.
+00012820: 3800 2004 3404 3504 3d04 3504 3604 3d04  8. .4.5.=.5.6.=.
+00012830: 3e04 3304 3e00 2004 3f04 3504 4004 3504  >.3.>. .?.5.@.5.
+00012840: 3204 3e04 3404 3000 2008 0000 0000 0600  2.>.4.0. .......
+00012850: 0000 2a4d 6f6e 6579 2074 7261 6e73 6665  ..*Money transfe
+00012860: 7220 6465 7363 7269 7074 696f 6e20 6d69  r description mi
+00012870: 7373 2073 6f6d 6520 6461 7461 2007 0000  ss some data ...
+00012880: 000d 5374 6174 656d 656e 7455 4b46 5501  ..StatementUKFU.
+00012890: 0300 0000 5604 1d04 3004 3904 3404 3504  ....V...0.9.4.5.
+000128a0: 3d04 4b00 2004 3d04 3504 4104 3a04 3e04  =.K. .=.5.A.:.>.
+000128b0: 3b04 4c04 3a04 3e00 2004 3704 3004 3f04  ;.L.:.>. .7.0.?.
+000128c0: 3804 4104 3504 3900 2004 3f04 3e04 3304  8.A.5.9. .?.>.3.
+000128d0: 3004 4804 3504 3d04 3804 4f00 2004 2604  0.H.5.=.8.O. .&.
+000128e0: 1100 2004 3404 3b04 4f00 2008 0000 0000  .. .4.;.O. .....
+000128f0: 0600 0000 264d 756c 7469 706c 6520 6173  ....&Multiple as
+00012900: 7365 7420 6361 6e63 656c 6c61 7469 6f6e  set cancellation
+00012910: 206d 6174 6368 2066 6f72 2007 0000 000d   match for .....
+00012920: 5374 6174 656d 656e 7455 4b46 5501 0300  StatementUKFU...
+00012930: 0000 2404 2104 3404 3504 3b04 3e04 3a00  ..$.!.4.5.;.>.:.
+00012940: 2004 3704 3004 3304 4004 4304 3604 3504   .7.0.3.@.C.6.5.
+00012950: 3d04 3e00 3a00 2008 0000 0000 0600 0000  =.>.:. .........
+00012960: 0f54 7261 6465 7320 6c6f 6164 6564 3a20  .Trades loaded: 
+00012970: 0700 0000 0d53 7461 7465 6d65 6e74 554b  .....StatementUK
+00012980: 4655 0103 0000 0040 0422 0432 043e 0439  FU.....@.".2.>.9
+00012990: 0020 0431 0440 043e 043a 0435 0440 0020  . .1.@.>.:.5.@. 
+000129a0: 0028 0065 0078 002e 0020 0431 0440 043e  .(.e.x... .1.@.>
+000129b0: 043a 0435 0440 0020 0423 0440 0430 043b  .:.5.@. .#.@.0.;
+000129c0: 0441 0438 0431 0029 0800 0000 0006 0000  .A.8.1.)........
+000129d0: 0020 5476 6f79 2042 726f 6b65 7220 2865  . Tvoy Broker (e
+000129e0: 782e 2055 7261 6c73 6962 2042 726f 6b65  x. Uralsib Broke
+000129f0: 7229 0700 0000 0d53 7461 7465 6d65 6e74  r).....Statement
+00012a00: 554b 4655 0103 0000 0032 041e 0442 0447  UKFU.....2...B.G
+00012a10: 0451 0442 0020 0422 0432 043e 0439 0020  .Q.B. .".2.>.9. 
+00012a20: 0431 0440 043e 043a 0435 0440 0020 0028  .1.@.>.:.5.@. .(
+00012a30: 002a 002e 007a 0069 0070 0029 0800 0000  .*...z.i.p.)....
+00012a40: 0006 0000 001d 5476 6f79 2042 726f 6b65  ......Tvoy Broke
+00012a50: 7220 7374 6174 656d 656e 7420 282a 2e7a  r statement (*.z
+00012a60: 6970 2907 0000 000d 5374 6174 656d 656e  ip).....Statemen
+00012a70: 7455 4b46 5501 0300 0000 3004 1d04 3504  tUKFU.....0...5.
+00012a80: 3804 3704 3204 3504 4104 4204 3d04 4b04  8.7.2.5.A.B.=.K.
+00012a90: 3900 2004 4204 3804 3f00 2004 4104 3404  9. .B.8.?. .A.4.
+00012aa0: 3504 3b04 3a04 3800 3a00 2008 0000 0000  5.;.:.8.:. .....
+00012ab0: 0600 0000 1455 6e6b 6e6f 776e 2074 7261  .....Unknown tra
+00012ac0: 6465 2074 7970 653a 2007 0000 000d 5374  de type: .....St
+00012ad0: 6174 656d 656e 7455 4b46 5501 0300 0000  atementUKFU.....
+00012ae0: 3e04 1d04 3504 3f04 3e04 3404 3404 3504  >...5.?.>.4.4.5.
+00012af0: 4004 3604 3804 3204 3004 3504 3c04 3004  @.6.8.2.0.5.<.0.
+00012b00: 4f00 2004 3e04 3f04 3504 4004 3004 4604  O. .>.?.5.@.0.F.
+00012b10: 3804 4f00 2004 4100 2004 2604 1100 2008  8.O. .A. .&... .
+00012b20: 0000 0000 0600 0000 1d55 6e73 7570 7070  .........Unsuppp
+00012b30: 6f72 7465 6420 6173 7365 7420 6f70 6572  orted asset oper
+00012b40: 6174 696f 6e20 0700 0000 0d53 7461 7465  ation .....State
+00012b50: 6d65 6e74 554b 4655 0103 0000 004a 041d  mentUKFU.....J..
+00012b60: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
+00012b70: 0438 0432 0430 0435 043c 0430 044f 0020  .8.2.0.5.<.0.O. 
+00012b80: 0434 0435 043d 0435 0436 043d 0430 044f  .4.5.=.5.6.=.0.O
+00012b90: 0020 0442 0440 0430 043d 0437 0430 043a  . .B.@.0.=.7.0.:
+00012ba0: 0446 0438 044f 0020 0800 0000 0006 0000  .F.8.O. ........
+00012bb0: 001e 556e 7375 7070 706f 7274 6564 2063  ..Unsuppported c
+00012bc0: 6173 6820 7472 616e 7361 6374 696f 6e20  ash transaction 
+00012bd0: 0700 0000 0d53 7461 7465 6d65 6e74 554b  .....StatementUK
+00012be0: 4655 0103 0000 003e 0410 0440 0445 0438  FU.....>...@.E.8
+00012bf0: 0432 0020 0441 043e 0434 0435 0440 0436  .2. .A.>.4.5.@.6
+00012c00: 0438 0442 0020 043d 0435 0441 043a 043e  .8.B. .=.5.A.:.>
+00012c10: 043b 044c 043a 043e 0020 0444 0430 0439  .;.L.:.>. .D.0.9
+00012c20: 043b 043e 0432 0800 0000 0006 0000 001f  .;.>.2..........
+00012c30: 4172 6368 6976 6520 636f 6e74 6169 6e73  Archive contains
+00012c40: 206d 756c 7469 706c 6520 6669 6c65 7307   multiple files.
+00012c50: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
+00012c60: 0103 0000 005a 041d 0435 0020 0443 0434  .....Z...5. .C.4
+00012c70: 0430 043b 043e 0441 044c 0020 043d 0430  .0.;.>.A.L. .=.0
+00012c80: 0439 0442 0438 0020 043e 0436 0438 0434  .9.B.8. .>.6.8.4
+00012c90: 0430 0435 043c 044b 0439 0020 0437 0430  .0.5.<.K.9. .7.0
+00012ca0: 0433 043e 043b 043e 0432 043e 043a 0020  .3.>.;.>.2.>.:. 
+00012cb0: 043e 0442 0447 0451 0442 0430 003a 0020  .>.B.G.Q.B.0.:. 
+00012cc0: 0800 0000 0006 0000 0023 4361 6e27 7420  .........#Can't 
+00012cd0: 6669 6e64 2065 7870 6563 7465 6420 7265  find expected re
+00012ce0: 706f 7274 2068 6561 6465 723a 2007 0000  port header: ...
+00012cf0: 000c 5374 6174 656d 656e 7458 4c53 0103  ..StatementXLS..
+00012d00: 0000 0066 041d 0435 0020 0443 0434 0430  ...f...5. .C.4.0
+00012d10: 043b 043e 0441 044c 0020 043e 043f 0440  .;.>.A.L. .>.?.@
+00012d20: 0435 0434 0435 043b 0438 0442 044c 0020  .5.4.5.;.8.B.L. 
+00012d30: 0432 0430 043b 044e 0442 044b 0020 0438  .2.0.;.N.B.K. .8
+00012d40: 0437 0020 043e 0431 0449 0435 0439 0020  .7. .>.1.I.5.9. 
+00012d50: 0441 0435 043a 0446 0438 0438 0020 043e  .A.5.:.F.8.8. .>
+00012d60: 0442 0447 0451 0442 0430 0800 0000 0006  .B.G.Q.B.0......
+00012d70: 0000 0036 4361 6e27 7420 6765 7420 6375  ...6Can't get cu
+00012d80: 7272 656e 6369 6573 2066 726f 6d20 7375  rrencies from su
+00012d90: 6d6d 6172 7920 7365 6374 696f 6e20 6f66  mmary section of
+00012da0: 2073 7461 7465 6d65 6e74 0700 0000 0c53   statement.....S
+00012db0: 7461 7465 6d65 6e74 584c 5301 0300 0000  tatementXLS.....
+00012dc0: 4604 1d04 3504 3204 3e04 3704 3c04 3e04  F...5.2.>.7.<.>.
+00012dd0: 3604 3d04 3e00 2004 3e04 3f04 4004 3504  6.=.>. .>.?.@.5.
+00012de0: 3404 3504 3b04 3804 4204 4c00 2004 3f04  4.5.;.8.B.L. .?.
+00012df0: 3504 4004 3804 3e04 3400 2004 3e04 4204  5.@.8.>.4. .>.B.
+00012e00: 4704 5104 4204 3008 0000 0000 0600 0000  G.Q.B.0.........
+00012e10: 1843 616e 2774 2072 6561 6420 7265 706f  .Can't read repo
+00012e20: 7274 2070 6572 696f 6407 0000 000c 5374  rt period.....St
+00012e30: 6174 656d 656e 7458 4c53 0103 0000 001c  atementXLS......
+00012e40: 0414 0421 0020 0437 0430 0433 0440 0443  ...!. .7.0.3.@.C
+00012e50: 0436 0435 043d 044b 003a 0020 0800 0000  .6.5.=.K.:. ....
+00012e60: 0006 0000 0016 4361 7368 2062 616c 616e  ......Cash balan
+00012e70: 6365 7320 6c6f 6164 6564 3a20 0700 0000  ces loaded: ....
+00012e80: 0c53 7461 7465 6d65 6e74 584c 5301 0300  .StatementXLS...
+00012e90: 0000 3604 2104 4204 3e04 3b04 3104 3504  ..6.!.B.>.;.1.5.
+00012ea0: 4600 2004 3d04 3500 2004 3d04 3004 3904  F. .=.5. .=.0.9.
+00012eb0: 3404 3504 3d00 2004 3200 2004 4104 3504  4.5.=. .2. .A.5.
+00012ec0: 3a04 4604 3804 3800 2008 0000 0000 0600  :.F.8.8. .......
+00012ed0: 0000 1c43 6f6c 756d 6e20 6e6f 7420 666f  ...Column not fo
+00012ee0: 756e 6420 696e 2073 6563 7469 6f6e 2007  und in section .
+00012ef0: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
+00012f00: 0103 0000 0034 041d 0435 0441 043a 043e  .....4...5.A.:.>
+00012f10: 043b 044c 043a 043e 0020 0441 0447 0435  .;.L.:.>. .A.G.5
+00012f20: 0442 043e 0432 0020 043d 0430 0439 0434  .B.>.2. .=.0.9.4
+00012f30: 0435 043d 043e 003a 0020 0800 0000 0006  .5.=.>.:. ......
+00012f40: 0000 0019 4d75 6c74 6970 6c65 2061 6363  ....Multiple acc
+00012f50: 6f75 6e74 7320 666f 756e 643a 2007 0000  ounts found: ...
+00012f60: 000c 5374 6174 656d 656e 7458 4c53 0103  ..StatementXLS..
+00012f70: 0000 001c 0426 0411 0020 0437 0430 0433  .....&... .7.0.3
+00012f80: 0440 0443 0436 0435 043d 044b 003a 0020  .@.C.6.5.=.K.:. 
+00012f90: 0800 0000 0006 0000 0013 5365 6375 7269  ..........Securi
+00012fa0: 7469 6573 206c 6f61 6465 643a 2007 0000  ties loaded: ...
+00012fb0: 000c 5374 6174 656d 656e 7458 4c53 0103  ..StatementXLS..
+00012fc0: 0000 0030 041e 0442 0447 0451 0442 0020  ...0...B.G.Q.B. 
+00012fd0: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
+00012fe0: 0020 0443 0441 043f 0435 0448 043d 043e  . .C.A.?.5.H.=.>
+00012ff0: 003a 0020 0800 0000 0006 0000 001f 5374  .:. ..........St
+00013000: 6174 656d 656e 7420 6c6f 6164 6564 2073  atement loaded s
+00013010: 7563 6365 7373 6675 6c6c 793a 2007 0000  uccessfully: ...
+00013020: 000c 5374 6174 656d 656e 7458 4c53 0103  ..StatementXLS..
+00013030: 0000 0022 0020 0437 0430 0433 0440 0443  ...". .7.0.3.@.C
+00013040: 0436 0435 043d 0020 0443 0441 043f 0435  .6.5.=. .C.A.?.5
+00013050: 0448 043d 043e 0800 0000 0006 0000 0014  .H.=.>..........
+00013060: 206c 6f61 6465 6420 7375 6363 6573 7366   loaded successf
+00013070: 756c 6c79 0700 0000 0c53 7461 7465 6d65  ully.....Stateme
+00013080: 6e74 584d 4c01 0300 0000 3604 1d04 3504  ntXML.....6...5.
+00013090: 3204 3504 4004 3d04 4b04 3900 2004 4404  2.5.@.=.K.9. .D.
+000130a0: 3e04 4004 3c04 3004 4200 2000 5800 4d00  >.@.<.0.B. .X.M.
+000130b0: 4c00 2004 4404 3004 3904 3b04 3000 3a00  L. .D.0.9.;.0.:.
+000130c0: 2008 0000 0000 0600 0000 1643 616e 2774   ..........Can't
+000130d0: 2070 6172 7365 2058 4d4c 2066 696c 653a   parse XML file:
+000130e0: 2007 0000 000c 5374 6174 656d 656e 7458   .....StatementX
+000130f0: 4d4c 0103 0000 0044 041d 0435 0432 043e  ML.....D...5.2.>
+00013100: 0437 043c 043e 0436 043d 043e 0020 0437  .7.<.>.6.=.>. .7
+00013110: 0430 0433 0440 0443 0437 0438 0442 044c  .0.3.@.C.7.8.B.L
+00013120: 0020 043e 0442 0447 0451 0442 0020 043d  . .>.B.G.Q.B. .=
+00013130: 043e 043c 0435 0440 003a 0020 0800 0000  .>.<.5.@.:. ....
+00013140: 0006 0000 0020 4661 696c 6564 2074 6f20  ..... Failed to 
+00013150: 6669 6e64 2073 7461 7465 6d65 6e74 2069  find statement i
+00013160: 6e64 6578 3a20 0700 0000 0c53 7461 7465  ndex: .....State
+00013170: 6d65 6e74 584d 4c01 0300 0000 3e04 1d04  mentXML.....>...
+00013180: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
+00013190: 3e00 2004 3704 3004 3304 4004 4304 3704  >. .7.0.3.@.C.7.
+000131a0: 3804 4204 4c00 2004 3004 4204 4204 4004  8.B.L. .0.B.B.@.
+000131b0: 3804 3104 4304 4200 3a00 2008 0000 0000  8.1.C.B.:. .....
+000131c0: 0600 0000 1a46 6169 6c65 6420 746f 206c  .....Failed to l
+000131d0: 6f61 6420 6174 7472 6962 7574 653a 2007  oad attribute: .
+000131e0: 0000 000c 5374 6174 656d 656e 7458 4d4c  ....StatementXML
+000131f0: 0103 0000 0042 041e 0442 0447 0451 0442  .....B...B.G.Q.B
+00013200: 0020 0431 0440 043e 043a 0435 0440 0430  . .1.@.>.:.5.@.0
+00013210: 0020 043d 0435 0020 043d 0430 0439 0434  . .=.5. .=.0.9.4
+00013220: 0435 043d 0020 0432 0020 0444 0430 0439  .5.=. .2. .D.0.9
+00013230: 043b 0435 003a 0020 0800 0000 0006 0000  .;.5.:. ........
+00013240: 0020 4e6f 2073 7461 7465 6d65 6e74 2077  . No statement w
+00013250: 6173 2066 6f75 6e64 2069 6e20 6669 6c65  as found in file
+00013260: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
+00013270: 584d 4c01 0300 0000 3404 1d04 3504 3804  XML.....4...5.8.
+00013280: 3704 3204 3504 4104 4204 3d04 3004 4f00  7.2.5.A.B.=.0.O.
+00013290: 2004 3c04 3504 4204 3a04 3000 2004 3e04   .<.5.B.:.0. .>.
+000132a0: 4204 4704 5104 4204 3000 3a00 2008 0000  B.G.Q.B.0.:. ...
+000132b0: 0000 0600 0000 1755 6e6b 6e6f 776e 2073  .......Unknown s
+000132c0: 7461 7465 6d65 6e74 2074 6167 3a20 0700  tatement tag: ..
+000132d0: 0000 0c53 7461 7465 6d65 6e74 584d 4c01  ...StatementXML.
+000132e0: 0300 0000 4c04 1d04 3504 3f04 3e04 3404  ....L...5.?.>.4.
+000132f0: 3404 3504 4004 3604 3804 3204 3004 3504  4.5.@.6.8.2.0.5.
+00013300: 3c04 4b04 3900 2004 4404 3e04 4004 3c04  <.K.9. .D.>.@.<.
+00013310: 3004 4200 2004 3404 3004 4204 4b00 2f04  0.B. .4.0.B.K./.
+00013320: 3204 4004 3504 3c04 3504 3d04 3800 3a00  2.@.5.<.5.=.8.:.
+00013330: 2008 0000 0000 0600 0000 1e55 6e73 7570   ..........Unsup
+00013340: 706f 7274 6564 2064 6174 652f 7469 6d65  ported date/time
+00013350: 2066 6f72 6d61 743a 2007 0000 000c 5374   format: .....St
+00013360: 6174 656d 656e 7458 4d4c 0103 0000 0020  atementXML..... 
+00013370: 041e 0448 0438 0431 043a 0430 0020 0438  ...H.8.1.:.0. .8
+00013380: 043c 043f 043e 0440 0442 0430 003a 0020  .<.?.>.@.B.0.:. 
+00013390: 0800 0000 0006 0000 000f 496d 706f 7274  ..........Import
+000133a0: 2066 6169 6c65 643a 2007 0000 000a 5374   failed: .....St
+000133b0: 6174 656d 656e 7473 0103 0000 0040 0412  atements.....@..
+000133c0: 044b 0431 0435 0440 0438 0442 0435 0020  .K.1.5.@.8.B.5. 
+000133d0: 0444 0430 0439 043b 0020 043e 0442 0447  .D.0.9.;. .>.B.G
+000133e0: 0435 0442 0430 0020 0434 043b 044f 0020  .5.B.0. .4.;.O. 
+000133f0: 0438 043c 043f 043e 0440 0442 0430 0800  .8.<.?.>.@.B.0..
+00013400: 0000 0006 0000 001f 5365 6c65 6374 2073  ........Select s
+00013410: 7461 7465 6d65 6e74 2066 696c 6520 746f  tatement file to
+00013420: 2069 6d70 6f72 7407 0000 000a 5374 6174   import.....Stat
+00013430: 656d 656e 7473 0103 0000 004a 041a 043b  ements.....J...;
+00013440: 0430 0441 0441 0020 043e 0442 0447 0451  .0.A.A. .>.B.G.Q
+00013450: 0442 0430 0020 043d 0435 0020 043c 043e  .B.0. .=.5. .<.>
+00013460: 0436 0435 0442 0020 0431 044b 0442 044c  .6.5.B. .1.K.B.L
+00013470: 0020 0437 0430 0433 0440 0443 0436 0435  . .7.0.3.@.C.6.5
+00013480: 043d 003a 0020 0800 0000 0006 0000 0021  .=.:. .........!
+00013490: 5374 6174 656d 656e 7420 636c 6173 7320  Statement class 
+000134a0: 6361 6e27 7420 6265 206c 6f61 6465 643a  can't be loaded:
+000134b0: 2007 0000 000a 5374 6174 656d 656e 7473   .....Statements
+000134c0: 0103 0000 0054 041c 043e 0434 0443 043b  .....T...>.4.C.;
+000134d0: 044c 0020 043e 0442 0447 0451 0442 0430  .L. .>.B.G.Q.B.0
+000134e0: 0020 043d 0435 0020 043c 043e 0436 0435  . .=.5. .<.>.6.5
+000134f0: 0442 0020 0431 044b 0442 044c 0020 0438  .B. .1.K.B.L. .8
+00013500: 043c 043f 043e 0440 0442 0438 0440 043e  .<.?.>.@.B.8.@.>
+00013510: 0432 0430 043d 003a 0020 0800 0000 0006  .2.0.=.:. ......
+00013520: 0000 0024 5374 6174 656d 656e 7420 6d6f  ...$Statement mo
+00013530: 6475 6c65 2063 616e 2774 2062 6520 696d  dule can't be im
+00013540: 706f 7274 6564 3a20 0700 0000 0a53 7461  ported: .....Sta
+00013550: 7465 6d65 6e74 7301 0300 0000 0804 1004  tements.........
+00013560: 3a04 4200 2e08 0000 0000 0600 0000 0441  :.B............A
+00013570: 6374 2e07 0000 0010 5379 6d62 6f6c 734c  ct......SymbolsL
+00013580: 6973 744d 6f64 656c 0103 0000 000c 0412  istModel........
+00013590: 0430 043b 044e 0442 0430 0800 0000 0006  .0.;.N.B.0......
+000135a0: 0000 0008 4375 7272 656e 6379 0700 0000  ....Currency....
+000135b0: 1053 796d 626f 6c73 4c69 7374 4d6f 6465  .SymbolsListMode
+000135c0: 6c01 0300 0000 1004 1e04 3f04 3804 4104  l.........?.8.A.
+000135d0: 3004 3d04 3804 3508 0000 0000 0600 0000  0.=.8.5.........
+000135e0: 0b44 6573 6372 6970 7469 6f6e 0700 0000  .Description....
+000135f0: 1053 796d 626f 6c73 4c69 7374 4d6f 6465  .SymbolsListMode
+00013600: 6c01 0300 0000 1204 1a04 3e04 4204 3804  l.........>.B.8.
+00013610: 4004 3e04 3204 3a04 3808 0000 0000 0600  @.>.2.:.8.......
+00013620: 0000 0651 756f 7465 7307 0000 0010 5379  ...Quotes.....Sy
+00013630: 6d62 6f6c 734c 6973 744d 6f64 656c 0103  mbolsListModel..
+00013640: 0000 000c 0421 0438 043c 0432 043e 043b  .....!.8.<.2.>.;
+00013650: 0800 0000 0006 0000 0006 5379 6d62 6f6c  ..........Symbol
+00013660: 0700 0000 1053 796d 626f 6c73 4c69 7374  .....SymbolsList
+00013670: 4d6f 6465 6c01 0300 0000 0604 2204 4d04  Model.......".M.
+00013680: 3308 0000 0000 0600 0000 0354 6167 0700  3..........Tag..
+00013690: 0000 0c54 6167 4c69 7374 4d6f 6465 6c01  ...TagListModel.
+000136a0: 0300 0000 1004 1e04 3f04 3504 4004 3004  ........?.5.@.0.
+000136b0: 4604 3804 3808 0000 0000 0600 0000 0a4f  F.8.8..........O
+000136c0: 7065 7261 7469 6f6e 7307 0000 0009 5461  perations.....Ta
+000136d0: 6752 6570 6f72 7401 0300 0000 1004 3f04  gReport.......?.
+000136e0: 3e00 2004 1c04 3504 4204 3a04 3508 0000  >. ...5.B.:.5...
+000136f0: 0000 0600 0000 0662 7920 5461 6707 0000  .......by Tag...
+00013700: 0009 5461 6752 6570 6f72 7401 0300 0000  ..TagReport.....
+00013710: 1c04 1e04 4204 4704 3504 4200 2004 3f04  ....B.G.5.B. .?.
+00013720: 3e00 2004 3c04 3504 4204 3a04 3508 0000  >. .<.5.B.:.5...
+00013730: 0000 0600 0000 0d52 6570 6f72 7420 6279  .......Report by
+00013740: 2074 6167 0700 0000 0f54 6167 5265 706f   tag.....TagRepo
+00013750: 7274 5769 6467 6574 0103 0000 000c 041c  rtWidget........
+00013760: 0435 0442 043a 0430 003a 0800 0000 0006  .5.B.:.0.:......
+00013770: 0000 0004 5461 673a 0700 0000 0f54 6167  ....Tag:.....Tag
+00013780: 5265 706f 7274 5769 6467 6574 0103 0000  ReportWidget....
+00013790: 0024 0027 0020 0437 0430 043c 0435 043d  .$.'. .7.0.<.5.=
+000137a0: 0435 043d 0430 0020 0443 0441 043f 0435  .5.=.0. .C.A.?.5
+000137b0: 0448 043d 043e 0800 0000 0006 0000 001b  .H.=.>..........
+000137c0: 2720 7761 7320 7375 6363 6573 7366 756c  ' was successful
+000137d0: 6c79 2072 6570 6c61 6365 6407 0000 000e  ly replaced.....
+000137e0: 5461 6773 4c69 7374 4469 616c 6f67 0103  TagsListDialog..
+000137f0: 0000 000c 0027 0020 043d 0430 003a 0020  .....'. .=.0.:. 
+00013800: 0800 0000 0006 0000 0008 2720 7769 7468  ..........' with
+00013810: 3a20 0700 0000 0e54 6167 734c 6973 7444  : .....TagsListD
+00013820: 6961 6c6f 6701 0300 0000 2004 1704 3004  ialog..... ...0.
+00013830: 3c04 3504 3d04 3804 4204 4c00 2004 3c04  <.5.=.8.B.L. .<.
+00013840: 3504 4204 3a04 4300 2000 2708 0000 0000  5.B.:.C. .'.....
+00013850: 0600 0000 0d52 6570 6c61 6365 2074 6167  .....Replace tag
+00013860: 2027 0700 0000 0e54 6167 734c 6973 7444   '.....TagsListD
+00013870: 6961 6c6f 6701 0300 0000 1c04 1704 3004  ialog.........0.
+00013880: 3c04 3504 3d04 3804 4204 4c00 2004 3d04  <.5.=.8.B.L. .=.
+00013890: 3000 2e00 2e00 2e08 0000 0000 0600 0000  0...............
+000138a0: 0f52 6570 6c61 6365 2077 6974 682e 2e2e  .Replace with...
+000138b0: 0700 0000 0e54 6167 734c 6973 7444 6961  .....TagsListDia
+000138c0: 6c6f 6701 0300 0000 3404 1f04 3e04 3a04  log.....4...>.:.
+000138d0: 3004 3704 3004 4204 4c00 2004 3e04 3f04  0.7.0.B.L. .>.?.
+000138e0: 3504 4004 3004 4604 3804 3800 2004 4100  5.@.0.F.8.8. .A.
+000138f0: 2004 1c04 3504 4204 3a04 3e04 3908 0000   ...5.B.:.>.9...
+00013900: 0000 0600 0000 1853 686f 7720 6f70 6572  .......Show oper
+00013910: 6174 696f 6e73 2077 6974 6820 5461 6707  ations with Tag.
+00013920: 0000 000e 5461 6773 4c69 7374 4469 616c  ....TagsListDial
+00013930: 6f67 0103 0000 000e 041c 0435 0442 043a  og.........5.B.:
+00013940: 0430 0020 0027 0800 0000 0006 0000 0005  .0. .'..........
+00013950: 5461 6720 2707 0000 000e 5461 6773 4c69  Tag '.....TagsLi
+00013960: 7374 4469 616c 6f67 0103 0000 0008 0422  stDialog......."
+00013970: 044d 0433 0438 0800 0000 0006 0000 0004  .M.3.8..........
+00013980: 5461 6773 0700 0000 0e54 6167 734c 6973  Tags.....TagsLis
+00013990: 7444 6961 6c6f 6701 0300 0000 1a04 2204  tDialog.......".
+000139a0: 3504 3a04 4304 4904 3804 3900 2004 3a04  5.:.C.I.8.9. .:.
+000139b0: 4304 4004 4100 3a08 0000 0000 0600 0000  C.@.A.:.........
+000139c0: 0d43 7572 7265 6e74 2072 6174 653a 0700  .Current rate:..
+000139d0: 0000 1354 6178 4573 7469 6d61 7469 6f6e  ...TaxEstimation
+000139e0: 4469 616c 6f67 0103 0000 0028 041f 043e  Dialog.....(...>
+000139f0: 0441 043b 0435 0434 043d 044f 044f 0020  .A.;.5.4.=.O.O. 
+00013a00: 043a 043e 0442 0438 0440 043e 0432 043a  .:.>.B.8.@.>.2.:
+00013a10: 0430 003a 0800 0000 0006 0000 000b 4c61  .0.:..........La
+00013a20: 7374 2071 756f 7465 3a07 0000 0013 5461  st quote:.....Ta
+00013a30: 7845 7374 696d 6174 696f 6e44 6961 6c6f  xEstimationDialo
+00013a40: 6701 0300 0000 1a04 1e04 4604 3504 3d04  g.........F.5.=.
+00013a50: 3a04 3000 2004 3d04 3004 3b04 3e04 3304  :.0. .=.0.;.>.3.
+00013a60: 3008 0000 0000 0600 0000 0e54 6178 2045  0..........Tax E
+00013a70: 7374 696d 6174 696f 6e07 0000 0013 5461  stimation.....Ta
+00013a80: 7845 7374 696d 6174 696f 6e44 6961 6c6f  xEstimationDialo
+00013a90: 6701 0300 0000 0800 5800 2e00 5800 5808  g.......X...X.X.
+00013aa0: 0000 0000 0600 0000 0458 2e58 5807 0000  .........X.XX...
+00013ab0: 0013 5461 7845 7374 696d 6174 696f 6e44  ..TaxEstimationD
+00013ac0: 6961 6c6f 6701 0300 0000 0a04 1804 2204  ialog.........".
+00013ad0: 1e04 1304 1e08 0000 0000 0600 0000 0554  ...............T
+00013ae0: 4f54 414c 0700 0000 0c54 6178 4573 7469  OTAL.....TaxEsti
+00013af0: 6d61 746f 7201 0300 0000 2404 1e04 4604  mator.....$...F.
+00013b00: 3504 3d04 3a04 3000 2004 3d04 3004 3b04  5.=.:.0. .=.0.;.
+00013b10: 3e04 3304 3000 2004 3404 3b04 4f00 2008  >.3.0. .4.;.O. .
+00013b20: 0000 0000 0600 0000 1354 6178 2065 7374  .........Tax est
+00013b30: 696d 6174 696f 6e20 666f 7220 0700 0000  imation for ....
+00013b40: 0c54 6178 4573 7469 6d61 746f 7201 0300  .TaxEstimator...
+00013b50: 0000 3c04 2104 4204 3004 3204 3a04 3000  ..<.!.B.0.2.:.0.
+00013b60: 2004 3d04 3004 3b04 3e04 3304 3000 2004   .=.0.;.>.3.0. .
+00013b70: 3d04 3500 2004 3d04 3004 3904 3404 3504  =.5. .=.0.9.4.5.
+00013b80: 3d04 3000 2004 3404 3b04 4f00 3a00 2008  =.0. .4.;.O.:. .
+00013b90: 0000 0000 0600 0000 1854 6178 2072 6174  .........Tax rat
+00013ba0: 6520 6e6f 7420 666f 756e 6420 666f 723a  e not found for:
+00013bb0: 2007 0000 000c 5461 7845 7374 696d 6174   .....TaxEstimat
+00013bc0: 6f72 0103 0000 0008 0414 0430 0442 0430  or.........0.B.0
+00013bd0: 0800 0000 0006 0000 0004 4461 7465 0700  ..........Date..
+00013be0: 0000 1154 6178 4573 7469 6d61 746f 724d  ...TaxEstimatorM
+00013bf0: 6f64 656c 0103 0000 0014 0426 0435 043d  odel.......&.5.=
+00013c00: 0430 0020 043e 0442 043a 0440 002e 0800  .0. .>.B.:.@....
+00013c10: 0000 0006 0000 0004 4f70 656e 0700 0000  ........Open....
+00013c20: 1154 6178 4573 7469 6d61 746f 724d 6f64  .TaxEstimatorMod
+00013c30: 656c 0103 0000 0012 041f 0440 0438 0431  el.........@.8.1
+00013c40: 044b 043b 044c 002c 0020 0800 0000 0006  .K.;.L.,. ......
+00013c50: 0000 0008 5072 6f66 6974 2c20 0700 0000  ....Profit, ....
+00013c60: 1154 6178 4573 7469 6d61 746f 724d 6f64  .TaxEstimatorMod
+00013c70: 656c 0103 0000 000c 041a 043e 043b 002d  el.........>.;.-
+00013c80: 0432 043e 0800 0000 0006 0000 0003 5174  .2.>..........Qt
+00013c90: 7907 0000 0011 5461 7845 7374 696d 6174  y.....TaxEstimat
+00013ca0: 6f72 4d6f 6465 6c01 0300 0000 0c04 1a04  orModel.........
+00013cb0: 4304 4004 4100 2c00 2008 0000 0000 0600  C.@.A.,. .......
+00013cc0: 0000 0652 6174 652c 2007 0000 0011 5461  ...Rate, .....Ta
+00013cd0: 7845 7374 696d 6174 6f72 4d6f 6465 6c01  xEstimatorModel.
+00013ce0: 0300 0000 0e04 1d04 3004 3b04 3e04 3300  ........0.;.>.3.
+00013cf0: 2c00 2008 0000 0000 0600 0000 0554 6178  ,. ..........Tax
+00013d00: 2c20 0700 0000 1154 6178 4573 7469 6d61  , .....TaxEstima
+00013d10: 746f 724d 6f64 656c 0103 0000 0074 041d  torModel.....t..
+00013d20: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
+00013d30: 043e 0020 0437 0430 0433 0440 0443 0437  .>. .7.0.3.@.C.7
+00013d40: 0438 0442 044c 0020 043f 0430 0440 0430  .8.B.L. .?.0.@.0
+00013d50: 043c 0435 0442 0440 044b 0020 043d 0430  .<.5.B.@.K. .=.0
+00013d60: 043b 043e 0433 043e 0432 043e 0433 043e  .;.>.3.>.2.>.3.>
+00013d70: 0020 043e 0442 0447 0451 0442 0430 0020  . .>.B.G.Q.B.0. 
+00013d80: 0438 0437 0020 0444 0430 0439 043b 0430  .8.7. .D.0.9.;.0
+00013d90: 0020 0800 0000 0006 0000 002b 4361 6e27  . .........+Can'
+00013da0: 7420 6c6f 6164 2074 6178 2072 6570 6f72  t load tax repor
+00013db0: 7420 7061 7261 6d65 7465 7273 2066 726f  t parameters fro
+00013dc0: 6d20 6669 6c65 2007 0000 0009 5461 7852  m file .....TaxR
+00013dd0: 6570 6f72 7401 0300 0000 2804 1d04 3504  eport.....(...5.
+00013de0: 3804 3704 3204 3504 4104 4204 3d04 3004  8.7.2.5.A.B.=.0.
+00013df0: 4f00 2004 3204 3004 3b04 4e04 4204 3000  O. .2.0.;.N.B.0.
+00013e00: 3a00 2008 0000 0000 0600 0000 1943 7572  :. ..........Cur
+00013e10: 7265 6e63 7920 6973 206e 6f74 2064 6566  rency is not def
+00013e20: 696e 6564 3a20 0700 0000 0954 6178 5265  ined: .....TaxRe
+00013e30: 706f 7274 0103 0000 004a 041d 0435 0020  port.....J...5. 
+00013e40: 0443 043a 0430 0437 0430 043d 0020 0448  .C.:.0.7.0.=. .H
+00013e50: 0430 0431 043b 043e 043d 0020 043e 0442  .0.1.;.>.=. .>.B
+00013e60: 0447 0435 0442 0430 0020 0434 043b 044f  .G.5.B.0. .4.;.O
+00013e70: 0020 0440 0430 0437 0434 0435 043b 0430  . .@.0.7.4.5.;.0
+00013e80: 003a 0020 0800 0000 0006 0000 0026 4e6f  .:. .........&No
+00013e90: 2072 6570 6f72 7420 7465 6d70 6c61 7465   report template
+00013ea0: 2066 6f75 6e64 2066 6f72 2073 6563 7469   found for secti
+00013eb0: 6f6e 3a20 0700 0000 0954 6178 5265 706f  on: .....TaxRepo
+00013ec0: 7274 0103 0000 006a 041d 0435 0442 0020  rt.....j...5.B. 
+00013ed0: 0438 043d 0444 043e 0440 043c 0430 0446  .8.=.D.>.@.<.0.F
+00013ee0: 0438 0438 0020 043e 0020 0421 043e 0418  .8.8. .>. .!.>..
+00013ef0: 0414 041d 0020 0432 0020 043f 0430 0440  ..... .2. .?.0.@
+00013f00: 0430 043c 0435 0442 0440 0430 0445 0020  .0.<.5.B.@.0.E. 
+00013f10: 043d 0430 043b 043e 0433 043e 0432 043e  .=.0.;.>.3.>.2.>
+00013f20: 0433 043e 0020 043e 0442 0447 0451 0442  .3.>. .>.B.G.Q.B
+00013f30: 0430 0800 0000 0006 0000 0042 5468 6572  .0.........BTher
+00013f40: 6520 6172 6520 6e6f 2069 6e66 6f72 6d61  e are no informa
+00013f50: 7469 6f6e 2061 626f 7574 2074 6178 2074  tion about tax t
+00013f60: 7265 6174 7920 696e 2074 6178 2072 6570  reaty in tax rep
+00013f70: 6f72 7420 7061 7261 6d65 7465 7273 0700  ort parameters..
+00013f80: 0000 0954 6178 5265 706f 7274 0103 0000  ...TaxReport....
+00013f90: 0060 041d 0435 0020 0437 0430 0434 0430  .`...5. .7.0.4.0
+00013fa0: 043d 044b 0020 043f 0430 0440 0430 043c  .=.K. .?.0.@.0.<
+00013fb0: 0435 0442 0440 044b 0020 043d 0430 043b  .5.B.@.K. .=.0.;
+00013fc0: 043e 0433 043e 0432 043e 0433 043e 0020  .>.3.>.2.>.3.>. 
+00013fd0: 043e 0442 0447 0451 0442 0430 0020 0434  .>.B.G.Q.B.0. .4
+00013fe0: 043b 044f 0020 0433 043e 0434 0430 003a  .;.O. .3.>.4.0.:
+00013ff0: 0020 0800 0000 0006 0000 0033 5468 6572  . .........3Ther
+00014000: 6520 6172 6520 6e6f 2070 6172 616d 6574  e are no paramet
+00014010: 6572 7320 666f 756e 6420 666f 7220 7461  ers found for ta
+00014020: 7820 7265 706f 7274 2079 6561 723a 2007  x report year: .
+00014030: 0000 0009 5461 7852 6570 6f72 7401 0300  ....TaxReport...
+00014040: 0000 0a00 2000 2e00 2e00 2e00 2008 0000  .... ....... ...
+00014050: 0000 0600 0000 0520 2e2e 2e20 0700 0000  ....... ... ....
+00014060: 0954 6178 5769 6467 6574 0103 0000 0006  .TaxWidget......
+00014070: 002e 002e 002e 0800 0000 0006 0000 0003  ................
+00014080: 2e2e 2e07 0000 0009 5461 7857 6964 6765  ........TaxWidge
+00014090: 7401 0300 0000 0a04 2104 4704 3504 4200  t.......!.G.5.B.
+000140a0: 3a08 0000 0000 0600 0000 0841 6363 6f75  :..........Accou
+000140b0: 6e74 3a07 0000 0009 5461 7857 6964 6765  nt:.....TaxWidge
+000140c0: 7401 0300 0000 9004 1d04 3804 3604 3500  t.........8.6.5.
+000140d0: 2004 4004 3004 4104 3f04 3e04 3b04 3e04   .@.0.A.?.>.;.>.
+000140e0: 3604 3504 3d04 4b00 2004 4d04 3a04 4104  6.5.=.K. .M.:.A.
+000140f0: 3f04 3504 4004 3804 3c04 3504 3d04 4204  ?.5.@.8.<.5.=.B.
+00014100: 3004 3b04 4c04 3d04 4b04 3500 2004 4404  0.;.L.=.K.5. .D.
+00014110: 4304 3d04 3a04 4604 3804 3800 2000 2d00  C.=.:.F.8.8. .-.
+00014120: 2004 3804 4104 3f04 3e04 3b04 4c04 3704   .8.A.?.>.;.L.7.
+00014130: 4304 3904 4204 3500 2004 4100 2004 3e04  C.9.B.5. .A. .>.
+00014140: 4104 4204 3e04 4004 3e04 3604 3d04 3e04  A.B.>.@.>.6.=.>.
+00014150: 4104 4204 4c04 4e08 0000 0000 0600 0000  A.B.L.N.........
+00014160: 3342 656c 6f77 2066 756e 6374 696f 6e73  3Below functions
+00014170: 2061 7265 2065 7870 6572 696d 656e 7461   are experimenta
+00014180: 6c20 2d20 7573 6520 6974 2077 6974 6820  l - use it with 
+00014190: 6361 7265 0700 0000 0954 6178 5769 6467  care.....TaxWidg
+000141a0: 6574 0103 0000 0044 041d 0435 0432 043e  et.....D...5.2.>
+000141b0: 0437 043c 043e 0436 043d 043e 0020 0437  .7.<.>.6.=.>. .7
+000141c0: 0430 043f 0438 0441 0430 0442 044c 0020  .0.?.8.A.0.B.L. 
+000141d0: 0033 002d 041d 0414 0424 041b 0020 0432  .3.-.....$... .2
+000141e0: 0020 0444 0430 0439 043b 0020 0800 0000  . .D.0.9.;. ....
+000141f0: 0006 0000 001f 4361 6e27 7420 7772 6974  ......Can't writ
+00014200: 6520 7461 7820 666f 726d 2069 6e74 6f20  e tax form into 
+00014210: 6669 6c65 2007 0000 0009 5461 7857 6964  file .....TaxWid
+00014220: 6765 7401 0300 0000 0e04 2104 4204 4004  get.......!.B.@.
+00014230: 3004 3d04 3000 3a08 0000 0000 0600 0000  0.=.0.:.........
+00014240: 0843 6f75 6e74 7279 3a07 0000 0009 5461  .Country:.....Ta
+00014250: 7857 6964 6765 7401 0300 0000 7804 2104  xWidget.....x.!.
+00014260: 3e04 3704 3404 3004 4204 4c00 2004 4404  >.7.4.0.B.L. .D.
+00014270: 3004 3904 3b00 2000 3300 2d04 1d04 2404  0.9.;. .3.-...$.
+00014280: 1404 1b00 2004 3200 2004 4404 3e04 4004  .... .2. .D.>.@.
+00014290: 3c04 3004 4204 3500 2004 3f04 4004 3e04  <.0.B.5. .?.@.>.
+000142a0: 3304 4004 3004 3c04 3c04 4b00 2000 2204  3.@.0.<.<.K. .".
+000142b0: 1404 3504 3a04 3b04 3004 4004 3004 4604  ..5.:.;.0.@.0.F.
+000142c0: 3804 4f00 2200 2000 2800 2a00 2e00 6400  8.O.". .(.*...d.
+000142d0: 6300 5800 2908 0000 0000 0600 0000 4043  c.X.).........@C
+000142e0: 7265 6174 6520 7461 7820 666f 726d 2069  reate tax form i
+000142f0: 6e20 22d0 94d0 b5d0 bad0 bbd0 b0d1 80d0  n ".............
+00014300: b0d1 86d0 b8d1 8f22 2070 726f 6772 616d  ......." program
+00014310: 2066 6f72 6d61 7420 282a 2e64 6358 2907   format (*.dcX).
+00014320: 0000 0009 5461 7857 6964 6765 7401 0300  ....TaxWidget...
+00014330: 0000 1e04 1404 3004 3d04 3d04 4b04 3500  ......0.=.=.K.5.
+00014340: 2004 3d04 3504 3f04 3e04 3b04 3d04 4b04   .=.5.?.>.;.=.K.
+00014350: 3508 0000 0000 0600 0000 1344 6174 6120  5..........Data 
+00014360: 6172 6520 696e 636f 6d70 6c65 7465 0700  are incomplete..
+00014370: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
+00014380: 005c 041d 0435 0020 0438 0441 043f 043e  .\...5. .8.A.?.>
+00014390: 043b 044c 0437 043e 0432 0430 0442 044c  .;.L.7.>.2.0.B.L
+000143a0: 0020 0434 0430 0442 0443 0020 043f 043e  . .4.0.B.C. .?.>
+000143b0: 0441 0442 0430 0432 043a 0438 0020 0434  .A.B.0.2.:.8. .4
+000143c0: 043b 044f 0020 043a 0443 0440 0441 043e  .;.O. .:.C.@.A.>
+000143d0: 0432 0020 0432 0430 043b 044e 0442 0800  .2. .2.0.;.N.B..
+000143e0: 0000 0006 0000 002d 446f 206e 6f74 2075  .......-Do not u
+000143f0: 7365 2073 6574 746c 656d 656e 7420 6461  se settlement da
+00014400: 7465 2066 6f72 2063 7572 7265 6e63 7920  te for currency 
+00014410: 7261 7465 7307 0000 0009 5461 7857 6964  rates.....TaxWid
+00014420: 6765 7401 0300 0000 1604 2404 3004 3904  get.......$.0.9.
+00014430: 3b00 2000 4500 7800 6300 6500 6c00 3a08  ;. .E.x.c.e.l.:.
+00014440: 0000 0000 0600 0000 0b45 7863 656c 2066  .........Excel f
+00014450: 696c 653a 0700 0000 0954 6178 5769 6467  ile:.....TaxWidg
+00014460: 6574 0103 0000 0028 0424 0430 0439 043b  et.....(.$.0.9.;
+00014470: 044b 0020 0045 0078 0063 0065 006c 0020  .K. .E.x.c.e.l. 
+00014480: 0028 002a 002e 0078 0073 006c 0078 0029  .(.*...x.s.l.x.)
+00014490: 0800 0000 0006 0000 0014 4578 6365 6c20  ..........Excel 
+000144a0: 6669 6c65 7320 282a 2e78 6c73 7829 0700  files (*.xlsx)..
+000144b0: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
+000144c0: 004a 0424 0430 0439 043b 0020 0434 043b  .J.$.0.9.;. .4.;
+000144d0: 044f 0020 0441 043e 0445 0440 0430 043d  .O. .A.>.E.@.0.=
+000144e0: 0435 043d 0438 044f 0020 0434 0435 043a  .5.=.8.O. .4.5.:
+000144f0: 043b 0430 0440 0430 0446 0438 0438 0020  .;.0.@.0.F.8.8. 
+00014500: 0033 002d 041d 0414 0424 041b 0800 0000  .3.-.....$......
+00014510: 0006 0000 0024 4669 6c65 2077 6865 7265  .....$File where
+00014520: 2074 6f20 7374 6f72 6520 7275 7373 6961   to store russia
+00014530: 6e20 7461 7820 666f 726d 0700 0000 0954  n tax form.....T
+00014540: 6178 5769 6467 6574 0103 0000 0056 0424  axWidget.....V.$
+00014550: 0430 0439 043b 0020 0434 043b 044f 0020  .0.9.;. .4.;.O. 
+00014560: 0441 043e 0445 0440 0430 043d 0435 043d  .A.>.E.@.0.=.5.=
+00014570: 0438 044f 0020 0440 0430 0441 0447 0451  .8.O. .@.0.A.G.Q
+00014580: 0442 0430 0020 0432 0020 0444 043e 0440  .B.0. .2. .D.>.@
+00014590: 043c 0430 0442 0435 0020 0045 0078 0063  .<.0.B.5. .E.x.c
+000145a0: 0065 006c 0800 0000 0006 0000 002e 4669  .e.l..........Fi
+000145b0: 6c65 2077 6865 7265 2074 6f20 7374 6f72  le where to stor
+000145c0: 6520 7461 7820 7265 706f 7274 2069 6e20  e tax report in 
+000145d0: 4578 6365 6c20 666f 726d 6174 0700 0000  Excel format....
+000145e0: 0954 6178 5769 6467 6574 0103 0000 0068  .TaxWidget.....h
+000145f0: 0417 0430 0440 0443 0431 0435 0436 043d  ...0.@.C.1.5.6.=
+00014600: 044b 0439 0020 0441 0447 0451 0442 0020  .K.9. .A.G.Q.B. 
+00014610: 0434 043b 044f 0020 043a 043e 0442 043e  .4.;.O. .:.>.B.>
+00014620: 0440 043e 0433 043e 0020 043d 0443 0436  .@.>.3.>. .=.C.6
+00014630: 043d 043e 0020 043f 043e 0434 0433 043e  .=.>. .?.>.4.3.>
+00014640: 0442 043e 0432 0438 0442 044c 0020 043e  .B.>.2.8.B.L. .>
+00014650: 0442 0447 0451 0442 0800 0000 0006 0000  .B.G.Q.B........
+00014660: 0029 466f 7265 6967 6e20 6163 636f 756e  .)Foreign accoun
+00014670: 7420 746f 2070 7265 7061 7265 2074 6178  t to prepare tax
+00014680: 2072 6570 6f72 7420 666f 7207 0000 0009   report for.....
+00014690: 5461 7857 6964 6765 7401 0300 0000 2604  TaxWidget.....&.
+000146a0: 2404 3004 3904 3b00 2004 4100 2004 4004  $.0.9.;. .A. .@.
+000146b0: 3504 3704 4304 3b04 4c04 4204 3004 4204  5.7.C.;.L.B.0.B.
+000146c0: 3e04 3c00 3a08 0000 0000 0600 0000 0c4f  >.<.:..........O
+000146d0: 7574 7075 7420 6669 6c65 3a07 0000 0009  utput file:.....
+000146e0: 5461 7857 6964 6765 7401 0300 0000 1e04  TaxWidget.......
+000146f0: 2104 3e04 4504 4004 3004 3d04 3804 4204  !.>.E.@.0.=.8.B.
+00014700: 4c00 2004 1e04 4204 4704 5104 4208 0000  L. ...B.G.Q.B...
+00014710: 0000 0600 0000 0b53 6176 6520 5265 706f  .......Save Repo
+00014720: 7274 0700 0000 0954 6178 5769 6467 6574  rt.....TaxWidget
+00014730: 0103 0000 0026 0421 043e 0445 0440 0430  .....&.!.>.E.@.0
+00014740: 043d 0438 0442 044c 0020 0033 002d 041d  .=.8.B.L. .3.-..
+00014750: 0414 0424 041b 0020 0432 003a 0800 0000  ...$... .2.:....
+00014760: 0006 0000 0011 5361 7665 2074 6178 2066  ......Save tax f
+00014770: 6f72 6d20 746f 3a07 0000 0009 5461 7857  orm to:.....TaxW
+00014780: 6964 6765 7401 0300 0000 3804 2104 3e04  idget.....8.!.>.
+00014790: 4504 4004 3004 3d04 3804 4204 4c00 2004  E.@.0.=.8.B.L. .
+000147a0: 3d04 3004 3b04 3e04 3304 3e04 3204 4b04  =.0.;.>.3.>.2.K.
+000147b0: 3900 2004 3e04 4204 4704 5104 4200 2004  9. .>.B.G.Q.B. .
+000147c0: 3200 3a08 0000 0000 0600 0000 1453 6176  2.:..........Sav
+000147d0: 6520 7461 7820 7265 706f 7274 7320 746f  e tax reports to
+000147e0: 3a07 0000 0009 5461 7857 6964 6765 7401  :.....TaxWidget.
+000147f0: 0300 0000 1804 1204 4b04 3104 3504 4004  ........K.1.5.@.
+00014800: 3804 4200 2004 4404 3004 3904 3b08 0000  8.B. .D.0.9.;...
+00014810: 0000 0600 0000 0b53 656c 6563 7420 6669  .......Select fi
+00014820: 6c65 0700 0000 0954 6178 5769 6467 6574  le.....TaxWidget
+00014830: 0103 0000 0028 041d 0430 043b 043e 0433  .....(...0.;.>.3
+00014840: 043e 0432 044b 0439 0020 043e 0442 0447  .>.2.K.9. .>.B.G
+00014850: 0451 0442 0020 043f 0443 0441 0442 0800  .Q.B. .?.C.A.B..
+00014860: 0000 0006 0000 0013 5461 7820 7265 706f  ........Tax repo
+00014870: 7274 2069 7320 656d 7074 7907 0000 0009  rt is empty.....
+00014880: 5461 7857 6964 6765 7401 0300 0000 4004  TaxWidget.....@.
+00014890: 1d04 3004 3b04 3e04 3304 3e04 3204 4b04  ..0.;.>.3.>.2.K.
+000148a0: 3900 2004 3e04 4204 4704 5104 4200 2004  9. .>.B.G.Q.B. .
+000148b0: 4104 3e04 4504 4004 3004 3d04 5104 3d00  A.>.E.@.0.=.Q.=.
+000148c0: 2004 3200 2004 4404 3004 3904 3b00 2008   .2. .D.0.9.;. .
+000148d0: 0000 0000 0600 0000 1954 6178 2072 6570  .........Tax rep
+000148e0: 6f72 7420 7361 7665 6420 746f 2066 696c  ort saved to fil
+000148f0: 6520 0700 0000 0954 6178 5769 6467 6574  e .....TaxWidget
+00014900: 0103 0000 0040 041d 0430 043b 043e 0433  .....@...0.;.>.3
+00014910: 043e 0432 044b 0439 0020 043e 0442 0447  .>.2.K.9. .>.B.G
+00014920: 0451 0442 0020 0441 043e 0445 0440 0430  .Q.B. .A.>.E.@.0
+00014930: 043d 0451 043d 0020 0432 0020 0444 0430  .=.Q.=. .2. .D.0
+00014940: 0439 043b 0020 0800 0000 0006 0000 001d  .9.;. ..........
+00014950: 5461 7820 7265 706f 7274 2077 6173 2073  Tax report was s
+00014960: 6176 6564 2074 6f20 6669 6c65 2007 0000  aved to file ...
+00014970: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
+00014980: 0c04 1d04 3004 3b04 3e04 3304 3808 0000  ....0.;.>.3.8...
+00014990: 0000 0600 0000 0554 6178 6573 0700 0000  .......Taxes....
+000149a0: 0954 6178 5769 6467 6574 0103 0000 004e  .TaxWidget.....N
+000149b0: 041e 0431 043d 043e 0432 0438 0442 044c  ...1.=.>.2.8.B.L
+000149c0: 0020 0442 043e 043b 044c 043a 043e 0020  . .B.>.;.L.:.>. 
+000149d0: 0438 043d 0444 043e 0440 043c 0430 0446  .8.=.D.>.@.<.0.F
+000149e0: 0438 044e 0020 043e 0020 0434 0438 0432  .8.N. .>. .4.8.2
+000149f0: 0438 0434 0435 043d 0434 0430 0445 0800  .8.4.5.=.4.0.E..
+00014a00: 0000 0006 0000 0027 5570 6461 7465 206f  .......'Update o
+00014a10: 6e6c 7920 696e 666f 726d 6174 696f 6e20  nly information 
+00014a20: 6162 6f75 7420 6469 7669 6465 6e64 7307  about dividends.
+00014a30: 0000 0009 5461 7857 6964 6765 7401 0300  ....TaxWidget...
+00014a40: 0000 6404 1804 4104 3f04 3e04 3b04 4c04  ..d...A.?.>.;.L.
+00014a50: 3704 3e04 3204 3004 4204 4c00 2004 3d04  7.>.2.0.B.L. .=.
+00014a60: 3004 3704 3204 3004 3d04 3804 3500 2004  0.7.2.0.=.8.5. .
+00014a70: 3104 4004 3e04 3a04 3504 4004 3000 2004  1.@.>.:.5.@.0. .
+00014a80: 3a04 3004 3a00 2004 3804 4104 4204 3e04  :.0.:. .8.A.B.>.
+00014a90: 4704 3d04 3804 3a00 2004 3204 4b04 3f04  G.=.8.:. .2.K.?.
+00014aa0: 3b04 3004 4204 4b08 0000 0000 0600 0000  ;.0.B.K.........
+00014ab0: 2055 7365 2062 726f 6b65 7220 6e61 6d65   Use broker name
+00014ac0: 2061 7320 696e 636f 6d65 2073 6f75 7263   as income sourc
+00014ad0: 6507 0000 0009 5461 7857 6964 6765 7401  e.....TaxWidget.
+00014ae0: 0300 0000 0804 1304 3e04 3400 3a08 0000  ........>.4.:...
+00014af0: 0000 0600 0000 0559 6561 723a 0700 0000  .......Year:....
+00014b00: 0954 6178 5769 6467 6574 0103 0000 0050  .TaxWidget.....P
+00014b10: 0412 044b 0020 043d 0435 0020 0432 044b  ...K. .=.5. .2.K
+00014b20: 0431 0440 0430 043b 0438 0020 0441 0447  .1.@.0.;.8. .A.G
+00014b30: 0451 0442 0020 0434 043b 044f 0020 043d  .Q.B. .4.;.O. .=
+00014b40: 0430 043b 043e 0433 043e 0432 043e 0433  .0.;.>.3.>.2.>.3
+00014b50: 043e 0020 043e 0442 0447 0451 0442 0430  .>. .>.B.G.Q.B.0
+00014b60: 0800 0000 0006 0000 002e 596f 7520 6861  ..........You ha
+00014b70: 7665 6e27 7420 7365 6c65 6374 6564 2061  ven't selected a
+00014b80: 6e20 6163 636f 756e 7420 666f 7220 7461  n account for ta
+00014b90: 7820 7265 706f 7274 0700 0000 0954 6178  x report.....Tax
+00014ba0: 5769 6467 6574 0103 0000 0098 041d 0435  Widget.........5
+00014bb0: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
+00014bc0: 0020 043e 0431 0440 0430 0431 043e 0442  . .>.1.@.0.1.>.B
+00014bd0: 0430 0442 044c 0020 0441 0434 0435 043b  .0.B.L. .A.4.5.;
+00014be0: 043a 0443 002c 0020 0442 002e 043a 002e  .:.C.,. .B...:..
+00014bf0: 0020 043d 0435 0020 0437 0430 0434 0430  . .=.5. .7.0.4.0
+00014c00: 043d 0020 0431 0430 043d 043a 0020 0434  .=. .1.0.=.:. .4
+00014c10: 043b 044f 0020 0438 043d 0432 0435 0441  .;.O. .8.=.2.5.A
+00014c20: 0442 0438 0446 0438 043e 043d 043d 043e  .B.8.F.8.>.=.=.>
+00014c30: 0433 043e 0020 0441 0447 0451 0442 0430  .3.>. .A.G.Q.B.0
+00014c40: 003a 0020 0800 0000 0006 0000 003e 4361  .:. .........>Ca
+00014c50: 6e27 7420 7072 6f63 6573 7320 7472 6164  n't process trad
+00014c60: 6520 6173 2062 616e 6b20 6973 6e27 7420  e as bank isn't 
+00014c70: 7365 7420 666f 7220 696e 7665 7374 6d65  set for investme
+00014c80: 6e74 2061 6363 6f75 6e74 3a20 0700 0000  nt account: ....
+00014c90: 0554 7261 6465 0103 0000 0002 2116 0800  .Trade......!...
+00014ca0: 0000 0006 0000 0001 2307 0000 000b 5472  ........#.....Tr
+00014cb0: 6164 6557 6964 6765 7401 0300 0000 0804  adeWidget.......
+00014cc0: 2104 4704 3504 4208 0000 0000 0600 0000  !.G.5.B.........
+00014cd0: 0741 6363 6f75 6e74 0700 0000 0b54 7261  .Account.....Tra
+00014ce0: 6465 5769 6467 6574 0103 0000 0004 0426  deWidget.......&
+00014cf0: 0411 0800 0000 0006 0000 0005 4173 7365  ............Asse
+00014d00: 7407 0000 000b 5472 6164 6557 6964 6765  t.....TradeWidge
+00014d10: 7401 0300 0000 2204 1f04 3e04 3a04 4304  t....."...>.:.C.
+00014d20: 3f04 3a04 3000 2000 2f00 2004 1f04 4004  ?.:.0. ./. ...@.
+00014d30: 3e04 3404 3004 3604 3008 0000 0000 0600  >.4.0.6.0.......
+00014d40: 0000 0a42 7579 202f 2053 656c 6c07 0000  ...Buy / Sell...
+00014d50: 000b 5472 6164 6557 6964 6765 7401 0300  ..TradeWidget...
+00014d60: 0000 1404 1404 3004 4204 3000 2f04 1204  ......0.B.0./...
+00014d70: 4004 3504 3c04 4f08 0000 0000 0600 0000  @.5.<.O.........
+00014d80: 0944 6174 652f 5469 6d65 0700 0000 0b54  .Date/Time.....T
+00014d90: 7261 6465 5769 6467 6574 0103 0000 0010  radeWidget......
+00014da0: 041a 043e 043c 0438 0441 0441 0438 044f  ...>.<.8.A.A.8.O
+00014db0: 0800 0000 0006 0000 0003 4665 6507 0000  ..........Fee...
+00014dc0: 000b 5472 6164 6557 6964 6765 7401 0300  ..TradeWidget...
+00014dd0: 0000 1004 1e04 3f04 3804 4104 3004 3d04  ......?.8.A.0.=.
+00014de0: 3804 3508 0000 0000 0600 0000 044e 6f74  8.5..........Not
+00014df0: 6507 0000 000b 5472 6164 6557 6964 6765  e.....TradeWidge
+00014e00: 7401 0300 0000 0804 2604 3504 3d04 3008  t.......&.5.=.0.
+00014e10: 0000 0000 0600 0000 0550 7269 6365 0700  .........Price..
+00014e20: 0000 0b54 7261 6465 5769 6467 6574 0103  ...TradeWidget..
+00014e30: 0000 000c 041a 043e 043b 002d 0432 043e  .......>.;.-.2.>
+00014e40: 0800 0000 0006 0000 0003 5174 7907 0000  ..........Qty...
+00014e50: 000b 5472 6164 6557 6964 6765 7401 0300  ..TradeWidget...
+00014e60: 0000 1a04 1404 3004 4204 3000 2004 4004  ......0.B.0. .@.
+00014e70: 3004 4104 4704 3504 4204 3e04 3208 0000  0.A.G.5.B.>.2...
+00014e80: 0000 0600 0000 0a53 6574 746c 656d 656e  .......Settlemen
+00014e90: 7407 0000 000b 5472 6164 6557 6964 6765  t.....TradeWidge
+00014ea0: 7401 0300 0000 7a04 1a04 3e04 3b04 3804  t.....z...>.;.8.
+00014eb0: 4704 3504 4104 4204 3204 3e00 2004 3004  G.5.A.B.2.>. .0.
+00014ec0: 3a04 4204 3804 3204 3000 2004 3d04 3504  :.B.8.2.0. .=.5.
+00014ed0: 3404 3e04 4104 4204 3004 4204 3e04 4704  4.>.A.B.0.B.>.G.
+00014ee0: 3d04 3e00 2004 3404 3b04 4f00 2004 3e04  =.>. .4.;.O. .>.
+00014ef0: 3104 4004 3004 3104 3e04 4204 3a04 3800  1.@.0.1.>.B.:.8.
+00014f00: 2004 3f04 3504 4004 3504 3204 3e04 3404   .?.5.@.5.2.>.4.
+00014f10: 3000 2e00 2004 1404 3004 4204 3000 3a00  0... ...0.B.0.:.
+00014f20: 2008 0000 0000 0600 0000 4041 7373 6574   .........@Asset
+00014f30: 2061 6d6f 756e 7420 6973 206e 6f74 2065   amount is not e
+00014f40: 6e6f 7567 6820 666f 7220 6173 7365 7420  nough for asset 
+00014f50: 7472 616e 7366 6572 2070 726f 6365 7373  transfer process
+00014f60: 696e 672e 2044 6174 653a 2007 0000 0008  ing. Date: .....
+00014f70: 5472 616e 7366 6572 0103 0000 0052 0421  Transfer.....R.!
+00014f80: 043f 0438 0441 0430 043d 0438 0435 0020  .?.8.A.0.=.8.5. 
+00014f90: 0430 043a 0442 0438 0432 0430 0020 043d  .0.:.B.8.2.0. .=
+00014fa0: 0435 0020 043d 0430 0439 0434 0435 043d  .5. .=.0.9.4.5.=
+00014fb0: 043e 0020 0434 043b 044f 0020 0442 0440  .>. .4.;.O. .B.@
+00014fc0: 0430 043d 0441 0444 0435 0440 0430 002e  .0.=.A.D.5.@.0..
+00014fd0: 0800 0000 0006 0000 0028 4173 7365 7420  .........(Asset 
+00014fe0: 7769 7468 6472 6177 616c 206e 6f74 2066  withdrawal not f
+00014ff0: 6f75 6e64 2066 6f72 2074 7261 6e73 6665  ound for transfe
+00015000: 722e 0700 0000 0854 7261 6e73 6665 7201  r......Transfer.
+00015010: 0300 0000 2e04 1e04 4804 3804 3104 3a04  ........H.8.1.:.
+00015020: 3000 2e00 2004 1a04 4304 4004 4100 2004  0... ...C.@.A. .
+00015030: 4004 3004 3204 3504 3d00 2004 3d04 4304  @.0.2.5.=. .=.C.
+00015040: 3b04 4e08 0000 0000 0600 0000 1045 7272  ;.N..........Err
+00015050: 6f72 2e20 5a65 726f 2072 6174 6507 0000  or. Zero rate...
+00015060: 0008 5472 616e 7366 6572 0103 0000 0084  ..Transfer......
+00015070: 041e 0431 0440 0430 0431 043e 0442 0430  ...1.@.0.1.>.B.0
+00015080: 043d 043d 043e 0435 0020 043a 043e 043b  .=.=.>.5. .:.>.;
+00015090: 0438 0447 0435 0441 0442 0432 043e 0020  .8.G.5.A.B.2.>. 
+000150a0: 043c 0435 043d 044c 0448 0435 002c 0020  .<.5.=.L.H.5.,. 
+000150b0: 0447 0435 043c 0020 043a 043e 043b 0438  .G.5.<. .:.>.;.8
+000150c0: 0447 0435 0441 0442 0432 043e 0020 0432  .G.5.A.B.2.>. .2
+000150d0: 0020 0442 0440 0430 043d 0441 0444 0435  . .B.@.0.=.A.D.5
+000150e0: 0440 0435 002e 0020 0414 0430 0442 0430  .@.5... ...0.B.0
+000150f0: 003a 0020 0800 0000 0006 0000 003b 5072  .:. .........;Pr
+00015100: 6f63 6573 7365 6420 6173 7365 7420 616d  ocessed asset am
+00015110: 6f75 6e74 2069 7320 6c65 7373 2074 6861  ount is less tha
+00015120: 6e20 7472 616e 7366 6572 2061 6d6f 756e  n transfer amoun
+00015130: 742e 2044 6174 653a 2007 0000 0008 5472  t. Date: .....Tr
+00015140: 616e 7366 6572 0103 0000 0002 2116 0800  ansfer......!...
+00015150: 0000 0006 0000 0001 2307 0000 000e 5472  ........#.....Tr
+00015160: 616e 7366 6572 5769 6467 6574 0103 0000  ansferWidget....
+00015170: 000a 0421 0443 043c 043c 0430 0800 0000  ...!.C.<.<.0....
+00015180: 0006 0000 0006 416d 6f75 6e74 0700 0000  ......Amount....
+00015190: 0e54 7261 6e73 6665 7257 6964 6765 7401  .TransferWidget.
+000151a0: 0300 0000 0404 2604 1108 0000 0000 0600  ......&.........
+000151b0: 0000 0541 7373 6574 0700 0000 0e54 7261  ...Asset.....Tra
 000151c0: 6e73 6665 7257 6964 6765 7401 0300 0000  nsferWidget.....
-000151d0: 0404 1f04 3e08 0000 0000 0600 0000 0845  ....>..........E
-000151e0: 6e64 2064 6174 6507 0000 000f 5570 6461  nd date.....Upda
-000151f0: 7465 5175 6f74 6573 446c 6701 0300 0000  teQuotesDlg.....
-00015200: 1204 1804 4104 4204 3e04 4704 3d04 3804  ....A.B.>.G.=.8.
-00015210: 3a04 3808 0000 0000 0600 0000 0753 6f75  :.8..........Sou
-00015220: 7263 6573 0700 0000 0f55 7064 6174 6551  rces.....UpdateQ
-00015230: 756f 7465 7344 6c67 0103 0000 0002 0421  uotesDlg.......!
-00015240: 0800 0000 0006 0000 000a 5374 6172 7420  ..........Start 
-00015250: 6461 7465 0700 0000 0f55 7064 6174 6551  date.....UpdateQ
-00015260: 756f 7465 7344 6c67 0103 0000 0028 041e  uotesDlg.....(..
-00015270: 0431 043d 043e 0432 043b 0435 043d 0438  .1.=.>.2.;.5.=.8
-00015280: 0435 0020 043a 043e 0442 0438 0440 043e  .5. .:.>.B.8.@.>
-00015290: 0432 043e 043a 0800 0000 0006 0000 0015  .2.>.:..........
-000152a0: 5570 6461 7465 2061 7373 6574 2773 2071  Update asset's q
-000152b0: 756f 7465 7307 0000 000f 5570 6461 7465  uotes.....Update
-000152c0: 5175 6f74 6573 446c 6701 0300 0000 1400  QuotesDlg.......
-000152d0: 6400 6400 2f00 4d00 4d00 2f00 7900 7900  d.d./.M.M./.y.y.
-000152e0: 7900 7908 0000 0000 0600 0000 0a64 642f  y.y..........dd/
-000152f0: 4d4d 2f79 7979 7907 0000 000f 5570 6461  MM/yyyy.....Upda
-00015300: 7465 5175 6f74 6573 446c 6701 0300 0000  teQuotesDlg.....
-00015310: 5804 1d04 3504 3204 3e04 3704 3c04 3e04  X...5.2.>.7.<.>.
-00015320: 3604 3d04 3e00 2004 3f04 4004 3e04 4704  6.=.>. .?.@.>.G.
-00015330: 3804 4204 3004 4204 4c00 2004 4804 3004  8.B.0.B.L. .H.0.
-00015340: 3104 3b04 3e04 3d00 2004 3e04 4204 4704  1.;.>.=. .>.B.G.
-00015350: 5104 4204 3000 2004 3804 3700 2004 4404  Q.B.0. .8.7. .D.
-00015360: 3004 3904 3b04 3000 2008 0000 0000 0600  0.9.;.0. .......
-00015370: 0000 2543 616e 2774 206c 6f61 6420 7265  ..%Can't load re
-00015380: 706f 7274 2074 656d 706c 6174 6520 6672  port template fr
-00015390: 6f6d 2066 696c 6520 0700 0000 0458 4c53  om file .....XLS
-000153a0: 5801 0300 0000 4404 1d04 3504 3204 3e04  X.....D...5.2.>.
-000153b0: 3704 3c04 3e04 3604 3d04 3e00 2004 4104  7.<.>.6.=.>. .A.
-000153c0: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
-000153d0: 2004 3e04 4204 4704 5104 4200 2004 3200   .>.B.G.Q.B. .2.
-000153e0: 2004 4404 3004 3904 3b00 2008 0000 0000   .D.0.9.;. .....
-000153f0: 0600 0000 1c43 616e 2774 2073 6176 6520  .....Can't save 
-00015400: 7265 706f 7274 2069 6e74 6f20 6669 6c65  report into file
-00015410: 2007 0000 0004 584c 5358 0103 0000 0044   .....XLSX.....D
-00015420: 041d 0435 0020 0443 043a 0430 0437 0430  ...5. .C.:.0.7.0
-00015430: 043d 0020 0444 043e 0440 043c 0430 0442  .=. .D.>.@.<.0.B
-00015440: 0020 0434 043b 044f 0020 043f 043e 043b  . .4.;.O. .?.>.;
-00015450: 044f 0020 043e 0442 0447 0451 0442 0430  .O. .>.B.G.Q.B.0
-00015460: 003a 0020 0800 0000 0006 0000 0024 466f  .:. .........$Fo
-00015470: 726d 6174 2069 7320 6d69 7373 696e 6720  rmat is missing 
-00015480: 666f 7220 7265 706f 7274 2066 6965 6c64  for report field
-00015490: 3a20 0700 0000 0458 4c53 5801 0300 0000  : .....XLSX.....
-000154a0: 4204 1d04 3500 2004 3704 3004 3404 3004  B...5. .7.0.4.0.
-000154b0: 3d00 2004 4804 3004 3104 3b04 3e04 3d00  =. .H.0.1.;.>.=.
-000154c0: 2004 3404 3b04 4f00 2004 3404 3004 3d04   .4.;.O. .4.0.=.
-000154d0: 3d04 4b04 4500 2004 3e04 4204 4704 5104  =.K.E. .>.B.G.Q.
-000154e0: 4204 3008 0000 0000 0600 0000 1a4e 6f20  B.0..........No 
-000154f0: 7265 706f 7274 2072 6f77 2074 656d 706c  report row templ
-00015500: 6174 6520 7365 7407 0000 0004 584c 5358  ate set.....XLSX
-00015510: 0103 0000 003a 0428 0430 0431 043b 043e  .....:.(.0.1.;.>
-00015520: 043d 0020 0434 043b 044f 0020 0434 0430  .=. .4.;.O. .4.0
-00015530: 043d 043d 044b 0445 0020 043d 0435 0020  .=.=.K.E. .=.5. 
-00015540: 043d 0430 0439 0434 0435 043d 003a 0020  .=.0.9.4.5.=.:. 
-00015550: 0800 0000 0006 0000 001f 5265 706f 7274  ..........Report
-00015560: 2072 6f77 2074 656d 706c 6174 6520 6e6f   row template no
-00015570: 7420 666f 756e 643a 2007 0000 0004 584c  t found: .....XL
-00015580: 5358 0103 0000 0046 041d 0435 0438 0437  SX.....F...5.8.7
-00015590: 0432 0435 0441 0442 043d 0430 044f 0020  .2.5.A.B.=.0.O. 
-000155a0: 0441 0442 0440 043e 043a 0430 0020 0444  .A.B.@.>.:.0. .D
-000155b0: 043e 0440 043c 0430 0442 0438 0440 043e  .>.@.<.0.B.8.@.>
-000155c0: 0432 0430 043d 0438 044f 003a 0020 0800  .2.0.=.8.O.:. ..
-000155d0: 0000 0006 0000 001c 556e 7265 636f 676e  ........Unrecogn
-000155e0: 697a 6564 2066 6f72 6d61 7420 7374 7269  ized format stri
-000155f0: 6e67 3a20 0700 0000 0458 4c53 5801 8800  ng: .....XLSX...
-00015600: 0000 0d11 01fd 290b ff14 0204 fd2c 0a13  ......)......,..
+000151d0: 1404 1404 3004 4204 3000 2f04 1204 4004  ....0.B.0./...@.
+000151e0: 3504 3c04 4f08 0000 0000 0600 0000 0944  5.<.O..........D
+000151f0: 6174 652f 5469 6d65 0700 0000 0e54 7261  ate/Time.....Tra
+00015200: 6e73 6665 7257 6964 6765 7401 0300 0000  nsferWidget.....
+00015210: 1e04 2004 3004 3704 3c04 3504 4000 2004  .. .0.7.<.5.@. .
+00015220: 3a04 3e04 3c04 3804 4104 4104 3804 3808  :.>.<.8.A.A.8.8.
+00015230: 0000 0000 0600 0000 0a46 6565 2061 6d6f  .........Fee amo
+00015240: 756e 7407 0000 000e 5472 616e 7366 6572  unt.....Transfer
+00015250: 5769 6467 6574 0103 0000 0016 041a 043e  Widget.........>
+00015260: 043c 043c 0438 0441 0441 0438 044f 0020  .<.<.8.A.A.8.O. 
+00015270: 0441 0800 0000 0006 0000 0008 4665 6520  .A..........Fee 
+00015280: 6672 6f6d 0700 0000 0e54 7261 6e73 6665  from.....Transfe
+00015290: 7257 6964 6765 7401 0300 0000 0204 2108  rWidget.......!.
+000152a0: 0000 0000 0600 0000 0446 726f 6d07 0000  .........From...
+000152b0: 000e 5472 616e 7366 6572 5769 6467 6574  ..TransferWidget
+000152c0: 0103 0000 0010 041e 043f 0438 0441 0430  .........?.8.A.0
+000152d0: 043d 0438 0435 0800 0000 0006 0000 0004  .=.8.5..........
+000152e0: 4e6f 7465 0700 0000 0e54 7261 6e73 6665  Note.....Transfe
+000152f0: 7257 6964 6765 7401 0300 0000 0404 1d04  rWidget.........
+00015300: 3008 0000 0000 0600 0000 0254 6f07 0000  0..........To...
+00015310: 000e 5472 616e 7366 6572 5769 6467 6574  ..TransferWidget
+00015320: 0103 0000 000e 041f 0435 0440 0435 0432  .........5.@.5.2
+00015330: 043e 0434 0800 0000 0006 0000 0008 5472  .>.4..........Tr
+00015340: 616e 7366 6572 0700 0000 0e54 7261 6e73  ansfer.....Trans
+00015350: 6665 7257 6964 6765 7401 0300 0000 0404  ferWidget.......
+00015360: 1f04 3e08 0000 0000 0600 0000 0845 6e64  ..>..........End
+00015370: 2064 6174 6507 0000 000f 5570 6461 7465   date.....Update
+00015380: 5175 6f74 6573 446c 6701 0300 0000 1204  QuotesDlg.......
+00015390: 1804 4104 4204 3e04 4704 3d04 3804 3a04  ..A.B.>.G.=.8.:.
+000153a0: 3808 0000 0000 0600 0000 0753 6f75 7263  8..........Sourc
+000153b0: 6573 0700 0000 0f55 7064 6174 6551 756f  es.....UpdateQuo
+000153c0: 7465 7344 6c67 0103 0000 0002 0421 0800  tesDlg.......!..
+000153d0: 0000 0006 0000 000a 5374 6172 7420 6461  ........Start da
+000153e0: 7465 0700 0000 0f55 7064 6174 6551 756f  te.....UpdateQuo
+000153f0: 7465 7344 6c67 0103 0000 0028 041e 0431  tesDlg.....(...1
+00015400: 043d 043e 0432 043b 0435 043d 0438 0435  .=.>.2.;.5.=.8.5
+00015410: 0020 043a 043e 0442 0438 0440 043e 0432  . .:.>.B.8.@.>.2
+00015420: 043e 043a 0800 0000 0006 0000 0015 5570  .>.:..........Up
+00015430: 6461 7465 2061 7373 6574 2773 2071 756f  date asset's quo
+00015440: 7465 7307 0000 000f 5570 6461 7465 5175  tes.....UpdateQu
+00015450: 6f74 6573 446c 6701 0300 0000 1400 6400  otesDlg.......d.
+00015460: 6400 2f00 4d00 4d00 2f00 7900 7900 7900  d./.M.M./.y.y.y.
+00015470: 7908 0000 0000 0600 0000 0a64 642f 4d4d  y..........dd/MM
+00015480: 2f79 7979 7907 0000 000f 5570 6461 7465  /yyyy.....Update
+00015490: 5175 6f74 6573 446c 6701 0300 0000 5804  QuotesDlg.....X.
+000154a0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
+000154b0: 3d04 3e00 2004 3f04 4004 3e04 4704 3804  =.>. .?.@.>.G.8.
+000154c0: 4204 3004 4204 4c00 2004 4804 3004 3104  B.0.B.L. .H.0.1.
+000154d0: 3b04 3e04 3d00 2004 3e04 4204 4704 5104  ;.>.=. .>.B.G.Q.
+000154e0: 4204 3000 2004 3804 3700 2004 4404 3004  B.0. .8.7. .D.0.
+000154f0: 3904 3b04 3000 2008 0000 0000 0600 0000  9.;.0. .........
+00015500: 2543 616e 2774 206c 6f61 6420 7265 706f  %Can't load repo
+00015510: 7274 2074 656d 706c 6174 6520 6672 6f6d  rt template from
+00015520: 2066 696c 6520 0700 0000 0458 4c53 5801   file .....XLSX.
+00015530: 0300 0000 4404 1d04 3504 3204 3e04 3704  ....D...5.2.>.7.
+00015540: 3c04 3e04 3604 3d04 3e00 2004 4104 3e04  <.>.6.=.>. .A.>.
+00015550: 4504 4004 3004 3d04 3804 4204 4c00 2004  E.@.0.=.8.B.L. .
+00015560: 3e04 4204 4704 5104 4200 2004 3200 2004  >.B.G.Q.B. .2. .
+00015570: 4404 3004 3904 3b00 2008 0000 0000 0600  D.0.9.;. .......
+00015580: 0000 1c43 616e 2774 2073 6176 6520 7265  ...Can't save re
+00015590: 706f 7274 2069 6e74 6f20 6669 6c65 2007  port into file .
+000155a0: 0000 0004 584c 5358 0103 0000 0044 041d  ....XLSX.....D..
+000155b0: 0435 0020 0443 043a 0430 0437 0430 043d  .5. .C.:.0.7.0.=
+000155c0: 0020 0444 043e 0440 043c 0430 0442 0020  . .D.>.@.<.0.B. 
+000155d0: 0434 043b 044f 0020 043f 043e 043b 044f  .4.;.O. .?.>.;.O
+000155e0: 0020 043e 0442 0447 0451 0442 0430 003a  . .>.B.G.Q.B.0.:
+000155f0: 0020 0800 0000 0006 0000 0024 466f 726d  . .........$Form
+00015600: 6174 2069 7320 6d69 7373 696e 6720 666f  at is missing fo
+00015610: 7220 7265 706f 7274 2066 6965 6c64 3a20  r report field: 
+00015620: 0700 0000 0458 4c53 5801 0300 0000 4204  .....XLSX.....B.
+00015630: 1d04 3500 2004 3704 3004 3404 3004 3d00  ..5. .7.0.4.0.=.
+00015640: 2004 4804 3004 3104 3b04 3e04 3d00 2004   .H.0.1.;.>.=. .
+00015650: 3404 3b04 4f00 2004 3404 3004 3d04 3d04  4.;.O. .4.0.=.=.
+00015660: 4b04 4500 2004 3e04 4204 4704 5104 4204  K.E. .>.B.G.Q.B.
+00015670: 3008 0000 0000 0600 0000 1a4e 6f20 7265  0..........No re
+00015680: 706f 7274 2072 6f77 2074 656d 706c 6174  port row templat
+00015690: 6520 7365 7407 0000 0004 584c 5358 0103  e set.....XLSX..
+000156a0: 0000 003a 0428 0430 0431 043b 043e 043d  ...:.(.0.1.;.>.=
+000156b0: 0020 0434 043b 044f 0020 0434 0430 043d  . .4.;.O. .4.0.=
+000156c0: 043d 044b 0445 0020 043d 0435 0020 043d  .=.K.E. .=.5. .=
+000156d0: 0430 0439 0434 0435 043d 003a 0020 0800  .0.9.4.5.=.:. ..
+000156e0: 0000 0006 0000 001f 5265 706f 7274 2072  ........Report r
+000156f0: 6f77 2074 656d 706c 6174 6520 6e6f 7420  ow template not 
+00015700: 666f 756e 643a 2007 0000 0004 584c 5358  found: .....XLSX
+00015710: 0103 0000 0046 041d 0435 0438 0437 0432  .....F...5.8.7.2
+00015720: 0435 0441 0442 043d 0430 044f 0020 0441  .5.A.B.=.0.O. .A
+00015730: 0442 0440 043e 043a 0430 0020 0444 043e  .B.@.>.:.0. .D.>
+00015740: 0440 043c 0430 0442 0438 0440 043e 0432  .@.<.0.B.8.@.>.2
+00015750: 0430 043d 0438 044f 003a 0020 0800 0000  .0.=.8.O.:. ....
+00015760: 0006 0000 001c 556e 7265 636f 676e 697a  ......Unrecogniz
+00015770: 6564 2066 6f72 6d61 7420 7374 7269 6e67  ed format string
+00015780: 3a20 0700 0000 0458 4c53 5801 8800 0000  : .....XLSX.....
+00015790: 0d11 01fd 290b ff14 0204 fd2c 0a13       ....)......,..
```

### Comparing `jal-2023.4.6/jal/net/downloader.py` & `jal-2023.4.7/jal/net/downloader.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/net/helpers.py` & `jal-2023.4.7/jal/net/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/pypi_description.md` & `jal-2023.4.7/jal/pypi_description.md`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/reports/category.py` & `jal-2023.4.7/jal/reports/category.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/reports/deals.py` & `jal-2023.4.7/jal/reports/deals.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/reports/holdings.py` & `jal-2023.4.7/jal/reports/holdings.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/reports/income_spending.py` & `jal-2023.4.7/jal/reports/income_spending.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,37 +5,55 @@
 from PySide6.QtWidgets import QMenu
 from jal.reports.reports import Reports
 from jal.db.asset import JalAsset
 from jal.ui.reports.ui_income_spending_report import Ui_IncomeSpendingReportWidget
 from jal.constants import CustomColor
 from jal.db.helpers import load_icon
 from jal.db.category import JalCategory
-from jal.widgets.helpers import is_signal_connected, month_list, month_start_ts, month_end_ts
+from jal.widgets.helpers import is_signal_connected, month_list, month_start_ts, month_end_ts, \
+    week_list, week_start_ts, week_end_ts, str2int
 from jal.widgets.delegates import GridLinesDelegate, FloatDelegate
 from jal.widgets.mdi import MdiWidget
 
 JAL_REPORT_CLASS = "IncomeSpendingReport"
 
+MONTHLY = 12
+WEEKLY = 53
+
 
 # ----------------------------------------------------------------------------------------------------------------------
-class ReportTreeItem:
-    def __init__(self, begin, end, item_id, name, parent=None):
+class ReportTreeItem(QObject):
+    def __init__(self, begin, end, item_id, name, periods=MONTHLY, parent=None):
+        super().__init__()
         self._parent = parent
+        if parent is not None:
+            self._periods = parent.periods   # Child should have the same periodicity as parent
+        else:
+            self._periods = periods
         self._id = item_id
         self.name = name
         self._begin = begin
         self._end = end
         self._y_s = int(datetime.utcfromtimestamp(begin).strftime('%Y'))
-        self._m_s = int(datetime.utcfromtimestamp(begin).strftime('%m').lstrip('0'))
         self._y_e = int(datetime.utcfromtimestamp(end).strftime('%Y'))
-        self._m_e = int(datetime.utcfromtimestamp(end).strftime('%m').lstrip('0'))
+        if self._periods == MONTHLY:
+            self._p_s = str2int(datetime.utcfromtimestamp(begin).strftime('%m'))
+            self._p_e = str2int(datetime.utcfromtimestamp(end).strftime('%m'))
+        elif self._periods == WEEKLY:
+            self._p_s = str2int(datetime.utcfromtimestamp(begin).strftime('%W'))
+            if self._p_s == 0:  # This is a week that starts a year before
+                self._y_s -= 1
+                self._p_s = 53
+            self._p_e = str2int(datetime.utcfromtimestamp(end).strftime('%W'))
+        else:
+            assert False, "Wrong period for Income/Spending report"
         # amounts is 2D-array of per month amounts:
-        # amounts[year][month] - amount for particular month
+        # amounts[year][period_id] - amount for particular month (period_id from 1 to 12) or week (from 1 to 53)
         # amounts[year][0] - total per year
-        self._amounts = [ [0] * 13 for _ in range(self._y_e - self._y_s + 1)]
+        self._amounts = [[0] * (self._periods + 1) for _ in range(self._y_e - self._y_s + 1)]
         self._total = 0
         self._children = []
 
     def appendChild(self, child):
         child.setParent(self)
         self._children.append(child)
 
@@ -50,116 +68,137 @@
     def removeEmptyChildren(self):
         for child in self._children:
             child.removeEmptyChildren()
         self._children = [x for x in self._children if x.getAmount(0, 0) != 0]
 
     def dataCount(self):
         if self._y_s == self._y_e:
-            return self._m_e - self._m_s + 3  # + 1 for year, + 1 for totals
+            return self._p_e - self._p_s + 3  # + 1 for year, + 1 for totals
         else:
-            # 13 * (self._y_e - self._y_s - 1) + (self._m_e + 1) + (12 - self._m_s + 2) + 1 simplified to:
-            return 13 * (self._y_e - self._y_s - 1) + (self._m_e - self._m_s + 16)
+            # (self._periods + 1) * (self._y_e - self._y_s - 1) + (self._p_e + 1) + (self._periods - self._p_s + 2) + 1 simplified to:
+            return (self._periods + 1) * (self._y_e - self._y_s - 1) + (self._p_e - self._p_s + self._periods + 4)
 
-    def column2calendar(self, column):
-        # column 0 - name of row - return (-1, -1)
-        # then repetition of [year], [jan], [feb] ... [nov], [dec] - return (year, 0), (year, 1) ... (year, 12)
-        # last column is total value - return (0, 0)
+    # Converts table column number into (year, period_id) value
+    # column 0 - name of row - return (-1, -1)
+    # then repetition of [year], [jan], [feb] ... [nov], [dec] - return (year, 0), (year, 1) ... (year, 12)
+    # or repetition of [year], [wk1], [wk2] .. [wk53] - return (year, 0), (year, 1) ... (year, 53)
+    # last column is total value - return (0, 0)
+    def column2calendar(self, column: int) -> (int, int):
         if column == 0:
             return -1, -1
         if column == self.dataCount():
             return 0, 0
         if column == 1:
             return self._y_s, 0
-        column = column + self._m_s - 2
-        year = self._y_s + int(column / 13)
-        month = column % 13
-        return year, month
+        column = column + self._p_s - 2
+        year = self._y_s + int(column / (self._periods + 1))
+        period_id = column % (self._periods + 1)
+        return year, period_id
+
+    def period_name(self, period_id: int) -> str:
+        month_name = [
+            self.tr('Jan'), self.tr('Feb'), self.tr('Mar'), self.tr('Apr'), self.tr('May'), self.tr('Jun'),
+            self.tr('Jul'), self.tr('Aug'), self.tr('Sep'), self.tr('Oct'), self.tr('Nov'), self.tr('Dec')
+        ]
+        if self._periods == MONTHLY:
+            return month_name[period_id - 1]
+        elif self._periods == WEEKLY:
+            prefix = self.tr("wk")   # On separate line as it won't be extracted for translation otherwise
+            return f"{prefix}{period_id}"
+        else:
+            assert False, "Wrong period for Income/Spending report"
 
     def setParent(self, parent):
         self._parent = parent
 
     def getParent(self):
         return self._parent
 
-    def addAmount(self, year, month, amount):
+    def addAmount(self, year, period_id, amount):
         y_i = year - self._y_s
-        self._amounts[y_i][month] += amount
+        self._amounts[y_i][period_id] += amount
         self._amounts[y_i][0] += amount
         self._total += amount
         if self._parent is not None:
-            self._parent.addAmount(year, month, amount)
+            self._parent.addAmount(year, period_id, amount)
 
-    # Return amount for given date and month or total amount if year==0
-    def getAmount(self, year, month):
+    # Return amount for given year and period or total amount if year==0
+    def getAmount(self, year, period_id):
         if year == 0:
             return self._total
         y_i = year - self._y_s
-        return self._amounts[y_i][month]
+        return self._amounts[y_i][period_id]
 
     def getLeafById(self, id):
         if self._id == id:
             return self
         leaf = None
         for child in self._children:
             leaf = child.getLeafById(id)
         return leaf
 
-    def details(self, year, month):
-        if month == 0:
-            m_begin = 1
-            m_end = 12
+    def details(self, year, period_id):
+        if period_id == 0:
+            p_begin = 1
+            p_end = self._periods
         else:
-            m_begin = m_end = month
+            p_begin = p_end = period_id
         if year == 0:
             begin_ts = self._begin
             end_ts = self._end
+        elif self._periods == MONTHLY:
+            begin_ts = month_start_ts(year, p_begin) if month_start_ts(year, p_begin) > self._begin else self._begin
+            end_ts = month_end_ts(year, p_end) if month_end_ts(year, p_end) < self._end else self._end
+        elif self._periods == WEEKLY:
+            begin_ts = week_start_ts(year, p_begin) if week_start_ts(year, p_begin) > self._begin else self._begin
+            end_ts = week_end_ts(year, p_end) if week_end_ts(year, p_end) < self._end else self._end
         else:
-            begin_ts = month_start_ts(year, m_begin) if month_start_ts(year, m_begin) > self._begin else self._begin
-            end_ts = month_end_ts(year, m_end) if month_end_ts(year, m_end) < self._end else self._end
+            assert False, "Wrong period for Income/Spending report"
         item_summary = {
             'category_id': self._id,
             'begin_ts': begin_ts,
             'end_ts': end_ts,
-            'total': self.getAmount(year, month)
+            'total': self.getAmount(year, period_id)
         }
         return item_summary
 
     @property
     def year_begin(self):
         return self._y_s
 
     @property
-    def month_begin(self):
-        return self._m_s
+    def period_begin(self):
+        return self._p_s
 
     @property
     def year_end(self):
         return self._y_e
 
     @property
-    def month_end(self):
-        return self._m_e
+    def period_end(self):
+        return self._p_e
+
+    @property
+    def periods(self):
+        return self._periods
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class IncomeSpendingReportModel(QAbstractItemModel):
     def __init__(self, parent_view):
         super().__init__(parent_view)
+        self._periodicity = MONTHLY
         self._begin = 0
         self._end = 0
         self._currency = 0
-        self._month_list = []
+        self._period_list = []
         self._view = parent_view
         self._root = None
         self._grid_delegate = None
         self._float_delegate = None
-        self.month_name = [
-            self.tr('Jan'), self.tr('Feb'), self.tr('Mar'), self.tr('Apr'), self.tr('May'), self.tr('Jun'),
-            self.tr('Jul'), self.tr('Aug'), self.tr('Sep'), self.tr('Oct'), self.tr('Nov'), self.tr('Dec')
-        ]
 
     def rowCount(self, parent=None):
         if not parent.isValid():
             parent_item = self._root
         else:
             parent_item = parent.internalPointer()
         if parent_item is not None:
@@ -178,25 +217,25 @@
             return parent_item.dataCount() + 1  # + 1 for row header
         else:
             return 0
 
     def headerData(self, section, orientation, role=Qt.DisplayRole):
         if orientation == Qt.Horizontal:
             if role == Qt.DisplayRole:
-                year, month = self._root.column2calendar(section)
+                year, period = self._root.column2calendar(section)
                 if year < 0:
                     col_name = ''
                 elif year == 0:
                     col_name = self.tr("TOTAL")
                 else:
-                    if month == 0:
+                    if period == 0:
                         status = '▼' if self._view.isColumnHidden(section + 1) else '▶'
                         col_name = f"{year} " + status
                     else:
-                        col_name = self.month_name[month-1]
+                        col_name = self._root.period_name(period)
                 return col_name
             if role == Qt.TextAlignmentRole:
                 return int(Qt.AlignCenter)
         return None
 
     def headerWidth(self, section):
         return self._view.header().sectionSize(section)
@@ -224,34 +263,34 @@
         if not index.isValid():
             return None
         item = index.internalPointer()
         if role == Qt.DisplayRole:
             if index.column() == 0:
                 return item.name
             else:
-                year, month = self._root.column2calendar(index.column())
-                return item.getAmount(year, month)
+                year, period = self._root.column2calendar(index.column())
+                return item.getAmount(year, period)
         if role == Qt.ForegroundRole:
             if index.column() != 0:
-                year, month = self._root.column2calendar(index.column())
-                if item.getAmount(year, month) > 0:
+                year, period = self._root.column2calendar(index.column())
+                if item.getAmount(year, period) > 0:
                     return QBrush(CustomColor.DarkGreen)
-                elif item.getAmount(year, month) < 0:
+                elif item.getAmount(year, period) < 0:
                     return QBrush(CustomColor.DarkRed)
                 else:
                     return QBrush(CustomColor.Grey)
         if role == Qt.TextAlignmentRole:
             if index.column() == 0:
                 return int(Qt.AlignLeft)
             else:
                 return int(Qt.AlignRight)
         if role == Qt.UserRole:  # return category id for given index
             if index.column() != 0:
-                year, month = self._root.column2calendar(index.column())
-                return item.details(year, month)
+                year, period = self._root.column2calendar(index.column())
+                return item.details(year, period)
         return None
 
     def configureView(self):
         self._grid_delegate = GridLinesDelegate(self._view)
         self._float_delegate = FloatDelegate(2, allow_tail=False, parent=self._view)
         for column in range(self.columnCount()):
             if column == 0:
@@ -264,61 +303,74 @@
         font.setBold(True)
         self._view.header().setFont(font)
 
         if not is_signal_connected(self._view.header(), "sectionDoubleClicked(int)"):
             self._view.header().sectionDoubleClicked.connect(self.toggeYearColumns)
 
     def toggeYearColumns(self, section):
-        year, month = self._root.column2calendar(section)
-        if year >= 0 and month == 0:
+        year, period = self._root.column2calendar(section)
+        if year >= 0 and period == 0:
             if year == self._root.year_begin:
-                year_columns = 12 - self._root.month_begin + 1
+                year_columns = 12 - self._root.period_begin + 1
             elif year == self._root.year_end:
-                year_columns = self._root.month_end
+                year_columns = self._root.period_end
             else:
                 year_columns = 12
             for i in range(year_columns):
                 new_state = not self._view.isColumnHidden(section + i + 1)
                 self._view.setColumnHidden(section + i + 1, new_state)
             self.headerDataChanged.emit(Qt.Horizontal, section, section)
 
+    def setPeriod(self, period_id):
+        if period_id == 1:
+            self._periodicity = WEEKLY
+        else:
+            self._periodicity = MONTHLY
+        self.prepareData()
+        self.configureView()
+
     def setDatesRange(self, begin, end):
         self._begin = begin
         self._end = end
-        self._month_list = month_list(begin, end)
         self.prepareData()
         self.configureView()
 
     def setCurrency(self, currency_id):
         if self._currency != currency_id:
             self._currency = currency_id
             self.prepareData()
             self.configureView()
 
     def prepareData(self):
         if not self._currency:
             return
         root_category = JalCategory(0)
-        self._root = ReportTreeItem(self._begin, self._end, -1, "ROOT")  # invisible root
-        self._root.appendChild(ReportTreeItem(self._begin, self._end, 0, self.tr("TOTAL")))  # visible root
+        if self._periodicity == MONTHLY:
+            self._period_list = month_list(self._begin, self._end)
+        elif self._periodicity == WEEKLY:
+            self._period_list = week_list(self._begin, self._end)
+        else:
+            assert False, "Wrong period for Income/Spending report"
+        self._root = ReportTreeItem(self._begin, self._end, -1, "ROOT", periods=self._periodicity)  # invisible root
+        self._root.appendChild(ReportTreeItem(self._begin, self._end, 0, self.tr("TOTAL"), periods=self._periodicity))  # visible root
         self._load_child_amounts(root_category)
         self._root.removeEmptyChildren()
         self.modelReset.emit()
         self._view.expandAll()
 
     def _load_child_amounts(self, parent_category: JalCategory):
         for category in parent_category.get_child_categories():
             leaf = self._root.getLeafById(category.id())
             if leaf is None:
                 parent = self._root.getLeafById(category.parent_id())
-                leaf = ReportTreeItem(self._begin, self._end, category.id(), category.name(), parent)
+                leaf = ReportTreeItem(self._begin, self._end, category.id(), category.name(), parent=parent)
                 parent.appendChild(leaf)
-            for month in self._month_list:
-                leaf.addAmount(month['year'], month['month'],
-                               category.get_turnover(month['begin_ts'], month['end_ts'], self._currency))
+            for period in self._period_list:
+                leaf.addAmount(period['year'], period['number'],
+                               category.get_turnover(period['begin_ts'], period['end_ts'], self._currency))
             self._load_child_amounts(category)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class IncomeSpendingReport(QObject):
     def __init__(self):
         super().__init__()
@@ -345,19 +397,22 @@
         self.actionDetails = QAction(load_icon("list.png"), self.tr("Show operations"), self)
         self.contextMenu.addAction(self.actionDetails)
 
         self.connect_signals_and_slots()
 
         if settings is None:
             begin, end = self.ui.ReportRange.getRange()
-            settings = {'begin_ts': begin, 'end_ts': end, 'currency_id': JalAsset.get_base_currency()}
+            period = self.ui.PeriodComboBox.currentIndex()
+            settings = {'period': period, 'begin_ts': begin, 'end_ts': end, 'currency_id': JalAsset.get_base_currency()}
+        self.ui.PeriodComboBox.setCurrentIndex(settings['period'])
         self.ui.ReportRange.setRange(settings['begin_ts'], settings['end_ts'])
         self.ui.CurrencyCombo.setIndex(settings['currency_id'])
 
     def connect_signals_and_slots(self):
+        self.ui.PeriodComboBox.currentIndexChanged.connect(self.ui.ReportTreeView.model().setPeriod)
         self.ui.ReportRange.changed.connect(self.ui.ReportTreeView.model().setDatesRange)
         self.ui.CurrencyCombo.changed.connect(self.ui.ReportTreeView.model().setCurrency)
         self.ui.ReportTreeView.customContextMenuRequested.connect(self.onCellContextMenu)
         self.actionDetails.triggered.connect(self.showDetailsReport)
         self.ui.SaveButton.pressed.connect(partial(self._parent.save_report, self.name, self.ui.ReportTreeView.model()))
 
     @Slot()
```

### Comparing `jal-2023.4.6/jal/reports/peer.py` & `jal-2023.4.7/jal/reports/peer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/reports/profit_loss.py` & `jal-2023.4.7/jal/reports/profit_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                 money_p = money_0 = values['money']
                 assets_p = assets_0 = values['assets']
             elif i == len(months) - 1:
                 row_name = self.tr("Period end")
                 money_p = money_0
                 assets_p = assets_0
             else:
-                row_name = f"{month['year']} {self.month_name[month['month'] - 1]}"
+                row_name = f"{month['year']} {self.month_name[month['number'] - 1]}"
             try:
                 rel_change = ((values['money'] + values['assets']) - (money_p + assets_p)) / (money_p + assets_p)
             except (ZeroDivisionError, decimal.InvalidOperation):
                 rel_change = Decimal('0')
             data_row = [row_name, values['money'], values['transfers'], values['dividends'], values['interest'],
                         values['fees'], values['taxes'], values['assets'], values['p&l'],
                         values['total'], (values['money'] + values['assets']) - (money_p + assets_p),
```

### Comparing `jal-2023.4.6/jal/reports/reports.py` & `jal-2023.4.7/jal/reports/reports.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/reports/tag.py` & `jal-2023.4.7/jal/reports/tag.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/reports/ui_category_report.py` & `jal-2023.4.7/jal/ui/reports/ui_category_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/reports/ui_deals_report.py` & `jal-2023.4.7/jal/ui/reports/ui_deals_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/reports/ui_holdings_report.py` & `jal-2023.4.7/jal/ui/reports/ui_holdings_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/reports/ui_income_spending_report.py` & `jal-2023.4.7/jal/ui/reports/ui_income_spending_report.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
 from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
     QFont, QFontDatabase, QGradient, QIcon,
     QImage, QKeySequence, QLinearGradient, QPainter,
     QPalette, QPixmap, QRadialGradient, QTransform)
-from PySide6.QtWidgets import (QAbstractItemView, QApplication, QFrame, QHBoxLayout,
-    QHeaderView, QLabel, QPushButton, QSizePolicy,
-    QSpacerItem, QTreeView, QVBoxLayout, QWidget)
+from PySide6.QtWidgets import (QAbstractItemView, QApplication, QComboBox, QFrame,
+    QHBoxLayout, QHeaderView, QLabel, QPushButton,
+    QSizePolicy, QSpacerItem, QTreeView, QVBoxLayout,
+    QWidget)
 
 from jal.widgets.account_select import CurrencyComboBox
 from jal.widgets.custom.date_range_selector import DateRangeSelector
 
 class Ui_IncomeSpendingReportWidget(object):
     def setupUi(self, IncomeSpendingReportWidget):
         if not IncomeSpendingReportWidget.objectName():
@@ -41,14 +42,26 @@
         self.horizontalLayout.setContentsMargins(2, 2, 2, 2)
         self.ReportRange = DateRangeSelector(self.ReportParamsFrame)
         self.ReportRange.setObjectName(u"ReportRange")
         self.ReportRange.setProperty("ItemsList", u"QTD;YTD;this_year;last_year")
 
         self.horizontalLayout.addWidget(self.ReportRange)
 
+        self.PeriodLbl = QLabel(self.ReportParamsFrame)
+        self.PeriodLbl.setObjectName(u"PeriodLbl")
+
+        self.horizontalLayout.addWidget(self.PeriodLbl)
+
+        self.PeriodComboBox = QComboBox(self.ReportParamsFrame)
+        self.PeriodComboBox.addItem("")
+        self.PeriodComboBox.addItem("")
+        self.PeriodComboBox.setObjectName(u"PeriodComboBox")
+
+        self.horizontalLayout.addWidget(self.PeriodComboBox)
+
         self.CurrencyLbl = QLabel(self.ReportParamsFrame)
         self.CurrencyLbl.setObjectName(u"CurrencyLbl")
 
         self.horizontalLayout.addWidget(self.CurrencyLbl)
 
         self.CurrencyCombo = CurrencyComboBox(self.ReportParamsFrame)
         self.CurrencyCombo.setObjectName(u"CurrencyCombo")
@@ -80,11 +93,15 @@
         self.retranslateUi(IncomeSpendingReportWidget)
 
         QMetaObject.connectSlotsByName(IncomeSpendingReportWidget)
     # setupUi
 
     def retranslateUi(self, IncomeSpendingReportWidget):
         IncomeSpendingReportWidget.setWindowTitle(QCoreApplication.translate("IncomeSpendingReportWidget", u"Income & Spending", None))
+        self.PeriodLbl.setText(QCoreApplication.translate("IncomeSpendingReportWidget", u"Periodicity:", None))
+        self.PeriodComboBox.setItemText(0, QCoreApplication.translate("IncomeSpendingReportWidget", u"Monthly", None))
+        self.PeriodComboBox.setItemText(1, QCoreApplication.translate("IncomeSpendingReportWidget", u"Weekly", None))
+
         self.CurrencyLbl.setText(QCoreApplication.translate("IncomeSpendingReportWidget", u"Currency:", None))
         self.SaveButton.setText(QCoreApplication.translate("IncomeSpendingReportWidget", u"Save...", None))
     # retranslateUi
```

### Comparing `jal-2023.4.6/jal/ui/reports/ui_peer_report.py` & `jal-2023.4.7/jal/ui/reports/ui_peer_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/reports/ui_profit_loss_report.py` & `jal-2023.4.7/jal/ui/reports/ui_profit_loss_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/reports/ui_tag_report.py` & `jal-2023.4.7/jal/ui/reports/ui_tag_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/reports/ui_tax_estimation.py` & `jal-2023.4.7/jal/ui/reports/ui_tax_estimation.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/ui_asset_dlg.py` & `jal-2023.4.7/jal/ui/ui_asset_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/ui_flow_export_widget.py` & `jal-2023.4.7/jal/ui/ui_flow_export_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/ui_login_fns_dlg.py` & `jal-2023.4.7/jal/ui/ui_login_fns_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/ui_main_window.py` & `jal-2023.4.7/jal/ui/ui_main_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/ui_operations_widget.py` & `jal-2023.4.7/jal/ui/ui_operations_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/ui_rebuild_window.py` & `jal-2023.4.7/jal/ui/ui_rebuild_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/ui_reference_data_dlg.py` & `jal-2023.4.7/jal/ui/ui_reference_data_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/ui_select_account_dlg.py` & `jal-2023.4.7/jal/ui/ui_select_account_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/ui_select_reference_dlg.py` & `jal-2023.4.7/jal/ui/ui_select_reference_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/ui_slip_import_dlg.py` & `jal-2023.4.7/jal/ui/ui_slip_import_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/ui_tax_export_widget.py` & `jal-2023.4.7/jal/ui/ui_tax_export_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/ui/ui_update_quotes_window.py` & `jal-2023.4.7/jal/ui/ui_update_quotes_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_10.sql` & `jal-2023.4.7/jal/updates/jal_delta_10.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_11.sql` & `jal-2023.4.7/jal/updates/jal_delta_11.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_12.sql` & `jal-2023.4.7/jal/updates/jal_delta_12.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_13.sql` & `jal-2023.4.7/jal/updates/jal_delta_13.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_14.sql` & `jal-2023.4.7/jal/updates/jal_delta_14.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_15.sql` & `jal-2023.4.7/jal/updates/jal_delta_15.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_16.sql` & `jal-2023.4.7/jal/updates/jal_delta_16.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_17.sql` & `jal-2023.4.7/jal/updates/jal_delta_17.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_18.sql` & `jal-2023.4.7/jal/updates/jal_delta_18.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_19.sql` & `jal-2023.4.7/jal/updates/jal_delta_19.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_20.sql` & `jal-2023.4.7/jal/updates/jal_delta_20.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_21.sql` & `jal-2023.4.7/jal/updates/jal_delta_21.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_22.sql` & `jal-2023.4.7/jal/updates/jal_delta_22.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_23.sql` & `jal-2023.4.7/jal/updates/jal_delta_23.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_25.sql` & `jal-2023.4.7/jal/updates/jal_delta_25.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_26.sql` & `jal-2023.4.7/jal/updates/jal_delta_26.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_27.sql` & `jal-2023.4.7/jal/updates/jal_delta_27.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_28.sql` & `jal-2023.4.7/jal/updates/jal_delta_28.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_29.sql` & `jal-2023.4.7/jal/updates/jal_delta_29.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_30.sql` & `jal-2023.4.7/jal/updates/jal_delta_30.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_31.sql` & `jal-2023.4.7/jal/updates/jal_delta_31.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_32.sql` & `jal-2023.4.7/jal/updates/jal_delta_32.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_33.sql` & `jal-2023.4.7/jal/updates/jal_delta_33.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_34.sql` & `jal-2023.4.7/jal/updates/jal_delta_34.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_35.sql` & `jal-2023.4.7/jal/updates/jal_delta_35.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_36.sql` & `jal-2023.4.7/jal/updates/jal_delta_36.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_37.sql` & `jal-2023.4.7/jal/updates/jal_delta_37.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_38.sql` & `jal-2023.4.7/jal/updates/jal_delta_38.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_40.sql` & `jal-2023.4.7/jal/updates/jal_delta_40.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_41.sql` & `jal-2023.4.7/jal/updates/jal_delta_41.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_42.sql` & `jal-2023.4.7/jal/updates/jal_delta_42.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_43.sql` & `jal-2023.4.7/jal/updates/jal_delta_43.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/updates/jal_delta_44.sql` & `jal-2023.4.7/jal/updates/jal_delta_44.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/abstract_operation_details.py` & `jal-2023.4.7/jal/widgets/abstract_operation_details.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/account_select.py` & `jal-2023.4.7/jal/widgets/account_select.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/asset_dialog.py` & `jal-2023.4.7/jal/widgets/asset_dialog.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/corporate_action_widget.py` & `jal-2023.4.7/jal/widgets/corporate_action_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/custom/date_range_selector.py` & `jal-2023.4.7/jal/widgets/custom/date_range_selector.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,31 +33,33 @@
 
         self.range_combo = QComboBox(self)
         self.layout.addWidget(self.range_combo)
 
         self.from_label = QLabel(self.tr("From:"), parent=self)
         self.layout.addWidget(self.from_label)
 
+        button_space = self.height()
         self.from_date = QDateEdit()
         self.from_date.setDisplayFormat("dd/MM/yyyy")
+        self.from_date.setFixedWidth(self.from_date.fontMetrics().horizontalAdvance("00/00/0000") + button_space)
         self.from_date.setCalendarPopup(True)
         self.from_date.setTimeSpec(Qt.UTC)
         self.layout.addWidget(self.from_date)
 
         self.from_label = QLabel(self.tr("To:"), parent=self)
         self.layout.addWidget(self.from_label)
 
         self.to_date = QDateEdit()
         self.to_date.setDisplayFormat("dd/MM/yyyy")
+        self.to_date.setFixedWidth(self.from_date.fontMetrics().horizontalAdvance("00/00/0000") + button_space)
         self.to_date.setCalendarPopup(True)
         self.to_date.setTimeSpec(Qt.UTC)
         self.layout.addWidget(self.to_date)
 
         self.setLayout(self.layout)
-
         self.setFocusProxy(self.range_combo)
 
         self.connect_signals_and_slots()
 
     def getConfig(self):
         return ';'.join(self._items)
```

### Comparing `jal-2023.4.6/jal/widgets/custom/db_lookup_combobox.py` & `jal-2023.4.7/jal/widgets/custom/db_lookup_combobox.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/custom/log_viewer.py` & `jal-2023.4.7/jal/widgets/custom/log_viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import logging
 from jal.constants import CustomColor
+from jal.db.helpers import load_icon
 from PySide6.QtCore import Qt, Slot
 from PySide6.QtWidgets import QApplication, QPlainTextEdit, QLabel, QPushButton
-from PySide6.QtGui import QBrush
+from PySide6.QtGui import QBrush, QAction
 
 
 # Adapter class to have custom log handler that may be passed to logger.addHandler/logger.removeHandler methods and
 # then forward all messages parent view to display them
 class LogHandler(logging.Handler):
     def __init__(self, parent_view):
         self._parent_view = parent_view
@@ -29,14 +30,24 @@
         self.status_bar = None    # Status bar where notifications and control are located
         self.expandButton = None  # Button that shows/hides log window
         self.notification = None  # Here is QLabel element to display LOG update status
         self.clear_color = None   # Variable to store initial "clear" background color
         self.collapsed_text = self.tr("▶ logs")
         self.expanded_text = self.tr("▲ logs")
 
+        self.setContextMenuPolicy(Qt.ActionsContextMenu)
+        self.addAction(load_icon("copy.png"), self.tr('Copy'), self._copy2clipboard)
+        self.addAction(self.tr('Select all'), self.selectAll)
+        self.addAction(load_icon("delete.png"), self.tr('Clear'), self.clear)
+
+    def _copy2clipboard(self):
+        cursor = self.textCursor()
+        text = cursor.selectedText() if cursor.selectedText().toPlainText() else self.toPlainText()
+        QApplication.clipboard().setText(text)
+
     def startLogging(self):
         self._logger = logging.getLogger()
         self._logger.addHandler(self._log_handler)
         log_level = os.environ.get('LOGLEVEL', 'INFO').upper()
         self._logger.setLevel(log_level)
         self._log_handler.setFormatter(logging.Formatter('%(asctime)s - %(levelname)s - %(message)s'))
```

### Comparing `jal-2023.4.6/jal/widgets/delegates.py` & `jal-2023.4.7/jal/widgets/delegates.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/dividend_widget.py` & `jal-2023.4.7/jal/widgets/dividend_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/helpers.py` & `jal-2023.4.7/jal/widgets/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,59 +35,104 @@
             main_window = widget
     if main_window:
         x = main_window.x() + main_window.width() / 2 - window.width() / 2
         y = main_window.y() + main_window.height() / 2 - window.height() / 2
         window.setGeometry(x, y, window.width(), window.height())
 
 # -----------------------------------------------------------------------------------------------------------------------
+# converts string with leading zeros to integer (like '03'->3, '00'->0, ''->0)
+def str2int(value: str) -> int:
+    value = value.lstrip('0')
+    if value:
+        return int(value)
+    else:
+        return 0
+
+# -----------------------------------------------------------------------------------------------------------------------
 # converts given unix-timestamp into string that represents date and time
 def ts2dt(timestamp: int) -> str:
     return datetime.utcfromtimestamp(timestamp).strftime('%d/%m/%Y %H:%M:%S')
 
 # -----------------------------------------------------------------------------------------------------------------------
 # converts given unix-timestamp into string that represents date
 def ts2d(timestamp: int) -> str:
     return datetime.utcfromtimestamp(timestamp).strftime('%d/%m/%Y')
 
 # -----------------------------------------------------------------------------------------------------------------------
+# converts given datetime value into unix-timestamp
+def dt2ts(value: datetime) -> int:
+    return int(value.replace(tzinfo=timezone.utc).timestamp())
+
+# -----------------------------------------------------------------------------------------------------------------------
 # returns unix timestamp for the first second of the month/year
 def month_start_ts(year: int, month: int) -> int:
     start = datetime(year=year, month=month, day=1, hour=0, minute=0, second=0)
-    start = int(start.replace(tzinfo=timezone.utc).timestamp())
-    return start
+    return dt2ts(start)
+
+# returns unix timestamp for the first second of the given week of the month
+def week_start_ts(year: int, week: int) -> int:
+    start = datetime.strptime(f"{year}-W{week}-1", "%Y-W%W-%w")
+    return dt2ts(start)
 
 # -----------------------------------------------------------------------------------------------------------------------
 # returns unix timestamp for the last second of the month/year
 def month_end_ts(year: int, month: int) -> int:
     start = datetime(year=year, month=month, day=1, hour=0, minute=0, second=0)
     if month == 12:
         end = start.replace(year=year + 1, month=1)
     else:
         end = start.replace(month=month + 1)
     end = end - timedelta(seconds=1)
-    end = int(end.replace(tzinfo=timezone.utc).timestamp())
-    return end
+    return dt2ts(end)
+
+# returns unix timestamp for the last second of the given week of the month
+def week_end_ts(year: int, week: int) -> int:
+    end = datetime.strptime(f"{year}-W{week}-1", "%Y-W%W-%w") + timedelta(days=7)
+    return dt2ts(end)
 
 # -----------------------------------------------------------------------------------------------------------------------
 # returns a list of dictionaries for each month between 'begin' and 'end' timestamps (including):
-# { year, month, begin_ts, end_ts }
+# { year, number, begin_ts, end_ts }
+# where number is a month number from 1 to 12
 def month_list(begin: int, end: int) -> list:
     result = []
     year_begin = int(datetime.utcfromtimestamp(begin).strftime('%Y'))
-    month_begin = int(datetime.utcfromtimestamp(begin).strftime('%m').lstrip('0'))
+    month_begin = str2int(datetime.utcfromtimestamp(begin).strftime('%m'))
     year_end = int(datetime.utcfromtimestamp(end).strftime('%Y'))
-    month_end = int(datetime.utcfromtimestamp(end).strftime('%m').lstrip('0'))
+    month_end = str2int(datetime.utcfromtimestamp(end).strftime('%m'))
     for year in range(year_begin, year_end+1):
         month1 = month_begin if year == year_begin else 1
         month2 = month_end + 1 if year == year_end else 13
         for month in range(month1, month2):
-            result.append({'year': year, 'month': month,
+            result.append({'year': year, 'number': month,
                            'begin_ts': month_start_ts(year, month), 'end_ts': month_end_ts(year, month)})
     return result
 
+# returns a list of dictionaries for each week between 'begin' and 'end' timestamps (including):
+# { year, number, begin_ts, end_ts }
+# where number is a week number in year from 1 to 53
+def week_list(begin: int, end: int) -> list:
+    result = []
+    year_begin = int(datetime.utcfromtimestamp(begin).strftime('%Y'))
+    week_begin = str2int(datetime.utcfromtimestamp(begin).strftime('%W'))
+    if week_begin == 0:
+        year_begin -= 1
+        week_begin = 53
+    year_end = int(datetime.utcfromtimestamp(end).strftime('%Y'))
+    week_end = int(datetime.utcfromtimestamp(end).strftime('%W'))
+    if week_end == 0:
+        year_end -= 1
+        week_end = 53
+    for year in range(year_begin, year_end + 1):
+        wk1 = week_begin if year == year_begin else 1
+        wk2 = week_end + 1 if year == year_end else 54
+        for week in range(wk1, wk2):
+            result.append({'year': year, 'number': week,
+                           'begin_ts': week_start_ts(year, week), 'end_ts': week_end_ts(year, week)})
+    return result
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Function takes an image and searches for QR in it. Content of first found QR is returned. Otherwise - empty string.
 def decodeQR(qr_image: QImage) -> str:
     if qr_image.isNull():
         return ''
     if not dependency_present(['pyzbar']):
```

### Comparing `jal-2023.4.6/jal/widgets/income_spending_widget.py` & `jal-2023.4.7/jal/widgets/income_spending_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/main_window.py` & `jal-2023.4.7/jal/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/mdi.py` & `jal-2023.4.7/jal/widgets/mdi.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/operations_tabs.py` & `jal-2023.4.7/jal/widgets/operations_tabs.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/operations_widget.py` & `jal-2023.4.7/jal/widgets/operations_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/price_chart.py` & `jal-2023.4.7/jal/widgets/price_chart.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/qr_scanner.py` & `jal-2023.4.7/jal/widgets/qr_scanner.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/reference_data.py` & `jal-2023.4.7/jal/widgets/reference_data.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/reference_dialogs.py` & `jal-2023.4.7/jal/widgets/reference_dialogs.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/reference_selector.py` & `jal-2023.4.7/jal/widgets/reference_selector.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/register_designer_plugins.py` & `jal-2023.4.7/jal/widgets/register_designer_plugins.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/selection_dialog.py` & `jal-2023.4.7/jal/widgets/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/tax_widget.py` & `jal-2023.4.7/jal/widgets/tax_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/trade_widget.py` & `jal-2023.4.7/jal/widgets/trade_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal/widgets/transfer_widget.py` & `jal-2023.4.7/jal/widgets/transfer_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/jal.egg-info/PKG-INFO` & `jal-2023.4.7/jal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jal
-Version: 2023.4.6
+Version: 2023.4.7
 Summary: Just Another Ledger - project to track personal financial records
 Home-page: https://github.com/titov-vv/jal
 Author-email: jal@gmx.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `jal-2023.4.6/jal.egg-info/SOURCES.txt` & `jal-2023.4.7/jal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jal-2023.4.6/setup.py` & `jal-2023.4.7/setup.py`

 * *Files identical despite different names*

