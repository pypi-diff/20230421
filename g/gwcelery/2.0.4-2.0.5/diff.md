# Comparing `tmp/gwcelery-2.0.4.tar.gz` & `tmp/gwcelery-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwcelery-2.0.4.tar", max compression
+gzip compressed data, was "gwcelery-2.0.5.tar", max compression
```

## Comparing `gwcelery-2.0.4.tar` & `gwcelery-2.0.5.tar`

### file list

```diff
@@ -1,220 +1,225 @@
--rw-r--r--   0        0        0    87219 2023-03-29 01:10:32.519050 gwcelery-2.0.4/CHANGES.rst
--rw-r--r--   0        0        0       64 2023-03-29 01:10:32.519050 gwcelery-2.0.4/CONTRIBUTING.rst
--rw-r--r--   0        0        0    19716 2023-03-29 01:10:32.519050 gwcelery-2.0.4/LICENSE.rst
--rw-r--r--   0        0        0     1351 2023-03-29 01:10:32.519050 gwcelery-2.0.4/README.rst
--rw-r--r--   0        0        0      634 2023-03-29 01:10:32.519050 gwcelery-2.0.4/doc/Makefile
--rw-r--r--   0        0        0   191486 2023-03-29 01:10:32.520050 gwcelery-2.0.4/doc/_static/acceptance-tests-checklist.png
--rw-r--r--   0        0        0   241593 2023-03-29 01:10:32.521050 gwcelery-2.0.4/doc/_static/celeryevent-screenshot.png
--rw-r--r--   0        0        0   206465 2023-03-29 01:10:32.522050 gwcelery-2.0.4/doc/_static/deployment-screenshot.png
--rw-r--r--   0        0        0   161306 2023-03-29 01:10:32.523050 gwcelery-2.0.4/doc/_static/flask-screenshot.png
--rw-r--r--   0        0        0   328056 2023-03-29 01:10:32.525050 gwcelery-2.0.4/doc/_static/flower-screenshot.png
--rw-r--r--   0        0        0   114719 2023-03-29 01:10:32.526050 gwcelery-2.0.4/doc/_static/logo-0.5x.png
--rw-r--r--   0        0        0   351955 2023-03-29 01:10:32.527050 gwcelery-2.0.4/doc/_static/logo.png
--rw-r--r--   0        0        0   230777 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/_static/sentry-screenshot.png
--rwxr-xr-x   0        0        0     7356 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/conf.py
--rw-r--r--   0        0        0     3543 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/configuration.rst
--rw-r--r--   0        0        0     5698 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/contributing.rst
--rw-r--r--   0        0        0     7204 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/deployment.rst
--rw-r--r--   0        0        0    10176 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/design.rst
--rw-r--r--   0        0        0      486 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.conf.rst
--rw-r--r--   0        0        0      284 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.email.rst
--rw-r--r--   0        0        0      329 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.igwn_alert.rst
--rw-r--r--   0        0        0      227 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.rst
--rw-r--r--   0        0        0       79 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.sentry.rst
--rw-r--r--   0        0        0       97 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.alerts.rst
--rw-r--r--   0        0        0      103 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.bayestar.rst
--rw-r--r--   0        0        0      107 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.circulars.rst
--rw-r--r--   0        0        0       98 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.condor.rst
--rw-r--r--   0        0        0     2404 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.detchar.rst
--rw-r--r--   0        0        0     1110 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.em_bright.rst
--rw-r--r--   0        0        0      129 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.external_skymaps.rst
--rw-r--r--   0        0        0     6738 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.external_triggers.rst
--rw-r--r--   0        0        0      112 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.first2years.rst
--rw-r--r--   0        0        0       88 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.gcn.rst
--rw-r--r--   0        0        0      100 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.gracedb.rst
--rw-r--r--   0        0        0      109 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.igwn_alert.rst
--rw-r--r--   0        0        0      109 2023-03-29 01:10:32.529050 gwcelery-2.0.4/doc/gwcelery.tasks.inference.rst
--rw-r--r--   0        0        0     8111 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/gwcelery.tasks.orchestrator.rst
--rw-r--r--   0        0        0      100 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/gwcelery.tasks.p_astro.rst
--rw-r--r--   0        0        0       94 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/gwcelery.tasks.raven.rst
--rw-r--r--   0        0        0      628 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/gwcelery.tasks.rst
--rw-r--r--   0        0        0      100 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/gwcelery.tasks.skymaps.rst
--rw-r--r--   0        0        0     7161 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/gwcelery.tasks.superevents.rst
--rw-r--r--   0        0        0       97 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/gwcelery.tools.condor.rst
--rw-r--r--   0        0        0       94 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/gwcelery.tools.flask.rst
--rw-r--r--   0        0        0       97 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/gwcelery.tools.nagios.rst
--rw-r--r--   0        0        0      185 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/gwcelery.tools.rst
--rw-r--r--   0        0        0       73 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/gwcelery.util.rst
--rw-r--r--   0        0        0      507 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/gwcelery.voevent.rst
--rw-r--r--   0        0        0     3564 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/htcondor.rst
--rw-r--r--   0        0        0     1576 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/index.rst
--rw-r--r--   0        0        0      800 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/make.bat
--rw-r--r--   0        0        0     4416 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/monitoring.rst
--rw-r--r--   0        0        0     5312 2023-03-29 01:10:32.530050 gwcelery-2.0.4/doc/quickstart.rst
--rw-r--r--   0        0        0     1149 2023-03-29 01:10:32.530050 gwcelery-2.0.4/gwcelery/__init__.py
--rw-r--r--   0        0        0    18447 2023-03-29 01:10:32.530050 gwcelery-2.0.4/gwcelery/_version.py
--rw-r--r--   0        0        0    14415 2023-03-29 01:10:32.531050 gwcelery-2.0.4/gwcelery/conf/__init__.py
--rw-r--r--   0        0        0      403 2023-03-29 01:10:32.531050 gwcelery-2.0.4/gwcelery/conf/development.py
--rw-r--r--   0        0        0     1026 2023-03-29 01:10:32.531050 gwcelery-2.0.4/gwcelery/conf/minikube.py
--rw-r--r--   0        0        0     1562 2023-03-29 01:10:32.531050 gwcelery-2.0.4/gwcelery/conf/playground.py
--rw-r--r--   0        0        0     3024 2023-03-29 01:10:32.531050 gwcelery-2.0.4/gwcelery/conf/production.py
--rw-r--r--   0        0        0     1044 2023-03-29 01:10:32.531050 gwcelery-2.0.4/gwcelery/conf/test.py
--rw-r--r--   0        0        0        0 2023-03-29 01:10:32.531050 gwcelery-2.0.4/gwcelery/data/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 01:10:32.531050 gwcelery-2.0.4/gwcelery/data/first2years/__init__.py
--rw-r--r--   0        0        0   731421 2023-03-29 01:10:32.533050 gwcelery-2.0.4/gwcelery/data/first2years/gstlal.xml.gz
--rwxr-xr-x   0        0        0     2519 2023-03-29 01:10:32.533050 gwcelery-2.0.4/gwcelery/data/gwcelery.sub
--rw-r--r--   0        0        0      505 2023-03-29 01:10:32.533050 gwcelery-2.0.4/gwcelery/email/__init__.py
--rw-r--r--   0        0        0     3317 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/email/bootsteps.py
--rw-r--r--   0        0        0      995 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/email/signals.py
--rw-r--r--   0        0        0     1457 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/flask.py
--rw-r--r--   0        0        0      529 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/igwn_alert/__init__.py
--rw-r--r--   0        0        0     4484 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/igwn_alert/bootsteps.py
--rw-r--r--   0        0        0      608 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/igwn_alert/signals.py
--rw-r--r--   0        0        0      275 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/jinja.py
--rw-r--r--   0        0        0      285 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/kafka/__init__.py
--rw-r--r--   0        0        0     6869 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/kafka/bootsteps.py
--rw-r--r--   0        0        0     2567 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/sentry/__init__.py
--rw-r--r--   0        0        0       34 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/sentry/integrations/__init__.py
--rw-r--r--   0        0        0      832 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/sentry/integrations/condor.py
--rw-r--r--   0        0        0      836 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/sentry/integrations/requests.py
--rw-r--r--   0        0        0      939 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/sentry/integrations/subprocess.py
--rw-r--r--   0        0        0     1302 2023-03-29 01:10:32.534050 gwcelery-2.0.4/gwcelery/static/typeahead.css
--rw-r--r--   0        0        0     4124 2023-03-29 01:10:32.535050 gwcelery-2.0.4/gwcelery/static/vega/index.html
--rw-r--r--   0        0        0      515 2023-03-29 01:10:32.535050 gwcelery-2.0.4/gwcelery/tasks/__init__.py
--rw-r--r--   0        0        0    10113 2023-03-29 01:10:32.535050 gwcelery-2.0.4/gwcelery/tasks/alerts.py
--rw-r--r--   0        0        0     2672 2023-03-29 01:10:32.535050 gwcelery-2.0.4/gwcelery/tasks/bayestar.py
--rw-r--r--   0        0        0     1296 2023-03-29 01:10:32.535050 gwcelery-2.0.4/gwcelery/tasks/circulars.py
--rw-r--r--   0        0        0     7502 2023-03-29 01:10:32.535050 gwcelery-2.0.4/gwcelery/tasks/condor.py
--rw-r--r--   0        0        0     2692 2023-03-29 01:10:32.535050 gwcelery-2.0.4/gwcelery/tasks/core.py
--rw-r--r--   0        0        0    20924 2023-03-29 01:10:32.535050 gwcelery-2.0.4/gwcelery/tasks/detchar.py
--rw-r--r--   0        0        0     4819 2023-03-29 01:10:32.535050 gwcelery-2.0.4/gwcelery/tasks/em_bright.py
--rw-r--r--   0        0        0    20767 2023-03-29 01:10:32.536050 gwcelery-2.0.4/gwcelery/tasks/external_skymaps.py
--rw-r--r--   0        0        0    20662 2023-03-29 01:10:32.536050 gwcelery-2.0.4/gwcelery/tasks/external_triggers.py
--rw-r--r--   0        0        0     6732 2023-03-29 01:10:32.536050 gwcelery-2.0.4/gwcelery/tasks/first2years.py
--rw-r--r--   0        0        0     5794 2023-03-29 01:10:32.536050 gwcelery-2.0.4/gwcelery/tasks/first2years_external.py
--rw-r--r--   0        0        0     4831 2023-03-29 01:10:32.536050 gwcelery-2.0.4/gwcelery/tasks/gcn.py
--rw-r--r--   0        0        0    11079 2023-03-29 01:10:32.536050 gwcelery-2.0.4/gwcelery/tasks/gracedb.py
--rw-r--r--   0        0        0     2453 2023-03-29 01:10:32.536050 gwcelery-2.0.4/gwcelery/tasks/igwn_alert.py
--rw-r--r--   0        0        0    28642 2023-03-29 01:10:32.536050 gwcelery-2.0.4/gwcelery/tasks/inference.py
--rw-r--r--   0        0        0     1396 2023-03-29 01:10:32.537050 gwcelery-2.0.4/gwcelery/tasks/legacy_gracedb.py
--rw-r--r--   0        0        0     7772 2023-03-29 01:10:32.537050 gwcelery-2.0.4/gwcelery/tasks/notice_text.py
--rw-r--r--   0        0        0    43872 2023-03-29 01:10:32.537050 gwcelery-2.0.4/gwcelery/tasks/orchestrator.py
--rw-r--r--   0        0        0     5776 2023-03-29 01:10:32.537050 gwcelery-2.0.4/gwcelery/tasks/p_astro.py
--rw-r--r--   0        0        0    18633 2023-03-29 01:10:32.537050 gwcelery-2.0.4/gwcelery/tasks/raven.py
--rw-r--r--   0        0        0    12528 2023-03-29 01:10:32.538050 gwcelery-2.0.4/gwcelery/tasks/skymaps.py
--rw-r--r--   0        0        0    23453 2023-03-29 01:10:32.538050 gwcelery-2.0.4/gwcelery/tasks/superevents.py
--rw-r--r--   0        0        0     1084 2023-03-29 01:10:32.538050 gwcelery-2.0.4/gwcelery/templates/fits_header.jinja2
--rw-r--r--   0        0        0    31039 2023-03-29 01:10:32.538050 gwcelery-2.0.4/gwcelery/templates/index.jinja2
--rw-r--r--   0        0        0     8505 2023-03-29 01:10:32.538050 gwcelery-2.0.4/gwcelery/templates/lalinference.jinja2
--rw-r--r--   0        0        0     8644 2023-03-29 01:10:32.538050 gwcelery-2.0.4/gwcelery/templates/rapidpe.jinja2
--rw-r--r--   0        0        0      806 2023-03-29 01:10:32.538050 gwcelery-2.0.4/gwcelery/templates/vector_table.jinja2
--rw-r--r--   0        0        0        0 2023-03-29 01:10:32.538050 gwcelery-2.0.4/gwcelery/tests/__init__.py
--rw-r--r--   0        0        0     4388 2023-03-29 01:10:32.539050 gwcelery-2.0.4/gwcelery/tests/conftest.py
--rw-r--r--   0        0        0      976 2023-03-29 01:10:32.539050 gwcelery-2.0.4/gwcelery/tests/data/G000012_S0040_preferred.json
--rw-r--r--   0        0        0     6258 2023-03-29 01:10:32.539050 gwcelery-2.0.4/gwcelery/tests/data/G298048-1-Initial.xml
--rw-r--r--   0        0        0      599 2023-03-29 01:10:32.539050 gwcelery-2.0.4/gwcelery/tests/data/G298048_log.json
--rw-r--r--   0        0        0      150 2023-03-29 01:10:32.539050 gwcelery-2.0.4/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
--rw-r--r--   0        0        0      974 2023-03-29 01:10:32.539050 gwcelery-2.0.4/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
--rw-r--r--   0        0        0    17560 2023-03-29 01:10:32.539050 gwcelery-2.0.4/gwcelery/tests/data/MS220722v.xml
--rw-r--r--   0        0        0   777600 2023-03-29 01:10:32.545050 gwcelery-2.0.4/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
--rw-r--r--   0        0        0     3387 2023-03-29 01:10:32.545050 gwcelery-2.0.4/gwcelery/tests/data/T0212_S0039_preferred.json
--rw-r--r--   0        0        0     3384 2023-03-29 01:10:32.545050 gwcelery-2.0.4/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
--rw-r--r--   0        0        0     5210 2023-03-29 01:10:32.545050 gwcelery-2.0.4/gwcelery/tests/data/T0219_S0041_nopreferred.json
--rw-r--r--   0        0        0        0 2023-03-29 01:10:32.545050 gwcelery-2.0.4/gwcelery/tests/data/__init__.py
--rw-r--r--   0        0        0     2290 2023-03-29 01:10:32.545050 gwcelery-2.0.4/gwcelery/tests/data/agile_grb_gcn.xml
--rw-r--r--   0        0        0   854036 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/coinc.xml
--rw-r--r--   0        0        0     6175 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/externaltrigger_original_data.xml
--rw-r--r--   0        0        0     5482 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/fermi_grb_gcn.xml
--rw-r--r--   0        0        0     5469 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/fermi_initial_grb_gcn.xml
--rw-r--r--   0        0        0     5865 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/fermi_noise_gcn.xml
--rw-r--r--   0        0        0     5864 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/fermi_noise_gcn_2.xml
--rw-r--r--   0        0        0     4914 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
--rw-r--r--   0        0        0     4914 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
--rw-r--r--   0        0        0     3407 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/fits_header_result.html
--rw-r--r--   0        0        0      882 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/gracedb_externaltrigger_log.json
--rw-r--r--   0        0        0      446 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/gracedb_setrigger_log.json
--rw-r--r--   0        0        0      870 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_detchar.json
--rw-r--r--   0        0        0     2025 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_exttrig_creation.json
--rw-r--r--   0        0        0     2007 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
--rw-r--r--   0        0        0      166 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_fits.json
--rw-r--r--   0        0        0      101 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_label_dqv.json
--rw-r--r--   0        0        0      743 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_psd.json
--rw-r--r--   0        0        0     2016 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_snews_creation.json
--rw-r--r--   0        0        0     2008 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_snews_test_creation.json
--rw-r--r--   0        0        0     2028 2023-03-29 01:10:32.551050 gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_subgrb_creation.json
--rw-r--r--   0        0        0     1235 2023-03-29 01:10:32.552050 gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_superevent_creation.json
--rw-r--r--   0        0        0      107 2023-03-29 01:10:32.552050 gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_superevent_label.json
--rw-r--r--   0        0        0     5021 2023-03-29 01:10:32.552050 gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_voevent.json
--rw-r--r--   0        0        0     4429 2023-03-29 01:10:32.552050 gwcelery-2.0.4/gwcelery/tests/data/integral_grb_gcn.xml
--rw-r--r--   0        0        0        0 2023-03-29 01:10:32.552050 gwcelery-2.0.4/gwcelery/tests/data/llhoft/__init__.py
--rw-r--r--   0        0        0    14622 2023-03-29 01:10:32.552050 gwcelery-2.0.4/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-03-29 01:10:32.552050 gwcelery-2.0.4/gwcelery/tests/data/llhoft/fail/L1/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 01:10:32.552050 gwcelery-2.0.4/gwcelery/tests/data/llhoft/fail/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 01:10:32.552050 gwcelery-2.0.4/gwcelery/tests/data/llhoft/omegascan/__init__.py
--rw-r--r--   0        0        0   516419 2023-03-29 01:10:32.553050 gwcelery-2.0.4/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
--rw-r--r--   0        0        0    14630 2023-03-29 01:10:32.553050 gwcelery-2.0.4/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-03-29 01:10:32.553050 gwcelery-2.0.4/gwcelery/tests/data/llhoft/pass/H1/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 01:10:32.553050 gwcelery-2.0.4/gwcelery/tests/data/llhoft/pass/__init__.py
--rw-r--r--   0        0        0    13099 2023-03-29 01:10:32.553050 gwcelery-2.0.4/gwcelery/tests/data/lvalert_event_creation.json
--rw-r--r--   0        0        0     9060 2023-03-29 01:10:32.554050 gwcelery-2.0.4/gwcelery/tests/data/lvalert_xmpp.xml
--rw-r--r--   0        0        0      864 2023-03-29 01:10:32.554050 gwcelery-2.0.4/gwcelery/tests/data/mock_superevent_object.json
--rw-r--r--   0        0        0   445440 2023-03-29 01:10:32.555050 gwcelery-2.0.4/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
--rw-r--r--   0        0        0   294426 2023-03-29 01:10:32.556050 gwcelery-2.0.4/gwcelery/tests/data/psd.xml.gz
--rw-r--r--   0        0        0     2964 2023-03-29 01:10:32.556050 gwcelery-2.0.4/gwcelery/tests/data/sample_events.json
--rw-r--r--   0        0        0     3648 2023-03-29 01:10:32.556050 gwcelery-2.0.4/gwcelery/tests/data/samples.hdf5
--rw-r--r--   0        0        0      616 2023-03-29 01:10:32.557050 gwcelery-2.0.4/gwcelery/tests/data/scaler_set_all.pickle
--rw-r--r--   0        0        0     6169 2023-03-29 01:10:32.557050 gwcelery-2.0.4/gwcelery/tests/data/snews_gcn.xml
--rw-r--r--   0        0        0     6161 2023-03-29 01:10:32.557050 gwcelery-2.0.4/gwcelery/tests/data/snews_gcn_test.xml
--rw-r--r--   0        0        0     9583 2023-03-29 01:10:32.557050 gwcelery-2.0.4/gwcelery/tests/data/superevents.json
--rw-r--r--   0        0        0     7713 2023-03-29 01:10:32.557050 gwcelery-2.0.4/gwcelery/tests/data/swift_grb_gcn.xml
--rw-r--r--   0        0        0   581918 2023-03-29 01:10:32.559050 gwcelery-2.0.4/gwcelery/tests/data/test_classifier.pickle
--rw-r--r--   0        0        0     4042 2023-03-29 01:10:32.559050 gwcelery-2.0.4/gwcelery/tests/process.py
--rw-r--r--   0        0        0     2307 2023-03-29 01:10:32.559050 gwcelery-2.0.4/gwcelery/tests/test_sentry.py
--rw-r--r--   0        0        0     3365 2023-03-29 01:10:32.559050 gwcelery-2.0.4/gwcelery/tests/test_tasks_alerts_validate.py
--rw-r--r--   0        0        0     1439 2023-03-29 01:10:32.559050 gwcelery-2.0.4/gwcelery/tests/test_tasks_bayestar.py
--rw-r--r--   0        0        0     2416 2023-03-29 01:10:32.559050 gwcelery-2.0.4/gwcelery/tests/test_tasks_circulars.py
--rw-r--r--   0        0        0     4550 2023-03-29 01:10:32.559050 gwcelery-2.0.4/gwcelery/tests/test_tasks_condor.py
--rw-r--r--   0        0        0    11689 2023-03-29 01:10:32.559050 gwcelery-2.0.4/gwcelery/tests/test_tasks_detchar.py
--rw-r--r--   0        0        0     2287 2023-03-29 01:10:32.559050 gwcelery-2.0.4/gwcelery/tests/test_tasks_em_bright.py
--rw-r--r--   0        0        0    10936 2023-03-29 01:10:32.559050 gwcelery-2.0.4/gwcelery/tests/test_tasks_external_skymaps.py
--rw-r--r--   0        0        0    29457 2023-03-29 01:10:32.560050 gwcelery-2.0.4/gwcelery/tests/test_tasks_external_triggers.py
--rw-r--r--   0        0        0     1816 2023-03-29 01:10:32.560050 gwcelery-2.0.4/gwcelery/tests/test_tasks_first2years.py
--rw-r--r--   0        0        0     3817 2023-03-29 01:10:32.560050 gwcelery-2.0.4/gwcelery/tests/test_tasks_first2years_external.py
--rw-r--r--   0        0        0     1826 2023-03-29 01:10:32.560050 gwcelery-2.0.4/gwcelery/tests/test_tasks_gcn.py
--rw-r--r--   0        0        0     1655 2023-03-29 01:10:32.560050 gwcelery-2.0.4/gwcelery/tests/test_tasks_gcn_validate.py
--rw-r--r--   0        0        0     5739 2023-03-29 01:10:32.560050 gwcelery-2.0.4/gwcelery/tests/test_tasks_gracedb.py
--rw-r--r--   0        0        0     3662 2023-03-29 01:10:32.560050 gwcelery-2.0.4/gwcelery/tests/test_tasks_igwn_alert.py
--rw-r--r--   0        0        0    20205 2023-03-29 01:10:32.560050 gwcelery-2.0.4/gwcelery/tests/test_tasks_inference.py
--rw-r--r--   0        0        0    30795 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tests/test_tasks_orchestrator.py
--rw-r--r--   0        0        0     1647 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tests/test_tasks_p_astro.py
--rw-r--r--   0        0        0    23933 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tests/test_tasks_raven.py
--rw-r--r--   0        0        0     5035 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tests/test_tasks_skymaps.py
--rw-r--r--   0        0        0    39941 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tests/test_tasks_superevents.py
--rw-r--r--   0        0        0      637 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tests/test_tempfile.py
--rw-r--r--   0        0        0     3520 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tests/test_tools_condor.py
--rw-r--r--   0        0        0     1098 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tests/test_tools_condor_submit_helper.py
--rw-r--r--   0        0        0      633 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tests/test_tools_flask.py
--rw-r--r--   0        0        0     8067 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tests/test_tools_nagios.py
--rw-r--r--   0        0        0      269 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tests/test_util.py
--rw-r--r--   0        0        0    11302 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tests/test_views.py
--rw-r--r--   0        0        0      216 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tools/__init__.py
--rw-r--r--   0        0        0     2948 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tools/condor.py
--rw-r--r--   0        0        0     1120 2023-03-29 01:10:32.561050 gwcelery-2.0.4/gwcelery/tools/condor_submit_helper.py
--rw-r--r--   0        0        0     1938 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/tools/flask.py
--rw-r--r--   0        0        0     5763 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/tools/nagios.py
--rw-r--r--   0        0        0      413 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/util/__init__.py
--rw-r--r--   0        0        0     1007 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/util/cmdline.py
--rw-r--r--   0        0        0      453 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/util/matplotlib.py
--rw-r--r--   0        0        0      390 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/util/proxy.py
--rw-r--r--   0        0        0      514 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/util/resources.py
--rw-r--r--   0        0        0      253 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/util/sphinx.py
--rw-r--r--   0        0        0      941 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/util/tempfile.py
--rw-r--r--   0        0        0    13516 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/views.py
--rw-r--r--   0        0        0      365 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/voevent/__init__.py
--rw-r--r--   0        0        0     6387 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/voevent/bootsteps.py
--rw-r--r--   0        0        0     1063 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/voevent/logging.py
--rw-r--r--   0        0        0      779 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/voevent/signals.py
--rw-r--r--   0        0        0      852 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/voevent/subscriber.py
--rw-r--r--   0        0        0     1454 2023-03-29 01:10:32.562050 gwcelery-2.0.4/gwcelery/voevent/util.py
--rw-r--r--   0        0        0     5793 2023-03-29 01:10:42.810053 gwcelery-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     4618 1970-01-01 00:00:00.000000 gwcelery-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0    90483 2023-04-20 23:28:05.189174 gwcelery-2.0.5/CHANGES.rst
+-rw-r--r--   0        0        0       64 2023-04-20 23:28:05.189174 gwcelery-2.0.5/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    19716 2023-04-20 23:28:05.189174 gwcelery-2.0.5/LICENSE.rst
+-rw-r--r--   0        0        0     1351 2023-04-20 23:28:05.189174 gwcelery-2.0.5/README.rst
+-rw-r--r--   0        0        0      634 2023-04-20 23:28:05.189174 gwcelery-2.0.5/doc/Makefile
+-rw-r--r--   0        0        0   191486 2023-04-20 23:28:05.190173 gwcelery-2.0.5/doc/_static/acceptance-tests-checklist.png
+-rw-r--r--   0        0        0   241593 2023-04-20 23:28:05.191174 gwcelery-2.0.5/doc/_static/celeryevent-screenshot.png
+-rw-r--r--   0        0        0   206465 2023-04-20 23:28:05.192174 gwcelery-2.0.5/doc/_static/deployment-screenshot.png
+-rw-r--r--   0        0        0   161306 2023-04-20 23:28:05.194174 gwcelery-2.0.5/doc/_static/flask-screenshot.png
+-rw-r--r--   0        0        0   328056 2023-04-20 23:28:05.195174 gwcelery-2.0.5/doc/_static/flower-screenshot.png
+-rw-r--r--   0        0        0   114719 2023-04-20 23:28:05.196174 gwcelery-2.0.5/doc/_static/logo-0.5x.png
+-rw-r--r--   0        0        0   351955 2023-04-20 23:28:05.198174 gwcelery-2.0.5/doc/_static/logo.png
+-rw-r--r--   0        0        0   230777 2023-04-20 23:28:05.199174 gwcelery-2.0.5/doc/_static/sentry-screenshot.png
+-rwxr-xr-x   0        0        0     7356 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/conf.py
+-rw-r--r--   0        0        0     3543 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/configuration.rst
+-rw-r--r--   0        0        0     5698 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/contributing.rst
+-rw-r--r--   0        0        0     7204 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/deployment.rst
+-rw-r--r--   0        0        0    10176 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/design.rst
+-rw-r--r--   0        0        0      486 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.conf.rst
+-rw-r--r--   0        0        0      284 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.email.rst
+-rw-r--r--   0        0        0      329 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.igwn_alert.rst
+-rw-r--r--   0        0        0      227 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.rst
+-rw-r--r--   0        0        0       79 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.sentry.rst
+-rw-r--r--   0        0        0       97 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.tasks.alerts.rst
+-rw-r--r--   0        0        0      103 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.tasks.bayestar.rst
+-rw-r--r--   0        0        0      107 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.tasks.circulars.rst
+-rw-r--r--   0        0        0       98 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.condor.rst
+-rw-r--r--   0        0        0     2404 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.detchar.rst
+-rw-r--r--   0        0        0     1110 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.em_bright.rst
+-rw-r--r--   0        0        0      129 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.external_skymaps.rst
+-rw-r--r--   0        0        0     6738 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.external_triggers.rst
+-rw-r--r--   0        0        0      112 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.first2years.rst
+-rw-r--r--   0        0        0       88 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.gcn.rst
+-rw-r--r--   0        0        0      100 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.gracedb.rst
+-rw-r--r--   0        0        0      109 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.igwn_alert.rst
+-rw-r--r--   0        0        0      109 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.inference.rst
+-rw-r--r--   0        0        0     8111 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.orchestrator.rst
+-rw-r--r--   0        0        0      100 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.p_astro.rst
+-rw-r--r--   0        0        0       94 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.raven.rst
+-rw-r--r--   0        0        0      628 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.rst
+-rw-r--r--   0        0        0      100 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.skymaps.rst
+-rw-r--r--   0        0        0     7161 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.superevents.rst
+-rw-r--r--   0        0        0       97 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tools.condor.rst
+-rw-r--r--   0        0        0       94 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tools.flask.rst
+-rw-r--r--   0        0        0       97 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tools.nagios.rst
+-rw-r--r--   0        0        0      185 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tools.rst
+-rw-r--r--   0        0        0       73 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.util.rst
+-rw-r--r--   0        0        0      507 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.voevent.rst
+-rw-r--r--   0        0        0     3564 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/htcondor.rst
+-rw-r--r--   0        0        0     1576 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/index.rst
+-rw-r--r--   0        0        0      800 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/make.bat
+-rw-r--r--   0        0        0     4416 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/monitoring.rst
+-rw-r--r--   0        0        0     5312 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/quickstart.rst
+-rw-r--r--   0        0        0     1149 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/__init__.py
+-rw-r--r--   0        0        0    18447 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/_version.py
+-rw-r--r--   0        0        0    14591 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/conf/__init__.py
+-rw-r--r--   0        0        0      403 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/conf/development.py
+-rw-r--r--   0        0        0     1026 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/conf/minikube.py
+-rw-r--r--   0        0        0     1562 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/conf/playground.py
+-rw-r--r--   0        0        0     3104 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/conf/production.py
+-rw-r--r--   0        0        0     1044 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/conf/test.py
+-rw-r--r--   0        0        0        0 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/data/first2years/__init__.py
+-rw-r--r--   0        0        0   731421 2023-04-20 23:28:05.204174 gwcelery-2.0.5/gwcelery/data/first2years/gstlal.xml.gz
+-rwxr-xr-x   0        0        0     2519 2023-04-20 23:28:05.204174 gwcelery-2.0.5/gwcelery/data/gwcelery.sub
+-rw-r--r--   0        0        0      505 2023-04-20 23:28:05.204174 gwcelery-2.0.5/gwcelery/email/__init__.py
+-rw-r--r--   0        0        0     3317 2023-04-20 23:28:05.204174 gwcelery-2.0.5/gwcelery/email/bootsteps.py
+-rw-r--r--   0        0        0      995 2023-04-20 23:28:05.204174 gwcelery-2.0.5/gwcelery/email/signals.py
+-rw-r--r--   0        0        0     1457 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/flask.py
+-rw-r--r--   0        0        0      529 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/igwn_alert/__init__.py
+-rw-r--r--   0        0        0     4484 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/igwn_alert/bootsteps.py
+-rw-r--r--   0        0        0      608 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/igwn_alert/signals.py
+-rw-r--r--   0        0        0      275 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/jinja.py
+-rw-r--r--   0        0        0      285 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/kafka/__init__.py
+-rw-r--r--   0        0        0     6544 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/kafka/bootsteps.py
+-rw-r--r--   0        0        0     2567 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/sentry/__init__.py
+-rw-r--r--   0        0        0       34 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/sentry/integrations/__init__.py
+-rw-r--r--   0        0        0      832 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/sentry/integrations/condor.py
+-rw-r--r--   0        0        0      836 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/sentry/integrations/requests.py
+-rw-r--r--   0        0        0      939 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/sentry/integrations/subprocess.py
+-rw-r--r--   0        0        0     1302 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/static/typeahead.css
+-rw-r--r--   0        0        0     4124 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/static/vega/index.html
+-rw-r--r--   0        0        0      515 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/tasks/__init__.py
+-rw-r--r--   0        0        0    11951 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/tasks/alerts.py
+-rw-r--r--   0        0        0     2672 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/tasks/bayestar.py
+-rw-r--r--   0        0        0     1296 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/circulars.py
+-rw-r--r--   0        0        0     7502 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/condor.py
+-rw-r--r--   0        0        0     2692 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/core.py
+-rw-r--r--   0        0        0    20924 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/detchar.py
+-rw-r--r--   0        0        0     4819 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/em_bright.py
+-rw-r--r--   0        0        0    21902 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/external_skymaps.py
+-rw-r--r--   0        0        0    22568 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/external_triggers.py
+-rw-r--r--   0        0        0     6832 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/first2years.py
+-rw-r--r--   0        0        0     6384 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/first2years_external.py
+-rw-r--r--   0        0        0     4831 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/gcn.py
+-rw-r--r--   0        0        0    11079 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/gracedb.py
+-rw-r--r--   0        0        0     2453 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/igwn_alert.py
+-rw-r--r--   0        0        0    30399 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/inference.py
+-rw-r--r--   0        0        0     1396 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/legacy_gracedb.py
+-rw-r--r--   0        0        0     7772 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/notice_text.py
+-rw-r--r--   0        0        0    46448 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/orchestrator.py
+-rw-r--r--   0        0        0     5796 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/p_astro.py
+-rw-r--r--   0        0        0    19628 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/raven.py
+-rw-r--r--   0        0        0    12528 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/skymaps.py
+-rw-r--r--   0        0        0    23386 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/tasks/superevents.py
+-rw-r--r--   0        0        0     1084 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/templates/fits_header.jinja2
+-rw-r--r--   0        0        0    34059 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/templates/index.jinja2
+-rw-r--r--   0        0        0     8505 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/templates/lalinference.jinja2
+-rw-r--r--   0        0        0     8939 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/templates/rapidpe.jinja2
+-rw-r--r--   0        0        0      806 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/templates/vector_table.jinja2
+-rw-r--r--   0        0        0        0 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/tests/__init__.py
+-rw-r--r--   0        0        0     4388 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/tests/conftest.py
+-rw-r--r--   0        0        0      976 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/tests/data/G000012_S0040_preferred.json
+-rw-r--r--   0        0        0     6258 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/tests/data/G298048-1-Initial.xml
+-rw-r--r--   0        0        0      599 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/tests/data/G298048_log.json
+-rw-r--r--   0        0        0      150 2023-04-20 23:28:05.209174 gwcelery-2.0.5/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
+-rw-r--r--   0        0        0      974 2023-04-20 23:28:05.209174 gwcelery-2.0.5/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
+-rw-r--r--   0        0        0    17572 2023-04-20 23:28:05.209174 gwcelery-2.0.5/gwcelery/tests/data/MS220722v.xml
+-rw-r--r--   0        0        0   777600 2023-04-20 23:28:05.213173 gwcelery-2.0.5/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
+-rw-r--r--   0        0        0     8220 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/S230413b.json
+-rw-r--r--   0        0        0     7255 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/S230413g.json
+-rw-r--r--   0        0        0     7721 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/S230413h.json
+-rw-r--r--   0        0        0     3387 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/T0212_S0039_preferred.json
+-rw-r--r--   0        0        0     3384 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
+-rw-r--r--   0        0        0     5210 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/T0219_S0041_nopreferred.json
+-rw-r--r--   0        0        0        0 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/__init__.py
+-rw-r--r--   0        0        0     2290 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/agile_grb_gcn.xml
+-rw-r--r--   0        0        0   854036 2023-04-20 23:28:05.218174 gwcelery-2.0.5/gwcelery/tests/data/coinc.xml
+-rw-r--r--   0        0        0     6175 2023-04-20 23:28:05.218174 gwcelery-2.0.5/gwcelery/tests/data/externaltrigger_original_data.xml
+-rw-r--r--   0        0        0     5482 2023-04-20 23:28:05.218174 gwcelery-2.0.5/gwcelery/tests/data/fermi_grb_gcn.xml
+-rw-r--r--   0        0        0     5469 2023-04-20 23:28:05.218174 gwcelery-2.0.5/gwcelery/tests/data/fermi_initial_grb_gcn.xml
+-rw-r--r--   0        0        0     5865 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/fermi_noise_gcn.xml
+-rw-r--r--   0        0        0     5864 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/fermi_noise_gcn_2.xml
+-rw-r--r--   0        0        0     4914 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
+-rw-r--r--   0        0        0     4914 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
+-rw-r--r--   0        0        0     3407 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/fits_header_result.html
+-rw-r--r--   0        0        0      882 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/gracedb_externaltrigger_log.json
+-rw-r--r--   0        0        0      446 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/gracedb_setrigger_log.json
+-rw-r--r--   0        0        0      870 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_detchar.json
+-rw-r--r--   0        0        0     2025 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_exttrig_creation.json
+-rw-r--r--   0        0        0     2007 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
+-rw-r--r--   0        0        0      166 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_fits.json
+-rw-r--r--   0        0        0      101 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_label_dqv.json
+-rw-r--r--   0        0        0      743 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_psd.json
+-rw-r--r--   0        0        0     2020 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_snews_creation.json
+-rw-r--r--   0        0        0     2012 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_snews_test_creation.json
+-rw-r--r--   0        0        0     2028 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_subgrb_creation.json
+-rw-r--r--   0        0        0     1235 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_superevent_creation.json
+-rw-r--r--   0        0        0      107 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_superevent_label.json
+-rw-r--r--   0        0        0     5021 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_voevent.json
+-rw-r--r--   0        0        0     4429 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/integral_grb_gcn.xml
+-rw-r--r--   0        0        0     4295 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/integral_mdc_gcn.xml
+-rw-r--r--   0        0        0        0 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/__init__.py
+-rw-r--r--   0        0        0    14622 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/fail/L1/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/fail/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/omegascan/__init__.py
+-rw-r--r--   0        0        0   516419 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
+-rw-r--r--   0        0        0    14630 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/pass/H1/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/pass/__init__.py
+-rw-r--r--   0        0        0    13099 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/lvalert_event_creation.json
+-rw-r--r--   0        0        0     9060 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/lvalert_xmpp.xml
+-rw-r--r--   0        0        0      864 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/mock_superevent_object.json
+-rw-r--r--   0        0        0   445440 2023-04-20 23:28:05.223174 gwcelery-2.0.5/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
+-rw-r--r--   0        0        0   294426 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/psd.xml.gz
+-rw-r--r--   0        0        0     2964 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/sample_events.json
+-rw-r--r--   0        0        0     3648 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/samples.hdf5
+-rw-r--r--   0        0        0      616 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/scaler_set_all.pickle
+-rw-r--r--   0        0        0     6169 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/snews_gcn.xml
+-rw-r--r--   0        0        0     6161 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/snews_gcn_test.xml
+-rw-r--r--   0        0        0     9583 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/superevents.json
+-rw-r--r--   0        0        0     7713 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/swift_grb_gcn.xml
+-rw-r--r--   0        0        0   581918 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/data/test_classifier.pickle
+-rw-r--r--   0        0        0     4042 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/process.py
+-rw-r--r--   0        0        0     2307 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/test_sentry.py
+-rw-r--r--   0        0        0     1705 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/test_tasks_alerts.py
+-rw-r--r--   0        0        0     4916 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/test_tasks_alerts_validate.py
+-rw-r--r--   0        0        0     1439 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/test_tasks_bayestar.py
+-rw-r--r--   0        0        0     2416 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/test_tasks_circulars.py
+-rw-r--r--   0        0        0     4550 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/test_tasks_condor.py
+-rw-r--r--   0        0        0    11689 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_detchar.py
+-rw-r--r--   0        0        0     2287 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_em_bright.py
+-rw-r--r--   0        0        0    12265 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_external_skymaps.py
+-rw-r--r--   0        0        0    31976 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_external_triggers.py
+-rw-r--r--   0        0        0     1816 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_first2years.py
+-rw-r--r--   0        0        0     4555 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_first2years_external.py
+-rw-r--r--   0        0        0     1826 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_gcn.py
+-rw-r--r--   0        0        0     1655 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_gcn_validate.py
+-rw-r--r--   0        0        0     5739 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_gracedb.py
+-rw-r--r--   0        0        0     3662 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_igwn_alert.py
+-rw-r--r--   0        0        0    21517 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_inference.py
+-rw-r--r--   0        0        0    32509 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tasks_orchestrator.py
+-rw-r--r--   0        0        0     1647 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tasks_p_astro.py
+-rw-r--r--   0        0        0    25900 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tasks_raven.py
+-rw-r--r--   0        0        0     5035 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tasks_skymaps.py
+-rw-r--r--   0        0        0    39981 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tasks_superevents.py
+-rw-r--r--   0        0        0      637 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tempfile.py
+-rw-r--r--   0        0        0     3520 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tools_condor.py
+-rw-r--r--   0        0        0     1098 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tools_condor_submit_helper.py
+-rw-r--r--   0        0        0      633 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tools_flask.py
+-rw-r--r--   0        0        0     8067 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tools_nagios.py
+-rw-r--r--   0        0        0      269 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_util.py
+-rw-r--r--   0        0        0    21450 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_views.py
+-rw-r--r--   0        0        0      216 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tools/__init__.py
+-rw-r--r--   0        0        0     2948 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tools/condor.py
+-rw-r--r--   0        0        0     1120 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/tools/condor_submit_helper.py
+-rw-r--r--   0        0        0     1938 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/tools/flask.py
+-rw-r--r--   0        0        0     5763 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/tools/nagios.py
+-rw-r--r--   0        0        0      413 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/__init__.py
+-rw-r--r--   0        0        0     1007 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/cmdline.py
+-rw-r--r--   0        0        0      453 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/matplotlib.py
+-rw-r--r--   0        0        0      390 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/proxy.py
+-rw-r--r--   0        0        0      514 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/resources.py
+-rw-r--r--   0        0        0      253 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/sphinx.py
+-rw-r--r--   0        0        0      941 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/tempfile.py
+-rw-r--r--   0        0        0    18472 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/views.py
+-rw-r--r--   0        0        0      365 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/voevent/__init__.py
+-rw-r--r--   0        0        0     6387 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/voevent/bootsteps.py
+-rw-r--r--   0        0        0     1063 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/voevent/logging.py
+-rw-r--r--   0        0        0      779 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/voevent/signals.py
+-rw-r--r--   0        0        0      852 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/voevent/subscriber.py
+-rw-r--r--   0        0        0     1454 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/voevent/util.py
+-rw-r--r--   0        0        0     5901 2023-04-20 23:28:18.384198 gwcelery-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4597 1970-01-01 00:00:00.000000 gwcelery-2.0.5/PKG-INFO
```

### Comparing `gwcelery-2.0.4/CHANGES.rst` & `gwcelery-2.0.5/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,94 @@
 Changelog
 =========
 
+2.0.5 "Mothman" (2023-04-20)
+----------------------------
+
+-   Add Mattermost channel creation for the RRT to discuss a superevent
+    candidate.
+
+-   Use Online_PE_MDC nodes for bilby jobs on O3-Replay injections.
+
+-   Do not remove PE run directory after the run completes or fails.
+
+-   Filter external events based on ``External`` group in ``superevents.py``,
+    instead of logic based on substring matching.
+
+-   Increase test coverage for views.py and fix manual mock coincidence
+    injections.
+
+-   Bump ligo.em-bright version to v1.1.1.
+
+-   Bump ligo-followup-advocate version to v1.2.1.
+
+-   Also update the preferred external event when issuing a manual RAVEN alert.
+
+-   Skip less significant alert workflow in case of both significant and EW
+    triggers. Previous workflow only accounted for blocking in presence of
+    significant events.
+
+-   Update rapidpe-rift-pipe version to 0.0.12. Use mchirp and q as the
+    coordinates for the rectilinear intrinsic grid. Update accounting_group to
+    ligo.dev.o4.cbc.pe.lalinferencerapid and add accouting_group_user. Add
+    an option to map the events to an injection. Upload only a select set
+    of log files to gracedb. 
+
+-   Prevent alternative collating method for O3 replay and MDC events with INTEGRAL.
+
+-   Pick RAVEN_ALERT preferred external event over one that doesn't pass the joint
+    alert publishing criteria.
+
+-   Avoid updating values in the combined sky map if missing in the GW sky map.
+
+-   Catch bug if instrument not in external sky map header. This could occur
+    if grabbing a sky map from an external URL such as from Fermi-GBM that
+    lacks this field.
+
+-   Prevent external event from switching superevents.
+
+-   Only plot sky map overlap with prefered external event when RAVEN_ALERT
+    label is applied.
+
+-   Populate the duration and central_frequency fields in Kafka notices for
+    burst events.
+
+-   Add periodic SNEWS MDC events to test the corresponding IGWN alert
+    listener.
+
+-   Use sky map from preferred event rather than superevent, triggering off 
+    EM_READY label instead of SKYMAP_READY. If SKYMAP_READY is applied or if a
+    sky map file is added to the superevent, we will once again try to get the
+    GW sky map from the superevent.
+
+-   Update bilby and bilby_pipe to 2.1.0 and 1.0.10 respectively. The number of
+    spline nodes for calibration errors is increased to 10 thanks to the bilby
+    optimizations. Change sampler settings into naccept=60, nlive=500.
+
+-   Add automatic PESummary task to postprocess bilby parameter estimation
+    results.
+
+-   Indicate dispatch of first less-significant alert with
+    ``LOW_SIGNIF_PRELIM_SENT``. Launch timer for revision and send second less
+    significant alert with the same label conditioned on blocking labels
+    indicating significant alert or advocate action.
+
+-   Replace ``EM_Selected`` and ``EM_SelectedConfident`` labels with
+    ``LOW_SIGNIF_LOCKED`` and ``SIGNIF_LOCKED``.
+
+-   Fix repeating of raven alert publishing criteria met log message.
+
+-   Don't compute p-astro for spiir/AllSky because it now computes and uploads
+    its own.
+
+-   Prevent repeating of sky map comparison pipeline with the secondary
+    flattened sky maps.
+
 2.0.4 "Skunk Ape" (2023-03-28)
-------------------
+------------------------------
 
 -   Add dashboard button to download sky map from a URL and upload to an
     external event.
 
 -   Set pipeline preferred events after revising preferred event. Provide dashboard to set them.
 
 -   Remove the ``prelimimary_alert_timeout`` variable and workflow, since the
@@ -100,14 +182,16 @@
 -   Add duration and central_frequency fields to Kafka notices. The fields are
     set to None for now.
 
 -   Set the ``Significant`` field in VOEvent XML packets and Kafka notices.
 
 -   Import Kafka notice schema from the new igwn-gwalert-schema library.
 
+-   Drop support for Python 3.8.
+
 2.0.3 "Ugly Merman" (2023-02-16)
 --------------------------------
 
 -   Require bilby_pipe>=1.0.7.
 
 -   Require matplotlib<3.7 to fix bleeding edge dependencies tests.
```

### Comparing `gwcelery-2.0.4/LICENSE.rst` & `gwcelery-2.0.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/README.rst` & `gwcelery-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/Makefile` & `gwcelery-2.0.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/_static/acceptance-tests-checklist.png` & `gwcelery-2.0.5/doc/_static/acceptance-tests-checklist.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/_static/celeryevent-screenshot.png` & `gwcelery-2.0.5/doc/_static/celeryevent-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/_static/deployment-screenshot.png` & `gwcelery-2.0.5/doc/_static/deployment-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/_static/flask-screenshot.png` & `gwcelery-2.0.5/doc/_static/flask-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/_static/flower-screenshot.png` & `gwcelery-2.0.5/doc/_static/flower-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/_static/logo-0.5x.png` & `gwcelery-2.0.5/doc/_static/logo-0.5x.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/_static/logo.png` & `gwcelery-2.0.5/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/_static/sentry-screenshot.png` & `gwcelery-2.0.5/doc/_static/sentry-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/conf.py` & `gwcelery-2.0.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/configuration.rst` & `gwcelery-2.0.5/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/contributing.rst` & `gwcelery-2.0.5/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/deployment.rst` & `gwcelery-2.0.5/doc/deployment.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/design.rst` & `gwcelery-2.0.5/doc/design.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/gwcelery.tasks.detchar.rst` & `gwcelery-2.0.5/doc/gwcelery.tasks.detchar.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/gwcelery.tasks.em_bright.rst` & `gwcelery-2.0.5/doc/gwcelery.tasks.em_bright.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/gwcelery.tasks.external_triggers.rst` & `gwcelery-2.0.5/doc/gwcelery.tasks.external_triggers.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/gwcelery.tasks.orchestrator.rst` & `gwcelery-2.0.5/doc/gwcelery.tasks.orchestrator.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/gwcelery.tasks.rst` & `gwcelery-2.0.5/doc/gwcelery.tasks.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/gwcelery.tasks.superevents.rst` & `gwcelery-2.0.5/doc/gwcelery.tasks.superevents.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/htcondor.rst` & `gwcelery-2.0.5/doc/htcondor.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/index.rst` & `gwcelery-2.0.5/doc/index.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/make.bat` & `gwcelery-2.0.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/monitoring.rst` & `gwcelery-2.0.5/doc/monitoring.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/doc/quickstart.rst` & `gwcelery-2.0.5/doc/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/__init__.py` & `gwcelery-2.0.5/gwcelery/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/_version.py` & `gwcelery-2.0.5/gwcelery/_version.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/conf/__init__.py` & `gwcelery-2.0.5/gwcelery/conf/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 
 igwn_alert_group = 'gracedb-playground'
 """IGWN alert group."""
 
 gracedb_host = 'gracedb-playground.ligo.org'
 """GraceDB host."""
 
+create_mattermost_channel = False
+"""Do not create Mattermost channel."""
+
 voevent_broadcaster_address = ':5342'
 """The VOEvent broker will bind to this address to send GCNs.
 This should be a string of the form `host:port`. If `host` is empty,
 then listen on all available interfaces."""
 
 voevent_broadcaster_whitelist = []
 """List of hosts from which the broker will accept connections.
@@ -164,14 +167,15 @@
 check_vector_prepost = {'gstlal': [2, 2],
                         'spiir': [2, 2],
                         'pycbc': [2, 2],
                         'MBTA': [2, 2],
                         'oLIB': [1.5, 1.5],
                         'LIB': [1.5, 1.5],
                         'CWB': [1.5, 1.5],
+                        'MLy': [1.5, 1.5],
                         'HardwareInjection': [2, 2],
                         'Swift': [2, 2],
                         'Fermi': [2, 2],
                         'INTEGRAL': [2, 2],
                         'AGILE': [2, 2],
                         'SNEWS': [10, 10]}
 """Seconds before and after the superevent start and end times which the DQ
@@ -180,14 +184,15 @@
 uses_gatedhoft = {'gstlal': True,
                   'spiir': True,
                   'pycbc': True,
                   'MBTA': True,
                   'oLIB': False,
                   'LIB': False,
                   'CWB': True,
+                  'MLy': False,
                   'HardwareInjection': False,
                   'Swift': False,
                   'Fermi': False,
                   'INTEGRAL': False,
                   'AGILE': False,
                   'SNEWS': False}
 """Whether or not a pipeline uses gated h(t). Determines whether or not
@@ -220,14 +225,15 @@
 idq_veto = {'gstlal': False,
             'spiir': False,
             'pycbc': False,
             'MBTA': False,
             'oLIB': False,
             'LIB': False,
             'CWB': False,
+            'MLy': False,
             'HardwareInjection': False,
             'Swift': False,
             'Fermi': False,
             'INTEGRAL': False,
             'AGILE': False,
             'SNEWS': False}
 """If true for a pipeline, iDQ values below the threshold defined in
```

### Comparing `gwcelery-2.0.4/gwcelery/conf/minikube.py` & `gwcelery-2.0.5/gwcelery/conf/minikube.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/conf/playground.py` & `gwcelery-2.0.5/gwcelery/conf/playground.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/conf/production.py` & `gwcelery-2.0.5/gwcelery/conf/production.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
 igwn_alert_group = 'gracedb'
 """IGWN alert group."""
 
 gracedb_host = 'gracedb.ligo.org'
 """GraceDB host."""
 
+create_mattermost_channel = True
+"""Create Mattermost channel in production"""
+
 kafka_alert_config = {
     'scimma': {'url': 'kafka://kafka.scimma.org/igwn.gwalert',
                'suffix': 'avro', 'skymap_encoder': lambda _: _},
     'gcn': {'url': 'kafka://kafka.gcn.nasa.gov/igwn.gwalert',
             'suffix': 'json', 'skymap_encoder': lambda b:
             b64encode(b).decode('utf-8')}
 }
```

### Comparing `gwcelery-2.0.4/gwcelery/conf/test.py` & `gwcelery-2.0.5/gwcelery/conf/test.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/data/first2years/gstlal.xml.gz` & `gwcelery-2.0.5/gwcelery/data/first2years/gstlal.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/data/gwcelery.sub` & `gwcelery-2.0.5/gwcelery/data/gwcelery.sub`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/email/bootsteps.py` & `gwcelery-2.0.5/gwcelery/email/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/email/signals.py` & `gwcelery-2.0.5/gwcelery/email/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/flask.py` & `gwcelery-2.0.5/gwcelery/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/igwn_alert/__init__.py` & `gwcelery-2.0.5/gwcelery/igwn_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/igwn_alert/bootsteps.py` & `gwcelery-2.0.5/gwcelery/igwn_alert/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/igwn_alert/signals.py` & `gwcelery-2.0.5/gwcelery/igwn_alert/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/kafka/bootsteps.py` & `gwcelery-2.0.5/gwcelery/kafka/bootsteps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+from functools import cache
+
 from celery import bootsteps
 from celery.concurrency import solo
 from celery.utils.log import get_logger
 from confluent_kafka.error import KafkaException
 from fastavro.schema import parse_schema
 from hop import stream
 from hop.io import list_topics
 from hop.models import AvroBlob, JSONBlob
 
-from ..util import PromiseProxy, read_json
+from ..util import read_json
 
 
 __all__ = ('Producer',)
 
 log = get_logger(__name__)
 
 
-@PromiseProxy
+@cache
 def schema():
     # The order does not matter other than the Alert schema must be loaded last
     # because it references the other schema. All of the schema are saved in
     # named_schemas, but we only need to save a reference to the the Alert
     # schema to write the packet.
     # NOTE Specifying expand=True when calling parse_schema is okay when only
     # one schema contains references to other schema, in our case only the
@@ -38,20 +40,15 @@
 
     return schema
 
 
 class AvroBlobWrapper(AvroBlob):
 
     def __init__(self, payload):
-        # NOTE fastavro appears to not like something about this PromiseProxy
-        # object. Returning a copy of the object is the only workaround I could
-        # find.
-        # FIXME Understand this behavior and write a less hacky fix. Possibly
-        # switch to using functools.cache once python3.8 support is dropped
-        return super().__init__([payload], schema.copy())
+        return super().__init__([payload], schema())
 
 
 class KafkaWriter:
     '''Class to write to kafka stream and monitor stream health.'''
 
     def __init__(self, config):
         self._config = config
```

### Comparing `gwcelery-2.0.4/gwcelery/sentry/__init__.py` & `gwcelery-2.0.5/gwcelery/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/sentry/integrations/condor.py` & `gwcelery-2.0.5/gwcelery/sentry/integrations/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/sentry/integrations/requests.py` & `gwcelery-2.0.5/gwcelery/sentry/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/sentry/integrations/subprocess.py` & `gwcelery-2.0.5/gwcelery/sentry/integrations/subprocess.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/static/typeahead.css` & `gwcelery-2.0.5/gwcelery/static/typeahead.css`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/static/vega/index.html` & `gwcelery-2.0.5/gwcelery/static/vega/index.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/__init__.py` & `gwcelery-2.0.5/gwcelery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/alerts.py` & `gwcelery-2.0.5/gwcelery/tasks/alerts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 
 from astropy import time
 from celery import group
 from celery.utils.log import get_logger
+import numpy as np
 
 from ..import app
 from . import gracedb
 
 log = get_logger(__name__)
 
 
@@ -41,34 +42,69 @@
         properties = {}
 
     if classification and classification[1] is not None:
         classification = json.loads(classification[1])
     else:
         classification = {}
 
+    duration = None
+    central_frequency = None
+
+    if superevent['preferred_event_data']['group'] == 'Burst':
+        if superevent['preferred_event_data']['pipeline'].lower() == 'cwb':
+            duration = \
+                superevent['preferred_event_data']['extra_attributes'].get(
+                    'MultiBurst', {}).get('duration', None)
+            central_frequency = \
+                superevent['preferred_event_data']['extra_attributes'].get(
+                    'MultiBurst', {}).get('central_freq', None)
+        elif superevent['preferred_event_data']['pipeline'].lower() == 'mly':
+            duration = \
+                superevent['preferred_event_data']['extra_attributes'].get(
+                    'MLyBurst', {}).get('duration', None)
+            central_frequency = \
+                superevent['preferred_event_data']['extra_attributes'].get(
+                    'MLyBurst', {}).get('central_freq', None)
+        elif superevent['preferred_event_data']['pipeline'].lower() == 'olib':
+            quality_mean = \
+                superevent['preferred_event_data']['extra_attributes'].get(
+                     'LalInferenceBurst', {}).get('quality_mean', None)
+            frequency_mean = \
+                superevent['preferred_event_data']['extra_attributes'].get(
+                     'LalInferenceBurst', {}).get('frequency_mean', None)
+            central_frequency = \
+                superevent['preferred_event_data']['extra_attributes'].get(
+                     'LalInferenceBurst', {}).get('frequency_mean', None)
+            duration = quality_mean / (2 * np.pi * frequency_mean)
+        else:
+            raise NotImplementedError(
+                'Duration and central_frequency not implemented for Burst '
+                'pipeline {}'.format(
+                    superevent['preferred_event_data']['pipeline'].lower()
+                )
+            )
+
     alert_dict['event'] = {
         # set 'significant' field based on
         # https://dcc.ligo.org/LIGO-G2300151/public
         'significant': False if alert_type == 'less-significant' else True,
         'time': time.Time(superevent['t_0'], format='gps').utc.isot + 'Z',
         'far': superevent['far'],
         'instruments': sorted(
             superevent['preferred_event_data']['instruments'].split(',')
         ),
         'group': superevent['preferred_event_data']['group'],
         'pipeline': superevent['preferred_event_data']['pipeline'],
         'search': superevent['preferred_event_data']['search'],
         'properties': properties,
-        'classification': classification
+        'classification': classification,
+        'duration': duration,
+        'central_frequency': central_frequency
     }
 
-    # FIXME Need to populate these fields for burst events
-    alert_dict['event']['duration'] = None
-    alert_dict['event']['central_frequency'] = None
-
     return alert_dict
 
 
 @gracedb.task(shared=False)
 def _add_external_coinc_to_alert(alert_dict, superevent,
                                  combined_skymap_filename):
     external_event = gracedb.get_event(superevent['em_type'])
```

### Comparing `gwcelery-2.0.4/gwcelery/tasks/bayestar.py` & `gwcelery-2.0.5/gwcelery/tasks/bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/circulars.py` & `gwcelery-2.0.5/gwcelery/tasks/circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/condor.py` & `gwcelery-2.0.5/gwcelery/tasks/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/core.py` & `gwcelery-2.0.5/gwcelery/tasks/core.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/detchar.py` & `gwcelery-2.0.5/gwcelery/tasks/detchar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/em_bright.py` & `gwcelery-2.0.5/gwcelery/tasks/em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/external_skymaps.py` & `gwcelery-2.0.5/gwcelery/tasks/external_skymaps.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,50 +33,54 @@
 
 COMBINED_SKYMAP_FILENAME_PNG = 'combined-ext.png'
 """Filename of combined sky map plot"""
 
 
 @app.task(shared=False,
           queue='exttrig')
-def create_combined_skymap(se_id, ext_id):
+def create_combined_skymap(se_id, ext_id, preferred_event=None):
     """Creates and uploads the combined LVK-external skymap, uploading to the
-    external trigger GraceDB page and the superevent GraceDB page if
-    indicated. The filename used for the combined sky map will be
-    'combined-ext.multiorder.fits' if the GW sky map is multi-ordered or
-    'combined-ext.fits.gz' if the GW sky map is not.
+    external trigger GraceDB page. The filename used for the combined sky map
+    will be 'combined-ext.multiorder.fits' if the GW sky map is multi-ordered
+    or 'combined-ext.fits.gz' if the GW sky map is not. Will use the GW sky map
+    in from the preferred event if given.
 
     Parameters
     ----------
     se_id : str
         Superevent GraceDB ID
     ext_id: str
         External event GraceDB ID
+    preferred_event: str
+        Preferred event GraceDB ID. If given, use sky map from preferred event
 
     """
-    se_skymap_filename = get_skymap_filename(se_id)
-    ext_skymap_filename = get_skymap_filename(ext_id)
+    # gw_id is either superevent or preferred event graceid
+    gw_id = preferred_event if preferred_event else se_id
+    gw_skymap_filename = get_skymap_filename(gw_id, is_gw=True)
+    ext_skymap_filename = get_skymap_filename(ext_id, is_gw=False)
     # Determine whether GW sky map is multiordered or flat
-    gw_moc = '.multiorder.fits' in se_skymap_filename
+    gw_moc = '.multiorder.fits' in gw_skymap_filename
 
     new_filename = \
         (COMBINED_SKYMAP_FILENAME_MULTIORDER if gw_moc else
          COMBINED_SKYMAP_FILENAME_FLAT)
 
     message = \
         ('Combined LVK-external sky map using {0} and {1}, with {2} and '
-         '{3}'.format(se_id, ext_id, se_skymap_filename, ext_skymap_filename))
+         '{3}'.format(gw_id, ext_id, gw_skymap_filename, ext_skymap_filename))
     message_png = (
         'Mollweide projection of <a href="/api/events/{graceid}/files/'
         '{filename}">{filename}</a>').format(
             graceid=ext_id,
             filename=new_filename)
 
     (
         _download_skymaps.si(
-            se_skymap_filename, ext_skymap_filename, se_id, ext_id
+            gw_skymap_filename, ext_skymap_filename, gw_id, ext_id
         )
         |
         combine_skymaps.s(gw_moc=gw_moc)
         |
         group(
             gracedb.upload.s(
                 new_filename, ext_id, message, ['sky_loc', 'ext_coinc']
@@ -91,22 +95,31 @@
         )
     ).delay()
 
 
 @app.task(autoretry_for=(ValueError,), retry_backoff=10,
           queue='exttrig',
           retry_backoff_max=600)
-def get_skymap_filename(graceid):
+def get_skymap_filename(graceid, is_gw):
     """Get the skymap fits filename.
 
     If not available, will try again 10 seconds later, then 20, then 40, etc.
     until up to 10 minutes after initial attempt.
+
+    Parameters
+    ----------
+    graceid : str
+        GraceDB ID
+    is_gw: bool
+        If True, uses method for superevent or preferred event. Otherwise uses
+        method for external event.
+
     """
     gracedb_log = gracedb.get_log(graceid)
-    if 'S' in graceid:
+    if is_gw:
         # Try first to get a multiordered sky map
         for message in reversed(gracedb_log):
             filename = message['filename']
             v = message['file_version']
             fv = '{},{}'.format(filename, v)
             if filename.endswith('.multiorder.fits') and \
                     "combined-ext." not in filename:
@@ -128,19 +141,19 @@
                     filename.endswith('.fits.gz')) and \
                     "combined-ext." not in filename:
                 return fv
     raise ValueError('No skymap available for {0} yet.'.format(graceid))
 
 
 @app.task(shared=False, queue='exttrig')
-def _download_skymaps(se_filename, ext_filename, se_id, ext_id):
+def _download_skymaps(gw_filename, ext_filename, gw_id, ext_id):
     """Download both superevent and external sky map to be combined."""
-    se_skymap = gracedb.download(se_filename, se_id)
+    gw_skymap = gracedb.download(gw_filename, gw_id)
     ext_skymap = gracedb.download(ext_filename, ext_id)
-    return se_skymap, ext_skymap
+    return gw_skymap, ext_skymap
 
 
 def combine_skymaps_moc_flat(gw_sky, ext_sky, ext_header):
     """This function combines a multiordered (MOC) GW sky map with a flattened
     external one by reweighting the MOC sky map using the values of the
     flattened one.
 
@@ -157,23 +170,31 @@
     ext_ind = ah.lonlat_to_healpix(
         ra_gw, dec_gw, ext_nside,
         order='nested' if ext_header['nest'] else 'ring')
     #  Reweight GW prob density by external sky map probabilities
     gw_sky['PROBDENSITY'] *= ext_sky[ext_ind]
     gw_sky['PROBDENSITY'] /= \
         np.sum(gw_sky['PROBDENSITY'] * areas).value
-    #  Modify GW sky map with new data
-    distmean, diststd = parameters_to_marginal_moments(
-        gw_sky['PROBDENSITY'] * areas.value,
-        gw_sky['DISTMU'], gw_sky['DISTSIGMA'])
-    gw_sky.meta['distmean'], gw_sky.meta['diststd'] = distmean, diststd
-    gw_sky.meta['instruments'].update(ext_header['instruments'])
-    gw_sky.meta['HISTORY'].extend([
-        '', 'The values were reweighted by using data from {}'.format(
-            list(ext_header['instruments'])[0])])
+    #  Modify GW sky map with new data, ensuring they exist first
+    if 'DISTMU' in gw_sky.keys() and 'DISTSIGMA' in gw_sky.keys():
+        distmean, diststd = parameters_to_marginal_moments(
+            gw_sky['PROBDENSITY'] * areas.value,
+            gw_sky['DISTMU'], gw_sky['DISTSIGMA'])
+        gw_sky.meta['distmean'], gw_sky.meta['diststd'] = distmean, diststd
+    if 'instruments' not in ext_header:
+        ext_header.update({'instruments': {'external instrument'}})
+    if 'instruments' in gw_sky.meta:
+        gw_sky.meta['instruments'].update(ext_header['instruments'])
+    if 'HISTORY' in gw_sky.meta:
+        ext_instrument = list(ext_header['instruments'])[0]
+        gw_sky.meta['HISTORY'].extend([
+            '', 'The values were reweighted by using data from {0}{1}'.format(
+                ('an ' if ext_instrument == 'external instrument'
+                 else ''),
+                ext_instrument)])
     return gw_sky
 
 
 @app.task(shared=False, queue='exttrig')
 def combine_skymaps(skymapsbytes, gw_moc=True):
     """This task combines the two input skymaps, in this case the external
     trigger skymap and the LVK skymap and writes to a temporary output file. It
@@ -510,34 +531,40 @@
                          ['sky_loc'])
         |
         gracedb.create_label.si('EXT_SKYMAP_READY', graceid)
     ).delay()
 
 
 @app.task(shared=False)
-def plot_overlap_integral(coinc_far_dict, superevent_id, ext_id,
+def plot_overlap_integral(coinc_far_dict, superevent, ext_event,
                           var_label=r"\mathcal{I}_{\Omega}"):
     """Plot and upload visualization of the sky map overlap integral computed
     by ligo.search.overlap_integral.
 
     Parameters
     ----------
     coinc_far_dict : dict
         Dictionary containing coincidence false alarm rate results from
         RAVEN
-    superevent_id : str
-        superevent GraceDB ID
-    ext_id: str
-        external event GraceDB ID
+    superevent : dict
+        superevent dictionary
+    ext_event : dict
+        external event dictionary
     var_label : str
         The variable symbol used in plotting
 
     """
     if coinc_far_dict['skymap_overlap'] is None:
         return
+    if superevent['em_type'] != ext_event['graceid'] and \
+            'RAVEN_ALERT' in superevent['labels']:
+        return
+
+    superevent_id = superevent['superevent_id']
+    ext_id = ext_event['graceid']
 
     log_overlap = np.log(coinc_far_dict['skymap_overlap'])
     logI_string = np.format_float_positional(log_overlap, 1, trim='0',
                                              sign=True)
     # Create plot
     fig, _ = skymaps.plot_bayes_factor(
         log_overlap, values=(1, 3, 5), xlim=7, var_label=var_label,
```

### Comparing `gwcelery-2.0.4/gwcelery/tasks/external_triggers.py` & `gwcelery-2.0.5/gwcelery/tasks/external_triggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from . import igwn_alert
 from . import raven
 
 log = get_logger(__name__)
 
 
 REQUIRED_LABELS_BY_TASK = {
-    'compare': {'SKYMAP_READY', 'EXT_SKYMAP_READY', 'EM_COINC'},
-    'combine': {'RAVEN_ALERT'},
+    # EM_READY implies preferred event sky map is available
+    'compare': {'EM_READY', 'EXT_SKYMAP_READY', 'EM_COINC'},
     'SoG': {'SKYMAP_READY', 'RAVEN_ALERT', 'ADVOK'}
 }
 """These labels should be present on an external event to consider it to
 be ready for sky map comparison or for post-alert analsis, such as a
 measurment of the speed of gravity (SoG).
 """
 
@@ -46,28 +46,32 @@
     root = etree.fromstring(payload)
 
     #  Get TrigID and Test Event Boolean
     trig_id = root.find("./What/Param[@name='TrigID']").attrib['value']
     ext_group = 'Test' if root.attrib['role'] == 'test' else 'External'
 
     event_observatory = 'SNEWS'
+    if 'mdc-test_event' in root.attrib['ivorn'].lower():
+        search = 'MDC'
+    else:
+        search = 'Supernova'
     query = 'group: External pipeline: {} grbevent.trigger_id = "{}"'.format(
         event_observatory, trig_id)
     events = gracedb.get_events(query=query)
 
     if events and ext_group == 'External':
         # Only update event if real
         assert len(events) == 1, 'Found more than one matching GraceDB entry'
         event, = events
         graceid = event['graceid']
         canvas = gracedb.replace_event.s(graceid, payload)
 
     else:
         canvas = gracedb.create_event.s(filecontents=payload,
-                                        search='Supernova',
+                                        search=search,
                                         group=ext_group,
                                         pipeline=event_observatory)
         canvas |= _launch_external_detchar.s()
 
     canvas.delay()
 
 
@@ -105,17 +109,19 @@
     stream_obsv_dict = {'/SWIFT': 'Swift',
                         '/Fermi': 'Fermi',
                         '/INTEGRAL': 'INTEGRAL',
                         '/AGILE': 'AGILE'}
     event_observatory = stream_obsv_dict[stream_path]
 
     #  Get TrigID
-    if event_observatory == 'INTEGRAL':
+    if event_observatory == 'INTEGRAL' and \
+            not any([x in u.fragment for x in ['O3-replay', 'MDC-test']]):
         #  FIXME: revert all this if INTEGRAL fixes their GCN notices
-        #  If INTGRAL, get trigger ID from ivorn rather than the TrigID field
+        #  If INTEGRAL, get trigger ID from ivorn rather than the TrigID field
+        #  unless O3 replay or MDC event
         trig_id = u.fragment.split('_')[-1].split('-')[0]
         #  Modify the TrigID field so GraceDB has the correct value
         root.find("./What/Param[@name='TrigID']").attrib['value'] = \
             str(trig_id).encode()
         #  Apply changes to payload delivered to GraceDB
         payload = etree.tostring(root, xml_declaration=True, encoding="UTF-8")
     else:
@@ -239,15 +245,15 @@
     This IGWN alert message handler is triggered by creating a new superevent
     or GRB external trigger event, or a label associated with completeness of
     skymaps:
 
     * Any new event triggers a coincidence search with
       :meth:`gwcelery.tasks.raven.coincidence_search`.
     * When both a GW and GRB sky map are available during a coincidence,
-      indicated by the labels ``SKYMAP_READY`` and ``EXT_SKYMAP_READY``
+      indicated by the labels ``EM_READY`` and ``EXT_SKYMAP_READY``
       respectively on the external event, this triggers the spacetime coinc
       FAR to be calculated and a combined GW-GRB sky map is created using
       :meth:`gwcelery.tasks.external_skymaps.create_combined_skymap`.
 
     """
     # Determine GraceDB ID
     graceid = alert['uid']
@@ -305,58 +311,68 @@
                 se_searches = []
             else:
                 se_searches = ['Allsky']
             # launch standard GRB search
             raven.coincidence_search(graceid, alert['object'],
                                      group=gw_group, searches=['GRB'],
                                      se_searches=se_searches)
-    # rerun raven pipeline and create combined sky map (if not a Swift event)
+    # re-run raven pipeline and create combined sky map (if not a Swift event)
     # when sky maps are available
     elif alert['alert_type'] == 'label_added' and \
             alert['object'].get('group') == 'External':
         if _skymaps_are_ready(alert['object'], alert['data']['name'],
                               'compare'):
-            # if both sky maps present and a coincidence, rreun RAVEN
+            # if both sky maps present and a coincidence, re-run RAVEN
             # pipeline and create combined sky maps
             ext_event = alert['object']
             superevent_id, ext_id = _get_superevent_ext_ids(
                 graceid, ext_event)
             superevent = gracedb.get_superevent(superevent_id)
             _relaunch_raven_pipeline_with_skymaps(
                 superevent, ext_event, graceid)
         elif 'EM_COINC' in alert['object']['labels']:
             # if not complete, check if GW sky map; apply label to external
             # event if GW sky map
             se_labels = gracedb.get_labels(alert['object']['superevent'])
             if 'SKYMAP_READY' in se_labels:
                 gracedb.create_label.si('SKYMAP_READY', graceid).delay()
+            if 'EM_READY' in se_labels:
+                gracedb.create_label.si('EM_READY', graceid).delay()
     # apply labels from superevent to external event to update state
     # and trigger functionality requiring sky maps, etc.
     elif alert['alert_type'] == 'label_added' and 'S' in graceid:
         if 'SKYMAP_READY' in alert['object']['labels']:
             # if sky map in superevent, apply label to all external events
             # at the time
             group(
                 gracedb.create_label.si('SKYMAP_READY', ext_id)
                 for ext_id in alert['object']['em_events']
             ).delay()
+        if 'EM_READY' in alert['object']['labels']:
+            # if sky map not in superevent but in preferred event, apply label
+            # to all external events at the time
+            group(
+                gracedb.create_label.si('EM_READY', ext_id)
+                for ext_id in alert['object']['em_events']
+            ).delay()
         if _skymaps_are_ready(alert['object'], alert['data']['name'], 'SoG') \
                 and alert['object']['space_coinc_far'] is not None:
             # if a superevent is vetted by ADVOK and a spatial joint FAR is
             # available, check if SoG publishing conditions are met
             (
                 gracedb.get_event.si(alert['object']['em_type'])
                 |
                 raven.sog_paper_pipeline.s(alert['object'])
             ).delay()
     # if new GW or external sky map after first being available, try to remake
     # combine sky map and rerun raven pipeline
     elif alert['alert_type'] == 'log' and \
             'EM_COINC' in alert['object']['labels'] and \
             'fit' in alert['data']['filename'] and \
+            'flat' not in alert['data']['comment'].lower() and \
             (alert['data']['filename'] not in
              {external_skymaps.COMBINED_SKYMAP_FILENAME_MULTIORDER,
               external_skymaps.COMBINED_SKYMAP_FILENAME_FLAT}):
         superevent_id, external_id = _get_superevent_ext_ids(
                                          graceid, alert['object'])
         if 'S' in graceid:
             superevent = alert['object']
@@ -368,15 +384,16 @@
         if 'S' in graceid:
             # Rerun for all eligible external events
             for ext_id in superevent['em_events']:
                 external_event = gracedb.get_event(ext_id)
                 if REQUIRED_LABELS_BY_TASK['compare'].issubset(
                         set(external_event['labels'])):
                     _relaunch_raven_pipeline_with_skymaps(
-                        superevent, external_event, graceid)
+                        superevent, external_event, graceid,
+                        use_superevent=True)
         else:
             if REQUIRED_LABELS_BY_TASK['compare'].issubset(
                     set(external_event['labels'])):
                 _relaunch_raven_pipeline_with_skymaps(
                     superevent, external_event, graceid)
     elif alert['alert_type'] == 'label_removed' and \
             alert['object'].get('group') == 'External':
@@ -414,24 +431,36 @@
     """
     # Determine GraceDB ID
     graceid = alert['uid']
 
     if alert['alert_type'] == 'new':
         if alert['object'].get('superevent_id'):
             group = alert['object']['preferred_event_data']['group']
+            search = alert['object']['preferred_event_data']['search']
+            if search == 'MDC':
+                raven.coincidence_search(graceid, alert['object'],
+                                         group='Burst', searches=['MDC'],
+                                         pipelines=['SNEWS'])
             # Run on Test and Burst superevents
-            if group in {'Burst', 'Test'}:
+            elif group in {'Burst', 'Test'}:
                 raven.coincidence_search(graceid, alert['object'],
                                          group='Burst', searches=['Supernova'],
                                          pipelines=['SNEWS'])
         else:
             # Run on SNEWS event, either real or test
-            raven.coincidence_search(graceid, alert['object'],
-                                     group='Burst', searches=['Supernova'],
-                                     pipelines=['SNEWS'])
+            search = alert['object']['search']
+            if search == 'MDC':
+                raven.coincidence_search(graceid, alert['object'],
+                                         group='Burst',
+                                         se_searches=['MDC'],
+                                         pipelines=['SNEWS'])
+            elif search == 'Supernova':
+                raven.coincidence_search(graceid, alert['object'],
+                                         group='Burst', searches=['Supernova'],
+                                         pipelines=['SNEWS'])
 
 
 def _skymaps_are_ready(event, label, task):
     label_set = set(event['labels'])
     required_labels = REQUIRED_LABELS_BY_TASK[task]
     return required_labels.issubset(label_set) and label in required_labels
 
@@ -446,37 +475,41 @@
     return se_id, ext_id
 
 
 @app.task(queue='exttrig',
           shared=False)
 def _launch_external_detchar(event):
     start = event['gpstime']
-    if event['search'] == 'Supernova':
+    if event['pipeline'] == 'SNEWS':
         start, end = event['gpstime'], event['gpstime']
     else:
         integration_time = \
             event['extra_attributes']['GRB']['trigger_duration'] or 4.0
         end = start + integration_time
     detchar.check_vectors.si(event, event['graceid'], start, end).delay()
 
     return event
 
 
-def _relaunch_raven_pipeline_with_skymaps(superevent, ext_event, graceid):
-    """Relaunch the RAVEN sky map comparision workflow, include recalculating
+def _relaunch_raven_pipeline_with_skymaps(superevent, ext_event, graceid,
+                                          use_superevent=False):
+    """Relaunch the RAVEN sky map comparison workflow, include recalculating
     the joint FAR with updated sky map info and create a new combined sky map.
 
     Parameters
     ----------
     superevent: dict
         superevent dictionary
     exttrig: dict
         external event dictionary
     graceid: str
         GraceDB ID of event
+    use_superevent: bool
+        If True, always use skymap info from superevent
+        regardless of SKYMAP_READY label.
 
     """
     gw_group = superevent['preferred_event_data']['group']
     tl, th = raven._time_window(graceid, gw_group,
                                 [ext_event['pipeline']],
                                 [ext_event['search']])
     # FIXME: both overlap integral and combined sky map could be
@@ -488,9 +521,13 @@
                  tl, th, gw_group)
     # Swift localizations are incredibly well localized and require
     # a different method from Fermi/Integral/AGILE
     # FIXME: Add Swift localization information in the future
     if ext_event['pipeline'] != 'Swift':
         # Create new updated combined sky map
         canvas |= external_skymaps.create_combined_skymap.si(
-                      superevent['superevent_id'], ext_event['graceid'])
+                      superevent['superevent_id'], ext_event['graceid'],
+                      preferred_event=(
+                          None if 'SKYMAP_READY' in ext_event['labels']
+                          or use_superevent
+                          else superevent['preferred_event']))
     canvas.delay()
```

### Comparing `gwcelery-2.0.4/gwcelery/tasks/first2years.py` & `gwcelery-2.0.5/gwcelery/tasks/first2years.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import lal
 from ligo.skymap.io.events.ligolw import ContentHandler
 import numpy as np
 
 from .core import get_last
 from ..data import first2years as data_first2years
 from ..import app
-from . import gracedb
+from . import gracedb, first2years_external
 
 log = get_task_logger(__name__)
 
 
 def pick_coinc():
     """Pick a coincidence from the "First Two Years" paper."""
     with resources.open_binary(data_first2years, 'gstlal.xml.gz') as f:
@@ -150,14 +150,15 @@
 def setup_periodic_tasks(sender, **kwargs):
     """Register periodic tasks.
 
     See
     https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html.
     """
     sender.add_periodic_task(3600.0, upload_event)
+    sender.add_periodic_task(7200.0, first2years_external.upload_snews_event)
 
 
 @app.task(ignore_result=True, shared=False)
 def upload_event():
     """Upload a random event from the "First Two Years" paper.
 
     After 2 minutes, randomly either retract or confirm the event to send a
```

### Comparing `gwcelery-2.0.4/gwcelery/tasks/first2years_external.py` & `gwcelery-2.0.5/gwcelery/tasks/first2years_external.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,31 +9,38 @@
 import re
 
 from ..import app
 from . import external_triggers
 from . import igwn_alert
 
 
-def create_grb_event(gpstime, pipeline, se_search):
-    """ Create a random GRB event for a certain percentage of MDC or O3-replay
-     superevents.
+def create_external_event(gpstime, pipeline, se_search):
+    """ Create a random external event VOEvent.
 
     Parameters
     ----------
     gpstime : float
         Event's gps time
     pipeline : str
         External trigger pipeline name
     se_search : str
         Search field for preferred event, 'MDC' or 'AllSky'
     """
     new_date = str(Time(gpstime, format='gps', scale='utc').isot) + 'Z'
     new_TrigID = str(int(gpstime))
+
+    if pipeline in {'Fermi', 'Swift', 'INTEGRAL', 'AGILE'}:
+        is_grb = True
+    else:
+        is_grb = False
+
     fname = str(Path(__file__).parent /
-                '../tests/data/{}_grb_gcn.xml'.format(pipeline.lower()))
+                '../tests/data/{0}_{1}gcn.xml'.format(
+                    pipeline.lower(),
+                    'grb_' if is_grb else ''))
 
     root = etree.parse(fname)
     # Change ivorn to indicate if this is an MDC event or O3 replay event
     root.xpath('.')[0].attrib['ivorn'] = \
         'ivo://lvk.internal/{0}#{1}_event{2}'.format(
             pipeline if pipeline != 'Swift' else 'SWIFT',
             'MDC-test' if se_search == 'MDC' else 'O3-replay',
@@ -43,29 +50,31 @@
     root.find("./Who/Date").text = str(new_date).encode()
     root.find(("./WhereWhen/ObsDataLocation/"
                "ObservationLocation/AstroCoords/Time/TimeInstant/"
                "ISOTime")).text = str(new_date).encode()
     root.find("./What/Param[@name='TrigID']").attrib['value'] = \
         str(new_TrigID).encode()
 
-    # Give random sky position
-    root.find(("./WhereWhen/ObsDataLocation/"
-               "ObservationLocation/AstroCoords/Position2D/Value2/"
-               "C1")).text = str(random.uniform(0, 360)).encode()
-    thetas = np.arange(-np.pi / 2, np.pi / 2, .01)
-    root.find(("./WhereWhen/ObsDataLocation/"
-               "ObservationLocation/AstroCoords/Position2D/Value2/"
-               "C2")).text = \
-        str(random.choices(
-            np.rad2deg(thetas),
-            weights=np.cos(thetas) / sum(np.cos(thetas)))[0]).encode()
-    if pipeline != 'Swift':
+    if is_grb:
+        # Give random sky position
+        root.find(("./WhereWhen/ObsDataLocation/"
+                   "ObservationLocation/AstroCoords/Position2D/Value2/"
+                   "C1")).text = str(random.uniform(0, 360)).encode()
+        thetas = np.arange(-np.pi / 2, np.pi / 2, .01)
         root.find(("./WhereWhen/ObsDataLocation/"
-                   "ObservationLocation/AstroCoords/Position2D/"
-                   "Error2Radius")).text = str(random.uniform(1, 30)).encode()
+                   "ObservationLocation/AstroCoords/Position2D/Value2/"
+                   "C2")).text = \
+            str(random.choices(
+                np.rad2deg(thetas),
+                weights=np.cos(thetas) / sum(np.cos(thetas)))[0]).encode()
+        if pipeline != 'Swift':
+            root.find(
+                ("./WhereWhen/ObsDataLocation/"
+                 "ObservationLocation/AstroCoords/Position2D/"
+                 "Error2Radius")).text = str(random.uniform(1, 30)).encode()
 
     return etree.tostring(root, xml_declaration=True, encoding="UTF-8",
                           pretty_print=True)
 
 
 def _offset_time(gpstime, group):
     """ This function checks coincident time windows for superevents if they
@@ -145,15 +154,26 @@
     for i in range(num):
         gpstime = float(alert['object']['t_0'])
         new_time = _offset_time(gpstime, group)
 
         # Choose external grb pipeline to simulate
         pipeline = np.random.choice(['Fermi', 'Swift', 'INTEGRAL', 'AGILE'],
                                     p=[.5, .3, .1, .1])
-        ext_event = create_grb_event(new_time, pipeline, se_search)
+        ext_event = create_external_event(new_time, pipeline, se_search)
 
         # Upload as from GCN
         external_triggers.handle_grb_gcn(ext_event)
 
         events.append(ext_event), pipelines.append(pipeline)
 
     return events, pipelines
+
+
+@app.task(queue='exttrig',
+          ignore_result=True,
+          shared=False)
+def upload_snews_event():
+    """Create and upload a SNEWS-like MDC external event."""
+    current_time = Time(Time.now(), format='gps').value
+    ext_event = create_external_event(current_time, 'SNEWS', 'MDC')
+    external_triggers.handle_snews_gcn(ext_event)
+    return ext_event
```

### Comparing `gwcelery-2.0.4/gwcelery/tasks/gcn.py` & `gwcelery-2.0.5/gwcelery/tasks/gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/gracedb.py` & `gwcelery-2.0.5/gwcelery/tasks/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/igwn_alert.py` & `gwcelery-2.0.5/gwcelery/tasks/igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/inference.py` & `gwcelery-2.0.5/gwcelery/tasks/inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Source Parameter Estimation with LALInference, Bilby, and RapidPE."""
 from distutils.spawn import find_executable
 from distutils.dir_util import mkpath
 import glob
 import json
 import os
-import shutil
 import subprocess
 import urllib
 
+from bilby_pipe.utils import convert_string_to_dict
+from bilby_pipe.bilbyargparser import BilbyConfigFileParser
 from celery import group
 from gwdatafind import find_urls
 import numpy as np
 
 from .. import app
 from ..jinja import env
 from . import condor
@@ -244,15 +245,14 @@
         contents = b'args:\n' + json.dumps(e.args[1]).encode('utf-8') + \
                    b'\n\nstdout:\n' + e.stdout + b'\n\nstderr:\n' + e.stderr
         gracedb.upload.delay(
             filecontents=contents, filename='lalinference_dag.log',
             graceid=superevent_id,
             message='Failed to prepare DAG for lalinference', tags='pe'
         )
-        shutil.rmtree(rundir)
         raise
 
     return os.path.join(rundir, 'multidag.dag')
 
 
 @app.task(shared=False)
 def _setup_dag_for_bilby(coinc, rundir, event, superevent_id, mode):
@@ -277,65 +277,69 @@
     -------
     path_to_dag : str
         The path to the .dag file
 
     Notes
     -----
     `--channel-dict o3replay` is added to bilby_pipe_gracedb arguments when the
-    gracedb host is different from `gracedb.ligo.org`.
+    gracedb host is different from `gracedb.ligo.org`. Condor queue is set to
+    `Online_PE` if gracedb host is `gracedb.ligo.org`, and `Online_PE_MDC`
+    otherwise.
 
     """
     path_to_json = os.path.join(rundir, 'event.json')
     with open(path_to_json, 'w') as f:
         json.dump(event, f, indent=2)
 
     path_to_psd = os.path.join(rundir, 'coinc.xml')
     with open(path_to_psd, 'wb') as f:
         f.write(coinc)
 
     path_to_webdir = os.path.join(
-        app.conf['pe_results_path'], superevent_id, 'bilby'
+        app.conf['pe_results_path'], superevent_id, 'bilby', mode
     )
 
     path_to_settings = os.path.join(rundir, 'settings.json')
     setup_arg = ['bilby_pipe_gracedb', '--webdir', path_to_webdir,
                  '--outdir', rundir, '--json', path_to_json,
                  '--psd-file', path_to_psd, '--settings', path_to_settings]
-    if app.conf['gracedb_host'] != 'gracedb.ligo.org':
-        setup_arg += ['--channel-dict', 'o3replay']
     settings = {'summarypages_arguments': {'gracedb': event['graceid'],
                                            'no_ligo_skymap': True},
-                'queue': 'Online_PE',
                 'accounting_user': 'soichiro.morisaki'}
+    if app.conf['gracedb_host'] != 'gracedb.ligo.org':
+        settings['queue'] = 'Online_PE_MDC'
+        setup_arg += ['--channel-dict', 'o3replay']
+    else:
+        settings['queue'] = 'Online_PE'
 
     if mode == 'quick_bns':
         setup_arg += ['--cbc-likelihood-mode', 'lowspin_phenomd_narrowmc_roq']
         settings.update(
             {'sampler_kwargs': {'naccept': 10, 'nlive': 500,
                                 'npool': 24, 'sample': 'acceptance-walk'},
              'n_parallel': 2,
              'request_cpus': 24,
-             'spline_calibration_nodes': 4,
+             'spline_calibration_nodes': 10,
              'request_memory_generation': 8.0}
         )
     elif mode == 'fast_test':
         # use pv2_nrtidalv2 below chirp mass of m1=3Msun, m2=1Msun
         if event['extra_attributes']['CoincInspiral']['mchirp'] < 1.465:
             setup_arg += ['--cbc-likelihood-mode', 'phenompv2nrtidalv2_roq']
             settings['request_memory_generation'] = 8.0
         # use bns-mass pv2 basis for chirp mass range where it is available
         elif event['extra_attributes']['CoincInspiral']['mchirp'] < 3.9:
             setup_arg += ['--cbc-likelihood-mode', 'phenompv2_bns_roq']
             settings['request_memory_generation'] = 8.0
         settings.update(
-            {'sampler_kwargs': {'naccept': 20, 'nlive': 1000,
+            {'sampler_kwargs': {'naccept': 60, 'nlive': 500,
                                 'npool': 24, 'sample': 'acceptance-walk'},
              'n_parallel': 2,
              'request_cpus': 24,
-             'spline_calibration_nodes': 4}
+             'spline_calibration_nodes': 10}
         )
     elif mode != 'production':
         raise ValueError(f"mode: {mode} not recognized.")
 
     with open(path_to_settings, 'w') as f:
         json.dump(settings, f, indent=2)
 
@@ -345,15 +349,14 @@
         contents = b'args:\n' + json.dumps(e.args[1]).encode('utf-8') + \
                    b'\n\nstdout:\n' + e.stdout + b'\n\nstderr:\n' + e.stderr
         gracedb.upload.delay(
             filecontents=contents, filename='bilby_dag.log',
             graceid=superevent_id,
             message=f'Failed to prepare DAG for {mode} bilby', tags='pe'
         )
-        shutil.rmtree(rundir)
         raise
     else:
         # Uploads bilby ini file to GraceDB
         with open(os.path.join(rundir, 'bilby_config.ini'), 'r') as f:
             ini_contents = f.read()
         gracedb.upload.delay(
             ini_contents, filename=f'bilby_{mode}_config.ini',
@@ -422,15 +425,14 @@
         contents = b'args:\n' + json.dumps(e.args[1]).encode('utf-8') + \
                    b'\n\nstdout:\n' + e.stdout + b'\n\nstderr:\n' + e.stderr
         gracedb.upload.delay(
             filecontents=contents, filename='rapidpe_dag.log',
             graceid=superevent_id,
             message='Failed to prepare DAG for Rapid PE', tags='pe'
         )
-        shutil.rmtree(rundir)
         raise
 
     # return path to dag
     dag = os.path.join(rundir, "event_all_iterations.dag")
     return dag
 
 
@@ -541,16 +543,22 @@
         )
     else:
         canvas = gracedb.upload.si(
             filecontents=None, filename=None, graceid=superevent_id, tags='pe',
             message=f'The {analysis} condor job failed.'
         )
 
-    # upload all the .log, .err, and .out files
-    for filename in ['*.log', '*.err', '*.out']:
+    if analysis == "rapidpe":
+        to_upload = [
+            'event_all_iterations.dag.lib.err',
+            'marginalize_extrinsic_parameters_iteration_*.dag.lib.err'
+        ]
+    else:
+        to_upload = ['*.log', '*.err', '*.out']
+    for filename in to_upload:
         tasks = []
         for path in _find_paths_from_name(rundir, filename):
             with open(path, 'rb') as f:
                 contents = f.read()
             if contents:
                 # put .log suffix in log file names so that users can directly
                 # read the contents instead of downloading them when they click
@@ -563,27 +571,14 @@
                     tags='pe'
                 ))
         canvas |= group(tasks)
 
     canvas.delay()
 
 
-@app.task(ignore_result=True, shared=False)
-def clean_up(rundir):
-    """Clean up a run directory.
-
-    Parameters
-    ----------
-    rundir : str
-        The path to a run directory where the DAG file exits
-
-    """
-    shutil.rmtree(rundir)
-
-
 def _upload_tasks_lalinference(rundir, superevent_id):
     """Return canvas of tasks to upload LALInference results
 
     Parameters
     ----------
     rundir : str
         The path to a run directory
@@ -690,38 +685,56 @@
     )
 
     with open(out_samples, 'rb') as f:
         canvas = gracedb.upload.si(
             f.read(), samples_filename,
             superevent_id, f'{mode} Bilby posterior samples', 'pe')
 
-    # plots
-    tasks = []
-    resultdir = os.path.join(rundir, 'result')
-    for parameter_type in ['extrinsic', 'intrinsic']:
-        # Here it is not required that only a single png file exists, so that
-        # posterior samples are uploaded whatever.
-        for path in glob.iglob(
-            os.path.join(resultdir, f'*_{parameter_type}_corner.png')
-        ):
-            with open(path, 'rb') as f:
-                tasks.append(gracedb.upload.si(
-                    f.read(), f'Bilby.{mode}.{parameter_type}.png',
-                    superevent_id,
-                    f'{mode} Bilby corner plot for {parameter_type} '
-                    'parameters', 'pe'
-                ))
-    canvas |= group(tasks)
+    # pesummary
+    pesummary_kwargs = {}
+    path_to_ini, = glob.glob(os.path.join(rundir, "*_complete.ini"))
+    pesummary_kwargs["config"] = path_to_ini
+    config_parser = BilbyConfigFileParser()
+    with open(path_to_ini, "r") as f:
+        config_content, _, _, _ = config_parser.parse(f)
+    pesummary_kwargs["psd"] = convert_string_to_dict(
+        config_content["psd-dict"]
+    )
+    pesummary_kwargs["calibration"] = convert_string_to_dict(
+        config_content["spline-calibration-envelope-dict"]
+    )
+    pesummary_kwargs["approximant"] = config_content["waveform-approximant"]
+    pesummary_kwargs["f_low"] = config_content["minimum-frequency"]
+    pesummary_kwargs["f_ref"] = config_content["reference-frequency"]
+
+    webdir = os.path.join(config_content["webdir"], 'pesummary')
+    url = urllib.parse.urljoin(
+        app.conf['pe_results_url'],
+        os.path.relpath(
+            os.path.join(webdir, 'home.html'),
+            app.conf['pe_results_path']
+        )
+    )
+    canvas = group(
+        canvas,
+        _pesummary_task(webdir, in_samples, **pesummary_kwargs)
+        |
+        gracedb.upload.si(
+            None, None, superevent_id,
+            'PESummary page for {mode} Bilby is available '
+            f'<a href={url}>here</a>'
+        )
+    )
 
     return canvas
 
 
 @app.task(ignore_result=True, shared=False)
 def dag_finished(rundir, superevent_id, pe_pipeline, **kwargs):
-    """Upload PE results and clean up run directory
+    """Upload PE results
 
     Parameters
     ----------
     rundir : str
         The path to a run directory where the DAG file exits
     superevent_id : str
         The GraceDB ID of a target superevent
@@ -739,21 +752,59 @@
         # TODO: upload rapidpe posterior samples
         canvas = gracedb.upload.si(
             None, None, superevent_id,
             'Online RapidPE-RIFT parameter estimation finished.', 'pe')
     else:
         raise NotImplementedError(f'Unknown PE pipeline {pe_pipeline}.')
 
-    canvas = canvas | clean_up.si(rundir)
     canvas.delay()
 
     if pe_pipeline == 'bilby':
         gracedb.create_label.delay('PE_READY', superevent_id)
 
 
+def _pesummary_task(webdir, samples, **pesummary_kwargs):
+    """Return a celery task to submit a pesummary condor job.
+
+    Parameters
+    ----------
+    webdir : str
+        output directory
+    samples : str
+        path to posterior sample file
+    **pesummary_kwargs
+        Extra arguments of summarypages
+
+    Returns
+    -------
+    celery task
+
+    """
+    args = [
+        "summarypages", "--webdir", webdir, "--samples", samples,
+        "--gw", "--redshift_method", "exact", "--evolve_spins_fowards"
+    ]
+    for key in pesummary_kwargs:
+        if key in ["psd", "calibration"]:
+            args += [f"--{key}"]
+            for ifo in pesummary_kwargs[key]:
+                args += [f'{ifo}:{pesummary_kwargs[key][ifo]}']
+        else:
+            args += [f"--{key}", pesummary_kwargs[key]]
+    if app.conf['gracedb_host'] != 'gracedb.ligo.org':
+        queue = 'Online_PE_MDC'
+    else:
+        queue = 'Online_PE'
+    return condor.check_output.si(
+        args, request_memory=16000, request_disk=5000, queue=queue,
+        accounting_group="ligo.dev.o4.cbc.pe.bilby",
+        accounting_group_user="soichiro.morisaki",
+    )
+
+
 @app.task(ignore_result=True, shared=False)
 def start_pe(frametype_dict, event, superevent_id, pe_pipeline):
     """Run Parameter Estimation on a given event.
 
     Parameters
     ----------
     frametype_dict : dict
```

### Comparing `gwcelery-2.0.4/gwcelery/tasks/legacy_gracedb.py` & `gwcelery-2.0.5/gwcelery/tasks/legacy_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/notice_text.py` & `gwcelery-2.0.5/gwcelery/tasks/notice_text.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/orchestrator.py` & `gwcelery-2.0.5/gwcelery/tasks/orchestrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from . import gracedb
 from . import inference
 from . import igwn_alert
 from . import p_astro
 from . import skymaps
 from . import superevents
 
+from ligo.rrt_chat import channel_creation
+
 
 @igwn_alert.handler('superevent',
                     'mdc_superevent',
                     shared=False)
 def handle_superevent(alert):
     """Schedule annotations for new superevents.
 
@@ -71,21 +73,25 @@
         label_name = alert['data']['name']
         query = f'superevent: {superevent_id} group: CBC Burst'
         if alert['object']['category'] == 'MDC':
             query += ' MDC'
         elif alert['object']['category'] == 'Test':
             query += ' Test'
 
-        # launch less-significant preliminary alerts on EM_Selected
+        # launch less-significant preliminary alerts on LOW_SIGNIF_LOCKED
         if label_name == superevents.FROZEN_LABEL:
-            # don't launch if EM_SelectedConfident is present
-            if superevents.SIGNIFICANT_LABEL in alert['object']['labels']:
+            # don't launch if EARLY_WARNING or SIGNIF_LOCKED is present
+            skipping_labels = {
+                superevents.SIGNIFICANT_LABEL,
+                superevents.EARLY_WARNING_LABEL
+            }.intersection(alert['object']['labels'])
+            if skipping_labels:
                 gracedb.upload.delay(
                     None, None, superevent_id,
-                    "The superevent already has a significant event, "
+                    "The superevent already has a significant/EW event, "
                     "skipping launching less-significant alert"
                 )
                 return
             (
                 gracedb.upload.s(
                     None,
                     None,
@@ -102,15 +108,15 @@
                     alert['object']['t_end']
                 )
                 |
                 earlywarning_preliminary_alert.s(
                     alert, alert_type='less-significant')
             ).apply_async()
 
-        # launch significant alert on EM_SelectedConfident
+        # launch significant alert on SIGNIF_LOCKED
         elif label_name == superevents.SIGNIFICANT_LABEL:
             # ensure superevent is locked before starting alert workflow
             if superevents.FROZEN_LABEL not in alert['object']['labels']:
                 gracedb.create_label(superevents.FROZEN_LABEL, superevent_id)
 
             (
                 gracedb.get_events.si(query)
@@ -179,23 +185,30 @@
                 gracedb.get_events.si(query)
                 |
                 superevents.select_pipeline_preferred_event.s()
                 |
                 _set_pipeline_preferred_events.s(superevent_id)
             ).apply_async(countdown=app.conf['superevent_clean_up_timeout'])
 
+        elif label_name == 'LOW_SIGNIF_PRELIM_SENT':
+            # similar workflow as the GCN_PRELIM_SENT
+            # except block by condition evaluated at the end of timeout
+            _revise_and_send_second_less_significant_alert.si(
+                    alert, query, superevent_id,
+            ).apply_async(countdown=app.conf['superevent_clean_up_timeout'])
+
         elif label_name == superevents.EARLY_WARNING_LABEL:
             if superevents.SIGNIFICANT_LABEL in alert['object']['labels']:
                 # stop if full BW significant event already present
                 gracedb.upload.delay(
                     None, None, superevent_id,
                     "Superevent superseded by full BW event, skipping EW."
                 )
                 return
-            # start the EW alert pipeline; is blocked by EM_SelectedConfident
+            # start the EW alert pipeline; is blocked by SIGNIF_LOCKED
             # ensure superevent is locked before starting pipeline
             if superevents.FROZEN_LABEL not in alert['object']['labels']:
                 gracedb.create_label(superevents.FROZEN_LABEL, superevent_id)
 
             (
                 gracedb.get_events.si(query)
                 |
@@ -213,14 +226,17 @@
             ).apply_async()
 
         # launch initial/retraction alert on ADVOK/ADVNO
         elif label_name == 'ADVOK':
             initial_alert((None, None, None), alert)
         elif label_name == 'ADVNO':
             retraction_alert(alert)
+        elif label_name == 'ADVREQ':
+            if app.conf['create_mattermost_channel']:
+                _create_mattermost_channel.si(superevent_id).delay()
 
     # check DQV label on superevent, run check_vectors if required
     elif alert['alert_type'] == 'event_added':
         # FIXME Check if this should be changed to 'update' alert_types instead
         # of 'event_added'. 'event_added' seems like it's just a new event in
         # the superevent window, not necessarily an event that should be
         # promoted to preferred event
@@ -277,16 +293,17 @@
     priority = 0 if superevents.should_publish(alert['object']) else 1
 
     # Pipelines that use the GWCelery p-astro method
     # - spiir (all searches)
     # - pycbc for EarlyWarning search
     # - periodic MDC generated by first-two-years (based on gstlal)
     # FIXME: Remove this once all pipelines compute their own p-astro
-    pipelines_stock_p_astro = {('spiir', 'allsky'), ('spiir', 'earlywarning'),
-                               ('pycbc', 'earlywarning'), ('gstlal', 'mdc')}
+    pipelines_stock_p_astro = {('spiir', 'earlywarning'),
+                               ('pycbc', 'earlywarning'),
+                               ('gstlal', 'mdc')}
 
     # em_bright and p_astro calculation
     if alert['alert_type'] == 'new':
         instruments = superevents.get_instruments_in_ranking_statistic(
             alert['object'])
         extra_attributes = alert['object']['extra_attributes']
         snr = superevents.get_snr(alert['object'])
@@ -424,14 +441,32 @@
         gracedb.upload.s(
             '{}.em_bright.json'.format(prefix), superevent_id,
             'em-bright computed from "{}"'.format(info)
         )
     ).delay()
 
 
+@app.task(bind=True, shared=False)
+def _create_mattermost_channel(self, superevent_id):
+    """
+    Creates a mattermost channel when ADVREQ label is applied and
+    posts a cooresponding gracedb link of that event in the channel
+
+    Channel name : O4 RRT {superevent_id}
+
+    Parameters:
+    ------------
+    superevent_id: str
+        The superevent id
+    """
+    gracedb_url = self.app.conf['gracedb_host']
+    channel_creation.rrt_channel_creation(
+        superevent_id, gracedb_url)
+
+
 @app.task(shared=False)
 def _set_pipeline_preferred_events(pipeline_event, superevent_id):
     """Return group for setting pipeline preferred event using
     :meth:`gracedb.add_pipeline_preferred_event`.
 
     Parameters
     ----------
@@ -574,19 +609,46 @@
     if blocking_labels:
         gracedb.upload.delay(
             None, None, superevent_id,
             f"Blocking automated notice due to labels {blocking_labels}"
         )
         return None
     else:
-        gracedb.upload.delay(None, None, superevent_id,
-                             "Sending preliminary notice")
         return files
 
 
+@gracedb.task(shared=False)
+def _revise_and_send_second_less_significant_alert(alert, query,
+                                                   superevent_id):
+    superevent_labels = gracedb.get_labels(superevent_id)
+    blocking_labels = {
+        'ADVREQ', 'ADVOK', 'ADVNO',
+        superevents.SIGNIFICANT_LABEL,
+        superevents.EARLY_WARNING_LABEL,
+    }
+    if blocking_labels.intersection(superevent_labels):
+        return
+
+    (
+        gracedb.get_events.si(query)
+        |
+        superevents.select_preferred_event.s()
+        |
+        _update_superevent_and_return_event_dict.s(superevent_id)
+        |
+        _leave_log_message_and_return_event_dict.s(
+            superevent_id,
+            "Superevent cleaned up before second less-significant alert"
+        )
+        |
+        earlywarning_preliminary_alert.s(
+            alert, alert_type='less-significant')
+    ).delay()
+
+
 @app.task(shared=False)
 def _annotate_fits_and_return_input(input_list, superevent_id):
     """Unpack the output of the skymap, embright, p-astro download group in the
     beginning of the
     :meth:`~gwcelery.tasks.orchestartor.earlywarning_preliminary_alert` canvas
     and call :meth:`~gwcelery.tasks.skymaps.annotate_fits`.
 
@@ -662,15 +724,17 @@
 
     1.   Copy any sky maps and source classification from the preferred event
          to the superevent.
     2.   Create standard annotations for sky maps including all-sky plots by
          calling :meth:`gwcelery.tasks.skymaps.annotate_fits`.
     3.   Create a preliminary VOEvent.
     4.   Send the VOEvent to GCN and notices to SCiMMA and GCN.
-    5.   Apply the GCN_PRELIM_SENT label to the superevent.
+    5.   Apply the GCN_PRELIM_SENT or LOW_SIGNIF_PRELIM_SENT
+         depending on the significant or less-significant alert
+         respectively.
     6.   Create and upload a GCN Circular draft.
     """
     priority = 0 if superevents.should_publish(event) else 1
     preferred_event_id = event['graceid']
     superevent_id = alert['uid']
 
     if event['group'] == 'CBC':
@@ -770,21 +834,28 @@
                  " send alerts for MDC events."))
             canvas.apply_async(priority=priority)
             return
 
     # Send notice and upload GCN circular draft for online events.
     if is_publishable and initiate_voevent:
         # presence of advocate action blocks significant prelim alert
-        # presence of adv action + significant event blocks less-significant
-        # prelim, or EW alert
+        # presence of adv action or significant event blocks EW alert
+        # presence of adv action or significant event or EW event blocks
+        # less significant alert
         blocking_labels = (
             {'ADVOK', 'ADVNO'} if alert_type == 'preliminary'
-            else {superevents.SIGNIFICANT_LABEL, 'ADVOK', 'ADVNO'}
-            if alert_type in ['less-significant', 'earlywarning']
-            else set()
+            else
+            {superevents.SIGNIFICANT_LABEL, 'ADVOK', 'ADVNO'}
+            if alert_type == 'earlywarning'
+            else
+            {superevents.EARLY_WARNING_LABEL, superevents.SIGNIFICANT_LABEL,
+             'ADVOK', 'ADVNO'}
+            if alert_type == 'less-significant'
+            else
+            set()
         )
         canvas |= (
             _proceed_if_not_blocked_by.s(superevent_id, blocking_labels)
             |
             _unpack_args_and_send_earlywarning_preliminary_alert.s(
                 alert, alert_type
             )
@@ -1083,26 +1154,34 @@
 
         gracedb.create_tag.s('public', superevent_id)
     )
 
     if combined_skymap_needed:
         download_andor_expose_group += [combined_skymap_canvas]
 
+    sent_label_canvas = identity.si()
+    if alert_type == 'less-significant':
+        sent_label_canvas = gracedb.create_label.si(
+            'LOW_SIGNIF_PRELIM_SENT',
+            superevent_id
+        )
+    elif alert_type == 'preliminary' or \
+            alert_type == 'earlywarning':
+        sent_label_canvas = gracedb.create_label.si(
+            'GCN_PRELIM_SENT',
+            superevent_id
+        )
+
     canvas = (
         group(download_andor_expose_group)
         |
         group(voevent_canvas, kafka_alert_canvas)
         |
         group(
-            (
-                gracedb.create_label.si('GCN_PRELIM_SENT', superevent_id)
-                if alert_type in {'earlywarning', 'preliminary'}
-                else identity.si()
-            ),
-
+            sent_label_canvas,
             circular_canvas,
         )
     )
 
     canvas.apply_async()
```

### Comparing `gwcelery-2.0.4/gwcelery/tasks/p_astro.py` & `gwcelery-2.0.5/gwcelery/tasks/p_astro.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,20 +167,23 @@
 @igwn_alert.handler('superevent',
                     'mdc_superevent',
                     shared=False)
 def handle(alert):
     """LVAlert handler to plot and upload a visualization of every
     ``*.p_astro.json`` file that is added to a superevent.
     """
+    if alert['alert_type'] != 'log':
+        return
+
     graceid = alert['uid']
     filename = alert['data'].get('filename')
     p_astro_filenames = {f'{pipeline}.p_astro.json' for pipeline in
                          ['gstlal', 'mbta', 'pycbc', 'spiir']}
 
-    if alert['alert_type'] == 'log' and filename in p_astro_filenames:
+    if filename in p_astro_filenames:
         (
             gracedb.download.s(filename, graceid)
             |
             plot.s()
             |
             gracedb.upload.s(
                 filename.replace('.json', '.png'), graceid,
```

### Comparing `gwcelery-2.0.4/gwcelery/tasks/raven.py` & `gwcelery-2.0.5/gwcelery/tasks/raven.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,30 +32,34 @@
     superevent_id = superevent['superevent_id']
     exttrig_id = exttrig['graceid']
 
     #  Don't compute coinc FAR for SNEWS coincidences
     if exttrig['pipeline'] == 'SNEWS':
         return {}
 
-    if {'EXT_SKYMAP_READY', 'SKYMAP_READY'}.issubset(exttrig['labels']):
+    if ({'EXT_SKYMAP_READY', 'SKYMAP_READY'}.issubset(exttrig['labels']) or
+            {'EXT_SKYMAP_READY', 'EM_READY'}.issubset(exttrig['labels'])):
         #  if both sky maps available, calculate spatial coinc far
+        use_preferred_event_skymap = 'SKYMAP_READY' not in exttrig['labels']
         se_skymap = external_skymaps.get_skymap_filename(
-            superevent_id)
+            (superevent['preferred_event'] if use_preferred_event_skymap
+             else superevent_id), is_gw=True)
         ext_skymap = external_skymaps.get_skymap_filename(
-            exttrig_id)
+            exttrig_id, is_gw=False)
 
         return ligo.raven.search.calc_signif_gracedb(
                    superevent_id, exttrig_id, tl, th,
                    se_dict=superevent, ext_dict=exttrig,
                    grb_search=exttrig['search'],
                    se_fitsfile=se_skymap, ext_fitsfile=ext_skymap,
                    se_moc=True, ext_moc=False,
                    use_radec=True if exttrig['pipeline'] == 'Swift' else False,
                    incl_sky=True, gracedb=gracedb.client,
-                   far_grb=exttrig['far'])
+                   far_grb=exttrig['far'],
+                   use_preferred_event_skymap=use_preferred_event_skymap)
     else:
         return ligo.raven.search.calc_signif_gracedb(
                    superevent_id, exttrig_id, tl, th,
                    se_dict=superevent, ext_dict=exttrig,
                    grb_search=exttrig['search'],
                    incl_sky=False, gracedb=gracedb.client,
                    far_grb=exttrig['far'])
@@ -74,14 +78,18 @@
         ID of the trigger used by GraceDB
     alert_object: dict
         Alert dictionary
     group: str
         Burst or CBC
     pipelines: list
         list of external trigger pipeline names
+    searches: list
+        list of external trigger searches
+    se_searches: list
+        list of superevent searches
 
     """
     tl, th = _time_window(gracedb_id, group, pipelines, searches)
 
     (
         search.si(gracedb_id, alert_object, tl, th, group, pipelines,
                   searches, se_searches)
@@ -98,15 +106,17 @@
     gracedb_id: str
         ID of the trigger used by GraceDB
     group: str
         Burst or CBC
     pipelines: list
         list of external trigger pipeline names
     searches: list
-        list of external trigger search names
+        list of external trigger searches
+    se_searches: list
+        list of superevent searches
 
     """
     tl_cbc, th_cbc = app.conf['raven_coincidence_windows']['GRB_CBC']
     tl_subfermi, th_subfermi = \
         app.conf['raven_coincidence_windows']['GRB_CBC_SubFermi']
     tl_subswift, th_subswift = \
         app.conf['raven_coincidence_windows']['GRB_CBC_SubSwift']
@@ -152,14 +162,18 @@
     th: int
         number of seconds to search after
     group: str
         Burst or CBC
     pipelines: list
         list of external trigger pipelines for performing coincidence search
         against
+    searches: list
+        list of external trigger searches
+    se_searches: list
+        list of superevent searches
 
     Returns
     -------
         list with the dictionaries of related gracedb events
 
     """
     return ligo.raven.search.search(gracedb_id, tl, th,
@@ -203,28 +217,32 @@
             superevent = alert_object
             ext_event = result
         else:
             superevent_id = result['superevent_id']
             exttrig_id = gracedb_id
             superevent = result
             ext_event = alert_object
+            # Don't continue if it is a different superevent than previous one.
+            if ext_event['superevent'] is not None \
+                    and ext_event['superevent'] != superevent['superevent_id']:
+                return
 
         canvas = (
             gracedb.add_event_to_superevent.si(superevent_id, exttrig_id)
             |
             calculate_coincidence_far.si(superevent, ext_event, tl, th)
             |
             update_coinc_far.s(superevent, ext_event)
             |
             group(gracedb.create_label.si('EM_COINC', superevent_id),
                   gracedb.create_label.si('EM_COINC', exttrig_id),
                   trigger_raven_alert.s(superevent, gracedb_id,
                                         ext_event, gw_group),
                   external_skymaps.plot_overlap_integral.s(
-                      superevent_id, exttrig_id))
+                      superevent, ext_event))
         )
         canvas.delay()
 
 
 @app.task(queue='exttrig',
           shared=False)
 def preferred_superevent(raven_search_results):
@@ -297,18 +315,23 @@
         snews_to_grb = \
             (emtype_event['pipeline'] == 'SNEWS' and
              ext_event['pipeline'] != 'SNEWS')
         #  Determine which events are likely real or not
         is_old_grb_real, is_new_grb_real = \
             ('NOT_GRB' not in emtype_event['labels'],
              'NOT_GRB' not in ext_event['labels'])
-        #  Use new event if real
-        is_event_improved = is_new_grb_real
+        is_old_raven_alert, is_new_raven_alert = \
+            ('RAVEN_ALERT' in emtype_event['labels'],
+             'RAVEN_ALERT' in ext_event['labels'])
+        #  Use new event only if it is better old event information
+        is_event_improved = ((is_new_grb_real and not is_old_grb_real) or
+                             (is_new_raven_alert and not is_old_raven_alert))
         #  if both real or both not, use FAR to differentiate
-        if is_old_grb_real == is_new_grb_real:
+        if is_old_grb_real == is_new_grb_real \
+                and is_old_raven_alert == is_new_raven_alert:
             is_event_improved = is_far_improved
     else:
         snews_to_grb = False
         is_event_improved = is_far_improved
 
     if is_event_improved and not snews_to_grb:
         gracedb.update_superevent(superevent_id, em_type=ext_id,
@@ -324,15 +347,15 @@
     """Determine whether an event should be published as a preliminary alert.
     If yes, then triggers an alert by applying `RAVEN_ALERT` to the preferred
     event.
 
     All of the following conditions must be true for a preliminary alert:
 
     *   The external event must be a threshold GRB or SNEWS event.
-    *   If triggered on a SNEW event, the GW false alarm rate must pass
+    *   If triggered on a SNEWS event, the GW false alarm rate must pass
         :obj:`~gwcelery.conf.snews_gw_far_threshold`.
     *   The event's RAVEN coincidence false alarm rate, weighted by the
         group-specific trials factor as specified by the
         :obj:`~gwcelery.conf.preliminary_alert_trials_factor` configuration
         setting, is less than or equal to
         :obj:`~gwcelery.conf.preliminary_alert_far_threshold`.
     *   If the external event is from Swift, both sky maps must be present.
@@ -353,15 +376,15 @@
 
     """
     preferred_gwevent_id = superevent['preferred_event']
     superevent_id = superevent['superevent_id']
     ext_id = ext_event['graceid']
     gw_group = gw_group.lower()
     pipeline = ext_event['pipeline']
-    trials_factor = app.conf['preliminary_alert_trials_factor'][gw_group]
+    trials_factor = app.conf['significant_alert_trials_factor'][gw_group]
     missing_skymap = True
     messages = []
 
     #  Since the significance of SNEWS triggers is so high, we will publish
     #  any trigger coincident with a decently significant GW candidate
     if 'SNEWS' == pipeline:
         gw_far = superevent['far']
@@ -387,42 +410,40 @@
         if space_coinc_far is not None:
             coinc_far = space_coinc_far
             missing_skymap = False
         else:
             coinc_far = time_coinc_far
 
         far_type = 'joint'
-        far_threshold = app.conf['preliminary_alert_far_threshold'][gw_group]
+        far_threshold = app.conf['significant_alert_far_threshold'][gw_group]
         coinc_far_f = coinc_far * trials_factor * (trials_factor - 1.)
         pass_far_threshold = coinc_far_f <= far_threshold
 
     #  Get most recent labels to prevent race conditions
     ext_labels = gracedb.get_labels(ext_id)
     no_previous_alert = {'RAVEN_ALERT'}.isdisjoint(ext_labels)
     likely_real_ext_event = {'NOT_GRB'}.isdisjoint(ext_labels)
     is_test_event = (superevent['preferred_event_data']['group'] == 'Test' or
                      ext_event['group'] == 'Test')
 
     #  If publishable, trigger an alert by applying `RAVEN_ALERT` label to
     #  preferred event
     if pass_far_threshold and not is_ext_subthreshold and \
             likely_real_ext_event and not missing_skymap and \
-            not is_test_event:
-        messages.append('RAVEN: publishing criteria met for {0}-{1}'.format(
-            preferred_gwevent_id, ext_id))
-        if no_previous_alert:
-            messages.append('Triggering RAVEN alert for {0}-{1}'.format(
-                preferred_gwevent_id, ext_id))
-            (
-                gracedb.create_label.si('RAVEN_ALERT', superevent_id)
-                |
-                gracedb.create_label.si('RAVEN_ALERT', ext_id)
-                |
-                gracedb.create_label.si('RAVEN_ALERT', preferred_gwevent_id)
-            ).delay()
+            not is_test_event and no_previous_alert:
+        messages.append(('RAVEN: publishing criteria met for {0}-{1}. '
+                         'Triggering RAVEN alert'.format(
+                             preferred_gwevent_id, ext_id)))
+        (
+            gracedb.create_label.si('RAVEN_ALERT', superevent_id)
+            |
+            gracedb.create_label.si('RAVEN_ALERT', ext_id)
+            |
+            gracedb.create_label.si('RAVEN_ALERT', preferred_gwevent_id)
+        ).delay()
     if not pass_far_threshold:
         messages.append(('RAVEN: publishing criteria not met for {0}-{1},'
                          ' {2} FAR (w/ trials) too large '
                          '({3:.4g} > {4:.4g})'.format(
                              preferred_gwevent_id, ext_id, far_type,
                              coinc_far_f, far_threshold)))
     if is_ext_subthreshold:
@@ -433,17 +454,14 @@
         messages.append(('RAVEN: publishing criteria not met for {0}-{1},'
                          ' {1} is likely non-astrophysical.'.format(
                              preferred_gwevent_id, ext_id)))
     if is_test_event:
         messages.append('RAVEN: {0}-{1} is non-astrophysical, '
                         'at least one event is a Test event'.format(
                             preferred_gwevent_id, ext_id))
-    if not no_previous_alert:
-        messages.append(('RAVEN: Alert already triggered for {}'.format(
-                            ext_id)))
     if missing_skymap:
         messages.append('RAVEN: Will only publish GRB coincidence '
                         'if spatial-temporal FAR is present. '
                         'Waiting for both sky maps to be available '
                         'first.')
     for message in messages:
         gracedb.upload.si(None, None, superevent_id, message,
```

### Comparing `gwcelery-2.0.4/gwcelery/tasks/skymaps.py` & `gwcelery-2.0.5/gwcelery/tasks/skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tasks/superevents.py` & `gwcelery-2.0.5/gwcelery/tasks/superevents.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
     'cbc': {'PASTRO_READY', 'EMBRIGHT_READY', 'SKYMAP_READY'},
     'burst': {'SKYMAP_READY'}
 }
 """These labels should be present on an event to consider it to
 be complete.
 """
 
-FROZEN_LABEL = 'EM_Selected'
+FROZEN_LABEL = 'LOW_SIGNIF_LOCKED'
 """This label indicates that the superevent manager should make no further
 changes to the preferred event."""
 
-SIGNIFICANT_LABEL = 'EM_SelectedConfident'
+SIGNIFICANT_LABEL = 'SIGNIF_LOCKED'
 """This label indicates that the superevent is elevated to significant"""
 
 EARLY_WARNING_LABEL = 'EARLY_WARNING'
 """This label indicates that the superevent contains a significant
 early warning event."""
 
 EARLY_WARNING_SEARCH_NAME = 'EarlyWarning'
@@ -386,15 +386,15 @@
 
     Returns
     -------
     dict
         pipeline, graceid pairs
     """
     g_events = list(
-        filterfalse(lambda x: x['graceid'].startswith('E'), events))
+        filterfalse(lambda x: x['group'] == "External", events))
     g_events_by_pipeline = groupby(
         sorted(g_events, key=lambda x: x['pipeline']),
         key=lambda x: x['pipeline']
     )
 
     return dict(
         (k, select_preferred_event(g)) for k, g in g_events_by_pipeline)
@@ -407,17 +407,16 @@
 
     Parameters
     ----------
     events : list
         list of event dictionaries
 
     """
-    # FIXME: Requires robust determination of an External event
     g_events = list(
-        filterfalse(lambda x: x['graceid'].startswith('E'), events))
+        filterfalse(lambda x: x['group'] == "External", events))
     return max(g_events, key=keyfunc)
 
 
 def is_complete(event):
     """
     Determine if a G event is complete in the sense of the event
     has its data products complete i.e. has PASTRO_READY, SKYMAP_READY,
@@ -586,15 +585,15 @@
     kwargs = {}
     if t_start is not None:
         kwargs['t_start'] = t_start
     if t_end is not None:
         kwargs['t_end'] = t_end
     if FROZEN_LABEL not in superevent_labels:
         if keyfunc(new_event_dict) > keyfunc(preferred_event_dict):
-            # update preferred event when EM_Selected is not applied
+            # update preferred event when LOW_SIGNIF_LOCKED is not applied
             kwargs['t_0'] = t_0
             kwargs['preferred_event'] = new_event_dict['graceid']
 
     if kwargs:
         gracedb.update_superevent(superevent_id, **kwargs)
 
     # completeness takes first precedence in deciding preferred event
```

### Comparing `gwcelery-2.0.4/gwcelery/templates/fits_header.jinja2` & `gwcelery-2.0.5/gwcelery/templates/fits_header.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/templates/index.jinja2` & `gwcelery-2.0.5/gwcelery/templates/index.jinja2`

 * *Files 3% similar despite different names*

```diff
@@ -255,14 +255,67 @@
                     </div>
                 </div>
             </form>
         </div>
     </div>
     <div class="card mb-3">
         <div class=card-header>
+            Change Pipeline-Preferred Event in Superevent
+        </div>
+        <div class=card-body>
+            <form method=post action="{{ url_for('change_pipeline_preferred_event') }}">
+                <div class=form-row>
+                    <div class=form-group>
+                        <div class=form-text>Change the pipeline preferred event of a superevent. Do not send any preliminary or update GCN Notice.</div>
+                    </div>
+                </div>
+                <div class="form-row">
+                    <div class="form-group col-md">
+                        <label for=superevent_id>Superevent ID</label>
+                        <input required name=superevent_id class="form-control typeahead">
+                    </div>
+                    <div class="form-group col-md">
+                        <label for=pipeline>Pipeline</label>
+                        <input required name=pipeline class="form-control typeahead">
+                    </div>
+                    <div class="form-group col-md">
+                        <label for=event_id>Preferred event ID</label>
+                        <input required name=event_id class="form-control typeahead" data-typeahead-url-template="{{ url_for('typeahead_event_id', superevent_id='SUPEREVENT_ID') }}">
+                    </div>
+                    <div class="form-group col-md">
+                        <label for=submit-button class=w-100>&nbsp;</label>
+                        <button type=submit id=submit-button name=submit-button class="btn btn-primary">Submit</button>
+                    </div>
+                </div>
+                <div class="modal fade" tabindex=-1 role=dialog aria-labelledby=change-preferred-event-confirm-label>
+                    <div class=modal-dialog role=document>
+                        <div class=modal-content>
+                            <div class=modal-header>
+                                <h5 class=modal-title id=change-preferred-event-confirm-label>
+                                    Really Change Pipeline-Preferred Event?
+                                </h5>
+                                <button type=button class=close data-dismiss=modal aria-label=Close>
+                                    <span aria-hidden="true">&times;</span>
+                                </button>
+                            </div>
+                            <div class=modal-body>
+                                Are you sure that you want to change the pipeline-preferred event?
+                            </div>
+                            <div class=modal-footer>
+                                <button type=button class="btn btn-secondary" data-dismiss=modal>Cancel</button>
+                                <button type=submit class="btn btn-danger">Submit</button>
+                            </div>
+                        </div>
+                    </div>
+                </div>
+            </form>
+        </div>
+    </div>
+    <div class="card mb-3">
+        <div class=card-header>
             Designate External Coincidence
         </div>
         <div class=card-body>
             <form method=post action="{{ url_for('apply_raven_labels') }}">
                 <div class=form-row>
                      <div class=form-group>
                         <div class=form-text>Apply RAVEN alert labels. These will launch a public alert if none have been issued for the superevent.</div>
```

#### html2text {}

```diff
@@ -58,14 +58,25 @@
 Superevent ID [superevent_id       ]
 Preferred event ID [event_id            ]
   Submit
 ** Really Change Preferred Event? **
  ×
 Are you sure that you want to change the preferred event?
 Cancel Submit
+Change Pipeline-Preferred Event in Superevent
+Change the pipeline preferred event of a superevent. Do not send any
+preliminary or update GCN Notice.
+Superevent ID [superevent_id       ]
+Pipeline [pipeline            ]
+Preferred event ID [event_id            ]
+  Submit
+** Really Change Pipeline-Preferred Event? **
+ ×
+Are you sure that you want to change the pipeline-preferred event?
+Cancel Submit
 Designate External Coincidence
 Apply RAVEN alert labels. These will launch a public alert if none have been
 issued for the superevent.
 Warning: this assumes a coincidence has been found, denoted by the presence of
 a EM_COINC label.
 Superevent ID [superevent_id       ]
 External event ID [ext_id              ]
```

### Comparing `gwcelery-2.0.4/gwcelery/templates/lalinference.jinja2` & `gwcelery-2.0.5/gwcelery/templates/lalinference.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/templates/rapidpe.jinja2` & `gwcelery-2.0.5/gwcelery/templates/rapidpe.jinja2`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 event_parameters_in_config_file=0
 
 #was n_samples_per_job in old RIT code. This defines how many iterations of rapidPE are run. Before each new iteration a new grid is generated which is finer than the previous grid, and covers a smaller region of intrinsic parameter space (hopefully around the signal)
 n_iterations_per_job=2
 
 #You need to specify an accounting group when submitting jobs to condor. Use this link to determine your accounting tag: https://ldas-gridmon.ligo.caltech.edu/ldg_accounting/user
 #accounting_group=cgca.sim.o3.cbc.pe.lalinferencerapid
-accounting_group=ligo.dev.o4.cbc.pe.rift
+accounting_group=ligo.dev.o4.cbc.pe.lalinferencerapid
+accounting_group_user=soichiro.morisaki
 
 #If the candidate output sub_directory, under the parent directory, it will not be overwritten by default. But if you're just testing things and not making submissions, you can force the overwrite with this option. default=0
 overwrite_existing_event_dag=1
 
 #If this is set, the script will submit the dag. set=0 if not sure everything is working
 submit_dag=0
 #If this is set, an email will be sent to this address once all jobs are complete, and the plotting scripts have run. If you don't want an email per event (likely if you're doing injections studies)  dont set it
@@ -48,29 +49,30 @@
 intrinsic_param_to_search=[mass1,mass2]
 
 web_dir={{ webdir }}
 
 [Event]
 superevent_id={{ superevent_id }}
 frame_data_types={{ frame_data_types | tojson }}
-
+mdc_event_injection_file =/home/vinaya.valsan/rapidPE/RapidPE_RIFT_Developments/RapidPE-RIFT_fork/gracedb_playground_events/injection_campaign_studies/lowlatency-replay-distributions/minSNR-4/injections-minSNR-4.xml.gz
+mdc_time_offset=101760000
 #Anything specified in this section is passed verbatim to rapidpe_compute_intrinsic_grid in generate_initial_grid_based_of_gstlal_O2_overlaps.py
 [InitialGridOnly]
 #mc-min = 5
 #mc-max = 61
 points-per-side=5
 
 [InitialGridSetup]
 #The arguments in this section are passed directly to the command line in the condor dag job which does the grid refinement. Do not include any arguments which change per iteration or per node.
 ##NOTE: The script is currently setup to work with rapidpe_compute_intrinsic_grid or util_ConstructIntrinsicPosterior.py
 
 [GridRefine]
 no-exact-match=
 #distance-coordinates=tau0_tau3
-distance-coordinates=mchirp_eta
+distance-coordinates=mchirp_q
 #distance-coordinates=mchirp_q
 overlap-thresh=0.99
 verbose=
 #get rid of this one intrinsic-param=[mass1,mass2]
 intrinsic-param=[mass1,mass2]
 
 #here you define information needed as input to the rapidpe scripts which computes the likelihood
```

### Comparing `gwcelery-2.0.4/gwcelery/templates/vector_table.jinja2` & `gwcelery-2.0.5/gwcelery/templates/vector_table.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/conftest.py` & `gwcelery-2.0.5/gwcelery/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/G000012_S0040_preferred.json` & `gwcelery-2.0.5/gwcelery/tests/data/G000012_S0040_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/G298048-1-Initial.xml` & `gwcelery-2.0.5/gwcelery/tests/data/G298048-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/G298048_log.json` & `gwcelery-2.0.5/gwcelery/tests/data/G298048_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json` & `gwcelery-2.0.5/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/MS220722v.xml` & `gwcelery-2.0.5/gwcelery/tests/data/MS220722v.xml`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930504792072775%*

 * *Differences: {"'labels'": "{insert: [(2, 'LOW_SIGNIF_LOCKED')], delete: [2]}",*

 * * "'preferred_event_data'": "{'superevent_neighbours': {'MS220722v': {'labels': {insert: [(2, "*

 * *                           "'LOW_SIGNIF_LOCKED')], delete: [2]}}}}"}*

```diff
@@ -22,15 +22,15 @@
         "M252703",
         "M252702"
     ],
     "gw_id": null,
     "labels": [
         "EM_READY",
         "ADVNO",
-        "EM_Selected",
+        "LOW_SIGNIF_LOCKED",
         "SKYMAP_READY",
         "EMBRIGHT_READY",
         "PASTRO_READY",
         "GCN_PRELIM_SENT"
     ],
     "links": {
         "emobservations": "https://gracedb-test.ligo.org/api/superevents/MS220722v/emobservations/",
@@ -235,15 +235,15 @@
                     "M252704",
                     "M252703",
                     "M252702"
                 ],
                 "labels": [
                     "EM_READY",
                     "ADVNO",
-                    "EM_Selected",
+                    "LOW_SIGNIF_LOCKED",
                     "SKYMAP_READY",
                     "EMBRIGHT_READY",
                     "PASTRO_READY",
                     "GCN_PRELIM_SENT"
                 ],
                 "preferred_event": "M252714",
                 "preferred_event_data": {
```

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits` & `gwcelery-2.0.5/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/T0212_S0039_preferred.json` & `gwcelery-2.0.5/gwcelery/tests/data/T0212_S0039_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json` & `gwcelery-2.0.5/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/T0219_S0041_nopreferred.json` & `gwcelery-2.0.5/gwcelery/tests/data/T0219_S0041_nopreferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/agile_grb_gcn.xml` & `gwcelery-2.0.5/gwcelery/tests/data/agile_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/coinc.xml` & `gwcelery-2.0.5/gwcelery/tests/data/coinc.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/externaltrigger_original_data.xml` & `gwcelery-2.0.5/gwcelery/tests/data/externaltrigger_original_data.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/fermi_grb_gcn.xml` & `gwcelery-2.0.5/gwcelery/tests/data/fermi_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/fermi_initial_grb_gcn.xml` & `gwcelery-2.0.5/gwcelery/tests/data/fermi_initial_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/fermi_noise_gcn.xml` & `gwcelery-2.0.5/gwcelery/tests/data/fermi_noise_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/fermi_noise_gcn_2.xml` & `gwcelery-2.0.5/gwcelery/tests/data/fermi_noise_gcn_2.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml` & `gwcelery-2.0.5/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml` & `gwcelery-2.0.5/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/fits_header_result.html` & `gwcelery-2.0.5/gwcelery/tests/data/fits_header_result.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/gracedb_externaltrigger_log.json` & `gwcelery-2.0.5/gwcelery/tests/data/gracedb_externaltrigger_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_detchar.json` & `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_detchar.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_exttrig_creation.json` & `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_exttrig_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json` & `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_psd.json` & `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_psd.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_snews_creation.json` & `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_snews_creation.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975490196078431%*

 * *Differences: {"'object'": "{'search': 'Supernova'}"}*

```diff
@@ -40,13 +40,13 @@
             "neighbors": "https://gracedb-playground.ligo.org/api/events/E1234/neighbors/",
             "self": "https://gracedb-playground.ligo.org/api/events/E1234",
             "tags": "https://gracedb-playground.ligo.org/api/events/E1234/tag/"
         },
         "nevents": null,
         "offline": false,
         "pipeline": "SNEWS",
-        "search": "SNEWS",
+        "search": "Supernova",
         "submitter": "emfollow",
         "superevent": null
     },
     "uid": "E1235"
 }
```

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_snews_test_creation.json` & `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_snews_test_creation.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975490196078431%*

 * *Differences: {"'object'": "{'search': 'Supernova'}"}*

```diff
@@ -40,13 +40,13 @@
             "neighbors": "https://gracedb-playground.ligo.org/api/events/E1234/neighbors/",
             "self": "https://gracedb-playground.ligo.org/api/events/E1234",
             "tags": "https://gracedb-playground.ligo.org/api/events/E1234/tag/"
         },
         "nevents": null,
         "offline": false,
         "pipeline": "SNEWS",
-        "search": "SNEWS",
+        "search": "Supernova",
         "submitter": "emfollow",
         "superevent": null
     },
     "uid": "E1236"
 }
```

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_subgrb_creation.json` & `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_subgrb_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_superevent_creation.json` & `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_superevent_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/igwn_alert_voevent.json` & `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_voevent.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/integral_grb_gcn.xml` & `gwcelery-2.0.5/gwcelery/tests/data/integral_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.0.5/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/llhoft/omegascan/scanme.gwf` & `gwcelery-2.0.5/gwcelery/tests/data/llhoft/omegascan/scanme.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.0.5/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/lvalert_event_creation.json` & `gwcelery-2.0.5/gwcelery/tests/data/lvalert_event_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/lvalert_xmpp.xml` & `gwcelery-2.0.5/gwcelery/tests/data/lvalert_xmpp.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/mock_superevent_object.json` & `gwcelery-2.0.5/gwcelery/tests/data/mock_superevent_object.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite` & `gwcelery-2.0.5/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/psd.xml.gz` & `gwcelery-2.0.5/gwcelery/tests/data/psd.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/sample_events.json` & `gwcelery-2.0.5/gwcelery/tests/data/sample_events.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/samples.hdf5` & `gwcelery-2.0.5/gwcelery/tests/data/samples.hdf5`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/scaler_set_all.pickle` & `gwcelery-2.0.5/gwcelery/tests/data/scaler_set_all.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/snews_gcn.xml` & `gwcelery-2.0.5/gwcelery/tests/data/snews_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/snews_gcn_test.xml` & `gwcelery-2.0.5/gwcelery/tests/data/snews_gcn_test.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/superevents.json` & `gwcelery-2.0.5/gwcelery/tests/data/superevents.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/swift_grb_gcn.xml` & `gwcelery-2.0.5/gwcelery/tests/data/swift_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/data/test_classifier.pickle` & `gwcelery-2.0.5/gwcelery/tests/data/test_classifier.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/process.py` & `gwcelery-2.0.5/gwcelery/tests/process.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_sentry.py` & `gwcelery-2.0.5/gwcelery/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_bayestar.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_circulars.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_condor.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_detchar.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_detchar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_em_bright.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_external_skymaps.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_external_skymaps.py`

 * *Files 8% similar despite different names*

```diff
@@ -125,35 +125,53 @@
         mock_read_sky_map.assert_called()
         mock_skymap_combine_moc_flat.assert_called_once()
         mock_write_sky_map.assert_called_once()
     else:
         mock_skymap_combine_flat_flat.assert_called()
 
 
-def test_create_combined_skymap_moc_flat():
+@pytest.mark.parametrize('missing_header_values,instrument',
+                         [[False, 'Fermi'],
+                          [True, 'Fermi'],
+                          [False, None],
+                          [True, None]])
+def test_create_combined_skymap_moc_flat(missing_header_values, instrument):
     """Test using our internal MOC-flat sky map combination gives back the
     input using a uniform sky map, ensuring the test is giving a sane result
     and is at least running to completion.
     """
     # Run function under test
     gw_sky = get_gw_moc_skymap()
+    if missing_header_values:
+        del gw_sky['DISTMU']
+        del gw_sky['DISTSIGMA']
+        gw_sky.meta.pop('instruments')
+        gw_sky.meta.pop('HISTORY')
     ext_sky = np.full(12, 1 / 12)
-    ext_header = {'instruments': set({'Fermi'}), 'nest': True}
+    if instrument:
+        ext_header = {'instruments': set({instrument}), 'nest': True}
+    else:
+        ext_header = {'nest': True}
     combined_sky = external_skymaps.combine_skymaps_moc_flat(gw_sky, ext_sky,
                                                              ext_header)
     assert all(combined_sky['PROBDENSITY'] == gw_sky['PROBDENSITY'])
-    assert 'Fermi' in combined_sky.meta['instruments']
+    if missing_header_values:
+        assert 'instruments' not in combined_sky.meta
+    else:
+        assert ('Fermi' in combined_sky.meta['instruments'] if instrument else
+                'external instrument' in combined_sky.meta['instruments'])
 
 
 @pytest.mark.parametrize('graceid',
                          ['S12345', 'E12345'])
 @patch('gwcelery.tasks.gracedb.get_log', side_effect=mock_get_log)
 def test_get_skymap_filename(mock_get_logs, graceid):
     """Test getting the LVC skymap fits filename"""
-    filename = external_skymaps.get_skymap_filename(graceid)
+    filename = external_skymaps.get_skymap_filename(graceid,
+                                                    is_gw='S' in graceid)
     if 'S' in graceid:
         assert filename == 'bayestar.multiorder.fits,0'
     elif 'E' in graceid:
         assert filename == 'fermi_skymap.fits.gz,0'
 
 
 @patch('gwcelery.tasks.gracedb.get_event', mock_get_event)
@@ -268,13 +286,28 @@
              'links': {
                  'self': 'https://gracedb.ligo.org/api/events/E356793'}}
     external_skymaps.create_upload_external_skymap(event, '111',
                                                    '2020-01-09T01:47:09')
     mock_upload.assert_not_called()
 
 
+@pytest.mark.parametrize(
+    'em_type,graceid,labels,expected_result',
+    [[None, 'E1', [], True],
+     ['E1', 'E1', [], True],
+     ['E1', 'E2', [], True],
+     ['E1', 'E1', ['RAVEN_ALERT'], True],
+     ['E1', 'E2', ['RAVEN_ALERT'], False]]
+)
 @patch('gwcelery.tasks.gracedb.upload.run')
-def test_plot_overlap_integral(mock_upload):
+def test_plot_overlap_integral(mock_upload,
+                               em_type, graceid, labels, expected_result):
 
     coinc_far_dict = {'skymap_overlap': 1e2}
-    external_skymaps.plot_overlap_integral(coinc_far_dict, 'S1234', 'E1234')
-    mock_upload.assert_called_once()
+    superevent = {'superevent_id': 'S1', 'em_type': em_type, 'labels': labels}
+    ext_event = {'graceid': graceid}
+    external_skymaps.plot_overlap_integral(coinc_far_dict, superevent,
+                                           ext_event)
+    if expected_result:
+        mock_upload.assert_called_once()
+    else:
+        mock_upload.assert_not_called()
```

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_external_triggers.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_external_triggers.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from ..tasks import detchar
 from ..util import read_json
 
 
 @pytest.mark.parametrize('pipeline, path',
                          [['Fermi', 'fermi_grb_gcn.xml'],
                           ['INTEGRAL', 'integral_grb_gcn.xml'],
+                          ['INTEGRAL_MDC', 'integral_mdc_gcn.xml'],
                           ['AGILE', 'agile_grb_gcn.xml']])
 @patch('gwcelery.tasks.external_skymaps.create_upload_external_skymap.run')
 @patch('gwcelery.tasks.external_skymaps.get_upload_external_skymap.run')
 @patch('gwcelery.tasks.detchar.dqr_json', return_value='dqrjson')
 @patch('gwcelery.tasks.gracedb.upload.run')
 @patch('gwcelery.tasks.gracedb.create_event.run', return_value={
     'graceid': 'E1', 'gpstime': 1, 'instruments': '', 'pipeline': 'Fermi',
@@ -35,19 +36,20 @@
         root = etree.parse(fname)
         root.find("./What/Param[@name='TrigID']").attrib['value'] = \
             '123456'.encode()
         text = etree.tostring(root, xml_declaration=True, encoding="UTF-8")
     else:
         text = resources.read_binary(data, path)
     external_triggers.handle_grb_gcn(payload=text)
-    mock_create_event.assert_called_once_with(filecontents=text,
-                                              search='GRB',
-                                              pipeline=pipeline,
-                                              group='External',
-                                              labels=None)
+    mock_create_event.assert_called_once_with(
+        filecontents=text,
+        search='GRB',
+        pipeline='INTEGRAL' if pipeline == 'INTEGRAL_MDC' else pipeline,
+        group='External',
+        labels=None)
     calls = [
         call(
             '"dqrjson"', 'gwcelerydetcharcheckvectors-E1.json', 'E1',
             'DQR-compatible json generated from check_vectors results'),
         call(
             None, None, 'E1',
             ('Detector state for active instruments is unknown.\n{}'
@@ -61,17 +63,19 @@
                       'H1:HOFT_OK', 'H1:OBSERVATION_INTENT',
                       'L1:HOFT_OK', 'L1:OBSERVATION_INTENT',
                       'V1:HOFT_OK', 'V1:OBSERVATION_INTENT',
                       'V1:GOOD_DATA_QUALITY_CAT1'])),
             ['data_quality'])
     ]
     mock_upload.assert_has_calls(calls, any_order=True)
-    gcn_type_dict = {'Fermi': 115, 'INTEGRAL': 53, 'AGILE': 105}
+    gcn_type_dict = {'Fermi': 115, 'INTEGRAL': 53, 'INTEGRAL_MDC': 53,
+                     'AGILE': 105}
     time_dict = {'Fermi': '2018-05-24T18:35:45',
                  'INTEGRAL': '2017-02-03T19:00:05',
+                 'INTEGRAL_MDC': '2023-04-04T06:31:24',
                  'AGILE': '2019-03-19T19:40:49'}
     mock_create_upload_external_skymap.assert_called_once_with(
         {'graceid': 'E1',
          'gpstime': 1,
          'instruments': '',
          'pipeline': 'Fermi',
          'search': 'GRB',
@@ -230,47 +234,49 @@
         mock_replace_event.assert_called_once_with('E1', text)
         mock_create_label.assert_called_once_with('NOT_GRB', 'E1')
 
 
 @patch('gwcelery.tasks.gracedb.get_group', return_value='CBC')
 @patch('gwcelery.tasks.gracedb.create_label.run')
 @patch('gwcelery.tasks.gracedb.get_labels',
-       return_value=['SKYMAP_READY'])
+       return_value=['SKYMAP_READY', 'EM_READY'])
 def test_handle_create_skymap_label_from_ext_event(mock_get_labels,
                                                    mock_create_label,
                                                    mock_get_group):
     alert = {"uid": "E1212",
              "alert_type": "label_added",
              "data": {"name": "EM_COINC"},
              "object": {
                  "group": "External",
                  "labels": ["EM_COINC", "EXT_SKYMAP_READY"],
                  "superevent": "S1234"
                        }
              }
     external_triggers.handle_grb_igwn_alert(alert)
-    mock_create_label.assert_called_once_with('SKYMAP_READY', 'E1212')
+    calls = [call('SKYMAP_READY', 'E1212'), call('EM_READY', 'E1212')]
+    mock_create_label.assert_has_calls(calls)
 
 
 @patch('gwcelery.tasks.gracedb.get_group', return_value='CBC')
 @patch('gwcelery.tasks.gracedb.create_label.run')
 def test_handle_create_skymap_label_from_superevent(mock_create_label,
                                                     mock_get_group):
     alert = {"uid": "S1234",
              "alert_type": "label_added",
              "data": {"name": "SKYMAP_READY"},
              "object": {
                  "group": "CBC",
-                 "labels": ["SKYMAP_READY"],
+                 "labels": ["SKYMAP_READY", "EM_READY"],
                  "superevent_id": "S1234",
                  "em_events": ['E1212']
                        }
              }
     external_triggers.handle_grb_igwn_alert(alert)
-    mock_create_label.assert_called_once_with('SKYMAP_READY', 'E1212')
+    calls = [call('SKYMAP_READY', 'E1212'), call('EM_READY', 'E1212')]
+    mock_create_label.assert_has_calls(calls)
 
 
 @pytest.mark.parametrize('pipeline',
                          ['Fermi', 'Swift'])
 @patch('gwcelery.tasks.raven.raven_pipeline.run')
 @patch('gwcelery.tasks.external_skymaps.create_combined_skymap.run')
 @patch('gwcelery.tasks.gracedb.get_superevent.run',
@@ -287,34 +293,34 @@
     """This test makes sure that once sky maps are available for a coincidence
     that the RAVEN pipeline is rerun to calculate the joint FAR with sky map
     information and check publishing conditions, as well as creating a
     combined sky map.
     """
     alert = {"uid": "E1212",
              "alert_type": "label_added",
-             "data": {"name": "SKYMAP_READY"},
+             "data": {"name": "EM_READY"},
              "object": {
                  "graceid": "E1212",
                  "group": "External",
-                 "labels": ["EM_COINC", "EXT_SKYMAP_READY", "SKYMAP_READY"],
+                 "labels": ["EM_COINC", "EXT_SKYMAP_READY", "EM_READY"],
                  "superevent": "S1234",
                  "pipeline": pipeline,
                  "search": "GRB"
                        }
              }
     external_triggers.handle_grb_igwn_alert(alert)
     mock_raven_pipeline.assert_called_once_with([{'superevent_id': 'S1234',
                                                   'preferred_event': 'G1234',
                                                   'preferred_event_data':
                                                       {'group': 'CBC'}}],
                                                 'E1212', alert['object'],
                                                 -5, 1, 'CBC')
     if pipeline != 'Swift':
         mock_create_combined_skymap.assert_called_once_with(
-            'S1234', 'E1212')
+            'S1234', 'E1212', preferred_event='G1234')
     else:
         mock_create_combined_skymap.assert_not_called()
 
 
 @patch('gwcelery.tasks.raven.trigger_raven_alert')
 @patch('gwcelery.tasks.gracedb.get_superevent',
        return_value={'superevent_id': 'S1234',
@@ -353,36 +359,44 @@
         alert['object'], 'CBC'
     )
 
 
 def _mock_get_event(graceid):
     if graceid == 'E1':
         pipeline = 'Fermi'
+        extra_labels = []
     elif graceid == 'E2':
         pipeline = 'Swift'
+        extra_labels = []
+    elif graceid == 'E3':
+        pipeline = 'Fermi'
+        extra_labels = ['SKYMAP_READY']
     return {'graceid': graceid,
             'pipeline': pipeline,
             'search': 'GRB',
             'superevent': 'S1',
-            'labels': ['EM_COINC', 'SKYMAP_READY', 'EXT_SKYMAP_READY']}
+            'labels': (['EM_COINC', 'EXT_SKYMAP_READY',
+                        'EM_READY'] + extra_labels)
+            }
 
 
 def _mock_get_superevent(graceid):
     return {'superevent_id': 'S1',
+            'preferred_event': 'G1',
             'preferred_event_data':
                 {'group': 'CBC'},
-            'em_events': ['E1', 'E2'],
+            'em_events': ['E1', 'E2', 'E3'],
             'em_type': 'E1',
             'far': 1e-5,
             'labels': ['COMBINEDSKYMAP_READY', 'RAVEN_ALERT',
                        'EM_COINC', 'GCN_PRELIM_SENT']}
 
 
 @pytest.mark.parametrize('graceid',
-                         ['S1', 'E1', 'E2'])
+                         ['S1', 'E1', 'E2', 'E3'])
 @patch('gwcelery.tasks.raven.raven_pipeline.run')
 @patch('gwcelery.tasks.external_skymaps.create_combined_skymap.run')
 @patch('gwcelery.tasks.gracedb.get_event', _mock_get_event)
 @patch('gwcelery.tasks.gracedb.get_superevent.run', _mock_get_superevent)
 def test_handle_rerun_combined_skymap(mock_create_combined_skymap,
                                       mock_raven_pipeline,
                                       graceid):
@@ -393,34 +407,45 @@
     the combined sky map is not required for Swift (E2) since these are
     produced in this case."""
     event = (_mock_get_superevent(graceid) if 'S' in graceid else
              _mock_get_event(graceid))
     alert = {
         "data": {"filename": ("skymap.multiorder.fits" if 'S' in graceid
                               else 'fermi_skymap.fits.gz'),
-                 "file_version": 1},
+                 "file_version": 1,
+                 "comment": ''},
         "uid": graceid,
         "alert_type": "log",
         "object": event
     }
     external_triggers.handle_grb_igwn_alert(alert)
-    if graceid in {'S1', 'E1'}:
+    if graceid == 'S1':
+        mock_create_combined_skymap.assert_has_calls(
+            [call('S1', 'E1', preferred_event=None),
+             call('S1', 'E3', preferred_event=None)]
+        )
+    elif graceid in {'E1', 'E3'}:
         mock_create_combined_skymap.assert_called_once_with(
-            'S1', 'E1')
+            'S1', graceid,
+            preferred_event=('G1' if graceid == 'E1' else None))
     else:
         mock_create_combined_skymap.assert_not_called()
     if 'S' in graceid:
         calls = [
             call(
                 [_mock_get_event('E1')],
                 graceid, event,
                 -1, 5, 'CBC'),
             call(
                 [_mock_get_event('E2')],
                 graceid, event,
+                -1, 5, 'CBC'),
+            call(
+                [_mock_get_event('E3')],
+                graceid, event,
                 -1, 5, 'CBC')
         ]
     else:
         calls = [
             call(
                 [_mock_get_superevent('S1')],
                 graceid, event,
@@ -559,36 +584,44 @@
         call('E1234', alert['object'], group='CBC',
              searches=['SubGRB', 'SubGRBTargeted'],
              pipelines=['Swift'])])
 
 
 @pytest.mark.parametrize('path',
                          ['igwn_alert_snews_test_creation.json',
-                          'igwn_alert_snews_creation.json'])
+                          'igwn_alert_snews_creation.json',
+                          'igwn_alert_superevent_creation.json'])
 @patch('gwcelery.tasks.raven.coincidence_search')
 def test_handle_sntrig_creation(mock_raven_coincidence_search, path):
     """Test dispatch of an IGWN alert message for SNEWS alerts
     This now includes both real and test SNEWS events to ensure both are
-    ingested correctly.
+    ingested correctly, as well as a superevent.
     """
     # Test IGWN alert payload.
     alert = read_json(data, path)
 
+    if 'superevent' in path:
+        alert['object']['preferred_event_data']['group'] = 'Burst'
+
     # Run function under test
     external_triggers.handle_snews_igwn_alert(alert)
 
     if 'test' in path:
         graceid = 'E1236'
     else:
         graceid = 'E1235'
 
-    mock_raven_coincidence_search.assert_has_calls([
-            call(graceid, alert['object'],
-                 group='Burst', searches=['Supernova'],
-                 pipelines=['SNEWS'])])
+    if 'superevent' in path:
+        mock_raven_coincidence_search.assert_called_once_with(
+            'S180616h', alert['object'], group='Burst', searches=['Supernova'],
+            pipelines=['SNEWS'])
+    elif 'snews' in path:
+        mock_raven_coincidence_search.assert_called_once_with(
+            graceid, alert['object'], group='Burst', searches=['Supernova'],
+            pipelines=['SNEWS'])
 
 
 @patch('gwcelery.tasks.gracedb.get_superevent',
        return_value={'preferred_event': 'M4634'})
 @patch('gwcelery.tasks.gracedb.get_group', return_value='CBC')
 @patch('gwcelery.tasks.raven.coincidence_search')
 def test_handle_superevent_cbc_creation(mock_raven_coincidence_search,
@@ -656,7 +689,37 @@
                       searches=['MDC'])]
     elif 'exttrig' in path:
         calls = [call('E1234', alert['object'], group='CBC',
                       se_searches=['MDC']),
                  call('E1234', alert['object'], group='Burst',
                       se_searches=['MDC'])]
     mock_raven_coincidence_search.assert_has_calls(calls, any_order=True)
+
+
+@pytest.mark.parametrize('path',
+                         ['igwn_alert_superevent_creation.json',
+                          'igwn_alert_snews_creation.json'])
+@patch('gwcelery.tasks.raven.coincidence_search')
+def test_handle_mdc_sn_creation(mock_raven_coincidence_search,
+                                path):
+    """Test dispatch of an MDC with the supernovae igwn alert listener,
+    both a superevent and external event."""
+    # Test IGWN alert payload.
+    alert = read_json(data, path)
+    if 'superevent' in path:
+        alert['object']['preferred_event_data']['search'] = 'MDC'
+        alert['object']['preferred_event_data']['group'] = 'Burst'
+    elif 'snews' in path:
+        alert['object']['search'] = 'MDC'
+
+    # Run function under test
+    external_triggers.handle_snews_igwn_alert(alert)
+
+    # Check that the correct tasks were dispatched.
+    if 'superevent' in path:
+        mock_raven_coincidence_search.assert_called_once_with(
+            'S180616h', alert['object'], group='Burst', searches=['MDC'],
+            pipelines=['SNEWS'])
+    elif 'snews' in path:
+        mock_raven_coincidence_search.assert_called_once_with(
+            'E1235', alert['object'], group='Burst', se_searches=['MDC'],
+            pipelines=['SNEWS'])
```

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_first2years.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_first2years_external.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_first2years_external.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from unittest.mock import call, Mock
+from unittest.mock import call, Mock, patch
 
 from . import data
 from .. import app
 from ..tasks import first2years_external
 from ..util import read_json
 
 
@@ -84,7 +84,25 @@
                           labels=None))
     if expected_result:
         mock_create_event.assert_has_calls(calls)
         mock_create_upload_external_skymap.assert_called()
     else:
         mock_create_event.assert_not_called()
         mock_create_upload_external_skymap.assert_not_called()
+
+
+@patch('gwcelery.tasks.detchar.check_vectors.run')
+@patch('gwcelery.tasks.gracedb.create_event.run', return_value={
+    'graceid': 'M1', 'gpstime': 1, 'instruments': '', 'pipeline': 'SNEWS',
+    'search': 'MDC',
+    'links': {'self': 'https://gracedb.ligo.org/events/E356793/'}})
+@patch('gwcelery.tasks.gracedb.get_events', return_value=[])
+def test_upload_snews_event(mock_get_events,
+                            mock_create_event,
+                            mock_check_vectors):
+    event = first2years_external.upload_snews_event()
+    mock_create_event.assert_called_once_with(
+        filecontents=event,
+        search='MDC',
+        pipeline='SNEWS',
+        group='External')
+    mock_check_vectors.assert_called_once()
```

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_gcn.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_gcn_validate.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_gcn_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_gracedb.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_igwn_alert.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_inference.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     monkeypatch.setitem(app.conf, 'gracedb_host', host)
 
     def _subprocess_run(cmd, **kwargs):
         if host != 'gracedb.ligo.org':
             assert 'o3replay' in cmd
 
         assert cmd[2] == os.path.join(
-            app.conf['pe_results_path'], sid, 'bilby')
+            app.conf['pe_results_path'], sid, 'bilby', mode)
 
         assert cmd[4] == rundir
 
         path_to_json = cmd[6]
         assert os.path.exists(path_to_json)
         with open(path_to_json, 'r') as f:
             assert event == json.load(f)
@@ -215,32 +215,34 @@
         assert os.path.exists(path_to_settings)
         ans = {
             'summarypages_arguments': {'gracedb': event['graceid'],
                                        'no_ligo_skymap': True},
             'queue': 'Online_PE',
             'accounting_user': 'soichiro.morisaki'
         }
+        if host != 'gracedb.ligo.org':
+            ans['queue'] = 'Online_PE_MDC'
         if mode == 'quick_bns':
             ans.update(
                 {'sampler_kwargs': {'naccept': 10, 'nlive': 500,
                                     'npool': 24, 'sample': 'acceptance-walk'},
                  'n_parallel': 2,
                  'request_cpus': 24,
-                 'spline_calibration_nodes': 4,
+                 'spline_calibration_nodes': 10,
                  'request_memory_generation': 8.0}
             )
         elif mode == 'fast_test':
             if mc < 3.9:
                 ans['request_memory_generation'] = 8.0
             ans.update(
-                {'sampler_kwargs': {'naccept': 20, 'nlive': 1000,
+                {'sampler_kwargs': {'naccept': 60, 'nlive': 500,
                                     'npool': 24, 'sample': 'acceptance-walk'},
                  'n_parallel': 2,
                  'request_cpus': 24,
-                 'spline_calibration_nodes': 4}
+                 'spline_calibration_nodes': 10}
             )
         with open(path_to_settings, 'r') as f:
             assert json.load(f) == ans
 
         with open(os.path.join(rundir, 'bilby_config.ini'), 'w') as f:
             f.write(ini)
         dir = os.path.join(rundir, 'submit')
@@ -315,15 +317,14 @@
             inference._setup_dag_for_lalinference(
                 b'coinc', rundir, event, 'S1234', {})
         elif pipeline == 'bilby':
             inference._setup_dag_for_bilby(
                 (b'psd'), rundir, event, 'S1234', 'production')
         elif pipeline == 'rapidpe':
             inference._setup_dag_for_rapidpe(rundir, 'S1234', {})
-    assert not os.path.exists(rundir)
     if pipeline == 'bilby':
         assert upload.call_count == 1
     else:
         # For pipelines except for bilby, an ini file is uploaded before dag
         # generation, and hence the call count is 2.
         assert upload.call_count == 2
 
@@ -449,37 +450,66 @@
                 assert os.path.exists(cmd[1])
 
             monkeypatch.setattr(
                 'subprocess.run', Mock(side_effect=_subprocess_run))
 
             kwargs['bilby_mode'] = 'production'
             paths = [os.path.join(sampledir,
-                                  'Bilby.production.posterior_samples.hdf5'),
-                     os.path.join(resultdir, 'bilby_extrinsic_corner.png'),
-                     os.path.join(resultdir, 'bilby_intrinsic_corner.png')]
+                                  'Bilby.production.posterior_samples.hdf5')]
+
+            path_to_bilby_config = os.path.join(rundir, "bilby_complete.ini")
+            with open(path_to_bilby_config, "w") as f:
+                f.write(
+                    "spline-calibration-envelope-dict="
+                    "{'H1': 'H1_cal.txt', 'L1': 'L1_cal.txt'}\n"
+                    "psd-dict={'H1': 'H1_psd.txt', 'L1': 'L1_psd.txt'}\n"
+                    "waveform-approximant=IMRPhenomPv2\n"
+                    "minimum-frequency=20\n"
+                    "reference-frequency=100\n"
+                    "webdir=webdir"
+                )
+
+            def mock_check_output(args, **kwargs):
+                assert args == [
+                    "summarypages", "--webdir", "webdir/pesummary",
+                    "--samples", os.path.join(sampledir, 'test_result.hdf5'),
+                    "--gw", "--redshift_method", "exact",
+                    "--evolve_spins_fowards",
+                    "--config", path_to_bilby_config,
+                    "--psd", "H1:H1_psd.txt", "L1:L1_psd.txt",
+                    "--calibration", "H1:H1_cal.txt", "L1:L1_cal.txt",
+                    "--approximant", "IMRPhenomPv2",
+                    "--f_low", "20", "--f_ref", "100"
+                ]
+
+            monkeypatch.setattr(
+                'gwcelery.tasks.condor.check_output.run', mock_check_output)
+
         else:
             paths = []
         for path in paths:
             with open(path, 'wb') as f:
                 f.write(b'result')
 
         inference.dag_finished(
             rundir, sid, pipeline, bilby_mode='production')
 
         if pipeline == 'rapidpe':
             upload.assert_called_once()
+        elif pipeline == 'bilby':
+            # +1 corresponds to pesummary link
+            assert upload.call_count == len(paths) + 1
         else:
             assert upload.call_count == len(paths)
 
         if pipeline == 'bilby':
             create_label.assert_called_once()
         else:
             create_label.assert_not_called()
 
-        assert not os.path.exists(rundir)
     else:
         with pytest.raises(NotImplementedError):
             inference.dag_finished(rundir, sid, pipeline)
 
 
 def test_start_pe(monkeypatch, tmp_path):
     path_to_sub = 'pe.dag.condor.sub'
```

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_orchestrator.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_orchestrator.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,36 +11,44 @@
 from .test_tasks_skymaps import toy_3d_fits_filecontents  # noqa: F401
 from . import data
 
 
 @pytest.mark.parametrize(  # noqa: F811
     'alert_type,alert_label,group,pipeline,offline,far,instruments,'
     'superevent_id,superevent_labels',
-    [['label_added', 'EM_Selected', 'CBC', 'gstlal', False, 1.e-9,
-        ['H1'], 'S1234', ['EM_Selected']],
-     ['label_added', 'EM_SelectedConfident', 'CBC', 'gstlal', False, 1.e-9,
-         ['H1', 'L1'], 'S1234', ['EM_Selected']],
-     ['label_added', 'EM_SelectedConfident', 'CBC', 'gstlal', False, 1.e-9,
-         ['H1', 'L1', 'V1'], 'S1234', ['EM_Selected']],
-     ['label_added', 'EM_SelectedConfident', 'CBC', 'gstlal', False, 1.e-9,
+    [['label_added', 'LOW_SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-9,
+        ['H1'], 'S1234', ['LOW_SIGNIF_LOCKED']],
+     ['label_added', 'ADVREQ', 'CBC', 'gstlal', False, 1.e-9,
+        ['H1'], 'S1234', ['ADVREQ']],
+     ['label_added', 'SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-9,
+         ['H1', 'L1'], 'S1234', ['LOW_SIGNIF_LOCKED']],
+     ['label_added', 'SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-9,
+         ['H1', 'L1', 'V1'], 'S1234', ['LOW_SIGNIF_LOCKED']],
+     ['label_added', 'SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-9,
          ['H1', 'L1', 'V1'], 'S2468',
-         ['EM_Selected', 'COMBINEDSKYMAP_READY',
+         ['LOW_SIGNIF_LOCKED', 'COMBINEDSKYMAP_READY',
           'RAVEN_ALERT', 'EM_COINC']],
-     ['label_added', 'EM_SelectedConfident', 'Burst', 'CWB', False, 1.e-9,
-         ['H1', 'L1', 'V1'], 'S1234', ['EM_Selected']],
-     ['label_added', 'EM_SelectedConfident', 'Burst', 'oLIB', False, 1.e-9,
-         ['H1', 'L1', 'V1'], 'S1234', ['EM_Selected']],
+     ['label_added', 'SIGNIF_LOCKED', 'Burst', 'CWB', False, 1.e-9,
+         ['H1', 'L1', 'V1'], 'S1234', ['LOW_SIGNIF_LOCKED']],
+     ['label_added', 'SIGNIF_LOCKED', 'Burst', 'oLIB', False, 1.e-9,
+         ['H1', 'L1', 'V1'], 'S1234', ['LOW_SIGNIF_LOCKED']],
      ['label_added', 'GCN_PRELIM_SENT', 'CBC', 'gstlal', False, 1.e-9,
-         ['H1', 'L1', 'V1'], 'S1234', ['EM_SelectedConfident']],
-     ['label_added', 'EM_Selected', 'CBC', 'gstlal', False, 1.e-9,
-         ['H1', 'L1', 'V1'], 'S1234', ['EM_SelectedConfident']],
-     ['label_added', 'EM_Selected', 'CBC', 'gstlal', False, 1.e-9,
+         ['H1', 'L1', 'V1'], 'S1234', ['SIGNIF_LOCKED']],
+     ['label_added', 'LOW_SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-9,
+         ['H1', 'L1', 'V1'], 'S1234', ['SIGNIF_LOCKED']],
+     ['label_added', 'LOW_SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-9,
          ['H1', 'L1', 'V1'], 'S1234', []],
+     ['label_added', 'LOW_SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-10,
+         ['H1', 'L1', 'V1'], 'S1234', ['EARLY_WARNING']],
+     ['label_added', 'LOW_SIGNIF_PRELIM_SENT', 'CBC', 'gstlal', False, 1.e-9,
+         ['H1', 'L1', 'V1'], 'S1234', ['EM_SelectedConfident']],
+     ['label_added', 'LOW_SIGNIF_PRELIM_SENT', 'CBC', 'gstlal', False, 1.e-7,
+         ['H1', 'L1', 'V1'], 'S1234', ['EM_Selected']],
      ['new', '', 'CBC', 'gstlal', False, 1.e-9, ['H1', 'L1'], 'S1234',
-         ['EM_Selected']]])
+         ['LOW_SIGNIF_LOCKED']]])
 def test_handle_superevent(monkeypatch, toy_3d_fits_filecontents,  # noqa: F811
                            alert_type, alert_label, group, pipeline,
                            offline, far, instruments, superevent_id,
                            superevent_labels):
     """Test a superevent is dispatched to the correct annotation task based on
     its preferred event's search group.
     """
@@ -128,21 +136,24 @@
         raven_coinc = False
     else:
         raven_coinc = True
 
     create_initial_circular = Mock()
     create_emcoinc_circular = Mock()
     expose = Mock()
+    rrt_channel_creation = Mock()
     annotate_fits = Mock(return_value=None)
-    proceed_if_not_blocked_by = Mock(
-        return_value=(
-            ('skymap', 'skymap-filename'),
-            ('em-bright', 'em-bright-filename'),
-            ('p-astro', 'p-astro-filename'))
-    )
+    # FIXME: remove logic of mocking return value
+    # when live worker testing is enabled
+    proceed_if_not_blocked_by = Mock(return_value=None) if \
+        alert_label == 'LOW_SIGNIF_PRELIM_SENT' and \
+        'EM_SelectedConfident' in superevent_labels else \
+        Mock(return_value=(('skymap', 'skymap-filename'),
+                           ('em-bright', 'em-bright-filename'),
+                           ('p-astro', 'p-astro-filename')))
     gcn_send = Mock()
     alerts_send = Mock()
     query_data = Mock()
     setup_dag = Mock()
     start_pe = Mock()
     create_voevent = Mock(return_value='S1234-1-Preliminary.xml')
     create_label = Mock()
@@ -212,15 +223,17 @@
     monkeypatch.setattr(
         'gwcelery.tasks.superevents.select_pipeline_preferred_event.run',
         select_pipeline_preferred_event_task
     )
     monkeypatch.setattr('gwcelery.tasks.detchar.omegascan.run', omegascan)
     monkeypatch.setattr('gwcelery.tasks.detchar.check_vectors.run',
                         check_vectors)
-
+    monkeypatch.setattr('gwcelery.tasks.orchestrator.channel_creation.'
+                        'rrt_channel_creation', rrt_channel_creation)
+    monkeypatch.setattr(app.conf, 'create_mattermost_channel', True)
     # Run function under test
     orchestrator.handle_superevent(alert)
 
     if alert_label == 'GCN_PRELIM_SENT':
         dqr_request_label = list(
             filter(
                 lambda x: x.args == ('DQR_REQUEST', superevent_id),
@@ -231,15 +244,15 @@
         select_preferred_event_task.assert_called_once()
         update_superevent_task.assert_called_once()
         select_pipeline_preferred_event_task.assert_called_once()
         assert add_pipeline_preferred_event_task.call_count == len(
             select_pipeline_preferred_event_task.return_value
         )
 
-    elif alert_label == 'EM_SelectedConfident':
+    elif alert_label == 'SIGNIF_LOCKED':
         annotate_fits.assert_called_once()
         _event_info = get_event('G1234')  # this gets the preferred event info
         assert superevents.should_publish(_event_info)
         expose.assert_called_once_with(superevent_id)
         create_tag.assert_has_calls(
             [call('S1234-1-Preliminary.xml', 'public', superevent_id),
              call('em-bright-filename', 'public', superevent_id),
@@ -259,15 +272,15 @@
         alerts_send.assert_called_once()
         if raven_coinc:
             create_emcoinc_circular.assert_called_once()
         else:
             create_initial_circular.assert_called_once()
 
     elif alert_label == 'EARLY_WARNING':
-        if 'EM_SelectedConfident' in superevent_labels:
+        if 'SIGNIF_LOCKED' in superevent_labels:
             expose.assert_not_called()
             alerts_send.assert_not_called()
             gcn_send.assert_not_called()
             create_tag.assert_not_called()
             create_initial_circular.assert_not_called()
         else:
             annotate_fits.assert_called_once()
@@ -278,28 +291,44 @@
             create_tag.assert_has_calls(
                 [call('S1234-1-Preliminary.xml', 'public', 'S1234'),
                  call('em-bright-filename', 'public', 'S1234'),
                  call('p-astro-filename', 'public', 'S1234'),
                  call('skymap-filename', 'public', 'S1234')],
                 any_order=True
             )
-    elif alert_label == 'EM_Selected':
-        if 'EM_SelectedConfident' in superevent_labels:
+    elif alert_label == 'LOW_SIGNIF_LOCKED':
+        if ('SIGNIF_LOCKED' in superevent_labels) or \
+                ('EARLY_WARNING' in superevent_labels):
             expose.assert_not_called()
             alerts_send.assert_not_called()
             gcn_send.assert_not_called()
             create_tag.assert_not_called()
             create_initial_circular.assert_not_called()
         else:
             annotate_fits.assert_called_once()
             # no superevent clean up needed
             update_superevent_task.assert_not_called()
             # no circular creation for less-significant alerts
             create_initial_circular.assert_not_called()
             create_emcoinc_circular.assert_not_called()
+    elif alert_label == 'ADVREQ':
+        rrt_channel_creation.assert_called_once_with(
+            superevent_id,
+            app.conf['gracedb_host'])
+    elif alert_label == 'LOW_SIGNIF_PRELIM_SENT':
+        if 'EM_SelectedConfident' in superevent_labels:
+            expose.assert_not_called()
+            alerts_send.assert_not_called()
+            gcn_send.assert_not_called()
+            create_tag.assert_not_called()
+            create_initial_circular.assert_not_called()
+        else:
+            # check alert type is less-significant
+            _files, _superevent, _alert_type = alerts_send.call_args.args
+            assert _alert_type == 'less-significant'
 
     if alert_type == 'new' and group == 'CBC':
         query_data.assert_called_once()
         threshold = (
             app.conf['preliminary_alert_far_threshold']['cbc'] /
             app.conf['preliminary_alert_trials_factor']['cbc']
         )
@@ -588,15 +617,15 @@
 @patch('gwcelery.tasks.p_astro.compute_p_astro.run')
 @patch('gwcelery.tasks.bayestar.localize.run')
 @patch('gwcelery.tasks.em_bright.source_properties.run')
 def test_handle_cbc_event_new_event(mock_source_properties,
                                     mock_localize, mock_p_astro,
                                     alert_search, alert_pipeline):
     alert = read_json(data, 'lvalert_event_creation.json')
-    pipelines_stock_p_astro = {('spiir', 'allsky'), ('spiir', 'earlywarning'),
+    pipelines_stock_p_astro = {('spiir', 'earlywarning'),
                                ('pycbc', 'earlywarning'), ('gstlal', 'mdc')}
     alert['object']['search'] = alert_search
     alert['object']['pipeline'] = alert_pipeline
     orchestrator.handle_cbc_event(alert)
     mock_source_properties.assert_called_once()
     if (alert_pipeline, alert_search) in pipelines_stock_p_astro:
         mock_p_astro.assert_called_once()
@@ -714,17 +743,17 @@
     else:
         mock_upload.assert_called_once()
 
 
 @pytest.mark.parametrize(
     "superevent_labels,block_by_labels",
     [
-        [["EM_Selected"], set()],
-        [["EM_Selected"], {"ADVOK", "ADVNO"}],
-        [["EM_SelectedConfident", "ADVOK"], {"ADVOK", "ADVNO"}]
+        [["LOW_SIGNIF_LOCKED"], set()],
+        [["LOW_SIGNIF_LOCKED"], {"ADVOK", "ADVNO"}],
+        [["SIGNIF_LOCKED", "ADVOK"], {"ADVOK", "ADVNO"}]
     ]
 )
 def test_blocking_labels(superevent_labels, block_by_labels):
     with patch('gwcelery.tasks.gracedb.get_labels',
                return_value=superevent_labels):
         r = orchestrator._proceed_if_not_blocked_by(
             ('bayestar', 'em-bright', 'p-astro'),
```

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_p_astro.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_raven.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_raven.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,16 @@
         'S1234', 'E4321', tl, th,
         incl_sky=True, grb_search='GRB',
         se_dict=se, ext_dict=ext,
         se_fitsfile='fermi_skymap.fits.gz',
         ext_fitsfile='fermi_skymap.fits.gz',
         se_moc=True, ext_moc=False,
         use_radec=False,
-        gracedb=gracedb.client, far_grb=None)
+        gracedb=gracedb.client, far_grb=None,
+        use_preferred_event_skymap=False)
 
 
 @pytest.mark.parametrize('group', ['CBC', 'Burst'])  # noqa: F811
 @patch('gwcelery.tasks.external_skymaps.get_skymap_filename',
        return_value='swift_skymap.fits.gz')
 @patch('ligo.raven.search.calc_signif_gracedb')
 def test_calculate_spacetime_coincidence_far_swift(
@@ -146,15 +147,46 @@
         'S1234', 'E4321', tl, th,
         incl_sky=True, grb_search='GRB',
         se_dict=se, ext_dict=ext,
         se_fitsfile='swift_skymap.fits.gz',
         ext_fitsfile='swift_skymap.fits.gz',
         se_moc=True, ext_moc=False,
         use_radec=True,
-        gracedb=gracedb.client, far_grb=None)
+        gracedb=gracedb.client, far_grb=None,
+        use_preferred_event_skymap=False)
+
+
+@pytest.mark.parametrize('group', ['CBC', 'Burst'])  # noqa: F811
+@patch('gwcelery.tasks.external_skymaps.get_skymap_filename',
+       return_value='fermi_skymap.fits.gz')
+@patch('ligo.raven.search.calc_signif_gracedb')
+def test_calculate_spacetime_coincidence_far_preferred(
+        mock_calc_signif, mock_get_skymap_filename, group):
+    se = {'superevent_id': 'S1234',
+          'preferred_event': 'G1'}
+    ext = {'graceid': 'E4321',
+           'pipeline': 'Fermi',
+           'search': 'GRB',
+           'labels': ['EXT_SKYMAP_READY', 'EM_READY'],
+           'far': None}
+    if group == 'CBC':
+        tl, th = -5, 1
+    else:
+        tl, th = -600, 60
+    raven.calculate_coincidence_far(se, ext, tl, th)
+    mock_calc_signif.assert_called_once_with(
+        'S1234', 'E4321', tl, th,
+        incl_sky=True, grb_search='GRB',
+        se_dict=se, ext_dict=ext,
+        se_fitsfile='fermi_skymap.fits.gz',
+        ext_fitsfile='fermi_skymap.fits.gz',
+        se_moc=True, ext_moc=False,
+        use_radec=False,
+        gracedb=gracedb.client, far_grb=None,
+        use_preferred_event_skymap=True)
 
 
 def mock_get_labels(superevent_id):
     if superevent_id == 'S14':
         return {'ADVREQ'}
     else:
         return {}
@@ -203,15 +235,17 @@
        {'superevent_id': 'S12', 'far': .001, 'preferred_event': 'G3'}],
         'E5', -1, 5, 'CBC'],
      [[], 'S13', -1, 5, 'CBC'],
      [[{'graceid': 'E4', 'pipeline': 'GRB'}], 'S14', -1, 5, 'CBC'],
      [[{'superevent_id': 'S12', 'far': .001, 'preferred_event': 'G3'}],
         'T4', -10, 10, 'Burst'],
      [[{'superevent_id': 'MS13', 'far': 1, 'preferred_event': 'M3'}],
-        'M15', -1, 5, 'CBC']])
+        'M15', -1, 5, 'CBC'],
+     [[{'superevent_id': 'S13', 'far': 1, 'preferred_event': 'G4'}],
+        'E6', -60, 600, 'Burst']])
 @patch('gwcelery.tasks.raven.trigger_raven_alert.run')
 @patch('gwcelery.tasks.gracedb.get_labels', mock_get_labels)
 @patch('gwcelery.tasks.raven.calculate_coincidence_far.run',
        return_value=mock_coinc_far())
 @patch('gwcelery.tasks.gracedb.update_superevent')
 @patch('gwcelery.tasks.gracedb.create_label.run')
 @patch('gwcelery.tasks.external_skymaps.plot_overlap_integral.run')
@@ -225,15 +259,16 @@
     """This function tests that the RAVEN pipeline runs correctly for scenarios
     where RAVEN finds nothing, a coincidence is found but does not pass
     threshold, when a coincidence is found but does pass threshold, and when
     multiple events are found.
     """
     alert_object = {'preferred_event': 'G1', 'pipeline': 'Fermi',
                     'search': 'Supernova' if graceid == 'T4' else 'GRB',
-                    'labels': []}
+                    'labels': [],
+                    'superevent': None if graceid != 'E6' else 'S14'}
     time_coinc_far = mock_coinc_far()['temporal_coinc_far']
     space_coinc_far = mock_coinc_far()['spatiotemporal_coinc_far']
 
     for result in raven_search_results:
         result['labels'] = []
     if 'S' not in graceid:
         alert_object['group'] = 'External'
@@ -266,44 +301,51 @@
             coinc_calls.append(call(alert_object, result, tl, th))
             label_calls.append(call('EM_COINC', graceid))
             update_calls.append(
                 call(graceid, em_type=result['graceid'],
                      time_coinc_far=time_coinc_far,
                      space_coinc_far=space_coinc_far))
             plot_calls.append(
-                call(mock_coinc_far(), graceid, result['graceid']))
+                call(mock_coinc_far(), alert_object, result))
     else:
         result = raven.preferred_superevent(raven_search_results)[0]
         label_calls.append(call('EM_COINC', result['superevent_id']))
         coinc_calls.append(call(result, alert_object, tl, th))
         label_calls.append(call('EM_COINC', graceid))
         update_calls.append(
             call(raven_search_results[-1]['superevent_id'],
                  em_type=graceid,
                  time_coinc_far=time_coinc_far,
                  space_coinc_far=space_coinc_far))
         plot_calls.append(
-            call(mock_coinc_far(), result['superevent_id'], graceid))
+            call(mock_coinc_far(), result, alert_object))
 
     alert_calls = []
     if 'S' in graceid:
         for result in raven_search_results:
             alert_calls.append(call(mock_coinc_far(),
                                     alert_object, graceid, result, group))
     else:
         alert_calls.append(call(
             mock_coinc_far(),
             result, graceid, alert_object, group))
-    mock_trigger_raven_alert.assert_has_calls(alert_calls, any_order=True)
+    if graceid != 'E6':
+        mock_trigger_raven_alert.assert_has_calls(alert_calls, any_order=True)
 
-    mock_calculate_coincidence_far.assert_has_calls(coinc_calls,
-                                                    any_order=True)
-    mock_update_superevent.assert_has_calls(update_calls, any_order=True)
-    mock_create_label.assert_has_calls(label_calls, any_order=True)
-    mock_plot_overlap_integral.assert_has_calls(plot_calls, any_order=True)
+        mock_calculate_coincidence_far.assert_has_calls(coinc_calls,
+                                                        any_order=True)
+        mock_update_superevent.assert_has_calls(update_calls, any_order=True)
+        mock_create_label.assert_has_calls(label_calls, any_order=True)
+        mock_plot_overlap_integral.assert_has_calls(plot_calls, any_order=True)
+    else:
+        mock_trigger_raven_alert.assert_not_called()
+        mock_calculate_coincidence_far.assert_not_called()
+        mock_update_superevent.assert_not_called()
+        mock_create_label.assert_not_called()
+        mock_plot_overlap_integral.assert_not_called()
 
 
 @pytest.mark.parametrize(
     'raven_search_results, testnum',
     [[[{'superevent_id': 'S10', 'far': 1, 'preferred_event': 'G1'}], 1],
      [[{'superevent_id': 'S11', 'far': 1, 'preferred_event': 'G2'},
        {'superevent_id': 'S12', 'far': .001, 'preferred_event': 'G3'}], 2],
@@ -365,14 +407,16 @@
             pipeline, search, labels = 'Fermi', 'GRB', []
         elif graceid == "E2":
             pipeline, search, labels = 'Fermi', 'GRB', ['NOT_GRB']
         elif graceid == "E3":
             pipeline, search, labels = 'SNEWS', 'Supernova', []
         elif graceid == "E4":
             pipeline, search, labels = 'Fermi', 'GRB', []
+        elif graceid == "E5":
+            pipeline, search, labels = 'Fermi', 'GRB', ['RAVEN_ALERT']
         return {'superevent_id': graceid.replace('E', 'S'),
                 'graceid': graceid,
                 'pipeline': pipeline,
                 'search': search,
                 'labels': labels}
     elif 'S' in graceid:
         return {'em_type': graceid.replace('S', 'E'),
@@ -380,20 +424,25 @@
                 'space_coinc_far': 1e-20,
                 'superevent_id': graceid,
                 'labels': ['COMBINEDSKYMAP_READY'] if graceid == 'S4' else []}
 
 
 @pytest.mark.parametrize(
     'superevent_id,ext_event_id_old,ext_event_id_new,result',
-    # NOT_GRB should not supersede NOT_GRB
+    # NOT_GRB should not supersede real GRB
     [['S1', 'E1', 'E2', False],
      # Real GRB should supersede NOT_GRB
      ['S2', 'E2', 'E1', True],
      # SNEWS event should not be overwritten by GRB
-     ['S3', 'E3', 'E1', False]])
+     ['S3', 'E3', 'E1', False],
+     # RAVEN_ALERT should supersede subthreshold joint candidate
+     ['S4', 'E4', 'E5', True],
+     # Subthreshold joint candidate should not overwrite RAVEN_ALERT
+     ['S5', 'E5', 'E4', False]]
+)
 @patch('gwcelery.tasks.gracedb.update_superevent')
 @patch('gwcelery.tasks.gracedb.get_event', mock_get_event)
 @patch('gwcelery.tasks.gracedb.get_superevent', mock_get_event)
 def test_update_superevent_w_emtype(mock_update_superevent,
                                     superevent_id,
                                     ext_event_id_old, ext_event_id_new,
                                     result):
```

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_skymaps.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tasks_superevents.py` & `gwcelery-2.0.5/gwcelery/tests/test_tasks_superevents.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
        'SKYMAP_READY'],
       ['EMBRIGHT_READY', 'PASTRO_READY',
        'SKYMAP_READY'], 'T1234'],
      [[],
       ['EMBRIGHT_READY', 'PASTRO_READY'],
       ['EMBRIGHT_READY', 'PASTRO_READY',
        'SKYMAP_READY'], 'T0212'],
-     [['EM_Selected', 'ADVREQ', 'DQOK'],
+     [['LOW_SIGNIF_LOCKED', 'ADVREQ', 'DQOK'],
       ['EMBRIGHT_READY', 'PASTRO_READY',
        'SKYMAP_READY'],
       ['EMBRIGHT_READY', 'PASTRO_READY',
        'SKYMAP_READY'], 'T1234']])
 def test_update_preferred_event(superevent_labels, new_event_labels,
                                 preferred_event_labels, new_event_id):
     """Test scenarios pertaining to superevent S0039, with a
@@ -277,16 +277,16 @@
     superevent_response = payload['object']['superevent_neighbours']['S100']
     with patch('gwcelery.tasks.gracedb.get_superevent',
                return_value=superevent_response):
         superevents.handle(payload)
     calls = [call('ADVREQ', 'S100')]
     if {'SKYMAP_READY', 'EMBRIGHT_READY', 'PASTRO_READY'}.issubset(labels):
         calls.extend(
-            [call('EM_READY', 'S100'), call('EM_Selected', 'S100'),
-             call('EM_SelectedConfident', 'S100')]
+            [call('EM_READY', 'S100'), call('LOW_SIGNIF_LOCKED', 'S100'),
+             call('SIGNIF_LOCKED', 'S100')]
         )
     mock_create_label.assert_has_calls(calls, any_order=True)
 
 
 @pytest.mark.parametrize('labels',
                          [['EMBRIGHT_READY', 'PASTRO_READY'],
                           ['SKYMAP_READY', 'EMBRIGHT_READY', 'PASTRO_READY']])
@@ -582,16 +582,16 @@
         p1.assert_called_once()
         p2.assert_called_once_with('S0039', preferred_event='G000003',
                                    t_0=1163905224.4332082)
         p3.assert_called_once()
         expected_calls = [call('ADVREQ', 'S0039')]
         if superevents.is_complete(event_dictionary):
             expected_calls.extend(
-                [call('EM_READY', 'S0039'), call('EM_Selected', 'S0039'),
-                 call('EM_SelectedConfident', 'S0039')])
+                [call('EM_READY', 'S0039'), call('LOW_SIGNIF_LOCKED', 'S0039'),
+                 call('SIGNIF_LOCKED', 'S0039')])
         create_label.assert_has_calls(expected_calls, any_order=True)
 
 
 def test_parse_trigger_cbc_3():
     """New trigger G000001, not present among superevents
     New superevent created.
     """
@@ -654,15 +654,15 @@
         superevents.handle(payload)
         mock_process.assert_not_called()
 
 
 def test_parse_trigger_cbc_5():
     """New trigger G000002 is complete, with no intersecting superevent,
     passes less-significant far, but not significant far. New superevent
-    should be created, and labeled EM_Selected."""
+    should be created, and labeled LOW_SIGNIF_LOCKED."""
     event_dictionary = {'graceid': 'G000002',
                         'gpstime': 1286741861.52678,
                         'group': 'CBC',
                         'pipeline': 'gstlal',
                         'search': 'AllSky',
                         'offline': False,
                         'far': 5.5e-07,
@@ -688,15 +688,15 @@
                return_value='S123456') as p1, \
             patch('gwcelery.tasks.gracedb.get_superevents',
                   return_value=SUPEREVENTS_NEIGHBOURS.values()) as p2, \
             patch('gwcelery.tasks.gracedb.create_label') as p3:
         superevents.handle(payload)
         p1.assert_called_once()
         p2.assert_called_once()
-        p3.assert_called_once_with('EM_Selected', 'S123456')
+        p3.assert_called_once_with('LOW_SIGNIF_LOCKED', 'S123456')
 
 
 def test_parse_trigger_burst_1():
     """New cwb trigger G000005 with gpstime lying partially in
     S0039 window, not more significant than existing preferred
     event, superevent window changed.
     """
@@ -849,15 +849,15 @@
             patch('gwcelery.tasks.gracedb.create_label'):
         superevents.handle(payload)
         p.assert_called_once()
 
 
 def test_parse_trigger_burst_5():
     """New less-significant oLIB trigger, which is complete, no intersecting
-    superevent. New superevent created and labeled EM_Selected.
+    superevent. New superevent created and labeled LOW_SIGNIF_LOCKED.
     """
     event_dictionary = {'graceid': 'G000007',
                         'gpstime': 1.0,
                         'group': 'Burst',
                         'pipeline': 'oLIB',
                         'search': 'AllSky',
                         'offline': False,
@@ -876,20 +876,20 @@
                    alert_type='new',
                    uid='G000007')
     with patch('gwcelery.tasks.gracedb.create_superevent',
                return_value='S123456') as p1, \
             patch('gwcelery.tasks.gracedb.create_label') as p2:
         superevents.handle(payload)
         p1.assert_called_once()
-        p2.assert_called_once_with('EM_Selected', 'S123456')
+        p2.assert_called_once_with('LOW_SIGNIF_LOCKED', 'S123456')
 
 
 def test_parse_trigger_burst_6():
     """New less-significant MLy trigger, which is complete, no intersecting
-    superevent. New superevent created and labeled EM_Selected.
+    superevent. New superevent created and labeled LOW_SIGNIF_LOCKED.
     """
     event_dictionary = {'graceid': 'G123456',
                         'gpstime': 1.0,
                         'group': 'Burst',
                         'pipeline': 'MLy',
                         'search': 'AllSky',
                         'offline': False,
@@ -907,15 +907,15 @@
                    alert_type='new',
                    uid='G123456')
     with patch('gwcelery.tasks.gracedb.create_superevent',
                return_value='S123456') as p1, \
             patch('gwcelery.tasks.gracedb.create_label') as p2:
         superevents.handle(payload)
         p1.assert_called_once()
-        p2.assert_called_once_with('EM_Selected', 'S123456')
+        p2.assert_called_once_with('LOW_SIGNIF_LOCKED', 'S123456')
 
 
 def test_S190421ar_spiir_scenario():    # noqa: N802
     """Test to ensure that a low FAR event with accidental high
     SNR is not promoted to the preferred event status. For example, here,
     the new event G330298 has SNR 10.51, higher than the preferred event
     G330308 which has SNR 10.17. But the preferred event is not changed on
```

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tempfile.py` & `gwcelery-2.0.5/gwcelery/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tools_condor.py` & `gwcelery-2.0.5/gwcelery/tests/test_tools_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tools_condor_submit_helper.py` & `gwcelery-2.0.5/gwcelery/tests/test_tools_condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tools_flask.py` & `gwcelery-2.0.5/gwcelery/tests/test_tools_flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tests/test_tools_nagios.py` & `gwcelery-2.0.5/gwcelery/tests/test_tools_nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tools/condor.py` & `gwcelery-2.0.5/gwcelery/tools/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tools/condor_submit_helper.py` & `gwcelery-2.0.5/gwcelery/tools/condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tools/flask.py` & `gwcelery-2.0.5/gwcelery/tools/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/tools/nagios.py` & `gwcelery-2.0.5/gwcelery/tools/nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/util/cmdline.py` & `gwcelery-2.0.5/gwcelery/util/cmdline.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/util/resources.py` & `gwcelery-2.0.5/gwcelery/util/resources.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/util/tempfile.py` & `gwcelery-2.0.5/gwcelery/util/tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/views.py` & `gwcelery-2.0.5/gwcelery/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 """Flask web application views."""
 import datetime
+from importlib import metadata
 import platform
 import re
 import socket
 import sys
 
-try:
-    from importlib import metadata
-except ImportError:
-    # FIXME Remove when we drop support for Python < 3.8
-    import importlib_metadata as metadata
-
 from astropy.time import Time
 from celery import group
 from flask import flash, jsonify, redirect, render_template, request, url_for
 from flask import make_response
 from requests.exceptions import HTTPError
 
 from . import app as celery_app
@@ -240,42 +235,129 @@
 
 @app.route('/change_preferred_event', methods=['POST'])
 def change_preferred_event():
     """Handle submission of preliminary alert form."""
     keys = ('superevent_id', 'event_id')
     superevent_id, event_id, *_ = tuple(request.form.get(key) for key in keys)
     if superevent_id and event_id:
+        try:
+            event = gracedb.get_event(event_id)
+        except HTTPError as e:
+            flash(f'No change performed. GraceDB query for {event_id} '
+                  f'returned error code {e.response.status_code}.', 'danger')
+            return redirect(url_for('index'))
+
+        try:
+            superevent = gracedb.get_superevent(superevent_id)
+        except HTTPError as e:
+            flash(f'No change performed. GraceDB query for {superevent_id} '
+                  f'returned error code {e.response.status_code}.', 'danger')
+            return redirect(url_for('index'))
         (
             gracedb.upload.s(
                 None, None, superevent_id,
                 'User {} queued a preferred event change to {}.'
                 .format(request.remote_user or '(unknown)', event_id),
                 tags=['em_follow'])
             |
             gracedb.update_superevent.si(
                 superevent_id, preferred_event=event_id)
             |
-            group(
-                gracedb.get_superevent.si(superevent_id),
-
-                gracedb.get_event.si(event_id)
-            )
-            |
-            _construct_igwn_alert_and_send_prelim_alert.s(
+            _construct_igwn_alert_and_send_prelim_alert.si(
+                [superevent, event],
                 superevent_id,
                 initiate_voevent=False
             )
         ).delay()
+
+        # Update pipeline-preferred event if the new preferred event is not
+        # already the pipeline-preferred event for the pipeline that uploaded
+        # it.
+        pipeline_pref_event = \
+            superevent['pipeline_preferred_events'].get(event['pipeline'], {})
+        if pipeline_pref_event.get('graceid', '') != event_id:
+            (
+                gracedb.upload.s(
+                    None, None, superevent_id,
+                    'Manual update of preferred event triggered update of '
+                    f'{event["pipeline"]}-preferred event to {event_id}',
+                    tags=['em_follow'])
+                |
+                gracedb.add_pipeline_preferred_event.si(
+                    superevent_id, event_id)
+            ).delay()
+
         flash('Changed preferred event for {}.'.format(superevent_id),
               'success')
     else:
         flash('No change performed. Please fill in all fields.', 'danger')
     return redirect(url_for('index'))
 
 
+@app.route('/change_pipeline_preferred_event', methods=['POST'])
+def change_pipeline_preferred_event():
+    """Handle submission of preliminary alert form."""
+    keys = ('superevent_id', 'pipeline', 'event_id')
+    superevent_id, pipeline, event_id, *_ = tuple(request.form.get(key) for
+                                                  key in keys)
+    if superevent_id and pipeline and event_id:
+        try:
+            event = gracedb.get_event(event_id)
+        except HTTPError as e:
+            flash(f'No change performed. GraceDB query for {event_id} '
+                  f'returned error code {e.response.status_code}.', 'danger')
+            return redirect(url_for('index'))
+
+        # Check that specified event is from specified pipeline
+        if event['pipeline'].lower() != pipeline.lower():
+            flash(f'No change performed. {event_id} was uploaded by '
+                  f'{event["pipeline"].lower()} and cannot be the '
+                  f'{pipeline.lower()}-preferred event.', 'danger')
+            return redirect(url_for('index'))
+
+        try:
+            superevent = gracedb.get_superevent(superevent_id)
+        except HTTPError as e:
+            flash(f'No change performed. GraceDB query for {superevent_id} '
+                  f'returned error code {e.response.status_code}.', 'danger')
+            return redirect(url_for('index'))
+
+        # Check that this pipeline's preferred event is not the
+        # superevent's preferred event
+        if superevent['preferred_event_data']['pipeline'].lower() == \
+                pipeline.lower():
+            flash(f'No change performed. User specified pipeline, '
+                  f'{pipeline.lower()}, is the same pipeline that '
+                  f'produced {superevent_id}\'s preferred event.', 'danger')
+            return redirect(url_for('index'))
+
+        (
+            gracedb.upload.s(
+                None, None, superevent_id,
+                'User {} queued a {} preferred event change to {}.'
+                .format(request.remote_user or '(unknown)', pipeline,
+                        event_id),
+                tags=['em_follow'])
+            |
+            gracedb.add_pipeline_preferred_event.si(
+                superevent_id, event_id)
+            |
+            _construct_igwn_alert_and_send_prelim_alert.si(
+                [superevent, event],
+                superevent_id,
+                initiate_voevent=False
+            )
+        ).delay()
+        flash(f'Changed {pipeline.lower()} preferred event for '
+              f'{superevent_id}.', 'success')
+    else:
+        flash('No change performed. Please fill in all fields.', 'danger')
+    return redirect(url_for('index'))
+
+
 @app.route('/send_update_gcn', methods=['POST'])
 def send_update_gcn():
     """Handle submission of update alert form."""
     keys = ('superevent_id', 'skymap_filename',
             'em_bright_filename', 'p_astro_filename')
     superevent_id, *filenames = args = tuple(
         request.form.get(key) for key in keys)
@@ -328,22 +410,46 @@
         flash('Downloaded sky map for {}.'.format(ext_id),
               'success')
     else:
         flash('No skymap uploaded. Please fill in all fields.', 'danger')
     return redirect(url_for('index'))
 
 
+@celery_app.task(queue='exttrig',
+                 shared=False)
+def _update_preferred_external_event(ext_event, superevent_id):
+    """Update preferred external event to given external event."""
+    # FIXME: Consider consolidating with raven.update_coinc_far by using
+    # a single function in superevents.py
+    if ext_event['search'] in {'GRB', 'SubGRB', 'SubGRBTargeted'}:
+        coinc_far_dict = gracedb.download(
+            'coincidence_far.json', ext_event['graceid'])
+        time_coinc_far = coinc_far_dict['temporal_coinc_far']
+        space_coinc_far = coinc_far_dict['spatiotemporal_coinc_far']
+    else:
+        time_coinc_far = None
+        space_coinc_far = None
+    gracedb.update_superevent(superevent_id, em_type=ext_event['graceid'],
+                              time_coinc_far=time_coinc_far,
+                              space_coinc_far=space_coinc_far)
+
+
 @app.route('/apply_raven_labels', methods=['POST'])
 def apply_raven_labels():
-    """Applying RAVEN alert label for the missed coincident alerts."""
+    """Applying RAVEN alert label and update the preferred external event
+    to the given coincidence."""
     keys = ('superevent_id', 'ext_id', 'event_id')
     superevent_id, ext_id, event_id, *_ = tuple(request.form.get(key)
                                                 for key in keys)
     if superevent_id and ext_id and event_id:
         (
+                gracedb.get_event.si(ext_id)
+                |
+                _update_preferred_external_event.s(superevent_id)
+                |
                 gracedb.create_label.si('RAVEN_ALERT', superevent_id)
                 |
                 gracedb.create_label.si('RAVEN_ALERT', ext_id)
                 |
                 gracedb.create_label.si('RAVEN_ALERT', event_id)
         ).delay()
         flash('Applied RAVEN alert label for {}.'.format(superevent_id),
@@ -359,17 +465,18 @@
     first2years.upload_event.delay()
     flash('Queued a mock event.', 'success')
     return redirect(url_for('index'))
 
 
 @gracedb.task(shared=False)
 def _create_upload_external_event(gpstime):
-    new_time = first2years_external._offset_time(gpstime)
+    new_time = first2years_external._offset_time(gpstime, 'CBC')
 
-    ext_event = first2years_external.create_grb_event(new_time, 'Fermi')
+    ext_event = first2years_external.create_external_event(new_time, 'Fermi',
+                                                           'MDC')
 
     # Upload as from GCN
     external_triggers.handle_grb_gcn(ext_event)
 
     return ext_event
```

### Comparing `gwcelery-2.0.4/gwcelery/voevent/bootsteps.py` & `gwcelery-2.0.5/gwcelery/voevent/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/voevent/logging.py` & `gwcelery-2.0.5/gwcelery/voevent/logging.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/voevent/signals.py` & `gwcelery-2.0.5/gwcelery/voevent/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/voevent/subscriber.py` & `gwcelery-2.0.5/gwcelery/voevent/subscriber.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/gwcelery/voevent/util.py` & `gwcelery-2.0.5/gwcelery/voevent/util.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.4/pyproject.toml` & `gwcelery-2.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwcelery"
-version = "2.0.4"
+version = "2.0.5"
 description = "Low-latency pipeline for annotating IGWN events"
 readme = "README.rst"
 authors = [
     "Deep Chatterjee <deep.chatterjee@ligo.org>",
     "Cody Messick <cody.messick@ligo.org>",
     "Geoffrey Mo <geoffrey.mo@ligo.org>",
     "Leo Singer <leo.singer@ligo.org>"
@@ -13,15 +13,14 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
     "Operating System :: POSIX",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Internet",
     "Topic :: Scientific/Engineering :: Astronomy",
     "Topic :: Scientific/Engineering :: Physics"
 ]
 homepage = "https://git.ligo.org/emfollow/gwcelery"
@@ -47,20 +46,21 @@
     "gwcelery/tests/data/*.hdf5"
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://git.ligo.org/emfollow/gwcelery/issues"
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.11"
+python = "^3.9,<3.11"
 adc-streaming = ">=2.3.0"  # https://github.com/astronomy-commons/adc-streaming/pull/62
 astropy = ">=4.3.1"  # https://github.com/astropy/astropy/issues/11879
-bilby = ">=2.0.0"
-bilby-pipe = ">=1.0.8"
+bilby = ">=2.1.0"
+bilby_pipe = ">=1.0.10"
 celery = {version = ">=5.1", extras = ["redis"]}
+ciecplib = {version = "*", extras = ["kerberos"]}  # for renew-cert.sh
 click = ">=7"
 comet = "*"
 confluent-kafka = "^1.9.2"
 dnspython = "*"  # silence "DNS: dnspython not found. Can not use SRV lookup." warning from SleekXMPP
 flask = ">=2.2"
 flask-caching = "*"
 gracedb-sdk = ">=0.2.0"  # https://git.ligo.org/emfollow/gracedb-sdk/-/merge_requests/7
@@ -70,32 +70,32 @@
 hop-client = ">=0.7.0"  # https://github.com/scimma/hop-client/pull/176
 igwn-alert = ">=0.2.2"
 igwn-gwalert-schema = "^1.0.0"
 imapclient = "*"
 importlib-metadata = { version = "*"}
 jinja2 = ">=2.11.2"  # https://github.com/pallets/jinja/issues/1168
 lalsuite = ">=6.82"  # https://git.ligo.org/lscsoft/lalsuite/-/issues/414
-ligo-followup-advocate = ">=1.1.6"
+ligo-followup-advocate = ">=1.2.1"
 ligo-gracedb = ">=2.7.5"  # https://git.ligo.org/lscsoft/gracedb-client/-/issues/28
-ligo-raven = "^2.0"
+ligo-raven = ">=3.1"
 ligo-segments = "*"
-"ligo.em-bright" = "==1.1.0"  # https://git.ligo.org/emfollow/em-properties/em-bright/-/merge_requests/45
+"ligo.em-bright" = ">=1.1.1"  # https://git.ligo.org/emfollow/em-properties/em-bright/-/issues/23
 "ligo.skymap" = ">=1.0.4"  # https://git.ligo.org/lscsoft/ligo.skymap/-/merge_requests/299
 lscsoft-glue = "*"
 lxml = "*"
 matplotlib = "<3.7"  # Matplotlib changed an axes behaviour which breaks some of our plotting scripts. When gwpy has a new release, we can unpin this.
-numba = ">=0.56" # Poetry update chooses an old version of numba and its deps that break the python3.9 and 3.10 build tests if this is not specified; dependence on numba comes from rift. Version chosen because it adds python 3.10 support. This requirement can be dropped here if RIFT adds it https://git.ligo.org/rapidpe-rift/rift/-/issues/24
+numba = ">=0.56"  # Poetry update chooses an old version of numba and its deps that break the python3.9 and 3.10 build tests if this is not specified; dependence on numba comes from rift. Version chosen because it adds python 3.10 support. This requirement can be dropped here if RIFT adds it https://git.ligo.org/rapidpe-rift/rift/-/issues/24
 numpy = "*"
-p-astro = ">=1.0.1"  # https://git.ligo.org/lscsoft/p-astro/-/merge_requests/40
+p_astro = ">=1.0.1"  # https://git.ligo.org/lscsoft/p-astro/-/merge_requests/40
 pesummary = "*"
 pygcn = ">=1.0.1"
 python-ligo-lw = "^1.8.3"
-rapid-pe = ">=0.0.4"
-rapidpe-rift-pipe = ">=0.0.8"
-redis = "<4.5.2" # https://git.ligo.org/emfollow/gwcelery/-/issues/556 May need to change to "!=4.5.2" if issue fixed upstream
+rapid-pe = ">=0.0.6"  # https://git.ligo.org/computing/sccb/-/issues/1154
+rapidpe-rift-pipe = ">=0.0.12"  # https://git.ligo.org/computing/sccb/-/issues/1155
+redis = "!=4.5.2,!=4.5.3"  # https://git.ligo.org/emfollow/gwcelery/-/issues/556
 RIFT = ">=0.0.15.7"
 scipy = "<1.10"  # https://github.com/astropy/astropy/issues/14230
 safe-netrc = "*"
 sentry-sdk = {version = "*", extras = ["flask", "tornado"]}
 service-identity = "*"  # We don't actually use this package, but it silences some annoying warnings from twistd.
 voeventlib = ">=1.2"
 werkzeug = ">=0.15.0"  # for werkzeug.middleware.proxy_fix.ProxyFix
@@ -107,14 +107,15 @@
 
 # For tests
 fastavro = {version = "^1.6.1", optional = true}
 pytest-celery = {version="*", optional=true}
 pytest-cov = {version="*", optional=true}
 pytest-flask = {version="*", optional=true}
 pytest-socket = {version="*", optional=true}
+ligo-rrt-chat = ">=0.1.1"
 
 [tool.poetry.extras]
 doc = ["pep517", "sphinx"]
 test = ["fastavro", "pytest-celery", "pytest-cov", "pytest-flask", "pytest-socket"]
 
 [tool.poetry.group.dev.dependencies]
 ipython = "*"  # Include IPython for a nicer ``gwcelery shell`` experience.
```

### Comparing `gwcelery-2.0.4/PKG-INFO` & `gwcelery-2.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: gwcelery
-Version: 2.0.4
+Version: 2.0.5
 Summary: Low-latency pipeline for annotating IGWN events
 Home-page: https://git.ligo.org/emfollow/gwcelery
 License: GPL-2.0+
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: RIFT (>=0.0.15.7)
 Requires-Dist: adc-streaming (>=2.3.0)
 Requires-Dist: astropy (>=4.3.1)
-Requires-Dist: bilby (>=2.0.0)
-Requires-Dist: bilby-pipe (>=1.0.8)
+Requires-Dist: bilby (>=2.1.0)
+Requires-Dist: bilby_pipe (>=1.0.10)
 Requires-Dist: celery[redis] (>=5.1)
+Requires-Dist: ciecplib[kerberos]
 Requires-Dist: click (>=7)
 Requires-Dist: comet
 Requires-Dist: confluent-kafka (>=1.9.2,<2.0.0)
 Requires-Dist: dnspython
 Requires-Dist: fastavro (>=1.6.1,<2.0.0) ; extra == "test"
 Requires-Dist: flask (>=2.2)
 Requires-Dist: flask-caching
@@ -45,37 +44,38 @@
 Requires-Dist: hop-client (>=0.7.0)
 Requires-Dist: igwn-alert (>=0.2.2)
 Requires-Dist: igwn-gwalert-schema (>=1.0.0,<2.0.0)
 Requires-Dist: imapclient
 Requires-Dist: importlib-metadata
 Requires-Dist: jinja2 (>=2.11.2)
 Requires-Dist: lalsuite (>=6.82)
-Requires-Dist: ligo-followup-advocate (>=1.1.6)
+Requires-Dist: ligo-followup-advocate (>=1.2.1)
 Requires-Dist: ligo-gracedb (>=2.7.5)
-Requires-Dist: ligo-raven (>=2.0,<3.0)
+Requires-Dist: ligo-raven (>=3.1)
+Requires-Dist: ligo-rrt-chat (>=0.1.1)
 Requires-Dist: ligo-segments
-Requires-Dist: ligo.em-bright (==1.1.0)
+Requires-Dist: ligo.em-bright (>=1.1.1)
 Requires-Dist: ligo.skymap (>=1.0.4)
 Requires-Dist: lscsoft-glue
 Requires-Dist: lxml
 Requires-Dist: matplotlib (<3.7)
 Requires-Dist: numba (>=0.56)
 Requires-Dist: numpy
-Requires-Dist: p-astro (>=1.0.1)
+Requires-Dist: p_astro (>=1.0.1)
 Requires-Dist: pep517 ; extra == "doc"
 Requires-Dist: pesummary
 Requires-Dist: pygcn (>=1.0.1)
 Requires-Dist: pytest-celery ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-flask ; extra == "test"
 Requires-Dist: pytest-socket ; extra == "test"
 Requires-Dist: python-ligo-lw (>=1.8.3,<2.0.0)
-Requires-Dist: rapid-pe (>=0.0.4)
-Requires-Dist: rapidpe-rift-pipe (>=0.0.8)
-Requires-Dist: redis (<4.5.2)
+Requires-Dist: rapid-pe (>=0.0.6)
+Requires-Dist: rapidpe-rift-pipe (>=0.0.12)
+Requires-Dist: redis (!=4.5.2,!=4.5.3)
 Requires-Dist: safe-netrc
 Requires-Dist: scipy (<1.10)
 Requires-Dist: sentry-sdk[flask,tornado]
 Requires-Dist: service-identity
 Requires-Dist: sphinx (>=4.0,<=5.3.0) ; extra == "doc"
 Requires-Dist: voeventlib (>=1.2)
 Requires-Dist: werkzeug (>=0.15.0)
```

