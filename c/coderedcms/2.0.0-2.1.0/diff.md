# Comparing `tmp/coderedcms-2.0.0.tar.gz` & `tmp/coderedcms-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coderedcms-2.0.0.tar", last modified: Mon Feb 27 19:47:13 2023, max compression
+gzip compressed data, was "coderedcms-2.1.0.tar", last modified: Fri Apr 21 16:43:51 2023, max compression
```

## Comparing `coderedcms-2.0.0.tar` & `coderedcms-2.1.0.tar`

### file list

```diff
@@ -1,513 +1,513 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.947552 coderedcms-2.0.0/
--rw-rw-rw-   0        0        0     1985 2022-08-03 20:24:51.000000 coderedcms-2.0.0/LICENSE
--rw-rw-rw-   0        0        0       94 2022-08-03 20:24:51.000000 coderedcms-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5776 2023-02-27 19:47:13.947552 coderedcms-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4358 2023-02-09 20:20:28.000000 coderedcms-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.611113 coderedcms-2.0.0/coderedcms/
--rw-rw-rw-   0        0        0      827 2023-02-27 19:45:50.000000 coderedcms-2.0.0/coderedcms/__init__.py
--rw-rw-rw-   0        0        0      482 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/admin_urls.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.616419 coderedcms-2.0.0/coderedcms/api/
--rw-rw-rw-   0        0        0     2996 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/api/mailchimp.py
--rw-rw-rw-   0        0        0      331 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/apps.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.616419 coderedcms-2.0.0/coderedcms/bin/
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/bin/__init__.py
--rw-rw-rw-   0        0        0     5239 2023-02-27 16:56:29.000000 coderedcms-2.0.0/coderedcms/bin/coderedcms.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.622286 coderedcms-2.0.0/coderedcms/blocks/
--rw-rw-rw-   0        0        0     4985 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/blocks/__init__.py
--rw-rw-rw-   0        0        0     8987 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/blocks/base_blocks.py
--rw-rw-rw-   0        0        0     7688 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/blocks/content_blocks.py
--rw-rw-rw-   0        0        0     8137 2023-02-17 20:46:38.000000 coderedcms-2.0.0/coderedcms/blocks/html_blocks.py
--rw-rw-rw-   0        0        0     2828 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/blocks/layout_blocks.py
--rw-rw-rw-   0        0        0     3856 2023-02-17 20:46:38.000000 coderedcms-2.0.0/coderedcms/blocks/stream_form_blocks.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.623287 coderedcms-2.0.0/coderedcms/blocks/tests/
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/blocks/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/blocks/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3201 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/fields.py
--rw-rw-rw-   0        0        0     5856 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/forms.py
--rw-rw-rw-   0        0        0     5656 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/importexport.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.654862 coderedcms-2.0.0/coderedcms/migrations/
--rw-rw-rw-   0        0        0    31791 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1460 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0002_auto_20180829_1538.py
--rw-rw-rw-   0        0        0     1445 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0003_auto_20180912_1632.py
--rw-rw-rw-   0        0        0     1160 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0004_auto_20181119_1507.py
--rw-rw-rw-   0        0        0     2371 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0005_auto_20181214_2214.py
--rw-rw-rw-   0        0        0      945 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0006_mailchimpapisettings.py
--rw-rw-rw-   0        0        0      514 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0007_auto_20190114_1515.py
--rw-rw-rw-   0        0        0     1108 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0008_auto_20190122_1242.py
--rw-rw-rw-   0        0        0      825 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0009_auto_20190201_1546.py
--rw-rw-rw-   0        0        0     1108 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0010_auto_20190320_1231.py
--rw-rw-rw-   0        0        0      618 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0010_generalsettings_email.py
--rw-rw-rw-   0        0        0      340 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0010_remove_generalsettings_robots.py
--rw-rw-rw-   0        0        0      293 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0011_merge_20190322_1309.py
--rw-rw-rw-   0        0        0      280 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0012_merge_20190322_1324.py
--rw-rw-rw-   0        0        0     1328 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0013_pagepreview_templates.py
--rw-rw-rw-   0        0        0     3846 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0014_classifiers.py
--rw-rw-rw-   0        0        0     2799 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0015_coderedsessionformsubmission_coderedsubmissionrevision.py
--rw-rw-rw-   0        0        0     1363 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0016_auto_20191025_1620.py
--rw-rw-rw-   0        0        0      460 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0017_generalsettings_external_new_tab.py
--rw-rw-rw-   0        0        0     1341 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0018_auto_20200805_1702.py
--rw-rw-rw-   0        0        0     1502 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0019_spelling_corrections.py
--rw-rw-rw-   0        0        0      997 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0020_auto_20210527_1030.py
--rw-rw-rw-   0        0        0      838 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0021_auto_20210730_1637.py
--rw-rw-rw-   0        0        0     1508 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0022_auto_20210731_1853.py
--rw-rw-rw-   0        0        0     1372 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0023_auto_20210908_1702.py
--rw-rw-rw-   0        0        0     1059 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0024_analyticssettings.py
--rw-rw-rw-   0        0        0      311 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0025_delete_socialmediasettings.py
--rw-rw-rw-   0        0        0     1336 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0026_auto_20220513_1627.py
--rw-rw-rw-   0        0        0      608 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0027_auto_20220603_1142.py
--rw-rw-rw-   0        0        0     1915 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0028_auto_20220609_1532.py
--rw-rw-rw-   0        0        0     3522 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0029_multinavs.py
--rw-rw-rw-   0        0        0      587 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/0030_alter_coderedtag_tag.py
--rw-rw-rw-   0        0        0     1840 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0031_wagtail3.py
--rw-rw-rw-   0        0        0     1784 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0032_accordion_accordionpanel.py
--rw-rw-rw-   0        0        0     2680 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0033_alter_coderedpage_struct_org_actions_and_more.py
--rw-rw-rw-   0        0        0      488 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0033_remove_carousel_animation_and_more.py
--rw-rw-rw-   0        0        0      319 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0034_delete_adasettings.py
--rw-rw-rw-   0        0        0     3367 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/migrations/0035_remove_googleapisettings_site_and_more.py
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.659015 coderedcms-2.0.0/coderedcms/models/
--rw-rw-rw-   0        0        0      323 2022-08-08 22:16:02.000000 coderedcms-2.0.0/coderedcms/models/__init__.py
--rw-rw-rw-   0        0        0     6389 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/models/integration_models.py
--rw-rw-rw-   0        0        0    68481 2023-02-27 16:56:29.000000 coderedcms-2.0.0/coderedcms/models/page_models.py
--rw-rw-rw-   0        0        0    12803 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/models/snippet_models.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.661659 coderedcms-2.0.0/coderedcms/models/tests/
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/models/tests/__init__.py
--rw-rw-rw-   0        0        0     4844 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/models/tests/test_navbars_and_footers.py
--rw-rw-rw-   0        0        0     9007 2023-02-17 22:51:24.000000 coderedcms-2.0.0/coderedcms/models/tests/test_page_models.py
--rw-rw-rw-   0        0        0     1953 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/models/tests/test_wagtailsettings_models.py
--rw-rw-rw-   0        0        0    10637 2023-02-27 16:56:29.000000 coderedcms-2.0.0/coderedcms/models/wagtailsettings_models.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.589043 coderedcms-2.0.0/coderedcms/project_template/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.665899 coderedcms-2.0.0/coderedcms/project_template/basic/
--rw-rw-rw-   0        0        0      722 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/basic/.editorconfig
--rw-rw-rw-   0        0        0      364 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/basic/.gitattributes
--rw-rw-rw-   0        0        0     5823 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/basic/.gitignore
--rw-rw-rw-   0        0        0      932 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/basic/README.md
--rw-rw-rw-   0        0        0      279 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/basic/manage.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.667890 coderedcms-2.0.0/coderedcms/project_template/basic/project_name/
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/basic/project_name/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.671113 coderedcms-2.0.0/coderedcms/project_template/basic/project_name/settings/
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/basic/project_name/settings/__init__.py
--rw-rw-rw-   0        0        0     5291 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/basic/project_name/settings/base.py
--rw-rw-rw-   0        0        0      388 2023-02-27 16:56:29.000000 coderedcms-2.0.0/coderedcms/project_template/basic/project_name/settings/dev.py
--rw-rw-rw-   0        0        0     1307 2023-02-27 16:56:29.000000 coderedcms-2.0.0/coderedcms/project_template/basic/project_name/settings/prod.py
--rw-rw-rw-   0        0        0     1223 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/basic/project_name/urls.py
--rw-rw-rw-   0        0        0      438 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/basic/project_name/wsgi.py
--rw-rw-rw-   0        0        0      119 2023-02-27 16:56:29.000000 coderedcms-2.0.0/coderedcms/project_template/basic/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.673391 coderedcms-2.0.0/coderedcms/project_template/basic/website/
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/basic/website/__init__.py
--rw-rw-rw-   0        0        0       89 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/basic/website/apps.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.675397 coderedcms-2.0.0/coderedcms/project_template/basic/website/migrations/
--rw-rw-rw-   0        0        0   259938 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/basic/website/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1552 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/basic/website/migrations/0002_initial_data.py
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/basic/website/migrations/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/basic/website/models.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.587577 coderedcms-2.0.0/coderedcms/project_template/basic/website/static/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.587577 coderedcms-2.0.0/coderedcms/project_template/basic/website/static/website/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.676852 coderedcms-2.0.0/coderedcms/project_template/basic/website/static/website/css/
--rw-rw-rw-   0        0        0      219 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/basic/website/static/website/css/custom.css
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.676852 coderedcms-2.0.0/coderedcms/project_template/basic/website/static/website/js/
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/basic/website/static/website/js/custom.js
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.589043 coderedcms-2.0.0/coderedcms/project_template/basic/website/templates/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.589043 coderedcms-2.0.0/coderedcms/project_template/basic/website/templates/coderedcms/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.677856 coderedcms-2.0.0/coderedcms/project_template/basic/website/templates/coderedcms/pages/
--rw-rw-rw-   0        0        0      392 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/basic/website/templates/coderedcms/pages/base.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.681989 coderedcms-2.0.0/coderedcms/project_template/sass/
--rw-rw-rw-   0        0        0      722 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/sass/.editorconfig
--rw-rw-rw-   0        0        0      364 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/sass/.gitattributes
--rw-rw-rw-   0        0        0     5823 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/sass/.gitignore
--rw-rw-rw-   0        0        0     1399 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/sass/README.md
--rw-rw-rw-   0        0        0      279 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/sass/manage.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.683989 coderedcms-2.0.0/coderedcms/project_template/sass/project_name/
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/sass/project_name/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.686989 coderedcms-2.0.0/coderedcms/project_template/sass/project_name/settings/
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/sass/project_name/settings/__init__.py
--rw-rw-rw-   0        0        0     5131 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/sass/project_name/settings/base.py
--rw-rw-rw-   0        0        0      438 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/sass/project_name/settings/dev.py
--rw-rw-rw-   0        0        0     1307 2023-02-27 16:56:29.000000 coderedcms-2.0.0/coderedcms/project_template/sass/project_name/settings/prod.py
--rw-rw-rw-   0        0        0     1223 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/sass/project_name/urls.py
--rw-rw-rw-   0        0        0      438 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/sass/project_name/wsgi.py
--rw-rw-rw-   0        0        0       44 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/sass/requirements-dev.txt
--rw-rw-rw-   0        0        0      251 2023-02-27 16:56:29.000000 coderedcms-2.0.0/coderedcms/project_template/sass/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.689112 coderedcms-2.0.0/coderedcms/project_template/sass/website/
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/sass/website/__init__.py
--rw-rw-rw-   0        0        0       89 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/sass/website/apps.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.691117 coderedcms-2.0.0/coderedcms/project_template/sass/website/migrations/
--rw-rw-rw-   0        0        0   259938 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/sass/website/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1552 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/sass/website/migrations/0002_initial_data.py
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/sass/website/migrations/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/sass/website/models.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.589043 coderedcms-2.0.0/coderedcms/project_template/sass/website/static/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.590388 coderedcms-2.0.0/coderedcms/project_template/sass/website/static/website/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.692188 coderedcms-2.0.0/coderedcms/project_template/sass/website/static/website/js/
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/project_template/sass/website/static/website/js/custom.js
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.694189 coderedcms-2.0.0/coderedcms/project_template/sass/website/static/website/src/
--rw-rw-rw-   0        0        0     1974 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/sass/website/static/website/src/_variables.scss
--rw-rw-rw-   0        0        0     1001 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/sass/website/static/website/src/custom.scss
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.590388 coderedcms-2.0.0/coderedcms/project_template/sass/website/templates/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.590388 coderedcms-2.0.0/coderedcms/project_template/sass/website/templates/coderedcms/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.694189 coderedcms-2.0.0/coderedcms/project_template/sass/website/templates/coderedcms/pages/
--rw-rw-rw-   0        0        0      913 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/project_template/sass/website/templates/coderedcms/pages/base.html
--rw-rw-rw-   0        0        0      125 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/search_urls.py
--rw-rw-rw-   0        0        0     9360 2023-02-17 20:46:38.000000 coderedcms-2.0.0/coderedcms/settings.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.590388 coderedcms-2.0.0/coderedcms/static/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.591784 coderedcms-2.0.0/coderedcms/static/coderedcms/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.698531 coderedcms-2.0.0/coderedcms/static/coderedcms/css/
--rw-rw-rw-   0        0        0      971 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/css/crx-admin.css
--rw-rw-rw-   0        0        0      886 2023-02-27 16:56:29.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/css/crx-editor.css
--rw-rw-rw-   0        0        0     5401 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/css/crx-front.css
--rw-rw-rw-   0        0        0     5363 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/css/crx-front.css.map
--rw-rw-rw-   0        0        0     4428 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/css/crx-front.min.css
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.703246 coderedcms-2.0.0/coderedcms/static/coderedcms/js/
--rw-rw-rw-   0        0        0      716 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/js/crx-editor.js
--rw-rw-rw-   0        0        0     1522 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/js/crx-events.js
--rw-rw-rw-   0        0        0     4496 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/js/crx-front.js
--rw-rw-rw-   0        0        0     5255 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/js/crx-maps.js
--rw-rw-rw-   0        0        0     1805 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/js/crx-streamforms.js
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.709869 coderedcms-2.0.0/coderedcms/static/coderedcms/scss/
--rw-rw-rw-   0        0        0      205 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/scss/_crx-article.scss
--rw-rw-rw-   0        0        0      367 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/scss/_crx-bs-overrides.scss
--rw-rw-rw-   0        0        0      152 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/scss/_crx-gallery.scss
--rw-rw-rw-   0        0        0      318 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/scss/_crx-hero.scss
--rw-rw-rw-   0        0        0     1749 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/scss/_crx-location.scss
--rw-rw-rw-   0        0        0     1988 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/scss/_crx-navbar.scss
--rw-rw-rw-   0        0        0      818 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/scss/_crx-pricelist.scss
--rw-rw-rw-   0        0        0      222 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/scss/_crx-richtext.scss
--rw-rw-rw-   0        0        0      403 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/scss/crx-front.scss
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.591784 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.710869 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/
--rw-rw-rw-   0        0        0     1131 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/LICENSE
--rw-rw-rw-   0        0        0      130 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/README.txt
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.591784 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.748019 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/
--rw-rw-rw-   0        0        0    71861 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0   210292 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0    53265 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0   131408 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css.map
--rw-rw-rw-   0        0        0    71935 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css
--rw-rw-rw-   0        0        0   210296 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css.map
--rw-rw-rw-   0        0        0    53340 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css
--rw-rw-rw-   0        0        0   131485 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
--rw-rw-rw-   0        0        0     7965 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0   110811 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0     6490 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0    40345 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css.map
--rw-rw-rw-   0        0        0     7958 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css
--rw-rw-rw-   0        0        0   110824 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
--rw-rw-rw-   0        0        0     6562 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
--rw-rw-rw-   0        0        0    48707 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-rw-   0        0        0    74135 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css
--rw-rw-rw-   0        0        0   196370 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css.map
--rw-rw-rw-   0        0        0    56365 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css
--rw-rw-rw-   0        0        0   115601 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css.map
--rw-rw-rw-   0        0        0    74002 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css
--rw-rw-rw-   0        0        0   196313 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
--rw-rw-rw-   0        0        0    56293 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
--rw-rw-rw-   0        0        0   115436 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-rw-   0        0        0   237872 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css
--rw-rw-rw-   0        0        0   606249 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   194699 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   521459 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0   237386 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css
--rw-rw-rw-   0        0        0   606069 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css.map
--rw-rw-rw-   0        0        0   194803 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css
--rw-rw-rw-   0        0        0   765329 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css.map
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.763775 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/
--rw-rw-rw-   0        0        0   207083 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0   448881 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js.map
--rw-rw-rw-   0        0        0    79790 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   330849 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0   135367 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js
--rw-rw-rw-   0        0        0   306814 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js.map
--rw-rw-rw-   0        0        0    73539 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js
--rw-rw-rw-   0        0        0   220143 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js.map
--rw-rw-rw-   0        0        0   144701 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js
--rw-rw-rw-   0        0        0   307954 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js.map
--rw-rw-rw-   0        0        0    60104 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   215897 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js.map
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.593037 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.776317 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/
--rw-rw-rw-   0        0        0     3801 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/alert.js
--rw-rw-rw-   0        0        0     6341 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/button.js
--rw-rw-rw-   0        0        0    16583 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/carousel.js
--rw-rw-rw-   0        0        0    10333 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/collapse.js
--rw-rw-rw-   0        0        0    14736 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dropdown.js
--rw-rw-rw-   0        0        0      773 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/index.js
--rw-rw-rw-   0        0        0    17563 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/modal.js
--rw-rw-rw-   0        0        0     4275 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/popover.js
--rw-rw-rw-   0        0        0     8777 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/scrollspy.js
--rw-rw-rw-   0        0        0     6635 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tab.js
--rw-rw-rw-   0        0        0     5178 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/toast.js
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.777318 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tools/
--rw-rw-rw-   0        0        0     3368 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tools/sanitizer.js
--rw-rw-rw-   0        0        0    18705 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tooltip.js
--rw-rw-rw-   0        0        0     5334 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util.js
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.810531 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/
--rw-rw-rw-   0        0        0     4757 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_accordion.scss
--rw-rw-rw-   0        0        0     2126 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_alert.scss
--rw-rw-rw-   0        0        0     1118 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_badge.scss
--rw-rw-rw-   0        0        0     1751 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_breadcrumb.scss
--rw-rw-rw-   0        0        0     3060 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_button-group.scss
--rw-rw-rw-   0        0        0     5959 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_buttons.scss
--rw-rw-rw-   0        0        0     6736 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_card.scss
--rw-rw-rw-   0        0        0     5625 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_carousel.scss
--rw-rw-rw-   0        0        0     1127 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_close.scss
--rw-rw-rw-   0        0        0     1201 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_containers.scss
--rw-rw-rw-   0        0        0     7950 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_dropdown.scss
--rw-rw-rw-   0        0        0      256 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_forms.scss
--rw-rw-rw-   0        0        0    10552 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_functions.scss
--rw-rw-rw-   0        0        0      575 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_grid.scss
--rw-rw-rw-   0        0        0      294 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_helpers.scss
--rw-rw-rw-   0        0        0     1158 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_images.scss
--rw-rw-rw-   0        0        0     6348 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_list-group.scss
--rw-rw-rw-   0        0        0     1648 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_maps.scss
--rw-rw-rw-   0        0        0      899 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_mixins.scss
--rw-rw-rw-   0        0        0     7762 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_modal.scss
--rw-rw-rw-   0        0        0     4665 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_nav.scss
--rw-rw-rw-   0        0        0     8854 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_navbar.scss
--rw-rw-rw-   0        0        0     4485 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_offcanvas.scss
--rw-rw-rw-   0        0        0     3946 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_pagination.scss
--rw-rw-rw-   0        0        0      859 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_placeholders.scss
--rw-rw-rw-   0        0        0     6907 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_popover.scss
--rw-rw-rw-   0        0        0     1875 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_progress.scss
--rw-rw-rw-   0        0        0    12311 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_reboot.scss
--rw-rw-rw-   0        0        0     2395 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_root.scss
--rw-rw-rw-   0        0        0     2429 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_spinners.scss
--rw-rw-rw-   0        0        0     4358 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tables.scss
--rw-rw-rw-   0        0        0     2381 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_toasts.scss
--rw-rw-rw-   0        0        0     3939 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tooltip.scss
--rw-rw-rw-   0        0        0      425 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_transitions.scss
--rw-rw-rw-   0        0        0     1420 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_type.scss
--rw-rw-rw-   0        0        0    14817 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_utilities.scss
--rw-rw-rw-   0        0        0    68533 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_variables.scss
--rw-rw-rw-   0        0        0     1198 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-grid.scss
--rw-rw-rw-   0        0        0      163 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-reboot.scss
--rw-rw-rw-   0        0        0      240 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-utilities.scss
--rw-rw-rw-   0        0        0      912 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap.scss
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.817531 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/
--rw-rw-rw-   0        0        0     2007 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_floating-labels.scss
--rw-rw-rw-   0        0        0     4287 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-check.scss
--rw-rw-rw-   0        0        0     5695 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-control.scss
--rw-rw-rw-   0        0        0     2796 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-range.scss
--rw-rw-rw-   0        0        0     2316 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-select.scss
--rw-rw-rw-   0        0        0      219 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-text.scss
--rw-rw-rw-   0        0        0     3812 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_input-group.scss
--rw-rw-rw-   0        0        0     1142 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_labels.scss
--rw-rw-rw-   0        0        0      478 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_validation.scss
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.823531 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/
--rw-rw-rw-   0        0        0       37 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_clearfix.scss
--rw-rw-rw-   0        0        0      454 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_color-bg.scss
--rw-rw-rw-   0        0        0      450 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_colored-links.scss
--rw-rw-rw-   0        0        0      621 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_position.scss
--rw-rw-rw-   0        0        0      399 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_ratio.scss
--rw-rw-rw-   0        0        0      245 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_stacks.scss
--rw-rw-rw-   0        0        0      223 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_stretched-link.scss
--rw-rw-rw-   0        0        0       73 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_text-truncation.scss
--rw-rw-rw-   0        0        0      136 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_visually-hidden.scss
--rw-rw-rw-   0        0        0      147 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_vr.scss
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.842291 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/
--rw-rw-rw-   0        0        0      393 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_alert.scss
--rw-rw-rw-   0        0        0      328 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_backdrop.scss
--rw-rw-rw-   0        0        0      275 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_banner.scss
--rw-rw-rw-   0        0        0     2031 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_border-radius.scss
--rw-rw-rw-   0        0        0      398 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_box-shadow.scss
--rw-rw-rw-   0        0        0     4580 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_breakpoints.scss
--rw-rw-rw-   0        0        0     3220 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_buttons.scss
--rw-rw-rw-   0        0        0     1473 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_caret.scss
--rw-rw-rw-   0        0        0      147 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_clearfix.scss
--rw-rw-rw-   0        0        0      167 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_color-scheme.scss
--rw-rw-rw-   0        0        0      410 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_container.scss
--rw-rw-rw-   0        0        0      613 2022-08-04 17:50:29.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_deprecate.scss
--rw-rw-rw-   0        0        0     4082 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_forms.scss
--rw-rw-rw-   0        0        0     1956 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_gradients.scss
--rw-rw-rw-   0        0        0     4726 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_grid.scss
--rw-rw-rw-   0        0        0      395 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_image.scss
--rw-rw-rw-   0        0        0      509 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_list-group.scss
--rw-rw-rw-   0        0        0      168 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_lists.scss
--rw-rw-rw-   0        0        0      387 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_pagination.scss
--rw-rw-rw-   0        0        0      495 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_reset-text.scss
--rw-rw-rw-   0        0        0      202 2022-08-04 17:50:29.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_resize.scss
--rw-rw-rw-   0        0        0     1089 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_table-variants.scss
--rw-rw-rw-   0        0        0      168 2022-08-04 17:50:29.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_text-truncate.scss
--rw-rw-rw-   0        0        0      661 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_transition.scss
--rw-rw-rw-   0        0        0     3379 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_utilities.scss
--rw-rw-rw-   0        0        0     1012 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_visually-hidden.scss
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.843291 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/utilities/
--rw-rw-rw-   0        0        0     1737 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/utilities/_api.scss
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.844299 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/vendor/
--rw-rw-rw-   0        0        0    10029 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/vendor/_rfs.scss
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.846393 coderedcms-2.0.0/coderedcms/templates/
--rw-rw-rw-   0        0        0      280 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/404.html
--rw-rw-rw-   0        0        0      725 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/500.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.595642 coderedcms-2.0.0/coderedcms/templates/coderedcms/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.880165 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/
--rw-rw-rw-   0        0        0     1129 2023-02-17 20:46:38.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/accordion_block.html
--rw-rw-rw-   0        0        0      778 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/article_block_card.html
--rw-rw-rw-   0        0        0      173 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/base_block.html
--rw-rw-rw-   0        0        0     1776 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/base_link_block.html
--rw-rw-rw-   0        0        0      617 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/button_block.html
--rw-rw-rw-   0        0        0      721 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/card_block.html
--rw-rw-rw-   0        0        0      827 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/card_blurb.html
--rw-rw-rw-   0        0        0      758 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/card_foot.html
--rw-rw-rw-   0        0        0      707 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/card_head.html
--rw-rw-rw-   0        0        0      744 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/card_head_foot.html
--rw-rw-rw-   0        0        0      762 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/card_img.html
--rw-rw-rw-   0        0        0      368 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/cardgrid_columns.html
--rw-rw-rw-   0        0        0      278 2023-02-17 20:46:38.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/cardgrid_deck.html
--rw-rw-rw-   0        0        0      262 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/cardgrid_group.html
--rw-rw-rw-   0        0        0     2141 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/carousel_block.html
--rw-rw-rw-   0        0        0      389 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/column_block.html
--rw-rw-rw-   0        0        0      833 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/content_wall_block.html
--rw-rw-rw-   0        0        0      141 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/document_link_block.html
--rw-rw-rw-   0        0        0      732 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/download_block.html
--rw-rw-rw-   0        0        0      105 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/embed_video_block.html
--rw-rw-rw-   0        0        0       99 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/external_link_block.html
--rw-rw-rw-   0        0        0      582 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/google_map.html
--rw-rw-rw-   0        0        0      374 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/grid_block.html
--rw-rw-rw-   0        0        0      198 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/h1_block.html
--rw-rw-rw-   0        0        0      198 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/h2_block.html
--rw-rw-rw-   0        0        0      198 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/h3_block.html
--rw-rw-rw-   0        0        0      833 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/hero_block.html
--rw-rw-rw-   0        0        0      286 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/image_block.html
--rw-rw-rw-   0        0        0     1170 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/image_gallery_block.html
--rw-rw-rw-   0        0        0      618 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/image_link_block.html
--rw-rw-rw-   0        0        0      992 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/modal_block.html
--rw-rw-rw-   0        0        0      167 2023-02-09 20:20:28.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/page_link_block.html
--rw-rw-rw-   0        0        0      444 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagelist_article_card_columns.html
--rw-rw-rw-   0        0        0      392 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagelist_article_card_deck.html
--rw-rw-rw-   0        0        0      324 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagelist_article_card_group.html
--rw-rw-rw-   0        0        0      903 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagelist_article_media.html
--rw-rw-rw-   0        0        0      394 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagelist_block.html
--rw-rw-rw-   0        0        0      561 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagelist_list_group.html
--rw-rw-rw-   0        0        0      279 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagepreview_block.html
--rw-rw-rw-   0        0        0      790 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagepreview_card.html
--rw-rw-rw-   0        0        0     1009 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagepreview_form.html
--rw-rw-rw-   0        0        0      227 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pricelist_block.html
--rw-rw-rw-   0        0        0      520 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pricelistitem_block.html
--rw-rw-rw-   0        0        0      337 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/quote_block.html
--rw-rw-rw-   0        0        0      258 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/reusable_content_block.html
--rw-rw-rw-   0        0        0       86 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/rich_text_block.html
--rw-rw-rw-   0        0        0      877 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/table_block.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.882165 coderedcms-2.0.0/coderedcms/templates/coderedcms/formfields/
--rw-rw-rw-   0        0        0      266 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/formfields/date.html
--rw-rw-rw-   0        0        0      410 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/formfields/datetime.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.883732 coderedcms-2.0.0/coderedcms/templates/coderedcms/formfields/mailchimp/
--rw-rw-rw-   0        0        0     6685 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_js.html
--rw-rw-rw-   0        0        0      793 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_widget.html
--rw-rw-rw-   0        0        0      263 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/formfields/time.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.898188 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/
--rw-rw-rw-   0        0        0      465 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-align-left.svg
--rw-rw-rw-   0        0        0      573 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-check-square-o.svg
--rw-rw-rw-   0        0        0      277 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-columns.svg
--rw-rw-rw-   0        0        0      359 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-desktop.svg
--rw-rw-rw-   0        0        0      571 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-font.svg
--rw-rw-rw-   0        0        0      292 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-google.svg
--rw-rw-rw-   0        0        0      813 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-hand-pointer-o.svg
--rw-rw-rw-   0        0        0      666 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-hashtag.svg
--rw-rw-rw-   0        0        0      840 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-header.svg
--rw-rw-rw-   0        0        0      835 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-list-alt.svg
--rw-rw-rw-   0        0        0      459 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-map.svg
--rw-rw-rw-   0        0        0      448 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-newspaper-o.svg
--rw-rw-rw-   0        0        0      721 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-puzzle-piece.svg
--rw-rw-rw-   0        0        0      635 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-recycle.svg
--rw-rw-rw-   0        0        0      174 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-stop.svg
--rw-rw-rw-   0        0        0      505 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-th-large.svg
--rw-rw-rw-   0        0        0      762 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-universal-access.svg
--rw-rw-rw-   0        0        0      548 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-usd.svg
--rw-rw-rw-   0        0        0      225 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-window-maximize.svg
--rw-rw-rw-   0        0        0      199 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-window-minimize.svg
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.903304 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/
--rw-rw-rw-   0        0        0      714 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/classifier_dropdowns.html
--rw-rw-rw-   0        0        0      534 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/classifier_nav.html
--rw-rw-rw-   0        0        0      296 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/crx_banner.html
--rw-rw-rw-   0        0        0      262 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/form_honeypot.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.906022 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/ical/
--rw-rw-rw-   0        0        0      531 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/ical/calendar.html
--rw-rw-rw-   0        0        0      365 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/ical/calendar_ical_button.html
--rw-rw-rw-   0        0        0      406 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/ical/recurring_ical_button.html
--rw-rw-rw-   0        0        0      565 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/ical/single_ical_button.html
--rw-rw-rw-   0        0        0      261 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/iframe_gmap.html
--rw-rw-rw-   0        0        0      320 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/map_list_description.html
--rw-rw-rw-   0        0        0      107 2022-08-04 15:54:45.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/map_pin_description.html
--rw-rw-rw-   0        0        0      983 2023-02-17 20:46:38.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/pagination.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.906022 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/stream_forms/
--rw-rw-rw-   0        0        0      533 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/stream_forms/render_field.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.918966 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/
--rw-rw-rw-   0        0        0     1513 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/article_index_page.html
--rw-rw-rw-   0        0        0     1251 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/article_page.html
--rw-rw-rw-   0        0        0     1081 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/article_page.search.html
--rw-rw-rw-   0        0        0     7491 2023-02-17 22:51:24.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/base.html
--rw-rw-rw-   0        0        0     1962 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/event_index_page.html
--rw-rw-rw-   0        0        0     1846 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/event_page.html
--rw-rw-rw-   0        0        0     1001 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/form_page.html
--rw-rw-rw-   0        0        0      244 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/form_page_landing.html
--rw-rw-rw-   0        0        0       55 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/home_page.html
--rw-rw-rw-   0        0        0     1580 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/location_index_page.html
--rw-rw-rw-   0        0        0      858 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/location_page.html
--rw-rw-rw-   0        0        0     2605 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/search.html
--rw-rw-rw-   0        0        0      417 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/search_result.html
--rw-rw-rw-   0        0        0     2525 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/stream_form_page.html
--rw-rw-rw-   0        0        0      515 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/web_page.html
--rw-rw-rw-   0        0        0      605 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/web_page_notitle.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.919966 coderedcms-2.0.0/coderedcms/templates/coderedcms/snippets/
--rw-rw-rw-   0        0        0      471 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/snippets/footer.html
--rw-rw-rw-   0        0        0     2411 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/snippets/navbar.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.920966 coderedcms-2.0.0/coderedcms/templates/coderedcms/widgets/
--rw-rw-rw-   0        0        0     1180 2023-02-27 16:56:29.000000 coderedcms-2.0.0/coderedcms/templates/coderedcms/widgets/checkbox_classifiers.html
--rw-rw-rw-   0        0        0      118 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/robots.txt
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.922966 coderedcms-2.0.0/coderedcms/templates/wagtailadmin/
--rw-rw-rw-   0        0        0      715 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/wagtailadmin/base.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.922966 coderedcms-2.0.0/coderedcms/templates/wagtailadmin/block_forms/
--rw-rw-rw-   0        0        0      716 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
--rw-rw-rw-   0        0        0       95 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/wagtailadmin/home.html
--rw-rw-rw-   0        0        0      177 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/wagtailadmin/login.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.924270 coderedcms-2.0.0/coderedcms/templates/wagtailcore/
--rw-rw-rw-   0        0        0      692 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/wagtailcore/password_required.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.925274 coderedcms-2.0.0/coderedcms/templates/wagtailembeds/
--rw-rw-rw-   0        0        0      522 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templates/wagtailembeds/embed_frontend.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.925274 coderedcms-2.0.0/coderedcms/templates/wagtailforms/
--rw-rw-rw-   0        0        0     1528 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/wagtailforms/list_submissions.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.927563 coderedcms-2.0.0/coderedcms/templates/wagtailimportexport/
--rw-rw-rw-   0        0        0     1396 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/wagtailimportexport/import_from_csv.html
--rw-rw-rw-   0        0        0      470 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/templates/wagtailimportexport/index.html
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.927563 coderedcms-2.0.0/coderedcms/templatetags/
--rw-rw-rw-   0        0        0     5877 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/templatetags/coderedcms_tags.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.932839 coderedcms-2.0.0/coderedcms/tests/
--rw-rw-rw-   0        0        0     5191 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/tests/settings.py
--rw-rw-rw-   0        0        0     2807 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/tests/test_bin.py
--rw-rw-rw-   0        0        0     1593 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/tests/test_templates.py
--rw-rw-rw-   0        0        0      821 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/tests/test_templatetags.py
--rw-rw-rw-   0        0        0    12221 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/tests/test_urls.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.933838 coderedcms-2.0.0/coderedcms/tests/testapp/
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.943972 coderedcms-2.0.0/coderedcms/tests/testapp/migrations/
--rw-rw-rw-   0        0        0   267269 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1481 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0002_initial.py
--rw-rw-rw-   0        0        0   250426 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0003_eventindexpage_eventoccurrence_eventpage_locationindexpage_locationpage.py
--rw-rw-rw-   0        0        0   101517 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0004_streamformconfirmemail_streamformpage.py
--rw-rw-rw-   0        0        0   346621 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0005_auto_20210908_1741.py
--rw-rw-rw-   0        0        0      770 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0006_indextestpage.py
--rw-rw-rw-   0        0        0     1011 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0007_auto_20210910_1614.py
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/tests/testapp/migrations/__init__.py
--rw-rw-rw-   0        0        0     3991 2023-02-17 20:46:38.000000 coderedcms-2.0.0/coderedcms/tests/testapp/models.py
--rw-rw-rw-   0        0        0      519 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/tests/urls.py
--rw-rw-rw-   0        0        0     1470 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/urls.py
--rw-rw-rw-   0        0        0     1390 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/utils.py
--rw-rw-rw-   0        0        0    10337 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/views.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.947552 coderedcms-2.0.0/coderedcms/wagtail_flexible_forms/
--rw-rw-rw-   0        0        0     1506 2022-08-03 20:24:51.000000 coderedcms-2.0.0/coderedcms/wagtail_flexible_forms/LICENSE
--rw-rw-rw-   0        0        0     7670 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/wagtail_flexible_forms/blocks.py
--rw-rw-rw-   0        0        0     1191 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/wagtail_flexible_forms/edit_handlers.py
--rw-rw-rw-   0        0        0    30401 2023-02-27 16:56:29.000000 coderedcms-2.0.0/coderedcms/wagtail_flexible_forms/models.py
--rw-rw-rw-   0        0        0    12527 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/wagtail_flexible_forms/wagtail_hooks.py
--rw-rw-rw-   0        0        0     4893 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/wagtail_hooks.py
--rw-rw-rw-   0        0        0     1473 2023-02-09 20:20:29.000000 coderedcms-2.0.0/coderedcms/widgets.py
-drwxrwxrwx   0        0        0        0 2023-02-27 19:47:13.615413 coderedcms-2.0.0/coderedcms.egg-info/
--rw-rw-rw-   0        0        0     5776 2023-02-27 19:47:13.000000 coderedcms-2.0.0/coderedcms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    25410 2023-02-27 19:47:13.000000 coderedcms-2.0.0/coderedcms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 19:47:13.000000 coderedcms-2.0.0/coderedcms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-02-27 19:47:13.000000 coderedcms-2.0.0/coderedcms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-08-04 17:39:55.000000 coderedcms-2.0.0/coderedcms.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      186 2023-02-27 19:47:13.000000 coderedcms-2.0.0/coderedcms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-27 19:47:13.000000 coderedcms-2.0.0/coderedcms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      299 2023-02-09 20:20:29.000000 coderedcms-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      384 2023-02-27 19:47:13.948885 coderedcms-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2229 2023-02-27 16:56:29.000000 coderedcms-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.201327 coderedcms-2.1.0/
+-rw-rw-rw-   0        0        0     1985 2022-08-03 20:24:51.000000 coderedcms-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0       94 2022-08-03 20:24:51.000000 coderedcms-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5776 2023-04-21 16:43:51.202323 coderedcms-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4358 2023-02-09 20:20:28.000000 coderedcms-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.936037 coderedcms-2.1.0/coderedcms/
+-rw-rw-rw-   0        0        0      827 2023-04-21 16:43:10.000000 coderedcms-2.1.0/coderedcms/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/admin_urls.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.941952 coderedcms-2.1.0/coderedcms/api/
+-rw-rw-rw-   0        0        0     2996 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/api/mailchimp.py
+-rw-rw-rw-   0        0        0      331 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.943957 coderedcms-2.1.0/coderedcms/bin/
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/bin/__init__.py
+-rw-rw-rw-   0        0        0     5239 2023-03-30 17:43:55.000000 coderedcms-2.1.0/coderedcms/bin/coderedcms.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.946957 coderedcms-2.1.0/coderedcms/blocks/
+-rw-rw-rw-   0        0        0     4985 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/blocks/__init__.py
+-rw-rw-rw-   0        0        0     8987 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/blocks/base_blocks.py
+-rw-rw-rw-   0        0        0     7688 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/blocks/content_blocks.py
+-rw-rw-rw-   0        0        0     8137 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/blocks/html_blocks.py
+-rw-rw-rw-   0        0        0     2828 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/blocks/layout_blocks.py
+-rw-rw-rw-   0        0        0     3856 2023-02-17 20:46:38.000000 coderedcms-2.1.0/coderedcms/blocks/stream_form_blocks.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.947956 coderedcms-2.1.0/coderedcms/blocks/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/blocks/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/blocks/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3201 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/fields.py
+-rw-rw-rw-   0        0        0     5856 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/forms.py
+-rw-rw-rw-   0        0        0     5656 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/importexport.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.972006 coderedcms-2.1.0/coderedcms/migrations/
+-rw-rw-rw-   0        0        0    31791 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1460 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0002_auto_20180829_1538.py
+-rw-rw-rw-   0        0        0     1445 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0003_auto_20180912_1632.py
+-rw-rw-rw-   0        0        0     1160 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0004_auto_20181119_1507.py
+-rw-rw-rw-   0        0        0     2371 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0005_auto_20181214_2214.py
+-rw-rw-rw-   0        0        0      945 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0006_mailchimpapisettings.py
+-rw-rw-rw-   0        0        0      514 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0007_auto_20190114_1515.py
+-rw-rw-rw-   0        0        0     1108 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0008_auto_20190122_1242.py
+-rw-rw-rw-   0        0        0      825 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0009_auto_20190201_1546.py
+-rw-rw-rw-   0        0        0     1108 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0010_auto_20190320_1231.py
+-rw-rw-rw-   0        0        0      618 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0010_generalsettings_email.py
+-rw-rw-rw-   0        0        0      340 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0010_remove_generalsettings_robots.py
+-rw-rw-rw-   0        0        0      293 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0011_merge_20190322_1309.py
+-rw-rw-rw-   0        0        0      280 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0012_merge_20190322_1324.py
+-rw-rw-rw-   0        0        0     1328 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0013_pagepreview_templates.py
+-rw-rw-rw-   0        0        0     3846 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0014_classifiers.py
+-rw-rw-rw-   0        0        0     2799 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0015_coderedsessionformsubmission_coderedsubmissionrevision.py
+-rw-rw-rw-   0        0        0     1363 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0016_auto_20191025_1620.py
+-rw-rw-rw-   0        0        0      460 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0017_generalsettings_external_new_tab.py
+-rw-rw-rw-   0        0        0     1341 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0018_auto_20200805_1702.py
+-rw-rw-rw-   0        0        0     1502 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0019_spelling_corrections.py
+-rw-rw-rw-   0        0        0      997 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0020_auto_20210527_1030.py
+-rw-rw-rw-   0        0        0      838 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0021_auto_20210730_1637.py
+-rw-rw-rw-   0        0        0     1508 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0022_auto_20210731_1853.py
+-rw-rw-rw-   0        0        0     1372 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0023_auto_20210908_1702.py
+-rw-rw-rw-   0        0        0     1059 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0024_analyticssettings.py
+-rw-rw-rw-   0        0        0      311 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0025_delete_socialmediasettings.py
+-rw-rw-rw-   0        0        0     1336 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0026_auto_20220513_1627.py
+-rw-rw-rw-   0        0        0      608 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0027_auto_20220603_1142.py
+-rw-rw-rw-   0        0        0     1915 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0028_auto_20220609_1532.py
+-rw-rw-rw-   0        0        0     3522 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0029_multinavs.py
+-rw-rw-rw-   0        0        0      587 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/0030_alter_coderedtag_tag.py
+-rw-rw-rw-   0        0        0     1840 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0031_wagtail3.py
+-rw-rw-rw-   0        0        0     1784 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0032_accordion_accordionpanel.py
+-rw-rw-rw-   0        0        0     2680 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0033_alter_coderedpage_struct_org_actions_and_more.py
+-rw-rw-rw-   0        0        0      488 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0033_remove_carousel_animation_and_more.py
+-rw-rw-rw-   0        0        0      319 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0034_delete_adasettings.py
+-rw-rw-rw-   0        0        0     3367 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/migrations/0035_remove_googleapisettings_site_and_more.py
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.975540 coderedcms-2.1.0/coderedcms/models/
+-rw-rw-rw-   0        0        0      323 2022-08-08 22:16:02.000000 coderedcms-2.1.0/coderedcms/models/__init__.py
+-rw-rw-rw-   0        0        0     6389 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/models/integration_models.py
+-rw-rw-rw-   0        0        0    68481 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/models/page_models.py
+-rw-rw-rw-   0        0        0    12803 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/models/snippet_models.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.977536 coderedcms-2.1.0/coderedcms/models/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/models/tests/__init__.py
+-rw-rw-rw-   0        0        0     4844 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/models/tests/test_navbars_and_footers.py
+-rw-rw-rw-   0        0        0     9007 2023-02-17 22:51:24.000000 coderedcms-2.1.0/coderedcms/models/tests/test_page_models.py
+-rw-rw-rw-   0        0        0     1953 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/models/tests/test_wagtailsettings_models.py
+-rw-rw-rw-   0        0        0    10637 2023-03-30 17:43:55.000000 coderedcms-2.1.0/coderedcms/models/wagtailsettings_models.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.913880 coderedcms-2.1.0/coderedcms/project_template/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.981682 coderedcms-2.1.0/coderedcms/project_template/basic/
+-rw-rw-rw-   0        0        0      722 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/basic/.editorconfig
+-rw-rw-rw-   0        0        0      364 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/basic/.gitattributes
+-rw-rw-rw-   0        0        0     5823 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/basic/.gitignore
+-rw-rw-rw-   0        0        0      932 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/basic/README.md
+-rw-rw-rw-   0        0        0      279 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/basic/manage.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.983704 coderedcms-2.1.0/coderedcms/project_template/basic/project_name/
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/basic/project_name/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.986239 coderedcms-2.1.0/coderedcms/project_template/basic/project_name/settings/
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/basic/project_name/settings/__init__.py
+-rw-rw-rw-   0        0        0     5291 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/basic/project_name/settings/base.py
+-rw-rw-rw-   0        0        0      388 2023-03-30 17:43:55.000000 coderedcms-2.1.0/coderedcms/project_template/basic/project_name/settings/dev.py
+-rw-rw-rw-   0        0        0     1307 2023-03-30 17:43:55.000000 coderedcms-2.1.0/coderedcms/project_template/basic/project_name/settings/prod.py
+-rw-rw-rw-   0        0        0     1223 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/basic/project_name/urls.py
+-rw-rw-rw-   0        0        0      438 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/basic/project_name/wsgi.py
+-rw-rw-rw-   0        0        0      119 2023-03-30 17:43:55.000000 coderedcms-2.1.0/coderedcms/project_template/basic/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.987762 coderedcms-2.1.0/coderedcms/project_template/basic/website/
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/basic/website/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/basic/website/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.990270 coderedcms-2.1.0/coderedcms/project_template/basic/website/migrations/
+-rw-rw-rw-   0        0        0   259938 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/project_template/basic/website/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1552 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/basic/website/migrations/0002_initial_data.py
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/basic/website/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-04-13 22:58:30.000000 coderedcms-2.1.0/coderedcms/project_template/basic/website/models.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.911855 coderedcms-2.1.0/coderedcms/project_template/basic/website/static/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.912869 coderedcms-2.1.0/coderedcms/project_template/basic/website/static/website/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.990270 coderedcms-2.1.0/coderedcms/project_template/basic/website/static/website/css/
+-rw-rw-rw-   0        0        0      219 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/basic/website/static/website/css/custom.css
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.991275 coderedcms-2.1.0/coderedcms/project_template/basic/website/static/website/js/
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/basic/website/static/website/js/custom.js
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.912869 coderedcms-2.1.0/coderedcms/project_template/basic/website/templates/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.912869 coderedcms-2.1.0/coderedcms/project_template/basic/website/templates/coderedcms/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.991275 coderedcms-2.1.0/coderedcms/project_template/basic/website/templates/coderedcms/pages/
+-rw-rw-rw-   0        0        0      392 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/basic/website/templates/coderedcms/pages/base.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.996279 coderedcms-2.1.0/coderedcms/project_template/sass/
+-rw-rw-rw-   0        0        0      722 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/sass/.editorconfig
+-rw-rw-rw-   0        0        0      364 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/sass/.gitattributes
+-rw-rw-rw-   0        0        0     5823 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/sass/.gitignore
+-rw-rw-rw-   0        0        0     1399 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/sass/README.md
+-rw-rw-rw-   0        0        0      279 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/sass/manage.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.997299 coderedcms-2.1.0/coderedcms/project_template/sass/project_name/
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/sass/project_name/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.000279 coderedcms-2.1.0/coderedcms/project_template/sass/project_name/settings/
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/sass/project_name/settings/__init__.py
+-rw-rw-rw-   0        0        0     5131 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/sass/project_name/settings/base.py
+-rw-rw-rw-   0        0        0      438 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/sass/project_name/settings/dev.py
+-rw-rw-rw-   0        0        0     1307 2023-03-30 17:43:55.000000 coderedcms-2.1.0/coderedcms/project_template/sass/project_name/settings/prod.py
+-rw-rw-rw-   0        0        0     1223 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/sass/project_name/urls.py
+-rw-rw-rw-   0        0        0      438 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/sass/project_name/wsgi.py
+-rw-rw-rw-   0        0        0       44 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/sass/requirements-dev.txt
+-rw-rw-rw-   0        0        0      251 2023-03-30 17:43:55.000000 coderedcms-2.1.0/coderedcms/project_template/sass/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.001280 coderedcms-2.1.0/coderedcms/project_template/sass/website/
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/sass/website/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/sass/website/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.003285 coderedcms-2.1.0/coderedcms/project_template/sass/website/migrations/
+-rw-rw-rw-   0        0        0   259938 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/project_template/sass/website/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1552 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/sass/website/migrations/0002_initial_data.py
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/sass/website/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/sass/website/models.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.914879 coderedcms-2.1.0/coderedcms/project_template/sass/website/static/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.914879 coderedcms-2.1.0/coderedcms/project_template/sass/website/static/website/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.004280 coderedcms-2.1.0/coderedcms/project_template/sass/website/static/website/js/
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/project_template/sass/website/static/website/js/custom.js
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.005280 coderedcms-2.1.0/coderedcms/project_template/sass/website/static/website/src/
+-rw-rw-rw-   0        0        0     1974 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/sass/website/static/website/src/_variables.scss
+-rw-rw-rw-   0        0        0     1001 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/sass/website/static/website/src/custom.scss
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.914879 coderedcms-2.1.0/coderedcms/project_template/sass/website/templates/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.914879 coderedcms-2.1.0/coderedcms/project_template/sass/website/templates/coderedcms/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.005280 coderedcms-2.1.0/coderedcms/project_template/sass/website/templates/coderedcms/pages/
+-rw-rw-rw-   0        0        0      913 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/project_template/sass/website/templates/coderedcms/pages/base.html
+-rw-rw-rw-   0        0        0      125 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/search_urls.py
+-rw-rw-rw-   0        0        0     9360 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.914879 coderedcms-2.1.0/coderedcms/static/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.915879 coderedcms-2.1.0/coderedcms/static/coderedcms/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.009300 coderedcms-2.1.0/coderedcms/static/coderedcms/css/
+-rw-rw-rw-   0        0        0      971 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/css/crx-admin.css
+-rw-rw-rw-   0        0        0      886 2023-03-30 17:43:55.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/css/crx-editor.css
+-rw-rw-rw-   0        0        0     5401 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/css/crx-front.css
+-rw-rw-rw-   0        0        0     5363 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/css/crx-front.css.map
+-rw-rw-rw-   0        0        0     4428 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/css/crx-front.min.css
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.012391 coderedcms-2.1.0/coderedcms/static/coderedcms/js/
+-rw-rw-rw-   0        0        0      716 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/js/crx-editor.js
+-rw-rw-rw-   0        0        0     1522 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/js/crx-events.js
+-rw-rw-rw-   0        0        0     4496 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/js/crx-front.js
+-rw-rw-rw-   0        0        0     5255 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/js/crx-maps.js
+-rw-rw-rw-   0        0        0     1805 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/js/crx-streamforms.js
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.017762 coderedcms-2.1.0/coderedcms/static/coderedcms/scss/
+-rw-rw-rw-   0        0        0      205 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/scss/_crx-article.scss
+-rw-rw-rw-   0        0        0      367 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/scss/_crx-bs-overrides.scss
+-rw-rw-rw-   0        0        0      152 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/scss/_crx-gallery.scss
+-rw-rw-rw-   0        0        0      318 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/scss/_crx-hero.scss
+-rw-rw-rw-   0        0        0     1749 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/scss/_crx-location.scss
+-rw-rw-rw-   0        0        0     1988 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/scss/_crx-navbar.scss
+-rw-rw-rw-   0        0        0      818 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/scss/_crx-pricelist.scss
+-rw-rw-rw-   0        0        0      222 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/scss/_crx-richtext.scss
+-rw-rw-rw-   0        0        0      403 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/scss/crx-front.scss
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.915879 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.018765 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/
+-rw-rw-rw-   0        0        0     1131 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/LICENSE
+-rw-rw-rw-   0        0        0      130 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.916879 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.043489 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/
+-rw-rw-rw-   0        0        0    71861 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0   210292 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0    53265 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0   131408 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css.map
+-rw-rw-rw-   0        0        0    71935 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css
+-rw-rw-rw-   0        0        0   210296 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css.map
+-rw-rw-rw-   0        0        0    53340 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css
+-rw-rw-rw-   0        0        0   131485 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-rw-   0        0        0     7965 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0   110811 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0     6490 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0    40345 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css.map
+-rw-rw-rw-   0        0        0     7958 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css
+-rw-rw-rw-   0        0        0   110824 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
+-rw-rw-rw-   0        0        0     6562 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
+-rw-rw-rw-   0        0        0    48707 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-rw-   0        0        0    74135 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0   196370 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css.map
+-rw-rw-rw-   0        0        0    56365 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css
+-rw-rw-rw-   0        0        0   115601 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css.map
+-rw-rw-rw-   0        0        0    74002 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css
+-rw-rw-rw-   0        0        0   196313 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
+-rw-rw-rw-   0        0        0    56293 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
+-rw-rw-rw-   0        0        0   115436 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-rw-   0        0        0   237872 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css
+-rw-rw-rw-   0        0        0   606249 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   194699 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   521459 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0   237386 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css
+-rw-rw-rw-   0        0        0   606069 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css.map
+-rw-rw-rw-   0        0        0   194803 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css
+-rw-rw-rw-   0        0        0   765329 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css.map
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.053877 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/
+-rw-rw-rw-   0        0        0   207083 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0   448881 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js.map
+-rw-rw-rw-   0        0        0    79790 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   330849 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0   135367 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js
+-rw-rw-rw-   0        0        0   306814 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js.map
+-rw-rw-rw-   0        0        0    73539 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js
+-rw-rw-rw-   0        0        0   220143 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js.map
+-rw-rw-rw-   0        0        0   144701 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js
+-rw-rw-rw-   0        0        0   307954 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js.map
+-rw-rw-rw-   0        0        0    60104 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0   215897 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js.map
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.916879 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.062133 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/
+-rw-rw-rw-   0        0        0     3801 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/alert.js
+-rw-rw-rw-   0        0        0     6341 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/button.js
+-rw-rw-rw-   0        0        0    16583 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/carousel.js
+-rw-rw-rw-   0        0        0    10333 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/collapse.js
+-rw-rw-rw-   0        0        0    14736 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dropdown.js
+-rw-rw-rw-   0        0        0      773 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/index.js
+-rw-rw-rw-   0        0        0    17563 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/modal.js
+-rw-rw-rw-   0        0        0     4275 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/popover.js
+-rw-rw-rw-   0        0        0     8777 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/scrollspy.js
+-rw-rw-rw-   0        0        0     6635 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tab.js
+-rw-rw-rw-   0        0        0     5178 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/toast.js
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.063110 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tools/
+-rw-rw-rw-   0        0        0     3368 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tools/sanitizer.js
+-rw-rw-rw-   0        0        0    18705 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tooltip.js
+-rw-rw-rw-   0        0        0     5334 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util.js
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.089489 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/
+-rw-rw-rw-   0        0        0     4757 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_accordion.scss
+-rw-rw-rw-   0        0        0     2126 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_alert.scss
+-rw-rw-rw-   0        0        0     1118 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_badge.scss
+-rw-rw-rw-   0        0        0     1751 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_breadcrumb.scss
+-rw-rw-rw-   0        0        0     3060 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_button-group.scss
+-rw-rw-rw-   0        0        0     5959 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_buttons.scss
+-rw-rw-rw-   0        0        0     6736 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_card.scss
+-rw-rw-rw-   0        0        0     5625 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_carousel.scss
+-rw-rw-rw-   0        0        0     1127 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_close.scss
+-rw-rw-rw-   0        0        0     1201 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_containers.scss
+-rw-rw-rw-   0        0        0     7950 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_dropdown.scss
+-rw-rw-rw-   0        0        0      256 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_forms.scss
+-rw-rw-rw-   0        0        0    10552 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_functions.scss
+-rw-rw-rw-   0        0        0      575 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_grid.scss
+-rw-rw-rw-   0        0        0      294 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_helpers.scss
+-rw-rw-rw-   0        0        0     1158 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_images.scss
+-rw-rw-rw-   0        0        0     6348 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_list-group.scss
+-rw-rw-rw-   0        0        0     1648 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_maps.scss
+-rw-rw-rw-   0        0        0      899 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_mixins.scss
+-rw-rw-rw-   0        0        0     7762 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_modal.scss
+-rw-rw-rw-   0        0        0     4665 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_nav.scss
+-rw-rw-rw-   0        0        0     8854 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_navbar.scss
+-rw-rw-rw-   0        0        0     4485 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_offcanvas.scss
+-rw-rw-rw-   0        0        0     3946 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_pagination.scss
+-rw-rw-rw-   0        0        0      859 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_placeholders.scss
+-rw-rw-rw-   0        0        0     6907 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_popover.scss
+-rw-rw-rw-   0        0        0     1875 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_progress.scss
+-rw-rw-rw-   0        0        0    12311 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_reboot.scss
+-rw-rw-rw-   0        0        0     2395 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_root.scss
+-rw-rw-rw-   0        0        0     2429 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_spinners.scss
+-rw-rw-rw-   0        0        0     4358 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tables.scss
+-rw-rw-rw-   0        0        0     2381 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_toasts.scss
+-rw-rw-rw-   0        0        0     3939 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tooltip.scss
+-rw-rw-rw-   0        0        0      425 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_transitions.scss
+-rw-rw-rw-   0        0        0     1420 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_type.scss
+-rw-rw-rw-   0        0        0    14817 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_utilities.scss
+-rw-rw-rw-   0        0        0    68533 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_variables.scss
+-rw-rw-rw-   0        0        0     1198 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-grid.scss
+-rw-rw-rw-   0        0        0      163 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-reboot.scss
+-rw-rw-rw-   0        0        0      240 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-utilities.scss
+-rw-rw-rw-   0        0        0      912 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap.scss
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.094761 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/
+-rw-rw-rw-   0        0        0     2007 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_floating-labels.scss
+-rw-rw-rw-   0        0        0     4287 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-check.scss
+-rw-rw-rw-   0        0        0     5695 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-control.scss
+-rw-rw-rw-   0        0        0     2796 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-range.scss
+-rw-rw-rw-   0        0        0     2316 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-select.scss
+-rw-rw-rw-   0        0        0      219 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-text.scss
+-rw-rw-rw-   0        0        0     3812 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_input-group.scss
+-rw-rw-rw-   0        0        0     1142 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_labels.scss
+-rw-rw-rw-   0        0        0      478 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_validation.scss
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.100765 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/
+-rw-rw-rw-   0        0        0       37 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_clearfix.scss
+-rw-rw-rw-   0        0        0      454 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_color-bg.scss
+-rw-rw-rw-   0        0        0      450 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_colored-links.scss
+-rw-rw-rw-   0        0        0      621 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_position.scss
+-rw-rw-rw-   0        0        0      399 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_ratio.scss
+-rw-rw-rw-   0        0        0      245 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_stacks.scss
+-rw-rw-rw-   0        0        0      223 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_stretched-link.scss
+-rw-rw-rw-   0        0        0       73 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_text-truncation.scss
+-rw-rw-rw-   0        0        0      136 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_visually-hidden.scss
+-rw-rw-rw-   0        0        0      147 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_vr.scss
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.116822 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/
+-rw-rw-rw-   0        0        0      393 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_alert.scss
+-rw-rw-rw-   0        0        0      328 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_backdrop.scss
+-rw-rw-rw-   0        0        0      275 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_banner.scss
+-rw-rw-rw-   0        0        0     2031 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_border-radius.scss
+-rw-rw-rw-   0        0        0      398 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_box-shadow.scss
+-rw-rw-rw-   0        0        0     4580 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_breakpoints.scss
+-rw-rw-rw-   0        0        0     3220 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_buttons.scss
+-rw-rw-rw-   0        0        0     1473 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_caret.scss
+-rw-rw-rw-   0        0        0      147 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_clearfix.scss
+-rw-rw-rw-   0        0        0      167 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_color-scheme.scss
+-rw-rw-rw-   0        0        0      410 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_container.scss
+-rw-rw-rw-   0        0        0      613 2022-08-04 17:50:29.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_deprecate.scss
+-rw-rw-rw-   0        0        0     4082 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_forms.scss
+-rw-rw-rw-   0        0        0     1956 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_gradients.scss
+-rw-rw-rw-   0        0        0     4726 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_grid.scss
+-rw-rw-rw-   0        0        0      395 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_image.scss
+-rw-rw-rw-   0        0        0      509 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_list-group.scss
+-rw-rw-rw-   0        0        0      168 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_lists.scss
+-rw-rw-rw-   0        0        0      387 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_pagination.scss
+-rw-rw-rw-   0        0        0      495 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_reset-text.scss
+-rw-rw-rw-   0        0        0      202 2022-08-04 17:50:29.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_resize.scss
+-rw-rw-rw-   0        0        0     1089 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_table-variants.scss
+-rw-rw-rw-   0        0        0      168 2022-08-04 17:50:29.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_text-truncate.scss
+-rw-rw-rw-   0        0        0      661 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_transition.scss
+-rw-rw-rw-   0        0        0     3379 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_utilities.scss
+-rw-rw-rw-   0        0        0     1012 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_visually-hidden.scss
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.117822 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/utilities/
+-rw-rw-rw-   0        0        0     1737 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/utilities/_api.scss
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.117822 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/vendor/
+-rw-rw-rw-   0        0        0    10029 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/vendor/_rfs.scss
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.119872 coderedcms-2.1.0/coderedcms/templates/
+-rw-rw-rw-   0        0        0      280 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/404.html
+-rw-rw-rw-   0        0        0      725 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/500.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.921881 coderedcms-2.1.0/coderedcms/templates/coderedcms/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.147083 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/
+-rw-rw-rw-   0        0        0     1129 2023-02-17 20:46:38.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/accordion_block.html
+-rw-rw-rw-   0        0        0      778 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/article_block_card.html
+-rw-rw-rw-   0        0        0      173 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/base_block.html
+-rw-rw-rw-   0        0        0     1776 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/base_link_block.html
+-rw-rw-rw-   0        0        0      617 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/button_block.html
+-rw-rw-rw-   0        0        0      721 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/card_block.html
+-rw-rw-rw-   0        0        0      827 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/card_blurb.html
+-rw-rw-rw-   0        0        0      758 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/card_foot.html
+-rw-rw-rw-   0        0        0      707 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/card_head.html
+-rw-rw-rw-   0        0        0      744 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/card_head_foot.html
+-rw-rw-rw-   0        0        0      762 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/card_img.html
+-rw-rw-rw-   0        0        0      368 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/cardgrid_columns.html
+-rw-rw-rw-   0        0        0      278 2023-02-17 20:46:38.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/cardgrid_deck.html
+-rw-rw-rw-   0        0        0      262 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/cardgrid_group.html
+-rw-rw-rw-   0        0        0     2141 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/carousel_block.html
+-rw-rw-rw-   0        0        0      389 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/column_block.html
+-rw-rw-rw-   0        0        0      833 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/content_wall_block.html
+-rw-rw-rw-   0        0        0      141 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/document_link_block.html
+-rw-rw-rw-   0        0        0      732 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/download_block.html
+-rw-rw-rw-   0        0        0      105 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/embed_video_block.html
+-rw-rw-rw-   0        0        0       99 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/external_link_block.html
+-rw-rw-rw-   0        0        0      582 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/google_map.html
+-rw-rw-rw-   0        0        0      374 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/grid_block.html
+-rw-rw-rw-   0        0        0      198 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/h1_block.html
+-rw-rw-rw-   0        0        0      198 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/h2_block.html
+-rw-rw-rw-   0        0        0      198 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/h3_block.html
+-rw-rw-rw-   0        0        0      833 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/hero_block.html
+-rw-rw-rw-   0        0        0      286 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/image_block.html
+-rw-rw-rw-   0        0        0     1170 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/image_gallery_block.html
+-rw-rw-rw-   0        0        0      618 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/image_link_block.html
+-rw-rw-rw-   0        0        0      992 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/modal_block.html
+-rw-rw-rw-   0        0        0      167 2023-02-09 20:20:28.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/page_link_block.html
+-rw-rw-rw-   0        0        0      444 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagelist_article_card_columns.html
+-rw-rw-rw-   0        0        0      392 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagelist_article_card_deck.html
+-rw-rw-rw-   0        0        0      324 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagelist_article_card_group.html
+-rw-rw-rw-   0        0        0      903 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagelist_article_media.html
+-rw-rw-rw-   0        0        0      394 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagelist_block.html
+-rw-rw-rw-   0        0        0      561 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagelist_list_group.html
+-rw-rw-rw-   0        0        0      279 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagepreview_block.html
+-rw-rw-rw-   0        0        0      790 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagepreview_card.html
+-rw-rw-rw-   0        0        0     1009 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagepreview_form.html
+-rw-rw-rw-   0        0        0      227 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pricelist_block.html
+-rw-rw-rw-   0        0        0      520 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pricelistitem_block.html
+-rw-rw-rw-   0        0        0      337 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/quote_block.html
+-rw-rw-rw-   0        0        0      258 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/reusable_content_block.html
+-rw-rw-rw-   0        0        0       86 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/rich_text_block.html
+-rw-rw-rw-   0        0        0      877 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/table_block.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.149649 coderedcms-2.1.0/coderedcms/templates/coderedcms/formfields/
+-rw-rw-rw-   0        0        0      266 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/formfields/date.html
+-rw-rw-rw-   0        0        0      410 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/formfields/datetime.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.150678 coderedcms-2.1.0/coderedcms/templates/coderedcms/formfields/mailchimp/
+-rw-rw-rw-   0        0        0     6685 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_js.html
+-rw-rw-rw-   0        0        0      793 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_widget.html
+-rw-rw-rw-   0        0        0      263 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/formfields/time.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.163793 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/
+-rw-rw-rw-   0        0        0      465 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-align-left.svg
+-rw-rw-rw-   0        0        0      573 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-check-square-o.svg
+-rw-rw-rw-   0        0        0      277 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-columns.svg
+-rw-rw-rw-   0        0        0      359 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-desktop.svg
+-rw-rw-rw-   0        0        0      571 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-font.svg
+-rw-rw-rw-   0        0        0      292 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-google.svg
+-rw-rw-rw-   0        0        0      813 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-hand-pointer-o.svg
+-rw-rw-rw-   0        0        0      666 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-hashtag.svg
+-rw-rw-rw-   0        0        0      840 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-header.svg
+-rw-rw-rw-   0        0        0      835 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-list-alt.svg
+-rw-rw-rw-   0        0        0      459 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-map.svg
+-rw-rw-rw-   0        0        0      448 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-newspaper-o.svg
+-rw-rw-rw-   0        0        0      721 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-puzzle-piece.svg
+-rw-rw-rw-   0        0        0      635 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-recycle.svg
+-rw-rw-rw-   0        0        0      174 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-stop.svg
+-rw-rw-rw-   0        0        0      505 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-th-large.svg
+-rw-rw-rw-   0        0        0      762 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-universal-access.svg
+-rw-rw-rw-   0        0        0      548 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-usd.svg
+-rw-rw-rw-   0        0        0      225 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-window-maximize.svg
+-rw-rw-rw-   0        0        0      199 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-window-minimize.svg
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.168333 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/
+-rw-rw-rw-   0        0        0      714 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/classifier_dropdowns.html
+-rw-rw-rw-   0        0        0      534 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/classifier_nav.html
+-rw-rw-rw-   0        0        0      296 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/crx_banner.html
+-rw-rw-rw-   0        0        0      262 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/form_honeypot.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.170339 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/ical/
+-rw-rw-rw-   0        0        0      531 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/ical/calendar.html
+-rw-rw-rw-   0        0        0      365 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/ical/calendar_ical_button.html
+-rw-rw-rw-   0        0        0      406 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/ical/recurring_ical_button.html
+-rw-rw-rw-   0        0        0      565 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/ical/single_ical_button.html
+-rw-rw-rw-   0        0        0      261 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/iframe_gmap.html
+-rw-rw-rw-   0        0        0      320 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/map_list_description.html
+-rw-rw-rw-   0        0        0      107 2022-08-04 15:54:45.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/map_pin_description.html
+-rw-rw-rw-   0        0        0      983 2023-03-30 19:10:04.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/pagination.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.171344 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/stream_forms/
+-rw-rw-rw-   0        0        0      533 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/stream_forms/render_field.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.180917 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/
+-rw-rw-rw-   0        0        0     1513 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/article_index_page.html
+-rw-rw-rw-   0        0        0     1251 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/article_page.html
+-rw-rw-rw-   0        0        0     1081 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/article_page.search.html
+-rw-rw-rw-   0        0        0     7491 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/base.html
+-rw-rw-rw-   0        0        0     1962 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/event_index_page.html
+-rw-rw-rw-   0        0        0     1846 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/event_page.html
+-rw-rw-rw-   0        0        0     1001 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/form_page.html
+-rw-rw-rw-   0        0        0      244 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/form_page_landing.html
+-rw-rw-rw-   0        0        0       55 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/home_page.html
+-rw-rw-rw-   0        0        0     1580 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/location_index_page.html
+-rw-rw-rw-   0        0        0      858 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/location_page.html
+-rw-rw-rw-   0        0        0     2605 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/search.html
+-rw-rw-rw-   0        0        0      417 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/search_result.html
+-rw-rw-rw-   0        0        0     2525 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/stream_form_page.html
+-rw-rw-rw-   0        0        0      515 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/web_page.html
+-rw-rw-rw-   0        0        0      605 2023-04-21 16:42:39.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/web_page_notitle.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.181921 coderedcms-2.1.0/coderedcms/templates/coderedcms/snippets/
+-rw-rw-rw-   0        0        0      471 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/snippets/footer.html
+-rw-rw-rw-   0        0        0     2411 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/snippets/navbar.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.181921 coderedcms-2.1.0/coderedcms/templates/coderedcms/widgets/
+-rw-rw-rw-   0        0        0     1180 2023-03-30 17:43:55.000000 coderedcms-2.1.0/coderedcms/templates/coderedcms/widgets/checkbox_classifiers.html
+-rw-rw-rw-   0        0        0      118 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/robots.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.183853 coderedcms-2.1.0/coderedcms/templates/wagtailadmin/
+-rw-rw-rw-   0        0        0      715 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/wagtailadmin/base.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.184863 coderedcms-2.1.0/coderedcms/templates/wagtailadmin/block_forms/
+-rw-rw-rw-   0        0        0      716 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-rw-rw-   0        0        0       95 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/wagtailadmin/home.html
+-rw-rw-rw-   0        0        0      177 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/wagtailadmin/login.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.184863 coderedcms-2.1.0/coderedcms/templates/wagtailcore/
+-rw-rw-rw-   0        0        0      692 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/wagtailcore/password_required.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.185859 coderedcms-2.1.0/coderedcms/templates/wagtailembeds/
+-rw-rw-rw-   0        0        0      522 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/templates/wagtailembeds/embed_frontend.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.185859 coderedcms-2.1.0/coderedcms/templates/wagtailforms/
+-rw-rw-rw-   0        0        0     1528 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/wagtailforms/list_submissions.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.187887 coderedcms-2.1.0/coderedcms/templates/wagtailimportexport/
+-rw-rw-rw-   0        0        0     1396 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/wagtailimportexport/import_from_csv.html
+-rw-rw-rw-   0        0        0      470 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/templates/wagtailimportexport/index.html
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.187887 coderedcms-2.1.0/coderedcms/templatetags/
+-rw-rw-rw-   0        0        0     5877 2023-04-13 21:16:09.000000 coderedcms-2.1.0/coderedcms/templatetags/coderedcms_tags.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.191183 coderedcms-2.1.0/coderedcms/tests/
+-rw-rw-rw-   0        0        0     5191 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/tests/settings.py
+-rw-rw-rw-   0        0        0     2807 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/tests/test_bin.py
+-rw-rw-rw-   0        0        0     1593 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/tests/test_templates.py
+-rw-rw-rw-   0        0        0      821 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/tests/test_templatetags.py
+-rw-rw-rw-   0        0        0    12221 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/tests/test_urls.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.192189 coderedcms-2.1.0/coderedcms/tests/testapp/
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.198322 coderedcms-2.1.0/coderedcms/tests/testapp/migrations/
+-rw-rw-rw-   0        0        0   267269 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1481 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0002_initial.py
+-rw-rw-rw-   0        0        0   250426 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0003_eventindexpage_eventoccurrence_eventpage_locationindexpage_locationpage.py
+-rw-rw-rw-   0        0        0   101517 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0004_streamformconfirmemail_streamformpage.py
+-rw-rw-rw-   0        0        0   346621 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0005_auto_20210908_1741.py
+-rw-rw-rw-   0        0        0      770 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0006_indextestpage.py
+-rw-rw-rw-   0        0        0     1011 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0007_auto_20210910_1614.py
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/tests/testapp/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3991 2023-02-17 20:46:38.000000 coderedcms-2.1.0/coderedcms/tests/testapp/models.py
+-rw-rw-rw-   0        0        0      519 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/tests/urls.py
+-rw-rw-rw-   0        0        0     1470 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/urls.py
+-rw-rw-rw-   0        0        0     1390 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/utils.py
+-rw-rw-rw-   0        0        0    10337 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/views.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:51.201327 coderedcms-2.1.0/coderedcms/wagtail_flexible_forms/
+-rw-rw-rw-   0        0        0     1506 2022-08-03 20:24:51.000000 coderedcms-2.1.0/coderedcms/wagtail_flexible_forms/LICENSE
+-rw-rw-rw-   0        0        0     7670 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/wagtail_flexible_forms/blocks.py
+-rw-rw-rw-   0        0        0     1191 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/wagtail_flexible_forms/edit_handlers.py
+-rw-rw-rw-   0        0        0    30401 2023-03-30 17:43:55.000000 coderedcms-2.1.0/coderedcms/wagtail_flexible_forms/models.py
+-rw-rw-rw-   0        0        0    12527 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/wagtail_flexible_forms/wagtail_hooks.py
+-rw-rw-rw-   0        0        0     4893 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/wagtail_hooks.py
+-rw-rw-rw-   0        0        0     1473 2023-02-09 20:20:29.000000 coderedcms-2.1.0/coderedcms/widgets.py
+drwxrwxrwx   0        0        0        0 2023-04-21 16:43:50.941952 coderedcms-2.1.0/coderedcms.egg-info/
+-rw-rw-rw-   0        0        0     5776 2023-04-21 16:43:50.000000 coderedcms-2.1.0/coderedcms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    25410 2023-04-21 16:43:50.000000 coderedcms-2.1.0/coderedcms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 16:43:50.000000 coderedcms-2.1.0/coderedcms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-04-21 16:43:50.000000 coderedcms-2.1.0/coderedcms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-08-04 17:39:55.000000 coderedcms-2.1.0/coderedcms.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      186 2023-04-21 16:43:50.000000 coderedcms-2.1.0/coderedcms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-21 16:43:50.000000 coderedcms-2.1.0/coderedcms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      299 2023-02-09 20:20:29.000000 coderedcms-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      384 2023-04-21 16:43:51.202323 coderedcms-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2229 2023-03-30 17:43:55.000000 coderedcms-2.1.0/setup.py
```

### Comparing `coderedcms-2.0.0/LICENSE` & `coderedcms-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/PKG-INFO` & `coderedcms-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coderedcms
-Version: 2.0.0
+Version: 2.1.0
 Summary: Wagtail-based CMS by CodeRed for building marketing websites.
 Home-page: https://github.com/coderedcorp/coderedcms
 Author: CodeRed LLC
 Author-email: info@coderedcorp.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `coderedcms-2.0.0/README.md` & `coderedcms-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/__init__.py` & `coderedcms-2.1.0/coderedcms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 5th element is for dev/post releases. Leave blank for stable releases.
 
     X.Y.Z.devN   # Development release
     X.Y.Z.postN  # Post release (e.g. docs changes but no actual code changes)
 
 See: https://www.python.org/dev/peps/pep-0440/
 """
-release = ["2", "0", "0", "", ""]
+release = ["2", "1", "0", "", ""]
 
 
 def _get_version() -> str:
     v = "{0}.{1}.{2}".format(release[0], release[1], release[2])
     if release[3]:
         v = "{0}{1}".format(v, release[3])
     if release[4]:
```

### Comparing `coderedcms-2.0.0/coderedcms/api/mailchimp.py` & `coderedcms-2.1.0/coderedcms/api/mailchimp.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/bin/coderedcms.py` & `coderedcms-2.1.0/coderedcms/bin/coderedcms.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/blocks/__init__.py` & `coderedcms-2.1.0/coderedcms/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/blocks/base_blocks.py` & `coderedcms-2.1.0/coderedcms/blocks/base_blocks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/blocks/content_blocks.py` & `coderedcms-2.1.0/coderedcms/blocks/content_blocks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/blocks/html_blocks.py` & `coderedcms-2.1.0/coderedcms/blocks/html_blocks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/blocks/layout_blocks.py` & `coderedcms-2.1.0/coderedcms/blocks/layout_blocks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/blocks/stream_form_blocks.py` & `coderedcms-2.1.0/coderedcms/blocks/stream_form_blocks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/fields.py` & `coderedcms-2.1.0/coderedcms/fields.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/forms.py` & `coderedcms-2.1.0/coderedcms/forms.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/importexport.py` & `coderedcms-2.1.0/coderedcms/importexport.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0001_initial.py` & `coderedcms-2.1.0/coderedcms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0002_auto_20180829_1538.py` & `coderedcms-2.1.0/coderedcms/migrations/0002_auto_20180829_1538.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0003_auto_20180912_1632.py` & `coderedcms-2.1.0/coderedcms/migrations/0003_auto_20180912_1632.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0004_auto_20181119_1507.py` & `coderedcms-2.1.0/coderedcms/migrations/0004_auto_20181119_1507.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0005_auto_20181214_2214.py` & `coderedcms-2.1.0/coderedcms/migrations/0005_auto_20181214_2214.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0006_mailchimpapisettings.py` & `coderedcms-2.1.0/coderedcms/migrations/0006_mailchimpapisettings.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0007_auto_20190114_1515.py` & `coderedcms-2.1.0/coderedcms/migrations/0007_auto_20190114_1515.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0008_auto_20190122_1242.py` & `coderedcms-2.1.0/coderedcms/migrations/0008_auto_20190122_1242.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0009_auto_20190201_1546.py` & `coderedcms-2.1.0/coderedcms/migrations/0009_auto_20190201_1546.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0010_auto_20190320_1231.py` & `coderedcms-2.1.0/coderedcms/migrations/0010_auto_20190320_1231.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0010_generalsettings_email.py` & `coderedcms-2.1.0/coderedcms/migrations/0010_generalsettings_email.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0013_pagepreview_templates.py` & `coderedcms-2.1.0/coderedcms/migrations/0013_pagepreview_templates.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0014_classifiers.py` & `coderedcms-2.1.0/coderedcms/migrations/0014_classifiers.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0015_coderedsessionformsubmission_coderedsubmissionrevision.py` & `coderedcms-2.1.0/coderedcms/migrations/0015_coderedsessionformsubmission_coderedsubmissionrevision.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0016_auto_20191025_1620.py` & `coderedcms-2.1.0/coderedcms/migrations/0016_auto_20191025_1620.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0018_auto_20200805_1702.py` & `coderedcms-2.1.0/coderedcms/migrations/0018_auto_20200805_1702.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0019_spelling_corrections.py` & `coderedcms-2.1.0/coderedcms/migrations/0019_spelling_corrections.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0020_auto_20210527_1030.py` & `coderedcms-2.1.0/coderedcms/migrations/0020_auto_20210527_1030.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0021_auto_20210730_1637.py` & `coderedcms-2.1.0/coderedcms/migrations/0021_auto_20210730_1637.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0022_auto_20210731_1853.py` & `coderedcms-2.1.0/coderedcms/migrations/0022_auto_20210731_1853.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0023_auto_20210908_1702.py` & `coderedcms-2.1.0/coderedcms/migrations/0023_auto_20210908_1702.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0024_analyticssettings.py` & `coderedcms-2.1.0/coderedcms/migrations/0024_analyticssettings.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0026_auto_20220513_1627.py` & `coderedcms-2.1.0/coderedcms/migrations/0026_auto_20220513_1627.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0027_auto_20220603_1142.py` & `coderedcms-2.1.0/coderedcms/migrations/0027_auto_20220603_1142.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0028_auto_20220609_1532.py` & `coderedcms-2.1.0/coderedcms/migrations/0028_auto_20220609_1532.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0029_multinavs.py` & `coderedcms-2.1.0/coderedcms/migrations/0029_multinavs.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0030_alter_coderedtag_tag.py` & `coderedcms-2.1.0/coderedcms/migrations/0030_alter_coderedtag_tag.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0031_wagtail3.py` & `coderedcms-2.1.0/coderedcms/migrations/0031_wagtail3.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0032_accordion_accordionpanel.py` & `coderedcms-2.1.0/coderedcms/migrations/0032_accordion_accordionpanel.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0033_alter_coderedpage_struct_org_actions_and_more.py` & `coderedcms-2.1.0/coderedcms/migrations/0033_alter_coderedpage_struct_org_actions_and_more.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/migrations/0035_remove_googleapisettings_site_and_more.py` & `coderedcms-2.1.0/coderedcms/migrations/0035_remove_googleapisettings_site_and_more.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/models/integration_models.py` & `coderedcms-2.1.0/coderedcms/models/integration_models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/models/page_models.py` & `coderedcms-2.1.0/coderedcms/models/page_models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/models/snippet_models.py` & `coderedcms-2.1.0/coderedcms/models/snippet_models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/models/tests/test_navbars_and_footers.py` & `coderedcms-2.1.0/coderedcms/models/tests/test_navbars_and_footers.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/models/tests/test_page_models.py` & `coderedcms-2.1.0/coderedcms/models/tests/test_page_models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/models/tests/test_wagtailsettings_models.py` & `coderedcms-2.1.0/coderedcms/models/tests/test_wagtailsettings_models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/models/wagtailsettings_models.py` & `coderedcms-2.1.0/coderedcms/models/wagtailsettings_models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/basic/.editorconfig` & `coderedcms-2.1.0/coderedcms/project_template/basic/.editorconfig`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/basic/.gitignore` & `coderedcms-2.1.0/coderedcms/project_template/basic/.gitignore`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/basic/README.md` & `coderedcms-2.1.0/coderedcms/project_template/basic/README.md`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/basic/project_name/settings/base.py` & `coderedcms-2.1.0/coderedcms/project_template/basic/project_name/settings/base.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/basic/project_name/settings/prod.py` & `coderedcms-2.1.0/coderedcms/project_template/basic/project_name/settings/prod.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/basic/project_name/urls.py` & `coderedcms-2.1.0/coderedcms/project_template/basic/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/basic/website/migrations/0001_initial.py` & `coderedcms-2.1.0/coderedcms/project_template/basic/website/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/basic/website/migrations/0002_initial_data.py` & `coderedcms-2.1.0/coderedcms/project_template/basic/website/migrations/0002_initial_data.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/basic/website/models.py` & `coderedcms-2.1.0/coderedcms/project_template/basic/website/models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/sass/.editorconfig` & `coderedcms-2.1.0/coderedcms/project_template/sass/.editorconfig`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/sass/.gitignore` & `coderedcms-2.1.0/coderedcms/project_template/sass/.gitignore`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/sass/README.md` & `coderedcms-2.1.0/coderedcms/project_template/sass/README.md`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/sass/project_name/settings/base.py` & `coderedcms-2.1.0/coderedcms/project_template/sass/project_name/settings/base.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/sass/project_name/settings/prod.py` & `coderedcms-2.1.0/coderedcms/project_template/sass/project_name/settings/prod.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/sass/project_name/urls.py` & `coderedcms-2.1.0/coderedcms/project_template/sass/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/sass/website/migrations/0001_initial.py` & `coderedcms-2.1.0/coderedcms/project_template/sass/website/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/sass/website/migrations/0002_initial_data.py` & `coderedcms-2.1.0/coderedcms/project_template/sass/website/migrations/0002_initial_data.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/sass/website/models.py` & `coderedcms-2.1.0/coderedcms/project_template/sass/website/models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/sass/website/static/website/src/_variables.scss` & `coderedcms-2.1.0/coderedcms/project_template/sass/website/static/website/src/_variables.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/sass/website/static/website/src/custom.scss` & `coderedcms-2.1.0/coderedcms/project_template/sass/website/static/website/src/custom.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/project_template/sass/website/templates/coderedcms/pages/base.html` & `coderedcms-2.1.0/coderedcms/project_template/sass/website/templates/coderedcms/pages/base.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/settings.py` & `coderedcms-2.1.0/coderedcms/settings.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/css/crx-admin.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/css/crx-admin.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/css/crx-editor.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/css/crx-editor.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/css/crx-front.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/css/crx-front.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/css/crx-front.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/css/crx-front.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/css/crx-front.min.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/css/crx-front.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/js/crx-editor.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/js/crx-editor.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/js/crx-events.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/js/crx-events.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/js/crx-front.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/js/crx-front.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/js/crx-maps.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/js/crx-maps.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/js/crx-streamforms.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/js/crx-streamforms.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/scss/_crx-location.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/scss/_crx-location.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/scss/_crx-navbar.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/scss/_crx-navbar.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/scss/_crx-pricelist.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/scss/_crx-pricelist.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/LICENSE` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js.map` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/alert.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/alert.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/button.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/button.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/carousel.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/carousel.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/collapse.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/collapse.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dropdown.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dropdown.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/index.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/index.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/modal.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/modal.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/popover.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/popover.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/scrollspy.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/scrollspy.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tab.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tab.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/toast.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/toast.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tools/sanitizer.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tools/sanitizer.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tooltip.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tooltip.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util.js` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util.js`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_accordion.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_alert.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_badge.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_breadcrumb.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_button-group.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_buttons.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_card.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_carousel.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_close.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_containers.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_dropdown.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_functions.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_grid.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_images.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_list-group.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_maps.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_maps.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_mixins.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_modal.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_nav.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_navbar.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_offcanvas.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_pagination.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_placeholders.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_popover.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_progress.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_reboot.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_root.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_spinners.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tables.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_toasts.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tooltip.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_type.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_utilities.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_variables.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-grid.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_floating-labels.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-check.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-control.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-range.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-select.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_input-group.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_labels.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_position.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_border-radius.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_breakpoints.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_buttons.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_caret.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_deprecate.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_forms.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_gradients.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_grid.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_table-variants.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_transition.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_utilities.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_visually-hidden.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/utilities/_api.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/vendor/_rfs.scss` & `coderedcms-2.1.0/coderedcms/static/coderedcms/vendor/bootstrap/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/500.html` & `coderedcms-2.1.0/coderedcms/templates/500.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/accordion_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/accordion_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/article_block_card.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/article_block_card.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/base_link_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/base_link_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/button_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/button_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/card_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/card_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/card_blurb.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/card_blurb.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/card_foot.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/card_foot.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/card_head.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/card_head.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/card_head_foot.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/card_head_foot.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/card_img.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/card_img.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/carousel_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/carousel_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/content_wall_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/content_wall_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/download_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/download_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/google_map.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/google_map.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/hero_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/hero_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/image_gallery_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/image_gallery_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/image_link_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/image_link_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/modal_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/modal_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagelist_article_media.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagelist_article_media.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagelist_list_group.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagelist_list_group.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagepreview_card.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagepreview_card.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pagepreview_form.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pagepreview_form.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/pricelistitem_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/pricelistitem_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/blocks/table_block.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/blocks/table_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_js.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_widget.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_widget.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-check-square-o.svg` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-check-square-o.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-font.svg` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-font.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-hand-pointer-o.svg` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-hand-pointer-o.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-hashtag.svg` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-hashtag.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-header.svg` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-header.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-list-alt.svg` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-list-alt.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-puzzle-piece.svg` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-puzzle-piece.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-recycle.svg` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-recycle.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-universal-access.svg` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-universal-access.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/icons/cr-usd.svg` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/icons/cr-usd.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/classifier_dropdowns.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/classifier_dropdowns.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/classifier_nav.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/classifier_nav.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/ical/calendar.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/ical/calendar.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/ical/single_ical_button.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/ical/single_ical_button.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/pagination.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/includes/stream_forms/render_field.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/includes/stream_forms/render_field.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/article_index_page.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/article_index_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/article_page.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/article_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/article_page.search.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/article_page.search.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/base.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/base.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/event_index_page.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/event_index_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/event_page.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/event_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/form_page.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/form_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/location_index_page.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/location_index_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/location_page.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/location_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/search.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/search.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/stream_form_page.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/stream_form_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/web_page.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/web_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/pages/web_page_notitle.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/pages/web_page_notitle.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/snippets/navbar.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/snippets/navbar.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/coderedcms/widgets/checkbox_classifiers.html` & `coderedcms-2.1.0/coderedcms/templates/coderedcms/widgets/checkbox_classifiers.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/wagtailadmin/base.html` & `coderedcms-2.1.0/coderedcms/templates/wagtailadmin/base.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `coderedcms-2.1.0/coderedcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/wagtailcore/password_required.html` & `coderedcms-2.1.0/coderedcms/templates/wagtailcore/password_required.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/wagtailembeds/embed_frontend.html` & `coderedcms-2.1.0/coderedcms/templates/wagtailembeds/embed_frontend.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/wagtailforms/list_submissions.html` & `coderedcms-2.1.0/coderedcms/templates/wagtailforms/list_submissions.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templates/wagtailimportexport/import_from_csv.html` & `coderedcms-2.1.0/coderedcms/templates/wagtailimportexport/import_from_csv.html`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/templatetags/coderedcms_tags.py` & `coderedcms-2.1.0/coderedcms/templatetags/coderedcms_tags.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/settings.py` & `coderedcms-2.1.0/coderedcms/tests/settings.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/test_bin.py` & `coderedcms-2.1.0/coderedcms/tests/test_bin.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/test_templates.py` & `coderedcms-2.1.0/coderedcms/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/test_templatetags.py` & `coderedcms-2.1.0/coderedcms/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/test_urls.py` & `coderedcms-2.1.0/coderedcms/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0001_initial.py` & `coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0002_initial.py` & `coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0003_eventindexpage_eventoccurrence_eventpage_locationindexpage_locationpage.py` & `coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0003_eventindexpage_eventoccurrence_eventpage_locationindexpage_locationpage.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0004_streamformconfirmemail_streamformpage.py` & `coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0004_streamformconfirmemail_streamformpage.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0005_auto_20210908_1741.py` & `coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0005_auto_20210908_1741.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0006_indextestpage.py` & `coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0006_indextestpage.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/testapp/migrations/0007_auto_20210910_1614.py` & `coderedcms-2.1.0/coderedcms/tests/testapp/migrations/0007_auto_20210910_1614.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/testapp/models.py` & `coderedcms-2.1.0/coderedcms/tests/testapp/models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/tests/urls.py` & `coderedcms-2.1.0/coderedcms/tests/urls.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/urls.py` & `coderedcms-2.1.0/coderedcms/urls.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/utils.py` & `coderedcms-2.1.0/coderedcms/utils.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/views.py` & `coderedcms-2.1.0/coderedcms/views.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/wagtail_flexible_forms/LICENSE` & `coderedcms-2.1.0/coderedcms/wagtail_flexible_forms/LICENSE`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/wagtail_flexible_forms/blocks.py` & `coderedcms-2.1.0/coderedcms/wagtail_flexible_forms/blocks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/wagtail_flexible_forms/edit_handlers.py` & `coderedcms-2.1.0/coderedcms/wagtail_flexible_forms/edit_handlers.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/wagtail_flexible_forms/models.py` & `coderedcms-2.1.0/coderedcms/wagtail_flexible_forms/models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/wagtail_flexible_forms/wagtail_hooks.py` & `coderedcms-2.1.0/coderedcms/wagtail_flexible_forms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/wagtail_hooks.py` & `coderedcms-2.1.0/coderedcms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms/widgets.py` & `coderedcms-2.1.0/coderedcms/widgets.py`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/coderedcms.egg-info/PKG-INFO` & `coderedcms-2.1.0/coderedcms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coderedcms
-Version: 2.0.0
+Version: 2.1.0
 Summary: Wagtail-based CMS by CodeRed for building marketing websites.
 Home-page: https://github.com/coderedcorp/coderedcms
 Author: CodeRed LLC
 Author-email: info@coderedcorp.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `coderedcms-2.0.0/coderedcms.egg-info/SOURCES.txt` & `coderedcms-2.1.0/coderedcms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coderedcms-2.0.0/setup.py` & `coderedcms-2.1.0/setup.py`

 * *Files identical despite different names*

