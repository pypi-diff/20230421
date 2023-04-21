# Comparing `tmp/arkdata-1.0.3.tar.gz` & `tmp/arkdata-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkdata-1.0.3.tar", last modified: Fri Apr 21 04:07:13 2023, max compression
+gzip compressed data, was "arkdata-1.0.4.tar", last modified: Fri Apr 21 04:20:10 2023, max compression
```

## Comparing `arkdata-1.0.3.tar` & `arkdata-1.0.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 04:07:13.008636 arkdata-1.0.3/
--rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:13.000000 arkdata-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      650 2023-04-21 04:07:13.009636 arkdata-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-03-25 16:35:13.000000 arkdata-1.0.3/README.md
--rw-rw-rw-   0        0        0      642 2023-04-16 02:13:53.000000 arkdata-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1223 2023-04-21 04:07:13.010636 arkdata-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 04:07:12.948580 arkdata-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 04:07:12.954580 arkdata-1.0.3/src/arkdata/
--rw-rw-rw-   0        0        0       54 2023-04-02 01:40:29.000000 arkdata-1.0.3/src/arkdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:07:12.964127 arkdata-1.0.3/src/arkdata/database/
--rw-rw-rw-   0        0        0      242 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/database/__init__.py
--rw-rw-rw-   0        0        0      860 2023-03-27 03:33:59.000000 arkdata-1.0.3/src/arkdata/database/configuration.py
--rw-rw-rw-   0        0        0     3371 2023-04-11 01:32:04.000000 arkdata-1.0.3/src/arkdata/database/cursor.py
--rw-rw-rw-   0        0        0     1470 2023-03-30 01:55:50.000000 arkdata-1.0.3/src/arkdata/database/database.py
--rw-rw-rw-   0        0        0     5948 2023-04-21 03:49:32.000000 arkdata-1.0.3/src/arkdata/database/table.py
--rw-rw-rw-   0        0        0        0 2023-03-27 03:33:59.000000 arkdata-1.0.3/src/arkdata/main.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:07:12.985636 arkdata-1.0.3/src/arkdata/models/
--rw-rw-rw-   0        0        0     2175 2023-04-21 00:38:08.000000 arkdata-1.0.3/src/arkdata/models/__init__.py
--rw-rw-rw-   0        0        0      961 2023-04-19 02:45:08.000000 arkdata-1.0.3/src/arkdata/models/account.py
--rw-rw-rw-   0        0        0     3556 2023-04-21 02:09:27.000000 arkdata-1.0.3/src/arkdata/models/admin.py
--rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/ammunition.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/armour.py
--rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/artifact.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/attachment.py
--rw-rw-rw-   0        0        0     1397 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/cart_item.py
--rw-rw-rw-   0        0        0     1684 2023-04-21 02:46:11.000000 arkdata-1.0.3/src/arkdata/models/command.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/consumable.py
--rw-rw-rw-   0        0        0     1808 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/creature.py
--rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/dye.py
--rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/egg.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/farm.py
--rw-rw-rw-   0        0        0     1416 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/order_item.py
--rw-rw-rw-   0        0        0     2782 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/product.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/recipe.py
--rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/resource.py
--rw-rw-rw-   0        0        0     1629 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/saddle.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/seed.py
--rw-rw-rw-   0        0        0      668 2023-04-20 02:17:11.000000 arkdata-1.0.3/src/arkdata/models/server.py
--rw-rw-rw-   0        0        0     1652 2023-04-19 03:24:44.000000 arkdata-1.0.3/src/arkdata/models/sessions.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/skin.py
--rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/structure.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/tool.py
--rw-rw-rw-   0        0        0     1289 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/trophy.py
--rw-rw-rw-   0        0        0     2735 2023-04-21 01:56:51.000000 arkdata-1.0.3/src/arkdata/models/user.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.3/src/arkdata/models/weapon.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:07:13.008636 arkdata-1.0.3/src/arkdata/seeds/
--rw-rw-rw-   0        0        0        0 2023-03-30 03:59:09.000000 arkdata-1.0.3/src/arkdata/seeds/__init__.py
--rw-rw-rw-   0        0        0      393 2023-04-16 22:10:50.000000 arkdata-1.0.3/src/arkdata/seeds/accounts.json
--rw-rw-rw-   0        0        0      103 2023-04-21 01:36:05.000000 arkdata-1.0.3/src/arkdata/seeds/admins.json
--rw-rw-rw-   0        0        0    16119 2023-03-30 06:36:40.000000 arkdata-1.0.3/src/arkdata/seeds/ammunitions.json
--rw-rw-rw-   0        0        0    36003 2023-03-30 03:50:59.000000 arkdata-1.0.3/src/arkdata/seeds/armours.json
--rw-rw-rw-   0        0        0    32929 2023-03-30 03:50:56.000000 arkdata-1.0.3/src/arkdata/seeds/artifacts.json
--rw-rw-rw-   0        0        0     3081 2023-03-30 03:50:48.000000 arkdata-1.0.3/src/arkdata/seeds/attachments.json
--rw-rw-rw-   0        0        0      567 2023-04-21 02:51:27.000000 arkdata-1.0.3/src/arkdata/seeds/commands.json
--rw-rw-rw-   0        0        0   100583 2023-03-30 03:50:36.000000 arkdata-1.0.3/src/arkdata/seeds/consumables.json
--rw-rw-rw-   0        0        0   589770 2023-03-30 03:50:20.000000 arkdata-1.0.3/src/arkdata/seeds/creatures.json
--rw-rw-rw-   0        0        0    11428 2023-03-30 03:50:14.000000 arkdata-1.0.3/src/arkdata/seeds/dyes.json
--rw-rw-rw-   0        0        0    57046 2023-03-30 03:50:12.000000 arkdata-1.0.3/src/arkdata/seeds/eggs.json
--rw-rw-rw-   0        0        0     3588 2023-03-30 03:50:09.000000 arkdata-1.0.3/src/arkdata/seeds/farms.json
--rw-rw-rw-   0        0        0   225349 2023-03-30 06:03:15.000000 arkdata-1.0.3/src/arkdata/seeds/products.json
--rw-rw-rw-   0        0        0     8457 2023-03-30 03:50:01.000000 arkdata-1.0.3/src/arkdata/seeds/recipes.json
--rw-rw-rw-   0        0        0    52865 2023-03-30 03:49:55.000000 arkdata-1.0.3/src/arkdata/seeds/resources.json
--rw-rw-rw-   0        0        0    57917 2023-03-30 07:19:16.000000 arkdata-1.0.3/src/arkdata/seeds/saddles.json
--rw-rw-rw-   0        0        0    16789 2023-03-30 03:47:57.000000 arkdata-1.0.3/src/arkdata/seeds/seeds.json
--rw-rw-rw-   0        0        0      494 2023-04-16 22:10:50.000000 arkdata-1.0.3/src/arkdata/seeds/sessions.json
--rw-rw-rw-   0        0        0   180774 2023-03-30 03:44:21.000000 arkdata-1.0.3/src/arkdata/seeds/skins.json
--rw-rw-rw-   0        0        0   185254 2023-03-30 03:44:16.000000 arkdata-1.0.3/src/arkdata/seeds/structures.json
--rw-rw-rw-   0        0        0    12933 2023-03-30 03:44:10.000000 arkdata-1.0.3/src/arkdata/seeds/tools.json
--rw-rw-rw-   0        0        0    23142 2023-03-30 03:44:02.000000 arkdata-1.0.3/src/arkdata/seeds/trophies.json
--rw-rw-rw-   0        0        0      292 2023-04-16 22:10:50.000000 arkdata-1.0.3/src/arkdata/seeds/users.json
--rw-rw-rw-   0        0        0    29591 2023-03-30 03:43:50.000000 arkdata-1.0.3/src/arkdata/seeds/weapons.json
-drwxrwxrwx   0        0        0        0 2023-04-21 04:07:12.958582 arkdata-1.0.3/src/arkdata.egg-info/
--rw-rw-rw-   0        0        0      650 2023-04-21 04:07:12.000000 arkdata-1.0.3/src/arkdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2038 2023-04-21 04:07:12.000000 arkdata-1.0.3/src/arkdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 04:07:12.000000 arkdata-1.0.3/src/arkdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      167 2023-04-21 04:07:12.000000 arkdata-1.0.3/src/arkdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 04:07:12.000000 arkdata-1.0.3/src/arkdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 04:20:10.901897 arkdata-1.0.4/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:13.000000 arkdata-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      650 2023-04-21 04:20:10.902898 arkdata-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-03-25 16:35:13.000000 arkdata-1.0.4/README.md
+-rw-rw-rw-   0        0        0      642 2023-04-16 02:13:53.000000 arkdata-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1223 2023-04-21 04:20:10.903899 arkdata-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 04:20:10.845890 arkdata-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 04:20:10.850892 arkdata-1.0.4/src/arkdata/
+-rw-rw-rw-   0        0        0       54 2023-04-02 01:40:29.000000 arkdata-1.0.4/src/arkdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:20:10.858893 arkdata-1.0.4/src/arkdata/database/
+-rw-rw-rw-   0        0        0      242 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/database/__init__.py
+-rw-rw-rw-   0        0        0      860 2023-03-27 03:33:59.000000 arkdata-1.0.4/src/arkdata/database/configuration.py
+-rw-rw-rw-   0        0        0     3371 2023-04-11 01:32:04.000000 arkdata-1.0.4/src/arkdata/database/cursor.py
+-rw-rw-rw-   0        0        0     1470 2023-03-30 01:55:50.000000 arkdata-1.0.4/src/arkdata/database/database.py
+-rw-rw-rw-   0        0        0     5948 2023-04-21 03:49:32.000000 arkdata-1.0.4/src/arkdata/database/table.py
+-rw-rw-rw-   0        0        0        0 2023-03-27 03:33:59.000000 arkdata-1.0.4/src/arkdata/main.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:20:10.880897 arkdata-1.0.4/src/arkdata/models/
+-rw-rw-rw-   0        0        0     2175 2023-04-21 00:38:08.000000 arkdata-1.0.4/src/arkdata/models/__init__.py
+-rw-rw-rw-   0        0        0      961 2023-04-19 02:45:08.000000 arkdata-1.0.4/src/arkdata/models/account.py
+-rw-rw-rw-   0        0        0     3556 2023-04-21 02:09:27.000000 arkdata-1.0.4/src/arkdata/models/admin.py
+-rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/ammunition.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/armour.py
+-rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/artifact.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/attachment.py
+-rw-rw-rw-   0        0        0     1397 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/cart_item.py
+-rw-rw-rw-   0        0        0     1684 2023-04-21 02:46:11.000000 arkdata-1.0.4/src/arkdata/models/command.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/consumable.py
+-rw-rw-rw-   0        0        0     1808 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/creature.py
+-rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/dye.py
+-rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/egg.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/farm.py
+-rw-rw-rw-   0        0        0     1416 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/order_item.py
+-rw-rw-rw-   0        0        0     2782 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/product.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/recipe.py
+-rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/resource.py
+-rw-rw-rw-   0        0        0     1629 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/saddle.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/seed.py
+-rw-rw-rw-   0        0        0      668 2023-04-20 02:17:11.000000 arkdata-1.0.4/src/arkdata/models/server.py
+-rw-rw-rw-   0        0        0     1652 2023-04-19 03:24:44.000000 arkdata-1.0.4/src/arkdata/models/sessions.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/skin.py
+-rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/structure.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/tool.py
+-rw-rw-rw-   0        0        0     1289 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/trophy.py
+-rw-rw-rw-   0        0        0     2735 2023-04-21 01:56:51.000000 arkdata-1.0.4/src/arkdata/models/user.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.4/src/arkdata/models/weapon.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:20:10.901897 arkdata-1.0.4/src/arkdata/seeds/
+-rw-rw-rw-   0        0        0        0 2023-03-30 03:59:09.000000 arkdata-1.0.4/src/arkdata/seeds/__init__.py
+-rw-rw-rw-   0        0        0      393 2023-04-16 22:10:50.000000 arkdata-1.0.4/src/arkdata/seeds/accounts.json
+-rw-rw-rw-   0        0        0      103 2023-04-21 01:36:05.000000 arkdata-1.0.4/src/arkdata/seeds/admins.json
+-rw-rw-rw-   0        0        0    16119 2023-03-30 06:36:40.000000 arkdata-1.0.4/src/arkdata/seeds/ammunitions.json
+-rw-rw-rw-   0        0        0    36003 2023-03-30 03:50:59.000000 arkdata-1.0.4/src/arkdata/seeds/armours.json
+-rw-rw-rw-   0        0        0    32929 2023-03-30 03:50:56.000000 arkdata-1.0.4/src/arkdata/seeds/artifacts.json
+-rw-rw-rw-   0        0        0     3081 2023-03-30 03:50:48.000000 arkdata-1.0.4/src/arkdata/seeds/attachments.json
+-rw-rw-rw-   0        0        0      567 2023-04-21 02:51:27.000000 arkdata-1.0.4/src/arkdata/seeds/commands.json
+-rw-rw-rw-   0        0        0   100583 2023-03-30 03:50:36.000000 arkdata-1.0.4/src/arkdata/seeds/consumables.json
+-rw-rw-rw-   0        0        0   589770 2023-03-30 03:50:20.000000 arkdata-1.0.4/src/arkdata/seeds/creatures.json
+-rw-rw-rw-   0        0        0    11428 2023-03-30 03:50:14.000000 arkdata-1.0.4/src/arkdata/seeds/dyes.json
+-rw-rw-rw-   0        0        0    57046 2023-03-30 03:50:12.000000 arkdata-1.0.4/src/arkdata/seeds/eggs.json
+-rw-rw-rw-   0        0        0     3588 2023-03-30 03:50:09.000000 arkdata-1.0.4/src/arkdata/seeds/farms.json
+-rw-rw-rw-   0        0        0   225349 2023-03-30 06:03:15.000000 arkdata-1.0.4/src/arkdata/seeds/products.json
+-rw-rw-rw-   0        0        0     8457 2023-03-30 03:50:01.000000 arkdata-1.0.4/src/arkdata/seeds/recipes.json
+-rw-rw-rw-   0        0        0    52865 2023-03-30 03:49:55.000000 arkdata-1.0.4/src/arkdata/seeds/resources.json
+-rw-rw-rw-   0        0        0    57917 2023-03-30 07:19:16.000000 arkdata-1.0.4/src/arkdata/seeds/saddles.json
+-rw-rw-rw-   0        0        0    16789 2023-03-30 03:47:57.000000 arkdata-1.0.4/src/arkdata/seeds/seeds.json
+-rw-rw-rw-   0        0        0      494 2023-04-16 22:10:50.000000 arkdata-1.0.4/src/arkdata/seeds/sessions.json
+-rw-rw-rw-   0        0        0   180774 2023-03-30 03:44:21.000000 arkdata-1.0.4/src/arkdata/seeds/skins.json
+-rw-rw-rw-   0        0        0   185254 2023-03-30 03:44:16.000000 arkdata-1.0.4/src/arkdata/seeds/structures.json
+-rw-rw-rw-   0        0        0    12933 2023-03-30 03:44:10.000000 arkdata-1.0.4/src/arkdata/seeds/tools.json
+-rw-rw-rw-   0        0        0    23142 2023-03-30 03:44:02.000000 arkdata-1.0.4/src/arkdata/seeds/trophies.json
+-rw-rw-rw-   0        0        0      292 2023-04-16 22:10:50.000000 arkdata-1.0.4/src/arkdata/seeds/users.json
+-rw-rw-rw-   0        0        0    29591 2023-03-30 03:43:50.000000 arkdata-1.0.4/src/arkdata/seeds/weapons.json
+drwxrwxrwx   0        0        0        0 2023-04-21 04:20:10.854888 arkdata-1.0.4/src/arkdata.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-04-21 04:20:10.000000 arkdata-1.0.4/src/arkdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2038 2023-04-21 04:20:10.000000 arkdata-1.0.4/src/arkdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 04:20:10.000000 arkdata-1.0.4/src/arkdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2023-04-21 04:20:10.000000 arkdata-1.0.4/src/arkdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 04:20:10.000000 arkdata-1.0.4/src/arkdata.egg-info/top_level.txt
```

### Comparing `arkdata-1.0.3/LICENSE` & `arkdata-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/PKG-INFO` & `arkdata-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdata
-Version: 1.0.3
+Version: 1.0.4
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Data
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Data/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdata-1.0.3/pyproject.toml` & `arkdata-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/setup.cfg` & `arkdata-1.0.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6461 7461 0d0a 7665 7273   = arkdata..vers
-00000020: 696f 6e20 3d20 312e 302e 330d 0a74 6573  ion = 1.0.3..tes
+00000020: 696f 6e20 3d20 312e 302e 340d 0a74 6573  ion = 1.0.4..tes
 00000030: 745f 7665 7273 696f 6e20 3d20 312e 302e  t_version = 1.0.
 00000040: 340d 0a70 726f 6475 6374 696f 6e5f 7665  4..production_ve
-00000050: 7273 696f 6e20 3d20 312e 302e 330d 0a61  rsion = 1.0.3..a
+00000050: 7273 696f 6e20 3d20 312e 302e 340d 0a61  rsion = 1.0.4..a
 00000060: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
 00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000080: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
 00000090: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 000000b0: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
 000000c0: 6363 6573 7365 7320 7468 6520 4172 6b20  ccesses the Ark
```

### Comparing `arkdata-1.0.3/src/arkdata/database/configuration.py` & `arkdata-1.0.4/src/arkdata/database/configuration.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/database/cursor.py` & `arkdata-1.0.4/src/arkdata/database/cursor.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/database/database.py` & `arkdata-1.0.4/src/arkdata/database/database.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/database/table.py` & `arkdata-1.0.4/src/arkdata/database/table.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/__init__.py` & `arkdata-1.0.4/src/arkdata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/account.py` & `arkdata-1.0.4/src/arkdata/models/account.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/admin.py` & `arkdata-1.0.4/src/arkdata/models/admin.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/ammunition.py` & `arkdata-1.0.4/src/arkdata/models/ammunition.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/armour.py` & `arkdata-1.0.4/src/arkdata/models/armour.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/artifact.py` & `arkdata-1.0.4/src/arkdata/models/artifact.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/attachment.py` & `arkdata-1.0.4/src/arkdata/models/attachment.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/cart_item.py` & `arkdata-1.0.4/src/arkdata/models/cart_item.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/command.py` & `arkdata-1.0.4/src/arkdata/models/command.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/consumable.py` & `arkdata-1.0.4/src/arkdata/models/consumable.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/creature.py` & `arkdata-1.0.4/src/arkdata/models/creature.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/dye.py` & `arkdata-1.0.4/src/arkdata/models/dye.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/egg.py` & `arkdata-1.0.4/src/arkdata/models/egg.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/farm.py` & `arkdata-1.0.4/src/arkdata/models/farm.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/order_item.py` & `arkdata-1.0.4/src/arkdata/models/order_item.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/product.py` & `arkdata-1.0.4/src/arkdata/models/product.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/recipe.py` & `arkdata-1.0.4/src/arkdata/models/recipe.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/resource.py` & `arkdata-1.0.4/src/arkdata/models/resource.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/saddle.py` & `arkdata-1.0.4/src/arkdata/models/saddle.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/seed.py` & `arkdata-1.0.4/src/arkdata/models/seed.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/server.py` & `arkdata-1.0.4/src/arkdata/models/server.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/sessions.py` & `arkdata-1.0.4/src/arkdata/models/sessions.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/skin.py` & `arkdata-1.0.4/src/arkdata/models/skin.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/structure.py` & `arkdata-1.0.4/src/arkdata/models/structure.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/tool.py` & `arkdata-1.0.4/src/arkdata/models/tool.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/trophy.py` & `arkdata-1.0.4/src/arkdata/models/trophy.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/user.py` & `arkdata-1.0.4/src/arkdata/models/user.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/models/weapon.py` & `arkdata-1.0.4/src/arkdata/models/weapon.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/ammunitions.json` & `arkdata-1.0.4/src/arkdata/seeds/ammunitions.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/armours.json` & `arkdata-1.0.4/src/arkdata/seeds/armours.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/artifacts.json` & `arkdata-1.0.4/src/arkdata/seeds/artifacts.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/attachments.json` & `arkdata-1.0.4/src/arkdata/seeds/attachments.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/commands.json` & `arkdata-1.0.4/src/arkdata/seeds/commands.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/consumables.json` & `arkdata-1.0.4/src/arkdata/seeds/consumables.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/creatures.json` & `arkdata-1.0.4/src/arkdata/seeds/creatures.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/dyes.json` & `arkdata-1.0.4/src/arkdata/seeds/dyes.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/eggs.json` & `arkdata-1.0.4/src/arkdata/seeds/eggs.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/farms.json` & `arkdata-1.0.4/src/arkdata/seeds/farms.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/products.json` & `arkdata-1.0.4/src/arkdata/seeds/products.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/recipes.json` & `arkdata-1.0.4/src/arkdata/seeds/recipes.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/resources.json` & `arkdata-1.0.4/src/arkdata/seeds/resources.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/saddles.json` & `arkdata-1.0.4/src/arkdata/seeds/saddles.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/seeds.json` & `arkdata-1.0.4/src/arkdata/seeds/seeds.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/skins.json` & `arkdata-1.0.4/src/arkdata/seeds/skins.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/structures.json` & `arkdata-1.0.4/src/arkdata/seeds/structures.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/tools.json` & `arkdata-1.0.4/src/arkdata/seeds/tools.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/trophies.json` & `arkdata-1.0.4/src/arkdata/seeds/trophies.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata/seeds/weapons.json` & `arkdata-1.0.4/src/arkdata/seeds/weapons.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.3/src/arkdata.egg-info/PKG-INFO` & `arkdata-1.0.4/src/arkdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdata
-Version: 1.0.3
+Version: 1.0.4
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Data
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Data/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdata-1.0.3/src/arkdata.egg-info/SOURCES.txt` & `arkdata-1.0.4/src/arkdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

