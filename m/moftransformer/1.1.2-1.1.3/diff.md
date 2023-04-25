# Comparing `tmp/moftransformer-1.1.2.tar.gz` & `tmp/moftransformer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moftransformer-1.1.2.tar", last modified: Mon Feb 20 04:39:21 2023, max compression
+gzip compressed data, was "moftransformer-1.1.3.tar", last modified: Tue Apr 25 05:16:40 2023, max compression
```

## Comparing `moftransformer-1.1.2.tar` & `moftransformer-1.1.3.tar`

### file list

```diff
@@ -1,276 +1,284 @@
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.530756 moftransformer-1.1.2/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8017 2023-02-20 04:39:21.530756 moftransformer-1.1.2/PKG-INFO
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7639 2023-02-13 06:36:32.000000 moftransformer-1.1.2/README.md
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.522756 moftransformer-1.1.2/moftransformer/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2022-12-19 09:02:28.000000 moftransformer-1.1.2/moftransformer/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.522756 moftransformer-1.1.2/moftransformer/assets/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       40 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/assets/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12616 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/assets/bbs.json
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9431 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/assets/colors.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12647 2023-01-26 02:06:32.000000 moftransformer-1.1.2/moftransformer/assets/topology.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.522756 moftransformer-1.1.2/moftransformer/cli/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        0 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/cli/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2316 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/cli/download.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      290 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/cli/install_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3117 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/cli/main.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      537 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/cli/run.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      294 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/cli/uninstall_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3558 2023-02-20 04:37:02.000000 moftransformer-1.1.2/moftransformer/config.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9445 2023-02-20 04:37:02.000000 moftransformer-1.1.2/moftransformer/config_ex.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.522756 moftransformer-1.1.2/moftransformer/database/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      430 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/database/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.522756 moftransformer-1.1.2/moftransformer/datamodules/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      176 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/datamodules/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2906 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/datamodules/datamodule.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10048 2022-12-29 08:18:25.000000 moftransformer-1.1.2/moftransformer/datamodules/dataset.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.522756 moftransformer-1.1.2/moftransformer/examples/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      468 2023-01-05 12:04:50.000000 moftransformer-1.1.2/moftransformer/examples/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.522756 moftransformer-1.1.2/moftransformer/examples/dataset/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.522756 moftransformer-1.1.2/moftransformer/examples/dataset/test/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       29 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/test_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.522756 moftransformer-1.1.2/moftransformer/examples/dataset/total/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-01-05 12:09:32.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/acs+N270+E33.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-01-05 12:09:32.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/acs+N270+E33.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:32.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/acs+N270+E33.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:32.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/acs+N270+E33.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-01-05 12:09:28.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-01-05 12:09:28.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:28.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:28.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-01-05 12:09:29.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/fee+N254+E185.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-01-05 12:09:29.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/fee+N254+E185.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/fee+N254+E185.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/fee+N254+E185.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-01-05 12:09:28.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/mok+N109+E146.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-01-05 12:09:28.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/mok+N109+E146.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:28.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/mok+N109+E146.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:28.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/mok+N109+E146.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-01-05 12:09:33.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-01-05 12:09:33.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:33.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:33.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-01-05 12:09:31.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-01-05 12:09:31.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/msp+N624+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:31.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/msp+N624+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:31.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/msp+N624+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-01-05 12:09:31.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/sml+N696+E182.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-01-05 12:09:31.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/sml+N696+E182.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:31.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/sml+N696+E182.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:31.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/sml+N696+E182.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-01-05 12:09:29.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/smm+N577+E166.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-01-05 12:09:29.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/smm+N577+E166.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/smm+N577+E166.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/smm+N577+E166.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-01-05 12:09:29.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-01-05 12:09:29.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-01-05 12:09:30.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/vna+N650+E120.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-01-05 12:09:30.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/vna+N650+E120.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:30.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/vna+N650+E120.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:30.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/vna+N650+E120.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-01-05 12:09:33.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-01-05 12:09:33.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:33.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:33.000000 moftransformer-1.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.526756 moftransformer-1.1.2/moftransformer/examples/dataset/train/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/fee+N254+E185.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/fee+N254+E185.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/fee+N254+E185.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/fee+N254+E185.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/mok+N109+E146.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/mok+N109+E146.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/mok+N109+E146.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/mok+N109+E146.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/msp+N624+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/msp+N624+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/msp+N624+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/sml+N696+E182.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/sml+N696+E182.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/sml+N696+E182.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/sml+N696+E182.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/vna+N650+E120.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/vna+N650+E120.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/vna+N650+E120.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/vna+N650+E120.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      206 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/train_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.526756 moftransformer-1.1.2/moftransformer/examples/dataset/val/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/val/acs+N270+E33.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/val/acs+N270+E33.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/val/acs+N270+E33.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/val/acs+N270+E33.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/val/smm+N577+E166.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/val/smm+N577+E166.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/val/smm+N577+E166.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/val/smm+N577+E166.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       43 2023-01-05 12:09:34.000000 moftransformer-1.1.2/moftransformer/examples/dataset/val_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.526756 moftransformer-1.1.2/moftransformer/examples/raw/
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7496 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/acs+N270+E33.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    17441 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9738 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/fee+N254+E185.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11392 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/mok+N109+E146.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    30404 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18345 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/raw_example.json
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11939 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/sml+N696+E182.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    24953 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/smm+N577+E166.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    28256 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/ukg+N387+E203.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    39904 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/vmk+N489+E8.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18930 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/vna+N650+E120.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    48803 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/raw/zzz+N96+N373+E34.cif
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.522756 moftransformer-1.1.2/moftransformer/examples/visualize/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.526756 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.526756 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9162 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12083 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6405 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8339 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7074 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9292 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    98728 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6419 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8357 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    93472 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6410 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8347 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6845 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8961 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   170530 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      164 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.526756 moftransformer-1.1.2/moftransformer/gadgets/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       45 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/gadgets/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1774 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/gadgets/my_metrics.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.522756 moftransformer-1.1.2/moftransformer/libs/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.530756 moftransformer-1.1.2/moftransformer/libs/GRIDAY/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2799 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/AtomTypeMap.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      654 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/AtomTypeMap.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    41808 2022-12-19 08:32:53.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/AtomTypeMap.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2448 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/Cell.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7789 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      414 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    33448 2022-12-19 08:32:54.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/ChannelAnalyzer.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54588 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/EnergyGrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18619 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3812 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/EnergyGrid.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   143440 2022-12-19 08:32:55.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/EnergyGrid.o
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.530756 moftransformer-1.1.2/moftransformer/libs/GRIDAY/FF/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4751 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/FF/UFF_FF.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      845 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/FF/UFF_Type.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      202 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      190 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      318 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       26 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7197 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/ForceField.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      866 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/ForceField.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    67552 2022-12-19 08:32:55.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/ForceField.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13991 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      865 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    57152 2022-12-19 08:32:56.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/FourierAnalyzer.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7362 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/Framework.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1197 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/Framework.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    47328 2022-12-19 08:32:57.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/Framework.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3007 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/Gaussian.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/Gaussian.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15032 2022-12-19 08:32:57.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/Gaussian.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9534 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridMaker.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      936 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridMaker.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    80288 2022-12-19 08:32:58.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridMaker.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/Griday.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      948 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridayException.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      669 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridayException.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15752 2022-12-19 08:32:58.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridayException.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      567 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridayTypes.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4380 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/LennardJones.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/LennardJones.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    14896 2022-12-19 08:32:58.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/LennardJones.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      334 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/Makefile
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    21824 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/MaterialGrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2366 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/MaterialGrid.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    75600 2022-12-19 08:32:59.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/MaterialGrid.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5664 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/NlistMaker.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      922 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/NlistMaker.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    65096 2022-12-19 08:32:59.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/NlistMaker.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      730 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/PairEnergy.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      570 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/Random.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5106 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/ShiftedLJ.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      764 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/ShiftedLJ.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15360 2022-12-19 08:33:00.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/ShiftedLJ.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      811 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/Timer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2277 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/Vector.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   698550 2022-12-19 08:33:00.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/libgriday.a
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.530756 moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      563 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/Makefile
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5834 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2022-12-19 08:33:06.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/grid2COTA
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   278928 2022-12-19 08:33:05.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/grid2props
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2022-12-19 08:33:04.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/grid2visit
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   161656 2022-12-19 08:33:03.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/grid_gen
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1046 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/main_cota.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1742 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      900 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/main_visit.cpp
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.530756 moftransformer-1.1.2/moftransformer/modules/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       90 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/modules/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5607 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/modules/cgcnn.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3217 2023-01-26 02:06:32.000000 moftransformer-1.1.2/moftransformer/modules/heads.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11253 2023-02-20 04:37:02.000000 moftransformer-1.1.2/moftransformer/modules/module.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7329 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/modules/module_utils.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7935 2023-02-20 04:37:02.000000 moftransformer-1.1.2/moftransformer/modules/objectives.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12841 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/modules/vision_transformer_3d.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10020 2023-02-13 06:36:32.000000 moftransformer-1.1.2/moftransformer/run.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.530756 moftransformer-1.1.2/moftransformer/utils/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      210 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/utils/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5316 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/utils/download.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3705 2023-02-13 06:37:39.000000 moftransformer-1.1.2/moftransformer/utils/install_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15554 2022-12-29 08:18:25.000000 moftransformer-1.1.2/moftransformer/utils/prepare_data.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2449 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/utils/validation.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.530756 moftransformer-1.1.2/moftransformer/visualize/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       98 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/visualize/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3887 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/visualize/drawer.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3628 2022-12-19 08:03:14.000000 moftransformer-1.1.2/moftransformer/visualize/setting.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8775 2023-01-05 12:55:58.000000 moftransformer-1.1.2/moftransformer/visualize/utils.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26335 2023-01-05 12:56:09.000000 moftransformer-1.1.2/moftransformer/visualize/visualizer.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-02-20 04:39:21.522756 moftransformer-1.1.2/moftransformer.egg-info/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8017 2023-02-20 04:39:21.000000 moftransformer-1.1.2/moftransformer.egg-info/PKG-INFO
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12773 2023-02-20 04:39:21.000000 moftransformer-1.1.2/moftransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        1 2023-02-20 04:39:21.000000 moftransformer-1.1.2/moftransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       64 2023-02-20 04:39:21.000000 moftransformer-1.1.2/moftransformer.egg-info/entry_points.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      288 2023-02-20 04:39:21.000000 moftransformer-1.1.2/moftransformer.egg-info/requires.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       15 2023-02-20 04:39:21.000000 moftransformer-1.1.2/moftransformer.egg-info/top_level.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       38 2023-02-20 04:39:21.530756 moftransformer-1.1.2/setup.cfg
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1548 2022-12-19 08:03:14.000000 moftransformer-1.1.2/setup.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.306906 moftransformer-1.1.3/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8389 2023-04-25 05:16:40.306906 moftransformer-1.1.3/PKG-INFO
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8011 2023-04-25 05:00:17.000000 moftransformer-1.1.3/README.md
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.262907 moftransformer-1.1.3/moftransformer/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2023-04-25 05:05:10.000000 moftransformer-1.1.3/moftransformer/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.262907 moftransformer-1.1.3/moftransformer/assets/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       40 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/assets/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12616 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/assets/bbs.json
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9431 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/assets/colors.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12647 2023-01-26 02:06:32.000000 moftransformer-1.1.3/moftransformer/assets/topology.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.266907 moftransformer-1.1.3/moftransformer/cli/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        0 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/cli/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2316 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/cli/download.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      290 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/cli/install_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3117 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/cli/main.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      537 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/cli/run.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      294 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/cli/uninstall_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3929 2023-04-25 05:00:17.000000 moftransformer-1.1.3/moftransformer/config.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10275 2023-04-25 04:35:31.000000 moftransformer-1.1.3/moftransformer/config_ex.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.266907 moftransformer-1.1.3/moftransformer/database/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      430 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/database/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.266907 moftransformer-1.1.3/moftransformer/datamodules/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      176 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/datamodules/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2906 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/datamodules/datamodule.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10145 2023-04-25 04:35:31.000000 moftransformer-1.1.3/moftransformer/datamodules/dataset.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.266907 moftransformer-1.1.3/moftransformer/examples/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      468 2023-01-05 12:04:50.000000 moftransformer-1.1.3/moftransformer/examples/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.266907 moftransformer-1.1.3/moftransformer/examples/dataset/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.266907 moftransformer-1.1.3/moftransformer/examples/dataset/test/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       73 2023-04-04 13:24:22.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.278907 moftransformer-1.1.3/moftransformer/examples/dataset/total/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-01-05 12:09:32.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-01-05 12:09:32.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:32.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:32.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-01-05 12:09:30.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-01-05 12:09:30.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:30.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:30.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.286907 moftransformer-1.1.3/moftransformer/examples/dataset/train/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      206 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.286907 moftransformer-1.1.3/moftransformer/examples/dataset/val/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/acs+N270+E33.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/acs+N270+E33.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/acs+N270+E33.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/acs+N270+E33.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/smm+N577+E166.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/smm+N577+E166.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/smm+N577+E166.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/smm+N577+E166.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       43 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.286907 moftransformer-1.1.3/moftransformer/examples/raw/
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7496 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/acs+N270+E33.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    17441 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9738 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/fee+N254+E185.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11392 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/mok+N109+E146.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    30404 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18345 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/raw_example.json
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11939 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/sml+N696+E182.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    24953 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/smm+N577+E166.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    28256 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/ukg+N387+E203.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    39904 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/vmk+N489+E8.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18930 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/vna+N650+E120.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    48803 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/zzz+N96+N373+E34.cif
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.262907 moftransformer-1.1.3/moftransformer/examples/visualize/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.286907 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.290907 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9162 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12083 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6405 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8339 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7074 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9292 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    98728 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6419 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8357 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    93472 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6410 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8347 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6845 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8961 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   170530 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      164 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.294906 moftransformer-1.1.3/moftransformer/gadgets/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       45 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/gadgets/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1774 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/gadgets/my_metrics.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.262907 moftransformer-1.1.3/moftransformer/libs/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.298906 moftransformer-1.1.3/moftransformer/libs/GRIDAY/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2799 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/AtomTypeMap.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      654 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/AtomTypeMap.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    41808 2022-12-19 08:32:53.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/AtomTypeMap.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2448 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Cell.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7789 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      414 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    33448 2022-12-19 08:32:54.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ChannelAnalyzer.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54588 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18619 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3812 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   143440 2022-12-19 08:32:55.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.o
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.302906 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4751 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/UFF_FF.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      845 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/UFF_Type.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      202 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      190 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      318 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       26 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7197 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ForceField.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      866 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ForceField.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    67552 2022-12-19 08:32:55.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ForceField.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13991 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      865 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    57152 2022-12-19 08:32:56.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FourierAnalyzer.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7362 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Framework.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1197 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Framework.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    47328 2022-12-19 08:32:57.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Framework.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3007 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Gaussian.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Gaussian.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15032 2022-12-19 08:32:57.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Gaussian.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9534 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridMaker.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      936 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridMaker.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    80288 2022-12-19 08:32:58.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridMaker.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Griday.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      948 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayException.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      669 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayException.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15752 2022-12-19 08:32:58.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayException.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      567 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayTypes.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4380 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/LennardJones.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/LennardJones.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    14896 2022-12-19 08:32:58.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/LennardJones.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      334 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Makefile
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    21824 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/MaterialGrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2366 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/MaterialGrid.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    75600 2022-12-19 08:32:59.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/MaterialGrid.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5664 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/NlistMaker.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      922 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/NlistMaker.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    65096 2022-12-19 08:32:59.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/NlistMaker.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      730 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/PairEnergy.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      570 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Random.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5106 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ShiftedLJ.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      764 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ShiftedLJ.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15360 2022-12-19 08:33:00.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ShiftedLJ.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      811 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Timer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2277 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Vector.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   698550 2022-12-19 08:33:00.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/libgriday.a
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.302906 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      563 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/Makefile
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5834 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2022-12-19 08:33:06.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid2COTA
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   278928 2022-12-19 08:33:05.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid2props
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2022-12-19 08:33:04.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid2visit
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   161656 2022-12-19 08:33:03.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid_gen
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1046 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/main_cota.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1742 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      900 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/main_visit.cpp
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.306906 moftransformer-1.1.3/moftransformer/modules/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       90 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/modules/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5607 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/modules/cgcnn.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3217 2023-01-26 02:06:32.000000 moftransformer-1.1.3/moftransformer/modules/heads.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11246 2023-04-25 05:00:17.000000 moftransformer-1.1.3/moftransformer/modules/module.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7329 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/modules/module_utils.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7934 2023-04-25 04:35:31.000000 moftransformer-1.1.3/moftransformer/modules/objectives.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12841 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/modules/vision_transformer_3d.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11715 2023-04-07 05:19:12.000000 moftransformer-1.1.3/moftransformer/run.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.306906 moftransformer-1.1.3/moftransformer/utils/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      210 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/utils/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5316 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/utils/download.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3705 2023-02-13 06:37:39.000000 moftransformer-1.1.3/moftransformer/utils/install_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15554 2023-04-25 04:35:31.000000 moftransformer-1.1.3/moftransformer/utils/prepare_data.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2449 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/utils/validation.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.306906 moftransformer-1.1.3/moftransformer/visualize/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       98 2023-03-09 07:32:31.000000 moftransformer-1.1.3/moftransformer/visualize/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3887 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/visualize/drawer.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3628 2023-03-09 07:32:31.000000 moftransformer-1.1.3/moftransformer/visualize/setting.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9107 2023-04-10 08:03:54.000000 moftransformer-1.1.3/moftransformer/visualize/utils.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26335 2023-03-09 07:32:31.000000 moftransformer-1.1.3/moftransformer/visualize/visualizer.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.262907 moftransformer-1.1.3/moftransformer.egg-info/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8389 2023-04-25 05:16:40.000000 moftransformer-1.1.3/moftransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13237 2023-04-25 05:16:40.000000 moftransformer-1.1.3/moftransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        1 2023-04-25 05:16:40.000000 moftransformer-1.1.3/moftransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       64 2023-04-25 05:16:40.000000 moftransformer-1.1.3/moftransformer.egg-info/entry_points.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      321 2023-04-25 05:16:40.000000 moftransformer-1.1.3/moftransformer.egg-info/requires.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       15 2023-04-25 05:16:40.000000 moftransformer-1.1.3/moftransformer.egg-info/top_level.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       38 2023-04-25 05:16:40.306906 moftransformer-1.1.3/setup.cfg
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1548 2022-12-19 08:03:14.000000 moftransformer-1.1.3/setup.py
```

### Comparing `moftransformer-1.1.2/PKG-INFO` & `moftransformer-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,20 @@
-Metadata-Version: 2.1
-Name: moftransformer
-Version: 1.1.2
-Summary: moftransformer
-Home-page: https://hspark1212.github.io/MOFTransformer/
-Download-URL: https://github.com/hspark1212/MOFTransformer
-Author: Yeonghun Kang, Hyunsoo Park
-Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v1.1.2-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v1.1.3-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v1.1.2-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v1.1.3-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
- <a href="https://chemrxiv.org/engage/chemrxiv/article-details/634fbf8a4a18764f58e9fda5">
+ <a href="https://doi.org/10.1038/s42256-023-00628-2">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
  <a href="https://pypi.org/project/moftransformer/">
      <img alt="Lincense" src="https://img.shields.io/badge/License-MIT-lightgrey.svg?style=plastic">
  </a>
 </p>
 
@@ -183,7 +171,12 @@
 |CO<sub>2</sub> Henry coefficient         | MAE : 0.30     | MAE : 0.42     | 8,183          | CoRE MOF         | 2         |
 |Solvent removal stability classification | ACC : 0.76     | ACC : 0.76     | 2,148          | Text-mining data | 3         |
 |Thermal stability regression             | R2 : 0.44      | R2 : 0.46      | 3,098          | Text-mining data | 3         |
 ### Reference
 1. [Prediction of O2/N2 Selectivity in Metal−Organic Frameworks via High-Throughput Computational Screening and Machine Learning](https://pubs.acs.org/doi/abs/10.1021/acsami.1c18521)
 2. [Understanding the diversity of the metal-organic framework ecosystem](https://www.nature.com/articles/s41467-020-17755-8)
 3. [Using Machine Learning and Data Mining to Leverage Community Knowledge for the Engineering of Stable Metal–Organic Frameworks](https://pubs.acs.org/doi/10.1021/jacs.1c07217)
+
+## Citation
+If you want to cite the MOFTransformer and the pre-training and fine-tuning dataset, please refer to the publication:
+
+Y. Kang, H. Park, B. Smit, J. Kim. "A multi-modal pre-training transformer for universal transfer learning in metal–organic frameworks", *Nature Machine Intelligence*, **(2023)** DOI: [https://doi.org/10.1038/s42256-023-00628-2](https://doi.org/10.1038/s42256-023-00628-2)
```

#### html2text {}

```diff
@@ -1,14 +1,9 @@
-Metadata-Version: 2.1 Name: moftransformer Version: 1.1.2 Summary:
-moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
-Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
-Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
-docs/source/assets/fig1.jpg)
+![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/
+source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
 # [MOFTransformer](https://hspark1212.github.io/MOFTransformer/index.html) This
 package provides universal transfer learing for metal-organic frameworks(MOFs)
 to construct structure-property relationships. `MOFTransformer` obtains state-
 of-the-art performance to predict accross various properties that include gas
 adsorption, diffusion, electronic properties regardless of gas types. Beyond
 its universal transfer learning capabilityies, it provides feature importance
@@ -83,8 +78,13 @@
 0.46 | 3,098 | Text-mining data | 3 | ### Reference 1. [Prediction of O2/N2
 Selectivity in MetalâOrganic Frameworks via High-Throughput Computational
 Screening and Machine Learning](https://pubs.acs.org/doi/abs/10.1021/
 acsami.1c18521) 2. [Understanding the diversity of the metal-organic framework
 ecosystem](https://www.nature.com/articles/s41467-020-17755-8) 3. [Using
 Machine Learning and Data Mining to Leverage Community Knowledge for the
 Engineering of Stable MetalâOrganic Frameworks](https://pubs.acs.org/doi/
-10.1021/jacs.1c07217)
+10.1021/jacs.1c07217) ## Citation If you want to cite the MOFTransformer and
+the pre-training and fine-tuning dataset, please refer to the publication: Y.
+Kang, H. Park, B. Smit, J. Kim. "A multi-modal pre-training transformer for
+universal transfer learning in metalâorganic frameworks", *Nature Machine
+Intelligence*, **(2023)** DOI: [https://doi.org/10.1038/s42256-023-00628-2]
+(https://doi.org/10.1038/s42256-023-00628-2)
```

### Comparing `moftransformer-1.1.2/README.md` & `moftransformer-1.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,32 @@
+Metadata-Version: 2.1
+Name: moftransformer
+Version: 1.1.3
+Summary: moftransformer
+Home-page: https://hspark1212.github.io/MOFTransformer/
+Download-URL: https://github.com/hspark1212/MOFTransformer
+Author: Yeonghun Kang, Hyunsoo Park
+Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v1.1.2-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v1.1.3-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v1.1.2-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v1.1.3-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
- <a href="https://chemrxiv.org/engage/chemrxiv/article-details/634fbf8a4a18764f58e9fda5">
+ <a href="https://doi.org/10.1038/s42256-023-00628-2">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
  <a href="https://pypi.org/project/moftransformer/">
      <img alt="Lincense" src="https://img.shields.io/badge/License-MIT-lightgrey.svg?style=plastic">
  </a>
 </p>
 
@@ -171,7 +183,12 @@
 |CO<sub>2</sub> Henry coefficient         | MAE : 0.30     | MAE : 0.42     | 8,183          | CoRE MOF         | 2         |
 |Solvent removal stability classification | ACC : 0.76     | ACC : 0.76     | 2,148          | Text-mining data | 3         |
 |Thermal stability regression             | R2 : 0.44      | R2 : 0.46      | 3,098          | Text-mining data | 3         |
 ### Reference
 1. [Prediction of O2/N2 Selectivity in Metal−Organic Frameworks via High-Throughput Computational Screening and Machine Learning](https://pubs.acs.org/doi/abs/10.1021/acsami.1c18521)
 2. [Understanding the diversity of the metal-organic framework ecosystem](https://www.nature.com/articles/s41467-020-17755-8)
 3. [Using Machine Learning and Data Mining to Leverage Community Knowledge for the Engineering of Stable Metal–Organic Frameworks](https://pubs.acs.org/doi/10.1021/jacs.1c07217)
+
+## Citation
+If you want to cite the MOFTransformer and the pre-training and fine-tuning dataset, please refer to the publication:
+
+Y. Kang, H. Park, B. Smit, J. Kim. "A multi-modal pre-training transformer for universal transfer learning in metal–organic frameworks", *Nature Machine Intelligence*, **(2023)** DOI: [https://doi.org/10.1038/s42256-023-00628-2](https://doi.org/10.1038/s42256-023-00628-2)
```

#### html2text {}

```diff
@@ -1,9 +1,14 @@
-![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/
-source/assets/fig1.jpg)
+Metadata-Version: 2.1 Name: moftransformer Version: 1.1.3 Summary:
+moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
+Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
+Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
+docs/source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
 # [MOFTransformer](https://hspark1212.github.io/MOFTransformer/index.html) This
 package provides universal transfer learing for metal-organic frameworks(MOFs)
 to construct structure-property relationships. `MOFTransformer` obtains state-
 of-the-art performance to predict accross various properties that include gas
 adsorption, diffusion, electronic properties regardless of gas types. Beyond
 its universal transfer learning capabilityies, it provides feature importance
@@ -78,8 +83,13 @@
 0.46 | 3,098 | Text-mining data | 3 | ### Reference 1. [Prediction of O2/N2
 Selectivity in MetalâOrganic Frameworks via High-Throughput Computational
 Screening and Machine Learning](https://pubs.acs.org/doi/abs/10.1021/
 acsami.1c18521) 2. [Understanding the diversity of the metal-organic framework
 ecosystem](https://www.nature.com/articles/s41467-020-17755-8) 3. [Using
 Machine Learning and Data Mining to Leverage Community Knowledge for the
 Engineering of Stable MetalâOrganic Frameworks](https://pubs.acs.org/doi/
-10.1021/jacs.1c07217)
+10.1021/jacs.1c07217) ## Citation If you want to cite the MOFTransformer and
+the pre-training and fine-tuning dataset, please refer to the publication: Y.
+Kang, H. Park, B. Smit, J. Kim. "A multi-modal pre-training transformer for
+universal transfer learning in metalâorganic frameworks", *Nature Machine
+Intelligence*, **(2023)** DOI: [https://doi.org/10.1038/s42256-023-00628-2]
+(https://doi.org/10.1038/s42256-023-00628-2)
```

### Comparing `moftransformer-1.1.2/moftransformer/assets/bbs.json` & `moftransformer-1.1.3/moftransformer/assets/bbs.json`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/assets/colors.py` & `moftransformer-1.1.3/moftransformer/assets/colors.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/assets/topology.json` & `moftransformer-1.1.3/moftransformer/assets/topology.json`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/cli/download.py` & `moftransformer-1.1.3/moftransformer/cli/download.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/cli/main.py` & `moftransformer-1.1.3/moftransformer/cli/main.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/cli/run.py` & `moftransformer-1.1.3/moftransformer/cli/run.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/config.py` & `moftransformer-1.1.3/moftransformer/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,32 +103,54 @@
     # visualize
     visualize = False  # return attention map
 
 
 @ex.named_config
 def example():
     exp_name = "example"
-    root_dataset = "moftransformer/examples/dataset"
+    root_dataset = "examples/dataset"
     downstream = "example"
     max_epochs = 20
     batch_size = 32
 
 
 @ex.named_config
 def test():
-    exp_name = "example"
+    exp_name = "test"
     loss_names = _loss_names({"regression": 0})
-    root_dataset = "moftransformer/examples/dataset"
-    downstream = "example"
+    root_dataset = "examples/dataset"
+    downstream = ""
     max_epochs = 20
     batch_size = 32
 
 
 @ex.named_config
 def total_h2_uptake():
     exp_name = "total_h2_uptake"
     # root_dataset = ##
     downstream = "h2_uptake"
     max_epochs = 20
     batch_size = 32
     mean = 423.251
     std = 136.293
+
+
+@ex.named_config
+def total_h2_wc():
+    exp_name = "total_h2_wc"
+    # root_dataset = ##
+    downstream = "h2_wc"
+    max_epochs = 20
+    batch_size = 32
+    mean = 241.300
+    std = 152.052
+
+
+@ex.named_config
+def qmof_bandgap():
+    exp_name = "qmof_bandgap"
+    # root_dataset = ##
+    downstream = "qmof_bandgap"
+    max_epochs = 20
+    batch_size = 32
+    mean = 2.086
+    std = 1.131
```

### Comparing `moftransformer-1.1.2/moftransformer/config_ex.py` & `moftransformer-1.1.3/moftransformer/config_ex.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,36 +380,80 @@
     # root_dataset = ##
     downstream = "h2_uptake"
     max_epochs = 20
     batch_size = 32
     mean = 259.878
     std = 112.928
 
+"""
+downstream example (H2 working capacity)
+"""
 @ex.named_config
-def total_h2_uptake():
-    exp_name = "total_h2_uptake"
+def mof_h2_wc():
+    exp_name = "mof_h2_wc"
     # root_dataset = ##
-    downstream = "h2_uptake"
+    downstream = "h2_wc"
+    max_epochs = 20
+    batch_size = 32
+    mean = 320.019
+    std = 87.993
+
+@ex.named_config
+def cof_h2_wc():
+    exp_name = "cof_h2_wc"
+    # root_dataset = ##
+    downstream = "h2_wc"
+    max_epochs = 20
+    batch_size = 32
+    mean = 326.740
+    std = 84.470
+
+@ex.named_config
+def ppn_h2_wc():
+    exp_name = "ppn_h2_wc"
+    # root_dataset = ##
+    downstream = "h2_wc"
+    max_epochs = 20
+    batch_size = 32
+    mean = 300.407
+    std = 116.746
+
+@ex.named_config
+def zeo_h2_wc():
+    exp_name = "zeo_h2_wc"
+    # root_dataset = ##
+    downstream = "h2_wc"
+    max_epochs = 20
+    batch_size = 32
+    mean = 28.667
+    std = 25.660
+
+
+@ex.named_config
+def total_h2_wc():
+    exp_name = "total_h2_wc"
+    # root_dataset = ##
+    downstream = "h2_wc"
     max_epochs = 20
     batch_size = 32
-    mean = 423.251
-    std = 136.293
+    mean = 241.300
+    std = 152.052
 
 """
 curated COF few shot
 """
 @ex.named_config
 def ccof_bandgap():
     exp_name = "ccof_bandgap"
     # root_dataset = ##
     downstream = "ccof_bandgap"
     max_epochs = 20
     batch_size = 32
-    mean = 1.587
-    std = 0.507
+    mean = 1.619
+    std = 0.557
 
 
 @ex.named_config
 def qmof_bandgap():
     exp_name = "qmof_bandgap"
     # root_dataset = ##
     downstream = "qmof_bandgap"
```

### Comparing `moftransformer-1.1.2/moftransformer/datamodules/datamodule.py` & `moftransformer-1.1.3/moftransformer/datamodules/datamodule.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/datamodules/dataset.py` & `moftransformer-1.1.3/moftransformer/datamodules/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,17 @@
 
         assert split in {"train", "test", "val"}
         if downstream:
             path_file = os.path.join(data_dir, f"{split}_{downstream}.json")
         else:
             path_file = os.path.join(data_dir, f"{split}.json")
         print(f"read {path_file}...")
-        assert os.path.isfile(path_file), f"{path_file} doesn't exist in {data_dir}"
+
+        if not os.path.isfile(path_file):
+            raise FileNotFoundError(f"{path_file} doesn't exist. Check 'root_dataset' in config")
 
         dict_target = json.load(open(path_file, "r"))
         self.cif_ids, self.targets = zip(*dict_target.items())
 
         self.nbr_fea_len = nbr_fea_len
 
         self.tasks = {}
@@ -218,20 +220,20 @@
         # graph
         batch_atom_num = dict_batch["atom_num"]
         batch_nbr_idx = dict_batch["nbr_idx"]
         batch_nbr_fea = dict_batch["nbr_fea"]
 
         crystal_atom_idx = []
         base_idx = 0
-
-        for bi in range(batch_size):
-            n_i = len(batch_atom_num[bi])
+        for i, nbr_idx in enumerate(batch_nbr_idx):
+            n_i = nbr_idx.shape[0]
             crystal_atom_idx.append(
                 torch.arange(n_i) + base_idx
             )
+            nbr_idx += base_idx
             base_idx += n_i
 
         dict_batch["atom_num"] = torch.cat(batch_atom_num, dim=0)
         dict_batch["nbr_idx"] = torch.cat(batch_nbr_idx, dim=0)
         dict_batch["nbr_fea"] = torch.cat(batch_nbr_fea, dim=0)
         dict_batch["crystal_atom_idx"] = crystal_atom_idx
```

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/acs+N270+E33.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/acs+N270+E33.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/acs+N270+E33.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/fee+N254+E185.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/fee+N254+E185.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/fee+N254+E185.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/mok+N109+E146.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/mok+N109+E146.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/mok+N109+E146.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/msp+N624+E8.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/msp+N624+E8.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/msp+N624+E8.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/sml+N696+E182.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/sml+N696+E182.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/sml+N696+E182.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/smm+N577+E166.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/smm+N577+E166.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/smm+N577+E166.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/vna+N650+E120.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/vna+N650+E120.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/vna+N650+E120.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/fee+N254+E185.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/fee+N254+E185.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/fee+N254+E185.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/mok+N109+E146.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/mok+N109+E146.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/mok+N109+E146.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/msp+N624+E8.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/msp+N624+E8.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/msp+N624+E8.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/sml+N696+E182.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/sml+N696+E182.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/sml+N696+E182.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/vna+N650+E120.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/vna+N650+E120.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/vna+N650+E120.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/val/acs+N270+E33.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/val/acs+N270+E33.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/val/acs+N270+E33.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/val/smm+N577+E166.cif` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/val/smm+N577+E166.graphdata` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/dataset/val/smm+N577+E166.griddata16` & `moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/raw/acs+N270+E33.cif` & `moftransformer-1.1.3/moftransformer/examples/raw/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif` & `moftransformer-1.1.3/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/raw/fee+N254+E185.cif` & `moftransformer-1.1.3/moftransformer/examples/raw/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/raw/mok+N109+E146.cif` & `moftransformer-1.1.3/moftransformer/examples/raw/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif` & `moftransformer-1.1.3/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/raw/msp+N624+E8.cif` & `moftransformer-1.1.3/moftransformer/examples/raw/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/raw/sml+N696+E182.cif` & `moftransformer-1.1.3/moftransformer/examples/raw/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/raw/smm+N577+E166.cif` & `moftransformer-1.1.3/moftransformer/examples/raw/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/raw/ukg+N387+E203.cif` & `moftransformer-1.1.3/moftransformer/examples/raw/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/raw/vmk+N489+E8.cif` & `moftransformer-1.1.3/moftransformer/examples/raw/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/raw/vna+N650+E120.cif` & `moftransformer-1.1.3/moftransformer/examples/raw/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/raw/zzz+N96+N373+E34.cif` & `moftransformer-1.1.3/moftransformer/examples/raw/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16` & `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/gadgets/my_metrics.py` & `moftransformer-1.1.3/moftransformer/gadgets/my_metrics.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/AtomTypeMap.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/AtomTypeMap.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/AtomTypeMap.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/AtomTypeMap.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/AtomTypeMap.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/AtomTypeMap.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/Cell.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Cell.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/ChannelAnalyzer.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ChannelAnalyzer.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/EnergyGrid.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/EnergyGrid.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/EnergyGrid.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/FF/UFF_FF.def` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/UFF_FF.def`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/FF/UFF_Type.def` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/UFF_Type.def`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/ForceField.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ForceField.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/ForceField.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ForceField.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/ForceField.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ForceField.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/FourierAnalyzer.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/FourierAnalyzer.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/Framework.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Framework.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/Framework.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Framework.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/Framework.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Framework.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/Gaussian.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Gaussian.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/Gaussian.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Gaussian.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/Gaussian.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Gaussian.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridMaker.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridMaker.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridMaker.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridMaker.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridMaker.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridMaker.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridayException.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayException.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridayException.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayException.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridayException.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayException.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/GridayTypes.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayTypes.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/LennardJones.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/LennardJones.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/LennardJones.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/LennardJones.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/LennardJones.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/LennardJones.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/MaterialGrid.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/MaterialGrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/MaterialGrid.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/MaterialGrid.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/MaterialGrid.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/MaterialGrid.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/NlistMaker.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/NlistMaker.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/NlistMaker.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/NlistMaker.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/NlistMaker.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/NlistMaker.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/PairEnergy.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/PairEnergy.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/Random.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Random.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/ShiftedLJ.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ShiftedLJ.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/ShiftedLJ.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ShiftedLJ.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/ShiftedLJ.o` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ShiftedLJ.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/Timer.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Timer.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/Vector.hpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Vector.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/libgriday.a` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/libgriday.a`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/Makefile` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/Makefile`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/grid2COTA` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid2COTA`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/grid2props` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid2props`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/grid2visit` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid2visit`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/grid_gen` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid_gen`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/main_cota.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/main_cota.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/libs/GRIDAY/scripts/main_visit.cpp` & `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/main_visit.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/modules/cgcnn.py` & `moftransformer-1.1.3/moftransformer/modules/cgcnn.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/modules/heads.py` & `moftransformer-1.1.3/moftransformer/modules/heads.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/modules/module.py` & `moftransformer-1.1.3/moftransformer/modules/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from moftransformer.modules import objectives, heads, module_utils
 from moftransformer.modules.cgcnn import GraphEmbeddings
 from moftransformer.modules.vision_transformer_3d import VisionTransformer3D
 
 from moftransformer.modules.module_utils import Normalizer
 
-from torchmetrics.functional import r2_score
+import numpy as np
+from sklearn.metrics import r2_score
 
 
 class Module(LightningModule):
     def __init__(self, config):
         super().__init__()
         self.save_hyperparameters()
 
@@ -265,27 +266,27 @@
 
     def validation_epoch_end(self, outputs):
         module_utils.epoch_wrapup(self)
 
     def test_step(self, batch, batch_idx):
         module_utils.set_task(self)
         output = self(batch)
-        output = {k : (v.cpu() if torch.is_tensor(v) else v ) for k, v in output.items()} # update cpu for memory
+        output = {k : (v.cpu() if torch.is_tensor(v) else v) for k, v in output.items()} # update cpu for memory
         return output
 
     def test_epoch_end(self, outputs):
         module_utils.epoch_wrapup(self)
 
         # calculate r2 score when regression
         if "regression_logits" in outputs[0].keys():
             logits = []
             labels = []
             for out in outputs:
                 logits += out["regression_logits"].tolist()
                 labels += out["regression_labels"].tolist()
 
             if len(logits) > 1:
-                r2 = r2_score(torch.FloatTensor(logits), torch.FloatTensor(labels))
+                r2 = r2_score(np.array(labels), np.array(logits))
                 self.log(f"test/r2_score", r2)
 
     def configure_optimizers(self):
         return module_utils.set_schedule(self)
```

### Comparing `moftransformer-1.1.2/moftransformer/modules/module_utils.py` & `moftransformer-1.1.3/moftransformer/modules/module_utils.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/modules/objectives.py` & `moftransformer-1.1.3/moftransformer/modules/objectives.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     labels = torch.FloatTensor(batch["target"]).to(logits.device)  # [B]
     assert len(labels.shape) == 1
 
     # normalize encode if config["mean"] and config["std], else pass
     labels = normalizer.encode(labels)
     loss = F.mse_loss(logits, labels)
     ret = {
-        "cif_ids": infer["cif_id"],
+        "cif_id": infer["cif_id"],
         "cls_feats": infer["cls_feats"],
         "regression_loss": loss,
         "regression_logits": normalizer.decode(logits),
         "regression_labels": normalizer.decode(labels),
     }
 
     # call update() loss and acc
```

### Comparing `moftransformer-1.1.2/moftransformer/modules/vision_transformer_3d.py` & `moftransformer-1.1.3/moftransformer/modules/vision_transformer_3d.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/run.py` & `moftransformer-1.1.3/moftransformer/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import sys
 import os
 import copy
 import warnings
+from pathlib import Path
+import re
 
 import pytorch_lightning as pl
 
 from moftransformer.config import ex
 from moftransformer.config import config as _config
 from moftransformer.datamodules.datamodule import Datamodule
 from moftransformer.modules.module import Module
+from moftransformer.modules.module_utils import set_task
 from moftransformer.utils.validation import get_valid_config, get_num_devices, ConfigurationError
 
 warnings.filterwarnings(
     "ignore", ".*Trying to infer the `batch_size` from an ambiguous collection.*"
 )
 
 
@@ -187,30 +190,82 @@
     ____________________________________
     resume_from = None
     val_check_interval = 1.0
     dataset_size = False  # experiments for dataset size with 100 [k] or 500 [k]
 
     """
 
-    config = _config()
+    config = copy.deepcopy(_config())
     for key in kwargs.keys():
         if key not in config:
             raise ConfigurationError(f'{key} is not in configuration.')
 
     config.update(kwargs)
     config['root_dataset'] = root_dataset
     config['downstream'] = downstream
     config['log_dir'] = log_dir
     config['test_only'] = test_only
 
     main(config)
 
 
-@ex.automain
-def main(_config):
+def predict(root_dataset, load_path, downstream=None, log_dir='logs/', split='all', **kwargs):
+    config = copy.deepcopy(_config())
+    for key in kwargs.keys():
+        if key not in config:
+            raise ConfigurationError(f'{key} is not in configuration.')
+
+    config.update(kwargs)
+    config['root_dataset'] = root_dataset
+    config['downstream'] = downstream
+    config['log_dir'] = log_dir
+    config['load_path'] = load_path
+    config['test_only'] = True
+    config['visualize'] = True
+
+    pl.seed_everything(config['seed'])
+    model = Module(config)
+    model.eval()
+    dm = Datamodule(config)
+
+    trainer, model, dm = get_trainer(config)
+    save_dir = Path(trainer.logger.log_dir)
+
+    dm.setup()
+    if split == 'all':
+        split = ['train', 'val', 'test']
+    elif isinstance(split, str):
+        split = re.split(r",\s?", split)
+
+    set_task(model)
+    for s in split:
+        if not s in ['train', 'test', 'val']:
+            raise ValueError(f'split must be train, test, or val, not {s}')
+        datamodule = getattr(dm, f'{s}_dataloader')()
+
+        # v1
+        # rets = trainer.predict(model, datamodule)
+
+        # v2
+        #for batch in iter(datamodules):
+        #    ret = model(batch)
+
+
+
+        logtis = []
+        labesl = []
+        for ret in rets:
+            print (ret.keys())
+            #logits.update(ret['regression_logits'])
+            #ret['regression_labels]
+
+
+
+
+def get_trainer(_config):
     _config = copy.deepcopy(_config)
     pl.seed_everything(_config["seed"])
 
     _config = get_valid_config(_config)
     dm = Datamodule(_config)
     model = Module(_config)
     exp_name = f"{_config['exp_name']}"
@@ -268,11 +323,18 @@
         accumulate_grad_batches=accumulate_grad_batches,
         log_every_n_steps=log_every_n_steps,
         resume_from_checkpoint=_config["resume_from"],
         val_check_interval=_config["val_check_interval"],
         deterministic=True,
     )
 
+    return trainer, model, dm
+
+
+@ex.automain
+def main(_config):
+    trainer, model, dm = get_trainer(_config)
+
     if not _config["test_only"]:
         trainer.fit(model, datamodule=dm)
     else:
         trainer.test(model, datamodule=dm)
```

### Comparing `moftransformer-1.1.2/moftransformer/utils/download.py` & `moftransformer-1.1.3/moftransformer/utils/download.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/utils/install_griday.py` & `moftransformer-1.1.3/moftransformer/utils/install_griday.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/utils/prepare_data.py` & `moftransformer-1.1.3/moftransformer/utils/prepare_data.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/utils/validation.py` & `moftransformer-1.1.3/moftransformer/utils/validation.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/visualize/drawer.py` & `moftransformer-1.1.3/moftransformer/visualize/drawer.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/visualize/setting.py` & `moftransformer-1.1.3/moftransformer/visualize/setting.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer/visualize/utils.py` & `moftransformer-1.1.3/moftransformer/visualize/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import copy
 import math
+import ase.io
+from ase.build import make_supercell
 from itertools import product
 from functools import lru_cache
 from pathlib import Path
 from collections.abc import Iterable
 import numpy as np
 
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
@@ -69,56 +71,66 @@
 @lru_cache
 def get_primitive_structure(path_cif, tolerance=2.0):
     st, = CifParser(path_cif, occupancy_tolerance=tolerance).get_structures(primitive=True)
     return st
 
 
 @lru_cache
-def get_structure(path_cif, make_supercell=False, dtype='pymatgen', *,
+def get_structure(path_cif, make_supercell=False, dtype='ase', *,
                   max_length=60, min_length=30):
     """
     get primitive structure from path_cif
     :param path_cif: <str> path for cif file
     :param make_supercell: <bool> if True,
     :param dtype: <str> -> ['ase', 'pymatgen'] return type for structure.
     :param max_length: <int/float> max p_lattice length of structure file (Å)
     :param min_length: <int/float> min p_lattice length of structure file (Å)
     :return: <pymatgen.Structure> structure file from path cif
     """
-    st = get_primitive_structure(path_cif, tolerance=2.0)
+    try:
+        CifParser(path_cif).get_structures()
+    except ValueError as e:   
+        raise ValueError(f'{path_cif} failed : (read pymatgen) {e}')
+
+    atoms = ase.io.read(path_cif)
 
     if make_supercell:
-        st = get_supercell_structure(st, max_length, min_length)
+        atoms = get_supercell_structure(atoms, max_length, min_length)
+    else:
+        atoms = get_supercell_structure(atoms, max_length, 8)
 
-    if type == 'pymatgen':
-        return st
-    elif type != 'ase':
-        return AseAtomsAdaptor().get_atoms(st)
+    if dtype == 'pymatgen':
+        return AseAtomsAdaptor().get_structure(atoms)
+    elif dtype == 'ase':
+        return atoms
     else:
         raise TypeError(f'type must be ase or pymatgen, not {dtype}')
 
 
-def get_supercell_structure(st, max_length=60, min_length=30):
+def get_supercell_structure(atoms, max_length=60, min_length=30):
     """
-    get supercell structure from <pymatgen.Structure>
-    :param st: <pymatgen.Structure> structure file
+    get supercell atoms from <ase.Atoms>
+    :param atoms: <ase.Atoms> object
     :param max_length: <int/float> max p_lattice length of structure file (Å)
     :param min_length: <int/float> min p_lattice length of structure file (Å)
     :return: <ase.Atoms or pymatgen.Structure> structure type.
     """
     scale_abc = []
-    for l in st.lattice.abc:
+    for l in atoms.cell.cellpar()[:3]:
         if l > max_length:
             raise ValueError(f"primitive p_lattice is larger than max_length {max_length}")
         elif l < min_length:
             scale_abc.append(math.ceil(min_length / l))
         else:
             scale_abc.append(1)
-    st.make_supercell(scale_abc)
-    return st
+
+    m = np.zeros([3,3])
+    np.fill_diagonal(m, scale_abc)
+    atoms = make_supercell(atoms, m)
+    return atoms
 
 
 def cuboid_data(position, color=None, num_patches=(6, 6, 6), lattice=None):
     """
     Get cuboid plain data from position and size data
     :param position: <list/tuple> patch positions => [x, y, z]
     :param color: <list/tuple> colors => [r, g, b, w]
```

### Comparing `moftransformer-1.1.2/moftransformer/visualize/visualizer.py` & `moftransformer-1.1.3/moftransformer/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.2/moftransformer.egg-info/PKG-INFO` & `moftransformer-1.1.3/moftransformer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: moftransformer
-Version: 1.1.2
+Version: 1.1.3
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
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v1.1.2-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v1.1.3-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v1.1.2-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v1.1.3-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
- <a href="https://chemrxiv.org/engage/chemrxiv/article-details/634fbf8a4a18764f58e9fda5">
+ <a href="https://doi.org/10.1038/s42256-023-00628-2">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
  <a href="https://pypi.org/project/moftransformer/">
      <img alt="Lincense" src="https://img.shields.io/badge/License-MIT-lightgrey.svg?style=plastic">
  </a>
 </p>
 
@@ -183,7 +183,12 @@
 |CO<sub>2</sub> Henry coefficient         | MAE : 0.30     | MAE : 0.42     | 8,183          | CoRE MOF         | 2         |
 |Solvent removal stability classification | ACC : 0.76     | ACC : 0.76     | 2,148          | Text-mining data | 3         |
 |Thermal stability regression             | R2 : 0.44      | R2 : 0.46      | 3,098          | Text-mining data | 3         |
 ### Reference
 1. [Prediction of O2/N2 Selectivity in Metal−Organic Frameworks via High-Throughput Computational Screening and Machine Learning](https://pubs.acs.org/doi/abs/10.1021/acsami.1c18521)
 2. [Understanding the diversity of the metal-organic framework ecosystem](https://www.nature.com/articles/s41467-020-17755-8)
 3. [Using Machine Learning and Data Mining to Leverage Community Knowledge for the Engineering of Stable Metal–Organic Frameworks](https://pubs.acs.org/doi/10.1021/jacs.1c07217)
+
+## Citation
+If you want to cite the MOFTransformer and the pre-training and fine-tuning dataset, please refer to the publication:
+
+Y. Kang, H. Park, B. Smit, J. Kim. "A multi-modal pre-training transformer for universal transfer learning in metal–organic frameworks", *Nature Machine Intelligence*, **(2023)** DOI: [https://doi.org/10.1038/s42256-023-00628-2](https://doi.org/10.1038/s42256-023-00628-2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moftransformer Version: 1.1.2 Summary:
+Metadata-Version: 2.1 Name: moftransformer Version: 1.1.3 Summary:
 moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
 Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
 docs/source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
@@ -83,8 +83,13 @@
 0.46 | 3,098 | Text-mining data | 3 | ### Reference 1. [Prediction of O2/N2
 Selectivity in MetalâOrganic Frameworks via High-Throughput Computational
 Screening and Machine Learning](https://pubs.acs.org/doi/abs/10.1021/
 acsami.1c18521) 2. [Understanding the diversity of the metal-organic framework
 ecosystem](https://www.nature.com/articles/s41467-020-17755-8) 3. [Using
 Machine Learning and Data Mining to Leverage Community Knowledge for the
 Engineering of Stable MetalâOrganic Frameworks](https://pubs.acs.org/doi/
-10.1021/jacs.1c07217)
+10.1021/jacs.1c07217) ## Citation If you want to cite the MOFTransformer and
+the pre-training and fine-tuning dataset, please refer to the publication: Y.
+Kang, H. Park, B. Smit, J. Kim. "A multi-modal pre-training transformer for
+universal transfer learning in metalâorganic frameworks", *Nature Machine
+Intelligence*, **(2023)** DOI: [https://doi.org/10.1038/s42256-023-00628-2]
+(https://doi.org/10.1038/s42256-023-00628-2)
```

### Comparing `moftransformer-1.1.2/moftransformer.egg-info/SOURCES.txt` & `moftransformer-1.1.3/moftransformer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,26 @@
 moftransformer/datamodules/__init__.py
 moftransformer/datamodules/datamodule.py
 moftransformer/datamodules/dataset.py
 moftransformer/examples/__init__.py
 moftransformer/examples/dataset/test_example.json
 moftransformer/examples/dataset/train_example.json
 moftransformer/examples/dataset/val_example.json
+moftransformer/examples/dataset/test/acs+N270+E33.cif
+moftransformer/examples/dataset/test/acs+N270+E33.graphdata
+moftransformer/examples/dataset/test/acs+N270+E33.grid
+moftransformer/examples/dataset/test/acs+N270+E33.griddata16
 moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif
 moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata
 moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.grid
 moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16
+moftransformer/examples/dataset/test/smm+N577+E166.cif
+moftransformer/examples/dataset/test/smm+N577+E166.graphdata
+moftransformer/examples/dataset/test/smm+N577+E166.grid
+moftransformer/examples/dataset/test/smm+N577+E166.griddata16
 moftransformer/examples/dataset/total/acs+N270+E33.cif
 moftransformer/examples/dataset/total/acs+N270+E33.graphdata
 moftransformer/examples/dataset/total/acs+N270+E33.grid
 moftransformer/examples/dataset/total/acs+N270+E33.griddata16
 moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif
 moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata
 moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.grid
```

### Comparing `moftransformer-1.1.2/setup.py` & `moftransformer-1.1.3/setup.py`

 * *Files identical despite different names*

