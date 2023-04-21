# Comparing `tmp/cg-29.0.3.tar.gz` & `tmp/cg-29.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cg-29.0.3.tar", last modified: Thu Apr 20 10:00:08 2023, max compression
+gzip compressed data, was "dist/cg-29.1.0.tar", last modified: Thu Apr 20 12:19:02 2023, max compression
```

## Comparing `cg-29.0.3.tar` & `cg-29.1.0.tar`

### file list

```diff
@@ -1,1229 +1,1229 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 10:00:00.000000 cg-29.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-20 10:00:08.000000 cg-29.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-20 10:00:00.000000 cg-29.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 10:00:00.000000 cg-29.0.3/cg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/crud/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/crud/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/crud/find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/cgstats/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/cgstats/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/db/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/db/models/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/db/models/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/db/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/db/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/db/models/support_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/db/models/unaligned.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/db/models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/dragen_demux_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/parsers/adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/parsers/conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/parsers/demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/parsers/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/parsers/run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/cgstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/crunchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/crunchy/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/crunchy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/crunchy/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/demultiplex/demux_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/demultiplex/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/demultiplex/sample_sheet/dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/hermes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/hermes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/hermes/hermes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/hermes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/housekeeper/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/housekeeper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/invoice/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/invoice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/lims/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/lims/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/lims/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/lims/samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/loqus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/madeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/madeline/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/mip/confighandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/orderform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/scout/scout_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/scout/scoutapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/slurm/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/slurm/slurm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/apps/tb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/tb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/tb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/tb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-20 10:00:00.000000 cg-29.0.3/cg/apps/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/compress/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/compress/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/delete/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/delete/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/delete/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/delete/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/deliver/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/demultiplex/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/demultiplex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/demultiplex/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/demultiplex/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/demultiplex/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/generate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/generate/report/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/generate/report/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/generate/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/set/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/set/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/set/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/store/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/fohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/nipt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/nipt/statina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/upload/observations/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/observations/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/fastq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/fluffy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/microsalt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/mip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/mip/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/workflow/mip_dna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/mip_dna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/workflow/mip_rna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/mip_rna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/workflow/mutant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/mutant/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/workflow/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/nextflow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/rnafusion/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/cli/workflow/tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-20 10:00:00.000000 cg-29.0.3/cg/cli/workflow/tower/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/cgstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/demultiplexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/gene_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/housekeeper_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/orderforms.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/sample_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/scout_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/sequencing.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-20 10:00:00.000000 cg-29.0.3/cg/constants/tb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-20 10:00:00.000000 cg-29.0.3/cg/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-20 10:00:00.000000 cg-29.0.3/cg/io/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-20 10:00:00.000000 cg-29.0.3/cg/io/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-20 10:00:00.000000 cg-29.0.3/cg/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-20 10:00:00.000000 cg-29.0.3/cg/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-20 10:00:00.000000 cg-29.0.3/cg/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/archive/ddn_dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18853 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/backup/pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/clean/demultiplexed_flow_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/clean/flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/compress/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/compress/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/deliver_ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/demultiplex/delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/demultiplex/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/observations/observations_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/case_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/pool_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/rml_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/orders/ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/report/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/report/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/report/field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/report/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/report/report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/report/templates/mip-dna_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/rsync/rsync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/rsync/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/tar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/tar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/tar/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/transfer/external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/transfer/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/transfer/lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/upload/fohm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/fohm/fohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/gisaid/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/upload/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/nipt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/nipt/nipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/upload/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/rnafusion/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    28473 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/fluffy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/mutant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/nextflow_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-20 10:00:00.000000 cg-29.0.3/cg/meta/workflow/tower_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/balsamic/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/balsamic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/balsamic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/cg_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/cgstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/cgstats/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/cgstats/stats_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/compression_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/deliverables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/deliverables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/deliverables/metric_deliverables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/demultiplex/demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/demultiplex/flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/invoice/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/lims/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/lims/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/mip/mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/mip/mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/mip/mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/nextflow/deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/nextflow/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/observations/input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/orders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/orders/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/orders/excel_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/orders/json_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/orders/orderform_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/orders/sample_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/orders/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/report/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/report/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/report/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/rnafusion/rnafusion_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/scout/scout_load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/slurm/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-20 10:00:00.000000 cg-29.0.3/cg/models/workflow/mutant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-04-20 10:00:00.000000 cg-29.0.3/cg/resources/20181012_Indices.csv
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 10:00:00.000000 cg-29.0.3/cg/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-20 10:00:00.000000 cg-29.0.3/cg/resources/rnafusion_bundle_filenames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16689 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/server/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/server/invoices/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/server/invoices/templates/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/invoices/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/server/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 10:00:00.000000 cg-29.0.3/cg/server/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/store/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/api/find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    31917 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/api/find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    39238 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_case_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/filters/status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    27648 2023-04-20 10:00:00.000000 cg-29.0.3/cg/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/utils/checksum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/checksum/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/utils/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/click/EnumChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg/utils/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/flask/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-20 10:00:00.000000 cg-29.0.3/cg/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/cg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-20 10:00:08.000000 cg-29.0.3/cg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39148 2023-04-20 10:00:08.000000 cg-29.0.3/cg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:00:08.000000 cg-29.0.3/cg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 10:00:08.000000 cg-29.0.3/cg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:00:08.000000 cg-29.0.3/cg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-20 10:00:08.000000 cg-29.0.3/cg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-20 10:00:08.000000 cg-29.0.3/cg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 10:00:00.000000 cg-29.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-20 10:00:00.000000 cg-29.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:00:08.000000 cg-29.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-20 10:00:00.000000 cg-29.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/cgstats/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/cgstats/crud/test_create_novaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/cgstats/crud/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/cgstats/parsers/test_adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/cgstats/parsers/test_conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/cgstats/parsers/test_demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/cgstats/parsers/test_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/cgstats/parsers/test_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/cgstats/test_cgstats_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/cgstats/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/coverage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/coverage/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/crunchy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/crunchy/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/crunchy/test_spring_decompression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/demultiplex/test_convert_to_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/demultiplex/test_parse_run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/demultiplex/test_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/gens/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/gens/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/gens/test_gens_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/gt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/gt/test_gt_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/hk/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/hk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/hk/test__getattr__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/hk/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/hk/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/hk/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/hk/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/hk/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/lims/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/lims/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/loqus/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/loqus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/loqus/test_loqusdb_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/madeline/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/madeline/test_madeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/mip/test_config_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/mutacc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/mutacc_auto/test_mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/orderform/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/orderform/test_orderform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/scout/test_scout_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/slurm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/test_apps_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/test_osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/apps/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-20 10:00:00.000000 cg-29.0.3/tests/apps/vogue/test_vogue_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/add/test_cli_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/add/test_cli_add_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/backup/test_backup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/clean/test_rsync_past_run_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/delete/test_cli_delete_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/deliver/test_run_deliver_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/demultiplex/test_add_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/demultiplex/test_stats_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/generate/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/generate/report/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/generate/test_cli_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/get/test_cli_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/get/test_cli_get_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/set/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/set/test_cli_set_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/store/test_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/test_cli_status_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/upload/test_cli_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/fastq/test_fastq_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/fluffy/test_cli_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/microsalt/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/workflow/microsalt/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/microsalt/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/microsalt/test_microsalt_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-20 10:00:00.000000 cg-29.0.3/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    61338 2023-04-20 10:00:00.000000 cg-29.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/DEMUX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/analysis/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/analysis/balsamic/tn_wgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/analysis/microsalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/analysis/mip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/analysis/sample_coverage.bed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/balsamic/case/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/crunchy/spring_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/hiseq_run/
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/raw_lims_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/fluffy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/fluffy/2020-23219-05/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/fluffy/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/gt/yellowhog.bcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/madeline/madeline.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/mip/dna/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/mip/dna/store/
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/mip/rna/
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/mip/rna/store/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/mip/sample_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/scout/panel_export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/apps/shipping/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/apps/shipping/scout-deploy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/cgweb_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/cgweb_orders/sarscov2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/data/cgfixture.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/data/hkstore.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/data/yellowhog/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/data/yellowhog/pedigree.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/io/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/io/example_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/io/example_json.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/orderforms/
--rw-r--r--   0 runner    (1001) docker     (123)   267284 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/1508.27.balsamic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   258613 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   266876 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   266141 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/1508.27.fastq.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   266967 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/1508.27.mip.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   266759 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    95878 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   163548 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/1604.15.rml.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    88463 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/1605.10.metagenome.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   227684 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/fixtures/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/report/case_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-20 10:00:00.000000 cg-29.0.3/tests/fixtures/report/lims_family.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-20 10:00:00.000000 cg-29.0.3/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-20 10:00:00.000000 cg-29.0.3/tests/io/test_io_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-20 10:00:00.000000 cg-29.0.3/tests/io/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-20 10:00:00.000000 cg-29.0.3/tests/io/test_io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-20 10:00:00.000000 cg-29.0.3/tests/io/test_io_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/archive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/archive/test_archiving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24579 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/backup/test_meta_pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/clean/test_clean_demultiplexed_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/clean/test_clean_flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/compress/test_compress_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/deliver/test_delivery_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/demultiplex/test_delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/demultiplex/test_rename_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/encryption/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/observations/test_meta_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/orders/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0 runner    (1001) docker     (123)    29074 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/orders/test_ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/report/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/report/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/report/test_report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/rsync/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/rsync/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/test_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/transfer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/transfer/test_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/transfer/test_meta_transfer_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/transfer/test_meta_transfer_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/gisaid/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/upload/gisaid/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/upload/mutacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/nipt/test_nipt_upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/test_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/test_upload_genotypes_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/upload/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/upload/vogue/test_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/workflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/workflow/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-20 10:00:00.000000 cg-29.0.3/tests/meta/workflow/test_prepare_fastq_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/hk_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/limsmock.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/madeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/osticket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/process_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/store_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-20 10:00:00.000000 cg-29.0.3/tests/mocks/tb_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/models/demultiplexing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/demultiplexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/demultiplexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/demultiplexing/test_demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/demultiplexing/test_flowcell_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/mip/test_mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/mip/test_mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/nextflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/nextflow/test_nextflow_deliver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/observations/test_observations_input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/report/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/test_cg_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/test_compression_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/test_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-20 10:00:00.000000 cg-29.0.3/tests/models/test_flowcell_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-20 10:00:00.000000 cg-29.0.3/tests/server/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-20 10:00:00.000000 cg-29.0.3/tests/server/test_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-20 10:00:00.000000 cg-29.0.3/tests/server/test_server_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 10:00:00.000000 cg-29.0.3/tests/small_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/store/api/add/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/add/test_store_add_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/add/test_store_add_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/add/test_store_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/add/test_store_add_flow_celll.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/store/api/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/delete/test_store_api_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/store/api/find/
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/find/test_find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/find/test_find_basic_data_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    28759 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/find/test_find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/find/test_find_business_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/find/test_find_business_data_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/find/test_find_business_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/store/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/status/test_analyses_to_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/status/test_analyses_to_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9779 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/status/test_store_api_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15264 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/status/test_store_api_status_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    54207 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/status/test_store_api_status_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/status/test_store_api_status_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/status/test_store_api_status_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/status/test_store_api_status_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    39472 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    26900 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29715 2023-04-20 10:00:00.000000 cg-29.0.3/tests/store_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-20 10:00:00.000000 cg-29.0.3/tests/test_store_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:08.000000 cg-29.0.3/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:00:00.000000 cg-29.0.3/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-20 10:00:00.000000 cg-29.0.3/tests/utils/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-20 10:00:00.000000 cg-29.0.3/tests/utils/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-20 10:00:00.000000 cg-29.0.3/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-20 10:00:00.000000 cg-29.0.3/tests/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-04-20 10:00:00.000000 cg-29.0.3/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-20 10:00:00.000000 cg-29.0.3/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 12:18:52.000000 cg-29.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-20 12:19:02.000000 cg-29.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-20 12:18:52.000000 cg-29.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 12:18:52.000000 cg-29.1.0/cg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/crud/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/crud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/crud/find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/cgstats/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/cgstats/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/db/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/db/models/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/db/models/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/db/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/db/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/db/models/support_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/db/models/unaligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/db/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/dragen_demux_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/parsers/adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/parsers/conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/parsers/demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/parsers/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/parsers/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/cgstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/crunchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/crunchy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/crunchy/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/demultiplex/demux_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/demultiplex/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/demultiplex/sample_sheet/dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/hermes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/hermes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/hermes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/housekeeper/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/housekeeper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/invoice/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/invoice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/lims/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/lims/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/lims/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/lims/samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/loqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/madeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/madeline/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/mip/confighandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/orderform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/scout/scout_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/scout/scoutapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/slurm/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/slurm/slurm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/apps/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/tb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/tb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/tb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-20 12:18:52.000000 cg-29.1.0/cg/apps/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19625 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/compress/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/compress/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/compress/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/delete/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/delete/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/delete/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/delete/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/deliver/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/demultiplex/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/demultiplex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/demultiplex/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/demultiplex/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/demultiplex/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/generate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/generate/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/generate/report/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/generate/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/set/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/set/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/set/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/store/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/fohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/nipt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/nipt/statina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/upload/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/observations/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/fastq/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/fluffy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/microsalt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/mip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/mip/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/workflow/mip_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/mip_dna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/workflow/mip_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/mip_rna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/workflow/mutant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/mutant/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/workflow/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/nextflow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/rnafusion/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/cli/workflow/tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-20 12:18:52.000000 cg-29.1.0/cg/cli/workflow/tower/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/cgstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/demultiplexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/gene_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/housekeeper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/orderforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/sample_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/scout_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/sequencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-20 12:18:52.000000 cg-29.1.0/cg/constants/tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-20 12:18:52.000000 cg-29.1.0/cg/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-20 12:18:52.000000 cg-29.1.0/cg/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-20 12:18:52.000000 cg-29.1.0/cg/io/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-20 12:18:52.000000 cg-29.1.0/cg/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-20 12:18:52.000000 cg-29.1.0/cg/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-20 12:18:52.000000 cg-29.1.0/cg/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/archive/ddn_dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/backup/pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/clean/demultiplexed_flow_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/clean/flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/compress/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/compress/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/deliver_ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/demultiplex/delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15617 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/demultiplex/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/observations/observations_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/case_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/orders/ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/report/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/report/field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/report/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/report/report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/report/templates/mip-dna_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/rsync/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/tar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/tar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/tar/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/transfer/external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/transfer/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/transfer/lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/upload/fohm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/fohm/fohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/upload/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/nipt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/nipt/nipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/upload/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/rnafusion/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20184 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28473 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/fluffy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/mutant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/nextflow_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-20 12:18:52.000000 cg-29.1.0/cg/meta/workflow/tower_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/balsamic/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/balsamic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/balsamic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/cg_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/cgstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/cgstats/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/cgstats/stats_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/compression_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/deliverables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/deliverables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/deliverables/metric_deliverables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/demultiplex/demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/demultiplex/flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/invoice/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/lims/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/mip/mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/mip/mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/mip/mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/nextflow/deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/nextflow/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/observations/input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/orders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/orders/excel_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/orders/json_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/orders/orderform_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/orders/sample_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/orders/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/report/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/report/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/report/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/rnafusion/rnafusion_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/scout/scout_load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/slurm/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-20 12:18:52.000000 cg-29.1.0/cg/models/workflow/mutant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-04-20 12:18:52.000000 cg-29.1.0/cg/resources/20181012_Indices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 12:18:52.000000 cg-29.1.0/cg/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-20 12:18:52.000000 cg-29.1.0/cg/resources/rnafusion_bundle_filenames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/server/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/server/invoices/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/server/invoices/templates/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/invoices/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 12:18:52.000000 cg-29.1.0/cg/server/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/api/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/api/find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31878 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/api/find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39247 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_case_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/filters/status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28524 2023-04-20 12:18:52.000000 cg-29.1.0/cg/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/utils/checksum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/checksum/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/utils/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/click/EnumChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg/utils/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/flask/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-20 12:18:52.000000 cg-29.1.0/cg/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/cg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-20 12:19:02.000000 cg-29.1.0/cg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39148 2023-04-20 12:19:02.000000 cg-29.1.0/cg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:19:02.000000 cg-29.1.0/cg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 12:19:02.000000 cg-29.1.0/cg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:19:02.000000 cg-29.1.0/cg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-20 12:19:02.000000 cg-29.1.0/cg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-20 12:19:02.000000 cg-29.1.0/cg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 12:18:52.000000 cg-29.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-20 12:18:52.000000 cg-29.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:19:02.000000 cg-29.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-20 12:18:52.000000 cg-29.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/cgstats/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/cgstats/crud/test_create_novaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/cgstats/crud/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/cgstats/parsers/test_adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/cgstats/parsers/test_conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/cgstats/parsers/test_demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/cgstats/parsers/test_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/cgstats/parsers/test_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/cgstats/test_cgstats_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/cgstats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/coverage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/coverage/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/crunchy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/crunchy/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/crunchy/test_spring_decompression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/demultiplex/test_convert_to_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/demultiplex/test_parse_run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/demultiplex/test_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/gens/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/gens/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/gens/test_gens_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/gt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/gt/test_gt_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/hk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/hk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/hk/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/hk/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/hk/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/hk/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/hk/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/lims/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/lims/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/loqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/loqus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/loqus/test_loqusdb_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/madeline/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/madeline/test_madeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/mip/test_config_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/mutacc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/mutacc_auto/test_mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/orderform/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/orderform/test_orderform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/scout/test_scout_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/slurm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/test_apps_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/test_osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/apps/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-20 12:18:52.000000 cg-29.1.0/tests/apps/vogue/test_vogue_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/add/test_cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/add/test_cli_add_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/backup/test_backup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/clean/test_rsync_past_run_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/delete/test_cli_delete_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/deliver/test_run_deliver_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/demultiplex/test_add_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/demultiplex/test_stats_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/generate/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/generate/test_cli_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/get/test_cli_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/get/test_cli_get_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/set/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/set/test_cli_set_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/store/test_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/test_cli_status_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/upload/test_cli_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    31010 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/fastq/test_fastq_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/fluffy/test_cli_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/microsalt/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/workflow/microsalt/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/microsalt/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/microsalt/test_microsalt_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-20 12:18:52.000000 cg-29.1.0/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61436 2023-04-20 12:18:52.000000 cg-29.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/DEMUX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/analysis/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/analysis/balsamic/tn_wgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/analysis/microsalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/analysis/mip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/analysis/sample_coverage.bed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/balsamic/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/crunchy/spring_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/hiseq_run/
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/fluffy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/fluffy/2020-23219-05/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/fluffy/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/gt/yellowhog.bcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/madeline/madeline.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/mip/dna/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/mip/dna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/mip/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/mip/rna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/mip/sample_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/scout/panel_export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/apps/shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/apps/shipping/scout-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/cgweb_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/cgweb_orders/sarscov2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/data/hkstore.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/data/yellowhog/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/data/yellowhog/pedigree.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/io/example_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/io/example_json.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/orderforms/
+-rw-r--r--   0 runner    (1001) docker     (123)   267284 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/1508.27.balsamic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   258613 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   266876 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   266141 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/1508.27.fastq.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   266967 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/1508.27.mip.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   266759 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    95878 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   163548 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/1604.15.rml.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    88463 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/1605.10.metagenome.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   227684 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/fixtures/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/report/case_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-20 12:18:52.000000 cg-29.1.0/tests/fixtures/report/lims_family.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-20 12:18:52.000000 cg-29.1.0/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-20 12:18:52.000000 cg-29.1.0/tests/io/test_io_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-20 12:18:52.000000 cg-29.1.0/tests/io/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-20 12:18:52.000000 cg-29.1.0/tests/io/test_io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-20 12:18:52.000000 cg-29.1.0/tests/io/test_io_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/archive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/archive/test_archiving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24603 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/backup/test_meta_pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/clean/test_clean_demultiplexed_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/clean/test_clean_flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/deliver/test_delivery_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/demultiplex/test_delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/demultiplex/test_rename_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/encryption/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/observations/test_meta_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/orders/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19944 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29129 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/orders/test_ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/report/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/report/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/report/test_report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/rsync/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/test_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/transfer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/transfer/test_meta_transfer_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/transfer/test_meta_transfer_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/gisaid/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/upload/gisaid/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/upload/mutacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/nipt/test_nipt_upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24993 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/test_upload_genotypes_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/upload/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/upload/vogue/test_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/workflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-20 12:18:52.000000 cg-29.1.0/tests/meta/workflow/test_prepare_fastq_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/hk_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/limsmock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/madeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/osticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/process_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/store_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-20 12:18:52.000000 cg-29.1.0/tests/mocks/tb_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/models/demultiplexing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/demultiplexing/test_demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/demultiplexing/test_flowcell_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/mip/test_mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/mip/test_mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/nextflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/nextflow/test_nextflow_deliver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/observations/test_observations_input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/report/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/test_cg_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/test_compression_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/test_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-20 12:18:52.000000 cg-29.1.0/tests/models/test_flowcell_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-20 12:18:52.000000 cg-29.1.0/tests/server/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-20 12:18:52.000000 cg-29.1.0/tests/server/test_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-20 12:18:52.000000 cg-29.1.0/tests/server/test_server_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 12:18:52.000000 cg-29.1.0/tests/small_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/store/api/add/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/add/test_store_add_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/add/test_store_add_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/add/test_store_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/add/test_store_add_flow_celll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19418 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/store/api/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/delete/test_store_api_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/store/api/find/
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/find/test_find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/find/test_find_basic_data_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28823 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/find/test_find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/find/test_find_business_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/find/test_find_business_data_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/find/test_find_business_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/store/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/status/test_analyses_to_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/status/test_analyses_to_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/status/test_store_api_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/status/test_store_api_status_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54240 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/status/test_store_api_status_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/status/test_store_api_status_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/status/test_store_api_status_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/status/test_store_api_status_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39481 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26900 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-04-20 12:18:52.000000 cg-29.1.0/tests/store_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-20 12:18:52.000000 cg-29.1.0/tests/test_store_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:19:02.000000 cg-29.1.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:18:52.000000 cg-29.1.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-20 12:18:52.000000 cg-29.1.0/tests/utils/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-20 12:18:52.000000 cg-29.1.0/tests/utils/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-20 12:18:52.000000 cg-29.1.0/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-20 12:18:52.000000 cg-29.1.0/tests/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-04-20 12:18:52.000000 cg-29.1.0/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-20 12:18:52.000000 cg-29.1.0/tests/utils/test_utils.py
```

### Comparing `cg-29.0.3/PKG-INFO` & `cg-29.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 29.0.3
+Version: 29.1.0
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-29.0.3/README.md` & `cg-29.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/crud/create.py` & `cg-29.1.0/cg/apps/cgstats/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/crud/delete.py` & `cg-29.1.0/cg/apps/cgstats/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/crud/find.py` & `cg-29.1.0/cg/apps/cgstats/crud/find.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/db/models/base.py` & `cg-29.1.0/cg/apps/cgstats/db/models/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/db/models/datasource.py` & `cg-29.1.0/cg/apps/cgstats/db/models/datasource.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/db/models/demux.py` & `cg-29.1.0/cg/apps/cgstats/db/models/demux.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/db/models/flowcell.py` & `cg-29.1.0/cg/apps/cgstats/db/models/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/db/models/project.py` & `cg-29.1.0/cg/apps/cgstats/db/models/project.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/db/models/sample.py` & `cg-29.1.0/cg/apps/cgstats/db/models/sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/db/models/support_params.py` & `cg-29.1.0/cg/apps/cgstats/db/models/support_params.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/db/models/unaligned.py` & `cg-29.1.0/cg/apps/cgstats/db/models/unaligned.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/db/models/version.py` & `cg-29.1.0/cg/apps/cgstats/db/models/version.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/demux_sample.py` & `cg-29.1.0/cg/apps/cgstats/demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/dragen_demux_sample.py` & `cg-29.1.0/cg/apps/cgstats/dragen_demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/parsers/adapter_metrics.py` & `cg-29.1.0/cg/apps/cgstats/parsers/adapter_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/parsers/conversion_stats.py` & `cg-29.1.0/cg/apps/cgstats/parsers/conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/parsers/demux_stats.py` & `cg-29.1.0/cg/apps/cgstats/parsers/demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py` & `cg-29.1.0/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/parsers/quality_metrics.py` & `cg-29.1.0/cg/apps/cgstats/parsers/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/parsers/run_info.py` & `cg-29.1.0/cg/apps/cgstats/parsers/run_info.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/cgstats/stats.py` & `cg-29.1.0/cg/apps/cgstats/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     def flow_cell_reads_and_q30_summary(self, flow_cell_name: str) -> Dict[str, Union[int, float]]:
         flow_cell_reads_and_q30_summary: Dict[str, Union[int, float]] = {"reads": 0, "q30": 0.0}
         flow_cell_obj: models.Flowcell = self.Flowcell.query.filter(
             models.Flowcell.flowcellname == flow_cell_name
         ).first()
 
-        if flow_cell_obj.exists(flowcell_name=flow_cell_name):
+        if flow_cell_obj and flow_cell_obj.exists(flowcell_name=flow_cell_name):
             sample_count: int = 0
             q30_list: List[float] = []
 
             for sample in self.flowcell_samples(flowcell_obj=flow_cell_obj):
                 sample_count += 1
                 sample_info = self.sample_reads(sample_obj=sample).first()
                 flow_cell_reads_and_q30_summary["reads"] += int(sample_info.reads)
```

### Comparing `cg-29.0.3/cg/apps/coverage/api.py` & `cg-29.1.0/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/crunchy/crunchy.py` & `cg-29.1.0/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/crunchy/files.py` & `cg-29.1.0/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/crunchy/sbatch.py` & `cg-29.1.0/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/demultiplex/demultiplex_api.py` & `cg-29.1.0/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/demultiplex/demux_report.py` & `cg-29.1.0/cg/apps/demultiplex/demux_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/demultiplex/sample_sheet/create.py` & `cg-29.1.0/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/demultiplex/sample_sheet/dummy_sample.py` & `cg-29.1.0/cg/apps/demultiplex/sample_sheet/dummy_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/demultiplex/sample_sheet/index.py` & `cg-29.1.0/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py` & `cg-29.1.0/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/demultiplex/sbatch.py` & `cg-29.1.0/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/gens.py` & `cg-29.1.0/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/gt.py` & `cg-29.1.0/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/hermes/hermes_api.py` & `cg-29.1.0/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/hermes/models.py` & `cg-29.1.0/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/housekeeper/hk.py` & `cg-29.1.0/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/invoice/render.py` & `cg-29.1.0/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-29.1.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-29.1.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-29.1.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-29.1.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/lims/api.py` & `cg-29.1.0/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/lims/batch.py` & `cg-29.1.0/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/lims/order.py` & `cg-29.1.0/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/lims/samplesheet.py` & `cg-29.1.0/cg/apps/lims/samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/loqus.py` & `cg-29.1.0/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/madeline/api.py` & `cg-29.1.0/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/mip/confighandler.py` & `cg-29.1.0/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/mutacc_auto.py` & `cg-29.1.0/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/orderform/excel_orderform_parser.py` & `cg-29.1.0/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/orderform/json_orderform_parser.py` & `cg-29.1.0/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/orderform/orderform_parser.py` & `cg-29.1.0/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/osticket.py` & `cg-29.1.0/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/scout/scout_export.py` & `cg-29.1.0/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/scout/scoutapi.py` & `cg-29.1.0/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/slurm/sbatch.py` & `cg-29.1.0/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/slurm/slurm_api.py` & `cg-29.1.0/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/tb/api.py` & `cg-29.1.0/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/tb/models.py` & `cg-29.1.0/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/apps/vogue.py` & `cg-29.1.0/cg/apps/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/add.py` & `cg-29.1.0/cg/cli/add.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,15 +84,16 @@
         internal_id=internal_id,
         name=name,
         invoice_address=invoice_address,
         invoice_reference=invoice_reference,
     )
     for collaboration in collaborations:
         new_customer.collaborations.append(collaboration)
-    status_db.add_commit(new_customer)
+    status_db.session.add(new_customer)
+    status_db.session.commit()
     message: str = f"customer added: {new_customer.internal_id} ({new_customer.id})"
     LOG.info(message)
 
 
 @add.command()
 @click.option("-a", "--admin", is_flag=True, help="make the user an admin")
 @click.option(
@@ -114,15 +115,16 @@
     if existing_user:
         LOG.error(f"{existing_user.name}: user already added")
         raise click.Abort
 
     new_user: User = status_db.add_user(
         customer=customer_obj, email=email, name=name, is_admin=admin
     )
-    status_db.add_commit(new_user)
+    status_db.session.add(new_user)
+    status_db.session.commit()
     LOG.info(f"User added: {new_user.email} ({new_user.id})")
 
 
 @add.command()
 @click.option("-l", "--lims", "lims_id", help="LIMS id for the sample")
 @click.option(
     "-d", "--down-sampled", type=int, help="How many reads is the sample down sampled to?"
@@ -177,15 +179,16 @@
         order=order,
         priority=priority,
     )
     new_record.application_version: ApplicationVersion = (
         status_db.get_current_application_version_by_tag(tag=application_tag)
     )
     new_record.customer: Customer = customer
-    status_db.add_commit(new_record)
+    status_db.session.add(new_record)
+    status_db.session.commit()
     LOG.info(f"{new_record.internal_id}: new sample added")
 
 
 @add.command()
 @click.option(
     "--priority",
     type=EnumChoice(Priority, use_value=False),
@@ -244,15 +247,16 @@
         name=name,
         panels=list(panel_abbreviations),
         priority=priority,
         ticket=ticket,
     )
 
     new_case.customer: Customer = customer
-    status_db.add_commit(new_case)
+    status_db.session.add(new_case)
+    status_db.session.commit()
     LOG.info(f"{new_case.internal_id}: new case added")
 
 
 @add.command()
 @click.option("-m", "--mother-id", help="Sample ID for mother of sample")
 @click.option("-f", "--father-id", help="Sample ID for father of sample")
 @click.option("-s", "--status", type=click.Choice(STATUS_OPTIONS), required=True)
@@ -292,15 +296,16 @@
         if father is None:
             LOG.error("%s: father not found", father_id)
             raise click.Abort
 
     new_record: FamilySample = status_db.relate_sample(
         family=case_obj, sample=sample, status=status, mother=mother, father=father
     )
-    status_db.add_commit(new_record)
+    status_db.session.add(new_record)
+    status_db.session.commit()
     LOG.info("related %s to %s", case_obj.internal_id, sample.internal_id)
 
 
 @add.command()
 @click.option(
     "-t",
     "--ticket",
```

### Comparing `cg-29.0.3/cg/cli/backup.py` & `cg-29.1.0/cg/cli/backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         hours = retrieval_time / 60 / 60
         LOG.info(f"Retrieval time: {hours:.1}h")
         return
 
     if not dry_run and flow_cell:
         LOG.info(f"{flow_cell}: updating flow cell status to {FlowCellStatus.REQUESTED}")
         flow_cell.status = FlowCellStatus.REQUESTED
-        status_api.commit()
+        status_api.session.commit()
 
 
 @backup.command("archive-spring-files")
 @DRY_RUN
 @click.pass_context
 @click.pass_obj
 def archive_spring_files(config: CGConfig, context: click.Context, dry_run: bool):
```

### Comparing `cg-29.0.3/cg/cli/base.py` & `cg-29.1.0/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/clean.py` & `cg-29.1.0/cg/cli/clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,15 @@
         if flow_cell.status != new_status:
             LOG.info(
                 f"Setting status of flow cell {flow_cell.name} from: {flow_cell.status} to {new_status}"
             )
             if dry_run:
                 continue
             flow_cell.status: str = new_status
-            status_db.commit()
+            status_db.session.commit()
 
 
 @clean.command("remove-old-flow-cell-run-dirs")
 @click.option(
     "-s",
     "--sequencer",
     type=click.Choice([Sequencers.HISEQX, Sequencers.HISEQGA, Sequencers.NOVASEQ, Sequencers.ALL]),
```

### Comparing `cg-29.0.3/cg/cli/compress/base.py` & `cg-29.1.0/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/compress/fastq.py` & `cg-29.1.0/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/compress/helpers.py` & `cg-29.1.0/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/delete/case.py` & `cg-29.1.0/cg/cli/delete/case.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,16 @@
         raise click.Abort
 
     if dry_run:
         LOG.info(f"Case: {case_id} was NOT deleted due to --dry-run")
         return
 
     LOG.info(f"Deleting case: {case_id}")
-    status_db.delete_commit(case)
+    status_db.session.delete(case)
+    status_db.session.commit()
 
 
 def _delete_links_and_samples(case_obj: Family, dry_run: bool, status_db: Store, yes: bool):
     """Delete all links from a case to samples"""
     samples_to_delete: List[Sample] = []
     for case_link in case_obj.links:
         if not (yes or click.confirm(f"Do you want to DELETE link: {case_link}?")):
@@ -66,15 +67,16 @@
 
         samples_to_delete.append(case_link.sample)
 
         if dry_run:
             LOG.info("Link: %s was NOT deleted due to --dry-run", case_link)
         else:
             LOG.info("Deleting link: %s", case_link)
-            status_db.delete_commit(case_link)
+            status_db.session.delete(case_link)
+            status_db.session.commit()
 
     for sample in samples_to_delete:
         _delete_sample(dry_run=dry_run, sample=sample, status_db=status_db, yes=yes)
 
 
 def _delete_sample(dry_run: bool, sample: Sample, status_db: Store, yes: bool):
     if _has_sample_been_lab_processed(sample):
@@ -97,15 +99,15 @@
         return
 
     if dry_run:
         LOG.info("Sample: %s was NOT deleted due to --dry-run", sample)
         return
 
     LOG.info("Deleting sample: %s", sample)
-    status_db.delete(sample)
+    status_db.session.delete(sample)
 
 
 def _log_sample_process_information(sample: Sample):
     LOG.info("Can NOT delete processed sample: %s", sample.internal_id)
     LOG.info("Sample was received: %s", sample.received_at)
     LOG.info("Sample was prepared: %s", sample.prepared_at)
     LOG.info("Sample was sequenced: %s", sample.sequenced_at)
```

### Comparing `cg-29.0.3/cg/cli/delete/cases.py` & `cg-29.1.0/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/delete/observations.py` & `cg-29.1.0/cg/cli/delete/observations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Delete observations CLI."""
 
 import logging
 from typing import Optional, Union
 
 import click
-from alchy import Query
+from sqlalchemy.orm import Query
 from cgmodels.cg.constants import Pipeline
 
 from cg.cli.upload.observations.utils import get_observations_api, get_observations_case
 from cg.cli.workflow.commands import OPTION_LOQUSDB_SUPPORTED_PIPELINES, ARGUMENT_CASE_ID
 from cg.exc import CaseNotFoundError, LoqusdbError
 from cg.meta.observations.balsamic_observations_api import BalsamicObservationsAPI
 from cg.meta.observations.mip_dna_observations_api import MipDNAObservationsAPI
```

### Comparing `cg-29.0.3/cg/cli/deliver/base.py` & `cg-29.1.0/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/demultiplex/add.py` & `cg-29.1.0/cg/cli/demultiplex/add.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/demultiplex/base.py` & `cg-29.1.0/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/demultiplex/demux.py` & `cg-29.1.0/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/demultiplex/finish.py` & `cg-29.1.0/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/demultiplex/report.py` & `cg-29.1.0/cg/cli/demultiplex/report.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/demultiplex/sample_sheet.py` & `cg-29.1.0/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/export.py` & `cg-29.1.0/cg/cli/export.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/generate/report/base.py` & `cg-29.1.0/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/generate/report/options.py` & `cg-29.1.0/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/generate/report/utils.py` & `cg-29.1.0/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/get.py` & `cg-29.1.0/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/set/base.py` & `cg-29.1.0/cg/cli/set/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
 
         if key == "comment":
             _update_comment(new_value, sample)
         else:
             setattr(sample, new_key, new_value)
             _update_comment(_generate_comment(new_key, old_value, new_value), sample)
 
-        status_db.commit()
+        status_db.session.commit()
 
     if not skip_lims:
         for key, value in kwargs:
             new_key = "application" if key == "application_version" else key
             new_value = sample.priority_human if key == "priority" else value
             LOG.info(f"Would set {new_key} to {new_value} for {sample.internal_id} in LIMS")
 
@@ -292,13 +292,13 @@
 
     if flowcell_obj is None:
         LOG.warning(f"flow cell not found: {flow_cell_name}")
         raise click.Abort
     prev_status: str = flowcell_obj.status
     flowcell_obj.status = status
 
-    status_db.commit()
+    status_db.session.commit()
     LOG.info(f"{flow_cell_name} set: {prev_status} -> {status}")
 
 
 set_cmd.add_command(case)
 set_cmd.add_command(cases)
```

### Comparing `cg-29.0.3/cg/cli/set/case.py` & `cg-29.1.0/cg/cli/set/case.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     if panel_abbreviations:
         update_panels(case=case, panel_abbreviations=panel_abbreviations, status_db=status_db)
 
     if priority:
         update_priority(case=case, priority=priority)
 
-    status_db.commit()
+    status_db.session.commit()
 
 
 def abort_on_empty_options(options: List[str]) -> None:
     if not any(options):
         LOG.error("Nothing to change")
         raise click.Abort
```

### Comparing `cg-29.0.3/cg/cli/set/cases.py` & `cg-29.1.0/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/status.py` & `cg-29.1.0/cg/cli/status.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/store/fastq.py` & `cg-29.1.0/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/store/store.py` & `cg-29.1.0/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/transfer.py` & `cg-29.1.0/cg/cli/transfer.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     """Populate results from a flow cell."""
     flow_cell_dir: Path = Path(flow_cell_dir)
     status_db: Store = context.status_db
     transfer_api: TransferFlowCell = context.meta_apis["transfer_flow_cell_api"]
     new_record: Flowcell = transfer_api.transfer(
         flow_cell_dir=flow_cell_dir, flow_cell_id=flow_cell_id, store=store
     )
-    status_db.add_commit(new_record)
+    status_db.session.add(new_record)
+    status_db.session.commit()
     LOG.info(f"flow cell added: {new_record}")
 
 
 @transfer_group.command()
 @click.option(
     "-s", "--status", type=click.Choice(["received", "prepared", "delivered"]), default="received"
 )
```

### Comparing `cg-29.0.3/cg/cli/upload/base.py` & `cg-29.1.0/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/clinical_delivery.py` & `cg-29.1.0/cg/cli/upload/clinical_delivery.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,8 +111,8 @@
                 )
             continue
         case: Family = analysis_obj.family
         LOG.info("Uploading family: %s", case.internal_id)
         analysis_obj.upload_started_at = dt.datetime.now()
         context.invoke(clinical_delivery, case_id=case.internal_id, dry_run=dry_run)
         if not dry_run:
-            status_db.commit()
+            status_db.session.commit()
```

### Comparing `cg-29.0.3/cg/cli/upload/coverage.py` & `cg-29.1.0/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/delivery_report.py` & `cg-29.1.0/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/fohm.py` & `cg-29.1.0/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/genotype.py` & `cg-29.1.0/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/gens.py` & `cg-29.1.0/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/gisaid.py` & `cg-29.1.0/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/mutacc.py` & `cg-29.1.0/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/nipt/base.py` & `cg-29.1.0/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/nipt/ftp.py` & `cg-29.1.0/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/nipt/statina.py` & `cg-29.1.0/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/observations/observations.py` & `cg-29.1.0/cg/cli/upload/observations/observations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import contextlib
 import logging
 from datetime import datetime
 from typing import Optional, Union
 
 import click
-from alchy import Query
+from sqlalchemy.orm import Query
 from cgmodels.cg.constants import Pipeline
 from pydantic import ValidationError
 
 from cg.cli.upload.observations.utils import get_observations_case_to_upload, get_observations_api
 from cg.exc import LoqusdbError, CaseNotFoundError
 from cg.meta.observations.balsamic_observations_api import BalsamicObservationsAPI
 from cg.meta.observations.mip_dna_observations_api import MipDNAObservationsAPI
```

### Comparing `cg-29.0.3/cg/cli/upload/observations/utils.py` & `cg-29.1.0/cg/cli/upload/observations/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Helper functions for observations related actions."""
 
 import logging
 from typing import Union
 
-from alchy import Query
+from sqlalchemy.orm import Query
 from cgmodels.cg.constants import Pipeline
 
 from cg.constants.observations import LOQUSDB_SUPPORTED_PIPELINES
 from cg.constants.sequencing import SequencingMethod
 from cg.exc import CaseNotFoundError, LoqusdbUploadCaseError
 from cg.meta.observations.balsamic_observations_api import BalsamicObservationsAPI
 from cg.meta.observations.mip_dna_observations_api import MipDNAObservationsAPI
```

### Comparing `cg-29.0.3/cg/cli/upload/scout.py` & `cg-29.1.0/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/utils.py` & `cg-29.1.0/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/validate.py` & `cg-29.1.0/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/upload/vogue.py` & `cg-29.1.0/cg/cli/upload/vogue.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import datetime as dt
 import logging
 from pathlib import Path
 from typing import Any, List, Optional, Tuple, Dict
 
 import click
-from sqlalchemy.orm import Query
 
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants import Pipeline
 from cg.exc import AnalysisUploadError
 from cg.meta.upload.vogue import UploadVogueAPI
 from cg.meta.workflow.mip_dna import MipDNAAnalysisAPI
 from cg.models.cg_config import CGConfig
@@ -265,15 +264,15 @@
             continue
 
         LOG.info("Found multiqc for %s, %s", case_name, existing_multiqc_file)
         try:
             context.invoke(bioinfo, case_name=case_name, cleanup=True, target_load="all", dry=dry)
             if not dry:
                 UploadVogueAPI.update_analysis_uploaded_to_vogue_date(analysis=analysis)
-                status_db.commit()
+                status_db.session.commit()
         except AnalysisUploadError:
             LOG.error("Case upload failed: %s", case_name, exc_info=True)
 
 
 def _get_multiqc_latest_file(hk_api: HousekeeperAPI, case_name: str) -> str:
     """Get latest multiqc_data.json path for a case_name
     Args:
```

### Comparing `cg-29.0.3/cg/cli/workflow/balsamic/base.py` & `cg-29.1.0/cg/cli/workflow/balsamic/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         raise error
     except CgError as error:
         LOG.error(f"Could not store bundle in Housekeeper and StatusDB: {error}")
         raise click.Abort()
     except Exception as error:
         LOG.error(f"Could not store bundle in Housekeeper and StatusDB: {error}!")
         housekeeper_api.rollback()
-        status_db.rollback()
+        status_db.session.rollback()
         raise click.Abort()
 
 
 @balsamic.command("start")
 @ARGUMENT_CASE_ID
 @OPTION_GENDER
 @OPTION_GENOME_VERSION
```

### Comparing `cg-29.0.3/cg/cli/workflow/balsamic/options.py` & `cg-29.1.0/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/workflow/balsamic/pon.py` & `cg-29.1.0/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/workflow/balsamic/qc.py` & `cg-29.1.0/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/workflow/balsamic/umi.py` & `cg-29.1.0/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/workflow/base.py` & `cg-29.1.0/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/workflow/commands.py` & `cg-29.1.0/cg/cli/workflow/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         return
     try:
         analysis_api.upload_bundle_housekeeper(case_id=case_id)
         analysis_api.upload_bundle_statusdb(case_id=case_id)
         analysis_api.set_statusdb_action(case_id=case_id, action=None)
     except Exception as exception_object:
         housekeeper_api.rollback()
-        status_db.rollback()
+        status_db.session.rollback()
         LOG.error("Error storing deliverables for case %s - %s", case_id, exception_object)
         raise
 
 
 @click.command("store-available")
 @OPTION_DRY
 @click.pass_context
```

### Comparing `cg-29.0.3/cg/cli/workflow/fastq/base.py` & `cg-29.1.0/cg/cli/workflow/fastq/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         completed_at=dt.datetime.now(),
         primary=True,
         started_at=dt.datetime.now(),
         family_id=case_obj.id,
     )
     if dry_run:
         return
-    status_db.add_commit(new_analysis)
+    status_db.session.add(new_analysis)
+    status_db.session.commit()
 
 
 @fastq.command("store-available")
 @DRY_RUN
 @click.pass_context
 def store_available_fastq_analysis(context: click.Context, dry_run: bool = False):
     """Creates an analysis object in status-db for all fastq cases to be delivered"""
```

### Comparing `cg-29.0.3/cg/cli/workflow/fluffy/base.py` & `cg-29.1.0/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/workflow/microsalt/base.py` & `cg-29.1.0/cg/cli/workflow/microsalt/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
     }
     analysis_api.vogue_api.load_bioinfo_raw(load_bioinfo_inputs=vogue_load_args)
     analysis_api.vogue_api.load_bioinfo_process(
         load_bioinfo_inputs=vogue_load_args, cleanup_flag=False
     )
     analysis_api.vogue_api.load_bioinfo_sample(load_bioinfo_inputs=vogue_load_args)
     case_obj.analyses[0].uploaded_at = dt.datetime.now()
-    analysis_api.status_db.commit()
+    analysis_api.status_db.session.commit()
     LOG.info("Successfully uploaded latest analysis data for case %s to Vogue!", unique_id)
 
 
 @microsalt.command("upload-latest-analyses-vogue")
 @OPTION_DRY_RUN
 @click.pass_context
 def upload_vogue_latest(context: click.Context, dry_run: bool) -> None:
```

### Comparing `cg-29.0.3/cg/cli/workflow/mip/base.py` & `cg-29.1.0/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/workflow/mip/options.py` & `cg-29.1.0/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/workflow/mip_dna/base.py` & `cg-29.1.0/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/workflow/mip_rna/base.py` & `cg-29.1.0/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/workflow/mutant/base.py` & `cg-29.1.0/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/workflow/nextflow/options.py` & `cg-29.1.0/cg/cli/workflow/nextflow/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/cli/workflow/rnafusion/base.py` & `cg-29.1.0/cg/cli/workflow/rnafusion/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
         raise error
     except CgError as error:
         LOG.error(f"Could not store bundle in Housekeeper and StatusDB: {error}")
         raise click.Abort()
     except Exception as error:
         LOG.error(f"Could not store bundle in Housekeeper and StatusDB: {error}!")
         housekeeper_api.rollback()
-        status_db.rollback()
+        status_db.session.rollback()
         raise click.Abort()
 
 
 @rnafusion.command("store")
 @ARGUMENT_CASE_ID
 @DRY_RUN
 @click.pass_context
```

### Comparing `cg-29.0.3/cg/cli/workflow/rnafusion/options.py` & `cg-29.1.0/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/__init__.py` & `cg-29.1.0/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/compression.py` & `cg-29.1.0/cg/constants/compression.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/constants.py` & `cg-29.1.0/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/delivery.py` & `cg-29.1.0/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/demultiplexing.py` & `cg-29.1.0/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/encryption.py` & `cg-29.1.0/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/gene_panel.py` & `cg-29.1.0/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/housekeeper_tags.py` & `cg-29.1.0/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/lims.py` & `cg-29.1.0/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/nextflow.py` & `cg-29.1.0/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/observations.py` & `cg-29.1.0/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/orderforms.py` & `cg-29.1.0/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/priority.py` & `cg-29.1.0/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/report.py` & `cg-29.1.0/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/rnafusion.py` & `cg-29.1.0/cg/constants/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/scout_upload.py` & `cg-29.1.0/cg/constants/scout_upload.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/sequencing.py` & `cg-29.1.0/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/constants/subject.py` & `cg-29.1.0/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/exc.py` & `cg-29.1.0/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/io/api.py` & `cg-29.1.0/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/io/controller.py` & `cg-29.1.0/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/io/csv.py` & `cg-29.1.0/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/io/json.py` & `cg-29.1.0/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/io/yaml.py` & `cg-29.1.0/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/archive/ddn_dataflow.py` & `cg-29.1.0/cg/meta/archive/ddn_dataflow.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/backup/backup.py` & `cg-29.1.0/cg/meta/backup/backup.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
         if not flow_cell:
             LOG.info("No flow cells requested")
             return None
 
         flow_cell.status: FlowCellStatus = FlowCellStatus.PROCESSING
         if not self.dry_run:
-            self.status.commit()
+            self.status.session.commit()
             LOG.info(f"{flow_cell.name}: retrieving from PDC")
 
         try:
             pdc_flow_cell_query: List[str] = self.query_pdc_for_flow_cell(flow_cell.name)
 
         except PdcNoFilesMatchingSearchError as error:
             LOG.error(f"PDC query failed: {error}")
@@ -126,15 +126,15 @@
             self.unlink_files(
                 decrypted_flow_cell, encryption_key, retrieved_flow_cell, retrieved_key
             )
         except subprocess.CalledProcessError as error:
             LOG.error(f"Decryption failed: {error.stderr}")
             if not self.dry_run:
                 flow_cell.status: str = FlowCellStatus.REQUESTED
-                self.status.commit()
+                self.status.session.commit()
             raise error
 
         return get_elapsed_time(start_time=start_time)
 
     def unlink_files(
         self,
         decrypted_flow_cell: Path,
@@ -214,15 +214,15 @@
                     f"WARNING for retrieval of encryption key of flow cell {flow_cell.name}, please check "
                     "dsmerror.log"
                 )
             else:
                 LOG.error(f"{flow_cell.name}: key retrieval failed")
                 if not self.dry_run:
                     flow_cell.status = FlowCellStatus.REQUESTED
-                    self.status.commit()
+                    self.status.session.commit()
                 raise error
 
     def retrieve_archived_flow_cell(
         self, archived_flow_cell: Path, flow_cell: Flowcell, run_dir: Path
     ):
         """Attempt to retrieve an archived flow cell."""
         try:
@@ -239,20 +239,20 @@
                 )
                 if not self.dry_run:
                     self._set_flow_cell_status_to_retrieved(flow_cell)
             else:
                 LOG.error(f"{flow_cell.name}: run directory retrieval failed")
                 if not self.dry_run:
                     flow_cell.status = FlowCellStatus.REQUESTED
-                    self.status.commit()
+                    self.status.session.commit()
                 raise error
 
     def _set_flow_cell_status_to_retrieved(self, flow_cell: Flowcell):
         flow_cell.status = FlowCellStatus.RETRIEVED
-        self.status.commit()
+        self.status.session.commit()
         LOG.info(f"Status for flow cell {flow_cell.name} set to {flow_cell.status}")
 
     def query_pdc_for_flow_cell(self, flow_cell_id) -> List[str]:
         """Query PDC for a given flow cell id."""
         search_patterns: List[str] = [
             dir + ASTERISK + flow_cell_id + ASTERISK for dir in self.encrypt_dir.values()
         ]
```

### Comparing `cg-29.0.3/cg/meta/backup/pdc.py` & `cg-29.1.0/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/clean/api.py` & `cg-29.1.0/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/clean/demultiplexed_flow_cells.py` & `cg-29.1.0/cg/meta/clean/demultiplexed_flow_cells.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         if self.is_correctly_named:
             self.archive_sample_sheet()
         shutil.rmtree(self.path, ignore_errors=True)
         if self.exists_in_statusdb and self.is_correctly_named:
             self.status_db.get_flow_cell_by_name(
                 flow_cell_name=self.id
             ).status = FlowCellStatus.REMOVED
-        self.status_db.commit()
+        self.status_db.session.commit()
 
     def remove_failed_flow_cell(self) -> None:
         """Performs the two removal actions for failed flow cells."""
         self.remove_from_demultiplexed_runs()
         if self.files_exist_in_housekeeper and self.is_correctly_named:
             self.remove_files_from_housekeeper()
```

### Comparing `cg-29.0.3/cg/meta/clean/flow_cell_run_directories.py` & `cg-29.1.0/cg/meta/clean/flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/compress/compress.py` & `cg-29.1.0/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/compress/files.py` & `cg-29.1.0/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/deliver.py` & `cg-29.1.0/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/deliver_ticket.py` & `cg-29.1.0/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/demultiplex/delete_demultiplex_api.py` & `cg-29.1.0/cg/meta/demultiplex/delete_demultiplex_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             )
             return
         if demultiplexing_dir and run_dir and self.status_db_presence:
             flow_cell_obj: Flowcell = self.status_db.get_flow_cell_by_name(
                 flow_cell_name=self.flow_cell_name
             )
             flow_cell_obj.status = "removed"
-            self.status_db.commit()
+            self.status_db.session.commit()
         if demultiplexing_dir and self.demultiplexing_path.exists():
             self._delete_demultiplexing_dir_hasta()
         else:
             log.info(
                 f"DeleteDemuxAPI-Hasta: Skipped demultiplexing directory, or no target: {self.demultiplexing_dir}"
             )
         if run_dir and self.run_path.exists():
```

### Comparing `cg-29.0.3/cg/meta/demultiplex/demux_post_processing.py` & `cg-29.1.0/cg/meta/demultiplex/demux_post_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,17 @@
         """Transfer flow cell and sequencing files."""
         flow_cell: Flowcell = self.transfer_flow_cell_api.transfer(
             flow_cell_dir=flow_cell_dir, flow_cell_id=flow_cell_id, store=store
         )
         if self.dry_run:
             LOG.info("Dry run will not commit flow cell to database")
             return
-        self.status_db.add_commit(flow_cell)
+        self.status_db.session.add(flow_cell)
+        self.status_db.session.commit()
+
         LOG.info(f"Flow cell added: {flow_cell}")
 
 
 class DemuxPostProcessingHiseqXAPI(DemuxPostProcessingAPI):
     """Post demultiplexing API class for Hiseq X flow cell."""
 
     def add_to_cgstats(self, flow_cell_path: Path) -> None:
```

### Comparing `cg-29.0.3/cg/meta/demultiplex/files.py` & `cg-29.1.0/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/encryption/encryption.py` & `cg-29.1.0/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/invoice.py` & `cg-29.1.0/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/meta.py` & `cg-29.1.0/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/observations/balsamic_observations_api.py` & `cg-29.1.0/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/observations/mip_dna_observations_api.py` & `cg-29.1.0/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/observations/observations_api.py` & `cg-29.1.0/cg/meta/observations/observations_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         )
         return bool(loqusdb_case or duplicate or case.loqusdb_uploaded_samples)
 
     def update_statusdb_loqusdb_id(self, samples: List[Family], loqusdb_id: Optional[str]) -> None:
         """Update Loqusdb ID field in StatusDB for each of the provided samples."""
         for sample in samples:
             sample.loqusdb_id = loqusdb_id
-        self.store.commit()
+        self.store.session.commit()
 
     def check_customer_loqusdb_permissions(self, customer: Customer) -> None:
         """Verifies that the customer is whitelisted for Loqusdb uploads."""
         if customer.internal_id not in [cust_id.value for cust_id in self.get_loqusdb_customers()]:
             LOG.error(
                 f"Customer {customer.internal_id} is not whitelisted for Loqusdb uploads. Cancelling upload."
             )
```

### Comparing `cg-29.0.3/cg/meta/orders/api.py` & `cg-29.1.0/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/orders/case_submitter.py` & `cg-29.1.0/cg/meta/orders/case_submitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,15 +285,16 @@
 
                 self._update_relationship(
                     father_obj=sample_father,
                     link_obj=case_sample,
                     mother_obj=sample_mother,
                     sample=sample,
                 )
-            self.status.add_commit(new_cases)
+            self.status.session.add_all(new_cases)
+            self.status.session.commit()
         return new_cases
 
     @staticmethod
     def _update_case_panel(panels: List[str], case: Family) -> None:
         """Update case panels."""
         case.panels = panels
 
@@ -317,15 +318,15 @@
         link_obj = self.status.relate_sample(
             family=case_obj,
             sample=family_samples[sample["name"]],
             status=sample["status"],
             mother=mother_obj,
             father=father_obj,
         )
-        self.status.add(link_obj)
+        self.status.session.add(link_obj)
         return link_obj
 
     def _create_sample(self, case, customer_obj, order, ordered, sample, ticket):
         sample_obj = self.status.add_sample(
             name=sample["name"],
             comment=sample["comment"],
             control=sample["control"],
@@ -345,17 +346,17 @@
         )
         sample_obj.customer = customer_obj
         with self.status.session.no_autoflush:
             application_tag = sample["application"]
             sample_obj.application_version: ApplicationVersion = (
                 self.status.get_current_application_version_by_tag(tag=application_tag)
             )
-        self.status.add(sample_obj)
+        self.status.session.add(sample_obj)
         new_delivery = self.status.add_delivery(destination="caesar", sample=sample_obj)
-        self.status.add(new_delivery)
+        self.status.session.add(new_delivery)
         return sample_obj
 
     def _create_case(self, case: dict, customer_obj: Customer, ticket: str):
         case_obj = self.status.add_case(
             cohorts=case["cohorts"],
             data_analysis=Pipeline(case["data_analysis"]),
             data_delivery=DataDelivery(case["data_delivery"]),
```

### Comparing `cg-29.0.3/cg/meta/orders/fastq_submitter.py` & `cg-29.1.0/cg/meta/orders/fastq_submitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         )
         case.customer: Customer = self.status.get_customer_by_internal_id(
             customer_internal_id=CustomerNames.CG_INTERNAL_CUSTOMER
         )
         relationship: FamilySample = self.status.relate_sample(
             family=case, sample=sample_obj, status=StatusEnum.unknown
         )
-        self.status.add(case, relationship)
+        self.status.session.add_all([case, relationship])
 
     def store_items_in_status(
         self, customer_id: str, order: str, ordered: dt.datetime, ticket_id: str, items: List[dict]
     ) -> List[Sample]:
         """Store fastq samples in the status database including family connection and delivery"""
         customer: Customer = self.status.get_customer_by_internal_id(
             customer_internal_id=customer_id
@@ -129,11 +129,12 @@
                 ):
                     self.create_maf_case(sample_obj=new_sample)
                 case.customer = customer
                 new_relationship = self.status.relate_sample(
                     family=case, sample=new_sample, status=StatusEnum.unknown
                 )
                 new_delivery = self.status.add_delivery(destination="caesar", sample=new_sample)
-                self.status.add(case, new_relationship, new_delivery)
+                self.status.session.add_all([case, new_relationship, new_delivery])
 
-        self.status.add_commit(new_samples)
+        self.status.session.add_all(new_samples)
+        self.status.session.commit()
         return new_samples
```

### Comparing `cg-29.0.3/cg/meta/orders/lims.py` & `cg-29.1.0/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/orders/metagenome_submitter.py` & `cg-29.1.0/cg/meta/orders/metagenome_submitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,16 +123,18 @@
                         data_delivery=DataDelivery(case_dict["data_delivery"]),
                         name=str(ticket_id),
                         panels=None,
                         priority=case_dict["priority"],
                         ticket=ticket_id,
                     )
                     case.customer: Customer = customer
-                    self.status.add(case)
+                    self.status.session.add(case)
+                    self.status.session.commit()
 
                 new_relationship: FamilySample = self.status.relate_sample(
                     family=case, sample=new_sample, status=StatusEnum.unknown
                 )
-                self.status.add(new_relationship)
+                self.status.session.add(new_relationship)
 
-        self.status.add_commit(new_samples)
+        self.status.session.add_all(new_samples)
+        self.status.session.commit()
         return new_samples
```

### Comparing `cg-29.0.3/cg/meta/orders/microbial_submitter.py` & `cg-29.1.0/cg/meta/orders/microbial_submitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -95,15 +95,16 @@
                         data_analysis=data_analysis,
                         data_delivery=data_delivery,
                         name=ticket_id,
                         panels=None,
                         ticket=ticket_id,
                     )
                     case.customer: Customer = customer
-                    self.status.add_commit(case)
+                    self.status.session.add(case)
+                    self.status.session.commit()
 
                 application_tag: str = sample_data["application"]
                 application_version: ApplicationVersion = (
                     self.status.get_current_application_version_by_tag(tag=application_tag)
                 )
                 organism: Organism = self.status.get_organism_by_internal_id(
                     sample_data["organism_id"]
@@ -111,15 +112,16 @@
 
                 if not organism:
                     organism: Organism = self.status.add_organism(
                         internal_id=sample_data["organism_id"],
                         name=sample_data["organism_id"],
                         reference_genome=sample_data["reference_genome"],
                     )
-                    self.status.add_commit(organism)
+                    self.status.session.add(organism)
+                    self.status.session.commit()
 
                 if comment:
                     case.comment: str = f"Order comment: {comment}"
 
                 new_sample = self.status.add_sample(
                     name=sample_data["name"],
                     sex="unknown",
@@ -138,15 +140,16 @@
 
                 priority = new_sample.priority
                 sample_objs.append(new_sample)
                 self.status.relate_sample(family=case, sample=new_sample, status="unknown")
                 new_samples.append(new_sample)
 
             case.priority = priority
-            self.status.add_commit(new_samples)
+            self.status.session.add_all(new_samples)
+            self.status.session.commit()
         return sample_objs
 
     def _fill_in_sample_verified_organism(self, samples: List[MicrobialSample]):
         for sample in samples:
             organism_id = sample.organism
             reference_genome = sample.reference_genome
             organism: Organism = self.status.get_organism_by_internal_id(internal_id=organism_id)
```

### Comparing `cg-29.0.3/cg/meta/orders/pool_submitter.py` & `cg-29.1.0/cg/meta/orders/pool_submitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                     data_delivery=data_delivery,
                     name=case_name,
                     panels=None,
                     priority=priority,
                     ticket=ticket_id,
                 )
                 case.customer = customer
-                self.status.add_commit(case)
+                self.status.session.add(case)
 
             new_pool: Pool = self.status.add_pool(
                 application_version=application_version,
                 customer=customer,
                 name=pool["name"],
                 order=order,
                 ordered=ordered,
@@ -161,18 +161,18 @@
                     application_version=application_version,
                     customer=customer,
                     no_invoice=True,
                 )
                 new_samples.append(new_sample)
                 self.status.relate_sample(family=case, sample=new_sample, status="unknown")
             new_delivery = self.status.add_delivery(destination="caesar", pool=new_pool)
-            self.status.add(new_delivery)
+            self.status.session.add(new_delivery)
             new_pools.append(new_pool)
-        self.status.add_commit(new_pools)
-
+        self.status.session.add_all(new_pools)
+        self.status.session.commit()
         return new_pools
 
     def _validate_case_names_are_available(
         self, customer_id: str, samples: List[RmlSample], ticket: str
     ):
         """Validate names of all samples are not already in use."""
         customer: Customer = self.status.get_customer_by_internal_id(
```

### Comparing `cg-29.0.3/cg/meta/orders/sars_cov_2_submitter.py` & `cg-29.1.0/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/orders/submitter.py` & `cg-29.1.0/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/orders/ticket_handler.py` & `cg-29.1.0/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/report/balsamic.py` & `cg-29.1.0/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/report/balsamic_umi.py` & `cg-29.1.0/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/report/field_validators.py` & `cg-29.1.0/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/report/mip_dna.py` & `cg-29.1.0/cg/meta/report/mip_dna.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from typing import List, Optional, Iterable
 
 from cgmodels.cg.constants import Pipeline
 from housekeeper.store.models import Version, File
-from sqlalchemy.orm import Query
 
 from cg.constants import (
     REQUIRED_REPORT_FIELDS,
     REQUIRED_CUSTOMER_FIELDS,
     REQUIRED_CASE_FIELDS,
     REQUIRED_APPLICATION_FIELDS,
     REQUIRED_DATA_ANALYSIS_MIP_DNA_FIELDS,
```

### Comparing `cg-29.0.3/cg/meta/report/report_api.py` & `cg-29.1.0/cg/meta/report/report_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from datetime import datetime
 import logging
 from pathlib import Path
 from typing import TextIO, Optional, List
 
 import requests
-from alchy import Query
+from sqlalchemy.orm import Query
 
 from cgmodels.cg.constants import Pipeline
 from housekeeper.store.models import File, Version
 
 from cg.constants.constants import FileFormat, MAX_ITEMS_TO_RETRIEVE
 from cg.exc import DeliveryReportError
 from cg.io.controller import WriteStream
@@ -159,15 +159,15 @@
     def update_delivery_report_date(self, case: Family, analysis_date: datetime) -> None:
         """Updates the date when delivery report was created."""
 
         analysis: Analysis = self.status_db.get_analysis_by_case_entry_id_and_started_at(
             case_entry_id=case.id, started_at_date=analysis_date
         )
         analysis.delivery_report_created_at = datetime.now()
-        self.status_db.commit()
+        self.status_db.session.commit()
 
     def get_report_data(self, case_id: str, analysis_date: datetime) -> ReportModel:
         """Fetches all the data needed to generate a delivery report."""
 
         case: Family = self.status_db.get_case_by_internal_id(internal_id=case_id)
         analysis: Analysis = self.status_db.get_analysis_by_case_entry_id_and_started_at(
             case_entry_id=case.id, started_at_date=analysis_date
```

### Comparing `cg-29.0.3/cg/meta/report/templates/balsamic_report.html` & `cg-29.1.0/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/report/templates/bootstrap.html` & `cg-29.1.0/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/report/templates/mip-dna_report.html` & `cg-29.1.0/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/rsync/rsync_api.py` & `cg-29.1.0/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/tar/tar.py` & `cg-29.1.0/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/transfer/external_data.py` & `cg-29.1.0/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/transfer/flowcell.py` & `cg-29.1.0/cg/meta/transfer/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/transfer/lims.py` & `cg-29.1.0/cg/meta/transfer/lims.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
                 LOG.info(
                     f"Found new {status_type.value} date for {sample_obj.internal_id}: "
                     f"{lims_date}, old value: {statusdb_date} "
                 )
 
                 setattr(sample_obj, f"{status_type.value}_at", lims_date)
-                self.status.commit()
+                self.status.session.commit()
             else:
                 LOG.debug(f"no {status_type.value} date found for {sample_obj.internal_id}")
 
     def _get_samples_to_include(self, include, status_type):
         samples = None
         if include == IncludeOptions.UNSET.value:
             samples = self._get_samples_in_step(status_type)
@@ -127,15 +127,15 @@
                 LOG.info(
                     "Found %s date for pool id %s: %s",
                     status_type.value,
                     pool_obj.id,
                     status_date,
                 )
                 setattr(pool_obj, f"{status_type.value}_at", status_date)
-                self.status.commit()
+                self.status.session.commit()
                 break
 
     def _get_samples_in_step(self, status_type) -> List[Sample]:
         return self._sample_functions[status_type]()
 
     @staticmethod
     def _is_pool_valid(pool_obj: Pool, ticket: str, number_of_samples: int) -> bool:
```

### Comparing `cg-29.0.3/cg/meta/upload/balsamic/balsamic.py` & `cg-29.1.0/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/coverage.py` & `cg-29.1.0/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/fohm/fohm.py` & `cg-29.1.0/cg/meta/upload/fohm/fohm.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,16 +278,16 @@
 
     def update_upload_started_at(self, case_id: str) -> None:
         """Update timestamp for cases which started being processed as batch"""
         if self._dry_run:
             return
         case_obj: Family = self.status_db.get_case_by_internal_id(internal_id=case_id)
         case_obj.analyses[0].upload_started_at = dt.datetime.now()
-        self.status_db.commit()
+        self.status_db.session.commit()
 
     def update_uploaded_at(self, case_id: str) -> None:
         """Update timestamp for cases which uploaded successfully"""
         if self._dry_run:
             return
         case_obj: Family = self.status_db.get_case_by_internal_id(internal_id=case_id)
         case_obj.analyses[0].uploaded_at = dt.datetime.now()
-        self.status_db.commit()
+        self.status_db.session.commit()
```

### Comparing `cg-29.0.3/cg/meta/upload/gisaid/constants.py` & `cg-29.1.0/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/gisaid/gisaid.py` & `cg-29.1.0/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/gisaid/models.py` & `cg-29.1.0/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/gt.py` & `cg-29.1.0/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/mip/mip_dna.py` & `cg-29.1.0/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/mip/mip_rna.py` & `cg-29.1.0/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/mutacc.py` & `cg-29.1.0/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/nipt/nipt.py` & `cg-29.1.0/cg/meta/upload/nipt/nipt.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,30 +120,30 @@
         """Updates analysis_uploaded_at for the uploaded analysis"""
 
         case_obj: Family = self.status_db.get_case_by_internal_id(internal_id=case_id)
         analysis_obj: Analysis = case_obj.analyses[0]
 
         if not self.dry_run:
             analysis_obj.uploaded_at = dt.datetime.now()
-            self.status_db.commit()
+            self.status_db.session.commit()
             self.trailblazer_api.set_analysis_uploaded(
                 case_id=case_id, uploaded_at=analysis_obj.uploaded_at
             )
 
         return analysis_obj
 
     def update_analysis_upload_started_date(self, case_id: str) -> Analysis:
         """Updates analysis_upload_started_at for the uploaded analysis"""
 
         case_obj: Family = self.status_db.get_case_by_internal_id(internal_id=case_id)
         analysis_obj: Analysis = case_obj.analyses[0]
 
         if not self.dry_run:
             analysis_obj.upload_started_at = dt.datetime.now()
-            self.status_db.commit()
+            self.status_db.session.commit()
 
         return analysis_obj
 
     def get_statina_files(self, case_id: str) -> StatinaUploadFiles:
         """Get statina files from housekeeper."""
 
         hk_results_file: str = self.get_housekeeper_results_file(
```

### Comparing `cg-29.0.3/cg/meta/upload/rnafusion/rnafusion.py` & `cg-29.1.0/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-29.1.0/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-29.1.0/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/scout/hk_tags.py` & `cg-29.1.0/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/scout/mip_config_builder.py` & `cg-29.1.0/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-29.1.0/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/scout/scout_config_builder.py` & `cg-29.1.0/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/scout/uploadscoutapi.py` & `cg-29.1.0/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/upload/upload_api.py` & `cg-29.1.0/cg/meta/upload/upload_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,22 +35,22 @@
 
         raise NotImplementedError
 
     def update_upload_started_at(self, analysis: Analysis) -> None:
         """Updates the upload_started_at field with the current local date and time"""
 
         analysis.upload_started_at = datetime.now()
-        self.status_db.commit()
+        self.status_db.session.commit()
 
     def update_uploaded_at(self, analysis: Analysis) -> None:
         """Updates the uploaded_at field with the current local date and time"""
 
         analysis.uploaded_at: datetime = datetime.now()
 
-        self.status_db.commit()
+        self.status_db.session.commit()
         self.trailblazer_api.set_analysis_uploaded(
             case_id=analysis.family.internal_id, uploaded_at=analysis.uploaded_at
         )
 
     @staticmethod
     def verify_analysis_upload(case_obj: Family, restart: bool) -> None:
         """Verifies the state of an analysis upload in StatusDB"""
```

### Comparing `cg-29.0.3/cg/meta/upload/vogue.py` & `cg-29.1.0/cg/meta/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/analysis.py` & `cg-29.1.0/cg/meta/workflow/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,16 @@
             completed_at=dt.datetime.now(),
             primary=(len(case_obj.analyses) == 0),
         )
         new_analysis.family = case_obj
         if dry_run:
             LOG.info("Dry-run: StatusDB changes will not be commited")
             return
-        self.status_db.add_commit(new_analysis)
+        self.status_db.session.add(new_analysis)
+        self.status_db.session.commit()
         LOG.info(f"Analysis successfully stored in StatusDB: {case_id} : {analysis_start}")
 
     def get_deliverables_file_path(self, case_id: str) -> Path:
         raise NotImplementedError
 
     def get_analysis_finish_path(self, case_id: str) -> Path:
         raise NotImplementedError
@@ -245,15 +246,15 @@
         """
         if dry_run:
             LOG.info(f"Dry-run: Action {action} would be set for case {case_id}")
             return
         if action in [None, *CASE_ACTIONS]:
             case_obj: Family = self.status_db.get_case_by_internal_id(internal_id=case_id)
             case_obj.action = action
-            self.status_db.commit()
+            self.status_db.session.commit()
             LOG.info("Action %s set for case %s", action, case_id)
             return
         LOG.warning(
             f"Action '{action}' not permitted by StatusDB and will not be set for case {case_id}"
         )
 
     def get_analyses_to_clean(self, before: dt.datetime) -> List[Analysis]:
@@ -451,15 +452,15 @@
 
     def clean_analyses(self, case_id: str) -> None:
         """Add a cleaned at date for all analyses related to a case."""
         analyses: list = self.status_db.get_case_by_internal_id(internal_id=case_id).analyses
         LOG.info(f"Adding a cleaned at date for case {case_id}")
         for analysis_obj in analyses:
             analysis_obj.cleaned_at = analysis_obj.cleaned_at or dt.datetime.now()
-            self.status_db.commit()
+            self.status_db.session.commit()
 
     def clean_run_dir(self, case_id: str, yes: bool, case_path: Union[List[Path], Path]) -> int:
         """Remove workflow run directory."""
 
         try:
             self.verify_case_path_exists(case_id=case_id)
         except FileNotFoundError:
```

### Comparing `cg-29.0.3/cg/meta/workflow/balsamic.py` & `cg-29.1.0/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/balsamic_pon.py` & `cg-29.1.0/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/balsamic_qc.py` & `cg-29.1.0/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/balsamic_umi.py` & `cg-29.1.0/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/fastq.py` & `cg-29.1.0/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/fluffy.py` & `cg-29.1.0/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/microsalt.py` & `cg-29.1.0/cg/meta/workflow/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/mip.py` & `cg-29.1.0/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/mip_dna.py` & `cg-29.1.0/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/mip_rna.py` & `cg-29.1.0/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/mutant.py` & `cg-29.1.0/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/nextflow_common.py` & `cg-29.1.0/cg/meta/workflow/nextflow_common.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/prepare_fastq.py` & `cg-29.1.0/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/rnafusion.py` & `cg-29.1.0/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/meta/workflow/tower_common.py` & `cg-29.1.0/cg/meta/workflow/tower_common.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/balsamic/config.py` & `cg-29.1.0/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/balsamic/metrics.py` & `cg-29.1.0/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/cg_config.py` & `cg-29.1.0/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/cgstats/stats_sample.py` & `cg-29.1.0/cg/models/cgstats/stats_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/compression_data.py` & `cg-29.1.0/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/deliverables/metric_deliverables.py` & `cg-29.1.0/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/demultiplex/demux_results.py` & `cg-29.1.0/cg/models/demultiplex/demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/demultiplex/flow_cell.py` & `cg-29.1.0/cg/models/demultiplex/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/demultiplex/run_parameters.py` & `cg-29.1.0/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/demultiplex/sbatch.py` & `cg-29.1.0/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/file_data.py` & `cg-29.1.0/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/invoice/invoice.py` & `cg-29.1.0/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/lims/sample.py` & `cg-29.1.0/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/mip/mip_config.py` & `cg-29.1.0/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/mip/mip_metrics_deliverables.py` & `cg-29.1.0/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/mip/mip_sample_info.py` & `cg-29.1.0/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/nextflow/deliverables.py` & `cg-29.1.0/cg/models/nextflow/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/nextflow/sample.py` & `cg-29.1.0/cg/models/nextflow/sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/observations/input_files.py` & `cg-29.1.0/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/orders/constants.py` & `cg-29.1.0/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/orders/excel_sample.py` & `cg-29.1.0/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/orders/json_sample.py` & `cg-29.1.0/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/orders/order.py` & `cg-29.1.0/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/orders/orderform_schema.py` & `cg-29.1.0/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/orders/sample_base.py` & `cg-29.1.0/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/orders/samples.py` & `cg-29.1.0/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/report/metadata.py` & `cg-29.1.0/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/report/report.py` & `cg-29.1.0/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/report/sample.py` & `cg-29.1.0/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/report/validators.py` & `cg-29.1.0/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/rnafusion/rnafusion_sample.py` & `cg-29.1.0/cg/models/rnafusion/rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/scout/scout_load_config.py` & `cg-29.1.0/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/slurm/sbatch.py` & `cg-29.1.0/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/models/workflow/mutant.py` & `cg-29.1.0/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/resources/20181012_Indices.csv` & `cg-29.1.0/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/resources/rnafusion_bundle_filenames.csv` & `cg-29.1.0/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/server/admin.py` & `cg-29.1.0/cg/server/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from cgmodels.cg.constants import Pipeline
 from flask import redirect, request, session, url_for, flash
 from flask_admin.actions import action
 from flask_admin.contrib.sqla import ModelView
 from flask_dance.contrib.google import google
 from markupsafe import Markup
-from sqlalchemy.orm import Query
 
 from cg.constants.constants import DataDelivery, CaseActions
 from cg.server.ext import db
 from cg.store.models import Family, Sample
 from cg.utils.flask.enum import SelectEnumField
 
 
@@ -265,15 +264,15 @@
     def set_action_for_cases(self, action: Union[CaseActions, None], case_entry_ids: List[str]):
         try:
             for entry_id in case_entry_ids:
                 family = self.get_case_by_entry_id(entry_id=entry_id)
                 if family:
                     family.action = action
 
-            db.commit()
+            db.session.commit()
 
             num_families = len(case_entry_ids)
             action_message = (
                 f"Families were set to {action}."
                 if num_families == 1
                 else f"{num_families} families were set to {action}."
             )
```

### Comparing `cg-29.0.3/cg/server/api.py` & `cg-29.1.0/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/server/app.py` & `cg-29.1.0/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/server/config.py` & `cg-29.1.0/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/server/ext.py` & `cg-29.1.0/cg/server/ext.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from flask_admin import Admin
-from flask_alchy import Alchy
+from sqlalchemy.orm import scoped_session, sessionmaker
 from flask_cors import CORS
 from flask_wtf.csrf import CSRFProtect
 
 from cg.apps.lims import LimsAPI
 from cg.apps.osticket import OsTicket
-from cg.store import api, models
-
-
-class CgAlchy(Alchy, api.CoreHandler):
-    pass
+from cg.store.api.core import Store
 
 
 class FlaskLims(LimsAPI):
     def __init__(self, app=None):
         if app:
             self.init_app(app)
 
@@ -24,13 +20,24 @@
                 "username": app.config["LIMS_USERNAME"],
                 "password": app.config["LIMS_PASSWORD"],
             }
         }
         super(FlaskLims, self).__init__(config)
 
 
+class FlaskStore(Store):
+    def __init__(self, app=None):
+        if app:
+            self.init_app(app)
+
+    def init_app(self, app):
+        uri = app.config["SQLALCHEMY_DATABASE_URI"]
+        super(FlaskStore, self).__init__(uri)
+
+
 cors = CORS(resources={r"/api/*": {"origins": "*"}}, supports_credentials=True)
 csrf = CSRFProtect()
-db = CgAlchy(Model=models.Model)
+db = FlaskStore()
+
 admin = Admin(name="Clinical Genomics")
 lims = FlaskLims()
 osticket = OsTicket()
```

### Comparing `cg-29.0.3/cg/server/invoices/templates/invoices/index.html` & `cg-29.1.0/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/server/invoices/templates/invoices/invoice.html` & `cg-29.1.0/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/server/invoices/templates/invoices/layout.html` & `cg-29.1.0/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/server/invoices/templates/invoices/new.html` & `cg-29.1.0/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/server/invoices/views.py` & `cg-29.1.0/cg/server/invoices/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 def undo_invoice(invoice_id):
     invoice_obj: Invoice = db.get_invoice_by_entry_id(entry_id=invoice_id)
     record_type: str = invoice_obj.record_type
     records: List[Union[Pool, Sample]] = db.get_pools_and_samples_for_invoice_by_invoice_id(
         invoice_id=invoice_id
     )
-    invoice_obj.delete()
+    db.session.delete(invoice_obj)
     for record in records:
         record.invoice_id = None
     db.session.commit()
 
     return url_for(".new", record_type=record_type)
 
 
@@ -76,15 +76,16 @@
             customer=customer,
             samples=samples,
             comment=request.form.get("comment"),
             discount=int(request.form.get("discount", "0")),
             record_type="Sample",
         )
 
-    db.add_commit(new_invoice)
+    db.session.add(new_invoice)
+    db.session.commit()
     return url_for(".invoice", invoice_id=new_invoice.id)
 
 
 def upload_invoice_news_to_db():
     invoice_id: int = request.form.get("invoice_id")
     invoice_obj: Invoice = db.get_invoice_by_entry_id(entry_id=invoice_id)
     invoice_obj.comment = request.form.get("comment")
@@ -99,15 +100,15 @@
 
     kth_excel_file = request.files.get("KTH_excel")
     if kth_excel_file:
         invoice_obj.excel_kth = kth_excel_file.stream.read()
     ki_excel_file = request.files.get("KI_excel")
     if ki_excel_file:
         invoice_obj.excel_ki = ki_excel_file.stream.read()
-    db.commit()
+    db.session.commit()
     return url_for("invoices.invoice", invoice_id=invoice_id)
 
 
 @BLUEPRINT.route("/")
 def index():
     """Retrieve invoices."""
     invoices = {
```

### Comparing `cg-29.0.3/cg/store/api/add.py` & `cg-29.1.0/cg/store/api/add.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from cg.constants import DataDelivery, Pipeline, FlowCellStatus
 from cg.store.api.base import BaseHandler
 
 from cg.constants import Priority
 from cg.store.models import (
     Flowcell,
+    Invoice,
     Organism,
     Customer,
     Sample,
     Pool,
     Delivery,
     ApplicationVersion,
     Panel,
@@ -47,32 +48,32 @@
         invoice_reference: str,
         scout_access: bool = False,
         *args,
         **kwargs,
     ) -> Customer:
         """Build a new customer record."""
 
-        return self.Customer(
+        return Customer(
             internal_id=internal_id,
             name=name,
             scout_access=scout_access,
             invoice_address=invoice_address,
             invoice_reference=invoice_reference,
             **kwargs,
         )
 
     def add_collaboration(self, internal_id: str, name: str, **kwargs) -> Collaboration:
         """Build a new customer group record."""
 
-        return self.Collaboration(internal_id=internal_id, name=name, **kwargs)
+        return Collaboration(internal_id=internal_id, name=name, **kwargs)
 
     def add_user(self, customer: Customer, email: str, name: str, is_admin: bool = False) -> User:
         """Build a new user record."""
 
-        new_user = self.User(name=name, email=email, is_admin=is_admin)
+        new_user = User(name=name, email=email, is_admin=is_admin)
         new_user.customers.append(customer)
         return new_user
 
     def add_application(
         self,
         tag: str,
         prep_category: str,
@@ -81,15 +82,15 @@
         percent_reads_guaranteed: int,
         is_accredited: bool = False,
         min_sequencing_depth: int = 0,
         **kwargs,
     ) -> Application:
         """Build a new application record."""
 
-        return self.Application(
+        return Application(
             tag=tag,
             prep_category=prep_category,
             description=description,
             is_accredited=is_accredited,
             min_sequencing_depth=min_sequencing_depth,
             percent_kth=percent_kth,
             percent_reads_guaranteed=percent_reads_guaranteed,
@@ -102,32 +103,32 @@
         version: int,
         valid_from: dt.datetime,
         prices: dict,
         **kwargs,
     ) -> ApplicationVersion:
         """Build a new application version record."""
 
-        new_record = self.ApplicationVersion(version=version, valid_from=valid_from, **kwargs)
+        new_record = ApplicationVersion(version=version, valid_from=valid_from, **kwargs)
         for price_key in [
             Priority.standard.name,
             Priority.priority.name,
             Priority.express.name,
             Priority.research.name,
         ]:
             setattr(new_record, f"price_{price_key}", prices[price_key])
         new_record.application = application
         return new_record
 
     def add_bed(self, name: str) -> Bed:
         """Build a new bed record."""
-        return self.Bed(name=name)
+        return Bed(name=name)
 
     def add_bed_version(self, bed: Bed, version: int, filename: str, shortname: str) -> BedVersion:
         """Build a new bed version record."""
-        bed_version: BedVersion = self.BedVersion(
+        bed_version: BedVersion = BedVersion(
             version=version, filename=filename, shortname=shortname
         )
         bed_version.bed = bed
         return bed_version
 
     def add_sample(
         self,
@@ -145,15 +146,15 @@
         tumour: bool = False,
         **kwargs,
     ) -> Sample:
         """Build a new Sample record."""
 
         internal_id = internal_id or self.generate_unique_petname()
         priority = priority or (Priority.research if downsampled_to else Priority.standard)
-        return self.Sample(
+        return Sample(
             comment=comment,
             control=control,
             downsampled_to=downsampled_to,
             internal_id=internal_id,
             is_tumour=tumour,
             name=name,
             order=order,
@@ -182,15 +183,15 @@
         while True:
             internal_id = petname.Generate(2, separator="")
             if self.get_case_by_internal_id(internal_id) is None:
                 break
             else:
                 LOG.debug(f"{internal_id} already used - trying another id")
 
-        return self.Family(
+        return Family(
             cohorts=cohorts,
             data_analysis=str(data_analysis),
             data_delivery=str(data_delivery),
             internal_id=internal_id,
             name=name,
             panels=panels,
             priority=priority,
@@ -204,15 +205,15 @@
         sample: Sample,
         status: str,
         mother: Sample = None,
         father: Sample = None,
     ) -> FamilySample:
         """Relate a sample record to a family record."""
 
-        new_record = self.FamilySample(status=status)
+        new_record: FamilySample = FamilySample(status=status)
         new_record.family = family
         new_record.sample = sample
         new_record.mother = mother
         new_record.father = father
         return new_record
 
     def add_flow_cell(
@@ -220,15 +221,15 @@
         flow_cell_name: str,
         sequencer_name: str,
         sequencer_type: str,
         date: dt.datetime,
         flow_cell_status: Optional[str] = FlowCellStatus.ON_DISK,
     ) -> Flowcell:
         """Build a new Flowcell record."""
-        return self.Flowcell(
+        return Flowcell(
             name=flow_cell_name,
             sequencer_name=sequencer_name,
             sequencer_type=sequencer_type,
             sequenced_at=date,
             status=flow_cell_status,
         )
 
@@ -239,15 +240,15 @@
         completed_at: dt.datetime = None,
         primary: bool = False,
         uploaded: dt.datetime = None,
         started_at: dt.datetime = None,
         **kwargs,
     ) -> Analysis:
         """Build a new Analysis record."""
-        return self.Analysis(
+        return Analysis(
             pipeline=str(pipeline),
             pipeline_version=version,
             completed_at=completed_at,
             is_primary=primary,
             uploaded_at=uploaded,
             started_at=started_at,
             **kwargs,
@@ -260,15 +261,15 @@
         abbrev: str,
         version: float,
         date: dt.datetime = None,
         genes: int = None,
     ) -> Panel:
         """Build a new panel record."""
 
-        new_record = self.Panel(
+        new_record: Panel = Panel(
             name=name, abbrev=abbrev, current_version=version, date=date, gene_count=genes
         )
         new_record.customer = customer
         return new_record
 
     def add_pool(
         self,
@@ -276,29 +277,27 @@
         name: str,
         order: str,
         ordered: dt.datetime,
         application_version: ApplicationVersion,
         ticket: str = None,
         comment: str = None,
         received_at: dt.datetime = None,
-        capture_kit: str = None,
         invoice_id: int = None,
         no_invoice: bool = None,
         delivered_at: dt.datetime = None,
     ) -> Pool:
         """Build a new Pool record."""
 
-        new_record = self.Pool(
+        new_record: Pool = Pool(
             name=name,
             ordered_at=ordered or dt.datetime.now(),
             order=order,
             ticket=ticket,
             received_at=received_at,
             comment=comment,
-            capture_kit=capture_kit,
             delivered_at=delivered_at,
             invoice_id=invoice_id,
             no_invoice=no_invoice,
         )
         new_record.customer = customer
         new_record.application_version = application_version
         return new_record
@@ -310,15 +309,15 @@
         pool: Pool = None,
         comment: str = None,
     ) -> Delivery:
         """Build a new Delivery record."""
 
         if not any([sample, pool]):
             raise ValueError("you have to provide a sample or a pool")
-        new_record = self.Delivery(destination=destination, comment=comment)
+        new_record: Delivery = Delivery(destination=destination, comment=comment)
         new_record.sample = sample
         new_record.pool = pool
         return new_record
 
     def add_invoice(
         self,
         customer: Customer,
@@ -329,15 +328,15 @@
         discount: int = 0,
         record_type: str = None,
         invoiced_at: Optional[dt.datetime] = None,
     ):
         """Build a new Invoice record."""
 
         new_id = self.new_invoice_id()
-        new_invoice = self.Invoice(
+        new_invoice: Invoice = Invoice(
             comment=comment,
             discount=discount,
             id=new_id,
             record_type=record_type,
             invoiced_at=invoiced_at,
         )
         new_invoice.customer = customer
@@ -354,14 +353,14 @@
         internal_id: str,
         name: str,
         reference_genome: str = None,
         verified: bool = False,
         **kwargs,
     ) -> Organism:
         """Build a new Organism record."""
-        return self.Organism(
+        return Organism(
             internal_id=internal_id,
             name=name,
             reference_genome=reference_genome,
             verified=verified,
             **kwargs,
         )
```

### Comparing `cg-29.0.3/cg/store/api/base.py` & `cg-29.1.0/cg/store/api/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """All models aggregated in a base class"""
-import datetime
 from typing import Callable, Optional, Type, List
 
-from alchy import Query, ModelBase
+from sqlalchemy.orm import Query, Session
+from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import and_, func
 from dataclasses import dataclass
 from cg.store.filters.status_case_filters import CaseFilter, apply_case_filter
 from cg.store.filters.status_customer_filters import CustomerFilter, apply_customer_filter
 from cg.store.filters.status_sample_filters import SampleFilter, apply_sample_filter
 from cg.store.models import (
     Analysis,
@@ -26,19 +26,24 @@
     Pool,
     Sample,
     User,
 )
 from cg.store.filters.status_analysis_filters import AnalysisFilter, apply_analysis_filter
 from cg.utils.date import get_date_days_ago
 
+from cg.store.models import Model as ModelBase
+
 
 @dataclass
 class BaseHandler:
     """All models in one base class."""
 
+    def __init__(self, session: Session):
+        self.session = session
+
     Analysis: Type[ModelBase] = Analysis
     Application: Type[ModelBase] = Application
     ApplicationVersion: Type[ModelBase] = ApplicationVersion
     Bed: Type[ModelBase] = Bed
     BedVersion: Type[ModelBase] = BedVersion
     Collaboration: Type[ModelBase] = Collaboration
     Customer: Type[ModelBase] = Customer
@@ -49,18 +54,17 @@
     Invoice: Type[ModelBase] = Invoice
     Organism: Type[ModelBase] = Organism
     Panel: Type[ModelBase] = Panel
     Pool: Type[ModelBase] = Pool
     Sample: Type[ModelBase] = Sample
     User: Type[ModelBase] = User
 
-    @staticmethod
-    def _get_query(table: Type[ModelBase]) -> Query:
+    def _get_query(self, table: Type[ModelBase]) -> Query:
         """Return a query for the given table."""
-        return table.query
+        return self.session.query(table)
 
     def _get_outer_join_cases_with_analyses_query(self) -> Query:
         """Return a query for all cases in the database with an analysis."""
         return (
             self._get_query(table=Family)
             .outerjoin(Analysis)
             .join(
```

### Comparing `cg-29.0.3/cg/store/api/core.py` & `cg-29.1.0/cg/store/api/core.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
-
-import alchy
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker
 
 from cg.store.models import Model
 from cg.store.api.delete import DeleteDataHandler
 from cg.store.api.find_business_data import FindBusinessDataHandler
 
 from .add import AddHandler
 from .find_basic_data import FindBasicDataHandler
@@ -18,16 +18,31 @@
     DeleteDataHandler,
     FindBasicDataHandler,
     FindBusinessDataHandler,
     StatusHandler,
 ):
     """Aggregating class for the store api handlers."""
 
-    pass
+    def __init__(self, session):
+        DeleteDataHandler.__init__(self, session)
+        FindBasicDataHandler.__init__(self, session)
+        FindBusinessDataHandler.__init__(self, session)
+        StatusHandler.__init__(self, session)
 
 
-class Store(alchy.Manager, CoreHandler):
+class Store(CoreHandler):
     uri: str = ""
 
     def __init__(self, uri):
         self.uri = uri
-        super(Store, self).__init__(config=dict(SQLALCHEMY_DATABASE_URI=uri), Model=Model)
+        self.engine = create_engine(uri)
+        session_factory = sessionmaker(bind=self.engine)
+        self.session = session_factory()
+        super(Store, self).__init__(self.session)
+
+    def create_all(self):
+        """Create all tables in the database."""
+        Model.metadata.create_all(bind=self.session.get_bind())
+
+    def drop_all(self):
+        """Drop all tables in the database."""
+        Model.metadata.drop_all(bind=self.session.get_bind())
```

### Comparing `cg-29.0.3/cg/store/api/delete.py` & `cg-29.1.0/cg/store/api/delete.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 """Handler to delete data objects"""
 
 from typing import List
 
 from cg.store.filters.status_flow_cell_filters import apply_flow_cell_filter, FlowCellFilter
 from cg.store.models import Flowcell, Family, Sample
 from cg.store.api.base import BaseHandler
+from sqlalchemy.orm import Session
 
 
 class DeleteDataHandler(BaseHandler):
     """Contains methods to delete business data model instances"""
 
+    def __init__(self, session: Session):
+        super().__init__(session=session)
+        self.session = session
+
     def delete_flow_cell(self, flow_cell_id: str) -> None:
         """Delete flow cell."""
         flow_cell: Flowcell = apply_flow_cell_filter(
             flow_cells=self._get_query(table=Flowcell),
             flow_cell_name=flow_cell_id,
             filter_functions=[FlowCellFilter.GET_BY_NAME],
         ).first()
 
         if flow_cell:
-            flow_cell.delete()
-            flow_cell.flush()
-            self.commit()
+            self.session.delete(flow_cell)
+            self.session.commit()
 
     def delete_relationships_sample(self, sample: Sample) -> None:
         """Delete relationships between all cases and the provided sample."""
         if sample and sample.links:
             for case_sample in sample.links:
-                case_sample.delete()
-            self.commit()
+                self.session.delete(case_sample)
+            self.session.commit()
 
     def delete_cases_without_samples(self, case_internal_ids: List[str]) -> None:
         """Delete any cases specified in case_ids without samples."""
         for case_internal_id in case_internal_ids:
             case: Family = self.get_case_by_internal_id(internal_id=case_internal_id)
             if case and not case.links:
-                case.delete()
-        self.commit()
+                self.session.delete(case)
+        self.session.commit()
```

### Comparing `cg-29.0.3/cg/store/api/find_basic_data.py` & `cg-29.1.0/cg/store/api/find_basic_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Handler to find basic data objects"""
 import datetime as dt
 from typing import List, Optional
 
-from sqlalchemy.orm import Query
+from sqlalchemy.orm import Query, Session
 
 from cg.store.models import (
     Application,
     ApplicationVersion,
     Bed,
     BedVersion,
     Customer,
@@ -32,14 +32,17 @@
 from cg.store.filters.status_panel_filters import PanelFilter, apply_panel_filter
 from cg.store.filters.status_user_filters import apply_user_filter, UserFilter
 
 
 class FindBasicDataHandler(BaseHandler):
     """Contains methods to find basic data model instances."""
 
+    def __init__(self, session: Session):
+        super().__init__(session=session)
+
     def get_application_by_tag(self, tag: str) -> Application:
         """Return an application by tag."""
         return apply_application_filter(
             applications=self._get_query(table=Application),
             filter_functions=[ApplicationFilter.FILTER_BY_TAG],
             tag=tag,
         ).first()
```

### Comparing `cg-29.0.3/cg/store/api/find_business_data.py` & `cg-29.1.0/cg/store/api/find_business_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Handler to find business data objects."""
 import datetime as dt
 import logging
 from typing import Callable, List, Optional, Iterator, Union, Dict
 
-from sqlalchemy import and_, func
-from sqlalchemy.orm import Query
+from sqlalchemy.orm import Query, Session
 
 from cg.constants import FlowCellStatus, Pipeline
 from cg.constants.constants import PrepCategory, SampleType
 from cg.constants.indexes import ListIndexes
 from cg.exc import CaseNotFoundError
 from cg.store.api.base import BaseHandler
 from cg.store.filters.status_application_version_filters import (
@@ -43,14 +42,17 @@
 
 LOG = logging.getLogger(__name__)
 
 
 class FindBusinessDataHandler(BaseHandler):
     """Contains methods to find business data model instances"""
 
+    def __init__(self, session: Session):
+        super().__init__(session=session)
+
     def get_analyses_by_case_entry_id(self, case_entry_id: int) -> List[Analysis]:
         """Return analysis by case entry id."""
         return apply_analysis_filter(
             analyses=self._get_query(Analysis),
             case_entry_id=case_entry_id,
             filter_functions=[AnalysisFilter.FILTER_BY_CASE_ENTRY_ID],
         ).all()
@@ -156,18 +158,14 @@
         return apply_analysis_filter(
             analyses=self._get_query(Analysis),
             case_entry_id=case_entry_id,
             started_at_date=started_at_date,
             filter_functions=filter_functions,
         ).first()
 
-    def deliveries(self) -> Query:
-        """Fetch all deliveries."""
-        return self.Delivery.query
-
     def get_cases_created_within_days(self, days: int) -> List[Family]:
         """Fetch all cases created within the past days."""
         newer_than_date = dt.datetime.now() - dt.timedelta(days=days)
         return apply_case_filter(
             filter_functions=[CaseFilter.GET_NEW_BY_CREATION_DATE],
             cases=self._get_query(table=Family),
             creation_date=newer_than_date,
@@ -468,15 +466,15 @@
             LOG.info(f"{flow_cell.name}: status is {flow_cell.status}")
             statuses += [flow_cell.status] if flow_cell.status else []
             if not flow_cell.status or flow_cell.status == FlowCellStatus.REMOVED:
                 LOG.info(f"{flow_cell.name}: flow cell not on disk, requesting")
                 flow_cell.status = FlowCellStatus.REQUESTED
             elif flow_cell.status != FlowCellStatus.ON_DISK:
                 LOG.warning(f"{flow_cell.name}: {flow_cell.status}")
-        self.commit()
+        self.session.commit()
         return all(status == FlowCellStatus.ON_DISK for status in statuses)
 
     def get_invoices_by_status(self, is_invoiced: bool = None) -> List[Invoice]:
         """Return invoices by invoiced status."""
         invoices: Query = self._get_query(table=Invoice)
         if is_invoiced:
             return apply_invoice_filter(
```

### Comparing `cg-29.0.3/cg/store/api/status.py` & `cg-29.1.0/cg/store/api/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from datetime import datetime, timedelta
 from types import SimpleNamespace
-from typing import Callable, List, Optional
+from typing import List, Optional
 
 
-from sqlalchemy.orm import Query
+from sqlalchemy.orm import Query, Session
 from typing_extensions import Literal
 
 from cg.constants import CASE_ACTIONS, Pipeline, FlowCellStatus
 from cg.constants.constants import CaseActions
 from cg.constants.invoice import CustomerNames
-from cg.store.filters.status_customer_filters import CustomerFilter, apply_customer_filter
 from cg.store.models import (
     Analysis,
     Application,
     ApplicationVersion,
     Customer,
     Family,
     FamilySample,
@@ -30,14 +29,17 @@
 from cg.store.filters.status_pool_filters import apply_pool_filter, PoolFilter
 from cg.store.filters.status_application_filters import apply_application_filter, ApplicationFilter
 
 
 class StatusHandler(BaseHandler):
     """Handles status states for entities in the database."""
 
+    def __init__(self, session: Session):
+        super().__init__(session=session)
+
     def get_samples_to_receive(self, external: bool = False) -> List[Sample]:
         """Return samples to receive."""
         records: Query = self._get_join_sample_application_version_query()
         sample_filter_functions: List[SampleFilter] = [
             SampleFilter.FILTER_IS_NOT_RECEIVED,
             SampleFilter.FILTER_IS_NOT_DOWN_SAMPLED,
         ]
@@ -203,23 +205,23 @@
 
         return sorted(cases, key=lambda k: k["tat"], reverse=True)
 
     def set_case_action(self, action: Literal[CASE_ACTIONS], case_internal_id: str) -> None:
         """Sets the action of provided cases to None or the given action."""
         case: Family = self.get_case_by_internal_id(internal_id=case_internal_id)
         case.action = action
-        self.commit()
+        self.session.commit()
 
     def add_sample_comment(self, sample: Sample, comment: str) -> None:
         """Update comment on sample with the provided comment."""
         if sample.comment:
             sample.comment = sample.comment + " " + comment
         else:
             sample.comment = comment
-        self.commit()
+        self.session.commit()
 
     def get_flow_cells_by_case(self, case: Family) -> List[Flowcell]:
         """Return flow cells for case."""
         return apply_flow_cell_filter(
             flow_cells=self._get_join_flow_cell_sample_links_query(),
             filter_functions=[FlowCellFilter.GET_BY_CASE],
             case=case,
```

### Comparing `cg-29.0.3/cg/store/filters/status_analysis_filters.py` & `cg-29.1.0/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_application_filters.py` & `cg-29.1.0/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_application_version_filters.py` & `cg-29.1.0/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_bed_filters.py` & `cg-29.1.0/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_bed_version_filters.py` & `cg-29.1.0/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_case_filters.py` & `cg-29.1.0/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_case_sample_filters.py` & `cg-29.1.0/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_collaboration_filters.py` & `cg-29.1.0/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_customer_filters.py` & `cg-29.1.0/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_flow_cell_filters.py` & `cg-29.1.0/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_invoice_filters.py` & `cg-29.1.0/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_organism_filters.py` & `cg-29.1.0/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_panel_filters.py` & `cg-29.1.0/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_pool_filters.py` & `cg-29.1.0/cg/store/filters/status_pool_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 from typing import List, Optional, Callable
-from alchy import Query
+from sqlalchemy.orm import Query
 from cg.store.models import Pool, Customer
 
 
 def filter_pools_by_customer_id(pools: Query, customer_ids: List[int], **kwargs) -> Query:
     """Return pools by customer id."""
     return pools.filter(Pool.customer_id.in_(customer_ids))
```

### Comparing `cg-29.0.3/cg/store/filters/status_sample_filters.py` & `cg-29.1.0/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/filters/status_user_filters.py` & `cg-29.1.0/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/store/models.py` & `cg-29.1.0/cg/store/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime as dt
 import re
 from typing import List, Optional, Set, Dict
 
-import alchy
+from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import Column, ForeignKey, Table, UniqueConstraint, orm, types
 from sqlalchemy.util import deprecated
 
 from cg.constants import (
     CASE_ACTIONS,
     FLOWCELL_STATUS,
     PREP_CATEGORIES,
@@ -15,15 +15,25 @@
     STATUS_OPTIONS,
     DataDelivery,
     Pipeline,
 )
 
 from cg.constants.constants import CONTROL_OPTIONS, PrepCategory
 
-Model = alchy.make_declarative_base(Base=alchy.ModelBase)
+Model = declarative_base()
+
+
+def to_dict(model_instance):
+    if hasattr(model_instance, "__table__"):
+        return {
+            column.name: getattr(model_instance, column.name)
+            for column in model_instance.__table__.columns
+        }
+
+
 flowcell_sample = Table(
     "flowcell_sample",
     Model.metadata,
     Column("flowcell_id", types.Integer, ForeignKey("flowcell.id"), nullable=False),
     Column("sample_id", types.Integer, ForeignKey("sample.id"), nullable=False),
     UniqueConstraint("flowcell_id", "sample_id", name="_flowcell_sample_uc"),
 )
@@ -72,14 +82,16 @@
     @property
     def low_priority(self):
         """Has low priority?"""
         return self.priority_int < 1
 
 
 class Application(Model):
+    __tablename__ = "application"
+
     id = Column(types.Integer, primary_key=True)
     tag = Column(types.String(32), unique=True, nullable=False)
     prep_category = Column(types.Enum(*PREP_CATEGORIES), nullable=False)
     is_external = Column(types.Boolean, nullable=False, default=False)
     description = Column(types.String(256), nullable=False)
     is_accredited = Column(types.Boolean, nullable=False)
 
@@ -123,16 +135,20 @@
 
         return (
             PrepCategory.WHOLE_GENOME_SEQUENCING.value
             if self.prep_category == PrepCategory.WHOLE_GENOME_SEQUENCING.value
             else PrepCategory.WHOLE_EXOME_SEQUENCING.value
         )
 
+    def to_dict(self):
+        return to_dict(model_instance=self)
+
 
 class ApplicationVersion(Model):
+    __tablename__ = "application_version"
     __table_args__ = (UniqueConstraint("application_id", "version", name="_app_version_uc"),)
 
     id = Column(types.Integer, primary_key=True)
     version = Column(types.Integer, nullable=False)
 
     valid_from = Column(types.DateTime, default=dt.datetime.now, nullable=False)
     price_standard = Column(types.Integer)
@@ -147,21 +163,23 @@
     application_id = Column(ForeignKey(Application.id), nullable=False)
 
     def __str__(self) -> str:
         return f"{self.application.tag} ({self.version})"
 
     def to_dict(self, application: bool = True):
         """Represent as dictionary"""
-        data = super(ApplicationVersion, self).to_dict()
+        data = to_dict(model_instance=self)
         if application:
             data["application"] = self.application.to_dict()
         return data
 
 
 class Analysis(Model):
+    __tablename__ = "analysis"
+
     id = Column(types.Integer, primary_key=True)
     pipeline = Column(types.Enum(*list(Pipeline)))
     pipeline_version = Column(types.String(32))
     started_at = Column(types.DateTime)
     completed_at = Column(types.DateTime)
     delivery_report_created_at = Column(types.DateTime)
     upload_started_at = Column(types.DateTime)
@@ -175,23 +193,24 @@
     uploaded_to_vogue_at = Column(types.DateTime, nullable=True)
 
     def __str__(self):
         return f"{self.family.internal_id} | {self.completed_at.date()}"
 
     def to_dict(self, family: bool = True):
         """Represent as dictionary"""
-        data = super(Analysis, self).to_dict()
+        data = to_dict(model_instance=self)
         if family:
             data["family"] = self.family.to_dict()
         return data
 
 
 class Bed(Model):
     """Model for bed target captures"""
 
+    __tablename__ = "bed"
     id = Column(types.Integer, primary_key=True)
     name = Column(types.String(32), unique=True, nullable=False)
     comment = Column(types.Text)
     is_archived = Column(types.Boolean, default=False)
     created_at = Column(types.DateTime, default=dt.datetime.now)
     updated_at = Column(types.DateTime, onupdate=dt.datetime.now)
 
@@ -200,14 +219,15 @@
     def __str__(self) -> str:
         return self.name
 
 
 class BedVersion(Model):
     """Model for bed target captures versions"""
 
+    __tablename__ = "bed_version"
     __table_args__ = (UniqueConstraint("bed_id", "version", name="_app_version_uc"),)
 
     id = Column(types.Integer, primary_key=True)
     shortname = Column(types.String(64))
     version = Column(types.Integer, nullable=False)
     filename = Column(types.String(256), nullable=False)
     checksum = Column(types.String(32))
@@ -220,21 +240,22 @@
     bed_id = Column(ForeignKey(Bed.id), nullable=False)
 
     def __str__(self) -> str:
         return f"{self.bed.name} ({self.version})"
 
     def to_dict(self, bed: bool = True):
         """Represent as dictionary"""
-        data = super(BedVersion, self).to_dict()
+        data = to_dict(model_instance=self)
         if bed:
             data["bed"] = self.bed.to_dict()
         return data
 
 
 class Customer(Model):
+    __tablename__ = "customer"
     agreement_date = Column(types.DateTime)
     agreement_registration = Column(types.String(32))
     comment = Column(types.Text)
     id = Column(types.Integer, primary_key=True)
     internal_id = Column(types.String(32), unique=True, nullable=False)
     invoice_address = Column(types.Text, nullable=False)
     invoice_reference = Column(types.String(32), nullable=False)
@@ -266,16 +287,20 @@
             customer
             for collaboration in self.collaborations
             for customer in collaboration.customers
         }
         customers.add(self)
         return customers
 
+    def to_dict(self):
+        return to_dict(model_instance=self)
+
 
 class Collaboration(Model):
+    __tablename__ = "collaboration"
     id = Column(types.Integer, primary_key=True)
     internal_id = Column(types.String(32), unique=True, nullable=False)
     name = Column(types.String(128), nullable=False)
     customers = orm.relationship(Customer, secondary=customer_collaboration)
 
     def __str__(self) -> str:
         return f"{self.internal_id} ({self.name})"
@@ -287,24 +312,26 @@
             "id": self.id,
             "name": self.name,
             "internal_id": self.internal_id,
         }
 
 
 class Delivery(Model):
+    __tablename__ = "delivery"
     id = Column(types.Integer, primary_key=True)
     delivered_at = Column(types.DateTime)
     removed_at = Column(types.DateTime)
     destination = Column(types.Enum("caesar", "pdc", "uppmax", "mh", "custom"), default="caesar")
     sample_id = Column(ForeignKey("sample.id", ondelete="CASCADE"))
     pool_id = Column(ForeignKey("pool.id", ondelete="CASCADE"))
     comment = Column(types.Text)
 
 
 class Family(Model, PriorityMixin):
+    __tablename__ = "family"
     __table_args__ = (UniqueConstraint("customer_id", "name", name="_customer_name_uc"),)
 
     action = Column(types.Enum(*CASE_ACTIONS))
     analyses = orm.relationship(Analysis, backref="family", order_by="-Analysis.completed_at")
     _cohorts = Column(types.Text)
     comment = Column(types.Text)
     created_at = Column(types.DateTime, default=dt.datetime.now)
@@ -413,28 +440,29 @@
         for data_delivery, pipeline in delivery_per_pipeline_map.items():
             if data_delivery in requested_deliveries:
                 delivery_arguments.add(pipeline)
         return delivery_arguments
 
     def to_dict(self, links: bool = False, analyses: bool = False) -> dict:
         """Represent as dictionary."""
-        data = super(Family, self).to_dict()
+        data = to_dict(model_instance=self)
         data["panels"] = self.panels
         data["priority"] = self.priority_human
         data["customer"] = self.customer.to_dict()
         if links:
             data["links"] = [link_obj.to_dict(samples=True) for link_obj in self.links]
         if analyses:
             data["analyses"] = [
                 analysis_obj.to_dict(family=False) for analysis_obj in self.analyses
             ]
         return data
 
 
 class FamilySample(Model):
+    __tablename__ = "family_sample"
     __table_args__ = (UniqueConstraint("family_id", "sample_id", name="_family_sample_uc"),)
 
     id = Column(types.Integer, primary_key=True)
     family_id = Column(ForeignKey("family.id", ondelete="CASCADE"), nullable=False)
     sample_id = Column(ForeignKey("sample.id", ondelete="CASCADE"), nullable=False)
     status = Column(types.Enum(*STATUS_OPTIONS), default="unknown", nullable=False)
 
@@ -447,15 +475,15 @@
     family = orm.relationship("Family", backref="links")
     sample = orm.relationship("Sample", foreign_keys=[sample_id], backref="links")
     mother = orm.relationship("Sample", foreign_keys=[mother_id], backref="mother_links")
     father = orm.relationship("Sample", foreign_keys=[father_id], backref="father_links")
 
     def to_dict(self, parents: bool = False, samples: bool = False, family: bool = False) -> dict:
         """Represent as dictionary"""
-        data = super(FamilySample, self).to_dict()
+        data = to_dict(model_instance=self)
         if samples:
             data["sample"] = self.sample.to_dict()
             data["mother"] = self.mother.to_dict() if self.mother else None
             data["father"] = self.father.to_dict() if self.father else None
         elif parents:
             data["mother"] = self.mother.to_dict() if self.mother else None
             data["father"] = self.father.to_dict() if self.father else None
@@ -464,14 +492,15 @@
         return data
 
     def __str__(self) -> str:
         return f"{self.family.internal_id} | {self.sample.internal_id}"
 
 
 class Flowcell(Model):
+    __tablename__ = "flowcell"
     id = Column(types.Integer, primary_key=True)
     name = Column(types.String(32), unique=True, nullable=False)
     sequencer_type = Column(types.Enum("hiseqga", "hiseqx", "novaseq"))
     sequencer_name = Column(types.String(32))
     sequenced_at = Column(types.DateTime)
     status = Column(types.Enum(*FLOWCELL_STATUS), default="ondisk")
     archived_at = Column(types.DateTime)
@@ -480,53 +509,56 @@
     samples = orm.relationship("Sample", secondary=flowcell_sample, backref="flowcells")
 
     def __str__(self):
         return self.name
 
     def to_dict(self, samples: bool = False):
         """Represent as dictionary"""
-        data = super(Flowcell, self).to_dict()
+        data = to_dict(model_instance=Flowcell)
         if samples:
             data["samples"] = [sample.to_dict() for sample in self.samples]
         return data
 
 
 class Organism(Model):
+    __tablename__ = "organism"
     id = Column(types.Integer, primary_key=True)
     internal_id = Column(types.String(32), nullable=False, unique=True)
     name = Column(types.String(255), nullable=False, unique=True)
     created_at = Column(types.DateTime, default=dt.datetime.now)
     updated_at = Column(types.DateTime, onupdate=dt.datetime.now)
     reference_genome = Column(types.String(255))
     verified = Column(types.Boolean, default=False)
     comment = Column(types.Text)
 
     def __str__(self) -> str:
         return f"{self.internal_id} ({self.name})"
 
     def to_dict(self) -> dict:
         """Represent as dictionary"""
-        return super(Organism, self).to_dict()
+        return to_dict(model_instance=self)
 
 
 class Panel(Model):
+    __tablename__ = "panel"
     abbrev = Column(types.String(32), unique=True)
     current_version = Column(types.Float, nullable=False)
     customer_id = Column(ForeignKey("customer.id", ondelete="CASCADE"), nullable=False)
     customer = orm.relationship(Customer, backref="panels")
     date = Column(types.DateTime, nullable=False)
     gene_count = Column(types.Integer)
     id = Column(types.Integer, primary_key=True)
     name = Column(types.String(64), unique=True)
 
     def __str__(self):
         return f"{self.abbrev} ({self.current_version})"
 
 
 class Pool(Model):
+    __tablename__ = "pool"
     __table_args__ = (UniqueConstraint("order", "name", name="_order_name_uc"),)
 
     application_version_id = Column(ForeignKey("application_version.id"), nullable=False)
     application_version = orm.relationship(
         ApplicationVersion, foreign_keys=[application_version_id]
     )
     comment = Column(types.Text)
@@ -542,14 +574,15 @@
     order = Column(types.String(64), nullable=False)
     ordered_at = Column(types.DateTime, nullable=False)
     received_at = Column(types.DateTime)
     ticket = Column(types.String(32))
 
 
 class Sample(Model, PriorityMixin):
+    __tablename__ = "sample"
     age_at_sampling = Column(types.FLOAT)
     application_version_id = Column(ForeignKey("application_version.id"), nullable=False)
     application_version = orm.relationship(
         ApplicationVersion, foreign_keys=[application_version_id]
     )
     capture_kit = Column(types.String(64))
     comment = Column(types.Text)
@@ -642,27 +675,28 @@
         if self.received_at:
             return f"Received {self.received_at.date()}"
 
         return f"Ordered {self.ordered_at.date()}"
 
     def to_dict(self, links: bool = False, flowcells: bool = False) -> dict:
         """Represent as dictionary"""
-        data = super(Sample, self).to_dict()
+        data = to_dict(model_instance=self)
         data["priority"] = self.priority_human
         data["customer"] = self.customer.to_dict()
         data["application_version"] = self.application_version.to_dict()
         data["application"] = self.application_version.application.to_dict()
         if links:
             data["links"] = [link_obj.to_dict(family=True, parents=True) for link_obj in self.links]
         if flowcells:
             data["flowcells"] = [flowcell_obj.to_dict() for flowcell_obj in self.flowcells]
         return data
 
 
 class Invoice(Model):
+    __tablename__ = "invoice"
     id = Column(types.Integer, primary_key=True)
     customer_id = Column(ForeignKey("customer.id"), nullable=False)
     customer = orm.relationship(Customer, foreign_keys=[customer_id])
     created_at = Column(types.DateTime, default=dt.datetime.now)
     updated_at = Column(types.DateTime, onupdate=dt.datetime.now)
     invoiced_at = Column(types.DateTime)
     comment = Column(types.Text)
@@ -676,27 +710,28 @@
     pools = orm.relationship(Pool, backref="invoice")
 
     def __str__(self):
         return f"{self.customer_id} ({self.invoiced_at})"
 
     def to_dict(self) -> dict:
         """Represent as dictionary"""
-        return super(Invoice, self).to_dict()
+        return to_dict(model_instance=self)
 
 
 class User(Model):
+    __tablename__ = "user"
     id = Column(types.Integer, primary_key=True)
     name = Column(types.String(128), nullable=False)
     email = Column(types.String(128), unique=True, nullable=False)
     is_admin = Column(types.Boolean, default=False)
     order_portal_login = Column(types.Boolean, default=False)
 
     customers = orm.relationship("Customer", secondary=customer_user, backref="users")
 
     def to_dict(self) -> dict:
         """Represent as dictionary"""
-        data = super(User, self).to_dict()
+        data = to_dict(model_instance=self)
         data["customers"] = [record.to_dict() for record in self.customers]
         return data
 
     def __str__(self) -> str:
         return self.name
```

### Comparing `cg-29.0.3/cg/utils/checksum/checksum.py` & `cg-29.1.0/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/utils/click/EnumChoice.py` & `cg-29.1.0/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/utils/commands.py` & `cg-29.1.0/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/utils/date.py` & `cg-29.1.0/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/utils/dict.py` & `cg-29.1.0/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/utils/dispatcher.py` & `cg-29.1.0/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/utils/email.py` & `cg-29.1.0/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/utils/flask/enum.py` & `cg-29.1.0/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg/utils/utils.py` & `cg-29.1.0/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/cg.egg-info/PKG-INFO` & `cg-29.1.0/cg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 29.0.3
+Version: 29.1.0
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-29.0.3/cg.egg-info/SOURCES.txt` & `cg-29.1.0/cg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/requirements.txt` & `cg-29.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/setup.py` & `cg-29.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="29.0.3",
+    version="29.1.0",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     include_package_data=True,
```

### Comparing `cg-29.0.3/tests/apps/cgstats/conftest.py` & `cg-29.1.0/tests/apps/cgstats/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/cgstats/crud/test_create_novaseq.py` & `cg-29.1.0/tests/apps/cgstats/crud/test_create_novaseq.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/cgstats/crud/test_delete.py` & `cg-29.1.0/tests/apps/cgstats/crud/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/cgstats/parsers/test_conversion_stats.py` & `cg-29.1.0/tests/apps/cgstats/parsers/test_conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/cgstats/parsers/test_demux_stats.py` & `cg-29.1.0/tests/apps/cgstats/parsers/test_demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/cgstats/parsers/test_run_info.py` & `cg-29.1.0/tests/apps/cgstats/parsers/test_run_info.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/cgstats/test_cgstats_create.py` & `cg-29.1.0/tests/apps/cgstats/test_cgstats_create.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/cgstats/test_stats.py` & `cg-29.1.0/tests/apps/cgstats/test_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/conftest.py` & `cg-29.1.0/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/coverage/test_coverage.py` & `cg-29.1.0/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/crunchy/conftest.py` & `cg-29.1.0/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/crunchy/test_compress_fastq.py` & `cg-29.1.0/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/crunchy/test_config.py` & `cg-29.1.0/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/crunchy/test_crunchy.py` & `cg-29.1.0/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/crunchy/test_spring_decompression.py` & `cg-29.1.0/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/demultiplex/conftest.py` & `cg-29.1.0/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/demultiplex/test_convert_to_sample_sheet.py` & `cg-29.1.0/tests/apps/demultiplex/test_convert_to_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-29.1.0/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/demultiplex/test_parse_run_parameters.py` & `cg-29.1.0/tests/apps/demultiplex/test_parse_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/demultiplex/test_sample_sheet.py` & `cg-29.1.0/tests/apps/demultiplex/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/gens/test_gens_api.py` & `cg-29.1.0/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/gt/conftest.py` & `cg-29.1.0/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/gt/test_gt_api.py` & `cg-29.1.0/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/hk/conftest.py` & `cg-29.1.0/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/hk/test__getattr__.py` & `cg-29.1.0/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/hk/test_add_file.py` & `cg-29.1.0/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/hk/test_bundles.py` & `cg-29.1.0/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/hk/test_core.py` & `cg-29.1.0/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/hk/test_file.py` & `cg-29.1.0/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/hk/test_version.py` & `cg-29.1.0/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/lims/conftest.py` & `cg-29.1.0/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/lims/test_api.py` & `cg-29.1.0/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/loqus/conftest.py` & `cg-29.1.0/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/loqus/test_loqusdb_api.py` & `cg-29.1.0/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/madeline/conftest.py` & `cg-29.1.0/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/madeline/test_madeline.py` & `cg-29.1.0/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/mip/conftest.py` & `cg-29.1.0/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/mip/test_config_mip.py` & `cg-29.1.0/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/mutacc_auto/conftest.py` & `cg-29.1.0/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-29.1.0/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/orderform/conftest.py` & `cg-29.1.0/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-29.1.0/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/orderform/test_excel_sample_schema.py` & `cg-29.1.0/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/orderform/test_json_orderform_parser.py` & `cg-29.1.0/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/orderform/test_orderform_parser.py` & `cg-29.1.0/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/scout/conftest.py` & `cg-29.1.0/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/scout/test_get_causative_variants.py` & `cg-29.1.0/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/scout/test_get_scout_cases.py` & `cg-29.1.0/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/scout/test_scout_load_config.py` & `cg-29.1.0/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/scout/test_scout_models.py` & `cg-29.1.0/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/slurm/conftest.py` & `cg-29.1.0/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/slurm/test_slurm_api.py` & `cg-29.1.0/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/test_apps_environ.py` & `cg-29.1.0/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/test_osticket.py` & `cg-29.1.0/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/vogue/conftest.py` & `cg-29.1.0/tests/apps/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/apps/vogue/test_vogue_api.py` & `cg-29.1.0/tests/apps/vogue/test_vogue_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/add/test_cli_add.py` & `cg-29.1.0/tests/cli/add/test_cli_add.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     customer = disk_store.add_customer(
         internal_id=customer_id,
         name="Test Customer",
         scout_access=False,
         invoice_address="Street nr, 12345 Uppsala",
         invoice_reference="ABCDEF",
     )
-    disk_store.add_commit(customer)
+    disk_store.session.add(customer)
+    disk_store.session.commit()
     # GIVEN that there is a certain number of users
     user_query = disk_store._get_query(table=User)
     nr_users = user_query.count()
 
     # WHEN adding a new user
     name, email = "Paul T. Anderson", "paul.anderson@magnolia.com"
     result = cli_runner.invoke(add, ["user", "-c", customer_id, email, name], obj=base_context)
```

### Comparing `cg-29.0.3/tests/cli/add/test_cli_add_customer.py` & `cg-29.1.0/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/add/test_cli_add_family.py` & `cg-29.1.0/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/add/test_cli_add_relationship.py` & `cg-29.1.0/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/add/test_cli_add_sample.py` & `cg-29.1.0/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/backup/conftest.py` & `cg-29.1.0/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/backup/test_backup_command.py` & `cg-29.1.0/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/clean/conftest.py` & `cg-29.1.0/tests/cli/clean/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     case_to_not_clean = helpers.add_case(
         store=store,
         internal_id=balsamic_case_not_clean,
         name=balsamic_case_not_clean,
         data_analysis=Pipeline.BALSAMIC,
     )
     case_to_not_clean.action = "running"
-    store.commit()
+    store.session.commit()
 
     sample_case_to_not_clean = helpers.add_sample(
         store,
         internal_id=balsamic_case_not_clean,
         is_tumour=True,
         application_type="wgs",
     )
```

### Comparing `cg-29.0.3/tests/cli/clean/test_balsamic_clean.py` & `cg-29.1.0/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-29.1.0/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/clean/test_hk_bundle_files.py` & `cg-29.1.0/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-29.1.0/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/clean/test_microbial_clean.py` & `cg-29.1.0/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-29.1.0/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/compress/conftest.py` & `cg-29.1.0/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/compress/test_cli_compress_fastq.py` & `cg-29.1.0/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         store=status_db,
         name=case_id,
         internal_id=case_id,
         data_analysis=Pipeline.MIP_DNA,
         action=None,
     )
     valid_compressable_case.created_at = dt.datetime.now() - dt.timedelta(days=1000)
-    status_db.commit()
+    status_db.session.commit()
 
     # WHEN running the compress command
     cases: List[Family] = get_cases_to_process(days_back=1, store=status_db)
 
     # THEN assert cases are returned
     assert cases
 
@@ -134,15 +134,15 @@
         case=valid_compressable_case,
     )
     helpers.add_relationship(
         store=status_db,
         sample=sample2,
         case=valid_compressable_case,
     )
-    status_db.commit()
+    status_db.session.commit()
 
     # GIVEN no adjusting according to readsa
     mocker.patch(MOCK_SET_MEM_ACCORDING_TO_READS_PATH, return_value=None)
 
     # WHEN running the compress command
     res = cli_runner.invoke(fastq_cmd, ["--case-id", case_id], obj=populated_compress_context)
```

### Comparing `cg-29.0.3/tests/cli/compress/test_cli_decompress_spring.py` & `cg-29.1.0/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/compress/test_compress_helpers.py` & `cg-29.1.0/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/compress/test_store_fastq.py` & `cg-29.1.0/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/conftest.py` & `cg-29.1.0/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/delete/test_cli_delete_case.py` & `cg-29.1.0/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/delete/test_cli_delete_cases.py` & `cg-29.1.0/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/deliver/conftest.py` & `cg-29.1.0/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/deliver/test_deliver_base.py` & `cg-29.1.0/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/deliver/test_rsync_base.py` & `cg-29.1.0/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-29.1.0/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/demultiplex/conftest.py` & `cg-29.1.0/tests/cli/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/demultiplex/test_add_flowcell.py` & `cg-29.1.0/tests/cli/demultiplex/test_add_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-29.1.0/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-29.1.0/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/demultiplex/test_finish_demux.py` & `cg-29.1.0/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/demultiplex/test_stats_command.py` & `cg-29.1.0/tests/cli/demultiplex/test_stats_command.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-29.1.0/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/generate/report/conftest.py` & `cg-29.1.0/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-29.1.0/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/generate/report/test_utils.py` & `cg-29.1.0/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/generate/test_cli_base.py` & `cg-29.1.0/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/get/test_cli_get.py` & `cg-29.1.0/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/get/test_cli_get_analysis.py` & `cg-29.1.0/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/get/test_cli_get_case.py` & `cg-29.1.0/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/get/test_cli_get_flow_cell.py` & `cg-29.1.0/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/get/test_cli_get_sample.py` & `cg-29.1.0/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/set/conftest.py` & `cg-29.1.0/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/set/test_cli_set_case.py` & `cg-29.1.0/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/set/test_cli_set_cases.py` & `cg-29.1.0/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/set/test_cli_set_flowcell.py` & `cg-29.1.0/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/set/test_cli_set_list_keys.py` & `cg-29.1.0/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/set/test_cli_set_sample.py` & `cg-29.1.0/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/set/test_cli_set_samples.py` & `cg-29.1.0/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/store/test_fastq.py` & `cg-29.1.0/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/test_base.py` & `cg-29.1.0/tests/cli/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,40 +28,40 @@
 def test_missing_command(cli_runner: CliRunner):
     # WHEN invoking a missing command
     result = cli_runner.invoke(cg, ["i_dont_exist"])
     # THEN context should abort
     assert result.exit_code != 0
 
 
-def test_cli_init(cli_runner: CliRunner, base_context: CGConfig, caplog):
+def test_cli_init(cli_runner: CliRunner, base_context: CGConfig, caplog, tmp_path: Path):
     caplog.set_level(logging.INFO)
     # GIVEN you want to setup a new database using the CLI
     database = "./test_db.sqlite3"
     database_path = Path(database)
     database_uri = f"sqlite:///{database}"
     base_context.status_db_ = Store(uri=database_uri)
-    with cli_runner.isolated_filesystem():
-        assert database_path.exists() is False
 
-        # WHEN calling "init"
-        result = cli_runner.invoke(init, [], obj=base_context)
+    assert database_path.exists() is False
 
-        # THEN it should setup the database with some tables
-        assert result.exit_code == 0
-        assert database_path.exists()
-        assert len(Store(uri=database_uri).engine.table_names()) > 0
-
-        # GIVEN the database already exists
-        # WHEN calling the init function
-        result = cli_runner.invoke(init, [], obj=base_context)
-
-        # THEN it should print an error and give error exit code
-        assert result.exit_code != 0
-        assert "Database already exists" in caplog.text
-
-        # GIVEN the database already exists
-        # WHEN calling "init" with "--reset"
-        result = cli_runner.invoke(init, ["--reset"], input="Yes", obj=base_context)
-
-        # THEN it should re-setup the tables and print new tables
-        assert result.exit_code == 0
-        assert "Success!" in caplog.text
+    # WHEN calling "init"
+    result = cli_runner.invoke(init, [], obj=base_context)
+
+    # THEN it should setup the database with some tables
+    assert result.exit_code == 0
+    assert database_path.exists()
+    assert len(Store(uri=database_uri).engine.table_names()) > 0
+
+    # GIVEN the database already exists
+    # WHEN calling the init function
+    result = cli_runner.invoke(init, [], obj=base_context)
+
+    # THEN it should print an error and give error exit code
+    assert result.exit_code != 0
+    assert "Database already exists" in caplog.text
+
+    # GIVEN the database already exists
+    # WHEN calling "init" with "--reset"
+    result = cli_runner.invoke(init, ["--reset"], input="Yes", obj=base_context)
+
+    # THEN it should re-setup the tables and print new tables
+    assert result.exit_code == 0
+    assert "Success!" in caplog.text
```

### Comparing `cg-29.0.3/tests/cli/test_clean.py` & `cg-29.1.0/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/test_cli_status_cases.py` & `cg-29.1.0/tests/cli/test_cli_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/upload/conftest.py` & `cg-29.1.0/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/upload/test_cli_scout.py` & `cg-29.1.0/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/upload/test_cli_upload.py` & `cg-29.1.0/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/upload/test_cli_upload_auto.py` & `cg-29.1.0/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-29.1.0/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/upload/test_cli_upload_fastq.py` & `cg-29.1.0/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,14 @@
     analysis_obj: Analysis, caplog, base_context, cli_runner, case_id: str
 ):
     """Tests if the command finds a non-uploaded analysis and attempts to start it"""
     caplog.set_level(logging.INFO)
     # GIVEN a case to be delivered
     analysis_obj.pipeline = Pipeline.FASTQ
     analysis_obj.family.data_delivery = DataDelivery.FASTQ
-    base_context.status_db.commit()
+    base_context.status_db.session.commit()
     base_context.status_db.session.close()
     # WHEN the upload command is invoked with dry run
     cli_runner.invoke(auto_fastq, ["--dry-run"], obj=base_context)
 
     # THEN the content of the .sh file should be in the caplog
     assert f"#SBATCH --job-name={case_id}_rsync" in caplog.text
```

### Comparing `cg-29.0.3/tests/cli/upload/test_cli_upload_genotype.py` & `cg-29.1.0/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/upload/test_cli_upload_gens.py` & `cg-29.1.0/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/upload/test_cli_upload_nipt.py` & `cg-29.1.0/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-29.1.0/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-29.1.0/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/upload/test_cli_upload_observations.py` & `cg-29.1.0/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/upload/test_cli_upload_vogue.py` & `cg-29.1.0/tests/cli/upload/test_cli_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/balsamic/conftest.py` & `cg-29.1.0/tests/cli/workflow/balsamic/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -723,30 +723,31 @@
     helpers.add_case(status_db, internal_id="no_sample_case", name="no_sample_case")
 
     # Create BED1 version 1
     bed1_name = "BalsamicBed1"
     bed1_filename = "balsamic_bed_1.bed"
     Path(cg_dir, bed1_filename).touch(exist_ok=True)
     bed1 = status_db.add_bed(name=bed1_name)
-    status_db.add_commit(bed1)
+    status_db.session.add(bed1)
     version1 = status_db.add_bed_version(
         bed=bed1, version=1, filename=bed1_filename, shortname=bed1_name
     )
-    status_db.add_commit(version1)
+    status_db.session.add(version1)
 
     # Create BED2 version 1
     bed2_name = "BalsamicBed2"
     bed2_filename = "balsamic_bed_2.bed"
     Path(cg_dir, bed2_filename).touch(exist_ok=True)
     bed2 = status_db.add_bed(name=bed2_name)
-    status_db.add_commit(bed2)
+    status_db.session.add(bed2)
     version2 = status_db.add_bed_version(
         bed=bed2, version=1, filename=bed2_filename, shortname=bed2_name
     )
-    status_db.add_commit(version2)
+    status_db.session.add(version2)
+    status_db.session.commit()
     return cg_context
 
 
 @pytest.fixture
 def mock_config(balsamic_dir: Path, balsamic_case_id: str) -> None:
     """Create dummy config file at specified path"""
```

### Comparing `cg-29.0.3/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-29.1.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-29.1.0/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     # GIVEN that HermesAPI returns a deliverables output
     mocker.patch.object(HermesApi, "convert_deliverables")
     HermesApi.convert_deliverables.return_value = CGDeliverables(**hermes_deliverables)
 
     # Ensure case was successfully picked up by start-available and status set to running
     result = cli_runner.invoke(start_available, ["--dry-run"], obj=balsamic_context)
     balsamic_context.status_db.get_case_by_internal_id(case_id_success).action = "running"
-    balsamic_context.status_db.commit()
+    balsamic_context.status_db.session.commit()
 
     # THEN command exits with 1 because one of the cases threw errors
     assert result.exit_code == 1
     assert case_id_success in caplog.text
     assert balsamic_context.status_db.get_case_by_internal_id(case_id_success).action == "running"
 
     balsamic_context.housekeeper_api_ = real_housekeeper_api
```

### Comparing `cg-29.0.3/tests/cli/workflow/balsamic/test_link.py` & `cg-29.1.0/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-29.1.0/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/balsamic/test_run.py` & `cg-29.1.0/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-29.1.0/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/conftest.py` & `cg-29.1.0/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-29.1.0/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/fluffy/conftest.py` & `cg-29.1.0/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-29.1.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-29.1.0/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-29.1.0/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-29.1.0/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-29.1.0/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 
     # GIVEN a case_id that does exist in database
 
     # GIVEN that case action is None
     fluffy_analysis_api.status_db.get_case_by_internal_id(
         internal_id=fluffy_case_id_existing
     ).action = None
-    fluffy_analysis_api.status_db.commit()
+    fluffy_analysis_api.status_db.session.commit()
 
     # GIVEN deliverables were generated and could be found
     mocker.patch.object(FluffyAnalysisAPI, "get_deliverables_file_path")
     FluffyAnalysisAPI.get_deliverables_file_path.return_value = deliverables_yaml_fixture_path
 
     # GIVEN the same timestamp is attained when storing analysis in different databases
     mocker.patch.object(FluffyAnalysisAPI, "get_date_from_file_path")
```

### Comparing `cg-29.0.3/tests/cli/workflow/microsalt/conftest.py` & `cg-29.1.0/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py` & `cg-29.1.0/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-29.1.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-29.1.0/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/mip/conftest.py` & `cg-29.1.0/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-29.1.0/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     caplog.set_level("INFO")
     mip_analysis_api: MipDNAAnalysisAPI = mip_dna_context.meta_apis["analysis_api"]
 
     # GIVEN a case_id that does exist in database
 
     # GIVEN that case action is None
     mip_analysis_api.status_db.get_case_by_internal_id(internal_id=mip_case_id).action = None
-    mip_analysis_api.status_db.commit()
+    mip_analysis_api.status_db.session.commit()
 
     # GIVEN deliverables were generated and could be found
     mocker.patch.object(MipDNAAnalysisAPI, "get_deliverables_file_path")
     MipDNAAnalysisAPI.get_deliverables_file_path.return_value = mip_deliverables_file
 
     # GIVEN the same timestamp is attained when storing analysis in different databases
     mocker.patch.object(MipDNAAnalysisAPI, "get_date_from_file_path")
```

### Comparing `cg-29.0.3/tests/cli/workflow/rnafusion/conftest.py` & `cg-29.1.0/tests/cli/workflow/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-29.1.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     HermesApi.convert_deliverables.return_value = CGDeliverables(**hermes_deliverables)
 
     # GIVEN a mocked config
 
     # Ensure case was successfully picked up by start-available and status set to running
     result = cli_runner.invoke(start_available, ["--dry-run"], obj=rnafusion_context)
     rnafusion_context.status_db.get_case_by_internal_id(case_id_success).action = "running"
-    rnafusion_context.status_db.commit()
+    rnafusion_context.status_db.session.commit()
 
     # THEN command exits with 0
     assert result.exit_code == EXIT_SUCCESS
     assert case_id_success in caplog.text
     assert rnafusion_context.status_db.get_case_by_internal_id(case_id_success).action == "running"
 
     rnafusion_context.housekeeper_api_ = real_housekeeper_api
```

### Comparing `cg-29.0.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-29.1.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py` & `cg-29.1.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-29.1.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-29.1.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/test_cli_workflow.py` & `cg-29.1.0/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-29.1.0/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/conftest.py` & `cg-29.1.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1149,15 +1149,15 @@
     invoice_reference: str,
     store: Store,
     prices: Dict[str, int],
 ) -> Store:
     """Setup and example store."""
     collaboration = store.add_collaboration(internal_id=collaboration_id, name=collaboration_id)
 
-    store.add_commit(collaboration)
+    store.session.add(collaboration)
     customers: List[Customer] = []
     customer_map: Dict[str, str] = {
         customer_id: "Production",
         "cust001": "Customer",
         "cust002": "Karolinska",
         "cust003": "CMMS",
     }
@@ -1170,15 +1170,15 @@
                 invoice_address=invoice_address,
                 invoice_reference=invoice_reference,
             )
         )
 
     for customer in customers:
         collaboration.customers.append(customer)
-    store.add_commit(customers)
+    store.session.add_all(customers)
     applications = [
         store.add_application(
             tag="WGXCUSC000",
             prep_category="wgs",
             description="External WGS",
             sequencing_depth=0,
             is_external=True,
@@ -1197,15 +1197,15 @@
             target_reads=10,
         ),
         store.add_application(
             tag="WGSPCFC060",
             prep_category="wgs",
             description="WGS, double",
             sequencing_depth=30,
-            accredited=True,
+            is_accredited=True,
             percent_kth=80,
             percent_reads_guaranteed=75,
             target_reads=10,
         ),
         store.add_application(
             tag="RMLP05R800",
             prep_category="rml",
@@ -1257,54 +1257,55 @@
         store.add_application(
             tag=apptag_rna,
             prep_category="tgs",
             description="RNA seq, poly-A based priming",
             percent_kth=80,
             percent_reads_guaranteed=75,
             sequencing_depth=25,
-            accredited=True,
+            is_accredited=True,
             target_reads=10,
             min_sequencing_depth=30,
         ),
         store.add_application(
             tag="VWGDPTR001",
             prep_category="cov",
             description="Viral whole genome  ",
             sequencing_depth=0,
             percent_kth=80,
             percent_reads_guaranteed=75,
             target_reads=10,
         ),
     ]
 
-    store.add_commit(applications)
+    store.session.add_all(applications)
 
     versions = [
         store.add_application_version(
             application=application, version=1, valid_from=datetime.now(), prices=prices
         )
         for application in applications
     ]
-    store.add_commit(versions)
+    store.session.add_all(versions)
 
     beds: List[Bed] = [store.add_bed(name=bed_name)]
-    store.add_commit(beds)
+    store.session.add_all(beds)
     bed_versions: List[BedVersion] = [
         store.add_bed_version(
             bed=bed,
             version=1,
             filename=bed_name + FileExtensions.BED,
             shortname=bed_version_short_name,
         )
         for bed in beds
     ]
-    store.add_commit(bed_versions)
+    store.session.add_all(bed_versions)
 
     organism = store.add_organism("C. jejuni", "C. jejuni")
-    store.add_commit(organism)
+    store.session.add(organism)
+    store.session.commit()
 
     yield store
 
 
 @pytest.fixture()
 def sample_store(base_store: Store) -> Store:
     """Populate store with samples."""
@@ -1313,18 +1314,16 @@
         base_store.add_sample(name="received", sex=Gender.UNKNOWN, received=datetime.now()),
         base_store.add_sample(
             name="received-prepared",
             sex=Gender.UNKNOWN,
             received=datetime.now(),
             prepared_at=datetime.now(),
         ),
-        base_store.add_sample("external", sex=Gender.FEMALE, external=True),
-        base_store.add_sample(
-            name="external-received", sex=Gender.FEMALE, received=datetime.now(), external=True
-        ),
+        base_store.add_sample(name="external", sex=Gender.FEMALE),
+        base_store.add_sample(name="external-received", sex=Gender.FEMALE, received=datetime.now()),
         base_store.add_sample(
             name="sequenced",
             sex=Gender.MALE,
             received=datetime.now(),
             prepared_at=datetime.now(),
             sequenced_at=datetime.now(),
             reads=(310 * 1000000),
@@ -1351,15 +1350,16 @@
     ]
     customer: Customer = (base_store.get_customers())[0]
     external_app = base_store.get_application_by_tag("WGXCUSC000").versions[0]
     wgs_app = base_store.get_application_by_tag("WGSPCFC030").versions[0]
     for sample in new_samples:
         sample.customer = customer
         sample.application_version = external_app if "external" in sample.name else wgs_app
-    base_store.add_commit(new_samples)
+    base_store.session.add_all(new_samples)
+    base_store.session.commit()
     return base_store
 
 
 @pytest.fixture(name="trailblazer_api")
 def fixture_trailblazer_api() -> MockTB:
     """Return a mock Trailblazer API."""
     return MockTB()
@@ -1805,15 +1805,16 @@
     ]
 
     organisms: List[Organism] = []
     for internal_id, name in organism_details:
         organism: Organism = helpers.add_organism(store, internal_id=internal_id, name=name)
         organisms.append(organism)
 
-    store.add_commit(organisms)
+    store.session.add_all(organisms)
+    store.session.commit()
     yield store
 
 
 @pytest.fixture(name="ok_response")
 def fixture_ok_response() -> Response:
     """Return a response with the OK status code."""
     response: Response = Response()
@@ -1852,15 +1853,15 @@
         ("user2@example.com", "User Two", True),
         ("user3@example.com", "User Three", False),
     ]
 
     for email, name, is_admin in user_details:
         store.add_user(customer=customer, email=email, name=name, is_admin=is_admin)
 
-    store.commit()
+    store.session.commit()
 
     yield store
 
 
 @pytest.fixture(name="store_with_cases_and_customers")
 def fixture_store_with_cases_and_customers(store: Store, helpers: StoreHelpers) -> Store:
     """Return a store with cases and customers."""
@@ -1895,9 +1896,9 @@
             store=store,
             case_name=case_name,
             case_id=case_id,
             data_analysis=pipeline.value,
             action=action.value,
             customer=customer,
         )
-    store.commit()
+    store.session.commit()
     yield store
```

### Comparing `cg-29.0.3/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml` & `cg-29.1.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-29.1.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-29.1.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/analysis/sample_coverage.bed` & `cg-29.1.0/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/balsamic/case/config.json` & `cg-29.1.0/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-29.1.0/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-29.1.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-29.1.0/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml` & `cg-29.1.0/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-29.1.0/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-29.1.0/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/madeline/madeline.xml` & `cg-29.1.0/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-29.1.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-29.1.0/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-29.1.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-29.1.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-29.1.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-29.1.0/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-29.1.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-29.1.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-29.1.0/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-29.1.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-29.1.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/scout/643594.config.yaml` & `cg-29.1.0/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/scout/case_export.json` & `cg-29.1.0/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/scout/export_causatives.json` & `cg-29.1.0/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/scout/none_case_export.json` & `cg-29.1.0/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/scout/other_sex_case.json` & `cg-29.1.0/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/scout/panel_export.bed` & `cg-29.1.0/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/apps/scout/panel_export.csv` & `cg-29.1.0/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/cgweb_orders/balsamic.json` & `cg-29.1.0/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/cgweb_orders/fastq.json` & `cg-29.1.0/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/cgweb_orders/metagenome.json` & `cg-29.1.0/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/cgweb_orders/microsalt.json` & `cg-29.1.0/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/cgweb_orders/mip.json` & `cg-29.1.0/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-29.1.0/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/cgweb_orders/rml.json` & `cg-29.1.0/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-29.1.0/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/data/SampleSheet.csv` & `cg-29.1.0/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/data/cgfixture.db` & `cg-29.1.0/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/data/hkstore.db` & `cg-29.1.0/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/io/example_json.json` & `cg-29.1.0/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/1508.27.balsamic.xlsx` & `cg-29.1.0/tests/fixtures/orderforms/1508.27.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx` & `cg-29.1.0/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx` & `cg-29.1.0/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/1508.27.fastq.xlsx` & `cg-29.1.0/tests/fixtures/orderforms/1508.27.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/1508.27.mip.xlsx` & `cg-29.1.0/tests/fixtures/orderforms/1508.27.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/1508.27.mip_rna.xlsx` & `cg-29.1.0/tests/fixtures/orderforms/1508.27.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-29.1.0/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/1604.15.rml.xlsx` & `cg-29.1.0/tests/fixtures/orderforms/1604.15.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/1605.10.metagenome.xlsx` & `cg-29.1.0/tests/fixtures/orderforms/1605.10.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/2184.7.sarscov2.xlsx` & `cg-29.1.0/tests/fixtures/orderforms/2184.7.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/NIPT-json.json` & `cg-29.1.0/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-29.1.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-29.1.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/report/case_data.json` & `cg-29.1.0/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/report/lims_exported_samples.json` & `cg-29.1.0/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/fixtures/report/lims_family.json` & `cg-29.1.0/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/io/conftest.py` & `cg-29.1.0/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/io/test_io_controller.py` & `cg-29.1.0/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/io/test_io_csv.py` & `cg-29.1.0/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/io/test_io_json.py` & `cg-29.1.0/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/io/test_io_yaml.py` & `cg-29.1.0/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/archive/conftest.py` & `cg-29.1.0/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/archive/test_archiving.py` & `cg-29.1.0/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/backup/conftest.py` & `cg-29.1.0/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/backup/test_meta_backup.py` & `cg-29.1.0/tests/meta/backup/test_meta_backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
     assert (
         f"Status for flow cell {mock_get_first_flow_cell.return_value.name} set to "
         f"{FlowCellStatus.RETRIEVED}" in caplog.text
     )
     assert mock_flow_cell.status == "retrieved"
 
     # AND status-db is updated with the new status
-    assert mock_store.commit.called
+    assert mock_store.session.commit.called
 
     # AND the elapsed time of the retrieval process is returned
     assert result > 0
 
 
 @mock.patch("cg.meta.backup.backup.BackupAPI.unlink_files")
 @mock.patch("cg.meta.backup.backup.BackupAPI.create_rta_complete")
@@ -287,15 +287,15 @@
     assert (
         f"Status for flow cell {mock_flow_cell.name} set to {FlowCellStatus.RETRIEVED}"
         in caplog.text
     )
     assert mock_flow_cell.status == "retrieved"
 
     # AND status-db is updated with the new status
-    assert mock_store.commit.called
+    assert mock_store.session.commit.called
 
     # AND the elapsed time of the retrieval process is returned
     assert result > 0
 
 
 @mock.patch("cg.meta.backup.backup.BackupAPI.unlink_files")
 @mock.patch("cg.meta.backup.backup.BackupAPI.create_rta_complete")
@@ -397,15 +397,15 @@
     assert (
         f"Status for flow cell {mock_flow_cell.name} set to {FlowCellStatus.RETRIEVED}"
         in caplog.text
     )
     assert mock_flow_cell.status == "retrieved"
 
     # AND status-db is updated with the new status
-    assert mock_store.commit.called
+    assert mock_store.session.commit.called
 
     # AND the elapsed time of the retrieval process is returned
     assert result > 0
 
 
 @mock.patch("cg.meta.backup.backup.SpringBackupAPI.is_spring_file_archived")
 @mock.patch("cg.meta.backup.backup.SpringBackupAPI.remove_archived_spring_file")
```

### Comparing `cg-29.0.3/tests/meta/backup/test_meta_pdc.py` & `cg-29.1.0/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/clean/conftest.py` & `cg-29.1.0/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/clean/test_clean_demultiplexed_runs.py` & `cg-29.1.0/tests/meta/clean/test_clean_demultiplexed_runs.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/clean/test_clean_flow_cell_run_directories.py` & `cg-29.1.0/tests/meta/clean/test_clean_flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/compress/conftest.py` & `cg-29.1.0/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/compress/test_clean_fastq.py` & `cg-29.1.0/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/compress/test_compress_files.py` & `cg-29.1.0/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/compress/test_compress_meta_fastq.py` & `cg-29.1.0/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/compress/test_decompress_spring_meta.py` & `cg-29.1.0/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-29.1.0/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/conftest.py` & `cg-29.1.0/tests/meta/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,16 +222,16 @@
         ).versions[0]
         sample: Sample = base_store.add_sample(
             name="NA", sex="male", internal_id=sample_data["name"]
         )
         sample.customer = customer
         sample.application_version = application_version
         sample.received_at = dt.datetime.now()
-        base_store.add(sample)
-    base_store.commit()
+        base_store.session.add(sample)
+    base_store.session.commit()
     yield base_store
 
 
 @pytest.fixture(name="transfer_flow_cell_api")
 def fixture_transfer_flow_cell_api(
     flowcell_store: Store, housekeeper_api: MockHousekeeperAPI, base_store_stats: StatsAPI
 ) -> Generator[TransferFlowCell, None, None]:
@@ -263,15 +263,15 @@
     store: Store,
     lims_api: MockLimsAPI,
     helpers: StoreHelpers,
     invoice_id: int = 0,
     customer_id: str = CustomerNames.cust032,
 ) -> InvoiceAPI:
     """Return an InvoiceAPI with a pool for NIPT customer."""
-    pool = helpers.ensure_pool(store, customer_id=customer_id)
+    pool = helpers.ensure_pool(store=store, customer_id=customer_id)
     invoice: Invoice = helpers.ensure_invoice(
         store,
         invoice_id=invoice_id,
         customer_id=customer_id,
         pools=[pool],
     )
     return InvoiceAPI(store, lims_api, invoice)
@@ -283,15 +283,15 @@
     lims_api: MockLimsAPI,
     helpers: StoreHelpers,
     invoice_id: int = 0,
     record_type: str = RecordType.Pool,
     customer_id: str = CustomerNames.cust132,
 ) -> InvoiceAPI:
     """Return an InvoiceAPI with a pool."""
-    pool = helpers.ensure_pool(store, customer_id=customer_id)
+    pool = helpers.ensure_pool(store=store, customer_id=customer_id)
     invoice: Invoice = helpers.ensure_invoice(
         store,
         invoice_id=invoice_id,
         pools=[pool],
         customer_id=customer_id,
     )
     return InvoiceAPI(store, lims_api, invoice)
```

### Comparing `cg-29.0.3/tests/meta/deliver/conftest.py` & `cg-29.1.0/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/deliver/test_deliver_ticket.py` & `cg-29.1.0/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/deliver/test_delivery_api.py` & `cg-29.1.0/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/demultiplex/conftest.py` & `cg-29.1.0/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/demultiplex/test_delete_demultiplex_api.py` & `cg-29.1.0/tests/meta/demultiplex/test_delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-29.1.0/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/demultiplex/test_rename_files.py` & `cg-29.1.0/tests/meta/demultiplex/test_rename_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/encryption/conftest.py` & `cg-29.1.0/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/encryption/test_encryption.py` & `cg-29.1.0/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/observations/conftest.py` & `cg-29.1.0/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/observations/test_meta_upload_observations.py` & `cg-29.1.0/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/orders/conftest.py` & `cg-29.1.0/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-29.1.0/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,13 +32,14 @@
         case = helpers.ensure_case(
             store=base_store,
             case_name=PoolSubmitter.create_case_name(ticket=order.ticket, pool_name=sample.pool),
             customer=customer,
             data_analysis=Pipeline.FLUFFY,
             data_delivery=DataDelivery.STATINA,
         )
-        base_store.add_commit(case)
+        base_store.session.add(case)
+        base_store.session.commit()
 
     # WHEN validating the order
     # THEN it should be regarded as invalid
     with pytest.raises(OrderError):
         PoolSubmitter(status=base_store, lims=None).validate_order(order=order)
```

### Comparing `cg-29.0.3/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-29.1.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-29.1.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-29.1.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/orders/test_meta_orders_api.py` & `cg-29.1.0/tests/meta/orders/test_meta_orders_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -150,19 +150,19 @@
     new_customer = sample_store.add_customer(
         "customer999",
         "customer 999",
         scout_access=True,
         invoice_address="dummy street",
         invoice_reference="dummy nr",
     )
-    sample_store.add_commit(new_customer)
+    sample_store.session.add(new_customer)
     existing_sample: Sample = sample_store.get_samples()[0]
     existing_sample.customer = new_customer
-    sample_store.add_commit(existing_sample)
-
+    sample_store.session.add(existing_sample)
+    sample_store.session.commit()
     for sample in order_data.samples:
         sample.internal_id = existing_sample.internal_id
 
     # WHEN calling submit
     # THEN an OrderError should be raised on illegal customer
     with pytest.raises(OrderError):
         orders_api.submit(
@@ -189,15 +189,15 @@
     user_name: str,
 ):
     order_data = OrderIn.parse_obj(obj=all_orders_to_submit[order_type], project=order_type)
     monkeypatch_process_lims(monkeypatch, order_data)
     # GIVEN we have an order with a customer that is in the same customer group as customer
     # that the samples originate from
     collaboration = sample_store.add_collaboration("customer999only", "customer 999 only group")
-    sample_store.add_commit(collaboration)
+    sample_store.session.add(collaboration)
     sample_customer = sample_store.add_customer(
         "customer1",
         "customer 1",
         scout_access=True,
         invoice_address="dummy street 1",
         invoice_reference="dummy nr",
     )
@@ -206,19 +206,19 @@
         "customer 2",
         scout_access=True,
         invoice_address="dummy street 2",
         invoice_reference="dummy nr",
     )
     sample_customer.collaborations.append(collaboration)
     order_customer.collaborations.append(collaboration)
-    sample_store.add_commit(sample_customer)
-    sample_store.add_commit(order_customer)
+    sample_store.session.add(sample_customer)
+    sample_store.session.add(order_customer)
     existing_sample: Sample = sample_store.get_samples()[0]
     existing_sample.customer = sample_customer
-    sample_store.commit()
+    sample_store.session.commit()
     order_data.customer = order_customer.internal_id
 
     for sample in order_data.samples:
         sample.internal_id = existing_sample.internal_id
         break
 
     # WHEN calling submit
@@ -252,15 +252,16 @@
             case: Family = store.add_case(
                 data_analysis=Pipeline.MIP_DNA,
                 data_delivery=DataDelivery.SCOUT,
                 name=case_id,
                 ticket=ticket_id,
             )
             case.customer = customer
-            store.add_commit(case)
+            store.session.add(case)
+        store.session.commit()
         assert store.get_case_by_name_and_customer(customer=customer, case_name=case_id)
 
     monkeypatch_process_lims(monkeypatch, order_data)
 
     # WHEN calling submit
     # THEN an OrderError should be raised on duplicate case name
     with pytest.raises(OrderError):
@@ -356,15 +357,16 @@
         sample_obj: Sample = helpers.add_sample(
             store=store,
             subject_id=sample.subject_id,
             name=sample.name,
             gender="male" if sample.sex == "female" else "female",
             customer_id=customer.internal_id,
         )
-        store.add_commit(sample_obj)
+        store.session.add(sample_obj)
+        store.session.commit()
         assert sample_obj.sex != sample.sex
 
     submitter: MipDnaSubmitter = MipDnaSubmitter(lims=orders_api.lims, status=orders_api.status)
 
     # WHEN calling _validate_sex
     # THEN an OrderError should be raised on non-matching sex
     with pytest.raises(OrderError):
@@ -385,15 +387,16 @@
         sample_obj: Sample = helpers.add_sample(
             store=store,
             subject_id=sample.subject_id,
             name=sample.name,
             gender=sample.sex,
             customer_id=customer.internal_id,
         )
-        store.add_commit(sample_obj)
+        store.session.add(sample_obj)
+        store.session.commit()
         assert sample_obj.sex == sample.sex
 
     submitter: MipDnaSubmitter = MipDnaSubmitter(lims=orders_api.lims, status=orders_api.status)
 
     # WHEN calling _validate_sex
     submitter._validate_subject_sex(samples=order_data.samples, customer_id=order_data.customer)
 
@@ -415,15 +418,16 @@
         sample_obj: Sample = helpers.add_sample(
             store=store,
             subject_id=sample.subject_id,
             name=sample.name,
             gender="unknown",
             customer_id=customer.internal_id,
         )
-        store.add_commit(sample_obj)
+        store.session.add(sample_obj)
+        store.session.commit()
         assert sample_obj.sex != sample.sex
 
     submitter: MipDnaSubmitter = MipDnaSubmitter(lims=orders_api.lims, status=orders_api.status)
 
     # WHEN calling _validate_sex
     submitter._validate_subject_sex(samples=order_data.samples, customer_id=order_data.customer)
 
@@ -445,15 +449,16 @@
             store=store,
             subject_id=sample.subject_id,
             name=sample.name,
             gender=sample.sex,
             customer_id=customer.internal_id,
         )
         sample.sex = "unknown"
-        store.add_commit(sample_obj)
+        store.session.add(sample_obj)
+        store.session.commit()
 
     for sample in order_data.samples:
         assert sample_obj.sex != sample.sex
 
     submitter: MipDnaSubmitter = MipDnaSubmitter(lims=orders_api.lims, status=orders_api.status)
 
     # WHEN calling _validate_sex
@@ -538,15 +543,16 @@
         sample_name = sample.name
         if not store.get_sample_by_customer_and_name(
             customer_entry_id=[customer.id], sample_name=sample_name
         ):
             sample_obj = helpers.add_sample(
                 store=store, name=sample_name, customer_id=customer.internal_id
             )
-            store.add_commit(sample_obj)
+            store.session.add(sample_obj)
+            store.session.commit()
 
 
 @patch("cg.meta.orders.ticket_handler.FormDataRequest.submit", return_value=None)
 @pytest.mark.parametrize(
     "order_type",
     [
         OrderType.BALSAMIC,
```

### Comparing `cg-29.0.3/tests/meta/orders/test_meta_orders_lims.py` & `cg-29.1.0/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/orders/test_meta_orders_status.py` & `cg-29.1.0/tests/meta/orders/test_meta_orders_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from cg.meta.orders.mip_rna_submitter import MipRnaSubmitter
 from cg.meta.orders.rml_submitter import RmlSubmitter
 from cg.meta.orders.sars_cov_2_submitter import SarsCov2Submitter
 from cg.meta.orders.submitter import Submitter
 from cg.models.orders.order import OrderIn, OrderType
 from cg.meta.orders import OrdersAPI
 from cg.store import Store
-from cg.store.models import Family, Pool
+from cg.store.models import Delivery, Family, Pool
 from cg.constants import Priority
 
 
 def test_pools_to_status(rml_order_to_submit):
     # GIVEN a rml order with three samples in one pool
     order = OrderIn.parse_obj(rml_order_to_submit, OrderType.RML)
 
@@ -526,15 +526,15 @@
 
     assert set(new_link.sample.phenotype_groups) == {"Phenotype-group"}
     assert set(new_link.sample.phenotype_terms) == {"HP:0012747", "HP:0025049"}
     assert new_link.sample.subject_id == "subject1"
 
     assert new_link.sample.age_at_sampling == 17.18192
 
-    assert base_store.deliveries().count() == len(base_store.get_samples())
+    assert base_store._get_query(table=Delivery).count() == len(base_store.get_samples())
     for link in new_case.links:
         assert len(link.sample.deliveries) == 1
 
 
 def test_store_mip_rna(orders_api, base_store, mip_rna_status_data, ticket_id: str):
     # GIVEN a basic store with no samples or nothing in it + rna order
     rna_application_tag = "RNAPOAR025"
@@ -608,15 +608,15 @@
         )
 
 
 @pytest.mark.parametrize(
     "submitter", [BalsamicSubmitter, BalsamicQCSubmitter, BalsamicUmiSubmitter]
 )
 def test_store_cancer_samples(
-    orders_api, base_store, balsamic_status_data, submitter, ticket_id: str
+    orders_api, base_store: Store, balsamic_status_data, submitter, ticket_id: str
 ):
     # GIVEN a basic store with no samples and a cancer order
     assert not base_store.get_samples()
     assert not base_store.get_cases()
 
     submitter: Submitter = submitter(lims=orders_api.lims, status=orders_api.status)
 
@@ -646,15 +646,15 @@
     new_link = new_case.links[0]
     assert new_link.sample.name == "s1"
     assert new_link.sample.sex == "male"
     assert new_link.sample.application_version.application.tag == "WGSPCFC030"
     assert new_link.sample.comment == "other Elution buffer"
     assert new_link.sample.is_tumour
 
-    assert base_store.deliveries().count() == len(base_store.get_samples())
+    assert base_store._get_query(table=Delivery).count() == len(base_store.get_samples())
     for link in new_case.links:
         assert len(link.sample.deliveries) == 1
 
 
 def test_store_existing_single_sample_from_trio(
     orders_api, base_store, mip_status_data, ticket_id: str
 ):
@@ -727,29 +727,29 @@
         customer_id=mip_status_data["customer"],
         order=mip_status_data["order"],
         ordered=dt.datetime.now(),
         ticket_id=ticket_id,
         items=mip_status_data["families"],
     )
 
-    base_store.close()
+    base_store.session.close()
     new_cases: List[Family] = base_store.get_cases()
 
     # Save internal id
-    stored_cases_internal_ids = dict([(case["name"], case["internal_id"]) for case in new_cases])
+    stored_cases_internal_ids = dict([(case.name, case.internal_id) for case in new_cases])
     for case in mip_status_data["families"]:
         case["internal_id"] = stored_cases_internal_ids[case["name"]]
 
     submitter.store_items_in_status(
         customer_id=mip_status_data["customer"],
         order=mip_status_data["order"],
         ordered=dt.datetime.now(),
         ticket_id=ticket_id,
         items=mip_status_data["families"],
     )
 
-    base_store.close()
+    base_store.session.close()
     rerun_cases: List[Family] = base_store.get_cases()
 
     # THEN the sample ticket should be appended to previos ticket and action set to analyze
     assert rerun_cases[0].tickets == f"{ticket_id},{ticket_id}"
     assert rerun_cases[0].action == CaseActions.ANALYZE
```

### Comparing `cg-29.0.3/tests/meta/orders/test_ticket_handler.py` & `cg-29.1.0/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/report/conftest.py` & `cg-29.1.0/tests/meta/report/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,35 +12,35 @@
 from cg.meta.report.mip_dna import MipDNAReportAPI
 from cg.models.cg_config import CGConfig
 from cg.store.models import Family
 from tests.apps.scout.conftest import MockScoutApi
 from tests.mocks.balsamic_analysis_mock import MockBalsamicAnalysis
 from tests.mocks.limsmock import MockLimsAPI
 from tests.mocks.mip_analysis_mock import MockMipAnalysis
-from tests.mocks.report import MockChanjo, MockDB, MockHousekeeperMipDNAReportAPI
+from tests.mocks.report import MockChanjo, MockHousekeeperMipDNAReportAPI
 
 
 @pytest.fixture(scope="function", name="report_api_mip_dna")
-def report_api_mip_dna(cg_context: CGConfig, lims_samples) -> MipDNAReportAPI:
+def report_api_mip_dna(cg_context: CGConfig, lims_samples, report_store) -> MipDNAReportAPI:
     """MIP DNA ReportAPI fixture."""
 
     cg_context.meta_apis["analysis_api"] = MockMipAnalysis()
-    cg_context.status_db_ = MockDB(report_store)
+    cg_context.status_db_ = report_store
     cg_context.lims_api_ = MockLimsAPI(cg_context, lims_samples)
     cg_context.chanjo_api_ = MockChanjo()
     cg_context.scout_api_ = MockScoutApi(cg_context)
     return MockHousekeeperMipDNAReportAPI(cg_context, cg_context.meta_apis["analysis_api"])
 
 
 @pytest.fixture(scope="function", name="report_api_balsamic")
-def report_api_balsamic(cg_context: CGConfig, lims_samples) -> BalsamicReportAPI:
+def report_api_balsamic(cg_context: CGConfig, lims_samples, report_store) -> BalsamicReportAPI:
     """BALSAMIC ReportAPI fixture."""
 
     cg_context.meta_apis["analysis_api"] = MockBalsamicAnalysis(cg_context)
-    cg_context.status_db_ = MockDB(report_store)
+    cg_context.status_db_ = report_store
     cg_context.lims_api_ = MockLimsAPI(cg_context, lims_samples)
     cg_context.scout_api_ = MockScoutApi(cg_context)
     return BalsamicReportAPI(cg_context, cg_context.meta_apis["analysis_api"])
 
 
 @pytest.fixture(scope="function", name="case_mip_dna")
 def case_mip_dna(case_id, report_api_mip_dna) -> Family:
```

### Comparing `cg-29.0.3/tests/meta/report/test_balsamic_api.py` & `cg-29.1.0/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/report/test_field_validators.py` & `cg-29.1.0/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/report/test_mip_dna_api.py` & `cg-29.1.0/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/report/test_report_api.py` & `cg-29.1.0/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/rsync/conftest.py` & `cg-29.1.0/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/rsync/test_rsync.py` & `cg-29.1.0/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/test_invoice.py` & `cg-29.1.0/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/transfer/conftest.py` & `cg-29.1.0/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/transfer/test_external_data.py` & `cg-29.1.0/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/transfer/test_meta_transfer_flowcell.py` & `cg-29.1.0/tests/meta/transfer/test_meta_transfer_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-29.1.0/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/balsamic/test_balsamic.py` & `cg-29.1.0/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/conftest.py` & `cg-29.1.0/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/gisaid/conftest.py` & `cg-29.1.0/tests/meta/upload/gisaid/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-29.1.0/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/mutacc/conftest.py` & `cg-29.1.0/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-29.1.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/nipt/conftest.py` & `cg-29.1.0/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-29.1.0/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/scout/conftest.py` & `cg-29.1.0/tests/meta/upload/scout/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
     helpers.add_relationship(
         store=store, sample=dna_sample_father, case=dna_case, status="affected"
     )
 
     for link in dna_case.links:
         link.sample.internal_id = link.sample.name
 
-    store.commit()
+    store.session.commit()
     return store
 
 
 @pytest.fixture(name="lims_family")
 def fixture_lims_family(fixtures_dir) -> dict:
     """Returns a LIMS-like case of samples."""
     return ReadFile.get_content_from_file(
```

### Comparing `cg-29.0.3/tests/meta/upload/scout/test_generate_load_config.py` & `cg-29.1.0/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-29.1.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-29.1.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests for RNA part of the scout upload API"""
 import logging
 from typing import Generator, List
 import pytest
 from _pytest.logging import LogCaptureFixture
 
-from alchy import Query
+from sqlalchemy.orm import Query
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants import Pipeline
 from cg.constants.sequencing import SequencingMethod
 from cg.exc import CgDataError
 from cg.meta.upload.scout.uploadscoutapi import UploadScoutAPI
 from cg.store.models import Family, Sample
 import cg.store as Store
@@ -44,15 +44,15 @@
         name=another_sample_id,
         subject_id=subject_id,
         is_tumour=True,
         application_tag=SequencingMethod.WGS,
         application_type=SequencingMethod.WGS,
     )
     helpers.add_relationship(store=rna_store, sample=another_sample_id, case=dna_extra_case)
-    rna_store.commit()
+    rna_store.session.commit()
 
 
 def ensure_extra_rna_case_match(
     another_rna_sample_id: str,
     helpers: StoreHelpers,
     rna_case_id: str,
     rna_store: Store,
@@ -252,15 +252,15 @@
     """Test that A RNA case's gene fusion report"""
 
     # GIVEN a sample in the RNA case is NOT connected to a sample in the DNA case via subject_id (i.e. same subject_id)
     for link in rna_store.get_case_by_internal_id(rna_case_id).links:
         link.sample.subject_id = ""
     for link in rna_store.get_case_by_internal_id(dna_case_id).links:
         link.sample.subject_id = ""
-    rna_store.commit()
+    rna_store.session.commit()
     upload_scout_api.status_db = rna_store
 
     # GIVEN the connected RNA case has a research fusion report in Housekeeper
 
     # WHEN running the method to upload RNA files to Scout
     caplog.set_level(logging.INFO)
     # THEN an exception should be raised on unconnected data
@@ -280,15 +280,15 @@
     command into an already existing DNA case"""
 
     # GIVEN a sample in the RNA case is NOT connected to a sample in the DNA case via subject_id (i.e. same subject_id)
     for link in rna_store.get_case_by_internal_id(rna_case_id).links:
         link.sample.subject_id = ""
     for link in rna_store.get_case_by_internal_id(dna_case_id).links:
         link.sample.subject_id = ""
-    rna_store.commit()
+    rna_store.session.commit()
     upload_scout_api.status_db = rna_store
 
     # GIVEN the connected RNA sample has a bigWig in Housekeeper
 
     # WHEN running the method to upload RNA files to Scout
     caplog.set_level(logging.INFO)
     # THEN an exception should be raised on unconnected data
@@ -308,15 +308,15 @@
     command into an already existing DNA case"""
 
     # GIVEN a sample in the RNA case is NOT connected to a sample in the DNA case via subject_id (i.e. same subject_id)
     for link in rna_store.get_case_by_internal_id(rna_case_id).links:
         link.sample.subject_id = ""
     for link in rna_store.get_case_by_internal_id(dna_case_id).links:
         link.sample.subject_id = ""
-    rna_store.commit()
+    rna_store.session.commit()
     upload_scout_api.status_db = rna_store
 
     # GIVEN the connected RNA sample has a junction bed in Housekeeper
 
     # WHEN running the method to upload RNA files to Scout
     caplog.set_level(logging.INFO)
     # THEN an exception should be raised on unconnected data
@@ -333,15 +333,15 @@
     upload_scout_api: UploadScoutAPI,
 ):
     """Test that an RNA case's gene fusion report is not uploaded if the is_tumour is not matching"""
 
     # GIVEN a sample in the RNA case is NOT connected to a sample in the DNA case via is_tumour (i.e. different is_tumour)
     set_is_tumour_on_case(store=rna_store, case_id=rna_case_id, is_tumour=True)
     set_is_tumour_on_case(store=rna_store, case_id=dna_case_id, is_tumour=False)
-    rna_store.commit()
+    rna_store.session.commit()
     upload_scout_api.status_db = rna_store
 
     # GIVEN the connected RNA case has a research fusion report in Housekeeper
 
     # WHEN running the method to upload RNA files to Scout
     caplog.set_level(logging.INFO)
 
@@ -359,15 +359,15 @@
     upload_scout_api: UploadScoutAPI,
 ):
     """Test that A RNA case's gene fusion report and junction splice files for all samples is not uploaded if the is_tumour is not matching"""
 
     # GIVEN a sample in the RNA case is NOT connected to a sample in the DNA case via is_tumour (i.e. different is_tumour)
     set_is_tumour_on_case(store=rna_store, case_id=rna_case_id, is_tumour=True)
     set_is_tumour_on_case(store=rna_store, case_id=dna_case_id, is_tumour=False)
-    rna_store.commit()
+    rna_store.session.commit()
     upload_scout_api.status_db = rna_store
 
     # GIVEN the connected RNA sample has a bigWig in Housekeeper
 
     # WHEN running the method to upload RNA files to Scout
     caplog.set_level(logging.INFO)
 
@@ -385,15 +385,15 @@
     upload_scout_api: UploadScoutAPI,
 ):
     """Test that A RNA case's junction splice files for all samples is not uploaded if the is_tumour is not matching"""
 
     # GIVEN a sample in the RNA case is NOT connected to a sample in the DNA case via is_tumour (i.e. different is_tumour)
     set_is_tumour_on_case(store=rna_store, case_id=rna_case_id, is_tumour=True)
     set_is_tumour_on_case(store=rna_store, case_id=dna_case_id, is_tumour=False)
-    rna_store.commit()
+    rna_store.session.commit()
     upload_scout_api.status_db = rna_store
 
     # GIVEN the connected RNA sample has a junction bed in Housekeeper
 
     # WHEN running the method to upload RNA files to Scout
     caplog.set_level(logging.INFO)
```

### Comparing `cg-29.0.3/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-29.1.0/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/test_meta_upload_coverage.py` & `cg-29.1.0/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/test_upload_api.py` & `cg-29.1.0/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/test_upload_genotypes_api.py` & `cg-29.1.0/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/vogue/conftest.py` & `cg-29.1.0/tests/meta/upload/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/upload/vogue/test_upload_vogue.py` & `cg-29.1.0/tests/meta/upload/vogue/test_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/workflow/conftest.py` & `cg-29.1.0/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/workflow/test_analysis.py` & `cg-29.1.0/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/workflow/test_balsamic.py` & `cg-29.1.0/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/workflow/test_microsalt.py` & `cg-29.1.0/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-29.1.0/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/mocks/balsamic_analysis_mock.py` & `cg-29.1.0/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/mocks/crunchy.py` & `cg-29.1.0/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/mocks/hk_mock.py` & `cg-29.1.0/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/mocks/limsmock.py` & `cg-29.1.0/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/mocks/madeline.py` & `cg-29.1.0/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/mocks/mip_analysis_mock.py` & `cg-29.1.0/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/mocks/osticket.py` & `cg-29.1.0/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/mocks/process_mock.py` & `cg-29.1.0/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/mocks/report.py` & `cg-29.1.0/tests/mocks/report.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,21 +93,14 @@
             analysis_date,
             force_report,
         )
 
         return file_path
 
 
-class MockDB(Store):
-    """Mock database"""
-
-    def __init__(self, store):
-        self.store = store
-
-
 class MockChanjo(ChanjoAPI):
     """Chanjo mock class"""
 
     def __init__(self):
         mock_config = {"chanjo": {"config_path": "/mock/path", "binary_path": "/mock/path"}}
         super().__init__(mock_config)
```

### Comparing `cg-29.0.3/tests/mocks/scout.py` & `cg-29.1.0/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/mocks/store_model.py` & `cg-29.1.0/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/mocks/tb_mock.py` & `cg-29.1.0/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/balsamic/conftest.py` & `cg-29.1.0/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/balsamic/test_balsamic_analysis.py` & `cg-29.1.0/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/conftest.py` & `cg-29.1.0/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/demultiplexing/conftest.py` & `cg-29.1.0/tests/models/demultiplexing/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/demultiplexing/test_demux_results.py` & `cg-29.1.0/tests/models/demultiplexing/test_demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/demultiplexing/test_flowcell_model.py` & `cg-29.1.0/tests/models/demultiplexing/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/mip/conftest.py` & `cg-29.1.0/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/mip/test_mip_analysis.py` & `cg-29.1.0/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/mip/test_mip_config.py` & `cg-29.1.0/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-29.1.0/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/mip/test_mip_sample_info.py` & `cg-29.1.0/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/nextflow/conftest.py` & `cg-29.1.0/tests/models/nextflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/nextflow/test_nextflow_deliver.py` & `cg-29.1.0/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/observations/conftest.py` & `cg-29.1.0/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/observations/test_observations_input_files.py` & `cg-29.1.0/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/report/test_validators.py` & `cg-29.1.0/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/rnafusion/conftest.py` & `cg-29.1.0/tests/models/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-29.1.0/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/test_cg_models.py` & `cg-29.1.0/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/test_compression_data.py` & `cg-29.1.0/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/test_file_data.py` & `cg-29.1.0/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/models/test_flowcell_class.py` & `cg-29.1.0/tests/models/test_flowcell_class.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/server/conftest.py` & `cg-29.1.0/tests/server/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Test fixtures for cg/server tests"""
 import os
 
 import pytest
 
 from cg.server.app import create_app
 
-os.environ["CG_SQL_DATABASE_URI"] = "dummy_value"
+os.environ["CG_SQL_DATABASE_URI"] = "sqlite:///:memory:"
 os.environ["LIMS_HOST"] = "dummy_value"
 os.environ["LIMS_USERNAME"] = "dummy_value"
 os.environ["LIMS_PASSWORD"] = "dummy_value"
 os.environ["GOOGLE_OAUTH_CLIENT_ID"] = "dummy_value"
 os.environ["GOOGLE_OAUTH_CLIENT_SECRET"] = "dummy_value"
```

### Comparing `cg-29.0.3/tests/store/api/add/test_store_add_application_version.py` & `cg-29.1.0/tests/store/api/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/api/add/test_store_add_base.py` & `cg-29.1.0/tests/store/api/add/test_store_add_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,36 +8,38 @@
     # GIVEN an empty database
     collaboration_query = store._get_query(table=Collaboration)
     assert collaboration_query.first() is None
     internal_id, name = "cust_group", "Test customer group"
 
     # WHEN adding a new customer group
     new_collaboration = store.add_collaboration(internal_id=internal_id, name=name)
-    store.add_commit(new_collaboration)
+    store.session.add(new_collaboration)
+    store.session.commit()
 
     # THEN it should be stored in the database
     assert collaboration_query.first() == new_collaboration
 
 
 def test_add_user(store: Store):
     # GIVEN a database with a customer in it that we can connect the user to
     customer = store.add_customer(
         internal_id="custtest",
         name="Test Customer",
         scout_access=False,
         invoice_address="dummy street 1",
         invoice_reference="dummy nr",
     )
-    store.add_commit(customer)
+    store.session.add(customer)
 
     # WHEN adding a new user
     name, email = "Paul T. Anderson", "paul.anderson@magnolia.com"
     new_user = store.add_user(customer=customer, email=email, name=name)
 
-    store.add_commit(new_user)
+    store.session.add(new_user)
+    store.session.commit()
 
     # THEN it should be stored in the database
     assert store._get_query(table=User).first() == new_user
 
 
 def test_add_microbial_sample(base_store: Store, helpers):
     # GIVEN an empty database
@@ -61,15 +63,16 @@
         internal_id=internal_id,
         priority=priority,
         application_version=application_version,
         organism=organism,
         reference_genome=reference_genome,
     )
     new_sample.customer = customer_obj
-    base_store.add_commit(new_sample)
+    base_store.session.add(new_sample)
+    base_store.session.commit()
 
     # THEN it should be stored in the database
     assert sample_query.first() == new_sample
     stored_microbial_sample = sample_query.first()
     assert stored_microbial_sample.name == name
     assert stored_microbial_sample.internal_id == internal_id
     assert stored_microbial_sample.reference_genome == reference_genome
@@ -92,11 +95,12 @@
         customer=customer,
         name="pool2",
         order="123456",
         ordered=dt.now(),
         application_version=app_version,
     )
 
-    rml_pool_store.add_commit(new_pool)
+    rml_pool_store.session.add(new_pool)
+    rml_pool_store.session.commit()
     # THEN the new pool should have no_invoice = False
     pool = rml_pool_store.get_pool_by_entry_id(entry_id=2)
     assert pool.no_invoice is False
```

### Comparing `cg-29.0.3/tests/store/api/add/test_store_add_customer.py` & `cg-29.1.0/tests/store/api/add/test_store_add_customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
         invoice_address="dummy street 1",
         invoice_reference="dummy nr",
     )
     new_user = store.add_user(new_customer, contact_email, contact_name)
 
     contact_field = f"{contact_type}_contact"
     setattr(new_customer, contact_field, new_user)
-    store.add_commit(new_customer)
+    store.session.add(new_customer)
+    store.session.commit()
 
     # THEN contact should be stored on the customer
     assert (
         getattr(store.get_customer_by_internal_id(customer_internal_id=internal_id), contact_field)
         == new_user
     )
 
@@ -58,11 +59,12 @@
         internal_id=internal_id,
         name=name,
         scout_access=scout_access,
         invoice_address="dummy street 1",
         invoice_reference="dummy nr",
     )
     new_customer.collaborations.append(collaboration)
-    store.add_commit(new_customer)
+    store.session.add(new_customer)
+    store.session.commit()
 
     # THEN it should be stored in the database
     assert (store._get_query(table=Customer)).first() == new_customer
```

### Comparing `cg-29.0.3/tests/store/api/add/test_store_add_flow_celll.py` & `cg-29.1.0/tests/store/api/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/api/conftest.py` & `cg-29.1.0/tests/store/api/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,64 +97,65 @@
     new_customer = store.add_customer(
         internal_id=customer_id,
         name="Test customer",
         scout_access=True,
         invoice_address="skolgatan 15",
         invoice_reference="abc",
     )
-    store.add_commit(new_customer)
+    store.session.add(new_customer)
 
     application = store.add_application(
         tag="RMLP05R800",
         prep_category="rml",
         description="Ready-made",
         percent_kth=80,
         percent_reads_guaranteed=75,
         sequencing_depth=0,
         target_reads=800,
     )
-    store.add_commit(application)
+    store.session.add(application)
 
     app_version = store.add_application_version(
         application=application,
         version=1,
         valid_from=timestamp_now,
         prices={
             PriorityTerms.STANDARD: 12,
             PriorityTerms.PRIORITY: 222,
             PriorityTerms.EXPRESS: 123,
             PriorityTerms.RESEARCH: 12,
         },
     )
-    store.add_commit(app_version)
+    store.session.add(app_version)
 
     new_pool = store.add_pool(
         customer=new_customer,
         name="Test",
         order="Test",
         ordered=dt.datetime.now(),
         application_version=app_version,
     )
-    store.add_commit(new_pool)
+    store.session.add(new_pool)
     new_case = helpers.add_case(
         store=store,
         internal_id=case_id,
         name=PoolSubmitter.create_case_name(ticket=ticket_id, pool_name="Test"),
     )
-    store.add_commit(new_case)
+    store.session.add(new_case)
 
     new_sample = helpers.add_sample(
         store=store,
         internal_id=sample_id,
         application_tag=application.tag,
         application_type=application.prep_category,
         customer_id=new_customer.id,
     )
     new_sample.application_version = app_version
-    store.add_commit(new_sample)
+    store.session.add(new_sample)
+    store.session.commit()
 
     helpers.add_relationship(
         store=store,
         sample=new_sample,
         case=new_case,
     )
```

### Comparing `cg-29.0.3/tests/store/api/delete/test_store_api_delete.py` & `cg-29.1.0/tests/store/api/delete/test_store_api_delete.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/api/find/test_find_basic_data.py` & `cg-29.1.0/tests/store/api/find/test_find_basic_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 def test_get_active_beds_when_archived(base_store: Store):
     """Test returning not archived bed records from the database when archived."""
 
     # GIVEN a store with beds
     beds: Query = base_store.get_active_beds()
     for bed in beds:
         bed.is_archived = True
-        base_store.add_commit(bed)
+        base_store.session.add(bed)
+        base_store.session.commit()
 
     # WHEN fetching beds
     active_beds: Query = base_store.get_active_beds()
 
     # THEN return no beds
     assert not list(active_beds)
```

### Comparing `cg-29.0.3/tests/store/api/find/test_find_basic_data_application_version.py` & `cg-29.1.0/tests/store/api/find/test_find_basic_data_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/api/find/test_find_business_data.py` & `cg-29.1.0/tests/store/api/find/test_find_business_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,16 @@
     """Test returning the latest flow cell from the database by statuses when multiple matches."""
 
     # GIVEN a store with two flow cells
 
     # GIVEN a flow cell that exist in status db with status "requested"
     flow_cells: List[Flowcell] = re_sequenced_sample_store._get_query(table=Flowcell)
     flow_cells[0].status = FlowCellStatus.REQUESTED
-    re_sequenced_sample_store.add_commit(flow_cells[0])
+    re_sequenced_sample_store.session.add(flow_cells[0])
+    re_sequenced_sample_store.session.commit()
 
     # WHEN fetching the latest flow cell
     flow_cells: List[Flowcell] = re_sequenced_sample_store.get_flow_cells_by_statuses(
         flow_cell_statuses=[FlowCellStatus.ON_DISK, FlowCellStatus.REQUESTED]
     )
 
     # THEN the flow cell status should be "ondisk" or "requested"
@@ -510,15 +511,15 @@
 
 
 def test_is_case_down_sampled_true(base_store: Store, case_obj: Family, sample_id: str):
     """Tests the down sampling check when all samples are down sampled."""
     # GIVEN a case where all samples are down sampled
     for sample in case_obj.samples:
         sample.from_sample = sample_id
-    base_store.commit()
+    base_store.session.commit()
 
     # WHEN checking if all sample in the case are down sampled
     is_down_sampled: bool = base_store.is_case_down_sampled(case_id=case_obj.internal_id)
 
     # THEN the return value should be True
     assert is_down_sampled
 
@@ -542,15 +543,15 @@
     """Tests the external case check when all the samples are external."""
     # GIVEN a case where all samples are not external
     external_application_version: ApplicationVersion = helpers.ensure_application_version(
         store=base_store, is_external=True
     )
     for sample in case_obj.samples:
         sample.application_version = external_application_version
-    base_store.commit()
+    base_store.session.commit()
 
     # WHEN checking if all sample in the case are external
     is_external: bool = base_store.is_case_external(case_id=case_obj.internal_id)
 
     # THEN the return value should be False
     assert is_external
```

### Comparing `cg-29.0.3/tests/store/api/find/test_find_business_data_analysis.py` & `cg-29.1.0/tests/store/api/find/test_find_business_data_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/api/find/test_find_business_data_case.py` & `cg-29.1.0/tests/store/api/find/test_find_business_data_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/api/find/test_find_business_data_sample.py` & `cg-29.1.0/tests/store/api/find/test_find_business_data_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/api/status/test_analyses_to_clean.py` & `cg-29.1.0/tests/store/api/status/test_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/api/status/test_analyses_to_delivery_report.py` & `cg-29.1.0/tests/store/api/status/test_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/api/status/test_store_api_status.py` & `cg-29.1.0/tests/store/api/status/test_store_api_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for store API status module."""
 
-from alchy import Query
+from sqlalchemy.orm import Query
 from typing import List
 from cg.constants import Pipeline, Priority
 from cg.constants.subject import PhenotypeStatus
 from cg.store import Store
 from cg.store.models import Analysis, Application, Family, Sample
 from tests.store_helpers import StoreHelpers
```

### Comparing `cg-29.0.3/tests/store/api/status/test_store_api_status_analysis.py` & `cg-29.1.0/tests/store/api/status/test_store_api_status_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """This script tests the cli methods to add cases to status-db"""
 from typing import List, Union
 
-from alchy import Query
+from sqlalchemy.orm import Query
 from datetime import datetime
 
 from cg.constants import Pipeline
 from cg.constants.constants import CaseActions
 from cg.constants.subject import Gender, PhenotypeStatus
 from cg.store import Store
 from cg.store.models import Analysis, Family, Sample
```

### Comparing `cg-29.0.3/tests/store/api/status/test_store_api_status_cases.py` & `cg-29.1.0/tests/store/api/status/test_store_api_status_cases.py`

 * *Files 0% similar despite different names*

```diff
@@ -1508,9 +1508,10 @@
         priority=priority,
         ticket=ticket,
     )
     case.customer = customer
     case.ordered_at = datetime.now() - timedelta(days=ordered_days_ago)
     if action:
         case.action = action
-    disk_store.add_commit(case)
+    disk_store.session.add(case)
+    disk_store.session.commit()
     return case
```

### Comparing `cg-29.0.3/tests/store/api/status/test_store_api_status_customer.py` & `cg-29.1.0/tests/store/api/status/test_store_api_status_customer.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/api/status/test_store_api_status_pool.py` & `cg-29.1.0/tests/store/api/status/test_store_api_status_pool.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/api/status/test_store_api_status_sample.py` & `cg-29.1.0/tests/store/api/status/test_store_api_status_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/api/test_base.py` & `cg-29.1.0/tests/store/api/test_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Tests for the BaseHandle class."""
 from typing import Type
+from mock import MagicMock
 
 import pytest
 from dataclasses import astuple
 
-from alchy import Query, ModelBase
+from sqlalchemy.orm import Query
 from cg.constants.subject import PhenotypeStatus
 from cg.store.api.base import BaseHandler
+from cg.store.models import Model
 
 
-@pytest.mark.parametrize("table", astuple(BaseHandler()))
-def test__get_query(base_store, table: Type[ModelBase]):
+@pytest.mark.parametrize("table", astuple(BaseHandler(MagicMock())))
+def test__get_query(base_store, table: Type[Model]):
     """Tests the _get_query function for all attributes of BaseHandler ie tables in the database."""
     assert isinstance(base_store._get_query(table=table), Query)
 
 
 def test_get_latest_analyses_for_cases_query(
     analysis_store, helpers, timestamp_now, timestamp_yesterday
 ):
@@ -25,15 +27,16 @@
     analysis_oldest = helpers.add_analysis(
         analysis_store,
         case=case,
         started_at=timestamp_yesterday,
         uploaded_at=timestamp_yesterday,
         delivery_reported_at=None,
     )
-    analysis_store.add_commit(analysis_oldest)
+    analysis_store.session.add(analysis_oldest)
+    analysis_store.session.commit()
     analysis_newest = helpers.add_analysis(
         analysis_store,
         case=case,
         started_at=timestamp_now,
         uploaded_at=timestamp_now,
         delivery_reported_at=None,
     )
```

### Comparing `cg-29.0.3/tests/store/conftest.py` & `cg-29.1.0/tests/store/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,29 +148,29 @@
     for sample_data in microbial_submitted_order["items"]:
         application_version = base_store.get_application_by_tag(
             sample_data["application"]
         ).versions[0]
         organism = base_store.Organism(
             internal_id=sample_data["organism"], name=sample_data["organism"]
         )
-        base_store.add(organism)
+        base_store.session.add(organism)
         sample = base_store.add_sample(
             name=sample_data["name"],
             sex=Gender.UNKNOWN,
             comment=sample_data["comment"],
             priority=sample_data["priority"],
             reads=sample_data["reads"],
             reference_genome=sample_data["reference_genome"],
         )
         sample.application_version = application_version
         sample.customer = customer
         sample.organism = organism
-        base_store.add(sample)
+        base_store.session.add(sample)
 
-    base_store.commit()
+    base_store.session.commit()
     yield base_store
 
 
 @pytest.fixture(name="analysis_obj")
 def fixture_analysis_obj(analysis_store: Store) -> Analysis:
     """Return an analysis object from a populated store."""
     return analysis_store._get_query(table=Analysis)[0]
@@ -405,15 +405,16 @@
     """Return a store with  older and newer analyses."""
     analysis = base_store._get_query(table=Analysis).first()
     analysis.uploaded_at = timestamp_now
     analysis.uploaded_to_vogue_at = timestamp_now
     analysis.cleaned_at = timestamp_now
     analysis.started_at = timestamp_now
     analysis.completed_at = timestamp_now
-    base_store.add_commit(analysis)
+    base_store.session.add(analysis)
+    base_store.session.commit()
     times = [timestamp_now, timestamp_yesterday, old_timestamp]
     for time in times:
         helpers.add_analysis(
             store=base_store,
             case=case_obj,
             pipeline=Pipeline.BALSAMIC,
             started_at=time,
```

### Comparing `cg-29.0.3/tests/store/filters/test_status_analyses_filters.py` & `cg-29.1.0/tests/store/filters/test_status_analyses_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime, timedelta
 
-from alchy import Query
+from sqlalchemy.orm import Query
 from cgmodels.cg.constants import Pipeline
 
 from typing import List
 from cg.store import Store
 from cg.store.models import Analysis, Family
 from cg.store.filters.status_analysis_filters import (
     filter_valid_analyses_in_production,
```

### Comparing `cg-29.0.3/tests/store/filters/test_status_application_filters.py` & `cg-29.1.0/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/filters/test_status_application_version_filters.py` & `cg-29.1.0/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/filters/test_status_bed_filters.py` & `cg-29.1.0/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/filters/test_status_bed_version_filters.py` & `cg-29.1.0/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/filters/test_status_case_sample_filters.py` & `cg-29.1.0/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/filters/test_status_cases_filters.py` & `cg-29.1.0/tests/store/filters/test_status_cases_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Union
 
-from alchy import Query
+from sqlalchemy.orm import Query
 from cgmodels.cg.constants import Pipeline
 from datetime import datetime
 
 from cg.constants.constants import CaseActions, DataDelivery
 from cg.constants.sequencing import SequencingMethod
 from cg.constants.subject import PhenotypeStatus
 from cg.store import Store
```

### Comparing `cg-29.0.3/tests/store/filters/test_status_collaboration_filters.py` & `cg-29.1.0/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/filters/test_status_customer_filters.py` & `cg-29.1.0/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/filters/test_status_flow_cell_filters.py` & `cg-29.1.0/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/filters/test_status_invoice_filters.py` & `cg-29.1.0/tests/store/filters/test_status_invoice_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from alchy import Query
+from sqlalchemy.orm import Query
 from cg.store import Store
 from cg.store.models import Invoice
 from tests.store_helpers import StoreHelpers
 from cg.store.filters.status_invoice_filters import (
     filter_invoices_by_invoice_id,
     filter_invoices_invoiced,
     filter_invoices_not_invoiced,
```

### Comparing `cg-29.0.3/tests/store/filters/test_status_organism_filters.py` & `cg-29.1.0/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/filters/test_status_panel_filters.py` & `cg-29.1.0/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/filters/test_status_pool_filters.py` & `cg-29.1.0/tests/store/filters/test_status_pool_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from alchy import Query
+from sqlalchemy.orm import Query
 from cg.store import Store
 from cg.store.models import Pool
 from cg.store.filters.status_pool_filters import (
     filter_pools_is_received,
     filter_pools_is_not_received,
     filter_pools_is_delivered,
     filter_pools_is_not_delivered,
```

### Comparing `cg-29.0.3/tests/store/filters/test_status_samples_filters.py` & `cg-29.1.0/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/filters/test_status_user_filters.py` & `cg-29.1.0/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/test_delivery.py` & `cg-29.1.0/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/store/test_store_models.py` & `cg-29.1.0/tests/store/test_store_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     # THEN the application version's application is the application used for instantiation
     assert application_version.application == application
 
 
 def test_microbial_sample_to_dict(microbial_store: Store, helpers):
     # GIVEN a store with a Microbial sample
     sample_obj = helpers.add_microbial_sample(microbial_store)
-    microbial_store.add_commit(sample_obj)
+    microbial_store.session.add(sample_obj)
+    microbial_store.session.commit()
     assert sample_obj
 
     # WHEN running to dict on that sample
     a_dict = sample_obj.to_dict(links=True)
 
     # THEN you should get a dictionary with
     assert a_dict["id"]
@@ -98,16 +99,17 @@
         invoice_address="Test street",
         invoice_reference="ABCDEF",
     )
     prod_customer: Customer = base_store.get_customer_by_internal_id(
         customer_internal_id=customer_id
     )
     collaboration.customers.extend([prod_customer, new_customer])
-    base_store.add_commit(new_customer, collaboration)
-    base_store.refresh(collaboration)
+    base_store.session.add_all([new_customer, collaboration])
+    base_store.session.commit()
+    base_store.session.refresh(collaboration)
     # WHEN calling the collaborators property
     collaborators = prod_customer.collaborators
     # THEN all customers in both collaborations should be returned
     assert len(collaborators) == 5
     assert all(
         collaborator.internal_id in ["cust001", new_customer_id, "cust002", "cust003", customer_id]
         for collaborator in collaborators
```

### Comparing `cg-29.0.3/tests/store_helpers.py` & `cg-29.1.0/tests/store_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,16 @@
         if not new_record:
             new_record: ApplicationVersion = store.add_application_version(
                 application=application,
                 version=version,
                 valid_from=valid_from,
                 prices=prices,
             )
-        store.add_commit(new_record)
+        store.session.add(new_record)
+        store.session.commit()
         return new_record
 
     @staticmethod
     def ensure_application(
         store: Store,
         tag: str,
         prep_category: str = "wgs",
@@ -184,31 +185,33 @@
             percent_reads_guaranteed=75,
             is_accredited=is_accredited,
             limitations="A limitation",
             is_external=is_external,
             min_sequencing_depth=min_sequencing_depth,
             **kwargs,
         )
-        store.add_commit(application)
+        store.session.add(application)
+        store.session.commit()
         return application
 
     @staticmethod
     def ensure_bed_version(store: Store, bed_name: str = "dummy_bed") -> BedVersion:
         """Return existing or create and return bed version for tests."""
         bed: Optional[Bed] = store.get_bed_by_name(bed_name=bed_name)
         if not bed:
             bed: Bed = store.add_bed(name=bed_name)
-            store.add_commit(bed)
+            store.session.add(bed)
 
         bed_version: Optional[BedVersion] = store.get_latest_bed_version(bed_name=bed_name)
         if not bed_version:
             bed_version: BedVersion = store.add_bed_version(
                 bed=bed, version=1, filename="dummy_filename", shortname=bed_name
             )
-            store.add_commit(bed_version)
+            store.session.add(bed_version)
+            store.session.commit()
         return bed_version
 
     @staticmethod
     def ensure_collaboration(store: Store, collaboration_id: str = "all_customers"):
         collaboration = store.get_collaboration_by_internal_id(collaboration_id)
         if not collaboration:
             collaboration = store.add_collaboration(collaboration_id, collaboration_id)
@@ -230,15 +233,16 @@
                 internal_id=customer_id,
                 name=customer_name,
                 scout_access=scout_access,
                 invoice_address="Test street",
                 invoice_reference="ABCDEF",
             )
             customer.collaborations.append(collaboration)
-            store.add_commit(customer)
+            store.session.add(customer)
+            store.session.commit()
         return customer
 
     @staticmethod
     def add_analysis(
         store: Store,
         case: Family = None,
         started_at: datetime = None,
@@ -277,15 +281,16 @@
         if pipeline:
             analysis.pipeline = str(pipeline)
         if uploaded_to_vogue_at:
             analysis.uploaded_to_vogue_at = uploaded_to_vogue_at
 
         analysis.limitations = "A limitation"
         analysis.family = case
-        store.add_commit(analysis)
+        store.session.add(analysis)
+        store.session.commit()
         return analysis
 
     @staticmethod
     def add_sample(
         store: Store,
         application_tag: str = "dummy_tag",
         application_type: str = "tgs",
@@ -336,15 +341,16 @@
             if key == "flowcell":
                 sample.flowcells.append(kwargs["flowcell"])
             elif hasattr(sample, key):
                 setattr(sample, key, value)
             else:
                 raise AttributeError(f"Unknown sample attribute/feature: {key}, {value}")
 
-        store.add_commit(sample)
+        store.session.add(sample)
+        store.session.commit()
         return sample
 
     @staticmethod
     def ensure_panel(
         store: Store, panel_abbreviation: str = "panel_test", customer_id: str = "cust000"
     ) -> Panel:
         """Utility function to add a panel to use in tests."""
@@ -355,15 +361,16 @@
                 customer=customer,
                 name=panel_abbreviation,
                 abbrev=panel_abbreviation,
                 version=1.0,
                 date=datetime.now(),
                 genes=1,
             )
-            store.add_commit(panel)
+            store.session.add(panel)
+            store.session.commit()
         return panel
 
     @staticmethod
     def add_case(
         store: Store,
         name: str = "case_test",
         data_analysis: str = Pipeline.MIP_DNA,
@@ -401,15 +408,16 @@
             )
         if action:
             case_obj.action = action
         if internal_id:
             case_obj.internal_id = internal_id
 
         case_obj.customer = customer
-        store.add_commit(case_obj)
+        store.session.add(case_obj)
+        store.session.commit()
         return case_obj
 
     @staticmethod
     def ensure_case(
         store: Store,
         case_name: str = "test-case",
         case_id: str = "blueeagle",
@@ -527,15 +535,16 @@
         name: str = "organism_name",
         reference_genome: str = "reference_genome_test",
     ) -> Organism:
         """Utility function to add an organism to use in tests."""
         organism = StoreHelpers.add_organism(
             store, internal_id=organism_id, name=name, reference_genome=reference_genome
         )
-        store.add_commit(organism)
+        store.session.add(organism)
+        store.session.commit()
         return organism
 
     @staticmethod
     def add_microbial_sample(
         store: Store,
         sample_id: str = "microbial_sample_id",
         priority: str = PriorityTerms.RESEARCH,
@@ -598,15 +607,16 @@
         )
         flow_cell.archived_at = archived_at
         if samples:
             flow_cell.samples = samples
         if status:
             flow_cell.status = status
 
-        store.add_commit(flow_cell)
+        store.session.add(flow_cell)
+        store.session.commit()
         return flow_cell
 
     @staticmethod
     def add_relationship(
         store: Store,
         sample: Sample,
         case: Family,
@@ -614,82 +624,84 @@
         father: Sample = None,
         mother: Sample = None,
     ) -> FamilySample:
         """Utility function to link a sample to a case."""
         link = store.relate_sample(
             sample=sample, family=case, status=status, father=father, mother=mother
         )
-        store.add_commit(link)
+        store.session.add(link)
+        store.session.commit()
         return link
 
     @staticmethod
     def add_synopsis_to_case(
         store: Store, case_id: str, synopsis: str = "a synopsis"
     ) -> Optional[Family]:
         """Function for adding a synopsis to a case in the database."""
         case_obj: Family = store.get_case_by_internal_id(internal_id=case_id)
         if not case_obj:
             LOG.warning("Could not find case")
             return None
         case_obj.synopsis = synopsis
-        store.commit()
+        store.session.commit()
         return case_obj
 
     @staticmethod
     def add_phenotype_groups_to_sample(
         store: Store, sample_id: str, phenotype_groups: [str] = None
     ) -> Optional[Sample]:
         """Function for adding a phenotype group to a sample in the database."""
         if phenotype_groups is None:
             phenotype_groups = ["a phenotype group"]
         sample_obj: Sample = store.get_sample_by_internal_id(internal_id=sample_id)
         if not sample_obj:
             LOG.warning("Could not find sample")
             return None
         sample_obj.phenotype_groups = phenotype_groups
-        store.commit()
+        store.session.commit()
         return sample_obj
 
     @staticmethod
     def add_phenotype_terms_to_sample(
         store: Store, sample_id: str, phenotype_terms: List[str] = []
     ) -> Optional[Sample]:
         """Function for adding a phenotype term to a sample in the database."""
         if not phenotype_terms:
             phenotype_terms: List[str] = ["a phenotype term"]
         sample_obj: Sample = store.get_sample_by_internal_id(internal_id=sample_id)
         if not sample_obj:
             LOG.warning("Could not find sample")
             return None
         sample_obj.phenotype_terms = phenotype_terms
-        store.commit()
+        store.session.commit()
         return sample_obj
 
     @staticmethod
     def add_subject_id_to_sample(
         store: Store, sample_id: str, subject_id: str = "a subject_id"
     ) -> Optional[Sample]:
         """Function for adding a subject_id to a sample in the database."""
         sample_obj: Sample = store.get_sample_by_internal_id(internal_id=sample_id)
         if not sample_obj:
             LOG.warning("Could not find sample")
             return None
         sample_obj.subject_id = subject_id
-        store.commit()
+        store.session.commit()
         return sample_obj
 
     @classmethod
     def relate_samples(cls, base_store: Store, case: Family, samples: List[Sample]):
         """Utility function to relate many samples to one case."""
 
         for sample in samples:
             link = base_store.relate_sample(
                 family=case, sample=sample, status=PhenotypeStatus.UNKNOWN
             )
-            base_store.add_commit(link)
+            base_store.session.add(link)
+            base_store.session.commit()
 
     @classmethod
     def add_case_with_samples(
         cls,
         base_store: Store,
         case_id: str,
         nr_samples: int,
@@ -755,15 +767,16 @@
             customer=customer,
             order=order,
             delivered_at=delivered_at,
             received_at=received_at,
             no_invoice=no_invoice,
             invoice_id=invoice_id,
         )
-        store.add_commit(pool)
+        store.session.add(pool)
+        store.session.commit()
         return pool
 
     @classmethod
     def ensure_user(
         cls,
         store: Store,
         customer: Customer,
@@ -771,15 +784,16 @@
         name: str = "Bob",
         is_admin: bool = False,
     ) -> User:
         """Utility function to add a user that can be used in tests."""
         user: User = store.get_user_by_email(email=email)
         if not user:
             user = store.add_user(customer=customer, email=email, name=name, is_admin=is_admin)
-            store.add_commit(user)
+            store.session.add(user)
+            store.session.commit()
         return user
 
     @classmethod
     def ensure_invoice(
         cls,
         store: Store,
         invoice_id: int = 0,
@@ -804,16 +818,16 @@
                 customer=customer_obj,
                 samples=samples,
                 pools=pools,
                 comment="just a test invoice",
                 discount=discount,
                 invoiced_at=invoiced_at,
             )
-            store.add_commit(invoice)
-
+            store.session.add(invoice)
+            store.session.commit()
         return invoice
 
     @classmethod
     def add_case_with_sample(cls, base_store: Store, case_id: str, sample_id: str) -> Family:
         """Helper function to add a case associated with a sample with the given ids."""
 
         case = cls.add_case(store=base_store, internal_id=case_id, name=case_id)
```

### Comparing `cg-29.0.3/tests/test_store_helpers.py` & `cg-29.1.0/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/utils/conftest.py` & `cg-29.1.0/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/utils/test_commands.py` & `cg-29.1.0/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/utils/test_date.py` & `cg-29.1.0/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/utils/test_dict.py` & `cg-29.1.0/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/utils/test_dispatcher.py` & `cg-29.1.0/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-29.0.3/tests/utils/test_utils.py` & `cg-29.1.0/tests/utils/test_utils.py`

 * *Files identical despite different names*

