# Comparing `tmp/fittings-2.0.0.tar.gz` & `tmp/fittings-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fittings-2.0.0.tar", last modified: Thu Apr 20 05:13:46 2023, max compression
+gzip compressed data, was "dist/fittings-2.0.1.tar", last modified: Fri Apr 21 05:03:00 2023, max compression
```

## Comparing `fittings-2.0.0.tar` & `fittings-2.0.1.tar`

### file list

```diff
@@ -1,150 +1,187 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/
--rw-r--r--   0 root         (0) root         (0)     5574 2023-04-20 05:13:46.000000 fittings-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35065 2023-04-20 05:13:35.000000 fittings-2.0.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/auth_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/cogs/
--rw-rw-rw-   0 root         (0) root         (0)     8433 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/cogs/fittings.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/templates/fittings/
--rw-rw-rw-   0 root         (0) root         (0)     2417 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/edit_fit.html
--rw-rw-rw-   0 root         (0) root         (0)    35170 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/view_fit.html
--rw-rw-rw-   0 root         (0) root         (0)     4478 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/view_all_categories.html
--rw-rw-rw-   0 root         (0) root         (0)     3666 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     6497 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/view_doctrine.html
--rw-rw-rw-   0 root         (0) root         (0)     3345 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/view_all_fits.html
--rw-rw-rw-   0 root         (0) root         (0)     6031 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/edit_category.html
--rw-rw-rw-   0 root         (0) root         (0)     6365 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/add_doctrine.html
--rw-rw-rw-   0 root         (0) root         (0)     3704 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/base.html
--rw-rw-rw-   0 root         (0) root         (0)     8161 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/view_category.html
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/add_fit.html
--rw-rw-rw-   0 root         (0) root         (0)     6312 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/create_category.html
--rw-rw-rw-   0 root         (0) root         (0)     6766 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/edit_doctrine.html
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      727 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/management/commands/fittings_preload_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/static/fittings/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/static/fittings/img/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/
--rw-rw-rw-   0 root         (0) root         (0)     8580 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/7m.png
--rw-rw-rw-   0 root         (0) root         (0)     4956 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/4m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/0l.png
--rw-rw-rw-   0 root         (0) root         (0)     5888 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/5l.png
--rw-rw-rw-   0 root         (0) root         (0)    43642 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/h.png
--rw-rw-rw-   0 root         (0) root         (0)     7439 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/6m.png
--rw-rw-rw-   0 root         (0) root         (0)     7399 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/5s.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/r.png
--rw-rw-rw-   0 root         (0) root         (0)     4607 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/3h.png
--rw-rw-rw-   0 root         (0) root         (0)     3541 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/2h.png
--rw-rw-rw-   0 root         (0) root         (0)    16840 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/circle.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/l.png
--rw-rw-rw-   0 root         (0) root         (0)     4886 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/3r.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/m.png
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/2m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/0r.png
--rw-rw-rw-   0 root         (0) root         (0)     3720 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/3m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/0m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/0s.png
--rw-rw-rw-   0 root         (0) root         (0)     6109 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/5h.png
--rw-rw-rw-   0 root         (0) root         (0)     4628 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/4l.png
--rw-rw-rw-   0 root         (0) root         (0)    33523 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/dustwheel.png
--rw-rw-rw-   0 root         (0) root         (0)     8972 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/8l.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/0h.png
--rw-rw-rw-   0 root         (0) root         (0)     9490 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/4s.png
--rw-rw-rw-   0 root         (0) root         (0)     6270 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/5m.png
--rw-rw-rw-   0 root         (0) root         (0)    38343 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_default.png
--rw-rw-rw-   0 root         (0) root         (0)    43560 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_blue.png
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/working.jpg
--rw-rw-rw-   0 root         (0) root         (0)     8067 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/7l.png
--rw-rw-rw-   0 root         (0) root         (0)     2512 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/1r.png
--rw-rw-rw-   0 root         (0) root         (0)     8879 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/noship.png
--rw-rw-rw-   0 root         (0) root         (0)     1976 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/1l.png
--rw-rw-rw-   0 root         (0) root         (0)     5309 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/4h.png
--rw-rw-rw-   0 root         (0) root         (0)     8288 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/7h.png
--rw-rw-rw-   0 root         (0) root         (0)     3523 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/3l.png
--rw-rw-rw-   0 root         (0) root         (0)     7203 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/6h.png
--rw-rw-rw-   0 root         (0) root         (0)     2590 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/1h.png
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/1m.png
--rw-rw-rw-   0 root         (0) root         (0)    42868 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_revelations.png
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/blank.png
--rw-rw-rw-   0 root         (0) root         (0)     2570 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/2l.png
--rw-rw-rw-   0 root         (0) root         (0)     3497 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/2r.png
--rw-rw-rw-   0 root         (0) root         (0)     7014 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/6l.png
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/error.jpg
--rw-rw-rw-   0 root         (0) root         (0)    42833 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_darkred.png
--rw-rw-rw-   0 root         (0) root         (0)     9541 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/8m.png
--rw-rw-rw-   0 root         (0) root         (0)     9276 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/8h.png
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6647 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/models.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/tests.py
--rw-rw-rw-   0 root         (0) root         (0)    24902 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/views.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0005_unicategory.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      750 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0003_remove_type_description_not_null.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0008_auto_20200605_0736.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0014_serverversion.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0010_auto_20200718_2227.py
--rw-rw-rw-   0 root         (0) root         (0)     6132 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0011_auto_20200815_2022.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0012_typehistory.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0013_alter_doctrine_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0007_auto_20200605_0735.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0004_add_item_category_and_group.py
--rw-rw-rw-   0 root         (0) root         (0)      718 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0009_auto_20200605_2117.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0002_add_dgm_unique_constraints.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0006_auto_20200605_0724.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10078 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/ru/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10229 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10085 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/fr_FR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/fr_FR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/fr_FR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10038 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6341 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/ja/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    13534 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5900 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    12224 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/ko_KR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/ko_KR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5263 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/ko_KR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    13034 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templatetags/filters.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1409 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-04-20 05:13:35.000000 fittings-2.0.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1645 2023-04-20 05:13:35.000000 fittings-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5574 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4857 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)     4554 2023-04-20 05:13:35.000000 fittings-2.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-20 05:13:46.000000 fittings-2.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-04-21 05:03:00.000000 fittings-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35065 2023-04-21 05:02:49.000000 fittings-2.0.1/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/auth_hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/cogs/
+-rw-rw-rw-   0 root         (0) root         (0)     8433 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/cogs/fittings.py
+-rw-rw-rw-   0 root         (0) root         (0)     9750 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/templates/fittings/
+-rw-rw-rw-   0 root         (0) root         (0)     2417 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/edit_fit.html
+-rw-rw-rw-   0 root         (0) root         (0)    35122 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/view_fit.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/templates/fittings/bundles/
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/bundles/multi-select-css.html
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/bundles/jquery.quicksearch-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      519 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/bundles/multi-select-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/bundles/slim-select-css.html
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/bundles/clipboard-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/bundles/slim-select-js.html
+-rw-rw-rw-   0 root         (0) root         (0)     4517 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/view_all_categories.html
+-rw-rw-rw-   0 root         (0) root         (0)     3705 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     6518 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/view_doctrine.html
+-rw-rw-rw-   0 root         (0) root         (0)     3384 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/view_all_fits.html
+-rw-rw-rw-   0 root         (0) root         (0)     5852 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/edit_category.html
+-rw-rw-rw-   0 root         (0) root         (0)     6080 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/add_doctrine.html
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     8161 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/view_category.html
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/add_fit.html
+-rw-rw-rw-   0 root         (0) root         (0)     6133 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/create_category.html
+-rw-rw-rw-   0 root         (0) root         (0)     6419 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/edit_doctrine.html
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/management/commands/fittings_preload_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     7759 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/zh.json
+-rw-rw-rw-   0 root         (0) root         (0)     8110 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/it-IT.json
+-rw-rw-rw-   0 root         (0) root         (0)     7731 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/en-GB.json
+-rw-rw-rw-   0 root         (0) root         (0)     8452 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/fr-FR.json
+-rw-rw-rw-   0 root         (0) root         (0)    10517 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/ru.json
+-rw-rw-rw-   0 root         (0) root         (0)     8241 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/es-ES.json
+-rw-rw-rw-   0 root         (0) root         (0)     2988 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/ja.json
+-rw-rw-rw-   0 root         (0) root         (0)     7318 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/uk.json
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/ko.json
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/de-DE.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/img/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/
+-rw-rw-rw-   0 root         (0) root         (0)     8580 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/7m.png
+-rw-rw-rw-   0 root         (0) root         (0)     4956 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/4m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/0l.png
+-rw-rw-rw-   0 root         (0) root         (0)     5888 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/5l.png
+-rw-rw-rw-   0 root         (0) root         (0)    43642 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/h.png
+-rw-rw-rw-   0 root         (0) root         (0)     7439 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/6m.png
+-rw-rw-rw-   0 root         (0) root         (0)     7399 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/5s.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/r.png
+-rw-rw-rw-   0 root         (0) root         (0)     4607 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/3h.png
+-rw-rw-rw-   0 root         (0) root         (0)     3541 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/2h.png
+-rw-rw-rw-   0 root         (0) root         (0)    16840 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/circle.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/l.png
+-rw-rw-rw-   0 root         (0) root         (0)     4886 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/3r.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/m.png
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/2m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/0r.png
+-rw-rw-rw-   0 root         (0) root         (0)     3720 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/3m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/0m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/0s.png
+-rw-rw-rw-   0 root         (0) root         (0)     6109 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/5h.png
+-rw-rw-rw-   0 root         (0) root         (0)     4628 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/4l.png
+-rw-rw-rw-   0 root         (0) root         (0)    33523 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/dustwheel.png
+-rw-rw-rw-   0 root         (0) root         (0)     8972 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/8l.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/0h.png
+-rw-rw-rw-   0 root         (0) root         (0)     9490 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/4s.png
+-rw-rw-rw-   0 root         (0) root         (0)     6270 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/5m.png
+-rw-rw-rw-   0 root         (0) root         (0)    38343 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_default.png
+-rw-rw-rw-   0 root         (0) root         (0)    43560 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_blue.png
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/working.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     8067 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/7l.png
+-rw-rw-rw-   0 root         (0) root         (0)     2512 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/1r.png
+-rw-rw-rw-   0 root         (0) root         (0)     8879 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/noship.png
+-rw-rw-rw-   0 root         (0) root         (0)     1976 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/1l.png
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/4h.png
+-rw-rw-rw-   0 root         (0) root         (0)     8288 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/7h.png
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/3l.png
+-rw-rw-rw-   0 root         (0) root         (0)     7203 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/6h.png
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/1h.png
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/1m.png
+-rw-rw-rw-   0 root         (0) root         (0)    42868 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_revelations.png
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/blank.png
+-rw-rw-rw-   0 root         (0) root         (0)     2570 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/2l.png
+-rw-rw-rw-   0 root         (0) root         (0)     3497 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/2r.png
+-rw-rw-rw-   0 root         (0) root         (0)     7014 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/6l.png
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/error.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    42833 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_darkred.png
+-rw-rw-rw-   0 root         (0) root         (0)     9541 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/8m.png
+-rw-rw-rw-   0 root         (0) root         (0)     9276 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/8h.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/clipboard.js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)    10753 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/clipboard.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/0.9.12/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/
+-rw-rw-rw-   0 root         (0) root         (0)    19224 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/jquery.multi-select.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/multi-select.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/jquery.quicksearch/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)    10904 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/jquery,quicksearch.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/slim-select/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/slim-select/1.26.0/
+-rw-rw-rw-   0 root         (0) root         (0)     6240 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.css
+-rw-rw-rw-   0 root         (0) root         (0)    35553 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.js
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6647 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)    24902 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/views.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0005_unicategory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      750 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0003_remove_type_description_not_null.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0008_auto_20200605_0736.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0014_serverversion.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0010_auto_20200718_2227.py
+-rw-rw-rw-   0 root         (0) root         (0)     6132 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0011_auto_20200815_2022.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0012_typehistory.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0013_alter_doctrine_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0007_auto_20200605_0735.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0004_add_item_category_and_group.py
+-rw-rw-rw-   0 root         (0) root         (0)      718 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0009_auto_20200605_2117.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0002_add_dgm_unique_constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0006_auto_20200605_0724.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10078 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10229 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10085 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/fr_FR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/fr_FR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10038 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6341 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13534 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5900 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    12224 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/ko_KR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/ko_KR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5263 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13034 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templatetags/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templatetags/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-04-21 05:02:49.000000 fittings-2.0.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1645 2023-04-21 05:02:49.000000 fittings-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-04-21 05:02:59.000000 fittings-2.0.1/fittings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6120 2023-04-21 05:02:59.000000 fittings-2.0.1/fittings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 05:02:59.000000 fittings-2.0.1/fittings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-21 05:02:59.000000 fittings-2.0.1/fittings.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-04-21 05:02:59.000000 fittings-2.0.1/fittings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 05:02:59.000000 fittings-2.0.1/fittings.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)     4554 2023-04-21 05:02:49.000000 fittings-2.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-21 05:03:00.000000 fittings-2.0.1/setup.cfg
```

### Comparing `fittings-2.0.0/PKG-INFO` & `fittings-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fittings
-Version: 2.0.0
+Version: 2.0.1
 Summary: A simple fittings and doctrine management application.
 Home-page: https://gitlab.com/colcrunch/fittings
 Author: Col Crunch
 Author-email: it-team@serin.space
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `fittings-2.0.0/LICENSE` & `fittings-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/auth_hooks.py` & `fittings-2.0.1/fittings/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/cogs/fittings.py` & `fittings-2.0.1/fittings/cogs/fittings.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/tasks.py` & `fittings-2.0.1/fittings/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,41 +134,42 @@
                 types.append(_get_type(line.split(',')[0].strip()))
             else:
                 quantity = line.split()[-1]
                 if 'x' in quantity and quantity[1:].isdigit():
                     types.append(_get_type(line.split(quantity)[0].strip()))
                 else:
                     types.append(_get_type(line.strip()))
-        return all(_type is not None and _type.group.category_id == 87 for _type in types)
+        return all(_type is not None and _type.eve_group.eve_category.id == 87 for _type in types)
 
 
 def _get_type(type_name):
     try:
         type_obj = EveType.objects.get(name=type_name)
     except:
         # If the type is not already in the db, then we have to resolve type_id before we have eveuniverse
         # create the object.
         c = esi.client
         type_id = c.Universe.post_universe_ids(names=[type_name]).result()['inventory_types'][0]["id"]
         type_obj = EveType.objects.get_or_create_esi(id=type_id,enabled_sections=[EveType.Section.DOGMAS])
+        type_obj = type_obj[0]
     return type_obj
 
 
 @shared_task()
 def create_fitting_item(fit, item):
     count = None
     quantity = None
     if 'count' in item:
         count = item['count']
 
     type_obj = _get_type(item['name'])
 
     # Dogma Effects
     flags = {11: 'LoSlot', 12: 'HiSlot', 13: 'MedSlot', 2663: 'RigSlot', 3772: 'SubSystemSlot', 6306: 'ServiceSlot'}
-    effects = type_obj.dogma_effects.filter(effect_id__in=flags).values_list('effect_id', flat=True)
+    effects = type_obj.dogma_effects.filter(effect_id__in=flags).values_list('eve_dogma_effect_id', flat=True)
     effects = list(effects)
     if count is None:
         flag = item['section_name']
         quantity = item['quantity']
     # Check due to active drug from pyfa not showing quantities
     elif len(effects) == 0:
         flag = 'Cargo'
```

### Comparing `fittings-2.0.0/fittings/templates/fittings/edit_fit.html` & `fittings-2.0.1/fittings/templates/fittings/edit_fit.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/templates/fittings/view_fit.html` & `fittings-2.0.1/fittings/templates/fittings/view_fit.html`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
               </div>
             </div>
           </div>
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/2.0.4/clipboard.min.js"></script>
+    {% include 'fittings/bundles/clipboard-js.html' %}
     <script>
         var clipboard = new ClipboardJS('#buyAllButton');
     </script>
 {% endblock %}
 
 {% block extra_script %}
      $(document).ready(function() {
```

#### html2text {}

```diff
@@ -253,10 +253,11 @@
       {drone.quantity}}
     * {% endfor %} {% if fitting.FighterBay|length > 0 %}
     * {% translate "Fighter Bay" %}
     * {% endif %} {% for fighter in fitting.FighterBay %}
     * [{{ fighter.type_id|type_icon_url:32 }}] {{fighter.item_name}} x{
       {fighter.quantity}}
     * {% endfor %}
-{% endblock %} {% block extra_javascript %}
+{% endblock %} {% block extra_javascript %} {% include 'fittings/bundles/
+clipboard-js.html' %}
  {% endblock %} {% block extra_script %} $(document).ready(function() { $('
 [data-toggle="tooltip"]').tooltip(); }); {% endblock %}
```

### Comparing `fittings-2.0.0/fittings/templates/fittings/view_all_categories.html` & `fittings-2.0.1/fittings/templates/fittings/view_all_categories.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 {% extends 'fittings/base.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
+{% load static %}
+{% load tags %}
 
 
 {% block page_title %}{% translate "View All Categories" %}{% endblock %}
 
 {% block fittings_block %}
     {% if msg %}
             <div class="alert alert-{{ msg.0 }} alert-dismissible" role="alert">
@@ -76,14 +78,15 @@
 {% endblock %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
 {% endblock %}
 
 {% block extra_script %}
+    {% get_dt_lang LANGUAGE_CODE as LANG_PATH %}
     $(document).ready(function(){
         $('#fitTable').DataTable({
-            language: { url: '//cdn.datatables.net/plug-ins/1.12.1/i18n/{{ LANGUAGE_CODE }}.json' },
+            language: { url: '{% static LANG_PATH %}' },
         });
         $('[data-toggle="tooltip"]').tooltip();
     })
 {% endblock %}
```

### Comparing `fittings-2.0.0/fittings/templates/fittings/dashboard.html` & `fittings-2.0.1/fittings/templates/fittings/dashboard.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 {% extends 'fittings/base.html' %}
+{% load static %}
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
 {% load evelinks %}
+{% load tags %}
 
 {% block page_title %}{% translate "Dashboard" %}{% endblock %}
 
 {% block fittings_block %}
     {% if msg %}
         <div class="alert alert-{{ msg.0 }} alert-dismissible" role="alert">
             <button type="button" class="close" data-dismiss="alert" aria-label="close">
@@ -69,15 +71,16 @@
 {% endblock %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
 {% endblock %}
 
 {% block extra_script %}
+    {% get_dt_lang LANGUAGE_CODE as LANG_PATH %}
     $(document).ready(function(){
         $('#docTable').DataTable({
-            language: { url: '//cdn.datatables.net/plug-ins/1.12.1/i18n/{{ LANGUAGE_CODE }}.json' },
+            language: { url: '{% static LANG_PATH %}' },
             "order": [[ 1, "asc" ]],
         });
         $('[data-toggle="tooltip"]').tooltip();
     })
 {% endblock %}
```

### Comparing `fittings-2.0.0/fittings/templates/fittings/view_doctrine.html` & `fittings-2.0.1/fittings/templates/fittings/view_doctrine.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 {% extends 'fittings/base.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
 {% load static %}
 {% load evelinks %}
+{% load tags %}
 
 {% block page_title %}{{ doctrine.name }} {% translate "Doctrine" %}{% endblock %}
 
 {% block fittings_block %}
     {# modal start #}
     <div class="modal fade" id="deleteModal" role="dialog" tabindex="-1" aria-labelledby="modalTitle">
         <div class="modal-dialog" role="document">
@@ -112,17 +113,18 @@
 {% endblock %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
 {% endblock %}
 
 {% block extra_script %}
+    {% get_dt_lang LANGUAGE_CODE as LANG_PATH %}
      $(document).ready(function(){
         $('#fitsTable').DataTable({
-            language: { url: '//cdn.datatables.net/plug-ins/1.12.1/i18n/{{ LANGUAGE_CODE }}.json' },
+            language: { url: '{% static LANG_PATH %}' },
             paging: false,
             searching: false,
             order: [[1, 'asc']],
         });
         $('[data-toggle="tooltip"]').tooltip();
     })
 {% endblock %}
```

### Comparing `fittings-2.0.0/fittings/templates/fittings/view_all_fits.html` & `fittings-2.0.1/fittings/templates/fittings/view_all_fits.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 {% extends 'fittings/base.html' %}
+{% load tags %}
+{% load static %}
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
 {% load evelinks %}
 
 {% block page_title %}{% translate "View All Fits" %}{% endblock %}
 
@@ -65,14 +67,15 @@
 {% endblock %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
 {% endblock %}
 
 {% block extra_script %}
+    {% get_dt_lang LANGUAGE_CODE as LANG_PATH %}
     $(document).ready(function(){
         $('#fitTable').DataTable({
-            language: { url: '//cdn.datatables.net/plug-ins/1.12.1/i18n/{{ LANGUAGE_CODE }}.json' },
+            language: { url: '{% static LANG_PATH %}' },
         });
         $('[data-toggle="tooltip"]').tooltip();
     })
 {% endblock %}
```

### Comparing `fittings-2.0.0/fittings/templates/fittings/edit_category.html` & `fittings-2.0.1/fittings/templates/fittings/edit_category.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends 'fittings/base.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
 {% load static %}
 
 {% block more_css %}
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/multi-select/0.9.12/css/multi-select.min.css" />
+    {% include 'fittings/bundles/multi-select-css.html' %}
     <style>
         .form-control {
             margin: 2px;
         }
 
         .ms-container {
             width: 100% !important;
@@ -20,15 +20,15 @@
             display: block;
             border: none;
             height:100%;
             width: 100%;
         }
     </style>
 
-    <link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/slim-select/1.26.0/slimselect.min.css">
+    {% include 'fittings/bundles/slim-select-css.html' %}
 
 {% endblock %}
 
 {% block page_title %}{% translate "Edit Category" %}{% endblock %}
 
 {% block fittings_block %}
     <div class="container col-sm-12">
@@ -99,15 +99,15 @@
                 </div>
             </div>
         </div>
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/slim-select/1.26.0/slimselect.min.js"></script>
+    {% include 'fittings/bundles/slim-select-js.html' %}
 {% endblock %}
 
 
 {% block extra_script %}
 var color_picker = document.getElementById("color");
 var color_picker_wrapper = document.getElementById("color-wrapper");
 color_picker.onchange = function() {
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 {% extends 'fittings/base.html' %} {% load i18n %} {% load humanize %} {% load
-filters %} {% load static %} {% block more_css %}
-
- {% endblock %} {% block page_title %}{% translate "Edit Category" %}{%
-endblock %} {% block fittings_block %}
+filters %} {% load static %} {% block more_css %} {% include 'fittings/bundles/
+multi-select-css.html' %}
+ {% include 'fittings/bundles/slim-select-css.html' %} {% endblock %} {% block
+page_title %}{% translate "Edit Category" %}{% endblock %} {% block
+fittings_block %}
 {% translate "Edit Category" %}
 {% csrf_token %}
 {% translate "Category Name" %} [{{cat.name}}        ]
 {% translate "Category Color" %}
 [Unknown INPUT type]
 {% for group in groups %}
 % if group in cat.groups.all %} selected {%endif%}>{{group.name}}
@@ -15,16 +16,16 @@
 % if fit in cat.fittings.all %} selected {% endif %}>{{fit.name}}
 {% endfor %}
 {% for doc in docs %}
 % if doc in cat.doctrines.all %} selected {% endif %}>{{doc.name}}
 {% endfor %}
 
 {% translate "Submit" %}
-{% endblock %} {% block extra_javascript %}
- {% endblock %} {% block extra_script %} var color_picker =
+{% endblock %} {% block extra_javascript %} {% include 'fittings/bundles/slim-
+select-js.html' %} {% endblock %} {% block extra_script %} var color_picker =
 document.getElementById("color"); var color_picker_wrapper =
 document.getElementById("color-wrapper"); color_picker.onchange = function()
 { color_picker_wrapper.style.backgroundColor = color_picker.value; }
 color_picker_wrapper.style.backgroundColor = color_picker.value; new SlimSelect
 ({ select: "#groupSelect", hideSelectedOption: true }); new SlimSelect({select:
 "#fitSelect", hideSelectedOption: true}); new SlimSelect({select: "#docSelect",
 hideSelectedOption: true}); {% endblock %}
```

### Comparing `fittings-2.0.0/fittings/templates/fittings/add_doctrine.html` & `fittings-2.0.1/fittings/templates/fittings/edit_doctrine.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 {% extends 'fittings/base.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
 {% load static %}
 {% load evelinks %}
-
 {% block more_css %}
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/multi-select/0.9.12/css/multi-select.min.css" />
+    {% include 'fittings/bundles/multi-select-css.html' %}
     <style>
         .form-control {
             margin: 2px;
         }
-
         .ms-container {
             width: 100% !important;
         }
 
     </style>
 
 {% endblock %}
 
-{% block page_title %}{% translate "Add Doctrine" %}{% endblock %}
+{% block page_title %}{% translate "Edit Doctrine" %}{% endblock %}
 
 {% block fittings_block %}
     {% if msg %}
             <div class="alert alert-{{ msg.0 }} alert-dismissible" role="alert">
                     <button type="button" class="close" data-dismiss="alert" aria-label="close">
                         <span aria-hidden="true">&times</span>
                     </button>
@@ -41,37 +39,41 @@
                 <div class="row">
                     <div class="col-md-10 col-md-offset-1">
                         <form class="form-signin" role="form" action="" method="POST">
                             {% csrf_token %}
                             <div class="form-group">
                                 <label for="name" class="col-sm-2 control-label">{% translate "Doctrine Name" %}</label>
                                 <div class="col-sm-10">
-                                    <input type="text" class="form-control" name="name" id="name" required/>
+                                    <input type="text" class="form-control" name="name" id="name" value="{{ doctrine.name }}" required/>
                                 </div>
                             </div>
                             <div class="form-group">
                                 <label for="description" class="col-sm-2 control-label">{% translate "Doctrine Description" %}</label>
                                 <div class="col-sm-10">
-                                    <textarea class="form-control" name="description" id="description" rows="4"></textarea>
+                                    <textarea class="form-control" name="description" id="description" rows="4">{{ doctrine.description }}</textarea>
                                 </div>
                             </div>
                             <div class="form-group">
                                 <label for="fitSelect" class="col-sm-2 control-label">{% translate "Select Fits" %}</label>
                                 <div class="col-sm-10" style="margin-top: 5px; margin-bottom: 5px;">
                                     <select multiple="multiple" id="fitSelect" name="fitSelect">
-                                        {% for fit in fittings %}
-                                            <option value="{{ fit.pk }}">{{ fit.name }} ({{fit.ship_type.name}})</option>
+                                        {% for fit in doc_fits %}
+                                            <option value="{{ fit.pk }}" selected>{{ fit.name }} ({{ fit.ship_type.name }})</option>
+                                        {% endfor %}
+                                        {% for fit in fits %}
+                                            <option value="{{ fit.pk }}">{{ fit.name }} ({{fit.ship_type.type_name}})</option>
                                         {% endfor %}
                                     </select>
                                 </div>
                             </div>
                             <div class="form-group">
                                 <label for="iconSelect" class="col-sm-2 control-label">{% translate "Select Doctrine Icon" %}</label>
                                 <div class="col-sm-10">
                                     <select class="form-control" name="iconSelect" id="iconSelect" aria-describedby="helpBlock">
+                                        <option value="{{ doctrine.icon_url }}" selected> {% translate "Current Icon" %} </option>
                                         {% for ship in ships %}
                                             <option value="{{ ship.ship_type|type_render_url:64 }}">{{ship.ship_type__name}}</option>
                                         {% endfor %}
                                     </select>
                                     <span id="helpBlock" class="help-block"> {% translate "If you do not see the ship type that you would like to use for the icon, add a fit that uses that ship type and try again." %}</span>
                                 </div>
                             </div>
@@ -82,22 +84,22 @@
                 </div>
             </div>
         </div>
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/multi-select/0.9.12/js/jquery.multi-select.js" integrity="sha256-JU2QMhOvXGZtWxxkQTEgpVjdPHMYMuVYbYzNqfsioNw=" crossorigin="anonymous"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery.quicksearch/2.4.0/jquery.quicksearch.min.js" integrity="sha256-hD1kpQcVntR40eMx9uED+E4HAjD2OJkLIFcP6ukVd+g=" crossorigin="anonymous"></script>
+    {% include 'fittings/bundles/multi-select-js.html' %}
+    {% include 'fittings/bundles/jquery.quicksearch-js.html' %}
 {% endblock %}
 
 {% block extra_script %}
     $('#fitSelect').multiSelect({
-          selectableHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='{% translate "Search" %}' style='margin-bottom: 3px;'>",
-          selectionHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='{% translate "Search" %}' style='margin-bottom: 3px;'>",
+          selectableHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='Search' style='margin-bottom: 3px;'>",
+          selectionHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='Search' style='margin-bottom: 3px;'>",
           afterInit: function(ms){
             var that = this,
                 $selectableSearch = that.$selectableUl.prev(),
                 $selectionSearch = that.$selectionUl.prev(),
                 selectableSearchString = '#'+that.$container.attr('id')+' .ms-elem-selectable:not(.ms-selected)',
                 selectionSearchString = '#'+that.$container.attr('id')+' .ms-elem-selection.ms-selected';
```

#### html2text {}

```diff
@@ -1,36 +1,41 @@
 {% extends 'fittings/base.html' %} {% load i18n %} {% load humanize %} {% load
-filters %} {% load static %} {% load evelinks %} {% block more_css %}
- {% endblock %} {% block page_title %}{% translate "Add Doctrine" %}{% endblock
-%} {% block fittings_block %} {% if msg %}
+filters %} {% load static %} {% load evelinks %} {% block more_css %} {%
+include 'fittings/bundles/multi-select-css.html' %}
+ {% endblock %} {% block page_title %}{% translate "Edit Doctrine" %}{%
+endblock %} {% block fittings_block %} {% if msg %}
  ×  {% if msg.0 != 'warning' %}
 *** {% if msg.0 == 'danger' %}Oh No!{% elif msg.0 == 'success' %}Success!{%
 endif %} ***
 {% endif %}
 {{ msg.1 }}
 {% endif %}
 {% translate "New Doctrine" %}
 {% csrf_token %}
 {% translate "Doctrine Name" %}
-[name                ]
+[{{ doctrine.name }} ]
 {% translate "Doctrine Description" %}
+{{ doctrine.description }}
 {% translate "Select Fits" %}
-{% for fit in fittings %}
-{{ fit.name }} ({{fit.ship_type.name}})
+{% for fit in doc_fits %}
+{{ fit.name }} ({{ fit.ship_type.name }})
+{% endfor %} {% for fit in fits %}
+{{ fit.name }} ({{fit.ship_type.type_name}})
 {% endfor %}
 {% translate "Select Doctrine Icon" %}
 {% for ship in ships %}
 {{ship.ship_type__name}}
 {% endfor %}
   {% translate "If you do not see the ship type that you would like to use for
 the icon, add a fit that uses that ship type and try again." %}
 
 {% translate "Submit" %}
-{% endblock %} {% block extra_javascript %}
- {% endblock %} {% block extra_script %} $('#fitSelect').multiSelect(
+{% endblock %} {% block extra_javascript %} {% include 'fittings/bundles/multi-
+select-js.html' %} {% include 'fittings/bundles/jquery.quicksearch-js.html' %}
+{% endblock %} {% block extra_script %} $('#fitSelect').multiSelect(
 { selectableHeader: "[                    ]", selectionHeader: "
 [                    ]", afterInit: function(ms){ var that = this,
 $selectableSearch = that.$selectableUl.prev(), $selectionSearch =
 that.$selectionUl.prev(), selectableSearchString = '#'+that.$container.attr
 ('id')+' .ms-elem-selectable:not(.ms-selected)', selectionSearchString =
 '#'+that.$container.attr('id')+' .ms-elem-selection.ms-selected'; that.qs1 =
 $selectableSearch.quicksearch(selectableSearchString) .on('keydown', function
```

### Comparing `fittings-2.0.0/fittings/templates/fittings/base.html` & `fittings-2.0.1/fittings/templates/fittings/base.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/templates/fittings/view_category.html` & `fittings-2.0.1/fittings/templates/fittings/view_category.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/templates/fittings/add_fit.html` & `fittings-2.0.1/fittings/templates/fittings/add_fit.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/templates/fittings/create_category.html` & `fittings-2.0.1/fittings/templates/fittings/add_doctrine.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,129 @@
 {% extends 'fittings/base.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
 {% load static %}
+{% load evelinks %}
 
 {% block more_css %}
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/multi-select/0.9.12/css/multi-select.min.css" />
     <style>
         .form-control {
             margin: 2px;
         }
 
         .ms-container {
             width: 100% !important;
         }
 
-        input[type="color"] {
-            opacity: 0;
-            display: block;
-            border: none;
-            height:100%;
-            width: 100%;
-        }
     </style>
 
-    <link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/slim-select/1.26.0/slimselect.min.css">
-
 {% endblock %}
 
-{% block page_title %}{% translate "Add Category" %}{% endblock %}
+{% block page_title %}{% translate "Add Doctrine" %}{% endblock %}
 
 {% block fittings_block %}
+    {% if msg %}
+            <div class="alert alert-{{ msg.0 }} alert-dismissible" role="alert">
+                    <button type="button" class="close" data-dismiss="alert" aria-label="close">
+                        <span aria-hidden="true">&times</span>
+                    </button>
+                    {% if msg.0 != 'warning' %}<h4>{% if msg.0 == 'danger' %}Oh No!{% elif msg.0 == 'success' %}Success!{% endif %}</h4>{% endif %}
+                    <p>{{ msg.1 }}</p>
+                </div>
+        {% endif %}
     <div class="container col-sm-12">
         <div class="panel panel-primary">
             <div class="panel-heading">
-                {% translate "New Category" %}
+                {% translate "New Doctrine" %}
             </div>
             <div class="panel-body">
                 <div class="row">
                     <div class="col-md-10 col-md-offset-1">
-                        <form class="form" role="form" action="" method="POST">
+                        <form class="form-signin" role="form" action="" method="POST">
                             {% csrf_token %}
-                            <div class="row">
+                            <div class="form-group">
+                                <label for="name" class="col-sm-2 control-label">{% translate "Doctrine Name" %}</label>
                                 <div class="col-sm-10">
-                                    <div class="form-group">
-                                        <label for="name">{% translate "Category Name" %}</label>
-                                        <input type="text" class="form-control" name="name" id="name" required/>
-                                    </div>
-                                </div>
-                                <div class="col-sm-2">
-                                    <div class="form-group">
-                                        <label for="color">{% translate "Category Color" %}</label>
-                                        <div class="form-control col-sm-1" id="color-wrapper" style="padding:0 !important;">
-                                            <input type="color" name="color" id="color" value="#39CCCC" required/>
-                                        </div>
-                                    </div>
+                                    <input type="text" class="form-control" name="name" id="name" required/>
                                 </div>
                             </div>
-                            <div class="row">
-                                <div class="col-sm-12">
-                                    <div class="form-group">
-                                        <label for="groupSelect" style="margin-bottom: 0;">{% translate "Select Groups" %}</label>
-                                        <span class="help-block" style="margin-top: 0; margin-bottom: 0; font-size: 10pt; font-style: italic;">{% translate "Only selected groups will have access to fittings and doctrines in this category. If no groups are selected the category will be visible to all with fittings module access." %}</span>
-                                        <select name="groupSelect" id="groupSelect" multiple>
-                                            {% for group in groups %}
-                                            <option value="{{group.pk}}">{{group.name}}</option>
-                                            {% endfor %}
-                                        </select>
-                                    </div>
+                            <div class="form-group">
+                                <label for="description" class="col-sm-2 control-label">{% translate "Doctrine Description" %}</label>
+                                <div class="col-sm-10">
+                                    <textarea class="form-control" name="description" id="description" rows="4"></textarea>
                                 </div>
                             </div>
-                            <div class="row">
-                                <div class="col-sm-6">
-                                    <div class="form-group">
-                                        <label for="fitSelect">{% translate "Select Fits" %}</label>
-                                        <select name="fitSelect" id="fitSelect" multiple>
-                                            {% for fit in fits %}
-                                            <option value="{{fit.pk}}">{{fit.name}}</option>
-                                            {% endfor %}
-                                        </select>
-                                    </div>
+                            <div class="form-group">
+                                <label for="fitSelect" class="col-sm-2 control-label">{% translate "Select Fits" %}</label>
+                                <div class="col-sm-10" style="margin-top: 5px; margin-bottom: 5px;">
+                                    <select multiple="multiple" id="fitSelect" name="fitSelect">
+                                        {% for fit in fittings %}
+                                            <option value="{{ fit.pk }}">{{ fit.name }} ({{fit.ship_type.name}})</option>
+                                        {% endfor %}
+                                    </select>
                                 </div>
-                                <div class="col-sm-6">
-                                    <div class="form-group">
-                                        <label for="docSelect">{% translate "Select Doctrines" %}</label>
-                                        <select name="docSelect" id="docSelect" multiple>
-                                            {% for doc in docs %}
-                                            <option value="{{doc.pk}}">{{doc.name}}</option>
-                                            {% endfor %}
-                                        </select>
-                                    </div>
+                            </div>
+                            <div class="form-group">
+                                <label for="iconSelect" class="col-sm-2 control-label">{% translate "Select Doctrine Icon" %}</label>
+                                <div class="col-sm-10">
+                                    <select class="form-control" name="iconSelect" id="iconSelect" aria-describedby="helpBlock">
+                                        {% for ship in ships %}
+                                            <option value="{{ ship.ship_type|type_render_url:64 }}">{{ship.ship_type__name}}</option>
+                                        {% endfor %}
+                                    </select>
+                                    <span id="helpBlock" class="help-block"> {% translate "If you do not see the ship type that you would like to use for the icon, add a fit that uses that ship type and try again." %}</span>
                                 </div>
                             </div>
                             <br />
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
             </div>
         </div>
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/slim-select/1.26.0/slimselect.min.js"></script>
+    {% include 'fittings/bundles/multi-select-js.html' %}
+    {% include 'fittings/bundles/jquery.quicksearch-js.html' %}
 {% endblock %}
 
-
 {% block extra_script %}
-var color_picker = document.getElementById("color");
-var color_picker_wrapper = document.getElementById("color-wrapper");
-color_picker.onchange = function() {
-	color_picker_wrapper.style.backgroundColor = color_picker.value;
-}
-color_picker_wrapper.style.backgroundColor = color_picker.value;
-
-new SlimSelect({
-    select: "#groupSelect",
-    hideSelectedOption: true,
-    placeholder: '{% translate "Select Value" %}',
-    searchText: '{% translate "No Results" %}',
-    searchPlaceholder: '{% translate "Search" %}'
-});
-
-new SlimSelect({
-    select: "#fitSelect",
-    hideSelectedOption: true,
-    placeholder: '{% translate "Select Value" %}',
-    searchText: '{% translate "No Results" %}',
-    searchPlaceholder: '{% translate "Search" %}'
-});
-
-new SlimSelect({
-    select: "#docSelect",
-    hideSelectedOption: true,
-    placeholder: '{% translate "Select Value" %}',
-    searchText: '{% translate "No Results" %}',
-    searchPlaceholder: '{% translate "Search" %}'
-});
-
+    $('#fitSelect').multiSelect({
+          selectableHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='{% translate "Search" %}' style='margin-bottom: 3px;'>",
+          selectionHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='{% translate "Search" %}' style='margin-bottom: 3px;'>",
+          afterInit: function(ms){
+            var that = this,
+                $selectableSearch = that.$selectableUl.prev(),
+                $selectionSearch = that.$selectionUl.prev(),
+                selectableSearchString = '#'+that.$container.attr('id')+' .ms-elem-selectable:not(.ms-selected)',
+                selectionSearchString = '#'+that.$container.attr('id')+' .ms-elem-selection.ms-selected';
+
+            that.qs1 = $selectableSearch.quicksearch(selectableSearchString)
+            .on('keydown', function(e){
+              if (e.which === 40){
+                that.$selectableUl.focus();
+                return false;
+              }
+            });
+
+            that.qs2 = $selectionSearch.quicksearch(selectionSearchString)
+            .on('keydown', function(e){
+              if (e.which == 40){
+                that.$selectionUl.focus();
+                return false;
+              }
+            });
+          },
+          afterSelect: function(){
+            this.qs1.cache();
+            this.qs2.cache();
+          },
+          afterDeselect: function(){
+            this.qs1.cache();
+            this.qs2.cache();
+          }
+        })
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,36 +1,43 @@
 {% extends 'fittings/base.html' %} {% load i18n %} {% load humanize %} {% load
-filters %} {% load static %} {% block more_css %}
-
- {% endblock %} {% block page_title %}{% translate "Add Category" %}{% endblock
-%} {% block fittings_block %}
-{% translate "New Category" %}
+filters %} {% load static %} {% load evelinks %} {% block more_css %}
+ {% endblock %} {% block page_title %}{% translate "Add Doctrine" %}{% endblock
+%} {% block fittings_block %} {% if msg %}
+ ×  {% if msg.0 != 'warning' %}
+*** {% if msg.0 == 'danger' %}Oh No!{% elif msg.0 == 'success' %}Success!{%
+endif %} ***
+{% endif %}
+{{ msg.1 }}
+{% endif %}
+{% translate "New Doctrine" %}
 {% csrf_token %}
-{% translate "Category Name" %} [name                ]
-{% translate "Category Color" %}
-[Unknown INPUT type]
-{% for group in groups %}
-{{group.name}}
-{% endfor %}
-{% for fit in fits %}
-{{fit.name}}
+{% translate "Doctrine Name" %}
+[name                ]
+{% translate "Doctrine Description" %}
+{% translate "Select Fits" %}
+{% for fit in fittings %}
+{{ fit.name }} ({{fit.ship_type.name}})
 {% endfor %}
-{% for doc in docs %}
-{{doc.name}}
+{% translate "Select Doctrine Icon" %}
+{% for ship in ships %}
+{{ship.ship_type__name}}
 {% endfor %}
+  {% translate "If you do not see the ship type that you would like to use for
+the icon, add a fit that uses that ship type and try again." %}
 
 {% translate "Submit" %}
-{% endblock %} {% block extra_javascript %}
- {% endblock %} {% block extra_script %} var color_picker =
-document.getElementById("color"); var color_picker_wrapper =
-document.getElementById("color-wrapper"); color_picker.onchange = function()
-{ color_picker_wrapper.style.backgroundColor = color_picker.value; }
-color_picker_wrapper.style.backgroundColor = color_picker.value; new SlimSelect
-({ select: "#groupSelect", hideSelectedOption: true, placeholder: '{% translate
-"Select Value" %}', searchText: '{% translate "No Results" %}',
-searchPlaceholder: '{% translate "Search" %}' }); new SlimSelect({ select:
-"#fitSelect", hideSelectedOption: true, placeholder: '{% translate "Select
-Value" %}', searchText: '{% translate "No Results" %}', searchPlaceholder: '{%
-translate "Search" %}' }); new SlimSelect({ select: "#docSelect",
-hideSelectedOption: true, placeholder: '{% translate "Select Value" %}',
-searchText: '{% translate "No Results" %}', searchPlaceholder: '{% translate
-"Search" %}' }); {% endblock %}
+{% endblock %} {% block extra_javascript %} {% include 'fittings/bundles/multi-
+select-js.html' %} {% include 'fittings/bundles/jquery.quicksearch-js.html' %}
+{% endblock %} {% block extra_script %} $('#fitSelect').multiSelect(
+{ selectableHeader: "[                    ]", selectionHeader: "
+[                    ]", afterInit: function(ms){ var that = this,
+$selectableSearch = that.$selectableUl.prev(), $selectionSearch =
+that.$selectionUl.prev(), selectableSearchString = '#'+that.$container.attr
+('id')+' .ms-elem-selectable:not(.ms-selected)', selectionSearchString =
+'#'+that.$container.attr('id')+' .ms-elem-selection.ms-selected'; that.qs1 =
+$selectableSearch.quicksearch(selectableSearchString) .on('keydown', function
+(e){ if (e.which === 40){ that.$selectableUl.focus(); return false; } });
+that.qs2 = $selectionSearch.quicksearch(selectionSearchString) .on('keydown',
+function(e){ if (e.which == 40){ that.$selectionUl.focus(); return false; } });
+}, afterSelect: function(){ this.qs1.cache(); this.qs2.cache(); },
+afterDeselect: function(){ this.qs1.cache(); this.qs2.cache(); } }) {% endblock
+%}
```

### Comparing `fittings-2.0.0/fittings/management/commands/fittings_preload_data.py` & `fittings-2.0.1/fittings/management/commands/fittings_preload_data.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/7m.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/7m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/4m.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/4m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/0l.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/0l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/5l.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/5l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/h.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/6m.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/6m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/5s.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/5s.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/r.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/3h.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/3h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/2h.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/2h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/circle.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/circle.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/l.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/3r.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/3r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/m.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/2m.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/2m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/0r.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/0r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/3m.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/3m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/0m.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/0m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/0s.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/0s.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/5h.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/5h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/4l.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/4l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/dustwheel.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/dustwheel.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/8l.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/8l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/0h.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/0h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/4s.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/4s.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/5m.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/5m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_default.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_default.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_blue.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_blue.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/working.jpg` & `fittings-2.0.1/fittings/static/fittings/img/pannel/working.jpg`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/7l.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/7l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/1r.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/1r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/noship.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/noship.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/1l.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/1l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/4h.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/4h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/7h.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/7h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/3l.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/3l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/6h.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/6h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/1h.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/1h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/1m.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/1m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_revelations.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_revelations.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/2l.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/2l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/2r.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/2r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/6l.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/6l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/error.jpg` & `fittings-2.0.1/fittings/static/fittings/img/pannel/error.jpg`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_darkred.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_darkred.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/8m.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/8m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/static/fittings/img/pannel/8h.png` & `fittings-2.0.1/fittings/static/fittings/img/pannel/8h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/models.py` & `fittings-2.0.1/fittings/models.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/admin.py` & `fittings-2.0.1/fittings/admin.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/views.py` & `fittings-2.0.1/fittings/views.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/migrations/0005_unicategory.py` & `fittings-2.0.1/fittings/migrations/0005_unicategory.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py` & `fittings-2.0.1/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py` & `fittings-2.0.1/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/migrations/0014_serverversion.py` & `fittings-2.0.1/fittings/migrations/0014_serverversion.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/migrations/0001_initial.py` & `fittings-2.0.1/fittings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/migrations/0011_auto_20200815_2022.py` & `fittings-2.0.1/fittings/migrations/0011_auto_20200815_2022.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/migrations/0012_typehistory.py` & `fittings-2.0.1/fittings/migrations/0012_typehistory.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/migrations/0007_auto_20200605_0735.py` & `fittings-2.0.1/fittings/migrations/0007_auto_20200605_0735.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/migrations/0004_add_item_category_and_group.py` & `fittings-2.0.1/fittings/migrations/0004_add_item_category_and_group.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/migrations/0009_auto_20200605_2117.py` & `fittings-2.0.1/fittings/migrations/0009_auto_20200605_2117.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/migrations/0002_add_dgm_unique_constraints.py` & `fittings-2.0.1/fittings/migrations/0002_add_dgm_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/locale/zh_Hans/LC_MESSAGES/django.po` & `fittings-2.0.1/fittings/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/locale/ru/LC_MESSAGES/django.mo` & `fittings-2.0.1/fittings/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/locale/ru/LC_MESSAGES/django.po` & `fittings-2.0.1/fittings/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/locale/es/LC_MESSAGES/django.po` & `fittings-2.0.1/fittings/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/locale/fr_FR/LC_MESSAGES/django.po` & `fittings-2.0.1/fittings/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/locale/ja/LC_MESSAGES/django.mo` & `fittings-2.0.1/fittings/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/locale/ja/LC_MESSAGES/django.po` & `fittings-2.0.1/fittings/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/locale/de/LC_MESSAGES/django.mo` & `fittings-2.0.1/fittings/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/locale/de/LC_MESSAGES/django.po` & `fittings-2.0.1/fittings/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/locale/ko_KR/LC_MESSAGES/django.mo` & `fittings-2.0.1/fittings/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/locale/ko_KR/LC_MESSAGES/django.po` & `fittings-2.0.1/fittings/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings/templatetags/filters.py` & `fittings-2.0.1/fittings/templatetags/filters.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.template.defaulttags import register
-from django.utils.safestring import mark_safe
 
 
 @register.filter()
 def get_item(dict_, key):
     return dict_.get(key)
 
+
 @register.filter(name='empty_slots')
 def empty_slots(fittings: dict, slot_type: str):
     keys = fittings.keys()
 
     for key in keys:
         if slot_type in key:
             # This slot type is not empty
@@ -17,8 +17,7 @@
     # This slot type is completely empty
     return True
 
 
 @register.filter
 def break_html_lines(value):
     return value.replace("<br>", "\n").replace("<br />", "\n")
-
```

### Comparing `fittings-2.0.0/fittings/urls.py` & `fittings-2.0.1/fittings/urls.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/setup.py` & `fittings-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.0/fittings.egg-info/PKG-INFO` & `fittings-2.0.1/fittings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fittings
-Version: 2.0.0
+Version: 2.0.1
 Summary: A simple fittings and doctrine management application.
 Home-page: https://gitlab.com/colcrunch/fittings
 Author: Col Crunch
 Author-email: it-team@serin.space
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `fittings-2.0.0/fittings.egg-info/SOURCES.txt` & `fittings-2.0.1/fittings.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -50,14 +50,30 @@
 fittings/migrations/0011_auto_20200815_2022.py
 fittings/migrations/0012_typehistory.py
 fittings/migrations/0013_alter_doctrine_description.py
 fittings/migrations/0014_serverversion.py
 fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py
 fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py
 fittings/migrations/__init__.py
+fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/clipboard.min.js
+fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/jquery,quicksearch.min.js
+fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/multi-select.min.css
+fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/jquery.multi-select.js
+fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.css
+fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.js
+fittings/static/fittings/dt-i18n/de-DE.json
+fittings/static/fittings/dt-i18n/en-GB.json
+fittings/static/fittings/dt-i18n/es-ES.json
+fittings/static/fittings/dt-i18n/fr-FR.json
+fittings/static/fittings/dt-i18n/it-IT.json
+fittings/static/fittings/dt-i18n/ja.json
+fittings/static/fittings/dt-i18n/ko.json
+fittings/static/fittings/dt-i18n/ru.json
+fittings/static/fittings/dt-i18n/uk.json
+fittings/static/fittings/dt-i18n/zh.json
 fittings/static/fittings/img/pannel/0h.png
 fittings/static/fittings/img/pannel/0l.png
 fittings/static/fittings/img/pannel/0m.png
 fittings/static/fittings/img/pannel/0r.png
 fittings/static/fittings/img/pannel/0s.png
 fittings/static/fittings/img/pannel/1h.png
 fittings/static/fittings/img/pannel/1l.png
@@ -112,9 +128,16 @@
 fittings/templates/fittings/edit_doctrine.html
 fittings/templates/fittings/edit_fit.html
 fittings/templates/fittings/view_all_categories.html
 fittings/templates/fittings/view_all_fits.html
 fittings/templates/fittings/view_category.html
 fittings/templates/fittings/view_doctrine.html
 fittings/templates/fittings/view_fit.html
+fittings/templates/fittings/bundles/clipboard-js.html
+fittings/templates/fittings/bundles/jquery.quicksearch-js.html
+fittings/templates/fittings/bundles/multi-select-css.html
+fittings/templates/fittings/bundles/multi-select-js.html
+fittings/templates/fittings/bundles/slim-select-css.html
+fittings/templates/fittings/bundles/slim-select-js.html
 fittings/templatetags/__init__.py
-fittings/templatetags/filters.py
+fittings/templatetags/filters.py
+fittings/templatetags/tags.py
```

### Comparing `fittings-2.0.0/README.md` & `fittings-2.0.1/README.md`

 * *Files identical despite different names*

