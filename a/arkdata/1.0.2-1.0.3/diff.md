# Comparing `tmp/arkdata-1.0.2.tar.gz` & `tmp/arkdata-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkdata-1.0.2.tar", last modified: Sun Apr 16 02:15:01 2023, max compression
+gzip compressed data, was "arkdata-1.0.3.tar", last modified: Fri Apr 21 04:07:13 2023, max compression
```

## Comparing `arkdata-1.0.2.tar` & `arkdata-1.0.3.tar`

### file list

```diff
@@ -1,74 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.554152 arkdata-1.0.2/
--rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:13.000000 arkdata-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      650 2023-04-16 02:15:01.555154 arkdata-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-03-25 16:35:13.000000 arkdata-1.0.2/README.md
--rw-rw-rw-   0        0        0      642 2023-04-16 02:13:53.000000 arkdata-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1223 2023-04-16 02:15:01.556153 arkdata-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.495014 arkdata-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.501219 arkdata-1.0.2/src/arkdata/
--rw-rw-rw-   0        0        0       54 2023-04-02 01:40:29.000000 arkdata-1.0.2/src/arkdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.510218 arkdata-1.0.2/src/arkdata/database/
--rw-rw-rw-   0        0        0      242 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/database/__init__.py
--rw-rw-rw-   0        0        0      860 2023-03-27 03:33:59.000000 arkdata-1.0.2/src/arkdata/database/configuration.py
--rw-rw-rw-   0        0        0     3371 2023-04-11 01:32:04.000000 arkdata-1.0.2/src/arkdata/database/cursor.py
--rw-rw-rw-   0        0        0     1470 2023-03-30 01:55:50.000000 arkdata-1.0.2/src/arkdata/database/database.py
--rw-rw-rw-   0        0        0     5190 2023-04-11 02:28:44.000000 arkdata-1.0.2/src/arkdata/database/table.py
--rw-rw-rw-   0        0        0        0 2023-03-27 03:33:59.000000 arkdata-1.0.2/src/arkdata/main.py
-drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.533156 arkdata-1.0.2/src/arkdata/models/
--rw-rw-rw-   0        0        0     2114 2023-04-04 00:26:27.000000 arkdata-1.0.2/src/arkdata/models/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-07 19:27:12.000000 arkdata-1.0.2/src/arkdata/models/account.py
--rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/ammunition.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/armour.py
--rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/artifact.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/attachment.py
--rw-rw-rw-   0        0        0     1397 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/cart_item.py
--rw-rw-rw-   0        0        0     1698 2023-04-12 17:31:52.000000 arkdata-1.0.2/src/arkdata/models/command.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/consumable.py
--rw-rw-rw-   0        0        0     1808 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/creature.py
--rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/dye.py
--rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/egg.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/farm.py
--rw-rw-rw-   0        0        0     1416 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/order_item.py
--rw-rw-rw-   0        0        0     2782 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/product.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/recipe.py
--rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/resource.py
--rw-rw-rw-   0        0        0     1629 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/saddle.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/seed.py
--rw-rw-rw-   0        0        0      810 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/server.py
--rw-rw-rw-   0        0        0     1757 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/sessions.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/skin.py
--rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/structure.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/tool.py
--rw-rw-rw-   0        0        0     1289 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/trophy.py
--rw-rw-rw-   0        0        0     1581 2023-04-11 01:12:51.000000 arkdata-1.0.2/src/arkdata/models/user.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/weapon.py
-drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.554152 arkdata-1.0.2/src/arkdata/seeds/
--rw-rw-rw-   0        0        0        0 2023-03-30 03:59:09.000000 arkdata-1.0.2/src/arkdata/seeds/__init__.py
--rw-rw-rw-   0        0        0     2041 2023-04-07 19:25:52.000000 arkdata-1.0.2/src/arkdata/seeds/accounts.json
--rw-rw-rw-   0        0        0    16119 2023-03-30 06:36:40.000000 arkdata-1.0.2/src/arkdata/seeds/ammunitions.json
--rw-rw-rw-   0        0        0    36003 2023-03-30 03:50:59.000000 arkdata-1.0.2/src/arkdata/seeds/armours.json
--rw-rw-rw-   0        0        0    32929 2023-03-30 03:50:56.000000 arkdata-1.0.2/src/arkdata/seeds/artifacts.json
--rw-rw-rw-   0        0        0     3081 2023-03-30 03:50:48.000000 arkdata-1.0.2/src/arkdata/seeds/attachments.json
--rw-rw-rw-   0        0        0      651 2023-03-30 03:50:40.000000 arkdata-1.0.2/src/arkdata/seeds/commands.json
--rw-rw-rw-   0        0        0   100583 2023-03-30 03:50:36.000000 arkdata-1.0.2/src/arkdata/seeds/consumables.json
--rw-rw-rw-   0        0        0   589770 2023-03-30 03:50:20.000000 arkdata-1.0.2/src/arkdata/seeds/creatures.json
--rw-rw-rw-   0        0        0    11428 2023-03-30 03:50:14.000000 arkdata-1.0.2/src/arkdata/seeds/dyes.json
--rw-rw-rw-   0        0        0    57046 2023-03-30 03:50:12.000000 arkdata-1.0.2/src/arkdata/seeds/eggs.json
--rw-rw-rw-   0        0        0     3588 2023-03-30 03:50:09.000000 arkdata-1.0.2/src/arkdata/seeds/farms.json
--rw-rw-rw-   0        0        0   225349 2023-03-30 06:03:15.000000 arkdata-1.0.2/src/arkdata/seeds/products.json
--rw-rw-rw-   0        0        0     8457 2023-03-30 03:50:01.000000 arkdata-1.0.2/src/arkdata/seeds/recipes.json
--rw-rw-rw-   0        0        0    52865 2023-03-30 03:49:55.000000 arkdata-1.0.2/src/arkdata/seeds/resources.json
--rw-rw-rw-   0        0        0    57917 2023-03-30 07:19:16.000000 arkdata-1.0.2/src/arkdata/seeds/saddles.json
--rw-rw-rw-   0        0        0    16789 2023-03-30 03:47:57.000000 arkdata-1.0.2/src/arkdata/seeds/seeds.json
--rw-rw-rw-   0        0        0   180774 2023-03-30 03:44:21.000000 arkdata-1.0.2/src/arkdata/seeds/skins.json
--rw-rw-rw-   0        0        0   185254 2023-03-30 03:44:16.000000 arkdata-1.0.2/src/arkdata/seeds/structures.json
--rw-rw-rw-   0        0        0    12933 2023-03-30 03:44:10.000000 arkdata-1.0.2/src/arkdata/seeds/tools.json
--rw-rw-rw-   0        0        0    23142 2023-03-30 03:44:02.000000 arkdata-1.0.2/src/arkdata/seeds/trophies.json
--rw-rw-rw-   0        0        0     1251 2023-03-30 04:20:15.000000 arkdata-1.0.2/src/arkdata/seeds/users.json
--rw-rw-rw-   0        0        0    29591 2023-03-30 03:43:50.000000 arkdata-1.0.2/src/arkdata/seeds/weapons.json
-drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.506217 arkdata-1.0.2/src/arkdata.egg-info/
--rw-rw-rw-   0        0        0      650 2023-04-16 02:15:01.000000 arkdata-1.0.2/src/arkdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1948 2023-04-16 02:15:01.000000 arkdata-1.0.2/src/arkdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 02:15:01.000000 arkdata-1.0.2/src/arkdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      167 2023-04-16 02:15:01.000000 arkdata-1.0.2/src/arkdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 02:15:01.000000 arkdata-1.0.2/src/arkdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 04:07:13.008636 arkdata-1.0.3/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:13.000000 arkdata-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      650 2023-04-21 04:07:13.009636 arkdata-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-03-25 16:35:13.000000 arkdata-1.0.3/README.md
+-rw-rw-rw-   0        0        0      642 2023-04-16 02:13:53.000000 arkdata-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1223 2023-04-21 04:07:13.010636 arkdata-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 04:07:12.948580 arkdata-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 04:07:12.954580 arkdata-1.0.3/src/arkdata/
+-rw-rw-rw-   0        0        0       54 2023-04-02 01:40:29.000000 arkdata-1.0.3/src/arkdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:07:12.964127 arkdata-1.0.3/src/arkdata/database/
+-rw-rw-rw-   0        0        0      242 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/database/__init__.py
+-rw-rw-rw-   0        0        0      860 2023-03-27 03:33:59.000000 arkdata-1.0.3/src/arkdata/database/configuration.py
+-rw-rw-rw-   0        0        0     3371 2023-04-11 01:32:04.000000 arkdata-1.0.3/src/arkdata/database/cursor.py
+-rw-rw-rw-   0        0        0     1470 2023-03-30 01:55:50.000000 arkdata-1.0.3/src/arkdata/database/database.py
+-rw-rw-rw-   0        0        0     5948 2023-04-21 03:49:32.000000 arkdata-1.0.3/src/arkdata/database/table.py
+-rw-rw-rw-   0        0        0        0 2023-03-27 03:33:59.000000 arkdata-1.0.3/src/arkdata/main.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:07:12.985636 arkdata-1.0.3/src/arkdata/models/
+-rw-rw-rw-   0        0        0     2175 2023-04-21 00:38:08.000000 arkdata-1.0.3/src/arkdata/models/__init__.py
+-rw-rw-rw-   0        0        0      961 2023-04-19 02:45:08.000000 arkdata-1.0.3/src/arkdata/models/account.py
+-rw-rw-rw-   0        0        0     3556 2023-04-21 02:09:27.000000 arkdata-1.0.3/src/arkdata/models/admin.py
+-rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/ammunition.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/armour.py
+-rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/artifact.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/attachment.py
+-rw-rw-rw-   0        0        0     1397 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/cart_item.py
+-rw-rw-rw-   0        0        0     1684 2023-04-21 02:46:11.000000 arkdata-1.0.3/src/arkdata/models/command.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/consumable.py
+-rw-rw-rw-   0        0        0     1808 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/creature.py
+-rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/dye.py
+-rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/egg.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/farm.py
+-rw-rw-rw-   0        0        0     1416 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/order_item.py
+-rw-rw-rw-   0        0        0     2782 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/product.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/recipe.py
+-rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/resource.py
+-rw-rw-rw-   0        0        0     1629 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/saddle.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/seed.py
+-rw-rw-rw-   0        0        0      668 2023-04-20 02:17:11.000000 arkdata-1.0.3/src/arkdata/models/server.py
+-rw-rw-rw-   0        0        0     1652 2023-04-19 03:24:44.000000 arkdata-1.0.3/src/arkdata/models/sessions.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/skin.py
+-rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/structure.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/tool.py
+-rw-rw-rw-   0        0        0     1289 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/trophy.py
+-rw-rw-rw-   0        0        0     2735 2023-04-21 01:56:51.000000 arkdata-1.0.3/src/arkdata/models/user.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/weapon.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:07:13.008636 arkdata-1.0.3/src/arkdata/seeds/
+-rw-rw-rw-   0        0        0        0 2023-03-30 03:59:09.000000 arkdata-1.0.3/src/arkdata/seeds/__init__.py
+-rw-rw-rw-   0        0        0      393 2023-04-16 22:10:50.000000 arkdata-1.0.3/src/arkdata/seeds/accounts.json
+-rw-rw-rw-   0        0        0      103 2023-04-21 01:36:05.000000 arkdata-1.0.3/src/arkdata/seeds/admins.json
+-rw-rw-rw-   0        0        0    16119 2023-03-30 06:36:40.000000 arkdata-1.0.3/src/arkdata/seeds/ammunitions.json
+-rw-rw-rw-   0        0        0    36003 2023-03-30 03:50:59.000000 arkdata-1.0.3/src/arkdata/seeds/armours.json
+-rw-rw-rw-   0        0        0    32929 2023-03-30 03:50:56.000000 arkdata-1.0.3/src/arkdata/seeds/artifacts.json
+-rw-rw-rw-   0        0        0     3081 2023-03-30 03:50:48.000000 arkdata-1.0.3/src/arkdata/seeds/attachments.json
+-rw-rw-rw-   0        0        0      567 2023-04-21 02:51:27.000000 arkdata-1.0.3/src/arkdata/seeds/commands.json
+-rw-rw-rw-   0        0        0   100583 2023-03-30 03:50:36.000000 arkdata-1.0.3/src/arkdata/seeds/consumables.json
+-rw-rw-rw-   0        0        0   589770 2023-03-30 03:50:20.000000 arkdata-1.0.3/src/arkdata/seeds/creatures.json
+-rw-rw-rw-   0        0        0    11428 2023-03-30 03:50:14.000000 arkdata-1.0.3/src/arkdata/seeds/dyes.json
+-rw-rw-rw-   0        0        0    57046 2023-03-30 03:50:12.000000 arkdata-1.0.3/src/arkdata/seeds/eggs.json
+-rw-rw-rw-   0        0        0     3588 2023-03-30 03:50:09.000000 arkdata-1.0.3/src/arkdata/seeds/farms.json
+-rw-rw-rw-   0        0        0   225349 2023-03-30 06:03:15.000000 arkdata-1.0.3/src/arkdata/seeds/products.json
+-rw-rw-rw-   0        0        0     8457 2023-03-30 03:50:01.000000 arkdata-1.0.3/src/arkdata/seeds/recipes.json
+-rw-rw-rw-   0        0        0    52865 2023-03-30 03:49:55.000000 arkdata-1.0.3/src/arkdata/seeds/resources.json
+-rw-rw-rw-   0        0        0    57917 2023-03-30 07:19:16.000000 arkdata-1.0.3/src/arkdata/seeds/saddles.json
+-rw-rw-rw-   0        0        0    16789 2023-03-30 03:47:57.000000 arkdata-1.0.3/src/arkdata/seeds/seeds.json
+-rw-rw-rw-   0        0        0      494 2023-04-16 22:10:50.000000 arkdata-1.0.3/src/arkdata/seeds/sessions.json
+-rw-rw-rw-   0        0        0   180774 2023-03-30 03:44:21.000000 arkdata-1.0.3/src/arkdata/seeds/skins.json
+-rw-rw-rw-   0        0        0   185254 2023-03-30 03:44:16.000000 arkdata-1.0.3/src/arkdata/seeds/structures.json
+-rw-rw-rw-   0        0        0    12933 2023-03-30 03:44:10.000000 arkdata-1.0.3/src/arkdata/seeds/tools.json
+-rw-rw-rw-   0        0        0    23142 2023-03-30 03:44:02.000000 arkdata-1.0.3/src/arkdata/seeds/trophies.json
+-rw-rw-rw-   0        0        0      292 2023-04-16 22:10:50.000000 arkdata-1.0.3/src/arkdata/seeds/users.json
+-rw-rw-rw-   0        0        0    29591 2023-03-30 03:43:50.000000 arkdata-1.0.3/src/arkdata/seeds/weapons.json
+drwxrwxrwx   0        0        0        0 2023-04-21 04:07:12.958582 arkdata-1.0.3/src/arkdata.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-04-21 04:07:12.000000 arkdata-1.0.3/src/arkdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2038 2023-04-21 04:07:12.000000 arkdata-1.0.3/src/arkdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 04:07:12.000000 arkdata-1.0.3/src/arkdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2023-04-21 04:07:12.000000 arkdata-1.0.3/src/arkdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 04:07:12.000000 arkdata-1.0.3/src/arkdata.egg-info/top_level.txt
```

### Comparing `arkdata-1.0.2/LICENSE` & `arkdata-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/PKG-INFO` & `arkdata-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdata
-Version: 1.0.2
+Version: 1.0.3
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Data
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Data/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdata-1.0.2/pyproject.toml` & `arkdata-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/setup.cfg` & `arkdata-1.0.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6461 7461 0d0a 7665 7273   = arkdata..vers
-00000020: 696f 6e20 3d20 312e 302e 320d 0a74 6573  ion = 1.0.2..tes
+00000020: 696f 6e20 3d20 312e 302e 330d 0a74 6573  ion = 1.0.3..tes
 00000030: 745f 7665 7273 696f 6e20 3d20 312e 302e  t_version = 1.0.
-00000040: 320d 0a70 726f 6475 6374 696f 6e5f 7665  2..production_ve
-00000050: 7273 696f 6e20 3d20 312e 302e 320d 0a61  rsion = 1.0.2..a
+00000040: 340d 0a70 726f 6475 6374 696f 6e5f 7665  4..production_ve
+00000050: 7273 696f 6e20 3d20 312e 302e 330d 0a61  rsion = 1.0.3..a
 00000060: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
 00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000080: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
 00000090: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 000000b0: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
 000000c0: 6363 6573 7365 7320 7468 6520 4172 6b20  ccesses the Ark
```

### Comparing `arkdata-1.0.2/src/arkdata/database/configuration.py` & `arkdata-1.0.3/src/arkdata/database/configuration.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/database/cursor.py` & `arkdata-1.0.3/src/arkdata/database/cursor.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/database/database.py` & `arkdata-1.0.3/src/arkdata/database/database.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/database/table.py` & `arkdata-1.0.3/src/arkdata/database/table.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,100 +5,116 @@
 from pathlib import Path
 
 
 class Table:
     id = Column(Integer, primary_key=True, autoincrement=True)
 
     @classmethod
-    def all(cls):
+    def all(cls) -> list:
         with sqlalchemy.app_context():
             return sqlalchemy.db.session.query(cls).all()
 
     @classmethod
     def find_by(cls, **kwargs):
         args = [cls.__dict__[param] == arg for param, arg in kwargs.items()]
         with sqlalchemy.app_context():
             return sqlalchemy.db.session.query(cls).filter(*args).first()
 
     @classmethod
-    def find_all_by(cls, **kwargs):
+    def find_all_by(cls, **kwargs) -> list:
         args = [cls.__dict__[param] == arg for param, arg in kwargs.items()]
         with sqlalchemy.app_context():
             record = sqlalchemy.db.session.query(cls).filter(*args).all()
             return record
 
     @classmethod
-    def columns(cls):
+    def columns(cls) -> list:
         return cls.metadata.tables[cls.__tablename__].columns.keys()
 
     @classmethod
     def first(cls):
         with sqlalchemy.app_context():
             return sqlalchemy.db.session.query(cls).first()
 
     @classmethod
-    def length(cls):
+    def length(cls) -> int:
         with sqlalchemy.app_context():
             return sqlalchemy.db.session.query(cls).count()
 
     @classmethod
-    def bulk_insert(cls, values: list):
+    def bulk_insert(cls, values: list) -> list:
         with sqlalchemy.app_context():
             items = []
             for kwargs in values:
                 record = cls(**kwargs)
                 sqlalchemy.db.session.add(record)
                 items.append(record)
             sqlalchemy.db.session.commit()
             ids = [r.id for r in items]
             return sqlalchemy.db.session.query(cls).filter(cls.id.in_(ids)).all()
 
     @classmethod
-    def bulk_delete(cls, items: list):
+    def bulk_update(cls, values: list) -> list:
+        ids = []
+        with sqlalchemy.app_context():
+            for kwargs in values:
+                if 'id' not in kwargs:
+                    continue
+                ids.append(kwargs['id'])
+                record = cls.find_by(id=kwargs['id'])
+                if record is not None:
+                    for key, val in kwargs.items():
+                        setattr(record, key, val)
+                    sqlalchemy.db.session.add(record)
+            sqlalchemy.db.session.commit()
+            return sqlalchemy.db.session.query(cls).filter(cls.id.in_(ids)).all()
+
+    @classmethod
+    def bulk_delete(cls, items: list) -> None:
         with sqlalchemy.app_context():
             for item in items:
                 sqlalchemy.db.session.delete(item)
             sqlalchemy.db.session.commit()
 
     @classmethod
-    def drop_table(cls):
+    def drop_table(cls) -> None:
         if cls.table_exists():
             with sqlalchemy.app_context():
                 cls.__table__.drop(sqlalchemy.db.engine)
 
     @classmethod
-    def create_table(cls):
+    def create_table(cls) -> None:
         if not cls.table_exists():
             with sqlalchemy.app_context():
                 cls.__table__.create(sqlalchemy.db.engine, checkfirst=True)
 
     @classmethod
-    def clear_table(cls):
+    def clear_table(cls) -> None:
         if cls.table_exists():
             cls.drop_table()
             cls.create_table()
 
     @classmethod
-    def table_exists(cls):
+    def table_exists(cls) -> bool:
         return sqlalchemy.has_table(cls.__tablename__)
 
     @classmethod
-    def _seed_table(cls, path: Path or str):
+    def _seed_table(cls, path: Path or str) -> None:
         if not cls.table_exists():
             cls.create_table()
         file = Path(path)
         if not file.exists():
             raise FileNotFoundError(f'Could not find: {str(file)}')
         with open(file, 'r') as r:
             values = json.load(r)
             assert isinstance(values, list)
             cls.bulk_insert(values)
 
     @classmethod
-    def seed_table(cls):
+    def seed_table(cls) -> None:
         ...
 
     @classmethod
     def group_by(cls):
         # TODO: add a group by
         # need execution to consoladate because
         # not all bots in the same server
@@ -107,15 +123,15 @@
 
     def create(self):
         with sqlalchemy.app_context():
             sqlalchemy.db.session.add(self)
             sqlalchemy.db.session.commit()
             return self.find_by(id=self.id)
 
-    def delete(self):
+    def delete(self) -> None:
         with sqlalchemy.app_context():
             sqlalchemy.db.session.delete(self)
             sqlalchemy.db.session.commit()
 
     def keys(self) -> list:
         return self.columns()
```

### Comparing `arkdata-1.0.2/src/arkdata/models/__init__.py` & `arkdata-1.0.3/src/arkdata/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 from arkdata.models.structure import Structure
 from arkdata.models.tool import Tool
 from arkdata.models.trophy import Trophy
 from arkdata.models.user import User
 from arkdata.models.weapon import Weapon
 from arkdata.models.server import Server
 from arkdata.models.sessions import Session
+from arkdata.models.admin import Admin
 
 
 __all__ = ['Account',
+           'Admin',
            'Ammunition',
            'Armour',
            'Artifact',
            'Attachment',
            'CartItem',
            'Command',
            'Consumable',
```

### Comparing `arkdata-1.0.2/src/arkdata/models/account.py` & `arkdata-1.0.3/src/arkdata/models/account.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 from arkdata.database.cursor import sqlalchemy
 from arkdata.database.table import Table
 from sqlalchemy import Column, String, Integer
 from pathlib import Path
 import os
 import arkdata
-from secrets import token_urlsafe
 
 
 class Account(sqlalchemy.db.Model, Table):
     xuid = Column(String(100), nullable=False, unique=True)
     player_name = Column(String(100), nullable=True, default=None)
     ark_player_id = Column(Integer, nullable=True, default=None)
     berry_bush_seeds = Column(Integer, nullable=False, default=0)
-    api_token = Column(String(100), nullable=True, default=token_urlsafe)
 
-    def __init__(self, xuid=None, player_name=None, ark_player_id=None, berry_bush_seeds=0, api_token=None):
+    def __init__(self, xuid=None, player_name=None, ark_player_id=None, berry_bush_seeds=0):
         self.xuid = xuid
         self.player_name = player_name
         self.ark_player_id = ark_player_id
         self.berry_bush_seeds = berry_bush_seeds
-        self.api_token = api_token
 
     @classmethod
     def seed_table(cls):
         directory = Path(os.path.dirname(arkdata.__file__))
         path = directory / Path('seeds/accounts.json')
         super()._seed_table(path)
 
-    def generate_api_token(self):
-        self.api_token = token_urlsafe()
-
+
```

### Comparing `arkdata-1.0.2/src/arkdata/models/ammunition.py` & `arkdata-1.0.3/src/arkdata/models/ammunition.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/armour.py` & `arkdata-1.0.3/src/arkdata/models/armour.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/artifact.py` & `arkdata-1.0.3/src/arkdata/models/artifact.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/attachment.py` & `arkdata-1.0.3/src/arkdata/models/attachment.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/cart_item.py` & `arkdata-1.0.3/src/arkdata/models/cart_item.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/command.py` & `arkdata-1.0.3/src/arkdata/models/seed.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,33 @@
 from arkdata.database.cursor import sqlalchemy
 from arkdata.database.table import Table
-from sqlalchemy import Column, String, Integer, Boolean
-
-
-class Command(sqlalchemy.db.Model, Table):
-
-    xuid = Column(String(100), unique=False, nullable=True)
-    operation = Column(String(100), unique=False, nullable=False, default="OTHER")
-    operation_id = Column(Integer, unique=False, nullable=True, default=None)
-    code = Column(String(500), unique=False, nullable=False)
-    executed = Column(Boolean, unique=False, nullable=False, default=False)
-
-    # Admin's player id
-    player_id = Column(String(100), unique=False, nullable=True, default=None)
-    # Game Server IP Address or URL
-    address = Column(String(100), unique=False, nullable=True, default=None)
-    # Server id
-    server_id = Column(Integer, unique=False, nullable=True, default=None)
-
-    def __init__(
-            self,
-            xuid=None,
-            operation=None,
-            operation_id=None,
-            code=None,
-            executed=None,
-            player_id=None,
-            address=None,
-            server_id=None
-    ):
-        self.xuid = xuid
-        self.operation = operation
-        self.operation_id = operation_id
-        self.code = code
-        self.executed = executed
-        self.player_id = player_id
-        self.address = address
-        self.server_id = server_id
-
-    @classmethod
-    def execute_all(cls):
-        pass
+from sqlalchemy import Column, String, Integer, Text
+import os
+import arkdata
+from pathlib import Path
+
+
+class Seed(sqlalchemy.db.Model, Table):
+
+    name = Column(String(100), unique=True, nullable=False)
+    stack_size = Column(Integer, nullable=True, default=None)
+    class_name = Column(String(100), nullable=True, default=None)
+    blueprint = Column(String(200), nullable=True, default=None)
+    description = Column(Text, nullable=True, default=None)
+    image_url = Column(String(500), nullable=True, default=None)
+    url = Column(String(500), nullable=True, default=None)
+
+    def __init__(self, id=None, name=None, stack_size=None, class_name=None, blueprint=None, description=None, image_url=None, url=None):
+        self.id = id
+        self.name = name
+        self.stack_size = stack_size
+        self.class_name = class_name
+        self.blueprint = blueprint
+        self.description = description
+        self.image_url = image_url
+        self.url = url
 
     @classmethod
-    def executes(cls, **where):
-        pass
-
-    def server(self):
-        pass
-
-    def execute(self):
-        pass
-
-    def product(self):
-        pass
-
-    def user(self):
-        pass
-
+    def seed_table(cls):
+        directory = Path(os.path.dirname(arkdata.__file__))
+        path = directory / Path('seeds/seeds.json')
+        super()._seed_table(path)
```

### Comparing `arkdata-1.0.2/src/arkdata/models/consumable.py` & `arkdata-1.0.3/src/arkdata/models/consumable.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/creature.py` & `arkdata-1.0.3/src/arkdata/models/creature.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/dye.py` & `arkdata-1.0.3/src/arkdata/models/dye.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/egg.py` & `arkdata-1.0.3/src/arkdata/models/egg.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/farm.py` & `arkdata-1.0.3/src/arkdata/models/farm.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/order_item.py` & `arkdata-1.0.3/src/arkdata/models/order_item.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/product.py` & `arkdata-1.0.3/src/arkdata/models/product.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/recipe.py` & `arkdata-1.0.3/src/arkdata/models/recipe.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/resource.py` & `arkdata-1.0.3/src/arkdata/models/resource.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/saddle.py` & `arkdata-1.0.3/src/arkdata/models/saddle.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/seed.py` & `arkdata-1.0.3/src/arkdata/models/skin.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from arkdata.database.table import Table
 from sqlalchemy import Column, String, Integer, Text
 import os
 import arkdata
 from pathlib import Path
 
 
-class Seed(sqlalchemy.db.Model, Table):
+class Skin(sqlalchemy.db.Model, Table):
 
     name = Column(String(100), unique=True, nullable=False)
     stack_size = Column(Integer, nullable=True, default=None)
     class_name = Column(String(100), nullable=True, default=None)
     blueprint = Column(String(200), nullable=True, default=None)
     description = Column(Text, nullable=True, default=None)
     image_url = Column(String(500), nullable=True, default=None)
@@ -25,9 +25,9 @@
         self.description = description
         self.image_url = image_url
         self.url = url
 
     @classmethod
     def seed_table(cls):
         directory = Path(os.path.dirname(arkdata.__file__))
-        path = directory / Path('seeds/seeds.json')
+        path = directory / Path('seeds/skins.json')
         super()._seed_table(path)
```

### Comparing `arkdata-1.0.2/src/arkdata/models/sessions.py` & `arkdata-1.0.3/src/arkdata/models/sessions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 from sqlalchemy import Column, String, Boolean
 from arkdata.database.cursor import sqlalchemy
 from arkdata.database.table import Table
 from secrets import token_urlsafe
-import bcrypt
-from arkdata import models
+from pathlib import Path
+import arkdata
+import os
 
 
 class Session(sqlalchemy.db.Model, Table):
     xuid = Column(String(100), nullable=False, unique=True)
-    session_token = Column(String(100), default=None)
-    security_token = Column(String(100), default=None)
+    session_token = Column(String(100), default=token_urlsafe)
+    security_token = Column(String(100), default=token_urlsafe)
+    api_token = Column(String(100), nullable=True, default=token_urlsafe)
     authenticated = Column(Boolean, default=False)
 
-    def __init__(self, xuid=None, session_token=None, security_token=None, authenticated=False):
+    def __init__(self, xuid=None, session_token=None, security_token=None, api_token=None, authenticated=False):
         self.xuid = xuid
         self.session_token = session_token
         self.security_token = security_token
+        self.api_token = api_token
         self.authenticated = authenticated
 
     @classmethod
-    def login(cls, gamertag: str, password: str) -> 'User' or None:
-        user = models.User.find_by(gamertag=gamertag)
-        if user is None:
-            return
-        is_password_valid = bcrypt.checkpw(password.encode(), user.password_digest.encode())
-        if not is_password_valid:
-            return
-        session = Session.find_by(xuid=user.xuid)
-        session.new_session_token()
-        return user
-
-    @classmethod
-    def authenticate_security_token(cls, security_token: str) -> 'User' or None:
-        session = Session.find_by(security_token=security_token)
-        if session is not None:
-            session.new_security_token()
-            return models.User.find_by(xuid=session.xuid)
+    def seed_table(cls):
+        dir = Path(os.path.dirname(arkdata.__file__))
+        path = dir / Path('seeds/sessions.json')
+        super()._seed_table(path)
 
     def logout(self) -> None:
-        self.session_token = token_urlsafe(64)
-        self.commit()
+        with sqlalchemy.app_context():
+            self.session_token = token_urlsafe(64)
+            sqlalchemy.db.session.commit()
+
+    def new_session_token(self):
+        self(session_token=token_urlsafe(64))
+        return self.session_token
 
     def new_security_token(self):
-        self.security_token = token_urlsafe(64)
-        self.commit()
+        self(session_token=token_urlsafe(64))
+        return self.security_token
         # TODO: Send token to xbox account
 
+    def new_api_token(self):
+        self(session_token=token_urlsafe(64))
+        return self.api_token
+
```

### Comparing `arkdata-1.0.2/src/arkdata/models/skin.py` & `arkdata-1.0.3/src/arkdata/models/tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from arkdata.database.table import Table
 from sqlalchemy import Column, String, Integer, Text
 import os
 import arkdata
 from pathlib import Path
 
 
-class Skin(sqlalchemy.db.Model, Table):
+class Tool(sqlalchemy.db.Model, Table):
 
     name = Column(String(100), unique=True, nullable=False)
     stack_size = Column(Integer, nullable=True, default=None)
     class_name = Column(String(100), nullable=True, default=None)
     blueprint = Column(String(200), nullable=True, default=None)
     description = Column(Text, nullable=True, default=None)
     image_url = Column(String(500), nullable=True, default=None)
@@ -25,9 +25,9 @@
         self.description = description
         self.image_url = image_url
         self.url = url
 
     @classmethod
     def seed_table(cls):
         directory = Path(os.path.dirname(arkdata.__file__))
-        path = directory / Path('seeds/skins.json')
+        path = directory / Path('seeds/tools.json')
         super()._seed_table(path)
```

### Comparing `arkdata-1.0.2/src/arkdata/models/structure.py` & `arkdata-1.0.3/src/arkdata/models/structure.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/models/tool.py` & `arkdata-1.0.3/src/arkdata/models/trophy.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from arkdata.database.table import Table
 from sqlalchemy import Column, String, Integer, Text
 import os
 import arkdata
 from pathlib import Path
 
 
-class Tool(sqlalchemy.db.Model, Table):
+
+class Trophy(sqlalchemy.db.Model, Table):
 
     name = Column(String(100), unique=True, nullable=False)
     stack_size = Column(Integer, nullable=True, default=None)
     class_name = Column(String(100), nullable=True, default=None)
     blueprint = Column(String(200), nullable=True, default=None)
     description = Column(Text, nullable=True, default=None)
     image_url = Column(String(500), nullable=True, default=None)
@@ -25,9 +26,9 @@
         self.description = description
         self.image_url = image_url
         self.url = url
 
     @classmethod
     def seed_table(cls):
         directory = Path(os.path.dirname(arkdata.__file__))
-        path = directory / Path('seeds/tools.json')
-        super()._seed_table(path)
+        path = directory / Path('seeds/trophies.json')
+        super()._seed_table(path)
```

### Comparing `arkdata-1.0.2/src/arkdata/models/trophy.py` & `arkdata-1.0.3/src/arkdata/models/weapon.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from arkdata.database.table import Table
 from sqlalchemy import Column, String, Integer, Text
 import os
 import arkdata
 from pathlib import Path
 
 
-
-class Trophy(sqlalchemy.db.Model, Table):
+class Weapon(sqlalchemy.db.Model, Table):
 
     name = Column(String(100), unique=True, nullable=False)
     stack_size = Column(Integer, nullable=True, default=None)
     class_name = Column(String(100), nullable=True, default=None)
     blueprint = Column(String(200), nullable=True, default=None)
     description = Column(Text, nullable=True, default=None)
     image_url = Column(String(500), nullable=True, default=None)
@@ -26,9 +25,9 @@
         self.description = description
         self.image_url = image_url
         self.url = url
 
     @classmethod
     def seed_table(cls):
         directory = Path(os.path.dirname(arkdata.__file__))
-        path = directory / Path('seeds/trophies.json')
-        super()._seed_table(path)
+        path = directory / Path('seeds/weapons.json')
+        super()._seed_table(path)
```

### Comparing `arkdata-1.0.2/src/arkdata/models/user.py` & `arkdata-1.0.3/src/arkdata/models/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,80 @@
 from sqlalchemy import Column, String
 from arkdata.database.cursor import sqlalchemy
 from arkdata.database.table import Table
 from pathlib import Path
 import os
 import arkdata
 from arkdata import models
-from secrets import token_urlsafe
 import bcrypt
 
 
+def random_xuid():
+    from random import randint
+    return f"temporary_xuid_{randint(1, 10000)}"
+
+
 class User(sqlalchemy.db.Model, Table):
     xuid = Column(String(100), nullable=False, unique=True)
     gamertag = Column(String(100))
     password_digest = Column(String(100))
 
     def __init__(self, xuid=None, gamertag=None, password_digest=None):
-        self.xuid = xuid
-        self.gamertag = gamertag
-        self.password_digest = password_digest
+        self.xuid: str = xuid
+        self.gamertag: str = gamertag
+        self.password_digest: str = password_digest
 
     @classmethod
-    def create_user(cls, gamertag=None, password=None):
-        xuid = token_urlsafe()
+    def create_user(cls, gamertag: str, password: str) -> 'User':
+        xuid = random_xuid()
         password_digest = bcrypt.hashpw(password.encode(), bcrypt.gensalt()).decode()
         user = cls(xuid=xuid, gamertag=gamertag, password_digest=password_digest)
         user.create()
         session = models.Session(xuid=xuid)
         session.create()
         session.new_session_token()
+        account = models.Account(xuid=xuid)
+        account.create()
         return user
 
     @classmethod
-    def seed_table(cls):
+    def seed_table(cls) -> None:
         dir = Path(os.path.dirname(arkdata.__file__))
         path = dir / Path('seeds/users.json')
         super()._seed_table(path)
 
+    @classmethod
+    def login(cls, gamertag: str, password: str) -> 'User' or None:
+        user = models.User.find_by(gamertag=gamertag)
+        if user is None:
+            return
+        is_password_valid = bcrypt.checkpw(password.encode(), user.password_digest.encode())
+        if not is_password_valid:
+            return
+        session = user.session()
+        session.new_session_token()
+        return user
+
+    def change_password(self, password: str) -> bool:
+        if not isinstance(password, str):
+            return False
+        password_digest = bcrypt.hashpw(password.encode(), bcrypt.gensalt()).decode()
+        self(password_digest=password_digest)
+        admin = models.Admin(xuid=self.xuid)
+        if admin:
+            admin(nitrado_api_key_digest=None)
+        return True
+
     def session(self):
         return models.Session.find_by(xuid=self.xuid)
 
     def account(self):
         return models.Account.find_by(xuid=self.xuid)
 
-    def cart_items(self):
+    def cart_items(self) -> list:
         return models.CartItem.find_all_by(xuid=self.xuid)
 
-    def orders(self):
-        return models.OrderItem.find_all_by(xuid=self.xuid)
+    def orders_by_id(self, order_number: str) -> list:
+        return models.OrderItem.find_all_by(xuid=self.xuid, order_number=order_number)
 
+    def is_admin(self):
+        return models.Admin.find_by(xuid=self.xuid) is not None
```

### Comparing `arkdata-1.0.2/src/arkdata/seeds/ammunitions.json` & `arkdata-1.0.3/src/arkdata/seeds/ammunitions.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/armours.json` & `arkdata-1.0.3/src/arkdata/seeds/armours.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/artifacts.json` & `arkdata-1.0.3/src/arkdata/seeds/artifacts.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/attachments.json` & `arkdata-1.0.3/src/arkdata/seeds/attachments.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/consumables.json` & `arkdata-1.0.3/src/arkdata/seeds/consumables.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/creatures.json` & `arkdata-1.0.3/src/arkdata/seeds/creatures.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/dyes.json` & `arkdata-1.0.3/src/arkdata/seeds/dyes.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/eggs.json` & `arkdata-1.0.3/src/arkdata/seeds/eggs.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/farms.json` & `arkdata-1.0.3/src/arkdata/seeds/farms.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/products.json` & `arkdata-1.0.3/src/arkdata/seeds/products.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/recipes.json` & `arkdata-1.0.3/src/arkdata/seeds/recipes.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/resources.json` & `arkdata-1.0.3/src/arkdata/seeds/resources.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/saddles.json` & `arkdata-1.0.3/src/arkdata/seeds/saddles.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/seeds.json` & `arkdata-1.0.3/src/arkdata/seeds/seeds.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/skins.json` & `arkdata-1.0.3/src/arkdata/seeds/skins.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/structures.json` & `arkdata-1.0.3/src/arkdata/seeds/structures.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/tools.json` & `arkdata-1.0.3/src/arkdata/seeds/tools.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/trophies.json` & `arkdata-1.0.3/src/arkdata/seeds/trophies.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata/seeds/weapons.json` & `arkdata-1.0.3/src/arkdata/seeds/weapons.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.2/src/arkdata.egg-info/PKG-INFO` & `arkdata-1.0.3/src/arkdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdata
-Version: 1.0.2
+Version: 1.0.3
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Data
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Data/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdata-1.0.2/src/arkdata.egg-info/SOURCES.txt` & `arkdata-1.0.3/src/arkdata.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/arkdata/database/__init__.py
 src/arkdata/database/configuration.py
 src/arkdata/database/cursor.py
 src/arkdata/database/database.py
 src/arkdata/database/table.py
 src/arkdata/models/__init__.py
 src/arkdata/models/account.py
+src/arkdata/models/admin.py
 src/arkdata/models/ammunition.py
 src/arkdata/models/armour.py
 src/arkdata/models/artifact.py
 src/arkdata/models/attachment.py
 src/arkdata/models/cart_item.py
 src/arkdata/models/command.py
 src/arkdata/models/consumable.py
@@ -39,14 +40,15 @@
 src/arkdata/models/structure.py
 src/arkdata/models/tool.py
 src/arkdata/models/trophy.py
 src/arkdata/models/user.py
 src/arkdata/models/weapon.py
 src/arkdata/seeds/__init__.py
 src/arkdata/seeds/accounts.json
+src/arkdata/seeds/admins.json
 src/arkdata/seeds/ammunitions.json
 src/arkdata/seeds/armours.json
 src/arkdata/seeds/artifacts.json
 src/arkdata/seeds/attachments.json
 src/arkdata/seeds/commands.json
 src/arkdata/seeds/consumables.json
 src/arkdata/seeds/creatures.json
@@ -54,13 +56,14 @@
 src/arkdata/seeds/eggs.json
 src/arkdata/seeds/farms.json
 src/arkdata/seeds/products.json
 src/arkdata/seeds/recipes.json
 src/arkdata/seeds/resources.json
 src/arkdata/seeds/saddles.json
 src/arkdata/seeds/seeds.json
+src/arkdata/seeds/sessions.json
 src/arkdata/seeds/skins.json
 src/arkdata/seeds/structures.json
 src/arkdata/seeds/tools.json
 src/arkdata/seeds/trophies.json
 src/arkdata/seeds/users.json
 src/arkdata/seeds/weapons.json
```

