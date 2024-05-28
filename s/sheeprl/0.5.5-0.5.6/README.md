# Comparing `tmp/sheeprl-0.5.5.tar.gz` & `tmp/sheeprl-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheeprl-0.5.5.tar", last modified: Mon Apr 22 09:34:12 2024, max compression
+gzip compressed data, was "sheeprl-0.5.6.tar", last modified: Tue May 28 09:23:27 2024, max compression
```

## Comparing `sheeprl-0.5.5.tar` & `sheeprl-0.5.6.tar`

### file list

```diff
@@ -1,268 +1,269 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.134818 sheeprl-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-22 09:34:07.000000 sheeprl-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-22 09:34:07.000000 sheeprl-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-04-22 09:34:12.134818 sheeprl-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24648 2024-04-22 09:34:07.000000 sheeprl-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.090818 sheeprl-0.5.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-22 09:34:07.000000 sheeprl-0.5.5/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.090818 sheeprl-0.5.5/hydra_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-22 09:34:07.000000 sheeprl-0.5.5/hydra_plugins/sheeprl_search_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-22 09:34:07.000000 sheeprl-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:34:12.134818 sheeprl-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-22 09:34:07.000000 sheeprl-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.094818 sheeprl-0.5.5/sheeprl/
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.094818 sheeprl-0.5.5/sheeprl/algos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.094818 sheeprl-0.5.5/sheeprl/algos/a2c/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/a2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16852 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/a2c/a2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/a2c/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/a2c/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/a2c/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/a2c/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.098818 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    36796 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/dreamer_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.098818 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50079 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    37400 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/dreamer_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.098818 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57479 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    35745 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/dreamer_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.098818 sheeprl-0.5.5/sheeprl/algos/droq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/droq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/droq/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/droq/droq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/droq/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/droq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.102818 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    39009 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/p2e_dv1_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)    20776 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/p2e_dv1_finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.102818 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    45472 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/p2e_dv2_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)    22095 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/p2e_dv2_finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.102818 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    50554 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/p2e_dv3_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)    22467 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/p2e_dv3_finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.106818 sheeprl-0.5.5/sheeprl/algos/ppo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    20146 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/ppo.py
--rw-r--r--   0 runner    (1001) docker     (127)    29280 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/ppo_decoupled.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.106818 sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    23740 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/ppo_recurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.106818 sheeprl-0.5.5/sheeprl/algos/sac/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    18646 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/sac.py
--rw-r--r--   0 runner    (1001) docker     (127)    25366 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/sac_decoupled.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.106818 sheeprl-0.5.5/sheeprl/algos/sac_ae/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac_ae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24357 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac_ae/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac_ae/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    22314 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac_ae/sac_ae.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac_ae/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/available_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    19690 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.106818 sheeprl-0.5.5/sheeprl/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.110818 sheeprl-0.5.5/sheeprl/configs/algo/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/a2c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3_L.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3_M.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3_S.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3_XL.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3_XS.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/droq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/p2e_dv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/p2e_dv2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/p2e_dv3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/ppo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/ppo_decoupled.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/ppo_recurrent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/sac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/sac_ae.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/sac_decoupled.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.110818 sheeprl-0.5.5/sheeprl/configs/buffer/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/buffer/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.110818 sheeprl-0.5.5/sheeprl/configs/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/checkpoint/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.110818 sheeprl-0.5.5/sheeprl/configs/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/distribution/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.114818 sheeprl-0.5.5/sheeprl/configs/env/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/atari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/crafter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/diambra.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/dmc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/dummy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/gym.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/minecraft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/minedojo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/minerl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/minerl_obtain_diamond.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/minerl_obtain_iron_pickaxe.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/mujoco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/super_mario_bros.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/eval_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.122818 sheeprl-0.5.5/sheeprl/configs/exp/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/a2c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/a2c_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v1_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2_crafter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_100k_boxing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_100k_ms_pacman.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_L_doapp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_L_navigate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_XL_crafter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_dmc_cartpole_swingup_sparse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_super_mario_bros.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/droq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv1_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv1_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv2_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv2_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_fntn_L_doapp_64px_gray_combo_discrete_5Mstps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/ppo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/ppo_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/ppo_decoupled.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/ppo_recurrent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/ppo_super_mario_bros.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/sac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/sac_ae.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/sac_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/sac_decoupled.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.122818 sheeprl-0.5.5/sheeprl/configs/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/fabric/ddp-cpu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/fabric/ddp-cuda.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/fabric/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.122818 sheeprl-0.5.5/sheeprl/configs/hydra/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/hydra/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.122818 sheeprl-0.5.5/sheeprl/configs/logger/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/logger/mlflow.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/logger/tensorboard.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.122818 sheeprl-0.5.5/sheeprl/configs/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/metric/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.126818 sheeprl-0.5.5/sheeprl/configs/model_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/a2c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/dreamer_v1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/dreamer_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/dreamer_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/droq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv1_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv1_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv2_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv2_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv3_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv3_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/ppo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/ppo_recurrent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/sac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/sac_ae.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.126818 sheeprl-0.5.5/sheeprl/configs/optim/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/optim/adam.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/optim/rmsprop.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/optim/rmsprop_tf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/optim/sgd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.126818 sheeprl-0.5.5/sheeprl/data/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54229 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/data/buffers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.126818 sheeprl-0.5.5/sheeprl/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/crafter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/diambra.py
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/dmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/minedojo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/minerl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.126818 sheeprl-0.5.5/sheeprl/envs/minerl_envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/minerl_envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/minerl_envs/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/minerl_envs/navigate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/minerl_envs/obtain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/super_mario_bros.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.130818 sheeprl-0.5.5/sheeprl/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21610 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.130818 sheeprl-0.5.5/sheeprl/optim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/optim/rmsprop_tf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.130818 sheeprl-0.5.5/sheeprl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    17999 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.130818 sheeprl-0.5.5/sheeprl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-04-22 09:34:12.000000 sheeprl-0.5.5/sheeprl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-22 09:34:12.000000 sheeprl-0.5.5/sheeprl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:34:12.000000 sheeprl-0.5.5/sheeprl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-22 09:34:12.000000 sheeprl-0.5.5/sheeprl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-22 09:34:12.000000 sheeprl-0.5.5/sheeprl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 09:34:12.000000 sheeprl-0.5.5/sheeprl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.554382 sheeprl-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-28 09:23:23.000000 sheeprl-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 09:23:23.000000 sheeprl-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-28 09:23:27.554382 sheeprl-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24648 2024-05-28 09:23:23.000000 sheeprl-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.510382 sheeprl-0.5.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-28 09:23:23.000000 sheeprl-0.5.6/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.510382 sheeprl-0.5.6/hydra_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-28 09:23:23.000000 sheeprl-0.5.6/hydra_plugins/sheeprl_search_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-28 09:23:23.000000 sheeprl-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:23:27.554382 sheeprl-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-28 09:23:23.000000 sheeprl-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.510382 sheeprl-0.5.6/sheeprl/
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.510382 sheeprl-0.5.6/sheeprl/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.514382 sheeprl-0.5.6/sheeprl/algos/a2c/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/a2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17056 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/a2c/a2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/a2c/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/a2c/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/a2c/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/a2c/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.514382 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37013 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/dreamer_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.514382 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50079 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37705 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/dreamer_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.518382 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57473 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36001 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/dreamer_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.518382 sheeprl-0.5.6/sheeprl/algos/droq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/droq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/droq/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19322 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/droq/droq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/droq/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/droq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.518382 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39226 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/p2e_dv1_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20966 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/p2e_dv1_finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.518382 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45740 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/p2e_dv2_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22312 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/p2e_dv2_finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.522382 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50773 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/p2e_dv3_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22684 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/p2e_dv3_finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.522382 sheeprl-0.5.6/sheeprl/algos/ppo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20232 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/ppo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29492 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/ppo_decoupled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.522382 sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23826 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/ppo_recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.526382 sheeprl-0.5.6/sheeprl/algos/sac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/sac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25840 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/sac_decoupled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.526382 sheeprl-0.5.6/sheeprl/algos/sac_ae/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac_ae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24357 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac_ae/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac_ae/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22522 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac_ae/sac_ae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac_ae/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/available_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20399 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.526382 sheeprl-0.5.6/sheeprl/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.530382 sheeprl-0.5.6/sheeprl/configs/algo/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/a2c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3_L.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3_M.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3_S.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3_XL.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3_XS.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/droq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/p2e_dv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/p2e_dv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/p2e_dv3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/ppo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/ppo_decoupled.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/ppo_recurrent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/sac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/sac_ae.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/sac_decoupled.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.530382 sheeprl-0.5.6/sheeprl/configs/buffer/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/buffer/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.530382 sheeprl-0.5.6/sheeprl/configs/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/checkpoint/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.530382 sheeprl-0.5.6/sheeprl/configs/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/distribution/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.534382 sheeprl-0.5.6/sheeprl/configs/env/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/atari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/crafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/diambra.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/dmc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/dummy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/gym.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/minecraft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/minedojo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/minerl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/minerl_obtain_diamond.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/minerl_obtain_iron_pickaxe.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/mujoco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/super_mario_bros.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/eval_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.538382 sheeprl-0.5.6/sheeprl/configs/exp/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/a2c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/a2c_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v1_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2_crafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_100k_boxing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_100k_ms_pacman.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_L_doapp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_L_navigate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_XL_crafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_dmc_cartpole_swingup_sparse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_minedojo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_super_mario_bros.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/droq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv1_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv1_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv2_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv2_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_fntn_L_doapp_64px_gray_combo_discrete_5Mstps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/ppo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/ppo_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/ppo_decoupled.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/ppo_recurrent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/ppo_super_mario_bros.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/sac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/sac_ae.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/sac_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/sac_decoupled.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.538382 sheeprl-0.5.6/sheeprl/configs/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/fabric/ddp-cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/fabric/ddp-cuda.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/fabric/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.538382 sheeprl-0.5.6/sheeprl/configs/hydra/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/hydra/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.542382 sheeprl-0.5.6/sheeprl/configs/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/logger/mlflow.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/logger/tensorboard.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.542382 sheeprl-0.5.6/sheeprl/configs/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/metric/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.542382 sheeprl-0.5.6/sheeprl/configs/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/a2c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/dreamer_v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/dreamer_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/dreamer_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/droq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv1_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv1_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv2_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv2_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv3_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv3_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/ppo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/ppo_recurrent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/sac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/sac_ae.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.542382 sheeprl-0.5.6/sheeprl/configs/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/optim/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/optim/rmsprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/optim/rmsprop_tf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/optim/sgd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.542382 sheeprl-0.5.6/sheeprl/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54229 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/data/buffers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.546382 sheeprl-0.5.6/sheeprl/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/crafter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/diambra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/dmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/minedojo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/minerl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.546382 sheeprl-0.5.6/sheeprl/envs/minerl_envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/minerl_envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/minerl_envs/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/minerl_envs/navigate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/minerl_envs/obtain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/super_mario_bros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.546382 sheeprl-0.5.6/sheeprl/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21610 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.546382 sheeprl-0.5.6/sheeprl/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/optim/rmsprop_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.550382 sheeprl-0.5.6/sheeprl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17999 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.550382 sheeprl-0.5.6/sheeprl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-28 09:23:27.000000 sheeprl-0.5.6/sheeprl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-05-28 09:23:27.000000 sheeprl-0.5.6/sheeprl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:23:27.000000 sheeprl-0.5.6/sheeprl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-28 09:23:27.000000 sheeprl-0.5.6/sheeprl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-28 09:23:27.000000 sheeprl-0.5.6/sheeprl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 09:23:27.000000 sheeprl-0.5.6/sheeprl.egg-info/top_level.txt
```

### Comparing `sheeprl-0.5.5/LICENSE` & `sheeprl-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/PKG-INFO` & `sheeprl-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheeprl
-Version: 0.5.5
+Version: 0.5.6
 Summary: High-quality, single file and distributed implementation of Deep Reinforcement Learning algorithms with production-friendly features
 Author-email: Federico Belotti <federico.belotti@orobix.com>, Davide Angioni <davide.angioni@orobix.com>, Refik Can Malli <refikcan.malli@orobix.com>, Michele Milesi <michele.milesi@orobix.com>
 Maintainer-email: Federico Belotti <federico.belotti@orobix.com>, Davide Angioni <davide.angioni@orobix.com>, Refik Can Malli <refikcan.malli@orobix.com>, Michele Milesi <michele.milesi@orobix.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `sheeprl-0.5.5/README.md` & `sheeprl-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/docs/README.md` & `sheeprl-0.5.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/hydra_plugins/sheeprl_search_path.py` & `sheeprl-0.5.6/hydra_plugins/sheeprl_search_path.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/pyproject.toml` & `sheeprl-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 # -> Level 4# This one isn't too hard to get passing, but return on investment is lower
 no_implicit_reexport = false
 # This one can be tricky to get passing if you use a lot of untyped libraries
 warn_return_any = false
 
 
 [tool.bumpver]
-current_version = "0.5.5"
+current_version = "0.5.6"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "v{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `sheeprl-0.5.5/setup.py` & `sheeprl-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/__init__.py` & `sheeprl-0.5.6/sheeprl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # fmt: on
 
 # Needed because MineRL 0.4.4 is not compatible with the latest version of numpy
 np.float = np.float32
 np.int = np.int64
 np.bool = bool
 
-__version__ = "0.5.5"
+__version__ = "0.5.6"
 
 
 # Replace `moviepy.decorators.use_clip_fps_by_default` method to work with python 3.8, 3.9, and 3.10
 import moviepy.decorators
 
 
 # Taken from https://github.com/Zulko/moviepy/blob/master/moviepy/decorators.py#L118
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/a2c/a2c.py` & `sheeprl-0.5.6/sheeprl/algos/a2c/a2c.py`

 * *Files 5% similar despite different names*

```diff
@@ -196,56 +196,58 @@
 
     # Global variables
     last_log = 0
     last_train = 0
     train_step = 0
     policy_step = 0
     last_checkpoint = 0
-    policy_steps_per_update = int(cfg.env.num_envs * cfg.algo.rollout_steps * world_size)
-    num_updates = cfg.algo.total_steps // policy_steps_per_update if not cfg.dry_run else 1
+    policy_steps_per_iter = int(cfg.env.num_envs * cfg.algo.rollout_steps * world_size)
+    total_iters = cfg.algo.total_steps // policy_steps_per_iter if not cfg.dry_run else 1
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     next_obs = envs.reset(seed=cfg.seed)[0]  # [N_envs, N_obs]
     for k in obs_keys:
         step_data[k] = next_obs[k][np.newaxis]
 
-    for update in range(1, num_updates + 1):
+    for iter_num in range(1, total_iters + 1):
         with torch.inference_mode():
             for _ in range(0, cfg.algo.rollout_steps):
-                policy_step += cfg.env.num_envs * world_size
+                policy_step += policy_steps_per_iter
 
                 # Measure environment interaction time: this considers both the model forward
                 # to get the action given the observation and the time taken into the environment
                 with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                     # Sample an action given the observation received by the environment
                     # This calls the `forward` method of the PyTorch module, escaping from Fabric
                     # because we don't want this to be a synchronization point
-                    torch_obs = prepare_obs(fabric, next_obs, num_envs=cfg.env.num_envs)
+                    torch_obs = prepare_obs(
+                        fabric, next_obs, mlp_keys=cfg.algo.mlp_keys.encoder, num_envs=cfg.env.num_envs
+                    )
                     actions, _, values = player(torch_obs)
                     if is_continuous:
-                        real_actions = torch.cat(actions, -1).cpu().numpy()
+                        real_actions = torch.stack(actions, -1).cpu().numpy()
                     else:
-                        real_actions = torch.cat([act.argmax(dim=-1) for act in actions], axis=-1).cpu().numpy()
+                        real_actions = torch.stack([act.argmax(dim=-1) for act in actions], axis=-1).cpu().numpy()
                     actions = torch.cat(actions, -1).cpu().numpy()
 
                     # Single environment step
                     obs, rewards, terminated, truncated, info = envs.step(real_actions.reshape(envs.action_space.shape))
                     truncated_envs = np.nonzero(truncated)[0]
                     if len(truncated_envs) > 0:
                         real_next_obs = {
@@ -300,15 +302,15 @@
                             fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
 
         # Transform the data into PyTorch Tensors
         local_data = rb.to_tensor(dtype=None, device=device, from_numpy=cfg.buffer.from_numpy)
 
         # Estimate returns with GAE (https://arxiv.org/abs/1506.02438)
         with torch.inference_mode():
-            torch_obs = prepare_obs(fabric, next_obs, num_envs=cfg.env.num_envs)
+            torch_obs = prepare_obs(fabric, next_obs, mlp_keys=cfg.algo.mlp_keys.encoder, num_envs=cfg.env.num_envs)
             next_values = player.get_values(torch_obs)
             returns, advantages = gae(
                 local_data["rewards"].to(torch.float64),
                 local_data["values"],
                 local_data["dones"],
                 next_values,
                 cfg.algo.rollout_steps,
@@ -321,31 +323,31 @@
             local_data["advantages"] = advantages.float()
 
         # Train the agent
         with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
             train(fabric, agent, optimizer, local_data, aggregator, cfg)
 
         # Log metrics
-        if policy_step - last_log >= cfg.metric.log_every or update == num_updates or cfg.dry_run:
+        if policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters or cfg.dry_run:
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
@@ -354,21 +356,21 @@
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint model
         if (
             (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every)
             or cfg.dry_run
-            or (update == num_updates and cfg.checkpoint.save_last)
+            or (iter_num == total_iters and cfg.checkpoint.save_last)
         ):
             last_checkpoint = policy_step
             state = {
                 "agent": agent.state_dict(),
                 "optimizer": optimizer.state_dict(),
-                "update_step": update,
+                "iter_num": iter_num * world_size,
             }
             ckpt_path = os.path.join(log_dir, f"checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt")
             fabric.call("on_checkpoint_coupled", fabric=fabric, ckpt_path=ckpt_path, state=state)
 
     envs.close()
     if fabric.is_global_zero and cfg.algo.run_test:
         test(player, fabric, cfg, log_dir)
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/a2c/agent.py` & `sheeprl-0.5.6/sheeprl/algos/a2c/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/a2c/evaluate.py` & `sheeprl-0.5.6/sheeprl/algos/a2c/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/a2c/loss.py` & `sheeprl-0.5.6/sheeprl/algos/a2c/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/a2c/utils.py` & `sheeprl-0.5.6/sheeprl/algos/a2c/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from __future__ import annotations
 
-from typing import Any, Dict
+from typing import Any, Dict, Sequence
 
 import numpy as np
 import torch
 from lightning import Fabric
 from torch import Tensor
 
 from sheeprl.algos.ppo.agent import PPOPlayer
 from sheeprl.utils.env import make_env
 
 AGGREGATOR_KEYS = {"Rewards/rew_avg", "Game/ep_len_avg", "Loss/value_loss", "Loss/policy_loss"}
 
 
-def prepare_obs(fabric: Fabric, obs: Dict[str, np.ndarray], *, num_envs: int = 1, **kwargs) -> Dict[str, Tensor]:
-    torch_obs = {k: torch.from_numpy(v.copy()).to(fabric.device).float().reshape(num_envs, -1) for k, v in obs.items()}
+def prepare_obs(
+    fabric: Fabric, obs: Dict[str, np.ndarray], *, mlp_keys: Sequence[str] = [], num_envs: int = 1, **kwargs
+) -> Dict[str, Tensor]:
+    torch_obs = {k: torch.from_numpy(obs[k].copy()).to(fabric.device).float().reshape(num_envs, -1) for k in mlp_keys}
     return torch_obs
 
 
 @torch.no_grad()
 def test(agent: PPOPlayer, fabric: Fabric, cfg: Dict[str, Any], log_dir: str):
     env = make_env(cfg, None, 0, log_dir, "test", vector_env_idx=0)()
     agent.eval()
     done = False
     cumulative_rew = 0
     obs = env.reset(seed=cfg.seed)[0]
 
     while not done:
         # Convert observations to tensors
-        torch_obs = prepare_obs(fabric, obs)
+        torch_obs = prepare_obs(fabric, obs, mlp_keys=cfg.algo.mlp_keys.encoder)
 
         # Act greedly through the environment
         actions = agent.get_actions(torch_obs, greedy=True)
         if agent.actor.is_continuous:
             actions = torch.cat(actions, dim=-1)
         else:
             actions = torch.cat([act.argmax(dim=-1) for act in actions], dim=-1)
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v1/agent.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v1/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v1/dreamer_v1.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v1/dreamer_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -492,52 +492,53 @@
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
 
     # Global variables
     train_step = 0
     last_train = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // world_size) + 1
+        (state["iter_num"] // world_size) + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
-    learning_starts = (cfg.algo.learning_starts // policy_steps_per_update) if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs * world_size)
+    total_iters = int(cfg.algo.total_steps // policy_steps_per_iter) if not cfg.dry_run else 1
+    learning_starts = (cfg.algo.learning_starts // policy_steps_per_iter) if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        if not cfg.buffer.checkpoint:
-            learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         if k in cfg.algo.cnn_keys.encoder:
@@ -547,24 +548,24 @@
     step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
     rb.add(step_data, validate_args=cfg.buffer.validate_args)
     player.init_states()
 
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
-        policy_step += cfg.env.num_envs * world_size
+    for iter_num in range(start_iter, total_iters + 1):
+        policy_step += policy_steps_per_iter
 
         with torch.inference_mode():
             # Measure environment interaction time: this considers both the model forward
             # to get the action given the observation and the time taken into the environment
             with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                 # Sample an action given the observation received by the environment
                 if (
-                    update <= learning_starts
+                    iter_num <= learning_starts
                     and cfg.checkpoint.resume_from is None
                     and "minedojo" not in cfg.env.wrapper._target_.lower()
                 ):
                     real_actions = actions = np.array(envs.action_space.sample())
                     if not is_continuous:
                         actions = np.concatenate(
                             [
@@ -577,15 +578,15 @@
                     torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
                     mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                     if len(mask) == 0:
                         mask = None
                     real_actions = actions = player.get_exploration_actions(torch_obs, mask=mask, step=policy_step)
                     actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
                     if is_continuous:
-                        real_actions = torch.cat(real_actions, -1).cpu().numpy()
+                        real_actions = torch.stack(real_actions, -1).cpu().numpy()
                     else:
                         real_actions = (
                             torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                         )
                 next_obs, rewards, terminated, truncated, infos = envs.step(
                     real_actions.reshape(envs.action_space.shape)
                 )
@@ -639,16 +640,17 @@
                 for d in dones_idxes:
                     step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
                     step_data["truncated"][0, d] = np.zeros_like(step_data["truncated"][0, d])
                 # Reset internal agent states
                 player.init_states(reset_envs=dones_idxes)
 
         # Train the agent
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / world_size)
+        if iter_num >= learning_starts:
+            ratio_steps = policy_step - prefill_steps * policy_steps_per_iter
+            per_rank_gradient_steps = ratio(ratio_steps / world_size)
             if per_rank_gradient_steps > 0:
                 with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
                     sample = rb.sample_tensors(
                         batch_size=cfg.algo.per_rank_batch_size,
                         sequence_length=cfg.algo.per_rank_sequence_length,
                         n_samples=per_rank_gradient_steps,
                         dtype=None,
@@ -671,62 +673,62 @@
                         )
                         cumulative_per_rank_gradient_steps += 1
                     train_step += world_size
                 if aggregator:
                     aggregator.update("Params/exploration_amount", actor._get_expl_amount(policy_step))
 
         # Log metrics
-        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Log replay ratio
             fabric.log(
                 "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
             )
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint Model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             state = {
                 "world_model": world_model.state_dict(),
                 "actor": actor.state_dict(),
                 "critic": critic.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "critic_optimizer": critic_optimizer.state_dict(),
                 "ratio": ratio.state_dict(),
-                "update": update * world_size,
+                "iter_num": iter_num * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
                 "on_checkpoint_coupled",
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v1/evaluate.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v1/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v1/loss.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v1/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v1/utils.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v1/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v2/agent.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v2/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v2/dreamer_v2.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v2/dreamer_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,15 +141,19 @@
     # Embed observations from the environment
     embedded_obs = world_model.encoder(batch_obs)
 
     for i in range(0, sequence_length):
         # One step of dynamic learning, which take the posterior state, the recurrent state, the action
         # and the observation and compute the next recurrent, prior and posterior states
         recurrent_state, posterior, _, posterior_logits, prior_logits = world_model.rssm.dynamic(
-            posterior, recurrent_state, data["actions"][i : i + 1], embedded_obs[i : i + 1], data["is_first"][i : i + 1]
+            posterior,
+            recurrent_state,
+            data["actions"][i : i + 1],
+            embedded_obs[i : i + 1],
+            data["is_first"][i : i + 1],
         )
         recurrent_states[i] = recurrent_state
         priors_logits[i] = prior_logits
         posteriors[i] = posterior
         posteriors_logits[i] = posterior_logits
 
     # Concatenate the posteriors with the recurrent states on the last dimension.
@@ -340,15 +344,18 @@
     # Critic optimization step. Eq. 5 from the paper.
     critic_optimizer.zero_grad(set_to_none=True)
     value_loss = -torch.mean(discount[:-1, ..., 0] * qv.log_prob(lambda_values.detach()))
     fabric.backward(value_loss)
     critic_grads = None
     if cfg.algo.critic.clip_gradients is not None and cfg.algo.critic.clip_gradients > 0:
         critic_grads = fabric.clip_gradients(
-            module=critic, optimizer=critic_optimizer, max_norm=cfg.algo.critic.clip_gradients, error_if_nonfinite=False
+            module=critic,
+            optimizer=critic_optimizer,
+            max_norm=cfg.algo.critic.clip_gradients,
+            error_if_nonfinite=False,
         )
     critic_optimizer.step()
 
     # Log metrics
     if aggregator and not aggregator.disabled:
         aggregator.update("Loss/world_model_loss", rec_loss.detach())
         aggregator.update("Loss/observation_loss", observation_loss.detach())
@@ -515,52 +522,53 @@
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
 
     # Global variables
     train_step = 0
     last_train = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // world_size) + 1
+        (state["iter_num"] // world_size) + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    num_updates = cfg.algo.total_steps // policy_steps_per_update if not cfg.dry_run else 1
-    learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs * world_size)
+    total_iters = cfg.algo.total_steps // policy_steps_per_iter if not cfg.dry_run else 1
+    learning_starts = cfg.algo.learning_starts // policy_steps_per_iter if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        if not cfg.buffer.checkpoint:
-            learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         step_data[k] = obs[k][np.newaxis]
@@ -572,24 +580,24 @@
     step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["is_first"] = np.ones_like(step_data["terminated"])
     rb.add(step_data, validate_args=cfg.buffer.validate_args)
     player.init_states()
 
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
-        policy_step += cfg.env.num_envs * world_size
+    for iter_num in range(start_iter, total_iters + 1):
+        policy_step += policy_steps_per_iter
 
         with torch.inference_mode():
             # Measure environment interaction time: this considers both the model forward
             # to get the action given the observation and the time taken into the environment
             with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                 # Sample an action given the observation received by the environment
                 if (
-                    update <= learning_starts
+                    iter_num <= learning_starts
                     and cfg.checkpoint.resume_from is None
                     and "minedojo" not in cfg.env.wrapper._target_.lower()
                 ):
                     real_actions = actions = np.array(envs.action_space.sample())
                     if not is_continuous:
                         actions = np.concatenate(
                             [
@@ -602,18 +610,18 @@
                     torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
                     mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                     if len(mask) == 0:
                         mask = None
                     real_actions = actions = player.get_actions(torch_obs, mask=mask)
                     actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
                     if is_continuous:
-                        real_actions = torch.cat(real_actions, -1).cpu().numpy()
+                        real_actions = torch.stack(real_actions, -1).cpu().numpy()
                     else:
                         real_actions = (
-                            torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
+                            torch.stack([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                         )
 
                 step_data["is_first"] = copy.deepcopy(np.logical_or(step_data["terminated"], step_data["truncated"]))
                 next_obs, rewards, terminated, truncated, infos = envs.step(
                     real_actions.reshape(envs.action_space.shape)
                 )
                 dones = np.logical_or(terminated, truncated).astype(np.uint8)
@@ -667,16 +675,17 @@
                 for d in dones_idxes:
                     step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
                     step_data["truncated"][0, d] = np.zeros_like(step_data["truncated"][0, d])
                 # Reset internal agent states
                 player.init_states(dones_idxes)
 
         # Train the agent
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / world_size)
+        if iter_num >= learning_starts:
+            ratio_steps = policy_step - prefill_steps * policy_steps_per_iter
+            per_rank_gradient_steps = ratio(ratio_steps / world_size)
             if per_rank_gradient_steps > 0:
                 local_data = rb.sample_tensors(
                     batch_size=cfg.algo.per_rank_batch_size,
                     sequence_length=cfg.algo.per_rank_sequence_length,
                     n_samples=per_rank_gradient_steps,
                     dtype=None,
                     device=fabric.device,
@@ -705,63 +714,63 @@
                             cfg,
                             actions_dim,
                         )
                         cumulative_per_rank_gradient_steps += 1
                     train_step += world_size
 
         # Log metrics
-        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Log replay ratio
             fabric.log(
                 "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
             )
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint Model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             state = {
                 "world_model": world_model.state_dict(),
                 "actor": actor.state_dict(),
                 "critic": critic.state_dict(),
                 "target_critic": target_critic.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "critic_optimizer": critic_optimizer.state_dict(),
                 "ratio": ratio.state_dict(),
-                "update": update * world_size,
+                "iter_num": iter_num * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
                 "on_checkpoint_coupled",
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v2/evaluate.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v2/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v2/loss.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v2/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v2/utils.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v2/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,17 +146,17 @@
     while not done:
         # Act greedly through the environment
         torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder)
         real_actions = player.get_actions(
             torch_obs, greedy, {k: v for k, v in torch_obs.items() if k.startswith("mask")}
         )
         if player.actor.is_continuous:
-            real_actions = torch.cat(real_actions, -1).cpu().numpy()
+            real_actions = torch.stack(real_actions, -1).cpu().numpy()
         else:
-            real_actions = torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
+            real_actions = torch.stack([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
 
         # Single environment step
         obs, reward, done, truncated, _ = env.step(real_actions.reshape(env.action_space.shape))
         done = done or truncated or cfg.dry_run
         cumulative_rew += reward
     fabric.print("Test - Reward:", cumulative_rew)
     if cfg.metric.log_level > 0 and len(fabric.loggers) > 0:
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v3/agent.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v3/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -909,15 +909,15 @@
                     mask["mask_craft_smelt"] = mask["mask_craft_smelt"].expand_as(logits)
                     for t in range(functional_action.shape[0]):
                         for b in range(functional_action.shape[1]):
                             sampled_action = functional_action[t, b].item()
                             if sampled_action == 15:  # Craft action
                                 logits[t, b][torch.logical_not(mask["mask_craft_smelt"][t, b])] = -torch.inf
                 elif i == 2:
-                    mask["mask_destroy"][t, b] = mask["mask_destroy"].expand_as(logits)
+                    mask["mask_destroy"] = mask["mask_destroy"].expand_as(logits)
                     mask["mask_equip_place"] = mask["mask_equip_place"].expand_as(logits)
                     for t in range(functional_action.shape[0]):
                         for b in range(functional_action.shape[1]):
                             sampled_action = functional_action[t, b].item()
                             if sampled_action in (16, 17):  # Equip/Place action
                                 logits[t, b][torch.logical_not(mask["mask_equip_place"][t, b])] = -torch.inf
                             elif sampled_action == 18:  # Destroy action
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v3/dreamer_v3.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v3/dreamer_v3.py`

 * *Files 3% similar despite different names*

```diff
@@ -315,15 +315,18 @@
     value_loss = value_loss - qv.log_prob(predicted_target_values.detach())
     value_loss = torch.mean(value_loss * discount[:-1].squeeze(-1))
 
     fabric.backward(value_loss)
     critic_grads = None
     if cfg.algo.critic.clip_gradients is not None and cfg.algo.critic.clip_gradients > 0:
         critic_grads = fabric.clip_gradients(
-            module=critic, optimizer=critic_optimizer, max_norm=cfg.algo.critic.clip_gradients, error_if_nonfinite=False
+            module=critic,
+            optimizer=critic_optimizer,
+            max_norm=cfg.algo.critic.clip_gradients,
+            error_if_nonfinite=False,
         )
     critic_optimizer.step()
 
     # Log metrics
     if aggregator and not aggregator.disabled:
         aggregator.update("Loss/world_model_loss", rec_loss.detach())
         aggregator.update("Loss/observation_loss", observation_loss.detach())
@@ -487,76 +490,77 @@
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {fabric.world_size} processes are instantiated")
 
     # Global variables
     train_step = 0
     last_train = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // fabric.world_size) + 1
+        (state["iter_num"] // fabric.world_size) + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs * fabric.world_size)
-    num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
-    learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs * fabric.world_size)
+    total_iters = int(cfg.algo.total_steps // policy_steps_per_iter) if not cfg.dry_run else 1
+    learning_starts = cfg.algo.learning_starts // policy_steps_per_iter if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // fabric.world_size
-        if not cfg.buffer.checkpoint:
-            learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         step_data[k] = obs[k][np.newaxis]
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["terminated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["is_first"] = np.ones_like(step_data["terminated"])
     player.init_states()
 
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
-        policy_step += cfg.env.num_envs * world_size
+    for iter_num in range(start_iter, total_iters + 1):
+        policy_step += policy_steps_per_iter
 
         with torch.inference_mode():
             # Measure environment interaction time: this considers both the model forward
             # to get the action given the observation and the time taken into the environment
             with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                 # Sample an action given the observation received by the environment
                 if (
-                    update <= learning_starts
+                    iter_num <= learning_starts
                     and cfg.checkpoint.resume_from is None
                     and "minedojo" not in cfg.env.wrapper._target_.lower()
                 ):
                     real_actions = actions = np.array(envs.action_space.sample())
                     if not is_continuous:
                         actions = np.concatenate(
                             [
@@ -569,18 +573,18 @@
                     torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
                     mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                     if len(mask) == 0:
                         mask = None
                     real_actions = actions = player.get_actions(torch_obs, mask=mask)
                     actions = torch.cat(actions, -1).cpu().numpy()
                     if is_continuous:
-                        real_actions = torch.cat(real_actions, dim=-1).cpu().numpy()
+                        real_actions = torch.stack(real_actions, dim=-1).cpu().numpy()
                     else:
                         real_actions = (
-                            torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
+                            torch.stack([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                         )
 
                 step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
                 rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
                 next_obs, rewards, terminated, truncated, infos = envs.step(
                     real_actions.reshape(envs.action_space.shape)
@@ -649,16 +653,17 @@
                 step_data["rewards"][:, dones_idxes] = np.zeros_like(reset_data["rewards"])
                 step_data["terminated"][:, dones_idxes] = np.zeros_like(step_data["terminated"][:, dones_idxes])
                 step_data["truncated"][:, dones_idxes] = np.zeros_like(step_data["truncated"][:, dones_idxes])
                 step_data["is_first"][:, dones_idxes] = np.ones_like(step_data["is_first"][:, dones_idxes])
                 player.init_states(dones_idxes)
 
         # Train the agent
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / world_size)
+        if iter_num >= learning_starts:
+            ratio_steps = policy_step - prefill_steps * policy_steps_per_iter
+            per_rank_gradient_steps = ratio(ratio_steps / world_size)
             if per_rank_gradient_steps > 0:
                 local_data = rb.sample_tensors(
                     cfg.algo.per_rank_batch_size,
                     sequence_length=cfg.algo.per_rank_sequence_length,
                     n_samples=per_rank_gradient_steps,
                     dtype=None,
                     device=fabric.device,
@@ -690,64 +695,64 @@
                             actions_dim,
                             moments,
                         )
                         cumulative_per_rank_gradient_steps += 1
                     train_step += world_size
 
         # Log metrics
-        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Log replay ratio
             fabric.log(
                 "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
             )
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint Model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             state = {
                 "world_model": world_model.state_dict(),
                 "actor": actor.state_dict(),
                 "critic": critic.state_dict(),
                 "target_critic": target_critic.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "critic_optimizer": critic_optimizer.state_dict(),
                 "moments": moments.state_dict(),
                 "ratio": ratio.state_dict(),
-                "update": update * fabric.world_size,
+                "iter_num": iter_num * fabric.world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * fabric.world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
                 "on_checkpoint_coupled",
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v3/evaluate.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v3/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v3/loss.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v3/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/dreamer_v3/utils.py` & `sheeprl-0.5.6/sheeprl/algos/dreamer_v3/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,17 +121,17 @@
     while not done:
         # Act greedly through the environment
         torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder)
         real_actions = player.get_actions(
             torch_obs, greedy, {k: v for k, v in torch_obs.items() if k.startswith("mask")}
         )
         if player.actor.is_continuous:
-            real_actions = torch.cat(real_actions, -1).cpu().numpy()
+            real_actions = torch.stack(real_actions, -1).cpu().numpy()
         else:
-            real_actions = torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
+            real_actions = torch.stack([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
 
         # Single environment step
         obs, reward, done, truncated, _ = env.step(real_actions.reshape(env.action_space.shape))
         done = done or truncated or cfg.dry_run
         cumulative_rew += reward
     fabric.print("Test - Reward:", cumulative_rew)
     if cfg.metric.log_level > 0 and len(fabric.loggers) > 0:
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/droq/agent.py` & `sheeprl-0.5.6/sheeprl/algos/droq/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/droq/droq.py` & `sheeprl-0.5.6/sheeprl/algos/droq/droq.py`

 * *Files 3% similar despite different names*

```diff
@@ -243,72 +243,73 @@
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {fabric.world_size} processes are instantiated")
 
     # Global variables
     last_train = 0
     train_step = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // fabric.world_size) + 1
+        (state["iter_num"] // fabric.world_size) + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs * fabric.world_size)
-    num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
-    learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs * fabric.world_size)
+    total_iters = int(cfg.algo.total_steps // policy_steps_per_iter) if not cfg.dry_run else 1
+    learning_starts = cfg.algo.learning_starts // policy_steps_per_iter if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // fabric.world_size
-        if not cfg.buffer.checkpoint:
-            learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     step_data = {}
     # Get the first environment observation and start the optimization
     obs = envs.reset(seed=cfg.seed)[0]
 
     per_rank_gradient_steps = 0
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
-        policy_step += cfg.env.num_envs * fabric.world_size
+    for iter_num in range(start_iter, total_iters + 1):
+        policy_step += policy_steps_per_iter
 
         # Measure environment interaction time: this considers both the model forward
         # to get the action given the observation and the time taken into the environment
         with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            if update <= learning_starts:
+            if iter_num <= learning_starts:
                 actions = envs.action_space.sample()
             else:
                 with torch.inference_mode():
                     # Sample an action given the observation received by the environment
-                    torch_obs = prepare_obs(fabric, obs, num_envs=cfg.env.num_envs)
+                    torch_obs = prepare_obs(fabric, obs, mlp_keys=cfg.algo.mlp_keys.encoder, num_envs=cfg.env.num_envs)
                     actions = player(torch_obs)
                     actions = actions.cpu().numpy()
             next_obs, rewards, terminated, truncated, infos = envs.step(actions.reshape(envs.action_space.shape))
 
         if cfg.metric.log_level > 0 and "final_info" in infos:
             for i, agent_ep_info in enumerate(infos["final_info"]):
                 if agent_ep_info is not None:
@@ -341,16 +342,17 @@
         step_data["rewards"] = rewards.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
         rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
         # next_obs becomes the new obs
         obs = next_obs
 
         # Train the agent
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / world_size)
+        if iter_num >= learning_starts:
+            ratio_steps = policy_step - prefill_steps * policy_steps_per_iter
+            per_rank_gradient_steps = ratio(ratio_steps / world_size)
             if per_rank_gradient_steps > 0:
                 train(
                     fabric,
                     agent,
                     actor_optimizer,
                     qf_optimizer,
                     alpha_optimizer,
@@ -359,60 +361,60 @@
                     cfg,
                     per_rank_gradient_steps,
                 )
                 train_step += world_size
                 cumulative_per_rank_gradient_steps += per_rank_gradient_steps
 
         # Log metrics
-        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Log replay ratio
             fabric.log(
                 "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
             )
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             state = {
                 "agent": agent.state_dict(),
                 "qf_optimizer": qf_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "alpha_optimizer": alpha_optimizer.state_dict(),
                 "ratio": ratio.state_dict(),
-                "update": update * fabric.world_size,
+                "iter_num": iter_num * fabric.world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * fabric.world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = os.path.join(log_dir, f"checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt")
             fabric.call(
                 "on_checkpoint_coupled",
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/droq/evaluate.py` & `sheeprl-0.5.6/sheeprl/algos/droq/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/droq/utils.py` & `sheeprl-0.5.6/sheeprl/algos/droq/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv1/agent.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv1/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv1/evaluate.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv1/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv1/p2e_dv1_exploration.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv1/p2e_dv1_exploration.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,52 +516,53 @@
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
     step_data = {}
 
     # Global variables
     train_step = 0
     last_train = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // world_size) + 1
+        (state["iter_num"] // world_size) + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
-    learning_starts = (cfg.algo.learning_starts // policy_steps_per_update) if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs * world_size)
+    total_iters = int(cfg.algo.total_steps // policy_steps_per_iter) if not cfg.dry_run else 1
+    learning_starts = (cfg.algo.learning_starts // policy_steps_per_iter) if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        if not cfg.buffer.checkpoint:
-            learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         if k in cfg.algo.cnn_keys.encoder:
@@ -571,24 +572,24 @@
     step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
     rb.add(step_data, validate_args=cfg.buffer.validate_args)
     player.init_states()
 
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
-        policy_step += cfg.env.num_envs * world_size
+    for iter_num in range(start_iter, total_iters + 1):
+        policy_step += policy_steps_per_iter
 
         with torch.inference_mode():
             # Measure environment interaction time: this considers both the model forward
             # to get the action given the observation and the time taken into the environment
             with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                 # Sample an action given the observation received by the environment
                 if (
-                    update <= learning_starts
+                    iter_num <= learning_starts
                     and cfg.checkpoint.resume_from is None
                     and "minedojo" not in cfg.env.wrapper._target_.lower()
                 ):
                     real_actions = actions = np.array(envs.action_space.sample())
                     if not is_continuous:
                         actions = np.concatenate(
                             [
@@ -601,15 +602,15 @@
                     torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
                     mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                     if len(mask) == 0:
                         mask = None
                     real_actions = actions = player.get_exploration_actions(torch_obs, mask=mask, step=policy_step)
                     actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
                     if is_continuous:
-                        real_actions = torch.cat(real_actions, -1).cpu().numpy()
+                        real_actions = torch.stack(real_actions, -1).cpu().numpy()
                     else:
                         real_actions = (
                             torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                         )
                 next_obs, rewards, terminated, truncated, infos = envs.step(
                     real_actions.reshape(envs.action_space.shape)
                 )
@@ -663,16 +664,17 @@
                 for d in dones_idxes:
                     step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
                     step_data["truncated"][0, d] = np.zeros_like(step_data["truncated"][0, d])
                 # Reset internal agent states
                 player.init_states(reset_envs=dones_idxes)
 
         # Train the agent
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / world_size)
+        if iter_num >= learning_starts:
+            ratio_steps = policy_step - prefill_steps * policy_steps_per_iter
+            per_rank_gradient_steps = ratio(ratio_steps / world_size)
             if per_rank_gradient_steps > 0:
                 with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
                     sample = rb.sample_tensors(
                         batch_size=cfg.algo.per_rank_batch_size,
                         sequence_length=cfg.algo.per_rank_sequence_length,
                         n_samples=per_rank_gradient_steps,
                         dtype=None,
@@ -705,64 +707,64 @@
                 if aggregator and not aggregator.disabled:
                     aggregator.update("Params/exploration_amount_task", actor_task._get_expl_amount(policy_step))
                     aggregator.update(
                         "Params/exploration_amount_exploration", actor_exploration._get_expl_amount(policy_step)
                     )
 
         # Log metrics
-        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Log replay ratio
             fabric.log(
                 "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
             )
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint Model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             state = {
                 "world_model": world_model.state_dict(),
                 "actor_task": actor_task.state_dict(),
                 "critic_task": critic_task.state_dict(),
                 "ensembles": ensembles.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_task_optimizer": actor_task_optimizer.state_dict(),
                 "critic_task_optimizer": critic_task_optimizer.state_dict(),
                 "ensemble_optimizer": ensemble_optimizer.state_dict(),
                 "ratio": ratio.state_dict(),
-                "update": update * world_size,
+                "iter_num": iter_num * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "actor_exploration": actor_exploration.state_dict(),
                 "critic_exploration": critic_exploration.state_dict(),
                 "actor_exploration_optimizer": actor_exploration_optimizer.state_dict(),
                 "critic_exploration_optimizer": critic_exploration_optimizer.state_dict(),
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv1/p2e_dv1_finetuning.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv1/p2e_dv1_finetuning.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,52 +187,53 @@
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
 
     # Global variables
     train_step = 0
     last_train = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // world_size) + 1
+        (state["iter_num"] // world_size) + 1
         if resume_from_checkpoint
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if resume_from_checkpoint else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if resume_from_checkpoint else 0
     last_log = state["last_log"] if resume_from_checkpoint else 0
     last_checkpoint = state["last_checkpoint"] if resume_from_checkpoint else 0
-    policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
-    learning_starts = (cfg.algo.learning_starts // policy_steps_per_update) if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs * world_size)
+    total_iters = int(cfg.algo.total_steps // policy_steps_per_iter) if not cfg.dry_run else 1
+    learning_starts = (cfg.algo.learning_starts // policy_steps_per_iter) if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if resume_from_checkpoint:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        if resume_from_checkpoint and not cfg.buffer.checkpoint:
-            learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         if k in cfg.algo.cnn_keys.encoder:
@@ -242,32 +243,32 @@
     step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
     rb.add(step_data, validate_args=cfg.buffer.validate_args)
     player.init_states()
 
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
-        policy_step += cfg.env.num_envs * world_size
+    for iter_num in range(start_iter, total_iters + 1):
+        policy_step += policy_steps_per_iter
 
         with torch.inference_mode():
             # Measure environment interaction time: this considers both the model forward
             # to get the action given the observation and the time taken into the environment
             with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                 torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
                 mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                 if len(mask) == 0:
                     mask = None
                 real_actions = actions = player.get_exploration_actions(torch_obs, mask=mask, step=policy_step)
                 actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
                 if is_continuous:
-                    real_actions = torch.cat(real_actions, -1).cpu().numpy()
+                    real_actions = torch.stack(real_actions, -1).cpu().numpy()
                 else:
                     real_actions = (
-                        torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
+                        torch.stack([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                     )
                 next_obs, rewards, terminated, truncated, infos = envs.step(
                     real_actions.reshape(envs.action_space.shape)
                 )
                 dones = np.logical_or(terminated, truncated).astype(np.uint8)
 
             if cfg.metric.log_level > 0 and "final_info" in infos:
@@ -318,16 +319,17 @@
                 for d in dones_idxes:
                     step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
                     step_data["truncated"][0, d] = np.zeros_like(step_data["truncated"][0, d])
                 # Reset internal agent states
                 player.init_states(reset_envs=dones_idxes)
 
         # Train the agent
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / world_size)
+        if iter_num >= learning_starts:
+            ratio_steps = policy_step - prefill_steps * policy_steps_per_iter
+            per_rank_gradient_steps = ratio(ratio_steps / world_size)
             if per_rank_gradient_steps > 0:
                 if player.actor_type != "task":
                     player.actor_type = "task"
                     player.actor = fabric_player.setup_module(unwrap_fabric(actor_task))
                     for agent_p, p in zip(actor_task.parameters(), player.actor.parameters()):
                         p.data = agent_p.data
                 with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
@@ -358,62 +360,62 @@
                 if aggregator and not aggregator.disabled:
                     aggregator.update("Params/exploration_amount_task", actor_task._get_expl_amount(policy_step))
                     aggregator.update(
                         "Params/exploration_amount_exploration", actor_exploration._get_expl_amount(policy_step)
                     )
 
         # Log metrics
-        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Log replay ratio
             fabric.log(
                 "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
             )
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint Model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             state = {
                 "world_model": world_model.state_dict(),
                 "actor_task": actor_task.state_dict(),
                 "critic_task": critic_task.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_task_optimizer": actor_task_optimizer.state_dict(),
                 "critic_task_optimizer": critic_task_optimizer.state_dict(),
                 "ratio": ratio.state_dict(),
-                "update": update * world_size,
+                "iter_num": iter_num * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "actor_exploration": actor_exploration.state_dict(),
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv1/utils.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv1/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv2/agent.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv2/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv2/evaluate.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv2/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv2/p2e_dv2_exploration.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv2/p2e_dv2_exploration.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,19 @@
     posteriors_logits = torch.empty(sequence_length, batch_size, stochastic_size * discrete_size, device=device)
 
     # embedded observations from the environment
     embedded_obs = world_model.encoder(batch_obs)
 
     for i in range(0, sequence_length):
         recurrent_state, posterior, prior, posterior_logits, prior_logits = world_model.rssm.dynamic(
-            posterior, recurrent_state, data["actions"][i : i + 1], embedded_obs[i : i + 1], data["is_first"][i : i + 1]
+            posterior,
+            recurrent_state,
+            data["actions"][i : i + 1],
+            embedded_obs[i : i + 1],
+            data["is_first"][i : i + 1],
         )
         recurrent_states[i] = recurrent_state
         priors[i] = prior
         priors_logits[i] = prior_logits
         posteriors[i] = posterior
         posteriors_logits[i] = posterior_logits
 
@@ -651,52 +655,53 @@
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
 
     # Global variables
     train_step = 0
     last_train = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // world_size) + 1
+        (state["iter_num"] // world_size) + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    num_updates = cfg.algo.total_steps // policy_steps_per_update if not cfg.dry_run else 1
-    learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs * world_size)
+    total_iters = cfg.algo.total_steps // policy_steps_per_iter if not cfg.dry_run else 1
+    learning_starts = cfg.algo.learning_starts // policy_steps_per_iter if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        if not cfg.buffer.checkpoint:
-            learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         step_data[k] = obs[k][np.newaxis]
@@ -708,24 +713,24 @@
     step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["is_first"] = np.ones_like(step_data["terminated"])
     rb.add(step_data, validate_args=cfg.buffer.validate_args)
     player.init_states()
 
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
-        policy_step += cfg.env.num_envs * world_size
+    for iter_num in range(start_iter, total_iters + 1):
+        policy_step += policy_steps_per_iter
 
         with torch.inference_mode():
             # Measure environment interaction time: this considers both the model forward
             # to get the action given the observation and the time taken into the environment
             with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                 # Sample an action given the observation received by the environment
                 if (
-                    update <= learning_starts
+                    iter_num <= learning_starts
                     and cfg.checkpoint.resume_from is None
                     and "minedojo" not in cfg.env.wrapper._target_.lower()
                 ):
                     real_actions = actions = np.array(envs.action_space.sample())
                     if not is_continuous:
                         actions = np.concatenate(
                             [
@@ -738,18 +743,18 @@
                     torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
                     mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                     if len(mask) == 0:
                         mask = None
                     real_actions = actions = player.get_actions(torch_obs, mask=mask)
                     actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
                     if is_continuous:
-                        real_actions = torch.cat(real_actions, -1).cpu().numpy()
+                        real_actions = torch.stack(real_actions, -1).cpu().numpy()
                     else:
                         real_actions = (
-                            torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
+                            torch.stack([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                         )
 
                 step_data["is_first"] = copy.deepcopy(np.logical_or(step_data["terminated"], step_data["truncated"]))
                 next_obs, rewards, terminated, truncated, infos = envs.step(
                     real_actions.reshape(envs.action_space.shape)
                 )
                 dones = np.logical_or(terminated, truncated).astype(np.uint8)
@@ -803,16 +808,17 @@
                 for d in dones_idxes:
                     step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
                     step_data["truncated"][0, d] = np.zeros_like(step_data["truncated"][0, d])
                 # Reset internal agent states
                 player.init_states(dones_idxes)
 
         # Train the agent
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / world_size)
+        if iter_num >= learning_starts:
+            ratio_steps = policy_step - prefill_steps * policy_steps_per_iter
+            per_rank_gradient_steps = ratio(ratio_steps / world_size)
             if per_rank_gradient_steps > 0:
                 local_data = rb.sample_tensors(
                     batch_size=cfg.algo.per_rank_batch_size,
                     sequence_length=cfg.algo.per_rank_sequence_length,
                     n_samples=per_rank_gradient_steps,
                     dtype=None,
                     device=fabric.device,
@@ -854,65 +860,65 @@
                             is_continuous=is_continuous,
                             actions_dim=actions_dim,
                         )
                         cumulative_per_rank_gradient_steps += 1
                     train_step += world_size
 
         # Log metrics
-        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Log replay ratio
             fabric.log(
                 "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
             )
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint Model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             state = {
                 "world_model": world_model.state_dict(),
                 "actor_task": actor_task.state_dict(),
                 "critic_task": critic_task.state_dict(),
                 "target_critic_task": target_critic_task.state_dict(),
                 "ensembles": ensembles.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_task_optimizer": actor_task_optimizer.state_dict(),
                 "critic_task_optimizer": critic_task_optimizer.state_dict(),
                 "ensemble_optimizer": ensemble_optimizer.state_dict(),
                 "ratio": ratio.state_dict(),
-                "update": update * world_size,
+                "iter_num": iter_num * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "actor_exploration": actor_exploration.state_dict(),
                 "critic_exploration": critic_exploration.state_dict(),
                 "target_critic_exploration": target_critic_exploration.state_dict(),
                 "actor_exploration_optimizer": actor_exploration_optimizer.state_dict(),
                 "critic_exploration_optimizer": critic_exploration_optimizer.state_dict(),
                 "last_log": last_log,
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv2/p2e_dv2_finetuning.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv2/p2e_dv2_finetuning.py`

 * *Files 4% similar despite different names*

```diff
@@ -205,52 +205,53 @@
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
 
     # Global variables
     train_step = 0
     last_train = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // world_size) + 1
+        (state["iter_num"] // world_size) + 1
         if resume_from_checkpoint
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if resume_from_checkpoint else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if resume_from_checkpoint else 0
     last_log = state["last_log"] if resume_from_checkpoint else 0
     last_checkpoint = state["last_checkpoint"] if resume_from_checkpoint else 0
-    policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    num_updates = cfg.algo.total_steps // policy_steps_per_update if not cfg.dry_run else 1
-    learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs * world_size)
+    total_iters = cfg.algo.total_steps // policy_steps_per_iter if not cfg.dry_run else 1
+    learning_starts = cfg.algo.learning_starts // policy_steps_per_iter if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if resume_from_checkpoint:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        if not cfg.buffer.checkpoint:
-            learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         step_data[k] = obs[k][np.newaxis]
@@ -262,32 +263,32 @@
     step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["is_first"] = np.ones_like(step_data["terminated"])
     rb.add(step_data, validate_args=cfg.buffer.validate_args)
     player.init_states()
 
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
-        policy_step += cfg.env.num_envs * world_size
+    for iter_num in range(start_iter, total_iters + 1):
+        policy_step += policy_steps_per_iter
 
         with torch.inference_mode():
             # Measure environment interaction time: this considers both the model forward
             # to get the action given the observation and the time taken into the environment
             with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                 torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
                 mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                 if len(mask) == 0:
                     mask = None
                 real_actions = actions = player.get_actions(torch_obs, mask=mask)
                 actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
                 if is_continuous:
-                    real_actions = torch.cat(real_actions, -1).cpu().numpy()
+                    real_actions = torch.stack(real_actions, -1).cpu().numpy()
                 else:
                     real_actions = (
-                        torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
+                        torch.stack([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                     )
 
                 step_data["is_first"] = copy.deepcopy(np.logical_or(step_data["terminated"], step_data["truncated"]))
                 next_obs, rewards, terminated, truncated, infos = envs.step(
                     real_actions.reshape(envs.action_space.shape)
                 )
                 dones = np.logical_or(terminated, truncated).astype(np.uint8)
@@ -341,16 +342,17 @@
                 for d in dones_idxes:
                     step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
                     step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
                 # Reset internal agent states
                 player.init_states(dones_idxes)
 
         # Train the agent
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / world_size)
+        if iter_num >= learning_starts:
+            ratio_steps = policy_step - prefill_steps * policy_steps_per_iter
+            per_rank_gradient_steps = ratio(ratio_steps / world_size)
             if per_rank_gradient_steps > 0:
                 if player.actor_type != "task":
                     player.actor_type = "task"
                     player.actor = fabric_player.setup_module(unwrap_fabric(actor_task))
                     for agent_p, p in zip(actor_task.parameters(), player.actor.parameters()):
                         p.data = agent_p.data
                 local_data = rb.sample_tensors(
@@ -385,63 +387,63 @@
                             cfg,
                             actions_dim=actions_dim,
                         )
                         cumulative_per_rank_gradient_steps += 1
                     train_step += world_size
 
         # Log metrics
-        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Log replay ratio
             fabric.log(
                 "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
             )
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint Model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             state = {
                 "world_model": world_model.state_dict(),
                 "actor_task": actor_task.state_dict(),
                 "critic_task": critic_task.state_dict(),
                 "target_critic_task": target_critic_task.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_task_optimizer": actor_task_optimizer.state_dict(),
                 "critic_task_optimizer": critic_task_optimizer.state_dict(),
                 "ratio": ratio.state_dict(),
-                "update": update * world_size,
+                "iter_num": iter_num * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "actor_exploration": actor_exploration.state_dict(),
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv2/utils.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv2/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv3/agent.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv3/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv3/evaluate.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv3/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv3/p2e_dv3_exploration.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv3/p2e_dv3_exploration.py`

 * *Files 1% similar despite different names*

```diff
@@ -728,76 +728,77 @@
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
 
     # Global variables
     train_step = 0
     last_train = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // fabric.world_size) + 1
+        (state["iter_num"] // fabric.world_size) + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs * fabric.world_size)
-    num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
-    learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs * fabric.world_size)
+    total_iters = int(cfg.algo.total_steps // policy_steps_per_iter) if not cfg.dry_run else 1
+    learning_starts = cfg.algo.learning_starts // policy_steps_per_iter if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        if not cfg.buffer.checkpoint:
-            learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         step_data[k] = obs[k][np.newaxis]
     step_data["terminated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["is_first"] = np.ones_like(step_data["terminated"])
     player.init_states()
 
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
-        policy_step += cfg.env.num_envs * world_size
+    for iter_num in range(start_iter, total_iters + 1):
+        policy_step += policy_steps_per_iter
 
         with torch.inference_mode():
             # Measure environment interaction time: this considers both the model forward
             # to get the action given the observation and the time taken into the environment
             with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                 # Sample an action given the observation received by the environment
                 if (
-                    update <= learning_starts
+                    iter_num <= learning_starts
                     and cfg.checkpoint.resume_from is None
                     and "minedojo" not in cfg.algo.actor.cls.lower()
                 ):
                     real_actions = actions = np.array(envs.action_space.sample())
                     if not is_continuous:
                         actions = np.concatenate(
                             [
@@ -810,18 +811,18 @@
                     torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
                     mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                     if len(mask) == 0:
                         mask = None
                     real_actions = actions = player.get_actions(torch_obs, mask=mask)
                     actions = torch.cat(actions, -1).cpu().numpy()
                     if is_continuous:
-                        real_actions = torch.cat(real_actions, dim=-1).cpu().numpy()
+                        real_actions = torch.stack(real_actions, dim=-1).cpu().numpy()
                     else:
                         real_actions = (
-                            torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
+                            torch.stack([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                         )
 
                 step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
                 rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
                 next_obs, rewards, terminated, truncated, infos = envs.step(
                     real_actions.reshape(envs.action_space.shape)
@@ -890,16 +891,17 @@
                 step_data["rewards"][:, dones_idxes] = np.zeros_like(reset_data["rewards"])
                 step_data["terminated"][:, dones_idxes] = np.zeros_like(step_data["terminated"][:, dones_idxes])
                 step_data["truncated"][:, dones_idxes] = np.zeros_like(step_data["truncated"][:, dones_idxes])
                 step_data["is_first"][:, dones_idxes] = np.ones_like(step_data["is_first"][:, dones_idxes])
                 player.init_states(dones_idxes)
 
         # Train the agent
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / world_size)
+        if iter_num >= learning_starts:
+            ratio_steps = policy_step - prefill_steps * policy_steps_per_iter
+            per_rank_gradient_steps = ratio(ratio_steps / world_size)
             if per_rank_gradient_steps > 0:
                 local_data = rb.sample_tensors(
                     cfg.algo.per_rank_batch_size,
                     sequence_length=cfg.algo.per_rank_sequence_length,
                     n_samples=per_rank_gradient_steps,
                     dtype=None,
                     device=fabric.device,
@@ -944,51 +946,51 @@
                             moments_exploration=moments_exploration,
                             moments_task=moments_task,
                         )
                         cumulative_per_rank_gradient_steps += 1
                     train_step += world_size
 
         # Log metrics
-        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Log replay ratio
             fabric.log(
                 "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
             )
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint Model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             critics_exploration_state = {"critics_exploration": {}}
             for k, c in critics_exploration.items():
                 critics_exploration_state["critics_exploration"][k] = {
                     "module": c["module"].state_dict(),
                     "target_module": c["target_module"].state_dict(),
@@ -1002,15 +1004,15 @@
                 "target_critic_task": target_critic_task.state_dict(),
                 "ensembles": ensembles.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_task_optimizer": actor_task_optimizer.state_dict(),
                 "critic_task_optimizer": critic_task_optimizer.state_dict(),
                 "ensemble_optimizer": ensemble_optimizer.state_dict(),
                 "ratio": ratio.state_dict(),
-                "update": update * world_size,
+                "iter_num": iter_num * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "actor_exploration": actor_exploration.state_dict(),
                 "actor_exploration_optimizer": actor_exploration_optimizer.state_dict(),
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
                 "moments_task": moments_task.state_dict(),
                 **critics_exploration_state,
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv3/p2e_dv3_finetuning.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv3/p2e_dv3_finetuning.py`

 * *Files 4% similar despite different names*

```diff
@@ -192,84 +192,85 @@
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
 
     # Global variables
     train_step = 0
     last_train = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // fabric.world_size) + 1
+        (state["iter_num"] // fabric.world_size) + 1
         if resume_from_checkpoint
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if resume_from_checkpoint else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if resume_from_checkpoint else 0
     last_log = state["last_log"] if resume_from_checkpoint else 0
     last_checkpoint = state["last_checkpoint"] if resume_from_checkpoint else 0
-    policy_steps_per_update = int(cfg.env.num_envs * fabric.world_size)
-    num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
-    learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs * fabric.world_size)
+    total_iters = int(cfg.algo.total_steps // policy_steps_per_iter) if not cfg.dry_run else 1
+    learning_starts = cfg.algo.learning_starts // policy_steps_per_iter if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if resume_from_checkpoint:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        if not cfg.buffer.checkpoint:
-            learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         step_data[k] = obs[k][np.newaxis]
     step_data["terminated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["is_first"] = np.ones_like(step_data["terminated"])
     player.init_states()
 
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
-        policy_step += cfg.env.num_envs * world_size
+    for iter_num in range(start_iter, total_iters + 1):
+        policy_step += policy_steps_per_iter
 
         with torch.inference_mode():
             # Measure environment interaction time: this considers both the model forward
             # to get the action given the observation and the time taken into the environment
             with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                 torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
                 mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                 if len(mask) == 0:
                     mask = None
                 real_actions = actions = player.get_actions(torch_obs, mask=mask)
                 actions = torch.cat(actions, -1).cpu().numpy()
                 if is_continuous:
-                    real_actions = torch.cat(real_actions, dim=-1).cpu().numpy()
+                    real_actions = torch.stack(real_actions, dim=-1).cpu().numpy()
                 else:
                     real_actions = (
-                        torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
+                        torch.stack([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                     )
 
                 step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
                 rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
                 next_obs, rewards, terminated, truncated, infos = envs.step(
                     real_actions.reshape(envs.action_space.shape)
@@ -338,16 +339,17 @@
                 step_data["rewards"][:, dones_idxes] = np.zeros_like(reset_data["rewards"])
                 step_data["terminated"][:, dones_idxes] = np.zeros_like(step_data["terminated"][:, dones_idxes])
                 step_data["truncated"][:, dones_idxes] = np.zeros_like(step_data["truncated"][:, dones_idxes])
                 step_data["is_first"][:, dones_idxes] = np.ones_like(step_data["is_first"][:, dones_idxes])
                 player.init_states(dones_idxes)
 
         # Train the agent
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / world_size)
+        if iter_num >= learning_starts:
+            ratio_steps = policy_step - prefill_steps * policy_steps_per_iter
+            per_rank_gradient_steps = ratio(ratio_steps / world_size)
             if per_rank_gradient_steps > 0:
                 if player.actor_type != "task":
                     player.actor_type = "task"
                     player.actor = fabric_player.setup_module(unwrap_fabric(actor_task))
                     for agent_p, p in zip(actor_task.parameters(), player.actor.parameters()):
                         p.data = agent_p.data
                 local_data = rb.sample_tensors(
@@ -385,63 +387,63 @@
                             actions_dim=actions_dim,
                             moments=moments_task,
                         )
                         cumulative_per_rank_gradient_steps += 1
                     train_step += world_size
 
         # Log metrics
-        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Log replay ratio
             fabric.log(
                 "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
             )
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint Model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             state = {
                 "world_model": world_model.state_dict(),
                 "actor_task": actor_task.state_dict(),
                 "critic_task": critic_task.state_dict(),
                 "target_critic_task": target_critic_task.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_task_optimizer": actor_task_optimizer.state_dict(),
                 "critic_task_optimizer": critic_task_optimizer.state_dict(),
                 "ratio": ratio.state_dict(),
-                "update": update * world_size,
+                "iter_num": iter_num * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "actor_exploration": actor_exploration.state_dict(),
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
                 "moments_task": moments_task.state_dict(),
             }
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/p2e_dv3/utils.py` & `sheeprl-0.5.6/sheeprl/algos/p2e_dv3/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/ppo/agent.py` & `sheeprl-0.5.6/sheeprl/algos/ppo/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/ppo/evaluate.py` & `sheeprl-0.5.6/sheeprl/algos/ppo/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/ppo/loss.py` & `sheeprl-0.5.6/sheeprl/algos/ppo/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/ppo/ppo.py` & `sheeprl-0.5.6/sheeprl/algos/ppo/ppo.py`

 * *Files 8% similar despite different names*

```diff
@@ -210,79 +210,79 @@
         memmap_dir=os.path.join(log_dir, "memmap_buffer", f"rank_{fabric.global_rank}"),
         obs_keys=obs_keys,
     )
 
     # Global variables
     last_train = 0
     train_step = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // fabric.world_size) + 1
+        (state["iter_num"] // fabric.world_size) + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs * cfg.algo.rollout_steps if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs * cfg.algo.rollout_steps if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs * cfg.algo.rollout_steps * world_size)
-    num_updates = cfg.algo.total_steps // policy_steps_per_update if not cfg.dry_run else 1
+    policy_steps_per_iter = int(cfg.env.num_envs * cfg.algo.rollout_steps * world_size)
+    total_iters = cfg.algo.total_steps // policy_steps_per_iter if not cfg.dry_run else 1
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // fabric.world_size
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Linear learning rate scheduler
     if cfg.algo.anneal_lr:
         from torch.optim.lr_scheduler import PolynomialLR
 
-        scheduler = PolynomialLR(optimizer=optimizer, total_iters=num_updates, power=1.0)
+        scheduler = PolynomialLR(optimizer=optimizer, total_iters=total_iters, power=1.0)
         if cfg.checkpoint.resume_from:
             scheduler.load_state_dict(state["scheduler"])
 
     # Get the first environment observation and start the optimization
     step_data = {}
     next_obs = envs.reset(seed=cfg.seed)[0]  # [N_envs, N_obs]
     for k in obs_keys:
         if k in cfg.algo.cnn_keys.encoder:
             next_obs[k] = next_obs[k].reshape(cfg.env.num_envs, -1, *next_obs[k].shape[-2:])
         step_data[k] = next_obs[k][np.newaxis]
 
-    for update in range(start_step, num_updates + 1):
+    for iter_num in range(start_iter, total_iters + 1):
         with torch.inference_mode():
             for _ in range(0, cfg.algo.rollout_steps):
-                policy_step += cfg.env.num_envs * world_size
+                policy_step += policy_steps_per_iter
 
                 # Measure environment interaction time: this considers both the model forward
                 # to get the action given the observation and the time taken into the environment
                 with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                     # Sample an action given the observation received by the environment
                     torch_obs = prepare_obs(
                         fabric, next_obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs
                     )
                     actions, logprobs, values = player(torch_obs)
                     if is_continuous:
-                        real_actions = torch.cat(actions, -1).cpu().numpy()
+                        real_actions = torch.stack(actions, -1).cpu().numpy()
                     else:
-                        real_actions = torch.cat([act.argmax(dim=-1) for act in actions], dim=-1).cpu().numpy()
+                        real_actions = torch.stack([act.argmax(dim=-1) for act in actions], dim=-1).cpu().numpy()
                     actions = torch.cat(actions, -1).cpu().numpy()
 
                     # Single environment step
                     obs, rewards, terminated, truncated, info = envs.step(real_actions.reshape(envs.action_space.shape))
                     truncated_envs = np.nonzero(truncated)[0]
                     if len(truncated_envs) > 0:
                         real_next_obs = {
@@ -378,31 +378,31 @@
                 fabric.log("Info/learning_rate", scheduler.get_last_lr()[0], policy_step)
             else:
                 fabric.log("Info/learning_rate", cfg.algo.optimizer.lr, policy_step)
             fabric.log("Info/clip_coef", cfg.algo.clip_coef, policy_step)
             fabric.log("Info/ent_coef", cfg.algo.ent_coef, policy_step)
 
             # Log metrics
-            if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+            if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
                 # Sync distributed metrics
                 if aggregator and not aggregator.disabled:
                     metrics_dict = aggregator.compute()
                     fabric.log_dict(metrics_dict, policy_step)
                     aggregator.reset()
 
                 # Sync distributed timers
                 if not timer.disabled:
                     timer_metrics = timer.compute()
-                    if "Time/train_time" in timer_metrics:
+                    if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                         fabric.log(
                             "Time/sps_train",
                             (train_step - last_train) / timer_metrics["Time/train_time"],
                             policy_step,
                         )
-                    if "Time/env_interaction_time" in timer_metrics:
+                    if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                         fabric.log(
                             "Time/sps_env_interaction",
                             ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                             / timer_metrics["Time/env_interaction_time"],
                             policy_step,
                         )
                     timer.reset()
@@ -412,31 +412,31 @@
                 last_train = train_step
 
         # Update lr and coefficients
         if cfg.algo.anneal_lr:
             scheduler.step()
         if cfg.algo.anneal_clip_coef:
             cfg.algo.clip_coef = polynomial_decay(
-                update, initial=initial_clip_coef, final=0.0, max_decay_steps=num_updates, power=1.0
+                iter_num, initial=initial_clip_coef, final=0.0, max_decay_steps=total_iters, power=1.0
             )
         if cfg.algo.anneal_ent_coef:
             cfg.algo.ent_coef = polynomial_decay(
-                update, initial=initial_ent_coef, final=0.0, max_decay_steps=num_updates, power=1.0
+                iter_num, initial=initial_ent_coef, final=0.0, max_decay_steps=total_iters, power=1.0
             )
 
         # Checkpoint model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             state = {
                 "agent": agent.state_dict(),
                 "optimizer": optimizer.state_dict(),
                 "scheduler": scheduler.state_dict() if cfg.algo.anneal_lr else None,
-                "update": update * world_size,
+                "iter_num": iter_num * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * fabric.world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = os.path.join(log_dir, f"checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt")
             fabric.call("on_checkpoint_coupled", fabric=fabric, ckpt_path=ckpt_path, state=state)
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/ppo/ppo_decoupled.py` & `sheeprl-0.5.6/sheeprl/algos/ppo/ppo_decoupled.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,83 +137,82 @@
         cfg.env.num_envs,
         memmap=cfg.buffer.memmap,
         memmap_dir=os.path.join(log_dir, "memmap_buffer", f"rank_{fabric.global_rank}"),
         obs_keys=obs_keys,
     )
 
     # Global variables
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        state["update"] + 1
+        state["iter_num"] + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs * cfg.algo.rollout_steps if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs * cfg.algo.rollout_steps if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs * cfg.algo.rollout_steps)
-    num_updates = cfg.algo.total_steps // policy_steps_per_update if not cfg.dry_run else 1
+    policy_steps_per_iter = int(cfg.env.num_envs * cfg.algo.rollout_steps)
+    total_iters = cfg.algo.total_steps // policy_steps_per_iter if not cfg.dry_run else 1
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if policy_steps_per_update < world_collective.world_size - 1:
+    if policy_steps_per_iter < world_collective.world_size - 1:
         raise RuntimeError(
             "The number of trainers ({}) is greater than the available collected data ({}). ".format(
-                world_collective.world_size - 1, policy_steps_per_update
+                world_collective.world_size - 1, policy_steps_per_iter
             )
             + "Consider to lower the number of trainers at least to the size of available collected data"
         )
     chunks_sizes = [
-        len(chunk)
-        for chunk in torch.tensor_split(torch.arange(policy_steps_per_update), world_collective.world_size - 1)
+        len(chunk) for chunk in torch.tensor_split(torch.arange(policy_steps_per_iter), world_collective.world_size - 1)
     ]
 
-    # Broadcast num_updates to all the world
-    update_t = torch.as_tensor([num_updates], device=device, dtype=torch.float32)
+    # Broadcast total_iters to all the world
+    update_t = torch.as_tensor([total_iters], device=device, dtype=torch.float32)
     world_collective.broadcast(update_t, src=0)
 
     # Get the first environment observation and start the optimization
     step_data = {}
     next_obs = envs.reset(seed=cfg.seed)[0]  # [N_envs, N_obs]
     for k in obs_keys:
         if k in cfg.algo.cnn_keys.encoder:
             next_obs[k] = next_obs[k].reshape(cfg.env.num_envs, -1, *next_obs[k].shape[-2:])
         step_data[k] = next_obs[k][np.newaxis]
 
-    params = {"update": start_step, "last_log": last_log, "last_checkpoint": last_checkpoint}
+    params = {"iter_num": start_iter, "last_log": last_log, "last_checkpoint": last_checkpoint}
     world_collective.scatter_object_list([None], [params] * world_collective.world_size, src=0)
-    for _ in range(start_step, num_updates + 1):
+    for _ in range(start_iter, total_iters + 1):
         for _ in range(0, cfg.algo.rollout_steps):
             policy_step += cfg.env.num_envs
 
             # Measure environment interaction time: this considers both the model forward
             # to get the action given the observation and the time taken into the environment
             with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                 # Sample an action given the observation received by the environment
                 torch_obs = prepare_obs(fabric, next_obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
                 actions, logprobs, values = agent(torch_obs)
                 if is_continuous:
-                    real_actions = torch.cat(actions, -1).cpu().numpy()
+                    real_actions = torch.stack(actions, -1).cpu().numpy()
                 else:
-                    real_actions = torch.cat([act.argmax(dim=-1) for act in actions], dim=-1).cpu().numpy()
+                    real_actions = torch.stack([act.argmax(dim=-1) for act in actions], dim=-1).cpu().numpy()
                 actions = torch.cat(actions, -1).cpu().numpy()
 
                 # Single environment step
                 obs, rewards, terminated, truncated, info = envs.step(real_actions.reshape(envs.action_space.shape))
                 truncated_envs = np.nonzero(truncated)[0]
                 if len(truncated_envs) > 0:
                     real_next_obs = {
@@ -316,19 +315,20 @@
             if aggregator and not aggregator.disabled:
                 fabric.log_dict(aggregator.compute(), policy_step)
                 aggregator.reset()
 
             # Sync timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                fabric.log(
-                    "Time/sps_env_interaction",
-                    ((policy_step - last_log) * cfg.env.action_repeat) / timer_metrics["Time/env_interaction_time"],
-                    policy_step,
-                )
+                if "Time/sps_env_interaction" in timer_metrics and timer_metrics["Time/sps_env_interaction"] > 0:
+                    fabric.log(
+                        "Time/sps_env_interaction",
+                        ((policy_step - last_log) * cfg.env.action_repeat) / timer_metrics["Time/env_interaction_time"],
+                        policy_step,
+                    )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
 
         # Checkpoint model
         if cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every:
@@ -420,41 +420,41 @@
     if global_rank == 1:
         player_trainer_collective.broadcast(
             torch.nn.utils.convert_parameters.parameters_to_vector(agent.parameters()),
             src=1,
         )
 
     # Receive maximum number of updates from the player
-    num_updates = torch.zeros(1, device=device)
-    world_collective.broadcast(num_updates, src=0)
-    num_updates = num_updates.item()
+    total_iters = torch.zeros(1, device=device)
+    world_collective.broadcast(total_iters, src=0)
+    total_iters = total_iters.item()
 
     # Linear learning rate scheduler
     if cfg.algo.anneal_lr:
         from torch.optim.lr_scheduler import PolynomialLR
 
-        scheduler = PolynomialLR(optimizer=optimizer, total_iters=num_updates, power=1.0)
+        scheduler = PolynomialLR(optimizer=optimizer, total_iters=total_iters, power=1.0)
         if cfg.checkpoint.resume_from:
             scheduler.load_state_dict(state["scheduler"])
 
     # Metrics
     aggregator = None
     if not MetricAggregator.disabled:
         aggregator: MetricAggregator = hydra.utils.instantiate(cfg.metric.aggregator, _convert_="all").to(device)
 
     # Start training
     last_train = 0
     train_step = 0
 
-    policy_steps_per_update = cfg.env.num_envs * cfg.algo.rollout_steps
+    policy_steps_per_iter = cfg.env.num_envs * cfg.algo.rollout_steps
     params = [None]
     world_collective.scatter_object_list(params, [None for _ in range(world_collective.world_size)], src=0)
     params = params[0]
-    update = params["update"]
-    policy_step = update * policy_steps_per_update
+    iter_num = params["iter_num"]
+    policy_step = iter_num * policy_steps_per_iter
     last_log = params["last_log"]
     last_checkpoint = params["last_checkpoint"]
     initial_ent_coef = copy.deepcopy(cfg.algo.ent_coef)
     initial_clip_coef = copy.deepcopy(cfg.algo.clip_coef)
     while True:
         # Wait for data
         data = [None]
@@ -463,15 +463,15 @@
         if not isinstance(data, dict) and data == -1:
             # Last Checkpoint
             if cfg.checkpoint.save_last:
                 state = {
                     "agent": agent.state_dict(),
                     "optimizer": optimizer.state_dict(),
                     "scheduler": scheduler.state_dict() if cfg.algo.anneal_lr else None,
-                    "update": update,
+                    "iter_num": iter_num,
                     "batch_size": cfg.algo.per_rank_batch_size * (world_collective.world_size - 1),
                     "last_log": last_log,
                     "last_checkpoint": last_checkpoint,
                 }
                 ckpt_path = cfg.checkpoint.log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
                 fabric.call(
                     "on_checkpoint_trainer",
@@ -559,15 +559,16 @@
             if aggregator and not aggregator.disabled:
                 metrics.update(aggregator.compute())
                 aggregator.reset()
 
             # Sync distributed timers
             if not timer.disabled:
                 timers = timer.compute()
-                metrics.update({"Time/sps_train": (train_step - last_train) / timers["Time/train_time"]})
+                if "Time/train_time" in timers and timers["Time/train_time"] > 0:
+                    metrics.update({"Time/sps_train": (train_step - last_train) / timers["Time/train_time"]})
                 timer.reset()
 
             # Send metrics to the player
             if global_rank == 1:
                 if cfg.algo.anneal_lr:
                     metrics["Info/learning_rate"] = scheduler.get_last_lr()[0]
                 else:
@@ -583,43 +584,43 @@
             last_train = train_step
 
         if cfg.algo.anneal_lr:
             scheduler.step()
 
         if cfg.algo.anneal_clip_coef:
             cfg.algo.clip_coef = polynomial_decay(
-                update, initial=initial_clip_coef, final=0.0, max_decay_steps=num_updates, power=1.0
+                iter_num, initial=initial_clip_coef, final=0.0, max_decay_steps=total_iters, power=1.0
             )
 
         if cfg.algo.anneal_ent_coef:
             cfg.algo.ent_coef = polynomial_decay(
-                update, initial=initial_ent_coef, final=0.0, max_decay_steps=num_updates, power=1.0
+                iter_num, initial=initial_ent_coef, final=0.0, max_decay_steps=total_iters, power=1.0
             )
 
         # Checkpoint model on rank-0: send it everything
         if cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every:
             last_checkpoint = policy_step
             state = {
                 "agent": agent.state_dict(),
                 "optimizer": optimizer.state_dict(),
                 "scheduler": scheduler.state_dict() if cfg.algo.anneal_lr else None,
-                "update": update,
+                "iter_num": iter_num,
                 "batch_size": cfg.algo.per_rank_batch_size * (world_collective.world_size - 1),
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = cfg.checkpoint.log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
                 "on_checkpoint_trainer",
                 fabric=fabric,
                 player_trainer_collective=player_trainer_collective,
                 ckpt_path=ckpt_path,
                 state=state,
             )
-        update += 1
+        iter_num += 1
         policy_step += cfg.env.num_envs * cfg.algo.rollout_steps
 
 
 @register_algorithm(decoupled=True)
 def main(fabric: Fabric, cfg: Dict[str, Any]):
     if fabric.world_size == 1:
         raise RuntimeError(
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/ppo/utils.py` & `sheeprl-0.5.6/sheeprl/algos/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/agent.py` & `sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/evaluate.py` & `sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/ppo_recurrent.py` & `sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/ppo_recurrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,51 +226,51 @@
     # Check that `rollout_steps` = k * `per_rank_sequence_length`
     if cfg.algo.rollout_steps % cfg.algo.per_rank_sequence_length != 0:
         pass
 
     # Global variables
     last_train = 0
     train_step = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // fabric.world_size) + 1
+        (state["iter_num"] // fabric.world_size) + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs * cfg.algo.rollout_steps if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs * cfg.algo.rollout_steps if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs * cfg.algo.rollout_steps * world_size)
-    num_updates = cfg.algo.total_steps // policy_steps_per_update if not cfg.dry_run else 1
+    policy_steps_per_iter = int(cfg.env.num_envs * cfg.algo.rollout_steps * world_size)
+    total_iters = cfg.algo.total_steps // policy_steps_per_iter if not cfg.dry_run else 1
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // fabric.world_size
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Linear learning rate scheduler
     if cfg.algo.anneal_lr:
         from torch.optim.lr_scheduler import PolynomialLR
 
-        scheduler = PolynomialLR(optimizer=optimizer, total_iters=num_updates, power=1.0)
+        scheduler = PolynomialLR(optimizer=optimizer, total_iters=total_iters, power=1.0)
         if cfg.checkpoint.resume_from:
             scheduler.load_state_dict(state["scheduler"])
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]  # [N_envs, N_obs]
     for k in obs_keys:
@@ -280,32 +280,32 @@
         step_data[k] = obs[k]
 
     # Get the resetted recurrent states from the agent
     prev_states = agent.initial_states
     prev_actions = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     torch_prev_actions = torch.zeros(1, cfg.env.num_envs, sum(actions_dim), device=device, dtype=torch.float32)
 
-    for update in range(start_step, num_updates + 1):
+    for iter_num in range(start_iter, total_iters + 1):
         with torch.inference_mode():
             for _ in range(0, cfg.algo.rollout_steps):
-                policy_step += cfg.env.num_envs * world_size
+                policy_step += policy_steps_per_iter
 
                 # Measure environment interaction time: this considers both the model forward
                 # to get the action given the observation and the time taken into the environment
                 with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                     # Sample an action given the observation received by the environment
                     # [Seq_len, Batch_size, D] --> [1, num_envs, D]
                     torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
                     actions, logprobs, values, states = player(
                         torch_obs, prev_actions=torch_prev_actions, prev_states=prev_states
                     )
                     if is_continuous:
-                        real_actions = torch.cat(actions, -1).cpu().numpy()
+                        real_actions = torch.stack(actions, -1).cpu().numpy()
                     else:
-                        real_actions = torch.cat([act.argmax(dim=-1) for act in actions], dim=-1).cpu().numpy()
+                        real_actions = torch.stack([act.argmax(dim=-1) for act in actions], dim=-1).cpu().numpy()
                     torch_actions = torch.cat(actions, dim=-1)
                     actions = torch_actions.cpu().numpy()
 
                     # Single environment step
                     next_obs, rewards, terminated, truncated, info = envs.step(
                         real_actions.reshape(envs.action_space.shape)
                     )
@@ -451,31 +451,31 @@
             fabric.log("Info/learning_rate", scheduler.get_last_lr()[0], policy_step)
         else:
             fabric.log("Info/learning_rate", cfg.algo.optimizer.lr, policy_step)
         fabric.log("Info/clip_coef", cfg.algo.clip_coef, policy_step)
         fabric.log("Info/ent_coef", cfg.algo.ent_coef, policy_step)
 
         # Log metrics
-        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
@@ -485,31 +485,31 @@
             last_train = train_step
 
         # Update lr and coefficients
         if cfg.algo.anneal_lr:
             scheduler.step()
         if cfg.algo.anneal_clip_coef:
             cfg.algo.clip_coef = polynomial_decay(
-                update, initial=initial_clip_coef, final=0.0, max_decay_steps=num_updates, power=1.0
+                iter_num, initial=initial_clip_coef, final=0.0, max_decay_steps=total_iters, power=1.0
             )
         if cfg.algo.anneal_ent_coef:
             cfg.algo.ent_coef = polynomial_decay(
-                update, initial=initial_ent_coef, final=0.0, max_decay_steps=num_updates, power=1.0
+                iter_num, initial=initial_ent_coef, final=0.0, max_decay_steps=total_iters, power=1.0
             )
 
         # Checkpoint model
         if (
             cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every
-        ) or update == num_updates:
+        ) or iter_num == total_iters:
             last_checkpoint = policy_step
             ckpt_state = {
                 "agent": agent.state_dict(),
                 "optimizer": optimizer.state_dict(),
                 "scheduler": scheduler.state_dict() if cfg.algo.anneal_lr else None,
-                "update": update * world_size,
+                "iter_num": iter_num * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * fabric.world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = os.path.join(log_dir, f"checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt")
             fabric.call("on_checkpoint_coupled", fabric=fabric, ckpt_path=ckpt_path, state=ckpt_state)
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/utils.py` & `sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,18 @@
         )
         actions = torch.zeros(1, 1, sum(agent.actions_dim), device=fabric.device)
     while not done:
         torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder)
         # Act greedly through the environment
         actions, state = agent.get_actions(torch_obs, actions, state, greedy=True)
         if agent.actor.is_continuous:
-            real_actions = torch.cat(actions, -1)
+            real_actions = torch.stack(actions, -1)
             actions = torch.cat(actions, dim=-1).view(1, 1, -1)
         else:
-            real_actions = torch.cat([act.argmax(dim=-1) for act in actions], dim=-1)
+            real_actions = torch.stack([act.argmax(dim=-1) for act in actions], dim=-1)
             actions = torch.cat([act for act in actions], dim=-1).view(1, 1, -1)
 
         # Single environment step
         obs, reward, done, truncated, info = env.step(real_actions.cpu().numpy().reshape(env.action_space.shape))
         done = done or truncated
         cumulative_rew += reward
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/sac/agent.py` & `sheeprl-0.5.6/sheeprl/algos/sac/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/sac/evaluate.py` & `sheeprl-0.5.6/sheeprl/algos/sac/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/sac/loss.py` & `sheeprl-0.5.6/sheeprl/algos/sac/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/sac/sac.py` & `sheeprl-0.5.6/sheeprl/algos/sac/sac.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,29 +35,29 @@
     actor_optimizer: Optimizer,
     qf_optimizer: Optimizer,
     alpha_optimizer: Optimizer,
     data: Dict[str, Tensor],
     aggregator: MetricAggregator | None,
     update: int,
     cfg: Dict[str, Any],
-    policy_steps_per_update: int,
+    policy_steps_per_iter: int,
     group: Optional[CollectibleGroup] = None,
 ):
     # Update the soft-critic
     next_target_qf_value = agent.get_next_target_q_values(
         data["next_observations"], data["rewards"], data["terminated"], cfg.algo.gamma
     )
     qf_values = agent.get_q_values(data["observations"], data["actions"])
     qf_loss = critic_loss(qf_values, next_target_qf_value, agent.num_critics)
     qf_optimizer.zero_grad(set_to_none=True)
     fabric.backward(qf_loss)
     qf_optimizer.step()
 
     # Update the target networks with EMA
-    if update % (cfg.algo.critic.target_network_frequency // policy_steps_per_update + 1) == 0:
+    if update % (cfg.algo.critic.target_network_frequency // policy_steps_per_iter + 1) == 0:
         agent.qfs_target_ema()
 
     # Update the actor
     actions, logprobs = agent.get_actions_and_log_probs(data["observations"])
     qf_values = agent.get_q_values(data["observations"], actions)
     min_qf_values = torch.min(qf_values, dim=-1, keepdim=True)[0]
     actor_loss = policy_loss(agent.alpha, logprobs, min_qf_values)
@@ -194,73 +194,73 @@
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {fabric.world_size} processes are instantiated")
 
     # Global variables
     last_train = 0
     train_step = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // fabric.world_size) + 1
+        (state["iter_num"] // fabric.world_size) + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs * fabric.world_size)
-    policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
-    learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs * fabric.world_size)
+    total_iters = int(cfg.algo.total_steps // policy_steps_per_iter) if not cfg.dry_run else 1
+    learning_starts = cfg.algo.learning_starts // policy_steps_per_iter if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // fabric.world_size
-        if not cfg.buffer.checkpoint:
-            learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     step_data = {}
     # Get the first environment observation and start the optimization
     obs = envs.reset(seed=cfg.seed)[0]
 
     per_rank_gradient_steps = 0
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
-        policy_step += cfg.env.num_envs * world_size
+    for iter_num in range(start_iter, total_iters + 1):
+        policy_step += policy_steps_per_iter
 
         # Measure environment interaction time: this considers both the model forward
         # to get the action given the observation and the time taken into the environment
         with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            if update <= learning_starts:
+            if iter_num <= learning_starts:
                 actions = envs.action_space.sample()
             else:
                 # Sample an action given the observation received by the environment
                 with torch.inference_mode():
-                    torch_obs = prepare_obs(fabric, obs, num_envs=cfg.env.num_envs)
+                    torch_obs = prepare_obs(fabric, obs, mlp_keys=cfg.algo.mlp_keys.encoder, num_envs=cfg.env.num_envs)
                     actions = player(torch_obs)
                     actions = actions.cpu().numpy()
             next_obs, rewards, terminated, truncated, infos = envs.step(actions.reshape(envs.action_space.shape))
             rewards = rewards.reshape(cfg.env.num_envs, -1)
 
         if cfg.metric.log_level > 0 and "final_info" in infos:
             for i, agent_ep_info in enumerate(infos["final_info"]):
@@ -292,16 +292,20 @@
         step_data["rewards"] = rewards[np.newaxis]
         rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
         # next_obs becomes the new obs
         obs = next_obs
 
         # Train the agent
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / world_size) if not cfg.run_benchmarks else 1
+        if iter_num >= learning_starts:
+            per_rank_gradient_steps = (
+                ratio((policy_step - prefill_steps + policy_steps_per_iter) / world_size)
+                if not cfg.run_benchmarks
+                else 1
+            )
             if per_rank_gradient_steps > 0:
                 # We sample one time to reduce the communications between processes
                 sample = rb.sample_tensors(
                     batch_size=per_rank_gradient_steps * cfg.algo.per_rank_batch_size,
                     sample_next_obs=cfg.buffer.sample_next_obs,
                     dtype=None,
                     device=device,
@@ -340,68 +344,68 @@
                             fabric,
                             agent,
                             actor_optimizer,
                             qf_optimizer,
                             alpha_optimizer,
                             batch,
                             aggregator,
-                            update,
+                            iter_num,
                             cfg,
-                            policy_steps_per_update,
+                            policy_steps_per_iter,
                         )
                         cumulative_per_rank_gradient_steps += 1
                     train_step += world_size
 
         # Log metrics
-        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Log replay ratio
             fabric.log(
                 "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
             )
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             state = {
                 "agent": agent.state_dict(),
                 "qf_optimizer": qf_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "alpha_optimizer": alpha_optimizer.state_dict(),
                 "ratio": ratio.state_dict(),
-                "update": update * fabric.world_size,
+                "iter_num": iter_num * fabric.world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * fabric.world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = os.path.join(log_dir, f"checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt")
             fabric.call(
                 "on_checkpoint_coupled",
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/sac/sac_decoupled.py` & `sheeprl-0.5.6/sheeprl/algos/sac/sac_decoupled.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,72 +127,74 @@
             raise RuntimeError(
                 "The replay buffer in the configs must be of type "
                 f"`sheeprl.data.buffers.ReplayBuffer`, got {type(state['rb'])}."
             )
 
     # Global variables
     first_info_sent = False
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        state["update"] + 1
+        state["iter_num"] + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs)
-    num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
-    learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs)
+    total_iters = int(cfg.algo.total_steps // policy_steps_per_iter) if not cfg.dry_run else 1
+    learning_starts = cfg.algo.learning_starts // policy_steps_per_iter if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if cfg.checkpoint.resume_from and not cfg.buffer.checkpoint:
-        learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     step_data = {}
     # Get the first environment observation and start the optimization
     obs = envs.reset(seed=cfg.seed)[0]
 
     per_rank_gradient_steps = 0
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
+    for iter_num in range(start_iter, total_iters + 1):
         policy_step += cfg.env.num_envs
 
         # Measure environment interaction time: this considers both the model forward
         # to get the action given the observation and the time taken into the environment
         with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            if update <= learning_starts:
+            if iter_num <= learning_starts:
                 actions = envs.action_space.sample()
             else:
                 # Sample an action given the observation received by the environment
-                torch_obs = prepare_obs(fabric, obs, num_envs=cfg.env.num_envs)
+                torch_obs = prepare_obs(fabric, obs, mlp_keys=cfg.algo.mlp_keys.encoder, num_envs=cfg.env.num_envs)
                 actions = actor(torch_obs)
                 actions = actions.cpu().numpy()
-            next_obs, rewards, terminated, truncated, infos = envs.step(actions)
+            next_obs, rewards, terminated, truncated, infos = envs.step(actions.reshape(envs.action_space.shape))
             rewards = rewards.reshape(cfg.env.num_envs, -1)
 
         if cfg.metric.log_level > 0 and "final_info" in infos:
             for i, agent_ep_info in enumerate(infos["final_info"]):
                 if agent_ep_info is not None:
                     ep_rew = agent_ep_info["episode"]["r"]
                     ep_len = agent_ep_info["episode"]["l"]
@@ -221,22 +223,23 @@
         step_data["rewards"] = rewards[np.newaxis]
         rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
         # next_obs becomes the new obs
         obs = next_obs
 
         # Send data to the training agents
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / (fabric.world_size - 1))
+        if iter_num >= learning_starts:
+            ratio_steps = policy_step - prefill_steps * policy_steps_per_iter
+            per_rank_gradient_steps = ratio(ratio_steps / (fabric.world_size - 1))
             cumulative_per_rank_gradient_steps += per_rank_gradient_steps
             if per_rank_gradient_steps > 0:
                 # Send local info to the trainers
                 if not first_info_sent:
                     world_collective.broadcast_object_list(
-                        [{"update": update, "last_log": last_log, "last_checkpoint": last_checkpoint}], src=0
+                        [{"iter_num": iter_num, "last_log": last_log, "last_checkpoint": last_checkpoint}], src=0
                     )
                     first_info_sent = True
 
                 # Sample data to be sent to the trainers
                 sample = rb.sample_tensors(
                     batch_size=per_rank_gradient_steps * cfg.algo.per_rank_batch_size * (fabric.world_size - 1),
                     sample_next_obs=cfg.buffer.sample_next_obs,
@@ -280,27 +283,28 @@
                 cumulative_per_rank_gradient_steps * (fabric.world_size - 1) / policy_step,
                 policy_step,
             )
 
             # Sync timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                fabric.log(
-                    "Time/sps_env_interaction",
-                    ((policy_step - last_log) * cfg.env.action_repeat) / timer_metrics["Time/env_interaction_time"],
-                    policy_step,
-                )
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
+                    fabric.log(
+                        "Time/sps_env_interaction",
+                        ((policy_step - last_log) * cfg.env.action_repeat) / timer_metrics["Time/env_interaction_time"],
+                        policy_step,
+                    )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
 
         # Checkpoint model
         if (
-            update >= learning_starts  # otherwise the processes end up deadlocked
+            iter_num >= learning_starts  # otherwise the processes end up deadlocked
             and cfg.checkpoint.every > 0
             and policy_step - last_checkpoint >= cfg.checkpoint.every
         ):
             last_checkpoint = policy_step
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
                 "on_checkpoint_player",
@@ -412,42 +416,42 @@
 
     # Metrics
     aggregator = None
     if not MetricAggregator.disabled:
         aggregator: MetricAggregator = hydra.utils.instantiate(cfg.metric.aggregator, _convert_="all").to(device)
 
     # Receive data from player regarding the:
-    # * update
+    # * iter_num
     # * last_log
     # * last_checkpoint
     data = [None]
     world_collective.broadcast_object_list(data, src=0)
-    update = data[0]["update"]
+    iter_num = data[0]["iter_num"]
     last_log = data[0]["last_log"]
     last_checkpoint = data[0]["last_checkpoint"]
 
     # Start training
     train_step = 0
     last_train = 0
-    policy_steps_per_update = cfg.env.num_envs
-    policy_step = update * policy_steps_per_update
+    policy_steps_per_iter = cfg.env.num_envs
+    policy_step = iter_num * policy_steps_per_iter
     while True:
         # Wait for data
         data = [None]
         world_collective.scatter_object_list(data, [None for _ in range(world_collective.world_size)], src=0)
         data = data[0]
         if not isinstance(data, dict) and data == -1:
             # Last Checkpoint
             if cfg.checkpoint.save_last:
                 state = {
                     "agent": agent.state_dict(),
                     "qf_optimizer": qf_optimizer.state_dict(),
                     "actor_optimizer": actor_optimizer.state_dict(),
                     "alpha_optimizer": alpha_optimizer.state_dict(),
-                    "update": update,
+                    "iter_num": iter_num,
                     "batch_size": cfg.algo.per_rank_batch_size * (world_collective.world_size - 1),
                     "last_log": last_log,
                     "last_checkpoint": last_checkpoint,
                 }
                 ckpt_path = cfg.checkpoint.log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
                 fabric.call(
                     "on_checkpoint_trainer",
@@ -474,17 +478,17 @@
                     fabric,
                     agent,
                     actor_optimizer,
                     qf_optimizer,
                     alpha_optimizer,
                     {k: data[k][batch_idxes] for k in data.keys()},
                     aggregator,
-                    update,
+                    iter_num,
                     cfg,
-                    policy_steps_per_update,
+                    policy_steps_per_iter,
                     group=optimization_pg,
                 )
             train_step += group_world_size
 
         if global_rank == 1:
             player_trainer_collective.broadcast(
                 torch.nn.utils.convert_parameters.parameters_to_vector(agent.actor.parameters()), src=1
@@ -496,15 +500,16 @@
             if aggregator and not aggregator.disabled:
                 metrics.update(aggregator.compute())
                 aggregator.reset()
 
             # Sync distributed timers
             if not timer.disabled:
                 timers = timer.compute()
-                metrics.update({"Time/sps_train": (train_step - last_train) / timers["Time/train_time"]})
+                if "Time/train_time" in timers and timers["Time/train_time"] > 0:
+                    metrics.update({"Time/sps_train": (train_step - last_train) / timers["Time/train_time"]})
                 timer.reset()
 
             if global_rank == 1:
                 player_trainer_collective.broadcast_object_list(
                     [metrics], src=1
                 )  # Broadcast metrics: fake send with object list between rank-0 and rank-1
 
@@ -516,31 +521,31 @@
         if cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every:
             last_checkpoint = policy_step
             state = {
                 "agent": agent.state_dict(),
                 "qf_optimizer": qf_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "alpha_optimizer": alpha_optimizer.state_dict(),
-                "update": update,
+                "iter_num": iter_num,
                 "batch_size": cfg.algo.per_rank_batch_size * (world_collective.world_size - 1),
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = cfg.checkpoint.log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
                 "on_checkpoint_trainer",
                 fabric=fabric,
                 player_trainer_collective=player_trainer_collective,
                 ckpt_path=ckpt_path,
                 state=state,
             )
 
         # Update counters
-        update += 1
-        policy_step += policy_steps_per_update
+        iter_num += 1
+        policy_step += policy_steps_per_iter
 
 
 @register_algorithm(decoupled=True)
 def main(fabric: Fabric, cfg: Dict[str, Any]):
     if fabric.world_size == 1:
         raise RuntimeError(
             "Please run the script with the number of devices greater than 1: "
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/sac/utils.py` & `sheeprl-0.5.6/sheeprl/algos/sac/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,30 +24,32 @@
     "Loss/value_loss",
     "Loss/policy_loss",
     "Loss/alpha_loss",
 }
 MODELS_TO_REGISTER = {"agent"}
 
 
-def prepare_obs(fabric: Fabric, obs: Dict[str, np.ndarray], *, num_envs: int = 1, **kwargs) -> Tensor:
+def prepare_obs(
+    fabric: Fabric, obs: Dict[str, np.ndarray], *, mlp_keys: Sequence[str] = [], num_envs: int = 1, **kwargs
+) -> Tensor:
     with fabric.device:
-        torch_obs = torch.cat([torch.as_tensor(obs[k].copy(), dtype=torch.float32) for k in obs.keys()], dim=-1)
+        torch_obs = torch.cat([torch.as_tensor(obs[k].copy(), dtype=torch.float32) for k in mlp_keys], dim=-1)
     return torch_obs.reshape(num_envs, -1)
 
 
 @torch.no_grad()
 def test(actor: SACPlayer, fabric: Fabric, cfg: Dict[str, Any], log_dir: str):
     env = make_env(cfg, None, 0, log_dir, "test", vector_env_idx=0)()
     actor.eval()
     done = False
     cumulative_rew = 0
     obs = env.reset(seed=cfg.seed)[0]
     while not done:
         # Act greedly through the environment
-        torch_obs = prepare_obs(fabric, obs)
+        torch_obs = prepare_obs(fabric, obs, mlp_keys=cfg.algo.mlp_keys.encoder)
         action = actor.get_actions(torch_obs, greedy=True)
 
         # Single environment step
         obs, reward, done, truncated, info = env.step(action.cpu().numpy().reshape(env.action_space.shape))
         done = done or truncated
         cumulative_rew += reward
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/sac_ae/agent.py` & `sheeprl-0.5.6/sheeprl/algos/sac_ae/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/sac_ae/evaluate.py` & `sheeprl-0.5.6/sheeprl/algos/sac_ae/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/algos/sac_ae/sac_ae.py` & `sheeprl-0.5.6/sheeprl/algos/sac_ae/sac_ae.py`

 * *Files 8% similar despite different names*

```diff
@@ -266,70 +266,71 @@
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {fabric.world_size} processes are instantiated")
 
     # Global variables
     last_train = 0
     train_step = 0
-    start_step = (
+    start_iter = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // fabric.world_size) + 1
+        (state["iter_num"] // fabric.world_size) + 1
         if cfg.checkpoint.resume_from
         else 1
     )
-    policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
+    policy_step = state["iter_num"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    policy_steps_per_update = int(cfg.env.num_envs * fabric.world_size)
-    num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
-    learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
+    policy_steps_per_iter = int(cfg.env.num_envs * fabric.world_size)
+    total_iters = int(cfg.algo.total_steps // policy_steps_per_iter) if not cfg.dry_run else 1
+    learning_starts = cfg.algo.learning_starts // policy_steps_per_iter if not cfg.dry_run else 0
+    prefill_steps = learning_starts - int(learning_starts > 0)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // fabric.world_size
-        if not cfg.buffer.checkpoint:
-            learning_starts += start_step
+        learning_starts += start_iter
+        prefill_steps += start_iter
 
     # Create Ratio class
     ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
     if cfg.checkpoint.resume_from:
         ratio.load_state_dict(state["ratio"])
 
     # Warning for log and checkpoint every
-    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
+    if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the metrics will be logged at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
-    if cfg.checkpoint.every % policy_steps_per_update != 0:
+    if cfg.checkpoint.every % policy_steps_per_iter != 0:
         warnings.warn(
             f"The checkpoint.every parameter ({cfg.checkpoint.every}) is not a multiple of the "
-            f"policy_steps_per_update value ({policy_steps_per_update}), so "
+            f"policy_steps_per_iter value ({policy_steps_per_iter}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
-            "policy_steps_per_update value."
+            "policy_steps_per_iter value."
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]  # [N_envs, N_obs]
     for k in obs_keys:
         if k in cfg.algo.cnn_keys.encoder:
             obs[k] = obs[k].reshape(cfg.env.num_envs, -1, *obs[k].shape[-2:])
 
     per_rank_gradient_steps = 0
     cumulative_per_rank_gradient_steps = 0
-    for update in range(start_step, num_updates + 1):
-        policy_step += cfg.env.num_envs * fabric.world_size
+    for iter_num in range(start_iter, total_iters + 1):
+        policy_step += policy_steps_per_iter
 
         # Measure environment interaction time: this considers both the model forward
         # to get the action given the observation and the time taken into the environment
         with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            if update <= learning_starts:
+            if iter_num <= learning_starts:
                 actions = envs.action_space.sample()
             else:
                 with torch.inference_mode():
                     torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
                     actions = player(torch_obs).cpu().numpy()
             next_obs, rewards, terminated, truncated, infos = envs.step(actions.reshape(envs.action_space.shape))
 
@@ -369,16 +370,17 @@
         step_data["rewards"] = rewards.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
         rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
         # next_obs becomes the new obs
         obs = next_obs
 
         # Train the agent
-        if update >= learning_starts:
-            per_rank_gradient_steps = ratio(policy_step / world_size)
+        if iter_num >= learning_starts:
+            ratio_steps = policy_step - prefill_steps * policy_steps_per_iter
+            per_rank_gradient_steps = ratio(ratio_steps / world_size)
             if per_rank_gradient_steps > 0:
                 # We sample one time to reduce the communications between processes
                 sample = rb.sample_tensors(
                     per_rank_gradient_steps * cfg.algo.per_rank_batch_size,
                     sample_next_obs=cfg.buffer.sample_next_obs,
                     from_numpy=cfg.buffer.from_numpy,
                 )  # [1, G*B]
@@ -421,64 +423,64 @@
                             cumulative_per_rank_gradient_steps,
                             cfg,
                         )
                         cumulative_per_rank_gradient_steps += 1
                     train_step += world_size
 
         # Log metrics
-        if cfg.metric.log_level and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
+        if cfg.metric.log_level and (policy_step - last_log >= cfg.metric.log_every or iter_num == total_iters):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
             # Log replay ratio
             fabric.log(
                 "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
             )
 
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
-                if "Time/train_time" in timer_metrics:
+                if "Time/train_time" in timer_metrics and timer_metrics["Time/train_time"] > 0:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
                         policy_step,
                     )
-                if "Time/env_interaction_time" in timer_metrics:
+                if "Time/env_interaction_time" in timer_metrics and timer_metrics["Time/env_interaction_time"] > 0:
                     fabric.log(
                         "Time/sps_env_interaction",
                         ((policy_step - last_log) / world_size * cfg.env.action_repeat)
                         / timer_metrics["Time/env_interaction_time"],
                         policy_step,
                     )
                 timer.reset()
 
             # Reset counters
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint model
         if (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every) or (
-            update == num_updates and cfg.checkpoint.save_last
+            iter_num == total_iters and cfg.checkpoint.save_last
         ):
             last_checkpoint = policy_step
             state = {
                 "agent": agent.state_dict(),
                 "encoder": encoder.state_dict(),
                 "decoder": decoder.state_dict(),
                 "qf_optimizer": qf_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "alpha_optimizer": alpha_optimizer.state_dict(),
                 "encoder_optimizer": encoder_optimizer.state_dict(),
                 "decoder_optimizer": decoder_optimizer.state_dict(),
                 "ratio": ratio.state_dict(),
-                "update": update * fabric.world_size,
+                "iter_num": iter_num * fabric.world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * fabric.world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = os.path.join(log_dir, f"checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt")
             fabric.call(
                 "on_checkpoint_coupled",
```

### Comparing `sheeprl-0.5.5/sheeprl/algos/sac_ae/utils.py` & `sheeprl-0.5.6/sheeprl/algos/sac_ae/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/available_agents.py` & `sheeprl-0.5.6/sheeprl/available_agents.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/cli.py` & `sheeprl-0.5.6/sheeprl/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,27 @@
         )
     if old_cfg.algo.name != cfg.algo.name:
         raise ValueError(
             "This experiment is run with a different algorithm from the one of the experiment you want to restart. "
             f"Got '{cfg.algo.name}', but the algorithm of the experiment of the checkpoint was {old_cfg.algo.name}. "
             "Set properly the algorithm name for restarting the experiment."
         )
+    if old_cfg.algo.learning_starts > 0:
+        warnings.warn(
+            "The `algo.learning_starts` parameter is greater than zero. "
+            "This means that the resuming experiment will pre-fill the buffer for `algo.learning_starts` steps. "
+            "If this is not intended please set the `algo.learning_starts=0` parameter in the experiment configuration "
+            "or through the CLI."
+        )
 
     # Remove keys from the `old_cfg` that must not be overridden
     old_cfg.pop("root_dir", None)
     old_cfg.pop("run_name", None)
     old_cfg.checkpoint.pop("resume_from", None)
+    old_cfg.algo.pop("learning_starts", None)
     # Substitute the config with the old one (except for the parameters removed before)
     # because the experiment must continue with the same parameters
     with open_dict(cfg):
         cfg.merge_with(old_cfg.as_dict())
     return cfg
 
 
@@ -325,14 +333,19 @@
         warnings.warn(
             "MLFlow is not installed. "
             "Please install it with 'pip install mlflow' if you want to use the MLFlow logger and log models. "
             "Setting `cfg.model_manager.disabled=True`",
             UserWarning,
         )
         cfg.model_manager.disabled = True
+    if cfg.algo.learning_starts is not None and cfg.algo.learning_starts < 0:
+        raise ValueError("The `algo.learning_starts` parameter must be greater or equal to zero.")
+
+    if cfg.env.action_repeat < 1:
+        cfg.env.action_repeat = 1
 
 
 def check_configs_evaluation(cfg: DictConfig):
     if cfg.float32_matmul_precision not in {"medium", "high", "highest"}:
         raise ValueError(
             f"Invalid value '{cfg.float32_matmul_precision}' for the 'float32_matmul_precision' parameter. "
             "It must be one of 'medium', 'high' or 'highest'."
```

### Comparing `sheeprl-0.5.5/sheeprl/configs/algo/a2c.yaml` & `sheeprl-0.5.6/sheeprl/configs/algo/a2c.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v1.yaml` & `sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v1.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v2.yaml` & `sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v2.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3.yaml` & `sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/algo/p2e_dv1.yaml` & `sheeprl-0.5.6/sheeprl/configs/algo/p2e_dv1.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/algo/p2e_dv2.yaml` & `sheeprl-0.5.6/sheeprl/configs/algo/p2e_dv2.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/algo/p2e_dv3.yaml` & `sheeprl-0.5.6/sheeprl/configs/algo/p2e_dv3.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/algo/ppo.yaml` & `sheeprl-0.5.6/sheeprl/configs/algo/ppo.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/algo/ppo_recurrent.yaml` & `sheeprl-0.5.6/sheeprl/configs/algo/ppo_recurrent.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/algo/sac.yaml` & `sheeprl-0.5.6/sheeprl/configs/algo/sac.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/algo/sac_ae.yaml` & `sheeprl-0.5.6/sheeprl/configs/algo/sac_ae.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/config.yaml` & `sheeprl-0.5.6/sheeprl/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/env/atari.yaml` & `sheeprl-0.5.6/sheeprl/configs/env/atari.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/env/diambra.yaml` & `sheeprl-0.5.6/sheeprl/configs/env/diambra.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/env/minerl.yaml` & `sheeprl-0.5.6/sheeprl/configs/env/minerl.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/a2c.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/a2c.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/a2c_benchmarks.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/a2c_benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v1.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v1.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Checkpoint
 checkpoint:
   every: 100000
 
 # Buffer
 buffer:
   size: 5000000
-  checkpoint: False
+  checkpoint: True
 
 # Distribution
 distribution:
   type: "auto"
 
 metric:
   aggregator:
```

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v1_benchmarks.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v1_benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 checkpoint:
   every: 100000
 
 # Buffer
 buffer:
   size: 5000000
   type: sequential
-  checkpoint: False
+  checkpoint: True
   prioritize_ends: False
 
 # Distribution
 distribution:
   type: "auto"
 
 metric:
```

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2_benchmarks.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2_benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2_crafter.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2_crafter.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # Checkpoint
 checkpoint:
   every: 100000
 
 # Buffer
 buffer:
   size: 1000000
-  checkpoint: False
+  checkpoint: True
 
 # Distribution
 distribution:
   type: "auto"
 
 metric:
   aggregator:
```

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_L_doapp.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_L_doapp.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_L_navigate.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_L_navigate.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_benchmarks.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_dmc_cartpole_swingup_sparse.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_dmc_cartpole_swingup_sparse.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv1_exploration.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv1_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv1_finetuning.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv1_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv2_exploration.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv2_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv2_finetuning.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv2_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_exploration.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_finetuning.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_fntn_L_doapp_64px_gray_combo_discrete_5Mstps.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_fntn_L_doapp_64px_gray_combo_discrete_5Mstps.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/ppo.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/ppo.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/ppo_benchmarks.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/ppo_benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/ppo_super_mario_bros.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/ppo_super_mario_bros.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/sac.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/sac.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Checkpoint
 checkpoint:
   every: 50000
 
 # Buffer
 buffer:
   size: 1000000
-  checkpoint: False
+  checkpoint: True
   sample_next_obs: False
 
 # Environment
 env:
   id: LunarLanderContinuous-v2
 
 metric:
```

### Comparing `sheeprl-0.5.5/sheeprl/configs/exp/sac_benchmarks.yaml` & `sheeprl-0.5.6/sheeprl/configs/exp/sac_benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/metric/default.yaml` & `sheeprl-0.5.6/sheeprl/configs/metric/default.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/model_manager/dreamer_v2.yaml` & `sheeprl-0.5.6/sheeprl/configs/model_manager/dreamer_v2.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/model_manager/dreamer_v3.yaml` & `sheeprl-0.5.6/sheeprl/configs/model_manager/dreamer_v3.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv1_exploration.yaml` & `sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv1_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv2_exploration.yaml` & `sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv2_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv2_finetuning.yaml` & `sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv2_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv3_exploration.yaml` & `sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv3_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv3_finetuning.yaml` & `sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv3_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/data/buffers.py` & `sheeprl-0.5.6/sheeprl/data/buffers.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/envs/crafter.py` & `sheeprl-0.5.6/sheeprl/envs/crafter.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/envs/diambra.py` & `sheeprl-0.5.6/sheeprl/envs/diambra.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/envs/dmc.py` & `sheeprl-0.5.6/sheeprl/envs/dmc.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/envs/dummy.py` & `sheeprl-0.5.6/sheeprl/envs/dummy.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/envs/minedojo.py` & `sheeprl-0.5.6/sheeprl/envs/minedojo.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     raise ModuleNotFoundError(_IS_MINEDOJO_AVAILABLE)
 
 import copy
 from typing import Any, Dict, Optional, SupportsFloat, Tuple
 
 import gymnasium as gym
 import minedojo
+import minedojo.tasks
 import numpy as np
 from gymnasium.core import RenderFrame
 from minedojo.sim import ALL_CRAFT_SMELT_ITEMS, ALL_ITEMS
 from minedojo.sim.wrappers.ar_nn import ARNNWrapper
 
 N_ALL_ITEMS = len(ALL_ITEMS)
 ACTION_MAP = {
@@ -35,14 +36,15 @@
     15: np.array([0, 0, 0, 12, 12, 4, 0, 0]),  # craft
     16: np.array([0, 0, 0, 12, 12, 5, 0, 0]),  # equip
     17: np.array([0, 0, 0, 12, 12, 6, 0, 0]),  # place
     18: np.array([0, 0, 0, 12, 12, 7, 0, 0]),  # destroy
 }
 ITEM_ID_TO_NAME = dict(enumerate(ALL_ITEMS))
 ITEM_NAME_TO_ID = dict(zip(ALL_ITEMS, range(N_ALL_ITEMS)))
+ALL_TASKS_SPECS = copy.deepcopy(minedojo.tasks.ALL_TASKS_SPECS)
 
 # Minedojo functional actions:
 # 0: noop
 # 1: use
 # 2: drop
 # 3: attack
 # 4: craft
@@ -63,15 +65,15 @@
         sticky_jump: Optional[int] = 10,
         **kwargs: Optional[Dict[Any, Any]],
     ):
         self._height = height
         self._width = width
         self._pitch_limits = pitch_limits
         self._pos = kwargs.get("start_position", None)
-        self._break_speed_multiplier = kwargs.get("break_speed_multiplier", 100)
+        self._break_speed_multiplier = kwargs.pop("break_speed_multiplier", 100)
         self._start_pos = copy.deepcopy(self._pos)
         self._sticky_attack = 0 if self._break_speed_multiplier > 1 else sticky_attack
         self._sticky_jump = sticky_jump
         self._sticky_attack_counter = 0
         self._sticky_jump_counter = 0
 
         if self._pos is not None and not (self._pitch_limits[0] <= self._pos["pitch"] <= self._pitch_limits[1]):
@@ -80,14 +82,15 @@
             )
 
         env: ARNNWrapper = minedojo.make(
             task_id=id,
             image_size=(height, width),
             world_seed=seed,
             fast_reset=True,
+            break_speed_multiplier=self._break_speed_multiplier,
             **kwargs,
         )
         super().__init__(env)
         self._inventory = {}
         self._inventory_names = None
         self._inventory_max = np.zeros(N_ALL_ITEMS)
         self.action_space = gym.spaces.MultiDiscrete(
@@ -105,14 +108,15 @@
                 "mask_equip_place": gym.spaces.Box(0, 1, (N_ALL_ITEMS,), bool),
                 "mask_destroy": gym.spaces.Box(0, 1, (N_ALL_ITEMS,), bool),
                 "mask_craft_smelt": gym.spaces.Box(0, 1, (len(ALL_CRAFT_SMELT_ITEMS),), bool),
             }
         )
         self._render_mode: str = "rgb_array"
         self.seed(seed=seed)
+        minedojo.tasks.ALL_TASKS_SPECS = copy.deepcopy(ALL_TASKS_SPECS)
 
     @property
     def render_mode(self) -> str | None:
         return self._render_mode
 
     def __getattr__(self, name):
         return getattr(self.env, name)
```

### Comparing `sheeprl-0.5.5/sheeprl/envs/minerl.py` & `sheeprl-0.5.6/sheeprl/envs/minerl.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/envs/minerl_envs/backend.py` & `sheeprl-0.5.6/sheeprl/envs/minerl_envs/backend.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/envs/minerl_envs/navigate.py` & `sheeprl-0.5.6/sheeprl/envs/minerl_envs/navigate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/envs/minerl_envs/obtain.py` & `sheeprl-0.5.6/sheeprl/envs/minerl_envs/obtain.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/envs/super_mario_bros.py` & `sheeprl-0.5.6/sheeprl/envs/super_mario_bros.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/models/models.py` & `sheeprl-0.5.6/sheeprl/models/models.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/optim/rmsprop_tf.py` & `sheeprl-0.5.6/sheeprl/optim/rmsprop_tf.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/utils/callback.py` & `sheeprl-0.5.6/sheeprl/utils/callback.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/utils/distribution.py` & `sheeprl-0.5.6/sheeprl/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/utils/env.py` & `sheeprl-0.5.6/sheeprl/utils/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import cv2
 import gymnasium as gym
 import hydra
 import numpy as np
 
 from sheeprl.envs.wrappers import (
     ActionRepeat,
+    ActionsAsObservationWrapper,
     FrameStack,
     GrayscaleRenderWrapper,
     MaskVelocityWrapper,
     RewardAsObservationWrapper,
 )
 from sheeprl.utils.imports import _IS_DIAMBRA_ARENA_AVAILABLE, _IS_DIAMBRA_AVAILABLE, _IS_DMC_AVAILABLE
 
@@ -203,14 +204,17 @@
         if cnn_keys is not None and len(cnn_keys) > 0 and cfg.env.frame_stack > 1:
             if cfg.env.frame_stack_dilation <= 0:
                 raise ValueError(
                     f"The frame stack dilation argument must be greater than zero, got: {cfg.env.frame_stack_dilation}"
                 )
             env = FrameStack(env, cfg.env.frame_stack, cnn_keys, cfg.env.frame_stack_dilation)
 
+        if cfg.env.actions_as_observation.num_stack > 0 and "diambra" not in cfg.env.wrapper._target_:
+            env = ActionsAsObservationWrapper(env, **cfg.env.actions_as_observation)
+
         if cfg.env.reward_as_observation:
             env = RewardAsObservationWrapper(env)
 
         env.action_space.seed(seed)
         env.observation_space.seed(seed)
         if cfg.env.max_episode_steps and cfg.env.max_episode_steps > 0:
             env = gym.wrappers.TimeLimit(env, max_episode_steps=cfg.env.max_episode_steps)
```

### Comparing `sheeprl-0.5.5/sheeprl/utils/fabric.py` & `sheeprl-0.5.6/sheeprl/utils/fabric.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/utils/imports.py` & `sheeprl-0.5.6/sheeprl/utils/imports.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/utils/logger.py` & `sheeprl-0.5.6/sheeprl/utils/logger.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/utils/memmap.py` & `sheeprl-0.5.6/sheeprl/utils/memmap.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/utils/metric.py` & `sheeprl-0.5.6/sheeprl/utils/metric.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/utils/mlflow.py` & `sheeprl-0.5.6/sheeprl/utils/mlflow.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/utils/model.py` & `sheeprl-0.5.6/sheeprl/utils/model.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/utils/registry.py` & `sheeprl-0.5.6/sheeprl/utils/registry.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/utils/timer.py` & `sheeprl-0.5.6/sheeprl/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.5/sheeprl/utils/utils.py` & `sheeprl-0.5.6/sheeprl/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         self._prev = None
 
     def __call__(self, step: int) -> int:
         if self._ratio == 0:
             return 0
         if self._prev is None:
             self._prev = step
-            repeats = 1
+            repeats = int(step * self._ratio)
             if self._pretrain_steps > 0:
                 if step < self._pretrain_steps:
                     warnings.warn(
                         "The number of pretrain steps is greater than the number of current steps. This could lead to "
                         f"a higher ratio than the one specified ({self._ratio}). Setting the 'pretrain_steps' equal to "
                         "the number of current steps."
                     )
```

### Comparing `sheeprl-0.5.5/sheeprl.egg-info/PKG-INFO` & `sheeprl-0.5.6/sheeprl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheeprl
-Version: 0.5.5
+Version: 0.5.6
 Summary: High-quality, single file and distributed implementation of Deep Reinforcement Learning algorithms with production-friendly features
 Author-email: Federico Belotti <federico.belotti@orobix.com>, Davide Angioni <davide.angioni@orobix.com>, Refik Can Malli <refikcan.malli@orobix.com>, Michele Milesi <michele.milesi@orobix.com>
 Maintainer-email: Federico Belotti <federico.belotti@orobix.com>, Davide Angioni <davide.angioni@orobix.com>, Refik Can Malli <refikcan.malli@orobix.com>, Michele Milesi <michele.milesi@orobix.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `sheeprl-0.5.5/sheeprl.egg-info/SOURCES.txt` & `sheeprl-0.5.6/sheeprl.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -144,14 +144,15 @@
 sheeprl/configs/exp/dreamer_v3_L_doapp.yaml
 sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml
 sheeprl/configs/exp/dreamer_v3_L_navigate.yaml
 sheeprl/configs/exp/dreamer_v3_XL_crafter.yaml
 sheeprl/configs/exp/dreamer_v3_benchmarks.yaml
 sheeprl/configs/exp/dreamer_v3_dmc_cartpole_swingup_sparse.yaml
 sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml
+sheeprl/configs/exp/dreamer_v3_minedojo.yaml
 sheeprl/configs/exp/dreamer_v3_super_mario_bros.yaml
 sheeprl/configs/exp/droq.yaml
 sheeprl/configs/exp/p2e_dv1_exploration.yaml
 sheeprl/configs/exp/p2e_dv1_finetuning.yaml
 sheeprl/configs/exp/p2e_dv2_exploration.yaml
 sheeprl/configs/exp/p2e_dv2_finetuning.yaml
 sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml
```

### Comparing `sheeprl-0.5.5/sheeprl.egg-info/requires.txt` & `sheeprl-0.5.6/sheeprl.egg-info/requires.txt`

 * *Files identical despite different names*

