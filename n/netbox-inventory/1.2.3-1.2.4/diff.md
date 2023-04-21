# Comparing `tmp/netbox-inventory-1.2.3.tar.gz` & `tmp/netbox-inventory-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-inventory-1.2.3.tar", last modified: Fri Apr 14 11:39:57 2023, max compression
+gzip compressed data, was "netbox-inventory-1.2.4.tar", last modified: Fri Apr 21 16:16:23 2023, max compression
```

## Comparing `netbox-inventory-1.2.3.tar` & `netbox-inventory-1.2.4.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.870301 netbox-inventory-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.854301 netbox-inventory-1.2.3/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.858301 netbox-inventory-1.2.3/netbox_inventory/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.858301 netbox-inventory-1.2.3/netbox_inventory/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)    17266 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/bulk_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/reassign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.858301 netbox-inventory-1.2.3/netbox_inventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/migrations/0001_initial_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/migrations/0002_alter_asset_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.850301 netbox-inventory-1.2.3/netbox_inventory/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.862301 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_assign.html
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_create.html
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_reassign.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.862301 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_tenant.html
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/purchase.html
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/supplier.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.862301 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.862301 netbox-inventory-1.2.3/netbox_inventory/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/netbox_inventory/tests/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_views_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_views_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_group/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_group/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_type/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_type/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/netbox_inventory/tests/purchase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/purchase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/purchase/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/purchase/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/netbox_inventory/tests/supplier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/supplier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/supplier/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/supplier/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/netbox_inventory/views/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/asset_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/asset_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/asset_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/inventoryitem_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/inventoryitem_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/purchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.854301 netbox-inventory-1.2.3/netbox_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-04-14 11:39:57.000000 netbox-inventory-1.2.3/netbox_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-14 11:39:57.000000 netbox-inventory-1.2.3/netbox_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:39:57.000000 netbox-inventory-1.2.3/netbox_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 11:39:57.000000 netbox-inventory-1.2.3/netbox_inventory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 11:39:57.870301 netbox-inventory-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.099333 netbox-inventory-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-04-21 16:16:23.099333 netbox-inventory-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.083334 netbox-inventory-1.2.4/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.083334 netbox-inventory-1.2.4/netbox_inventory/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.087334 netbox-inventory-1.2.4/netbox_inventory/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/bulk_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/reassign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.087334 netbox-inventory-1.2.4/netbox_inventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/migrations/0001_initial_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/migrations/0002_alter_asset_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.079334 netbox-inventory-1.2.4/netbox_inventory/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.091333 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_assign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_reassign.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.091333 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_tenant.html
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/purchase.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/supplier.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.091333 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.091333 netbox-inventory-1.2.4/netbox_inventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.095333 netbox-inventory-1.2.4/netbox_inventory/tests/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_views_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_views_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.095333 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_group/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_group/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.095333 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_type/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_type/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.095333 netbox-inventory-1.2.4/netbox_inventory/tests/purchase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/purchase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/purchase/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/purchase/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.099333 netbox-inventory-1.2.4/netbox_inventory/tests/supplier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/supplier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/supplier/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/supplier/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.099333 netbox-inventory-1.2.4/netbox_inventory/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/asset_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/asset_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/asset_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/inventoryitem_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/inventoryitem_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/tabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.083334 netbox-inventory-1.2.4/netbox_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-04-21 16:16:23.000000 netbox-inventory-1.2.4/netbox_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-21 16:16:23.000000 netbox-inventory-1.2.4/netbox_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:16:23.000000 netbox-inventory-1.2.4/netbox_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 16:16:23.000000 netbox-inventory-1.2.4/netbox_inventory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 16:16:23.099333 netbox-inventory-1.2.4/setup.cfg
```

### Comparing `netbox-inventory-1.2.3/LICENSE` & `netbox-inventory-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/PKG-INFO` & `netbox-inventory-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.2.3
+Version: 1.2.4
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netbox-inventory-1.2.3/README.md` & `netbox-inventory-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/__init__.py` & `netbox-inventory-1.2.4/netbox_inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/analyzers.py` & `netbox-inventory-1.2.4/netbox_inventory/analyzers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/api/nested_serializers.py` & `netbox-inventory-1.2.4/netbox_inventory/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/api/serializers.py` & `netbox-inventory-1.2.4/netbox_inventory/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/api/urls.py` & `netbox-inventory-1.2.4/netbox_inventory/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/api/views.py` & `netbox-inventory-1.2.4/netbox_inventory/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/filtersets.py` & `netbox-inventory-1.2.4/netbox_inventory/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/forms/assign.py` & `netbox-inventory-1.2.4/netbox_inventory/forms/assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/forms/bulk.py` & `netbox-inventory-1.2.4/netbox_inventory/forms/bulk.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
     class Meta:
         model = Asset
         fields = (
             'name', 'asset_tag', 'serial', 'status',
             'hardware_kind', 'manufacturer', 'model_name', 'part_number',
             'model_comments', 'storage_site', 'storage_location',
             'owner', 'purchase', 'purchase_date', 'supplier',
-            'warranty_start', 'warranty_end', 'comments', 'tenant', 'contact',
+            'warranty_start', 'warranty_end', 'comments', 'tenant', 'contact', 'tags',
         )
 
     def clean_model_name(self):
         hardware_kind = self.cleaned_data.get('hardware_kind')
         manufacturer = self.cleaned_data.get('manufacturer')
         model = self.cleaned_data.get('model_name')
         if not hardware_kind or not manufacturer:
@@ -330,15 +330,15 @@
         Returns cleaned value for a given field from self.data
         Used when creating additional related objects on import, since the values
         are otherwise not validated by forms.
         Used for DateTime, Boolean and similar fields. If used on ModelField and
         instance does not exist it raises Exception but no feedback is given to user.
         """
         try:
-            return self.fields[field_name].clean(self.data.get(field_name))
+            return self.base_fields[field_name].clean(self.data.get(field_name))
         except forms.ValidationError as e:
             self.add_error(field_name, e)
             raise
 
 
 class SupplierImportForm(NetBoxModelImportForm):
     class Meta:
```

### Comparing `netbox-inventory-1.2.3/netbox_inventory/forms/create.py` & `netbox-inventory-1.2.4/netbox_inventory/forms/create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/forms/filters.py` & `netbox-inventory-1.2.4/netbox_inventory/forms/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/forms/models.py` & `netbox-inventory-1.2.4/netbox_inventory/forms/models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/forms/reassign.py` & `netbox-inventory-1.2.4/netbox_inventory/forms/reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/migrations/0001_initial_prod.py` & `netbox-inventory-1.2.4/netbox_inventory/migrations/0001_initial_prod.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/migrations/0003_add_inventoryitemgroup.py` & `netbox-inventory-1.2.4/netbox_inventory/migrations/0003_add_inventoryitemgroup.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py` & `netbox-inventory-1.2.4/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/models.py` & `netbox-inventory-1.2.4/netbox_inventory/models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/navigation.py` & `netbox-inventory-1.2.4/netbox_inventory/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/search.py` & `netbox-inventory-1.2.4/netbox_inventory/search.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/signals.py` & `netbox-inventory-1.2.4/netbox_inventory/signals.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tables.py` & `netbox-inventory-1.2.4/netbox_inventory/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/template_content.py` & `netbox-inventory-1.2.4/netbox_inventory/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_reassign.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_reassign.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_info.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_info.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_tenant.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_tenant.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/purchase.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/purchase.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/supplier.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/supplier.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html` & `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_api.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_models.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_views.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_views_create.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_views_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_views_reassign.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_views_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/custom.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_group/test_api.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_group/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_group/test_views.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_group/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_type/test_api.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_type/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_type/test_views.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_type/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/purchase/test_api.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/purchase/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/purchase/test_views.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/purchase/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/settings.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/settings.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/supplier/test_api.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/supplier/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/supplier/test_views.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/supplier/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/tests/test_load.py` & `netbox-inventory-1.2.4/netbox_inventory/tests/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class NetboxDnsVersionTestCase(SimpleTestCase):
     """
     Test for netbox_inventory package
     """
 
     def test_version(self):
-        assert __version__ == "1.2.3"
+        assert __version__ == "1.2.4"
 
 
 class AppTest(APITestCase):
     """
     Test the availability of the plugin API root
     """
```

### Comparing `netbox-inventory-1.2.3/netbox_inventory/urls.py` & `netbox-inventory-1.2.4/netbox_inventory/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/utils.py` & `netbox-inventory-1.2.4/netbox_inventory/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/views/asset.py` & `netbox-inventory-1.2.4/netbox_inventory/views/asset.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/views/asset_assign.py` & `netbox-inventory-1.2.4/netbox_inventory/views/asset_assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/views/asset_create.py` & `netbox-inventory-1.2.4/netbox_inventory/views/asset_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/views/asset_reassign.py` & `netbox-inventory-1.2.4/netbox_inventory/views/asset_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/views/inventoryitem_group.py` & `netbox-inventory-1.2.4/netbox_inventory/views/inventoryitem_group.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/views/inventoryitem_type.py` & `netbox-inventory-1.2.4/netbox_inventory/views/inventoryitem_type.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/views/purchase.py` & `netbox-inventory-1.2.4/netbox_inventory/views/purchase.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/views/supplier.py` & `netbox-inventory-1.2.4/netbox_inventory/views/supplier.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory/views/tabs.py` & `netbox-inventory-1.2.4/netbox_inventory/views/tabs.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/netbox_inventory.egg-info/PKG-INFO` & `netbox-inventory-1.2.4/netbox_inventory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.2.3
+Version: 1.2.4
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netbox-inventory-1.2.3/netbox_inventory.egg-info/SOURCES.txt` & `netbox-inventory-1.2.4/netbox_inventory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.3/pyproject.toml` & `netbox-inventory-1.2.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-inventory"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   { name="Matej Vadnjal", email="matej.vadnjal@arnes.si" },
 ]
 description = "Inventory asset management in NetBox"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

