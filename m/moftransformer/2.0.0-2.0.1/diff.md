# Comparing `tmp/moftransformer-2.0.0.tar.gz` & `tmp/moftransformer-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moftransformer-2.0.0.tar", last modified: Thu Apr 27 12:01:12 2023, max compression
+gzip compressed data, was "moftransformer-2.0.1.tar", last modified: Fri May  5 08:01:44 2023, max compression
```

## Comparing `moftransformer-2.0.0.tar` & `moftransformer-2.0.1.tar`

### file list

```diff
@@ -1,285 +1,154 @@
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8153 2023-04-27 12:01:12.629117 moftransformer-2.0.0/PKG-INFO
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7775 2023-04-27 05:35:23.000000 moftransformer-2.0.0/README.md
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      398 2023-04-27 11:58:33.000000 moftransformer-2.0.0/moftransformer/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/assets/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       72 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/assets/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12616 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/assets/bbs.json
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8140 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/assets/colors.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12647 2023-01-26 02:06:32.000000 moftransformer-2.0.0/moftransformer/assets/topology.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/cli/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       31 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/cli/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2443 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/cli/download.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      324 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/cli/install_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3040 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/cli/main.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      576 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/cli/run.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      328 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/cli/uninstall_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3427 2023-04-27 11:43:43.000000 moftransformer-2.0.0/moftransformer/config.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10515 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/config_ex.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/database/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      633 2023-04-27 04:48:37.000000 moftransformer-2.0.0/moftransformer/database/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/datamodules/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      210 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/datamodules/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2938 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/datamodules/datamodule.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10088 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/datamodules/dataset.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/examples/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      477 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/examples/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/examples/dataset/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.621117 moftransformer-2.0.0/moftransformer/examples/dataset/test/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/acs+N270+E33.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/acs+N270+E33.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/acs+N270+E33.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/acs+N270+E33.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/smm+N577+E166.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/smm+N577+E166.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/smm+N577+E166.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/smm+N577+E166.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       73 2023-04-04 13:24:22.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.621117 moftransformer-2.0.0/moftransformer/examples/dataset/total/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-01-05 12:09:32.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/acs+N270+E33.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-01-05 12:09:32.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/acs+N270+E33.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:32.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/acs+N270+E33.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:32.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/acs+N270+E33.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/fee+N254+E185.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/fee+N254+E185.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/fee+N254+E185.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/fee+N254+E185.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mok+N109+E146.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mok+N109+E146.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mok+N109+E146.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mok+N109+E146.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/msp+N624+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/msp+N624+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/msp+N624+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/sml+N696+E182.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/sml+N696+E182.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/sml+N696+E182.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/sml+N696+E182.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/smm+N577+E166.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/smm+N577+E166.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/smm+N577+E166.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/smm+N577+E166.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/ukg+N387+E203.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/ukg+N387+E203.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vmk+N489+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vmk+N489+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-01-05 12:09:30.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vna+N650+E120.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-01-05 12:09:30.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vna+N650+E120.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:30.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vna+N650+E120.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:30.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vna+N650+E120.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.625117 moftransformer-2.0.0/moftransformer/examples/dataset/train/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/fee+N254+E185.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/fee+N254+E185.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/fee+N254+E185.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/fee+N254+E185.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mok+N109+E146.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mok+N109+E146.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mok+N109+E146.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mok+N109+E146.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/msp+N624+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/msp+N624+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/msp+N624+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/sml+N696+E182.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/sml+N696+E182.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/sml+N696+E182.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/sml+N696+E182.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/ukg+N387+E203.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/ukg+N387+E203.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vmk+N489+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vmk+N489+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vna+N650+E120.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vna+N650+E120.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vna+N650+E120.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vna+N650+E120.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      206 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.625117 moftransformer-2.0.0/moftransformer/examples/dataset/val/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/acs+N270+E33.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/acs+N270+E33.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/acs+N270+E33.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/acs+N270+E33.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/smm+N577+E166.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/smm+N577+E166.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/smm+N577+E166.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/smm+N577+E166.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       43 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.625117 moftransformer-2.0.0/moftransformer/examples/raw/
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7496 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/acs+N270+E33.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    17441 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9738 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/fee+N254+E185.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11392 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/mok+N109+E146.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    30404 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18345 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/raw_example.json
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11939 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/sml+N696+E182.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    24953 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/smm+N577+E166.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    28256 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/ukg+N387+E203.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    39904 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/vmk+N489+E8.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18930 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/vna+N650+E120.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    48803 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/zzz+N96+N373+E34.cif
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/examples/visualize/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.625117 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.625117 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9162 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12083 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6405 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8339 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7074 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9292 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    98728 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6419 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8357 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    93472 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6410 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8347 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6845 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8961 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   170530 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      164 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.625117 moftransformer-2.0.0/moftransformer/gadgets/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       77 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/gadgets/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1806 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/gadgets/my_metrics.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/libs/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/moftransformer/libs/GRIDAY/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2799 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/AtomTypeMap.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      654 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/AtomTypeMap.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    41808 2022-12-19 08:32:53.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/AtomTypeMap.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2448 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Cell.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7789 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      414 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    33448 2022-12-19 08:32:54.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54588 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18619 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3812 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   143440 2022-12-19 08:32:55.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.o
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4751 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/UFF_FF.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      845 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/UFF_Type.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      202 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      190 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      318 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       26 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7197 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ForceField.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      866 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ForceField.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    67552 2022-12-19 08:32:55.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ForceField.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13991 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      865 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    57152 2022-12-19 08:32:56.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FourierAnalyzer.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7362 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Framework.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1197 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Framework.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    47328 2022-12-19 08:32:57.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Framework.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3007 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Gaussian.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Gaussian.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15032 2022-12-19 08:32:57.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Gaussian.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9534 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridMaker.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      936 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridMaker.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    80288 2022-12-19 08:32:58.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridMaker.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Griday.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      948 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayException.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      669 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayException.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15752 2022-12-19 08:32:58.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayException.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      567 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayTypes.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4380 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/LennardJones.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/LennardJones.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    14896 2022-12-19 08:32:58.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/LennardJones.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      334 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Makefile
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    21824 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/MaterialGrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2366 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/MaterialGrid.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    75600 2022-12-19 08:32:59.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/MaterialGrid.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5664 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/NlistMaker.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      922 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/NlistMaker.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    65096 2022-12-19 08:32:59.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/NlistMaker.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      730 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/PairEnergy.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      570 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Random.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5106 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ShiftedLJ.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      764 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ShiftedLJ.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15360 2022-12-19 08:33:00.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ShiftedLJ.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      811 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Timer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2277 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Vector.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   698550 2022-12-19 08:33:00.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/libgriday.a
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      563 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/Makefile
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5834 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2022-12-19 08:33:06.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/grid2COTA
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   278928 2022-12-19 08:33:05.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/grid2props
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2022-12-19 08:33:04.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/grid2visit
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   161656 2022-12-19 08:33:03.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/grid_gen
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1046 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/main_cota.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1742 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      900 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/main_visit.cpp
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/moftransformer/modules/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      122 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/modules/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5783 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/modules/cgcnn.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3255 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/modules/heads.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11518 2023-04-27 06:22:20.000000 moftransformer-2.0.0/moftransformer/modules/module.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7374 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/modules/module_utils.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8004 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/modules/objectives.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12812 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/modules/vision_transformer_3d.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10096 2023-04-27 07:30:12.000000 moftransformer-2.0.0/moftransformer/run.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11715 2023-04-07 05:19:12.000000 moftransformer-2.0.0/moftransformer/run_cp.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/moftransformer/utils/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      242 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/utils/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5552 2023-04-27 04:54:01.000000 moftransformer-2.0.0/moftransformer/utils/download.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3913 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/utils/install_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16072 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/utils/prepare_data.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4355 2023-04-27 11:41:45.000000 moftransformer-2.0.0/moftransformer/utils/validation.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/moftransformer/visualize/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      130 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/visualize/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3994 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/visualize/drawer.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3705 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/visualize/setting.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9201 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/visualize/utils.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    27623 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/visualize/visualizer.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer.egg-info/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8153 2023-04-27 12:01:12.000000 moftransformer-2.0.0/moftransformer.egg-info/PKG-INFO
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13262 2023-04-27 12:01:12.000000 moftransformer-2.0.0/moftransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        1 2023-04-27 12:01:12.000000 moftransformer-2.0.0/moftransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       64 2023-04-27 12:01:12.000000 moftransformer-2.0.0/moftransformer.egg-info/entry_points.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      321 2023-04-27 12:01:12.000000 moftransformer-2.0.0/moftransformer.egg-info/requires.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       15 2023-04-27 12:01:12.000000 moftransformer-2.0.0/moftransformer.egg-info/top_level.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       38 2023-04-27 12:01:12.629117 moftransformer-2.0.0/setup.cfg
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1654 2023-04-27 05:16:55.000000 moftransformer-2.0.0/setup.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8991 2023-05-05 08:01:44.805183 moftransformer-2.0.1/PKG-INFO
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8612 2023-05-05 06:56:57.000000 moftransformer-2.0.1/README.md
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.797183 moftransformer-2.0.1/moftransformer/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      398 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/assets/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       72 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/assets/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12616 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/assets/bbs.json
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8140 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/assets/colors.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12647 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/assets/topology.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/cli/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       31 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/cli/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2443 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/cli/download.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      324 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/cli/install_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3040 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/cli/main.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      576 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/cli/run.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      328 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/cli/uninstall_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3425 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/config.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10515 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/config_ex.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/database/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      633 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/database/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/datamodules/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      210 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/datamodules/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2938 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/datamodules/datamodule.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10088 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/datamodules/dataset.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/examples/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      477 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/examples/raw/
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7496 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/acs+N270+E33.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    17441 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9738 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/fee+N254+E185.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11392 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/mok+N109+E146.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    30404 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18345 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/raw_example.json
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11939 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/sml+N696+E182.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    24953 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/smm+N577+E166.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    28256 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/ukg+N387+E203.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    39904 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/vmk+N489+E8.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18930 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/vna+N650+E120.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    48803 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/zzz+N96+N373+E34.cif
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.797183 moftransformer-2.0.1/moftransformer/examples/visualize/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9162 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12083 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6405 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8339 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7074 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9292 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    98728 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6419 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8357 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    93472 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6410 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8347 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6845 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8961 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   170530 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      164 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/gadgets/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       77 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/gadgets/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1806 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/gadgets/my_metrics.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.797183 moftransformer-2.0.1/moftransformer/libs/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/moftransformer/libs/GRIDAY/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2799 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/AtomTypeMap.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      654 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/AtomTypeMap.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2448 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Cell.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7789 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      414 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54588 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18619 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3812 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/EnergyGrid.hpp
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4751 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/UFF_FF.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      845 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/UFF_Type.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      202 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      190 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      318 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       26 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7197 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/ForceField.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      866 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/ForceField.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13991 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      865 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7362 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Framework.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1197 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Framework.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3007 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Gaussian.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Gaussian.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9534 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridMaker.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      936 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridMaker.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Griday.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      948 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridayException.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      669 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridayException.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      567 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridayTypes.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4380 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/LennardJones.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/LennardJones.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      334 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Makefile
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    21824 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/MaterialGrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2366 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/MaterialGrid.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5664 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/NlistMaker.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      922 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/NlistMaker.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      730 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/PairEnergy.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      570 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Random.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5106 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/ShiftedLJ.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      764 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/ShiftedLJ.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      811 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Timer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2277 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Vector.hpp
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      563 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/Makefile
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5834 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1046 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/main_cota.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1742 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      900 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/main_visit.cpp
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/moftransformer/modules/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      122 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5783 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/cgcnn.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3255 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/heads.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11518 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/module.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7374 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/module_utils.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8004 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/objectives.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12812 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/vision_transformer_3d.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10096 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/run.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/moftransformer/utils/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      242 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/utils/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5552 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/utils/download.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3913 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/utils/install_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16072 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/utils/prepare_data.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3567 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/utils/validation.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/moftransformer/visualize/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      130 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/visualize/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3994 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/visualize/drawer.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3705 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/visualize/setting.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9201 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/visualize/utils.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    27623 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/visualize/visualizer.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.797183 moftransformer-2.0.1/moftransformer.egg-info/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8991 2023-05-05 08:01:44.000000 moftransformer-2.0.1/moftransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     6064 2023-05-05 08:01:44.000000 moftransformer-2.0.1/moftransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        1 2023-05-05 08:01:44.000000 moftransformer-2.0.1/moftransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       64 2023-05-05 08:01:44.000000 moftransformer-2.0.1/moftransformer.egg-info/entry_points.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      313 2023-05-05 08:01:44.000000 moftransformer-2.0.1/moftransformer.egg-info/requires.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       15 2023-05-05 08:01:44.000000 moftransformer-2.0.1/moftransformer.egg-info/top_level.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       38 2023-05-05 08:01:44.805183 moftransformer-2.0.1/setup.cfg
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1524 2023-05-05 07:10:36.000000 moftransformer-2.0.1/setup.py
```

### Comparing `moftransformer-2.0.0/PKG-INFO` & `moftransformer-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: moftransformer
-Version: 2.0.0
+Version: 2.0.1
 Summary: moftransformer
 Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer
 Author: Yeonghun Kang, Hyunsoo Park
 Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.0.0-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.0.1-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.0.0-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.0.1-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
  <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
@@ -46,15 +46,15 @@
 
 ### Installation using PIP 
 ```
 $ pip install moftransformer
 ```
 
 ### Download the pretrained models (ckpt file)
-- you can download the pretrained models (`PMTransformer.ckpt` and `MOFTransformer.ckpt`) [figshare](https://figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2)
+- you can download the pretrained models (`PMTransformer.ckpt` and `MOFTransformer.ckpt`) via [figshare](https://figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2)
 
 or you can download with a command line:
 ```
 $ moftransformer download pretrain_model
 ```
 ### (Optional) Download pre-embeddings for CoREMOF, QMOF
 - we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database.
@@ -134,15 +134,15 @@
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/getting_started/assets/3.gif" width="400">
 </p>
 
 ## Universal Transfer Learning
 
-Comparison of mean absolute error (MAE) values for various baseline models, scratch, MOFTransformer, and PMTransformer on different properties of MOFs, COFs, PPNs, and zeolites. The bold values indicate the lowest MAE value for each property. The details of information can be found in [PMTransformer paper]()
+Comparison of mean absolute error (MAE) values for various baseline models, scratch, MOFTransformer, and PMTransformer on different properties of MOFs, COFs, PPNs, and zeolites. The bold values indicate the lowest MAE value for each property. The details of information can be found in [PMTransformer paper](https://chemrxiv.org/engage/chemrxiv/article-details/644a0651df78ec50157390c9)
 
 | Material | Property | Number of Dataset | Energy histogram | Descriptor-based ML | CGCNN | Scratch | MOFTransformer | PMTransformer |
 | --- | --- | --- | --- | --- | --- | --- | --- | --- |
 | MOF | H<sub>2</sub> Uptake (100 bar) | 20,000 | 9.183 | 9.456 | 32.864 | 7.018 | 6.377 | **5.963** |
 | MOF | H<sub>2</sub> diffusivity (dilute) | 20,000 | 0.644 | 0.398 | 0.6600 | 0.391 | 0.367 | 0.**366** |
 | MOF | Band-gap | 20.373 | 0.913 | 0.590 | 0.290 | 0.271 | 0.224 | **0.216** |
 | MOF | N<sub>2</sub> uptake (1 bar) | 5,286 | 0.178 | 0.115 | 0.108 | 0.102 | 0.071 | **0.069** |
@@ -156,7 +156,20 @@
 | COF | CO<sub>2</sub> heat of adsorption | 39,304 | 2.101 | 1.341 | 1.846 | 1.058 | 0.874 | **0.842** |
 | COF | CO<sub>2</sub> log KH | 39,304 | 0.242 | 0.169 | 0.238 | 0.134 | 0.108 | **0.103** |
 | PPN | CH<sub>4</sub> uptake (65bar) | 17,870 | 6.260 | 4.233 | 9.731 | 3.748 | 3.187 | **2.995** | 
 | PPN | CH<sub>4</sub> uptake (1bar) | 17,870  | 1.356	| 0.563	| 1.525	| 0.602	| 0.493	| **0.461** | 
 | Zeolite | CH<sub>4</sub>  KH (unitless) | 99,204	| 8.032	| 6.268	| 6.334	| 4.286	| 4.103	| **3.998** |
 | Zeolite | CH<sub>4</sub>  Heat of adsorption | 99,204	| 1.612	|1.033	| 1.603	| 0.670	| 0.647	|**0.639** |
 
+## Citation
+if you want to cite PMTransformer or MOFTransformer, please refer to the following paper:
+1. A multi-modal pre-training transformer for universal transfer learning in metal–organic frameworks, Nature Machine Intelligence, 5, 2023. [link](https://www.nature.com/articles/s42256-023-00628-2)
+
+2. PMTransformer: Universal Transfer Learning and Cross-material Few-shot Learning in Porous Materials, (submitted). [link](https://chemrxiv.org/engage/chemrxiv/article-details/644a0651df78ec50157390c9)
+
+## Contributing 🙌
+
+Contributions are welcome! If you have any suggestions or find any issues, please open an issue or a pull request.
+
+## License 📄
+
+This project is licensed under the MIT License. See the `LICENSE` file for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moftransformer Version: 2.0.0 Summary:
+Metadata-Version: 2.1 Name: moftransformer Version: 2.0.1 Summary:
 moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
 Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
 docs/source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
@@ -20,15 +20,15 @@
 porous materials as well as MOFs. The `PMTransformer` outperforms the
 `MOFTransformer` in predicting various properties of porous materials. ##
 [Install](https://hspark1212.github.io/MOFTransformer/installation.html) ###
 Depedencies ``` python>=3.8 ``` Given that MOFTransformer is based on pytorch,
 please install pytorch (>= 1.12.0) according to your environments. ###
 Installation using PIP ``` $ pip install moftransformer ``` ### Download the
 pretrained models (ckpt file) - you can download the pretrained models
-(`PMTransformer.ckpt` and `MOFTransformer.ckpt`) [figshare](https://
+(`PMTransformer.ckpt` and `MOFTransformer.ckpt`) via [figshare](https://
 figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2) or
 you can download with a command line: ``` $ moftransformer download
 pretrain_model ``` ### (Optional) Download pre-embeddings for CoREMOF, QMOF -
 we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-
 grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database. ``` $
 moftransformer download coremof $ moftransformer download qmof ``` ## [Getting
 Started](https://hspark1212.github.io/MOFTransformer/tutorial.html) 1. At
@@ -66,15 +66,16 @@
 vis.draw_grid() ```
    [https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/
                      source/getting_started/assets/3.gif]
 ## Universal Transfer Learning Comparison of mean absolute error (MAE) values
 for various baseline models, scratch, MOFTransformer, and PMTransformer on
 different properties of MOFs, COFs, PPNs, and zeolites. The bold values
 indicate the lowest MAE value for each property. The details of information can
-be found in [PMTransformer paper]() | Material | Property | Number of Dataset |
+be found in [PMTransformer paper](https://chemrxiv.org/engage/chemrxiv/article-
+details/644a0651df78ec50157390c9) | Material | Property | Number of Dataset |
 Energy histogram | Descriptor-based ML | CGCNN | Scratch | MOFTransformer |
 PMTransformer | | --- | --- | --- | --- | --- | --- | --- | --- | --- | | MOF |
 H2 Uptake (100 bar) | 20,000 | 9.183 | 9.456 | 32.864 | 7.018 | 6.377 |
 **5.963** | | MOF | H2 diffusivity (dilute) | 20,000 | 0.644 | 0.398 | 0.6600 |
 0.391 | 0.367 | 0.**366** | | MOF | Band-gap | 20.373 | 0.913 | 0.590 | 0.290 |
 0.271 | 0.224 | **0.216** | | MOF | N2 uptake (1 bar) | 5,286 | 0.178 | 0.115 |
 0.108 | 0.102 | 0.071 | **0.069** | | MOF | O2 uptake (1 bar) | 5,286 | 0.162 |
@@ -88,8 +89,18 @@
 (5.8bar) | 39,304 | 3.444 | 1.853 | 5.620 | 1.255 | **0.999** | 1.009 | | COF |
 CO2 heat of adsorption | 39,304 | 2.101 | 1.341 | 1.846 | 1.058 | 0.874 |
 **0.842** | | COF | CO2 log KH | 39,304 | 0.242 | 0.169 | 0.238 | 0.134 | 0.108
 | **0.103** | | PPN | CH4 uptake (65bar) | 17,870 | 6.260 | 4.233 | 9.731 |
 3.748 | 3.187 | **2.995** | | PPN | CH4 uptake (1bar) | 17,870 | 1.356 | 0.563
 | 1.525 | 0.602 | 0.493 | **0.461** | | Zeolite | CH4 KH (unitless) | 99,204 |
 8.032 | 6.268 | 6.334 | 4.286 | 4.103 | **3.998** | | Zeolite | CH4 Heat of
-adsorption | 99,204 | 1.612 |1.033 | 1.603 | 0.670 | 0.647 |**0.639** |
+adsorption | 99,204 | 1.612 |1.033 | 1.603 | 0.670 | 0.647 |**0.639** | ##
+Citation if you want to cite PMTransformer or MOFTransformer, please refer to
+the following paper: 1. A multi-modal pre-training transformer for universal
+transfer learning in metalâorganic frameworks, Nature Machine Intelligence,
+5, 2023. [link](https://www.nature.com/articles/s42256-023-00628-2) 2.
+PMTransformer: Universal Transfer Learning and Cross-material Few-shot Learning
+in Porous Materials, (submitted). [link](https://chemrxiv.org/engage/chemrxiv/
+article-details/644a0651df78ec50157390c9) ## Contributing ð Contributions
+are welcome! If you have any suggestions or find any issues, please open an
+issue or a pull request. ## License ð This project is licensed under the MIT
+License. See the `LICENSE` file for more information.
```

### Comparing `moftransformer-2.0.0/README.md` & `moftransformer-2.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.0.0-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.0.1-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.0.0-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.0.1-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
  <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
@@ -34,15 +34,15 @@
 
 ### Installation using PIP 
 ```
 $ pip install moftransformer
 ```
 
 ### Download the pretrained models (ckpt file)
-- you can download the pretrained models (`PMTransformer.ckpt` and `MOFTransformer.ckpt`) [figshare](https://figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2)
+- you can download the pretrained models (`PMTransformer.ckpt` and `MOFTransformer.ckpt`) via [figshare](https://figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2)
 
 or you can download with a command line:
 ```
 $ moftransformer download pretrain_model
 ```
 ### (Optional) Download pre-embeddings for CoREMOF, QMOF
 - we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database.
@@ -122,15 +122,15 @@
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/getting_started/assets/3.gif" width="400">
 </p>
 
 ## Universal Transfer Learning
 
-Comparison of mean absolute error (MAE) values for various baseline models, scratch, MOFTransformer, and PMTransformer on different properties of MOFs, COFs, PPNs, and zeolites. The bold values indicate the lowest MAE value for each property. The details of information can be found in [PMTransformer paper]()
+Comparison of mean absolute error (MAE) values for various baseline models, scratch, MOFTransformer, and PMTransformer on different properties of MOFs, COFs, PPNs, and zeolites. The bold values indicate the lowest MAE value for each property. The details of information can be found in [PMTransformer paper](https://chemrxiv.org/engage/chemrxiv/article-details/644a0651df78ec50157390c9)
 
 | Material | Property | Number of Dataset | Energy histogram | Descriptor-based ML | CGCNN | Scratch | MOFTransformer | PMTransformer |
 | --- | --- | --- | --- | --- | --- | --- | --- | --- |
 | MOF | H<sub>2</sub> Uptake (100 bar) | 20,000 | 9.183 | 9.456 | 32.864 | 7.018 | 6.377 | **5.963** |
 | MOF | H<sub>2</sub> diffusivity (dilute) | 20,000 | 0.644 | 0.398 | 0.6600 | 0.391 | 0.367 | 0.**366** |
 | MOF | Band-gap | 20.373 | 0.913 | 0.590 | 0.290 | 0.271 | 0.224 | **0.216** |
 | MOF | N<sub>2</sub> uptake (1 bar) | 5,286 | 0.178 | 0.115 | 0.108 | 0.102 | 0.071 | **0.069** |
@@ -144,7 +144,20 @@
 | COF | CO<sub>2</sub> heat of adsorption | 39,304 | 2.101 | 1.341 | 1.846 | 1.058 | 0.874 | **0.842** |
 | COF | CO<sub>2</sub> log KH | 39,304 | 0.242 | 0.169 | 0.238 | 0.134 | 0.108 | **0.103** |
 | PPN | CH<sub>4</sub> uptake (65bar) | 17,870 | 6.260 | 4.233 | 9.731 | 3.748 | 3.187 | **2.995** | 
 | PPN | CH<sub>4</sub> uptake (1bar) | 17,870  | 1.356	| 0.563	| 1.525	| 0.602	| 0.493	| **0.461** | 
 | Zeolite | CH<sub>4</sub>  KH (unitless) | 99,204	| 8.032	| 6.268	| 6.334	| 4.286	| 4.103	| **3.998** |
 | Zeolite | CH<sub>4</sub>  Heat of adsorption | 99,204	| 1.612	|1.033	| 1.603	| 0.670	| 0.647	|**0.639** |
 
+## Citation
+if you want to cite PMTransformer or MOFTransformer, please refer to the following paper:
+1. A multi-modal pre-training transformer for universal transfer learning in metal–organic frameworks, Nature Machine Intelligence, 5, 2023. [link](https://www.nature.com/articles/s42256-023-00628-2)
+
+2. PMTransformer: Universal Transfer Learning and Cross-material Few-shot Learning in Porous Materials, (submitted). [link](https://chemrxiv.org/engage/chemrxiv/article-details/644a0651df78ec50157390c9)
+
+## Contributing 🙌
+
+Contributions are welcome! If you have any suggestions or find any issues, please open an issue or a pull request.
+
+## License 📄
+
+This project is licensed under the MIT License. See the `LICENSE` file for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -15,15 +15,15 @@
 porous materials as well as MOFs. The `PMTransformer` outperforms the
 `MOFTransformer` in predicting various properties of porous materials. ##
 [Install](https://hspark1212.github.io/MOFTransformer/installation.html) ###
 Depedencies ``` python>=3.8 ``` Given that MOFTransformer is based on pytorch,
 please install pytorch (>= 1.12.0) according to your environments. ###
 Installation using PIP ``` $ pip install moftransformer ``` ### Download the
 pretrained models (ckpt file) - you can download the pretrained models
-(`PMTransformer.ckpt` and `MOFTransformer.ckpt`) [figshare](https://
+(`PMTransformer.ckpt` and `MOFTransformer.ckpt`) via [figshare](https://
 figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2) or
 you can download with a command line: ``` $ moftransformer download
 pretrain_model ``` ### (Optional) Download pre-embeddings for CoREMOF, QMOF -
 we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-
 grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database. ``` $
 moftransformer download coremof $ moftransformer download qmof ``` ## [Getting
 Started](https://hspark1212.github.io/MOFTransformer/tutorial.html) 1. At
@@ -61,15 +61,16 @@
 vis.draw_grid() ```
    [https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/
                      source/getting_started/assets/3.gif]
 ## Universal Transfer Learning Comparison of mean absolute error (MAE) values
 for various baseline models, scratch, MOFTransformer, and PMTransformer on
 different properties of MOFs, COFs, PPNs, and zeolites. The bold values
 indicate the lowest MAE value for each property. The details of information can
-be found in [PMTransformer paper]() | Material | Property | Number of Dataset |
+be found in [PMTransformer paper](https://chemrxiv.org/engage/chemrxiv/article-
+details/644a0651df78ec50157390c9) | Material | Property | Number of Dataset |
 Energy histogram | Descriptor-based ML | CGCNN | Scratch | MOFTransformer |
 PMTransformer | | --- | --- | --- | --- | --- | --- | --- | --- | --- | | MOF |
 H2 Uptake (100 bar) | 20,000 | 9.183 | 9.456 | 32.864 | 7.018 | 6.377 |
 **5.963** | | MOF | H2 diffusivity (dilute) | 20,000 | 0.644 | 0.398 | 0.6600 |
 0.391 | 0.367 | 0.**366** | | MOF | Band-gap | 20.373 | 0.913 | 0.590 | 0.290 |
 0.271 | 0.224 | **0.216** | | MOF | N2 uptake (1 bar) | 5,286 | 0.178 | 0.115 |
 0.108 | 0.102 | 0.071 | **0.069** | | MOF | O2 uptake (1 bar) | 5,286 | 0.162 |
@@ -83,8 +84,18 @@
 (5.8bar) | 39,304 | 3.444 | 1.853 | 5.620 | 1.255 | **0.999** | 1.009 | | COF |
 CO2 heat of adsorption | 39,304 | 2.101 | 1.341 | 1.846 | 1.058 | 0.874 |
 **0.842** | | COF | CO2 log KH | 39,304 | 0.242 | 0.169 | 0.238 | 0.134 | 0.108
 | **0.103** | | PPN | CH4 uptake (65bar) | 17,870 | 6.260 | 4.233 | 9.731 |
 3.748 | 3.187 | **2.995** | | PPN | CH4 uptake (1bar) | 17,870 | 1.356 | 0.563
 | 1.525 | 0.602 | 0.493 | **0.461** | | Zeolite | CH4 KH (unitless) | 99,204 |
 8.032 | 6.268 | 6.334 | 4.286 | 4.103 | **3.998** | | Zeolite | CH4 Heat of
-adsorption | 99,204 | 1.612 |1.033 | 1.603 | 0.670 | 0.647 |**0.639** |
+adsorption | 99,204 | 1.612 |1.033 | 1.603 | 0.670 | 0.647 |**0.639** | ##
+Citation if you want to cite PMTransformer or MOFTransformer, please refer to
+the following paper: 1. A multi-modal pre-training transformer for universal
+transfer learning in metalâorganic frameworks, Nature Machine Intelligence,
+5, 2023. [link](https://www.nature.com/articles/s42256-023-00628-2) 2.
+PMTransformer: Universal Transfer Learning and Cross-material Few-shot Learning
+in Porous Materials, (submitted). [link](https://chemrxiv.org/engage/chemrxiv/
+article-details/644a0651df78ec50157390c9) ## Contributing ð Contributions
+are welcome! If you have any suggestions or find any issues, please open an
+issue or a pull request. ## License ð This project is licensed under the MIT
+License. See the `LICENSE` file for more information.
```

### Comparing `moftransformer-2.0.0/moftransformer/assets/bbs.json` & `moftransformer-2.0.1/moftransformer/assets/bbs.json`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/assets/colors.py` & `moftransformer-2.0.1/moftransformer/assets/colors.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/assets/topology.json` & `moftransformer-2.0.1/moftransformer/assets/topology.json`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/cli/download.py` & `moftransformer-2.0.1/moftransformer/cli/download.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/cli/main.py` & `moftransformer-2.0.1/moftransformer/cli/main.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/cli/run.py` & `moftransformer-2.0.1/moftransformer/cli/run.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/config.py` & `moftransformer-2.0.1/moftransformer/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# MOFTransformer version 2.0.0
+# MOFTransformer version 2.0.1
 import os
 from sacred import Experiment
 from moftransformer import __root_dir__
 from moftransformer.utils.validation import _set_load_path, _loss_names
 
 ex = Experiment("pretrained_mof", save_git_info=False)
 
@@ -65,15 +65,15 @@
     resume_from = None
     val_check_interval = 1.0
     test_only = False
 
     # below params varies with the environment
     root_dataset = os.path.join(__root_dir__, "examples/dataset")
     log_dir = "logs/"
-    batch_size = 1024  # desired batch size; for gradient accumulation
+    batch_size = 32  # desired batch size; for gradient accumulation
     per_gpu_batchsize = 8  # you should define this manually with per_gpu_batch_size
     accelerator = "gpu"
     devices = 1
     num_nodes = 1
 
     load_path = _set_load_path('pmtransformer')
```

### Comparing `moftransformer-2.0.0/moftransformer/config_ex.py` & `moftransformer-2.0.1/moftransformer/config_ex.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/database/__init__.py` & `moftransformer-2.0.1/moftransformer/database/__init__.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/datamodules/datamodule.py` & `moftransformer-2.0.1/moftransformer/datamodules/datamodule.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/datamodules/dataset.py` & `moftransformer-2.0.1/moftransformer/datamodules/dataset.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/dataset/test/acs+N270+E33.cif` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 data_image0
-_chemical_formula_structural       C72Ga6H24O26
-_chemical_formula_sum              "C72 Ga6 H24 O26"
-_cell_length_a       22.242
-_cell_length_b       22.4662
-_cell_length_c       22.6575
-_cell_angle_alpha    90
-_cell_angle_beta     90
-_cell_angle_gamma    118.388
+_chemical_formula_structural       Zn8H30C48N6O26
+_chemical_formula_sum              "Zn8 H30 C48 N6 O26"
+_cell_length_a       18.3679
+_cell_length_b       18.2349
+_cell_length_c       18.387
+_cell_angle_alpha    60.5571
+_cell_angle_beta     60.8763
+_cell_angle_gamma    60.1754
 
 _space_group_name_H-M_alt    "P 1"
 _space_group_IT_number       1
 
 loop_
   _space_group_symop_operation_xyz
   'x, y, z'
@@ -19,135 +19,125 @@
   _atom_site_type_symbol
   _atom_site_label
   _atom_site_symmetry_multiplicity
   _atom_site_fract_x
   _atom_site_fract_y
   _atom_site_fract_z
   _atom_site_occupancy
-  C   C1        1.0  0.46099  0.76288  0.39553  1.0000
-  C   C2        1.0  0.46885  0.56983  0.39492  1.0000
-  C   C3        1.0  0.26887  0.56589  0.39516  1.0000
-  C   C4        1.0  0.26889  0.56595  0.23826  1.0000
-  C   C5        1.0  0.46843  0.56933  0.23848  1.0000
-  C   C6        1.0  0.46097  0.76294  0.23781  1.0000
-  C   C7        1.0  0.67192  0.16628  0.89554  1.0000
-  C   C8        1.0  0.66497  0.35998  0.89482  1.0000
-  C   C9        1.0  0.86412  0.36498  0.89545  1.0000
-  C   C10       1.0  0.86458  0.36343  0.73824  1.0000
-  C   C11       1.0  0.66324  0.35822  0.73822  1.0000
-  C   C12       1.0  0.67309  0.16690  0.73791  1.0000
-  C   C13       1.0  0.91608  0.39224  0.94103  1.0000
-  C   C14       1.0  0.95976  0.41280  0.97920  1.0000
-  C   C15       1.0  0.01255  0.43711  0.02476  1.0000
-  C   C16       1.0  0.06501  0.42009  0.02342  1.0000
-  C   C17       1.0  0.11859  0.44690  0.06444  1.0000
-  C   C18       1.0  0.12071  0.49084  0.10870  1.0000
-  C   C19       1.0  0.06811  0.50770  0.11016  1.0000
-  C   C20       1.0  0.01462  0.48102  0.06904  1.0000
-  C   C21       1.0  0.17512  0.51771  0.15286  1.0000
-  C   C22       1.0  0.21784  0.54024  0.19180  1.0000
-  C   C23       1.0  0.64766  0.11588  0.69140  1.0000
-  C   C24       1.0  0.62269  0.07317  0.65270  1.0000
-  C   C25       1.0  0.59525  0.01955  0.60787  1.0000
-  C   C26       1.0  0.54784  0.01528  0.56548  1.0000
-  C   C27       1.0  0.52002  0.96164  0.52491  1.0000
-  C   C28       1.0  0.53832  0.91048  0.52516  1.0000
-  C   C29       1.0  0.58578  0.91474  0.56748  1.0000
-  C   C30       1.0  0.61356  0.96836  0.60812  1.0000
-  C   C31       1.0  0.50938  0.85582  0.48140  1.0000
-  C   C32       1.0  0.48586  0.81346  0.44234  1.0000
-  C   C33       1.0  0.49260  0.54328  0.19125  1.0000
-  C   C34       1.0  0.51206  0.52055  0.15162  1.0000
-  C   C35       1.0  0.54055  0.49424  0.10756  1.0000
-  C   C36       1.0  0.50809  0.46915  0.05390  1.0000
-  C   C37       1.0  0.53385  0.44015  0.01342  1.0000
-  C   C38       1.0  0.59262  0.43546  0.02537  1.0000
-  C   C39       1.0  0.62564  0.46117  0.07885  1.0000
-  C   C40       1.0  0.59972  0.49009  0.11948  1.0000
-  C   C41       1.0  0.61926  0.40680  0.98174  1.0000
-  C   C42       1.0  0.64023  0.38552  0.94206  1.0000
-  C   C43       1.0  0.91504  0.38919  0.69133  1.0000
-  C   C44       1.0  0.95731  0.41159  0.65201  1.0000
-  C   C45       1.0  0.01223  0.43836  0.60834  1.0000
-  C   C46       1.0  0.00231  0.45449  0.55106  1.0000
-  C   C47       1.0  0.05597  0.48058  0.51012  1.0000
-  C   C48       1.0  0.12091  0.49093  0.52482  1.0000
-  C   C49       1.0  0.13093  0.47513  0.58220  1.0000
-  C   C50       1.0  0.07725  0.44905  0.62318  1.0000
-  C   C51       1.0  0.17570  0.51750  0.48102  1.0000
-  C   C52       1.0  0.21813  0.54052  0.44188  1.0000
-  C   C53       1.0  0.64575  0.11455  0.94120  1.0000
-  C   C54       1.0  0.62234  0.07122  0.97938  1.0000
-  C   C55       1.0  0.59487  0.01905  0.02525  1.0000
-  C   C56       1.0  0.52929  0.99570  0.04810  1.0000
-  C   C57       1.0  0.50168  0.94223  0.08879  1.0000
-  C   C58       1.0  0.53866  0.91067  0.10844  1.0000
-  C   C59       1.0  0.60445  0.93429  0.08587  1.0000
-  C   C60       1.0  0.63205  0.98775  0.04510  1.0000
-  C   C61       1.0  0.50968  0.85639  0.15247  1.0000
-  C   C62       1.0  0.48595  0.81379  0.19130  1.0000
-  C   C63       1.0  0.63684  0.38231  0.69121  1.0000
-  C   C64       1.0  0.61778  0.40572  0.65184  1.0000
-  C   C65       1.0  0.59307  0.43639  0.60848  1.0000
-  C   C66       1.0  0.56274  0.47498  0.62649  1.0000
-  C   C67       1.0  0.53676  0.50327  0.58537  1.0000
-  C   C68       1.0  0.54146  0.49430  0.52510  1.0000
-  C   C69       1.0  0.57195  0.45591  0.50721  1.0000
-  C   C70       1.0  0.59786  0.42762  0.54826  1.0000
-  C   C71       1.0  0.51498  0.52299  0.48141  1.0000
-  C   C72       1.0  0.49435  0.54482  0.44194  1.0000
-  Ga  Ga1       1.0  0.48345  0.67567  0.31652  1.0000
-  Ga  Ga2       1.0  0.36088  0.55065  0.31682  1.0000
-  Ga  Ga3       1.0  0.35519  0.67334  0.31669  1.0000
-  Ga  Ga4       1.0  0.65057  0.25384  0.81696  1.0000
-  Ga  Ga5       1.0  0.77217  0.37896  0.81602  1.0000
-  Ga  Ga6       1.0  0.77877  0.25627  0.81733  1.0000
-  H   H1        1.0  0.06524  0.38676  0.99005  1.0000
-  H   H2        1.0  0.15848  0.43359  0.06093  1.0000
-  H   H3        1.0  0.06860  0.54201  0.14287  1.0000
-  H   H4        1.0  0.97547  0.49545  0.07168  1.0000
-  H   H5        1.0  0.53146  0.05274  0.56362  1.0000
-  H   H6        1.0  0.48393  0.96001  0.49315  1.0000
-  H   H7        1.0  0.60172  0.87693  0.56956  1.0000
-  H   H8        1.0  0.64926  0.96970  0.64018  1.0000
-  H   H9        1.0  0.46202  0.47037  0.04350  1.0000
-  H   H10       1.0  0.50764  0.42110  0.97274  1.0000
-  H   H11       1.0  0.67125  0.45906  0.08956  1.0000
-  H   H12       1.0  0.62526  0.50821  0.16066  1.0000
-  H   H13       1.0  0.95326  0.44670  0.53746  1.0000
-  H   H14       1.0  0.04672  0.49271  0.46674  1.0000
-  H   H15       1.0  0.17997  0.48278  0.59576  1.0000
-  H   H16       1.0  0.08644  0.43678  0.66654  1.0000
-  H   H17       1.0  0.49866  0.01790  0.03420  1.0000
-  H   H18       1.0  0.45102  0.92518  0.10466  1.0000
-  H   H19       1.0  0.63473  0.91149  0.09920  1.0000
-  H   H20       1.0  0.68229  0.00413  0.02842  1.0000
-  H   H21       1.0  0.55850  0.48264  0.67244  1.0000
-  H   H22       1.0  0.51236  0.53116  0.60100  1.0000
-  H   H23       1.0  0.57493  0.44705  0.46135  1.0000
-  H   H24       1.0  0.62095  0.39855  0.53265  1.0000
-  O   O1        1.0  0.50402  0.74288  0.37362  1.0000
-  O   O2        1.0  0.40734  0.52855  0.37334  1.0000
-  O   O3        1.0  0.28768  0.62747  0.37379  1.0000
-  O   O4        1.0  0.29324  0.52620  0.25901  1.0000
-  O   O5        1.0  0.50828  0.63180  0.25854  1.0000
-  O   O6        1.0  0.39752  0.74020  0.25833  1.0000
-  O   O7        1.0  0.50400  0.74291  0.25961  1.0000
-  O   O8        1.0  0.40717  0.52841  0.26055  1.0000
-  O   O9        1.0  0.28771  0.62757  0.25959  1.0000
-  O   O10       1.0  0.29319  0.52610  0.37444  1.0000
-  O   O11       1.0  0.50829  0.63210  0.37444  1.0000
-  O   O12       1.0  0.39755  0.74017  0.37504  1.0000
-  O   O13       1.0  0.39999  0.63335  0.31665  1.0000
-  O   O14       1.0  0.62944  0.18683  0.87367  1.0000
-  O   O15       1.0  0.72607  0.40120  0.87260  1.0000
-  O   O16       1.0  0.84606  0.30321  0.87460  1.0000
-  O   O17       1.0  0.84018  0.40319  0.75881  1.0000
-  O   O18       1.0  0.62463  0.29607  0.75905  1.0000
-  O   O19       1.0  0.73652  0.18951  0.75854  1.0000
-  O   O20       1.0  0.63006  0.18669  0.76006  1.0000
-  O   O21       1.0  0.72474  0.40025  0.75950  1.0000
-  O   O22       1.0  0.84623  0.30197  0.75997  1.0000
-  O   O23       1.0  0.83924  0.40401  0.87416  1.0000
-  O   O24       1.0  0.62549  0.29753  0.87474  1.0000
-  O   O25       1.0  0.73555  0.18878  0.87539  1.0000
-  O   O26       1.0  0.73392  0.29628  0.81674  1.0000
+  Zn  Zn1       1.0  0.04456  0.84993  0.05181  1.0000
+  Zn  Zn2       1.0  0.04461  0.02865  0.04846  1.0000
+  Zn  Zn3       1.0  0.87206  0.02586  0.04810  1.0000
+  Zn  Zn4       1.0  0.04541  0.02317  0.87750  1.0000
+  Zn  Zn5       1.0  0.45929  0.61046  0.46844  1.0000
+  Zn  Zn6       1.0  0.45609  0.43666  0.46286  1.0000
+  Zn  Zn7       1.0  0.45831  0.44030  0.63304  1.0000
+  Zn  Zn8       1.0  0.63154  0.44025  0.46507  1.0000
+  H   H1        1.0  0.18851  0.66529  0.22701  1.0000
+  H   H2        1.0  0.28184  0.57392  0.32651  1.0000
+  H   H3        1.0  0.28468  0.89181  0.27896  1.0000
+  H   H4        1.0  0.33696  0.78911  0.34712  1.0000
+  H   H5        1.0  0.21090  0.90296  0.19688  1.0000
+  H   H6        1.0  0.91307  0.66129  0.19299  1.0000
+  H   H7        1.0  0.81210  0.57030  0.28887  1.0000
+  H   H8        1.0  0.54628  0.88873  0.29909  1.0000
+  H   H9        1.0  0.52726  0.78664  0.35244  1.0000
+  H   H10       1.0  0.68878  0.89925  0.22108  1.0000
+  H   H11       1.0  0.16988  0.66570  0.91140  1.0000
+  H   H12       1.0  0.27041  0.57405  0.81046  1.0000
+  H   H13       1.0  0.38864  0.85522  0.58658  1.0000
+  H   H14       1.0  0.42231  0.76272  0.55698  1.0000
+  H   H15       1.0  0.26500  0.88253  0.71340  1.0000
+  H   H16       1.0  0.68482  0.21950  0.17588  1.0000
+  H   H17       1.0  0.59231  0.31138  0.27664  1.0000
+  H   H18       1.0  0.89516  0.19760  0.34663  1.0000
+  H   H19       1.0  0.79426  0.27218  0.39341  1.0000
+  H   H20       1.0  0.91143  0.14540  0.24322  1.0000
+  H   H21       1.0  0.21613  0.16750  0.69035  1.0000
+  H   H22       1.0  0.31321  0.26261  0.59610  1.0000
+  H   H23       1.0  0.22878  0.31786  0.89685  1.0000
+  H   H24       1.0  0.30114  0.36363  0.79610  1.0000
+  H   H25       1.0  0.17422  0.21458  0.91692  1.0000
+  H   H26       1.0  0.91228  0.20471  0.69008  1.0000
+  H   H27       1.0  0.81052  0.30453  0.59886  1.0000
+  H   H28       1.0  0.55306  0.19783  0.89834  1.0000
+  H   H29       1.0  0.53187  0.27473  0.79856  1.0000
+  H   H30       1.0  0.69257  0.14155  0.91572  1.0000
+  C   C1        1.0  0.13954  0.84618  0.14635  1.0000
+  C   C2        1.0  0.19481  0.78975  0.20636  1.0000
+  C   C3        1.0  0.21420  0.69634  0.24262  1.0000
+  C   C4        1.0  0.26565  0.64628  0.29761  1.0000
+  C   C5        1.0  0.29867  0.68580  0.31905  1.0000
+  C   C6        1.0  0.35351  0.62653  0.37808  1.0000
+  C   C7        1.0  0.27870  0.78061  0.28253  1.0000
+  C   C8        1.0  0.22664  0.83055  0.22603  1.0000
+  C   C9        1.0  0.86351  0.84249  0.14518  1.0000
+  C   C10       1.0  0.80553  0.78589  0.20194  1.0000
+  C   C11       1.0  0.84205  0.69244  0.22054  1.0000
+  C   C12       1.0  0.78609  0.64263  0.27349  1.0000
+  C   C13       1.0  0.69391  0.68240  0.30921  1.0000
+  C   C14       1.0  0.63904  0.62408  0.36437  1.0000
+  C   C15       1.0  0.65705  0.77712  0.29070  1.0000
+  C   C16       1.0  0.71505  0.82683  0.23643  1.0000
+  C   C17       1.0  0.14939  0.83785  0.87332  1.0000
+  C   C18       1.0  0.21227  0.77961  0.81695  1.0000
+  C   C19       1.0  0.21343  0.69181  0.84644  1.0000
+  C   C20       1.0  0.26902  0.64162  0.79051  1.0000
+  C   C21       1.0  0.32477  0.67543  0.70575  1.0000
+  C   C22       1.0  0.37897  0.61804  0.64972  1.0000
+  C   C23       1.0  0.32566  0.76347  0.67691  1.0000
+  C   C24       1.0  0.26760  0.81416  0.73445  1.0000
+  C   C25       1.0  0.86157  0.12294  0.14366  1.0000
+  C   C26       1.0  0.80389  0.17748  0.20412  1.0000
+  C   C27       1.0  0.71316  0.22365  0.21316  1.0000
+  C   C28       1.0  0.66240  0.27408  0.26903  1.0000
+  C   C29       1.0  0.69836  0.28046  0.31740  1.0000
+  C   C30       1.0  0.63963  0.33793  0.37361  1.0000
+  C   C31       1.0  0.79011  0.23226  0.30943  1.0000
+  C   C32       1.0  0.84106  0.18186  0.25137  1.0000
+  C   C33       1.0  0.13345  0.12794  0.86750  1.0000
+  C   C34       1.0  0.19004  0.18592  0.80941  1.0000
+  C   C35       1.0  0.22862  0.19910  0.71824  1.0000
+  C   C36       1.0  0.28191  0.25171  0.66665  1.0000
+  C   C37       1.0  0.29825  0.29314  0.70219  1.0000
+  C   C38       1.0  0.35630  0.34802  0.64255  1.0000
+  C   C39       1.0  0.25810  0.28076  0.79450  1.0000
+  C   C40       1.0  0.20462  0.22611  0.84617  1.0000
+  C   C41       1.0  0.86500  0.11087  0.86568  1.0000
+  C   C42       1.0  0.80711  0.16765  0.80837  1.0000
+  C   C43       1.0  0.84226  0.21268  0.71827  1.0000
+  C   C44       1.0  0.78584  0.26743  0.66831  1.0000
+  C   C45       1.0  0.69484  0.27851  0.70431  1.0000
+  C   C46       1.0  0.63957  0.33930  0.64618  1.0000
+  C   C47       1.0  0.65962  0.23125  0.79535  1.0000
+  C   C48       1.0  0.71802  0.17682  0.84568  1.0000
+  N   N1        1.0  0.30977  0.82425  0.29789  1.0000
+  N   N2        1.0  0.56896  0.82124  0.32519  1.0000
+  N   N3        1.0  0.37887  0.80066  0.59664  1.0000
+  N   N4        1.0  0.82986  0.23189  0.35572  1.0000
+  N   N5        1.0  0.27028  0.31738  0.83541  1.0000
+  N   N6        1.0  0.57308  0.23701  0.83543  1.0000
+  O   O1        1.0  0.00197  0.98138  0.00675  1.0000
+  O   O2        1.0  0.12317  0.93061  0.11727  1.0000
+  O   O3        1.0  0.11332  0.80523  0.12907  1.0000
+  O   O4        1.0  0.37681  0.54214  0.39811  1.0000
+  O   O5        1.0  0.37441  0.66405  0.40601  1.0000
+  O   O6        1.0  0.82485  0.92711  0.12736  1.0000
+  O   O7        1.0  0.94683  0.80167  0.11943  1.0000
+  O   O8        1.0  0.67834  0.53926  0.38448  1.0000
+  O   O9        1.0  0.55413  0.66243  0.38888  1.0000
+  O   O10       1.0  0.13162  0.92215  0.83409  1.0000
+  O   O11       1.0  0.11823  0.79867  0.95561  1.0000
+  O   O12       1.0  0.38699  0.53508  0.68648  1.0000
+  O   O13       1.0  0.41459  0.65453  0.56660  1.0000
+  O   O14       1.0  0.82271  0.10873  0.11250  1.0000
+  O   O15       1.0  0.94511  0.09476  0.12810  1.0000
+  O   O16       1.0  0.67574  0.35095  0.40955  1.0000
+  O   O17       1.0  0.55687  0.37183  0.38301  1.0000
+  O   O18       1.0  0.11337  0.10198  0.82883  1.0000
+  O   O19       1.0  0.10993  0.10892  0.95081  1.0000
+  O   O20       1.0  0.37129  0.38338  0.67757  1.0000
+  O   O21       1.0  0.38843  0.35776  0.56028  1.0000
+  O   O22       1.0  0.94856  0.09121  0.82693  1.0000
+  O   O23       1.0  0.82600  0.08707  0.94885  1.0000
+  O   O24       1.0  0.55571  0.35130  0.68061  1.0000
+  O   O25       1.0  0.67715  0.37725  0.56509  1.0000
+  O   O26       1.0  0.50195  0.48102  0.50486  1.0000
```

### Comparing `moftransformer-2.0.0/moftransformer/examples/dataset/total/acs+N270+E33.cif` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 data_image0
-_chemical_formula_structural       C72Ga6H24O26
-_chemical_formula_sum              "C72 Ga6 H24 O26"
-_cell_length_a       22.242
-_cell_length_b       22.4662
-_cell_length_c       22.6575
-_cell_angle_alpha    90
-_cell_angle_beta     90
-_cell_angle_gamma    118.388
+_chemical_formula_structural       Zr6H28C48O32
+_chemical_formula_sum              "Zr6 H28 C48 O32"
+_cell_length_a       14.7734
+_cell_length_b       14.7734
+_cell_length_c       14.7735
+_cell_angle_alpha    59.9994
+_cell_angle_beta     60
+_cell_angle_gamma    60.0001
 
 _space_group_name_H-M_alt    "P 1"
 _space_group_IT_number       1
 
 loop_
   _space_group_symop_operation_xyz
   'x, y, z'
@@ -19,135 +19,121 @@
   _atom_site_type_symbol
   _atom_site_label
   _atom_site_symmetry_multiplicity
   _atom_site_fract_x
   _atom_site_fract_y
   _atom_site_fract_z
   _atom_site_occupancy
-  C   C1        1.0  0.46099  0.76288  0.39553  1.0000
-  C   C2        1.0  0.46885  0.56983  0.39492  1.0000
-  C   C3        1.0  0.26887  0.56589  0.39516  1.0000
-  C   C4        1.0  0.26889  0.56595  0.23826  1.0000
-  C   C5        1.0  0.46843  0.56933  0.23848  1.0000
-  C   C6        1.0  0.46097  0.76294  0.23781  1.0000
-  C   C7        1.0  0.67192  0.16628  0.89554  1.0000
-  C   C8        1.0  0.66497  0.35998  0.89482  1.0000
-  C   C9        1.0  0.86412  0.36498  0.89545  1.0000
-  C   C10       1.0  0.86458  0.36343  0.73824  1.0000
-  C   C11       1.0  0.66324  0.35822  0.73822  1.0000
-  C   C12       1.0  0.67309  0.16690  0.73791  1.0000
-  C   C13       1.0  0.91608  0.39224  0.94103  1.0000
-  C   C14       1.0  0.95976  0.41280  0.97920  1.0000
-  C   C15       1.0  0.01255  0.43711  0.02476  1.0000
-  C   C16       1.0  0.06501  0.42009  0.02342  1.0000
-  C   C17       1.0  0.11859  0.44690  0.06444  1.0000
-  C   C18       1.0  0.12071  0.49084  0.10870  1.0000
-  C   C19       1.0  0.06811  0.50770  0.11016  1.0000
-  C   C20       1.0  0.01462  0.48102  0.06904  1.0000
-  C   C21       1.0  0.17512  0.51771  0.15286  1.0000
-  C   C22       1.0  0.21784  0.54024  0.19180  1.0000
-  C   C23       1.0  0.64766  0.11588  0.69140  1.0000
-  C   C24       1.0  0.62269  0.07317  0.65270  1.0000
-  C   C25       1.0  0.59525  0.01955  0.60787  1.0000
-  C   C26       1.0  0.54784  0.01528  0.56548  1.0000
-  C   C27       1.0  0.52002  0.96164  0.52491  1.0000
-  C   C28       1.0  0.53832  0.91048  0.52516  1.0000
-  C   C29       1.0  0.58578  0.91474  0.56748  1.0000
-  C   C30       1.0  0.61356  0.96836  0.60812  1.0000
-  C   C31       1.0  0.50938  0.85582  0.48140  1.0000
-  C   C32       1.0  0.48586  0.81346  0.44234  1.0000
-  C   C33       1.0  0.49260  0.54328  0.19125  1.0000
-  C   C34       1.0  0.51206  0.52055  0.15162  1.0000
-  C   C35       1.0  0.54055  0.49424  0.10756  1.0000
-  C   C36       1.0  0.50809  0.46915  0.05390  1.0000
-  C   C37       1.0  0.53385  0.44015  0.01342  1.0000
-  C   C38       1.0  0.59262  0.43546  0.02537  1.0000
-  C   C39       1.0  0.62564  0.46117  0.07885  1.0000
-  C   C40       1.0  0.59972  0.49009  0.11948  1.0000
-  C   C41       1.0  0.61926  0.40680  0.98174  1.0000
-  C   C42       1.0  0.64023  0.38552  0.94206  1.0000
-  C   C43       1.0  0.91504  0.38919  0.69133  1.0000
-  C   C44       1.0  0.95731  0.41159  0.65201  1.0000
-  C   C45       1.0  0.01223  0.43836  0.60834  1.0000
-  C   C46       1.0  0.00231  0.45449  0.55106  1.0000
-  C   C47       1.0  0.05597  0.48058  0.51012  1.0000
-  C   C48       1.0  0.12091  0.49093  0.52482  1.0000
-  C   C49       1.0  0.13093  0.47513  0.58220  1.0000
-  C   C50       1.0  0.07725  0.44905  0.62318  1.0000
-  C   C51       1.0  0.17570  0.51750  0.48102  1.0000
-  C   C52       1.0  0.21813  0.54052  0.44188  1.0000
-  C   C53       1.0  0.64575  0.11455  0.94120  1.0000
-  C   C54       1.0  0.62234  0.07122  0.97938  1.0000
-  C   C55       1.0  0.59487  0.01905  0.02525  1.0000
-  C   C56       1.0  0.52929  0.99570  0.04810  1.0000
-  C   C57       1.0  0.50168  0.94223  0.08879  1.0000
-  C   C58       1.0  0.53866  0.91067  0.10844  1.0000
-  C   C59       1.0  0.60445  0.93429  0.08587  1.0000
-  C   C60       1.0  0.63205  0.98775  0.04510  1.0000
-  C   C61       1.0  0.50968  0.85639  0.15247  1.0000
-  C   C62       1.0  0.48595  0.81379  0.19130  1.0000
-  C   C63       1.0  0.63684  0.38231  0.69121  1.0000
-  C   C64       1.0  0.61778  0.40572  0.65184  1.0000
-  C   C65       1.0  0.59307  0.43639  0.60848  1.0000
-  C   C66       1.0  0.56274  0.47498  0.62649  1.0000
-  C   C67       1.0  0.53676  0.50327  0.58537  1.0000
-  C   C68       1.0  0.54146  0.49430  0.52510  1.0000
-  C   C69       1.0  0.57195  0.45591  0.50721  1.0000
-  C   C70       1.0  0.59786  0.42762  0.54826  1.0000
-  C   C71       1.0  0.51498  0.52299  0.48141  1.0000
-  C   C72       1.0  0.49435  0.54482  0.44194  1.0000
-  Ga  Ga1       1.0  0.48345  0.67567  0.31652  1.0000
-  Ga  Ga2       1.0  0.36088  0.55065  0.31682  1.0000
-  Ga  Ga3       1.0  0.35519  0.67334  0.31669  1.0000
-  Ga  Ga4       1.0  0.65057  0.25384  0.81696  1.0000
-  Ga  Ga5       1.0  0.77217  0.37896  0.81602  1.0000
-  Ga  Ga6       1.0  0.77877  0.25627  0.81733  1.0000
-  H   H1        1.0  0.06524  0.38676  0.99005  1.0000
-  H   H2        1.0  0.15848  0.43359  0.06093  1.0000
-  H   H3        1.0  0.06860  0.54201  0.14287  1.0000
-  H   H4        1.0  0.97547  0.49545  0.07168  1.0000
-  H   H5        1.0  0.53146  0.05274  0.56362  1.0000
-  H   H6        1.0  0.48393  0.96001  0.49315  1.0000
-  H   H7        1.0  0.60172  0.87693  0.56956  1.0000
-  H   H8        1.0  0.64926  0.96970  0.64018  1.0000
-  H   H9        1.0  0.46202  0.47037  0.04350  1.0000
-  H   H10       1.0  0.50764  0.42110  0.97274  1.0000
-  H   H11       1.0  0.67125  0.45906  0.08956  1.0000
-  H   H12       1.0  0.62526  0.50821  0.16066  1.0000
-  H   H13       1.0  0.95326  0.44670  0.53746  1.0000
-  H   H14       1.0  0.04672  0.49271  0.46674  1.0000
-  H   H15       1.0  0.17997  0.48278  0.59576  1.0000
-  H   H16       1.0  0.08644  0.43678  0.66654  1.0000
-  H   H17       1.0  0.49866  0.01790  0.03420  1.0000
-  H   H18       1.0  0.45102  0.92518  0.10466  1.0000
-  H   H19       1.0  0.63473  0.91149  0.09920  1.0000
-  H   H20       1.0  0.68229  0.00413  0.02842  1.0000
-  H   H21       1.0  0.55850  0.48264  0.67244  1.0000
-  H   H22       1.0  0.51236  0.53116  0.60100  1.0000
-  H   H23       1.0  0.57493  0.44705  0.46135  1.0000
-  H   H24       1.0  0.62095  0.39855  0.53265  1.0000
-  O   O1        1.0  0.50402  0.74288  0.37362  1.0000
-  O   O2        1.0  0.40734  0.52855  0.37334  1.0000
-  O   O3        1.0  0.28768  0.62747  0.37379  1.0000
-  O   O4        1.0  0.29324  0.52620  0.25901  1.0000
-  O   O5        1.0  0.50828  0.63180  0.25854  1.0000
-  O   O6        1.0  0.39752  0.74020  0.25833  1.0000
-  O   O7        1.0  0.50400  0.74291  0.25961  1.0000
-  O   O8        1.0  0.40717  0.52841  0.26055  1.0000
-  O   O9        1.0  0.28771  0.62757  0.25959  1.0000
-  O   O10       1.0  0.29319  0.52610  0.37444  1.0000
-  O   O11       1.0  0.50829  0.63210  0.37444  1.0000
-  O   O12       1.0  0.39755  0.74017  0.37504  1.0000
-  O   O13       1.0  0.39999  0.63335  0.31665  1.0000
-  O   O14       1.0  0.62944  0.18683  0.87367  1.0000
-  O   O15       1.0  0.72607  0.40120  0.87260  1.0000
-  O   O16       1.0  0.84606  0.30321  0.87460  1.0000
-  O   O17       1.0  0.84018  0.40319  0.75881  1.0000
-  O   O18       1.0  0.62463  0.29607  0.75905  1.0000
-  O   O19       1.0  0.73652  0.18951  0.75854  1.0000
-  O   O20       1.0  0.63006  0.18669  0.76006  1.0000
-  O   O21       1.0  0.72474  0.40025  0.75950  1.0000
-  O   O22       1.0  0.84623  0.30197  0.75997  1.0000
-  O   O23       1.0  0.83924  0.40401  0.87416  1.0000
-  O   O24       1.0  0.62549  0.29753  0.87474  1.0000
-  O   O25       1.0  0.73555  0.18878  0.87539  1.0000
-  O   O26       1.0  0.73392  0.29628  0.81674  1.0000
+  Zr  Zr1       1.0  0.88033  0.88033  0.61967  1.0000
+  Zr  Zr2       1.0  0.11967  0.11967  0.38033  1.0000
+  Zr  Zr3       1.0  0.11968  0.88032  0.61968  1.0000
+  Zr  Zr4       1.0  0.88032  0.11968  0.38032  1.0000
+  Zr  Zr5       1.0  0.11969  0.88031  0.38031  1.0000
+  Zr  Zr6       1.0  0.88031  0.11968  0.61969  1.0000
+  H   H1        1.0  0.09416  0.71751  0.59416  1.0000
+  H   H2        1.0  0.09417  0.09416  0.21751  1.0000
+  H   H3        1.0  0.09416  0.09416  0.59416  1.0000
+  H   H4        1.0  0.71752  0.09416  0.59416  1.0000
+  H   H5        1.0  0.14415  0.41584  0.35362  1.0000
+  H   H6        1.0  0.85362  0.58639  0.64414  1.0000
+  H   H7        1.0  0.14415  0.58640  0.35362  1.0000
+  H   H8        1.0  0.85362  0.41583  0.64415  1.0000
+  H   H9        1.0  0.41584  0.14414  0.08639  1.0000
+  H   H10       1.0  0.58640  0.85362  0.91584  1.0000
+  H   H11       1.0  0.58640  0.14415  0.91583  1.0000
+  H   H12       1.0  0.41584  0.85362  0.08640  1.0000
+  H   H13       1.0  0.85362  0.14415  0.91583  1.0000
+  H   H14       1.0  0.14414  0.85362  0.08640  1.0000
+  H   H15       1.0  0.85362  0.14415  0.08639  1.0000
+  H   H16       1.0  0.14414  0.85362  0.91584  1.0000
+  H   H17       1.0  0.41584  0.58640  0.35361  1.0000
+  H   H18       1.0  0.58640  0.41584  0.64415  1.0000
+  H   H19       1.0  0.58640  0.41584  0.35362  1.0000
+  H   H20       1.0  0.41584  0.58640  0.64414  1.0000
+  H   H21       1.0  0.85362  0.41583  0.08640  1.0000
+  H   H22       1.0  0.14415  0.58640  0.91583  1.0000
+  H   H23       1.0  0.85362  0.58640  0.91584  1.0000
+  H   H24       1.0  0.14415  0.41584  0.08640  1.0000
+  H   H25       1.0  0.41584  0.85362  0.64415  1.0000
+  H   H26       1.0  0.58640  0.14415  0.35361  1.0000
+  H   H27       1.0  0.58640  0.85362  0.64415  1.0000
+  H   H28       1.0  0.41584  0.14414  0.35362  1.0000
+  C   C1        1.0  0.99754  0.69815  0.49751  1.0000
+  C   C2        1.0  0.30680  0.99750  0.19816  1.0000
+  C   C3        1.0  0.99752  0.30680  0.49754  1.0000
+  C   C4        1.0  0.69816  0.99754  0.80680  1.0000
+  C   C5        1.0  0.99754  0.69816  0.80680  1.0000
+  C   C6        1.0  0.69816  0.99753  0.49751  1.0000
+  C   C7        1.0  0.99752  0.30680  0.19815  1.0000
+  C   C8        1.0  0.30679  0.99751  0.49754  1.0000
+  C   C9        1.0  0.30681  0.69815  0.49752  1.0000
+  C   C10       1.0  0.99752  0.99753  0.80680  1.0000
+  C   C11       1.0  0.69815  0.30681  0.49753  1.0000
+  C   C12       1.0  0.99753  0.99752  0.19815  1.0000
+  C   C13       1.0  0.99829  0.40717  0.49827  1.0000
+  C   C14       1.0  0.99827  0.59628  0.49828  1.0000
+  C   C15       1.0  0.08094  0.45423  0.41649  1.0000
+  C   C16       1.0  0.91649  0.54833  0.58094  1.0000
+  C   C17       1.0  0.08094  0.54833  0.41648  1.0000
+  C   C18       1.0  0.91649  0.45424  0.58094  1.0000
+  C   C19       1.0  0.40717  0.99828  0.09627  1.0000
+  C   C20       1.0  0.59628  0.99827  0.90717  1.0000
+  C   C21       1.0  0.45423  0.08094  0.04833  1.0000
+  C   C22       1.0  0.54834  0.91649  0.95423  1.0000
+  C   C23       1.0  0.54834  0.08094  0.95424  1.0000
+  C   C24       1.0  0.45424  0.91649  0.04833  1.0000
+  C   C25       1.0  0.99828  0.99827  0.90718  1.0000
+  C   C26       1.0  0.99827  0.99828  0.09627  1.0000
+  C   C27       1.0  0.91649  0.08094  0.95423  1.0000
+  C   C28       1.0  0.08094  0.91649  0.04833  1.0000
+  C   C29       1.0  0.91649  0.08094  0.04833  1.0000
+  C   C30       1.0  0.08094  0.91649  0.95423  1.0000
+  C   C31       1.0  0.40717  0.59627  0.49828  1.0000
+  C   C32       1.0  0.59628  0.40717  0.49827  1.0000
+  C   C33       1.0  0.45425  0.54833  0.41649  1.0000
+  C   C34       1.0  0.54834  0.45424  0.58093  1.0000
+  C   C35       1.0  0.54834  0.45424  0.41649  1.0000
+  C   C36       1.0  0.45424  0.54834  0.58094  1.0000
+  C   C37       1.0  0.99829  0.40716  0.09628  1.0000
+  C   C38       1.0  0.99827  0.59628  0.90717  1.0000
+  C   C39       1.0  0.91649  0.45424  0.04834  1.0000
+  C   C40       1.0  0.08094  0.54834  0.95424  1.0000
+  C   C41       1.0  0.91649  0.54833  0.95424  1.0000
+  C   C42       1.0  0.08094  0.45424  0.04834  1.0000
+  C   C43       1.0  0.40717  0.99829  0.49827  1.0000
+  C   C44       1.0  0.59628  0.99827  0.49828  1.0000
+  C   C45       1.0  0.45424  0.91649  0.58094  1.0000
+  C   C46       1.0  0.54834  0.08094  0.41648  1.0000
+  C   C47       1.0  0.54834  0.91649  0.58094  1.0000
+  C   C48       1.0  0.45424  0.08094  0.41649  1.0000
+  O   O1        1.0  0.92066  0.73771  0.57454  1.0000
+  O   O2        1.0  0.26709  0.07454  0.23771  1.0000
+  O   O3        1.0  0.07455  0.26708  0.42066  1.0000
+  O   O4        1.0  0.73771  0.92066  0.76709  1.0000
+  O   O5        1.0  0.07456  0.73770  0.76710  1.0000
+  O   O6        1.0  0.73770  0.07456  0.42065  1.0000
+  O   O7        1.0  0.92065  0.26709  0.23769  1.0000
+  O   O8        1.0  0.26710  0.92064  0.57456  1.0000
+  O   O9        1.0  0.26710  0.73769  0.42065  1.0000
+  O   O10       1.0  0.92065  0.07456  0.76710  1.0000
+  O   O11       1.0  0.73769  0.26711  0.57456  1.0000
+  O   O12       1.0  0.07456  0.92065  0.23769  1.0000
+  O   O13       1.0  0.07456  0.92065  0.76710  1.0000
+  O   O14       1.0  0.73770  0.26710  0.42066  1.0000
+  O   O15       1.0  0.92065  0.07456  0.23770  1.0000
+  O   O16       1.0  0.26710  0.73769  0.57455  1.0000
+  O   O17       1.0  0.92066  0.73771  0.76708  1.0000
+  O   O18       1.0  0.26708  0.07454  0.42066  1.0000
+  O   O19       1.0  0.07455  0.26709  0.23770  1.0000
+  O   O20       1.0  0.73771  0.92066  0.57454  1.0000
+  O   O21       1.0  0.73770  0.07457  0.76710  1.0000
+  O   O22       1.0  0.07457  0.73769  0.42064  1.0000
+  O   O23       1.0  0.26710  0.92064  0.23769  1.0000
+  O   O24       1.0  0.92065  0.26710  0.57457  1.0000
+  O   O25       1.0  0.79786  0.06738  0.56738  1.0000
+  O   O26       1.0  0.06738  0.06739  0.56738  1.0000
+  O   O27       1.0  0.06738  0.06738  0.29786  1.0000
+  O   O28       1.0  0.06738  0.79786  0.56738  1.0000
+  O   O29       1.0  0.14878  0.95040  0.45040  1.0000
+  O   O30       1.0  0.95042  0.95041  0.45040  1.0000
+  O   O31       1.0  0.95039  0.14878  0.45042  1.0000
+  O   O32       1.0  0.95040  0.95042  0.64878  1.0000
```

### Comparing `moftransformer-2.0.0/moftransformer/examples/dataset/total/fee+N254+E185.cif` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 data_image0
-_chemical_formula_structural       Br40C80Cd8O40
-_chemical_formula_sum              "Br40 C80 Cd8 O40"
-_cell_length_a       14.5896
-_cell_length_b       24.7263
-_cell_length_c       24.8436
-_cell_angle_alpha    76.571
-_cell_angle_beta     84.249
-_cell_angle_gamma    89.853
+_chemical_formula_structural       Cu12H24C72O48
+_chemical_formula_sum              "Cu12 H24 C72 O48"
+_cell_length_a       18.7231
+_cell_length_b       18.7189
+_cell_length_c       18.7168
+_cell_angle_alpha    60.0188
+_cell_angle_beta     60.0035
+_cell_angle_gamma    59.9851
 
 _space_group_name_H-M_alt    "P 1"
 _space_group_IT_number       1
 
 loop_
   _space_group_symop_operation_xyz
   'x, y, z'
@@ -19,175 +19,163 @@
   _atom_site_type_symbol
   _atom_site_label
   _atom_site_symmetry_multiplicity
   _atom_site_fract_x
   _atom_site_fract_y
   _atom_site_fract_z
   _atom_site_occupancy
-  Br  Br1       1.0  0.33932  0.28668  0.47336  1.0000
-  Br  Br2       1.0  0.56258  0.29340  0.48206  1.0000
-  Br  Br3       1.0  0.30505  0.09740  0.66400  1.0000
-  Br  Br4       1.0  0.53146  0.09285  0.66014  1.0000
-  Br  Br5       1.0  0.55570  0.61022  0.79250  1.0000
-  Br  Br6       1.0  0.32926  0.60910  0.79776  1.0000
-  Br  Br7       1.0  0.55628  0.37730  0.78320  1.0000
-  Br  Br8       1.0  0.33446  0.38256  0.76798  1.0000
-  Br  Br9       1.0  0.34490  0.71854  0.39224  1.0000
-  Br  Br10      1.0  0.57048  0.71506  0.39718  1.0000
-  Br  Br11      1.0  0.34316  0.94174  0.43054  1.0000
-  Br  Br12      1.0  0.56966  0.93856  0.43220  1.0000
-  Br  Br13      1.0  0.34054  0.41808  0.19198  1.0000
-  Br  Br14      1.0  0.56632  0.42002  0.18942  1.0000
-  Br  Br15      1.0  0.33536  0.65014  0.20540  1.0000
-  Br  Br16      1.0  0.55696  0.64524  0.22188  1.0000
-  Br  Br17      1.0  0.99981  0.02427  0.36056  1.0000
-  Br  Br18      1.0  0.97981  0.13462  0.41538  1.0000
-  Br  Br19      1.0  0.87052  0.88260  0.57432  1.0000
-  Br  Br20      1.0  0.87416  0.99100  0.63274  1.0000
-  Br  Br21      1.0  0.99626  0.62170  0.89346  1.0000
-  Br  Br22      1.0  0.02054  0.62392  0.02454  1.0000
-  Br  Br23      1.0  0.86598  0.39208  0.96584  1.0000
-  Br  Br24      1.0  0.88440  0.39638  0.09746  1.0000
-  Br  Br25      1.0  0.85064  0.29266  0.84368  1.0000
-  Br  Br26      1.0  0.83437  0.19100  0.77592  1.0000
-  Br  Br27      1.0  0.04708  0.43132  0.64432  1.0000
-  Br  Br28      1.0  0.04016  0.32946  0.58184  1.0000
-  Br  Br29      1.0  0.06300  0.78220  0.59366  1.0000
-  Br  Br30      1.0  0.06474  0.68044  0.70712  1.0000
-  Br  Br31      1.0  0.83984  0.64280  0.49657  1.0000
-  Br  Br32      1.0  0.84298  0.54129  0.61010  1.0000
-  Br  Br33      1.0  0.04870  0.58894  0.32022  1.0000
-  Br  Br34      1.0  0.07452  0.69116  0.38196  1.0000
-  Br  Br35      1.0  0.86514  0.73500  0.14894  1.0000
-  Br  Br36      1.0  0.88198  0.83850  0.21476  1.0000
-  Br  Br37      1.0  0.81062  0.46894  0.38858  1.0000
-  Br  Br38      1.0  0.81456  0.36644  0.50026  1.0000
-  Br  Br39      1.0  0.08371  0.35682  0.26864  1.0000
-  Br  Br40      1.0  0.10450  0.26232  0.38422  1.0000
-  C   C1        1.0  0.63606  0.19259  0.57068  1.0000
-  C   C2        1.0  0.92564  0.22666  0.65248  1.0000
-  C   C3        1.0  0.23304  0.19222  0.56820  1.0000
-  C   C4        1.0  0.94686  0.27054  0.48026  1.0000
-  C   C5        1.0  0.93642  0.10160  0.54496  1.0000
-  C   C6        1.0  0.64440  0.49320  0.78878  1.0000
-  C   C7        1.0  0.95134  0.57508  0.70038  1.0000
-  C   C8        1.0  0.24350  0.49634  0.78170  1.0000
-  C   C9        1.0  0.94792  0.40085  0.76526  1.0000
-  C   C10       1.0  0.93380  0.50416  0.88248  1.0000
-  C   C11       1.0  0.65612  0.82516  0.41674  1.0000
-  C   C12       1.0  0.97054  0.79660  0.32744  1.0000
-  C   C13       1.0  0.25550  0.83054  0.41222  1.0000
-  C   C14       1.0  0.94704  0.75040  0.50438  1.0000
-  C   C15       1.0  0.94574  0.91466  0.44862  1.0000
-  C   C16       1.0  0.24890  0.53460  0.19596  1.0000
-  C   C17       1.0  0.94957  0.62474  0.21380  1.0000
-  C   C18       1.0  0.64942  0.53194  0.20846  1.0000
-  C   C19       1.0  0.94324  0.44994  0.28662  1.0000
-  C   C20       1.0  0.95572  0.51246  0.10684  1.0000
-  C   C21       1.0  0.33626  0.19214  0.56894  1.0000
-  C   C22       1.0  0.37908  0.15174  0.60828  1.0000
-  C   C23       1.0  0.47626  0.15168  0.60874  1.0000
-  C   C24       1.0  0.53274  0.19282  0.57078  1.0000
-  C   C25       1.0  0.48980  0.23374  0.53202  1.0000
-  C   C26       1.0  0.39292  0.23293  0.53058  1.0000
-  C   C27       1.0  0.54164  0.49388  0.78760  1.0000
-  C   C28       1.0  0.49272  0.44606  0.78286  1.0000
-  C   C29       1.0  0.39628  0.44722  0.77984  1.0000
-  C   C30       1.0  0.34618  0.49567  0.78326  1.0000
-  C   C31       1.0  0.39490  0.54320  0.78888  1.0000
-  C   C32       1.0  0.49174  0.54258  0.79018  1.0000
-  C   C33       1.0  0.35844  0.82978  0.41214  1.0000
-  C   C34       1.0  0.40796  0.87652  0.41897  1.0000
-  C   C35       1.0  0.50486  0.87513  0.42002  1.0000
-  C   C36       1.0  0.55388  0.82694  0.41474  1.0000
-  C   C37       1.0  0.50468  0.78032  0.40774  1.0000
-  C   C38       1.0  0.40796  0.78178  0.40616  1.0000
-  C   C39       1.0  0.35170  0.53422  0.19852  1.0000
-  C   C40       1.0  0.39973  0.58184  0.20478  1.0000
-  C   C41       1.0  0.49602  0.58084  0.20886  1.0000
-  C   C42       1.0  0.54690  0.53270  0.20554  1.0000
-  C   C43       1.0  0.49922  0.48536  0.19856  1.0000
-  C   C44       1.0  0.40262  0.48580  0.19594  1.0000
-  C   C45       1.0  0.93856  0.96258  0.47266  1.0000
-  C   C46       1.0  0.90858  0.95528  0.52956  1.0000
-  C   C47       1.0  0.90792  0.00100  0.55384  1.0000
-  C   C48       1.0  0.93456  0.05372  0.52048  1.0000
-  C   C49       1.0  0.95884  0.06124  0.46282  1.0000
-  C   C50       1.0  0.96301  0.01526  0.43910  1.0000
-  C   C51       1.0  0.93285  0.50716  0.94010  1.0000
-  C   C52       1.0  0.90802  0.45968  0.98284  1.0000
-  C   C53       1.0  0.91774  0.46090  0.03798  1.0000
-  C   C54       1.0  0.95350  0.50912  0.04968  1.0000
-  C   C55       1.0  0.97744  0.55670  0.00714  1.0000
-  C   C56       1.0  0.96686  0.55580  0.95212  1.0000
-  C   C57       1.0  0.95086  0.35304  0.74030  1.0000
-  C   C58       1.0  0.99202  0.36040  0.68524  1.0000
-  C   C59       1.0  0.98698  0.31746  0.65788  1.0000
-  C   C60       1.0  0.93962  0.26750  0.68486  1.0000
-  C   C61       1.0  0.89936  0.25966  0.73996  1.0000
-  C   C62       1.0  0.90524  0.30260  0.76796  1.0000
-  C   C63       1.0  0.94832  0.70564  0.55454  1.0000
-  C   C64       1.0  0.90164  0.65488  0.55824  1.0000
-  C   C65       1.0  0.90360  0.61180  0.60602  1.0000
-  C   C66       1.0  0.95238  0.61946  0.64996  1.0000
-  C   C67       1.0  0.00034  0.66972  0.64596  1.0000
-  C   C68       1.0  0.99866  0.71284  0.59814  1.0000
-  C   C69       1.0  0.96270  0.67166  0.23810  1.0000
-  C   C70       1.0  0.92730  0.72396  0.21542  1.0000
-  C   C71       1.0  0.93506  0.76730  0.24264  1.0000
-  C   C72       1.0  0.97990  0.75796  0.29140  1.0000
-  C   C73       1.0  0.01792  0.70584  0.31288  1.0000
-  C   C74       1.0  0.00806  0.66250  0.28658  1.0000
-  C   C75       1.0  0.94528  0.40452  0.33638  1.0000
-  C   C76       1.0  0.00798  0.36100  0.33606  1.0000
-  C   C77       1.0  0.01286  0.31878  0.38432  1.0000
-  C   C78       1.0  0.95102  0.31808  0.43190  1.0000
-  C   C79       1.0  0.89028  0.36252  0.43274  1.0000
-  C   C80       1.0  0.88810  0.40596  0.38522  1.0000
-  Cd  Cd1       1.0  0.80892  0.19254  0.56892  1.0000
-  Cd  Cd2       1.0  0.06024  0.19322  0.56686  1.0000
-  Cd  Cd3       1.0  0.81700  0.49380  0.78818  1.0000
-  Cd  Cd4       1.0  0.07126  0.49766  0.78124  1.0000
-  Cd  Cd5       1.0  0.82678  0.82250  0.42060  1.0000
-  Cd  Cd6       1.0  0.08312  0.83044  0.41292  1.0000
-  Cd  Cd7       1.0  0.07602  0.53170  0.19586  1.0000
-  Cd  Cd8       1.0  0.82201  0.52810  0.20836  1.0000
-  O   O1        1.0  0.86496  0.24862  0.50056  1.0000
-  O   O2        1.0  0.02360  0.25408  0.50222  1.0000
-  O   O3        1.0  0.01408  0.13040  0.53714  1.0000
-  O   O4        1.0  0.85852  0.11616  0.56846  1.0000
-  O   O5        1.0  0.69302  0.20400  0.52520  1.0000
-  O   O6        1.0  0.67946  0.18090  0.61562  1.0000
-  O   O7        1.0  0.85508  0.23398  0.62282  1.0000
-  O   O8        1.0  0.99569  0.19562  0.64286  1.0000
-  O   O9        1.0  0.18100  0.14728  0.57712  1.0000
-  O   O10       1.0  0.18480  0.23748  0.55854  1.0000
-  O   O11       1.0  0.86632  0.42024  0.77704  1.0000
-  O   O12       1.0  0.02614  0.42750  0.76390  1.0000
-  O   O13       1.0  0.01412  0.51210  0.85282  1.0000
-  O   O14       1.0  0.85676  0.49182  0.86435  1.0000
-  O   O15       1.0  0.69990  0.46804  0.75836  1.0000
-  O   O16       1.0  0.68894  0.51830  0.81952  1.0000
-  O   O17       1.0  0.87056  0.55830  0.72734  1.0000
-  O   O18       1.0  0.03026  0.55348  0.71480  1.0000
-  O   O19       1.0  0.18846  0.45424  0.80610  1.0000
-  O   O20       1.0  0.19862  0.53918  0.75654  1.0000
-  O   O21       1.0  0.86664  0.76748  0.48790  1.0000
-  O   O22       1.0  0.02710  0.77040  0.47834  1.0000
-  O   O23       1.0  0.02856  0.89606  0.43868  1.0000
-  O   O24       1.0  0.86862  0.89124  0.44186  1.0000
-  O   O25       1.0  0.69754  0.78508  0.44904  1.0000
-  O   O26       1.0  0.71358  0.86356  0.38646  1.0000
-  O   O27       1.0  0.88932  0.79620  0.35550  1.0000
-  O   O28       1.0  0.04694  0.81456  0.34174  1.0000
-  O   O29       1.0  0.20130  0.78850  0.43790  1.0000
-  O   O30       1.0  0.20974  0.87298  0.38690  1.0000
-  O   O31       1.0  0.02246  0.47316  0.26280  1.0000
-  O   O32       1.0  0.86308  0.46554  0.26898  1.0000
-  O   O33       1.0  0.87568  0.51560  0.13488  1.0000
-  O   O34       1.0  0.03608  0.51782  0.12482  1.0000
-  O   O35       1.0  0.20566  0.50790  0.16596  1.0000
-  O   O36       1.0  0.19186  0.56052  0.22484  1.0000
-  O   O37       1.0  0.02292  0.60876  0.18692  1.0000
-  O   O38       1.0  0.87524  0.59336  0.23260  1.0000
-  O   O39       1.0  0.70576  0.57314  0.18312  1.0000
-  O   O40       1.0  0.69302  0.48918  0.23498  1.0000
+  Cu  Cu1       1.0  0.43438  0.00001  0.56562  1.0000
+  Cu  Cu2       1.0  0.99999  0.56563  0.00001  1.0000
+  Cu  Cu3       1.0  0.56561  0.99999  0.43439  1.0000
+  Cu  Cu4       1.0  0.00001  0.43434  0.99999  1.0000
+  Cu  Cu5       1.0  0.43437  0.00000  1.00000  1.0000
+  Cu  Cu6       1.0  0.00000  0.43435  0.56565  1.0000
+  Cu  Cu7       1.0  0.99999  0.00000  0.56568  1.0000
+  Cu  Cu8       1.0  0.43436  0.56564  0.00001  1.0000
+  Cu  Cu9       1.0  0.99999  0.56560  0.43439  1.0000
+  Cu  Cu10      1.0  0.56564  0.43436  0.99999  1.0000
+  Cu  Cu11      1.0  0.56561  0.99999  0.00000  1.0000
+  Cu  Cu12      1.0  0.00001  1.00000  0.43438  1.0000
+  H   H1        1.0  0.49629  0.26606  0.26617  1.0000
+  H   H2        1.0  0.02854  0.50369  0.73383  1.0000
+  H   H3        1.0  0.26617  0.97147  0.49629  1.0000
+  H   H4        1.0  0.73384  0.73394  0.02854  1.0000
+  H   H5        1.0  0.73382  0.02853  0.73393  1.0000
+  H   H6        1.0  0.26611  0.49627  0.97150  1.0000
+  H   H7        1.0  0.02854  0.73384  0.50366  1.0000
+  H   H8        1.0  0.73383  0.02853  0.50370  1.0000
+  H   H9        1.0  0.97149  0.26612  0.26611  1.0000
+  H   H10       1.0  0.73389  0.50373  0.02851  1.0000
+  H   H11       1.0  0.49634  0.26604  0.97146  1.0000
+  H   H12       1.0  0.49634  0.97144  0.26611  1.0000
+  H   H13       1.0  0.26610  0.26612  0.49634  1.0000
+  H   H14       1.0  0.26607  0.49628  0.26619  1.0000
+  H   H15       1.0  0.26617  0.26606  0.97146  1.0000
+  H   H16       1.0  0.97146  0.26616  0.49633  1.0000
+  H   H17       1.0  0.26619  0.97147  0.26606  1.0000
+  H   H18       1.0  0.97146  0.49632  0.26617  1.0000
+  H   H19       1.0  0.73390  0.73388  0.50365  1.0000
+  H   H20       1.0  0.50366  0.02856  0.73390  1.0000
+  H   H21       1.0  0.73393  0.50373  0.73381  1.0000
+  H   H22       1.0  0.50367  0.73396  0.02854  1.0000
+  H   H23       1.0  0.02851  0.73387  0.73389  1.0000
+  H   H24       1.0  0.50371  0.73393  0.73383  1.0000
+  C   C1        1.0  0.38638  0.25700  0.38643  1.0000
+  C   C2        1.0  0.02979  0.61360  0.74298  1.0000
+  C   C3        1.0  0.38643  0.97018  0.38639  1.0000
+  C   C4        1.0  0.74298  0.61364  0.02979  1.0000
+  C   C5        1.0  0.61357  0.02982  0.74299  1.0000
+  C   C6        1.0  0.25702  0.38637  0.97021  1.0000
+  C   C7        1.0  0.02980  0.61360  0.61358  1.0000
+  C   C8        1.0  0.74295  0.02981  0.61361  1.0000
+  C   C9        1.0  0.97021  0.38641  0.25702  1.0000
+  C   C10       1.0  0.61359  0.61364  0.02979  1.0000
+  C   C11       1.0  0.38642  0.38636  0.97021  1.0000
+  C   C12       1.0  0.38644  0.97018  0.25700  1.0000
+  C   C13       1.0  0.25700  0.38639  0.38643  1.0000
+  C   C14       1.0  0.38639  0.38637  0.25705  1.0000
+  C   C15       1.0  0.38642  0.25698  0.97020  1.0000
+  C   C16       1.0  0.97021  0.25702  0.38641  1.0000
+  C   C17       1.0  0.25705  0.97019  0.38638  1.0000
+  C   C18       1.0  0.97020  0.38641  0.38642  1.0000
+  C   C19       1.0  0.61362  0.74300  0.61357  1.0000
+  C   C20       1.0  0.61357  0.02982  0.61361  1.0000
+  C   C21       1.0  0.74300  0.61363  0.61356  1.0000
+  C   C22       1.0  0.61358  0.74302  0.02980  1.0000
+  C   C23       1.0  0.02979  0.74298  0.61358  1.0000
+  C   C24       1.0  0.61362  0.61362  0.74295  1.0000
+  C   C25       1.0  0.43057  0.16298  0.43060  1.0000
+  C   C26       1.0  0.02417  0.56940  0.83700  1.0000
+  C   C27       1.0  0.43059  0.97586  0.43057  1.0000
+  C   C28       1.0  0.83700  0.56943  0.02418  1.0000
+  C   C29       1.0  0.56940  0.02413  0.83703  1.0000
+  C   C30       1.0  0.16300  0.43058  0.97582  1.0000
+  C   C31       1.0  0.02413  0.56942  0.56940  1.0000
+  C   C32       1.0  0.83696  0.02418  0.56942  1.0000
+  C   C33       1.0  0.97582  0.43060  0.16300  1.0000
+  C   C34       1.0  0.56939  0.56943  0.02419  1.0000
+  C   C35       1.0  0.43062  0.43057  0.97581  1.0000
+  C   C36       1.0  0.43060  0.97587  0.16297  1.0000
+  C   C37       1.0  0.16297  0.43056  0.43060  1.0000
+  C   C38       1.0  0.43058  0.43056  0.16304  1.0000
+  C   C39       1.0  0.43060  0.16294  0.97587  1.0000
+  C   C40       1.0  0.97581  0.16301  0.43061  1.0000
+  C   C41       1.0  0.16304  0.97582  0.43058  1.0000
+  C   C42       1.0  0.97587  0.43058  0.43060  1.0000
+  C   C43       1.0  0.56943  0.83702  0.56941  1.0000
+  C   C44       1.0  0.56940  0.02414  0.56944  1.0000
+  C   C45       1.0  0.83703  0.56945  0.56940  1.0000
+  C   C46       1.0  0.56940  0.83706  0.02413  1.0000
+  C   C47       1.0  0.02418  0.83699  0.56939  1.0000
+  C   C48       1.0  0.56942  0.56942  0.83696  1.0000
+  C   C49       1.0  0.42966  0.30010  0.30017  1.0000
+  C   C50       1.0  0.02993  0.57031  0.69984  1.0000
+  C   C51       1.0  0.30017  0.97007  0.42966  1.0000
+  C   C52       1.0  0.69985  0.69992  0.02993  1.0000
+  C   C53       1.0  0.69983  0.02993  0.69989  1.0000
+  C   C54       1.0  0.30014  0.42963  0.97011  1.0000
+  C   C55       1.0  0.02993  0.69986  0.57029  1.0000
+  C   C56       1.0  0.69983  0.02993  0.57034  1.0000
+  C   C57       1.0  0.97011  0.30013  0.30013  1.0000
+  C   C58       1.0  0.69987  0.57037  0.02990  1.0000
+  C   C59       1.0  0.42970  0.30007  0.97008  1.0000
+  C   C60       1.0  0.42973  0.97004  0.30012  1.0000
+  C   C61       1.0  0.30011  0.30012  0.42972  1.0000
+  C   C62       1.0  0.30011  0.42965  0.30017  1.0000
+  C   C63       1.0  0.30015  0.30008  0.97008  1.0000
+  C   C64       1.0  0.97008  0.30015  0.42970  1.0000
+  C   C65       1.0  0.30018  0.97007  0.30010  1.0000
+  C   C66       1.0  0.97007  0.42969  0.30015  1.0000
+  C   C67       1.0  0.69988  0.69988  0.57027  1.0000
+  C   C68       1.0  0.57028  0.02996  0.69988  1.0000
+  C   C69       1.0  0.69990  0.57035  0.69982  1.0000
+  C   C70       1.0  0.57030  0.69992  0.02992  1.0000
+  C   C71       1.0  0.02990  0.69987  0.69986  1.0000
+  C   C72       1.0  0.57034  0.69990  0.69983  1.0000
+  O   O1        1.0  0.38627  0.12647  0.50815  1.0000
+  O   O2        1.0  0.02092  0.61371  0.87353  1.0000
+  O   O3        1.0  0.50814  0.97912  0.38627  1.0000
+  O   O4        1.0  0.87352  0.49184  0.02092  1.0000
+  O   O5        1.0  0.49186  0.02086  0.87354  1.0000
+  O   O6        1.0  0.12650  0.38626  0.97908  1.0000
+  O   O7        1.0  0.02086  0.49188  0.61369  1.0000
+  O   O8        1.0  0.87347  0.02093  0.61374  1.0000
+  O   O9        1.0  0.97908  0.50816  0.12650  1.0000
+  O   O10       1.0  0.49182  0.61373  0.02094  1.0000
+  O   O11       1.0  0.38629  0.50816  0.97907  1.0000
+  O   O12       1.0  0.38630  0.97914  0.12645  1.0000
+  O   O13       1.0  0.12644  0.50813  0.38629  1.0000
+  O   O14       1.0  0.50817  0.38625  0.12651  1.0000
+  O   O15       1.0  0.50816  0.12641  0.97913  1.0000
+  O   O16       1.0  0.97906  0.12648  0.38630  1.0000
+  O   O17       1.0  0.12651  0.97906  0.50816  1.0000
+  O   O18       1.0  0.97913  0.38630  0.50816  1.0000
+  O   O19       1.0  0.49186  0.87356  0.61371  1.0000
+  O   O20       1.0  0.61370  0.02088  0.49186  1.0000
+  O   O21       1.0  0.87355  0.61374  0.49185  1.0000
+  O   O22       1.0  0.61369  0.87357  0.02087  1.0000
+  O   O23       1.0  0.02093  0.87352  0.49181  1.0000
+  O   O24       1.0  0.61374  0.49185  0.87348  1.0000
+  O   O25       1.0  0.61373  0.87353  0.49186  1.0000
+  O   O26       1.0  0.97907  0.38629  0.12648  1.0000
+  O   O27       1.0  0.49186  0.02088  0.61373  1.0000
+  O   O28       1.0  0.12647  0.50817  0.97908  1.0000
+  O   O29       1.0  0.50814  0.97914  0.12645  1.0000
+  O   O30       1.0  0.87351  0.61374  0.02092  1.0000
+  O   O31       1.0  0.97913  0.50814  0.38630  1.0000
+  O   O32       1.0  0.12651  0.97908  0.38626  1.0000
+  O   O33       1.0  0.02092  0.49184  0.87350  1.0000
+  O   O34       1.0  0.50819  0.38626  0.97906  1.0000
+  O   O35       1.0  0.61371  0.49183  0.02094  1.0000
+  O   O36       1.0  0.61370  0.02086  0.87356  1.0000
+  O   O37       1.0  0.87355  0.49189  0.61369  1.0000
+  O   O38       1.0  0.49184  0.61373  0.87349  1.0000
+  O   O39       1.0  0.49184  0.87359  0.02087  1.0000
+  O   O40       1.0  0.02093  0.87351  0.61371  1.0000
+  O   O41       1.0  0.87350  0.02093  0.49183  1.0000
+  O   O42       1.0  0.02087  0.61371  0.49183  1.0000
+  O   O43       1.0  0.50814  0.12644  0.38630  1.0000
+  O   O44       1.0  0.38630  0.97912  0.50814  1.0000
+  O   O45       1.0  0.12645  0.38628  0.50813  1.0000
+  O   O46       1.0  0.38630  0.12643  0.97913  1.0000
+  O   O47       1.0  0.97905  0.12650  0.50818  1.0000
+  O   O48       1.0  0.38626  0.50813  0.12653  1.0000
```

### Comparing `moftransformer-2.0.0/moftransformer/examples/dataset/total/ukg+N387+E203.cif` & `moftransformer-2.0.1/moftransformer/examples/raw/ukg+N387+E203.cif`

 * *Files 25% similar despite different names*

```diff
@@ -1,537 +1,538 @@
-data_image0
-_chemical_formula_structural       Nd16H240C160O96
-_chemical_formula_sum              "Nd16 H240 C160 O96"
-_cell_length_a       34.1054
-_cell_length_b       36.7791
-_cell_length_c       42.6074
-_cell_angle_alpha    90.155
-_cell_angle_beta     90.263
-_cell_angle_gamma    92.855
-
-_space_group_name_H-M_alt    "P 1"
-_space_group_IT_number       1
-
+# generated using pymatgen
+data_NdH15(C5O3)2
+_symmetry_space_group_name_H-M   'P 1'
+_cell_length_a   34.10540000
+_cell_length_b   36.77910000
+_cell_length_c   42.60740000
+_cell_angle_alpha   90.15500000
+_cell_angle_beta   90.26300000
+_cell_angle_gamma   92.85500000
+_symmetry_Int_Tables_number   1
+_chemical_formula_structural   NdH15(C5O3)2
+_chemical_formula_sum   'Nd16 H240 C160 O96'
+_cell_volume   53378.14063596
+_cell_formula_units_Z   16
 loop_
-  _space_group_symop_operation_xyz
-  'x, y, z'
-
+ _symmetry_equiv_pos_site_id
+ _symmetry_equiv_pos_as_xyz
+  1  'x, y, z'
 loop_
-  _atom_site_type_symbol
-  _atom_site_label
-  _atom_site_symmetry_multiplicity
-  _atom_site_fract_x
-  _atom_site_fract_y
-  _atom_site_fract_z
-  _atom_site_occupancy
-  Nd  Nd1       1.0  0.69604  0.94027  0.14098  1.0000
-  Nd  Nd2       1.0  0.65069  0.02063  0.15613  1.0000
-  Nd  Nd3       1.0  0.43877  0.63496  0.64894  1.0000
-  Nd  Nd4       1.0  0.52174  0.68257  0.63232  1.0000
-  Nd  Nd5       1.0  0.79754  0.52846  0.14198  1.0000
-  Nd  Nd6       1.0  0.84488  0.45579  0.15941  1.0000
-  Nd  Nd7       1.0  0.04062  0.84261  0.65648  1.0000
-  Nd  Nd8       1.0  0.94701  0.80851  0.66546  1.0000
-  Nd  Nd9       1.0  0.34650  0.05106  0.88646  1.0000
-  Nd  Nd10      1.0  0.37889  0.96688  0.87457  1.0000
-  Nd  Nd11      1.0  0.44870  0.37289  0.36890  1.0000
-  Nd  Nd12      1.0  0.45404  0.30985  0.32343  1.0000
-  Nd  Nd13      1.0  0.15956  0.43422  0.89243  1.0000
-  Nd  Nd14      1.0  0.11890  0.51607  0.88183  1.0000
-  Nd  Nd15      1.0  0.03119  0.10253  0.38320  1.0000
-  Nd  Nd16      1.0  0.03049  0.15860  0.31941  1.0000
-  H   H1        1.0  0.60421  0.93206  0.19101  1.0000
-  H   H2        1.0  0.73333  0.03313  0.10210  1.0000
-  H   H3        1.0  0.52385  0.60369  0.69423  1.0000
-  H   H4        1.0  0.42856  0.69963  0.57923  1.0000
-  H   H5        1.0  0.88384  0.53941  0.20530  1.0000
-  H   H6        1.0  0.77879  0.44096  0.08945  1.0000
-  H   H7        1.0  0.97496  0.89110  0.71845  1.0000
-  H   H8        1.0  0.00980  0.74994  0.61596  1.0000
-  H   H9        1.0  0.30958  0.97473  0.94500  1.0000
-  H   H10       1.0  0.42895  0.03590  0.82423  1.0000
-  H   H11       1.0  0.40623  0.38109  0.27510  1.0000
-  H   H12       1.0  0.47969  0.28521  0.41040  1.0000
-  H   H13       1.0  0.19849  0.51344  0.94588  1.0000
-  H   H14       1.0  0.06771  0.44275  0.83693  1.0000
-  H   H15       1.0  0.07274  0.06372  0.30737  1.0000
-  H   H16       1.0  0.99809  0.20262  0.39109  1.0000
-  H   H17       1.0  0.46704  0.06512  0.94639  1.0000
-  H   H18       1.0  0.63170  0.98466  0.04354  1.0000
-  H   H19       1.0  0.56885  0.01074  0.06839  1.0000
-  H   H20       1.0  0.57970  0.01357  0.01239  1.0000
-  H   H21       1.0  0.50750  0.01930  0.03163  1.0000
-  H   H22       1.0  0.52506  0.04153  0.98033  1.0000
-  H   H23       1.0  0.45025  0.02378  0.98839  1.0000
-  H   H24       1.0  0.49072  0.03051  0.92424  1.0000
-  H   H25       1.0  0.60984  0.94010  0.05050  1.0000
-  H   H26       1.0  0.54782  0.96476  0.06631  1.0000
-  H   H27       1.0  0.56720  0.96584  0.00714  1.0000
-  H   H28       1.0  0.49864  0.97312  0.01786  1.0000
-  H   H29       1.0  0.52875  0.99651  0.96437  1.0000
-  H   H30       1.0  0.45890  0.98390  0.96522  1.0000
-  H   H31       1.0  0.53025  0.55424  0.58636  1.0000
-  H   H32       1.0  0.48631  0.47457  0.42152  1.0000
-  H   H33       1.0  0.46212  0.44127  0.47323  1.0000
-  H   H34       1.0  0.50562  0.49444  0.47682  1.0000
-  H   H35       1.0  0.46078  0.48338  0.52595  1.0000
-  H   H36       1.0  0.51969  0.52132  0.53190  1.0000
-  H   H37       1.0  0.46468  0.53380  0.57264  1.0000
-  H   H38       1.0  0.53333  0.58803  0.55613  1.0000
-  H   H39       1.0  0.43691  0.48825  0.41721  1.0000
-  H   H40       1.0  0.41901  0.46752  0.46906  1.0000
-  H   H41       1.0  0.46919  0.52438  0.46319  1.0000
-  H   H42       1.0  0.43283  0.52034  0.51150  1.0000
-  H   H43       1.0  0.50079  0.55783  0.50932  1.0000
-  H   H44       1.0  0.45594  0.57409  0.55004  1.0000
-  H   H45       1.0  0.93788  0.52016  0.09471  1.0000
-  H   H46       1.0  0.04527  0.41864  0.96170  1.0000
-  H   H47       1.0  0.99551  0.46116  0.95120  1.0000
-  H   H48       1.0  0.00762  0.44232  0.01059  1.0000
-  H   H49       1.0  0.94323  0.46080  0.00018  1.0000
-  H   H50       1.0  0.97331  0.47491  0.05712  1.0000
-  H   H51       1.0  0.90433  0.46715  0.05673  1.0000
-  H   H52       1.0  0.90801  0.54915  0.07171  1.0000
-  H   H53       1.0  0.07519  0.45104  0.98309  1.0000
-  H   H54       1.0  0.02734  0.50041  0.96048  1.0000
-  H   H55       1.0  0.02801  0.48798  0.01523  1.0000
-  H   H56       1.0  0.95929  0.50716  0.99164  1.0000
-  H   H57       1.0  0.97391  0.52159  0.04491  1.0000
-  H   H58       1.0  0.89735  0.50556  0.03169  1.0000
-  H   H59       1.0  0.02041  0.06361  0.48787  1.0000
-  H   H60       1.0  0.92776  0.89976  0.58356  1.0000
-  H   H61       1.0  0.97378  0.89172  0.54232  1.0000
-  H   H62       1.0  0.95126  0.95888  0.54959  1.0000
-  H   H63       1.0  0.97453  0.94600  0.49834  1.0000
-  H   H64       1.0  0.98386  0.01369  0.51828  1.0000
-  H   H65       1.0  0.98359  0.00580  0.46216  1.0000
-  H   H66       1.0  0.06484  0.04294  0.47576  1.0000
-  H   H67       1.0  0.96061  0.93046  0.60486  1.0000
-  H   H68       1.0  0.01576  0.90626  0.56568  1.0000
-  H   H69       1.0  0.99958  0.96877  0.56536  1.0000
-  H   H70       1.0  0.02435  0.94103  0.51146  1.0000
-  H   H71       1.0  0.03505  0.00493  0.52189  1.0000
-  H   H72       1.0  0.03125  0.98649  0.46208  1.0000
-  H   H73       1.0  0.71670  0.82846  0.09735  1.0000
-  H   H74       1.0  0.74252  0.63093  0.09600  1.0000
-  H   H75       1.0  0.79051  0.66848  0.12968  1.0000
-  H   H76       1.0  0.73427  0.69641  0.10144  1.0000
-  H   H77       1.0  0.77984  0.73863  0.13315  1.0000
-  H   H78       1.0  0.72448  0.76185  0.10182  1.0000
-  H   H79       1.0  0.76473  0.80816  0.13547  1.0000
-  H   H80       1.0  0.67652  0.81747  0.12365  1.0000
-  H   H81       1.0  0.71148  0.62300  0.12897  1.0000
-  H   H82       1.0  0.75914  0.66024  0.16337  1.0000
-  H   H83       1.0  0.70397  0.68906  0.13551  1.0000
-  H   H84       1.0  0.74783  0.73204  0.16667  1.0000
-  H   H85       1.0  0.69175  0.75468  0.13444  1.0000
-  H   H86       1.0  0.72766  0.80230  0.16558  1.0000
-  H   H87       1.0  0.62075  0.76834  0.59905  1.0000
-  H   H88       1.0  0.83487  0.82659  0.60312  1.0000
-  H   H89       1.0  0.80457  0.79639  0.65130  1.0000
-  H   H90       1.0  0.76305  0.80508  0.60365  1.0000
-  H   H91       1.0  0.73205  0.77300  0.65055  1.0000
-  H   H92       1.0  0.69203  0.78570  0.60297  1.0000
-  H   H93       1.0  0.65799  0.75133  0.64725  1.0000
-  H   H94       1.0  0.63403  0.72782  0.57972  1.0000
-  H   H95       1.0  0.84820  0.78239  0.58930  1.0000
-  H   H96       1.0  0.81775  0.75256  0.63661  1.0000
-  H   H97       1.0  0.77659  0.76169  0.58845  1.0000
-  H   H98       1.0  0.74458  0.72981  0.63396  1.0000
-  H   H99       1.0  0.70487  0.74311  0.58580  1.0000
-  H   H100      1.0  0.67021  0.70888  0.62898  1.0000
-  H   H101      1.0  0.20040  0.32767  0.94035  1.0000
-  H   H102      1.0  0.30980  0.15866  0.93511  1.0000
-  H   H103      1.0  0.25542  0.16462  0.89471  1.0000
-  H   H104      1.0  0.27375  0.21452  0.93278  1.0000
-  H   H105      1.0  0.22181  0.22797  0.89170  1.0000
-  H   H106      1.0  0.23713  0.27118  0.93488  1.0000
-  H   H107      1.0  0.19279  0.29409  0.89051  1.0000
-  H   H108      1.0  0.24678  0.34768  0.92920  1.0000
-  H   H109      1.0  0.34485  0.17460  0.90597  1.0000
-  H   H110      1.0  0.29156  0.18289  0.86726  1.0000
-  H   H111      1.0  0.31078  0.23265  0.90645  1.0000
-  H   H112      1.0  0.26024  0.24895  0.86772  1.0000
-  H   H113      1.0  0.27852  0.29106  0.91408  1.0000
-  H   H114      1.0  0.23606  0.31755  0.87444  1.0000
-  H   H115      1.0  0.31950  0.31943  0.39098  1.0000
-  H   H116      1.0  0.13259  0.20557  0.39985  1.0000
-  H   H117      1.0  0.15700  0.21975  0.34482  1.0000
-  H   H118      1.0  0.19365  0.24472  0.39115  1.0000
-  H   H119      1.0  0.22725  0.25554  0.33860  1.0000
-  H   H120      1.0  0.25636  0.28333  0.38720  1.0000
-  H   H121      1.0  0.29767  0.29276  0.33853  1.0000
-  H   H122      1.0  0.34415  0.27876  0.39942  1.0000
-  H   H123      1.0  0.15827  0.16441  0.39971  1.0000
-  H   H124      1.0  0.18422  0.17883  0.34586  1.0000
-  H   H125      1.0  0.21917  0.20345  0.39535  1.0000
-  H   H126      1.0  0.25386  0.21487  0.34477  1.0000
-  H   H127      1.0  0.28113  0.24249  0.39567  1.0000
-  H   H128      1.0  0.32261  0.25177  0.34749  1.0000
-  H   H129      1.0  0.56433  0.24320  0.31932  1.0000
-  H   H130      1.0  0.68212  0.10681  0.23535  1.0000
-  H   H131      1.0  0.60816  0.10681  0.22656  1.0000
-  H   H132      1.0  0.64093  0.15195  0.26300  1.0000
-  H   H133      1.0  0.56821  0.15447  0.25262  1.0000
-  H   H134      1.0  0.60152  0.19746  0.29074  1.0000
-  H   H135      1.0  0.52924  0.20282  0.28048  1.0000
-  H   H136      1.0  0.57747  0.27575  0.28893  1.0000
-  H   H137      1.0  0.68835  0.13556  0.20082  1.0000
-  H   H138      1.0  0.61650  0.13763  0.19407  1.0000
-  H   H139      1.0  0.65048  0.18284  0.23072  1.0000
-  H   H140      1.0  0.57850  0.18636  0.22111  1.0000
-  H   H141      1.0  0.61255  0.22930  0.25947  1.0000
-  H   H142      1.0  0.54076  0.23528  0.24958  1.0000
-  H   H143      1.0  0.36383  0.65685  0.73967  1.0000
-  H   H144      1.0  0.25999  0.51767  0.84857  1.0000
-  H   H145      1.0  0.21787  0.55414  0.80875  1.0000
-  H   H146      1.0  0.28566  0.57090  0.81623  1.0000
-  H   H147      1.0  0.25822  0.58780  0.76125  1.0000
-  H   H148      1.0  0.31769  0.61916  0.77793  1.0000
-  H   H149      1.0  0.31169  0.61634  0.71807  1.0000
-  H   H150      1.0  0.39315  0.61899  0.74985  1.0000
-  H   H151      1.0  0.25680  0.48101  0.82082  1.0000
-  H   H152      1.0  0.22737  0.51822  0.78121  1.0000
-  H   H153      1.0  0.30186  0.53013  0.79801  1.0000
-  H   H154      1.0  0.28316  0.54915  0.74635  1.0000
-  H   H155      1.0  0.34561  0.57895  0.77617  1.0000
-  H   H156      1.0  0.34219  0.57755  0.71874  1.0000
-  H   H157      1.0  0.81099  0.33394  0.18601  1.0000
-  H   H158      1.0  0.92423  0.18298  0.25277  1.0000
-  H   H159      1.0  0.95994  0.24374  0.24611  1.0000
-  H   H160      1.0  0.88829  0.23456  0.23068  1.0000
-  H   H161      1.0  0.92287  0.29425  0.21980  1.0000
-  H   H162      1.0  0.85053  0.28480  0.20792  1.0000
-  H   H163      1.0  0.88488  0.34347  0.19397  1.0000
-  H   H164      1.0  0.80383  0.35660  0.22350  1.0000
-  H   H165      1.0  0.90744  0.19634  0.29056  1.0000
-  H   H166      1.0  0.94481  0.25733  0.28491  1.0000
-  H   H167      1.0  0.87472  0.25019  0.26915  1.0000
-  H   H168      1.0  0.91101  0.31027  0.25863  1.0000
-  H   H169      1.0  0.83948  0.30222  0.24640  1.0000
-  H   H170      1.0  0.87558  0.36156  0.23251  1.0000
-  H   H171      1.0  0.23582  0.00826  0.82615  1.0000
-  H   H172      1.0  0.09280  0.87895  0.75074  1.0000
-  H   H173      1.0  0.14404  0.91447  0.71735  1.0000
-  H   H174      1.0  0.14270  0.91849  0.77495  1.0000
-  H   H175      1.0  0.20287  0.94726  0.74566  1.0000
-  H   H176      1.0  0.18908  0.96147  0.80029  1.0000
-  H   H177      1.0  0.25929  0.97930  0.77945  1.0000
-  H   H178      1.0  0.23801  0.96730  0.84878  1.0000
-  H   H179      1.0  0.12135  0.83935  0.74688  1.0000
-  H   H180      1.0  0.17367  0.87497  0.71905  1.0000
-  H   H181      1.0  0.16972  0.87784  0.77873  1.0000
-  H   H182      1.0  0.22875  0.90735  0.75670  1.0000
-  H   H183      1.0  0.20915  0.91990  0.81381  1.0000
-  H   H184      1.0  0.27524  0.94010  0.80061  1.0000
-  H   H185      1.0  0.37209  0.91336  0.77593  1.0000
-  H   H186      1.0  0.45665  0.77844  0.67453  1.0000
-  H   H187      1.0  0.47511  0.77266  0.72940  1.0000
-  H   H188      1.0  0.42535  0.81899  0.71141  1.0000
-  H   H189      1.0  0.45247  0.82491  0.76536  1.0000
-  H   H190      1.0  0.39846  0.86419  0.74523  1.0000
-  H   H191      1.0  0.42754  0.87767  0.79806  1.0000
-  H   H192      1.0  0.33693  0.88330  0.79542  1.0000
-  H   H193      1.0  0.41048  0.75353  0.68053  1.0000
-  H   H194      1.0  0.43364  0.74124  0.73714  1.0000
-  H   H195      1.0  0.38684  0.78760  0.72478  1.0000
-  H   H196      1.0  0.41493  0.79256  0.77965  1.0000
-  H   H197      1.0  0.36262  0.83270  0.76249  1.0000
-  H   H198      1.0  0.39153  0.84637  0.81578  1.0000
-  H   H199      1.0  0.58900  0.36472  0.32880  1.0000
-  H   H200      1.0  0.75442  0.45943  0.24631  1.0000
-  H   H201      1.0  0.70591  0.42130  0.21342  1.0000
-  H   H202      1.0  0.69666  0.43051  0.27096  1.0000
-  H   H203      1.0  0.64206  0.39477  0.24099  1.0000
-  H   H204      1.0  0.64217  0.39845  0.29874  1.0000
-  H   H205      1.0  0.57907  0.37084  0.27269  1.0000
-  H   H206      1.0  0.57743  0.41108  0.33647  1.0000
-  H   H207      1.0  0.72857  0.49949  0.23607  1.0000
-  H   H208      1.0  0.67955  0.46176  0.20527  1.0000
-  H   H209      1.0  0.67125  0.47135  0.26362  1.0000
-  H   H210      1.0  0.61631  0.43650  0.23805  1.0000
-  H   H211      1.0  0.62026  0.44192  0.29784  1.0000
-  H   H212      1.0  0.55817  0.41481  0.27731  1.0000
-  H   H213      1.0  0.14439  0.58772  0.79062  1.0000
-  H   H214      1.0  0.05613  0.76868  0.74729  1.0000
-  H   H215      1.0  0.04986  0.71052  0.70969  1.0000
-  H   H216      1.0  0.09131  0.70981  0.75459  1.0000
-  H   H217      1.0  0.05888  0.64530  0.73908  1.0000
-  H   H218      1.0  0.11911  0.64732  0.76752  1.0000
-  H   H219      1.0  0.07497  0.58853  0.77814  1.0000
-  H   H220      1.0  0.14035  0.61833  0.82275  1.0000
-  H   H221      1.0  0.00535  0.75725  0.75618  1.0000
-  H   H222      1.0  0.00577  0.69930  0.73169  1.0000
-  H   H223      1.0  0.05153  0.71199  0.78192  1.0000
-  H   H224      1.0  0.02952  0.65025  0.77388  1.0000
-  H   H225      1.0  0.09800  0.66576  0.80235  1.0000
-  H   H226      1.0  0.06333  0.60924  0.81528  1.0000
-  H   H227      1.0  0.75637  0.96566  0.24155  1.0000
-  H   H228      1.0  0.91004  0.05291  0.34201  1.0000
-  H   H229      1.0  0.92572  0.05255  0.28311  1.0000
-  H   H230      1.0  0.86319  0.02583  0.30477  1.0000
-  H   H231      1.0  0.86762  0.02811  0.24539  1.0000
-  H   H232      1.0  0.81047  0.99729  0.27211  1.0000
-  H   H233      1.0  0.80672  0.00245  0.21248  1.0000
-  H   H234      1.0  0.72993  0.00595  0.25041  1.0000
-  H   H235      1.0  0.89435  0.09836  0.33755  1.0000
-  H   H236      1.0  0.90485  0.09676  0.28027  1.0000
-  H   H237      1.0  0.84195  0.06962  0.30436  1.0000
-  H   H238      1.0  0.84371  0.07096  0.24619  1.0000
-  H   H239      1.0  0.78654  0.03967  0.27508  1.0000
-  H   H240      1.0  0.77959  0.04307  0.21743  1.0000
-  C   C1        1.0  0.66676  0.08157  0.19158  1.0000
-  C   C2        1.0  0.72478  0.98751  0.20323  1.0000
-  C   C3        1.0  0.61524  0.95791  0.18192  1.0000
-  C   C4        1.0  0.70966  0.86606  0.13472  1.0000
-  C   C5        1.0  0.62863  0.97073  0.09118  1.0000
-  C   C6        1.0  0.72637  0.00745  0.11341  1.0000
-  C   C7        1.0  0.59073  0.72000  0.61463  1.0000
-  C   C8        1.0  0.50203  0.60283  0.59682  1.0000
-  C   C9        1.0  0.52478  0.62652  0.67839  1.0000
-  C   C10       1.0  0.39317  0.63135  0.70181  1.0000
-  C   C11       1.0  0.45974  0.72098  0.67849  1.0000
-  C   C12       1.0  0.42949  0.68054  0.59834  1.0000
-  C   C13       1.0  0.82788  0.38994  0.18664  1.0000
-  C   C14       1.0  0.76193  0.47738  0.19921  1.0000
-  C   C15       1.0  0.87423  0.51471  0.19326  1.0000
-  C   C16       1.0  0.76312  0.59361  0.12913  1.0000
-  C   C17       1.0  0.87746  0.50991  0.10122  1.0000
-  C   C18       1.0  0.78248  0.46516  0.10371  1.0000
-  C   C19       1.0  0.88073  0.80222  0.62870  1.0000
-  C   C20       1.0  0.97179  0.87559  0.61184  1.0000
-  C   C21       1.0  0.96552  0.86775  0.70448  1.0000
-  C   C22       1.0  0.09272  0.85677  0.70539  1.0000
-  C   C23       1.0  0.01637  0.77521  0.70951  1.0000
-  C   C24       1.0  0.01939  0.77618  0.62529  1.0000
-  C   C25       1.0  0.37141  0.91918  0.82506  1.0000
-  C   C26       1.0  0.29255  0.99451  0.84272  1.0000
-  C   C27       1.0  0.32954  0.97065  0.92591  1.0000
-  C   C28       1.0  0.32105  0.12081  0.89877  1.0000
-  C   C29       1.0  0.42907  0.02672  0.92135  1.0000
-  C   C30       1.0  0.40512  0.04153  0.83976  1.0000
-  C   C31       1.0  0.51727  0.27288  0.30220  1.0000
-  C   C32       1.0  0.52840  0.37437  0.32747  1.0000
-  C   C33       1.0  0.42001  0.36021  0.28827  1.0000
-  C   C34       1.0  0.44567  0.43146  0.41063  1.0000
-  C   C35       1.0  0.37312  0.31300  0.36626  1.0000
-  C   C36       1.0  0.47057  0.30972  0.39929  1.0000
-  C   C37       1.0  0.12096  0.56469  0.83275  1.0000
-  C   C38       1.0  0.20389  0.49266  0.84472  1.0000
-  C   C39       1.0  0.17534  0.51610  0.92883  1.0000
-  C   C40       1.0  0.19777  0.37149  0.90846  1.0000
-  C   C41       1.0  0.08089  0.45561  0.93423  1.0000
-  C   C42       1.0  0.09412  0.43896  0.85026  1.0000
-  C   C43       1.0  0.96771  0.18616  0.28851  1.0000
-  C   C44       1.0  0.95566  0.09363  0.33491  1.0000
-  C   C45       1.0  0.06320  0.09115  0.30922  1.0000
-  C   C46       1.0  0.02932  0.06196  0.43865  1.0000
-  C   C47       1.0  0.10624  0.16392  0.37148  1.0000
-  C   C48       1.0  0.00426  0.17415  0.39038  1.0000
-  C   C49       1.0  0.46565  0.03584  0.93990  1.0000
-  C   C50       1.0  0.61096  0.96874  0.05888  1.0000
-  C   C51       1.0  0.56993  0.98427  0.05581  1.0000
-  C   C52       1.0  0.56034  0.99045  0.02090  1.0000
-  C   C53       1.0  0.51713  0.99857  0.01466  1.0000
-  C   C54       1.0  0.51214  0.01317  0.98108  1.0000
-  C   C55       1.0  0.46910  0.01265  0.96983  1.0000
-  C   C56       1.0  0.51333  0.57455  0.57357  1.0000
-  C   C57       1.0  0.45521  0.46696  0.42726  1.0000
-  C   C58       1.0  0.45067  0.46656  0.46323  1.0000
-  C   C59       1.0  0.47381  0.49981  0.47768  1.0000
-  C   C60       1.0  0.46227  0.50866  0.51169  1.0000
-  C   C61       1.0  0.49275  0.53603  0.52653  1.0000
-  C   C62       1.0  0.47842  0.55451  0.55661  1.0000
-  C   C63       1.0  0.91094  0.52082  0.07995  1.0000
-  C   C64       1.0  0.05540  0.44777  0.96236  1.0000
-  C   C65       1.0  0.01975  0.47160  0.96680  1.0000
-  C   C66       1.0  0.00654  0.47057  0.00144  1.0000
-  C   C67       1.0  0.96465  0.48332  0.00677  1.0000
-  C   C68       1.0  0.95885  0.49434  0.04137  1.0000
-  C   C69       1.0  0.91535  0.49543  0.05131  1.0000
-  C   C70       1.0  0.03313  0.04497  0.47048  1.0000
-  C   C71       1.0  0.95892  0.90518  0.59046  1.0000
-  C   C72       1.0  0.98442  0.91126  0.56077  1.0000
-  C   C73       1.0  0.98221  0.95072  0.54888  1.0000
-  C   C74       1.0  0.99752  0.95645  0.51509  1.0000
-  C   C75       1.0  0.00757  0.99714  0.50881  1.0000
-  C   C76       1.0  0.01293  0.00670  0.47371  1.0000
-  C   C77       1.0  0.70771  0.82774  0.12237  1.0000
-  C   C78       1.0  0.74262  0.62777  0.12191  1.0000
-  C   C79       1.0  0.75969  0.66308  0.13740  1.0000
-  C   C80       1.0  0.73465  0.69496  0.12753  1.0000
-  C   C81       1.0  0.74906  0.73245  0.14062  1.0000
-  C   C82       1.0  0.72271  0.76198  0.12790  1.0000
-  C   C83       1.0  0.73322  0.80093  0.13992  1.0000
-  C   C84       1.0  0.62749  0.73950  0.60308  1.0000
-  C   C85       1.0  0.84305  0.79903  0.61051  1.0000
-  C   C86       1.0  0.80952  0.78031  0.62965  1.0000
-  C   C87       1.0  0.77130  0.77725  0.61032  1.0000
-  C   C88       1.0  0.73704  0.75812  0.62830  1.0000
-  C   C89       1.0  0.69931  0.75722  0.60836  1.0000
-  C   C90       1.0  0.66378  0.73776  0.62451  1.0000
-  C   C91       1.0  0.21749  0.33827  0.91993  1.0000
-  C   C92       1.0  0.31631  0.15933  0.90959  1.0000
-  C   C93       1.0  0.28416  0.18001  0.89254  1.0000
-  C   C94       1.0  0.28139  0.21817  0.90758  1.0000
-  C   C95       1.0  0.25112  0.24258  0.89217  1.0000
-  C   C96       1.0  0.24846  0.27829  0.91111  1.0000
-  C   C97       1.0  0.22215  0.30687  0.89631  1.0000
-  C   C98       1.0  0.33543  0.29699  0.38015  1.0000
-  C   C99       1.0  0.14280  0.18358  0.38447  1.0000
-  C   C100      1.0  0.17220  0.20073  0.36043  1.0000
-  C   C101      1.0  0.20621  0.22194  0.37795  1.0000
-  C   C102      1.0  0.23969  0.23765  0.35668  1.0000
-  C   C103      1.0  0.27081  0.25996  0.37635  1.0000
-  C   C104      1.0  0.30724  0.27489  0.35781  1.0000
-  C   C105      1.0  0.55488  0.25486  0.29665  1.0000
-  C   C106      1.0  0.66935  0.11423  0.21235  1.0000
-  C   C107      1.0  0.62834  0.12879  0.21705  1.0000
-  C   C108      1.0  0.62984  0.16105  0.23987  1.0000
-  C   C109      1.0  0.58914  0.17636  0.24408  1.0000
-  C   C110      1.0  0.59106  0.20773  0.26779  1.0000
-  C   C111      1.0  0.55099  0.22423  0.27231  1.0000
-  C   C112      1.0  0.37211  0.62926  0.73239  1.0000
-  C   C113      1.0  0.24157  0.50507  0.82945  1.0000
-  C   C114      1.0  0.23839  0.53269  0.80268  1.0000
-  C   C115      1.0  0.27927  0.55095  0.79695  1.0000
-  C   C116      1.0  0.28331  0.57017  0.76517  1.0000
-  C   C117      1.0  0.32187  0.59370  0.76446  1.0000
-  C   C118      1.0  0.33547  0.60319  0.73109  1.0000
-  C   C119      1.0  0.82356  0.35431  0.20301  1.0000
-  C   C120      1.0  0.93189  0.20022  0.27357  1.0000
-  C   C121      1.0  0.93647  0.24033  0.26406  1.0000
-  C   C122      1.0  0.89756  0.25265  0.25061  1.0000
-  C   C123      1.0  0.90094  0.29203  0.23903  1.0000
-  C   C124      1.0  0.86108  0.30372  0.22692  1.0000
-  C   C125      1.0  0.86395  0.34252  0.21397  1.0000
-  C   C126      1.0  0.25287  0.98368  0.82997  1.0000
-  C   C127      1.0  0.11380  0.86519  0.73539  1.0000
-  C   C128      1.0  0.15082  0.89007  0.73136  1.0000
-  C   C129      1.0  0.16567  0.90225  0.76389  1.0000
-  C   C130      1.0  0.20455  0.92504  0.76318  1.0000
-  C   C131      1.0  0.21211  0.94170  0.79577  1.0000
-  C   C132      1.0  0.25279  0.96098  0.79966  1.0000
-  C   C133      1.0  0.36738  0.89544  0.79666  1.0000
-  C   C134      1.0  0.44189  0.75569  0.68780  1.0000
-  C   C135      1.0  0.44419  0.76500  0.72287  1.0000
-  C   C136      1.0  0.41795  0.79715  0.72878  1.0000
-  C   C137      1.0  0.42187  0.81379  0.76173  1.0000
-  C   C138      1.0  0.39316  0.84454  0.76477  1.0000
-  C   C139      1.0  0.39716  0.86541  0.79590  1.0000
-  C   C140      1.0  0.57018  0.38696  0.32136  1.0000
-  C   C141      1.0  0.73669  0.47221  0.22779  1.0000
-  C   C142      1.0  0.69866  0.44849  0.22257  1.0000
-  C   C143      1.0  0.67696  0.44390  0.25413  1.0000
-  C   C144      1.0  0.63756  0.42150  0.25227  1.0000
-  C   C145      1.0  0.62133  0.41520  0.28562  1.0000
-  C   C146      1.0  0.57996  0.39625  0.28694  1.0000
-  C   C147      1.0  0.12475  0.59547  0.80997  1.0000
-  C   C148      1.0  0.02851  0.75510  0.73813  1.0000
-  C   C149      1.0  0.03476  0.71452  0.73245  1.0000
-  C   C150      1.0  0.06039  0.70017  0.75909  1.0000
-  C   C151      1.0  0.05785  0.65854  0.76252  1.0000
-  C   C152      1.0  0.09245  0.64636  0.78252  1.0000
-  C   C153      1.0  0.08581  0.60809  0.79651  1.0000
-  C   C154      1.0  0.74848  0.99275  0.23275  1.0000
-  C   C155      1.0  0.91478  0.07839  0.32826  1.0000
-  C   C156      1.0  0.90423  0.07078  0.29357  1.0000
-  C   C157      1.0  0.86269  0.05214  0.29198  1.0000
-  C   C158      1.0  0.84681  0.04469  0.25855  1.0000
-  C   C159      1.0  0.80649  0.02383  0.26034  1.0000
-  C   C160      1.0  0.78651  0.01663  0.22825  1.0000
-  O   O1        1.0  0.65391  0.08270  0.16238  1.0000
-  O   O2        1.0  0.67378  0.04843  0.20153  1.0000
-  O   O3        1.0  0.73027  0.95707  0.18637  1.0000
-  O   O4        1.0  0.69786  0.01269  0.19730  1.0000
-  O   O5        1.0  0.64553  0.96337  0.16442  1.0000
-  O   O6        1.0  0.60078  0.98974  0.18654  1.0000
-  O   O7        1.0  0.73246  0.89230  0.12281  1.0000
-  O   O8        1.0  0.68050  0.87907  0.15029  1.0000
-  O   O9        1.0  0.62458  0.00162  0.10750  1.0000
-  O   O10       1.0  0.65148  0.94336  0.09919  1.0000
-  O   O11       1.0  0.70814  0.00239  0.13912  1.0000
-  O   O12       1.0  0.73409  0.97552  0.10367  1.0000
-  O   O13       1.0  0.58765  0.70042  0.64035  1.0000
-  O   O14       1.0  0.55773  0.72004  0.59863  1.0000
-  O   O15       1.0  0.46946  0.59628  0.61390  1.0000
-  O   O16       1.0  0.52661  0.63240  0.59933  1.0000
-  O   O17       1.0  0.49651  0.64695  0.67228  1.0000
-  O   O18       1.0  0.55491  0.63971  0.66330  1.0000
-  O   O19       1.0  0.40680  0.60248  0.68799  1.0000
-  O   O20       1.0  0.40418  0.66253  0.68813  1.0000
-  O   O21       1.0  0.49624  0.72404  0.66667  1.0000
-  O   O22       1.0  0.43450  0.69141  0.67611  1.0000
-  O   O23       1.0  0.46002  0.67456  0.61531  1.0000
-  O   O24       1.0  0.39989  0.65982  0.60889  1.0000
-  O   O25       1.0  0.84631  0.39367  0.15962  1.0000
-  O   O26       1.0  0.81611  0.42085  0.19867  1.0000
-  O   O27       1.0  0.75555  0.50642  0.18109  1.0000
-  O   O28       1.0  0.79267  0.45562  0.19656  1.0000
-  O   O29       1.0  0.84596  0.51186  0.17285  1.0000
-  O   O30       1.0  0.88930  0.48262  0.19647  1.0000
-  O   O31       1.0  0.75099  0.56194  0.11733  1.0000
-  O   O32       1.0  0.79373  0.59132  0.14774  1.0000
-  O   O33       1.0  0.88056  0.47848  0.11660  1.0000
-  O   O34       1.0  0.85020  0.53432  0.10678  1.0000
-  O   O35       1.0  0.78968  0.46602  0.13321  1.0000
-  O   O36       1.0  0.77685  0.49804  0.09503  1.0000
-  O   O37       1.0  0.89443  0.77493  0.64467  1.0000
-  O   O38       1.0  0.90346  0.83258  0.63032  1.0000
-  O   O39       1.0  0.01034  0.87529  0.61791  1.0000
-  O   O40       1.0  0.94330  0.85477  0.62627  1.0000
-  O   O41       1.0  0.98672  0.85111  0.68447  1.0000
-  O   O42       1.0  0.93035  0.85144  0.70432  1.0000
-  O   O43       1.0  0.08224  0.88175  0.68539  1.0000
-  O   O44       1.0  0.07558  0.82437  0.69972  1.0000
-  O   O45       1.0  0.97863  0.77222  0.70107  1.0000
-  O   O46       1.0  0.04344  0.79912  0.69750  1.0000
-  O   O47       1.0  0.99717  0.80209  0.63236  1.0000
-  O   O48       1.0  0.05540  0.78841  0.62941  1.0000
-  O   O49       1.0  0.40556  0.92990  0.83746  1.0000
-  O   O50       1.0  0.34106  0.93432  0.83824  1.0000
-  O   O51       1.0  0.29711  0.02900  0.85325  1.0000
-  O   O52       1.0  0.31767  0.96759  0.84738  1.0000
-  O   O53       1.0  0.34285  0.99536  0.90676  1.0000
-  O   O54       1.0  0.34417  0.93977  0.91747  1.0000
-  O   O55       1.0  0.34114  0.11235  0.87379  1.0000
-  O   O56       1.0  0.31479  0.09266  0.91734  1.0000
-  O   O57       1.0  0.42757  0.99435  0.90665  1.0000
-  O   O58       1.0  0.40275  0.05263  0.91836  1.0000
-  O   O59       1.0  0.37747  0.01902  0.84823  1.0000
-  O   O60       1.0  0.39846  0.07223  0.85286  1.0000
-  O   O61       1.0  0.48613  0.25647  0.31524  1.0000
-  O   O62       1.0  0.51496  0.30865  0.30027  1.0000
-  O   O63       1.0  0.51052  0.39044  0.35119  1.0000
-  O   O64       1.0  0.51353  0.34444  0.31240  1.0000
-  O   O65       1.0  0.43053  0.36486  0.31783  1.0000
-  O   O66       1.0  0.42682  0.32760  0.27688  1.0000
-  O   O67       1.0  0.46250  0.40098  0.41726  1.0000
-  O   O68       1.0  0.42946  0.43044  0.38258  1.0000
-  O   O69       1.0  0.39300  0.29330  0.34592  1.0000
-  O   O70       1.0  0.38711  0.34468  0.37841  1.0000
-  O   O71       1.0  0.48006  0.31899  0.37103  1.0000
-  O   O72       1.0  0.45849  0.33804  0.41411  1.0000
-  O   O73       1.0  0.08820  0.55404  0.84714  1.0000
-  O   O74       1.0  0.15223  0.54892  0.84365  1.0000
-  O   O75       1.0  0.20296  0.45841  0.85574  1.0000
-  O   O76       1.0  0.17728  0.51800  0.85071  1.0000
-  O   O77       1.0  0.16024  0.49043  0.91125  1.0000
-  O   O78       1.0  0.15793  0.54598  0.92153  1.0000
-  O   O79       1.0  0.17347  0.37299  0.88447  1.0000
-  O   O80       1.0  0.20122  0.40243  0.92386  1.0000
-  O   O81       1.0  0.07691  0.48702  0.91863  1.0000
-  O   O82       1.0  0.10872  0.43155  0.92910  1.0000
-  O   O83       1.0  0.12121  0.46311  0.85637  1.0000
-  O   O84       1.0  0.10454  0.40942  0.86325  1.0000
-  O   O85       1.0  0.99727  0.20689  0.29975  1.0000
-  O   O86       1.0  0.97112  0.15100  0.29381  1.0000
-  O   O87       1.0  0.97148  0.08244  0.36197  1.0000
-  O   O88       1.0  0.97119  0.12014  0.31591  1.0000
-  O   O89       1.0  0.05256  0.10716  0.33434  1.0000
-  O   O90       1.0  0.05875  0.11427  0.28641  1.0000
-  O   O91       1.0  0.01121  0.09213  0.43446  1.0000
-  O   O92       1.0  0.04947  0.05320  0.41377  1.0000
-  O   O93       1.0  0.08936  0.17749  0.34562  1.0000
-  O   O94       1.0  0.09107  0.13629  0.38921  1.0000
-  O   O95       1.0  0.00245  0.15345  0.36619  1.0000
-  O   O96       1.0  0.01561  0.15452  0.41346  1.0000
+ _atom_site_type_symbol
+ _atom_site_label
+ _atom_site_symmetry_multiplicity
+ _atom_site_fract_x
+ _atom_site_fract_y
+ _atom_site_fract_z
+ _atom_site_occupancy
+  Nd  Nd0  1  0.69604000  0.94027000  0.14098000  1.0
+  Nd  Nd1  1  0.65069000  0.02063000  0.15613000  1.0
+  Nd  Nd2  1  0.43877000  0.63496000  0.64894000  1.0
+  Nd  Nd3  1  0.52174000  0.68257000  0.63232000  1.0
+  Nd  Nd4  1  0.79754000  0.52846000  0.14198000  1.0
+  Nd  Nd5  1  0.84488000  0.45579000  0.15941000  1.0
+  Nd  Nd6  1  0.04062000  0.84261000  0.65648000  1.0
+  Nd  Nd7  1  0.94701000  0.80851000  0.66546000  1.0
+  Nd  Nd8  1  0.34650000  0.05106000  0.88646000  1.0
+  Nd  Nd9  1  0.37889000  0.96688000  0.87457000  1.0
+  Nd  Nd10  1  0.44870000  0.37289000  0.36890000  1.0
+  Nd  Nd11  1  0.45404000  0.30985000  0.32343000  1.0
+  Nd  Nd12  1  0.15956000  0.43422000  0.89243000  1.0
+  Nd  Nd13  1  0.11890000  0.51607000  0.88183000  1.0
+  Nd  Nd14  1  0.03119000  0.10253000  0.38320000  1.0
+  Nd  Nd15  1  0.03049000  0.15860000  0.31941000  1.0
+  H  H16  1  0.60421000  0.93206000  0.19101000  1.0
+  H  H17  1  0.73333000  0.03313000  0.10210000  1.0
+  H  H18  1  0.52385000  0.60369000  0.69423000  1.0
+  H  H19  1  0.42856000  0.69963000  0.57923000  1.0
+  H  H20  1  0.88384000  0.53941000  0.20530000  1.0
+  H  H21  1  0.77879000  0.44096000  0.08945000  1.0
+  H  H22  1  0.97496000  0.89110000  0.71845000  1.0
+  H  H23  1  0.00980000  0.74994000  0.61596000  1.0
+  H  H24  1  0.30958000  0.97473000  0.94500000  1.0
+  H  H25  1  0.42895000  0.03590000  0.82423000  1.0
+  H  H26  1  0.40623000  0.38109000  0.27510000  1.0
+  H  H27  1  0.47969000  0.28521000  0.41040000  1.0
+  H  H28  1  0.19849000  0.51344000  0.94588000  1.0
+  H  H29  1  0.06771000  0.44275000  0.83693000  1.0
+  H  H30  1  0.07274000  0.06372000  0.30737000  1.0
+  H  H31  1  0.99809000  0.20262000  0.39109000  1.0
+  H  H32  1  0.46704000  0.06512000  0.94639000  1.0
+  H  H33  1  0.63170000  0.98466000  0.04354000  1.0
+  H  H34  1  0.56885000  0.01074000  0.06839000  1.0
+  H  H35  1  0.57970000  0.01357000  0.01239000  1.0
+  H  H36  1  0.50750000  0.01930000  0.03163000  1.0
+  H  H37  1  0.52506000  0.04153000  0.98033000  1.0
+  H  H38  1  0.45025000  0.02378000  0.98839000  1.0
+  H  H39  1  0.49072000  0.03051000  0.92424000  1.0
+  H  H40  1  0.60984000  0.94010000  0.05050000  1.0
+  H  H41  1  0.54782000  0.96476000  0.06631000  1.0
+  H  H42  1  0.56720000  0.96584000  0.00714000  1.0
+  H  H43  1  0.49864000  0.97312000  0.01786000  1.0
+  H  H44  1  0.52875000  0.99651000  0.96437000  1.0
+  H  H45  1  0.45890000  0.98390000  0.96522000  1.0
+  H  H46  1  0.53025000  0.55424000  0.58636000  1.0
+  H  H47  1  0.48631000  0.47457000  0.42152000  1.0
+  H  H48  1  0.46212000  0.44127000  0.47323000  1.0
+  H  H49  1  0.50562000  0.49444000  0.47682000  1.0
+  H  H50  1  0.46078000  0.48338000  0.52595000  1.0
+  H  H51  1  0.51969000  0.52132000  0.53190000  1.0
+  H  H52  1  0.46468000  0.53380000  0.57264000  1.0
+  H  H53  1  0.53333000  0.58803000  0.55613000  1.0
+  H  H54  1  0.43691000  0.48825000  0.41721000  1.0
+  H  H55  1  0.41901000  0.46752000  0.46906000  1.0
+  H  H56  1  0.46919000  0.52438000  0.46319000  1.0
+  H  H57  1  0.43283000  0.52034000  0.51150000  1.0
+  H  H58  1  0.50079000  0.55783000  0.50932000  1.0
+  H  H59  1  0.45594000  0.57409000  0.55004000  1.0
+  H  H60  1  0.93788000  0.52016000  0.09471000  1.0
+  H  H61  1  0.04527000  0.41864000  0.96170000  1.0
+  H  H62  1  0.99551000  0.46116000  0.95120000  1.0
+  H  H63  1  0.00762000  0.44232000  0.01059000  1.0
+  H  H64  1  0.94323000  0.46080000  0.00018000  1.0
+  H  H65  1  0.97331000  0.47491000  0.05712000  1.0
+  H  H66  1  0.90433000  0.46715000  0.05673000  1.0
+  H  H67  1  0.90801000  0.54915000  0.07171000  1.0
+  H  H68  1  0.07519000  0.45104000  0.98309000  1.0
+  H  H69  1  0.02734000  0.50041000  0.96048000  1.0
+  H  H70  1  0.02801000  0.48798000  0.01523000  1.0
+  H  H71  1  0.95929000  0.50716000  0.99164000  1.0
+  H  H72  1  0.97391000  0.52159000  0.04491000  1.0
+  H  H73  1  0.89735000  0.50556000  0.03169000  1.0
+  H  H74  1  0.02041000  0.06361000  0.48787000  1.0
+  H  H75  1  0.92776000  0.89976000  0.58356000  1.0
+  H  H76  1  0.97378000  0.89172000  0.54232000  1.0
+  H  H77  1  0.95126000  0.95888000  0.54959000  1.0
+  H  H78  1  0.97453000  0.94600000  0.49834000  1.0
+  H  H79  1  0.98386000  0.01369000  0.51828000  1.0
+  H  H80  1  0.98359000  0.00580000  0.46216000  1.0
+  H  H81  1  0.06484000  0.04294000  0.47576000  1.0
+  H  H82  1  0.96061000  0.93046000  0.60486000  1.0
+  H  H83  1  0.01576000  0.90626000  0.56568000  1.0
+  H  H84  1  0.99958000  0.96877000  0.56536000  1.0
+  H  H85  1  0.02435000  0.94103000  0.51146000  1.0
+  H  H86  1  0.03505000  0.00493000  0.52189000  1.0
+  H  H87  1  0.03125000  0.98649000  0.46208000  1.0
+  H  H88  1  0.71670000  0.82846000  0.09735000  1.0
+  H  H89  1  0.74252000  0.63093000  0.09600000  1.0
+  H  H90  1  0.79051000  0.66848000  0.12968000  1.0
+  H  H91  1  0.73427000  0.69641000  0.10144000  1.0
+  H  H92  1  0.77984000  0.73863000  0.13315000  1.0
+  H  H93  1  0.72448000  0.76185000  0.10182000  1.0
+  H  H94  1  0.76473000  0.80816000  0.13547000  1.0
+  H  H95  1  0.67652000  0.81747000  0.12365000  1.0
+  H  H96  1  0.71148000  0.62300000  0.12897000  1.0
+  H  H97  1  0.75914000  0.66024000  0.16337000  1.0
+  H  H98  1  0.70397000  0.68906000  0.13551000  1.0
+  H  H99  1  0.74783000  0.73204000  0.16667000  1.0
+  H  H100  1  0.69175000  0.75468000  0.13444000  1.0
+  H  H101  1  0.72766000  0.80230000  0.16558000  1.0
+  H  H102  1  0.62075000  0.76834000  0.59905000  1.0
+  H  H103  1  0.83487000  0.82659000  0.60312000  1.0
+  H  H104  1  0.80457000  0.79639000  0.65130000  1.0
+  H  H105  1  0.76305000  0.80508000  0.60365000  1.0
+  H  H106  1  0.73205000  0.77300000  0.65055000  1.0
+  H  H107  1  0.69203000  0.78570000  0.60297000  1.0
+  H  H108  1  0.65799000  0.75133000  0.64725000  1.0
+  H  H109  1  0.63403000  0.72782000  0.57972000  1.0
+  H  H110  1  0.84820000  0.78239000  0.58930000  1.0
+  H  H111  1  0.81775000  0.75256000  0.63661000  1.0
+  H  H112  1  0.77659000  0.76169000  0.58845000  1.0
+  H  H113  1  0.74458000  0.72981000  0.63396000  1.0
+  H  H114  1  0.70487000  0.74311000  0.58580000  1.0
+  H  H115  1  0.67021000  0.70888000  0.62898000  1.0
+  H  H116  1  0.20040000  0.32767000  0.94035000  1.0
+  H  H117  1  0.30980000  0.15866000  0.93511000  1.0
+  H  H118  1  0.25542000  0.16462000  0.89471000  1.0
+  H  H119  1  0.27375000  0.21452000  0.93278000  1.0
+  H  H120  1  0.22181000  0.22797000  0.89170000  1.0
+  H  H121  1  0.23713000  0.27118000  0.93488000  1.0
+  H  H122  1  0.19279000  0.29409000  0.89051000  1.0
+  H  H123  1  0.24678000  0.34768000  0.92920000  1.0
+  H  H124  1  0.34485000  0.17460000  0.90597000  1.0
+  H  H125  1  0.29156000  0.18289000  0.86726000  1.0
+  H  H126  1  0.31078000  0.23265000  0.90645000  1.0
+  H  H127  1  0.26024000  0.24895000  0.86772000  1.0
+  H  H128  1  0.27852000  0.29106000  0.91408000  1.0
+  H  H129  1  0.23606000  0.31755000  0.87444000  1.0
+  H  H130  1  0.31950000  0.31943000  0.39098000  1.0
+  H  H131  1  0.13259000  0.20557000  0.39985000  1.0
+  H  H132  1  0.15700000  0.21975000  0.34482000  1.0
+  H  H133  1  0.19365000  0.24472000  0.39115000  1.0
+  H  H134  1  0.22725000  0.25554000  0.33860000  1.0
+  H  H135  1  0.25636000  0.28333000  0.38720000  1.0
+  H  H136  1  0.29767000  0.29276000  0.33853000  1.0
+  H  H137  1  0.34415000  0.27876000  0.39942000  1.0
+  H  H138  1  0.15827000  0.16441000  0.39971000  1.0
+  H  H139  1  0.18422000  0.17883000  0.34586000  1.0
+  H  H140  1  0.21917000  0.20345000  0.39535000  1.0
+  H  H141  1  0.25386000  0.21487000  0.34477000  1.0
+  H  H142  1  0.28113000  0.24249000  0.39567000  1.0
+  H  H143  1  0.32261000  0.25177000  0.34749000  1.0
+  H  H144  1  0.56433000  0.24320000  0.31932000  1.0
+  H  H145  1  0.68212000  0.10681000  0.23535000  1.0
+  H  H146  1  0.60816000  0.10681000  0.22656000  1.0
+  H  H147  1  0.64093000  0.15195000  0.26300000  1.0
+  H  H148  1  0.56821000  0.15447000  0.25262000  1.0
+  H  H149  1  0.60152000  0.19746000  0.29074000  1.0
+  H  H150  1  0.52924000  0.20282000  0.28048000  1.0
+  H  H151  1  0.57747000  0.27575000  0.28893000  1.0
+  H  H152  1  0.68835000  0.13556000  0.20082000  1.0
+  H  H153  1  0.61650000  0.13763000  0.19407000  1.0
+  H  H154  1  0.65048000  0.18284000  0.23072000  1.0
+  H  H155  1  0.57850000  0.18636000  0.22111000  1.0
+  H  H156  1  0.61255000  0.22930000  0.25947000  1.0
+  H  H157  1  0.54076000  0.23528000  0.24958000  1.0
+  H  H158  1  0.36383000  0.65685000  0.73967000  1.0
+  H  H159  1  0.25999000  0.51767000  0.84857000  1.0
+  H  H160  1  0.21787000  0.55414000  0.80875000  1.0
+  H  H161  1  0.28566000  0.57090000  0.81623000  1.0
+  H  H162  1  0.25822000  0.58780000  0.76125000  1.0
+  H  H163  1  0.31769000  0.61916000  0.77793000  1.0
+  H  H164  1  0.31169000  0.61634000  0.71807000  1.0
+  H  H165  1  0.39315000  0.61899000  0.74985000  1.0
+  H  H166  1  0.25680000  0.48101000  0.82082000  1.0
+  H  H167  1  0.22737000  0.51822000  0.78121000  1.0
+  H  H168  1  0.30186000  0.53013000  0.79801000  1.0
+  H  H169  1  0.28316000  0.54915000  0.74635000  1.0
+  H  H170  1  0.34561000  0.57895000  0.77617000  1.0
+  H  H171  1  0.34219000  0.57755000  0.71874000  1.0
+  H  H172  1  0.81099000  0.33394000  0.18601000  1.0
+  H  H173  1  0.92423000  0.18298000  0.25277000  1.0
+  H  H174  1  0.95994000  0.24374000  0.24611000  1.0
+  H  H175  1  0.88829000  0.23456000  0.23068000  1.0
+  H  H176  1  0.92287000  0.29425000  0.21980000  1.0
+  H  H177  1  0.85053000  0.28480000  0.20792000  1.0
+  H  H178  1  0.88488000  0.34347000  0.19397000  1.0
+  H  H179  1  0.80383000  0.35660000  0.22350000  1.0
+  H  H180  1  0.90744000  0.19634000  0.29056000  1.0
+  H  H181  1  0.94481000  0.25733000  0.28491000  1.0
+  H  H182  1  0.87472000  0.25019000  0.26915000  1.0
+  H  H183  1  0.91101000  0.31027000  0.25863000  1.0
+  H  H184  1  0.83948000  0.30222000  0.24640000  1.0
+  H  H185  1  0.87558000  0.36156000  0.23251000  1.0
+  H  H186  1  0.23582000  0.00826000  0.82615000  1.0
+  H  H187  1  0.09280000  0.87895000  0.75074000  1.0
+  H  H188  1  0.14404000  0.91447000  0.71735000  1.0
+  H  H189  1  0.14270000  0.91849000  0.77495000  1.0
+  H  H190  1  0.20287000  0.94726000  0.74566000  1.0
+  H  H191  1  0.18908000  0.96147000  0.80029000  1.0
+  H  H192  1  0.25929000  0.97930000  0.77945000  1.0
+  H  H193  1  0.23801000  0.96730000  0.84878000  1.0
+  H  H194  1  0.12135000  0.83935000  0.74688000  1.0
+  H  H195  1  0.17367000  0.87497000  0.71905000  1.0
+  H  H196  1  0.16972000  0.87784000  0.77873000  1.0
+  H  H197  1  0.22875000  0.90735000  0.75670000  1.0
+  H  H198  1  0.20915000  0.91990000  0.81381000  1.0
+  H  H199  1  0.27524000  0.94010000  0.80061000  1.0
+  H  H200  1  0.37209000  0.91336000  0.77593000  1.0
+  H  H201  1  0.45665000  0.77844000  0.67453000  1.0
+  H  H202  1  0.47511000  0.77266000  0.72940000  1.0
+  H  H203  1  0.42535000  0.81899000  0.71141000  1.0
+  H  H204  1  0.45247000  0.82491000  0.76536000  1.0
+  H  H205  1  0.39846000  0.86419000  0.74523000  1.0
+  H  H206  1  0.42754000  0.87767000  0.79806000  1.0
+  H  H207  1  0.33693000  0.88330000  0.79542000  1.0
+  H  H208  1  0.41048000  0.75353000  0.68053000  1.0
+  H  H209  1  0.43364000  0.74124000  0.73714000  1.0
+  H  H210  1  0.38684000  0.78760000  0.72478000  1.0
+  H  H211  1  0.41493000  0.79256000  0.77965000  1.0
+  H  H212  1  0.36262000  0.83270000  0.76249000  1.0
+  H  H213  1  0.39153000  0.84637000  0.81578000  1.0
+  H  H214  1  0.58900000  0.36472000  0.32880000  1.0
+  H  H215  1  0.75442000  0.45943000  0.24631000  1.0
+  H  H216  1  0.70591000  0.42130000  0.21342000  1.0
+  H  H217  1  0.69666000  0.43051000  0.27096000  1.0
+  H  H218  1  0.64206000  0.39477000  0.24099000  1.0
+  H  H219  1  0.64217000  0.39845000  0.29874000  1.0
+  H  H220  1  0.57907000  0.37084000  0.27269000  1.0
+  H  H221  1  0.57743000  0.41108000  0.33647000  1.0
+  H  H222  1  0.72857000  0.49949000  0.23607000  1.0
+  H  H223  1  0.67955000  0.46176000  0.20527000  1.0
+  H  H224  1  0.67125000  0.47135000  0.26362000  1.0
+  H  H225  1  0.61631000  0.43650000  0.23805000  1.0
+  H  H226  1  0.62026000  0.44192000  0.29784000  1.0
+  H  H227  1  0.55817000  0.41481000  0.27731000  1.0
+  H  H228  1  0.14439000  0.58772000  0.79062000  1.0
+  H  H229  1  0.05613000  0.76868000  0.74729000  1.0
+  H  H230  1  0.04986000  0.71052000  0.70969000  1.0
+  H  H231  1  0.09131000  0.70981000  0.75459000  1.0
+  H  H232  1  0.05888000  0.64530000  0.73908000  1.0
+  H  H233  1  0.11911000  0.64732000  0.76752000  1.0
+  H  H234  1  0.07497000  0.58853000  0.77814000  1.0
+  H  H235  1  0.14035000  0.61833000  0.82275000  1.0
+  H  H236  1  0.00535000  0.75725000  0.75618000  1.0
+  H  H237  1  0.00577000  0.69930000  0.73169000  1.0
+  H  H238  1  0.05153000  0.71199000  0.78192000  1.0
+  H  H239  1  0.02952000  0.65025000  0.77388000  1.0
+  H  H240  1  0.09800000  0.66576000  0.80235000  1.0
+  H  H241  1  0.06333000  0.60924000  0.81528000  1.0
+  H  H242  1  0.75637000  0.96566000  0.24155000  1.0
+  H  H243  1  0.91004000  0.05291000  0.34201000  1.0
+  H  H244  1  0.92572000  0.05255000  0.28311000  1.0
+  H  H245  1  0.86319000  0.02583000  0.30477000  1.0
+  H  H246  1  0.86762000  0.02811000  0.24539000  1.0
+  H  H247  1  0.81047000  0.99729000  0.27211000  1.0
+  H  H248  1  0.80672000  0.00245000  0.21248000  1.0
+  H  H249  1  0.72993000  0.00595000  0.25041000  1.0
+  H  H250  1  0.89435000  0.09836000  0.33755000  1.0
+  H  H251  1  0.90485000  0.09676000  0.28027000  1.0
+  H  H252  1  0.84195000  0.06962000  0.30436000  1.0
+  H  H253  1  0.84371000  0.07096000  0.24619000  1.0
+  H  H254  1  0.78654000  0.03967000  0.27508000  1.0
+  H  H255  1  0.77959000  0.04307000  0.21743000  1.0
+  C  C256  1  0.66676000  0.08157000  0.19158000  1.0
+  C  C257  1  0.72478000  0.98751000  0.20323000  1.0
+  C  C258  1  0.61524000  0.95791000  0.18192000  1.0
+  C  C259  1  0.70966000  0.86606000  0.13472000  1.0
+  C  C260  1  0.62863000  0.97073000  0.09118000  1.0
+  C  C261  1  0.72637000  0.00745000  0.11341000  1.0
+  C  C262  1  0.59073000  0.72000000  0.61463000  1.0
+  C  C263  1  0.50203000  0.60283000  0.59682000  1.0
+  C  C264  1  0.52478000  0.62652000  0.67839000  1.0
+  C  C265  1  0.39317000  0.63135000  0.70181000  1.0
+  C  C266  1  0.45974000  0.72098000  0.67849000  1.0
+  C  C267  1  0.42949000  0.68054000  0.59834000  1.0
+  C  C268  1  0.82788000  0.38994000  0.18664000  1.0
+  C  C269  1  0.76193000  0.47738000  0.19921000  1.0
+  C  C270  1  0.87423000  0.51471000  0.19326000  1.0
+  C  C271  1  0.76312000  0.59361000  0.12913000  1.0
+  C  C272  1  0.87746000  0.50991000  0.10122000  1.0
+  C  C273  1  0.78248000  0.46516000  0.10371000  1.0
+  C  C274  1  0.88073000  0.80222000  0.62870000  1.0
+  C  C275  1  0.97179000  0.87559000  0.61184000  1.0
+  C  C276  1  0.96552000  0.86775000  0.70448000  1.0
+  C  C277  1  0.09272000  0.85677000  0.70539000  1.0
+  C  C278  1  0.01637000  0.77521000  0.70951000  1.0
+  C  C279  1  0.01939000  0.77618000  0.62529000  1.0
+  C  C280  1  0.37141000  0.91918000  0.82506000  1.0
+  C  C281  1  0.29255000  0.99451000  0.84272000  1.0
+  C  C282  1  0.32954000  0.97065000  0.92591000  1.0
+  C  C283  1  0.32105000  0.12081000  0.89877000  1.0
+  C  C284  1  0.42907000  0.02672000  0.92135000  1.0
+  C  C285  1  0.40512000  0.04153000  0.83976000  1.0
+  C  C286  1  0.51727000  0.27288000  0.30220000  1.0
+  C  C287  1  0.52840000  0.37437000  0.32747000  1.0
+  C  C288  1  0.42001000  0.36021000  0.28827000  1.0
+  C  C289  1  0.44567000  0.43146000  0.41063000  1.0
+  C  C290  1  0.37312000  0.31300000  0.36626000  1.0
+  C  C291  1  0.47057000  0.30972000  0.39929000  1.0
+  C  C292  1  0.12096000  0.56469000  0.83275000  1.0
+  C  C293  1  0.20389000  0.49266000  0.84472000  1.0
+  C  C294  1  0.17534000  0.51610000  0.92883000  1.0
+  C  C295  1  0.19777000  0.37149000  0.90846000  1.0
+  C  C296  1  0.08089000  0.45561000  0.93423000  1.0
+  C  C297  1  0.09412000  0.43896000  0.85026000  1.0
+  C  C298  1  0.96771000  0.18616000  0.28851000  1.0
+  C  C299  1  0.95566000  0.09363000  0.33491000  1.0
+  C  C300  1  0.06320000  0.09115000  0.30922000  1.0
+  C  C301  1  0.02932000  0.06196000  0.43865000  1.0
+  C  C302  1  0.10624000  0.16392000  0.37148000  1.0
+  C  C303  1  0.00426000  0.17415000  0.39038000  1.0
+  C  C304  1  0.46565000  0.03584000  0.93990000  1.0
+  C  C305  1  0.61096000  0.96874000  0.05888000  1.0
+  C  C306  1  0.56993000  0.98427000  0.05581000  1.0
+  C  C307  1  0.56034000  0.99045000  0.02090000  1.0
+  C  C308  1  0.51713000  0.99857000  0.01466000  1.0
+  C  C309  1  0.51214000  0.01317000  0.98108000  1.0
+  C  C310  1  0.46910000  0.01265000  0.96983000  1.0
+  C  C311  1  0.51333000  0.57455000  0.57357000  1.0
+  C  C312  1  0.45521000  0.46696000  0.42726000  1.0
+  C  C313  1  0.45067000  0.46656000  0.46323000  1.0
+  C  C314  1  0.47381000  0.49981000  0.47768000  1.0
+  C  C315  1  0.46227000  0.50866000  0.51169000  1.0
+  C  C316  1  0.49275000  0.53603000  0.52653000  1.0
+  C  C317  1  0.47842000  0.55451000  0.55661000  1.0
+  C  C318  1  0.91094000  0.52082000  0.07995000  1.0
+  C  C319  1  0.05540000  0.44777000  0.96236000  1.0
+  C  C320  1  0.01975000  0.47160000  0.96680000  1.0
+  C  C321  1  0.00654000  0.47057000  0.00144000  1.0
+  C  C322  1  0.96465000  0.48332000  0.00677000  1.0
+  C  C323  1  0.95885000  0.49434000  0.04137000  1.0
+  C  C324  1  0.91535000  0.49543000  0.05131000  1.0
+  C  C325  1  0.03313000  0.04497000  0.47048000  1.0
+  C  C326  1  0.95892000  0.90518000  0.59046000  1.0
+  C  C327  1  0.98442000  0.91126000  0.56077000  1.0
+  C  C328  1  0.98221000  0.95072000  0.54888000  1.0
+  C  C329  1  0.99752000  0.95645000  0.51509000  1.0
+  C  C330  1  0.00757000  0.99714000  0.50881000  1.0
+  C  C331  1  0.01293000  0.00670000  0.47371000  1.0
+  C  C332  1  0.70771000  0.82774000  0.12237000  1.0
+  C  C333  1  0.74262000  0.62777000  0.12191000  1.0
+  C  C334  1  0.75969000  0.66308000  0.13740000  1.0
+  C  C335  1  0.73465000  0.69496000  0.12753000  1.0
+  C  C336  1  0.74906000  0.73245000  0.14062000  1.0
+  C  C337  1  0.72271000  0.76198000  0.12790000  1.0
+  C  C338  1  0.73322000  0.80093000  0.13992000  1.0
+  C  C339  1  0.62749000  0.73950000  0.60308000  1.0
+  C  C340  1  0.84305000  0.79903000  0.61051000  1.0
+  C  C341  1  0.80952000  0.78031000  0.62965000  1.0
+  C  C342  1  0.77130000  0.77725000  0.61032000  1.0
+  C  C343  1  0.73704000  0.75812000  0.62830000  1.0
+  C  C344  1  0.69931000  0.75722000  0.60836000  1.0
+  C  C345  1  0.66378000  0.73776000  0.62451000  1.0
+  C  C346  1  0.21749000  0.33827000  0.91993000  1.0
+  C  C347  1  0.31631000  0.15933000  0.90959000  1.0
+  C  C348  1  0.28416000  0.18001000  0.89254000  1.0
+  C  C349  1  0.28139000  0.21817000  0.90758000  1.0
+  C  C350  1  0.25112000  0.24258000  0.89217000  1.0
+  C  C351  1  0.24846000  0.27829000  0.91111000  1.0
+  C  C352  1  0.22215000  0.30687000  0.89631000  1.0
+  C  C353  1  0.33543000  0.29699000  0.38015000  1.0
+  C  C354  1  0.14280000  0.18358000  0.38447000  1.0
+  C  C355  1  0.17220000  0.20073000  0.36043000  1.0
+  C  C356  1  0.20621000  0.22194000  0.37795000  1.0
+  C  C357  1  0.23969000  0.23765000  0.35668000  1.0
+  C  C358  1  0.27081000  0.25996000  0.37635000  1.0
+  C  C359  1  0.30724000  0.27489000  0.35781000  1.0
+  C  C360  1  0.55488000  0.25486000  0.29665000  1.0
+  C  C361  1  0.66935000  0.11423000  0.21235000  1.0
+  C  C362  1  0.62834000  0.12879000  0.21705000  1.0
+  C  C363  1  0.62984000  0.16105000  0.23987000  1.0
+  C  C364  1  0.58914000  0.17636000  0.24408000  1.0
+  C  C365  1  0.59106000  0.20773000  0.26779000  1.0
+  C  C366  1  0.55099000  0.22423000  0.27231000  1.0
+  C  C367  1  0.37211000  0.62926000  0.73239000  1.0
+  C  C368  1  0.24157000  0.50507000  0.82945000  1.0
+  C  C369  1  0.23839000  0.53269000  0.80268000  1.0
+  C  C370  1  0.27927000  0.55095000  0.79695000  1.0
+  C  C371  1  0.28331000  0.57017000  0.76517000  1.0
+  C  C372  1  0.32187000  0.59370000  0.76446000  1.0
+  C  C373  1  0.33547000  0.60319000  0.73109000  1.0
+  C  C374  1  0.82356000  0.35431000  0.20301000  1.0
+  C  C375  1  0.93189000  0.20022000  0.27357000  1.0
+  C  C376  1  0.93647000  0.24033000  0.26406000  1.0
+  C  C377  1  0.89756000  0.25265000  0.25061000  1.0
+  C  C378  1  0.90094000  0.29203000  0.23903000  1.0
+  C  C379  1  0.86108000  0.30372000  0.22692000  1.0
+  C  C380  1  0.86395000  0.34252000  0.21397000  1.0
+  C  C381  1  0.25287000  0.98368000  0.82997000  1.0
+  C  C382  1  0.11380000  0.86519000  0.73539000  1.0
+  C  C383  1  0.15082000  0.89007000  0.73136000  1.0
+  C  C384  1  0.16567000  0.90225000  0.76389000  1.0
+  C  C385  1  0.20455000  0.92504000  0.76318000  1.0
+  C  C386  1  0.21211000  0.94170000  0.79577000  1.0
+  C  C387  1  0.25279000  0.96098000  0.79966000  1.0
+  C  C388  1  0.36738000  0.89544000  0.79666000  1.0
+  C  C389  1  0.44189000  0.75569000  0.68780000  1.0
+  C  C390  1  0.44419000  0.76500000  0.72287000  1.0
+  C  C391  1  0.41795000  0.79715000  0.72878000  1.0
+  C  C392  1  0.42187000  0.81379000  0.76173000  1.0
+  C  C393  1  0.39316000  0.84454000  0.76477000  1.0
+  C  C394  1  0.39716000  0.86541000  0.79590000  1.0
+  C  C395  1  0.57018000  0.38696000  0.32136000  1.0
+  C  C396  1  0.73669000  0.47221000  0.22779000  1.0
+  C  C397  1  0.69866000  0.44849000  0.22257000  1.0
+  C  C398  1  0.67696000  0.44390000  0.25413000  1.0
+  C  C399  1  0.63756000  0.42150000  0.25227000  1.0
+  C  C400  1  0.62133000  0.41520000  0.28562000  1.0
+  C  C401  1  0.57996000  0.39625000  0.28694000  1.0
+  C  C402  1  0.12475000  0.59547000  0.80997000  1.0
+  C  C403  1  0.02851000  0.75510000  0.73813000  1.0
+  C  C404  1  0.03476000  0.71452000  0.73245000  1.0
+  C  C405  1  0.06039000  0.70017000  0.75909000  1.0
+  C  C406  1  0.05785000  0.65854000  0.76252000  1.0
+  C  C407  1  0.09245000  0.64636000  0.78252000  1.0
+  C  C408  1  0.08581000  0.60809000  0.79651000  1.0
+  C  C409  1  0.74848000  0.99275000  0.23275000  1.0
+  C  C410  1  0.91478000  0.07839000  0.32826000  1.0
+  C  C411  1  0.90423000  0.07078000  0.29357000  1.0
+  C  C412  1  0.86269000  0.05214000  0.29198000  1.0
+  C  C413  1  0.84681000  0.04469000  0.25855000  1.0
+  C  C414  1  0.80649000  0.02383000  0.26034000  1.0
+  C  C415  1  0.78651000  0.01663000  0.22825000  1.0
+  O  O416  1  0.65391000  0.08270000  0.16238000  1.0
+  O  O417  1  0.67378000  0.04843000  0.20153000  1.0
+  O  O418  1  0.73027000  0.95707000  0.18637000  1.0
+  O  O419  1  0.69786000  0.01269000  0.19730000  1.0
+  O  O420  1  0.64553000  0.96337000  0.16442000  1.0
+  O  O421  1  0.60078000  0.98974000  0.18654000  1.0
+  O  O422  1  0.73246000  0.89230000  0.12281000  1.0
+  O  O423  1  0.68050000  0.87907000  0.15029000  1.0
+  O  O424  1  0.62458000  0.00162000  0.10750000  1.0
+  O  O425  1  0.65148000  0.94336000  0.09919000  1.0
+  O  O426  1  0.70814000  0.00239000  0.13912000  1.0
+  O  O427  1  0.73409000  0.97552000  0.10367000  1.0
+  O  O428  1  0.58765000  0.70042000  0.64035000  1.0
+  O  O429  1  0.55773000  0.72004000  0.59863000  1.0
+  O  O430  1  0.46946000  0.59628000  0.61390000  1.0
+  O  O431  1  0.52661000  0.63240000  0.59933000  1.0
+  O  O432  1  0.49651000  0.64695000  0.67228000  1.0
+  O  O433  1  0.55491000  0.63971000  0.66330000  1.0
+  O  O434  1  0.40680000  0.60248000  0.68799000  1.0
+  O  O435  1  0.40418000  0.66253000  0.68813000  1.0
+  O  O436  1  0.49624000  0.72404000  0.66666667  1.0
+  O  O437  1  0.43450000  0.69141000  0.67611000  1.0
+  O  O438  1  0.46002000  0.67456000  0.61531000  1.0
+  O  O439  1  0.39989000  0.65982000  0.60889000  1.0
+  O  O440  1  0.84631000  0.39367000  0.15962000  1.0
+  O  O441  1  0.81611000  0.42085000  0.19867000  1.0
+  O  O442  1  0.75555000  0.50642000  0.18109000  1.0
+  O  O443  1  0.79267000  0.45562000  0.19656000  1.0
+  O  O444  1  0.84596000  0.51186000  0.17285000  1.0
+  O  O445  1  0.88930000  0.48262000  0.19647000  1.0
+  O  O446  1  0.75099000  0.56194000  0.11733000  1.0
+  O  O447  1  0.79373000  0.59132000  0.14774000  1.0
+  O  O448  1  0.88056000  0.47848000  0.11660000  1.0
+  O  O449  1  0.85020000  0.53432000  0.10678000  1.0
+  O  O450  1  0.78968000  0.46602000  0.13321000  1.0
+  O  O451  1  0.77685000  0.49804000  0.09503000  1.0
+  O  O452  1  0.89443000  0.77493000  0.64467000  1.0
+  O  O453  1  0.90346000  0.83258000  0.63032000  1.0
+  O  O454  1  0.01034000  0.87529000  0.61791000  1.0
+  O  O455  1  0.94330000  0.85477000  0.62627000  1.0
+  O  O456  1  0.98672000  0.85111000  0.68447000  1.0
+  O  O457  1  0.93035000  0.85144000  0.70432000  1.0
+  O  O458  1  0.08224000  0.88175000  0.68539000  1.0
+  O  O459  1  0.07558000  0.82437000  0.69972000  1.0
+  O  O460  1  0.97863000  0.77222000  0.70107000  1.0
+  O  O461  1  0.04344000  0.79912000  0.69750000  1.0
+  O  O462  1  0.99717000  0.80209000  0.63236000  1.0
+  O  O463  1  0.05540000  0.78841000  0.62941000  1.0
+  O  O464  1  0.40556000  0.92990000  0.83746000  1.0
+  O  O465  1  0.34106000  0.93432000  0.83824000  1.0
+  O  O466  1  0.29711000  0.02900000  0.85325000  1.0
+  O  O467  1  0.31767000  0.96759000  0.84738000  1.0
+  O  O468  1  0.34285000  0.99536000  0.90676000  1.0
+  O  O469  1  0.34417000  0.93977000  0.91747000  1.0
+  O  O470  1  0.34114000  0.11235000  0.87379000  1.0
+  O  O471  1  0.31479000  0.09266000  0.91734000  1.0
+  O  O472  1  0.42757000  0.99435000  0.90665000  1.0
+  O  O473  1  0.40275000  0.05263000  0.91836000  1.0
+  O  O474  1  0.37747000  0.01902000  0.84823000  1.0
+  O  O475  1  0.39846000  0.07223000  0.85286000  1.0
+  O  O476  1  0.48613000  0.25647000  0.31524000  1.0
+  O  O477  1  0.51496000  0.30865000  0.30027000  1.0
+  O  O478  1  0.51052000  0.39044000  0.35119000  1.0
+  O  O479  1  0.51353000  0.34444000  0.31240000  1.0
+  O  O480  1  0.43053000  0.36486000  0.31783000  1.0
+  O  O481  1  0.42682000  0.32760000  0.27688000  1.0
+  O  O482  1  0.46250000  0.40098000  0.41726000  1.0
+  O  O483  1  0.42946000  0.43044000  0.38258000  1.0
+  O  O484  1  0.39300000  0.29330000  0.34592000  1.0
+  O  O485  1  0.38711000  0.34468000  0.37841000  1.0
+  O  O486  1  0.48006000  0.31899000  0.37103000  1.0
+  O  O487  1  0.45849000  0.33804000  0.41411000  1.0
+  O  O488  1  0.08820000  0.55404000  0.84714000  1.0
+  O  O489  1  0.15223000  0.54892000  0.84365000  1.0
+  O  O490  1  0.20296000  0.45841000  0.85574000  1.0
+  O  O491  1  0.17728000  0.51800000  0.85071000  1.0
+  O  O492  1  0.16024000  0.49043000  0.91125000  1.0
+  O  O493  1  0.15793000  0.54598000  0.92153000  1.0
+  O  O494  1  0.17347000  0.37299000  0.88447000  1.0
+  O  O495  1  0.20122000  0.40243000  0.92386000  1.0
+  O  O496  1  0.07691000  0.48702000  0.91863000  1.0
+  O  O497  1  0.10872000  0.43155000  0.92910000  1.0
+  O  O498  1  0.12121000  0.46311000  0.85637000  1.0
+  O  O499  1  0.10454000  0.40942000  0.86325000  1.0
+  O  O500  1  0.99727000  0.20689000  0.29975000  1.0
+  O  O501  1  0.97112000  0.15100000  0.29381000  1.0
+  O  O502  1  0.97148000  0.08244000  0.36197000  1.0
+  O  O503  1  0.97119000  0.12014000  0.31591000  1.0
+  O  O504  1  0.05256000  0.10716000  0.33434000  1.0
+  O  O505  1  0.05875000  0.11427000  0.28641000  1.0
+  O  O506  1  0.01121000  0.09213000  0.43446000  1.0
+  O  O507  1  0.04947000  0.05320000  0.41377000  1.0
+  O  O508  1  0.08936000  0.17749000  0.34562000  1.0
+  O  O509  1  0.09107000  0.13629000  0.38921000  1.0
+  O  O510  1  0.00245000  0.15345000  0.36619000  1.0
+  O  O511  1  0.01561000  0.15452000  0.41346000  1.0
```

### Comparing `moftransformer-2.0.0/moftransformer/examples/dataset/train/ukg+N387+E203.cif` & `moftransformer-2.0.1/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif`

 * *Files 25% similar despite different names*

```diff
@@ -1,537 +1,578 @@
-data_image0
-_chemical_formula_structural       Nd16H240C160O96
-_chemical_formula_sum              "Nd16 H240 C160 O96"
-_cell_length_a       34.1054
-_cell_length_b       36.7791
-_cell_length_c       42.6074
-_cell_angle_alpha    90.155
-_cell_angle_beta     90.263
-_cell_angle_gamma    92.855
-
-_space_group_name_H-M_alt    "P 1"
-_space_group_IT_number       1
-
+# generated using pymatgen
+data_NaCdH50C71O15
+_symmetry_space_group_name_H-M   'P 1'
+_cell_length_a   25.67190000
+_cell_length_b   36.74890000
+_cell_length_c   37.72950000
+_cell_angle_alpha   88.51300000
+_cell_angle_beta   89.79300000
+_cell_angle_gamma   85.69100000
+_symmetry_Int_Tables_number   1
+_chemical_formula_structural   NaCdH50C71O15
+_chemical_formula_sum   'Na4 Cd4 H200 C284 O60'
+_cell_volume   35481.92585124
+_cell_formula_units_Z   4
 loop_
-  _space_group_symop_operation_xyz
-  'x, y, z'
-
+ _symmetry_equiv_pos_site_id
+ _symmetry_equiv_pos_as_xyz
+  1  'x, y, z'
 loop_
-  _atom_site_type_symbol
-  _atom_site_label
-  _atom_site_symmetry_multiplicity
-  _atom_site_fract_x
-  _atom_site_fract_y
-  _atom_site_fract_z
-  _atom_site_occupancy
-  Nd  Nd1       1.0  0.69604  0.94027  0.14098  1.0000
-  Nd  Nd2       1.0  0.65069  0.02063  0.15613  1.0000
-  Nd  Nd3       1.0  0.43877  0.63496  0.64894  1.0000
-  Nd  Nd4       1.0  0.52174  0.68257  0.63232  1.0000
-  Nd  Nd5       1.0  0.79754  0.52846  0.14198  1.0000
-  Nd  Nd6       1.0  0.84488  0.45579  0.15941  1.0000
-  Nd  Nd7       1.0  0.04062  0.84261  0.65648  1.0000
-  Nd  Nd8       1.0  0.94701  0.80851  0.66546  1.0000
-  Nd  Nd9       1.0  0.34650  0.05106  0.88646  1.0000
-  Nd  Nd10      1.0  0.37889  0.96688  0.87457  1.0000
-  Nd  Nd11      1.0  0.44870  0.37289  0.36890  1.0000
-  Nd  Nd12      1.0  0.45404  0.30985  0.32343  1.0000
-  Nd  Nd13      1.0  0.15956  0.43422  0.89243  1.0000
-  Nd  Nd14      1.0  0.11890  0.51607  0.88183  1.0000
-  Nd  Nd15      1.0  0.03119  0.10253  0.38320  1.0000
-  Nd  Nd16      1.0  0.03049  0.15860  0.31941  1.0000
-  H   H1        1.0  0.60421  0.93206  0.19101  1.0000
-  H   H2        1.0  0.73333  0.03313  0.10210  1.0000
-  H   H3        1.0  0.52385  0.60369  0.69423  1.0000
-  H   H4        1.0  0.42856  0.69963  0.57923  1.0000
-  H   H5        1.0  0.88384  0.53941  0.20530  1.0000
-  H   H6        1.0  0.77879  0.44096  0.08945  1.0000
-  H   H7        1.0  0.97496  0.89110  0.71845  1.0000
-  H   H8        1.0  0.00980  0.74994  0.61596  1.0000
-  H   H9        1.0  0.30958  0.97473  0.94500  1.0000
-  H   H10       1.0  0.42895  0.03590  0.82423  1.0000
-  H   H11       1.0  0.40623  0.38109  0.27510  1.0000
-  H   H12       1.0  0.47969  0.28521  0.41040  1.0000
-  H   H13       1.0  0.19849  0.51344  0.94588  1.0000
-  H   H14       1.0  0.06771  0.44275  0.83693  1.0000
-  H   H15       1.0  0.07274  0.06372  0.30737  1.0000
-  H   H16       1.0  0.99809  0.20262  0.39109  1.0000
-  H   H17       1.0  0.46704  0.06512  0.94639  1.0000
-  H   H18       1.0  0.63170  0.98466  0.04354  1.0000
-  H   H19       1.0  0.56885  0.01074  0.06839  1.0000
-  H   H20       1.0  0.57970  0.01357  0.01239  1.0000
-  H   H21       1.0  0.50750  0.01930  0.03163  1.0000
-  H   H22       1.0  0.52506  0.04153  0.98033  1.0000
-  H   H23       1.0  0.45025  0.02378  0.98839  1.0000
-  H   H24       1.0  0.49072  0.03051  0.92424  1.0000
-  H   H25       1.0  0.60984  0.94010  0.05050  1.0000
-  H   H26       1.0  0.54782  0.96476  0.06631  1.0000
-  H   H27       1.0  0.56720  0.96584  0.00714  1.0000
-  H   H28       1.0  0.49864  0.97312  0.01786  1.0000
-  H   H29       1.0  0.52875  0.99651  0.96437  1.0000
-  H   H30       1.0  0.45890  0.98390  0.96522  1.0000
-  H   H31       1.0  0.53025  0.55424  0.58636  1.0000
-  H   H32       1.0  0.48631  0.47457  0.42152  1.0000
-  H   H33       1.0  0.46212  0.44127  0.47323  1.0000
-  H   H34       1.0  0.50562  0.49444  0.47682  1.0000
-  H   H35       1.0  0.46078  0.48338  0.52595  1.0000
-  H   H36       1.0  0.51969  0.52132  0.53190  1.0000
-  H   H37       1.0  0.46468  0.53380  0.57264  1.0000
-  H   H38       1.0  0.53333  0.58803  0.55613  1.0000
-  H   H39       1.0  0.43691  0.48825  0.41721  1.0000
-  H   H40       1.0  0.41901  0.46752  0.46906  1.0000
-  H   H41       1.0  0.46919  0.52438  0.46319  1.0000
-  H   H42       1.0  0.43283  0.52034  0.51150  1.0000
-  H   H43       1.0  0.50079  0.55783  0.50932  1.0000
-  H   H44       1.0  0.45594  0.57409  0.55004  1.0000
-  H   H45       1.0  0.93788  0.52016  0.09471  1.0000
-  H   H46       1.0  0.04527  0.41864  0.96170  1.0000
-  H   H47       1.0  0.99551  0.46116  0.95120  1.0000
-  H   H48       1.0  0.00762  0.44232  0.01059  1.0000
-  H   H49       1.0  0.94323  0.46080  0.00018  1.0000
-  H   H50       1.0  0.97331  0.47491  0.05712  1.0000
-  H   H51       1.0  0.90433  0.46715  0.05673  1.0000
-  H   H52       1.0  0.90801  0.54915  0.07171  1.0000
-  H   H53       1.0  0.07519  0.45104  0.98309  1.0000
-  H   H54       1.0  0.02734  0.50041  0.96048  1.0000
-  H   H55       1.0  0.02801  0.48798  0.01523  1.0000
-  H   H56       1.0  0.95929  0.50716  0.99164  1.0000
-  H   H57       1.0  0.97391  0.52159  0.04491  1.0000
-  H   H58       1.0  0.89735  0.50556  0.03169  1.0000
-  H   H59       1.0  0.02041  0.06361  0.48787  1.0000
-  H   H60       1.0  0.92776  0.89976  0.58356  1.0000
-  H   H61       1.0  0.97378  0.89172  0.54232  1.0000
-  H   H62       1.0  0.95126  0.95888  0.54959  1.0000
-  H   H63       1.0  0.97453  0.94600  0.49834  1.0000
-  H   H64       1.0  0.98386  0.01369  0.51828  1.0000
-  H   H65       1.0  0.98359  0.00580  0.46216  1.0000
-  H   H66       1.0  0.06484  0.04294  0.47576  1.0000
-  H   H67       1.0  0.96061  0.93046  0.60486  1.0000
-  H   H68       1.0  0.01576  0.90626  0.56568  1.0000
-  H   H69       1.0  0.99958  0.96877  0.56536  1.0000
-  H   H70       1.0  0.02435  0.94103  0.51146  1.0000
-  H   H71       1.0  0.03505  0.00493  0.52189  1.0000
-  H   H72       1.0  0.03125  0.98649  0.46208  1.0000
-  H   H73       1.0  0.71670  0.82846  0.09735  1.0000
-  H   H74       1.0  0.74252  0.63093  0.09600  1.0000
-  H   H75       1.0  0.79051  0.66848  0.12968  1.0000
-  H   H76       1.0  0.73427  0.69641  0.10144  1.0000
-  H   H77       1.0  0.77984  0.73863  0.13315  1.0000
-  H   H78       1.0  0.72448  0.76185  0.10182  1.0000
-  H   H79       1.0  0.76473  0.80816  0.13547  1.0000
-  H   H80       1.0  0.67652  0.81747  0.12365  1.0000
-  H   H81       1.0  0.71148  0.62300  0.12897  1.0000
-  H   H82       1.0  0.75914  0.66024  0.16337  1.0000
-  H   H83       1.0  0.70397  0.68906  0.13551  1.0000
-  H   H84       1.0  0.74783  0.73204  0.16667  1.0000
-  H   H85       1.0  0.69175  0.75468  0.13444  1.0000
-  H   H86       1.0  0.72766  0.80230  0.16558  1.0000
-  H   H87       1.0  0.62075  0.76834  0.59905  1.0000
-  H   H88       1.0  0.83487  0.82659  0.60312  1.0000
-  H   H89       1.0  0.80457  0.79639  0.65130  1.0000
-  H   H90       1.0  0.76305  0.80508  0.60365  1.0000
-  H   H91       1.0  0.73205  0.77300  0.65055  1.0000
-  H   H92       1.0  0.69203  0.78570  0.60297  1.0000
-  H   H93       1.0  0.65799  0.75133  0.64725  1.0000
-  H   H94       1.0  0.63403  0.72782  0.57972  1.0000
-  H   H95       1.0  0.84820  0.78239  0.58930  1.0000
-  H   H96       1.0  0.81775  0.75256  0.63661  1.0000
-  H   H97       1.0  0.77659  0.76169  0.58845  1.0000
-  H   H98       1.0  0.74458  0.72981  0.63396  1.0000
-  H   H99       1.0  0.70487  0.74311  0.58580  1.0000
-  H   H100      1.0  0.67021  0.70888  0.62898  1.0000
-  H   H101      1.0  0.20040  0.32767  0.94035  1.0000
-  H   H102      1.0  0.30980  0.15866  0.93511  1.0000
-  H   H103      1.0  0.25542  0.16462  0.89471  1.0000
-  H   H104      1.0  0.27375  0.21452  0.93278  1.0000
-  H   H105      1.0  0.22181  0.22797  0.89170  1.0000
-  H   H106      1.0  0.23713  0.27118  0.93488  1.0000
-  H   H107      1.0  0.19279  0.29409  0.89051  1.0000
-  H   H108      1.0  0.24678  0.34768  0.92920  1.0000
-  H   H109      1.0  0.34485  0.17460  0.90597  1.0000
-  H   H110      1.0  0.29156  0.18289  0.86726  1.0000
-  H   H111      1.0  0.31078  0.23265  0.90645  1.0000
-  H   H112      1.0  0.26024  0.24895  0.86772  1.0000
-  H   H113      1.0  0.27852  0.29106  0.91408  1.0000
-  H   H114      1.0  0.23606  0.31755  0.87444  1.0000
-  H   H115      1.0  0.31950  0.31943  0.39098  1.0000
-  H   H116      1.0  0.13259  0.20557  0.39985  1.0000
-  H   H117      1.0  0.15700  0.21975  0.34482  1.0000
-  H   H118      1.0  0.19365  0.24472  0.39115  1.0000
-  H   H119      1.0  0.22725  0.25554  0.33860  1.0000
-  H   H120      1.0  0.25636  0.28333  0.38720  1.0000
-  H   H121      1.0  0.29767  0.29276  0.33853  1.0000
-  H   H122      1.0  0.34415  0.27876  0.39942  1.0000
-  H   H123      1.0  0.15827  0.16441  0.39971  1.0000
-  H   H124      1.0  0.18422  0.17883  0.34586  1.0000
-  H   H125      1.0  0.21917  0.20345  0.39535  1.0000
-  H   H126      1.0  0.25386  0.21487  0.34477  1.0000
-  H   H127      1.0  0.28113  0.24249  0.39567  1.0000
-  H   H128      1.0  0.32261  0.25177  0.34749  1.0000
-  H   H129      1.0  0.56433  0.24320  0.31932  1.0000
-  H   H130      1.0  0.68212  0.10681  0.23535  1.0000
-  H   H131      1.0  0.60816  0.10681  0.22656  1.0000
-  H   H132      1.0  0.64093  0.15195  0.26300  1.0000
-  H   H133      1.0  0.56821  0.15447  0.25262  1.0000
-  H   H134      1.0  0.60152  0.19746  0.29074  1.0000
-  H   H135      1.0  0.52924  0.20282  0.28048  1.0000
-  H   H136      1.0  0.57747  0.27575  0.28893  1.0000
-  H   H137      1.0  0.68835  0.13556  0.20082  1.0000
-  H   H138      1.0  0.61650  0.13763  0.19407  1.0000
-  H   H139      1.0  0.65048  0.18284  0.23072  1.0000
-  H   H140      1.0  0.57850  0.18636  0.22111  1.0000
-  H   H141      1.0  0.61255  0.22930  0.25947  1.0000
-  H   H142      1.0  0.54076  0.23528  0.24958  1.0000
-  H   H143      1.0  0.36383  0.65685  0.73967  1.0000
-  H   H144      1.0  0.25999  0.51767  0.84857  1.0000
-  H   H145      1.0  0.21787  0.55414  0.80875  1.0000
-  H   H146      1.0  0.28566  0.57090  0.81623  1.0000
-  H   H147      1.0  0.25822  0.58780  0.76125  1.0000
-  H   H148      1.0  0.31769  0.61916  0.77793  1.0000
-  H   H149      1.0  0.31169  0.61634  0.71807  1.0000
-  H   H150      1.0  0.39315  0.61899  0.74985  1.0000
-  H   H151      1.0  0.25680  0.48101  0.82082  1.0000
-  H   H152      1.0  0.22737  0.51822  0.78121  1.0000
-  H   H153      1.0  0.30186  0.53013  0.79801  1.0000
-  H   H154      1.0  0.28316  0.54915  0.74635  1.0000
-  H   H155      1.0  0.34561  0.57895  0.77617  1.0000
-  H   H156      1.0  0.34219  0.57755  0.71874  1.0000
-  H   H157      1.0  0.81099  0.33394  0.18601  1.0000
-  H   H158      1.0  0.92423  0.18298  0.25277  1.0000
-  H   H159      1.0  0.95994  0.24374  0.24611  1.0000
-  H   H160      1.0  0.88829  0.23456  0.23068  1.0000
-  H   H161      1.0  0.92287  0.29425  0.21980  1.0000
-  H   H162      1.0  0.85053  0.28480  0.20792  1.0000
-  H   H163      1.0  0.88488  0.34347  0.19397  1.0000
-  H   H164      1.0  0.80383  0.35660  0.22350  1.0000
-  H   H165      1.0  0.90744  0.19634  0.29056  1.0000
-  H   H166      1.0  0.94481  0.25733  0.28491  1.0000
-  H   H167      1.0  0.87472  0.25019  0.26915  1.0000
-  H   H168      1.0  0.91101  0.31027  0.25863  1.0000
-  H   H169      1.0  0.83948  0.30222  0.24640  1.0000
-  H   H170      1.0  0.87558  0.36156  0.23251  1.0000
-  H   H171      1.0  0.23582  0.00826  0.82615  1.0000
-  H   H172      1.0  0.09280  0.87895  0.75074  1.0000
-  H   H173      1.0  0.14404  0.91447  0.71735  1.0000
-  H   H174      1.0  0.14270  0.91849  0.77495  1.0000
-  H   H175      1.0  0.20287  0.94726  0.74566  1.0000
-  H   H176      1.0  0.18908  0.96147  0.80029  1.0000
-  H   H177      1.0  0.25929  0.97930  0.77945  1.0000
-  H   H178      1.0  0.23801  0.96730  0.84878  1.0000
-  H   H179      1.0  0.12135  0.83935  0.74688  1.0000
-  H   H180      1.0  0.17367  0.87497  0.71905  1.0000
-  H   H181      1.0  0.16972  0.87784  0.77873  1.0000
-  H   H182      1.0  0.22875  0.90735  0.75670  1.0000
-  H   H183      1.0  0.20915  0.91990  0.81381  1.0000
-  H   H184      1.0  0.27524  0.94010  0.80061  1.0000
-  H   H185      1.0  0.37209  0.91336  0.77593  1.0000
-  H   H186      1.0  0.45665  0.77844  0.67453  1.0000
-  H   H187      1.0  0.47511  0.77266  0.72940  1.0000
-  H   H188      1.0  0.42535  0.81899  0.71141  1.0000
-  H   H189      1.0  0.45247  0.82491  0.76536  1.0000
-  H   H190      1.0  0.39846  0.86419  0.74523  1.0000
-  H   H191      1.0  0.42754  0.87767  0.79806  1.0000
-  H   H192      1.0  0.33693  0.88330  0.79542  1.0000
-  H   H193      1.0  0.41048  0.75353  0.68053  1.0000
-  H   H194      1.0  0.43364  0.74124  0.73714  1.0000
-  H   H195      1.0  0.38684  0.78760  0.72478  1.0000
-  H   H196      1.0  0.41493  0.79256  0.77965  1.0000
-  H   H197      1.0  0.36262  0.83270  0.76249  1.0000
-  H   H198      1.0  0.39153  0.84637  0.81578  1.0000
-  H   H199      1.0  0.58900  0.36472  0.32880  1.0000
-  H   H200      1.0  0.75442  0.45943  0.24631  1.0000
-  H   H201      1.0  0.70591  0.42130  0.21342  1.0000
-  H   H202      1.0  0.69666  0.43051  0.27096  1.0000
-  H   H203      1.0  0.64206  0.39477  0.24099  1.0000
-  H   H204      1.0  0.64217  0.39845  0.29874  1.0000
-  H   H205      1.0  0.57907  0.37084  0.27269  1.0000
-  H   H206      1.0  0.57743  0.41108  0.33647  1.0000
-  H   H207      1.0  0.72857  0.49949  0.23607  1.0000
-  H   H208      1.0  0.67955  0.46176  0.20527  1.0000
-  H   H209      1.0  0.67125  0.47135  0.26362  1.0000
-  H   H210      1.0  0.61631  0.43650  0.23805  1.0000
-  H   H211      1.0  0.62026  0.44192  0.29784  1.0000
-  H   H212      1.0  0.55817  0.41481  0.27731  1.0000
-  H   H213      1.0  0.14439  0.58772  0.79062  1.0000
-  H   H214      1.0  0.05613  0.76868  0.74729  1.0000
-  H   H215      1.0  0.04986  0.71052  0.70969  1.0000
-  H   H216      1.0  0.09131  0.70981  0.75459  1.0000
-  H   H217      1.0  0.05888  0.64530  0.73908  1.0000
-  H   H218      1.0  0.11911  0.64732  0.76752  1.0000
-  H   H219      1.0  0.07497  0.58853  0.77814  1.0000
-  H   H220      1.0  0.14035  0.61833  0.82275  1.0000
-  H   H221      1.0  0.00535  0.75725  0.75618  1.0000
-  H   H222      1.0  0.00577  0.69930  0.73169  1.0000
-  H   H223      1.0  0.05153  0.71199  0.78192  1.0000
-  H   H224      1.0  0.02952  0.65025  0.77388  1.0000
-  H   H225      1.0  0.09800  0.66576  0.80235  1.0000
-  H   H226      1.0  0.06333  0.60924  0.81528  1.0000
-  H   H227      1.0  0.75637  0.96566  0.24155  1.0000
-  H   H228      1.0  0.91004  0.05291  0.34201  1.0000
-  H   H229      1.0  0.92572  0.05255  0.28311  1.0000
-  H   H230      1.0  0.86319  0.02583  0.30477  1.0000
-  H   H231      1.0  0.86762  0.02811  0.24539  1.0000
-  H   H232      1.0  0.81047  0.99729  0.27211  1.0000
-  H   H233      1.0  0.80672  0.00245  0.21248  1.0000
-  H   H234      1.0  0.72993  0.00595  0.25041  1.0000
-  H   H235      1.0  0.89435  0.09836  0.33755  1.0000
-  H   H236      1.0  0.90485  0.09676  0.28027  1.0000
-  H   H237      1.0  0.84195  0.06962  0.30436  1.0000
-  H   H238      1.0  0.84371  0.07096  0.24619  1.0000
-  H   H239      1.0  0.78654  0.03967  0.27508  1.0000
-  H   H240      1.0  0.77959  0.04307  0.21743  1.0000
-  C   C1        1.0  0.66676  0.08157  0.19158  1.0000
-  C   C2        1.0  0.72478  0.98751  0.20323  1.0000
-  C   C3        1.0  0.61524  0.95791  0.18192  1.0000
-  C   C4        1.0  0.70966  0.86606  0.13472  1.0000
-  C   C5        1.0  0.62863  0.97073  0.09118  1.0000
-  C   C6        1.0  0.72637  0.00745  0.11341  1.0000
-  C   C7        1.0  0.59073  0.72000  0.61463  1.0000
-  C   C8        1.0  0.50203  0.60283  0.59682  1.0000
-  C   C9        1.0  0.52478  0.62652  0.67839  1.0000
-  C   C10       1.0  0.39317  0.63135  0.70181  1.0000
-  C   C11       1.0  0.45974  0.72098  0.67849  1.0000
-  C   C12       1.0  0.42949  0.68054  0.59834  1.0000
-  C   C13       1.0  0.82788  0.38994  0.18664  1.0000
-  C   C14       1.0  0.76193  0.47738  0.19921  1.0000
-  C   C15       1.0  0.87423  0.51471  0.19326  1.0000
-  C   C16       1.0  0.76312  0.59361  0.12913  1.0000
-  C   C17       1.0  0.87746  0.50991  0.10122  1.0000
-  C   C18       1.0  0.78248  0.46516  0.10371  1.0000
-  C   C19       1.0  0.88073  0.80222  0.62870  1.0000
-  C   C20       1.0  0.97179  0.87559  0.61184  1.0000
-  C   C21       1.0  0.96552  0.86775  0.70448  1.0000
-  C   C22       1.0  0.09272  0.85677  0.70539  1.0000
-  C   C23       1.0  0.01637  0.77521  0.70951  1.0000
-  C   C24       1.0  0.01939  0.77618  0.62529  1.0000
-  C   C25       1.0  0.37141  0.91918  0.82506  1.0000
-  C   C26       1.0  0.29255  0.99451  0.84272  1.0000
-  C   C27       1.0  0.32954  0.97065  0.92591  1.0000
-  C   C28       1.0  0.32105  0.12081  0.89877  1.0000
-  C   C29       1.0  0.42907  0.02672  0.92135  1.0000
-  C   C30       1.0  0.40512  0.04153  0.83976  1.0000
-  C   C31       1.0  0.51727  0.27288  0.30220  1.0000
-  C   C32       1.0  0.52840  0.37437  0.32747  1.0000
-  C   C33       1.0  0.42001  0.36021  0.28827  1.0000
-  C   C34       1.0  0.44567  0.43146  0.41063  1.0000
-  C   C35       1.0  0.37312  0.31300  0.36626  1.0000
-  C   C36       1.0  0.47057  0.30972  0.39929  1.0000
-  C   C37       1.0  0.12096  0.56469  0.83275  1.0000
-  C   C38       1.0  0.20389  0.49266  0.84472  1.0000
-  C   C39       1.0  0.17534  0.51610  0.92883  1.0000
-  C   C40       1.0  0.19777  0.37149  0.90846  1.0000
-  C   C41       1.0  0.08089  0.45561  0.93423  1.0000
-  C   C42       1.0  0.09412  0.43896  0.85026  1.0000
-  C   C43       1.0  0.96771  0.18616  0.28851  1.0000
-  C   C44       1.0  0.95566  0.09363  0.33491  1.0000
-  C   C45       1.0  0.06320  0.09115  0.30922  1.0000
-  C   C46       1.0  0.02932  0.06196  0.43865  1.0000
-  C   C47       1.0  0.10624  0.16392  0.37148  1.0000
-  C   C48       1.0  0.00426  0.17415  0.39038  1.0000
-  C   C49       1.0  0.46565  0.03584  0.93990  1.0000
-  C   C50       1.0  0.61096  0.96874  0.05888  1.0000
-  C   C51       1.0  0.56993  0.98427  0.05581  1.0000
-  C   C52       1.0  0.56034  0.99045  0.02090  1.0000
-  C   C53       1.0  0.51713  0.99857  0.01466  1.0000
-  C   C54       1.0  0.51214  0.01317  0.98108  1.0000
-  C   C55       1.0  0.46910  0.01265  0.96983  1.0000
-  C   C56       1.0  0.51333  0.57455  0.57357  1.0000
-  C   C57       1.0  0.45521  0.46696  0.42726  1.0000
-  C   C58       1.0  0.45067  0.46656  0.46323  1.0000
-  C   C59       1.0  0.47381  0.49981  0.47768  1.0000
-  C   C60       1.0  0.46227  0.50866  0.51169  1.0000
-  C   C61       1.0  0.49275  0.53603  0.52653  1.0000
-  C   C62       1.0  0.47842  0.55451  0.55661  1.0000
-  C   C63       1.0  0.91094  0.52082  0.07995  1.0000
-  C   C64       1.0  0.05540  0.44777  0.96236  1.0000
-  C   C65       1.0  0.01975  0.47160  0.96680  1.0000
-  C   C66       1.0  0.00654  0.47057  0.00144  1.0000
-  C   C67       1.0  0.96465  0.48332  0.00677  1.0000
-  C   C68       1.0  0.95885  0.49434  0.04137  1.0000
-  C   C69       1.0  0.91535  0.49543  0.05131  1.0000
-  C   C70       1.0  0.03313  0.04497  0.47048  1.0000
-  C   C71       1.0  0.95892  0.90518  0.59046  1.0000
-  C   C72       1.0  0.98442  0.91126  0.56077  1.0000
-  C   C73       1.0  0.98221  0.95072  0.54888  1.0000
-  C   C74       1.0  0.99752  0.95645  0.51509  1.0000
-  C   C75       1.0  0.00757  0.99714  0.50881  1.0000
-  C   C76       1.0  0.01293  0.00670  0.47371  1.0000
-  C   C77       1.0  0.70771  0.82774  0.12237  1.0000
-  C   C78       1.0  0.74262  0.62777  0.12191  1.0000
-  C   C79       1.0  0.75969  0.66308  0.13740  1.0000
-  C   C80       1.0  0.73465  0.69496  0.12753  1.0000
-  C   C81       1.0  0.74906  0.73245  0.14062  1.0000
-  C   C82       1.0  0.72271  0.76198  0.12790  1.0000
-  C   C83       1.0  0.73322  0.80093  0.13992  1.0000
-  C   C84       1.0  0.62749  0.73950  0.60308  1.0000
-  C   C85       1.0  0.84305  0.79903  0.61051  1.0000
-  C   C86       1.0  0.80952  0.78031  0.62965  1.0000
-  C   C87       1.0  0.77130  0.77725  0.61032  1.0000
-  C   C88       1.0  0.73704  0.75812  0.62830  1.0000
-  C   C89       1.0  0.69931  0.75722  0.60836  1.0000
-  C   C90       1.0  0.66378  0.73776  0.62451  1.0000
-  C   C91       1.0  0.21749  0.33827  0.91993  1.0000
-  C   C92       1.0  0.31631  0.15933  0.90959  1.0000
-  C   C93       1.0  0.28416  0.18001  0.89254  1.0000
-  C   C94       1.0  0.28139  0.21817  0.90758  1.0000
-  C   C95       1.0  0.25112  0.24258  0.89217  1.0000
-  C   C96       1.0  0.24846  0.27829  0.91111  1.0000
-  C   C97       1.0  0.22215  0.30687  0.89631  1.0000
-  C   C98       1.0  0.33543  0.29699  0.38015  1.0000
-  C   C99       1.0  0.14280  0.18358  0.38447  1.0000
-  C   C100      1.0  0.17220  0.20073  0.36043  1.0000
-  C   C101      1.0  0.20621  0.22194  0.37795  1.0000
-  C   C102      1.0  0.23969  0.23765  0.35668  1.0000
-  C   C103      1.0  0.27081  0.25996  0.37635  1.0000
-  C   C104      1.0  0.30724  0.27489  0.35781  1.0000
-  C   C105      1.0  0.55488  0.25486  0.29665  1.0000
-  C   C106      1.0  0.66935  0.11423  0.21235  1.0000
-  C   C107      1.0  0.62834  0.12879  0.21705  1.0000
-  C   C108      1.0  0.62984  0.16105  0.23987  1.0000
-  C   C109      1.0  0.58914  0.17636  0.24408  1.0000
-  C   C110      1.0  0.59106  0.20773  0.26779  1.0000
-  C   C111      1.0  0.55099  0.22423  0.27231  1.0000
-  C   C112      1.0  0.37211  0.62926  0.73239  1.0000
-  C   C113      1.0  0.24157  0.50507  0.82945  1.0000
-  C   C114      1.0  0.23839  0.53269  0.80268  1.0000
-  C   C115      1.0  0.27927  0.55095  0.79695  1.0000
-  C   C116      1.0  0.28331  0.57017  0.76517  1.0000
-  C   C117      1.0  0.32187  0.59370  0.76446  1.0000
-  C   C118      1.0  0.33547  0.60319  0.73109  1.0000
-  C   C119      1.0  0.82356  0.35431  0.20301  1.0000
-  C   C120      1.0  0.93189  0.20022  0.27357  1.0000
-  C   C121      1.0  0.93647  0.24033  0.26406  1.0000
-  C   C122      1.0  0.89756  0.25265  0.25061  1.0000
-  C   C123      1.0  0.90094  0.29203  0.23903  1.0000
-  C   C124      1.0  0.86108  0.30372  0.22692  1.0000
-  C   C125      1.0  0.86395  0.34252  0.21397  1.0000
-  C   C126      1.0  0.25287  0.98368  0.82997  1.0000
-  C   C127      1.0  0.11380  0.86519  0.73539  1.0000
-  C   C128      1.0  0.15082  0.89007  0.73136  1.0000
-  C   C129      1.0  0.16567  0.90225  0.76389  1.0000
-  C   C130      1.0  0.20455  0.92504  0.76318  1.0000
-  C   C131      1.0  0.21211  0.94170  0.79577  1.0000
-  C   C132      1.0  0.25279  0.96098  0.79966  1.0000
-  C   C133      1.0  0.36738  0.89544  0.79666  1.0000
-  C   C134      1.0  0.44189  0.75569  0.68780  1.0000
-  C   C135      1.0  0.44419  0.76500  0.72287  1.0000
-  C   C136      1.0  0.41795  0.79715  0.72878  1.0000
-  C   C137      1.0  0.42187  0.81379  0.76173  1.0000
-  C   C138      1.0  0.39316  0.84454  0.76477  1.0000
-  C   C139      1.0  0.39716  0.86541  0.79590  1.0000
-  C   C140      1.0  0.57018  0.38696  0.32136  1.0000
-  C   C141      1.0  0.73669  0.47221  0.22779  1.0000
-  C   C142      1.0  0.69866  0.44849  0.22257  1.0000
-  C   C143      1.0  0.67696  0.44390  0.25413  1.0000
-  C   C144      1.0  0.63756  0.42150  0.25227  1.0000
-  C   C145      1.0  0.62133  0.41520  0.28562  1.0000
-  C   C146      1.0  0.57996  0.39625  0.28694  1.0000
-  C   C147      1.0  0.12475  0.59547  0.80997  1.0000
-  C   C148      1.0  0.02851  0.75510  0.73813  1.0000
-  C   C149      1.0  0.03476  0.71452  0.73245  1.0000
-  C   C150      1.0  0.06039  0.70017  0.75909  1.0000
-  C   C151      1.0  0.05785  0.65854  0.76252  1.0000
-  C   C152      1.0  0.09245  0.64636  0.78252  1.0000
-  C   C153      1.0  0.08581  0.60809  0.79651  1.0000
-  C   C154      1.0  0.74848  0.99275  0.23275  1.0000
-  C   C155      1.0  0.91478  0.07839  0.32826  1.0000
-  C   C156      1.0  0.90423  0.07078  0.29357  1.0000
-  C   C157      1.0  0.86269  0.05214  0.29198  1.0000
-  C   C158      1.0  0.84681  0.04469  0.25855  1.0000
-  C   C159      1.0  0.80649  0.02383  0.26034  1.0000
-  C   C160      1.0  0.78651  0.01663  0.22825  1.0000
-  O   O1        1.0  0.65391  0.08270  0.16238  1.0000
-  O   O2        1.0  0.67378  0.04843  0.20153  1.0000
-  O   O3        1.0  0.73027  0.95707  0.18637  1.0000
-  O   O4        1.0  0.69786  0.01269  0.19730  1.0000
-  O   O5        1.0  0.64553  0.96337  0.16442  1.0000
-  O   O6        1.0  0.60078  0.98974  0.18654  1.0000
-  O   O7        1.0  0.73246  0.89230  0.12281  1.0000
-  O   O8        1.0  0.68050  0.87907  0.15029  1.0000
-  O   O9        1.0  0.62458  0.00162  0.10750  1.0000
-  O   O10       1.0  0.65148  0.94336  0.09919  1.0000
-  O   O11       1.0  0.70814  0.00239  0.13912  1.0000
-  O   O12       1.0  0.73409  0.97552  0.10367  1.0000
-  O   O13       1.0  0.58765  0.70042  0.64035  1.0000
-  O   O14       1.0  0.55773  0.72004  0.59863  1.0000
-  O   O15       1.0  0.46946  0.59628  0.61390  1.0000
-  O   O16       1.0  0.52661  0.63240  0.59933  1.0000
-  O   O17       1.0  0.49651  0.64695  0.67228  1.0000
-  O   O18       1.0  0.55491  0.63971  0.66330  1.0000
-  O   O19       1.0  0.40680  0.60248  0.68799  1.0000
-  O   O20       1.0  0.40418  0.66253  0.68813  1.0000
-  O   O21       1.0  0.49624  0.72404  0.66667  1.0000
-  O   O22       1.0  0.43450  0.69141  0.67611  1.0000
-  O   O23       1.0  0.46002  0.67456  0.61531  1.0000
-  O   O24       1.0  0.39989  0.65982  0.60889  1.0000
-  O   O25       1.0  0.84631  0.39367  0.15962  1.0000
-  O   O26       1.0  0.81611  0.42085  0.19867  1.0000
-  O   O27       1.0  0.75555  0.50642  0.18109  1.0000
-  O   O28       1.0  0.79267  0.45562  0.19656  1.0000
-  O   O29       1.0  0.84596  0.51186  0.17285  1.0000
-  O   O30       1.0  0.88930  0.48262  0.19647  1.0000
-  O   O31       1.0  0.75099  0.56194  0.11733  1.0000
-  O   O32       1.0  0.79373  0.59132  0.14774  1.0000
-  O   O33       1.0  0.88056  0.47848  0.11660  1.0000
-  O   O34       1.0  0.85020  0.53432  0.10678  1.0000
-  O   O35       1.0  0.78968  0.46602  0.13321  1.0000
-  O   O36       1.0  0.77685  0.49804  0.09503  1.0000
-  O   O37       1.0  0.89443  0.77493  0.64467  1.0000
-  O   O38       1.0  0.90346  0.83258  0.63032  1.0000
-  O   O39       1.0  0.01034  0.87529  0.61791  1.0000
-  O   O40       1.0  0.94330  0.85477  0.62627  1.0000
-  O   O41       1.0  0.98672  0.85111  0.68447  1.0000
-  O   O42       1.0  0.93035  0.85144  0.70432  1.0000
-  O   O43       1.0  0.08224  0.88175  0.68539  1.0000
-  O   O44       1.0  0.07558  0.82437  0.69972  1.0000
-  O   O45       1.0  0.97863  0.77222  0.70107  1.0000
-  O   O46       1.0  0.04344  0.79912  0.69750  1.0000
-  O   O47       1.0  0.99717  0.80209  0.63236  1.0000
-  O   O48       1.0  0.05540  0.78841  0.62941  1.0000
-  O   O49       1.0  0.40556  0.92990  0.83746  1.0000
-  O   O50       1.0  0.34106  0.93432  0.83824  1.0000
-  O   O51       1.0  0.29711  0.02900  0.85325  1.0000
-  O   O52       1.0  0.31767  0.96759  0.84738  1.0000
-  O   O53       1.0  0.34285  0.99536  0.90676  1.0000
-  O   O54       1.0  0.34417  0.93977  0.91747  1.0000
-  O   O55       1.0  0.34114  0.11235  0.87379  1.0000
-  O   O56       1.0  0.31479  0.09266  0.91734  1.0000
-  O   O57       1.0  0.42757  0.99435  0.90665  1.0000
-  O   O58       1.0  0.40275  0.05263  0.91836  1.0000
-  O   O59       1.0  0.37747  0.01902  0.84823  1.0000
-  O   O60       1.0  0.39846  0.07223  0.85286  1.0000
-  O   O61       1.0  0.48613  0.25647  0.31524  1.0000
-  O   O62       1.0  0.51496  0.30865  0.30027  1.0000
-  O   O63       1.0  0.51052  0.39044  0.35119  1.0000
-  O   O64       1.0  0.51353  0.34444  0.31240  1.0000
-  O   O65       1.0  0.43053  0.36486  0.31783  1.0000
-  O   O66       1.0  0.42682  0.32760  0.27688  1.0000
-  O   O67       1.0  0.46250  0.40098  0.41726  1.0000
-  O   O68       1.0  0.42946  0.43044  0.38258  1.0000
-  O   O69       1.0  0.39300  0.29330  0.34592  1.0000
-  O   O70       1.0  0.38711  0.34468  0.37841  1.0000
-  O   O71       1.0  0.48006  0.31899  0.37103  1.0000
-  O   O72       1.0  0.45849  0.33804  0.41411  1.0000
-  O   O73       1.0  0.08820  0.55404  0.84714  1.0000
-  O   O74       1.0  0.15223  0.54892  0.84365  1.0000
-  O   O75       1.0  0.20296  0.45841  0.85574  1.0000
-  O   O76       1.0  0.17728  0.51800  0.85071  1.0000
-  O   O77       1.0  0.16024  0.49043  0.91125  1.0000
-  O   O78       1.0  0.15793  0.54598  0.92153  1.0000
-  O   O79       1.0  0.17347  0.37299  0.88447  1.0000
-  O   O80       1.0  0.20122  0.40243  0.92386  1.0000
-  O   O81       1.0  0.07691  0.48702  0.91863  1.0000
-  O   O82       1.0  0.10872  0.43155  0.92910  1.0000
-  O   O83       1.0  0.12121  0.46311  0.85637  1.0000
-  O   O84       1.0  0.10454  0.40942  0.86325  1.0000
-  O   O85       1.0  0.99727  0.20689  0.29975  1.0000
-  O   O86       1.0  0.97112  0.15100  0.29381  1.0000
-  O   O87       1.0  0.97148  0.08244  0.36197  1.0000
-  O   O88       1.0  0.97119  0.12014  0.31591  1.0000
-  O   O89       1.0  0.05256  0.10716  0.33434  1.0000
-  O   O90       1.0  0.05875  0.11427  0.28641  1.0000
-  O   O91       1.0  0.01121  0.09213  0.43446  1.0000
-  O   O92       1.0  0.04947  0.05320  0.41377  1.0000
-  O   O93       1.0  0.08936  0.17749  0.34562  1.0000
-  O   O94       1.0  0.09107  0.13629  0.38921  1.0000
-  O   O95       1.0  0.00245  0.15345  0.36619  1.0000
-  O   O96       1.0  0.01561  0.15452  0.41346  1.0000
+ _atom_site_type_symbol
+ _atom_site_label
+ _atom_site_symmetry_multiplicity
+ _atom_site_fract_x
+ _atom_site_fract_y
+ _atom_site_fract_z
+ _atom_site_occupancy
+  Na  Na0  1  0.96708000  0.10660000  0.05596000  1.0
+  Na  Na1  1  0.94273000  0.87919000  0.96008000  1.0
+  Na  Na2  1  0.48234000  0.60248000  0.44114000  1.0
+  Na  Na3  1  0.45618000  0.39005000  0.57242000  1.0
+  Cd  Cd4  1  0.98858000  0.01984000  0.01381000  1.0
+  Cd  Cd5  1  0.91938000  0.97002000  0.98470000  1.0
+  Cd  Cd6  1  0.50775000  0.51996000  0.48299000  1.0
+  Cd  Cd7  1  0.43785000  0.47072000  0.51546000  1.0
+  H  H8  1  0.05505000  0.78976000  0.36452000  1.0
+  H  H9  1  0.95180000  0.75063000  0.41890000  1.0
+  H  H10  1  0.92066000  0.77622000  0.34222000  1.0
+  H  H11  1  0.04058000  0.72093000  0.32509000  1.0
+  H  H12  1  0.03701000  0.20900000  0.62705000  1.0
+  H  H13  1  0.91681000  0.24289000  0.58061000  1.0
+  H  H14  1  0.89074000  0.20977000  0.64972000  1.0
+  H  H15  1  0.99841000  0.26526000  0.67723000  1.0
+  H  H16  1  0.39572000  0.27124000  0.11682000  1.0
+  H  H17  1  0.51345000  0.24389000  0.09459000  1.0
+  H  H18  1  0.53678000  0.26449000  0.16845000  1.0
+  H  H19  1  0.42420000  0.21514000  0.18717000  1.0
+  H  H20  1  0.37853000  0.71960000  0.89264000  1.0
+  H  H21  1  0.48217000  0.74773000  0.90748000  1.0
+  H  H22  1  0.50913000  0.71925000  0.83353000  1.0
+  H  H23  1  0.38885000  0.77585000  0.81520000  1.0
+  H  H24  1  0.70727000  0.91674000  0.88177000  1.0
+  H  H25  1  0.75549000  0.96837000  0.87518000  1.0
+  H  H26  1  0.80845000  0.97696000  0.90601000  1.0
+  H  H27  1  0.73577000  0.83920000  0.96854000  1.0
+  H  H28  1  0.80018000  0.84443000  0.01012000  1.0
+  H  H29  1  0.84219000  0.88289000  0.00869000  1.0
+  H  H30  1  0.67512000  0.81115000  0.95303000  1.0
+  H  H31  1  0.62902000  0.75912000  0.96080000  1.0
+  H  H32  1  0.57852000  0.74839000  0.92899000  1.0
+  H  H33  1  0.64802000  0.88619000  0.86346000  1.0
+  H  H34  1  0.58148000  0.87742000  0.82137000  1.0
+  H  H35  1  0.54204000  0.83754000  0.82513000  1.0
+  H  H36  1  0.75134000  0.05752000  0.11083000  1.0
+  H  H37  1  0.80717000  0.00320000  0.11342000  1.0
+  H  H38  1  0.86174000  0.99560000  0.08198000  1.0
+  H  H39  1  0.75991000  0.13280000  0.02194000  1.0
+  H  H40  1  0.83526000  0.13698000  0.98975000  1.0
+  H  H41  1  0.89524000  0.10970000  0.00428000  1.0
+  H  H42  1  0.71027000  0.16965000  0.04546000  1.0
+  H  H43  1  0.65948000  0.22459000  0.03963000  1.0
+  H  H44  1  0.60916000  0.23767000  0.07270000  1.0
+  H  H45  1  0.68921000  0.09145000  0.13133000  1.0
+  H  H46  1  0.62488000  0.10426000  0.17606000  1.0
+  H  H47  1  0.58254000  0.14714000  0.17441000  1.0
+  H  H48  1  0.64415000  0.34343000  0.52717000  1.0
+  H  H49  1  0.55885000  0.33964000  0.51066000  1.0
+  H  H50  1  0.51064000  0.37898000  0.51269000  1.0
+  H  H51  1  0.69322000  0.43333000  0.58665000  1.0
+  H  H52  1  0.64714000  0.49124000  0.58163000  1.0
+  H  H53  1  0.58463000  0.49769000  0.55788000  1.0
+  H  H54  1  0.75452000  0.39900000  0.60787000  1.0
+  H  H55  1  0.82948000  0.39006000  0.64477000  1.0
+  H  H56  1  0.86539000  0.34485000  0.64958000  1.0
+  H  H57  1  0.69693000  0.30869000  0.55199000  1.0
+  H  H58  1  0.73920000  0.25072000  0.55341000  1.0
+  H  H59  1  0.79746000  0.23994000  0.58112000  1.0
+  H  H60  1  0.73973000  0.57371000  0.40023000  1.0
+  H  H61  1  0.70394000  0.51697000  0.39876000  1.0
+  H  H62  1  0.64307000  0.50844000  0.42267000  1.0
+  H  H63  1  0.67303000  0.66010000  0.46549000  1.0
+  H  H64  1  0.59546000  0.65542000  0.49637000  1.0
+  H  H65  1  0.55762000  0.61506000  0.49210000  1.0
+  H  H66  1  0.73042000  0.69236000  0.45023000  1.0
+  H  H67  1  0.76681000  0.74852000  0.45402000  1.0
+  H  H68  1  0.82630000  0.75798000  0.42928000  1.0
+  H  H69  1  0.79892000  0.60578000  0.38518000  1.0
+  H  H70  1  0.87529000  0.61312000  0.35168000  1.0
+  H  H71  1  0.90711000  0.65632000  0.35122000  1.0
+  H  H72  1  0.22653000  0.06657000  0.09223000  1.0
+  H  H73  1  0.19243000  0.01025000  0.08950000  1.0
+  H  H74  1  0.12727000  0.00477000  0.07149000  1.0
+  H  H75  1  0.14160000  0.16563000  0.05536000  1.0
+  H  H76  1  0.06603000  0.16593000  0.02288000  1.0
+  H  H77  1  0.03795000  0.12386000  0.01005000  1.0
+  H  H78  1  0.20252000  0.19533000  0.06925000  1.0
+  H  H79  1  0.23638000  0.25263000  0.07511000  1.0
+  H  H80  1  0.29780000  0.25706000  0.09923000  1.0
+  H  H81  1  0.28640000  0.09623000  0.10893000  1.0
+  H  H82  1  0.36408000  0.09737000  0.14130000  1.0
+  H  H83  1  0.38947000  0.14046000  0.15407000  1.0
+  H  H84  1  0.18252000  0.88739000  0.98658000  1.0
+  H  H85  1  0.14289000  0.91797000  0.03587000  1.0
+  H  H86  1  0.07734000  0.94190000  0.03226000  1.0
+  H  H87  1  0.10930000  0.89787000  0.88373000  1.0
+  H  H88  1  0.02280000  0.91746000  0.87620000  1.0
+  H  H89  1  0.98195000  0.93401000  0.91366000  1.0
+  H  H90  1  0.16651000  0.86478000  0.86279000  1.0
+  H  H91  1  0.19911000  0.83624000  0.81266000  1.0
+  H  H92  1  0.26046000  0.80699000  0.81389000  1.0
+  H  H93  1  0.24348000  0.85299000  0.96466000  1.0
+  H  H94  1  0.32347000  0.81635000  0.97140000  1.0
+  H  H95  1  0.35314000  0.79086000  0.93406000  1.0
+  H  H96  1  0.27656000  0.63690000  0.49616000  1.0
+  H  H97  1  0.33416000  0.62058000  0.54384000  1.0
+  H  H98  1  0.38651000  0.58374000  0.53948000  1.0
+  H  H99  1  0.27990000  0.57247000  0.40186000  1.0
+  H  H100  1  0.35359000  0.53523000  0.38744000  1.0
+  H  H101  1  0.41242000  0.53989000  0.41551000  1.0
+  H  H102  1  0.22637000  0.60802000  0.37813000  1.0
+  H  H103  1  0.17423000  0.62394000  0.32859000  1.0
+  H  H104  1  0.12755000  0.66451000  0.32867000  1.0
+  H  H105  1  0.21407000  0.66915000  0.47490000  1.0
+  H  H106  1  0.15171000  0.71933000  0.48034000  1.0
+  H  H107  1  0.10883000  0.73485000  0.44283000  1.0
+  H  H108  1  0.19959000  0.41830000  0.58709000  1.0
+  H  H109  1  0.23359000  0.47498000  0.58746000  1.0
+  H  H110  1  0.29875000  0.48202000  0.56905000  1.0
+  H  H111  1  0.28403000  0.32348000  0.54380000  1.0
+  H  H112  1  0.36374000  0.32782000  0.51394000  1.0
+  H  H113  1  0.39428000  0.37144000  0.50913000  1.0
+  H  H114  1  0.22242000  0.29214000  0.55746000  1.0
+  H  H115  1  0.18604000  0.23479000  0.56091000  1.0
+  H  H116  1  0.12479000  0.22892000  0.58546000  1.0
+  H  H117  1  0.13873000  0.38809000  0.59922000  1.0
+  H  H118  1  0.06285000  0.38551000  0.63225000  1.0
+  H  H119  1  0.03668000  0.34206000  0.64488000  1.0
+  H  H120  1  0.93597000  0.85277000  0.44878000  1.0
+  H  H121  1  0.92669000  0.90891000  0.48289000  1.0
+  H  H122  1  0.07730000  0.93745000  0.44335000  1.0
+  H  H123  1  0.08284000  0.88412000  0.40646000  1.0
+  H  H124  1  0.96814000  0.99473000  0.56883000  1.0
+  H  H125  1  0.02340000  0.99130000  0.44346000  1.0
+  H  H126  1  0.02705000  0.03463000  0.59384000  1.0
+  H  H127  1  0.02264000  0.09202000  0.62516000  1.0
+  H  H128  1  0.95691000  0.14854000  0.53203000  1.0
+  H  H129  1  0.95779000  0.09084000  0.50148000  1.0
+  H  H130  1  0.01659000  0.06871000  0.45386000  1.0
+  H  H131  1  0.06199000  0.07225000  0.49039000  1.0
+  H  H132  1  0.13946000  0.05156000  0.41070000  1.0
+  H  H133  1  0.11982000  0.08837000  0.43918000  1.0
+  H  H134  1  0.07484000  0.07273000  0.40614000  1.0
+  H  H135  1  0.93254000  0.92547000  0.54949000  1.0
+  H  H136  1  0.99281000  0.90076000  0.53543000  1.0
+  H  H137  1  0.99623000  0.90723000  0.63243000  1.0
+  H  H138  1  0.98879000  0.87501000  0.59833000  1.0
+  H  H139  1  0.93542000  0.90885000  0.60950000  1.0
+  H  H140  1  0.50298000  0.62022000  0.91312000  1.0
+  H  H141  1  0.51378000  0.56942000  0.95667000  1.0
+  H  H142  1  0.34886000  0.58284000  0.98063000  1.0
+  H  H143  1  0.33752000  0.63111000  0.93495000  1.0
+  H  H144  1  0.50135000  0.48638000  0.05726000  1.0
+  H  H145  1  0.37130000  0.51833000  0.96308000  1.0
+  H  H146  1  0.44902000  0.45729000  0.10127000  1.0
+  H  H147  1  0.44743000  0.39954000  0.13442000  1.0
+  H  H148  1  0.42144000  0.34370000  0.03763000  1.0
+  H  H149  1  0.42766000  0.40126000  0.00364000  1.0
+  H  H150  1  0.35595000  0.43986000  0.97711000  1.0
+  H  H151  1  0.33832000  0.44222000  0.02385000  1.0
+  H  H152  1  0.22638000  0.48279000  0.97470000  1.0
+  H  H153  1  0.24923000  0.44258000  0.99953000  1.0
+  H  H154  1  0.27099000  0.45033000  0.95379000  1.0
+  H  H155  1  0.54864000  0.54562000  0.02127000  1.0
+  H  H156  1  0.49854000  0.58307000  0.02408000  1.0
+  H  H157  1  0.55530000  0.56921000  0.11220000  1.0
+  H  H158  1  0.55125000  0.60064000  0.07502000  1.0
+  H  H159  1  0.59247000  0.55771000  0.07343000  1.0
+  H  H160  1  0.93324000  0.85297000  0.12675000  1.0
+  H  H161  1  0.90965000  0.85607000  0.06892000  1.0
+  H  H162  1  0.91788000  0.89569000  0.04031000  1.0
+  H  H163  1  0.99713000  0.94101000  0.18104000  1.0
+  H  H164  1  0.00969000  0.99647000  0.15358000  1.0
+  H  H165  1  0.98988000  0.00739000  0.10780000  1.0
+  H  H166  1  0.00791000  0.90782000  0.22565000  1.0
+  H  H167  1  0.02852000  0.90123000  0.28659000  1.0
+  H  H168  1  0.01499000  0.85947000  0.31195000  1.0
+  H  H169  1  0.94925000  0.81860000  0.16873000  1.0
+  H  H170  1  0.92885000  0.76412000  0.19801000  1.0
+  H  H171  1  0.93881000  0.75798000  0.24640000  1.0
+  H  H172  1  0.97416000  0.04827000  0.81332000  1.0
+  H  H173  1  0.00168000  0.99129000  0.84071000  1.0
+  H  H174  1  0.00721000  0.98900000  0.88970000  1.0
+  H  H175  1  0.92226000  0.14062000  0.87665000  1.0
+  H  H176  1  0.89625000  0.13223000  0.93528000  1.0
+  H  H177  1  0.90027000  0.08486000  0.95421000  1.0
+  H  H178  1  0.92303000  0.17422000  0.83350000  1.0
+  H  H179  1  0.89833000  0.23135000  0.80747000  1.0
+  H  H180  1  0.90486000  0.23918000  0.75910000  1.0
+  H  H181  1  0.98839000  0.08408000  0.77208000  1.0
+  H  H182  1  0.00214000  0.09009000  0.71111000  1.0
+  H  H183  1  0.98442000  0.13289000  0.68662000  1.0
+  H  H184  1  0.50647000  0.34217000  0.38589000  1.0
+  H  H185  1  0.54051000  0.35208000  0.44220000  1.0
+  H  H186  1  0.54129000  0.39968000  0.45771000  1.0
+  H  H187  1  0.45399000  0.43368000  0.31787000  1.0
+  H  H188  1  0.43075000  0.49081000  0.34060000  1.0
+  H  H189  1  0.43518000  0.49552000  0.38884000  1.0
+  H  H190  1  0.43462000  0.39856000  0.27940000  1.0
+  H  H191  1  0.41939000  0.39287000  0.21826000  1.0
+  H  H192  1  0.43880000  0.35022000  0.19569000  1.0
+  H  H193  1  0.50703000  0.30914000  0.34297000  1.0
+  H  H194  1  0.53223000  0.25247000  0.31824000  1.0
+  H  H195  1  0.52428000  0.24533000  0.27024000  1.0
+  H  H196  1  0.43287000  0.55625000  0.67910000  1.0
+  H  H197  1  0.42146000  0.49919000  0.65678000  1.0
+  H  H198  1  0.43871000  0.48723000  0.61120000  1.0
+  H  H199  1  0.48960000  0.64333000  0.61501000  1.0
+  H  H200  1  0.51176000  0.63793000  0.55714000  1.0
+  H  H201  1  0.50316000  0.59693000  0.53268000  1.0
+  H  H202  1  0.47784000  0.67876000  0.65513000  1.0
+  H  H203  1  0.49638000  0.73495000  0.67856000  1.0
+  H  H204  1  0.48726000  0.74353000  0.72631000  1.0
+  H  H205  1  0.42321000  0.59149000  0.72109000  1.0
+  H  H206  1  0.40468000  0.59979000  0.78149000  1.0
+  H  H207  1  0.41688000  0.64245000  0.80312000  1.0
+  C  C208  1  0.95614000  0.03050000  0.93546000  1.0
+  C  C209  1  0.06590000  0.05569000  0.03480000  1.0
+  C  C210  1  0.89727000  0.04361000  0.03519000  1.0
+  C  C211  1  0.95635000  0.95917000  0.06079000  1.0
+  C  C212  1  0.84190000  0.93671000  0.96124000  1.0
+  C  C213  1  0.01240000  0.94229000  0.97975000  1.0
+  C  C214  1  0.47766000  0.45476000  0.43887000  1.0
+  C  C215  1  0.58495000  0.55386000  0.46015000  1.0
+  C  C216  1  0.41562000  0.54938000  0.48208000  1.0
+  C  C217  1  0.46946000  0.53312000  0.55910000  1.0
+  C  C218  1  0.36053000  0.43473000  0.53485000  1.0
+  C  C219  1  0.52825000  0.44516000  0.53412000  1.0
+  C  C220  1  0.02628000  0.82594000  0.41912000  1.0
+  C  C221  1  0.02154000  0.78166000  0.37993000  1.0
+  C  C222  1  0.95678000  0.73705000  0.39363000  1.0
+  C  C223  1  0.87319000  0.71675000  0.38238000  1.0
+  C  C224  1  0.94950000  0.81218000  0.28982000  1.0
+  C  C225  1  0.96074000  0.76946000  0.33455000  1.0
+  C  C226  1  0.02969000  0.72180000  0.35293000  1.0
+  C  C227  1  0.11393000  0.71074000  0.37820000  1.0
+  C  C228  1  0.99192000  0.75190000  0.36514000  1.0
+  C  C229  1  0.01488000  0.15764000  0.58971000  1.0
+  C  C230  1  0.99692000  0.20925000  0.61780000  1.0
+  C  C231  1  0.92325000  0.25627000  0.60541000  1.0
+  C  C232  1  0.84098000  0.28427000  0.62225000  1.0
+  C  C233  1  0.91863000  0.18692000  0.71268000  1.0
+  C  C234  1  0.92661000  0.21880000  0.66061000  1.0
+  C  C235  1  0.99096000  0.26601000  0.64888000  1.0
+  C  C236  1  0.07812000  0.27651000  0.62972000  1.0
+  C  C237  1  0.95873000  0.23768000  0.63331000  1.0
+  C  C238  1  0.41921000  0.33655000  0.11077000  1.0
+  C  C239  1  0.43404000  0.27649000  0.12697000  1.0
+  C  C240  1  0.50446000  0.22830000  0.11854000  1.0
+  C  C241  1  0.58986000  0.20236000  0.13044000  1.0
+  C  C242  1  0.50491000  0.29804000  0.22212000  1.0
+  C  C243  1  0.49668000  0.26032000  0.17541000  1.0
+  C  C244  1  0.43176000  0.21747000  0.15886000  1.0
+  C  C245  1  0.34603000  0.20665000  0.14066000  1.0
+  C  C246  1  0.46681000  0.24559000  0.14514000  1.0
+  C  C247  1  0.41118000  0.65265000  0.88859000  1.0
+  C  C248  1  0.41288000  0.71286000  0.87636000  1.0
+  C  C249  1  0.47372000  0.76087000  0.88168000  1.0
+  C  C250  1  0.55686000  0.78169000  0.86923000  1.0
+  C  C251  1  0.47918000  0.69246000  0.77579000  1.0
+  C  C252  1  0.46896000  0.72680000  0.82579000  1.0
+  C  C253  1  0.39669000  0.77202000  0.84343000  1.0
+  C  C254  1  0.31373000  0.78570000  0.86985000  1.0
+  C  C255  1  0.43778000  0.74340000  0.85643000  1.0
+  C  C256  1  0.76785000  0.92778000  0.91786000  1.0
+  C  C257  1  0.72753000  0.90697000  0.90558000  1.0
+  C  C258  1  0.77807000  0.95971000  0.89864000  1.0
+  C  C259  1  0.78465000  0.88310000  0.96614000  1.0
+  C  C260  1  0.74358000  0.86350000  0.95360000  1.0
+  C  C261  1  0.81092000  0.86942000  0.99679000  1.0
+  C  C262  1  0.61821000  0.79802000  0.91637000  1.0
+  C  C263  1  0.65639000  0.82009000  0.92858000  1.0
+  C  C264  1  0.60795000  0.76648000  0.93644000  1.0
+  C  C265  1  0.60128000  0.84067000  0.86633000  1.0
+  C  C266  1  0.64071000  0.86195000  0.87885000  1.0
+  C  C267  1  0.57339000  0.85238000  0.83558000  1.0
+  C  C268  1  0.79758000  0.91582000  0.94836000  1.0
+  C  C269  1  0.71394000  0.87453000  0.92312000  1.0
+  C  C270  1  0.59109000  0.80788000  0.88461000  1.0
+  C  C271  1  0.66995000  0.85208000  0.90995000  1.0
+  C  C272  1  0.81472000  0.04709000  0.07453000  1.0
+  C  C273  1  0.77003000  0.06770000  0.08726000  1.0
+  C  C274  1  0.82939000  0.01329000  0.09110000  1.0
+  C  C275  1  0.82428000  0.09442000  0.02934000  1.0
+  C  C276  1  0.77525000  0.11035000  0.03851000  1.0
+  C  C277  1  0.85330000  0.11407000  0.00540000  1.0
+  C  C278  1  0.65215000  0.18437000  0.08257000  1.0
+  C  C279  1  0.69123000  0.16010000  0.06889000  1.0
+  C  C280  1  0.63954000  0.21766000  0.06406000  1.0
+  C  C281  1  0.63963000  0.14076000  0.13135000  1.0
+  C  C282  1  0.67932000  0.11682000  0.11695000  1.0
+  C  C283  1  0.61421000  0.13024000  0.16266000  1.0
+  C  C284  1  0.84445000  0.06130000  0.04609000  1.0
+  C  C285  1  0.75006000  0.10045000  0.07013000  1.0
+  C  C286  1  0.62656000  0.17489000  0.11430000  1.0
+  C  C287  1  0.70581000  0.12561000  0.08535000  1.0
+  C  C288  1  0.58861000  0.38809000  0.53252000  1.0
+  C  C289  1  0.63730000  0.36952000  0.53912000  1.0
+  C  C290  1  0.55010000  0.36781000  0.51817000  1.0
+  C  C291  1  0.62045000  0.44202000  0.55910000  1.0
+  C  C292  1  0.66548000  0.42043000  0.57069000  1.0
+  C  C293  1  0.61668000  0.47920000  0.56697000  1.0
+  C  C294  1  0.79731000  0.34734000  0.61456000  1.0
+  C  C295  1  0.75670000  0.37093000  0.59997000  1.0
+  C  C296  1  0.83290000  0.36152000  0.63777000  1.0
+  C  C297  1  0.76443000  0.29681000  0.58247000  1.0
+  C  C298  1  0.72443000  0.32079000  0.56860000  1.0
+  C  C299  1  0.76718000  0.26018000  0.57198000  1.0
+  C  C300  1  0.57994000  0.42534000  0.54140000  1.0
+  C  C301  1  0.67431000  0.38339000  0.56163000  1.0
+  C  C302  1  0.80080000  0.31001000  0.60597000  1.0
+  C  C303  1  0.71946000  0.35847000  0.57640000  1.0
+  C  C304  1  0.66999000  0.56311000  0.42805000  1.0
+  C  C305  1  0.71044000  0.58532000  0.41798000  1.0
+  C  C306  1  0.67209000  0.52735000  0.41563000  1.0
+  C  C307  1  0.63078000  0.61287000  0.46302000  1.0
+  C  C308  1  0.67301000  0.63365000  0.45388000  1.0
+  C  C309  1  0.59223000  0.62856000  0.48544000  1.0
+  C  C310  1  0.79772000  0.70385000  0.42117000  1.0
+  C  C311  1  0.75897000  0.68095000  0.43190000  1.0
+  C  C312  1  0.79691000  0.73900000  0.43544000  1.0
+  C  C313  1  0.83712000  0.65500000  0.38472000  1.0
+  C  C314  1  0.79746000  0.63273000  0.39584000  1.0
+  C  C315  1  0.87551000  0.64080000  0.36106000  1.0
+  C  C316  1  0.62856000  0.57710000  0.45002000  1.0
+  C  C317  1  0.71320000  0.62108000  0.43054000  1.0
+  C  C318  1  0.83656000  0.69110000  0.39686000  1.0
+  C  C319  1  0.75704000  0.64506000  0.41937000  1.0
+  C  C320  1  0.15329000  0.06024000  0.06741000  1.0
+  C  C321  1  0.19382000  0.08119000  0.07904000  1.0
+  C  C322  1  0.15789000  0.02271000  0.07599000  1.0
+  C  C323  1  0.10690000  0.11631000  0.04448000  1.0
+  C  C324  1  0.14663000  0.13636000  0.05850000  1.0
+  C  C325  1  0.06719000  0.13629000  0.02515000  1.0
+  C  C326  1  0.27114000  0.20176000  0.09870000  1.0
+  C  C327  1  0.23325000  0.18064000  0.08428000  1.0
+  C  C328  1  0.26796000  0.23958000  0.09111000  1.0
+  C  C329  1  0.31788000  0.14590000  0.12190000  1.0
+  C  C330  1  0.28011000  0.12546000  0.10628000  1.0
+  C  C331  1  0.35971000  0.12699000  0.14024000  1.0
+  C  C332  1  0.10912000  0.07745000  0.04896000  1.0
+  C  C333  1  0.19179000  0.11961000  0.07506000  1.0
+  C  C334  1  0.31208000  0.18450000  0.11956000  1.0
+  C  C335  1  0.23540000  0.14210000  0.08872000  1.0
+  C  C336  1  0.10636000  0.91553000  0.98416000  1.0
+  C  C337  1  0.15016000  0.89556000  0.96922000  1.0
+  C  C338  1  0.10860000  0.92547000  0.01971000  1.0
+  C  C339  1  0.06291000  0.91633000  0.92683000  1.0
+  C  C340  1  0.10913000  0.90027000  0.91208000  1.0
+  C  C341  1  0.01948000  0.92256000  0.90449000  1.0
+  C  C342  1  0.23545000  0.83032000  0.86481000  1.0
+  C  C343  1  0.19705000  0.85399000  0.88034000  1.0
+  C  C344  1  0.23151000  0.82379000  0.82829000  1.0
+  C  C345  1  0.28016000  0.82356000  0.92191000  1.0
+  C  C346  1  0.24046000  0.84740000  0.93683000  1.0
+  C  C347  1  0.32141000  0.80919000  0.94368000  1.0
+  C  C348  1  0.06109000  0.92491000  0.96325000  1.0
+  C  C349  1  0.15230000  0.88684000  0.93284000  1.0
+  C  C350  1  0.27691000  0.81408000  0.88570000  1.0
+  C  C351  1  0.19752000  0.86292000  0.91655000  1.0
+  C  C352  1  0.33773000  0.59459000  0.49272000  1.0
+  C  C353  1  0.29336000  0.61569000  0.47950000  1.0
+  C  C354  1  0.35440000  0.60025000  0.52735000  1.0
+  C  C355  1  0.34254000  0.56227000  0.43753000  1.0
+  C  C356  1  0.29503000  0.58014000  0.42693000  1.0
+  C  C357  1  0.37064000  0.54243000  0.41245000  1.0
+  C  C358  1  0.17239000  0.65390000  0.37779000  1.0
+  C  C359  1  0.21046000  0.62990000  0.39418000  1.0
+  C  C360  1  0.15722000  0.64726000  0.34283000  1.0
+  C  C361  1  0.16464000  0.68844000  0.43229000  1.0
+  C  C362  1  0.20346000  0.66419000  0.44795000  1.0
+  C  C363  1  0.14054000  0.71626000  0.45287000  1.0
+  C  C364  1  0.36431000  0.56841000  0.47093000  1.0
+  C  C365  1  0.27165000  0.60957000  0.44585000  1.0
+  C  C366  1  0.15035000  0.68394000  0.39660000  1.0
+  C  C367  1  0.22767000  0.63455000  0.42939000  1.0
+  C  C368  1  0.27278000  0.42697000  0.56378000  1.0
+  C  C369  1  0.23215000  0.40493000  0.57337000  1.0
+  C  C370  1  0.26816000  0.46369000  0.57367000  1.0
+  C  C371  1  0.32026000  0.37372000  0.53844000  1.0
+  C  C372  1  0.27940000  0.35220000  0.54933000  1.0
+  C  C373  1  0.36235000  0.35673000  0.51965000  1.0
+  C  C374  1  0.15298000  0.28366000  0.58673000  1.0
+  C  C375  1  0.19154000  0.30559000  0.57287000  1.0
+  C  C376  1  0.15511000  0.24665000  0.57778000  1.0
+  C  C377  1  0.10729000  0.33793000  0.61151000  1.0
+  C  C378  1  0.14509000  0.35914000  0.59612000  1.0
+  C  C379  1  0.06633000  0.35598000  0.63066000  1.0
+  C  C380  1  0.31732000  0.41163000  0.54569000  1.0
+  C  C381  1  0.23398000  0.36715000  0.56655000  1.0
+  C  C382  1  0.11237000  0.29957000  0.60836000  1.0
+  C  C383  1  0.18987000  0.34366000  0.57850000  1.0
+  C  C384  1  0.01182000  0.86372000  0.42725000  1.0
+  C  C385  1  0.96604000  0.87196000  0.44680000  1.0
+  C  C386  1  0.96127000  0.90338000  0.46679000  1.0
+  C  C387  1  0.00247000  0.92638000  0.46715000  1.0
+  C  C388  1  0.04550000  0.91966000  0.44436000  1.0
+  C  C389  1  0.04916000  0.88912000  0.42359000  1.0
+  C  C390  1  0.99993000  0.95930000  0.48871000  1.0
+  C  C391  1  0.98693000  0.95964000  0.52535000  1.0
+  C  C392  1  0.98337000  0.99323000  0.54199000  1.0
+  C  C393  1  0.00021000  0.02479000  0.52514000  1.0
+  C  C394  1  0.02001000  0.02300000  0.49007000  1.0
+  C  C395  1  0.01428000  0.99132000  0.47156000  1.0
+  C  C396  1  0.99468000  0.05887000  0.54478000  1.0
+  C  C397  1  0.01015000  0.05915000  0.58046000  1.0
+  C  C398  1  0.00725000  0.09183000  0.59843000  1.0
+  C  C399  1  0.99092000  0.12451000  0.58039000  1.0
+  C  C400  1  0.96948000  0.12355000  0.54639000  1.0
+  C  C401  1  0.97157000  0.09080000  0.52855000  1.0
+  C  C402  1  0.04655000  0.05357000  0.47101000  1.0
+  C  C403  1  0.10593000  0.06435000  0.42578000  1.0
+  C  C404  1  0.97584000  0.92609000  0.54773000  1.0
+  C  C405  1  0.97836000  0.90359000  0.60611000  1.0
+  C  C406  1  0.41921000  0.62875000  0.92034000  1.0
+  C  C407  1  0.46932000  0.61252000  0.92821000  1.0
+  C  C408  1  0.47559000  0.58379000  0.95330000  1.0
+  C  C409  1  0.43206000  0.57216000  0.97193000  1.0
+  C  C410  1  0.38294000  0.59105000  0.96633000  1.0
+  C  C411  1  0.37635000  0.61861000  0.94029000  1.0
+  C  C412  1  0.43501000  0.53725000  0.99289000  1.0
+  C  C413  1  0.47119000  0.52863000  0.02071000  1.0
+  C  C414  1  0.47160000  0.49405000  0.03756000  1.0
+  C  C415  1  0.43356000  0.46963000  0.03030000  1.0
+  C  C416  1  0.39390000  0.48015000  0.00523000  1.0
+  C  C417  1  0.39829000  0.51220000  0.98487000  1.0
+  C  C418  1  0.43596000  0.43401000  0.04997000  1.0
+  C  C419  1  0.44374000  0.43272000  0.08687000  1.0
+  C  C420  1  0.44243000  0.39992000  0.10588000  1.0
+  C  C421  1  0.43199000  0.36803000  0.08869000  1.0
+  C  C422  1  0.42828000  0.36827000  0.05158000  1.0
+  C  C423  1  0.43101000  0.40124000  0.03222000  1.0
+  C  C424  1  0.34664000  0.45845000  0.99947000  1.0
+  C  C425  1  0.26083000  0.46319000  0.97950000  1.0
+  C  C426  1  0.51007000  0.55461000  0.03308000  1.0
+  C  C427  1  0.55487000  0.57118000  0.08279000  1.0
+  C  C428  1  0.94172000  0.90096000  0.09599000  1.0
+  C  C429  1  0.94673000  0.87991000  0.12752000  1.0
+  C  C430  1  0.92168000  0.88378000  0.06658000  1.0
+  C  C431  1  0.97842000  0.95120000  0.12658000  1.0
+  C  C432  1  0.98276000  0.92892000  0.15760000  1.0
+  C  C433  1  0.99372000  0.98708000  0.12904000  1.0
+  C  C434  1  0.99225000  0.86052000  0.25597000  1.0
+  C  C435  1  0.99294000  0.88128000  0.22422000  1.0
+  C  C436  1  0.01249000  0.87470000  0.28691000  1.0
+  C  C437  1  0.95658000  0.81111000  0.22408000  1.0
+  C  C438  1  0.95946000  0.83185000  0.19254000  1.0
+  C  C439  1  0.93993000  0.77560000  0.22290000  1.0
+  C  C440  1  0.95827000  0.93718000  0.09481000  1.0
+  C  C441  1  0.96836000  0.89261000  0.15867000  1.0
+  C  C442  1  0.96985000  0.82652000  0.25626000  1.0
+  C  C443  1  0.97376000  0.86841000  0.19210000  1.0
+  C  C444  1  0.96965000  0.03873000  0.86898000  1.0
+  C  C445  1  0.96508000  0.06110000  0.83820000  1.0
+  C  C446  1  0.99270000  0.00340000  0.86621000  1.0
+  C  C447  1  0.93427000  0.08977000  0.90321000  1.0
+  C  C448  1  0.93591000  0.11258000  0.87322000  1.0
+  C  C449  1  0.91014000  0.10369000  0.93342000  1.0
+  C  C450  1  0.92782000  0.18370000  0.77835000  1.0
+  C  C451  1  0.93380000  0.16147000  0.80896000  1.0
+  C  C452  1  0.90868000  0.22030000  0.78170000  1.0
+  C  C453  1  0.96562000  0.13310000  0.74347000  1.0
+  C  C454  1  0.97036000  0.11133000  0.77454000  1.0
+  C  C455  1  0.98453000  0.11790000  0.71166000  1.0
+  C  C456  1  0.95377000  0.05301000  0.90204000  1.0
+  C  C457  1  0.95148000  0.09908000  0.83992000  1.0
+  C  C458  1  0.94072000  0.16879000  0.74508000  1.0
+  C  C459  1  0.95177000  0.12416000  0.80750000  1.0
+  C  C460  1  0.49961000  0.39415000  0.40934000  1.0
+  C  C461  1  0.49431000  0.37051000  0.38103000  1.0
+  C  C462  1  0.52737000  0.38080000  0.43907000  1.0
+  C  C463  1  0.46370000  0.44441000  0.37229000  1.0
+  C  C464  1  0.46467000  0.42131000  0.34329000  1.0
+  C  C465  1  0.44321000  0.47982000  0.36650000  1.0
+  C  C466  1  0.45811000  0.35028000  0.25227000  1.0
+  C  C467  1  0.45383000  0.37158000  0.28266000  1.0
+  C  C468  1  0.43800000  0.36535000  0.22001000  1.0
+  C  C469  1  0.49928000  0.29989000  0.28817000  1.0
+  C  C470  1  0.49407000  0.32167000  0.31814000  1.0
+  C  C471  1  0.52037000  0.26368000  0.29231000  1.0
+  C  C472  1  0.48079000  0.43120000  0.40637000  1.0
+  C  C473  1  0.47697000  0.38350000  0.34718000  1.0
+  C  C474  1  0.48396000  0.31493000  0.25468000  1.0
+  C  C475  1  0.47461000  0.35864000  0.31580000  1.0
+  C  C476  1  0.44894000  0.54413000  0.62490000  1.0
+  C  C477  1  0.44544000  0.56764000  0.65416000  1.0
+  C  C478  1  0.43534000  0.50809000  0.63092000  1.0
+  C  C479  1  0.48208000  0.59369000  0.58897000  1.0
+  C  C480  1  0.47765000  0.61607000  0.61869000  1.0
+  C  C481  1  0.50033000  0.61000000  0.55769000  1.0
+  C  C482  1  0.47091000  0.68889000  0.70986000  1.0
+  C  C483  1  0.46822000  0.66654000  0.68031000  1.0
+  C  C484  1  0.48622000  0.72460000  0.70473000  1.0
+  C  C485  1  0.43804000  0.64040000  0.74701000  1.0
+  C  C486  1  0.43718000  0.61822000  0.71708000  1.0
+  C  C487  1  0.41952000  0.62667000  0.77937000  1.0
+  C  C488  1  0.46708000  0.55699000  0.59127000  1.0
+  C  C489  1  0.45864000  0.60430000  0.65172000  1.0
+  C  C490  1  0.45864000  0.67512000  0.74396000  1.0
+  C  C491  1  0.45461000  0.62986000  0.68332000  1.0
+  O  O492  1  0.07148000  0.02265000  0.02247000  1.0
+  O  O493  1  0.01677000  0.06672000  0.03407000  1.0
+  O  O494  1  0.90461000  0.01490000  0.01546000  1.0
+  O  O495  1  0.94005000  0.05833000  0.03977000  1.0
+  O  O496  1  0.98458000  0.04087000  0.96215000  1.0
+  O  O497  1  0.92563000  0.00323000  0.93958000  1.0
+  O  O498  1  0.83782000  0.97084000  0.97035000  1.0
+  O  O499  1  0.88980000  0.92335000  0.96521000  1.0
+  O  O500  1  0.99981000  0.97767000  0.97723000  1.0
+  O  O501  1  0.97059000  0.92457000  0.98348000  1.0
+  O  O502  1  0.91681000  0.95764000  0.03864000  1.0
+  O  O503  1  0.99473000  0.97961000  0.05250000  1.0
+  O  O504  1  0.59029000  0.52554000  0.48176000  1.0
+  O  O505  1  0.53644000  0.55989000  0.45052000  1.0
+  O  O506  1  0.42711000  0.51401000  0.47887000  1.0
+  O  O507  1  0.45798000  0.56680000  0.48114000  1.0
+  O  O508  1  0.50580000  0.48353000  0.44076000  1.0
+  O  O509  1  0.44775000  0.44562000  0.46600000  1.0
+  O  O510  1  0.35525000  0.46443000  0.51496000  1.0
+  O  O511  1  0.40891000  0.42742000  0.54344000  1.0
+  O  O512  1  0.52017000  0.47456000  0.51403000  1.0
+  O  O513  1  0.48435000  0.43341000  0.54472000  1.0
+  O  O514  1  0.43172000  0.51160000  0.55276000  1.0
+  O  O515  1  0.50806000  0.53513000  0.53596000  1.0
+  O  O516  1  0.06435000  0.81023000  0.43397000  1.0
+  O  O517  1  0.99281000  0.80768000  0.39897000  1.0
+  O  O518  1  0.92547000  0.71010000  0.38674000  1.0
+  O  O519  1  0.85523000  0.74437000  0.36673000  1.0
+  O  O520  1  0.90411000  0.82140000  0.29759000  1.0
+  O  O521  1  0.98401000  0.79609000  0.31463000  1.0
+  O  O522  1  0.06260000  0.70479000  0.37705000  1.0
+  O  O523  1  0.13084000  0.73720000  0.36295000  1.0
+  O  O524  1  0.06243000  0.15548000  0.59366000  1.0
+  O  O525  1  0.98777000  0.19159000  0.58677000  1.0
+  O  O526  1  0.89177000  0.28619000  0.61315000  1.0
+  O  O527  1  0.82758000  0.26116000  0.64357000  1.0
+  O  O528  1  0.87089000  0.18925000  0.70945000  1.0
+  O  O529  1  0.95175000  0.19466000  0.68474000  1.0
+  O  O530  1  0.02525000  0.28175000  0.62674000  1.0
+  O  O531  1  0.09807000  0.25302000  0.65006000  1.0
+  O  O532  1  0.37787000  0.33870000  0.12729000  1.0
+  O  O533  1  0.45717000  0.30809000  0.11677000  1.0
+  O  O534  1  0.53769000  0.19948000  0.12842000  1.0
+  O  O535  1  0.60733000  0.22860000  0.14422000  1.0
+  O  O536  1  0.55064000  0.30241000  0.21474000  1.0
+  O  O537  1  0.47075000  0.28529000  0.19753000  1.0
+  O  O538  1  0.39850000  0.20350000  0.13595000  1.0
+  O  O539  1  0.32604000  0.22844000  0.16166000  1.0
+  O  O540  1  0.37931000  0.64537000  0.86626000  1.0
+  O  O541  1  0.44342000  0.68059000  0.88268000  1.0
+  O  O542  1  0.50409000  0.78752000  0.87038000  1.0
+  O  O543  1  0.57718000  0.75382000  0.85655000  1.0
+  O  O544  1  0.52680000  0.69292000  0.77804000  1.0
+  O  O545  1  0.44632000  0.70230000  0.80413000  1.0
+  O  O546  1  0.36540000  0.79062000  0.86694000  1.0
+  O  O547  1  0.29639000  0.75812000  0.85855000  1.0
+  O  O548  1  0.99865000  0.92871000  0.58172000  1.0
+  O  O549  1  0.08909000  0.03829000  0.45067000  1.0
+  O  O550  1  0.51182000  0.55328000  0.07064000  1.0
+  O  O551  1  0.30218000  0.48271000  0.99193000  1.0
```

### Comparing `moftransformer-2.0.0/moftransformer/examples/dataset/val/acs+N270+E33.cif` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 data_image0
-_chemical_formula_structural       C72Ga6H24O26
-_chemical_formula_sum              "C72 Ga6 H24 O26"
-_cell_length_a       22.242
-_cell_length_b       22.4662
-_cell_length_c       22.6575
-_cell_angle_alpha    90
-_cell_angle_beta     90
-_cell_angle_gamma    118.388
+_chemical_formula_structural       Zn8H24C48O26
+_chemical_formula_sum              "Zn8 H24 C48 O26"
+_cell_length_a       18.4202
+_cell_length_b       18.4202
+_cell_length_c       18.4202
+_cell_angle_alpha    60
+_cell_angle_beta     60.0001
+_cell_angle_gamma    60.0001
 
 _space_group_name_H-M_alt    "P 1"
 _space_group_IT_number       1
 
 loop_
   _space_group_symop_operation_xyz
   'x, y, z'
@@ -19,135 +19,113 @@
   _atom_site_type_symbol
   _atom_site_label
   _atom_site_symmetry_multiplicity
   _atom_site_fract_x
   _atom_site_fract_y
   _atom_site_fract_z
   _atom_site_occupancy
-  C   C1        1.0  0.46099  0.76288  0.39553  1.0000
-  C   C2        1.0  0.46885  0.56983  0.39492  1.0000
-  C   C3        1.0  0.26887  0.56589  0.39516  1.0000
-  C   C4        1.0  0.26889  0.56595  0.23826  1.0000
-  C   C5        1.0  0.46843  0.56933  0.23848  1.0000
-  C   C6        1.0  0.46097  0.76294  0.23781  1.0000
-  C   C7        1.0  0.67192  0.16628  0.89554  1.0000
-  C   C8        1.0  0.66497  0.35998  0.89482  1.0000
-  C   C9        1.0  0.86412  0.36498  0.89545  1.0000
-  C   C10       1.0  0.86458  0.36343  0.73824  1.0000
-  C   C11       1.0  0.66324  0.35822  0.73822  1.0000
-  C   C12       1.0  0.67309  0.16690  0.73791  1.0000
-  C   C13       1.0  0.91608  0.39224  0.94103  1.0000
-  C   C14       1.0  0.95976  0.41280  0.97920  1.0000
-  C   C15       1.0  0.01255  0.43711  0.02476  1.0000
-  C   C16       1.0  0.06501  0.42009  0.02342  1.0000
-  C   C17       1.0  0.11859  0.44690  0.06444  1.0000
-  C   C18       1.0  0.12071  0.49084  0.10870  1.0000
-  C   C19       1.0  0.06811  0.50770  0.11016  1.0000
-  C   C20       1.0  0.01462  0.48102  0.06904  1.0000
-  C   C21       1.0  0.17512  0.51771  0.15286  1.0000
-  C   C22       1.0  0.21784  0.54024  0.19180  1.0000
-  C   C23       1.0  0.64766  0.11588  0.69140  1.0000
-  C   C24       1.0  0.62269  0.07317  0.65270  1.0000
-  C   C25       1.0  0.59525  0.01955  0.60787  1.0000
-  C   C26       1.0  0.54784  0.01528  0.56548  1.0000
-  C   C27       1.0  0.52002  0.96164  0.52491  1.0000
-  C   C28       1.0  0.53832  0.91048  0.52516  1.0000
-  C   C29       1.0  0.58578  0.91474  0.56748  1.0000
-  C   C30       1.0  0.61356  0.96836  0.60812  1.0000
-  C   C31       1.0  0.50938  0.85582  0.48140  1.0000
-  C   C32       1.0  0.48586  0.81346  0.44234  1.0000
-  C   C33       1.0  0.49260  0.54328  0.19125  1.0000
-  C   C34       1.0  0.51206  0.52055  0.15162  1.0000
-  C   C35       1.0  0.54055  0.49424  0.10756  1.0000
-  C   C36       1.0  0.50809  0.46915  0.05390  1.0000
-  C   C37       1.0  0.53385  0.44015  0.01342  1.0000
-  C   C38       1.0  0.59262  0.43546  0.02537  1.0000
-  C   C39       1.0  0.62564  0.46117  0.07885  1.0000
-  C   C40       1.0  0.59972  0.49009  0.11948  1.0000
-  C   C41       1.0  0.61926  0.40680  0.98174  1.0000
-  C   C42       1.0  0.64023  0.38552  0.94206  1.0000
-  C   C43       1.0  0.91504  0.38919  0.69133  1.0000
-  C   C44       1.0  0.95731  0.41159  0.65201  1.0000
-  C   C45       1.0  0.01223  0.43836  0.60834  1.0000
-  C   C46       1.0  0.00231  0.45449  0.55106  1.0000
-  C   C47       1.0  0.05597  0.48058  0.51012  1.0000
-  C   C48       1.0  0.12091  0.49093  0.52482  1.0000
-  C   C49       1.0  0.13093  0.47513  0.58220  1.0000
-  C   C50       1.0  0.07725  0.44905  0.62318  1.0000
-  C   C51       1.0  0.17570  0.51750  0.48102  1.0000
-  C   C52       1.0  0.21813  0.54052  0.44188  1.0000
-  C   C53       1.0  0.64575  0.11455  0.94120  1.0000
-  C   C54       1.0  0.62234  0.07122  0.97938  1.0000
-  C   C55       1.0  0.59487  0.01905  0.02525  1.0000
-  C   C56       1.0  0.52929  0.99570  0.04810  1.0000
-  C   C57       1.0  0.50168  0.94223  0.08879  1.0000
-  C   C58       1.0  0.53866  0.91067  0.10844  1.0000
-  C   C59       1.0  0.60445  0.93429  0.08587  1.0000
-  C   C60       1.0  0.63205  0.98775  0.04510  1.0000
-  C   C61       1.0  0.50968  0.85639  0.15247  1.0000
-  C   C62       1.0  0.48595  0.81379  0.19130  1.0000
-  C   C63       1.0  0.63684  0.38231  0.69121  1.0000
-  C   C64       1.0  0.61778  0.40572  0.65184  1.0000
-  C   C65       1.0  0.59307  0.43639  0.60848  1.0000
-  C   C66       1.0  0.56274  0.47498  0.62649  1.0000
-  C   C67       1.0  0.53676  0.50327  0.58537  1.0000
-  C   C68       1.0  0.54146  0.49430  0.52510  1.0000
-  C   C69       1.0  0.57195  0.45591  0.50721  1.0000
-  C   C70       1.0  0.59786  0.42762  0.54826  1.0000
-  C   C71       1.0  0.51498  0.52299  0.48141  1.0000
-  C   C72       1.0  0.49435  0.54482  0.44194  1.0000
-  Ga  Ga1       1.0  0.48345  0.67567  0.31652  1.0000
-  Ga  Ga2       1.0  0.36088  0.55065  0.31682  1.0000
-  Ga  Ga3       1.0  0.35519  0.67334  0.31669  1.0000
-  Ga  Ga4       1.0  0.65057  0.25384  0.81696  1.0000
-  Ga  Ga5       1.0  0.77217  0.37896  0.81602  1.0000
-  Ga  Ga6       1.0  0.77877  0.25627  0.81733  1.0000
-  H   H1        1.0  0.06524  0.38676  0.99005  1.0000
-  H   H2        1.0  0.15848  0.43359  0.06093  1.0000
-  H   H3        1.0  0.06860  0.54201  0.14287  1.0000
-  H   H4        1.0  0.97547  0.49545  0.07168  1.0000
-  H   H5        1.0  0.53146  0.05274  0.56362  1.0000
-  H   H6        1.0  0.48393  0.96001  0.49315  1.0000
-  H   H7        1.0  0.60172  0.87693  0.56956  1.0000
-  H   H8        1.0  0.64926  0.96970  0.64018  1.0000
-  H   H9        1.0  0.46202  0.47037  0.04350  1.0000
-  H   H10       1.0  0.50764  0.42110  0.97274  1.0000
-  H   H11       1.0  0.67125  0.45906  0.08956  1.0000
-  H   H12       1.0  0.62526  0.50821  0.16066  1.0000
-  H   H13       1.0  0.95326  0.44670  0.53746  1.0000
-  H   H14       1.0  0.04672  0.49271  0.46674  1.0000
-  H   H15       1.0  0.17997  0.48278  0.59576  1.0000
-  H   H16       1.0  0.08644  0.43678  0.66654  1.0000
-  H   H17       1.0  0.49866  0.01790  0.03420  1.0000
-  H   H18       1.0  0.45102  0.92518  0.10466  1.0000
-  H   H19       1.0  0.63473  0.91149  0.09920  1.0000
-  H   H20       1.0  0.68229  0.00413  0.02842  1.0000
-  H   H21       1.0  0.55850  0.48264  0.67244  1.0000
-  H   H22       1.0  0.51236  0.53116  0.60100  1.0000
-  H   H23       1.0  0.57493  0.44705  0.46135  1.0000
-  H   H24       1.0  0.62095  0.39855  0.53265  1.0000
-  O   O1        1.0  0.50402  0.74288  0.37362  1.0000
-  O   O2        1.0  0.40734  0.52855  0.37334  1.0000
-  O   O3        1.0  0.28768  0.62747  0.37379  1.0000
-  O   O4        1.0  0.29324  0.52620  0.25901  1.0000
-  O   O5        1.0  0.50828  0.63180  0.25854  1.0000
-  O   O6        1.0  0.39752  0.74020  0.25833  1.0000
-  O   O7        1.0  0.50400  0.74291  0.25961  1.0000
-  O   O8        1.0  0.40717  0.52841  0.26055  1.0000
-  O   O9        1.0  0.28771  0.62757  0.25959  1.0000
-  O   O10       1.0  0.29319  0.52610  0.37444  1.0000
-  O   O11       1.0  0.50829  0.63210  0.37444  1.0000
-  O   O12       1.0  0.39755  0.74017  0.37504  1.0000
-  O   O13       1.0  0.39999  0.63335  0.31665  1.0000
-  O   O14       1.0  0.62944  0.18683  0.87367  1.0000
-  O   O15       1.0  0.72607  0.40120  0.87260  1.0000
-  O   O16       1.0  0.84606  0.30321  0.87460  1.0000
-  O   O17       1.0  0.84018  0.40319  0.75881  1.0000
-  O   O18       1.0  0.62463  0.29607  0.75905  1.0000
-  O   O19       1.0  0.73652  0.18951  0.75854  1.0000
-  O   O20       1.0  0.63006  0.18669  0.76006  1.0000
-  O   O21       1.0  0.72474  0.40025  0.75950  1.0000
-  O   O22       1.0  0.84623  0.30197  0.75997  1.0000
-  O   O23       1.0  0.83924  0.40401  0.87416  1.0000
-  O   O24       1.0  0.62549  0.29753  0.87474  1.0000
-  O   O25       1.0  0.73555  0.18878  0.87539  1.0000
-  O   O26       1.0  0.73392  0.29628  0.81674  1.0000
+  Zn  Zn1       1.0  0.70648  0.70648  0.88055  1.0000
+  Zn  Zn2       1.0  0.70648  0.88055  0.70648  1.0000
+  Zn  Zn3       1.0  0.88055  0.70648  0.70648  1.0000
+  Zn  Zn4       1.0  0.70648  0.70648  0.70648  1.0000
+  Zn  Zn5       1.0  0.29352  0.29352  0.11945  1.0000
+  Zn  Zn6       1.0  0.29352  0.11945  0.29352  1.0000
+  Zn  Zn7       1.0  0.29352  0.29352  0.29352  1.0000
+  Zn  Zn8       1.0  0.11945  0.29351  0.29352  1.0000
+  H   H1        1.0  0.54831  0.83516  0.06823  1.0000
+  H   H2        1.0  0.54831  0.06823  0.83516  1.0000
+  H   H3        1.0  0.06823  0.54831  0.54831  1.0000
+  H   H4        1.0  0.83516  0.54831  0.54831  1.0000
+  H   H5        1.0  0.54831  0.54831  0.83516  1.0000
+  H   H6        1.0  0.54831  0.54831  0.06823  1.0000
+  H   H7        1.0  0.06823  0.83516  0.54831  1.0000
+  H   H8        1.0  0.83516  0.06823  0.54831  1.0000
+  H   H9        1.0  0.54831  0.06823  0.54831  1.0000
+  H   H10       1.0  0.54831  0.83516  0.54831  1.0000
+  H   H11       1.0  0.06823  0.54831  0.83516  1.0000
+  H   H12       1.0  0.83516  0.54831  0.06823  1.0000
+  H   H13       1.0  0.45169  0.16484  0.93177  1.0000
+  H   H14       1.0  0.45169  0.93177  0.16484  1.0000
+  H   H15       1.0  0.16484  0.45169  0.45169  1.0000
+  H   H16       1.0  0.93177  0.45169  0.45169  1.0000
+  H   H17       1.0  0.93177  0.45169  0.16484  1.0000
+  H   H18       1.0  0.16485  0.45169  0.93177  1.0000
+  H   H19       1.0  0.45169  0.16484  0.45169  1.0000
+  H   H20       1.0  0.45169  0.93177  0.45169  1.0000
+  H   H21       1.0  0.16484  0.93177  0.45169  1.0000
+  H   H22       1.0  0.93177  0.16484  0.45169  1.0000
+  H   H23       1.0  0.45169  0.45169  0.16484  1.0000
+  H   H24       1.0  0.45169  0.45169  0.93177  1.0000
+  C   C1        1.0  0.61101  0.88899  0.88899  1.0000
+  C   C2        1.0  0.88899  0.61101  0.61101  1.0000
+  C   C3        1.0  0.61101  0.61101  0.88899  1.0000
+  C   C4        1.0  0.88899  0.88899  0.61101  1.0000
+  C   C5        1.0  0.61101  0.88899  0.61101  1.0000
+  C   C6        1.0  0.88899  0.61101  0.88899  1.0000
+  C   C7        1.0  0.38899  0.11101  0.11101  1.0000
+  C   C8        1.0  0.11101  0.38899  0.38899  1.0000
+  C   C9        1.0  0.11101  0.38899  0.11101  1.0000
+  C   C10       1.0  0.38899  0.11101  0.38899  1.0000
+  C   C11       1.0  0.11101  0.11101  0.38899  1.0000
+  C   C12       1.0  0.38899  0.38899  0.11101  1.0000
+  C   C13       1.0  0.55364  0.94636  0.94636  1.0000
+  C   C14       1.0  0.94636  0.55364  0.55364  1.0000
+  C   C15       1.0  0.55364  0.55364  0.94636  1.0000
+  C   C16       1.0  0.94636  0.94636  0.55364  1.0000
+  C   C17       1.0  0.55364  0.94636  0.55364  1.0000
+  C   C18       1.0  0.94636  0.55364  0.94636  1.0000
+  C   C19       1.0  0.44636  0.05364  0.05364  1.0000
+  C   C20       1.0  0.05364  0.44636  0.44636  1.0000
+  C   C21       1.0  0.05364  0.44636  0.05364  1.0000
+  C   C22       1.0  0.44636  0.05364  0.44636  1.0000
+  C   C23       1.0  0.05364  0.05364  0.44636  1.0000
+  C   C24       1.0  0.44636  0.44636  0.05364  1.0000
+  C   C25       1.0  0.52669  0.90740  0.03923  1.0000
+  C   C26       1.0  0.52669  0.03923  0.90740  1.0000
+  C   C27       1.0  0.03923  0.52669  0.52669  1.0000
+  C   C28       1.0  0.90740  0.52669  0.52669  1.0000
+  C   C29       1.0  0.52669  0.52669  0.90740  1.0000
+  C   C30       1.0  0.52669  0.52669  0.03923  1.0000
+  C   C31       1.0  0.03923  0.90740  0.52669  1.0000
+  C   C32       1.0  0.90740  0.03923  0.52669  1.0000
+  C   C33       1.0  0.52669  0.03923  0.52669  1.0000
+  C   C34       1.0  0.52669  0.90740  0.52669  1.0000
+  C   C35       1.0  0.03923  0.52669  0.90740  1.0000
+  C   C36       1.0  0.90740  0.52669  0.03923  1.0000
+  C   C37       1.0  0.47331  0.09260  0.96077  1.0000
+  C   C38       1.0  0.47331  0.96077  0.09260  1.0000
+  C   C39       1.0  0.09260  0.47331  0.47331  1.0000
+  C   C40       1.0  0.96077  0.47331  0.47331  1.0000
+  C   C41       1.0  0.96077  0.47331  0.09260  1.0000
+  C   C42       1.0  0.09260  0.47331  0.96077  1.0000
+  C   C43       1.0  0.47331  0.09260  0.47331  1.0000
+  C   C44       1.0  0.47331  0.96077  0.47331  1.0000
+  C   C45       1.0  0.09260  0.96077  0.47331  1.0000
+  C   C46       1.0  0.96077  0.09260  0.47331  1.0000
+  C   C47       1.0  0.47331  0.47331  0.09260  1.0000
+  C   C48       1.0  0.47331  0.47331  0.96077  1.0000
+  O   O1        1.0  0.75000  0.75000  0.75000  1.0000
+  O   O2        1.0  0.25000  0.25000  0.25000  1.0000
+  O   O3        1.0  0.63317  0.80498  0.92868  1.0000
+  O   O4        1.0  0.63317  0.92868  0.80498  1.0000
+  O   O5        1.0  0.92868  0.63317  0.63317  1.0000
+  O   O6        1.0  0.80498  0.63317  0.63317  1.0000
+  O   O7        1.0  0.63317  0.63317  0.80498  1.0000
+  O   O8        1.0  0.63317  0.63317  0.92868  1.0000
+  O   O9        1.0  0.92868  0.80498  0.63317  1.0000
+  O   O10       1.0  0.80498  0.92868  0.63317  1.0000
+  O   O11       1.0  0.63317  0.92868  0.63317  1.0000
+  O   O12       1.0  0.63317  0.80498  0.63317  1.0000
+  O   O13       1.0  0.92868  0.63317  0.80498  1.0000
+  O   O14       1.0  0.80498  0.63317  0.92869  1.0000
+  O   O15       1.0  0.36683  0.19502  0.07131  1.0000
+  O   O16       1.0  0.36683  0.07131  0.19502  1.0000
+  O   O17       1.0  0.19502  0.36683  0.36683  1.0000
+  O   O18       1.0  0.07132  0.36683  0.36683  1.0000
+  O   O19       1.0  0.07132  0.36683  0.19502  1.0000
+  O   O20       1.0  0.19502  0.36683  0.07132  1.0000
+  O   O21       1.0  0.36683  0.19502  0.36683  1.0000
+  O   O22       1.0  0.36683  0.07132  0.36683  1.0000
+  O   O23       1.0  0.19502  0.07131  0.36683  1.0000
+  O   O24       1.0  0.07132  0.19502  0.36683  1.0000
+  O   O25       1.0  0.36683  0.36683  0.19502  1.0000
+  O   O26       1.0  0.36683  0.36683  0.07132  1.0000
```

### Comparing `moftransformer-2.0.0/moftransformer/examples/raw/acs+N270+E33.cif` & `moftransformer-2.0.1/moftransformer/examples/raw/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif` & `moftransformer-2.0.1/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/raw/fee+N254+E185.cif` & `moftransformer-2.0.1/moftransformer/examples/raw/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/raw/mok+N109+E146.cif` & `moftransformer-2.0.1/moftransformer/examples/raw/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif` & `moftransformer-2.0.1/moftransformer/examples/raw/smm+N577+E166.cif`

 * *Files 14% similar despite different names*

```diff
@@ -1,578 +1,476 @@
 # generated using pymatgen
-data_NaCdH50C71O15
+data_Zn4H9C21N3O13
 _symmetry_space_group_name_H-M   'P 1'
-_cell_length_a   25.67190000
-_cell_length_b   36.74890000
-_cell_length_c   37.72950000
-_cell_angle_alpha   88.51300000
-_cell_angle_beta   89.79300000
-_cell_angle_gamma   85.69100000
+_cell_length_a   12.45673333
+_cell_length_b   41.24760000
+_cell_length_c   41.48976758
+_cell_angle_alpha   60.57624191
+_cell_angle_beta   88.41892283
+_cell_angle_gamma   89.20800000
 _symmetry_Int_Tables_number   1
-_chemical_formula_structural   NaCdH50C71O15
-_chemical_formula_sum   'Na4 Cd4 H200 C284 O60'
-_cell_volume   35481.92585124
-_cell_formula_units_Z   4
+_chemical_formula_structural   Zn4H9C21N3O13
+_chemical_formula_sum   'Zn36 H81 C189 N27 O117'
+_cell_volume   18561.01358109
+_cell_formula_units_Z   9
 loop_
  _symmetry_equiv_pos_site_id
  _symmetry_equiv_pos_as_xyz
   1  'x, y, z'
 loop_
  _atom_site_type_symbol
  _atom_site_label
  _atom_site_symmetry_multiplicity
  _atom_site_fract_x
  _atom_site_fract_y
  _atom_site_fract_z
  _atom_site_occupancy
-  Na  Na0  1  0.96708000  0.10660000  0.05596000  1.0
-  Na  Na1  1  0.94273000  0.87919000  0.96008000  1.0
-  Na  Na2  1  0.48234000  0.60248000  0.44114000  1.0
-  Na  Na3  1  0.45618000  0.39005000  0.57242000  1.0
-  Cd  Cd4  1  0.98858000  0.01984000  0.01381000  1.0
-  Cd  Cd5  1  0.91938000  0.97002000  0.98470000  1.0
-  Cd  Cd6  1  0.50775000  0.51996000  0.48299000  1.0
-  Cd  Cd7  1  0.43785000  0.47072000  0.51546000  1.0
-  H  H8  1  0.05505000  0.78976000  0.36452000  1.0
-  H  H9  1  0.95180000  0.75063000  0.41890000  1.0
-  H  H10  1  0.92066000  0.77622000  0.34222000  1.0
-  H  H11  1  0.04058000  0.72093000  0.32509000  1.0
-  H  H12  1  0.03701000  0.20900000  0.62705000  1.0
-  H  H13  1  0.91681000  0.24289000  0.58061000  1.0
-  H  H14  1  0.89074000  0.20977000  0.64972000  1.0
-  H  H15  1  0.99841000  0.26526000  0.67723000  1.0
-  H  H16  1  0.39572000  0.27124000  0.11682000  1.0
-  H  H17  1  0.51345000  0.24389000  0.09459000  1.0
-  H  H18  1  0.53678000  0.26449000  0.16845000  1.0
-  H  H19  1  0.42420000  0.21514000  0.18717000  1.0
-  H  H20  1  0.37853000  0.71960000  0.89264000  1.0
-  H  H21  1  0.48217000  0.74773000  0.90748000  1.0
-  H  H22  1  0.50913000  0.71925000  0.83353000  1.0
-  H  H23  1  0.38885000  0.77585000  0.81520000  1.0
-  H  H24  1  0.70727000  0.91674000  0.88177000  1.0
-  H  H25  1  0.75549000  0.96837000  0.87518000  1.0
-  H  H26  1  0.80845000  0.97696000  0.90601000  1.0
-  H  H27  1  0.73577000  0.83920000  0.96854000  1.0
-  H  H28  1  0.80018000  0.84443000  0.01012000  1.0
-  H  H29  1  0.84219000  0.88289000  0.00869000  1.0
-  H  H30  1  0.67512000  0.81115000  0.95303000  1.0
-  H  H31  1  0.62902000  0.75912000  0.96080000  1.0
-  H  H32  1  0.57852000  0.74839000  0.92899000  1.0
-  H  H33  1  0.64802000  0.88619000  0.86346000  1.0
-  H  H34  1  0.58148000  0.87742000  0.82137000  1.0
-  H  H35  1  0.54204000  0.83754000  0.82513000  1.0
-  H  H36  1  0.75134000  0.05752000  0.11083000  1.0
-  H  H37  1  0.80717000  0.00320000  0.11342000  1.0
-  H  H38  1  0.86174000  0.99560000  0.08198000  1.0
-  H  H39  1  0.75991000  0.13280000  0.02194000  1.0
-  H  H40  1  0.83526000  0.13698000  0.98975000  1.0
-  H  H41  1  0.89524000  0.10970000  0.00428000  1.0
-  H  H42  1  0.71027000  0.16965000  0.04546000  1.0
-  H  H43  1  0.65948000  0.22459000  0.03963000  1.0
-  H  H44  1  0.60916000  0.23767000  0.07270000  1.0
-  H  H45  1  0.68921000  0.09145000  0.13133000  1.0
-  H  H46  1  0.62488000  0.10426000  0.17606000  1.0
-  H  H47  1  0.58254000  0.14714000  0.17441000  1.0
-  H  H48  1  0.64415000  0.34343000  0.52717000  1.0
-  H  H49  1  0.55885000  0.33964000  0.51066000  1.0
-  H  H50  1  0.51064000  0.37898000  0.51269000  1.0
-  H  H51  1  0.69322000  0.43333000  0.58665000  1.0
-  H  H52  1  0.64714000  0.49124000  0.58163000  1.0
-  H  H53  1  0.58463000  0.49769000  0.55788000  1.0
-  H  H54  1  0.75452000  0.39900000  0.60787000  1.0
-  H  H55  1  0.82948000  0.39006000  0.64477000  1.0
-  H  H56  1  0.86539000  0.34485000  0.64958000  1.0
-  H  H57  1  0.69693000  0.30869000  0.55199000  1.0
-  H  H58  1  0.73920000  0.25072000  0.55341000  1.0
-  H  H59  1  0.79746000  0.23994000  0.58112000  1.0
-  H  H60  1  0.73973000  0.57371000  0.40023000  1.0
-  H  H61  1  0.70394000  0.51697000  0.39876000  1.0
-  H  H62  1  0.64307000  0.50844000  0.42267000  1.0
-  H  H63  1  0.67303000  0.66010000  0.46549000  1.0
-  H  H64  1  0.59546000  0.65542000  0.49637000  1.0
-  H  H65  1  0.55762000  0.61506000  0.49210000  1.0
-  H  H66  1  0.73042000  0.69236000  0.45023000  1.0
-  H  H67  1  0.76681000  0.74852000  0.45402000  1.0
-  H  H68  1  0.82630000  0.75798000  0.42928000  1.0
-  H  H69  1  0.79892000  0.60578000  0.38518000  1.0
-  H  H70  1  0.87529000  0.61312000  0.35168000  1.0
-  H  H71  1  0.90711000  0.65632000  0.35122000  1.0
-  H  H72  1  0.22653000  0.06657000  0.09223000  1.0
-  H  H73  1  0.19243000  0.01025000  0.08950000  1.0
-  H  H74  1  0.12727000  0.00477000  0.07149000  1.0
-  H  H75  1  0.14160000  0.16563000  0.05536000  1.0
-  H  H76  1  0.06603000  0.16593000  0.02288000  1.0
-  H  H77  1  0.03795000  0.12386000  0.01005000  1.0
-  H  H78  1  0.20252000  0.19533000  0.06925000  1.0
-  H  H79  1  0.23638000  0.25263000  0.07511000  1.0
-  H  H80  1  0.29780000  0.25706000  0.09923000  1.0
-  H  H81  1  0.28640000  0.09623000  0.10893000  1.0
-  H  H82  1  0.36408000  0.09737000  0.14130000  1.0
-  H  H83  1  0.38947000  0.14046000  0.15407000  1.0
-  H  H84  1  0.18252000  0.88739000  0.98658000  1.0
-  H  H85  1  0.14289000  0.91797000  0.03587000  1.0
-  H  H86  1  0.07734000  0.94190000  0.03226000  1.0
-  H  H87  1  0.10930000  0.89787000  0.88373000  1.0
-  H  H88  1  0.02280000  0.91746000  0.87620000  1.0
-  H  H89  1  0.98195000  0.93401000  0.91366000  1.0
-  H  H90  1  0.16651000  0.86478000  0.86279000  1.0
-  H  H91  1  0.19911000  0.83624000  0.81266000  1.0
-  H  H92  1  0.26046000  0.80699000  0.81389000  1.0
-  H  H93  1  0.24348000  0.85299000  0.96466000  1.0
-  H  H94  1  0.32347000  0.81635000  0.97140000  1.0
-  H  H95  1  0.35314000  0.79086000  0.93406000  1.0
-  H  H96  1  0.27656000  0.63690000  0.49616000  1.0
-  H  H97  1  0.33416000  0.62058000  0.54384000  1.0
-  H  H98  1  0.38651000  0.58374000  0.53948000  1.0
-  H  H99  1  0.27990000  0.57247000  0.40186000  1.0
-  H  H100  1  0.35359000  0.53523000  0.38744000  1.0
-  H  H101  1  0.41242000  0.53989000  0.41551000  1.0
-  H  H102  1  0.22637000  0.60802000  0.37813000  1.0
-  H  H103  1  0.17423000  0.62394000  0.32859000  1.0
-  H  H104  1  0.12755000  0.66451000  0.32867000  1.0
-  H  H105  1  0.21407000  0.66915000  0.47490000  1.0
-  H  H106  1  0.15171000  0.71933000  0.48034000  1.0
-  H  H107  1  0.10883000  0.73485000  0.44283000  1.0
-  H  H108  1  0.19959000  0.41830000  0.58709000  1.0
-  H  H109  1  0.23359000  0.47498000  0.58746000  1.0
-  H  H110  1  0.29875000  0.48202000  0.56905000  1.0
-  H  H111  1  0.28403000  0.32348000  0.54380000  1.0
-  H  H112  1  0.36374000  0.32782000  0.51394000  1.0
-  H  H113  1  0.39428000  0.37144000  0.50913000  1.0
-  H  H114  1  0.22242000  0.29214000  0.55746000  1.0
-  H  H115  1  0.18604000  0.23479000  0.56091000  1.0
-  H  H116  1  0.12479000  0.22892000  0.58546000  1.0
-  H  H117  1  0.13873000  0.38809000  0.59922000  1.0
-  H  H118  1  0.06285000  0.38551000  0.63225000  1.0
-  H  H119  1  0.03668000  0.34206000  0.64488000  1.0
-  H  H120  1  0.93597000  0.85277000  0.44878000  1.0
-  H  H121  1  0.92669000  0.90891000  0.48289000  1.0
-  H  H122  1  0.07730000  0.93745000  0.44335000  1.0
-  H  H123  1  0.08284000  0.88412000  0.40646000  1.0
-  H  H124  1  0.96814000  0.99473000  0.56883000  1.0
-  H  H125  1  0.02340000  0.99130000  0.44346000  1.0
-  H  H126  1  0.02705000  0.03463000  0.59384000  1.0
-  H  H127  1  0.02264000  0.09202000  0.62516000  1.0
-  H  H128  1  0.95691000  0.14854000  0.53203000  1.0
-  H  H129  1  0.95779000  0.09084000  0.50148000  1.0
-  H  H130  1  0.01659000  0.06871000  0.45386000  1.0
-  H  H131  1  0.06199000  0.07225000  0.49039000  1.0
-  H  H132  1  0.13946000  0.05156000  0.41070000  1.0
-  H  H133  1  0.11982000  0.08837000  0.43918000  1.0
-  H  H134  1  0.07484000  0.07273000  0.40614000  1.0
-  H  H135  1  0.93254000  0.92547000  0.54949000  1.0
-  H  H136  1  0.99281000  0.90076000  0.53543000  1.0
-  H  H137  1  0.99623000  0.90723000  0.63243000  1.0
-  H  H138  1  0.98879000  0.87501000  0.59833000  1.0
-  H  H139  1  0.93542000  0.90885000  0.60950000  1.0
-  H  H140  1  0.50298000  0.62022000  0.91312000  1.0
-  H  H141  1  0.51378000  0.56942000  0.95667000  1.0
-  H  H142  1  0.34886000  0.58284000  0.98063000  1.0
-  H  H143  1  0.33752000  0.63111000  0.93495000  1.0
-  H  H144  1  0.50135000  0.48638000  0.05726000  1.0
-  H  H145  1  0.37130000  0.51833000  0.96308000  1.0
-  H  H146  1  0.44902000  0.45729000  0.10127000  1.0
-  H  H147  1  0.44743000  0.39954000  0.13442000  1.0
-  H  H148  1  0.42144000  0.34370000  0.03763000  1.0
-  H  H149  1  0.42766000  0.40126000  0.00364000  1.0
-  H  H150  1  0.35595000  0.43986000  0.97711000  1.0
-  H  H151  1  0.33832000  0.44222000  0.02385000  1.0
-  H  H152  1  0.22638000  0.48279000  0.97470000  1.0
-  H  H153  1  0.24923000  0.44258000  0.99953000  1.0
-  H  H154  1  0.27099000  0.45033000  0.95379000  1.0
-  H  H155  1  0.54864000  0.54562000  0.02127000  1.0
-  H  H156  1  0.49854000  0.58307000  0.02408000  1.0
-  H  H157  1  0.55530000  0.56921000  0.11220000  1.0
-  H  H158  1  0.55125000  0.60064000  0.07502000  1.0
-  H  H159  1  0.59247000  0.55771000  0.07343000  1.0
-  H  H160  1  0.93324000  0.85297000  0.12675000  1.0
-  H  H161  1  0.90965000  0.85607000  0.06892000  1.0
-  H  H162  1  0.91788000  0.89569000  0.04031000  1.0
-  H  H163  1  0.99713000  0.94101000  0.18104000  1.0
-  H  H164  1  0.00969000  0.99647000  0.15358000  1.0
-  H  H165  1  0.98988000  0.00739000  0.10780000  1.0
-  H  H166  1  0.00791000  0.90782000  0.22565000  1.0
-  H  H167  1  0.02852000  0.90123000  0.28659000  1.0
-  H  H168  1  0.01499000  0.85947000  0.31195000  1.0
-  H  H169  1  0.94925000  0.81860000  0.16873000  1.0
-  H  H170  1  0.92885000  0.76412000  0.19801000  1.0
-  H  H171  1  0.93881000  0.75798000  0.24640000  1.0
-  H  H172  1  0.97416000  0.04827000  0.81332000  1.0
-  H  H173  1  0.00168000  0.99129000  0.84071000  1.0
-  H  H174  1  0.00721000  0.98900000  0.88970000  1.0
-  H  H175  1  0.92226000  0.14062000  0.87665000  1.0
-  H  H176  1  0.89625000  0.13223000  0.93528000  1.0
-  H  H177  1  0.90027000  0.08486000  0.95421000  1.0
-  H  H178  1  0.92303000  0.17422000  0.83350000  1.0
-  H  H179  1  0.89833000  0.23135000  0.80747000  1.0
-  H  H180  1  0.90486000  0.23918000  0.75910000  1.0
-  H  H181  1  0.98839000  0.08408000  0.77208000  1.0
-  H  H182  1  0.00214000  0.09009000  0.71111000  1.0
-  H  H183  1  0.98442000  0.13289000  0.68662000  1.0
-  H  H184  1  0.50647000  0.34217000  0.38589000  1.0
-  H  H185  1  0.54051000  0.35208000  0.44220000  1.0
-  H  H186  1  0.54129000  0.39968000  0.45771000  1.0
-  H  H187  1  0.45399000  0.43368000  0.31787000  1.0
-  H  H188  1  0.43075000  0.49081000  0.34060000  1.0
-  H  H189  1  0.43518000  0.49552000  0.38884000  1.0
-  H  H190  1  0.43462000  0.39856000  0.27940000  1.0
-  H  H191  1  0.41939000  0.39287000  0.21826000  1.0
-  H  H192  1  0.43880000  0.35022000  0.19569000  1.0
-  H  H193  1  0.50703000  0.30914000  0.34297000  1.0
-  H  H194  1  0.53223000  0.25247000  0.31824000  1.0
-  H  H195  1  0.52428000  0.24533000  0.27024000  1.0
-  H  H196  1  0.43287000  0.55625000  0.67910000  1.0
-  H  H197  1  0.42146000  0.49919000  0.65678000  1.0
-  H  H198  1  0.43871000  0.48723000  0.61120000  1.0
-  H  H199  1  0.48960000  0.64333000  0.61501000  1.0
-  H  H200  1  0.51176000  0.63793000  0.55714000  1.0
-  H  H201  1  0.50316000  0.59693000  0.53268000  1.0
-  H  H202  1  0.47784000  0.67876000  0.65513000  1.0
-  H  H203  1  0.49638000  0.73495000  0.67856000  1.0
-  H  H204  1  0.48726000  0.74353000  0.72631000  1.0
-  H  H205  1  0.42321000  0.59149000  0.72109000  1.0
-  H  H206  1  0.40468000  0.59979000  0.78149000  1.0
-  H  H207  1  0.41688000  0.64245000  0.80312000  1.0
-  C  C208  1  0.95614000  0.03050000  0.93546000  1.0
-  C  C209  1  0.06590000  0.05569000  0.03480000  1.0
-  C  C210  1  0.89727000  0.04361000  0.03519000  1.0
-  C  C211  1  0.95635000  0.95917000  0.06079000  1.0
-  C  C212  1  0.84190000  0.93671000  0.96124000  1.0
-  C  C213  1  0.01240000  0.94229000  0.97975000  1.0
-  C  C214  1  0.47766000  0.45476000  0.43887000  1.0
-  C  C215  1  0.58495000  0.55386000  0.46015000  1.0
-  C  C216  1  0.41562000  0.54938000  0.48208000  1.0
-  C  C217  1  0.46946000  0.53312000  0.55910000  1.0
-  C  C218  1  0.36053000  0.43473000  0.53485000  1.0
-  C  C219  1  0.52825000  0.44516000  0.53412000  1.0
-  C  C220  1  0.02628000  0.82594000  0.41912000  1.0
-  C  C221  1  0.02154000  0.78166000  0.37993000  1.0
-  C  C222  1  0.95678000  0.73705000  0.39363000  1.0
-  C  C223  1  0.87319000  0.71675000  0.38238000  1.0
-  C  C224  1  0.94950000  0.81218000  0.28982000  1.0
-  C  C225  1  0.96074000  0.76946000  0.33455000  1.0
-  C  C226  1  0.02969000  0.72180000  0.35293000  1.0
-  C  C227  1  0.11393000  0.71074000  0.37820000  1.0
-  C  C228  1  0.99192000  0.75190000  0.36514000  1.0
-  C  C229  1  0.01488000  0.15764000  0.58971000  1.0
-  C  C230  1  0.99692000  0.20925000  0.61780000  1.0
-  C  C231  1  0.92325000  0.25627000  0.60541000  1.0
-  C  C232  1  0.84098000  0.28427000  0.62225000  1.0
-  C  C233  1  0.91863000  0.18692000  0.71268000  1.0
-  C  C234  1  0.92661000  0.21880000  0.66061000  1.0
-  C  C235  1  0.99096000  0.26601000  0.64888000  1.0
-  C  C236  1  0.07812000  0.27651000  0.62972000  1.0
-  C  C237  1  0.95873000  0.23768000  0.63331000  1.0
-  C  C238  1  0.41921000  0.33655000  0.11077000  1.0
-  C  C239  1  0.43404000  0.27649000  0.12697000  1.0
-  C  C240  1  0.50446000  0.22830000  0.11854000  1.0
-  C  C241  1  0.58986000  0.20236000  0.13044000  1.0
-  C  C242  1  0.50491000  0.29804000  0.22212000  1.0
-  C  C243  1  0.49668000  0.26032000  0.17541000  1.0
-  C  C244  1  0.43176000  0.21747000  0.15886000  1.0
-  C  C245  1  0.34603000  0.20665000  0.14066000  1.0
-  C  C246  1  0.46681000  0.24559000  0.14514000  1.0
-  C  C247  1  0.41118000  0.65265000  0.88859000  1.0
-  C  C248  1  0.41288000  0.71286000  0.87636000  1.0
-  C  C249  1  0.47372000  0.76087000  0.88168000  1.0
-  C  C250  1  0.55686000  0.78169000  0.86923000  1.0
-  C  C251  1  0.47918000  0.69246000  0.77579000  1.0
-  C  C252  1  0.46896000  0.72680000  0.82579000  1.0
-  C  C253  1  0.39669000  0.77202000  0.84343000  1.0
-  C  C254  1  0.31373000  0.78570000  0.86985000  1.0
-  C  C255  1  0.43778000  0.74340000  0.85643000  1.0
-  C  C256  1  0.76785000  0.92778000  0.91786000  1.0
-  C  C257  1  0.72753000  0.90697000  0.90558000  1.0
-  C  C258  1  0.77807000  0.95971000  0.89864000  1.0
-  C  C259  1  0.78465000  0.88310000  0.96614000  1.0
-  C  C260  1  0.74358000  0.86350000  0.95360000  1.0
-  C  C261  1  0.81092000  0.86942000  0.99679000  1.0
-  C  C262  1  0.61821000  0.79802000  0.91637000  1.0
-  C  C263  1  0.65639000  0.82009000  0.92858000  1.0
-  C  C264  1  0.60795000  0.76648000  0.93644000  1.0
-  C  C265  1  0.60128000  0.84067000  0.86633000  1.0
-  C  C266  1  0.64071000  0.86195000  0.87885000  1.0
-  C  C267  1  0.57339000  0.85238000  0.83558000  1.0
-  C  C268  1  0.79758000  0.91582000  0.94836000  1.0
-  C  C269  1  0.71394000  0.87453000  0.92312000  1.0
-  C  C270  1  0.59109000  0.80788000  0.88461000  1.0
-  C  C271  1  0.66995000  0.85208000  0.90995000  1.0
-  C  C272  1  0.81472000  0.04709000  0.07453000  1.0
-  C  C273  1  0.77003000  0.06770000  0.08726000  1.0
-  C  C274  1  0.82939000  0.01329000  0.09110000  1.0
-  C  C275  1  0.82428000  0.09442000  0.02934000  1.0
-  C  C276  1  0.77525000  0.11035000  0.03851000  1.0
-  C  C277  1  0.85330000  0.11407000  0.00540000  1.0
-  C  C278  1  0.65215000  0.18437000  0.08257000  1.0
-  C  C279  1  0.69123000  0.16010000  0.06889000  1.0
-  C  C280  1  0.63954000  0.21766000  0.06406000  1.0
-  C  C281  1  0.63963000  0.14076000  0.13135000  1.0
-  C  C282  1  0.67932000  0.11682000  0.11695000  1.0
-  C  C283  1  0.61421000  0.13024000  0.16266000  1.0
-  C  C284  1  0.84445000  0.06130000  0.04609000  1.0
-  C  C285  1  0.75006000  0.10045000  0.07013000  1.0
-  C  C286  1  0.62656000  0.17489000  0.11430000  1.0
-  C  C287  1  0.70581000  0.12561000  0.08535000  1.0
-  C  C288  1  0.58861000  0.38809000  0.53252000  1.0
-  C  C289  1  0.63730000  0.36952000  0.53912000  1.0
-  C  C290  1  0.55010000  0.36781000  0.51817000  1.0
-  C  C291  1  0.62045000  0.44202000  0.55910000  1.0
-  C  C292  1  0.66548000  0.42043000  0.57069000  1.0
-  C  C293  1  0.61668000  0.47920000  0.56697000  1.0
-  C  C294  1  0.79731000  0.34734000  0.61456000  1.0
-  C  C295  1  0.75670000  0.37093000  0.59997000  1.0
-  C  C296  1  0.83290000  0.36152000  0.63777000  1.0
-  C  C297  1  0.76443000  0.29681000  0.58247000  1.0
-  C  C298  1  0.72443000  0.32079000  0.56860000  1.0
-  C  C299  1  0.76718000  0.26018000  0.57198000  1.0
-  C  C300  1  0.57994000  0.42534000  0.54140000  1.0
-  C  C301  1  0.67431000  0.38339000  0.56163000  1.0
-  C  C302  1  0.80080000  0.31001000  0.60597000  1.0
-  C  C303  1  0.71946000  0.35847000  0.57640000  1.0
-  C  C304  1  0.66999000  0.56311000  0.42805000  1.0
-  C  C305  1  0.71044000  0.58532000  0.41798000  1.0
-  C  C306  1  0.67209000  0.52735000  0.41563000  1.0
-  C  C307  1  0.63078000  0.61287000  0.46302000  1.0
-  C  C308  1  0.67301000  0.63365000  0.45388000  1.0
-  C  C309  1  0.59223000  0.62856000  0.48544000  1.0
-  C  C310  1  0.79772000  0.70385000  0.42117000  1.0
-  C  C311  1  0.75897000  0.68095000  0.43190000  1.0
-  C  C312  1  0.79691000  0.73900000  0.43544000  1.0
-  C  C313  1  0.83712000  0.65500000  0.38472000  1.0
-  C  C314  1  0.79746000  0.63273000  0.39584000  1.0
-  C  C315  1  0.87551000  0.64080000  0.36106000  1.0
-  C  C316  1  0.62856000  0.57710000  0.45002000  1.0
-  C  C317  1  0.71320000  0.62108000  0.43054000  1.0
-  C  C318  1  0.83656000  0.69110000  0.39686000  1.0
-  C  C319  1  0.75704000  0.64506000  0.41937000  1.0
-  C  C320  1  0.15329000  0.06024000  0.06741000  1.0
-  C  C321  1  0.19382000  0.08119000  0.07904000  1.0
-  C  C322  1  0.15789000  0.02271000  0.07599000  1.0
-  C  C323  1  0.10690000  0.11631000  0.04448000  1.0
-  C  C324  1  0.14663000  0.13636000  0.05850000  1.0
-  C  C325  1  0.06719000  0.13629000  0.02515000  1.0
-  C  C326  1  0.27114000  0.20176000  0.09870000  1.0
-  C  C327  1  0.23325000  0.18064000  0.08428000  1.0
-  C  C328  1  0.26796000  0.23958000  0.09111000  1.0
-  C  C329  1  0.31788000  0.14590000  0.12190000  1.0
-  C  C330  1  0.28011000  0.12546000  0.10628000  1.0
-  C  C331  1  0.35971000  0.12699000  0.14024000  1.0
-  C  C332  1  0.10912000  0.07745000  0.04896000  1.0
-  C  C333  1  0.19179000  0.11961000  0.07506000  1.0
-  C  C334  1  0.31208000  0.18450000  0.11956000  1.0
-  C  C335  1  0.23540000  0.14210000  0.08872000  1.0
-  C  C336  1  0.10636000  0.91553000  0.98416000  1.0
-  C  C337  1  0.15016000  0.89556000  0.96922000  1.0
-  C  C338  1  0.10860000  0.92547000  0.01971000  1.0
-  C  C339  1  0.06291000  0.91633000  0.92683000  1.0
-  C  C340  1  0.10913000  0.90027000  0.91208000  1.0
-  C  C341  1  0.01948000  0.92256000  0.90449000  1.0
-  C  C342  1  0.23545000  0.83032000  0.86481000  1.0
-  C  C343  1  0.19705000  0.85399000  0.88034000  1.0
-  C  C344  1  0.23151000  0.82379000  0.82829000  1.0
-  C  C345  1  0.28016000  0.82356000  0.92191000  1.0
-  C  C346  1  0.24046000  0.84740000  0.93683000  1.0
-  C  C347  1  0.32141000  0.80919000  0.94368000  1.0
-  C  C348  1  0.06109000  0.92491000  0.96325000  1.0
-  C  C349  1  0.15230000  0.88684000  0.93284000  1.0
-  C  C350  1  0.27691000  0.81408000  0.88570000  1.0
-  C  C351  1  0.19752000  0.86292000  0.91655000  1.0
-  C  C352  1  0.33773000  0.59459000  0.49272000  1.0
-  C  C353  1  0.29336000  0.61569000  0.47950000  1.0
-  C  C354  1  0.35440000  0.60025000  0.52735000  1.0
-  C  C355  1  0.34254000  0.56227000  0.43753000  1.0
-  C  C356  1  0.29503000  0.58014000  0.42693000  1.0
-  C  C357  1  0.37064000  0.54243000  0.41245000  1.0
-  C  C358  1  0.17239000  0.65390000  0.37779000  1.0
-  C  C359  1  0.21046000  0.62990000  0.39418000  1.0
-  C  C360  1  0.15722000  0.64726000  0.34283000  1.0
-  C  C361  1  0.16464000  0.68844000  0.43229000  1.0
-  C  C362  1  0.20346000  0.66419000  0.44795000  1.0
-  C  C363  1  0.14054000  0.71626000  0.45287000  1.0
-  C  C364  1  0.36431000  0.56841000  0.47093000  1.0
-  C  C365  1  0.27165000  0.60957000  0.44585000  1.0
-  C  C366  1  0.15035000  0.68394000  0.39660000  1.0
-  C  C367  1  0.22767000  0.63455000  0.42939000  1.0
-  C  C368  1  0.27278000  0.42697000  0.56378000  1.0
-  C  C369  1  0.23215000  0.40493000  0.57337000  1.0
-  C  C370  1  0.26816000  0.46369000  0.57367000  1.0
-  C  C371  1  0.32026000  0.37372000  0.53844000  1.0
-  C  C372  1  0.27940000  0.35220000  0.54933000  1.0
-  C  C373  1  0.36235000  0.35673000  0.51965000  1.0
-  C  C374  1  0.15298000  0.28366000  0.58673000  1.0
-  C  C375  1  0.19154000  0.30559000  0.57287000  1.0
-  C  C376  1  0.15511000  0.24665000  0.57778000  1.0
-  C  C377  1  0.10729000  0.33793000  0.61151000  1.0
-  C  C378  1  0.14509000  0.35914000  0.59612000  1.0
-  C  C379  1  0.06633000  0.35598000  0.63066000  1.0
-  C  C380  1  0.31732000  0.41163000  0.54569000  1.0
-  C  C381  1  0.23398000  0.36715000  0.56655000  1.0
-  C  C382  1  0.11237000  0.29957000  0.60836000  1.0
-  C  C383  1  0.18987000  0.34366000  0.57850000  1.0
-  C  C384  1  0.01182000  0.86372000  0.42725000  1.0
-  C  C385  1  0.96604000  0.87196000  0.44680000  1.0
-  C  C386  1  0.96127000  0.90338000  0.46679000  1.0
-  C  C387  1  0.00247000  0.92638000  0.46715000  1.0
-  C  C388  1  0.04550000  0.91966000  0.44436000  1.0
-  C  C389  1  0.04916000  0.88912000  0.42359000  1.0
-  C  C390  1  0.99993000  0.95930000  0.48871000  1.0
-  C  C391  1  0.98693000  0.95964000  0.52535000  1.0
-  C  C392  1  0.98337000  0.99323000  0.54199000  1.0
-  C  C393  1  0.00021000  0.02479000  0.52514000  1.0
-  C  C394  1  0.02001000  0.02300000  0.49007000  1.0
-  C  C395  1  0.01428000  0.99132000  0.47156000  1.0
-  C  C396  1  0.99468000  0.05887000  0.54478000  1.0
-  C  C397  1  0.01015000  0.05915000  0.58046000  1.0
-  C  C398  1  0.00725000  0.09183000  0.59843000  1.0
-  C  C399  1  0.99092000  0.12451000  0.58039000  1.0
-  C  C400  1  0.96948000  0.12355000  0.54639000  1.0
-  C  C401  1  0.97157000  0.09080000  0.52855000  1.0
-  C  C402  1  0.04655000  0.05357000  0.47101000  1.0
-  C  C403  1  0.10593000  0.06435000  0.42578000  1.0
-  C  C404  1  0.97584000  0.92609000  0.54773000  1.0
-  C  C405  1  0.97836000  0.90359000  0.60611000  1.0
-  C  C406  1  0.41921000  0.62875000  0.92034000  1.0
-  C  C407  1  0.46932000  0.61252000  0.92821000  1.0
-  C  C408  1  0.47559000  0.58379000  0.95330000  1.0
-  C  C409  1  0.43206000  0.57216000  0.97193000  1.0
-  C  C410  1  0.38294000  0.59105000  0.96633000  1.0
-  C  C411  1  0.37635000  0.61861000  0.94029000  1.0
-  C  C412  1  0.43501000  0.53725000  0.99289000  1.0
-  C  C413  1  0.47119000  0.52863000  0.02071000  1.0
-  C  C414  1  0.47160000  0.49405000  0.03756000  1.0
-  C  C415  1  0.43356000  0.46963000  0.03030000  1.0
-  C  C416  1  0.39390000  0.48015000  0.00523000  1.0
-  C  C417  1  0.39829000  0.51220000  0.98487000  1.0
-  C  C418  1  0.43596000  0.43401000  0.04997000  1.0
-  C  C419  1  0.44374000  0.43272000  0.08687000  1.0
-  C  C420  1  0.44243000  0.39992000  0.10588000  1.0
-  C  C421  1  0.43199000  0.36803000  0.08869000  1.0
-  C  C422  1  0.42828000  0.36827000  0.05158000  1.0
-  C  C423  1  0.43101000  0.40124000  0.03222000  1.0
-  C  C424  1  0.34664000  0.45845000  0.99947000  1.0
-  C  C425  1  0.26083000  0.46319000  0.97950000  1.0
-  C  C426  1  0.51007000  0.55461000  0.03308000  1.0
-  C  C427  1  0.55487000  0.57118000  0.08279000  1.0
-  C  C428  1  0.94172000  0.90096000  0.09599000  1.0
-  C  C429  1  0.94673000  0.87991000  0.12752000  1.0
-  C  C430  1  0.92168000  0.88378000  0.06658000  1.0
-  C  C431  1  0.97842000  0.95120000  0.12658000  1.0
-  C  C432  1  0.98276000  0.92892000  0.15760000  1.0
-  C  C433  1  0.99372000  0.98708000  0.12904000  1.0
-  C  C434  1  0.99225000  0.86052000  0.25597000  1.0
-  C  C435  1  0.99294000  0.88128000  0.22422000  1.0
-  C  C436  1  0.01249000  0.87470000  0.28691000  1.0
-  C  C437  1  0.95658000  0.81111000  0.22408000  1.0
-  C  C438  1  0.95946000  0.83185000  0.19254000  1.0
-  C  C439  1  0.93993000  0.77560000  0.22290000  1.0
-  C  C440  1  0.95827000  0.93718000  0.09481000  1.0
-  C  C441  1  0.96836000  0.89261000  0.15867000  1.0
-  C  C442  1  0.96985000  0.82652000  0.25626000  1.0
-  C  C443  1  0.97376000  0.86841000  0.19210000  1.0
-  C  C444  1  0.96965000  0.03873000  0.86898000  1.0
-  C  C445  1  0.96508000  0.06110000  0.83820000  1.0
-  C  C446  1  0.99270000  0.00340000  0.86621000  1.0
-  C  C447  1  0.93427000  0.08977000  0.90321000  1.0
-  C  C448  1  0.93591000  0.11258000  0.87322000  1.0
-  C  C449  1  0.91014000  0.10369000  0.93342000  1.0
-  C  C450  1  0.92782000  0.18370000  0.77835000  1.0
-  C  C451  1  0.93380000  0.16147000  0.80896000  1.0
-  C  C452  1  0.90868000  0.22030000  0.78170000  1.0
-  C  C453  1  0.96562000  0.13310000  0.74347000  1.0
-  C  C454  1  0.97036000  0.11133000  0.77454000  1.0
-  C  C455  1  0.98453000  0.11790000  0.71166000  1.0
-  C  C456  1  0.95377000  0.05301000  0.90204000  1.0
-  C  C457  1  0.95148000  0.09908000  0.83992000  1.0
-  C  C458  1  0.94072000  0.16879000  0.74508000  1.0
-  C  C459  1  0.95177000  0.12416000  0.80750000  1.0
-  C  C460  1  0.49961000  0.39415000  0.40934000  1.0
-  C  C461  1  0.49431000  0.37051000  0.38103000  1.0
-  C  C462  1  0.52737000  0.38080000  0.43907000  1.0
-  C  C463  1  0.46370000  0.44441000  0.37229000  1.0
-  C  C464  1  0.46467000  0.42131000  0.34329000  1.0
-  C  C465  1  0.44321000  0.47982000  0.36650000  1.0
-  C  C466  1  0.45811000  0.35028000  0.25227000  1.0
-  C  C467  1  0.45383000  0.37158000  0.28266000  1.0
-  C  C468  1  0.43800000  0.36535000  0.22001000  1.0
-  C  C469  1  0.49928000  0.29989000  0.28817000  1.0
-  C  C470  1  0.49407000  0.32167000  0.31814000  1.0
-  C  C471  1  0.52037000  0.26368000  0.29231000  1.0
-  C  C472  1  0.48079000  0.43120000  0.40637000  1.0
-  C  C473  1  0.47697000  0.38350000  0.34718000  1.0
-  C  C474  1  0.48396000  0.31493000  0.25468000  1.0
-  C  C475  1  0.47461000  0.35864000  0.31580000  1.0
-  C  C476  1  0.44894000  0.54413000  0.62490000  1.0
-  C  C477  1  0.44544000  0.56764000  0.65416000  1.0
-  C  C478  1  0.43534000  0.50809000  0.63092000  1.0
-  C  C479  1  0.48208000  0.59369000  0.58897000  1.0
-  C  C480  1  0.47765000  0.61607000  0.61869000  1.0
-  C  C481  1  0.50033000  0.61000000  0.55769000  1.0
-  C  C482  1  0.47091000  0.68889000  0.70986000  1.0
-  C  C483  1  0.46822000  0.66654000  0.68031000  1.0
-  C  C484  1  0.48622000  0.72460000  0.70473000  1.0
-  C  C485  1  0.43804000  0.64040000  0.74701000  1.0
-  C  C486  1  0.43718000  0.61822000  0.71708000  1.0
-  C  C487  1  0.41952000  0.62667000  0.77937000  1.0
-  C  C488  1  0.46708000  0.55699000  0.59127000  1.0
-  C  C489  1  0.45864000  0.60430000  0.65172000  1.0
-  C  C490  1  0.45864000  0.67512000  0.74396000  1.0
-  C  C491  1  0.45461000  0.62986000  0.68332000  1.0
-  O  O492  1  0.07148000  0.02265000  0.02247000  1.0
-  O  O493  1  0.01677000  0.06672000  0.03407000  1.0
-  O  O494  1  0.90461000  0.01490000  0.01546000  1.0
-  O  O495  1  0.94005000  0.05833000  0.03977000  1.0
-  O  O496  1  0.98458000  0.04087000  0.96215000  1.0
-  O  O497  1  0.92563000  0.00323000  0.93958000  1.0
-  O  O498  1  0.83782000  0.97084000  0.97035000  1.0
-  O  O499  1  0.88980000  0.92335000  0.96521000  1.0
-  O  O500  1  0.99981000  0.97767000  0.97723000  1.0
-  O  O501  1  0.97059000  0.92457000  0.98348000  1.0
-  O  O502  1  0.91681000  0.95764000  0.03864000  1.0
-  O  O503  1  0.99473000  0.97961000  0.05250000  1.0
-  O  O504  1  0.59029000  0.52554000  0.48176000  1.0
-  O  O505  1  0.53644000  0.55989000  0.45052000  1.0
-  O  O506  1  0.42711000  0.51401000  0.47887000  1.0
-  O  O507  1  0.45798000  0.56680000  0.48114000  1.0
-  O  O508  1  0.50580000  0.48353000  0.44076000  1.0
-  O  O509  1  0.44775000  0.44562000  0.46600000  1.0
-  O  O510  1  0.35525000  0.46443000  0.51496000  1.0
-  O  O511  1  0.40891000  0.42742000  0.54344000  1.0
-  O  O512  1  0.52017000  0.47456000  0.51403000  1.0
-  O  O513  1  0.48435000  0.43341000  0.54472000  1.0
-  O  O514  1  0.43172000  0.51160000  0.55276000  1.0
-  O  O515  1  0.50806000  0.53513000  0.53596000  1.0
-  O  O516  1  0.06435000  0.81023000  0.43397000  1.0
-  O  O517  1  0.99281000  0.80768000  0.39897000  1.0
-  O  O518  1  0.92547000  0.71010000  0.38674000  1.0
-  O  O519  1  0.85523000  0.74437000  0.36673000  1.0
-  O  O520  1  0.90411000  0.82140000  0.29759000  1.0
-  O  O521  1  0.98401000  0.79609000  0.31463000  1.0
-  O  O522  1  0.06260000  0.70479000  0.37705000  1.0
-  O  O523  1  0.13084000  0.73720000  0.36295000  1.0
-  O  O524  1  0.06243000  0.15548000  0.59366000  1.0
-  O  O525  1  0.98777000  0.19159000  0.58677000  1.0
-  O  O526  1  0.89177000  0.28619000  0.61315000  1.0
-  O  O527  1  0.82758000  0.26116000  0.64357000  1.0
-  O  O528  1  0.87089000  0.18925000  0.70945000  1.0
-  O  O529  1  0.95175000  0.19466000  0.68474000  1.0
-  O  O530  1  0.02525000  0.28175000  0.62674000  1.0
-  O  O531  1  0.09807000  0.25302000  0.65006000  1.0
-  O  O532  1  0.37787000  0.33870000  0.12729000  1.0
-  O  O533  1  0.45717000  0.30809000  0.11677000  1.0
-  O  O534  1  0.53769000  0.19948000  0.12842000  1.0
-  O  O535  1  0.60733000  0.22860000  0.14422000  1.0
-  O  O536  1  0.55064000  0.30241000  0.21474000  1.0
-  O  O537  1  0.47075000  0.28529000  0.19753000  1.0
-  O  O538  1  0.39850000  0.20350000  0.13595000  1.0
-  O  O539  1  0.32604000  0.22844000  0.16166000  1.0
-  O  O540  1  0.37931000  0.64537000  0.86626000  1.0
-  O  O541  1  0.44342000  0.68059000  0.88268000  1.0
-  O  O542  1  0.50409000  0.78752000  0.87038000  1.0
-  O  O543  1  0.57718000  0.75382000  0.85655000  1.0
-  O  O544  1  0.52680000  0.69292000  0.77804000  1.0
-  O  O545  1  0.44632000  0.70230000  0.80413000  1.0
-  O  O546  1  0.36540000  0.79062000  0.86694000  1.0
-  O  O547  1  0.29639000  0.75812000  0.85855000  1.0
-  O  O548  1  0.99865000  0.92871000  0.58172000  1.0
-  O  O549  1  0.08909000  0.03829000  0.45067000  1.0
-  O  O550  1  0.51182000  0.55328000  0.07064000  1.0
-  O  O551  1  0.30218000  0.48271000  0.99193000  1.0
+  C  C0  1  0.66208000  0.18383000  0.99413000  1.0
+  C  C1  1  0.92735000  0.08846000  0.07141000  1.0
+  C  C2  1  0.08899000  0.21925000  0.04375000  1.0
+  C  C3  1  0.95140000  0.15293000  0.93662000  1.0
+  C  C4  1  0.90000000  0.27340000  0.95258000  1.0
+  C  C5  1  0.20669000  0.18617000  0.98308000  1.0
+  C  C6  1  0.31804000  0.02129000  0.82488000  1.0
+  C  C7  1  0.03287000  0.93683000  0.91181000  1.0
+  C  C8  1  0.88684000  0.97891000  0.77688000  1.0
+  C  C9  1  0.02871000  0.07450000  0.85606000  1.0
+  C  C10  1  0.09014000  0.06271000  0.73312000  1.0
+  C  C11  1  0.77484000  0.03339000  0.81922000  1.0
+  C  C12  1  0.68999000  0.84546000  0.15705000  1.0
+  C  C13  1  0.98276000  0.85868667  0.06636000  1.0
+  C  C14  1  0.13346000  0.76013000  0.19976000  1.0
+  C  C15  1  0.95036000  0.93137000  0.13692000  1.0
+  C  C16  1  0.92745000  0.79357000  0.24898000  1.0
+  C  C17  1  0.23372000  0.85552000  0.16157000  1.0
+  C  C18  1  0.03063000  0.85792000  0.64878000  1.0
+  C  C19  1  0.76910000  0.83280000  0.57856000  1.0
+  C  C20  1  0.60218000  0.94070000  0.60268000  1.0
+  C  C21  1  0.75598000  0.76980000  0.71957000  1.0
+  C  C22  1  0.77851000  0.90761000  0.69317000  1.0
+  C  C23  1  0.48527000  0.84862000  0.66053000  1.0
+  C  C24  1  0.04037000  0.66239000  0.50048000  1.0
+  C  C25  1  0.74589000  0.61203000  0.58912000  1.0
+  C  C26  1  0.62792000  0.62232000  0.45908000  1.0
+  C  C27  1  0.77905000  0.74856000  0.50427000  1.0
+  C  C28  1  0.79363000  0.71639333  0.40134667  1.0
+  C  C29  1  0.49509000  0.67692000  0.49571000  1.0
+  C  C30  1  0.00612000  0.51749000  0.83098000  1.0
+  C  C31  1  0.74730000  0.61330000  0.81218000  1.0
+  C  C32  1  0.56912000  0.48764000  0.91365000  1.0
+  C  C33  1  0.72387000  0.54406000  0.74667000  1.0
+  C  C34  1  0.77436000  0.42688000  0.87984000  1.0
+  C  C35  1  0.46368000  0.51542000  0.82312000  1.0
+  C  C36  1  0.03923000  0.51926000  0.32662000  1.0
+  C  C37  1  0.29941000  0.42428000  0.40620000  1.0
+  C  C38  1  0.47120000  0.55148000  0.37979000  1.0
+  C  C39  1  0.32799000  0.48255000  0.27497000  1.0
+  C  C40  1  0.27338000  0.60827000  0.28168000  1.0
+  C  C41  1  0.58350000  0.52149000  0.31585000  1.0
+  C  C42  1  0.63957000  0.35487000  0.15092000  1.0
+  C  C43  1  0.35630000  0.27279000  0.24348000  1.0
+  C  C44  1  0.21779000  0.30136000  0.11507000  1.0
+  C  C45  1  0.36133000  0.40482000  0.19182000  1.0
+  C  C46  1  0.40702000  0.40445000  0.06301000  1.0
+  C  C47  1  0.09494000  0.36782000  0.14532000  1.0
+  C  C48  1  0.02844000  0.17687000  0.49284000  1.0
+  C  C49  1  0.31483000  0.19730000  0.39973000  1.0
+  C  C50  1  0.46002000  0.09277000  0.53074000  1.0
+  C  C51  1  0.29845000  0.26683000  0.47126000  1.0
+  C  C52  1  0.25732000  0.13323000  0.58430000  1.0
+  C  C53  1  0.57274000  0.18594000  0.49826000  1.0
+  C  C54  1  0.12025000  0.23929000  0.06343000  1.0
+  C  C55  1  0.12997000  0.27826000  0.04399000  1.0
+  C  C56  1  0.18877000  0.27894000  0.09778000  1.0
+  C  C57  1  0.18085000  0.23998667  0.11828000  1.0
+  C  C58  1  0.14584000  0.22025000  0.10105000  1.0
+  C  C59  1  0.12473000  0.08304000  0.69387000  1.0
+  C  C60  1  0.13621000  0.06376667  0.67397000  1.0
+  C  C61  1  0.21641000  0.11647000  0.62269000  1.0
+  C  C62  1  0.20521000  0.13705000  0.64132000  1.0
+  C  C63  1  0.15876000  0.12023000  0.67696000  1.0
+  C  C64  1  0.16884000  0.72091000  0.21982000  1.0
+  C  C65  1  0.18299000  0.70317000  0.25819000  1.0
+  C  C66  1  0.24333000  0.64770000  0.25910000  1.0
+  C  C67  1  0.23163000  0.66445000  0.22067000  1.0
+  C  C68  1  0.19358000  0.70105000  0.20112000  1.0
+  C  C69  1  0.82076000  0.73661000  0.36152000  1.0
+  C  C70  1  0.83789000  0.77522000  0.34259000  1.0
+  C  C71  1  0.89620000  0.77341000  0.28837000  1.0
+  C  C72  1  0.87888000  0.73490000  0.30624000  1.0
+  C  C73  1  0.84161000  0.71661000  0.34277000  1.0
+  C  C74  1  0.80384000  0.38712000  0.89764000  1.0
+  C  C75  1  0.82049000  0.36708000  0.93586000  1.0
+  C  C76  1  0.87248000  0.31315000  0.93232000  1.0
+  C  C77  1  0.85779000  0.33217000  0.89396000  1.0
+  C  C78  1  0.82259000  0.36915000  0.87672000  1.0
+  C  C79  1  0.85896000  0.96097000  0.75497000  1.0
+  C  C80  1  0.83422000  0.92288000  0.77227000  1.0
+  C  C81  1  0.80088000  0.92692000  0.71414000  1.0
+  C  C82  1  0.82467000  0.96508333  0.69580667  1.0
+  C  C83  1  0.85295000  0.98204000  0.71631000  1.0
+  C  C84  1  0.43975000  0.42799000  0.02371000  1.0
+  C  C85  1  0.45924000  0.41140000  0.00160000  1.0
+  C  C86  1  0.52505000  0.46837000  0.95174000  1.0
+  C  C87  1  0.50464000  0.48649000  0.97239000  1.0
+  C  C88  1  0.46175000  0.46614667  0.00849000  1.0
+  C  C89  1  0.49421000  0.05339000  0.54830000  1.0
+  C  C90  1  0.50942000  0.03312000  0.58662000  1.0
+  C  C91  1  0.56857000  0.97997000  0.58272000  1.0
+  C  C92  1  0.55508000  0.99917000  0.54430000  1.0
+  C  C93  1  0.51723000  0.03586000  0.52719000  1.0
+  C  C94  1  0.59462000  0.60314000  0.43873000  1.0
+  C  C95  1  0.56818000  0.56511000  0.45684000  1.0
+  C  C96  1  0.51182000  0.56957000  0.40023000  1.0
+  C  C97  1  0.53913000  0.60742000  0.38114000  1.0
+  C  C98  1  0.58002000  0.62403000  0.40039000  1.0
+  C  C99  1  0.93866000  0.97070000  0.12707000  1.0
+  C  C100  1  0.85065000  0.99078000  0.10622000  1.0
+  C  C101  1  0.92580000  0.04784000  0.09609000  1.0
+  C  C102  1  0.01178000  0.02852667  0.11908000  1.0
+  C  C103  1  0.01760000  0.98968000  0.13480000  1.0
+  C  C104  1  0.00546000  0.09715000  0.87409000  1.0
+  C  C105  1  0.97389000  0.07877333  0.91156667  1.0
+  C  C106  1  0.96989000  0.13562000  0.91321000  1.0
+  C  C107  1  0.00022000  0.15550000  0.87553000  1.0
+  C  C108  1  0.01708000  0.13607000  0.85586000  1.0
+  C  C109  1  0.99524000  0.86913000  0.02718000  1.0
+  C  C110  1  0.09770000  0.87753667  0.01020000  1.0
+  C  C111  1  0.02119000  0.90755000  0.95059000  1.0
+  C  C112  1  0.91816000  0.89603000  0.96655000  1.0
+  C  C113  1  0.90529000  0.87748000  0.00497000  1.0
+  C  C114  1  0.75869000  0.73091000  0.74970000  1.0
+  C  C115  1  0.66678000  0.71269000  0.77095000  1.0
+  C  C116  1  0.75625000  0.65401000  0.79627000  1.0
+  C  C117  1  0.85228000  0.67193000  0.77817000  1.0
+  C  C118  1  0.85269000  0.71019000  0.75458000  1.0
+  C  C119  1  0.77711000  0.81952000  0.55126000  1.0
+  C  C120  1  0.86905000  0.79997000  0.55034000  1.0
+  C  C121  1  0.78135000  0.77828667  0.51422333  1.0
+  C  C122  1  0.69115000  0.80027000  0.51133000  1.0
+  C  C123  1  0.68919000  0.82086000  0.53007000  1.0
+  C  C124  1  0.72945000  0.59238000  0.62965000  1.0
+  C  C125  1  0.73568000  0.61327000  0.64788000  1.0
+  C  C126  1  0.71705000  0.55906000  0.70661000  1.0
+  C  C127  1  0.70514000  0.53694000  0.68978000  1.0
+  C  C128  1  0.71130000  0.55386000  0.65095000  1.0
+  C  C129  1  0.29500000  0.30646000  0.46088000  1.0
+  C  C130  1  0.20705000  0.32803333  0.44137667  1.0
+  C  C131  1  0.29399000  0.38366000  0.43041000  1.0
+  C  C132  1  0.38087000  0.36289000  0.45188000  1.0
+  C  C133  1  0.38072000  0.32406000  0.46737000  1.0
+  C  C134  1  0.35231000  0.42590000  0.21219000  1.0
+  C  C135  1  0.34775000  0.46504000  0.19450000  1.0
+  C  C136  1  0.34142000  0.46360000  0.25276000  1.0
+  C  C137  1  0.34633000  0.42465000  0.27117000  1.0
+  C  C138  1  0.35191000  0.40607000  0.25099000  1.0
+  C  C139  1  0.32447000  0.20897000  0.36005000  1.0
+  C  C140  1  0.23472000  0.22201000  0.33746000  1.0
+  C  C141  1  0.34656000  0.24595000  0.28318000  1.0
+  C  C142  1  0.43771000  0.23118000  0.30476000  1.0
+  C  C143  1  0.42621000  0.21233000  0.34327000  1.0
+  C  C144  1  0.32419000  0.18932000  0.97870000  1.0
+  C  C145  1  0.38544000  0.15840000  0.98402000  1.0
+  C  C146  1  0.54622000  0.18742000  0.98677000  1.0
+  C  C147  1  0.48826000  0.21938000  0.98043000  1.0
+  C  C148  1  0.37702000  0.22035000  0.97606000  1.0
+  C  C149  1  0.43439000  0.03007000  0.82177000  1.0
+  C  C150  1  0.49434000  0.03967000  0.78904000  1.0
+  C  C151  1  0.65767000  0.03880000  0.81808000  1.0
+  C  C152  1  0.60041000  0.03079000  0.85072000  1.0
+  C  C153  1  0.48890000  0.02691000  0.85234000  1.0
+  C  C154  1  0.35087000  0.85777000  0.16361000  1.0
+  C  C155  1  0.41142000  0.87994000  0.13122000  1.0
+  C  C156  1  0.57345000  0.85013000  0.16065000  1.0
+  C  C157  1  0.51631000  0.82824000  0.19402000  1.0
+  C  C158  1  0.40482000  0.83237000  0.19547000  1.0
+  C  C159  1  0.36787000  0.84819000  0.66306000  1.0
+  C  C160  1  0.31019000  0.82441000  0.65482000  1.0
+  C  C161  1  0.14672000  0.85498000  0.65446000  1.0
+  C  C162  1  0.20122000  0.87901000  0.66330000  1.0
+  C  C163  1  0.31218000  0.87524000  0.66801000  1.0
+  C  C164  1  0.37768000  0.67661000  0.49664000  1.0
+  C  C165  1  0.32021000  0.68701000  0.46444000  1.0
+  C  C166  1  0.15722000  0.66594000  0.49972000  1.0
+  C  C167  1  0.21166000  0.65602000  0.53239000  1.0
+  C  C168  1  0.32218000  0.66096000  0.53078000  1.0
+  C  C169  1  0.34673000  0.51256000  0.82180000  1.0
+  C  C170  1  0.28912000  0.48509000  0.85237000  1.0
+  C  C171  1  0.12328000  0.51482000  0.82662000  1.0
+  C  C172  1  0.17801000  0.54180000  0.79482000  1.0
+  C  C173  1  0.28989000  0.54093000  0.79284000  1.0
+  C  C174  1  0.70083000  0.52509000  0.31083000  1.0
+  C  C175  1  0.75510000  0.55230000  0.31508000  1.0
+  C  C176  1  0.92323000  0.52241000  0.31882000  1.0
+  C  C177  1  0.87209000  0.49575000  0.31280000  1.0
+  C  C178  1  0.76078000  0.49687000  0.30942000  1.0
+  C  C179  1  0.97835000  0.37378000  0.14123000  1.0
+  C  C180  1  0.92414000  0.36581333  0.11673667  1.0
+  C  C181  1  0.75569000  0.36378000  0.14645000  1.0
+  C  C182  1  0.80667000  0.37342667  0.17037333  1.0
+  C  C183  1  0.91808000  0.37805000  0.16788000  1.0
+  C  C184  1  0.68969000  0.18705000  0.50055000  1.0
+  C  C185  1  0.74998000  0.21151000  0.46903000  1.0
+  C  C186  1  0.91175000  0.18011000  0.49676000  1.0
+  C  C187  1  0.85471000  0.15563000  0.52926000  1.0
+  C  C188  1  0.74329000  0.15939000  0.53116000  1.0
+  H  H189  1  0.14019000  0.19021000  0.11698000  1.0
+  H  H190  1  0.11101000  0.29410000  0.01495000  1.0
+  H  H191  1  0.19993000  0.22499000  0.14736000  1.0
+  H  H192  1  0.15249000  0.13587000  0.69161000  1.0
+  H  H193  1  0.11090000  0.03505000  0.68595000  1.0
+  H  H194  1  0.23138000  0.16574000  0.62850000  1.0
+  H  H195  1  0.18461000  0.71385000  0.17146000  1.0
+  H  H196  1  0.16495000  0.71743000  0.27372000  1.0
+  H  H197  1  0.24955000  0.64929000  0.20601000  1.0
+  H  H198  1  0.82983000  0.68675000  0.35641000  1.0
+  H  H199  1  0.82440000  0.79147000  0.35636000  1.0
+  H  H200  1  0.89413000  0.71898000  0.29218000  1.0
+  H  H201  1  0.81176000  0.38378000  0.84707000  1.0
+  H  H202  1  0.80715000  0.37984000  0.95304000  1.0
+  H  H203  1  0.87139000  0.31849000  0.87763000  1.0
+  H  H204  1  0.87122000  0.01153000  0.70186000  1.0
+  H  H205  1  0.83657000  0.90576000  0.80207000  1.0
+  H  H206  1  0.82187000  0.98165000  0.66594000  1.0
+  H  H207  1  0.44857000  0.47997000  0.02470000  1.0
+  H  H208  1  0.44319000  0.38215000  0.01200000  1.0
+  H  H209  1  0.52231000  0.51579000  0.96097000  1.0
+  H  H210  1  0.50737000  0.05059000  0.49749000  1.0
+  H  H211  1  0.49278000  0.04550000  0.60398000  1.0
+  H  H212  1  0.57231000  0.98591000  0.52776000  1.0
+  H  H213  1  0.59940000  0.65342000  0.38519000  1.0
+  H  H214  1  0.57732000  0.54810000  0.48643000  1.0
+  H  H215  1  0.52857000  0.62419000  0.35158000  1.0
+  H  H216  1  0.08659000  0.97494000  0.15091000  1.0
+  H  H217  1  0.78695000  0.97694000  0.10038000  1.0
+  H  H218  1  0.07651000  0.04332000  0.12313000  1.0
+  H  H219  1  0.04150000  0.15120000  0.82691000  1.0
+  H  H220  1  0.96248000  0.04890000  0.92667000  1.0
+  H  H221  1  0.01081000  0.18540000  0.86159000  1.0
+  H  H222  1  0.82505000  0.87147000  0.01723000  1.0
+  H  H223  1  0.16893000  0.87154000  0.02658000  1.0
+  H  H224  1  0.84743000  0.90426000  0.94969000  1.0
+  H  H225  1  0.92558000  0.72340000  0.73899000  1.0
+  H  H226  1  0.59299000  0.72798000  0.76803000  1.0
+  H  H227  1  0.92482000  0.65631000  0.78020000  1.0
+  H  H228  1  0.61654000  0.83560000  0.53006000  1.0
+  H  H229  1  0.93954000  0.79876333  0.56559667  1.0
+  H  H230  1  0.62033000  0.79937000  0.49722000  1.0
+  H  H231  1  0.70531000  0.53689000  0.63779000  1.0
+  H  H232  1  0.74684000  0.64316000  0.63273000  1.0
+  H  H233  1  0.69467000  0.50710000  0.70629000  1.0
+  H  H234  1  0.44983000  0.30817000  0.48245000  1.0
+  H  H235  1  0.13828000  0.31534000  0.43655000  1.0
+  H  H236  1  0.45025000  0.37654000  0.45503000  1.0
+  H  H237  1  0.35518000  0.37593000  0.26605000  1.0
+  H  H238  1  0.34897000  0.48138000  0.16460000  1.0
+  H  H239  1  0.34562000  0.40844000  0.30112000  1.0
+  H  H240  1  0.49761000  0.20277000  0.35977000  1.0
+  H  H241  1  0.15483000  0.21951000  0.34942000  1.0
+  H  H242  1  0.51725000  0.23568000  0.29208000  1.0
+  H  H243  1  0.33170000  0.24437000  0.97277000  1.0
+  H  H244  1  0.34694000  0.13385000  0.98653000  1.0
+  H  H245  1  0.52807000  0.24298000  0.97957000  1.0
+  H  H246  1  0.44623000  0.01957000  0.87813000  1.0
+  H  H247  1  0.45524000  0.04295000  0.76463000  1.0
+  H  H248  1  0.64217000  0.02600000  0.87525000  1.0
+  H  H249  1  0.36028000  0.81419000  0.22069000  1.0
+  H  H250  1  0.37216000  0.89955000  0.10602000  1.0
+  H  H251  1  0.55695000  0.80773000  0.21844000  1.0
+  H  H252  1  0.35498000  0.89451000  0.67368000  1.0
+  H  H253  1  0.35113000  0.80341000  0.65058000  1.0
+  H  H254  1  0.15876000  0.90048000  0.66635000  1.0
+  H  H255  1  0.36452000  0.65223000  0.55623000  1.0
+  H  H256  1  0.36123000  0.69840000  0.43774000  1.0
+  H  H257  1  0.16953000  0.64405000  0.55894000  1.0
+  H  H258  1  0.33219000  0.56295000  0.76919000  1.0
+  H  H259  1  0.33101000  0.46326000  0.87558000  1.0
+  H  H260  1  0.13526000  0.56431000  0.77248000  1.0
+  H  H261  1  0.72107000  0.47495000  0.30704000  1.0
+  H  H262  1  0.71067000  0.57397000  0.31718000  1.0
+  H  H263  1  0.91681000  0.47322000  0.31243000  1.0
+  H  H264  1  0.95772000  0.38309000  0.18793000  1.0
+  H  H265  1  0.96868000  0.36137333  0.09644667  1.0
+  H  H266  1  0.76171000  0.37589667  0.19178333  1.0
+  H  H267  1  0.69861000  0.13952000  0.55559000  1.0
+  H  H268  1  0.71073000  0.23292000  0.44479000  1.0
+  H  H269  1  0.89546000  0.13361000  0.55267000  1.0
+  N  N270  1  0.16262000  0.29680000  0.06145000  1.0
+  N  N271  1  0.18066000  0.08076000  0.63939000  1.0
+  N  N272  1  0.21833000  0.66746000  0.27660000  1.0
+  N  N273  1  0.87506000  0.79250000  0.30687000  1.0
+  N  N274  1  0.85287000  0.33107000  0.95201000  1.0
+  N  N275  1  0.80599000  0.90702000  0.75170000  1.0
+  N  N276  1  0.50083000  0.43166000  0.96684000  1.0
+  N  N277  1  0.54495000  0.99742000  0.60262000  1.0
+  N  N278  1  0.52759000  0.54947000  0.43741000  1.0
+  N  N279  1  0.84718000  0.02826667  0.09114333  1.0
+  N  N280  1  0.95706000  0.09814000  0.92971000  1.0
+  N  N281  1  0.10788000  0.89751000  0.97273000  1.0
+  N  N282  1  0.66690000  0.67490000  0.79276000  1.0
+  N  N283  1  0.86786000  0.77956000  0.53286000  1.0
+  N  N284  1  0.73046000  0.59631000  0.68514000  1.0
+  N  N285  1  0.20928000  0.36551000  0.42654000  1.0
+  N  N286  1  0.34262000  0.48280000  0.21500000  1.0
+  N  N287  1  0.24792000  0.24022000  0.30004000  1.0
+  N  N288  1  0.49350000  0.15826000  0.98773000  1.0
+  N  N289  1  0.60321000  0.04334000  0.78813000  1.0
+  N  N290  1  0.51970000  0.87572000  0.13057000  1.0
+  N  N291  1  0.20221000  0.82814000  0.65106000  1.0
+  N  N292  1  0.21244000  0.68121000  0.46676000  1.0
+  N  N293  1  0.18011000  0.48721000  0.85432000  1.0
+  N  N294  1  0.86351000  0.55004000  0.31946000  1.0
+  N  N295  1  0.81567000  0.36079333  0.12006000  1.0
+  N  N296  1  0.85815000  0.20761000  0.46799000  1.0
+  O  O297  1  0.71762000  0.15932000  0.98923000  1.0
+  O  O298  1  0.85231000  0.10244000  0.04662000  1.0
+  O  O299  1  0.01097000  0.10840000  0.06976000  1.0
+  O  O300  1  0.70698000  0.20340000  0.00732000  1.0
+  O  O301  1  0.93628000  0.17973667  0.00225000  1.0
+  O  O302  1  0.05959000  0.18401333  0.06175667  1.0
+  O  O303  1  0.91025000  0.13150000  0.96977000  1.0
+  O  O304  1  0.97843000  0.18766000  0.92568000  1.0
+  O  O305  1  0.88109000  0.25559000  0.98851000  1.0
+  O  O306  1  0.93610000  0.25596000  0.93495000  1.0
+  O  O307  1  0.16797000  0.15866000  0.01405000  1.0
+  O  O308  1  0.14369000  0.21226000  0.95891000  1.0
+  O  O309  1  0.09590000  0.23641000  0.00752000  1.0
+  O  O310  1  0.25889000  0.02161000  0.85143000  1.0
+  O  O311  1  0.10886000  0.96174000  0.90314000  1.0
+  O  O312  1  0.95649000  0.94144000  0.88877000  1.0
+  O  O313  1  0.27620000  0.01152000  0.80219000  1.0
+  O  O314  1  0.04399000  0.01238000  0.82525000  1.0
+  O  O315  1  0.91747000  0.95891000  0.81133000  1.0
+  O  O316  1  0.05840000  0.03985000  0.87741000  1.0
+  O  O317  1  0.01516000  0.08789000  0.82028000  1.0
+  O  O318  1  0.10588000  0.02654000  0.75095000  1.0
+  O  O319  1  0.05442000  0.08061000  0.75040000  1.0
+  O  O320  1  0.81000000  0.00068000  0.84392000  1.0
+  O  O321  1  0.84076000  0.05864000  0.79435000  1.0
+  O  O322  1  0.87662000  0.01506000  0.76240000  1.0
+  O  O323  1  0.74409000  0.87245000  0.12974000  1.0
+  O  O324  1  0.91044000  0.87633000  0.07563000  1.0
+  O  O325  1  0.05401000  0.83658000  0.08980000  1.0
+  O  O326  1  0.73763000  0.81441000  0.18032000  1.0
+  O  O327  1  0.96556000  0.84120000  0.15590000  1.0
+  O  O328  1  0.09922000  0.77520000  0.16566000  1.0
+  O  O329  1  0.92232000  0.92210000  0.11223000  1.0
+  O  O330  1  0.98327000  0.90642000  0.16986000  1.0
+  O  O331  1  0.91179000  0.77718000  0.22921000  1.0
+  O  O332  1  0.96091000  0.82833000  0.23363000  1.0
+  O  O333  1  0.19885000  0.84916000  0.13572000  1.0
+  O  O334  1  0.16812000  0.85463000  0.18751000  1.0
+  O  O335  1  0.14138000  0.78081000  0.21551000  1.0
+  O  O336  1  0.97915000  0.82819000  0.65415000  1.0
+  O  O337  1  0.83153000  0.81710000  0.60728000  1.0
+  O  O338  1  0.69483000  0.85687000  0.57595000  1.0
+  O  O339  1  0.98117000  0.88982000  0.63785000  1.0
+  O  O340  1  0.75649000  0.85903000  0.64604000  1.0
+  O  O341  1  0.63670000  0.92314000  0.58510000  1.0
+  O  O342  1  0.80353000  0.77744000  0.68803000  1.0
+  O  O343  1  0.71026000  0.79590000  0.72464000  1.0
+  O  O344  1  0.80637000  0.92372000  0.65789000  1.0
+  O  O345  1  0.73860000  0.87367000  0.71058000  1.0
+  O  O346  1  0.52972000  0.85092000  0.63046000  1.0
+  O  O347  1  0.54235000  0.85131000  0.68535000  1.0
+  O  O348  1  0.59184000  0.92238000  0.63882000  1.0
+  O  O349  1  0.98484000  0.66311000  0.52733000  1.0
+  O  O350  1  0.79299000  0.64456000  0.57434000  1.0
+  O  O351  1  0.70955000  0.59898000  0.56826000  1.0
+  O  O352  1  0.99320000  0.66137000  0.47317000  1.0
+  O  O353  1  0.76651000  0.66979000  0.49521000  1.0
+  O  O354  1  0.66198000  0.60419000  0.49333000  1.0
+  O  O355  1  0.84283000  0.72026000  0.52258000  1.0
+  O  O356  1  0.70908000  0.74830000  0.48125000  1.0
+  O  O357  1  0.82570000  0.68169000  0.42021000  1.0
+  O  O358  1  0.74602000  0.73353000  0.41761000  1.0
+  O  O359  1  0.54309000  0.64729000  0.52127000  1.0
+  O  O360  1  0.54893000  0.70421000  0.46820000  1.0
+  O  O361  1  0.61531000  0.65845000  0.44342000  1.0
+  O  O362  1  0.94913000  0.53733000  0.80154000  1.0
+  O  O363  1  0.82441000  0.59629000  0.80418000  1.0
+  O  O364  1  0.65689000  0.59600000  0.82805000  1.0
+  O  O365  1  0.96087000  0.50175000  0.86423000  1.0
+  O  O366  1  0.73103000  0.52060000  0.83717000  1.0
+  O  O367  1  0.59256000  0.52333000  0.89625000  1.0
+  O  O368  1  0.75826000  0.56688000  0.75756000  1.0
+  O  O369  1  0.70063000  0.50921000  0.77064000  1.0
+  O  O370  1  0.79496000  0.44539000  0.89728000  1.0
+  O  O371  1  0.73388000  0.44346000  0.84646000  1.0
+  O  O372  1  0.50098000  0.54448000  0.82419000  1.0
+  O  O373  1  0.52704000  0.48788000  0.82714000  1.0
+  O  O374  1  0.57961000  0.46886000  0.89587000  1.0
+  O  O375  1  0.09760000  0.49570000  0.32110000  1.0
+  O  O376  1  0.22007000  0.44003000  0.38352000  1.0
+  O  O377  1  0.38913000  0.44248000  0.40218000  1.0
+  O  O378  1  0.08180000  0.53844000  0.34069000  1.0
+  O  O379  1  0.31369000  0.51520000  0.33618000  1.0
+  O  O380  1  0.44024000  0.51646000  0.39714000  1.0
+  O  O381  1  0.29032000  0.46265667  0.30889000  1.0
+  O  O382  1  0.35181000  0.51801000  0.26150000  1.0
+  O  O383  1  0.25509000  0.59242000  0.31761000  1.0
+  O  O384  1  0.31010000  0.58904000  0.26597000  1.0
+  O  O385  1  0.54641000  0.49411000  0.34724000  1.0
+  O  O386  1  0.51905000  0.54666000  0.29137000  1.0
+  O  O387  1  0.47331000  0.56973000  0.34348000  1.0
+  O  O388  1  0.58390000  0.35572000  0.17778000  1.0
+  O  O389  1  0.44294000  0.29350000  0.23078000  1.0
+  O  O390  1  0.27083000  0.28041000  0.22320000  1.0
+  O  O391  1  0.59394000  0.34504000  0.12882000  1.0
+  O  O392  1  0.36415000  0.34701000  0.15507000  1.0
+  O  O393  1  0.25237000  0.28560000  0.14916000  1.0
+  O  O394  1  0.39385000  0.37016000  0.21037000  1.0
+  O  O395  1  0.33731000  0.41995000  0.15654000  1.0
+  O  O396  1  0.41832000  0.36821000  0.07764000  1.0
+  O  O397  1  0.37658000  0.41949000  0.08349000  1.0
+  O  O398  1  0.12653000  0.33402000  0.16852000  1.0
+  O  O399  1  0.16397000  0.39469000  0.12528000  1.0
+  O  O400  1  0.19979000  0.33736000  0.09731000  1.0
+  O  O401  1  0.08100000  0.20591000  0.46754000  1.0
+  O  O402  1  0.24118000  0.21302000  0.41080000  1.0
+  O  O403  1  0.38828000  0.17536000  0.42216000  1.0
+  O  O404  1  0.07774000  0.14541000  0.51411000  1.0
+  O  O405  1  0.30335000  0.17597000  0.49103000  1.0
+  O  O406  1  0.43001000  0.11054000  0.49609000  1.0
+  O  O407  1  0.25564000  0.25716000  0.44867000  1.0
+  O  O408  1  0.34072000  0.24213000  0.50260000  1.0
+  O  O409  1  0.24525000  0.11435000  0.56676000  1.0
+  O  O410  1  0.29563000  0.16739000  0.56724000  1.0
+  O  O411  1  0.53608000  0.18268000  0.47073000  1.0
+  O  O412  1  0.50819000  0.18421000  0.52475000  1.0
+  O  O413  1  0.46645000  0.11100000  0.54909000  1.0
+  Zn  Zn414  1  0.03876000  0.15806000  0.03614000  1.0
+  Zn  Zn415  1  0.99493000  0.20828000  0.95675000  1.0
+  Zn  Zn416  1  0.85097000  0.20620000  0.01583000  1.0
+  Zn  Zn417  1  0.85642000  0.14495000  0.00223000  1.0
+  Zn  Zn418  1  0.93668000  0.97946000  0.84173000  1.0
+  Zn  Zn419  1  0.99172000  0.05865000  0.79794000  1.0
+  Zn  Zn420  1  0.13472000  0.99991000  0.79960000  1.0
+  Zn  Zn421  1  0.11618000  0.00860000  0.86280000  1.0
+  Zn  Zn422  1  0.07427000  0.82603000  0.13742000  1.0
+  Zn  Zn423  1  0.01745000  0.85689000  0.18593000  1.0
+  Zn  Zn424  1  0.88055000  0.80189000  0.18057000  1.0
+  Zn  Zn425  1  0.88925000  0.87615000  0.11964000  1.0
+  Zn  Zn426  1  0.65942000  0.87188000  0.61038000  1.0
+  Zn  Zn427  1  0.69020000  0.84568000  0.69001000  1.0
+  Zn  Zn428  1  0.83640000  0.89992000  0.63132000  1.0
+  Zn  Zn429  1  0.83807000  0.82225000  0.64844000  1.0
+  Zn  Zn430  1  0.67676000  0.63067000  0.51897000  1.0
+  Zn  Zn431  1  0.69565000  0.71250000  0.46638000  1.0
+  Zn  Zn432  1  0.84945000  0.65509000  0.46931000  1.0
+  Zn  Zn433  1  0.84356000  0.67399000  0.52803000  1.0
+  Zn  Zn434  1  0.62551000  0.54589000  0.84589000  1.0
+  Zn  Zn435  1  0.67629000  0.49093000  0.82120000  1.0
+  Zn  Zn436  1  0.81483000  0.49560000  0.87625000  1.0
+  Zn  Zn437  1  0.81292000  0.55371667  0.80193000  1.0
+  Zn  Zn438  1  0.41702000  0.49248000  0.36983000  1.0
+  Zn  Zn439  1  0.37032000  0.54161000  0.29005000  1.0
+  Zn  Zn440  1  0.22694000  0.54304000  0.34776000  1.0
+  Zn  Zn441  1  0.23286000  0.48015000  0.33759000  1.0
+  Zn  Zn442  1  0.25847000  0.31299000  0.17352000  1.0
+  Zn  Zn443  1  0.31339000  0.39395000  0.13073000  1.0
+  Zn  Zn444  1  0.44881000  0.33699000  0.12583000  1.0
+  Zn  Zn445  1  0.44414000  0.34129000  0.19185000  1.0
+  Zn  Zn446  1  0.40922000  0.16171000  0.47064000  1.0
+  Zn  Zn447  1  0.35985000  0.19156000  0.52058000  1.0
+  Zn  Zn448  1  0.22289000  0.13535000  0.51730000  1.0
+  Zn  Zn449  1  0.22417000  0.21115000  0.45581000  1.0
```

### Comparing `moftransformer-2.0.0/moftransformer/examples/raw/msp+N624+E8.cif` & `moftransformer-2.0.1/moftransformer/examples/raw/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/raw/sml+N696+E182.cif` & `moftransformer-2.0.1/moftransformer/examples/raw/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/raw/vmk+N489+E8.cif` & `moftransformer-2.0.1/moftransformer/examples/raw/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/raw/vna+N650+E120.cif` & `moftransformer-2.0.1/moftransformer/examples/raw/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/raw/zzz+N96+N373+E34.cif` & `moftransformer-2.0.1/moftransformer/examples/raw/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 data_image0
-_chemical_formula_structural       Zn8H24C48O26
-_chemical_formula_sum              "Zn8 H24 C48 O26"
-_cell_length_a       18.4202
-_cell_length_b       18.4202
-_cell_length_c       18.4202
-_cell_angle_alpha    60
-_cell_angle_beta     60.0001
-_cell_angle_gamma    60.0001
+_chemical_formula_structural       Zn8H12C48Br12O26
+_chemical_formula_sum              "Zn8 H12 C48 Br12 O26"
+_cell_length_a       18.1188
+_cell_length_b       18.2004
+_cell_length_c       18.2326
+_cell_angle_alpha    61.7008
+_cell_angle_beta     61.6541
+_cell_angle_gamma    61.5361
 
 _space_group_name_H-M_alt    "P 1"
 _space_group_IT_number       1
 
 loop_
   _space_group_symop_operation_xyz
   'x, y, z'
@@ -19,113 +19,113 @@
   _atom_site_type_symbol
   _atom_site_label
   _atom_site_symmetry_multiplicity
   _atom_site_fract_x
   _atom_site_fract_y
   _atom_site_fract_z
   _atom_site_occupancy
-  Zn  Zn1       1.0  0.70648  0.70648  0.88055  1.0000
-  Zn  Zn2       1.0  0.70648  0.88055  0.70648  1.0000
-  Zn  Zn3       1.0  0.88055  0.70648  0.70648  1.0000
-  Zn  Zn4       1.0  0.70648  0.70648  0.70648  1.0000
-  Zn  Zn5       1.0  0.29352  0.29352  0.11945  1.0000
-  Zn  Zn6       1.0  0.29352  0.11945  0.29352  1.0000
-  Zn  Zn7       1.0  0.29352  0.29352  0.29352  1.0000
-  Zn  Zn8       1.0  0.11945  0.29351  0.29352  1.0000
-  H   H1        1.0  0.54831  0.83516  0.06823  1.0000
-  H   H2        1.0  0.54831  0.06823  0.83516  1.0000
-  H   H3        1.0  0.06823  0.54831  0.54831  1.0000
-  H   H4        1.0  0.83516  0.54831  0.54831  1.0000
-  H   H5        1.0  0.54831  0.54831  0.83516  1.0000
-  H   H6        1.0  0.54831  0.54831  0.06823  1.0000
-  H   H7        1.0  0.06823  0.83516  0.54831  1.0000
-  H   H8        1.0  0.83516  0.06823  0.54831  1.0000
-  H   H9        1.0  0.54831  0.06823  0.54831  1.0000
-  H   H10       1.0  0.54831  0.83516  0.54831  1.0000
-  H   H11       1.0  0.06823  0.54831  0.83516  1.0000
-  H   H12       1.0  0.83516  0.54831  0.06823  1.0000
-  H   H13       1.0  0.45169  0.16484  0.93177  1.0000
-  H   H14       1.0  0.45169  0.93177  0.16484  1.0000
-  H   H15       1.0  0.16484  0.45169  0.45169  1.0000
-  H   H16       1.0  0.93177  0.45169  0.45169  1.0000
-  H   H17       1.0  0.93177  0.45169  0.16484  1.0000
-  H   H18       1.0  0.16485  0.45169  0.93177  1.0000
-  H   H19       1.0  0.45169  0.16484  0.45169  1.0000
-  H   H20       1.0  0.45169  0.93177  0.45169  1.0000
-  H   H21       1.0  0.16484  0.93177  0.45169  1.0000
-  H   H22       1.0  0.93177  0.16484  0.45169  1.0000
-  H   H23       1.0  0.45169  0.45169  0.16484  1.0000
-  H   H24       1.0  0.45169  0.45169  0.93177  1.0000
-  C   C1        1.0  0.61101  0.88899  0.88899  1.0000
-  C   C2        1.0  0.88899  0.61101  0.61101  1.0000
-  C   C3        1.0  0.61101  0.61101  0.88899  1.0000
-  C   C4        1.0  0.88899  0.88899  0.61101  1.0000
-  C   C5        1.0  0.61101  0.88899  0.61101  1.0000
-  C   C6        1.0  0.88899  0.61101  0.88899  1.0000
-  C   C7        1.0  0.38899  0.11101  0.11101  1.0000
-  C   C8        1.0  0.11101  0.38899  0.38899  1.0000
-  C   C9        1.0  0.11101  0.38899  0.11101  1.0000
-  C   C10       1.0  0.38899  0.11101  0.38899  1.0000
-  C   C11       1.0  0.11101  0.11101  0.38899  1.0000
-  C   C12       1.0  0.38899  0.38899  0.11101  1.0000
-  C   C13       1.0  0.55364  0.94636  0.94636  1.0000
-  C   C14       1.0  0.94636  0.55364  0.55364  1.0000
-  C   C15       1.0  0.55364  0.55364  0.94636  1.0000
-  C   C16       1.0  0.94636  0.94636  0.55364  1.0000
-  C   C17       1.0  0.55364  0.94636  0.55364  1.0000
-  C   C18       1.0  0.94636  0.55364  0.94636  1.0000
-  C   C19       1.0  0.44636  0.05364  0.05364  1.0000
-  C   C20       1.0  0.05364  0.44636  0.44636  1.0000
-  C   C21       1.0  0.05364  0.44636  0.05364  1.0000
-  C   C22       1.0  0.44636  0.05364  0.44636  1.0000
-  C   C23       1.0  0.05364  0.05364  0.44636  1.0000
-  C   C24       1.0  0.44636  0.44636  0.05364  1.0000
-  C   C25       1.0  0.52669  0.90740  0.03923  1.0000
-  C   C26       1.0  0.52669  0.03923  0.90740  1.0000
-  C   C27       1.0  0.03923  0.52669  0.52669  1.0000
-  C   C28       1.0  0.90740  0.52669  0.52669  1.0000
-  C   C29       1.0  0.52669  0.52669  0.90740  1.0000
-  C   C30       1.0  0.52669  0.52669  0.03923  1.0000
-  C   C31       1.0  0.03923  0.90740  0.52669  1.0000
-  C   C32       1.0  0.90740  0.03923  0.52669  1.0000
-  C   C33       1.0  0.52669  0.03923  0.52669  1.0000
-  C   C34       1.0  0.52669  0.90740  0.52669  1.0000
-  C   C35       1.0  0.03923  0.52669  0.90740  1.0000
-  C   C36       1.0  0.90740  0.52669  0.03923  1.0000
-  C   C37       1.0  0.47331  0.09260  0.96077  1.0000
-  C   C38       1.0  0.47331  0.96077  0.09260  1.0000
-  C   C39       1.0  0.09260  0.47331  0.47331  1.0000
-  C   C40       1.0  0.96077  0.47331  0.47331  1.0000
-  C   C41       1.0  0.96077  0.47331  0.09260  1.0000
-  C   C42       1.0  0.09260  0.47331  0.96077  1.0000
-  C   C43       1.0  0.47331  0.09260  0.47331  1.0000
-  C   C44       1.0  0.47331  0.96077  0.47331  1.0000
-  C   C45       1.0  0.09260  0.96077  0.47331  1.0000
-  C   C46       1.0  0.96077  0.09260  0.47331  1.0000
-  C   C47       1.0  0.47331  0.47331  0.09260  1.0000
-  C   C48       1.0  0.47331  0.47331  0.96077  1.0000
-  O   O1        1.0  0.75000  0.75000  0.75000  1.0000
-  O   O2        1.0  0.25000  0.25000  0.25000  1.0000
-  O   O3        1.0  0.63317  0.80498  0.92868  1.0000
-  O   O4        1.0  0.63317  0.92868  0.80498  1.0000
-  O   O5        1.0  0.92868  0.63317  0.63317  1.0000
-  O   O6        1.0  0.80498  0.63317  0.63317  1.0000
-  O   O7        1.0  0.63317  0.63317  0.80498  1.0000
-  O   O8        1.0  0.63317  0.63317  0.92868  1.0000
-  O   O9        1.0  0.92868  0.80498  0.63317  1.0000
-  O   O10       1.0  0.80498  0.92868  0.63317  1.0000
-  O   O11       1.0  0.63317  0.92868  0.63317  1.0000
-  O   O12       1.0  0.63317  0.80498  0.63317  1.0000
-  O   O13       1.0  0.92868  0.63317  0.80498  1.0000
-  O   O14       1.0  0.80498  0.63317  0.92869  1.0000
-  O   O15       1.0  0.36683  0.19502  0.07131  1.0000
-  O   O16       1.0  0.36683  0.07131  0.19502  1.0000
-  O   O17       1.0  0.19502  0.36683  0.36683  1.0000
-  O   O18       1.0  0.07132  0.36683  0.36683  1.0000
-  O   O19       1.0  0.07132  0.36683  0.19502  1.0000
-  O   O20       1.0  0.19502  0.36683  0.07132  1.0000
-  O   O21       1.0  0.36683  0.19502  0.36683  1.0000
-  O   O22       1.0  0.36683  0.07132  0.36683  1.0000
-  O   O23       1.0  0.19502  0.07131  0.36683  1.0000
-  O   O24       1.0  0.07132  0.19502  0.36683  1.0000
-  O   O25       1.0  0.36683  0.36683  0.19502  1.0000
-  O   O26       1.0  0.36683  0.36683  0.07132  1.0000
+  Zn  Zn1       1.0  0.85884  0.04963  0.05993  1.0000
+  Zn  Zn2       1.0  0.03507  0.04798  0.06675  1.0000
+  Zn  Zn3       1.0  0.03160  0.05096  0.88964  1.0000
+  Zn  Zn4       1.0  0.03113  0.87677  0.05820  1.0000
+  Zn  Zn5       1.0  0.61961  0.46477  0.47491  1.0000
+  Zn  Zn6       1.0  0.44408  0.45708  0.47747  1.0000
+  Zn  Zn7       1.0  0.44592  0.63582  0.47483  1.0000
+  Zn  Zn8       1.0  0.44680  0.46801  0.64765  1.0000
+  H   H1        1.0  0.78927  0.31872  0.11003  1.0000
+  H   H2        1.0  0.68795  0.18436  0.43565  1.0000
+  H   H3        1.0  0.78625  0.09728  0.80933  1.0000
+  H   H4        1.0  0.69392  0.42391  0.72453  1.0000
+  H   H5        1.0  0.78727  0.81484  0.33013  1.0000
+  H   H6        1.0  0.68825  0.70094  0.20412  1.0000
+  H   H7        1.0  0.07139  0.32490  0.82413  1.0000
+  H   H8        1.0  0.40024  0.19446  0.72604  1.0000
+  H   H9        1.0  0.30907  0.80250  0.10571  1.0000
+  H   H10       1.0  0.17135  0.69410  0.43049  1.0000
+  H   H11       1.0  0.30311  0.82510  0.80670  1.0000
+  H   H12       1.0  0.17703  0.70047  0.71906  1.0000
+  C   C1        1.0  0.85390  0.14116  0.16032  1.0000
+  C   C2        1.0  0.79532  0.19755  0.21939  1.0000
+  C   C3        1.0  0.76770  0.28929  0.18133  1.0000
+  C   C4        1.0  0.71236  0.34262  0.23476  1.0000
+  C   C5        1.0  0.68324  0.30571  0.32636  1.0000
+  C   C6        1.0  0.71030  0.21393  0.36438  1.0000
+  C   C7        1.0  0.76616  0.16056  0.31093  1.0000
+  C   C8        1.0  0.62503  0.36286  0.38473  1.0000
+  C   C9        1.0  0.85063  0.14598  0.87950  1.0000
+  C   C10       1.0  0.79331  0.20601  0.82140  1.0000
+  C   C11       1.0  0.76602  0.16874  0.79084  1.0000
+  C   C12       1.0  0.71302  0.22332  0.73694  1.0000
+  C   C13       1.0  0.68678  0.31510  0.71266  1.0000
+  C   C14       1.0  0.71417  0.35241  0.74306  1.0000
+  C   C15       1.0  0.76712  0.29781  0.79714  1.0000
+  C   C16       1.0  0.62892  0.37415  0.65509  1.0000
+  C   C17       1.0  0.84946  0.86915  0.15279  1.0000
+  C   C18       1.0  0.79136  0.81180  0.21124  1.0000
+  C   C19       1.0  0.76560  0.78995  0.30248  1.0000
+  C   C20       1.0  0.71244  0.73625  0.35767  1.0000
+  C   C21       1.0  0.68420  0.70396  0.32295  1.0000
+  C   C22       1.0  0.70985  0.72590  0.23174  1.0000
+  C   C23       1.0  0.76307  0.77951  0.17659  1.0000
+  C   C24       1.0  0.62683  0.64585  0.38096  1.0000
+  C   C25       1.0  0.12577  0.14669  0.88857  1.0000
+  C   C26       1.0  0.18328  0.20476  0.83159  1.0000
+  C   C27       1.0  0.14341  0.29630  0.80333  1.0000
+  C   C28       1.0  0.19599  0.35055  0.74786  1.0000
+  C   C29       1.0  0.28844  0.31466  0.71951  1.0000
+  C   C30       1.0  0.32827  0.22313  0.74773  1.0000
+  C   C31       1.0  0.27573  0.16894  0.80343  1.0000
+  C   C32       1.0  0.34684  0.37167  0.65971  1.0000
+  C   C33       1.0  0.13008  0.86608  0.15517  1.0000
+  C   C34       1.0  0.18649  0.80571  0.21424  1.0000
+  C   C35       1.0  0.27879  0.77898  0.17681  1.0000
+  C   C36       1.0  0.33174  0.72246  0.23069  1.0000
+  C   C37       1.0  0.29386  0.69172  0.32204  1.0000
+  C   C38       1.0  0.20156  0.71775  0.35941  1.0000
+  C   C39       1.0  0.14860  0.77445  0.30555  1.0000
+  C   C40       1.0  0.35039  0.63459  0.38119  1.0000
+  C   C41       1.0  0.12525  0.87228  0.87607  1.0000
+  C   C42       1.0  0.18383  0.81581  0.81722  1.0000
+  C   C43       1.0  0.27553  0.79753  0.78780  1.0000
+  C   C44       1.0  0.33121  0.74382  0.73473  1.0000
+  C   C45       1.0  0.29641  0.70859  0.70968  1.0000
+  C   C46       1.0  0.20465  0.72757  0.73842  1.0000
+  C   C47       1.0  0.14900  0.78071  0.79205  1.0000
+  C   C48       1.0  0.35474  0.64979  0.65313  1.0000
+  Br  Br1       1.0  0.67556  0.46725  0.18137  1.0000
+  Br  Br2       1.0  0.80227  0.03588  0.36387  1.0000
+  Br  Br3       1.0  0.67580  0.17148  0.69658  1.0000
+  Br  Br4       1.0  0.80373  0.34973  0.83792  1.0000
+  Br  Br5       1.0  0.67889  0.70663  0.48153  1.0000
+  Br  Br6       1.0  0.79706  0.80858  0.05273  1.0000
+  Br  Br7       1.0  0.14019  0.47487  0.70993  1.0000
+  Br  Br8       1.0  0.33152  0.04453  0.83988  1.0000
+  Br  Br9       1.0  0.45719  0.68718  0.17855  1.0000
+  Br  Br10      1.0  0.02316  0.80979  0.35784  1.0000
+  Br  Br11      1.0  0.45581  0.71868  0.69635  1.0000
+  Br  Br12      1.0  0.02443  0.80583  0.83025  1.0000
+  O   O1        1.0  0.98945  0.00666  0.01907  1.0000
+  O   O2        1.0  0.93702  0.11864  0.14243  1.0000
+  O   O3        1.0  0.81348  0.12346  0.13294  1.0000
+  O   O4        1.0  0.54199  0.37866  0.40959  1.0000
+  O   O5        1.0  0.66557  0.38853  0.40413  1.0000
+  O   O6        1.0  0.93368  0.12295  0.84017  1.0000
+  O   O7        1.0  0.81026  0.12311  0.96175  1.0000
+  O   O8        1.0  0.54597  0.39605  0.69515  1.0000
+  O   O9        1.0  0.66870  0.39661  0.57275  1.0000
+  O   O10       1.0  0.93248  0.82891  0.13197  1.0000
+  O   O11       1.0  0.80974  0.95188  0.13152  1.0000
+  O   O12       1.0  0.54365  0.68516  0.40229  1.0000
+  O   O13       1.0  0.66743  0.56327  0.40106  1.0000
+  O   O14       1.0  0.10224  0.12651  0.84696  1.0000
+  O   O15       1.0  0.10571  0.12481  0.97131  1.0000
+  O   O16       1.0  0.36772  0.39877  0.69761  1.0000
+  O   O17       1.0  0.37091  0.38522  0.57783  1.0000
+  O   O18       1.0  0.10929  0.82794  0.12825  1.0000
+  O   O19       1.0  0.11024  0.94845  0.13708  1.0000
+  O   O20       1.0  0.37119  0.67649  0.40384  1.0000
+  O   O21       1.0  0.37025  0.55161  0.40352  1.0000
+  O   O22       1.0  0.10621  0.95514  0.83796  1.0000
+  O   O23       1.0  0.10227  0.83123  0.95808  1.0000
+  O   O24       1.0  0.37981  0.56769  0.69400  1.0000
+  O   O25       1.0  0.37123  0.68767  0.57062  1.0000
+  O   O26       1.0  0.48900  0.50585  0.51823  1.0000
```

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 data_image0
-_chemical_formula_structural       Zn8H30C48N6O26
-_chemical_formula_sum              "Zn8 H30 C48 N6 O26"
-_cell_length_a       18.3679
-_cell_length_b       18.2349
-_cell_length_c       18.387
-_cell_angle_alpha    60.5571
-_cell_angle_beta     60.8763
-_cell_angle_gamma    60.1754
+_chemical_formula_structural       Ni8H24C48O26
+_chemical_formula_sum              "Ni8 H24 C48 O26"
+_cell_length_a       18.2553
+_cell_length_b       18.2552
+_cell_length_c       18.2554
+_cell_angle_alpha    59.9991
+_cell_angle_beta     59.9992
+_cell_angle_gamma    59.9988
 
 _space_group_name_H-M_alt    "P 1"
 _space_group_IT_number       1
 
 loop_
   _space_group_symop_operation_xyz
   'x, y, z'
@@ -19,125 +19,113 @@
   _atom_site_type_symbol
   _atom_site_label
   _atom_site_symmetry_multiplicity
   _atom_site_fract_x
   _atom_site_fract_y
   _atom_site_fract_z
   _atom_site_occupancy
-  Zn  Zn1       1.0  0.04456  0.84993  0.05181  1.0000
-  Zn  Zn2       1.0  0.04461  0.02865  0.04846  1.0000
-  Zn  Zn3       1.0  0.87206  0.02586  0.04810  1.0000
-  Zn  Zn4       1.0  0.04541  0.02317  0.87750  1.0000
-  Zn  Zn5       1.0  0.45929  0.61046  0.46844  1.0000
-  Zn  Zn6       1.0  0.45609  0.43666  0.46286  1.0000
-  Zn  Zn7       1.0  0.45831  0.44030  0.63304  1.0000
-  Zn  Zn8       1.0  0.63154  0.44025  0.46507  1.0000
-  H   H1        1.0  0.18851  0.66529  0.22701  1.0000
-  H   H2        1.0  0.28184  0.57392  0.32651  1.0000
-  H   H3        1.0  0.28468  0.89181  0.27896  1.0000
-  H   H4        1.0  0.33696  0.78911  0.34712  1.0000
-  H   H5        1.0  0.21090  0.90296  0.19688  1.0000
-  H   H6        1.0  0.91307  0.66129  0.19299  1.0000
-  H   H7        1.0  0.81210  0.57030  0.28887  1.0000
-  H   H8        1.0  0.54628  0.88873  0.29909  1.0000
-  H   H9        1.0  0.52726  0.78664  0.35244  1.0000
-  H   H10       1.0  0.68878  0.89925  0.22108  1.0000
-  H   H11       1.0  0.16988  0.66570  0.91140  1.0000
-  H   H12       1.0  0.27041  0.57405  0.81046  1.0000
-  H   H13       1.0  0.38864  0.85522  0.58658  1.0000
-  H   H14       1.0  0.42231  0.76272  0.55698  1.0000
-  H   H15       1.0  0.26500  0.88253  0.71340  1.0000
-  H   H16       1.0  0.68482  0.21950  0.17588  1.0000
-  H   H17       1.0  0.59231  0.31138  0.27664  1.0000
-  H   H18       1.0  0.89516  0.19760  0.34663  1.0000
-  H   H19       1.0  0.79426  0.27218  0.39341  1.0000
-  H   H20       1.0  0.91143  0.14540  0.24322  1.0000
-  H   H21       1.0  0.21613  0.16750  0.69035  1.0000
-  H   H22       1.0  0.31321  0.26261  0.59610  1.0000
-  H   H23       1.0  0.22878  0.31786  0.89685  1.0000
-  H   H24       1.0  0.30114  0.36363  0.79610  1.0000
-  H   H25       1.0  0.17422  0.21458  0.91692  1.0000
-  H   H26       1.0  0.91228  0.20471  0.69008  1.0000
-  H   H27       1.0  0.81052  0.30453  0.59886  1.0000
-  H   H28       1.0  0.55306  0.19783  0.89834  1.0000
-  H   H29       1.0  0.53187  0.27473  0.79856  1.0000
-  H   H30       1.0  0.69257  0.14155  0.91572  1.0000
-  C   C1        1.0  0.13954  0.84618  0.14635  1.0000
-  C   C2        1.0  0.19481  0.78975  0.20636  1.0000
-  C   C3        1.0  0.21420  0.69634  0.24262  1.0000
-  C   C4        1.0  0.26565  0.64628  0.29761  1.0000
-  C   C5        1.0  0.29867  0.68580  0.31905  1.0000
-  C   C6        1.0  0.35351  0.62653  0.37808  1.0000
-  C   C7        1.0  0.27870  0.78061  0.28253  1.0000
-  C   C8        1.0  0.22664  0.83055  0.22603  1.0000
-  C   C9        1.0  0.86351  0.84249  0.14518  1.0000
-  C   C10       1.0  0.80553  0.78589  0.20194  1.0000
-  C   C11       1.0  0.84205  0.69244  0.22054  1.0000
-  C   C12       1.0  0.78609  0.64263  0.27349  1.0000
-  C   C13       1.0  0.69391  0.68240  0.30921  1.0000
-  C   C14       1.0  0.63904  0.62408  0.36437  1.0000
-  C   C15       1.0  0.65705  0.77712  0.29070  1.0000
-  C   C16       1.0  0.71505  0.82683  0.23643  1.0000
-  C   C17       1.0  0.14939  0.83785  0.87332  1.0000
-  C   C18       1.0  0.21227  0.77961  0.81695  1.0000
-  C   C19       1.0  0.21343  0.69181  0.84644  1.0000
-  C   C20       1.0  0.26902  0.64162  0.79051  1.0000
-  C   C21       1.0  0.32477  0.67543  0.70575  1.0000
-  C   C22       1.0  0.37897  0.61804  0.64972  1.0000
-  C   C23       1.0  0.32566  0.76347  0.67691  1.0000
-  C   C24       1.0  0.26760  0.81416  0.73445  1.0000
-  C   C25       1.0  0.86157  0.12294  0.14366  1.0000
-  C   C26       1.0  0.80389  0.17748  0.20412  1.0000
-  C   C27       1.0  0.71316  0.22365  0.21316  1.0000
-  C   C28       1.0  0.66240  0.27408  0.26903  1.0000
-  C   C29       1.0  0.69836  0.28046  0.31740  1.0000
-  C   C30       1.0  0.63963  0.33793  0.37361  1.0000
-  C   C31       1.0  0.79011  0.23226  0.30943  1.0000
-  C   C32       1.0  0.84106  0.18186  0.25137  1.0000
-  C   C33       1.0  0.13345  0.12794  0.86750  1.0000
-  C   C34       1.0  0.19004  0.18592  0.80941  1.0000
-  C   C35       1.0  0.22862  0.19910  0.71824  1.0000
-  C   C36       1.0  0.28191  0.25171  0.66665  1.0000
-  C   C37       1.0  0.29825  0.29314  0.70219  1.0000
-  C   C38       1.0  0.35630  0.34802  0.64255  1.0000
-  C   C39       1.0  0.25810  0.28076  0.79450  1.0000
-  C   C40       1.0  0.20462  0.22611  0.84617  1.0000
-  C   C41       1.0  0.86500  0.11087  0.86568  1.0000
-  C   C42       1.0  0.80711  0.16765  0.80837  1.0000
-  C   C43       1.0  0.84226  0.21268  0.71827  1.0000
-  C   C44       1.0  0.78584  0.26743  0.66831  1.0000
-  C   C45       1.0  0.69484  0.27851  0.70431  1.0000
-  C   C46       1.0  0.63957  0.33930  0.64618  1.0000
-  C   C47       1.0  0.65962  0.23125  0.79535  1.0000
-  C   C48       1.0  0.71802  0.17682  0.84568  1.0000
-  N   N1        1.0  0.30977  0.82425  0.29789  1.0000
-  N   N2        1.0  0.56896  0.82124  0.32519  1.0000
-  N   N3        1.0  0.37887  0.80066  0.59664  1.0000
-  N   N4        1.0  0.82986  0.23189  0.35572  1.0000
-  N   N5        1.0  0.27028  0.31738  0.83541  1.0000
-  N   N6        1.0  0.57308  0.23701  0.83543  1.0000
-  O   O1        1.0  0.00197  0.98138  0.00675  1.0000
-  O   O2        1.0  0.12317  0.93061  0.11727  1.0000
-  O   O3        1.0  0.11332  0.80523  0.12907  1.0000
-  O   O4        1.0  0.37681  0.54214  0.39811  1.0000
-  O   O5        1.0  0.37441  0.66405  0.40601  1.0000
-  O   O6        1.0  0.82485  0.92711  0.12736  1.0000
-  O   O7        1.0  0.94683  0.80167  0.11943  1.0000
-  O   O8        1.0  0.67834  0.53926  0.38448  1.0000
-  O   O9        1.0  0.55413  0.66243  0.38888  1.0000
-  O   O10       1.0  0.13162  0.92215  0.83409  1.0000
-  O   O11       1.0  0.11823  0.79867  0.95561  1.0000
-  O   O12       1.0  0.38699  0.53508  0.68648  1.0000
-  O   O13       1.0  0.41459  0.65453  0.56660  1.0000
-  O   O14       1.0  0.82271  0.10873  0.11250  1.0000
-  O   O15       1.0  0.94511  0.09476  0.12810  1.0000
-  O   O16       1.0  0.67574  0.35095  0.40955  1.0000
-  O   O17       1.0  0.55687  0.37183  0.38301  1.0000
-  O   O18       1.0  0.11337  0.10198  0.82883  1.0000
-  O   O19       1.0  0.10993  0.10892  0.95081  1.0000
-  O   O20       1.0  0.37129  0.38338  0.67757  1.0000
-  O   O21       1.0  0.38843  0.35776  0.56028  1.0000
-  O   O22       1.0  0.94856  0.09121  0.82693  1.0000
-  O   O23       1.0  0.82600  0.08707  0.94885  1.0000
-  O   O24       1.0  0.55571  0.35130  0.68061  1.0000
-  O   O25       1.0  0.67715  0.37725  0.56509  1.0000
-  O   O26       1.0  0.50195  0.48102  0.50486  1.0000
+  Ni  Ni1       1.0  0.79235  0.79234  0.79232  1.0000
+  Ni  Ni2       1.0  0.62303  0.79234  0.79231  1.0000
+  Ni  Ni3       1.0  0.79235  0.62300  0.79232  1.0000
+  Ni  Ni4       1.0  0.79234  0.79234  0.62300  1.0000
+  Ni  Ni5       1.0  0.37699  0.20766  0.20766  1.0000
+  Ni  Ni6       1.0  0.20766  0.20765  0.20766  1.0000
+  Ni  Ni7       1.0  0.20766  0.37698  0.20766  1.0000
+  Ni  Ni8       1.0  0.20766  0.20766  0.37699  1.0000
+  H   H1        1.0  0.66624  0.95146  0.95146  1.0000
+  H   H2        1.0  0.43084  0.95146  0.95146  1.0000
+  H   H3        1.0  0.95146  0.43085  0.66624  1.0000
+  H   H4        1.0  0.95146  0.66624  0.43085  1.0000
+  H   H5        1.0  0.95146  0.95146  0.66624  1.0000
+  H   H6        1.0  0.95146  0.95146  0.43085  1.0000
+  H   H7        1.0  0.43085  0.66624  0.95146  1.0000
+  H   H8        1.0  0.66624  0.43085  0.95146  1.0000
+  H   H9        1.0  0.95146  0.66624  0.95146  1.0000
+  H   H10       1.0  0.95146  0.43084  0.95146  1.0000
+  H   H11       1.0  0.66624  0.95146  0.43085  1.0000
+  H   H12       1.0  0.43085  0.95146  0.66624  1.0000
+  H   H13       1.0  0.56915  0.04855  0.04855  1.0000
+  H   H14       1.0  0.33375  0.04855  0.04855  1.0000
+  H   H15       1.0  0.04854  0.56916  0.33376  1.0000
+  H   H16       1.0  0.04854  0.33376  0.56916  1.0000
+  H   H17       1.0  0.56916  0.04855  0.33376  1.0000
+  H   H18       1.0  0.33376  0.04855  0.56916  1.0000
+  H   H19       1.0  0.04855  0.33375  0.04855  1.0000
+  H   H20       1.0  0.04855  0.56915  0.04855  1.0000
+  H   H21       1.0  0.56915  0.33376  0.04855  1.0000
+  H   H22       1.0  0.33376  0.56916  0.04855  1.0000
+  H   H23       1.0  0.04855  0.04855  0.56915  1.0000
+  H   H24       1.0  0.04854  0.04855  0.33376  1.0000
+  C   C1        1.0  0.59341  0.97309  0.97309  1.0000
+  C   C2        1.0  0.46041  0.97309  0.97309  1.0000
+  C   C3        1.0  0.97308  0.46042  0.59342  1.0000
+  C   C4        1.0  0.97308  0.59342  0.46042  1.0000
+  C   C5        1.0  0.97308  0.97308  0.59342  1.0000
+  C   C6        1.0  0.97308  0.97308  0.46042  1.0000
+  C   C7        1.0  0.46041  0.59342  0.97308  1.0000
+  C   C8        1.0  0.59342  0.46042  0.97308  1.0000
+  C   C9        1.0  0.97309  0.59341  0.97309  1.0000
+  C   C10       1.0  0.97309  0.46042  0.97309  1.0000
+  C   C11       1.0  0.59342  0.97308  0.46042  1.0000
+  C   C12       1.0  0.46042  0.97308  0.59342  1.0000
+  C   C13       1.0  0.53957  0.02693  0.02693  1.0000
+  C   C14       1.0  0.40657  0.02693  0.02693  1.0000
+  C   C15       1.0  0.02692  0.53958  0.40658  1.0000
+  C   C16       1.0  0.02692  0.40658  0.53958  1.0000
+  C   C17       1.0  0.53958  0.02692  0.40658  1.0000
+  C   C18       1.0  0.40658  0.02692  0.53958  1.0000
+  C   C19       1.0  0.02693  0.40657  0.02693  1.0000
+  C   C20       1.0  0.02693  0.53957  0.02693  1.0000
+  C   C21       1.0  0.53958  0.40658  0.02692  1.0000
+  C   C22       1.0  0.40658  0.53958  0.02692  1.0000
+  C   C23       1.0  0.02692  0.02693  0.53957  1.0000
+  C   C24       1.0  0.02692  0.02693  0.40658  1.0000
+  C   C25       1.0  0.61192  0.88808  0.88807  1.0000
+  C   C26       1.0  0.55416  0.94584  0.94585  1.0000
+  C   C27       1.0  0.88807  0.61194  0.61192  1.0000
+  C   C28       1.0  0.94583  0.55417  0.55416  1.0000
+  C   C29       1.0  0.88807  0.88807  0.61192  1.0000
+  C   C30       1.0  0.94583  0.94584  0.55416  1.0000
+  C   C31       1.0  0.61192  0.61193  0.88808  1.0000
+  C   C32       1.0  0.55415  0.55415  0.94584  1.0000
+  C   C33       1.0  0.88807  0.61193  0.88807  1.0000
+  C   C34       1.0  0.94584  0.55416  0.94584  1.0000
+  C   C35       1.0  0.61194  0.88808  0.61192  1.0000
+  C   C36       1.0  0.55417  0.94584  0.55415  1.0000
+  C   C37       1.0  0.38805  0.11194  0.11194  1.0000
+  C   C38       1.0  0.44582  0.05418  0.05417  1.0000
+  C   C39       1.0  0.11193  0.38807  0.38807  1.0000
+  C   C40       1.0  0.05416  0.44584  0.44584  1.0000
+  C   C41       1.0  0.38807  0.11193  0.38807  1.0000
+  C   C42       1.0  0.44584  0.05416  0.44584  1.0000
+  C   C43       1.0  0.11194  0.38805  0.11194  1.0000
+  C   C44       1.0  0.05417  0.44582  0.05418  1.0000
+  C   C45       1.0  0.38806  0.38807  0.11194  1.0000
+  C   C46       1.0  0.44583  0.44583  0.05417  1.0000
+  C   C47       1.0  0.11193  0.11193  0.38806  1.0000
+  C   C48       1.0  0.05417  0.05417  0.44583  1.0000
+  O   O1        1.0  0.75007  0.75002  0.74999  1.0000
+  O   O2        1.0  0.24999  0.24994  0.24997  1.0000
+  O   O3        1.0  0.69689  0.86551  0.86551  1.0000
+  O   O4        1.0  0.57210  0.86551  0.86551  1.0000
+  O   O5        1.0  0.86551  0.57211  0.69687  1.0000
+  O   O6        1.0  0.86550  0.69691  0.57210  1.0000
+  O   O7        1.0  0.86551  0.86551  0.69688  1.0000
+  O   O8        1.0  0.86550  0.86550  0.57211  1.0000
+  O   O9        1.0  0.57209  0.69688  0.86551  1.0000
+  O   O10       1.0  0.69688  0.57210  0.86551  1.0000
+  O   O11       1.0  0.86550  0.69689  0.86550  1.0000
+  O   O12       1.0  0.86550  0.57211  0.86551  1.0000
+  O   O13       1.0  0.69690  0.86550  0.57209  1.0000
+  O   O14       1.0  0.57210  0.86552  0.69686  1.0000
+  O   O15       1.0  0.42789  0.13449  0.13449  1.0000
+  O   O16       1.0  0.30309  0.13451  0.13451  1.0000
+  O   O17       1.0  0.13449  0.42790  0.30312  1.0000
+  O   O18       1.0  0.13449  0.30312  0.42790  1.0000
+  O   O19       1.0  0.42790  0.13450  0.30311  1.0000
+  O   O20       1.0  0.30312  0.13449  0.42789  1.0000
+  O   O21       1.0  0.13451  0.30308  0.13451  1.0000
+  O   O22       1.0  0.13449  0.42788  0.13450  1.0000
+  O   O23       1.0  0.42790  0.30310  0.13450  1.0000
+  O   O24       1.0  0.30312  0.42788  0.13450  1.0000
+  O   O25       1.0  0.13449  0.13449  0.42789  1.0000
+  O   O26       1.0  0.13450  0.13450  0.30309  1.0000
```

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16` & `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/gadgets/my_metrics.py` & `moftransformer-2.0.1/moftransformer/gadgets/my_metrics.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/AtomTypeMap.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/AtomTypeMap.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/AtomTypeMap.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/AtomTypeMap.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Cell.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Cell.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/EnergyGrid.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/UFF_FF.def` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/UFF_FF.def`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/UFF_Type.def` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/UFF_Type.def`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ForceField.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/ForceField.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ForceField.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/ForceField.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Framework.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Framework.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Framework.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Framework.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Gaussian.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Gaussian.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Gaussian.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Gaussian.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridMaker.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridMaker.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridMaker.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridMaker.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayException.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridayException.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayException.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridayException.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayTypes.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridayTypes.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/LennardJones.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/LennardJones.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/LennardJones.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/LennardJones.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/MaterialGrid.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/MaterialGrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/MaterialGrid.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/MaterialGrid.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/NlistMaker.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/NlistMaker.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/NlistMaker.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/NlistMaker.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/PairEnergy.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/PairEnergy.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Random.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Random.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ShiftedLJ.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/ShiftedLJ.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ShiftedLJ.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/ShiftedLJ.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Timer.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Timer.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Vector.hpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Vector.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/Makefile` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/Makefile`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/main_cota.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/main_cota.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/main_visit.cpp` & `moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/main_visit.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/modules/cgcnn.py` & `moftransformer-2.0.1/moftransformer/modules/cgcnn.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/modules/heads.py` & `moftransformer-2.0.1/moftransformer/modules/heads.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/modules/module.py` & `moftransformer-2.0.1/moftransformer/modules/module.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/modules/module_utils.py` & `moftransformer-2.0.1/moftransformer/modules/module_utils.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/modules/objectives.py` & `moftransformer-2.0.1/moftransformer/modules/objectives.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/modules/vision_transformer_3d.py` & `moftransformer-2.0.1/moftransformer/modules/vision_transformer_3d.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/run.py` & `moftransformer-2.0.1/moftransformer/run.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/utils/download.py` & `moftransformer-2.0.1/moftransformer/utils/download.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/utils/install_griday.py` & `moftransformer-2.0.1/moftransformer/utils/install_griday.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/utils/prepare_data.py` & `moftransformer-2.0.1/moftransformer/utils/prepare_data.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/visualize/drawer.py` & `moftransformer-2.0.1/moftransformer/visualize/drawer.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/visualize/setting.py` & `moftransformer-2.0.1/moftransformer/visualize/setting.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/visualize/utils.py` & `moftransformer-2.0.1/moftransformer/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer/visualize/visualizer.py` & `moftransformer-2.0.1/moftransformer/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.0/moftransformer.egg-info/PKG-INFO` & `moftransformer-2.0.1/moftransformer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: moftransformer
-Version: 2.0.0
+Version: 2.0.1
 Summary: moftransformer
 Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer
 Author: Yeonghun Kang, Hyunsoo Park
 Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.0.0-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.0.1-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.0.0-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.0.1-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
  <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
@@ -46,15 +46,15 @@
 
 ### Installation using PIP 
 ```
 $ pip install moftransformer
 ```
 
 ### Download the pretrained models (ckpt file)
-- you can download the pretrained models (`PMTransformer.ckpt` and `MOFTransformer.ckpt`) [figshare](https://figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2)
+- you can download the pretrained models (`PMTransformer.ckpt` and `MOFTransformer.ckpt`) via [figshare](https://figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2)
 
 or you can download with a command line:
 ```
 $ moftransformer download pretrain_model
 ```
 ### (Optional) Download pre-embeddings for CoREMOF, QMOF
 - we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database.
@@ -134,15 +134,15 @@
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/getting_started/assets/3.gif" width="400">
 </p>
 
 ## Universal Transfer Learning
 
-Comparison of mean absolute error (MAE) values for various baseline models, scratch, MOFTransformer, and PMTransformer on different properties of MOFs, COFs, PPNs, and zeolites. The bold values indicate the lowest MAE value for each property. The details of information can be found in [PMTransformer paper]()
+Comparison of mean absolute error (MAE) values for various baseline models, scratch, MOFTransformer, and PMTransformer on different properties of MOFs, COFs, PPNs, and zeolites. The bold values indicate the lowest MAE value for each property. The details of information can be found in [PMTransformer paper](https://chemrxiv.org/engage/chemrxiv/article-details/644a0651df78ec50157390c9)
 
 | Material | Property | Number of Dataset | Energy histogram | Descriptor-based ML | CGCNN | Scratch | MOFTransformer | PMTransformer |
 | --- | --- | --- | --- | --- | --- | --- | --- | --- |
 | MOF | H<sub>2</sub> Uptake (100 bar) | 20,000 | 9.183 | 9.456 | 32.864 | 7.018 | 6.377 | **5.963** |
 | MOF | H<sub>2</sub> diffusivity (dilute) | 20,000 | 0.644 | 0.398 | 0.6600 | 0.391 | 0.367 | 0.**366** |
 | MOF | Band-gap | 20.373 | 0.913 | 0.590 | 0.290 | 0.271 | 0.224 | **0.216** |
 | MOF | N<sub>2</sub> uptake (1 bar) | 5,286 | 0.178 | 0.115 | 0.108 | 0.102 | 0.071 | **0.069** |
@@ -156,7 +156,20 @@
 | COF | CO<sub>2</sub> heat of adsorption | 39,304 | 2.101 | 1.341 | 1.846 | 1.058 | 0.874 | **0.842** |
 | COF | CO<sub>2</sub> log KH | 39,304 | 0.242 | 0.169 | 0.238 | 0.134 | 0.108 | **0.103** |
 | PPN | CH<sub>4</sub> uptake (65bar) | 17,870 | 6.260 | 4.233 | 9.731 | 3.748 | 3.187 | **2.995** | 
 | PPN | CH<sub>4</sub> uptake (1bar) | 17,870  | 1.356	| 0.563	| 1.525	| 0.602	| 0.493	| **0.461** | 
 | Zeolite | CH<sub>4</sub>  KH (unitless) | 99,204	| 8.032	| 6.268	| 6.334	| 4.286	| 4.103	| **3.998** |
 | Zeolite | CH<sub>4</sub>  Heat of adsorption | 99,204	| 1.612	|1.033	| 1.603	| 0.670	| 0.647	|**0.639** |
 
+## Citation
+if you want to cite PMTransformer or MOFTransformer, please refer to the following paper:
+1. A multi-modal pre-training transformer for universal transfer learning in metal–organic frameworks, Nature Machine Intelligence, 5, 2023. [link](https://www.nature.com/articles/s42256-023-00628-2)
+
+2. PMTransformer: Universal Transfer Learning and Cross-material Few-shot Learning in Porous Materials, (submitted). [link](https://chemrxiv.org/engage/chemrxiv/article-details/644a0651df78ec50157390c9)
+
+## Contributing 🙌
+
+Contributions are welcome! If you have any suggestions or find any issues, please open an issue or a pull request.
+
+## License 📄
+
+This project is licensed under the MIT License. See the `LICENSE` file for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moftransformer Version: 2.0.0 Summary:
+Metadata-Version: 2.1 Name: moftransformer Version: 2.0.1 Summary:
 moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
 Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
 docs/source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
@@ -20,15 +20,15 @@
 porous materials as well as MOFs. The `PMTransformer` outperforms the
 `MOFTransformer` in predicting various properties of porous materials. ##
 [Install](https://hspark1212.github.io/MOFTransformer/installation.html) ###
 Depedencies ``` python>=3.8 ``` Given that MOFTransformer is based on pytorch,
 please install pytorch (>= 1.12.0) according to your environments. ###
 Installation using PIP ``` $ pip install moftransformer ``` ### Download the
 pretrained models (ckpt file) - you can download the pretrained models
-(`PMTransformer.ckpt` and `MOFTransformer.ckpt`) [figshare](https://
+(`PMTransformer.ckpt` and `MOFTransformer.ckpt`) via [figshare](https://
 figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2) or
 you can download with a command line: ``` $ moftransformer download
 pretrain_model ``` ### (Optional) Download pre-embeddings for CoREMOF, QMOF -
 we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-
 grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database. ``` $
 moftransformer download coremof $ moftransformer download qmof ``` ## [Getting
 Started](https://hspark1212.github.io/MOFTransformer/tutorial.html) 1. At
@@ -66,15 +66,16 @@
 vis.draw_grid() ```
    [https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/
                      source/getting_started/assets/3.gif]
 ## Universal Transfer Learning Comparison of mean absolute error (MAE) values
 for various baseline models, scratch, MOFTransformer, and PMTransformer on
 different properties of MOFs, COFs, PPNs, and zeolites. The bold values
 indicate the lowest MAE value for each property. The details of information can
-be found in [PMTransformer paper]() | Material | Property | Number of Dataset |
+be found in [PMTransformer paper](https://chemrxiv.org/engage/chemrxiv/article-
+details/644a0651df78ec50157390c9) | Material | Property | Number of Dataset |
 Energy histogram | Descriptor-based ML | CGCNN | Scratch | MOFTransformer |
 PMTransformer | | --- | --- | --- | --- | --- | --- | --- | --- | --- | | MOF |
 H2 Uptake (100 bar) | 20,000 | 9.183 | 9.456 | 32.864 | 7.018 | 6.377 |
 **5.963** | | MOF | H2 diffusivity (dilute) | 20,000 | 0.644 | 0.398 | 0.6600 |
 0.391 | 0.367 | 0.**366** | | MOF | Band-gap | 20.373 | 0.913 | 0.590 | 0.290 |
 0.271 | 0.224 | **0.216** | | MOF | N2 uptake (1 bar) | 5,286 | 0.178 | 0.115 |
 0.108 | 0.102 | 0.071 | **0.069** | | MOF | O2 uptake (1 bar) | 5,286 | 0.162 |
@@ -88,8 +89,18 @@
 (5.8bar) | 39,304 | 3.444 | 1.853 | 5.620 | 1.255 | **0.999** | 1.009 | | COF |
 CO2 heat of adsorption | 39,304 | 2.101 | 1.341 | 1.846 | 1.058 | 0.874 |
 **0.842** | | COF | CO2 log KH | 39,304 | 0.242 | 0.169 | 0.238 | 0.134 | 0.108
 | **0.103** | | PPN | CH4 uptake (65bar) | 17,870 | 6.260 | 4.233 | 9.731 |
 3.748 | 3.187 | **2.995** | | PPN | CH4 uptake (1bar) | 17,870 | 1.356 | 0.563
 | 1.525 | 0.602 | 0.493 | **0.461** | | Zeolite | CH4 KH (unitless) | 99,204 |
 8.032 | 6.268 | 6.334 | 4.286 | 4.103 | **3.998** | | Zeolite | CH4 Heat of
-adsorption | 99,204 | 1.612 |1.033 | 1.603 | 0.670 | 0.647 |**0.639** |
+adsorption | 99,204 | 1.612 |1.033 | 1.603 | 0.670 | 0.647 |**0.639** | ##
+Citation if you want to cite PMTransformer or MOFTransformer, please refer to
+the following paper: 1. A multi-modal pre-training transformer for universal
+transfer learning in metalâorganic frameworks, Nature Machine Intelligence,
+5, 2023. [link](https://www.nature.com/articles/s42256-023-00628-2) 2.
+PMTransformer: Universal Transfer Learning and Cross-material Few-shot Learning
+in Porous Materials, (submitted). [link](https://chemrxiv.org/engage/chemrxiv/
+article-details/644a0651df78ec50157390c9) ## Contributing ð Contributions
+are welcome! If you have any suggestions or find any issues, please open an
+issue or a pull request. ## License ð This project is licensed under the MIT
+License. See the `LICENSE` file for more information.
```

### Comparing `moftransformer-2.0.0/setup.py` & `moftransformer-2.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # MOFTransformer version 2.0.0
 import re
 from setuptools import setup, find_packages
 
-try:
-    import torch
-except ImportError:
-    raise EnvironmentError("Torch must be installed before install moftransformer")
 
 with open("requirements.txt", "r") as f:
     install_requires = f.readlines()
 
 with open("README.md", "r") as f:
     long_description = f.read()
```

