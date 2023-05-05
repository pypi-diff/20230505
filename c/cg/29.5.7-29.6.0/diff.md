# Comparing `tmp/cg-29.5.7.tar.gz` & `tmp/cg-29.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cg-29.5.7.tar", last modified: Thu May  4 10:11:57 2023, max compression
+gzip compressed data, was "dist/cg-29.6.0.tar", last modified: Thu May  4 13:15:32 2023, max compression
```

## Comparing `cg-29.5.7.tar` & `cg-29.6.0.tar`

### file list

```diff
@@ -1,1245 +1,1245 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-04 10:11:47.000000 cg-29.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-04 10:11:57.000000 cg-29.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-04 10:11:47.000000 cg-29.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 10:11:47.000000 cg-29.5.7/cg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/crud/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/crud/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/crud/find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/cgstats/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/cgstats/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/db/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/db/models/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/db/models/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/db/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/db/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/db/models/support_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/db/models/unaligned.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/db/models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/dragen_demux_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/parsers/adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/parsers/conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/parsers/demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/parsers/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/parsers/run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/cgstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/crunchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/crunchy/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/crunchy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/crunchy/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/demultiplex/demux_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/demultiplex/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/demultiplex/sample_sheet/dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/demultiplex/sample_sheet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/demultiplex/sample_sheet/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/hermes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/hermes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/hermes/hermes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/hermes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17538 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/housekeeper/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/housekeeper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/invoice/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/invoice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/lims/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/lims/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/lims/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/lims/samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/loqus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/madeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/madeline/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/mip/confighandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/orderform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/scout/scout_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/scout/scoutapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/slurm/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/slurm/slurm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/apps/tb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/tb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/tb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/tb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-04 10:11:47.000000 cg-29.5.7/cg/apps/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/compress/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/compress/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/delete/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/delete/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/delete/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/delete/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/deliver/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/demultiplex/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/demultiplex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/demultiplex/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/demultiplex/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/demultiplex/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/generate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/generate/report/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/generate/report/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/generate/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/set/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/set/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/set/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/store/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/fohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/nipt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/nipt/statina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/upload/observations/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/observations/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/fastq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/fluffy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/microsalt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/mip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/mip/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/mip_dna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/mip_dna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/mip_rna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/mip_rna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/mutant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/mutant/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/nextflow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/rnafusion/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/taxprofiler/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/cli/workflow/tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 10:11:47.000000 cg-29.5.7/cg/cli/workflow/tower/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/cgstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/demultiplexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/gene_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/housekeeper_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/orderforms.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/sample_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/scout_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/sequencing.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 10:11:47.000000 cg-29.5.7/cg/constants/tb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-04 10:11:47.000000 cg-29.5.7/cg/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-04 10:11:47.000000 cg-29.5.7/cg/io/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-04 10:11:47.000000 cg-29.5.7/cg/io/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-04 10:11:47.000000 cg-29.5.7/cg/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 10:11:47.000000 cg-29.5.7/cg/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-04 10:11:47.000000 cg-29.5.7/cg/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/archive/ddn_dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/backup/pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/clean/demultiplexed_flow_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/clean/flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/compress/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/compress/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/deliver_ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/demultiplex/delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/demultiplex/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/observations/observations_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/case_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/pool_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/rml_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/orders/ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/report/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/report/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/report/field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/report/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/report/report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/report/templates/mip-dna_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/rsync/rsync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/rsync/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/tar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/tar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/tar/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/transfer/external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/transfer/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/transfer/lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/upload/fohm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/fohm/fohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/gisaid/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/upload/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/nipt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/nipt/nipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/upload/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/rnafusion/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19775 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20224 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    28473 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/fluffy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/mutant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/nextflow_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 10:11:47.000000 cg-29.5.7/cg/meta/workflow/tower_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/balsamic/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/balsamic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/balsamic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/cg_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/cgstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/cgstats/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/cgstats/stats_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/compression_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/deliverables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/deliverables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/deliverables/metric_deliverables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/demultiplex/demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/demultiplex/flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/invoice/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/lims/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/lims/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/mip/mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/mip/mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/mip/mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/nextflow/deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/nextflow/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/observations/input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/orders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/orders/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/orders/excel_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/orders/json_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/orders/orderform_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/orders/sample_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/orders/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/report/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/report/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/report/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/rnafusion/rnafusion_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/scout/scout_load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/slurm/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/taxprofiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-04 10:11:47.000000 cg-29.5.7/cg/models/workflow/mutant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-05-04 10:11:47.000000 cg-29.5.7/cg/resources/20181012_Indices.csv
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-04 10:11:47.000000 cg-29.5.7/cg/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-04 10:11:47.000000 cg-29.5.7/cg/resources/rnafusion_bundle_filenames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/cg/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18089 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/cg/server/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/server/invoices/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/cg/server/invoices/templates/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/invoices/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/cg/server/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-04 10:11:47.000000 cg-29.5.7/cg/server/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/cg/store/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/cg/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/api/find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    32042 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/api/find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    39247 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/cg/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_case_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/filters/status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    29141 2023-05-04 10:11:47.000000 cg-29.5.7/cg/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/cg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/cg/utils/checksum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/checksum/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/cg/utils/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/click/EnumChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/cg/utils/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/flask/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-04 10:11:47.000000 cg-29.5.7/cg/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/cg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-04 10:11:56.000000 cg-29.5.7/cg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39785 2023-05-04 10:11:56.000000 cg-29.5.7/cg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:11:56.000000 cg-29.5.7/cg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 10:11:56.000000 cg-29.5.7/cg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:11:56.000000 cg-29.5.7/cg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-04 10:11:56.000000 cg-29.5.7/cg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 10:11:56.000000 cg-29.5.7/cg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 10:11:47.000000 cg-29.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 10:11:47.000000 cg-29.5.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 10:11:57.000000 cg-29.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-04 10:11:47.000000 cg-29.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/cgstats/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/cgstats/crud/test_create_novaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/cgstats/crud/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/cgstats/parsers/test_adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/cgstats/parsers/test_conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/cgstats/parsers/test_demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/cgstats/parsers/test_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/cgstats/parsers/test_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/cgstats/test_cgstats_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/cgstats/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/coverage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/coverage/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/crunchy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/crunchy/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/crunchy/test_spring_decompression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/demultiplex/test_convert_to_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/demultiplex/test_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/gens/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/gens/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/gens/test_gens_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/gt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/gt/test_gt_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/hk/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/hk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/hk/test__getattr__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/hk/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/hk/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/hk/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/hk/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/hk/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/lims/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/lims/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/loqus/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/loqus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/loqus/test_loqusdb_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/madeline/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/madeline/test_madeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/mip/test_config_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/mutacc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/mutacc_auto/test_mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/orderform/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/orderform/test_orderform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/scout/test_scout_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/slurm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/test_apps_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/test_osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/apps/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-04 10:11:47.000000 cg-29.5.7/tests/apps/vogue/test_vogue_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/add/test_cli_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/add/test_cli_add_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/backup/test_backup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/clean/test_rsync_past_run_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/delete/test_cli_delete_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/deliver/test_run_deliver_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/demultiplex/test_add_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/demultiplex/test_stats_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/generate/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/generate/report/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/generate/test_cli_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/get/test_cli_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/get/test_cli_get_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/set/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/set/test_cli_set_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/store/test_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/test_cli_status_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/cli/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/upload/test_cli_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)    31010 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/fastq/test_fastq_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/fluffy/test_cli_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/microsalt/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/workflow/microsalt/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/microsalt/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/microsalt/test_microsalt_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/taxprofiler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-04 10:11:47.000000 cg-29.5.7/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    63291 2023-05-04 10:11:47.000000 cg-29.5.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/DEMUX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/analysis/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/analysis/balsamic/tn_wgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/analysis/microsalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/analysis/mip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/analysis/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/analysis/sample_coverage.bed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/balsamic/case/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/crunchy/spring_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters_different_index_cycles.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/hiseq_run/
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/raw_lims_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/fluffy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/fluffy/2020-23219-05/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/fluffy/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/gt/yellowhog.bcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/madeline/madeline.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/fixtures/apps/mip/dna/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/mip/dna/store/
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/mip/rna/
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/mip/rna/store/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/mip/sample_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/scout/panel_export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/apps/shipping/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/apps/shipping/scout-deploy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/cgweb_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/cgweb_orders/sarscov2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/data/cgfixture.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/data/hkstore.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/data/yellowhog/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/data/yellowhog/pedigree.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/io/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/io/example_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/io/example_json.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/orderforms/
--rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/1508.27.balsamic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/1508.27.fastq.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/1508.27.mip.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/1604.15.rml.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/1605.10.metagenome.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/fixtures/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/report/case_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-04 10:11:47.000000 cg-29.5.7/tests/fixtures/report/lims_family.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-04 10:11:47.000000 cg-29.5.7/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-04 10:11:47.000000 cg-29.5.7/tests/io/test_io_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-04 10:11:47.000000 cg-29.5.7/tests/io/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-04 10:11:47.000000 cg-29.5.7/tests/io/test_io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-04 10:11:47.000000 cg-29.5.7/tests/io/test_io_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/archive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/archive/test_archiving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24603 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/backup/test_meta_pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/clean/test_clean_demultiplexed_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/clean/test_clean_flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/compress/test_compress_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/deliver/test_delivery_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/demultiplex/test_delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/demultiplex/test_rename_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/encryption/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/observations/test_meta_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/orders/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19944 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0 runner    (1001) docker     (123)    29129 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/orders/test_ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/report/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/report/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/report/test_report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/rsync/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/rsync/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/test_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/transfer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/transfer/test_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/transfer/test_meta_transfer_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/transfer/test_meta_transfer_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/gisaid/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/upload/gisaid/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/upload/mutacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/nipt/test_nipt_upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    24993 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/test_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/test_upload_genotypes_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/upload/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/upload/vogue/test_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/workflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/workflow/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-04 10:11:47.000000 cg-29.5.7/tests/meta/workflow/test_prepare_fastq_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/hk_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/limsmock.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/madeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/osticket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/process_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/store_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-04 10:11:47.000000 cg-29.5.7/tests/mocks/tb_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/models/demultiplexing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/demultiplexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/demultiplexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/demultiplexing/test_demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/demultiplexing/test_flowcell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/demultiplexing/test_run_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/mip/test_mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/mip/test_mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/nextflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/nextflow/test_nextflow_deliver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/observations/test_observations_input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/report/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/test_cg_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/test_compression_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/test_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 10:11:47.000000 cg-29.5.7/tests/models/test_flowcell_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-04 10:11:47.000000 cg-29.5.7/tests/server/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-04 10:11:47.000000 cg-29.5.7/tests/server/test_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-04 10:11:47.000000 cg-29.5.7/tests/server/test_server_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 10:11:47.000000 cg-29.5.7/tests/small_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/store/api/add/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/add/test_store_add_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/add/test_store_add_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/add/test_store_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/add/test_store_add_flow_celll.py
--rw-r--r--   0 runner    (1001) docker     (123)    19418 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/store/api/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/delete/test_store_api_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/store/api/find/
--rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/find/test_find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/find/test_find_basic_data_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    28823 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/find/test_find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/find/test_find_business_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/find/test_find_business_data_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/find/test_find_business_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/store/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/status/test_analyses_to_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/status/test_analyses_to_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/status/test_store_api_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/status/test_store_api_status_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    54240 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/status/test_store_api_status_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/status/test_store_api_status_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/status/test_store_api_status_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/status/test_store_api_status_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    39481 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    26900 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30278 2023-05-04 10:11:47.000000 cg-29.5.7/tests/store_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-04 10:11:47.000000 cg-29.5.7/tests/test_store_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:56.000000 cg-29.5.7/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:57.000000 cg-29.5.7/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:47.000000 cg-29.5.7/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-04 10:11:47.000000 cg-29.5.7/tests/utils/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-04 10:11:47.000000 cg-29.5.7/tests/utils/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-04 10:11:47.000000 cg-29.5.7/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-04 10:11:47.000000 cg-29.5.7/tests/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-04 10:11:47.000000 cg-29.5.7/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-04 10:11:47.000000 cg-29.5.7/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-04 13:15:21.000000 cg-29.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-04 13:15:32.000000 cg-29.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-04 13:15:21.000000 cg-29.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 13:15:21.000000 cg-29.6.0/cg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/crud/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/crud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/crud/find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/cgstats/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/cgstats/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/db/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/db/models/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/db/models/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/db/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/db/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/db/models/support_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/db/models/unaligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/db/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/dragen_demux_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/parsers/adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/parsers/conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/parsers/demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/parsers/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/parsers/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/cgstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/crunchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/crunchy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/crunchy/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/demultiplex/demux_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/demultiplex/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/demultiplex/sample_sheet/dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/demultiplex/sample_sheet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/demultiplex/sample_sheet/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/hermes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/hermes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/hermes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17538 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/housekeeper/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/housekeeper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/invoice/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/invoice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/lims/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/lims/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/lims/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/lims/samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/loqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/madeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/madeline/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/mip/confighandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/orderform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/scout/scout_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/scout/scoutapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/slurm/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/slurm/slurm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/apps/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/tb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/tb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/tb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-04 13:15:21.000000 cg-29.6.0/cg/apps/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/compress/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/compress/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/compress/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/delete/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/delete/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/delete/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/delete/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/deliver/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/demultiplex/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/demultiplex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/demultiplex/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/demultiplex/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/demultiplex/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/generate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/generate/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/generate/report/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/generate/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/set/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/set/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/set/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/store/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/fohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/nipt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/nipt/statina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/upload/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/observations/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/fastq/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/fluffy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/microsalt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/mip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/mip/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/mip_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/mip_dna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/mip_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/mip_rna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/mutant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/mutant/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/nextflow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/rnafusion/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/taxprofiler/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/cli/workflow/tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 13:15:21.000000 cg-29.6.0/cg/cli/workflow/tower/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/cgstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/demultiplexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/gene_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/housekeeper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/orderforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/sample_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/scout_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/sequencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 13:15:21.000000 cg-29.6.0/cg/constants/tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-04 13:15:21.000000 cg-29.6.0/cg/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-04 13:15:21.000000 cg-29.6.0/cg/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-04 13:15:21.000000 cg-29.6.0/cg/io/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-04 13:15:21.000000 cg-29.6.0/cg/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 13:15:21.000000 cg-29.6.0/cg/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-04 13:15:21.000000 cg-29.6.0/cg/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/archive/ddn_dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/backup/pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/clean/demultiplexed_flow_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/clean/flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/compress/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/compress/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/deliver_ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/demultiplex/delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/demultiplex/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/observations/observations_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/case_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/orders/ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/report/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/report/field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/report/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/report/report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/report/templates/mip-dna_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/rsync/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/tar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/tar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/tar/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/transfer/external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/transfer/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/transfer/lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/upload/fohm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/fohm/fohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/upload/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/nipt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/nipt/nipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/upload/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/rnafusion/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20192 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28473 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/fluffy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/mutant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/nextflow_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 13:15:21.000000 cg-29.6.0/cg/meta/workflow/tower_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/balsamic/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/balsamic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/balsamic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/cg_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/cgstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/cgstats/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/cgstats/stats_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/compression_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/deliverables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/deliverables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/deliverables/metric_deliverables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/demultiplex/demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/demultiplex/flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/invoice/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/lims/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/mip/mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/mip/mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/mip/mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/nextflow/deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/nextflow/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/observations/input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/orders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/orders/excel_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/orders/json_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/orders/orderform_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/orders/sample_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/orders/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/report/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/report/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/report/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/rnafusion/rnafusion_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/scout/scout_load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/slurm/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/taxprofiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-04 13:15:21.000000 cg-29.6.0/cg/models/workflow/mutant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-05-04 13:15:21.000000 cg-29.6.0/cg/resources/20181012_Indices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-04 13:15:21.000000 cg-29.6.0/cg/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-04 13:15:21.000000 cg-29.6.0/cg/resources/rnafusion_bundle_filenames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18089 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/server/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/server/invoices/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/server/invoices/templates/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/invoices/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-04 13:15:21.000000 cg-29.6.0/cg/server/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/api/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/api/find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32042 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/api/find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39247 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_case_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/filters/status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29319 2023-05-04 13:15:21.000000 cg-29.6.0/cg/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/utils/checksum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/checksum/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/utils/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/click/EnumChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg/utils/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/flask/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-04 13:15:21.000000 cg-29.6.0/cg/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/cg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-04 13:15:32.000000 cg-29.6.0/cg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39785 2023-05-04 13:15:32.000000 cg-29.6.0/cg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:15:32.000000 cg-29.6.0/cg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 13:15:32.000000 cg-29.6.0/cg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:15:32.000000 cg-29.6.0/cg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-04 13:15:32.000000 cg-29.6.0/cg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 13:15:32.000000 cg-29.6.0/cg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 13:15:21.000000 cg-29.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 13:15:21.000000 cg-29.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:15:32.000000 cg-29.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-04 13:15:21.000000 cg-29.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/cgstats/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/cgstats/crud/test_create_novaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/cgstats/crud/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/cgstats/parsers/test_adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/cgstats/parsers/test_conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/cgstats/parsers/test_demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/cgstats/parsers/test_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/cgstats/parsers/test_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/cgstats/test_cgstats_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/cgstats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/coverage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/coverage/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/crunchy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/crunchy/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/crunchy/test_spring_decompression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/demultiplex/test_convert_to_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/demultiplex/test_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/gens/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/gens/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/gens/test_gens_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/gt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/gt/test_gt_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/hk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/hk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/hk/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/hk/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/hk/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/hk/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/hk/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/lims/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/lims/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/loqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/loqus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/loqus/test_loqusdb_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/madeline/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/madeline/test_madeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/mip/test_config_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/mutacc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/mutacc_auto/test_mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/orderform/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/orderform/test_orderform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/scout/test_scout_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/slurm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/test_apps_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/test_osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/apps/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-04 13:15:21.000000 cg-29.6.0/tests/apps/vogue/test_vogue_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/add/test_cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/add/test_cli_add_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/backup/test_backup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/clean/test_rsync_past_run_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/delete/test_cli_delete_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/deliver/test_run_deliver_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/demultiplex/test_add_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/demultiplex/test_stats_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/generate/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/generate/test_cli_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/get/test_cli_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/get/test_cli_get_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/set/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/set/test_cli_set_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/store/test_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/test_cli_status_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/upload/test_cli_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    31891 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15354 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/fastq/test_fastq_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/fluffy/test_cli_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/microsalt/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/workflow/microsalt/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/microsalt/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/microsalt/test_microsalt_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/taxprofiler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-04 13:15:21.000000 cg-29.6.0/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64049 2023-05-04 13:15:21.000000 cg-29.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/DEMUX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/analysis/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/analysis/balsamic/tn_wgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/analysis/microsalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/analysis/mip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/analysis/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/analysis/sample_coverage.bed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/balsamic/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/crunchy/spring_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters_different_index_cycles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/hiseq_run/
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/fluffy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/fluffy/2020-23219-05/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/fluffy/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/gt/yellowhog.bcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/madeline/madeline.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/mip/dna/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/mip/dna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/mip/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/mip/rna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/mip/sample_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/scout/panel_export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/apps/shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/apps/shipping/scout-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/cgweb_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/cgweb_orders/sarscov2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/data/hkstore.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/data/yellowhog/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/data/yellowhog/pedigree.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/io/example_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/io/example_json.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/orderforms/
+-rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/1508.27.balsamic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/1508.27.fastq.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/1508.27.mip.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/1604.15.rml.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/1605.10.metagenome.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/fixtures/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/report/case_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-04 13:15:21.000000 cg-29.6.0/tests/fixtures/report/lims_family.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-04 13:15:21.000000 cg-29.6.0/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-04 13:15:21.000000 cg-29.6.0/tests/io/test_io_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-04 13:15:21.000000 cg-29.6.0/tests/io/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-04 13:15:21.000000 cg-29.6.0/tests/io/test_io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-04 13:15:21.000000 cg-29.6.0/tests/io/test_io_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/archive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/archive/test_archiving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24603 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/backup/test_meta_pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/clean/test_clean_demultiplexed_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/clean/test_clean_flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/deliver/test_delivery_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/demultiplex/test_delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/demultiplex/test_rename_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/encryption/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/observations/test_meta_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/orders/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19944 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29129 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/orders/test_ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/report/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/report/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/report/test_report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/rsync/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/test_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/transfer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/transfer/test_meta_transfer_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/transfer/test_meta_transfer_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/gisaid/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/upload/gisaid/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/upload/mutacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/nipt/test_nipt_upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32161 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/test_upload_genotypes_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/upload/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/upload/vogue/test_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/workflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-04 13:15:21.000000 cg-29.6.0/tests/meta/workflow/test_prepare_fastq_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/hk_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/limsmock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/madeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/osticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/process_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/store_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-04 13:15:21.000000 cg-29.6.0/tests/mocks/tb_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/models/demultiplexing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/demultiplexing/test_demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/demultiplexing/test_flowcell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/demultiplexing/test_run_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/mip/test_mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/mip/test_mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/nextflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/nextflow/test_nextflow_deliver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/observations/test_observations_input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/report/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/test_cg_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/test_compression_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/test_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 13:15:21.000000 cg-29.6.0/tests/models/test_flowcell_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-04 13:15:21.000000 cg-29.6.0/tests/server/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-04 13:15:21.000000 cg-29.6.0/tests/server/test_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-04 13:15:21.000000 cg-29.6.0/tests/server/test_server_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 13:15:21.000000 cg-29.6.0/tests/small_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/store/api/add/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/add/test_store_add_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/add/test_store_add_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/add/test_store_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/add/test_store_add_flow_celll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19418 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/store/api/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/delete/test_store_api_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/store/api/find/
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/find/test_find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/find/test_find_basic_data_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28823 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/find/test_find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/find/test_find_business_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/find/test_find_business_data_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/find/test_find_business_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/store/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/status/test_analyses_to_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/status/test_analyses_to_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/status/test_store_api_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/status/test_store_api_status_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/status/test_store_api_status_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/status/test_store_api_status_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/status/test_store_api_status_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/status/test_store_api_status_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39481 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26900 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30278 2023-05-04 13:15:21.000000 cg-29.6.0/tests/store_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-04 13:15:21.000000 cg-29.6.0/tests/test_store_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:32.000000 cg-29.6.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:15:21.000000 cg-29.6.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-04 13:15:21.000000 cg-29.6.0/tests/utils/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-04 13:15:21.000000 cg-29.6.0/tests/utils/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-04 13:15:21.000000 cg-29.6.0/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-04 13:15:21.000000 cg-29.6.0/tests/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-04 13:15:21.000000 cg-29.6.0/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-04 13:15:21.000000 cg-29.6.0/tests/utils/test_utils.py
```

### Comparing `cg-29.5.7/PKG-INFO` & `cg-29.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 29.5.7
+Version: 29.6.0
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-29.5.7/README.md` & `cg-29.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/crud/create.py` & `cg-29.6.0/cg/apps/cgstats/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/crud/delete.py` & `cg-29.6.0/cg/apps/cgstats/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/crud/find.py` & `cg-29.6.0/cg/apps/cgstats/crud/find.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/db/models/base.py` & `cg-29.6.0/cg/apps/cgstats/db/models/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/db/models/datasource.py` & `cg-29.6.0/cg/apps/cgstats/db/models/datasource.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/db/models/demux.py` & `cg-29.6.0/cg/apps/cgstats/db/models/demux.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/db/models/flowcell.py` & `cg-29.6.0/cg/apps/cgstats/db/models/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/db/models/project.py` & `cg-29.6.0/cg/apps/cgstats/db/models/project.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/db/models/sample.py` & `cg-29.6.0/cg/apps/cgstats/db/models/sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/db/models/support_params.py` & `cg-29.6.0/cg/apps/cgstats/db/models/support_params.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/db/models/unaligned.py` & `cg-29.6.0/cg/apps/cgstats/db/models/unaligned.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/db/models/version.py` & `cg-29.6.0/cg/apps/cgstats/db/models/version.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/demux_sample.py` & `cg-29.6.0/cg/apps/cgstats/demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/dragen_demux_sample.py` & `cg-29.6.0/cg/apps/cgstats/dragen_demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/parsers/adapter_metrics.py` & `cg-29.6.0/cg/apps/cgstats/parsers/adapter_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/parsers/conversion_stats.py` & `cg-29.6.0/cg/apps/cgstats/parsers/conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/parsers/demux_stats.py` & `cg-29.6.0/cg/apps/cgstats/parsers/demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py` & `cg-29.6.0/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/parsers/quality_metrics.py` & `cg-29.6.0/cg/apps/cgstats/parsers/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/parsers/run_info.py` & `cg-29.6.0/cg/apps/cgstats/parsers/run_info.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/cgstats/stats.py` & `cg-29.6.0/cg/apps/cgstats/stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/coverage/api.py` & `cg-29.6.0/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/crunchy/crunchy.py` & `cg-29.6.0/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/crunchy/files.py` & `cg-29.6.0/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/crunchy/sbatch.py` & `cg-29.6.0/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/demultiplex/demultiplex_api.py` & `cg-29.6.0/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/demultiplex/demux_report.py` & `cg-29.6.0/cg/apps/demultiplex/demux_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/demultiplex/sample_sheet/create.py` & `cg-29.6.0/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/demultiplex/sample_sheet/dummy_sample.py` & `cg-29.6.0/cg/apps/demultiplex/sample_sheet/dummy_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/demultiplex/sample_sheet/index.py` & `cg-29.6.0/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/demultiplex/sample_sheet/models.py` & `cg-29.6.0/cg/apps/demultiplex/sample_sheet/models.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py` & `cg-29.6.0/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/demultiplex/sample_sheet/validate.py` & `cg-29.6.0/cg/apps/demultiplex/sample_sheet/validate.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/demultiplex/sbatch.py` & `cg-29.6.0/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/gens.py` & `cg-29.6.0/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/gt.py` & `cg-29.6.0/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/hermes/hermes_api.py` & `cg-29.6.0/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/hermes/models.py` & `cg-29.6.0/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/housekeeper/hk.py` & `cg-29.6.0/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/invoice/render.py` & `cg-29.6.0/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-29.6.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-29.6.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-29.6.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-29.6.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/lims/api.py` & `cg-29.6.0/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/lims/batch.py` & `cg-29.6.0/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/lims/order.py` & `cg-29.6.0/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/lims/samplesheet.py` & `cg-29.6.0/cg/apps/lims/samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/loqus.py` & `cg-29.6.0/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/madeline/api.py` & `cg-29.6.0/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/mip/confighandler.py` & `cg-29.6.0/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/mutacc_auto.py` & `cg-29.6.0/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/orderform/excel_orderform_parser.py` & `cg-29.6.0/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/orderform/json_orderform_parser.py` & `cg-29.6.0/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/orderform/orderform_parser.py` & `cg-29.6.0/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/osticket.py` & `cg-29.6.0/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/scout/scout_export.py` & `cg-29.6.0/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/scout/scoutapi.py` & `cg-29.6.0/cg/apps/scout/scoutapi.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import List, Optional
 
 from cg.apps.scout.scout_export import ScoutExportCase, Variant
 from cg.constants.constants import FileFormat
 from cg.constants.gene_panel import GENOME_BUILD_37
+from cg.constants.scout_upload import ScoutCustomCaseReportTags
 from cg.exc import ScoutUploadError
 from cg.io.controller import ReadFile, ReadStream
 from cg.models.scout.scout_load_config import ScoutLoadConfig
 from cg.utils.commands import Process
 
 LOG = logging.getLogger(__name__)
 
@@ -38,15 +39,15 @@
         load_command = ["load", "case", str(scout_load_config)]
         if existing_case:
             if force or scout_load_config_object.analysis_date > existing_case.analysis_date:
                 load_command.append("--update")
                 LOG.info("update existing Scout case")
             else:
                 existing_date = existing_case.analysis_date.date()
-                LOG.warning("analysis of case already loaded: %s", existing_date)
+                LOG.warning(f"Analysis of case already loaded: {existing_date}")
                 return
         LOG.debug("load new Scout case")
         self.process.run_command(load_command)
         LOG.debug("Case loaded successfully to Scout")
 
     def update_alignment_file(self, case_id: str, sample_id: str, alignment_path: Path):
         """Update alignment file for individual in case"""
@@ -64,101 +65,89 @@
 
     def export_panels(self, panels: List[str], build: str = GENOME_BUILD_37) -> List[str]:
         """Pass through to export of a list of gene panels.
 
         Return list of lines in bed format
         """
         export_panels_command = ["export", "panel", "--bed"]
-        for panel_id in panels:
-            export_panels_command.append(panel_id)
+        export_panels_command.extend(iter(panels))
 
         if build:
             export_panels_command.extend(["--build", build])
 
         try:
             self.process.run_command(export_panels_command)
             if not self.process.stdout:
                 return []
         except CalledProcessError:
             LOG.info("Could not find panels")
             return []
 
-        return [line for line in self.process.stdout_lines()]
+        return list(self.process.stdout_lines())
 
-    def get_genes(self, panel_id: str, build: str = None) -> list:
-        """Fetch panel genes.
-
-        Args:
-            panel_id (str): unique id for the panel
-            build (str): version of the panel. If 'None' latest version will be returned
-
-        Returns:
-            panel genes: panel genes list
-        """
-        # This can be run from CLI with `scout export panels <panel1> `
+    def get_genes(self, panel_id: str, build: str = None) -> List[dict]:
+        """Return panel genes."""
         export_panel_command = ["export", "panel", panel_id]
         if build:
             export_panel_command.extend(["--build", build])
 
         try:
             self.process.run_command(export_panel_command)
             if not self.process.stdout:
                 return []
         except CalledProcessError:
-            LOG.info("Could not find panel %s", panel_id)
+            LOG.info(f"Could not find panel {panel_id}")
             return []
 
         panel_genes = []
         for gene_line in self.process.stdout_lines():
             if gene_line.startswith("#"):
                 continue
             gene_info = gene_line.strip().split("\t")
-            if not len(gene_info) > 1:
+            if len(gene_info) <= 1:
                 continue
             panel_genes.append({"hgnc_id": int(gene_info[0]), "hgnc_symbol": gene_info[1]})
 
         return panel_genes
 
     def get_causative_variants(self, case_id: str) -> List[Variant]:
         """
-        Get causative variants for a case
+        Get causative variants for a case.
         """
-        # These commands can be run with `scout export variants`
         get_causatives_command = ["export", "variants", "--json", "--case-id", case_id]
         try:
             self.process.run_command(get_causatives_command)
             if not self.process.stdout:
                 return []
         except CalledProcessError:
-            LOG.warning("Could not find case %s in scout", case_id)
+            LOG.warning(f"Could not find case {case_id} in scout")
             return []
-        variants: List[Variant] = []
-        for variant_info in ReadStream.get_content_from_stream(
-            file_format=FileFormat.JSON, stream=self.process.stdout
-        ):
-            variants.append(Variant(**variant_info))
+        variants: List[Variant] = [
+            Variant(**variant_info)
+            for variant_info in ReadStream.get_content_from_stream(
+                file_format=FileFormat.JSON, stream=self.process.stdout
+            )
+        ]
+
         return variants
 
     def get_case(self, case_id: str) -> Optional[ScoutExportCase]:
         """Fetch a case from Scout"""
         cases: List[ScoutExportCase] = self.get_cases(case_id=case_id)
-        if not cases:
-            return None
-        return cases[0]
+        return cases[0] if cases else None
 
     def get_cases(
         self,
         case_id: Optional[str] = None,
         reruns: bool = False,
         finished: bool = False,
         status: Optional[str] = None,
         days_ago: int = None,
     ) -> List[ScoutExportCase]:
         """Interact with cases existing in the database."""
-        # These commands can be run with `scout export cases`
         get_cases_command = ["export", "cases", "--json"]
         if case_id:
             get_cases_command.extend(["--case-id", case_id])
 
         elif status:
             get_cases_command.extend(["--status", status])
 
@@ -180,146 +169,107 @@
             LOG.info("Could not find cases")
             return []
 
         cases: List[ScoutExportCase] = []
         for case_export in ReadStream.get_content_from_stream(
             file_format=FileFormat.JSON, stream=self.process.stdout
         ):
-            LOG.info("Validating case %s", case_export.get("_id"))
+            LOG.info(f"Validating case {case_export.get('_id')}")
             cases.append(ScoutExportCase(**case_export))
         return cases
 
     def get_solved_cases(self, days_ago: int) -> List[ScoutExportCase]:
         """
-        Get cases solved within chosen timespan
-
-        Args:
-            days_ago (int): Maximum days ago a case has been solved
-
-        Return:
-            cases (list): list of cases
+        Get cases solved within chosen time span.
         """
         return self.get_cases(status="solved", days_ago=days_ago)
 
     def upload_delivery_report(self, report_path: str, case_id: str, update: bool = False) -> None:
-        """Load a delivery report into a case in the database
-
+        """Load a delivery report into a case in the database.
         If the report already exists the function will exit.
         If the user want to load a report that is already in the database
-        'update' has to be 'True'
-
-        Args:
-            report_path (string):       Path to delivery report
-            case_id     (string):       Case identifier
-            update      (bool):         If an existing report should be replaced
+        'update' has to be 'True'."""
 
-        Returns:
-            updated_case(dict)
-
-        """
-        # This command can be run with `scout load delivery-report <CASE-ID> <REPORT-PATH>`
-        upload_command = ["load", "delivery-report", case_id, report_path]
+        upload_command: List[str] = ["load", "delivery-report", case_id, report_path]
 
         if update:
             upload_command.append("--update")
 
         try:
-            LOG.info("Uploading delivery report %s to case %s", report_path, case_id)
+            LOG.info(f"Uploading delivery report {report_path} to case {case_id}")
             self.process.run_command(upload_command)
         except CalledProcessError:
             LOG.warning("Something went wrong when uploading delivery report")
 
-    def upload_fusion_report(
-        self, case_id: str, report_path: str, research: bool, update: bool
-    ) -> None:
-        """Load a fusion report into a case in the database
-
-        Args:
-            report_path (string):       Path to delivery report
-            case_id     (string):       Case identifier
-            research    (bool):         Research report
-            update      (bool):         If an existing report should be replaced
-        Returns:
-            Nothing
-        """
-
-        # This command can be run with
-        # `scout load gene-fusion-report [-r] <case_id> <path/to/research_gene_fusion_report.pdf>`
-        upload_command = ["load", "gene-fusion-report"]
+    def upload_report(self, case_id: str, report_path: str, report_type: str) -> None:
+        """Load report into a case in the database."""
 
-        if research:
-            upload_command.append("--research")
-
-        if update:
-            upload_command.append("--update")
-
-        upload_command.extend([case_id, report_path])
+        upload_report_command: List[str] = [
+            "load",
+            "report",
+            "-t",
+            report_type,
+            case_id,
+            report_path,
+        ]
 
         try:
-            LOG.info("Uploading fusion report %s to case %s", report_path, case_id)
-            self.process.run_command(upload_command)
+            LOG.info(f"Uploading {report_type} report to case {case_id}")
+            self.process.run_command(upload_report_command)
         except CalledProcessError:
-            raise ScoutUploadError("Something went wrong when uploading fusion report")
+            LOG.warning(f"Something went wrong when uploading {report_type} for case {case_id}")
 
-    def upload_splice_junctions_bed(self, file_path: str, case_id: str, customer_sample_id: str):
-        """Load a splice junctions bed file into a case in the database.
+    def upload_fusion_report(self, case_id: str, report_path: str, research: bool) -> None:
+        """Load a fusion report into a case in the database."""
 
-        Args:
-            file_path           (string):       Path to delivery report
-            case_id             (string):       Case identifier
-            customer_sample_id  (string):       Customers sample identifier
-        Returns:
-            updated_case(dict)
+        report_type: str = (
+            ScoutCustomCaseReportTags.GENE_FUSION_RESEARCH
+            if research
+            else ScoutCustomCaseReportTags.GENE_FUSION
+        )
+        self.upload_report(case_id=case_id, report_path=report_path, report_type=report_type)
 
-        """
+    def upload_splice_junctions_bed(self, file_path: str, case_id: str, customer_sample_id: str):
+        """Load a splice junctions bed file into a case in the database."""
 
-        # This command can be run with
-        # `scout update individual -c <case_id> -n <customer_sample_id> splice_junctions_bed
-        #   <path/to/junction_file.bed>`
-        upload_command = [
+        upload_command: List[str] = [
             "update",
             "individual",
             "-c",
             case_id,
             "-n",
             customer_sample_id,
             "splice_junctions_bed",
             file_path,
         ]
 
         try:
-            LOG.info("Uploading splice junctions bed file %s to case %s", file_path, case_id)
+            LOG.info("Uploading splice junctions bed file {file_path} to case {case_id}")
             self.process.run_command(upload_command)
-        except CalledProcessError:
-            raise ScoutUploadError("Something went wrong when uploading splice junctions bed file")
-
-    def upload_rna_coverage_bigwig(self, file_path: str, case_id: str, customer_sample_id: str):
-        """Load a rna coverage bigwig file into a case in the database
+        except CalledProcessError as error:
+            raise ScoutUploadError(
+                "Something went wrong when uploading splice junctions bed file"
+            ) from error
 
-        Args:
-            file_path           (string):       Path to delivery report
-            case_id             (string):       Case identifier
-            customer_sample_id  (string):       Customers sample identifier
-        Returns:
-            updated_case(dict)
-
-        """
+    def upload_rna_coverage_bigwig(
+        self, file_path: str, case_id: str, customer_sample_id: str
+    ) -> None:
+        """Load a rna coverage bigwig file into a case in the database."""
 
-        # This command can be run with
-        # `scout update individual -c <case_id> -n <customer_sample_id> rna_coverage_bigwig
-        #         <path/to/coverage_file.bigWig>`
-        upload_command = [
+        upload_command: List[str] = [
             "update",
             "individual",
             "-c",
             case_id,
             "-n",
             customer_sample_id,
             "rna_coverage_bigwig",
             file_path,
         ]
 
         try:
-            LOG.info("Uploading rna coverage bigwig file %s to case %s", file_path, case_id)
+            LOG.info(f"Uploading rna coverage bigwig file {file_path} to case {case_id}")
             self.process.run_command(upload_command)
-        except CalledProcessError:
-            raise ScoutUploadError("Something went wrong when uploading rna coverage bigwig file")
+        except CalledProcessError as error:
+            raise ScoutUploadError(
+                "Something went wrong when uploading rna coverage bigwig file"
+            ) from error
```

### Comparing `cg-29.5.7/cg/apps/slurm/sbatch.py` & `cg-29.6.0/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/slurm/slurm_api.py` & `cg-29.6.0/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/tb/api.py` & `cg-29.6.0/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/tb/models.py` & `cg-29.6.0/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/apps/vogue.py` & `cg-29.6.0/cg/apps/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/add.py` & `cg-29.6.0/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/backup.py` & `cg-29.6.0/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/base.py` & `cg-29.6.0/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/clean.py` & `cg-29.6.0/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/compress/base.py` & `cg-29.6.0/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/compress/fastq.py` & `cg-29.6.0/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/compress/helpers.py` & `cg-29.6.0/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/delete/case.py` & `cg-29.6.0/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/delete/cases.py` & `cg-29.6.0/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/delete/observations.py` & `cg-29.6.0/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/deliver/base.py` & `cg-29.6.0/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/demultiplex/add.py` & `cg-29.6.0/cg/cli/demultiplex/add.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/demultiplex/base.py` & `cg-29.6.0/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/demultiplex/demux.py` & `cg-29.6.0/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/demultiplex/finish.py` & `cg-29.6.0/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/demultiplex/report.py` & `cg-29.6.0/cg/cli/demultiplex/report.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/demultiplex/sample_sheet.py` & `cg-29.6.0/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/export.py` & `cg-29.6.0/cg/cli/export.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/generate/report/base.py` & `cg-29.6.0/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/generate/report/options.py` & `cg-29.6.0/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/generate/report/utils.py` & `cg-29.6.0/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/get.py` & `cg-29.6.0/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/set/base.py` & `cg-29.6.0/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/set/case.py` & `cg-29.6.0/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/set/cases.py` & `cg-29.6.0/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/status.py` & `cg-29.6.0/cg/cli/status.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/store/fastq.py` & `cg-29.6.0/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/store/store.py` & `cg-29.6.0/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/transfer.py` & `cg-29.6.0/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/base.py` & `cg-29.6.0/cg/cli/upload/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from cg.cli.upload.mutacc import process_solved, processed_solved
 from cg.cli.upload.nipt import nipt
 from cg.cli.upload.observations import available_observations, observations
 from cg.cli.upload.scout import (
     create_scout_load_config,
     scout,
     upload_case_to_scout,
+    upload_multiqc_to_scout,
     upload_rna_fusion_report_to_scout,
     upload_rna_junctions_to_scout,
     upload_rna_to_scout,
 )
 from cg.cli.upload.utils import suggest_cases_to_upload
 from cg.cli.upload.validate import validate
 from cg.constants import Pipeline
@@ -131,11 +132,12 @@
 upload.add_command(processed_solved)
 upload.add_command(scout)
 upload.add_command(upload_case_to_scout)
 upload.add_command(upload_delivery_report_to_scout)
 upload.add_command(upload_rna_fusion_report_to_scout)
 upload.add_command(upload_rna_junctions_to_scout)
 upload.add_command(upload_rna_to_scout)
+upload.add_command(upload_multiqc_to_scout)
 upload.add_command(observations)
 upload.add_command(available_observations)
 upload.add_command(validate)
 upload.add_command(vogue)
```

### Comparing `cg-29.5.7/cg/cli/upload/clinical_delivery.py` & `cg-29.6.0/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/coverage.py` & `cg-29.6.0/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/delivery_report.py` & `cg-29.6.0/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/fohm.py` & `cg-29.6.0/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/genotype.py` & `cg-29.6.0/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/gens.py` & `cg-29.6.0/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/gisaid.py` & `cg-29.6.0/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/mutacc.py` & `cg-29.6.0/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/nipt/base.py` & `cg-29.6.0/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/nipt/ftp.py` & `cg-29.6.0/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/nipt/statina.py` & `cg-29.6.0/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/observations/observations.py` & `cg-29.6.0/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/observations/utils.py` & `cg-29.6.0/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/scout.py` & `cg-29.6.0/cg/cli/upload/scout.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from typing import Dict, Optional
 
 import click
 from housekeeper.store.models import File, Version
 
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.apps.scout.scoutapi import ScoutAPI
+from cg.constants import Pipeline
+from cg.constants.constants import FileFormat
+from cg.constants.scout_upload import ScoutCustomCaseReportTags
 from cg.cli.upload.utils import suggest_cases_to_upload
 from cg.constants import Pipeline
 from cg.constants.constants import FileFormat
-from cg.exc import CgDataError, ScoutUploadError
 from cg.io.controller import WriteStream
 from cg.meta.upload.upload_api import UploadAPI
 from cg.meta.upload.scout.uploadscoutapi import UploadScoutAPI
 from cg.meta.workflow.balsamic import BalsamicAnalysisAPI
 from cg.meta.workflow.balsamic_umi import BalsamicUmiAnalysisAPI
 from cg.meta.workflow.mip_dna import MipDNAAnalysisAPI
 from cg.meta.workflow.mip_rna import MipRNAAnalysisAPI
@@ -113,16 +115,16 @@
 
     try:
         LOG.info("Add config file to housekeeper")
         scout_upload_api.add_scout_config_to_hk(
             config_file_path=file_path, case_id=case_id, delete=re_upload
         )
     except FileExistsError as error:
-        LOG.warning("%s, consider removing the file from housekeeper and try again", str(error))
-        raise click.Abort
+        LOG.warning(f"{error}, consider removing the file from housekeeper and try again")
+        raise click.Abort from error
 
 
 @click.command(name="upload-case-to-scout")
 @click.option(
     "-r",
     "--re-upload",
     is_flag=True,
@@ -166,108 +168,89 @@
     is_flag=True,
     help="re-upload existing fusion report",
 )
 @click.argument("case_id")
 @click.pass_context
 def upload_rna_to_scout(
     context, case_id: str, dry_run: bool, update_fusion_report: bool, research: bool
-) -> int:
-    """Upload an RNA case's gene fusion report and junction splice files for all samples connect via subject_id
-
-    Args:
-        case_id                 (string):       RNA case identifier
-        dry_run                 (bool):         Skip uploading
-        research                (bool):         Upload research report instead of clinical
-        update_fusion_report    (bool):         Overwrite existing fusion report
-    Returns:
-
-    """
+) -> None:
+    """Upload an RNA case's gene fusion report and junction splice files for all samples connect via subject_id."""
 
     LOG.info("----------------- UPLOAD RNA TO SCOUT -----------------------")
 
-    result: int = context.invoke(
+    context.invoke(upload_multiqc_to_scout, case_id=case_id, dry_run=dry_run)
+    context.invoke(
         upload_rna_fusion_report_to_scout,
         case_id=case_id,
         dry_run=dry_run,
         research=research,
         update=update_fusion_report,
     )
-    if result == 0:
-        result = context.invoke(upload_rna_junctions_to_scout, case_id=case_id, dry_run=dry_run)
-    return result
+    context.invoke(upload_rna_junctions_to_scout, case_id=case_id, dry_run=dry_run)
 
 
 @click.command(name="rna-fusion-report-to-scout")
 @click.option("--dry-run", is_flag=True)
 @click.option("--research", is_flag=True)
-@click.option(
-    "-u",
-    "--update",
-    is_flag=True,
-    help="Overwrite existing report",
-)
 @click.argument("case_id")
 @click.pass_obj
 def upload_rna_fusion_report_to_scout(
-    context: CGConfig, dry_run: bool, case_id: str, update: bool, research: bool
-) -> int:
-    """Upload fusion report file for a case to Scout.
-    This can also be run as
-    `housekeeper get file -V --tag fusion --tag pdf --tag clinical/research <case_id>`
-    `scout load gene-fusion-report [-r] <case_id> <path/to/research_gene_fusion_report.pdf>`
-
-    Args:
-        dry_run     (bool):         Skip uploading
-        case_id     (string):       RNA case identifier
-        research    (bool):         Upload research report instead of clinical
-        update      (bool):         Overwrite existing report
-    Returns:
+    context: CGConfig, dry_run: bool, case_id: str, research: bool
+) -> None:
+    """Upload fusion report file for a case to Scout."""
 
-    """
     LOG.info("----------------- UPLOAD RNA FUSION REPORT TO SCOUT -----------------------")
 
     scout_upload_api: UploadScoutAPI = context.meta_apis["upload_api"].scout_upload_api
-    try:
-        scout_upload_api.upload_fusion_report_to_scout(
-            dry_run=dry_run, research=research, case_id=case_id, update=update
-        )
-    except (CgDataError, ScoutUploadError) as error:
-        LOG.error(error)
-        return 1
-    return 0
+    scout_upload_api.upload_fusion_report_to_scout(
+        dry_run=dry_run, research=research, case_id=case_id
+    )
 
 
 @click.command(name="rna-junctions-to-scout")
 @click.option("--dry-run", is_flag=True)
 @click.argument("case_id")
 @click.pass_obj
-def upload_rna_junctions_to_scout(context: CGConfig, case_id: str, dry_run: bool) -> int:
-    """Upload RNA junctions splice files to Scout.
-        This can also be run as
-        `housekeeper get file -V --tag junction --tag bed <sample_id>`
-        `scout update individual -c <case_id> -n <customer_sample_id> splice_junctions_bed <path/to/junction_file.bed>`
-        `housekeeper get file -V --tag coverage --tag bigwig <sample_id>`
-        scout update individual -c <case_id> -n <customer_sample_id> rna_coverage_bigwig <path/to/coverage_file.bigWig>
-    `   ```
-
-        Args:
-            dry_run     (bool):         Skip uploading
-            case_id     (string):       RNA case identifier
-        Returns:
-
-    """
+def upload_rna_junctions_to_scout(context: CGConfig, case_id: str, dry_run: bool) -> None:
+    """Upload RNA junctions splice files to Scout."""
     LOG.info("----------------- UPLOAD RNA JUNCTIONS TO SCOUT -----------------------")
 
     scout_upload_api: UploadScoutAPI = context.meta_apis["upload_api"].scout_upload_api
-    try:
-        scout_upload_api.upload_rna_junctions_to_scout(dry_run=dry_run, case_id=case_id)
-    except (CgDataError, ScoutUploadError) as error:
-        LOG.error(error)
-        return 1
-    return 0
+
+    scout_upload_api.upload_rna_junctions_to_scout(dry_run=dry_run, case_id=case_id)
+
+
+@click.command(name="multiqc-to-scout")
+@click.option("--dry-run", is_flag=True)
+@click.argument("case_id")
+@click.pass_obj
+def upload_multiqc_to_scout(context: CGConfig, case_id: str, dry_run: bool) -> None:
+    """Upload multiqc report to Scout."""
+    LOG.info("----------------- UPLOAD MULTIQC TO SCOUT -----------------------")
+
+    scout_upload_api: UploadScoutAPI = context.meta_apis["upload_api"].scout_upload_api
+    status_db: Store = context.status_db
+    case: Family = status_db.get_case_by_internal_id(internal_id=case_id)
+    scout_report_type, multiqc_report = scout_upload_api.get_multiqc_html_report(
+        case_id=case_id, pipeline=case.data_analysis
+    )
+    if scout_report_type == ScoutCustomCaseReportTags.MULTIQC_RNA:
+        scout_upload_api.upload_rna_report_to_dna_case_in_scout(
+            dry_run=dry_run,
+            rna_case_id=case_id,
+            report_type=scout_report_type,
+            report_file=multiqc_report,
+        )
+    else:
+        scout_upload_api.upload_report_to_scout(
+            dry_run=dry_run,
+            case_id=case_id,
+            report_type=scout_report_type,
+            report_file=multiqc_report,
+        )
 
 
 def get_upload_api(case: Family, cg_config: CGConfig) -> UploadAPI:
     """Return the upload API based on the data analysis type"""
 
     analysis_apis: Dict[Pipeline, UploadAPI] = {
         Pipeline.BALSAMIC: BalsamicAnalysisAPI,
```

### Comparing `cg-29.5.7/cg/cli/upload/utils.py` & `cg-29.6.0/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/validate.py` & `cg-29.6.0/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/upload/vogue.py` & `cg-29.6.0/cg/cli/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/balsamic/base.py` & `cg-29.6.0/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/balsamic/options.py` & `cg-29.6.0/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/balsamic/pon.py` & `cg-29.6.0/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/balsamic/qc.py` & `cg-29.6.0/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/balsamic/umi.py` & `cg-29.6.0/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/base.py` & `cg-29.6.0/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/commands.py` & `cg-29.6.0/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/fastq/base.py` & `cg-29.6.0/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/fluffy/base.py` & `cg-29.6.0/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/microsalt/base.py` & `cg-29.6.0/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/mip/base.py` & `cg-29.6.0/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/mip/options.py` & `cg-29.6.0/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/mip_dna/base.py` & `cg-29.6.0/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/mip_rna/base.py` & `cg-29.6.0/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/mutant/base.py` & `cg-29.6.0/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/nextflow/options.py` & `cg-29.6.0/cg/cli/workflow/nextflow/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/rnafusion/base.py` & `cg-29.6.0/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/rnafusion/options.py` & `cg-29.6.0/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/cli/workflow/taxprofiler/base.py` & `cg-29.6.0/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/__init__.py` & `cg-29.6.0/cg/constants/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,14 @@
     SEX_OPTIONS,
     STATUS_OPTIONS,
     DataDelivery,
     FileExtensions,
     FlowCellStatus,
 )
 from cg.constants.gene_panel import GenePanelMasterList
-from cg.constants.housekeeper_tags import HK_FASTQ_TAGS, SequencingFileTag
+from cg.constants.housekeeper_tags import HK_FASTQ_TAGS, HK_MULTIQC_HTML_TAG, SequencingFileTag
 from cg.constants.paths import TMP_DIR
 from cg.constants.priority import Priority
 from cg.constants.process import EXIT_FAIL, EXIT_SUCCESS, RETURN_SUCCESS
 from cg.constants.report import *
 from cg.constants.sample_sources import ANALYSIS_SOURCES, METAGENOME_SOURCES
 from cg.constants.symbols import SINGLE_QUOTE, SPACE
```

### Comparing `cg-29.5.7/cg/constants/compression.py` & `cg-29.6.0/cg/constants/compression.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/constants.py` & `cg-29.6.0/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/delivery.py` & `cg-29.6.0/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/demultiplexing.py` & `cg-29.6.0/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/encryption.py` & `cg-29.6.0/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/gene_panel.py` & `cg-29.6.0/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/housekeeper_tags.py` & `cg-29.6.0/cg/constants/housekeeper_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     CGSTATS_LOG: str = "log"
     FASTQ: str = "fastq"
     SAMPLE_SHEET: str = "samplesheet"
     SPRING: str = "spring"
     SPRING_METADATA: str = "spring-metadata"
 
 
+HK_MULTIQC_HTML_TAG = ["multiqc-html"]
+
 HK_FASTQ_TAGS = [SequencingFileTag.FASTQ]
 
 HK_DELIVERY_REPORT_TAG = "delivery-report"
 
 
 class HkMipAnalysisTag:
     CONFIG: List[str] = ["mip-config"]
```

### Comparing `cg-29.5.7/cg/constants/lims.py` & `cg-29.6.0/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/nextflow.py` & `cg-29.6.0/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/observations.py` & `cg-29.6.0/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/orderforms.py` & `cg-29.6.0/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/priority.py` & `cg-29.6.0/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/report.py` & `cg-29.6.0/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/rnafusion.py` & `cg-29.6.0/cg/constants/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/scout_upload.py` & `cg-29.6.0/cg/constants/scout_upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,27 @@
-from typing import Dict, Set
+from cg.utils.enums import StrEnum
 
-from cgmodels.cg.constants import StrEnum
+from typing import Dict, Set
 
 
 class GenomeBuild(StrEnum):
     hg19: str = "37"
     hg38: str = "38"
 
 
+class ScoutCustomCaseReportTags(StrEnum):
+    DELIVERY: str = "delivery_report"
+    CNV: str = "cnv_report"
+    COV_QC: str = "coverage_qc_report"
+    MULTIQC: str = "multiqc"
+    MULTIQC_RNA: str = "multiqc_rna"
+    GENE_FUSION: str = "gene_fusion"
+    GENE_FUSION_RESEARCH: str = "gene_fusion_research"
+
+
 MIP_CASE_TAGS = dict(
     snv_vcf={"vcf-snv-clinical"},
     snv_research_vcf={"vcf-snv-research"},
     sv_vcf={"vcf-sv-clinical"},
     sv_research_vcf={"vcf-sv-research"},
     vcf_str={"vcf-str"},
     smn_tsv={"smn-calling"},
@@ -70,8 +80,9 @@
 )
 
 BALSAMIC_UMI_SAMPLE_TAGS = dict(
     bam_file={"umi-bam"},
     alignment_file={"umi-cram"},
 )
 
-RNAFUSION_SAMPLE_TAGS = dict()
+
+RNAFUSION_SAMPLE_TAGS = {}
```

### Comparing `cg-29.5.7/cg/constants/sequencing.py` & `cg-29.6.0/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/constants/subject.py` & `cg-29.6.0/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/exc.py` & `cg-29.6.0/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/io/api.py` & `cg-29.6.0/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/io/controller.py` & `cg-29.6.0/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/io/csv.py` & `cg-29.6.0/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/io/json.py` & `cg-29.6.0/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/io/yaml.py` & `cg-29.6.0/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/archive/ddn_dataflow.py` & `cg-29.6.0/cg/meta/archive/ddn_dataflow.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/backup/backup.py` & `cg-29.6.0/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/backup/pdc.py` & `cg-29.6.0/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/clean/api.py` & `cg-29.6.0/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/clean/demultiplexed_flow_cells.py` & `cg-29.6.0/cg/meta/clean/demultiplexed_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/clean/flow_cell_run_directories.py` & `cg-29.6.0/cg/meta/clean/flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/compress/compress.py` & `cg-29.6.0/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/compress/files.py` & `cg-29.6.0/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/deliver.py` & `cg-29.6.0/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/deliver_ticket.py` & `cg-29.6.0/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/demultiplex/delete_demultiplex_api.py` & `cg-29.6.0/cg/meta/demultiplex/delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/demultiplex/demux_post_processing.py` & `cg-29.6.0/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/demultiplex/files.py` & `cg-29.6.0/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/encryption/encryption.py` & `cg-29.6.0/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/invoice.py` & `cg-29.6.0/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/meta.py` & `cg-29.6.0/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/observations/balsamic_observations_api.py` & `cg-29.6.0/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/observations/mip_dna_observations_api.py` & `cg-29.6.0/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/observations/observations_api.py` & `cg-29.6.0/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/orders/api.py` & `cg-29.6.0/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/orders/case_submitter.py` & `cg-29.6.0/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/orders/fastq_submitter.py` & `cg-29.6.0/cg/meta/orders/fastq_submitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from cg.exc import OrderError
 from cg.meta.orders.lims import process_lims
 from cg.meta.orders.submitter import Submitter
 from cg.models.orders.order import OrderIn
 from cg.models.orders.sample_base import StatusEnum
 from cg.constants.priority import Priority
 from cg.store.models import Sample, Family, FamilySample, Customer, ApplicationVersion
+from cg.constants.constants import PrepCategory
 
 
 class FastqSubmitter(Submitter):
     def submit_order(self, order: OrderIn) -> dict:
         """Submit a batch of samples for FASTQ delivery."""
 
         project_data, lims_map = process_lims(
@@ -120,16 +121,15 @@
                         name=ticket_id,
                         panels=None,
                         priority=submitted_case["priority"],
                         ticket=ticket_id,
                     )
                 if (
                     not new_sample.is_tumour
-                    and new_sample.application_version.application.prep_category
-                    == PrepCategory.WHOLE_GENOME_SEQUENCING
+                    and new_sample.prep_category == PrepCategory.WHOLE_GENOME_SEQUENCING
                 ):
                     self.create_maf_case(sample_obj=new_sample)
                 case.customer = customer
                 new_relationship = self.status.relate_sample(
                     family=case, sample=new_sample, status=StatusEnum.unknown
                 )
                 new_delivery = self.status.add_delivery(destination="caesar", sample=new_sample)
```

### Comparing `cg-29.5.7/cg/meta/orders/lims.py` & `cg-29.6.0/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/orders/metagenome_submitter.py` & `cg-29.6.0/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/orders/microbial_submitter.py` & `cg-29.6.0/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/orders/pool_submitter.py` & `cg-29.6.0/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/orders/sars_cov_2_submitter.py` & `cg-29.6.0/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/orders/submitter.py` & `cg-29.6.0/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/orders/ticket_handler.py` & `cg-29.6.0/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/report/balsamic.py` & `cg-29.6.0/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/report/balsamic_umi.py` & `cg-29.6.0/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/report/field_validators.py` & `cg-29.6.0/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/report/mip_dna.py` & `cg-29.6.0/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/report/report_api.py` & `cg-29.6.0/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/report/templates/balsamic_report.html` & `cg-29.6.0/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/report/templates/bootstrap.html` & `cg-29.6.0/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/report/templates/mip-dna_report.html` & `cg-29.6.0/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/rsync/rsync_api.py` & `cg-29.6.0/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/tar/tar.py` & `cg-29.6.0/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/transfer/external_data.py` & `cg-29.6.0/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/transfer/flowcell.py` & `cg-29.6.0/cg/meta/transfer/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/transfer/lims.py` & `cg-29.6.0/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/balsamic/balsamic.py` & `cg-29.6.0/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/coverage.py` & `cg-29.6.0/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/fohm/fohm.py` & `cg-29.6.0/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/gisaid/constants.py` & `cg-29.6.0/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/gisaid/gisaid.py` & `cg-29.6.0/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/gisaid/models.py` & `cg-29.6.0/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/gt.py` & `cg-29.6.0/cg/meta/upload/gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,13 +129,11 @@
         return self.hk.files(version=version_id, tags=["genotype"]).all()
 
     @staticmethod
     def is_suitable_for_genotype_upload(case_obj: Family) -> bool:
         """Check if a cancer case is contains WGS and normal sample."""
 
         samples: List[Sample] = case_obj.samples
-        for sample in samples:
-            sample_prep_category: str = sample.application_version.application.prep_category
-            if not sample.is_tumour:
-                if PrepCategory.WHOLE_GENOME_SEQUENCING == sample_prep_category:
-                    return True
-        return False
+        return any(
+            (not sample.is_tumour and PrepCategory.WHOLE_GENOME_SEQUENCING == sample.prep_category)
+            for sample in samples
+        )
```

### Comparing `cg-29.5.7/cg/meta/upload/mip/mip_dna.py` & `cg-29.6.0/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/mip/mip_rna.py` & `cg-29.6.0/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/mutacc.py` & `cg-29.6.0/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/nipt/nipt.py` & `cg-29.6.0/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/rnafusion/rnafusion.py` & `cg-29.6.0/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-29.6.0/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-29.6.0/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/scout/hk_tags.py` & `cg-29.6.0/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/scout/mip_config_builder.py` & `cg-29.6.0/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-29.6.0/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/scout/scout_config_builder.py` & `cg-29.6.0/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/scout/uploadscoutapi.py` & `cg-29.6.0/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """File includes api to uploading data into Scout."""
 
 import logging
 from pathlib import Path
-from typing import Dict, List, Optional, Set
+from typing import Dict, List, Optional, Set, Tuple
 
 from housekeeper.store.models import File, Version
 
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.apps.lims import LimsAPI
 from cg.apps.madeline.api import MadelineAPI
 from cg.apps.scout.scoutapi import ScoutAPI
-from cg.constants import Pipeline
-from cg.constants.constants import FileFormat
+from cg.constants import Pipeline, HK_MULTIQC_HTML_TAG
+from cg.constants.constants import FileFormat, PrepCategory
+from cg.constants.scout_upload import ScoutCustomCaseReportTags
 from cg.constants.sequencing import SequencingMethod
 from cg.exc import CgDataError, HousekeeperBundleVersionMissingError
 from cg.io.controller import WriteFile
 from cg.meta.upload.scout.balsamic_config_builder import BalsamicConfigBuilder
 from cg.meta.upload.scout.balsamic_umi_config_builder import BalsamicUmiConfigBuilder
 from cg.meta.upload.scout.mip_config_builder import MipConfigBuilder
 from cg.meta.upload.scout.rnafusion_config_builder import RnafusionConfigBuilder
@@ -37,15 +38,15 @@
         scout_api: ScoutAPI,
         lims_api: LimsAPI,
         analysis_api: AnalysisAPI,
         madeline_api: MadelineAPI,
         status_db: Store,
     ):
         self.housekeeper = hk_api
-        self.scout = scout_api
+        self.scout_api = scout_api
         self.madeline_api = madeline_api
         self.mip_analysis_api = analysis_api
         self.lims = lims_api
         self.status_db = status_db
 
     def generate_config(self, analysis_obj: Analysis) -> ScoutLoadConfig:
         """Fetch data about an analysis to load Scout."""
@@ -101,149 +102,148 @@
         )
         self.housekeeper.include_file(file_obj=file_obj, version_obj=version)
         self.housekeeper.add_commit(file_obj)
 
         LOG.info(f"Added Scout load config to Housekeeper: {config_file_path}")
         return file_obj
 
-    def get_fusion_report(self, case_id: str, research: bool) -> Optional[File]:
-        """Get a fusion report for case in housekeeper
+    def get_multiqc_html_report(
+        self, case_id: str, pipeline: Pipeline
+    ) -> Tuple[ScoutCustomCaseReportTags, Optional[File]]:
+        """Return a multiqc report for a case in Housekeeper."""
+        if pipeline == Pipeline.MIP_RNA:
+            return (
+                ScoutCustomCaseReportTags.MULTIQC_RNA,
+                self.housekeeper.files(bundle=case_id, tags=HK_MULTIQC_HTML_TAG).first(),
+            )
+        return (
+            ScoutCustomCaseReportTags.MULTIQC,
+            self.housekeeper.files(bundle=case_id, tags=HK_MULTIQC_HTML_TAG).first(),
+        )
 
-        Args:
-            case_id     (string):       Case identifier
-            research    (bool):         Research report
-        Returns:
-            File in housekeeper (Optional[File])
-        """
+    def get_fusion_report(self, case_id: str, research: bool) -> Optional[File]:
+        """Return a fusion report for case in housekeeper."""
 
-        # This command can be executed as:
-        # ´housekeeper get file -V --tag fusion --tag pdf --tag clinical/research <case_id>´
         tags = {"fusion"}
         if research:
             tags.add("research")
         else:
             tags.add("clinical")
 
-        fusion_report: Optional[File] = self.housekeeper.get_file_from_latest_version(
-            bundle_name=case_id, tags=tags
-        )
-
-        return fusion_report
+        return self.housekeeper.get_file_from_latest_version(bundle_name=case_id, tags=tags)
 
     def get_splice_junctions_bed(self, case_id: str, sample_id: str) -> Optional[File]:
-        """Get a splice junctions bed file for case in housekeeper
-
-        Args:
-            case_id     (string):       Case identifier
-            sample_id   (string):       Sample identifier
-        Returns:
-            File in housekeeper (Optional[File])
-        """
+        """Return a splice junctions bed file for case in housekeeper."""
 
-        # This command can be executed as:
-        # ´housekeeper get file -V --tag junction --tag bed <sample_id>´
-        tags: {str} = {"junction", "bed", sample_id}
+        tags: Set[str] = {"junction", "bed", sample_id}
         splice_junctions_bed: Optional[File]
         try:
             splice_junctions_bed = self.housekeeper.get_file_from_latest_version(
                 bundle_name=case_id, tags=tags
             )
         except HousekeeperBundleVersionMissingError:
             LOG.debug("Could not find bundle for case %s", case_id)
 
         return splice_junctions_bed
 
     def get_rna_coverage_bigwig(self, case_id: str, sample_id: str) -> Optional[File]:
-        """Get a rna coverage bigwig file for case in housekeeper
+        """Return a RNA coverage bigwig file for case in housekeeper."""
 
-        Args:
-            case_id     (string):       Case identifier
-            sample_id   (string):       Sample identifier
-        Returns:
-            File in housekeeper (Optional[File])
-        """
+        tags: Set[str] = {"coverage", "bigwig", sample_id}
 
-        # This command can be executed as:
-        # ´housekeeper get file -V --tag coverage --tag bigwig <sample_id>´
-        tags: {str} = {"coverage", "bigwig", sample_id}
+        return self.housekeeper.get_file_from_latest_version(bundle_name=case_id, tags=tags)
 
-        rna_coverage_bigwig: Optional[File] = self.housekeeper.get_file_from_latest_version(
-            bundle_name=case_id, tags=tags
-        )
+    def get_unique_dna_cases_related_to_rna_case(self, case_id: str) -> Set[str]:
+        """Return a set of unique dna cases related to a RNA case"""
+        case: Family = self.status_db.get_case_by_internal_id(internal_id=case_id)
+        rna_dna_sample_case_map: Dict[
+            str, Dict[str, List[str]]
+        ] = self.create_rna_dna_sample_case_map(rna_case=case)
+        dna_sample_case_dict: Dict[str, List[str]]
+        unique_dna_cases_related_to_rna_case: Set[str] = set()
+        for dna_sample_case_dict in rna_dna_sample_case_map.values():
+            case_list: List[str]
+            for case_list in dna_sample_case_dict.values():
+                unique_dna_cases_related_to_rna_case.update(case_list)
 
-        return rna_coverage_bigwig
+        return unique_dna_cases_related_to_rna_case
 
     def upload_fusion_report_to_scout(
-        self, dry_run: bool, case_id: str, research: bool = False, update: bool = False
+        self, dry_run: bool, case_id: str, research: bool = False
     ) -> None:
-        """Upload fusion report file for a case to Scout.
-        This can also be run as
-        `housekeeper get file -V --tag fusion --tag pdf --tag clinical/research <case_id>`
-        `scout load gene-fusion-report [-r] <case_id> <path/to/research_gene_fusion_report.pdf>`
-
-        Args:
-            dry_run     (bool):         Skip uploading
-            case_id     (string):       Case identifier
-            research    (bool):         Upload research report instead of clinical
-            update      (bool):         Overwrite existing report
-        Returns:
-            Nothing
-        """
+        """Upload fusion report file for a case to Scout."""
 
-        scout_api: ScoutAPI = self.scout
-        status_db: Store = self.status_db
         report_type: str = "Research" if research else "Clinical"
-        rna_case: Family = status_db.get_case_by_internal_id(internal_id=case_id)
 
-        rna_dna_sample_case_map: Dict[str, Dict[str, list]] = self.create_rna_dna_sample_case_map(
-            rna_case=rna_case
-        )
-        unique_dna_cases: Set[str] = set()
         fusion_report: Optional[File] = self.get_fusion_report(case_id, research)
         if fusion_report is None:
             raise FileNotFoundError(
                 f"{report_type} fusion report was not found in housekeeper for {case_id}"
             )
 
         LOG.info(f"{report_type} fusion report {fusion_report.path} found")
-        for rna_sample_id in rna_dna_sample_case_map:
-            dna_cases: List[str]
-            dna_sample_id, dna_cases = rna_dna_sample_case_map[rna_sample_id].popitem()
-            unique_dna_cases.update(dna_cases)
 
-        for dna_case_id in unique_dna_cases:
+        for dna_case_id in self.get_unique_dna_cases_related_to_rna_case(case_id=case_id):
             LOG.info(f"Uploading {report_type} fusion report to scout for case {dna_case_id}")
 
             if dry_run:
                 continue
-            scout_api.upload_fusion_report(
+            self.scout_api.upload_fusion_report(
                 case_id=dna_case_id,
                 report_path=fusion_report.full_path,
                 research=research,
-                update=update,
             )
-            LOG.info("Uploaded %s fusion report", report_type)
+            LOG.info(
+                f"Uploaded {report_type} fusion report",
+            )
+
+        LOG.info(f"Upload {report_type} fusion report finished!")
+
+    def upload_rna_report_to_dna_case_in_scout(
+        self,
+        dry_run: bool,
+        report_type: str,
+        report_file: File,
+        rna_case_id: str,
+    ) -> None:
+        """Upload report file to DNA cases related to a RNA case in scout."""
+        LOG.info(f"Finding DNA cases related to RNA case {rna_case_id}")
+        for dna_case_id in self.get_unique_dna_cases_related_to_rna_case(rna_case_id):
+            self.upload_report_to_scout(
+                dry_run=dry_run,
+                report_type=report_type,
+                report_file=report_file,
+                case_id=dna_case_id,
+            )
 
-        LOG.info("Upload %s fusion report finished!", report_type)
+    def upload_report_to_scout(
+        self,
+        dry_run: bool,
+        case_id: str,
+        report_type: str,
+        report_file: File,
+    ) -> None:
+        """Upload report file a case to Scout."""
+
+        LOG.info(f"Uploading {report_type} report to scout for case {case_id}")
+
+        if dry_run:
+            LOG.info(f"Would have uploaded {report_type} report")
+            return
+        self.scout_api.upload_report(
+            case_id=case_id,
+            report_path=report_file.full_path,
+            report_type=report_type,
+        )
+        LOG.info(f"Uploaded {report_type} report")
+        LOG.info(f"Upload {report_type} report finished!")
 
     def upload_rna_coverage_bigwig_to_scout(self, case_id: str, dry_run: bool) -> None:
-        """Upload rna_coverage_bigwig file for a case to Scout.
-            This command can be executed as:
-            `housekeeper get file -V --tag coverage --tag bigwig <sample_id>;`
-            `scout update individual -c <case_id> -n <customer_sample_id> rna_coverage_bigwig
-            <path/to/coverage_file.bigWig>;`
-
-        Args:
-            dry_run     (bool):         Skip uploading
-            case_id     (string):       Case identifier
-        Returns:
-            Nothing
-        """
+        """Upload rna_coverage_bigwig file for a case to Scout."""
 
-        scout_api: ScoutAPI = self.scout
         status_db: Store = self.status_db
         rna_case = status_db.get_case_by_internal_id(internal_id=case_id)
         rna_dna_sample_case_map: Dict[str, Dict[str, list]] = self.create_rna_dna_sample_case_map(
             rna_case=rna_case
         )
         for rna_sample_id in rna_dna_sample_case_map:
             rna_coverage_bigwig: Optional[File] = self.get_rna_coverage_bigwig(
@@ -263,38 +263,28 @@
                 LOG.info(
                     f"Uploading RNA coverage bigwig file for {dna_sample_id} in case {dna_case_id} in scout"
                 )
 
                 if dry_run:
                     continue
 
-                scout_api.upload_rna_coverage_bigwig(
+                self.scout_api.upload_rna_coverage_bigwig(
                     file_path=rna_coverage_bigwig.full_path,
                     case_id=dna_case_id,
                     customer_sample_id=dna_sample_id,
                 )
                 LOG.info(
                     f"Uploaded RNA coverage bigwig file for {dna_sample_id} in case {dna_case_id}"
                 )
 
         LOG.info("Upload RNA coverage bigwig file finished!")
 
     def upload_splice_junctions_bed_to_scout(self, dry_run: bool, case_id: str) -> None:
-        """Upload splice_junctions_bed file for a case to Scout.
-            This command can be executed as:
-            `housekeeper get file -V --tag junction --tag bed <sample_id>;`
-            `scout update individual -c <case_id> -n <customer_sample_id> splice_junctions_bed <path/to/junction_file.bed>;`
-
-        Args:
-            dry_run     (bool):         Skip uploading
-            case_id     (string):       Case identifier
-        Returns:
-            Nothing
-        """
-        scout_api: ScoutAPI = self.scout
+        """Upload splice_junctions_bed file for a case to Scout."""
+
         status_db: Store = self.status_db
         rna_case: Family = status_db.get_case_by_internal_id(internal_id=case_id)
 
         rna_dna_sample_case_map: Dict[str, Dict[str, list]] = self.create_rna_dna_sample_case_map(
             rna_case=rna_case
         )
         for rna_sample_id in rna_dna_sample_case_map:
@@ -315,47 +305,33 @@
                 LOG.info(
                     f"Uploading splice junctions bed file for sample {dna_sample_id} in case {dna_case_id} in scout"
                 )
 
                 if dry_run:
                     continue
 
-                scout_api.upload_splice_junctions_bed(
+                self.scout_api.upload_splice_junctions_bed(
                     file_path=splice_junctions_bed.full_path,
                     case_id=dna_case_id,
                     customer_sample_id=dna_sample_id,
                 )
                 LOG.info(
                     f"Uploaded splice junctions bed file {dna_sample_id} in case {dna_case_id}"
                 )
 
         LOG.info("Upload splice junctions bed file finished!")
 
     def upload_rna_junctions_to_scout(self, dry_run: bool, case_id: str) -> None:
-        """Upload RNA junctions splice files to Scout.
-
-        Args:
-            dry_run     (bool):         Skip uploading
-            case_id     (string):       RNA case identifier
-        Returns:
-            Nothing
-        """
+        """Upload RNA junctions splice files to Scout."""
         self.upload_splice_junctions_bed_to_scout(dry_run=dry_run, case_id=case_id)
         self.upload_rna_coverage_bigwig_to_scout(case_id=case_id, dry_run=dry_run)
 
     @staticmethod
     def _get_sample(case: Family, subject_id: str) -> Optional[Sample]:
-        """Get sample of a case for a subject_id.
-
-        Args:
-            case     (Family):               Case
-            subject_id   (str):                     Subject id to search for
-        Returns:
-            matching sample (Sample)
-        """
+        """Return sample of a case for a subject_id."""
 
         link: FamilySample
         for link in case.links:
             sample: Sample = link.sample
             if sample.subject_id == subject_id:
                 return sample
 
@@ -384,50 +360,45 @@
             Pipeline.RNAFUSION: RnafusionConfigBuilder(
                 hk_version_obj=hk_version, analysis_obj=analysis, lims_api=self.lims
             ),
         }
 
         return config_builders[analysis.pipeline]
 
-    def create_rna_dna_sample_case_map(self, rna_case: Family) -> Dict[str, Dict[str, list]]:
+    def create_rna_dna_sample_case_map(self, rna_case: Family) -> Dict[str, Dict[str, List[str]]]:
         """Returns a nested dictionary for mapping an RNA sample to a DNA sample and its DNA cases based on
         subject_id. Example dictionary {rna_sample_id : {dna_sample_id : [dna_case1_id, dna_case2_id]}}.
-
-        Args:
-            rna_case                (Family):  RNA case identifier
-        Case Returns:
-            rna_dna_sample_case_map     (Dict):       rna-dna relationships, and related dna cases based on subject id
         """
-        rna_dna_sample_case_map: Dict[str, Dict[str, list]] = {}
-        for rna_case.link in rna_case.links:
-            self._add_rna_sample(
-                rna_sample=rna_case.link.sample, rna_dna_sample_case_map=rna_dna_sample_case_map
+        rna_dna_sample_case_map: Dict[str, Dict[str, List[str]]] = {}
+        for link in rna_case.links:
+            self.build_rna_sample_map(
+                rna_sample=link.sample, rna_dna_sample_case_map=rna_dna_sample_case_map
             )
         return rna_dna_sample_case_map
 
-    def _add_rna_sample(
-        self, rna_sample: Sample, rna_dna_sample_case_map: Dict[str, Dict[str, list]]
-    ) -> Dict[str, Dict[str, list]]:
-        """Adds an RNA sample and its matching DNA sample, and cases."""
-        dna_sample: Sample = self._link_rna_sample_to_dna_sample(
+    def build_rna_sample_map(
+        self, rna_sample: Sample, rna_dna_sample_case_map: Dict[str, Dict[str, List[str]]]
+    ) -> None:
+        """Create a dictionary of all DNA samples, and their related cases, related to a RNA sample."""
+        dna_sample: Sample = self._map_dna_samples_related_to_rna_sample(
             rna_sample=rna_sample, rna_dna_sample_case_map=rna_dna_sample_case_map
         )
-        self._add_dna_cases_to_dna_sample(
+        self._map_dna_cases_to_dna_sample(
             dna_sample=dna_sample,
             rna_dna_sample_case_map=rna_dna_sample_case_map,
             rna_sample=rna_sample,
         )
-        return rna_dna_sample_case_map
 
-    def _link_rna_sample_to_dna_sample(
-        self, rna_sample: Sample, rna_dna_sample_case_map: Dict[str, Dict[str, list]]
+    def _map_dna_samples_related_to_rna_sample(
+        self, rna_sample: Sample, rna_dna_sample_case_map: Dict[str, Dict[str, List[str]]]
     ) -> Sample:
+        """Maps an RNA sample to a DNA sample based on subject id."""
         if not rna_sample.subject_id:
             raise CgDataError(
-                f"Failed on RNA sample {rna_sample.internal_id} as subject_id field is empty"
+                f"Failed to link RNA sample {rna_sample.internal_id} to dna samples - subject_id field is empty"
             )
 
         collaborator_ids = [customer.id for customer in rna_sample.customer.collaborators]
 
         subject_id_samples: List[
             Sample
         ] = self.status_db.get_samples_by_customer_id_list_and_subject_id_and_is_tumour(
@@ -443,42 +414,48 @@
         if len(subject_id_dna_samples) != 1:
             raise CgDataError(
                 f"Failed to upload files for RNA case: unexpected number of DNA sample matches for subject_id: {rna_sample.subject_id}. Number of matches: {len(subject_id_dna_samples)} "
             )
         rna_dna_sample_case_map[rna_sample.internal_id]: Dict[str, list] = {}
         sample: Sample
         for sample in subject_id_dna_samples:
-            rna_dna_sample_case_map[rna_sample.internal_id][sample.name]: list = []
-            return sample
+            if sample.internal_id != rna_sample.internal_id:
+                rna_dna_sample_case_map[rna_sample.internal_id][sample.name]: List[str] = []
+                return sample
 
     @staticmethod
-    def _add_dna_cases_to_dna_sample(
+    def _map_dna_cases_to_dna_sample(
         dna_sample: Sample,
         rna_dna_sample_case_map: Dict[str, Dict[str, list]],
         rna_sample: Sample,
     ) -> None:
-        for dna_sample.link in dna_sample.links:
-            case_object: Family = dna_sample.link.family
-            if any(
-                [
-                    case_object.data_analysis
-                    in [Pipeline.MIP_DNA, Pipeline.BALSAMIC, Pipeline.BALSAMIC_UMI]
-                    and case_object.customer.id
-                    in [customer.id for customer in rna_sample.customer.collaborators]
-                ]
-            ):
+        """Maps a list of DNA cases linked to DNA sample."""
+        cases_related_to_dna_sample: List[Family] = [
+            dna_sample_family_relation.family for dna_sample_family_relation in dna_sample.links
+        ]
+        for case in cases_related_to_dna_sample:
+            if case.data_analysis in [
+                Pipeline.MIP_DNA,
+                Pipeline.BALSAMIC,
+                Pipeline.BALSAMIC_UMI,
+            ] and case.customer in [customer for customer in rna_sample.customer.collaborators]:
                 rna_dna_sample_case_map[rna_sample.internal_id][dna_sample.name].append(
-                    case_object.internal_id
+                    case.internal_id
                 )
 
     @staticmethod
-    def _get_application_prep_category(subject_id_samples: List[Sample]) -> List[Sample]:
-        """Filter a Sample list, returning DNA samples selected on their prep_category."""
-        subject_id_dna_samples: List[Sample] = []
-        for sample in subject_id_samples:
-            if sample.application_version.application.prep_category in [
-                SequencingMethod.WGS,
-                SequencingMethod.TGS,
-                SequencingMethod.WES,
-            ]:
-                subject_id_dna_samples.append(sample)
+    def _get_application_prep_category(
+        subject_id_samples: List[Sample],
+    ) -> List[Optional[Sample]]:
+        """Filter a models Sample list, returning DNA samples selected on their preparation category."""
+        subject_id_dna_samples: List[Optional[Sample]] = [
+            sample
+            for sample in subject_id_samples
+            if sample.prep_category
+            in [
+                PrepCategory.WHOLE_GENOME_SEQUENCING.value,
+                PrepCategory.TARGETED_GENOME_SEQUENCING.value,
+                PrepCategory.WHOLE_EXOME_SEQUENCING.value,
+            ]
+        ]
+
         return subject_id_dna_samples
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cg-29.5.7/cg/meta/upload/upload_api.py` & `cg-29.6.0/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/upload/vogue.py` & `cg-29.6.0/cg/meta/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/analysis.py` & `cg-29.6.0/cg/meta/workflow/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
     @staticmethod
     def get_application_type(sample_obj: Sample) -> str:
         """
         Gets application type for sample. Only application types supported by trailblazer (or other)
         are valid outputs.
         """
-        prep_category: str = sample_obj.application_version.application.prep_category
+        prep_category: str = sample_obj.prep_category
         if prep_category and prep_category.lower() in {
             AnalysisType.TARGETED_GENOME_SEQUENCING,
             AnalysisType.WHOLE_EXOME_SEQUENCING,
             AnalysisType.WHOLE_GENOME_SEQUENCING,
             AnalysisType.WHOLE_TRANSCRIPTOME_SEQUENCING,
         }:
             return prep_category.lower()
```

### Comparing `cg-29.5.7/cg/meta/workflow/balsamic.py` & `cg-29.6.0/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/balsamic_pon.py` & `cg-29.6.0/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/balsamic_qc.py` & `cg-29.6.0/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/balsamic_umi.py` & `cg-29.6.0/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/fastq.py` & `cg-29.6.0/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/fluffy.py` & `cg-29.6.0/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/microsalt.py` & `cg-29.6.0/cg/meta/workflow/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/mip.py` & `cg-29.6.0/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/mip_dna.py` & `cg-29.6.0/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/mip_rna.py` & `cg-29.6.0/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/mutant.py` & `cg-29.6.0/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/nextflow_common.py` & `cg-29.6.0/cg/meta/workflow/nextflow_common.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/prepare_fastq.py` & `cg-29.6.0/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/rnafusion.py` & `cg-29.6.0/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/taxprofiler.py` & `cg-29.6.0/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/meta/workflow/tower_common.py` & `cg-29.6.0/cg/meta/workflow/tower_common.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/balsamic/config.py` & `cg-29.6.0/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/balsamic/metrics.py` & `cg-29.6.0/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/cg_config.py` & `cg-29.6.0/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/cgstats/stats_sample.py` & `cg-29.6.0/cg/models/cgstats/stats_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/compression_data.py` & `cg-29.6.0/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/deliverables/metric_deliverables.py` & `cg-29.6.0/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/demultiplex/demux_results.py` & `cg-29.6.0/cg/models/demultiplex/demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/demultiplex/flow_cell.py` & `cg-29.6.0/cg/models/demultiplex/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/demultiplex/run_parameters.py` & `cg-29.6.0/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/demultiplex/sbatch.py` & `cg-29.6.0/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/file_data.py` & `cg-29.6.0/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/invoice/invoice.py` & `cg-29.6.0/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/lims/sample.py` & `cg-29.6.0/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/mip/mip_config.py` & `cg-29.6.0/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/mip/mip_metrics_deliverables.py` & `cg-29.6.0/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/mip/mip_sample_info.py` & `cg-29.6.0/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/nextflow/deliverables.py` & `cg-29.6.0/cg/models/nextflow/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/nextflow/sample.py` & `cg-29.6.0/cg/models/nextflow/sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/observations/input_files.py` & `cg-29.6.0/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/orders/constants.py` & `cg-29.6.0/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/orders/excel_sample.py` & `cg-29.6.0/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/orders/json_sample.py` & `cg-29.6.0/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/orders/order.py` & `cg-29.6.0/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/orders/orderform_schema.py` & `cg-29.6.0/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/orders/sample_base.py` & `cg-29.6.0/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/orders/samples.py` & `cg-29.6.0/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/report/metadata.py` & `cg-29.6.0/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/report/report.py` & `cg-29.6.0/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/report/sample.py` & `cg-29.6.0/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/report/validators.py` & `cg-29.6.0/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/rnafusion/rnafusion_sample.py` & `cg-29.6.0/cg/models/rnafusion/rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/scout/scout_load_config.py` & `cg-29.6.0/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/slurm/sbatch.py` & `cg-29.6.0/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/models/workflow/mutant.py` & `cg-29.6.0/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/resources/20181012_Indices.csv` & `cg-29.6.0/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/resources/rnafusion_bundle_filenames.csv` & `cg-29.6.0/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/server/admin.py` & `cg-29.6.0/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/server/api.py` & `cg-29.6.0/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/server/app.py` & `cg-29.6.0/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/server/config.py` & `cg-29.6.0/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/server/ext.py` & `cg-29.6.0/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/server/invoices/templates/invoices/index.html` & `cg-29.6.0/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/server/invoices/templates/invoices/invoice.html` & `cg-29.6.0/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/server/invoices/templates/invoices/layout.html` & `cg-29.6.0/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/server/invoices/templates/invoices/new.html` & `cg-29.6.0/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/server/invoices/views.py` & `cg-29.6.0/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/api/add.py` & `cg-29.6.0/cg/store/api/add.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/api/base.py` & `cg-29.6.0/cg/store/api/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/api/core.py` & `cg-29.6.0/cg/store/api/core.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/api/delete.py` & `cg-29.6.0/cg/store/api/delete.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/api/find_basic_data.py` & `cg-29.6.0/cg/store/api/find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/api/find_business_data.py` & `cg-29.6.0/cg/store/api/find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/api/status.py` & `cg-29.6.0/cg/store/api/status.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_analysis_filters.py` & `cg-29.6.0/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_application_filters.py` & `cg-29.6.0/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_application_version_filters.py` & `cg-29.6.0/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_bed_filters.py` & `cg-29.6.0/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_bed_version_filters.py` & `cg-29.6.0/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_case_filters.py` & `cg-29.6.0/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_case_sample_filters.py` & `cg-29.6.0/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_collaboration_filters.py` & `cg-29.6.0/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_customer_filters.py` & `cg-29.6.0/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_flow_cell_filters.py` & `cg-29.6.0/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_invoice_filters.py` & `cg-29.6.0/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_organism_filters.py` & `cg-29.6.0/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_panel_filters.py` & `cg-29.6.0/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_pool_filters.py` & `cg-29.6.0/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_sample_filters.py` & `cg-29.6.0/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/filters/status_user_filters.py` & `cg-29.6.0/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/store/models.py` & `cg-29.6.0/cg/store/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -678,14 +678,19 @@
         return self._phenotype_terms.split(",") if self._phenotype_terms else []
 
     @phenotype_terms.setter
     def phenotype_terms(self, phenotype_term_list: List[str]):
         self._phenotype_terms = ",".join(phenotype_term_list) if phenotype_term_list else None
 
     @property
+    def prep_category(self) -> str:
+        """Return the preparation category of the sample."""
+        return self.application_version.application.prep_category
+
+    @property
     def state(self) -> str:
         """Get the current sample state."""
         if self.delivered_at:
             return f"Delivered {self.delivered_at.date()}"
         if self.sequenced_at:
             return f"Sequenced {self.sequenced_at.date()}"
         if self.sequence_start:
```

### Comparing `cg-29.5.7/cg/utils/checksum/checksum.py` & `cg-29.6.0/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/utils/click/EnumChoice.py` & `cg-29.6.0/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/utils/commands.py` & `cg-29.6.0/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/utils/date.py` & `cg-29.6.0/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/utils/dict.py` & `cg-29.6.0/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/utils/dispatcher.py` & `cg-29.6.0/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/utils/email.py` & `cg-29.6.0/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/utils/flask/enum.py` & `cg-29.6.0/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg/utils/utils.py` & `cg-29.6.0/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/cg.egg-info/PKG-INFO` & `cg-29.6.0/cg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 29.5.7
+Version: 29.6.0
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-29.5.7/cg.egg-info/SOURCES.txt` & `cg-29.6.0/cg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/requirements.txt` & `cg-29.6.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/setup.py` & `cg-29.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="29.5.7",
+    version="29.6.0",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     include_package_data=True,
```

### Comparing `cg-29.5.7/tests/apps/cgstats/conftest.py` & `cg-29.6.0/tests/apps/cgstats/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/cgstats/crud/test_create_novaseq.py` & `cg-29.6.0/tests/apps/cgstats/crud/test_create_novaseq.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/cgstats/crud/test_delete.py` & `cg-29.6.0/tests/apps/cgstats/crud/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/cgstats/parsers/test_conversion_stats.py` & `cg-29.6.0/tests/apps/cgstats/parsers/test_conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/cgstats/parsers/test_demux_stats.py` & `cg-29.6.0/tests/apps/cgstats/parsers/test_demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/cgstats/parsers/test_run_info.py` & `cg-29.6.0/tests/apps/cgstats/parsers/test_run_info.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/cgstats/test_cgstats_create.py` & `cg-29.6.0/tests/apps/cgstats/test_cgstats_create.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/cgstats/test_stats.py` & `cg-29.6.0/tests/apps/cgstats/test_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/conftest.py` & `cg-29.6.0/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/coverage/test_coverage.py` & `cg-29.6.0/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/crunchy/conftest.py` & `cg-29.6.0/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/crunchy/test_compress_fastq.py` & `cg-29.6.0/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/crunchy/test_config.py` & `cg-29.6.0/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/crunchy/test_crunchy.py` & `cg-29.6.0/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/crunchy/test_spring_decompression.py` & `cg-29.6.0/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/demultiplex/conftest.py` & `cg-29.6.0/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/demultiplex/test_convert_to_sample_sheet.py` & `cg-29.6.0/tests/apps/demultiplex/test_convert_to_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-29.6.0/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/demultiplex/test_sample_sheet.py` & `cg-29.6.0/tests/apps/demultiplex/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/demultiplex/test_validate_sample_sheet.py` & `cg-29.6.0/tests/apps/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/gens/test_gens_api.py` & `cg-29.6.0/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/gt/conftest.py` & `cg-29.6.0/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/gt/test_gt_api.py` & `cg-29.6.0/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/hk/conftest.py` & `cg-29.6.0/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/hk/test__getattr__.py` & `cg-29.6.0/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/hk/test_add_file.py` & `cg-29.6.0/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/hk/test_bundles.py` & `cg-29.6.0/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/hk/test_core.py` & `cg-29.6.0/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/hk/test_file.py` & `cg-29.6.0/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/hk/test_version.py` & `cg-29.6.0/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/lims/conftest.py` & `cg-29.6.0/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/lims/test_api.py` & `cg-29.6.0/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/loqus/conftest.py` & `cg-29.6.0/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/loqus/test_loqusdb_api.py` & `cg-29.6.0/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/madeline/conftest.py` & `cg-29.6.0/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/madeline/test_madeline.py` & `cg-29.6.0/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/mip/conftest.py` & `cg-29.6.0/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/mip/test_config_mip.py` & `cg-29.6.0/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/mutacc_auto/conftest.py` & `cg-29.6.0/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-29.6.0/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/orderform/conftest.py` & `cg-29.6.0/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-29.6.0/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/orderform/test_excel_sample_schema.py` & `cg-29.6.0/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/orderform/test_json_orderform_parser.py` & `cg-29.6.0/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/orderform/test_orderform_parser.py` & `cg-29.6.0/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/scout/conftest.py` & `cg-29.6.0/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/scout/test_get_causative_variants.py` & `cg-29.6.0/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/scout/test_get_scout_cases.py` & `cg-29.6.0/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/scout/test_scout_load_config.py` & `cg-29.6.0/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/scout/test_scout_models.py` & `cg-29.6.0/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/slurm/conftest.py` & `cg-29.6.0/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/slurm/test_slurm_api.py` & `cg-29.6.0/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/test_apps_environ.py` & `cg-29.6.0/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/test_osticket.py` & `cg-29.6.0/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/vogue/conftest.py` & `cg-29.6.0/tests/apps/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/apps/vogue/test_vogue_api.py` & `cg-29.6.0/tests/apps/vogue/test_vogue_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/add/test_cli_add.py` & `cg-29.6.0/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/add/test_cli_add_customer.py` & `cg-29.6.0/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/add/test_cli_add_family.py` & `cg-29.6.0/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/add/test_cli_add_relationship.py` & `cg-29.6.0/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/add/test_cli_add_sample.py` & `cg-29.6.0/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/backup/conftest.py` & `cg-29.6.0/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/backup/test_backup_command.py` & `cg-29.6.0/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/clean/conftest.py` & `cg-29.6.0/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/clean/test_balsamic_clean.py` & `cg-29.6.0/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-29.6.0/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/clean/test_hk_bundle_files.py` & `cg-29.6.0/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-29.6.0/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/clean/test_microbial_clean.py` & `cg-29.6.0/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-29.6.0/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/compress/conftest.py` & `cg-29.6.0/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/compress/test_cli_compress_fastq.py` & `cg-29.6.0/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/compress/test_cli_decompress_spring.py` & `cg-29.6.0/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/compress/test_compress_helpers.py` & `cg-29.6.0/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/compress/test_store_fastq.py` & `cg-29.6.0/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/conftest.py` & `cg-29.6.0/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/delete/test_cli_delete_case.py` & `cg-29.6.0/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/delete/test_cli_delete_cases.py` & `cg-29.6.0/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/deliver/conftest.py` & `cg-29.6.0/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/deliver/test_deliver_base.py` & `cg-29.6.0/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/deliver/test_rsync_base.py` & `cg-29.6.0/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-29.6.0/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/demultiplex/conftest.py` & `cg-29.6.0/tests/cli/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/demultiplex/test_add_flowcell.py` & `cg-29.6.0/tests/cli/demultiplex/test_add_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-29.6.0/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-29.6.0/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/demultiplex/test_finish_demux.py` & `cg-29.6.0/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/demultiplex/test_stats_command.py` & `cg-29.6.0/tests/cli/demultiplex/test_stats_command.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-29.6.0/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/generate/report/conftest.py` & `cg-29.6.0/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-29.6.0/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/generate/report/test_utils.py` & `cg-29.6.0/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/generate/test_cli_base.py` & `cg-29.6.0/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/get/test_cli_get.py` & `cg-29.6.0/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/get/test_cli_get_analysis.py` & `cg-29.6.0/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/get/test_cli_get_case.py` & `cg-29.6.0/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/get/test_cli_get_flow_cell.py` & `cg-29.6.0/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/get/test_cli_get_sample.py` & `cg-29.6.0/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/set/conftest.py` & `cg-29.6.0/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/set/test_cli_set_case.py` & `cg-29.6.0/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/set/test_cli_set_cases.py` & `cg-29.6.0/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/set/test_cli_set_flowcell.py` & `cg-29.6.0/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/set/test_cli_set_list_keys.py` & `cg-29.6.0/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/set/test_cli_set_sample.py` & `cg-29.6.0/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/set/test_cli_set_samples.py` & `cg-29.6.0/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/store/test_fastq.py` & `cg-29.6.0/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/test_base.py` & `cg-29.6.0/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/test_clean.py` & `cg-29.6.0/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/test_cli_status_cases.py` & `cg-29.6.0/tests/cli/test_cli_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/conftest.py` & `cg-29.6.0/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/test_cli_scout.py` & `cg-29.6.0/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/test_cli_upload.py` & `cg-29.6.0/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/test_cli_upload_auto.py` & `cg-29.6.0/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-29.6.0/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/test_cli_upload_fastq.py` & `cg-29.6.0/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/test_cli_upload_genotype.py` & `cg-29.6.0/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/test_cli_upload_gens.py` & `cg-29.6.0/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/test_cli_upload_nipt.py` & `cg-29.6.0/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-29.6.0/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-29.6.0/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/test_cli_upload_observations.py` & `cg-29.6.0/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/upload/test_cli_upload_vogue.py` & `cg-29.6.0/tests/cli/upload/test_cli_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/balsamic/conftest.py` & `cg-29.6.0/tests/cli/workflow/balsamic/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from typing import List
 
 import pytest
 from cg.apps.hermes.hermes_api import HermesApi
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants import Pipeline
-from cg.constants.constants import FileFormat
+from cg.constants.constants import FileFormat, PrepCategory
 from cg.io.controller import WriteFile, WriteStream
 from cg.meta.workflow.balsamic import BalsamicAnalysisAPI
 from cg.models.cg_config import CGConfig
 from cg.store import Store
 from tests.mocks.limsmock import MockLimsAPI
 from tests.mocks.process_mock import ProcessMock
 from tests.mocks.tb_mock import MockTB
@@ -317,39 +317,47 @@
     cg_context.housekeeper_api_ = balsamic_housekeeper
     cg_context.lims_api_ = balsamic_lims
     cg_context.trailblazer_api_ = trailblazer_api
     cg_context.meta_apis["analysis_api"] = BalsamicAnalysisAPI(config=cg_context)
     status_db: Store = cg_context.status_db
 
     # Create tgs application version
-    helpers.ensure_application_version(store=status_db, application_tag="TGSA", prep_category="tgs")
+    helpers.ensure_application_version(
+        store=status_db,
+        application_tag="TGSA",
+        prep_category=PrepCategory.TARGETED_GENOME_SEQUENCING,
+    )
 
     # Create wes application version
-    helpers.ensure_application_version(store=status_db, application_tag="WESA", prep_category="wes")
+    helpers.ensure_application_version(
+        store=status_db,
+        application_tag="WESA",
+        prep_category=PrepCategory.WHOLE_EXOME_SEQUENCING,
+    )
 
     # Create textbook case for WGS PAIRED with enough reads
     case_wgs_paired_enough_reads = helpers.add_case(
         store=status_db,
         internal_id="balsamic_case_wgs_paired_enough_reads",
         name="balsamic_case_wgs_paired_enough_reads",
         data_analysis=Pipeline.BALSAMIC,
     )
     sample_case_wgs_paired_tumor_enough_reads = helpers.add_sample(
         status_db,
         internal_id="sample_case_wgs_paired_tumor_enough_reads",
         is_tumour=True,
-        application_type="wgs",
+        application_type=PrepCategory.WHOLE_GENOME_SEQUENCING,
         reads=10,
         sequenced_at=dt.datetime.now(),
     )
     sample_case_wgs_paired_normal_enough_reads = helpers.add_sample(
         status_db,
         internal_id="sample_case_wgs_paired_normal_enough_reads",
         is_tumour=False,
-        application_type="wgs",
+        application_type=PrepCategory.WHOLE_GENOME_SEQUENCING,
         reads=10,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(
         status_db,
         case=case_wgs_paired_enough_reads,
         sample=sample_case_wgs_paired_tumor_enough_reads,
@@ -367,23 +375,23 @@
         name="balsamic_case_wgs_paired",
         data_analysis=Pipeline.BALSAMIC,
     )
     sample_case_wgs_paired_tumor = helpers.add_sample(
         status_db,
         internal_id="sample_case_wgs_paired_tumor",
         is_tumour=True,
-        application_type="wgs",
+        application_type=PrepCategory.WHOLE_GENOME_SEQUENCING,
         reads=10,
         sequenced_at=dt.datetime.now(),
     )
     sample_case_wgs_paired_normal = helpers.add_sample(
         status_db,
         internal_id="sample_case_wgs_paired_normal",
         is_tumour=False,
-        application_type="wgs",
+        application_type=PrepCategory.WHOLE_GENOME_SEQUENCING,
         reads=10,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(status_db, case=case_wgs_paired, sample=sample_case_wgs_paired_tumor)
     helpers.add_relationship(status_db, case=case_wgs_paired, sample=sample_case_wgs_paired_normal)
 
     # Create textbook case for TGS PAIRED without enough reads
@@ -394,24 +402,24 @@
         data_analysis=Pipeline.BALSAMIC,
     )
     sample_case_tgs_paired_tumor = helpers.add_sample(
         status_db,
         internal_id="sample_case_tgs_paired_tumor",
         is_tumour=True,
         application_tag="TGSA",
-        application_type="tgs",
+        application_type=PrepCategory.TARGETED_GENOME_SEQUENCING,
         reads=10,
         sequenced_at=dt.datetime.now(),
     )
     sample_case_tgs_paired_normal = helpers.add_sample(
         status_db,
         internal_id="sample_case_tgs_paired_normal",
         is_tumour=False,
         application_tag="TGSA",
-        application_type="tgs",
+        application_type=PrepCategory.TARGETED_GENOME_SEQUENCING,
         reads=0,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(status_db, case=case_tgs_paired, sample=sample_case_tgs_paired_tumor)
     helpers.add_relationship(status_db, case=case_tgs_paired, sample=sample_case_tgs_paired_normal)
 
     # Create textbook case for WGS TUMOR ONLY
@@ -421,15 +429,15 @@
         name="balsamic_case_wgs_single",
         data_analysis=Pipeline.BALSAMIC,
     )
     sample_case_wgs_single_tumor = helpers.add_sample(
         status_db,
         internal_id="sample_case_wgs_single_tumor",
         is_tumour=True,
-        application_type="wgs",
+        application_type=PrepCategory.WHOLE_GENOME_SEQUENCING,
         reads=100,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(status_db, case=case_wgs_single, sample=sample_case_wgs_single_tumor)
 
     # Create textbook case for TGS TUMOR ONLY
     case_tgs_single = helpers.add_case(
@@ -439,15 +447,15 @@
         data_analysis=Pipeline.BALSAMIC,
     )
     sample_case_tgs_single_tumor = helpers.add_sample(
         status_db,
         internal_id="sample_case_tgs_single_tumor",
         is_tumour=True,
         application_tag="TGSA",
-        application_type="tgs",
+        application_type=PrepCategory.TARGETED_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(status_db, case=case_tgs_single, sample=sample_case_tgs_single_tumor)
 
     # Create ERROR case for TGS NORMAL ONLY
     case_tgs_single_error = helpers.add_case(
         status_db,
@@ -456,15 +464,15 @@
         data_analysis=Pipeline.BALSAMIC,
     )
     sample_case_tgs_single_normal_error = helpers.add_sample(
         status_db,
         internal_id="sample_case_tgs_single_normal_error",
         is_tumour=False,
         application_tag="TGSA",
-        application_type="tgs",
+        application_type=PrepCategory.TARGETED_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(
         status_db,
         case=case_tgs_single_error,
         sample=sample_case_tgs_single_normal_error,
     )
@@ -477,31 +485,31 @@
         data_analysis=Pipeline.BALSAMIC,
     )
     sample_case_tgs_paired_tumor_error = helpers.add_sample(
         status_db,
         internal_id="sample_case_tgs_paired_tumor_error",
         is_tumour=True,
         application_tag="TGSA",
-        application_type="tgs",
+        application_type=PrepCategory.TARGETED_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     sample_case_tgs_paired_tumor2_error = helpers.add_sample(
         status_db,
         internal_id="sample_case_tgs_paired_tumor2_error",
         is_tumour=True,
         application_tag="TGSA",
-        application_type="tgs",
+        application_type=PrepCategory.TARGETED_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     sample_case_tgs_paired_normal_error = helpers.add_sample(
         status_db,
         internal_id="sample_case_tgs_paired_normal_error",
         is_tumour=False,
         application_tag="TGSA",
-        application_type="tgs",
+        application_type=PrepCategory.TARGETED_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(
         status_db,
         case=case_tgs_paired_error,
         sample=sample_case_tgs_paired_tumor_error,
     )
@@ -523,23 +531,23 @@
         name="balsamic_case_mixed_paired_error",
         data_analysis=Pipeline.BALSAMIC,
     )
     mixed_sample_case_wgs_paired_tumor_error = helpers.add_sample(
         status_db,
         internal_id="mixed_sample_case_wgs_paired_tumor_error",
         is_tumour=True,
-        application_type="wgs",
+        application_type=PrepCategory.WHOLE_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     mixed_sample_case_tgs_paired_normal_error = helpers.add_sample(
         status_db,
         internal_id="mixed_sample_case_tgs_paired_normal_error",
         is_tumour=False,
         application_tag="TGSA",
-        application_type="tgs",
+        application_type=PrepCategory.TARGETED_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(
         status_db,
         case=case_mixed_paired_error,
         sample=mixed_sample_case_wgs_paired_tumor_error,
     )
@@ -556,15 +564,15 @@
         name="balsamic_case_mixed_wgs_mic_paired_error",
         data_analysis=Pipeline.BALSAMIC,
     )
     mixed_sample_case_wgs_mic_paired_tumor_error = helpers.add_sample(
         status_db,
         internal_id="mixed_sample_case_wgs_mic_paired_tumor_error",
         is_tumour=True,
-        application_type="wgs",
+        application_type=PrepCategory.WHOLE_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     mixed_sample_case_wgs_mic_paired_normal_error = helpers.add_sample(
         status_db,
         internal_id="mixed_sample_case_wgs_mic_paired_normal_error",
         is_tumour=False,
         application_tag="MICA",
@@ -590,23 +598,23 @@
         data_analysis=Pipeline.BALSAMIC,
     )
     mixed_sample_case_mixed_bed_paired_tumor_error = helpers.add_sample(
         status_db,
         internal_id="mixed_sample_case_mixed_bed_paired_tumor_error",
         is_tumour=True,
         application_tag="TGSA",
-        application_type="tgs",
+        application_type=PrepCategory.TARGETED_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     mixed_sample_case_mixed_bed_paired_normal_error = helpers.add_sample(
         status_db,
         internal_id="mixed_sample_case_mixed_bed_paired_normal_error",
         is_tumour=False,
         application_tag="TGSA",
-        application_type="tgs",
+        application_type=PrepCategory.TARGETED_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(
         status_db,
         case=case_mixed_bed_paired_error,
         sample=mixed_sample_case_mixed_bed_paired_tumor_error,
     )
@@ -623,15 +631,15 @@
         name="mip_case_wgs_single",
         data_analysis=Pipeline.MIP_DNA,
     )
     mip_sample_case_wgs_single_tumor = helpers.add_sample(
         status_db,
         internal_id="mip_sample_case_wgs_single_tumor",
         is_tumour=True,
-        application_type="wgs",
+        application_type=PrepCategory.WHOLE_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(
         status_db,
         case=mip_case_wgs_single,
         sample=mip_sample_case_wgs_single_tumor,
     )
@@ -644,31 +652,31 @@
         data_analysis=Pipeline.BALSAMIC,
     )
     sample_case_wgs_paired_two_normal_tumor_error = helpers.add_sample(
         status_db,
         internal_id="sample_case_wgs_paired_two_normal_tumor_error",
         is_tumour=True,
         application_tag="WGSA",
-        application_type="wgs",
+        application_type=PrepCategory.WHOLE_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     sample_case_wgs_paired_two_normal_normal1_error = helpers.add_sample(
         status_db,
         internal_id="sample_case_wgs_paired_two_normal_normal1_error",
         is_tumour=False,
         application_tag="WGSA",
-        application_type="wgs",
+        application_type=PrepCategory.WHOLE_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     sample_case_wgs_paired_two_normal_normal2_error = helpers.add_sample(
         status_db,
         internal_id="sample_case_wgs_paired_two_normal_normal2_error",
         is_tumour=False,
         application_tag="WGSA",
-        application_type="wgs",
+        application_type=PrepCategory.WHOLE_GENOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(
         status_db,
         case=case_wgs_paired_two_normal_error,
         sample=sample_case_wgs_paired_two_normal_tumor_error,
     )
@@ -691,15 +699,15 @@
         data_analysis=Pipeline.BALSAMIC,
     )
     sample_case_wes_tumor = helpers.add_sample(
         status_db,
         internal_id="sample_case_wes_tumor",
         is_tumour=True,
         application_tag="WESA",
-        application_type="wes",
+        application_type=PrepCategory.WHOLE_EXOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(status_db, case=case_wes_tumor, sample=sample_case_wes_tumor)
 
     # Create ERROR case for WES when no panel is found
     case_wes_panel_error = helpers.add_case(
         status_db,
@@ -708,15 +716,15 @@
         data_analysis=Pipeline.BALSAMIC,
     )
     sample_case_wes_panel_error = helpers.add_sample(
         status_db,
         internal_id="sample_case_wes_panel_error",
         is_tumour=True,
         application_tag="WESA",
-        application_type="wes",
+        application_type=PrepCategory.WHOLE_EXOME_SEQUENCING,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_relationship(
         status_db, case=case_wes_panel_error, sample=sample_case_wes_panel_error
     )
 
     # Create ERROR case with NO SAMPLES
```

### Comparing `cg-29.5.7/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-29.6.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 
 from _pytest.logging import LogCaptureFixture
 
 from cg.cli.workflow.balsamic.base import config_case
 from click.testing import CliRunner
 
+from cg.store import Store
 from cg.models.cg_config import CGConfig
 
 EXIT_SUCCESS = 0
 
 
 def test_without_options(cli_runner: CliRunner, balsamic_context: CGConfig):
     """Test command without case_id."""
```

### Comparing `cg-29.5.7/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-29.6.0/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/balsamic/test_link.py` & `cg-29.6.0/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-29.6.0/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/balsamic/test_run.py` & `cg-29.6.0/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-29.6.0/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/conftest.py` & `cg-29.6.0/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-29.6.0/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/fluffy/conftest.py` & `cg-29.6.0/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-29.6.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-29.6.0/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-29.6.0/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-29.6.0/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-29.6.0/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/microsalt/conftest.py` & `cg-29.6.0/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py` & `cg-29.6.0/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-29.6.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-29.6.0/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/mip/conftest.py` & `cg-29.6.0/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-29.6.0/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/rnafusion/conftest.py` & `cg-29.6.0/tests/cli/workflow/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-29.6.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-29.6.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py` & `cg-29.6.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py` & `cg-29.6.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-29.6.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-29.6.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py` & `cg-29.6.0/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/test_cli_workflow.py` & `cg-29.6.0/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-29.6.0/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/conftest.py` & `cg-29.6.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,14 +426,40 @@
     api = MockOsTicket()
     api.set_ticket_nr(ticket_id)
     return api
 
 
 # Files fixtures
 
+# Common file name fixtures
+
+
+@pytest.fixture(name="snv_vcf_file")
+def fixture_snv_vcf_file() -> str:
+    """Return a single nucleotide variant file name."""
+    return f"snv{FileExtensions.VCF}"
+
+
+@pytest.fixture(name="sv_vcf_file")
+def fixture_sv_vcf_file() -> str:
+    """Return a structural variant file name."""
+    return f"sv{FileExtensions.VCF}"
+
+
+@pytest.fixture(name="snv_research_vcf_file")
+def fixture_snv_research_vcf_file() -> str:
+    #    """Return a single nucleotide variant research file name."""
+    return f"snv_research{FileExtensions.VCF}"
+
+
+@pytest.fixture(name="sv_research_vcf_file")
+def fixture_sv_research_vcf_file() -> str:
+    """Return a structural variant research file name."""
+    return f"sv_research{FileExtensions.VCF}"
+
 
 # Common file fixtures
 @pytest.fixture(scope="session", name="fixtures_dir")
 def fixture_fixtures_dir() -> Path:
     """Return the path to the fixtures dir."""
     return Path("tests", "fixtures")
```

### Comparing `cg-29.5.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml` & `cg-29.6.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-29.6.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-29.6.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-29.6.0/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/analysis/sample_coverage.bed` & `cg-29.6.0/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/balsamic/case/config.json` & `cg-29.6.0/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-29.6.0/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-29.6.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-29.6.0/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters_different_index_cycles.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml` & `cg-29.6.0/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-29.6.0/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-29.6.0/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/madeline/madeline.xml` & `cg-29.6.0/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-29.6.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-29.6.0/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-29.6.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-29.6.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-29.6.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-29.6.0/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-29.6.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-29.6.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-29.6.0/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-29.6.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-29.6.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/scout/643594.config.yaml` & `cg-29.6.0/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/scout/case_export.json` & `cg-29.6.0/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/scout/export_causatives.json` & `cg-29.6.0/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/scout/none_case_export.json` & `cg-29.6.0/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/scout/other_sex_case.json` & `cg-29.6.0/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/scout/panel_export.bed` & `cg-29.6.0/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/apps/scout/panel_export.csv` & `cg-29.6.0/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/cgweb_orders/balsamic.json` & `cg-29.6.0/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/cgweb_orders/fastq.json` & `cg-29.6.0/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/cgweb_orders/metagenome.json` & `cg-29.6.0/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/cgweb_orders/microsalt.json` & `cg-29.6.0/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/cgweb_orders/mip.json` & `cg-29.6.0/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-29.6.0/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/cgweb_orders/rml.json` & `cg-29.6.0/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-29.6.0/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/data/SampleSheet.csv` & `cg-29.6.0/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/data/cgfixture.db` & `cg-29.6.0/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/data/hkstore.db` & `cg-29.6.0/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/io/example_json.json` & `cg-29.6.0/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/1508.27.balsamic.xlsx` & `cg-29.6.0/tests/fixtures/orderforms/1508.27.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx` & `cg-29.6.0/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx` & `cg-29.6.0/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/1508.27.fastq.xlsx` & `cg-29.6.0/tests/fixtures/orderforms/1508.27.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/1508.27.mip.xlsx` & `cg-29.6.0/tests/fixtures/orderforms/1508.27.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/1508.27.mip_rna.xlsx` & `cg-29.6.0/tests/fixtures/orderforms/1508.27.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-29.6.0/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/1604.15.rml.xlsx` & `cg-29.6.0/tests/fixtures/orderforms/1604.15.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/1605.10.metagenome.xlsx` & `cg-29.6.0/tests/fixtures/orderforms/1605.10.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/2184.7.sarscov2.xlsx` & `cg-29.6.0/tests/fixtures/orderforms/2184.7.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/NIPT-json.json` & `cg-29.6.0/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-29.6.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-29.6.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/report/case_data.json` & `cg-29.6.0/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/report/lims_exported_samples.json` & `cg-29.6.0/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/fixtures/report/lims_family.json` & `cg-29.6.0/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/io/conftest.py` & `cg-29.6.0/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/io/test_io_controller.py` & `cg-29.6.0/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/io/test_io_csv.py` & `cg-29.6.0/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/io/test_io_json.py` & `cg-29.6.0/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/io/test_io_yaml.py` & `cg-29.6.0/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/archive/conftest.py` & `cg-29.6.0/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/archive/test_archiving.py` & `cg-29.6.0/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/backup/conftest.py` & `cg-29.6.0/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/backup/test_meta_backup.py` & `cg-29.6.0/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/backup/test_meta_pdc.py` & `cg-29.6.0/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/clean/conftest.py` & `cg-29.6.0/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/clean/test_clean_demultiplexed_runs.py` & `cg-29.6.0/tests/meta/clean/test_clean_demultiplexed_runs.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/clean/test_clean_flow_cell_run_directories.py` & `cg-29.6.0/tests/meta/clean/test_clean_flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/compress/conftest.py` & `cg-29.6.0/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/compress/test_clean_fastq.py` & `cg-29.6.0/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/compress/test_compress_files.py` & `cg-29.6.0/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/compress/test_compress_meta_fastq.py` & `cg-29.6.0/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/compress/test_decompress_spring_meta.py` & `cg-29.6.0/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-29.6.0/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/conftest.py` & `cg-29.6.0/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/deliver/conftest.py` & `cg-29.6.0/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/deliver/test_deliver_ticket.py` & `cg-29.6.0/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/deliver/test_delivery_api.py` & `cg-29.6.0/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/demultiplex/conftest.py` & `cg-29.6.0/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/demultiplex/test_delete_demultiplex_api.py` & `cg-29.6.0/tests/meta/demultiplex/test_delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-29.6.0/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/demultiplex/test_rename_files.py` & `cg-29.6.0/tests/meta/demultiplex/test_rename_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/encryption/conftest.py` & `cg-29.6.0/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/encryption/test_encryption.py` & `cg-29.6.0/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/observations/conftest.py` & `cg-29.6.0/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/observations/test_meta_upload_observations.py` & `cg-29.6.0/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/orders/conftest.py` & `cg-29.6.0/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-29.6.0/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-29.6.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-29.6.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-29.6.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/orders/test_meta_orders_api.py` & `cg-29.6.0/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/orders/test_meta_orders_lims.py` & `cg-29.6.0/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/orders/test_meta_orders_status.py` & `cg-29.6.0/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/orders/test_ticket_handler.py` & `cg-29.6.0/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/report/conftest.py` & `cg-29.6.0/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/report/test_balsamic_api.py` & `cg-29.6.0/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/report/test_field_validators.py` & `cg-29.6.0/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/report/test_mip_dna_api.py` & `cg-29.6.0/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/report/test_report_api.py` & `cg-29.6.0/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/rsync/conftest.py` & `cg-29.6.0/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/rsync/test_rsync.py` & `cg-29.6.0/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/test_invoice.py` & `cg-29.6.0/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/transfer/conftest.py` & `cg-29.6.0/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/transfer/test_external_data.py` & `cg-29.6.0/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/transfer/test_meta_transfer_flowcell.py` & `cg-29.6.0/tests/meta/transfer/test_meta_transfer_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-29.6.0/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/balsamic/test_balsamic.py` & `cg-29.6.0/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/conftest.py` & `cg-29.6.0/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/gisaid/conftest.py` & `cg-29.6.0/tests/meta/upload/gisaid/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-29.6.0/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/mutacc/conftest.py` & `cg-29.6.0/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-29.6.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/nipt/conftest.py` & `cg-29.6.0/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-29.6.0/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/scout/conftest.py` & `cg-29.6.0/tests/meta/upload/scout/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 """Fixtures for the upload Scout API tests."""
 
 import logging
 from datetime import datetime
 from pathlib import Path
-from typing import Generator, List
+from typing import Dict, Generator, List
 
 import pytest
 from housekeeper.store.models import Version
 
 from cg.constants import DataDelivery, FileExtensions, Pipeline
 from cg.constants.constants import FileFormat, PrepCategory
 from cg.constants.sequencing import SequencingMethod
 from cg.io.controller import ReadFile
 from cg.meta.upload.scout.balsamic_config_builder import BalsamicConfigBuilder
 from cg.meta.upload.scout.mip_config_builder import MipConfigBuilder
 from cg.meta.upload.scout.uploadscoutapi import UploadScoutAPI
 from cg.models.scout.scout_load_config import MipLoadConfig
 from cg.store import Store
-from cg.store.models import Analysis, Family
+from cg.store.models import Analysis, Family, Sample
 
 # Mocks
 from tests.mocks.hk_mock import MockHousekeeperAPI
 from tests.mocks.limsmock import MockLimsAPI
 from tests.mocks.madeline import MockMadelineAPI
 from tests.mocks.mip_analysis_mock import MockMipAnalysis
 from tests.mocks.scout import MockScoutAPI
 from tests.store_helpers import StoreHelpers
 
 LOG = logging.getLogger(__name__)
-SNV_FILE_NAME: str = f"snv{FileExtensions.VCF}"
 
 
 @pytest.fixture(name="rna_case_id")
 def fixture_rna_case_id() -> str:
     """Return a rna case id."""
     return "affirmativecat"
 
@@ -254,39 +253,46 @@
 def fixture_lims_samples(lims_family: dict) -> List[dict]:
     """Returns the samples of a LIMS case."""
     return lims_family["samples"]
 
 
 @pytest.fixture(scope="function", name="mip_dna_analysis_hk_bundle_data")
 def fixture_mip_dna_analysis_hk_bundle_data(
-    case_id: str, timestamp: datetime, mip_dna_analysis_dir: Path, sample_id: str
+    case_id: str,
+    timestamp: datetime,
+    mip_dna_analysis_dir: Path,
+    sample_id: str,
+    snv_vcf_file: str,
+    sv_vcf_file: str,
+    snv_research_vcf_file: str,
+    sv_research_vcf_file: str,
 ) -> dict:
     """Return MIP DNA bundle data for Housekeeper."""
     return {
         "name": case_id,
         "created": timestamp,
         "expires": timestamp,
         "files": [
             {
-                "path": Path(mip_dna_analysis_dir, SNV_FILE_NAME).as_posix(),
+                "path": Path(mip_dna_analysis_dir, snv_vcf_file).as_posix(),
                 "archive": False,
                 "tags": ["vcf-snv-clinical"],
             },
             {
-                "path": Path(mip_dna_analysis_dir, "sv.vcf").as_posix(),
+                "path": Path(mip_dna_analysis_dir, sv_vcf_file).as_posix(),
                 "archive": False,
                 "tags": ["vcf-sv-clinical"],
             },
             {
-                "path": Path(mip_dna_analysis_dir, "snv_research.vcf").as_posix(),
+                "path": Path(mip_dna_analysis_dir, snv_research_vcf_file).as_posix(),
                 "archive": False,
                 "tags": ["vcf-snv-research"],
             },
             {
-                "path": Path(mip_dna_analysis_dir, "sv_research.vcf").as_posix(),
+                "path": Path(mip_dna_analysis_dir, sv_research_vcf_file).as_posix(),
                 "archive": False,
                 "tags": ["vcf-sv-research"],
             },
             {
                 "path": Path(mip_dna_analysis_dir, "str.vcf").as_posix(),
                 "archive": False,
                 "tags": ["vcf-str"],
@@ -333,15 +339,15 @@
     rna_sample_son_id: str,
     rna_sample_daughter_id: str,
     rna_sample_mother_id: str,
     rna_sample_father_id: str,
 ) -> dict:
     """Return MIP RNA bundle data for Housekeeper."""
 
-    files: [dict] = [
+    files: List[dict] = [
         {
             "path": Path(mip_dna_analysis_dir, f"{rna_case_id}_report.selected.pdf").as_posix(),
             "archive": False,
             "tags": ["fusion", "pdf", "clinical", rna_case_id],
         },
         {
             "path": Path(mip_dna_analysis_dir, f"{rna_case_id}_report.pdf").as_posix(),
@@ -380,29 +386,34 @@
         "expires": timestamp,
         "files": files,
     }
 
 
 @pytest.fixture(scope="function", name="balsamic_analysis_hk_bundle_data")
 def fixture_balsamic_analysis_hk_bundle_data(
-    case_id: str, timestamp: datetime, balsamic_wgs_analysis_dir: Path, sample_id: str
+    case_id: str,
+    timestamp: datetime,
+    balsamic_wgs_analysis_dir: Path,
+    sample_id: str,
+    snv_vcf_file: str,
+    sv_vcf_file: str,
 ) -> dict:
     """Return Balsamic bundle data for Housekeeper,"""
     return {
         "name": case_id,
         "created": timestamp,
         "expires": timestamp,
         "files": [
             {
-                "path": Path(balsamic_wgs_analysis_dir, SNV_FILE_NAME).as_posix(),
+                "path": Path(balsamic_wgs_analysis_dir, snv_vcf_file).as_posix(),
                 "archive": False,
                 "tags": ["vcf-snv-clinical"],
             },
             {
-                "path": Path(balsamic_wgs_analysis_dir, "sv.vcf").as_posix(),
+                "path": Path(balsamic_wgs_analysis_dir, sv_vcf_file).as_posix(),
                 "archive": False,
                 "tags": ["vcf-sv-clinical"],
             },
             {
                 "path": Path(balsamic_wgs_analysis_dir, "umi.sv.vcf").as_posix(),
                 "archive": False,
                 "tags": ["vcf-umi-snv-clinical"],
@@ -603,21 +614,21 @@
         analysis_obj=balsamic_analysis_obj,
         lims_api=lims_api,
     )
 
 
 @pytest.fixture(name="mip_load_config")
 def fixture_mip_load_config(
-    mip_dna_analysis_dir: Path, case_id: str, customer_id: str
+    mip_dna_analysis_dir: Path, case_id: str, customer_id: str, snv_vcf_file: str
 ) -> MipLoadConfig:
     """Return a valid MIP load_config."""
     return MipLoadConfig(
         owner=customer_id,
         family=case_id,
-        vcf_snv=Path(mip_dna_analysis_dir, SNV_FILE_NAME).as_posix(),
+        vcf_snv=Path(mip_dna_analysis_dir, snv_vcf_file).as_posix(),
         track="rare",
     )
 
 
 @pytest.fixture(name="lims_api")
 def fixture_lims_api(lims_samples: List[dict]) -> MockLimsAPI:
     """Return a LIMS API."""
@@ -692,14 +703,32 @@
         madeline_api=madeline_api,
         analysis_api=analysis_mock,
         lims_api=lims_api,
         status_db=store,
     )
 
 
+@pytest.fixture(name="rna_dna_sample_case_map")
+def fixture_rna_dna_sample_case_map(
+    rna_sample_son_id: str,
+    rna_store: Store,
+    upload_scout_api: UploadScoutAPI,
+) -> Dict[str, List[str]]:
+    """Return a valid RNA-DNA case map."""
+    rna_sample: Sample = rna_store.get_sample_by_internal_id(internal_id=rna_sample_son_id)
+
+    # WHEN adding the RNA sample rna_dna_case_map
+    rna_dna_sample_case_map: Dict[str, Dict[str, List[str]]] = {}
+    upload_scout_api._map_dna_samples_related_to_rna_sample(
+        rna_sample=rna_sample, rna_dna_sample_case_map=rna_dna_sample_case_map
+    )
+
+    return rna_dna_sample_case_map
+
+
 @pytest.fixture(name="upload_rnafusion_analysis_scout_api")
 def fixture_upload_rnafusion_analysis_scout_api(
     scout_api: MockScoutAPI,
     madeline_api: MockMadelineAPI,
     lims_samples: List[dict],
     rnafusion_analysis_hk_api: MockHousekeeperAPI,
     store: Store,
```

### Comparing `cg-29.5.7/tests/meta/upload/scout/test_generate_load_config.py` & `cg-29.6.0/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-29.6.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-29.6.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 """Tests for RNA part of the scout upload API"""
 import logging
-from typing import Generator, List
+from typing import Dict, Generator, List, Set
+from pathlib import Path
+
 import pytest
 from _pytest.logging import LogCaptureFixture
 
 from sqlalchemy.orm import Query
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants import Pipeline
 from cg.constants.sequencing import SequencingMethod
+from cg.constants.scout_upload import ScoutCustomCaseReportTags
 from cg.exc import CgDataError
 from cg.meta.upload.scout.uploadscoutapi import UploadScoutAPI
 from cg.store.models import Family, Sample
 import cg.store as Store
 from tests.store_helpers import StoreHelpers
+from tests.mocks.hk_mock import MockHousekeeperAPI
+from housekeeper.store.models import File
 
 
 def set_is_tumour_on_case(store: Store, case_id: str, is_tumour: bool):
     for link in store.get_case_by_internal_id(internal_id=case_id).links:
         link.sample.is_tumour = is_tumour
 
 
@@ -555,15 +560,15 @@
     """Test for a given RNA sample, the associated DNA sample name matches and is present in rna_dna_case_map."""
 
     # GIVEN an RNA sample
     rna_sample: Sample = rna_store.get_sample_by_internal_id(rna_sample_son_id)
 
     # WHEN adding the RNA sample to the rna_dna_case_map
     rna_dna_case_map: dict = {}
-    upload_scout_api._add_rna_sample(
+    upload_scout_api.build_rna_sample_map(
         rna_sample=rna_sample, rna_dna_sample_case_map=rna_dna_case_map
     )
 
     # THEN the rna_dna_case_map should contain the RNA sample
     assert rna_sample_son_id in rna_dna_case_map
 
     # THEN the rna_dna_case_map values should contain the associated DNA sample
@@ -577,20 +582,209 @@
     rna_sample_son_id: str,
     rna_store: Store,
     upload_scout_api: UploadScoutAPI,
 ):
     """Test for a given RNA sample, the DNA case name matches to the case name of the DNA sample in rna_dna_case_map."""
 
     # GIVEN an RNA sample, a DNA sample, and a DNA case
-    rna_sample: Sample = rna_store.get_sample_by_internal_id(rna_sample_son_id)
-    dna_sample: Sample = rna_store.get_sample_by_internal_id(dna_sample_son_id)
+    rna_sample: Sample = rna_store.get_sample_by_internal_id(internal_id=rna_sample_son_id)
+    dna_sample: Sample = rna_store.get_sample_by_internal_id(internal_id=dna_sample_son_id)
     dna_case: Family = rna_store.get_case_by_internal_id(internal_id=dna_case_id)
 
     # WHEN adding the RNA sample rna_dna_case_map
     rna_dna_case_map: dict = {}
-    upload_scout_api._add_rna_sample(
+    upload_scout_api.build_rna_sample_map(
         rna_sample=rna_sample, rna_dna_sample_case_map=rna_dna_case_map
     )
 
     # THEN the rna_dna_case_map should contain the DNA_case name associated with the DNA sample
     case_names: list = rna_dna_case_map[rna_sample.internal_id][dna_sample.name]
     assert dna_case.internal_id in case_names
+
+
+def test_map_dna_cases_to_dna_sample(
+    rna_store: Store,
+    upload_scout_api: UploadScoutAPI,
+    dna_sample_son_id: str,
+    rna_sample_son_id: str,
+    rna_dna_sample_case_map: Dict[str, Dict[str, List[str]]],
+):
+    """Test that the DNA case name is mapped to the DNA sample name in the rna_dna_case_map."""
+
+    # GIVEN an RNA sample, a DNA sample, and a rna-dna case map
+
+    dna_sample: Sample = rna_store.get_sample_by_internal_id(internal_id=dna_sample_son_id)
+    rna_sample: Sample = rna_store.get_sample_by_internal_id(internal_id=rna_sample_son_id)
+
+    # WHEN mapping the DNA case name to the DNA sample name in the rna_dna_case_map
+    upload_scout_api._map_dna_cases_to_dna_sample(
+        dna_sample=dna_sample,
+        rna_dna_sample_case_map=rna_dna_sample_case_map,
+        rna_sample=rna_sample,
+    )
+
+    # THEN the rna_dna_case_map should contain the DNA case name associated with the DNA sample name
+    assert dna_sample.name in rna_dna_sample_case_map[rna_sample.internal_id]
+
+
+def test_map_dna_cases_to_dna_sample_incorrect_pipeline(
+    rna_store: Store,
+    upload_scout_api: UploadScoutAPI,
+    dna_sample_son_id: str,
+    dna_case_id: str,
+    rna_sample_son_id: str,
+    rna_dna_sample_case_map: Dict[str, Dict[str, List[str]]],
+):
+    """Test that the DNA case name is not mapped to the DNA sample name in the rna-dna-sample-case map."""
+
+    # GIVEN an RNA sample, a DNA sample, and a rna-dna case map
+
+    dna_sample: Sample = rna_store.get_sample_by_internal_id(internal_id=dna_sample_son_id)
+    dna_case: Family = rna_store.get_case_by_internal_id(internal_id=dna_case_id)
+    rna_sample: Sample = rna_store.get_sample_by_internal_id(internal_id=rna_sample_son_id)
+
+    # GIVEN that the DNA case has a different pipeline than the expected pipeline
+    dna_case.data_analysis: Pipeline = Pipeline.FASTQ
+
+    # WHEN mapping the DNA case name to the DNA sample name in the rna-dna-sample-case map
+    upload_scout_api._map_dna_cases_to_dna_sample(
+        dna_sample=dna_sample,
+        rna_dna_sample_case_map=rna_dna_sample_case_map,
+        rna_sample=rna_sample,
+    )
+
+    # THEN the rna-dna-sample-case map should not contain the DNA case name associated with the DNA sample name
+    assert (
+        dna_case.internal_id
+        not in rna_dna_sample_case_map[rna_sample.internal_id][dna_sample_son_id]
+    )
+
+
+def test_map_dna_cases_to_dna_sample_incorrect_customer(
+    rna_store: Store,
+    upload_scout_api: UploadScoutAPI,
+    dna_sample_son_id: str,
+    dna_case_id: str,
+    rna_sample_son_id: str,
+    rna_dna_sample_case_map: Dict[str, Dict[str, List[str]]],
+):
+    """Test that the DNA case name is not mapped to the DNA sample name in the rna-dna-sample-case map."""
+
+    # GIVEN an RNA sample, a DNA sample, and a rna-dna case map
+
+    dna_sample: Sample = rna_store.get_sample_by_internal_id(internal_id=dna_sample_son_id)
+    dna_case: Family = rna_store.get_case_by_internal_id(internal_id=dna_case_id)
+    rna_sample: Sample = rna_store.get_sample_by_internal_id(internal_id=rna_sample_son_id)
+
+    # GIVEN that the DNA case has a different customer than the expected customer
+    dna_case.customer_id: int = 1000
+
+    # WHEN mapping the DNA case name to the DNA sample name in the rna-dna-sample-case map
+    upload_scout_api._map_dna_cases_to_dna_sample(
+        dna_sample=dna_sample,
+        rna_dna_sample_case_map=rna_dna_sample_case_map,
+        rna_sample=rna_sample,
+    )
+
+    # THEN the rna-dna-sample-case map should not contain the DNA case name associated with the DNA sample name
+    assert (
+        dna_case.internal_id
+        not in rna_dna_sample_case_map[rna_sample.internal_id][dna_sample_son_id]
+    )
+
+
+def test_get_multiqc_html_report(
+    dna_case_id: str,
+    rna_store: Store,
+    upload_mip_analysis_scout_api: UploadScoutAPI,
+    mip_dna_analysis_hk_api: MockHousekeeperAPI,
+):
+    """Test that the multiqc html report is returned."""
+
+    # GIVEN an DNA case with a multiqc-htlml report
+    case: Family = rna_store.get_case_by_internal_id(internal_id=dna_case_id)
+    multiqc_file: File = mip_dna_analysis_hk_api.files(
+        bundle=dna_case_id, tags=[ScoutCustomCaseReportTags.MULTIQC]
+    )[0]
+
+    # WHEN getting the multiqc html report
+    report_type, multiqc_report = upload_mip_analysis_scout_api.get_multiqc_html_report(
+        case_id=dna_case_id, pipeline=case.data_analysis
+    )
+
+    # THEN the multiqc html report should be returned and the correct report type
+    assert multiqc_report.full_path == multiqc_file.full_path
+    assert report_type == ScoutCustomCaseReportTags.MULTIQC
+
+
+def test_upload_report_to_scout(
+    caplog,
+    dna_case_id: str,
+    upload_mip_analysis_scout_api: UploadScoutAPI,
+    mip_dna_analysis_hk_api: MockHousekeeperAPI,
+):
+    """Test that the uploaded of a report to Scout is possible."""
+
+    caplog.set_level(logging.INFO)
+
+    # GIVEN an DNA case with a multiqc-htlml report
+    multiqc_file: File = mip_dna_analysis_hk_api.files(
+        bundle=dna_case_id, tags=[ScoutCustomCaseReportTags.MULTIQC]
+    )[0]
+    assert multiqc_file
+
+    # WHEN uploading a report to Scout
+    upload_mip_analysis_scout_api.upload_report_to_scout(
+        dry_run=False,
+        case_id=dna_case_id,
+        report_type=ScoutCustomCaseReportTags.MULTIQC,
+        report_file=multiqc_file,
+    )
+
+    # THEN the report should be uploaded to Scout
+    assert (
+        f"Uploading {ScoutCustomCaseReportTags.MULTIQC} report to case {dna_case_id}" in caplog.text
+    )
+
+
+def test_upload_rna_report_to_dna_case_in_scout(
+    caplog,
+    rna_case_id: str,
+    rna_store: Store,
+    upload_mip_analysis_scout_api: UploadScoutAPI,
+    mip_rna_analysis_hk_api: MockHousekeeperAPI,
+):
+    """Test that the report is uploaded to Scout."""
+
+    caplog.set_level(logging.INFO)
+
+    # GIVEN an RNA case, and an store with an rna connected to it
+    upload_mip_analysis_scout_api.status_db: Store = rna_store
+
+    # GIVEN an RNA case with a multiqc-htlml report
+    multiqc_file: File = mip_rna_analysis_hk_api.files(
+        bundle=rna_case_id, tags=[ScoutCustomCaseReportTags.MULTIQC]
+    )[0]
+
+    # WHEN uploading a report to Scout
+    upload_mip_analysis_scout_api.upload_rna_report_to_dna_case_in_scout(
+        dry_run=False,
+        rna_case_id=rna_case_id,
+        report_type=ScoutCustomCaseReportTags.MULTIQC,
+        report_file=multiqc_file,
+    )
+
+    # WHEN finding the related DNA case
+    dna_case_ids: Set[str] = upload_mip_analysis_scout_api.get_unique_dna_cases_related_to_rna_case(
+        case_id=rna_case_id
+    )
+
+    # THEN the api should know that it should find related DNA cases
+
+    assert f"Finding DNA cases related to RNA case {rna_case_id}" in caplog.text
+
+    # THEN the report should be uploaded to Scout
+    for case_id in dna_case_ids:
+        assert (
+            f"Uploading {ScoutCustomCaseReportTags.MULTIQC} report to scout for case {case_id}"
+            in caplog.text
+        )
```

### Comparing `cg-29.5.7/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-29.6.0/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/test_meta_upload_coverage.py` & `cg-29.6.0/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/test_upload_api.py` & `cg-29.6.0/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/test_upload_genotypes_api.py` & `cg-29.6.0/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/vogue/conftest.py` & `cg-29.6.0/tests/meta/upload/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/upload/vogue/test_upload_vogue.py` & `cg-29.6.0/tests/meta/upload/vogue/test_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/workflow/conftest.py` & `cg-29.6.0/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/workflow/test_analysis.py` & `cg-29.6.0/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/workflow/test_balsamic.py` & `cg-29.6.0/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/workflow/test_microsalt.py` & `cg-29.6.0/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-29.6.0/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/mocks/balsamic_analysis_mock.py` & `cg-29.6.0/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/mocks/crunchy.py` & `cg-29.6.0/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/mocks/hk_mock.py` & `cg-29.6.0/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/mocks/limsmock.py` & `cg-29.6.0/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/mocks/madeline.py` & `cg-29.6.0/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/mocks/mip_analysis_mock.py` & `cg-29.6.0/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/mocks/osticket.py` & `cg-29.6.0/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/mocks/process_mock.py` & `cg-29.6.0/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/mocks/report.py` & `cg-29.6.0/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/mocks/scout.py` & `cg-29.6.0/tests/mocks/scout.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import logging
 from pathlib import Path
 from pydantic import BaseModel, validator
 from typing import List
 from typing_extensions import Literal
 
 from cg.apps.scout.scoutapi import ScoutAPI
+from tests.mocks.process_mock import ProcessMock
+
 
 LOG = logging.getLogger(__name__)
 
 
 class MockScoutIndividual(BaseModel):
     sample_id: str = "sample_id"
     sex: str = "female"
@@ -53,14 +55,15 @@
         self._config = config or {}
         self._gene_panel = {}
         self._panels = []
         self._causatives = []
         self._cases = []
         self._upload_report_success = True
         self._alignment_file_updated = 0
+        self.process = ProcessMock(binary="scout", error=False)
 
     # Mock specific functions
 
     def set_report_fail(self):
         """Sets the upload report to fail"""
         self._upload_report_success = False
```

### Comparing `cg-29.5.7/tests/mocks/store_model.py` & `cg-29.6.0/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/mocks/tb_mock.py` & `cg-29.6.0/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/balsamic/conftest.py` & `cg-29.6.0/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/balsamic/test_balsamic_analysis.py` & `cg-29.6.0/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/conftest.py` & `cg-29.6.0/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/demultiplexing/conftest.py` & `cg-29.6.0/tests/models/demultiplexing/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/demultiplexing/test_demux_results.py` & `cg-29.6.0/tests/models/demultiplexing/test_demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/demultiplexing/test_flowcell_model.py` & `cg-29.6.0/tests/models/demultiplexing/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/demultiplexing/test_run_parameters.py` & `cg-29.6.0/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/mip/conftest.py` & `cg-29.6.0/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/mip/test_mip_analysis.py` & `cg-29.6.0/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/mip/test_mip_config.py` & `cg-29.6.0/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-29.6.0/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/mip/test_mip_sample_info.py` & `cg-29.6.0/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/nextflow/conftest.py` & `cg-29.6.0/tests/models/nextflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/nextflow/test_nextflow_deliver.py` & `cg-29.6.0/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/observations/conftest.py` & `cg-29.6.0/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/observations/test_observations_input_files.py` & `cg-29.6.0/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/report/test_validators.py` & `cg-29.6.0/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/rnafusion/conftest.py` & `cg-29.6.0/tests/models/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-29.6.0/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/test_cg_models.py` & `cg-29.6.0/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/test_compression_data.py` & `cg-29.6.0/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/test_file_data.py` & `cg-29.6.0/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/models/test_flowcell_class.py` & `cg-29.6.0/tests/models/test_flowcell_class.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/server/conftest.py` & `cg-29.6.0/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/add/test_store_add_application_version.py` & `cg-29.6.0/tests/store/api/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/add/test_store_add_base.py` & `cg-29.6.0/tests/store/api/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/add/test_store_add_customer.py` & `cg-29.6.0/tests/store/api/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/add/test_store_add_flow_celll.py` & `cg-29.6.0/tests/store/api/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/conftest.py` & `cg-29.6.0/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/delete/test_store_api_delete.py` & `cg-29.6.0/tests/store/api/delete/test_store_api_delete.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/find/test_find_basic_data.py` & `cg-29.6.0/tests/store/api/find/test_find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/find/test_find_basic_data_application_version.py` & `cg-29.6.0/tests/store/api/find/test_find_basic_data_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/find/test_find_business_data.py` & `cg-29.6.0/tests/store/api/find/test_find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/find/test_find_business_data_analysis.py` & `cg-29.6.0/tests/store/api/find/test_find_business_data_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/find/test_find_business_data_case.py` & `cg-29.6.0/tests/store/api/find/test_find_business_data_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/find/test_find_business_data_sample.py` & `cg-29.6.0/tests/store/api/find/test_find_business_data_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/status/test_analyses_to_clean.py` & `cg-29.6.0/tests/store/api/status/test_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/status/test_analyses_to_delivery_report.py` & `cg-29.6.0/tests/store/api/status/test_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/status/test_store_api_status.py` & `cg-29.6.0/tests/store/api/status/test_store_api_status.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/status/test_store_api_status_analysis.py` & `cg-29.6.0/tests/store/api/status/test_store_api_status_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/status/test_store_api_status_cases.py` & `cg-29.6.0/tests/store/api/status/test_store_api_status_cases.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-"""This script tests the cli methods to add families to status-db"""
-from datetime import datetime, timedelta
-
 from cg.constants import CASE_ACTIONS, DataDelivery, Pipeline
 from cg.store import Store
 from cg.store.models import Analysis, Family
 from cg.constants import Priority
+from datetime import datetime, timedelta
 
 
 def test_delivered_at_affects_tat(base_store: Store, helpers):
     """test that the estimated turnaround time is affected by the delivered_at date"""
 
     # GIVEN a database with a case and a samples receive_at, prepared_at, sequenced_at,
     # delivered_at one week ago
```

### Comparing `cg-29.5.7/tests/store/api/status/test_store_api_status_customer.py` & `cg-29.6.0/tests/store/api/status/test_store_api_status_customer.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/status/test_store_api_status_pool.py` & `cg-29.6.0/tests/store/api/status/test_store_api_status_pool.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/status/test_store_api_status_sample.py` & `cg-29.6.0/tests/store/api/status/test_store_api_status_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/api/test_base.py` & `cg-29.6.0/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/conftest.py` & `cg-29.6.0/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_analyses_filters.py` & `cg-29.6.0/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_application_filters.py` & `cg-29.6.0/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_application_version_filters.py` & `cg-29.6.0/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_bed_filters.py` & `cg-29.6.0/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_bed_version_filters.py` & `cg-29.6.0/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_case_sample_filters.py` & `cg-29.6.0/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_cases_filters.py` & `cg-29.6.0/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_collaboration_filters.py` & `cg-29.6.0/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_customer_filters.py` & `cg-29.6.0/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_flow_cell_filters.py` & `cg-29.6.0/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_invoice_filters.py` & `cg-29.6.0/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_organism_filters.py` & `cg-29.6.0/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_panel_filters.py` & `cg-29.6.0/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_pool_filters.py` & `cg-29.6.0/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_samples_filters.py` & `cg-29.6.0/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/filters/test_status_user_filters.py` & `cg-29.6.0/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/test_delivery.py` & `cg-29.6.0/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store/test_store_models.py` & `cg-29.6.0/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/store_helpers.py` & `cg-29.6.0/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/test_store_helpers.py` & `cg-29.6.0/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/utils/conftest.py` & `cg-29.6.0/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/utils/test_commands.py` & `cg-29.6.0/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/utils/test_date.py` & `cg-29.6.0/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/utils/test_dict.py` & `cg-29.6.0/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/utils/test_dispatcher.py` & `cg-29.6.0/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-29.5.7/tests/utils/test_utils.py` & `cg-29.6.0/tests/utils/test_utils.py`

 * *Files identical despite different names*

