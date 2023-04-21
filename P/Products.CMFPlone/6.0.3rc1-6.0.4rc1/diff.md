# Comparing `tmp/Products.CMFPlone-6.0.3rc1.tar.gz` & `tmp/Products.CMFPlone-6.0.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.CMFPlone-6.0.3rc1.tar", last modified: Thu Mar 23 12:26:37 2023, max compression
+gzip compressed data, was "Products.CMFPlone-6.0.4rc1.tar", last modified: Fri Apr 21 14:51:45 2023, max compression
```

## Comparing `Products.CMFPlone-6.0.3rc1.tar` & `Products.CMFPlone-6.0.4rc1.tar`

### file list

```diff
@@ -1,653 +1,654 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.358169 Products.CMFPlone-6.0.3rc1/
--rw-r--r--   0 maurits    (501) staff       (20)      575 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)    23961 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/CHANGES.md
--rw-r--r--   0 maurits    (501) staff       (20)       95 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/CONTRIBUTING.md
--rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/LICENSE
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    31923 2023-03-23 12:26:37.358571 Products.CMFPlone-6.0.3rc1/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.182433 Products.CMFPlone-6.0.3rc1/Products/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.197664 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/
--rw-r--r--   0 maurits    (501) staff       (20)     4684 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/ActionsTool.py
--rw-r--r--   0 maurits    (501) staff       (20)    18328 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/CatalogTool.py
--rw-r--r--   0 maurits    (501) staff       (20)    13993 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/MigrationTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     8096 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/PasswordResetTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     4535 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/PloneBaseTool.py
--rw-r--r--   0 maurits    (501) staff       (20)       78 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/PloneBatch.py
--rw-r--r--   0 maurits    (501) staff       (20)    10947 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/PloneControlPanel.py
--rw-r--r--   0 maurits    (501) staff       (20)    41550 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/PloneTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     8661 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/Portal.py
--rw-r--r--   0 maurits    (501) staff       (20)     4984 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/PropertiesTool.py
--rw-r--r--   0 maurits    (501) staff       (20)    20097 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/RegistrationTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     1419 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/SkinsTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     6506 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/TranslationServiceTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     3302 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/TypesTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     1777 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/URLTool.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.198539 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/UnicodeSplitter/
--rw-r--r--   0 maurits    (501) staff       (20)       93 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/UnicodeSplitter/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1734 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/UnicodeSplitter/config.py
--rw-r--r--   0 maurits    (501) staff       (20)     6624 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/UnicodeSplitter/splitter.py
--rw-r--r--   0 maurits    (501) staff       (20)    15127 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/WorkflowTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     6979 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      188 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/bbb.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.205236 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/
--rw-r--r--   0 maurits    (501) staff       (20)       18 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    13074 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/admin.py
--rw-r--r--   0 maurits    (501) staff       (20)     1840 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/admin.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1752 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/atd.py
--rw-r--r--   0 maurits    (501) staff       (20)     7834 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/author.py
--rw-r--r--   0 maurits    (501) staff       (20)      342 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/caching.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     7400 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3350 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/contact_info.py
--rw-r--r--   0 maurits    (501) staff       (20)      523 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/defaultpage.py
--rw-r--r--   0 maurits    (501) staff       (20)     2063 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/exceptions.py
--rw-r--r--   0 maurits    (501) staff       (20)     1802 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/favicon.py
--rw-r--r--   0 maurits    (501) staff       (20)      537 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/global_statusmessage.py
--rw-r--r--   0 maurits    (501) staff       (20)     4344 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/icons.py
--rw-r--r--   0 maurits    (501) staff       (20)     9737 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.207604 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4584 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9768 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/login.py
--rw-r--r--   0 maurits    (501) staff       (20)     8055 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/login_help.py
--rw-r--r--   0 maurits    (501) staff       (20)     1966 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/logout.py
--rw-r--r--   0 maurits    (501) staff       (20)      938 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/mail_password.py
--rw-r--r--   0 maurits    (501) staff       (20)    10590 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/password_reset.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.212472 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     2073 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/explainPWResetTool.pt
--rw-r--r--   0 maurits    (501) staff       (20)      895 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/forced_password_change.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1205 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/initial_login_password_change.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/insufficient_privileges.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1488 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/logged_out.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2128 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/login.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2969 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/login_failsafe.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2061 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/login_help.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4018 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/mail_password_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1046 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/mail_password_response.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1693 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/mail_password_template.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1300 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/pwreset_expired.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1023 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/pwreset_finish.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6094 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/pwreset_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1474 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/pwreset_invalid.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1408 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/registered_notify_template.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2098 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/subform_render.pt
--rw-r--r--   0 maurits    (501) staff       (20)      915 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1066 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/main_template.py
--rw-r--r--   0 maurits    (501) staff       (20)     8914 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/navigation.py
--rw-r--r--   0 maurits    (501) staff       (20)     8165 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/navtree.py
--rw-r--r--   0 maurits    (501) staff       (20)     1053 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/okay.py
--rw-r--r--   0 maurits    (501) staff       (20)     8742 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/ploneview.py
--rw-r--r--   0 maurits    (501) staff       (20)      889 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/robots.py
--rw-r--r--   0 maurits    (501) staff       (20)    11633 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/search.py
--rw-r--r--   0 maurits    (501) staff       (20)     3567 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/sendto.py
--rw-r--r--   0 maurits    (501) staff       (20)      920 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/sitelogo.py
--rw-r--r--   0 maurits    (501) staff       (20)     1230 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/sitemap.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.214396 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/
--rw-r--r--   0 maurits    (501) staff       (20)       43 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/blank.html
--rw-r--r--   0 maurits    (501) staff       (20)     5430 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/favicon.ico
--rw-r--r--   0 maurits    (501) staff       (20)     5434 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/jstz-1.0.4.min.js
--rw-r--r--   0 maurits    (501) staff       (20)      187 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/plone-admin-ui.css
--rw-r--r--   0 maurits    (501) staff       (20)      534 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/plone-admin-ui.js
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/plone-logo.png
--rw-r--r--   0 maurits    (501) staff       (20)     3766 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/plone-logo.svg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.216189 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     9117 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/adapters.py
--rw-r--r--   0 maurits    (501) staff       (20)     2664 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2048 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/settings.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.218129 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     2111 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/RSS.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3546 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/atom.xml.pt
--rw-r--r--   0 maurits    (501) staff       (20)      191 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/content_core.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1790 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/itunes.xml.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4620 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/newsml.xml.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1265 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/rss.xml.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2199 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/search-rss.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2912 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/tool.py
--rw-r--r--   0 maurits    (501) staff       (20)     2900 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     3196 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/views.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.227402 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     3749 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/accessibility-info.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4576 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/ajax_main_template.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10729 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/author.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1071 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/author_feedback_template.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1177 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/basic_error_message.pt
--rw-r--r--   0 maurits    (501) staff       (20)      687 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/colophon.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1134 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/contact-info-email.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1725 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/contact-info.pt
--rw-r--r--   0 maurits    (501) staff       (20)      135 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/description.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6441 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/error_message.pt
--rw-r--r--   0 maurits    (501) staff       (20)      344 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/five_template.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1539 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/footer.pt
--rw-r--r--   0 maurits    (501) staff       (20)      454 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/global_statusmessage.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5666 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/main_template.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9235 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/plone-addsite.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1394 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/plone-admin-logged-out.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4827 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/plone-frontpage.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6504 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/plone-overview.pt
--rw-r--r--   0 maurits    (501) staff       (20)     7000 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/plone-upgrade.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4066 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/recently_modified.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4096 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/recently_published.pt
--rw-r--r--   0 maurits    (501) staff       (20)    17995 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/search.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1521 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/sendto_template.pt
--rw-r--r--   0 maurits    (501) staff       (20)      825 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/sitemap-item.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1179 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/sitemap.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3612 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/test_rendering.pt
--rw-r--r--   0 maurits    (501) staff       (20)    90136 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/test_rendering_cheatsheet.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3228 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/test_rendering_icons.pt
--rw-r--r--   0 maurits    (501) staff       (20)      100 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/title.pt
--rw-r--r--   0 maurits    (501) staff       (20)       54 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/toolbar.pt
--rw-r--r--   0 maurits    (501) staff       (20)      973 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/test_rendering.py
--rw-r--r--   0 maurits    (501) staff       (20)     1201 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/catalog.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4530 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.229529 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/
--rw-r--r--   0 maurits    (501) staff       (20)     4867 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.233182 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      849 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1769 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/editing.py
--rw-r--r--   0 maurits    (501) staff       (20)     1439 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/filter.py
--rw-r--r--   0 maurits    (501) staff       (20)     4726 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/language.py
--rw-r--r--   0 maurits    (501) staff       (20)     3231 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/mail.py
--rw-r--r--   0 maurits    (501) staff       (20)      766 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/maintenance.py
--rw-r--r--   0 maurits    (501) staff       (20)      891 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/markup.py
--rw-r--r--   0 maurits    (501) staff       (20)     2522 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/navigation.py
--rw-r--r--   0 maurits    (501) staff       (20)     1446 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/search.py
--rw-r--r--   0 maurits    (501) staff       (20)     2692 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/security.py
--rw-r--r--   0 maurits    (501) staff       (20)     1160 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/site.py
--rw-r--r--   0 maurits    (501) staff       (20)     1327 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/usergroups.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.248967 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3498 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/actions.pt
--rw-r--r--   0 maurits    (501) staff       (20)     7113 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)    10862 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      880 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/controlpanel_usergroups_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)      703 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/dateandtime.py
--rw-r--r--   0 maurits    (501) staff       (20)      654 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/editing.py
--rw-r--r--   0 maurits    (501) staff       (20)     2756 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/emaillogin.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6715 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/error_log_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2187 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/error_log_form.py
--rw-r--r--   0 maurits    (501) staff       (20)     3683 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/error_log_show_entry.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2070 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/filter.py
--rw-r--r--   0 maurits    (501) staff       (20)      687 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/filter_controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)      510 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/imaging.py
--rw-r--r--   0 maurits    (501) staff       (20)     2330 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/language.py
--rw-r--r--   0 maurits    (501) staff       (20)     3837 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/mail.py
--rw-r--r--   0 maurits    (501) staff       (20)     6382 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/maintenance.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5290 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/maintenance.py
--rw-r--r--   0 maurits    (501) staff       (20)      635 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/markup.py
--rw-r--r--   0 maurits    (501) staff       (20)     1114 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/navigation.py
--rw-r--r--   0 maurits    (501) staff       (20)     7477 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/overview.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4690 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/overview.py
--rw-r--r--   0 maurits    (501) staff       (20)     3926 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/prefsmaintemplate.pt
--rw-r--r--   0 maurits    (501) staff       (20)      408 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/prefsmaintemplate.py
--rw-r--r--   0 maurits    (501) staff       (20)    10262 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/quickinstaller.pt
--rw-r--r--   0 maurits    (501) staff       (20)    23365 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/quickinstaller.py
--rw-r--r--   0 maurits    (501) staff       (20)    12623 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/redirects-controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4768 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/redirects-manage.pt
--rw-r--r--   0 maurits    (501) staff       (20)    19982 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/redirects.py
--rw-r--r--   0 maurits    (501) staff       (20)     3683 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/relations.py
--rw-r--r--   0 maurits    (501) staff       (20)     4963 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/relations_inspect.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4683 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/relations_rebuild.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10206 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/resourceregistry.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5612 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/resourceregistry.py
--rw-r--r--   0 maurits    (501) staff       (20)     2092 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/search.py
--rw-r--r--   0 maurits    (501) staff       (20)     4586 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/security.py
--rw-r--r--   0 maurits    (501) staff       (20)      939 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/site.py
--rw-r--r--   0 maurits    (501) staff       (20)      500 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/socialmedia.py
--rw-r--r--   0 maurits    (501) staff       (20)     3879 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/syndication.py
--rw-r--r--   0 maurits    (501) staff       (20)     1667 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/tinymce.py
--rw-r--r--   0 maurits    (501) staff       (20)    14509 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/types.pt
--rw-r--r--   0 maurits    (501) staff       (20)    21314 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/types.py
--rw-r--r--   0 maurits    (501) staff       (20)     5693 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups.py
--rw-r--r--   0 maurits    (501) staff       (20)    11351 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupdetails.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3859 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupdetails.py
--rw-r--r--   0 maurits    (501) staff       (20)    17772 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupmembership.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4324 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupmembership.py
--rw-r--r--   0 maurits    (501) staff       (20)    10602 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupsoverview.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6451 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupsoverview.py
--rw-r--r--   0 maurits    (501) staff       (20)    10094 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_usermembership.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2675 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_usermembership.py
--rw-r--r--   0 maurits    (501) staff       (20)    11225 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_usersoverview.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10376 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_usersoverview.py
--rw-r--r--   0 maurits    (501) staff       (20)      296 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4522 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/events.py
--rw-r--r--   0 maurits    (501) staff       (20)      246 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/events.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1495 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.263927 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1459 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_actions.py
--rw-r--r--   0 maurits    (501) staff       (20)     3561 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_editing_adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)     2177 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_filter_adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)     9454 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_language_adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)     4727 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_mail_adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)     1484 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_maintenance_adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)     1812 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_markup_adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)     4962 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_navigation_adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)     2227 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_search_adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)     4029 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_security_adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)     2088 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_site_adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)     1439 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_usergroups_adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)     4125 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_editing.py
--rw-r--r--   0 maurits    (501) staff       (20)     2608 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_error_log.py
--rw-r--r--   0 maurits    (501) staff       (20)     4109 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_filter.py
--rw-r--r--   0 maurits    (501) staff       (20)     5264 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_installer.py
--rw-r--r--   0 maurits    (501) staff       (20)    11410 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_language.py
--rw-r--r--   0 maurits    (501) staff       (20)     8588 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_mail.py
--rw-r--r--   0 maurits    (501) staff       (20)     3449 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_maintenance.py
--rw-r--r--   0 maurits    (501) staff       (20)     3819 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_markup.py
--rw-r--r--   0 maurits    (501) staff       (20)     6772 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_navigation.py
--rw-r--r--   0 maurits    (501) staff       (20)    37430 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_redirection.py
--rw-r--r--   0 maurits    (501) staff       (20)     2756 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_relations.py
--rw-r--r--   0 maurits    (501) staff       (20)     2844 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_search.py
--rw-r--r--   0 maurits    (501) staff       (20)     3768 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_security.py
--rw-r--r--   0 maurits    (501) staff       (20)     7464 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_site.py
--rw-r--r--   0 maurits    (501) staff       (20)     4075 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_syndication.py
--rw-r--r--   0 maurits    (501) staff       (20)     9137 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_types.py
--rw-r--r--   0 maurits    (501) staff       (20)    18911 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_usergroups.py
--rw-r--r--   0 maurits    (501) staff       (20)    14697 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_usergroups_siteadmin_role.py
--rw-r--r--   0 maurits    (501) staff       (20)     1883 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_dateandtime.py
--rw-r--r--   0 maurits    (501) staff       (20)      724 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_doctest.py
--rw-r--r--   0 maurits    (501) staff       (20)     1742 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_editing.py
--rw-r--r--   0 maurits    (501) staff       (20)     6145 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_events.py
--rw-r--r--   0 maurits    (501) staff       (20)     1677 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_filter.py
--rw-r--r--   0 maurits    (501) staff       (20)    17858 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_installer.py
--rw-r--r--   0 maurits    (501) staff       (20)     2686 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_language.py
--rw-r--r--   0 maurits    (501) staff       (20)     1318 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_mail.py
--rw-r--r--   0 maurits    (501) staff       (20)     1520 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_markup.py
--rw-r--r--   0 maurits    (501) staff       (20)     2021 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_navigation.py
--rw-r--r--   0 maurits    (501) staff       (20)     2632 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_overview.py
--rw-r--r--   0 maurits    (501) staff       (20)     6834 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_relations.py
--rw-r--r--   0 maurits    (501) staff       (20)     1556 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_search.py
--rw-r--r--   0 maurits    (501) staff       (20)     2132 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_security.py
--rw-r--r--   0 maurits    (501) staff       (20)     1770 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_site.py
--rw-r--r--   0 maurits    (501) staff       (20)     1230 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_types.py
--rw-r--r--   0 maurits    (501) staff       (20)     1656 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_usergroups.py
--rw-r--r--   0 maurits    (501) staff       (20)      884 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     1221 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_upgrades1.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1778 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_upgrades2.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1729 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      972 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/widgets.py
--rw-r--r--   0 maurits    (501) staff       (20)       84 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/defaultpage.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.264448 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/earlypatches/
--rw-r--r--   0 maurits    (501) staff       (20)       82 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/earlypatches/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2524 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/earlypatches/security.py
--rw-r--r--   0 maurits    (501) staff       (20)     1186 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/events.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.265917 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)       27 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5366 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6325 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     1298 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/memberdata_properties.py
--rw-r--r--   0 maurits    (501) staff       (20)     4807 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/propertiestool.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.266993 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       33 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      374 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     2106 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/tests/testControlPanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     3376 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/tests/testPropertiesTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     7351 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/factory.py
--rw-r--r--   0 maurits    (501) staff       (20)       81 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/i18nl10n.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.268005 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/image_scales/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/image_scales/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1168 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/image_scales/adapters.py
--rw-r--r--   0 maurits    (501) staff       (20)      290 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/image_scales/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      765 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/image_scales/indexer.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.268762 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/image_scales/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/image_scales/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      419 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/image_scales/tests/images.xml
--rw-r--r--   0 maurits    (501) staff       (20)     6078 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/image_scales/tests/test_image_scales_metadata.py
--rw-r--r--   0 maurits    (501) staff       (20)      199 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/index.gif
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.274690 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/
--rw-r--r--   0 maurits    (501) staff       (20)     4678 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       87 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/atd.py
--rw-r--r--   0 maurits    (501) staff       (20)       92 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/basetool.py
--rw-r--r--   0 maurits    (501) staff       (20)       95 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/breadcrumbs.py
--rw-r--r--   0 maurits    (501) staff       (20)       94 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/constrains.py
--rw-r--r--   0 maurits    (501) staff       (20)       96 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)       95 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/defaultpage.py
--rw-r--r--   0 maurits    (501) staff       (20)       90 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/events.py
--rw-r--r--   0 maurits    (501) staff       (20)       95 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/installable.py
--rw-r--r--   0 maurits    (501) staff       (20)       93 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/interface.py
--rw-r--r--   0 maurits    (501) staff       (20)       92 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/language.py
--rw-r--r--   0 maurits    (501) staff       (20)       89 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/login.py
--rw-r--r--   0 maurits    (501) staff       (20)       93 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/migration.py
--rw-r--r--   0 maurits    (501) staff       (20)       98 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/password_reset.py
--rw-r--r--   0 maurits    (501) staff       (20)       92 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/patterns.py
--rw-r--r--   0 maurits    (501) staff       (20)       94 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/properties.py
--rw-r--r--   0 maurits    (501) staff       (20)       93 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/resources.py
--rw-r--r--   0 maurits    (501) staff       (20)       92 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/siteroot.py
--rw-r--r--   0 maurits    (501) staff       (20)       93 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/structure.py
--rw-r--r--   0 maurits    (501) staff       (20)       95 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/syndication.py
--rw-r--r--   0 maurits    (501) staff       (20)      102 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/translationservice.py
--rw-r--r--   0 maurits    (501) staff       (20)      165 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)      869 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/log.py
--rw-r--r--   0 maurits    (501) staff       (20)     1608 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1038 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/overrides.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.279001 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/
--rw-r--r--   0 maurits    (501) staff       (20)      944 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1501 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/addzmiplonesite.py
--rw-r--r--   0 maurits    (501) staff       (20)      863 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/addzmisecuritywarning.py
--rw-r--r--   0 maurits    (501) staff       (20)     1781 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)      796 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/dateIndexPatch.py
--rw-r--r--   0 maurits    (501) staff       (20)     2596 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/gtbn.py
--rw-r--r--   0 maurits    (501) staff       (20)      653 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/iso8601.py
--rw-r--r--   0 maurits    (501) staff       (20)     1510 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/publishing.py
--rw-r--r--   0 maurits    (501) staff       (20)      244 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/security.py
--rw-r--r--   0 maurits    (501) staff       (20)     1660 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/sendmail.py
--rw-r--r--   0 maurits    (501) staff       (20)     1075 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/speed.py
--rw-r--r--   0 maurits    (501) staff       (20)      952 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/templatecookcheck.py
--rw-r--r--   0 maurits    (501) staff       (20)     1855 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/unicodeFallbackPatch.py
--rw-r--r--   0 maurits    (501) staff       (20)     1031 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/unicodehacks.py
--rw-r--r--   0 maurits    (501) staff       (20)     2551 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/z3c_form.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.280514 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patterns/
--rw-r--r--   0 maurits    (501) staff       (20)      405 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patterns/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      722 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patterns/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6678 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patterns/settings.py
--rw-r--r--   0 maurits    (501) staff       (20)     8916 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patterns/tinymce.py
--rw-r--r--   0 maurits    (501) staff       (20)      799 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patterns/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1618 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patterns/view.py
--rw-r--r--   0 maurits    (501) staff       (20)       84 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/permissions.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.177386 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.284913 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)    16012 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)     5143 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)     3553 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/componentregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2629 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/contenttyperegistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     9540 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      125 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/mailhost.xml
--rw-r--r--   0 maurits    (501) staff       (20)      961 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/memberdata_properties.xml
--rw-r--r--   0 maurits    (501) staff       (20)       71 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      119 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/properties.xml
--rw-r--r--   0 maurits    (501) staff       (20)      376 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/propertiestool.xml
--rw-r--r--   0 maurits    (501) staff       (20)    10601 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/rolemap.xml
--rw-r--r--   0 maurits    (501) staff       (20)      781 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/skins.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2838 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/toolset.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.285694 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     1460 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/types/Discussion_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2782 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/types/Plone_Site.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1366 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/types/TempFolder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      386 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1746 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/viewlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.177043 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.285965 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/folder_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     7684 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/folder_workflow/definition.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.286235 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/intranet_folder_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     6170 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/intranet_folder_workflow/definition.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.286500 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/intranet_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)    13766 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/intranet_workflow/definition.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.286786 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/one_state_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     3117 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/one_state_workflow/definition.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.287063 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/plone_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)    10574 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/plone_workflow/definition.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.287335 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/simple_publication_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     8772 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/simple_publication_workflow/definition.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.288174 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/dependencies/
--rw-r--r--   0 maurits    (501) staff       (20)     1049 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/dependencies/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     4765 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/dependencies/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)     4738 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/dependencies/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.288965 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/testfixture/
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/testfixture/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/testfixture/plone-update-workflow-rolemap.txt
--rw-r--r--   0 maurits    (501) staff       (20)      369 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/testfixture/workflows.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1147 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    11709 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/relationhelper.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.290449 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/
--rw-r--r--   0 maurits    (501) staff       (20)     1109 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.291695 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      346 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/browser/combine.py
--rw-r--r--   0 maurits    (501) staff       (20)      846 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    12200 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/browser/resource.py
--rw-r--r--   0 maurits    (501) staff       (20)      139 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4539 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2707 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/webresource.py
--rw-r--r--   0 maurits    (501) staff       (20)     8829 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/setuphandlers.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.178342 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.307187 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/
--rw-r--r--   0 maurits    (501) staff       (20)      114 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowBottom.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowBottom.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      112 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowDown.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowDown.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      109 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowLeft.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowLeft.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      117 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowLeftmost.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowLeftmost.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      108 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowRight.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowRight.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      117 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowRightmost.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowRightmost.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      114 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowTop.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowTop.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      112 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowUp.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/arrowUp.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      313 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/book_icon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/book_icon.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      367 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/confirm_icon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/confirm_icon.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      859 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/defaultUser.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/defaultUser.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/document_icon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/document_icon.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      455 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/group.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/group.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      675 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/info_icon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/info_icon.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      338 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/link_icon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/link_icon.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      278 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/lock_icon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/lock_icon.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)     1338 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/logo.png
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/logo.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      226 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/logoIcon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/logoIcon.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)     1097 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/pb_close.png
--rw-r--r--   0 maurits    (501) staff       (20)      226 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/pencil_icon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/pencil_icon.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      410 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/product_icon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/product_icon.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      608 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/rss.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/rss.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      226 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/site_icon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/site_icon.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      663 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/skins_icon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/skins_icon.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      223 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/topic_icon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/topic_icon.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      359 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/user.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/user.png.metadata
--rw-r--r--   0 maurits    (501) staff       (20)      228 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/workflow_icon.png
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/workflow_icon.png.metadata
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.310386 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/
--rw-r--r--   0 maurits    (501) staff       (20)      271 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/browserDefault.py
--rw-r--r--   0 maurits    (501) staff       (20)     1088 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/externalEditorEnabled.py
--rw-r--r--   0 maurits    (501) staff       (20)      786 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/external_edit.py
--rw-r--r--   0 maurits    (501) staff       (20)     1671 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/getFolderContents.py
--rw-r--r--   0 maurits    (501) staff       (20)      425 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/pretty_title_or_id.py
--rw-r--r--   0 maurits    (501) staff       (20)     3634 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/queryCatalog.py
--rw-r--r--   0 maurits    (501) staff       (20)      473 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/toLocalizedTime.py
--rw-r--r--   0 maurits    (501) staff       (20)     1095 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/translate.py
--rw-r--r--   0 maurits    (501) staff       (20)     2281 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/unique.py
--rw-r--r--   0 maurits    (501) staff       (20)     1119 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/utranslate.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.310660 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_wysiwyg/
--rw-r--r--   0 maurits    (501) staff       (20)     1999 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_wysiwyg/wysiwyg_support.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3899 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.340775 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/
--rw-r--r--   0 maurits    (501) staff       (20)   160651 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/900.jpg
--rw-r--r--   0 maurits    (501) staff       (20)     7089 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/AddMoveAndDeleteDocument.txt
--rw-r--r--   0 maurits    (501) staff       (20)     7127 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/LoginAndLogout.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1479 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/PloneTestCase.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       84 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/accesscontrol_direct.pt
--rw-r--r--   0 maurits    (501) staff       (20)      107 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/accesscontrol_sm.pt
--rw-r--r--   0 maurits    (501) staff       (20)      170 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/accesscontrol_via_dict.pt
--rw-r--r--   0 maurits    (501) staff       (20)       99 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/accesscontrol_via_modules.pt
--rw-r--r--   0 maurits    (501) staff       (20)      104 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/bad1.pt
--rw-r--r--   0 maurits    (501) staff       (20)      104 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/bad2.pt
--rw-r--r--   0 maurits    (501) staff       (20)      247 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/bad3.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1119 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/base_tag_not_present.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2669 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/browser.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4785 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/browser_collection_views.txt
--rw-r--r--   0 maurits    (501) staff       (20)      299 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    17940 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/csrf.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4937 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/dummy.py
--rw-r--r--   0 maurits    (501) staff       (20)    10571 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/emaillogin.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3583 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/link_redirect_view.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2317 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/mails.txt
--rw-r--r--   0 maurits    (501) staff       (20)      105 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/normal_zope3_page_template.pt
--rw-r--r--   0 maurits    (501) staff       (20)       49 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/options_authenticator.pt
--rw-r--r--   0 maurits    (501) staff       (20)       35 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/options_name.pt
--rw-r--r--   0 maurits    (501) staff       (20)       36 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/options_underscore.pt
--rw-r--r--   0 maurits    (501) staff       (20)       43 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/options_view_name.pt
--rw-r--r--   0 maurits    (501) staff       (20)    20500 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/pwreset_browser.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.349761 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2197 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/common.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1318 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/keywords.robot
--rw-r--r--   0 maurits    (501) staff       (20)       69 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/pixel.png
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/plone-logo.png
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.353291 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/
--rw-r--r--   0 maurits    (501) staff       (20)     3617 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      417 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/TODO.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2799 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/anonymous.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1125 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/collaboration-advanced_control.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2515 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/collaboration.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1705 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/common.robot
--rw-r--r--   0 maurits    (501) staff       (20)     6188 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/config-screens.robot
--rw-r--r--   0 maurits    (501) staff       (20)     9471 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/content.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3889 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/managing-working_copy.robot
--rw-r--r--   0 maurits    (501) staff       (20)     6372 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/managing_content.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1148 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/personalsettings.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2187 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/working_with_tinymce.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1177 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robot_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     5850 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_actionmenu.robot
--rw-r--r--   0 maurits    (501) staff       (20)     4658 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_actions.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3955 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_editing.robot
--rw-r--r--   0 maurits    (501) staff       (20)     6628 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_filter.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1633 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_language.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3627 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_markup.robot
--rw-r--r--   0 maurits    (501) staff       (20)     4571 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_navigation.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3491 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_redirection.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2935 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_search.robot
--rw-r--r--   0 maurits    (501) staff       (20)     6960 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_security.robot
--rw-r--r--   0 maurits    (501) staff       (20)     4630 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_site.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2742 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_social.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2770 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_types.robot
--rw-r--r--   0 maurits    (501) staff       (20)     4184 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_usergroups.robot
--rw-r--r--   0 maurits    (501) staff       (20)     6053 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_edit.robot
--rw-r--r--   0 maurits    (501) staff       (20)     7606 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_edit_user_schema.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3973 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_folder_contents.robot
--rw-r--r--   0 maurits    (501) staff       (20)     6135 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_linkintegrity.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3055 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_livesearch.robot
--rw-r--r--   0 maurits    (501) staff       (20)    12377 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_overlays.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2569 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_portlets.robot
--rw-r--r--   0 maurits    (501) staff       (20)    14599 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_querystring.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3075 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_tinymce.robot
--rw-r--r--   0 maurits    (501) staff       (20)       81 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/variables.py
--rw-r--r--   0 maurits    (501) staff       (20)      542 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/scripts.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1492 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/search_form.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5069 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testActionsTool.py
--rw-r--r--   0 maurits    (501) staff       (20)      852 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testBatch.py
--rw-r--r--   0 maurits    (501) staff       (20)     1367 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testBrowserAdmin.py
--rw-r--r--   0 maurits    (501) staff       (20)    15829 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testBrowserDefault.py
--rw-r--r--   0 maurits    (501) staff       (20)     1329 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testBrowserLayerPrecedence.py
--rw-r--r--   0 maurits    (501) staff       (20)     3475 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testCSRFProtection.py
--rw-r--r--   0 maurits    (501) staff       (20)    56012 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testCatalogTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     8225 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testCheckId.py
--rw-r--r--   0 maurits    (501) staff       (20)     8355 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testContentSecurity.py
--rw-r--r--   0 maurits    (501) staff       (20)     5130 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testContentTypeScripts.py
--rw-r--r--   0 maurits    (501) staff       (20)     1269 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testControlPanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     1072 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testControlPanelScripts.py
--rw-r--r--   0 maurits    (501) staff       (20)     2321 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testCookieAuth.py
--rw-r--r--   0 maurits    (501) staff       (20)     8154 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testCutPasteSecurity.py
--rw-r--r--   0 maurits    (501) staff       (20)      925 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testDateIndexRanges.py
--rw-r--r--   0 maurits    (501) staff       (20)     2432 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testDateTimeIntegration.py
--rw-r--r--   0 maurits    (501) staff       (20)     5726 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testEmailLogin.py
--rw-r--r--   0 maurits    (501) staff       (20)     3248 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testExternalEditorEnabled.py
--rw-r--r--   0 maurits    (501) staff       (20)      829 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testIImagingSchema.py
--rw-r--r--   0 maurits    (501) staff       (20)    12541 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testInterfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    10770 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testMigrationTool.py
--rw-r--r--   0 maurits    (501) staff       (20)    28213 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testNavTree.py
--rw-r--r--   0 maurits    (501) staff       (20)    19832 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testNavigationView.py
--rw-r--r--   0 maurits    (501) staff       (20)     4383 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testNextPrevious.py
--rw-r--r--   0 maurits    (501) staff       (20)     9801 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testOrderSupport.py
--rw-r--r--   0 maurits    (501) staff       (20)     1462 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testPloneTestCase.py
--rw-r--r--   0 maurits    (501) staff       (20)    26401 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testPloneTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     8765 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testPloneView.py
--rw-r--r--   0 maurits    (501) staff       (20)    40324 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testPortalCreation.py
--rw-r--r--   0 maurits    (501) staff       (20)    11130 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testQueryCatalog.py
--rw-r--r--   0 maurits    (501) staff       (20)    14244 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testRegistrationTool.py
--rw-r--r--   0 maurits    (501) staff       (20)    18000 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testResourceRegistries.py
--rw-r--r--   0 maurits    (501) staff       (20)     1773 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testRestrictedAcquisition.py
--rw-r--r--   0 maurits    (501) staff       (20)    14341 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testSearch.py
--rw-r--r--   0 maurits    (501) staff       (20)    10136 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testSecurity.py
--rw-r--r--   0 maurits    (501) staff       (20)    15250 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testSecurityDeclarations.py
--rw-r--r--   0 maurits    (501) staff       (20)    12813 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testSiteAdminRole.py
--rw-r--r--   0 maurits    (501) staff       (20)    14071 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testSyndication.py
--rw-r--r--   0 maurits    (501) staff       (20)     2705 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testTranslationServiceTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     7327 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testURLTool.py
--rw-r--r--   0 maurits    (501) staff       (20)    14556 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testUnicodeSplitter.py
--rw-r--r--   0 maurits    (501) staff       (20)     5405 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testUserFolderBasics.py
--rw-r--r--   0 maurits    (501) staff       (20)    20154 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testWebDAV.py
--rw-r--r--   0 maurits    (501) staff       (20)     6235 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testWorkflowTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     5823 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_PloneTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     4807 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_defaultpage.py
--rw-r--r--   0 maurits    (501) staff       (20)      309 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     2618 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_error_message.py
--rw-r--r--   0 maurits    (501) staff       (20)    12186 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_expressions.py
--rw-r--r--   0 maurits    (501) staff       (20)     2833 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_factory.py
--rw-r--r--   0 maurits    (501) staff       (20)     2448 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     2470 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_icons.py
--rw-r--r--   0 maurits    (501) staff       (20)     7976 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_login_form.py
--rw-r--r--   0 maurits    (501) staff       (20)     8259 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_login_help.py
--rw-r--r--   0 maurits    (501) staff       (20)     3905 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_login_logout.py
--rw-r--r--   0 maurits    (501) staff       (20)      714 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_login_views.py
--rw-r--r--   0 maurits    (501) staff       (20)     1870 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_mails.py
--rw-r--r--   0 maurits    (501) staff       (20)     1659 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_nogopip.py
--rw-r--r--   0 maurits    (501) staff       (20)     1949 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_okay.py
--rw-r--r--   0 maurits    (501) staff       (20)      910 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_passwordreset.py
--rw-r--r--   0 maurits    (501) staff       (20)     3703 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_patternsettings.py
--rw-r--r--   0 maurits    (501) staff       (20)    10894 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_redirect_after_login.py
--rw-r--r--   0 maurits    (501) staff       (20)     3484 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_redirection.py
--rw-r--r--   0 maurits    (501) staff       (20)      907 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)      846 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_robots_txt.py
--rw-r--r--   0 maurits    (501) staff       (20)    16875 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_safe_formatter.py
--rw-r--r--   0 maurits    (501) staff       (20)     1582 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_sitelogo.py
--rw-r--r--   0 maurits    (501) staff       (20)     2319 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_sitemap.py
--rw-r--r--   0 maurits    (501) staff       (20)     2417 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     4110 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_z3c_form_widgets.py
--rw-r--r--   0 maurits    (501) staff       (20)     8057 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_zmi.py
--rw-r--r--   0 maurits    (501) staff       (20)      448 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/using_format_zope3_page_template.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2383 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)       35 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/view_name.pt
--rw-r--r--   0 maurits    (501) staff       (20)      168 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tool.gif
--rw-r--r--   0 maurits    (501) staff       (20)     3274 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)      541 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/unicodeconflictresolver.py
--rw-r--r--   0 maurits    (501) staff       (20)    25220 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1953 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/workflow.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.354658 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/www/
--rw-r--r--   0 maurits    (501) staff       (20)      205 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/www/addConfigletForm.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1040 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/www/addPropertySheet.zpt
--rw-r--r--   0 maurits    (501) staff       (20)     4801 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/www/catalogAdvanced.dtml
--rw-r--r--   0 maurits    (501) staff       (20)     6064 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/www/editPloneConfiglets.dtml
--rw-r--r--   0 maurits    (501) staff       (20)     2332 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/CMFPlone/www/zmi_metadata.dtml
--rw-r--r--   0 maurits    (501) staff       (20)      244 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/Products/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.184836 Products.CMFPlone-6.0.3rc1/Products.CMFPlone.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    31923 2023-03-23 12:26:37.000000 Products.CMFPlone-6.0.3rc1/Products.CMFPlone.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    30026 2023-03-23 12:26:37.000000 Products.CMFPlone-6.0.3rc1/Products.CMFPlone.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 12:26:37.000000 Products.CMFPlone-6.0.3rc1/Products.CMFPlone.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2023-03-23 12:26:37.000000 Products.CMFPlone-6.0.3rc1/Products.CMFPlone.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 12:26:37.000000 Products.CMFPlone-6.0.3rc1/Products.CMFPlone.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)     1433 2023-03-23 12:26:37.000000 Products.CMFPlone-6.0.3rc1/Products.CMFPlone.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2023-03-23 12:26:37.000000 Products.CMFPlone-6.0.3rc1/Products.CMFPlone.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     6424 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/README.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:26:37.357942 Products.CMFPlone-6.0.3rc1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     6320 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/docs/CREDITS.txt
--rw-r--r--   0 maurits    (501) staff       (20)   537526 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/docs/HISTORY.rst
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)     2070 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/docs/LICENSE.ZPL
--rw-r--r--   0 maurits    (501) staff       (20)      667 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1460 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/docs/UPGRADE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      308 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/docs/changelog_template.jinja
--rw-r--r--   0 maurits    (501) staff       (20)      503 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      215 2023-03-23 12:26:37.359141 Products.CMFPlone-6.0.3rc1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     4258 2023-03-23 12:26:36.000000 Products.CMFPlone-6.0.3rc1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.695776 Products.CMFPlone-6.0.4rc1/
+-rw-r--r--   0 maurits    (501) staff       (20)      575 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/.gitignore
+-rw-r--r--   0 maurits    (501) staff       (20)    25226 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/CHANGES.md
+-rw-r--r--   0 maurits    (501) staff       (20)       95 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/CONTRIBUTING.md
+-rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/LICENSE
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    33188 2023-04-21 14:51:45.696017 Products.CMFPlone-6.0.4rc1/PKG-INFO
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.492049 Products.CMFPlone-6.0.4rc1/Products/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.507775 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/
+-rw-r--r--   0 maurits    (501) staff       (20)     4684 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/ActionsTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18328 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/CatalogTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13993 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/MigrationTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8096 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/PasswordResetTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4535 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/PloneBaseTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)       78 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/PloneBatch.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10947 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/PloneControlPanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)    41550 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/PloneTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8661 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/Portal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4984 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/PropertiesTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20413 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/RegistrationTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1419 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/SkinsTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6506 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/TranslationServiceTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3302 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/TypesTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1777 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/URLTool.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.508728 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/UnicodeSplitter/
+-rw-r--r--   0 maurits    (501) staff       (20)       93 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/UnicodeSplitter/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1734 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/UnicodeSplitter/config.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6624 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/UnicodeSplitter/splitter.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15127 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/WorkflowTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6979 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      188 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/bbb.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.516225 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)       18 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13074 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/admin.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1840 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/admin.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1752 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/atd.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7834 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/author.py
+-rw-r--r--   0 maurits    (501) staff       (20)      342 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/caching.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     7400 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4310 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/contact_info.py
+-rw-r--r--   0 maurits    (501) staff       (20)      523 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/defaultpage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2063 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/exceptions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1802 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/favicon.py
+-rw-r--r--   0 maurits    (501) staff       (20)      537 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/global_statusmessage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4344 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/icons.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9737 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.518769 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4584 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9768 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/login.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8372 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/login_help.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1966 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/logout.py
+-rw-r--r--   0 maurits    (501) staff       (20)      938 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/mail_password.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10590 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/password_reset.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.525168 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     2073 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/explainPWResetTool.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      895 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/forced_password_change.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1205 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/initial_login_password_change.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/insufficient_privileges.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1488 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/logged_out.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2128 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/login.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2969 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/login_failsafe.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2061 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/login_help.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4018 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/mail_password_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1046 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/mail_password_response.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1693 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/mail_password_template.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1300 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/pwreset_expired.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1023 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/pwreset_finish.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6094 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/pwreset_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1474 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/pwreset_invalid.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1408 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/registered_notify_template.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2098 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/subform_render.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      915 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1066 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/main_template.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8914 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/navigation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8165 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/navtree.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1053 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/okay.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8742 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/ploneview.py
+-rw-r--r--   0 maurits    (501) staff       (20)      889 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/robots.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11770 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/search.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3567 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/sendto.py
+-rw-r--r--   0 maurits    (501) staff       (20)      920 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/sitelogo.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1230 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/sitemap.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.527511 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/
+-rw-r--r--   0 maurits    (501) staff       (20)       43 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/blank.html
+-rw-r--r--   0 maurits    (501) staff       (20)     5430 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/favicon.ico
+-rw-r--r--   0 maurits    (501) staff       (20)     5434 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/jstz-1.0.4.min.js
+-rw-r--r--   0 maurits    (501) staff       (20)      187 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/plone-admin-ui.css
+-rw-r--r--   0 maurits    (501) staff       (20)      534 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/plone-admin-ui.js
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/plone-logo.png
+-rw-r--r--   0 maurits    (501) staff       (20)     3766 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/plone-logo.svg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.529665 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9117 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/adapters.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2664 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2048 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/settings.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.532524 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     2111 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/RSS.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3546 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/atom.xml.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      191 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/content_core.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1790 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/itunes.xml.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4620 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/newsml.xml.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1265 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/rss.xml.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2199 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/search-rss.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2912 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/tool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2900 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3196 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/views.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.542712 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     3749 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/accessibility-info.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4576 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/ajax_main_template.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10729 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/author.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1071 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/author_feedback_template.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1177 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/basic_error_message.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      687 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/colophon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1134 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/contact-info-email.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1725 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/contact-info.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      135 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/description.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6441 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/error_message.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      344 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/five_template.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1539 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/footer.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      454 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/global_statusmessage.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5666 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/main_template.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9235 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/plone-addsite.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1394 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/plone-admin-logged-out.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4827 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/plone-frontpage.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6504 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/plone-overview.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     7000 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/plone-upgrade.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4066 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/recently_modified.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4096 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/recently_published.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    17995 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/search.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1521 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/sendto_template.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      825 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/sitemap-item.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1179 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/sitemap.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3612 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/test_rendering.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    90136 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/test_rendering_cheatsheet.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3228 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/test_rendering_icons.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      100 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/title.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       54 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/toolbar.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      973 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/test_rendering.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1201 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/catalog.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4530 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.545197 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/
+-rw-r--r--   0 maurits    (501) staff       (20)     4867 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.549962 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      849 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1769 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/editing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1439 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/filter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4726 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/language.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3231 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/mail.py
+-rw-r--r--   0 maurits    (501) staff       (20)      766 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/maintenance.py
+-rw-r--r--   0 maurits    (501) staff       (20)      891 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/markup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2522 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/navigation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1446 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/search.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2692 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/security.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1160 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/site.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1327 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/usergroups.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.568314 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3498 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/actions.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     7113 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10862 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      880 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/controlpanel_usergroups_layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      703 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/dateandtime.py
+-rw-r--r--   0 maurits    (501) staff       (20)      654 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/editing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2756 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/emaillogin.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6715 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/error_log_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2187 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/error_log_form.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3683 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/error_log_show_entry.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2070 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/filter.py
+-rw-r--r--   0 maurits    (501) staff       (20)      687 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/filter_controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      510 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/imaging.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2061 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/language.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3837 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/mail.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6382 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/maintenance.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5290 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/maintenance.py
+-rw-r--r--   0 maurits    (501) staff       (20)      635 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/markup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1114 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/navigation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7477 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/overview.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4690 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/overview.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3926 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/prefsmaintemplate.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      408 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/prefsmaintemplate.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10262 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/quickinstaller.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    23365 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/quickinstaller.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12623 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/redirects-controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4768 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/redirects-manage.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    19982 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/redirects.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3683 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/relations.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4963 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/relations_inspect.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4683 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/relations_rebuild.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10139 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/resourceregistry.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5741 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/resourceregistry.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2092 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/search.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4586 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/security.py
+-rw-r--r--   0 maurits    (501) staff       (20)      939 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/site.py
+-rw-r--r--   0 maurits    (501) staff       (20)      500 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/socialmedia.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3879 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/syndication.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1667 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/tinymce.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14509 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/types.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    21314 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5693 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11351 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupdetails.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3859 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupdetails.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17772 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupmembership.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4324 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupmembership.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10602 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupsoverview.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6451 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupsoverview.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10094 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_usermembership.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2675 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_usermembership.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11225 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_usersoverview.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10376 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_usersoverview.py
+-rw-r--r--   0 maurits    (501) staff       (20)      296 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4522 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)      246 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/events.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1495 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.585729 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1459 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3561 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_editing_adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2177 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_filter_adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9454 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_language_adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4727 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_mail_adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1484 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_maintenance_adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1812 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_markup_adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4962 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_navigation_adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2227 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_search_adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4029 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_security_adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2088 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_site_adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1439 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_usergroups_adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4125 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_editing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2608 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_error_log.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4109 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_filter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5264 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_installer.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11410 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_language.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8588 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_mail.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3449 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_maintenance.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3819 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_markup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6772 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_navigation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    37430 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_redirection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2756 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_relations.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2844 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_search.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3768 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_security.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7464 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_site.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4075 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_syndication.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9137 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_types.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18911 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_usergroups.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14697 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_usergroups_siteadmin_role.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1883 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_dateandtime.py
+-rw-r--r--   0 maurits    (501) staff       (20)      724 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_doctest.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1742 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_editing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6145 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_events.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1677 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_filter.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17858 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_installer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2686 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_language.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1318 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_mail.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1520 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_markup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2021 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_navigation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2632 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_overview.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6834 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_relations.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1556 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_search.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2132 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_security.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1770 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_site.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1230 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1656 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_usergroups.py
+-rw-r--r--   0 maurits    (501) staff       (20)      884 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1221 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_upgrades1.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1778 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_upgrades2.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1729 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      972 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/widgets.py
+-rw-r--r--   0 maurits    (501) staff       (20)       84 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/defaultpage.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.586410 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/earlypatches/
+-rw-r--r--   0 maurits    (501) staff       (20)       82 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/earlypatches/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2524 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/earlypatches/security.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1186 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/events.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.588087 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/
+-rw-r--r--   0 maurits    (501) staff       (20)       27 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5366 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6325 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1298 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/memberdata_properties.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4807 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/propertiestool.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.589417 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)       33 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      374 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2106 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/tests/testControlPanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3376 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/tests/testPropertiesTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7351 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/factory.py
+-rw-r--r--   0 maurits    (501) staff       (20)       81 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/i18nl10n.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.591103 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/image_scales/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/image_scales/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1168 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/image_scales/adapters.py
+-rw-r--r--   0 maurits    (501) staff       (20)      290 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/image_scales/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      765 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/image_scales/indexer.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.592001 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/image_scales/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/image_scales/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      419 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/image_scales/tests/images.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     6078 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/image_scales/tests/test_image_scales_metadata.py
+-rw-r--r--   0 maurits    (501) staff       (20)      199 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/index.gif
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.599634 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/
+-rw-r--r--   0 maurits    (501) staff       (20)     4678 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)       87 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/atd.py
+-rw-r--r--   0 maurits    (501) staff       (20)       92 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/basetool.py
+-rw-r--r--   0 maurits    (501) staff       (20)       95 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/breadcrumbs.py
+-rw-r--r--   0 maurits    (501) staff       (20)       94 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/constrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)       96 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)       95 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/defaultpage.py
+-rw-r--r--   0 maurits    (501) staff       (20)       90 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)       95 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/installable.py
+-rw-r--r--   0 maurits    (501) staff       (20)       93 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/interface.py
+-rw-r--r--   0 maurits    (501) staff       (20)       92 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/language.py
+-rw-r--r--   0 maurits    (501) staff       (20)       89 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/login.py
+-rw-r--r--   0 maurits    (501) staff       (20)       93 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/migration.py
+-rw-r--r--   0 maurits    (501) staff       (20)       98 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/password_reset.py
+-rw-r--r--   0 maurits    (501) staff       (20)       92 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)       94 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/properties.py
+-rw-r--r--   0 maurits    (501) staff       (20)       93 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/resources.py
+-rw-r--r--   0 maurits    (501) staff       (20)       92 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/siteroot.py
+-rw-r--r--   0 maurits    (501) staff       (20)       93 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/structure.py
+-rw-r--r--   0 maurits    (501) staff       (20)       95 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/syndication.py
+-rw-r--r--   0 maurits    (501) staff       (20)      102 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/translationservice.py
+-rw-r--r--   0 maurits    (501) staff       (20)      165 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/workflow.py
+-rw-r--r--   0 maurits    (501) staff       (20)      869 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/log.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1608 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/meta.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1038 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/overrides.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.604655 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/
+-rw-r--r--   0 maurits    (501) staff       (20)      944 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1501 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/addzmiplonesite.py
+-rw-r--r--   0 maurits    (501) staff       (20)      863 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/addzmisecuritywarning.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1781 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      796 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/dateIndexPatch.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2596 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/gtbn.py
+-rw-r--r--   0 maurits    (501) staff       (20)      653 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/iso8601.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1510 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/publishing.py
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/security.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1660 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/sendmail.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1075 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/speed.py
+-rw-r--r--   0 maurits    (501) staff       (20)      952 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/templatecookcheck.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1855 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/unicodeFallbackPatch.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1031 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/unicodehacks.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2551 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/z3c_form.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.606772 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patterns/
+-rw-r--r--   0 maurits    (501) staff       (20)      405 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patterns/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      722 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patterns/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6678 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patterns/settings.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9151 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patterns/tinymce.py
+-rw-r--r--   0 maurits    (501) staff       (20)      799 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patterns/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1618 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patterns/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)       84 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/permissions.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.486396 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.611672 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)    16012 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     5143 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     3553 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/componentregistry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2629 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/contenttyperegistry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     9540 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      125 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/mailhost.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      961 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/memberdata_properties.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       71 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      119 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/properties.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      376 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/propertiestool.xml
+-rw-r--r--   0 maurits    (501) staff       (20)    10601 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/rolemap.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      781 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/skins.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2838 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/toolset.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.612905 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     1460 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/types/Discussion_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2782 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/types/Plone_Site.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1366 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/types/TempFolder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      386 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1746 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/viewlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.486028 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.613575 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/folder_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     7684 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/folder_workflow/definition.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.613935 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/intranet_folder_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     6170 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/intranet_folder_workflow/definition.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.614260 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/intranet_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)    13766 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/intranet_workflow/definition.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.614585 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/one_state_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     3117 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/one_state_workflow/definition.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.614927 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/plone_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)    10574 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/plone_workflow/definition.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.615267 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/simple_publication_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     8772 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/simple_publication_workflow/definition.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.616228 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/dependencies/
+-rw-r--r--   0 maurits    (501) staff       (20)     1049 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/dependencies/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     4765 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/dependencies/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     4738 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/dependencies/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.617201 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/testfixture/
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/testfixture/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/testfixture/plone-update-workflow-rolemap.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      369 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/testfixture/workflows.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1147 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    11709 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/relationhelper.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.618761 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/
+-rw-r--r--   0 maurits    (501) staff       (20)     1109 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.620057 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      346 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/browser/combine.py
+-rw-r--r--   0 maurits    (501) staff       (20)      846 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    13197 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/browser/resource.py
+-rw-r--r--   0 maurits    (501) staff       (20)      205 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      678 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/eventhandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4539 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2707 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/webresource.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8829 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/setuphandlers.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.487507 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.637846 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/
+-rw-r--r--   0 maurits    (501) staff       (20)      114 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowBottom.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowBottom.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      112 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowDown.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowDown.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      109 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowLeft.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowLeft.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      117 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowLeftmost.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowLeftmost.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      108 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowRight.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowRight.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      117 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowRightmost.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowRightmost.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      114 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowTop.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowTop.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      112 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowUp.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/arrowUp.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      313 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/book_icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/book_icon.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      367 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/confirm_icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/confirm_icon.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      859 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/defaultUser.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/defaultUser.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/document_icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/document_icon.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      455 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/group.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/group.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      675 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/info_icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/info_icon.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      338 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/link_icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/link_icon.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      278 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/lock_icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/lock_icon.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)     1338 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/logo.png
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/logo.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      226 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/logoIcon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/logoIcon.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)     1097 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/pb_close.png
+-rw-r--r--   0 maurits    (501) staff       (20)      226 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/pencil_icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/pencil_icon.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      410 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/product_icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/product_icon.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      608 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/rss.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/rss.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      226 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/site_icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/site_icon.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      663 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/skins_icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/skins_icon.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      223 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/topic_icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/topic_icon.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      359 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/user.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/user.png.metadata
+-rw-r--r--   0 maurits    (501) staff       (20)      228 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/workflow_icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/workflow_icon.png.metadata
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.641134 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/
+-rw-r--r--   0 maurits    (501) staff       (20)      271 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/browserDefault.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1088 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/externalEditorEnabled.py
+-rw-r--r--   0 maurits    (501) staff       (20)      786 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/external_edit.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1671 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/getFolderContents.py
+-rw-r--r--   0 maurits    (501) staff       (20)      425 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/pretty_title_or_id.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3634 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/queryCatalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)      473 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/toLocalizedTime.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1095 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/translate.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2281 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/unique.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1119 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/utranslate.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.641441 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_wysiwyg/
+-rw-r--r--   0 maurits    (501) staff       (20)     1999 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_wysiwyg/wysiwyg_support.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3899 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.676941 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)   160651 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/900.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)     7089 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/AddMoveAndDeleteDocument.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     7127 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/LoginAndLogout.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1479 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/PloneTestCase.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)       84 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/accesscontrol_direct.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      107 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/accesscontrol_sm.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      170 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/accesscontrol_via_dict.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       99 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/accesscontrol_via_modules.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      104 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/bad1.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      104 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/bad2.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      247 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/bad3.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1119 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/base_tag_not_present.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2669 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/browser.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4785 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/browser_collection_views.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      299 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    17940 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/csrf.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4937 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/dummy.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10571 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/emaillogin.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3583 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/link_redirect_view.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2534 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/mails.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      105 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/normal_zope3_page_template.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       49 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/options_authenticator.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       35 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/options_name.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       36 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/options_underscore.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       43 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/options_view_name.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    20500 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/pwreset_browser.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.686630 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2197 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/common.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1318 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/keywords.robot
+-rw-r--r--   0 maurits    (501) staff       (20)       69 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/pixel.png
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/plone-logo.png
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.690708 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/
+-rw-r--r--   0 maurits    (501) staff       (20)     3617 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      417 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/TODO.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2799 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/anonymous.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1125 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/collaboration-advanced_control.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2515 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/collaboration.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1705 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/common.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     6188 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/config-screens.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     9471 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/content.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3889 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/managing-working_copy.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     6372 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/managing_content.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1148 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/personalsettings.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2187 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/working_with_tinymce.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1177 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robot_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5850 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_actionmenu.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     4658 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_actions.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3955 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_editing.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     6628 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_filter.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1633 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_language.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3627 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_markup.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     4571 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_navigation.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3491 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_redirection.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2935 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_search.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     6960 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_security.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     4630 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_site.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2742 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_social.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2770 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_types.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     4184 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_usergroups.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     6053 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_edit.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     7606 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_edit_user_schema.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3973 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_folder_contents.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     6135 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_linkintegrity.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3055 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_livesearch.robot
+-rw-r--r--   0 maurits    (501) staff       (20)    12377 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_overlays.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2569 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_portlets.robot
+-rw-r--r--   0 maurits    (501) staff       (20)    14599 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_querystring.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3075 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_tinymce.robot
+-rw-r--r--   0 maurits    (501) staff       (20)       81 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/variables.py
+-rw-r--r--   0 maurits    (501) staff       (20)      542 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/scripts.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1492 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/search_form.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5069 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testActionsTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)      852 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testBatch.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1367 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testBrowserAdmin.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15829 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testBrowserDefault.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1329 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testBrowserLayerPrecedence.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3475 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testCSRFProtection.py
+-rw-r--r--   0 maurits    (501) staff       (20)    56012 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testCatalogTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8225 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testCheckId.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8355 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testContentSecurity.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5130 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testContentTypeScripts.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1269 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testControlPanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1072 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testControlPanelScripts.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2321 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testCookieAuth.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8154 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testCutPasteSecurity.py
+-rw-r--r--   0 maurits    (501) staff       (20)      925 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testDateIndexRanges.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2432 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testDateTimeIntegration.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5726 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testEmailLogin.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3248 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testExternalEditorEnabled.py
+-rw-r--r--   0 maurits    (501) staff       (20)      829 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testIImagingSchema.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12541 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testInterfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10770 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testMigrationTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)    28213 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testNavTree.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19832 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testNavigationView.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4383 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testNextPrevious.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9801 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testOrderSupport.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1462 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testPloneTestCase.py
+-rw-r--r--   0 maurits    (501) staff       (20)    26401 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testPloneTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8765 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testPloneView.py
+-rw-r--r--   0 maurits    (501) staff       (20)    40324 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testPortalCreation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11130 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testQueryCatalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14244 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testRegistrationTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18000 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testResourceRegistries.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1773 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testRestrictedAcquisition.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14341 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testSearch.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10136 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testSecurity.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15250 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testSecurityDeclarations.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12813 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testSiteAdminRole.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14071 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testSyndication.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2705 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testTranslationServiceTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7327 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testURLTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14556 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testUnicodeSplitter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5405 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testUserFolderBasics.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20154 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testWebDAV.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6235 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testWorkflowTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5823 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_PloneTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4807 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_defaultpage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      309 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2618 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_error_message.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12186 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_expressions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2833 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_factory.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2448 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2470 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_icons.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7976 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_login_form.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8259 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_login_help.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3905 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_login_logout.py
+-rw-r--r--   0 maurits    (501) staff       (20)      714 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_login_views.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1870 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_mails.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1659 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_nogopip.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1949 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_okay.py
+-rw-r--r--   0 maurits    (501) staff       (20)      910 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_passwordreset.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5197 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_patternsettings.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10894 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_redirect_after_login.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3484 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_redirection.py
+-rw-r--r--   0 maurits    (501) staff       (20)      907 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)      846 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_robots_txt.py
+-rw-r--r--   0 maurits    (501) staff       (20)    16875 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_safe_formatter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1582 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_sitelogo.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2319 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_sitemap.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2417 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4110 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_z3c_form_widgets.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8057 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_zmi.py
+-rw-r--r--   0 maurits    (501) staff       (20)      448 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/using_format_zope3_page_template.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2383 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)       35 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/view_name.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      168 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tool.gif
+-rw-r--r--   0 maurits    (501) staff       (20)     3274 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)      541 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/unicodeconflictresolver.py
+-rw-r--r--   0 maurits    (501) staff       (20)    25220 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1953 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/workflow.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.692315 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/www/
+-rw-r--r--   0 maurits    (501) staff       (20)      205 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/www/addConfigletForm.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1040 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/www/addPropertySheet.zpt
+-rw-r--r--   0 maurits    (501) staff       (20)     4801 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/www/catalogAdvanced.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)     6064 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/www/editPloneConfiglets.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)     2332 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/CMFPlone/www/zmi_metadata.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/Products/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.495288 Products.CMFPlone-6.0.4rc1/Products.CMFPlone.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    33188 2023-04-21 14:51:45.000000 Products.CMFPlone-6.0.4rc1/Products.CMFPlone.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    30071 2023-04-21 14:51:45.000000 Products.CMFPlone-6.0.4rc1/Products.CMFPlone.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-21 14:51:45.000000 Products.CMFPlone-6.0.4rc1/Products.CMFPlone.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2023-04-21 14:51:45.000000 Products.CMFPlone-6.0.4rc1/Products.CMFPlone.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-21 14:51:45.000000 Products.CMFPlone-6.0.4rc1/Products.CMFPlone.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)     1433 2023-04-21 14:51:45.000000 Products.CMFPlone-6.0.4rc1/Products.CMFPlone.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2023-04-21 14:51:45.000000 Products.CMFPlone-6.0.4rc1/Products.CMFPlone.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     6424 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/README.md
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:51:45.695449 Products.CMFPlone-6.0.4rc1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     6320 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/docs/CREDITS.txt
+-rw-r--r--   0 maurits    (501) staff       (20)   537526 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/docs/HISTORY.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)     2070 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/docs/LICENSE.ZPL
+-rw-r--r--   0 maurits    (501) staff       (20)      667 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1460 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/docs/UPGRADE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      308 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/docs/changelog_template.jinja
+-rw-r--r--   0 maurits    (501) staff       (20)      503 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      215 2023-04-21 14:51:45.696594 Products.CMFPlone-6.0.4rc1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     4258 2023-04-21 14:51:44.000000 Products.CMFPlone-6.0.4rc1/setup.py
```

### Comparing `Products.CMFPlone-6.0.3rc1/.gitignore` & `Products.CMFPlone-6.0.4rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/CHANGES.md` & `Products.CMFPlone-6.0.4rc1/CHANGES.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,52 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 6.0.4rc1 (2023-04-21)
+
+
+### Bug fixes:
+
+- Prepare 6.0.3 final. No changes compared to the release candidate.
+  [maurits] #603
+- Add a last modification time of the resource registry.
+  We update this when changing anything related: when changing the resource registry in its control panel or activating an add-on.
+  This avoids needing a restart before seeing changes when you run in production mode.
+  Fixes [issue 3505](https://github.com/plone/Products.CMFPlone/issues/3505).
+  [maurits] #3505
+- Removed path query from search view when context is site root.
+  [malthe] #3753
+- Fixed encoding issue on Python 3 for some mail servers.
+  This could result in missing characters in an email body.
+  [maurits] #3754
+- Mockup TinyMCE settings: Fix URLs in TinyMCE external_plugins settings.
+
+  Add the portal URL to external_plugins values for relative and absolute
+  URLs.
+
+  Before this fix external plugins could not be found if they were not added with
+  the full path or a full URL. The path is different for virtual hosted sites and
+  sites directly served from Zope. #3767
+- Updated metadata version to 6015.
+  [maurits] #6015
+
+
+## 6.0.3 (2023-03-27)
+
+
+### Bug fixes:
+
+- Prepare 6.0.3 final. No changes compared to the release candidate.
+  [maurits] #603
+
+
 ## 6.0.3rc1 (2023-03-23)
 
 
 ### Bug fixes:
 
 - Remove unused template send_feedback_confirm.pt. 
   [jensens] #3122
```

### Comparing `Products.CMFPlone-6.0.3rc1/LICENSE` & `Products.CMFPlone-6.0.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/PKG-INFO` & `Products.CMFPlone-6.0.4rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.CMFPlone
-Version: 6.0.3rc1
+Version: 6.0.4rc1
 Summary: The Plone Content Management System (core)
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -190,14 +190,52 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 6.0.4rc1 (2023-04-21)
+
+
+### Bug fixes:
+
+- Prepare 6.0.3 final. No changes compared to the release candidate.
+  [maurits] #603
+- Add a last modification time of the resource registry.
+  We update this when changing anything related: when changing the resource registry in its control panel or activating an add-on.
+  This avoids needing a restart before seeing changes when you run in production mode.
+  Fixes [issue 3505](https://github.com/plone/Products.CMFPlone/issues/3505).
+  [maurits] #3505
+- Removed path query from search view when context is site root.
+  [malthe] #3753
+- Fixed encoding issue on Python 3 for some mail servers.
+  This could result in missing characters in an email body.
+  [maurits] #3754
+- Mockup TinyMCE settings: Fix URLs in TinyMCE external_plugins settings.
+
+  Add the portal URL to external_plugins values for relative and absolute
+  URLs.
+
+  Before this fix external plugins could not be found if they were not added with
+  the full path or a full URL. The path is different for virtual hosted sites and
+  sites directly served from Zope. #3767
+- Updated metadata version to 6015.
+  [maurits] #6015
+
+
+## 6.0.3 (2023-03-27)
+
+
+### Bug fixes:
+
+- Prepare 6.0.3 final. No changes compared to the release candidate.
+  [maurits] #603
+
+
 ## 6.0.3rc1 (2023-03-23)
 
 
 ### Bug fixes:
 
 - Remove unused template send_feedback_confirm.pt. 
   [jensens] #3122
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/ActionsTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/ActionsTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/CatalogTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/CatalogTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/MigrationTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/MigrationTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/PasswordResetTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/PasswordResetTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/PloneBaseTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/PloneBaseTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/PloneControlPanel.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/PloneControlPanel.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/PloneTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/PloneTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/Portal.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/Portal.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/PropertiesTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/PropertiesTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/RegistrationTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/RegistrationTool.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from AccessControl import Unauthorized
 from AccessControl.class_init import InitializeClass
 from AccessControl.requestmethod import postonly
 from AccessControl.SecurityManagement import newSecurityManager
 from AccessControl.SecurityManagement import setSecurityManager
 from Acquisition import aq_base
 from Acquisition import aq_chain
-from email import message_from_string
 from hashlib import md5
 from plone.base import PloneMessageFactory as _
 from plone.base.interfaces import ISecuritySchema
 from plone.base.permissions import ManagePortal
 from plone.protect import CheckAuthenticator
 from plone.protect import protect
 from plone.registry.interfaces import IRegistry
@@ -30,14 +29,21 @@
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.schema import ValidationError
 
 import random
 import re
 
+try:
+    # Products.MailHost has a patch to fix quoted-printable soft line breaks.
+    # See https://github.com/zopefoundation/Products.MailHost/issues/35
+    from Products.MailHost.MailHost import message_from_string
+except ImportError:
+    # If the patch is ever removed, we fall back to the standard library.
+    from email import message_from_string
 
 # - remove '1', 'l', and 'I' to avoid confusion
 # - remove '0', 'O', and 'Q' to avoid confusion
 # - remove vowels to avoid spelling words
 invalid_password_chars = ['a', 'e', 'i', 'o', 'u', 'y', 'l', 'q']
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/SkinsTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/SkinsTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/TranslationServiceTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/TranslationServiceTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/TypesTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/TypesTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/URLTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/URLTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/UnicodeSplitter/config.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/UnicodeSplitter/config.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/UnicodeSplitter/splitter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/UnicodeSplitter/splitter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/WorkflowTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/WorkflowTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/__init__.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/admin.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/admin.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/admin.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/admin.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/atd.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/atd.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/author.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/author.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/configure.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/contact_info.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/sendto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,105 @@
-from email.mime.text import MIMEText
-from plone.autoform.form import AutoExtensibleForm
+from .interfaces import ISendToForm
 from plone.base import PloneMessageFactory as _
 from plone.base.interfaces.controlpanel import IMailSchema
+from plone.base.utils import pretty_title_or_id
 from plone.registry.interfaces import IRegistry
-from Products.CMFCore.utils import getToolByName
-from Products.CMFPlone.browser.interfaces import IContactForm
+from plone.z3cform import layout
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
+from Products.MailHost.interfaces import IMailHost
 from Products.statusmessages.interfaces import IStatusMessage
-from smtplib import SMTPException
 from z3c.form import button
+from z3c.form import field
 from z3c.form import form
+from ZODB.POSException import ConflictError
 from zope.component import getUtility
-from zope.component.hooks import getSite
 
 import logging
 
 
-log = logging.getLogger(__name__)
+logger = logging.getLogger("Plone")
 
 
-class ContactForm(AutoExtensibleForm, form.Form):
+class SendToForm(form.Form):
+    label = _('heading_send_page_to',
+              default='Send this page to someone')
 
-    template = ViewPageTemplateFile('templates/contact-info.pt')
-    template_mailview = '@@contact-info-email'
+    description = _('description_send_page_url_to',
+                    default='Fill in the email address of your '
+                    'friend, and we will send an email '
+                    'that contains a link to this page.')
 
-    schema = IContactForm
+    fields = field.Fields(ISendToForm)
     ignoreContext = True
-    success = False
 
-    def mailhost_is_configured(self):
-        registry = getUtility(IRegistry)
-        mail_settings = registry.forInterface(IMailSchema, prefix="plone")
-        if not mail_settings.email_from_address:
-            return False
-        return True
+    mail_template = ViewPageTemplateFile('templates/sendto_template.pt')
 
-    @button.buttonAndHandler(_('label_send', default='Send'), name='send')
+    @button.buttonAndHandler(_('label_send', default='Send'),
+                             name='send')
     def handle_send(self, action):
         data, errors = self.extractData()
         if errors:
-            IStatusMessage(self.request).add(
+            IStatusMessage(self.request).addStatusMessage(
                 self.formErrorsMessage,
                 type='error'
             )
-
             return
 
-        self.send_message(data)
-        self.send_feedback()
-        self.success = True
-
-    def generate_mail(self, variables, encoding='utf-8'):
-        template = self.context.restrictedTraverse(self.template_mailview)
-        return template(self.context, **variables).encode(encoding)
-
-    def send_message(self, data):
-        subject = data.get('subject')
-
-        portal = getSite()
+        send_from_address = data.get('send_from_address')
+        send_to_address = data.get('send_to_address')
+        subject = pretty_title_or_id(self, self.context)
+        title = pretty_title_or_id(self, self.context)
+        description = self.context.Description()
+        comment = data.get('comment', None)
         registry = getUtility(IRegistry)
         mail_settings = registry.forInterface(IMailSchema, prefix='plone')
-        send_to_address = mail_settings.email_from_address
-        from_address = mail_settings.email_from_address
-        registry = getUtility(IRegistry)
-        encoding = registry.get('plone.email_charset', 'utf-8')
-        host = getToolByName(self.context, 'MailHost')
-
-        data['url'] = portal.absolute_url()
-        message = self.generate_mail(data, encoding)
-        message = MIMEText(message, 'plain', encoding)
-        message['Reply-To'] = data['sender_from_address']
+        envelope_from = mail_settings.email_from_address
+        email_from_name = mail_settings.email_from_name
 
         try:
-            # This actually sends out the mail
+            # Sends a link of a page to someone.
+            host = getUtility(IMailHost)
+            registry = getUtility(IRegistry)
+            encoding = registry.get('plone.email_charset', 'utf-8')
+
+            if not envelope_from:
+                envelope_from = send_from_address
+
+            # Cook from template
+            message = self.mail_template(
+                self,
+                send_to_address=send_to_address,
+                send_from_address=send_from_address,
+                comment=comment,
+                subject=subject,
+                title=title,
+                description=description,
+                email_from_name=email_from_name
+            )
+
+            message = message.encode(encoding)
+
             host.send(
                 message,
-                send_to_address,
-                from_address,
+                mto=send_to_address,
+                mfrom=envelope_from,
                 subject=subject,
-                charset=encoding
+                charset='utf-8'
+            )
+
+        except ConflictError:
+            raise
+        except Exception as e:
+            # TODO To many things could possibly go wrong. So we catch all.
+            logger.info("Unable to send mail: " + str(e))
+            IStatusMessage(self.request).addStatusMessage(
+                _('Unable to send mail.'),
+                type='error'
             )
-        except (SMTPException, RuntimeError) as e:
-            log.error(e)
-            plone_utils = getToolByName(portal, 'plone_utils')
-            exception = plone_utils.exceptionString()
-            message = _('Unable to send mail: ${exception}',
-                        mapping={'exception': exception})
-            IStatusMessage(self.request).add(message, type='error')
-
-    def send_feedback(self):
-        IStatusMessage(self.request).add(
-            _('A mail has now been sent to the site administrator '
-              'regarding your questions and/or comments.')
+            return
+
+        IStatusMessage(self.request).addStatusMessage(
+            _('Mail sent.'),
+            type='info'
         )
+
+send_to_form = layout.wrap_form(SendToForm)
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/defaultpage.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/defaultpage.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/exceptions.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/exceptions.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/favicon.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/favicon.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/global_statusmessage.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/global_statusmessage.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/icons.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/icons.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/interfaces.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/configure.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/login.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/login.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/login_help.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/login_help.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from email import message_from_string
 from email.header import Header
 from plone.base import PloneMessageFactory as _
 from plone.base.interfaces import ILoginHelpForm
 from plone.base.interfaces import ILoginHelpFormSchema
 from plone.base.interfaces import ISecuritySchema
 from plone.base.interfaces.controlpanel import IMailSchema
 from plone.base.utils import safe_text
@@ -18,14 +17,22 @@
 from zope.component import getUtility
 from zope.component.hooks import getSite
 from zope.i18n import translate
 from zope.interface import implementer
 
 import logging
 
+try:
+    # Products.MailHost has a patch to fix quoted-printable soft line breaks.
+    # See https://github.com/zopefoundation/Products.MailHost/issues/35
+    from Products.MailHost.MailHost import message_from_string
+except ImportError:
+    # If the patch is ever removed, we fall back to the standard library.
+    from email import message_from_string
+
 
 SEND_USERNAME_TEMPLATE = _("mailtemplate_username_info", default="""From: {encoded_mail_sender}
 To: {email}
 Subject: Your username for {portal_url}
 Content-Type: text/plain
 Precedence: bulk
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/logout.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/logout.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/mail_password.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/mail_password.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/password_reset.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/password_reset.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/explainPWResetTool.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/explainPWResetTool.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/forced_password_change.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/forced_password_change.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/initial_login_password_change.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/initial_login_password_change.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/insufficient_privileges.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/insufficient_privileges.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/logged_out.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/logged_out.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/login.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/login.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/login_failsafe.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/login_failsafe.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/login_help.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/login_help.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/mail_password_form.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/mail_password_form.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/mail_password_response.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/mail_password_response.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/mail_password_template.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/mail_password_template.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/pwreset_expired.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/pwreset_expired.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/pwreset_finish.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/pwreset_finish.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/pwreset_form.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/pwreset_form.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/pwreset_invalid.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/pwreset_invalid.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/registered_notify_template.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/registered_notify_template.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/templates/subform_render.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/templates/subform_render.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/login/utils.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/login/utils.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/main_template.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/main_template.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/navigation.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/navigation.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/navtree.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/navtree.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/okay.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/okay.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/ploneview.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/ploneview.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/robots.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/robots.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/search.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from DateTime import DateTime
 from plone.app.contentlisting.interfaces import IContentListing
 from plone.app.layout.navigation.interfaces import INavigationRoot
 from plone.base.batch import Batch
+from plone.base.interfaces.siteroot import IPloneSiteRoot
 from plone.base.interfaces import ISearchSchema
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone.browser.navtree import getNavigationRoot
 from Products.ZCTextIndex.ParseTree import ParseError
 from zope.cachedescriptors.property import Lazy as lazy_property
 from zope.component import getMultiAdapter
@@ -138,16 +139,16 @@
         # respect `types_not_searched` setting
         types = query.get('portal_type', [])
         if 'query' in types:
             types = types['query']
         query['portal_type'] = self.filter_types(types)
         # respect effective/expiration date
         query['show_inactive'] = False
-        # respect navigation root
-        if 'path' not in query:
+        # respect navigation root if we're not at the site root.
+        if 'path' not in query and not IPloneSiteRoot.providedBy(self.context):
             query['path'] = getNavigationRoot(self.context)
 
         if 'sort_order' in query and not query['sort_order']:
             del query['sort_order']
         return query
 
     @lazy_property
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/sitelogo.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/sitelogo.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/sitemap.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/sitemap.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/favicon.ico` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/jstz-1.0.4.min.js` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/jstz-1.0.4.min.js`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/plone-admin-ui.js` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/plone-admin-ui.js`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/plone-logo.png` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/plone-logo.png`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/static/plone-logo.svg` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/static/plone-logo.svg`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/adapters.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/adapters.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/configure.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/settings.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/settings.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/RSS.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/RSS.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/atom.xml.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/atom.xml.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/itunes.xml.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/itunes.xml.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/newsml.xml.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/newsml.xml.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/rss.xml.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/rss.xml.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/templates/search-rss.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/templates/search-rss.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/tool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/tool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/utils.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/utils.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/syndication/views.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/syndication/views.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/accessibility-info.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/accessibility-info.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/ajax_main_template.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/ajax_main_template.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/author.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/author.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/author_feedback_template.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/author_feedback_template.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/basic_error_message.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/basic_error_message.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/colophon.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/colophon.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/contact-info-email.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/contact-info-email.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/contact-info.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/contact-info.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/error_message.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/error_message.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/footer.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/footer.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/main_template.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/main_template.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/plone-addsite.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/plone-addsite.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/plone-admin-logged-out.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/plone-admin-logged-out.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/plone-frontpage.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/plone-frontpage.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/plone-overview.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/plone-overview.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/plone-upgrade.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/plone-upgrade.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/recently_modified.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/recently_modified.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/recently_published.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/recently_published.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/search.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/search.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/sendto_template.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/sendto_template.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/sitemap-item.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/sitemap-item.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/sitemap.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/sitemap.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/test_rendering.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/test_rendering.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/test_rendering_cheatsheet.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/test_rendering_cheatsheet.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/templates/test_rendering_icons.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/templates/test_rendering_icons.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/browser/test_rendering.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/browser/test_rendering.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/catalog.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/catalog.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/configure.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/README.rst` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/README.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/configure.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/editing.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/editing.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/filter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/filter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/language.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/language.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/mail.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/mail.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/maintenance.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/maintenance.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/markup.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/markup.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/navigation.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/navigation.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/search.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/search.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/security.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/security.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/site.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/site.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/bbb/usergroups.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/bbb/usergroups.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/actions.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/actions.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/actions.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/actions.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/configure.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/controlpanel_usergroups_layout.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/controlpanel_usergroups_layout.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/dateandtime.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/dateandtime.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/editing.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/editing.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/emaillogin.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/emaillogin.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/error_log_form.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/error_log_form.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/error_log_form.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/error_log_form.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/error_log_show_entry.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/error_log_show_entry.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/filter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/filter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/filter_controlpanel.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/filter_controlpanel.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/language.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/language.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,15 +47,7 @@
         self.request.response.redirect("{}/{}".format(
             self.context.absolute_url(),
             self.control_panel_view))
 
 
 class LanguageControlPanel(controlpanel.ControlPanelFormWrapper):
     form = LanguageControlPanelForm
-
-
-# class LanguageControlPanel(ControlPanelForm):
-#    form_fields = FormFields(ILanguageSchema)
-#    form_fields['default_language'].custom_widget = \
-#       LanguageDropdownChoiceWidget
-#
-#    form_name = _(u"heading_language_settings", default="Language Settings")
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/mail.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/mail.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/maintenance.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/maintenance.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/maintenance.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/maintenance.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/markup.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/markup.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/navigation.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/navigation.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/overview.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/overview.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/overview.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/overview.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/prefsmaintemplate.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/prefsmaintemplate.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/quickinstaller.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/quickinstaller.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/quickinstaller.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/quickinstaller.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/redirects-controlpanel.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/redirects-controlpanel.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/redirects-manage.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/redirects-manage.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/redirects.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/redirects.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/relations.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/relations.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/relations_inspect.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/relations_inspect.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/relations_rebuild.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/relations_rebuild.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/resourceregistry.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/resourceregistry.pt`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,14 @@
          role="alert">
           <button name="action" value="activate_cache" type="submit" class="btn btn-primary ms-1 me-1 mb-1 float-end" i18n:translate="">Activate Debug Mode</button>
         <tal:icon tal:replace="structure python:icons.tag('plone-statusmessage-info', tag_alt='', tag_class='statusmessage-icon mb-1')" />
         <strong i18n:translate="">Production Mode Activated</strong>
         <span class="content"
               i18n:translate="">
             Resources are fast and hashes are cached in Plone.
-            Changes in resource settings are not applied directly.
         </span>
       </div>
     </form>
     <div class="accordion" id="accordionRR" tal:define="dummy python:view.process_form()">
       <tal:block tal:repeat="bundle python:view.bundles_data">
       <div class="accordion-item ${python:'active' if bundle['name'] == request.form.get('name', None) else ''}">
            <h2 class="accordion-header" id="heading-${python:bundle['safe_name']}">
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
  Global Debug Mode Activated  This is great for development. Resource hashes
 will be recalculated on each request. This is expensive, do not use use in
 production!
 Deactivate  Resource Debug Mode Activated  Resources are not cached in Plone.
 Their hashes will be recalculated on each request. This is expensive, do not
 use use in production!
 Activate Debug Mode  Production Mode Activated  Resources are fast and hashes
-are cached in Plone. Changes in resource settings are not applied directly.
+are cached in Plone.
 *****     ${python:bundle["name"]} Add new bundle  *****
 Name [${python:bundle['name']}]
 Javascript [${python:bundle['jscompilation']}]
 CSS [${python:bundle['csscompilation']}]
 {python:"checked" if bundle["enabled"] else ''} />  enabled
 Condition [${python:bundle['expression']}]
 Depends on [${python:bundle['depends']}]
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/resourceregistry.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/resourceregistry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from App.config import getConfiguration
 from plone.base import PloneMessageFactory as _
 from plone.base.interfaces import IBundleRegistry
 from plone.registry.interfaces import IRegistry
+from Products.CMFPlone.resources.browser.resource import update_resource_registry_mtime
 from Products.Five.browser import BrowserView
 from Products.statusmessages.interfaces import IStatusMessage
 from zope.component import getUtility
 
 import operator
 
 
@@ -145,8 +146,9 @@
             self._delete()
         elif action == "activate_cache":
             self._switch_cache(True)
         elif action == "deactivate_cache":
             self._switch_cache(False)
         else:
             raise ValueError("Invalid form data")
+        update_resource_registry_mtime()
         self.request.response.redirect(self.request["ACTUAL_URL"])
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/search.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/search.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/security.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/security.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/site.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/site.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/syndication.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/syndication.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/tinymce.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/tinymce.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/types.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/types.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/types.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/types.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupdetails.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupdetails.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupdetails.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupdetails.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupmembership.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupmembership.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupmembership.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupmembership.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupsoverview.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupsoverview.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupsoverview.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_groupsoverview.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_usermembership.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_usermembership.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_usermembership.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_usermembership.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_usersoverview.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_usersoverview.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/browser/usergroups_usersoverview.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/browser/usergroups_usersoverview.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/events.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/events.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/permissions.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/permissions.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_actions.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_actions.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_editing_adapter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_editing_adapter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_filter_adapter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_filter_adapter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_language_adapter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_language_adapter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_mail_adapter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_mail_adapter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_maintenance_adapter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_maintenance_adapter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_markup_adapter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_markup_adapter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_navigation_adapter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_navigation_adapter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_search_adapter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_search_adapter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_security_adapter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_security_adapter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_site_adapter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_site_adapter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_usergroups_adapter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_bbb_usergroups_adapter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_editing.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_editing.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_error_log.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_error_log.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_filter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_filter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_installer.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_installer.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_language.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_language.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_mail.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_mail.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_maintenance.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_maintenance.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_markup.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_markup.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_navigation.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_navigation.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_redirection.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_redirection.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_relations.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_relations.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_search.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_search.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_security.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_security.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_site.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_site.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_syndication.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_syndication.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_types.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_types.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_usergroups.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_usergroups.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_usergroups_siteadmin_role.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_browser_usergroups_siteadmin_role.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_dateandtime.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_dateandtime.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_doctest.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_doctest.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_editing.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_editing.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_events.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_events.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_filter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_filter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_installer.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_installer.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_language.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_language.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_mail.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_mail.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_markup.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_markup.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_navigation.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_navigation.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_overview.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_overview.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_relations.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_relations.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_search.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_search.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_security.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_security.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_site.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_site.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_types.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_types.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_usergroups.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_controlpanel_usergroups.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_doctests.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_upgrades1.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_upgrades1.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/tests/test_upgrades2.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/tests/test_upgrades2.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/utils.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/utils.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/controlpanel/widgets.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/controlpanel/widgets.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/earlypatches/security.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/earlypatches/security.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/events.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/events.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/configure.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/controlpanel.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/controlpanel.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/memberdata_properties.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/memberdata_properties.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/propertiestool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/propertiestool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/tests/testControlPanel.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/tests/testControlPanel.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/exportimport/tests/testPropertiesTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/exportimport/tests/testPropertiesTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/factory.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/factory.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/image_scales/adapters.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/image_scales/adapters.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/image_scales/indexer.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/image_scales/indexer.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/image_scales/tests/test_image_scales_metadata.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/image_scales/tests/test_image_scales_metadata.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/interfaces/__init__.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/log.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/log.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/meta.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/meta.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/overrides.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/overrides.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/__init__.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/addzmiplonesite.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/addzmiplonesite.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/addzmisecuritywarning.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/addzmisecuritywarning.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/csrf.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/csrf.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/dateIndexPatch.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/dateIndexPatch.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/gtbn.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/gtbn.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/iso8601.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/iso8601.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/publishing.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/publishing.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/sendmail.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/sendmail.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/speed.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/speed.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/templatecookcheck.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/templatecookcheck.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/unicodeFallbackPatch.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/unicodeFallbackPatch.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/unicodehacks.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/unicodehacks.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patches/z3c_form.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patches/z3c_form.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patterns/configure.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patterns/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patterns/settings.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patterns/settings.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patterns/tinymce.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patterns/tinymce.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,15 +167,21 @@
         if toolbar_additions:
             tiny_config["toolbar"] += " | {}".format(" ".join(toolbar_additions))
 
         for plugin in settings.custom_plugins or []:
             parts = plugin.split("|")
             if len(parts) != 2:
                 continue
-            tiny_config["external_plugins"][parts[0]] = parts[1]
+            url = parts[1].strip()
+            if not url:
+                continue
+            if url.find("//", 0, 8) == -1:
+                # assuming relative/absolute w/out url scheme
+                url = f"{self.nav_root_url}/{url}"
+            tiny_config["external_plugins"][parts[0]] = url
 
         tiny_config["style_formats"] = self.get_all_style_formats()
         if settings.formats:
             try:
                 tiny_config["formats"] = json.loads(settings.formats)
             except ValueError:
                 pass
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patterns/utils.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patterns/utils.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/patterns/view.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/patterns/view.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/actions.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/catalog.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/componentregistry.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/componentregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/contenttyperegistry.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/contenttyperegistry.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/controlpanel.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/memberdata_properties.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/memberdata_properties.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/rolemap.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/skins.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/toolset.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/toolset.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/types/Discussion_Item.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/types/Discussion_Item.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/types/Plone_Site.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/types/Plone_Site.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/types/TempFolder.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/types/TempFolder.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/viewlets.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/viewlets.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/folder_workflow/definition.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/folder_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/intranet_folder_workflow/definition.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/intranet_folder_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/intranet_workflow/definition.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/intranet_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/one_state_workflow/definition.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/one_state_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/plone_workflow/definition.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/plone_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows/simple_publication_workflow/definition.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows/simple_publication_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/default/workflows.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/dependencies/metadata.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/dependencies/metadata.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/dependencies/portlets.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/dependencies/portlets.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles/dependencies/registry.xml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles/dependencies/registry.xml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/profiles.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/relationhelper.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/relationhelper.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/__init__.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/browser/configure.zcml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/browser/resource.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/browser/resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 from App.config import getConfiguration
 from plone.app.layout.viewlets.common import ViewletBase
 from plone.app.theming.interfaces import IThemeSettings
 from plone.app.theming.utils import theming_policy
 from plone.base.interfaces import IBundleRegistry
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
+from time import time
 from zope.component import getMultiAdapter
 from zope.component import getUtility
+from zope.component import queryUtility
 from zope.component.hooks import getSite
 
 import hashlib
 import logging
 import webresource
 
 
 logger = logging.getLogger(__name__)
 
 REQUEST_CACHE_KEY = "_WEBRESOURCE_CACHE_"
-
+_RESOURCE_REGISTRY_MTIME = "__RESOURCE_REGISTRY_MTIME"
 GRACEFUL_DEPENDENCY_REWRITE = {
     "plone-base": "plone",
     "plone-legacy": "plone",
     "plone-logged-in": "plone",
 }
 
 
@@ -55,15 +57,20 @@
         hashtool = hashlib.sha256()
         hashtool.update(self.__class__.__name__.encode('utf8'))
         hashtool.update(site.absolute_url().encode('utf8'))
         e_bundles, d_bundles = self._request_bundles()
         for bundle in e_bundles | d_bundles:
             hashtool.update(bundle.encode('utf8'))
         hashtool.update(self._user_local_roles(site).encode("utf8"))
-        return f"_v_renderend_cache_{hashtool.hexdigest()}"
+        if not getattr(self, "registry", None):
+            self.registry = getUtility(IRegistry)
+            mtime = getattr(self.registry, _RESOURCE_REGISTRY_MTIME, None)
+            if mtime is not None:
+                hashtool.update(str(mtime).encode('utf8'))
+        return f"_v_rendered_cache_{hashtool.hexdigest()}"
 
     @property
     def _rendered_cache(self):
         if getConfiguration().debug_mode:
             return
         self.registry = getUtility(IRegistry)
         if not self.registry["plone.resources.development"]:
@@ -309,7 +316,23 @@
 
     def index(self):
         rendered = self._rendered_cache
         if not rendered:
             rendered = self.renderer["css"].render()
             self._rendered_cache = rendered
         return rendered
+
+
+def update_resource_registry_mtime():
+    """Update the last modification time of the resource registry.
+
+    Call this when you change anything that may influence the resource registry
+    and any of its rendered cache.
+    See discussion in https://github.com/plone/Products.CMFPlone/issues/3505
+    and https://github.com/plone/Products.CMFPlone/pull/3771
+    """
+    registry = queryUtility(IRegistry)
+    if registry is None:
+        # This can happen for example during site creation.
+        return
+    setattr(registry, _RESOURCE_REGISTRY_MTIME, time())
+    logger.info("Updated resource registry mtime.")
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/utils.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/utils.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/resources/webresource.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/resources/webresource.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/setuphandlers.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/defaultUser.png` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/defaultUser.png`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/info_icon.png` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/info_icon.png`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/logo.png` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/logo.png`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/pb_close.png` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/pb_close.png`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/rss.png` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/rss.png`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_images/skins_icon.png` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_images/skins_icon.png`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/externalEditorEnabled.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/externalEditorEnabled.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/external_edit.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/external_edit.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/getFolderContents.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/getFolderContents.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/queryCatalog.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/queryCatalog.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/translate.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/translate.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/unique.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/unique.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_scripts/utranslate.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_scripts/utranslate.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/skins/plone_wysiwyg/wysiwyg_support.pt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/skins/plone_wysiwyg/wysiwyg_support.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/testing.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/testing.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/900.jpg` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/900.jpg`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/AddMoveAndDeleteDocument.txt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/AddMoveAndDeleteDocument.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/LoginAndLogout.rst` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/LoginAndLogout.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/PloneTestCase.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/PloneTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/base_tag_not_present.txt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/base_tag_not_present.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/browser.txt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/browser.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/browser_collection_views.txt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/browser_collection_views.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/csrf.txt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/csrf.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/dummy.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/emaillogin.rst` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/emaillogin.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/link_redirect_view.txt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/link_redirect_view.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/mails.txt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/mails.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 =============================
 
 Some initial setup:
 
   >>> from plone.testing.zope import Browser
   >>> app = layer['app']
   >>> browser = Browser(app)
+  >>> browser.handleErrors = False
 
 
 Contact form
 ------------
 
 Let's go to the contact form:
 
@@ -54,20 +55,26 @@
   True
 
 We expect the headers to be properly header encoded (7-bit):
 
   >>> b'Subject: =?utf-8?q?Some_t=C3=A4st_subject=2E?=' in msg
   True
 
-The output should be encoded in a reasonable manner (in this case
-quoted-printable).  There may be some small differences in where
-exactly the lines are cut off, depending on whether you use five.pt
-(in Zope 2.13) or not, so we turn the message into one line first:
+The output should be encoded in a reasonable manner, in this case quoted-printable.
+On Python 3 there may be problems with quoted printable messages on some mail servers.
+See https://github.com/zopefoundation/Products.MailHost/issues/35
+When '\r\n' is used as line ending, all is well.
 
-  >>> msg.replace(b'=\n', b'').replace(b'\n', b' ')
+  >>> msg.count(b'\r\n') > 0
+  True
+
+There may be some small differences in where exactly the lines are cut off,
+so we turn the message into one line first:
+
+  >>> msg.replace(b'=\r\n', b'').replace(b'\r\n', b' ')
   b'...Another t=C3=A4st message...You are receiving this mail because T=C3=A4st user test@plone.test...is sending feedback about the site you administer at...'
 
 We can also decode the string, though we should still be careful about
 lines ending in different spots:
 
   >>> import quopri
   >>> quopri.decodestring(msg).replace(b'\n', b' ')
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/pwreset_browser.rst` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/pwreset_browser.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/common.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/common.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/keywords.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/keywords.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/plone-logo.png` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/plone-logo.png`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/README.rst` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/README.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/anonymous.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/anonymous.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/collaboration-advanced_control.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/collaboration-advanced_control.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/collaboration.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/collaboration.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/common.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/common.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/config-screens.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/config-screens.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/content.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/content.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/managing-working_copy.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/managing-working_copy.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/managing_content.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/managing_content.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/personalsettings.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/personalsettings.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robodoc/working_with_tinymce.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robodoc/working_with_tinymce.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/robot_setup.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/robot_setup.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_actionmenu.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_actionmenu.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_actions.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_actions.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_editing.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_editing.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_filter.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_filter.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_language.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_language.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_markup.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_markup.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_navigation.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_navigation.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_redirection.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_redirection.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_search.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_search.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_security.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_security.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_site.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_site.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_social.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_social.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_types.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_types.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_controlpanel_usergroups.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_controlpanel_usergroups.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_edit.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_edit.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_edit_user_schema.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_edit_user_schema.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_folder_contents.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_folder_contents.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_linkintegrity.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_linkintegrity.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_livesearch.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_livesearch.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_overlays.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_overlays.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_portlets.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_portlets.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_querystring.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_querystring.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/robot/test_tinymce.robot` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/robot/test_tinymce.robot`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/scripts.txt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/scripts.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/search_form.rst` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/search_form.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testActionsTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testActionsTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testBatch.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testBatch.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testBrowserAdmin.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testBrowserAdmin.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testBrowserDefault.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testBrowserDefault.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testBrowserLayerPrecedence.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testBrowserLayerPrecedence.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testCSRFProtection.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testCSRFProtection.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testCatalogTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testCatalogTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testCheckId.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testCheckId.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testContentSecurity.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testContentSecurity.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testContentTypeScripts.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testContentTypeScripts.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testControlPanel.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testControlPanel.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testControlPanelScripts.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testControlPanelScripts.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testCookieAuth.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testCookieAuth.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testCutPasteSecurity.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testCutPasteSecurity.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testDateIndexRanges.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testDateIndexRanges.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testDateTimeIntegration.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testDateTimeIntegration.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testEmailLogin.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testEmailLogin.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testExternalEditorEnabled.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testExternalEditorEnabled.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testIImagingSchema.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testIImagingSchema.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testInterfaces.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testInterfaces.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testMigrationTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testMigrationTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testNavTree.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testNavTree.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testNavigationView.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testNavigationView.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testNextPrevious.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testNextPrevious.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testOrderSupport.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testOrderSupport.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testPloneTestCase.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testPloneTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testPloneTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testPloneTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testPloneView.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testPloneView.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testPortalCreation.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testPortalCreation.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testQueryCatalog.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testQueryCatalog.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testRegistrationTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testRegistrationTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testResourceRegistries.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testResourceRegistries.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testRestrictedAcquisition.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testRestrictedAcquisition.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testSearch.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testSearch.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testSecurity.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testSecurity.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testSecurityDeclarations.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testSecurityDeclarations.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testSiteAdminRole.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testSiteAdminRole.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testSyndication.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testSyndication.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testTranslationServiceTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testTranslationServiceTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testURLTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testURLTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testUnicodeSplitter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testUnicodeSplitter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testUserFolderBasics.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testUserFolderBasics.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testWebDAV.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testWebDAV.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/testWorkflowTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/testWorkflowTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_PloneTool.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_PloneTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_defaultpage.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_defaultpage.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_error_message.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_error_message.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_expressions.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_factory.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_functional.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_icons.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_icons.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_login_form.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_login_form.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_login_help.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_login_help.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_login_logout.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_login_logout.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_login_views.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_login_views.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_mails.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_mails.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_nogopip.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_nogopip.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_okay.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_okay.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_passwordreset.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_passwordreset.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_redirect_after_login.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_redirect_after_login.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_redirection.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_redirection.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_robot.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_robots_txt.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_robots_txt.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_safe_formatter.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_safe_formatter.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_sitelogo.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_sitelogo.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_sitemap.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_sitemap.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_utils.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_z3c_form_widgets.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_z3c_form_widgets.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/test_zmi.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/test_zmi.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/tests/utils.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/tests/utils.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/traversal.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/traversal.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/unicodeconflictresolver.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/unicodeconflictresolver.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/utils.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/utils.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/workflow.py` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/workflow.py`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/www/addPropertySheet.zpt` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/www/addPropertySheet.zpt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/www/catalogAdvanced.dtml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/www/catalogAdvanced.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/www/editPloneConfiglets.dtml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/www/editPloneConfiglets.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products/CMFPlone/www/zmi_metadata.dtml` & `Products.CMFPlone-6.0.4rc1/Products/CMFPlone/www/zmi_metadata.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/Products.CMFPlone.egg-info/PKG-INFO` & `Products.CMFPlone-6.0.4rc1/Products.CMFPlone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.CMFPlone
-Version: 6.0.3rc1
+Version: 6.0.4rc1
 Summary: The Plone Content Management System (core)
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -190,14 +190,52 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 6.0.4rc1 (2023-04-21)
+
+
+### Bug fixes:
+
+- Prepare 6.0.3 final. No changes compared to the release candidate.
+  [maurits] #603
+- Add a last modification time of the resource registry.
+  We update this when changing anything related: when changing the resource registry in its control panel or activating an add-on.
+  This avoids needing a restart before seeing changes when you run in production mode.
+  Fixes [issue 3505](https://github.com/plone/Products.CMFPlone/issues/3505).
+  [maurits] #3505
+- Removed path query from search view when context is site root.
+  [malthe] #3753
+- Fixed encoding issue on Python 3 for some mail servers.
+  This could result in missing characters in an email body.
+  [maurits] #3754
+- Mockup TinyMCE settings: Fix URLs in TinyMCE external_plugins settings.
+
+  Add the portal URL to external_plugins values for relative and absolute
+  URLs.
+
+  Before this fix external plugins could not be found if they were not added with
+  the full path or a full URL. The path is different for virtual hosted sites and
+  sites directly served from Zope. #3767
+- Updated metadata version to 6015.
+  [maurits] #6015
+
+
+## 6.0.3 (2023-03-27)
+
+
+### Bug fixes:
+
+- Prepare 6.0.3 final. No changes compared to the release candidate.
+  [maurits] #603
+
+
 ## 6.0.3rc1 (2023-03-23)
 
 
 ### Bug fixes:
 
 - Remove unused template send_feedback_confirm.pt. 
   [jensens] #3122
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products.CMFPlone.egg-info/SOURCES.txt` & `Products.CMFPlone-6.0.4rc1/Products.CMFPlone.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -372,14 +372,15 @@
 Products/CMFPlone/profiles/dependencies/portlets.xml
 Products/CMFPlone/profiles/dependencies/registry.xml
 Products/CMFPlone/profiles/testfixture/metadata.xml
 Products/CMFPlone/profiles/testfixture/plone-update-workflow-rolemap.txt
 Products/CMFPlone/profiles/testfixture/workflows.xml
 Products/CMFPlone/resources/__init__.py
 Products/CMFPlone/resources/configure.zcml
+Products/CMFPlone/resources/eventhandlers.py
 Products/CMFPlone/resources/utils.py
 Products/CMFPlone/resources/webresource.py
 Products/CMFPlone/resources/browser/__init__.py
 Products/CMFPlone/resources/browser/combine.py
 Products/CMFPlone/resources/browser/configure.zcml
 Products/CMFPlone/resources/browser/resource.py
 Products/CMFPlone/skins/plone_images/arrowBottom.png
```

### Comparing `Products.CMFPlone-6.0.3rc1/Products.CMFPlone.egg-info/requires.txt` & `Products.CMFPlone-6.0.4rc1/Products.CMFPlone.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/README.md` & `Products.CMFPlone-6.0.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/docs/CREDITS.txt` & `Products.CMFPlone-6.0.4rc1/docs/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/docs/HISTORY.rst` & `Products.CMFPlone-6.0.4rc1/docs/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/docs/LICENSE.GPL` & `Products.CMFPlone-6.0.4rc1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/docs/LICENSE.ZPL` & `Products.CMFPlone-6.0.4rc1/docs/LICENSE.ZPL`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/docs/LICENSE.txt` & `Products.CMFPlone-6.0.4rc1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/docs/UPGRADE.txt` & `Products.CMFPlone-6.0.4rc1/docs/UPGRADE.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFPlone-6.0.3rc1/setup.py` & `Products.CMFPlone-6.0.4rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '6.0.3rc1'
+version = '6.0.4rc1'
 
 
 setup(
     name='Products.CMFPlone',
     version=version,
     description="The Plone Content Management System (core)",
     long_description=open("README.md").read() + "\n" +
```

