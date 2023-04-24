# Comparing `tmp/parsl-2023.4.24.tar.gz` & `tmp/parsl-2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsl-2023.4.24.tar", last modified: Mon Apr 24 22:42:52 2023, max compression
+gzip compressed data, was "parsl-2023.4.3.tar", last modified: Mon Apr  3 22:43:04 2023, max compression
```

## Comparing `parsl-2023.4.24.tar` & `parsl-2023.4.3.tar`

### file list

```diff
@@ -1,476 +1,472 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.541700 parsl-2023.4.24/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 22:42:46.000000 parsl-2023.4.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 22:42:46.000000 parsl-2023.4.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-24 22:42:52.541700 parsl-2023.4.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-24 22:42:46.000000 parsl-2023.4.24/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.485700 parsl-2023.4.24/parsl/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.485700 parsl-2023.4.24/parsl/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/app/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/app/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/app/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.485700 parsl-2023.4.24/parsl/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/benchmark/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.485700 parsl-2023.4.24/parsl/channels/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/channels/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.485700 parsl-2023.4.24/parsl/channels/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/channels/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/channels/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.489699 parsl-2023.4.24/parsl/channels/oauth_ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/channels/oauth_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/channels/oauth_ssh/oauth_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.489699 parsl-2023.4.24/parsl/channels/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/channels/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/channels/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.489699 parsl-2023.4.24/parsl/channels/ssh_il/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/channels/ssh_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/channels/ssh_il/ssh_il.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.489699 parsl-2023.4.24/parsl/concurrent/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.489699 parsl-2023.4.24/parsl/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/ASPIRE1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/Azure.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/cooley.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/cori.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/exex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/illinoiscluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/osg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/polaris.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/stampede2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/toss3_llnl.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/configs/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.493700 parsl-2023.4.24/parsl/data_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/data_provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/data_provider/file_noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/data_provider/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/data_provider/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/data_provider/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/data_provider/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/data_provider/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/data_provider/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.493700 parsl-2023.4.24/parsl/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62326 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/dflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/executor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/flow_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/job_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/job_status_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/memoization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/rundirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/states.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/dataflow/taskrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.493700 parsl-2023.4.24/parsl/executors/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.493700 parsl-2023.4.24/parsl/executors/extreme_scale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/extreme_scale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/extreme_scale/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18718 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/extreme_scale/mpi_worker_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.493700 parsl-2023.4.24/parsl/executors/flux/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/flux/execute_parsl_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/flux/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/flux/flux_instance_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.497700 parsl-2023.4.24/parsl/executors/high_throughput/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/high_throughput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/high_throughput/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    33291 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/high_throughput/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29937 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/high_throughput/interchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/high_throughput/manager_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/high_throughput/monitoring_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/high_throughput/probe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33015 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/high_throughput/process_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/status_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/swift_t.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.497700 parsl-2023.4.24/parsl/executors/workqueue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/workqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/workqueue/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/workqueue/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    47999 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/workqueue/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/workqueue/parsl_coprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/executors/workqueue/parsl_coprocess_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.497700 parsl-2023.4.24/parsl/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/launchers/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/launchers/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.497700 parsl-2023.4.24/parsl/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36232 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    23301 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.497700 parsl-2023.4.24/parsl/monitoring/queries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/queries/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/radios.py
--rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.497700 parsl-2023.4.24/parsl/monitoring/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.501700 parsl-2023.4.24/parsl/monitoring/visualization/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.501700 parsl-2023.4.24/parsl/monitoring/visualization/plots/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/plots/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/plots/default/task_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/plots/default/workflow_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.501700 parsl-2023.4.24/parsl/monitoring/visualization/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/static/parsl-logo-white.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/static/parsl-monitor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.501700 parsl-2023.4.24/parsl/monitoring/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/templates/app.html
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/templates/dag.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/templates/resource_usage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/templates/task.html
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/templates/workflow.html
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/templates/workflows_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/monitoring/visualization/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/process_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.501700 parsl-2023.4.24/parsl/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.501700 parsl-2023.4.24/parsl/providers/ad_hoc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/ad_hoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/ad_hoc/ad_hoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.501700 parsl-2023.4.24/parsl/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29082 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/aws/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.501700 parsl-2023.4.24/parsl/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/azure/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/azure/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/cluster_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.501700 parsl-2023.4.24/parsl/providers/cobalt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/cobalt/cobalt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/cobalt/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.501700 parsl-2023.4.24/parsl/providers/condor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/condor/condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/condor/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.505700 parsl-2023.4.24/parsl/providers/googlecloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/googlecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/googlecloud/googlecloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.505700 parsl-2023.4.24/parsl/providers/grid_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/grid_engine/grid_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/grid_engine/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.505700 parsl-2023.4.24/parsl/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/kubernetes/kube.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/kubernetes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.505700 parsl-2023.4.24/parsl/providers/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.505700 parsl-2023.4.24/parsl/providers/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/lsf/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/lsf/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.505700 parsl-2023.4.24/parsl/providers/pbspro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/pbspro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/pbspro/pbspro.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/pbspro/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.505700 parsl-2023.4.24/parsl/providers/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/slurm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.505700 parsl-2023.4.24/parsl/providers/torque/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/torque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/torque/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/providers/torque/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.505700 parsl-2023.4.24/parsl/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/serialize/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/serialize/concretes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/serialize/facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.509700 parsl-2023.4.24/parsl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/callables_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.513700 parsl-2023.4.24/parsl/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/ad_hoc_cluster_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/azure_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/cooley_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/cori.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/ec2_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/ec2_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/exex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/htex_ad_hoc_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/htex_local_alternate.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/htex_local_intask_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/htex_local_rsync_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/local_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/local_threads_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/local_threads_checkpoint_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/local_threads_checkpoint_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/local_threads_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/local_threads_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/local_threads_http_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/local_threads_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/local_threads_no_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/nscc_singapore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/osg_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/petrelkube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/swan_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/user_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/workqueue_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/configs/workqueue_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.513700 parsl-2023.4.24/parsl/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/latency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.513700 parsl-2023.4.24/parsl/tests/integration/test_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.513700 parsl-2023.4.24/parsl/tests/integration/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_channels/test_local_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_channels/test_scp_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_channels/test_ssh_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_channels/test_ssh_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_channels/test_ssh_file_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_channels/test_ssh_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_parsl_load_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.513700 parsl-2023.4.24/parsl/tests/integration/test_stress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_stress/test_python_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/integration/test_stress/test_python_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.513700 parsl-2023.4.24/parsl/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/manual_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/manual_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/manual_tests/test_ad_hoc_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/manual_tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/manual_tests/test_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/manual_tests/test_memory_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/manual_tests/test_oauth_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/manual_tests/test_udp_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/manual_tests/test_worker_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.517700 parsl-2023.4.24/parsl/tests/site_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/site_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/site_tests/site_config_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/site_tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/site_tests/test_site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.517700 parsl-2023.4.24/parsl/tests/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/sites/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/sites/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/sites/test_dynamic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/sites/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/sites/test_launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/sites/test_local_adhoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.517700 parsl-2023.4.24/parsl/tests/sites/test_mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/sites/test_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/sites/test_start_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/sites/test_worker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_aalst_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.517700 parsl-2023.4.24/parsl/tests/test_bash_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/test_apptimeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/test_file_bug_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/test_keyword_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/test_kwarg_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/test_memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_bash_apps/test_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_callables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.517700 parsl-2023.4.24/parsl/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_channels/test_large_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.521700 parsl-2023.4.24/parsl/tests/test_checkpointing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_checkpointing/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_checkpointing/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_checkpointing/test_regression_233.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_checkpointing/test_regression_239.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_checkpointing/test_task_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.521700 parsl-2023.4.24/parsl/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_data/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_data/test_file_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_data/test_file_staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.521700 parsl-2023.4.24/parsl/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_docs/test_from_slides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_docs/test_tutorial_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_docs/test_workflow1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_docs/test_workflow2.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_docs/test_workflow3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_docs/test_workflow4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.521700 parsl-2023.4.24/parsl/tests/test_error_handling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/test_htex_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/test_htex_missing_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/test_htex_worker_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/test_python_walltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/test_rand_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/test_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/test_retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/test_retry_handler_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/test_serialization_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_error_handling/test_wrap_with_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.521700 parsl-2023.4.24/parsl/tests/test_flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_flowcontrol/test_one_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_flowcontrol/test_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.521700 parsl-2023.4.24/parsl/tests/test_manual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_manual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_manual/test_regression_220.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.521700 parsl-2023.4.24/parsl/tests/test_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_monitoring/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_monitoring/test_db_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_monitoring/test_fuzz_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_monitoring/test_memoization_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.525700 parsl-2023.4.24/parsl/tests/test_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_providers/test_local_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.529700 parsl-2023.4.24/parsl/tests/test_python_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_arg_input_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_at_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_dep_standard_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_depfail_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_fibonacci_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_fibonacci_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_import_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_mapred.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_joinapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_type5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_python_apps/test_worker_fail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.533700 parsl-2023.4.24/parsl/tests/test_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_regression/test_1480.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_regression/test_1653.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_regression/test_221.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_regression/test_226.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_regression/test_2652.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_regression/test_69a.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_regression/test_69b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_regression/test_854.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_regression/test_97.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_regression/test_98.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.533700 parsl-2023.4.24/parsl/tests/test_scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_scaling/test_scale_down.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.537700 parsl-2023.4.24/parsl/tests/test_staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_staging/staging_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_staging/test_1316.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_staging/test_docs_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_staging/test_docs_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_staging/test_elaborate_noop_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_staging/test_staging_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_staging/test_staging_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_staging/test_staging_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_staging/test_staging_https.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_staging/test_staging_https_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_thread_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.537700 parsl-2023.4.24/parsl/tests/test_threads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_threads/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/test_threads/test_lazy_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.541700 parsl-2023.4.24/parsl/tests/workqueue_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/workqueue_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/workqueue_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/workqueue_tests/local_threads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3835 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/workqueue_tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/workqueue_tests/wqex_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/tests/workqueue_tests/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.541700 parsl-2023.4.24/parsl/usage_tracking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/usage_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/usage_tracking/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-24 22:42:46.000000 parsl-2023.4.24/parsl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 22:42:51.000000 parsl-2023.4.24/parsl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:42:52.485700 parsl-2023.4.24/parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-24 22:42:52.000000 parsl-2023.4.24/parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15591 2023-04-24 22:42:52.000000 parsl-2023.4.24/parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:42:52.000000 parsl-2023.4.24/parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-24 22:42:52.000000 parsl-2023.4.24/parsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-24 22:42:52.000000 parsl-2023.4.24/parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 22:42:52.000000 parsl-2023.4.24/parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 22:42:46.000000 parsl-2023.4.24/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:42:52.541700 parsl-2023.4.24/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-04-24 22:42:46.000000 parsl-2023.4.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.937177 parsl-2023.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 22:42:52.000000 parsl-2023.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-03 22:42:52.000000 parsl-2023.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-03 22:43:04.937177 parsl-2023.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-03 22:42:52.000000 parsl-2023.4.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.865176 parsl-2023.4.3/parsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.869176 parsl-2023.4.3/parsl/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/app/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/app/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/app/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.869176 parsl-2023.4.3/parsl/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/channels/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.869176 parsl-2023.4.3/parsl/channels/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/channels/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/channels/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.869176 parsl-2023.4.3/parsl/channels/oauth_ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/channels/oauth_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/channels/oauth_ssh/oauth_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.869176 parsl-2023.4.3/parsl/channels/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/channels/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/channels/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.869176 parsl-2023.4.3/parsl/channels/ssh_il/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/channels/ssh_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/channels/ssh_il/ssh_il.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.869176 parsl-2023.4.3/parsl/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.873176 parsl-2023.4.3/parsl/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/ASPIRE1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/Azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/cooley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/cori.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/exex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/illinoiscluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/osg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/polaris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/stampede2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/toss3_llnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/configs/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.877176 parsl-2023.4.3/parsl/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/data_provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/data_provider/file_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/data_provider/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/data_provider/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/data_provider/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/data_provider/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/data_provider/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/data_provider/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.877176 parsl-2023.4.3/parsl/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58239 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/dflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/flow_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/job_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/job_status_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/rundirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/dataflow/taskrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.881176 parsl-2023.4.3/parsl/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.881176 parsl-2023.4.3/parsl/executors/extreme_scale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/extreme_scale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/extreme_scale/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18718 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/extreme_scale/mpi_worker_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.881176 parsl-2023.4.3/parsl/executors/flux/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/flux/execute_parsl_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/flux/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/flux/flux_instance_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.881176 parsl-2023.4.3/parsl/executors/high_throughput/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/high_throughput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/high_throughput/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32923 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/high_throughput/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29811 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/high_throughput/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/high_throughput/manager_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/high_throughput/monitoring_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/high_throughput/probe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32753 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/high_throughput/process_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/status_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/swift_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.885176 parsl-2023.4.3/parsl/executors/workqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/workqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/workqueue/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/workqueue/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/workqueue/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/workqueue/parsl_coprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/executors/workqueue/parsl_coprocess_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.885176 parsl-2023.4.3/parsl/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/launchers/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/launchers/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.885176 parsl-2023.4.3/parsl/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36503 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23301 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.885176 parsl-2023.4.3/parsl/monitoring/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/queries/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/radios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.885176 parsl-2023.4.3/parsl/monitoring/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.885176 parsl-2023.4.3/parsl/monitoring/visualization/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.889176 parsl-2023.4.3/parsl/monitoring/visualization/plots/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/plots/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/plots/default/task_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/plots/default/workflow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.889176 parsl-2023.4.3/parsl/monitoring/visualization/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/static/parsl-logo-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/static/parsl-monitor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.889176 parsl-2023.4.3/parsl/monitoring/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/templates/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/templates/dag.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/templates/resource_usage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/templates/task.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/templates/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/templates/workflows_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/monitoring/visualization/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/process_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.889176 parsl-2023.4.3/parsl/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.889176 parsl-2023.4.3/parsl/providers/ad_hoc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/ad_hoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/ad_hoc/ad_hoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.889176 parsl-2023.4.3/parsl/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29081 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/aws/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.893176 parsl-2023.4.3/parsl/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/azure/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/azure/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/cluster_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.893176 parsl-2023.4.3/parsl/providers/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/cobalt/cobalt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/cobalt/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.893176 parsl-2023.4.3/parsl/providers/condor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/condor/condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/condor/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.893176 parsl-2023.4.3/parsl/providers/googlecloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/googlecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/googlecloud/googlecloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.893176 parsl-2023.4.3/parsl/providers/grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/grid_engine/grid_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/grid_engine/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.893176 parsl-2023.4.3/parsl/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/kubernetes/kube.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/kubernetes/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.893176 parsl-2023.4.3/parsl/providers/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.897176 parsl-2023.4.3/parsl/providers/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/lsf/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/lsf/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.897176 parsl-2023.4.3/parsl/providers/pbspro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/pbspro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/pbspro/pbspro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/pbspro/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.897176 parsl-2023.4.3/parsl/providers/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/slurm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.897176 parsl-2023.4.3/parsl/providers/torque/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/torque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/torque/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/providers/torque/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.897176 parsl-2023.4.3/parsl/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/serialize/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/serialize/concretes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/serialize/facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.901177 parsl-2023.4.3/parsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/callables_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.909176 parsl-2023.4.3/parsl/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/ad_hoc_cluster_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/azure_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/cooley_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/cori.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/ec2_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/ec2_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/exex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/htex_ad_hoc_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/htex_local_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/htex_local_intask_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/htex_local_rsync_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/local_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/local_threads_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/local_threads_checkpoint_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/local_threads_checkpoint_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/local_threads_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/local_threads_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/local_threads_http_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/local_threads_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/local_threads_no_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/nscc_singapore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/osg_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/petrelkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/swan_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/user_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/workqueue_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/configs/workqueue_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.909176 parsl-2023.4.3/parsl/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/latency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.909176 parsl-2023.4.3/parsl/tests/integration/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.909176 parsl-2023.4.3/parsl/tests/integration/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_channels/test_local_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_channels/test_scp_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_channels/test_ssh_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_channels/test_ssh_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_channels/test_ssh_file_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_channels/test_ssh_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_parsl_load_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.913177 parsl-2023.4.3/parsl/tests/integration/test_stress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_stress/test_python_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/integration/test_stress/test_python_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.913177 parsl-2023.4.3/parsl/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/manual_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/manual_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/manual_tests/test_ad_hoc_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/manual_tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/manual_tests/test_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/manual_tests/test_memory_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/manual_tests/test_oauth_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/manual_tests/test_udp_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/manual_tests/test_worker_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.917177 parsl-2023.4.3/parsl/tests/site_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/site_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/site_tests/site_config_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/site_tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/site_tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.917177 parsl-2023.4.3/parsl/tests/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/sites/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/sites/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/sites/test_dynamic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/sites/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/sites/test_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/sites/test_local_adhoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.917177 parsl-2023.4.3/parsl/tests/sites/test_mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/sites/test_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/sites/test_start_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/sites/test_worker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_aalst_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.921177 parsl-2023.4.3/parsl/tests/test_bash_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/test_apptimeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/test_file_bug_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/test_keyword_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/test_kwarg_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/test_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_bash_apps/test_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_callables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.921177 parsl-2023.4.3/parsl/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_channels/test_large_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.921177 parsl-2023.4.3/parsl/tests/test_checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_checkpointing/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_checkpointing/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_checkpointing/test_regression_233.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_checkpointing/test_regression_239.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_checkpointing/test_task_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.921177 parsl-2023.4.3/parsl/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_data/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_data/test_file_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_data/test_file_staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.921177 parsl-2023.4.3/parsl/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_docs/test_from_slides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_docs/test_tutorial_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_docs/test_workflow1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_docs/test_workflow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_docs/test_workflow3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_docs/test_workflow4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.925176 parsl-2023.4.3/parsl/tests/test_error_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/test_htex_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/test_htex_missing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/test_htex_worker_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/test_python_walltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/test_rand_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/test_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/test_retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/test_retry_handler_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/test_serialization_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_error_handling/test_wrap_with_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.925176 parsl-2023.4.3/parsl/tests/test_flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_flowcontrol/test_one_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_flowcontrol/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.925176 parsl-2023.4.3/parsl/tests/test_manual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_manual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_manual/test_regression_220.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.925176 parsl-2023.4.3/parsl/tests/test_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_monitoring/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_monitoring/test_db_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_monitoring/test_fuzz_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_monitoring/test_memoization_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.925176 parsl-2023.4.3/parsl/tests/test_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_providers/test_local_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.929177 parsl-2023.4.3/parsl/tests/test_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_arg_input_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_at_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_dep_standard_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_depfail_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_fibonacci_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_fibonacci_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_import_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_mapred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_joinapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_type5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_python_apps/test_worker_fail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.933177 parsl-2023.4.3/parsl/tests/test_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_regression/test_1480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_regression/test_1653.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_regression/test_221.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_regression/test_226.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_regression/test_69a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_regression/test_69b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_regression/test_854.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_regression/test_97.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_regression/test_98.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.933177 parsl-2023.4.3/parsl/tests/test_scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_scaling/test_scale_down.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.933177 parsl-2023.4.3/parsl/tests/test_staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_staging/staging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_staging/test_1316.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_staging/test_docs_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_staging/test_docs_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_staging/test_elaborate_noop_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_staging/test_staging_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_staging/test_staging_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_staging/test_staging_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_staging/test_staging_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_staging/test_staging_https_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_swift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_thread_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.933177 parsl-2023.4.3/parsl/tests/test_threads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_threads/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/test_threads/test_lazy_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.937177 parsl-2023.4.3/parsl/tests/workqueue_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/workqueue_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/workqueue_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/workqueue_tests/local_threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3835 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/workqueue_tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/workqueue_tests/wqex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/tests/workqueue_tests/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.937177 parsl-2023.4.3/parsl/usage_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/usage_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/usage_tracking/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-04-03 22:42:52.000000 parsl-2023.4.3/parsl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-03 22:43:02.000000 parsl-2023.4.3/parsl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:43:04.865176 parsl-2023.4.3/parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-03 22:43:04.000000 parsl-2023.4.3/parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15496 2023-04-03 22:43:04.000000 parsl-2023.4.3/parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 22:43:04.000000 parsl-2023.4.3/parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-03 22:43:04.000000 parsl-2023.4.3/parsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-03 22:43:04.000000 parsl-2023.4.3/parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-03 22:43:04.000000 parsl-2023.4.3/parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-03 22:42:52.000000 parsl-2023.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 22:43:04.937177 parsl-2023.4.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-03 22:42:52.000000 parsl-2023.4.3/setup.py
```

### Comparing `parsl-2023.4.24/LICENSE` & `parsl-2023.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/PKG-INFO` & `parsl-2023.4.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.4.24
+Version: 2023.4.3
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.04.24.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.04.03.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2023.4.24/README.rst` & `parsl-2023.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/__init__.py` & `parsl-2023.4.3/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/addresses.py` & `parsl-2023.4.3/parsl/addresses.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/app/app.py` & `parsl-2023.4.3/parsl/app/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/app/bash.py` & `parsl-2023.4.3/parsl/app/bash.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/app/errors.py` & `parsl-2023.4.3/parsl/app/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,25 @@
 from types import TracebackType
 import logging
 from tblib import Traceback
 
 from six import reraise
 
 from parsl.data_provider.files import File
-from parsl.errors import ParslError
 
 logger = logging.getLogger(__name__)
 
 
+class ParslError(Exception):
+    """Base class for all exceptions.
+
+    Only to be invoked when a more specific error is not available.
+    """
+
+
 class AppException(ParslError):
     """An error raised during execution of an app.
 
     What this exception contains depends entirely on context
     """
```

### Comparing `parsl-2023.4.24/parsl/app/futures.py` & `parsl-2023.4.3/parsl/app/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/app/python.py` & `parsl-2023.4.3/parsl/app/python.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/channels/base.py` & `parsl-2023.4.3/parsl/channels/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/channels/errors.py` & `parsl-2023.4.3/parsl/channels/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/channels/local/local.py` & `parsl-2023.4.3/parsl/channels/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/channels/oauth_ssh/oauth_ssh.py` & `parsl-2023.4.3/parsl/channels/oauth_ssh/oauth_ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/channels/ssh/ssh.py` & `parsl-2023.4.3/parsl/channels/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/channels/ssh_il/ssh_il.py` & `parsl-2023.4.3/parsl/channels/ssh_il/ssh_il.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/concurrent/__init__.py` & `parsl-2023.4.3/parsl/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/config.py` & `parsl-2023.4.3/parsl/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from typing import Callable, List, Optional, Sequence, Union
 from typing_extensions import Literal
 
 from parsl.utils import RepresentationMixin
 from parsl.executors.base import ParslExecutor
 from parsl.executors.threads import ThreadPoolExecutor
-from parsl.dataflow.errors import ConfigurationError
+from parsl.dataflow.error import ConfigurationError
 from parsl.dataflow.taskrecord import TaskRecord
 from parsl.monitoring import MonitoringHub
 
 logger = logging.getLogger(__name__)
 
 
 class Config(RepresentationMixin):
```

### Comparing `parsl-2023.4.24/parsl/configs/ASPIRE1.py` & `parsl-2023.4.3/parsl/configs/ASPIRE1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/Azure.py` & `parsl-2023.4.3/parsl/configs/Azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/ad_hoc.py` & `parsl-2023.4.3/parsl/configs/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/bluewaters.py` & `parsl-2023.4.3/parsl/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/bridges.py` & `parsl-2023.4.3/parsl/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/cc_in2p3.py` & `parsl-2023.4.3/parsl/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/comet.py` & `parsl-2023.4.3/parsl/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/cooley.py` & `parsl-2023.4.3/parsl/configs/cooley.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/cori.py` & `parsl-2023.4.3/parsl/configs/cori.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/ec2.py` & `parsl-2023.4.3/parsl/configs/ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/exex_local.py` & `parsl-2023.4.3/parsl/configs/exex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/frontera.py` & `parsl-2023.4.3/parsl/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/illinoiscluster.py` & `parsl-2023.4.3/parsl/configs/illinoiscluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/kubernetes.py` & `parsl-2023.4.3/parsl/configs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/midway.py` & `parsl-2023.4.3/parsl/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/osg.py` & `parsl-2023.4.3/parsl/configs/osg.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/polaris.py` & `parsl-2023.4.3/parsl/configs/polaris.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/stampede2.py` & `parsl-2023.4.3/parsl/configs/stampede2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/summit.py` & `parsl-2023.4.3/parsl/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/theta.py` & `parsl-2023.4.3/parsl/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/toss3_llnl.py` & `parsl-2023.4.3/parsl/configs/toss3_llnl.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/configs/wqex_local.py` & `parsl-2023.4.3/parsl/configs/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/data_provider/data_manager.py` & `parsl-2023.4.3/parsl/data_provider/data_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/data_provider/files.py` & `parsl-2023.4.3/parsl/data_provider/files.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/data_provider/ftp.py` & `parsl-2023.4.3/parsl/data_provider/ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/data_provider/globus.py` & `parsl-2023.4.3/parsl/data_provider/globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/data_provider/http.py` & `parsl-2023.4.3/parsl/data_provider/http.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/data_provider/rsync.py` & `parsl-2023.4.3/parsl/data_provider/rsync.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/data_provider/staging.py` & `parsl-2023.4.3/parsl/data_provider/staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/dataflow/dflow.py` & `parsl-2023.4.3/parsl/dataflow/dflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import parsl
 from parsl.app.errors import RemoteExceptionWrapper
 from parsl.app.futures import DataFuture
 from parsl.channels import Channel
 from parsl.config import Config
 from parsl.data_provider.data_manager import DataManager
 from parsl.data_provider.files import File
-from parsl.dataflow.errors import BadCheckpoint, ConfigurationError, DependencyError, JoinError
+from parsl.dataflow.error import BadCheckpoint, ConfigurationError, DependencyError
 from parsl.dataflow.flow_control import FlowControl, Timer
 from parsl.dataflow.futures import AppFuture
 from parsl.dataflow.memoization import Memoizer
 from parsl.dataflow.rundirs import make_rundir
 from parsl.dataflow.states import States, FINAL_STATES, FINAL_FAILURE_STATES
 from parsl.dataflow.taskrecord import TaskRecord
 from parsl.usage_tracking.usage import UsageTracker
@@ -241,23 +241,20 @@
         task_log_info['task_stdout'] = stdout_name
         task_log_info['task_stderr'] = stderr_name
         task_log_info['task_fail_history'] = ",".join(task_record['fail_history'])
         task_log_info['task_depends'] = None
         if task_record['depends'] is not None:
             task_log_info['task_depends'] = ",".join([str(t.tid) for t in task_record['depends']
                                                       if isinstance(t, AppFuture) or isinstance(t, DataFuture)])
-        task_log_info['task_joins'] = None
-
-        if isinstance(task_record['joins'], list):
-            task_log_info['task_joins'] = ",".join([str(t.tid) for t in task_record['joins']
-                                                    if isinstance(t, AppFuture) or isinstance(t, DataFuture)])
-        elif isinstance(task_record['joins'], Future):
-            task_log_info['task_joins'] = ",".join([str(t.tid) for t in [task_record['joins']]
-                                                    if isinstance(t, AppFuture) or isinstance(t, DataFuture)])
 
+        j = task_record['joins']
+        if isinstance(j, AppFuture) or isinstance(j, DataFuture):
+            task_log_info['task_joins'] = j.tid
+        else:
+            task_log_info['task_joins'] = None
         return task_log_info
 
     def _count_deps(self, depends: Sequence[Future]) -> int:
         """Count the number of unresolved futures in the list depends.
         """
         count = 0
         for dep in depends:
@@ -322,180 +319,110 @@
                     task_record['fail_cost'] += cost
             else:
                 task_record['fail_cost'] += 1
 
             if task_record['status'] == States.dep_fail:
                 logger.info("Task {} failed due to dependency failure so skipping retries".format(task_id))
                 task_record['time_returned'] = datetime.datetime.now()
-                self._send_task_log_info(task_record)
                 with task_record['app_fu']._update_lock:
                     task_record['app_fu'].set_exception(e)
 
             elif task_record['fail_cost'] <= self._config.retries:
 
                 # record the final state for this try before we mutate for retries
                 self.update_task_state(task_record, States.fail_retryable)
                 self._send_task_log_info(task_record)
 
                 task_record['try_id'] += 1
                 self.update_task_state(task_record, States.pending)
                 task_record['try_time_launched'] = None
                 task_record['try_time_returned'] = None
                 task_record['fail_history'] = []
-                self._send_task_log_info(task_record)
 
                 logger.info("Task {} marked for retry".format(task_id))
 
             else:
                 logger.exception("Task {} failed after {} retry attempts".format(task_id,
                                                                                  task_record['try_id']))
                 task_record['time_returned'] = datetime.datetime.now()
                 self.update_task_state(task_record, States.failed)
                 task_record['time_returned'] = datetime.datetime.now()
-                self._send_task_log_info(task_record)
                 with task_record['app_fu']._update_lock:
                     task_record['app_fu'].set_exception(e)
 
         else:
             if task_record['from_memo']:
                 self._complete_task(task_record, States.memo_done, res)
-                self._send_task_log_info(task_record)
             else:
                 if not task_record['join']:
                     self._complete_task(task_record, States.exec_done, res)
-                    self._send_task_log_info(task_record)
                 else:
                     # This is a join task, and the original task's function code has
                     # completed. That means that the future returned by that code
                     # will be available inside the executor future, so we can now
                     # record the inner app ID in monitoring, and add a completion
                     # listener to that inner future.
 
-                    joinable = future.result()
+                    inner_future = future.result()
 
                     # Fail with a TypeError if the joinapp python body returned
                     # something we can't join on.
-                    if isinstance(joinable, Future):
+                    if isinstance(inner_future, Future):
                         self.update_task_state(task_record, States.joining)
-                        task_record['joins'] = joinable
-                        task_record['join_lock'] = threading.Lock()
-                        self._send_task_log_info(task_record)
-                        joinable.add_done_callback(partial(self.handle_join_update, task_record))
-                    elif isinstance(joinable, list) and [j for j in joinable if not isinstance(j, Future)] == []:
-                        self.update_task_state(task_record, States.joining)
-                        task_record['joins'] = joinable
-                        task_record['join_lock'] = threading.Lock()
-                        self._send_task_log_info(task_record)
-                        for inner_future in joinable:
-                            inner_future.add_done_callback(partial(self.handle_join_update, task_record))
+                        task_record['joins'] = inner_future
+                        inner_future.add_done_callback(partial(self.handle_join_update, task_record))
                     else:
                         task_record['time_returned'] = datetime.datetime.now()
                         self.update_task_state(task_record, States.failed)
                         task_record['time_returned'] = datetime.datetime.now()
-                        self._send_task_log_info(task_record)
                         with task_record['app_fu']._update_lock:
-                            task_record['app_fu'].set_exception(
-                                TypeError(f"join_app body must return a Future or list of Futures, got {joinable} of type {type(joinable)}"))
+                            task_record['app_fu'].set_exception(TypeError(f"join_app body must return a Future, got {type(inner_future)}"))
 
         self._log_std_streams(task_record)
 
+        # record current state for this task: maybe a new try, maybe the original try marked as failed, maybe the original try joining
+        self._send_task_log_info(task_record)
+
         # it might be that in the course of the update, we've gone back to being
         # pending - in which case, we should consider ourself for relaunch
         if task_record['status'] == States.pending:
             self.launch_if_ready(task_record)
 
     def handle_join_update(self, task_record: TaskRecord, inner_app_future: AppFuture) -> None:
-        with task_record['join_lock']:
-            # inner_app_future has completed, which is one (potentially of many)
-            # futures the outer task is joining on.
-
-            # If the outer task is joining on a single future, then
-            # use the result of the inner_app_future as the final result of
-            # the outer app future.
-
-            # If the outer task is joining on a list of futures, then
-            # check if the list is all done, and if so, return a list
-            # of the results. Otherwise, this callback can do nothing and
-            # processing will happen in another callback (on the final Future
-            # to complete)
-
-            # There is no retry handling here: inner apps are responsible for
-            # their own retrying, and joining state is responsible for passing
-            # on whatever the result of that retrying was (if any).
-
-            outer_task_id = task_record['id']
-            logger.debug(f"Join callback for task {outer_task_id}, inner_app_future {inner_app_future}")
-
-            if task_record['status'] != States.joining:
-                logger.debug(f"Join callback for task {outer_task_id} skipping because task is not in joining state")
-                return
-
-            joinable = task_record['joins']
-
-            if isinstance(joinable, list):
-                for future in joinable:
-                    if not future.done():
-                        logger.debug(f"A joinable future {future} is not done for task {outer_task_id} - skipping callback")
-                        return  # abandon this callback processing if joinables are not all done
-
-            # now we know each joinable Future is done
-            # so now look for any exceptions
-            exceptions_tids: List[Tuple[BaseException, Optional[str]]]
-            exceptions_tids = []
-            if isinstance(joinable, Future):
-                je = joinable.exception()
-                if je is not None:
-                    if hasattr(joinable, 'task_def'):
-                        tid = joinable.task_def['id']
-                    else:
-                        tid = None
-                    exceptions_tids = [(je, tid)]
-            elif isinstance(joinable, list):
-                for future in joinable:
-                    je = future.exception()
-                    if je is not None:
-                        if hasattr(joinable, 'task_def'):
-                            tid = joinable.task_def['id']
-                        else:
-                            tid = None
-                        exceptions_tids.append((je, tid))
-            else:
-                raise TypeError(f"Unknown joinable type {type(joinable)}")
+        # Use the result of the inner_app_future as the final result of
+        # the outer app future.
 
-            if exceptions_tids:
-                logger.debug("Task {} failed due to failure of an inner join future".format(outer_task_id))
-                e = JoinError(exceptions_tids, outer_task_id)
-                # We keep the history separately, since the future itself could be
-                # tossed.
-                task_record['fail_history'].append(repr(e))
-                task_record['fail_count'] += 1
-                # no need to update the fail cost because join apps are never
-                # retried
+        # There is no retry handling here: inner apps are responsible for
+        # their own retrying, and joining state is responsible for passing
+        # on whatever the result of that retrying was (if any).
+
+        outer_task_id = task_record['id']
+
+        if inner_app_future.exception():
+            e = inner_app_future.exception()
+            logger.debug("Task {} failed due to failure of inner join future".format(outer_task_id))
+            # We keep the history separately, since the future itself could be
+            # tossed.
+            task_record['fail_history'].append(repr(e))
+            task_record['fail_count'] += 1
+            # no need to update the fail cost because join apps are never
+            # retried
 
-                self.update_task_state(task_record, States.failed)
-                task_record['time_returned'] = datetime.datetime.now()
-                with task_record['app_fu']._update_lock:
-                    task_record['app_fu'].set_exception(e)
+            self.update_task_state(task_record, States.failed)
+            task_record['time_returned'] = datetime.datetime.now()
+            with task_record['app_fu']._update_lock:
+                task_record['app_fu'].set_exception(e)
 
-            else:
-                # all the joinables succeeded, so construct a result:
-                if isinstance(joinable, Future):
-                    assert inner_app_future is joinable
-                    res = joinable.result()
-                elif isinstance(joinable, list):
-                    res = []
-                    for future in joinable:
-                        res.append(future.result())
-                else:
-                    raise TypeError(f"Unknown joinable type {type(joinable)}")
-                self._complete_task(task_record, States.exec_done, res)
+        else:
+            res = inner_app_future.result()
+            self._complete_task(task_record, States.exec_done, res)
 
-            self._log_std_streams(task_record)
+        self._log_std_streams(task_record)
 
-            self._send_task_log_info(task_record)
+        self._send_task_log_info(task_record)
 
     def handle_app_update(self, task_record: TaskRecord, future: AppFuture) -> None:
         """This function is called as a callback when an AppFuture
         is in its final state.
 
         It will trigger post-app processing such as checkpointing.
```

### Comparing `parsl-2023.4.24/parsl/dataflow/errors.py` & `parsl-2023.4.3/parsl/dataflow/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Sequence, Tuple
+from typing import Sequence, Tuple
 
 
 class DataFlowException(Exception):
     """Base class for all exceptions.
 
     Only to be invoked when only a more specific error is not available.
 
@@ -47,21 +47,7 @@
     def __init__(self, dependent_exceptions_tids: Sequence[Tuple[Exception, str]], task_id: int) -> None:
         self.dependent_exceptions_tids = dependent_exceptions_tids
         self.task_id = task_id
 
     def __str__(self) -> str:
         dep_tids = [tid for (exception, tid) in self.dependent_exceptions_tids]
         return "Dependency failure for task {} with failed dependencies from tasks {}".format(self.task_id, dep_tids)
-
-
-class JoinError(DataFlowException):
-    """Error raised if apps joining into a join_app raise exceptions.
-       There can be several exceptions (one from each joining app),
-       and JoinError collects them all together.
-    """
-    def __init__(self, dependent_exceptions_tids: Sequence[Tuple[BaseException, Optional[str]]], task_id: int) -> None:
-        self.dependent_exceptions_tids = dependent_exceptions_tids
-        self.task_id = task_id
-
-    def __str__(self) -> str:
-        dep_tids = [tid for (exception, tid) in self.dependent_exceptions_tids]
-        return "Join failure for task {} with failed join dependencies from tasks {}".format(self.task_id, dep_tids)
```

### Comparing `parsl-2023.4.24/parsl/dataflow/flow_control.py` & `parsl-2023.4.3/parsl/dataflow/flow_control.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/dataflow/futures.py` & `parsl-2023.4.3/parsl/dataflow/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/dataflow/job_error_handler.py` & `parsl-2023.4.3/parsl/dataflow/job_error_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/dataflow/job_status_poller.py` & `parsl-2023.4.3/parsl/dataflow/job_status_poller.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/dataflow/memoization.py` & `parsl-2023.4.3/parsl/dataflow/memoization.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/dataflow/rundirs.py` & `parsl-2023.4.3/parsl/dataflow/rundirs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/dataflow/states.py` & `parsl-2023.4.3/parsl/dataflow/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/dataflow/strategy.py` & `parsl-2023.4.3/parsl/dataflow/strategy.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/dataflow/taskrecord.py` & `parsl-2023.4.3/parsl/dataflow/taskrecord.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import threading
 import datetime
 from typing_extensions import TypedDict
 from concurrent.futures import Future
 
 # only for type checking:
-from typing import Any, Callable, Dict, Optional, List, Sequence, TYPE_CHECKING, Union
+from typing import Any, Callable, Dict, Optional, List, Sequence, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from parsl.dataflow.futures import AppFuture
 
 from parsl.dataflow.states import States
 
 
@@ -80,15 +80,10 @@
     try_id: int
 
     resource_specification: Dict[str, Any]
 
     join: bool
     """Is this a join_app?"""
 
-    joins: Union[None, Future, List[Future]]
+    joins: Optional[Future]
     """If this is a join app and the python body has executed, then this
-    contains the Future or list of Futures that the join app will join."""
-
-    join_lock: threading.Lock
-    """Restricts access to end-of-join behavior to ensure that joins
-    only complete once, even if several joining Futures complete close
-    together in time."""
+    contains the Future that the join app will join."""
```

### Comparing `parsl-2023.4.24/parsl/errors.py` & `parsl-2023.4.3/parsl/errors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-from typing import List
-
+from parsl.app.errors import ParslError
 
-class ParslError(Exception):
-    """Base class for all exceptions.
-
-    Only to be invoked when a more specific error is not available.
-    """
+from typing import List
 
 
 class OptionalModuleMissing(ParslError):
     ''' Error raised when a required module is missing for a optional/extra component
     '''
 
     def __init__(self, module_names: List[str], reason: str):
```

### Comparing `parsl-2023.4.24/parsl/executors/base.py` & `parsl-2023.4.3/parsl/executors/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/executors/errors.py` & `parsl-2023.4.3/parsl/executors/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Exceptions raise by Executors."""
-from parsl.errors import ParslError
+from parsl.app.errors import ParslError
 from parsl.executors.base import ParslExecutor
 
 
 class ExecutorError(ParslError):
     """Base class for executor related exceptions.
 
     Only to be invoked when only a more specific error is not available.
```

### Comparing `parsl-2023.4.24/parsl/executors/extreme_scale/executor.py` & `parsl-2023.4.3/parsl/executors/extreme_scale/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/executors/extreme_scale/mpi_worker_pool.py` & `parsl-2023.4.3/parsl/executors/extreme_scale/mpi_worker_pool.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/executors/flux/execute_parsl_task.py` & `parsl-2023.4.3/parsl/executors/flux/execute_parsl_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/executors/flux/executor.py` & `parsl-2023.4.3/parsl/executors/flux/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/executors/flux/flux_instance_manager.py` & `parsl-2023.4.3/parsl/executors/flux/flux_instance_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/executors/high_throughput/executor.py` & `parsl-2023.4.3/parsl/executors/high_throughput/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from concurrent.futures import Future
 import typeguard
 import logging
 import threading
 import queue
 import datetime
 import pickle
-import warnings
 from multiprocessing import Queue
 from typing import Dict, Sequence  # noqa F401 (used in type annotation)
 from typing import List, Optional, Tuple, Union
 import math
 
 from parsl.serialize import pack_apply_message, deserialize
 from parsl.app.errors import RemoteExceptionWrapper
@@ -129,21 +128,19 @@
         will check the available memory at startup and limit the number of workers such that
         the there's sufficient memory for each worker. Default: None
 
     max_workers : int
         Caps the number of workers launched per node. Default: infinity
 
     cpu_affinity: string
-        Whether or how each worker process sets thread affinity. Options include "none" to forgo
+        Whether or how each worker process sets thread affinity. Options are "none" to forgo
         any CPU affinity configuration, "block" to assign adjacent cores to workers
         (ex: assign 0-1 to worker 0, 2-3 to worker 1), and
         "alternating" to assign cores to workers in round-robin
         (ex: assign 0,2 to worker 0, 1,3 to worker 1).
-        The "block-reverse" option assigns adjacent cores to workers, but assigns
-        the CPUs with large indices to low index workers (ex: assign 2-3 to worker 1, 0,1 to worker 2)
 
     available_accelerators: int | list
         Accelerators available for workers to use. Each worker will be pinned to exactly one of the provided
         accelerators, and no more workers will be launched than the number of accelerators.
 
         Either provide the list of accelerator names or the number available. If a number is provided,
         Parsl will create names as integers starting with 0.
@@ -199,15 +196,15 @@
                  working_dir: Optional[str] = None,
                  worker_debug: bool = False,
                  cores_per_worker: float = 1.0,
                  mem_per_worker: Optional[float] = None,
                  max_workers: Union[int, float] = float('inf'),
                  cpu_affinity: str = 'none',
                  available_accelerators: Union[int, Sequence[str]] = (),
-                 start_method: str = 'spawn',
+                 start_method: str = 'fork',
                  prefetch_capacity: int = 0,
                  heartbeat_threshold: int = 120,
                  heartbeat_period: int = 30,
                  poll_period: int = 10,
                  address_probe_timeout: Optional[int] = None,
                  worker_logdir_root: Optional[str] = None,
                  block_error_handler: bool = True):
@@ -252,17 +249,14 @@
         # Raise errors for incompatible settings
         if start_method not in _start_methods:
             raise ValueError(f'Start method "{start_method}" not recognized. Expected one of: {", ".join(_start_methods)}')
         if start_method == "thread" and cpu_affinity != "none":
             raise ValueError('Thread affinity is not available with start method: "thread"')
         if start_method == "thread" and len(available_accelerators) > 0:
             raise ValueError('Accelerator pinning not available with start method: "thread"')
-        if start_method == "fork":
-            logger.warning("The 'fork' start method is deprecated")
-            warnings.warn("The 'fork' start method is deprecated")
 
         # Determine the number of workers per node
         self._workers_per_node = min(max_workers, mem_slots, cpu_slots)
         if len(self.available_accelerators) > 0:
             self._workers_per_node = min(self._workers_per_node, len(available_accelerators))
         if self._workers_per_node == float('inf'):
             self._workers_per_node = 1  # our best guess-- we do not have any provider hints
@@ -536,28 +530,29 @@
         return outstanding_c
 
     @property
     def connected_workers(self):
         workers = self.command_client.run("WORKERS")
         return workers
 
+    @property
     def connected_managers(self):
-        managers = self.command_client.run("MANAGERS")
-        return managers
+        workers = self.command_client.run("MANAGERS")
+        return workers
 
     def _hold_block(self, block_id):
         """ Sends hold command to all managers which are in a specific block
 
         Parameters
         ----------
         block_id : str
              Block identifier of the block to be put on hold
         """
 
-        managers = self.connected_managers()
+        managers = self.connected_managers
 
         for manager in managers:
             if manager['block_id'] == block_id:
                 logger.debug("Sending hold to manager: {}".format(manager['manager']))
                 self.hold_worker(manager['manager'])
 
     def submit(self, func, resource_specification, *args, **kwargs):
@@ -665,15 +660,15 @@
         -------
         List of job_ids marked for termination
         """
         logger.debug(f"Scale in called, blocks={blocks}, block_ids={block_ids}")
         if block_ids:
             block_ids_to_kill = block_ids
         else:
-            managers = self.connected_managers()
+            managers = self.connected_managers
             block_info = {}  # block id -> list( tasks, idle duration )
             for manager in managers:
                 if not manager['active']:
                     continue
                 b_id = manager['block_id']
                 if b_id not in block_info:
                     block_info[b_id] = [0, float('inf')]
```

### Comparing `parsl-2023.4.24/parsl/executors/high_throughput/interchange.py` & `parsl-2023.4.3/parsl/executors/high_throughput/interchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,21 +347,19 @@
         hub_channel = self._create_monitoring_channel()
 
         poll_period = self.poll_period
 
         start = time.time()
 
         self._task_puller_thread = threading.Thread(target=self.task_puller,
-                                                    name="Interchange-Task-Puller",
-                                                    daemon=True)
+                                                    name="Interchange-Task-Puller")
         self._task_puller_thread.start()
 
         self._command_thread = threading.Thread(target=self._command_server,
-                                                name="Interchange-Command",
-                                                daemon=True)
+                                                name="Interchange-Command")
         self._command_thread.start()
 
         kill_event = threading.Event()
 
         poller = zmq.Poller()
         poller.register(self.task_outgoing, zmq.POLLIN)
         poller.register(self.results_incoming, zmq.POLLIN)
```

### Comparing `parsl-2023.4.24/parsl/executors/high_throughput/probe.py` & `parsl-2023.4.3/parsl/executors/high_throughput/probe.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/executors/high_throughput/process_worker_pool.py` & `parsl-2023.4.3/parsl/executors/high_throughput/process_worker_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
              Number of seconds after which a heartbeat message is sent to the interchange, and workers
              are checked for liveness.
 
         poll_period : int
              Timeout period used by the manager in milliseconds. Default: 10ms
 
         cpu_affinity : str
-             Whether or how each worker should force its affinity to different CPUs
+             Whether each worker should force its affinity to different CPUs
 
         available_accelerators: list of str
             List of accelerators available to the workers. Default: Empty list
 
         start_method: str
             What method to use to start new worker processes. Choices are fork, spawn, and thread.
             Default: fork
@@ -545,17 +545,14 @@
         avail_cores = sorted(os.sched_getaffinity(0))  # Get the available processors
         cores_per_worker = len(avail_cores) // pool_size
         assert cores_per_worker > 0, "Affinity does not work if there are more workers than cores"
 
         # Determine this worker's cores
         if cpu_affinity == "block":
             my_cores = avail_cores[cores_per_worker * worker_id:cores_per_worker * (worker_id + 1)]
-        elif cpu_affinity == "block-reverse":
-            cpu_worker_id = pool_size - worker_id - 1  # To assign in reverse order
-            my_cores = avail_cores[cores_per_worker * cpu_worker_id:cores_per_worker * (cpu_worker_id + 1)]
         elif cpu_affinity == "alternating":
             my_cores = avail_cores[worker_id::pool_size]
         else:
             raise ValueError("Affinity strategy {} is not supported".format(cpu_affinity))
 
         # Set the affinity for OpenMP
         #  See: https://hpc-tutorials.llnl.gov/openmp/ProcessThreadAffinity.pdf
@@ -672,15 +669,15 @@
                         help="Heartbeat threshold in seconds. Uses manager default unless set")
     parser.add_argument("--address_probe_timeout", default=30,
                         help="Timeout to probe for viable address to interchange. Default: 30s")
     parser.add_argument("--poll", default=10,
                         help="Poll period used in milliseconds")
     parser.add_argument("-r", "--result_port", required=True,
                         help="REQUIRED: Result port for posting results to the interchange")
-    parser.add_argument("--cpu-affinity", type=str, choices=["none", "block", "alternating", "block-reverse"],
+    parser.add_argument("--cpu-affinity", type=str, choices=["none", "block", "alternating"],
                         help="Whether/how workers should control CPU affinity.")
     parser.add_argument("--available-accelerators", type=str, nargs="*",
                         help="Names of available accelerators")
     parser.add_argument("--start-method", type=str, choices=["fork", "spawn", "thread"], default="fork",
                         help="Method used to start new worker processes")
 
     args = parser.parse_args()
```

### Comparing `parsl-2023.4.24/parsl/executors/high_throughput/zmq_pipes.py` & `parsl-2023.4.3/parsl/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/executors/status_handling.py` & `parsl-2023.4.3/parsl/executors/status_handling.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/executors/swift_t.py` & `parsl-2023.4.3/parsl/executors/swift_t.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/executors/threads.py` & `parsl-2023.4.3/parsl/executors/threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/executors/workqueue/exec_parsl_function.py` & `parsl-2023.4.3/parsl/executors/workqueue/exec_parsl_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,18 +60,17 @@
     # remap any keyword argument in the same way, but we need to treat
     # "inputs" and "outputs" specially because they are lists, and
     # "stdout" and "stderr", because they are not File's.
     for kwarg, maybe_file in fn_kwargs.items():
         if kwarg in ["inputs", "outputs"]:
             remap_list_of_files(mapping, maybe_file)
         if kwarg in ["stdout", "stderr"]:
-            if maybe_file:
-                (fname, mode) = get_std_fname_mode(kwarg, maybe_file)
-                if fname in mapping:
-                    fn_kwargs[kwarg] = (mapping[fname], mode)
+            (fname, mode) = get_std_fname_mode(kwarg, maybe_file)
+            if fname in mapping:
+                fn_kwargs[kwarg] = (mapping[fname], mode)
         else:
             # Treat anything else as a possible File to be remapped.
             remap_location(mapping, maybe_file)
 
 
 def unpack_function(function_info, user_namespace):
     if "source code" in function_info:
```

### Comparing `parsl-2023.4.24/parsl/executors/workqueue/executor.py` & `parsl-2023.4.3/parsl/executors/workqueue/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -743,32 +743,32 @@
                 for fu in self.tasks.values():
                     if not fu.done():
                         fu.set_exception(WorkQueueFailure("work queue executor failed to execute the task."))
         logger.debug("Exiting Collector Thread")
 
 
 @wrap_with_logs
-def _work_queue_submit_wait(*,
-                            port_mailbox: multiprocessing.Queue,
-                            task_queue: multiprocessing.Queue,
-                            launch_cmd: str,
-                            collector_queue: multiprocessing.Queue,
-                            data_dir: str,
-                            full: bool,
-                            shared_fs: bool,
-                            autolabel: bool,
-                            autolabel_window: int,
-                            autocategory: bool,
-                            max_retries: Optional[int],
-                            should_stop,  # multiprocessing.Value is an awkward type alias from inside multiprocessing
-                            port: int,
-                            wq_log_dir: str,
-                            project_password_file: Optional[str],
-                            project_name: Optional[str],
-                            coprocess: bool) -> int:
+def _work_queue_submit_wait(port_mailbox=None,
+                            task_queue=multiprocessing.Queue(),
+                            launch_cmd=None,
+                            env=None,
+                            collector_queue=multiprocessing.Queue(),
+                            data_dir=".",
+                            full=False,
+                            shared_fs=False,
+                            autolabel=False,
+                            autolabel_window=None,
+                            autocategory=False,
+                            max_retries=0,
+                            should_stop=None,
+                            port=WORK_QUEUE_DEFAULT_PORT,
+                            wq_log_dir=None,
+                            project_password_file=None,
+                            project_name=None,
+                            coprocess=False):
     """Thread to handle Parsl app submissions to the Work Queue objects.
     Takes in Parsl functions submitted using submit(), and creates a
     Work Queue task with the appropriate specifications, which is then
     submitted to Work Queue. After tasks are completed, processes the
     exit status and exit code of the task, and sends results to the
     Work Queue collector thread.
     To avoid python's global interpreter lock with work queue's wait, this
@@ -835,22 +835,20 @@
             # Obtain task from task_queue
             try:
                 task = task_queue.get(timeout=1)
                 logger.debug("Removing task from queue")
             except queue.Empty:
                 continue
 
-            try:
-                pkg_pfx = ""
-                if task.env_pkg is not None:
-                    if package_run_script is None:
-                        raise ValueError("package_run_script must be specified")
-                    pkg_pfx = "./{} -e {} ".format(os.path.basename(package_run_script),
-                                                   os.path.basename(task.env_pkg))
+            pkg_pfx = ""
+            if task.env_pkg is not None:
+                pkg_pfx = "./{} -e {} ".format(os.path.basename(package_run_script),
+                                               os.path.basename(task.env_pkg))
 
+            try:
                 if not coprocess:
                     # Create command string
                     logger.debug(launch_cmd)
                     command_str = launch_cmd.format(package_prefix=pkg_pfx,
                                                     mapping=os.path.basename(task.map_file),
                                                     function=os.path.basename(task.function_file),
                                                     result=os.path.basename(task.result_file))
@@ -892,14 +890,19 @@
 
             if max_retries is not None:
                 logger.debug(f"Specifying max_retries {max_retries}")
                 t.specify_max_retries(max_retries)
             else:
                 logger.debug("Not specifying max_retries")
 
+            # Specify environment variables for the task
+            if env is not None:
+                for var in env:
+                    t.specify_environment_variable(var, env[var])
+
             if task.env_pkg is not None:
                 t.specify_input_file(package_run_script, cache=True)
                 t.specify_input_file(task.env_pkg, cache=True)
 
             # Specify script, and data/result files for task
             t.specify_input_file(exec_parsl_function.__file__, cache=True)
             t.specify_input_file(task.function_file, cache=False)
```

### Comparing `parsl-2023.4.24/parsl/executors/workqueue/parsl_coprocess.py` & `parsl-2023.4.3/parsl/executors/workqueue/parsl_coprocess.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/executors/workqueue/parsl_coprocess_stub.py` & `parsl-2023.4.3/parsl/executors/workqueue/parsl_coprocess_stub.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/launchers/__init__.py` & `parsl-2023.4.3/parsl/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/launchers/launchers.py` & `parsl-2023.4.3/parsl/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/log_utils.py` & `parsl-2023.4.3/parsl/log_utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/db_manager.py` & `parsl-2023.4.3/parsl/monitoring/db_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 logger = logging.getLogger("database_manager")
 
 X = TypeVar('X')
 
 try:
     import sqlalchemy as sa
-    from sqlalchemy import Column, Text, Float, Boolean, BigInteger, Integer, DateTime, PrimaryKeyConstraint, Table
+    from sqlalchemy import Column, Text, Float, Boolean, Integer, DateTime, PrimaryKeyConstraint, Table
     from sqlalchemy.orm import Mapper
     from sqlalchemy.orm import mapperlib
     from sqlalchemy.orm import sessionmaker
     from sqlalchemy.ext.declarative import declarative_base
 except ImportError:
     _sqlalchemy_enabled = False
 else:
@@ -41,16 +41,16 @@
 BLOCK = 'block'          # Block table include the status for block polling
 
 
 class Database:
 
     if not _sqlalchemy_enabled:
         raise OptionalModuleMissing(['sqlalchemy'],
-                                    ("Monitoring requires the sqlalchemy library."
-                                     " Install monitoring dependencies with: pip install 'parsl[monitoring]'"))
+                                    ("Default database logging requires the sqlalchemy library."
+                                     " Enable monitoring support with: pip install 'parsl[monitoring]'"))
     Base = declarative_base()
 
     def __init__(self,
                  url: str = 'sqlite:///runinfomonitoring.db',
                  ):
 
         self.eng = sa.create_engine(url)
@@ -64,17 +64,20 @@
 
         self.meta.reflect(bind=self.eng)
 
         Session = sessionmaker(bind=self.eng)
         self.session = Session()
 
     def _get_mapper(self, table_obj: Table) -> Mapper:
-        all_mappers = set()
-        for mapper_registry in mapperlib._all_registries():  # type: ignore
-            all_mappers.update(mapper_registry.mappers)
+        if hasattr(mapperlib, '_all_registries'):
+            all_mappers = set()
+            for mapper_registry in mapperlib._all_registries():
+                all_mappers.update(mapper_registry.mappers)
+        else:  # SQLAlchemy <1.4
+            all_mappers = mapperlib._mapper_registry  # type: ignore
         mapper_gen = (
             mapper for mapper in all_mappers
             if table_obj in mapper.tables
         )
         try:
             mapper = next(mapper_gen)
             second_mapper = next(mapper_gen, False)
@@ -125,15 +128,16 @@
         user = Column(Text, nullable=False)
         rundir = Column(Text, nullable=False)
         tasks_failed_count = Column(Integer, nullable=False)
         tasks_completed_count = Column(Integer, nullable=False)
 
     class Status(Base):
         __tablename__ = STATUS
-        task_id = Column(Integer, nullable=False)
+        task_id = Column(Integer, sa.ForeignKey(
+            'task.task_id'), nullable=False)
         task_status_name = Column(Text, nullable=False)
         timestamp = Column(DateTime, nullable=False)
         run_id = Column(Text, sa.ForeignKey('workflow.run_id'), nullable=False)
         try_id = Column('try_id', Integer, nullable=False)
         __table_args__ = (
             PrimaryKeyConstraint('task_id', 'run_id',
                                  'task_status_name', 'timestamp'),
@@ -198,15 +202,15 @@
         __tablename__ = NODE
         id = Column('id', Integer, nullable=False, primary_key=True, autoincrement=True)
         run_id = Column('run_id', Text, nullable=False)
         hostname = Column('hostname', Text, nullable=False)
         uid = Column('uid', Text, nullable=False)
         block_id = Column('block_id', Text, nullable=False)
         cpu_count = Column('cpu_count', Integer, nullable=False)
-        total_memory = Column('total_memory', BigInteger, nullable=False)
+        total_memory = Column('total_memory', Integer, nullable=False)
         active = Column('active', Boolean, nullable=False)
         worker_count = Column('worker_count', Integer, nullable=False)
         python_v = Column('python_v', Text, nullable=False)
         timestamp = Column('timestamp', DateTime, nullable=False)
         last_heartbeat = Column('last_heartbeat', DateTime, nullable=False)
 
     class Block(Base):
@@ -219,16 +223,18 @@
         status = Column("status", Text, nullable=False)
         __table_args__ = (
             PrimaryKeyConstraint('run_id', 'block_id', 'executor_label', 'timestamp'),
         )
 
     class Resource(Base):
         __tablename__ = RESOURCE
-        try_id = Column('try_id', Integer, nullable=False)
-        task_id = Column('task_id', Integer, nullable=False)
+        try_id = Column('try_id', Integer, sa.ForeignKey(
+            'try.try_id'), nullable=False)
+        task_id = Column('task_id', Integer, sa.ForeignKey(
+            'task.task_id'), nullable=False)
         run_id = Column('run_id', Text, sa.ForeignKey(
             'workflow.run_id'), nullable=False)
         timestamp = Column('timestamp', DateTime, nullable=False)
         resource_monitoring_interval = Column(
             'resource_monitoring_interval', Float, nullable=True)
         psutil_process_pid = Column(
             'psutil_process_pid', Integer, nullable=True)
```

### Comparing `parsl-2023.4.24/parsl/monitoring/monitoring.py` & `parsl-2023.4.3/parsl/monitoring/monitoring.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/queries/pandas.py` & `parsl-2023.4.3/parsl/monitoring/queries/pandas.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/radios.py` & `parsl-2023.4.3/parsl/monitoring/radios.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/remote.py` & `parsl-2023.4.3/parsl/monitoring/remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/types.py` & `parsl-2023.4.3/parsl/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/app.py` & `parsl-2023.4.3/parsl/monitoring/visualization/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/models.py` & `parsl-2023.4.3/parsl/monitoring/visualization/models.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/plots/default/task_plots.py` & `parsl-2023.4.3/parsl/monitoring/visualization/plots/default/task_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/plots/default/workflow_plots.py` & `parsl-2023.4.3/parsl/monitoring/visualization/plots/default/workflow_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py` & `parsl-2023.4.3/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/static/parsl-logo-white.png` & `parsl-2023.4.3/parsl/monitoring/visualization/static/parsl-logo-white.png`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/templates/app.html` & `parsl-2023.4.3/parsl/monitoring/visualization/templates/app.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/templates/dag.html` & `parsl-2023.4.3/parsl/monitoring/visualization/templates/dag.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/templates/layout.html` & `parsl-2023.4.3/parsl/monitoring/visualization/templates/layout.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/templates/resource_usage.html` & `parsl-2023.4.3/parsl/monitoring/visualization/templates/resource_usage.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/templates/task.html` & `parsl-2023.4.3/parsl/monitoring/visualization/templates/task.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/templates/workflow.html` & `parsl-2023.4.3/parsl/monitoring/visualization/templates/workflow.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/templates/workflows_summary.html` & `parsl-2023.4.3/parsl/monitoring/visualization/templates/workflows_summary.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/monitoring/visualization/views.py` & `parsl-2023.4.3/parsl/monitoring/visualization/views.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/multiprocessing.py` & `parsl-2023.4.3/parsl/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/process_loggers.py` & `parsl-2023.4.3/parsl/process_loggers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/providers/__init__.py` & `parsl-2023.4.3/parsl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/providers/ad_hoc/ad_hoc.py` & `parsl-2023.4.3/parsl/providers/ad_hoc/ad_hoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 import time
 
 from parsl.channels import LocalChannel
 from parsl.launchers import SimpleLauncher
 from parsl.providers.base import ExecutionProvider, JobStatus, JobState
-from parsl.providers.errors import ScriptPathError
+from parsl.providers.error import ScriptPathError
 from parsl.utils import RepresentationMixin
 
 logger = logging.getLogger(__name__)
 
 
 class AdHocProvider(ExecutionProvider, RepresentationMixin):
     """ Ad-hoc execution provider
```

### Comparing `parsl-2023.4.24/parsl/providers/aws/aws.py` & `parsl-2023.4.3/parsl/providers/aws/aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import os
 import time
 from string import Template
 
-from parsl.dataflow.errors import ConfigurationError
+from parsl.dataflow.error import ConfigurationError
 from parsl.providers.aws.template import template_string
 from parsl.providers.base import ExecutionProvider, JobState, JobStatus
 from parsl.errors import OptionalModuleMissing
 from parsl.utils import RepresentationMixin
 from parsl.launchers import SingleNodeLauncher
 
 logger = logging.getLogger(__name__)
```

### Comparing `parsl-2023.4.24/parsl/providers/azure/azure.py` & `parsl-2023.4.3/parsl/providers/azure/azure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import os
 import time
 from string import Template
 
-from parsl.dataflow.errors import ConfigurationError
+from parsl.dataflow.error import ConfigurationError
 from parsl.providers.azure.template import template_string
 from parsl.providers.base import ExecutionProvider, JobState, JobStatus
 from parsl.errors import OptionalModuleMissing
 from parsl.utils import RepresentationMixin
 from parsl.launchers import SingleNodeLauncher
 
 logger = logging.getLogger(__name__)
```

### Comparing `parsl-2023.4.24/parsl/providers/base.py` & `parsl-2023.4.3/parsl/providers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import os
 from abc import ABCMeta, abstractmethod, abstractproperty
-from enum import IntEnum
+from enum import Enum
 import logging
 from typing import Any, Dict, List, Optional
 
 from parsl.channels.base import Channel
 
 logger = logging.getLogger(__name__)
 
 
-class JobState(IntEnum):
+class JobState(bytes, Enum):
     """Defines a set of states that a job can be in"""
-    UNKNOWN = 0
-    PENDING = 1
-    RUNNING = 2
-    CANCELLED = 3
-    COMPLETED = 4
-    FAILED = 5
-    TIMEOUT = 6
-    HELD = 7
-
-    def __str__(self) -> str:
-        return self.__class__.__name__ + "." + self.name
-
-
-TERMINAL_STATES = [JobState.CANCELLED, JobState.COMPLETED, JobState.FAILED,
-                   JobState.TIMEOUT]
+    def __new__(cls, value: int, terminal: bool, status_name: str) -> "JobState":
+        obj = bytes.__new__(cls, [value])
+        obj._value_ = value
+        obj.terminal = terminal
+        obj.status_name = status_name
+        return obj
+
+    value: int
+    terminal: bool
+    status_name: str
+
+    UNKNOWN = (0, False, "UNKNOWN")
+    PENDING = (1, False, "PENDING")
+    RUNNING = (2, False, "RUNNING")
+    CANCELLED = (3, True, "CANCELLED")
+    COMPLETED = (4, True, "COMPLETED")
+    FAILED = (5, True, "FAILED")
+    TIMEOUT = (6, True, "TIMEOUT")
+    HELD = (7, False, "HELD")
 
 
 class JobStatus(object):
     """Encapsulates a job state together with other details:
 
     Args:
         state: The machine-readable state of the job this status refers to
@@ -46,19 +50,19 @@
         self.message = message
         self.exit_code = exit_code
         self.stdout_path = stdout_path
         self.stderr_path = stderr_path
 
     @property
     def terminal(self) -> bool:
-        return self.state in TERMINAL_STATES
+        return self.state.terminal
 
     @property
     def status_name(self) -> str:
-        return self.state.name
+        return self.state.status_name
 
     def __repr__(self) -> str:
         if self.message is not None:
             extra = f"state={self.state} message={self.message}".format(self.state, self.message)
         else:
             extra = f"state={self.state}".format(self.state)
         return f"<{type(self).__module__}.{type(self).__qualname__} object at {hex(id(self))}, {extra}>"
```

### Comparing `parsl-2023.4.24/parsl/providers/cluster_provider.py` & `parsl-2023.4.3/parsl/providers/cluster_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from abc import abstractmethod
 from string import Template
 
-from parsl.providers.errors import SchedulerMissingArgs, ScriptPathError
+from parsl.providers.error import SchedulerMissingArgs, ScriptPathError
 from parsl.launchers.error import BadLauncher
 from parsl.providers.base import ExecutionProvider
 
 logger = logging.getLogger(__name__)
 
 
 class ClusterProvider(ExecutionProvider):
```

### Comparing `parsl-2023.4.24/parsl/providers/cobalt/cobalt.py` & `parsl-2023.4.3/parsl/providers/cobalt/cobalt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 import time
 
-from parsl.providers.errors import ScaleOutFailed
+from parsl.providers.error import ScaleOutFailed
 from parsl.channels import LocalChannel
 from parsl.launchers import AprunLauncher
 from parsl.providers.cobalt.template import template_string
 from parsl.providers.cluster_provider import ClusterProvider
 from parsl.providers.base import JobState, JobStatus
 from parsl.utils import RepresentationMixin, wtime_to_minutes
```

### Comparing `parsl-2023.4.24/parsl/providers/condor/condor.py` & `parsl-2023.4.3/parsl/providers/condor/condor.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from parsl.channels import LocalChannel
 from parsl.providers.base import JobState, JobStatus
 from parsl.utils import RepresentationMixin
 from parsl.launchers import SingleNodeLauncher
 from parsl.providers.condor.template import template_string
 from parsl.providers.cluster_provider import ClusterProvider
-from parsl.providers.errors import ScaleOutFailed
+from parsl.providers.error import ScaleOutFailed
 
 logger = logging.getLogger(__name__)
 
 from typing import Dict, List, Optional
 from parsl.channels.base import Channel
 from parsl.launchers.launchers import Launcher
```

### Comparing `parsl-2023.4.24/parsl/providers/condor/template.py` & `parsl-2023.4.3/parsl/providers/condor/template.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/providers/errors.py` & `parsl-2023.4.3/parsl/providers/error.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/providers/googlecloud/googlecloud.py` & `parsl-2023.4.3/parsl/providers/googlecloud/googlecloud.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/providers/grid_engine/grid_engine.py` & `parsl-2023.4.3/parsl/providers/grid_engine/grid_engine.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/providers/kubernetes/kube.py` & `parsl-2023.4.3/parsl/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/providers/local/local.py` & `parsl-2023.4.3/parsl/providers/local/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 import time
 
 from parsl.channels import LocalChannel
 from parsl.launchers import SingleNodeLauncher
 from parsl.providers.base import ExecutionProvider, JobState, JobStatus
-from parsl.providers.errors import SchedulerMissingArgs, ScriptPathError, SubmitException
+from parsl.providers.error import SchedulerMissingArgs, ScriptPathError, SubmitException
 from parsl.utils import RepresentationMixin
 
 logger = logging.getLogger(__name__)
 
 
 class LocalProvider(ExecutionProvider, RepresentationMixin):
     """ Local Execution Provider
```

### Comparing `parsl-2023.4.24/parsl/providers/lsf/lsf.py` & `parsl-2023.4.3/parsl/providers/lsf/lsf.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/providers/pbspro/pbspro.py` & `parsl-2023.4.3/parsl/providers/pbspro/pbspro.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/providers/slurm/slurm.py` & `parsl-2023.4.3/parsl/providers/slurm/slurm.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/providers/torque/torque.py` & `parsl-2023.4.3/parsl/providers/torque/torque.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/serialize/base.py` & `parsl-2023.4.3/parsl/serialize/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/serialize/concretes.py` & `parsl-2023.4.3/parsl/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/serialize/facade.py` & `parsl-2023.4.3/parsl/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/ad_hoc_cluster_htex.py` & `parsl-2023.4.3/parsl/tests/configs/ad_hoc_cluster_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/azure_single_node.py` & `parsl-2023.4.3/parsl/tests/configs/azure_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/bluewaters.py` & `parsl-2023.4.3/parsl/tests/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/bridges.py` & `parsl-2023.4.3/parsl/tests/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/cc_in2p3.py` & `parsl-2023.4.3/parsl/tests/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/comet.py` & `parsl-2023.4.3/parsl/tests/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/cooley_htex.py` & `parsl-2023.4.3/parsl/tests/configs/cooley_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/cori.py` & `parsl-2023.4.3/parsl/tests/configs/cori.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/ec2_single_node.py` & `parsl-2023.4.3/parsl/tests/configs/ec2_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/ec2_spot.py` & `parsl-2023.4.3/parsl/tests/configs/ec2_spot.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/exex_local.py` & `parsl-2023.4.3/parsl/tests/configs/exex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/frontera.py` & `parsl-2023.4.3/parsl/tests/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/htex_ad_hoc_cluster.py` & `parsl-2023.4.3/parsl/tests/configs/htex_ad_hoc_cluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/htex_local.py` & `parsl-2023.4.3/parsl/tests/configs/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/htex_local_alternate.py` & `parsl-2023.4.3/parsl/tests/configs/htex_local_alternate.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/htex_local_intask_staging.py` & `parsl-2023.4.3/parsl/tests/configs/htex_local_intask_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/htex_local_rsync_staging.py` & `parsl-2023.4.3/parsl/tests/configs/htex_local_rsync_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/local_threads_globus.py` & `parsl-2023.4.3/parsl/tests/configs/local_threads_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/midway.py` & `parsl-2023.4.3/parsl/tests/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/nscc_singapore.py` & `parsl-2023.4.3/parsl/tests/configs/nscc_singapore.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/osg_htex.py` & `parsl-2023.4.3/parsl/tests/configs/osg_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/petrelkube.py` & `parsl-2023.4.3/parsl/tests/configs/petrelkube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/summit.py` & `parsl-2023.4.3/parsl/tests/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/swan_htex.py` & `parsl-2023.4.3/parsl/tests/configs/swan_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/theta.py` & `parsl-2023.4.3/parsl/tests/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/user_opts.py` & `parsl-2023.4.3/parsl/tests/configs/user_opts.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/configs/workqueue_blocks.py` & `parsl-2023.4.3/parsl/tests/configs/workqueue_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/conftest.py` & `parsl-2023.4.3/parsl/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 def pytest_addoption(parser):
     """Add parsl-specific command-line options to pytest.
     """
     parser.addoption(
         '--config',
         action='store',
         metavar='CONFIG',
-        type=str,
+        type='string',
         nargs=1,
         required=True,
         help="run with parsl CONFIG; use 'local' to run locally-defined config"
     )
 
 
 def pytest_configure(config):
```

### Comparing `parsl-2023.4.24/parsl/tests/integration/latency.py` & `parsl-2023.4.3/parsl/tests/integration/latency.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/integration/test_channels/test_local_channel.py` & `parsl-2023.4.3/parsl/tests/integration/test_channels/test_local_channel.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/integration/test_channels/test_scp_1.py` & `parsl-2023.4.3/parsl/tests/integration/test_channels/test_scp_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/integration/test_channels/test_ssh_1.py` & `parsl-2023.4.3/parsl/tests/integration/test_channels/test_ssh_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/integration/test_channels/test_ssh_errors.py` & `parsl-2023.4.3/parsl/tests/integration/test_channels/test_ssh_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/integration/test_channels/test_ssh_file_transport.py` & `parsl-2023.4.3/parsl/tests/integration/test_channels/test_ssh_file_transport.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/integration/test_channels/test_ssh_interactive.py` & `parsl-2023.4.3/parsl/tests/integration/test_channels/test_ssh_interactive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/integration/test_stress/test_python_simple.py` & `parsl-2023.4.3/parsl/tests/integration/test_stress/test_python_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/integration/test_stress/test_python_threads.py` & `parsl-2023.4.3/parsl/tests/integration/test_stress/test_python_threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/manual_tests/htex_local.py` & `parsl-2023.4.3/parsl/tests/manual_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/manual_tests/test_ad_hoc_htex.py` & `parsl-2023.4.3/parsl/tests/manual_tests/test_ad_hoc_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/manual_tests/test_basic.py` & `parsl-2023.4.3/parsl/tests/manual_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py` & `parsl-2023.4.3/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/manual_tests/test_log_filter.py` & `parsl-2023.4.3/parsl/tests/manual_tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/manual_tests/test_memory_limits.py` & `parsl-2023.4.3/parsl/tests/manual_tests/test_memory_limits.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/manual_tests/test_udp_simple.py` & `parsl-2023.4.3/parsl/tests/manual_tests/test_udp_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/manual_tests/test_worker_count.py` & `parsl-2023.4.3/parsl/tests/manual_tests/test_worker_count.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/site_tests/site_config_selector.py` & `parsl-2023.4.3/parsl/tests/site_tests/site_config_selector.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/site_tests/test_provider.py` & `parsl-2023.4.3/parsl/tests/site_tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/site_tests/test_site.py` & `parsl-2023.4.3/parsl/tests/site_tests/test_site.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/sites/test_affinity.py` & `parsl-2023.4.3/parsl/tests/sites/test_affinity.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/sites/test_concurrent.py` & `parsl-2023.4.3/parsl/tests/sites/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/sites/test_dynamic_executor.py` & `parsl-2023.4.3/parsl/tests/sites/test_dynamic_executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/sites/test_ec2.py` & `parsl-2023.4.3/parsl/tests/sites/test_ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/sites/test_local_adhoc.py` & `parsl-2023.4.3/parsl/tests/sites/test_local_adhoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/sites/test_start_method.py` & `parsl-2023.4.3/parsl/tests/sites/test_start_method.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/sites/test_worker_info.py` & `parsl-2023.4.3/parsl/tests/sites/test_worker_info.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_aalst_patterns.py` & `parsl-2023.4.3/parsl/tests/test_aalst_patterns.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_bash_apps/test_apptimeout.py` & `parsl-2023.4.3/parsl/tests/test_bash_apps/test_apptimeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_bash_apps/test_basic.py` & `parsl-2023.4.3/parsl/tests/test_bash_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_bash_apps/test_error_codes.py` & `parsl-2023.4.3/parsl/tests/test_bash_apps/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_bash_apps/test_file_bug_1.py` & `parsl-2023.4.3/parsl/tests/test_bash_apps/test_file_bug_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_bash_apps/test_kwarg_storage.py` & `parsl-2023.4.3/parsl/tests/test_bash_apps/test_kwarg_storage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_bash_apps/test_memoize.py` & `parsl-2023.4.3/parsl/tests/test_bash_apps/test_memoize.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_bash_apps/test_memoize_ignore_args.py` & `parsl-2023.4.3/parsl/tests/test_bash_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py` & `parsl-2023.4.3/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_bash_apps/test_multiline.py` & `parsl-2023.4.3/parsl/tests/test_bash_apps/test_multiline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_bash_apps/test_pipeline.py` & `parsl-2023.4.3/parsl/tests/test_bash_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_bash_apps/test_stdout.py` & `parsl-2023.4.3/parsl/tests/test_bash_apps/test_stdout.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,17 +44,18 @@
     """
 
     fn = echo_to_streams("Hello world", stdout=spec, stderr='t.err')
 
     try:
         fn.result()
     except Exception as e:
-        assert isinstance(e, TypeError) or isinstance(e, perror.BadStdStreamFile), "Exception is wrong type"
+        assert isinstance(
+            e, perror.BadStdStreamFile), "Expected BadStdStreamFile, got: {0}".format(type(e))
     else:
-        assert False, "Did not raise expected exception"
+        assert False, "Did not raise expected exception BadStdStreamFile"
 
     return
 
 
 @pytest.mark.issue363
 def test_bad_stderr_file():
 
@@ -63,16 +64,17 @@
     out = "t2.out"
     err = "/bad/dir/t2.err"
 
     fn = echo_to_streams("Hello world", stdout=out, stderr=err)
 
     try:
         fn.result()
-    except perror.BadStdStreamFile:
-        pass
+    except Exception as e:
+        assert isinstance(
+            e, perror.BadStdStreamFile), "Expected BadStdStreamFile, got: {0}".format(type(e))
     else:
         assert False, "Did not raise expected exception BadStdStreamFile"
 
     return
 
 
 @pytest.mark.issue363
```

### Comparing `parsl-2023.4.24/parsl/tests/test_callables.py` & `parsl-2023.4.3/parsl/tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_channels/test_large_output.py` & `parsl-2023.4.3/parsl/tests/test_channels/test_large_output.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_checkpointing/test_periodic.py` & `parsl-2023.4.3/parsl/tests/test_checkpointing/test_periodic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_checkpointing/test_python_checkpoint_1.py` & `parsl-2023.4.3/parsl/tests/test_checkpointing/test_python_checkpoint_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_checkpointing/test_python_checkpoint_2.py` & `parsl-2023.4.3/parsl/tests/test_checkpointing/test_python_checkpoint_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_checkpointing/test_python_checkpoint_3.py` & `parsl-2023.4.3/parsl/tests/test_checkpointing/test_python_checkpoint_3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_checkpointing/test_regression_232.py` & `parsl-2023.4.3/parsl/tests/test_checkpointing/test_regression_232.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_checkpointing/test_regression_233.py` & `parsl-2023.4.3/parsl/tests/test_checkpointing/test_regression_233.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_checkpointing/test_regression_239.py` & `parsl-2023.4.3/parsl/tests/test_checkpointing/test_regression_239.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_checkpointing/test_task_exit.py` & `parsl-2023.4.3/parsl/tests/test_checkpointing/test_task_exit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_data/test_file.py` & `parsl-2023.4.3/parsl/tests/test_data/test_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_data/test_file_apps.py` & `parsl-2023.4.3/parsl/tests/test_data/test_file_apps.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_data/test_file_staging.py` & `parsl-2023.4.3/parsl/tests/test_data/test_file_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_docs/test_from_slides.py` & `parsl-2023.4.3/parsl/tests/test_docs/test_from_slides.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_docs/test_tutorial_1.py` & `parsl-2023.4.3/parsl/tests/test_docs/test_tutorial_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_docs/test_workflow1.py` & `parsl-2023.4.3/parsl/tests/test_docs/test_workflow1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_docs/test_workflow2.py` & `parsl-2023.4.3/parsl/tests/test_docs/test_workflow2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_docs/test_workflow3.py` & `parsl-2023.4.3/parsl/tests/test_docs/test_workflow3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_docs/test_workflow4.py` & `parsl-2023.4.3/parsl/tests/test_docs/test_workflow4.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_error_handling/test_htex_missing_worker.py` & `parsl-2023.4.3/parsl/tests/test_error_handling/test_htex_missing_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_error_handling/test_htex_worker_failure.py` & `parsl-2023.4.3/parsl/tests/test_error_handling/test_htex_worker_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_error_handling/test_python_walltime.py` & `parsl-2023.4.3/parsl/tests/test_error_handling/test_python_walltime.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_error_handling/test_rand_fail.py` & `parsl-2023.4.3/parsl/tests/test_error_handling/test_rand_fail.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     #     \     |      /
     #       App_Final
 
     fu_final = sleep_fail(1, 0, 0, inputs=fus_2)
 
     try:
         print("Final status : ", fu_final.result())
-    except parsl.dataflow.errors.DependencyError as e:
+    except parsl.dataflow.error.DependencyError as e:
         print("Caught the right exception")
         print("Exception : ", e)
     except Exception as e:
         assert 5 == 1, "Expected DependencyError got : %s" % e
     else:
         print("Shoot! no errors ")
```

### Comparing `parsl-2023.4.24/parsl/tests/test_error_handling/test_resource_spec.py` & `parsl-2023.4.3/parsl/tests/test_error_handling/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_error_handling/test_retries.py` & `parsl-2023.4.3/parsl/tests/test_error_handling/test_retries.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_error_handling/test_retry_handler.py` & `parsl-2023.4.3/parsl/tests/test_error_handling/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_error_handling/test_retry_handler_failure.py` & `parsl-2023.4.3/parsl/tests/test_error_handling/test_retry_handler_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_error_handling/test_serialization_fail.py` & `parsl-2023.4.3/parsl/tests/test_error_handling/test_serialization_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_error_handling/test_wrap_with_logs.py` & `parsl-2023.4.3/parsl/tests/test_error_handling/test_wrap_with_logs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_flowcontrol/test_one_block.py` & `parsl-2023.4.3/parsl/tests/test_flowcontrol/test_one_block.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_flowcontrol/test_python.py` & `parsl-2023.4.3/parsl/tests/test_flowcontrol/test_python.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_flux.py` & `parsl-2023.4.3/parsl/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_manual/test_regression_220.py` & `parsl-2023.4.3/parsl/tests/test_manual/test_regression_220.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_monitoring/test_basic.py` & `parsl-2023.4.3/parsl/tests/test_monitoring/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_monitoring/test_db_locks.py` & `parsl-2023.4.3/parsl/tests/test_monitoring/test_db_locks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_monitoring/test_fuzz_zmq.py` & `parsl-2023.4.3/parsl/tests/test_monitoring/test_fuzz_zmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_monitoring/test_memoization_representation.py` & `parsl-2023.4.3/parsl/tests/test_monitoring/test_memoization_representation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_providers/test_local_provider.py` & `parsl-2023.4.3/parsl/tests/test_providers/test_local_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_arg_input_types.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_arg_input_types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_at_scale.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_at_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_basic.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_dep_standard_futures.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_dep_standard_futures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import parsl
-from parsl.dataflow.errors import DependencyError
+from parsl.dataflow.error import DependencyError
 from concurrent.futures import Future
 
 
 @parsl.python_app
 def copy_app(v):
     return v
```

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_depfail_propagation.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_depfail_propagation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from parsl import python_app
-from parsl.dataflow.errors import DependencyError
+from parsl.dataflow.error import DependencyError
 
 
 @python_app
 def fails():
     raise ValueError("Deliberate failure")
```

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_fail.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_fail.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     #     \     |      /
     # App_Final
 
     fu_final = sleep_fail(1, 0, 0, inputs=fus_2)
 
     try:
         print("Final status : ", fu_final.result())
-    except parsl.dataflow.errors.DependencyError as e:
+    except parsl.dataflow.error.DependencyError as e:
         print("Caught the right exception")
         print("Exception : ", e)
     except Exception as e:
         assert False, "Expected DependencyError but got: %s" % e
     else:
         raise RuntimeError("Expected DependencyError, but got no exception")
```

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_fibonacci_iterative.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_fibonacci_iterative.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_fibonacci_recursive.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_fibonacci_recursive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_futures.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_garbage_collect.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_garbage_collect.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_import_fail.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_import_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_mapred.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_mapred.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_1.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_2.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_4.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_4.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_5.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_5.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_memoize_ignore_args.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_outputs.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_outputs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_overview.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_overview.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_pipeline.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_simple.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_type5.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_type5.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_python_apps/test_worker_fail.py` & `parsl-2023.4.3/parsl/tests/test_python_apps/test_worker_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_regression/test_1480.py` & `parsl-2023.4.3/parsl/tests/test_regression/test_1480.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py` & `parsl-2023.4.3/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_regression/test_1653.py` & `parsl-2023.4.3/parsl/tests/test_regression/test_1653.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_regression/test_221.py` & `parsl-2023.4.3/parsl/tests/test_regression/test_221.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_regression/test_226.py` & `parsl-2023.4.3/parsl/tests/test_regression/test_226.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_regression/test_69a.py` & `parsl-2023.4.3/parsl/tests/test_regression/test_69a.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_regression/test_69b.py` & `parsl-2023.4.3/parsl/tests/test_regression/test_69b.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_regression/test_854.py` & `parsl-2023.4.3/parsl/tests/test_regression/test_854.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_regression/test_97.py` & `parsl-2023.4.3/parsl/tests/test_regression/test_97.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_regression/test_98.py` & `parsl-2023.4.3/parsl/tests/test_regression/test_98.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_scaling/test_scale_down.py` & `parsl-2023.4.3/parsl/tests/test_scaling/test_scale_down.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,32 +49,32 @@
 # in CI.
 @pytest.mark.local
 def test_scale_out():
     logger.info("start")
     dfk = parsl.dfk()
 
     logger.info("initial asserts")
-    assert len(dfk.executors['htex_local'].connected_managers()) == 0, "Expected 0 managers at start"
+    assert len(dfk.executors['htex_local'].connected_managers) == 0, "Expected 0 managers at start"
     assert dfk.executors['htex_local'].outstanding == 0, "Expected 0 tasks at start"
 
     logger.info("launching tasks")
     fus = [sleeper(i) for i in [15 for x in range(0, 10)]]
 
     logger.info("waiting for warm up")
     time.sleep(15)
 
     logger.info("asserting 5 managers")
-    assert len(dfk.executors['htex_local'].connected_managers()) == 5, "Expected 5 managers after some time"
+    assert len(dfk.executors['htex_local'].connected_managers) == 5, "Expected 5 managers after some time"
 
     logger.info("waiting for all futures to complete")
     [x.result() for x in fus]
 
     logger.info("asserting 0 outstanding tasks after completion")
     assert dfk.executors['htex_local'].outstanding == 0, "Expected 0 outstanding tasks after future completion"
 
     logger.info("waiting a while for scale down")
     time.sleep(25)
 
     logger.info("asserting 2 managers remain")
-    assert len(dfk.executors['htex_local'].connected_managers()) == 2, "Expected 2 managers when no tasks, lower bound by min_blocks"
+    assert len(dfk.executors['htex_local'].connected_managers) == 2, "Expected 2 managers when no tasks, lower bound by min_blocks"
 
     logger.info("test passed")
```

### Comparing `parsl-2023.4.24/parsl/tests/test_staging/staging_provider.py` & `parsl-2023.4.3/parsl/tests/test_staging/staging_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_staging/test_1316.py` & `parsl-2023.4.3/parsl/tests/test_staging/test_1316.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_staging/test_docs_1.py` & `parsl-2023.4.3/parsl/tests/test_staging/test_docs_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_staging/test_elaborate_noop_file.py` & `parsl-2023.4.3/parsl/tests/test_staging/test_elaborate_noop_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_staging/test_staging_ftp.py` & `parsl-2023.4.3/parsl/tests/test_staging/test_staging_ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_staging/test_staging_ftp_in_task.py` & `parsl-2023.4.3/parsl/tests/test_staging/test_staging_ftp_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_staging/test_staging_globus.py` & `parsl-2023.4.3/parsl/tests/test_staging/test_staging_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_staging/test_staging_https.py` & `parsl-2023.4.3/parsl/tests/test_staging/test_staging_https.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_staging/test_staging_https_in_task.py` & `parsl-2023.4.3/parsl/tests/test_staging/test_staging_https_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_summary.py` & `parsl-2023.4.3/parsl/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_swift.py` & `parsl-2023.4.3/parsl/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_thread_parallelism.py` & `parsl-2023.4.3/parsl/tests/test_thread_parallelism.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_threads/test_configs.py` & `parsl-2023.4.3/parsl/tests/test_threads/test_configs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/test_threads/test_lazy_errors.py` & `parsl-2023.4.3/parsl/tests/test_threads/test_lazy_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/workqueue_tests/htex_local.py` & `parsl-2023.4.3/parsl/tests/workqueue_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/workqueue_tests/test_scale.py` & `parsl-2023.4.3/parsl/tests/workqueue_tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/workqueue_tests/wqex_condor.py` & `parsl-2023.4.3/parsl/tests/workqueue_tests/wqex_condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/tests/workqueue_tests/wqex_local.py` & `parsl-2023.4.3/parsl/tests/workqueue_tests/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/usage_tracking/usage.py` & `parsl-2023.4.3/parsl/usage_tracking/usage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.4.24/parsl/utils.py` & `parsl-2023.4.3/parsl/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,26 +101,34 @@
 
     if(not(os.path.isdir(last_checkpoint))):
         return []
 
     return [last_checkpoint]
 
 
-@typeguard.typechecked
 def get_std_fname_mode(fdname: str, stdfspec: Union[str, Tuple[str, str]]) -> Tuple[str, str]:
     import parsl.app.errors as pe
-    if isinstance(stdfspec, str):
+    if stdfspec is None:
+        return None, None
+    elif isinstance(stdfspec, str):
         fname = stdfspec
         mode = 'a+'
     elif isinstance(stdfspec, tuple):
         if len(stdfspec) != 2:
             msg = (f"std descriptor {fdname} has incorrect tuple length "
                    f"{len(stdfspec)}")
             raise pe.BadStdStreamFile(msg, TypeError('Bad Tuple Length'))
         fname, mode = stdfspec
+        if not isinstance(fname, str) or not isinstance(mode, str):
+            msg = (f"std descriptor {fdname} has unexpected type "
+                   f"{type(stdfspec)}")
+            raise pe.BadStdStreamFile(msg, TypeError('Bad Tuple Type'))
+    else:
+        msg = f"std descriptor {fdname} has unexpected type {type(stdfspec)}"
+        raise pe.BadStdStreamFile(msg, TypeError('Bad Tuple Type'))
     return fname, mode
 
 
 @contextmanager
 def wait_for_file(path: str, seconds: int = 10) -> Generator[None, None, None]:
     for i in range(0, int(seconds * 100)):
         time.sleep(seconds / 100.)
@@ -243,19 +251,19 @@
             return assemble_multiline(args, kwargs)
 
 
 class AtomicIDCounter:
     """A class to allocate counter-style IDs, in a thread-safe way.
     """
 
-    def __init__(self) -> None:
+    def __init__(self):
         self.count = 0
         self.lock = threading.Lock()
 
-    def get_id(self) -> int:
+    def get_id(self):
         with self.lock:
             new_id = self.count
             self.count += 1
             return new_id
 
 
 def setproctitle(title: str) -> None:
```

### Comparing `parsl-2023.4.24/parsl.egg-info/PKG-INFO` & `parsl-2023.4.3/parsl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.4.24
+Version: 2023.4.3
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.04.24.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.04.03.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2023.4.24/parsl.egg-info/SOURCES.txt` & `parsl-2023.4.3/parsl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 parsl.egg-info/top_level.txt
 parsl/app/__init__.py
 parsl/app/app.py
 parsl/app/bash.py
 parsl/app/errors.py
 parsl/app/futures.py
 parsl/app/python.py
-parsl/benchmark/__init__.py
-parsl/benchmark/perf.py
 parsl/channels/__init__.py
 parsl/channels/base.py
 parsl/channels/errors.py
 parsl/channels/local/__init__.py
 parsl/channels/local/local.py
 parsl/channels/oauth_ssh/__init__.py
 parsl/channels/oauth_ssh/oauth_ssh.py
@@ -71,15 +69,15 @@
 parsl/data_provider/ftp.py
 parsl/data_provider/globus.py
 parsl/data_provider/http.py
 parsl/data_provider/rsync.py
 parsl/data_provider/staging.py
 parsl/dataflow/__init__.py
 parsl/dataflow/dflow.py
-parsl/dataflow/errors.py
+parsl/dataflow/error.py
 parsl/dataflow/executor_status.py
 parsl/dataflow/flow_control.py
 parsl/dataflow/futures.py
 parsl/dataflow/job_error_handler.py
 parsl/dataflow/job_status_poller.py
 parsl/dataflow/memoization.py
 parsl/dataflow/rundirs.py
@@ -146,15 +144,15 @@
 parsl/monitoring/visualization/templates/resource_usage.html
 parsl/monitoring/visualization/templates/task.html
 parsl/monitoring/visualization/templates/workflow.html
 parsl/monitoring/visualization/templates/workflows_summary.html
 parsl/providers/__init__.py
 parsl/providers/base.py
 parsl/providers/cluster_provider.py
-parsl/providers/errors.py
+parsl/providers/error.py
 parsl/providers/ad_hoc/__init__.py
 parsl/providers/ad_hoc/ad_hoc.py
 parsl/providers/aws/__init__.py
 parsl/providers/aws/aws.py
 parsl/providers/aws/template.py
 parsl/providers/azure/__init__.py
 parsl/providers/azure/azure.py
@@ -369,15 +367,14 @@
 parsl/tests/test_python_apps/test_worker_fail.py
 parsl/tests/test_regression/__init__.py
 parsl/tests/test_regression/test_1480.py
 parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
 parsl/tests/test_regression/test_1653.py
 parsl/tests/test_regression/test_221.py
 parsl/tests/test_regression/test_226.py
-parsl/tests/test_regression/test_2652.py
 parsl/tests/test_regression/test_69a.py
 parsl/tests/test_regression/test_69b.py
 parsl/tests/test_regression/test_854.py
 parsl/tests/test_regression/test_97.py
 parsl/tests/test_regression/test_98.py
 parsl/tests/test_scaling/__init__.py
 parsl/tests/test_scaling/test_scale_down.py
```

### Comparing `parsl-2023.4.24/parsl.egg-info/requires.txt` & `parsl-2023.4.3/parsl.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 tblib
 requests
 paramiko
 psutil>=5.5.1
 setproctitle
 
 [all]
-sqlalchemy<2,>=1.4
+sqlalchemy<2,>=1.3.0
 pydot
 networkx<2.6,>=2.5
 Flask>=1.0.2
 flask_sqlalchemy
 pandas<2
 plotly
 python-daemon
@@ -62,15 +62,15 @@
 [gssapi]
 python-gssapi
 
 [kubernetes]
 kubernetes
 
 [monitoring]
-sqlalchemy<2,>=1.4
+sqlalchemy<2,>=1.3.0
 pydot
 networkx<2.6,>=2.5
 Flask>=1.0.2
 flask_sqlalchemy
 pandas<2
 plotly
 python-daemon
```

### Comparing `parsl-2023.4.24/setup.py` & `parsl-2023.4.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     exec(f.read())
 
 with open('requirements.txt') as f:
     install_requires = f.readlines()
 
 extras_require = {
     'monitoring' : [
-        'sqlalchemy>=1.4,<2',
+        'sqlalchemy>=1.3.0,<2',
         'pydot',
         'networkx>=2.5,<2.6',
         'Flask>=1.0.2',
         'flask_sqlalchemy',
         'pandas<2',
         'plotly',
         'python-daemon'
@@ -66,10 +66,9 @@
         'Programming Language :: Python :: 3.9',
     ],
     keywords=['Workflows', 'Scientific computing'],
     entry_points={'console_scripts':
       [
        'parsl-globus-auth=parsl.data_provider.globus:cli_run',
        'parsl-visualize=parsl.monitoring.visualization.app:cli_run',
-       'parsl-perf=parsl.benchmark.perf:cli_run',
       ]}
 )
```

