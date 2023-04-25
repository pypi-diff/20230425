# Comparing `tmp/tsfpga-8.0.1.tar.gz` & `tmp/tsfpga-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tsfpga-8.0.1.tar", last modified: Thu Jul 15 16:36:03 2021, max compression
+gzip compressed data, was "tsfpga-9.0.0.tar", last modified: Tue Oct 19 08:05:16 2021, max compression
```

## Comparing `tsfpga-8.0.1.tar` & `tsfpga-9.0.0.tar`

### file list

```diff
@@ -1,364 +1,327 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      261 2021-07-15 16:35:49.000000 tsfpga-8.0.1/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      184 2021-07-15 16:35:49.000000 tsfpga-8.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4998 2021-07-15 16:35:49.000000 tsfpga-8.0.1/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     3509 2021-07-15 16:36:03.000000 tsfpga-8.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/doc/readme/
--rw-rw-rw-   0 root         (0) root         (0)     1264 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/readme/badges.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/doc/release_notes/
--rw-rw-rw-   0 root         (0) root         (0)       16 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/0.1.0.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/0.1.1.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/0.1.2.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/0.1.3.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/0.1.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      854 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/1.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)       64 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/1.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)     1647 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/2.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      663 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/3.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)     1527 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/4.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)       46 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/4.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)     3692 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/5.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)     1517 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/6.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)     2121 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/7.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)     2560 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/8.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/8.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)       18 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/release_notes/unreleased.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/doc/sphinx/
--rw-rw-rw-   0 root         (0) root         (0)     4988 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/Python-logo-notext.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/doc/sphinx/api_reference/
--rw-rw-rw-   0 root         (0) root         (0)       67 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/api_reference/tsfpga.registers.rst
--rw-rw-rw-   0 root         (0) root         (0)       57 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/api_reference/tsfpga.rst
--rw-rw-rw-   0 root         (0) root         (0)       64 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/api_reference/tsfpga.vivado.rst
--rw-rw-rw-   0 root         (0) root         (0)     2901 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     3575 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/contributing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/doc/sphinx/files/
--rw-rw-rw-   0 root         (0) root         (0)    30874 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/files/ci_deploy_jobs.png
--rw-rw-rw-   0 root         (0) root         (0)    57884 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/files/ci_deploy_pipelines.png
--rw-rw-rw-   0 root         (0) root         (0)     2795 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/files/formal_sby_example.sby
--rw-rw-rw-   0 root         (0) root         (0)     4047 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/formal.rst
--rw-rw-rw-   0 root         (0) root         (0)     7728 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/fpga_build.rst
--rw-rw-rw-   0 root         (0) root         (0)      462 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       48 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/license_information.rst
--rw-rw-rw-   0 root         (0) root         (0)     6616 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/module_structure.rst
--rw-rw-rw-   0 root         (0) root         (0)     3450 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/netlist_build.rst
--rw-rw-rw-   0 root         (0) root         (0)    15477 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/registers.rst
--rw-rw-rw-   0 root         (0) root         (0)       54 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/release_notes.rst
--rw-rw-rw-   0 root         (0) root         (0)       55 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/robots.txt
--rw-rw-rw-   0 root         (0) root         (0)    10316 2021-07-15 16:35:49.000000 tsfpga-8.0.1/doc/sphinx/simulation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/docker/formal/
--rw-rw-rw-   0 root         (0) root         (0)      453 2021-07-15 16:35:49.000000 tsfpga-8.0.1/docker/formal/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     1140 2021-07-15 16:35:49.000000 tsfpga-8.0.1/docker/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/
--rw-rw-rw-   0 root         (0) root         (0)      351 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6924 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/build.py
--rw-rw-rw-   0 root         (0) root         (0)     3063 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/formal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules/artyz7/
--rw-rw-rw-   0 root         (0) root         (0)     1808 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/artyz7/module_artyz7.py
--rw-rw-rw-   0 root         (0) root         (0)     1789 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/artyz7/regs_artyz7.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules/artyz7/src/
--rw-rw-rw-   0 root         (0) root         (0)    11939 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/artyz7/src/artyz7_top.vhd
--rw-rw-rw-   0 root         (0) root         (0)     1438 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/artyz7/src/artyz7_top_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     5042 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/artyz7/src/block_design_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     6879 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/artyz7/src/block_design_wrapper.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules/artyz7/tcl/
--rw-rw-rw-   0 root         (0) root         (0)     2617 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/artyz7/tcl/artyz7_pinning.tcl
--rw-rw-rw-   0 root         (0) root         (0)    44962 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/artyz7/tcl/block_design.tcl
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules/artyz7/test/
--rw-rw-rw-   0 root         (0) root         (0)     2472 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/artyz7/test/block_design_mock.vhd
--rw-rw-rw-   0 root         (0) root         (0)     6528 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/artyz7/test/tb_artyz7_top.vhd
--rw-rw-rw-   0 root         (0) root         (0)      596 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/artyz7/test/top_level_sim_pkg.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules/ddr_buffer/
--rw-rw-rw-   0 root         (0) root         (0)      837 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/ddr_buffer/module_ddr_buffer.py
--rw-rw-rw-   0 root         (0) root         (0)     1764 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/ddr_buffer/regs_ddr_buffer.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules/ddr_buffer/sim/
--rw-rw-rw-   0 root         (0) root         (0)     2374 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/ddr_buffer/sim/ddr_buffer_sim_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2212 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/ddr_buffer/sim/example_reg_operations_pkg.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules/ddr_buffer/src/
--rw-rw-rw-   0 root         (0) root         (0)     4596 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/ddr_buffer/src/ddr_buffer_top.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules/ddr_buffer/test/
--rw-rw-rw-   0 root         (0) root         (0)     3810 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules/ddr_buffer/test/tb_ddr_buffer.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules_with_ip/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules_with_ip/module_with_ip_cores/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules_with_ip/module_with_ip_cores/ip_cores/
--rw-rw-rw-   0 root         (0) root         (0)      555 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules_with_ip/module_with_ip_cores/ip_cores/fifo_generator_0.tcl
--rw-rw-rw-   0 root         (0) root         (0)      621 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules_with_ip/module_with_ip_cores/ip_cores/mult_u12_u5.tcl
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules_with_ip/module_with_ip_cores/src/
--rw-rw-rw-   0 root         (0) root         (0)      926 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules_with_ip/module_with_ip_cores/src/mult.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/examples/modules_with_ip/module_with_ip_cores/test/
--rw-rw-rw-   0 root         (0) root         (0)     1505 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/modules_with_ip/module_with_ip_cores/test/tb_mult.vhd
--rwxrwxrwx   0 root         (0) root         (0)      813 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/run_formal.sh
--rw-rw-rw-   0 root         (0) root         (0)     8675 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/simulate.py
--rw-rw-rw-   0 root         (0) root         (0)     2079 2021-07-15 16:35:49.000000 tsfpga-8.0.1/examples/tsfpga_example_env.py
--rw-rw-rw-   0 root         (0) root         (0)     1594 2021-07-15 16:35:49.000000 tsfpga-8.0.1/license.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/axi/
--rw-rw-rw-   0 root         (0) root         (0)     4996 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/module_axi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/axi/src/
--rw-rw-rw-   0 root         (0) root         (0)     2578 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_address_fifo.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2500 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_b_fifo.vhd
--rw-rw-rw-   0 root         (0) root         (0)     5622 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_lite_cdc.vhd
--rw-rw-rw-   0 root         (0) root         (0)     9569 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_lite_mux.vhd
--rw-rw-rw-   0 root         (0) root         (0)     6314 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_lite_pipeline.vhd
--rw-rw-rw-   0 root         (0) root         (0)     9437 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_lite_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3522 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_lite_simple_read_crossbar.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3800 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_lite_simple_write_crossbar.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3085 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_lite_to_vec.vhd
--rw-rw-rw-   0 root         (0) root         (0)    20890 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2903 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_r_fifo.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2595 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_read_cdc.vhd
--rw-rw-rw-   0 root         (0) root         (0)     7763 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_read_throttle.vhd
--rw-rw-rw-   0 root         (0) root         (0)     4815 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_simple_read_crossbar.vhd
--rw-rw-rw-   0 root         (0) root         (0)     5129 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_simple_write_crossbar.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2299 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_stream_fifo.vhd
--rw-rw-rw-   0 root         (0) root         (0)     4061 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_stream_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     5193 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_to_axi_lite.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3158 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_to_axi_lite_vec.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2860 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_w_fifo.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3195 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_write_cdc.vhd
--rw-rw-rw-   0 root         (0) root         (0)     7819 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/src/axi_write_throttle.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/axi/test/
--rw-rw-rw-   0 root         (0) root         (0)     8543 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_cdc.vhd
--rw-rw-rw-   0 root         (0) root         (0)     6858 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_fifo.vhd
--rw-rw-rw-   0 root         (0) root         (0)     4533 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_lite_cdc.vhd
--rw-rw-rw-   0 root         (0) root         (0)     8750 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_lite_mux.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3996 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_lite_pipeline.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2550 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_lite_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     5039 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     9486 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_simple_crossbar.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2999 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_stream_fifo.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2185 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_stream_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3911 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_to_axi_lite.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3915 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_to_axi_lite_bus_error.vhd
--rw-rw-rw-   0 root         (0) root         (0)     5256 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/axi/test/tb_axi_to_axi_lite_vec.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/bfm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/bfm/sim/
--rw-rw-rw-   0 root         (0) root         (0)     2340 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/bfm/sim/axi_lite_master.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2255 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/bfm/sim/axi_lite_read_slave.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2406 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/bfm/sim/axi_lite_slave.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2427 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/bfm/sim/axi_lite_write_slave.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2813 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/bfm/sim/axi_master.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2418 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/bfm/sim/axi_read_slave.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2539 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/bfm/sim/axi_slave.vhd
--rw-rw-rw-   0 root         (0) root         (0)     1078 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/bfm/sim/axi_slave_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3463 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/bfm/sim/axi_write_slave.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3761 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/bfm/sim/bfm_pkg.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/common/
--rw-rw-rw-   0 root         (0) root         (0)     9627 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/module_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/common/src/
--rw-rw-rw-   0 root         (0) root         (0)     2148 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/src/addr_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3711 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/src/attribute_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3172 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/src/clock_counter.vhd
--rw-rw-rw-   0 root         (0) root         (0)      692 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/src/common_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2255 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/src/debounce.vhd
--rw-rw-rw-   0 root         (0) root         (0)     7202 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/src/handshake_pipeline.vhd
--rw-rw-rw-   0 root         (0) root         (0)     1227 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/src/handshake_splitter.vhd
--rw-rw-rw-   0 root         (0) root         (0)     7268 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/src/periodic_pulser.vhd
--rw-rw-rw-   0 root         (0) root         (0)     4351 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/src/types_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)    13282 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/src/width_conversion.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/common/test/
--rw-rw-rw-   0 root         (0) root         (0)     2225 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/test/tb_addr_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2846 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/test/tb_clock_counter.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3353 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/test/tb_debounce.vhd
--rw-rw-rw-   0 root         (0) root         (0)     5985 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/test/tb_handshake_pipeline.vhd
--rw-rw-rw-   0 root         (0) root         (0)     5147 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/test/tb_handshake_splitter.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2789 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/test/tb_periodic_pulser.vhd
--rw-rw-rw-   0 root         (0) root         (0)     4153 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/test/tb_types_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     8685 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/common/test/tb_width_conversion.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/fifo/
--rw-rw-rw-   0 root         (0) root         (0)    12080 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/fifo/module_fifo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/fifo/rtl/
--rw-rw-rw-   0 root         (0) root         (0)     1732 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/fifo/rtl/fifo_netlist_build_wrapper.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/fifo/scoped_constraints/
--rw-rw-rw-   0 root         (0) root         (0)     1329 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/fifo/scoped_constraints/asynchronous_fifo.tcl
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/fifo/src/
--rw-rw-rw-   0 root         (0) root         (0)    12225 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/fifo/src/asynchronous_fifo.vhd
--rw-rw-rw-   0 root         (0) root         (0)    11817 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/fifo/src/fifo.vhd
--rw-rw-rw-   0 root         (0) root         (0)     4969 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/fifo/src/fifo_wrapper.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/fifo/test/
--rw-rw-rw-   0 root         (0) root         (0)    15719 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/fifo/test/tb_asynchronous_fifo.vhd
--rw-rw-rw-   0 root         (0) root         (0)    13677 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/fifo/test/tb_fifo.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/math/
--rw-rw-rw-   0 root         (0) root         (0)      874 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/math/module_math.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/math/src/
--rw-rw-rw-   0 root         (0) root         (0)     6015 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/math/src/math_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3422 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/math/src/unsigned_divider.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/math/test/
--rw-rw-rw-   0 root         (0) root         (0)     5441 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/math/test/tb_math_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3255 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/math/test/tb_unsigned_divider.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/reg_file/
--rw-rw-rw-   0 root         (0) root         (0)     2626 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/reg_file/module_reg_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/reg_file/rtl/
--rw-rw-rw-   0 root         (0) root         (0)     2395 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/reg_file/rtl/axi_lite_reg_file_wrapper.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/reg_file/sim/
--rw-rw-rw-   0 root         (0) root         (0)    20525 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/reg_file/sim/reg_operations_pkg.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/reg_file/src/
--rw-rw-rw-   0 root         (0) root         (0)     7314 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/reg_file/src/axi_lite_reg_file.vhd
--rw-rw-rw-   0 root         (0) root         (0)     1261 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/reg_file/src/interrupt_register.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3625 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/reg_file/src/reg_file_pkg.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/reg_file/test/
--rw-rw-rw-   0 root         (0) root         (0)     8356 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/reg_file/test/tb_axi_lite_reg_file.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2909 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/reg_file/test/tb_interrupt_register.vhd
--rw-rw-rw-   0 root         (0) root         (0)     1789 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/reg_file/test/tb_reg_file_pkg.vhd
--rw-rw-rw-   0 root         (0) root         (0)     1997 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/reg_file/test/tb_reg_operations_pkg.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/resync/
--rw-rw-rw-   0 root         (0) root         (0)     4115 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/module_resync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/resync/scoped_constraints/
--rw-rw-rw-   0 root         (0) root         (0)     1899 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/scoped_constraints/resync_counter.tcl
--rw-rw-rw-   0 root         (0) root         (0)     1547 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/scoped_constraints/resync_level.tcl
--rw-rw-rw-   0 root         (0) root         (0)      490 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/scoped_constraints/resync_level_on_signal.tcl
--rw-rw-rw-   0 root         (0) root         (0)     1505 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/scoped_constraints/resync_slv_level_coherent.tcl
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/resync/src/
--rw-rw-rw-   0 root         (0) root         (0)     2674 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/src/resync_counter.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2988 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/src/resync_cycles.vhd
--rw-rw-rw-   0 root         (0) root         (0)     4868 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/src/resync_level.vhd
--rw-rw-rw-   0 root         (0) root         (0)     1697 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/src/resync_level_on_signal.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2879 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/src/resync_pulse.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2163 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/src/resync_slv_level.vhd
--rw-rw-rw-   0 root         (0) root         (0)     4673 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/src/resync_slv_level_coherent.vhd
--rw-rw-rw-   0 root         (0) root         (0)     1914 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/src/resync_slv_level_on_signal.vhd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/modules/resync/test/
--rw-rw-rw-   0 root         (0) root         (0)     2586 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/test/tb_resync_counter.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3478 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/test/tb_resync_cycles.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3058 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/test/tb_resync_pulse.vhd
--rw-rw-rw-   0 root         (0) root         (0)     3744 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/test/tb_resync_slv_level.vhd
--rw-rw-rw-   0 root         (0) root         (0)     2233 2021-07-15 16:35:49.000000 tsfpga-8.0.1/modules/resync/test/tb_resync_slv_level_on_signal.vhd
--rw-rw-rw-   0 root         (0) root         (0)       31 2021-07-15 16:35:49.000000 tsfpga-8.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2649 2021-07-15 16:35:49.000000 tsfpga-8.0.1/readme.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2021-07-15 16:35:49.000000 tsfpga-8.0.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      123 2021-07-15 16:35:49.000000 tsfpga-8.0.1/requirements_develop.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-15 16:36:03.000000 tsfpga-8.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2628 2021-07-15 16:35:49.000000 tsfpga-8.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tools/
--rw-rw-rw-   0 root         (0) root         (0)    10560 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tools/build_docs.py
--rw-rw-rw-   0 root         (0) root         (0)     3529 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tools/release.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/
--rw-rw-rw-   0 root         (0) root         (0)     1016 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1881 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/about.py
--rw-rw-rw-   0 root         (0) root         (0)    19887 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/build_project_list.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/build_step_tcl_hook.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     3307 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/create_vhdl_ls_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8234 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/formal_project.py
--rw-rw-rw-   0 root         (0) root         (0)     7839 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/git_simulation_subset.py
--rw-rw-rw-   0 root         (0) root         (0)     3550 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/git_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/hdl_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/ip_core_file.py
--rw-rw-rw-   0 root         (0) root         (0)    17138 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/module.py
--rw-rw-rw-   0 root         (0) root         (0)     1866 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/module_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/registers/
--rw-rw-rw-   0 root         (0) root         (0)      374 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2443 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/bit.py
--rw-rw-rw-   0 root         (0) root         (0)     3699 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/bit_vector.py
--rw-rw-rw-   0 root         (0) root         (0)      912 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/constant.py
--rw-rw-rw-   0 root         (0) root         (0)     2774 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/html_translator.py
--rw-rw-rw-   0 root         (0) root         (0)    10134 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5682 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/register.py
--rw-rw-rw-   0 root         (0) root         (0)     3320 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/register_array.py
--rw-rw-rw-   0 root         (0) root         (0)     7113 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/register_c_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/register_code_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    10008 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/register_cpp_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     2186 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/register_field.py
--rw-rw-rw-   0 root         (0) root         (0)     8449 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/register_html_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    16975 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/register_list.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/register_python_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     7800 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/register_vhdl_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/registers/test/
--rw-rw-rw-   0 root         (0) root         (0)      351 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3272 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/test_bit.py
--rw-rw-rw-   0 root         (0) root         (0)     4929 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/test_bit_vector.py
--rw-rw-rw-   0 root         (0) root         (0)      944 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/test_constant.py
--rw-rw-rw-   0 root         (0) root         (0)     3794 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/test_html_translator.py
--rw-rw-rw-   0 root         (0) root         (0)    15082 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5423 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/test_register.py
--rw-rw-rw-   0 root         (0) root         (0)     4660 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/test_register_array.py
--rw-rw-rw-   0 root         (0) root         (0)     3429 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/test_register_code_generation.py
--rw-rw-rw-   0 root         (0) root         (0)     7064 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/test_register_html_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    16138 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/test_register_list.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/test_register_python_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     3337 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/registers/test/test_register_vhdl_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/sby_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     3658 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/svn_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3365 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/system_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/test/
--rw-rw-rw-   0 root         (0) root         (0)      432 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      871 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/test/functional/
--rw-rw-rw-   0 root         (0) root         (0)      351 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/functional/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/test/functional/commercial_simulators/
--rw-rw-rw-   0 root         (0) root         (0)      351 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/functional/commercial_simulators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/functional/commercial_simulators/test_compilation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/test/functional/gcc/
--rw-rw-rw-   0 root         (0) root         (0)      351 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/functional/gcc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11355 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/functional/gcc/test_register_compilation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/test/functional/vivado/
--rw-rw-rw-   0 root         (0) root         (0)      351 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/functional/vivado/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9349 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/functional/vivado/test_building_vivado_project.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/test/lint/
--rw-rw-rw-   0 root         (0) root         (0)      351 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/lint/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15081 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/lint/pylintrc
--rw-rw-rw-   0 root         (0) root         (0)    16267 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/lint/pylintrc_original
--rw-rw-rw-   0 root         (0) root         (0)     6290 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/lint/test_copyright.py
--rw-rw-rw-   0 root         (0) root         (0)     5393 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/lint/test_file_format.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/lint/test_python_lint.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/test/unit/
--rw-rw-rw-   0 root         (0) root         (0)      351 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8800 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_build_project_list.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_build_step_tcl_hook.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     3723 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_formal_project.py
--rw-rw-rw-   0 root         (0) root         (0)     4973 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_git_simulation_subset.py
--rw-rw-rw-   0 root         (0) root         (0)     4671 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_git_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_hdl_file.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_ip_core_file.py
--rw-rw-rw-   0 root         (0) root         (0)     8752 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_module.py
--rw-rw-rw-   0 root         (0) root         (0)     2766 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_module_list.py
--rw-rw-rw-   0 root         (0) root         (0)     2369 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_sby_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     2846 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_svn_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2374 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_system_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2128 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/test/unit/test_yosys_project.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/vivado/
--rw-rw-rw-   0 root         (0) root         (0)      351 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3227 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/build_result.py
--rw-rw-rw-   0 root         (0) root         (0)     4333 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/build_result_checker.py
--rw-rw-rw-   0 root         (0) root         (0)     2784 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/common.py
--rw-rw-rw-   0 root         (0) root         (0)     1809 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/hierarchical_utilization_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4446 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/ip_cores.py
--rw-rw-rw-   0 root         (0) root         (0)     1664 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/logic_level_distribution_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    25206 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/project.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/simlib.py
--rw-rw-rw-   0 root         (0) root         (0)     3273 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/simlib_commercial.py
--rw-rw-rw-   0 root         (0) root         (0)     4315 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/simlib_common.py
--rw-rw-rw-   0 root         (0) root         (0)     5190 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/simlib_ghdl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/vivado/tcl/
--rw-rw-rw-   0 root         (0) root         (0)     1557 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/tcl/check_timing.tcl
--rw-rw-rw-   0 root         (0) root         (0)      440 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/tcl/report_logic_level_distribution.tcl
--rw-rw-rw-   0 root         (0) root         (0)      494 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/tcl/report_utilization.tcl
--rw-rw-rw-   0 root         (0) root         (0)     3136 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/tcl/vivado_default_run.tcl
--rw-rw-rw-   0 root         (0) root         (0)     1199 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/tcl/vivado_fast_run.tcl
--rw-rw-rw-   0 root         (0) root         (0)     2320 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/tcl/vivado_messages.tcl
--rw-rw-rw-   0 root         (0) root         (0)    14038 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/tcl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga/vivado/test/
--rw-rw-rw-   0 root         (0) root         (0)      351 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/test/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1933 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/test/test_build_result.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/test/test_build_result_checker.py
--rw-rw-rw-   0 root         (0) root         (0)     1635 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/test/test_common.py
--rw-rw-rw-   0 root         (0) root         (0)     1078 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/test/test_hierarchical_utilization_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     6249 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/test/test_ip_cores.py
--rw-rw-rw-   0 root         (0) root         (0)     2053 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/test/test_logic_level_distribution_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    16765 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/test/test_project.py
--rw-rw-rw-   0 root         (0) root         (0)     5861 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/test/test_simlib.py
--rw-rw-rw-   0 root         (0) root         (0)    11093 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/vivado/test/test_tcl.py
--rw-rw-rw-   0 root         (0) root         (0)     1674 2021-07-15 16:35:49.000000 tsfpga-8.0.1/tsfpga/yosys_project.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3509 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10721 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      158 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2021-07-15 16:36:03.000000 tsfpga-8.0.1/tsfpga.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.188296 tsfpga-9.0.0/
+-rw-r--r--   0 root         (0) root         (0)     3186 2021-10-19 08:05:16.188296 tsfpga-9.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.091289 tsfpga-9.0.0/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.107290 tsfpga-9.0.0/modules/axi/
+-rw-rw-rw-   0 root         (0) root         (0)     4992 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/module_axi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.115291 tsfpga-9.0.0/modules/axi/src/
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_address_fifo.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2500 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_b_fifo.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     5622 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_lite_cdc.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     9569 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_lite_mux.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     6314 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_lite_pipeline.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     9437 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_lite_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3522 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_lite_simple_read_crossbar.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3800 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_lite_simple_write_crossbar.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3085 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_lite_to_vec.vhd
+-rw-rw-rw-   0 root         (0) root         (0)    20890 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2903 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_r_fifo.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_read_cdc.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     7896 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_read_throttle.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     4815 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_simple_read_crossbar.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     5129 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_simple_write_crossbar.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_stream_fifo.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     4061 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_stream_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     5193 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_to_axi_lite.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3158 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_to_axi_lite_vec.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_w_fifo.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3195 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_write_cdc.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     7819 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/src/axi_write_throttle.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.119291 tsfpga-9.0.0/modules/axi/test/
+-rw-rw-rw-   0 root         (0) root         (0)     8543 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_cdc.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     6858 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_fifo.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_lite_cdc.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     8750 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_lite_mux.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3996 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_lite_pipeline.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_lite_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     5039 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     9486 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_simple_crossbar.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2999 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_stream_fifo.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2185 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_stream_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3911 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_to_axi_lite.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3915 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_to_axi_lite_bus_error.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/axi/test/tb_axi_to_axi_lite_vec.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.119291 tsfpga-9.0.0/modules/bfm/
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/module_bfm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.124292 tsfpga-9.0.0/modules/bfm/sim/
+-rw-rw-rw-   0 root         (0) root         (0)     2340 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/axi_lite_master.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2255 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/axi_lite_read_slave.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2406 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/axi_lite_slave.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2427 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/axi_lite_write_slave.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2813 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/axi_master.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2418 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/axi_read_slave.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/axi_slave.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/axi_slave_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     5280 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/axi_stream_master.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     9149 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/axi_stream_slave.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3463 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/axi_write_slave.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     4552 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/bfm_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     4231 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/handshake_master.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     6714 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/sim/handshake_slave.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.125292 tsfpga-9.0.0/modules/bfm/test/
+-rw-rw-rw-   0 root         (0) root         (0)     7370 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/bfm/test/tb_handshake_bfm.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.125292 tsfpga-9.0.0/modules/common/
+-rw-rw-rw-   0 root         (0) root         (0)    13304 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/module_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.126292 tsfpga-9.0.0/modules/common/sim/
+-rw-rw-rw-   0 root         (0) root         (0)     3155 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/sim/axi_stream_protocol_checker.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.130292 tsfpga-9.0.0/modules/common/src/
+-rw-rw-rw-   0 root         (0) root         (0)     2360 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/src/addr_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3711 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/src/attribute_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/src/clock_counter.vhd
+-rw-rw-rw-   0 root         (0) root         (0)      692 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/src/common_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2255 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/src/debounce.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     8243 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/src/handshake_pipeline.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/src/handshake_splitter.vhd
+-rw-rw-rw-   0 root         (0) root         (0)    13450 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/src/keep_remover.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     7279 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/src/periodic_pulser.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     5632 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/src/strobe_on_last.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     4668 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/src/types_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)    19083 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/src/width_conversion.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.133292 tsfpga-9.0.0/modules/common/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/test/tb_addr_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2846 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/test/tb_clock_counter.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3353 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/test/tb_debounce.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     5796 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/test/tb_handshake_pipeline.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     5057 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/test/tb_handshake_splitter.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     9116 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/test/tb_keep_remover.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2789 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/test/tb_periodic_pulser.vhd
+-rw-rw-rw-   0 root         (0) root         (0)    10052 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/test/tb_strobe_on_last.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     4492 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/test/tb_types_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     8025 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/common/test/tb_width_conversion.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.134292 tsfpga-9.0.0/modules/fifo/
+-rw-rw-rw-   0 root         (0) root         (0)    13859 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/fifo/module_fifo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.134292 tsfpga-9.0.0/modules/fifo/rtl/
+-rw-rw-rw-   0 root         (0) root         (0)     1732 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/fifo/rtl/fifo_netlist_build_wrapper.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.135292 tsfpga-9.0.0/modules/fifo/scoped_constraints/
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/fifo/scoped_constraints/asynchronous_fifo.tcl
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.136293 tsfpga-9.0.0/modules/fifo/src/
+-rw-rw-rw-   0 root         (0) root         (0)    12303 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/fifo/src/asynchronous_fifo.vhd
+-rw-rw-rw-   0 root         (0) root         (0)    14648 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/fifo/src/fifo.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/fifo/src/fifo_wrapper.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.136293 tsfpga-9.0.0/modules/fifo/test/
+-rw-rw-rw-   0 root         (0) root         (0)    15719 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/fifo/test/tb_asynchronous_fifo.vhd
+-rw-rw-rw-   0 root         (0) root         (0)    16335 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/fifo/test/tb_fifo.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.137292 tsfpga-9.0.0/modules/math/
+-rw-rw-rw-   0 root         (0) root         (0)      909 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/math/module_math.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.137292 tsfpga-9.0.0/modules/math/src/
+-rw-rw-rw-   0 root         (0) root         (0)     6015 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/math/src/math_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3422 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/math/src/unsigned_divider.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.138293 tsfpga-9.0.0/modules/math/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5441 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/math/test/tb_math_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3255 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/math/test/tb_unsigned_divider.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.139293 tsfpga-9.0.0/modules/reg_file/
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/reg_file/module_reg_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.139293 tsfpga-9.0.0/modules/reg_file/rtl/
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/reg_file/rtl/axi_lite_reg_file_wrapper.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.139293 tsfpga-9.0.0/modules/reg_file/sim/
+-rw-rw-rw-   0 root         (0) root         (0)    20537 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/reg_file/sim/reg_operations_pkg.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.140293 tsfpga-9.0.0/modules/reg_file/src/
+-rw-rw-rw-   0 root         (0) root         (0)     7889 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/reg_file/src/axi_lite_reg_file.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/reg_file/src/interrupt_register.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3625 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/reg_file/src/reg_file_pkg.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.142293 tsfpga-9.0.0/modules/reg_file/test/
+-rw-rw-rw-   0 root         (0) root         (0)     8356 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/reg_file/test/tb_axi_lite_reg_file.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2909 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/reg_file/test/tb_interrupt_register.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/reg_file/test/tb_reg_file_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/reg_file/test/tb_reg_operations_pkg.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.142293 tsfpga-9.0.0/modules/resync/
+-rw-rw-rw-   0 root         (0) root         (0)     4111 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/module_resync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.143293 tsfpga-9.0.0/modules/resync/scoped_constraints/
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/scoped_constraints/resync_counter.tcl
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/scoped_constraints/resync_level.tcl
+-rw-rw-rw-   0 root         (0) root         (0)      490 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/scoped_constraints/resync_level_on_signal.tcl
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/scoped_constraints/resync_slv_level_coherent.tcl
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.146293 tsfpga-9.0.0/modules/resync/src/
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/src/resync_counter.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2988 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/src/resync_cycles.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     4868 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/src/resync_level.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     1697 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/src/resync_level_on_signal.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2879 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/src/resync_pulse.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2163 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/src/resync_slv_level.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     4673 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/src/resync_slv_level_coherent.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/src/resync_slv_level_on_signal.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.148293 tsfpga-9.0.0/modules/resync/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/test/tb_resync_counter.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/test/tb_resync_cycles.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3058 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/test/tb_resync_pulse.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     3744 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/test/tb_resync_slv_level.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2233 2021-10-19 08:05:04.000000 tsfpga-9.0.0/modules/resync/test/tb_resync_slv_level_on_signal.vhd
+-rw-rw-rw-   0 root         (0) root         (0)       31 2021-10-19 08:05:04.000000 tsfpga-9.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-10-19 08:05:16.188296 tsfpga-9.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5296 2021-10-19 08:05:04.000000 tsfpga-9.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.105290 tsfpga-9.0.0/tsfpga/
+-rw-rw-rw-   0 root         (0) root         (0)      984 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4200 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/about.py
+-rw-rw-rw-   0 root         (0) root         (0)    19887 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/build_project_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/build_step_tcl_hook.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/create_vhdl_ls_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.150293 tsfpga-9.0.0/tsfpga/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8389 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/build.py
+-rw-rw-rw-   0 root         (0) root         (0)     2366 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/example_env.py
+-rw-rw-rw-   0 root         (0) root         (0)     3306 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/formal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.094290 tsfpga-9.0.0/tsfpga/examples/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.151294 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/module_artyz7.py
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/regs_artyz7.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.152294 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/src/
+-rw-rw-rw-   0 root         (0) root         (0)    12849 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/src/artyz7_top.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/src/artyz7_top_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     5042 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/src/block_design_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     6879 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/src/block_design_wrapper.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.153294 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/tcl/
+-rw-rw-rw-   0 root         (0) root         (0)     2617 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/tcl/artyz7_pinning.tcl
+-rw-rw-rw-   0 root         (0) root         (0)    44962 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/tcl/block_design.tcl
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.154294 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/test/block_design_mock.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     6528 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/test/tb_artyz7_top.vhd
+-rw-rw-rw-   0 root         (0) root         (0)      596 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/artyz7/test/top_level_sim_pkg.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.154294 tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/
+-rw-rw-rw-   0 root         (0) root         (0)      837 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/module_ddr_buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/regs_ddr_buffer.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.155294 tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/sim/
+-rw-rw-rw-   0 root         (0) root         (0)     2374 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/sim/ddr_buffer_sim_pkg.vhd
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/sim/example_reg_operations_pkg.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.155294 tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/src/
+-rw-rw-rw-   0 root         (0) root         (0)     4596 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/src/ddr_buffer_top.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.156294 tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/test/
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/test/tb_ddr_buffer.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.156294 tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.157294 tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/ip_cores/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/ip_cores/fifo_generator_0.tcl
+-rw-rw-rw-   0 root         (0) root         (0)      621 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/ip_cores/mult_u12_u5.tcl
+-rw-rw-rw-   0 root         (0) root         (0)      954 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/module_multiplication_ip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.157294 tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/src/
+-rw-rw-rw-   0 root         (0) root         (0)      946 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/src/multiplication.vhd
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.157294 tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/test/tb_multiplication.vhd
+-rwxrwxrwx   0 root         (0) root         (0)      920 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/run_formal.sh
+-rw-rw-rw-   0 root         (0) root         (0)     4355 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/simulate.py
+-rw-rw-rw-   0 root         (0) root         (0)    11173 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/examples/simulation_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     8342 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/formal_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     7835 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/git_simulation_subset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3582 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/git_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/hdl_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/ip_core_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    17321 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/module.py
+-rw-rw-rw-   0 root         (0) root         (0)     6527 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/module_documentation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1937 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/module_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.163294 tsfpga-9.0.0/tsfpga/registers/
+-rw-rw-rw-   0 root         (0) root         (0)      374 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/bit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/bit_vector.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     2774 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/html_translator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10134 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5682 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/register.py
+-rw-rw-rw-   0 root         (0) root         (0)     3320 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/register_array.py
+-rw-rw-rw-   0 root         (0) root         (0)     7113 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/register_c_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/register_code_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10008 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/register_cpp_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2186 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/register_field.py
+-rw-rw-rw-   0 root         (0) root         (0)     8449 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/register_html_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    17195 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/register_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/register_python_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     7800 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/register_vhdl_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.167295 tsfpga-9.0.0/tsfpga/registers/test/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3272 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/test_bit.py
+-rw-rw-rw-   0 root         (0) root         (0)     4929 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/test_bit_vector.py
+-rw-rw-rw-   0 root         (0) root         (0)      944 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/test_constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     3794 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/test_html_translator.py
+-rw-rw-rw-   0 root         (0) root         (0)    15074 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5423 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/test_register.py
+-rw-rw-rw-   0 root         (0) root         (0)     4660 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/test_register_array.py
+-rw-rw-rw-   0 root         (0) root         (0)     3429 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/test_register_code_generation.py
+-rw-rw-rw-   0 root         (0) root         (0)     7064 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/test_register_html_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    16138 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/test_register_list.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/test_register_python_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3337 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/registers/test/test_register_vhdl_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)       28 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      123 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/requirements_develop.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/sby_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3658 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/svn_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/system_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.168295 tsfpga-9.0.0/tsfpga/test/
+-rw-rw-rw-   0 root         (0) root         (0)      432 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.169295 tsfpga-9.0.0/tsfpga/test/functional/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/functional/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.169295 tsfpga-9.0.0/tsfpga/test/functional/commercial_simulators/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/functional/commercial_simulators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2569 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/functional/commercial_simulators/test_simulation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.170295 tsfpga-9.0.0/tsfpga/test/functional/gcc/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/functional/gcc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11355 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/functional/gcc/test_register_compilation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.171295 tsfpga-9.0.0/tsfpga/test/functional/vivado/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/functional/vivado/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9349 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/functional/vivado/test_building_vivado_project.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.173295 tsfpga-9.0.0/tsfpga/test/lint/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/lint/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15081 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/lint/pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)    16267 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/lint/pylintrc_original
+-rw-rw-rw-   0 root         (0) root         (0)     6290 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/lint/test_copyright.py
+-rw-rw-rw-   0 root         (0) root         (0)     5543 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/lint/test_file_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/lint/test_python_lint.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.178295 tsfpga-9.0.0/tsfpga/test/unit/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8800 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_build_project_list.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_build_step_tcl_hook.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_formal_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     4973 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_git_simulation_subset.py
+-rw-rw-rw-   0 root         (0) root         (0)     4866 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_git_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_hdl_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_ip_core_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     8704 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     3106 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_module_documentation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_module_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     2369 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_sby_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2846 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_svn_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2374 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_system_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_vhdl_file_documentation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/test/unit/test_yosys_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     3552 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vhdl_file_documentation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.182296 tsfpga-9.0.0/tsfpga/vivado/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3227 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/build_result.py
+-rw-rw-rw-   0 root         (0) root         (0)     4333 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/build_result_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2784 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     1805 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/hierarchical_utilization_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4562 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/ip_cores.py
+-rw-rw-rw-   0 root         (0) root         (0)     1664 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/logic_level_distribution_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    25202 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/simlib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3273 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/simlib_commercial.py
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/simlib_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     5282 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/simlib_ghdl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.184296 tsfpga-9.0.0/tsfpga/vivado/tcl/
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/tcl/check_timing.tcl
+-rw-rw-rw-   0 root         (0) root         (0)      440 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/tcl/report_logic_level_distribution.tcl
+-rw-rw-rw-   0 root         (0) root         (0)      494 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/tcl/report_utilization.tcl
+-rw-rw-rw-   0 root         (0) root         (0)     3136 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/tcl/vivado_default_run.tcl
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/tcl/vivado_fast_run.tcl
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/tcl/vivado_messages.tcl
+-rw-rw-rw-   0 root         (0) root         (0)    14026 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/tcl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.187296 tsfpga-9.0.0/tsfpga/vivado/test/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/test/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1933 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/test/test_build_result.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/test/test_build_result_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1635 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/test/test_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/test/test_hierarchical_utilization_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/test/test_ip_cores.py
+-rw-rw-rw-   0 root         (0) root         (0)     2053 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/test/test_logic_level_distribution_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    16761 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/test/test_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     5861 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/test/test_simlib.py
+-rw-rw-rw-   0 root         (0) root         (0)    11093 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/vivado/test/test_tcl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2021-10-19 08:05:04.000000 tsfpga-9.0.0/tsfpga/yosys_project.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-19 08:05:16.107290 tsfpga-9.0.0/tsfpga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3186 2021-10-19 08:05:16.000000 tsfpga-9.0.0/tsfpga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11517 2021-10-19 08:05:16.000000 tsfpga-9.0.0/tsfpga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-19 08:05:16.000000 tsfpga-9.0.0/tsfpga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-19 08:05:16.000000 tsfpga-9.0.0/tsfpga.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      158 2021-10-19 08:05:16.000000 tsfpga-9.0.0/tsfpga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2021-10-19 08:05:16.000000 tsfpga-9.0.0/tsfpga.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tsfpga-8.0.1/PKG-INFO` & `tsfpga-9.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsfpga
-Version: 8.0.1
+Version: 9.0.0
 Summary: tsfpga is a development platform that aims to streamline all aspects of your FPGA project.
 Home-page: https://tsfpga.com
 Author: Lukas Vik
 Author-email: 2767848-LukasVik@users.noreply.gitlab.com
 License: BSD 3-Clause License
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 
 About tsfpga
 ============
 
-|pic_website| |pic_gitlab| |pic_gitter| |pic_pip_install| |pic_license| |pic_python_line_coverage| |pic_vhdl_line_coverage| |pic_vhdl_branch_coverage|
+|pic_website| |pic_gitlab| |pic_gitter| |pic_pip_install| |pic_license| |pic_python_line_coverage|
 
 .. |pic_website| image:: https://tsfpga.com/badges/website.svg
   :alt: Website
   :target: https://tsfpga.com
 
 .. |pic_gitlab| image:: https://tsfpga.com/badges/gitlab.svg
   :alt: Gitlab
@@ -45,22 +45,14 @@
   :alt: License
   :target: https://tsfpga.com/license_information.html
 
 .. |pic_python_line_coverage| image:: https://tsfpga.com/badges/python_coverage.svg
   :alt: Python line coverage
   :target: https://tsfpga.com/python_coverage_html
 
-.. |pic_vhdl_line_coverage| image:: https://tsfpga.com/badges/vhdl_line_coverage.svg
-  :alt: VHDL line coverage
-  :target: https://tsfpga.com/vhdl_coverage_html
-
-.. |pic_vhdl_branch_coverage| image:: https://tsfpga.com/badges/vhdl_branch_coverage.svg
-  :alt: VHDL branch coverage
-  :target: https://tsfpga.com/vhdl_coverage_html
-
 tsfpga is a development platform that aims to streamline all aspects of your FPGA project.
 With its python build/simulation flow, along with complementary VHDL components, it is perfect for CI/CD and test-driven development.
 Focus has been placed on flexibility and modularization, achieving scalability even in very large multi-vendor code bases.
 
 **See documentation on the website**: https://tsfpga.com
 
 Key features
@@ -69,12 +61,13 @@
 * Source code centric project structure: Build projects, test configurations, constraints, IP cores, etc. are handled close to the source code.
 * Automatically adds build/simulation sources if a recognized folder structure is used.
 * Enables local VUnit configuration setup without multiple ``run.py``.
 * Handling of IP cores and simlib for your simulation project, with automatic re-compile when necessary.
 * Python-based parallel Vivado build system.
 * Register code generation from TOML: VHDL package, HTML documentation, C header, C++ class.
 * VHDL AXI components that enable the register bus: AXI-to-AXI-Lite converter, AXI-Lite interconnect, AXI-Lite mux (splitter), AXI-Lite clock domain crossing, AXI-Lite generic register file.
+* Released under the very permissive BSD 3-Clause License.
 
 The maintainers place high focus on quality, with everything having good unit test coverage and a thought-out structure.
 The project is mature and used in many production environments.
```

### Comparing `tsfpga-8.0.1/examples/build.py` & `tsfpga-9.0.0/tsfpga/examples/build.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,103 +8,136 @@
 
 import argparse
 from pathlib import Path
 from shutil import copy2, make_archive
 import sys
 
 # Do PYTHONPATH insert() instead of append() to prefer any local repo checkout over any pip install
-PATH_TO_TSFPGA = Path(__file__).parent.parent.resolve()
+PATH_TO_TSFPGA = Path(__file__).parent.parent.parent.resolve()
 sys.path.insert(0, str(PATH_TO_TSFPGA))
-PATH_TO_VUNIT = PATH_TO_TSFPGA.parent / "vunit"
-sys.path.insert(0, str(PATH_TO_VUNIT))
+
+from tsfpga.examples.example_env import get_tsfpga_example_modules, TSFPGA_EXAMPLES_TEMP_DIR
 
 from tsfpga.build_project_list import BuildProjectList
+from tsfpga.module import get_tsfpga_modules
 from tsfpga.system_utils import create_directory, delete
 
-from examples.tsfpga_example_env import get_tsfpga_modules, TSFPGA_EXAMPLES_TEMP_DIR
-
 
 def arguments(default_temp_dir=TSFPGA_EXAMPLES_TEMP_DIR):
+    """
+    Setup of arguments for the example build flow.
+
+    Arguments:
+        default_temp_dir (`pathlib.Path`): Default value for output paths.
+    """
     parser = argparse.ArgumentParser(
         "Create, synth and build an FPGA project",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
+
     parser.add_argument("--no-color", action="store_true", help="disable color in printouts")
+
     parser.add_argument("--list-only", action="store_true", help="list the available projects")
+
     parser.add_argument("--open", action="store_true", help="open existing projects in the GUI")
+
     parser.add_argument(
         "--use-existing-project",
         action="store_true",
         help="build existing projects, or create first if they do not exist",
     )
+
     parser.add_argument(
         "--generate-registers-only",
         action="store_true",
         help="only generate the register artifacts (C/C++ code, HTML, ...) for inspection",
     )
+
     parser.add_argument("--create-only", action="store_true", help="only create projects")
+
     parser.add_argument("--synth-only", action="store_true", help="only synthesize projects")
+
     parser.add_argument(
         "--netlist-builds",
         action="store_true",
         help="use netlist build projects instead of top level build projects",
     )
+
     parser.add_argument(
         "--projects-path",
         type=Path,
         default=default_temp_dir / "projects",
         help="the FPGA build projects will be placed here",
     )
+
     parser.add_argument(
         "--ip-cache-path",
         type=Path,
         default=default_temp_dir / "vivado_ip_cache",
         help="location of Vivado IP cache",
     )
+
     parser.add_argument(
         "--output-path",
         type=Path,
         required=False,
         help="the output products (bit file, ...) will be placed here",
     )
+
     parser.add_argument(
-        "--num-parallel-builds", type=int, default=4, help="Number of parallel builds to launch"
+        "--num-parallel-builds", type=int, default=8, help="Number of parallel builds to launch"
     )
+
     parser.add_argument(
         "--num-threads-per-build",
         type=int,
         default=4,
         help="number of threads for each build process",
     )
+
     parser.add_argument(
         "project_filters",
         nargs="*",
         help="filter for which projects to build. Can use wildcards. Leave empty for all.",
     )
+
     args = parser.parse_args()
 
     return args
 
 
 def main():
+    """
+    Main function for building FPGA projects. If you are setting up a new build flow from scratch,
+    you probably want to copy and modify this function, and reuse the others.
+    """
     args = arguments()
-    modules = get_tsfpga_modules()
+    modules = get_tsfpga_modules() + get_tsfpga_example_modules()
     projects = BuildProjectList(
         modules=modules,
         project_filters=args.project_filters,
         include_netlist_not_top_builds=args.netlist_builds,
         no_color=args.no_color,
     )
 
     sys.exit(setup_and_run(modules, projects, args))
 
 
 def setup_and_run(modules, projects, args):
     """
-    Returns 0 if everything passed, otherwise non-zero.
+    Setup build projects, and execute as instructed by the arguments.
+
+    Arguments:
+        modules (:class:`.ModuleList`): When running a register generation, registers from these
+            modules will be included.
+        projects (:class:`.BuildProjectList`): These build projects will be built.
+        args: Command line argument namespace.
+
+    Return:
+        int: 0 if everything passed, otherwise non-zero. Can be used for system exit code.
     """
     if args.list_only:
         print(projects)
         return 0
 
     if args.generate_registers_only:
         # Generate register output from all modules. Note that this is not used by the
@@ -151,14 +184,24 @@
 
     if build_ok:
         return 0
     return 1
 
 
 def collect_artifacts(project, output_path):
+    """
+    Example of a method to collect build artifacts. Will create a zip file with the bitstream,
+    hardware definition (.xsa) and register documentation.
+
+    Arguments:
+        project (:class:`.VivadoProject`): Project object that has been built,
+            and who's artifacts shall now be collected.
+        output_path (`pathlib.Path`): Path to the build output. Artifact zip will be placed here
+            as well.
+    """
     version = "0.0.0.0"
     release_dir = create_directory(output_path / f"{project.name}-{version}", empty=True)
     print(f"Creating release in {release_dir.resolve()}.zip")
 
     generate_registers(project.modules, release_dir / "registers")
     copy2(output_path / f"{project.name }.bit", release_dir)
     copy2(output_path / f"{project.name}.bin", release_dir)
@@ -170,14 +213,21 @@
     # Remove folder so that only zip remains
     delete(release_dir)
 
     return True
 
 
 def generate_registers(modules, output_path):
+    """
+    Generate all register artifacts from the given modules.
+
+    Arguments:
+        modules (:class:`.ModuleList`): Registers from these modules will be included.
+        output_path (`pathlib.Path`): Register artifacts will be placed here.
+    """
     print(f"Generating registers in {output_path.resolve()}")
 
     for module in modules:
         if module.registers is not None:
             vhdl_path = create_directory(output_path / "vhdl", empty=False)
             module.registers.create_vhdl_package(vhdl_path)
```

### Comparing `tsfpga-8.0.1/examples/formal.py` & `tsfpga-9.0.0/tsfpga/examples/formal.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,75 +9,91 @@
 # --------------------------------------------------------------------------------------------------
 
 import argparse
 from pathlib import Path
 import sys
 
 # Do PYTHONPATH insert() instead of append() to prefer any local repo checkout over any pip install
-PATH_TO_TSFPGA = Path(__file__).parent.parent.resolve()
+PATH_TO_TSFPGA = Path(__file__).parent.parent.parent.resolve()
 sys.path.insert(0, str(PATH_TO_TSFPGA))
-PATH_TO_VUNIT = PATH_TO_TSFPGA.parent / "vunit"
-sys.path.insert(0, str(PATH_TO_VUNIT))
 
-from examples.tsfpga_example_env import get_tsfpga_modules, TSFPGA_EXAMPLES_TEMP_DIR
+from tsfpga.examples.example_env import TSFPGA_EXAMPLES_TEMP_DIR
 
-import tsfpga
 from tsfpga.formal_project import FormalProject
+from tsfpga.module import get_tsfpga_modules
 from tsfpga.system_utils import delete
 
 
 def arguments(default_temp_dir=TSFPGA_EXAMPLES_TEMP_DIR):
+    """
+    Setup of arguments for the example build flow.
+
+    Arguments:
+        default_temp_dir (`pathlib.Path`): Default value for output paths.
+    """
     parser = argparse.ArgumentParser(
         "Run formal tests", formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
+
     parser.add_argument("--list-only", action="store_true", help="list the available tests")
+
     parser.add_argument("--clean-only", action="store_true", help="clears the project path")
+
     parser.add_argument(
         "--project-path",
         type=Path,
         default=default_temp_dir / "formal_project",
         help="the formal project will be placed here",
     )
+
     parser.add_argument("test_filters", nargs="*", default="*", help="Tests to run")
+
     parser.add_argument(
         "--num-threads",
         "-p",
         type=int,
         default=8,
         help="number of threads to use when building project",
     )
+
     parser.add_argument(
         "--verbose",
         action="store_true",
         help="print all build output, even if the run is successful",
     )
+
     parser.add_argument(
         "--quiet",
         action="store_true",
         help="do not print any build output, even if the run has failed",
     )
+
     parser.add_argument(
         "--no-color",
         action="store_true",
         help="disable color in printouts",
     )
 
     args = parser.parse_args()
 
     return args
 
 
 def main():
+    """
+    Main function for running formal test. If you are setting up a new formal flow from scratch,
+    you probably want to copy and modify this function.
+    """
     args = arguments()
 
     if args.clean_only:
         delete(args.project_path)
         return
 
-    modules = get_tsfpga_modules([tsfpga.TSFPGA_MODULES])
+    modules = get_tsfpga_modules()
     formal_project = FormalProject(modules=modules, project_path=args.project_path)
     for module in modules:
         module.setup_formal(formal_project)
 
     if args.list_only:
         formal_project.list_tests(args.test_filters)
         return
```

### Comparing `tsfpga-8.0.1/examples/modules/artyz7/module_artyz7.py` & `tsfpga-9.0.0/tsfpga/examples/modules/artyz7/module_artyz7.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 # https://tsfpga.com
 # https://gitlab.com/tsfpga/tsfpga
 # --------------------------------------------------------------------------------------------------
 
 from pathlib import Path
 
 from tsfpga.constraint import Constraint
-from tsfpga.module import BaseModule
+from tsfpga.module import BaseModule, get_tsfpga_modules
+from tsfpga.examples.example_env import get_tsfpga_example_modules
 from tsfpga.vivado.project import VivadoProject
 
-from examples.tsfpga_example_env import get_tsfpga_modules
 
 THIS_FILE = Path(__file__)
 
 
 class Module(BaseModule):
     def get_build_projects(self):
         projects = []
 
-        modules = get_tsfpga_modules()
+        modules = get_tsfpga_modules() + get_tsfpga_example_modules()
         part = "xc7z020clg400-1"
 
         tcl_dir = self.path / "tcl"
         pinning = Constraint(tcl_dir / "artyz7_pinning.tcl")
         block_design = tcl_dir / "block_design.tcl"
 
         projects.append(
```

### Comparing `tsfpga-8.0.1/examples/modules/artyz7/regs_artyz7.toml` & `tsfpga-9.0.0/tsfpga/examples/modules/artyz7/regs_artyz7.toml`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/artyz7/src/artyz7_top.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/artyz7/src/artyz7_top.vhd`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,30 @@
 --
 -- This file is part of the tsfpga project.
 -- https://tsfpga.com
 -- https://gitlab.com/tsfpga/tsfpga
 -- -------------------------------------------------------------------------------------------------
 
 library ieee;
-use ieee.std_logic_1164.all;
 use ieee.numeric_std.all;
+use ieee.std_logic_1164.all;
 
 library axi;
 use axi.axi_pkg.all;
 use axi.axi_lite_pkg.all;
 
+library common;
+use common.common_pkg.all;
+
 library ddr_buffer;
+
 library fifo;
+
 library reg_file;
+
 library resync;
 
 use work.artyz7_top_pkg.all;
 use work.artyz7_regs_pkg.all;
 
 
 entity artyz7_top is
@@ -102,14 +108,15 @@
         port map (
           clk => clk_m_gp0,
           --
           axi_lite_m2s => regs_m2s(slave),
           axi_lite_s2m => regs_s2m(slave)
         );
     end generate;
+
   end block;
 
 
   ------------------------------------------------------------------------------
   ddr_buffer_inst : entity ddr_buffer.ddr_buffer_top
     port map (
       clk => clk_s_hp0,
@@ -386,8 +393,31 @@
           pulse_out => fifo_read_ready
         );
 
     end block;
 
   end block;
 
+
+  ------------------------------------------------------------------------------
+  -- Instantiate protocol checker within a simulation guard. To show that it is indeed possible to
+  -- synthesize code with this instance.
+  protocol_checker_test_gen : if in_simulation generate
+
+    ------------------------------------------------------------------------------
+    axi_stream_protocol_checker_inst : entity common.axi_stream_protocol_checker
+      generic map (
+        data_width => m_gp0_data_width
+      )
+      port map (
+        clk => clk_m_gp0,
+        --
+        ready => m_gp0_s2m.write.w.ready,
+        valid => m_gp0_m2s.write.w.valid,
+        last => m_gp0_m2s.write.w.last,
+        data => m_gp0_m2s.write.w.data(m_gp0_data_width - 1 downto 0),
+        strobe => m_gp0_m2s.write.w.strb(m_gp0_data_width / 8 - 1 downto 0)
+      );
+
+  end generate;
+
 end architecture;
```

### Comparing `tsfpga-8.0.1/examples/modules/artyz7/src/artyz7_top_pkg.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/artyz7/src/artyz7_top_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/artyz7/src/block_design_pkg.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/artyz7/src/block_design_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/artyz7/src/block_design_wrapper.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/artyz7/src/block_design_wrapper.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/artyz7/tcl/artyz7_pinning.tcl` & `tsfpga-9.0.0/tsfpga/examples/modules/artyz7/tcl/artyz7_pinning.tcl`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/artyz7/tcl/block_design.tcl` & `tsfpga-9.0.0/tsfpga/examples/modules/artyz7/tcl/block_design.tcl`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/artyz7/test/block_design_mock.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/artyz7/test/block_design_mock.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/artyz7/test/tb_artyz7_top.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/artyz7/test/tb_artyz7_top.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/artyz7/test/top_level_sim_pkg.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/artyz7/test/top_level_sim_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/ddr_buffer/module_ddr_buffer.py` & `tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/module_ddr_buffer.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/ddr_buffer/regs_ddr_buffer.toml` & `tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/regs_ddr_buffer.toml`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/ddr_buffer/sim/ddr_buffer_sim_pkg.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/sim/ddr_buffer_sim_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/ddr_buffer/sim/example_reg_operations_pkg.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/sim/example_reg_operations_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/ddr_buffer/src/ddr_buffer_top.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/src/ddr_buffer_top.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules/ddr_buffer/test/tb_ddr_buffer.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/ddr_buffer/test/tb_ddr_buffer.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules_with_ip/module_with_ip_cores/ip_cores/fifo_generator_0.tcl` & `tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/ip_cores/fifo_generator_0.tcl`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules_with_ip/module_with_ip_cores/ip_cores/mult_u12_u5.tcl` & `tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/ip_cores/mult_u12_u5.tcl`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/examples/modules_with_ip/module_with_ip_cores/src/mult.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/src/multiplication.vhd`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 library ieee;
 use ieee.std_logic_1164.all;
 use ieee.numeric_std.all;
 
 library xil_defaultlib;
 
 
-entity mult is
+entity multiplication is
   port (
     clk : in std_logic;
     --
     multiplicand : in unsigned(12 - 1 downto 0);
     multiplier : in unsigned(5 - 1 downto 0);
     --
     product : out unsigned(17 - 1 downto 0)
   );
 end entity;
 
-architecture a of mult is
+architecture a of multiplication is
 
 begin
 
   mult_inst : entity xil_defaultlib.mult_u12_u5
     port map (
       clk => clk,
       a => std_logic_vector(multiplicand),
```

### Comparing `tsfpga-8.0.1/examples/modules_with_ip/module_with_ip_cores/test/tb_mult.vhd` & `tsfpga-9.0.0/tsfpga/examples/modules/multiplication_ip/test/tb_multiplication.vhd`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 use ieee.std_logic_1164.all;
 use ieee.numeric_std.all;
 
 library vunit_lib;
 context vunit_lib.vunit_context;
 
 
-entity tb_mult is
+entity tb_multiplication is
   generic (
     runner_cfg : string
   );
 end entity;
 
-architecture tb of tb_mult is
+architecture tb of tb_multiplication is
 
   signal clk : std_logic := '0';
 
   signal multiplicand : unsigned(12 - 1 downto 0);
   signal multiplier : unsigned(5 - 1 downto 0);
   signal product : unsigned(17 - 1 downto 0);
 
@@ -35,27 +35,29 @@
 
 
   ------------------------------------------------------------------------------
   main : process
   begin
     test_runner_setup(runner, runner_cfg);
 
+    check_equal(product, 0);
+
     multiplicand <= to_unsigned(3125, multiplicand);
     multiplier <= to_unsigned(18, multiplier);
 
     wait until rising_edge(clk);
     wait until rising_edge(clk);
     check_equal(product, 3125 * 18);
 
     test_runner_cleanup(runner);
   end process;
 
 
   ------------------------------------------------------------------------------
-  dut : entity work.mult
+  dut : entity work.multiplication
     port map (
       clk => clk,
 
       multiplicand => multiplicand,
       multiplier => multiplier,
 
       product => product
```

### Comparing `tsfpga-8.0.1/examples/tsfpga_example_env.py` & `tsfpga-9.0.0/tsfpga/examples/example_env.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,42 +6,30 @@
 # https://gitlab.com/tsfpga/tsfpga
 # --------------------------------------------------------------------------------------------------
 
 """
 Common functions and definitions in the example build environment.
 """
 
+import sys
+
 import tsfpga
 from tsfpga.module import get_modules
-
 from tsfpga.registers.register_list import Register
 
+# Do PYTHONPATH insert() instead of append() to prefer any local repo checkout over any pip install
+PATH_TO_VUNIT = tsfpga.REPO_ROOT.parent.parent / "vunit" / "vunit"
+sys.path.insert(0, str(PATH_TO_VUNIT))
 
 TSFPGA_EXAMPLES_TEMP_DIR = tsfpga.TSFPGA_GENERATED
 
 
-def get_tsfpga_modules(modules_folders=None, names_include=None, names_avoid=None):
-    """
-    Wrapper of the regular get_modules call with correct settings for tsfpga modules.
-    """
-    modules_folders = (
-        tsfpga.ALL_TSFPGA_MODULES_FOLDERS if modules_folders is None else modules_folders
-    )
-    return get_modules(
-        modules_folders,
-        names_include=names_include,
-        names_avoid=names_avoid,
-        library_name_has_lib_suffix=False,
-        default_registers=get_default_registers(),
-    )
-
-
 def get_default_registers():
     """
-    tsfpga default registers
+    Default registers for tsfpga examples.
     """
     registers = [
         Register("config", 0, "r_w", "Configuration register."),
         Register(
             "command",
             1,
             "wpulse",
@@ -61,7 +49,24 @@
             "irq_mask",
             4,
             "r_w",
             "A '1' in this register means that the corresponding interrupt is enabled.",
         ),
     ]
     return registers
+
+
+def get_tsfpga_example_modules(names_include=None, names_avoid=None):
+    """
+    Wrapper of the regular :func:`.get_modules`. call with correct settings for tsfpga
+    example modules.
+    This will include the example tsfpga modules, but not the "real" modules.
+
+    Arguments will be passed on to :func:`.get_modules`.
+    """
+    return get_modules(
+        modules_folders=[tsfpga.TSFPGA_EXAMPLE_MODULES],
+        names_include=names_include,
+        names_avoid=names_avoid,
+        library_name_has_lib_suffix=False,
+        default_registers=get_default_registers(),
+    )
```

### Comparing `tsfpga-8.0.1/modules/axi/module_axi.py` & `tsfpga-9.0.0/modules/axi/module_axi.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 # Copyright (c) Lukas Vik. All rights reserved.
 #
 # This file is part of the tsfpga project.
 # https://tsfpga.com
 # https://gitlab.com/tsfpga/tsfpga
 # --------------------------------------------------------------------------------------------------
 
-from tsfpga.module import BaseModule
+from tsfpga.module import BaseModule, get_tsfpga_modules
 from tsfpga.vivado.project import VivadoNetlistProject
-from examples.tsfpga_example_env import get_tsfpga_modules
 
 
 class Module(BaseModule):
-    def setup_vunit(self, vunit_proj, **kwargs):
+    def setup_vunit(self, vunit_proj, **kwargs):  # pylint: disable=unused-argument
         tb = vunit_proj.library(self.library_name).test_bench("tb_axi_pkg")
         for data_width in [32, 64]:
             for id_width in [0, 5]:
                 for addr_width in [32, 40]:
                     generics = dict(data_width=data_width, id_width=id_width, addr_width=addr_width)
                     self.add_vunit_config(tb, generics=generics)
```

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_address_fifo.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_address_fifo.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_b_fifo.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_b_fifo.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_lite_cdc.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_lite_cdc.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_lite_mux.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_lite_mux.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_lite_pipeline.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_lite_pipeline.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_lite_pkg.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_lite_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_lite_simple_read_crossbar.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_lite_simple_read_crossbar.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_lite_simple_write_crossbar.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_lite_simple_write_crossbar.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_lite_to_vec.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_lite_to_vec.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_pkg.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_r_fifo.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_r_fifo.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_read_cdc.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_read_cdc.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_read_throttle.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_read_throttle.vhd`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 
     -- +1 in range for sign bit
   signal minus_burst_length_beats : signed(len_width + 1 - 1 downto 0) :=
     (others => '0');
 
   -- Number of data beats that have been negotiated via address transactions,
   -- but have not yet been sent by the master. Aka outstanding beats.
+  -- Note that according to the AXI standard, RVALID may never arrive before ARREADY.
+  -- Hence this counter can never go negative.
   subtype data_counter_t is integer range 0 to data_fifo_depth;
   signal num_beats_negotiated_but_not_sent : data_counter_t := 0;
 
   -- Negation of:
   -- Number of data beat words empty in the FIFO, that are not claimed by oustanding transactions.
   signal minus_num_empty_words_in_fifo_that_have_not_been_negotiated :
     integer range -data_fifo_depth to 0 := 0;
```

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_simple_read_crossbar.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_simple_read_crossbar.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_simple_write_crossbar.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_simple_write_crossbar.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_stream_fifo.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_stream_fifo.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_stream_pkg.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_stream_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_to_axi_lite.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_to_axi_lite.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_to_axi_lite_vec.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_to_axi_lite_vec.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_w_fifo.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_w_fifo.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_write_cdc.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_write_cdc.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/src/axi_write_throttle.vhd` & `tsfpga-9.0.0/modules/axi/src/axi_write_throttle.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_cdc.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_cdc.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_fifo.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_fifo.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_lite_cdc.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_lite_cdc.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_lite_mux.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_lite_mux.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_lite_pipeline.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_lite_pipeline.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_lite_pkg.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_lite_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_pkg.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_simple_crossbar.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_simple_crossbar.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_stream_fifo.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_stream_fifo.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_stream_pkg.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_stream_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_to_axi_lite.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_to_axi_lite.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_to_axi_lite_bus_error.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_to_axi_lite_bus_error.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/axi/test/tb_axi_to_axi_lite_vec.vhd` & `tsfpga-9.0.0/modules/axi/test/tb_axi_to_axi_lite_vec.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/bfm/sim/axi_lite_master.vhd` & `tsfpga-9.0.0/modules/bfm/sim/axi_lite_master.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/bfm/sim/axi_lite_read_slave.vhd` & `tsfpga-9.0.0/modules/bfm/sim/axi_lite_read_slave.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/bfm/sim/axi_lite_slave.vhd` & `tsfpga-9.0.0/modules/bfm/sim/axi_lite_slave.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/bfm/sim/axi_lite_write_slave.vhd` & `tsfpga-9.0.0/modules/bfm/sim/axi_lite_write_slave.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/bfm/sim/axi_master.vhd` & `tsfpga-9.0.0/modules/bfm/sim/axi_master.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/bfm/sim/axi_read_slave.vhd` & `tsfpga-9.0.0/modules/bfm/sim/axi_read_slave.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/bfm/sim/axi_slave.vhd` & `tsfpga-9.0.0/modules/bfm/sim/axi_slave.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/bfm/sim/axi_slave_pkg.vhd` & `tsfpga-9.0.0/modules/bfm/sim/axi_slave_pkg.vhd`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 --
 -- This file is part of the tsfpga project.
 -- https://tsfpga.com
 -- https://gitlab.com/tsfpga/tsfpga
 -- -------------------------------------------------------------------------------------------------
 
 library vunit_lib;
-context vunit_lib.vc_context;
+use vunit_lib.axi_slave_pkg.all;
+use vunit_lib.memory_pkg.all;
+context vunit_lib.com_context;
 context vunit_lib.vunit_context;
 
 
 package axi_slave_pkg is
 
   -- Perhaps this should be commited to VUnit's axi_slave_pkg (under the name null_axi_slave)?
   constant axi_slave_init : axi_slave_t := (
```

### Comparing `tsfpga-8.0.1/modules/bfm/sim/axi_write_slave.vhd` & `tsfpga-9.0.0/modules/bfm/sim/axi_write_slave.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/bfm/sim/bfm_pkg.vhd` & `tsfpga-9.0.0/modules/bfm/sim/bfm_pkg.vhd`

 * *Files 24% similar despite different names*

```diff
@@ -4,23 +4,33 @@
 -- This file is part of the tsfpga project.
 -- https://tsfpga.com
 -- https://gitlab.com/tsfpga/tsfpga
 -- -------------------------------------------------------------------------------------------------
 
 library ieee;
 use ieee.numeric_std.all;
+use ieee.std_logic_1164.all;
 
 library vunit_lib;
 context vunit_lib.vc_context;
 context vunit_lib.vunit_context;
 
+library osvvm;
+use osvvm.RandomPkg.RandomPType;
+
 
 package bfm_pkg is
 
-  -- Convenience method for getting vectors of BFM/VC elements.
+  procedure random_stall(
+    stall_config : in stall_config_t;
+    rnd : inout RandomPType;
+    signal clk : in std_logic
+  );
+
+  -- Some convenience method for getting vectors of BFM/VC elements.
   -- When doing e.g.
   --   constant my_masters : axi_stream_master_vec_t(0 to 1) :=
   --     (others => new_axi_stream_master(...));
   -- works well in some simulators (GHDL), meaning that the function is evaluated once for each
   -- element of the vector. In e.g. modelsim the function is only evaluated once, and all elements
   -- get the same value. Hence the need for this function.
 
@@ -43,18 +53,39 @@
   impure function get_new_axi_stream_slaves(
     count : positive;
     data_width : positive;
     logger_name : string;
     stall_config : stall_config_t
   ) return axi_stream_slave_vec_t;
 
+  type bus_master_vec_t is array (integer range <>) of bus_master_t;
+
 end package;
 
 package body bfm_pkg is
 
+  procedure random_stall(
+    stall_config : in stall_config_t;
+    rnd : inout RandomPType;
+    signal clk : in std_logic
+  ) is
+    variable num_stall_cycles : natural := 0;
+  begin
+    if rnd.Uniform(0.0, 1.0) < stall_config.stall_probability then
+      num_stall_cycles := rnd.FavorSmall(
+        stall_config.min_stall_cycles,
+        stall_config.max_stall_cycles
+      );
+
+      for stall in 1 to num_stall_cycles loop
+        wait until rising_edge(clk);
+      end loop;
+    end if;
+  end procedure;
+
   impure function get_new_queues(count : positive) return queue_vec_t is
     variable result : queue_vec_t(0 to count - 1) := (others => null_queue);
   begin
     for queue_idx in result'range loop
       result(queue_idx) := new_queue;
     end loop;
     return result;
```

### Comparing `tsfpga-8.0.1/modules/common/module_common.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_build_project_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,250 +2,222 @@
 # Copyright (c) Lukas Vik. All rights reserved.
 #
 # This file is part of the tsfpga project.
 # https://tsfpga.com
 # https://gitlab.com/tsfpga/tsfpga
 # --------------------------------------------------------------------------------------------------
 
+import unittest
+from unittest.mock import MagicMock
+import pytest
+
+from tsfpga.build_project_list import BuildProjectList
 from tsfpga.module import BaseModule
-from tsfpga.vivado.project import VivadoNetlistProject
-from tsfpga.vivado.build_result_checker import EqualTo, Ffs, Srls, TotalLuts
-from examples.tsfpga_example_env import get_tsfpga_modules
-
-
-class Module(BaseModule):
-    def setup_vunit(self, vunit_proj, **kwargs):
-        tb = vunit_proj.library(self.library_name).test_bench("tb_clock_counter")
-        self.add_vunit_config(
-            tb, generics=dict(reference_clock_rate_mhz=250, target_clock_rate_mhz=50)
-        )
-        self.add_vunit_config(
-            tb, generics=dict(reference_clock_rate_mhz=50, target_clock_rate_mhz=250)
-        )
-
-        tb = vunit_proj.library(self.library_name).test_bench("tb_periodic_pulser")
-
-        for period in [5, 15, 37, 300, 4032]:
-            self.add_vunit_config(tb, generics=dict(period=period, shift_register_length=8))
-
-        tb = vunit_proj.library(self.library_name).test_bench("tb_width_conversion")
-
-        test = tb.get_tests("test_data")[0]
-        for input_width in [8, 16, 32]:
-            for output_width in [8, 16, 32]:
-                if input_width == output_width:
-                    continue
-
-                for enable_strobe in [True, False]:
-                    generics = dict(
-                        input_width=input_width,
-                        output_width=output_width,
-                        enable_strobe=enable_strobe,
-                    )
-
-                    if enable_strobe and input_width < output_width:
-                        generics["support_unaligned_burst_length"] = True
-
-                    self.add_vunit_config(test, generics=generics)
-
-        test = tb.get_tests("test_full_throughput")[0]
-        test.add_config(
-            name="input_16.output_8",
-            generics=dict(input_width=16, output_width=8, enable_strobe=False, data_jitter=False),
-        )
-        test.add_config(
-            name="input_8.output_16",
-            generics=dict(input_width=8, output_width=16, enable_strobe=False, data_jitter=False),
-        )
-
-        for test in (
-            vunit_proj.library(self.library_name).test_bench("tb_handshake_pipeline").get_tests()
-        ):
-            if "full_throughput" in test.name:
-                for allow_poor_input_ready_timing in [False, True]:
-                    generics = dict(
-                        full_throughput=True,
-                        allow_poor_input_ready_timing=allow_poor_input_ready_timing,
-                    )
-                    self.add_vunit_config(test=test, generics=generics)
-
-            if "random_data" in test.name:
-                for full_throughput in [False, True]:
-                    for allow_poor_input_ready_timing in [False, True]:
-                        generics = dict(
-                            data_jitter=True,
-                            full_throughput=full_throughput,
-                            allow_poor_input_ready_timing=allow_poor_input_ready_timing,
-                        )
-                        self.add_vunit_config(test=test, generics=generics)
-
-    def get_build_projects(self):
-        projects = []
-        part = "xc7z020clg400-1"
-        self._get_handshake_pipeline_build_projects(part, projects)
-        self._get_clock_counter_build_projects(part, projects)
-        self._get_period_pulser_build_projects(part, projects)
-        self._get_width_conversion_build_projects(part, projects)
-        return projects
-
-    def _get_handshake_pipeline_build_projects(self, part, projects):
-        generics = dict(data_width=32)
-
-        generics.update(full_throughput=True, allow_poor_input_ready_timing=True)
-        projects.append(
-            VivadoNetlistProject(
-                name=self.test_case_name("handshake_pipeline", generics),
-                modules=[self],
-                part=part,
-                top="handshake_pipeline",
-                generics=generics,
-                build_result_checkers=[
-                    TotalLuts(EqualTo(1)),
-                    Ffs(EqualTo(34)),
-                ],
-            )
-        )
-
-        # Full skid-aside buffer is quite large.
-        generics.update(full_throughput=True, allow_poor_input_ready_timing=False)
-        projects.append(
-            VivadoNetlistProject(
-                name=self.test_case_name("handshake_pipeline", generics),
-                modules=[self],
-                part=part,
-                top="handshake_pipeline",
-                generics=generics,
-                build_result_checkers=[
-                    TotalLuts(EqualTo(37)),
-                    Ffs(EqualTo(70)),
-                ],
-            )
-        )
-
-        generics.update(full_throughput=False, allow_poor_input_ready_timing=True)
-        projects.append(
-            VivadoNetlistProject(
-                name=self.test_case_name("handshake_pipeline", generics),
-                modules=[self],
-                part=part,
-                top="handshake_pipeline",
-                generics=generics,
-                build_result_checkers=[
-                    TotalLuts(EqualTo(2)),
-                    Ffs(EqualTo(34)),
-                ],
-            )
-        )
-
-        generics.update(full_throughput=False, allow_poor_input_ready_timing=False)
-        projects.append(
-            VivadoNetlistProject(
-                name=self.test_case_name("handshake_pipeline", generics),
-                modules=[self],
-                part=part,
-                top="handshake_pipeline",
-                generics=generics,
-                build_result_checkers=[
-                    TotalLuts(EqualTo(1)),
-                    Ffs(EqualTo(35)),
-                ],
-            )
-        )
-
-    def _get_clock_counter_build_projects(self, part, projects):
-        modules = get_tsfpga_modules(names_include=[self.name, "math", "resync"])
-
-        generics = dict(resolution_bits=24, max_relation_bits=6)
-        projects.append(
-            VivadoNetlistProject(
-                name=self.test_case_name(name=f"{self.name}.clock_counter", generics=generics),
-                modules=modules,
-                part=part,
-                top="clock_counter",
-                generics=generics,
-                build_result_checkers=[
-                    TotalLuts(EqualTo(84)),
-                    Srls(EqualTo(5)),
-                    Ffs(EqualTo(185)),
-                ],
-            )
-        )
-
-        generics = dict(resolution_bits=10, max_relation_bits=4)
-        projects.append(
-            VivadoNetlistProject(
-                name=self.test_case_name(name=f"{self.name}.clock_counter", generics=generics),
-                modules=modules,
-                part=part,
-                top="clock_counter",
-                generics=generics,
-                build_result_checkers=[
-                    TotalLuts(EqualTo(38)),
-                    Srls(EqualTo(2)),
-                    Ffs(EqualTo(86)),
-                ],
-            )
-        )
-
-    def _get_period_pulser_build_projects(self, part, projects):
-        modules = get_tsfpga_modules(names_include=[self.name, "math"])
-
-        periods = [32, 37, 300, 63 * 64, 311000000]
-        total_luts = [2, 7, 4, 5, 18]
-        srls = [1, 0, 2, 3, 4]
-        ffs = [1, 6, 2, 3, 15]
-
-        for idx, period in enumerate(periods):
-            generics = dict(period=period, shift_register_length=32)
-            projects.append(
-                VivadoNetlistProject(
-                    name=self.test_case_name(f"{self.name}.periodic_pulser", generics),
-                    modules=modules,
-                    part=part,
-                    top="periodic_pulser",
-                    generics=generics,
-                    build_result_checkers=[
-                        TotalLuts(EqualTo(total_luts[idx])),
-                        Srls(EqualTo(srls[idx])),
-                        Ffs(EqualTo(ffs[idx])),
-                    ],
-                )
-            )
-
-    def _get_width_conversion_build_projects(self, part, projects):
-        modules = [self]
-        generic_configurations = [
-            dict(input_width=32, output_width=16, enable_strobe=False),
-            dict(input_width=16, output_width=32, enable_strobe=False),
-            dict(
-                input_width=32,
-                output_width=16,
-                enable_strobe=True,
-                strobe_unit_width=8,
-            ),
-            dict(
-                input_width=16,
-                output_width=32,
-                enable_strobe=True,
-                support_unaligned_burst_length=True,
-                strobe_unit_width=8,
-            ),
-        ]
-        total_luts = [21, 36, 26, 46]
-        ffs = [52, 52, 62, 65]
-
-        for idx, generics in enumerate(generic_configurations):
-            projects.append(
-                VivadoNetlistProject(
-                    name=self.test_case_name(
-                        name=f"{self.name}.width_conversion", generics=generics
-                    ),
-                    modules=modules,
-                    part=part,
-                    top="width_conversion",
-                    generics=generics,
-                    build_result_checkers=[
-                        TotalLuts(EqualTo(total_luts[idx])),
-                        Ffs(EqualTo(ffs[idx])),
-                    ],
-                )
-            )
+from tsfpga.system_utils import create_directory
+from tsfpga.vivado.project import VivadoProject, BuildResult
+
+
+# pylint: disable=too-many-instance-attributes
+@pytest.mark.usefixtures("fixture_tmp_path")
+class TestBuildProjectList(unittest.TestCase):
+
+    tmp_path = None
+
+    @staticmethod
+    def _get_mocks(name, is_netlist_build):
+        project = MagicMock(spec=VivadoProject)
+        project.name = name
+        project.__str__.return_value = f"MockProject {name}"
+        project.is_netlist_build = is_netlist_build
+
+        module = MagicMock(spec=BaseModule)
+        module.name = name
+        module.get_build_projects.return_value = [project]
+
+        return module, project
+
+    def setUp(self):
+        self.module_one, self.project_one = self._get_mocks("one", False)
+        self.module_two, self.project_two = self._get_mocks("two", False)
+
+        self.module_three, self.project_three = self._get_mocks("three", True)
+        self.module_four, self.project_four = self._get_mocks("four", True)
+
+        self.modules = [self.module_one, self.module_two, self.module_three, self.module_four]
+
+    def test_can_list_without_error(self):
+        list_str = str(BuildProjectList(self.modules))
+        assert "one" in list_str
+        assert "two" in list_str
+
+    def test_project_filtering(self):
+        project_list = BuildProjectList(self.modules)
+        assert len(project_list.projects) == 2
+        assert self.project_one in project_list.projects
+        assert self.project_two in project_list.projects
+
+        project_list = BuildProjectList(
+            self.modules, project_filters=["apa", "*ne", "three", "four"]
+        )
+        assert len(project_list.projects) == 1
+        assert self.project_one in project_list.projects
+
+        project_list = BuildProjectList(self.modules, include_netlist_not_top_builds=True)
+        assert len(project_list.projects) == 2
+        assert self.project_three in project_list.projects
+        assert self.project_four in project_list.projects
+
+        project_list = BuildProjectList(
+            self.modules,
+            include_netlist_not_top_builds=True,
+            project_filters=["apa", "one", "two", "thr*"],
+        )
+        assert len(project_list.projects) == 1
+        assert self.project_three in project_list.projects
+
+    def test_create(self):
+        project_list = BuildProjectList(self.modules, project_filters=["one", "two"])
+        assert project_list.create(
+            projects_path=self.tmp_path / "projects_path",
+            num_parallel_builds=2,
+            ip_cache_path=self.tmp_path / "ip_cache_path",
+        )
+
+        self.project_one.create.assert_called_once_with(
+            project_path=self.tmp_path / "projects_path" / "one" / "project",
+            ip_cache_path=self.tmp_path / "ip_cache_path",
+        )
+
+        self.project_two.create.assert_called_once_with(
+            project_path=self.tmp_path / "projects_path" / "two" / "project",
+            ip_cache_path=self.tmp_path / "ip_cache_path",
+        )
+
+        self.project_three.create.assert_not_called()
+        self.project_four.create.assert_not_called()
+
+    def test_create_unless_exists(self):
+        project_list = BuildProjectList(self.modules, project_filters=["one"])
+        assert project_list.create_unless_exists(
+            projects_path=self.tmp_path / "projects_path",
+            num_parallel_builds=2,
+            ip_cache_path=self.tmp_path / "ip_cache_path",
+        )
+
+        self.project_one.create.assert_called_once_with(
+            project_path=self.tmp_path / "projects_path" / "one" / "project",
+            ip_cache_path=self.tmp_path / "ip_cache_path",
+        )
+
+        # Create project file manually
+        create_directory(self.tmp_path / "projects_path" / "one" / "project")
+        (self.tmp_path / "projects_path" / "one" / "project" / "one.xpr").write_text("")
+
+        assert project_list.create_unless_exists(
+            projects_path=self.tmp_path / "projects_path",
+            num_parallel_builds=2,
+            ip_cache_path=self.tmp_path / "ip_cache_path",
+        )
+
+        # Still only called once after second create_unless_exists()
+        self.project_one.create.assert_called_once()
+
+        self.project_two.create.assert_not_called()
+        self.project_three.create.assert_not_called()
+        self.project_four.create.assert_not_called()
+
+    def test_build(self):
+        project_list = BuildProjectList(self.modules, project_filters=["one"])
+        assert project_list.build(
+            projects_path=self.tmp_path / "projects_path",
+            num_parallel_builds=2,
+            num_threads_per_build=4,
+            other_build_argument=True,
+        )
+
+        self.project_one.build.assert_called_once_with(
+            project_path=self.tmp_path / "projects_path" / "one" / "project",
+            output_path=self.tmp_path / "projects_path" / "one",
+            num_threads=4,
+            other_build_argument=True,
+        )
+
+    def test_build_fail_should_return_false(self):
+        project_list = BuildProjectList(self.modules, project_filters=["one"])
+        self.project_one.build.return_value = MagicMock(spec=BuildResult)
+        self.project_one.build.return_value.success = False
+
+        assert not project_list.build(
+            projects_path=self.tmp_path / "projects_path",
+            num_parallel_builds=2,
+            num_threads_per_build=4,
+            other_build_argument=True,
+        )
+
+    def test_build_with_output_path(self):
+        project_list = BuildProjectList(self.modules, project_filters=["one"])
+        assert project_list.build(
+            projects_path=self.tmp_path / "projects_path",
+            num_parallel_builds=2,
+            num_threads_per_build=4,
+            output_path=self.tmp_path / "output_path",
+        )
+
+        self.project_one.build.assert_called_once_with(
+            project_path=self.tmp_path / "projects_path" / "one" / "project",
+            output_path=self.tmp_path / "output_path" / "one",
+            num_threads=4,
+        )
+
+    def test_build_with_collect_artifacts(self):
+        project_list = BuildProjectList(self.modules, project_filters=["one"])
+        collect_artifacts = MagicMock()
+        assert project_list.build(
+            projects_path=self.tmp_path / "projects_path",
+            num_parallel_builds=2,
+            num_threads_per_build=4,
+            collect_artifacts=collect_artifacts,
+        )
+
+        collect_artifacts.assert_called_once_with(
+            project=self.project_one,
+            output_path=self.tmp_path / "projects_path" / "one",
+        )
+
+    def test_build_with_collect_artifacts_and_output_path(self):
+        project_list = BuildProjectList(self.modules, project_filters=["one"])
+        collect_artifacts = MagicMock()
+        assert project_list.build(
+            projects_path=self.tmp_path / "projects_path",
+            num_parallel_builds=2,
+            num_threads_per_build=4,
+            output_path=self.tmp_path / "output_path",
+            collect_artifacts=collect_artifacts,
+        )
+
+        collect_artifacts.assert_called_once_with(
+            project=self.project_one, output_path=self.tmp_path / "output_path" / "one"
+        )
+
+    def test_build_with_collect_artifacts_return_false_should_fail_build(self):
+        project_list = BuildProjectList(self.modules, project_filters=["one"])
+        collect_artifacts = MagicMock()
+        collect_artifacts.return_value = False
+        assert not project_list.build(
+            projects_path=self.tmp_path / "projects_path",
+            num_parallel_builds=2,
+            num_threads_per_build=4,
+            collect_artifacts=collect_artifacts,
+        )
+
+    def test_open(self):
+        project_list = BuildProjectList(self.modules, include_netlist_not_top_builds=True)
+        assert project_list.open(projects_path=self.tmp_path / "projects_path")
+
+        self.project_three.open.assert_called_once_with(
+            project_path=self.tmp_path / "projects_path" / "three" / "project"
+        )
+        self.project_four.open.assert_called_once_with(
+            project_path=self.tmp_path / "projects_path" / "four" / "project"
+        )
+        self.project_one.open.assert_not_called()
+        self.project_two.open.assert_not_called()
```

### Comparing `tsfpga-8.0.1/modules/common/src/addr_pkg.vhd` & `tsfpga-9.0.0/modules/common/src/addr_pkg.vhd`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 package addr_pkg is
 
   constant addr_width : integer := 32;
   subtype addr_t is unsigned(addr_width - 1 downto 0);
   type addr_vec_t is array (integer range <>) of addr_t;
+  function to_addr(value : natural) return addr_t;
 
   type addr_and_mask_t is record
     addr : addr_t;
     mask : addr_t;
   end record;
   type addr_and_mask_vec_t is array (integer range <>) of addr_and_mask_t;
 
@@ -32,14 +33,20 @@
 
   function decode(addr : unsigned; addrs : addr_and_mask_vec_t) return integer;
 
 end package;
 
 package body addr_pkg is
 
+  function to_addr(value : natural) return addr_t is
+    constant result : addr_t := to_unsigned(value, addr_width);
+  begin
+    return result;
+  end function;
+
   function addr_bits_needed(addrs : addr_and_mask_vec_t) return positive is
     variable result : positive := 1;
   begin
     -- Return the number of bits that are needed to decode and handle the addresses.
     for addr_idx in addrs'range loop
       result := maximum(result, num_bits_needed(addrs(addr_idx).mask));
     end loop;
```

### Comparing `tsfpga-8.0.1/modules/common/src/attribute_pkg.vhd` & `tsfpga-9.0.0/modules/common/src/attribute_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/common/src/clock_counter.vhd` & `tsfpga-9.0.0/modules/common/src/clock_counter.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/common/src/common_pkg.vhd` & `tsfpga-9.0.0/modules/common/src/common_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/common/src/debounce.vhd` & `tsfpga-9.0.0/modules/common/src/debounce.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/common/src/handshake_pipeline.vhd` & `tsfpga-9.0.0/modules/common/src/handshake_pipeline.vhd`

 * *Files 24% similar despite different names*

```diff
@@ -19,28 +19,38 @@
 entity handshake_pipeline is
   generic (
     data_width : integer;
     -- Setting to false can save logic footprint, at the cost of lower throughput
     full_throughput : boolean := true;
     -- Can result in smaller logic footprint and higher througphput, at the cost of worse timing
     -- on the input_ready signal.
-    allow_poor_input_ready_timing : boolean := false
+    allow_poor_input_ready_timing : boolean := false;
+    -- In the typical use case where we want a "byte strobe", this would be eight.
+    -- In other cases, for example when the data is packed, we migh use a higher value.
+    -- Must assign a valid value if input/output strobe is to be used.
+    strobe_unit_width : positive := 8
   );
   port (
     clk : in std_logic;
     --
     input_ready : out std_logic := '0';
     input_valid : in std_logic;
+    -- Optional to connect.
     input_last : in std_logic := '-';
     input_data : in std_logic_vector(data_width - 1 downto 0);
+    -- Optional to connect. Must set valid 'strobe_unit_width' generic value in order to use this.
+    input_strobe : in std_logic_vector(data_width / strobe_unit_width - 1 downto 0) :=
+      (others => '-');
     --
     output_ready : in std_logic;
     output_valid : out std_logic := '0';
     output_last : out std_logic := '0';
-    output_data : out std_logic_vector(data_width - 1 downto 0) := (others => '0')
+    output_data : out std_logic_vector(data_width - 1 downto 0) := (others => '0');
+    output_strobe : out std_logic_vector(data_width / strobe_unit_width - 1 downto 0) :=
+      (others => '0')
   );
 end entity;
 
 architecture a of handshake_pipeline is
 
 begin
 
@@ -61,16 +71,17 @@
     ------------------------------------------------------------------------------
     main : process
     begin
       wait until rising_edge(clk);
 
       if input_ready then
         output_valid <= input_valid;
-        output_data <= input_data;
         output_last <= input_last;
+        output_data <= input_data;
+        output_strobe <= input_strobe;
       end if;
     end process;
 
 
   ------------------------------------------------------------------------------
   elsif full_throughput and not allow_poor_input_ready_timing generate
 
@@ -81,16 +92,17 @@
     -- characteristics but also the largest logic footprint.
 
     signal input_ready_int : std_logic := '1';
 
     type state_t is (wait_for_input_valid, full_handshake_throughput, wait_for_output_ready);
     signal state : state_t := wait_for_input_valid;
 
-    signal input_data_skid : std_logic_vector(input_data'range);
-    signal input_last_skid : std_logic;
+    signal input_last_skid : std_logic := '0';
+    signal input_data_skid : std_logic_vector(input_data'range) := (others => '0');
+    signal input_strobe_skid : std_logic_vector(input_strobe'range) := (others => '0');
 
   begin
 
     input_ready <= input_ready_int;
 
 
     ------------------------------------------------------------------------------
@@ -99,50 +111,61 @@
       wait until rising_edge(clk);
 
       case state is
         when wait_for_input_valid =>
           if input_valid then
             -- input_ready is '1', so if we get here an input transaction has occured
             output_valid <= '1';
-            output_data <= input_data;
             output_last <= input_last;
+            output_data <= input_data;
+            output_strobe <= input_strobe;
+
             state <= full_handshake_throughput;
           end if;
 
         when full_handshake_throughput =>
           -- input_ready and output_valid are always '1' in this state
 
           if input_valid and output_ready then
             -- Input and output transactions have occured. Update data register.
-            output_data <= input_data;
             output_last <= input_last;
+            output_data <= input_data;
+            output_strobe <= input_strobe;
+
           elsif output_ready then
             -- Output transaction has occured, but no input transaction
             output_valid <= '0';
+
             state <= wait_for_input_valid;
+
           elsif input_valid then
             -- Input transaction has occured, but no output transaction
             -- Values from input transaction will be saved in the skid-aside buffer while we wait for output_ready.
             input_ready_int <= '0';
+
             state <= wait_for_output_ready;
           end if;
 
         when wait_for_output_ready =>
           if output_ready then
             -- output_valid is '1', so if we get here an output transaction has occured
             input_ready_int <= '1';
-            output_data <= input_data_skid;
+
             output_last <= input_last_skid;
+            output_data <= input_data_skid;
+            output_strobe <= input_strobe_skid;
+
             state <= full_handshake_throughput;
           end if;
       end case;
 
       if input_ready and input_valid then
-        input_data_skid <= input_data;
         input_last_skid <= input_last;
+        input_data_skid <= input_data;
+        input_strobe_skid <= input_strobe;
       end if;
     end process;
 
 
   ------------------------------------------------------------------------------
   elsif (not full_throughput) and allow_poor_input_ready_timing generate
 
@@ -160,16 +183,17 @@
 
     ------------------------------------------------------------------------------
     main : process
     begin
       wait until rising_edge(clk);
 
       output_valid <= input_valid and not (output_valid and output_ready);
-      output_data <= input_data;
       output_last <= input_last;
+      output_data <= input_data;
+      output_strobe <= input_strobe;
     end process;
 
 
   ------------------------------------------------------------------------------
   elsif (not full_throughput) and (not allow_poor_input_ready_timing) generate
 
     -- All signals are driven by registers, which results in the best timing but also the lowest
@@ -184,14 +208,15 @@
       wait until rising_edge(clk);
 
       input_ready <= output_ready and output_valid;
       -- Since there is a one cycle latency on output_valid, and a one cycle latency on input_ready,
       -- we have to stall for two cycles after a transaction, to allow the "input" master to update
       -- data and valid.
       output_valid <= input_valid and not (output_valid and output_ready) and not input_ready;
-      output_data <= input_data;
       output_last <= input_last;
+      output_data <= input_data;
+      output_strobe <= input_strobe;
     end process;
 
   end generate;
 
 end architecture;
```

### Comparing `tsfpga-8.0.1/modules/common/src/handshake_splitter.vhd` & `tsfpga-9.0.0/modules/common/src/handshake_splitter.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/common/src/periodic_pulser.vhd` & `tsfpga-9.0.0/modules/common/src/periodic_pulser.vhd`

 * *Files 0% similar despite different names*

```diff
@@ -132,24 +132,26 @@
         end if;
       end if;
     end process;
 
     pulse <= count_enable when tick_count = period - 1 else '0';
   end generate;
 
+
   ------------------------------------------------------------------------------
   -- Create one or more shift registers
   -- This generate is "else generate" with gen_counter, but "else generate"
   -- statements seem to fail recursive instantiation in Vivado.
   ------------------------------------------------------------------------------
   gen_shift_registers : if factors.num_factors_this_stage > 0 generate
     gen_mutual_prime_srls : for idx in factors.this_stage'range generate
       gen_only_if_not_0 : if factors.this_stage(idx) /= 0 generate
         -- Create a shift register of the length of the current factor factor
-        signal shift_reg : std_logic_vector(0 to factors.this_stage(idx) - 1) := (0 => '1', others => '0');
+        signal shift_reg : std_logic_vector(0 to factors.this_stage(idx) - 1) :=
+          (0 => '1', others => '0');
       begin
         shift : process
         begin
           wait until rising_edge(clk);
           if count_enable then
             shift_reg <= shift_reg(shift_reg'high) & shift_reg(0 to shift_reg'high - 1);
           end if;
```

### Comparing `tsfpga-8.0.1/modules/common/src/types_pkg.vhd` & `tsfpga-9.0.0/modules/common/src/types_pkg.vhd`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,35 @@
 library ieee;
 use ieee.numeric_std.all;
 use ieee.std_logic_1164.all;
 
 
 package types_pkg is
 
+  type slv_vec_t is array (integer range <>) of std_logic_vector;
+  type unsigned_vec_t is array (integer range <>) of unsigned;
+  type signed_vec_t is array (integer range <>) of signed;
+
   type natural_vec_t is array (integer range <>) of natural;
   type positive_vec_t is array (integer range <>) of positive;
   type boolean_vec_t is array (integer range <>) of boolean;
 
   function get_maximum(values : positive_vec_t) return positive;
 
   function to_sl(value : boolean) return std_logic;
   function to_bool(value : std_logic) return boolean;
   function to_bool(value : natural) return boolean;
 
   subtype binary_integer_t is integer range 0 to 1;
   function to_int(value : boolean) return binary_integer_t;
   function to_int(value : std_logic) return binary_integer_t;
 
+  subtype binary_real_t is real range 0.0 to 1.0;
+  function to_real(value : boolean) return binary_real_t;
+
   function swap_byte_order(data : std_logic_vector) return std_logic_vector;
   function swap_bit_order(data : std_logic_vector) return std_logic_vector;
 
   function count_ones(data : std_logic_vector) return natural;
 
 end package;
 
@@ -87,22 +94,26 @@
     end if;
   end function;
 
   function to_int(value : std_logic) return binary_integer_t is
   begin
     if value = '1' then
       return 1;
-    elsif value = '0' then
-      return 0;
     end if;
-
-    assert false report "Can not convert value " & to_string(value) severity warning;
     return 0;
   end function;
 
+  function to_real(value : boolean) return binary_real_t is
+  begin
+    if value then
+      return 1.0;
+    end if;
+    return 0.0;
+  end function;
+
   function swap_byte_order(data : std_logic_vector) return std_logic_vector is
     variable result : std_logic_vector(data'range);
     constant num_bytes : integer := data'length / 8;
     variable result_byte_idx : integer;
   begin
     -- Swap endianness of the input word.
     -- I.e., while maintaining the range and vector direction, swap the location of the data bytes.
```

### Comparing `tsfpga-8.0.1/modules/common/src/width_conversion.vhd` & `tsfpga-9.0.0/modules/common/src/keep_remover.vhd`

 * *Files 21% similar despite different names*

```diff
@@ -1,356 +1,360 @@
 -- -------------------------------------------------------------------------------------------------
 -- Copyright (c) Lukas Vik. All rights reserved.
 --
 -- This file is part of the tsfpga project.
 -- https://tsfpga.com
 -- https://gitlab.com/tsfpga/tsfpga
 -- -------------------------------------------------------------------------------------------------
--- Width conversion of a data bus. Can handle downconversion (wide to thin) or upconversion (thin
--- to wide). The data widths must be a power-of-two multiple of each other. E.g. 4->16 is
--- supported while 8->24 is not.
+-- This entity removes strobe'd out lanes from the input, resulting in an output stream where all
+-- lanes are always strobed (except for the last beat, potentially). The strobe on input can be
+-- considered as the TKEEP signal in AXI-Stream terminology, and the output strobe would be
+-- TKEEP/TSTRB.
 --
--- There is a generic to enable strobing of data. The data and strobe will be passed on from
--- 'input' to 'output' side as is. This means that there might be output words where all strobe
--- lanes are zero.
+-- The entity works by continously filling up a data buffer with data from the input. Only the lanes
+-- that are strobed will be saved to the buffer. Note that input words may have all their lanes
+-- strobed out (except for the last beat, see below).
+-- When enough lanes are saved to fill a whole word, data is passed to the output by asserting
+-- output_valid. When input_last is asserted for an input
+-- word, an output word will be sent out, with output_last asserted, even if a whole strobed word
+-- is not currently filled in the buffer.
 --
--- We have done some experimentation with removing words that are strobed out, so that they never
--- reach the 'output' side. See comments in code. It increases the resource utilization by a lot,
--- and it is not super clear if it is correct behavior for the common use case.
+-- The strobe unit data width is configurable via a generic. Most of the time it would be eight,
+-- i.e. a byte strobe. But in some cases the strobe represents a wider quanta, in which case the
+-- generic can be increased. Increasing the generic will drastically decrease the
+-- resourse utilization, since that is the "atom" of data that is handled internally.
 --
--- When upconverting, the 'input' side burst length must align with the 'output' side data width.
--- If it is not, then the 'input' stream must be padded.
--- Consider the example when converting 32->64, and 'last' is asserted in the third 'input' word.
--- Unless the 'support_unaligned_burst_length' generic is set there will still only be one word sent
--- to the 'output'. If the generic is set, however, the 'input' stream will be padded so that a
--- whole 'output' word is filled. The padded lanes will have their 'strobe' set to zero.
+-- The handling of input_last presents a corner case.
+-- Lets assume that data_width is 16 and strobe_unit_width is 8.
+-- Furthermore, there is one atom of data available in the buffer, and input stream has both lanes
+-- strobed. In this case, one input word shall result in two output words. The output word
+-- comes from a whole word being filled in the buffer. The second word comes from a half filled word
+-- in the buffer, but input_last being asserted.
+-- This is solved by having a small state machine that pads input data with an extra word when
+-- this corner case arises. The padding stage makes it possible to have a very simple data buffer
+-- stage, with low resource utilization.
+--
+-- The entity achieves full throughput, except for the corner case mentioned above, where it might
+-- stall one cycle on the input.
+--
+-- Limitations:
+--
+-- * 'input_last' may not be asserted on an input word that has all lanes strobed out.
+-- * There may never be a '1' above a '0' in the input strobe. E.g. "0111" is allowed,
+--   but "1100" is not.
 -- -------------------------------------------------------------------------------------------------
 
 library ieee;
-use ieee.std_logic_1164.all;
-use ieee.numeric_std.all;
+context ieee.ieee_std_context;
 
-use work.types_pkg.all;
+library common;
+use common.types_pkg.all;
 
 
-entity width_conversion is
+entity keep_remover is
   generic (
-    input_width : positive;
-    output_width : positive;
-    -- Enable usage of the 'input_strobe' and 'output_strobe' ports.
-    -- Will increase the logic footprint.
-    enable_strobe : boolean := false;
-    -- In the typical use case where we want a "byte strobe", this would be set to 8.
-    -- In other cases, for example when the data is packed, we migh use a higher value.
-    -- Must assign a positive value if 'enable_strobe' is true.
-    strobe_unit_width : integer := -1;
-    -- Enable if 'input' burst lengths are not a multiple of the 'output' width.
-    -- Will increase the logic footprint.
-    support_unaligned_burst_length : boolean := false
+    data_width : positive;
+    strobe_unit_width : positive
   );
   port (
     clk : in std_logic;
     --
-    input_ready : out std_logic := '1';
+    input_ready : out std_logic := '0';
     input_valid : in std_logic;
     input_last : in std_logic;
-    input_data : in std_logic_vector(input_width - 1 downto 0);
-    -- Optional word strobe. Must set 'enable_strobe' generic in order to use this.
-    input_strobe : in std_logic_vector(input_width / strobe_unit_width - 1 downto 0) :=
-      (others => '1');
+    input_data : in std_logic_vector(data_width - 1 downto 0);
+    input_keep : in std_logic_vector(data_width / strobe_unit_width - 1 downto 0);
     --
     output_ready : in std_logic;
     output_valid : out std_logic := '0';
-    output_last : out std_logic;
-    output_data : out std_logic_vector(output_width - 1 downto 0);
-    -- Optional word strobe. Must set 'enable_strobe' generic in order to use this.
-    output_strobe : out std_logic_vector(output_width / strobe_unit_width - 1 downto 0) :=
-      (others => '1')
+    output_last : out std_logic := '0';
+    output_data : out std_logic_vector(data_width - 1 downto 0) := (others => '0');
+    output_strobe : out std_logic_vector(data_width / strobe_unit_width - 1 downto 0) :=
+      (others => '0')
   );
 end entity;
 
-architecture a of width_conversion is
+architecture a of keep_remover is
 
-  function get_atom_width return positive is
-  begin
-    if enable_strobe then
-      assert strobe_unit_width > 0
-        report "Must set a valid strobe width when strobing is enabled."
-        severity failure;
-      return strobe_unit_width;
-    end if;
-
-    -- When converting e.g. 16->32 the data atom that is handled internally will be of width 16.
-    -- This gives lower resource utilization than if it was e.g. always 8.
-    return minimum(input_width, output_width);
-  end function;
-  constant atom_width : positive := get_atom_width;
-  subtype atom_range is natural range atom_width - 1 downto 0;
-
-  constant num_atoms_per_input : positive := input_width / atom_width;
-  constant num_atoms_per_output : positive := output_width / atom_width;
-
-  -- +1 for last
-  constant packed_atom_width : positive := atom_width + 1 + to_int(enable_strobe);
-  constant stored_atom_count_max : positive := num_atoms_per_input + num_atoms_per_output;
-
-  constant shift_reg_length : positive := stored_atom_count_max * packed_atom_width;
-  signal shift_reg : std_logic_vector(shift_reg_length - 1 downto 0) := (others => '0');
-
-  signal num_atoms_stored : natural range 0 to stored_atom_count_max := 0;
-
-  impure function pack(
-    atom_data : std_logic_vector(atom_range);
-    atom_strobe : std_logic;
-    atom_last : std_logic
-  ) return std_logic_vector is
-    variable result : std_logic_vector(packed_atom_width - 1 downto 0) := (others => '0');
-  begin
-    result(atom_data'range) := atom_data;
+  -- The unit of data that we will be working with
+  constant atom_width : positive := strobe_unit_width;
 
-    if enable_strobe then
-      result(result'high - 1) := atom_strobe;
-    end if;
+  -- +1 for 'strobe' bit and 'last' bit
+  constant packed_atom_width : positive := atom_width + 1 + 1;
 
-    result(result'high) := atom_last;
-
-    return result;
-  end function;
-
-  procedure unpack(
-    packed : in std_logic_vector(packed_atom_width - 1 downto 0);
-    atom_data : out std_logic_vector(atom_range);
-    atom_strobe : out std_logic;
-    atom_last : out std_logic
-  ) is
-  begin
-    atom_data := packed(atom_data'range);
-
-    if enable_strobe then
-      atom_strobe := packed(packed'high - 1);
-    end if;
+  constant num_atoms_per_word : positive := input_keep'length;
 
-    atom_last := packed(packed'high);
-  end procedure;
+  -- Since there is a pipeline step in this entity, we must be able to hold at least two maximum
+  -- size input words in order to preserve full throughput.
+  constant max_num_words_in_buffer : positive := 2;
+  constant max_num_atoms_in_buffer : positive := max_num_words_in_buffer * num_atoms_per_word;
 
   signal padded_input_ready, padded_input_valid, padded_input_last : std_logic := '0';
   signal padded_input_data : std_logic_vector(input_data'range) := (others => '0');
-  signal padded_input_strobe : std_logic_vector(input_strobe'range) := (others => '0');
+  signal padded_input_keep : std_logic_vector(input_keep'range) := (others => '0');
 
-begin
+  signal num_atoms_in_buffer : natural range 0 to max_num_atoms_in_buffer := 0;
+  signal num_atoms_written_in_current_word : natural range 0 to num_atoms_per_word := 0;
 
-  ------------------------------------------------------------------------------
-  assert input_width /= output_width
-    report "Do not use this module with equal widths" severity failure;
+begin
 
-  assert input_width mod output_width = 0 or output_width mod input_width = 0
-    report "Larger width has to be multiple of smaller." severity failure;
+  assert data_width mod strobe_unit_width = 0
+    report "Data width must be a multiple of strobe unit width." severity failure;
 
-  assert (output_width / input_width) mod 2 = 0 and (input_width / output_width) mod 2 = 0
-    report "Larger width has to be power of two multiple of smaller." severity failure;
 
-  assert strobe_unit_width > 0 or not enable_strobe
-    report "Must set a valid strobe width when strobing is enabled." severity failure;
+  ------------------------------------------------------------------------------
+  assert_input : process
+  begin
+    wait until input_valid = '1' and rising_edge(clk);
 
-  assert input_width < output_width or not support_unaligned_burst_length
-    report "Unaligned burst length only makes sense when upconverting." severity failure;
+    assert (or input_keep) or not input_last report
+      "'last' may not be asserted on a strobed out word";
 
-  assert enable_strobe or not support_unaligned_burst_length
-    report "Must enable strobing when doing unaligned bursts." severity failure;
+    for strobe_idx in input_keep'range loop
+      if input_keep(strobe_idx) = '0' then
+        assert (or input_keep(input_keep'high downto strobe_idx)) = '0'
+          report "There must never be a '1' above a '0' in the input strobe";
+      end if;
+    end loop;
+  end process;
 
 
   ------------------------------------------------------------------------------
-  pad_input_data_generate : if support_unaligned_burst_length generate
+  pad_block : block
+    signal num_atoms_strobed : natural range 0 to num_atoms_per_word := 0;
 
-    type state_t is (let_data_pass, send_padding);
-    signal state : state_t := let_data_pass;
+    signal num_atoms_written_in_current_word_plus_this_write :
+      natural range 0 to 2 * num_atoms_per_word - 1 := 0;
 
-    constant input_beats_per_output_beat : natural := output_width / input_width;
-    signal output_words_filled : natural range 0 to input_beats_per_output_beat := 0;
+    signal last_input_needs_padding : std_logic := '0';
 
+    type state_t is (let_data_pass, handle_last);
+    signal state : state_t := let_data_pass;
   begin
 
-    ------------------------------------------------------------------------------
-    assign : process(all)
-    begin
-      padded_input_data <= input_data;
-      padded_input_last <= input_last;
-
-      if state = let_data_pass then
+    num_atoms_strobed <= count_ones(input_keep);
 
-        -- Passthrough.
-        input_ready <= padded_input_ready;
-        padded_input_valid <= input_valid;
-        padded_input_strobe <= input_strobe;
+    num_atoms_written_in_current_word <= num_atoms_in_buffer mod num_atoms_per_word;
 
-      else -- send_padding
+    num_atoms_written_in_current_word_plus_this_write <=
+      num_atoms_written_in_current_word + num_atoms_strobed;
 
-        input_ready <= '0';
-        padded_input_valid <= '1';
-        padded_input_strobe <= (others => '0');
-
-      end if;
-    end process;
+    -- The current input word, along with handling of last, will result in more than one
+    -- word being written to buffer
+    last_input_needs_padding <=
+      to_sl(num_atoms_written_in_current_word_plus_this_write > num_atoms_per_word);
 
 
     ------------------------------------------------------------------------------
-    pad_input_data : process
+    pad_input_fsm : process
     begin
-      wait until rising_edge(clk) and support_unaligned_burst_length;
-
-      if padded_input_ready and padded_input_valid then
-        if output_words_filled = input_beats_per_output_beat then
-          output_words_filled <= 1;
-        else
-          output_words_filled <= output_words_filled + 1;
-        end if;
-      end if;
+      wait until rising_edge(clk);
 
       case state is
         when let_data_pass =>
-          if (
-            padded_input_ready = '1'
-            and padded_input_valid = '1'
-            and padded_input_last = '1'
-            and output_words_filled /= input_beats_per_output_beat - 1
-          ) then
-            state <= send_padding;
+          if
+            padded_input_ready
+            and padded_input_valid
+            and input_last
+            and last_input_needs_padding
+          then
+            state <= handle_last;
           end if;
 
-        when send_padding =>
+        when handle_last =>
+        -- Let one extra word pass and then go back to default state
           if padded_input_ready and padded_input_valid then
-            if output_words_filled = input_beats_per_output_beat - 1 then
-              -- This transaction fills the last words out the output.
-              state <= let_data_pass;
-            end if;
+            state <= let_data_pass;
           end if;
 
       end case;
     end process;
 
-  else generate
 
-    -- Passthrough.
-    input_ready <= padded_input_ready;
-    padded_input_valid <= input_valid;
-    padded_input_last <= input_last;
-    padded_input_data <= input_data;
-    padded_input_strobe <= input_strobe;
+    ------------------------------------------------------------------------------
+    pad_input_assign : process(all)
+    begin
+      padded_input_data <= input_data;
+
+      case state is
+        when let_data_pass =>
+          input_ready <= padded_input_ready;
 
-  end generate;
+          padded_input_valid <= input_valid;
+
+          padded_input_keep <= input_keep;
+
+          if input_valid and input_last and last_input_needs_padding then
+            -- We will send an extra word, where 'last' will be asserted
+            padded_input_last <= '0';
+          else
+            padded_input_last <= input_last;
+          end if;
+
+        when handle_last =>
+          input_ready <= '0';
+
+          padded_input_valid <= '1';
+
+          -- None of these atoms should be sent to output, they are all padding
+          padded_input_keep <= (others => '0');
+          padded_input_last <= '1';
+      end case;
+
+    end process;
+
+  end block;
 
 
   ------------------------------------------------------------------------------
-  main : process
-    variable num_atoms_next : natural range 0 to stored_atom_count_max;
+  processing_block : block
 
-    variable atom_strobe, atom_last : std_logic := '0';
-    variable num_atoms_strobed : natural range 0 to num_atoms_per_input := num_atoms_per_input;
+    -- Data buffer as a long SLV, containing many packed atoms.
+    -- Note that an array of records (data, strobe, last) result in greater resource utilization
+    -- that this SLV.
+    constant data_buffer_length : positive := max_num_atoms_in_buffer * packed_atom_width;
+    signal data_buffer : std_logic_vector(data_buffer_length - 1 downto 0) := (others => '0');
+
+    subtype atom_pointer_t is natural range 0 to max_num_atoms_in_buffer - 1;
+    subtype word_pointer_t is natural range 0 to max_num_words_in_buffer - 1;
+
+    signal write_pointer : atom_pointer_t := 0;
+    -- We always read whole words, so a narrower pointer can be used
+    signal read_pointer : word_pointer_t := 0;
+
+    function pack(
+      atom_data : std_logic_vector(atom_width - 1 downto 0);
+      atom_strobe : std_logic;
+      atom_last : std_logic
+    ) return std_logic_vector is
+      variable result : std_logic_vector(packed_atom_width - 1 downto 0) := (others => '0');
+    begin
+      result(atom_data'range) := atom_data;
+      result(result'high - 1) := atom_strobe;
+      result(result'high) := atom_last;
+
+      return result;
+    end function;
+
+    procedure unpack(
+      packed : in std_logic_vector(packed_atom_width - 1 downto 0);
+      atom_data : out std_logic_vector(atom_width - 1 downto 0);
+      atom_strobe : out std_logic;
+      atom_last : out std_logic
+    ) is
+    begin
+      atom_data := packed(atom_data'range);
+      atom_strobe := packed(packed'high - 1);
+      atom_last := packed(packed'high);
+    end procedure;
 
-    variable packed_data_to_shift_in : std_logic_vector(packed_atom_width - 1 downto 0) :=
-      (others => '0');
-    variable shift_reg_next : std_logic_vector(shift_reg'range) := (others => '0');
   begin
-    wait until rising_edge(clk);
 
-    num_atoms_next := num_atoms_stored;
+    ------------------------------------------------------------------------------
+    main : process
+      variable atom_write_idx : atom_pointer_t := 0;
 
-    shift_reg_next := shift_reg;
-    if padded_input_ready and padded_input_valid then
-      if enable_strobe then
-        num_atoms_strobed := count_ones(padded_input_strobe);
-      end if;
+      variable data_to_write : std_logic_vector(atom_width - 1 downto 0) := (others => '0');
+      variable strobe_to_write, last_to_write : std_logic := '0';
 
-      -- In order to remove words that are strobed out, num_atoms_strobed could be used instead
-      -- of num_atoms_per_input below. This increases the LUT usage by a factor of four.
-      num_atoms_next := num_atoms_next + num_atoms_per_input;
-
-      for input_atom_idx in 0 to num_atoms_per_input - 1 loop
-        if enable_strobe then
-          -- When strobing, the atom size is always one strobe unit, so this indexing works.
-          atom_strobe := padded_input_strobe(input_atom_idx);
-        end if;
+      variable packed_atom : std_logic_vector(packed_atom_width - 1 downto 0) := (others => '0');
+      variable data_buffer_next : std_logic_vector(data_buffer'range) := (others=> '0');
 
-        -- Set 'last' only on the last strobed atom of the input word.
-        if input_atom_idx = num_atoms_strobed - 1 then
-          atom_last := padded_input_last;
-        else
-          atom_last := '0';
-        end if;
+      variable num_atoms_needed_to_fill_current_word : natural := 0;
 
-        packed_data_to_shift_in := pack(
-          atom_data=>padded_input_data(
-            (input_atom_idx + 1) * atom_width - 1 downto input_atom_idx * atom_width
-          ),
-          atom_strobe=>atom_strobe,
-          atom_last=>atom_last
+      variable num_atoms_to_read, num_atoms_to_write : natural range 0 to num_atoms_per_word := 0;
+      variable num_words_to_read : natural range 0 to 1 := 0;
+    begin
+      wait until rising_edge(clk);
+
+      -- Note that all atoms are written to the buffer, but the write pointer is only incremented
+      -- with the number of atoms that are strobed.
+      data_buffer_next := data_buffer;
+      for atom_idx in 0 to num_atoms_per_word - 1 loop
+        atom_write_idx := (write_pointer + atom_idx) mod max_num_atoms_in_buffer;
+
+        data_to_write := padded_input_data((atom_idx + 1) * atom_width - 1 downto atom_idx * atom_width);
+        strobe_to_write := padded_input_keep(atom_idx);
+        last_to_write := padded_input_last;
+
+        packed_atom := pack(
+          data_to_write,
+          strobe_to_write,
+          last_to_write
         );
-        shift_reg_next :=
-          packed_data_to_shift_in
-          & shift_reg_next(shift_reg_next'left downto packed_data_to_shift_in'length);
+
+        data_buffer_next(
+          (atom_write_idx + 1) * packed_atom_width - 1 downto atom_write_idx * packed_atom_width
+        ) := packed_atom;
       end loop;
-    end if;
-    shift_reg <= shift_reg_next;
 
-    if output_ready and output_valid then
-      num_atoms_next := num_atoms_next - num_atoms_per_output;
-    end if;
+      num_atoms_to_write := 0;
+      if padded_input_ready and padded_input_valid then
+        if padded_input_last then
+          num_atoms_needed_to_fill_current_word :=
+            num_atoms_per_word - num_atoms_written_in_current_word;
 
-    num_atoms_stored <= num_atoms_next;
-  end process;
+          num_atoms_to_write := num_atoms_needed_to_fill_current_word;
 
-  padded_input_ready <= to_sl(num_atoms_stored <= stored_atom_count_max - num_atoms_per_input);
+          assert num_atoms_to_write >= count_ones(padded_input_keep);
+        else
+          num_atoms_to_write := count_ones(padded_input_keep);
+        end if;
 
+        data_buffer <= data_buffer_next;
+      end if;
 
-  ------------------------------------------------------------------------------
-  slice_output : process(all)
-    variable output_atoms_base : natural range 0 to stored_atom_count_max := 0;
+      num_atoms_to_read := 0;
+      num_words_to_read := 0;
+      if output_ready and output_valid then
+        num_atoms_to_read := num_atoms_per_word;
+        num_words_to_read := 1;
+      end if;
 
-    variable packed_atom : std_logic_vector(packed_atom_width - 1 downto 0) := (others => '0');
+      write_pointer <= (write_pointer + num_atoms_to_write) mod max_num_atoms_in_buffer;
 
-    variable atom_data : std_logic_vector(atom_width - 1 downto 0) := (others => '0');
-    variable atom_strobe, atom_last : std_logic_vector(num_atoms_per_output - 1 downto 0) :=
-      (others => '0');
-  begin
-    output_valid <= to_sl(num_atoms_stored >= num_atoms_per_output);
+      read_pointer <= (read_pointer + num_words_to_read) mod max_num_words_in_buffer;
 
-    output_atoms_base := stored_atom_count_max - num_atoms_stored;
+      num_atoms_in_buffer <=
+        num_atoms_in_buffer
+        + num_atoms_to_write
+        - num_atoms_to_read;
+    end process;
 
-    for output_atom_idx in 0 to num_atoms_per_output - 1 loop
-      if output_atom_idx < num_atoms_stored then
-        packed_atom := shift_reg(
-          (output_atoms_base + output_atom_idx + 1) * packed_atom_width - 1
-          downto (output_atoms_base + output_atom_idx) * packed_atom_width
-        );
+    padded_input_ready <=
+      to_sl(num_atoms_in_buffer <= (max_num_atoms_in_buffer - num_atoms_per_word));
+
+    output_valid <= to_sl(num_atoms_in_buffer >= num_atoms_per_word);
+
+
+    ------------------------------------------------------------------------------
+    assign_output : process(all)
+      variable atom_read_idx : atom_pointer_t := 0;
 
-        unpack(
-          packed=>packed_atom,
-          atom_data=>atom_data,
-          atom_strobe=>atom_strobe(output_atom_idx),
-          atom_last=>atom_last(output_atom_idx)
+      variable packed_atom : std_logic_vector(packed_atom_width - 1 downto 0) := (others => '0');
+      variable unpacked_data : std_logic_vector(atom_width - 1 downto 0) := (others => '0');
+      variable unpacked_strobe, unpacked_last : std_logic := '0';
+
+      variable is_last : std_logic := '0';
+    begin
+      is_last := '0';
+
+      for atom_idx in 0 to num_atoms_per_word - 1 loop
+        atom_read_idx := read_pointer * num_atoms_per_word + atom_idx;
+
+        packed_atom := data_buffer(
+          (atom_read_idx + 1) * packed_atom_width - 1 downto atom_read_idx * packed_atom_width
         );
+        unpack(packed_atom, unpacked_data, unpacked_strobe, unpacked_last);
 
-        output_data((output_atom_idx + 1) * atom_width - 1 downto output_atom_idx * atom_width) <=
-          atom_data;
-      else
-
-        -- This is just so that the indexing does not go out of range. When the condition for
-        -- output_valid is met, we will not end up here for any atom.
-        output_data((output_atom_idx + 1) * atom_width - 1 downto output_atom_idx * atom_width) <=
-          (others => '-');
-        atom_strobe(output_atom_idx) := '-';
-        atom_last(output_atom_idx) := '-';
+        output_data((atom_idx + 1) * atom_width - 1 downto atom_idx * atom_width) <= unpacked_data;
+        output_strobe(atom_idx) <= unpacked_strobe;
 
-      end if;
-    end loop;
+        is_last := is_last or unpacked_last;
+      end loop;
 
-    if enable_strobe then
-      -- The top atome might be strobed out and not have 'last' set. Instead it is found in one of
-      -- the lower atoms.
-      output_last <= or atom_last;
-      output_strobe <= atom_strobe;
-    else
-      output_last <= atom_last(atom_last'high);
-    end if;
-  end process;
+      output_last <= is_last;
+    end process;
+
+  end block;
 
 end architecture;
```

### Comparing `tsfpga-8.0.1/modules/common/test/tb_addr_pkg.vhd` & `tsfpga-9.0.0/modules/common/test/tb_addr_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/common/test/tb_clock_counter.vhd` & `tsfpga-9.0.0/modules/common/test/tb_clock_counter.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/common/test/tb_debounce.vhd` & `tsfpga-9.0.0/modules/common/test/tb_debounce.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/common/test/tb_handshake_pipeline.vhd` & `tsfpga-9.0.0/modules/common/test/tb_handshake_pipeline.vhd`

 * *Files 21% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 use vunit_lib.random_pkg.all;
 context vunit_lib.vunit_context;
 context vunit_lib.vc_context;
 
 library osvvm;
 use osvvm.RandomPkg.all;
 
+library bfm;
+
 use work.types_pkg.all;
 
 
 entity tb_handshake_pipeline is
   generic (
     full_throughput : boolean;
     allow_poor_input_ready_timing : boolean;
@@ -31,173 +33,174 @@
 end entity;
 
 architecture tb of tb_handshake_pipeline is
 
   signal clk : std_logic := '0';
   constant clk_period : time := 10 ns;
 
-  constant data_width : integer := 16;
+  constant data_width : positive := 16;
+  constant bytes_per_beat : positive := data_width / 8;
 
   signal input_ready, input_valid, input_last : std_logic := '0';
   signal output_ready, output_valid, output_last : std_logic := '0';
+
   signal input_data, output_data : std_logic_vector(data_width - 1 downto 0) := (others => '0');
+  signal input_strobe, output_strobe : std_logic_vector(data_width / 8 - 1 downto 0) :=
+    (others => '0');
 
-  constant num_words : integer := 1024;
+  constant input_data_queue, output_data_queue : queue_t := new_queue;
 
   constant stall_config : stall_config_t := (
     stall_probability => 0.5 * real(to_int(data_jitter)),
     min_stall_cycles => 1,
     max_stall_cycles => 2
   );
 
-  constant input_master : axi_stream_master_t := new_axi_stream_master(
-    data_length => input_data'length,
-    protocol_checker => new_axi_stream_protocol_checker(
-      logger => get_logger("input_master"),
-      data_length => input_data'length
-    ),
-    stall_config => stall_config
-  );
+  signal num_output_bursts_checked : natural := 0;
 
-  constant output_slave : axi_stream_slave_t := new_axi_stream_slave(
-    data_length => input_data'length,
-    protocol_checker => new_axi_stream_protocol_checker(
-      logger => get_logger("output_slave"),
-      data_length => output_data'length
-    ),
-    stall_config => stall_config
-  );
-
-  signal start, stimuli_done, data_check_done : boolean := false;
+  constant full_throughput_num_beats : positive := 1024;
 
 begin
 
   test_runner_watchdog(runner, 2 ms);
   clk <= not clk after clk_period / 2;
 
 
   ------------------------------------------------------------------------------
   main : process
     variable rnd : RandomPType;
+    variable num_output_bursts_expected : natural := 0;
 
-    procedure run_test is
-      variable data : integer_array_t := null_integer_array;
-
-      variable reference_data, got_data : std_logic_vector(input_data'range) := (others => '0');
-      variable got_last : std_logic := '0';
-
-      variable axi_stream_pop_reference : axi_stream_reference_t;
-      variable axi_stream_pop_reference_queue : queue_t := new_queue;
+    procedure run_test(fixed_length_beats : natural := 0) is
+      variable burst_length_bytes : positive := 1;
+      variable data_in, data_out : integer_array_t := null_integer_array;
     begin
-      report "Starting test";
-      data := random_integer_array(width=>num_words, bits_per_word=>data_width, is_signed=>false);
+      if fixed_length_beats /= 0 then
+        burst_length_bytes := fixed_length_beats * bytes_per_beat;
 
-      for word_idx in 0 to length(data) - 1 loop
-        reference_data := std_logic_vector(to_unsigned(get(data, word_idx), reference_data'length));
-        push_axi_stream(
-          net,
-          input_master,
-          tdata=>reference_data,
-          tlast=>to_sl(word_idx=length(data) - 1)
-        );
-      end loop;
+      else
+        -- Set a random length, up to a number of words
+        burst_length_bytes := rnd.RandInt(1, 5 * bytes_per_beat);
+      end if;
+
+      random_integer_array(
+        rnd => rnd,
+        integer_array => data_in,
+        width => burst_length_bytes,
+        bits_per_word => 8,
+        is_signed => false
+      );
+      data_out := copy(data_in);
 
-      -- Queue up reads in order to get full throughput. We need to keep track of
-      -- the pop_reference when we read the reply later. Hence it is pushed to a queue.
-      for word_idx in 0 to length(data) - 1 loop
-        pop_axi_stream(net, output_slave, axi_stream_pop_reference);
-        push(axi_stream_pop_reference_queue, axi_stream_pop_reference);
-      end loop;
+      push_ref(input_data_queue, data_in);
+      push_ref(output_data_queue, data_out);
 
-      for word_idx in 0 to length(data) - 1 loop
-        axi_stream_pop_reference := pop(axi_stream_pop_reference_queue);
-        await_pop_axi_stream_reply(
-          net,
-          axi_stream_pop_reference,
-          tdata=>got_data,
-          tlast=>got_last
-        );
-
-        reference_data := std_logic_vector(to_unsigned(get(data, word_idx), reference_data'length));
-        check_equal(got_data, reference_data, "word_idx=" & to_string(word_idx));
-        check_equal(got_last, word_idx = num_words - 1);
-      end loop;
+      num_output_bursts_expected := num_output_bursts_expected + 1;
+    end procedure;
+
+    procedure wait_until_done is
+    begin
+      wait until
+        is_empty(input_data_queue)
+        and is_empty(output_data_queue)
+        and num_output_bursts_checked = num_output_bursts_expected
+        and rising_edge(clk);
+      wait until rising_edge(clk);
     end procedure;
 
     variable start_time, time_diff : time;
 
   begin
     test_runner_setup(runner, runner_cfg);
     rnd.InitSeed(rnd'instance_name);
 
     -- Decrease noise
     disable(get_logger("input_master:rule 4"), warning);
     disable(get_logger("output_slave:rule 4"), warning);
 
     if run("test_random_data") then
-      run_test;
-      run_test;
-      run_test;
-      run_test;
+      for idx in 0 to 300 loop
+        run_test;
+      end loop;
+
+      wait_until_done;
 
     elsif run("test_full_throughput") then
       start_time := now;
-      run_test;
-      time_diff := now - start_time;
 
-      check_relation(time_diff < (num_words + 3) * clk_period);
+      run_test(fixed_length_beats=>full_throughput_num_beats);
+      wait_until_done;
+
+      time_diff := now - start_time;
+      check_relation(time_diff < (full_throughput_num_beats + 4) * clk_period);
     end if;
 
     test_runner_cleanup(runner);
   end process;
 
 
   ------------------------------------------------------------------------------
-  axi_stream_master_inst : entity vunit_lib.axi_stream_master
-    generic map(
-      master => input_master
+  axi_stream_master_inst : entity bfm.axi_stream_master
+    generic map (
+      data_width_bits => input_data'length,
+      data_queue => input_data_queue,
+      stall_config => stall_config,
+      logger_name_suffix => "_input",
+      strobe_unit_width_bits => input_data'length / input_strobe'length
     )
-    port map(
-      aclk => clk,
-      tvalid => input_valid,
-      tready => input_ready,
-      tdata => input_data,
-      tlast => input_last
+    port map (
+      clk => clk,
+      --
+      ready => input_ready,
+      valid => input_valid,
+      last => input_last,
+      data => input_data,
+      strobe => input_strobe
     );
 
 
   ------------------------------------------------------------------------------
-  axi_stream_slave_inst : entity vunit_lib.axi_stream_slave
-    generic map(
-      slave => output_slave
+  axi_stream_slave_inst : entity bfm.axi_stream_slave
+    generic map (
+      data_width_bits => output_data'length,
+      reference_data_queue => output_data_queue,
+      stall_config => stall_config,
+      logger_name_suffix => "_output"
     )
-    port map(
-      aclk => clk,
-      tvalid => output_valid,
-      tready => output_ready,
-      tdata => output_data,
-      tlast => output_last
+    port map (
+      clk => clk,
+      --
+      ready => output_ready,
+      valid => output_valid,
+      last => output_last,
+      data => output_data,
+      strobe => output_strobe,
+      --
+      num_bursts_checked => num_output_bursts_checked
     );
 
 
   ------------------------------------------------------------------------------
   dut : entity work.handshake_pipeline
     generic map (
       data_width => data_width,
       full_throughput => full_throughput,
-      allow_poor_input_ready_timing => allow_poor_input_ready_timing
+      allow_poor_input_ready_timing => allow_poor_input_ready_timing,
+      strobe_unit_width => input_data'length / input_strobe'length
     )
     port map (
       clk => clk,
       --
       input_ready => input_ready,
       input_valid => input_valid,
       input_last => input_last,
       input_data => input_data,
+      input_strobe => input_strobe,
       --
       output_ready => output_ready,
       output_valid => output_valid,
       output_last => output_last,
-      output_data => output_data
+      output_data => output_data,
+      output_strobe => output_strobe
     );
 
 end architecture;
```

### Comparing `tsfpga-8.0.1/modules/common/test/tb_handshake_splitter.vhd` & `tsfpga-9.0.0/modules/common/test/tb_handshake_splitter.vhd`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 library vunit_lib;
 context vunit_lib.vunit_context;
 context vunit_lib.vc_context;
 
 library osvvm;
 use osvvm.RandomPkg.all;
 
+library common;
+
 use work.types_pkg.all;
 
 
 entity tb_handshake_splitter is
   generic (
     runner_cfg : string
   );
@@ -96,24 +98,25 @@
     assert is_empty(data_queue0);
     data_check0_done <= true;
     wait;
   end process;
 
 
   ------------------------------------------------------------------------------
-  output0_axi_stream_protocol_checker_inst : entity vunit_lib.axi_stream_protocol_checker
+  output0_axi_stream_protocol_checker_inst : entity common.axi_stream_protocol_checker
     generic map (
-      protocol_checker => new_axi_stream_protocol_checker(
-        logger => get_logger("output0"), data_length => input_data'length)
+      data_width => input_data'length,
+      logger_name_suffix => "_output0"
     )
     port map (
-      aclk => clk,
-      tvalid => output0_valid,
-      tready => output0_ready,
-      tdata => input_data
+      clk => clk,
+      --
+      ready => output0_ready,
+      valid => output0_valid,
+      data => input_data
     );
 
 
   ------------------------------------------------------------------------------
   data_check1 : process
     variable data : std_logic_vector(input_data'range) := (others => '0');
   begin
@@ -133,26 +136,28 @@
     assert is_empty(data_queue1);
     data_check1_done <= true;
     wait;
   end process;
 
 
   ------------------------------------------------------------------------------
-  output1_axi_stream_protocol_checker_inst : entity vunit_lib.axi_stream_protocol_checker
+  output1_axi_stream_protocol_checker_inst : entity common.axi_stream_protocol_checker
     generic map (
-      protocol_checker => new_axi_stream_protocol_checker(
-        logger => get_logger("output1"), data_length => input_data'length)
+      data_width => input_data'length,
+      logger_name_suffix => "_output1"
     )
     port map (
-      aclk => clk,
-      tvalid => output1_valid,
-      tready => output1_ready,
-      tdata => input_data
+      clk => clk,
+      --
+      ready => output1_ready,
+      valid => output1_valid,
+      data => input_data
     );
 
+
   ------------------------------------------------------------------------------
   axi_stream_master_inst : entity vunit_lib.axi_stream_master
   generic map(
     master => axi_stream_master
   )
   port map(
     aclk   => clk,
```

### Comparing `tsfpga-8.0.1/modules/common/test/tb_periodic_pulser.vhd` & `tsfpga-9.0.0/modules/common/test/tb_periodic_pulser.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/common/test/tb_types_pkg.vhd` & `tsfpga-9.0.0/modules/common/test/tb_types_pkg.vhd`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     constant bit_data3_swapped : std_logic_vector(bit_data2'range) := "010101";
 
     variable positive_vec : positive_vec_t(0 to 3) := (others => 1);
 
   begin
     test_runner_setup(runner, runner_cfg);
 
-
     if run("test_get_maximum_positive") then
       positive_vec := (1, 1, 1, 1);
       check_equal(get_maximum(positive_vec), 1);
 
       positive_vec := (4, 3, 2, 1);
       check_equal(get_maximum(positive_vec), 4);
 
@@ -62,14 +61,25 @@
       check_equal(to_bool('0'), false);
       check_equal(to_bool('1'), true);
 
     elsif run("test_to_bool_integer") then
       check_equal(to_bool(0), false);
       check_equal(to_bool(1), true);
 
+    elsif run("test_to_int_std_logic") then
+      check_equal(to_int('0'), 0);
+      check_equal(to_int('-'), 0);
+      check_equal(to_int('X'), 0);
+      check_equal(to_int('H'), 0);
+      check_equal(to_int('1'), 1);
+
+    elsif run("test_to_real_bool") then
+      check_equal(to_real(true), 1.0);
+      check_equal(to_real(false), 0.0);
+
     elsif run("test_swap_byte_order") then
       byte_data0 := swap_byte_order(byte_data0);
       check_equal(byte_data0, byte_data0_swapped);
       check_equal(byte_data0'high, 4 * 8 - 1);
       check_equal(byte_data0'low, 0);
       check_equal(byte_data0'left, byte_data0'high);
       check_equal(byte_data0'right, byte_data0'low);
```

### Comparing `tsfpga-8.0.1/modules/common/test/tb_width_conversion.vhd` & `tsfpga-9.0.0/modules/common/test/tb_width_conversion.vhd`

 * *Files 23% similar despite different names*

```diff
@@ -7,37 +7,47 @@
 -- -------------------------------------------------------------------------------------------------
 
 library ieee;
 use ieee.std_logic_1164.all;
 use ieee.numeric_std.all;
 
 library vunit_lib;
+use vunit_lib.random_pkg.all;
+context vunit_lib.vc_context;
 context vunit_lib.vunit_context;
 
 library osvvm;
 use osvvm.RandomPkg.all;
 
+library bfm;
+
 use work.types_pkg.all;
 
 
 entity tb_width_conversion is
   generic (
     input_width : positive;
     output_width : positive;
     enable_strobe : boolean;
+    enable_last : boolean;
     support_unaligned_burst_length : boolean := false;
-    data_jitter : boolean := true;
+    enable_jitter : boolean := true;
     runner_cfg : string
   );
 end entity;
 
 architecture tb of tb_width_conversion is
 
   constant input_bytes_per_beat : positive := input_width / 8;
   constant output_bytes_per_beat : positive := output_width / 8;
+  constant minimum_width_bytes : positive := minimum(input_bytes_per_beat, output_bytes_per_beat);
+  constant maximum_width_bytes : positive := maximum(input_bytes_per_beat, output_bytes_per_beat);
+
+  constant is_upconversion : boolean := output_width > input_width;
+  constant is_downconversion : boolean := output_width < input_width;
 
   signal clk : std_logic := '0';
   constant clk_period : time := 10 ns;
 
   signal input_ready, input_valid, input_last : std_logic := '0';
   signal output_ready, output_valid, output_last : std_logic := '0';
 
@@ -46,205 +56,190 @@
 
   constant strobe_unit_width : positive := 8;
   signal input_strobe : std_logic_vector(input_width / strobe_unit_width - 1 downto 0) :=
     (others => '0');
   signal output_strobe : std_logic_vector(output_width / strobe_unit_width - 1 downto 0) :=
     (others => '0');
 
-  -- If there is strobing, there will be more words, but the amount of enabled bytes will be
-  -- the same in the end.
-  constant num_bytes_per_test : positive := 64;
-  constant num_test_loops : positive := 100;
+  constant input_data_queue, output_data_queue : queue_t := new_queue;
 
-  signal num_stimuli_done, num_data_check_done : natural := 0;
+  constant stall_config : stall_config_t := (
+    stall_probability => 0.2 * to_real(enable_jitter),
+    min_stall_cycles => 1,
+    max_stall_cycles => 4
+  );
 
-  procedure random_slv(rnd : inout RandomPType; data : out std_logic_vector) is
-    variable random_sl : std_logic_vector(0 downto 0);
-  begin
-    -- Build up a word from LSB to MSB, which corresponds to little endian when
-    -- comparing wide words with packed thin words.
-    for i in 0 to data'length - 1 loop
-      random_sl := rnd.RandSlv(1);
-      data(i) := random_sl(0);
-    end loop;
-  end procedure;
+  signal num_output_bursts_checked : natural := 0;
 
 begin
 
-  test_runner_watchdog(runner, 2 ms);
+  test_runner_watchdog(runner, 200 us);
   clk <= not clk after clk_period / 2;
 
 
   ------------------------------------------------------------------------------
   main : process
     variable rnd : RandomPType;
+    variable num_output_bursts_expected : natural := 0;
 
-    variable start_time, time_diff : time;
-
-  constant num_input_words_when_no_strobing : positive := num_bytes_per_test / (input_width / 8);
-  constant num_output_words_when_no_strobing : integer :=
-    num_input_words_when_no_strobing * input_width / output_width;
-  constant num_cycles_when_no_stall_and_no_strobing : integer :=
-    maximum(num_input_words_when_no_strobing, num_output_words_when_no_strobing);
-
-  begin
-    test_runner_setup(runner, runner_cfg);
-    rnd.InitSeed(rnd'instance_name);
-
-    if run("test_data") then
-      wait until
-        num_stimuli_done = num_test_loops
-        and num_data_check_done = num_test_loops
-        and rising_edge(clk);
+    procedure run_test(fixed_length_bytes : natural := 0) is
+      variable burst_length_bytes : positive := 1;
+      variable num_input_bytes_to_remove : natural := 0;
+
+      variable data_in, data_out : integer_array_t := null_integer_array;
+    begin
+      if fixed_length_bytes /= 0 then
+        burst_length_bytes := fixed_length_bytes;
+
+      else
+        -- Set a random length that will fill up whole input and output words
+        burst_length_bytes := rnd.RandInt(1, 5) * maximum_width_bytes;
+
+        if support_unaligned_burst_length then
+          -- In this case we can unstrobe/remove more than a whole word.
+          -- If upconverting, and we remove more than one whole input word, the entity will pad.
+          -- If downconverting, and we remove more than one whole output word, the entity
+          -- will strip.
+          num_input_bytes_to_remove := rnd.RandInt(0, maximum_width_bytes - 1);
+
+        elsif enable_strobe then
+          -- Unstrobe a number of byte lanes on the last input beat.
+          -- We must still be aligned in terms of number of output beats.
+          num_input_bytes_to_remove := rnd.RandInt(0, minimum_width_bytes - 1);
+        end if;
 
-    elsif run("test_full_throughput") then
-      start_time := now;
-      wait until
-        num_stimuli_done = num_test_loops
-        and num_data_check_done = num_test_loops
-        and rising_edge(clk);
-      time_diff := now - start_time;
+        burst_length_bytes := maximum(1, burst_length_bytes - num_input_bytes_to_remove);
+      end if;
 
-      check_relation(
-        time_diff < (num_test_loops * num_cycles_when_no_stall_and_no_strobing + 2) * clk_period
+      random_integer_array(
+        rnd => rnd,
+        integer_array => data_in,
+        width => burst_length_bytes,
+        bits_per_word => 8,
+        is_signed => false
       );
-    end if;
+      data_out := copy(data_in);
 
-    test_runner_cleanup(runner);
-  end process;
+      push_ref(input_data_queue, data_in);
+      push_ref(output_data_queue, data_out);
 
+      num_output_bursts_expected := num_output_bursts_expected + 1;
+    end procedure;
 
-  ------------------------------------------------------------------------------
-  stimuli : process
-    variable rnd_jitter, rnd_data : RandomPType;
-    variable input_data_v : std_logic_vector(input_data'range);
+    variable start_time, time_diff : time;
 
-    variable num_strobes_in_word : positive := input_bytes_per_beat;
-    variable num_bytes_remaining : natural := 0;
+    constant full_throughput_num_bytes : positive := maximum_width_bytes * 100 * 10;
 
-    variable num_input_words_sent, num_padding_words : natural := 0;
-  begin
-    rnd_jitter.InitSeed("stimuli" & rnd_jitter'instance_name);
-    rnd_data.InitSeed("rnd_data");
+    constant full_throughput_num_input_beats : positive :=
+      full_throughput_num_bytes / input_bytes_per_beat;
+    constant full_throughput_num_output_beats : positive :=
+      full_throughput_num_bytes / output_bytes_per_beat;
 
-    while num_stimuli_done < num_test_loops loop
-      num_bytes_remaining := num_bytes_per_test;
-      num_input_words_sent := 0;
-
-      while num_bytes_remaining > 0 loop
-        if enable_strobe then
-          num_strobes_in_word :=
-            minimum(rnd_jitter.RandInt(1, input_bytes_per_beat), num_bytes_remaining);
+    constant full_throughput_num_cycles : positive :=
+      maximum(full_throughput_num_input_beats, full_throughput_num_output_beats);
 
-          input_strobe <= (others => '0');
-          input_strobe(num_strobes_in_word - 1 downto 0) <= (others => '1');
+    procedure wait_until_done is
+    begin
+      wait until
+        is_empty(input_data_queue)
+        and is_empty(output_data_queue)
+        and num_output_bursts_checked = num_output_bursts_expected
+        and rising_edge(clk);
+      wait until rising_edge(clk);
+    end procedure;
 
-          -- Reset the data word to zero. Only the appropriate bytes will be assigned below.
-          input_data_v := (others => '0');
-        end if;
+  begin
+    test_runner_setup(runner, runner_cfg);
+    rnd.InitSeed(rnd'instance_name);
 
-        random_slv(rnd_data, input_data_v(num_strobes_in_word * 8 - 1 downto 0));
+    if run("test_data") then
+      for idx in 0 to 200 loop
+        run_test;
+      end loop;
 
-        input_valid <= '1';
+      wait_until_done;
 
-        input_data <= input_data_v;
-        num_bytes_remaining := num_bytes_remaining - num_strobes_in_word;
+    elsif run("test_full_throughput") then
+      start_time := now;
 
-        input_last <= to_sl(num_bytes_remaining = 0);
-        wait until (input_ready and input_valid) = '1' and rising_edge(clk);
-        num_input_words_sent := num_input_words_sent + 1;
-
-        if data_jitter then
-          input_valid <= '0';
-          for wait_cycle in 1 to rnd_jitter.FavorSmall(0, 2) loop
-            wait until rising_edge(clk);
-          end loop;
-        end if;
+      for idx in 0 to 10 - 1 loop
+        run_test(fixed_length_bytes=>full_throughput_num_bytes / 10);
       end loop;
+      wait_until_done;
 
-      if output_width > input_width and not support_unaligned_burst_length then
-        -- Pad so that we send the input burst length is a multiple of the output data width.
-        num_padding_words := num_input_words_sent mod (output_width / input_width);
-
-        for padding_word_idx in 1 to num_padding_words loop
-          input_valid <= '1';
-          input_last <= '0';
-          input_data <= (others => '0');
-          input_strobe <= (others => '0');
-          wait until (input_ready and input_valid) = '1' and rising_edge(clk);
-        end loop;
-      end if;
+      time_diff := now - start_time;
+      check_relation(
+        time_diff < (full_throughput_num_cycles + 4) * clk_period
+      );
+    end if;
 
-      input_valid <= '0';
-      num_stimuli_done <= num_stimuli_done + 1;
-    end loop;
+    test_runner_cleanup(runner);
   end process;
 
 
   ------------------------------------------------------------------------------
-  data_check : process
-    variable rnd_jitter, rnd_data : RandomPType;
+  axi_stream_master_inst : entity bfm.axi_stream_master
+    generic map (
+      data_width_bits => input_data'length,
+      data_queue => input_data_queue,
+      stall_config => stall_config,
+      logger_name_suffix => "_input",
+      strobe_unit_width_bits => input_data'length / input_strobe'length
+    )
+    port map (
+      clk => clk,
+      --
+      ready => input_ready,
+      valid => input_valid,
+      last => input_last,
+      data => input_data,
+      strobe => input_strobe
+    );
 
-    variable num_bytes_remaining : natural := 0;
 
-    variable expected_byte : std_logic_vector(8 - 1 downto 0) := (others => '0');
+  ------------------------------------------------------------------------------
+  output_block : block
+    signal strobe : std_logic_vector(output_strobe'range) := (others => '0');
   begin
-    rnd_jitter.InitSeed("data_check" & rnd_jitter'instance_name);
-    rnd_data.InitSeed("rnd_data");
 
-    while num_data_check_done < num_test_loops loop
-      num_bytes_remaining := num_bytes_per_test;
+    strobe <= output_strobe when enable_strobe else (others => '1');
 
-      while num_bytes_remaining > 0 loop
-        output_ready <= '1';
-        wait until (output_ready and output_valid) = '1' and rising_edge(clk);
-
-        for byte_lane_idx in 0 to output_bytes_per_beat - 1 loop
-          if (not enable_strobe) or output_strobe(byte_lane_idx) = '1' then
-            -- Build up the expected output data vector in same way that input data
-            -- is generated above. Note that the same random seed is used.
-            random_slv(rnd_data, expected_byte);
-            check_equal(
-              output_data((byte_lane_idx + 1) * 8 - 1 downto byte_lane_idx * 8),
-              expected_byte,
-              "byte_lane_idx=" & to_string(byte_lane_idx)
-              & ",num_bytes_remaining=" & to_string(num_bytes_remaining)
-            );
-
-            num_bytes_remaining := num_bytes_remaining - 1;
-          end if;
-        end loop;
-
-        check_equal(
-          output_last,
-          to_sl(num_bytes_remaining = 0),
-          "num_bytes_remaining=" & to_string(num_bytes_remaining)
-        );
-
-        if data_jitter then
-          output_ready <= '0';
-          for wait_cycle in 1 to rnd_jitter.FavorSmall(0, 2) loop
-            wait until rising_edge(clk);
-          end loop;
-        end if;
-      end loop;
 
-      output_ready <= '0';
-      num_data_check_done <= num_data_check_done + 1;
-    end loop;
-  end process;
+    ------------------------------------------------------------------------------
+    axi_stream_slave_inst : entity bfm.axi_stream_slave
+      generic map (
+        data_width_bits => output_data'length,
+        reference_data_queue => output_data_queue,
+        stall_config => stall_config,
+        logger_name_suffix => "_output",
+        disable_last_check => not enable_last
+      )
+      port map (
+        clk => clk,
+        --
+        ready => output_ready,
+        valid => output_valid,
+        last => output_last,
+        data => output_data,
+        strobe => strobe,
+        --
+        num_bursts_checked => num_output_bursts_checked
+      );
+
+  end block;
 
 
   ------------------------------------------------------------------------------
   dut : entity work.width_conversion
     generic map (
       input_width => input_width,
       output_width => output_width,
       enable_strobe => enable_strobe,
       strobe_unit_width => strobe_unit_width,
+      enable_last => enable_last,
       support_unaligned_burst_length => support_unaligned_burst_length
     )
     port map (
       clk => clk,
       --
       input_ready => input_ready,
       input_valid => input_valid,
```

### Comparing `tsfpga-8.0.1/modules/fifo/module_fifo.py` & `tsfpga-9.0.0/modules/fifo/module_fifo.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 # Copyright (c) Lukas Vik. All rights reserved.
 #
 # This file is part of the tsfpga project.
 # https://tsfpga.com
 # https://gitlab.com/tsfpga/tsfpga
 # --------------------------------------------------------------------------------------------------
 
-from tsfpga.module import BaseModule
+from tsfpga.module import BaseModule, get_tsfpga_modules
 from tsfpga.vivado.project import VivadoNetlistProject
-from tsfpga.vivado.build_result_checker import EqualTo, Ffs, Ramb18, Ramb36, TotalLuts
-from examples.tsfpga_example_env import get_tsfpga_modules
+from tsfpga.vivado.build_result_checker import (
+    EqualTo,
+    Ffs,
+    MaximumLogicLevel,
+    Ramb18,
+    Ramb36,
+    TotalLuts,
+)
 
 
 class Module(BaseModule):
-    def setup_vunit(self, vunit_proj, **kwargs):
+    def setup_vunit(self, vunit_proj, **kwargs):  # pylint: disable=unused-argument
         for test in (
             vunit_proj.library(self.library_name).test_bench("tb_asynchronous_fifo").get_tests()
         ):
             for read_clock_is_faster in [True, False]:
                 original_generics = dict(read_clock_is_faster=read_clock_is_faster)
 
                 for generics in self.generate_common_fifo_test_generics(
@@ -27,29 +33,38 @@
 
         for test in vunit_proj.library(self.library_name).test_bench("tb_fifo").get_tests():
             for generics in self.generate_common_fifo_test_generics(test.name):
                 self.add_vunit_config(test, generics=generics)
 
     @staticmethod
     def generate_common_fifo_test_generics(test_name, original_generics=None):
-        generics = original_generics if original_generics is not None else dict()
+        generics = original_generics if original_generics is not None else {}
 
         if "write_faster_than_read" in test_name:
             generics.update(read_stall_probability_percent=90)
             generics.update(enable_last=True)
 
         if "read_faster_than_write" in test_name:
             generics.update(write_stall_probability_percent=90)
 
         if "packet_mode" in test_name:
             generics.update(enable_last=True, enable_packet_mode=True)
 
         if "drop_packet" in test_name:
             generics.update(enable_last=True, enable_packet_mode=True, enable_drop_packet=True)
 
+        if "peek_mode" in test_name:
+            generics.update(
+                enable_last=True,
+                enable_packet_mode=True,
+                enable_peek_mode=True,
+                read_stall_probability_percent=20,
+                write_stall_probability_percent=20,
+            )
+
         if "init_state" in test_name or "almost" in test_name:
             # Note that
             #   almost_full_level = depth, or
             #   almost_empty_level = 0
             # result in alternative ways of calculating almost full/empty.
             depth = 32
 
@@ -73,15 +88,15 @@
         else:
             # For most test, generate configuration with two different depths
             for depth in [16, 512]:
                 generics.update(depth=depth)
 
                 yield generics
 
-    def setup_formal(self, formal_proj, **kwargs):
+    def setup_formal(self, formal_proj, **kwargs):  # pylint: disable=unused-argument,no-self-use
         depth = 4
         base_generics = dict(
             width=3,
             depth=depth,
             enable_last=True,
         )
 
@@ -122,14 +137,15 @@
                 top="fifo_netlist_build_wrapper",
                 generics=generics,
                 build_result_checkers=[
                     TotalLuts(EqualTo(14)),
                     Ffs(EqualTo(24)),
                     Ramb36(EqualTo(1)),
                     Ramb18(EqualTo(0)),
+                    MaximumLogicLevel(EqualTo(6)),
                 ],
             )
         )
 
         # A FIFO with level counter port and non-default almost_full_level, which
         # increases resource utilization.
         generics.update(almost_full_level=800)
@@ -141,14 +157,15 @@
                 top="fifo_wrapper",
                 generics=generics,
                 build_result_checkers=[
                     TotalLuts(EqualTo(26)),
                     Ffs(EqualTo(35)),
                     Ramb36(EqualTo(1)),
                     Ramb18(EqualTo(0)),
+                    MaximumLogicLevel(EqualTo(6)),
                 ],
             )
         )
 
         # Enabling last should not increase resource utilization
         generics.update(enable_last=True)
         projects.append(
@@ -159,14 +176,15 @@
                 top="fifo_wrapper",
                 generics=generics,
                 build_result_checkers=[
                     TotalLuts(EqualTo(26)),
                     Ffs(EqualTo(35)),
                     Ramb36(EqualTo(1)),
                     Ramb18(EqualTo(0)),
+                    MaximumLogicLevel(EqualTo(6)),
                 ],
             )
         )
 
         # Enabling packet mode increases resource utilization a bit, since an extra counter
         # and some further logic is introduced.
         generics.update(enable_packet_mode=True)
@@ -178,33 +196,55 @@
                 top="fifo_wrapper",
                 generics=generics,
                 build_result_checkers=[
                     TotalLuts(EqualTo(41)),
                     Ffs(EqualTo(46)),
                     Ramb36(EqualTo(1)),
                     Ramb18(EqualTo(0)),
+                    MaximumLogicLevel(EqualTo(6)),
                 ],
             )
         )
 
-        # Enabling drop packet support increases utilization further, since an extra counter
-        # and some further logic is introduced.
+        # Enabling drop packet support increases utilization compared to only packet mode,
+        # since an extra counter and some further logic is introduced.
         generics.update(enable_drop_packet=True)
         projects.append(
             VivadoNetlistProject(
                 name=self.test_case_name("fifo_with_drop_packet_support", generics),
                 modules=modules,
                 part=part,
                 top="fifo_wrapper",
                 generics=generics,
                 build_result_checkers=[
                     TotalLuts(EqualTo(47)),
                     Ffs(EqualTo(57)),
                     Ramb36(EqualTo(1)),
                     Ramb18(EqualTo(0)),
+                    MaximumLogicLevel(EqualTo(6)),
+                ],
+            )
+        )
+
+        # Enabling peek mode support increases utilization compared to only packet mode,
+        # since an extra address pointer and some further muxing is introduced.
+        generics.update(enable_drop_packet=False, enable_peek_mode=True)
+        projects.append(
+            VivadoNetlistProject(
+                name=self.test_case_name("fifo_with_peek_mode_support", generics),
+                modules=modules,
+                part=part,
+                top="fifo_wrapper",
+                generics=generics,
+                build_result_checkers=[
+                    TotalLuts(EqualTo(59)),
+                    Ffs(EqualTo(57)),
+                    Ramb36(EqualTo(1)),
+                    Ramb18(EqualTo(0)),
+                    MaximumLogicLevel(EqualTo(6)),
                 ],
             )
         )
 
     def _setup_asynchronous_fifo_build_projects(self, projects, modules, part):
         generics = dict(use_asynchronous_fifo=True, width=32, depth=1024)
 
@@ -218,14 +258,15 @@
                 top="fifo_netlist_build_wrapper",
                 generics=generics,
                 build_result_checkers=[
                     TotalLuts(EqualTo(44)),
                     Ffs(EqualTo(90)),
                     Ramb36(EqualTo(1)),
                     Ramb18(EqualTo(0)),
+                    MaximumLogicLevel(EqualTo(6)),
                 ],
             )
         )
 
         # A FIFO with level counter ports and non-default almost_full_level, which
         # increases resource utilization.
         generics.update(almost_full_level=800)
@@ -237,14 +278,15 @@
                 top="fifo_wrapper",
                 generics=generics,
                 build_result_checkers=[
                     TotalLuts(EqualTo(67)),
                     Ffs(EqualTo(112)),
                     Ramb36(EqualTo(1)),
                     Ramb18(EqualTo(0)),
+                    MaximumLogicLevel(EqualTo(6)),
                 ],
             )
         )
 
         # Enabling last should not increase resource utilization
         generics.update(enable_last=True)
         projects.append(
@@ -255,14 +297,15 @@
                 top="fifo_wrapper",
                 generics=generics,
                 build_result_checkers=[
                     TotalLuts(EqualTo(67)),
                     Ffs(EqualTo(112)),
                     Ramb36(EqualTo(1)),
                     Ramb18(EqualTo(0)),
+                    MaximumLogicLevel(EqualTo(6)),
                 ],
             )
         )
 
         # Enabling packet mode increases resource utilization quite a lot since another
         # resync_counter is added.
         generics.update(enable_packet_mode=True)
@@ -274,14 +317,15 @@
                 top="fifo_wrapper",
                 generics=generics,
                 build_result_checkers=[
                     TotalLuts(EqualTo(86)),
                     Ffs(EqualTo(167)),
                     Ramb36(EqualTo(1)),
                     Ramb18(EqualTo(0)),
+                    MaximumLogicLevel(EqualTo(6)),
                 ],
             )
         )
 
         # Enabling drop_packet support actually decreases utilization. Some logic is added for
         # handling the drop_packet functionality, but one resync_counter instance is saved since
         # the read_level value is not used.
@@ -294,14 +338,15 @@
                 top="fifo_wrapper",
                 generics=generics,
                 build_result_checkers=[
                     TotalLuts(EqualTo(66)),
                     Ffs(EqualTo(134)),
                     Ramb36(EqualTo(1)),
                     Ramb18(EqualTo(0)),
+                    MaximumLogicLevel(EqualTo(6)),
                 ],
             )
         )
 
         # A shallow FIFO, which commonly would be used to resync a coherent bit vector.
         # Note that this uses the minimal top level wrapper so that only the barebone features
         # are available.
@@ -314,10 +359,11 @@
                 top="fifo_netlist_build_wrapper",
                 generics=generics,
                 build_result_checkers=[
                     TotalLuts(EqualTo(35)),
                     Ffs(EqualTo(50)),
                     Ramb36(EqualTo(0)),
                     Ramb18(EqualTo(0)),
+                    MaximumLogicLevel(EqualTo(4)),
                 ],
             )
         )
```

### Comparing `tsfpga-8.0.1/modules/fifo/rtl/fifo_netlist_build_wrapper.vhd` & `tsfpga-9.0.0/modules/fifo/rtl/fifo_netlist_build_wrapper.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/fifo/scoped_constraints/asynchronous_fifo.tcl` & `tsfpga-9.0.0/modules/fifo/scoped_constraints/asynchronous_fifo.tcl`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/fifo/src/asynchronous_fifo.vhd` & `tsfpga-9.0.0/modules/fifo/src/asynchronous_fifo.vhd`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     enable_last : boolean := false;
     -- If enabled, read_valid will not be asserted until a full packet is available in
     -- FIFO. I.e. when write_last has been received.
     enable_packet_mode : boolean := false;
     -- Set to true in order to use the drop_packet port. Must set enable_packet_mode as
     -- well to use this.
     enable_drop_packet : boolean := false;
+    -- Select what FPGA primitives will be used to implement the FIFO memory.
     ram_type : ram_style_t := ram_style_auto
   );
   port (
     -- Read data interface
     clk_read : in std_logic;
     read_ready : in  std_logic;
     -- '1' if FIFO is not empty
```

### Comparing `tsfpga-8.0.1/modules/fifo/src/fifo.vhd` & `tsfpga-9.0.0/modules/fifo/src/fifo.vhd`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 -- Copyright (c) Lukas Vik. All rights reserved.
 --
 -- This file is part of the tsfpga project.
 -- https://tsfpga.com
 -- https://gitlab.com/tsfpga/tsfpga
 -- -------------------------------------------------------------------------------------------------
 -- Synchronous FIFO.
+--
+-- This FIFO implementation has an optional "peek read" mode that is enabled by setting the
+-- enable_peek_mode generic. It makes it possible to read a packet multiple times.
+-- If the read_peek_mode signal is asserted when read_ready is asserted, the current packet will
+-- not be popped from the FIFO, but can instead be read again. Once the readout encounters
+-- read_last, the readout will return again to the first word of the packet.
+-- Note that the read_peek_mode value may not be changed during the readout of a packet.
+-- It must be static for all words in a packet, but may be updated after read_last.
 -- -------------------------------------------------------------------------------------------------
 
 library ieee;
 use ieee.std_logic_1164.all;
 use ieee.numeric_std.all;
 
 library common;
@@ -31,14 +39,18 @@
     enable_last : boolean := false;
     -- If enabled, read_valid will not be asserted until a full packet is available in
     -- FIFO. I.e. when write_last has been received. Must set enable_last as well to use this.
     enable_packet_mode : boolean := false;
     -- Set to true in order to use the drop_packet port. Must set enable_packet_mode as
     -- well to use this.
     enable_drop_packet : boolean := false;
+    -- Set to true in order to read words without popping from FIFO using the read_peek_mode port.
+    -- Must set enable_packet_mode as well to use this.
+    enable_peek_mode : boolean := false;
+    -- Select what FPGA primitives will be used to implement the FIFO memory.
     ram_type : ram_style_t := ram_style_auto
   );
   port (
     clk : in std_logic;
     -- When packet_mode is enabled, this value will still reflect the number of words that are in
     -- the FIFO RAM. This is not necessarily the same as the number of words that can be read, in
     -- this mode.
@@ -46,14 +58,17 @@
 
     read_ready : in std_logic;
     -- '1' if FIFO is not empty
     read_valid : out std_logic := '0';
     read_data : out std_logic_vector(width - 1 downto 0) := (others => '0');
     -- Must set enable_last generic in order to use this
     read_last : out std_logic := '0';
+    -- When this is asserted, packets can be read multiple times from the FIFO.
+    -- Must set enable_peek_mode generic in order to use this.
+    read_peek_mode : in std_logic := '0';
     -- '1' if there are almost_empty_level or fewer words available to read
     almost_empty : out std_logic := '1';
 
     -- '1' if FIFO is not full
     write_ready : out std_logic := '1';
     write_valid : in std_logic;
     write_data : in std_logic_vector(width - 1 downto 0);
@@ -68,63 +83,72 @@
 end entity;
 
 architecture a of fifo is
 
   -- Need one extra bit in the addresses to be able to make the distinction if the FIFO
   -- is full or empty (where the addresses would otherwise be equal).
   subtype fifo_addr_t is unsigned(num_bits_needed(2 * depth - 1) - 1 downto 0);
-  signal read_addr_next, read_addr : fifo_addr_t := (others => '0');
+  signal read_addr_next, read_addr, read_addr_peek : fifo_addr_t := (others => '0');
   signal write_addr_next, write_addr, write_addr_next_if_not_drop, write_addr_start_of_packet :
     fifo_addr_t := (others => '0');
 
   -- The part of the address that actually goes to the BRAM address port
   subtype bram_addr_range is integer range num_bits_needed(depth - 1) - 1 downto 0;
 
   signal num_lasts_in_fifo : integer range 0 to depth := 0;
 
-  signal should_drop_packet : std_logic := '0';
+  signal should_drop_packet, should_peek_read : std_logic := '0';
 
 begin
 
   assert is_power_of_two(depth) report "Depth must be a power of two" severity failure;
 
   assert enable_last or (not enable_packet_mode)
     report "Must set enable_last for packet mode" severity failure;
   assert enable_packet_mode or (not enable_drop_packet)
     report "Must set enable_packet_mode for drop packet support" severity failure;
+  assert enable_packet_mode or (not enable_peek_mode)
+    report "Must set enable_packet_mode for peek mode support" severity failure;
+
 
-  -- The flags will update one cycle after the write/read that puts them over/below the line.
-  -- Except for almost_empty when almost_empty_level is zero.
-  -- In that case, when a write puts it over the line there will be a two cycle latency, since
-  -- that write must propagate into the RAM before the data is valid to read.
-  -- For a read that puts it below the line there is always one cycle latency.
+  -- These flags will update one cycle after the write/read that puts them over/below the line.
+  -- Except for the fringe cases:
+  --
+  -- When almost_full_level is 'depth' and a read puts it below the line there will be a two
+  -- cycle latency. For a write that puts it above the line there is always one cycle latency.
+  --
+  -- When almost_empty_level is zero and a write puts it over the line there will be a two
+  -- cycle latency. For a read that puts it below the line there is always one cycle latency.
 
   assign_almost_full : if almost_full_level = depth generate
     almost_full <= not write_ready;
   else generate
     almost_full <= to_sl(level > almost_full_level - 1);
   end generate;
 
   assign_almost_empty : if almost_empty_level = 0 generate
     almost_empty <= not read_valid;
   else generate
     almost_empty <= to_sl(level < almost_empty_level + 1);
   end generate;
 
+  should_drop_packet <= to_sl(enable_drop_packet) and drop_packet;
+  should_peek_read <= to_sl(enable_peek_mode) and read_peek_mode;
+
 
   ------------------------------------------------------------------------------
   status : process
     variable num_lasts_in_fifo_next : integer range 0 to depth := 0;
   begin
     wait until rising_edge(clk);
 
     if enable_packet_mode then
       num_lasts_in_fifo_next := num_lasts_in_fifo
         + to_int(write_ready and write_valid and write_last and not should_drop_packet)
-        - to_int(read_ready and read_valid and read_last);
+        - to_int(read_ready and read_valid and read_last and not should_peek_read);
 
       -- We look at num_lasts_in_fifo_next since we need to update read_valid the same cycle when
       -- the read happens.
       -- We also look at num_lasts_in_fifo since a write needs an additional clock
       -- cycle to propagate into the RAM. This is really only needed when the FIFO is empty and
       -- a packet of length one is written. With this condition, there will be a two cycle latency
       -- from write_last being written to read_valid being asserted.
@@ -153,28 +177,68 @@
       if write_ready and write_valid and write_last and not should_drop_packet then
         write_addr_start_of_packet <= write_addr_next;
       end if;
     end if;
 
     -- These signals however must have the updated values to be valid for the next cycle.
     write_addr <= write_addr_next;
-    read_addr <= read_addr_next;
+
+    if enable_peek_mode then
+      -- In peek mode we maintain two addresses for read. The 'read_addr' points to where the
+      -- current packet starts. This is the address that affects 'write_ready', so that data that
+      -- is not yet popped may not be overwritten.
+      -- The read_addr_peek is the address that controls where we read in the memory.
+      -- This one can be ahead of 'read_addr' and will revert back to 'read_addr' once the whole
+      -- packet has been read out.
+      read_addr_peek <= read_addr_next;
+
+      if not read_peek_mode then
+        -- If not peek reading, the read address shall be updated as normal.
+        read_addr <= read_addr_next;
+      end if;
+    else
+      read_addr <= read_addr_next;
+    end if;
+
     -- The level count shall always be correct, and hence uses the updated values. Note that this
     -- can create some wonky situations, e.g. when level read as 1023 for a 1024 deep FIFO
     -- but write_ready is false.
     -- Also in packet_mode, the level is incremented for words that might be dropped later.
     level <= to_integer(write_addr_next - read_addr_next) mod (2 * depth);
   end process;
 
-  should_drop_packet <= to_sl(enable_drop_packet) and drop_packet;
 
   write_addr_next_if_not_drop <= write_addr + to_int(write_ready and write_valid);
   write_addr_next <=
     write_addr_start_of_packet when should_drop_packet else write_addr_next_if_not_drop;
-  read_addr_next <= read_addr + to_int(read_ready and read_valid);
+
+
+  ------------------------------------------------------------------------------
+  read_addr_calc : if enable_peek_mode generate
+
+    ------------------------------------------------------------------------------
+    calc_peek_addr : process(all)
+    begin
+      if read_ready and read_valid then
+        if read_last and read_peek_mode then
+          -- Go back to where the packet we just read out started, so it can be read again
+          read_addr_next <= read_addr;
+        else
+          read_addr_next <= read_addr_peek + 1;
+        end if;
+      else
+        read_addr_next <= read_addr_peek;
+      end if;
+    end process;
+
+  else generate
+
+    read_addr_next <= read_addr + to_int(read_ready and read_valid);
+
+  end generate;
 
 
   ------------------------------------------------------------------------------
   memory_block : block
     constant memory_word_width : integer := width + to_int(enable_last);
     subtype word_t is std_logic_vector(memory_word_width - 1 downto 0);
     type mem_t is array (integer range <>) of word_t;
```

### Comparing `tsfpga-8.0.1/modules/fifo/src/fifo_wrapper.vhd` & `tsfpga-9.0.0/modules/fifo/src/fifo_wrapper.vhd`

 * *Files 18% similar despite different names*

```diff
@@ -25,27 +25,29 @@
     width : positive;
     depth : natural;
     almost_full_level : integer range 0 to depth := depth;
     almost_empty_level : integer range 0 to depth := 0;
     enable_last : boolean := false;
     enable_packet_mode : boolean := false;
     enable_drop_packet : boolean := false;
+    enable_peek_mode : boolean := false;
     ram_type : ram_style_t := ram_style_auto
   );
   port (
     -- This clock is used for a synchronous FIFO
     clk : in std_logic;
     -- These clocks are used for an asynchronous FIFO
     clk_read : in std_logic := '0';
     clk_write : in std_logic := '0';
 
     read_ready : in  std_logic;
     read_valid : out std_logic := '0';
     read_data : out std_logic_vector(width - 1 downto 0) := (others => '0');
     read_last : out std_logic := '0';
+    read_peek_mode : in std_logic := '0';
 
     -- Note that this is the same as write_level for a synchronous FIFO.
     read_level : out integer range 0 to depth := 0;
     -- Note that for an asynchronous FIFO, this signal is in the "read" clock domain.
     almost_empty : out std_logic := '1';
 
     write_ready : out std_logic := '1';
@@ -75,14 +77,17 @@
     write_ready <= read_ready;
     read_valid <= write_valid;
     read_data <= write_data;
     read_last <= write_last;
 
   elsif use_asynchronous_fifo generate
 
+    assert not enable_peek_mode report "Only available for synchronous FIFO" severity failure;
+
+
     ------------------------------------------------------------------------------
     asynchronous_fifo_inst : entity work.asynchronous_fifo
       generic map (
         width => width,
         depth => depth,
         almost_full_level => almost_full_level,
         almost_empty_level => almost_empty_level,
@@ -121,24 +126,26 @@
         width => width,
         depth => depth,
         almost_full_level => almost_full_level,
         almost_empty_level => almost_empty_level,
         enable_last => enable_last,
         enable_packet_mode => enable_packet_mode,
         enable_drop_packet => enable_drop_packet,
+        enable_peek_mode => enable_peek_mode,
         ram_type => ram_type
       )
       port map (
         clk => clk,
         level => read_level,
         --
         read_ready => read_ready,
         read_valid => read_valid,
         read_data => read_data,
         read_last => read_last,
+        read_peek_mode => read_peek_mode,
         almost_empty => almost_empty,
         --
         write_ready => write_ready,
         write_valid => write_valid,
         write_data => write_data,
         write_last => write_last,
         almost_full => almost_full,
```

### Comparing `tsfpga-8.0.1/modules/fifo/test/tb_asynchronous_fifo.vhd` & `tsfpga-9.0.0/modules/fifo/test/tb_asynchronous_fifo.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/fifo/test/tb_fifo.vhd` & `tsfpga-9.0.0/modules/fifo/test/tb_fifo.vhd`

 * *Files 24% similar despite different names*

```diff
@@ -15,124 +15,127 @@
 
 library vunit_lib;
 use vunit_lib.axi_stream_pkg.all;
 use vunit_lib.sync_pkg.all;
 context vunit_lib.com_context;
 context vunit_lib.vunit_context;
 
+library bfm;
+
 library common;
 use common.types_pkg.all;
 
 
 entity tb_fifo is
   generic (
     depth : integer;
     almost_full_level : integer := 0;
     almost_empty_level : integer := 0;
     read_stall_probability_percent : integer := 0;
     write_stall_probability_percent : integer := 0;
     enable_last : boolean := false;
     enable_packet_mode : boolean := false;
     enable_drop_packet : boolean := false;
+    enable_peek_mode : boolean := false;
     runner_cfg : string
   );
 end entity;
 
 architecture tb of tb_fifo is
 
   constant width : integer := 8;
 
   signal clk : std_logic := '0';
   signal level : integer;
 
-  signal read_ready, read_valid, read_last, almost_empty : std_logic := '0';
+  signal read_ready, read_valid, read_last, read_peek_mode, almost_empty : std_logic := '0';
   signal write_ready, write_valid, write_last, almost_full : std_logic := '0';
   signal read_data, write_data : std_logic_vector(width - 1 downto 0) := (others => '0');
   signal drop_packet : std_logic := '0';
 
   signal has_gone_full_times, has_gone_empty_times : integer := 0;
 
   constant read_stall_config : stall_config_t := new_stall_config(
     stall_probability => real(read_stall_probability_percent) / 100.0,
     min_stall_cycles => 1,
-    max_stall_cycles => 4);
-  constant read_slave : axi_stream_slave_t := new_axi_stream_slave(
-    data_length => width,
-    stall_config => read_stall_config,
-    protocol_checker => new_axi_stream_protocol_checker(data_length => width,
-                                                        logger => get_logger("read_slave")));
-
+    max_stall_cycles => 3
+  );
   constant write_stall_config : stall_config_t := new_stall_config(
     stall_probability => real(write_stall_probability_percent) / 100.0,
     min_stall_cycles => 1,
-    max_stall_cycles => 4);
-  constant write_master : axi_stream_master_t := new_axi_stream_master(
-    data_length => width,
-    stall_config => write_stall_config,
-    protocol_checker => new_axi_stream_protocol_checker(data_length => width,
-                                                        logger => get_logger("write_master")));
+    max_stall_cycles => 3
+  );
+
+  constant write_data_queue, write_last_queue, read_data_queue, read_last_queue : queue_t :=
+    new_queue;
+
+  signal stimuli_inactive, read_is_ready : std_logic := '0';
 
 begin
 
   test_runner_watchdog(runner, 1 ms);
   clk <= not clk after 2 ns;
 
 
   ------------------------------------------------------------------------------
   main : process
 
-    variable data_queue, last_queue, axi_stream_pop_reference_queue : queue_t := new_queue;
     variable rnd : RandomPType;
 
-    procedure run_test(read_count, write_count : natural; set_last_flag : boolean := true) is
-      variable data : std_logic_vector(write_data'range);
-      variable last, last_expected : std_logic := '0';
-      variable axi_stream_pop_reference : axi_stream_reference_t;
+    procedure run_read(count : natural; wait_for_status_to_update : boolean := true) is
+      variable last_expected : std_logic := '0';
     begin
-      for write_idx in 0 to write_count - 1 loop
-        data := rnd.RandSLV(data'length);
-        last := to_sl(write_idx = write_count - 1 and set_last_flag);
+      for read_idx in 0 to count - 1 loop
+        read_is_ready <= '1';
+        wait until (read_ready and read_valid) = '1' and rising_edge(clk);
 
-        push_axi_stream(net, write_master, data, last);
+        check_equal(read_data, pop_std_ulogic_vector(read_data_queue), "read_idx=" & to_string(read_idx));
 
-        push(data_queue, data);
-        push(last_queue, last);
-      end loop;
-
-      -- Queue up reads in order to get full throughput
-      for read_idx in 0 to read_count - 1 loop
-        pop_axi_stream(net, read_slave, axi_stream_pop_reference);
-        -- We need to keep track of the pop_reference when we read the reply later.
-        -- Hence it is pushed to a queue.
-        push(axi_stream_pop_reference_queue, axi_stream_pop_reference);
-      end loop;
-
-      for read_idx in 0 to read_count - 1 loop
-        axi_stream_pop_reference := pop(axi_stream_pop_reference_queue);
-        await_pop_axi_stream_reply(net, axi_stream_pop_reference, data, last);
-
-        check_equal(data, pop_std_ulogic_vector(data_queue), "read_idx " & to_string(read_idx));
-        last_expected := pop(last_queue);
+        last_expected := pop(read_last_queue);
         if enable_last then
-          check_equal(last, last_expected, "read_idx " & to_string(read_idx));
+          check_equal(read_last, last_expected, "read_idx=" & to_string(read_idx));
         end if;
       end loop;
+      read_is_ready <= '0';
 
-      wait_until_idle(net, as_sync(write_master));
-      wait until rising_edge(clk);
+      if wait_for_status_to_update then
+        -- Wait one cycle for read_valid to fall and counters to update
+        wait until rising_edge(clk);
+      end if;
     end procedure;
 
-    procedure run_read(count : natural) is
+    procedure run_write(
+      count : natural;
+      set_last_flag : boolean := true;
+      wait_until_done : boolean := true
+    ) is
+      variable data : std_logic_vector(write_data'range);
+      variable last : std_logic := '0';
     begin
-      run_test(count, 0);
+      for write_idx in 0 to count - 1 loop
+        data := rnd.RandSLV(data'length);
+        last := to_sl(write_idx = count - 1 and set_last_flag);
+
+        push(write_data_queue, data);
+        push(write_last_queue, last);
+
+        push(read_data_queue, data);
+        push(read_last_queue, last);
+      end loop;
+
+      if wait_until_done then
+        wait until is_empty(write_data_queue) and rising_edge(clk);
+        wait until stimuli_inactive = '1' and rising_edge(clk);
+      end if;
     end procedure;
 
-    procedure run_write(count : natural) is
+    procedure run_test(read_count, write_count : natural) is
     begin
-      run_test(0, count);
+      run_write(count=>write_count, wait_until_done=>false);
+      run_read(read_count);
     end procedure;
 
     procedure clear_queue(queue : queue_t) is
       variable dummy : character;
     begin
       while not is_empty(queue) loop
         dummy := unsafe_pop(queue);
@@ -142,23 +145,31 @@
     procedure pulse_drop_packet is
     begin
       drop_packet <= '1';
       wait until rising_edge(clk);
       drop_packet <= '0';
     end procedure;
 
+    constant null_data : std_logic_vector(width - 1 downto 0) := (others => '0');
+    constant one : std_logic := '1';
+    constant zero : std_logic := '0';
+
+    -- For peek mode test, which is handled differently than the other tests
+    constant num_packets : positive := 12;
+    variable num_peek_iterations : positive := 1;
+    variable num_words : positive := 1;
+    variable data : std_logic_vector(write_data'range);
+    variable last : std_logic := '0';
+
   begin
     test_runner_setup(runner, runner_cfg);
     rnd.InitSeed(rnd'instance_name);
 
-    -- Decrease noise
-    disable(get_logger("read_slave:rule 4"), warning);
-    disable(get_logger("write_master:rule 4"), warning);
     -- Some tests leave data unread in the FIFO
-    disable(get_logger("read_slave:rule 9"), error);
+    disable(get_logger("handshake_slave:rule 9"), error);
 
 
     if run("test_init_state") then
       check_equal(read_valid, '0');
       check_equal(write_ready, '1');
       check_equal(almost_full, '0');
       check_equal(almost_empty, '1');
@@ -170,34 +181,34 @@
       check_equal(read_valid, '0');
       check_equal(write_ready, '1');
       check_equal(almost_full, '0');
       check_equal(almost_empty, '1');
 
     elsif run("test_write_faster_than_read") then
       run_test(5000, 5000);
-      check_true(is_empty(data_queue));
+      check_true(is_empty(read_data_queue));
       check_relation(has_gone_full_times > 500, "Got " & to_string(has_gone_full_times));
 
     elsif run("test_read_faster_than_write") then
       run_test(5000, 5000);
-      check_true(is_empty(data_queue));
+      check_true(is_empty(read_data_queue));
       check_relation(has_gone_empty_times > 500, "Got " & to_string(has_gone_empty_times));
 
     elsif run("test_packet_mode") then
       -- Write and immediately read a short packet
       run_test(read_count=>1, write_count=>1);
 
       -- Write a few words, without setting last
-      run_test(read_count=>0, write_count=>3, set_last_flag=>false);
+      run_write(count=>3, set_last_flag=>false);
       check_relation(level > 0);
       check_equal(read_valid, False);
 
       -- Writing another word, with last set, shall enable read valid.
-      -- Note that the read_valid latency is one cycle higher in packet_mode.
-      run_test(read_count=>0, write_count=>1);
+      run_write(count=>1);
+      -- Takes one cycle extra to propagate in packet mode.
       wait until rising_edge(clk);
       check_equal(read_valid, True);
 
       -- Write further packets
       for i in 1 to 3 loop
         run_test(read_count=>0, write_count=>4);
         check_equal(read_valid, True);
@@ -205,45 +216,48 @@
 
       -- Read and check all the packets (will only work if read_valid is set properly)
       run_read(4 * 4);
       check_equal(read_valid, False);
       check_equal(level, 0);
 
       -- Write a few words, without setting last
-      run_test(read_count=>0, write_count=>3, set_last_flag=>false);
+      run_write(count=>3, set_last_flag=>false);
       check_relation(level > 0);
       check_equal(read_valid, False);
 
       -- Writing another word, with last set, shall enable read valid.
-      -- Note that the read_valid latency is one cycle higher in packet_mode.
-      run_test(read_count=>0, write_count=>1);
+      run_write(count=>1);
+      -- Takes one cycle extra to propagate in packet mode.
       wait until rising_edge(clk);
       check_equal(read_valid, True);
 
+      -- Read the last word to finish test
+      run_read(4);
+
     elsif run("test_packet_mode_deep") then
       -- Show that the FIFO can be filled with lasts
 
       -- Fill the FIFO with lasts
       for i in 1 to depth loop
-        run_test(read_count=>0, write_count=>1, set_last_flag=>true);
+        run_write(count=>1, set_last_flag=>true);
       end loop;
       check_equal(read_valid, True);
 
       run_read(1);
       check_equal(read_valid, True);
 
       run_write(1);
       check_equal(read_valid, True);
 
       run_read(depth);
       check_equal(read_valid, False);
 
       -- Fill the FIFO with lasts again
       for i in 1 to depth loop
-        run_test(read_count=>0, write_count=>1, set_last_flag=>true);
+        run_write(count=>1, set_last_flag=>true);
       end loop;
       check_equal(read_valid, True);
 
       run_read(depth - 1);
       check_equal(read_valid, True);
 
       run_read(1);
@@ -254,41 +268,43 @@
       -- Note that this will set write_last on the last write, and some data will be left unread.
       run_test(read_count=>depth / 2, write_count=>depth * 3 / 4);
       check_equal(level, depth / 4);
 
       -- Write some data without setting last, simulating a packet in progress.
       -- Drop the packet, and then read out the remainder of the previous packet.
       -- Note that the counts chosen will make the pointers wraparound.
-      run_test(read_count=>0, write_count=>depth / 2, set_last_flag=>false);
+      run_write(count=>depth / 2, set_last_flag=>false);
       pulse_drop_packet;
       run_read(depth / 4);
 
       check_equal(read_valid, '0');
       check_equal(level, 0);
 
       -- Clear the data in the reference queues. This will be the data that was written, and then
       -- cleared. Hence it was never read and therefore the data is left in the queues.
-      clear_queue(data_queue);
-      clear_queue(last_queue);
+      clear_queue(read_data_queue);
+      clear_queue(read_last_queue);
 
       -- Write and verify a packet. Should be the only thing remaining in the FIFO.
       run_write(4);
       check_equal(level, 4);
 
       run_read(4);
       check_equal(read_valid, '0');
       check_equal(level, 0);
 
     elsif run("test_drop_packet_in_same_cycle_as_write_last_should_drop_the_packet") then
       check_equal(level, 0);
 
-      push_axi_stream(net, write_master, tdata=>x"00", tlast=>'0');
-      push_axi_stream(net, write_master, tdata=>x"00", tlast=>'1');
+      push(write_data_queue, null_data);
+      push(write_last_queue, zero);
+      push(write_data_queue, null_data);
+      push(write_last_queue, one);
 
-      -- Time the behavior of the AXI-Stream master. Appears to be a one cycle delay.
+      -- Time the behavior of the handshake master. Appears to be a one cycle delay.
       wait until rising_edge(clk);
 
       -- The first write happens at this rising edge.
       wait until rising_edge(clk);
 
       -- Set drop signal on same cycle as the "last" write
       drop_packet <= '1';
@@ -310,39 +326,149 @@
       run_write(almost_full_level - 1);
       check_equal(almost_full, '0');
 
       run_write(1);
       check_equal(almost_full, '1');
 
       run_read(1);
+      if almost_full_level = depth then
+        -- One cycle more latency in this configuration
+        check_equal(almost_full, '1');
+        wait until rising_edge(clk);
+      end if;
       check_equal(almost_full, '0');
 
     elsif run("test_almost_empty") then
       check_equal(almost_empty, '1');
 
       run_write(almost_empty_level);
       check_equal(almost_empty, '1');
 
       run_write(1);
       if almost_empty_level = 0 then
-        -- almost_empty is updated one cycle later, since write must propagate into RAM before
-        -- read data is valid
+        -- One cycle more latency in this configuration
+        check_equal(almost_empty, '1');
         wait until rising_edge(clk);
       end if;
       check_equal(almost_empty, '0');
 
       run_read(1);
       check_equal(almost_empty, '1');
+
+    elsif run("test_peek_mode") then
+      for packet_idx in 0 to num_packets - 1 loop
+        num_words := depth / 4 + packet_idx;
+
+        -- Push stimuli data to write queue.
+        rnd.InitSeed(rnd'instance_name & to_string(packet_idx));
+
+        for write_idx in 0 to num_words - 1 loop
+          data := rnd.RandSLV(data'length);
+          last := to_sl(write_idx = num_words - 1);
+
+          push(write_data_queue, data);
+          push(write_last_queue, last);
+        end loop;
+
+        -- Push the same data to read reference queue a couple of times. One time extra for each
+        -- time we will read the packet with peek mode.
+        num_peek_iterations := 1 + (packet_idx mod 3);
+        for peek_iteration in 0 to num_peek_iterations - 1 loop
+          -- Set known seed to get same data as is pushed to write queue.
+          rnd.InitSeed(rnd'instance_name & to_string(packet_idx));
+
+          for write_idx in 0 to num_words - 1 loop
+            data := rnd.RandSlv(data'length);
+            last := to_sl(write_idx = num_words - 1);
+
+            push(read_data_queue, data);
+            push(read_last_queue, last);
+          end loop;
+        end loop;
+      end loop;
+
+      -- Read out all the data
+      for packet_idx in 0 to num_packets - 1 loop
+        num_words := depth / 4 + packet_idx;
+
+        -- Read each packet a number of times. But actually pop data only on the last iteration.
+        num_peek_iterations := 1 + (packet_idx mod 3);
+        for peek_iteration in 0 to num_peek_iterations - 1 loop
+          report "peek_iteration=" & to_string(peek_iteration) ;
+          read_peek_mode <= to_sl(peek_iteration /= num_peek_iterations - 1);
+          run_read(num_words, wait_for_status_to_update=>rnd.RandInt(1) = 0);
+        end loop;
+      end loop;
+
     end if;
 
     test_runner_cleanup(runner, allow_disabled_errors=>true);
   end process;
 
 
   ------------------------------------------------------------------------------
+  stimuli_block : block
+    signal data_is_valid : std_logic := '0';
+  begin
+
+    stimuli_inactive <= not data_is_valid;
+
+    ------------------------------------------------------------------------------
+    write_data_stimuli : process
+    begin
+      while is_empty(write_data_queue) loop
+        wait until rising_edge(clk);
+      end loop;
+
+      data_is_valid <= '1';
+
+      write_data <= pop(write_data_queue);
+      write_last <= pop(write_last_queue);
+      wait until (write_ready and write_valid) = '1' and rising_edge(clk);
+
+      data_is_valid <= '0';
+    end process;
+
+
+    ------------------------------------------------------------------------------
+    handshake_master_inst : entity bfm.handshake_master
+      generic map (
+        stall_config => write_stall_config
+      )
+      port map (
+        clk => clk,
+        --
+        data_is_valid => data_is_valid,
+        --
+        ready => write_ready,
+        valid => write_valid
+      );
+
+  end block;
+
+
+  ------------------------------------------------------------------------------
+  handshake_slave_inst : entity bfm.handshake_slave
+    generic map (
+      stall_config => read_stall_config,
+      data_width => read_data'length
+    )
+    port map (
+      clk => clk,
+      --
+      data_is_ready => read_is_ready,
+      --
+      ready => read_ready,
+      valid => read_valid,
+      last => read_last or to_sl(not enable_last),
+      data => read_data
+    );
+
+
+  ------------------------------------------------------------------------------
   status_tracking : process
     variable read_transaction, write_transaction : std_logic := '0';
   begin
     wait until rising_edge(clk);
 
     -- If there was a read transaction last clock cycle, and we now want to read but there is no
     -- data available.
@@ -358,59 +484,34 @@
 
     read_transaction := read_ready and read_valid;
     write_transaction := write_ready and write_valid;
   end process;
 
 
   ------------------------------------------------------------------------------
-  axi_stream_slave_inst : entity vunit_lib.axi_stream_slave
-    generic map(
-      slave => read_slave
-    )
-    port map(
-      aclk => clk,
-      tvalid => read_valid,
-      tready => read_ready,
-      tdata => read_data,
-      tlast => read_last
-    );
-
-
-  ------------------------------------------------------------------------------
-  axi_stream_master_inst : entity vunit_lib.axi_stream_master
-    generic map(
-      master => write_master)
-    port map(
-      aclk => clk,
-      tvalid => write_valid,
-      tready => write_ready,
-      tdata => write_data,
-      tlast => write_last
-    );
-
-
-  ------------------------------------------------------------------------------
   dut : entity work.fifo
     generic map (
       width => width,
       depth => depth,
       almost_full_level => almost_full_level,
       almost_empty_level => almost_empty_level,
       enable_last => enable_last,
       enable_packet_mode => enable_packet_mode,
-      enable_drop_packet => enable_drop_packet
+      enable_drop_packet => enable_drop_packet,
+      enable_peek_mode => enable_peek_mode
     )
     port map (
       clk => clk,
       level => level,
 
       read_ready => read_ready,
       read_valid => read_valid,
       read_data => read_data,
       read_last => read_last,
+      read_peek_mode => read_peek_mode,
       almost_empty => almost_empty,
 
       write_ready => write_ready,
       write_valid => write_valid,
       write_data => write_data,
       write_last => write_last,
       almost_full => almost_full,
```

### Comparing `tsfpga-8.0.1/modules/math/src/math_pkg.vhd` & `tsfpga-9.0.0/modules/math/src/math_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/math/src/unsigned_divider.vhd` & `tsfpga-9.0.0/modules/math/src/unsigned_divider.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/math/test/tb_math_pkg.vhd` & `tsfpga-9.0.0/modules/math/test/tb_math_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/math/test/tb_unsigned_divider.vhd` & `tsfpga-9.0.0/modules/math/test/tb_unsigned_divider.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/reg_file/module_reg_file.py` & `tsfpga-9.0.0/modules/reg_file/module_reg_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,37 +2,36 @@
 # Copyright (c) Lukas Vik. All rights reserved.
 #
 # This file is part of the tsfpga project.
 # https://tsfpga.com
 # https://gitlab.com/tsfpga/tsfpga
 # --------------------------------------------------------------------------------------------------
 
-from tsfpga.module import BaseModule
+from tsfpga.module import BaseModule, get_tsfpga_modules
 from tsfpga.vivado.project import VivadoNetlistProject
 from tsfpga.vivado.build_result_checker import (
     EqualTo,
     Ffs,
     LogicLuts,
     MaximumLogicLevel,
     Ramb18,
     Ramb36,
     TotalLuts,
 )
-from examples.tsfpga_example_env import get_tsfpga_modules
 
 
 class Module(BaseModule):
-    def setup_vunit(self, vunit_proj, **kwargs):
+    def setup_vunit(self, vunit_proj, **kwargs):  # pylint: disable=unused-argument
         tb = vunit_proj.library(self.library_name).test_bench("tb_axi_lite_reg_file")
         tb.test("read_from_non_existent_register").set_generic("use_axi_lite_bfm", False)
         tb.test("read_from_non_read_type_register").set_generic("use_axi_lite_bfm", False)
         tb.test("write_to_non_existent_register").set_generic("use_axi_lite_bfm", False)
         tb.test("write_to_non_write_type_register").set_generic("use_axi_lite_bfm", False)
 
-    def setup_formal(self, formal_proj, **kwargs):
+    def setup_formal(self, formal_proj, **kwargs):  # pylint: disable=unused-argument,no-self-use
         formal_proj.add_config(
             top="axi_lite_reg_file_wrapper",
             engine_command="smtbmc",
             solver_command="z3",
             mode="prove",
         )
 
@@ -44,17 +43,17 @@
         projects.append(
             VivadoNetlistProject(
                 name=f"{self.library_name}.axi_lite_reg_file",
                 modules=all_modules,
                 part=part,
                 top="axi_lite_reg_file_wrapper",
                 build_result_checkers=[
-                    TotalLuts(EqualTo(199)),
-                    LogicLuts(EqualTo(199)),
-                    Ffs(EqualTo(456)),
+                    TotalLuts(EqualTo(197)),
+                    LogicLuts(EqualTo(197)),
+                    Ffs(EqualTo(447)),
                     Ramb36(EqualTo(0)),
                     Ramb18(EqualTo(0)),
                     MaximumLogicLevel(EqualTo(4)),
                 ],
             )
         )
```

### Comparing `tsfpga-8.0.1/modules/reg_file/rtl/axi_lite_reg_file_wrapper.vhd` & `tsfpga-9.0.0/modules/reg_file/rtl/axi_lite_reg_file_wrapper.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/reg_file/sim/reg_operations_pkg.vhd` & `tsfpga-9.0.0/modules/reg_file/sim/reg_operations_pkg.vhd`

 * *Files 0% similar despite different names*

```diff
@@ -601,15 +601,15 @@
     base_address : in addr_t := (others => '0');
     bus_handle : in bus_master_t := regs_bus_master
   ) is
   begin
     -- Read-modify-write where the 'bit_index' bit will be set to 'value'.
     -- Note that the read portion of this call is blocking, but the write portion is non-blocking.
 
-    write_reg_bits(
+    read_modify_write_reg_bits(
       net=>net,
       reg_index=>reg_index,
       bit_indexes=>(0 => bit_index),
       values=>(0 => value),
       base_address=>base_address,
       bus_handle=>bus_handle
     );
```

### Comparing `tsfpga-8.0.1/modules/reg_file/src/axi_lite_reg_file.vhd` & `tsfpga-9.0.0/modules/reg_file/src/axi_lite_reg_file.vhd`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,18 @@
         aw => (ready => '1'),
         w => axi_lite_s2m_w_init,
         b => axi_lite_s2m_b_init)
       );
     -- Register values
     regs_up : in reg_vec_t(regs'range) := default_values;
     regs_down : out reg_vec_t(regs'range) := default_values;
-    -- Each bit is pulsed for one cycle when the corresponding register is read/written
+    -- Each bit is pulsed for one cycle when the corresponding register is read/written.
+    -- For read, the bit is asserted the exact same cycle as the AXI-Lite R transaction occurs.
+    -- For write, the bit is asserted the cycle after the AXI-Lite W transaction occurs, so that
+    -- 'regs_down' is updated with the new value.
     reg_was_read : out std_logic_vector(regs'range) := (others => '0');
     reg_was_written : out std_logic_vector(regs'range) := (others => '0')
   );
 end entity;
 
 architecture a of axi_lite_reg_file is
 
@@ -70,22 +73,33 @@
     signal read_idx : decoded_idx_t := invalid_addr;
     signal valid_read_address : boolean := false;
   begin
 
     -- An address transaction has occured and the address points to a valid read register
     valid_read_address <= read_idx /= invalid_addr and is_read_type(regs(read_idx).reg_type);
 
+
+    ------------------------------------------------------------------------------
+    set_status : process(all)
+    begin
+      reg_was_read <= (others => '0');
+
+      if valid_read_address then
+        reg_was_read(read_idx) <= axi_lite_m2s.read.r.ready and axi_lite_s2m.read.r.valid;
+      end if;
+    end process;
+
+
+    ------------------------------------------------------------------------------
     read_process : process
     begin
       wait until rising_edge(clk);
 
       axi_lite_s2m.read.r.valid <= '0';
 
-      reg_was_read <= (others => '0');
-
       if valid_read_address then
         axi_lite_s2m.read.r.resp <= axi_resp_okay;
 
         if is_fabric_gives_value_type(regs(read_idx).reg_type) then
           axi_lite_s2m.read.r.data(reg_values(0)'range) <= regs_up(read_idx);
         else
           axi_lite_s2m.read.r.data(reg_values(0)'range) <= reg_values(read_idx);
@@ -106,18 +120,14 @@
 
         when r =>
           axi_lite_s2m.read.r.valid <= '1';
           if axi_lite_m2s.read.r.ready and axi_lite_s2m.read.r.valid then
             axi_lite_s2m.read.r.valid <= '0';
             axi_lite_s2m.read.ar.ready <= '1';
 
-            if valid_read_address then
-              reg_was_read(read_idx) <= '1';
-            end if;
-
             read_state <= ar;
           end if;
       end case;
     end process;
   end block;
 
 
@@ -133,14 +143,16 @@
     -- to assume invalid (initial) values.
     -- psl write_state_enum_should_be_valid : assert always
     --   (write_state = aw or write_state = w or write_state = b) @ rising_edge(clk);
 
     -- An address transaction has occured and the address points to a valid write register
     valid_write_address <= write_idx /= invalid_addr and is_write_type(regs(write_idx).reg_type);
 
+
+    ------------------------------------------------------------------------------
     write_process : process
     begin
       wait until rising_edge(clk);
 
       reg_was_written <= (others => '0');
 
       if valid_write_address then
@@ -200,14 +212,14 @@
     -- psl reg_was_written_should_pulse_only_one_clock_cycle : assert always
     --   {reg_was_written /= reg_was_accessed_zero} |=> (reg_was_written = reg_was_accessed_zero);
     --
     -- psl reg_was_read_should_pulse_only_one_clock_cycle : assert always
     --   {reg_was_read /= reg_was_accessed_zero} |=> (reg_was_read = reg_was_accessed_zero);
     --
     -- Asserting reg_was_read typically prompts something in the PL that changes the register value.
-    -- Hence it is important that reg_was_read is asserted after the actual read (R) transaction
-    -- has occured, and not e.g. after the AR transaction.
+    -- Hence it is important that reg_was_read is asserted at the actual read (R) transaction
+    -- has occured, and not e.g. at the AR transaction.
     -- psl reg_was_read_should_pulse_when_read_transaction_occurs : assert always
-    --   (reg_was_read /= reg_was_accessed_zero) -> prev(axi_lite_m2s.read.r.ready and axi_lite_s2m.read.r.valid);
+    --   (reg_was_read /= reg_was_accessed_zero) -> axi_lite_m2s.read.r.ready and axi_lite_s2m.read.r.valid;
   end block;
 
 end architecture;
```

### Comparing `tsfpga-8.0.1/modules/reg_file/src/interrupt_register.vhd` & `tsfpga-9.0.0/modules/reg_file/src/interrupt_register.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/reg_file/src/reg_file_pkg.vhd` & `tsfpga-9.0.0/modules/reg_file/src/reg_file_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/reg_file/test/tb_axi_lite_reg_file.vhd` & `tsfpga-9.0.0/modules/reg_file/test/tb_axi_lite_reg_file.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/reg_file/test/tb_interrupt_register.vhd` & `tsfpga-9.0.0/modules/reg_file/test/tb_interrupt_register.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/reg_file/test/tb_reg_file_pkg.vhd` & `tsfpga-9.0.0/modules/reg_file/test/tb_reg_file_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/reg_file/test/tb_reg_operations_pkg.vhd` & `tsfpga-9.0.0/modules/reg_file/test/tb_reg_operations_pkg.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/module_resync.py` & `tsfpga-9.0.0/modules/resync/module_resync.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 # Copyright (c) Lukas Vik. All rights reserved.
 #
 # This file is part of the tsfpga project.
 # https://tsfpga.com
 # https://gitlab.com/tsfpga/tsfpga
 # --------------------------------------------------------------------------------------------------
 
-from tsfpga.module import BaseModule
+from tsfpga.module import BaseModule, get_tsfpga_modules
 from tsfpga.vivado.build_result_checker import EqualTo, Ffs, TotalLuts
 from tsfpga.vivado.project import VivadoNetlistProject
-from examples.tsfpga_example_env import get_tsfpga_modules
 
 
 class Module(BaseModule):
-    def setup_vunit(self, vunit_proj, **kwargs):
+    def setup_vunit(self, vunit_proj, **kwargs):  # pylint: disable=unused-argument
         tb = vunit_proj.library(self.library_name).test_bench("tb_resync_slv_level")
         for output_clock_is_faster in [True, False]:
             for test_coherent in [True, False]:
                 for enable_input_register in [True, False]:
                     if test_coherent and enable_input_register:
                         # Coherent implementation does not have the 'input_register' mode
                         continue
```

### Comparing `tsfpga-8.0.1/modules/resync/scoped_constraints/resync_counter.tcl` & `tsfpga-9.0.0/modules/resync/scoped_constraints/resync_counter.tcl`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/scoped_constraints/resync_level.tcl` & `tsfpga-9.0.0/modules/resync/scoped_constraints/resync_level.tcl`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/scoped_constraints/resync_slv_level_coherent.tcl` & `tsfpga-9.0.0/modules/resync/scoped_constraints/resync_slv_level_coherent.tcl`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/src/resync_counter.vhd` & `tsfpga-9.0.0/modules/resync/src/resync_counter.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/src/resync_cycles.vhd` & `tsfpga-9.0.0/modules/resync/src/resync_cycles.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/src/resync_level.vhd` & `tsfpga-9.0.0/modules/resync/src/resync_level.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/src/resync_level_on_signal.vhd` & `tsfpga-9.0.0/modules/resync/src/resync_level_on_signal.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/src/resync_pulse.vhd` & `tsfpga-9.0.0/modules/resync/src/resync_pulse.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/src/resync_slv_level.vhd` & `tsfpga-9.0.0/modules/resync/src/resync_slv_level.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/src/resync_slv_level_coherent.vhd` & `tsfpga-9.0.0/modules/resync/src/resync_slv_level_coherent.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/src/resync_slv_level_on_signal.vhd` & `tsfpga-9.0.0/modules/resync/src/resync_slv_level_on_signal.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/test/tb_resync_counter.vhd` & `tsfpga-9.0.0/modules/resync/test/tb_resync_counter.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/test/tb_resync_cycles.vhd` & `tsfpga-9.0.0/modules/resync/test/tb_resync_cycles.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/test/tb_resync_pulse.vhd` & `tsfpga-9.0.0/modules/resync/test/tb_resync_pulse.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/test/tb_resync_slv_level.vhd` & `tsfpga-9.0.0/modules/resync/test/tb_resync_slv_level.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/modules/resync/test/tb_resync_slv_level_on_signal.vhd` & `tsfpga-9.0.0/modules/resync/test/tb_resync_slv_level_on_signal.vhd`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/readme.rst` & `tsfpga-9.0.0/tsfpga.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,33 @@
+Metadata-Version: 2.1
+Name: tsfpga
+Version: 9.0.0
+Summary: tsfpga is a development platform that aims to streamline all aspects of your FPGA project.
+Home-page: https://tsfpga.com
+Author: Lukas Vik
+Author-email: 2767848-LukasVik@users.noreply.gitlab.com
+License: BSD 3-Clause License
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+
 About tsfpga
 ============
 
-|pic_website| |pic_gitlab| |pic_gitter| |pic_pip_install| |pic_license| |pic_python_line_coverage| |pic_vhdl_line_coverage| |pic_vhdl_branch_coverage|
+|pic_website| |pic_gitlab| |pic_gitter| |pic_pip_install| |pic_license| |pic_python_line_coverage|
 
 .. |pic_website| image:: https://tsfpga.com/badges/website.svg
   :alt: Website
   :target: https://tsfpga.com
 
 .. |pic_gitlab| image:: https://tsfpga.com/badges/gitlab.svg
   :alt: Gitlab
@@ -23,22 +45,14 @@
   :alt: License
   :target: https://tsfpga.com/license_information.html
 
 .. |pic_python_line_coverage| image:: https://tsfpga.com/badges/python_coverage.svg
   :alt: Python line coverage
   :target: https://tsfpga.com/python_coverage_html
 
-.. |pic_vhdl_line_coverage| image:: https://tsfpga.com/badges/vhdl_line_coverage.svg
-  :alt: VHDL line coverage
-  :target: https://tsfpga.com/vhdl_coverage_html
-
-.. |pic_vhdl_branch_coverage| image:: https://tsfpga.com/badges/vhdl_branch_coverage.svg
-  :alt: VHDL branch coverage
-  :target: https://tsfpga.com/vhdl_coverage_html
-
 tsfpga is a development platform that aims to streamline all aspects of your FPGA project.
 With its python build/simulation flow, along with complementary VHDL components, it is perfect for CI/CD and test-driven development.
 Focus has been placed on flexibility and modularization, achieving scalability even in very large multi-vendor code bases.
 
 **See documentation on the website**: https://tsfpga.com
 
 Key features
@@ -47,10 +61,13 @@
 * Source code centric project structure: Build projects, test configurations, constraints, IP cores, etc. are handled close to the source code.
 * Automatically adds build/simulation sources if a recognized folder structure is used.
 * Enables local VUnit configuration setup without multiple ``run.py``.
 * Handling of IP cores and simlib for your simulation project, with automatic re-compile when necessary.
 * Python-based parallel Vivado build system.
 * Register code generation from TOML: VHDL package, HTML documentation, C header, C++ class.
 * VHDL AXI components that enable the register bus: AXI-to-AXI-Lite converter, AXI-Lite interconnect, AXI-Lite mux (splitter), AXI-Lite clock domain crossing, AXI-Lite generic register file.
+* Released under the very permissive BSD 3-Clause License.
 
 The maintainers place high focus on quality, with everything having good unit test coverage and a thought-out structure.
 The project is mature and used in many production environments.
+
+
```

### Comparing `tsfpga-8.0.1/tsfpga/__init__.py` & `tsfpga-9.0.0/tsfpga/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 
 TSFPGA_PATH = REPO_ROOT / "tsfpga"
 TSFPGA_DOC = REPO_ROOT / "doc"
 TSFPGA_MODULES = REPO_ROOT / "modules"
 TSFPGA_TCL = THIS_DIR / "vivado" / "tcl"
 TSFPGA_GENERATED = REPO_ROOT / "generated"
 
-TSFPGA_EXAMPLES = REPO_ROOT / "examples"
+TSFPGA_EXAMPLES = TSFPGA_PATH / "examples"
 TSFPGA_EXAMPLE_MODULES = TSFPGA_EXAMPLES / "modules"
-TSFPGA_EXAMPLE_MODULES_WITH_IP = TSFPGA_EXAMPLES / "modules_with_ip"
 
 ALL_TSFPGA_MODULES_FOLDERS = [
     TSFPGA_MODULES,
     TSFPGA_EXAMPLE_MODULES,
-    TSFPGA_EXAMPLE_MODULES_WITH_IP,
 ]
 
-__version__ = "8.0.1"
+# Default encoding when opening files
+DEFAULT_FILE_ENCODING = "utf-8"
+
+__version__ = "9.0.0"
```

### Comparing `tsfpga-8.0.1/tsfpga/build_project_list.py` & `tsfpga-9.0.0/tsfpga/build_project_list.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/build_step_tcl_hook.py` & `tsfpga-9.0.0/tsfpga/build_step_tcl_hook.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/constraint.py` & `tsfpga-9.0.0/tsfpga/constraint.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/create_vhdl_ls_config.py` & `tsfpga-9.0.0/tsfpga/create_vhdl_ls_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         vunit_proj: A VUnit project.
         vivado_location (`pathlib.Path`): Vivado binary path. Will add unisim from this Vivado
             installation.
         ip_core_vivado_project_directory (`pathlib.Path`): Path to a Vivado project that contains
             generated "simulation" and "synthesis" files of IP cores
             (the "generate_target" TCL command). See simulate.py for an example of using this.
     """
-    toml_data = dict(libraries=dict())
+    toml_data = dict(libraries={})
 
     if modules is not None:
         for module in modules:
             vhd_file_wildcard = module.path.resolve() / "**" / "*.vhd"
             toml_data["libraries"][module.library_name] = dict(files=[str(vhd_file_wildcard)])
 
     if vunit_proj is not None:
```

### Comparing `tsfpga-8.0.1/tsfpga/formal_project.py` & `tsfpga-9.0.0/tsfpga/formal_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,17 @@
         return test_list
 
     def _compile_source_code(self, no_color=False):
         # Set up a VUnit project for compilation of sources
         args = VUnitCLI().parse_args(["--no-color", no_color])
         args.output_path = self.project_path / "vunit_out"
         vunit_proj = VUnit.from_args(args=args)
+        vunit_proj.add_verification_components()
+        vunit_proj.add_random()
+        vunit_proj.add_osvvm()
 
         src_files = []
         compiled_libraries = []
 
         for module in self.modules:
             vunit_library = vunit_proj.add_library(module.library_name)
             compiled_libraries.append(args.output_path / "ghdl" / "libraries" / module.library_name)
@@ -156,15 +159,15 @@
         Setup fields that are needed in a test case for VUnit test handling to work.
         These are unused by us. I think we are mimicking a IndependentSimTestCase object.
         """
         self.attribute_names = set()
 
         class TestConfiguration:
 
-            attributes = dict()
+            attributes = {}
 
         self.test_configuration = TestConfiguration()
 
     @property
     def name(self):
         return self._formal_config.test_name
```

### Comparing `tsfpga-8.0.1/tsfpga/git_simulation_subset.py` & `tsfpga-9.0.0/tsfpga/git_simulation_subset.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     _re_tb_filename = re.compile(r"(tb_.+\.vhd)|(.+\_tb.vhd)")
 
     def __init__(
         self, repo_root, reference_branch, vunit_proj, vunit_preprocessed_path=None, modules=None
     ):
         """
         Arguments:
-            repo_root (``pathlib.Path``): Root directory where git commands will be run.
+            repo_root (`pathlib.Path`): Root directory where git commands will be run.
             reference_branch (str): What git branch to compare against, when finding what files have
                 changed. Typically "origin/master".
             vunit_proj: A vunit project with all source files and testbenches added. Will be used
                 for dependency scanning.
-            vunit_preprocessed_path (``pathlib.Path``): If location/check preprocessing is enabled
+            vunit_preprocessed_path (`pathlib.Path`): If location/check preprocessing is enabled
                 in your VUnit project, supply the path to vunit_out/preprocessed.
             modules (.ModuleList): A list of modules that are included in the VUnit project. Must be
                 supplied only if preprocessing is enabled.
         """
         self._repo_root = repo_root
         self._reference_branch = reference_branch
         self._vunit_proj = vunit_proj
```

### Comparing `tsfpga-8.0.1/tsfpga/git_utils.py` & `tsfpga-9.0.0/tsfpga/git_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         return os.environ["GIT_COMMIT"][0:sha_length]
 
     # Import fails if "git" executable is not available, hence it can not be on top level.
     # This function should only be called if git is available.
     # pylint: disable=import-outside-toplevel
     from git import Repo
 
-    repo = Repo(directory)
+    repo = Repo(directory, search_parent_directories=True)
     git_commit = repo.head.commit.hexsha[0:sha_length]
     if repo.is_dirty():
         git_commit += " (local changes present)"
 
     return git_commit
```

### Comparing `tsfpga-8.0.1/tsfpga/hdl_file.py` & `tsfpga-9.0.0/tsfpga/hdl_file.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/ip_core_file.py` & `tsfpga-9.0.0/tsfpga/ip_core_file.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/module.py` & `tsfpga-9.0.0/tsfpga/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) Lukas Vik. All rights reserved.
 #
 # This file is part of the tsfpga project.
 # https://tsfpga.com
 # https://gitlab.com/tsfpga/tsfpga
 # --------------------------------------------------------------------------------------------------
 
+import tsfpga
 from tsfpga.constraint import Constraint
 from tsfpga.hdl_file import HdlFile
 from tsfpga.ip_core_file import IpCoreFile
 from tsfpga.module_list import ModuleList
 from tsfpga.system_utils import load_python_module
 from tsfpga.registers.parser import from_toml
 
@@ -156,23 +157,16 @@
         self, include_tests=True, files_include=None, files_avoid=None, **kwargs
     ):
         """
         See :meth:`.get_synthesis_files` for instructions on how to use ``files_include``
         and ``files_avoid``.
 
         Arguments:
-            include_tests (bool): When ``False`` the ``test`` folder is not included.
-                The use case is when testing a primary module that depends on other
-                secondary modules.
-                In this case we may want to compile the simulation files (``sim`` folder) of the
-                secondary modules but not their test files (``test`` folder).
-
-                .. Note::
-                    The ``test`` files are considered private to the module and should never be used
-                    by other modules.
+            include_tests (bool): When ``False`` the ``test`` folder, where testbenches usually
+                reside, is not included. The ``sim`` folder is always included.
             files_include (set(`pathlib.Path`)): Optionally filter to only include these files.
             files_avoid (set(`pathlib.Path`)): Optionally filter to discard these files.
             kwargs: Further parameters that can be sent by simulation flow to control what
                 files are included.
 
         Return:
             list(:class:`.HdlFile`): Files that should be included in a simulation project.
@@ -192,32 +186,32 @@
         )
 
         return synthesis_files + test_files
 
     def get_formal_files(self, files_include=None, files_avoid=None, **kwargs):
         """
         Returns the files to be used for formal verification.
-        By default these are the same that are used by synthesis
-        (by calling :meth:`get_synthesis_files`).
+        By default these are the simulation files, with testbenches excluded
+        (by calling :meth:`get_simulation_files`).
         Overload this method to select files manually.
 
         See :meth:`.get_synthesis_files` for instructions on how to use ``files_include``
         and ``files_avoid``.
 
         Arguments:
             files_include (set(`pathlib.Path`)): Optionally filter to only include these files.
             files_avoid (set(`pathlib.Path`)): Optionally filter to discard these files.
             kwargs: Further parameters that can be sent by formal flow to control what
                 files are included.
 
         Return:
             list(:class:`.HdlFile`): Files that should be included in a formal verification project.
         """
-        return self.get_synthesis_files(
-            files_include=files_include, files_avoid=files_avoid, **kwargs
+        return self.get_simulation_files(
+            include_tests=False, files_include=files_include, files_avoid=files_avoid, **kwargs
         )
 
     # pylint: disable=unused-argument
     def get_ip_core_files(self, files_include=None, files_avoid=None, **kwargs):
         """
         Get IP cores for this module.
 
@@ -440,7 +434,22 @@
         modules.append(
             get_module_object(
                 module_folder, module_name, library_name_has_lib_suffix, default_registers
             )
         )
 
     return modules
+
+
+def get_tsfpga_modules(names_include=None, names_avoid=None):
+    """
+    Wrapper of the regular :func:`.get_modules`. call with correct settings for tsfpga modules.
+    This will include the "real" tsfpga modules, but not the example modules.
+
+    Arguments will be passed on to :func:`.get_modules`.
+    """
+    return get_modules(
+        modules_folders=[tsfpga.TSFPGA_MODULES],
+        names_include=names_include,
+        names_avoid=names_avoid,
+        library_name_has_lib_suffix=False,
+    )
```

### Comparing `tsfpga-8.0.1/tsfpga/module_list.py` & `tsfpga-9.0.0/tsfpga/module_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,17 @@
                 return module
 
         raise ValueError(f'No module "{module_name}" available')
 
     def __iter__(self):
         return iter(self._modules)
 
+    def __getitem__(self, index):
+        return self._modules[index]
+
     def __len__(self):
         return len(self._modules)
 
     def __add__(self, other):
         if not isinstance(other, self.__class__):
             raise TypeError(f"Can only concatenate with another {self.__class__.__name__}")
```

### Comparing `tsfpga-8.0.1/tsfpga/registers/bit.py` & `tsfpga-9.0.0/tsfpga/registers/bit.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/bit_vector.py` & `tsfpga-9.0.0/tsfpga/registers/bit_vector.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/constant.py` & `tsfpga-9.0.0/tsfpga/registers/constant.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/html_translator.py` & `tsfpga-9.0.0/tsfpga/registers/html_translator.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/parser.py` & `tsfpga-9.0.0/tsfpga/registers/parser.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/register.py` & `tsfpga-9.0.0/tsfpga/registers/register.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/register_array.py` & `tsfpga-9.0.0/tsfpga/registers/register_array.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/register_c_generator.py` & `tsfpga-9.0.0/tsfpga/registers/register_c_generator.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/register_code_generator.py` & `tsfpga-9.0.0/tsfpga/registers/register_code_generator.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/register_cpp_generator.py` & `tsfpga-9.0.0/tsfpga/registers/register_cpp_generator.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/register_field.py` & `tsfpga-9.0.0/tsfpga/registers/register_field.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/register_html_generator.py` & `tsfpga-9.0.0/tsfpga/registers/register_html_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         return "".join([self._comment(header_line) for header_line in self.generated_info])
 
     @staticmethod
     def _to_hex_string(value, num_nibbles=4):
         if value < 0:
             return "N/A"
 
-        formatting_string = "0x{:0%iX}" % num_nibbles
+        formatting_string = f"0x{{:0{num_nibbles}X}}"
         return formatting_string.format(value)
 
     def _annotate_register_array(self, register_object):
         description = self._html_translator.translate(register_object.description)
         html = f"""
   <tr>
     <td class="array_header" colspan=5>
```

### Comparing `tsfpga-8.0.1/tsfpga/registers/register_list.py` & `tsfpga-9.0.0/tsfpga/registers/register_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import hashlib
 import datetime
 import re
 from shutil import copy2
 
 from pathlib import Path
 
+from tsfpga import DEFAULT_FILE_ENCODING
 from tsfpga.git_utils import git_commands_are_available, get_git_commit
 from tsfpga.svn_utils import svn_commands_are_available, get_svn_revision_information
 from tsfpga.system_utils import create_directory, create_file, read_file
 from . import __version__
 from .constant import Constant
 from .register import Register
 from .register_array import RegisterArray
@@ -254,15 +255,15 @@
     def _create_vhdl_package(self, vhd_file, self_hash):
         print(f"Creating VHDL register package {vhd_file}")
         # Add a header line with the hash
         generated_info = self.generated_source_info() + [
             f"Register hash {self_hash}, generator version {__version__}."
         ]
         register_vhdl_generator = RegisterVhdlGenerator(self.name, generated_info)
-        with vhd_file.open("w") as file_handle:
+        with open(vhd_file, "w", encoding=DEFAULT_FILE_ENCODING) as file_handle:
             file_handle.write(
                 register_vhdl_generator.get_package(self.register_objects, self.constants)
             )
 
     def create_c_header(self, output_path):
         """
         Create a C header file with register and field definitions.
@@ -390,25 +391,29 @@
 
     def generated_source_info(self):
         """
         Return:
             list(str): Line(s) informing the user that a file is automatically generated, containing
             info about the source of the generated register information.
         """
+        # Default to the user's current working directory
+        directory = Path(".")
+
         time_info = datetime.datetime.now().strftime("%Y-%m-%d %H:%M")
 
         file_info = ""
         if self.source_definition_file is not None:
+            directory = self.source_definition_file.parent
             file_info = f" from file {self.source_definition_file.name}"
 
         commit_info = ""
-        if git_commands_are_available(directory=Path(".")):
-            commit_info = f" at commit {get_git_commit(directory=Path('.'))}"
-        elif svn_commands_are_available():
-            commit_info = f" at revision {get_svn_revision_information()}"
+        if git_commands_are_available(directory):
+            commit_info = f" at commit {get_git_commit(directory)}"
+        elif svn_commands_are_available(directory):
+            commit_info = f" at revision {get_svn_revision_information(directory)}"
 
         info = f"Generated {time_info}{file_info}{commit_info}."
 
         return self.generated_info() + [info]
 
     def _hash(self):
         """
```

### Comparing `tsfpga-8.0.1/tsfpga/registers/register_python_generator.py` & `tsfpga-9.0.0/tsfpga/registers/register_python_generator.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/register_vhdl_generator.py` & `tsfpga-9.0.0/tsfpga/registers/register_vhdl_generator.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/test/test_bit.py` & `tsfpga-9.0.0/tsfpga/registers/test/test_bit.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/test/test_bit_vector.py` & `tsfpga-9.0.0/tsfpga/registers/test/test_bit_vector.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/test/test_constant.py` & `tsfpga-9.0.0/tsfpga/registers/test/test_constant.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/test/test_html_translator.py` & `tsfpga-9.0.0/tsfpga/registers/test/test_html_translator.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/test/test_parser.py` & `tsfpga-9.0.0/tsfpga/registers/test/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,22 +113,21 @@
 
 width=16
 description = "Some data"
 default_value="0000000000000011"
 
 
 ################################################################################
-%s
 """
 
     def setUp(self):
-        self.toml_file = create_file(self.tmp_path / "sensor_regs.toml", self.toml_data % "")
+        self.toml_file = create_file(self.tmp_path / "sensor_regs.toml", self.toml_data)
 
     def create_toml_file_with_extras(self, toml_extras):
-        data = self.toml_data % toml_extras
+        data = self.toml_data + toml_extras
         create_file(self.toml_file, data)
 
     def test_order_of_registers_and_bits(self):
         registers = from_toml(self.module_name, self.toml_file).register_objects
 
         assert registers[0].name == "data"
         assert registers[0].mode == "w"
```

### Comparing `tsfpga-8.0.1/tsfpga/registers/test/test_register.py` & `tsfpga-9.0.0/tsfpga/registers/test/test_register.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/test/test_register_array.py` & `tsfpga-9.0.0/tsfpga/registers/test/test_register_array.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/test/test_register_code_generation.py` & `tsfpga-9.0.0/tsfpga/registers/test/test_register_code_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import pytest
 
 import tsfpga
 from tsfpga.system_utils import read_file
 from tsfpga.registers.parser import from_toml
 
-from examples.tsfpga_example_env import get_default_registers
+from tsfpga.examples.example_env import get_default_registers
 
 
 # Test with the two example TOML files that we have available
 REGISTER_LISTS = [
     from_toml(
         module_name="ddr_buffer",
         toml_file=tsfpga.TSFPGA_EXAMPLE_MODULES / "ddr_buffer" / "regs_ddr_buffer.toml",
```

### Comparing `tsfpga-8.0.1/tsfpga/registers/test/test_register_html_generator.py` & `tsfpga-9.0.0/tsfpga/registers/test/test_register_html_generator.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/test/test_register_list.py` & `tsfpga-9.0.0/tsfpga/registers/test/test_register_list.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/test/test_register_python_generator.py` & `tsfpga-9.0.0/tsfpga/registers/test/test_register_python_generator.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/registers/test/test_register_vhdl_generator.py` & `tsfpga-9.0.0/tsfpga/registers/test/test_register_vhdl_generator.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/sby_writer.py` & `tsfpga-9.0.0/tsfpga/sby_writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # Copyright (c) Lukas Vik. All rights reserved.
 #
 # This file is part of the tsfpga project.
 # https://tsfpga.com
 # https://gitlab.com/tsfpga/tsfpga
 # --------------------------------------------------------------------------------------------------
 
+from tsfpga import DEFAULT_FILE_ENCODING
+
 
 class SbyWriter:
     """
     Writes a SymbiYosys script file
     """
 
     @staticmethod
@@ -46,9 +48,9 @@
         sby += f"{' '.join(ghdl_synth_cmd)} \n"
         sby += f"prep -top {top} \n"
         sby += "\n"
         sby += "[files]\n"
         sby += "\n".join([str(src_file) for src_file in src_files])
         sby += "\n"
 
-        with open(output_path, "w") as file_handle:
+        with open(output_path, "w", encoding=DEFAULT_FILE_ENCODING) as file_handle:
             file_handle.write(sby)
```

### Comparing `tsfpga-8.0.1/tsfpga/svn_utils.py` & `tsfpga-9.0.0/tsfpga/svn_utils.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/system_utils.py` & `tsfpga-9.0.0/tsfpga/system_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 import importlib.util
 import os
 from os.path import commonpath
 from platform import system
 from shutil import rmtree
 import subprocess
 
+from tsfpga import DEFAULT_FILE_ENCODING
+
 
 def create_file(file, contents=None):
     create_directory(file.parent, empty=False)
 
     contents = "" if contents is None else contents
-    with file.open("w") as file_handle:
+    with open(file, "w", encoding=DEFAULT_FILE_ENCODING) as file_handle:
         file_handle.write(contents)
 
     return file
 
 
 def read_file(file):
-    with file.open() as file_handle:
+    with open(file, encoding=DEFAULT_FILE_ENCODING) as file_handle:
         return file_handle.read()
 
 
 def read_last_lines_of_file(file, num_lines):
     """
     Read a number of lines from the end of a file, without buffering the whole file.
     Similar to unix ``tail`` command.
@@ -40,15 +42,15 @@
 
     Return:
         str: The last lines of the file.
     """
     result_lines = []
     blocks_to_read = 0
 
-    with open(file) as file_handle:
+    with open(file, encoding=DEFAULT_FILE_ENCODING) as file_handle:
         while len(result_lines) < num_lines:
             # Since we do not know the line lengths, there is some guessing involved. Keep reading
             # larger and larger blocks until we have all the lines that are requested.
             blocks_to_read += 1
 
             try:
                 # Read a block from the end
@@ -90,27 +92,27 @@
     Check if the file is in any of the directories.
 
     Arguments:
         file_path (`pathlib.Path`): The file to be checked.
         directories (list(`pathlib.Path`)): The directories to be controlled.
 
     Returns:
-        bool: True if there is a comon path.
+        bool: True if there is a common path.
     """
     for directory in directories:
         if commonpath([str(file_path), str(directory)]) == str(directory):
             return True
     return False
 
 
-def run_command(cmd, cwd=None):
+def run_command(cmd, cwd=None, env=None):
     if not isinstance(cmd, list):
         raise ValueError("Must be called with a list, not a string")
 
-    subprocess.check_call(cmd, cwd=cwd)
+    subprocess.check_call(cmd, cwd=cwd, env=env)
 
 
 def load_python_module(file):
     python_module_name = file.stem
 
     spec = importlib.util.spec_from_file_location(python_module_name, file)
     module = importlib.util.module_from_spec(spec)
```

### Comparing `tsfpga-8.0.1/tsfpga/test/conftest.py` & `tsfpga-9.0.0/tsfpga/test/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import sys
 import pytest
 
 import tsfpga
 
 # Do PYTHONPATH insert() instead of append() to prefer any local repo checkout over any pip install
-PATH_TO_VUNIT = tsfpga.REPO_ROOT.parent / "vunit"
+PATH_TO_VUNIT = tsfpga.REPO_ROOT.parent.parent / "vunit" / "vunit"
 sys.path.insert(0, str(PATH_TO_VUNIT.resolve()))
 
 
 @pytest.fixture
 def fixture_tmp_path(request, tmp_path):
     """
     A pytest fixture for usage in unittest.TestCase style test classes which gives
```

### Comparing `tsfpga-8.0.1/tsfpga/test/functional/gcc/test_register_compilation.py` & `tsfpga-9.0.0/tsfpga/test/functional/gcc/test_register_compilation.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/functional/vivado/test_building_vivado_project.py` & `tsfpga-9.0.0/tsfpga/test/functional/vivado/test_building_vivado_project.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/lint/pylintrc` & `tsfpga-9.0.0/tsfpga/test/lint/pylintrc`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/lint/pylintrc_original` & `tsfpga-9.0.0/tsfpga/test/lint/pylintrc_original`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/lint/test_copyright.py` & `tsfpga-9.0.0/tsfpga/test/lint/test_copyright.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/lint/test_file_format.py` & `tsfpga-9.0.0/tsfpga/test/lint/test_file_format.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,41 +4,39 @@
 # This file is part of the tsfpga project.
 # https://tsfpga.com
 # https://gitlab.com/tsfpga/tsfpga
 # --------------------------------------------------------------------------------------------------
 
 import pytest
 
-import tsfpga
+from tsfpga import DEFAULT_FILE_ENCODING, REPO_ROOT, TSFPGA_DOC
 from tsfpga.git_utils import find_git_files
 from tsfpga.system_utils import create_file
 
 
 def open_file_with_encoding(file):
     print(file)
-    with file.open(encoding="ascii") as file_handle:
+    with open(file, encoding="ascii") as file_handle:
         file_handle.read()
 
 
 def test_all_checked_in_files_are_properly_encoded():
     """
     To avoid problems with different editors and different file encodings, all checked in files
     should contain only ASCII characters.
 
     Avoid one of the documentation files that uses wonky characters to illustrate a directory tree.
     """
-    for file in files_to_test(
-        exclude_directories=[tsfpga.TSFPGA_DOC / "sphinx" / "module_structure.rst"]
-    ):
+    for file in files_to_test(exclude_directories=[TSFPGA_DOC / "sphinx" / "module_structure.rst"]):
         open_file_with_encoding(file)
 
 
 def check_file_ends_with_newline(file):
     test_ok = True
-    with file.open() as file_handle:
+    with open(file, encoding=DEFAULT_FILE_ENCODING) as file_handle:
         file_data = file_handle.read()
         if len(file_data) != 0:
             if file_data[-1] != "\n":
                 print(f"File {file} didn't end with newline")
                 test_ok = False
     return test_ok
 
@@ -52,15 +50,15 @@
     for file in files_to_test():
         test_ok &= check_file_ends_with_newline(file)
     assert test_ok
 
 
 def check_file_for_tab_character(file):
     test_ok = True
-    with file.open() as file_handle:
+    with open(file, encoding=DEFAULT_FILE_ENCODING) as file_handle:
         for idx, line in enumerate(file_handle.readlines()):
             if "\t" in line:
                 test_ok = False
                 print(f"TAB charatcher (\\t) on line {idx + 1} in {file}")
     return test_ok
 
 
@@ -73,15 +71,15 @@
     for file in files_to_test():
         test_ok &= check_file_for_tab_character(file)
     assert test_ok
 
 
 def check_file_for_carriage_return(file):
     test_ok = True
-    with file.open(newline="") as file_handle:
+    with open(file, encoding=DEFAULT_FILE_ENCODING, newline="") as file_handle:
         if "\r" in file_handle.read():
             test_ok = False
             print(f"Windows style line breaks (\\r\\n aka CR/LF) in {file}")
     return test_ok
 
 
 def test_no_checked_in_files_contain_carriage_return():
@@ -94,15 +92,15 @@
     for file in files_to_test():
         test_ok &= check_file_for_carriage_return(file)
     assert test_ok
 
 
 def check_file_for_trailing_whitespace(file):
     test_ok = True
-    with file.open() as file_handle:
+    with open(file, encoding=DEFAULT_FILE_ENCODING) as file_handle:
         for idx, line in enumerate(file_handle.readlines()):
             if " \n" in line:
                 test_ok = False
                 print(f"Trailing whitespace on line {idx + 1} in {file}")
     return test_ok
 
 
@@ -116,26 +114,26 @@
         test_ok &= check_file_for_trailing_whitespace(file)
     assert test_ok
 
 
 def files_to_test(exclude_directories=None):
     # Do not test binary image files
     return find_git_files(
-        directory=tsfpga.REPO_ROOT,
+        directory=REPO_ROOT,
         exclude_directories=exclude_directories,
         file_endings_avoid=("png", "svg"),
     )
 
 
 def test_open_file_with_encoding_should_raise_exception_on_bad_file(tmp_path):
     """
     Sanity check that the function we use actually triggers on bad files.
     """
     file = tmp_path / "temp_file_for_test.txt"
-    with file.open("w", encoding="utf-8") as file_handle:
+    with open(file, "w", encoding="utf-8") as file_handle:
         # Swedish word for island = non-ASCII character
         data = "\N{LATIN CAPITAL LETTER O WITH DIAERESIS}"
         file_handle.write(data)
 
     with pytest.raises(UnicodeDecodeError):
         open_file_with_encoding(file)
```

### Comparing `tsfpga-8.0.1/tsfpga/test/lint/test_python_lint.py` & `tsfpga-9.0.0/tsfpga/test/lint/test_python_lint.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/test_utils.py` & `tsfpga-9.0.0/tsfpga/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_build_step_tcl_hook.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_build_step_tcl_hook.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_constraint.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_constraint.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_formal_project.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_formal_project.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_git_simulation_subset.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_git_simulation_subset.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_git_utils.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_git_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from tsfpga import REPO_ROOT, TSFPGA_MODULES
 from tsfpga.git_utils import (
     git_commands_are_available,
     find_git_files,
     get_git_commit,
 )
-from tsfpga.system_utils import create_file, system_is_windows
+from tsfpga.system_utils import create_directory, create_file, system_is_windows
 
 
 THIS_FILE = Path(__file__)
 THIS_DIR = THIS_FILE.parent
 
 
 def test_this_file_is_listed_by_find_git_files():
@@ -92,25 +92,23 @@
     _local_changes_present = " (local changes present)"
 
     def setUp(self):
         self.repo_path = self.tmp_path / "my_repo"
         self.repo = Repo.init(self.repo_path)
         self.actor = Actor("A name", "an@email.com")
 
-        initial_file = self.repo_path / "initial_commit_file.txt"
-        create_file(initial_file)
+        initial_file = create_file(self.repo_path / "initial_commit_file.txt")
         self.repo.index.add(str(initial_file))
         self.repo.index.commit("Initial commit", author=self.actor, committer=self.actor)
 
-        self.trash_file = self.repo_path / "local_file_for_git_test.apa"
-        create_file(self.trash_file)
-        self.repo.index.add(str(self.trash_file))
+        trash_file = create_file(self.repo_path / "local_file_for_git_test.apa")
+        self.repo.index.add(str(trash_file))
 
     def test_get_git_commit_with_local_changes(self):
-        assert get_git_commit(directory=self.repo_path).endswith(" (local changes present)")
+        assert get_git_commit(directory=self.repo_path).endswith(self._local_changes_present)
 
     def test_get_git_commit_with_env_variable_and_local_changes(self):
         if "GIT_COMMIT" in os.environ:
             old_env = os.environ["GIT_COMMIT"]
         else:
             old_env = None
 
@@ -121,7 +119,11 @@
             del os.environ["GIT_COMMIT"]
         else:
             os.environ["GIT_COMMIT"] = old_env
 
     def test_get_git_commit_without_local_changes(self):
         self.repo.index.commit("Trash commit", author=self.actor, committer=self.actor)
         assert not get_git_commit(directory=self.repo_path).endswith(self._local_changes_present)
+
+    def test_get_git_commit_from_child_directory(self):
+        child_directory = create_directory(self.repo_path / "child_directory")
+        assert get_git_commit(directory=child_directory).endswith(self._local_changes_present)
```

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_hdl_file.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_hdl_file.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_ip_core_file.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_ip_core_file.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_module.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_module.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,48 +19,48 @@
 def test_file_list_filtering(tmp_path):
     module_name = "zebra"
     path = tmp_path / module_name
 
     create_directory(path / "folder_should_not_be_included")
     create_file(path / "should_not_be_included.apa")
 
-    synth_files = [
+    synth_files = {
         create_file(path / "syn.v"),
         create_file(path / "rtl" / "syn.v"),
         create_file(path / "src" / "syn.vhd"),
         create_file(path / "hdl" / "rtl" / "syn.vhd"),
         create_file(path / "hdl" / "package" / "syn.vhd"),
-    ]
+    }
 
-    test_files = [
+    test_files = {
         create_file(path / "test" / "test.v"),
         create_file(path / "rtl" / "tb" / "test.vhd"),
-    ]
+    }
 
-    sim_files = [create_file(path / "sim" / "sim.vhd")]
+    sim_files = {create_file(path / "sim" / "sim.vhd")}
 
     my_module = BaseModule(path, "zebra")
 
-    files = [file.path for file in my_module.get_synthesis_files()]
-    assert set(files) == set(synth_files)
+    files = {file.path for file in my_module.get_synthesis_files()}
+    assert files == synth_files
 
-    files = [file.path for file in my_module.get_simulation_files()]
-    assert set(files) == set(synth_files + test_files + sim_files)
+    files = {file.path for file in my_module.get_simulation_files()}
+    assert files == synth_files | test_files | sim_files
 
-    files = [file.path for file in my_module.get_simulation_files(include_tests=False)]
-    assert set(files) == set(synth_files + sim_files)
+    files = {file.path for file in my_module.get_simulation_files(include_tests=False)}
+    assert files == synth_files | sim_files
 
-    files = [file.path for file in my_module.get_simulation_files(files_include=synth_files)]
-    assert set(files) == set(synth_files)
+    files = {file.path for file in my_module.get_simulation_files(files_include=synth_files)}
+    assert files == synth_files
 
-    files = [file.path for file in my_module.get_simulation_files(files_avoid=synth_files)]
-    assert set(files) == set(test_files + sim_files)
+    files = {file.path for file in my_module.get_simulation_files(files_avoid=synth_files)}
+    assert files == test_files | sim_files
 
-    files = [file.path for file in my_module.get_formal_files()]
-    assert set(files) == set(synth_files)
+    files = {file.path for file in my_module.get_formal_files()}
+    assert files == synth_files | sim_files
 
 
 def test_get_synthesis_files_calls_get_simulation_files_with_correct_arguments():
     module = BaseModule(path=Path(), library_name="")
     with patch("tsfpga.module.BaseModule.get_synthesis_files") as get_synthesis_files:
         module.get_simulation_files(files_include=True, files_avoid=False, apa=123)
         get_synthesis_files.assert_called_once_with(files_include=True, files_avoid=False, apa=123)
```

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_module_list.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_module_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,27 @@
 from unittest.mock import MagicMock
 
 import pytest
 
 from tsfpga.module_list import ModuleList
 
 
+def test_module_list_indexing():
+    modules = ModuleList()
+
+    module_a = MagicMock()
+    module_b = MagicMock()
+
+    modules.append(module_a)
+    modules.append(module_b)
+
+    assert modules[0] is module_a
+    assert modules[1] is module_b
+
+
 class TestModuleList(TestCase):
     def setUp(self):
         self.modules = ModuleList()
 
         self.module_a = MagicMock()
         self.module_b = MagicMock()
         self.module_c = MagicMock()
```

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_sby_writer.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_sby_writer.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_svn_utils.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_svn_utils.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_system_utils.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_system_utils.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/test/unit/test_yosys_project.py` & `tsfpga-9.0.0/tsfpga/test/unit/test_yosys_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         )
         assert yosys_project.top == self.top
         assert yosys_project.generics == self.generics
         assert yosys_project.formal_settings == self.formal_settings
 
     def test_can_create_without_generics(self):
         yosys_project = YosysProject(top=self.top, formal_settings=self.formal_settings)
-        assert yosys_project.generics == dict()
+        assert yosys_project.generics == {}
 
     def test_runs_symbiyosys(self):
         yosys_project = YosysProject(
             top=self.top, generics=self.generics, formal_settings=self.formal_settings
         )
 
         # Check run_function, but mock the subprocess
```

### Comparing `tsfpga-8.0.1/tsfpga/vivado/build_result.py` & `tsfpga-9.0.0/tsfpga/vivado/build_result.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/build_result_checker.py` & `tsfpga-9.0.0/tsfpga/vivado/build_result_checker.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/common.py` & `tsfpga-9.0.0/tsfpga/vivado/common.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/hierarchical_utilization_parser.py` & `tsfpga-9.0.0/tsfpga/vivado/hierarchical_utilization_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,8 +37,8 @@
                 # The first columns contain entity name, etc. We only want the numbers
                 headers = headers[3:-1]
                 numbers = numbers[3:-1]
                 # Convert numbers from string to integers
                 numbers = [int(number) for number in numbers]
                 return OrderedDict(zip(headers, numbers))
 
-        return dict()
+        return {}
```

### Comparing `tsfpga-8.0.1/tsfpga/vivado/ip_cores.py` & `tsfpga-9.0.0/tsfpga/vivado/ip_cores.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,31 @@
     """
     Handle a list of IP core sources. Has a mechanism to detect whether a regenerate of IP files
     is needed.
     """
 
     project_name = "vivado_ip_project"
 
-    def __init__(self, modules, output_path, part_name, vivado_project_class=VivadoIpCoreProject):
+    def __init__(self, modules, output_path, part_name, vivado_project_class=None):
         """
         Arguments:
             modules (list(:class:`Module <.BaseModule>`)): IP cores from  these modules will be
                 included.
             output_path (`pathlib.Path`): The Vivado project will be placed here.
             part_name (str): Vivado part name to be used for the project.
             vivado_project_class: The Vivado project class that will be used for the IP core
                 project. Is safe to leave at default in most cases.
         """
         self.project_directory = output_path.resolve() / self.project_name
         self._part_name = part_name
+
+        vivado_project_class = (
+            VivadoIpCoreProject if vivado_project_class is None else vivado_project_class
+        )
+
         self._hash_file = self.project_directory / "ip_files_hash.txt"
 
         self._setup(modules, vivado_project_class)
 
     @property
     def compile_order_file(self):
         """
@@ -85,15 +90,15 @@
         self._vivado_project = vivado_project_class(
             name=self.project_name, modules=modules, part=self._part_name
         )
 
         ip_core_files = []
         for module in modules:
             # Send the same two arguments that are sent in the VivadoProject create flow
-            ip_core_files += module.get_ip_core_files(generics=dict(), part=self._part_name)
+            ip_core_files += module.get_ip_core_files(generics={}, part=self._part_name)
 
         self._hash = self._calculate_hash(ip_core_files)
 
     @staticmethod
     def _calculate_hash(ip_core_files):
         """
         A string with hashes of the different IP core files.
```

### Comparing `tsfpga-8.0.1/tsfpga/vivado/logic_level_distribution_parser.py` & `tsfpga-9.0.0/tsfpga/vivado/logic_level_distribution_parser.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/project.py` & `tsfpga-9.0.0/tsfpga/vivado/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
                 .. note::
                     This is a "kwargs" style argument. You can pass any number of named arguments.
         """
         self.name = name
         self.modules = modules.copy()
         self.part = part
-        self.static_generics = dict() if generics is None else generics.copy()
+        self.static_generics = {} if generics is None else generics.copy()
         self.constraints = [] if constraints is None else constraints.copy()
         self.tcl_sources = [] if tcl_sources is None else tcl_sources.copy()
         self.build_step_hooks = [] if build_step_hooks is None else build_step_hooks.copy()
         self._vivado_path = vivado_path
         self.default_run_index = default_run_index
         self.defined_at = defined_at
         self.other_arguments = None if other_arguments is None else other_arguments.copy()
```

### Comparing `tsfpga-8.0.1/tsfpga/vivado/simlib.py` & `tsfpga-9.0.0/tsfpga/vivado/simlib.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/simlib_commercial.py` & `tsfpga-9.0.0/tsfpga/vivado/simlib_commercial.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/simlib_common.py` & `tsfpga-9.0.0/tsfpga/vivado/simlib_common.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/simlib_ghdl.py` & `tsfpga-9.0.0/tsfpga/vivado/simlib_ghdl.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # https://gitlab.com/tsfpga/tsfpga
 # --------------------------------------------------------------------------------------------------
 
 import re
 import subprocess
 from pathlib import Path
 
+from tsfpga import DEFAULT_FILE_ENCODING
 from tsfpga.system_utils import create_directory
 from .common import get_vivado_path
 from .simlib_common import VivadoSimlibCommon
 
 
 class VivadoSimlibGhdl(VivadoSimlibCommon):
 
@@ -77,15 +78,17 @@
 
     def _compile_unifast(self, library_path):
         for vhd_file in self._iterate_compile_order(library_path):
             self._compile_ghdl_file(vhd_file, "unifast")
 
     @staticmethod
     def _iterate_compile_order(library_path):
-        with (library_path / "vhdl_analyze_order").open() as file_handle:
+        with open(
+            library_path / "vhdl_analyze_order", encoding=DEFAULT_FILE_ENCODING
+        ) as file_handle:
             for vhd_file_base in file_handle.readlines():
                 vhd_file = library_path / vhd_file_base.strip()
                 assert vhd_file.exists(), vhd_file
                 yield vhd_file
 
     def _compile_ghdl_file(self, vhd_file, library_name):
         print(f"Compiling {vhd_file} into {library_name}")
```

### Comparing `tsfpga-8.0.1/tsfpga/vivado/tcl/check_timing.tcl` & `tsfpga-9.0.0/tsfpga/vivado/tcl/check_timing.tcl`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/tcl/vivado_default_run.tcl` & `tsfpga-9.0.0/tsfpga/vivado/tcl/vivado_default_run.tcl`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/tcl/vivado_fast_run.tcl` & `tsfpga-9.0.0/tsfpga/vivado/tcl/vivado_fast_run.tcl`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/tcl/vivado_messages.tcl` & `tsfpga-9.0.0/tsfpga/vivado/tcl/vivado_messages.tcl`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/tcl.py` & `tsfpga-9.0.0/tsfpga/vivado/tcl.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         ip_cache_path=None,
         disable_io_buffers=True,
         # Add no sources other than IP cores
         ip_cores_only=False,
         # Will be passed on to module functions. Enables parameterization of e.g. IP cores.
         other_arguments=None,
     ):
-        generics = dict() if generics is None else generics
-        other_arguments = dict() if other_arguments is None else other_arguments
+        generics = {} if generics is None else generics
+        other_arguments = {} if other_arguments is None else other_arguments
 
         tcl = f"create_project {self.name} {{{to_tcl_path(project_folder)}}} -part {part}\n"
         tcl += "set_property target_language VHDL [current_project]\n"
 
         if ip_cache_path is not None:
             tcl += f"config_ip_cache -use_cache_location {{{to_tcl_path(ip_cache_path)}}}\n"
             tcl += "\n"
@@ -163,15 +163,15 @@
 
     def _add_build_step_hooks(self, build_step_hooks, project_folder):
         if build_step_hooks is None:
             return ""
 
         # There can be many hooks for the same step. Reorganize them into a dict, according
         # to the format step_name: [list of hooks]
-        hook_steps = dict()
+        hook_steps = {}
         for build_step_hook in build_step_hooks:
             if build_step_hook.hook_step in hook_steps:
                 hook_steps[build_step_hook.hook_step].append(build_step_hook)
             else:
                 hook_steps[build_step_hook.hook_step] = [build_step_hook]
 
         tcl = ""
```

### Comparing `tsfpga-8.0.1/tsfpga/vivado/test/conftest.py` & `tsfpga-9.0.0/tsfpga/vivado/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/test/test_build_result.py` & `tsfpga-9.0.0/tsfpga/vivado/test/test_build_result.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/test/test_build_result_checker.py` & `tsfpga-9.0.0/tsfpga/vivado/test/test_build_result_checker.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/test/test_common.py` & `tsfpga-9.0.0/tsfpga/vivado/test/test_common.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/test/test_hierarchical_utilization_parser.py` & `tsfpga-9.0.0/tsfpga/vivado/test/test_hierarchical_utilization_parser.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/test/test_ip_cores.py` & `tsfpga-9.0.0/tsfpga/vivado/test/test_ip_cores.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def test_get_ip_core_files_is_called_with_the_correct_arguments(tmp_path):
     modules = [MagicMock(spec=BaseModule)]
 
     with patch("tsfpga.vivado.ip_cores.VivadoIpCoreProject.create", autospec=True):
         VivadoIpCores(modules, tmp_path, part_name="test_part")
 
-    modules[0].get_ip_core_files.assert_called_once_with(generics=dict(), part="test_part")
+    modules[0].get_ip_core_files.assert_called_once_with(generics={}, part="test_part")
 
 
 @pytest.mark.usefixtures("fixture_tmp_path")
 class TestVivadoIpCores(TestCase):
 
     tmp_path = None
```

### Comparing `tsfpga-8.0.1/tsfpga/vivado/test/test_logic_level_distribution_parser.py` & `tsfpga-9.0.0/tsfpga/vivado/test/test_logic_level_distribution_parser.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/test/test_project.py` & `tsfpga-9.0.0/tsfpga/vivado/test/test_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,15 @@
 
         # No generics
         self.build_time_generics = None
         build_result = self._build(VivadoProject(name="apa", modules=[], part=""))
         assert build_result.success
         # Note: In python 3.8 we can use call_args.kwargs straight away
         _, kwargs = mocked_vivado_tcl.return_value.build.call_args
-        assert kwargs["generics"] == dict()
+        assert kwargs["generics"] == {}
 
         # Only build time generics
         self.build_time_generics = dict(runtime="value")
         build_result = self._build(VivadoProject(name="apa", modules=[], part=""))
         assert build_result.success
         _, kwargs = mocked_vivado_tcl.return_value.build.call_args
         assert kwargs["generics"] == dict(runtime="value")
```

### Comparing `tsfpga-8.0.1/tsfpga/vivado/test/test_simlib.py` & `tsfpga-9.0.0/tsfpga/vivado/test/test_simlib.py`

 * *Files identical despite different names*

### Comparing `tsfpga-8.0.1/tsfpga/vivado/test/test_tcl.py` & `tsfpga-9.0.0/tsfpga/vivado/test/test_tcl.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,19 +192,19 @@
 
     def test_source_file_list_is_correctly_formatted(self):
         tcl = self.tcl.create(
             project_folder=Path(), modules=self.modules, part="", top="", run_index=1
         )
 
         # Order of files is not really deterministic
-        expected_1 = "\nread_vhdl -library apa -vhdl2008 {{%s} {%s}}\n" % (self.b_vhd, self.a_vhd)
-        expected_2 = "\nread_vhdl -library apa -vhdl2008 {{%s} {%s}}\n" % (self.a_vhd, self.b_vhd)
+        expected_1 = f"\nread_vhdl -library apa -vhdl2008 {{{{{self.b_vhd}}} {{{self.a_vhd}}}}}\n"
+        expected_2 = f"\nread_vhdl -library apa -vhdl2008 {{{{{self.a_vhd}}} {{{self.b_vhd}}}}}\n"
         assert expected_1 in tcl or expected_2 in tcl
 
-        expected = "\nread_verilog {%s}\n" % self.c_v
+        expected = f"\nread_verilog {{{self.c_v}}}\n"
         assert expected in tcl
 
     def test_only_synthesis_files_added_to_create_project_tcl(self):
         tcl = self.tcl.create(
             project_folder=Path(), modules=self.modules, part="", top="", run_index=1
         )
         assert self.a_vhd in tcl and self.c_v in tcl
```

### Comparing `tsfpga-8.0.1/tsfpga/yosys_project.py` & `tsfpga-9.0.0/tsfpga/yosys_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def __init__(
         self,
         top=None,
         generics=None,
         formal_settings=None,
     ):
         self.top = top
-        self.generics = dict() if generics is None else generics
+        self.generics = {} if generics is None else generics
         self.formal_settings = formal_settings
 
     def run_formal(self, project_path, src_files, compiled_libraries):
         if not exists(project_path):
             makedirs(project_path)
 
         run_symbiyosys_sby = project_path / "run_symbiyosys.sby"
```

