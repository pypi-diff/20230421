# Comparing `tmp/impsparc-2.0.2.tar.gz` & `tmp/impsparc-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impsparc-2.0.2.tar", last modified: Mon Apr 17 16:25:04 2023, max compression
+gzip compressed data, was "impsparc-2.0.4.tar", last modified: Fri Apr 21 13:34:59 2023, max compression
```

## Comparing `impsparc-2.0.2.tar` & `impsparc-2.0.4.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.560164 impsparc-2.0.2/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1064 2023-04-06 04:16:23.000000 impsparc-2.0.2/LICENSE.md
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      244 2023-04-06 04:16:23.000000 impsparc-2.0.2/MANIFEST.in
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-04-17 16:25:04.559888 impsparc-2.0.2/PKG-INFO
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      626 2023-04-06 04:18:27.000000 impsparc-2.0.2/README.md
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.338197 impsparc-2.0.2/cvsvc_apirisk/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/__init__.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.357154 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   363678 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   262350 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      615 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      753 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23616 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16394 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16378 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.358863 impsparc-2.0.2/cvsvc_apirisk/score/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2914 2023-04-17 14:42:16.000000 impsparc-2.0.2/cvsvc_apirisk/score/base.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.370710 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       80 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    59992 2023-04-17 15:04:42.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1503 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.424161 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2433 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2453 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2662 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2684 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2697 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2117 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2387 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2385 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2393 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2391 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2722 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2731 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.472904 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2346 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2474 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2477 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2459 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2462 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2760 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3371 2023-04-17 15:04:03.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/json_line.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.488972 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2084 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2418 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2339 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2867 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2292 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2163 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     5713 2023-04-17 16:21:41.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2685 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2635 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2479 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2769 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.490411 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.333743 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.537608 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.544739 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15291 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16918 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15192 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    28781 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11370 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1363 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11350 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11421 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      966 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.556058 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      423 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16193 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      209 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3581 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3478 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3944 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      309 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      406 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6482 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     9574 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1212 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    88994 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.493009 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.330965 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.500709 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   207965 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      687 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      756 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2033 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.505305 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    59219 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   195090 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4023 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    56178 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.513775 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   100782 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   163872 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    80388 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11245 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      393 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.530448 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   181852 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   105536 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60520 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23940 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   388460 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   154228 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    10556 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4960 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6244 2023-04-17 15:01:30.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_common.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3358 2023-04-17 14:46:48.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_main.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    27120 2023-04-17 15:02:48.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_main_cr.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    14646 2023-04-17 15:02:09.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_spec_util.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1192 2023-04-17 15:03:29.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/yaml_line.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.559378 impsparc-2.0.2/impsparc.egg-info/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/PKG-INFO
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6777 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/SOURCES.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        1 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/dependency_links.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      164 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/entry_points.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      185 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/requires.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       14 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/top_level.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       38 2023-04-17 16:25:04.560245 impsparc-2.0.2/setup.cfg
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1196 2023-04-17 14:30:26.000000 impsparc-2.0.2/setup.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.823481 impsparc-2.0.4/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1064 2023-04-06 04:16:23.000000 impsparc-2.0.4/LICENSE.md
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      244 2023-04-06 04:16:23.000000 impsparc-2.0.4/MANIFEST.in
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-04-21 13:34:59.822923 impsparc-2.0.4/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      626 2023-04-06 04:18:27.000000 impsparc-2.0.4/README.md
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.629014 impsparc-2.0.4/cvsvc_apirisk/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/__init__.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.641939 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   363678 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   262350 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      615 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      753 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23616 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16394 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16378 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.644281 impsparc-2.0.4/cvsvc_apirisk/score/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2914 2023-04-17 14:42:16.000000 impsparc-2.0.4/cvsvc_apirisk/score/base.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.676888 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       80 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60112 2023-04-21 10:43:22.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1503 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.715713 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2433 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2453 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2662 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2684 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2697 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2117 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2387 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2385 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2393 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2391 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2722 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2731 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.726664 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2346 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2474 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2477 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2459 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2462 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2760 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3371 2023-04-17 15:04:03.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/json_line.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.744526 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2084 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2418 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2339 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2867 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2292 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2163 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     5713 2023-04-17 16:21:41.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2685 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2635 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2479 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2769 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.745782 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.622204 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.797361 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.802528 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15291 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16918 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15192 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    28781 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11370 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1363 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11350 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11421 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      966 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.815589 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      423 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16193 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      209 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3581 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3478 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3944 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      309 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      406 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6482 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     9574 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1212 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    88994 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.747992 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.620233 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.755218 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   207965 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      687 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      756 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2033 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.761145 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    59219 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   195090 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4023 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    56178 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.770852 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   100782 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   163872 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    80388 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11245 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      393 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.789831 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   181852 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   105536 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60520 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23940 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   388460 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   154228 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    10556 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4960 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6244 2023-04-17 15:01:30.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_common.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3358 2023-04-17 14:46:48.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_main.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    27120 2023-04-17 15:02:48.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_main_cr.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    17455 2023-04-21 10:44:55.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_spec_util.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1192 2023-04-17 15:03:29.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/yaml_line.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.821898 impsparc-2.0.4/impsparc.egg-info/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-04-21 13:34:59.000000 impsparc-2.0.4/impsparc.egg-info/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6777 2023-04-21 13:34:59.000000 impsparc-2.0.4/impsparc.egg-info/SOURCES.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        1 2023-04-21 13:34:59.000000 impsparc-2.0.4/impsparc.egg-info/dependency_links.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      164 2023-04-21 13:34:59.000000 impsparc-2.0.4/impsparc.egg-info/entry_points.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      217 2023-04-21 13:34:59.000000 impsparc-2.0.4/impsparc.egg-info/requires.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       14 2023-04-21 13:34:59.000000 impsparc-2.0.4/impsparc.egg-info/top_level.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       38 2023-04-21 13:34:59.823638 impsparc-2.0.4/setup.cfg
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1250 2023-04-21 13:34:49.000000 impsparc-2.0.4/setup.py
```

### Comparing `impsparc-2.0.2/LICENSE.md` & `impsparc-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/PKG-INFO` & `impsparc-2.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 2.0.2
+Version: 2.0.4
 Summary: API Specification Analysis for Risks and Compliance
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `impsparc-2.0.2/README.md` & `impsparc-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf` & `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf` & `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json` & `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt` & `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip` & `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json` & `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json` & `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/base.py` & `impsparc-2.0.4/cvsvc_apirisk/score/base.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,37 +107,42 @@
 
             spec_main_cr.analyze_rules(rule_exps, abs_path=abs_path)
             spec_main = spec_main_cr.spec_main
 
             global RISK_CTGS, RISK_SUBCTGS
 
             RISK_CTGS, RISK_SUBCTGS = init_rules_ds(rule_exps)
+
+            param_node_names, data_types, op_node_names, response_node_names, response_code_count = spec_main.qspec.get_param_method_response_obj()
+
             report['files'][abs_path]['status'] = 'valid'
             report['files'][abs_path]['score'] = spec_main.score
             report['files'][abs_path]['meta'] = spec_main.meta
             report['files'][abs_path]['num_apis'] = \
                 len(spec_main.qspec.spec_obj['paths'])
             report['files'][abs_path]['num_params'] = \
-                len(spec_main.qspec.get_param_objs()[0])
+                len(param_node_names)
             report['files'][abs_path]['version'] = \
                 target_obj['raw_spec']['info']['version']
             report['files'][abs_path]['num_evaluations'] = \
                 spec_main_cr.num_evaluations
-            report['files'][abs_path]['req_method'] = spec_main.qspec.get_method_objs()
-            report['files'][abs_path]['response_codes'] = spec_main.qspec.get_response_objs()[1]
-            report['files'][abs_path]['data_types'] = spec_main.qspec.get_param_objs()[1]
+            report['files'][abs_path]['req_method'] = op_node_names
+            report['files'][abs_path]['response_codes'] = response_code_count
+            report['files'][abs_path]['data_types'] = data_types
 
             qspecs[abs_path] = spec_main.qspec
 
             # Init API data structures
             report['files'][abs_path]['apis'] = {}
             for api_url in spec_main.qspec.spec_obj['paths']:
                 api = abs_path.split('/')[-1] + ':' + api_url
                 init_api_ds(report, abs_path, api)
 
+            spec_main.qspec.node_id_mapping.close()
+
         except OpenAPIValidationError as e:
             report['files'][abs_path]['status'] = 'err'
             report['files'][abs_path]['meta'] = str(e)
             print('-> Error encountered for ', abs_path)
 
 
 def check_specs(spec_zip, cvrules_path, rules_path=None):
```

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/json_line.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/json_line.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_common.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_common.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_main.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_main.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_main_cr.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_main_cr.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_spec_util.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_spec_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python
 
 import sys
 from argparse import ArgumentParser
 from configparser import ConfigParser
 
 import networkit as nk
+from sqlitedict import SqliteDict
 
 
 PATH_OPS_v2 = ['get', 'put', 'post', 'delete', 'options', 'head', 'patch']
 
 
 class QuerySpec(object):
 
@@ -27,15 +28,15 @@
         -------
         result: int
             Result desc
         """
         self.ROOT_NODE = '#'
         self.spec_obj = spec_obj
         self.G = nk.Graph(directed=True)
-        self.node_id_mapping = dict()
+        self.node_id_mapping = None
 
         node_name_sp = self.G.attachNodeAttribute('nodenamesp', str)
         node_name_raw = self.G.attachNodeAttribute('nodenameraw', str)
         child_type = self.G.attachNodeAttribute('childtype', str)
 
         self.node_attributes = {'node_name_sp': node_name_sp,
                                 'node_name_raw': node_name_raw,
@@ -43,17 +44,75 @@
 
         self.load_spec2graph()
 
         self.create_node_id_key_mapping()
         # this variable to passed in get node index while querying node-id-mapping variable
         self.total_node_plus_ten = self.G.numberOfNodes() + 10
 
+
     def create_node_id_key_mapping(self):
+        self.node_id_mapping = SqliteDict("node_id_key_mapping.sqlite",
+                                          tablename='node_id_key_mapping',
+                                          outer_stack=False)
         for node in self.G.iterNodes():
             self.node_id_mapping[self.node_attributes['node_name_sp'][node]] = node
+        self.node_id_mapping.commit()
+    #     self.node_id_mapping.close()
+
+    # def create_node_id_key_mapping(self):
+    #     for node in self.G.iterNodes():
+    #         self.node_id_mapping[self.node_attributes['node_name_sp'][node]] = node
+
+
+    def get_param_method_response_obj(self):
+        param_node_names = []
+        data_types = {}
+        op_node_names = {}
+        response_node_names = []
+        response_code_count = {}
+        op_obj_list = self.get_op_objs_list()
+        for node in self.G.iterNodes():
+            nodename = self.node_attributes['node_name_raw'][node]
+            if nodename == 'parameters':
+                self.get_param_obj(node, param_node_names, data_types)
+            elif nodename == 'responses':
+                self.get_response_obj(node, response_node_names, response_code_count)
+            if nodename in op_obj_list:
+                if nodename in op_node_names:
+                    op_node_names[nodename] = op_node_names[nodename] + 1
+                else:
+                    op_node_names[nodename] = 1
+
+        return param_node_names, data_types, op_node_names, response_node_names, response_code_count
+
+    def get_param_obj(self, node, param_node_name, data_types):
+        for param_obj_node in self.G.iterNeighbors(node):
+            param_node_name.append(self.node_attributes['node_name_sp'][param_obj_node])
+            for param_list in self.G.iterNeighbors(param_obj_node):
+                if self.node_attributes['node_name_raw'][param_list] == 'type':
+                    for _type in self.G.iterNeighbors(param_list):
+                        param_type = self.node_attributes['node_name_sp'][_type]
+                        p_type = param_type.split('->')[-1]
+                        if p_type in data_types:
+                            data_types[p_type] = data_types[p_type] + 1
+                        else:
+                            data_types[p_type] = 1
+        return  param_node_name, data_types
+
+    def get_response_obj(self, node, response_node_names, response_code_count):
+        for n in self.G.iterNeighbors(node):
+            response_node_names.append(self.node_attributes['node_name_sp'][n])
+            response_code = self.node_attributes['node_name_raw'][n]
+            if response_code in response_code_count:
+                response_code_count[response_code] = response_code_count[response_code] + 1
+            else:
+                response_code_count[response_code] = 1
+
+        return response_node_names, response_code_count
+
 
     def get_desc_objs(self):
         """
         Description
 
         Params
         ------
@@ -112,17 +171,18 @@
         methods = self.get_op_objs()
         for method in methods:
             method_set.add(method.split('->')[-1])
         return list(method_set)
 
     def get_method_objs(self):
         node_names = {}
+        op_obj_list = self.get_op_objs_list()
         for node in self.G.iterNodes():
             nodename = self.node_attributes['node_name_raw'][node]
-            if nodename in self.get_op_objs_list():
+            if nodename in op_obj_list:
                 if nodename in node_names:
                     node_names[nodename] = node_names[nodename] + 1
                 else:
                     node_names[nodename] = 1
         return node_names
 
     def get_header_objs(self):
```

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/yaml_line.py` & `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/yaml_line.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/impsparc.egg-info/PKG-INFO` & `impsparc-2.0.4/impsparc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 2.0.2
+Version: 2.0.4
 Summary: API Specification Analysis for Risks and Compliance
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `impsparc-2.0.2/impsparc.egg-info/SOURCES.txt` & `impsparc-2.0.4/impsparc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/setup.py` & `impsparc-2.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impsparc",
-    version=os.environ.get("VER", "2.0.2"),
+    version=os.environ.get("VER", "2.0.4"),
     author="Priyank Chheda",
     author_email="priyank.chheda@imperva.com",
     description="API Specification Analysis for Risks and Compliance",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
@@ -31,10 +31,12 @@
         "numpy==1.22.3",
         "networkit==10.1",
         "parsimonious==0.8.1",
         "sanic==20.3.0",
         "jinja2==3.0.3",
         "idna==2.10",
         "PyYAML==6.0",
+        "sqlitedict==2.1.0",
+        "pandas==2.0.0",
     ],
     include_package_data=True,
 )
```

