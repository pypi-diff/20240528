# Comparing `tmp/amaze-benchmarker-1.0rc0.post1.tar.gz` & `tmp/amaze_benchmarker-1.0rc0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amaze-benchmarker-1.0rc0.post1.tar", last modified: Fri Mar 22 07:41:38 2024, max compression
+gzip compressed data, was "amaze_benchmarker-1.0rc0.post2.tar", last modified: Tue May 28 04:53:19 2024, max compression
```

## Comparing `amaze-benchmarker-1.0rc0.post1.tar` & `amaze_benchmarker-1.0rc0.post2.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.510860 amaze-benchmarker-1.0rc0.post1/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     3315 2024-02-29 07:33:48.000000 amaze-benchmarker-1.0rc0.post1/.gitignore
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      272 2024-03-07 10:02:48.000000 amaze-benchmarker-1.0rc0.post1/.readthedocs.yaml
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     1075 2023-06-01 09:12:37.000000 amaze-benchmarker-1.0rc0.post1/LICENSE
--rw-r--r--   0 kgd       (1000) kgd       (1000)     6108 2024-03-22 07:41:38.510860 amaze-benchmarker-1.0rc0.post1/PKG-INFO
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     4335 2024-03-21 09:36:52.000000 amaze-benchmarker-1.0rc0.post1/README.md
--rwxrw-r--   0 kgd       (1000) kgd       (1000)     2210 2024-03-22 06:47:42.000000 amaze-benchmarker-1.0rc0.post1/deploy_test.sh
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.490860 amaze-benchmarker-1.0rc0.post1/docs/
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)      306 2024-02-29 10:36:52.000000 amaze-benchmarker-1.0rc0.post1/docs/autorebuild.sh
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.494860 amaze-benchmarker-1.0rc0.post1/docs/demo/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)  1082176 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/demo/cc.gif
--rw-rw-r--   0 kgd       (1000) kgd       (1000)   189119 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/demo/cd.gif
--rw-rw-r--   0 kgd       (1000) kgd       (1000)   159118 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/demo/dd.gif
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.494860 amaze-benchmarker-1.0rc0.post1/docs/dependencies/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     5539 2024-02-29 07:33:48.000000 amaze-benchmarker-1.0rc0.post1/docs/dependencies/extract.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.498860 amaze-benchmarker-1.0rc0.post1/docs/latex/
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.498860 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     3748 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/agents.tex
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    12594 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/dark-0.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    11978 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/dark-1.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    40630 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/dark-2.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     9661 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/dark-3.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    12597 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/light-0.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    11995 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/light-1.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    40399 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/light-2.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     9152 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/light-3.png
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.490860 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.498860 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/cd/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      796 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/cd/000_start.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      863 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/cd/011_clue.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      874 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/cd/030_lure.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      849 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/cd/053_trap.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      806 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/cd/060_end.png
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.498860 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/dd/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      861 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/dd/000_start.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      861 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/dd/011_clue.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      864 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/dd/030_lure.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      865 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/dd/053_trap.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      857 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/dd/060_end.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      666 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/common.tex
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)      503 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/compile.sh
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.502860 amaze-benchmarker-1.0rc0.post1/docs/latex/maze/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    45931 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/maze/dark.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    46013 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/maze/light.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     2954 2024-02-16 14:59:54.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/maze/maze.tex
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     4011 2024-02-15 07:59:41.000000 amaze-benchmarker-1.0rc0.post1/docs/latex/maze/sample_maze.png
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.502860 amaze-benchmarker-1.0rc0.post1/docs/src/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      319 2024-02-27 07:40:08.000000 amaze-benchmarker-1.0rc0.post1/docs/src/api.rst
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     9053 2024-03-14 14:31:32.000000 amaze-benchmarker-1.0rc0.post1/docs/src/conf.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      238 2024-03-12 12:47:26.000000 amaze-benchmarker-1.0rc0.post1/docs/src/index.rst
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      138 2024-02-20 06:46:24.000000 amaze-benchmarker-1.0rc0.post1/docs/src/misc.rst
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.502860 amaze-benchmarker-1.0rc0.post1/docs/src/static/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      378 2024-02-20 06:46:24.000000 amaze-benchmarker-1.0rc0.post1/docs/src/static/custom.css
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      456 2024-03-12 12:35:03.000000 amaze-benchmarker-1.0rc0.post1/docs/src/static/favicon-dark.png
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      477 2024-03-12 12:34:29.000000 amaze-benchmarker-1.0rc0.post1/docs/src/static/favicon-light.png
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.502860 amaze-benchmarker-1.0rc0.post1/docs/src/usage/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     2077 2024-02-29 07:33:48.000000 amaze-benchmarker-1.0rc0.post1/docs/src/usage/basics.rst
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     1930 2024-03-21 09:34:18.000000 amaze-benchmarker-1.0rc0.post1/docs/src/usage/index.rst
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     2844 2024-03-21 13:34:10.000000 amaze-benchmarker-1.0rc0.post1/docs/src/usage/interface.rst
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     3377 2024-03-07 09:33:07.000000 amaze-benchmarker-1.0rc0.post1/docs/src/usage/sb3.rst
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     4489 2024-03-07 08:08:05.000000 amaze-benchmarker-1.0rc0.post1/docs/src/usage/training.rst
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     2040 2024-03-21 09:31:38.000000 amaze-benchmarker-1.0rc0.post1/docs/src/usage/visualization.rst
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.502860 amaze-benchmarker-1.0rc0.post1/examples/
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.502860 amaze-benchmarker-1.0rc0.post1/examples/agents/
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)   149605 2024-03-07 08:53:33.000000 amaze-benchmarker-1.0rc0.post1/examples/agents/simple_sb3-ppo.zip
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     6003 2024-02-25 08:31:28.000000 amaze-benchmarker-1.0rc0.post1/examples/agents/unicursive_tabular.zip
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      619 2024-02-29 07:33:48.000000 amaze-benchmarker-1.0rc0.post1/examples/basics.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.502860 amaze-benchmarker-1.0rc0.post1/examples/extensions/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     3726 2024-03-21 19:37:39.000000 amaze-benchmarker-1.0rc0.post1/examples/extensions/sb3.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     2749 2024-03-21 13:35:58.000000 amaze-benchmarker-1.0rc0.post1/examples/interface.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     5208 2024-03-21 13:37:52.000000 amaze-benchmarker-1.0rc0.post1/examples/q_learning.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     1312 2024-03-21 19:37:14.000000 amaze-benchmarker-1.0rc0.post1/examples/visualization.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     1885 2024-03-22 07:40:48.000000 amaze-benchmarker-1.0rc0.post1/pyproject.toml
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/scripts/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      355 2023-08-11 11:37:43.000000 amaze-benchmarker-1.0rc0.post1/scripts/mazes.dat
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)     1412 2023-08-10 12:01:45.000000 amaze-benchmarker-1.0rc0.post1/scripts/pull_from_ripper.sh
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)      337 2023-08-09 06:52:03.000000 amaze-benchmarker-1.0rc0.post1/scripts/push_to_ripper.sh
--rwxrw-r--   0 kgd       (1000) kgd       (1000)      708 2023-08-11 06:45:13.000000 amaze-benchmarker-1.0rc0.post1/scripts/sst_ripper_replicate.sh
--rwxrw-r--   0 kgd       (1000) kgd       (1000)     1057 2023-08-11 11:37:55.000000 amaze-benchmarker-1.0rc0.post1/scripts/sst_run.sh
--rw-rw-r--   0 kgd       (1000) kgd       (1000)       38 2024-03-22 07:41:38.510860 amaze-benchmarker-1.0rc0.post1/setup.cfg
--rw-rw-r--   0 kgd       (1000) kgd       (1000)       38 2024-02-20 06:46:24.000000 amaze-benchmarker-1.0rc0.post1/setup.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.490860 amaze-benchmarker-1.0rc0.post1/src/
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/src/amaze/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      346 2024-03-21 11:34:21.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/__init__.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/src/amaze/bin/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)       72 2024-02-27 07:40:08.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/bin/__init__.py
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)    10050 2024-03-21 19:34:26.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/bin/main.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/src/amaze/bin/tools/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)        0 2024-02-27 07:40:08.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/bin/tools/__init__.py
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)     3433 2024-03-20 16:48:43.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/bin/tools/interpolator.py
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)     2647 2024-02-27 07:40:08.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/bin/tools/stats.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)        0 2024-02-27 07:40:08.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/__init__.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)     1952 2024-03-07 08:22:15.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/__init__.py
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)     7573 2024-03-07 06:45:22.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/callbacks.py
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)     4611 2024-03-07 08:48:55.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/controller.py
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)     6092 2024-02-29 07:33:48.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/graph.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     1675 2024-03-07 08:19:03.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/guard.py
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)     7883 2024-03-20 16:48:43.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/maze_env.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     1680 2024-03-07 06:45:22.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/networks.py
--rwxrwxr-x   0 kgd       (1000) kgd       (1000)      900 2024-03-07 06:45:22.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/utils.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      282 2024-03-21 11:34:10.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/__init__.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     3515 2024-02-27 07:40:08.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/_build_data.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     8618 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/_maze_metrics.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      109 2024-02-20 06:46:24.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/__init__.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     1917 2024-03-07 06:45:22.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/base.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     1819 2024-03-21 18:18:33.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/cheater.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     3991 2024-03-21 14:51:59.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/control.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     3099 2024-03-07 06:45:22.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/keyboard.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     2182 2024-03-21 16:03:52.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/random.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     5743 2024-03-07 06:45:22.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/tabular.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    20084 2024-03-21 11:33:59.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/maze.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     1652 2024-02-27 07:40:08.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/pos.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     4108 2024-03-20 09:18:10.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/robot.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    14178 2024-03-20 09:16:31.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/simulation.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     1119 2024-03-21 11:33:59.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/simu/types.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)       61 2024-02-27 07:40:08.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/__init__.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     5881 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/maze.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/plotters/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)        0 2023-08-02 06:03:47.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/plotters/__init__.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     1653 2024-02-27 07:40:08.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/plotters/tabular.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     9271 2024-03-21 07:10:47.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/resources.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    33499 2024-03-21 19:36:39.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/viewer.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      708 2024-02-29 08:17:19.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/__init__.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    16063 2024-02-29 08:16:15.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/_trajectory_plotter.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     1979 2023-08-08 07:33:20.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/collapsible.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      772 2023-06-01 09:12:37.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/combobox.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     6068 2024-02-24 10:05:33.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/labels.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     3902 2023-08-21 10:41:19.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/lists.py
--rw-rw-r--   0 kgd       (1000) kgd       (1000)    14387 2024-03-21 07:09:27.000000 amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/maze.py
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/src/amaze_benchmarker.egg-info/
--rw-r--r--   0 kgd       (1000) kgd       (1000)     6108 2024-03-22 07:41:38.000000 amaze-benchmarker-1.0rc0.post1/src/amaze_benchmarker.egg-info/PKG-INFO
--rw-rw-r--   0 kgd       (1000) kgd       (1000)     3341 2024-03-22 07:41:38.000000 amaze-benchmarker-1.0rc0.post1/src/amaze_benchmarker.egg-info/SOURCES.txt
--rw-rw-r--   0 kgd       (1000) kgd       (1000)        1 2024-03-22 07:41:38.000000 amaze-benchmarker-1.0rc0.post1/src/amaze_benchmarker.egg-info/dependency_links.txt
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      141 2024-03-22 07:41:38.000000 amaze-benchmarker-1.0rc0.post1/src/amaze_benchmarker.egg-info/entry_points.txt
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      300 2024-03-22 07:41:38.000000 amaze-benchmarker-1.0rc0.post1/src/amaze_benchmarker.egg-info/requires.txt
--rw-rw-r--   0 kgd       (1000) kgd       (1000)        6 2024-03-22 07:41:38.000000 amaze-benchmarker-1.0rc0.post1/src/amaze_benchmarker.egg-info/top_level.txt
-drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-03-22 07:41:38.506860 amaze-benchmarker-1.0rc0.post1/tests/
--rw-rw-r--   0 kgd       (1000) kgd       (1000)      467 2024-03-21 13:36:40.000000 amaze-benchmarker-1.0rc0.post1/tests/simple_test.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.888095 amaze_benchmarker-1.0rc0.post2/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     3325 2024-05-02 11:08:05.000000 amaze_benchmarker-1.0rc0.post2/.gitignore
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      272 2024-03-07 10:02:48.000000 amaze_benchmarker-1.0rc0.post2/.readthedocs.yaml
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     1075 2023-06-01 09:12:37.000000 amaze_benchmarker-1.0rc0.post2/LICENSE
+-rw-r--r--   0 kgd       (1000) kgd       (1000)     6108 2024-05-28 04:53:19.888095 amaze_benchmarker-1.0rc0.post2/PKG-INFO
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     4335 2024-03-21 09:36:52.000000 amaze_benchmarker-1.0rc0.post2/README.md
+-rwxrw-r--   0 kgd       (1000) kgd       (1000)     2210 2024-03-22 06:47:42.000000 amaze_benchmarker-1.0rc0.post2/deploy_test.sh
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.880095 amaze_benchmarker-1.0rc0.post2/docs/
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)      306 2024-02-29 10:36:52.000000 amaze_benchmarker-1.0rc0.post2/docs/autorebuild.sh
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.880095 amaze_benchmarker-1.0rc0.post2/docs/demo/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)  1082176 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/demo/cc.gif
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)   189119 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/demo/cd.gif
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)   159118 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/demo/dd.gif
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.880095 amaze_benchmarker-1.0rc0.post2/docs/dependencies/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     5539 2024-02-29 07:33:48.000000 amaze_benchmarker-1.0rc0.post2/docs/dependencies/extract.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.880095 amaze_benchmarker-1.0rc0.post2/docs/latex/
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     3748 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/agents.tex
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    12594 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/dark-0.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    11978 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/dark-1.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    40630 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/dark-2.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     9661 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/dark-3.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    12597 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/light-0.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    11995 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/light-1.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    40399 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/light-2.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     9152 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/light-3.png
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.880095 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/cd/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      796 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/cd/000_start.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      863 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/cd/011_clue.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      874 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/cd/030_lure.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      849 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/cd/053_trap.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      806 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/cd/060_end.png
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/dd/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      861 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/dd/000_start.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      861 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/dd/011_clue.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      864 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/dd/030_lure.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      865 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/dd/053_trap.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      857 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/dd/060_end.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      666 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/common.tex
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)      503 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/compile.sh
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/docs/latex/maze/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    45931 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/maze/dark.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    46013 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/maze/light.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     2954 2024-02-16 14:59:54.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/maze/maze.tex
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     4011 2024-02-15 07:59:41.000000 amaze_benchmarker-1.0rc0.post2/docs/latex/maze/sample_maze.png
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/docs/src/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      319 2024-02-27 07:40:08.000000 amaze_benchmarker-1.0rc0.post2/docs/src/api.rst
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     9053 2024-03-14 14:31:32.000000 amaze_benchmarker-1.0rc0.post2/docs/src/conf.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      238 2024-03-12 12:47:26.000000 amaze_benchmarker-1.0rc0.post2/docs/src/index.rst
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      138 2024-02-20 06:46:24.000000 amaze_benchmarker-1.0rc0.post2/docs/src/misc.rst
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/docs/src/static/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      378 2024-02-20 06:46:24.000000 amaze_benchmarker-1.0rc0.post2/docs/src/static/custom.css
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      456 2024-03-12 12:35:03.000000 amaze_benchmarker-1.0rc0.post2/docs/src/static/favicon-dark.png
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      477 2024-03-12 12:34:29.000000 amaze_benchmarker-1.0rc0.post2/docs/src/static/favicon-light.png
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/docs/src/usage/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     2077 2024-02-29 07:33:48.000000 amaze_benchmarker-1.0rc0.post2/docs/src/usage/basics.rst
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     1930 2024-03-21 09:34:18.000000 amaze_benchmarker-1.0rc0.post2/docs/src/usage/index.rst
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     2844 2024-03-21 13:34:10.000000 amaze_benchmarker-1.0rc0.post2/docs/src/usage/interface.rst
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     3377 2024-03-07 09:33:07.000000 amaze_benchmarker-1.0rc0.post2/docs/src/usage/sb3.rst
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     4489 2024-03-07 08:08:05.000000 amaze_benchmarker-1.0rc0.post2/docs/src/usage/training.rst
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     2040 2024-03-21 09:31:38.000000 amaze_benchmarker-1.0rc0.post2/docs/src/usage/visualization.rst
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/examples/
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/examples/agents/
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)   149605 2024-03-07 08:53:33.000000 amaze_benchmarker-1.0rc0.post2/examples/agents/simple_sb3-ppo.zip
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     6003 2024-02-25 08:31:28.000000 amaze_benchmarker-1.0rc0.post2/examples/agents/unicursive_tabular.zip
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      619 2024-02-29 07:33:48.000000 amaze_benchmarker-1.0rc0.post2/examples/basics.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/examples/extensions/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     3726 2024-04-18 08:58:28.000000 amaze_benchmarker-1.0rc0.post2/examples/extensions/sb3.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     2749 2024-03-21 13:35:58.000000 amaze_benchmarker-1.0rc0.post2/examples/interface.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     5208 2024-03-21 13:37:52.000000 amaze_benchmarker-1.0rc0.post2/examples/q_learning.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     1312 2024-03-21 19:37:14.000000 amaze_benchmarker-1.0rc0.post2/examples/visualization.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     1885 2024-05-28 04:51:32.000000 amaze_benchmarker-1.0rc0.post2/pyproject.toml
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/scripts/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      355 2023-08-11 11:37:43.000000 amaze_benchmarker-1.0rc0.post2/scripts/mazes.dat
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)     1412 2023-08-10 12:01:45.000000 amaze_benchmarker-1.0rc0.post2/scripts/pull_from_ripper.sh
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)      337 2023-08-09 06:52:03.000000 amaze_benchmarker-1.0rc0.post2/scripts/push_to_ripper.sh
+-rwxrw-r--   0 kgd       (1000) kgd       (1000)      708 2023-08-11 06:45:13.000000 amaze_benchmarker-1.0rc0.post2/scripts/sst_ripper_replicate.sh
+-rwxrw-r--   0 kgd       (1000) kgd       (1000)     1057 2023-08-11 11:37:55.000000 amaze_benchmarker-1.0rc0.post2/scripts/sst_run.sh
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)       38 2024-05-28 04:53:19.888095 amaze_benchmarker-1.0rc0.post2/setup.cfg
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)       38 2024-02-20 06:46:24.000000 amaze_benchmarker-1.0rc0.post2/setup.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.880095 amaze_benchmarker-1.0rc0.post2/src/
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/src/amaze/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      346 2024-03-21 11:34:21.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/__init__.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/src/amaze/bin/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)       72 2024-02-27 07:40:08.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/bin/__init__.py
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)    10050 2024-03-21 19:34:26.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/bin/main.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/src/amaze/bin/tools/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)        0 2024-02-27 07:40:08.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/bin/tools/__init__.py
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)     3433 2024-03-20 16:48:43.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/bin/tools/interpolator.py
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)     2647 2024-02-27 07:40:08.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/bin/tools/stats.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)        0 2024-02-27 07:40:08.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/__init__.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)     1952 2024-03-07 08:22:15.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/__init__.py
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)     7573 2024-03-07 06:45:22.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/callbacks.py
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)     4611 2024-05-07 11:57:51.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/controller.py
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)     6092 2024-02-29 07:33:48.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/graph.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     1675 2024-03-07 08:19:03.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/guard.py
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)     7605 2024-03-26 09:05:12.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/maze_env.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     1680 2024-03-07 06:45:22.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/networks.py
+-rwxrwxr-x   0 kgd       (1000) kgd       (1000)      900 2024-03-07 06:45:22.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/utils.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.884095 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      282 2024-03-21 11:34:10.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/__init__.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     3515 2024-02-27 07:40:08.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/_build_data.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     8618 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/_maze_metrics.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.888095 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      109 2024-02-20 06:46:24.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/__init__.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     1917 2024-03-07 06:45:22.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/base.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     2275 2024-03-26 12:11:45.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/cheater.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     3991 2024-03-21 14:51:59.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/control.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     3099 2024-03-07 06:45:22.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/keyboard.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     2182 2024-03-21 16:03:52.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/random.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     5743 2024-03-07 06:45:22.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/tabular.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    20084 2024-03-21 11:33:59.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/maze.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     1652 2024-02-27 07:40:08.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/pos.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     4108 2024-03-20 09:18:10.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/robot.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    14178 2024-03-20 09:16:31.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/simulation.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     1119 2024-03-21 11:33:59.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/simu/types.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.888095 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)       61 2024-02-27 07:40:08.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/__init__.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     5881 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/maze.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.888095 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/plotters/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)        0 2023-08-02 06:03:47.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/plotters/__init__.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     1653 2024-02-27 07:40:08.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/plotters/tabular.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    11720 2024-05-28 04:50:30.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/resources.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    33689 2024-05-02 11:07:19.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/viewer.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.888095 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      708 2024-02-29 08:17:19.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/__init__.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    16063 2024-02-29 08:16:15.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/_trajectory_plotter.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     1979 2023-08-08 07:33:20.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/collapsible.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      772 2023-06-01 09:12:37.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/combobox.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     6068 2024-02-24 10:05:33.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/labels.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     3902 2023-08-21 10:41:19.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/lists.py
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)    14520 2024-03-26 12:12:31.000000 amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/maze.py
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.888095 amaze_benchmarker-1.0rc0.post2/src/amaze_benchmarker.egg-info/
+-rw-r--r--   0 kgd       (1000) kgd       (1000)     6108 2024-05-28 04:53:19.000000 amaze_benchmarker-1.0rc0.post2/src/amaze_benchmarker.egg-info/PKG-INFO
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)     3341 2024-05-28 04:53:19.000000 amaze_benchmarker-1.0rc0.post2/src/amaze_benchmarker.egg-info/SOURCES.txt
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)        1 2024-05-28 04:53:19.000000 amaze_benchmarker-1.0rc0.post2/src/amaze_benchmarker.egg-info/dependency_links.txt
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      141 2024-05-28 04:53:19.000000 amaze_benchmarker-1.0rc0.post2/src/amaze_benchmarker.egg-info/entry_points.txt
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      300 2024-05-28 04:53:19.000000 amaze_benchmarker-1.0rc0.post2/src/amaze_benchmarker.egg-info/requires.txt
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)        6 2024-05-28 04:53:19.000000 amaze_benchmarker-1.0rc0.post2/src/amaze_benchmarker.egg-info/top_level.txt
+drwxrwxr-x   0 kgd       (1000) kgd       (1000)        0 2024-05-28 04:53:19.888095 amaze_benchmarker-1.0rc0.post2/tests/
+-rw-rw-r--   0 kgd       (1000) kgd       (1000)      467 2024-03-21 13:36:40.000000 amaze_benchmarker-1.0rc0.post2/tests/simple_test.py
```

### Comparing `amaze-benchmarker-1.0rc0.post1/.gitignore` & `amaze_benchmarker-1.0rc0.post2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Personal exclusion
 
 .idea/
-cache/
+resources/cache/
 data/
 obsolete/
 remote/
 results/
 backup_results/
 stash/
 tmp/
```

### Comparing `amaze-benchmarker-1.0rc0.post1/LICENSE` & `amaze_benchmarker-1.0rc0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/PKG-INFO` & `amaze_benchmarker-1.0rc0.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amaze-benchmarker
-Version: 1.0rc0.post1
+Version: 1.0rc0.post2
 Summary: Benchmark generator for sighted maze-navigating agents
 Author-email: Kevin Godin-Dubois <k.j.m.godin-dubois@vu.nl>
 Project-URL: Homepage, https://github.com/kgd-al/amaze
 Project-URL: Documentation, https://amaze.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/kgd-al/amaze/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `amaze-benchmarker-1.0rc0.post1/README.md` & `amaze_benchmarker-1.0rc0.post2/README.md`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/deploy_test.sh` & `amaze_benchmarker-1.0rc0.post2/deploy_test.sh`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/demo/cc.gif` & `amaze_benchmarker-1.0rc0.post2/docs/demo/cc.gif`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/demo/cd.gif` & `amaze_benchmarker-1.0rc0.post2/docs/demo/cd.gif`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/demo/dd.gif` & `amaze_benchmarker-1.0rc0.post2/docs/demo/dd.gif`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/dependencies/extract.py` & `amaze_benchmarker-1.0rc0.post2/docs/dependencies/extract.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/agents.tex` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/agents.tex`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/dark-0.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/dark-0.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/dark-1.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/dark-1.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/dark-2.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/dark-2.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/dark-3.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/dark-3.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/light-0.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/light-0.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/light-1.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/light-1.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/light-2.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/light-2.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/light-3.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/light-3.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/cd/000_start.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/cd/000_start.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/cd/011_clue.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/cd/011_clue.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/cd/030_lure.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/cd/030_lure.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/cd/053_trap.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/cd/053_trap.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/cd/060_end.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/cd/060_end.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/dd/000_start.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/dd/000_start.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/dd/011_clue.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/dd/011_clue.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/dd/030_lure.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/dd/030_lure.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/dd/053_trap.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/dd/053_trap.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/agents/vision/dd/060_end.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/agents/vision/dd/060_end.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/common.tex` & `amaze_benchmarker-1.0rc0.post2/docs/latex/common.tex`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/maze/dark.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/maze/dark.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/maze/light.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/maze/light.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/maze/maze.tex` & `amaze_benchmarker-1.0rc0.post2/docs/latex/maze/maze.tex`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/latex/maze/sample_maze.png` & `amaze_benchmarker-1.0rc0.post2/docs/latex/maze/sample_maze.png`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/src/conf.py` & `amaze_benchmarker-1.0rc0.post2/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/src/usage/basics.rst` & `amaze_benchmarker-1.0rc0.post2/docs/src/usage/basics.rst`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/src/usage/index.rst` & `amaze_benchmarker-1.0rc0.post2/docs/src/usage/index.rst`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/src/usage/interface.rst` & `amaze_benchmarker-1.0rc0.post2/docs/src/usage/interface.rst`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/src/usage/sb3.rst` & `amaze_benchmarker-1.0rc0.post2/docs/src/usage/sb3.rst`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/src/usage/training.rst` & `amaze_benchmarker-1.0rc0.post2/docs/src/usage/training.rst`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/docs/src/usage/visualization.rst` & `amaze_benchmarker-1.0rc0.post2/docs/src/usage/visualization.rst`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/examples/agents/simple_sb3-ppo.zip` & `amaze_benchmarker-1.0rc0.post2/examples/agents/simple_sb3-ppo.zip`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/examples/agents/unicursive_tabular.zip` & `amaze_benchmarker-1.0rc0.post2/examples/agents/unicursive_tabular.zip`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/examples/basics.py` & `amaze_benchmarker-1.0rc0.post2/examples/basics.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/examples/extensions/sb3.py` & `amaze_benchmarker-1.0rc0.post2/examples/extensions/sb3.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/examples/interface.py` & `amaze_benchmarker-1.0rc0.post2/examples/interface.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/examples/q_learning.py` & `amaze_benchmarker-1.0rc0.post2/examples/q_learning.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/examples/visualization.py` & `amaze_benchmarker-1.0rc0.post2/examples/visualization.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/pyproject.toml` & `amaze_benchmarker-1.0rc0.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "amaze-benchmarker"
-version = "1.0rc0.post1"
+version = "1.0rc0.post2"
 authors = [{ name="Kevin Godin-Dubois", email="k.j.m.godin-dubois@vu.nl"}]
 description = "Benchmark generator for sighted maze-navigating agents"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `amaze-benchmarker-1.0rc0.post1/scripts/pull_from_ripper.sh` & `amaze_benchmarker-1.0rc0.post2/scripts/pull_from_ripper.sh`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/scripts/sst_ripper_replicate.sh` & `amaze_benchmarker-1.0rc0.post2/scripts/sst_ripper_replicate.sh`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/scripts/sst_run.sh` & `amaze_benchmarker-1.0rc0.post2/scripts/sst_run.sh`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/bin/main.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/bin/main.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/bin/tools/interpolator.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/bin/tools/interpolator.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/bin/tools/stats.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/bin/tools/stats.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/__init__.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/__init__.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/callbacks.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/callbacks.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/controller.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/controller.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/graph.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/graph.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/guard.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/guard.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/maze_env.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/maze_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from amaze import application
 from amaze.extensions.sb3.utils import IOMapper
 from amaze.extensions.sb3 import CV2QTGuard
 from amaze.simu.maze import Maze
 from amaze.simu.robot import Robot
 from amaze.simu.simulation import Simulation
 from amaze.simu.types import InputType, OutputType
+from amaze.visu.resources import qimage_to_numpy
 from amaze.visu.widgets.maze import MazeWidget
 
 logger = logging.getLogger(__name__)
 
 
 def make_vec_maze_env(mazes: List[Maze.BuildData],
                       robot: Robot.BuildData,
@@ -159,15 +160,15 @@
             img = QImage(s, s, QImage.Format_RGB888)
             img.fill(Qt.white)
 
             painter = QPainter(img)
             self.widget.render_onto(painter, width=s)
             painter.end()
 
-            return self._qimage_to_numpy(img)
+            return qimage_to_numpy(img)
 
     def close(self):
         """ Stub """
         pass
 
     def name(self): return self.name
     def atomic_rewards(self): return self._simulation.rewards
@@ -199,15 +200,15 @@
                 ),
                 side=cb_side,
                 verbose=verbose,
                 square=square,
                 img_format=QImage.Format_RGBA8888,
                 path=None
             )
-            img = self._qimage_to_numpy(plot)
+            img = qimage_to_numpy(plot)
         return img
 
     def _create_widget(self, show_robot=False):
         if self.widget:
             return self.widget
 
         app = QtWidgets.QApplication.instance()
@@ -220,19 +221,11 @@
         self.widget = MazeWidget.from_simulation(
             simulation=self._simulation
         )
         self.widget.update_config(
             robot=show_robot, solution=True, dark=True)
         return self.widget
 
-    @staticmethod
-    def _qimage_to_numpy(img: QImage) -> np.ndarray:
-        w, h, d = img.width(), img.height(), img.depth() // 8
-        b = img.constBits().asstring(img.byteCount())
-        bw = img.bytesPerLine() // d
-        return np.ndarray(
-            shape=(h, bw, d), buffer=b, dtype=np.uint8)[:, :w]
-
     def _observations(self):
         return self.mapper.map_observation(self._simulation.observations)
 
     def infos(self): return self._simulation.infos()
```

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/networks.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/networks.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/extensions/sb3/utils.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/extensions/sb3/utils.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/simu/_build_data.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/simu/_build_data.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/simu/_maze_metrics.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/simu/_maze_metrics.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/base.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/base.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/control.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/control.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/keyboard.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/keyboard.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/random.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/random.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/simu/controllers/tabular.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/simu/controllers/tabular.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/simu/maze.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/simu/maze.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/simu/pos.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/simu/pos.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/simu/robot.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/simu/robot.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/simu/simulation.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/simu/simulation.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/simu/types.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/simu/types.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/visu/maze.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/visu/maze.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/visu/plotters/tabular.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/visu/plotters/tabular.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/visu/resources.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/visu/resources.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import logging
 import os
 import pprint
 import sys
 from enum import Enum
 from functools import cache
 from logging import getLogger
 from pathlib import Path
@@ -10,14 +11,19 @@
 
 import numpy as np
 from PyQt5.QtCore import Qt, QRectF, QPointF
 from PyQt5.QtGui import QPainter, QPainterPath, QColor, QImage, QTransform, QPolygonF
 
 logger = getLogger(__name__)
 
+# Change cache location to /resources/cache
+# change custom folder location  /resources/custom
+# extension always png
+# change test from path.suffix to path.exists()
+
 
 # =============================================================================
 # Public API
 
 def _default_builtin() -> str: return "arrow"
 def _default_lightness() -> float: return .5
 def _default_size() -> int: return 15
@@ -73,25 +79,20 @@
                 val = float(tokens[1])
             except ValueError:
                 raise ValueError(
                     f"'{tokens[1]} is not a valid cue value")
         else:
             raise ValueError(f"Mis-formed sign: {tokens}")
 
-        p_name = Path(name)
-        if p_name.suffix:
-            if p_name.exists():
-                name = p_name
-            else:
-                raise ValueError(f"Path like argument '{p_name}' does not"
-                                 f" refer to an existing file")
-
-        elif name not in builtins():
+        if name not in names():
             raise ValueError(f"Unknown cue name '{name}'."
-                             f" Valid values are {pprint.pformat(builtins())}")
+                             f" Valid values are:\n"
+                             f" > {', '.join(builtins())} (built-ins)\n"
+                             f" > {', '.join(_custom_paths.keys())}"
+                             f" (custom from {custom_resources_path()})")
 
         return cls(name, val)
 
     def to_string(self) -> str:
         s = []
         if self.name != _default_builtin():
             s.append(self.name)
@@ -101,59 +102,118 @@
 
 Signs = List[Sign]
 DataKey = Tuple[str, float, int]
 
 
 def resources_path():
     """ Where to look for sign images and where to cache built-ins """
-    return Path("cache/resources/")
+    return Path("resources")
+
+
+def cached_resources_path() -> Path:
+    """ Where to look for cached built-ins """
+    return resources_path().joinpath("cache")
+
+
+def custom_resources_path() -> Path:
+    """ Where to look for custom images """
+    return resources_path().joinpath("custom")
+
+
+def resources_format() -> str:
+    """ Image format for the cached and custom resources """
+    return "png"
 
 
 # =============================================================================
 # Image loader/generator
 
 def _key_to_path(key: DataKey) -> str:
-    return f"{key[0]}_{key[1]:.2}_{key[2]}.png"
+    return f"{key[0]}_{key[1]:.2}_{key[2]}.{resources_format()}"
 
 
 @cache
 def _factories():
     factories = {}
     for k, v in sorted(sys.modules[__name__].__dict__.items()):
         if callable(v) and k.startswith("__generator__"):
             factories[k[13:]] = v
     return factories
 
 
-@cache
 def _get_image(key: DataKey):
-    filename = resources_path().joinpath(_key_to_path(key))
+    # First look in RAM cache
+    if (img := _cache.get(key)) is not None:
+        return img
 
-    if False and not os.environ["KGD_AMAZE_NOCACHE"]:
+    # Else look in file cache
+    filename = cached_resources_path().joinpath(_key_to_path(key))
+    if not os.environ.get("KGD_AMAZE_NOCACHE", False):
         if filename.exists():
             img = QImage(str(filename))
             if not img.isNull():
+                _cache[key] = img
                 return img
             else:
                 logger.warning(f"Error loading file {filename}")
+                return __generator__error()
+
+    if (factory := _factories().get(key[0])) is not None:
+        img = factory(*key[1:])
+        if img.isNull():
+            logger.warning(f"Error generating {key}")
+            return __generator__error()
 
-    img = _factories()[key[0]](*key[1:])
-    if not img.isNull():
         filename.parent.mkdir(parents=True, exist_ok=True)
         img.save(str(filename))
+        _cache[key] = img
+        return img
+
+    if (source := _custom_paths.get(key[0])) is not None:
+        img = QImage(str(source))
+        w, h = img.width(), img.height()
+        if w != h and 4*w != h:
+            logger.warning(f"Malformed image for {key} at {source}: Size is"
+                           f" {w}x{h} which is neither a single or 4 squares")
+        img = _process_custom_image(img, *key[1:])
+        if img.isNull():
+            logger.warning(f"Error loading {key} from {source}")
+            return __generator__error()
+        logger.info(f"Using custom sign ({source}) of size {img.size()}")
+        ok = img.save(str(filename))
+        if ok:
+            logger.info(f"Saved {key} to cache")
+        else:
+            logger.warning(f"Could not save {key} to cache")
+
+        _cache[key] = img
+
         return img
-    else:
-        logger.warning(f"Error generating {key}")
-        return __generator__error()
 
 
 # =============================================================================
 # Internals
 
 
+def _process_custom_image(img: QImage, lightness: float, size: int):
+    img = img.convertTo(QImage.Format_ARGB32) \
+             .scaledToWidth(size, mode=Qt.SmoothTransformation)
+
+    if lightness != _default_lightness():
+        logging.warning("Specifying lightness for custom images is not yet"
+                        " supported.")
+    # depth = 4
+    # for j in range(img.height()):
+    #     scan = img.scanLine(j)
+    #     for i in range(img.width()):
+    #         rgb =
+
+    return img
+
+
 def _image(width: int, lightness: float, multi=False):
     img = QImage(width, 4 * width if multi else width, QImage.Format_ARGB32)
     img.fill(Qt.transparent)
     painter = QPainter(img)
     pen = painter.pen()
     pen.setColor(__pen_color(lightness))
     pen.setWidthF(.1)
@@ -237,22 +297,30 @@
 def builtins():
     """ List of all programmatically drawn signs """
     return list(_factories().keys())
 
 
 def __extract_names():
     nlist = []
-    for f in resources_path().glob("*.png"):
-        if f.name.count('_') == 0:  # Base (user-provided) file
-            nlist.append(f.name)
+    cdict = {}
+    for f in custom_resources_path().glob(f"*.{resources_format()}"):
+        nlist.append(f.stem)
+        cdict[f.stem] = f
     nlist.extend(builtins())
-    return nlist
+    return nlist, cdict
+
 
+_names, _custom_paths = __extract_names()
+_cache: dict[DataKey, QImage] = {}
+cached_resources_path().mkdir(parents=True, exist_ok=True)
 
-_names = __extract_names()
+# print("[kgd-debug] cached resources lists:")
+# pprint.pprint(_names)
+# pprint.pprint(_custom_paths)
+# print("[kgd-debug] =====")
 
 
 def names():
     """ List of all possible sign shapes, including both built-ins and those
     found in :meth:`~resources_path`"""
     return _names
 
@@ -301,17 +369,25 @@
         subarray = []
         for j, p in enumerate(p_list):
             img = QImage(p.size(), QImage.Format_Grayscale8)
             img.fill(QColor.fromRgb(rgb_fill))
             painter = QPainter(img)
             painter.drawImage(img.rect(), p, p.rect())
             painter.end()
-            w, h = img.width(), img.height()
-            b = img.constBits().asstring(img.byteCount())
-            bw = img.bytesPerLine()
-            arr = np.ndarray(shape=(h, bw),
-                             buffer=b,
-                             dtype=np.uint8)[:, :w]
-            subarray.append(copy.deepcopy(_v_scale(np.flipud(arr))))
+            subarray.append(
+                copy.deepcopy(
+                    _v_scale(
+                        np.flipud(
+                            qimage_to_numpy(img)))))
         arrays.append(subarray)
 
     return arrays
+
+
+def qimage_to_numpy(img: QImage) -> np.ndarray:
+    w, h, d = img.width(), img.height(), img.depth() // 8
+    b = img.constBits().asstring(img.byteCount())
+    bw = img.bytesPerLine() // d
+    shape = (h, bw) if d == 1 else (h, bw, d)
+    return np.ndarray(
+        shape=shape, buffer=b, dtype=np.uint8)[:, :w]
+
```

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/visu/viewer.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/visu/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,16 @@
         self.layout = QHBoxLayout()
 
         self.runnable = runnable
 
         if runnable:
             self.playing = False
             self.speed = 1
-            self.timer_dt = args.dt or .1
+
+            self.timer_dt = args.dt if args and args.dt else .1
 
             self.timer = QTimer()
 
             self.next_action = None
         self.controller = None
 
         # ----
@@ -137,19 +138,21 @@
             self.timer.timeout.connect(self._step)
 
         self._connect_signals()
 
         self._update()
         self.buttons["play"].setFocus()
 
-        self._movie = _MovieRecorder(self, args.movie) if args.movie else None
+        self._movie = _MovieRecorder(self, args.movie) if args and args.movie else None
 
         if self.robot_mode:  # Trimmed down version for the robot
             self._set_robot_mode_layout()
 
+        self.maze_changed.emit()
+
     # =========================================================================
     # == Miscellaneous controllers
     # =========================================================================
 
     def set_maze(self, bd: Maze.BuildData):
         assert isinstance(bd, Maze.BuildData)
         self._restore_from_maze_build_data(bd)
@@ -205,15 +208,15 @@
         )
         if self.controller and flags & reset.CONTROL:
             self.controller.reset()
 
         self.maze_w.reset_from_simulation(self.simulation)
         self.simulation.generate_inputs()
         self.sections[self.Sections.CONFIG].setEnabled(True)
-        if self.runnable:
+        if self.runnable and self.controller:
             self.next_action = self._think()
         self._update()
 
         maze_metrics = Simulation.compute_metrics(
             self.simulation.maze, self.simulation.data.inputs,
             self.simulation.data.vision)
         s_str = (
@@ -228,14 +231,17 @@
             self.stats[f"m_{m.name.lower()}"].setText(v)
 
         title = self.simulation.maze.to_string()
         if self.controller:
             title += f" | {self.controller.name()}"
         self.setWindowTitle(title)
 
+        if flags & reset.MAZE:
+            self.maze_changed.emit()
+
     # =========================================================================
     # == Private control
     # =========================================================================
 
     def _play(self, play: Optional[bool] = None):
         if play is None:
             self.playing = not self.playing
@@ -320,16 +326,17 @@
                f"{self.simulation.last_reward:+g}"
                f" ({self.simulation.robot.reward:g})")
 
         if self.simulation.data is not None:
             def lbl(k): return self.visu["img_" + k]
             lbl("inputs").set_inputs(self.simulation.observations,
                                      self.simulation.data.inputs)
-            lbl("outputs").set_outputs(self.next_action,
-                                       self.simulation.data.outputs)
+            if self.controller is not None:
+                lbl("outputs").set_outputs(self.next_action,
+                                           self.simulation.data.outputs)
             lbl("values").set_values(self.controller,
                                      self.simulation.observations)
 
     # =========================================================================
     # == Config collectors
     # =========================================================================
 
@@ -342,16 +349,14 @@
         self.stats["m_intersections"].setText(str(stats['intersections']))
         for t in [SignType.LURE, SignType.TRAP]:
             key = t.value.lower() + "s"
             data = stats[key]
             self.stats[f"m_{key}"].setText(
                 str(data) if data is not None else "/")
 
-        self.maze_changed.emit()
-
         return maze
 
     def _combobox_value(self, name):
         return self.config[name].currentText().upper()
 
     def _enum_value(self, name, enum): return enum[self._combobox_value(name)]
 
@@ -641,15 +646,15 @@
         row("Inputs", cb)
 
         cb = widget(QComboBox, "outputs")
         cb.addItems([v.name.lower() for v in OutputType])
         row("Outputs", cb)
 
         cb = widget(QComboBox, "control")
-        cb.addItems([v.lower() for v in ["Random", "Cheater",
+        cb.addItems([v.lower() for v in ["Cheater", "Random",
                                          "Keyboard", "Autonomous"]])
         row("Control", cb)
 
         return layout
 
     def _build_controller_label(self):
         layout = QVBoxLayout()
@@ -825,15 +830,15 @@
             self.sections[k].set_collapsed(
                 bool(int(config.value(k.value.lower(), False))))
         config.endGroup()
 
         return viewer_options
 
     def _save_settings(self):
-        if not self.args.restore_config:
+        if not self.args or not self.args.restore_config:
             return
 
         config = self._settings()
         logger.info(f"Saving configuration to {config.fileName()}")
 
         config.setValue('pos', self.pos())
         config.setValue('size', self.size())
```

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/__init__.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/_trajectory_plotter.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/_trajectory_plotter.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/collapsible.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/collapsible.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/combobox.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/combobox.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/labels.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/labels.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/lists.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/lists.py`

 * *Files identical despite different names*

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze/visu/widgets/maze.py` & `amaze_benchmarker-1.0rc0.post2/src/amaze/visu/widgets/maze.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from amaze import Robot
 from amaze.simu.maze import Maze
 from amaze.simu.simulation import Simulation
 from amaze.simu.types import InputType, OutputType
 from amaze.visu import resources
 from amaze.visu.maze import MazePainter, Color, logger
-from amaze.visu.resources import SignType
+from amaze.visu.resources import SignType, qimage_to_numpy
 from amaze.visu.widgets import _trajectory_plotter, has_qt_application
 
 
 class QtPainter(MazePainter):
     def __init__(self, p: QPainter, config: dict):
         self.painter = p
         dark = config['dark']
@@ -243,14 +243,17 @@
 
     def pretty_render(self, width: Optional[int] = None):
         img, painter = self._image_drawer(width=width)
         self.render_onto(painter, width=width - 2)
         painter.end()
         return img
 
+    def numpy_render(self, width: Optional[int] = None):
+        return qimage_to_numpy(self.pretty_render(width))
+
     @classmethod
     def static_render_to_file(cls, maze, path, size=None, **kwargs):
         """ Render the provided maze to a file (in png format).
 
         Additional arguments refer to the rendering configuration, see
         :meth:`default_config`.
         """
```

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze_benchmarker.egg-info/PKG-INFO` & `amaze_benchmarker-1.0rc0.post2/src/amaze_benchmarker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amaze-benchmarker
-Version: 1.0rc0.post1
+Version: 1.0rc0.post2
 Summary: Benchmark generator for sighted maze-navigating agents
 Author-email: Kevin Godin-Dubois <k.j.m.godin-dubois@vu.nl>
 Project-URL: Homepage, https://github.com/kgd-al/amaze
 Project-URL: Documentation, https://amaze.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/kgd-al/amaze/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `amaze-benchmarker-1.0rc0.post1/src/amaze_benchmarker.egg-info/SOURCES.txt` & `amaze_benchmarker-1.0rc0.post2/src/amaze_benchmarker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

