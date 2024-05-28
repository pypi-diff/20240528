# Comparing `tmp/reframe_hpc-4.6.0.tar.gz` & `tmp/reframe_hpc-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reframe_hpc-4.6.0.tar", last modified: Sat Apr 20 17:40:59 2024, max compression
+gzip compressed data, was "reframe_hpc-4.6.1.tar", last modified: Tue May 28 20:34:05 2024, max compression
```

## Comparing `reframe_hpc-4.6.0.tar` & `reframe_hpc-4.6.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/README_minimal.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/ReFrame_HPC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-20 17:40:59.000000 reframe_hpc-4.6.0/ReFrame_HPC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-20 17:40:59.000000 reframe_hpc-4.6.0/ReFrame_HPC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:40:59.000000 reframe_hpc-4.6.0/ReFrame_HPC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-20 17:40:59.000000 reframe_hpc-4.6.0/ReFrame_HPC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 17:40:59.000000 reframe_hpc-4.6.0/ReFrame_HPC.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/bin/reframe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/data_analytics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/data_analytics/spark/
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/data_analytics/spark/spark_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/data_analytics/spark/src/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/data_analytics/spark/src/spark_pi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/interactive/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/interactive/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/interactive/jupyter/ipcmagic/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/interactive/jupyter/ipcmagic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/dgemm/
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/dgemm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/gpu_burn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/kernel_latency/
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/kernel_latency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/memory_bandwidth/
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/memory_bandwidth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/pointer_chase/
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/pointer_chase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.167196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/shmem/
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/shmem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/microbenchmarks/mpi/osu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/ml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/ml/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/ml/pytorch/horovod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/ml/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/ml/tensorflow/horovod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/python/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/python/numpy/numpy_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/python/numpy/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/python/numpy/src/np_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/sciapps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/sciapps/amber/
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/sciapps/amber/nve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/sciapps/gromacs/
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/sciapps/gromacs/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/sciapps/qespresso/
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/sciapps/qespresso/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.163196 reframe_hpc-4.6.0/hpctestlib/system/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/system/fs/
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/system/fs/mnt_opts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/hpctestlib/system/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/hpctestlib/system/ssh/host_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.171196 reframe_hpc-4.6.0/reframe/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.175196 reframe_hpc-4.6.0/reframe/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)    32254 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/buildsystems.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    24544 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/deferrable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    44509 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.179196 reframe_hpc-4.6.0/reframe/core/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/launchers/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/launchers/mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/launchers/rsh.py
--rw-r--r--   0 runner    (1001) docker     (127)    34616 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    36668 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    38767 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    16460 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    95804 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    14317 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.179196 reframe_hpc-4.6.0/reframe/core/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)    21040 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/oar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/sge.py
--rw-r--r--   0 runner    (1001) docker     (127)    26548 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/schedulers/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)    23494 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/systems.py
--rw-r--r--   0 runner    (1001) docker     (127)    32104 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/core/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/reframe/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/autodetect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/ci.py
--rw-r--r--   0 runner    (1001) docker     (127)    58260 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/reframe/frontend/executors/
--rw-r--r--   0 runner    (1001) docker     (127)    21499 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/executors/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/runreport.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/frontend/testgenerators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/reframe/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    26802 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/schemas/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/schemas/junit.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/schemas/runreport.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/reframe/utility/
--rw-r--r--   0 runner    (1001) docker     (127)    50528 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/color.py
--rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/cpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/jsonext.py
--rw-r--r--   0 runner    (1001) docker     (127)    28585 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/osext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    32327 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/sanity.py
--rw-r--r--   0 runner    (1001) docker     (127)    14696 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/udeps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-20 17:40:53.000000 reframe_hpc-4.6.0/reframe/utility/versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-20 17:40:59.183196 reframe_hpc-4.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.418746 reframe_hpc-4.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-05-28 20:34:05.418746 reframe_hpc-4.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/README_minimal.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.418746 reframe_hpc-4.6.1/ReFrame_HPC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-05-28 20:34:05.000000 reframe_hpc-4.6.1/ReFrame_HPC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-28 20:34:05.000000 reframe_hpc-4.6.1/ReFrame_HPC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:34:05.000000 reframe_hpc-4.6.1/ReFrame_HPC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:34:05.000000 reframe_hpc-4.6.1/ReFrame_HPC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 20:34:05.000000 reframe_hpc-4.6.1/ReFrame_HPC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.402746 reframe_hpc-4.6.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/bin/reframe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.398746 reframe_hpc-4.6.1/hpctestlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.394745 reframe_hpc-4.6.1/hpctestlib/data_analytics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.402746 reframe_hpc-4.6.1/hpctestlib/data_analytics/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/data_analytics/spark/spark_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.402746 reframe_hpc-4.6.1/hpctestlib/data_analytics/spark/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/data_analytics/spark/src/spark_pi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.398746 reframe_hpc-4.6.1/hpctestlib/interactive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.398746 reframe_hpc-4.6.1/hpctestlib/interactive/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.402746 reframe_hpc-4.6.1/hpctestlib/interactive/jupyter/ipcmagic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/interactive/jupyter/ipcmagic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.398746 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.402746 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.402746 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/dgemm/
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/dgemm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/gpu_burn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.402746 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/kernel_latency/
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/kernel_latency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.402746 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/memory_bandwidth/
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/memory_bandwidth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/pointer_chase/
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/pointer_chase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/shmem/
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/shmem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/microbenchmarks/mpi/osu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.398746 reframe_hpc-4.6.1/hpctestlib/ml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/hpctestlib/ml/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/ml/pytorch/horovod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/hpctestlib/ml/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/ml/tensorflow/horovod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.398746 reframe_hpc-4.6.1/hpctestlib/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/hpctestlib/python/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/python/numpy/numpy_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/hpctestlib/python/numpy/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/python/numpy/src/np_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.398746 reframe_hpc-4.6.1/hpctestlib/sciapps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/hpctestlib/sciapps/amber/
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/sciapps/amber/nve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/hpctestlib/sciapps/gromacs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/sciapps/gromacs/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/hpctestlib/sciapps/qespresso/
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/sciapps/qespresso/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.398746 reframe_hpc-4.6.1/hpctestlib/system/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/hpctestlib/system/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/system/fs/mnt_opts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/hpctestlib/system/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/hpctestlib/system/ssh/host_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.406746 reframe_hpc-4.6.1/reframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.410746 reframe_hpc-4.6.1/reframe/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32254 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/buildsystems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24544 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/deferrable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44509 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.410746 reframe_hpc-4.6.1/reframe/core/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/launchers/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/launchers/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/launchers/rsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34801 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36668 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38767 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16460 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95804 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14317 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.414746 reframe_hpc-4.6.1/reframe/core/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)    21040 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/schedulers/flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/schedulers/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/schedulers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/schedulers/oar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/schedulers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/schedulers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/schedulers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26697 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/schedulers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/schedulers/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23494 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32104 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/core/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.414746 reframe_hpc-4.6.1/reframe/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/autodetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58194 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.418746 reframe_hpc-4.6.1/reframe/frontend/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)    21499 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/executors/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/runreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/frontend/testgenerators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.418746 reframe_hpc-4.6.1/reframe/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    26802 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/schemas/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/schemas/junit.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/schemas/runreport.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:05.418746 reframe_hpc-4.6.1/reframe/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)    50528 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/utility/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/utility/cpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/utility/jsonext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28624 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/utility/osext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/utility/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32327 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/utility/sanity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14696 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/utility/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/utility/udeps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-28 20:33:53.000000 reframe_hpc-4.6.1/reframe/utility/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-28 20:34:05.418746 reframe_hpc-4.6.1/setup.cfg
```

### Comparing `reframe_hpc-4.6.0/LICENSE` & `reframe_hpc-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/PKG-INFO` & `reframe_hpc-4.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.6.0
+Version: 4.6.1
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `reframe_hpc-4.6.0/README.md` & `reframe_hpc-4.6.1/README.md`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/README_minimal.md` & `reframe_hpc-4.6.1/README_minimal.md`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/ReFrame_HPC.egg-info/PKG-INFO` & `reframe_hpc-4.6.1/ReFrame_HPC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.6.0
+Version: 4.6.1
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `reframe_hpc-4.6.0/ReFrame_HPC.egg-info/SOURCES.txt` & `reframe_hpc-4.6.1/ReFrame_HPC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/bin/reframe` & `reframe_hpc-4.6.1/bin/reframe`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/data_analytics/spark/spark_checks.py` & `reframe_hpc-4.6.1/hpctestlib/data_analytics/spark/spark_checks.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/interactive/jupyter/ipcmagic/__init__.py` & `reframe_hpc-4.6.1/hpctestlib/interactive/jupyter/ipcmagic/__init__.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/dgemm/__init__.py` & `reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/dgemm/__init__.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/gpu_burn.py` & `reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/gpu_burn.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/kernel_latency/__init__.py` & `reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/kernel_latency/__init__.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/memory_bandwidth/__init__.py` & `reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/memory_bandwidth/__init__.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/pointer_chase/__init__.py` & `reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/pointer_chase/__init__.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/gpu/shmem/__init__.py` & `reframe_hpc-4.6.1/hpctestlib/microbenchmarks/gpu/shmem/__init__.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/microbenchmarks/mpi/osu.py` & `reframe_hpc-4.6.1/hpctestlib/microbenchmarks/mpi/osu.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/ml/pytorch/horovod.py` & `reframe_hpc-4.6.1/hpctestlib/ml/pytorch/horovod.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/ml/tensorflow/horovod.py` & `reframe_hpc-4.6.1/hpctestlib/ml/tensorflow/horovod.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/python/numpy/numpy_ops.py` & `reframe_hpc-4.6.1/hpctestlib/python/numpy/numpy_ops.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/python/numpy/src/np_ops.py` & `reframe_hpc-4.6.1/hpctestlib/python/numpy/src/np_ops.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/sciapps/amber/nve.py` & `reframe_hpc-4.6.1/hpctestlib/sciapps/amber/nve.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/sciapps/gromacs/benchmarks.py` & `reframe_hpc-4.6.1/hpctestlib/sciapps/gromacs/benchmarks.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/sciapps/qespresso/benchmarks.py` & `reframe_hpc-4.6.1/hpctestlib/sciapps/qespresso/benchmarks.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/system/fs/mnt_opts.py` & `reframe_hpc-4.6.1/hpctestlib/system/fs/mnt_opts.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/hpctestlib/system/ssh/host_keys.py` & `reframe_hpc-4.6.1/hpctestlib/system/ssh/host_keys.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/__init__.py` & `reframe_hpc-4.6.1/reframe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ReFrame Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import os
 import sys
 
-VERSION = '4.6.0'
+VERSION = '4.6.1'
 INSTALL_PREFIX = os.path.normpath(
     os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 )
 MIN_PYTHON_VERSION = (3, 6, 0)
 
 # Check python version
 if sys.version_info[:3] < MIN_PYTHON_VERSION:
```

### Comparing `reframe_hpc-4.6.0/reframe/core/backends.py` & `reframe_hpc-4.6.1/reframe/core/backends.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/buildsystems.py` & `reframe_hpc-4.6.1/reframe/core/buildsystems.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/builtins.py` & `reframe_hpc-4.6.1/reframe/core/builtins.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/config.py` & `reframe_hpc-4.6.1/reframe/core/config.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/containers.py` & `reframe_hpc-4.6.1/reframe/core/containers.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/decorators.py` & `reframe_hpc-4.6.1/reframe/core/decorators.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/deferrable.py` & `reframe_hpc-4.6.1/reframe/core/deferrable.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/environments.py` & `reframe_hpc-4.6.1/reframe/core/environments.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/exceptions.py` & `reframe_hpc-4.6.1/reframe/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/fields.py` & `reframe_hpc-4.6.1/reframe/core/fields.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/fixtures.py` & `reframe_hpc-4.6.1/reframe/core/fixtures.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/hooks.py` & `reframe_hpc-4.6.1/reframe/core/hooks.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/launchers/__init__.py` & `reframe_hpc-4.6.1/reframe/core/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/launchers/local.py` & `reframe_hpc-4.6.1/reframe/core/launchers/local.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/launchers/mpi.py` & `reframe_hpc-4.6.1/reframe/core/launchers/mpi.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/launchers/rsh.py` & `reframe_hpc-4.6.1/reframe/core/launchers/rsh.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/logging.py` & `reframe_hpc-4.6.1/reframe/core/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
         # Associates filenames with open streams
         self.__streams = {}
 
         # Format specifiers
         self.__fmt = fmt
         self.__perffmt = perffmt
-        self.__attr_patt = re.compile(r'\%\((.*?)\)s(.)?')
+        self.__attr_patt = re.compile(r'\%\((.*?)\)s(.*?(?=%|$))?')
         self.__ignore_keys = set(ignore_keys) if ignore_keys else set()
 
     def __generate_header(self, record):
         # Generate the header from the record and fmt
 
         # Expand the special check_#ALL specifier
         if '%(check_#ALL)s' in self.__fmt:
@@ -297,15 +297,19 @@
 class CheckFieldFormatter(logging.Formatter):
     '''Log formatter that dynamically looks up format specifiers inside a
     regression test.'''
 
     # NOTE: This formatter will work only for the '%' style
     def __init__(self, fmt=None, datefmt=None, perffmt=None,
                  ignore_keys=None, style='%'):
-        super().__init__(fmt, datefmt, style)
+        if sys.version_info[:2] <= (3, 7):
+            super().__init__(fmt, datefmt, style)
+        else:
+            super().__init__(fmt, datefmt, style,
+                             validate=(fmt != '%(check_#ALL)s'))
 
         self.__fmt = fmt
         self.__fmtperf = perffmt[:-1] if perffmt else ''
         self.__specs = re.findall(r'\%\((\S+?)\)s', fmt)
         self.__delim = perffmt[-1] if perffmt else ''
         self.__expand_vars = '%(check_#ALL)s' in self.__fmt
         self.__expanded_fmt = {}
```

### Comparing `reframe_hpc-4.6.0/reframe/core/meta.py` & `reframe_hpc-4.6.1/reframe/core/meta.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/modules.py` & `reframe_hpc-4.6.1/reframe/core/modules.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/namespaces.py` & `reframe_hpc-4.6.1/reframe/core/namespaces.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/parameters.py` & `reframe_hpc-4.6.1/reframe/core/parameters.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/pipeline.py` & `reframe_hpc-4.6.1/reframe/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/runtime.py` & `reframe_hpc-4.6.1/reframe/core/runtime.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/schedulers/__init__.py` & `reframe_hpc-4.6.1/reframe/core/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/schedulers/flux.py` & `reframe_hpc-4.6.1/reframe/core/schedulers/flux.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/schedulers/local.py` & `reframe_hpc-4.6.1/reframe/core/schedulers/local.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/schedulers/lsf.py` & `reframe_hpc-4.6.1/reframe/core/schedulers/lsf.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/schedulers/oar.py` & `reframe_hpc-4.6.1/reframe/core/schedulers/oar.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/schedulers/pbs.py` & `reframe_hpc-4.6.1/reframe/core/schedulers/pbs.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/schedulers/registry.py` & `reframe_hpc-4.6.1/reframe/core/schedulers/registry.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/schedulers/sge.py` & `reframe_hpc-4.6.1/reframe/core/schedulers/sge.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/schedulers/slurm.py` & `reframe_hpc-4.6.1/reframe/core/schedulers/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -617,14 +617,17 @@
                 job_match = jobinfo[job.jobid]
             except KeyError:
                 job._state = 'CANCELLED' if job.is_cancelling else 'COMPLETED'
                 continue
 
             # Join the states with ',' in case of job arrays
             job._state = ','.join(s.group('state') for s in job_match)
+
+            # Use ',' to join nodes to be consistent with Slurm syntax
+            job._nodespec = ','.join(m.group('nodespec') for m in job_match)
             self._cancel_if_blocked(
                 job, [s.group('reason') for s in state_match]
             )
             self._cancel_if_pending_too_long(job)
 
 
 def _create_nodes(descriptions):
```

### Comparing `reframe_hpc-4.6.0/reframe/core/schedulers/ssh.py` & `reframe_hpc-4.6.1/reframe/core/schedulers/ssh.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/settings.py` & `reframe_hpc-4.6.1/reframe/core/settings.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/shell.py` & `reframe_hpc-4.6.1/reframe/core/shell.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/systems.py` & `reframe_hpc-4.6.1/reframe/core/systems.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/variables.py` & `reframe_hpc-4.6.1/reframe/core/variables.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/core/warnings.py` & `reframe_hpc-4.6.1/reframe/core/warnings.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/frontend/argparse.py` & `reframe_hpc-4.6.1/reframe/frontend/argparse.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/frontend/autodetect.py` & `reframe_hpc-4.6.1/reframe/frontend/autodetect.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/frontend/ci.py` & `reframe_hpc-4.6.1/reframe/frontend/ci.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/frontend/cli.py` & `reframe_hpc-4.6.1/reframe/frontend/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
     )
     output_options.add_argument(
         '-s', '--stage', action='store', metavar='DIR',
         help='Set stage directory prefix to DIR',
         envvar='RFM_STAGE_DIR', configvar='systems/stagedir'
     )
     output_options.add_argument(
-        '--save-log-files', action='store_true', default=False,
+        '--save-log-files', action='store_true',
         help='Save ReFrame log files to the output directory',
         envvar='RFM_SAVE_LOG_FILES', configvar='general/save_log_files'
     )
     output_options.add_argument(
         '--timestamp', action='store', nargs='?', const='%y%m%dT%H%M%S%z',
         metavar='TIMEFMT',
         help=('Append a timestamp to the output and stage directory prefixes '
@@ -470,20 +470,20 @@
         '--skip-system-check', action='store_true',
         help='Skip system check'
     )
 
     # Environment options
     env_options.add_argument(
         '-M', '--map-module', action='append', metavar='MAPPING',
-        dest='module_mappings', default=[],
+        dest='module_mappings',
         help='Add a module mapping',
         envvar='RFM_MODULE_MAPPINGS ,', configvar='general/module_mappings'
     )
     env_options.add_argument(
-        '-m', '--module', action='append', default=[],
+        '-m', '--module', action='append',
         metavar='MOD', dest='user_modules',
         help='Load module MOD before running any regression check',
         envvar='RFM_USER_MODULES ,', configvar='general/user_modules'
     )
     env_options.add_argument(
         '--module-mappings', action='store', metavar='FILE',
         dest='module_map_file',
@@ -497,21 +497,21 @@
     )
     env_options.add_argument(
         '--non-default-craype', action='store_true',
         help='Test a non-default Cray Programming Environment',
         envvar='RFM_NON_DEFAULT_CRAYPE', configvar='general/non_default_craype'
     )
     env_options.add_argument(
-        '--purge-env', action='store_true', dest='purge_env', default=False,
+        '--purge-env', action='store_true', dest='purge_env',
         help='Unload all modules before running any regression check',
         envvar='RFM_PURGE_ENVIRONMENT', configvar='general/purge_environment'
     )
     env_options.add_argument(
         '-u', '--unload-module', action='append', metavar='MOD',
-        dest='unload_modules', default=[],
+        dest='unload_modules',
         help='Unload module MOD before running any regression check',
         envvar='RFM_UNLOAD_MODULES ,', configvar='general/unload_modules'
     )
 
     # Test generation options
     testgen_options.add_argument(
         '--distribute', action='store', metavar='{all|avail|STATE}',
```

### Comparing `reframe_hpc-4.6.0/reframe/frontend/dependencies.py` & `reframe_hpc-4.6.1/reframe/frontend/dependencies.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/frontend/executors/__init__.py` & `reframe_hpc-4.6.1/reframe/frontend/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/frontend/executors/policies.py` & `reframe_hpc-4.6.1/reframe/frontend/executors/policies.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/frontend/filters.py` & `reframe_hpc-4.6.1/reframe/frontend/filters.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/frontend/loader.py` & `reframe_hpc-4.6.1/reframe/frontend/loader.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/frontend/printer.py` & `reframe_hpc-4.6.1/reframe/frontend/printer.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/frontend/runreport.py` & `reframe_hpc-4.6.1/reframe/frontend/runreport.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/frontend/statistics.py` & `reframe_hpc-4.6.1/reframe/frontend/statistics.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/frontend/testgenerators.py` & `reframe_hpc-4.6.1/reframe/frontend/testgenerators.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/schemas/config.json` & `reframe_hpc-4.6.1/reframe/schemas/config.json`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/schemas/junit.xsd` & `reframe_hpc-4.6.1/reframe/schemas/junit.xsd`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/schemas/runreport.json` & `reframe_hpc-4.6.1/reframe/schemas/runreport.json`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/utility/__init__.py` & `reframe_hpc-4.6.1/reframe/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/utility/color.py` & `reframe_hpc-4.6.1/reframe/utility/color.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/utility/cpuinfo.py` & `reframe_hpc-4.6.1/reframe/utility/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/utility/jsonext.py` & `reframe_hpc-4.6.1/reframe/utility/jsonext.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/utility/osext.py` & `reframe_hpc-4.6.1/reframe/utility/osext.py`

 * *Files 2% similar despite different names*

```diff
@@ -688,35 +688,34 @@
                     timeout=timeout)
     except (SpawnedProcessTimeout, SpawnedProcessError):
         return False
     else:
         return True
 
 
-def git_repo_hash(commit='HEAD', short=True, wd=None):
+def git_repo_hash(commit='HEAD', short=True, wd='.'):
     '''Return the SHA1 hash of a Git commit.
 
     :arg commit: The commit to look at.
     :arg short: Return a short hash. This always corresponds to the first 8
         characters of the long hash. We don't rely on Git for the short hash,
         since depending on the version it might return either 7 or 8
         characters.
-    :arg wd: Change to this directory before retrieving the hash. If ``None``,
-        ReFrame's install prefix will be used.
+    :arg wd: Change to this directory before retrieving the hash.
     :returns: The Git commit hash or ``None`` if the hash could not be
         retrieved.
+
+    .. versionchanged:: 4.6.1
+       Default working directory is now ``.``.
     '''
     try:
-        wd = wd or reframe.INSTALL_PREFIX
-        with change_dir(wd):
-            # Do not log this command, since we need to call this function
-            # from the logger
-            completed = run_command(f'git rev-parse {commit}',
-                                    check=True, log=False)
-
+        # Do not log this command, since we need to call this function
+        # from the logger
+        completed = run_command(f'git -C {wd} rev-parse {commit}',
+                                check=True, log=False)
     except (SpawnedProcessError, FileNotFoundError):
         return None
 
     hash = completed.stdout.strip()
     if hash:
         return hash[:8] if short else hash
     else:
@@ -726,21 +725,22 @@
 @util.cache_return_value
 def reframe_version():
     '''Return ReFrame version.
 
     If ReFrame's installation contains the repository metadata and the current
     version is a pre-release version, the repository's hash will be appended
     to the actual version.
-
     '''
-    repo_hash = git_repo_hash()
-    if repo_hash and semver.VersionInfo.parse(reframe.VERSION).prerelease:
-        return f'{reframe.VERSION}+{repo_hash}'
-    else:
-        return reframe.VERSION
+    if (semver.VersionInfo.parse(reframe.VERSION).prerelease and
+        os.path.exists(os.path.join(reframe.INSTALL_PREFIX, '.git'))):
+        repo_hash = git_repo_hash(wd=reframe.INSTALL_PREFIX)
+        if repo_hash:
+            return f'{reframe.VERSION}+{repo_hash}'
+
+    return reframe.VERSION
 
 
 def expandvars(s):
     '''Expand environment variables in ``s`` and perform any command
     substitution.
 
     This function is the same as :py:func:`os.path.expandvars`, except that it
```

### Comparing `reframe_hpc-4.6.0/reframe/utility/profile.py` & `reframe_hpc-4.6.1/reframe/utility/profile.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/utility/sanity.py` & `reframe_hpc-4.6.1/reframe/utility/sanity.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/utility/typecheck.py` & `reframe_hpc-4.6.1/reframe/utility/typecheck.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/utility/udeps.py` & `reframe_hpc-4.6.1/reframe/utility/udeps.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/reframe/utility/versioning.py` & `reframe_hpc-4.6.1/reframe/utility/versioning.py`

 * *Files identical despite different names*

### Comparing `reframe_hpc-4.6.0/setup.cfg` & `reframe_hpc-4.6.1/setup.cfg`

 * *Files identical despite different names*

