# Comparing `tmp/budy-0.7.8.tar.gz` & `tmp/budy-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/budy-0.7.8.tar", last modified: Mon Mar 20 21:40:49 2023, max compression
+gzip compressed data, was "dist/budy-0.7.9.tar", last modified: Mon Mar 20 21:50:20 2023, max compression
```

## Comparing `budy-0.7.8.tar` & `budy-0.7.9.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy/models/
--rw-r--r--   0 root         (0) root         (0)     1304 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/brand.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/country.py
--rw-r--r--   0 root         (0) root         (0)     2220 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/store.py
--rw-r--r--   0 root         (0) root         (0)    14054 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/voucher.py
--rw-r--r--   0 root         (0) root         (0)     2314 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/order_line.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/season.py
--rw-r--r--   0 root         (0) root         (0)     5892 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/bag.py
--rw-r--r--   0 root         (0) root         (0)     1304 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/color.py
--rw-r--r--   0 root         (0) root         (0)     2815 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8248 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/media.py
--rw-r--r--   0 root         (0) root         (0)     2067 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/composition.py
--rw-r--r--   0 root         (0) root         (0)     2425 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/referral.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/live_model.py
--rw-r--r--   0 root         (0) root         (0)    10167 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/bundle_line.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/category.py
--rw-r--r--   0 root         (0) root         (0)     8566 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/account.py
--rw-r--r--   0 root         (0) root         (0)     4880 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/base.py
--rw-r--r--   0 root         (0) root         (0)    39035 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/product.py
--rw-r--r--   0 root         (0) root         (0)     4679 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/section.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     3207 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/address.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/collection.py
--rw-r--r--   0 root         (0) root         (0)     6046 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/group.py
--rw-r--r--   0 root         (0) root         (0)    13815 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/measurement.py
--rw-r--r--   0 root         (0) root         (0)    17323 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/bundle.py
--rw-r--r--   0 root         (0) root         (0)     4190 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/wishlist.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/wishlist_line.py
--rw-r--r--   0 root         (0) root         (0)    69370 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/order.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/bag_line.py
--rw-r--r--   0 root         (0) root         (0)     4290 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/currency.py
--rw-r--r--   0 root         (0) root         (0)     4115 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/models/exchange_rate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy/controllers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy/controllers/api/
--rw-r--r--   0 root         (0) root         (0)     1988 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/brand.py
--rw-r--r--   0 root         (0) root         (0)     2508 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/country.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/voucher.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/root.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/season.py
--rw-r--r--   0 root         (0) root         (0)     4428 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/bag.py
--rw-r--r--   0 root         (0) root         (0)     1988 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/color.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3427 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/media.py
--rw-r--r--   0 root         (0) root         (0)     1583 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/referral.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/category.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/easypay.py
--rw-r--r--   0 root         (0) root         (0)     5873 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/account.py
--rw-r--r--   0 root         (0) root         (0)     1808 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/base.py
--rw-r--r--   0 root         (0) root         (0)     6299 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/product.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/section.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/subscription.py
--rw-r--r--   0 root         (0) root         (0)     2544 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/address.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/collection.py
--rw-r--r--   0 root         (0) root         (0)    18739 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/order.py
--rw-r--r--   0 root         (0) root         (0)     2382 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/seeplus.py
--rw-r--r--   0 root         (0) root         (0)     2315 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/api/currency.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy/controllers/web/
--rw-r--r--   0 root         (0) root         (0)     1606 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/web/admin.py
--rw-r--r--   0 root         (0) root         (0)     1387 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/web/_stripe.py
--rw-r--r--   0 root         (0) root         (0)     2734 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/web/base.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/controllers/web/order.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3069 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy/test/
--rw-r--r--   0 root         (0) root         (0)    14883 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/test/voucher.py
--rw-r--r--   0 root         (0) root         (0)    12257 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/test/bag.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/test/referral.py
--rw-r--r--   0 root         (0) root         (0)     2805 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/test/account.py
--rw-r--r--   0 root         (0) root         (0)     9252 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/test/product.py
--rw-r--r--   0 root         (0) root         (0)     5692 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/test/measurement.py
--rw-r--r--   0 root         (0) root         (0)     3536 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/test/wishlist.py
--rw-r--r--   0 root         (0) root         (0)    37405 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/test/order.py
--rw-r--r--   0 root         (0) root         (0)     3647 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/test/currency.py
--rw-r--r--   0 root         (0) root         (0)     2238 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/test/exchange_rate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy/templates/
--rw-r--r--   0 root         (0) root         (0)     1112 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/templates/signin.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy/templates/partials/
--rw-r--r--   0 root         (0) root         (0)      452 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/templates/partials/base.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1063 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/templates/partials/internal.html.tpl
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/templates/partials/external.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy/templates/order/
--rw-r--r--   0 root         (0) root         (0)      876 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/templates/order/me.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy/static/js/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 21:40:33.000000 budy-0.7.8/src/budy/static/js/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 21:40:40.000000 budy-0.7.8/src/budy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     2624 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    12361 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       32 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-03-20 21:40:49.000000 budy-0.7.8/src/budy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    10669 2023-03-20 21:40:33.000000 budy-0.7.8/README.md
--rw-r--r--   0 root         (0) root         (0)    12361 2023-03-20 21:40:49.000000 budy-0.7.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3127 2023-03-20 21:40:33.000000 budy-0.7.8/setup.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-03-20 21:40:49.000000 budy-0.7.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/models/
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/brand.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/country.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/store.py
+-rw-r--r--   0 root         (0) root         (0)    14054 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/voucher.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/order_line.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/season.py
+-rw-r--r--   0 root         (0) root         (0)     5892 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/bag.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/color.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8248 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/media.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/composition.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/referral.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/live_model.py
+-rw-r--r--   0 root         (0) root         (0)    10167 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/bundle_line.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/category.py
+-rw-r--r--   0 root         (0) root         (0)     8566 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/account.py
+-rw-r--r--   0 root         (0) root         (0)     4880 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/base.py
+-rw-r--r--   0 root         (0) root         (0)    39035 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/product.py
+-rw-r--r--   0 root         (0) root         (0)     4679 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/section.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     3207 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/address.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/collection.py
+-rw-r--r--   0 root         (0) root         (0)     6046 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/group.py
+-rw-r--r--   0 root         (0) root         (0)    13815 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/measurement.py
+-rw-r--r--   0 root         (0) root         (0)    17323 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/bundle.py
+-rw-r--r--   0 root         (0) root         (0)     4190 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/wishlist.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/wishlist_line.py
+-rw-r--r--   0 root         (0) root         (0)    69370 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/order.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/bag_line.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/currency.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/exchange_rate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/controllers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/controllers/api/
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/brand.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/country.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/voucher.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/root.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/season.py
+-rw-r--r--   0 root         (0) root         (0)     4428 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/bag.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/color.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/media.py
+-rw-r--r--   0 root         (0) root         (0)     1583 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/referral.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/category.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/easypay.py
+-rw-r--r--   0 root         (0) root         (0)     5873 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/account.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/base.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/product.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/section.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/address.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/collection.py
+-rw-r--r--   0 root         (0) root         (0)    18739 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/order.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/seeplus.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/currency.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/controllers/web/
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/web/admin.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/web/_stripe.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/web/base.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/web/order.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/test/
+-rw-r--r--   0 root         (0) root         (0)    14883 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/voucher.py
+-rw-r--r--   0 root         (0) root         (0)    12257 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/bag.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/referral.py
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/account.py
+-rw-r--r--   0 root         (0) root         (0)     9252 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/product.py
+-rw-r--r--   0 root         (0) root         (0)     5692 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/measurement.py
+-rw-r--r--   0 root         (0) root         (0)     3536 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/wishlist.py
+-rw-r--r--   0 root         (0) root         (0)    37405 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/order.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/currency.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/exchange_rate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/templates/
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/templates/signin.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/templates/partials/
+-rw-r--r--   0 root         (0) root         (0)      452 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/templates/partials/base.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/templates/partials/internal.html.tpl
+-rw-r--r--   0 root         (0) root         (0)       40 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/templates/partials/external.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/templates/order/
+-rw-r--r--   0 root         (0) root         (0)      876 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/templates/order/me.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/static/js/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/static/js/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 21:50:10.000000 budy-0.7.9/src/budy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    12361 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       32 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    10669 2023-03-20 21:50:04.000000 budy-0.7.9/README.md
+-rw-r--r--   0 root         (0) root         (0)    12361 2023-03-20 21:50:20.000000 budy-0.7.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-03-20 21:50:04.000000 budy-0.7.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-03-20 21:50:20.000000 budy-0.7.9/setup.cfg
```

### Comparing `budy-0.7.8/src/budy/models/brand.py` & `budy-0.7.9/src/budy/models/brand.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/country.py` & `budy-0.7.9/src/budy/models/country.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/store.py` & `budy-0.7.9/src/budy/models/store.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/voucher.py` & `budy-0.7.9/src/budy/models/voucher.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/order_line.py` & `budy-0.7.9/src/budy/models/order_line.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/season.py` & `budy-0.7.9/src/budy/models/season.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/bag.py` & `budy-0.7.9/src/budy/models/bag.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/color.py` & `budy-0.7.9/src/budy/models/color.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/__init__.py` & `budy-0.7.9/src/budy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/media.py` & `budy-0.7.9/src/budy/models/media.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/composition.py` & `budy-0.7.9/src/budy/models/composition.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/referral.py` & `budy-0.7.9/src/budy/models/referral.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/live_model.py` & `budy-0.7.9/src/budy/models/live_model.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/bundle_line.py` & `budy-0.7.9/src/budy/models/bundle_line.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/category.py` & `budy-0.7.9/src/budy/models/category.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/account.py` & `budy-0.7.9/src/budy/models/account.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/base.py` & `budy-0.7.9/src/budy/models/base.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/product.py` & `budy-0.7.9/src/budy/models/product.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/section.py` & `budy-0.7.9/src/budy/models/section.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/subscription.py` & `budy-0.7.9/src/budy/models/subscription.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/address.py` & `budy-0.7.9/src/budy/models/address.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/collection.py` & `budy-0.7.9/src/budy/models/collection.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/group.py` & `budy-0.7.9/src/budy/models/group.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/measurement.py` & `budy-0.7.9/src/budy/models/measurement.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/bundle.py` & `budy-0.7.9/src/budy/models/bundle.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/wishlist.py` & `budy-0.7.9/src/budy/models/wishlist.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/wishlist_line.py` & `budy-0.7.9/src/budy/models/wishlist_line.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/order.py` & `budy-0.7.9/src/budy/models/order.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/bag_line.py` & `budy-0.7.9/src/budy/models/bag_line.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/currency.py` & `budy-0.7.9/src/budy/models/currency.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/models/exchange_rate.py` & `budy-0.7.9/src/budy/models/exchange_rate.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/brand.py` & `budy-0.7.9/src/budy/controllers/api/brand.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/country.py` & `budy-0.7.9/src/budy/controllers/api/country.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/voucher.py` & `budy-0.7.9/src/budy/controllers/api/voucher.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/root.py` & `budy-0.7.9/src/budy/controllers/api/root.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/season.py` & `budy-0.7.9/src/budy/controllers/api/season.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/bag.py` & `budy-0.7.9/src/budy/controllers/api/bag.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/color.py` & `budy-0.7.9/src/budy/controllers/api/color.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/__init__.py` & `budy-0.7.9/src/budy/controllers/api/__init__.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/media.py` & `budy-0.7.9/src/budy/controllers/api/media.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/referral.py` & `budy-0.7.9/src/budy/controllers/api/referral.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/category.py` & `budy-0.7.9/src/budy/controllers/api/category.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/easypay.py` & `budy-0.7.9/src/budy/controllers/api/easypay.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/account.py` & `budy-0.7.9/src/budy/controllers/api/account.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/base.py` & `budy-0.7.9/src/budy/controllers/api/base.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/product.py` & `budy-0.7.9/src/budy/controllers/api/product.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/section.py` & `budy-0.7.9/src/budy/controllers/api/section.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/subscription.py` & `budy-0.7.9/src/budy/controllers/api/subscription.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/address.py` & `budy-0.7.9/src/budy/controllers/api/address.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/collection.py` & `budy-0.7.9/src/budy/controllers/api/collection.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/order.py` & `budy-0.7.9/src/budy/controllers/api/order.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/api/seeplus.py` & `budy-0.7.9/src/budy/controllers/api/seeplus.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 class SeeplusAPIController(root.RootAPIController):
 
     @appier.route("/api/seeplus/update", "POST", json = True)
     def update(self):
         key = self.request.get_header("X-Seeplus-Key", None)
         _key = appier.conf("SEEPLUS_KEY", None)
-        if _key and _key == key:
+        if _key and not _key == key:
             raise appier.SecurityError(
                 message = "Mismatch in Seeplus key",
                 code = 401 
             )
         object = appier.get_object()
         event = object.get("event", "OrderManagement.StatusChanged")
         data = object.get("data", {})
@@ -65,12 +65,16 @@
             result = "Handled"
         return dict(result = result)
 
     def _status_change_s(self, data):
         reference = data["code"]
         status = data["status"]
         order = budy.Order.get(reference = reference)
+        seeplus_timestamp = order.meta.get("seeplus_timestamp", None)
+        if not seeplus_timestamp: raise appier.OperationalError(
+            message = "Order not imported in Seeplus"
+        )
         order.meta.update(
             seeplus_status = status,
             seeplus_update = time.time()
         )
         order.save()
```

### Comparing `budy-0.7.8/src/budy/controllers/api/currency.py` & `budy-0.7.9/src/budy/controllers/api/currency.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/__init__.py` & `budy-0.7.9/src/budy/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/web/admin.py` & `budy-0.7.9/src/budy/controllers/web/admin.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/web/__init__.py` & `budy-0.7.9/src/budy/controllers/web/__init__.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/web/_stripe.py` & `budy-0.7.9/src/budy/controllers/web/_stripe.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/web/base.py` & `budy-0.7.9/src/budy/controllers/web/base.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/controllers/web/order.py` & `budy-0.7.9/src/budy/controllers/web/order.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/__init__.py` & `budy-0.7.9/src/budy/__init__.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/main.py` & `budy-0.7.9/src/budy/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     def get_seeplus_api(self):
         import seeplus
         if self.seeplus_api: return self.seeplus_api
         self.seeplus_api = seeplus.API()
         return self.seeplus_api
 
     def _version(self):
-        return "0.7.8"
+        return "0.7.9"
 
     def _description(self):
         return "Budy"
 
     def _observations(self):
         return "Simple and easy to use E-commerce engine"
```

### Comparing `budy-0.7.8/src/budy/test/voucher.py` & `budy-0.7.9/src/budy/test/voucher.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/test/bag.py` & `budy-0.7.9/src/budy/test/bag.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/test/__init__.py` & `budy-0.7.9/src/budy/test/__init__.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/test/referral.py` & `budy-0.7.9/src/budy/test/referral.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/test/account.py` & `budy-0.7.9/src/budy/test/account.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/test/product.py` & `budy-0.7.9/src/budy/test/product.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/test/measurement.py` & `budy-0.7.9/src/budy/test/measurement.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/test/wishlist.py` & `budy-0.7.9/src/budy/test/wishlist.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/test/order.py` & `budy-0.7.9/src/budy/test/order.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/test/currency.py` & `budy-0.7.9/src/budy/test/currency.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/test/exchange_rate.py` & `budy-0.7.9/src/budy/test/exchange_rate.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/templates/signin.html.tpl` & `budy-0.7.9/src/budy/templates/signin.html.tpl`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/templates/partials/internal.html.tpl` & `budy-0.7.9/src/budy/templates/partials/internal.html.tpl`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy/templates/order/me.html.tpl` & `budy-0.7.9/src/budy/templates/order/me.html.tpl`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy.egg-info/SOURCES.txt` & `budy-0.7.9/src/budy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/src/budy.egg-info/PKG-INFO` & `budy-0.7.9/src/budy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budy
-Version: 0.7.8
+Version: 0.7.9
 Summary: Budy E-commerce System
 Home-page: http://budy.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Budy](http://budy.hive.pt)
```

### Comparing `budy-0.7.8/README.md` & `budy-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `budy-0.7.8/PKG-INFO` & `budy-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budy
-Version: 0.7.8
+Version: 0.7.9
 Summary: Budy E-commerce System
 Home-page: http://budy.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Budy](http://budy.hive.pt)
```

### Comparing `budy-0.7.8/setup.py` & `budy-0.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
     name = "budy",
-    version = "0.7.8",
+    version = "0.7.9",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "Budy E-commerce System",
     license = "Apache License, Version 2.0",
     keywords = "budy e-commerce engine web json",
     url = "http://budy.hive.pt",
     zip_safe = False,
```

