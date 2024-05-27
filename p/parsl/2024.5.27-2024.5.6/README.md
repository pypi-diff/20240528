# Comparing `tmp/parsl-2024.5.27.tar.gz` & `tmp/parsl-2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsl-2024.5.27.tar", last modified: Mon May 27 22:42:42 2024, max compression
+gzip compressed data, was "parsl-2024.5.6.tar", last modified: Mon May  6 22:42:36 2024, max compression
```

## Comparing `parsl-2024.5.27.tar` & `parsl-2024.5.6.tar`

### file list

```diff
@@ -1,551 +1,545 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.346873 parsl-2024.5.27/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 22:42:39.000000 parsl-2024.5.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-27 22:42:39.000000 parsl-2024.5.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-27 22:42:42.346873 parsl-2024.5.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-27 22:42:39.000000 parsl-2024.5.27/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.278873 parsl-2024.5.27/parsl/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.282873 parsl-2024.5.27/parsl/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/app/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/app/futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/app/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.282873 parsl-2024.5.27/parsl/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/benchmark/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.282873 parsl-2024.5.27/parsl/channels/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/channels/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.282873 parsl-2024.5.27/parsl/channels/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/channels/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/channels/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.282873 parsl-2024.5.27/parsl/channels/oauth_ssh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/channels/oauth_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/channels/oauth_ssh/oauth_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.282873 parsl-2024.5.27/parsl/channels/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/channels/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/channels/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.282873 parsl-2024.5.27/parsl/channels/ssh_il/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/channels/ssh_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/channels/ssh_il/ssh_il.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.282873 parsl-2024.5.27/parsl/concurrent/
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.286873 parsl-2024.5.27/parsl/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/ASPIRE1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/Azure.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/expanse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/illinoiscluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/osg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/polaris.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/stampede2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/toss3_llnl.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/configs/wqex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/curvezmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.286873 parsl-2024.5.27/parsl/data_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/data_provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/data_provider/file_noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/data_provider/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/data_provider/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/data_provider/globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/data_provider/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/data_provider/rsync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/data_provider/staging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/data_provider/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.290873 parsl-2024.5.27/parsl/dataflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/dataflow/dependency_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    66320 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/dataflow/dflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/dataflow/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/dataflow/futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/dataflow/memoization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/dataflow/rundirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/dataflow/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/dataflow/taskrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.290873 parsl-2024.5.27/parsl/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.290873 parsl-2024.5.27/parsl/executors/flux/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/flux/execute_parsl_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/flux/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/flux/flux_instance_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.294873 parsl-2024.5.27/parsl/executors/high_throughput/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/high_throughput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/high_throughput/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    37265 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/high_throughput/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    31904 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/high_throughput/interchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/high_throughput/manager_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/high_throughput/monitoring_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/high_throughput/mpi_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/high_throughput/mpi_prefix_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/high_throughput/mpi_resource_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/high_throughput/probe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    41267 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/high_throughput/process_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/high_throughput/zmq_pipes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.294873 parsl-2024.5.27/parsl/executors/radical/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/radical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21024 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/radical/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/radical/rpex_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/radical/rpex_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/radical/rpex_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/status_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.294873 parsl-2024.5.27/parsl/executors/taskvine/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/taskvine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/taskvine/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/taskvine/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    31806 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/taskvine/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/taskvine/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/taskvine/factory_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25822 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/taskvine/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/taskvine/manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/taskvine/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.294873 parsl-2024.5.27/parsl/executors/workqueue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/workqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/workqueue/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/workqueue/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    49312 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/workqueue/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5737 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/workqueue/parsl_coprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      735 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/executors/workqueue/parsl_coprocess_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.298873 parsl-2024.5.27/parsl/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/jobs/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/jobs/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/jobs/job_status_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/jobs/states.py
--rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/jobs/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.298873 parsl-2024.5.27/parsl/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/launchers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/launchers/launchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.298873 parsl-2024.5.27/parsl/monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37021 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/message_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.298873 parsl-2024.5.27/parsl/monitoring/queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/queries/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/radios.py
--rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.298873 parsl-2024.5.27/parsl/monitoring/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.298873 parsl-2024.5.27/parsl/monitoring/visualization/plots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.302873 parsl-2024.5.27/parsl/monitoring/visualization/plots/default/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/plots/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/plots/default/task_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/plots/default/workflow_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.302873 parsl-2024.5.27/parsl/monitoring/visualization/static/
--rwxr-xr-x   0 runner    (1001) docker     (127)    14199 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/static/parsl-logo-white.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/static/parsl-monitor.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.302873 parsl-2024.5.27/parsl/monitoring/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/templates/app.html
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/templates/dag.html
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/templates/resource_usage.html
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/templates/task.html
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/templates/workflow.html
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/templates/workflows_summary.html
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/monitoring/visualization/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/process_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.302873 parsl-2024.5.27/parsl/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.302873 parsl-2024.5.27/parsl/providers/ad_hoc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/ad_hoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/ad_hoc/ad_hoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.302873 parsl-2024.5.27/parsl/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29009 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/aws/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.302873 parsl-2024.5.27/parsl/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18396 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/azure/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/azure/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/cluster_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.302873 parsl-2024.5.27/parsl/providers/cobalt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/cobalt/cobalt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/cobalt/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.306873 parsl-2024.5.27/parsl/providers/condor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/condor/condor.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/condor/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.306873 parsl-2024.5.27/parsl/providers/googlecloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/googlecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/googlecloud/googlecloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.306873 parsl-2024.5.27/parsl/providers/grid_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/grid_engine/grid_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/grid_engine/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.306873 parsl-2024.5.27/parsl/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/kubernetes/kube.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/kubernetes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.306873 parsl-2024.5.27/parsl/providers/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.306873 parsl-2024.5.27/parsl/providers/lsf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/lsf/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/lsf/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.306873 parsl-2024.5.27/parsl/providers/pbspro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/pbspro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/pbspro/pbspro.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/pbspro/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.306873 parsl-2024.5.27/parsl/providers/slurm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/slurm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.306873 parsl-2024.5.27/parsl/providers/torque/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/torque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/torque/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/providers/torque/torque.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.306873 parsl-2024.5.27/parsl/serialize/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/serialize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/serialize/concretes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/serialize/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/serialize/facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/serialize/proxystore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.310873 parsl-2024.5.27/parsl/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/callables_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.314873 parsl-2024.5.27/parsl/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/ad_hoc_cluster_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/azure_single_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/cooley_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/ec2_single_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/ec2_spot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/htex_ad_hoc_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/htex_local_alternate.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/htex_local_intask_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/htex_local_rsync_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_radical.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_radical_mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_threads_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_threads_checkpoint_periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_threads_checkpoint_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_threads_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_threads_globus.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_threads_http_in_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_threads_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/local_threads_no_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/nscc_singapore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/osg_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/petrelkube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/swan_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/taskvine_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/user_opts.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/configs/workqueue_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)    14633 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.314873 parsl-2024.5.27/parsl/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/latency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.314873 parsl-2024.5.27/parsl/tests/integration/test_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.318873 parsl-2024.5.27/parsl/tests/integration/test_channels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_channels/test_local_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_channels/test_scp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_channels/test_ssh_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_channels/test_ssh_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_channels/test_ssh_file_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_channels/test_ssh_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_parsl_load_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.318873 parsl-2024.5.27/parsl/tests/integration/test_stress/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_stress/test_python_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/integration/test_stress/test_python_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.318873 parsl-2024.5.27/parsl/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/manual_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/manual_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/manual_tests/test_ad_hoc_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/manual_tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/manual_tests/test_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/manual_tests/test_memory_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/manual_tests/test_oauth_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/manual_tests/test_regression_220.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/manual_tests/test_udp_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/manual_tests/test_worker_count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.318873 parsl-2024.5.27/parsl/tests/scaling_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/scaling_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/scaling_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/scaling_tests/local_threads.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3751 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/scaling_tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/scaling_tests/vineex_condor.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/scaling_tests/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/scaling_tests/wqex_condor.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/scaling_tests/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.322873 parsl-2024.5.27/parsl/tests/site_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/site_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/site_tests/site_config_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/site_tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/site_tests/test_site.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.322873 parsl-2024.5.27/parsl/tests/sites/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/sites/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/sites/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/sites/test_dynamic_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/sites/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/sites/test_launchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/sites/test_local_adhoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.322873 parsl-2024.5.27/parsl/tests/sites/test_mpi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/sites/test_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/sites/test_worker_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_aalst_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.322873 parsl-2024.5.27/parsl/tests/test_bash_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/test_apptimeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/test_keyword_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/test_kwarg_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/test_memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/test_std_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_bash_apps/test_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_callables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.322873 parsl-2024.5.27/parsl/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_channels/test_large_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.326873 parsl-2024.5.27/parsl/tests/test_checkpointing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_checkpointing/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_checkpointing/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_checkpointing/test_regression_233.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_checkpointing/test_regression_239.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_checkpointing/test_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_curvezmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.326873 parsl-2024.5.27/parsl/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_docs/test_from_slides.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_docs/test_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_docs/test_tutorial_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_docs/test_workflow1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_docs/test_workflow2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_docs/test_workflow4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.326873 parsl-2024.5.27/parsl/tests/test_error_handling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_error_handling/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_error_handling/test_python_walltime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_error_handling/test_rand_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_error_handling/test_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_error_handling/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_error_handling/test_retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_error_handling/test_retry_handler_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_error_handling/test_serialization_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_error_handling/test_wrap_with_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.326873 parsl-2024.5.27/parsl/tests/test_flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.330873 parsl-2024.5.27/parsl/tests/test_htex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_command_client_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_connected_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_cpu_affinity_explicit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_disconnected_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_drain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_manager_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_managers_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_missing_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_multiple_disconnected_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_worker_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_htex/test_zmq_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.330873 parsl-2024.5.27/parsl/tests/test_monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_monitoring/test_app_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_monitoring/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_monitoring/test_db_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_monitoring/test_fuzz_zmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_monitoring/test_incomplete_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_monitoring/test_memoization_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_monitoring/test_stdouterr.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_monitoring/test_viz_colouring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.334873 parsl-2024.5.27/parsl/tests/test_mpi_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_mpi_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_mpi_apps/test_bad_mpi_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_mpi_apps/test_mpi_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_mpi_apps/test_mpi_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_mpi_apps/test_mpiex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_mpi_apps/test_resource_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.334873 parsl-2024.5.27/parsl/tests/test_providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_providers/test_cobalt_deprecation_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_providers/test_local_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_providers/test_pbspro_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_providers/test_slurm_instantiate.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_providers/test_slurm_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_providers/test_submiterror_deprecation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.338873 parsl-2024.5.27/parsl/tests/test_python_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_arg_input_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_dep_standard_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_depfail_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_fibonacci_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_fibonacci_recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_import_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_lifted.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_mapred.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_memoize_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_memoize_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_memoize_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_memoize_joinapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_pluggable_future_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_python_apps/test_type5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.338873 parsl-2024.5.27/parsl/tests/test_radical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_radical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_radical/test_mpi_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.338873 parsl-2024.5.27/parsl/tests/test_regression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_regression/test_1480.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_regression/test_1653.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_regression/test_221.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_regression/test_226.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_regression/test_2652.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_regression/test_69a.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_regression/test_854.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_regression/test_97_parallelism_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_regression/test_98.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.342873 parsl-2024.5.27/parsl/tests/test_scaling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_scaling/test_block_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_scaling/test_regression_1621.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_scaling/test_scale_down.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_scaling/test_scale_down_htex_unregistered.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_scaling/test_shutdown_scalein.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.342873 parsl-2024.5.27/parsl/tests/test_serialization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_serialization/test_2555_caching_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_serialization/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_serialization/test_htex_code_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_serialization/test_pack_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_serialization/test_proxystore_configured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_serialization/test_proxystore_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.342873 parsl-2024.5.27/parsl/tests/test_shutdown/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_shutdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_shutdown/test_kill_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.342873 parsl-2024.5.27/parsl/tests/test_staging/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/staging_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_1316.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_docs_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_docs_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_elaborate_noop_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_file_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_file_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_output_chain_filenames.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_staging_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_staging_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_staging_globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_staging_https.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_staging_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_zip_in.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_zip_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_staging/test_zip_to_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_thread_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.346873 parsl-2024.5.27/parsl/tests/test_threads/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_threads/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_threads/test_lazy_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.346873 parsl-2024.5.27/parsl/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/test_utils/test_representation_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.346873 parsl-2024.5.27/parsl/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/unit/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.346873 parsl-2024.5.27/parsl/usage_tracking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/usage_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/usage_tracking/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/usage_tracking/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-27 22:42:39.000000 parsl-2024.5.27/parsl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-27 22:42:41.000000 parsl-2024.5.27/parsl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:42:42.282873 parsl-2024.5.27/parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-27 22:42:42.000000 parsl-2024.5.27/parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18686 2024-05-27 22:42:42.000000 parsl-2024.5.27/parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:42:42.000000 parsl-2024.5.27/parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-27 22:42:42.000000 parsl-2024.5.27/parsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-27 22:42:42.000000 parsl-2024.5.27/parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 22:42:42.000000 parsl-2024.5.27/parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-27 22:42:39.000000 parsl-2024.5.27/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:42:42.346873 parsl-2024.5.27/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2897 2024-05-27 22:42:39.000000 parsl-2024.5.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.068936 parsl-2024.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 22:42:31.000000 parsl-2024.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 22:42:31.000000 parsl-2024.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-06 22:42:36.068936 parsl-2024.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-06 22:42:31.000000 parsl-2024.5.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.012937 parsl-2024.5.6/parsl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.012937 parsl-2024.5.6/parsl/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/app/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/app/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/app/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.012937 parsl-2024.5.6/parsl/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/benchmark/perf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.016937 parsl-2024.5.6/parsl/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/channels/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.016937 parsl-2024.5.6/parsl/channels/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/channels/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/channels/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.016937 parsl-2024.5.6/parsl/channels/oauth_ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/channels/oauth_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/channels/oauth_ssh/oauth_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.016937 parsl-2024.5.6/parsl/channels/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/channels/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/channels/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.016937 parsl-2024.5.6/parsl/channels/ssh_il/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/channels/ssh_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/channels/ssh_il/ssh_il.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.016937 parsl-2024.5.6/parsl/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.016937 parsl-2024.5.6/parsl/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/ASPIRE1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/Azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/expanse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/illinoiscluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/osg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/polaris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/stampede2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/toss3_llnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/configs/wqex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/curvezmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.020937 parsl-2024.5.6/parsl/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/data_provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/data_provider/file_noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/data_provider/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/data_provider/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/data_provider/globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/data_provider/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/data_provider/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/data_provider/staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/data_provider/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.020937 parsl-2024.5.6/parsl/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65903 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/dataflow/dflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/dataflow/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/dataflow/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/dataflow/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/dataflow/rundirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/dataflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/dataflow/taskrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.020937 parsl-2024.5.6/parsl/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.020937 parsl-2024.5.6/parsl/executors/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/flux/execute_parsl_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/flux/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/flux/flux_instance_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.024937 parsl-2024.5.6/parsl/executors/high_throughput/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/high_throughput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/high_throughput/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37318 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/high_throughput/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31491 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/high_throughput/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/high_throughput/manager_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/high_throughput/monitoring_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/high_throughput/mpi_prefix_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/high_throughput/mpi_resource_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/high_throughput/probe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41267 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/high_throughput/process_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/high_throughput/zmq_pipes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.024937 parsl-2024.5.6/parsl/executors/radical/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/radical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21024 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/radical/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/radical/rpex_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/radical/rpex_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/radical/rpex_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/status_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.024937 parsl-2024.5.6/parsl/executors/taskvine/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/taskvine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/taskvine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/taskvine/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31806 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/taskvine/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/taskvine/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/taskvine/factory_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25822 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/taskvine/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/taskvine/manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/taskvine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.024937 parsl-2024.5.6/parsl/executors/workqueue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/workqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/workqueue/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/workqueue/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49312 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/workqueue/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5737 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/workqueue/parsl_coprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      735 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/executors/workqueue/parsl_coprocess_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.028937 parsl-2024.5.6/parsl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/jobs/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/jobs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/jobs/job_status_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/jobs/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/jobs/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.028937 parsl-2024.5.6/parsl/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/launchers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/launchers/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.028937 parsl-2024.5.6/parsl/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37021 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.028937 parsl-2024.5.6/parsl/monitoring/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/queries/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/radios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.028937 parsl-2024.5.6/parsl/monitoring/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.028937 parsl-2024.5.6/parsl/monitoring/visualization/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.028937 parsl-2024.5.6/parsl/monitoring/visualization/plots/default/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/plots/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/plots/default/task_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/plots/default/workflow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.028937 parsl-2024.5.6/parsl/monitoring/visualization/static/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14199 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/static/parsl-logo-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/static/parsl-monitor.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.032937 parsl-2024.5.6/parsl/monitoring/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/templates/app.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/templates/dag.html
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/templates/resource_usage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/templates/task.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/templates/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/templates/workflows_summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/monitoring/visualization/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/process_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.032937 parsl-2024.5.6/parsl/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.032937 parsl-2024.5.6/parsl/providers/ad_hoc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/ad_hoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/ad_hoc/ad_hoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.032937 parsl-2024.5.6/parsl/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29009 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/aws/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.032937 parsl-2024.5.6/parsl/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18396 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/azure/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/azure/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/cluster_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.032937 parsl-2024.5.6/parsl/providers/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/cobalt/cobalt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/cobalt/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.032937 parsl-2024.5.6/parsl/providers/condor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/condor/condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/condor/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.032937 parsl-2024.5.6/parsl/providers/googlecloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/googlecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/googlecloud/googlecloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.032937 parsl-2024.5.6/parsl/providers/grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/grid_engine/grid_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/grid_engine/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.036937 parsl-2024.5.6/parsl/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/kubernetes/kube.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/kubernetes/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.036937 parsl-2024.5.6/parsl/providers/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.036937 parsl-2024.5.6/parsl/providers/lsf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/lsf/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/lsf/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.036937 parsl-2024.5.6/parsl/providers/pbspro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/pbspro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/pbspro/pbspro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/pbspro/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.036937 parsl-2024.5.6/parsl/providers/slurm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/slurm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.036937 parsl-2024.5.6/parsl/providers/torque/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/torque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/torque/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/providers/torque/torque.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.036937 parsl-2024.5.6/parsl/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/serialize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/serialize/concretes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/serialize/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/serialize/facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/serialize/proxystore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.040937 parsl-2024.5.6/parsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/callables_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.044937 parsl-2024.5.6/parsl/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/ad_hoc_cluster_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/azure_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/cooley_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/ec2_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/ec2_spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/htex_ad_hoc_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/htex_local_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/htex_local_intask_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/htex_local_rsync_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_radical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_radical_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_threads_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_threads_checkpoint_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_threads_checkpoint_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_threads_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_threads_globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_threads_http_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_threads_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/local_threads_no_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/nscc_singapore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/osg_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/petrelkube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/swan_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/taskvine_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/user_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/configs/workqueue_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.044937 parsl-2024.5.6/parsl/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/latency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.044937 parsl-2024.5.6/parsl/tests/integration/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.044937 parsl-2024.5.6/parsl/tests/integration/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_channels/test_local_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_channels/test_scp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_channels/test_ssh_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_channels/test_ssh_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_channels/test_ssh_file_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_channels/test_ssh_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_parsl_load_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.044937 parsl-2024.5.6/parsl/tests/integration/test_stress/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_stress/test_python_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/integration/test_stress/test_python_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.048936 parsl-2024.5.6/parsl/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/manual_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/manual_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/manual_tests/test_ad_hoc_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/manual_tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/manual_tests/test_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/manual_tests/test_memory_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/manual_tests/test_oauth_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/manual_tests/test_regression_220.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/manual_tests/test_udp_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/manual_tests/test_worker_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.048936 parsl-2024.5.6/parsl/tests/scaling_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/scaling_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/scaling_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/scaling_tests/local_threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3751 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/scaling_tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/scaling_tests/vineex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/scaling_tests/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/scaling_tests/wqex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/scaling_tests/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.048936 parsl-2024.5.6/parsl/tests/site_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/site_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/site_tests/site_config_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/site_tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/site_tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.048936 parsl-2024.5.6/parsl/tests/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/sites/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/sites/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/sites/test_dynamic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/sites/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/sites/test_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/sites/test_local_adhoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.048936 parsl-2024.5.6/parsl/tests/sites/test_mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/sites/test_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/sites/test_worker_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_aalst_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.052936 parsl-2024.5.6/parsl/tests/test_bash_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/test_apptimeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/test_keyword_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/test_kwarg_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/test_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/test_std_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_bash_apps/test_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_callables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.052936 parsl-2024.5.6/parsl/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_channels/test_large_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.052936 parsl-2024.5.6/parsl/tests/test_checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_checkpointing/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_checkpointing/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_checkpointing/test_regression_233.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_checkpointing/test_regression_239.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_checkpointing/test_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_curvezmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.052936 parsl-2024.5.6/parsl/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_docs/test_from_slides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_docs/test_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_docs/test_tutorial_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_docs/test_workflow1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_docs/test_workflow2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_docs/test_workflow4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.052936 parsl-2024.5.6/parsl/tests/test_error_handling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_error_handling/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_error_handling/test_python_walltime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_error_handling/test_rand_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_error_handling/test_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_error_handling/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_error_handling/test_retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_error_handling/test_retry_handler_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_error_handling/test_serialization_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_error_handling/test_wrap_with_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.052936 parsl-2024.5.6/parsl/tests/test_flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.056936 parsl-2024.5.6/parsl/tests/test_htex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_htex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_htex/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_htex/test_connected_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_htex/test_cpu_affinity_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_htex/test_disconnected_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_htex/test_drain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_htex/test_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_htex/test_manager_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_htex/test_missing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_htex/test_multiple_disconnected_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_htex/test_worker_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_htex/test_zmq_binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.056936 parsl-2024.5.6/parsl/tests/test_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_monitoring/test_app_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_monitoring/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_monitoring/test_db_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_monitoring/test_fuzz_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_monitoring/test_incomplete_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_monitoring/test_memoization_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_monitoring/test_stdouterr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_monitoring/test_viz_colouring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.056936 parsl-2024.5.6/parsl/tests/test_mpi_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_mpi_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_mpi_apps/test_bad_mpi_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_mpi_apps/test_mpi_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_mpi_apps/test_mpi_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_mpi_apps/test_resource_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.060937 parsl-2024.5.6/parsl/tests/test_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_providers/test_cobalt_deprecation_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_providers/test_local_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_providers/test_pbspro_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_providers/test_slurm_instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_providers/test_slurm_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_providers/test_submiterror_deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.060937 parsl-2024.5.6/parsl/tests/test_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_arg_input_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_dep_standard_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_depfail_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_fibonacci_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_fibonacci_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_import_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_lifted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_mapred.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_memoize_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_memoize_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_memoize_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_memoize_joinapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_python_apps/test_type5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.060937 parsl-2024.5.6/parsl/tests/test_radical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_radical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_radical/test_mpi_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.064936 parsl-2024.5.6/parsl/tests/test_regression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_regression/test_1480.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_regression/test_1653.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_regression/test_221.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_regression/test_226.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_regression/test_2652.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_regression/test_69a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_regression/test_854.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_regression/test_97_parallelism_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_regression/test_98.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.064936 parsl-2024.5.6/parsl/tests/test_scaling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_scaling/test_block_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_scaling/test_regression_1621.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_scaling/test_scale_down.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_scaling/test_scale_down_htex_unregistered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_scaling/test_shutdown_scalein.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.064936 parsl-2024.5.6/parsl/tests/test_serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_serialization/test_2555_caching_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_serialization/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_serialization/test_htex_code_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_serialization/test_pack_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_serialization/test_proxystore_configured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_serialization/test_proxystore_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.064936 parsl-2024.5.6/parsl/tests/test_shutdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_shutdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_shutdown/test_kill_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.068936 parsl-2024.5.6/parsl/tests/test_staging/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/staging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_1316.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_docs_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_docs_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_elaborate_noop_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_file_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_file_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_output_chain_filenames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_staging_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_staging_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_staging_globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_staging_https.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_staging_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_zip_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_zip_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_staging/test_zip_to_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_thread_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.068936 parsl-2024.5.6/parsl/tests/test_threads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_threads/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_threads/test_lazy_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.068936 parsl-2024.5.6/parsl/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/test_utils/test_representation_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.068936 parsl-2024.5.6/parsl/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/unit/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.068936 parsl-2024.5.6/parsl/usage_tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/usage_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/usage_tracking/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/usage_tracking/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-06 22:42:31.000000 parsl-2024.5.6/parsl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-06 22:42:33.000000 parsl-2024.5.6/parsl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:42:36.012937 parsl-2024.5.6/parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-06 22:42:35.000000 parsl-2024.5.6/parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18394 2024-05-06 22:42:35.000000 parsl-2024.5.6/parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:42:35.000000 parsl-2024.5.6/parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-06 22:42:35.000000 parsl-2024.5.6/parsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-06 22:42:35.000000 parsl-2024.5.6/parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 22:42:35.000000 parsl-2024.5.6/parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 22:42:31.000000 parsl-2024.5.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 22:42:36.068936 parsl-2024.5.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-05-06 22:42:31.000000 parsl-2024.5.6/setup.py
```

### Comparing `parsl-2024.5.27/LICENSE` & `parsl-2024.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/PKG-INFO` & `parsl-2024.5.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2024.5.27
+Version: 2024.5.6
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2024.05.27.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2024.05.06.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2024.5.27/README.rst` & `parsl-2024.5.6/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -18,27 +18,25 @@
 
     # Make functions parallel by decorating them
     @python_app
     def f(x):
         return x + 1
 
     @python_app
-    def g(x, y):
-        return x + y
+    def g(x):
+        return x * 2
 
     # Start Parsl on a single computer
     with parsl.load():
-        # These functions now return Futures
+        # These functions now return Futures, and can be chained
         future = f(1)
         assert future.result() == 2
 
-        # Functions run concurrently, can be chained
-        f_a, f_b = f(2), f(3)
-        future = g(f_a, f_b)
-        assert future.result() == 7
+        future = g(f(1))
+        assert future.result() == 4
 
 
 Start with the `configuration quickstart <https://parsl.readthedocs.io/en/stable/quickstart.html#getting-started>`_ to learn how to tell Parsl how to use your computing resource,
 then explore the `parallel computing patterns <https://parsl.readthedocs.io/en/stable/userguide/workflow.html>`_ to determine how to use parallelism best in your application.
 
 .. |licence| image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
    :target: https://github.com/Parsl/parsl/blob/master/LICENSE
@@ -118,13 +116,13 @@
 ============
 
 Parsl is supported in Python 3.8+. Requirements can be found `here <requirements.txt>`_. Requirements for running tests can be found `here <test-requirements.txt>`_.
 
 Code of Conduct
 ===============
 
-Parsl seeks to foster an open and welcoming environment - Please see the `Parsl Code of Conduct <https://github.com/Parsl/parsl?tab=coc-ov-file#parsl-code-of-conduct>`_ for more details.
+Parsl seeks to foster an open and welcoming environment - Please see the `Parsl Code of Conduct <https://github.com/Parsl/parsl/blob/master/CODE_OF_CONDUCT.md>`_ for more details.
 
 Contributing
 ============
 
 We welcome contributions from the community. Please see our `contributing guide <https://github.com/Parsl/parsl/blob/master/CONTRIBUTING.rst>`_.
```

### Comparing `parsl-2024.5.27/parsl/__init__.py` & `parsl-2024.5.6/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/addresses.py` & `parsl-2024.5.6/parsl/addresses.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/app/app.py` & `parsl-2024.5.6/parsl/app/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/app/bash.py` & `parsl-2024.5.6/parsl/app/bash.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/app/errors.py` & `parsl-2024.5.6/parsl/app/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/app/futures.py` & `parsl-2024.5.6/parsl/app/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/app/python.py` & `parsl-2024.5.6/parsl/app/python.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/benchmark/perf.py` & `parsl-2024.5.6/parsl/benchmark/perf.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/channels/base.py` & `parsl-2024.5.6/parsl/channels/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,23 @@
 
         Returns:
             destination_path (string)
         '''
         pass
 
     @abstractmethod
-    def close(self) -> None:
-        ''' Closes the channel.
+    def close(self) -> bool:
+        ''' Closes the channel. Clean out any auth credentials.
+
+        Args:
+            None
+
+        Returns:
+            Bool
+
         '''
         pass
 
     @abstractmethod
     def makedirs(self, path: str, mode: int = 0o511, exist_ok: bool = False) -> None:
         """Create a directory.
```

### Comparing `parsl-2024.5.27/parsl/channels/errors.py` & `parsl-2024.5.6/parsl/channels/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/channels/local/local.py` & `parsl-2024.5.6/parsl/channels/local/local.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,18 +103,21 @@
             os.chmod(local_dest, 0o700)
 
         return local_dest
 
     def pull_file(self, remote_source, local_dir):
         return self.push_file(remote_source, local_dir)
 
-    def close(self) -> None:
-        ''' There's nothing to close here, and so this doesn't do anything
+    def close(self):
+        ''' There's nothing to close here, and this really doesn't do anything
+
+        Returns:
+             - False, because it really did not "close" this channel.
         '''
-        pass
+        return False
 
     def isdir(self, path):
         """Return true if the path refers to an existing directory.
 
         Parameters
         ----------
         path : str
```

### Comparing `parsl-2024.5.27/parsl/channels/oauth_ssh/oauth_ssh.py` & `parsl-2024.5.6/parsl/channels/oauth_ssh/oauth_ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,9 +102,9 @@
 
         except socket.timeout:
             logger.exception("Command failed to execute without timeout limit on {}".format(self))
             raise
 
         return exit_status, stdout, stderr
 
-    def close(self) -> None:
-        self.transport.close()
+    def close(self):
+        return self.transport.close()
```

### Comparing `parsl-2024.5.27/parsl/channels/ssh/ssh.py` & `parsl-2024.5.6/parsl/channels/ssh/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,17 +213,17 @@
             self._valid_sftp_client().get(remote_source, local_dest)
         except Exception as e:
             logger.exception("File pull failed")
             raise FileCopyException(e, self.hostname)
 
         return local_dest
 
-    def close(self) -> None:
+    def close(self):
         if self._is_connected():
-            self.ssh_client.close()
+            return self.ssh_client.close()
 
     def isdir(self, path):
         """Return true if the path refers to an existing directory.
 
         Parameters
         ----------
         path : str
```

### Comparing `parsl-2024.5.27/parsl/channels/ssh_il/ssh_il.py` & `parsl-2024.5.6/parsl/channels/ssh_il/ssh_il.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/concurrent/__init__.py` & `parsl-2024.5.6/parsl/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/config.py` & `parsl-2024.5.6/parsl/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import typeguard
 
 from typing import Callable, Iterable, Optional, Sequence, Union
 from typing_extensions import Literal
 
 from parsl.utils import RepresentationMixin
-from parsl.dataflow.dependency_resolvers import DependencyResolver
 from parsl.executors.base import ParslExecutor
 from parsl.executors.threads import ThreadPoolExecutor
 from parsl.errors import ConfigurationError
 from parsl.dataflow.taskrecord import TaskRecord
 from parsl.monitoring import MonitoringHub
 from parsl.usage_tracking.api import UsageInformation
 
@@ -32,16 +31,14 @@
         :func:`parsl.utils.get_last_checkpoint` for helpers. Default is None.
     checkpoint_mode : str, optional
         Checkpoint mode to use, can be ``'dfk_exit'``, ``'task_exit'``, ``'periodic'`` or ``'manual'``.
         If set to `None`, checkpointing will be disabled. Default is None.
     checkpoint_period : str, optional
         Time interval (in "HH:MM:SS") at which to checkpoint completed tasks. Only has an effect if
         ``checkpoint_mode='periodic'``.
-    dependency_resolver: plugin point for custom dependency resolvers. Default: only resolve Futures,
-        using the `SHALLOW_DEPENDENCY_RESOLVER`.
     garbage_collect : bool. optional.
         Delete task records from DFK when tasks have completed. Default: True
     internal_tasks_max_threads : int, optional
         Maximum number of threads to allocate for submit side internal tasks such as some data transfers
         or @joinapps
         Default is 10.
     monitoring : MonitoringHub, optional
@@ -87,15 +84,14 @@
                  checkpoint_files: Optional[Sequence[str]] = None,
                  checkpoint_mode: Union[None,
                                         Literal['task_exit'],
                                         Literal['periodic'],
                                         Literal['dfk_exit'],
                                         Literal['manual']] = None,
                  checkpoint_period: Optional[str] = None,
-                 dependency_resolver: Optional[DependencyResolver] = None,
                  garbage_collect: bool = True,
                  internal_tasks_max_threads: int = 10,
                  retries: int = 0,
                  retry_handler: Optional[Callable[[Exception, TaskRecord], float]] = None,
                  run_dir: str = 'runinfo',
                  std_autopath: Optional[Callable] = None,
                  strategy: Optional[str] = 'simple',
@@ -123,15 +119,14 @@
             elif checkpoint_mode != 'periodic':
                 logger.debug("Requested checkpoint period of {} only has an effect with checkpoint_mode='periodic'".format(
                     checkpoint_period)
                 )
         if checkpoint_mode == 'periodic' and checkpoint_period is None:
             checkpoint_period = "00:30:00"
         self.checkpoint_period = checkpoint_period
-        self.dependency_resolver = dependency_resolver
         self.garbage_collect = garbage_collect
         self.internal_tasks_max_threads = internal_tasks_max_threads
         self.retries = retries
         self.retry_handler = retry_handler
         self.run_dir = run_dir
         self.strategy = strategy
         self.strategy_period = strategy_period
@@ -153,9 +148,8 @@
         labels = [e.label for e in self.executors]
         duplicates = [e for n, e in enumerate(labels) if e in labels[:n]]
         if len(duplicates) > 0:
             raise ConfigurationError('Executors must have unique labels ({})'.format(
                 ', '.join(['label={}'.format(repr(d)) for d in duplicates])))
 
     def get_usage_information(self):
-        return {"executors_len": len(self.executors),
-                "dependency_resolver": self.dependency_resolver is not None}
+        return {"executors_len": len(self.executors)}
```

### Comparing `parsl-2024.5.27/parsl/configs/ASPIRE1.py` & `parsl-2024.5.6/parsl/configs/ASPIRE1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/Azure.py` & `parsl-2024.5.6/parsl/configs/Azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/ad_hoc.py` & `parsl-2024.5.6/parsl/configs/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/bridges.py` & `parsl-2024.5.6/parsl/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/cc_in2p3.py` & `parsl-2024.5.6/parsl/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/ec2.py` & `parsl-2024.5.6/parsl/configs/ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/expanse.py` & `parsl-2024.5.6/parsl/configs/expanse.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/frontera.py` & `parsl-2024.5.6/parsl/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/illinoiscluster.py` & `parsl-2024.5.6/parsl/configs/illinoiscluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/kubernetes.py` & `parsl-2024.5.6/parsl/configs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/midway.py` & `parsl-2024.5.6/parsl/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/osg.py` & `parsl-2024.5.6/parsl/configs/osg.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/polaris.py` & `parsl-2024.5.6/parsl/configs/polaris.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/stampede2.py` & `parsl-2024.5.6/parsl/configs/stampede2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/summit.py` & `parsl-2024.5.6/parsl/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/toss3_llnl.py` & `parsl-2024.5.6/parsl/configs/toss3_llnl.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/vineex_local.py` & `parsl-2024.5.6/parsl/configs/vineex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/configs/wqex_local.py` & `parsl-2024.5.6/parsl/configs/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/curvezmq.py` & `parsl-2024.5.6/parsl/curvezmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/data_provider/data_manager.py` & `parsl-2024.5.6/parsl/data_provider/data_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/data_provider/files.py` & `parsl-2024.5.6/parsl/data_provider/files.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/data_provider/ftp.py` & `parsl-2024.5.6/parsl/data_provider/ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/data_provider/globus.py` & `parsl-2024.5.6/parsl/data_provider/globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/data_provider/http.py` & `parsl-2024.5.6/parsl/data_provider/http.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/data_provider/rsync.py` & `parsl-2024.5.6/parsl/data_provider/rsync.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/data_provider/staging.py` & `parsl-2024.5.6/parsl/data_provider/staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/data_provider/zip.py` & `parsl-2024.5.6/parsl/data_provider/zip.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/dataflow/dflow.py` & `parsl-2024.5.6/parsl/dataflow/dflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import parsl
 from parsl.app.errors import RemoteExceptionWrapper
 from parsl.app.futures import DataFuture
 from parsl.channels import Channel
 from parsl.config import Config
 from parsl.data_provider.data_manager import DataManager
 from parsl.data_provider.files import File
-from parsl.dataflow.dependency_resolvers import SHALLOW_DEPENDENCY_RESOLVER
 from parsl.dataflow.errors import BadCheckpoint, DependencyError, JoinError
 from parsl.dataflow.futures import AppFuture
 from parsl.dataflow.memoization import Memoizer
 from parsl.dataflow.rundirs import make_rundir
 from parsl.dataflow.states import States, FINAL_STATES, FINAL_FAILURE_STATES
 from parsl.dataflow.taskrecord import TaskRecord
 from parsl.errors import ConfigurationError, InternalConsistencyError, NoDataFlowKernelError
@@ -200,17 +199,14 @@
                 checkpoint_period = (h * 3600) + (m * 60) + s
                 self._checkpoint_timer = Timer(self.checkpoint, interval=checkpoint_period, name="Checkpoint")
 
         self.task_count = 0
         self.tasks: Dict[int, TaskRecord] = {}
         self.submitter_lock = threading.Lock()
 
-        self.dependency_resolver = self.config.dependency_resolver if self.config.dependency_resolver is not None \
-            else SHALLOW_DEPENDENCY_RESOLVER
-
         atexit.register(self.atexit_cleanup)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         logger.debug("Exiting the context manager, calling cleanup for DFK")
@@ -852,19 +848,16 @@
         Returns:
             - list of dependencies
 
         """
         depends: List[Future] = []
 
         def check_dep(d: Any) -> None:
-            try:
-                depends.extend(self.dependency_resolver.traverse_to_gather(d))
-            except Exception:
-                logger.exception("Exception in dependency_resolver.traverse_to_gather")
-                raise
+            if isinstance(d, Future):
+                depends.extend([d])
 
         # Check the positional args
         for dep in args:
             check_dep(dep)
 
         # Check for explicit kwargs ex, fu_1=<fut>
         for key in kwargs:
@@ -873,16 +866,15 @@
 
         # Check for futures in inputs=[<fut>...]
         for dep in kwargs.get('inputs', []):
             check_dep(dep)
 
         return depends
 
-    def _unwrap_futures(self, args: Sequence[Any], kwargs: Dict[str, Any]) \
-            -> Tuple[Sequence[Any], Dict[str, Any], Sequence[Tuple[Exception, str]]]:
+    def _unwrap_futures(self, args, kwargs):
         """This function should be called when all dependencies have completed.
 
         It will rewrite the arguments for that task, replacing each Future
         with the result of that future.
 
         If the user hid futures a level below, we will not catch
         it, and will (most likely) result in a type error.
@@ -895,48 +887,61 @@
             a rewritten args list
             a rewritten kwargs dict
             pairs of exceptions, task ids from any Futures which stored
             exceptions rather than results.
         """
         dep_failures = []
 
-        def append_failure(e: Exception, dep: Future) -> None:
-            # If this Future is associated with a task inside this DFK,
-            # then refer to the task ID.
-            # Otherwise make a repr of the Future object.
-            if hasattr(dep, 'task_record') and dep.task_record['dfk'] == self:
-                tid = "task " + repr(dep.task_record['id'])
-            else:
-                tid = repr(dep)
-            dep_failures.extend([(e, tid)])
-
         # Replace item in args
         new_args = []
         for dep in args:
-            try:
-                new_args.extend([self.dependency_resolver.traverse_to_unwrap(dep)])
-            except Exception as e:
-                append_failure(e, dep)
+            if isinstance(dep, Future):
+                try:
+                    new_args.extend([dep.result()])
+                except Exception as e:
+                    # If this Future is associated with a task inside this DFK,
+                    # then refer to the task ID.
+                    # Otherwise make a repr of the Future object.
+                    if hasattr(dep, 'task_record') and dep.task_record['dfk'] == self:
+                        tid = "task " + repr(dep.task_record['id'])
+                    else:
+                        tid = repr(dep)
+                    dep_failures.extend([(e, tid)])
+            else:
+                new_args.extend([dep])
 
         # Check for explicit kwargs ex, fu_1=<fut>
         for key in kwargs:
             dep = kwargs[key]
-            try:
-                kwargs[key] = self.dependency_resolver.traverse_to_unwrap(dep)
-            except Exception as e:
-                append_failure(e, dep)
+            if isinstance(dep, Future):
+                try:
+                    kwargs[key] = dep.result()
+                except Exception as e:
+                    if hasattr(dep, 'task_record'):
+                        tid = dep.task_record['id']
+                    else:
+                        tid = None
+                    dep_failures.extend([(e, tid)])
 
         # Check for futures in inputs=[<fut>...]
         if 'inputs' in kwargs:
             new_inputs = []
             for dep in kwargs['inputs']:
-                try:
-                    new_inputs.extend([self.dependency_resolver.traverse_to_unwrap(dep)])
-                except Exception as e:
-                    append_failure(e, dep)
+                if isinstance(dep, Future):
+                    try:
+                        new_inputs.extend([dep.result()])
+                    except Exception as e:
+                        if hasattr(dep, 'task_record'):
+                            tid = dep.task_record['id']
+                        else:
+                            tid = None
+                        dep_failures.extend([(e, tid)])
+
+                else:
+                    new_inputs.extend([dep])
             kwargs['inputs'] = new_inputs
 
         return new_args, kwargs, dep_failures
 
     def submit(self,
                func: Callable,
                app_args: Sequence[Any],
@@ -1033,31 +1038,27 @@
         task_record['app_fu'] = app_fu
 
         # Transform remote input files to data futures
         app_args, app_kwargs, func = self._add_input_deps(executor, app_args, app_kwargs, func)
 
         func = self._add_output_deps(executor, app_args, app_kwargs, app_fu, func)
 
-        logger.debug("Added output dependencies")
-
         # Replace the function invocation in the TaskRecord with whatever file-staging
         # substitutions have been made.
         task_record.update({
                     'args': app_args,
                     'func': func,
                     'kwargs': app_kwargs})
 
         assert task_id not in self.tasks
 
         self.tasks[task_id] = task_record
 
-        logger.debug("Gathering dependencies")
         # Get the list of dependencies for the task
         depends = self._gather_all_deps(app_args, app_kwargs)
-        logger.debug("Gathered dependencies")
         task_record['depends'] = depends
 
         depend_descs = []
         for d in depends:
             if isinstance(d, AppFuture) or isinstance(d, DataFuture):
                 depend_descs.append("task {}".format(d.tid))
             else:
@@ -1151,15 +1152,15 @@
         channel.makedirs(channel.script_dir, exist_ok=True)
 
     def add_executors(self, executors: Sequence[ParslExecutor]) -> None:
         for executor in executors:
             executor.run_id = self.run_id
             executor.run_dir = self.run_dir
             executor.hub_address = self.hub_address
-            executor.hub_zmq_port = self.hub_zmq_port
+            executor.hub_port = self.hub_zmq_port
             if self.monitoring:
                 executor.monitoring_radio = self.monitoring.radio
             if hasattr(executor, 'provider'):
                 if hasattr(executor.provider, 'script_dir'):
                     executor.provider.script_dir = os.path.join(self.run_dir, 'submit_scripts')
                     os.makedirs(executor.provider.script_dir, exist_ok=True)
 
@@ -1172,17 +1173,20 @@
 
             self.executors[executor.label] = executor
             executor.start()
         block_executors = [e for e in executors if isinstance(e, BlockProviderExecutor)]
         self.job_status_poller.add_executors(block_executors)
 
     def atexit_cleanup(self) -> None:
-        logger.warning("Python is exiting with a DFK still running. "
-                       "You should call parsl.dfk().cleanup() before "
-                       "exiting to release any resources")
+        if not self.cleanup_called:
+            logger.warning("Python is exiting with a DFK still running. "
+                           "You should call parsl.dfk().cleanup() before "
+                           "exiting to release any resources")
+        else:
+            logger.info("python process is exiting, but DFK has already been cleaned up")
 
     def wait_for_current_tasks(self) -> None:
         """Waits for all tasks in the task list to be completed, by waiting for their
         AppFuture to be completed. This method will not necessarily wait for any tasks
         added after cleanup has started (such as data stageout?)
         """
 
@@ -1262,25 +1266,14 @@
                                   'time_completed': self.time_completed,
                                   'run_id': self.run_id, 'rundir': self.run_dir})
 
             logger.info("Terminating monitoring")
             self.monitoring.close()
             logger.info("Terminated monitoring")
 
-        logger.info("Unregistering atexit hook")
-        atexit.unregister(self.atexit_cleanup)
-        logger.info("Unregistered atexit hook")
-
-        if DataFlowKernelLoader._dfk is self:
-            logger.info("Unregistering default DFK")
-            parsl.clear()
-            logger.info("Unregistered default DFK")
-        else:
-            logger.debug("Cleaning up non-default DFK - not unregistering")
-
         logger.info("DFK cleanup complete")
 
     def checkpoint(self, tasks: Optional[Sequence[TaskRecord]] = None) -> str:
         """Checkpoint the dfk incrementally to a checkpoint file.
 
         When called, every task that has been completed yet not
         checkpointed is checkpointed to a file.
```

### Comparing `parsl-2024.5.27/parsl/dataflow/errors.py` & `parsl-2024.5.6/parsl/dataflow/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/dataflow/futures.py` & `parsl-2024.5.6/parsl/dataflow/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/dataflow/memoization.py` & `parsl-2024.5.6/parsl/dataflow/memoization.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/dataflow/rundirs.py` & `parsl-2024.5.6/parsl/dataflow/rundirs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/dataflow/states.py` & `parsl-2024.5.6/parsl/dataflow/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/dataflow/taskrecord.py` & `parsl-2024.5.6/parsl/dataflow/taskrecord.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/errors.py` & `parsl-2024.5.6/parsl/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/base.py` & `parsl-2024.5.6/parsl/executors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,21 +46,21 @@
     label: str = "undefined"
     radio_mode: str = "udp"
 
     def __init__(
         self,
         *,
         hub_address: Optional[str] = None,
-        hub_zmq_port: Optional[int] = None,
+        hub_port: Optional[int] = None,
         monitoring_radio: Optional[MonitoringRadio] = None,
         run_dir: str = ".",
         run_id: Optional[str] = None,
     ):
         self.hub_address = hub_address
-        self.hub_zmq_port = hub_zmq_port
+        self.hub_port = hub_port
         self.monitoring_radio = monitoring_radio
         self.run_dir = os.path.abspath(run_dir)
         self.run_id = run_id
 
     def __enter__(self) -> Self:
         return self
 
@@ -132,22 +132,22 @@
         return self._hub_address
 
     @hub_address.setter
     def hub_address(self, value: Optional[str]) -> None:
         self._hub_address = value
 
     @property
-    def hub_zmq_port(self) -> Optional[int]:
+    def hub_port(self) -> Optional[int]:
         """Port to the Hub for monitoring.
         """
-        return self._hub_zmq_port
+        return self._hub_port
 
-    @hub_zmq_port.setter
-    def hub_zmq_port(self, value: Optional[int]) -> None:
-        self._hub_zmq_port = value
+    @hub_port.setter
+    def hub_port(self, value: Optional[int]) -> None:
+        self._hub_port = value
 
     @property
     def monitoring_radio(self) -> Optional[MonitoringRadio]:
         """Local radio for sending monitoring messages
         """
         return self._monitoring_radio
```

### Comparing `parsl-2024.5.27/parsl/executors/errors.py` & `parsl-2024.5.6/parsl/executors/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/flux/execute_parsl_task.py` & `parsl-2024.5.6/parsl/executors/flux/execute_parsl_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/flux/executor.py` & `parsl-2024.5.6/parsl/executors/flux/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/flux/flux_instance_manager.py` & `parsl-2024.5.6/parsl/executors/flux/flux_instance_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/high_throughput/executor.py` & `parsl-2024.5.6/parsl/executors/high_throughput/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,55 @@
                       "--hb_threshold={heartbeat_threshold} "
                       "--drain_period={drain_period} "
                       "--cpu-affinity {cpu_affinity} "
                       "{enable_mpi_mode} "
                       "--mpi-launcher={mpi_launcher} "
                       "--available-accelerators {accelerators}")
 
-GENERAL_HTEX_PARAM_DOCS = """provider : :class:`~parsl.providers.base.ExecutionProvider`
+
+class HighThroughputExecutor(BlockProviderExecutor, RepresentationMixin, UsageInformation):
+    """Executor designed for cluster-scale
+
+    The HighThroughputExecutor system has the following components:
+      1. The HighThroughputExecutor instance which is run as part of the Parsl script.
+      2. The Interchange which acts as a load-balancing proxy between workers and Parsl
+      3. The multiprocessing based worker pool which coordinates task execution over several
+         cores on a node.
+      4. ZeroMQ pipes connect the HighThroughputExecutor, Interchange and the process_worker_pool
+
+    Here is a diagram
+
+    .. code:: python
+
+
+                        |  Data   |  Executor   |  Interchange  | External Process(es)
+                        |  Flow   |             |               |
+                   Task | Kernel  |             |               |
+                 +----->|-------->|------------>|->outgoing_q---|-> process_worker_pool
+                 |      |         |             | batching      |    |         |
+           Parsl<---Fut-|         |             | load-balancing|  result   exception
+                     ^  |         |             | watchdogs     |    |         |
+                     |  |         |   Q_mngmnt  |               |    V         V
+                     |  |         |    Thread<--|-incoming_q<---|--- +---------+
+                     |  |         |      |      |               |
+                     |  |         |      |      |               |
+                     +----update_fut-----+
+
+
+    Each of the workers in each process_worker_pool has access to its local rank through
+    an environmental variable, ``PARSL_WORKER_RANK``. The local rank is unique for each process
+    and is an integer in the range from 0 to the number of workers per in the pool minus 1.
+    The workers also have access to the ID of the worker pool as ``PARSL_WORKER_POOL_ID``
+    and the size of the worker pool as ``PARSL_WORKER_COUNT``.
+
+
+    Parameters
+    ----------
+
+    provider : :class:`~parsl.providers.base.ExecutionProvider`
        Provider to access computation resources. Can be one of :class:`~parsl.providers.aws.aws.EC2Provider`,
         :class:`~parsl.providers.cobalt.cobalt.Cobalt`,
         :class:`~parsl.providers.condor.condor.Condor`,
         :class:`~parsl.providers.googlecloud.googlecloud.GoogleCloud`,
         :class:`~parsl.providers.gridEngine.gridEngine.GridEngine`,
         :class:`~parsl.providers.local.local.Local`,
         :class:`~parsl.providers.sge.sge.GridEngine`,
@@ -104,93 +144,14 @@
 
     working_dir : str
         Working dir to be used by the executor.
 
     worker_debug : Bool
         Enables worker debug logging.
 
-    prefetch_capacity : int
-        Number of tasks that could be prefetched over available worker capacity.
-        When there are a few tasks (<100) or when tasks are long running, this option should
-        be set to 0 for better load balancing. Default is 0.
-
-    address_probe_timeout : int | None
-        Managers attempt connecting over many different addresses to determine a viable address.
-        This option sets a time limit in seconds on the connection attempt.
-        Default of None implies 30s timeout set on worker.
-
-    heartbeat_threshold : int
-        Seconds since the last message from the counterpart in the communication pair:
-        (interchange, manager) after which the counterpart is assumed to be un-available. Default: 120s
-
-    heartbeat_period : int
-        Number of seconds after which a heartbeat message indicating liveness is sent to the
-        counterpart (interchange, manager). Default: 30s
-
-    poll_period : int
-        Timeout period to be used by the executor components in milliseconds. Increasing poll_periods
-        trades performance for cpu efficiency. Default: 10ms
-
-    drain_period : int
-        The number of seconds after start when workers will begin to drain
-        and then exit. Set this to a time that is slightly less than the
-        maximum walltime of batch jobs to avoid killing tasks while they
-        execute. For example, you could set this to the walltime minus a grace
-        period for the batch job to start the workers, minus the expected
-        maximum length of an individual task.
-
-    worker_logdir_root : string
-        In case of a remote file system, specify the path to where logs will be kept.
-
-    encrypted : bool
-        Flag to enable/disable encryption (CurveZMQ). Default is False.
-"""  # Documentation for params used by both HTEx and MPIEx
-
-
-class HighThroughputExecutor(BlockProviderExecutor, RepresentationMixin, UsageInformation):
-    __doc__ = f"""Executor designed for cluster-scale
-
-    The HighThroughputExecutor system has the following components:
-      1. The HighThroughputExecutor instance which is run as part of the Parsl script.
-      2. The Interchange which acts as a load-balancing proxy between workers and Parsl
-      3. The multiprocessing based worker pool which coordinates task execution over several
-         cores on a node.
-      4. ZeroMQ pipes connect the HighThroughputExecutor, Interchange and the process_worker_pool
-
-    Here is a diagram
-
-    .. code:: python
-
-
-                        |  Data   |  Executor   |  Interchange  | External Process(es)
-                        |  Flow   |             |               |
-                   Task | Kernel  |             |               |
-                 +----->|-------->|------------>|->outgoing_q---|-> process_worker_pool
-                 |      |         |             | batching      |    |         |
-           Parsl<---Fut-|         |             | load-balancing|  result   exception
-                     ^  |         |             | watchdogs     |    |         |
-                     |  |         |   Q_mngmnt  |               |    V         V
-                     |  |         |    Thread<--|-incoming_q<---|--- +---------+
-                     |  |         |      |      |               |
-                     |  |         |      |      |               |
-                     +----update_fut-----+
-
-
-    Each of the workers in each process_worker_pool has access to its local rank through
-    an environmental variable, ``PARSL_WORKER_RANK``. The local rank is unique for each process
-    and is an integer in the range from 0 to the number of workers per in the pool minus 1.
-    The workers also have access to the ID of the worker pool as ``PARSL_WORKER_POOL_ID``
-    and the size of the worker pool as ``PARSL_WORKER_COUNT``.
-
-
-    Parameters
-    ----------
-
-    {GENERAL_HTEX_PARAM_DOCS}
-
     cores_per_worker : float
         cores to be assigned to each worker. Oversubscription is possible
         by setting cores_per_worker < 1.0. Default=1
 
     mem_per_worker : float
         GB of memory required per worker. If this option is specified, the node manager
         will check the available memory at startup and limit the number of workers such that
@@ -216,24 +177,60 @@
         accelerators, and no more workers will be launched than the number of accelerators.
 
         Either provide the list of accelerator names or the number available. If a number is provided,
         Parsl will create names as integers starting with 0.
 
         default: empty list
 
+    prefetch_capacity : int
+        Number of tasks that could be prefetched over available worker capacity.
+        When there are a few tasks (<100) or when tasks are long running, this option should
+        be set to 0 for better load balancing. Default is 0.
+
+    address_probe_timeout : int | None
+        Managers attempt connecting over many different addresses to determine a viable address.
+        This option sets a time limit in seconds on the connection attempt.
+        Default of None implies 30s timeout set on worker.
+
+    heartbeat_threshold : int
+        Seconds since the last message from the counterpart in the communication pair:
+        (interchange, manager) after which the counterpart is assumed to be un-available. Default: 120s
+
+    heartbeat_period : int
+        Number of seconds after which a heartbeat message indicating liveness is sent to the
+        counterpart (interchange, manager). Default: 30s
+
+    poll_period : int
+        Timeout period to be used by the executor components in milliseconds. Increasing poll_periods
+        trades performance for cpu efficiency. Default: 10ms
+
+    drain_period : int
+        The number of seconds after start when workers will begin to drain
+        and then exit. Set this to a time that is slightly less than the
+        maximum walltime of batch jobs to avoid killing tasks while they
+        execute. For example, you could set this to the walltime minus a grace
+        period for the batch job to start the workers, minus the expected
+        maximum length of an individual task.
+
+    worker_logdir_root : string
+        In case of a remote file system, specify the path to where logs will be kept.
+
     enable_mpi_mode: bool
         If enabled, MPI launch prefixes will be composed for the batch scheduler based on
         the nodes available in each batch job and the resource_specification dict passed
         from the app. This is an experimental feature, please refer to the following doc section
         before use:  https://parsl.readthedocs.io/en/stable/userguide/mpi_apps.html
 
     mpi_launcher: str
         This field is only used if enable_mpi_mode is set. Select one from the
         list of supported MPI launchers = ("srun", "aprun", "mpiexec").
         default: "mpiexec"
+
+    encrypted : bool
+        Flag to enable/disable encryption (CurveZMQ). Default is False.
     """
 
     @typeguard.typechecked
     def __init__(self,
                  label: str = 'HighThroughputExecutor',
                  provider: ExecutionProvider = LocalProvider(),
                  launch_cmd: Optional[str] = None,
@@ -304,14 +301,17 @@
         self._workers_per_node = min(self.max_workers_per_node, mem_slots, cpu_slots)
         if len(self.available_accelerators) > 0:
             self._workers_per_node = min(self._workers_per_node, len(available_accelerators))
         if self._workers_per_node == float('inf'):
             self._workers_per_node = 1  # our best guess-- we do not have any provider hints
 
         self._task_counter = 0
+        self.run_id = None  # set to the correct run_id in dfk
+        self.hub_address = None  # set to the correct hub address in dfk
+        self.hub_port = None  # set to the correct hub port in dfk
         self.worker_ports = worker_ports
         self.worker_port_range = worker_port_range
         self.interchange_proc: Optional[Process] = None
         self.interchange_port_range = interchange_port_range
         self.heartbeat_threshold = heartbeat_threshold
         self.heartbeat_period = heartbeat_period
         self.drain_period = drain_period
@@ -322,16 +322,16 @@
         self.encrypted = encrypted
         self.cert_dir = None
 
         self.enable_mpi_mode = enable_mpi_mode
         assert mpi_launcher in VALID_LAUNCHERS, \
             f"mpi_launcher must be set to one of {VALID_LAUNCHERS}"
         if self.enable_mpi_mode:
-            assert isinstance(self.provider.launcher, parsl.launchers.SimpleLauncher), \
-                "mpi_mode requires the provider to be configured to use a SimpleLauncher"
+            assert isinstance(self.provider.launcher, parsl.launchers.SingleNodeLauncher), \
+                "mpi_mode requires the provider to be configured to use a SingleNodeLauncher"
 
         self.mpi_launcher = mpi_launcher
 
         if not launch_cmd:
             launch_cmd = DEFAULT_LAUNCH_CMD
         self.launch_cmd = launch_cmd
 
@@ -537,15 +537,15 @@
                                             kwargs={"client_ports": (self.outgoing_q.port,
                                                                      self.incoming_q.port,
                                                                      self.command_client.port),
                                                     "interchange_address": self.address,
                                                     "worker_ports": self.worker_ports,
                                                     "worker_port_range": self.worker_port_range,
                                                     "hub_address": self.hub_address,
-                                                    "hub_zmq_port": self.hub_zmq_port,
+                                                    "hub_port": self.hub_port,
                                                     "logdir": self.logdir,
                                                     "heartbeat_threshold": self.heartbeat_threshold,
                                                     "poll_period": self.poll_period,
                                                     "logging_level": logging.DEBUG if self.worker_debug else logging.INFO,
                                                     "cert_dir": self.cert_dir,
                                                     },
                                             daemon=True,
@@ -641,16 +641,15 @@
 
         Kwargs:
             - kwargs (dict) : A dictionary of arbitrary keyword args for func.
 
         Returns:
               Future
         """
-
-        validate_resource_spec(resource_specification, self.enable_mpi_mode)
+        validate_resource_spec(resource_specification)
 
         if self.bad_state_is_set:
             raise self.executor_exception
 
         self._task_counter += 1
         task_id = self._task_counter
```

### Comparing `parsl-2024.5.27/parsl/executors/high_throughput/interchange.py` & `parsl-2024.5.6/parsl/executors/high_throughput/interchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     def __init__(self,
                  client_address: str = "127.0.0.1",
                  interchange_address: Optional[str] = None,
                  client_ports: Tuple[int, int, int] = (50055, 50056, 50057),
                  worker_ports: Optional[Tuple[int, int]] = None,
                  worker_port_range: Tuple[int, int] = (54000, 55000),
                  hub_address: Optional[str] = None,
-                 hub_zmq_port: Optional[int] = None,
+                 hub_port: Optional[int] = None,
                  heartbeat_threshold: int = 60,
                  logdir: str = ".",
                  logging_level: int = logging.INFO,
                  poll_period: int = 10,
                  cert_dir: Optional[str] = None,
                  ) -> None:
         """
@@ -101,15 +101,15 @@
              The interchange picks ports at random from the range which will be used by workers.
              This is overridden when the worker_ports option is set. Default: (54000, 55000)
 
         hub_address : str
              The IP address at which the interchange can send info about managers to when monitoring is enabled.
              Default: None (meaning monitoring disabled)
 
-        hub_zmq_port : str
+        hub_port : str
              The port at which the interchange can send info about managers to when monitoring is enabled.
              Default: None (meaning monitoring disabled)
 
         heartbeat_threshold : int
              Number of seconds since the last heartbeat after which worker is considered lost.
 
         logdir : str
@@ -147,15 +147,15 @@
         self.results_outgoing.connect("tcp://{}:{}".format(client_address, client_ports[1]))
 
         self.command_channel = self.zmq_context.socket(zmq.REP)
         self.command_channel.connect("tcp://{}:{}".format(client_address, client_ports[2]))
         logger.info("Connected to client")
 
         self.hub_address = hub_address
-        self.hub_zmq_port = hub_zmq_port
+        self.hub_port = hub_port
 
         self.pending_task_queue: queue.Queue[Any] = queue.Queue(maxsize=10 ** 6)
         self.count = 0
 
         self.worker_ports = worker_ports
         self.worker_port_range = worker_port_range
 
@@ -240,20 +240,20 @@
 
             logger.debug("putting message onto pending_task_queue")
             self.pending_task_queue.put(msg)
             task_counter += 1
             logger.debug(f"Fetched {task_counter} tasks so far")
 
     def _create_monitoring_channel(self) -> Optional[zmq.Socket]:
-        if self.hub_address and self.hub_zmq_port:
+        if self.hub_address and self.hub_port:
             logger.info("Connecting to MonitoringHub")
             # This is a one-off because monitoring is unencrypted
             hub_channel = zmq.Context().socket(zmq.DEALER)
             hub_channel.set_hwm(0)
-            hub_channel.connect("tcp://{}:{}".format(self.hub_address, self.hub_zmq_port))
+            hub_channel.connect("tcp://{}:{}".format(self.hub_address, self.hub_port))
             logger.info("Connected to MonitoringHub")
             return hub_channel
         else:
             return None
 
     def _send_monitoring_info(self, hub_channel: Optional[zmq.Socket], manager: ManagerRecord) -> None:
         if hub_channel:
@@ -306,16 +306,14 @@
                             idle_duration = 0.0
                         resp = {'manager': manager_id.decode('utf-8'),
                                 'block_id': m['block_id'],
                                 'worker_count': m['worker_count'],
                                 'tasks': len(m['tasks']),
                                 'idle_duration': idle_duration,
                                 'active': m['active'],
-                                'parsl_version': m['parsl_version'],
-                                'python_version': m['python_version'],
                                 'draining': m['draining']}
                         reply.append(resp)
 
                 elif command_req.startswith("HOLD_WORKER"):
                     cmd, s_manager = command_req.split(';')
                     manager_id = s_manager.encode('utf-8')
                     logger.info("Received HOLD_WORKER for {!r}".format(manager_id))
@@ -325,15 +323,14 @@
                         self._send_monitoring_info(hub_channel, m)
                     else:
                         logger.warning("Worker to hold was not in ready managers list")
 
                     reply = None
 
                 else:
-                    logger.error(f"Received unknown command: {command_req}")
                     reply = None
 
                 logger.debug("Reply: {}".format(reply))
                 self.command_channel.send_pyobj(reply)
 
             except zmq.Again:
                 logger.debug("Command thread is alive")
@@ -434,16 +431,14 @@
                 self._ready_managers[manager_id] = {'last_heartbeat': time.time(),
                                                     'idle_since': time.time(),
                                                     'block_id': None,
                                                     'max_capacity': 0,
                                                     'worker_count': 0,
                                                     'active': True,
                                                     'draining': False,
-                                                    'parsl_version': msg['parsl_v'],
-                                                    'python_version': msg['python_v'],
                                                     'tasks': []}
                 self.connected_block_history.append(msg['block_id'])
 
                 interesting_managers.add(manager_id)
                 logger.info("Adding manager: {!r} to ready queue".format(manager_id))
                 m = self._ready_managers[manager_id]
```

### Comparing `parsl-2024.5.27/parsl/executors/high_throughput/mpi_prefix_composer.py` & `parsl-2024.5.6/parsl/executors/high_throughput/mpi_prefix_composer.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,47 +4,31 @@
 logger = logging.getLogger(__name__)
 
 VALID_LAUNCHERS = ('srun',
                    'aprun',
                    'mpiexec')
 
 
-class MissingResourceSpecification(Exception):
-    """Exception raised when input is  not supplied a resource specification"""
-
-    def __init__(self, reason: str):
-        self.reason = reason
-
-    def __str__(self):
-        return f"Missing resource specification: {self.reason}"
-
-
 class InvalidResourceSpecification(Exception):
-    """Exception raised when Invalid input is supplied via resource specification"""
+    """Exception raised when Invalid keys are supplied via resource specification"""
 
     def __init__(self, invalid_keys: Set[str]):
         self.invalid_keys = invalid_keys
 
     def __str__(self):
         return f"Invalid resource specification options supplied: {self.invalid_keys}"
 
 
-def validate_resource_spec(resource_spec: Dict[str, str], is_mpi_enabled: bool):
+def validate_resource_spec(resource_spec: Dict[str, str]):
     """Basic validation of keys in the resource_spec
 
     Raises: InvalidResourceSpecification if the resource_spec
         is invalid (e.g, contains invalid keys)
     """
     user_keys = set(resource_spec.keys())
-
-    # empty resource_spec when mpi_mode is set causes parsl to hang
-    # ref issue #3427
-    if is_mpi_enabled and len(user_keys) == 0:
-        raise MissingResourceSpecification('MPI mode requires optional parsl_resource_specification keyword argument to be configured')
-
     legal_keys = set(("ranks_per_node",
                       "num_nodes",
                       "num_ranks",
                       "launcher_options",
                       ))
     invalid_keys = user_keys - legal_keys
     if invalid_keys:
```

### Comparing `parsl-2024.5.27/parsl/executors/high_throughput/mpi_resource_management.py` & `parsl-2024.5.6/parsl/executors/high_throughput/mpi_resource_management.py`

 * *Files 8% similar despite different names*

```diff
@@ -204,17 +204,14 @@
             # Keep attempting to schedule tasks till we are out of resources
             self._schedule_backlog_tasks()
 
     def get_result(self, block: bool, timeout: float):
         """Return result and relinquish provisioned nodes"""
         result_pkl = self.pending_result_q.get(block, timeout=timeout)
         result_dict = pickle.loads(result_pkl)
-        # TODO (wardlt): If the task did not request nodes, it won't be in `self._map_tasks_to_nodes`.
-        #  Causes Parsl to hang. See Issue #3427
         if result_dict["type"] == "result":
             task_id = result_dict["task_id"]
-            assert task_id in self._map_tasks_to_nodes, "You are about to experience issue #3427"
             nodes_to_reallocate = self._map_tasks_to_nodes[task_id]
             self._return_nodes(nodes_to_reallocate)
             self._schedule_backlog_tasks()
 
         return result_pkl
```

### Comparing `parsl-2024.5.27/parsl/executors/high_throughput/probe.py` & `parsl-2024.5.6/parsl/executors/high_throughput/probe.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/high_throughput/process_worker_pool.py` & `parsl-2024.5.6/parsl/executors/high_throughput/process_worker_pool.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/radical/executor.py` & `parsl-2024.5.6/parsl/executors/radical/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/radical/rpex_master.py` & `parsl-2024.5.6/parsl/executors/radical/rpex_master.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/radical/rpex_resources.py` & `parsl-2024.5.6/parsl/executors/radical/rpex_resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import sys
 import json
 
 from typing import List
 
-_setup_paths: List[str] = []
+_setup_paths: List[str]
 try:
     import radical.pilot as rp
+    import radical.utils as ru
 except ImportError:
-    pass
+    _setup_paths = []
+else:
+    _setup_paths = [rp.sdist_path,
+                    ru.sdist_path]
 
 
 MPI = "mpi"
 RP_ENV = "rp"
 CLIENT = "client"
 RPEX_ENV = "ve_rpex"
 MPI_WORKER = "MPIWorker"
@@ -69,15 +73,15 @@
 
     pilot_env_type : str
         The type of the pilot environment (e.g., 'venv', 'conda').
         Default is "venv".
 
     pilot_env_setup : list
         List of setup commands/packages for the pilot environment.
-        Default is an empty list.
+        Default setup includes "parsl", rp.sdist_path, and ru.sdist_path.
 
     python_v : str
         The Python version to be used in the pilot environment.
         Default is determined by the system's Python version.
 
     worker_type : str
         The type of worker(s) to be deployed by RAPTOR on the compute
```

### Comparing `parsl-2024.5.27/parsl/executors/radical/rpex_worker.py` & `parsl-2024.5.6/parsl/executors/radical/rpex_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/status_handling.py` & `parsl-2024.5.6/parsl/executors/status_handling.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/taskvine/errors.py` & `parsl-2024.5.6/parsl/executors/taskvine/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/taskvine/exec_parsl_function.py` & `parsl-2024.5.6/parsl/executors/taskvine/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/taskvine/executor.py` & `parsl-2024.5.6/parsl/executors/taskvine/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/taskvine/factory.py` & `parsl-2024.5.6/parsl/executors/taskvine/factory.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/taskvine/factory_config.py` & `parsl-2024.5.6/parsl/executors/taskvine/factory_config.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/taskvine/manager.py` & `parsl-2024.5.6/parsl/executors/taskvine/manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/taskvine/manager_config.py` & `parsl-2024.5.6/parsl/executors/taskvine/manager_config.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/taskvine/utils.py` & `parsl-2024.5.6/parsl/executors/taskvine/utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/threads.py` & `parsl-2024.5.6/parsl/executors/threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/workqueue/errors.py` & `parsl-2024.5.6/parsl/executors/workqueue/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/workqueue/exec_parsl_function.py` & `parsl-2024.5.6/parsl/executors/workqueue/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/workqueue/executor.py` & `parsl-2024.5.6/parsl/executors/workqueue/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/workqueue/parsl_coprocess.py` & `parsl-2024.5.6/parsl/executors/workqueue/parsl_coprocess.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/executors/workqueue/parsl_coprocess_stub.py` & `parsl-2024.5.6/parsl/executors/workqueue/parsl_coprocess_stub.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/jobs/error_handlers.py` & `parsl-2024.5.6/parsl/jobs/error_handlers.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/jobs/job_status_poller.py` & `parsl-2024.5.6/parsl/jobs/job_status_poller.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/jobs/states.py` & `parsl-2024.5.6/parsl/jobs/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/jobs/strategy.py` & `parsl-2024.5.6/parsl/jobs/strategy.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/launchers/__init__.py` & `parsl-2024.5.6/parsl/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/launchers/base.py` & `parsl-2024.5.6/parsl/launchers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/launchers/launchers.py` & `parsl-2024.5.6/parsl/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/log_utils.py` & `parsl-2024.5.6/parsl/log_utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/db_manager.py` & `parsl-2024.5.6/parsl/monitoring/db_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/monitoring.py` & `parsl-2024.5.6/parsl/monitoring/monitoring.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/queries/pandas.py` & `parsl-2024.5.6/parsl/monitoring/queries/pandas.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/radios.py` & `parsl-2024.5.6/parsl/monitoring/radios.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/remote.py` & `parsl-2024.5.6/parsl/monitoring/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,30 +92,14 @@
     new_kwargs = kwargs.copy()
     new_kwargs['_parsl_monitoring_task_id'] = x_task_id
     new_kwargs['_parsl_monitoring_try_id'] = x_try_id
 
     return (wrapped, args, new_kwargs)
 
 
-def get_radio(radio_mode: str, monitoring_hub_url: str, task_id: int, run_dir: str) -> MonitoringRadio:
-    radio: MonitoringRadio
-    if radio_mode == "udp":
-        radio = UDPRadio(monitoring_hub_url,
-                         source_id=task_id)
-    elif radio_mode == "htex":
-        radio = HTEXRadio(monitoring_hub_url,
-                          source_id=task_id)
-    elif radio_mode == "filesystem":
-        radio = FilesystemRadio(monitoring_url=monitoring_hub_url,
-                                source_id=task_id, run_dir=run_dir)
-    else:
-        raise RuntimeError(f"Unknown radio mode: {radio_mode}")
-    return radio
-
-
 @wrap_with_logs
 def send_first_message(try_id: int,
                        task_id: int,
                        monitoring_hub_url: str,
                        run_id: str, radio_mode: str, run_dir: str) -> None:
     send_first_last_message(try_id, task_id, monitoring_hub_url, run_id,
                             radio_mode, run_dir, False)
@@ -134,15 +118,26 @@
                             task_id: int,
                             monitoring_hub_url: str,
                             run_id: str, radio_mode: str, run_dir: str,
                             is_last: bool) -> None:
     import platform
     import os
 
-    radio = get_radio(radio_mode, monitoring_hub_url, task_id, run_dir)
+    radio: MonitoringRadio
+    if radio_mode == "udp":
+        radio = UDPRadio(monitoring_hub_url,
+                         source_id=task_id)
+    elif radio_mode == "htex":
+        radio = HTEXRadio(monitoring_hub_url,
+                          source_id=task_id)
+    elif radio_mode == "filesystem":
+        radio = FilesystemRadio(monitoring_url=monitoring_hub_url,
+                                source_id=task_id, run_dir=run_dir)
+    else:
+        raise RuntimeError(f"Unknown radio mode: {radio_mode}")
 
     msg = (MessageType.RESOURCE_INFO,
            {'run_id': run_id,
             'try_id': try_id,
             'task_id': task_id,
             'hostname': platform.node(),
             'block_id': os.environ.get('PARSL_WORKER_BLOCK_ID'),
@@ -179,15 +174,26 @@
     import platform
     import psutil
 
     from parsl.utils import setproctitle
 
     setproctitle("parsl: task resource monitor")
 
-    radio = get_radio(radio_mode, monitoring_hub_url, task_id, run_dir)
+    radio: MonitoringRadio
+    if radio_mode == "udp":
+        radio = UDPRadio(monitoring_hub_url,
+                         source_id=task_id)
+    elif radio_mode == "htex":
+        radio = HTEXRadio(monitoring_hub_url,
+                          source_id=task_id)
+    elif radio_mode == "filesystem":
+        radio = FilesystemRadio(monitoring_url=monitoring_hub_url,
+                                source_id=task_id, run_dir=run_dir)
+    else:
+        raise RuntimeError(f"Unknown radio mode: {radio_mode}")
 
     logging.debug("start of monitor")
 
     # these values are simple to log. Other information is available in special formats such as memory below.
     simple = ["cpu_num", 'create_time', 'cwd', 'exe', 'memory_percent', 'nice', 'name', 'num_threads', 'pid', 'ppid', 'status', 'username']
     # values that can be summed up to see total resources used by task process and its children
     summable_values = ['memory_percent', 'num_threads']
```

### Comparing `parsl-2024.5.27/parsl/monitoring/router.py` & `parsl-2024.5.6/parsl/monitoring/router.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/types.py` & `parsl-2024.5.6/parsl/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/app.py` & `parsl-2024.5.6/parsl/monitoring/visualization/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/models.py` & `parsl-2024.5.6/parsl/monitoring/visualization/models.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/plots/default/task_plots.py` & `parsl-2024.5.6/parsl/monitoring/visualization/plots/default/task_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/plots/default/workflow_plots.py` & `parsl-2024.5.6/parsl/monitoring/visualization/plots/default/workflow_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py` & `parsl-2024.5.6/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/static/parsl-logo-white.png` & `parsl-2024.5.6/parsl/monitoring/visualization/static/parsl-logo-white.png`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/templates/app.html` & `parsl-2024.5.6/parsl/monitoring/visualization/templates/app.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/templates/dag.html` & `parsl-2024.5.6/parsl/monitoring/visualization/templates/dag.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/templates/layout.html` & `parsl-2024.5.6/parsl/monitoring/visualization/templates/layout.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/templates/resource_usage.html` & `parsl-2024.5.6/parsl/monitoring/visualization/templates/resource_usage.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/templates/task.html` & `parsl-2024.5.6/parsl/monitoring/visualization/templates/task.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/templates/workflow.html` & `parsl-2024.5.6/parsl/monitoring/visualization/templates/workflow.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/templates/workflows_summary.html` & `parsl-2024.5.6/parsl/monitoring/visualization/templates/workflows_summary.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/monitoring/visualization/views.py` & `parsl-2024.5.6/parsl/monitoring/visualization/views.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/multiprocessing.py` & `parsl-2024.5.6/parsl/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/process_loggers.py` & `parsl-2024.5.6/parsl/process_loggers.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/__init__.py` & `parsl-2024.5.6/parsl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/ad_hoc/ad_hoc.py` & `parsl-2024.5.6/parsl/providers/ad_hoc/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/aws/aws.py` & `parsl-2024.5.6/parsl/providers/aws/aws.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/azure/azure.py` & `parsl-2024.5.6/parsl/providers/azure/azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/base.py` & `parsl-2024.5.6/parsl/providers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/cluster_provider.py` & `parsl-2024.5.6/parsl/providers/cluster_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/cobalt/cobalt.py` & `parsl-2024.5.6/parsl/providers/cobalt/cobalt.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/condor/condor.py` & `parsl-2024.5.6/parsl/providers/condor/condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/condor/template.py` & `parsl-2024.5.6/parsl/providers/condor/template.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/errors.py` & `parsl-2024.5.6/parsl/providers/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/googlecloud/googlecloud.py` & `parsl-2024.5.6/parsl/providers/googlecloud/googlecloud.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/grid_engine/grid_engine.py` & `parsl-2024.5.6/parsl/providers/grid_engine/grid_engine.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/kubernetes/kube.py` & `parsl-2024.5.6/parsl/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/local/local.py` & `parsl-2024.5.6/parsl/providers/local/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
         job_name = "{0}.{1}".format(job_name, time.time())
 
         # Set script path
         script_path = "{0}/{1}.sh".format(self.script_dir, job_name)
         script_path = os.path.abspath(script_path)
 
-        wrap_command = self.worker_init + f'\nexport JOBNAME={job_name}\n' + self.launcher(command, tasks_per_node, self.nodes_per_block)
+        wrap_command = self.worker_init + f'\nexport JOBNAME=${job_name}\n' + self.launcher(command, tasks_per_node, self.nodes_per_block)
 
         self._write_submit_script(wrap_command, script_path)
 
         job_id = None
         remote_pid = None
         if self._should_move_files():
             logger.debug("Pushing start script")
```

### Comparing `parsl-2024.5.27/parsl/providers/lsf/lsf.py` & `parsl-2024.5.6/parsl/providers/lsf/lsf.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/pbspro/pbspro.py` & `parsl-2024.5.6/parsl/providers/pbspro/pbspro.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import time
 import json
 
 from parsl.channels import LocalChannel
 from parsl.jobs.states import JobState, JobStatus
 from parsl.launchers import SingleNodeLauncher
 from parsl.providers.pbspro.template import template_string
-from parsl.providers.torque.torque import TorqueProvider, translate_table
+from parsl.providers import TorqueProvider
+
+from parsl.providers.torque.torque import translate_table
 
 logger = logging.getLogger(__name__)
 
 
 class PBSProProvider(TorqueProvider):
     """PBS Pro Execution Provider
```

### Comparing `parsl-2024.5.27/parsl/providers/slurm/slurm.py` & `parsl-2024.5.6/parsl/providers/slurm/slurm.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/providers/torque/torque.py` & `parsl-2024.5.6/parsl/providers/torque/torque.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/serialize/base.py` & `parsl-2024.5.6/parsl/serialize/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/serialize/concretes.py` & `parsl-2024.5.6/parsl/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/serialize/errors.py` & `parsl-2024.5.6/parsl/serialize/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/serialize/facade.py` & `parsl-2024.5.6/parsl/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/serialize/proxystore.py` & `parsl-2024.5.6/parsl/serialize/proxystore.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/ad_hoc_cluster_htex.py` & `parsl-2024.5.6/parsl/tests/configs/ad_hoc_cluster_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/azure_single_node.py` & `parsl-2024.5.6/parsl/tests/configs/azure_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/bluewaters.py` & `parsl-2024.5.6/parsl/tests/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/bridges.py` & `parsl-2024.5.6/parsl/tests/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/cc_in2p3.py` & `parsl-2024.5.6/parsl/tests/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/comet.py` & `parsl-2024.5.6/parsl/tests/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/cooley_htex.py` & `parsl-2024.5.6/parsl/tests/configs/cooley_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/ec2_single_node.py` & `parsl-2024.5.6/parsl/tests/configs/ec2_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/ec2_spot.py` & `parsl-2024.5.6/parsl/tests/configs/ec2_spot.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/frontera.py` & `parsl-2024.5.6/parsl/tests/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/htex_ad_hoc_cluster.py` & `parsl-2024.5.6/parsl/tests/configs/htex_ad_hoc_cluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/htex_local.py` & `parsl-2024.5.6/parsl/tests/configs/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/htex_local_alternate.py` & `parsl-2024.5.6/parsl/tests/configs/htex_local_alternate.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/htex_local_intask_staging.py` & `parsl-2024.5.6/parsl/tests/configs/htex_local_intask_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/htex_local_rsync_staging.py` & `parsl-2024.5.6/parsl/tests/configs/htex_local_rsync_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/local_radical_mpi.py` & `parsl-2024.5.6/parsl/tests/configs/local_radical_mpi.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/local_threads_globus.py` & `parsl-2024.5.6/parsl/tests/configs/local_threads_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/midway.py` & `parsl-2024.5.6/parsl/tests/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/nscc_singapore.py` & `parsl-2024.5.6/parsl/tests/configs/nscc_singapore.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/osg_htex.py` & `parsl-2024.5.6/parsl/tests/configs/osg_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/petrelkube.py` & `parsl-2024.5.6/parsl/tests/configs/petrelkube.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/summit.py` & `parsl-2024.5.6/parsl/tests/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/swan_htex.py` & `parsl-2024.5.6/parsl/tests/configs/swan_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/theta.py` & `parsl-2024.5.6/parsl/tests/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/configs/user_opts.py` & `parsl-2024.5.6/parsl/tests/configs/user_opts.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/conftest.py` & `parsl-2024.5.6/parsl/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
             ex.working_dir = tmpd_cwd_session
 
         yield
 
         if parsl.dfk() != dfk:
             raise RuntimeError("DFK changed unexpectedly during test")
         dfk.cleanup()
-        assert DataFlowKernelLoader._dfk is None
+        parsl.clear()
     else:
         yield
 
 
 @pytest.fixture(autouse=True, scope='module')
 def load_dfk_local_module(request, pytestconfig, tmpd_cwd_session):
     """Load the dfk around test modules, in local mode.
@@ -249,15 +249,15 @@
             local_teardown()
             assert DataFlowKernelLoader._dfk is None, "Expected teardown to clear DFK"
 
         if local_config:
             if parsl.dfk() != dfk:
                 raise RuntimeError("DFK changed unexpectedly during test")
             dfk.cleanup()
-            assert DataFlowKernelLoader._dfk is None
+            parsl.clear()
 
     else:
         yield
 
 
 @pytest.fixture(autouse=True)
 def apply_masks(request, pytestconfig):
```

### Comparing `parsl-2024.5.27/parsl/tests/integration/latency.py` & `parsl-2024.5.6/parsl/tests/integration/latency.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/integration/test_channels/test_local_channel.py` & `parsl-2024.5.6/parsl/tests/integration/test_channels/test_local_channel.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/integration/test_channels/test_scp_1.py` & `parsl-2024.5.6/parsl/tests/integration/test_channels/test_scp_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/integration/test_channels/test_ssh_1.py` & `parsl-2024.5.6/parsl/tests/integration/test_channels/test_ssh_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/integration/test_channels/test_ssh_errors.py` & `parsl-2024.5.6/parsl/tests/integration/test_channels/test_ssh_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/integration/test_channels/test_ssh_file_transport.py` & `parsl-2024.5.6/parsl/tests/integration/test_channels/test_ssh_file_transport.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/integration/test_channels/test_ssh_interactive.py` & `parsl-2024.5.6/parsl/tests/integration/test_channels/test_ssh_interactive.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/integration/test_stress/test_python_simple.py` & `parsl-2024.5.6/parsl/tests/integration/test_stress/test_python_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/integration/test_stress/test_python_threads.py` & `parsl-2024.5.6/parsl/tests/integration/test_stress/test_python_threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/manual_tests/htex_local.py` & `parsl-2024.5.6/parsl/tests/manual_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/manual_tests/test_ad_hoc_htex.py` & `parsl-2024.5.6/parsl/tests/manual_tests/test_ad_hoc_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/manual_tests/test_basic.py` & `parsl-2024.5.6/parsl/tests/manual_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py` & `parsl-2024.5.6/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/manual_tests/test_log_filter.py` & `parsl-2024.5.6/parsl/tests/manual_tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/manual_tests/test_memory_limits.py` & `parsl-2024.5.6/parsl/tests/manual_tests/test_memory_limits.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/manual_tests/test_regression_220.py` & `parsl-2024.5.6/parsl/tests/manual_tests/test_regression_220.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/manual_tests/test_udp_simple.py` & `parsl-2024.5.6/parsl/tests/manual_tests/test_udp_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/manual_tests/test_worker_count.py` & `parsl-2024.5.6/parsl/tests/manual_tests/test_worker_count.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/scaling_tests/htex_local.py` & `parsl-2024.5.6/parsl/tests/scaling_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/scaling_tests/test_scale.py` & `parsl-2024.5.6/parsl/tests/scaling_tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/scaling_tests/wqex_condor.py` & `parsl-2024.5.6/parsl/tests/scaling_tests/wqex_condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/scaling_tests/wqex_local.py` & `parsl-2024.5.6/parsl/tests/scaling_tests/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/site_tests/site_config_selector.py` & `parsl-2024.5.6/parsl/tests/site_tests/site_config_selector.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/site_tests/test_provider.py` & `parsl-2024.5.6/parsl/tests/site_tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/site_tests/test_site.py` & `parsl-2024.5.6/parsl/tests/site_tests/test_site.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/sites/test_affinity.py` & `parsl-2024.5.6/parsl/tests/sites/test_affinity.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/sites/test_concurrent.py` & `parsl-2024.5.6/parsl/tests/sites/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/sites/test_dynamic_executor.py` & `parsl-2024.5.6/parsl/tests/sites/test_dynamic_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,7 +71,8 @@
     tasks = [add() for i in range(10)]
     results = [i.result() for i in tasks]
     print("Successfully added htex executor and ran with it. The results are", results)
 
     print("Done testing")
 
     dfk.cleanup()
+    parsl.clear()
```

### Comparing `parsl-2024.5.27/parsl/tests/sites/test_ec2.py` & `parsl-2024.5.6/parsl/tests/sites/test_ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/sites/test_local_adhoc.py` & `parsl-2024.5.6/parsl/tests/sites/test_local_adhoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/sites/test_worker_info.py` & `parsl-2024.5.6/parsl/tests/sites/test_worker_info.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_aalst_patterns.py` & `parsl-2024.5.6/parsl/tests/test_aalst_patterns.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_bash_apps/test_apptimeout.py` & `parsl-2024.5.6/parsl/tests/test_bash_apps/test_apptimeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_bash_apps/test_basic.py` & `parsl-2024.5.6/parsl/tests/test_bash_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_bash_apps/test_error_codes.py` & `parsl-2024.5.6/parsl/tests/test_bash_apps/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_bash_apps/test_kwarg_storage.py` & `parsl-2024.5.6/parsl/tests/test_bash_apps/test_kwarg_storage.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_bash_apps/test_memoize.py` & `parsl-2024.5.6/parsl/tests/test_bash_apps/test_memoize.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_bash_apps/test_memoize_ignore_args.py` & `parsl-2024.5.6/parsl/tests/test_bash_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py` & `parsl-2024.5.6/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_bash_apps/test_multiline.py` & `parsl-2024.5.6/parsl/tests/test_bash_apps/test_multiline.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_bash_apps/test_pipeline.py` & `parsl-2024.5.6/parsl/tests/test_bash_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_bash_apps/test_std_uri.py` & `parsl-2024.5.6/parsl/tests/test_bash_apps/test_std_uri.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
     with open(content_path, "r") as file:
         assert file.readlines() == ["hello\n"]
 
     for record in caplog.records:
         assert record.levelno < logging.ERROR
 
+    parsl.clear()
+
 
 @pytest.mark.local
 def test_std_autopath_const_str(caplog, tmpd_cwd):
     """Tests str and tuple mode autopaths with constant autopath, which should
     all be passed through unmodified.
     """
     cpath = str(tmpd_cwd / "CONST")
@@ -68,14 +70,16 @@
 
 @pytest.mark.local
 def test_std_autopath_fail(caplog):
     with parsl.load(parsl.Config(std_autopath=fail_uri)):
         with pytest.raises(URIFailError):
             app_stdout()
 
+    parsl.clear()
+
 
 @parsl.bash_app
 def app_both(stdout=parsl.AUTO_LOGNAME, stderr=parsl.AUTO_LOGNAME):
     return "echo hello; echo goodbye >&2"
 
 
 def zip_uri(base, task_record, err_or_out):
@@ -116,7 +120,9 @@
 
                 stderr_relative_path = f"app_both.{fut.tid}.0.stderr"
                 with z.open(stderr_relative_path) as f:
                     assert f.readlines()[-1] == b'goodbye\n'
 
     for record in caplog.records:
         assert record.levelno < logging.ERROR
+
+    parsl.clear()
```

### Comparing `parsl-2024.5.27/parsl/tests/test_bash_apps/test_stdout.py` & `parsl-2024.5.6/parsl/tests/test_bash_apps/test_stdout.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_callables.py` & `parsl-2024.5.6/parsl/tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_channels/test_large_output.py` & `parsl-2024.5.6/parsl/tests/test_channels/test_large_output.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_checkpointing/test_periodic.py` & `parsl-2024.5.6/parsl/tests/test_checkpointing/test_periodic.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 from parsl.tests.configs.local_threads_checkpoint_periodic import fresh_config
 
 
 def local_setup():
     parsl.load(fresh_config())
 
 
+def local_teardown():
+    # explicit clear without dfk.cleanup here, because the
+    # test does that already
+    parsl.clear()
+
+
 @python_app(cache=True)
 def slow_double(x, sleep_dur=1):
     import time
     time.sleep(sleep_dur)
     return x * 2
 
 
@@ -29,18 +35,17 @@
     assert h == 0, "Verify test setup"
     assert m == 0, "Verify test setup"
     assert s > 0, "Verify test setup"
     sleep_for = s + 1
     with parsl.dfk():
         futs = [slow_double(sleep_for) for _ in range(4)]
         [f.result() for f in futs]
-        run_dir = parsl.dfk().run_dir
 
     # Here we will check if the loglines came back with 5 seconds deltas
-    with open("{}/parsl.log".format(run_dir)) as f:
+    with open("{}/parsl.log".format(parsl.dfk().run_dir)) as f:
         log_lines = f.readlines()
     expected_msg = " Done checkpointing"
     expected_msg2 = " No tasks checkpointed in this pass"
 
     lines = [line for line in log_lines if expected_msg in line or expected_msg2 in line]
     assert len(lines) >= 3, "Insufficient checkpoint lines in logfile"
     deltas = [tstamp_to_seconds(line) for line in lines]
```

### Comparing `parsl-2024.5.27/parsl/tests/test_checkpointing/test_python_checkpoint_1.py` & `parsl-2024.5.6/parsl/tests/test_checkpointing/test_python_checkpoint_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_checkpointing/test_python_checkpoint_2.py` & `parsl-2024.5.6/parsl/tests/test_checkpointing/test_python_checkpoint_2.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         setattr(c, config_attr, config_val)
     dfk = parsl.load(c)
     for ex in dfk.executors.values():
         ex.working_dir = run_dir
     yield dfk
 
     parsl.dfk().cleanup()
+    parsl.clear()
 
 
 @python_app(cache=True)
 def uuid_app():
     import uuid
     return uuid.uuid4()
```

### Comparing `parsl-2024.5.27/parsl/tests/test_checkpointing/test_python_checkpoint_3.py` & `parsl-2024.5.6/parsl/tests/test_checkpointing/test_python_checkpoint_3.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def local_setup():
     global dfk
     dfk = parsl.load(config)
 
 
 def local_teardown():
     parsl.dfk().cleanup()
+    parsl.clear()
 
 
 @python_app
 def slow_double(x, sleep_dur=1, cache=True):
     import time
     time.sleep(sleep_dur)
     return x * 2
```

### Comparing `parsl-2024.5.27/parsl/tests/test_checkpointing/test_regression_232.py` & `parsl-2024.5.6/parsl/tests/test_checkpointing/test_regression_232.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_checkpointing/test_regression_233.py` & `parsl-2024.5.6/parsl/tests/test_checkpointing/test_regression_233.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_checkpointing/test_regression_239.py` & `parsl-2024.5.6/parsl/tests/test_checkpointing/test_regression_239.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_checkpointing/test_task_exit.py` & `parsl-2024.5.6/parsl/tests/test_checkpointing/test_task_exit.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def local_setup():
     global dfk
     dfk = parsl.load(config)
 
 
 def local_teardown():
     parsl.dfk().cleanup()
+    parsl.clear()
 
 
 @python_app(cache=True)
 def slow_double(x, sleep_dur=1):
     import time
     time.sleep(sleep_dur)
     return x * 2
```

### Comparing `parsl-2024.5.27/parsl/tests/test_curvezmq.py` & `parsl-2024.5.6/parsl/tests/test_curvezmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_docs/test_from_slides.py` & `parsl-2024.5.6/parsl/tests/test_docs/test_from_slides.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_docs/test_kwargs.py` & `parsl-2024.5.6/parsl/tests/test_docs/test_kwargs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_docs/test_tutorial_1.py` & `parsl-2024.5.6/parsl/tests/test_docs/test_tutorial_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_docs/test_workflow1.py` & `parsl-2024.5.6/parsl/tests/test_docs/test_workflow1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_docs/test_workflow2.py` & `parsl-2024.5.6/parsl/tests/test_docs/test_workflow2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_docs/test_workflow4.py` & `parsl-2024.5.6/parsl/tests/test_docs/test_workflow4.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_error_handling/test_python_walltime.py` & `parsl-2024.5.6/parsl/tests/test_error_handling/test_python_walltime.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_error_handling/test_rand_fail.py` & `parsl-2024.5.6/parsl/tests/test_error_handling/test_rand_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_error_handling/test_resource_spec.py` & `parsl-2024.5.6/parsl/tests/test_error_handling/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_error_handling/test_retries.py` & `parsl-2024.5.6/parsl/tests/test_error_handling/test_retries.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_error_handling/test_retry_handler.py` & `parsl-2024.5.6/parsl/tests/test_error_handling/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_error_handling/test_retry_handler_failure.py` & `parsl-2024.5.6/parsl/tests/test_error_handling/test_retry_handler_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_error_handling/test_serialization_fail.py` & `parsl-2024.5.6/parsl/tests/test_error_handling/test_serialization_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_error_handling/test_wrap_with_logs.py` & `parsl-2024.5.6/parsl/tests/test_error_handling/test_wrap_with_logs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_flux.py` & `parsl-2024.5.6/parsl/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_htex/test_connected_blocks.py` & `parsl-2024.5.6/parsl/tests/test_htex/test_connected_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_htex/test_cpu_affinity_explicit.py` & `parsl-2024.5.6/parsl/tests/test_htex/test_cpu_affinity_explicit.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,13 +33,20 @@
     logger.debug(f"Will test with affinity for one worker, one core: {affinity}")
 
     config = fresh_config()
     config.executors[0].cpu_affinity = affinity
     config.executors[0].max_workers_per_node = 1
 
     logger.debug(f"config: {config}")
+    # TODO: is there a `with` style for this, to properly deal with exceptions?
+
+    parsl.load(config)
+    try:
 
-    with parsl.load(config):
         worker_affinity = my_affinity().result()
         logger.debug(f"worker reported this affinity: {worker_affinity}")
         assert len(worker_affinity) == 1
         assert worker_affinity == set((single_core,))
+
+    finally:
+        parsl.dfk().cleanup()
+        parsl.clear()
```

### Comparing `parsl-2024.5.27/parsl/tests/test_htex/test_disconnected_blocks.py` & `parsl-2024.5.6/parsl/tests/test_htex/test_disconnected_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_htex/test_drain.py` & `parsl-2024.5.6/parsl/tests/test_htex/test_drain.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_htex/test_htex.py` & `parsl-2024.5.6/parsl/tests/test_htex/test_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_htex/test_manager_failure.py` & `parsl-2024.5.6/parsl/tests/test_htex/test_manager_failure.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     config.executors[0].max_workers_per_node = 1
     config.executors[0].heartbeat_period = 1
 
     parsl.load(config)
     yield
 
     parsl.dfk().cleanup()
+    parsl.clear()
 
 
 @python_app
 def get_worker_pid():
     import os
     return os.getpid()
```

### Comparing `parsl-2024.5.27/parsl/tests/test_htex/test_missing_worker.py` & `parsl-2024.5.6/parsl/tests/test_htex/test_missing_worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import pytest
 
 import parsl
 from parsl.app.app import python_app
 from parsl.tests.configs.htex_local import fresh_config
 
 
-def local_config():
+def local_setup():
     config = fresh_config()
     config.executors[0].poll_period = 1
     config.executors[0].max_workers_per_node = 1
     config.executors[0].launch_cmd = "executable_that_hopefully_does_not_exist_1030509.py"
-    return config
+    parsl.load(config)
+
+
+def local_teardown():
+
+    parsl.dfk().cleanup()
+    parsl.clear()
 
 
 @python_app
 def dummy():
     pass
```

### Comparing `parsl-2024.5.27/parsl/tests/test_htex/test_multiple_disconnected_blocks.py` & `parsl-2024.5.6/parsl/tests/test_htex/test_multiple_disconnected_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_htex/test_worker_failure.py` & `parsl-2024.5.6/parsl/tests/test_htex/test_worker_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_htex/test_zmq_binding.py` & `parsl-2024.5.6/parsl/tests/test_htex/test_zmq_binding.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_monitoring/test_app_names.py` & `parsl-2024.5.6/parsl/tests/test_monitoring/test_app_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     c.monitoring.logging_endpoint = f"sqlite:///{tmpd_cwd}/monitoring.db"
     parsl.load(c)
 
     app = get_app()
     assert app().result() == expected_result
 
     parsl.dfk().cleanup()
+    parsl.clear()
 
     engine = sqlalchemy.create_engine(c.monitoring.logging_endpoint)
     with engine.begin() as connection:
 
         def count_rows(table: str):
             result = connection.execute(f"SELECT COUNT(*) FROM {table}")
             (c, ) = result.first()
```

### Comparing `parsl-2024.5.27/parsl/tests/test_monitoring/test_basic.py` & `parsl-2024.5.6/parsl/tests/test_monitoring/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,16 @@
     config = fresh_config()
     config.run_dir = tmpd_cwd
     config.monitoring.logging_endpoint = db_url
 
     with parsl.load(config):
         assert this_app().result() == 5
 
+    parsl.clear()
+
     # at this point, we should find one row in the monitoring database.
 
     engine = sqlalchemy.create_engine(db_url)
     with engine.begin() as connection:
 
         result = connection.execute(text("SELECT COUNT(*) FROM workflow"))
         (c, ) = result.first()
```

### Comparing `parsl-2024.5.27/parsl/tests/test_monitoring/test_db_locks.py` & `parsl-2024.5.6/parsl/tests/test_monitoring/test_db_locks.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         # the database manager actually tries to write while the
         # read lock is held. I'm not sure if there is a better way
         # to detect this other than a hopefully long-enough sleep.
         time.sleep(10)
 
     logger.info("cleaning up parsl")
     parsl.dfk().cleanup()
+    parsl.clear()
 
     # at this point, we should find data consistent with executing one
     # task in the database.
 
     logger.info("checking database content")
     with engine.begin() as connection:
```

### Comparing `parsl-2024.5.27/parsl/tests/test_monitoring/test_fuzz_zmq.py` & `parsl-2024.5.6/parsl/tests/test_monitoring/test_fuzz_zmq.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     time.sleep(5)
 
     assert this_app().result() == 5
     assert this_app().result() == 5
 
     logger.info("cleaning up parsl")
     parsl.dfk().cleanup()
+    parsl.clear()
 
     # at this point, we should find one row in the monitoring database.
 
     logger.info("checking database content")
     engine = sqlalchemy.create_engine("sqlite:///runinfo/monitoring.db")
     with engine.begin() as connection:
```

### Comparing `parsl-2024.5.27/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py` & `parsl-2024.5.6/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,16 @@
     db_url = f"sqlite:///{tmpd_cwd}/monitoring.db"
     with parsl.load(fresh_config(tmpd_cwd, strategy, db_url)):
         dfk = parsl.dfk()
         run_id = dfk.run_id
 
         this_app().result()
 
+    parsl.clear()
+
     engine = sqlalchemy.create_engine(db_url)
     with engine.begin() as connection:
 
         binds = {"run_id": run_id}
 
         result = connection.execute(text("SELECT COUNT(DISTINCT block_id) FROM block WHERE run_id = :run_id"), binds)
         (c, ) = result.first()
```

### Comparing `parsl-2024.5.27/parsl/tests/test_monitoring/test_incomplete_futures.py` & `parsl-2024.5.6/parsl/tests/test_monitoring/test_incomplete_futures.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     # this cleanup gives a barrier that allows the monitoring code to store
     # everything it has in the database - without this, there's a race
     # condition that the task will not have arrived in the database yet.
     # A different approach for this test might be to poll the DB for a few
     # seconds, with the assumption "data will arrive in the DB within
     # 30 seconds, but probably much sooner".
     parsl.dfk().cleanup()
+    parsl.clear()
 
     engine = sqlalchemy.create_engine(monitoring_url)
     with engine.begin() as connection:
         result = connection.execute(text("SELECT COUNT(*) FROM task"))
         (task_count, ) = result.first()
         assert task_count == 1
```

### Comparing `parsl-2024.5.27/parsl/tests/test_monitoring/test_memoization_representation.py` & `parsl-2024.5.6/parsl/tests/test_monitoring/test_memoization_representation.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
     assert f1.task_record['hashsum'] == f3.task_record['hashsum']
     assert f1.task_record['hashsum'] == f4.task_record['hashsum']
     assert f1.task_record['hashsum'] != f2.task_record['hashsum']
 
     logger.info("cleaning up parsl")
     parsl.dfk().cleanup()
+    parsl.clear()
 
     # at this point, we should find one row in the monitoring database.
 
     logger.info("checking database content")
     engine = sqlalchemy.create_engine("sqlite:///runinfo/monitoring.db")
     with engine.begin() as connection:
```

### Comparing `parsl-2024.5.27/parsl/tests/test_monitoring/test_stdouterr.py` & `parsl-2024.5.6/parsl/tests/test_monitoring/test_stdouterr.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,16 @@
     c.monitoring.logging_endpoint = f"sqlite:///{tmpd_cwd}/monitoring.db"
     c.executors[0].storage_access = default_staging + [ArbitraryStaging()]
 
     with parsl.load(c):
         kwargs = {stream: stdx}
         stdapp(**kwargs).result()
 
+    parsl.clear()
+
     engine = sqlalchemy.create_engine(c.monitoring.logging_endpoint)
     with engine.begin() as connection:
 
         def count_rows(table: str):
             result = connection.execute(f"SELECT COUNT(*) FROM {table}")
             (c, ) = result.first()
             return c
```

### Comparing `parsl-2024.5.27/parsl/tests/test_monitoring/test_viz_colouring.py` & `parsl-2024.5.6/parsl/tests/test_monitoring/test_viz_colouring.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_mpi_apps/test_bad_mpi_config.py` & `parsl-2024.5.6/parsl/tests/test_mpi_apps/test_bad_mpi_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 import pytest
 
 from parsl import Config
 from parsl.executors import HighThroughputExecutor
-from parsl.launchers import SrunLauncher, AprunLauncher, SimpleLauncher
+from parsl.launchers import SrunLauncher, SingleNodeLauncher, SimpleLauncher, AprunLauncher
 from parsl.providers import SlurmProvider
 
 
 @pytest.mark.local
 def test_bad_launcher_with_mpi_mode():
-    """AssertionError if a launcher other than SimpleLauncher is supplied"""
+    """AssertionError if a launcher other than SingleNodeLauncher is supplied"""
 
-    for launcher in [SrunLauncher(), AprunLauncher()]:
+    for launcher in [SrunLauncher(), SimpleLauncher(), AprunLauncher()]:
         with pytest.raises(AssertionError):
             Config(executors=[
                 HighThroughputExecutor(
                     enable_mpi_mode=True,
                     provider=SlurmProvider(launcher=launcher),
                 )
             ])
 
 
 @pytest.mark.local
 def test_correct_launcher_with_mpi_mode():
-    """Confirm that SimpleLauncher works with mpi_mode"""
+    """Confirm that SingleNodeLauncer works with mpi_mode"""
 
     config = Config(executors=[
         HighThroughputExecutor(
             enable_mpi_mode=True,
-            provider=SlurmProvider(launcher=SimpleLauncher()),
+            provider=SlurmProvider(launcher=SingleNodeLauncher()),
         )
     ])
-    assert isinstance(config.executors[0].provider.launcher, SimpleLauncher)
+    assert isinstance(config.executors[0].provider.launcher, SingleNodeLauncher)
+
+    config = Config(executors=[
+        HighThroughputExecutor(
+            enable_mpi_mode=True,
+            provider=SlurmProvider(),
+        )
+    ])
+    assert isinstance(config.executors[0].provider.launcher, SingleNodeLauncher)
```

### Comparing `parsl-2024.5.27/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py` & `parsl-2024.5.6/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+import logging
 from typing import Dict
 import pytest
 import parsl
 from parsl import python_app
 from parsl.tests.configs.htex_local import fresh_config
 
 EXECUTOR_LABEL = "MPI_TEST"
 
 
-def local_config():
+def local_setup():
     config = fresh_config()
     config.executors[0].label = EXECUTOR_LABEL
     config.executors[0].max_workers_per_node = 1
     config.executors[0].enable_mpi_mode = False
-    return config
+    parsl.load(config)
+
+
+def local_teardown():
+    parsl.dfk().cleanup()
+    parsl.clear()
 
 
 @python_app
 def get_env_vars(parsl_resource_specification: Dict = {}) -> Dict:
     import os
 
     parsl_vars = {}
```

### Comparing `parsl-2024.5.27/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py` & `parsl-2024.5.6/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import random
 from typing import Dict
 import pytest
 import parsl
 from parsl import python_app, bash_app
 from parsl.tests.configs.htex_local import fresh_config
 
-from parsl.executors.high_throughput.mpi_prefix_composer import MissingResourceSpecification
-
 import os
 
 EXECUTOR_LABEL = "MPI_TEST"
 
 
 def local_setup():
     config = fresh_config()
@@ -26,14 +24,15 @@
     config.executors[0].provider.worker_init = f"export PBS_NODEFILE={pbs_nodefile}"
 
     parsl.load(config)
 
 
 def local_teardown():
     parsl.dfk().cleanup()
+    parsl.clear()
 
 
 @python_app
 def get_env_vars(parsl_resource_specification: Dict = {}) -> Dict:
     import os
 
     parsl_vars = {}
@@ -166,15 +165,7 @@
                           parsl_resource_specification=resource_spec)
         futures[future] = resource_spec
 
     for future in futures:
         total_ranks, nodes = future.result(timeout=10)
         assert len(nodes) == futures[future]["num_nodes"]
         assert total_ranks == futures[future]["num_nodes"] * futures[future]["ranks_per_node"]
-
-
-@pytest.mark.local
-def test_missing_resource_spec():
-
-    with pytest.raises(MissingResourceSpecification):
-        future = mock_app(sleep_dur=0.4)
-        future.result(timeout=10)
```

### Comparing `parsl-2024.5.27/parsl/tests/test_mpi_apps/test_mpi_prefix.py` & `parsl-2024.5.6/parsl/tests/test_mpi_apps/test_mpi_prefix.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_mpi_apps/test_mpi_scheduler.py` & `parsl-2024.5.6/parsl/tests/test_mpi_apps/test_mpi_scheduler.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_mpi_apps/test_resource_spec.py` & `parsl-2024.5.6/parsl/tests/test_mpi_apps/test_resource_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     get_pbs_hosts_list,
     get_slurm_hosts_list,
     get_nodes_in_batchjob,
     identify_scheduler,
 )
 from parsl.executors.high_throughput.mpi_prefix_composer import (
     validate_resource_spec,
-    InvalidResourceSpecification,
-    MissingResourceSpecification
+    InvalidResourceSpecification
 )
 
 EXECUTOR_LABEL = "MPI_TEST"
 
 
 def local_config():
     config = fresh_config()
@@ -119,26 +118,22 @@
         scheduler = identify_scheduler()
         nodelist = get_nodes_in_batchjob(scheduler)
         assert len(nodelist) > 0
 
 
 @pytest.mark.local
 @pytest.mark.parametrize(
-    "resource_spec, is_mpi_enabled, exception",
+    "resource_spec, exception",
     (
-        ({"num_nodes": 2, "ranks_per_node": 1}, False, None),
-        ({"launcher_options": "--debug_foo"}, False, None),
-        ({"num_nodes": 2, "BAD_OPT": 1}, False, InvalidResourceSpecification),
-        ({}, False, None),
-        ({"num_nodes": 2, "ranks_per_node": 1}, True, None),
-        ({"launcher_options": "--debug_foo"}, True, None),
-        ({"num_nodes": 2, "BAD_OPT": 1}, True, InvalidResourceSpecification),
-        ({}, True, MissingResourceSpecification),
+        ({"num_nodes": 2, "ranks_per_node": 1}, None),
+        ({"launcher_options": "--debug_foo"}, None),
+        ({"num_nodes": 2, "BAD_OPT": 1}, InvalidResourceSpecification),
+        ({}, None),
     )
 )
-def test_resource_spec(resource_spec: Dict, is_mpi_enabled: bool, exception):
+def test_resource_spec(resource_spec: Dict, exception):
     if exception:
         with pytest.raises(exception):
-            validate_resource_spec(resource_spec, is_mpi_enabled)
+            validate_resource_spec(resource_spec)
     else:
-        result = validate_resource_spec(resource_spec, is_mpi_enabled)
+        result = validate_resource_spec(resource_spec)
         assert result is None
```

### Comparing `parsl-2024.5.27/parsl/tests/test_providers/test_local_provider.py` & `parsl-2024.5.6/parsl/tests/test_providers/test_local_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_providers/test_pbspro_template.py` & `parsl-2024.5.6/parsl/tests/test_providers/test_pbspro_template.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_providers/test_slurm_template.py` & `parsl-2024.5.6/parsl/tests/test_providers/test_slurm_template.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_arg_input_types.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_arg_input_types.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_basic.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_context_manager.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_context_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,22 +11,30 @@
 
 
 @parsl.bash_app
 def foo(x, stdout='foo.stdout'):
     return f"echo {x + 1}"
 
 
+def local_setup():
+    pass
+
+
+def local_teardown():
+    parsl.clear()
+
+
 @pytest.mark.local
 def test_within_context_manger(tmpd_cwd):
     config = fresh_config()
     with parsl.load(config=config) as dfk:
         assert isinstance(dfk, DataFlowKernel)
 
         bash_future = foo(1, stdout=tmpd_cwd / 'foo.stdout')
         assert bash_future.result() == 0
 
         with open(tmpd_cwd / 'foo.stdout', 'r') as f:
             assert f.read() == "2\n"
 
     with pytest.raises(NoDataFlowKernelError) as excinfo:
         square(2).result()
-    assert str(excinfo.value) == "Must first load config"
+    assert str(excinfo.value) == "Cannot submit to a DFK that has been cleaned up"
```

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_dep_standard_futures.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_dep_standard_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_depfail_propagation.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_depfail_propagation.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_fail.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_fibonacci_iterative.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_fibonacci_iterative.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_fibonacci_recursive.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_fibonacci_recursive.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_futures.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_garbage_collect.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_garbage_collect.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_import_fail.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_import_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_join.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_join.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_lifted.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_lifted.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 import pytest
 
 from concurrent.futures import Future
 from parsl import python_app
 
-from typing import TypeVar
-
-T = TypeVar('T')
-
 
 @python_app
-def returns_a_dict() -> dict:
+def returns_a_dict():
     return {"a": "X", "b": "Y"}
 
 
 @python_app
-def returns_a_list() -> list:
+def returns_a_list():
     return ["X", "Y"]
 
 
 @python_app
-def returns_a_tuple() -> tuple:
+def returns_a_tuple():
     return ("X", "Y")
 
 
 @python_app
-def returns_a_class() -> type:
+def returns_a_class():
     from dataclasses import dataclass
 
     @dataclass
     class MyClass:
         a: str = "X"
         b: str = "Y"
 
@@ -38,15 +34,15 @@
 class MyOuterClass():
     def __init__(self):
         self.q = "A"
         self.r = "B"
 
 
 @python_app
-def returns_a_class_instance() -> object:
+def returns_a_class_instance():
     return MyOuterClass()
 
 
 def test_returns_a_dict():
 
     # precondition that returns_a_dict behaves
     # correctly
@@ -110,15 +106,15 @@
     assert returns_a_class().a.result() == "X"
 
     # when the result is not indexable, a sensible error should
     # appear in the appropriate future
 
 
 @python_app
-def passthrough(v: T) -> T:
+def passthrough(v):
     return v
 
 
 def test_lifted_getitem_ordering():
     # this should test that lifting getitem has the correct execution
     # order: that it does not defer the execution of following code
```

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_mapred.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_mapred.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_memoize_1.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_memoize_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_memoize_2.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_memoize_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_memoize_4.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_memoize_4.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_memoize_ignore_args.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_outputs.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_outputs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_pipeline.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_simple.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_timeout.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_timeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_python_apps/test_type5.py` & `parsl-2024.5.6/parsl/tests/test_python_apps/test_type5.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_radical/test_mpi_funcs.py` & `parsl-2024.5.6/parsl/tests/test_radical/test_mpi_funcs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_regression/test_1480.py` & `parsl-2024.5.6/parsl/tests/test_regression/test_1480.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py` & `parsl-2024.5.6/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_regression/test_1653.py` & `parsl-2024.5.6/parsl/tests/test_regression/test_1653.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_regression/test_221.py` & `parsl-2024.5.6/parsl/tests/test_regression/test_221.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_regression/test_226.py` & `parsl-2024.5.6/parsl/tests/test_regression/test_226.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_regression/test_2652.py` & `parsl-2024.5.6/parsl/tests/test_regression/test_2652.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_regression/test_69a.py` & `parsl-2024.5.6/parsl/tests/test_regression/test_69a.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_regression/test_854.py` & `parsl-2024.5.6/parsl/tests/test_regression/test_854.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_regression/test_97_parallelism_0.py` & `parsl-2024.5.6/parsl/tests/test_regression/test_97_parallelism_0.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_scaling/test_block_error_handler.py` & `parsl-2024.5.6/parsl/tests/test_scaling/test_block_error_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_scaling/test_regression_1621.py` & `parsl-2024.5.6/parsl/tests/test_scaling/test_regression_1621.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,8 +65,10 @@
         strategy='simple',
         strategy_period=0.1
     )
 
     with parsl.load(config):
         app().result()
 
+    parsl.clear()
+
     assert oneshot_provider.recorded_submits == 1
```

### Comparing `parsl-2024.5.27/parsl/tests/test_scaling/test_scale_down.py` & `parsl-2024.5.6/parsl/tests/test_scaling/test_scale_down.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py` & `parsl-2024.5.6/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_scaling/test_scale_down_htex_unregistered.py` & `parsl-2024.5.6/parsl/tests/test_scaling/test_scale_down_htex_unregistered.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_scaling/test_shutdown_scalein.py` & `parsl-2024.5.6/parsl/tests/test_scaling/test_shutdown_scalein.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,9 +68,11 @@
         run_dir=str(tmpd_cwd)
     )
 
     with parsl.load(config):
         # this will wait for everything to be scaled out fully
         try_assert(lambda: len(htex.connected_managers()) == BLOCK_COUNT)
 
+    parsl.clear()
+
     assert len(accumulating_provider.submit_job_ids) == BLOCK_COUNT, f"Exactly {BLOCK_COUNT} blocks should have been launched"
     assert len(accumulating_provider.cancel_job_ids) == BLOCK_COUNT, f"Exactly {BLOCK_COUNT} blocks should have been scaled in"
```

### Comparing `parsl-2024.5.27/parsl/tests/test_serialization/test_2555_caching_deserializer.py` & `parsl-2024.5.6/parsl/tests/test_serialization/test_2555_caching_deserializer.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_serialization/test_basic.py` & `parsl-2024.5.6/parsl/tests/test_serialization/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_serialization/test_htex_code_cache.py` & `parsl-2024.5.6/parsl/tests/test_serialization/test_htex_code_cache.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_serialization/test_pack_resource_spec.py` & `parsl-2024.5.6/parsl/tests/test_serialization/test_pack_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_serialization/test_proxystore_configured.py` & `parsl-2024.5.6/parsl/tests/test_serialization/test_proxystore_configured.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
     register_method_for_data(s)
     logger.info(f"BENC: methods for data: {methods_for_data}")
 
 
 def local_teardown():
     parsl.dfk().cleanup()
+    parsl.clear()
 
     methods_for_data.clear()
     methods_for_data.update(previous_methods)
 
     additional_methods_for_deserialization.clear()
```

### Comparing `parsl-2024.5.27/parsl/tests/test_serialization/test_proxystore_impl.py` & `parsl-2024.5.6/parsl/tests/test_serialization/test_proxystore_impl.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_shutdown/test_kill_monitoring.py` & `parsl-2024.5.6/parsl/tests/test_shutdown/test_kill_monitoring.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     """This tests that we can create a monitoring-enabled DFK and shut it down."""
 
     parsl.load(fresh_config())
 
     assert parsl.dfk().monitoring is not None, "This test requires monitoring"
 
     parsl.dfk().cleanup()
+    parsl.clear()
 
 
 @pytest.mark.local
 @pytest.mark.parametrize("sig", [signal.SIGINT, signal.SIGTERM, signal.SIGKILL, signal.SIGQUIT])
 @pytest.mark.parametrize("process_attr", ["router_proc", "dbm_proc"])
 def test_kill_monitoring_helper_process(sig, process_attr, try_assert):
     """This tests that we can kill a monitoring process and still have successful shutdown.
@@ -57,7 +58,8 @@
 
     # now we have broken one piece of the monitoring system, do some app
     # execution and then shut down.
 
     simple_app().result()
 
     parsl.dfk().cleanup()
+    parsl.clear()
```

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/staging_provider.py` & `parsl-2024.5.6/parsl/tests/test_staging/staging_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_1316.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_1316.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     p = observe_input_local_path(file).result()
 
     assert p == "./test1.tmp", "File object on the execution side gets the local_path set by the staging provider"
 
     assert not file.local_path, "The local_path on the submit side should not be set"
 
     parsl.dfk().cleanup()
+    parsl.clear()
 
 
 @pytest.mark.local
 def test_1316_local_path_setting_preserves_dependency_sp2():
     config = Config(executors=[ThreadPoolExecutor(storage_access=[SP2()])])
 
     file = File("sp2://test")
@@ -78,7 +79,8 @@
     assert wc_app_future.done(), "wait_and_create should finish before observe_input_local_path finishes"
 
     assert p == "./test1.tmp", "File object on the execution side gets the local_path set by the staging provider"
 
     assert not file.local_path, "The local_path on the submit side should not be set"
 
     parsl.dfk().cleanup()
+    parsl.clear()
```

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_docs_1.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_docs_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_elaborate_noop_file.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_elaborate_noop_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         )
         config = Config(executors=[tpe])
         parsl.load(config)
 
     yield _setup_config
 
     parsl.dfk().cleanup()
+    parsl.clear()
 
 
 @pytest.mark.local
 def test_regression_stage_out_does_not_stage_in(storage_access_parsl, tmpd_cwd):
     storage_access_parsl(allow_stage_in=False)
 
     # Test that the helper app runs with no staging
```

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_file.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_file_apps.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_file_apps.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_file_staging.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_file_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_output_chain_filenames.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_output_chain_filenames.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_staging_ftp.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_staging_ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_staging_ftp_in_task.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_staging_ftp_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_staging_globus.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_staging_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_staging_https.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_staging_https.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_staging_stdout.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_staging_stdout.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_zip_in.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_zip_in.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_zip_out.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_zip_out.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_staging/test_zip_to_zip.py` & `parsl-2024.5.6/parsl/tests/test_staging/test_zip_to_zip.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_summary.py` & `parsl-2024.5.6/parsl/tests/test_summary.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 
     parsl.load(fresh_config())
 
     succeed().result()
     fail().exception()
 
     parsl.dfk().cleanup()
+    parsl.clear()
 
     assert "Summary of tasks in DFK:" in caplog.text
     assert "Tasks in state States.exec_done: 1" in caplog.text
     assert "Tasks in state States.failed: 1" in caplog.text
```

### Comparing `parsl-2024.5.27/parsl/tests/test_thread_parallelism.py` & `parsl-2024.5.6/parsl/tests/test_thread_parallelism.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/test_threads/test_configs.py` & `parsl-2024.5.6/parsl/tests/test_threads/test_configs.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,8 +26,9 @@
     [item.result() for item in d]
 
     thread_count = len(set([item.result()['tid'] for item in d]))
     process_count = len(set([item.result()['pid'] for item in d]))
     assert thread_count <= config.executors[0].max_threads, "More threads than allowed"
     assert process_count == 1, "More processes than allowed"
     dfk.cleanup()
+    parsl.clear()
     return d
```

### Comparing `parsl-2024.5.27/parsl/tests/test_threads/test_lazy_errors.py` & `parsl-2024.5.6/parsl/tests/test_threads/test_lazy_errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,8 +20,9 @@
         futures.append(divide(10, 0))
 
     for f in futures:
         assert isinstance(f.exception(), ZeroDivisionError)
         assert f.done()
 
     parsl.dfk().cleanup()
+    parsl.clear()
     return
```

### Comparing `parsl-2024.5.27/parsl/tests/test_utils/test_representation_mixin.py` & `parsl-2024.5.6/parsl/tests/test_utils/test_representation_mixin.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/tests/unit/test_file.py` & `parsl-2024.5.6/parsl/tests/unit/test_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/usage_tracking/api.py` & `parsl-2024.5.6/parsl/usage_tracking/api.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/usage_tracking/usage.py` & `parsl-2024.5.6/parsl/usage_tracking/usage.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl/utils.py` & `parsl-2024.5.6/parsl/utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.5.27/parsl.egg-info/PKG-INFO` & `parsl-2024.5.6/parsl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2024.5.27
+Version: 2024.5.6
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2024.05.27.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2024.05.06.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2024.5.27/parsl.egg-info/SOURCES.txt` & `parsl-2024.5.6/parsl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 parsl/data_provider/ftp.py
 parsl/data_provider/globus.py
 parsl/data_provider/http.py
 parsl/data_provider/rsync.py
 parsl/data_provider/staging.py
 parsl/data_provider/zip.py
 parsl/dataflow/__init__.py
-parsl/dataflow/dependency_resolvers.py
 parsl/dataflow/dflow.py
 parsl/dataflow/errors.py
 parsl/dataflow/futures.py
 parsl/dataflow/memoization.py
 parsl/dataflow/rundirs.py
 parsl/dataflow/states.py
 parsl/dataflow/taskrecord.py
@@ -91,15 +90,14 @@
 parsl/executors/flux/flux_instance_manager.py
 parsl/executors/high_throughput/__init__.py
 parsl/executors/high_throughput/errors.py
 parsl/executors/high_throughput/executor.py
 parsl/executors/high_throughput/interchange.py
 parsl/executors/high_throughput/manager_record.py
 parsl/executors/high_throughput/monitoring_info.py
-parsl/executors/high_throughput/mpi_executor.py
 parsl/executors/high_throughput/mpi_prefix_composer.py
 parsl/executors/high_throughput/mpi_resource_management.py
 parsl/executors/high_throughput/probe.py
 parsl/executors/high_throughput/process_worker_pool.py
 parsl/executors/high_throughput/zmq_pipes.py
 parsl/executors/radical/__init__.py
 parsl/executors/radical/executor.py
@@ -344,22 +342,20 @@
 parsl/tests/test_error_handling/test_retry_handler.py
 parsl/tests/test_error_handling/test_retry_handler_failure.py
 parsl/tests/test_error_handling/test_serialization_fail.py
 parsl/tests/test_error_handling/test_wrap_with_logs.py
 parsl/tests/test_flowcontrol/__init__.py
 parsl/tests/test_htex/__init__.py
 parsl/tests/test_htex/test_basic.py
-parsl/tests/test_htex/test_command_client_timeout.py
 parsl/tests/test_htex/test_connected_blocks.py
 parsl/tests/test_htex/test_cpu_affinity_explicit.py
 parsl/tests/test_htex/test_disconnected_blocks.py
 parsl/tests/test_htex/test_drain.py
 parsl/tests/test_htex/test_htex.py
 parsl/tests/test_htex/test_manager_failure.py
-parsl/tests/test_htex/test_managers_command.py
 parsl/tests/test_htex/test_missing_worker.py
 parsl/tests/test_htex/test_multiple_disconnected_blocks.py
 parsl/tests/test_htex/test_worker_failure.py
 parsl/tests/test_htex/test_zmq_binding.py
 parsl/tests/test_monitoring/__init__.py
 parsl/tests/test_monitoring/test_app_names.py
 parsl/tests/test_monitoring/test_basic.py
@@ -372,15 +368,14 @@
 parsl/tests/test_monitoring/test_viz_colouring.py
 parsl/tests/test_mpi_apps/__init__.py
 parsl/tests/test_mpi_apps/test_bad_mpi_config.py
 parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py
 parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py
 parsl/tests/test_mpi_apps/test_mpi_prefix.py
 parsl/tests/test_mpi_apps/test_mpi_scheduler.py
-parsl/tests/test_mpi_apps/test_mpiex.py
 parsl/tests/test_mpi_apps/test_resource_spec.py
 parsl/tests/test_providers/__init__.py
 parsl/tests/test_providers/test_cobalt_deprecation_warning.py
 parsl/tests/test_providers/test_local_provider.py
 parsl/tests/test_providers/test_pbspro_template.py
 parsl/tests/test_providers/test_slurm_instantiate.py
 parsl/tests/test_providers/test_slurm_template.py
@@ -406,15 +401,14 @@
 parsl/tests/test_python_apps/test_memoize_4.py
 parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
 parsl/tests/test_python_apps/test_memoize_ignore_args.py
 parsl/tests/test_python_apps/test_memoize_joinapp.py
 parsl/tests/test_python_apps/test_outputs.py
 parsl/tests/test_python_apps/test_overview.py
 parsl/tests/test_python_apps/test_pipeline.py
-parsl/tests/test_python_apps/test_pluggable_future_resolution.py
 parsl/tests/test_python_apps/test_simple.py
 parsl/tests/test_python_apps/test_timeout.py
 parsl/tests/test_python_apps/test_type5.py
 parsl/tests/test_radical/__init__.py
 parsl/tests/test_radical/test_mpi_funcs.py
 parsl/tests/test_regression/__init__.py
 parsl/tests/test_regression/test_1480.py
```

### Comparing `parsl-2024.5.27/parsl.egg-info/requires.txt` & `parsl-2024.5.6/parsl.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 azure<=4
 msrestazure
 work_queue
 pyyaml
 cffi
 jsonschema
 proxystore
-radical.pilot==1.60
-radical.utils==1.60
+radical.pilot==1.52.1
 
 [aws]
 boto3
 
 [azure]
 azure<=4
 msrestazure
@@ -73,16 +72,15 @@
 [oauth_ssh]
 oauth-ssh>=0.9
 
 [proxystore]
 proxystore
 
 [radical-pilot]
-radical.pilot==1.60
-radical.utils==1.60
+radical.pilot==1.52.1
 
 [visualization]
 pydot
 networkx<2.6,>=2.5
 Flask>=1.0.2
 flask_sqlalchemy
 pandas<2.2
```

### Comparing `parsl-2024.5.27/setup.py` & `parsl-2024.5.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     ],
     'google_cloud' : ['google-auth', 'google-api-python-client'],
     'gssapi' : ['python-gssapi'],
     'azure' : ['azure<=4', 'msrestazure'],
     'workqueue': ['work_queue'],
     'flux': ['pyyaml', 'cffi', 'jsonschema'],
     'proxystore': ['proxystore'],
-    'radical-pilot': ['radical.pilot==1.60', 'radical.utils==1.60'],
+    'radical-pilot': ['radical.pilot==1.52.1'],
     # Disabling psi-j since github direct links are not allowed by pypi
     # 'psij': ['psi-j-parsl@git+https://github.com/ExaWorks/psi-j-parsl']
 }
 extras_require['all'] = sum(extras_require.values(), [])
 
 setup(
     name='parsl',
```

